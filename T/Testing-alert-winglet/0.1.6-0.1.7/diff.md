# Comparing `tmp/Testing-alert-winglet-0.1.6.tar.gz` & `tmp/Testing-alert-winglet-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Testing-alert-winglet-0.1.6.tar", last modified: Mon Aug  7 17:42:06 2023, max compression
+gzip compressed data, was "Testing-alert-winglet-0.1.7.tar", last modified: Mon Aug  7 17:50:20 2023, max compression
```

## Comparing `Testing-alert-winglet-0.1.6.tar` & `Testing-alert-winglet-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:06.855018 Testing-alert-winglet-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 17:41:49.000000 Testing-alert-winglet-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-07 17:42:06.855018 Testing-alert-winglet-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-07 17:41:49.000000 Testing-alert-winglet-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:06.855018 Testing-alert-winglet-0.1.6/Testing_alert_winglet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 17:42:06.000000 Testing-alert-winglet-0.1.6/Testing_alert_winglet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-07 17:41:49.000000 Testing-alert-winglet-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-07 17:42:06.855018 Testing-alert-winglet-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-07 17:41:49.000000 Testing-alert-winglet-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.690249 Testing-alert-winglet-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-07 17:50:20.690249 Testing-alert-winglet-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.686249 Testing-alert-winglet-0.1.7/Testing_alert_winglet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-07 17:50:20.000000 Testing-alert-winglet-0.1.7/Testing_alert_winglet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-07 17:50:20.000000 Testing-alert-winglet-0.1.7/Testing_alert_winglet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:50:20.000000 Testing-alert-winglet-0.1.7/Testing_alert_winglet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 17:50:20.000000 Testing-alert-winglet-0.1.7/Testing_alert_winglet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 17:50:20.000000 Testing-alert-winglet-0.1.7/Testing_alert_winglet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.686249 Testing-alert-winglet-0.1.7/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.686249 Testing-alert-winglet-0.1.7/apps/alert_winglet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/alert_winglet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/alert_winglet/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.686249 Testing-alert-winglet-0.1.7/apps/alert_winglet/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/alert_winglet/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/alert_winglet/base/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/alert_winglet/base/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.686249 Testing-alert-winglet-0.1.7/apps/alert_winglet/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/alert_winglet/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/alert_winglet/discord/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/alert_winglet/discord/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.686249 Testing-alert-winglet-0.1.7/apps/alert_winglet/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/alert_winglet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/alert_winglet/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/alert_winglet/tests/test_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.686249 Testing-alert-winglet-0.1.7/apps/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.686249 Testing-alert-winglet-0.1.7/apps/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.686249 Testing-alert-winglet-0.1.7/apps/core/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/management/commands/checkdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/management/commands/fcmup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/management/commands/renameproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/management/commands/startapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/management/commands/startapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/management/commands/startcelery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/management/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.686249 Testing-alert-winglet-0.1.7/apps/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/apps/core/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.686249 Testing-alert-winglet-0.1.7/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:50:20.690249 Testing-alert-winglet-0.1.7/config/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/settings/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/settings/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/settings/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/settings/firebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/settings/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/settings/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/settings/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/settings/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/config/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-07 17:50:20.690249 Testing-alert-winglet-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-07 17:50:11.000000 Testing-alert-winglet-0.1.7/setup.py
```

### Comparing `Testing-alert-winglet-0.1.6/LICENSE` & `Testing-alert-winglet-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.1.6/PKG-INFO` & `Testing-alert-winglet-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Testing-alert-winglet
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
 Project-URL: Issues, https://github.com/Mojitaba34/alert-winglet/issues
 Project-URL: Source Code, https://github.com/Mojitaba34/alert-winglet
 Classifier: Environment :: Web Environment
```

### Comparing `Testing-alert-winglet-0.1.6/README.rst` & `Testing-alert-winglet-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.1.6/setup.cfg` & `Testing-alert-winglet-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Testing-alert-winglet
-version = 0.1.6
+version = 0.1.7
 description = A Django app to send any exception to discord channel.
 long_description_content_type = text/x-rst
 long_description = file: README.rst
 author = Mojtaba
 author_email = Mojtabadavi14@gmail.com
 license = MIT License
 classifiers =
```

