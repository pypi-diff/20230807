# Comparing `tmp/pythonsqlipackagesV1-1.0.0.tar.gz` & `tmp/pythonsqlipackagesV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsqlipackagesV1-1.0.0.tar", last modified: Mon Aug  7 03:24:30 2023, max compression
+gzip compressed data, was "pythonsqlipackagesV1-1.1.0.tar", last modified: Mon Aug  7 03:26:35 2023, max compression
```

## Comparing `pythonsqlipackagesV1-1.0.0.tar` & `pythonsqlipackagesV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 03:24:30.381715 pythonsqlipackagesV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      348 2023-08-07 03:24:30.381715 pythonsqlipackagesV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 03:24:30.377715 pythonsqlipackagesV1-1.0.0/pythonsqlipackagesV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 03:24:29.000000 pythonsqlipackagesV1-1.0.0/pythonsqlipackagesV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 03:24:30.381715 pythonsqlipackagesV1-1.0.0/pythonsqlipackagesV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      348 2023-08-07 03:24:30.000000 pythonsqlipackagesV1-1.0.0/pythonsqlipackagesV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-08-07 03:24:30.000000 pythonsqlipackagesV1-1.0.0/pythonsqlipackagesV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 03:24:30.000000 pythonsqlipackagesV1-1.0.0/pythonsqlipackagesV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 03:24:30.000000 pythonsqlipackagesV1-1.0.0/pythonsqlipackagesV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 03:24:30.381715 pythonsqlipackagesV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      561 2023-08-07 03:24:29.000000 pythonsqlipackagesV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 03:26:35.897276 pythonsqlipackagesV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-08-07 03:26:35.897276 pythonsqlipackagesV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 03:26:35.893276 pythonsqlipackagesV1-1.1.0/pythonsqlipackagesV1/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-08-07 03:26:35.000000 pythonsqlipackagesV1-1.1.0/pythonsqlipackagesV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 03:26:35.897276 pythonsqlipackagesV1-1.1.0/pythonsqlipackagesV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-08-07 03:26:35.000000 pythonsqlipackagesV1-1.1.0/pythonsqlipackagesV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-08-07 03:26:35.000000 pythonsqlipackagesV1-1.1.0/pythonsqlipackagesV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 03:26:35.000000 pythonsqlipackagesV1-1.1.0/pythonsqlipackagesV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 03:26:35.000000 pythonsqlipackagesV1-1.1.0/pythonsqlipackagesV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 03:26:35.897276 pythonsqlipackagesV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      561 2023-08-07 03:26:35.000000 pythonsqlipackagesV1-1.1.0/setup.py
```

### Comparing `pythonsqlipackagesV1-1.0.0/setup.py` & `pythonsqlipackagesV1-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull tweak package"
 LONG_DESCRIPTION = "Usefull tweak package"
 
 # Setting up
 setup(
     name="pythonsqlipackagesV1",
     version=VERSION,
```

