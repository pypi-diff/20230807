# Comparing `tmp/micropython-dps310-0.1.1.tar.gz` & `tmp/micropython-dps310-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-dps310-0.1.1.tar", last modified: Sat Jun 17 15:23:28 2023, max compression
+gzip compressed data, was "micropython-dps310-0.1.2.tar", last modified: Mon Aug  7 13:50:55 2023, max compression
```

## Comparing `micropython-dps310-0.1.1.tar` & `micropython-dps310-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.080263 micropython-dps310-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.072263 micropython-dps310-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/examples/dps310_advanced.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/examples/dps310_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/examples/dps310_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/micropython_dps310/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/micropython_dps310/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23255 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/micropython_dps310/dps310.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/micropython_dps310/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/micropython_dps310.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-17 15:23:28.000000 micropython-dps310-0.1.1/micropython_dps310.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-17 15:23:28.000000 micropython-dps310-0.1.1/micropython_dps310.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:23:28.000000 micropython-dps310-0.1.1/micropython_dps310.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 15:23:28.000000 micropython-dps310-0.1.1/micropython_dps310.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 15:23:28.000000 micropython-dps310-0.1.1/micropython_dps310.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:23:28.080263 micropython-dps310-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:55.683752 micropython-dps310-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:55.679751 micropython-dps310-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:55.683752 micropython-dps310-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-07 13:50:55.683752 micropython-dps310-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:55.683752 micropython-dps310-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:55.683752 micropython-dps310-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:55.683752 micropython-dps310-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-07 13:50:48.000000 micropython-dps310-0.1.2/examples/dps310_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-07 13:50:48.000000 micropython-dps310-0.1.2/examples/dps310_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-07 13:50:48.000000 micropython-dps310-0.1.2/examples/dps310_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:55.683752 micropython-dps310-0.1.2/micropython_dps310/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:48.000000 micropython-dps310-0.1.2/micropython_dps310/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23717 2023-08-07 13:50:48.000000 micropython-dps310-0.1.2/micropython_dps310/dps310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-07 13:50:48.000000 micropython-dps310-0.1.2/micropython_dps310/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:55.683752 micropython-dps310-0.1.2/micropython_dps310.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-07 13:50:55.000000 micropython-dps310-0.1.2/micropython_dps310.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-07 13:50:55.000000 micropython-dps310-0.1.2/micropython_dps310.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:50:55.000000 micropython-dps310-0.1.2/micropython_dps310.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 13:50:55.000000 micropython-dps310-0.1.2/micropython_dps310.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-07 13:50:48.000000 micropython-dps310-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:50:40.000000 micropython-dps310-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:50:55.683752 micropython-dps310-0.1.2/setup.cfg
```

### Comparing `micropython-dps310-0.1.1/.pre-commit-config.yaml` & `micropython-dps310-0.1.2/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-# SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
+# SPDX-FileCopyrightText: 2023 Jose D. Montoya
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

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `micropython-dps310-0.1.1/LICENSE` & `micropython-dps310-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-dps310-0.1.1/PKG-INFO` & `micropython-dps310-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: micropython-dps310
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the DPS310 sensor
 Author-email: "Jose D. Montoya" <dps310@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_dps310
 Keywords: micropython,dps310,DPS310,sensor,temperature,pressure,altitude
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 
 .. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
```

