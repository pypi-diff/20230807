# Comparing `tmp/MGSurvE-1.0.8.tar.gz` & `tmp/MGSurvE-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGSurvE-1.0.8.tar", last modified: Fri Jul 14 19:45:38 2023, max compression
+gzip compressed data, was "MGSurvE-1.0.9.tar", last modified: Mon Aug  7 19:43:31 2023, max compression
```

## Comparing `MGSurvE-1.0.8.tar` & `MGSurvE-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 19:45:38.332280 MGSurvE-1.0.8/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/LICENSE
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 19:45:38.331108 MGSurvE-1.0.8/MGSurvE/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/MGSurvE/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/MGSurvE/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-1.0.8/MGSurvE/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-06-29 19:56:26.000000 MGSurvE-1.0.8/MGSurvE/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-1.0.8/MGSurvE/kernels.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21887 2023-07-14 17:12:03.000000 MGSurvE-1.0.8/MGSurvE/landscape.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/MGSurvE/matrices.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/MGSurvE/network.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    48723 2023-07-14 18:52:09.000000 MGSurvE-1.0.8/MGSurvE/optimization.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-06-26 18:35:57.000000 MGSurvE-1.0.8/MGSurvE/optimizationPSO.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18819 2023-07-14 17:50:13.000000 MGSurvE-1.0.8/MGSurvE/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/MGSurvE/pointProcess.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 19:45:38.331930 MGSurvE-1.0.8/MGSurvE.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      231 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-14 19:45:38.332131 MGSurvE-1.0.8/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4172 2023-06-29 18:04:52.000000 MGSurvE-1.0.8/README.md
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-07-14 19:45:38.332340 MGSurvE-1.0.8/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1441 2023-06-28 20:50:45.000000 MGSurvE-1.0.8/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-08-07 19:43:31.140963 MGSurvE-1.0.9/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-1.0.9/LICENSE
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-08-07 19:43:31.139817 MGSurvE-1.0.9/MGSurvE/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-1.0.9/MGSurvE/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-08-07 19:43:30.000000 MGSurvE-1.0.9/MGSurvE/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-1.0.9/MGSurvE/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-1.0.9/MGSurvE/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-06-29 19:56:26.000000 MGSurvE-1.0.9/MGSurvE/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-1.0.9/MGSurvE/kernels.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21887 2023-08-03 18:51:46.000000 MGSurvE-1.0.9/MGSurvE/landscape.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-1.0.9/MGSurvE/matrices.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-1.0.9/MGSurvE/network.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    48723 2023-07-14 18:52:09.000000 MGSurvE-1.0.9/MGSurvE/optimization.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-06-26 18:35:57.000000 MGSurvE-1.0.9/MGSurvE/optimizationPSO.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18819 2023-07-14 17:50:13.000000 MGSurvE-1.0.9/MGSurvE/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-1.0.9/MGSurvE/pointProcess.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-08-07 19:43:31.140591 MGSurvE-1.0.9/MGSurvE.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-08-07 19:43:31.000000 MGSurvE-1.0.9/MGSurvE.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-08-07 19:43:31.000000 MGSurvE-1.0.9/MGSurvE.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-08-07 19:43:31.000000 MGSurvE-1.0.9/MGSurvE.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      231 2023-08-07 19:43:31.000000 MGSurvE-1.0.9/MGSurvE.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-08-07 19:43:31.000000 MGSurvE-1.0.9/MGSurvE.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-08-07 19:43:31.140814 MGSurvE-1.0.9/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4172 2023-06-29 18:04:52.000000 MGSurvE-1.0.9/README.md
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-08-07 19:43:31.141016 MGSurvE-1.0.9/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1441 2023-06-28 20:50:45.000000 MGSurvE-1.0.9/setup.py
```

### Comparing `MGSurvE-1.0.8/LICENSE` & `MGSurvE-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE/auxiliary.py` & `MGSurvE-1.0.9/MGSurvE/auxiliary.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE/colors.py` & `MGSurvE-1.0.9/MGSurvE/colors.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE/constants.py` & `MGSurvE-1.0.9/MGSurvE/constants.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE/kernels.py` & `MGSurvE-1.0.9/MGSurvE/kernels.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE/landscape.py` & `MGSurvE-1.0.9/MGSurvE/landscape.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE/matrices.py` & `MGSurvE-1.0.9/MGSurvE/matrices.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE/network.py` & `MGSurvE-1.0.9/MGSurvE/network.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE/optimization.py` & `MGSurvE-1.0.9/MGSurvE/optimization.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE/optimizationPSO.py` & `MGSurvE-1.0.9/MGSurvE/optimizationPSO.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE/plots.py` & `MGSurvE-1.0.9/MGSurvE/plots.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE/pointProcess.py` & `MGSurvE-1.0.9/MGSurvE/pointProcess.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/MGSurvE.egg-info/PKG-INFO` & `MGSurvE-1.0.9/MGSurvE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 1.0.8
+Version: 1.0.9
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-1.0.8/PKG-INFO` & `MGSurvE-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 1.0.8
+Version: 1.0.9
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-1.0.8/README.md` & `MGSurvE-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.8/setup.py` & `MGSurvE-1.0.9/setup.py`

 * *Files identical despite different names*

