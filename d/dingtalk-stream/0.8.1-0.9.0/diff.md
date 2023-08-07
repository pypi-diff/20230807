# Comparing `tmp/dingtalk-stream-0.8.1.tar.gz` & `tmp/dingtalk-stream-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.8.1.tar", last modified: Fri Aug  4 02:58:28 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.9.0.tar", last modified: Mon Aug  7 09:04:46 2023, max compression
```

## Comparing `dingtalk-stream-0.8.1.tar` & `dingtalk-stream-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:58:28.029870 dingtalk-stream-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-04 02:58:28.029870 dingtalk-stream-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:58:28.025870 dingtalk-stream-0.8.1/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/card_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/card_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/card_replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    25730 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/dingtalk_stream/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:58:28.029870 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-04 02:58:27.000000 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-04 02:58:28.000000 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 02:58:27.000000 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 02:58:27.000000 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 02:58:27.000000 dingtalk-stream-0.8.1/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 02:58:28.029870 dingtalk-stream-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-04 02:58:26.000000 dingtalk-stream-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:04:46.156772 dingtalk-stream-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-07 09:04:46.156772 dingtalk-stream-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:04:46.156772 dingtalk-stream-0.9.0/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/card_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/card_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/card_replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25730 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/dingtalk_stream/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:04:46.156772 dingtalk-stream-0.9.0/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-07 09:04:46.000000 dingtalk-stream-0.9.0/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-07 09:04:46.000000 dingtalk-stream-0.9.0/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:04:46.000000 dingtalk-stream-0.9.0/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 09:04:46.000000 dingtalk-stream-0.9.0/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 09:04:46.000000 dingtalk-stream-0.9.0/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:04:46.156772 dingtalk-stream-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-07 09:04:45.000000 dingtalk-stream-0.9.0/setup.py
```

### Comparing `dingtalk-stream-0.8.1/LICENSE` & `dingtalk-stream-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.1/PKG-INFO` & `dingtalk-stream-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.8.1
+Version: 0.9.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.8.1/README.md` & `dingtalk-stream-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.1/dingtalk_stream/__init__.py` & `dingtalk-stream-0.9.0/dingtalk_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.1/dingtalk_stream/card_callback.py` & `dingtalk-stream-0.9.0/dingtalk_stream/card_callback.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.1/dingtalk_stream/card_instance.py` & `dingtalk-stream-0.9.0/dingtalk_stream/card_instance.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.1/dingtalk_stream/card_replier.py` & `dingtalk-stream-0.9.0/dingtalk_stream/card_replier.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.1/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.9.0/dingtalk_stream/chatbot.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.1/dingtalk_stream/frames.py` & `dingtalk-stream-0.9.0/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.1/dingtalk_stream/handlers.py` & `dingtalk-stream-0.9.0/dingtalk_stream/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-import logging
+import json
 
 from .frames import Headers
 from .frames import AckMessage
 from .frames import SystemMessage
 from .frames import EventMessage
 from .frames import CallbackMessage
 from .log import setup_default_logger
 
 
 class CallbackHandler(object):
+    TOPIC_CARD_CALLBACK = '/v1.0/card/instances/callback'
+
     def __init__(self):
         self.dingtalk_client = None
         self.logger = setup_default_logger('dingtalk_stream.handler')
-    
+
     def pre_start(self):
         return
 
     async def process(self, message):
         return AckMessage.STATUS_NOT_IMPLEMENT, 'not implement'
 
     async def raw_process(self, callback_message: CallbackMessage):
         code, message = await self.process(callback_message)
         ack_message = AckMessage()
         ack_message.code = code
         ack_message.headers.message_id = callback_message.headers.message_id
         ack_message.headers.content_type = Headers.CONTENT_TYPE_APPLICATION_JSON
-        ack_message.message = message
-        ack_message.data = callback_message.data
+        ack_message.data = {"response": message}
         return ack_message
 
 
 class EventHandler(object):
     def __init__(self):
         self.dingtalk_client = None
         self.logger = setup_default_logger('dingtalk_stream.handler')
```

### Comparing `dingtalk-stream-0.8.1/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.9.0/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.1/dingtalk_stream/stream.py` & `dingtalk-stream-0.9.0/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.1/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.9.0/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.8.1
+Version: 0.9.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.8.1/dingtalk_stream.egg-info/SOURCES.txt` & `dingtalk-stream-0.9.0/dingtalk_stream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.8.1/setup.py` & `dingtalk-stream-0.9.0/setup.py`

 * *Files identical despite different names*

