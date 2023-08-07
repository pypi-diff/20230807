# Comparing `tmp/pyfritzhome-0.6.8.tar.gz` & `tmp/pyfritzhome-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-fritzhome/python-fritzhome/dist/.tmp-ef4javgt/pyfritzhome-0.6.8.tar", last modified: Fri Mar  3 22:23:17 2023, max compression
+gzip compressed data, was "/home/runner/work/python-fritzhome/python-fritzhome/dist/.tmp-x1uxjsov/pyfritzhome-0.6.9.tar", last modified: Mon Aug  7 18:23:34 2023, max compression
```

## Comparing `pyfritzhome-0.6.8.tar` & `pyfritzhome-0.6.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/pyfritzhome/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicealarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedeviceblind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicebutton.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicefeatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicelightbulb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicepowermeter.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicerepeater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedeviceswitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicetemperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicethermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomeentitybase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhometemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14073 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/fritzhome.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/pyfritzhome/fritzhomedevice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/pyfritzhome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/pyfritzhome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/pyfritzhome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/pyfritzhome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/pyfritzhome.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/pyfritzhome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/pyfritzhome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:23:17.000000 pyfritzhome-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhomedevicealarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhomedevicebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhomedeviceblind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhomedevicebutton.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhomedevicelightbulb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhomedevicepowermeter.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhomedevicerepeater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhomedeviceswitch.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhomedevicetemperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhomedevicethermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-03-03 22:23:08.000000 pyfritzhome-0.6.8/tests/test_fritzhometemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/pyfritzhome/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicealarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedeviceblind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicebutton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicefeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicelightbulb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicepowermeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicerepeater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedeviceswitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicetemperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicethermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomeentitybase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhometemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/fritzhome.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/pyfritzhome/fritzhomedevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/pyfritzhome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/pyfritzhome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/pyfritzhome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/pyfritzhome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/pyfritzhome.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/pyfritzhome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/pyfritzhome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:23:34.000000 pyfritzhome-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhomedevicealarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhomedevicebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhomedeviceblind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhomedevicebutton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhomedevicelightbulb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhomedevicepowermeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhomedevicerepeater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhomedeviceswitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhomedevicetemperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhomedevicethermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-08-07 18:23:24.000000 pyfritzhome-0.6.9/tests/test_fritzhometemplate.py
```

### Comparing `pyfritzhome-0.6.8/LICENSE` & `pyfritzhome-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/PKG-INFO` & `pyfritzhome-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfritzhome
-Version: 0.6.8
+Version: 0.6.9
 Summary: Fritz!Box Smarthome Python Library
 Home-page: http://github.com/hthiery/python-fritzhome
 Author: Heiko Thiery
 Author-email: heiko.thiery@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfritzhome-0.6.8/README.rst` & `pyfritzhome-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/cli.py` & `pyfritzhome-0.6.9/pyfritzhome/cli.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/__init__.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicealarm.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicealarm.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicebase.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicebase.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedeviceblind.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedeviceblind.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicebutton.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicebutton.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicelightbulb.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicelightbulb.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicepowermeter.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicepowermeter.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicerepeater.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicerepeater.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedeviceswitch.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedeviceswitch.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicetemperature.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicetemperature.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomedevicethermostat.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomedevicethermostat.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhomeentitybase.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhomeentitybase.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/devicetypes/fritzhometemplate.py` & `pyfritzhome-0.6.9/pyfritzhome/devicetypes/fritzhometemplate.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome/fritzhome.py` & `pyfritzhome-0.6.9/pyfritzhome/fritzhome.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,28 +88,22 @@
 
         if rf == bool:
             return bool(int(plain))
         return rf(plain)
 
     def login(self):
         """Login and get a valid session ID."""
-        try:
-            (sid, challenge) = self._login_request()
-            if sid == "0000000000000000":
-                secret = self._create_login_secret(challenge, self._password)
-                (sid2, challenge) = self._login_request(
-                    username=self._user, secret=secret
-                )
-                if sid2 == "0000000000000000":
-                    _LOGGER.warning("login failed %s", sid2)
-                    raise LoginError(self._user)
-                self._sid = sid2
-        except Exception as ex:
-            _LOGGER.error(ex)
-            raise LoginError(self._user)
+        (sid, challenge) = self._login_request()
+        if sid == "0000000000000000":
+            secret = self._create_login_secret(challenge, self._password)
+            (sid2, challenge) = self._login_request(username=self._user, secret=secret)
+            if sid2 == "0000000000000000":
+                _LOGGER.warning("login failed %s", sid2)
+                raise LoginError(self._user)
+            self._sid = sid2
 
     def logout(self):
         """Logout."""
         self._logout_request()
         self._sid = None
 
     def get_prefixed_host(self):
