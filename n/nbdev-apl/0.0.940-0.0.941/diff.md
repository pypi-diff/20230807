# Comparing `tmp/nbdev-apl-0.0.940.tar.gz` & `tmp/nbdev-apl-0.0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdev-apl-0.0.940.tar", last modified: Sun Aug  6 13:16:19 2023, max compression
+gzip compressed data, was "nbdev-apl-0.0.941.tar", last modified: Mon Aug  7 01:43:18 2023, max compression
```

## Comparing `nbdev-apl-0.0.940.tar` & `nbdev-apl-0.0.941.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:16:19.498844 nbdev-apl-0.0.940/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-06 13:05:11.000000 nbdev-apl-0.0.940/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-06 13:05:11.000000 nbdev-apl-0.0.940/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-06 13:16:19.498844 nbdev-apl-0.0.940/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 13:05:11.000000 nbdev-apl-0.0.940/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:16:19.498844 nbdev-apl-0.0.940/nbdev_apl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:16:19.000000 nbdev-apl-0.0.940/nbdev_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-08-06 13:05:11.000000 nbdev-apl-0.0.940/nbdev_apl/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-06 13:16:19.000000 nbdev-apl-0.0.940/nbdev_apl/_nbdev.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:16:19.498844 nbdev-apl-0.0.940/nbdev_apl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-06 13:16:19.000000 nbdev-apl-0.0.940/nbdev_apl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-06 13:16:19.000000 nbdev-apl-0.0.940/nbdev_apl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:16:19.000000 nbdev-apl-0.0.940/nbdev_apl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-06 13:16:19.000000 nbdev-apl-0.0.940/nbdev_apl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:16:19.000000 nbdev-apl-0.0.940/nbdev_apl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-06 13:16:19.000000 nbdev-apl-0.0.940/nbdev_apl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 13:16:19.000000 nbdev-apl-0.0.940/nbdev_apl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-06 13:16:19.000000 nbdev-apl-0.0.940/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 13:16:19.498844 nbdev-apl-0.0.940/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-06 13:05:11.000000 nbdev-apl-0.0.940/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:43:18.449327 nbdev-apl-0.0.941/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 01:31:48.000000 nbdev-apl-0.0.941/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-07 01:31:48.000000 nbdev-apl-0.0.941/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-07 01:43:18.449327 nbdev-apl-0.0.941/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-07 01:31:48.000000 nbdev-apl-0.0.941/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:43:18.449327 nbdev-apl-0.0.941/nbdev_apl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 01:43:18.000000 nbdev-apl-0.0.941/nbdev_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-08-07 01:31:48.000000 nbdev-apl-0.0.941/nbdev_apl/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-07 01:43:18.000000 nbdev-apl-0.0.941/nbdev_apl/_nbdev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:43:18.449327 nbdev-apl-0.0.941/nbdev_apl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-07 01:43:18.000000 nbdev-apl-0.0.941/nbdev_apl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-07 01:43:18.000000 nbdev-apl-0.0.941/nbdev_apl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 01:43:18.000000 nbdev-apl-0.0.941/nbdev_apl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-07 01:43:18.000000 nbdev-apl-0.0.941/nbdev_apl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 01:43:18.000000 nbdev-apl-0.0.941/nbdev_apl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 01:43:18.000000 nbdev-apl-0.0.941/nbdev_apl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 01:43:18.000000 nbdev-apl-0.0.941/nbdev_apl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-07 01:43:18.000000 nbdev-apl-0.0.941/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 01:43:18.449327 nbdev-apl-0.0.941/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-07 01:31:48.000000 nbdev-apl-0.0.941/setup.py
```

### Comparing `nbdev-apl-0.0.940/LICENSE` & `nbdev-apl-0.0.941/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdev-apl-0.0.940/PKG-INFO` & `nbdev-apl-0.0.941/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev-apl
-Version: 0.0.940
+Version: 0.0.941
 Summary: nbdev docs lookup for numpy
 Home-page: https://github.com/fastai/nbdev-index/tree/master/
 Author: Jeremy Howard
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: nbdev fastai python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nbdev-apl-0.0.940/nbdev_apl/_modidx.py` & `nbdev-apl-0.0.941/nbdev_apl/_modidx.py`

 * *Files identical despite different names*

### Comparing `nbdev-apl-0.0.940/nbdev_apl.egg-info/PKG-INFO` & `nbdev-apl-0.0.941/nbdev_apl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev-apl
-Version: 0.0.940
+Version: 0.0.941
 Summary: nbdev docs lookup for numpy
 Home-page: https://github.com/fastai/nbdev-index/tree/master/
 Author: Jeremy Howard
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: nbdev fastai python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nbdev-apl-0.0.940/settings.ini` & `nbdev-apl-0.0.941/settings.ini`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = fastai
 description = nbdev docs lookup for numpy
 keywords = nbdev fastai python
 author = Jeremy Howard
 author_email = info@fast.ai
 copyright = fast.ai, inc
 branch = master
-version = 0.0.940
+version = 0.0.941
 min_python = 3.6
 audience = Developers
 language = English
 license = apache2
 status = 2
 lib_path = nbdev_apl
 nbs_path = .
```

### Comparing `nbdev-apl-0.0.940/setup.py` & `nbdev-apl-0.0.941/setup.py`

 * *Files identical despite different names*

