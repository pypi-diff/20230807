# Comparing `tmp/pipfontingpkg-1.0.0.tar.gz` & `tmp/pipfontingpkg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipfontingpkg-1.0.0.tar", last modified: Mon Aug  7 02:37:03 2023, max compression
+gzip compressed data, was "pipfontingpkg-1.1.0.tar", last modified: Mon Aug  7 02:39:09 2023, max compression
```

## Comparing `pipfontingpkg-1.0.0.tar` & `pipfontingpkg-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 02:37:03.820564 pipfontingpkg-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      341 2023-08-07 02:37:03.820564 pipfontingpkg-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 02:37:03.820564 pipfontingpkg-1.0.0/pipfontingpkg/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 02:37:03.000000 pipfontingpkg-1.0.0/pipfontingpkg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 02:37:03.820564 pipfontingpkg-1.0.0/pipfontingpkg.egg-info/
--rw-r--r--   0 root         (0) root         (0)      341 2023-08-07 02:37:03.000000 pipfontingpkg-1.0.0/pipfontingpkg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2023-08-07 02:37:03.000000 pipfontingpkg-1.0.0/pipfontingpkg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 02:37:03.000000 pipfontingpkg-1.0.0/pipfontingpkg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-08-07 02:37:03.000000 pipfontingpkg-1.0.0/pipfontingpkg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 02:37:03.820564 pipfontingpkg-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      554 2023-08-07 02:37:03.000000 pipfontingpkg-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 02:39:09.243909 pipfontingpkg-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-08-07 02:39:09.243909 pipfontingpkg-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 02:39:09.243909 pipfontingpkg-1.1.0/pipfontingpkg/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-08-07 02:39:08.000000 pipfontingpkg-1.1.0/pipfontingpkg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 02:39:09.243909 pipfontingpkg-1.1.0/pipfontingpkg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-08-07 02:39:09.000000 pipfontingpkg-1.1.0/pipfontingpkg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2023-08-07 02:39:09.000000 pipfontingpkg-1.1.0/pipfontingpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 02:39:09.000000 pipfontingpkg-1.1.0/pipfontingpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-08-07 02:39:09.000000 pipfontingpkg-1.1.0/pipfontingpkg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 02:39:09.243909 pipfontingpkg-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      554 2023-08-07 02:39:08.000000 pipfontingpkg-1.1.0/setup.py
```

### Comparing `pipfontingpkg-1.0.0/setup.py` & `pipfontingpkg-1.1.0/setup.py`

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
     name="pipfontingpkg",
     version=VERSION,
```

