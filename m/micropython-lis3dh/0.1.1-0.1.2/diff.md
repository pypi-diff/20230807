# Comparing `tmp/micropython-lis3dh-0.1.1.tar.gz` & `tmp/micropython-lis3dh-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-lis3dh-0.1.1.tar", last modified: Sat Jun 17 15:03:06 2023, max compression
+gzip compressed data, was "micropython-lis3dh-0.1.2.tar", last modified: Mon Aug  7 13:42:10 2023, max compression
```

## Comparing `micropython-lis3dh-0.1.1.tar` & `micropython-lis3dh-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.389334 micropython-lis3dh-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.381333 micropython-lis3dh-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.385334 micropython-lis3dh-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-17 15:03:06.389334 micropython-lis3dh-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.385334 micropython-lis3dh-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.385334 micropython-lis3dh-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.385334 micropython-lis3dh-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/examples/lis3dg_data_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/examples/lis3dh_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/examples/lis3dh_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.385334 micropython-lis3dh-0.1.1/micropython_lis3dh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/micropython_lis3dh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/micropython_lis3dh/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/micropython_lis3dh/lis3dh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.389334 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-17 15:03:06.000000 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 15:03:06.000000 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:03:06.000000 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:03:06.000000 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 15:03:06.000000 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:03:06.389334 micropython-lis3dh-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:42:10.771617 micropython-lis3dh-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:42:10.763616 micropython-lis3dh-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:42:10.767616 micropython-lis3dh-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-08-07 13:42:10.771617 micropython-lis3dh-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:42:10.767616 micropython-lis3dh-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:42:10.767616 micropython-lis3dh-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:42:10.767616 micropython-lis3dh-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-07 13:42:01.000000 micropython-lis3dh-0.1.2/examples/lis3dg_data_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-07 13:42:01.000000 micropython-lis3dh-0.1.2/examples/lis3dh_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-07 13:42:01.000000 micropython-lis3dh-0.1.2/examples/lis3dh_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:42:10.771617 micropython-lis3dh-0.1.2/micropython_lis3dh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:42:01.000000 micropython-lis3dh-0.1.2/micropython_lis3dh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-07 13:42:01.000000 micropython-lis3dh-0.1.2/micropython_lis3dh/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-08-07 13:42:01.000000 micropython-lis3dh-0.1.2/micropython_lis3dh/lis3dh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:42:10.771617 micropython-lis3dh-0.1.2/micropython_lis3dh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-08-07 13:42:10.000000 micropython-lis3dh-0.1.2/micropython_lis3dh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-07 13:42:10.000000 micropython-lis3dh-0.1.2/micropython_lis3dh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:42:10.000000 micropython-lis3dh-0.1.2/micropython_lis3dh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 13:42:10.000000 micropython-lis3dh-0.1.2/micropython_lis3dh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-07 13:42:01.000000 micropython-lis3dh-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:41:48.000000 micropython-lis3dh-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:42:10.771617 micropython-lis3dh-0.1.2/setup.cfg
```

### Comparing `micropython-lis3dh-0.1.1/.pre-commit-config.yaml` & `micropython-lis3dh-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-lis3dh-0.1.1/.pylintrc` & `micropython-lis3dh-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-lis3dh-0.1.1/LICENSE` & `micropython-lis3dh-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-lis3dh-0.1.1/PKG-INFO` & `micropython-lis3dh-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-lis3dh
-Version: 0.1.1
+Version: 0.1.2
 Summary: LIS3DH MicroPython Driver
 Author-email: "Jose D. Montoya" <lis3dh@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_LIS3DH
 Keywords: micropython,lis3dh,sernsor,acceleration,tap,movement,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-lis3dh-0.1.1/README.rst` & `micropython-lis3dh-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-lis3dh-0.1.1/docs/_static/Logo.png` & `micropython-lis3dh-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-lis3dh-0.1.1/docs/_static/favicon.ico` & `micropython-lis3dh-0.1.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-lis3dh-0.1.1/docs/conf.py` & `micropython-lis3dh-0.1.2/docs/conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,39 @@
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
+    import micropython_lis3dh
+except ImportError:
+    raise SystemExit("micropython_lis3dh has to be importable")
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
 
 # autodoc_mock_imports = [""]
 
 autodoc_preserve_defaults = True
