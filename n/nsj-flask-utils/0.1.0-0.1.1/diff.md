# Comparing `tmp/nsj_flask_utils-0.1.0.tar.gz` & `tmp/nsj_flask_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_flask_utils-0.1.0.tar", max compression
+gzip compressed data, was "nsj_flask_utils-0.1.1.tar", max compression
```

## Comparing `nsj_flask_utils-0.1.0.tar` & `nsj_flask_utils-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       72 2023-08-04 20:16:13.230462 nsj_flask_utils-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-08-04 19:16:54.719394 nsj_flask_utils-0.1.0/nsj_flask_utils/__init__.py
--rw-r--r--   0        0        0       53 2023-08-04 20:08:10.746192 nsj_flask_utils-0.1.0/nsj_flask_utils/daos/__init__.py
--rw-r--r--   0        0        0     3153 2023-08-04 19:58:22.274631 nsj_flask_utils-0.1.0/nsj_flask_utils/daos/base_dao.py
--rw-r--r--   0        0        0       53 2023-08-04 20:08:26.739234 nsj_flask_utils-0.1.0/nsj_flask_utils/dtos/__init__.py
--rw-r--r--   0        0        0      212 2023-08-04 18:49:58.954112 nsj_flask_utils-0.1.0/nsj_flask_utils/dtos/base_dto.py
--rw-r--r--   0        0        0      629 2023-08-04 19:15:17.291078 nsj_flask_utils-0.1.0/nsj_flask_utils/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 18:34:53.078783 nsj_flask_utils-0.1.0/nsj_flask_utils/service/__init__.py
--rw-r--r--   0        0        0     3077 2023-08-04 20:14:05.516126 nsj_flask_utils-0.1.0/nsj_flask_utils/service/base_service.py
--rw-r--r--   0        0        0      212 2023-08-04 20:01:49.619187 nsj_flask_utils-0.1.0/nsj_flask_utils/utils/__init__.py
--rw-r--r--   0        0        0     1059 2023-08-04 19:16:06.086236 nsj_flask_utils-0.1.0/nsj_flask_utils/utils/error_handlers.py
--rw-r--r--   0        0        0      147 2023-07-06 20:22:50.549765 nsj_flask_utils-0.1.0/nsj_flask_utils/utils/filter_params.py
--rw-r--r--   0        0        0      434 2023-08-04 19:57:27.085483 nsj_flask_utils-0.1.0/nsj_flask_utils/utils/json.py
--rw-r--r--   0        0        0     1051 2023-08-04 19:04:40.476273 nsj_flask_utils-0.1.0/nsj_flask_utils/utils/pagination_params.py
--rw-r--r--   0        0        0     2953 2023-08-04 19:59:57.791888 nsj_flask_utils-0.1.0/nsj_flask_utils/utils/request_args.py
--rw-r--r--   0        0        0      508 2023-08-04 19:46:17.982703 nsj_flask_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 nsj_flask_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-08-04 20:16:13.230462 nsj_flask_utils-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 19:16:54.719394 nsj_flask_utils-0.1.1/nsj_flask_utils/__init__.py
+-rw-r--r--   0        0        0       53 2023-08-04 20:08:10.746192 nsj_flask_utils-0.1.1/nsj_flask_utils/daos/__init__.py
+-rw-r--r--   0        0        0     3153 2023-08-04 19:58:22.274631 nsj_flask_utils-0.1.1/nsj_flask_utils/daos/base_dao.py
+-rw-r--r--   0        0        0       53 2023-08-04 20:08:26.739234 nsj_flask_utils-0.1.1/nsj_flask_utils/dtos/__init__.py
+-rw-r--r--   0        0        0      212 2023-08-04 18:49:58.954112 nsj_flask_utils-0.1.1/nsj_flask_utils/dtos/base_dto.py
+-rw-r--r--   0        0        0      629 2023-08-04 19:15:17.291078 nsj_flask_utils-0.1.1/nsj_flask_utils/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 19:42:03.906006 nsj_flask_utils-0.1.1/nsj_flask_utils/py.typed
+-rw-r--r--   0        0        0        0 2023-08-04 18:34:53.078783 nsj_flask_utils-0.1.1/nsj_flask_utils/service/__init__.py
+-rw-r--r--   0        0        0     3077 2023-08-04 20:14:05.516126 nsj_flask_utils-0.1.1/nsj_flask_utils/service/base_service.py
+-rw-r--r--   0        0        0      212 2023-08-04 20:01:49.619187 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/__init__.py
+-rw-r--r--   0        0        0     1059 2023-08-04 19:16:06.086236 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/error_handlers.py
+-rw-r--r--   0        0        0      147 2023-07-06 20:22:50.549765 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/filter_params.py
+-rw-r--r--   0        0        0      434 2023-08-04 19:57:27.085483 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/json.py
+-rw-r--r--   0        0        0     1051 2023-08-04 19:04:40.476273 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/pagination_params.py
+-rw-r--r--   0        0        0     2953 2023-08-04 19:59:57.791888 nsj_flask_utils-0.1.1/nsj_flask_utils/utils/request_args.py
+-rw-r--r--   0        0        0      508 2023-08-07 19:43:59.133159 nsj_flask_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 nsj_flask_utils-0.1.1/PKG-INFO
```

### Comparing `nsj_flask_utils-0.1.0/nsj_flask_utils/daos/base_dao.py` & `nsj_flask_utils-0.1.1/nsj_flask_utils/daos/base_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.0/nsj_flask_utils/exceptions/__init__.py` & `nsj_flask_utils-0.1.1/nsj_flask_utils/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.0/nsj_flask_utils/service/base_service.py` & `nsj_flask_utils-0.1.1/nsj_flask_utils/service/base_service.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.0/nsj_flask_utils/utils/error_handlers.py` & `nsj_flask_utils-0.1.1/nsj_flask_utils/utils/error_handlers.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.0/nsj_flask_utils/utils/pagination_params.py` & `nsj_flask_utils-0.1.1/nsj_flask_utils/utils/pagination_params.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.0/nsj_flask_utils/utils/request_args.py` & `nsj_flask_utils-0.1.1/nsj_flask_utils/utils/request_args.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.0/PKG-INFO` & `nsj_flask_utils-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-flask-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utils for Flask
 License: MIT
 Author: Vinicius Teshima
 Author-email: viniciusteshima@nasajon.com.br
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

