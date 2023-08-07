# Comparing `tmp/micropython-adxl343-0.1.1.tar.gz` & `tmp/micropython-adxl343-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-adxl343-0.1.1.tar", last modified: Sat Jun 17 14:35:04 2023, max compression
+gzip compressed data, was "micropython-adxl343-0.1.2.tar", last modified: Mon Aug  7 13:23:56 2023, max compression
```

## Comparing `micropython-adxl343-0.1.1.tar` & `micropython-adxl343-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.574675 micropython-adxl343-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.574675 micropython-adxl343-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.574675 micropython-adxl343-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_acceleration_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_activity_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_double_tap_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_inactivity_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_resolution_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_single_tap_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/micropython_adxl343/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/micropython_adxl343/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/micropython_adxl343/adxl343.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/micropython_adxl343/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-17 14:35:04.000000 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-17 14:35:04.000000 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:35:04.000000 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:35:04.000000 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 14:35:04.000000 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:23:56.673863 micropython-adxl343-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:23:56.661862 micropython-adxl343-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:23:56.665862 micropython-adxl343-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-08-07 13:23:56.673863 micropython-adxl343-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:23:56.665862 micropython-adxl343-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:23:56.669863 micropython-adxl343-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:23:56.669863 micropython-adxl343-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/examples/adxl343_acceleration_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/examples/adxl343_activity_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/examples/adxl343_double_tap_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/examples/adxl343_inactivity_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/examples/adxl343_inactivity_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/examples/adxl343_resolution_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/examples/adxl343_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/examples/adxl343_single_tap_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:23:56.669863 micropython-adxl343-0.1.2/micropython_adxl343/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/micropython_adxl343/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/micropython_adxl343/adxl343.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/micropython_adxl343/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:23:56.673863 micropython-adxl343-0.1.2/micropython_adxl343.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-08-07 13:23:56.000000 micropython-adxl343-0.1.2/micropython_adxl343.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-07 13:23:56.000000 micropython-adxl343-0.1.2/micropython_adxl343.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:23:56.000000 micropython-adxl343-0.1.2/micropython_adxl343.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 13:23:56.000000 micropython-adxl343-0.1.2/micropython_adxl343.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-07 13:23:47.000000 micropython-adxl343-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:23:36.000000 micropython-adxl343-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:23:56.673863 micropython-adxl343-0.1.2/setup.cfg
```

### Comparing `micropython-adxl343-0.1.1/.pre-commit-config.yaml` & `micropython-adxl343-0.1.2/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
-        exclude: "^(docs/|examples/|tests/|setup.py$)"
+        exclude: "^(docs/|examples/|tests/)"
       - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
           - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-      - id: pylint
