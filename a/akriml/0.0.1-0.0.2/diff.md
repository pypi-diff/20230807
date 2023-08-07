# Comparing `tmp/akriml-0.0.1.tar.gz` & `tmp/akriml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akriml-0.0.1.tar", last modified: Fri Jul 28 11:35:33 2023, max compression
+gzip compressed data, was "akriml-0.0.2.tar", last modified: Mon Aug  7 11:12:04 2023, max compression
```

## Comparing `akriml-0.0.1.tar` & `akriml-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sabarish   (502) staff       (20)        0 2023-07-28 11:35:33.601171 akriml-0.0.1/
--rw-r--r--   0 sabarish   (502) staff       (20)    11357 2023-07-27 09:53:22.000000 akriml-0.0.1/LICENSE
--rw-r--r--   0 sabarish   (502) staff       (20)    13468 2023-07-28 11:35:33.600950 akriml-0.0.1/PKG-INFO
--rw-r--r--   0 sabarish   (502) staff       (20)      372 2023-07-12 05:29:32.000000 akriml-0.0.1/README.md
-drwxr-xr-x   0 sabarish   (502) staff       (20)        0 2023-07-28 11:35:33.597821 akriml-0.0.1/akriml/
--rw-r--r--   0 sabarish   (502) staff       (20)        0 2023-07-12 10:40:38.000000 akriml-0.0.1/akriml/__init__.py
-drwxr-xr-x   0 sabarish   (502) staff       (20)        0 2023-07-28 11:35:33.599456 akriml-0.0.1/akriml/sketch/
--rw-r--r--   0 sabarish   (502) staff       (20)        0 2023-07-12 11:26:55.000000 akriml-0.0.1/akriml/sketch/__init__.py
--rw-r--r--   0 sabarish   (502) staff       (20)    23460 2023-07-27 09:48:54.000000 akriml-0.0.1/akriml/sketch/fastsketch.py
--rw-r--r--   0 sabarish   (502) staff       (20)    27097 2023-07-13 09:57:53.000000 akriml-0.0.1/akriml/sketch/sketch_utils.py
--rw-r--r--   0 sabarish   (502) staff       (20)     2479 2023-07-27 09:48:54.000000 akriml-0.0.1/akriml/utils.py
-drwxr-xr-x   0 sabarish   (502) staff       (20)        0 2023-07-28 11:35:33.598619 akriml-0.0.1/akriml.egg-info/
--rw-r--r--   0 sabarish   (502) staff       (20)    13468 2023-07-28 11:35:33.000000 akriml-0.0.1/akriml.egg-info/PKG-INFO
--rw-r--r--   0 sabarish   (502) staff       (20)      381 2023-07-28 11:35:33.000000 akriml-0.0.1/akriml.egg-info/SOURCES.txt
--rw-r--r--   0 sabarish   (502) staff       (20)        1 2023-07-28 11:35:33.000000 akriml-0.0.1/akriml.egg-info/dependency_links.txt
--rw-r--r--   0 sabarish   (502) staff       (20)      150 2023-07-28 11:35:33.000000 akriml-0.0.1/akriml.egg-info/requires.txt
--rw-r--r--   0 sabarish   (502) staff       (20)        7 2023-07-28 11:35:33.000000 akriml-0.0.1/akriml.egg-info/top_level.txt
--rw-r--r--   0 sabarish   (502) staff       (20)      928 2023-07-28 11:34:59.000000 akriml-0.0.1/pyproject.toml
--rw-r--r--   0 sabarish   (502) staff       (20)       38 2023-07-28 11:35:33.601215 akriml-0.0.1/setup.cfg
--rw-r--r--   0 sabarish   (502) staff       (20)      109 2023-07-12 10:06:37.000000 akriml-0.0.1/setup.py
-drwxr-xr-x   0 sabarish   (502) staff       (20)        0 2023-07-28 11:35:33.600435 akriml-0.0.1/tests/
--rw-r--r--   0 sabarish   (502) staff       (20)    14739 2023-07-27 09:48:57.000000 akriml-0.0.1/tests/test_fastsketch.py
--rw-r--r--   0 sabarish   (502) staff       (20)    15167 2023-07-27 09:48:57.000000 akriml-0.0.1/tests/test_sketch_utils.py
--rw-r--r--   0 sabarish   (502) staff       (20)     1820 2023-07-27 09:48:57.000000 akriml-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 sabarish   (502) staff       (20)        0 2023-08-07 11:12:04.866480 akriml-0.0.2/
+-rw-r--r--   0 sabarish   (502) staff       (20)    11357 2023-08-07 11:11:01.000000 akriml-0.0.2/LICENSE
+-rw-r--r--   0 sabarish   (502) staff       (20)    13468 2023-08-07 11:12:04.866315 akriml-0.0.2/PKG-INFO
+-rw-r--r--   0 sabarish   (502) staff       (20)      372 2023-08-07 11:11:01.000000 akriml-0.0.2/README.md
+drwxr-xr-x   0 sabarish   (502) staff       (20)        0 2023-08-07 11:12:04.864935 akriml-0.0.2/akriml/
+-rw-r--r--   0 sabarish   (502) staff       (20)        0 2023-08-07 11:11:01.000000 akriml-0.0.2/akriml/__init__.py
+drwxr-xr-x   0 sabarish   (502) staff       (20)        0 2023-08-07 11:12:04.865799 akriml-0.0.2/akriml/sketch/
+-rw-r--r--   0 sabarish   (502) staff       (20)        0 2023-08-07 11:11:01.000000 akriml-0.0.2/akriml/sketch/__init__.py
+-rw-r--r--   0 sabarish   (502) staff       (20)    23460 2023-08-07 11:11:01.000000 akriml-0.0.2/akriml/sketch/fastsketch.py
+-rw-r--r--   0 sabarish   (502) staff       (20)    27097 2023-08-07 11:11:01.000000 akriml-0.0.2/akriml/sketch/sketch_utils.py
+-rw-r--r--   0 sabarish   (502) staff       (20)     2479 2023-08-07 11:11:01.000000 akriml-0.0.2/akriml/utils.py
+drwxr-xr-x   0 sabarish   (502) staff       (20)        0 2023-08-07 11:12:04.865480 akriml-0.0.2/akriml.egg-info/
+-rw-r--r--   0 sabarish   (502) staff       (20)    13468 2023-08-07 11:12:04.000000 akriml-0.0.2/akriml.egg-info/PKG-INFO
+-rw-r--r--   0 sabarish   (502) staff       (20)      381 2023-08-07 11:12:04.000000 akriml-0.0.2/akriml.egg-info/SOURCES.txt
+-rw-r--r--   0 sabarish   (502) staff       (20)        1 2023-08-07 11:12:04.000000 akriml-0.0.2/akriml.egg-info/dependency_links.txt
+-rw-r--r--   0 sabarish   (502) staff       (20)      150 2023-08-07 11:12:04.000000 akriml-0.0.2/akriml.egg-info/requires.txt
+-rw-r--r--   0 sabarish   (502) staff       (20)        7 2023-08-07 11:12:04.000000 akriml-0.0.2/akriml.egg-info/top_level.txt
+-rw-r--r--   0 sabarish   (502) staff       (20)      945 2023-08-07 11:11:01.000000 akriml-0.0.2/pyproject.toml
+-rw-r--r--   0 sabarish   (502) staff       (20)       38 2023-08-07 11:12:04.866516 akriml-0.0.2/setup.cfg
+-rw-r--r--   0 sabarish   (502) staff       (20)      109 2023-08-07 11:11:01.000000 akriml-0.0.2/setup.py
+drwxr-xr-x   0 sabarish   (502) staff       (20)        0 2023-08-07 11:12:04.866144 akriml-0.0.2/tests/
+-rw-r--r--   0 sabarish   (502) staff       (20)    14739 2023-08-07 11:11:01.000000 akriml-0.0.2/tests/test_fastsketch.py
+-rw-r--r--   0 sabarish   (502) staff       (20)    15167 2023-08-07 11:11:01.000000 akriml-0.0.2/tests/test_sketch_utils.py
+-rw-r--r--   0 sabarish   (502) staff       (20)     1820 2023-08-07 11:11:01.000000 akriml-0.0.2/tests/test_utils.py
```

### Comparing `akriml-0.0.1/LICENSE` & `akriml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `akriml-0.0.1/PKG-INFO` & `akriml-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akriml
-Version: 0.0.1
+Version: 0.0.2
 Summary: ML methods for exploration and curation of large, high-dimensional datasets.
 Author: Sabarish Vadarevu
 Author-email: sabarish.vadarevu@akridata.ai
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akriml-0.0.1/akriml/sketch/fastsketch.py` & `akriml-0.0.2/akriml/sketch/fastsketch.py`

 * *Files identical despite different names*

