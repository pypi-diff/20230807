# Comparing `tmp/pythonsqliextV2-1.0.0.tar.gz` & `tmp/pythonsqliextV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsqliextV2-1.0.0.tar", last modified: Mon Aug  7 13:14:11 2023, max compression
+gzip compressed data, was "pythonsqliextV2-1.1.0.tar", last modified: Mon Aug  7 13:16:17 2023, max compression
```

## Comparing `pythonsqliextV2-1.0.0.tar` & `pythonsqliextV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:14:11.991468 pythonsqliextV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      343 2023-08-07 13:14:11.991468 pythonsqliextV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:14:11.987468 pythonsqliextV2-1.0.0/pythonsqliextV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 13:14:11.000000 pythonsqliextV2-1.0.0/pythonsqliextV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:14:11.991468 pythonsqliextV2-1.0.0/pythonsqliextV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      343 2023-08-07 13:14:11.000000 pythonsqliextV2-1.0.0/pythonsqliextV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-08-07 13:14:11.000000 pythonsqliextV2-1.0.0/pythonsqliextV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 13:14:11.000000 pythonsqliextV2-1.0.0/pythonsqliextV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-08-07 13:14:11.000000 pythonsqliextV2-1.0.0/pythonsqliextV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 13:14:11.991468 pythonsqliextV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      556 2023-08-07 13:14:11.000000 pythonsqliextV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:16:17.019108 pythonsqliextV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-08-07 13:16:17.019108 pythonsqliextV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:16:17.015108 pythonsqliextV2-1.1.0/pythonsqliextV2/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-08-07 13:16:16.000000 pythonsqliextV2-1.1.0/pythonsqliextV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:16:17.015108 pythonsqliextV2-1.1.0/pythonsqliextV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-08-07 13:16:16.000000 pythonsqliextV2-1.1.0/pythonsqliextV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-08-07 13:16:16.000000 pythonsqliextV2-1.1.0/pythonsqliextV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 13:16:16.000000 pythonsqliextV2-1.1.0/pythonsqliextV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-07 13:16:16.000000 pythonsqliextV2-1.1.0/pythonsqliextV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 13:16:17.019108 pythonsqliextV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      556 2023-08-07 13:16:16.000000 pythonsqliextV2-1.1.0/setup.py
```

### Comparing `pythonsqliextV2-1.0.0/setup.py` & `pythonsqliextV2-1.1.0/setup.py`

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
     name="pythonsqliextV2",
     version=VERSION,
```

