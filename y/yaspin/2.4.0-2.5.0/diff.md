# Comparing `tmp/yaspin-2.4.0.tar.gz` & `tmp/yaspin-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaspin-2.4.0.tar", max compression
+gzip compressed data, was "yaspin-2.5.0.tar", max compression
```

## Comparing `yaspin-2.4.0.tar` & `yaspin-2.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     5419 2023-08-06 12:43:09.749394 yaspin-2.4.0/HISTORY.rst
--rw-r--r--   0        0        0     1072 2022-07-11 11:51:22.114125 yaspin-2.4.0/LICENSE
--rw-r--r--   0        0        0    11970 2023-08-06 12:43:09.749394 yaspin-2.4.0/README.rst
--rw-r--r--   0        0        0      909 2023-01-06 13:49:42.862298 yaspin-2.4.0/examples/advanced_colors.py
--rw-r--r--   0        0        0     1089 2023-08-06 12:02:54.701543 yaspin-2.4.0/examples/basic_usage.py
--rw-r--r--   0        0        0      493 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/cli_spinners.py
--rw-r--r--   0        0        0     1577 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/colors.py
--rw-r--r--   0        0        0     4879 2023-01-06 14:18:08.246403 yaspin-2.4.0/examples/demo.py
--rw-r--r--   0        0        0      552 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/dynamic_text.py
--rw-r--r--   0        0        0      699 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/finalizers.py
--rw-r--r--   0        0        0      621 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/hide_show.py
--rw-r--r--   0        0        0     1532 2023-02-26 15:11:07.363981 yaspin-2.4.0/examples/hide_show_prompt_toolkit.py
--rw-r--r--   0        0        0      481 2023-02-26 15:11:07.363981 yaspin-2.4.0/examples/reverse_spinner.py
--rw-r--r--   0        0        0      415 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/right_spinner.py
--rw-r--r--   0        0        0     4030 2023-08-06 12:02:54.702543 yaspin-2.4.0/examples/signals.py
--rw-r--r--   0        0        0      854 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/spinner_properties.py
--rw-r--r--   0        0        0      359 2022-07-19 11:35:29.002311 yaspin-2.4.0/examples/timer_spinner.py
--rw-r--r--   0        0        0      452 2022-07-11 11:51:22.116125 yaspin-2.4.0/examples/write_method.py
--rw-r--r--   0        0        0     2455 2023-08-06 12:43:09.750394 yaspin-2.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-07-11 11:51:22.128125 yaspin-2.4.0/tests/__init__.py
--rw-r--r--   0        0        0     7252 2023-08-06 12:43:09.750394 yaspin-2.4.0/tests/conftest.py
--rw-r--r--   0        0        0     3025 2022-07-19 10:41:34.977459 yaspin-2.4.0/tests/test_attrs.py
--rw-r--r--   0        0        0      730 2022-07-11 11:51:22.128125 yaspin-2.4.0/tests/test_finalizers.py
--rw-r--r--   0        0        0     7813 2023-02-26 15:11:07.365981 yaspin-2.4.0/tests/test_in_out.py
--rw-r--r--   0        0        0     1507 2023-08-06 12:02:54.704543 yaspin-2.4.0/tests/test_pipes.py
--rw-r--r--   0        0        0     3479 2023-08-06 12:02:54.704543 yaspin-2.4.0/tests/test_properties.py
--rw-r--r--   0        0        0     2167 2022-07-19 10:41:34.979459 yaspin-2.4.0/tests/test_signals.py
--rw-r--r--   0        0        0      695 2022-07-11 11:51:22.128125 yaspin-2.4.0/tests/test_spinners.py
--rw-r--r--   0        0        0     1373 2022-07-11 11:51:22.128125 yaspin-2.4.0/tests/test_timer.py
--rw-r--r--   0        0        0     1217 2023-08-06 12:02:54.704543 yaspin-2.4.0/tests/test_yaspin.py
--rw-r--r--   0        0        0      218 2023-08-06 12:02:54.704543 yaspin-2.4.0/yaspin/__init__.py
--rw-r--r--   0        0        0     2600 2023-08-06 12:02:54.704543 yaspin-2.4.0/yaspin/api.py
--rw-r--r--   0        0        0      351 2023-08-06 12:02:54.704543 yaspin-2.4.0/yaspin/base_spinner.py
--rw-r--r--   0        0        0     2749 2023-08-06 12:43:09.751394 yaspin-2.4.0/yaspin/constants.py
--rw-r--r--   0        0        0    17974 2023-08-06 12:02:54.705543 yaspin-2.4.0/yaspin/core.py
--rw-r--r--   0        0        0    26255 2023-08-06 12:43:09.751394 yaspin-2.4.0/yaspin/data/spinners.json
--rw-r--r--   0        0        0      329 2023-08-06 12:02:54.705543 yaspin-2.4.0/yaspin/helpers.py
--rw-r--r--   0        0        0     1065 2023-08-06 12:02:54.705543 yaspin-2.4.0/yaspin/signal_handlers.py
--rw-r--r--   0        0        0      505 2023-08-06 12:02:54.705543 yaspin-2.4.0/yaspin/spinners.py
--rw-r--r--   0        0        0    14175 1970-01-01 00:00:00.000000 yaspin-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     5508 2023-08-07 16:04:19.180885 yaspin-2.5.0/HISTORY.rst
+-rw-r--r--   0        0        0     1072 2022-07-11 11:51:22.114125 yaspin-2.5.0/LICENSE
+-rw-r--r--   0        0        0    11963 2023-08-07 16:04:19.180885 yaspin-2.5.0/README.rst
+-rw-r--r--   0        0        0      909 2023-01-06 13:49:42.862298 yaspin-2.5.0/examples/advanced_colors.py
+-rw-r--r--   0        0        0     1089 2023-08-06 12:02:54.701543 yaspin-2.5.0/examples/basic_usage.py
+-rw-r--r--   0        0        0      493 2022-07-11 11:51:22.115125 yaspin-2.5.0/examples/cli_spinners.py
+-rw-r--r--   0        0        0     1577 2022-07-11 11:51:22.115125 yaspin-2.5.0/examples/colors.py
+-rw-r--r--   0        0        0     4879 2023-01-06 14:18:08.246403 yaspin-2.5.0/examples/demo.py
+-rw-r--r--   0        0        0      552 2022-07-11 11:51:22.115125 yaspin-2.5.0/examples/dynamic_text.py
+-rw-r--r--   0        0        0      699 2022-07-11 11:51:22.115125 yaspin-2.5.0/examples/finalizers.py
+-rw-r--r--   0        0        0      621 2022-07-11 11:51:22.115125 yaspin-2.5.0/examples/hide_show.py
+-rw-r--r--   0        0        0     1532 2023-02-26 15:11:07.363981 yaspin-2.5.0/examples/hide_show_prompt_toolkit.py
+-rw-r--r--   0        0        0      481 2023-02-26 15:11:07.363981 yaspin-2.5.0/examples/reverse_spinner.py
+-rw-r--r--   0        0        0      415 2022-07-11 11:51:22.115125 yaspin-2.5.0/examples/right_spinner.py
+-rw-r--r--   0        0        0     4030 2023-08-06 12:02:54.702543 yaspin-2.5.0/examples/signals.py
+-rw-r--r--   0        0        0      854 2022-07-11 11:51:22.115125 yaspin-2.5.0/examples/spinner_properties.py
+-rw-r--r--   0        0        0      359 2022-07-19 11:35:29.002311 yaspin-2.5.0/examples/timer_spinner.py
+-rw-r--r--   0        0        0      452 2022-07-11 11:51:22.116125 yaspin-2.5.0/examples/write_method.py
+-rw-r--r--   0        0        0     2410 2023-08-07 16:04:19.181885 yaspin-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-07-11 11:51:22.128125 yaspin-2.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     7252 2023-08-06 12:43:09.750394 yaspin-2.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     3025 2022-07-19 10:41:34.977459 yaspin-2.5.0/tests/test_attrs.py
+-rw-r--r--   0        0        0      730 2022-07-11 11:51:22.128125 yaspin-2.5.0/tests/test_finalizers.py
+-rw-r--r--   0        0        0     7813 2023-02-26 15:11:07.365981 yaspin-2.5.0/tests/test_in_out.py
+-rw-r--r--   0        0        0     1507 2023-08-06 12:02:54.704543 yaspin-2.5.0/tests/test_pipes.py
+-rw-r--r--   0        0        0     3479 2023-08-06 12:02:54.704543 yaspin-2.5.0/tests/test_properties.py
+-rw-r--r--   0        0        0     2167 2022-07-19 10:41:34.979459 yaspin-2.5.0/tests/test_signals.py
+-rw-r--r--   0        0        0      695 2022-07-11 11:51:22.128125 yaspin-2.5.0/tests/test_spinners.py
+-rw-r--r--   0        0        0     1373 2022-07-11 11:51:22.128125 yaspin-2.5.0/tests/test_timer.py
+-rw-r--r--   0        0        0     1217 2023-08-06 12:02:54.704543 yaspin-2.5.0/tests/test_yaspin.py
+-rw-r--r--   0        0        0      218 2023-08-06 12:02:54.704543 yaspin-2.5.0/yaspin/__init__.py
+-rw-r--r--   0        0        0     2600 2023-08-06 12:02:54.704543 yaspin-2.5.0/yaspin/api.py
+-rw-r--r--   0        0        0      351 2023-08-06 12:02:54.704543 yaspin-2.5.0/yaspin/base_spinner.py
+-rw-r--r--   0        0        0     2749 2023-08-06 12:43:09.751394 yaspin-2.5.0/yaspin/constants.py
+-rw-r--r--   0        0        0    17974 2023-08-06 12:02:54.705543 yaspin-2.5.0/yaspin/core.py
+-rw-r--r--   0        0        0    26255 2023-08-06 12:43:09.751394 yaspin-2.5.0/yaspin/data/spinners.json
+-rw-r--r--   0        0        0      329 2023-08-06 12:02:54.705543 yaspin-2.5.0/yaspin/helpers.py
+-rw-r--r--   0        0        0     1065 2023-08-06 12:02:54.705543 yaspin-2.5.0/yaspin/signal_handlers.py
+-rw-r--r--   0        0        0      505 2023-08-06 12:02:54.705543 yaspin-2.5.0/yaspin/spinners.py
+-rw-r--r--   0        0        0    14118 1970-01-01 00:00:00.000000 yaspin-2.5.0/PKG-INFO
```

### Comparing `yaspin-2.4.0/HISTORY.rst` & `yaspin-2.5.0/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Release History
 ===============
 
