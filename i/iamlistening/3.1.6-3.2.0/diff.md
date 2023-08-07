# Comparing `tmp/iamlistening-3.1.6.tar.gz` & `tmp/iamlistening-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-3.1.6.tar", max compression
+gzip compressed data, was "iamlistening-3.2.0.tar", max compression
```

## Comparing `iamlistening-3.1.6.tar` & `iamlistening-3.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-08-07 12:04:38.200574 iamlistening-3.1.6/LICENSE
--rw-r--r--   0        0        0     2457 2023-08-07 12:04:38.200574 iamlistening-3.1.6/README.md
--rw-r--r--   0        0        0       81 2023-08-07 12:04:40.080722 iamlistening-3.1.6/iamlistening/__init__.py
--rw-r--r--   0        0        0      688 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/config.py
--rw-r--r--   0        0        0     1376 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     1673 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/main.py
--rw-r--r--   0        0        0        0 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/__init__.py
--rw-r--r--   0        0        0     3276 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/chat_manager.py
--rw-r--r--   0        0        0       56 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/__init__.py
--rw-r--r--   0        0        0      876 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/discord.py
--rw-r--r--   0        0        0      738 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/guilded.py
--rw-r--r--   0        0        0      672 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/lemmy.py
--rw-r--r--   0        0        0     1349 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/mastodon.py
--rw-r--r--   0        0        0     1616 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/matrix.py
--rw-r--r--   0        0        0      912 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/revolt.py
--rw-r--r--   0        0        0      806 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/rocket_chat.py
--rw-r--r--   0        0        0     1176 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/telegram.py
--rw-r--r--   0        0        0      568 2023-08-07 12:04:38.204574 iamlistening-3.1.6/iamlistening/platform/clients/tinode.py
--rw-r--r--   0        0        0     3313 2023-08-07 12:04:40.072721 iamlistening-3.1.6/pyproject.toml
--rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 iamlistening-3.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-07 18:53:00.559901 iamlistening-3.2.0/LICENSE
+-rw-r--r--   0        0        0     2457 2023-08-07 18:53:00.563901 iamlistening-3.2.0/README.md
+-rw-r--r--   0        0        0       81 2023-08-07 18:53:03.336063 iamlistening-3.2.0/iamlistening/__init__.py
+-rw-r--r--   0        0        0      688 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/config.py
+-rw-r--r--   0        0        0     1376 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     1673 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/main.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/__init__.py
+-rw-r--r--   0        0        0     3398 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/chat_manager.py
+-rw-r--r--   0        0        0       60 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/clients/__init__.py
+-rw-r--r--   0        0        0      876 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/clients/discord.py
+-rw-r--r--   0        0        0      738 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/clients/guilded.py
+-rw-r--r--   0        0        0      867 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/clients/lemmy.py
+-rw-r--r--   0        0        0     1349 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/clients/mastodon.py
+-rw-r--r--   0        0        0     1616 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/clients/matrix.py
+-rw-r--r--   0        0        0      912 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/clients/revolt.py
+-rw-r--r--   0        0        0      806 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/clients/rocket_chat.py
+-rw-r--r--   0        0        0     1176 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/clients/telegram.py
+-rw-r--r--   0        0        0      568 2023-08-07 18:53:00.567901 iamlistening-3.2.0/iamlistening/platform/clients/tinode.py
+-rw-r--r--   0        0        0     3371 2023-08-07 18:53:03.328062 iamlistening-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3807 1970-01-01 00:00:00.000000 iamlistening-3.2.0/PKG-INFO
```

### Comparing `iamlistening-3.1.6/LICENSE` & `iamlistening-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/README.md` & `iamlistening-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/iamlistening/config.py` & `iamlistening-3.2.0/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/iamlistening/default_settings.toml` & `iamlistening-3.2.0/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/iamlistening/main.py` & `iamlistening-3.2.0/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/iamlistening/platform/chat_manager.py` & `iamlistening-3.2.0/iamlistening/platform/chat_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-
 import asyncio
 
 from loguru import logger
 
 from iamlistening.config import settings
 
 
-class ChatManager():
+class ChatManager:
     """
     Chat manager
 
     Attributes:
         platform (str): The platform to use
         bot (object): The bot
         is_connected (bool): Is the bot connected
         latest_message (str): The latest message
         iteration_limit (int): The iteration limit
         iteration_count (int): The iteration count
 
     Methods:
         start(self)
         get_handler(self)
-        
+
 
     """
+
     @staticmethod
     def get_handler(platform=None):
         """
         Get platform handler.
 
         Args:
             platform (str): The platform to use
@@ -36,46 +36,53 @@
             PlatformHandler
 
 
         """
         handler = None
         if platform == "telegram":
             from .clients.telegram import TelegramHandler
+
             handler = TelegramHandler()
         elif platform == "discord":
             from .clients.discord import DiscordHandler
+
             handler = DiscordHandler()
         if platform == "matrix":
             from .clients.matrix import MatrixHandler
+
             handler = MatrixHandler()
         elif platform == "guilded":
             from .clients.guilded import GuildedHandler
+
             handler = GuildedHandler()
         elif platform == "mastodon":
             from .clients.mastodon import MastodonHandler
+
             handler = MastodonHandler()
+        elif platform == "lemmy":
+            from .clients.lemmy import LemmyHandler
 
+            handler = LemmyHandler()
+            
         return handler
 
-    
     def __init__(self):
         """
         Initialize the chat manager.
         """
         self.platform = None
         self.bot = None
         self.is_connected = True
         self.latest_message = None
         self.lock = asyncio.Lock()
         self.iteration_limit = settings.iteration_limit or -1
         self.iteration_count = 0
 
