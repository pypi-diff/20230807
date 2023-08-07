# Comparing `tmp/trove-classifiers-2023.7.6.tar.gz` & `tmp/trove-classifiers-2023.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trove-classifiers-2023.7.6.tar", last modified: Thu Jul  6 14:42:43 2023, max compression
+gzip compressed data, was "trove-classifiers-2023.8.7.tar", last modified: Mon Aug  7 19:52:03 2023, max compression
```

## Comparing `trove-classifiers-2023.7.6.tar` & `trove-classifiers-2023.8.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:42:43.275078 trove-classifiers-2023.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-06 14:42:43.275078 trove-classifiers-2023.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:42:43.271078 trove-classifiers-2023.7.6/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/bin/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:42:43.271078 trove-classifiers-2023.7.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 14:42:43.275078 trove-classifiers-2023.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:42:43.271078 trove-classifiers-2023.7.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:42:43.271078 trove-classifiers-2023.7.6/src/trove_classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)    40140 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/src/trove_classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/src/trove_classifiers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/src/trove_classifiers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:42:43.275078 trove-classifiers-2023.7.6/src/trove_classifiers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-06 14:42:43.000000 trove-classifiers-2023.7.6/src/trove_classifiers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-06 14:42:43.000000 trove-classifiers-2023.7.6/src/trove_classifiers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:42:43.000000 trove-classifiers-2023.7.6/src/trove_classifiers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 14:42:43.000000 trove-classifiers-2023.7.6/src/trove_classifiers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:42:43.275078 trove-classifiers-2023.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:42:43.275078 trove-classifiers-2023.7.6/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/tests/lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-06 14:42:15.000000 trove-classifiers-2023.7.6/tests/test_classifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:52:03.145185 trove-classifiers-2023.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-08-07 19:52:03.145185 trove-classifiers-2023.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:52:03.141185 trove-classifiers-2023.8.7/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/bin/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:52:03.141185 trove-classifiers-2023.8.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:52:03.145185 trove-classifiers-2023.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:52:03.141185 trove-classifiers-2023.8.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:52:03.145185 trove-classifiers-2023.8.7/src/trove_classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)    40186 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/src/trove_classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/src/trove_classifiers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/src/trove_classifiers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:52:03.145185 trove-classifiers-2023.8.7/src/trove_classifiers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-08-07 19:52:03.000000 trove-classifiers-2023.8.7/src/trove_classifiers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-07 19:52:03.000000 trove-classifiers-2023.8.7/src/trove_classifiers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:52:03.000000 trove-classifiers-2023.8.7/src/trove_classifiers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 19:52:03.000000 trove-classifiers-2023.8.7/src/trove_classifiers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:52:03.145185 trove-classifiers-2023.8.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:52:03.145185 trove-classifiers-2023.8.7/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/tests/lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-08-07 19:51:28.000000 trove-classifiers-2023.8.7/tests/test_classifiers.py
```

### Comparing `trove-classifiers-2023.7.6/CONTRIBUTING.md` & `trove-classifiers-2023.8.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.7.6/LICENSE` & `trove-classifiers-2023.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.7.6/Makefile` & `trove-classifiers-2023.8.7/Makefile`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.7.6/PKG-INFO` & `trove-classifiers-2023.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2023.7.6
+Version: 2023.8.7
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2023.7.6/README.md` & `trove-classifiers-2023.8.7/README.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.7.6/bin/sort.py` & `trove-classifiers-2023.8.7/bin/sort.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.7.6/setup.py` & `trove-classifiers-2023.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.7.6/src/trove_classifiers/__init__.py` & `trove-classifiers-2023.8.7/src/trove_classifiers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,14 +491,15 @@
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Programming Language :: Python :: Implementation",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: IronPython",
     "Programming Language :: Python :: Implementation :: Jython",
     "Programming Language :: Python :: Implementation :: MicroPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: Implementation :: Stackless",
```

### Comparing `trove-classifiers-2023.7.6/src/trove_classifiers.egg-info/PKG-INFO` & `trove-classifiers-2023.8.7/src/trove_classifiers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2023.7.6
+Version: 2023.8.7
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2023.7.6/tests/lib/__init__.py` & `trove-classifiers-2023.8.7/tests/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2023.7.6/tests/test_classifiers.py` & `trove-classifiers-2023.8.7/tests/test_classifiers.py`

 * *Files identical despite different names*

