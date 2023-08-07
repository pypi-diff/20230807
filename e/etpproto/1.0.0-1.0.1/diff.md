# Comparing `tmp/etpproto-1.0.0.tar.gz` & `tmp/etpproto-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etpproto-1.0.0.tar", max compression
+gzip compressed data, was "etpproto-1.0.1.tar", max compression
```

## Comparing `etpproto-1.0.0.tar` & `etpproto-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11338 2022-09-22 00:53:58.263961 etpproto-1.0.0/LICENSE
--rw-r--r--   0        0        0     1961 2022-09-22 00:53:58.263961 etpproto-1.0.0/README.md
--rw-r--r--   0        0        0        0 2022-09-22 00:53:58.263961 etpproto-1.0.0/etpproto/__init__.py
--rw-r--r--   0        0        0     2424 2022-09-22 00:53:58.263961 etpproto-1.0.0/etpproto/client_info.py
--rw-r--r--   0        0        0    20082 2022-09-22 00:53:58.263961 etpproto-1.0.0/etpproto/connection.py
--rw-r--r--   0        0        0    11645 2022-09-22 00:53:58.263961 etpproto-1.0.0/etpproto/endpoint_capability_kind.py
--rw-r--r--   0        0        0    12876 2022-09-22 00:53:58.263961 etpproto-1.0.0/etpproto/error.py
--rw-r--r--   0        0        0    25374 2022-09-22 00:53:58.263961 etpproto-1.0.0/etpproto/messages.py
--rw-r--r--   0        0        0        0 2022-09-22 00:53:58.263961 etpproto-1.0.0/etpproto/protocols/__init__.py
--rw-r--r--   0        0        0     3695 2022-09-22 00:53:58.263961 etpproto-1.0.0/etpproto/protocols/channel_data_frame.py
--rw-r--r--   0        0        0     4961 2022-09-22 00:53:58.263961 etpproto-1.0.0/etpproto/protocols/channel_data_load.py
--rw-r--r--   0        0        0     3156 2022-09-22 00:53:58.263961 etpproto-1.0.0/etpproto/protocols/channel_streaming.py
--rw-r--r--   0        0        0     7311 2022-09-22 00:53:58.263961 etpproto-1.0.0/etpproto/protocols/channel_subscribe.py
--rw-r--r--   0        0        0     4602 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/core.py
--rw-r--r--   0        0        0     6496 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/data_array.py
--rw-r--r--   0        0        0     3640 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/dataspace.py
--rw-r--r--   0        0        0     3257 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/discovery.py
--rw-r--r--   0        0        0     1881 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/discovery_query.py
--rw-r--r--   0        0        0     9286 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/growing_object.py
--rw-r--r--   0        0        0     4836 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/growing_object_notification.py
--rw-r--r--   0        0        0     1863 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/growing_object_query.py
--rw-r--r--   0        0        0     4022 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/store.py
--rw-r--r--   0        0        0     5572 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/store_notification.py
--rw-r--r--   0        0        0     2269 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/store_query.py
--rw-r--r--   0        0        0     1917 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/supported_types.py
--rw-r--r--   0        0        0     3734 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/protocols/transaction.py
--rw-r--r--   0        0        0        0 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/py.typed
--rw-r--r--   0        0        0     3201 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/uri.py
--rw-r--r--   0        0        0     4033 2022-09-22 00:53:58.267961 etpproto-1.0.0/etpproto/utils.py
--rw-r--r--   0        0        0     2056 2022-09-22 00:54:10.204052 etpproto-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 etpproto-1.0.0/setup.py
--rw-r--r--   0        0        0     2774 1970-01-01 00:00:00.000000 etpproto-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2022-09-22 17:04:17.284825 etpproto-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2137 2022-09-22 17:04:17.284825 etpproto-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/__init__.py
+-rw-r--r--   0        0        0     2374 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/client_info.py
+-rw-r--r--   0        0        0    20026 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/connection.py
+-rw-r--r--   0        0        0    11647 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/endpoint_capability_kind.py
+-rw-r--r--   0        0        0    12876 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/error.py
+-rw-r--r--   0        0        0    24705 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/messages.py
+-rw-r--r--   0        0        0        0 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/__init__.py
+-rw-r--r--   0        0        0     3695 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/channel_data_frame.py
+-rw-r--r--   0        0        0     4961 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/channel_data_load.py
+-rw-r--r--   0        0        0     3156 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/channel_streaming.py
+-rw-r--r--   0        0        0     7311 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/channel_subscribe.py
+-rw-r--r--   0        0        0     4602 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/core.py
+-rw-r--r--   0        0        0     6496 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/data_array.py
+-rw-r--r--   0        0        0     3640 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/dataspace.py
+-rw-r--r--   0        0        0     3257 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/discovery.py
+-rw-r--r--   0        0        0     1881 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/discovery_query.py
+-rw-r--r--   0        0        0     9286 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/growing_object.py
+-rw-r--r--   0        0        0     4836 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/growing_object_notification.py
+-rw-r--r--   0        0        0     1863 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/growing_object_query.py
+-rw-r--r--   0        0        0     4022 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/store.py
+-rw-r--r--   0        0        0     5572 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/store_notification.py
+-rw-r--r--   0        0        0     2269 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/store_query.py
+-rw-r--r--   0        0        0     1917 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/supported_types.py
+-rw-r--r--   0        0        0     3734 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/protocols/transaction.py
+-rw-r--r--   0        0        0        0 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/py.typed
+-rw-r--r--   0        0        0     3202 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/uri.py
+-rw-r--r--   0        0        0     4033 2022-09-22 17:04:17.284825 etpproto-1.0.1/etpproto/utils.py
+-rw-r--r--   0        0        0     2839 2022-09-22 17:04:34.288932 etpproto-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 etpproto-1.0.1/setup.py
+-rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 etpproto-1.0.1/PKG-INFO
```

### Comparing `etpproto-1.0.0/LICENSE` & `etpproto-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/README.md` & `etpproto-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ETP Protocol Implementation
 ==========
 
 [![License](https://img.shields.io/pypi/l/etpproto)](https://github.com/geosiris-technologies/etpproto-python/blob/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/etpproto-python/badge/?version=latest)](https://etpproto-python.readthedocs.io/en/latest/?badge=latest)
 [![Python CI](https://github.com/geosiris-technologies/etpproto-python/actions/workflows/ci-tests.yml/badge.svg)](https://github.com/geosiris-technologies/etpproto-python/actions/workflows/ci-tests.yml)
-![Python version](https://img.shields.io/pypi/pyversions/etpproto-python)
-[![PyPI](https://img.shields.io/pypi/v/etpproto-python)](https://badge.fury.io/py/etpproto-python)
-![Status](https://img.shields.io/pypi/status/etpproto-python)
+![Python version](https://img.shields.io/pypi/pyversions/etpproto)
+[![PyPI](https://img.shields.io/pypi/v/etpproto)](https://badge.fury.io/py/etpproto)
+![Status](https://img.shields.io/pypi/status/etpproto)
 [![codecov](https://codecov.io/gh/geosiris-technologies/etpproto-python/branch/main/graph/badge.svg)](https://codecov.io/gh/geosiris-technologies/etpproto-python)
 
 
 
 
 Installation
 ----------
@@ -54,12 +54,23 @@
 simply run
 
 ```console
     poetry run pre-commit autoupdate
 ```
 to have pre-commit install the new version.
 
-To bump a new version of the project simply run: 
+To bump a new version of the project simply publish a release name 'vX.X.X' with X replaced by your numbers
+
+Test
+----------
+
+Run tests with poetry
 ```console
-    poetry version [patch, minor, major]
+poetry run pytest -v --cache-clear -rf --cov=etpproto/ --cov-report=term --cov-report=html --maxfail=10
 ```
-You must choose between the semver rules [patch, minor, major]
+
+Test the code validity : 
+```console
+poetry run black .
+poetry run flake8 .
+poetry run mypy etpproto
+```
```

### Comparing `etpproto-1.0.0/etpproto/client_info.py` & `etpproto-1.0.1/etpproto/client_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from typing import Any, ClassVar, Dict, Union
 
+from dataclasses import dataclass, field
+
 from etptypes.energistics.etp.v12.protocol.core.open_session import OpenSession
 from etptypes.energistics.etp.v12.protocol.core.request_session import (
     RequestSession,
 )
 
 from etpproto.endpoint_capability_kind import kind_from_name
 
 
+@dataclass
 class ClientInfo:
     count_instance: ClassVar[int] = 0
 
-    endpoint_capabilities: Dict[str, Any] = {}
-
-    def __init__(
-        self,
-        ip: str = "0.0.0.0",
-        login: str = "anonymousUser",
-        endpoint_capabilities: Dict[str, Any] = {
+    endpoint_capabilities: Dict[str, Any] = field(
+        default_factory=lambda: {
             "MaxWebSocketFramePayloadSize": 10000,
             "MaxWebSocketMessagePayloadSize": 10000,
-        },
-    ):
+        }
+    )
+    login: str = field(default="anonymousUser")
+    ip: str = field(default="0.0.0.0")
+
+    def __post_init__(self):
         self._id = self.count_instance
         ClientInfo.count_instance = ClientInfo.count_instance + 1
-        self.ip = ip
-        self.login = login
-        self.endpoint_capabilities = endpoint_capabilities
 
     def getCapability(self, name: str) -> Any:
         if name in self.endpoint_capabilities:
             return self.endpoint_capabilities[name]
         return None
 
     def negotiate(self, msg: Union[OpenSession, RequestSession]):
@@ -48,14 +47,15 @@
                     print(e1)
 
             if cap_class is not None:
                 if cap_class._min is not None:
                     val = max(val, cap_class._min)
                 if cap_class._max is not None:
                     val = min(val, cap_class._max)
+
             self.endpoint_capabilities[k] = val
 
         print("Negotiated capa : ", self.endpoint_capabilities)
         # else:
         # print("No capability found for name '" + k + "'")
 
     def __str__(self) -> str:
```

### Comparing `etpproto-1.0.0/etpproto/connection.py` & `etpproto-1.0.1/etpproto/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,21 +137,21 @@
     #    ______           __                                      __             ________                __
     #   / ____/___ ______/ /_  ___     ____  ____  __  _______   / /__  _____   / ____/ /_  __  ______  / /_______   ____ ___  ___  ______________ _____ ____
     #  / /   / __ `/ ___/ __ \/ _ \   / __ \/ __ \/ / / / ___/  / / _ \/ ___/  / /   / __ \/ / / / __ \/ //_/ ___/  / __ `__ \/ _ \/ ___/ ___/ __ `/ __ `/ _ \
     # / /___/ /_/ / /__/ / / /  __/  / /_/ / /_/ / /_/ / /     / /  __(__  )  / /___/ / / / /_/ / / / / ,< (__  )  / / / / / /  __(__  |__  ) /_/ / /_/ /  __/
     # \____/\__,_/\___/_/ /_/\___/  / .___/\____/\__,_/_/     /_/\___/____/   \____/_/ /_/\__,_/_/ /_/_/|_/____/  /_/ /_/ /_/\___/____/____/\__,_/\__, /\___/
     #                              /_/                                                                                                           /____/
 
-    chunk_msg_cache: ClassVar[dict] = field(
-        default={}
-    )  #: Dict[int, Message] = field(default_factory={})
+    chunk_msg_cache: Dict[int, List[Message]] = field(
+        default_factory=lambda: {}
+    )
 
-    error_msg_cache: ClassVar[dict] = field(
-        default={}
-    )  #: Dict[int, List[Optional[Message]]] = field(default_factory={})
+    error_msg_cache: Dict[int, List[Optional[Message]]] = field(
+        default_factory=lambda: {}
+    )
 
     client_info: ClientInfo = field(default=ClientInfo())
 
     connection_type: ConnectionType = field(default=ConnectionType.SERVER)
     # TODO : last msg recieve date
     # TODO : max timeout before disconnecting
```

### Comparing `etpproto-1.0.0/etpproto/endpoint_capability_kind.py` & `etpproto-1.0.1/etpproto/endpoint_capability_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,23 +230,23 @@
 class SupportsAlternateRequestUris(EndpointCapabilityKind):
     """
     Indicates whether an endpoint supports alternate URI formats--beyond the canonical Energistics URIs, which MUST be supported for requests.
     """
 
     _default = False
     _unit = None
-    value: Optional[int] = field(default=False)
+    value: Optional[bool] = field(default=False)
 
 
 @dataclass
 class SupportsMessageHeaderExtensions(EndpointCapabilityKind):
     """
     Indicates whether an endpoint supports message header extensions. For more information about message header extensions and their use, see Section 3.6.2.
     """
 
     _default = False
     _unit = None
-    value: Optional[int] = field(default=False)
+    value: Optional[bool] = field(default=False)
 
 
 def kind_from_name(classname):
     return getattr(sys.modules[__name__], classname)
```

### Comparing `etpproto-1.0.0/etpproto/error.py` & `etpproto-1.0.1/etpproto/error.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/messages.py` & `etpproto-1.0.1/etpproto/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,23 +384,27 @@
                 object_res = schemaless_reader(
                     fo,
                     json.loads(avro_schema(object_class)),
                     return_record_name=True,
                     return_record_name_override=True,
                 )
 
+                print("HEADER", recMH, flush=True)
+
                 print(
                     "classmethod decode_binary_message", object_res, flush=True
                 )
+                print(" ==> object_class ", object_class)
 
                 return Message(
                     mh.MessageHeader.parse_obj(recMH),
                     object_class.parse_obj(object_res),
                 )
-            except Exception:
+            except Exception as e:
+                print(e)
                 # error, now we try to read it as an error, because error has now the protocol of the message send by the clien
                 # try:
                 object_class = dict_map_pro_to_class["0"][
                     str(recMH["messageType"])
                 ]
 
                 print(" ==> object_class ", object_class)
@@ -482,42 +486,14 @@
 
     return (
         mh.MessageHeader.parse_obj(recMH),
         object_class.parse_obj(object_res),
     )
 
 
-# Ecrit un message complet a partir d'un objet ETP dans un BytesIO
-# Retourne le nouveau msg_id
-def write_etp_message(
-    bio: BytesIO,
-    msg_id: int,
-    etp_object: ETPModel,
-    message_flags: int = 0,
-) -> int:
-    header_schema = json.loads(avro_schema(mh.MessageHeader))
-    objSchema = json.loads(avro_schema(type(etp_object)))
-
-    header = mh.MessageHeader(
-        protocol=int(objSchema["protocol"]),
-        messageType=int(objSchema["messageType"]),
-        correlationId=0,
-        messageId=msg_id,
-        messageFlags=message_flags,
-    )
-
-    objectDict = etp_object.dict(by_alias=True)
-
-    print("write_etp_message", objectDict, flush=True)
-
-    schemaless_writer(bio, header_schema, header.dict(by_alias=True))
-    schemaless_writer(bio, objSchema, objectDict)
-    return msg_id + 1
-
-
 # When calling thins function we are supposed to have only one entry in the data_objects map/list
 async def _encode_message_generator_chunk(
     chunkable_msg: Message,
     encoded_msg_size: int,
     max_bytes_per_msg: int,
     connection,
 ) -> AsyncGenerator[bytes, None]:
```

### Comparing `etpproto-1.0.0/etpproto/protocols/channel_data_frame.py` & `etpproto-1.0.1/etpproto/protocols/channel_data_frame.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/channel_data_load.py` & `etpproto-1.0.1/etpproto/protocols/channel_data_load.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/channel_streaming.py` & `etpproto-1.0.1/etpproto/protocols/channel_streaming.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/channel_subscribe.py` & `etpproto-1.0.1/etpproto/protocols/channel_subscribe.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/core.py` & `etpproto-1.0.1/etpproto/protocols/core.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/data_array.py` & `etpproto-1.0.1/etpproto/protocols/data_array.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/dataspace.py` & `etpproto-1.0.1/etpproto/protocols/dataspace.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/discovery.py` & `etpproto-1.0.1/etpproto/protocols/discovery.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/discovery_query.py` & `etpproto-1.0.1/etpproto/protocols/discovery_query.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/growing_object.py` & `etpproto-1.0.1/etpproto/protocols/growing_object.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/growing_object_notification.py` & `etpproto-1.0.1/etpproto/protocols/growing_object_notification.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/growing_object_query.py` & `etpproto-1.0.1/etpproto/protocols/growing_object_query.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/store.py` & `etpproto-1.0.1/etpproto/protocols/store.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/store_notification.py` & `etpproto-1.0.1/etpproto/protocols/store_notification.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/store_query.py` & `etpproto-1.0.1/etpproto/protocols/store_query.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/supported_types.py` & `etpproto-1.0.1/etpproto/protocols/supported_types.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/protocols/transaction.py` & `etpproto-1.0.1/etpproto/protocols/transaction.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/etpproto/uri.py` & `etpproto-1.0.1/etpproto/uri.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             raise AttributeError
 
     @staticmethod
     def validate(uri: str) -> bool:
         return re.match(CANONICAL_DATA_OBJECT_URIS, uri) is not None
 
 
-def findUuid(input: str) -> Optional[str]:
+def find_uuid(input: str) -> Optional[str]:
     p = re.compile(UUID_REGEX)
     result = p.search(input)
     if result is not None:
         return result.group() if result else None
     else:
         return None
```

### Comparing `etpproto-1.0.0/etpproto/utils.py` & `etpproto-1.0.1/etpproto/utils.py`

 * *Files identical despite different names*

### Comparing `etpproto-1.0.0/pyproject.toml` & `etpproto-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,54 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "etpproto"
-version = "1.0.0" # Set at build time
+version = "1.0.1" # Set at build time
 description = "ETP protocol implementation"
 authors = [
     "Lionel Untereiner <lionel.untereiner@geosiris.com>"
 ]
 maintainers = [
     "Lionel Untereiner <lionel.untereiner@geosiris.com>", 
     "Valentin Gauthier <valentin.gauthier@geosiris.com>"
 ]
 license = "Apache-2.0"
 readme = "README.md"
-repository = "https://github.com/bp/resqpy"
+repository = "https://github.com/geosiris-technologies/etpproto-python"
 homepage = "http://www.geosiris.com"
 classifiers = [
-    "Programming Language :: Python :: 3.9",
+    "Development Status :: 4 - Beta",
+    "Environment :: Web Environment",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Information Technology",
+    "License :: OSI Approved :: Apache Software License",
     "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python",
+    "Topic :: Internet :: WWW/HTTP",
+    "Topic :: Internet",
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: Software Development",
+    "Typing :: Typed",
 ]
 keywords = ["ETP"]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
-fastavro = "1.5.3"
+fastavro = "^1.6.1"
 coverage = {extras = ["toml"], version = "^6.2"}
-etptypes = "^1.0.0"
+etptypes = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.0"
 flake8 = "^4.0.0"
 black = "^22.3.0"
 pytest-cov = "^3.0.0"
 pre-commit = "^2.11.1"
```

### Comparing `etpproto-1.0.0/setup.py` & `etpproto-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['etpproto', 'etpproto.protocols']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['coverage[toml]>=6.2,<7.0', 'etptypes>=1.0.0,<2.0.0', 'fastavro==1.5.3']
+['coverage[toml]>=6.2,<7.0', 'etptypes>=1.0.1,<2.0.0', 'fastavro>=1.6.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'etpproto',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'ETP protocol implementation',
-    'long_description': 'ETP Protocol Implementation\n==========\n\n[![License](https://img.shields.io/pypi/l/etpproto)](https://github.com/geosiris-technologies/etpproto-python/blob/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/etpproto-python/badge/?version=latest)](https://etpproto-python.readthedocs.io/en/latest/?badge=latest)\n[![Python CI](https://github.com/geosiris-technologies/etpproto-python/actions/workflows/ci-tests.yml/badge.svg)](https://github.com/geosiris-technologies/etpproto-python/actions/workflows/ci-tests.yml)\n![Python version](https://img.shields.io/pypi/pyversions/etpproto-python)\n[![PyPI](https://img.shields.io/pypi/v/etpproto-python)](https://badge.fury.io/py/etpproto-python)\n![Status](https://img.shields.io/pypi/status/etpproto-python)\n[![codecov](https://codecov.io/gh/geosiris-technologies/etpproto-python/branch/main/graph/badge.svg)](https://codecov.io/gh/geosiris-technologies/etpproto-python)\n\n\n\n\nInstallation\n----------\n\nEtpproto-python can be installed with pip : \n\n```console\npip install etpproto\n```\n\nor with poetry: \n```console\npoetry add etpproto\n```\n\n\nDeveloping\n----------\n\nFirst clone the repo from gitlab.\n\n```console\n    git clone https://github.com/geosiris-technologies/etpproto-python.git\n```\n\nTo develop, you should use **[Poetry](https://python-poetry.org/)**.\n\nInstall all necessary packages (including for development) with:\n\n```console\n    poetry install\n```\n\nThen setup the Git pre-commit hook for **[Black](<https://github.com/psf/black>)** and **[Pylint](https://www.pylint.org/)**  by running\n\n```console\n    poetry run pre-commit install\n```\n\nas the ``rev`` gets updated through time to track changes of different hooks,\nsimply run\n\n```console\n    poetry run pre-commit autoupdate\n```\nto have pre-commit install the new version.\n\nTo bump a new version of the project simply run: \n```console\n    poetry version [patch, minor, major]\n```\nYou must choose between the semver rules [patch, minor, major]',
+    'long_description': "ETP Protocol Implementation\n==========\n\n[![License](https://img.shields.io/pypi/l/etpproto)](https://github.com/geosiris-technologies/etpproto-python/blob/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/etpproto-python/badge/?version=latest)](https://etpproto-python.readthedocs.io/en/latest/?badge=latest)\n[![Python CI](https://github.com/geosiris-technologies/etpproto-python/actions/workflows/ci-tests.yml/badge.svg)](https://github.com/geosiris-technologies/etpproto-python/actions/workflows/ci-tests.yml)\n![Python version](https://img.shields.io/pypi/pyversions/etpproto)\n[![PyPI](https://img.shields.io/pypi/v/etpproto)](https://badge.fury.io/py/etpproto)\n![Status](https://img.shields.io/pypi/status/etpproto)\n[![codecov](https://codecov.io/gh/geosiris-technologies/etpproto-python/branch/main/graph/badge.svg)](https://codecov.io/gh/geosiris-technologies/etpproto-python)\n\n\n\n\nInstallation\n----------\n\nEtpproto-python can be installed with pip : \n\n```console\npip install etpproto\n```\n\nor with poetry: \n```console\npoetry add etpproto\n```\n\n\nDeveloping\n----------\n\nFirst clone the repo from gitlab.\n\n```console\n    git clone https://github.com/geosiris-technologies/etpproto-python.git\n```\n\nTo develop, you should use **[Poetry](https://python-poetry.org/)**.\n\nInstall all necessary packages (including for development) with:\n\n```console\n    poetry install\n```\n\nThen setup the Git pre-commit hook for **[Black](<https://github.com/psf/black>)** and **[Pylint](https://www.pylint.org/)**  by running\n\n```console\n    poetry run pre-commit install\n```\n\nas the ``rev`` gets updated through time to track changes of different hooks,\nsimply run\n\n```console\n    poetry run pre-commit autoupdate\n```\nto have pre-commit install the new version.\n\nTo bump a new version of the project simply publish a release name 'vX.X.X' with X replaced by your numbers\n\nTest\n----------\n\nRun tests with poetry\n```console\npoetry run pytest -v --cache-clear -rf --cov=etpproto/ --cov-report=term --cov-report=html --maxfail=10\n```\n\nTest the code validity : \n```console\npoetry run black .\npoetry run flake8 .\npoetry run mypy etpproto\n```",
     'author': 'Lionel Untereiner',
     'author_email': 'lionel.untereiner@geosiris.com',
     'maintainer': 'Lionel Untereiner',
     'maintainer_email': 'lionel.untereiner@geosiris.com',
     'url': 'http://www.geosiris.com',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `etpproto-1.0.0/PKG-INFO` & `etpproto-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 Metadata-Version: 2.1
 Name: etpproto
-Version: 1.0.0
+Version: 1.0.1
 Summary: ETP protocol implementation
 Home-page: http://www.geosiris.com
 License: Apache-2.0
 Keywords: ETP
 Author: Lionel Untereiner
 Author-email: lionel.untereiner@geosiris.com
 Maintainer: Lionel Untereiner
 Maintainer-email: lionel.untereiner@geosiris.com
 Requires-Python: >=3.9,<3.11
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Dist: coverage[toml] (>=6.2,<7.0)
-Requires-Dist: etptypes (>=1.0.0,<2.0.0)
-Requires-Dist: fastavro (==1.5.3)
-Project-URL: Repository, https://github.com/bp/resqpy
+Requires-Dist: etptypes (>=1.0.1,<2.0.0)
+Requires-Dist: fastavro (>=1.6.1,<2.0.0)
+Project-URL: Repository, https://github.com/geosiris-technologies/etpproto-python
 Description-Content-Type: text/markdown
 
 ETP Protocol Implementation
 ==========
 
 [![License](https://img.shields.io/pypi/l/etpproto)](https://github.com/geosiris-technologies/etpproto-python/blob/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/etpproto-python/badge/?version=latest)](https://etpproto-python.readthedocs.io/en/latest/?badge=latest)
 [![Python CI](https://github.com/geosiris-technologies/etpproto-python/actions/workflows/ci-tests.yml/badge.svg)](https://github.com/geosiris-technologies/etpproto-python/actions/workflows/ci-tests.yml)
-![Python version](https://img.shields.io/pypi/pyversions/etpproto-python)
-[![PyPI](https://img.shields.io/pypi/v/etpproto-python)](https://badge.fury.io/py/etpproto-python)
-![Status](https://img.shields.io/pypi/status/etpproto-python)
+![Python version](https://img.shields.io/pypi/pyversions/etpproto)
+[![PyPI](https://img.shields.io/pypi/v/etpproto)](https://badge.fury.io/py/etpproto)
+![Status](https://img.shields.io/pypi/status/etpproto)
 [![codecov](https://codecov.io/gh/geosiris-technologies/etpproto-python/branch/main/graph/badge.svg)](https://codecov.io/gh/geosiris-technologies/etpproto-python)
 
 
 
 
 Installation
 ----------
@@ -77,12 +93,23 @@
 simply run
 
 ```console
     poetry run pre-commit autoupdate
 ```
 to have pre-commit install the new version.
 
-To bump a new version of the project simply run: 
+To bump a new version of the project simply publish a release name 'vX.X.X' with X replaced by your numbers
+
+Test
+----------
+
+Run tests with poetry
+```console
+poetry run pytest -v --cache-clear -rf --cov=etpproto/ --cov-report=term --cov-report=html --maxfail=10
+```
+
+Test the code validity : 
 ```console
-    poetry version [patch, minor, major]
+poetry run black .
+poetry run flake8 .
+poetry run mypy etpproto
 ```
-You must choose between the semver rules [patch, minor, major]
```