-
     async def start(self):
-        """ 
+        """
         Start the chat manager.
         Specific to the client platform
         """
 
     def connected(self):
         """
         Asynchronously checks if the listener is connected.
@@ -100,15 +107,14 @@
             if self.latest_message:
                 msg = self.latest_message
                 self.latest_message = None
                 return msg
 
         await asyncio.sleep(0.1)
 
-
     async def handle_message(self, message_content):
         """
         Handle a new message.
 
         Args:
             message_content (str): The content of the message.
         """
@@ -126,15 +132,14 @@
             await asyncio.sleep(0.1)
             self.iteration_count += 1
         else:
             await self.disconnected()
 
         return
 
-
     async def disconnected(self):
         """
         Asynchronously disconnect the listener.
 
         Returns:
             None
         """
```

### Comparing `iamlistening-3.1.6/iamlistening/platform/clients/discord.py` & `iamlistening-3.2.0/iamlistening/platform/clients/discord.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/iamlistening/platform/clients/guilded.py` & `iamlistening-3.2.0/iamlistening/platform/clients/guilded.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/iamlistening/platform/clients/mastodon.py` & `iamlistening-3.2.0/iamlistening/platform/clients/mastodon.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/iamlistening/platform/clients/matrix.py` & `iamlistening-3.2.0/iamlistening/platform/clients/matrix.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/iamlistening/platform/clients/revolt.py` & `iamlistening-3.2.0/iamlistening/platform/clients/revolt.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/iamlistening/platform/clients/rocket_chat.py` & `iamlistening-3.2.0/iamlistening/platform/clients/rocket_chat.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/iamlistening/platform/clients/telegram.py` & `iamlistening-3.2.0/iamlistening/platform/clients/telegram.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/iamlistening/platform/clients/tinode.py` & `iamlistening-3.2.0/iamlistening/platform/clients/tinode.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.6/pyproject.toml` & `iamlistening-3.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "3.1.6"
+version = "3.2.0"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix","rocket chat",
@@ -34,15 +34,15 @@
 py-cord= "^2.4.1"
 simplematrixbotlib= "^2.9.0"
 rocketchat-API= "^1.30.0"
 "Mastodon.py" = "^1.8.1"
 "guilded.py" = "^1.9.1"
 tinode_grpc = "^0.22.3"
 "revolt.py" = "^0.1.11"
-
+pythorhead = {version ="^0.15.4", python = ">=3.10,<3.12"}
 
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^8.0.4"
 ruff = "^0.0.281"
```

### Comparing `iamlistening-3.1.6/PKG-INFO` & `iamlistening-3.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 3.1.6
+Version: 3.2.0
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix,rocket chat
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Mastodon.py (>=1.8.1,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: guilded.py (>=1.9.1,<2.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: py-cord (>=2.4.1,<3.0.0)
+Requires-Dist: pythorhead (>=0.15.4,<0.16.0) ; python_version >= "3.10" and python_version < "3.12"
 Requires-Dist: revolt.py (>=0.1.11,<0.2.0)
 Requires-Dist: rocketchat-API (>=1.30.0,<2.0.0)
 Requires-Dist: simplematrixbotlib (>=2.9.0,<3.0.0)
 Requires-Dist: telethon (>=1.28.5,<2.0.0)
 Requires-Dist: tinode_grpc (>=0.22.3,<0.23.0)
 Project-URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/iamlistening/issues
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 3.1.6 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 3.2.0 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix,rocket chat Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Mastodon.py
 (>=1.8.1,<2.0.0) Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist:
 dynaconf (>=3.1.12,<4.0.0) Requires-Dist: guilded.py (>=1.9.1,<2.0.0) Requires-
 Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: py-cord (>=2.4.1,<3.0.0) Requires-
-Dist: revolt.py (>=0.1.11,<0.2.0) Requires-Dist: rocketchat-API
-(>=1.30.0,<2.0.0) Requires-Dist: simplematrixbotlib (>=2.9.0,<3.0.0) Requires-
-Dist: telethon (>=1.28.5,<2.0.0) Requires-Dist: tinode_grpc (>=0.22.3,<0.23.0)
-Project-URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/
-CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/iamlistening/
-issues Project-URL: Support, https://github.com/mraniki/iamlistening/
-discussions Description-Content-Type: text/markdown
+Dist: pythorhead (>=0.15.4,<0.16.0) ; python_version >= "3.10" and
+python_version < "3.12" Requires-Dist: revolt.py (>=0.1.11,<0.2.0) Requires-
+Dist: rocketchat-API (>=1.30.0,<2.0.0) Requires-Dist: simplematrixbotlib
+(>=2.9.0,<3.0.0) Requires-Dist: telethon (>=1.28.5,<2.0.0) Requires-Dist:
+tinode_grpc (>=0.22.3,<0.23.0) Project-URL: Changelog, https://github.com/
+mraniki/iamlistening/blob/dev/CHANGELOG.rst Project-URL: Issues, https://
+github.com/mraniki/iamlistening/issues Project-URL: Support, https://
+github.com/mraniki/iamlistening/discussions Description-Content-Type: text/
+markdown
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
 the-badge&logo=wikipedia&logoColor=white] [https://
 img.shields.io/badge/github-%23000000.svg?style=for-the-             [Logo]
 badge&logo=github&logoColor=white]
 [https://img.shields.io/docker/pulls/mraniki/tt?style=for-
 the-badge]
 [https://img.shields.io/pypi/v/iamlistening?style=for-the-
```

