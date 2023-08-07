# Comparing `tmp/micropython-bmi160-0.1.1.tar.gz` & `tmp/micropython-bmi160-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-bmi160-0.1.1.tar", last modified: Sat Jun 17 15:33:04 2023, max compression
+gzip compressed data, was "micropython-bmi160-0.1.2.tar", last modified: Mon Aug  7 13:46:09 2023, max compression
```

## Comparing `micropython-bmi160-0.1.1.tar` & `micropython-bmi160-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.712855 micropython-bmi160-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.704855 micropython-bmi160-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.708855 micropython-bmi160-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-17 15:33:04.712855 micropython-bmi160-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.708855 micropython-bmi160-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.708855 micropython-bmi160-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.708855 micropython-bmi160-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_acc_datarate.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_acce_datarange.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_gyro_datarate.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_gyro_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_gyro_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.708855 micropython-bmi160-0.1.1/micropython_bmi160/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/micropython_bmi160/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26971 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/micropython_bmi160/bmi160.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/micropython_bmi160/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.712855 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-17 15:33:04.000000 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-17 15:33:04.000000 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:33:04.000000 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:33:04.000000 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 15:33:04.000000 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:33:04.712855 micropython-bmi160-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:09.203394 micropython-bmi160-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:09.191393 micropython-bmi160-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:09.195393 micropython-bmi160-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-07 13:46:09.203394 micropython-bmi160-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:09.195393 micropython-bmi160-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:09.199393 micropython-bmi160-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:09.199393 micropython-bmi160-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-07 13:46:00.000000 micropython-bmi160-0.1.2/examples/bmi160_acc_datarate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-07 13:46:00.000000 micropython-bmi160-0.1.2/examples/bmi160_acce_datarange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-07 13:46:00.000000 micropython-bmi160-0.1.2/examples/bmi160_gyro_datarate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-07 13:46:00.000000 micropython-bmi160-0.1.2/examples/bmi160_gyro_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-07 13:46:00.000000 micropython-bmi160-0.1.2/examples/bmi160_gyro_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-07 13:46:00.000000 micropython-bmi160-0.1.2/examples/bmi160_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-07 13:46:00.000000 micropython-bmi160-0.1.2/examples/bmi160_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:09.203394 micropython-bmi160-0.1.2/micropython_bmi160/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:00.000000 micropython-bmi160-0.1.2/micropython_bmi160/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27042 2023-08-07 13:46:00.000000 micropython-bmi160-0.1.2/micropython_bmi160/bmi160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-07 13:46:00.000000 micropython-bmi160-0.1.2/micropython_bmi160/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:09.203394 micropython-bmi160-0.1.2/micropython_bmi160.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-07 13:46:09.000000 micropython-bmi160-0.1.2/micropython_bmi160.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-07 13:46:09.000000 micropython-bmi160-0.1.2/micropython_bmi160.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:46:09.000000 micropython-bmi160-0.1.2/micropython_bmi160.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 13:46:09.000000 micropython-bmi160-0.1.2/micropython_bmi160.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-07 13:46:00.000000 micropython-bmi160-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:45:51.000000 micropython-bmi160-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:46:09.203394 micropython-bmi160-0.1.2/setup.cfg
```

### Comparing `micropython-bmi160-0.1.1/.pre-commit-config.yaml` & `micropython-bmi160-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-bmi160-0.1.1/.pylintrc` & `micropython-bmi160-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.1/LICENSE` & `micropython-bmi160-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.1/PKG-INFO` & `micropython-bmi160-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-bmi160
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Bosch BMI160 Acc/Gyro Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMI160
 Keywords: sensor,micropython,bmi160,gyro,acceleration,accelerometer,temperature,vector,gravity,micropython,rotation
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-bmi160-0.1.1/README.rst` & `micropython-bmi160-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.1/docs/_static/Logo.png` & `micropython-bmi160-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.1/docs/conf.py` & `micropython-bmi160-0.1.2/docs/conf.py`

 * *Files 24% similar despite different names*

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
+    import micropython_bmi160
+except ImportError:
+    raise SystemExit("micropython_bmi160 has to be importable")
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
-        "MicroPython_bmi160_Library.tex",
-        "MicroPython bmi160 Library Documentation",
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
-        "MicroPython_bmi160_Library",
-        "MicroPython bmi160 Library Documentation",
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
-        "MicroPython_bmi160_Library",
-        "MicroPython bmi160 Library Documentation",
-        author,
-        "MicroPython_bmi160_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-bmi160-0.1.1/docs/examples.rst` & `micropython-bmi160-0.1.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.1/examples/bmi160_acce_datarange.py` & `micropython-bmi160-0.1.2/examples/bmi160_acce_datarange.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 bmi.acceleration_range = bmi160.ACCEL_RANGE_4G
 
 while True:
     for data_range in bmi160.acc_range_values:
         print("Current Acceleration Data Rate: ", bmi.acceleration_range)
         for _ in range(10):
             accx, accy, accz = bmi.acceleration
-            print("x:{:.2f}m/s2, y:{:.2f}m/s2, z{:.2f}m/s2".format(accx, accy, accz))
+            print(f"x:{accx:.2f}m/s2, y:{accy:.2f}m/s2, z{accz:.2f}m/s2")
             time.sleep(0.5)
         bmi.acceleration_range = data_range
```

