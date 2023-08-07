# Comparing `tmp/cefeste-1.1.8.tar.gz` & `tmp/cefeste-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefeste-1.1.8.tar", last modified: Wed May 24 10:07:49 2023, max compression
+gzip compressed data, was "cefeste-1.1.9.tar", last modified: Wed May 24 10:24:36 2023, max compression
```

## Comparing `cefeste-1.1.8.tar` & `cefeste-1.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.203394 cefeste-1.1.8/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.8/LICENCE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2683 2023-05-24 10:07:49.203394 cefeste-1.1.8/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2321 2023-05-22 20:53:27.000000 cefeste-1.1.8/README.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      758 2023-05-24 10:06:35.000000 cefeste-1.1.8/pyproject.toml
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-24 10:07:49.203394 cefeste-1.1.8/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1001 2023-05-24 10:06:45.000000 cefeste-1.1.8/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.187393 cefeste-1.1.8/src/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.195394 cefeste-1.1.8/src/cefeste/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.199394 cefeste-1.1.8/src/cefeste/elimination/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15613 2023-05-24 10:03:32.000000 cefeste-1.1.8/src/cefeste/elimination/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27438 2023-05-24 10:05:17.000000 cefeste-1.1.8/src/cefeste/elimination/shap_rfe.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.203394 cefeste-1.1.8/src/cefeste/selection/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/selection/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/selection/explanatory.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/selection/multivariate.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.8/src/cefeste/selection/univariate.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.203394 cefeste-1.1.8/src/cefeste/transform/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2801 2023-05-24 08:21:06.000000 cefeste-1.1.8/src/cefeste/transform/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-10 10:23:33.000000 cefeste-1.1.8/src/cefeste/utils.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:07:49.199394 cefeste-1.1.8/src/cefeste.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2683 2023-05-24 10:07:49.000000 cefeste-1.1.8/src/cefeste.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-24 10:07:49.000000 cefeste-1.1.8/src/cefeste.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-24 10:07:49.000000 cefeste-1.1.8/src/cefeste.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      131 2023-05-24 10:07:49.000000 cefeste-1.1.8/src/cefeste.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-24 10:07:49.000000 cefeste-1.1.8/src/cefeste.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:24:36.620337 cefeste-1.1.9/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.9/LICENCE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2683 2023-05-24 10:24:36.616337 cefeste-1.1.9/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2321 2023-05-22 20:53:27.000000 cefeste-1.1.9/README.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      758 2023-05-24 10:22:29.000000 cefeste-1.1.9/pyproject.toml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-24 10:24:36.620337 cefeste-1.1.9/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1001 2023-05-24 10:22:25.000000 cefeste-1.1.9/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:24:36.596335 cefeste-1.1.9/src/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:24:36.608336 cefeste-1.1.9/src/cefeste/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.9/src/cefeste/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.9/src/cefeste/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:24:36.612336 cefeste-1.1.9/src/cefeste/elimination/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15613 2023-05-24 10:03:32.000000 cefeste-1.1.9/src/cefeste/elimination/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27522 2023-05-24 10:23:41.000000 cefeste-1.1.9/src/cefeste/elimination/shap_rfe.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:24:36.616337 cefeste-1.1.9/src/cefeste/selection/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.9/src/cefeste/selection/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.9/src/cefeste/selection/explanatory.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.9/src/cefeste/selection/multivariate.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.9/src/cefeste/selection/univariate.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:24:36.616337 cefeste-1.1.9/src/cefeste/transform/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2801 2023-05-24 08:21:06.000000 cefeste-1.1.9/src/cefeste/transform/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-10 10:23:33.000000 cefeste-1.1.9/src/cefeste/utils.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-24 10:24:36.612336 cefeste-1.1.9/src/cefeste.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2683 2023-05-24 10:24:36.000000 cefeste-1.1.9/src/cefeste.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-24 10:24:36.000000 cefeste-1.1.9/src/cefeste.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-24 10:24:36.000000 cefeste-1.1.9/src/cefeste.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      131 2023-05-24 10:24:36.000000 cefeste-1.1.9/src/cefeste.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-24 10:24:36.000000 cefeste-1.1.9/src/cefeste.egg-info/top_level.txt
```

### Comparing `cefeste-1.1.8/LICENCE` & `cefeste-1.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.8/PKG-INFO` & `cefeste-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.8
+Version: 1.1.9
 Summary: Feature Selection and Elimination
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <4
```

### Comparing `cefeste-1.1.8/README.md` & `cefeste-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.8/pyproject.toml` & `cefeste-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cefeste"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   { name="DAT - Mattia Centurelli", email="mcenturelli@credem.it" },
 ]
 description = "Feature Selection and Elimination"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cefeste-1.1.8/setup.py` & `cefeste-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ce-feste",
-    version="1.1.8",
+    version="1.1.9",
     description="Package for Feature Selection, Transformation, Elimination",
     author="DAT/Mattia Centurelli",
     author_email="mcenturelli@credem.it",
     # url="https://dev.azure.com/credem-data/DAT/_git/ce-feste",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

### Comparing `cefeste-1.1.8/src/cefeste/__init__.py` & `cefeste-1.1.9/src/cefeste/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.8/src/cefeste/elimination/__init__.py` & `cefeste-1.1.9/src/cefeste/elimination/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.8/src/cefeste/elimination/shap_rfe.py` & `cefeste-1.1.9/src/cefeste/elimination/shap_rfe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import pandas as pd
 import numpy as np
-import shap
 from sklearn.metrics import roc_auc_score, r2_score, balanced_accuracy_score
 from sklearn.model_selection import RandomizedSearchCV, StratifiedKFold, GroupKFold
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.compose import ColumnTransformer
 import re
 from cefeste.utils import remove_features, time_step
 from functools import reduce
 import warnings
 
+try:
+    import shap
+except Exception:
+    warnings.warn("The usage of shap is not possible.")
+
 
 @time_step
 def Shap_RFE_full(
     X_train,
     y_train,
     model,
     grid,
```

### Comparing `cefeste-1.1.8/src/cefeste/selection/__init__.py` & `cefeste-1.1.9/src/cefeste/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.8/src/cefeste/selection/explanatory.py` & `cefeste-1.1.9/src/cefeste/selection/explanatory.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.8/src/cefeste/selection/multivariate.py` & `cefeste-1.1.9/src/cefeste/selection/multivariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.8/src/cefeste/selection/univariate.py` & `cefeste-1.1.9/src/cefeste/selection/univariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.8/src/cefeste/transform/__init__.py` & `cefeste-1.1.9/src/cefeste/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.8/src/cefeste/utils.py` & `cefeste-1.1.9/src/cefeste/utils.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.8/src/cefeste.egg-info/PKG-INFO` & `cefeste-1.1.9/src/cefeste.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.8
+Version: 1.1.9
 Summary: Feature Selection and Elimination
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <4
```

### Comparing `cefeste-1.1.8/src/cefeste.egg-info/SOURCES.txt` & `cefeste-1.1.9/src/cefeste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

