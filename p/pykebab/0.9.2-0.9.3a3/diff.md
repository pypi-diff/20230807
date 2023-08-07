# Comparing `tmp/pykebab-0.9.2.tar.gz` & `tmp/pykebab-0.9.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykebab-0.9.2.tar", max compression
+gzip compressed data, was "pykebab-0.9.3a3.tar", max compression
```

## Comparing `pykebab-0.9.2.tar` & `pykebab-0.9.3a3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      821 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/__init__.py
--rw-r--r--   0        0        0     3920 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/aws.py
--rw-r--r--   0        0        0       40 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/cli/__init__.py
--rw-r--r--   0        0        0     1801 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/cli/cli.py
--rw-r--r--   0        0        0      902 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/constants.py
--rw-r--r--   0        0        0       42 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/exceptions.py
--rw-r--r--   0        0        0     2586 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/k8s.py
--rw-r--r--   0        0        0      744 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/loaders.py
--rw-r--r--   0        0        0     2368 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/magic.py
--rw-r--r--   0        0        0     1575 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/openers.py
--rw-r--r--   0        0        0    23051 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/sources.py
--rw-r--r--   0        0        0     4825 2023-08-04 12:11:33.828234 pykebab-0.9.2/kebab/utils.py
--rw-r--r--   0        0        0      956 2023-08-04 12:11:33.832234 pykebab-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 pykebab-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/__init__.py
+-rw-r--r--   0        0        0     3920 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/aws.py
+-rw-r--r--   0        0        0       40 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/cli/__init__.py
+-rw-r--r--   0        0        0     1801 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/cli/cli.py
+-rw-r--r--   0        0        0      902 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/constants.py
+-rw-r--r--   0        0        0       42 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/exceptions.py
+-rw-r--r--   0        0        0     2586 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/k8s.py
+-rw-r--r--   0        0        0      744 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/loaders.py
+-rw-r--r--   0        0        0     2368 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/magic.py
+-rw-r--r--   0        0        0     1575 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/openers.py
+-rw-r--r--   0        0        0    23051 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/sources.py
+-rw-r--r--   0        0        0     4825 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/kebab/utils.py
+-rw-r--r--   0        0        0      958 2023-08-07 05:37:00.069829 pykebab-0.9.3a3/pyproject.toml
+-rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 pykebab-0.9.3a3/PKG-INFO
```

### Comparing `pykebab-0.9.2/kebab/__init__.py` & `pykebab-0.9.3a3/kebab/__init__.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.2/kebab/aws.py` & `pykebab-0.9.3a3/kebab/aws.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.2/kebab/cli/cli.py` & `pykebab-0.9.3a3/kebab/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.2/kebab/constants.py` & `pykebab-0.9.3a3/kebab/constants.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.2/kebab/k8s.py` & `pykebab-0.9.3a3/kebab/k8s.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.2/kebab/loaders.py` & `pykebab-0.9.3a3/kebab/loaders.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.2/kebab/magic.py` & `pykebab-0.9.3a3/kebab/magic.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.2/kebab/openers.py` & `pykebab-0.9.3a3/kebab/openers.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.2/kebab/sources.py` & `pykebab-0.9.3a3/kebab/sources.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.2/kebab/utils.py` & `pykebab-0.9.3a3/kebab/utils.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.2/pyproject.toml` & `pykebab-0.9.3a3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykebab"
-version = "0.9.2"
+version = "0.9.3a3"
 description = ""
 authors = ["Yangming Huang <leonmax@gmail.com>"]
 packages = [
     { include = "kebab" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `pykebab-0.9.2/PKG-INFO` & `pykebab-0.9.3a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykebab
-Version: 0.9.2
+Version: 0.9.3a3
 Summary: 
 Author: Yangming Huang
 Author-email: leonmax@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

