# Comparing `tmp/ovos-bus-client-0.0.6a2.tar.gz` & `tmp/ovos-bus-client-0.0.6a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-bus-client-0.0.6a2.tar", last modified: Fri Aug  4 17:40:17 2023, max compression
+gzip compressed data, was "ovos-bus-client-0.0.6a3.tar", last modified: Mon Aug  7 19:45:40 2023, max compression
```

## Comparing `ovos-bus-client-0.0.6a2.tar` & `ovos-bus-client-0.0.6a3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/ovos_bus_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/ovos_bus_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16208 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/client/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/client/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/send_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/ovos_bus_client/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:45:40.405468 ovos-bus-client-0.0.6a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-07 19:45:40.405468 ovos-bus-client-0.0.6a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:45:40.405468 ovos-bus-client-0.0.6a3/ovos_bus_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:45:40.405468 ovos-bus-client-0.0.6a3/ovos_bus_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16208 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/client/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/client/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/send_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:45:40.405468 ovos-bus-client-0.0.6a3/ovos_bus_client/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/ovos_bus_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:45:40.405468 ovos-bus-client-0.0.6a3/ovos_bus_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-07 19:45:40.000000 ovos-bus-client-0.0.6a3/ovos_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-07 19:45:40.000000 ovos-bus-client-0.0.6a3/ovos_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:45:40.000000 ovos-bus-client-0.0.6a3/ovos_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-07 19:45:40.000000 ovos-bus-client-0.0.6a3/ovos_bus_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-07 19:45:40.000000 ovos-bus-client-0.0.6a3/ovos_bus_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 19:45:40.000000 ovos-bus-client-0.0.6a3/ovos_bus_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:45:40.405468 ovos-bus-client-0.0.6a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-07 19:45:39.000000 ovos-bus-client-0.0.6a3/setup.py
```

### Comparing `ovos-bus-client-0.0.6a2/LICENSE.md` & `ovos-bus-client-0.0.6a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/PKG-INFO` & `ovos-bus-client-0.0.6a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.6a2
+Version: 0.0.6a3
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/__init__.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/client/__init__.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/client/client.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/client/client.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/client/collector.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/client/collector.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/client/waiter.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/client/waiter.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/conf.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/conf.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/message.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/message.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/scripts.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/scripts.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/send_func.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/send_func.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/session.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/session.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/util/__init__.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client/util/utils.py` & `ovos-bus-client-0.0.6a3/ovos_bus_client/util/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/PKG-INFO` & `ovos-bus-client-0.0.6a3/ovos_bus_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.6a2
+Version: 0.0.6a3
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/SOURCES.txt` & `ovos-bus-client-0.0.6a3/ovos_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a2/setup.py` & `ovos-bus-client-0.0.6a3/setup.py`

 * *Files identical despite different names*

