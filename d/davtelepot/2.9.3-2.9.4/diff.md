# Comparing `tmp/davtelepot-2.9.3.tar.gz` & `tmp/davtelepot-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davtelepot-2.9.3.tar", last modified: Tue Jul 25 16:59:11 2023, max compression
+gzip compressed data, was "davtelepot-2.9.4.tar", last modified: Mon Aug  7 18:20:06 2023, max compression
```

## Comparing `davtelepot-2.9.3.tar` & `davtelepot-2.9.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 16:59:11.787166 davtelepot-2.9.3/
--rw-r--r--   0 davte     (1000) davte     (1000)       68 2020-01-05 17:46:41.000000 davtelepot-2.9.3/LICENSE
--rw-r--r--   0 davte     (1000) davte     (1000)      153 2020-01-05 17:46:41.000000 davtelepot-2.9.3/MANIFEST.in
--rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-07-25 16:59:11.787166 davtelepot-2.9.3/PKG-INFO
--rw-r--r--   0 davte     (1000) davte     (1000)     2781 2020-01-05 17:46:41.000000 davtelepot-2.9.3/README.md
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 16:59:11.783167 davtelepot-2.9.3/davtelepot/
--rw-rw-r--   0 davte     (1000) davte     (1000)      747 2023-07-25 16:58:45.000000 davtelepot-2.9.3/davtelepot/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)      106 2023-07-25 13:31:04.000000 davtelepot-2.9.3/davtelepot/__main__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    73001 2023-07-25 16:58:45.000000 davtelepot-2.9.3/davtelepot/administration_tools.py
--rw-rw-r--   0 davte     (1000) davte     (1000)   111657 2023-07-25 13:38:59.000000 davtelepot-2.9.3/davtelepot/api.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    10956 2023-07-25 13:28:11.000000 davtelepot-2.9.3/davtelepot/api_helper.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    31329 2023-07-25 13:28:11.000000 davtelepot-2.9.3/davtelepot/authorization.py
--rw-rw-r--   0 davte     (1000) davte     (1000)   143116 2023-07-25 13:38:59.000000 davtelepot-2.9.3/davtelepot/bot.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     8393 2023-07-25 14:42:15.000000 davtelepot-2.9.3/davtelepot/cli.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 16:59:11.783167 davtelepot-2.9.3/davtelepot/data/
--rw-r--r--   0 davte     (1000) davte     (1000)        0 2020-01-05 17:46:41.000000 davtelepot-2.9.3/davtelepot/data/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     3779 2023-07-25 13:28:11.000000 davtelepot-2.9.3/davtelepot/database.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     9773 2020-12-11 08:47:41.000000 davtelepot-2.9.3/davtelepot/helper.py
--rw-r--r--   0 davte     (1000) davte     (1000)    16258 2020-01-05 17:46:41.000000 davtelepot-2.9.3/davtelepot/ietf_language_tags.csv
--rw-rw-r--   0 davte     (1000) davte     (1000)    11316 2020-12-11 08:47:41.000000 davtelepot-2.9.3/davtelepot/languages.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    48464 2023-07-25 14:26:13.000000 davtelepot-2.9.3/davtelepot/messages.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    10720 2020-12-11 08:47:41.000000 davtelepot-2.9.3/davtelepot/suggestions.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 16:59:11.783167 davtelepot-2.9.3/davtelepot/tools/
--rw-rw-r--   0 davte     (1000) davte     (1000)        0 2020-07-04 17:30:12.000000 davtelepot-2.9.3/davtelepot/tools/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     2543 2020-07-04 17:30:12.000000 davtelepot-2.9.3/davtelepot/tools/merge_files.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    24204 2020-12-11 08:47:41.000000 davtelepot-2.9.3/davtelepot/useful_tools.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    50246 2023-07-25 14:36:42.000000 davtelepot-2.9.3/davtelepot/utilities.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 16:59:11.783167 davtelepot-2.9.3/davtelepot.egg-info/
--rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-07-25 16:59:11.000000 davtelepot-2.9.3/davtelepot.egg-info/PKG-INFO
--rw-rw-r--   0 davte     (1000) davte     (1000)      795 2023-07-25 16:59:11.000000 davtelepot-2.9.3/davtelepot.egg-info/SOURCES.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)        1 2023-07-25 16:59:11.000000 davtelepot-2.9.3/davtelepot.egg-info/dependency_links.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-07-25 16:59:11.000000 davtelepot-2.9.3/davtelepot.egg-info/requires.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-07-25 16:59:11.000000 davtelepot-2.9.3/davtelepot.egg-info/top_level.txt
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 16:59:11.783167 davtelepot-2.9.3/examples/
--rw-r--r--   0 davte     (1000) davte     (1000)        0 2020-01-05 17:46:41.000000 davtelepot-2.9.3/examples/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     6760 2020-09-26 17:25:48.000000 davtelepot-2.9.3/examples/a_simple_bot.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     3937 2020-09-26 17:25:48.000000 davtelepot-2.9.3/examples/more_bots_together.py
--rw-r--r--   0 davte     (1000) davte     (1000)     3245 2020-01-05 17:46:41.000000 davtelepot-2.9.3/examples/webhook_powered_bot.py
--rw-rw-r--   0 davte     (1000) davte     (1000)       38 2023-07-25 16:59:11.787166 davtelepot-2.9.3/setup.cfg
--rw-rw-r--   0 davte     (1000) davte     (1000)     2237 2020-04-27 21:57:40.000000 davtelepot-2.9.3/setup.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-08-07 18:20:06.239095 davtelepot-2.9.4/
+-rw-r--r--   0 davte     (1000) davte     (1000)       68 2018-10-23 15:20:11.000000 davtelepot-2.9.4/LICENSE
+-rw-rw-r--   0 davte     (1000) davte     (1000)      153 2019-07-19 08:07:29.000000 davtelepot-2.9.4/MANIFEST.in
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-08-07 18:20:06.239095 davtelepot-2.9.4/PKG-INFO
+-rw-rw-r--   0 davte     (1000) davte     (1000)     2781 2019-07-18 12:44:21.000000 davtelepot-2.9.4/README.md
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-08-07 18:20:06.239095 davtelepot-2.9.4/davtelepot/
+-rw-rw-r--   0 davte     (1000) davte     (1000)      747 2023-08-07 18:19:50.000000 davtelepot-2.9.4/davtelepot/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)      106 2023-08-07 18:19:33.000000 davtelepot-2.9.4/davtelepot/__main__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    73001 2023-08-07 18:19:33.000000 davtelepot-2.9.4/davtelepot/administration_tools.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)   111720 2023-08-07 18:19:50.000000 davtelepot-2.9.4/davtelepot/api.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    10956 2023-01-06 09:30:24.000000 davtelepot-2.9.4/davtelepot/api_helper.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    31329 2022-12-06 21:18:51.000000 davtelepot-2.9.4/davtelepot/authorization.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)   143116 2023-08-07 18:19:33.000000 davtelepot-2.9.4/davtelepot/bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     8393 2023-08-07 18:19:33.000000 davtelepot-2.9.4/davtelepot/cli.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-08-07 18:20:06.239095 davtelepot-2.9.4/davtelepot/data/
+-rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-19 07:39:50.000000 davtelepot-2.9.4/davtelepot/data/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3779 2022-12-10 17:46:29.000000 davtelepot-2.9.4/davtelepot/database.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     9773 2020-11-19 14:18:50.000000 davtelepot-2.9.4/davtelepot/helper.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    16258 2019-07-18 12:44:21.000000 davtelepot-2.9.4/davtelepot/ietf_language_tags.csv
+-rw-rw-r--   0 davte     (1000) davte     (1000)    11316 2022-10-12 11:53:43.000000 davtelepot-2.9.4/davtelepot/languages.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    48464 2023-08-07 18:19:33.000000 davtelepot-2.9.4/davtelepot/messages.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    10720 2022-10-12 11:53:43.000000 davtelepot-2.9.4/davtelepot/suggestions.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-08-07 18:20:06.239095 davtelepot-2.9.4/davtelepot/tools/
+-rw-rw-r--   0 davte     (1000) davte     (1000)        0 2020-06-22 20:56:16.000000 davtelepot-2.9.4/davtelepot/tools/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     2543 2020-06-22 20:56:16.000000 davtelepot-2.9.4/davtelepot/tools/merge_files.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    24204 2022-10-12 11:53:43.000000 davtelepot-2.9.4/davtelepot/useful_tools.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    50246 2023-08-07 18:19:33.000000 davtelepot-2.9.4/davtelepot/utilities.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-08-07 18:20:06.239095 davtelepot-2.9.4/davtelepot.egg-info/
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-08-07 18:20:06.000000 davtelepot-2.9.4/davtelepot.egg-info/PKG-INFO
+-rw-rw-r--   0 davte     (1000) davte     (1000)      795 2023-08-07 18:20:06.000000 davtelepot-2.9.4/davtelepot.egg-info/SOURCES.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)        1 2023-08-07 18:20:06.000000 davtelepot-2.9.4/davtelepot.egg-info/dependency_links.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-08-07 18:20:06.000000 davtelepot-2.9.4/davtelepot.egg-info/requires.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-08-07 18:20:06.000000 davtelepot-2.9.4/davtelepot.egg-info/top_level.txt
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-08-07 18:20:06.239095 davtelepot-2.9.4/examples/
+-rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-18 12:44:21.000000 davtelepot-2.9.4/examples/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     6760 2020-08-23 12:21:45.000000 davtelepot-2.9.4/examples/a_simple_bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3937 2020-08-23 12:21:45.000000 davtelepot-2.9.4/examples/more_bots_together.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3245 2020-08-23 12:11:09.000000 davtelepot-2.9.4/examples/webhook_powered_bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)       38 2023-08-07 18:20:06.239095 davtelepot-2.9.4/setup.cfg
+-rw-rw-r--   0 davte     (1000) davte     (1000)     2237 2020-08-23 12:11:09.000000 davtelepot-2.9.4/setup.py
```

### Comparing `davtelepot-2.9.3/PKG-INFO` & `davtelepot-2.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: davtelepot
-Version: 2.9.3
+Version: 2.9.4
 Summary: Telegram bot API mirroring class, featuring dataset-powered SQLite databases.
 Home-page: https://gogs.davte.it/davte/davtelepot
 Author: Davide Testa
 Author-email: davide@davte.it
 License: GNU General Public License v3.0
 Keywords: telegram bot python asyncio async aiohttp
 Platform: any
