# Comparing `tmp/tensorflow-ml-1.1.tar.gz` & `tmp/tensorflow-ml-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow-ml-1.1.tar", last modified: Sun Aug  6 21:04:02 2023, max compression
+gzip compressed data, was "tensorflow-ml-1.1.1.tar", last modified: Sun Aug  6 22:26:28 2023, max compression
```

## Comparing `tensorflow-ml-1.1.tar` & `tensorflow-ml-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:04:02.706984 tensorflow-ml-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-06 21:01:34.000000 tensorflow-ml-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-08-06 21:04:02.706984 tensorflow-ml-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-08-06 21:01:34.000000 tensorflow-ml-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 21:04:02.706984 tensorflow-ml-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-06 21:01:34.000000 tensorflow-ml-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:04:02.706984 tensorflow-ml-1.1/tensorflow_ml/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-06 21:01:34.000000 tensorflow-ml-1.1/tensorflow_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:04:02.706984 tensorflow-ml-1.1/tensorflow_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-08-06 21:04:02.000000 tensorflow-ml-1.1/tensorflow_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-06 21:04:02.000000 tensorflow-ml-1.1/tensorflow_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 21:04:02.000000 tensorflow-ml-1.1/tensorflow_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-06 21:04:02.000000 tensorflow-ml-1.1/tensorflow_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-06 21:04:02.000000 tensorflow-ml-1.1/tensorflow_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:26:28.033131 tensorflow-ml-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-06 22:24:10.000000 tensorflow-ml-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-08-06 22:26:28.033131 tensorflow-ml-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-08-06 22:24:10.000000 tensorflow-ml-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 22:26:28.033131 tensorflow-ml-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-06 22:24:10.000000 tensorflow-ml-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:26:28.029131 tensorflow-ml-1.1.1/tensorflow_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-06 22:24:10.000000 tensorflow-ml-1.1.1/tensorflow_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:26:28.033131 tensorflow-ml-1.1.1/tensorflow_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-08-06 22:26:27.000000 tensorflow-ml-1.1.1/tensorflow_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-06 22:26:28.000000 tensorflow-ml-1.1.1/tensorflow_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 22:26:27.000000 tensorflow-ml-1.1.1/tensorflow_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-06 22:26:27.000000 tensorflow-ml-1.1.1/tensorflow_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-06 22:26:27.000000 tensorflow-ml-1.1.1/tensorflow_ml.egg-info/top_level.txt
```

### Comparing `tensorflow-ml-1.1/LICENSE` & `tensorflow-ml-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1/PKG-INFO` & `tensorflow-ml-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-ml
-Version: 1.1
+Version: 1.1.1
 Summary: Tensorflow ML
 Author: Siddhant Pathak
 Author-email: siddhantpathak2@gmail.com
 Keywords: python,tensorflow,ml,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `tensorflow-ml-1.1/README.md` & `tensorflow-ml-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1/setup.py` & `tensorflow-ml-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '1.1' 
+VERSION = '1.1.1' 
 
 DESCRIPTION = 'Tensorflow ML'
 
 with open("README.md", 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 lib_folder = os.path.dirname(os.path.realpath(__file__))
```

### Comparing `tensorflow-ml-1.1/tensorflow_ml.egg-info/PKG-INFO` & `tensorflow-ml-1.1.1/tensorflow_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-ml
-Version: 1.1
+Version: 1.1.1
 Summary: Tensorflow ML
 Author: Siddhant Pathak
 Author-email: siddhantpathak2@gmail.com
 Keywords: python,tensorflow,ml,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `tensorflow-ml-1.1/tensorflow_ml.egg-info/requires.txt` & `tensorflow-ml-1.1.1/tensorflow_ml.egg-info/requires.txt`

 * *Files identical despite different names*

