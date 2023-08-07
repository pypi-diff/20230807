# Comparing `tmp/micropython-h3lis200dl-0.1.1.tar.gz` & `tmp/micropython-h3lis200dl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-h3lis200dl-0.1.1.tar", last modified: Sat Jun 17 15:17:13 2023, max compression
+gzip compressed data, was "micropython-h3lis200dl-0.1.2.tar", last modified: Mon Aug  7 13:40:00 2023, max compression
```

## Comparing `micropython-h3lis200dl-0.1.1.tar` & `micropython-h3lis200dl-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.286739 micropython-h3lis200dl-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.278739 micropython-h3lis200dl-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.282739 micropython-h3lis200dl-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-17 15:17:13.286739 micropython-h3lis200dl-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.282739 micropython-h3lis200dl-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.282739 micropython-h3lis200dl-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.282739 micropython-h3lis200dl-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_full_scale_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_high_pass_filter_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_interrupt_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_operation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.282739 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21195 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/h3lis200dl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.286739 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-17 15:17:13.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-17 15:17:13.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:17:13.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:17:13.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 15:17:13.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:17:13.286739 micropython-h3lis200dl-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:00.036225 micropython-h3lis200dl-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:00.032225 micropython-h3lis200dl-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:00.032225 micropython-h3lis200dl-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-07 13:40:00.036225 micropython-h3lis200dl-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:00.036225 micropython-h3lis200dl-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:00.036225 micropython-h3lis200dl-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:00.036225 micropython-h3lis200dl-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-07 13:39:52.000000 micropython-h3lis200dl-0.1.2/examples/h3lis200dl_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-07 13:39:52.000000 micropython-h3lis200dl-0.1.2/examples/h3lis200dl_full_scale_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-07 13:39:52.000000 micropython-h3lis200dl-0.1.2/examples/h3lis200dl_high_pass_filter_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-07 13:39:52.000000 micropython-h3lis200dl-0.1.2/examples/h3lis200dl_interrupt_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-07 13:39:52.000000 micropython-h3lis200dl-0.1.2/examples/h3lis200dl_operation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-07 13:39:52.000000 micropython-h3lis200dl-0.1.2/examples/h3lis200dl_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:00.036225 micropython-h3lis200dl-0.1.2/micropython_h3lis200dl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:39:52.000000 micropython-h3lis200dl-0.1.2/micropython_h3lis200dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21496 2023-08-07 13:39:52.000000 micropython-h3lis200dl-0.1.2/micropython_h3lis200dl/h3lis200dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 13:39:52.000000 micropython-h3lis200dl-0.1.2/micropython_h3lis200dl/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:00.036225 micropython-h3lis200dl-0.1.2/micropython_h3lis200dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-07 13:40:00.000000 micropython-h3lis200dl-0.1.2/micropython_h3lis200dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-07 13:40:00.000000 micropython-h3lis200dl-0.1.2/micropython_h3lis200dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:40:00.000000 micropython-h3lis200dl-0.1.2/micropython_h3lis200dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 13:40:00.000000 micropython-h3lis200dl-0.1.2/micropython_h3lis200dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-07 13:39:52.000000 micropython-h3lis200dl-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:39:42.000000 micropython-h3lis200dl-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:40:00.036225 micropython-h3lis200dl-0.1.2/setup.cfg
```

### Comparing `micropython-h3lis200dl-0.1.1/.pre-commit-config.yaml` & `micropython-h3lis200dl-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-h3lis200dl-0.1.1/.pylintrc` & `micropython-h3lis200dl-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.1/LICENSE` & `micropython-h3lis200dl-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.1/PKG-INFO` & `micropython-h3lis200dl-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-h3lis200dl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Micropython Driver for the ST H3LIS200DL Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_H3LIS200DL
 Keywords: sensor,micropython,h3lis200dl,aceleration,Micropython,gravity,accelerometer,H3LIS200DL
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -23,15 +23,14 @@
     :target: https://micropython.org
     :alt: micropython
 
 .. image:: https://readthedocs.org/projects/micropython-h3lis200dl/badge/?version=latest
     :target: https://micropython-h3lis200dl.readthedocs.io/en/latest/
     :alt: Documentation Status
 
-
 .. image:: https://img.shields.io/pypi/v/micropython-h3lis200dl.svg
     :alt: latest version on PyPI
     :target: https://pypi.python.org/pypi/micropython-h3lis200dl
 
 .. image:: https://static.pepy.tech/personalized-badge/micropython-h3lis200dl?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
     :alt: Total PyPI downloads
     :target: https://pepy.tech/project/micropython-h3lis200dl
