# Comparing `tmp/micropython-bmp581-0.1.1.tar.gz` & `tmp/micropython-bmp581-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-bmp581-0.1.1.tar", last modified: Sat Jun 17 15:28:30 2023, max compression
+gzip compressed data, was "micropython-bmp581-0.1.2.tar", last modified: Mon Aug  7 13:53:01 2023, max compression
```

## Comparing `micropython-bmp581-0.1.1.tar` & `micropython-bmp581-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.499702 micropython-bmp581-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.503702 micropython-bmp581-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.503702 micropython-bmp581-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.503702 micropython-bmp581-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_output_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_power_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_pressure_oversample_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_temperature_oversample_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/micropython_bmp581/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/micropython_bmp581/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/micropython_bmp581/bmp581.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/micropython_bmp581/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-17 15:28:30.000000 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-17 15:28:30.000000 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:28:30.000000 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:28:30.000000 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 15:28:30.000000 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:01.404835 micropython-bmp581-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:01.396835 micropython-bmp581-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:01.400835 micropython-bmp581-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:52:45.000000 micropython-bmp581-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:52:45.000000 micropython-bmp581-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:52:45.000000 micropython-bmp581-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:52:45.000000 micropython-bmp581-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:52:45.000000 micropython-bmp581-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:52:45.000000 micropython-bmp581-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-07 13:53:01.400835 micropython-bmp581-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-08-07 13:52:45.000000 micropython-bmp581-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:01.400835 micropython-bmp581-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:01.400835 micropython-bmp581-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:52:45.000000 micropython-bmp581-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:52:45.000000 micropython-bmp581-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:52:45.000000 micropython-bmp581-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:52:45.000000 micropython-bmp581-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:52:46.000000 micropython-bmp581-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:52:46.000000 micropython-bmp581-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-07 13:52:46.000000 micropython-bmp581-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-08-07 13:52:46.000000 micropython-bmp581-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-07 13:52:46.000000 micropython-bmp581-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 13:52:46.000000 micropython-bmp581-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:52:46.000000 micropython-bmp581-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:01.400835 micropython-bmp581-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-07 13:52:53.000000 micropython-bmp581-0.1.2/examples/bmp581_altitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-07 13:52:53.000000 micropython-bmp581-0.1.2/examples/bmp581_output_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-07 13:52:53.000000 micropython-bmp581-0.1.2/examples/bmp581_power_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-07 13:52:53.000000 micropython-bmp581-0.1.2/examples/bmp581_pressure_oversample_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-07 13:52:53.000000 micropython-bmp581-0.1.2/examples/bmp581_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-07 13:52:53.000000 micropython-bmp581-0.1.2/examples/bmp581_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-07 13:52:53.000000 micropython-bmp581-0.1.2/examples/bmp581_temperature_oversample_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-07 13:52:46.000000 micropython-bmp581-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:01.400835 micropython-bmp581-0.1.2/micropython_bmp581/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:52:53.000000 micropython-bmp581-0.1.2/micropython_bmp581/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-07 13:52:53.000000 micropython-bmp581-0.1.2/micropython_bmp581/bmp581.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-07 13:52:53.000000 micropython-bmp581-0.1.2/micropython_bmp581/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:53:01.400835 micropython-bmp581-0.1.2/micropython_bmp581.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-07 13:53:01.000000 micropython-bmp581-0.1.2/micropython_bmp581.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-07 13:53:01.000000 micropython-bmp581-0.1.2/micropython_bmp581.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:53:01.000000 micropython-bmp581-0.1.2/micropython_bmp581.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 13:53:01.000000 micropython-bmp581-0.1.2/micropython_bmp581.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 13:52:46.000000 micropython-bmp581-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-07 13:52:53.000000 micropython-bmp581-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:52:46.000000 micropython-bmp581-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:53:01.404835 micropython-bmp581-0.1.2/setup.cfg
```

### Comparing `micropython-bmp581-0.1.1/.pre-commit-config.yaml` & `micropython-bmp581-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-bmp581-0.1.1/.pylintrc` & `micropython-bmp581-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.1/LICENSE` & `micropython-bmp581-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.1/PKG-INFO` & `micropython-bmp581-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-bmp581
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Bosch BMP581 pressure sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMP581
-Keywords: sensor,micropython,bmp581,pressure,altitude,bosch,bmp581,micropython,sensor,pressure,altitude
+Keywords: sensor,micropython,pressure,bosch,bmp581,altitude
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-bmp581-0.1.1/README.rst` & `micropython-bmp581-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.1/docs/_static/Logo.png` & `micropython-bmp581-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.1/docs/conf.py` & `micropython-bmp581-0.1.2/docs/conf.py`

 * *Files 22% similar despite different names*

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
+    import micropython_bmp581
+except ImportError:
+    raise SystemExit("micropython_bmp581 has to be importable")
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
-        "MicroPython_bmp581_Library.tex",
-        "MicroPython bmp581 Library Documentation",
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
-        "MicroPython_bmp581_Library",
-        "MicroPython bmp581 Library Documentation",
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
-        "MicroPython_bmp581_Library",
-        "MicroPython bmp581 Library Documentation",
-        author,
-        "MicroPython_bmp581_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-bmp581-0.1.1/docs/examples.rst` & `micropython-bmp581-0.1.2/docs/examples.rst`

 * *Files 4% similar despite different names*

