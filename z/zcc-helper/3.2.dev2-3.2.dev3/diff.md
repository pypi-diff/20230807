# Comparing `tmp/zcc-helper-3.2.dev2.tar.gz` & `tmp/zcc-helper-3.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcc-helper-3.2.dev2.tar", last modified: Sun Aug  6 07:02:55 2023, max compression
+gzip compressed data, was "zcc-helper-3.2.dev3.tar", last modified: Mon Aug  7 06:46:42 2023, max compression
```

## Comparing `zcc-helper-3.2.dev2.tar` & `zcc-helper-3.2.dev3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-06 07:02:55.298365 zcc-helper-3.2.dev2/
--rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-06 07:02:55.298135 zcc-helper-3.2.dev2/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     9867 2022-06-20 04:14:44.000000 zcc-helper-3.2.dev2/README.md
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-06 07:02:55.298420 zcc-helper-3.2.dev2/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)      661 2022-03-20 04:59:07.000000 zcc-helper-3.2.dev2/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-06 07:02:55.296324 zcc-helper-3.2.dev2/zcc/
--rw-r--r--   0 mark       (501) staff       (20)      313 2022-05-23 13:52:19.000000 zcc-helper-3.2.dev2/zcc/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4633 2022-06-17 23:28:44.000000 zcc-helper-3.2.dev2/zcc/__main__.py
--rw-r--r--   0 mark       (501) staff       (20)      248 2023-08-06 07:02:49.000000 zcc-helper-3.2.dev2/zcc/constants.py
--rw-r--r--   0 mark       (501) staff       (20)    17921 2023-08-06 07:02:41.000000 zcc-helper-3.2.dev2/zcc/controller.py
--rw-r--r--   0 mark       (501) staff       (20)      417 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev2/zcc/description.py
--rw-r--r--   0 mark       (501) staff       (20)     9773 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev2/zcc/device.py
--rw-r--r--   0 mark       (501) staff       (20)     4430 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev2/zcc/discovery.py
--rw-r--r--   0 mark       (501) staff       (20)      114 2022-02-14 13:53:41.000000 zcc-helper-3.2.dev2/zcc/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     3767 2023-08-06 06:56:34.000000 zcc-helper-3.2.dev2/zcc/protocol.py
--rw-r--r--   0 mark       (501) staff       (20)     6384 2023-08-06 07:00:14.000000 zcc-helper-3.2.dev2/zcc/socket.py
--rw-r--r--   0 mark       (501) staff       (20)     1954 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev2/zcc/trace.py
--rw-r--r--   0 mark       (501) staff       (20)      971 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev2/zcc/watchdog.py
--rwxr-xr-x   0 mark       (501) staff       (20)       29 2021-10-12 07:44:33.000000 zcc-helper-3.2.dev2/zcc.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-06 07:02:55.297737 zcc-helper-3.2.dev2/zcc_helper.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-06 07:02:55.000000 zcc-helper-3.2.dev2/zcc_helper.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      351 2023-08-06 07:02:55.000000 zcc-helper-3.2.dev2/zcc_helper.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-06 07:02:55.000000 zcc-helper-3.2.dev2/zcc_helper.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        4 2023-08-06 07:02:55.000000 zcc-helper-3.2.dev2/zcc_helper.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-07 06:46:42.593829 zcc-helper-3.2.dev3/
+-rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-07 06:46:42.593617 zcc-helper-3.2.dev3/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     9867 2022-06-20 04:14:44.000000 zcc-helper-3.2.dev3/README.md
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-07 06:46:42.593881 zcc-helper-3.2.dev3/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)      661 2022-03-20 04:59:07.000000 zcc-helper-3.2.dev3/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-07 06:46:42.591920 zcc-helper-3.2.dev3/zcc/
+-rw-r--r--   0 mark       (501) staff       (20)      313 2022-05-23 13:52:19.000000 zcc-helper-3.2.dev3/zcc/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4633 2022-06-17 23:28:44.000000 zcc-helper-3.2.dev3/zcc/__main__.py
+-rw-r--r--   0 mark       (501) staff       (20)      248 2023-08-07 06:46:34.000000 zcc-helper-3.2.dev3/zcc/constants.py
+-rw-r--r--   0 mark       (501) staff       (20)    17920 2023-08-07 06:46:29.000000 zcc-helper-3.2.dev3/zcc/controller.py
+-rw-r--r--   0 mark       (501) staff       (20)      417 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev3/zcc/description.py
+-rw-r--r--   0 mark       (501) staff       (20)     9773 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev3/zcc/device.py
+-rw-r--r--   0 mark       (501) staff       (20)     4430 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev3/zcc/discovery.py
+-rw-r--r--   0 mark       (501) staff       (20)      114 2022-02-14 13:53:41.000000 zcc-helper-3.2.dev3/zcc/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     3767 2023-08-06 06:56:34.000000 zcc-helper-3.2.dev3/zcc/protocol.py
+-rw-r--r--   0 mark       (501) staff       (20)     6384 2023-08-06 07:00:14.000000 zcc-helper-3.2.dev3/zcc/socket.py
+-rw-r--r--   0 mark       (501) staff       (20)     1954 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev3/zcc/trace.py
+-rw-r--r--   0 mark       (501) staff       (20)      971 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev3/zcc/watchdog.py
+-rwxr-xr-x   0 mark       (501) staff       (20)       29 2021-10-12 07:44:33.000000 zcc-helper-3.2.dev3/zcc.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-07 06:46:42.593236 zcc-helper-3.2.dev3/zcc_helper.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-07 06:46:42.000000 zcc-helper-3.2.dev3/zcc_helper.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      351 2023-08-07 06:46:42.000000 zcc-helper-3.2.dev3/zcc_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-07 06:46:42.000000 zcc-helper-3.2.dev3/zcc_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        4 2023-08-07 06:46:42.000000 zcc-helper-3.2.dev3/zcc_helper.egg-info/top_level.txt
```

### Comparing `zcc-helper-3.2.dev2/PKG-INFO` & `zcc-helper-3.2.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcc-helper
-Version: 3.2.dev2
+Version: 3.2.dev3
 Summary: ZIMI ZCC helper module
 Home-page: UNKNOWN
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `zcc-helper-3.2.dev2/README.md` & `zcc-helper-3.2.dev3/README.md`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev2/setup.py` & `zcc-helper-3.2.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev2/zcc/__main__.py` & `zcc-helper-3.2.dev3/zcc/__main__.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev2/zcc/controller.py` & `zcc-helper-3.2.dev3/zcc/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,16 +317,18 @@
         '''Re-connect to a new socket and resend any queued messages.'''
 
         self.logger.error('Existing socket closed')
 
         self.socket.unsubscribe(self)
 
         self.closed_socket = self.socket
