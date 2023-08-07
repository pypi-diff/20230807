# Comparing `tmp/findmyorder-1.7.7.tar.gz` & `tmp/findmyorder-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.7.7.tar", max compression
+gzip compressed data, was "findmyorder-1.7.8.tar", max compression
```

## Comparing `findmyorder-1.7.7.tar` & `findmyorder-1.7.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-08-06 14:11:15.876749 findmyorder-1.7.7/LICENSE
--rw-r--r--   0        0        0     2923 2023-08-06 14:11:15.876749 findmyorder-1.7.7/README.md
--rw-r--r--   0        0        0      113 2023-08-06 14:11:19.016749 findmyorder-1.7.7/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-08-06 14:11:15.876749 findmyorder-1.7.7/findmyorder/config.py
--rw-r--r--   0        0        0     3221 2023-08-06 14:11:15.876749 findmyorder-1.7.7/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5931 2023-08-06 14:11:15.876749 findmyorder-1.7.7/findmyorder/main.py
--rw-r--r--   0        0        0     2878 2023-08-06 14:11:19.012750 findmyorder-1.7.7/pyproject.toml
--rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 findmyorder-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-07 06:28:05.794532 findmyorder-1.7.8/LICENSE
+-rw-r--r--   0        0        0     2923 2023-08-07 06:28:05.794532 findmyorder-1.7.8/README.md
+-rw-r--r--   0        0        0      113 2023-08-07 06:28:10.394569 findmyorder-1.7.8/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-08-07 06:28:05.794532 findmyorder-1.7.8/findmyorder/config.py
+-rw-r--r--   0        0        0     3221 2023-08-07 06:28:05.794532 findmyorder-1.7.8/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5931 2023-08-07 06:28:05.794532 findmyorder-1.7.8/findmyorder/main.py
+-rw-r--r--   0        0        0     2864 2023-08-07 06:28:10.386569 findmyorder-1.7.8/pyproject.toml
+-rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 findmyorder-1.7.8/PKG-INFO
```

### Comparing `findmyorder-1.7.7/LICENSE` & `findmyorder-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.7/README.md` & `findmyorder-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.7/findmyorder/config.py` & `findmyorder-1.7.8/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.7/findmyorder/default_settings.toml` & `findmyorder-1.7.8/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.7/findmyorder/main.py` & `findmyorder-1.7.8/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.7/pyproject.toml` & `findmyorder-1.7.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "findmyorder"
-version = "1.7.7"
+version = "1.7.8"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -65,15 +65,15 @@
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=5,<6"
 sphinx_bootstrap_theme = "^0.8.1"
-sphinxext-remoteliteralinclude = "^0.4.0"
+sphinx-hoverxref = "^1.3.0"
 
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
```

### Comparing `findmyorder-1.7.7/PKG-INFO` & `findmyorder-1.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.7.7
+Version: 1.7.8
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
-Metadata-Version: 2.1 Name: findmyorder Version: 1.7.7 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.7.8 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist: loguru
```

