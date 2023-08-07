# Comparing `tmp/micropython-stts22h-0.1.1.tar.gz` & `tmp/micropython-stts22h-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-stts22h-0.1.1.tar", last modified: Sat Jun 17 14:44:39 2023, max compression
+gzip compressed data, was "micropython-stts22h-0.1.2.tar", last modified: Mon Aug  7 13:45:22 2023, max compression
```

## Comparing `micropython-stts22h-0.1.1.tar` & `micropython-stts22h-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.682183 micropython-stts22h-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.674183 micropython-stts22h-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/examples/stts22h_output_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/examples/stts22h_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/micropython_stts22h/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/micropython_stts22h/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/micropython_stts22h/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/micropython_stts22h/stts22h.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-17 14:44:39.000000 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-17 14:44:39.000000 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:44:39.000000 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:44:39.000000 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 14:44:39.000000 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:44:39.682183 micropython-stts22h-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:45:22.419452 micropython-stts22h-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:45:22.415452 micropython-stts22h-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:45:22.415452 micropython-stts22h-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-08-07 13:45:22.419452 micropython-stts22h-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:45:22.415452 micropython-stts22h-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:45:22.419452 micropython-stts22h-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:45:22.419452 micropython-stts22h-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-07 13:45:14.000000 micropython-stts22h-0.1.2/examples/stts22h_output_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-07 13:45:14.000000 micropython-stts22h-0.1.2/examples/stts22h_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:45:22.419452 micropython-stts22h-0.1.2/micropython_stts22h/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:45:14.000000 micropython-stts22h-0.1.2/micropython_stts22h/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 13:45:14.000000 micropython-stts22h-0.1.2/micropython_stts22h/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-08-07 13:45:14.000000 micropython-stts22h-0.1.2/micropython_stts22h/stts22h.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:45:22.419452 micropython-stts22h-0.1.2/micropython_stts22h.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-08-07 13:45:22.000000 micropython-stts22h-0.1.2/micropython_stts22h.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-08-07 13:45:22.000000 micropython-stts22h-0.1.2/micropython_stts22h.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:45:22.000000 micropython-stts22h-0.1.2/micropython_stts22h.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 13:45:22.000000 micropython-stts22h-0.1.2/micropython_stts22h.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-07 13:45:14.000000 micropython-stts22h-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:45:07.000000 micropython-stts22h-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:45:22.419452 micropython-stts22h-0.1.2/setup.cfg
```

### Comparing `micropython-stts22h-0.1.1/.pre-commit-config.yaml` & `micropython-stts22h-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-stts22h-0.1.1/.pylintrc` & `micropython-stts22h-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.1/LICENSE` & `micropython-stts22h-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.1/PKG-INFO` & `micropython-stts22h-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-stts22h
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the STTS22H Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_STTS22H
-Keywords: sensor,micropython,stts22h,temperature,sensor,stts22h,st,micropython,celsius
+Keywords: sensor,stts22h,temperature,sensor,st,micropython,celsius
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-stts22h-0.1.1/README.rst` & `micropython-stts22h-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.1/docs/_static/Logo.png` & `micropython-stts22h-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.1/docs/conf.py` & `micropython-stts22h-0.1.2/docs/conf.py`

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
+    import micropython_stts22h
+except ImportError:
+    raise SystemExit("micropython_stts22h has to be importable")
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
-        "MicroPython_stts22h_Library.tex",
-        "MicroPython stts22h Library Documentation",
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
-        "MicroPython_stts22h_Library",
-        "MicroPython stts22h Library Documentation",
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
-        "MicroPython_stts22h_Library",
-        "MicroPython stts22h Library Documentation",
-        author,
-        "MicroPython_stts22h_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-stts22h-0.1.1/micropython_stts22h/i2c_helpers.py` & `micropython-stts22h-0.1.2/micropython_stts22h/i2c_helpers.py`

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

### Comparing `micropython-stts22h-0.1.1/micropython_stts22h/stts22h.py` & `micropython-stts22h-0.1.2/micropython_stts22h/stts22h.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 """
 
 from micropython import const
 from micropython_stts22h.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_STTS22H.git"
 
 _REG_WHOAMI = const(0x01)
 _CTRL = const(0x04)
 
 
 ODR_25_HZ = const(0b00)
