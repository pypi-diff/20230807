# Comparing `tmp/Testing-alert-winglet-0.2.3.tar.gz` & `tmp/Testing-alert-winglet-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Testing-alert-winglet-0.2.3.tar", last modified: Mon Aug  7 19:21:40 2023, max compression
+gzip compressed data, was "Testing-alert-winglet-0.2.4.tar", last modified: Mon Aug  7 19:28:40 2023, max compression
```

## Comparing `Testing-alert-winglet-0.2.3.tar` & `Testing-alert-winglet-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:21:40.593002 Testing-alert-winglet-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 19:21:30.000000 Testing-alert-winglet-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-07 19:21:40.593002 Testing-alert-winglet-0.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:21:40.593002 Testing-alert-winglet-0.2.3/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:21:40.593002 Testing-alert-winglet-0.2.3/apps/Testing_alert_winglet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 19:21:40.000000 Testing-alert-winglet-0.2.3/apps/Testing_alert_winglet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:21:40.593002 Testing-alert-winglet-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:40.859206 Testing-alert-winglet-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-07 19:28:40.859206 Testing-alert-winglet-0.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:40.855206 Testing-alert-winglet-0.2.4/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:40.859206 Testing-alert-winglet-0.2.4/apps/Testing_alert_winglet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-07 19:28:40.000000 Testing-alert-winglet-0.2.4/apps/Testing_alert_winglet.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:40.855206 Testing-alert-winglet-0.2.4/apps/alert_winglet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/apps/alert_winglet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/apps/alert_winglet/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:40.855206 Testing-alert-winglet-0.2.4/apps/alert_winglet/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/apps/alert_winglet/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/apps/alert_winglet/base/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/apps/alert_winglet/base/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:40.855206 Testing-alert-winglet-0.2.4/apps/alert_winglet/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/apps/alert_winglet/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/apps/alert_winglet/discord/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/apps/alert_winglet/discord/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:40.859206 Testing-alert-winglet-0.2.4/apps/alert_winglet/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/apps/alert_winglet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/apps/alert_winglet/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-07 19:28:31.000000 Testing-alert-winglet-0.2.4/apps/alert_winglet/tests/test_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:28:40.859206 Testing-alert-winglet-0.2.4/setup.cfg
```

### Comparing `Testing-alert-winglet-0.2.3/LICENSE` & `Testing-alert-winglet-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.2.3/PKG-INFO` & `Testing-alert-winglet-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Testing-alert-winglet
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
 Project-URL: Issues, https://github.com/Mojitaba34/alert-winglet/issues
 Project-URL: Source Code, https://github.com/Mojitaba34/alert-winglet
 Classifier: Environment :: Web Environment
```

