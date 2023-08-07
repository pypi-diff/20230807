# Comparing `tmp/nxtomo-0.2.0.tar.gz` & `tmp/nxtomo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxtomo-0.2.0.tar", last modified: Fri Aug  4 14:17:47 2023, max compression
+gzip compressed data, was "nxtomo-1.0.0.tar", last modified: Mon Aug  7 08:38:36 2023, max compression
```

## Comparing `nxtomo-0.2.0.tar` & `nxtomo-1.0.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/
--rw-r--r--   0 payno     (1000) payno     (1000)     1266 2023-08-04 08:57:20.000000 nxtomo-0.2.0/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     3233 2023-08-04 14:17:47.883110 nxtomo-0.2.0/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      187 2023-08-04 12:40:29.000000 nxtomo-0.2.0/README.md
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.879110 nxtomo-0.2.0/nxtomo/
--rw-r--r--   0 payno     (1000) payno     (1000)      103 2023-08-04 13:11:37.000000 nxtomo-0.2.0/nxtomo/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.879110 nxtomo-0.2.0/nxtomo/application/
--rw-r--r--   0 payno     (1000) payno     (1000)    27475 2023-08-04 13:11:48.000000 nxtomo-0.2.0/nxtomo/application/nxtomo.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.879110 nxtomo-0.2.0/nxtomo/application/test/
--rw-r--r--   0 payno     (1000) payno     (1000)    16816 2023-08-04 13:29:54.000000 nxtomo-0.2.0/nxtomo/application/test/test_nxtomo.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8666 2023-08-04 12:27:55.000000 nxtomo-0.2.0/nxtomo/io.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/nxobject/
--rw-r--r--   0 payno     (1000) payno     (1000)      224 2023-08-04 12:09:44.000000 nxtomo-0.2.0/nxtomo/nxobject/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    37631 2023-08-04 13:17:20.000000 nxtomo-0.2.0/nxtomo/nxobject/nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     7106 2023-08-04 13:13:10.000000 nxtomo-0.2.0/nxtomo/nxobject/nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3391 2023-08-04 12:17:45.000000 nxtomo-0.2.0/nxtomo/nxobject/nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)    12997 2023-08-04 12:37:48.000000 nxtomo-0.2.0/nxtomo/nxobject/nxobject.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9619 2023-08-04 12:15:33.000000 nxtomo-0.2.0/nxtomo/nxobject/nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)     6252 2023-08-04 13:13:19.000000 nxtomo-0.2.0/nxtomo/nxobject/nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)     9446 2023-08-04 13:13:26.000000 nxtomo-0.2.0/nxtomo/nxobject/nxtransformations.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/nxobject/test/
--rw-r--r--   0 payno     (1000) payno     (1000)    14678 2023-08-04 14:15:03.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1333 2023-08-04 13:34:34.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1077 2023-08-04 13:35:22.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2706 2023-08-04 13:15:03.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxobject.py
--rw-r--r--   0 payno     (1000) payno     (1000)     2076 2023-08-04 13:35:34.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1127 2023-08-04 13:35:43.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)     5146 2023-08-04 14:15:06.000000 nxtomo-0.2.0/nxtomo/nxobject/test/test_nxtransformations.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3588 2023-08-04 13:35:20.000000 nxtomo-0.2.0/nxtomo/nxobject/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/paths/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1242 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxdetector.py
--rw-r--r--   0 payno     (1000) payno     (1000)      481 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxinstrument.py
--rw-r--r--   0 payno     (1000) payno     (1000)      319 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxmonitor.py
--rw-r--r--   0 payno     (1000) payno     (1000)      826 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxsample.py
--rw-r--r--   0 payno     (1000) payno     (1000)      343 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxsource.py
--rw-r--r--   0 payno     (1000) payno     (1000)    11877 2023-08-04 13:36:04.000000 nxtomo-0.2.0/nxtomo/paths/nxtomo.py
--rw-r--r--   0 payno     (1000) payno     (1000)      543 2023-08-04 08:15:45.000000 nxtomo-0.2.0/nxtomo/paths/nxtransformations.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/paths/test/
--rw-r--r--   0 payno     (1000) payno     (1000)     6676 2023-08-04 13:33:31.000000 nxtomo-0.2.0/nxtomo/paths/test/test_backward_compatibility.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/utils/
--rw-r--r--   0 payno     (1000) payno     (1000)       34 2023-08-04 12:05:19.000000 nxtomo-0.2.0/nxtomo/utils/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)    15108 2023-08-04 13:35:54.000000 nxtomo-0.2.0/nxtomo/utils/frameappender.py
--rw-r--r--   0 payno     (1000) payno     (1000)     1990 2023-08-04 12:27:23.000000 nxtomo-0.2.0/nxtomo/utils/io.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.883110 nxtomo-0.2.0/nxtomo/utils/test/
--rw-r--r--   0 payno     (1000) payno     (1000)     7620 2023-08-04 14:15:09.000000 nxtomo-0.2.0/nxtomo/utils/test/test_transformation.py
--rw-r--r--   0 payno     (1000) payno     (1000)    20767 2023-08-04 12:21:10.000000 nxtomo-0.2.0/nxtomo/utils/transformation.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3720 2023-08-04 13:05:11.000000 nxtomo-0.2.0/nxtomo/utils/utils.py
--rw-r--r--   0 payno     (1000) payno     (1000)       18 2023-08-04 14:16:59.000000 nxtomo-0.2.0/nxtomo/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-04 14:17:47.879110 nxtomo-0.2.0/nxtomo.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     3233 2023-08-04 14:17:47.000000 nxtomo-0.2.0/nxtomo.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)     1286 2023-08-04 14:17:47.000000 nxtomo-0.2.0/nxtomo.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2023-08-04 14:17:47.000000 nxtomo-0.2.0/nxtomo.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       67 2023-08-04 14:17:47.000000 nxtomo-0.2.0/nxtomo.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       22 2023-08-04 14:17:47.000000 nxtomo-0.2.0/nxtomo.egg-info/top_level.txt
--rw-r--r--   0 payno     (1000) payno     (1000)     2060 2023-08-04 12:59:55.000000 nxtomo-0.2.0/pyproject.toml
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-04 14:17:47.883110 nxtomo-0.2.0/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-04 12:40:53.000000 nxtomo-0.2.0/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 08:38:36.164622 nxtomo-1.0.0/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1266 2023-08-07 06:43:41.000000 nxtomo-1.0.0/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     3233 2023-08-07 08:38:36.164622 nxtomo-1.0.0/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      187 2023-08-07 06:43:41.000000 nxtomo-1.0.0/README.md
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 08:38:36.164622 nxtomo-1.0.0/nxtomo/
+-rw-r--r--   0 payno     (1000) payno     (1000)      116 2023-08-07 07:06:45.000000 nxtomo-1.0.0/nxtomo/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 08:38:36.164622 nxtomo-1.0.0/nxtomo/application/
+-rw-r--r--   0 payno     (1000) payno     (1000)    27475 2023-08-07 07:08:25.000000 nxtomo-1.0.0/nxtomo/application/nxtomo.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 08:38:36.164622 nxtomo-1.0.0/nxtomo/application/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)    16816 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/application/test/test_nxtomo.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8666 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/io.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 08:38:36.164622 nxtomo-1.0.0/nxtomo/nxobject/
+-rw-r--r--   0 payno     (1000) payno     (1000)      224 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    37631 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     7106 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3391 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    12997 2023-08-07 07:09:59.000000 nxtomo-1.0.0/nxtomo/nxobject/nxobject.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9619 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     6252 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     9446 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/nxtransformations.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 08:38:36.164622 nxtomo-1.0.0/nxtomo/nxobject/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)    14678 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/test/test_nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1333 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/test/test_nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1077 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/test/test_nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2706 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/test/test_nxobject.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     2076 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/test/test_nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1127 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/test/test_nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     5146 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/test/test_nxtransformations.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3588 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/nxobject/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 08:38:36.164622 nxtomo-1.0.0/nxtomo/paths/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/paths/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1242 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/paths/nxdetector.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      481 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/paths/nxinstrument.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      319 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/paths/nxmonitor.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      826 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/paths/nxsample.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      343 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/paths/nxsource.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    11877 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/paths/nxtomo.py
+-rw-r--r--   0 payno     (1000) payno     (1000)      543 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/paths/nxtransformations.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 08:38:36.164622 nxtomo-1.0.0/nxtomo/paths/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     6676 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/paths/test/test_backward_compatibility.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 08:38:36.164622 nxtomo-1.0.0/nxtomo/utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)       34 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/utils/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    15108 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/utils/frameappender.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     1990 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/utils/io.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 08:38:36.164622 nxtomo-1.0.0/nxtomo/utils/test/
+-rw-r--r--   0 payno     (1000) payno     (1000)     7620 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/utils/test/test_transformation.py
+-rw-r--r--   0 payno     (1000) payno     (1000)    20735 2023-08-07 07:47:54.000000 nxtomo-1.0.0/nxtomo/utils/transformation.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3720 2023-08-07 06:43:41.000000 nxtomo-1.0.0/nxtomo/utils/utils.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       18 2023-08-07 08:24:29.000000 nxtomo-1.0.0/nxtomo/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2023-08-07 08:38:36.164622 nxtomo-1.0.0/nxtomo.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3233 2023-08-07 08:38:36.000000 nxtomo-1.0.0/nxtomo.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)     1286 2023-08-07 08:38:36.000000 nxtomo-1.0.0/nxtomo.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2023-08-07 08:38:36.000000 nxtomo-1.0.0/nxtomo.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      160 2023-08-07 08:38:36.000000 nxtomo-1.0.0/nxtomo.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       11 2023-08-07 08:38:36.000000 nxtomo-1.0.0/nxtomo.egg-info/top_level.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)     2209 2023-08-07 07:21:19.000000 nxtomo-1.0.0/pyproject.toml
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-07 08:38:36.164622 nxtomo-1.0.0/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2023-08-07 06:43:41.000000 nxtomo-1.0.0/setup.py
```

### Comparing `nxtomo-0.2.0/LICENSE` & `nxtomo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/PKG-INFO` & `nxtomo-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxtomo
-Version: 0.2.0
+Version: 1.0.0
 Summary: module to create / edit NXtomo application
 Author-email: Henri Payno <henri.payno@esrf.fr>, Pierre Paleo <pierre.paleo@esrf.fr>, Alessandro Mirone <mirone@esrf.fr>, Jérôme Lesaint <jerome.lesaint@esrf.fr>
 License: 
         The nxtomo library goal is to provide a powerful python interface to read / write nexus NXtomo application
         
         nxtomo is distributed under the MIT license.
