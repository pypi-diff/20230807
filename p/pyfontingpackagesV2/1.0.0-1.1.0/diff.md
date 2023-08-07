# Comparing `tmp/pyfontingpackagesV2-1.0.0.tar.gz` & `tmp/pyfontingpackagesV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfontingpackagesV2-1.0.0.tar", last modified: Mon Aug  7 01:24:38 2023, max compression
+gzip compressed data, was "pyfontingpackagesV2-1.1.0.tar", last modified: Mon Aug  7 01:26:43 2023, max compression
```

## Comparing `pyfontingpackagesV2-1.0.0.tar` & `pyfontingpackagesV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:24:38.881037 pyfontingpackagesV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-08-07 01:24:38.881037 pyfontingpackagesV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:24:38.877037 pyfontingpackagesV2-1.0.0/pyfontingpackagesV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 01:24:38.000000 pyfontingpackagesV2-1.0.0/pyfontingpackagesV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:24:38.877037 pyfontingpackagesV2-1.0.0/pyfontingpackagesV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-08-07 01:24:38.000000 pyfontingpackagesV2-1.0.0/pyfontingpackagesV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2023-08-07 01:24:38.000000 pyfontingpackagesV2-1.0.0/pyfontingpackagesV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 01:24:38.000000 pyfontingpackagesV2-1.0.0/pyfontingpackagesV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-08-07 01:24:38.000000 pyfontingpackagesV2-1.0.0/pyfontingpackagesV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 01:24:38.881037 pyfontingpackagesV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-08-07 01:24:38.000000 pyfontingpackagesV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:26:43.628358 pyfontingpackagesV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-08-07 01:26:43.628358 pyfontingpackagesV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:26:43.628358 pyfontingpackagesV2-1.1.0/pyfontingpackagesV2/
+-rw-r--r--   0 root         (0) root         (0)    96635 2023-08-07 01:26:43.000000 pyfontingpackagesV2-1.1.0/pyfontingpackagesV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 01:26:43.628358 pyfontingpackagesV2-1.1.0/pyfontingpackagesV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-08-07 01:26:43.000000 pyfontingpackagesV2-1.1.0/pyfontingpackagesV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-08-07 01:26:43.000000 pyfontingpackagesV2-1.1.0/pyfontingpackagesV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 01:26:43.000000 pyfontingpackagesV2-1.1.0/pyfontingpackagesV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-07 01:26:43.000000 pyfontingpackagesV2-1.1.0/pyfontingpackagesV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 01:26:43.628358 pyfontingpackagesV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-08-07 01:26:43.000000 pyfontingpackagesV2-1.1.0/setup.py
```

### Comparing `pyfontingpackagesV2-1.0.0/setup.py` & `pyfontingpackagesV2-1.1.0/setup.py`

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
     name="pyfontingpackagesV2",
     version=VERSION,
```

