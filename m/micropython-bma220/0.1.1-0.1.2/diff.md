# Comparing `tmp/micropython-bma220-0.1.1.tar.gz` & `tmp/micropython-bma220-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-bma220-0.1.1.tar", last modified: Sat Jun 17 14:00:39 2023, max compression
+gzip compressed data, was "micropython-bma220-0.1.2.tar", last modified: Mon Aug  7 13:34:15 2023, max compression
```

## Comparing `micropython-bma220-0.1.1.tar` & `micropython-bma220-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.151820 micropython-bma220-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.139820 micropython-bma220-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.143820 micropython-bma220-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-17 14:00:39.151820 micropython-bma220-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.143820 micropython-bma220-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.143820 micropython-bma220-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.147820 micropython-bma220-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_acc_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_double_tap_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_filter_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_latched_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_lowg_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_sleep_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_slope_slope_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_slope_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.147820 micropython-bma220-0.1.1/micropython_bma220/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220_lowg_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220_slope.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220_tap_sensing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.151820 micropython-bma220-0.1.1/micropython_bma220.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-17 14:00:39.000000 micropython-bma220-0.1.1/micropython_bma220.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-17 14:00:39.000000 micropython-bma220-0.1.1/micropython_bma220.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:00:39.000000 micropython-bma220-0.1.1/micropython_bma220.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:00:39.000000 micropython-bma220-0.1.1/micropython_bma220.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 14:00:39.000000 micropython-bma220-0.1.1/micropython_bma220.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:00:39.151820 micropython-bma220-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:34:15.864417 micropython-bma220-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:34:15.860417 micropython-bma220-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:34:15.860417 micropython-bma220-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-08-07 13:34:15.864417 micropython-bma220-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:34:15.860417 micropython-bma220-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:34:15.860417 micropython-bma220-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:34:15.864417 micropython-bma220-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/examples/bma220_acc_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/examples/bma220_double_tap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/examples/bma220_filter_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/examples/bma220_latched_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/examples/bma220_lowg_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/examples/bma220_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/examples/bma220_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/examples/bma220_sleep_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/examples/bma220_slope_slope_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/examples/bma220_slope_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:34:15.864417 micropython-bma220-0.1.2/micropython_bma220/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/micropython_bma220/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/micropython_bma220/bma220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/micropython_bma220/bma220_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/micropython_bma220/bma220_lowg_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/micropython_bma220/bma220_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/micropython_bma220/bma220_slope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/micropython_bma220/bma220_tap_sensing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/micropython_bma220/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:34:15.864417 micropython-bma220-0.1.2/micropython_bma220.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-08-07 13:34:15.000000 micropython-bma220-0.1.2/micropython_bma220.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-07 13:34:15.000000 micropython-bma220-0.1.2/micropython_bma220.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:34:15.000000 micropython-bma220-0.1.2/micropython_bma220.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 13:34:15.000000 micropython-bma220-0.1.2/micropython_bma220.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-07 13:34:07.000000 micropython-bma220-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:33:59.000000 micropython-bma220-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:34:15.864417 micropython-bma220-0.1.2/setup.cfg
```

### Comparing `micropython-bma220-0.1.1/.pre-commit-config.yaml` & `micropython-bma220-0.1.2/.pre-commit-config.yaml`

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

### Comparing `micropython-bma220-0.1.1/.pylintrc` & `micropython-bma220-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.1/LICENSE` & `micropython-bma220-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.1/PKG-INFO` & `micropython-bma220-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-bma220
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Bosch BMA220 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMA220
-Keywords: sensor,micropython,bma220,acceleration,driver,bosch,bma220,accelerometer,gravity,slope,tap,orientation
+Keywords: sensor,micropython,bma220,acceleration,driver,bosch,accelerometer,gravity,slope,tap,orientation
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-bma220-0.1.1/README.rst` & `micropython-bma220-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.1/docs/_static/Logo.png` & `micropython-bma220-0.1.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.1/docs/examples.rst` & `micropython-bma220-0.1.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.1/examples/bma220_acc_range.py` & `micropython-bma220-0.1.2/examples/bma220_sleep_duration.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import time
 from machine import Pin, I2C
 from micropython_bma220 import bma220
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 bma = bma220.BMA220(i2c)
 
-bma.acc_range = bma220.ACC_RANGE_16
+bma.sleep_duration = bma220.SLEEP_10MS
 
 while True:
