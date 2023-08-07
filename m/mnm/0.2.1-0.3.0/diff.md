# Comparing `tmp/mnm-0.2.1.tar.gz` & `tmp/mnm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnm-0.2.1.tar", last modified: Fri May  5 06:30:57 2023, max compression
+gzip compressed data, was "mnm-0.3.0.tar", last modified: Mon Aug  7 12:09:30 2023, max compression
```

## Comparing `mnm-0.2.1.tar` & `mnm-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:30:57.049017 mnm-0.2.1/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1067 2023-05-01 04:28:16.000000 mnm-0.2.1/LICENSE
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1328 2023-05-05 06:30:57.049017 mnm-0.2.1/PKG-INFO
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      830 2023-05-05 06:29:37.000000 mnm-0.2.1/README.md
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      604 2023-05-05 06:30:13.000000 mnm-0.2.1/pyproject.toml
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       38 2023-05-05 06:30:57.049017 mnm-0.2.1/setup.cfg
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:30:57.039017 mnm-0.2.1/src/
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:30:57.049017 mnm-0.2.1/src/mnm/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      256 2023-05-05 05:43:08.000000 mnm-0.2.1/src/mnm/__init__.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      655 2023-05-05 05:37:33.000000 mnm-0.2.1/src/mnm/_internal_utils.py
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:30:57.049017 mnm-0.2.1/src/mnm/examples/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      427 2023-05-05 06:14:01.000000 mnm-0.2.1/src/mnm/examples/mixed_options.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      382 2023-05-05 06:13:22.000000 mnm-0.2.1/src/mnm/examples/mixed_simple.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      445 2023-05-05 06:17:27.000000 mnm-0.2.1/src/mnm/examples/with_pattern.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      723 2023-05-05 06:16:06.000000 mnm-0.2.1/src/mnm/global_functions.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1795 2023-05-05 06:16:10.000000 mnm-0.2.1/src/mnm/header_mocking.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      638 2023-05-05 06:16:15.000000 mnm-0.2.1/src/mnm/mixed.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     2074 2023-05-05 06:16:19.000000 mnm-0.2.1/src/mnm/socket_fragmentation.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      353 2023-05-05 06:16:22.000000 mnm-0.2.1/src/mnm/wrapper.py
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:30:57.049017 mnm-0.2.1/src/mnm.egg-info/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1328 2023-05-05 06:30:57.000000 mnm-0.2.1/src/mnm.egg-info/PKG-INFO
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      455 2023-05-05 06:30:57.000000 mnm-0.2.1/src/mnm.egg-info/SOURCES.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        1 2023-05-05 06:30:57.000000 mnm-0.2.1/src/mnm.egg-info/dependency_links.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       17 2023-05-05 06:30:57.000000 mnm-0.2.1/src/mnm.egg-info/requires.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        4 2023-05-05 06:30:57.000000 mnm-0.2.1/src/mnm.egg-info/top_level.txt
+drwxrwxr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-08-07 12:09:30.694385 mnm-0.3.0/
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)     1067 2023-08-07 11:11:06.000000 mnm-0.3.0/LICENSE
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)     1328 2023-08-07 12:09:30.694385 mnm-0.3.0/PKG-INFO
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      830 2023-08-07 11:11:06.000000 mnm-0.3.0/README.md
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      604 2023-08-07 12:07:57.000000 mnm-0.3.0/pyproject.toml
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)       38 2023-08-07 12:09:30.694385 mnm-0.3.0/setup.cfg
+drwxrwxr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-08-07 12:09:30.694385 mnm-0.3.0/src/
+drwxrwxr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-08-07 12:09:30.694385 mnm-0.3.0/src/mnm/
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      256 2023-08-07 11:11:06.000000 mnm-0.3.0/src/mnm/__init__.py
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      655 2023-08-07 11:11:06.000000 mnm-0.3.0/src/mnm/_internal_utils.py
+drwxrwxr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-08-07 12:09:30.694385 mnm-0.3.0/src/mnm/examples/
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      427 2023-08-07 11:36:21.000000 mnm-0.3.0/src/mnm/examples/mixed_options.py
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      382 2023-08-07 11:11:06.000000 mnm-0.3.0/src/mnm/examples/mixed_simple.py
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      394 2023-08-07 11:52:58.000000 mnm-0.3.0/src/mnm/examples/ssl_test.py
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      445 2023-08-07 11:11:06.000000 mnm-0.3.0/src/mnm/examples/with_pattern.py
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      723 2023-08-07 11:11:06.000000 mnm-0.3.0/src/mnm/global_functions.py
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)     1795 2023-08-07 11:11:06.000000 mnm-0.3.0/src/mnm/header_mocking.py
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      638 2023-08-07 11:11:06.000000 mnm-0.3.0/src/mnm/mixed.py
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)     3128 2023-08-07 12:06:48.000000 mnm-0.3.0/src/mnm/socket_fragmentation.py
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      353 2023-08-07 11:11:06.000000 mnm-0.3.0/src/mnm/wrapper.py
+drwxrwxr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-08-07 12:09:30.694385 mnm-0.3.0/src/mnm.egg-info/
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)     1328 2023-08-07 12:09:30.000000 mnm-0.3.0/src/mnm.egg-info/PKG-INFO
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)      484 2023-08-07 12:09:30.000000 mnm-0.3.0/src/mnm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)        1 2023-08-07 12:09:30.000000 mnm-0.3.0/src/mnm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)       17 2023-08-07 12:09:30.000000 mnm-0.3.0/src/mnm.egg-info/requires.txt
+-rw-rw-r--   0 ohk990102  (1000) ohk990102  (1000)        4 2023-08-07 12:09:30.000000 mnm-0.3.0/src/mnm.egg-info/top_level.txt
```

### Comparing `mnm-0.2.1/LICENSE` & `mnm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mnm-0.2.1/PKG-INFO` & `mnm-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnm
-Version: 0.2.1
+Version: 0.3.0
 Summary: A simple python library for pentesting firewall protected webapp
 Author-email: ohk990102 <ohk990102@gmail.com>
 Project-URL: Homepage, https://github.com/ohk990102/mnm
 Project-URL: Bug Tracker, https://github.com/ohk990102/mnm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `mnm-0.2.1/README.md` & `mnm-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mnm-0.2.1/pyproject.toml` & `mnm-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mnm"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
   { name="ohk990102", email="ohk990102@gmail.com" },
 ]
 description = "A simple python library for pentesting firewall protected webapp"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `mnm-0.2.1/src/mnm/_internal_utils.py` & `mnm-0.3.0/src/mnm/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `mnm-0.2.1/src/mnm/global_functions.py` & `mnm-0.3.0/src/mnm/global_functions.py`

 * *Files identical despite different names*

### Comparing `mnm-0.2.1/src/mnm/header_mocking.py` & `mnm-0.3.0/src/mnm/header_mocking.py`

 * *Files identical despite different names*

### Comparing `mnm-0.2.1/src/mnm/mixed.py` & `mnm-0.3.0/src/mnm/mixed.py`

 * *Files identical despite different names*

### Comparing `mnm-0.2.1/src/mnm/socket_fragmentation.py` & `mnm-0.3.0/src/mnm/socket_fragmentation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import socket
+import ssl
+import time
+from sys import platform
 from .wrapper import MnmWrapper
 
 class SocketFragmentation(MnmWrapper):
