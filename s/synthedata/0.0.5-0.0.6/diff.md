# Comparing `tmp/synthedata-0.0.5.tar.gz` & `tmp/synthedata-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/synthedata-0.0.5.tar", last modified: Fri Aug  4 18:47:09 2023, max compression
+gzip compressed data, was "dist/synthedata-0.0.6.tar", last modified: Mon Aug  7 20:03:21 2023, max compression
```

## Comparing `synthedata-0.0.5.tar` & `synthedata-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-08-04 18:47:09.357787 synthedata-0.0.5/
--rw-r--r--   0 annli      (501) staff       (20)     8768 2023-08-04 18:47:09.357342 synthedata-0.0.5/PKG-INFO
--rw-r--r--   0 annli      (501) staff       (20)     7176 2023-05-25 20:34:45.000000 synthedata-0.0.5/README.md
--rw-r--r--   0 annli      (501) staff       (20)       38 2023-08-04 18:47:09.358004 synthedata-0.0.5/setup.cfg
--rw-r--r--   0 annli      (501) staff       (20)      662 2023-08-04 18:38:38.000000 synthedata-0.0.5/setup.py
-drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-08-04 18:47:09.351648 synthedata-0.0.5/synthedata/
--rw-r--r--   0 annli      (501) staff       (20)       18 2023-05-25 20:33:58.000000 synthedata-0.0.5/synthedata/__init__.py
--rw-r--r--   0 annli      (501) staff       (20)    33531 2023-08-04 18:36:02.000000 synthedata-0.0.5/synthedata/data_creator.py
-drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-08-04 18:47:09.355675 synthedata-0.0.5/synthedata.egg-info/
--rw-r--r--   0 annli      (501) staff       (20)     8768 2023-08-04 18:47:09.000000 synthedata-0.0.5/synthedata.egg-info/PKG-INFO
--rw-r--r--   0 annli      (501) staff       (20)      204 2023-08-04 18:47:09.000000 synthedata-0.0.5/synthedata.egg-info/SOURCES.txt
--rw-r--r--   0 annli      (501) staff       (20)        1 2023-08-04 18:47:09.000000 synthedata-0.0.5/synthedata.egg-info/dependency_links.txt
--rw-r--r--   0 annli      (501) staff       (20)       11 2023-08-04 18:47:09.000000 synthedata-0.0.5/synthedata.egg-info/top_level.txt
+drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-08-07 20:03:21.645569 synthedata-0.0.6/
+-rw-r--r--   0 annli      (501) staff       (20)     8768 2023-08-07 20:03:21.644838 synthedata-0.0.6/PKG-INFO
+-rw-r--r--   0 annli      (501) staff       (20)     7176 2023-05-25 20:34:45.000000 synthedata-0.0.6/README.md
+-rw-r--r--   0 annli      (501) staff       (20)       38 2023-08-07 20:03:21.645915 synthedata-0.0.6/setup.cfg
+-rw-r--r--   0 annli      (501) staff       (20)      662 2023-08-07 20:02:19.000000 synthedata-0.0.6/setup.py
+drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-08-07 20:03:21.640541 synthedata-0.0.6/synthedata/
+-rw-r--r--   0 annli      (501) staff       (20)       18 2023-05-25 20:33:58.000000 synthedata-0.0.6/synthedata/__init__.py
+-rw-r--r--   0 annli      (501) staff       (20)    33531 2023-08-04 18:36:02.000000 synthedata-0.0.6/synthedata/data_creator.py
+drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-08-07 20:03:21.643734 synthedata-0.0.6/synthedata.egg-info/
+-rw-r--r--   0 annli      (501) staff       (20)     8768 2023-08-07 20:03:21.000000 synthedata-0.0.6/synthedata.egg-info/PKG-INFO
+-rw-r--r--   0 annli      (501) staff       (20)      204 2023-08-07 20:03:21.000000 synthedata-0.0.6/synthedata.egg-info/SOURCES.txt
+-rw-r--r--   0 annli      (501) staff       (20)        1 2023-08-07 20:03:21.000000 synthedata-0.0.6/synthedata.egg-info/dependency_links.txt
+-rw-r--r--   0 annli      (501) staff       (20)       11 2023-08-07 20:03:21.000000 synthedata-0.0.6/synthedata.egg-info/top_level.txt
```

### Comparing `synthedata-0.0.5/PKG-INFO` & `synthedata-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthedata
-Version: 0.0.5
+Version: 0.0.6
 Summary: A synthetic data creator package
 Home-page: https://github.com/fau-syn-data/synthetic-data.git
 Author: BACS_group1
 Author-email: fausyndata@gmail.com
 License: UNKNOWN
 Description: ﻿# Welcome to StackEdit!
```

### Comparing `synthedata-0.0.5/README.md` & `synthedata-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `synthedata-0.0.5/setup.py` & `synthedata-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="synthedata",
-    version="0.0.5",
+    version="0.0.6",
     author="BACS_group1",
     author_email="fausyndata@gmail.com",
     description="A synthetic data creator package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fau-syn-data/synthetic-data.git",
     #packages=setuptools.find_packages(),
```

### Comparing `synthedata-0.0.5/synthedata/data_creator.py` & `synthedata-0.0.6/synthedata/data_creator.py`

 * *Files identical despite different names*

### Comparing `synthedata-0.0.5/synthedata.egg-info/PKG-INFO` & `synthedata-0.0.6/synthedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthedata
-Version: 0.0.5
+Version: 0.0.6
 Summary: A synthetic data creator package
 Home-page: https://github.com/fau-syn-data/synthetic-data.git
 Author: BACS_group1
 Author-email: fausyndata@gmail.com
 License: UNKNOWN
 Description: ﻿# Welcome to StackEdit!
```

