# Comparing `tmp/save-thread-result-0.1.1.post0.tar.gz` & `tmp/save-thread-result-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "save-thread-result-0.1.1.post0.tar", last modified: Wed Jun 14 19:09:57 2023, max compression
+gzip compressed data, was "save-thread-result-0.1.1.post1.tar", last modified: Mon Aug  7 18:23:03 2023, max compression
```

## Comparing `save-thread-result-0.1.1.post0.tar` & `save-thread-result-0.1.1.post1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-06-14 19:09:57.065144 save-thread-result-0.1.1.post0/
--rw-r--r--   0 shail      (503) staff       (20)    19275 2023-06-14 19:09:57.064550 save-thread-result-0.1.1.post0/PKG-INFO
--rw-r--r--   0 shail      (503) staff       (20)     3981 2023-05-29 23:34:08.000000 save-thread-result-0.1.1.post0/README.md
-drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-06-14 19:09:57.060766 save-thread-result-0.1.1.post0/save_thread_result/
--rw-r--r--   0 shail      (503) staff       (20)    17141 2023-06-14 19:05:43.000000 save-thread-result-0.1.1.post0/save_thread_result/__init__.py
-drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-06-14 19:09:57.063642 save-thread-result-0.1.1.post0/save_thread_result.egg-info/
--rw-r--r--   0 shail      (503) staff       (20)    19275 2023-06-14 19:09:57.000000 save-thread-result-0.1.1.post0/save_thread_result.egg-info/PKG-INFO
--rw-r--r--   0 shail      (503) staff       (20)      217 2023-06-14 19:09:57.000000 save-thread-result-0.1.1.post0/save_thread_result.egg-info/SOURCES.txt
--rw-r--r--   0 shail      (503) staff       (20)        1 2023-06-14 19:09:57.000000 save-thread-result-0.1.1.post0/save_thread_result.egg-info/dependency_links.txt
--rw-r--r--   0 shail      (503) staff       (20)       19 2023-06-14 19:09:57.000000 save-thread-result-0.1.1.post0/save_thread_result.egg-info/top_level.txt
--rw-r--r--   0 shail      (503) staff       (20)       38 2023-06-14 19:09:57.065366 save-thread-result-0.1.1.post0/setup.cfg
--rw-r--r--   0 shail      (503) staff       (20)    19297 2023-06-14 19:05:43.000000 save-thread-result-0.1.1.post0/setup.py
+drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-08-07 18:23:03.470476 save-thread-result-0.1.1.post1/
+-rw-r--r--   0 shail      (503) staff       (20)    19274 2023-08-07 18:23:03.469875 save-thread-result-0.1.1.post1/PKG-INFO
+-rw-r--r--   0 shail      (503) staff       (20)     3981 2023-06-16 21:10:10.000000 save-thread-result-0.1.1.post1/README.md
+drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-08-07 18:23:03.466732 save-thread-result-0.1.1.post1/save_thread_result/
+-rw-r--r--   0 shail      (503) staff       (20)    17141 2023-08-07 17:43:00.000000 save-thread-result-0.1.1.post1/save_thread_result/__init__.py
+drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-08-07 18:23:03.468927 save-thread-result-0.1.1.post1/save_thread_result.egg-info/
+-rw-r--r--   0 shail      (503) staff       (20)    19274 2023-08-07 18:23:03.000000 save-thread-result-0.1.1.post1/save_thread_result.egg-info/PKG-INFO
+-rw-r--r--   0 shail      (503) staff       (20)      217 2023-08-07 18:23:03.000000 save-thread-result-0.1.1.post1/save_thread_result.egg-info/SOURCES.txt
+-rw-r--r--   0 shail      (503) staff       (20)        1 2023-08-07 18:23:03.000000 save-thread-result-0.1.1.post1/save_thread_result.egg-info/dependency_links.txt
+-rw-r--r--   0 shail      (503) staff       (20)       19 2023-08-07 18:23:03.000000 save-thread-result-0.1.1.post1/save_thread_result.egg-info/top_level.txt
+-rw-r--r--   0 shail      (503) staff       (20)       38 2023-08-07 18:23:03.470634 save-thread-result-0.1.1.post1/setup.cfg
+-rw-r--r--   0 shail      (503) staff       (20)    19296 2023-08-07 17:43:00.000000 save-thread-result-0.1.1.post1/setup.py
```

### Comparing `save-thread-result-0.1.1.post0/PKG-INFO` & `save-thread-result-0.1.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: save-thread-result
-Version: 0.1.1.post0
+Version: 0.1.1.post1
 Summary: Simple subclass wrapper around `threading.Thread` to get the return value from a thread in python. Exact same interface as `threading.Thread`! 🌟 Star this repo if you found it useful! 🌟
 Home-page: https://github.com/slow-but-steady/save-thread-result/tree/main/python
 Author: slow-but-steady
 Author-email: slowbutsteady1234@gmail.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/slow-but-steady/save-thread-result/issues
 Project-URL: PyPi Funding, https://donate.pypi.org
