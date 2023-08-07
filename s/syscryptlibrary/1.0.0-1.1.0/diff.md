# Comparing `tmp/syscryptlibrary-1.0.0.tar.gz` & `tmp/syscryptlibrary-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscryptlibrary-1.0.0.tar", last modified: Mon Aug  7 18:22:38 2023, max compression
+gzip compressed data, was "syscryptlibrary-1.1.0.tar", last modified: Mon Aug  7 18:24:43 2023, max compression
```

## Comparing `syscryptlibrary-1.0.0.tar` & `syscryptlibrary-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 18:22:38.227319 syscryptlibrary-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      343 2023-08-07 18:22:38.227319 syscryptlibrary-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 18:22:38.227319 syscryptlibrary-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      556 2023-08-07 18:22:37.000000 syscryptlibrary-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 18:22:38.227319 syscryptlibrary-1.0.0/syscryptlibrary/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 18:22:37.000000 syscryptlibrary-1.0.0/syscryptlibrary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 18:22:38.227319 syscryptlibrary-1.0.0/syscryptlibrary.egg-info/
--rw-r--r--   0 root         (0) root         (0)      343 2023-08-07 18:22:38.000000 syscryptlibrary-1.0.0/syscryptlibrary.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-08-07 18:22:38.000000 syscryptlibrary-1.0.0/syscryptlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 18:22:38.000000 syscryptlibrary-1.0.0/syscryptlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-08-07 18:22:38.000000 syscryptlibrary-1.0.0/syscryptlibrary.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 18:24:43.254918 syscryptlibrary-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-08-07 18:24:43.254918 syscryptlibrary-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 18:24:43.254918 syscryptlibrary-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      556 2023-08-07 18:24:42.000000 syscryptlibrary-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 18:24:43.254918 syscryptlibrary-1.1.0/syscryptlibrary/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-08-07 18:24:42.000000 syscryptlibrary-1.1.0/syscryptlibrary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 18:24:43.254918 syscryptlibrary-1.1.0/syscryptlibrary.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-08-07 18:24:43.000000 syscryptlibrary-1.1.0/syscryptlibrary.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-08-07 18:24:43.000000 syscryptlibrary-1.1.0/syscryptlibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 18:24:43.000000 syscryptlibrary-1.1.0/syscryptlibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-07 18:24:43.000000 syscryptlibrary-1.1.0/syscryptlibrary.egg-info/top_level.txt
```

### Comparing `syscryptlibrary-1.0.0/setup.py` & `syscryptlibrary-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull tweak package"
 LONG_DESCRIPTION = "Usefull tweak package"
 
 # Setting up
 setup(
     name="syscryptlibrary",
     version=VERSION,
```

