# Comparing `tmp/Testing-alert-winglet-0.2.2.tar.gz` & `tmp/Testing-alert-winglet-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Testing-alert-winglet-0.2.2.tar", last modified: Mon Aug  7 19:06:33 2023, max compression
+gzip compressed data, was "Testing-alert-winglet-0.2.3.tar", last modified: Mon Aug  7 19:21:40 2023, max compression
```

## Comparing `Testing-alert-winglet-0.2.2.tar` & `Testing-alert-winglet-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/
--rw-rw-rw-   0        0        0     1090 2023-07-26 14:10:13.000000 Testing-alert-winglet-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      470 2023-08-07 18:59:46.000000 Testing-alert-winglet-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2904 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1737 2023-08-07 17:00:09.000000 Testing-alert-winglet-0.2.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.295602 Testing-alert-winglet-0.2.2/apps/
-drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/
--rw-rw-rw-   0        0        0     2904 2023-08-07 19:06:33.000000 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      708 2023-08-07 19:06:33.000000 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 19:06:33.000000 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-08-07 19:06:33.000000 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 19:06:33.000000 Testing-alert-winglet-0.2.2/apps/Testing_alert_winglet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/apps/alert_winglet/
--rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/__init__.py
--rw-rw-rw-   0        0        0      160 2023-07-31 07:24:20.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/apps.py
-drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/apps/alert_winglet/base/
--rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/base/__init__.py
--rw-rw-rw-   0        0        0      329 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/base/manager.py
--rw-rw-rw-   0        0        0      142 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/base/sender.py
-drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/apps/alert_winglet/discord/
--rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/discord/__init__.py
--rw-rw-rw-   0        0        0     4650 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/discord/manager.py
--rw-rw-rw-   0        0        0     4653 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/discord/sender.py
-drwxrwxrwx   0        0        0        0 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/apps/alert_winglet/tests/
--rw-rw-rw-   0        0        0        0 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/tests/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/tests/test_manager.py
--rw-rw-rw-   0        0        0     2051 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.2/apps/alert_winglet/tests/test_sender.py
--rw-rw-rw-   0        0        0       94 2023-08-07 18:33:44.000000 Testing-alert-winglet-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0     1045 2023-08-07 19:06:33.311784 Testing-alert-winglet-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      280 2023-08-07 19:02:09.000000 Testing-alert-winglet-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:21:40.593002 Testing-alert-winglet-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 19:21:30.000000 Testing-alert-winglet-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-07 19:21:40.593002 Testing-alert-winglet-0.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:21:40.593002 Testing-alert-winglet-0.2.3/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:21:40.593002 Testing-alert-winglet-0.2.3/apps/Testing_alert_winglet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 19:21:40.000000 Testing-alert-winglet-0.2.3/apps/Testing_alert_winglet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:21:40.593002 Testing-alert-winglet-0.2.3/setup.cfg
```

### Comparing `Testing-alert-winglet-0.2.2/PKG-INFO` & `Testing-alert-winglet-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-Metadata-Version: 2.1
-Name: Testing-alert-winglet
-Version: 0.2.2
-Summary: A Django app to send any exception to discord channel.
-Author: Mojtaba
-Author-email: Mojtabadavi14@gmail.com
-License: MIT License
-Project-URL: Issues, https://github.com/Mojitaba34/alert-winglet/issues
-Project-URL: Source Code, https://github.com/Mojitaba34/alert-winglet
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-alert-winglet
-=============
-
-A Django app to send any exception to a Discord channel.
-
-Quick start
------------
-
-Installation
-------------
-
-You can install ``django-alert-winglet`` using ``pip``::
-    pip install django-alert-winglet
-
-1. Add "alert_winglet" to your `INSTALLED_APPS` setting in your Django project's settings file::
-
-    INSTALLED_APPS = [
-        ...,
-        "alert_winglet",
-    ]
-
-Discord
--------
-
-1. Set the `DISCORD_WEBHOOK_URL` variable in your Django settings. This is the URL of the Discord webhook you want to use for sending exceptions.
-
-2. Use the `DiscordEmbedManager` class to create a Discord Embed object.::
-
-    # If the request is not provided, the `extra_detail` variable will be None
-    discord_manager = DiscordEmbedManager(
-          exc,
-      )
-    formatted_exc, extra_detail = discord_manager.format_exception()
-    data = discord_manager.prepare_embed_data(formatted_exc, extra_detail)
-
-3. Then use the `DiscordDelivery` class to send the exception to your Discord channel using the webhook.
-This class can be used for other purposes as well, like sending messages or files... ::
-
-    delivery = DiscordDelivery(
-        embeds=[
-            data,
-        ]
-    )
-    delivery.send()
-
-Requirements
-------------
-
-- django >= 3.0
-- discord.py ~=2.2.3
-- requests ~=2.28.2
-
-License
--------
-
-This project is licensed under the MIT License.
-
-Bug Reports and Feature Requests
---------------------------------
-
-Please use the GitHub_issue_ tracker to report any bugs or submit feature requests.
-
-Authors
--------
-
-- Mojtaba Davi
-- Email: Mojtabadavi14@gmail.com
-
-
-.. _GitHub_issue: https://github.com/Mojitaba34/alert-winglet/issues
+Metadata-Version: 2.1
+Name: Testing-alert-winglet
+Version: 0.2.3
+Summary: A Django app to send any exception to discord channel.
+Author: Mojtaba
+Author-email: Mojtabadavi14@gmail.com
+License: MIT License
+Project-URL: Issues, https://github.com/Mojitaba34/alert-winglet/issues
+Project-URL: Source Code, https://github.com/Mojitaba34/alert-winglet
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: ~=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+alert-winglet
+=============
+
+A Django app to send any exception to a Discord channel.
+
+Quick start
+-----------
+
+Installation
+------------
+
+You can install ``django-alert-winglet`` using ``pip``::
+    pip install django-alert-winglet
+
+1. Add "alert_winglet" to your `INSTALLED_APPS` setting in your Django project's settings file::
+
+    INSTALLED_APPS = [
+        ...,
+        "alert_winglet",
+    ]
+
+Discord
+-------
+
+1. Set the `DISCORD_WEBHOOK_URL` variable in your Django settings. This is the URL of the Discord webhook you want to use for sending exceptions.
+
+2. Use the `DiscordEmbedManager` class to create a Discord Embed object.::
+
+    # If the request is not provided, the `extra_detail` variable will be None
+    discord_manager = DiscordEmbedManager(
+          exc,
+      )
+    formatted_exc, extra_detail = discord_manager.format_exception()
+    data = discord_manager.prepare_embed_data(formatted_exc, extra_detail)
+
+3. Then use the `DiscordDelivery` class to send the exception to your Discord channel using the webhook.
+This class can be used for other purposes as well, like sending messages or files... ::
+
+    delivery = DiscordDelivery(
+        embeds=[
+            data,
+        ]
+    )
+    delivery.send()
+
+Requirements
+------------
+
+- django >= 3.0
+- discord.py ~=2.2.3
+- requests ~=2.28.2
+
+License
+-------
+
+This project is licensed under the MIT License.
+
+Bug Reports and Feature Requests
+--------------------------------
+
+Please use the GitHub_issue_ tracker to report any bugs or submit feature requests.
+
+Authors
+-------
+
+- Mojtaba Davi
+- Email: Mojtabadavi14@gmail.com
+
+
+.. _GitHub_issue: https://github.com/Mojitaba34/alert-winglet/issues
```

