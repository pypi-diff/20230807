# Comparing `tmp/micropython-qmc5883l-0.1.1.tar.gz` & `tmp/micropython-qmc5883l-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-qmc5883l-0.1.1.tar", last modified: Sat Jun 17 14:51:06 2023, max compression
+gzip compressed data, was "micropython-qmc5883l-0.1.2.tar", last modified: Mon Aug  7 13:37:06 2023, max compression
```

## Comparing `micropython-qmc5883l-0.1.1.tar` & `micropython-qmc5883l-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.542938 micropython-qmc5883l-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-17 14:51:06.542938 micropython-qmc5883l-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_advanced_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_field_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_magnetic_compass.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_oversample.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/micropython_qmc5883l/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l/qmc5883l.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.542938 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-17 14:51:06.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-17 14:51:06.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:51:06.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:51:06.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 14:51:06.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:51:06.542938 micropython-qmc5883l-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:37:06.128467 micropython-qmc5883l-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:37:06.124467 micropython-qmc5883l-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:37:06.124467 micropython-qmc5883l-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-07 13:37:06.128467 micropython-qmc5883l-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:37:06.124467 micropython-qmc5883l-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:37:06.124467 micropython-qmc5883l-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:37:06.128467 micropython-qmc5883l-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-07 13:36:57.000000 micropython-qmc5883l-0.1.2/examples/qmc5883l_advanced_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-07 13:36:57.000000 micropython-qmc5883l-0.1.2/examples/qmc5883l_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-07 13:36:57.000000 micropython-qmc5883l-0.1.2/examples/qmc5883l_field_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-07 13:36:57.000000 micropython-qmc5883l-0.1.2/examples/qmc5883l_magnetic_compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-07 13:36:57.000000 micropython-qmc5883l-0.1.2/examples/qmc5883l_oversample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-07 13:36:57.000000 micropython-qmc5883l-0.1.2/examples/qmc5883l_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:37:06.128467 micropython-qmc5883l-0.1.2/micropython_qmc5883l/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:36:57.000000 micropython-qmc5883l-0.1.2/micropython_qmc5883l/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 13:36:57.000000 micropython-qmc5883l-0.1.2/micropython_qmc5883l/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-08-07 13:36:57.000000 micropython-qmc5883l-0.1.2/micropython_qmc5883l/qmc5883l.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:37:06.128467 micropython-qmc5883l-0.1.2/micropython_qmc5883l.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-07 13:37:06.000000 micropython-qmc5883l-0.1.2/micropython_qmc5883l.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-07 13:37:06.000000 micropython-qmc5883l-0.1.2/micropython_qmc5883l.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:37:06.000000 micropython-qmc5883l-0.1.2/micropython_qmc5883l.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 13:37:06.000000 micropython-qmc5883l-0.1.2/micropython_qmc5883l.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-07 13:36:57.000000 micropython-qmc5883l-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:36:48.000000 micropython-qmc5883l-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:37:06.128467 micropython-qmc5883l-0.1.2/setup.cfg
```

### Comparing `micropython-qmc5883l-0.1.1/.pre-commit-config.yaml` & `micropython-qmc5883l-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-qmc5883l-0.1.1/.pylintrc` & `micropython-qmc5883l-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.1/LICENSE` & `micropython-qmc5883l-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.1/PKG-INFO` & `micropython-qmc5883l-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-qmc5883l
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the QMC5883L Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_QMC5883L
-Keywords: sensor,micropython,qmc5883l,acceleration,heading,driver,sensor,gravity,micropython,accelerometer
+Keywords: sensor,micropython,qmc5883l,acceleration,heading,driver,gravity,accelerometer
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-qmc5883l-0.1.1/README.rst` & `micropython-qmc5883l-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.1/docs/_static/Logo.png` & `micropython-qmc5883l-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.1/docs/conf.py` & `micropython-qmc5883l-0.1.2/docs/conf.py`

 * *Files 24% similar despite different names*

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
+    import micropython_qmc5883l
+except ImportError:
+    raise SystemExit("micropython_qmc5883l has to be importable")
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
-        "MicroPython_qmc5883l_Library.tex",
-        "MicroPython qmc5883l Library Documentation",
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
-        "MicroPython_qmc5883l_Library",
-        "MicroPython qmc5883l Library Documentation",
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
-        "MicroPython_qmc5883l_Library",
-        "MicroPython qmc5883l Library Documentation",
-        author,
-        "MicroPython_qmc5883l_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-qmc5883l-0.1.1/docs/examples.rst` & `micropython-qmc5883l-0.1.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.1/examples/qmc5883l_advanced_settings.py` & `micropython-qmc5883l-0.1.2/examples/qmc5883l_advanced_settings.py`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.1/examples/qmc5883l_data_rate.py` & `micropython-qmc5883l-0.1.2/examples/qmc5883l_data_rate.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 qmc = qmc5883l.QMC5883L(i2c)
 
 while True:
     for data_rate in qmc5883l.data_rate_values:
         print("Current Data Rate Setting: ", qmc.output_data_rate)
         for _ in range(10):
             mag_x, mag_y, mag_z = qmc.magnetic
