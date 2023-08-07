# Comparing `tmp/django-alert-winglet-0.1.5.tar.gz` & `tmp/django-alert-winglet-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-alert-winglet-0.1.5.tar", last modified: Wed Jul 26 12:43:17 2023, max compression
+gzip compressed data, was "django-alert-winglet-0.1.6.tar", last modified: Mon Aug  7 19:39:22 2023, max compression
```

## Comparing `django-alert-winglet-0.1.5.tar` & `django-alert-winglet-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:17.710616 django-alert-winglet-0.1.5/
--rw-rw-rw-   0        0        0     1064 2023-07-26 12:38:37.000000 django-alert-winglet-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       37 2023-06-06 11:31:41.000000 django-alert-winglet-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2009 2023-07-26 12:43:17.710817 django-alert-winglet-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1143 2023-07-26 12:41:19.000000 django-alert-winglet-0.1.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:17.692280 django-alert-winglet-0.1.5/alert_winglet/
--rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.5/alert_winglet/__init__.py
--rw-rw-rw-   0        0        0      160 2023-07-26 11:36:28.000000 django-alert-winglet-0.1.5/alert_winglet/apps.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:17.693825 django-alert-winglet-0.1.5/alert_winglet/base/
--rw-rw-rw-   0        0        0        0 2023-07-21 15:58:29.000000 django-alert-winglet-0.1.5/alert_winglet/base/__init__.py
--rw-rw-rw-   0        0        0      317 2023-07-21 11:39:55.000000 django-alert-winglet-0.1.5/alert_winglet/base/manager.py
--rw-rw-rw-   0        0        0      142 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.5/alert_winglet/base/sender.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:17.695185 django-alert-winglet-0.1.5/alert_winglet/discord/
--rw-rw-rw-   0        0        0        0 2023-07-21 09:53:37.000000 django-alert-winglet-0.1.5/alert_winglet/discord/__init__.py
--rw-rw-rw-   0        0        0     4544 2023-07-26 11:37:00.000000 django-alert-winglet-0.1.5/alert_winglet/discord/manager.py
--rw-rw-rw-   0        0        0     4448 2023-07-26 11:37:00.000000 django-alert-winglet-0.1.5/alert_winglet/discord/sender.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:43:17.709733 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/
--rw-rw-rw-   0        0        0     2009 2023-07-26 12:43:17.000000 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-07-26 12:43:17.000000 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 12:43:17.000000 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-26 12:43:17.000000 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 12:43:17.000000 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2023-06-06 11:27:00.000000 django-alert-winglet-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      952 2023-07-26 12:43:17.714033 django-alert-winglet-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-06-06 11:30:18.000000 django-alert-winglet-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.879943 django-alert-winglet-0.1.6/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.879943 django-alert-winglet-0.1.6/apps/alert_winglet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/apps/alert_winglet/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/base/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/base/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/apps/alert_winglet/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/discord/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/discord/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/apps/alert_winglet/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/apps/alert_winglet/tests/test_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-07 19:39:22.000000 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-07 19:39:22.000000 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:39:22.000000 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 19:39:22.000000 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 19:39:22.000000 django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-07 19:39:22.883942 django-alert-winglet-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-07 19:39:12.000000 django-alert-winglet-0.1.6/setup.py
```

### Comparing `django-alert-winglet-0.1.5/LICENSE` & `django-alert-winglet-0.1.6/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,21 @@
-MIT License
-
-Copyright (c) 2023
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Mojtaba Davi
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `django-alert-winglet-0.1.5/PKG-INFO` & `django-alert-winglet-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,99 @@
-Metadata-Version: 2.1
-Name: django-alert-winglet
-Version: 0.1.5
-Summary: A Django app to send any exception to discord channel.
-Author: Mojtaba
-Author-email: Mojtabadavi14@gmail.com
-License: MIT License
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.1
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: Django :: 4.1
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-alert-wing
-===========
-A Django app to send any exception to a Discord channel.
-
-Quick start
------------
-
-1. Add "alert-wing" to your `INSTALLED_APPS` setting in your Django project's settings file:
-
-   .. code-block:: Django
-
-        INSTALLED_APPS = [
-            ...,
-            "alert-winglet",
-        ]
-
-
-Discord:
-    1.Set the `DISCORD_WEBHOOK_URL` variable in your Django settings. This is the URL of the Discord webhook you want to use for sending exceptions.
-
-    2.Use the `DiscordEmbedManager` class to create a Discord Embed object, and then use the `Discord` delivery method to send the exception to your Discord channel using the webhook.
-
-
-Requirements
-------------
-
-- django ~= 4.1.5
-- discord.py ~=2.2.3
-- requests ~=2.28.2
-
-License
--------
-This project is licensed under the MIT License.
-
-
-Bug Reports and Feature Requests
---------------------------------
-
-Please use the GitHub_issue_ tracker to report any bugs or submit feature requests.
-
-
-Authors
--------
-
-- Mojtaba
-- Email: Mojtabadavi14@gmail.com
-
-
-.. _GitHub_issue: https://github.com/Mojitaba34/alert-winglet/issues
+Metadata-Version: 2.1
+Name: django-alert-winglet
+Version: 0.1.6
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

### Comparing `django-alert-winglet-0.1.5/alert_winglet/discord/manager.py` & `django-alert-winglet-0.1.6/apps/alert_winglet/discord/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 import discord
 from discord import Embed
 from django.http import HttpRequest
 from django.utils import timezone
 