-        self.socket = None
+        self.closed_socket.close()
+        self.closed_socket = None
 
+        self.socket = None
         self.ready = False
 
         while not self.ready:
 
             try:
                 self.logger.info('Re-connecting to ZCC with new socket')
                 await self.connect(fast=True)
@@ -341,17 +343,14 @@
                         break
             except ControlPointError as error:
                 self.logger.error(
                     "Re-connection to ZCC failed with ControlPointError: %s - will retry in %d",
                     error, ControlPointProtocol.RETRY_TIMEOUT)
                 await asyncio.sleep(ControlPointProtocol.RETRY_TIMEOUT)
 
-        self.closed_socket.close()
-        self.closed_socket = None
-
         if self.watchdog_timer:
             self.watchdog_timer.reset()
 
     async def set(self, identifier: str, action: str, params: object = None):
         '''Sends an action for a device.'''
 
         while not self.connected_ready.is_set():
```

### Comparing `zcc-helper-3.2.dev2/zcc/device.py` & `zcc-helper-3.2.dev3/zcc/device.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev2/zcc/discovery.py` & `zcc-helper-3.2.dev3/zcc/discovery.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev2/zcc/protocol.py` & `zcc-helper-3.2.dev3/zcc/protocol.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev2/zcc/socket.py` & `zcc-helper-3.2.dev3/zcc/socket.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev2/zcc/trace.py` & `zcc-helper-3.2.dev3/zcc/trace.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev2/zcc/watchdog.py` & `zcc-helper-3.2.dev3/zcc/watchdog.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev2/zcc_helper.egg-info/PKG-INFO` & `zcc-helper-3.2.dev3/zcc_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcc-helper
-Version: 3.2.dev2
+Version: 3.2.dev3
 Summary: ZIMI ZCC helper module
 Home-page: UNKNOWN
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

