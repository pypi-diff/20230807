# Comparing `tmp/cmn-1.1.0.tar.gz` & `tmp/cmn-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmn-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cmn-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cmn-1.1.0.tar` & `cmn-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1005 2023-07-31 22:03:09.378237 cmn-1.1.0/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1127 2023-08-07 18:53:04.536799 cmn-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       88 2023-08-07 19:14:41.930601 cmn-1.1.0/.gitignore
--rw-r--r--   0        0        0     9229 2023-08-06 00:34:24.799239 cmn-1.1.0/LICENSE
--rw-r--r--   0        0        0     2649 2023-08-03 22:44:06.242819 cmn-1.1.0/README.md
--rw-r--r--   0        0        0      502 2023-08-06 01:32:58.152292 cmn-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       15 2023-08-03 22:48:42.765195 cmn-1.1.0/requirements.txt
--rw-r--r--   0        0        0     4726 2023-08-07 19:02:33.161717 cmn-1.1.0/src/ChangeMediaName/ChangeMediaName.py
--rw-r--r--   0        0        0     1104 2023-08-06 01:09:25.634489 cmn-1.1.0/src/ColoredLogger/ColoredLogger.py
--rw-r--r--   0        0        0     2860 2023-08-06 01:09:25.666374 cmn-1.1.0/src/OutputFormatter/OutputFormatter.py
--rw-r--r--   0        0        0     2301 2023-08-07 19:01:17.007069 cmn-1.1.0/src/OutputFormatter/test_OutputFormatter.py
--rw-r--r--   0        0        0     6480 2023-08-07 19:13:10.500439 cmn-1.1.0/src/cmn/__init__.py
--rw-r--r--   0        0        0     7046 2023-08-07 19:12:00.845729 cmn-1.1.0/src/test_main.py
--rw-r--r--   0        0        0     3048 1970-01-01 00:00:00.000000 cmn-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1005 2023-07-31 22:03:09.378237 cmn-1.1.1/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1127 2023-08-07 18:53:04.536799 cmn-1.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       88 2023-08-07 19:14:41.930601 cmn-1.1.1/.gitignore
+-rw-r--r--   0        0        0     9229 2023-08-06 00:34:24.799239 cmn-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2649 2023-08-03 22:44:06.242819 cmn-1.1.1/README.md
+-rw-r--r--   0        0        0      502 2023-08-06 01:32:58.152292 cmn-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       15 2023-08-03 22:48:42.765195 cmn-1.1.1/requirements.txt
+-rw-r--r--   0        0        0     4726 2023-08-07 19:02:33.161717 cmn-1.1.1/src/ChangeMediaName/ChangeMediaName.py
+-rw-r--r--   0        0        0     1104 2023-08-06 01:09:25.634489 cmn-1.1.1/src/ColoredLogger/ColoredLogger.py
+-rw-r--r--   0        0        0     2860 2023-08-06 01:09:25.666374 cmn-1.1.1/src/OutputFormatter/OutputFormatter.py
+-rw-r--r--   0        0        0     2301 2023-08-07 19:01:17.007069 cmn-1.1.1/src/OutputFormatter/test_OutputFormatter.py
+-rw-r--r--   0        0        0     6480 2023-08-07 19:22:40.414045 cmn-1.1.1/src/cmn/__init__.py
+-rw-r--r--   0        0        0       68 2023-08-07 19:21:31.582055 cmn-1.1.1/src/cmn/__main__.py
+-rw-r--r--   0        0        0     7046 2023-08-07 19:12:00.845729 cmn-1.1.1/src/test_main.py
+-rw-r--r--   0        0        0     3048 1970-01-01 00:00:00.000000 cmn-1.1.1/PKG-INFO
```

### Comparing `cmn-1.1.0/.github/workflows/python-app.yml` & `cmn-1.1.1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `cmn-1.1.0/.github/workflows/python-publish.yml` & `cmn-1.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cmn-1.1.0/LICENSE` & `cmn-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmn-1.1.0/README.md` & `cmn-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cmn-1.1.0/src/ChangeMediaName/ChangeMediaName.py` & `cmn-1.1.1/src/ChangeMediaName/ChangeMediaName.py`

 * *Files identical despite different names*

### Comparing `cmn-1.1.0/src/ColoredLogger/ColoredLogger.py` & `cmn-1.1.1/src/ColoredLogger/ColoredLogger.py`

 * *Files identical despite different names*

### Comparing `cmn-1.1.0/src/OutputFormatter/OutputFormatter.py` & `cmn-1.1.1/src/OutputFormatter/OutputFormatter.py`

 * *Files identical despite different names*

### Comparing `cmn-1.1.0/src/OutputFormatter/test_OutputFormatter.py` & `cmn-1.1.1/src/OutputFormatter/test_OutputFormatter.py`

 * *Files identical despite different names*

### Comparing `cmn-1.1.0/src/cmn/__init__.py` & `cmn-1.1.1/src/cmn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Main - Module responsible for the main program. Parses the arguments and calls the other modules.
 """
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 import argparse
 import os
 import re
 
 from src.ColoredLogger.ColoredLogger import ColoredLogger
```

### Comparing `cmn-1.1.0/src/test_main.py` & `cmn-1.1.1/src/test_main.py`

 * *Files identical despite different names*

### Comparing `cmn-1.1.0/PKG-INFO` & `cmn-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmn
-Version: 1.1.0
+Version: 1.1.1
 Summary: Main - Module responsible for the main program. Parses the arguments and calls the other modules.
 Author-email: Henrique Alvelos <henriquealvelos@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: colorama >= 0.4.6
 Project-URL: Home, https://github.com/Henrique-190/ChangeMediaName
```

