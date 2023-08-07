# Comparing `tmp/micropython-mcp9808-0.2.0.tar.gz` & `tmp/micropython-mcp9808-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-mcp9808-0.2.0.tar", last modified: Sun Jun 18 19:12:59 2023, max compression
+gzip compressed data, was "micropython-mcp9808-0.2.1.tar", last modified: Mon Aug  7 13:41:01 2023, max compression
```

## Comparing `micropython-mcp9808-0.2.0.tar` & `micropython-mcp9808-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.566573 micropython-mcp9808-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.566573 micropython-mcp9808-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/examples/mcp9808_hysteresis.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/examples/mcp9808_power_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/examples/mcp9808_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/examples/mcp9808_temperature_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/examples/mcp9808_temperature_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/micropython_mcp9808/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/micropython_mcp9808/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/micropython_mcp9808/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/micropython_mcp9808/mcp9808.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-18 19:12:59.000000 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-18 19:12:59.000000 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 19:12:59.000000 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 19:12:59.000000 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 19:12:59.000000 micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-18 19:12:51.000000 micropython-mcp9808-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 19:12:42.000000 micropython-mcp9808-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 19:12:59.570573 micropython-mcp9808-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:01.901215 micropython-mcp9808-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:01.897215 micropython-mcp9808-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:01.901215 micropython-mcp9808-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-08-07 13:41:01.901215 micropython-mcp9808-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:01.901215 micropython-mcp9808-0.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:01.901215 micropython-mcp9808-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:01.901215 micropython-mcp9808-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-07 13:40:54.000000 micropython-mcp9808-0.2.1/examples/mcp9808_hysteresis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-07 13:40:54.000000 micropython-mcp9808-0.2.1/examples/mcp9808_power_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 13:40:54.000000 micropython-mcp9808-0.2.1/examples/mcp9808_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-07 13:40:54.000000 micropython-mcp9808-0.2.1/examples/mcp9808_temperature_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-07 13:40:54.000000 micropython-mcp9808-0.2.1/examples/mcp9808_temperature_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:01.901215 micropython-mcp9808-0.2.1/micropython_mcp9808/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:54.000000 micropython-mcp9808-0.2.1/micropython_mcp9808/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 13:40:54.000000 micropython-mcp9808-0.2.1/micropython_mcp9808/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-08-07 13:40:54.000000 micropython-mcp9808-0.2.1/micropython_mcp9808/mcp9808.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:01.901215 micropython-mcp9808-0.2.1/micropython_mcp9808.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-08-07 13:41:01.000000 micropython-mcp9808-0.2.1/micropython_mcp9808.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-08-07 13:41:01.000000 micropython-mcp9808-0.2.1/micropython_mcp9808.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:41:01.000000 micropython-mcp9808-0.2.1/micropython_mcp9808.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 13:41:01.000000 micropython-mcp9808-0.2.1/micropython_mcp9808.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-07 13:40:54.000000 micropython-mcp9808-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:40:45.000000 micropython-mcp9808-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:41:01.901215 micropython-mcp9808-0.2.1/setup.cfg
```

### Comparing `micropython-mcp9808-0.2.0/.pre-commit-config.yaml` & `micropython-mcp9808-0.2.1/.pre-commit-config.yaml`

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

### Comparing `micropython-mcp9808-0.2.0/.pylintrc` & `micropython-mcp9808-0.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.2.0/LICENSE` & `micropython-mcp9808-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.2.0/PKG-INFO` & `micropython-mcp9808-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-mcp9808
-Version: 0.2.0
+Version: 0.2.1
 Summary: MicroPython Driver for the Microchip MCP9808 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MCP9808
-Keywords: sensor,micropython,mcp9808,temperature,microchip,mcp9808,temperature,micropython
+Keywords: sensor,mcp9808,temperature,microchip,temperature,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-mcp9808-0.2.0/README.rst` & `micropython-mcp9808-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.2.0/docs/_static/Logo.png` & `micropython-mcp9808-0.2.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.2.0/docs/examples.rst` & `micropython-mcp9808-0.2.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-mcp9808-0.2.0/examples/mcp9808_hysteresis.py` & `micropython-mcp9808-0.2.1/examples/mcp9808_hysteresis.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 
 mcp.hysteresis = mcp9808.HYSTERESIS_0
 
 while True:
     for hysteresis in mcp9808.hysteresis_values:
         print("Current Hysteresis setting: ", mcp.hysteresis)
         for _ in range(10):
-            temp = mcp.temperature
-            print("Temperature: {:.2f}C".format(temp))
+            print(f"Temperature: {mcp.temperature:.2f}°C")
+            print()
             time.sleep(0.5)
+        mcp.hysteresis = hysteresis
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-mcp9808-0.2.0/examples/mcp9808_power_mode.py` & `micropython-mcp9808-0.2.1/examples/mcp9808_power_mode.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 
 mcp.power_mode = mcp9808.SHUTDOWN
 
 while True:
     for power_mode in mcp9808.power_mode_values:
         print("Current Power mode setting: ", mcp.power_mode)
         for _ in range(10):
-            temp = mcp.temperature
-            print("Temperature: {:.2f}C".format(temp))
+            print(f"Temperature: {mcp.temperature:.2f}°C")
+            print()
             time.sleep(0.5)
