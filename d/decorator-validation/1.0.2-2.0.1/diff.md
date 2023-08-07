# Comparing `tmp/decorator_validation-1.0.2.tar.gz` & `tmp/decorator_validation-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorator_validation-1.0.2.tar", max compression
+gzip compressed data, was "decorator_validation-2.0.1.tar", max compression
```

## Comparing `decorator_validation-1.0.2.tar` & `decorator_validation-2.0.1.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0      116 2023-08-05 05:49:37.771287 decorator_validation-1.0.2/decorator_validation/__init__.py
--rw-r--r--   0        0        0     2646 2023-08-05 05:30:05.838165 decorator_validation-1.0.2/decorator_validation/decorators.py
--rw-r--r--   0        0        0     1086 2023-08-05 06:26:33.296117 decorator_validation-1.0.2/LICENSE
--rw-r--r--   0        0        0      667 2023-08-05 06:27:45.742172 decorator_validation-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2196 2023-08-05 05:49:18.386963 decorator_validation-1.0.2/README.md
--rw-r--r--   0        0        0     2623 1970-01-01 00:00:00.000000 decorator_validation-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2023-08-07 18:01:40.419170 decorator_validation-2.0.1/decorator_validation/__init__.py
+-rw-r--r--   0        0        0     7879 2023-08-07 18:01:40.419170 decorator_validation-2.0.1/decorator_validation/decorators.py
+-rw-r--r--   0        0        0      180 2023-08-07 18:01:40.419170 decorator_validation-2.0.1/decorator_validation/std_validators.py
+-rw-r--r--   0        0        0      228 2023-08-07 18:01:40.420171 decorator_validation-2.0.1/decorator_validation/types.py
+-rw-r--r--   0        0        0     1086 2023-08-05 06:26:33.296117 decorator_validation-2.0.1/LICENSE
+-rw-r--r--   0        0        0      667 2023-08-07 18:03:38.521159 decorator_validation-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3327 2023-08-07 18:01:40.419170 decorator_validation-2.0.1/README.md
+-rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 decorator_validation-2.0.1/PKG-INFO
```

### Comparing `decorator_validation-1.0.2/LICENSE` & `decorator_validation-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decorator_validation-1.0.2/pyproject.toml` & `decorator_validation-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decorator_validation"
-version = "1.0.2"
+version = "2.0.1"
 description = "Fast Argument validation for functions using decorators"
 authors = ["FailedRobot <sry@nomail.com>"]
 homepage = "https://github.com/ahartlba/decoration_validation"
 readme = "README.md"
 packages = [{include = "decorator_validation"}]
 
 [tool.poetry.dependencies]
```

### Comparing `decorator_validation-1.0.2/README.md` & `decorator_validation-2.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -47,40 +47,80 @@
     ...
 
 ```
 
 Skip Type-checks by providing the `SkipTypecheck` class as a type, this is very usefull for methods.
 
 ```python
-from decorator_validation.decorators import validate_types, SkipTypeCheck
+from decorator_validation.decorators import validate_types
+from decorator_validation.types import SkipTypeCheck
 
 class FileReader:
 
     @validate_types((SkipTypeCheck,), file_path=(str,))
     def __init__(self, file_path: str):
         ...
 
 ```
 
 Of course, sometimes you want to have custom error messages.
 Then, just use the following code:
 
-
 ```python
 from decorator_validation.decorators import validate_with
 from pathlib import Path
 
 def my_validation_func(obj, file_path:str) -> True:
-    
+
     if not isinstance(file_path, str):
         raise TypeError(...)
-    if not Path(file_path).resolver().is_file():
+    if not Path(file_path).resolve().is_file():
         raise ValueError(...)
     return True
 
 class FileReader:
 
     @validate_with(my_validation_func)
     def __init__(self, file_path: str):
         ...
 
 ```
+
+## Map Multiple functions for subtypes
+
+You can also directly map different validation functions to your arguments.
+
+```python
+
+from decorator_validation.decorators import validate_map
+from decorator_validation.std_validators import is_file
+
+class FileReader:
+
+    @validate_map(None, file_path=is_file)
+    def __init__(self, file_path: str):
+        ...
+
+```
+
+## Validate Arbitrary Arguments
+
+Starting with version `2.0.0`, the package allows for a single use decorator called `validate`.
+
+Depending on the argument, it will either check the type or use a function to validate.
+If a tuple is used, the standard typecheck will be applied, if not it expectes a Callable that returns a boolean value.
+All of the examples above can be directly copied and just the name of the decorator has to be changed.
+
+An example.
+
+```python
+
+from decorator_validation.decorators import validate
+from decorator_validation.std_validators import is_file
+
+class Logger:
+
+    @validate(file_path=is_file, message:str)
+    def log(file_path: str, message:str):
+        ...
+
+```
```

### Comparing `decorator_validation-1.0.2/PKG-INFO` & `decorator_validation-2.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorator-validation
-Version: 1.0.2
+Version: 2.0.1
 Summary: Fast Argument validation for functions using decorators
 Home-page: https://github.com/ahartlba/decoration_validation
 Author: FailedRobot
 Author-email: sry@nomail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -61,41 +61,81 @@
     ...
 
 ```
 
 Skip Type-checks by providing the `SkipTypecheck` class as a type, this is very usefull for methods.
 
 ```python
-from decorator_validation.decorators import validate_types, SkipTypeCheck
+from decorator_validation.decorators import validate_types
+from decorator_validation.types import SkipTypeCheck
 
 class FileReader:
 
     @validate_types((SkipTypeCheck,), file_path=(str,))
     def __init__(self, file_path: str):
         ...
 
 ```
 
 Of course, sometimes you want to have custom error messages.
 Then, just use the following code:
 
-
 ```python
 from decorator_validation.decorators import validate_with
 from pathlib import Path
 
 def my_validation_func(obj, file_path:str) -> True:
-    
+
     if not isinstance(file_path, str):
         raise TypeError(...)
-    if not Path(file_path).resolver().is_file():
+    if not Path(file_path).resolve().is_file():
         raise ValueError(...)
     return True
 
 class FileReader:
 
     @validate_with(my_validation_func)
     def __init__(self, file_path: str):
         ...
 
 ```
 
+## Map Multiple functions for subtypes
+
+You can also directly map different validation functions to your arguments.
+
+```python
+
+from decorator_validation.decorators import validate_map
+from decorator_validation.std_validators import is_file
+
+class FileReader:
+
+    @validate_map(None, file_path=is_file)
+    def __init__(self, file_path: str):
+        ...
+
+```
+
+## Validate Arbitrary Arguments
+
+Starting with version `2.0.0`, the package allows for a single use decorator called `validate`.
+
+Depending on the argument, it will either check the type or use a function to validate.
+If a tuple is used, the standard typecheck will be applied, if not it expectes a Callable that returns a boolean value.
+All of the examples above can be directly copied and just the name of the decorator has to be changed.
+
+An example.
+
+```python
+
+from decorator_validation.decorators import validate
+from decorator_validation.std_validators import is_file
+
+class Logger:
+
+    @validate(file_path=is_file, message:str)
+    def log(file_path: str, message:str):
+        ...
+
+```
+
```