+2.5.0 / 2023-08-07
+------------------
+
+* Drop Python 3.7 support
+* Update dependencies
+
+
 2.4.0 / 2023-08-06
 ------------------
 
 * Add Python 3.12 support
 * Update cli-spinners to ``v2.9.0``
 * Update dependencies
```

### Comparing `yaspin-2.4.0/LICENSE` & `yaspin-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/README.rst` & `yaspin-2.5.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 .. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/shark.gif
 
 
 Features
 --------
 
-- Runs at all major **CPython** versions (*3.7*, *3.8*, *3.9*, *3.10*, *3.11*, *3.12*), **PyPy**
+- Runs at all major **CPython** versions (*3.8*, *3.9*, *3.10*, *3.11*, *3.12*), **PyPy**
 - Supports all (70+) spinners from `cli-spinners`_
 - Supports all *colors*, *highlights*, *attributes* and their mixes from `termcolor`_ library
 - Easy to combine with other command-line libraries, e.g. `prompt-toolkit`_
 - Flexible API, easy to integrate with existing code
 - User-friendly API for handling POSIX `signals`_
 - Safe **pipes** and **redirects**:
```

### Comparing `yaspin-2.4.0/examples/advanced_colors.py` & `yaspin-2.5.0/examples/advanced_colors.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/examples/basic_usage.py` & `yaspin-2.5.0/examples/basic_usage.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/examples/colors.py` & `yaspin-2.5.0/examples/colors.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/examples/demo.py` & `yaspin-2.5.0/examples/demo.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/examples/dynamic_text.py` & `yaspin-2.5.0/examples/dynamic_text.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/examples/finalizers.py` & `yaspin-2.5.0/examples/finalizers.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/examples/hide_show.py` & `yaspin-2.5.0/examples/hide_show.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/examples/hide_show_prompt_toolkit.py` & `yaspin-2.5.0/examples/hide_show_prompt_toolkit.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/examples/signals.py` & `yaspin-2.5.0/examples/signals.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/examples/spinner_properties.py` & `yaspin-2.5.0/examples/spinner_properties.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/pyproject.toml` & `yaspin-2.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yaspin"
-version = "2.4.0"
+version = "2.5.0"
 description = "Yet Another Terminal Spinner"
 license = "MIT"
 authors = ["Pavlo Dmytrenko <pavdmyt@aiven.io>"]
 readme = "README.rst"
 homepage = "https://github.com/pavdmyt/yaspin"
 repository = "https://github.com/pavdmyt/yaspin"
 documentation = "https://github.com/pavdmyt/yaspin/blob/master/README.rst"
