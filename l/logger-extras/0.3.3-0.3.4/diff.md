# Comparing `tmp/logger_extras-0.3.3.tar.gz` & `tmp/logger_extras-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_extras-0.3.3.tar", last modified: Fri Aug  4 21:14:07 2023, max compression
+gzip compressed data, was "logger_extras-0.3.4.tar", last modified: Mon Aug  7 20:08:51 2023, max compression
```

## Comparing `logger_extras-0.3.3.tar` & `logger_extras-0.3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-04 21:13:52.000000 logger_extras-0.3.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-04 21:13:52.000000 logger_extras-0.3.3/.github/workflows/test_build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-04 21:13:52.000000 logger_extras-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-04 21:13:52.000000 logger_extras-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-04 21:13:52.000000 logger_extras-0.3.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-04 21:14:07.704247 logger_extras-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-08-04 21:13:52.000000 logger_extras-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/logger_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/logger_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-04 21:13:52.000000 logger_extras-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:14:07.704247 logger_extras-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-04 21:13:52.000000 logger_extras-0.3.3/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:08:51.684948 logger_extras-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-07 20:08:37.000000 logger_extras-0.3.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:08:51.680948 logger_extras-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:08:51.684948 logger_extras-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-07 20:08:37.000000 logger_extras-0.3.4/.github/workflows/test_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-07 20:08:37.000000 logger_extras-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-07 20:08:37.000000 logger_extras-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-07 20:08:37.000000 logger_extras-0.3.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-07 20:08:51.684948 logger_extras-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-08-07 20:08:37.000000 logger_extras-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:08:51.684948 logger_extras-0.3.4/logger_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-07 20:08:37.000000 logger_extras-0.3.4/logger_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 20:08:51.000000 logger_extras-0.3.4/logger_extras/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-07 20:08:37.000000 logger_extras-0.3.4/logger_extras/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-07 20:08:37.000000 logger_extras-0.3.4/logger_extras/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-08-07 20:08:37.000000 logger_extras-0.3.4/logger_extras/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 20:08:37.000000 logger_extras-0.3.4/logger_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-07 20:08:37.000000 logger_extras-0.3.4/logger_extras/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:08:51.684948 logger_extras-0.3.4/logger_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-07 20:08:51.000000 logger_extras-0.3.4/logger_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-07 20:08:51.000000 logger_extras-0.3.4/logger_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 20:08:51.000000 logger_extras-0.3.4/logger_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 20:08:51.000000 logger_extras-0.3.4/logger_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 20:08:51.000000 logger_extras-0.3.4/logger_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-07 20:08:37.000000 logger_extras-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 20:08:51.684948 logger_extras-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 20:08:51.684948 logger_extras-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-07 20:08:37.000000 logger_extras-0.3.4/tests/test_tools.py
```

### Comparing `logger_extras-0.3.3/.github/workflows/test_build.yml` & `logger_extras-0.3.4/.github/workflows/test_build.yml`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.3/.gitignore` & `logger_extras-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.3/LICENSE` & `logger_extras-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.3/PKG-INFO` & `logger_extras-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger_extras
-Version: 0.3.3
+Version: 0.3.4
 Summary: A collection of useful logging tools
 Author: Will Barber
 License: MIT License
         
         Copyright (c) 2023 Will Barber
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `logger_extras-0.3.3/README.md` & `logger_extras-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.3/logger_extras/filters.py` & `logger_extras-0.3.4/logger_extras/filters.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.3/logger_extras/formatters.py` & `logger_extras-0.3.4/logger_extras/formatters.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.3/logger_extras/mqtt.py` & `logger_extras-0.3.4/logger_extras/mqtt.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,18 @@
             client.publish(
                 self._connected_topic, '{"state": "connected"}', qos=1, retain=True)
 
     def __del__(self) -> None:
         if self._connected_topic:
             res = self.mqtt.publish(
                 self._connected_topic, '{"state": "disconnected"}', qos=1, retain=True)
-            res.wait_for_publish(1)
+            try:
+                res.wait_for_publish(1)
+            except (ValueError, RuntimeError):
+                pass
         self.mqtt.disconnect()
         self.mqtt.loop_stop()
 
     def emit(self, record: logging.LogRecord) -> None:
         try:
             if (
                 self.mqtt._logger  # type: ignore[attr-defined]
@@ -89,14 +92,17 @@
                 # Avoid sending log messages of the MQTT client itself
                 return
             if self._append_logger_name:
                 topic = f"{self._topic}/{record.name.replace('.', '/')}"
             else:
                 topic = self._topic
 
+            if self.mqtt.is_connected() is False:
+                self.mqtt.reconnect()
+
             msg = self.format(record)
 
             _ = self.mqtt.publish(
                 topic=topic,
                 payload=json.dumps({
                     "timestamp": record.created,
                     "message": msg,
```

### Comparing `logger_extras-0.3.3/logger_extras/utils.py` & `logger_extras-0.3.4/logger_extras/utils.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.3/logger_extras.egg-info/PKG-INFO` & `logger_extras-0.3.4/logger_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-extras
-Version: 0.3.3
+Version: 0.3.4
 Summary: A collection of useful logging tools
 Author: Will Barber
 License: MIT License
         
         Copyright (c) 2023 Will Barber
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `logger_extras-0.3.3/pyproject.toml` & `logger_extras-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.3/tests/test_tools.py` & `logger_extras-0.3.4/tests/test_tools.py`

 * *Files identical despite different names*

