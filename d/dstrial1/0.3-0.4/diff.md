# Comparing `tmp/dstrial1-0.3.tar.gz` & `tmp/dstrial1-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstrial1-0.3.tar", last modified: Mon Aug  7 00:59:47 2023, max compression
+gzip compressed data, was "dstrial1-0.4.tar", last modified: Mon Aug  7 12:26:31 2023, max compression
```

## Comparing `dstrial1-0.3.tar` & `dstrial1-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 00:59:47.437479 dstrial1-0.3/
-drwxrwxrwx   0        0        0        0 2023-08-07 00:59:47.430484 dstrial1-0.3/DSTRIAL1.egg-info/
--rw-rw-rw-   0        0        0     1382 2023-08-07 00:59:47.000000 dstrial1-0.3/DSTRIAL1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-08-07 00:59:47.000000 dstrial1-0.3/DSTRIAL1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 00:59:47.000000 dstrial1-0.3/DSTRIAL1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-08-07 00:59:47.000000 dstrial1-0.3/DSTRIAL1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 00:59:47.000000 dstrial1-0.3/DSTRIAL1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1093 2023-08-06 22:44:16.000000 dstrial1-0.3/LICENSE
--rw-rw-rw-   0        0        0     1382 2023-08-07 00:59:47.436478 dstrial1-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      635 2023-08-06 23:35:04.000000 dstrial1-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-08-07 00:59:47.437479 dstrial1-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1328 2023-08-07 00:58:20.000000 dstrial1-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:26:31.819700 dstrial1-0.4/
+drwxrwxrwx   0        0        0        0 2023-08-07 12:26:31.809706 dstrial1-0.4/DSTRIAL1.egg-info/
+-rw-rw-rw-   0        0        0     1382 2023-08-07 12:26:31.000000 dstrial1-0.4/DSTRIAL1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-08-07 12:26:31.000000 dstrial1-0.4/DSTRIAL1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 12:26:31.000000 dstrial1-0.4/DSTRIAL1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-07 12:26:31.000000 dstrial1-0.4/DSTRIAL1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 12:26:31.000000 dstrial1-0.4/DSTRIAL1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1093 2023-08-06 22:44:16.000000 dstrial1-0.4/LICENSE
+-rw-rw-rw-   0        0        0     1382 2023-08-07 12:26:31.817702 dstrial1-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      635 2023-08-06 23:35:04.000000 dstrial1-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 12:26:31.820701 dstrial1-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2023-08-07 12:22:14.000000 dstrial1-0.4/setup.py
```

### Comparing `dstrial1-0.3/DSTRIAL1.egg-info/PKG-INFO` & `dstrial1-0.4/DSTRIAL1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dstrial1
-Version: 0.3
+Version: 0.4
 Summary: Data cleaning package
 Home-page: https://github.com/muganga-charles/dstrial1.git
 Author: Charles Muganga
 Author-email: mugangacharle5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dstrial1-0.3/LICENSE` & `dstrial1-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dstrial1-0.3/PKG-INFO` & `dstrial1-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dstrial1
-Version: 0.3
+Version: 0.4
 Summary: Data cleaning package
 Home-page: https://github.com/muganga-charles/dstrial1.git
 Author: Charles Muganga
 Author-email: mugangacharle5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dstrial1-0.3/README.md` & `dstrial1-0.4/README.md`

 * *Files identical despite different names*

### Comparing `dstrial1-0.3/setup.py` & `dstrial1-0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 PACKAGE_NAME = 'dstrial1'
-VERSION = '0.3'
+VERSION = '0.4'
 AUTHOR = 'Charles Muganga'
 AUTHOR_EMAIL = 'mugangacharle5@gmail.com'
 URL = 'https://github.com/muganga-charles/dstrial1.git'
 LICENSE = 'MIT'
 # Read content of Readme.md
 with open("README.md", "r", encoding = 'utf-8') as f:
     long_description = f.read()
```

