# Comparing `tmp/dycodebase-0.0.4.tar.gz` & `tmp/dycodebase-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dycodebase-0.0.4.tar", last modified: Mon Aug  7 12:32:35 2023, max compression
+gzip compressed data, was "dycodebase-0.0.5.tar", last modified: Mon Aug  7 12:49:40 2023, max compression
```

## Comparing `dycodebase-0.0.4.tar` & `dycodebase-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:32:35.830650 dycodebase-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-07 12:32:35.830650 dycodebase-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 12:32:19.000000 dycodebase-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:32:35.826650 dycodebase-0.0.4/dycodebase/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 12:32:19.000000 dycodebase-0.0.4/dycodebase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:32:35.826650 dycodebase-0.0.4/dycodebase/model/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 12:32:19.000000 dycodebase-0.0.4/dycodebase/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:32:35.830650 dycodebase-0.0.4/dycodebase/model/components/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 12:32:19.000000 dycodebase-0.0.4/dycodebase/model/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-07 12:32:19.000000 dycodebase-0.0.4/dycodebase/model/components/squeeze_excite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:32:35.826650 dycodebase-0.0.4/dycodebase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-07 12:32:35.000000 dycodebase-0.0.4/dycodebase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-07 12:32:35.000000 dycodebase-0.0.4/dycodebase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:32:35.000000 dycodebase-0.0.4/dycodebase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 12:32:35.000000 dycodebase-0.0.4/dycodebase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 12:32:35.000000 dycodebase-0.0.4/dycodebase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 12:32:35.830650 dycodebase-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-07 12:32:19.000000 dycodebase-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:49:40.161742 dycodebase-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-07 12:49:40.161742 dycodebase-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 12:49:28.000000 dycodebase-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:49:40.157741 dycodebase-0.0.5/dycodebase/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 12:49:28.000000 dycodebase-0.0.5/dycodebase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:49:40.157741 dycodebase-0.0.5/dycodebase/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-07 12:49:28.000000 dycodebase-0.0.5/dycodebase/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:49:40.161742 dycodebase-0.0.5/dycodebase/model/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 12:49:28.000000 dycodebase-0.0.5/dycodebase/model/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-07 12:49:28.000000 dycodebase-0.0.5/dycodebase/model/components/squeeze_excite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:49:40.157741 dycodebase-0.0.5/dycodebase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-07 12:49:40.000000 dycodebase-0.0.5/dycodebase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-07 12:49:40.000000 dycodebase-0.0.5/dycodebase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:49:40.000000 dycodebase-0.0.5/dycodebase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 12:49:40.000000 dycodebase-0.0.5/dycodebase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 12:49:40.000000 dycodebase-0.0.5/dycodebase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 12:49:40.161742 dycodebase-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-07 12:49:28.000000 dycodebase-0.0.5/setup.py
```

### Comparing `dycodebase-0.0.4/dycodebase/model/components/squeeze_excite.py` & `dycodebase-0.0.5/dycodebase/model/components/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `dycodebase-0.0.4/setup.py` & `dycodebase-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'CodeBase of important Functions'
 LONG_DESCRIPTION = 'Contains Pytorch/ TensorFlow algorithms I have found in a single module'
 
 # Setting up
 setup(
         name="dycodebase", 
         version=VERSION,
```