@@ -26,15 +26,14 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -46,26 +45,26 @@
     "Topic :: System :: Monitoring",
     "Topic :: System :: Shells",
     "Topic :: Terminals",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
-termcolor = "^2.2"
+python = "^3.8.1"
+termcolor = "^2.3"
 
 [tool.poetry.dev-dependencies]
-black = "^23.0"
+black = "^23.3"
 twine = "^4.0"
-flake8 = "^5.0"
+flake8 = "^6.1"
 isort = "^5.10"
-pytest = "^7.2"
-pytest-xdist = "^3.2"
-pytest-cov = "^4.0"
-pylint = "^2.16"
+pytest = "^7.4"
+pytest-xdist = "^3.3"
+pytest-cov = "^4.1"
+pylint = "^2.17"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/pavdmyt/yaspin/issues"
 "Changelog" = "https://github.com/pavdmyt/yaspin/releases"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
```

### Comparing `yaspin-2.4.0/tests/conftest.py` & `yaspin-2.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/tests/test_attrs.py` & `yaspin-2.5.0/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/tests/test_finalizers.py` & `yaspin-2.5.0/tests/test_finalizers.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/tests/test_in_out.py` & `yaspin-2.5.0/tests/test_in_out.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/tests/test_pipes.py` & `yaspin-2.5.0/tests/test_pipes.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/tests/test_properties.py` & `yaspin-2.5.0/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/tests/test_signals.py` & `yaspin-2.5.0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/tests/test_spinners.py` & `yaspin-2.5.0/tests/test_spinners.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/tests/test_timer.py` & `yaspin-2.5.0/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/tests/test_yaspin.py` & `yaspin-2.5.0/tests/test_yaspin.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/yaspin/api.py` & `yaspin-2.5.0/yaspin/api.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/yaspin/constants.py` & `yaspin-2.5.0/yaspin/constants.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/yaspin/core.py` & `yaspin-2.5.0/yaspin/core.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/yaspin/data/spinners.json` & `yaspin-2.5.0/yaspin/data/spinners.json`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/yaspin/signal_handlers.py` & `yaspin-2.5.0/yaspin/signal_handlers.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.4.0/PKG-INFO` & `yaspin-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 Metadata-Version: 2.1
 Name: yaspin
-Version: 2.4.0
+Version: 2.5.0
 Summary: Yet Another Terminal Spinner
 Home-page: https://github.com/pavdmyt/yaspin
 License: MIT
 Keywords: spinner,console,terminal,loader,indicator
 Author: Pavlo Dmytrenko
 Author-email: pavdmyt@aiven.io
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
-Requires-Dist: termcolor (>=2.2,<3.0)
+Requires-Dist: termcolor (>=2.3,<3.0)
 Project-URL: Bug Tracker, https://github.com/pavdmyt/yaspin/issues
 Project-URL: Changelog, https://github.com/pavdmyt/yaspin/releases
 Project-URL: Documentation, https://github.com/pavdmyt/yaspin/blob/master/README.rst
 Project-URL: Repository, https://github.com/pavdmyt/yaspin
 Description-Content-Type: text/x-rst
 
 |Logo|
@@ -97,15 +96,15 @@
 
 .. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/shark.gif
 
 
 Features
 --------
 
-- Runs at all major **CPython** versions (*3.7*, *3.8*, *3.9*, *3.10*, *3.11*, *3.12*), **PyPy**
+- Runs at all major **CPython** versions (*3.8*, *3.9*, *3.10*, *3.11*, *3.12*), **PyPy**
 - Supports all (70+) spinners from `cli-spinners`_
 - Supports all *colors*, *highlights*, *attributes* and their mixes from `termcolor`_ library
 - Easy to combine with other command-line libraries, e.g. `prompt-toolkit`_
 - Flexible API, easy to integrate with existing code
 - User-friendly API for handling POSIX `signals`_
 - Safe **pipes** and **redirects**:
```