@@ -199,64 +212,7 @@
 # pixels large.
 #
 html_favicon = "_static/favicon.ico"
 
 html_logo = "_static/Logo.png"
 # Output file base name for HTML help builder.
 htmlhelp_basename = "MicroPython_Lis3dh_Librarydoc"
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
-        "MicroPython_LIS3DH_Library.tex",
-        "MicroPython LIS3DH Library Documentation",
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
-        "MicroPython_LIS3DH_Library",
-        "MicroPython LIS3DH Library Documentation",
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
-        "MicroPython_LIS3DH_Library",
-        "MicroPython LIS3DH Library Documentation",
-        author,
-        "MicroPython_LIS3DH_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-lis3dh-0.1.1/docs/examples.rst` & `micropython-lis3dh-0.1.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-lis3dh-0.1.1/examples/lis3dh_data_rate.py` & `micropython-lis3dh-0.1.2/examples/lis3dh_data_rate.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,23 +7,19 @@
 i2c = I2C(sda=Pin(8), scl=Pin(9))
 lis = lis3dh.LIS3DH(i2c)
 
 # Getting information about the current Accelerometers Data Rate
 print("Accelerometer Data Rate: ", lis.data_rate)
 for _ in range(3):
     accx, accy, accz = lis.acceleration
-    print("X: ", accx)
-    print("Y: ", accy)
-    print("Z: ", accz)
-    print("----------")
+    print(f"x: {accx}m/s^2, y: {accy}m/s^2, z: {accz}m/s^2")
+    print()
     time.sleep(1)
 
 # Changing Data Rate of the accelerometer
 lis.data_rate = lis3dh.DATARATE_200
 print("Accelerometer Changed Data Rate: ", lis.data_rate)
 for _ in range(3):
     accx, accy, accz = lis.acceleration
-    print("X: ", accx)
-    print("Y: ", accy)
-    print("Z: ", accz)
-    print("----------")
+    print(f"x: {accx}m/s^2, y: {accy}m/s^2, z: {accz}m/s^2")
+    print()
     time.sleep(1)
```

### Comparing `micropython-lis3dh-0.1.1/micropython_lis3dh/i2c_helpers.py` & `micropython-lis3dh-0.1.2/micropython_lis3dh/i2c_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,17 @@
 
 
 * Author(s): Jose D. Montoya
 
 
 """
 # pylint: disable=unused-argument, no-name-in-module
+import struct
 
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
-
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/LIS3DH.git"
 
 
 class CBits:
     """
     Changes bits from a byte register
     """
@@ -34,22 +30,20 @@
         self.star_bit = start_bit
 
     def __get__(
         self,
         obj,
         objtype=None,
     ) -> int:
-
         reg = obj._i2c.readfrom_mem(obj._address, self.register, True)[0]
         reg = (reg & self.bit_mask) >> self.star_bit
 
         return reg
 
     def __set__(self, obj, value: int) -> None:
-
         memory_value = obj._i2c.readfrom_mem(obj._address, self.register, True)[0]
         memory_value &= ~self.bit_mask
 
         value <<= self.star_bit
         memory_value |= value
 
         obj._i2c.writeto_mem(obj._address, self.register, bytes([memory_value]))
@@ -79,9 +73,9 @@
                     obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
                 ),
             )
 
         return value
 
     def __set__(self, obj, value):
-
-        obj._i2c.writeto_mem(obj._address, self.register, bytes([value]))
+        mem_value = struct.pack(self.format, value)
+        obj._i2c.writeto_mem(obj._address, self.register, mem_value)
```

### Comparing `micropython-lis3dh-0.1.1/micropython_lis3dh/lis3dh.py` & `micropython-lis3dh-0.1.2/micropython_lis3dh/lis3dh.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 """
 # pylint: disable=unused-argument, no-name-in-module
 
 import time
 from micropython import const
 from micropython_lis3dh.i2c_helpers import RegisterStruct, CBits
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_LIS3DH.git"
 
 
 _REG_WHOAMI = const(0x0F)
 _REG_TEMPCFG = const(0x1F)
 _REG_CTRL1 = const(0x20)  # Defaults to 0b00000000
 _REG_CTRL3 = const(0x22)
 _REG_CTRL4 = const(0x23)
 _REG_CTRL5 = const(0x24)
 _REG_OUT_X_L = const(0x28)
