# Comparing `tmp/fracsuite-0.1.2.tar.gz` & `tmp/fracsuite-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fracsuite-0.1.2.tar", last modified: Sun Aug  6 21:36:13 2023, max compression
+gzip compressed data, was "fracsuite-0.1.3.tar", last modified: Sun Aug  6 21:47:56 2023, max compression
```

## Comparing `fracsuite-0.1.2.tar` & `fracsuite-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:36:13.439169 fracsuite-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-06 21:36:13.439169 fracsuite-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-06 21:36:03.000000 fracsuite-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:36:13.439169 fracsuite-0.1.2/fracsuite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 21:36:03.000000 fracsuite-0.1.2/fracsuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-06 21:36:03.000000 fracsuite-0.1.2/fracsuite/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-08-06 21:36:03.000000 fracsuite-0.1.2/fracsuite/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-06 21:36:03.000000 fracsuite-0.1.2/fracsuite/splinter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:36:13.439169 fracsuite-0.1.2/fracsuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-06 21:36:13.000000 fracsuite-0.1.2/fracsuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-06 21:36:13.000000 fracsuite-0.1.2/fracsuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 21:36:13.000000 fracsuite-0.1.2/fracsuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 21:36:13.000000 fracsuite-0.1.2/fracsuite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 21:36:13.000000 fracsuite-0.1.2/fracsuite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-06 21:36:03.000000 fracsuite-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 21:36:13.439169 fracsuite-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:47:56.339513 fracsuite-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-06 21:47:56.335513 fracsuite-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-06 21:47:46.000000 fracsuite-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:47:56.335513 fracsuite-0.1.3/fracsuite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 21:47:46.000000 fracsuite-0.1.3/fracsuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-06 21:47:46.000000 fracsuite-0.1.3/fracsuite/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-08-06 21:47:46.000000 fracsuite-0.1.3/fracsuite/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-06 21:47:46.000000 fracsuite-0.1.3/fracsuite/splinter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:47:56.335513 fracsuite-0.1.3/fracsuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-06 21:47:56.000000 fracsuite-0.1.3/fracsuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-06 21:47:56.000000 fracsuite-0.1.3/fracsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 21:47:56.000000 fracsuite-0.1.3/fracsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 21:47:56.000000 fracsuite-0.1.3/fracsuite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 21:47:56.000000 fracsuite-0.1.3/fracsuite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-06 21:47:46.000000 fracsuite-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 21:47:56.339513 fracsuite-0.1.3/setup.cfg
```

### Comparing `fracsuite-0.1.2/fracsuite/analyzer.py` & `fracsuite-0.1.3/fracsuite/analyzer.py`

 * *Files identical despite different names*

### Comparing `fracsuite-0.1.2/fracsuite/splinter.py` & `fracsuite-0.1.3/fracsuite/splinter.py`

 * *Files identical despite different names*

### Comparing `fracsuite-0.1.2/pyproject.toml` & `fracsuite-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = ["matplotlib", "opencv-python", "numpy", "tqdm", "scikit-image"]
 name = "fracsuite"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Leon Bohmann", email="mail@leonbohmann.de" },
 ]
 description = "Package to help analyze fracture patterns on broken glass plys."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

