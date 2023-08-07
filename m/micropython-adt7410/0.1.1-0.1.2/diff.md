# Comparing `tmp/micropython-adt7410-0.1.1.tar.gz` & `tmp/micropython-adt7410-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-adt7410-0.1.1.tar", last modified: Sat Jun 17 15:38:21 2023, max compression
+gzip compressed data, was "micropython-adt7410-0.1.2.tar", last modified: Mon Aug  7 13:10:45 2023, max compression
```

## Comparing `micropython-adt7410-0.1.1.tar` & `micropython-adt7410-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.207476 micropython-adt7410-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/examples/adt7410_operation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/examples/adt7410_resolution_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/examples/adt7410_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/examples/adt7410_temp_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/micropython_adt7410/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/micropython_adt7410/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/micropython_adt7410/adt7410.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/micropython_adt7410/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-17 15:38:21.000000 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-17 15:38:21.000000 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:38:21.000000 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:38:21.000000 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 15:38:21.000000 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.373851 micropython-adt7410-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.365851 micropython-adt7410-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.369851 micropython-adt7410-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-07 13:10:45.373851 micropython-adt7410-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.369851 micropython-adt7410-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.369851 micropython-adt7410-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.369851 micropython-adt7410-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/examples/adt7410_operation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/examples/adt7410_resolution_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/examples/adt7410_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/examples/adt7410_temp_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.369851 micropython-adt7410-0.1.2/micropython_adt7410/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/micropython_adt7410/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/micropython_adt7410/adt7410.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/micropython_adt7410/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.373851 micropython-adt7410-0.1.2/micropython_adt7410.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-07 13:10:45.000000 micropython-adt7410-0.1.2/micropython_adt7410.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-07 13:10:45.000000 micropython-adt7410-0.1.2/micropython_adt7410.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:10:45.000000 micropython-adt7410-0.1.2/micropython_adt7410.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 13:10:45.000000 micropython-adt7410-0.1.2/micropython_adt7410.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:10:45.373851 micropython-adt7410-0.1.2/setup.cfg
```

### Comparing `micropython-adt7410-0.1.1/.pre-commit-config.yaml` & `micropython-adt7410-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-adt7410-0.1.1/.pylintrc` & `micropython-adt7410-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.1/LICENSE` & `micropython-adt7410-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.1/PKG-INFO` & `micropython-adt7410-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-adt7410
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Analog Devices ADT7410 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ADT7410
-Keywords: sensor,micropython,adt7410,temperature,adt7410,sensor,driver,micropython
+Keywords: sensor,micropython,adt7410,temperature,adt7410,driver,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-adt7410-0.1.1/README.rst` & `micropython-adt7410-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.1/docs/_static/Logo.png` & `micropython-adt7410-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.1/docs/conf.py` & `micropython-adt7410-0.1.2/docs/conf.py`

 * *Files 22% similar despite different names*

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
+    import micropython_adt7410
+except ImportError:
+    raise SystemExit("micropython_adt7410 has to be importable")
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
-        "MicroPython_adt7410_Library.tex",
-        "MicroPython adt7410 Library Documentation",
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
-        "MicroPython_adt7410_Library",
-        "MicroPython adt7410 Library Documentation",
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
-        "MicroPython_adt7410_Library",
-        "MicroPython adt7410 Library Documentation",
-        author,
-        "MicroPython_adt7410_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-adt7410-0.1.1/docs/examples.rst` & `micropython-adt7410-0.1.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.1/examples/adt7410_operation_mode.py` & `micropython-adt7410-0.1.2/examples/adt7410_operation_mode.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 
 adt.operation_mode = adt7410.SPS
 
 while True:
     for operation_mode in adt7410.operation_mode_values:
         print("Current Operation mode setting: ", adt.operation_mode)
         for _ in range(10):
-            print("Temperature: {:.2f}C".format(adt.temperature))
+            print(f"Temperature: {adt.temperature:.2f}°C")
+            print()
             time.sleep(0.5)
         adt.operation_mode = operation_mode
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-adt7410-0.1.1/examples/adt7410_resolution_mode.py` & `micropython-adt7410-0.1.2/examples/adt7410_resolution_mode.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 
 adt.resolution_mode = adt7410.HIGH_RESOLUTION
 
 while True:
     for resolution_mode in adt7410.resolution_mode_values:
         print("Current Resolution mode setting: ", adt.resolution_mode)
         for _ in range(10):
-            temp = adt.temperature
-            print("Temperature :{:.2f}C".format(temp))
+            print(f"Temperature: {adt.temperature:.2f}°C")
+            print()
             time.sleep(0.5)
         adt.resolution_mode = resolution_mode
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-adt7410-0.1.1/examples/adt7410_temp_limits.py` & `micropython-adt7410-0.1.2/examples/adt7410_temp_limits.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 adt = adt7410.ADT7410(i2c)
 
 adt.low_temperature = 18
 adt.high_temperature = 29
 adt.critical_temperature = 35
 adt.hysteresis_temperature = 2
 
-print("High limit: {}C".format(adt.high_temperature))
-print("Low limit: {}C".format(adt.low_temperature))
-print("Critical limit: {}C".format(adt.critical_temperature))
+print("High limit: {}°C".format(adt.high_temperature))
+print("Low limit: {}°C".format(adt.low_temperature))
+print("Critical limit: {}°C".format(adt.critical_temperature))
 
 adt.comparator_mode = adt7410.COMP_ENABLED
 
 while True:
-    print("Temperature: {:.2f}C".format(adt.temperature))
+    print(f"Temperature: {adt.temperature:.2f}°C")
+    print()
     alert_status = adt.alert_status
     if alert_status.high_alert:
         print("Temperature above high set limit!")
     if alert_status.low_alert:
         print("Temperature below low set limit!")
     if alert_status.critical_alert:
         print("Temperature above critical set limit!")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-adt7410-0.1.1/examples.json` & `micropython-adt7410-0.1.2/examples.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'version'": "'1'"}*

```diff
@@ -13,9 +13,9 @@
             "github:jposada202020/MicroPython_ADT7410/examples/adt7410_resolution_mode.py"
         ],
         [
             "micropython_adt7410/examples/adt7410_operation_mode.py",
             "github:jposada202020/MicroPython_ADT7410/examples/adt7410_operation_mode.py"
         ]
     ],
