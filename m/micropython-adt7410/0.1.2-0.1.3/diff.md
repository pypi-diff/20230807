# Comparing `tmp/micropython-adt7410-0.1.2.tar.gz` & `tmp/micropython-adt7410-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-adt7410-0.1.2.tar", last modified: Mon Aug  7 13:10:45 2023, max compression
+gzip compressed data, was "micropython-adt7410-0.1.3.tar", last modified: Mon Aug  7 14:49:19 2023, max compression
```

## Comparing `micropython-adt7410-0.1.2.tar` & `micropython-adt7410-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.373851 micropython-adt7410-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.365851 micropython-adt7410-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.369851 micropython-adt7410-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-07 13:10:45.373851 micropython-adt7410-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.369851 micropython-adt7410-0.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.369851 micropython-adt7410-0.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.369851 micropython-adt7410-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/examples/adt7410_operation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/examples/adt7410_resolution_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/examples/adt7410_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/examples/adt7410_temp_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.369851 micropython-adt7410-0.1.2/micropython_adt7410/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/micropython_adt7410/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/micropython_adt7410/adt7410.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/micropython_adt7410/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:10:45.373851 micropython-adt7410-0.1.2/micropython_adt7410.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-07 13:10:45.000000 micropython-adt7410-0.1.2/micropython_adt7410.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-07 13:10:45.000000 micropython-adt7410-0.1.2/micropython_adt7410.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:10:45.000000 micropython-adt7410-0.1.2/micropython_adt7410.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 13:10:45.000000 micropython-adt7410-0.1.2/micropython_adt7410.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-07 13:10:35.000000 micropython-adt7410-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:10:21.000000 micropython-adt7410-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 13:10:45.373851 micropython-adt7410-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:49:19.823458 micropython-adt7410-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:49:19.811458 micropython-adt7410-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:49:19.815458 micropython-adt7410-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-07 14:49:19.823458 micropython-adt7410-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:49:19.815458 micropython-adt7410-0.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:49:19.819458 micropython-adt7410-0.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:49:19.819458 micropython-adt7410-0.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-07 14:49:11.000000 micropython-adt7410-0.1.3/examples/adt7410_operation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-07 14:49:11.000000 micropython-adt7410-0.1.3/examples/adt7410_resolution_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 14:49:11.000000 micropython-adt7410-0.1.3/examples/adt7410_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-07 14:49:11.000000 micropython-adt7410-0.1.3/examples/adt7410_temp_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:49:19.819458 micropython-adt7410-0.1.3/micropython_adt7410/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:49:11.000000 micropython-adt7410-0.1.3/micropython_adt7410/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-08-07 14:49:11.000000 micropython-adt7410-0.1.3/micropython_adt7410/adt7410.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-07 14:49:11.000000 micropython-adt7410-0.1.3/micropython_adt7410/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:49:19.823458 micropython-adt7410-0.1.3/micropython_adt7410.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-07 14:49:19.000000 micropython-adt7410-0.1.3/micropython_adt7410.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-07 14:49:19.000000 micropython-adt7410-0.1.3/micropython_adt7410.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:49:19.000000 micropython-adt7410-0.1.3/micropython_adt7410.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 14:49:19.000000 micropython-adt7410-0.1.3/micropython_adt7410.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-07 14:49:11.000000 micropython-adt7410-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 14:49:03.000000 micropython-adt7410-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:49:19.823458 micropython-adt7410-0.1.3/setup.cfg
```

### Comparing `micropython-adt7410-0.1.2/.pre-commit-config.yaml` & `micropython-adt7410-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/.pylintrc` & `micropython-adt7410-0.1.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/LICENSE` & `micropython-adt7410-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/PKG-INFO` & `micropython-adt7410-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-adt7410
-Version: 0.1.2
+Version: 0.1.3
 Summary: MicroPython Driver for the Analog Devices ADT7410 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ADT7410
-Keywords: sensor,micropython,adt7410,temperature,adt7410,driver,micropython
+Keywords: sensor,adt7410,temperature,driver,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-adt7410-0.1.2/README.rst` & `micropython-adt7410-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/docs/_static/Logo.png` & `micropython-adt7410-0.1.3/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/docs/_static/favicon.ico` & `micropython-adt7410-0.1.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/docs/conf.py` & `micropython-adt7410-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/docs/examples.rst` & `micropython-adt7410-0.1.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/examples/adt7410_operation_mode.py` & `micropython-adt7410-0.1.3/examples/adt7410_operation_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/examples/adt7410_resolution_mode.py` & `micropython-adt7410-0.1.3/examples/adt7410_resolution_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 
 adt.resolution_mode = adt7410.HIGH_RESOLUTION
 
 while True:
     for resolution_mode in adt7410.resolution_mode_values:
         print("Current Resolution mode setting: ", adt.resolution_mode)
         for _ in range(10):
