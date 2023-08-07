# Comparing `tmp/micropython-bma400-0.1.1.tar.gz` & `tmp/micropython-bma400-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-bma400-0.1.1.tar", last modified: Sat Jun 17 14:28:43 2023, max compression
+gzip compressed data, was "micropython-bma400-0.1.2.tar", last modified: Mon Aug  7 13:43:45 2023, max compression
```

## Comparing `micropython-bma400-0.1.1.tar` & `micropython-bma400-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:28:43.604507 micropython-bma400-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:28:43.596507 micropython-bma400-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:28:43.600507 micropython-bma400-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-17 14:28:43.604507 micropython-bma400-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:28:43.600507 micropython-bma400-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:28:43.604507 micropython-bma400-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:28:43.604507 micropython-bma400-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-17 14:28:33.000000 micropython-bma400-0.1.1/examples/bma400_acc_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-17 14:28:33.000000 micropython-bma400-0.1.1/examples/bma400_filter_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-17 14:28:33.000000 micropython-bma400-0.1.1/examples/bma400_output_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-17 14:28:33.000000 micropython-bma400-0.1.1/examples/bma400_oversampling_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-17 14:28:33.000000 micropython-bma400-0.1.1/examples/bma400_power_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-17 14:28:33.000000 micropython-bma400-0.1.1/examples/bma400_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-17 14:28:33.000000 micropython-bma400-0.1.1/examples/bma400_source_data_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:28:43.604507 micropython-bma400-0.1.1/micropython_bma400/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:28:33.000000 micropython-bma400-0.1.1/micropython_bma400/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-06-17 14:28:33.000000 micropython-bma400-0.1.1/micropython_bma400/bma400.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:28:33.000000 micropython-bma400-0.1.1/micropython_bma400/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:28:43.604507 micropython-bma400-0.1.1/micropython_bma400.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-17 14:28:43.000000 micropython-bma400-0.1.1/micropython_bma400.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-17 14:28:43.000000 micropython-bma400-0.1.1/micropython_bma400.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:28:43.000000 micropython-bma400-0.1.1/micropython_bma400.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:28:43.000000 micropython-bma400-0.1.1/micropython_bma400.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 14:28:43.000000 micropython-bma400-0.1.1/micropython_bma400.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-17 14:28:33.000000 micropython-bma400-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:28:23.000000 micropython-bma400-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:28:43.604507 micropython-bma400-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:43:45.532995 micropython-bma400-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:43:45.528995 micropython-bma400-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:43:45.528995 micropython-bma400-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-08-07 13:43:45.532995 micropython-bma400-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:43:45.532995 micropython-bma400-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:43:45.532995 micropython-bma400-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:43:45.532995 micropython-bma400-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-07 13:43:37.000000 micropython-bma400-0.1.2/examples/bma400_acc_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-07 13:43:37.000000 micropython-bma400-0.1.2/examples/bma400_filter_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-07 13:43:37.000000 micropython-bma400-0.1.2/examples/bma400_output_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-07 13:43:37.000000 micropython-bma400-0.1.2/examples/bma400_oversampling_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-07 13:43:37.000000 micropython-bma400-0.1.2/examples/bma400_power_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-07 13:43:37.000000 micropython-bma400-0.1.2/examples/bma400_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-07 13:43:37.000000 micropython-bma400-0.1.2/examples/bma400_source_data_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:43:45.532995 micropython-bma400-0.1.2/micropython_bma400/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:43:37.000000 micropython-bma400-0.1.2/micropython_bma400/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-08-07 13:43:37.000000 micropython-bma400-0.1.2/micropython_bma400/bma400.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-07 13:43:37.000000 micropython-bma400-0.1.2/micropython_bma400/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:43:45.532995 micropython-bma400-0.1.2/micropython_bma400.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-08-07 13:43:45.000000 micropython-bma400-0.1.2/micropython_bma400.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-07 13:43:45.000000 micropython-bma400-0.1.2/micropython_bma400.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:43:45.000000 micropython-bma400-0.1.2/micropython_bma400.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 13:43:45.000000 micropython-bma400-0.1.2/micropython_bma400.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-07 13:43:37.000000 micropython-bma400-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:43:29.000000 micropython-bma400-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:43:45.532995 micropython-bma400-0.1.2/setup.cfg
```

### Comparing `micropython-bma400-0.1.1/.pre-commit-config.yaml` & `micropython-bma400-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-bma400-0.1.1/.pylintrc` & `micropython-bma400-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-bma400-0.1.1/LICENSE` & `micropython-bma400-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-bma400-0.1.1/PKG-INFO` & `micropython-bma400-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-bma400
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Bosch BMA400 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMA400
-Keywords: sensor,micropython,bma400,acceleration,gravity,sensor,bosch,bma400,accelerometer
+Keywords: sensor,micropython,bma400,acceleration,gravity,sensor,bosch,accelerometer
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-bma400-0.1.1/README.rst` & `micropython-bma400-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-bma400-0.1.1/docs/_static/Logo.png` & `micropython-bma400-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-bma400-0.1.1/docs/conf.py` & `micropython-bma400-0.1.2/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,31 @@
 
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
+    import micropython_bma400
+except ImportError:
+    raise SystemExit("micropython_bma400 has to be importable")
+
 # -- General configuration ------------------------------------------------
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
@@ -182,65 +199,7 @@
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
-        "MicroPython_bma400_Library.tex",
-        "MicroPython bma400 Library Documentation",
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
-        "MicroPython_bma400_Library",
-        "MicroPython bma400 Library Documentation",
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
-        "MicroPython_bma400_Library",
-        "MicroPython bma400 Library Documentation",
-        author,
-        "MicroPython_bma400_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-bma400-0.1.1/docs/examples.rst` & `micropython-bma400-0.1.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-bma400-0.1.1/examples/bma400_acc_range.py` & `micropython-bma400-0.1.2/examples/bma400_acc_range.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 bma.acc_range = bma400.ACC_RANGE_16
 
 while True:
     for acc_range in bma400.acc_range_values:
         print("Current Acc range setting: ", bma.acc_range)
         for _ in range(10):
             accx, accy, accz = bma.acceleration