### Comparing `akriml-0.0.1/akriml/sketch/sketch_utils.py` & `akriml-0.0.2/akriml/sketch/sketch_utils.py`

 * *Files identical despite different names*

### Comparing `akriml-0.0.1/akriml/utils.py` & `akriml-0.0.2/akriml/utils.py`

 * *Files identical despite different names*

### Comparing `akriml-0.0.1/akriml.egg-info/PKG-INFO` & `akriml-0.0.2/akriml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akriml
-Version: 0.0.1
+Version: 0.0.2
 Summary: ML methods for exploration and curation of large, high-dimensional datasets.
 Author: Sabarish Vadarevu
 Author-email: sabarish.vadarevu@akridata.ai
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akriml-0.0.1/pyproject.toml` & `akriml-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 name = "akriml"
 authors = [
     {name = "Sabarish Vadarevu"},
     {email = "sabarish.vadarevu@akridata.ai"}
 ]
 # We'll specify version statically
 # dynamic = ["version"]
-version = "0.0.1"
+version = "0.0.2"
 description = "ML methods for exploration and curation of large, high-dimensional datasets."
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 classifiers = [
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
 ]
 dependencies = [
-    "cython>=0.29.32", "numpy>=1.23.4", "scikit-learn>=1.1.3", "scipy>=1.9.3"
+    "cython>=0.29.32", "numpy>=1.19.2", "scikit-learn>=1.1.3", "scipy>=1.9.3"
 ]
 
 [project.urls]
 homepage = "https://akridata.ai"
 repository = "https://github.com/akridata-ai/AkriML"
 
 [project.optional-dependencies]
 dev = ["flake8", "pre-commit", "pytest", "black", "mypy", "pylint", "doctest", "twine"]
 test = ["pytest", "doctest"]
 
 [tool.setuptools]
-packages = ["akriml"]
+packages = ["akriml", "akriml.sketch"]
```

### Comparing `akriml-0.0.1/tests/test_fastsketch.py` & `akriml-0.0.2/tests/test_fastsketch.py`

 * *Files identical despite different names*

### Comparing `akriml-0.0.1/tests/test_sketch_utils.py` & `akriml-0.0.2/tests/test_sketch_utils.py`

 * *Files identical despite different names*

### Comparing `akriml-0.0.1/tests/test_utils.py` & `akriml-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

