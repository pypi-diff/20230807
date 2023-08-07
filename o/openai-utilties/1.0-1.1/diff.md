# Comparing `tmp/openai-utilties-1.0.tar.gz` & `tmp/openai-utilties-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-utilties-1.0.tar", last modified: Mon Aug  7 13:41:26 2023, max compression
+gzip compressed data, was "openai-utilties-1.1.tar", last modified: Mon Aug  7 13:53:16 2023, max compression
```

## Comparing `openai-utilties-1.0.tar` & `openai-utilties-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-07 13:41:26.129138 openai-utilties-1.0/
--rw-r--r--   0 andrewzhuang   (501) staff       (20)     2727 2023-08-07 13:41:26.129001 openai-utilties-1.0/PKG-INFO
--rw-r--r--   0 andrewzhuang   (501) staff       (20)     2210 2023-08-07 13:39:15.000000 openai-utilties-1.0/README.md
-drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-07 13:41:26.127820 openai-utilties-1.0/openai-utils/
--rw-r--r--   0 andrewzhuang   (501) staff       (20)      669 2023-08-07 13:38:20.000000 openai-utilties-1.0/openai-utils/__init__.py
-drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-07 13:41:26.128783 openai-utilties-1.0/openai_utilties.egg-info/
--rw-r--r--   0 andrewzhuang   (501) staff       (20)     2727 2023-08-07 13:41:26.000000 openai-utilties-1.0/openai_utilties.egg-info/PKG-INFO
--rw-r--r--   0 andrewzhuang   (501) staff       (20)      237 2023-08-07 13:41:26.000000 openai-utilties-1.0/openai_utilties.egg-info/SOURCES.txt
--rw-r--r--   0 andrewzhuang   (501) staff       (20)        1 2023-08-07 13:41:26.000000 openai-utilties-1.0/openai_utilties.egg-info/dependency_links.txt
--rw-r--r--   0 andrewzhuang   (501) staff       (20)       13 2023-08-07 13:41:26.000000 openai-utilties-1.0/openai_utilties.egg-info/requires.txt
--rw-r--r--   0 andrewzhuang   (501) staff       (20)       13 2023-08-07 13:41:26.000000 openai-utilties-1.0/openai_utilties.egg-info/top_level.txt
--rw-r--r--   0 andrewzhuang   (501) staff       (20)       38 2023-08-07 13:41:26.129186 openai-utilties-1.0/setup.cfg
--rw-r--r--   0 andrewzhuang   (501) staff       (20)      997 2023-08-07 13:40:52.000000 openai-utilties-1.0/setup.py
+drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-07 13:53:16.252116 openai-utilties-1.1/
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)     2727 2023-08-07 13:53:16.251978 openai-utilties-1.1/PKG-INFO
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)     2210 2023-08-07 13:39:15.000000 openai-utilties-1.1/README.md
+drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-07 13:53:16.250942 openai-utilties-1.1/openai_utils/
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)      669 2023-08-07 13:49:23.000000 openai-utilties-1.1/openai_utils/__init__.py
+drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-07 13:53:16.251763 openai-utilties-1.1/openai_utilties.egg-info/
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)     2727 2023-08-07 13:53:16.000000 openai-utilties-1.1/openai_utilties.egg-info/PKG-INFO
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)      237 2023-08-07 13:53:16.000000 openai-utilties-1.1/openai_utilties.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)        1 2023-08-07 13:53:16.000000 openai-utilties-1.1/openai_utilties.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)       13 2023-08-07 13:53:16.000000 openai-utilties-1.1/openai_utilties.egg-info/requires.txt
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)       13 2023-08-07 13:53:16.000000 openai-utilties-1.1/openai_utilties.egg-info/top_level.txt
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)       38 2023-08-07 13:53:16.252174 openai-utilties-1.1/setup.cfg
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)      997 2023-08-07 13:52:41.000000 openai-utilties-1.1/setup.py
```

### Comparing `openai-utilties-1.0/PKG-INFO` & `openai-utilties-1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-utilties
-Version: 1.0
+Version: 1.1
 Summary: Some external utilities to facilitate OpenAI's Utilites
 Author: YourAverageDev
 License: MIT
 Keywords: openai,utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `openai-utilties-1.0/README.md` & `openai-utilties-1.1/README.md`

 * *Files identical despite different names*

### Comparing `openai-utilties-1.0/openai-utils/__init__.py` & `openai-utilties-1.1/openai_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-utilties-1.0/openai_utilties.egg-info/PKG-INFO` & `openai-utilties-1.1/openai_utilties.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-utilties
-Version: 1.0
+Version: 1.1
 Summary: Some external utilities to facilitate OpenAI's Utilites
 Author: YourAverageDev
 License: MIT
 Keywords: openai,utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `openai-utilties-1.0/setup.py` & `openai-utilties-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 import os
 
-VERSION = '1.0'
+VERSION = '1.1'
 
 DESCRIPTION = "Some external utilities to facilitate OpenAI's Utilites"
 
 with open("README.md", 'r') as r:
 
     long_description = r.read()
```