-        name: pylint (test code)
-        description: Run pylint rules on "tests/*.py" files
-        types: [python]
-        files: "^tests/"
-        args:
-          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `micropython-adxl343-0.1.1/.pylintrc` & `micropython-adxl343-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1.1/LICENSE` & `micropython-adxl343-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1.1/PKG-INFO` & `micropython-adxl343-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-adxl343
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Analog Devices ADXL343 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ADXL343
-Keywords: sensor,micropython,adxl343,tap,double,activity,acceleration,accelerometer,adxl343,micropython,gravity,sensor,driver
+Keywords: sensor,micropython,adxl343,tap,double,activity,acceleration,accelerometer,adxl343,gravity,sensor,driver
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-adxl343-0.1.1/README.rst` & `micropython-adxl343-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1.1/docs/_static/Logo.png` & `micropython-adxl343-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1.1/docs/conf.py` & `micropython-adxl343-0.1.2/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,39 @@
-# -*- coding: utf-8 -*-
-
 # SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
 import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
+try:
+    # Inject mock modules so that we can build the
+    # documentation without having the real stuff available
+    from mock import Mock
+
+    to_be_mocked = [
+        "micropython",
+        "machine",
+    ]
+    for module in to_be_mocked:
+        sys.modules[module] = Mock()
+        print("Mocked '{}' module".format(module))
+
+    import micropython_adxl343
+except ImportError:
+    raise SystemExit("micropython_adxl343 has to be importable")
+
 # -- General configuration ------------------------------------------------
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
-    "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinx_immaterial",
 ]
 
 autodoc_preserve_defaults = True
 
 intersphinx_mapping = {
@@ -182,65 +196,7 @@
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # These paths are either relative to html_static_path
 # or fully qualified paths (eg. https://...)
 html_css_files = ["extra_css.css"]
-
-
-# -- Options for LaTeX output ---------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    # 'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    # 'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    # 'preamble': '',
-    # Latex figure (float) alignment
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title,
-#  author, documentclass [howto, manual, or own class]).
-latex_documents = [
-    (
-        master_doc,
-        "MicroPython_adxl343_Library.tex",
-        "MicroPython adxl343 Library Documentation",
-        author,
-        "manual",
-    ),
-]
-
-# -- Options for manual page output ---------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (
-        master_doc,
-        "MicroPython_adxl343_Library",
-        "MicroPython adxl343 Library Documentation",
-        [author],
-        1,
-    ),
-]
-
-# -- Options for Texinfo output -------------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (
-        master_doc,
-        "MicroPython_adxl343_Library",
-        "MicroPython adxl343 Library Documentation",
-        author,
-        "MicroPython_adxl343_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-adxl343-0.1.1/docs/examples.rst` & `micropython-adxl343-0.1.2/docs/examples.rst`

 * *Files 6% similar despite different names*

```diff
@@ -56,7 +56,16 @@
 -------------------------
 
 Example showing an inactivity detection example
 
 .. literalinclude:: ../examples/adxl343_inactivity_detection.py
     :caption: examples/adxl343_inactivity_detection.py
     :lines: 5-
+
+Inactivity mode settings
+-------------------------
+
+Example showing the Inactivity mode setting
+
+.. literalinclude:: ../examples/adxl343_inactivity_mode.py
+    :caption: examples/adxl343_inactivity_mode.py
+    :lines: 5-
```

### Comparing `micropython-adxl343-0.1.1/examples/adxl343_acceleration_range.py` & `micropython-adxl343-0.1.2/examples/adxl343_resolution_mode.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from machine import Pin, I2C
 from micropython_adxl343 import adxl343
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 adx = adxl343.ADXL343(i2c)
 
 
+adx.resolution_mode = adxl343.LOW_RES
 adx.acceleration_range = adxl343.RANGE_16
 
 while True:
     for acceleration_range in adxl343.acceleration_range_values:
         print("Current Acceleration range setting: ", adx.acceleration_range)
-        for _ in range(10):
+        for _ in range(2):
             accx, accy, accz = adx.acceleration
-            print("x:{:.2f}m/s2, y:{:.2f}m/s2, z:{:.2f}m/s2".format(accx, accy, accz))
+            print(f"x:{accx:.2f}m/s2, y:{accy:.2f}m/s2, z:{accz:.2f}m/s2")
             time.sleep(0.5)
         adx.acceleration_range = acceleration_range
```

### Comparing `micropython-adxl343-0.1.1/examples/adxl343_double_tap_mode.py` & `micropython-adxl343-0.1.2/examples/adxl343_double_tap_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1.1/micropython_adxl343/adxl343.py` & `micropython-adxl343-0.1.2/micropython_adxl343/adxl343.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_ADXL343.git"
 
 _STANDARD_GRAVITY = 9.80665
 _REG_WHOAMI = const(0x00)
 _POWER_CTL = const(0x2D)
 _DATA_FORMAT = const(0x31)
 _ACC = const(0x32)
@@ -82,21 +82,21 @@
 
     Here is an example of using the :class:`ADXL343` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import adxl343
