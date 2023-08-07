# Comparing `tmp/pythoncryptV2-1.0.0.tar.gz` & `tmp/pythoncryptV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncryptV2-1.0.0.tar", last modified: Mon Aug  7 14:55:35 2023, max compression
+gzip compressed data, was "pythoncryptV2-1.1.0.tar", last modified: Mon Aug  7 14:57:40 2023, max compression
```

## Comparing `pythoncryptV2-1.0.0.tar` & `pythoncryptV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:55:35.219376 pythoncryptV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      341 2023-08-07 14:55:35.219376 pythoncryptV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:55:35.215376 pythoncryptV2-1.0.0/pythoncryptV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 14:55:34.000000 pythoncryptV2-1.0.0/pythoncryptV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:55:35.219376 pythoncryptV2-1.0.0/pythoncryptV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      341 2023-08-07 14:55:35.000000 pythoncryptV2-1.0.0/pythoncryptV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2023-08-07 14:55:35.000000 pythoncryptV2-1.0.0/pythoncryptV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 14:55:35.000000 pythoncryptV2-1.0.0/pythoncryptV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-08-07 14:55:35.000000 pythoncryptV2-1.0.0/pythoncryptV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 14:55:35.219376 pythoncryptV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      554 2023-08-07 14:55:34.000000 pythoncryptV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:57:40.806893 pythoncryptV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-08-07 14:57:40.806893 pythoncryptV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:57:40.802893 pythoncryptV2-1.1.0/pythoncryptV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-08-07 14:57:40.000000 pythoncryptV2-1.1.0/pythoncryptV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 14:57:40.806893 pythoncryptV2-1.1.0/pythoncryptV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-08-07 14:57:40.000000 pythoncryptV2-1.1.0/pythoncryptV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2023-08-07 14:57:40.000000 pythoncryptV2-1.1.0/pythoncryptV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 14:57:40.000000 pythoncryptV2-1.1.0/pythoncryptV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-08-07 14:57:40.000000 pythoncryptV2-1.1.0/pythoncryptV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 14:57:40.806893 pythoncryptV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      554 2023-08-07 14:57:40.000000 pythoncryptV2-1.1.0/setup.py
```

### Comparing `pythoncryptV2-1.0.0/setup.py` & `pythoncryptV2-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull tweak package"
 LONG_DESCRIPTION = "Usefull tweak package"
 
 # Setting up
 setup(
     name="pythoncryptV2",
     version=VERSION,
```