### Comparing `micropython-dps310-0.1.1/README.rst` & `micropython-dps310-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-dps310-0.1.1/docs/_static/Logo.png` & `micropython-dps310-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-dps310-0.1.1/docs/_static/favicon.ico` & `micropython-dps310-0.1.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-dps310-0.1.1/docs/conf.py` & `micropython-dps310-0.1.2/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,21 +6,37 @@
 
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
+    import micropython_dps310
+except ImportError:
+    raise SystemExit("micropython_dps310 has to be importable")
+
 # -- General configuration ------------------------------------------------
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
-    "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "sphinx_immaterial",
 ]
 
 autodoc_preserve_defaults = True
 
 intersphinx_mapping = {
@@ -196,64 +212,7 @@
 # pixels large.
 #
 html_favicon = "_static/favicon.ico"
 
 html_logo = "_static/Logo.png"
 # Output file base name for HTML help builder.
 htmlhelp_basename = "MicroPython_Dps310_Librarydoc"
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
-        "MicroPython_dps310_Library.tex",
-        "MicroPython dps310 Library Documentation",
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
-        "MicroPython_dps310_Library",
-        "MicroPython dps310 Library Documentation",
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
-        "MicroPython_dps310_Library",
-        "MicroPython dps310 Library Documentation",
-        author,
-        "MicroPython_dps310_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-dps310-0.1.1/docs/examples.rst` & `micropython-dps310-0.1.2/docs/examples.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Simple test
 ------------
 
 Ensure your device works with this simple test.
 
 .. literalinclude:: ../examples/dps310_simpletest.py
     :caption: examples/dps310_simpletest.py
-    :linenos:
+    :lines: 3-
 
 Temperature test
 ----------------
 
 Example showing how to use the sensor temperture
 
 .. literalinclude:: ../examples/dps310_temperature.py
     :caption: examples/dps310_temperature.py
-    :linenos:
+    :lines: 3-
 
 Advanced Options
 ----------------
 
 Example showing how to use the advanced options
 
 .. literalinclude:: ../examples/dps310_simpletest.py
     :caption: examples/dps310_simpletest.py
-    :linenos:
+    :lines: 3-
```

### Comparing `micropython-dps310-0.1.1/examples/dps310_advanced.py` & `micropython-dps310-0.1.2/examples/dps310_advanced.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 
 from machine import Pin, I2C
-import dps310
+from micropython_dps310 import dps310
 
 i2c = I2C(sda=Pin(8), scl=Pin(9))  # Correct I2C pins for UM FeatherS2
 dps = dps310.DPS310(i2c)
 
 print("Current Pressure Oversample Configuration: ", dps.pressure_oversample)
 print("Current Pressure Rate Configuration:  ", dps.pressure_rate)
 dps.pressure_oversample = dps310.SAMPLE_PER_SECOND_64
```

### Comparing `micropython-dps310-0.1.1/micropython_dps310/dps310.py` & `micropython-dps310-0.1.2/micropython_dps310/dps310.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,30 +15,27 @@
 
 **Software and Dependencies:**
 
 This library depends on Micropython
 
 """
 
-# pylint: disable=too-many-arguments, line-too-long, too-many-instance-attributes
+# pylint: disable=line-too-long
 
 import time
 import math
+import struct
 from micropython import const
 from micropython_dps310.i2c_helpers import CBits, RegisterStruct
 
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_DPS310.git"
 
-_REG_WHOAMI = const(0x77)
+
 _DEVICE_ID = const(0x0D)
 _PRS_CFG = const(0x06)
 _TMP_CFG = const(0x07)
 _MEAS_CFG = const(0x08)
 _CFGREG = const(0x09)
 _RESET = const(0x0C)
 
@@ -59,16 +56,15 @@
     SAMPLE_PER_SECOND_4,
     SAMPLE_PER_SECOND_8,
     SAMPLE_PER_SECOND_16,
     SAMPLE_PER_SECOND_32,
     SAMPLE_PER_SECOND_64,
     SAMPLE_PER_SECOND_128,
 )
-# ** Note: For Pressure to be used in combination with a bit shift. See Interrupt
-# and FIFO configuration (CFG_REG) register
+
 
 # DPS310 Pressure Sample Rate
 RATE_1_HZ = const(0b000)
 RATE_2_HZ = const(0b001)
 RATE_4_HZ = const(0b010)
 RATE_8_HZ = const(0b011)
 RATE_16_HZ = const(0b100)
@@ -88,14 +84,22 @@
 
 IDLE = const(0b000)
 ONE_PRESSURE = const(0b001)
 ONE_TEMPERATURE = const(0b010)
 CONT_PRESSURE = const(0b101)
 CONT_TEMP = const(0b110)
 CONT_PRESTEMP = const(0b111)
+mode_values = (
+    IDLE,
+    ONE_PRESSURE,
+    ONE_TEMPERATURE,
+    CONT_PRESSURE,
+    CONT_TEMP,
+    CONT_PRESTEMP,
+)
 
 
 class DPS310:
     """Main class for the Sensor
 
     :param ~machine.I2C i2c: The I2C bus the DPS310 is connected to.
     :param int address: The I2C device address. Defaults to :const:`0x77`
@@ -113,15 +117,15 @@
         from machine import Pin, I2C
         import micropython_dps310.dps310 as dps310
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin(8), scl=Pin(9))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         dps = dps310.DPS310(i2c)
 
     Now you have access to the :attr:`pressure` attribute
 
     .. code-block:: python
 
         press = dps.pressure