-            print(f"Temperature: {adt.temperature:.2f}°C")
+            print(f"Temperature: {adt.temperature:.4f}°C")
             print()
             time.sleep(0.5)
         adt.resolution_mode = resolution_mode
```

### Comparing `micropython-adt7410-0.1.2/examples/adt7410_temp_limits.py` & `micropython-adt7410-0.1.3/examples/adt7410_temp_limits.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 adt = adt7410.ADT7410(i2c)
 
 adt.low_temperature = 18
 adt.high_temperature = 29
 adt.critical_temperature = 35
 adt.hysteresis_temperature = 2
 
-print("High limit: {}°C".format(adt.high_temperature))
-print("Low limit: {}°C".format(adt.low_temperature))
-print("Critical limit: {}°C".format(adt.critical_temperature))
+print(f"High limit: {adt.high_temperature}°C")
+print(f"Low limit: {adt.low_temperature}°C")
+print(f"Critical limit: {adt.critical_temperature}°C")
 
 adt.comparator_mode = adt7410.COMP_ENABLED
 
 while True:
     print(f"Temperature: {adt.temperature:.2f}°C")
     print()
     alert_status = adt.alert_status
```

### Comparing `micropython-adt7410-0.1.2/examples.json` & `micropython-adt7410-0.1.3/examples.json`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/micropython_adt7410/adt7410.py` & `micropython-adt7410-0.1.3/micropython_adt7410/adt7410.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import time
 from collections import namedtuple
 from micropython import const
 from micropython_adt7410.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __repo__ = "https://github.com/jposada202020/MicroPython_ADT7410.git"
 
 
 _REG_WHOAMI = const(0xB)
 _TEMP = const(0x00)
 _STATUS = const(0x02)
 _CONFIGURATION = const(0x03)
@@ -55,15 +55,15 @@
     The ADT7410 is a high accuracy digital temperature sensor. it has
     a 13-bit ADC to monitor and digitize the temperature to a
     0.0625°C resolution.
 
     The ADC resolution, by default, is set to 13 bits (0.0625°C).
     This can be changed to 16 bits (0.0078°C) by :attr:`resolution_mode`
 
-    The ADT7410 is rated for operation over the −55°C to +150°C temperature
+    The ADT7410 is rated for operation over the -55°C to +150°C temperature
     range
 
     In normal mode, the ADT7410 runs an automatic conversion
     sequence. During this automatic conversion sequence, a conversion
     takes 240 ms to complete and the ADT7410 is continuously
     converting.
 
@@ -117,15 +117,15 @@
     _low_alert = CBits(1, _STATUS, 4)
 
     def __init__(self, i2c, address: int = 0x48) -> None:
         self._i2c = i2c
         self._address = address
 
         if self._device_id != 0xCB:
-            raise RuntimeError("Failed to find ADT7410")
+            raise RuntimeError("Failed to find the ADT7410 sensor")
 
     @property
     def operation_mode(self) -> str:
         """
         Sensor operation_mode
 
         Continuous Mode
@@ -236,31 +236,31 @@
         """The current triggered status of the high and low temperature alerts as a AlertStatus
         named tuple with attributes for the triggered status of each alert.
 
         .. code-block :: python
 
             import time
             from machine import Pin, I2C
-            from micropython_mcp9808 import mcp9808
+            from micropython_adt7410 import adat7410
 
             i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
-            mcp = mcp9808.MCP9808(i2c)
+            adt = adt7410.ADT7410(i2c)
 
             tmp.low_temperature = 20
             tmp.high_temperature = 23
             tmp.critical_temperature = 30
 
-            print("High limit: {}".format(tmp.high_temperature))
-            print("Low limit: {}".format(tmp.low_temperature))
-            print("Critical limit: {}".format(tmp.critical_temperature))
+            print(f"High limit: {tmp.high_temperature}")
+            print(f"Low limit: {tmp.low_temperature}")
+            print(f"Critical limit: {tmp.critical_temperature}")
 
             adt.comparator_mode = adt7410.COMP_ENABLED
 
             while True:
-                print("Temperature: {:.2f}C".format(adt.temperature))
+                print(f"Temperature: {adt.temperature:.2f}°C")
                 alert_status = tmp.alert_status
                 if alert_status.high_alert:
                     print("Temperature above high set limit!")
                 if alert_status.low_alert:
                     print("Temperature below low set limit!")
                 if alert_status.critical_alert:
                     print("Temperature above critical set limit!")
@@ -276,15 +276,15 @@
 
     @property
     def comparator_mode(self) -> str:
         """
         Sensor comparator_mode
         In comparator mode, the INT pin returns to its inactive status
         when the temperature drops below the
-        :attr:`high_temperature` − :attr:`hysteresis_temperature` limit or
+        :attr:`high_temperature` - :attr:`hysteresis_temperature` limit or
         rises above the :attr:`low_temperature` + :attr:`hysteresis_temperature`
         limit.
         Putting the ADT7410 into shutdown mode does not reset the
         INT state in comparator mode
 
         +-----------------------------------+-----------------+
         | Mode                              | Value           |
@@ -321,15 +321,15 @@
 
         """
         return self._temperature_high // 128
 
     @high_temperature.setter
     def high_temperature(self, value: int) -> None:
         if value not in range(-55, 151, 1):
-            raise ValueError("Temperature should be between -55C and 150C")
+            raise ValueError("Temperature should be between -55°C and 150°C")
         self._temperature_high = value * 128
 
     @property
     def low_temperature(self) -> float:
         """
         Low temperature limit value in Celsius.
         When the temperature goes below the :attr:`low_temperature`,
@@ -337,20 +337,20 @@
         low_alert clears to 0 when the status register is read and/or when
         the temperature measured goes back above the limit set in the set point
         :attr:`low_temperature` + :attr:`hysteresis_temperature`
 
         The INT pin is activated if an under temperature event occur
         The default setting is 10°C
         """
-        return self._temperature_low // 128
+        return self._temperature_low / 128
 
     @low_temperature.setter
     def low_temperature(self, value: int) -> None:
         if value not in range(-55, 151, 1):
-            raise ValueError("Temperature should be between -55C and 150C")
+            raise ValueError("Temperature should be between -55°C and 150°C")
         self._temperature_low = value * 128
 
     @property
     def critical_temperature(self) -> float:
         """
         Critical temperature limit value in Celsius
         When the temperature goes above the :attr:`critical_temperature`,
@@ -358,29 +358,29 @@
         critical_alert clears to 0 when the status register is read and/or when
         the temperature measured goes back below the limit set in
         :attr:`critical_temperature` + :attr:`hysteresis_temperature`
 
         The INT pin is activated if a critical over temperature event occur
         The default setting is 147°C
         """
-        return self._temperature_critical // 128
+        return self._temperature_critical / 128
 
     @critical_temperature.setter
     def critical_temperature(self, value: int) -> None:
         if value not in range(-55, 151, 1):
-            raise ValueError("Temperature should be between -55C and 15C")
+            raise ValueError("Temperature should be between -55°C and 150°C")
         self._temperature_critical = value * 128
 
     @property
     def hysteresis_temperature(self) -> float:
         """
         Hysteresis temperature limit value in Celsius for the
         :attr:`critical_temperature`, :attr:`high_temperature` and
         :attr:`low_temperature` limits
         """
         return self._temperature_hysteresis
 
     @hysteresis_temperature.setter
     def hysteresis_temperature(self, value: int) -> None:
         if value not in range(0, 16, 1):
-            raise ValueError("Temperature should be between 0C and 15C")
+            raise ValueError("Temperature should be between 0°C and 15°C")
         self._temperature_hysteresis = value
```

