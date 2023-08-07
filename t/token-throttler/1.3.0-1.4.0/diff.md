# Comparing `tmp/token_throttler-1.3.0.tar.gz` & `tmp/token_throttler-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "token_throttler-1.3.0.tar", max compression
+gzip compressed data, was "token_throttler-1.4.0.tar", max compression
```

## Comparing `token_throttler-1.3.0.tar` & `token_throttler-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1058 2022-03-30 22:46:19.422357 token_throttler-1.3.0/LICENSE
--rw-r--r--   0        0        0     6505 2023-05-22 00:08:07.486464 token_throttler-1.3.0/README.md
--rw-r--r--   0        0        0     2614 2023-05-22 00:08:07.489798 token_throttler-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      230 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/__init__.py
--rw-r--r--   0        0        0      238 2022-03-31 21:15:42.896315 token_throttler-1.3.0/src/token_throttler/exception.py
--rw-r--r--   0        0        0        0 2023-05-22 00:08:07.489798 token_throttler-1.3.0/src/token_throttler/ext/__init__.py
--rw-r--r--   0        0        0      814 2023-05-22 00:08:07.489798 token_throttler-1.3.0/src/token_throttler/ext/fastapi.py
--rw-r--r--   0        0        0        0 2022-04-01 23:18:33.555504 token_throttler-1.3.0/src/token_throttler/py.typed
--rw-r--r--   0        0        0      139 2023-05-22 00:08:07.489798 token_throttler-1.3.0/src/token_throttler/storage/__init__.py
--rw-r--r--   0        0        0     1099 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/storage/bucket_storage.py
--rw-r--r--   0        0        0     1160 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/storage/bucket_storage_async.py
--rw-r--r--   0        0        0       91 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/storage/redis/__init__.py
--rw-r--r--   0        0        0     3806 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/storage/redis/redis_storage.py
--rw-r--r--   0        0        0     4001 2022-10-28 20:06:32.855333 token_throttler-1.3.0/src/token_throttler/storage/redis/redis_storage_async.py
--rw-r--r--   0        0        0     1728 2023-05-22 00:08:07.489798 token_throttler-1.3.0/src/token_throttler/storage/runtime_storage.py
--rw-r--r--   0        0        0      794 2022-04-18 20:45:02.610504 token_throttler-1.3.0/src/token_throttler/throttler_config.py
--rw-r--r--   0        0        0      753 2022-04-13 19:09:46.862268 token_throttler-1.3.0/src/token_throttler/token_bucket.py
--rw-r--r--   0        0        0     3919 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/token_throttler.py
--rw-r--r--   0        0        0     3709 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/token_throttler_async.py
--rw-r--r--   0        0        0     1945 2022-10-01 22:11:29.780129 token_throttler-1.3.0/src/token_throttler/validate.py
--rw-r--r--   0        0        0     8377 1970-01-01 00:00:00.000000 token_throttler-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-08-07 11:11:30.394312 token_throttler-1.4.0/LICENSE
+-rw-r--r--   0        0        0     8417 2023-08-07 11:11:30.394312 token_throttler-1.4.0/README.md
+-rw-r--r--   0        0        0     2648 2023-08-07 11:11:30.397645 token_throttler-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-08-07 11:11:30.397645 token_throttler-1.4.0/src/token_throttler/__init__.py
+-rw-r--r--   0        0        0      238 2022-03-31 21:15:42.896315 token_throttler-1.4.0/src/token_throttler/exception.py
+-rw-r--r--   0        0        0        0 2023-05-22 00:08:07.489798 token_throttler-1.4.0/src/token_throttler/ext/__init__.py
+-rw-r--r--   0        0        0      799 2023-08-07 11:11:30.397645 token_throttler-1.4.0/src/token_throttler/ext/fastapi.py
+-rw-r--r--   0        0        0        0 2022-04-01 23:18:33.555504 token_throttler-1.4.0/src/token_throttler/py.typed
+-rw-r--r--   0        0        0      139 2023-05-22 00:08:07.489798 token_throttler-1.4.0/src/token_throttler/storage/__init__.py
+-rw-r--r--   0        0        0     1099 2022-10-18 11:35:18.519274 token_throttler-1.4.0/src/token_throttler/storage/bucket_storage.py
+-rw-r--r--   0        0        0     1160 2022-10-18 11:35:18.519274 token_throttler-1.4.0/src/token_throttler/storage/bucket_storage_async.py
+-rw-r--r--   0        0        0       91 2022-10-18 11:35:18.519274 token_throttler-1.4.0/src/token_throttler/storage/redis/__init__.py
+-rw-r--r--   0        0        0     3806 2022-10-18 11:35:18.519274 token_throttler-1.4.0/src/token_throttler/storage/redis/redis_storage.py
+-rw-r--r--   0        0        0     4001 2022-10-28 20:06:32.855333 token_throttler-1.4.0/src/token_throttler/storage/redis/redis_storage_async.py
+-rw-r--r--   0        0        0     1728 2023-05-22 00:08:07.489798 token_throttler-1.4.0/src/token_throttler/storage/runtime_storage.py
+-rw-r--r--   0        0        0     2033 2023-08-07 11:11:30.397645 token_throttler-1.4.0/src/token_throttler/throttler_config.py
+-rw-r--r--   0        0        0      753 2022-04-13 19:09:46.862268 token_throttler-1.4.0/src/token_throttler/token_bucket.py
+-rw-r--r--   0        0        0     4165 2023-08-07 11:11:30.397645 token_throttler-1.4.0/src/token_throttler/token_throttler.py
+-rw-r--r--   0        0        0     3955 2023-08-07 11:11:30.397645 token_throttler-1.4.0/src/token_throttler/token_throttler_async.py
+-rw-r--r--   0        0        0     1945 2022-10-01 22:11:29.780129 token_throttler-1.4.0/src/token_throttler/validate.py
+-rw-r--r--   0        0        0     9989 1970-01-01 00:00:00.000000 token_throttler-1.4.0/PKG-INFO
```

### Comparing `token_throttler-1.3.0/LICENSE` & `token_throttler-1.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Vojko Pribudić
+Copyright (c) 2023 Vojko Pribudić
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `token_throttler-1.3.0/README.md` & `token_throttler-1.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 2. [ Features ](#features)
 3. [ Usage ](#usage)
     1. [ Manual usage example ](#usage-manual)
     2. [ Decorator usage example ](#usage-decorator)
     3. [ FastAPI usage example ](#usage-fastapi)
 4. [ Storage ](#storage)
 5. [ Configuration ](#configuration)
-   1. [ Configuration usage ](#configuration-usage)
+   1. [ Global configuration usage ](#configuration-global)
+   2. [ Instance configuration usage ](#configuration-instance)
 
 <a name="installation"></a>
 ## 1. Installation
 
 Token throttler is available on PyPI:
 ```console 
 $ python -m pip install token-throttler