-    for acc_range in bma220.acc_range_values:
-        print("Current Acc range setting: ", bma.acc_range)
+    for sleep_duration in bma220.sleep_duration_values:
+        print("Current Sleep duration setting: ", bma.sleep_duration)
         for _ in range(10):
             accx, accy, accz = bma.acceleration
-            print("x:{:.2f}m/s2, y:{:.2f}m/s2, z:{:.2f}m/s2".format(accx, accy, accz))
+            print(f"x:{accx:.2f}m/s², y:{accy:.2f}m/s², z:{accz:.2f}m/s²")
             time.sleep(0.5)
-        bma.acc_range = acc_range
+        bma.sleep_duration = sleep_duration
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-bma220-0.1.1/examples/bma220_double_tap_test.py` & `micropython-bma220-0.1.2/examples/bma220_double_tap_test.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.1/examples/bma220_filter_bandwidth.py` & `micropython-bma220-0.1.2/examples/bma220_filter_bandwidth.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 bma.filter_bandwidth = bma220.ACCEL_500HZ
 
 while True:
     for filter_bandwidth in bma220.filter_bandwidth_values:
         print("Current Filter bandwidth setting: ", bma.filter_bandwidth)
         for _ in range(10):
             accx, accy, accz = bma.acceleration
-            print("x:{:.2f}g, y:{:.2f}g, z:{:.2f}g".format(accx, accy, accz))
+            print(f"x:{accx:.2f}m/s², y:{accy:.2f}m/s², z:{accz:.2f}m/s²")
             time.sleep(0.5)
         bma.filter_bandwidth = filter_bandwidth
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-bma220-0.1.1/examples/bma220_latched_mode.py` & `micropython-bma220-0.1.2/examples/bma220_latched_mode.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 bma.latched_mode = bma220.LATCH_FOR_2S
 
 while True:
     for latched_mode in bma220.latched_mode_values:
         print("Current Latched mode setting: ", bma.latched_mode)
         for _ in range(10):
             accx, accy, accz = bma.acceleration
-            print("x:{:.2f}g, y:{:.2f}g, z:{:.2f}g".format(accx, accy, accz))
+            print(f"x:{accx:.2f}m/s², y:{accy:.2f}m/s², z:{accz:.2f}m/s²")
             time.sleep(0.5)
         bma.latched_mode = latched_mode
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-bma220-0.1.1/examples/bma220_orientation.py` & `micropython-bma220-0.1.2/examples/bma220_orientation.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.1/examples/bma220_slope_slope_sign.py` & `micropython-bma220-0.1.2/examples/bma220_slope_slope_sign.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 
 while True:
     for slope_sign in bma220_slope.slope_sign_values:
         print("Current Slope sign setting: ", bma.slope_sign)
         for _ in range(10):
             print("Slope Interrupt Triggered:", bma.slope_interrupt)
             infox, infoy, infoz = bma.slope_interrupt_info
-            print("Slope First interrupt x:{} y:{} z:{}".format(infox, infoy, infoz))
+            print(f"Slope x:{infox}, y:{infoy}, z:{infoz}")
             time.sleep(0.5)
         bma.slope_sign = slope_sign
```

### Comparing `micropython-bma220-0.1.1/examples/bma220_slope_test.py` & `micropython-bma220-0.1.2/examples/bma220_slope_test.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.1/examples.json` & `micropython-bma220-0.1.2/examples.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'version'": "'1'"}*

```diff
@@ -37,9 +37,9 @@
             "github:jposada202020/MicroPython_BMA220/examples/bma220_latched_mode.py"
         ],
         [
             "micropython_bma220/examples/bma220_acc_range.py",
             "github:jposada202020/MicroPython_BMA220/examples/bma220_acc_range.py"
         ]
     ],
-    "version": "0.1"
+    "version": "1"
 }
```

### Comparing `micropython-bma220-0.1.1/micropython_bma220/bma220.py` & `micropython-bma220-0.1.2/micropython_bma220/bma220.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 _REG_WHOAMI = const(0x00)
 _FILTER_CONF = const(0x20)
 _ACC_RANGE = const(0x22)
 _SLEEP_CONF = const(0x0F)
 _LATCH_CONF = const(0x1C)
@@ -103,14 +103,16 @@
     LATCH_FOR_1S,
     LATCH_FOR_2S,
     LATCH_FOR_4S,
     LATCH_FOR_8S,
     LATCHED,
 )
 
