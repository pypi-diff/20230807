# Comparing `tmp/airthings_ble-0.5.6.post3.tar.gz` & `tmp/airthings_ble-0.5.6.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airthings_ble-0.5.6.post3.tar", max compression
+gzip compressed data, was "airthings_ble-0.5.6.post4.tar", max compression
```

## Comparing `airthings_ble-0.5.6.post3.tar` & `airthings_ble-0.5.6.post4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2023-08-07 16:51:31.916774 airthings_ble-0.5.6.post3/LICENSE
--rw-r--r--   0        0        0      113 2023-08-07 16:51:31.916774 airthings_ble-0.5.6.post3/README.md
--rw-r--r--   0        0        0      238 2023-08-07 16:51:33.860835 airthings_ble-0.5.6.post3/airthings_ble/__init__.py
--rw-r--r--   0        0        0     2109 2023-08-07 16:51:31.916774 airthings_ble-0.5.6.post3/airthings_ble/const.py
--rw-r--r--   0        0        0    20993 2023-08-07 16:51:31.916774 airthings_ble-0.5.6.post3/airthings_ble/parser.py
--rw-r--r--   0        0        0        0 2023-08-07 16:51:31.916774 airthings_ble-0.5.6.post3/airthings_ble/py.typed
--rw-r--r--   0        0        0     2161 2023-08-07 16:51:33.832834 airthings_ble-0.5.6.post3/pyproject.toml
--rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 airthings_ble-0.5.6.post3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-08-07 16:54:34.894154 airthings_ble-0.5.6.post4/LICENSE
+-rw-r--r--   0        0        0      113 2023-08-07 16:54:34.894154 airthings_ble-0.5.6.post4/README.md
+-rw-r--r--   0        0        0      238 2023-08-07 16:54:37.150328 airthings_ble-0.5.6.post4/airthings_ble/__init__.py
+-rw-r--r--   0        0        0     2109 2023-08-07 16:54:34.894154 airthings_ble-0.5.6.post4/airthings_ble/const.py
+-rw-r--r--   0        0        0    20993 2023-08-07 16:54:34.894154 airthings_ble-0.5.6.post4/airthings_ble/parser.py
+-rw-r--r--   0        0        0        0 2023-08-07 16:54:34.894154 airthings_ble-0.5.6.post4/airthings_ble/py.typed
+-rw-r--r--   0        0        0     2161 2023-08-07 16:54:37.118325 airthings_ble-0.5.6.post4/pyproject.toml
+-rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 airthings_ble-0.5.6.post4/PKG-INFO
```

### Comparing `airthings_ble-0.5.6.post3/LICENSE` & `airthings_ble-0.5.6.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.5.6.post3/airthings_ble/const.py` & `airthings_ble-0.5.6.post4/airthings_ble/const.py`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.5.6.post3/airthings_ble/parser.py` & `airthings_ble-0.5.6.post4/airthings_ble/parser.py`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.5.6.post3/pyproject.toml` & `airthings_ble-0.5.6.post4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airthings-ble"
-version = "v0.5.6-3"
+version = "v0.5.6-4"
 description = "Manage Airthings BLE devices"
 authors = ["Vincent Giorgi"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/vincegio/airthings-ble"
 documentation = "https://airthings-ble.readthedocs.io"
 classifiers = [
```

### Comparing `airthings_ble-0.5.6.post3/PKG-INFO` & `airthings_ble-0.5.6.post4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airthings-ble
-Version: 0.5.6.post3
+Version: 0.5.6.post4
 Summary: Manage Airthings BLE devices
 Home-page: https://github.com/vincegio/airthings-ble
 License: Apache Software License 2.0
 Author: Vincent Giorgi
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

