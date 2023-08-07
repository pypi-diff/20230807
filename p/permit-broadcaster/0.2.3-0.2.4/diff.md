# Comparing `tmp/permit-broadcaster-0.2.3.tar.gz` & `tmp/permit-broadcaster-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-broadcaster-0.2.3.tar", last modified: Tue Jun 20 11:36:40 2023, max compression
+gzip compressed data, was "permit-broadcaster-0.2.4.tar", last modified: Mon Aug  7 13:47:37 2023, max compression
```

## Comparing `permit-broadcaster-0.2.3.tar` & `permit-broadcaster-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:36:40.933358 permit-broadcaster-0.2.3/
--rw-r--r--   0 roekatz    (501) staff       (20)     1518 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.3/LICENSE.md
--rw-r--r--   0 roekatz    (501) staff       (20)     5933 2023-06-20 11:36:40.933726 permit-broadcaster-0.2.3/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     5003 2023-06-20 11:32:57.000000 permit-broadcaster-0.2.3/README.md
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:36:40.908324 permit-broadcaster-0.2.3/broadcaster/
--rw-r--r--   0 roekatz    (501) staff       (20)       92 2023-06-20 11:34:27.000000 permit-broadcaster-0.2.3/broadcaster/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:36:40.924429 permit-broadcaster-0.2.3/broadcaster/_backends/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.3/broadcaster/_backends/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      667 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.3/broadcaster/_backends/base.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3277 2023-06-20 11:32:57.000000 permit-broadcaster-0.2.3/broadcaster/_backends/kafka.py
--rw-r--r--   0 roekatz    (501) staff       (20)      912 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.3/broadcaster/_backends/memory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1300 2023-06-20 11:33:07.000000 permit-broadcaster-0.2.3/broadcaster/_backends/postgres.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1351 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.3/broadcaster/_backends/redis.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3827 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.3/broadcaster/_base.py
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.3/broadcaster/py.typed
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:36:40.928680 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     5933 2023-06-20 11:36:40.000000 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)      530 2023-06-20 11:36:40.000000 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-20 11:36:40.000000 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       91 2023-06-20 11:36:40.000000 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       34 2023-06-20 11:36:40.000000 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      548 2023-06-20 11:36:40.934337 permit-broadcaster-0.2.3/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     1928 2023-06-20 11:33:35.000000 permit-broadcaster-0.2.3/setup.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:36:40.928819 permit-broadcaster-0.2.3/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)     1613 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.3/tests/test_broadcast.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-08-07 13:47:37.709515 permit-broadcaster-0.2.4/
+-rw-r--r--   0 roekatz    (501) staff       (20)     1518 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.4/LICENSE.md
+-rw-r--r--   0 roekatz    (501) staff       (20)     5933 2023-08-07 13:47:37.709598 permit-broadcaster-0.2.4/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     5003 2023-06-20 11:32:57.000000 permit-broadcaster-0.2.4/README.md
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-08-07 13:47:37.706789 permit-broadcaster-0.2.4/broadcaster/
+-rw-r--r--   0 roekatz    (501) staff       (20)       92 2023-08-07 13:46:55.000000 permit-broadcaster-0.2.4/broadcaster/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-08-07 13:47:37.708269 permit-broadcaster-0.2.4/broadcaster/_backends/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.4/broadcaster/_backends/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      667 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.4/broadcaster/_backends/base.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3277 2023-06-20 11:32:57.000000 permit-broadcaster-0.2.4/broadcaster/_backends/kafka.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      912 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.4/broadcaster/_backends/memory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1906 2023-08-07 08:30:22.000000 permit-broadcaster-0.2.4/broadcaster/_backends/postgres.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1351 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.4/broadcaster/_backends/redis.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3827 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.4/broadcaster/_base.py
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.4/broadcaster/py.typed
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-08-07 13:47:37.709043 permit-broadcaster-0.2.4/permit_broadcaster.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     5933 2023-08-07 13:47:37.000000 permit-broadcaster-0.2.4/permit_broadcaster.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)      530 2023-08-07 13:47:37.000000 permit-broadcaster-0.2.4/permit_broadcaster.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-08-07 13:47:37.000000 permit-broadcaster-0.2.4/permit_broadcaster.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       91 2023-08-07 13:47:37.000000 permit-broadcaster-0.2.4/permit_broadcaster.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       34 2023-08-07 13:47:37.000000 permit-broadcaster-0.2.4/permit_broadcaster.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      548 2023-08-07 13:47:37.709907 permit-broadcaster-0.2.4/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     1928 2023-06-20 11:33:35.000000 permit-broadcaster-0.2.4/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-08-07 13:47:37.709215 permit-broadcaster-0.2.4/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)     1613 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.4/tests/test_broadcast.py
```

### Comparing `permit-broadcaster-0.2.3/LICENSE.md` & `permit-broadcaster-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.3/PKG-INFO` & `permit-broadcaster-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permit-broadcaster
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple broadcast channels (Permit fork)
 Home-page: https://github.com/permitio/broadcaster
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `permit-broadcaster-0.2.3/README.md` & `permit-broadcaster-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.3/broadcaster/_backends/base.py` & `permit-broadcaster-0.2.4/broadcaster/_backends/base.py`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.3/broadcaster/_backends/kafka.py` & `permit-broadcaster-0.2.4/broadcaster/_backends/kafka.py`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.3/broadcaster/_backends/memory.py` & `permit-broadcaster-0.2.4/broadcaster/_backends/memory.py`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.3/broadcaster/_backends/postgres.py` & `permit-broadcaster-0.2.4/broadcaster/_backends/postgres.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 import asyncio
 from typing import Any
 
 import asyncpg