-    "version": "0.1"
+    "version": "1"
 }
```

### Comparing `micropython-adt7410-0.1.1/micropython_adt7410/adt7410.py` & `micropython-adt7410-0.1.2/micropython_adt7410/adt7410.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import time
 from collections import namedtuple
 from micropython import const
 from micropython_adt7410.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_ADT7410.git"
 
 
 _REG_WHOAMI = const(0xB)
 _TEMP = const(0x00)
 _STATUS = const(0x02)
 _CONFIGURATION = const(0x03)
@@ -48,34 +48,50 @@
 
 AlertStatus = namedtuple("AlertStatus", ["high_alert", "low_alert", "critical_alert"])
 
 
 class ADT7410:
     """Driver for the ADT7410 Sensor connected over I2C.
 
+    The ADT7410 is a high accuracy digital temperature sensor. it has
+    a 13-bit ADC to monitor and digitize the temperature to a
+    0.0625°C resolution.
+
+    The ADC resolution, by default, is set to 13 bits (0.0625°C).
+    This can be changed to 16 bits (0.0078°C) by :attr:`resolution_mode`
+
+    The ADT7410 is rated for operation over the −55°C to +150°C temperature
+    range
+
+    In normal mode, the ADT7410 runs an automatic conversion
+    sequence. During this automatic conversion sequence, a conversion
+    takes 240 ms to complete and the ADT7410 is continuously
+    converting.
+
+
     :param ~machine.I2C i2c: The I2C bus the ADT7410 is connected to.
-    :param int address: The I2C device address. Defaults to :const:`0x69`
+    :param int address: The I2C device address. Defaults to :const:`0x48`
 
     :raises RuntimeError: if the sensor is not found
 
     **Quickstart: Importing and using the device**
 
     Here is an example of using the :class:`ADT7410` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import adt7410
+        from micropython_adt7410 import adt7410
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         adt = adt7410.ADT7410(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
         temp = adt.temperature
@@ -219,19 +235,19 @@
     def alert_status(self):
         """The current triggered status of the high and low temperature alerts as a AlertStatus
         named tuple with attributes for the triggered status of each alert.
 
         .. code-block :: python
 
             import time
