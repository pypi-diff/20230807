# Comparing `tmp/red_utils-0.1.8.tar.gz` & `tmp/red_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red_utils-0.1.8.tar", last modified: Sat Jul 29 03:20:48 2023, max compression
+gzip compressed data, was "red_utils-0.1.9.tar", last modified: Sat Jul 29 04:07:04 2023, max compression
```

## Comparing `red_utils-0.1.8.tar` & `red_utils-0.1.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     3923 2023-07-22 00:39:16.936009 red_utils-0.1.8/README.md
--rw-r--r--   0        0        0     1839 2023-07-29 03:20:48.640715 red_utils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1265 2023-07-29 03:14:21.570786 red_utils-0.1.8/red_utils/__init__.py
--rw-r--r--   0        0        0      149 2023-07-22 00:39:16.940009 red_utils-0.1.8/red_utils/context_managers/__init__.py
--rw-r--r--   0        0        0       90 2023-07-22 00:39:16.944009 red_utils-0.1.8/red_utils/context_managers/benchmarks/__init__.py
--rw-r--r--   0        0        0      967 2023-07-29 03:14:21.570786 red_utils-0.1.8/red_utils/context_managers/benchmarks/fn_benchmarks.py
--rw-r--r--   0        0        0       69 2023-07-22 00:39:16.944009 red_utils-0.1.8/red_utils/context_managers/object_managers/__init__.py
--rw-r--r--   0        0        0     4823 2023-07-29 03:14:21.570786 red_utils-0.1.8/red_utils/context_managers/object_managers/protect.py
--rw-r--r--   0        0        0       13 2023-07-17 19:37:27.561219 red_utils-0.1.8/red_utils/dict_utils/README.md
--rw-r--r--   0        0        0      135 2023-07-29 03:14:21.570786 red_utils-0.1.8/red_utils/dict_utils/__init__.py
--rw-r--r--   0        0        0     1968 2023-07-29 03:14:21.570786 red_utils-0.1.8/red_utils/dict_utils/operations.py
--rw-r--r--   0        0        0      349 2023-07-29 03:14:21.570786 red_utils-0.1.8/red_utils/dict_utils/validators.py
--rw-r--r--   0        0        0       18 2023-07-17 19:37:27.561219 red_utils-0.1.8/red_utils/diskcache_utils/README.md
--rw-r--r--   0        0        0      849 2023-07-29 03:14:21.570786 red_utils-0.1.8/red_utils/diskcache_utils/__init__.py
--rw-r--r--   0        0        0      414 2023-07-29 03:14:21.570786 red_utils-0.1.8/red_utils/diskcache_utils/constants.py
--rw-r--r--   0        0        0     7474 2023-07-29 03:14:21.570786 red_utils-0.1.8/red_utils/diskcache_utils/operations.py
--rw-r--r--   0        0        0     5287 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/diskcache_utils/validators.py
--rw-r--r--   0        0        0       16 2023-07-17 19:37:27.565219 red_utils-0.1.8/red_utils/fastapi_utils/README.md
--rw-r--r--   0        0        0      853 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/fastapi_utils/__init__.py
--rw-r--r--   0        0        0      761 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/fastapi_utils/constants.py
--rw-r--r--   0        0        0      780 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/fastapi_utils/dependencies.py
--rw-r--r--   0        0        0     1149 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/fastapi_utils/healthcheck.py
--rw-r--r--   0        0        0     4559 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/fastapi_utils/operations.py
--rw-r--r--   0        0        0     1290 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/fastapi_utils/tag_definitions.py
--rw-r--r--   0        0        0     1964 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/fastapi_utils/uvicorn_override.py
--rw-r--r--   0        0        0     2185 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/fastapi_utils/validators.py
--rw-r--r--   0        0        0       13 2023-07-17 19:37:27.565219 red_utils-0.1.8/red_utils/file_utils/README.md
--rw-r--r--   0        0        0      127 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/file_utils/__init__.py
--rw-r--r--   0        0        0      186 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/file_utils/constants.py
--rw-r--r--   0        0        0     4483 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/file_utils/operations.py
--rw-r--r--   0        0        0       13 2023-07-17 19:37:27.577219 red_utils-0.1.8/red_utils/hash_utils/README.md
--rw-r--r--   0        0        0       78 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/hash_utils/__init__.py
--rw-r--r--   0        0        0     1054 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/hash_utils/operations.py
--rw-r--r--   0        0        0       14 2023-07-17 19:37:27.577219 red_utils-0.1.8/red_utils/httpx_utils/README.md
--rw-r--r--   0        0        0      249 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/httpx_utils/__init__.py
--rw-r--r--   0        0        0      177 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/httpx_utils/constants.py
--rw-r--r--   0        0        0     2953 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/httpx_utils/operations.py
--rw-r--r--   0        0        0     1168 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/httpx_utils/validators.py
--rw-r--r--   0        0        0       15 2023-07-17 19:37:27.581219 red_utils-0.1.8/red_utils/loguru_utils/README.md
--rw-r--r--   0        0        0      611 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/loguru_utils/__init__.py
--rw-r--r--   0        0        0     3921 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/loguru_utils/constants.py
--rw-r--r--   0        0        0     2583 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/loguru_utils/operations.py
--rw-r--r--   0        0        0     1694 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/loguru_utils/sinks.py
--rw-r--r--   0        0        0     1954 2023-07-29 03:14:21.574786 red_utils-0.1.8/red_utils/loguru_utils/validators.py
--rw-r--r--   0        0        0       16 2023-07-17 19:37:27.581219 red_utils-0.1.8/red_utils/msgpack_utils/README.md
--rw-r--r--   0        0        0      232 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/msgpack_utils/__init__.py
--rw-r--r--   0        0        0       78 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/msgpack_utils/constants.py
--rw-r--r--   0        0        0     5462 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/msgpack_utils/operations.py
--rw-r--r--   0        0        0     1673 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/sqlalchemy_utils/__init__.py
--rw-r--r--   0        0        0     1552 2023-07-29 02:41:32.408505 red_utils-0.1.8/red_utils/sqlalchemy_utils/base.py
--rw-r--r--   0        0        0     5864 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/sqlalchemy_utils/connection_models.py
--rw-r--r--   0        0        0      133 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/sqlalchemy_utils/constants.py
--rw-r--r--   0        0        0     5922 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/sqlalchemy_utils/utils.py
--rw-r--r--   0        0        0       13 2023-07-17 19:37:27.585219 red_utils-0.1.8/red_utils/time_utils/README.md
--rw-r--r--   0        0        0      158 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/time_utils/__init__.py
--rw-r--r--   0        0        0      126 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/time_utils/constants.py
--rw-r--r--   0        0        0     1340 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/time_utils/operations.py
--rw-r--r--   0        0        0       13 2023-07-17 19:37:27.585219 red_utils-0.1.8/red_utils/uuid_utils/README.md
--rw-r--r--   0        0        0      180 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/uuid_utils/__init__.py
--rw-r--r--   0        0        0      199 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/uuid_utils/classes.py
--rw-r--r--   0        0        0      144 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/uuid_utils/constants.py
--rw-r--r--   0        0        0     8283 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/uuid_utils/operations.py
--rw-r--r--   0        0        0     2803 2023-07-29 03:14:21.578786 red_utils-0.1.8/red_utils/uuid_utils/validators.py
--rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 red_utils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3923 2023-07-22 00:39:16.936009 red_utils-0.1.9/README.md
+-rw-r--r--   0        0        0     1839 2023-07-29 04:07:04.250239 red_utils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1265 2023-07-29 03:14:21.570786 red_utils-0.1.9/red_utils/__init__.py
+-rw-r--r--   0        0        0      149 2023-07-22 00:39:16.940009 red_utils-0.1.9/red_utils/context_managers/__init__.py
+-rw-r--r--   0        0        0       90 2023-07-22 00:39:16.944009 red_utils-0.1.9/red_utils/context_managers/benchmarks/__init__.py
+-rw-r--r--   0        0        0      967 2023-07-29 04:03:01.955534 red_utils-0.1.9/red_utils/context_managers/benchmarks/fn_benchmarks.py
+-rw-r--r--   0        0        0       69 2023-07-22 00:39:16.944009 red_utils-0.1.9/red_utils/context_managers/object_managers/__init__.py
+-rw-r--r--   0        0        0     4823 2023-07-29 04:03:01.955534 red_utils-0.1.9/red_utils/context_managers/object_managers/protect.py
+-rw-r--r--   0        0        0       13 2023-07-17 19:37:27.561219 red_utils-0.1.9/red_utils/dict_utils/README.md
+-rw-r--r--   0        0        0      135 2023-07-29 03:14:21.570786 red_utils-0.1.9/red_utils/dict_utils/__init__.py
+-rw-r--r--   0        0        0     1968 2023-07-29 04:03:01.963533 red_utils-0.1.9/red_utils/dict_utils/operations.py
+-rw-r--r--   0        0        0      349 2023-07-29 04:03:01.963533 red_utils-0.1.9/red_utils/dict_utils/validators.py
+-rw-r--r--   0        0        0       18 2023-07-17 19:37:27.561219 red_utils-0.1.9/red_utils/diskcache_utils/README.md
+-rw-r--r--   0        0        0      839 2023-07-29 04:03:56.967236 red_utils-0.1.9/red_utils/diskcache_utils/__init__.py
+-rw-r--r--   0        0        0      414 2023-07-29 03:14:21.570786 red_utils-0.1.9/red_utils/diskcache_utils/constants.py
+-rw-r--r--   0        0        0     7444 2023-07-29 04:03:56.967236 red_utils-0.1.9/red_utils/diskcache_utils/operations.py
+-rw-r--r--   0        0        0     5287 2023-07-29 04:03:01.963533 red_utils-0.1.9/red_utils/diskcache_utils/validators.py
+-rw-r--r--   0        0        0       16 2023-07-17 19:37:27.565219 red_utils-0.1.9/red_utils/fastapi_utils/README.md
+-rw-r--r--   0        0        0      853 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/fastapi_utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/fastapi_utils/constants.py
+-rw-r--r--   0        0        0      780 2023-07-29 04:03:01.959534 red_utils-0.1.9/red_utils/fastapi_utils/dependencies.py
+-rw-r--r--   0        0        0     1149 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/fastapi_utils/healthcheck.py
+-rw-r--r--   0        0        0     5089 2023-07-29 04:03:56.967236 red_utils-0.1.9/red_utils/fastapi_utils/operations.py
+-rw-r--r--   0        0        0     1290 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/fastapi_utils/tag_definitions.py
+-rw-r--r--   0        0        0     1964 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/fastapi_utils/uvicorn_override.py
+-rw-r--r--   0        0        0     2185 2023-07-29 04:03:01.963533 red_utils-0.1.9/red_utils/fastapi_utils/validators.py
+-rw-r--r--   0        0        0       13 2023-07-17 19:37:27.565219 red_utils-0.1.9/red_utils/file_utils/README.md
+-rw-r--r--   0        0        0      127 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/file_utils/__init__.py
+-rw-r--r--   0        0        0      186 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/file_utils/constants.py
+-rw-r--r--   0        0        0     4483 2023-07-29 04:03:01.963533 red_utils-0.1.9/red_utils/file_utils/operations.py
+-rw-r--r--   0        0        0       13 2023-07-17 19:37:27.577219 red_utils-0.1.9/red_utils/hash_utils/README.md
+-rw-r--r--   0        0        0       78 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/hash_utils/__init__.py
+-rw-r--r--   0        0        0     1054 2023-07-29 04:03:01.955534 red_utils-0.1.9/red_utils/hash_utils/operations.py
+-rw-r--r--   0        0        0       14 2023-07-17 19:37:27.577219 red_utils-0.1.9/red_utils/httpx_utils/README.md
+-rw-r--r--   0        0        0      249 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/httpx_utils/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/httpx_utils/constants.py
+-rw-r--r--   0        0        0     2953 2023-07-29 04:03:01.959534 red_utils-0.1.9/red_utils/httpx_utils/operations.py
+-rw-r--r--   0        0        0     1168 2023-07-29 04:03:01.955534 red_utils-0.1.9/red_utils/httpx_utils/validators.py
+-rw-r--r--   0        0        0       15 2023-07-17 19:37:27.581219 red_utils-0.1.9/red_utils/loguru_utils/README.md
+-rw-r--r--   0        0        0      611 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/loguru_utils/__init__.py
+-rw-r--r--   0        0        0     3921 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/loguru_utils/constants.py
+-rw-r--r--   0        0        0     2583 2023-07-29 04:03:01.963533 red_utils-0.1.9/red_utils/loguru_utils/operations.py
+-rw-r--r--   0        0        0     1694 2023-07-29 03:14:21.574786 red_utils-0.1.9/red_utils/loguru_utils/sinks.py
+-rw-r--r--   0        0        0     1954 2023-07-29 04:03:01.963533 red_utils-0.1.9/red_utils/loguru_utils/validators.py
+-rw-r--r--   0        0        0       16 2023-07-17 19:37:27.581219 red_utils-0.1.9/red_utils/msgpack_utils/README.md
+-rw-r--r--   0        0        0      232 2023-07-29 03:14:21.578786 red_utils-0.1.9/red_utils/msgpack_utils/__init__.py
+-rw-r--r--   0        0        0       78 2023-07-29 03:14:21.578786 red_utils-0.1.9/red_utils/msgpack_utils/constants.py
+-rw-r--r--   0        0        0     5462 2023-07-29 04:03:01.959534 red_utils-0.1.9/red_utils/msgpack_utils/operations.py
+-rw-r--r--   0        0        0     1673 2023-07-29 03:14:21.578786 red_utils-0.1.9/red_utils/sqlalchemy_utils/__init__.py
+-rw-r--r--   0        0        0     1552 2023-07-29 02:41:32.408505 red_utils-0.1.9/red_utils/sqlalchemy_utils/base.py
+-rw-r--r--   0        0        0     5864 2023-07-29 04:03:01.959534 red_utils-0.1.9/red_utils/sqlalchemy_utils/connection_models.py
+-rw-r--r--   0        0        0      133 2023-07-29 03:14:21.578786 red_utils-0.1.9/red_utils/sqlalchemy_utils/constants.py
+-rw-r--r--   0        0        0     5922 2023-07-29 04:03:01.959534 red_utils-0.1.9/red_utils/sqlalchemy_utils/utils.py
+-rw-r--r--   0        0        0       13 2023-07-17 19:37:27.585219 red_utils-0.1.9/red_utils/time_utils/README.md
+-rw-r--r--   0        0        0      158 2023-07-29 03:14:21.578786 red_utils-0.1.9/red_utils/time_utils/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-29 03:14:21.578786 red_utils-0.1.9/red_utils/time_utils/constants.py
+-rw-r--r--   0        0        0     1340 2023-07-29 04:03:01.955534 red_utils-0.1.9/red_utils/time_utils/operations.py
+-rw-r--r--   0        0        0       13 2023-07-17 19:37:27.585219 red_utils-0.1.9/red_utils/uuid_utils/README.md
+-rw-r--r--   0        0        0      180 2023-07-29 03:14:21.578786 red_utils-0.1.9/red_utils/uuid_utils/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-29 04:03:01.963533 red_utils-0.1.9/red_utils/uuid_utils/classes.py
+-rw-r--r--   0        0        0      144 2023-07-29 03:14:21.578786 red_utils-0.1.9/red_utils/uuid_utils/constants.py
+-rw-r--r--   0        0        0     8283 2023-07-29 03:14:21.578786 red_utils-0.1.9/red_utils/uuid_utils/operations.py
+-rw-r--r--   0        0        0     2803 2023-07-29 03:14:21.578786 red_utils-0.1.9/red_utils/uuid_utils/validators.py
+-rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 red_utils-0.1.9/PKG-INFO
```

### Comparing `red_utils-0.1.8/README.md` & `red_utils-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/pyproject.toml` & `red_utils-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "red_utils"
-version = "0.1.8"
+version = "0.1.9"
 description = "Collection of utility scripts/functions that I use frequently."
 authors = [
     { name = "redjax", email = "none@none.com" },
 ]
 dependencies = [
     "diskcache>=5.6.1",
     "loguru>=0.7.0",
```

### Comparing `red_utils-0.1.8/red_utils/__init__.py` & `red_utils-0.1.9/red_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/context_managers/benchmarks/fn_benchmarks.py` & `red_utils-0.1.9/red_utils/context_managers/benchmarks/fn_benchmarks.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/context_managers/object_managers/protect.py` & `red_utils-0.1.9/red_utils/context_managers/object_managers/protect.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/dict_utils/operations.py` & `red_utils-0.1.9/red_utils/dict_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/diskcache_utils/__init__.py` & `red_utils-0.1.9/red_utils/diskcache_utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     default_timeout_dict,
     valid_key_types,
     valid_tag_types,
     valid_val_types,
 )
 from .operations import (
     check_cache,
-    check_cache_key_exists,
     clear_cache,
     convert_to_seconds,
     delete_val,
     get_cache_size,
     get_val,
     manage_cache_tag_index,
     new_cache,
+    search_cache,
     set_expire,
     set_val,
 )
 from .validators import (
     validate_cache,
     validate_expire,
     validate_key,
```

### Comparing `red_utils-0.1.8/red_utils/diskcache_utils/operations.py` & `red_utils-0.1.9/red_utils/diskcache_utils/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
     except Exception as exc:
         raise Exception(
             f"Unhandled exception clearing cache at {cache.directory}. Details: {exc}"
         )
 
 
-def check_cache_key_exists(key: str = None, cache: diskcache.core.Cache = None) -> bool:
+def search_cache(key: str = None, cache: diskcache.core.Cache = None) -> bool:
     """Check if a key exists in a cache."""
     ## Key validation
     validate_key(key=key)
     validate_cache(cache=cache)
 
     ## Check if key exists in cache
     if key in cache:
@@ -194,15 +194,15 @@
 def set_expire(
     key: str = None, cache: Cache = None, expire: int = None
 ) -> Union[dict[str, str], None]:
     validate_key(key)
     validate_cache(cache)
     validate_expire(expire)
 
-    if not check_cache_key_exists(key=key, cache=cache):
+    if not search_cache(key=key, cache=cache):
         return {
             "warning": f"Cache item with key [{key}] does not exist in cache at {cache.directory}/"
         }
 
     try:
         with cache as ref:
             ref.touch(key, expire=expire)
@@ -214,15 +214,15 @@
 
 
 def get_val(key: valid_key_types = None, cache: Cache = None, tags: list[str] = None):
     validate_key(key)
     validate_cache(cache)
     validate_tags(tags)
 
-    if check_cache_key_exists(key=key, cache=cache):
+    if search_cache(key=key, cache=cache):
         try:
             with cache as ref:
                 _val = ref.get(key=key)
 
                 return _val
 
         except Exception as exc:
```

### Comparing `red_utils-0.1.8/red_utils/diskcache_utils/validators.py` & `red_utils-0.1.9/red_utils/diskcache_utils/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/fastapi_utils/__init__.py` & `red_utils-0.1.9/red_utils/fastapi_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/fastapi_utils/constants.py` & `red_utils-0.1.9/red_utils/fastapi_utils/constants.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/fastapi_utils/dependencies.py` & `red_utils-0.1.9/red_utils/fastapi_utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/fastapi_utils/healthcheck.py` & `red_utils-0.1.9/red_utils/fastapi_utils/healthcheck.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/fastapi_utils/operations.py` & `red_utils-0.1.9/red_utils/fastapi_utils/operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,31 @@
 )
 
 import fastapi
 
 from fastapi import APIRouter, FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 