+_REG_OUT_X_LM = const(0xA8)
 
 # Data rate
 DATARATE_1344 = const(0b1001)  # 1344 Hz
 DATARATE_400 = const(0b0111)  # 400Hz
 DATARATE_200 = const(0b0110)  # 200Hz
 DATARATE_100 = const(0b0101)  # 100Hz
 DATARATE_50 = const(0b0100)  # 50Hz
@@ -93,15 +94,15 @@
 
     """
 
     _device_id = RegisterStruct(_REG_WHOAMI, "B")
     _device_control = RegisterStruct(_REG_CTRL1, "B")
     _reboot_register = RegisterStruct(_REG_CTRL5, "B")
     _ctrl4_register = RegisterStruct(_REG_CTRL4, "B")
-    _reg_xl = RegisterStruct(_REG_OUT_X_L | 0x80, "<hhh")
+    _reg_xl = RegisterStruct(_REG_OUT_X_LM, "<hhh")
     _temp_comp = RegisterStruct(_REG_TEMPCFG, "B")
 
     # CTRL_REG1 (20h) ODR3|ODR2|ODR1|ODR0|LPen|Zen|Yen|Xen
     _axes_enabled = CBits(3, _REG_CTRL1, 3)  # Zen|Yen|Xen
     _data_rate = CBits(4, _REG_CTRL1, 4)  # ODR3|ODR2|ODR1|ODR0
 
     # TEMP_CFG_REG (1Fh) ADC_PD|TEMP_EN
@@ -161,15 +162,14 @@
 
         """
 
         return self._axes_enabled
 
     @axes_enabled.setter
     def axes_enabled(self, value):
-
         self._axes_enabled = value
 
     @property
     def data_rate(self):
         """The data rate of the accelerometer
         ODR <3:0> is used to set power mode and ODR selection. In the following
         table are reported all frequency resulting in combination of ODR<3:0>
@@ -202,15 +202,14 @@
 
         """
 
         return self._data_rate
 
     @data_rate.setter
     def data_rate(self, value):
-
         self._data_rate = value
 
     @property
     def data_range(self):
         """The range of the accelerometer. The LIS3DH has dynamically user
         selectable full scales of ±2g/±4g/±8g/±16g and it is capable of
         measuring accelerations with output data rates from 1 Hz to 5 kHz.
```

### Comparing `micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/PKG-INFO` & `micropython-lis3dh-0.1.2/micropython_lis3dh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-lis3dh
-Version: 0.1.1
+Version: 0.1.2
 Summary: LIS3DH MicroPython Driver
 Author-email: "Jose D. Montoya" <lis3dh@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_LIS3DH
 Keywords: micropython,lis3dh,sernsor,acceleration,tap,movement,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/SOURCES.txt` & `micropython-lis3dh-0.1.2/micropython_lis3dh.egg-info/SOURCES.txt`

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
@@ -23,9 +23,8 @@
 examples/lis3dh_simpletest.py
 micropython_lis3dh/__init__.py
 micropython_lis3dh/i2c_helpers.py
 micropython_lis3dh/lis3dh.py
 micropython_lis3dh.egg-info/PKG-INFO
 micropython_lis3dh.egg-info/SOURCES.txt
 micropython_lis3dh.egg-info/dependency_links.txt
-micropython_lis3dh.egg-info/requires.txt
 micropython_lis3dh.egg-info/top_level.txt
```

### Comparing `micropython-lis3dh-0.1.1/pyproject.toml` & `micropython-lis3dh-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-lis3dh"
 description = "LIS3DH MicroPython Driver"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "lis3dh@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_LIS3DH"}
 keywords = [
     "micropython",
```

