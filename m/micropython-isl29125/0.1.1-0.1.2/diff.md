# Comparing `tmp/micropython-isl29125-0.1.1.tar.gz` & `tmp/micropython-isl29125-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-isl29125-0.1.1.tar", last modified: Sat Jun 17 15:10:49 2023, max compression
+gzip compressed data, was "micropython-isl29125-0.1.2.tar", last modified: Mon Aug  7 13:44:29 2023, max compression
```

## Comparing `micropython-isl29125-0.1.1.tar` & `micropython-isl29125-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.070340 micropython-isl29125-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.070340 micropython-isl29125-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.070340 micropython-isl29125-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/examples/isl29125_ADC_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/examples/isl29125_operation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/examples/isl29125_rgb_sensing_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/examples/isl29125_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/examples/isl29125_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/micropython_isl29125/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/micropython_isl29125/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/micropython_isl29125/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/micropython_isl29125/isl29125.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-17 15:10:49.000000 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-17 15:10:49.000000 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:10:49.000000 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:10:49.000000 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 15:10:49.000000 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:44:29.006210 micropython-isl29125-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:44:29.002210 micropython-isl29125-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:44:29.002210 micropython-isl29125-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-08-07 13:44:29.006210 micropython-isl29125-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:44:29.002210 micropython-isl29125-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:44:29.006210 micropython-isl29125-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:44:29.006210 micropython-isl29125-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-07 13:44:21.000000 micropython-isl29125-0.1.2/examples/isl29125_ADC_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-07 13:44:21.000000 micropython-isl29125-0.1.2/examples/isl29125_operation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-07 13:44:21.000000 micropython-isl29125-0.1.2/examples/isl29125_rgb_sensing_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-07 13:44:21.000000 micropython-isl29125-0.1.2/examples/isl29125_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-07 13:44:21.000000 micropython-isl29125-0.1.2/examples/isl29125_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:44:29.006210 micropython-isl29125-0.1.2/micropython_isl29125/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:44:21.000000 micropython-isl29125-0.1.2/micropython_isl29125/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 13:44:21.000000 micropython-isl29125-0.1.2/micropython_isl29125/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-08-07 13:44:21.000000 micropython-isl29125-0.1.2/micropython_isl29125/isl29125.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:44:29.006210 micropython-isl29125-0.1.2/micropython_isl29125.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-08-07 13:44:28.000000 micropython-isl29125-0.1.2/micropython_isl29125.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:44:28.000000 micropython-isl29125-0.1.2/micropython_isl29125.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:44:28.000000 micropython-isl29125-0.1.2/micropython_isl29125.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 13:44:28.000000 micropython-isl29125-0.1.2/micropython_isl29125.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-07 13:44:21.000000 micropython-isl29125-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:44:12.000000 micropython-isl29125-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:44:29.006210 micropython-isl29125-0.1.2/setup.cfg
```

### Comparing `micropython-isl29125-0.1.1/.pre-commit-config.yaml` & `micropython-isl29125-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-isl29125-0.1.1/.pylintrc` & `micropython-isl29125-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.1/LICENSE` & `micropython-isl29125-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.1/PKG-INFO` & `micropython-isl29125-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-isl29125
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Intersil ISL29125 Color Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ISL29125
-Keywords: sensor,micropython,isl29125,color,sensor,intersil,RGB,mciropython,isl29125
+Keywords: sensor,micropython,color,sensor,intersil,RGB,isl29125
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-isl29125-0.1.1/README.rst` & `micropython-isl29125-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.1/docs/_static/Logo.png` & `micropython-isl29125-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.1/docs/conf.py` & `micropython-isl29125-0.1.2/docs/conf.py`

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
+    import micropython_isl29125
+except ImportError:
+    raise SystemExit("micropython_isl29125 has to be importable")
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
-        "MicroPython_isl29125_Library.tex",
-        "MicroPython isl29125 Library Documentation",
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
-        "MicroPython_isl29125_Library",
-        "MicroPython isl29125 Library Documentation",
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
-        "MicroPython_isl29125_Library",
-        "MicroPython isl29125 Library Documentation",
-        author,
-        "MicroPython_isl29125_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-isl29125-0.1.1/docs/examples.rst` & `micropython-isl29125-0.1.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.1/examples/isl29125_ADC_resolution.py` & `micropython-isl29125-0.1.2/examples/isl29125_ADC_resolution.py`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.1/examples/isl29125_operation_mode.py` & `micropython-isl29125-0.1.2/examples/isl29125_operation_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.1/examples/isl29125_rgb_sensing_range.py` & `micropython-isl29125-0.1.2/examples/isl29125_rgb_sensing_range.py`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.1/examples/isl29125_threshold.py` & `micropython-isl29125-0.1.2/examples/isl29125_threshold.py`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.1/examples.json` & `micropython-isl29125-0.1.2/examples.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'version'": "'1'"}*