```

### Comparing `davtelepot-2.9.3/README.md` & `davtelepot-2.9.4/README.md`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/__init__.py` & `davtelepot-2.9.4/davtelepot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ```
 """
 
 __author__ = "Davide Testa"
 __email__ = "davide@davte.it"
 __credits__ = ["Marco Origlia", "Nick Lee @Nickoala"]
 __license__ = "GNU General Public License v3.0"
-__version__ = "2.9.3"
+__version__ = "2.9.4"
 __maintainer__ = "Davide Testa"
 __contact__ = "t.me/davte"
 
 from davtelepot import (administration_tools, api, authorization,
                         bot, helper, languages, messages, suggestions,
                         useful_tools, utilities)
```

### Comparing `davtelepot-2.9.3/davtelepot/administration_tools.py` & `davtelepot-2.9.4/davtelepot/administration_tools.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/api.py` & `davtelepot-2.9.4/davtelepot/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1764,17 +1764,17 @@
                                 **kwargs):
         """Send answers to an inline query.
 
         On success, True is returned.
         No more than 50 results per query are allowed.
         See https://core.telegram.org/bots/api#answerinlinequery for details.
         """
-        if 'switch_pm_text' in kwargs:
+        if 'switch_pm_text' in kwargs and kwargs['switch_pm_text']:
             button = InlineQueryResultsButton(text=kwargs['switch_pm_text'])
-        if 'switch_pm_parameter' in kwargs:
+        if 'switch_pm_parameter' in kwargs and kwargs['switch_pm_parameter']:
             button = InlineQueryResultsButton(start_parameter=kwargs['switch_pm_parameter'])
         return await self.api_request(
             'answerInlineQuery',
             parameters=locals()
         )
 
     async def sendInvoice(self, chat_id: int, title: str, description: str,
```

### Comparing `davtelepot-2.9.3/davtelepot/api_helper.py` & `davtelepot-2.9.4/davtelepot/api_helper.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/authorization.py` & `davtelepot-2.9.4/davtelepot/authorization.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/bot.py` & `davtelepot-2.9.4/davtelepot/bot.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/cli.py` & `davtelepot-2.9.4/davtelepot/cli.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/database.py` & `davtelepot-2.9.4/davtelepot/database.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/helper.py` & `davtelepot-2.9.4/davtelepot/helper.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/ietf_language_tags.csv` & `davtelepot-2.9.4/davtelepot/ietf_language_tags.csv`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/languages.py` & `davtelepot-2.9.4/davtelepot/languages.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/messages.py` & `davtelepot-2.9.4/davtelepot/messages.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/suggestions.py` & `davtelepot-2.9.4/davtelepot/suggestions.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/tools/merge_files.py` & `davtelepot-2.9.4/davtelepot/tools/merge_files.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/useful_tools.py` & `davtelepot-2.9.4/davtelepot/useful_tools.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot/utilities.py` & `davtelepot-2.9.4/davtelepot/utilities.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/davtelepot.egg-info/PKG-INFO` & `davtelepot-2.9.4/davtelepot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: davtelepot
-Version: 2.9.3
+Version: 2.9.4
 Summary: Telegram bot API mirroring class, featuring dataset-powered SQLite databases.
 Home-page: https://gogs.davte.it/davte/davtelepot
 Author: Davide Testa
 Author-email: davide@davte.it
 License: GNU General Public License v3.0
 Keywords: telegram bot python asyncio async aiohttp
 Platform: any
```

### Comparing `davtelepot-2.9.3/davtelepot.egg-info/SOURCES.txt` & `davtelepot-2.9.4/davtelepot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/examples/a_simple_bot.py` & `davtelepot-2.9.4/examples/a_simple_bot.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/examples/more_bots_together.py` & `davtelepot-2.9.4/examples/more_bots_together.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/examples/webhook_powered_bot.py` & `davtelepot-2.9.4/examples/webhook_powered_bot.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.3/setup.py` & `davtelepot-2.9.4/setup.py`

 * *Files identical despite different names*

