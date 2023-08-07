# Comparing `tmp/OCRTest-0.0.2.tar.gz` & `tmp/OCRTest-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OCRTest-0.0.2.tar", last modified: Mon Aug  7 04:25:42 2023, max compression
+gzip compressed data, was "OCRTest-0.0.3.tar", last modified: Mon Aug  7 04:29:17 2023, max compression
```

## Comparing `OCRTest-0.0.2.tar` & `OCRTest-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 twel      (1000) twel      (1000)        0 2023-08-07 04:25:42.052227 OCRTest-0.0.2/
--rw-r--r--   0 twel      (1000) twel      (1000)     1068 2023-08-07 04:11:03.000000 OCRTest-0.0.2/LICENSE
-drwxr-xr-x   0 twel      (1000) twel      (1000)        0 2023-08-07 04:25:42.052227 OCRTest-0.0.2/OCRTest.egg-info/
--rw-r--r--   0 twel      (1000) twel      (1000)      464 2023-08-07 04:25:42.000000 OCRTest-0.0.2/OCRTest.egg-info/PKG-INFO
--rw-r--r--   0 twel      (1000) twel      (1000)      187 2023-08-07 04:25:42.000000 OCRTest-0.0.2/OCRTest.egg-info/SOURCES.txt
--rw-r--r--   0 twel      (1000) twel      (1000)        1 2023-08-07 04:25:42.000000 OCRTest-0.0.2/OCRTest.egg-info/dependency_links.txt
--rw-r--r--   0 twel      (1000) twel      (1000)        8 2023-08-07 04:25:42.000000 OCRTest-0.0.2/OCRTest.egg-info/top_level.txt
--rw-r--r--   0 twel      (1000) twel      (1000)      464 2023-08-07 04:25:42.052227 OCRTest-0.0.2/PKG-INFO
--rw-r--r--   0 twel      (1000) twel      (1000)      112 2023-08-07 04:10:06.000000 OCRTest-0.0.2/README.md
-drwxr-xr-x   0 twel      (1000) twel      (1000)        0 2023-08-07 04:25:42.052227 OCRTest-0.0.2/ocrtest/
--rw-r--r--   0 twel      (1000) twel      (1000)        0 2023-08-07 04:21:40.000000 OCRTest-0.0.2/ocrtest/__init__.py
--rw-r--r--   0 twel      (1000) twel      (1000)      131 2023-08-07 04:22:06.000000 OCRTest-0.0.2/ocrtest/hello.py
--rw-r--r--   0 twel      (1000) twel      (1000)       38 2023-08-07 04:25:42.052227 OCRTest-0.0.2/setup.cfg
--rw-r--r--   0 twel      (1000) twel      (1000)      837 2023-08-07 04:25:39.000000 OCRTest-0.0.2/setup.py
+drwxr-xr-x   0 twel      (1000) twel      (1000)        0 2023-08-07 04:29:17.492227 OCRTest-0.0.3/
+-rw-r--r--   0 twel      (1000) twel      (1000)     1068 2023-08-07 04:11:03.000000 OCRTest-0.0.3/LICENSE
+drwxr-xr-x   0 twel      (1000) twel      (1000)        0 2023-08-07 04:29:17.492227 OCRTest-0.0.3/OCRTest.egg-info/
+-rw-r--r--   0 twel      (1000) twel      (1000)      464 2023-08-07 04:29:17.000000 OCRTest-0.0.3/OCRTest.egg-info/PKG-INFO
+-rw-r--r--   0 twel      (1000) twel      (1000)      187 2023-08-07 04:29:17.000000 OCRTest-0.0.3/OCRTest.egg-info/SOURCES.txt
+-rw-r--r--   0 twel      (1000) twel      (1000)        1 2023-08-07 04:29:17.000000 OCRTest-0.0.3/OCRTest.egg-info/dependency_links.txt
+-rw-r--r--   0 twel      (1000) twel      (1000)        8 2023-08-07 04:29:17.000000 OCRTest-0.0.3/OCRTest.egg-info/top_level.txt
+-rw-r--r--   0 twel      (1000) twel      (1000)      464 2023-08-07 04:29:17.492227 OCRTest-0.0.3/PKG-INFO
+-rw-r--r--   0 twel      (1000) twel      (1000)      112 2023-08-07 04:10:06.000000 OCRTest-0.0.3/README.md
+drwxr-xr-x   0 twel      (1000) twel      (1000)        0 2023-08-07 04:29:17.492227 OCRTest-0.0.3/ocrtest/
+-rw-r--r--   0 twel      (1000) twel      (1000)        0 2023-08-07 04:21:40.000000 OCRTest-0.0.3/ocrtest/__init__.py
+-rw-r--r--   0 twel      (1000) twel      (1000)      135 2023-08-07 04:28:55.000000 OCRTest-0.0.3/ocrtest/hello.py
+-rw-r--r--   0 twel      (1000) twel      (1000)       38 2023-08-07 04:29:17.492227 OCRTest-0.0.3/setup.cfg
+-rw-r--r--   0 twel      (1000) twel      (1000)      837 2023-08-07 04:29:11.000000 OCRTest-0.0.3/setup.py
```

### Comparing `OCRTest-0.0.2/LICENSE` & `OCRTest-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `OCRTest-0.0.2/setup.py` & `OCRTest-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'An OCR hello package'
 
 # Setting up
 setup(
     name="OCRTest",
     version=VERSION,
     author="OCR Research Lab",
```

