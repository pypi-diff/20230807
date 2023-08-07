# Comparing `tmp/OCRTest_2-0.0.1.tar.gz` & `tmp/OCRTest_2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OCRTest_2-0.0.1.tar", last modified: Mon Aug  7 07:38:24 2023, max compression
+gzip compressed data, was "OCRTest_2-0.0.2.tar", last modified: Mon Aug  7 08:41:21 2023, max compression
```

## Comparing `OCRTest_2-0.0.1.tar` & `OCRTest_2-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 twel      (1000) twel      (1000)        0 2023-08-07 07:38:24.962227 OCRTest_2-0.0.1/
--rw-r--r--   0 twel      (1000) twel      (1000)     1068 2023-08-07 04:11:03.000000 OCRTest_2-0.0.1/LICENSE
-drwxr-xr-x   0 twel      (1000) twel      (1000)        0 2023-08-07 07:38:24.962227 OCRTest_2-0.0.1/OCRTest_2.egg-info/
--rw-r--r--   0 twel      (1000) twel      (1000)      400 2023-08-07 07:38:24.000000 OCRTest_2-0.0.1/OCRTest_2.egg-info/PKG-INFO
--rw-r--r--   0 twel      (1000) twel      (1000)      195 2023-08-07 07:38:24.000000 OCRTest_2-0.0.1/OCRTest_2.egg-info/SOURCES.txt
--rw-r--r--   0 twel      (1000) twel      (1000)        1 2023-08-07 07:38:24.000000 OCRTest_2-0.0.1/OCRTest_2.egg-info/dependency_links.txt
--rw-r--r--   0 twel      (1000) twel      (1000)        8 2023-08-07 07:38:24.000000 OCRTest_2-0.0.1/OCRTest_2.egg-info/top_level.txt
--rw-r--r--   0 twel      (1000) twel      (1000)      400 2023-08-07 07:38:24.962227 OCRTest_2-0.0.1/PKG-INFO
--rw-r--r--   0 twel      (1000) twel      (1000)      112 2023-08-07 04:10:06.000000 OCRTest_2-0.0.1/README.md
-drwxr-xr-x   0 twel      (1000) twel      (1000)        0 2023-08-07 07:38:24.962227 OCRTest_2-0.0.1/ocrtest/
--rw-r--r--   0 twel      (1000) twel      (1000)       37 2023-08-07 04:48:06.000000 OCRTest_2-0.0.1/ocrtest/__init__.py
--rw-r--r--   0 twel      (1000) twel      (1000)      141 2023-08-07 04:32:12.000000 OCRTest_2-0.0.1/ocrtest/hello.py
--rw-r--r--   0 twel      (1000) twel      (1000)       38 2023-08-07 07:38:24.962227 OCRTest_2-0.0.1/setup.cfg
--rw-r--r--   0 twel      (1000) twel      (1000)      843 2023-08-07 07:38:12.000000 OCRTest_2-0.0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-07 08:41:21.622460 OCRTest_2-0.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-08-07 08:41:03.000000 OCRTest_2-0.0.2/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-07 08:41:21.618461 OCRTest_2-0.0.2/OCRTest_2.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-08-07 08:41:21.000000 OCRTest_2-0.0.2/OCRTest_2.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-08-07 08:41:21.000000 OCRTest_2-0.0.2/OCRTest_2.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-08-07 08:41:21.000000 OCRTest_2-0.0.2/OCRTest_2.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-08-07 08:41:21.000000 OCRTest_2-0.0.2/OCRTest_2.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-08-07 08:41:21.622460 OCRTest_2-0.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-08-07 08:41:03.000000 OCRTest_2-0.0.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-07 08:41:21.618461 OCRTest_2-0.0.2/ocrtest/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-08-07 08:41:03.000000 OCRTest_2-0.0.2/ocrtest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-08-07 08:41:03.000000 OCRTest_2-0.0.2/ocrtest/hello.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-07 08:41:21.622460 OCRTest_2-0.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-08-07 08:41:03.000000 OCRTest_2-0.0.2/setup.py
```

### Comparing `OCRTest_2-0.0.1/LICENSE` & `OCRTest_2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OCRTest_2-0.0.1/setup.py` & `OCRTest_2-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'An OCR hello package'
 
 # Setting up
 setup(
     name="OCRTest_2",
     version=VERSION,
-    # author="OCR Research Lab",
-    # author_email="<vuquocminhdang@gmail.com>",
+    author="OCR Research Lab",
+    author_email="<ai.r3search.lab@gmail.com>",
     description=DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
```

