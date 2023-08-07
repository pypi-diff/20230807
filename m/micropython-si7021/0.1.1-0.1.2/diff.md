# Comparing `tmp/micropython-si7021-0.1.1.tar.gz` & `tmp/micropython-si7021-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-si7021-0.1.1.tar", last modified: Sat Jun 17 14:47:58 2023, max compression
+gzip compressed data, was "micropython-si7021-0.1.2.tar", last modified: Mon Aug  7 13:38:22 2023, max compression
```

## Comparing `micropython-si7021-0.1.1.tar` & `micropython-si7021-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.747110 micropython-si7021-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-17 14:47:51.000000 micropython-si7021-0.1.1/examples/si7021_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/micropython_si7021/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:51.000000 micropython-si7021-0.1.1/micropython_si7021/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-06-17 14:47:51.000000 micropython-si7021-0.1.1/micropython_si7021/si7021.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/micropython_si7021.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-17 14:47:58.000000 micropython-si7021-0.1.1/micropython_si7021.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-17 14:47:58.000000 micropython-si7021-0.1.1/micropython_si7021.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:47:58.000000 micropython-si7021-0.1.1/micropython_si7021.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 14:47:58.000000 micropython-si7021-0.1.1/micropython_si7021.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 14:47:58.000000 micropython-si7021-0.1.1/micropython_si7021.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-17 14:47:51.000000 micropython-si7021-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:47:58.747110 micropython-si7021-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:38:22.795201 micropython-si7021-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:38:22.791201 micropython-si7021-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:38:22.795201 micropython-si7021-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-07 13:38:22.795201 micropython-si7021-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:38:22.795201 micropython-si7021-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:38:22.795201 micropython-si7021-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:38:22.795201 micropython-si7021-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-07 13:38:14.000000 micropython-si7021-0.1.2/examples/si7021_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:38:22.795201 micropython-si7021-0.1.2/micropython_si7021/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:38:14.000000 micropython-si7021-0.1.2/micropython_si7021/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-08-07 13:38:14.000000 micropython-si7021-0.1.2/micropython_si7021/si7021.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:38:22.795201 micropython-si7021-0.1.2/micropython_si7021.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-07 13:38:22.000000 micropython-si7021-0.1.2/micropython_si7021.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-07 13:38:22.000000 micropython-si7021-0.1.2/micropython_si7021.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:38:22.000000 micropython-si7021-0.1.2/micropython_si7021.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 13:38:22.000000 micropython-si7021-0.1.2/micropython_si7021.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-07 13:38:14.000000 micropython-si7021-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:38:04.000000 micropython-si7021-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:38:22.795201 micropython-si7021-0.1.2/setup.cfg
```

### Comparing `micropython-si7021-0.1.1/.pre-commit-config.yaml` & `micropython-si7021-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-si7021-0.1.1/.pylintrc` & `micropython-si7021-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-si7021-0.1.1/LICENSE` & `micropython-si7021-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-si7021-0.1.1/PKG-INFO` & `micropython-si7021-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: micropython-si7021
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Library for the the Temperature and Humidity SI7021 Sensor
 Author-email: "Jose D. Montoya" <si7021@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_SI7021
-Keywords: micropython,micropython_si7021,sensor,temperature,humidity
+Keywords: micropython,micropython_si7021,si7021,sensor,temperature,humidity
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

### Comparing `micropython-si7021-0.1.1/README.rst` & `micropython-si7021-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-si7021-0.1.1/docs/_static/Logo.png` & `micropython-si7021-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-si7021-0.1.1/docs/_static/favicon.ico` & `micropython-si7021-0.1.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-si7021-0.1.1/docs/conf.py` & `micropython-si7021-0.1.2/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,21 +4,36 @@
 
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
+    import micropython_si7021
+except ImportError:
+    raise SystemExit("micropython_si7021 has to be importable")
+
 # -- General configuration ------------------------------------------------
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
-    "sphinx.ext.napoleon",
-    "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "sphinx_immaterial",
 ]
 
 # autodoc_mock_imports = ["digitalio", "busio"]
 
 autodoc_preserve_defaults = True
@@ -198,64 +213,7 @@
 # pixels large.
 #
 html_favicon = "_static/favicon.ico"
 
 html_logo = "_static/Logo.png"
 # Output file base name for HTML help builder.
 htmlhelp_basename = "MicropythonSI7021Librarydoc"
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
-        "MicroPython_SI7021_Library.tex",
-        "MicroPython_SI7021 Library Documentation",
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
-        "MicroPython_SI7021_Library",
-        "MicroPython_SI7021 Library Documentation",
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
-        "MicroPython_SI7021_Library",
-        "MicroPython_SI7021 Library Documentation",
-        author,
-        "MicroPython_SI7021_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-si7021-0.1.1/micropython_si7021/si7021.py` & `micropython-si7021-0.1.2/micropython_si7021/si7021.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,19 @@
 This library depends on Micropython
 
 """
 
 # pylint: disable=too-many-arguments, missing-function-docstring, unused-variable
 
 import time
+import struct
 from micropython import const
 
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_SI7021.git"
 
 
 class RegisterStructRW:
     """
     Register Struct
     """
```

### Comparing `micropython-si7021-0.1.1/micropython_si7021.egg-info/PKG-INFO` & `micropython-si7021-0.1.2/micropython_si7021.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: micropython-si7021
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Library for the the Temperature and Humidity SI7021 Sensor
 Author-email: "Jose D. Montoya" <si7021@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_SI7021
-Keywords: micropython,micropython_si7021,sensor,temperature,humidity
+Keywords: micropython,micropython_si7021,si7021,sensor,temperature,humidity
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

### Comparing `micropython-si7021-0.1.1/micropython_si7021.egg-info/SOURCES.txt` & `micropython-si7021-0.1.2/micropython_si7021.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

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
@@ -21,9 +20,8 @@
 docs/_static/favicon.ico.license
 examples/si7021_simpletest.py
 micropython_si7021/__init__.py
 micropython_si7021/si7021.py
 micropython_si7021.egg-info/PKG-INFO
 micropython_si7021.egg-info/SOURCES.txt
 micropython_si7021.egg-info/dependency_links.txt
-micropython_si7021.egg-info/requires.txt
 micropython_si7021.egg-info/top_level.txt
```

### Comparing `micropython-si7021-0.1.1/pyproject.toml` & `micropython-si7021-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,24 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-si7021"
 description = "MicroPython Library for the the Temperature and Humidity SI7021 Sensor"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "si7021@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_SI7021"}
 keywords = [
     "micropython",
     "micropython_si7021",
+    "si7021",
     "sensor",
     "temperature",
     "humidity",
 ]
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
@@ -33,12 +34,11 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["micropython_si7021"]
+packages = ["micropython_si7021"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
-optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```