```

### Comparing `micropython-h3lis200dl-0.1.1/README.rst` & `micropython-h3lis200dl-0.1.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     :target: https://micropython.org
     :alt: micropython
 
 .. image:: https://readthedocs.org/projects/micropython-h3lis200dl/badge/?version=latest
     :target: https://micropython-h3lis200dl.readthedocs.io/en/latest/
     :alt: Documentation Status
 
-
 .. image:: https://img.shields.io/pypi/v/micropython-h3lis200dl.svg
     :alt: latest version on PyPI
     :target: https://pypi.python.org/pypi/micropython-h3lis200dl
 
 .. image:: https://static.pepy.tech/personalized-badge/micropython-h3lis200dl?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
     :alt: Total PyPI downloads
     :target: https://pepy.tech/project/micropython-h3lis200dl
```

### Comparing `micropython-h3lis200dl-0.1.1/docs/_static/Logo.png` & `micropython-h3lis200dl-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.1/docs/examples.rst` & `micropython-h3lis200dl-0.1.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.1/examples/h3lis200dl_data_rate.py` & `micropython-h3lis200dl-0.1.2/examples/h3lis200dl_data_rate.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 h3lis.data_rate = h3lis200dl.RATE_400HZ
 
 while True:
     for data_rate in h3lis200dl.data_rate_values:
         print("Current Data rate setting: ", h3lis.data_rate)
         for _ in range(10):
             accx, accy, accz = h3lis.acceleration
-            print("x:{:.2f}g, y:{:.2f}g, z:{:.2f}g".format(accx, accy, accz))
+            print(f"x:{accx:2f}g, y:{accy:2f}g, z:{accz:2f}g")
             time.sleep(0.5)
         h3lis.data_rate = data_rate
```

### Comparing `micropython-h3lis200dl-0.1.1/examples/h3lis200dl_high_pass_filter_cutoff.py` & `micropython-h3lis200dl-0.1.2/examples/h3lis200dl_high_pass_filter_cutoff.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 while True:
     for high_pass_filter_cutoff in h3lis200dl.high_pass_filter_cutoff_values:
         print(
             "Current High pass filter cutoff setting: ", h3lis.high_pass_filter_cutoff
         )
         for _ in range(10):
             accx, accy, accz = h3lis.acceleration
-            print("x:{:.2f}g, y:{:.2f}g, z:{:.2f}g".format(accx, accy, accz))
+            print(f"x:{accx:2f}g, y:{accy:2f}g, z:{accz:2f}g")
             time.sleep(0.5)
         h3lis.high_pass_filter_cutoff = high_pass_filter_cutoff
```

### Comparing `micropython-h3lis200dl-0.1.1/examples/h3lis200dl_interrupt_example.py` & `micropython-h3lis200dl-0.1.2/examples/h3lis200dl_interrupt_example.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 h3lis.interrupt1_threshold = 2  # roughly 1.5 gs
 h3lis.interrupt1_duration = 127  # Latch for 127 steps
 h3lis.interrupt1_configuration = 42  # 0b101010 See Datasheet for options
 h3lis.interrupt1_latched = 1  # 1 for True interrupt 1
 
 while True:
     accx, accy, accz = h3lis.acceleration
-    print("x:{:.2f}g, y:{:.2f}g, z:{:.2f}g".format(accx, accy, accz))
+    print(f"x:{accx:2f}g, y:{accy:2f}g, z:{accz:2f}g")
     print(h3lis.interrupt1_source_register)
     time.sleep(1)
```

### Comparing `micropython-h3lis200dl-0.1.1/examples/h3lis200dl_operation_mode.py` & `micropython-h3lis200dl-0.1.2/examples/h3lis200dl_operation_mode.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 h3lis.operation_mode = h3lis200dl.LOW_POWER_ODR0_5
 
 while True:
     for operation_mode in h3lis200dl.operation_mode_values:
         print("Current Operation mode setting: ", h3lis.operation_mode)
         for _ in range(10):
             accx, accy, accz = h3lis.acceleration
-            print("x:{:.2f}g, y:{:.2f}g, z:{:.2f}g".format(accx, accy, accz))
+            print(f"x:{accx:2f}g, y:{accy:2f}g, z:{accz:2f}g")
             time.sleep(0.5)
         h3lis.operation_mode = operation_mode
```

### Comparing `micropython-h3lis200dl-0.1.1/examples.json` & `micropython-h3lis200dl-0.1.2/examples.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'version'": "'1'"}*

