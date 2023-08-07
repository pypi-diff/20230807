# Comparing `tmp/normalize_json-0.0.1.tar.gz` & `tmp/normalize_json-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "normalize_json-0.0.1.tar", last modified: Mon Aug  7 03:02:22 2023, max compression
+gzip compressed data, was "normalize_json-0.0.2.tar", last modified: Mon Aug  7 03:18:28 2023, max compression
```

## Comparing `normalize_json-0.0.1.tar` & `normalize_json-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 03:02:22.075494 normalize_json-0.0.1/
--rw-r--r--   0 mega      (1000) mega      (1000)     1083 2023-08-04 22:32:02.000000 normalize_json-0.0.1/LICENSE
--rw-r--r--   0 mega      (1000) mega      (1000)     4547 2023-08-07 03:02:22.072160 normalize_json-0.0.1/PKG-INFO
--rw-r--r--   0 mega      (1000) mega      (1000)     4114 2023-08-07 01:23:20.000000 normalize_json-0.0.1/README.md
--rw-r--r--   0 mega      (1000) mega      (1000)      423 2023-08-07 00:24:22.000000 normalize_json-0.0.1/pyproject.toml
--rw-r--r--   0 mega      (1000) mega      (1000)       38 2023-08-07 03:02:22.075494 normalize_json-0.0.1/setup.cfg
-drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 03:02:22.072160 normalize_json-0.0.1/src/
--rw-r--r--   0 mega      (1000) mega      (1000)       25 2023-08-04 23:11:44.000000 normalize_json-0.0.1/src/__init__.py
--rw-r--r--   0 mega      (1000) mega      (1000)     1410 2023-08-05 00:11:28.000000 normalize_json-0.0.1/src/cli.py
--rw-r--r--   0 mega      (1000) mega      (1000)     6699 2023-08-07 01:19:01.000000 normalize_json-0.0.1/src/normalize.py
-drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 03:02:22.072160 normalize_json-0.0.1/src/normalize_json.egg-info/
--rw-r--r--   0 mega      (1000) mega      (1000)     4547 2023-08-07 03:02:22.000000 normalize_json-0.0.1/src/normalize_json.egg-info/PKG-INFO
--rw-r--r--   0 mega      (1000) mega      (1000)      244 2023-08-07 03:02:22.000000 normalize_json-0.0.1/src/normalize_json.egg-info/SOURCES.txt
--rw-r--r--   0 mega      (1000) mega      (1000)        1 2023-08-07 03:02:22.000000 normalize_json-0.0.1/src/normalize_json.egg-info/dependency_links.txt
--rw-r--r--   0 mega      (1000) mega      (1000)       23 2023-08-07 03:02:22.000000 normalize_json-0.0.1/src/normalize_json.egg-info/top_level.txt
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 03:18:28.725555 normalize_json-0.0.2/
+-rw-r--r--   0 mega      (1000) mega      (1000)     1083 2023-08-04 22:32:02.000000 normalize_json-0.0.2/LICENSE
+-rw-r--r--   0 mega      (1000) mega      (1000)     4547 2023-08-07 03:18:28.725555 normalize_json-0.0.2/PKG-INFO
+-rw-r--r--   0 mega      (1000) mega      (1000)     4114 2023-08-07 01:23:20.000000 normalize_json-0.0.2/README.md
+-rw-r--r--   0 mega      (1000) mega      (1000)      506 2023-08-07 03:17:38.000000 normalize_json-0.0.2/pyproject.toml
+-rw-r--r--   0 mega      (1000) mega      (1000)       38 2023-08-07 03:18:28.725555 normalize_json-0.0.2/setup.cfg
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 03:18:28.725555 normalize_json-0.0.2/src/
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 03:18:28.725555 normalize_json-0.0.2/src/normalize_json/
+-rw-r--r--   0 mega      (1000) mega      (1000)       25 2023-08-04 23:11:44.000000 normalize_json-0.0.2/src/normalize_json/__init__.py
+-rw-r--r--   0 mega      (1000) mega      (1000)     1410 2023-08-05 00:11:28.000000 normalize_json-0.0.2/src/normalize_json/cli.py
+-rw-r--r--   0 mega      (1000) mega      (1000)     6699 2023-08-07 01:19:01.000000 normalize_json-0.0.2/src/normalize_json/normalize.py
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 03:18:28.725555 normalize_json-0.0.2/src/normalize_json.egg-info/
+-rw-r--r--   0 mega      (1000) mega      (1000)     4547 2023-08-07 03:18:28.000000 normalize_json-0.0.2/src/normalize_json.egg-info/PKG-INFO
+-rw-r--r--   0 mega      (1000) mega      (1000)      289 2023-08-07 03:18:28.000000 normalize_json-0.0.2/src/normalize_json.egg-info/SOURCES.txt
+-rw-r--r--   0 mega      (1000) mega      (1000)        1 2023-08-07 03:18:28.000000 normalize_json-0.0.2/src/normalize_json.egg-info/dependency_links.txt
+-rw-r--r--   0 mega      (1000) mega      (1000)       15 2023-08-07 03:18:28.000000 normalize_json-0.0.2/src/normalize_json.egg-info/top_level.txt
```

### Comparing `normalize_json-0.0.1/LICENSE` & `normalize_json-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `normalize_json-0.0.1/PKG-INFO` & `normalize_json-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normalize_json
-Version: 0.0.1
+Version: 0.0.2
 Summary: todo
 Author-email: João Gabriel Santos <joaosan177@gmail.com>
 Project-URL: Homepage, https://github.com/capsulbrasil/normalize-json
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `normalize_json-0.0.1/README.md` & `normalize_json-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `normalize_json-0.0.1/src/cli.py` & `normalize_json-0.0.2/src/normalize_json/cli.py`

 * *Files identical despite different names*

### Comparing `normalize_json-0.0.1/src/normalize.py` & `normalize_json-0.0.2/src/normalize_json/normalize.py`

 * *Files identical despite different names*

### Comparing `normalize_json-0.0.1/src/normalize_json.egg-info/PKG-INFO` & `normalize_json-0.0.2/src/normalize_json.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normalize-json
-Version: 0.0.1
+Version: 0.0.2
 Summary: todo
 Author-email: João Gabriel Santos <joaosan177@gmail.com>
 Project-URL: Homepage, https://github.com/capsulbrasil/normalize-json
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