+        mcp.power_mode = power_mode
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-mcp9808-0.2.0/examples/mcp9808_temperature_limits.py` & `micropython-mcp9808-0.2.1/examples/mcp9808_temperature_resolution.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,21 +5,17 @@
 import time
 from machine import Pin, I2C
 from micropython_mcp9808 import mcp9808
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 mcp = mcp9808.MCP9808(i2c)
 
-mcp.temperature_lower = 10
-mcp.temperature_upper = 25
-mcp.temperature_critical = 35
+mcp.temperature_resolution = mcp9808.RESOLUTION_0_625_C
 
 while True:
-    print("Temperature: {:.2f}C".format(mcp.temperature))
-    alert_status = mcp.alert_status
-    if alert_status.high_alert:
-        print("Temperature above high set limit!")
-    if alert_status.low_alert:
-        print("Temperature below low set limit!")
-    if alert_status.critical_alert:
-        print("Temperature above critical set limit!")
-    time.sleep(1)
+    for temperature_resolution in mcp9808.temperature_resolution_values:
+        print("Current Temperature resolution setting: ", mcp.temperature_resolution)
+        for _ in range(10):
+            print(f"Temperature: {mcp.temperature:.2f}°C")
+            print()
+            time.sleep(0.5)
+        mcp.temperature_resolution = temperature_resolution
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-mcp9808-0.2.0/examples.json` & `micropython-mcp9808-0.2.1/examples.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'version'": "'1'"}*

```diff
@@ -17,9 +17,9 @@
             "github:jposada202020/MicroPython_MCP9808/examples/mcp9808_temperature_limits.py"
         ],
         [
             "micropython_mcp9808/examples/mcp9808_temperature_resolution.py",
             "github:jposada202020/MicroPython_MCP9808/examples/mcp9808_temperature_resolution.py"
         ]
     ],
-    "version": "0.1"
+    "version": "1"
 }
```

### Comparing `micropython-mcp9808-0.2.0/micropython_mcp9808/i2c_helpers.py` & `micropython-mcp9808-0.2.1/micropython_mcp9808/i2c_helpers.py`

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

### Comparing `micropython-mcp9808-0.2.0/micropython_mcp9808/mcp9808.py` & `micropython-mcp9808-0.2.1/micropython_mcp9808/mcp9808.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 from collections import namedtuple
 from micropython import const
 from micropython_mcp9808.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_MCP9808.git"
 
 
 _CONFIG = const(0x01)
 _UPPER_TEMP = const(0x02)
 _LOWER_TEMP = const(0x03)
 _CRITICAL_TEMP = const(0x04)
@@ -170,15 +170,14 @@
         data = bytearray(2)
         self._i2c.readfrom_mem_into(self._address, _TEMP, data)
 
         return self._convert_temperature(data)
 
     @staticmethod
     def _convert_temperature(temp: bytearray) -> float:
-
         temp[0] = temp[0] & 0x1F
         if temp[0] & 0x10 == 0x10:
             temp[0] = temp[0] & 0x0F
             return (temp[0] * 16 + temp[1] / 16.0) - 256
         return temp[0] * 16 + temp[1] / 16.0
 
     @property
@@ -191,15 +190,14 @@
     @temperature_upper.setter
     def temperature_upper(self, value: int) -> None:
         if not isinstance(value, int):
             raise ValueError("Temperature must be an int value")
         self._limit_temperatures(value, _UPPER_TEMP)
 
     def _get_temperature(self, register_address):
-
         data = bytearray(2)
         self._i2c.readfrom_mem_into(self._address, register_address, data)
 
         return self._convert_temperature(data)
 
     def _limit_temperatures(self, temp: int, register_address):
         """Internal function to setup limit temperature
```

### Comparing `micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/PKG-INFO` & `micropython-mcp9808-0.2.1/micropython_mcp9808.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-mcp9808
-Version: 0.2.0
+Version: 0.2.1
 Summary: MicroPython Driver for the Microchip MCP9808 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MCP9808
-Keywords: sensor,micropython,mcp9808,temperature,microchip,mcp9808,temperature,micropython
+Keywords: sensor,mcp9808,temperature,microchip,temperature,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-mcp9808-0.2.0/micropython_mcp9808.egg-info/SOURCES.txt` & `micropython-mcp9808-0.2.1/micropython_mcp9808.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,9 +27,8 @@
 examples/mcp9808_temperature_resolution.py
 micropython_mcp9808/__init__.py
 micropython_mcp9808/i2c_helpers.py
 micropython_mcp9808/mcp9808.py
 micropython_mcp9808.egg-info/PKG-INFO
 micropython_mcp9808.egg-info/SOURCES.txt
 micropython_mcp9808.egg-info/dependency_links.txt
-micropython_mcp9808.egg-info/requires.txt
 micropython_mcp9808.egg-info/top_level.txt
```

### Comparing `micropython-mcp9808-0.2.0/pyproject.toml` & `micropython-mcp9808-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,25 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-mcp9808"
 description = "MicroPython Driver for the Microchip MCP9808 Temperature Sensor"
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_MCP9808"}
 keywords = [
     "sensor",
-    "micropython",
     "mcp9808",
     "temperature",
     "microchip",
-    "mcp9808",
     "temperature",
     "micropython",
 ]
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
```