-            print("x:{:.2f}Gs, y:{:.2f}Gs, z:{:.2f}Gs".format(accx, accy, accz))
+            print(f"x:{accx:.2f}Gs, y:{accy:.2f}Gs, z:{accz:.2f}Gs")
             time.sleep(0.5)
         bma.acc_range = acc_range
```

### Comparing `micropython-bma400-0.1.1/examples/bma400_filter_bandwidth.py` & `micropython-bma400-0.1.2/examples/bma400_filter_bandwidth.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 bma.filter_bandwidth = bma400.ACC_FILT_BW0
 
 while True:
     for filter_bandwidth in bma400.filter_bandwidth_values:
         print("Current Filter bandwidth setting: ", bma.filter_bandwidth)
         for _ in range(10):
             accx, accy, accz = bma.acceleration
-            print("x:{:.2f}Gs, y:{:.2f}Gs, z:{:.2f}Gs".format(accx, accy, accz))
+            print(f"x:{accx:.2f}Gs, y:{accy:.2f}Gs, z:{accz:.2f}Gs")
             time.sleep(0.5)
         bma.filter_bandwidth = filter_bandwidth
```

### Comparing `micropython-bma400-0.1.1/examples/bma400_output_data_rate.py` & `micropython-bma400-0.1.2/examples/bma400_output_data_rate.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 bma.output_data_rate = bma400.ACCEL_50HZ
 
 while True:
     for output_data_rate in bma400.output_data_rate_values:
         print("Current Output data rate setting: ", bma.output_data_rate)
         for _ in range(10):
             accx, accy, accz = bma.acceleration
-            print("x:{:.2f}Gs, y:{:.2f}Gs, z:{:.2f}Gs".format(accx, accy, accz))
+            print(f"x:{accx:.2f}Gs, y:{accy:.2f}Gs, z:{accz:.2f}Gs")
             time.sleep(0.5)
         bma.output_data_rate = output_data_rate
```

### Comparing `micropython-bma400-0.1.1/examples/bma400_oversampling_rate.py` & `micropython-bma400-0.1.2/examples/bma400_oversampling_rate.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 bma.oversampling_rate = bma400.OVERSAMPLING_2
 
 while True:
     for oversampling_rate in bma400.oversampling_rate_values:
         print("Current Oversampling rate setting: ", bma.oversampling_rate)
         for _ in range(10):
             accx, accy, accz = bma.acceleration
-            print("x:{:.2f}Gs, y:{:.2f}Gs, z:{:.2f}Gs".format(accx, accy, accz))
+            print(f"x:{accx:.2f}Gs, y:{accy:.2f}Gs, z:{accz:.2f}Gs")
             time.sleep(0.5)
         bma.oversampling_rate = oversampling_rate
```

### Comparing `micropython-bma400-0.1.1/examples/bma400_source_data_registers.py` & `micropython-bma400-0.1.2/examples/bma400_source_data_registers.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 bma.source_data_registers = bma400.ACC_FILT2
 
 while True:
     for source_data_registers in bma400.source_data_registers_values:
         print("Current Source data registers setting: ", bma.source_data_registers)
         for _ in range(10):
             accx, accy, accz = bma.acceleration