```diff
@@ -47,7 +47,16 @@
 --------------------------
 
 Example showing the Output data rate setting
 
 .. literalinclude:: ../examples/bmp581_output_data_rate.py
     :caption: examples/bmp581_output_data_rate.py
     :linenos:
+
+Altitude example
+-----------------
+
+Example showing the Output data rate setting
+
+.. literalinclude:: ../examples/bmp581_altitude.py
+    :caption: examples/bmp581_altitude.py
+    :linenos:
```

### Comparing `micropython-bmp581-0.1.1/examples/bmp581_output_data_rate.py` & `micropython-bmp581-0.1.2/examples/bmp581_output_data_rate.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 import time
 from machine import Pin, I2C
 from micropython_bmp581 import bmp581
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 bmp = bmp581.BMP581(i2c)
 
-bmp.output_data_rate = bmp581.ODR240
-
 while True:
     for output_data_rate in range(0, 32, 1):
         print("Current Output data rate setting: ", bmp.output_data_rate)
         for _ in range(10):
-            press = bmp.pressure
-            print("pressure:{:.2f}kPa".format(press))
+            print(f"Pressure: {bmp.pressure:.2f}kPa")
             time.sleep(0.5)
         bmp.output_data_rate = output_data_rate
```

### Comparing `micropython-bmp581-0.1.1/examples/bmp581_power_mode.py` & `micropython-bmp581-0.1.2/examples/bmp581_power_mode.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,11 +11,10 @@
 
 bmp.power_mode = bmp581.NORMAL
 
 while True:
     for power_mode in bmp581.power_mode_values:
         print("Current Power mode setting: ", bmp.power_mode)
         for _ in range(10):
-            press = bmp.pressure
-            print("pressure:{:.2f}kPa".format(press))
+            print(f"Pressure: {bmp.pressure:.2f}kPa")
             time.sleep(0.5)
         bmp.power_mode = power_mode
```

### Comparing `micropython-bmp581-0.1.1/examples/bmp581_temperature_oversample_rate.py` & `micropython-bmp581-0.1.2/examples/bmp581_temperature_oversample_rate.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,10 +15,10 @@
     for temperature_oversample_rate in bmp581.temperature_oversample_rate_values:
         print(
             "Current Temperature oversample rate setting: ",
             bmp.temperature_oversample_rate,
         )
         for _ in range(10):
             temp = bmp.temperature
-            print("temperature:{:.2f}C".format(temp))
+            print(f"Temperature: {bmp.temperature:.2f}C")
             time.sleep(0.5)
         bmp.temperature_oversample_rate = temperature_oversample_rate
```

### Comparing `micropython-bmp581-0.1.1/micropython_bmp581/bmp581.py` & `micropython-bmp581-0.1.2/micropython_bmp581/bmp581.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 """
 
 from micropython import const
 from micropython_bmp581.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMP581.git"
 
 _REG_WHOAMI = const(0x01)
 _OSR_CONF = const(0x36)
 _ODR_CONFIG = const(0x37)
 
 
@@ -55,33 +55,33 @@
 )
 
 
 class BMP581:
     """Driver for the BMP581 Sensor connected over I2C.
 
     :param ~machine.I2C i2c: The I2C bus the BMP581 is connected to.
