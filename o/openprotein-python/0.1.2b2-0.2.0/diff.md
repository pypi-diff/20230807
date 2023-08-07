# Comparing `tmp/openprotein_python-0.1.2b2.tar.gz` & `tmp/openprotein_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openprotein_python-0.1.2b2.tar", max compression
+gzip compressed data, was "openprotein_python-0.2.0.tar", max compression
```

## Comparing `openprotein_python-0.1.2b2.tar` & `openprotein_python-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.1.2b2/LICENSE.txt
--rw-r--r--   0        0        0     4779 2023-08-04 09:20:47.647431 openprotein_python-0.1.2b2/README.md
--rw-r--r--   0        0        0     2038 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/__init__.py
--rw-r--r--   0        0        0      215 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/_version.py
--rw-r--r--   0        0        0      127 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/__init__.py
--rw-r--r--   0        0        0    13237 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/data.py
--rw-r--r--   0        0        0     8533 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/design.py
--rw-r--r--   0        0        0    22209 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/embedding.py
--rw-r--r--   0        0        0    14511 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/jobs.py
--rw-r--r--   0        0        0    41896 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/poet.py
--rw-r--r--   0        0        0    17751 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/predict.py
--rw-r--r--   0        0        0    19453 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/api/train.py
--rw-r--r--   0        0        0     3069 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/base.py
--rw-r--r--   0        0        0      170 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/config.py
--rw-r--r--   0        0        0     1146 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/errors.py
--rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/fasta.py
--rw-r--r--   0        0        0     8620 2023-08-04 09:17:01.541290 openprotein_python-0.1.2b2/openprotein/models.py
--rw-r--r--   0        0        0      597 2023-08-04 09:21:17.895719 openprotein_python-0.1.2b2/pyproject.toml
--rw-r--r--   0        0        0     5559 1970-01-01 00:00:00.000000 openprotein_python-0.1.2b2/PKG-INFO
+-rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4851 2023-08-07 08:19:00.806389 openprotein_python-0.2.0/README.md
+-rw-r--r--   0        0        0     2038 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/__init__.py
+-rw-r--r--   0        0        0      215 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/_version.py
+-rw-r--r--   0        0        0      127 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/__init__.py
+-rw-r--r--   0        0        0    13237 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/data.py
+-rw-r--r--   0        0        0     8533 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/design.py
+-rw-r--r--   0        0        0    22209 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/embedding.py
+-rw-r--r--   0        0        0    14511 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/jobs.py
+-rw-r--r--   0        0        0    41900 2023-08-07 08:12:44.252399 openprotein_python-0.2.0/openprotein/api/poet.py
+-rw-r--r--   0        0        0    17751 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/predict.py
+-rw-r--r--   0        0        0    19453 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/train.py
+-rw-r--r--   0        0        0     3069 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/base.py
+-rw-r--r--   0        0        0      170 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/config.py
+-rw-r--r--   0        0        0     1146 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/errors.py
+-rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/fasta.py
+-rw-r--r--   0        0        0     8620 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/models.py
+-rw-r--r--   0        0        0      595 2023-08-07 08:34:30.643273 openprotein_python-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5581 1970-01-01 00:00:00.000000 openprotein_python-0.2.0/PKG-INFO
```

### Comparing `openprotein_python-0.1.2b2/LICENSE.txt` & `openprotein_python-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/README.md` & `openprotein_python-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 
 ## Installation 
 
 To install the python interface using pip, run the following command: 
 ```
 pip install openprotein-python
 ```
+
+or with conda:
+```
+conda install -c openprotein openprotein-python
+```
 ## Requirements
 
 - Python 3.7 or higher.
 - pydantic version 1.0 or newer.
 - requests version 2.0 or newer.
 - tqdm version 4.0 or newer.
 - pandas version 1.0 or newer.
```

### Comparing `openprotein_python-0.1.2b2/openprotein/__init__.py` & `openprotein_python-0.2.0/openprotein/__init__.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/openprotein/api/data.py` & `openprotein_python-0.2.0/openprotein/api/data.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/openprotein/api/design.py` & `openprotein_python-0.2.0/openprotein/api/design.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/openprotein/api/embedding.py` & `openprotein_python-0.2.0/openprotein/api/embedding.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/openprotein/api/jobs.py` & `openprotein_python-0.2.0/openprotein/api/jobs.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/openprotein/api/poet.py` & `openprotein_python-0.2.0/openprotein/api/poet.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,19 +360,18 @@
 
     Returns
     -------
     PromptJob
         An object representing the status and results of the prompt job.
     """
 
-    endpoint = "v1/align/upload_prompt"
-
+    endpoint = "v1/poet/align/upload_prompt"
+    files = {"prompt_file ": prompt_file}
     try:
-        body = {"prompt_file": prompt_file}
-        response = session.post(endpoint, body=body)
+        response = session.post(endpoint, files=files)
         return PromptJob(**response.json())
     except Exception as exc:
         raise APIError(f"Failed to upload prompt post: {exc}") from exc
 
 
 def poet_score_post(
     session: APISession, prompt_id: str, queries: List[str]
```

### Comparing `openprotein_python-0.1.2b2/openprotein/api/predict.py` & `openprotein_python-0.2.0/openprotein/api/predict.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/openprotein/api/train.py` & `openprotein_python-0.2.0/openprotein/api/train.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/openprotein/base.py` & `openprotein_python-0.2.0/openprotein/base.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/openprotein/errors.py` & `openprotein_python-0.2.0/openprotein/errors.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/openprotein/fasta.py` & `openprotein_python-0.2.0/openprotein/fasta.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/openprotein/models.py` & `openprotein_python-0.2.0/openprotein/models.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.2b2/pyproject.toml` & `openprotein_python-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "openprotein_python"
 packages = [{include = "openprotein"}]
-version = "0.1.2b2"
+version = "0.2.0"
 description = "OpenProtein Python interface."
 license = "MIT"
 readme = "README.md"
 homepage = "https://docs.openprotein.ai/"
 authors = ["OpenProtein <info@ne47.bio>"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `openprotein_python-0.1.2b2/PKG-INFO` & `openprotein_python-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: openprotein-python
-Version: 0.1.2b2
+Version: 0.2.0
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
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: pandas (>=1)
 Requires-Dist: pydantic (>=1)
 Requires-Dist: requests (>=2)
 Requires-Dist: tqdm (>=4)
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/openprotein-python.svg)](https://pypi.org/project/openprotein-python/)
@@ -28,14 +27,19 @@
 
 ## Installation 
 
 To install the python interface using pip, run the following command: 
 ```
 pip install openprotein-python
 ```
+
+or with conda:
+```
+conda install -c openprotein openprotein-python
+```
 ## Requirements
 
 - Python 3.7 or higher.
 - pydantic version 1.0 or newer.
 - requests version 2.0 or newer.
 - tqdm version 4.0 or newer.
 - pandas version 1.0 or newer.
```