+_ACC_CONVERSION = const(9.80665)
+
 
 class BMA220:
     """Driver for the BMA220 Sensor connected over I2C.
 
     :param ~machine.I2C i2c: The I2C bus the BMA220 is connected to.
     :param int address: The I2C device address. Defaults to :const:`0x0A`
 
@@ -120,27 +122,29 @@
 
     Here is an example of using the :class:`BMA220` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import bma220
+        from micropython_bma220 import bma220
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
-        i2c = I2C(sda=Pin28), scl=Pin(3))
+        i2c = I2C(1, sda=Pin(2), scl=Pin(3))
         bma220 = bma220.BMA220(i2c)
 
     Now you have access to the attributes
 
     .. code-block:: python
 
+        accx, accy, accz = bma220.acceleration
+
     """
 
     _device_id = RegisterStruct(_REG_WHOAMI, "B")
 
     _acc_range = CBits(2, _ACC_RANGE, 0)
     _filter_bandwidth = CBits(4, _FILTER_CONF, 0)
     _latched_mode = CBits(3, _LATCH_CONF, 4)
@@ -400,15 +404,15 @@
           the INT pin is asserted and must be reset by the external master through
           the digital interface.
 
         - **Non-Latched mode**: The interrupt controller clears the INT signal once
           the interrupt condition no longer applies.
 
         The interrupt output can be programmed by :attr:`latched_mode` to be either
-        unlatched (‘000’) or latched permanently (‘111’) or have different latching times.
+        unlatched ('000') or latched permanently ('111') or have different latching times.
 
         +-----------------------------------+--------------------------------+
         | Mode                              | Value                          |
         +===================================+================================+
         | :py:const:`bma220.UNLATCHED`      | :py:const:`0b000`              |
         +-----------------------------------+--------------------------------+
         | :py:const:`bma220.LATCH_FOR_025S` | :py:const:`0b001` 0.25 seconds |
@@ -444,19 +448,19 @@
             raise ValueError("Value must be a valid latched_mode setting")
         self._latched_mode = value
 
     @property
     def acceleration(self) -> Tuple[float, float, float]:
         """
         Acceleration
-        :return: acceleration
+        :return: acceleration x, y, z in m/s²
         """
         bufx, bufy, bufz = self._acceleration
 
-        factor = acc_range_factor[self._acc_range_mem]
+        factor = acc_range_factor[self._acc_range_mem] * _ACC_CONVERSION
 
         return (
             self._twos_comp(bufx >> 2, 6) / factor,
             self._twos_comp(bufy >> 2, 6) / factor,
             self._twos_comp(bufz >> 2, 6) / factor,
         )
```

### Comparing `micropython-bma220-0.1.1/micropython_bma220/bma220_const.py` & `micropython-bma220-0.1.2/micropython_bma220/bma220_const.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * Author(s): Jose D. Montoya
 
 
 """
 
 from micropython import const
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 # pylint: disable=duplicate-code
 # Acceleration range
 ACC_RANGE_2 = const(0b00)
 ACC_RANGE_4 = const(0b01)
 ACC_RANGE_8 = const(0b10)
```

### Comparing `micropython-bma220-0.1.1/micropython_bma220/bma220_lowg_detection.py` & `micropython-bma220-0.1.2/micropython_bma220/bma220_lowg_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # pylint: disable=useless-parent-delegation,no-name-in-module
 
 from micropython import const
 from micropython_bma220.i2c_helpers import CBits
 from micropython_bma220.bma220 import BMA220
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 _CONF = const(0x1A)
 _LG_CONF = const(0x1C)
 _LG_CONF2 = const(0x0E)
 _LG_CONF3 = const(0x0C)
 _INTERRUPTS = const(0x18)
@@ -45,15 +45,15 @@
 
     _lowg_enabled = CBits(1, _LG_CONF, 3)
     _lowg_int = CBits(1, _INTERRUPTS, 3)
     _lowg_duration = CBits(5, _LG_CONF2, 0)
     _lowg_threshold = CBits(4, _LG_CONF3, 3)
     _lowg_hysteresis = CBits(2, _LG_CONF, 6)
 
-    def __init__(self, i2c_bus):
+    def __init__(self, i2c_bus) -> None:
         super().__init__(i2c_bus)
 
     @property
     def lowg_enabled(self) -> str:
         """
         Sensor _lowg_enabled
