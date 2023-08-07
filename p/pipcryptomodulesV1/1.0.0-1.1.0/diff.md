# Comparing `tmp/pipcryptomodulesV1-1.0.0.tar.gz` & `tmp/pipcryptomodulesV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcryptomodulesV1-1.0.0.tar", last modified: Mon Aug  7 01:07:13 2023, max compression
+gzip compressed data, was "pipcryptomodulesV1-1.1.0.tar", last modified: Mon Aug  7 01:09:18 2023, max compression
```

## Comparing `pipcryptomodulesV1-1.0.0.tar` & `pipcryptomodulesV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:07:13.840786 pipcryptomodulesV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      346 2023-08-07 01:07:13.840786 pipcryptomodulesV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:07:13.840786 pipcryptomodulesV1-1.0.0/pipcryptomodulesV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 01:07:13.000000 pipcryptomodulesV1-1.0.0/pipcryptomodulesV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:07:13.840786 pipcryptomodulesV1-1.0.0/pipcryptomodulesV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      346 2023-08-07 01:07:13.000000 pipcryptomodulesV1-1.0.0/pipcryptomodulesV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-08-07 01:07:13.000000 pipcryptomodulesV1-1.0.0/pipcryptomodulesV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 01:07:13.000000 pipcryptomodulesV1-1.0.0/pipcryptomodulesV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-08-07 01:07:13.000000 pipcryptomodulesV1-1.0.0/pipcryptomodulesV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 01:07:13.840786 pipcryptomodulesV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      559 2023-08-07 01:07:13.000000 pipcryptomodulesV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:09:18.184351 pipcryptomodulesV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-08-07 01:09:18.184351 pipcryptomodulesV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:09:18.184351 pipcryptomodulesV1-1.1.0/pipcryptomodulesV1/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-08-07 01:09:17.000000 pipcryptomodulesV1-1.1.0/pipcryptomodulesV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:09:18.184351 pipcryptomodulesV1-1.1.0/pipcryptomodulesV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-08-07 01:09:18.000000 pipcryptomodulesV1-1.1.0/pipcryptomodulesV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-08-07 01:09:18.000000 pipcryptomodulesV1-1.1.0/pipcryptomodulesV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 01:09:18.000000 pipcryptomodulesV1-1.1.0/pipcryptomodulesV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-07 01:09:18.000000 pipcryptomodulesV1-1.1.0/pipcryptomodulesV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 01:09:18.184351 pipcryptomodulesV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      559 2023-08-07 01:09:17.000000 pipcryptomodulesV1-1.1.0/setup.py
```

### Comparing `pipcryptomodulesV1-1.0.0/setup.py` & `pipcryptomodulesV1-1.1.0/setup.py`

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
     name="pipcryptomodulesV1",
     version=VERSION,
```

