# Comparing `tmp/dynamic-service-1.5.0.tar.gz` & `tmp/dynamic-service-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.5.0.tar", last modified: Wed Jul 12 13:02:51 2023, max compression
+gzip compressed data, was "dynamic-service-1.5.1.tar", last modified: Tue Jul 25 09:27:56 2023, max compression
```

## Comparing `dynamic-service-1.5.0.tar` & `dynamic-service-1.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.079254 dynamic-service-1.5.0/
--rw-rw-rw-   0        0        0      236 2023-07-12 13:02:48.000000 dynamic-service-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-07-12 13:02:51.079254 dynamic-service-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.017291 dynamic-service-1.5.0/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.062075 dynamic-service-1.5.0/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.5.0/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     8954 2023-07-08 15:55:29.000000 dynamic-service-1.5.0/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.5.0/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.5.0/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.072245 dynamic-service-1.5.0/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    20656 2023-07-12 13:02:21.000000 dynamic-service-1.5.0/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.5.0/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.006088 dynamic-service-1.5.0/dynamic_service/source/
-drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.007088 dynamic-service-1.5.0/dynamic_service/source/assets/
-drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.077256 dynamic-service-1.5.0/dynamic_service/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/dynamic_service/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.5.0/dynamic_service/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-07-12 13:02:51.031104 dynamic-service-1.5.0/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-12 13:02:50.000000 dynamic-service-1.5.0/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-07-12 13:02:50.000000 dynamic-service-1.5.0/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 13:02:50.000000 dynamic-service-1.5.0/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-12 13:02:50.000000 dynamic-service-1.5.0/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-12 13:02:50.000000 dynamic-service-1.5.0/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-07-12 13:02:48.000000 dynamic-service-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.5.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 13:02:51.079254 dynamic-service-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-07-12 13:02:34.000000 dynamic-service-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.747994 dynamic-service-1.5.1/
+-rw-rw-rw-   0        0        0      236 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-25 09:27:56.747994 dynamic-service-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.734990 dynamic-service-1.5.1/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.744024 dynamic-service-1.5.1/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.5.1/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0     9485 2023-07-25 09:26:13.000000 dynamic-service-1.5.1/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.5.1/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.5.1/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.746025 dynamic-service-1.5.1/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    20656 2023-07-12 13:02:21.000000 dynamic-service-1.5.1/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.5.1/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.728036 dynamic-service-1.5.1/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.728036 dynamic-service-1.5.1/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.746995 dynamic-service-1.5.1/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.5.1/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-07-25 09:27:56.740021 dynamic-service-1.5.1/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-25 09:27:56.000000 dynamic-service-1.5.1/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-07-25 09:25:47.000000 dynamic-service-1.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.5.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.5.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 09:27:56.747994 dynamic-service-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-07-25 09:25:43.000000 dynamic-service-1.5.1/setup.py
```

### Comparing `dynamic-service-1.5.0/PKG-INFO` & `dynamic-service-1.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.5.0
+Version: 1.5.1
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.5.0/README.md` & `dynamic-service-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.0/build.py` & `dynamic-service-1.5.1/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.0/dynamic_service/base.py` & `dynamic-service-1.5.1/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.0/dynamic_service/endpoints/data.py` & `dynamic-service-1.5.1/dynamic_service/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.0/dynamic_service/endpoints/engine.py` & `dynamic-service-1.5.1/dynamic_service/endpoints/engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,40 +101,49 @@
 
     __modifiers__ = Modifiers(
         excluded=["options"], hidden=["record", "service"]
     )
 
     PATH: str
     METHODS: List[str]
+    RECORD: bool = False
 
     __slots__ = (
         "path", "methods", "service", "description",
-        "root", "options", "record"
+        "root", "options", "record", "recording"
     )
 
     def __init__(
             self,
             path: Optional[str] = None,
             methods: Optional[Iterable[str]] = None,
             service: Optional[_ServiceType] = None,
+            record: Optional[bool] = None,
             description: Optional[str] = None,
             root: Optional[str] = None,
             options: Optional[Dict[str, Any]] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param path: The path to the endpoint.
         :param methods: The endpoint methods.
+        :param record: The value to record the endpoint.
         :param description: The description of the object.
         :param root: The root to the path.
         :param options: Any keyword arguments.
         :param service: The service object.
         """
 
+        if record is None:
+            record = self.RECORD
+        # end if
+
+        self.recording = record
+
         self.record: List[Record] = []
 
         self.options = options or {}
 
         self.path = str(path or self.PATH)
         self.root = root or ""
         self.description = description
@@ -150,29 +159,43 @@
 
         :param name: The intent that activated the command.
         :param message: The message for the intent.
 
         :return: The function to command the command.
         """
 
-        return self.process(self.wrap(self.endpoint)(*args, **kwargs))
+        record = None
+
+        if self.recording:
+            record = Record(args=args, kwargs=kwargs)
+        # end if
+
+        returns = self.wrap(self.endpoint)(*args, **kwargs)
+
+        if record:
+            record.returns = returns
+
+            self.record.append(record)
+        # end if
+
+        return self.process(returns)
     # end __call__
 
     @staticmethod
     def call(instance) -> Callable[..., _ReturnType]:
         """
         Returns the function to command the command.
 
         :param instance: An instance of the class.
 
         :return: The function to command the command.
         """
 
         return instance.__call__
-    # end __call__
+    # end call
 
     def process(self, response: _ReturnType) -> _ProcessedReturnType:
         """
         Processes the response of the endpoint.
 
         :param response: The endpoint response to process.
```

### Comparing `dynamic-service-1.5.0/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.5.1/dynamic_service/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.0/dynamic_service/endpoints/process.py` & `dynamic-service-1.5.1/dynamic_service/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.0/dynamic_service/service/rest.py` & `dynamic-service-1.5.1/dynamic_service/service/rest.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.0/dynamic_service/service/sockets.py` & `dynamic-service-1.5.1/dynamic_service/service/sockets.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.0/dynamic_service/source/assets/icon/icon.ico` & `dynamic-service-1.5.1/dynamic_service/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.0/dynamic_service/source/assets/icon/icon.png` & `dynamic-service-1.5.1/dynamic_service/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.0/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.5.1/dynamic_service.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.5.0
+Version: 1.5.1
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.5.0/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.5.1/dynamic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.0/pyproject.toml` & `dynamic-service-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.5.0'
+version = '1.5.1'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.5.0/setup.py` & `dynamic-service-1.5.1/setup.py`

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
-        version='1.5.0',
+        version='1.5.1',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