### Comparing `micropython-adt7410-0.1.2/micropython_adt7410/i2c_helpers.py` & `micropython-adt7410-0.1.3/micropython_adt7410/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/micropython_adt7410.egg-info/PKG-INFO` & `micropython-adt7410-0.1.3/micropython_adt7410.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: micropython-adt7410
-Version: 0.1.2
+Version: 0.1.3
 Summary: MicroPython Driver for the Analog Devices ADT7410 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ADT7410
-Keywords: sensor,micropython,adt7410,temperature,adt7410,driver,micropython
+Keywords: sensor,adt7410,temperature,driver,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
```

### Comparing `micropython-adt7410-0.1.2/micropython_adt7410.egg-info/SOURCES.txt` & `micropython-adt7410-0.1.3/micropython_adt7410.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.2/pyproject.toml` & `micropython-adt7410-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,31 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 [build-system]
-requires = [
-    "setuptools",
-    "wheel",
-    "setuptools-scm",
-]
+requires = ["setuptools", "wheel", "setuptools-scm"]
 
 [project]
 name = "micropython-adt7410"
 description = "MicroPython Driver for the Analog Devices ADT7410 Temperature Sensor"
-version = "0.1.2"
+version = "0.1.3"
 readme = "README.rst"
-authors = [
-    {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
-]
-urls = {Homepage = "https://github.com/jposada202020/MicroPython_ADT7410"}
-keywords = [
-    "sensor",
-    "micropython",
-    "adt7410",
-    "temperature",
-    "adt7410",
-    "driver",
-    "micropython",
-]
-license = {text = "MIT"}
+authors = [{ name = "JDM", email = "xxyx@mailmeto.mozmail.com" }]
+urls = { Homepage = "https://github.com/jposada202020/MicroPython_ADT7410" }
+keywords = ["sensor", "adt7410", "temperature", "driver", "micropython"]
+license = { text = "MIT" }
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
 packages = ["micropython_adt7410"]
 
 [tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
+dependencies = { file = ["requirements.txt"] }
```

