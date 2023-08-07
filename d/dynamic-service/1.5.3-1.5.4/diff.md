# Comparing `tmp/dynamic-service-1.5.3.tar.gz` & `tmp/dynamic-service-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.5.3.tar", last modified: Mon Aug  7 12:24:20 2023, max compression
+gzip compressed data, was "dynamic-service-1.5.4.tar", last modified: Mon Aug  7 16:40:26 2023, max compression
```

## Comparing `dynamic-service-1.5.3.tar` & `dynamic-service-1.5.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 12:24:20.361771 dynamic-service-1.5.3/
--rw-rw-rw-   0        0        0      236 2023-08-07 12:24:20.000000 dynamic-service-1.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-08-07 12:24:20.361771 dynamic-service-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.5.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.5.3/build.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:24:20.297970 dynamic-service-1.5.3/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.5.3/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:24:20.344905 dynamic-service-1.5.3/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.5.3/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.5.3/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     9485 2023-07-25 09:26:13.000000 dynamic-service-1.5.3/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.5.3/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.5.3/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:24:20.354771 dynamic-service-1.5.3/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.5.3/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    20735 2023-08-07 12:24:08.000000 dynamic-service-1.5.3/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.5.3/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:24:20.287334 dynamic-service-1.5.3/dynamic_service/source/
-drwxrwxrwx   0        0        0        0 2023-08-07 12:24:20.287334 dynamic-service-1.5.3/dynamic_service/source/assets/
-drwxrwxrwx   0        0        0        0 2023-08-07 12:24:20.359772 dynamic-service-1.5.3/dynamic_service/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.5.3/dynamic_service/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.5.3/dynamic_service/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-08-07 12:24:20.311641 dynamic-service-1.5.3/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-08-07 12:24:20.000000 dynamic-service-1.5.3/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-08-07 12:24:20.000000 dynamic-service-1.5.3/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 12:24:20.000000 dynamic-service-1.5.3/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-08-07 12:24:20.000000 dynamic-service-1.5.3/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-07 12:24:20.000000 dynamic-service-1.5.3/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-08-07 12:24:20.000000 dynamic-service-1.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.5.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.5.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 12:24:20.361771 dynamic-service-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-08-07 12:24:16.000000 dynamic-service-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:40:26.372222 dynamic-service-1.5.4/
+-rw-rw-rw-   0        0        0      236 2023-08-07 16:40:25.000000 dynamic-service-1.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-08-07 16:40:26.371221 dynamic-service-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.5.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.5.4/build.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:40:26.345218 dynamic-service-1.5.4/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.5.4/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:40:26.367222 dynamic-service-1.5.4/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.5.4/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.5.4/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0     9485 2023-07-25 09:26:13.000000 dynamic-service-1.5.4/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.5.4/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.5.4/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:40:26.369223 dynamic-service-1.5.4/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.5.4/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    20725 2023-08-07 16:38:56.000000 dynamic-service-1.5.4/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.5.4/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:40:26.340225 dynamic-service-1.5.4/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-08-07 16:40:26.340225 dynamic-service-1.5.4/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-08-07 16:40:26.370222 dynamic-service-1.5.4/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.5.4/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.5.4/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-08-07 16:40:26.363217 dynamic-service-1.5.4/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-08-07 16:40:26.000000 dynamic-service-1.5.4/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-08-07 16:40:26.000000 dynamic-service-1.5.4/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 16:40:26.000000 dynamic-service-1.5.4/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-08-07 16:40:26.000000 dynamic-service-1.5.4/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-07 16:40:26.000000 dynamic-service-1.5.4/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-08-07 16:40:25.000000 dynamic-service-1.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.5.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.5.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 16:40:26.372222 dynamic-service-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-08-07 16:40:18.000000 dynamic-service-1.5.4/setup.py
```

### Comparing `dynamic-service-1.5.3/PKG-INFO` & `dynamic-service-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.5.3
+Version: 1.5.4
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.5.3/README.md` & `dynamic-service-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.3/build.py` & `dynamic-service-1.5.4/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.3/dynamic_service/base.py` & `dynamic-service-1.5.4/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.3/dynamic_service/endpoints/data.py` & `dynamic-service-1.5.4/dynamic_service/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.3/dynamic_service/endpoints/engine.py` & `dynamic-service-1.5.4/dynamic_service/endpoints/engine.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.3/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.5.4/dynamic_service/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.3/dynamic_service/endpoints/process.py` & `dynamic-service-1.5.4/dynamic_service/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.3/dynamic_service/service/rest.py` & `dynamic-service-1.5.4/dynamic_service/service/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -698,15 +698,15 @@
             self._serving_process = None
 
             self.server.should_exit = True
             self.server = None
         # end if
     # end stop_serving
 
-    def terminate(self) -> None:
+    def stop(self) -> None:
         """Pauses the process of service."""
 
-        super().terminate()
+        super().stop()
 
         self.stop_serving()
     # end terminate
 # end BaseService
```

### Comparing `dynamic-service-1.5.3/dynamic_service/service/sockets.py` & `dynamic-service-1.5.4/dynamic_service/service/sockets.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.3/dynamic_service/source/assets/icon/icon.ico` & `dynamic-service-1.5.4/dynamic_service/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.3/dynamic_service/source/assets/icon/icon.png` & `dynamic-service-1.5.4/dynamic_service/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.3/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.5.4/dynamic_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.5.3
+Version: 1.5.4
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.5.3/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.5.4/dynamic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.3/pyproject.toml` & `dynamic-service-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.5.3'
+version = '1.5.4'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.5.3/setup.py` & `dynamic-service-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "dynamic_service/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='dynamic-service',
-        version='1.5.3',
+        version='1.5.4',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

