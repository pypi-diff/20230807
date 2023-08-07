# Comparing `tmp/sppam-0.0.8.tar.gz` & `tmp/sppam-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sppam-0.0.8.tar", last modified: Wed Aug  2 02:35:53 2023, max compression
+gzip compressed data, was "sppam-0.0.9.tar", last modified: Wed Aug  2 02:45:14 2023, max compression
```

## Comparing `sppam-0.0.8.tar` & `sppam-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:35:53.067112 sppam-0.0.8/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-07-30 01:58:42.000000 sppam-0.0.8/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-30 01:58:42.000000 sppam-0.0.8/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2904 2023-08-02 02:35:53.067112 sppam-0.0.8/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2071 2023-08-01 23:51:40.000000 sppam-0.0.8/README.rst
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      142 2023-08-01 20:18:30.000000 sppam-0.0.8/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-02 02:35:53.071112 sppam-0.0.8/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2617 2023-08-01 23:57:37.000000 sppam-0.0.8/setup.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:35:53.059112 sppam-0.0.8/sppam/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      145 2023-08-01 18:31:29.000000 sppam-0.0.8/sppam/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-02 02:34:13.000000 sppam-0.0.8/sppam/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8291 2023-08-02 02:34:31.000000 sppam-0.0.8/sppam/sppam.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:35:53.067112 sppam-0.0.8/sppam/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-30 01:58:42.000000 sppam-0.0.8/sppam/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      239 2023-08-01 18:32:49.000000 sppam-0.0.8/sppam/tests/test_common.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      389 2023-08-01 20:08:16.000000 sppam-0.0.8/sppam/tests/test_template.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:35:53.063112 sppam-0.0.8/sppam.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2904 2023-08-02 02:35:53.000000 sppam-0.0.8/sppam.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      369 2023-08-02 02:35:53.000000 sppam-0.0.8/sppam.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-02 02:35:53.000000 sppam-0.0.8/sppam.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-01 22:53:39.000000 sppam-0.0.8/sppam.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-02 02:35:53.000000 sppam-0.0.8/sppam.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        6 2023-08-02 02:35:53.000000 sppam-0.0.8/sppam.egg-info/top_level.txt
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:45:14.484481 sppam-0.0.9/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-07-30 01:58:42.000000 sppam-0.0.9/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-30 01:58:42.000000 sppam-0.0.9/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2904 2023-08-02 02:45:14.484481 sppam-0.0.9/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2071 2023-08-01 23:51:40.000000 sppam-0.0.9/README.rst
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      142 2023-08-01 20:18:30.000000 sppam-0.0.9/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-02 02:45:14.484481 sppam-0.0.9/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2617 2023-08-01 23:57:37.000000 sppam-0.0.9/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:45:14.480481 sppam-0.0.9/sppam/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      145 2023-08-01 18:31:29.000000 sppam-0.0.9/sppam/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-02 02:42:13.000000 sppam-0.0.9/sppam/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     8291 2023-08-02 02:34:31.000000 sppam-0.0.9/sppam/sppam.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:45:14.484481 sppam-0.0.9/sppam/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-30 01:58:42.000000 sppam-0.0.9/sppam/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      239 2023-08-01 18:32:49.000000 sppam-0.0.9/sppam/tests/test_common.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      389 2023-08-01 20:08:16.000000 sppam-0.0.9/sppam/tests/test_template.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:45:14.484481 sppam-0.0.9/sppam.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2904 2023-08-02 02:45:14.000000 sppam-0.0.9/sppam.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      369 2023-08-02 02:45:14.000000 sppam-0.0.9/sppam.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-02 02:45:14.000000 sppam-0.0.9/sppam.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-01 22:53:39.000000 sppam-0.0.9/sppam.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-02 02:45:14.000000 sppam-0.0.9/sppam.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        6 2023-08-02 02:45:14.000000 sppam-0.0.9/sppam.egg-info/top_level.txt
```

### Comparing `sppam-0.0.8/LICENSE` & `sppam-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sppam-0.0.8/PKG-INFO` & `sppam-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sppam
-Version: 0.0.8
+Version: 0.0.9
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/sppam
 Download-URL: https://github.com/hrolfrc/sppam
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sppam-0.0.8/README.rst` & `sppam-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `sppam-0.0.8/setup.py` & `sppam-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sppam-0.0.8/sppam/sppam.py` & `sppam-0.0.9/sppam/sppam.py`

 * *Files identical despite different names*

### Comparing `sppam-0.0.8/sppam.egg-info/PKG-INFO` & `sppam-0.0.9/sppam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sppam
-Version: 0.0.8
+Version: 0.0.9
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/sppam
 Download-URL: https://github.com/hrolfrc/sppam
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

