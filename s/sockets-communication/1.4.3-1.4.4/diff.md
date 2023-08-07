# Comparing `tmp/sockets-communication-1.4.3.tar.gz` & `tmp/sockets-communication-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockets-communication-1.4.3.tar", last modified: Mon Aug  7 16:35:01 2023, max compression
+gzip compressed data, was "sockets-communication-1.4.4.tar", last modified: Mon Aug  7 16:36:55 2023, max compression
```

## Comparing `sockets-communication-1.4.3.tar` & `sockets-communication-1.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 16:35:01.250398 sockets-communication-1.4.3/
--rw-rw-rw-   0        0        0       98 2023-08-07 16:35:00.000000 sockets-communication-1.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2107 2023-08-07 16:35:01.250398 sockets-communication-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.4.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.4.3/build.py
--rw-rw-rw-   0        0        0      708 2023-08-07 16:35:00.000000 sockets-communication-1.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.4.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.4.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 16:35:01.251398 sockets-communication-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1643 2023-08-07 16:34:55.000000 sockets-communication-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:35:01.233399 sockets-communication-1.4.3/sockets_communication/
--rw-rw-rw-   0        0        0      364 2023-07-08 10:32:37.000000 sockets-communication-1.4.3/sockets_communication/bluetooth.py
--rw-rw-rw-   0        0        0     5786 2023-07-08 15:47:06.000000 sockets-communication-1.4.3/sockets_communication/client.py
--rw-rw-rw-   0        0        0     3624 2023-07-08 15:47:46.000000 sockets-communication-1.4.3/sockets_communication/communication.py
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.4.3/sockets_communication/exceptions.py
--rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.4.3/sockets_communication/process.py
--rw-rw-rw-   0        0        0    15292 2023-07-08 16:02:53.000000 sockets-communication-1.4.3/sockets_communication/server.py
--rw-rw-rw-   0        0        0     9904 2023-08-07 16:34:20.000000 sockets-communication-1.4.3/sockets_communication/service.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:35:01.249429 sockets-communication-1.4.3/sockets_communication.egg-info/
--rw-rw-rw-   0        0        0     2107 2023-08-07 16:35:01.000000 sockets-communication-1.4.3/sockets_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-08-07 16:35:01.000000 sockets-communication-1.4.3/sockets_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 16:35:01.000000 sockets-communication-1.4.3/sockets_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-08-07 16:35:01.000000 sockets-communication-1.4.3/sockets_communication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-08-07 16:35:01.000000 sockets-communication-1.4.3/sockets_communication.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 16:36:55.296126 sockets-communication-1.4.4/
+-rw-rw-rw-   0        0        0       98 2023-08-07 16:36:55.000000 sockets-communication-1.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2107 2023-08-07 16:36:55.295126 sockets-communication-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.4.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.4.4/build.py
+-rw-rw-rw-   0        0        0      708 2023-08-07 16:36:55.000000 sockets-communication-1.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.4.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.4.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 16:36:55.296126 sockets-communication-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1643 2023-08-07 16:36:51.000000 sockets-communication-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:36:55.281046 sockets-communication-1.4.4/sockets_communication/
+-rw-rw-rw-   0        0        0      364 2023-07-08 10:32:37.000000 sockets-communication-1.4.4/sockets_communication/bluetooth.py
+-rw-rw-rw-   0        0        0     5786 2023-07-08 15:47:06.000000 sockets-communication-1.4.4/sockets_communication/client.py
+-rw-rw-rw-   0        0        0     3624 2023-07-08 15:47:46.000000 sockets-communication-1.4.4/sockets_communication/communication.py
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.4.4/sockets_communication/exceptions.py
+-rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.4.4/sockets_communication/process.py
+-rw-rw-rw-   0        0        0    15292 2023-07-08 16:02:53.000000 sockets-communication-1.4.4/sockets_communication/server.py
+-rw-rw-rw-   0        0        0    10037 2023-08-07 16:36:43.000000 sockets-communication-1.4.4/sockets_communication/service.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:36:55.295126 sockets-communication-1.4.4/sockets_communication.egg-info/
+-rw-rw-rw-   0        0        0     2107 2023-08-07 16:36:55.000000 sockets-communication-1.4.4/sockets_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-08-07 16:36:55.000000 sockets-communication-1.4.4/sockets_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 16:36:55.000000 sockets-communication-1.4.4/sockets_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-08-07 16:36:55.000000 sockets-communication-1.4.4/sockets_communication.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-08-07 16:36:55.000000 sockets-communication-1.4.4/sockets_communication.egg-info/top_level.txt
```

### Comparing `sockets-communication-1.4.3/PKG-INFO` & `sockets-communication-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.4.3
+Version: 1.4.4
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sockets-communication-1.4.3/README.md` & `sockets-communication-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.4.3/build.py` & `sockets-communication-1.4.4/build.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.4.3/pyproject.toml` & `sockets-communication-1.4.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'sockets-communication'
-version = '1.4.3'
+version = '1.4.4'
 description = 'This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `sockets-communication-1.4.3/setup.py` & `sockets-communication-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sockets-communication',
-        version='1.4.3',
+        version='1.4.4',
         description=(
             "This module provides a wrapper for the built-in "
             "socket module in python. The program provides server and. "
             "client classes, with the communication methods."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sockets-communication-1.4.3/sockets_communication/client.py` & `sockets-communication-1.4.4/sockets_communication/client.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.4.3/sockets_communication/communication.py` & `sockets-communication-1.4.4/sockets_communication/communication.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.4.3/sockets_communication/exceptions.py` & `sockets-communication-1.4.4/sockets_communication/exceptions.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.4.3/sockets_communication/process.py` & `sockets-communication-1.4.4/sockets_communication/process.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.4.3/sockets_communication/server.py` & `sockets-communication-1.4.4/sockets_communication/server.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.4.3/sockets_communication/service.py` & `sockets-communication-1.4.4/sockets_communication/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,12 +374,19 @@
             self._refreshing_process = None
         # end if
     # end stop_refreshing
 
     def terminate(self) -> None:
         """Pauses the process of service."""
 
+        self.stop()
+    # end terminate
+
+    def stop(self) -> None:
+        """Stops the service."""
+
         self.stop_blocking()
         self.stop_updating()
         self.stop_refreshing()
-    # end terminate
+        self.stop_timeout()
+    # end stop
 # end ServiceInterface
```

### Comparing `sockets-communication-1.4.3/sockets_communication.egg-info/PKG-INFO` & `sockets-communication-1.4.4/sockets_communication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.4.3
+Version: 1.4.4
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sockets-communication-1.4.3/sockets_communication.egg-info/SOURCES.txt` & `sockets-communication-1.4.4/sockets_communication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

