# Comparing `tmp/micropython-ds3502-0.1.1.tar.gz` & `tmp/micropython-ds3502-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-ds3502-0.1.1.tar", last modified: Sat Jun 17 14:22:54 2023, max compression
+gzip compressed data, was "micropython-ds3502-0.1.2.tar", last modified: Mon Aug  7 14:00:24 2023, max compression
```

## Comparing `micropython-ds3502-0.1.1.tar` & `micropython-ds3502-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:54.617637 micropython-ds3502-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:54.613638 micropython-ds3502-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:54.613638 micropython-ds3502-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-17 14:22:54.617637 micropython-ds3502-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:54.617637 micropython-ds3502-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:54.617637 micropython-ds3502-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:54.617637 micropython-ds3502-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 14:22:47.000000 micropython-ds3502-0.1.1/examples/ds3502_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:54.617637 micropython-ds3502-0.1.1/micropython_ds3502/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:47.000000 micropython-ds3502-0.1.1/micropython_ds3502/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-17 14:22:47.000000 micropython-ds3502-0.1.1/micropython_ds3502/ds3502.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:22:47.000000 micropython-ds3502-0.1.1/micropython_ds3502/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:54.617637 micropython-ds3502-0.1.1/micropython_ds3502.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-17 14:22:54.000000 micropython-ds3502-0.1.1/micropython_ds3502.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-17 14:22:54.000000 micropython-ds3502-0.1.1/micropython_ds3502.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:22:54.000000 micropython-ds3502-0.1.1/micropython_ds3502.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:22:54.000000 micropython-ds3502-0.1.1/micropython_ds3502.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 14:22:54.000000 micropython-ds3502-0.1.1/micropython_ds3502.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-17 14:22:47.000000 micropython-ds3502-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:22:36.000000 micropython-ds3502-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:22:54.617637 micropython-ds3502-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:00:24.106246 micropython-ds3502-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:00:24.098246 micropython-ds3502-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:00:24.102246 micropython-ds3502-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-07 14:00:24.106246 micropython-ds3502-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:00:24.102246 micropython-ds3502-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:00:24.102246 micropython-ds3502-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:00:24.102246 micropython-ds3502-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-07 14:00:13.000000 micropython-ds3502-0.1.2/examples/ds3502_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:00:24.102246 micropython-ds3502-0.1.2/micropython_ds3502/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:00:13.000000 micropython-ds3502-0.1.2/micropython_ds3502/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-08-07 14:00:13.000000 micropython-ds3502-0.1.2/micropython_ds3502/ds3502.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-07 14:00:13.000000 micropython-ds3502-0.1.2/micropython_ds3502/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:00:24.106246 micropython-ds3502-0.1.2/micropython_ds3502.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-07 14:00:24.000000 micropython-ds3502-0.1.2/micropython_ds3502.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-07 14:00:24.000000 micropython-ds3502-0.1.2/micropython_ds3502.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:00:24.000000 micropython-ds3502-0.1.2/micropython_ds3502.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 14:00:24.000000 micropython-ds3502-0.1.2/micropython_ds3502.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-07 14:00:13.000000 micropython-ds3502-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:59:59.000000 micropython-ds3502-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:00:24.106246 micropython-ds3502-0.1.2/setup.cfg
```

### Comparing `micropython-ds3502-0.1.1/.pre-commit-config.yaml` & `micropython-ds3502-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-ds3502-0.1.1/.pylintrc` & `micropython-ds3502-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-ds3502-0.1.1/LICENSE` & `micropython-ds3502-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-ds3502-0.1.1/PKG-INFO` & `micropython-ds3502-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-ds3502
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the DS3502 Potentiometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_DS3502
-Keywords: sensor,micropython,ds3502,potentiometer,resistance,variable,driver,micropython,maxim,ds3502
+Keywords: sensor,ds3502,potentiometer,resistance,variable,driver,micropython,maxim
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-ds3502-0.1.1/README.rst` & `micropython-ds3502-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-ds3502-0.1.1/docs/_static/Logo.png` & `micropython-ds3502-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-ds3502-0.1.1/docs/conf.py` & `micropython-ds3502-0.1.2/docs/conf.py`

 * *Files 26% similar despite different names*

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
+    import micropython_ds3502
+except ImportError:
+    raise SystemExit("micropython_ds3502 has to be importable")
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
@@ -52,17 +66,14 @@
 # The short X.Y version.
 version = "1.0"
 # The full version, including alpha/beta/rc tags.
 release = "1.0"
 
 language = "en"
 autoclass_content = "both"
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = [
     "_build",
     "Thumbs.db",
     ".DS_Store",
     ".env",
     "requirements.txt",
 ]
@@ -182,65 +193,7 @@
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
-        "MicroPython_ds3502_Library.tex",
-        "MicroPython ds3502 Library Documentation",
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
-        "MicroPython_ds3502_Library",
-        "MicroPython ds3502 Library Documentation",
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
-        "MicroPython_ds3502_Library",
-        "MicroPython ds3502 Library Documentation",
-        author,
-        "MicroPython_ds3502_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-ds3502-0.1.1/examples/ds3502_simpletest.py` & `micropython-ds3502-0.1.2/examples/ds3502_simpletest.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 ds3502 = ds3502.DS3502(i2c)
 
 wiper_output = ADC(Pin(26, mode=Pin.IN))
 
 while True:
     # set th
     ds3502.wiper = 127
-    print("Wiper set to %d" % ds3502.wiper)
+    print(f"Wiper set to {ds3502.wiper}")
     voltage = wiper_output.read_u16()
     voltage *= 3.3
     voltage /= 65535
-    print("Wiper voltage: %.2f V" % voltage)
-    print("")
+    print(f"Wiper voltage {voltage:.2f}V")
+    print()
     sleep(1.0)
 
     ds3502.wiper = 0
-    print("Wiper set to %d" % ds3502.wiper)
+    print(f"Wiper set to {ds3502.wiper}")
     voltage = wiper_output.read_u16()
     voltage *= 3.3
     voltage /= 65535
-    print("Wiper voltage: %.2f V" % voltage)
-    print("")
+    print(f"Wiper voltage {voltage:.2f}V")
+    print()
     sleep(1.0)
 
     ds3502.wiper = 63
-    print("Wiper set to %d" % ds3502.wiper)
+    print(f"Wiper set to {ds3502.wiper}")
     voltage = wiper_output.read_u16()
     voltage *= 3.3
     voltage /= 65535
-    print("Wiper voltage: %.2f V" % voltage)
+    print(f"Wiper voltage {voltage:.2f}V")
     print("")
     sleep(1.0)
```