-            print("x:{:.2f}Gs, y:{:.2f}Gs, z:{:.2f}Gs".format(accx, accy, accz))
+            print(f"x:{accx:.2f}Gs, y:{accy:.2f}Gs, z:{accz:.2f}Gs")
             time.sleep(0.5)
         bma.source_data_registers = source_data_registers
```

### Comparing `micropython-bma400-0.1.1/micropython_bma400/bma400.py` & `micropython-bma400-0.1.2/micropython_bma400/bma400.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA400.git"
 
 _REG_WHOAMI = const(0x00)
 _ACC_CONFIG0 = const(0x19)
 _ACC_CONFIG1 = const(0x1A)
 _ACC_CONFIG2 = const(0x1B)
+_ACC_CONVERSION = const(9.80665)
 
 # Power Modes
 SLEEP_MODE = const(0x00)
 LOW_POWER_MODE = const(0x01)
 NORMAL_MODE = const(0x02)
 SWITCH_TO_SLEEP = const(0x03)
 power_mode_values = (SLEEP_MODE, LOW_POWER_MODE, NORMAL_MODE, SWITCH_TO_SLEEP)
@@ -100,21 +101,21 @@
 
     Here is an example of using the :class:`BMA400` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import bma400
+        from micropython_bma400 import bma400
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         bma400 = bma400.BMA400(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
         accx, accy, accz = bma.acceleration
@@ -352,29 +353,29 @@
         if value not in source_data_registers_values:
             raise ValueError("Value must be a valid source_data_registers setting")
         self._source_data_registers = value
 
     @property
     def acceleration(self) -> Tuple[int, int, int]:
         """
-        Acceleration
+        Acceleration in :math:`m/s^2`
         :return: acceleration
         """
         rawx, rawy, rawz = self._acceleration
 
         if rawx > 2047:
             rawx = rawx - 4096
 
         if rawy > 2047:
             rawy = rawy - 4096
 
         if rawz > 2047:
             rawz = rawz - 4096
 
-        factor = acc_range_factor[self._acc_range_mem]
+        factor = acc_range_factor[self._acc_range_mem] * _ACC_CONVERSION
 
         return rawx / factor, rawy / factor, rawz / factor
 
     @property
     def temperature(self) -> float:
         """
         The temperature sensor is calibrated with a precision of +/-5°C.
@@ -383,11 +384,10 @@
         raw_temp = self._temperature
         time.sleep(0.16)
         temp = self._twos_comp(raw_temp, 8)
         return (temp * 0.5) + 23
 
     @staticmethod
     def _twos_comp(val: int, bits: int) -> int:
-
         if val & (1 << (bits - 1)) != 0:
             return val - (1 << bits)
         return val
```

### Comparing `micropython-bma400-0.1.1/micropython_bma400/i2c_helpers.py` & `micropython-bma400-0.1.2/micropython_bma400/i2c_helpers.py`

 * *Files 8% similar despite different names*

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
@@ -131,9 +125,9 @@
                 memoryview(
                     obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
                 ),
             )
         return value
 
     def __set__(self, obj, value):
-        mem_value = value.to_bytes(self.lenght, "big")
+        mem_value = struct.pack(self.format, value)
         obj._i2c.writeto_mem(obj._address, self.register, mem_value)
```

### Comparing `micropython-bma400-0.1.1/micropython_bma400.egg-info/PKG-INFO` & `micropython-bma400-0.1.2/micropython_bma400.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-bma400
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Bosch BMA400 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMA400
-Keywords: sensor,micropython,bma400,acceleration,gravity,sensor,bosch,bma400,accelerometer
+Keywords: sensor,micropython,bma400,acceleration,gravity,sensor,bosch,accelerometer
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-bma400-0.1.1/micropython_bma400.egg-info/SOURCES.txt` & `micropython-bma400-0.1.2/micropython_bma400.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,9 +29,8 @@
 examples/bma400_source_data_registers.py
 micropython_bma400/__init__.py
 micropython_bma400/bma400.py
 micropython_bma400/i2c_helpers.py
 micropython_bma400.egg-info/PKG-INFO
 micropython_bma400.egg-info/SOURCES.txt
 micropython_bma400.egg-info/dependency_links.txt
-micropython_bma400.egg-info/requires.txt
 micropython_bma400.egg-info/top_level.txt
```

### Comparing `micropython-bma400-0.1.1/pyproject.toml` & `micropython-bma400-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,40 +8,39 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-bma400"
 description = "MicroPython Driver for the Bosch BMA400 Accelerometer"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_BMA400"}
 keywords = [
     "sensor",
     "micropython",
     "bma400",
     "acceleration",
     "gravity",
     "sensor",
     "bosch",
-    "bma400",
     "accelerometer",
 ]
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Embedded Systems",
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["bma400"]
+packages = ["micropython_bma400"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

