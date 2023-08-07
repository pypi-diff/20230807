# Comparing `tmp/dynamic-service-1.5.1.tar.gz` & `tmp/dynamic-service-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.5.1.tar", last modified: Tue Jul 25 09:27:56 2023, max compression
+gzip compressed data, was "dynamic-service-1.5.2.tar", last modified: Mon Aug  7 09:31:12 2023, max compression
```

## Comparing `dynamic-service-1.5.1.tar` & `dynamic-service-1.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.747994 dynamic-service-1.5.1/
--rw-rw-rw-   0        0        0      236 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-07-25 09:27:56.747994 dynamic-service-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.734990 dynamic-service-1.5.1/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.744024 dynamic-service-1.5.1/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.5.1/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     9485 2023-07-25 09:26:13.000000 dynamic-service-1.5.1/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.5.1/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.5.1/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.746025 dynamic-service-1.5.1/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    20656 2023-07-12 13:02:21.000000 dynamic-service-1.5.1/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.5.1/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.728036 dynamic-service-1.5.1/dynamic_service/source/
-drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.728036 dynamic-service-1.5.1/dynamic_service/source/assets/
-drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.746995 dynamic-service-1.5.1/dynamic_service/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/dynamic_service/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/dynamic_service/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.740021 dynamic-service-1.5.1/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-07-25 09:25:47.000000 dynamic-service-1.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.5.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.5.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 09:27:56.747994 dynamic-service-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-07-25 09:25:43.000000 dynamic-service-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:31:12.667425 dynamic-service-1.5.2/
+-rw-rw-rw-   0        0        0      236 2023-08-07 09:31:10.000000 dynamic-service-1.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-08-07 09:31:12.667425 dynamic-service-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.5.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.5.2/build.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:31:12.641629 dynamic-service-1.5.2/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.5.2/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:31:12.663427 dynamic-service-1.5.2/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.5.2/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.5.2/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0     9485 2023-07-25 09:26:13.000000 dynamic-service-1.5.2/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.5.2/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.5.2/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:31:12.665426 dynamic-service-1.5.2/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.5.2/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    20657 2023-08-07 09:30:58.000000 dynamic-service-1.5.2/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.5.2/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:31:12.636118 dynamic-service-1.5.2/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-08-07 09:31:12.636118 dynamic-service-1.5.2/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-08-07 09:31:12.666426 dynamic-service-1.5.2/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.5.2/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.5.2/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-08-07 09:31:12.659149 dynamic-service-1.5.2/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-08-07 09:31:12.000000 dynamic-service-1.5.2/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-08-07 09:31:12.000000 dynamic-service-1.5.2/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:31:12.000000 dynamic-service-1.5.2/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-08-07 09:31:12.000000 dynamic-service-1.5.2/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-07 09:31:12.000000 dynamic-service-1.5.2/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-08-07 09:31:10.000000 dynamic-service-1.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.5.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.5.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 09:31:12.667425 dynamic-service-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-08-07 09:31:08.000000 dynamic-service-1.5.2/setup.py
```

### Comparing `dynamic-service-1.5.1/PKG-INFO` & `dynamic-service-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.5.1
+Version: 1.5.2
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.5.1/README.md` & `dynamic-service-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.1/build.py` & `dynamic-service-1.5.2/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.1/dynamic_service/base.py` & `dynamic-service-1.5.2/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.1/dynamic_service/endpoints/data.py` & `dynamic-service-1.5.2/dynamic_service/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.1/dynamic_service/endpoints/engine.py` & `dynamic-service-1.5.2/dynamic_service/endpoints/engine.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.1/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.5.2/dynamic_service/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.1/dynamic_service/endpoints/process.py` & `dynamic-service-1.5.2/dynamic_service/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.1/dynamic_service/service/rest.py` & `dynamic-service-1.5.2/dynamic_service/service/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -594,15 +594,15 @@
 
     def run(
             self,
             serve: Optional[bool] = True,
             host: Optional[Host] = None,
             port: Optional[Port] = None,
             silent: Optional[bool] = None,
-            daemon: Optional[bool] = True,
+            daemon: Optional[bool] = False,
             block: Optional[bool] = False,
             update: Optional[bool] = True,
             refresh: Optional[Union[Number, dt.timedelta]] = True,
             wait: Union[Number, dt.timedelta, dt.datetime] = None,
             timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
     ) -> None:
         """
```

### Comparing `dynamic-service-1.5.1/dynamic_service/service/sockets.py` & `dynamic-service-1.5.2/dynamic_service/service/sockets.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.1/dynamic_service/source/assets/icon/icon.ico` & `dynamic-service-1.5.2/dynamic_service/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.1/dynamic_service/source/assets/icon/icon.png` & `dynamic-service-1.5.2/dynamic_service/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.1/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.5.2/dynamic_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.5.1
+Version: 1.5.2
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.5.1/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.5.2/dynamic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.1/pyproject.toml` & `dynamic-service-1.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.5.1'
+version = '1.5.2'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.5.1/setup.py` & `dynamic-service-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "dynamic_service/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='dynamic-service',
-        version='1.5.1',
+        version='1.5.2',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