-            import board
-            import adt7410
+            from machine import Pin, I2C
+            from micropython_mcp9808 import mcp9808
 
-            i2c = board.I2C()  # uses board.SCL and board.SDA
-            adt = adt7410.ADT7410(i2c)
+            i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
+            mcp = mcp9808.MCP9808(i2c)
 
             tmp.low_temperature = 20
             tmp.high_temperature = 23
             tmp.critical_temperature = 30
 
             print("High limit: {}".format(tmp.high_temperature))
             print("Low limit: {}".format(tmp.low_temperature))
@@ -258,14 +274,21 @@
             critical_alert=self._critical_alert,
         )
 
     @property
     def comparator_mode(self) -> str:
         """
         Sensor comparator_mode
+        In comparator mode, the INT pin returns to its inactive status
+        when the temperature drops below the
+        :attr:`high_temperature` − :attr:`hysteresis_temperature` limit or
+        rises above the :attr:`low_temperature` + :attr:`hysteresis_temperature`
+        limit.
+        Putting the ADT7410 into shutdown mode does not reset the
+        INT state in comparator mode
 
         +-----------------------------------+-----------------+
         | Mode                              | Value           |
         +===================================+=================+
         | :py:const:`adt7410.COMP_DISABLED` | :py:const:`0b0` |
         +-----------------------------------+-----------------+
         | :py:const:`adt7410.COMP_ENABLED`  | :py:const:`0b1` |
```

### Comparing `micropython-adt7410-0.1.1/micropython_adt7410/i2c_helpers.py` & `micropython-adt7410-0.1.2/micropython_adt7410/i2c_helpers.py`

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

### Comparing `micropython-adt7410-0.1.1/micropython_adt7410.egg-info/PKG-INFO` & `micropython-adt7410-0.1.2/micropython_adt7410.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-adt7410
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Analog Devices ADT7410 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ADT7410
-Keywords: sensor,micropython,adt7410,temperature,adt7410,sensor,driver,micropython
+Keywords: sensor,micropython,adt7410,temperature,adt7410,driver,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-adt7410-0.1.1/micropython_adt7410.egg-info/SOURCES.txt` & `micropython-adt7410-0.1.2/micropython_adt7410.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -26,9 +26,8 @@
 examples/adt7410_temp_limits.py
 micropython_adt7410/__init__.py
 micropython_adt7410/adt7410.py
 micropython_adt7410/i2c_helpers.py
 micropython_adt7410.egg-info/PKG-INFO
 micropython_adt7410.egg-info/SOURCES.txt
 micropython_adt7410.egg-info/dependency_links.txt
-micropython_adt7410.egg-info/requires.txt
 micropython_adt7410.egg-info/top_level.txt
```

### Comparing `micropython-adt7410-0.1.1/pyproject.toml` & `micropython-adt7410-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -8,27 +8,26 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-adt7410"
 description = "MicroPython Driver for the Analog Devices ADT7410 Temperature Sensor"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_ADT7410"}
 keywords = [
     "sensor",
     "micropython",
     "adt7410",
     "temperature",
     "adt7410",
-    "sensor",
     "driver",
     "micropython",
 ]
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
@@ -36,11 +35,11 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["adt7410"]
+packages = ["micropython_adt7410"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

