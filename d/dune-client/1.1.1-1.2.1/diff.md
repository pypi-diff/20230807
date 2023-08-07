# Comparing `tmp/dune_client-1.1.1.tar.gz` & `tmp/dune_client-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_client-1.1.1.tar", last modified: Mon Jun  5 15:33:58 2023, max compression
+gzip compressed data, was "dune_client-1.2.1.tar", last modified: Mon Aug  7 20:57:15 2023, max compression
```

## Comparing `dune_client-1.1.1.tar` & `dune_client-1.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 15:33:40.000000 dune_client-1.1.1/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.327243 dune_client-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.331243 dune_client-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-05 15:33:40.000000 dune_client-1.1.1/.github/workflows/cla.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 15:33:40.000000 dune_client-1.1.1/.github/workflows/pull-request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-05 15:33:40.000000 dune_client-1.1.1/.github/workflows/py-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 15:33:40.000000 dune_client-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 15:33:40.000000 dune_client-1.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 15:33:40.000000 dune_client-1.1.1/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 15:33:40.000000 dune_client-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-05 15:33:40.000000 dune_client-1.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-05 15:33:58.335243 dune_client-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-05 15:33:40.000000 dune_client-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/dune_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/client_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/dune_client/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/file/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 15:33:40.000000 dune_client-1.1.1/dune_client/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/dune_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 15:33:58.000000 dune_client-1.1.1/dune_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-05 15:33:40.000000 dune_client-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-05 15:33:40.000000 dune_client-1.1.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 15:33:40.000000 dune_client-1.1.1/requirements/prod.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-05 15:33:58.339243 dune_client-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 15:33:40.000000 dune_client-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.327243 dune_client-1.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/e2e/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/e2e/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:33:58.335243 dune_client-1.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/unit/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/unit/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-05 15:33:40.000000 dune_client-1.1.1/tests/unit/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:57:15.705750 dune_client-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 20:56:59.000000 dune_client-1.2.1/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:57:15.693750 dune_client-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:57:15.697750 dune_client-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-07 20:56:59.000000 dune_client-1.2.1/.github/workflows/cla.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-08-07 20:56:59.000000 dune_client-1.2.1/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-07 20:56:59.000000 dune_client-1.2.1/.github/workflows/py-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 20:56:59.000000 dune_client-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 20:56:59.000000 dune_client-1.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-07 20:56:59.000000 dune_client-1.2.1/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 20:56:59.000000 dune_client-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-07 20:56:59.000000 dune_client-1.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-07 20:57:15.705750 dune_client-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-07 20:56:59.000000 dune_client-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:57:15.701750 dune_client-1.2.1/dune_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/client_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:57:15.701750 dune_client-1.2.1/dune_client/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/file/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-07 20:56:59.000000 dune_client-1.2.1/dune_client/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:57:15.701750 dune_client-1.2.1/dune_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-07 20:57:15.000000 dune_client-1.2.1/dune_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-07 20:57:15.000000 dune_client-1.2.1/dune_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:57:15.000000 dune_client-1.2.1/dune_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:57:15.000000 dune_client-1.2.1/dune_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-07 20:57:15.000000 dune_client-1.2.1/dune_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 20:57:15.000000 dune_client-1.2.1/dune_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-07 20:56:59.000000 dune_client-1.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:57:15.701750 dune_client-1.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-07 20:56:59.000000 dune_client-1.2.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-07 20:56:59.000000 dune_client-1.2.1/requirements/prod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-07 20:57:15.705750 dune_client-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 20:56:59.000000 dune_client-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:57:15.693750 dune_client-1.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:57:15.701750 dune_client-1.2.1/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-07 20:56:59.000000 dune_client-1.2.1/tests/e2e/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-08-07 20:56:59.000000 dune_client-1.2.1/tests/e2e/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:57:15.705750 dune_client-1.2.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-08-07 20:56:59.000000 dune_client-1.2.1/tests/unit/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-08-07 20:56:59.000000 dune_client-1.2.1/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-07 20:56:59.000000 dune_client-1.2.1/tests/unit/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-07 20:56:59.000000 dune_client-1.2.1/tests/unit/test_types.py
```

### Comparing `dune_client-1.1.1/.github/workflows/cla.yaml` & `dune_client-1.2.1/.github/workflows/cla.yaml`

 * *Files identical despite different names*

### Comparing `dune_client-1.1.1/.github/workflows/pull-request.yaml` & `dune_client-1.2.1/.github/workflows/pull-request.yaml`

 * *Files identical despite different names*

### Comparing `dune_client-1.1.1/.github/workflows/py-publish.yaml` & `dune_client-1.2.1/.github/workflows/py-publish.yaml`

 * *Files identical despite different names*

### Comparing `dune_client-1.1.1/LICENSE` & `dune_client-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_client-1.1.1/Makefile` & `dune_client-1.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `dune_client-1.1.1/PKG-INFO` & `dune_client-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune_client
-Version: 1.1.1
+Version: 1.2.1
 Summary: A simple framework for interacting with Dune Analytics official API service.
 Home-page: https://github.com/cowprotocol/dune-client
 Author: Benjamin H. Smith
 Author-email: ben@cow.fi
 License: Apache License Version 2.0
 Project-URL: Tracker, https://github.com/cowprotocol/dune-client/issues
 Classifier: Programming Language :: Python :: 3
@@ -34,17 +34,17 @@
 
 ```python
 import dotenv
 import os
 
 from dune_client.types import QueryParameter
 from dune_client.client import DuneClient
