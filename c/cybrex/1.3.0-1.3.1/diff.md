# Comparing `tmp/cybrex-1.3.0.tar.gz` & `tmp/cybrex-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.3.0.tar", last modified: Mon Aug  7 13:44:11 2023, max compression
+gzip compressed data, was "cybrex-1.3.1.tar", last modified: Mon Aug  7 13:54:20 2023, max compression
```

## Comparing `cybrex-1.3.0.tar` & `cybrex-1.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.015717 cybrex-1.3.0/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.3.0/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 13:44:11.015448 cybrex-1.3.0/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.3.0/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.011270 cybrex-1.3.0/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.3.0/cybrex/__init__.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.013787 cybrex-1.3.0/cybrex/chains/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.0/cybrex/chains/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.3.0/cybrex/chains/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2381 2023-08-07 13:01:11.000000 cybrex-1.3.0/cybrex/chains/map_reduce.py
--rw-r--r--   0 pasha      (501) staff       (20)     5550 2023-08-07 10:16:43.000000 cybrex-1.3.0/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    10794 2023-08-07 13:42:48.000000 cybrex-1.3.0/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)     1676 2023-08-05 19:44:06.000000 cybrex-1.3.0/cybrex/document_chunker.py
--rw-r--r--   0 pasha      (501) staff       (20)     4830 2023-08-07 11:07:40.000000 cybrex-1.3.0/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.014262 cybrex-1.3.0/cybrex/prompts/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.0/cybrex/prompts/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     9756 2023-08-07 13:43:38.000000 cybrex-1.3.0/cybrex/prompts/base.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.015014 cybrex-1.3.0/cybrex/vector_storage/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.0/cybrex/vector_storage/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)      206 2023-08-07 13:42:48.000000 cybrex-1.3.0/cybrex/vector_storage/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2987 2023-08-07 12:50:10.000000 cybrex-1.3.0/cybrex/vector_storage/chroma.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:44:11.013079 cybrex-1.3.0/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 13:44:10.000000 cybrex-1.3.0/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      554 2023-08-07 13:44:11.000000 cybrex-1.3.0/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-07 13:44:11.000000 cybrex-1.3.0/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-07 13:44:11.000000 cybrex-1.3.0/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-07 13:44:11.000000 cybrex-1.3.0/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-07 13:44:11.000000 cybrex-1.3.0/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-07 13:43:56.000000 cybrex-1.3.0/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.3.0/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-07 13:44:11.015817 cybrex-1.3.0/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.930799 cybrex-1.3.1/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.3.1/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 13:54:20.930512 cybrex-1.3.1/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.3.1/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.924952 cybrex-1.3.1/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.3.1/cybrex/__init__.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.928617 cybrex-1.3.1/cybrex/chains/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.1/cybrex/chains/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.3.1/cybrex/chains/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2381 2023-08-07 13:01:11.000000 cybrex-1.3.1/cybrex/chains/map_reduce.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5564 2023-08-07 13:54:06.000000 cybrex-1.3.1/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    10794 2023-08-07 13:42:48.000000 cybrex-1.3.1/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1676 2023-08-05 19:44:06.000000 cybrex-1.3.1/cybrex/document_chunker.py
+-rw-r--r--   0 pasha      (501) staff       (20)     4830 2023-08-07 11:07:40.000000 cybrex-1.3.1/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.929139 cybrex-1.3.1/cybrex/prompts/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.1/cybrex/prompts/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     9756 2023-08-07 13:43:38.000000 cybrex-1.3.1/cybrex/prompts/base.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.930033 cybrex-1.3.1/cybrex/vector_storage/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.1/cybrex/vector_storage/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)      206 2023-08-07 13:42:48.000000 cybrex-1.3.1/cybrex/vector_storage/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2987 2023-08-07 12:50:10.000000 cybrex-1.3.1/cybrex/vector_storage/chroma.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.927754 cybrex-1.3.1/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      554 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-07 13:54:09.000000 cybrex-1.3.1/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.3.1/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-07 13:54:20.930904 cybrex-1.3.1/setup.cfg
```

### Comparing `cybrex-1.3.0/PKG-INFO` & `cybrex-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.3.0
+Version: 1.3.1
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.3.0/README.md` & `cybrex-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.0/cybrex/chains/map_reduce.py` & `cybrex-1.3.1/cybrex/chains/map_reduce.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.0/cybrex/cli.py` & `cybrex-1.3.1/cybrex/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,37 +20,37 @@
 
     async def add_all_documents(self):
         async with self.cybrex as cybrex:
             async for document in cybrex.geck.get_summa_client().documents('nexus_science'):
                 document = json.loads(document)
                 await self.cybrex.add_full_documents([document])
 
-    async def dump_texts(self, query: str, output_path: str, n_documents: int = 100):
+    async def export_chunks(self, query: str, output_path: str, n_documents: int = 100):
         """
         Store STC text chunks in ZIP archive
 
         :param query: query to STC
         :param output_path: where to store result
         :param n_documents: the number of chunks to extract
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Q', 'green')}: {query}")
-            await cybrex.export_texts(
+            await cybrex.export_chunks(
                 query=query,
                 output_path=output_path,
                 n_documents=n_documents
             )
 
-    async def import_texts(self, input_path: str):
+    async def import_chunks(self, input_path: str):
         """
         Import binary file with embeddings
 
         :param input_path:
         """
-        await self.cybrex.import_texts(input_path=input_path)
+        await self.cybrex.import_chunks(input_path=input_path)
 
     async def chat_doc(self, field: str, value: str, question: str, n_chunks: int = 4):
         """
         Ask a question about content of document identified by DOI.
 
         :param field: name of the field in document used for selection
         :param value: value of the field in document used for selection
@@ -135,16 +135,16 @@
     """
     logging.basicConfig(stream=sys.stdout, level=logging.INFO if debug else logging.ERROR)
     cybrex_ai = CybrexCli()
     return {
         'add-all-chunks': cybrex_ai.add_all_documents,
         'chat-doc': cybrex_ai.chat_doc,
         'chat-sci': cybrex_ai.chat_sci,
-        'dump-texts': cybrex_ai.dump_texts,
-        'import-texts': cybrex_ai.import_texts,
+        'export-chunks': cybrex_ai.export_chunks,
+        'import-chunks': cybrex_ai.import_chunks,
         'semantic-search': cybrex_ai.semantic_search,
         'sum-doc': cybrex_ai.sum_doc,
     }
 
 
 def main():
     fire.Fire(cybrex_cli, name='cybrex')
```

### Comparing `cybrex-1.3.0/cybrex/cybrex_ai.py` & `cybrex-1.3.1/cybrex/cybrex_ai.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.0/cybrex/document_chunker.py` & `cybrex-1.3.1/cybrex/document_chunker.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.0/cybrex/models.py` & `cybrex-1.3.1/cybrex/models.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.0/cybrex/prompts/base.py` & `cybrex-1.3.1/cybrex/prompts/base.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.0/cybrex/vector_storage/chroma.py` & `cybrex-1.3.1/cybrex/vector_storage/chroma.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.0/cybrex.egg-info/PKG-INFO` & `cybrex-1.3.1/cybrex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.3.0
+Version: 1.3.1
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.3.0/cybrex.egg-info/SOURCES.txt` & `cybrex-1.3.1/cybrex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.0/pyproject.toml` & `cybrex-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.3.0"
+version = "1.3.1"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

