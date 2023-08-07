# Comparing `tmp/Gehu_erp-0.1.tar.gz` & `tmp/Gehu_erp-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Gehu_erp-0.1.tar", last modified: Mon Aug  7 18:30:12 2023, max compression
+gzip compressed data, was "Gehu_erp-0.2.tar", last modified: Mon Aug  7 18:42:01 2023, max compression
```

## Comparing `Gehu_erp-0.1.tar` & `Gehu_erp-0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 18:30:12.001459 Gehu_erp-0.1/
-drwxrwxrwx   0        0        0        0 2023-08-07 18:30:12.001459 Gehu_erp-0.1/Gehu_erp.egg-info/
--rw-rw-rw-   0        0        0      323 2023-08-07 18:30:11.000000 Gehu_erp-0.1/Gehu_erp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-08-07 18:30:11.000000 Gehu_erp-0.1/Gehu_erp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 18:30:11.000000 Gehu_erp-0.1/Gehu_erp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-08-07 18:30:11.000000 Gehu_erp-0.1/Gehu_erp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-07 18:30:11.000000 Gehu_erp-0.1/Gehu_erp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      323 2023-08-07 18:30:12.001459 Gehu_erp-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 18:30:12.001459 Gehu_erp-0.1/erp/
--rw-rw-rw-   0        0        0       71 2023-08-07 17:14:37.000000 Gehu_erp-0.1/erp/__init__.py
--rw-rw-rw-   0        0        0     3289 2023-08-07 17:56:50.000000 Gehu_erp-0.1/erp/client.py
-drwxrwxrwx   0        0        0        0 2023-08-07 18:30:12.001459 Gehu_erp-0.1/erp/util/
--rw-rw-rw-   0        0        0       22 2023-08-07 17:14:02.000000 Gehu_erp-0.1/erp/util/__init__.py
--rw-rw-rw-   0        0        0     1903 2023-08-07 16:45:38.000000 Gehu_erp-0.1/erp/util/headers.py
--rw-rw-rw-   0        0        0       42 2023-08-07 18:30:12.001459 Gehu_erp-0.1/setup.cfg
--rw-rw-rw-   0        0        0      545 2023-08-07 18:29:34.000000 Gehu_erp-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:42:01.414814 Gehu_erp-0.2/
+drwxrwxrwx   0        0        0        0 2023-08-07 18:42:01.414814 Gehu_erp-0.2/Gehu_erp.egg-info/
+-rw-rw-rw-   0        0        0     2219 2023-08-07 18:42:01.000000 Gehu_erp-0.2/Gehu_erp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-08-07 18:42:01.000000 Gehu_erp-0.2/Gehu_erp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 18:42:01.000000 Gehu_erp-0.2/Gehu_erp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-08-07 18:42:01.000000 Gehu_erp-0.2/Gehu_erp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-07 18:42:01.000000 Gehu_erp-0.2/Gehu_erp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2219 2023-08-07 18:42:01.414814 Gehu_erp-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1851 2023-08-07 18:40:16.000000 Gehu_erp-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 18:42:01.414814 Gehu_erp-0.2/erp/
+-rw-rw-rw-   0        0        0       71 2023-08-07 17:14:37.000000 Gehu_erp-0.2/erp/__init__.py
+-rw-rw-rw-   0        0        0     3289 2023-08-07 17:56:50.000000 Gehu_erp-0.2/erp/client.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:42:01.414814 Gehu_erp-0.2/erp/util/
+-rw-rw-rw-   0        0        0       22 2023-08-07 17:14:02.000000 Gehu_erp-0.2/erp/util/__init__.py
+-rw-rw-rw-   0        0        0     1903 2023-08-07 16:45:38.000000 Gehu_erp-0.2/erp/util/headers.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 18:42:01.414814 Gehu_erp-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      721 2023-08-07 18:41:15.000000 Gehu_erp-0.2/setup.py
```

### Comparing `Gehu_erp-0.1/erp/client.py` & `Gehu_erp-0.2/erp/client.py`

 * *Files identical despite different names*

### Comparing `Gehu_erp-0.1/erp/util/headers.py` & `Gehu_erp-0.2/erp/util/headers.py`

 * *Files identical despite different names*

### Comparing `Gehu_erp-0.1/setup.py` & `Gehu_erp-0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
     name="Gehu_erp",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     install_requires=[
         "requests",
         "Pillow",
         "beautifulsoup4"
     ],
-    
     author="yato",
     description="A Python library for interacting with GEHU Student API",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     url="https://github.com/aminobot22",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