@@ -275,15 +275,15 @@
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
-Requires-Python: >3.0, <4
+Requires-Python: >=3, <4
 Description-Content-Type: text/markdown
 
 # Python API
 
 ## Quickstart
 
 Installing the `save_thread_result` module:
```

### Comparing `save-thread-result-0.1.1.post0/README.md` & `save-thread-result-0.1.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `save-thread-result-0.1.1.post0/save_thread_result/__init__.py` & `save-thread-result-0.1.1.post1/save_thread_result/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 import sys
 import time
 import threading
 from datetime import datetime
 
 
-__version__              = '0.1.1.post0'
+__version__              = '0.1.1.post1'
 
 
 _general_documentation = '''
     The `threading.Thread` subclass `ThreadWithResult` saves the result of a thread
     as its `result` attribute - i.e. call `thread_with_result_instance_1.result`
     after `thread_with_result_instance_1` finishes running to get the return
     value from the function that ran on that thread:
```

### Comparing `save-thread-result-0.1.1.post0/save_thread_result.egg-info/PKG-INFO` & `save-thread-result-0.1.1.post1/save_thread_result.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: save-thread-result
-Version: 0.1.1.post0
+Version: 0.1.1.post1
 Summary: Simple subclass wrapper around `threading.Thread` to get the return value from a thread in python. Exact same interface as `threading.Thread`! 🌟 Star this repo if you found it useful! 🌟
 Home-page: https://github.com/slow-but-steady/save-thread-result/tree/main/python
 Author: slow-but-steady
 Author-email: slowbutsteady1234@gmail.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/slow-but-steady/save-thread-result/issues
 Project-URL: PyPi Funding, https://donate.pypi.org
@@ -275,15 +275,15 @@
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
-Requires-Python: >3.0, <4
+Requires-Python: >=3, <4
 Description-Content-Type: text/markdown
 
 # Python API
 
 ## Quickstart
 
 Installing the `save_thread_result` module:
```

### Comparing `save-thread-result-0.1.1.post0/setup.py` & `save-thread-result-0.1.1.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # For new projects, the recommended versioning scheme is based on Semantic Versioning, but adopts a different approach to handling pre-releases and build metadata.
     # The essence of semantic versioning is a 3-part MAJOR.MINOR.MAINTENANCE numbering scheme, where the project author increments:
     # 1. MAJOR version when they make incompatible API changes,
     # 2. MINOR version when they add functionality in a backwards-compatible manner, and
     # 3. MAINTENANCE version when they make backwards-compatible bug fixes.
     # Adopting this approach as a project author allows users to make use of “compatible release” specifiers, where name ~= X.Y requires at least release X.Y, but also allows any later release with a matching MAJOR version.
     # Python projects adopting semantic versioning should abide by clauses 1-8 of the Semantic Versioning 2.0.0 specification: https://semver.org/.
-    version                       = '0.1.1.post0',
+    version                       = '0.1.1.post1',
     name                          = 'save-thread-result',
     description                   = 'Simple subclass wrapper around `threading.Thread` to get the return value from a thread in python. Exact same interface as `threading.Thread`! 🌟 Star this repo if you found it useful! 🌟',
     long_description              = long_description,
     long_description_content_type = 'text/markdown',
     url                           = 'https://github.com/slow-but-steady/save-thread-result/tree/main/python',
     author                        = 'slow-but-steady',
     author_email                  = 'slowbutsteady1234@gmail.com',
@@ -315,15 +315,15 @@
     # http://code.nabla.net/doc/setuptools/api/setuptools/setuptools.find_packages.html
     # https://stackoverflow.com/questions/51286928/what-is-where-argument-for-in-setuptools-find-packages
     packages=find_packages(exclude=['*dev*']),
     # packages=find_namespace_packages(include=['ship']),
     # package_dir={'':'src'},
 
 
-    python_requires  = '>3.0, <4',
+    python_requires  = '>=3, <4',
     install_requires = [],  # Optional
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
 
 
     # If there are data files included in your packages that need to be installed, specify them here.
     # If using Python 2.6 or earlier, then these have to be included in MANIFEST.in as well.
     package_data = {  # Optional
```

