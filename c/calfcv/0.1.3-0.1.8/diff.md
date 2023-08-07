# Comparing `tmp/calfcv-0.1.3.tar.gz` & `tmp/calfcv-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfcv-0.1.3.tar", last modified: Mon Aug  7 03:08:46 2023, max compression
+gzip compressed data, was "calfcv-0.1.8.tar", last modified: Mon Aug  7 04:01:30 2023, max compression
```

## Comparing `calfcv-0.1.3.tar` & `calfcv-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 03:08:46.467417 calfcv-0.1.3/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-08-05 15:55:07.000000 calfcv-0.1.3/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-08-05 15:55:07.000000 calfcv-0.1.3/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3323 2023-08-07 03:08:46.467417 calfcv-0.1.3/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2571 2023-08-07 03:02:16.000000 calfcv-0.1.3/README.rst
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 03:08:46.463417 calfcv-0.1.3/calfcv/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      124 2023-08-05 16:36:58.000000 calfcv-0.1.3/calfcv/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-07 03:03:18.000000 calfcv-0.1.3/calfcv/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)    14036 2023-08-07 01:20:37.000000 calfcv-0.1.3/calfcv/calfcv.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 03:08:46.463417 calfcv-0.1.3/calfcv/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-08-05 15:55:07.000000 calfcv-0.1.3/calfcv/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.1.3/calfcv/tests/test_calfcv.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-08-05 16:13:09.000000 calfcv-0.1.3/calfcv/tests/test_common.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 03:08:46.463417 calfcv-0.1.3/calfcv.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3323 2023-08-07 03:08:46.000000 calfcv-0.1.3/calfcv.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-08-07 03:08:46.000000 calfcv-0.1.3/calfcv.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-07 03:08:46.000000 calfcv-0.1.3/calfcv.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-06 22:43:48.000000 calfcv-0.1.3/calfcv.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-07 03:08:46.000000 calfcv-0.1.3/calfcv.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-08-07 03:08:46.000000 calfcv-0.1.3/calfcv.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      134 2023-08-05 16:12:02.000000 calfcv-0.1.3/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-07 03:08:46.467417 calfcv-0.1.3/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2533 2023-08-05 16:22:01.000000 calfcv-0.1.3/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 04:01:30.339361 calfcv-0.1.8/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-08-05 15:55:07.000000 calfcv-0.1.8/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-08-05 15:55:07.000000 calfcv-0.1.8/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     3284 2023-08-07 04:01:30.339361 calfcv-0.1.8/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2532 2023-08-07 03:29:58.000000 calfcv-0.1.8/README.rst
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 04:01:30.339361 calfcv-0.1.8/calfcv/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      124 2023-08-05 16:36:58.000000 calfcv-0.1.8/calfcv/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-07 03:58:38.000000 calfcv-0.1.8/calfcv/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)    14036 2023-08-07 01:20:37.000000 calfcv-0.1.8/calfcv/calfcv.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 04:01:30.339361 calfcv-0.1.8/calfcv/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-08-05 15:55:07.000000 calfcv-0.1.8/calfcv/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.1.8/calfcv/tests/test_calfcv.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-08-05 16:13:09.000000 calfcv-0.1.8/calfcv/tests/test_common.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-07 04:01:30.339361 calfcv-0.1.8/calfcv.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     3284 2023-08-07 04:01:30.000000 calfcv-0.1.8/calfcv.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-08-07 04:01:30.000000 calfcv-0.1.8/calfcv.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-07 04:01:30.000000 calfcv-0.1.8/calfcv.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-06 22:43:48.000000 calfcv-0.1.8/calfcv.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-07 04:01:30.000000 calfcv-0.1.8/calfcv.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-08-07 04:01:30.000000 calfcv-0.1.8/calfcv.egg-info/top_level.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      134 2023-08-05 16:12:02.000000 calfcv-0.1.8/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-07 04:01:30.339361 calfcv-0.1.8/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2533 2023-08-05 16:22:01.000000 calfcv-0.1.8/setup.py
```

### Comparing `calfcv-0.1.3/LICENSE` & `calfcv-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `calfcv-0.1.3/PKG-INFO` & `calfcv-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfcv
-Version: 0.1.3
+Version: 0.1.8
 Summary: Coarse approximation linear function with cross validation
 Home-page: https://github.com/hrolfrc/calfcv
 Download-URL: https://github.com/hrolfrc/calfcv
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -19,16 +19,16 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
 |CircleCI|_ |ReadTheDocs|_
 
-.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calfcv.svg?style=shield&circle-token=:circle-token
-.. _CircleCI: https://circleci.com/gh/hrolfrc/calfcv/tree/master
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calfcv.svg?style=shield
+.. _CircleCI: https://circleci.com/gh/hrolfrc/calfcv
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calfcv/badge/?version=latest
 .. _ReadTheDocs: https://calfcv.readthedocs.io/en/latest/?badge=latest
 
 
 CalfCV
 #####################################
```

### Comparing `calfcv-0.1.3/README.rst` & `calfcv-0.1.8/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. -*- mode: rst -*-
 
 |CircleCI|_ |ReadTheDocs|_
 
-.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calfcv.svg?style=shield&circle-token=:circle-token
-.. _CircleCI: https://circleci.com/gh/hrolfrc/calfcv/tree/master
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calfcv.svg?style=shield
+.. _CircleCI: https://circleci.com/gh/hrolfrc/calfcv
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calfcv/badge/?version=latest
 .. _ReadTheDocs: https://calfcv.readthedocs.io/en/latest/?badge=latest
 
 
 CalfCV
 #####################################
```

### Comparing `calfcv-0.1.3/calfcv/calfcv.py` & `calfcv-0.1.8/calfcv/calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.1.3/calfcv/tests/test_calfcv.py` & `calfcv-0.1.8/calfcv/tests/test_calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.1.3/calfcv.egg-info/PKG-INFO` & `calfcv-0.1.8/calfcv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfcv
-Version: 0.1.3
+Version: 0.1.8
 Summary: Coarse approximation linear function with cross validation
 Home-page: https://github.com/hrolfrc/calfcv
 Download-URL: https://github.com/hrolfrc/calfcv
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -19,16 +19,16 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
 |CircleCI|_ |ReadTheDocs|_
 
-.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calfcv.svg?style=shield&circle-token=:circle-token
-.. _CircleCI: https://circleci.com/gh/hrolfrc/calfcv/tree/master
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calfcv.svg?style=shield
+.. _CircleCI: https://circleci.com/gh/hrolfrc/calfcv
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calfcv/badge/?version=latest
 .. _ReadTheDocs: https://calfcv.readthedocs.io/en/latest/?badge=latest
 
 
 CalfCV
 #####################################
```

### Comparing `calfcv-0.1.3/setup.py` & `calfcv-0.1.8/setup.py`

 * *Files identical despite different names*

