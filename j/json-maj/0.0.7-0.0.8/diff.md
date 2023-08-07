# Comparing `tmp/json_maj-0.0.7.tar.gz` & `tmp/json_maj-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_maj-0.0.7.tar", max compression
+gzip compressed data, was "json_maj-0.0.8.tar", max compression
```

## Comparing `json_maj-0.0.7.tar` & `json_maj-0.0.8.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0        0 2022-09-08 19:12:31.249636 json_maj-0.0.7/json_maj/__init__.py
--rw-r--r--   0        0        0     2364 2022-09-08 19:12:31.249753 json_maj-0.0.7/json_maj/cli.py
--rwxr-xr-x   0        0        0     1841 2022-09-08 19:12:31.249875 json_maj-0.0.7/json_maj/create_executable.py
--rw-r--r--   0        0        0     2346 2022-11-03 19:53:39.587337 json_maj-0.0.7/json_maj/main.py
--rw-r--r--   0        0        0      490 2022-11-03 19:40:19.515058 json_maj-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 json_maj-0.0.7/setup.py
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 json_maj-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-08 19:12:31.249636 json_maj-0.0.8/json_maj/__init__.py
+-rw-r--r--   0        0        0     4317 2023-08-07 19:42:37.920672 json_maj-0.0.8/json_maj/cli.py
+-rwxr-xr-x   0        0        0     1841 2022-09-08 19:12:31.249875 json_maj-0.0.8/json_maj/create_executable.py
+-rw-r--r--   0        0        0     2346 2022-11-03 19:53:39.587337 json_maj-0.0.8/json_maj/main.py
+-rw-r--r--   0        0        0      490 2023-08-07 19:43:41.708792 json_maj-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 json_maj-0.0.8/PKG-INFO
```

### Comparing `json_maj-0.0.7/json_maj/create_executable.py` & `json_maj-0.0.8/json_maj/create_executable.py`

 * *Files identical despite different names*

### Comparing `json_maj-0.0.7/json_maj/main.py` & `json_maj-0.0.8/json_maj/main.py`

 * *Files identical despite different names*

### Comparing `json_maj-0.0.7/PKG-INFO` & `json_maj-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: json-maj
-Version: 0.0.7
+Version: 0.0.8
 Summary: Updates Jsons w/ json, key pair, or entire dictionary as arguments
 License: MIT
 Author: anthony galassi
 Author-email: 28850131+bendhouseart@users.noreply.github.com
 Requires-Python: >=3.5,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

