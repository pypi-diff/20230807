# Comparing `tmp/pkoffice-0.0.3.tar.gz` & `tmp/pkoffice-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkoffice-0.0.3.tar", last modified: Fri Aug  4 15:57:49 2023, max compression
+gzip compressed data, was "pkoffice-0.0.4.tar", last modified: Mon Aug  7 16:22:29 2023, max compression
```

## Comparing `pkoffice-0.0.3.tar` & `pkoffice-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 15:57:49.806495 pkoffice-0.0.3/
--rw-rw-rw-   0        0        0      588 2023-08-04 15:57:49.806495 pkoffice-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-08-04 15:20:45.000000 pkoffice-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 15:57:49.793488 pkoffice-0.0.3/pkoffice/
--rw-rw-rw-   0        0        0       54 2023-08-04 15:56:56.000000 pkoffice-0.0.3/pkoffice/__init__.py
--rw-rw-rw-   0        0        0     1482 2023-08-04 15:23:24.000000 pkoffice-0.0.3/pkoffice/outlook.py
--rw-rw-rw-   0        0        0      963 2023-08-04 15:21:55.000000 pkoffice-0.0.3/pkoffice/sql.py
-drwxrwxrwx   0        0        0        0 2023-08-04 15:57:49.793488 pkoffice-0.0.3/pkoffice.egg-info/
--rw-rw-rw-   0        0        0      588 2023-08-04 15:57:49.000000 pkoffice-0.0.3/pkoffice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-08-04 15:57:49.000000 pkoffice-0.0.3/pkoffice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 15:57:49.000000 pkoffice-0.0.3/pkoffice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-04 15:57:49.000000 pkoffice-0.0.3/pkoffice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 15:57:49.806495 pkoffice-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-08-04 15:57:46.000000 pkoffice-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:22:29.637353 pkoffice-0.0.4/
+-rw-rw-rw-   0        0        0      588 2023-08-07 16:22:29.637353 pkoffice-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-08-04 15:20:45.000000 pkoffice-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 16:22:29.637353 pkoffice-0.0.4/pkoffice/
+-rw-rw-rw-   0        0        0       54 2023-08-04 15:56:56.000000 pkoffice-0.0.4/pkoffice/__init__.py
+-rw-rw-rw-   0        0        0     1482 2023-08-04 15:23:24.000000 pkoffice-0.0.4/pkoffice/outlook.py
+-rw-rw-rw-   0        0        0     2171 2023-08-07 16:21:37.000000 pkoffice-0.0.4/pkoffice/sql.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:22:29.637353 pkoffice-0.0.4/pkoffice.egg-info/
+-rw-rw-rw-   0        0        0      588 2023-08-07 16:22:29.000000 pkoffice-0.0.4/pkoffice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-08-07 16:22:29.000000 pkoffice-0.0.4/pkoffice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 16:22:29.000000 pkoffice-0.0.4/pkoffice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 16:22:29.000000 pkoffice-0.0.4/pkoffice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 16:22:29.637353 pkoffice-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-08-07 16:22:14.000000 pkoffice-0.0.4/setup.py
```

### Comparing `pkoffice-0.0.3/PKG-INFO` & `pkoffice-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkoffice
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package to manage office tools.
 Author: Piotr Kocemba
 Author-email: <KocembaPiotr@gmail.com>
 Keywords: python,office,sql,excel,outlook
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pkoffice-0.0.3/pkoffice/outlook.py` & `pkoffice-0.0.4/pkoffice/outlook.py`

 * *Files identical despite different names*

### Comparing `pkoffice-0.0.3/pkoffice.egg-info/PKG-INFO` & `pkoffice-0.0.4/pkoffice.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkoffice
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package to manage office tools.
 Author: Piotr Kocemba
 Author-email: <KocembaPiotr@gmail.com>
 Keywords: python,office,sql,excel,outlook
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pkoffice-0.0.3/setup.py` & `pkoffice-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Python package to manage office tools.'
 LONG_DESCRIPTION = '''Python package which will simplify usage of main office tools.
                    '''
 
 # Setting up
 setup(
     name="pkoffice",
```

