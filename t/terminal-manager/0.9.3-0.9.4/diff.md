# Comparing `tmp/terminal_manager-0.9.3.tar.gz` & `tmp/terminal_manager-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.9.3.tar", last modified: Sat Aug  5 03:16:54 2023, max compression
+gzip compressed data, was "terminal_manager-0.9.4.tar", last modified: Mon Aug  7 07:54:28 2023, max compression
```

## Comparing `terminal_manager-0.9.3.tar` & `terminal_manager-0.9.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:16:54.637850 terminal_manager-0.9.3/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.9.3/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      725 2023-08-05 03:16:54.637850 terminal_manager-0.9.3/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.9.3/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      778 2023-08-03 04:57:50.000000 terminal_manager-0.9.3/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-08-05 03:16:54.637850 terminal_manager-0.9.3/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:16:54.629849 terminal_manager-0.9.3/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:16:54.633849 terminal_manager-0.9.3/src/terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7211 2023-08-03 04:25:16.000000 terminal_manager-0.9.3/src/terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/collection.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     6319 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/command.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:16:54.637850 terminal_manager-0.9.3/src/terminal_manager/default_collections/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/default_collections/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1147 2023-08-03 08:21:01.000000 terminal_manager-0.9.3/src/terminal_manager/default_collections/const.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4371 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/default_collections/linux.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/default_collections/windows_cmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5368 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/default_collections/windows_ps.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/errors.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/event.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-23 04:56:11.000000 terminal_manager-0.9.3/src/terminal_manager/helpers.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     8421 2023-08-04 06:41:52.000000 terminal_manager-0.9.3/src/terminal_manager/sensor.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-08-03 04:29:54.000000 terminal_manager-0.9.3/src/terminal_manager/synchronizer.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-05 03:16:54.637850 terminal_manager-0.9.3/src/terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      725 2023-08-05 03:16:54.000000 terminal_manager-0.9.3/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-08-05 03:16:54.000000 terminal_manager-0.9.3/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-08-05 03:16:54.000000 terminal_manager-0.9.3/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-08-05 03:16:54.000000 terminal_manager-0.9.3/src/terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-08-05 03:16:54.000000 terminal_manager-0.9.3/src/terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-07 07:54:28.451942 terminal_manager-0.9.4/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.9.4/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      725 2023-08-07 07:54:28.451942 terminal_manager-0.9.4/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.9.4/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      778 2023-08-07 06:57:49.000000 terminal_manager-0.9.4/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-08-07 07:54:28.451942 terminal_manager-0.9.4/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-07 07:54:28.443942 terminal_manager-0.9.4/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-07 07:54:28.447942 terminal_manager-0.9.4/src/terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     7343 2023-08-07 04:59:05.000000 terminal_manager-0.9.4/src/terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-23 04:56:11.000000 terminal_manager-0.9.4/src/terminal_manager/collection.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     6319 2023-07-23 04:56:11.000000 terminal_manager-0.9.4/src/terminal_manager/command.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-07 07:54:28.451942 terminal_manager-0.9.4/src/terminal_manager/default_collections/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-23 04:56:11.000000 terminal_manager-0.9.4/src/terminal_manager/default_collections/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-08-07 04:39:13.000000 terminal_manager-0.9.4/src/terminal_manager/default_collections/const.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4371 2023-07-23 04:56:11.000000 terminal_manager-0.9.4/src/terminal_manager/default_collections/linux.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-23 04:56:11.000000 terminal_manager-0.9.4/src/terminal_manager/default_collections/windows_cmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5368 2023-07-23 04:56:11.000000 terminal_manager-0.9.4/src/terminal_manager/default_collections/windows_ps.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-23 04:56:11.000000 terminal_manager-0.9.4/src/terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-23 04:56:11.000000 terminal_manager-0.9.4/src/terminal_manager/event.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-23 04:56:11.000000 terminal_manager-0.9.4/src/terminal_manager/helpers.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     8421 2023-08-04 06:41:52.000000 terminal_manager-0.9.4/src/terminal_manager/sensor.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-08-03 04:29:54.000000 terminal_manager-0.9.4/src/terminal_manager/synchronizer.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-07 07:54:28.447942 terminal_manager-0.9.4/src/terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      725 2023-08-07 07:54:28.000000 terminal_manager-0.9.4/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-08-07 07:54:28.000000 terminal_manager-0.9.4/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-08-07 07:54:28.000000 terminal_manager-0.9.4/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-08-07 07:54:28.000000 terminal_manager-0.9.4/src/terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-08-07 07:54:28.000000 terminal_manager-0.9.4/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.9.3/LICENSE` & `terminal_manager-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.3/PKG-INFO` & `terminal_manager-0.9.4/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: terminal_manager
-Version: 0.9.3
+Name: terminal-manager
+Version: 0.9.4
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,console,shell,bash,cmd,power shell,commands,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.9.3/pyproject.toml` & `terminal_manager-0.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.9.3"
+version = "0.9.4"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor devices"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `terminal_manager-0.9.3/src/terminal_manager/__init__.py` & `terminal_manager-0.9.4/src/terminal_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,16 +203,20 @@
             CommandError (only with `raise_errors=True`)
         """
         sensors = await self.async_poll_sensors(keys, raise_errors=raise_errors)
 
         for i, sensor in enumerate(sensors):
             if sensor.value is None:
                 continue
+            if callable(values[i]):
+                value = values[i](sensor.value)
+            else:
+                value = values[i]
             try:
-                await sensor.async_set(self, values[i])
+                await sensor.async_set(self, value)
             except (TypeError, ValueError, CommandError):
                 if raise_errors:
                     raise
 
         return await self.async_poll_sensors(keys, raise_errors=raise_errors)
 
     async def async_turn_off(self) -> CommandOutput:
```

### Comparing `terminal_manager-0.9.3/src/terminal_manager/collection.py` & `terminal_manager-0.9.4/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.3/src/terminal_manager/command.py` & `terminal_manager-0.9.4/src/terminal_manager/command.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.3/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.9.4/src/terminal_manager/default_collections/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-from enum import StrEnum
-
-
-class ActionKey(StrEnum):
+class ActionKey:
     TURN_OFF = "turn_off"
     RESTART = "restart"
 
 
-class ActionName(StrEnum):
+class ActionName:
     TURN_OFF = "Turn off"
     RESTART = "Restart"
 
 
-class SensorKey(StrEnum):
+class SensorKey:
     NETWORK_INTERFACE = "network_interface"
     MAC_ADDRESS = "mac_address"
     WAKE_ON_LAN = "wake_on_lan"
     MACHINE_TYPE = "machine_type"
     HOSTNAME = "hostname"
     OS_NAME = "os_name"
     OS_VERSION = "os_version"
@@ -24,15 +21,15 @@
     FREE_MEMORY = "free_memory"
     CPU_LOAD = "cpu_load"
     FREE_DISK_SPACE = "free_disk_space"
     TEMPERATURE = "temperature"
     PROCESSES = "processes"
 
 
-class SensorName(StrEnum):
+class SensorName:
     NETWORK_INTERFACE = "Network Interface"
     MAC_ADDRESS = "MAC Address"
     WAKE_ON_LAN = "Wake on LAN"
     MACHINE_TYPE = "Machine Type"
     HOSTNAME = "Hostname"
     OS_NAME = "OS Name"
     OS_VERSION = "OS Version"
```

### Comparing `terminal_manager-0.9.3/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.9.4/src/terminal_manager/default_collections/linux.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.3/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.9.4/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.3/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.9.4/src/terminal_manager/default_collections/windows_ps.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.3/src/terminal_manager/event.py` & `terminal_manager-0.9.4/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.3/src/terminal_manager/sensor.py` & `terminal_manager-0.9.4/src/terminal_manager/sensor.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.3/src/terminal_manager/synchronizer.py` & `terminal_manager-0.9.4/src/terminal_manager/synchronizer.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.9.3/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.9.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: terminal-manager
-Version: 0.9.3
+Name: terminal_manager
+Version: 0.9.4
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,console,shell,bash,cmd,power shell,commands,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.9.3/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.9.4/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

