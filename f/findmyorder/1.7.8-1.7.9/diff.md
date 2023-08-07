# Comparing `tmp/findmyorder-1.7.8.tar.gz` & `tmp/findmyorder-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.7.8.tar", max compression
+gzip compressed data, was "findmyorder-1.7.9.tar", max compression
```

## Comparing `findmyorder-1.7.8.tar` & `findmyorder-1.7.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-08-07 06:28:05.794532 findmyorder-1.7.8/LICENSE
--rw-r--r--   0        0        0     2923 2023-08-07 06:28:05.794532 findmyorder-1.7.8/README.md
--rw-r--r--   0        0        0      113 2023-08-07 06:28:10.394569 findmyorder-1.7.8/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-08-07 06:28:05.794532 findmyorder-1.7.8/findmyorder/config.py
--rw-r--r--   0        0        0     3221 2023-08-07 06:28:05.794532 findmyorder-1.7.8/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5931 2023-08-07 06:28:05.794532 findmyorder-1.7.8/findmyorder/main.py
--rw-r--r--   0        0        0     2864 2023-08-07 06:28:10.386569 findmyorder-1.7.8/pyproject.toml
--rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 findmyorder-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-07 08:13:48.954023 findmyorder-1.7.9/LICENSE
+-rw-r--r--   0        0        0     2923 2023-08-07 08:13:48.954023 findmyorder-1.7.9/README.md
+-rw-r--r--   0        0        0      113 2023-08-07 08:13:52.038030 findmyorder-1.7.9/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-08-07 08:13:48.954023 findmyorder-1.7.9/findmyorder/config.py
+-rw-r--r--   0        0        0     3221 2023-08-07 08:13:48.954023 findmyorder-1.7.9/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5931 2023-08-07 08:13:48.954023 findmyorder-1.7.9/findmyorder/main.py
+-rw-r--r--   0        0        0     2969 2023-08-07 08:13:52.030030 findmyorder-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 findmyorder-1.7.9/PKG-INFO
```

### Comparing `findmyorder-1.7.8/LICENSE` & `findmyorder-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.8/README.md` & `findmyorder-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.8/findmyorder/config.py` & `findmyorder-1.7.9/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.8/findmyorder/default_settings.toml` & `findmyorder-1.7.9/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.8/findmyorder/main.py` & `findmyorder-1.7.9/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.8/pyproject.toml` & `findmyorder-1.7.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "findmyorder"
-version = "1.7.8"
+version = "1.7.9"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -63,18 +63,21 @@
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.2.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = ">=5,<6"
-sphinx_bootstrap_theme = "^0.8.1"
+sphinx = "^7.0.0"
+pydata-sphinx-theme = "^0.13.3"
 sphinx-hoverxref = "^1.3.0"
-
+sphinx-notfound-page = "^0.8.3"
+sphinx_copybutton = "0.5.2"
+myst_parser = "^2.0.0"
+sphinx_design = "^0.5.0"
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
```

### Comparing `findmyorder-1.7.8/PKG-INFO` & `findmyorder-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.7.8
+Version: 1.7.9
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findmyorder Version: 1.7.8 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.7.9 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist: loguru
```