### Comparing `micropython-ds3502-0.1.1/micropython_ds3502/ds3502.py` & `micropython-ds3502-0.1.2/micropython_ds3502/ds3502.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 
 from time import sleep
 from micropython import const
 from micropython_ds3502.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_DS3502.git"
 
 _REG_WIPER = const(0x00)  # Wiper value register (R/W)
 _REG_CONTROL = const(0x02)  # Configuration Register (R/W)
 
 
 class DS3502:
@@ -41,21 +41,21 @@
 
     Here is an example of using the :class:`DS3502` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import ds3502
+        from micropython_ds3502 import ds3502
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         ds3502 = ds3502.DS3502(i2c)
 
 
     """
 
     _wiper = RegisterStruct(_REG_WIPER, ">B")
     _write_only_to_wiper = CBits(1, _REG_CONTROL, 7)
```

### Comparing `micropython-ds3502-0.1.1/micropython_ds3502/i2c_helpers.py` & `micropython-ds3502-0.1.2/micropython_ds3502/i2c_helpers.py`

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

### Comparing `micropython-ds3502-0.1.1/micropython_ds3502.egg-info/PKG-INFO` & `micropython-ds3502-0.1.2/micropython_ds3502.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-ds3502
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the DS3502 Potentiometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_DS3502
-Keywords: sensor,micropython,ds3502,potentiometer,resistance,variable,driver,micropython,maxim,ds3502
+Keywords: sensor,ds3502,potentiometer,resistance,variable,driver,micropython,maxim
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-ds3502-0.1.1/micropython_ds3502.egg-info/SOURCES.txt` & `micropython-ds3502-0.1.2/micropython_ds3502.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -23,9 +23,8 @@
 examples/ds3502_simpletest.py
 micropython_ds3502/__init__.py
 micropython_ds3502/ds3502.py
 micropython_ds3502/i2c_helpers.py
 micropython_ds3502.egg-info/PKG-INFO
 micropython_ds3502.egg-info/SOURCES.txt
 micropython_ds3502.egg-info/dependency_links.txt
-micropython_ds3502.egg-info/requires.txt
 micropython_ds3502.egg-info/top_level.txt
```

### Comparing `micropython-ds3502-0.1.1/pyproject.toml` & `micropython-ds3502-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,41 +8,39 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-ds3502"
 description = "MicroPython Driver for the DS3502 Potentiometer"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_DS3502"}
 keywords = [
     "sensor",
-    "micropython",
     "ds3502",
     "potentiometer",
     "resistance",
     "variable",
     "driver",
     "micropython",
     "maxim",
-    "ds3502",
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
-py-modules = ["ds3502"]
+packages = ["micropython_ds3502"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