@@ -175,31 +176,65 @@
 If you want your own storage engine, feel free to extend the `token_throttler.storage.BucketStorage` or `token_throttler.storage.BucketStorageAsync` classes.
 
 For storage examples see [**examples**](https://gitlab.com/vojko.pribudic/token-throttler/-/tree/main/examples) directory.
 
 <a name="configuration"></a>
 ## 5. Configuration
 
-Token throttler supports global configuration by making use of `ThrottlerConfig` class.
+Token throttler supports global and per instance configurations.
 
 Configuration params:
-- `IDENTIFIER_FAIL_SAFE` - if invalid identifier is given as a param for the `consume` method and `IDENTIFIER_FAIL_SAFE`
+- `IDENTIFIER_FAIL_SAFE` (default `False`) - if invalid identifier is given as a param for the `consume` method and `IDENTIFIER_FAIL_SAFE`
 is set to `True`, no `KeyError` exception will be raised and `consume` will act like a limitless bucket is being consumed.
-- `ENABLE_THREAD_LOCK` - if set to `True`, throttler will acquire a thread lock upon calling `consume` method and release
+- `ENABLE_THREAD_LOCK` (default `False`) - if set to `True`, throttler will acquire a thread lock upon calling `consume` method and release
 the lock once the `consume` is finished. This avoids various race conditions at a slight performance cost.
 
-<a name="configuration-usage"></a>
-### Configuration usage
+<a name="configuration-global"></a>
+### Global configuration usage
+
+Global configuration means that all the throttler instances will use the same configuration from
+the `ThrottlerConfigGlobal` class singleton (!) instance - `default_config`.
 
 ```python
-from token_throttler import ThrottlerConfig, TokenBucket, TokenThrottler
+from token_throttler import TokenBucket, TokenThrottler, default_config
 from token_throttler.storage import RuntimeStorage
 
-ThrottlerConfig.set({
+default_config.set({
    "ENABLE_THREAD_LOCK": False,
    "IDENTIFIER_FAIL_SAFE": True,
 })
 throttler: TokenThrottler = TokenThrottler(1, RuntimeStorage())
 throttler.add_bucket("hello_world", TokenBucket(10, 10))
 throttler.add_bucket("hello_world", TokenBucket(30, 20))
 ...
 ```
+
+Whenever you change the options inside `default_config` object, all of the `TokenThrottler` instances, that are not
+using the instance specific configuration, will get updated with the new settings.
+
+*NOTE*: If any modifications are attempted on the `default_config` object during runtime, a `RuntimeWarning` will be emitted. The `default_config` object is designed to be a singleton instance of the `ThrottlerConfigGlobal` class, responsible for storing and managing configuration settings. To ensure the proper functioning of the throttling mechanism and to maintain the integrity of the configuration, it is recommended to avoid making runtime changes to the `default_config` object. Any such modifications may result in unexpected behavior or inconsistencies in the throttling behavior. Instead, consider utilizing [instance-specific configuration](#Instance configuration usage).
+
+<a name="configuration-instance"></a>
+### Instance configuration usage
+
+Instance configuration is to be used when `TokenThrottler` instance(s) needs a different configuration that the global one.
+If no instance configuration is passed, `TokenThrottler` object will use the global configuration.
+
+```python
+from token_throttler import ThrottlerConfig, TokenBucket, TokenThrottler
+from token_throttler.storage import RuntimeStorage
+
+
+throttler: TokenThrottler = TokenThrottler(
+    1,
+    RuntimeStorage(),
+    ThrottlerConfig(
+        {
+            "ENABLE_THREAD_LOCK": True,
+            "IDENTIFIER_FAIL_SAFE": True,
+        }
+    ),
+)
+throttler.add_bucket("hello_world", TokenBucket(10, 10))
+throttler.add_bucket("hello_world", TokenBucket(30, 20))
+...
+```
```

### Comparing `token_throttler-1.3.0/pyproject.toml` & `token_throttler-1.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "token-throttler"
-version = "1.3.0"
+version = "1.4.0"
 description = "Token throttler is an extendable rate-limiting library somewhat based on a token bucket algorithm"
 authors = ["Vojko Pribudić <dmanthing@gmail.com>"]
 maintainers = [
         "Vojko Pribudić <dmanthing@gmail.com>",
         "Rino Dugonjić <dugonjic.rino@gmail.com>",
 ]
 repository = "https://gitlab.com/vojko.pribudic/token-throttler"
@@ -46,17 +46,19 @@
 redis = ["redis"]
 fastapi = ["fastapi"]
 
 [tool.poetry.group.test.dependencies]
 fakeredis = "^2.2"
 fastapi = "^0.95.2"
 freezegun = "^1.2"
+httpx = "^0.24.1"
 pytest = "^7.2"
 pytest-asyncio = "^0.20"
 pytest-cov = "^4.0"
+redis = "4.5.4"
 tox = "^4.4"
 
 [tool.coverage.paths]
 source = ["src"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `token_throttler-1.3.0/src/token_throttler/ext/fastapi.py` & `token_throttler-1.4.0/src/token_throttler/ext/fastapi.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Callable, Optional
+from typing import Callable, Union
 
-from fastapi import Depends, FastAPI, HTTPException, Request
+from fastapi import Depends, HTTPException
 from starlette import status
 
 from ..token_throttler import TokenThrottler, TokenThrottlerException
 
 
 class FastAPIThrottler:
-    def __init__(self, throttler: TokenThrottler, exc: Optional[Exception] = None):
+    def __init__(self, throttler: TokenThrottler, exc: Union[Exception, None] = None):
         self._throttler: TokenThrottler = throttler
-        self._exc: Optional[Exception] = exc
+        self._exc: Union[Exception, None] = exc
 
     def enable(self, callback) -> Callable:
         def _dependency(identifier: str = Depends(callback)) -> None:
             if not self._throttler.consume(identifier=identifier):
                 raise self._exc or HTTPException(
                     status_code=status.HTTP_429_TOO_MANY_REQUESTS,
                     detail=TokenThrottlerException().message,
```

### Comparing `token_throttler-1.3.0/src/token_throttler/storage/bucket_storage.py` & `token_throttler-1.4.0/src/token_throttler/storage/bucket_storage.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.3.0/src/token_throttler/storage/bucket_storage_async.py` & `token_throttler-1.4.0/src/token_throttler/storage/bucket_storage_async.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.3.0/src/token_throttler/storage/redis/redis_storage.py` & `token_throttler-1.4.0/src/token_throttler/storage/redis/redis_storage.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.3.0/src/token_throttler/storage/redis/redis_storage_async.py` & `token_throttler-1.4.0/src/token_throttler/storage/redis/redis_storage_async.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.3.0/src/token_throttler/storage/runtime_storage.py` & `token_throttler-1.4.0/src/token_throttler/storage/runtime_storage.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.3.0/src/token_throttler/token_bucket.py` & `token_throttler-1.4.0/src/token_throttler/token_bucket.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.3.0/src/token_throttler/token_throttler.py` & `token_throttler-1.4.0/src/token_throttler/token_throttler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 import asyncio
 from threading import Lock
 from typing import Any, Callable, Dict, List, Union
 
-from . import ThrottlerConfig, TokenBucket, TokenThrottlerException
+from . import (
+    ThrottlerConfig,
+    ThrottlerConfigGlobal,
+    TokenBucket,
+    TokenThrottlerException,
+    default_config,
+)
 from .storage import BucketStorage
 from .validate import (
     validate_bucket,
     validate_bucket_config,
     validate_bucket_key,
     validate_cost,
     validate_identifier,
     validate_storage,
 )
 
 
 class TokenThrottler:
-    def __init__(self, cost: int, storage: BucketStorage) -> None:
+    def __init__(
+        self,
+        cost: int,
+        storage: BucketStorage,
+        config: Union[ThrottlerConfig, ThrottlerConfigGlobal] = default_config,
+    ) -> None:
         self._cost: int = cost
         self._storage: BucketStorage = storage
         self._lock: Lock = Lock()
+        self._config: Union[ThrottlerConfig, ThrottlerConfigGlobal] = config
         validate_cost(self._cost)
         validate_storage(self._storage, BucketStorage)
 
     def _add_identifier(self, identifier: str) -> None:
         validate_identifier(identifier)
         if identifier not in self._storage.buckets:
             self._storage.buckets[identifier] = {}
@@ -71,20 +83,20 @@
             )
             self.add_bucket(identifier, token_bucket)
 
     def consume(self, identifier: str) -> bool:
         return_value: bool = True
         validate_identifier(identifier)
         if identifier not in self._storage.buckets.keys():
-            if not ThrottlerConfig.IDENTIFIER_FAIL_SAFE:
+            if not self._config.IDENTIFIER_FAIL_SAFE:
                 raise KeyError(f"Invalid identifier: `{identifier}`")
             else:
                 return return_value
 
-        if ThrottlerConfig.ENABLE_THREAD_LOCK:
+        if self._config.ENABLE_THREAD_LOCK:
             self._lock.acquire()
 
         if not all(
             self._storage.consume(identifier, str(bucket_key))
             for bucket_key in self._storage.buckets[identifier].keys()
         ):
             return_value = False
```

### Comparing `token_throttler-1.3.0/src/token_throttler/token_throttler_async.py` & `token_throttler-1.4.0/src/token_throttler/token_throttler_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 from threading import Lock
 from typing import Any, Callable, Dict, List, Union
 
-from . import ThrottlerConfig, TokenBucket, TokenThrottlerException
+from . import (
+    ThrottlerConfig,
+    ThrottlerConfigGlobal,
+    TokenBucket,
+    TokenThrottlerException,
+    default_config,
+)
 from .storage import BucketStorageAsync
 from .validate import (
     validate_bucket,
     validate_bucket_config,
     validate_bucket_key,
     validate_cost,
     validate_identifier,
     validate_storage,
 )
 
 
 class TokenThrottlerAsync:
-    def __init__(self, cost: int, storage: BucketStorageAsync) -> None:
+    def __init__(
+        self,
+        cost: int,
+        storage: BucketStorageAsync,
+        config: Union[ThrottlerConfig, ThrottlerConfigGlobal] = default_config,
+    ) -> None:
         self._cost: int = cost
         self._storage: BucketStorageAsync = storage
         self._lock: Lock = Lock()
+        self._config: Union[ThrottlerConfig, ThrottlerConfigGlobal] = config
         validate_cost(self._cost)
         validate_storage(self._storage, BucketStorageAsync)
 
     def _add_identifier(self, identifier: str) -> None:
         validate_identifier(identifier)
         if identifier not in self._storage.buckets:
             self._storage.buckets[identifier] = {}
@@ -74,20 +86,20 @@
             )
             await self.add_bucket(identifier, token_bucket)
 
     async def consume(self, identifier: str) -> bool:
         return_value: bool = True
         validate_identifier(identifier)
         if identifier not in self._storage.buckets.keys():
-            if not ThrottlerConfig.IDENTIFIER_FAIL_SAFE:
+            if not self._config.IDENTIFIER_FAIL_SAFE:
                 raise KeyError(f"Invalid identifier: `{identifier}`")
             else:
                 return return_value
 
-        if ThrottlerConfig.ENABLE_THREAD_LOCK:
+        if self._config.ENABLE_THREAD_LOCK:
             self._lock.acquire()
 
         for bucket_key in self._storage.buckets[identifier].keys():
             if not await self._storage.consume(identifier, str(bucket_key)):
                 return_value = False
 
         if self._lock.locked():
```

### Comparing `token_throttler-1.3.0/src/token_throttler/validate.py` & `token_throttler-1.4.0/src/token_throttler/validate.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.3.0/PKG-INFO` & `token_throttler-1.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: token-throttler
-Version: 1.3.0
+Version: 1.4.0
 Summary: Token throttler is an extendable rate-limiting library somewhat based on a token bucket algorithm
 Home-page: https://gitlab.com/vojko.pribudic/token-throttler
 License: MIT
 Author: Vojko Pribudić
 Author-email: dmanthing@gmail.com
 Maintainer: Vojko Pribudić
 Maintainer-email: dmanthing@gmail.com
@@ -18,21 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: fastapi
 Provides-Extra: redis
 Requires-Dist: fastapi (>=0.95.2,<0.96.0) ; extra == "fastapi"
 Requires-Dist: redis (>=4.4,<5.0) ; extra == "redis"
 Project-URL: Changelog, https://gitlab.com/vojko.pribudic/token-throttler/-/releases
 Project-URL: Repository, https://gitlab.com/vojko.pribudic/token-throttler
@@ -55,15 +49,16 @@
 2. [ Features ](#features)
 3. [ Usage ](#usage)
     1. [ Manual usage example ](#usage-manual)
     2. [ Decorator usage example ](#usage-decorator)
     3. [ FastAPI usage example ](#usage-fastapi)
 4. [ Storage ](#storage)
 5. [ Configuration ](#configuration)
-   1. [ Configuration usage ](#configuration-usage)
+   1. [ Global configuration usage ](#configuration-global)
+   2. [ Instance configuration usage ](#configuration-instance)
 
 <a name="installation"></a>
 ## 1. Installation
 
 Token throttler is available on PyPI:
 ```console 
 $ python -m pip install token-throttler
@@ -216,32 +211,66 @@
 If you want your own storage engine, feel free to extend the `token_throttler.storage.BucketStorage` or `token_throttler.storage.BucketStorageAsync` classes.
 
 For storage examples see [**examples**](https://gitlab.com/vojko.pribudic/token-throttler/-/tree/main/examples) directory.
 
 <a name="configuration"></a>
 ## 5. Configuration
 
-Token throttler supports global configuration by making use of `ThrottlerConfig` class.
+Token throttler supports global and per instance configurations.
 
 Configuration params:
-- `IDENTIFIER_FAIL_SAFE` - if invalid identifier is given as a param for the `consume` method and `IDENTIFIER_FAIL_SAFE`
+- `IDENTIFIER_FAIL_SAFE` (default `False`) - if invalid identifier is given as a param for the `consume` method and `IDENTIFIER_FAIL_SAFE`
 is set to `True`, no `KeyError` exception will be raised and `consume` will act like a limitless bucket is being consumed.
-- `ENABLE_THREAD_LOCK` - if set to `True`, throttler will acquire a thread lock upon calling `consume` method and release
+- `ENABLE_THREAD_LOCK` (default `False`) - if set to `True`, throttler will acquire a thread lock upon calling `consume` method and release
 the lock once the `consume` is finished. This avoids various race conditions at a slight performance cost.
 
-<a name="configuration-usage"></a>
-### Configuration usage
+<a name="configuration-global"></a>
+### Global configuration usage
+
+Global configuration means that all the throttler instances will use the same configuration from
+the `ThrottlerConfigGlobal` class singleton (!) instance - `default_config`.
 
 ```python
-from token_throttler import ThrottlerConfig, TokenBucket, TokenThrottler
+from token_throttler import TokenBucket, TokenThrottler, default_config
 from token_throttler.storage import RuntimeStorage
 
-ThrottlerConfig.set({
+default_config.set({
    "ENABLE_THREAD_LOCK": False,
    "IDENTIFIER_FAIL_SAFE": True,
 })
 throttler: TokenThrottler = TokenThrottler(1, RuntimeStorage())
 throttler.add_bucket("hello_world", TokenBucket(10, 10))
 throttler.add_bucket("hello_world", TokenBucket(30, 20))
 ...
 ```
 
+Whenever you change the options inside `default_config` object, all of the `TokenThrottler` instances, that are not
+using the instance specific configuration, will get updated with the new settings.
+
+*NOTE*: If any modifications are attempted on the `default_config` object during runtime, a `RuntimeWarning` will be emitted. The `default_config` object is designed to be a singleton instance of the `ThrottlerConfigGlobal` class, responsible for storing and managing configuration settings. To ensure the proper functioning of the throttling mechanism and to maintain the integrity of the configuration, it is recommended to avoid making runtime changes to the `default_config` object. Any such modifications may result in unexpected behavior or inconsistencies in the throttling behavior. Instead, consider utilizing [instance-specific configuration](#Instance configuration usage).
+
+<a name="configuration-instance"></a>
+### Instance configuration usage
+
+Instance configuration is to be used when `TokenThrottler` instance(s) needs a different configuration that the global one.
+If no instance configuration is passed, `TokenThrottler` object will use the global configuration.
+
+```python
+from token_throttler import ThrottlerConfig, TokenBucket, TokenThrottler
+from token_throttler.storage import RuntimeStorage
+
+
+throttler: TokenThrottler = TokenThrottler(
+    1,
+    RuntimeStorage(),
+    ThrottlerConfig(
+        {
+            "ENABLE_THREAD_LOCK": True,
+            "IDENTIFIER_FAIL_SAFE": True,
+        }
+    ),
+)
+throttler.add_bucket("hello_world", TokenBucket(10, 10))
+throttler.add_bucket("hello_world", TokenBucket(30, 20))
+...
+```
+
```