```

### Comparing `nxtomo-0.2.0/nxtomo/application/nxtomo.py` & `nxtomo-1.0.0/nxtomo/application/nxtomo.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/application/test/test_nxtomo.py` & `nxtomo-1.0.0/nxtomo/application/test/test_nxtomo.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/io.py` & `nxtomo-1.0.0/nxtomo/io.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/nxdetector.py` & `nxtomo-1.0.0/nxtomo/nxobject/nxdetector.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/nxinstrument.py` & `nxtomo-1.0.0/nxtomo/nxobject/nxinstrument.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/nxmonitor.py` & `nxtomo-1.0.0/nxtomo/nxobject/nxmonitor.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/nxobject.py` & `nxtomo-1.0.0/nxtomo/nxobject/nxobject.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/nxsample.py` & `nxtomo-1.0.0/nxtomo/nxobject/nxsample.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/nxsource.py` & `nxtomo-1.0.0/nxtomo/nxobject/nxsource.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/nxtransformations.py` & `nxtomo-1.0.0/nxtomo/nxobject/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxdetector.py` & `nxtomo-1.0.0/nxtomo/nxobject/test/test_nxdetector.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxinstrument.py` & `nxtomo-1.0.0/nxtomo/nxobject/test/test_nxinstrument.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxmonitor.py` & `nxtomo-1.0.0/nxtomo/nxobject/test/test_nxmonitor.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxobject.py` & `nxtomo-1.0.0/nxtomo/nxobject/test/test_nxobject.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxsample.py` & `nxtomo-1.0.0/nxtomo/nxobject/test/test_nxsample.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxsource.py` & `nxtomo-1.0.0/nxtomo/nxobject/test/test_nxsource.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/test/test_nxtransformations.py` & `nxtomo-1.0.0/nxtomo/nxobject/test/test_nxtransformations.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/nxobject/utils.py` & `nxtomo-1.0.0/nxtomo/nxobject/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/paths/nxdetector.py` & `nxtomo-1.0.0/nxtomo/paths/nxdetector.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/paths/nxsample.py` & `nxtomo-1.0.0/nxtomo/paths/nxsample.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/paths/nxtomo.py` & `nxtomo-1.0.0/nxtomo/paths/nxtomo.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/paths/nxtransformations.py` & `nxtomo-1.0.0/nxtomo/paths/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/paths/test/test_backward_compatibility.py` & `nxtomo-1.0.0/nxtomo/paths/test/test_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/utils/frameappender.py` & `nxtomo-1.0.0/nxtomo/utils/frameappender.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/utils/io.py` & `nxtomo-1.0.0/nxtomo/utils/io.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/utils/test/test_transformation.py` & `nxtomo-1.0.0/nxtomo/utils/test/test_transformation.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo/utils/transformation.py` & `nxtomo-1.0.0/nxtomo/utils/transformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -554,15 +554,14 @@
                 raise ValueError(
                     f"Unable to find transformation {transformation.depends_on}. Unable to build matrix. reason is: broken dependancy chain"
                 )
             else:
                 matrix = handle_transformation(
                     transformations[transformation.depends_on], matrix
                 )