```diff
@@ -21,9 +21,9 @@
             "github:jposada202020/MicroPython_H3LIS200DL/examples/h3lis200dl_full_scale_selection.py"
         ],
         [
             "micropython_h3lis200dl/examples/h3lis200dl_data_rate.py",
             "github:jposada202020/MicroPython_H3LIS200DL/examples/h3lis200dl_data_rate.py"
         ]
     ],
-    "version": "0.1"
+    "version": "1"
 }
```

### Comparing `micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/h3lis200dl.py` & `micropython-h3lis200dl-0.1.2/micropython_h3lis200dl/h3lis200dl.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_H3LIS200DL.git"
 
 _REG_WHOAMI = const(0x0F)
 _CTRL_REG1 = const(0x20)
 _CTRL_REG2 = const(0x21)
 _CTRL_REG3 = const(0x22)
 _CTRL_REG4 = const(0x23)
@@ -96,41 +96,47 @@
 
 AlertStatus = namedtuple("AlertStatus", ["high_g", "low_g"])
 
 
 # pylint: disable=too-many-instance-attributes
 class H3LIS200DL:
     """Driver for the H3LIS200DL Sensor connected over I2C.
+    The H3LIS200DL is a low-power high-performance 3-axis linear accelerometer
+
+    The H3LIS200DL has scales of ±100g/±200g and is capable of measuring
+    accelerations with output data rates from 0.5 Hz to 1 kHz.
 
     :param ~machine.I2C i2c: The I2C bus the H3LIS200DL is connected to.
-    :param int address: The I2C device address. Defaults to :const:`0x69`
+    :param int address: The I2C device address. Defaults to :const:`0x19`
 
     :raises RuntimeError: if the sensor is not found
 
     **Quickstart: Importing and using the device**
 
     Here is an example of using the :class:`H3LIS200DL` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import h3lis200dl
+        from micropython_h3lis200dl import h3lis200dl
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         h3lis200dl = h3lis200dl.H3LIS200DL(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
+        accx, accy, accz = h3lis200dl.acceleration
+
     """
 
     _device_id = RegisterStruct(_REG_WHOAMI, "B")
     _int1_configuration = RegisterStruct(_INT1_CFG, "B")
     _int1_source_register = RegisterStruct(_INT1_SRC, "B")
     _int1_threshold = RegisterStruct(_INT1_THS, "B")
     _int1_duration = RegisterStruct(_INT1_DURATION, "B")
```

### Comparing `micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/i2c_helpers.py` & `micropython-h3lis200dl-0.1.2/micropython_h3lis200dl/i2c_helpers.py`

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

### Comparing `micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/PKG-INFO` & `micropython-h3lis200dl-0.1.2/micropython_h3lis200dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-h3lis200dl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Micropython Driver for the ST H3LIS200DL Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_H3LIS200DL
 Keywords: sensor,micropython,h3lis200dl,aceleration,Micropython,gravity,accelerometer,H3LIS200DL
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -23,15 +23,14 @@
     :target: https://micropython.org
     :alt: micropython
 
 .. image:: https://readthedocs.org/projects/micropython-h3lis200dl/badge/?version=latest
     :target: https://micropython-h3lis200dl.readthedocs.io/en/latest/
     :alt: Documentation Status
 
-
 .. image:: https://img.shields.io/pypi/v/micropython-h3lis200dl.svg
     :alt: latest version on PyPI
     :target: https://pypi.python.org/pypi/micropython-h3lis200dl
 
 .. image:: https://static.pepy.tech/personalized-badge/micropython-h3lis200dl?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
     :alt: Total PyPI downloads
     :target: https://pepy.tech/project/micropython-h3lis200dl
```

### Comparing `micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/SOURCES.txt` & `micropython-h3lis200dl-0.1.2/micropython_h3lis200dl.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

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
@@ -28,9 +28,8 @@
 examples/h3lis200dl_simpletest.py
 micropython_h3lis200dl/__init__.py
 micropython_h3lis200dl/h3lis200dl.py
 micropython_h3lis200dl/i2c_helpers.py
 micropython_h3lis200dl.egg-info/PKG-INFO
 micropython_h3lis200dl.egg-info/SOURCES.txt
 micropython_h3lis200dl.egg-info/dependency_links.txt
-micropython_h3lis200dl.egg-info/requires.txt
 micropython_h3lis200dl.egg-info/top_level.txt
```

### Comparing `micropython-h3lis200dl-0.1.1/pyproject.toml` & `micropython-h3lis200dl-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-h3lis200dl"
 description = "Micropython Driver for the ST H3LIS200DL Accelerometer"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_H3LIS200DL"}
 keywords = [
     "sensor",
@@ -36,11 +36,11 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["h3lis200dl"]
+packages = ["micropython_h3lis200dl"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