```diff
@@ -17,9 +17,9 @@
             "github:jposada202020/MicroPython_ISL29125/examples/isl29125_rgb_sensing_range.py"
         ],
         [
             "micropython_isl29125/examples/isl29125_simpletest.py",
             "github:jposada202020/MicroPython_ISL29125/examples/isl29125_simpletest.py"
         ]
     ],
-    "version": "0.1"
+    "version": "1"
 }
```

### Comparing `micropython-isl29125-0.1.1/micropython_isl29125/i2c_helpers.py` & `micropython-isl29125-0.1.2/micropython_isl29125/i2c_helpers.py`

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

### Comparing `micropython-isl29125-0.1.1/micropython_isl29125/isl29125.py` & `micropython-isl29125-0.1.2/micropython_isl29125/isl29125.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 """
 
 from micropython import const
 from micropython_isl29125.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_ISL29125.git"
 
 _REG_WHOAMI = const(0x00)
 _CONFIG1 = const(0x01)
 _CONFIG2 = const(0x02)
 _CONFIG3 = const(0x03)
 _FLAG_REGISTER = const(0x08)
@@ -70,33 +70,33 @@
 persistent_control_values = (IC1, IC2, IC4, IC8)
 
 
 class ISL29125:
     """Driver for the ISL29125 Sensor connected over I2C.
 
     :param ~machine.I2C i2c: The I2C bus the ISL29125 is connected to.
-    :param int address: The I2C device address. Defaults to :const:`0x69`
+    :param int address: The I2C device address. Defaults to :const:`0x44`
 
     :raises RuntimeError: if the sensor is not found
 
     **Quickstart: Importing and using the device**
 
     Here is an example of using the :class:`ISL29125` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import isl29125
+        from micropython_isl29125 import isl29125
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         isl29125 = isl29125.ISL29125(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
     red, green, blue = isl.colors
```

### Comparing `micropython-isl29125-0.1.1/micropython_isl29125.egg-info/PKG-INFO` & `micropython-isl29125-0.1.2/micropython_isl29125.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-isl29125
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Intersil ISL29125 Color Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ISL29125
-Keywords: sensor,micropython,isl29125,color,sensor,intersil,RGB,mciropython,isl29125
+Keywords: sensor,micropython,color,sensor,intersil,RGB,isl29125
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-isl29125-0.1.1/micropython_isl29125.egg-info/SOURCES.txt` & `micropython-isl29125-0.1.2/micropython_isl29125.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

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
@@ -27,9 +27,8 @@
 examples/isl29125_threshold.py
 micropython_isl29125/__init__.py
 micropython_isl29125/i2c_helpers.py
 micropython_isl29125/isl29125.py
 micropython_isl29125.egg-info/PKG-INFO
 micropython_isl29125.egg-info/SOURCES.txt
 micropython_isl29125.egg-info/dependency_links.txt
-micropython_isl29125.egg-info/requires.txt
 micropython_isl29125.egg-info/top_level.txt
```

### Comparing `micropython-isl29125-0.1.1/pyproject.toml` & `micropython-isl29125-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -8,40 +8,38 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-isl29125"
 description = "MicroPython Driver for the Intersil ISL29125 Color Sensor"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_ISL29125"}
 keywords = [
     "sensor",
     "micropython",
-    "isl29125",
     "color",
     "sensor",
     "intersil",
     "RGB",
-    "mciropython",
     "isl29125",
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
-py-modules = ["isl29125"]
+packages = ["micropython_isl29125"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