@@ -179,33 +183,33 @@
         7: 206.8,
     }
 
     _calib_coeff_temp_src_bit = CBits(1, _TMPCOEFSRCE, 7)
 
     _soft_reset = CBits(4, 0x0C, 0)
 
-    def __init__(self, i2c, address=_REG_WHOAMI):
+    def __init__(self, i2c, address=0x77) -> None:
         self._i2c = i2c
         self._address = address
 
         if self._device_id != 0x10:
             raise RuntimeError("Failed to find the DPS310 sensor!")
 
         self._pressure_scale = None
         self._temp_scale = None
 
         self._oversample_scalefactor = (
-            524288,
-            1572864,
-            3670016,
-            7864320,
-            253952,
-            516096,
-            1040384,
-            2088960,
+            524288.0,
+            1572864.0,
+            3670016.0,
+            7864320.0,
+            253952.0,
+            516096.0,
+            1040384.0,
+            2088960.0,
         )
         self._sea_level_pressure = 1013.25
 
         self._correct_temp()
         self._read_calibration()
         self._temp_measurement_src_bit = self._calib_coeff_temp_src_bit
 
@@ -213,15 +217,15 @@
         self.temperature_oversample = RATE_64_HZ
         self._sensor_mode = CONT_PRESTEMP
 
         self._wait_temperature_ready()
         self._wait_pressure_ready()
 
     @property
-    def pressure_oversample(self):
+    def pressure_oversample(self) -> str:
         """
         Pressure Oversample. In order to achieve a higher precision, the sensor DPS310
         will read multiple times ( oversampling ), and combine the readings into one result.
         This increases the current consumption and also the measurement time, reducing the
         maximum possible measurement rate. It is necessary to balance the accuracy and data rate
         required for each application with the allowable current consumption.
 
@@ -241,37 +245,36 @@
         | :py:const:`dps310.SAMPLE_PER_SECOND_32`  | :py:const:`0b101`  # 32 times **                                  |
         +------------------------------------------+-------------------------------------------------------------------+
         | :py:const:`dps310.SAMPLE_PER_SECOND_64`  | :py:const:`0b110`  # 64 times (Pressure High Precision) **        |
         +------------------------------------------+-------------------------------------------------------------------+
         | :py:const:`dps310.SAMPLE_PER_SECOND_128` | :py:const:`0b111`  # 128 times **                                 |
         +------------------------------------------+-------------------------------------------------------------------+
         """
