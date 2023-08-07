# Comparing `tmp/sherpa-onnx-1.6.0.tar.gz` & `tmp/sherpa-onnx-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.6.0.tar", last modified: Mon Aug  7 05:09:29 2023, max compression
+gzip compressed data, was "sherpa-onnx-1.6.1.tar", last modified: Mon Aug  7 12:32:39 2023, max compression
```

## Comparing `sherpa-onnx-1.6.0.tar` & `sherpa-onnx-1.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/sherpa-onnx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/sherpa-onnx/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-07 04:56:02.000000 sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:29.709365 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 05:09:29.000000 sherpa-onnx-1.6.0/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:32:39.444085 sherpa-onnx-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-07 12:20:53.000000 sherpa-onnx-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-07 12:32:39.444085 sherpa-onnx-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-07 12:20:53.000000 sherpa-onnx-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 12:32:39.444085 sherpa-onnx-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-07 12:20:53.000000 sherpa-onnx-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:32:39.444085 sherpa-onnx-1.6.1/sherpa-onnx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:32:39.444085 sherpa-onnx-1.6.1/sherpa-onnx/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:32:39.444085 sherpa-onnx-1.6.1/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-07 12:32:39.000000 sherpa-onnx-1.6.1/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-08-07 12:20:53.000000 sherpa-onnx-1.6.1/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-08-07 12:20:53.000000 sherpa-onnx-1.6.1/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-07 12:20:53.000000 sherpa-onnx-1.6.1/sherpa-onnx/python/sherpa_onnx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:32:39.444085 sherpa-onnx-1.6.1/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-07 12:32:39.000000 sherpa-onnx-1.6.1/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-07 12:32:39.000000 sherpa-onnx-1.6.1/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:32:39.000000 sherpa-onnx-1.6.1/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:32:39.000000 sherpa-onnx-1.6.1/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 12:32:39.000000 sherpa-onnx-1.6.1/sherpa_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 12:32:39.000000 sherpa-onnx-1.6.1/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.6.0/LICENSE` & `sherpa-onnx-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.6.0/PKG-INFO` & `sherpa-onnx-1.6.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.6.0
+Version: 1.6.1
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.6.0/setup.py` & `sherpa-onnx-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.6.1/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.6.1/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.6.0/sherpa-onnx/python/sherpa_onnx/utils.py` & `sherpa-onnx-1.6.1/sherpa-onnx/python/sherpa_onnx/utils.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.6.0/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.6.1/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.6.0
+Version: 1.6.1
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

