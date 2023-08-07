# Comparing `tmp/Testing-alert-winglet-0.2.tar.gz` & `tmp/Testing-alert-winglet-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Testing-alert-winglet-0.2.tar", last modified: Mon Aug  7 18:55:03 2023, max compression
+gzip compressed data, was "Testing-alert-winglet-0.2.1.tar", last modified: Mon Aug  7 18:58:02 2023, max compression
```

## Comparing `Testing-alert-winglet-0.2.tar` & `Testing-alert-winglet-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.460489 Testing-alert-winglet-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-08-07 18:55:03.460489 Testing-alert-winglet-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.452489 Testing-alert-winglet-0.2/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.456489 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-08-07 18:55:03.000000 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-07 18:55:03.000000 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:55:03.000000 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 18:55:03.000000 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:55:03.000000 Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.456489 Testing-alert-winglet-0.2/apps/alert_winglet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.456489 Testing-alert-winglet-0.2/apps/alert_winglet/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/base/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/base/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.456489 Testing-alert-winglet-0.2/apps/alert_winglet/discord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/discord/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/discord/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:55:03.456489 Testing-alert-winglet-0.2/apps/alert_winglet/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/apps/alert_winglet/tests/test_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-07 18:55:03.460489 Testing-alert-winglet-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 18:54:54.000000 Testing-alert-winglet-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.415518 Testing-alert-winglet-0.2.1/
+-rw-rw-rw-   0        0        0     1090 2023-07-26 14:10:13.000000 Testing-alert-winglet-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      470 2023-08-07 18:39:30.000000 Testing-alert-winglet-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2760 2023-08-07 18:58:02.415518 Testing-alert-winglet-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1737 2023-08-07 17:00:09.000000 Testing-alert-winglet-0.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.392241 Testing-alert-winglet-0.2.1/apps/
+drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.411325 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/
+-rw-rw-rw-   0        0        0     2760 2023-08-07 18:58:02.000000 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2023-08-07 18:58:02.000000 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 18:58:02.000000 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-08-07 18:58:02.000000 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 18:58:02.000000 Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.412366 Testing-alert-winglet-0.2.1/apps/alert_winglet/
+-rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/__init__.py
+-rw-rw-rw-   0        0        0      160 2023-07-31 07:24:20.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.413406 Testing-alert-winglet-0.2.1/apps/alert_winglet/base/
+-rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/base/__init__.py
+-rw-rw-rw-   0        0        0      329 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/base/manager.py
+-rw-rw-rw-   0        0        0      142 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/base/sender.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.414479 Testing-alert-winglet-0.2.1/apps/alert_winglet/discord/
+-rw-rw-rw-   0        0        0        0 2023-07-26 14:11:02.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/discord/__init__.py
+-rw-rw-rw-   0        0        0     4650 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/discord/manager.py
+-rw-rw-rw-   0        0        0     4653 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/discord/sender.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:58:02.415518 Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/
+-rw-rw-rw-   0        0        0        0 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/test_manager.py
+-rw-rw-rw-   0        0        0     2051 2023-08-07 13:40:43.000000 Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/test_sender.py
+-rw-rw-rw-   0        0        0       94 2023-08-07 18:33:44.000000 Testing-alert-winglet-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1045 2023-08-07 18:58:02.415518 Testing-alert-winglet-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-08-07 18:53:56.000000 Testing-alert-winglet-0.2.1/setup.py
```

### Comparing `Testing-alert-winglet-0.2/PKG-INFO` & `Testing-alert-winglet-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-Metadata-Version: 2.1
-Name: Testing-alert-winglet
-Version: 0.2
-Summary: A Django app to send any exception to discord channel.
-Author: Mojtaba
-Author-email: Mojtabadavi14@gmail.com
-License: MIT License
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
+Version: 0.2.1
+Summary: A Django app to send any exception to discord channel.
+Author: Mojtaba
+Author-email: Mojtabadavi14@gmail.com
+License: MIT License
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

### Comparing `Testing-alert-winglet-0.2/README.rst` & `Testing-alert-winglet-0.2.1/README.rst`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,70 @@
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

