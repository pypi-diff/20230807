# Comparing `tmp/zcc-helper-3.2.dev3.tar.gz` & `tmp/zcc-helper-3.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcc-helper-3.2.dev3.tar", last modified: Mon Aug  7 06:46:42 2023, max compression
+gzip compressed data, was "zcc-helper-3.2.dev4.tar", last modified: Mon Aug  7 06:53:04 2023, max compression
```

## Comparing `zcc-helper-3.2.dev3.tar` & `zcc-helper-3.2.dev4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-07 06:46:42.593829 zcc-helper-3.2.dev3/
--rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-07 06:46:42.593617 zcc-helper-3.2.dev3/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     9867 2022-06-20 04:14:44.000000 zcc-helper-3.2.dev3/README.md
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-07 06:46:42.593881 zcc-helper-3.2.dev3/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)      661 2022-03-20 04:59:07.000000 zcc-helper-3.2.dev3/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-07 06:46:42.591920 zcc-helper-3.2.dev3/zcc/
--rw-r--r--   0 mark       (501) staff       (20)      313 2022-05-23 13:52:19.000000 zcc-helper-3.2.dev3/zcc/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4633 2022-06-17 23:28:44.000000 zcc-helper-3.2.dev3/zcc/__main__.py
--rw-r--r--   0 mark       (501) staff       (20)      248 2023-08-07 06:46:34.000000 zcc-helper-3.2.dev3/zcc/constants.py
--rw-r--r--   0 mark       (501) staff       (20)    17920 2023-08-07 06:46:29.000000 zcc-helper-3.2.dev3/zcc/controller.py
--rw-r--r--   0 mark       (501) staff       (20)      417 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev3/zcc/description.py
--rw-r--r--   0 mark       (501) staff       (20)     9773 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev3/zcc/device.py
--rw-r--r--   0 mark       (501) staff       (20)     4430 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev3/zcc/discovery.py
--rw-r--r--   0 mark       (501) staff       (20)      114 2022-02-14 13:53:41.000000 zcc-helper-3.2.dev3/zcc/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     3767 2023-08-06 06:56:34.000000 zcc-helper-3.2.dev3/zcc/protocol.py
--rw-r--r--   0 mark       (501) staff       (20)     6384 2023-08-06 07:00:14.000000 zcc-helper-3.2.dev3/zcc/socket.py
--rw-r--r--   0 mark       (501) staff       (20)     1954 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev3/zcc/trace.py
--rw-r--r--   0 mark       (501) staff       (20)      971 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev3/zcc/watchdog.py
--rwxr-xr-x   0 mark       (501) staff       (20)       29 2021-10-12 07:44:33.000000 zcc-helper-3.2.dev3/zcc.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-07 06:46:42.593236 zcc-helper-3.2.dev3/zcc_helper.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-07 06:46:42.000000 zcc-helper-3.2.dev3/zcc_helper.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      351 2023-08-07 06:46:42.000000 zcc-helper-3.2.dev3/zcc_helper.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-07 06:46:42.000000 zcc-helper-3.2.dev3/zcc_helper.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        4 2023-08-07 06:46:42.000000 zcc-helper-3.2.dev3/zcc_helper.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-07 06:53:04.701190 zcc-helper-3.2.dev4/
+-rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-07 06:53:04.700964 zcc-helper-3.2.dev4/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     9867 2022-06-20 04:14:44.000000 zcc-helper-3.2.dev4/README.md
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-07 06:53:04.701243 zcc-helper-3.2.dev4/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)      661 2022-03-20 04:59:07.000000 zcc-helper-3.2.dev4/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-07 06:53:04.699023 zcc-helper-3.2.dev4/zcc/
+-rw-r--r--   0 mark       (501) staff       (20)      313 2022-05-23 13:52:19.000000 zcc-helper-3.2.dev4/zcc/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4633 2022-06-17 23:28:44.000000 zcc-helper-3.2.dev4/zcc/__main__.py
+-rw-r--r--   0 mark       (501) staff       (20)      248 2023-08-07 06:52:58.000000 zcc-helper-3.2.dev4/zcc/constants.py
+-rw-r--r--   0 mark       (501) staff       (20)    17953 2023-08-07 06:52:48.000000 zcc-helper-3.2.dev4/zcc/controller.py
+-rw-r--r--   0 mark       (501) staff       (20)      417 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev4/zcc/description.py
+-rw-r--r--   0 mark       (501) staff       (20)     9773 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev4/zcc/device.py
+-rw-r--r--   0 mark       (501) staff       (20)     4430 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev4/zcc/discovery.py
+-rw-r--r--   0 mark       (501) staff       (20)      114 2022-02-14 13:53:41.000000 zcc-helper-3.2.dev4/zcc/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     3767 2023-08-06 06:56:34.000000 zcc-helper-3.2.dev4/zcc/protocol.py
+-rw-r--r--   0 mark       (501) staff       (20)     6384 2023-08-06 07:00:14.000000 zcc-helper-3.2.dev4/zcc/socket.py
+-rw-r--r--   0 mark       (501) staff       (20)     1954 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev4/zcc/trace.py
+-rw-r--r--   0 mark       (501) staff       (20)      971 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev4/zcc/watchdog.py
+-rwxr-xr-x   0 mark       (501) staff       (20)       29 2021-10-12 07:44:33.000000 zcc-helper-3.2.dev4/zcc.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-07 06:53:04.700635 zcc-helper-3.2.dev4/zcc_helper.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-07 06:53:04.000000 zcc-helper-3.2.dev4/zcc_helper.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      351 2023-08-07 06:53:04.000000 zcc-helper-3.2.dev4/zcc_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-07 06:53:04.000000 zcc-helper-3.2.dev4/zcc_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        4 2023-08-07 06:53:04.000000 zcc-helper-3.2.dev4/zcc_helper.egg-info/top_level.txt
```

### Comparing `zcc-helper-3.2.dev3/PKG-INFO` & `zcc-helper-3.2.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcc-helper
-Version: 3.2.dev3
+Version: 3.2.dev4
 Summary: ZIMI ZCC helper module
 Home-page: UNKNOWN
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `zcc-helper-3.2.dev3/README.md` & `zcc-helper-3.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev3/setup.py` & `zcc-helper-3.2.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev3/zcc/__main__.py` & `zcc-helper-3.2.dev4/zcc/__main__.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev3/zcc/controller.py` & `zcc-helper-3.2.dev4/zcc/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,25 +314,26 @@
             self.logger.error("ZCC status message\n%s", pformat(response))
 
     async def re_connect(self):
         '''Re-connect to a new socket and resend any queued messages.'''
 
         self.logger.error('Existing socket closed')
 
-        self.socket.unsubscribe(self)
-
-        self.closed_socket = self.socket
-        self.closed_socket.close()
-        self.closed_socket = None
-
-        self.socket = None
         self.ready = False
 
         while not self.ready:
 
+            self.socket.unsubscribe(self)
+
+            self.closed_socket = self.socket
+            self.closed_socket.close()
+            self.closed_socket = None
+
+            self.socket = None
+            
             try:
                 self.logger.info('Re-connecting to ZCC with new socket')
                 await self.connect(fast=True)
 
                 while True:
                     message = self.closed_socket.unsent()
                     if message:
```

### Comparing `zcc-helper-3.2.dev3/zcc/device.py` & `zcc-helper-3.2.dev4/zcc/device.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev3/zcc/discovery.py` & `zcc-helper-3.2.dev4/zcc/discovery.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev3/zcc/protocol.py` & `zcc-helper-3.2.dev4/zcc/protocol.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev3/zcc/socket.py` & `zcc-helper-3.2.dev4/zcc/socket.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev3/zcc/trace.py` & `zcc-helper-3.2.dev4/zcc/trace.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev3/zcc/watchdog.py` & `zcc-helper-3.2.dev4/zcc/watchdog.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev3/zcc_helper.egg-info/PKG-INFO` & `zcc-helper-3.2.dev4/zcc_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcc-helper
-Version: 3.2.dev3
+Version: 3.2.dev4
 Summary: ZIMI ZCC helper module
 Home-page: UNKNOWN
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

