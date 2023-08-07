# Comparing `tmp/openprotein_python-0.2.1.tar.gz` & `tmp/openprotein_python-0.2.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openprotein_python-0.2.1.tar", max compression
+gzip compressed data, was "openprotein_python-0.2.1.post1.tar", max compression
```

## Comparing `openprotein_python-0.2.1.tar` & `openprotein_python-0.2.1.post1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     4851 2023-08-07 08:19:00.806389 openprotein_python-0.2.1/README.md
--rw-r--r--   0        0        0     2038 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/__init__.py
--rw-r--r--   0        0        0      215 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/_version.py
--rw-r--r--   0        0        0      127 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/__init__.py
--rw-r--r--   0        0        0    13237 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/data.py
--rw-r--r--   0        0        0     8533 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/design.py
--rw-r--r--   0        0        0    22209 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/embedding.py
--rw-r--r--   0        0        0    14511 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/jobs.py
--rw-r--r--   0        0        0    41899 2023-08-07 08:50:23.240291 openprotein_python-0.2.1/openprotein/api/poet.py
--rw-r--r--   0        0        0    17751 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/predict.py
--rw-r--r--   0        0        0    19453 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/train.py
--rw-r--r--   0        0        0     3069 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/base.py
--rw-r--r--   0        0        0      170 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/config.py
--rw-r--r--   0        0        0     1146 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/errors.py
--rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/fasta.py
--rw-r--r--   0        0        0     8620 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/models.py
--rw-r--r--   0        0        0      595 2023-08-07 08:51:46.732732 openprotein_python-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5581 1970-01-01 00:00:00.000000 openprotein_python-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1543 2023-08-07 09:39:52.360055 openprotein_python-0.2.1.post1/LICENSE.txt
+-rw-r--r--   0        0        0     4997 2023-08-07 09:51:46.711873 openprotein_python-0.2.1.post1/README.md
+-rw-r--r--   0        0        0     2038 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/__init__.py
+-rw-r--r--   0        0        0      215 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/_version.py
+-rw-r--r--   0        0        0      127 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/api/__init__.py
+-rw-r--r--   0        0        0    13237 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/api/data.py
+-rw-r--r--   0        0        0     8533 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/api/design.py
+-rw-r--r--   0        0        0    22209 2023-08-07 09:39:52.528056 openprotein_python-0.2.1.post1/openprotein/api/embedding.py
+-rw-r--r--   0        0        0    14511 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/api/jobs.py
+-rw-r--r--   0        0        0    41899 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/api/poet.py
+-rw-r--r--   0        0        0    17751 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/api/predict.py
+-rw-r--r--   0        0        0    19453 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/api/train.py
+-rw-r--r--   0        0        0     3069 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/base.py
+-rw-r--r--   0        0        0      170 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/config.py
+-rw-r--r--   0        0        0     1146 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/errors.py
+-rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.2.1.post1/openprotein/fasta.py
+-rw-r--r--   0        0        0     8620 2023-08-07 09:39:52.532056 openprotein_python-0.2.1.post1/openprotein/models.py
+-rw-r--r--   0        0        0      601 2023-08-07 10:05:47.616391 openprotein_python-0.2.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     5781 1970-01-01 00:00:00.000000 openprotein_python-0.2.1.post1/PKG-INFO
```

### Comparing `openprotein_python-0.2.1/LICENSE.txt` & `openprotein_python-0.2.1.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/README.md` & `openprotein_python-0.2.1.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 [![PyPI version](https://badge.fury.io/py/openprotein-python.svg)](https://pypi.org/project/openprotein-python/)
 [![Coverage](https://dev.docs.openprotein.ai/api-python/_images/coverage.svg)](https://pypi.org/project/openprotein-python/)
+[![Conda version](https://anaconda.org/openprotein/openprotein_python/badges/version.svg)](https://anaconda.org/openprotein/openprotein_python)
+
+
 # openprotein-python
 The OpenProtein.AI Python Interface provides a user-friendly library to interact with the OpenProtein.AI REST API, enabling various tasks related to protein analysis and modeling.
 
 ## Installation 
 
 To install the python interface using pip, run the following command: 
 ```
```

### Comparing `openprotein_python-0.2.1/openprotein/__init__.py` & `openprotein_python-0.2.1.post1/openprotein/__init__.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/openprotein/api/data.py` & `openprotein_python-0.2.1.post1/openprotein/api/data.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/openprotein/api/design.py` & `openprotein_python-0.2.1.post1/openprotein/api/design.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/openprotein/api/embedding.py` & `openprotein_python-0.2.1.post1/openprotein/api/embedding.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/openprotein/api/jobs.py` & `openprotein_python-0.2.1.post1/openprotein/api/jobs.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/openprotein/api/poet.py` & `openprotein_python-0.2.1.post1/openprotein/api/poet.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/openprotein/api/predict.py` & `openprotein_python-0.2.1.post1/openprotein/api/predict.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/openprotein/api/train.py` & `openprotein_python-0.2.1.post1/openprotein/api/train.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/openprotein/base.py` & `openprotein_python-0.2.1.post1/openprotein/base.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/openprotein/errors.py` & `openprotein_python-0.2.1.post1/openprotein/errors.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/openprotein/fasta.py` & `openprotein_python-0.2.1.post1/openprotein/fasta.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/openprotein/models.py` & `openprotein_python-0.2.1.post1/openprotein/models.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.1/pyproject.toml` & `openprotein_python-0.2.1.post1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "openprotein_python"
 packages = [{include = "openprotein"}]
-version = "0.2.1"
+version = "0.2.1.post1"
 description = "OpenProtein Python interface."
 license = "MIT"
 readme = "README.md"
 homepage = "https://docs.openprotein.ai/"
 authors = ["OpenProtein <info@ne47.bio>"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `openprotein_python-0.2.1/PKG-INFO` & `openprotein_python-0.2.1.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: openprotein-python
-Version: 0.2.1
+Version: 0.2.1.post1
 Summary: OpenProtein Python interface.
 Home-page: https://docs.openprotein.ai/
 License: MIT
 Author: OpenProtein
 Author-email: info@ne47.bio
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Requires-Dist: pandas (>=1)
 Requires-Dist: pydantic (>=1)
 Requires-Dist: requests (>=2)
 Requires-Dist: tqdm (>=4)
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/openprotein-python.svg)](https://pypi.org/project/openprotein-python/)
 [![Coverage](https://dev.docs.openprotein.ai/api-python/_images/coverage.svg)](https://pypi.org/project/openprotein-python/)
+[![Conda version](https://anaconda.org/openprotein/openprotein_python/badges/version.svg)](https://anaconda.org/openprotein/openprotein_python)
+
+
 # openprotein-python
 The OpenProtein.AI Python Interface provides a user-friendly library to interact with the OpenProtein.AI REST API, enabling various tasks related to protein analysis and modeling.
 
 ## Installation 
 
 To install the python interface using pip, run the following command: 
 ```
```

