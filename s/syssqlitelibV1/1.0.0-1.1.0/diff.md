# Comparing `tmp/syssqlitelibV1-1.0.0.tar.gz` & `tmp/syssqlitelibV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqlitelibV1-1.0.0.tar", last modified: Mon Aug  7 21:46:11 2023, max compression
+gzip compressed data, was "syssqlitelibV1-1.1.0.tar", last modified: Mon Aug  7 21:48:19 2023, max compression
```

## Comparing `syssqlitelibV1-1.0.0.tar` & `syssqlitelibV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 21:46:11.562563 syssqlitelibV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      342 2023-08-07 21:46:11.562563 syssqlitelibV1-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 21:46:11.562563 syssqlitelibV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      555 2023-08-07 21:46:11.000000 syssqlitelibV1-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 21:46:11.562563 syssqlitelibV1-1.0.0/syssqlitelibV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 21:46:11.000000 syssqlitelibV1-1.0.0/syssqlitelibV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 21:46:11.562563 syssqlitelibV1-1.0.0/syssqlitelibV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      342 2023-08-07 21:46:11.000000 syssqlitelibV1-1.0.0/syssqlitelibV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-08-07 21:46:11.000000 syssqlitelibV1-1.0.0/syssqlitelibV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 21:46:11.000000 syssqlitelibV1-1.0.0/syssqlitelibV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-08-07 21:46:11.000000 syssqlitelibV1-1.0.0/syssqlitelibV1.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 21:48:19.502089 syssqlitelibV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-08-07 21:48:19.502089 syssqlitelibV1-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 21:48:19.502089 syssqlitelibV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      555 2023-08-07 21:48:19.000000 syssqlitelibV1-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 21:48:19.502089 syssqlitelibV1-1.1.0/syssqlitelibV1/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-08-07 21:48:19.000000 syssqlitelibV1-1.1.0/syssqlitelibV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 21:48:19.502089 syssqlitelibV1-1.1.0/syssqlitelibV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-08-07 21:48:19.000000 syssqlitelibV1-1.1.0/syssqlitelibV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-08-07 21:48:19.000000 syssqlitelibV1-1.1.0/syssqlitelibV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 21:48:19.000000 syssqlitelibV1-1.1.0/syssqlitelibV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-07 21:48:19.000000 syssqlitelibV1-1.1.0/syssqlitelibV1.egg-info/top_level.txt
```

### Comparing `syssqlitelibV1-1.0.0/setup.py` & `syssqlitelibV1-1.1.0/setup.py`

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
     name="syssqlitelibV1",
     version=VERSION,
```

