# Comparing `tmp/macrometa-target-collection-0.0.82.tar.gz` & `tmp/macrometa-target-collection-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.82.tar", last modified: Mon Jul 17 05:29:03 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.83.tar", last modified: Mon Aug  7 15:58:46 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.82.tar` & `macrometa-target-collection-0.0.83.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:29:03.271810 macrometa-target-collection-0.0.82/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-07-17 05:28:38.000000 macrometa-target-collection-0.0.82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-17 05:29:03.271810 macrometa-target-collection-0.0.82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 05:28:38.000000 macrometa-target-collection-0.0.82/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:29:03.271810 macrometa-target-collection-0.0.82/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-17 05:28:38.000000 macrometa-target-collection-0.0.82/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16617 2023-07-17 05:28:38.000000 macrometa-target-collection-0.0.82/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:29:03.271810 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 05:29:03.000000 macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-17 05:28:38.000000 macrometa-target-collection-0.0.82/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 05:29:03.271810 macrometa-target-collection-0.0.82/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:46.435134 macrometa-target-collection-0.0.83/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-08-07 15:58:24.000000 macrometa-target-collection-0.0.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-08-07 15:58:46.435134 macrometa-target-collection-0.0.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-07 15:58:24.000000 macrometa-target-collection-0.0.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:46.431134 macrometa-target-collection-0.0.83/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-08-07 15:58:24.000000 macrometa-target-collection-0.0.83/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16617 2023-08-07 15:58:24.000000 macrometa-target-collection-0.0.83/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:46.431134 macrometa-target-collection-0.0.83/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-08-07 15:58:46.000000 macrometa-target-collection-0.0.83/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-07 15:58:46.000000 macrometa-target-collection-0.0.83/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:58:46.000000 macrometa-target-collection-0.0.83/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-07 15:58:46.000000 macrometa-target-collection-0.0.83/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 15:58:46.000000 macrometa-target-collection-0.0.83/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 15:58:46.000000 macrometa-target-collection-0.0.83/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-07 15:58:24.000000 macrometa-target-collection-0.0.83/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 15:58:46.435134 macrometa-target-collection-0.0.83/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.82/LICENSE` & `macrometa-target-collection-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.82/PKG-INFO` & `macrometa-target-collection-0.0.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.82
+Version: 0.0.83
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.82/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.83/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.82/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.83/macrometa_target_collection/main.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.82/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.83/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.82
+Version: 0.0.83
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.82/pyproject.toml` & `macrometa-target-collection-0.0.83/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.82"
+version = "0.0.83"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
     'pipelinewise-singer-python==1.2.0',
     'adjust-precision-for-schema==0.3.4',
-    'pyc8==0.17.1',
+    'pyc8==1.0.1',
     'c8connector>=0.0.29',
     'prometheus-client==0.16.0'
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Operating System :: OS Independent",
```