+def fix_api_docs(app: FastAPI):
+    """Fix Not Found /api/v1/openapi.json error when a root_path is set.
+
+    NOTE: This is *only* necessary if you set a root_path in the FastAPI app,
+    i.e. app = FastAPI(root_path="/some/path").
+
+    If a FastAPI app is initialized with root_path=$some_path, the /docs
+    route breaks. Pass the FastAPI app to through this function to fix,
+    i.e.:
+    fix_api_docs(app)
+    """
+
+    @app.get(app.root_path + "/openapi.json")
+    def custom_swagger_ui_html():
+        return app.openapi()
+
+
 def update_tags_metadata(
     tags_metadata: list = tags_metadata,
     update_metadata: Union[list[dict[str, str]], dict[str, str]] = None,
 ):
     """Update the global tags_metadata list with new values.
 
     Import this function in another app, create a new list of tags (or
```

### Comparing `red_utils-0.1.8/red_utils/fastapi_utils/tag_definitions.py` & `red_utils-0.1.9/red_utils/fastapi_utils/tag_definitions.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/fastapi_utils/uvicorn_override.py` & `red_utils-0.1.9/red_utils/fastapi_utils/uvicorn_override.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/fastapi_utils/validators.py` & `red_utils-0.1.9/red_utils/fastapi_utils/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/file_utils/operations.py` & `red_utils-0.1.9/red_utils/file_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/hash_utils/operations.py` & `red_utils-0.1.9/red_utils/hash_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/httpx_utils/operations.py` & `red_utils-0.1.9/red_utils/httpx_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/httpx_utils/validators.py` & `red_utils-0.1.9/red_utils/httpx_utils/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/loguru_utils/__init__.py` & `red_utils-0.1.9/red_utils/loguru_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/loguru_utils/constants.py` & `red_utils-0.1.9/red_utils/loguru_utils/constants.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/loguru_utils/operations.py` & `red_utils-0.1.9/red_utils/loguru_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/loguru_utils/sinks.py` & `red_utils-0.1.9/red_utils/loguru_utils/sinks.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/loguru_utils/validators.py` & `red_utils-0.1.9/red_utils/loguru_utils/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/msgpack_utils/operations.py` & `red_utils-0.1.9/red_utils/msgpack_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/sqlalchemy_utils/__init__.py` & `red_utils-0.1.9/red_utils/sqlalchemy_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/sqlalchemy_utils/base.py` & `red_utils-0.1.9/red_utils/sqlalchemy_utils/base.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/sqlalchemy_utils/connection_models.py` & `red_utils-0.1.9/red_utils/sqlalchemy_utils/connection_models.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/sqlalchemy_utils/utils.py` & `red_utils-0.1.9/red_utils/sqlalchemy_utils/utils.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/time_utils/operations.py` & `red_utils-0.1.9/red_utils/time_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/uuid_utils/operations.py` & `red_utils-0.1.9/red_utils/uuid_utils/operations.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/red_utils/uuid_utils/validators.py` & `red_utils-0.1.9/red_utils/uuid_utils/validators.py`

 * *Files identical despite different names*

### Comparing `red_utils-0.1.8/PKG-INFO` & `red_utils-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red_utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: Collection of utility scripts/functions that I use frequently.
 Author-Email: redjax <none@none.com>
 License: MIT
 Project-URL: Repository, https://github.com/redjax/red-utils
 Requires-Python: >=3.11
 Requires-Dist: diskcache>=5.6.1
 Requires-Dist: loguru>=0.7.0
```

