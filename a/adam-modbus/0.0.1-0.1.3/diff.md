# Comparing `tmp/adam_modbus-0.0.1.tar.gz` & `tmp/adam_modbus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam_modbus-0.0.1.tar", max compression
+gzip compressed data, was "adam_modbus-0.1.3.tar", max compression
```

## Comparing `adam_modbus-0.0.1.tar` & `adam_modbus-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2023-08-07 19:07:49.932809 adam_modbus-0.0.1/LICENSE
--rw-r--r--   0        0        0       86 2023-08-07 19:07:49.932809 adam_modbus-0.0.1/README.md
--rw-r--r--   0        0        0       22 2023-08-07 19:07:49.932809 adam_modbus-0.0.1/adam_modbus/__init__.py
--rw-r--r--   0        0        0     2806 2023-08-07 19:07:49.932809 adam_modbus-0.0.1/adam_modbus/interface.py
--rw-r--r--   0        0        0      769 2023-08-07 19:07:49.936810 adam_modbus-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 adam_modbus-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-07 20:21:15.706056 adam_modbus-0.1.3/LICENSE
+-rw-r--r--   0        0        0       86 2023-08-07 20:21:15.706056 adam_modbus-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-08-07 20:21:16.854177 adam_modbus-0.1.3/adam_modbus/__init__.py
+-rw-r--r--   0        0        0     3555 2023-08-07 20:21:15.706056 adam_modbus-0.1.3/adam_modbus/interface.py
+-rw-r--r--   0        0        0      724 2023-08-07 20:21:16.846176 adam_modbus-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 adam_modbus-0.1.3/PKG-INFO
```

### Comparing `adam_modbus-0.0.1/LICENSE` & `adam_modbus-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adam_modbus-0.0.1/adam_modbus/interface.py` & `adam_modbus-0.1.3/adam_modbus/interface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,123 @@
 import asyncio
 import socket
 from collections.abc import AsyncIterator
 from contextlib import asynccontextmanager
-from typing import Literal, assert_never
+from dataclasses import dataclass
+from typing import Literal
 
 
 class AdamConnectionError(RuntimeError):
     pass
 
 
-ADAM_PORT = 1025
+DEFAULT_ADAM_PORT = 1025
 ADAM_CONNECTION_TIMEOUT = 0.1
 
 
-@asynccontextmanager
-async def adam_socket_context(
-    ip: str,
-) -> AsyncIterator[socket.socket]:
-    adam_sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-
-    loop = asyncio.get_running_loop()
-
-    # according to chatgpt, asyncio does not support timeouts on UDP sockets
-    # so we manually do this with asyncio.wait_for, otherwise it will hang forever
-    adam_sock.setblocking(False)
-
-    try:
-        await loop.sock_connect(adam_sock, (ip, ADAM_PORT))
-        yield adam_sock
-
-    # TODO: are these right now that this is async?
-    except (TimeoutError, OSError, asyncio.TimeoutError):
-        raise AdamConnectionError(f"Could not connect to ADAM at {ip}")
-
-    finally:
-        adam_sock.close()
-
+@dataclass
+class AdamConnection:
+    socket: socket.socket
+    ip: str
+    port: int
+    timeout: float = ADAM_CONNECTION_TIMEOUT
+    model: str | None = None
 
-async def _adam_send_and_receive(message: str, ip: str) -> str:
-    async with adam_socket_context(ip) as adam_socket:
+    async def _send_and_receive(self, message: str) -> str:
         loop = asyncio.get_running_loop()
 
-        await asyncio.wait_for(
-            loop.sock_sendall(adam_socket, message.encode("ascii")),
-            ADAM_CONNECTION_TIMEOUT,
-        )
-        adam_out = await asyncio.wait_for(
-            loop.sock_recv(adam_socket, 100), ADAM_CONNECTION_TIMEOUT
-        )
+        try:
+            await asyncio.wait_for(
+                loop.sock_sendall(self.socket, message.encode("ascii")),
+                self.timeout,
+            )
+            adam_out = await asyncio.wait_for(
+                loop.sock_recv(self.socket, 100), self.timeout
+            )
+        except asyncio.TimeoutError:
+            raise AdamConnectionError("ADAM connection timed out")
 
         response = adam_out.decode().strip()
         return response
 
