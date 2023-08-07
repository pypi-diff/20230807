# Comparing `tmp/psl-2023.7.31.tar.gz` & `tmp/psl-2023.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2023.7.31.tar", last modified: Mon Jul 31 13:06:52 2023, max compression
+gzip compressed data, was "psl-2023.8.7.tar", last modified: Mon Aug  7 13:05:53 2023, max compression
```

## Comparing `psl-2023.7.31.tar` & `psl-2023.8.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:06:52.813912 psl-2023.7.31/
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-31 13:06:20.000000 psl-2023.7.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 13:06:20.000000 psl-2023.7.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-31 13:06:52.813912 psl-2023.7.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-31 13:06:20.000000 psl-2023.7.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:06:52.809912 psl-2023.7.31/psl/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-07-31 13:06:27.000000 psl-2023.7.31/psl/__init__.py
--rw-------   0 runner    (1001) docker     (123)   110946 2023-07-31 13:06:27.000000 psl-2023.7.31/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:06:20.000000 psl-2023.7.31/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:06:52.813912 psl-2023.7.31/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-31 13:06:52.000000 psl-2023.7.31/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-31 13:06:52.000000 psl-2023.7.31/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:06:52.000000 psl-2023.7.31/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:06:40.000000 psl-2023.7.31/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-31 13:06:52.000000 psl-2023.7.31/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:06:52.813912 psl-2023.7.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-31 13:06:20.000000 psl-2023.7.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:53.420557 psl-2023.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-08-07 13:05:13.000000 psl-2023.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-07 13:05:13.000000 psl-2023.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-07 13:05:53.420557 psl-2023.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-07 13:05:13.000000 psl-2023.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:53.416556 psl-2023.8.7/psl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-08-07 13:05:24.000000 psl-2023.8.7/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (123)   110939 2023-08-07 13:05:24.000000 psl-2023.8.7/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:13.000000 psl-2023.8.7/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:05:53.420557 psl-2023.8.7/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-07 13:05:53.000000 psl-2023.8.7/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-07 13:05:53.000000 psl-2023.8.7/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:05:53.000000 psl-2023.8.7/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:05:39.000000 psl-2023.8.7/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-07 13:05:53.000000 psl-2023.8.7/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:05:53.420557 psl-2023.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-07 13:05:13.000000 psl-2023.8.7/setup.py
```

### Comparing `psl-2023.7.31/LICENSE` & `psl-2023.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2023.7.31/PKG-INFO` & `psl-2023.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.7.31
+Version: 2023.8.7
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.7.31/README.md` & `psl-2023.8.7/README.md`

 * *Files identical despite different names*

### Comparing `psl-2023.7.31/psl/__init__.py` & `psl-2023.8.7/psl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2023.7.31"
-__checksum__ = "651ed65f9f69cc54e7057ce04a1700a2de89d5cf"
+__version__ = "2023.8.7"
+__checksum__ = "f81cd112a0542c603f81e3e7e38c38e581ea9c57"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2023.7.31/psl/psl.txt` & `psl-2023.8.7/psl/psl.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6391,15 +6391,14 @@
 motorcycles
 mov
 movie
 msd
 mtn
 mtr
 music
-mutual
 nab
 nagoya
 natura
 navy
 nba
 nec
 netbank
```

### Comparing `psl-2023.7.31/psl.egg-info/PKG-INFO` & `psl-2023.8.7/psl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.7.31
+Version: 2023.8.7
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.7.31/setup.py` & `psl-2023.8.7/setup.py`

 * *Files identical despite different names*

