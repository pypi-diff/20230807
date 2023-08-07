# Comparing `tmp/Testing-alert-winglet-0.1.8.tar.gz` & `tmp/Testing-alert-winglet-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Testing-alert-winglet-0.1.8.tar", last modified: Mon Aug  7 18:00:20 2023, max compression
+gzip compressed data, was "Testing-alert-winglet-0.2.tar", last modified: Mon Aug  7 18:55:03 2023, max compression
```

## Comparing `Testing-alert-winglet-0.1.8.tar` & `Testing-alert-winglet-0.2.tar`

### file list

```diff
@@ -1,69 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.576180 Testing-alert-winglet-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-07 18:00:20.576180 Testing-alert-winglet-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.572180 Testing-alert-winglet-0.1.8/Testing_alert_winglet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-07 18:00:20.000000 Testing-alert-winglet-0.1.8/Testing_alert_winglet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-07 18:00:20.000000 Testing-alert-winglet-0.1.8/Testing_alert_winglet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:00:20.000000 Testing-alert-winglet-0.1.8/Testing_alert_winglet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 18:00:20.000000 Testing-alert-winglet-0.1.8/Testing_alert_winglet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 18:00:20.000000 Testing-alert-winglet-0.1.8/Testing_alert_winglet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.572180 Testing-alert-winglet-0.1.8/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.572180 Testing-alert-winglet-0.1.8/apps/alert_winglet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/alert_winglet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/alert_winglet/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.572180 Testing-alert-winglet-0.1.8/apps/alert_winglet/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/alert_winglet/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/alert_winglet/base/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/alert_winglet/base/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.572180 Testing-alert-winglet-0.1.8/apps/alert_winglet/discord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/alert_winglet/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/alert_winglet/discord/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/alert_winglet/discord/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.572180 Testing-alert-winglet-0.1.8/apps/alert_winglet/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/alert_winglet/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/alert_winglet/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/alert_winglet/tests/test_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.576180 Testing-alert-winglet-0.1.8/apps/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.576180 Testing-alert-winglet-0.1.8/apps/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.576180 Testing-alert-winglet-0.1.8/apps/core/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/management/commands/checkdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/management/commands/fcmup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/management/commands/renameproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/management/commands/startapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/management/commands/startapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/management/commands/startcelery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/management/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.576180 Testing-alert-winglet-0.1.8/apps/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/apps/core/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.576180 Testing-alert-winglet-0.1.8/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:00:20.576180 Testing-alert-winglet-0.1.8/config/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/settings/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/settings/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/settings/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/settings/firebase.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/settings/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/settings/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/settings/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/settings/swagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/config/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-07 18:00:20.576180 Testing-alert-winglet-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-07 18:00:12.000000 Testing-alert-winglet-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.460489 Testing-alert-winglet-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-08-07 18:55:03.460489 Testing-alert-winglet-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.452489 Testing-alert-winglet-0.2/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.456489 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-08-07 18:55:03.000000 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-07 18:55:03.000000 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:55:03.000000 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 18:55:03.000000 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:55:03.000000 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.456489 Testing-alert-winglet-0.2/apps/alert_winglet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.456489 Testing-alert-winglet-0.2/apps/alert_winglet/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/base/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/base/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.456489 Testing-alert-winglet-0.2/apps/alert_winglet/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/discord/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/discord/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.456489 Testing-alert-winglet-0.2/apps/alert_winglet/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/tests/test_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-07 18:55:03.460489 Testing-alert-winglet-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/setup.py
```

### Comparing `Testing-alert-winglet-0.1.8/LICENSE` & `Testing-alert-winglet-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.1.8/PKG-INFO` & `Testing-alert-winglet-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: Testing-alert-winglet
-Version: 0.1.8
+Version: 0.2
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
-Project-URL: Issues, https://github.com/Mojitaba34/alert-winglet/issues
-Project-URL: Source Code, https://github.com/Mojitaba34/alert-winglet
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `Testing-alert-winglet-0.1.8/README.rst` & `Testing-alert-winglet-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.1.8/Testing_alert_winglet.egg-info/PKG-INFO` & `Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: Testing-alert-winglet
-Version: 0.1.8
+Version: 0.2
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
-Project-URL: Issues, https://github.com/Mojitaba34/alert-winglet/issues
-Project-URL: Source Code, https://github.com/Mojitaba34/alert-winglet
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `Testing-alert-winglet-0.1.8/apps/alert_winglet/discord/manager.py` & `Testing-alert-winglet-0.2/apps/alert_winglet/discord/manager.py`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.1.8/apps/alert_winglet/discord/sender.py` & `Testing-alert-winglet-0.2/apps/alert_winglet/discord/sender.py`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.1.8/apps/alert_winglet/tests/test_manager.py` & `Testing-alert-winglet-0.2/apps/alert_winglet/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.1.8/apps/alert_winglet/tests/test_sender.py` & `Testing-alert-winglet-0.2/apps/alert_winglet/tests/test_sender.py`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.1.8/setup.cfg` & `Testing-alert-winglet-0.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Testing-alert-winglet
-version = 0.1.8
+version = 0.2
 description = A Django app to send any exception to discord channel.
 long_description_content_type = text/x-rst
 long_description = file: README.rst
 author = Mojtaba
 author_email = Mojtabadavi14@gmail.com
 license = MIT License
 classifiers = 
@@ -23,15 +23,14 @@
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
-packages = find:
 python_requires = ~=3.10
 install_requires = 
 	django >= 3.0
 	discord.py ~=2.2.3
 	requests ~=2.28.2
 
 [egg_info]
```

