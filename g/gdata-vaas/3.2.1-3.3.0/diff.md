# Comparing `tmp/gdata-vaas-3.2.1.tar.gz` & `tmp/gdata-vaas-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdata-vaas-3.2.1.tar", last modified: Wed Jul 19 08:02:53 2023, max compression
+gzip compressed data, was "gdata-vaas-3.3.0.tar", last modified: Mon Aug  7 10:10:04 2023, max compression
```

## Comparing `gdata-vaas-3.2.1.tar` & `gdata-vaas-3.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:02:53.757228 gdata-vaas-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-07-19 08:02:53.757228 gdata-vaas-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-19 08:02:53.757228 gdata-vaas-3.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:02:53.753228 gdata-vaas-3.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:02:53.753228 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-07-19 08:02:53.000000 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-07-19 08:02:53.000000 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 08:02:53.000000 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-19 08:02:53.000000 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-19 08:02:53.000000 gdata-vaas-3.2.1/src/gdata_vaas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:02:53.753228 gdata-vaas-3.2.1/src/vaas/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/src/vaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      938 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/src/vaas/client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11337 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/src/vaas/vaas.py
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/src/vaas/vaas_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 08:02:53.757228 gdata-vaas-3.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/tests/test_client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-07-19 08:02:04.000000 gdata-vaas-3.2.1/tests/test_vaas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 10:10:04.935415 gdata-vaas-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-08-07 10:10:04.000000 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-08-07 10:10:04.000000 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-07 10:10:04.000000 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-08-07 10:10:04.000000 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-07 10:10:04.000000 gdata-vaas-3.3.0/src/gdata_vaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/src/vaas/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/src/vaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/src/vaas/client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11419 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/src/vaas/vaas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/src/vaas/vaas_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 10:10:04.939415 gdata-vaas-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/tests/test_client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-08-07 10:09:12.000000 gdata-vaas-3.3.0/tests/test_vaas.py
```

### Comparing `gdata-vaas-3.2.1/LICENSE` & `gdata-vaas-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.2.1/PKG-INFO` & `gdata-vaas-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 3.2.1
+Version: 3.3.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-3.2.1/README.md` & `gdata-vaas-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.2.1/setup.cfg` & `gdata-vaas-3.3.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdata-vaas
-version = 3.2.1
+version = 3.3.0
 author = G DATA CyberDefense AG
 author_email = oem@gdata.de
 description = gdata-vaas is a Python library for the VaaS-API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GDATASoftwareAG/vaas/tree/main/python
 project_urls = 
@@ -15,15 +15,15 @@
 	Operating System :: OS Independent
 
 [options]
 python_requires = >=3.8
 install_requires = 
 	websockets ==10.4
 	httpx[http2] ==0.24.1
-	jwt == 1.3.1
+	pyjwt == 2.3.0
 	authlib ==1.2.1
 	aiofiles==23.1.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `gdata-vaas-3.2.1/src/gdata_vaas.egg-info/PKG-INFO` & `gdata-vaas-3.3.0/src/gdata_vaas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 3.2.1
+Version: 3.3.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-3.2.1/src/vaas/__init__.py` & `gdata-vaas-3.3.0/src/vaas/__init__.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.2.1/src/vaas/client_credentials_grant_authenticator.py` & `gdata-vaas-3.3.0/src/vaas/client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.2.1/src/vaas/vaas.py` & `gdata-vaas-3.3.0/src/vaas/vaas.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import uuid
 from typing import Optional
 import asyncio
 from asyncio import Future
 import ssl
 from urllib.parse import urlparse
 import aiofiles
-from jwt import JWT
+from jwt import PyJWT
 import httpx
 import websockets.client
 from .vaas_errors import (
     VaasInvalidStateError,
     VaasConnectionClosedError,
     VaasTimeoutError,
 )
@@ -101,15 +101,15 @@
         self.session_id = None
         self.results = {}
         self.httpx_client: Optional[httpx.AsyncClient] = None
         self.options = options
         self.url = url
 
     def get_authenticated_websocket(self):
-        """Get authenticated websocket"""        
+        """Get authenticated websocket"""
         if self.websocket is None:
             raise VaasInvalidStateError("connect() was not called")
         if not self.websocket.open:
             raise VaasConnectionClosedError(
                 "connection closed or connect() was not awaited"
             )
         if self.session_id is None:
@@ -154,15 +154,17 @@
         return self
 
     async def __aexit__(self, exc_type, exc, traceback):
         await self.close()
 
     async def for_sha256(self, sha256, verdict_request_attributes=None, guid=None):
         """Returns the verdict for a SHA256 checksum"""
-        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes, guid)
+        verdict_response = await self.__for_sha256(
+            sha256, verdict_request_attributes, guid
+        )
         return {
             "Sha256": verdict_response.get("sha256"),
             "Guid": verdict_response.get("guid"),
             "Verdict": verdict_response.get("verdict"),
         }
 
     async def __for_sha256(self, sha256, verdict_request_attributes=None, guid=None):
@@ -217,15 +219,17 @@
         """Returns the verdict for a buffer"""
 
         loop = asyncio.get_running_loop()
         sha256 = await loop.run_in_executor(
             None, lambda: hashlib.sha256(buffer).hexdigest()
         )
 
-        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes, guid)
+        verdict_response = await self.__for_sha256(
+            sha256, verdict_request_attributes, guid
+        )
         verdict = verdict_response.get("verdict")
 
         if verdict == "Unknown":
             verdict_response = await self._for_unknown_buffer(
                 verdict_response, buffer, len(buffer)
             )
 
@@ -252,15 +256,17 @@
 
     async def for_file(self, path, verdict_request_attributes=None, guid=None):
         """Returns the verdict for a file"""
 
         loop = asyncio.get_running_loop()
         sha256 = await loop.run_in_executor(None, lambda: hash_file(path))
 
-        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes, guid)
+        verdict_response = await self.__for_sha256(
+            sha256, verdict_request_attributes, guid
+        )
         verdict = verdict_response.get("verdict")
 
         if verdict == "Unknown":
             async with aiofiles.open(path, mode="rb") as file:
                 buffer = await file.read()
                 verdict_response = await self._for_unknown_buffer(
                     verdict_response, buffer, len(buffer)
@@ -269,16 +275,16 @@
         return {
             "Sha256": verdict_response.get("sha256"),
             "Guid": verdict_response.get("guid"),
             "Verdict": verdict_response.get("verdict"),
         }
 
     async def __upload(self, token, upload_uri, buffer_or_file, content_length):
-        jwt = JWT()
-        decoded_token = jwt.decode(token, do_verify=False)
+        jwt = PyJWT()
+        decoded_token = jwt.decode(token, options={"verify_signature": False})
         trace_id = decoded_token.get("traceId")
         try:
             await self.httpx_client.put(
                 url=upload_uri,
                 content=buffer_or_file,
                 headers={
                     "Authorization": token,
```

### Comparing `gdata-vaas-3.2.1/tests/test_client_credentials_grant_authenticator.py` & `gdata-vaas-3.3.0/tests/test_client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.2.1/tests/test_vaas.py` & `gdata-vaas-3.3.0/tests/test_vaas.py`

 * *Files identical despite different names*

