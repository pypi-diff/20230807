# Comparing `tmp/openprotein_python-0.2.0.tar.gz` & `tmp/openprotein_python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openprotein_python-0.2.0.tar", max compression
+gzip compressed data, was "openprotein_python-0.2.1.tar", max compression
```

## Comparing `openprotein_python-0.2.0.tar` & `openprotein_python-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     4851 2023-08-07 08:19:00.806389 openprotein_python-0.2.0/README.md
--rw-r--r--   0        0        0     2038 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/__init__.py
--rw-r--r--   0        0        0      215 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/_version.py
--rw-r--r--   0        0        0      127 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/__init__.py
--rw-r--r--   0        0        0    13237 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/data.py
--rw-r--r--   0        0        0     8533 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/design.py
--rw-r--r--   0        0        0    22209 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/embedding.py
--rw-r--r--   0        0        0    14511 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/jobs.py
--rw-r--r--   0        0        0    41900 2023-08-07 08:12:44.252399 openprotein_python-0.2.0/openprotein/api/poet.py
--rw-r--r--   0        0        0    17751 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/predict.py
--rw-r--r--   0        0        0    19453 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/api/train.py
--rw-r--r--   0        0        0     3069 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/base.py
--rw-r--r--   0        0        0      170 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/config.py
--rw-r--r--   0        0        0     1146 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/errors.py
--rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/fasta.py
--rw-r--r--   0        0        0     8620 2023-08-04 09:17:01.541290 openprotein_python-0.2.0/openprotein/models.py
--rw-r--r--   0        0        0      595 2023-08-07 08:34:30.643273 openprotein_python-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5581 1970-01-01 00:00:00.000000 openprotein_python-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     4851 2023-08-07 08:19:00.806389 openprotein_python-0.2.1/README.md
+-rw-r--r--   0        0        0     2038 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/__init__.py
+-rw-r--r--   0        0        0      215 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/_version.py
+-rw-r--r--   0        0        0      127 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/__init__.py
+-rw-r--r--   0        0        0    13237 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/data.py
+-rw-r--r--   0        0        0     8533 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/design.py
+-rw-r--r--   0        0        0    22209 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/embedding.py
+-rw-r--r--   0        0        0    14511 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/jobs.py
+-rw-r--r--   0        0        0    41899 2023-08-07 08:50:23.240291 openprotein_python-0.2.1/openprotein/api/poet.py
+-rw-r--r--   0        0        0    17751 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/predict.py
+-rw-r--r--   0        0        0    19453 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/api/train.py
+-rw-r--r--   0        0        0     3069 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/base.py
+-rw-r--r--   0        0        0      170 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/config.py
+-rw-r--r--   0        0        0     1146 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/errors.py
+-rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/fasta.py
+-rw-r--r--   0        0        0     8620 2023-08-04 09:17:01.541290 openprotein_python-0.2.1/openprotein/models.py
+-rw-r--r--   0        0        0      595 2023-08-07 08:51:46.732732 openprotein_python-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5581 1970-01-01 00:00:00.000000 openprotein_python-0.2.1/PKG-INFO
```

### Comparing `openprotein_python-0.2.0/LICENSE.txt` & `openprotein_python-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/README.md` & `openprotein_python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/openprotein/__init__.py` & `openprotein_python-0.2.1/openprotein/__init__.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/openprotein/api/data.py` & `openprotein_python-0.2.1/openprotein/api/data.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/openprotein/api/design.py` & `openprotein_python-0.2.1/openprotein/api/design.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/openprotein/api/embedding.py` & `openprotein_python-0.2.1/openprotein/api/embedding.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/openprotein/api/jobs.py` & `openprotein_python-0.2.1/openprotein/api/jobs.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/openprotein/api/poet.py` & `openprotein_python-0.2.1/openprotein/api/poet.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
     Returns
     -------
     PromptJob
         An object representing the status and results of the prompt job.
     """
 
     endpoint = "v1/poet/align/upload_prompt"
-    files = {"prompt_file ": prompt_file}
+    files = {"prompt_file": prompt_file}
     try:
         response = session.post(endpoint, files=files)
         return PromptJob(**response.json())
     except Exception as exc:
         raise APIError(f"Failed to upload prompt post: {exc}") from exc
```

### Comparing `openprotein_python-0.2.0/openprotein/api/predict.py` & `openprotein_python-0.2.1/openprotein/api/predict.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/openprotein/api/train.py` & `openprotein_python-0.2.1/openprotein/api/train.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/openprotein/base.py` & `openprotein_python-0.2.1/openprotein/base.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/openprotein/errors.py` & `openprotein_python-0.2.1/openprotein/errors.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/openprotein/fasta.py` & `openprotein_python-0.2.1/openprotein/fasta.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/openprotein/models.py` & `openprotein_python-0.2.1/openprotein/models.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.2.0/pyproject.toml` & `openprotein_python-0.2.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "openprotein_python"
 packages = [{include = "openprotein"}]
-version = "0.2.0"
+version = "0.2.1"
 description = "OpenProtein Python interface."
 license = "MIT"
 readme = "README.md"
 homepage = "https://docs.openprotein.ai/"
 authors = ["OpenProtein <info@ne47.bio>"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `openprotein_python-0.2.0/PKG-INFO` & `openprotein_python-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openprotein-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: OpenProtein Python interface.
 Home-page: https://docs.openprotein.ai/
 License: MIT
 Author: OpenProtein
 Author-email: info@ne47.bio
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