-
-        oversamples = {
-            0: "SAMPLE_PER_SECOND_1",
-            1: "SAMPLE_PER_SECOND_2",
-            2: "SAMPLE_PER_SECOND_4",
-            3: "SAMPLE_PER_SECOND_8",
-            4: "SAMPLE_PER_SECOND_16",
-            5: "SAMPLE_PER_SECOND_32",
-            6: "SAMPLE_PER_SECOND_64",
-            7: "SAMPLE_PER_SECOND_128",
-        }
-        return oversamples[self._pressure_oversample]
+        values = (
+            "SAMPLE_PER_SECOND_1",
+            "SAMPLE_PER_SECOND_2",
+            "SAMPLE_PER_SECOND_4",
+            "SAMPLE_PER_SECOND_8",
+            "SAMPLE_PER_SECOND_16",
+            "SAMPLE_PER_SECOND_32",
+            "SAMPLE_PER_SECOND_64",
+            "SAMPLE_PER_SECOND_128",
+        )
+        return values[self._pressure_oversample]
 
     @pressure_oversample.setter
-    def pressure_oversample(self, value: int):
+    def pressure_oversample(self, value: int) -> None:
         if value not in oversamples_values:
             raise ValueError("Value must be a valid oversample setting")
         self._pressure_oversample = value
         self._p_shift = value > SAMPLE_PER_SECOND_8
         self._pressure_scale = self._oversample_scalefactor[value]
 
     @property
-    def pressure_rate(self):
+    def pressure_rate(self) -> str:
         """
         +--------------------------------+--------------------------+
         | Mode                           | Value                    |
         +================================+==========================+
         | :py:const:`dps310.RATE_1_HZ`   | :py:const:`0b000`        |
         +--------------------------------+--------------------------+
         | :py:const:`dps310.RATE_2_HZ`   | :py:const:`0b001`        |
@@ -286,34 +289,34 @@
         +--------------------------------+--------------------------+
         | :py:const:`dps310.RATE_64_HZ`  | :py:const:`0b110`        |
         +--------------------------------+--------------------------+
         | :py:const:`dps310.RATE_128_HZ` | :py:const:`0b111`        |
         +--------------------------------+--------------------------+
         """
 
-        rates = {
-            0: "RATE_1_HZ",
-            1: "RATE_2_HZ",
-            2: "RATE_4_HZ",
-            3: "RATE_8_HZ",
-            4: "RATE_16_HZ",
-            5: "RATE_32_HZ",
-            6: "RATE_64_HZ",
-            7: "RATE_128_HZ",
-        }
-        return rates[self._pressure_rate]
+        values = (
+            "RATE_1_HZ",
+            "RATE_2_HZ",
+            "RATE_4_HZ",
+            "RATE_8_HZ",
+            "RATE_16_HZ",
+            "RATE_32_HZ",
+            "RATE_64_HZ",
+            "RATE_128_HZ",
+        )
+        return values[self._pressure_rate]
 
     @pressure_rate.setter
-    def pressure_rate(self, value: int):
+    def pressure_rate(self, value: int) -> None:
         if value not in rates_values:
             raise ValueError("Value must be a valid rate setting")
         self._pressure_rate = value
 
     @property
-    def temperature_oversample(self):
+    def temperature_oversample(self) -> str:
         """
         Temperature Oversample. In order to achieve a higher precision, the sensor DPS310
         will read multiple times ( oversampling ), and combine the readings into one result.
         This increases the current consumption and also the measurement time, reducing the
         maximum possible measurement rate. It is necessary to balance the accuracy and data rate
         required for each application with the allowable current consumption.
 
@@ -333,26 +336,36 @@
         | :py:const:`dps310.SAMPLE_PER_SECOND_32`  | :py:const:`0b101`  # 32 times         |
         +------------------------------------------+---------------------------------------+
         | :py:const:`dps310.SAMPLE_PER_SECOND_64`  | :py:const:`0b110`  # 64 times         |
         +------------------------------------------+---------------------------------------+
         | :py:const:`dps310.SAMPLE_PER_SECOND_128` | :py:const:`0b111`  # 128 times        |
         +------------------------------------------+---------------------------------------+
         """