+import os
 
 from .._base import Event
 from .base import BroadcastBackend
 
+try:
+    POOL_MAX_SIZE = int(os.getenv("BROADCASTER_PG_MAX_POOL_SIZE"))
+except TypeError:
+    POOL_MAX_SIZE = 10
 
 class PostgresBackend(BroadcastBackend):
+    _pools = {}
+    _pools_lock = asyncio.Lock()
+
     def __init__(self, url: str):
         self._url = url
 
+    async def _get_pool(self):
+        async with self.__class__._pools_lock:
+            if self._url not in self.__class__._pools:
+                self.__class__._pools[self._url] = await asyncpg.create_pool(self._url, max_size=POOL_MAX_SIZE)
+            return self.__class__._pools[self._url]
+
     async def connect(self) -> None:
-        self._conn = await asyncpg.connect(self._url)
+        self._conn = await (await self._get_pool()).acquire()
         self._listen_queue: asyncio.Queue = asyncio.Queue()
         self._conn.add_termination_listener(self._termination_listener)
 
     async def disconnect(self) -> None:
-        await self._conn.close()
+        self._conn.remove_termination_listener(self._termination_listener)
+        await (await self._get_pool()).release(self._conn)
+        self._conn = None
 
     async def subscribe(self, channel: str) -> None:
         await self._conn.add_listener(channel, self._listener)
 
     async def unsubscribe(self, channel: str) -> None:
         await self._conn.remove_listener(channel, self._listener)
```

### Comparing `permit-broadcaster-0.2.3/broadcaster/_backends/redis.py` & `permit-broadcaster-0.2.4/broadcaster/_backends/redis.py`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.3/broadcaster/_base.py` & `permit-broadcaster-0.2.4/broadcaster/_base.py`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.3/permit_broadcaster.egg-info/PKG-INFO` & `permit-broadcaster-0.2.4/permit_broadcaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permit-broadcaster
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple broadcast channels (Permit fork)
 Home-page: https://github.com/permitio/broadcaster
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

### Comparing `permit-broadcaster-0.2.3/permit_broadcaster.egg-info/SOURCES.txt` & `permit-broadcaster-0.2.4/permit_broadcaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.3/setup.cfg` & `permit-broadcaster-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.3/setup.py` & `permit-broadcaster-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.3/tests/test_broadcast.py` & `permit-broadcaster-0.2.4/tests/test_broadcast.py`

 * *Files identical despite different names*

