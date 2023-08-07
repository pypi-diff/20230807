# Comparing `tmp/micropython-kx132-0.1.1.tar.gz` & `tmp/micropython-kx132-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-kx132-0.1.1.tar", last modified: Sat Jun 17 15:07:29 2023, max compression
+gzip compressed data, was "micropython-kx132-0.1.2.tar", last modified: Mon Aug  7 13:53:32 2023, max compression
```

## Comparing `micropython-kx132-0.1.1.tar` & `micropython-kx132-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.907171 micropython-kx132-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.891171 micropython-kx132-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.895171 micropython-kx132-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-17 15:07:29.907171 micropython-kx132-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.899171 micropython-kx132-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.899171 micropython-kx132-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.903171 micropython-kx132-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_acc_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_adp_enabled.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_output_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_previous_tilt_position_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_tap_doubletap_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_tilt_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.907171 micropython-kx132-0.1.1/micropython_kx132/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/micropython_kx132/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/micropython_kx132/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/micropython_kx132/kx132.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.907171 micropython-kx132-0.1.1/micropython_kx132.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-17 15:07:29.000000 micropython-kx132-0.1.1/micropython_kx132.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-17 15:07:29.000000 micropython-kx132-0.1.1/micropython_kx132.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:07:29.000000 micropython-kx132-0.1.1/micropython_kx132.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:07:29.000000 micropython-kx132-0.1.1/micropython_kx132.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-17 15:07:29.000000 micropython-kx132-0.1.1/micropython_kx132.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:07:29.907171 micropython-kx132-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:32.335926 micropython-kx132-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:32.327926 micropython-kx132-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:32.327926 micropython-kx132-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-07 13:53:32.335926 micropython-kx132-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:32.331926 micropython-kx132-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:32.331926 micropython-kx132-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:32.331926 micropython-kx132-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-07 13:53:21.000000 micropython-kx132-0.1.2/examples/kx132_acc_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-07 13:53:21.000000 micropython-kx132-0.1.2/examples/kx132_adp_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-07 13:53:21.000000 micropython-kx132-0.1.2/examples/kx132_output_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-07 13:53:21.000000 micropython-kx132-0.1.2/examples/kx132_previous_tilt_position_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-07 13:53:21.000000 micropython-kx132-0.1.2/examples/kx132_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-07 13:53:21.000000 micropython-kx132-0.1.2/examples/kx132_tap_doubletap_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-07 13:53:21.000000 micropython-kx132-0.1.2/examples/kx132_tilt_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:32.331926 micropython-kx132-0.1.2/micropython_kx132/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:21.000000 micropython-kx132-0.1.2/micropython_kx132/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 13:53:21.000000 micropython-kx132-0.1.2/micropython_kx132/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-08-07 13:53:21.000000 micropython-kx132-0.1.2/micropython_kx132/kx132.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:32.335926 micropython-kx132-0.1.2/micropython_kx132.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-07 13:53:32.000000 micropython-kx132-0.1.2/micropython_kx132.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-07 13:53:32.000000 micropython-kx132-0.1.2/micropython_kx132.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:53:32.000000 micropython-kx132-0.1.2/micropython_kx132.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 13:53:32.000000 micropython-kx132-0.1.2/micropython_kx132.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-07 13:53:21.000000 micropython-kx132-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:53:08.000000 micropython-kx132-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:53:32.335926 micropython-kx132-0.1.2/setup.cfg
```

### Comparing `micropython-kx132-0.1.1/.pre-commit-config.yaml` & `micropython-kx132-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-kx132-0.1.1/.pylintrc` & `micropython-kx132-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.1/LICENSE` & `micropython-kx132-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.1/PKG-INFO` & `micropython-kx132-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-kx132
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Kionix KX132 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_KX132
 Keywords: sensor,micropython,kx132,acceleration
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-kx132-0.1.1/README.rst` & `micropython-kx132-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.1/docs/_static/Logo.png` & `micropython-kx132-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.1/docs/conf.py` & `micropython-kx132-0.1.2/docs/conf.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,20 +6,36 @@
 
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
+    import micropython_kx132
+except ImportError:
+    raise SystemExit("micropython_kx132 has to be importable")
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
@@ -182,65 +198,7 @@
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
-        "MicroPython_kx132_Library.tex",
-        "MicroPython kx132 Library Documentation",
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
-        "MicroPython_kx132_Library",
-        "MicroPython kx132 Library Documentation",
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
-        "MicroPython_kx132_Library",
-        "MicroPython kx132 Library Documentation",
-        author,
-        "MicroPython_kx132_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-kx132-0.1.1/docs/examples.rst` & `micropython-kx132-0.1.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.1/examples/kx132_acc_range.py` & `micropython-kx132-0.1.2/examples/kx132_acc_range.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 kx.acc_range = kx132.ACC_RANGE_16
 
 while True:
     for acc_range in kx132.acc_range_values:
         print("Current Acc range setting: ", kx.acc_range)
         for _ in range(10):
             accx, accy, accz = kx.acceleration
-            print("x:{:.2f}m/s2, y:{:.2f}m/s2, z:{:.2f}m/s2".format(accx, accy, accz))
+            print(f"x:{accx:.2f}g, y:{accy:.2f}g, z:{accz:.2f}g")
             time.sleep(0.5)
         kx.acc_range = acc_range
```

### Comparing `micropython-kx132-0.1.1/examples/kx132_adp_enabled.py` & `micropython-kx132-0.1.2/examples/kx132_adp_enabled.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 kx = kx132.KX132(i2c)
 
 while True:
     kx.adp_enabled = kx132.ADP_DISABLED
     print("Current ADP setting: ", kx.adp_enabled)
     for _ in range(10):
         adpx, adpy, adpz = kx.advanced_data_path