### Comparing `Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/PKG-INFO` & `Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-Metadata-Version: 2.1
-Name: Testing-alert-winglet
-Version: 0.2
-Summary: A Django app to send any exception to discord channel.
-Author: Mojtaba
-Author-email: Mojtabadavi14@gmail.com
-License: MIT License
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
+Version: 0.2.1
+Summary: A Django app to send any exception to discord channel.
+Author: Mojtaba
+Author-email: Mojtabadavi14@gmail.com
+License: MIT License
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

### Comparing `Testing-alert-winglet-0.2/apps/Testing_alert_winglet.egg-info/SOURCES.txt` & `Testing-alert-winglet-0.2.1/apps/Testing_alert_winglet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Testing-alert-winglet-0.2/apps/alert_winglet/discord/sender.py` & `Testing-alert-winglet-0.2.1/apps/alert_winglet/discord/sender.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import json
-from typing import Any
-
-import requests
-from django.conf import settings
-
-from ..base.sender import BaseSender
-
-
-class DiscordDelivery(BaseSender):
-    """
-    A class for sending messages or files to a Discord webhook.
-
-    Attributes:
-        DATA (dict): A class-level dictionary to store the message data.
-
-    Args:
-        content (str): The text content of the message. If `None`, either `file` or `embeds` must be provided.
-        username (str): The username to display for the message sender.
-        avatar_url (str): The URL of the avatar image to display for the message sender.
-        tts (bool): Specifies if the message should be sent as a text-to-speech message.
-        file (file-like object): A file-like object to upload and send along with the message.
-        embeds (list): A list of Discord embed objects to include with the message.
-        allowed_mentions (dict): A dictionary specifying the allowed mentions in the message.
-        webhook (str): The URL of the Discord webhook to send the message to.
-
-    Raises:
-        ValueError: If neither `content`, `file`, nor `embeds` are provided.
-        AttributeError: If `DISCORD_WEBHOOK_URL` is not provided in settings.
-
-    Methods:
-        post():
-            Sends the constructed message or file to the specified Discord webhook.
-
-    Usage example:
-        discord = Discord(
-            content="Hello, everyone!",
-            username="MyBot",
-            avatar_url="https://example.com/avatar.png",
-            tts=False,
-            file=open("example.txt", "rb"),
-            embeds=[{
-                "title": "Example Embed",
-                "description": "This is an example embed."
-            }],
-            allowed_mentions={"users": [1234567890]},
-            webhook="https://discord.com/api/webhooks/1234567890/abcdefgh"
-        )
-        response = discord.post()
-        print(response.status_code)
-    """
-
-    DATA = {}
-
-    def __init__(
-        self,
-        content: str = None,
-        username: str = None,
-        avatar_url: str = None,
-        tts: bool = False,
-        file: Any = None,
-        embeds: list = None,
-        allowed_mentions=None,
-    ):
-        """
-        Initializes a new Discord message or file.
-
-        Args:
-            content (str): The text content of the message. If `None`, either `file` or `embeds` must be provided.
-            username (str): The username to display for the message sender.
-            avatar_url (str): The URL of the avatar image to display for the message sender.
-            tts (bool): Specifies if the message should be sent as a text-to-speech message.
-            file (file-like object): A file-like object to upload and send along with the message.
-            embeds (list): A list of Discord embed objects to include with the message.
-            allowed_mentions (dict): A dictionary specifying the allowed mentions in the message.
-            webhook (str): The URL of the Discord webhook to send the message to.
-
-        Raises:
-            ValueError: If neither `content`, `file`, nor `embeds` are provided.
-            AttributeError: If `DISCORD_WEBHOOK_URL` is not provided in settings.
-        """
-        if content is None and file is None and embeds is None:
-            raise ValueError("Required one of content, file, embeds")
-
-        if content is not None:
-            self.DATA["content"] = content
-
-        if username is not None:
-            self.DATA["username"] = username
-
-        if avatar_url is not None:
-            self.DATA["avatar_url"] = avatar_url
-
-        if embeds is not None:
-            self.DATA["embeds"] = embeds
-
-        if allowed_mentions is not None:
-            self.DATA["allowed_mentions"] = allowed_mentions
-
-        self.file = file
-
-        try:
-            self.webhook = settings.DISCORD_WEBHOOK_URL
-        except AttributeError:
-            raise AttributeError(
-                "DISCORD_WEBHOOK_URL variable must set in django settings"
-            )
-
-        self.DATA["tts"] = tts
-
-    def send(self):
-        """
-        Sends the constructed message or file to the specified Discord webhook.
-
-        Returns:
-            The response
-        """
-        if self.file is not None:
-            return requests.post(
-                self.webhook, {"payload_json": json.dumps(self.DATA)}, files=self.file
-            )
-
-        return requests.post(
-            self.webhook,
-            json.dumps(self.DATA),
-            headers={"Content-Type": "application/json"},
-        )
+import json
+from typing import Any
+
+import requests
+from django.conf import settings
+
+from ..base.sender import BaseSender
+
+
+class DiscordDelivery(BaseSender):
+    """
+    A class for sending messages or files to a Discord webhook.
+
+    Attributes:
+        DATA (dict): A class-level dictionary to store the message data.
+
+    Args:
+        content (str): The text content of the message. If `None`, either `file` or `embeds` must be provided.
+        username (str): The username to display for the message sender.
+        avatar_url (str): The URL of the avatar image to display for the message sender.
+        tts (bool): Specifies if the message should be sent as a text-to-speech message.
+        file (file-like object): A file-like object to upload and send along with the message.
+        embeds (list): A list of Discord embed objects to include with the message.
+        allowed_mentions (dict): A dictionary specifying the allowed mentions in the message.
+        webhook (str): The URL of the Discord webhook to send the message to.
+
+    Raises:
+        ValueError: If neither `content`, `file`, nor `embeds` are provided.
+        AttributeError: If `DISCORD_WEBHOOK_URL` is not provided in settings.
+
+    Methods:
+        post():
+            Sends the constructed message or file to the specified Discord webhook.
+
+    Usage example:
+        discord = Discord(
+            content="Hello, everyone!",
+            username="MyBot",
+            avatar_url="https://example.com/avatar.png",
+            tts=False,
+            file=open("example.txt", "rb"),
+            embeds=[{
+                "title": "Example Embed",
+                "description": "This is an example embed."
+            }],
+            allowed_mentions={"users": [1234567890]},
+            webhook="https://discord.com/api/webhooks/1234567890/abcdefgh"
+        )
+        response = discord.post()
+        print(response.status_code)
+    """
+
+    DATA = {}
+
+    def __init__(
+        self,
+        content: str = None,
+        username: str = None,
+        avatar_url: str = None,
+        tts: bool = False,
+        file: Any = None,
+        embeds: list = None,
+        allowed_mentions=None,
+    ):
+        """
+        Initializes a new Discord message or file.
+
+        Args:
+            content (str): The text content of the message. If `None`, either `file` or `embeds` must be provided.
+            username (str): The username to display for the message sender.
+            avatar_url (str): The URL of the avatar image to display for the message sender.
+            tts (bool): Specifies if the message should be sent as a text-to-speech message.
+            file (file-like object): A file-like object to upload and send along with the message.
+            embeds (list): A list of Discord embed objects to include with the message.
+            allowed_mentions (dict): A dictionary specifying the allowed mentions in the message.
+            webhook (str): The URL of the Discord webhook to send the message to.
+
+        Raises:
+            ValueError: If neither `content`, `file`, nor `embeds` are provided.
+            AttributeError: If `DISCORD_WEBHOOK_URL` is not provided in settings.
+        """
+        if content is None and file is None and embeds is None:
+            raise ValueError("Required one of content, file, embeds")
+
+        if content is not None:
+            self.DATA["content"] = content
+
+        if username is not None:
+            self.DATA["username"] = username
+
+        if avatar_url is not None:
+            self.DATA["avatar_url"] = avatar_url
+
+        if embeds is not None:
+            self.DATA["embeds"] = embeds
+
+        if allowed_mentions is not None:
+            self.DATA["allowed_mentions"] = allowed_mentions
+
+        self.file = file
+
+        try:
+            self.webhook = settings.DISCORD_WEBHOOK_URL
+        except AttributeError:
+            raise AttributeError(
+                "DISCORD_WEBHOOK_URL variable must set in django settings"
+            )
+
+        self.DATA["tts"] = tts
+
+    def send(self):
+        """
+        Sends the constructed message or file to the specified Discord webhook.
+
+        Returns:
+            The response
+        """
+        if self.file is not None:
+            return requests.post(
+                self.webhook, {"payload_json": json.dumps(self.DATA)}, files=self.file
+            )
+
+        return requests.post(
+            self.webhook,
+            json.dumps(self.DATA),
+            headers={"Content-Type": "application/json"},
+        )
```

### Comparing `Testing-alert-winglet-0.2/apps/alert_winglet/tests/test_manager.py` & `Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/test_manager.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from unittest import TestCase
-
-from discord import Embed
-from django.http import HttpRequest
-
-from ..discord.manager import DiscordEmbedManager
-import discord
-
-
-class DiscordEmbedManagerTest(TestCase):
-    def create_test_request(self):
-        request = HttpRequest()
-        request.method = "GET"
-        request.META["SERVER_NAME"] = "localhost"
-        request.META["SERVER_PORT"] = "8000"
-        return request
-
-    def test_init(self):
-        exc = Exception("Test exception for DiscordEmbedManager init")
-        request = self.create_test_request()
-        exc_id = "123456789-321654987"
-        title = "Test title for init"
-        description = "Test discription for init "
-        embed_color = discord.Color.red()
-        embed = Embed(
-            title="Embed Test title",
-            description="Embed Test description",
-            colour=discord.Color.red(),
-        )
-        discord_manager = DiscordEmbedManager(
-            exc, request, exc_id, title, description, embed_color, embed
-        )
-
-        self.assertEqual(discord_manager.exc, exc)
-        self.assertEqual(request, request)
-        self.assertEqual(exc_id, exc_id)
-        self.assertTrue(title, title)
-        self.assertEqual(description, description)
-        self.assertEqual(embed_color, embed_color)
-        self.assertEqual(embed, embed)
-
-    def test_discord_manager_without_request(self):
-        discord_manager = DiscordEmbedManager(Exception("This is a test Exception"))
-        formatted_exc, extra_detail = discord_manager.format_exception()
-        self.assertEqual(extra_detail, None)
-        self.assertIsInstance(formatted_exc, str)
-
-    def test_discord_manager_with_request(self):
-        discord_manager = DiscordEmbedManager(
-            Exception("This is a test Exception"), request=self.create_test_request()
-        )
-        formatted_exc, extra_detail = discord_manager.format_exception()
-        self.assertNotEquals(extra_detail, None)
-        self.assertIsInstance(formatted_exc, str)
-
-    def test_embed_data_instance(self):
-        discord_manager = DiscordEmbedManager(Exception("This is a test Exception"))
-        formatted_exc, extra_detail = discord_manager.format_exception()
-        data = discord_manager.prepare_embed_data(formatted_exc, extra_detail)
-        self.assertIsInstance(data, dict)
-
-    def test_embed_data_keys(self):
-        discord_manager = DiscordEmbedManager(Exception("This is a test Exception"))
-        formatted_exc, extra_detail = discord_manager.format_exception()
-        data = discord_manager.prepare_embed_data(formatted_exc, extra_detail)
-
-        data_keys = data.keys()
-        self.assertIn("color", data_keys)
-        self.assertIn("fields", data_keys)
-        self.assertIn("footer", data_keys)
-        self.assertIn("type", data_keys)
+from unittest import TestCase
+
+from discord import Embed
+from django.http import HttpRequest
+
+from ..discord.manager import DiscordEmbedManager
+import discord
+
+
+class DiscordEmbedManagerTest(TestCase):
+    def create_test_request(self):
+        request = HttpRequest()
+        request.method = "GET"
+        request.META["SERVER_NAME"] = "localhost"
+        request.META["SERVER_PORT"] = "8000"
+        return request
+
+    def test_init(self):
+        exc = Exception("Test exception for DiscordEmbedManager init")
+        request = self.create_test_request()
+        exc_id = "123456789-321654987"
+        title = "Test title for init"
+        description = "Test discription for init "
+        embed_color = discord.Color.red()
+        embed = Embed(
+            title="Embed Test title",
+            description="Embed Test description",
+            colour=discord.Color.red(),
+        )
+        discord_manager = DiscordEmbedManager(
+            exc, request, exc_id, title, description, embed_color, embed
+        )
+
+        self.assertEqual(discord_manager.exc, exc)
+        self.assertEqual(request, request)
+        self.assertEqual(exc_id, exc_id)
+        self.assertTrue(title, title)
+        self.assertEqual(description, description)
+        self.assertEqual(embed_color, embed_color)
+        self.assertEqual(embed, embed)
+
+    def test_discord_manager_without_request(self):
+        discord_manager = DiscordEmbedManager(Exception("This is a test Exception"))
+        formatted_exc, extra_detail = discord_manager.format_exception()
+        self.assertEqual(extra_detail, None)
+        self.assertIsInstance(formatted_exc, str)
+
+    def test_discord_manager_with_request(self):
+        discord_manager = DiscordEmbedManager(
+            Exception("This is a test Exception"), request=self.create_test_request()
+        )
+        formatted_exc, extra_detail = discord_manager.format_exception()
+        self.assertNotEquals(extra_detail, None)
+        self.assertIsInstance(formatted_exc, str)
+
+    def test_embed_data_instance(self):
+        discord_manager = DiscordEmbedManager(Exception("This is a test Exception"))
+        formatted_exc, extra_detail = discord_manager.format_exception()
+        data = discord_manager.prepare_embed_data(formatted_exc, extra_detail)
+        self.assertIsInstance(data, dict)
+
+    def test_embed_data_keys(self):
+        discord_manager = DiscordEmbedManager(Exception("This is a test Exception"))
+        formatted_exc, extra_detail = discord_manager.format_exception()
+        data = discord_manager.prepare_embed_data(formatted_exc, extra_detail)
+
+        data_keys = data.keys()
+        self.assertIn("color", data_keys)
+        self.assertIn("fields", data_keys)
+        self.assertIn("footer", data_keys)
+        self.assertIn("type", data_keys)
```

### Comparing `Testing-alert-winglet-0.2/apps/alert_winglet/tests/test_sender.py` & `Testing-alert-winglet-0.2.1/apps/alert_winglet/tests/test_sender.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import unittest
-
-from django.test import override_settings
-from ..discord.manager import DiscordEmbedManager
-from ..discord.sender import DiscordDelivery
-from config import settings
-
-
-class DiscordDeliveryTest(unittest.TestCase):
-    @override_settings(DISCORD_WEBHOOK_URL="https://your.temporary.webhook.url")
-    def test_init(self):
-
-        content = "Test message"
-        username = "TestUser"
-        avatar_url = "http://example.com/avatar.png"
-        tts = True
-        embeds = [{"title": "Test Embed", "description": "This is a test embed"}]
-
-        delivery = DiscordDelivery(
-            content=content,
-            username=username,
-            avatar_url=avatar_url,
-            tts=tts,
-            embeds=embeds,
-        )
-
-        self.assertEqual(delivery.DATA["content"], content)
-        self.assertEqual(delivery.DATA["username"], username)
-        self.assertEqual(delivery.DATA["avatar_url"], avatar_url)
-        self.assertTrue(delivery.DATA["tts"])
-        self.assertEqual(delivery.DATA["embeds"], embeds)
-
-    def test_send(self):
-        try:
-            raise Exception("This is a test Exception for discord delivery")
-        except Exception as exc:
-            discord_manager = DiscordEmbedManager(
-                exc,
-            )
-        formatted_exc, extra_detail = discord_manager.format_exception()
-        data = discord_manager.prepare_embed_data(formatted_exc, extra_detail)
-        if hasattr(settings, "DISCORD_WEBHOOK_URL"):
-            delivery = DiscordDelivery(
-                embeds=[
-                    data,
-                ]
-            )
-            response = delivery.send()
-            self.assertEquals(response.status_code, 204)
-
-    def test_send_without_content_file_embeds(self):
-        self.assertRaises(ValueError, DiscordDelivery)
-
-    def test_send_without_webhook_url(self):
-        if not hasattr(settings, "DISCORD_WEBHOOK_URL"):
-            self.assertRaises(AttributeError, DiscordDelivery, content="Test message")
+import unittest
+
+from django.test import override_settings
+from ..discord.manager import DiscordEmbedManager
+from ..discord.sender import DiscordDelivery
+from config import settings
+
+
+class DiscordDeliveryTest(unittest.TestCase):
+    @override_settings(DISCORD_WEBHOOK_URL="https://your.temporary.webhook.url")
+    def test_init(self):
+
+        content = "Test message"
+        username = "TestUser"
+        avatar_url = "http://example.com/avatar.png"
+        tts = True
+        embeds = [{"title": "Test Embed", "description": "This is a test embed"}]
+
+        delivery = DiscordDelivery(
+            content=content,
+            username=username,
+            avatar_url=avatar_url,
+            tts=tts,
+            embeds=embeds,
+        )
+
+        self.assertEqual(delivery.DATA["content"], content)
+        self.assertEqual(delivery.DATA["username"], username)
+        self.assertEqual(delivery.DATA["avatar_url"], avatar_url)
+        self.assertTrue(delivery.DATA["tts"])
+        self.assertEqual(delivery.DATA["embeds"], embeds)
+
+    def test_send(self):
+        try:
+            raise Exception("This is a test Exception for discord delivery")
+        except Exception as exc:
+            discord_manager = DiscordEmbedManager(
+                exc,
+            )
+        formatted_exc, extra_detail = discord_manager.format_exception()
+        data = discord_manager.prepare_embed_data(formatted_exc, extra_detail)
+        if hasattr(settings, "DISCORD_WEBHOOK_URL"):
+            delivery = DiscordDelivery(
+                embeds=[
+                    data,
+                ]
+            )
+            response = delivery.send()
+            self.assertEquals(response.status_code, 204)
+
+    def test_send_without_content_file_embeds(self):
+        self.assertRaises(ValueError, DiscordDelivery)
+
+    def test_send_without_webhook_url(self):
+        if not hasattr(settings, "DISCORD_WEBHOOK_URL"):
+            self.assertRaises(AttributeError, DiscordDelivery, content="Test message")
```

### Comparing `Testing-alert-winglet-0.2/setup.cfg` & `Testing-alert-winglet-0.2.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,66 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 5465 7374 696e 672d 616c 6572 742d  = Testing-alert-
-00000020: 7769 6e67 6c65 740a 7665 7273 696f 6e20  winglet.version 
-00000030: 3d20 302e 320a 6465 7363 7269 7074 696f  = 0.2.descriptio
-00000040: 6e20 3d20 4120 446a 616e 676f 2061 7070  n = A Django app
-00000050: 2074 6f20 7365 6e64 2061 6e79 2065 7863   to send any exc
-00000060: 6570 7469 6f6e 2074 6f20 6469 7363 6f72  eption to discor
-00000070: 6420 6368 616e 6e65 6c2e 0a6c 6f6e 675f  d channel..long_
-00000080: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-00000090: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-000000a0: 782d 7273 740a 6c6f 6e67 5f64 6573 6372  x-rst.long_descr
-000000b0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
-000000c0: 4541 444d 452e 7273 740a 6175 7468 6f72  EADME.rst.author
-000000d0: 203d 204d 6f6a 7461 6261 0a61 7574 686f   = Mojtaba.autho
-000000e0: 725f 656d 6169 6c20 3d20 4d6f 6a74 6162  r_email = Mojtab
-000000f0: 6164 6176 6931 3440 676d 6169 6c2e 636f  adavi14@gmail.co
-00000100: 6d0a 6c69 6365 6e73 6520 3d20 4d49 5420  m.license = MIT 
-00000110: 4c69 6365 6e73 650a 636c 6173 7369 6669  License.classifi
-00000120: 6572 7320 3d20 0a09 456e 7669 726f 6e6d  ers = ..Environm
-00000130: 656e 7420 3a3a 2057 6562 2045 6e76 6972  ent :: Web Envir
-00000140: 6f6e 6d65 6e74 0a09 496e 7465 6e64 6564  onment..Intended
-00000150: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
-00000160: 656c 6f70 6572 730a 094c 6963 656e 7365  elopers..License
-00000170: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000180: 203a 3a20 4d49 5420 4c69 6365 6e73 650a   :: MIT License.
-00000190: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-000001a0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000001b0: 656e 740a 0950 726f 6772 616d 6d69 6e67  ent..Programming
-000001c0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000001d0: 686f 6e20 3a3a 2033 203a 3a20 4f6e 6c79  hon :: 3 :: Only
-000001e0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000001f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000200: 203a 3a20 332e 3130 0a09 5072 6f67 7261   :: 3.10..Progra
-00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000220: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
-00000230: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
-00000240: 6a61 6e67 6f0a 0946 7261 6d65 776f 726b  jango..Framework
-00000250: 203a 3a20 446a 616e 676f 203a 3a20 330a   :: Django :: 3.
-00000260: 0946 7261 6d65 776f 726b 203a 3a20 446a  .Framework :: Dj
-00000270: 616e 676f 203a 3a20 332e 300a 0946 7261  ango :: 3.0..Fra
-00000280: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
-00000290: 203a 3a20 332e 320a 0946 7261 6d65 776f   :: 3.2..Framewo
-000002a0: 726b 203a 3a20 446a 616e 676f 203a 3a20  rk :: Django :: 
-000002b0: 340a 0946 7261 6d65 776f 726b 203a 3a20  4..Framework :: 
-000002c0: 446a 616e 676f 203a 3a20 342e 300a 0946  Django :: 4.0..F
-000002d0: 7261 6d65 776f 726b 203a 3a20 446a 616e  ramework :: Djan
-000002e0: 676f 203a 3a20 342e 310a 0954 6f70 6963  go :: 4.1..Topic
-000002f0: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
-00000300: 5757 572f 4854 5450 0a09 546f 7069 6320  WWW/HTTP..Topic 
-00000310: 3a3a 2049 6e74 6572 6e65 7420 3a3a 2057  :: Internet :: W
-00000320: 5757 2f48 5454 5020 3a3a 2044 796e 616d  WW/HTTP :: Dynam
-00000330: 6963 2043 6f6e 7465 6e74 0a0a 5b6f 7074  ic Content..[opt
-00000340: 696f 6e73 5d0a 696e 636c 7564 655f 7061  ions].include_pa
-00000350: 636b 6167 655f 6461 7461 203d 2074 7275  ckage_data = tru
-00000360: 650a 7079 7468 6f6e 5f72 6571 7569 7265  e.python_require
-00000370: 7320 3d20 7e3d 332e 3130 0a69 6e73 7461  s = ~=3.10.insta
-00000380: 6c6c 5f72 6571 7569 7265 7320 3d20 0a09  ll_requires = ..
-00000390: 646a 616e 676f 203e 3d20 332e 300a 0964  django >= 3.0..d
-000003a0: 6973 636f 7264 2e70 7920 7e3d 322e 322e  iscord.py ~=2.2.
-000003b0: 330a 0972 6571 7565 7374 7320 7e3d 322e  3..requests ~=2.
-000003c0: 3238 2e32 0a0a 5b65 6767 5f69 6e66 6f5d  28.2..[egg_info]
-000003d0: 0a74 6167 5f62 7569 6c64 203d 200a 7461  .tag_build = .ta
-000003e0: 675f 6461 7465 203d 2030 0a0a            g_date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2054 6573 7469 6e67 2d61 6c65 7274   = Testing-alert
+00000020: 2d77 696e 676c 6574 0d0a 7665 7273 696f  -winglet..versio
+00000030: 6e20 3d20 302e 322e 310d 0a64 6573 6372  n = 0.2.1..descr
+00000040: 6970 7469 6f6e 203d 2041 2044 6a61 6e67  iption = A Djang
+00000050: 6f20 6170 7020 746f 2073 656e 6420 616e  o app to send an
+00000060: 7920 6578 6365 7074 696f 6e20 746f 2064  y exception to d
+00000070: 6973 636f 7264 2063 6861 6e6e 656c 2e0d  iscord channel..
+00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+00000090: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
+000000a0: 2074 6578 742f 782d 7273 740d 0a6c 6f6e   text/x-rst..lon
+000000b0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
+000000c0: 6669 6c65 3a20 5245 4144 4d45 2e72 7374  file: README.rst
+000000d0: 0d0a 6175 7468 6f72 203d 204d 6f6a 7461  ..author = Mojta
+000000e0: 6261 0d0a 6175 7468 6f72 5f65 6d61 696c  ba..author_email
+000000f0: 203d 204d 6f6a 7461 6261 6461 7669 3134   = Mojtabadavi14
+00000100: 4067 6d61 696c 2e63 6f6d 0d0a 6c69 6365  @gmail.com..lice
+00000110: 6e73 6520 3d20 4d49 5420 4c69 6365 6e73  nse = MIT Licens
+00000120: 650d 0a63 6c61 7373 6966 6965 7273 203d  e..classifiers =
+00000130: 200d 0a09 456e 7669 726f 6e6d 656e 7420   ...Environment 
+00000140: 3a3a 2057 6562 2045 6e76 6972 6f6e 6d65  :: Web Environme
+00000150: 6e74 0d0a 0949 6e74 656e 6465 6420 4175  nt...Intended Au
+00000160: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
+00000170: 7065 7273 0d0a 094c 6963 656e 7365 203a  pers...License :
+00000180: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000190: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
+000001a0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000001b0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000001c0: 6e74 0d0a 0950 726f 6772 616d 6d69 6e67  nt...Programming
+000001d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001e0: 686f 6e20 3a3a 2033 203a 3a20 4f6e 6c79  hon :: 3 :: Only
+000001f0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000200: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000210: 6e20 3a3a 2033 2e31 300d 0a09 5072 6f67  n :: 3.10...Prog
+00000220: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000230: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000240: 3131 0d0a 0946 7261 6d65 776f 726b 203a  11...Framework :
+00000250: 3a20 446a 616e 676f 0d0a 0946 7261 6d65  : Django...Frame
+00000260: 776f 726b 203a 3a20 446a 616e 676f 203a  work :: Django :
+00000270: 3a20 330d 0a09 4672 616d 6577 6f72 6b20  : 3...Framework 
+00000280: 3a3a 2044 6a61 6e67 6f20 3a3a 2033 2e30  :: Django :: 3.0
+00000290: 0d0a 0946 7261 6d65 776f 726b 203a 3a20  ...Framework :: 
+000002a0: 446a 616e 676f 203a 3a20 332e 320d 0a09  Django :: 3.2...
+000002b0: 4672 616d 6577 6f72 6b20 3a3a 2044 6a61  Framework :: Dja
+000002c0: 6e67 6f20 3a3a 2034 0d0a 0946 7261 6d65  ngo :: 4...Frame
+000002d0: 776f 726b 203a 3a20 446a 616e 676f 203a  work :: Django :
+000002e0: 3a20 342e 300d 0a09 4672 616d 6577 6f72  : 4.0...Framewor
+000002f0: 6b20 3a3a 2044 6a61 6e67 6f20 3a3a 2034  k :: Django :: 4
+00000300: 2e31 0d0a 0954 6f70 6963 203a 3a20 496e  .1...Topic :: In
+00000310: 7465 726e 6574 203a 3a20 5757 572f 4854  ternet :: WWW/HT
+00000320: 5450 0d0a 0954 6f70 6963 203a 3a20 496e  TP...Topic :: In
+00000330: 7465 726e 6574 203a 3a20 5757 572f 4854  ternet :: WWW/HT
+00000340: 5450 203a 3a20 4479 6e61 6d69 6320 436f  TP :: Dynamic Co
+00000350: 6e74 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ntent....[option
+00000360: 735d 0d0a 696e 636c 7564 655f 7061 636b  s]..include_pack
+00000370: 6167 655f 6461 7461 203d 2074 7275 650d  age_data = true.
+00000380: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+00000390: 203d 207e 3d33 2e31 300d 0a69 6e73 7461   = ~=3.10..insta
+000003a0: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
+000003b0: 0964 6a61 6e67 6f20 3e3d 2033 2e30 0d0a  .django >= 3.0..
+000003c0: 0964 6973 636f 7264 2e70 7920 7e3d 322e  .discord.py ~=2.
+000003d0: 322e 330d 0a09 7265 7175 6573 7473 207e  2.3...requests ~
+000003e0: 3d32 2e32 382e 320d 0a0d 0a5b 6567 675f  =2.28.2....[egg_
+000003f0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000400: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000410: 300d 0a0d 0a                             0....
```

