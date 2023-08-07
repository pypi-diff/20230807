# Comparing `tmp/stc-geck-1.3.4.tar.gz` & `tmp/stc-geck-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.3.4.tar", last modified: Tue Aug  1 14:43:04 2023, max compression
+gzip compressed data, was "stc-geck-1.3.5.tar", last modified: Mon Aug  7 17:12:04 2023, max compression
```

## Comparing `stc-geck-1.3.4.tar` & `stc-geck-1.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 14:43:04.371915 stc-geck-1.3.4/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.3.4/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-01 14:43:04.371614 stc-geck-1.3.4/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)     6985 2023-07-23 19:18:57.000000 stc-geck-1.3.4/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-08-01 14:41:13.000000 stc-geck-1.3.4/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      161 2023-07-30 14:20:06.000000 stc-geck-1.3.4/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 14:43:04.372036 stc-geck-1.3.4/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 14:43:04.368168 stc-geck-1.3.4/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-19 19:56:31.000000 stc-geck-1.3.4/stc_geck/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)      923 2023-07-06 11:45:56.000000 stc-geck-1.3.4/stc_geck/advices.py
--rw-r--r--   0 pasha      (501) staff       (20)     7346 2023-07-23 18:24:49.000000 stc-geck-1.3.4/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     7231 2023-07-23 18:24:49.000000 stc-geck-1.3.4/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1877 2023-07-22 08:16:03.000000 stc-geck-1.3.4/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 14:43:04.371119 stc-geck-1.3.4/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      341 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      162 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-08-01 14:43:04.000000 stc-geck-1.3.4/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 17:12:04.986117 stc-geck-1.3.5/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.3.5/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-07 17:12:04.985904 stc-geck-1.3.5/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     6985 2023-07-23 19:18:57.000000 stc-geck-1.3.5/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-08-07 17:11:41.000000 stc-geck-1.3.5/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      161 2023-07-30 14:20:06.000000 stc-geck-1.3.5/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-07 17:12:04.986201 stc-geck-1.3.5/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 17:12:04.983183 stc-geck-1.3.5/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-19 19:56:31.000000 stc-geck-1.3.5/stc_geck/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1451 2023-08-07 17:11:41.000000 stc-geck-1.3.5/stc_geck/advices.py
+-rw-r--r--   0 pasha      (501) staff       (20)     7337 2023-08-06 13:26:45.000000 stc-geck-1.3.5/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     7257 2023-08-07 14:38:25.000000 stc-geck-1.3.5/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1877 2023-07-22 08:16:03.000000 stc-geck-1.3.5/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 17:12:04.985527 stc-geck-1.3.5/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      341 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      162 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-08-07 17:12:04.000000 stc-geck-1.3.5/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.3.4/PKG-INFO` & `stc-geck-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.3.4
+Version: 1.3.5
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `stc-geck-1.3.4/README.md` & `stc-geck-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `stc-geck-1.3.4/pyproject.toml` & `stc-geck-1.3.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.3.4"
+version = "1.3.5"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.3.4/stc_geck/cli.py` & `stc-geck-1.3.5/stc_geck/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             timeout=timeout,
         )
         self.grpc_api_endpoint = grpc_api_endpoint
         self.index_name = index_name
 
     async def documents(self):
         """
-        Stream all STC documents.
+        Stream all STC chunks.
 
         :return: metadata records
         """
         print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_name}...")
         async with self.geck as geck:
             async for document in geck.get_summa_client().documents(self.index_name):
                 print(document)
@@ -147,15 +147,15 @@
         self,
         output_car: str,
         query: str = None,
         limit: int = 100,
         name_template: str = '{id}.{extension}',
     ):
         """
-        Stream all STC documents.
+        Stream all STC chunks.
 
         :return: metadata records
         """
         print(f"{colored('INFO', 'green')}: Setting up indices: {self.index_name}...")
         async with self.geck as geck:
             return await geck.create_ipfs_directory(self.index_name, output_car, query, limit, name_template)
 
@@ -186,15 +186,15 @@
         index_name=index_name,
         grpc_api_endpoint=grpc_api_endpoint,
         timeout=timeout,
     )
     return {
         'create-ipfs-directory': stc_geck_client.create_ipfs_directory,
         'download': stc_geck_client.download,
-        'documents': stc_geck_client.documents,
+        'chunks': stc_geck_client.documents,
         'random-cids': stc_geck_client.random_cids,
         'search': stc_geck_client.search,
         'serve': stc_geck_client.serve,
     }
 
 
 def main():
```

### Comparing `stc-geck-1.3.4/stc_geck/client.py` & `stc-geck-1.3.5/stc_geck/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,24 @@
 from urllib.parse import urlparse
 
 import aiohttp
 import orjson
 import summa_embed
 from aiokit import AioThing
 from aiosumma import SummaClient
-from izihawa_ipfs_api import IpfsApiClient, IpfsHttpClient
+from izihawa_ipfs_api import (
+    IpfsApiClient,
+    IpfsHttpClient,
+)
 from izihawa_utils.random import reservoir_sampling_async
 
-from .utils import create_car, is_endpoint_listening
+from .utils import (
+    create_car,
+    is_endpoint_listening,
+)
 
 
 def get_config():
     return {
         'debug': True,
         'api': {
             'http_endpoint': None,
```

### Comparing `stc-geck-1.3.4/stc_geck/utils.py` & `stc-geck-1.3.5/stc_geck/utils.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.3.4/stc_geck.egg-info/PKG-INFO` & `stc-geck-1.3.5/stc_geck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.3.4
+Version: 1.3.5
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