@@ -31,39 +31,41 @@
 output_data_rate_values = (ODR_25_HZ, ODR_50_HZ, ODR_100_HZ, ODR_200_HZ)
 
 
 class STTS22H:
     """Driver for the STTS22H Sensor connected over I2C.
 
     :param ~machine.I2C i2c: The I2C bus the STTS22H is connected to.
-    :param int address: The I2C device address. Defaults to :const:`0x69`
+    :param int address: The I2C device address. Defaults to :const:`0x3C`
 
     :raises RuntimeError: if the sensor is not found
 
     **Quickstart: Importing and using the device**
 
     Here is an example of using the :class:`STTS22H` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import stts22h
+        from micropython_stts22h import stts22h
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
-        stts22h = stts22h.STTS22H(i2c)
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
+        stts = stts22h.STTS22H(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
+        temp = stts.temperature
+
     """
 
     _device_id = RegisterStruct(_REG_WHOAMI, "B")
 
     _temperature_high_limit = RegisterStruct(0x02, "B")
     _temperature_low_limit = RegisterStruct(0x03, "B")
 
@@ -84,15 +86,15 @@
             raise RuntimeError("Failed to find STTS22H")
 
         self._freerun = True
 
     @property
     def temperature(self) -> float:
         """
-        The temperature sensor in C
+        The temperature sensor in Celsius
         :return: Temperature
         """
 
         return (self._temperature_MSB * 256 + self._temperature_LSB) / 100
 
     @property
     def temperature_high_limit(self) -> float:
@@ -115,24 +117,24 @@
     @temperature_low_limit.setter
     def temperature_low_limit(self, value: float):
         self._temperature_low_limit = value
 
     @property
     def high_limit(self) -> bool:
         """
-        The bit is automatically reset to ‘0’ upon reading the STATUS register.
+        The bit is automatically reset to '0' upon reading the STATUS register.
         :return: value if the temperature exceeds the high limit
         """
         value = (False, True)
         return value[self._high_limit]
 
     @property
     def low_limit(self) -> bool:
         """
-        The bit is automatically reset to ‘0’ upon reading the STATUS register.
+        The bit is automatically reset to '0' upon reading the STATUS register.
         :return: value if the temperature went under the low limit
         """
         value = (False, True)
         return value[self._low_limit]
 
     @property
     def output_data_rate(self) -> str:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `micropython-stts22h-0.1.1/micropython_stts22h.egg-info/PKG-INFO` & `micropython-stts22h-0.1.2/micropython_stts22h.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-stts22h
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the STTS22H Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_STTS22H
-Keywords: sensor,micropython,stts22h,temperature,sensor,stts22h,st,micropython,celsius
+Keywords: sensor,stts22h,temperature,sensor,st,micropython,celsius
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-stts22h-0.1.1/micropython_stts22h.egg-info/SOURCES.txt` & `micropython-stts22h-0.1.2/micropython_stts22h.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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
@@ -24,9 +24,8 @@
 examples/stts22h_simpletest.py
 micropython_stts22h/__init__.py
 micropython_stts22h/i2c_helpers.py
 micropython_stts22h/stts22h.py
 micropython_stts22h.egg-info/PKG-INFO
 micropython_stts22h.egg-info/SOURCES.txt
 micropython_stts22h.egg-info/dependency_links.txt
-micropython_stts22h.egg-info/requires.txt
 micropython_stts22h.egg-info/top_level.txt
```

### Comparing `micropython-stts22h-0.1.1/pyproject.toml` & `micropython-stts22h-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -8,27 +8,25 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-stts22h"
 description = "MicroPython Driver for the STTS22H Temperature Sensor"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_STTS22H"}
 keywords = [
     "sensor",
-    "micropython",
     "stts22h",
     "temperature",
     "sensor",
-    "stts22h",
     "st",
     "micropython",
     "celsius",
 ]
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
@@ -37,11 +35,11 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["stts22h"]
+packages = ["micropython_stts22h"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