```

### Comparing `pyfritzhome-0.6.8/pyfritzhome/fritzhomedevice.py` & `pyfritzhome-0.6.9/pyfritzhome/fritzhomedevice.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/pyfritzhome.egg-info/PKG-INFO` & `pyfritzhome-0.6.9/pyfritzhome.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfritzhome
-Version: 0.6.8
+Version: 0.6.9
 Summary: Fritz!Box Smarthome Python Library
 Home-page: http://github.com/hthiery/python-fritzhome
 Author: Heiko Thiery
 Author-email: heiko.thiery@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfritzhome-0.6.8/pyfritzhome.egg-info/SOURCES.txt` & `pyfritzhome-0.6.9/pyfritzhome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/setup.cfg` & `pyfritzhome-0.6.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyfritzhome
-version = 0.6.8
+version = 0.6.9
 description = Fritz!Box Smarthome Python Library
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = http://github.com/hthiery/python-fritzhome
 author = Heiko Thiery
 author_email = heiko.thiery@gmail.com
 license = MIT
```

### Comparing `pyfritzhome-0.6.8/tests/test_fritzhome.py` & `pyfritzhome-0.6.9/tests/test_fritzhome.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 
+from requests.exceptions import ConnectionError
 from unittest.mock import MagicMock, patch
 
 import pytest
 
 from pyfritzhome import Fritzhome, InvalidError, LoginError
 
 from .helper import Helper
@@ -17,15 +18,22 @@
 
     def test_login_fail(self):
         self.mock.side_effect = [
             Helper.response("login_rsp_without_valid_sid"),
             Helper.response("login_rsp_without_valid_sid"),
         ]
 
-        with pytest.raises(LoginError):
+        with pytest.raises(LoginError) as ex:
+            self.fritz.login()
+        assert str(ex.value) == 'login for user="user" failed'
+
+    def test_login_connection_error(self):
+        self.mock.side_effect = ConnectionError
+
+        with pytest.raises(ConnectionError):
             self.fritz.login()
 
     def test_login(self):
         self.mock.side_effect = [
             Helper.response("login_rsp_without_valid_sid"),
             Helper.response("login_rsp_with_valid_sid"),
         ]
```

### Comparing `pyfritzhome-0.6.8/tests/test_fritzhomedevicealarm.py` & `pyfritzhome-0.6.9/tests/test_fritzhomedevicealarm.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/tests/test_fritzhomedevicebase.py` & `pyfritzhome-0.6.9/tests/test_fritzhomedevicebase.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/tests/test_fritzhomedeviceblind.py` & `pyfritzhome-0.6.9/tests/test_fritzhomedeviceblind.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/tests/test_fritzhomedevicebutton.py` & `pyfritzhome-0.6.9/tests/test_fritzhomedevicebutton.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/tests/test_fritzhomedevicelightbulb.py` & `pyfritzhome-0.6.9/tests/test_fritzhomedevicelightbulb.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/tests/test_fritzhomedevicepowermeter.py` & `pyfritzhome-0.6.9/tests/test_fritzhomedevicepowermeter.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/tests/test_fritzhomedeviceswitch.py` & `pyfritzhome-0.6.9/tests/test_fritzhomedeviceswitch.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/tests/test_fritzhomedevicetemperature.py` & `pyfritzhome-0.6.9/tests/test_fritzhomedevicetemperature.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/tests/test_fritzhomedevicethermostat.py` & `pyfritzhome-0.6.9/tests/test_fritzhomedevicethermostat.py`

 * *Files identical despite different names*

### Comparing `pyfritzhome-0.6.8/tests/test_fritzhometemplate.py` & `pyfritzhome-0.6.9/tests/test_fritzhometemplate.py`

 * *Files identical despite different names*