-            print("x:{:.2f}Gs, y:{:.2f}Gs, z{:.2f}Gs".format(mag_x, mag_y, mag_z))
+            print(f"x:{mag_x:.2f}Gs, y:{mag_y:.2f}Gs, z{mag_z:.2f}Gs")
             time.sleep(0.5)
         qmc.output_data_rate = data_rate
```

### Comparing `micropython-qmc5883l-0.1.1/examples/qmc5883l_field_range.py` & `micropython-qmc5883l-0.1.2/examples/qmc5883l_field_range.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 qmc = qmc5883l.QMC5883L(i2c)
 
 while True:
     for field_range in qmc5883l.field_range_values:
         print("Current Field Range Setting: ", qmc.field_range)
         for _ in range(10):
             mag_x, mag_y, mag_z = qmc.magnetic
-            print("x:{:.2f}Gs, y:{:.2f}Gs, z{:.2f}Gs".format(mag_x, mag_y, mag_z))
+            print(f"x:{mag_x:.2f}Gs, y:{mag_y:.2f}Gs, z{mag_z:.2f}Gs")
             time.sleep(0.5)
         qmc.field_range = field_range
```

### Comparing `micropython-qmc5883l-0.1.1/micropython_qmc5883l/i2c_helpers.py` & `micropython-qmc5883l-0.1.2/micropython_qmc5883l/i2c_helpers.py`

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

### Comparing `micropython-qmc5883l-0.1.1/micropython_qmc5883l/qmc5883l.py` & `micropython-qmc5883l-0.1.2/micropython_qmc5883l/qmc5883l.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 """
 
 import time
 from micropython import const
 from micropython_qmc5883l.i2c_helpers import CBits, RegisterStruct
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_QMC5883L.git"
 
 _REG_WHOAMI = const(0x0D)
 _REG_SET_RESET = const(0x0B)
 _REG_OPERATION_MODE = const(0x09)
 _REG_STATUS = const(0x06)
 
@@ -65,21 +65,21 @@
 
     Here is an example of using the :class:`QMC5883L` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import qmc5883l
+        from micropython_qmc5883l import qmc5883l
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         qmc5883l = qmc5883l.QMC5883L(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
         mag_x, mag_y, mag_z = qmc.magnetic
@@ -256,15 +256,14 @@
             "OUTPUT_DATA_RATE_200",
         )
 
         return rates[self._output_data_rate]
 
     @output_data_rate.setter
     def output_data_rate(self, value: int) -> None:
-
         if value not in data_rate_values:
             raise ValueError("Value must be a valid data rate setting")
 
         self._output_data_rate = value
 
     @property
     def mode_control(self) -> int:
```

### Comparing `micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/PKG-INFO` & `micropython-qmc5883l-0.1.2/micropython_qmc5883l.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-qmc5883l
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the QMC5883L Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_QMC5883L
-Keywords: sensor,micropython,qmc5883l,acceleration,heading,driver,sensor,gravity,micropython,accelerometer
+Keywords: sensor,micropython,qmc5883l,acceleration,heading,driver,gravity,accelerometer
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/SOURCES.txt` & `micropython-qmc5883l-0.1.2/micropython_qmc5883l.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 LICENSE
 README.rst
 examples.json
-packages.json
+package.json
 pyproject.toml
 requirements.txt
 .github/workflows/release_pypi.yml
 docs/api.rst
 docs/conf.py
 docs/examples.rst
 docs/index.rst
@@ -28,9 +28,8 @@
 examples/qmc5883l_simpletest.py
 micropython_qmc5883l/__init__.py
 micropython_qmc5883l/i2c_helpers.py
 micropython_qmc5883l/qmc5883l.py
 micropython_qmc5883l.egg-info/PKG-INFO
 micropython_qmc5883l.egg-info/SOURCES.txt
 micropython_qmc5883l.egg-info/dependency_links.txt
-micropython_qmc5883l.egg-info/requires.txt
 micropython_qmc5883l.egg-info/top_level.txt
```

### Comparing `micropython-qmc5883l-0.1.1/pyproject.toml` & `micropython-qmc5883l-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,41 +8,39 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-qmc5883l"
 description = "MicroPython Driver for the QMC5883L Accelerometer"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_QMC5883L"}
 keywords = [
     "sensor",
     "micropython",
     "qmc5883l",
     "acceleration",
     "heading",
     "driver",
-    "sensor",
     "gravity",
-    "micropython",
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
-py-modules = ["qmc5883l"]
+packages = ["micropython_qmc5883l"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

