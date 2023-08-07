# Comparing `tmp/dstrial1-0.4.tar.gz` & `tmp/dstrial1-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstrial1-0.4.tar", last modified: Mon Aug  7 12:26:31 2023, max compression
+gzip compressed data, was "dstrial1-0.5.tar", last modified: Mon Aug  7 12:43:39 2023, max compression
```

## Comparing `dstrial1-0.4.tar` & `dstrial1-0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 12:26:31.819700 dstrial1-0.4/
-drwxrwxrwx   0        0        0        0 2023-08-07 12:26:31.809706 dstrial1-0.4/DSTRIAL1.egg-info/
--rw-rw-rw-   0        0        0     1382 2023-08-07 12:26:31.000000 dstrial1-0.4/DSTRIAL1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-08-07 12:26:31.000000 dstrial1-0.4/DSTRIAL1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 12:26:31.000000 dstrial1-0.4/DSTRIAL1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-08-07 12:26:31.000000 dstrial1-0.4/DSTRIAL1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 12:26:31.000000 dstrial1-0.4/DSTRIAL1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1093 2023-08-06 22:44:16.000000 dstrial1-0.4/LICENSE
--rw-rw-rw-   0        0        0     1382 2023-08-07 12:26:31.817702 dstrial1-0.4/PKG-INFO
--rw-rw-rw-   0        0        0      635 2023-08-06 23:35:04.000000 dstrial1-0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-08-07 12:26:31.820701 dstrial1-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1328 2023-08-07 12:22:14.000000 dstrial1-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:43:39.364154 dstrial1-0.5/
+drwxrwxrwx   0        0        0        0 2023-08-07 12:43:39.352162 dstrial1-0.5/DSTRIAL1.egg-info/
+-rw-rw-rw-   0        0        0     1382 2023-08-07 12:43:38.000000 dstrial1-0.5/DSTRIAL1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-08-07 12:43:39.000000 dstrial1-0.5/DSTRIAL1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 12:43:38.000000 dstrial1-0.5/DSTRIAL1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-07 12:43:38.000000 dstrial1-0.5/DSTRIAL1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 12:43:38.000000 dstrial1-0.5/DSTRIAL1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1093 2023-08-06 22:44:16.000000 dstrial1-0.5/LICENSE
+-rw-rw-rw-   0        0        0     1382 2023-08-07 12:43:39.363157 dstrial1-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      635 2023-08-06 23:35:04.000000 dstrial1-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 12:43:39.365155 dstrial1-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2023-08-07 12:42:33.000000 dstrial1-0.5/setup.py
```

### Comparing `dstrial1-0.4/DSTRIAL1.egg-info/PKG-INFO` & `dstrial1-0.5/DSTRIAL1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dstrial1
-Version: 0.4
+Version: 0.5
 Summary: Data cleaning package
 Home-page: https://github.com/muganga-charles/dstrial1.git
 Author: Charles Muganga
 Author-email: mugangacharle5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dstrial1-0.4/LICENSE` & `dstrial1-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dstrial1-0.4/PKG-INFO` & `dstrial1-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dstrial1
-Version: 0.4
+Version: 0.5
 Summary: Data cleaning package
 Home-page: https://github.com/muganga-charles/dstrial1.git
 Author: Charles Muganga
 Author-email: mugangacharle5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dstrial1-0.4/README.md` & `dstrial1-0.5/README.md`

 * *Files identical despite different names*

### Comparing `dstrial1-0.4/setup.py` & `dstrial1-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 PACKAGE_NAME = 'dstrial1'
-VERSION = '0.4'
+VERSION = '0.5'
 AUTHOR = 'Charles Muganga'
 AUTHOR_EMAIL = 'mugangacharle5@gmail.com'
 URL = 'https://github.com/muganga-charles/dstrial1.git'
 LICENSE = 'MIT'
 # Read content of Readme.md
 with open("README.md", "r", encoding = 'utf-8') as f:
     long_description = f.read()
```

