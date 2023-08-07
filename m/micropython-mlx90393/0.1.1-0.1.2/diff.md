# Comparing `tmp/micropython-mlx90393-0.1.1.tar.gz` & `tmp/micropython-mlx90393-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-mlx90393-0.1.1.tar", last modified: Sat Jun 17 14:55:34 2023, max compression
+gzip compressed data, was "micropython-mlx90393-0.1.2.tar", last modified: Mon Aug  7 13:50:37 2023, max compression
```

## Comparing `micropython-mlx90393-0.1.1.tar` & `micropython-mlx90393-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.200568 micropython-mlx90393-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.200568 micropython-mlx90393-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 14:55:25.000000 micropython-mlx90393-0.1.1/examples/micropython_mlx90393_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/micropython_mlx90393/
--rw-r--r--   0 runner    (1001) docker     (123)    18031 2023-06-17 14:55:25.000000 micropython-mlx90393-0.1.1/micropython_mlx90393/mlx90393.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-17 14:55:34.000000 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-17 14:55:34.000000 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:55:34.000000 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 14:55:34.000000 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-17 14:55:34.000000 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-17 14:55:25.000000 micropython-mlx90393-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:37.167945 micropython-mlx90393-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:37.163945 micropython-mlx90393-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:37.163945 micropython-mlx90393-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-08-07 13:50:37.167945 micropython-mlx90393-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:37.163945 micropython-mlx90393-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:37.163945 micropython-mlx90393-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:37.163945 micropython-mlx90393-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-07 13:50:29.000000 micropython-mlx90393-0.1.2/examples/micropython_mlx90393_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:37.167945 micropython-mlx90393-0.1.2/micropython_mlx90393/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:29.000000 micropython-mlx90393-0.1.2/micropython_mlx90393/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-08-07 13:50:29.000000 micropython-mlx90393-0.1.2/micropython_mlx90393/mlx90393.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:50:37.167945 micropython-mlx90393-0.1.2/micropython_mlx90393.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-08-07 13:50:37.000000 micropython-mlx90393-0.1.2/micropython_mlx90393.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-07 13:50:37.000000 micropython-mlx90393-0.1.2/micropython_mlx90393.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:50:37.000000 micropython-mlx90393-0.1.2/micropython_mlx90393.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 13:50:37.000000 micropython-mlx90393-0.1.2/micropython_mlx90393.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 13:50:37.000000 micropython-mlx90393-0.1.2/micropython_mlx90393.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-07 13:50:29.000000 micropython-mlx90393-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:50:22.000000 micropython-mlx90393-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:50:37.167945 micropython-mlx90393-0.1.2/setup.cfg
```

### Comparing `micropython-mlx90393-0.1.1/.pre-commit-config.yaml` & `micropython-mlx90393-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-mlx90393-0.1.1/.pylintrc` & `micropython-mlx90393-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-mlx90393-0.1.1/LICENSE` & `micropython-mlx90393-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-mlx90393-0.1.1/PKG-INFO` & `micropython-mlx90393-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-mlx90393
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the MLX90393 Sensor
 Author-email: "Jose D. Montoya" <mlx90393@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MLX90393
 Keywords: micropython,micropython_mlx90393,MicroPython,Sensor,Magnetic,magnetometer
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-mlx90393-0.1.1/README.rst` & `micropython-mlx90393-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-mlx90393-0.1.1/docs/_static/Logo.png` & `micropython-mlx90393-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-mlx90393-0.1.1/docs/_static/favicon.ico` & `micropython-mlx90393-0.1.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-mlx90393-0.1.1/docs/conf.py` & `micropython-mlx90393-0.1.2/docs/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,42 @@
-# -*- coding: utf-8 -*-
-
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
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
+    import micropython_mlx90393
+except ImportError:
+    raise SystemExit("micropython_mlx90393 has to be importable")
+
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
-    "sphinx.ext.napoleon",
-    "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "sphinx_immaterial",
 ]
 
 autodoc_preserve_defaults = True
 
 
@@ -201,64 +214,7 @@
 # pixels large.
 #
 html_favicon = "_static/favicon.ico"
 
 html_logo = "_static/Logo.png"
 # Output file base name for HTML help builder.
 htmlhelp_basename = "MicropythonMLX90393Librarydoc"
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
-        "MicroPython_MLX90393_Library.tex",
-        "MicroPython_MLX90393 Library Documentation",
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
-        "MicroPython_MLX90393_Library",
-        "MicroPython_MLX90393 Library Documentation",
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
-        "MicroPython_MLX90393_Library",
-        "MicroPython_MLX90393 Library Documentation",
-        author,
-        "MicroPython_MLX90393_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-mlx90393-0.1.1/micropython_mlx90393/mlx90393.py` & `micropython-mlx90393-0.1.2/micropython_mlx90393/mlx90393.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,19 @@
 This library depends on Micropython
 
 """
 
 # pylint: disable=too-many-arguments, line-too-long
 
 import time
+import struct
 from micropython import const
 
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_MLX90393.git"
 
 
 class CBits:
     """
     Changes bits from a byte register
     """
```

### Comparing `micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/PKG-INFO` & `micropython-mlx90393-0.1.2/micropython_mlx90393.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-mlx90393
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the MLX90393 Sensor
 Author-email: "Jose D. Montoya" <mlx90393@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MLX90393
 Keywords: micropython,micropython_mlx90393,MicroPython,Sensor,Magnetic,magnetometer
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/SOURCES.txt` & `micropython-mlx90393-0.1.2/micropython_mlx90393.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 LICENSE
 README.rst
 examples.json
 optional_requirements.txt
-packages.json
+package.json
 pyproject.toml
 requirements.txt
 .github/workflows/release_pypi.yml
 docs/api.rst
 docs/conf.py
 docs/examples.rst
 docs/index.rst
 docs/requirements.txt
 docs/_static/Logo.png
 docs/_static/extra_css.css
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/micropython_mlx90393_simpletest.py
+micropython_mlx90393/__init__.py
 micropython_mlx90393/mlx90393.py
 micropython_mlx90393.egg-info/PKG-INFO
 micropython_mlx90393.egg-info/SOURCES.txt
 micropython_mlx90393.egg-info/dependency_links.txt
 micropython_mlx90393.egg-info/requires.txt
 micropython_mlx90393.egg-info/top_level.txt
```

### Comparing `micropython-mlx90393-0.1.1/pyproject.toml` & `micropython-mlx90393-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# SPDX-FileCopyrightText: 2022 Alec Delaney, written for Adafruit Industries
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 [build-system]
 requires = [
     "setuptools",
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-mlx90393"
 description = "MicroPython Driver for the MLX90393 Sensor"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "mlx90393@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_MLX90393"}
 keywords = [
     "micropython",
```