-from dune_client.query import Query
+from dune_client.query import QueryBase
 
-query = Query(
+query = QueryBase(
     name="Sample Query",
     query_id=1215383,
     params=[
         QueryParameter.text_type(name="TextField", value="Word"),
         QueryParameter.number_type(name="NumberField", value=3.1415926535),
         QueryParameter.date_type(name="DateField", value="2022-05-04 00:00:00"),
         QueryParameter.enum_type(name="EnumField", value="Option 1"),
```

### Comparing `dune_client-1.1.1/README.md` & `dune_client-1.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 ```python
 import dotenv
 import os
 
 from dune_client.types import QueryParameter
 from dune_client.client import DuneClient
-from dune_client.query import Query
+from dune_client.query import QueryBase
 
-query = Query(
+query = QueryBase(
     name="Sample Query",
     query_id=1215383,
     params=[
         QueryParameter.text_type(name="TextField", value="Word"),
         QueryParameter.number_type(name="NumberField", value=3.1415926535),
         QueryParameter.date_type(name="DateField", value="2022-05-04 00:00:00"),
         QueryParameter.enum_type(name="EnumField", value="Option 1"),
```

### Comparing `dune_client-1.1.1/dune_client/client.py` & `dune_client-1.2.1/dune_client/client_async.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,240 +1,288 @@
 """"
-Basic Dune Client Class responsible for refreshing Dune Queries
+Async Dune Client Class responsible for refreshing Dune Queries
 Framework built on Dune's API Documentation
 https://duneanalytics.notion.site/API-Documentation-1b93d16e0fa941398e15047f643e003a
 """
 from __future__ import annotations
 
-import time
+import asyncio
 from io import BytesIO
 from typing import Any, Optional, Union
 
-import requests
-from requests import Response, JSONDecodeError
+from aiohttp import (
+    ClientSession,
+    ClientResponse,
+    ContentTypeError,
+    TCPConnector,
+    ClientTimeout,
+)
 
 from dune_client.base_client import BaseDuneClient
-from dune_client.interface import DuneInterface
 from dune_client.models import (
     ExecutionResponse,
     ExecutionResultCSV,
     DuneError,
     QueryFailed,
     ExecutionStatusResponse,
     ResultsResponse,
     ExecutionState,
 )
 
-from dune_client.query import Query
+from dune_client.query import QueryBase
 
 
-class DuneClient(DuneInterface, BaseDuneClient):
+# pylint: disable=duplicate-code
+class AsyncDuneClient(BaseDuneClient):
     """
-    An interface for Dune API with a few convenience methods
+    An asynchronous interface for Dune API with a few convenience methods
     combining the use of endpoints (e.g. refresh)
     """
 
-    def _handle_response(
-        self,
-        response: Response,
-    ) -> Any:
+    _connection_limit = 3
+
+    def __init__(
+        self, api_key: str, connection_limit: int = 3, performance: str = "medium"
+    ):
+        """
+        api_key - Dune API key
+        connection_limit - number of parallel requests to execute.
+        For non-pro accounts Dune allows only up to 3 requests but that number can be increased.
+        """
+        super().__init__(api_key=api_key, performance=performance)
+        self._connection_limit = connection_limit
+        self._session: Optional[ClientSession] = None
+
+    async def _create_session(self) -> ClientSession:
+        conn = TCPConnector(limit=self._connection_limit)
+        return ClientSession(
+            connector=conn,
+            base_url=self.BASE_URL,
+            timeout=ClientTimeout(total=self.DEFAULT_TIMEOUT),
+        )
+
+    async def connect(self) -> None:
+        """Opens a client session (can be used instead of async with)"""
+        self._session = await self._create_session()
+
+    async def disconnect(self) -> None:
+        """Closes client session"""
+        if self._session:
+            await self._session.close()
+
+    async def __aenter__(self) -> AsyncDuneClient:
+        self._session = await self._create_session()
+        return self
+
+    async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
+        await self.disconnect()
+
+    async def _handle_response(self, response: ClientResponse) -> Any:
         try:
             # Some responses can be decoded and converted to DuneErrors
-            response_json = response.json()
+            response_json = await response.json()
             self.logger.debug(f"received response {response_json}")
             return response_json
-        except JSONDecodeError as err:
+        except ContentTypeError as err:
             # Others can't. Only raise HTTP error for not decodable errors
             response.raise_for_status()
             raise ValueError("Unreachable since previous line raises") from err
 
     def _route_url(self, route: str) -> str:
-        return f"{self.BASE_URL}{self.API_PATH}/{route}"
+        return f"{self.api_version}{route}"
 
-    def _get(self, route: str, params: Optional[Any] = None) -> Any:
+    async def _get(
+        self,
+        route: str,
+        params: Optional[Any] = None,
+        raw: bool = False,
+    ) -> Any:
         url = self._route_url(route)
+        if self._session is None:
+            raise ValueError("Client is not connected; call `await cl.connect()`")
         self.logger.debug(f"GET received input url={url}")
-        response = requests.get(
-            url,
-            headers={"x-dune-api-key": self.token},
-            timeout=self.DEFAULT_TIMEOUT,
+        response = await self._session.get(
+            url=url,
+            headers=self.default_headers(),
             params=params,
         )
-        return self._handle_response(response)
+        if raw:
+            return response
+        return await self._handle_response(response)
 
-    def _post(self, route: str, params: Any) -> Any:
+    async def _post(self, route: str, params: Any) -> Any:
         url = self._route_url(route)
+        if self._session is None:
+            raise ValueError("Client is not connected; call `await cl.connect()`")
         self.logger.debug(f"POST received input url={url}, params={params}")
-        response = requests.post(
+        response = await self._session.post(
             url=url,
             json=params,
-            headers={"x-dune-api-key": self.token},
-            timeout=self.DEFAULT_TIMEOUT,
+            headers=self.default_headers(),
         )
-        return self._handle_response(response)
+        return await self._handle_response(response)
 
-    def execute(
-        self, query: Query, performance: Optional[str] = None
+    async def execute(
+        self, query: QueryBase, performance: Optional[str] = None
     ) -> ExecutionResponse:
         """Post's to Dune API for execute `query`"""
+        params = query.request_format()
+        params["performance"] = performance or self.performance
+
         self.logger.info(
             f"executing {query.query_id} on {performance or self.performance} cluster"
         )
-        response_json = self._post(
-            route=f"query/{query.query_id}/execute",
-            params={
-                "query_parameters": {
-                    p.key: p.to_dict()["value"] for p in query.parameters()
-                },
-                "performance": performance or self.performance,
-            },
+        response_json = await self._post(
+            route=f"/query/{query.query_id}/execute",
+            params=params,
         )
         try:
             return ExecutionResponse.from_dict(response_json)
         except KeyError as err:
             raise DuneError(response_json, "ExecutionResponse", err) from err
 
-    def get_status(self, job_id: str) -> ExecutionStatusResponse:
+    async def get_status(self, job_id: str) -> ExecutionStatusResponse:
         """GET status from Dune API for `job_id` (aka `execution_id`)"""
-        response_json = self._get(
-            route=f"execution/{job_id}/status",
-        )
+        response_json = await self._get(route=f"/execution/{job_id}/status")
         try:
             return ExecutionStatusResponse.from_dict(response_json)
         except KeyError as err:
             raise DuneError(response_json, "ExecutionStatusResponse", err) from err
 
-    def get_result(self, job_id: str) -> ResultsResponse:
+    async def get_result(self, job_id: str) -> ResultsResponse:
         """GET results from Dune API for `job_id` (aka `execution_id`)"""
-        response_json = self._get(route=f"execution/{job_id}/results")
+        response_json = await self._get(route=f"/execution/{job_id}/results")
         try:
             return ResultsResponse.from_dict(response_json)
         except KeyError as err:
             raise DuneError(response_json, "ResultsResponse", err) from err
 
-    def get_result_csv(self, job_id: str) -> ExecutionResultCSV:
+    async def get_result_csv(self, job_id: str) -> ExecutionResultCSV:
         """
         GET results in CSV format from Dune API for `job_id` (aka `execution_id`)
 
         this API only returns the raw data in CSV format, it is faster & lighterweight
         use this method for large results where you want lower CPU and memory overhead
         if you need metadata information use get_results() or get_status()
         """
-        url = self._route_url(f"execution/{job_id}/results/csv")
+        route = f"/execution/{job_id}/results/csv"
+        url = self._route_url(f"/execution/{job_id}/results/csv")
         self.logger.debug(f"GET CSV received input url={url}")
-        response = requests.get(
-            url,
-            headers={"x-dune-api-key": self.token},
-            timeout=self.DEFAULT_TIMEOUT,
-        )
+        response = await self._get(route=route, raw=True)
         response.raise_for_status()
-        return ExecutionResultCSV(data=BytesIO(response.content))
+        return ExecutionResultCSV(data=BytesIO(await response.content.read(-1)))
 
-    def get_latest_result(self, query: Union[Query, str, int]) -> ResultsResponse:
+    async def get_latest_result(
+        self, query: Union[QueryBase, str, int]
+    ) -> ResultsResponse:
         """
         GET the latest results for a query_id without having to execute the query again.
 
         :param query: :class:`Query` object OR query id as string | int
 
         https://dune.com/docs/api/api-reference/latest_results/
         """
-        if isinstance(query, Query):
+        if isinstance(query, QueryBase):
             params = {
                 f"params.{p.key}": p.to_dict()["value"] for p in query.parameters()
             }
             query_id = query.query_id
         else:
             params = None
             query_id = int(query)
 
-        response_json = self._get(
-            route=f"query/{query_id}/results",
+        response_json = await self._get(
+            route=f"/query/{query_id}/results",
             params=params,
         )
         try:
             return ResultsResponse.from_dict(response_json)
         except KeyError as err:
             raise DuneError(response_json, "ResultsResponse", err) from err
 
-    def cancel_execution(self, job_id: str) -> bool:
+    async def cancel_execution(self, job_id: str) -> bool:
         """POST Execution Cancellation to Dune API for `job_id` (aka `execution_id`)"""
-        response_json = self._post(route=f"execution/{job_id}/cancel", params=None)
+        response_json = await self._post(
+            route=f"/execution/{job_id}/cancel",
+            params=None,
+        )
         try:
             # No need to make a dataclass for this since it's just a boolean.
             success: bool = response_json["success"]
             return success
         except KeyError as err:
             raise DuneError(response_json, "CancellationResponse", err) from err
 
-    def _refresh(
+    async def _refresh(
         self,
-        query: Query,
+        query: QueryBase,
         ping_frequency: int = 5,
         performance: Optional[str] = None,
     ) -> str:
-        job_id = self.execute(query=query, performance=performance).execution_id
-        status = self.get_status(job_id)
+        """
+        Executes a Dune `query`, waits until execution completes,
+        fetches and returns the results.
+        Sleeps `ping_frequency` seconds between each status request.
+        """
+        job_id = (await self.execute(query=query, performance=performance)).execution_id
+        status = await self.get_status(job_id)
         while status.state not in ExecutionState.terminal_states():
             self.logger.info(
                 f"waiting for query execution {job_id} to complete: {status}"
             )
-            time.sleep(ping_frequency)
-            status = self.get_status(job_id)
+            await asyncio.sleep(ping_frequency)
+            status = await self.get_status(job_id)
         if status.state == ExecutionState.FAILED:
             self.logger.error(status)
             raise QueryFailed(f"{status}. Perhaps your query took too long to run!")
 
         return job_id
 
-    def refresh(
+    async def refresh(
         self,
-        query: Query,
+        query: QueryBase,
         ping_frequency: int = 5,
         performance: Optional[str] = None,
     ) -> ResultsResponse:
         """
         Executes a Dune `query`, waits until execution completes,
         fetches and returns the results.
         Sleeps `ping_frequency` seconds between each status request.
         """
-        job_id = self._refresh(
-            query,
-            ping_frequency=ping_frequency,
-            performance=performance,
+        job_id = await self._refresh(
+            query, ping_frequency=ping_frequency, performance=performance
         )
-        return self.get_result(job_id)
+        return await self.get_result(job_id)
 
-    def refresh_csv(
+    async def refresh_csv(
         self,
-        query: Query,
+        query: QueryBase,
         ping_frequency: int = 5,
         performance: Optional[str] = None,
     ) -> ExecutionResultCSV:
         """
         Executes a Dune query, waits till execution completes,
         fetches and the results in CSV format
         (use it load the data directly in pandas.from_csv() or similar frameworks)
         """
-        job_id = self._refresh(
-            query,
-            ping_frequency=ping_frequency,
-            performance=performance,
+        job_id = await self._refresh(
+            query, ping_frequency=ping_frequency, performance=performance
         )
-        return self.get_result_csv(job_id)
+        return await self.get_result_csv(job_id)
 
-    def refresh_into_dataframe(
-        self, query: Query, performance: Optional[str] = None
+    async def refresh_into_dataframe(
+        self, query: QueryBase, performance: Optional[str] = None
     ) -> Any:
         """
         Execute a Dune Query, waits till execution completes,
         fetched and returns the result as a Pandas DataFrame
 
         This is a convenience method that uses refresh_csv underneath
         """
         try:
             import pandas  # type: ignore # pylint: disable=import-outside-toplevel
         except ImportError as exc:
             raise ImportError(
                 "dependency failure, pandas is required but missing"
             ) from exc
-        data = self.refresh_csv(query, performance=performance).data
+        data = (await self.refresh_csv(query, performance=performance)).data
         return pandas.read_csv(data)
```

### Comparing `dune_client-1.1.1/dune_client/file/base.py` & `dune_client-1.2.1/dune_client/file/base.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.1.1/dune_client/file/interface.py` & `dune_client-1.2.1/dune_client/file/interface.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.1.1/dune_client/interface.py` & `dune_client-1.2.1/dune_client/interface.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
 Abstract class for a basic Dune Interface with refresh method used by Query Runner.
 """
 import abc
 from typing import Any
 
 from dune_client.models import ResultsResponse, ExecutionResultCSV
-from dune_client.query import Query
+from dune_client.query import QueryBase
 
 
 # pylint: disable=too-few-public-methods
 class DuneInterface(abc.ABC):
     """
     User Facing Methods for a Dune Client
     """
 
     @abc.abstractmethod
-    def refresh(self, query: Query) -> ResultsResponse:
+    def refresh(self, query: QueryBase) -> ResultsResponse:
         """
         Executes a Dune query, waits till query execution completes,
         fetches and returns the results.
         """
 
     @abc.abstractmethod
-    def refresh_csv(self, query: Query) -> ExecutionResultCSV:
+    def refresh_csv(self, query: QueryBase) -> ExecutionResultCSV:
         """
         Executes a Dune query, waits till execution completes,
         fetches and the results in CSV format
         (use it load the data directly in pandas.from_csv() or similar frameworks)
 
         this Dune API only returns the raw data in CSV format, it is faster & lighterweight
         use this method for large results where you want lower CPU and memory overhead
         """
 
     @abc.abstractmethod
-    def refresh_into_dataframe(self, query: Query) -> Any:
+    def refresh_into_dataframe(self, query: QueryBase) -> Any:
         """
         Execute a Dune Query, waits till execution completes,
         fetched and returns the result as a Pandas DataFrame
 
         This is a convenience method that uses refresh_csv underneath
         it assumes the caller has already called `import pandas`
         """
```

### Comparing `dune_client-1.1.1/dune_client/models.py` & `dune_client-1.2.1/dune_client/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from io import BytesIO
 from typing import Optional, Any, Union, List, Dict
 
 from dateutil.parser import parse
-from dune_client.types import DuneRecord
 
+from dune_client.types import DuneRecord
 
 log = logging.getLogger(__name__)
 logging.basicConfig(
     format="%(asctime)s %(levelname)s %(name)s %(message)s", level=logging.INFO
 )
```

### Comparing `dune_client-1.1.1/dune_client/types.py` & `dune_client-1.2.1/dune_client/types.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.1.1/dune_client.egg-info/PKG-INFO` & `dune_client-1.2.1/dune_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-client
-Version: 1.1.1
+Version: 1.2.1
 Summary: A simple framework for interacting with Dune Analytics official API service.
 Home-page: https://github.com/cowprotocol/dune-client
 Author: Benjamin H. Smith
 Author-email: ben@cow.fi
 License: Apache License Version 2.0
 Project-URL: Tracker, https://github.com/cowprotocol/dune-client/issues
 Classifier: Programming Language :: Python :: 3
@@ -34,17 +34,17 @@
 
 ```python
 import dotenv
 import os
 
 from dune_client.types import QueryParameter
 from dune_client.client import DuneClient
-from dune_client.query import Query
+from dune_client.query import QueryBase
 
-query = Query(
+query = QueryBase(
     name="Sample Query",
     query_id=1215383,
     params=[
         QueryParameter.text_type(name="TextField", value="Word"),
         QueryParameter.number_type(name="NumberField", value=3.1415926535),
         QueryParameter.date_type(name="DateField", value="2022-05-04 00:00:00"),
         QueryParameter.enum_type(name="EnumField", value="Option 1"),
```

### Comparing `dune_client-1.1.1/dune_client.egg-info/SOURCES.txt` & `dune_client-1.2.1/dune_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dune_client-1.1.1/setup.cfg` & `dune_client-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dune_client-1.1.1/tests/e2e/test_client.py` & `dune_client-1.2.1/tests/e2e/test_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,47 +8,52 @@
 from dune_client.client import (
     DuneClient,
     ExecutionResponse,
     ExecutionStatusResponse,
     ExecutionState,
     DuneError,
 )
-from dune_client.query import Query
+from dune_client.query import QueryBase
 
 
 class TestDuneClient(unittest.TestCase):
     def setUp(self) -> None:
-        self.query = Query(
+        self.query = QueryBase(
             name="Sample Query",
             query_id=1215383,
             params=[
                 # These are the queries default parameters.
                 QueryParameter.text_type(name="TextField", value="Plain Text"),
                 QueryParameter.number_type(name="NumberField", value=3.1415926535),
                 QueryParameter.date_type(name="DateField", value="2022-05-04 00:00:00"),
                 QueryParameter.enum_type(name="ListField", value="Option 1"),
             ],
         )
         dotenv.load_dotenv()
         self.valid_api_key = os.environ["DUNE_API_KEY"]
 
     def test_get_status(self):
-        query = Query(name="No Name", query_id=1276442, params=[])
+        query = QueryBase(name="No Name", query_id=1276442, params=[])
         dune = DuneClient(self.valid_api_key)
         job_id = dune.execute(query).execution_id
         status = dune.get_status(job_id)
         self.assertTrue(
             status.state in [ExecutionState.EXECUTING, ExecutionState.PENDING]
         )
 
     def test_refresh(self):
         dune = DuneClient(self.valid_api_key)
         results = dune.refresh(self.query).get_rows()
         self.assertGreater(len(results), 0)
 
+    def test_refresh_performance_large(self):
+        dune = DuneClient(self.valid_api_key)
+        results = dune.refresh(self.query, performance="large").get_rows()
+        self.assertGreater(len(results), 0)
+
     def test_refresh_into_dataframe(self):
         dune = DuneClient(self.valid_api_key)
         pd = dune.refresh_into_dataframe(self.query)
         self.assertGreater(len(pd), 0)
 
     def test_parameters_recognized(self):
         query = copy.copy(self.query)
@@ -66,15 +71,15 @@
         results = dune.refresh(query)
         self.assertEqual(
             results.get_rows(),
             [
                 {
                     "text_field": "different word",
                     "number_field": 22,
-                    "date_field": "1991-01-01T00:00:00",
+                    "date_field": "1991-01-01 00:00:00.000",
                     "list_field": "Option 2",
                 }
             ],
         )
 
     def test_endpoints(self):
         dune = DuneClient(self.valid_api_key)
@@ -86,15 +91,15 @@
         while dune.get_status(job_id).state != ExecutionState.COMPLETED:
             time.sleep(1)
         results = dune.get_result(job_id).result.rows
         self.assertGreater(len(results), 0)
 
     def test_cancel_execution(self):
         dune = DuneClient(self.valid_api_key)
-        query = Query(
+        query = QueryBase(
             name="Long Running Query",
             query_id=1229120,
         )
         execution_response = dune.execute(query)
         job_id = execution_response.execution_id
         # POST Cancellation
         success = dune.cancel_execution(job_id)
@@ -156,10 +161,57 @@
             dune.get_status("Wonky Job ID")
         self.assertEqual(
             str(err.exception),
             "Can't build ExecutionStatusResponse from "
             "{'error': 'The requested execution ID (ID: Wonky Job ID) is invalid.'}",
         )
 
+    def test_get_latest_result_with_query_object(self):
+        dune = DuneClient(self.valid_api_key)
+        results = dune.get_latest_result(self.query).get_rows()
+        self.assertGreater(len(results), 0)
+
+    def test_get_latest_result_with_query_id(self):
+        dune = DuneClient(self.valid_api_key)
+        results = dune.get_latest_result(self.query.query_id).get_rows()
+        self.assertGreater(len(results), 0)
+
+
+class TestCRUDOps(unittest.TestCase):
+    def setUp(self) -> None:
+        dotenv.load_dotenv()
+        self.valid_api_key = os.environ["DUNE_API_KEY"]
+        self.client = DuneClient(self.valid_api_key, client_version="alpha/v1")
+        self.existing_query_id = 2713571
+
+    @unittest.skip("Works fine, but creates too many queries")
+    def test_create(self):
+        new_query = self.client.create_query(name="test_create", query_sql="")
+        self.assertGreater(new_query.base.query_id, 0)
+
+    def test_get(self):
+        q_id = 12345
+        query = self.client.get_query(q_id)
+        self.assertEqual(query.base.query_id, q_id)
+
+    def test_update(self):
+        test_id = self.existing_query_id
+        current_sql = self.client.get_query(test_id).sql
+        self.client.update_query(query_id=test_id, query_sql="")
+        self.assertEqual(self.client.get_query(test_id).sql, "")
+        # Reset:
+        self.client.update_query(query_id=test_id, query_sql=current_sql)
+
+    def test_make_private_and_public(self):
+        q_id = self.existing_query_id
+        self.client.make_private(q_id)
+        self.assertEqual(self.client.get_query(q_id).meta.is_private, True)
+        self.client.make_public(q_id)
+        self.assertEqual(self.client.get_query(q_id).meta.is_private, False)
+
+    def test_archive(self):
+        self.assertEqual(self.client.archive_query(self.existing_query_id), True)
+        self.assertEqual(self.client.unarchive_query(self.existing_query_id), False)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `dune_client-1.1.1/tests/unit/test_file.py` & `dune_client-1.2.1/tests/unit/test_file.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.1.1/tests/unit/test_models.py` & `dune_client-1.2.1/tests/unit/test_models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import unittest
 import csv
 from datetime import datetime
 from io import BytesIO, TextIOWrapper
 
 from dateutil.parser import parse
 from dateutil.tz import tzutc
@@ -13,14 +14,16 @@
     ExecutionState,
     ResultsResponse,
     TimeData,
     ExecutionResult,
     ResultMetadata,
     DuneError,
 )
+from dune_client.types import QueryParameter
+from dune_client.query import DuneQuery, QueryMeta, QueryBase
 
 
 class MyTestCase(unittest.TestCase):
     def setUp(self) -> None:
         self.execution_id = "01GBM4W2N0NMCGPZYW8AYK4YF1"
         self.query_id = 980708
         self.submission_time_str = "2022-08-29T06:33:24.913138Z"
@@ -222,10 +225,49 @@
                 ["TableName", "ct"],
                 ["eth_blocks", "6296"],
                 ["eth_traces", "4474223"],
             ],
             [r for r in result],
         )
 
+    def test_dune_query_from_dict(self):
+        example_response = """{
+            "query_id": 60066,
+            "name": "Ethereum transactions",
+            "description": "Returns ethereum transactions starting from the oldest by block time",
+            "tags": ["ethereum", "transactions"],
+            "version": 15,
+            "parameters": [{"key": "limit", "value": "5", "type": "number"}],
+            "query_engine": "v2 Dune SQL",
+            "query_sql": "select block_number from ethereum.transactions limit {{limit}};",
+            "is_private": true,
+            "is_archived": false,
+            "is_unsaved": false,
+            "owner": "Owner Name"
+        }"""
+        expected = DuneQuery(
+            base=QueryBase(
+                query_id=60066,
+                name="Ethereum transactions",
+                params=[
+                    QueryParameter.from_dict(
+                        {"key": "limit", "value": "5", "type": "number"}
+                    )
+                ],
+            ),
+            meta=QueryMeta(
+                description="Returns ethereum transactions starting from the oldest by block time",
+                tags=["ethereum", "transactions"],
+                version=15,
+                engine="v2 Dune SQL",
+                is_private=True,
+                is_archived=False,
+                is_unsaved=False,
+                owner="Owner Name",
+            ),
+            sql="select block_number from ethereum.transactions limit {{limit}};",
+        )
+        self.assertEqual(expected, DuneQuery.from_dict(json.loads(example_response)))
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `dune_client-1.1.1/tests/unit/test_query.py` & `dune_client-1.2.1/tests/unit/test_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import unittest
 from datetime import datetime
 
-from dune_client.query import Query
+from dune_client.query import QueryBase
 from dune_client.types import QueryParameter
 
 
 class TestQueryMonitor(unittest.TestCase):
     def setUp(self) -> None:
         self.date = datetime(year=1985, month=3, day=10)
         self.query_params = [
             QueryParameter.enum_type("Enum", "option1"),
             QueryParameter.text_type("Text", "plain text"),
             QueryParameter.number_type("Number", 12),
             QueryParameter.date_type("Date", "2021-01-01 12:34:56"),
         ]
-        self.query = Query(name="", query_id=0, params=self.query_params)
+        self.query = QueryBase(name="", query_id=0, params=self.query_params)
 
     def test_base_url(self):
         self.assertEqual(self.query.base_url(), "https://dune.com/queries/0")
 
     def test_url(self):
         self.assertEqual(
             self.query.url(),
             "https://dune.com/queries/0?Enum=option1&Text=plain+text&Number=12&Date=2021-01-01+12%3A34%3A56",
         )
-        self.assertEqual(Query(0, "", []).url(), "https://dune.com/queries/0")
+        self.assertEqual(QueryBase(0, "", []).url(), "https://dune.com/queries/0")
 
     def test_parameters(self):
         self.assertEqual(self.query.parameters(), self.query_params)
 
     def test_request_format(self):
         expected_answer = {
             "query_parameters": {
@@ -38,24 +38,28 @@
                 "Date": "2021-01-01 12:34:56",
             }
         }
         self.assertEqual(self.query.request_format(), expected_answer)
 
     def test_hash(self):
         # Same ID, different params
-        query1 = Query(query_id=0, params=[QueryParameter.text_type("Text", "word1")])
-        query2 = Query(query_id=0, params=[QueryParameter.text_type("Text", "word2")])
+        query1 = QueryBase(
+            query_id=0, params=[QueryParameter.text_type("Text", "word1")]
+        )
+        query2 = QueryBase(
+            query_id=0, params=[QueryParameter.text_type("Text", "word2")]
+        )
         self.assertNotEqual(hash(query1), hash(query2))
 
         # Different ID, same
-        query1 = Query(query_id=0)
-        query2 = Query(query_id=1)
+        query1 = QueryBase(query_id=0)
+        query2 = QueryBase(query_id=1)
         self.assertNotEqual(hash(query1), hash(query2))
 
         # Different ID different params
-        query1 = Query(query_id=0)
-        query2 = Query(query_id=1, params=[QueryParameter.number_type("num", 1)])
+        query1 = QueryBase(query_id=0)
+        query2 = QueryBase(query_id=1, params=[QueryParameter.number_type("num", 1)])
         self.assertNotEqual(hash(query1), hash(query2))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `dune_client-1.1.1/tests/unit/test_types.py` & `dune_client-1.2.1/tests/unit/test_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import unittest
 
-from dune_client.query import Query
+from dune_client.query import QueryBase
 from dune_client.types import QueryParameter, Address
 
 
 class TestAddress(unittest.TestCase):
     def setUp(self) -> None:
         self.lower_case_address = "0xde1c59bc25d806ad9ddcbe246c4b5e5505645718"
         self.check_sum_address = "0xDEf1CA1fb7FBcDC777520aa7f396b4E015F497aB"
@@ -65,22 +65,22 @@
         )
         self.assertEqual(
             self.date_type.to_dict(),
             {"key": "Date", "type": "datetime", "value": "2022-03-10 00:00:00"},
         )
 
     def test_repr_method(self):
-        query = Query(
+        query = QueryBase(
             query_id=1,
             name="Test Query",
             params=[self.number_type, self.text_type],
         )
 
         self.assertEqual(
-            "Query(query_id=1, name='Test Query', "
+            "QueryBase(query_id=1, name='Test Query', "
             "params=["
             "Parameter(name=Number, value=1, type=number), "
             "Parameter(name=Text, value=hello, type=text)"
             "])",
             str(query),
         )
```

