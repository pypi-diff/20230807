# Comparing `tmp/skcan-compare-0.0.1.tar.gz` & `tmp/skcan-compare-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skcan-compare-0.0.1.tar", last modified: Mon Aug  7 08:27:34 2023, max compression
+gzip compressed data, was "skcan-compare-0.0.2.tar", last modified: Mon Aug  7 10:50:29 2023, max compression
```

## Comparing `skcan-compare-0.0.1.tar` & `skcan-compare-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-07 08:27:34.627574 skcan-compare-0.0.1/
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    11356 2023-08-07 08:19:50.000000 skcan-compare-0.0.1/LICENSE
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-07 08:27:34.627574 skcan-compare-0.0.1/PKG-INFO
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     1325 2023-08-05 14:05:19.000000 skcan-compare-0.0.1/README.md
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       38 2023-08-07 08:27:34.627574 skcan-compare-0.0.1/setup.cfg
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      901 2023-08-07 08:23:58.000000 skcan-compare-0.0.1/setup.py
-drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-07 08:27:34.627574 skcan-compare-0.0.1/skcan_compare/
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)        0 2023-08-07 07:48:50.000000 skcan-compare-0.0.1/skcan_compare/__init__.py
-drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-07 08:27:34.627574 skcan-compare-0.0.1/skcan_compare.egg-info/
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-07 08:27:34.000000 skcan-compare-0.0.1/skcan_compare.egg-info/PKG-INFO
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      200 2023-08-07 08:27:34.000000 skcan-compare-0.0.1/skcan_compare.egg-info/SOURCES.txt
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)        1 2023-08-07 08:27:34.000000 skcan-compare-0.0.1/skcan_compare.egg-info/dependency_links.txt
--rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       14 2023-08-07 08:27:34.000000 skcan-compare-0.0.1/skcan_compare.egg-info/top_level.txt
+drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-07 10:50:29.123831 skcan-compare-0.0.2/
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)    11356 2023-08-07 08:19:50.000000 skcan-compare-0.0.2/LICENSE
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-07 10:50:29.123831 skcan-compare-0.0.2/PKG-INFO
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     1325 2023-08-05 14:05:19.000000 skcan-compare-0.0.2/README.md
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       38 2023-08-07 10:50:29.123831 skcan-compare-0.0.2/setup.cfg
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      914 2023-08-07 10:50:25.000000 skcan-compare-0.0.2/setup.py
+drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-07 10:50:29.119831 skcan-compare-0.0.2/skcan_compare/
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     2114 2023-08-07 10:46:37.000000 skcan-compare-0.0.2/skcan_compare/__init__.py
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       73 2023-08-07 09:47:01.000000 skcan-compare-0.0.2/skcan_compare/globals.py
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     2745 2023-08-07 08:52:05.000000 skcan-compare-0.0.2/skcan_compare/query.py
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)     7944 2023-08-07 10:36:02.000000 skcan-compare-0.0.2/skcan_compare/visualize.py
+drwxrwxr-x   0 shailesh  (1000) shailesh  (1000)        0 2023-08-07 10:50:29.123831 skcan-compare-0.0.2/skcan_compare.egg-info/
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      412 2023-08-07 10:50:29.000000 skcan-compare-0.0.2/skcan_compare.egg-info/PKG-INFO
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)      275 2023-08-07 10:50:29.000000 skcan-compare-0.0.2/skcan_compare.egg-info/SOURCES.txt
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)        1 2023-08-07 10:50:29.000000 skcan-compare-0.0.2/skcan_compare.egg-info/dependency_links.txt
+-rw-rw-r--   0 shailesh  (1000) shailesh  (1000)       14 2023-08-07 10:50:29.000000 skcan-compare-0.0.2/skcan_compare.egg-info/top_level.txt
```

### Comparing `skcan-compare-0.0.1/LICENSE` & `skcan-compare-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skcan-compare-0.0.1/README.md` & `skcan-compare-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `skcan-compare-0.0.1/setup.py` & `skcan-compare-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Author: Shailesh Appukuttan
 Date: 07/08/2023
 """
 import os
 from setuptools import setup, find_packages
 
-def package_files(directory):
+def package_files(base_dir, directory):
     """function to load package data"""
     paths = []
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join('..', path, filename))
     return paths
 
-json_files = package_files('skcan_compare/data')
+json_files = package_files("skcan_compare", "data")
 
 setup(
     name="skcan-compare",
-    version="0.0.1",
+    version="0.0.2",
     description="A package for retrieving and visualizing data contained in     SCKAN (e.g., across species, relationship to spinal segments) to highlight similarities and differences in neuronal pathways",
     author="Shailesh Appukuttan, Hiba Ben Aribi, Pranjal Garg, Gautam Kumar",
     author_email="appukuttan.shailesh@gmail.com",
     license="Apache-2.0",
     package_data={"": json_files},
     packages=find_packages(),
 )
```

