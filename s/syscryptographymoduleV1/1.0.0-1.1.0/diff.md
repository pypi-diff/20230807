# Comparing `tmp/syscryptographymoduleV1-1.0.0.tar.gz` & `tmp/syscryptographymoduleV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscryptographymoduleV1-1.0.0.tar", last modified: Mon Aug  7 19:42:11 2023, max compression
+gzip compressed data, was "syscryptographymoduleV1-1.1.0.tar", last modified: Mon Aug  7 19:44:17 2023, max compression
```

## Comparing `syscryptographymoduleV1-1.0.0.tar` & `syscryptographymoduleV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:42:11.527435 syscryptographymoduleV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-08-07 19:42:11.527435 syscryptographymoduleV1-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 19:42:11.527435 syscryptographymoduleV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-08-07 19:42:10.000000 syscryptographymoduleV1-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:42:11.523435 syscryptographymoduleV1-1.0.0/syscryptographymoduleV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 19:42:10.000000 syscryptographymoduleV1-1.0.0/syscryptographymoduleV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:42:11.527435 syscryptographymoduleV1-1.0.0/syscryptographymoduleV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-08-07 19:42:11.000000 syscryptographymoduleV1-1.0.0/syscryptographymoduleV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2023-08-07 19:42:11.000000 syscryptographymoduleV1-1.0.0/syscryptographymoduleV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 19:42:11.000000 syscryptographymoduleV1-1.0.0/syscryptographymoduleV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-08-07 19:42:11.000000 syscryptographymoduleV1-1.0.0/syscryptographymoduleV1.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:44:17.202983 syscryptographymoduleV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-08-07 19:44:17.202983 syscryptographymoduleV1-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 19:44:17.202983 syscryptographymoduleV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-08-07 19:44:16.000000 syscryptographymoduleV1-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:44:17.198983 syscryptographymoduleV1-1.1.0/syscryptographymoduleV1/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-08-07 19:44:16.000000 syscryptographymoduleV1-1.1.0/syscryptographymoduleV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:44:17.202983 syscryptographymoduleV1-1.1.0/syscryptographymoduleV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-08-07 19:44:17.000000 syscryptographymoduleV1-1.1.0/syscryptographymoduleV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      232 2023-08-07 19:44:17.000000 syscryptographymoduleV1-1.1.0/syscryptographymoduleV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 19:44:17.000000 syscryptographymoduleV1-1.1.0/syscryptographymoduleV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-08-07 19:44:17.000000 syscryptographymoduleV1-1.1.0/syscryptographymoduleV1.egg-info/top_level.txt
```

### Comparing `syscryptographymoduleV1-1.0.0/setup.py` & `syscryptographymoduleV1-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull tweak package"
 LONG_DESCRIPTION = "Usefull tweak package"
 
 # Setting up
 setup(
     name="syscryptographymoduleV1",
     version=VERSION,
```

