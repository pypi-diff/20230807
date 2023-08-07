# Comparing `tmp/calfcv-0.1.1.tar.gz` & `tmp/calfcv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfcv-0.1.1.tar", last modified: Mon Aug  7 01:54:33 2023, max compression
+gzip compressed data, was "calfcv-0.1.3.tar", last modified: Mon Aug  7 03:08:46 2023, max compression
```

## Comparing `calfcv-0.1.1.tar` & `calfcv-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 01:54:33.965838 calfcv-0.1.1/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-08-05 15:55:07.000000 calfcv-0.1.1/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-08-05 15:55:07.000000 calfcv-0.1.1/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3139 2023-08-07 01:54:33.965838 calfcv-0.1.1/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2387 2023-08-06 22:40:20.000000 calfcv-0.1.1/README.rst
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 01:54:33.961838 calfcv-0.1.1/calfcv/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      124 2023-08-05 16:36:58.000000 calfcv-0.1.1/calfcv/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-07 01:48:49.000000 calfcv-0.1.1/calfcv/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)    14036 2023-08-07 01:20:37.000000 calfcv-0.1.1/calfcv/calfcv.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 01:54:33.965838 calfcv-0.1.1/calfcv/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-08-05 15:55:07.000000 calfcv-0.1.1/calfcv/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.1.1/calfcv/tests/test_calfcv.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-08-05 16:13:09.000000 calfcv-0.1.1/calfcv/tests/test_common.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 01:54:33.965838 calfcv-0.1.1/calfcv.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3139 2023-08-07 01:54:33.000000 calfcv-0.1.1/calfcv.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-08-07 01:54:33.000000 calfcv-0.1.1/calfcv.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-07 01:54:33.000000 calfcv-0.1.1/calfcv.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-06 22:43:48.000000 calfcv-0.1.1/calfcv.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-07 01:54:33.000000 calfcv-0.1.1/calfcv.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-08-07 01:54:33.000000 calfcv-0.1.1/calfcv.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      134 2023-08-05 16:12:02.000000 calfcv-0.1.1/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-07 01:54:33.965838 calfcv-0.1.1/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2533 2023-08-05 16:22:01.000000 calfcv-0.1.1/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 03:08:46.467417 calfcv-0.1.3/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-08-05 15:55:07.000000 calfcv-0.1.3/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-08-05 15:55:07.000000 calfcv-0.1.3/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     3323 2023-08-07 03:08:46.467417 calfcv-0.1.3/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2571 2023-08-07 03:02:16.000000 calfcv-0.1.3/README.rst
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 03:08:46.463417 calfcv-0.1.3/calfcv/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      124 2023-08-05 16:36:58.000000 calfcv-0.1.3/calfcv/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-07 03:03:18.000000 calfcv-0.1.3/calfcv/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)    14036 2023-08-07 01:20:37.000000 calfcv-0.1.3/calfcv/calfcv.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 03:08:46.463417 calfcv-0.1.3/calfcv/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-08-05 15:55:07.000000 calfcv-0.1.3/calfcv/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.1.3/calfcv/tests/test_calfcv.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-08-05 16:13:09.000000 calfcv-0.1.3/calfcv/tests/test_common.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 03:08:46.463417 calfcv-0.1.3/calfcv.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     3323 2023-08-07 03:08:46.000000 calfcv-0.1.3/calfcv.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-08-07 03:08:46.000000 calfcv-0.1.3/calfcv.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-07 03:08:46.000000 calfcv-0.1.3/calfcv.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-06 22:43:48.000000 calfcv-0.1.3/calfcv.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-07 03:08:46.000000 calfcv-0.1.3/calfcv.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-08-07 03:08:46.000000 calfcv-0.1.3/calfcv.egg-info/top_level.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      134 2023-08-05 16:12:02.000000 calfcv-0.1.3/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-07 03:08:46.467417 calfcv-0.1.3/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2533 2023-08-05 16:22:01.000000 calfcv-0.1.3/setup.py
```

### Comparing `calfcv-0.1.1/LICENSE` & `calfcv-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calfcv-0.1.1/PKG-INFO` & `calfcv-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfcv
-Version: 0.1.1
+Version: 0.1.3
 Summary: Coarse approximation linear function with cross validation
 Home-page: https://github.com/hrolfrc/calfcv
 Download-URL: https://github.com/hrolfrc/calfcv
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -17,19 +17,23 @@
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
-|ReadTheDocs|_
+|CircleCI|_ |ReadTheDocs|_
+
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calfcv.svg?style=shield&circle-token=:circle-token
+.. _CircleCI: https://circleci.com/gh/hrolfrc/calfcv/tree/master
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calfcv/badge/?version=latest
 .. _ReadTheDocs: https://calfcv.readthedocs.io/en/latest/?badge=latest
 
+
 CalfCV
 #####################################
 
 A binomial classifier that implements the Coarse Approximation Linear Function (CALF).
 
 Contact
 ------------------
```

### Comparing `calfcv-0.1.1/README.rst` & `calfcv-0.1.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 .. -*- mode: rst -*-
 
-|ReadTheDocs|_
+|CircleCI|_ |ReadTheDocs|_
+
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calfcv.svg?style=shield&circle-token=:circle-token
+.. _CircleCI: https://circleci.com/gh/hrolfrc/calfcv/tree/master
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calfcv/badge/?version=latest
 .. _ReadTheDocs: https://calfcv.readthedocs.io/en/latest/?badge=latest
 
+
 CalfCV
 #####################################
 
 A binomial classifier that implements the Coarse Approximation Linear Function (CALF).
 
 Contact
 ------------------
```

### Comparing `calfcv-0.1.1/calfcv/calfcv.py` & `calfcv-0.1.3/calfcv/calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.1.1/calfcv/tests/test_calfcv.py` & `calfcv-0.1.3/calfcv/tests/test_calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.1.1/calfcv.egg-info/PKG-INFO` & `calfcv-0.1.3/calfcv.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfcv
-Version: 0.1.1
+Version: 0.1.3
 Summary: Coarse approximation linear function with cross validation
 Home-page: https://github.com/hrolfrc/calfcv
 Download-URL: https://github.com/hrolfrc/calfcv
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -17,19 +17,23 @@
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
-|ReadTheDocs|_
+|CircleCI|_ |ReadTheDocs|_
+
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calfcv.svg?style=shield&circle-token=:circle-token
+.. _CircleCI: https://circleci.com/gh/hrolfrc/calfcv/tree/master
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calfcv/badge/?version=latest
 .. _ReadTheDocs: https://calfcv.readthedocs.io/en/latest/?badge=latest
 
+
 CalfCV
 #####################################
 
 A binomial classifier that implements the Coarse Approximation Linear Function (CALF).
 
 Contact
 ------------------
```

### Comparing `calfcv-0.1.1/setup.py` & `calfcv-0.1.3/setup.py`

 * *Files identical despite different names*