-    :param int address: The I2C device address. Defaults to :const:`0x69`
+    :param int address: The I2C device address. Defaults to :const:`0x47`
 
     :raises RuntimeError: if the sensor is not found
 
     **Quickstart: Importing and using the device**
 
     Here is an example of using the :class:`BMP581` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import bmp581
+        from micropython_bmp581 import bmp581
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         bmp581 = bmp581.BMP581(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
         press = bmp.pressure
@@ -243,49 +243,46 @@
         if value not in range(0, 32, 1):
             raise ValueError("Value must be a valid output_data_rate setting")
         self._output_data_rate = value
 
     @property
     def temperature(self) -> float:
         """
-        The temperature sensor in C
-        :return: Temperature
+        The temperature sensor in Celsius
+        :return: Temperature in Celsius
         """
         raw_temp = self._temperature
 
         return self._twos_comp(raw_temp, 24) / 2**16.0
 
     @property
     def pressure(self) -> float:
         """
         The sensor pressure in kPa
         :return: Pressure in kPa
         """
         raw_pressure = self._pressure
 
-        return self._twos_comp(raw_pressure, 24) / 2**6.0 / 1000
+        return self._twos_comp(raw_pressure, 24) / 2**6.0 / 1000.0
 
     @property
     def altitude(self):
         """
         With the measured pressure p and the pressure at sea level p0 e.g. 1013.25hPa,
         the altitude in meters can be calculated with the international barometric formula
 
-        With the measured pressure p and the absolute altitude the pressure at sea level
-        can be calculated too. See the altitude setter for this calculation
         """
 
         altitude = 44330.0 * (
             1.0 - ((self.pressure / self.sea_level_pressure) ** 0.190284)
         )
         return round(altitude, 1)
 
     @altitude.setter
     def altitude(self, value: float) -> None:
         self.sea_level_pressure = self.pressure / (1.0 - value / 44330.0) ** 5.255
 
     @staticmethod
     def _twos_comp(val: int, bits: int) -> int:
-
         if val & (1 << (bits - 1)) != 0:
             return val - (1 << bits)
         return val
```

### Comparing `micropython-bmp581-0.1.1/micropython_bmp581/i2c_helpers.py` & `micropython-bmp581-0.1.2/micropython_bmp581/i2c_helpers.py`

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

### Comparing `micropython-bmp581-0.1.1/micropython_bmp581.egg-info/PKG-INFO` & `micropython-bmp581-0.1.2/micropython_bmp581.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-bmp581
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Bosch BMP581 pressure sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMP581
-Keywords: sensor,micropython,bmp581,pressure,altitude,bosch,bmp581,micropython,sensor,pressure,altitude
+Keywords: sensor,micropython,pressure,bosch,bmp581,altitude
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-bmp581-0.1.1/micropython_bmp581.egg-info/SOURCES.txt` & `micropython-bmp581-0.1.2/micropython_bmp581.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 docs/requirements.txt
 docs/_static/Logo.png
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/bmp581_altitude.py
 examples/bmp581_output_data_rate.py
 examples/bmp581_power_mode.py
 examples/bmp581_pressure_oversample_rate.py
 examples/bmp581_simpletest.py
 examples/bmp581_temperature.py
 examples/bmp581_temperature_oversample_rate.py
 micropython_bmp581/__init__.py
 micropython_bmp581/bmp581.py
 micropython_bmp581/i2c_helpers.py
 micropython_bmp581.egg-info/PKG-INFO
 micropython_bmp581.egg-info/SOURCES.txt
 micropython_bmp581.egg-info/dependency_links.txt
-micropython_bmp581.egg-info/requires.txt
 micropython_bmp581.egg-info/top_level.txt
```

### Comparing `micropython-bmp581-0.1.1/pyproject.toml` & `micropython-bmp581-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -8,42 +8,37 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-bmp581"
 description = "MicroPython Driver for the Bosch BMP581 pressure sensor"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_BMP581"}
 keywords = [
     "sensor",
     "micropython",
-    "bmp581",
     "pressure",
-    "altitude",
     "bosch",
     "bmp581",
-    "micropython",
-    "sensor",
-    "pressure",
     "altitude",
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
-py-modules = ["bmp581"]
+packages = ["micropython_bmp581"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