```

### Comparing `micropython-bma220-0.1.1/micropython_bma220/bma220_orientation.py` & `micropython-bma220-0.1.2/micropython_bma220/bma220_orientation.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 
 from micropython import const
 from micropython_bma220.i2c_helpers import CBits
 from micropython_bma220.bma220 import BMA220
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 _CONF = const(0x1A)
 _ORIENT_EX = const(0x12)
 _INTERRUPTS = const(0x16)
 
 # Orientation Enabled
@@ -82,15 +82,15 @@
 
     """
 
     _orientation_int = CBits(1, _INTERRUPTS, 7)
     _orientation_enabled = CBits(1, _CONF, 6)
     _orientation_exchange = CBits(1, _ORIENT_EX, 7)
 
-    def __init__(self, i2c_bus):
+    def __init__(self, i2c_bus) -> None:
         super().__init__(i2c_bus)
         self._orientation_enabled = True
 
     @property
     def orientation_enabled(self) -> str:
         """
         Sensor orientation_enabled. By default, the sensor gets enabled when starting this
```

### Comparing `micropython-bma220-0.1.1/micropython_bma220/bma220_slope.py` & `micropython-bma220-0.1.2/micropython_bma220/bma220_slope.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from micropython_bma220.bma220 import BMA220
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 _CONF = const(0x1A)
 _SLOPE_INFO = const(0x12)
 _SLOPE_INFO2 = const(0x16)
 _INTERRUPTS = const(0x18)
 
@@ -84,15 +84,15 @@
     _slope_filter_enable = CBits(1, _SLOPE_INFO, 6)
 
     _slope_sign = CBits(1, _SLOPE_INFO2, 0)
     _slope_z_first = CBits(1, _SLOPE_INFO2, 1)
     _slope_y_first = CBits(1, _SLOPE_INFO2, 2)
     _slope_x_first = CBits(1, _SLOPE_INFO2, 3)
 
-    def __init__(self, i2c_bus):
+    def __init__(self, i2c_bus) -> None:
         super().__init__(i2c_bus)
 
     @property
     def slope_x_enabled(self) -> str:
         """
         Sensor slope_x_enabled
```

### Comparing `micropython-bma220-0.1.1/micropython_bma220/bma220_tap_sensing.py` & `micropython-bma220-0.1.2/micropython_bma220/bma220_tap_sensing.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from micropython_bma220.bma220 import BMA220
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 _CONF = const(0x1A)
 _TT_INFO = const(0x10)
 _TT_INFO2 = const(0x16)
 _INTERRUPTS = const(0x18)
```

### Comparing `micropython-bma220-0.1.1/micropython_bma220/i2c_helpers.py` & `micropython-bma220-0.1.2/micropython_bma220/i2c_helpers.py`

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

### Comparing `micropython-bma220-0.1.1/micropython_bma220.egg-info/PKG-INFO` & `micropython-bma220-0.1.2/micropython_bma220.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-bma220
-Version: 0.1.1
+Version: 0.1.2
 Summary: MicroPython Driver for the Bosch BMA220 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMA220
-Keywords: sensor,micropython,bma220,acceleration,driver,bosch,bma220,accelerometer,gravity,slope,tap,orientation
+Keywords: sensor,micropython,bma220,acceleration,driver,bosch,accelerometer,gravity,slope,tap,orientation
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-bma220-0.1.1/micropython_bma220.egg-info/SOURCES.txt` & `micropython-bma220-0.1.2/micropython_bma220.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

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
@@ -37,9 +37,8 @@
 micropython_bma220/bma220_orientation.py
 micropython_bma220/bma220_slope.py
 micropython_bma220/bma220_tap_sensing.py
 micropython_bma220/i2c_helpers.py
 micropython_bma220.egg-info/PKG-INFO
 micropython_bma220.egg-info/SOURCES.txt
 micropython_bma220.egg-info/dependency_links.txt
-micropython_bma220.egg-info/requires.txt
 micropython_bma220.egg-info/top_level.txt
```

### Comparing `micropython-bma220-0.1.1/pyproject.toml` & `micropython-bma220-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,27 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-bma220"
 description = "MicroPython Driver for the Bosch BMA220 Accelerometer"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_BMA220"}
 keywords = [
     "sensor",
     "micropython",
     "bma220",
     "acceleration",
     "driver",
     "bosch",
-    "bma220",
     "accelerometer",
     "gravity",
     "slope",
     "tap",
     "orientation",
 ]
 license = {text = "MIT"}
@@ -40,11 +39,11 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["bma220"]
+packages = ["micropython_bma220"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