+    async def set_digital_out(
+        self,
+        pin: int,
+        value: bool,
+        model: None | Literal["6052"] | Literal["6317"] = None,
+    ) -> None:
+        if model is not None:
+            self.model = model
+
+        assert self.model is not None, "Model must be set before setting digital out"
+
+        if self.model == "6052":
+            command = f"#011{pin:x}0{int(value)}\r"
+        elif self.model == "6317":
+            command = f"#01D0{pin:x}{int(value)}\r"
+        else:
+            raise NotImplementedError(
+                f"Digital out not implemented for Adam-{self.model}"
+            )
+
+        response = await self._send_and_receive(command)
+        assert response[:3] == ">01", response[:3]
+
+    async def get_adam_digital_inputs(self) -> list[bool]:
+        response = await self._send_and_receive("$016\r")
+        assert response[:3] == "!01", f"Unexpected response: {response}"
+
+        binary_string = "".join(f"{int(char, 16):0>4b}" for char in response[3:])
+        return [char == "1" for char in binary_string][::-1]
+
+    async def get_adam_analog_inputs(self) -> list[float]:
+        response = await self._send_and_receive("#01\r")
+
+        assert response[:3] == ">01", response
+        response_data = response[3:]
+
+        # 7 characters per channel: +00.011
+        assert len(response_data) % 7 == 0, response_data
+
+        return [
+            float(response_data[i * 7 : i * 7 + 7])
+            for i in range(len(response_data) // 7)
+        ]
 
-async def set_adam_digital_out(
-    ip: str, model: Literal["6052"] | Literal["6317"], pin: int, value: bool
-) -> None:
-    if model == "6052":
-        command = f"#011{pin:x}0{int(value)}\r"
-    elif model == "6317":
-        command = f"#01D0{pin:x}{int(value)}\r"
-    else:
-        assert_never(model)
-
-    response = await _adam_send_and_receive(command, ip)
-    assert response[:3] == ">01", response[:3]
-
-
-async def get_adam_digital_inputs(ip: str) -> list[bool]:
-    response = await _adam_send_and_receive("$016\r", ip)
-    assert response[:3] == "!01", f"Unexpected response: {response}"
+    async def get_adam_model(self) -> str:
+        response = await self._send_and_receive("$01M\r")
 
-    binary_string = "".join(f"{int(char, 16):0>4b}" for char in response[3:])
-    return [char == "1" for char in binary_string][::-1]
+        assert response[:3] == "!01", f"Unexpected response: {response}"
 
+        self.model = response[3:]
 
-async def get_adam_analog_inputs(ip: str) -> list[float]:
-    response = await _adam_send_and_receive("#01\r", ip)
+        return self.model
 
-    assert response[:3] == ">01", response
-    response_data = response[3:]
 
-    # 7 characters per channel: +00.011
-    assert len(response_data) % 7 == 0, response_data
+@asynccontextmanager
+async def adam_connection_context(
+    ip: str,
+    port: int = DEFAULT_ADAM_PORT,
+    timeout: float = ADAM_CONNECTION_TIMEOUT,
+) -> AsyncIterator[AdamConnection]:
+    adam_sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
 
-    return [
-        float(response_data[i * 7 : i * 7 + 7]) for i in range(len(response_data) // 7)
-    ]
+    loop = asyncio.get_running_loop()
 
+    # according to chatgpt, asyncio does not support timeouts on UDP sockets
+    # so we manually do this with asyncio.wait_for, otherwise it will hang forever
+    adam_sock.setblocking(False)
 
-async def get_adam_model(ip: str) -> str:
-    response = await _adam_send_and_receive("$01M\r", ip)
+    try:
+        await loop.sock_connect(adam_sock, (ip, port))
+        yield AdamConnection(
+            adam_sock,
+            ip,
+            port,
+            timeout,
+        )
 
-    assert response[:3] == "!01", f"Unexpected response: {response}"
+    except OSError:
+        raise AdamConnectionError(f"Could not connect to ADAM at {ip}")
 
-    return response[3:]
+    finally:
+        adam_sock.close()
```

### Comparing `adam_modbus-0.0.1/pyproject.toml` & `adam_modbus-0.1.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adam-modbus"
-version = "0.0.1"
+version = "0.1.3"
 description = "asyncio python interface for Advantech ADAM modules"
 authors = ["Josh Gruenstein <josh@tutorintelligence.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -20,15 +20,10 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 style = "poetry_scripts:style"
 
 [tool.semantic_release]
-version_variable = [
-    "adam_modbus/__init__.py:__version__",
-    "pyproject.toml:version"
-]
-branch = "main"
-upload_to_pypi = true
-upload_to_release = false
+version_variables = ["adam_modbus/__init__.py:__version__"]
+version_toml = ["pyproject.toml:tool.poetry.version"]
 build_command = "pip install poetry && poetry build"
```

### Comparing `adam_modbus-0.0.1/PKG-INFO` & `adam_modbus-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam-modbus
-Version: 0.0.1
+Version: 0.1.3
 Summary: asyncio python interface for Advantech ADAM modules
 License: MIT
 Author: Josh Gruenstein
 Author-email: josh@tutorintelligence.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

