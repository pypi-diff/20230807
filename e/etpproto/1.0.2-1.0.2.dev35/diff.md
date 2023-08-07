# Comparing `tmp/etpproto-1.0.2.tar.gz` & `tmp/etpproto-1.0.2.dev35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etpproto-1.0.2.tar", max compression
+gzip compressed data, was "etpproto-1.0.2.dev35.tar", max compression
```

## Comparing `etpproto-1.0.2.tar` & `etpproto-1.0.2.dev35.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11338 2023-08-07 15:09:19.543805 etpproto-1.0.2/LICENSE
--rw-r--r--   0        0        0     2216 2023-08-07 15:09:19.543805 etpproto-1.0.2/README.md
--rw-r--r--   0        0        0       74 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/__init__.py
--rw-r--r--   0        0        0     2449 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/client_info.py
--rw-r--r--   0        0        0    20101 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/connection.py
--rw-r--r--   0        0        0    11722 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/endpoint_capability_kind.py
--rw-r--r--   0        0        0    12951 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/error.py
--rw-r--r--   0        0        0    24780 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/messages.py
--rw-r--r--   0        0        0       74 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/__init__.py
--rw-r--r--   0        0        0     3770 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/channel_data_frame.py
--rw-r--r--   0        0        0     5036 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/channel_data_load.py
--rw-r--r--   0        0        0     3231 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/channel_streaming.py
--rw-r--r--   0        0        0     7386 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/channel_subscribe.py
--rw-r--r--   0        0        0     4677 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/core.py
--rw-r--r--   0        0        0     6571 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/data_array.py
--rw-r--r--   0        0        0     3715 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/dataspace.py
--rw-r--r--   0        0        0     3332 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/discovery.py
--rw-r--r--   0        0        0     1956 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/discovery_query.py
--rw-r--r--   0        0        0     9361 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/growing_object.py
--rw-r--r--   0        0        0     4911 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/growing_object_notification.py
--rw-r--r--   0        0        0     1938 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/growing_object_query.py
--rw-r--r--   0        0        0     4097 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/store.py
--rw-r--r--   0        0        0     5647 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/store_notification.py
--rw-r--r--   0        0        0     2344 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/store_query.py
--rw-r--r--   0        0        0     1992 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/supported_types.py
--rw-r--r--   0        0        0     3809 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/protocols/transaction.py
--rw-r--r--   0        0        0        0 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/py.typed
--rw-r--r--   0        0        0     3277 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/uri.py
--rw-r--r--   0        0        0     4108 2023-08-07 15:09:19.543805 etpproto-1.0.2/etpproto/utils.py
--rw-r--r--   0        0        0     2834 2023-08-07 15:09:38.416147 etpproto-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3691 1970-01-01 00:00:00.000000 etpproto-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/LICENSE
+-rw-r--r--   0        0        0     2216 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/README.md
+-rw-r--r--   0        0        0       74 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/__init__.py
+-rw-r--r--   0        0        0     2449 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/client_info.py
+-rw-r--r--   0        0        0    20101 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/connection.py
+-rw-r--r--   0        0        0    11722 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/endpoint_capability_kind.py
+-rw-r--r--   0        0        0    12951 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/error.py
+-rw-r--r--   0        0        0    24780 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/messages.py
+-rw-r--r--   0        0        0       74 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/__init__.py
+-rw-r--r--   0        0        0     3770 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/channel_data_frame.py
+-rw-r--r--   0        0        0     5036 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/channel_data_load.py
+-rw-r--r--   0        0        0     3231 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/channel_streaming.py
+-rw-r--r--   0        0        0     7386 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/channel_subscribe.py
+-rw-r--r--   0        0        0     4677 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/core.py
+-rw-r--r--   0        0        0     6571 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/data_array.py
+-rw-r--r--   0        0        0     3715 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/dataspace.py
+-rw-r--r--   0        0        0     3332 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/discovery.py
+-rw-r--r--   0        0        0     1956 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/discovery_query.py
+-rw-r--r--   0        0        0     9361 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/growing_object.py
+-rw-r--r--   0        0        0     4911 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/growing_object_notification.py
+-rw-r--r--   0        0        0     1938 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/growing_object_query.py
+-rw-r--r--   0        0        0     4097 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/store.py
+-rw-r--r--   0        0        0     5647 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/store_notification.py
+-rw-r--r--   0        0        0     2344 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/store_query.py
+-rw-r--r--   0        0        0     1992 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/supported_types.py
+-rw-r--r--   0        0        0     3809 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/protocols/transaction.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/py.typed
+-rw-r--r--   0        0        0     3277 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/uri.py
+-rw-r--r--   0        0        0     4108 2023-08-07 14:43:59.334746 etpproto-1.0.2.dev35/etpproto/utils.py
+-rw-r--r--   0        0        0     2840 2023-08-07 14:44:21.706999 etpproto-1.0.2.dev35/pyproject.toml
+-rw-r--r--   0        0        0     3697 1970-01-01 00:00:00.000000 etpproto-1.0.2.dev35/PKG-INFO
```

### Comparing `etpproto-1.0.2/LICENSE` & `etpproto-1.0.2.dev35/LICENSE`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/README.md` & `etpproto-1.0.2.dev35/README.md`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/client_info.py` & `etpproto-1.0.2.dev35/etpproto/client_info.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/connection.py` & `etpproto-1.0.2.dev35/etpproto/connection.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/endpoint_capability_kind.py` & `etpproto-1.0.2.dev35/etpproto/endpoint_capability_kind.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/error.py` & `etpproto-1.0.2.dev35/etpproto/error.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/messages.py` & `etpproto-1.0.2.dev35/etpproto/messages.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/channel_data_frame.py` & `etpproto-1.0.2.dev35/etpproto/protocols/channel_data_frame.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/channel_data_load.py` & `etpproto-1.0.2.dev35/etpproto/protocols/channel_data_load.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/channel_streaming.py` & `etpproto-1.0.2.dev35/etpproto/protocols/channel_streaming.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/channel_subscribe.py` & `etpproto-1.0.2.dev35/etpproto/protocols/channel_subscribe.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/core.py` & `etpproto-1.0.2.dev35/etpproto/protocols/core.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/data_array.py` & `etpproto-1.0.2.dev35/etpproto/protocols/data_array.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/dataspace.py` & `etpproto-1.0.2.dev35/etpproto/protocols/dataspace.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/discovery.py` & `etpproto-1.0.2.dev35/etpproto/protocols/discovery.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/discovery_query.py` & `etpproto-1.0.2.dev35/etpproto/protocols/discovery_query.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/growing_object.py` & `etpproto-1.0.2.dev35/etpproto/protocols/growing_object.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/growing_object_notification.py` & `etpproto-1.0.2.dev35/etpproto/protocols/growing_object_notification.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/growing_object_query.py` & `etpproto-1.0.2.dev35/etpproto/protocols/growing_object_query.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/store.py` & `etpproto-1.0.2.dev35/etpproto/protocols/store.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/store_notification.py` & `etpproto-1.0.2.dev35/etpproto/protocols/store_notification.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/store_query.py` & `etpproto-1.0.2.dev35/etpproto/protocols/store_query.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/supported_types.py` & `etpproto-1.0.2.dev35/etpproto/protocols/supported_types.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/protocols/transaction.py` & `etpproto-1.0.2.dev35/etpproto/protocols/transaction.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/uri.py` & `etpproto-1.0.2.dev35/etpproto/uri.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/etpproto/utils.py` & `etpproto-1.0.2.dev35/etpproto/utils.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.2/pyproject.toml` & `etpproto-1.0.2.dev35/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "etpproto"
-version = "1.0.2" # Set at build time
+version = "1.0.2.dev35" # Set at build time
 description = "ETP protocol implementation"
 authors = [
     "Lionel Untereiner <lionel.untereiner@geosiris.com>"
 ]
 maintainers = [
     "Lionel Untereiner <lionel.untereiner@geosiris.com>", 
     "Valentin Gauthier <valentin.gauthier@geosiris.com>"
```

### Comparing `etpproto-1.0.2/PKG-INFO` & `etpproto-1.0.2.dev35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etpproto
-Version: 1.0.2
+Version: 1.0.2.dev35
 Summary: ETP protocol implementation
 Home-page: http://www.geosiris.com
 License: Apache-2.0
 Keywords: ETP
 Author: Lionel Untereiner
 Author-email: lionel.untereiner@geosiris.com
 Maintainer: Lionel Untereiner
```