### Comparing `micropython-bmi160-0.1.1/examples/bmi160_gyro_datarate.py` & `micropython-bmi160-0.1.2/examples/bmi160_acc_datarate.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import time
 from machine import Pin, I2C
 from micropython_bmi160 import bmi160
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 bmi = bmi160.BMI160(i2c)
 
-bmi.gyro_output_data_rate = bmi160.BANDWIDTH_200
+bmi.acceleration_output_data_rate = bmi160.BANDWIDTH_25_32
 
 while True:
-    for data_rate in bmi160.gyro_bandwidth_values:
-        print("Current Gyro Data Range: ", bmi.gyro_output_data_rate)
+    for data_rate in bmi160.bandwidth_values:
+        print("Current Acceleration Data Rate: ", bmi.acceleration_output_data_rate)
         for _ in range(10):
-            gyrox, gyroy, gyroz = bmi.gyro
-            print("x:{:.2f}°/s, y:{:.2f}°/s, z{:.2f}°/s".format(gyrox, gyroy, gyroz))
+            accx, accy, accz = bmi.acceleration
+            print(f"x:{accx:.2f}m/s2, y:{accy:.2f}m/s2, z{accz:.2f}m/s2")
             time.sleep(0.5)
-        bmi.gyro_output_data_rate = data_rate
+        bmi.acceleration_output_data_rate = data_rate
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `micropython-bmi160-0.1.1/examples/bmi160_gyro_range.py` & `micropython-bmi160-0.1.2/examples/bmi160_gyro_datarate.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import time
 from machine import Pin, I2C
 from micropython_bmi160 import bmi160
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 bmi = bmi160.BMI160(i2c)
 
-bmi.gyro_range = bmi160.GYRO_RANGE_500
+bmi.gyro_output_data_rate = bmi160.BANDWIDTH_200
 
 while True:
-    for data_range in bmi160.gyro_values:
-        print("Current Gyro Data Range: ", bmi.gyro_range)
+    for data_rate in bmi160.gyro_bandwidth_values:
+        print("Current Gyro Data Range: ", bmi.gyro_output_data_rate)
         for _ in range(10):
             gyrox, gyroy, gyroz = bmi.gyro
-            print("x:{:.2f}°/s, y:{:.2f}°/s, z{:.2f}°/s".format(gyrox, gyroy, gyroz))
+            print(f"x:{gyrox:.2f}°/s, y:{gyroy:.2f}°/s, z{gyroz:.2f}°/s")
             time.sleep(0.5)
-        bmi.gyro_range = data_range
+        bmi.gyro_output_data_rate = data_rate
```

### Comparing `micropython-bmi160-0.1.1/examples/bmi160_simpletest.py` & `micropython-bmi160-0.1.2/examples/bmi160_gyro_range.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,13 +5,17 @@
 import time
 from machine import Pin, I2C
 from micropython_bmi160 import bmi160
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 bmi = bmi160.BMI160(i2c)
 
+bmi.gyro_range = bmi160.GYRO_RANGE_500
+
 while True:
-    accx, accy, accz = bmi.acceleration
-    print("x:{:.2f}m/s2, y:{:.2f}m/s2, z{:.2f}m/s2".format(accx, accy, accz))
-    gyrox, gyroy, gyroz = bmi.gyro
-    print("x:{:.2f}°/s, y:{:.2f}°/s, z{:.2f}°/s".format(gyrox, gyroy, gyroz))
-    time.sleep(0.5)
+    for data_range in bmi160.gyro_values:
+        print("Current Gyro Data Range: ", bmi.gyro_range)
+        for _ in range(10):
+            gyrox, gyroy, gyroz = bmi.gyro
+            print(f"x:{gyrox:.2f}°/s, y:{gyroy:.2f}°/s, z{gyroz:.2f}°/s")
+            time.sleep(0.5)
+        bmi.gyro_range = data_range
```

### Comparing `micropython-bmi160-0.1.1/examples.json` & `micropython-bmi160-0.1.2/examples.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'version'": "'1'"}*

