# Comparing `tmp/adafruit-circuitpython-bme680-3.5.0.tar.gz` & `tmp/adafruit-circuitpython-bme680-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bme680-3.5.0.tar", last modified: Mon Jun  5 20:57:14 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-bme680-3.6.0.tar", last modified: Mon Aug  7 17:20:43 2023, max compression
```

## Comparing `adafruit-circuitpython-bme680-3.5.0.tar` & `adafruit-circuitpython-bme680-3.6.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.368552 adafruit-circuitpython-bme680-3.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.376552 adafruit-circuitpython-bme680-3.5.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.376552 adafruit-circuitpython-bme680-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.380552 adafruit-circuitpython-bme680-3.5.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    29359 2023-06-05 20:57:06.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_bme680.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.380552 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-05 20:57:14.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-05 20:57:14.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:57:14.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 20:57:14.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 20:57:14.000000 adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/contributors.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-05 20:57:06.000000 adafruit-circuitpython-bme680-3.5.0/examples/bme680_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-05 20:57:06.000000 adafruit-circuitpython-bme680-3.5.0/examples/bme680_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-05 20:57:06.000000 adafruit-circuitpython-bme680-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-05 20:56:58.000000 adafruit-circuitpython-bme680-3.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:57:14.384552 adafruit-circuitpython-bme680-3.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:43.370575 adafruit-circuitpython-bme680-3.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:43.358575 adafruit-circuitpython-bme680-3.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:43.362575 adafruit-circuitpython-bme680-3.6.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:43.362575 adafruit-circuitpython-bme680-3.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:43.362575 adafruit-circuitpython-bme680-3.6.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-08-07 17:20:43.370575 adafruit-circuitpython-bme680-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    29360 2023-08-07 17:20:34.000000 adafruit-circuitpython-bme680-3.6.0/adafruit_bme680.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:43.366575 adafruit-circuitpython-bme680-3.6.0/adafruit_circuitpython_bme680.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-08-07 17:20:43.000000 adafruit-circuitpython-bme680-3.6.0/adafruit_circuitpython_bme680.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-07 17:20:43.000000 adafruit-circuitpython-bme680-3.6.0/adafruit_circuitpython_bme680.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:20:43.000000 adafruit-circuitpython-bme680-3.6.0/adafruit_circuitpython_bme680.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 17:20:43.000000 adafruit-circuitpython-bme680-3.6.0/adafruit_circuitpython_bme680.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 17:20:43.000000 adafruit-circuitpython-bme680-3.6.0/adafruit_circuitpython_bme680.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/contributors.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:43.366575 adafruit-circuitpython-bme680-3.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:43.366575 adafruit-circuitpython-bme680-3.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:20:43.366575 adafruit-circuitpython-bme680-3.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 17:20:34.000000 adafruit-circuitpython-bme680-3.6.0/examples/bme680_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-07 17:20:34.000000 adafruit-circuitpython-bme680-3.6.0/examples/bme680_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-07 17:20:34.000000 adafruit-circuitpython-bme680-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-07 17:20:25.000000 adafruit-circuitpython-bme680-3.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 17:20:43.370575 adafruit-circuitpython-bme680-3.6.0/setup.cfg
```

### Comparing `adafruit-circuitpython-bme680-3.5.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bme680-3.6.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/.gitignore` & `adafruit-circuitpython-bme680-3.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/.pre-commit-config.yaml` & `adafruit-circuitpython-bme680-3.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/.pylintrc` & `adafruit-circuitpython-bme680-3.6.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bme680-3.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/LICENSE` & `adafruit-circuitpython-bme680-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/LICENSES/BSD-3-Clause.txt` & `adafruit-circuitpython-bme680-3.6.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bme680-3.6.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/LICENSES/MIT.txt` & `adafruit-circuitpython-bme680-3.6.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bme680-3.6.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/PKG-INFO` & `adafruit-circuitpython-bme680-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bme680
-Version: 3.5.0
+Version: 3.6.0
 Summary: CircuitPython driver for BME680 sensor over I2C
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BME680
 Keywords: adafruit,blinka,circuitpython,micropython,bme680,hardware,temperature,pressure,humidity,gas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bme680-3.5.0/README.rst` & `adafruit-circuitpython-bme680-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/adafruit_bme680.py` & `adafruit-circuitpython-bme680-3.6.0/adafruit_bme680.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     from circuitpython_typing import ReadableBuffer
     from busio import I2C, SPI
     from digitalio import DigitalInOut
 
 except ImportError:
     pass
 
-__version__ = "3.5.0"
+__version__ = "3.6.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BME680.git"
 
 
 # garberw added begin  ===========================
 #    I2C ADDRESS/BITS/SETTINGS NEW
 #    -----------------------------------------------------------------------
 _BME68X_ENABLE_HEATER = const(0x00)
@@ -387,15 +387,15 @@
         self._perform_reading()
         if self._chip_variant == 0x01:
             # taken from https://github.com/BoschSensortec/BME68x-Sensor-API
             var1 = 262144 >> self._gas_range
             var2 = self._adc_gas - 512
             var2 *= 3
             var2 = 4096 + var2
-            calc_gas_res = (1000 * var1) / var2
+            calc_gas_res = (10000 * var1) / var2
             calc_gas_res = calc_gas_res * 100
         else:
             var1 = (
                 (1340 + (5 * self._sw_err)) * (_LOOKUP_TABLE_1[self._gas_range])
             ) / 65536
             var2 = ((self._adc_gas * 32768) - 16777216) + var1
             var3 = (_LOOKUP_TABLE_2[self._gas_range] * var1) / 512
```

### Comparing `adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/PKG-INFO` & `adafruit-circuitpython-bme680-3.6.0/adafruit_circuitpython_bme680.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bme680
-Version: 3.5.0
+Version: 3.6.0
 Summary: CircuitPython driver for BME680 sensor over I2C
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BME680
 Keywords: adafruit,blinka,circuitpython,micropython,bme680,hardware,temperature,pressure,humidity,gas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bme680-3.5.0/adafruit_circuitpython_bme680.egg-info/SOURCES.txt` & `adafruit-circuitpython-bme680-3.6.0/adafruit_circuitpython_bme680.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/docs/_static/favicon.ico` & `adafruit-circuitpython-bme680-3.6.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/docs/conf.py` & `adafruit-circuitpython-bme680-3.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/docs/index.rst` & `adafruit-circuitpython-bme680-3.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/examples/bme680_simpletest.py` & `adafruit-circuitpython-bme680-3.6.0/examples/bme680_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/examples/bme680_spi.py` & `adafruit-circuitpython-bme680-3.6.0/examples/bme680_spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.5.0/pyproject.toml` & `adafruit-circuitpython-bme680-3.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bme680"
 description = "CircuitPython driver for BME680 sensor over I2C"
-version = "3.5.0"
+version = "3.6.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BME680"}
 keywords = [
     "adafruit",
```