-from alert_winglet.base.manager import BaseManager
+from ..base.manager import BaseManager
 
 
 class DiscordEmbedManager(BaseManager):
     """
     A class for managing Discord embed messages for exception handling.
 
     Args:
```

### Comparing `django-alert-winglet-0.1.5/alert_winglet/discord/sender.py` & `django-alert-winglet-0.1.6/apps/alert_winglet/discord/sender.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from typing import Any
 
 import requests
 from django.conf import settings
 
-from alert_winglet.base.sender import BaseSender
+from ..base.sender import BaseSender
 
 
 class DiscordDelivery(BaseSender):
     """
     A class for sending messages or files to a Discord webhook.
 
     Attributes:
@@ -22,15 +22,15 @@
         file (file-like object): A file-like object to upload and send along with the message.
         embeds (list): A list of Discord embed objects to include with the message.
         allowed_mentions (dict): A dictionary specifying the allowed mentions in the message.
         webhook (str): The URL of the Discord webhook to send the message to.
 
     Raises:
         ValueError: If neither `content`, `file`, nor `embeds` are provided.
-        ValueError: If `webhook` is not provided.
+        AttributeError: If `DISCORD_WEBHOOK_URL` is not provided in settings.
 
     Methods:
         post():
             Sends the constructed message or file to the specified Discord webhook.
 
     Usage example:
         discord = Discord(
@@ -73,15 +73,15 @@
             file (file-like object): A file-like object to upload and send along with the message.
             embeds (list): A list of Discord embed objects to include with the message.
             allowed_mentions (dict): A dictionary specifying the allowed mentions in the message.
             webhook (str): The URL of the Discord webhook to send the message to.
 
         Raises:
             ValueError: If neither `content`, `file`, nor `embeds` are provided.
-            ValueError: If `webhook` is not provided.
+            AttributeError: If `DISCORD_WEBHOOK_URL` is not provided in settings.
         """
         if content is None and file is None and embeds is None:
             raise ValueError("Required one of content, file, embeds")
 
         if content is not None:
             self.DATA["content"] = content
 
@@ -98,15 +98,17 @@
             self.DATA["allowed_mentions"] = allowed_mentions
 
         self.file = file
 
         try:
             self.webhook = settings.DISCORD_WEBHOOK_URL
         except AttributeError:
-            raise ValueError("DISCORD_WEBHOOK_URL variable must set in django settings")
+            raise AttributeError(
+                "DISCORD_WEBHOOK_URL variable must set in django settings"
+            )
 
         self.DATA["tts"] = tts
 
     def send(self):
         """
         Sends the constructed message or file to the specified Discord webhook.
```

### Comparing `django-alert-winglet-0.1.5/django_alert_winglet.egg-info/PKG-INFO` & `django-alert-winglet-0.1.6/apps/django_alert_winglet.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,99 @@
-Metadata-Version: 2.1
-Name: django-alert-winglet
-Version: 0.1.5
-Summary: A Django app to send any exception to discord channel.
-Author: Mojtaba
-Author-email: Mojtabadavi14@gmail.com
-License: MIT License
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.1
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: Django :: 4.1
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-alert-wing
-===========
-A Django app to send any exception to a Discord channel.
-
-Quick start
------------
-
-1. Add "alert-wing" to your `INSTALLED_APPS` setting in your Django project's settings file:
-
-   .. code-block:: Django
-
-        INSTALLED_APPS = [
-            ...,
-            "alert-winglet",
-        ]
-
-
-Discord:
-    1.Set the `DISCORD_WEBHOOK_URL` variable in your Django settings. This is the URL of the Discord webhook you want to use for sending exceptions.
-
-    2.Use the `DiscordEmbedManager` class to create a Discord Embed object, and then use the `Discord` delivery method to send the exception to your Discord channel using the webhook.
-
-
-Requirements
-------------
-
-- django ~= 4.1.5
-- discord.py ~=2.2.3
-- requests ~=2.28.2
-
-License
--------
-This project is licensed under the MIT License.
-
-
-Bug Reports and Feature Requests
---------------------------------
-
-Please use the GitHub_issue_ tracker to report any bugs or submit feature requests.
-
-
-Authors
--------
-
-- Mojtaba
-- Email: Mojtabadavi14@gmail.com
-
-
-.. _GitHub_issue: https://github.com/Mojitaba34/alert-winglet/issues
+Metadata-Version: 2.1
+Name: django-alert-winglet
+Version: 0.1.6
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

