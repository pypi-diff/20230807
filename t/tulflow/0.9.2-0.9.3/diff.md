# Comparing `tmp/tulflow-0.9.2.tar.gz` & `tmp/tulflow-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulflow-0.9.2.tar", last modified: Fri May 19 19:59:21 2023, max compression
+gzip compressed data, was "tulflow-0.9.3.tar", last modified: Mon Aug  7 14:58:17 2023, max compression
```

## Comparing `tulflow-0.9.2.tar` & `tulflow-0.9.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-19 19:59:21.077649 tulflow-0.9.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-05-19 19:59:13.000000 tulflow-0.9.2/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2067 2023-05-19 19:59:21.077649 tulflow-0.9.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1562 2023-05-19 19:59:13.000000 tulflow-0.9.2/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-19 19:59:21.077649 tulflow-0.9.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1376 2023-05-19 19:59:13.000000 tulflow-0.9.2/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-19 19:59:21.077649 tulflow-0.9.2/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-19 19:59:13.000000 tulflow-0.9.2/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1013 2023-05-19 19:59:13.000000 tulflow-0.9.2/tests/test_devo-256_lxml_bug.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27321 2023-05-19 19:59:13.000000 tulflow-0.9.2/tests/test_harvest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10879 2023-05-19 19:59:13.000000 tulflow-0.9.2/tests/test_process.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6929 2023-05-19 19:59:13.000000 tulflow-0.9.2/tests/test_solr_api_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5361 2023-05-19 19:59:13.000000 tulflow-0.9.2/tests/test_tasks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6536 2023-05-19 19:59:13.000000 tulflow-0.9.2/tests/test_transform.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39623 2023-05-19 19:59:13.000000 tulflow-0.9.2/tests/test_validate.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-19 19:59:21.077649 tulflow-0.9.2/tulflow/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-19 19:59:13.000000 tulflow-0.9.2/tulflow/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10241 2023-05-19 19:59:13.000000 tulflow-0.9.2/tulflow/harvest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4926 2023-05-19 19:59:13.000000 tulflow-0.9.2/tulflow/process.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8536 2023-05-19 19:59:13.000000 tulflow-0.9.2/tulflow/solr_api_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5201 2023-05-19 19:59:13.000000 tulflow-0.9.2/tulflow/tasks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3102 2023-05-19 19:59:13.000000 tulflow-0.9.2/tulflow/transform.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6372 2023-05-19 19:59:13.000000 tulflow-0.9.2/tulflow/validate.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-19 19:59:21.077649 tulflow-0.9.2/tulflow.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2067 2023-05-19 19:59:21.000000 tulflow-0.9.2/tulflow.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      482 2023-05-19 19:59:21.000000 tulflow-0.9.2/tulflow.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-19 19:59:21.000000 tulflow-0.9.2/tulflow.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2023-05-19 19:59:21.000000 tulflow-0.9.2/tulflow.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 14:58:17.488450 tulflow-0.9.3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-08-07 14:58:10.000000 tulflow-0.9.3/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2067 2023-08-07 14:58:17.488450 tulflow-0.9.3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1562 2023-08-07 14:58:10.000000 tulflow-0.9.3/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-08-07 14:58:17.488450 tulflow-0.9.3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1376 2023-08-07 14:58:10.000000 tulflow-0.9.3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 14:58:17.488450 tulflow-0.9.3/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-08-07 14:58:10.000000 tulflow-0.9.3/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1013 2023-08-07 14:58:10.000000 tulflow-0.9.3/tests/test_devo-256_lxml_bug.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27321 2023-08-07 14:58:10.000000 tulflow-0.9.3/tests/test_harvest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10879 2023-08-07 14:58:10.000000 tulflow-0.9.3/tests/test_process.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6929 2023-08-07 14:58:10.000000 tulflow-0.9.3/tests/test_solr_api_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5361 2023-08-07 14:58:10.000000 tulflow-0.9.3/tests/test_tasks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6536 2023-08-07 14:58:10.000000 tulflow-0.9.3/tests/test_transform.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39623 2023-08-07 14:58:10.000000 tulflow-0.9.3/tests/test_validate.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 14:58:17.488450 tulflow-0.9.3/tulflow/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-08-07 14:58:10.000000 tulflow-0.9.3/tulflow/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10241 2023-08-07 14:58:10.000000 tulflow-0.9.3/tulflow/harvest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4926 2023-08-07 14:58:10.000000 tulflow-0.9.3/tulflow/process.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8536 2023-08-07 14:58:10.000000 tulflow-0.9.3/tulflow/solr_api_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5201 2023-08-07 14:58:10.000000 tulflow-0.9.3/tulflow/tasks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3102 2023-08-07 14:58:10.000000 tulflow-0.9.3/tulflow/transform.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6372 2023-08-07 14:58:10.000000 tulflow-0.9.3/tulflow/validate.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-08-07 14:58:17.488450 tulflow-0.9.3/tulflow.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2067 2023-08-07 14:58:17.000000 tulflow-0.9.3/tulflow.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      482 2023-08-07 14:58:17.000000 tulflow-0.9.3/tulflow.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-08-07 14:58:17.000000 tulflow-0.9.3/tulflow.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2023-08-07 14:58:17.000000 tulflow-0.9.3/tulflow.egg-info/top_level.txt
```

### Comparing `tulflow-0.9.2/LICENSE` & `tulflow-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/PKG-INFO` & `tulflow-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulflow
-Version: 0.9.2
+Version: 0.9.3
 Summary: Package of Temple University Library Indexing & ETL functions used by Airflow.
 Home-page: https://github.com/tulibraries/tulflow
 Author: Temple University Libraries
 Author-email: tul08567@temple.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tulflow-0.9.2/README.md` & `tulflow-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/setup.py` & `tulflow-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """tulflow Python package setup."""
 
 import os
 import sys
 import setuptools
 from setuptools.command.install import install
 
-VERSION = "v0.9.2"
+VERSION = "v0.9.3"
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 class VerifyVersionCommand(install):
     """Custom command to verify that the git tag matches our version"""
     description = 'verify that the git tag matches our version'
```

### Comparing `tulflow-0.9.2/tests/test_devo-256_lxml_bug.py` & `tulflow-0.9.3/tests/test_devo-256_lxml_bug.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tests/test_harvest.py` & `tulflow-0.9.3/tests/test_harvest.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tests/test_process.py` & `tulflow-0.9.3/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tests/test_solr_api_utils.py` & `tulflow-0.9.3/tests/test_solr_api_utils.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tests/test_tasks.py` & `tulflow-0.9.3/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tests/test_transform.py` & `tulflow-0.9.3/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tests/test_validate.py` & `tulflow-0.9.3/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tulflow/harvest.py` & `tulflow-0.9.3/tulflow/harvest.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tulflow/process.py` & `tulflow-0.9.3/tulflow/process.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tulflow/solr_api_utils.py` & `tulflow-0.9.3/tulflow/solr_api_utils.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tulflow/tasks.py` & `tulflow-0.9.3/tulflow/tasks.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tulflow/transform.py` & `tulflow-0.9.3/tulflow/transform.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tulflow/validate.py` & `tulflow-0.9.3/tulflow/validate.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.2/tulflow.egg-info/PKG-INFO` & `tulflow-0.9.3/tulflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulflow
-Version: 0.9.2
+Version: 0.9.3
 Summary: Package of Temple University Library Indexing & ETL functions used by Airflow.
 Home-page: https://github.com/tulibraries/tulflow
 Author: Temple University Libraries
 Author-email: tul08567@temple.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

