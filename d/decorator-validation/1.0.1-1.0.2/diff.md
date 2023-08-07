# Comparing `tmp/decorator_validation-1.0.1.tar.gz` & `tmp/decorator_validation-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorator_validation-1.0.1.tar", max compression
+gzip compressed data, was "decorator_validation-1.0.2.tar", max compression
```

## Comparing `decorator_validation-1.0.1.tar` & `decorator_validation-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      116 2023-08-05 05:49:37.771287 decorator_validation-1.0.1/decorator_validation/__init__.py
--rw-r--r--   0        0        0     2646 2023-08-05 05:30:05.838165 decorator_validation-1.0.1/decorator_validation/decorators.py
--rw-r--r--   0        0        0      603 2023-08-05 05:40:40.584014 decorator_validation-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2196 2023-08-05 05:49:18.386963 decorator_validation-1.0.1/README.md
--rw-r--r--   0        0        0     2562 1970-01-01 00:00:00.000000 decorator_validation-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-08-05 05:49:37.771287 decorator_validation-1.0.2/decorator_validation/__init__.py
+-rw-r--r--   0        0        0     2646 2023-08-05 05:30:05.838165 decorator_validation-1.0.2/decorator_validation/decorators.py
+-rw-r--r--   0        0        0     1086 2023-08-05 06:26:33.296117 decorator_validation-1.0.2/LICENSE
+-rw-r--r--   0        0        0      667 2023-08-05 06:27:45.742172 decorator_validation-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2196 2023-08-05 05:49:18.386963 decorator_validation-1.0.2/README.md
+-rw-r--r--   0        0        0     2623 1970-01-01 00:00:00.000000 decorator_validation-1.0.2/PKG-INFO
```

### Comparing `decorator_validation-1.0.1/decorator_validation/decorators.py` & `decorator_validation-1.0.2/decorator_validation/decorators.py`

 * *Files identical despite different names*

### Comparing `decorator_validation-1.0.1/pyproject.toml` & `decorator_validation-1.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "decorator_validation"
-version = "1.0.1"
+version = "1.0.2"
 description = "Fast Argument validation for functions using decorators"
 authors = ["FailedRobot <sry@nomail.com>"]
+homepage = "https://github.com/ahartlba/decoration_validation"
 readme = "README.md"
 packages = [{include = "decorator_validation"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 
 [tool.poetry.group.dev]
```

### Comparing `decorator_validation-1.0.1/README.md` & `decorator_validation-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `decorator_validation-1.0.1/PKG-INFO` & `decorator_validation-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: decorator-validation
-Version: 1.0.1
+Version: 1.0.2
 Summary: Fast Argument validation for functions using decorators
+Home-page: https://github.com/ahartlba/decoration_validation
 Author: FailedRobot
 Author-email: sry@nomail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

