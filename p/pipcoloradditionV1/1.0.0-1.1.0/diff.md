# Comparing `tmp/pipcoloradditionV1-1.0.0.tar.gz` & `tmp/pipcoloradditionV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcoloradditionV1-1.0.0.tar", last modified: Sun Aug  6 22:09:44 2023, max compression
+gzip compressed data, was "pipcoloradditionV1-1.1.0.tar", last modified: Sun Aug  6 22:11:49 2023, max compression
```

## Comparing `pipcoloradditionV1-1.0.0.tar` & `pipcoloradditionV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:09:44.260008 pipcoloradditionV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      346 2023-08-06 22:09:44.260008 pipcoloradditionV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:09:44.256008 pipcoloradditionV1-1.0.0/pipcoloradditionV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-06 22:09:43.000000 pipcoloradditionV1-1.0.0/pipcoloradditionV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:09:44.260008 pipcoloradditionV1-1.0.0/pipcoloradditionV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      346 2023-08-06 22:09:44.000000 pipcoloradditionV1-1.0.0/pipcoloradditionV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-08-06 22:09:44.000000 pipcoloradditionV1-1.0.0/pipcoloradditionV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 22:09:44.000000 pipcoloradditionV1-1.0.0/pipcoloradditionV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-08-06 22:09:44.000000 pipcoloradditionV1-1.0.0/pipcoloradditionV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 22:09:44.260008 pipcoloradditionV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      559 2023-08-06 22:09:43.000000 pipcoloradditionV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:11:49.739529 pipcoloradditionV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-08-06 22:11:49.739529 pipcoloradditionV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:11:49.735529 pipcoloradditionV1-1.1.0/pipcoloradditionV1/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-08-06 22:11:49.000000 pipcoloradditionV1-1.1.0/pipcoloradditionV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 22:11:49.735529 pipcoloradditionV1-1.1.0/pipcoloradditionV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-08-06 22:11:49.000000 pipcoloradditionV1-1.1.0/pipcoloradditionV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-08-06 22:11:49.000000 pipcoloradditionV1-1.1.0/pipcoloradditionV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 22:11:49.000000 pipcoloradditionV1-1.1.0/pipcoloradditionV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-06 22:11:49.000000 pipcoloradditionV1-1.1.0/pipcoloradditionV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 22:11:49.739529 pipcoloradditionV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      559 2023-08-06 22:11:49.000000 pipcoloradditionV1-1.1.0/setup.py
```

### Comparing `pipcoloradditionV1-1.0.0/setup.py` & `pipcoloradditionV1-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull tweak package"
 LONG_DESCRIPTION = "Usefull tweak package"
 
 # Setting up
 setup(
     name="pipcoloradditionV1",
     version=VERSION,
```