-    def __init__(self, timeout=0.1, interval=0.01, slice=1):
+    def __init__(self, timeout=0.1, interval=0.01, slice=1, linux_ack_check=True):
         super().__init__()
         self.timeout = timeout
         self.interval = interval
         self.slice = slice
+        self.linux_ack_check = linux_ack_check
 
     def enable(self):
         if self.saved_state:
             return
 
         def flush_socket(sock: socket.socket) -> bool:
-            from sys import platform
-            import time
-            if platform == 'linux' or platform == 'linux2':
+            
+            if self.linux_ack_check and platform == 'linux' or platform == 'linux2':
                 from ctypes import c_ulong
                 from termios import TIOCOUTQ
                 from fcntl import ioctl
                 
                 cu = time.time()
 
                 while time.time() - cu < self.timeout and sock.fileno() != -1:
@@ -32,35 +35,53 @@
                     time.sleep(self.interval)
             else:
                 time.sleep(self.timeout)
 
             # not all data has been sent
             return False
 
-        def send(s, data, flags=0):
+        def _socket_send(s, data, flags=0):
             nbytes = 0
             for i in range(0, len(data), self.slice):
-                nbytes += super(socket.socket, s).send(data[i:i+self.slice], flags)
+                nbytes += self.saved_state['socket.send'].send(s, data[i:i+self.slice], flags)
                 flush_socket(s)
             return nbytes
 
-        def sendall(s, data, flags=0):
+        def _socket_sendall(s, data, flags=0):
             for i in range(0, len(data), self.slice):
-                super(socket.socket, s).sendall(data[i:i+self.slice], flags)
+                self.saved_state['socket.sendall'].sendall(s, data[i:i+self.slice], flags)
+                flush_socket(s)
+            return None
+
+        def _sslsocket_send(s: ssl.SSLSocket, data, flags=0):
+            nbytes = 0
+            for i in range(0, len(data), self.slice):
+                nbytes += self.saved_state['SSLSocket.send'](s, data[i:i+self.slice], flags)
+                flush_socket(s)
+            return nbytes
+
+        def _sslsocket_sendall(s: ssl.SSLSocket, data, flags=0):
+            for i in range(0, len(data), self.slice):
+                self.saved_state['SSLSocket.sendall'](s, data[i:i+self.slice], flags)
                 flush_socket(s)
             return None
 
         self.saved_state = {
-            'send': socket.socket.send,
-            'sendall': socket.socket.sendall
+            'socket.send': socket.socket.send,
+            'socket.sendall': socket.socket.sendall,
+            'SSLSocket.send': ssl.SSLSocket.send,
+            'SSLSocket.sendall': ssl.SSLSocket.sendall
         }
 
-        socket.socket.send = send
-        socket.socket.sendall = sendall
+        socket.socket.send = _socket_send
+        socket.socket.sendall = _socket_sendall
+        ssl.SSLSocket.send = _sslsocket_send
+        ssl.SSLSocket.sendall = _sslsocket_sendall
 
     def disable(self):
-        import socket
         if self.saved_state:
-            socket.socket.send = self.saved_state['send']
-            socket.socket.sendall = self.saved_state['sendall']
+            socket.socket.send = self.saved_state['socket.send']
+            socket.socket.sendall = self.saved_state['socket.sendall']
+            ssl.SSLSocket.send = self.saved_state['SSLSocket.send']
+            ssl.SSLSocket.sendall = self.saved_state['SSLSocket.sendall']
 
         self.saved_state = None
```

### Comparing `mnm-0.2.1/src/mnm.egg-info/PKG-INFO` & `mnm-0.3.0/src/mnm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnm
-Version: 0.2.1
+Version: 0.3.0
 Summary: A simple python library for pentesting firewall protected webapp
 Author-email: ohk990102 <ohk990102@gmail.com>
 Project-URL: Homepage, https://github.com/ohk990102/mnm
 Project-URL: Bug Tracker, https://github.com/ohk990102/mnm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

