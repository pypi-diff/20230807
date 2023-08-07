# Comparing `tmp/types-protobuf-4.23.0.2.tar.gz` & `tmp/types-protobuf-4.23.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-protobuf-4.23.0.2.tar", last modified: Sat Jul 22 15:13:31 2023, max compression
+gzip compressed data, was "types-protobuf-4.23.0.3.tar", last modified: Mon Aug  7 06:18:50 2023, max compression
```

## Comparing `types-protobuf-4.23.0.2.tar` & `types-protobuf-4.23.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-22 15:13:29.000000 types-protobuf-4.23.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-22 15:13:29.000000 types-protobuf-4.23.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.591401 types-protobuf-4.23.0.2/google-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-22 15:13:29.000000 types-protobuf-4.23.0.2/google-stubs/METADATA.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/google-stubs/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/any_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/api_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/google-stubs/protobuf/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/compiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/compiler/plugin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    76549 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor_pool.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/duration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/field_mask_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/api_implementation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/enum_type_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/extension_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/message_listener.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/python_message.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/type_checkers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/well_known_types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/internal/wire_format.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/json_format.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/message.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/message_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/reflection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/source_context_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/symbol_database.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/text_format.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/timestamp_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/type_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/google-stubs/protobuf/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-22 15:13:13.000000 types-protobuf-4.23.0.2/google-stubs/protobuf/wrappers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-22 15:13:29.000000 types-protobuf-4.23.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:13:31.595401 types-protobuf-4.23.0.2/types_protobuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-22 15:13:31.000000 types-protobuf-4.23.0.2/types_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-22 15:13:31.000000 types-protobuf-4.23.0.2/types_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:13:31.000000 types-protobuf-4.23.0.2/types_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-22 15:13:31.000000 types-protobuf-4.23.0.2/types_protobuf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:50.411821 types-protobuf-4.23.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-08-07 06:18:48.000000 types-protobuf-4.23.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 06:18:48.000000 types-protobuf-4.23.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-07 06:18:50.411821 types-protobuf-4.23.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:50.407821 types-protobuf-4.23.0.3/google-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-07 06:18:48.000000 types-protobuf-4.23.0.3/google-stubs/METADATA.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:50.411821 types-protobuf-4.23.0.3/google-stubs/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/any_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/api_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:50.411821 types-protobuf-4.23.0.3/google-stubs/protobuf/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/compiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/compiler/plugin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/descriptor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    76549 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/descriptor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/descriptor_pool.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/duration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/field_mask_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:50.411821 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/api_implementation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/enum_type_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/extension_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/message_listener.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/python_message.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/type_checkers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/well_known_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/internal/wire_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/json_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/message_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/reflection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/source_context_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/symbol_database.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/text_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/timestamp_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/type_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:50.411821 types-protobuf-4.23.0.3/google-stubs/protobuf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-08-07 06:18:37.000000 types-protobuf-4.23.0.3/google-stubs/protobuf/wrappers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 06:18:50.411821 types-protobuf-4.23.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-08-07 06:18:48.000000 types-protobuf-4.23.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:50.411821 types-protobuf-4.23.0.3/types_protobuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-07 06:18:50.000000 types-protobuf-4.23.0.3/types_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-07 06:18:50.000000 types-protobuf-4.23.0.3/types_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:18:50.000000 types-protobuf-4.23.0.3/types_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 06:18:50.000000 types-protobuf-4.23.0.3/types_protobuf.egg-info/top_level.txt
```

### Comparing `types-protobuf-4.23.0.2/CHANGELOG.md` & `types-protobuf-4.23.0.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 4.23.0.3 (2023-08-07)
+
+Add missing stubs in google.protobuf.message_factory module (#10537)
+
 ## 4.23.0.2 (2023-07-22)
 
 Pretend `_EnumTypeWrapper` inherits from `type` (#10203)
 
 Pretend `google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper` inherits from `type`. It doesn't really, but this makes type checkers stop complaining when you use it as a metaclass, which is the only reason the class exists.
 
 ## 4.23.0.1 (2023-05-10)
```

### Comparing `types-protobuf-4.23.0.2/PKG-INFO` & `types-protobuf-4.23.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 4.23.0.2
+Version: 4.23.0.3
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 Generated with aid from mypy-protobuf v3.4.0
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `53a893279713c8abcc970a578d6f28e97efdd68f` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
+This package was generated from typeshed commit `7e497f052df7398262ced89c93f4e8bd573698f7` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
 pytype 2023.7.21.
```

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/any_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/any_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/api_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/compiler/plugin_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/compiler/plugin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/descriptor.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/descriptor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/descriptor_pool.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/descriptor_pool.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/duration_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/duration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/empty_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/field_mask_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/field_mask_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/containers.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/internal/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/decoder.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/internal/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/encoder.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/internal/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/enum_type_wrapper.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/internal/enum_type_wrapper.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/extension_dict.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/internal/extension_dict.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/well_known_types.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/internal/well_known_types.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/internal/wire_format.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/internal/wire_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/json_format.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/json_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/message.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/message.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/message_factory.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/message_factory.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -8,8 +8,10 @@
 
 class MessageFactory:
     pool: Any
     def __init__(self, pool: DescriptorPool | None = ...) -> None: ...
     def GetPrototype(self, descriptor: Descriptor) -> type[Message]: ...
     def GetMessages(self, files: Iterable[str]) -> dict[str, type[Message]]: ...
 
+def GetMessageClass(descriptor: Descriptor) -> type[Message]: ...
+def GetMessageClassesForFiles(files: Iterable[str], pool: DescriptorPool) -> dict[str, type[Message]]: ...
 def GetMessages(file_protos: Iterable[FileDescriptorProto], pool: DescriptorPool | None = ...) -> dict[str, type[Message]]: ...
```

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/service.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/service.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/source_context_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/source_context_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/struct_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/struct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/symbol_database.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/symbol_database.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/text_format.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/text_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/timestamp_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/timestamp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/type_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/google-stubs/protobuf/wrappers_pb2.pyi` & `types-protobuf-4.23.0.3/google-stubs/protobuf/wrappers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.23.0.2/setup.py` & `types-protobuf-4.23.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 Generated with aid from mypy-protobuf v3.4.0
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `53a893279713c8abcc970a578d6f28e97efdd68f` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
+This package was generated from typeshed commit `7e497f052df7398262ced89c93f4e8bd573698f7` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
 pytype 2023.7.21.
 '''.lstrip()
 
 setup(name=name,
-      version="4.23.0.2",
+      version="4.23.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md",
```

### Comparing `types-protobuf-4.23.0.2/types_protobuf.egg-info/PKG-INFO` & `types-protobuf-4.23.0.3/types_protobuf.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 4.23.0.2
+Version: 4.23.0.3
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 Generated with aid from mypy-protobuf v3.4.0
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `53a893279713c8abcc970a578d6f28e97efdd68f` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
+This package was generated from typeshed commit `7e497f052df7398262ced89c93f4e8bd573698f7` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
 pytype 2023.7.21.
```

### Comparing `types-protobuf-4.23.0.2/types_protobuf.egg-info/SOURCES.txt` & `types-protobuf-4.23.0.3/types_protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