+        from micropython_adxl343 import adxl343
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         adxl = adxl343.ADXL343(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
         accx, accy, accz = adx.acceleration
@@ -263,15 +263,14 @@
         Tap threshold in :math:`m / s ^ 2`
         :return:
         """
         return self._tap_threshold * 0.0627451 * _STANDARD_GRAVITY
 
     @tap_threshold.setter
     def tap_threshold(self, value: float) -> None:
-
         if 156 < value < 1:
             raise ValueError("Value should be a valid tap_threshold setting")
         self._tap_threshold = int(value / _STANDARD_GRAVITY / 0.0627451)
 
     @property
     def single_tap_mode(self) -> str:
         """
```

### Comparing `micropython-adxl343-0.1.1/micropython_adxl343/i2c_helpers.py` & `micropython-adxl343-0.1.2/micropython_adxl343/i2c_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,18 +35,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 """
 # pylint: disable=too-many-arguments
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
+import struct
 
 
 class CBits:
     """
     Changes bits from a byte register
     """
 
@@ -65,30 +62,28 @@
         self.lsb_first = lsb_first
 
     def __get__(
         self,
         obj,
         objtype=None,
     ) -> int:
-
         mem_value = obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
 
         reg = 0
         order = range(len(mem_value) - 1, -1, -1)
         if not self.lsb_first:
             order = reversed(order)
         for i in order:
             reg = (reg << 8) | mem_value[i]
 
         reg = (reg & self.bit_mask) >> self.star_bit
 
         return reg
 
     def __set__(self, obj, value: int) -> None:
-
         memory_value = obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
 
         reg = 0
         order = range(len(memory_value) - 1, -1, -1)
         if not self.lsb_first:
             order = range(0, len(memory_value))
         for i in order:
@@ -113,15 +108,14 @@
         self.lenght = struct.calcsize(form)
 
     def __get__(
         self,
         obj,
         objtype=None,
     ):
-
         if self.lenght <= 2:
             value = struct.unpack(
                 self.format,
                 memoryview(
                     obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
                 ),
             )[0]
```

### Comparing `micropython-adxl343-0.1.1/micropython_adxl343.egg-info/PKG-INFO` & `micropython-adxl343-0.1.2/micropython_adxl343.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-adxl343
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Analog Devices ADXL343 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ADXL343
-Keywords: sensor,micropython,adxl343,tap,double,activity,acceleration,accelerometer,adxl343,micropython,gravity,sensor,driver
+Keywords: sensor,micropython,adxl343,tap,double,activity,acceleration,accelerometer,adxl343,gravity,sensor,driver
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-adxl343-0.1.1/micropython_adxl343.egg-info/SOURCES.txt` & `micropython-adxl343-0.1.2/micropython_adxl343.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/adxl343_acceleration_range.py
 examples/adxl343_activity_detection.py
 examples/adxl343_double_tap_mode.py
 examples/adxl343_inactivity_detection.py
+examples/adxl343_inactivity_mode.py
 examples/adxl343_resolution_mode.py
 examples/adxl343_simpletest.py
 examples/adxl343_single_tap_mode.py
 micropython_adxl343/__init__.py
 micropython_adxl343/adxl343.py
 micropython_adxl343/i2c_helpers.py
 micropython_adxl343.egg-info/PKG-INFO
 micropython_adxl343.egg-info/SOURCES.txt
 micropython_adxl343.egg-info/dependency_links.txt
-micropython_adxl343.egg-info/requires.txt
 micropython_adxl343.egg-info/top_level.txt
```

### Comparing `micropython-adxl343-0.1.1/pyproject.toml` & `micropython-adxl343-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-adxl343"
 description = "MicroPython Driver for the Analog Devices ADXL343 Accelerometer"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_ADXL343"}
 keywords = [
     "sensor",
@@ -24,15 +24,14 @@
     "adxl343",
     "tap",
     "double",
     "activity",
     "acceleration",
     "accelerometer",
     "adxl343",
-    "micropython",
     "gravity",
     "sensor",
     "driver",
 ]
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
@@ -41,11 +40,11 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["adxl343"]
+packages = ["micropython_adxl343"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

