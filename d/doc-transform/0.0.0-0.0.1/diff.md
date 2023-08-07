# Comparing `tmp/doc-transform-0.0.0.tar.gz` & `tmp/doc-transform-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc-transform-0.0.0.tar", last modified: Mon Aug  7 19:16:16 2023, max compression
+gzip compressed data, was "doc-transform-0.0.1.tar", last modified: Mon Aug  7 19:19:44 2023, max compression
```

## Comparing `doc-transform-0.0.0.tar` & `doc-transform-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2023-08-07 19:16:16.183192 doc-transform-0.0.0/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1070 2023-08-02 18:52:02.000000 doc-transform-0.0.0/LICENSE
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      709 2023-08-07 19:16:16.183192 doc-transform-0.0.0/PKG-INFO
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      192 2023-08-02 19:09:50.000000 doc-transform-0.0.0/README.md
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2023-08-07 19:16:16.182192 doc-transform-0.0.0/doc_transform/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)        0 2023-08-02 18:53:04.000000 doc-transform-0.0.0/doc_transform/__init__.py
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2023-08-07 19:16:16.183192 doc-transform-0.0.0/doc_transform.egg-info/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      709 2023-08-07 19:16:16.000000 doc-transform-0.0.0/doc_transform.egg-info/PKG-INFO
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      248 2023-08-07 19:16:16.000000 doc-transform-0.0.0/doc_transform.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2023-08-07 19:16:16.000000 doc-transform-0.0.0/doc_transform.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       14 2023-08-07 19:16:16.000000 doc-transform-0.0.0/doc_transform.egg-info/top_level.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2023-08-07 19:14:27.000000 doc-transform-0.0.0/doc_transform.egg-info/zip-safe
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      112 2023-08-02 18:51:09.000000 doc-transform-0.0.0/pyproject.toml
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      637 2023-08-07 19:16:16.183192 doc-transform-0.0.0/setup.cfg
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2023-08-07 19:19:44.410509 doc-transform-0.0.1/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1070 2023-08-02 18:52:02.000000 doc-transform-0.0.1/LICENSE
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      715 2023-08-07 19:19:44.410509 doc-transform-0.0.1/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      198 2023-08-07 19:18:16.000000 doc-transform-0.0.1/README.md
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2023-08-07 19:19:44.409509 doc-transform-0.0.1/doc_transform/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)        0 2023-08-02 18:53:04.000000 doc-transform-0.0.1/doc_transform/__init__.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2023-08-07 19:19:44.410509 doc-transform-0.0.1/doc_transform.egg-info/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      715 2023-08-07 19:19:44.000000 doc-transform-0.0.1/doc_transform.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      248 2023-08-07 19:19:44.000000 doc-transform-0.0.1/doc_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2023-08-07 19:19:44.000000 doc-transform-0.0.1/doc_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       14 2023-08-07 19:19:44.000000 doc-transform-0.0.1/doc_transform.egg-info/top_level.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2023-08-07 19:14:27.000000 doc-transform-0.0.1/doc_transform.egg-info/zip-safe
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      112 2023-08-02 18:51:09.000000 doc-transform-0.0.1/pyproject.toml
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      637 2023-08-07 19:19:44.410509 doc-transform-0.0.1/setup.cfg
```

### Comparing `doc-transform-0.0.0/LICENSE` & `doc-transform-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doc-transform-0.0.0/PKG-INFO` & `doc-transform-0.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: doc-transform
-Version: 0.0.0
+Version: 0.0.1
 Summary: Transformations for text data to improve information retreval.
 Home-page: https://doc-transform.readthedocs.io/en/latest/
 Author: Jeremy McMinis
 Author-email: jeremy@sawtoothdata.com
 License: MIT
 Keywords: information retreival,large language models,semantic search
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Brainstorm
+# doc-transform
 
-Brainstorm is a python library used to improve information retreival performance primarily for RAG applications.
+doc-transform is a python library used to improve information retreival performance primarily for RAG applications.
 
 ## Get document summary
 
 ## Segment text
 
 ## Compute embeddings
```

### Comparing `doc-transform-0.0.0/doc_transform.egg-info/PKG-INFO` & `doc-transform-0.0.1/doc_transform.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: doc-transform
-Version: 0.0.0
+Version: 0.0.1
 Summary: Transformations for text data to improve information retreval.
 Home-page: https://doc-transform.readthedocs.io/en/latest/
 Author: Jeremy McMinis
 Author-email: jeremy@sawtoothdata.com
 License: MIT
 Keywords: information retreival,large language models,semantic search
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Brainstorm
+# doc-transform
 
-Brainstorm is a python library used to improve information retreival performance primarily for RAG applications.
+doc-transform is a python library used to improve information retreival performance primarily for RAG applications.
 
 ## Get document summary
 
 ## Segment text
 
 ## Compute embeddings
```

### Comparing `doc-transform-0.0.0/setup.cfg` & `doc-transform-0.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = doc-transform
-version = 0.0.0
+version = 0.0.1
 author = Jeremy McMinis
 author_email = jeremy@sawtoothdata.com
 url = https://doc-transform.readthedocs.io/en/latest/
 description = Transformations for text data to improve information retreval.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = information retreival, large language models, semantic search
```

