# Comparing `tmp/DSTRIAL1-0.1.tar.gz` & `tmp/dstrial1-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DSTRIAL1-0.1.tar", last modified: Sun Aug  6 23:47:15 2023, max compression
+gzip compressed data, was "dstrial1-0.2.tar", last modified: Mon Aug  7 00:13:49 2023, max compression
```

## Comparing `DSTRIAL1-0.1.tar` & `dstrial1-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 23:47:15.964738 DSTRIAL1-0.1/
-drwxrwxrwx   0        0        0        0 2023-08-06 23:47:15.960742 DSTRIAL1-0.1/DSTRIAL1.egg-info/
--rw-rw-rw-   0        0        0     1227 2023-08-06 23:47:15.000000 DSTRIAL1-0.1/DSTRIAL1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-08-06 23:47:15.000000 DSTRIAL1-0.1/DSTRIAL1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 23:47:15.000000 DSTRIAL1-0.1/DSTRIAL1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-08-06 23:47:15.000000 DSTRIAL1-0.1/DSTRIAL1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 23:47:15.000000 DSTRIAL1-0.1/DSTRIAL1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1093 2023-08-06 22:44:16.000000 DSTRIAL1-0.1/LICENSE
--rw-rw-rw-   0        0        0     1227 2023-08-06 23:47:15.962740 DSTRIAL1-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      635 2023-08-06 23:35:04.000000 DSTRIAL1-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-06 23:47:15.964738 DSTRIAL1-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1176 2023-08-06 23:22:00.000000 DSTRIAL1-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 00:13:49.858249 dstrial1-0.2/
+drwxrwxrwx   0        0        0        0 2023-08-07 00:13:49.851252 dstrial1-0.2/DSTRIAL1.egg-info/
+-rw-rw-rw-   0        0        0     1227 2023-08-07 00:13:49.000000 dstrial1-0.2/DSTRIAL1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-08-07 00:13:49.000000 dstrial1-0.2/DSTRIAL1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 00:13:49.000000 dstrial1-0.2/DSTRIAL1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-07 00:13:49.000000 dstrial1-0.2/DSTRIAL1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 00:13:49.000000 dstrial1-0.2/DSTRIAL1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1093 2023-08-06 22:44:16.000000 dstrial1-0.2/LICENSE
+-rw-rw-rw-   0        0        0     1227 2023-08-07 00:13:49.857250 dstrial1-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      635 2023-08-06 23:35:04.000000 dstrial1-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 00:13:49.859247 dstrial1-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1176 2023-08-07 00:10:04.000000 dstrial1-0.2/setup.py
```

### Comparing `DSTRIAL1-0.1/DSTRIAL1.egg-info/PKG-INFO` & `dstrial1-0.2/DSTRIAL1.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: DSTRIAL1
-Version: 0.1
+Name: dstrial1
+Version: 0.2
 Summary: Data cleaning package
 Home-page: https://github.com/muganga-charles/dstrial1.git
 Author: Charles Muganga
 Author-email: mugangacharle5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `DSTRIAL1-0.1/LICENSE` & `dstrial1-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DSTRIAL1-0.1/PKG-INFO` & `dstrial1-0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: DSTRIAL1
-Version: 0.1
+Name: dstrial1
+Version: 0.2
 Summary: Data cleaning package
 Home-page: https://github.com/muganga-charles/dstrial1.git
 Author: Charles Muganga
 Author-email: mugangacharle5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `DSTRIAL1-0.1/README.md` & `dstrial1-0.2/README.md`

 * *Files identical despite different names*

### Comparing `DSTRIAL1-0.1/setup.py` & `dstrial1-0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
-PACKAGE_NAME = 'DSTRIAL1'
-VERSION = '0.1'
+PACKAGE_NAME = 'dstrial1'
+VERSION = '0.2'
 AUTHOR = 'Charles Muganga'
 AUTHOR_EMAIL = 'mugangacharle5@gmail.com'
 URL = 'https://github.com/muganga-charles/dstrial1.git'
 LICENSE = 'MIT'
 # Read content of Readme.md
 with open("README.md", "r", encoding = 'utf-8') as f:
     long_description = f.read()
```

