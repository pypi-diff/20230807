# Comparing `tmp/pysqlitepkgV2-1.0.0.tar.gz` & `tmp/pysqlitepkgV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqlitepkgV2-1.0.0.tar", last modified: Sun Aug  6 22:37:50 2023, max compression
+gzip compressed data, was "pysqlitepkgV2-1.1.0.tar", last modified: Sun Aug  6 22:39:56 2023, max compression
```

## Comparing `pysqlitepkgV2-1.0.0.tar` & `pysqlitepkgV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:37:50.510752 pysqlitepkgV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      341 2023-08-06 22:37:50.510752 pysqlitepkgV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:37:50.510752 pysqlitepkgV2-1.0.0/pysqlitepkgV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-06 22:37:49.000000 pysqlitepkgV2-1.0.0/pysqlitepkgV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:37:50.510752 pysqlitepkgV2-1.0.0/pysqlitepkgV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      341 2023-08-06 22:37:50.000000 pysqlitepkgV2-1.0.0/pysqlitepkgV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2023-08-06 22:37:50.000000 pysqlitepkgV2-1.0.0/pysqlitepkgV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 22:37:50.000000 pysqlitepkgV2-1.0.0/pysqlitepkgV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-08-06 22:37:50.000000 pysqlitepkgV2-1.0.0/pysqlitepkgV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 22:37:50.510752 pysqlitepkgV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      554 2023-08-06 22:37:49.000000 pysqlitepkgV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:39:56.210663 pysqlitepkgV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-08-06 22:39:56.210663 pysqlitepkgV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:39:56.206663 pysqlitepkgV2-1.1.0/pysqlitepkgV2/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-08-06 22:39:55.000000 pysqlitepkgV2-1.1.0/pysqlitepkgV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:39:56.210663 pysqlitepkgV2-1.1.0/pysqlitepkgV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-08-06 22:39:56.000000 pysqlitepkgV2-1.1.0/pysqlitepkgV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2023-08-06 22:39:56.000000 pysqlitepkgV2-1.1.0/pysqlitepkgV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 22:39:56.000000 pysqlitepkgV2-1.1.0/pysqlitepkgV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-08-06 22:39:56.000000 pysqlitepkgV2-1.1.0/pysqlitepkgV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 22:39:56.210663 pysqlitepkgV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      554 2023-08-06 22:39:55.000000 pysqlitepkgV2-1.1.0/setup.py
```

### Comparing `pysqlitepkgV2-1.0.0/setup.py` & `pysqlitepkgV2-1.1.0/setup.py`

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
     name="pysqlitepkgV2",
     version=VERSION,
```