-        print("update matrice")
         matrix = numpy.matmul(matrix, transformation.as_matrix())
         already_applied_transformations.add(transformation.axis_name)
         return matrix
 
     matrix = numpy.identity(3, dtype=numpy.float32)
     for transformation in transformations.values():
         matrix = handle_transformation(transformation, matrix)
```

### Comparing `nxtomo-0.2.0/nxtomo/utils/utils.py` & `nxtomo-1.0.0/nxtomo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/nxtomo.egg-info/PKG-INFO` & `nxtomo-1.0.0/nxtomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxtomo
-Version: 0.2.0
+Version: 1.0.0
 Summary: module to create / edit NXtomo application
 Author-email: Henri Payno <henri.payno@esrf.fr>, Pierre Paleo <pierre.paleo@esrf.fr>, Alessandro Mirone <mirone@esrf.fr>, Jérôme Lesaint <jerome.lesaint@esrf.fr>
 License: 
         The nxtomo library goal is to provide a powerful python interface to read / write nexus NXtomo application
         
         nxtomo is distributed under the MIT license.
```

### Comparing `nxtomo-0.2.0/nxtomo.egg-info/SOURCES.txt` & `nxtomo-1.0.0/nxtomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxtomo-0.2.0/pyproject.toml` & `nxtomo-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
 ]
 
 dependencies = [
     "numpy",
     "h5py>=3.0",
     "silx >= 0.15.0",
+    "pyunitsystem>=1.0",
 ]
 
 [project.urls]
 Homepage = "https://gitlab.esrf.fr/tomotools/nxtomo"
 Documentation = "https://gitlab.esrf.fr/tomotools/nxtomo/pages"
 Repository = "https://gitlab.esrf.fr/tomotools/nxtomo"
 Changelog = "https://gitlab.esrf.fr/tomotools/nxtomo/-/blob/master/CHANGELOG.md"
@@ -53,14 +54,21 @@
 [project.optional-dependencies]
 test = [
     "pytest",
 ]
 doc = [
     "sphinx",
     "nbsphinx",
+    "jupyterlab",
+    "ipykernel",
+    "nbconvert",
+    "pandoc",
+    "scikit-image",
+    "h5glance",
+    "jupyter_client",
 ]
 
 [build_sphinx]
 source_dir = "doc"
 build_dir = "build/sphinx"
 
 [tool.setuptools.dynamic]
```

