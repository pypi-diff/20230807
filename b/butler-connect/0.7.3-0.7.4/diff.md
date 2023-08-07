# Comparing `tmp/butler-connect-0.7.3.tar.gz` & `tmp/butler-connect-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.7.3.tar", last modified: Tue Jul 18 21:28:19 2023, max compression
+gzip compressed data, was "butler-connect-0.7.4.tar", last modified: Mon Aug  7 18:32:39 2023, max compression
```

## Comparing `butler-connect-0.7.3.tar` & `butler-connect-0.7.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 21:28:19.580041 butler-connect-0.7.3/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.7.3/LICENSE
--rw-rw-rw-   0        0        0     2828 2023-07-18 21:28:19.579101 butler-connect-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     1046 2023-07-18 21:27:25.000000 butler-connect-0.7.3/README.md
--rw-rw-rw-   0        0        0      738 2023-07-18 21:27:42.000000 butler-connect-0.7.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 21:28:19.581065 butler-connect-0.7.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 21:28:19.492148 butler-connect-0.7.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 21:28:19.501840 butler-connect-0.7.3/src/butlerConnect/
--rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.7.3/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    18719 2023-05-20 09:13:29.000000 butler-connect-0.7.3/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:28:19.534489 butler-connect-0.7.3/src/butlerDescription/
--rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.7.3/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.7.3/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.7.3/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0      512 2023-07-18 21:25:05.000000 butler-connect-0.7.3/src/butlerDescription/group.py
--rw-rw-rw-   0        0        0     2844 2023-07-18 21:21:52.000000 butler-connect-0.7.3/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:28:19.573027 butler-connect-0.7.3/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     2828 2023-07-18 21:28:19.000000 butler-connect-0.7.3/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-07-18 21:28:19.000000 butler-connect-0.7.3/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 21:28:19.000000 butler-connect-0.7.3/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-07-18 21:28:19.000000 butler-connect-0.7.3/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-07-18 21:28:19.000000 butler-connect-0.7.3/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 18:32:39.102615 butler-connect-0.7.4/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.7.4/LICENSE
+-rw-rw-rw-   0        0        0     2900 2023-08-07 18:32:39.100613 butler-connect-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2023-08-07 18:32:21.000000 butler-connect-0.7.4/README.md
+-rw-rw-rw-   0        0        0      738 2023-08-07 18:31:45.000000 butler-connect-0.7.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 18:32:39.102615 butler-connect-0.7.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 18:32:39.062277 butler-connect-0.7.4/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 18:32:39.065785 butler-connect-0.7.4/src/butlerConnect/
+-rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.7.4/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    18719 2023-05-20 09:13:29.000000 butler-connect-0.7.4/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:32:39.075870 butler-connect-0.7.4/src/butlerDescription/
+-rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.7.4/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.7.4/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.7.4/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0      512 2023-07-18 21:25:05.000000 butler-connect-0.7.4/src/butlerDescription/group.py
+-rw-rw-rw-   0        0        0     3147 2023-08-07 18:31:30.000000 butler-connect-0.7.4/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:32:39.099606 butler-connect-0.7.4/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     2900 2023-08-07 18:32:39.000000 butler-connect-0.7.4/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-08-07 18:32:39.000000 butler-connect-0.7.4/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 18:32:39.000000 butler-connect-0.7.4/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-08-07 18:32:39.000000 butler-connect-0.7.4/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-08-07 18:32:39.000000 butler-connect-0.7.4/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.7.3/LICENSE` & `butler-connect-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.3/PKG-INFO` & `butler-connect-0.7.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.7.3
+Version: 0.7.4
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -64,7 +64,10 @@
 ### 0.7.2
 - create SignalDirection()
 - add convertFrom to SignalOptionType
 - add different consumptionSignals to SignalType
 ### 0.7.3
 - add buildingHardware to signalOptionType and groupOptionType
 - add agent_building to groupOptionType
+### 0.7.4 
+- add SignalType co2
+- add SignalType consumption*Current
```

### Comparing `butler-connect-0.7.3/README.md` & `butler-connect-0.7.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,8 +28,11 @@
 - Bugifx in Signal().__init__(.. ext was missing)
 ### 0.7.2
 - create SignalDirection()
 - add convertFrom to SignalOptionType
 - add different consumptionSignals to SignalType
 ### 0.7.3
 - add buildingHardware to signalOptionType and groupOptionType
-- add agent_building to groupOptionType
+- add agent_building to groupOptionType
+### 0.7.4 
+- add SignalType co2
+- add SignalType consumption*Current
```

### Comparing `butler-connect-0.7.3/pyproject.toml` & `butler-connect-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "butler-connect"
-version = "0.7.3"
+version = "0.7.4"
 description = "Access libraries (with pika) and data definitions for the Buttler project."
 readme = "README.md"
 authors = [{ name = "Oliver Birkholz", email = "info@aibutler.de" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `butler-connect-0.7.3/src/butlerConnect/pikaButler.py` & `butler-connect-0.7.4/src/butlerConnect/pikaButler.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.3/src/butlerDescription/control.py` & `butler-connect-0.7.4/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.3/src/butlerDescription/group.py` & `butler-connect-0.7.4/src/butlerDescription/group.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.3/src/butlerDescription/signal.py` & `butler-connect-0.7.4/src/butlerDescription/signal.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,36 @@
         cooler = 'set_temperature_cooler'
     humidity = 'humidity'
     windowIsOpen = 'window_is_open'
     presence = 'presence'
     motion = 'motion'
     presence_merged = 'presence_merged'
     illumination = 'illumination'
+    co2 = 'co2'
     actuatorValue = 'actuator_value'
     systemState = 'system_state'
     class systemState_():
         heater = 'system_state_heater'
         cooler = 'system_state_cooler'
     consumptionGas = 'consumption_gas'
     consumptionGasRel = 'consumption_gas_rel'
+    consumptionGasCurrent = 'consumption_gas_current'
     consumptionPower = 'consumption_power'
     consumptionPowerRel = 'consumption_power_rel'
+    consumptionPowerCurrent = 'consumption_power_current'
     consumptionWater = 'consumption_water'
     consumptionWaterRel = 'consumption_water_rel'
+    consumptionWaterCurrent = 'consumption_water_current'
     consumptionHeat = 'consumption_heat'
     consumptionHeatRel = 'consumption_heat_rel'
+    consumptionHeatCurrent = 'consumption_heat_current'
     consumptionCool = 'consumption_cool'
     consumptionCoolRel = 'consumption_cool_rel'
+    consumptionCoolCurrent = 'consumption_cool_current'
+    
     
     
 
 class SignalOptionType():
     unDef = 'undef'
     forwardingMQTT = 'forwarding_mqtt'
     convertFrom    = 'convert_from'
```

### Comparing `butler-connect-0.7.3/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.7.4/src/butler_connect.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.7.3
+Version: 0.7.4
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -64,7 +64,10 @@
 ### 0.7.2
 - create SignalDirection()
 - add convertFrom to SignalOptionType
 - add different consumptionSignals to SignalType
 ### 0.7.3
 - add buildingHardware to signalOptionType and groupOptionType
 - add agent_building to groupOptionType
+### 0.7.4 
+- add SignalType co2
+- add SignalType consumption*Current
```