-        return oversamples_values[self._temperature_oversample]
+        values = (
+            "SAMPLE_PER_SECOND_1",
+            "SAMPLE_PER_SECOND_2",
+            "SAMPLE_PER_SECOND_4",
+            "SAMPLE_PER_SECOND_8",
+            "SAMPLE_PER_SECOND_16",
+            "SAMPLE_PER_SECOND_32",
+            "SAMPLE_PER_SECOND_64",
+            "SAMPLE_PER_SECOND_128",
+        )
+        return values[self._temperature_oversample]
 
     @temperature_oversample.setter
-    def temperature_oversample(self, value: int):
+    def temperature_oversample(self, value: int) -> None:
         if value not in oversamples_values:
             raise ValueError("Value must be a valid oversample setting")
         self._temperature_oversample = value
         self._temp_scale = self._oversample_scalefactor[value]
         self._t_shift = value > SAMPLE_PER_SECOND_8
 
     @property
-    def temperature_rate(self):
+    def temperature_rate(self) -> str:
         """
         +--------------------------------+--------------------------+
         | Mode                           | Value                    |
         +================================+==========================+
         | :py:const:`dps310.RATE_1_HZ`   | :py:const:`0b000`        |
         +--------------------------------+--------------------------+
         | :py:const:`dps310.RATE_2_HZ`   | :py:const:`0b001`        |
@@ -366,35 +379,36 @@
         | :py:const:`dps310.RATE_32_HZ`  | :py:const:`0b101`        |
         +--------------------------------+--------------------------+
         | :py:const:`dps310.RATE_64_HZ`  | :py:const:`0b110`        |
         +--------------------------------+--------------------------+
         | :py:const:`dps310.RATE_128_HZ` | :py:const:`0b111`        |
         +--------------------------------+--------------------------+
         """
-        rates = {
-            0: "RATE_1_HZ",
-            1: "RATE_2_HZ",
-            2: "RATE_4_HZ",
-            3: "RATE_8_HZ",
-            4: "RATE_16_HZ",
-            5: "RATE_32_HZ",
-            6: "RATE_64_HZ",
-            7: "RATE_128_HZ",
-        }
 
-        return rates[self._temperature_rate]
+        values = (
+            "RATE_1_HZ",
+            "RATE_2_HZ",
+            "RATE_4_HZ",
+            "RATE_8_HZ",
+            "RATE_16_HZ",
+            "RATE_32_HZ",
+            "RATE_64_HZ",
+            "RATE_128_HZ",
+        )
+
+        return values[self._temperature_rate]
 
     @temperature_rate.setter
-    def temperature_rate(self, value: int):
+    def temperature_rate(self, value: int) -> None:
         if value not in rates_values:
             raise ValueError("Value must be a valid rate setting")
         self._temperature_rate = value
 
     @property
-    def mode(self):
+    def mode(self) -> str:
         """
         +------------------------------------+------------------------------------------------------------------+
         | Mode                               | Description                                                      |
         +------------------------------------+------------------------------------------------------------------+
         | :py:const:`dps310.IDLE`            | Puts the sensor into a shutdown state                            |
         +------------------------------------+------------------------------------------------------------------+
         | :py:const:`dps310.ONE_PRESSURE`    | Setting `mode` to ``dps310.ONE_PRESSURE`` takes a single pressure|
@@ -411,46 +425,56 @@
         +------------------------------------+------------------------------------------------------------------+
         | :py:const:`dps310.CONT_PRESTEMP`   | Take temperature and pressure measurements at the current        |
         |                                    | `pressure_rate` and `temperature_rate`                           |
         +------------------------------------+------------------------------------------------------------------+
 
 
         """
-        return self._sensor_mode
+        values = (
+            "IDLE",
+            "ONE_PRESSURE",
+            "ONE_TEMPERATURE",
+            "CONT_PRESSURE",
+            "CONT_TEMP",
+            "CONT_PRESTEMP",
+        )
+        return values[self._sensor_mode]
 
     @mode.setter
