# Comparing `tmp/micropython-htu21df-0.1.1.tar.gz` & `tmp/micropython-htu21df-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-htu21df-0.1.1.tar", last modified: Sat Jun 17 15:20:16 2023, max compression
+gzip compressed data, was "micropython-htu21df-0.1.2.tar", last modified: Mon Aug  7 13:59:48 2023, max compression
```

## Comparing `micropython-htu21df-0.1.1.tar` & `micropython-htu21df-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:20:16.632566 micropython-htu21df-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:20:16.628566 micropython-htu21df-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:20:16.632566 micropython-htu21df-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-17 15:20:16.632566 micropython-htu21df-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:20:16.632566 micropython-htu21df-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:20:16.632566 micropython-htu21df-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:20:16.632566 micropython-htu21df-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-17 15:20:09.000000 micropython-htu21df-0.1.1/examples/htu21df_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-17 15:20:09.000000 micropython-htu21df-0.1.1/examples/htu21df_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:20:16.632566 micropython-htu21df-0.1.1/micropython_htu21df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:20:09.000000 micropython-htu21df-0.1.1/micropython_htu21df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-17 15:20:09.000000 micropython-htu21df-0.1.1/micropython_htu21df/htu21df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:20:16.632566 micropython-htu21df-0.1.1/micropython_htu21df.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-17 15:20:16.000000 micropython-htu21df-0.1.1/micropython_htu21df.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-17 15:20:16.000000 micropython-htu21df-0.1.1/micropython_htu21df.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:20:16.000000 micropython-htu21df-0.1.1/micropython_htu21df.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:20:16.000000 micropython-htu21df-0.1.1/micropython_htu21df.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 15:20:16.000000 micropython-htu21df-0.1.1/micropython_htu21df.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-17 15:20:09.000000 micropython-htu21df-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:20:01.000000 micropython-htu21df-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:20:16.632566 micropython-htu21df-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:59:48.257908 micropython-htu21df-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:59:48.253908 micropython-htu21df-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:59:48.257908 micropython-htu21df-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-07 13:59:48.257908 micropython-htu21df-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:59:48.257908 micropython-htu21df-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:59:48.257908 micropython-htu21df-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:59:48.257908 micropython-htu21df-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-07 13:59:40.000000 micropython-htu21df-0.1.2/examples/htu21df_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-07 13:59:40.000000 micropython-htu21df-0.1.2/examples/htu21df_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:59:48.257908 micropython-htu21df-0.1.2/micropython_htu21df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:59:40.000000 micropython-htu21df-0.1.2/micropython_htu21df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-07 13:59:40.000000 micropython-htu21df-0.1.2/micropython_htu21df/htu21df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:59:48.257908 micropython-htu21df-0.1.2/micropython_htu21df.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-07 13:59:48.000000 micropython-htu21df-0.1.2/micropython_htu21df.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-07 13:59:48.000000 micropython-htu21df-0.1.2/micropython_htu21df.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:59:48.000000 micropython-htu21df-0.1.2/micropython_htu21df.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 13:59:48.000000 micropython-htu21df-0.1.2/micropython_htu21df.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-07 13:59:40.000000 micropython-htu21df-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:59:33.000000 micropython-htu21df-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:59:48.257908 micropython-htu21df-0.1.2/setup.cfg
```

### Comparing `micropython-htu21df-0.1.1/.pre-commit-config.yaml` & `micropython-htu21df-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-htu21df-0.1.1/.pylintrc` & `micropython-htu21df-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-htu21df-0.1.1/LICENSE` & `micropython-htu21df-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-htu21df-0.1.1/PKG-INFO` & `micropython-htu21df-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-htu21df
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython HTU21D-F Temperature & Humidity
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_HTU21DF
-Keywords: sensor,micropython,htu21df,Sensortemperature,humidity,htu21df,sensor,micropython
+Keywords: sensor,htu21df,temperature,humidity,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-htu21df-0.1.1/README.rst` & `micropython-htu21df-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-htu21df-0.1.1/docs/_static/Logo.png` & `micropython-htu21df-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-htu21df-0.1.1/docs/conf.py` & `micropython-htu21df-0.1.2/docs/conf.py`

 * *Files 22% similar despite different names*

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
+    import micropython_htu21df
+except ImportError:
+    raise SystemExit("micropython_htu21df has to be importable")
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
-        "MicroPython_htu21df_Library.tex",
-        "MicroPython htu21df Library Documentation",
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
-        "MicroPython_htu21df_Library",
-        "MicroPython htu21df Library Documentation",
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
-        "MicroPython_htu21df_Library",
-        "MicroPython htu21df Library Documentation",
-        author,
-        "MicroPython_htu21df_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-htu21df-0.1.1/examples/htu21df_resolution.py` & `micropython-htu21df-0.1.2/examples/htu21df_resolution.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 print("Current Resolution")
 print(htu.temp_rh_resolution)
 htu.temp_rh_resolution = 0x81  # Take a look at the library for correct values
 print("Changed Resolution")
 print(htu.temp_rh_resolution)
 
 while True:
-    print("Temperature: {:.2f} C".format(htu.temperature))
-    print("Humidity: {:.2f} %%".format(htu.humidity))
+    print(f"Temperature: {htu.temperature:.2f}°C")
+    print(f"Humidity: {htu.humidity:.2%}%")
     print("")
     time.sleep(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-htu21df-0.1.1/micropython_htu21df/htu21df.py` & `micropython-htu21df-0.1.2/micropython_htu21df/htu21df.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """
 
 import time
 import struct
 from micropython import const
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_HTU21DF.git"
 
 _SOFTRESET = const(0xFE)
 _TEMPERATURE = const(0xF3)
 _HUMIDITY = const(0xF5)
 _READ_USER1 = const(0xE7)
 _WRITE_USER1 = const(0xE6)
@@ -47,15 +47,15 @@
         from machine import Pin, I2C
         from micropython_htu21df import htu21df
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         htu21df = htu21df.HTU21DF(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
         temp = htu.temperature
```

### Comparing `micropython-htu21df-0.1.1/micropython_htu21df.egg-info/PKG-INFO` & `micropython-htu21df-0.1.2/micropython_htu21df.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-htu21df
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython HTU21D-F Temperature & Humidity
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_HTU21DF
-Keywords: sensor,micropython,htu21df,Sensortemperature,humidity,htu21df,sensor,micropython
+Keywords: sensor,htu21df,temperature,humidity,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-htu21df-0.1.1/micropython_htu21df.egg-info/SOURCES.txt` & `micropython-htu21df-0.1.2/micropython_htu21df.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -23,9 +23,8 @@
 examples/htu21df_resolution.py
 examples/htu21df_simpletest.py
 micropython_htu21df/__init__.py
 micropython_htu21df/htu21df.py
 micropython_htu21df.egg-info/PKG-INFO
 micropython_htu21df.egg-info/SOURCES.txt
 micropython_htu21df.egg-info/dependency_links.txt
-micropython_htu21df.egg-info/requires.txt
 micropython_htu21df.egg-info/top_level.txt
```

### Comparing `micropython-htu21df-0.1.1/pyproject.toml` & `micropython-htu21df-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,39 +8,36 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-htu21df"
 description = "MicroPython HTU21D-F Temperature & Humidity"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_HTU21DF"}
 keywords = [
     "sensor",
-    "micropython",
     "htu21df",
-    "Sensortemperature",
+    "temperature",
     "humidity",
-    "htu21df",
-    "sensor",
     "micropython",
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
-py-modules = ["htu21df"]
+packages = ["micropython_htu21df"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

