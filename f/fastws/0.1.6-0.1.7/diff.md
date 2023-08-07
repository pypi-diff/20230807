# Comparing `tmp/fastws-0.1.6.tar.gz` & `tmp/fastws-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastws-0.1.6.tar", max compression
+gzip compressed data, was "fastws-0.1.7.tar", max compression
```

## Comparing `fastws-0.1.6.tar` & `fastws-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-07-06 20:53:23.287732 fastws-0.1.6/LICENSE
--rw-r--r--   0        0        0    10497 2023-07-27 10:53:34.903557 fastws-0.1.6/README.md
--rw-r--r--   0        0        0      437 2023-07-27 11:14:57.453092 fastws-0.1.6/fastws/__init__.py
--rw-r--r--   0        0        0     6890 2023-07-27 10:32:07.574023 fastws-0.1.6/fastws/application.py
--rw-r--r--   0        0        0     1643 2023-07-07 20:52:02.052422 fastws-0.1.6/fastws/asyncapi.py
--rw-r--r--   0        0        0     4505 2023-07-07 21:04:00.652291 fastws-0.1.6/fastws/broker.py
--rw-r--r--   0        0        0     6404 2023-07-07 20:54:39.992394 fastws-0.1.6/fastws/docs.py
--rw-r--r--   0        0        0     7148 2023-07-27 11:13:29.813122 fastws-0.1.6/fastws/routing.py
--rw-r--r--   0        0        0     1261 2023-07-27 11:14:57.363093 fastws-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    11609 1970-01-01 00:00:00.000000 fastws-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-06 20:53:23.287732 fastws-0.1.7/LICENSE
+-rw-r--r--   0        0        0    10497 2023-07-27 10:53:34.903557 fastws-0.1.7/README.md
+-rw-r--r--   0        0        0      437 2023-08-07 15:05:15.561111 fastws-0.1.7/fastws/__init__.py
+-rw-r--r--   0        0        0     6891 2023-08-07 14:52:01.541399 fastws-0.1.7/fastws/application.py
+-rw-r--r--   0        0        0     1643 2023-07-07 20:52:02.052422 fastws-0.1.7/fastws/asyncapi.py
+-rw-r--r--   0        0        0     4505 2023-07-07 21:04:00.652291 fastws-0.1.7/fastws/broker.py
+-rw-r--r--   0        0        0     6404 2023-07-07 20:54:39.992394 fastws-0.1.7/fastws/docs.py
+-rw-r--r--   0        0        0     7148 2023-07-27 11:13:29.813122 fastws-0.1.7/fastws/routing.py
+-rw-r--r--   0        0        0     1261 2023-08-07 15:05:15.451111 fastws-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    11609 1970-01-01 00:00:00.000000 fastws-0.1.7/PKG-INFO
```

### Comparing `fastws-0.1.6/LICENSE` & `fastws-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastws-0.1.6/README.md` & `fastws-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fastws-0.1.6/fastws/application.py` & `fastws-0.1.7/fastws/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,27 +118,27 @@
 
     async def handle_exception(
         self,
         exc: ValueError | ValidationError | NoMatchingOperation | TimeoutError,
     ):
         self.log(f"could not parse message {exc}")
         error = WebSocketException(
-            code=status.WS_1006_ABNORMAL_CLOSURE, reason="Could not decode message"
+            code=status.WS_1003_UNSUPPORTED_DATA, reason="Could not decode message"
         )
         if isinstance(exc, ValidationError):
-            error.add_note("Could not validate payload")
+            error.reason = "Could not validate payload"
         if isinstance(exc, NoMatchingOperation):
-            error.add_note("No matching type")
+            error.reason = "No matching type"
         if isinstance(exc, TimeoutError):
-            error.add_note(
+            error.reason = (
                 "Connection timed out. "
                 + f"Heartbeat interval {self.heartbeat_interval or 'unset'}. "
                 + f"Max connection lifespan {self.max_connection_lifespan or 'unset'}"
             )
-        raise exc
+        raise error
 
     async def serve(self, client: Client):
         try:
             async with asyncio.timeout(
                 self.heartbeat_interval
             ) as heartbeat_cm, asyncio.timeout(
                 self.max_connection_lifespan,
```

### Comparing `fastws-0.1.6/fastws/asyncapi.py` & `fastws-0.1.7/fastws/asyncapi.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.6/fastws/broker.py` & `fastws-0.1.7/fastws/broker.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.6/fastws/docs.py` & `fastws-0.1.7/fastws/docs.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.6/fastws/routing.py` & `fastws-0.1.7/fastws/routing.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.6/pyproject.toml` & `fastws-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastws"
-version = "0.1.6"
+version = "0.1.7"
 description = "FastWS framework. A WebSocket wrapper around FastAPI with auto-documentation using AsyncAPI."
 authors = ["Endre Krohn <endre@skript.no>"]
 readme = "README.md"
 packages = [{ include = "fastws" }]
 repository = "https://github.com/endrekrohn/fastws"
 documentation = "https://github.com/endrekrohn/fastws"
 keywords = ["fastapi", "pydantic", "starlette", "websockets", "asyncapi"]
```

### Comparing `fastws-0.1.6/PKG-INFO` & `fastws-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastws
-Version: 0.1.6
+Version: 0.1.7
 Summary: FastWS framework. A WebSocket wrapper around FastAPI with auto-documentation using AsyncAPI.
 Home-page: https://github.com/endrekrohn/fastws
 Keywords: fastapi,pydantic,starlette,websockets,asyncapi
 Author: Endre Krohn
 Author-email: endre@skript.no
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