-        print("x:{:.2f}g, y:{:.2f}g, z:{:.2f}g".format(adpx, adpy, adpz))
+        print(f"x:{adpx:.2f}g, y:{adpy:.2f}g, z:{adpz:.2f}g")
         time.sleep(0.5)
     kx.adp_enabled = kx132.ADP_ENABLED
     print("Current ADP setting: ", kx.adp_enabled)
     for _ in range(10):
         adpx, adpy, adpz = kx.advanced_data_path
-        print("x:{:.2f}g, y:{:.2f}g, z:{:.2f}g".format(adpx, adpy, adpz))
+        print(f"x:{adpx:.2f}g, y:{adpy:.2f}g, z:{adpz:.2f}g")
         time.sleep(0.5)
     kx.soft_reset()
```

### Comparing `micropython-kx132-0.1.1/examples/kx132_output_data_rate.py` & `micropython-kx132-0.1.2/examples/kx132_output_data_rate.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 while True:
     kx.performance_mode = kx132.HIGH_PERFORMANCE_MODE
     kx.output_data_rate = 12  # 3200 Hz
     print("Current Performance Mode setting: ", kx.performance_mode)
     for _ in range(10):
         accx, accy, accz = kx.acceleration
-        print("x:{:.2f}m/s2, y:{:.2f}m/s2, z:{:.2f}m/s2".format(accx, accy, accz))
+        print(f"x:{accx:.2f}g, y:{accy:.2f}g, z:{accz:.2f}g")
         time.sleep(0.5)
     kx.performance_mode = kx132.LOW_POWER_MODE
     kx.output_data_rate = 3  # 6.25 Hz
     print("Current Performance Mode setting: ", kx.performance_mode)
     for _ in range(10):
         accx, accy, accz = kx.acceleration
-        print("x:{:.2f}m/s2, y:{:.2f}m/s2, z:{:.2f}m/s2".format(accx, accy, accz))
+        print(f"x:{accx:.2f}g, y:{accy:.2f}g, z:{accz:.2f}g")
         time.sleep(0.5)
```

### Comparing `micropython-kx132-0.1.1/examples.json` & `micropython-kx132-0.1.2/examples.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'version'": "'1'"}*

```diff
@@ -25,9 +25,9 @@
             "github:jposada202020/MicroPython_KX132/examples/kx132_simpletest.py"
         ],
         [
             "micropython_kx132/examples/kx132_output_data_rate.py",
             "github:jposada202020/MicroPython_KX132/examples/kx132_output_data_rate.py"
         ]
     ],
-    "version": "0.1"
+    "version": "1"
 }
```

### Comparing `micropython-kx132-0.1.1/micropython_kx132/i2c_helpers.py` & `micropython-kx132-0.1.2/micropython_kx132/i2c_helpers.py`

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

### Comparing `micropython-kx132-0.1.1/micropython_kx132/kx132.py` & `micropython-kx132-0.1.2/micropython_kx132/kx132.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_KX132.git"
 
 _ADP = const(0x02)
 _ACC = const(0x08)
 _REG_WHOAMI = const(0x13)
 _TILT_POSITION = const(0x14)
 _PREVIOUS_TILT_POSITION = const(0x15)
@@ -75,39 +75,41 @@
 # pylint: disable=too-many-instance-attributes
 
 
 class KX132:
     """Driver for the KX132 Sensor connected over I2C.
 
     :param ~machine.I2C i2c: The I2C bus the KX132 is connected to.
-    :param int address: The I2C device address. Defaults to :const:`0x69`
+    :param int address: The I2C device address. Defaults to :const:`0x1F`
 
     :raises RuntimeError: if the sensor is not found
 
     **Quickstart: Importing and using the device**
 
     Here is an example of using the :class:`KX132` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import kx132
+        from micropython_kx132 import kx132
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         kx132 = kx132.KX132(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
+        accx, accy, accz = kx132.acceleration
+
     """
 
     _device_id = RegisterStruct(_REG_WHOAMI, "B")
     _control_register1 = RegisterStruct(_CNTL1, "B")
     _interrupt1 = RegisterStruct(_INS1, "B")
     _interrupt_release = RegisterStruct(_INT_REL, "B")
```

### Comparing `micropython-kx132-0.1.1/micropython_kx132.egg-info/PKG-INFO` & `micropython-kx132-0.1.2/micropython_kx132.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-kx132
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Kionix KX132 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_KX132
 Keywords: sensor,micropython,kx132,acceleration
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-kx132-0.1.1/micropython_kx132.egg-info/SOURCES.txt` & `micropython-kx132-0.1.2/micropython_kx132.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

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
@@ -29,9 +29,8 @@
 examples/kx132_tilt_example.py
 micropython_kx132/__init__.py
 micropython_kx132/i2c_helpers.py
 micropython_kx132/kx132.py
 micropython_kx132.egg-info/PKG-INFO
 micropython_kx132.egg-info/SOURCES.txt
 micropython_kx132.egg-info/dependency_links.txt
-micropython_kx132.egg-info/requires.txt
 micropython_kx132.egg-info/top_level.txt
```

### Comparing `micropython-kx132-0.1.1/pyproject.toml` & `micropython-kx132-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-kx132"
 description = "MicroPython Driver for the Kionix KX132 Accelerometer"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_KX132"}
 keywords = [
     "sensor",
```