```diff
@@ -25,9 +25,9 @@
             "github:jposada202020/MicroPython_BMI160/examples/bmi160_gyro_simpletest.py"
         ],
         [
             "micropython_bmi160/examples/bmi160_acc_datarate.py",
             "github:jposada202020/MicroPython_BMI160/examples/bmi160_acc_datarate.py"
         ]
     ],
-    "version": "0.1"
+    "version": "1"
 }
```

### Comparing `micropython-bmi160-0.1.1/micropython_bmi160/bmi160.py` & `micropython-bmi160-0.1.2/micropython_bmi160/bmi160.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMI160.git"
 
 
 _I2C_ADDR = const(0x69)
 _REG_WHOAMI = const(0x00)
 _ERROR_CODE = const(0x02)
 _COMMAND = const(0x7E)
@@ -137,14 +137,16 @@
     GYRO_RANGE_125,
     GYRO_RANGE_250,
     GYRO_RANGE_500,
     GYRO_RANGE_1000,
     GYRO_RANGE_2000,
 )
 
+_ACC_CONVERSION = const(9.80665)
+
 # pylint: disable= invalid-name
 
 
 class BMI160:
     """Driver for the BMI160 Sensor connected over I2C.
 
     :param ~machine.I2C i2c: The I2C bus the BMI160 is connected to.
@@ -156,21 +158,21 @@
 
     Here is an example of using the :class:`BMI160` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import bmi160
+        from micropython_bmi160 import bmi160
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         bmi160 = bmi160.BMI160(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
         accx, accy, accz = bmi.acceleration
@@ -291,16 +293,16 @@
         if fatal_error:
             print("Fatal Error")
 
     @property
     def acceleration_undersample(self) -> str:
         """
         The undersampling parameter is typically used in low power mode.
-        When acc_us is set to ‘0’ and the accelerometer is in low-power mode,
-        it will change to normal mode. If the acc_us is set to ‘0’ and a
+        When acc_us is set to '0' and the accelerometer is in low-power mode,
+        it will change to normal mode. If the acc_us is set to '0' and a
         command to enter low-power mode is sent to the Register (0x7E) CMD,
         this command is ignored.
 
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
         +========================================+=========================+
         | :py:const:`bmi160.NO_UNDERSAMPLE`      | :py:const:`0`           |
@@ -443,15 +445,15 @@
 
     @property
     def acceleration(self) -> Tuple[int, int, int]:
         """
         Sensor Acceleration
         """
 
-        factor = self.acceleration_scale[self.acceleration_range]
+        factor = self.acceleration_scale[self.acceleration_range] * _ACC_CONVERSION
 
         x = self._acc_data_x / factor
         y = self._acc_data_y / factor
         z = self._acc_data_z / factor
         return x, y, z
 
     def power_mode_status(self) -> None:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `micropython-bmi160-0.1.1/micropython_bmi160/i2c_helpers.py` & `micropython-bmi160-0.1.2/micropython_bmi160/i2c_helpers.py`

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

### Comparing `micropython-bmi160-0.1.1/micropython_bmi160.egg-info/PKG-INFO` & `micropython-bmi160-0.1.2/micropython_bmi160.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-bmi160
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Bosch BMI160 Acc/Gyro Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMI160
 Keywords: sensor,micropython,bmi160,gyro,acceleration,accelerometer,temperature,vector,gravity,micropython,rotation
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-bmi160-0.1.1/micropython_bmi160.egg-info/SOURCES.txt` & `micropython-bmi160-0.1.2/micropython_bmi160.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

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
 examples/bmi160_temperature.py
 micropython_bmi160/__init__.py
 micropython_bmi160/bmi160.py
 micropython_bmi160/i2c_helpers.py
 micropython_bmi160.egg-info/PKG-INFO
 micropython_bmi160.egg-info/SOURCES.txt
 micropython_bmi160.egg-info/dependency_links.txt
-micropython_bmi160.egg-info/requires.txt
 micropython_bmi160.egg-info/top_level.txt
```

### Comparing `micropython-bmi160-0.1.1/pyproject.toml` & `micropython-bmi160-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-bmi160"
 description = "MicroPython Driver for the Bosch BMI160 Acc/Gyro Sensor"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_BMI160"}
 keywords = [
     "sensor",
@@ -39,11 +39,11 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["bmi160"]
+packages = ["micropython_bmi160"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