-    def mode(self, value: int):
+    def mode(self, value: int) -> None:
         self._sensor_mode = value
 
     def _wait_pressure_ready(self) -> None:
         """Wait until a pressure measurement is available. To avoid waiting indefinitely
         this function raises an error if the sensor isn't configured for pressure measurements,
 
         """
         if self.mode in (IDLE, ONE_TEMPERATURE, CONT_TEMP):
             raise RuntimeError(
                 "Sensor mode is set to idle or temperature measurement, can't wait for a pressure measurement"
             )
         while self._pressure_ready is False:
             time.sleep(0.001)
 
-    def _wait_temperature_ready(self):
+    def _wait_temperature_ready(self) -> None:
         """Wait until a temperature measurement is available.
         To avoid waiting indefinitely this function raises an
         error if the sensor isn't configured for temperate measurements,
         """
         if self.mode in (IDLE, ONE_PRESSURE, CONT_PRESSURE):
             raise RuntimeError(
                 "Sensor mode is set to idle or pressure measurement, can't wait for a temperature measurement"
             )
         while self._temp_ready is False:
             time.sleep(0.001)
 
     def _read_calibration(self) -> None:
-
+        """
+        Read the calibration data from the sensor
+        """
         while not self._coefficients_ready:
             time.sleep(0.001)
 
         coeffs = [None] * 18
         for offset in range(18):
             register = 0x10 + offset
             coeffs[offset] = struct.unpack(
@@ -516,17 +540,17 @@
 
         final_pressure = pres_calc / 100
 
         return final_pressure
 
     @property
     def altitude(self) -> float:
-        """The altitude in meters based on the sea level pressure
-        (:attr:`sea_level_pressure`) - which you must enter
-        ahead of time
+        """
+        The altitude in meters based on the sea level pressure
+        (:attr:`sea_level_pressure`) - which you must enter ahead of time
         """
         return 44330 * (
             1.0 - math.pow(self.pressure / self._sea_level_pressure, 0.1903)
         )
 
     @property
     def temperature(self) -> float:
```

### Comparing `micropython-dps310-0.1.1/micropython_dps310/i2c_helpers.py` & `micropython-dps310-0.1.2/micropython_dps310/i2c_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,18 +34,15 @@
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
 
@@ -64,30 +61,28 @@
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
@@ -112,15 +107,14 @@
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
@@ -130,15 +124,15 @@
                 memoryview(
                     obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
                 ),
             )
         return value
 
     def __set__(self, obj, value):
-        mem_value = value.to_bytes(self.lenght, "big")
+        mem_value = struct.pack(self.format, value)
         obj._i2c.writeto_mem(obj._address, self.register, mem_value)
 
 
 def twos_complement(val: int, bits: int) -> int:
     """
     Two complements
     """
```

### Comparing `micropython-dps310-0.1.1/micropython_dps310.egg-info/PKG-INFO` & `micropython-dps310-0.1.2/micropython_dps310.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: micropython-dps310
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the DPS310 sensor
 Author-email: "Jose D. Montoya" <dps310@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_dps310
 Keywords: micropython,dps310,DPS310,sensor,temperature,pressure,altitude
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 
 .. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
```

### Comparing `micropython-dps310-0.1.1/micropython_dps310.egg-info/SOURCES.txt` & `micropython-dps310-0.1.2/micropython_dps310.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 LICENSE
 README.rst
 examples.json
-optional_requirements.txt
-packages.json
+package.json
 pyproject.toml
 requirements.txt
 .github/workflows/release_pypi.yml
 docs/api.rst
 docs/conf.py
 docs/examples.rst
 docs/index.rst
@@ -24,9 +23,8 @@
 examples/dps310_temperature.py
 micropython_dps310/__init__.py
 micropython_dps310/dps310.py
 micropython_dps310/i2c_helpers.py
 micropython_dps310.egg-info/PKG-INFO
 micropython_dps310.egg-info/SOURCES.txt
 micropython_dps310.egg-info/dependency_links.txt
-micropython_dps310.egg-info/requires.txt
 micropython_dps310.egg-info/top_level.txt
```

