# Comparing `tmp/dstrial1-0.2.tar.gz` & `tmp/dstrial1-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstrial1-0.2.tar", last modified: Mon Aug  7 00:13:49 2023, max compression
+gzip compressed data, was "dstrial1-0.3.tar", last modified: Mon Aug  7 00:59:47 2023, max compression
```

## Comparing `dstrial1-0.2.tar` & `dstrial1-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 00:13:49.858249 dstrial1-0.2/
-drwxrwxrwx   0        0        0        0 2023-08-07 00:13:49.851252 dstrial1-0.2/DSTRIAL1.egg-info/
--rw-rw-rw-   0        0        0     1227 2023-08-07 00:13:49.000000 dstrial1-0.2/DSTRIAL1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-08-07 00:13:49.000000 dstrial1-0.2/DSTRIAL1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 00:13:49.000000 dstrial1-0.2/DSTRIAL1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-08-07 00:13:49.000000 dstrial1-0.2/DSTRIAL1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 00:13:49.000000 dstrial1-0.2/DSTRIAL1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1093 2023-08-06 22:44:16.000000 dstrial1-0.2/LICENSE
--rw-rw-rw-   0        0        0     1227 2023-08-07 00:13:49.857250 dstrial1-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      635 2023-08-06 23:35:04.000000 dstrial1-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-07 00:13:49.859247 dstrial1-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1176 2023-08-07 00:10:04.000000 dstrial1-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 00:59:47.437479 dstrial1-0.3/
+drwxrwxrwx   0        0        0        0 2023-08-07 00:59:47.430484 dstrial1-0.3/DSTRIAL1.egg-info/
+-rw-rw-rw-   0        0        0     1382 2023-08-07 00:59:47.000000 dstrial1-0.3/DSTRIAL1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-08-07 00:59:47.000000 dstrial1-0.3/DSTRIAL1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 00:59:47.000000 dstrial1-0.3/DSTRIAL1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-07 00:59:47.000000 dstrial1-0.3/DSTRIAL1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 00:59:47.000000 dstrial1-0.3/DSTRIAL1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1093 2023-08-06 22:44:16.000000 dstrial1-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1382 2023-08-07 00:59:47.436478 dstrial1-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      635 2023-08-06 23:35:04.000000 dstrial1-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 00:59:47.437479 dstrial1-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2023-08-07 00:58:20.000000 dstrial1-0.3/setup.py
```

### Comparing `dstrial1-0.2/DSTRIAL1.egg-info/PKG-INFO` & `dstrial1-0.3/DSTRIAL1.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: dstrial1
-Version: 0.2
+Version: 0.3
 Summary: Data cleaning package
 Home-page: https://github.com/muganga-charles/dstrial1.git
 Author: Charles Muganga
 Author-email: mugangacharle5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dstrial1
 First trial for package
 ## FUNCTIONS
```

### Comparing `dstrial1-0.2/LICENSE` & `dstrial1-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dstrial1-0.2/PKG-INFO` & `dstrial1-0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: dstrial1
-Version: 0.2
+Version: 0.3
 Summary: Data cleaning package
 Home-page: https://github.com/muganga-charles/dstrial1.git
 Author: Charles Muganga
 Author-email: mugangacharle5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dstrial1
 First trial for package
 ## FUNCTIONS
```

### Comparing `dstrial1-0.2/README.md` & `dstrial1-0.3/README.md`

 * *Files identical despite different names*

### Comparing `dstrial1-0.2/setup.py` & `dstrial1-0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 PACKAGE_NAME = 'dstrial1'
-VERSION = '0.2'
+VERSION = '0.3'
 AUTHOR = 'Charles Muganga'
 AUTHOR_EMAIL = 'mugangacharle5@gmail.com'
 URL = 'https://github.com/muganga-charles/dstrial1.git'
 LICENSE = 'MIT'
 # Read content of Readme.md
 with open("README.md", "r", encoding = 'utf-8') as f:
     long_description = f.read()
@@ -32,10 +32,13 @@
     install_requires=INSTALL_REQUIRES,
     classifiers=[
            "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
     ],
 )
```

