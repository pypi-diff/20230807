# Comparing `tmp/boticordpy-3.0.1.tar.gz` & `tmp/boticordpy-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boticordpy-3.0.1.tar", last modified: Tue Jul  4 10:06:04 2023, max compression
+gzip compressed data, was "boticordpy-3.0.2.tar", last modified: Mon Aug  7 12:07:59 2023, max compression
```

## Comparing `boticordpy-3.0.1.tar` & `boticordpy-3.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 10:06:04.381419 boticordpy-3.0.1/
--rw-rw-rw-   0        0        0     1074 2023-06-28 06:47:50.000000 boticordpy-3.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3293 2023-07-04 10:06:04.382429 boticordpy-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2585 2023-07-04 10:03:21.000000 boticordpy-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 10:06:04.369820 boticordpy-3.0.1/boticordpy/
--rw-rw-rw-   0        0        0      421 2023-07-04 10:03:21.000000 boticordpy-3.0.1/boticordpy/__init__.py
--rw-rw-rw-   0        0        0     6189 2023-06-28 06:47:50.000000 boticordpy-3.0.1/boticordpy/autopost.py
--rw-rw-rw-   0        0        0     6748 2023-07-04 10:03:21.000000 boticordpy-3.0.1/boticordpy/client.py
--rw-rw-rw-   0        0        0     3865 2023-06-28 06:47:50.000000 boticordpy-3.0.1/boticordpy/exceptions.py
--rw-rw-rw-   0        0        0     2996 2023-07-04 10:03:21.000000 boticordpy-3.0.1/boticordpy/http.py
--rw-rw-rw-   0        0        0    26747 2023-06-28 06:47:50.000000 boticordpy-3.0.1/boticordpy/types.py
--rw-rw-rw-   0        0        0     4941 2023-07-04 10:03:21.000000 boticordpy-3.0.1/boticordpy/websocket.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:06:04.380912 boticordpy-3.0.1/boticordpy.egg-info/
--rw-rw-rw-   0        0        0     3293 2023-07-04 10:06:04.000000 boticordpy-3.0.1/boticordpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-07-04 10:06:04.000000 boticordpy-3.0.1/boticordpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 10:06:04.000000 boticordpy-3.0.1/boticordpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-04 10:06:04.000000 boticordpy-3.0.1/boticordpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-04 10:06:04.000000 boticordpy-3.0.1/boticordpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-04 10:06:04.383429 boticordpy-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1990 2023-06-28 06:47:50.000000 boticordpy-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:07:59.831944 boticordpy-3.0.2/
+-rw-rw-rw-   0        0        0     1074 2023-06-28 06:47:50.000000 boticordpy-3.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3290 2023-08-07 12:07:59.832943 boticordpy-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2582 2023-08-07 12:07:15.000000 boticordpy-3.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 12:07:59.822400 boticordpy-3.0.2/boticordpy/
+-rw-rw-rw-   0        0        0      421 2023-08-07 12:07:15.000000 boticordpy-3.0.2/boticordpy/__init__.py
+-rw-rw-rw-   0        0        0     6316 2023-08-07 12:07:15.000000 boticordpy-3.0.2/boticordpy/autopost.py
+-rw-rw-rw-   0        0        0     6853 2023-08-07 12:07:15.000000 boticordpy-3.0.2/boticordpy/client.py
+-rw-rw-rw-   0        0        0     3865 2023-06-28 06:47:50.000000 boticordpy-3.0.2/boticordpy/exceptions.py
+-rw-rw-rw-   0        0        0     2996 2023-07-04 10:03:21.000000 boticordpy-3.0.2/boticordpy/http.py
+-rw-rw-rw-   0        0        0    26747 2023-06-28 06:47:50.000000 boticordpy-3.0.2/boticordpy/types.py
+-rw-rw-rw-   0        0        0     4985 2023-08-07 12:07:15.000000 boticordpy-3.0.2/boticordpy/websocket.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:07:59.830942 boticordpy-3.0.2/boticordpy.egg-info/
+-rw-rw-rw-   0        0        0     3290 2023-08-07 12:07:59.000000 boticordpy-3.0.2/boticordpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-08-07 12:07:59.000000 boticordpy-3.0.2/boticordpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 12:07:59.000000 boticordpy-3.0.2/boticordpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-08-07 12:07:59.000000 boticordpy-3.0.2/boticordpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 12:07:59.000000 boticordpy-3.0.2/boticordpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-07 12:07:59.833451 boticordpy-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1990 2023-06-28 06:47:50.000000 boticordpy-3.0.2/setup.py
```

### Comparing `boticordpy-3.0.1/LICENSE.txt` & `boticordpy-3.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `boticordpy-3.0.1/PKG-INFO` & `boticordpy-3.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boticordpy
-Version: 3.0.1
+Version: 3.0.2
 Summary: A Python wrapper for BotiCord API
 Home-page: https://github.com/boticord/boticordpy
 Author: Marakarka
 Author-email: support@kerdoku.top
 License: MIT
 Project-URL: Documentation, https://py.boticord.top/en/stable
 Project-URL: Issue tracker, https://github.com/boticord/boticordpy/issues
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <p align="center">
-<img width="520" src="https://media.discordapp.net/attachments/929108234709639208/943873379809787964/boticordpylogo.png" alt="">
+<img width="560" src="https://github.com/boticord/boticordpy/assets/61203964/87393a07-2afa-4568-a324-500d1940b4fc" alt="">
 </p>
 
 <p align="center">
   <b>
     The easiest way to use BotiCord API in Python.
     <span> · </span>
     <a href="https://py.boticord.top/">Docs</a>
@@ -71,15 +71,15 @@
 from boticordpy import BoticordClient
 
 bot = commands.Bot(command_prefix="!")
 
 
 # Function that will return the current bot's stats.
 async def get_stats():
-    return {"servers": len(bot.guilds), "shards": 0, "members": len(bot.users)}
+    return {"servers": len(bot.guilds), "shards": None, "members": len(bot.users)}
 
 
 # Function that will be called if stats are posted successfully.
 async def on_success_posting():
     print("wow stats posting works")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: boticordpy Version: 3.0.1 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: boticordpy Version: 3.0.2 Summary: A Python wrapper
 for BotiCord API Home-page: https://github.com/boticord/boticordpy Author:
 Marakarka Author-email: support@kerdoku.top License: MIT Project-URL:
 Documentation, https://py.boticord.top/en/stable Project-URL: Issue tracker,
 https://github.com/boticord/boticordpy/issues Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -19,17 +19,17 @@
 library: ``` pip install boticordpy ``` ``` python3 -m pip install boticordpy
 ``` Or just clone the repo: https://github.com/boticord/boticordpy
 ***** Examples *****
 You can find other examples in an examples folder. **Discord.py Autopost
 example** ```py from discord.ext import commands from boticordpy import
 BoticordClient bot = commands.Bot(command_prefix="!") # Function that will
 return the current bot's stats. async def get_stats(): return {"servers": len
-(bot.guilds), "shards": 0, "members": len(bot.users)} # Function that will be
-called if stats are posted successfully. async def on_success_posting(): print
-("wow stats posting works") boticord_client = BoticordClient
+(bot.guilds), "shards": None, "members": len(bot.users)} # Function that will
+be called if stats are posted successfully. async def on_success_posting():
+print("wow stats posting works") boticord_client = BoticordClient
 ( "your_boticord_api_token", version=3 ) # <--- BotiCord API token autopost =
 ( boticord_client.autopost() .init_stats(get_stats) .on_success
 (on_success_posting) .start("id_of_your_bot") # <--- ID of your bot ) bot.run
 ("bot token") # <--- Discord bot's token ```
 ***** Links *****
 * [PyPi](https://pypi.org/project/boticordpy) * [Documentation](https://
 py.boticord.top) * [Github](https://github.com/boticord/boticordpy) *
```

### Comparing `boticordpy-3.0.1/README.md` & `boticordpy-3.0.2/boticordpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,28 @@
+Metadata-Version: 2.1
+Name: boticordpy
+Version: 3.0.2
+Summary: A Python wrapper for BotiCord API
+Home-page: https://github.com/boticord/boticordpy
+Author: Marakarka
+Author-email: support@kerdoku.top
+License: MIT
+Project-URL: Documentation, https://py.boticord.top/en/stable
+Project-URL: Issue tracker, https://github.com/boticord/boticordpy/issues
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >= 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 <p align="center">
-<img width="520" src="https://media.discordapp.net/attachments/929108234709639208/943873379809787964/boticordpylogo.png" alt="">
+<img width="560" src="https://github.com/boticord/boticordpy/assets/61203964/87393a07-2afa-4568-a324-500d1940b4fc" alt="">
 </p>
 
 <p align="center">
   <b>
     The easiest way to use BotiCord API in Python.
     <span> · </span>
     <a href="https://py.boticord.top/">Docs</a>
@@ -52,15 +71,15 @@
 from boticordpy import BoticordClient
 
 bot = commands.Bot(command_prefix="!")
 
 
 # Function that will return the current bot's stats.
 async def get_stats():
-    return {"servers": len(bot.guilds), "shards": 0, "members": len(bot.users)}
+    return {"servers": len(bot.guilds), "shards": None, "members": len(bot.users)}
 
 
 # Function that will be called if stats are posted successfully.
 async def on_success_posting():
     print("wow stats posting works")
```

#### html2text {}

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1 Name: boticordpy Version: 3.0.2 Summary: A Python wrapper
+for BotiCord API Home-page: https://github.com/boticord/boticordpy Author:
+Marakarka Author-email: support@kerdoku.top License: MIT Project-URL:
+Documentation, https://py.boticord.top/en/stable Project-URL: Issue tracker,
+https://github.com/boticord/boticordpy/issues Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >= 3.8 Description-Content-Type: text/markdown License-File:
+LICENSE.txt
            The easiest way to use BotiCord API in Python.  Â·  Docs
 
 ***** Features *****
 * Object-oriented * Full BotiCord API Coverage * Modern Pythonic API using
 `async`/`await` syntax * BotiCord Websocket * It is not necessary to use any
 particular library used to interact with the Discord API.
 ***** Installation *****
@@ -9,17 +19,17 @@
 library: ``` pip install boticordpy ``` ``` python3 -m pip install boticordpy
 ``` Or just clone the repo: https://github.com/boticord/boticordpy
 ***** Examples *****
 You can find other examples in an examples folder. **Discord.py Autopost
 example** ```py from discord.ext import commands from boticordpy import
 BoticordClient bot = commands.Bot(command_prefix="!") # Function that will
 return the current bot's stats. async def get_stats(): return {"servers": len
-(bot.guilds), "shards": 0, "members": len(bot.users)} # Function that will be
-called if stats are posted successfully. async def on_success_posting(): print
-("wow stats posting works") boticord_client = BoticordClient
+(bot.guilds), "shards": None, "members": len(bot.users)} # Function that will
+be called if stats are posted successfully. async def on_success_posting():
+print("wow stats posting works") boticord_client = BoticordClient
 ( "your_boticord_api_token", version=3 ) # <--- BotiCord API token autopost =
 ( boticord_client.autopost() .init_stats(get_stats) .on_success
 (on_success_posting) .start("id_of_your_bot") # <--- ID of your bot ) bot.run
 ("bot token") # <--- Discord bot's token ```
 ***** Links *****
 * [PyPi](https://pypi.org/project/boticordpy) * [Documentation](https://
 py.boticord.top) * [Github](https://github.com/boticord/boticordpy) *
```

### Comparing `boticordpy-3.0.1/boticordpy/autopost.py` & `boticordpy-3.0.2/boticordpy/autopost.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 from . import exceptions as bexc
 
 _logger = logging.getLogger("boticord.autopost")
 
 
 class AutoPost:
     """
-    You can use this class to post stats automatically.
+    You can use this to post stats automatically.
 
     Args:
         client (:obj:`~.client.BoticordClient`)
             An instance of BoticordClient.
     """
 
     __slots__ = (
         "client",
         "_interval",
         "_success",
         "_error",
         "_stats",
         "_task",
         "_stopped",
+        "bot_id"
     )
 
     _success: typing.Any
     _error: typing.Any
     _stats: typing.Any
     _task: typing.Optional["asyncio.Task[None]"]
 
@@ -106,14 +107,18 @@
 
     def init_stats(self, callback: typing.Any = None):
         """
         Registers a function that will return stats. Registered Function Must return dictionary.
 
         .. warning::
 
+            None of the values must be equal to 0. Specify None instead of 0.
+
+        .. warning::
+
             Callback functions must be a **coroutine**. If they aren't, then you might get unexpected
             errors. In order to turn a function into a coroutine they must be ``async def``
             functions.
 
         This method can be used as a decorator (if you want).
         """
         if callback is not None:
@@ -135,14 +140,15 @@
     def interval(self) -> float:
         """The interval between posting stats."""
         return self._interval
 
     def set_interval(self, seconds: int) -> "AutoPost":
         """
         Sets the interval between posting stats.
+        
         Args:
             seconds (:obj:`int`)
                 The interval.
         Raises:
             :obj:`ValueError`
                 Boticord recommends not to set interval lower than 900 seconds!
         """
```

### Comparing `boticordpy-3.0.1/boticordpy/client.py` & `boticordpy-3.0.2/boticordpy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,18 @@
         *,
         servers: typing.Optional[int] = None,
         shards: typing.Optional[int] = None,
         users: typing.Optional[int] = None,
     ) -> boticord_types.ResourceBot:
         """Post Bot's stats.
 
+        .. warning::
+
+            None of the values must be equal to 0. Specify None instead of 0.
+
         Args:
             bot_id (Union[:obj:`str`, :obj:`int`])
                 Id of the bot to post stats of.
             servers ( Optional[:obj:`int`] )
                 Bot's servers count
             shards ( Optional[:obj:`int`] )
                 Bot's shards count
```

### Comparing `boticordpy-3.0.1/boticordpy/exceptions.py` & `boticordpy-3.0.2/boticordpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `boticordpy-3.0.1/boticordpy/http.py` & `boticordpy-3.0.2/boticordpy/http.py`

 * *Files identical despite different names*

### Comparing `boticordpy-3.0.1/boticordpy/types.py` & `boticordpy-3.0.2/boticordpy/types.py`

 * *Files identical despite different names*

### Comparing `boticordpy-3.0.1/boticordpy/websocket.py` & `boticordpy-3.0.2/boticordpy/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,16 @@
         if code == 4000:
             _logger.info("Closed connection successfully.")
             return
         elif code == 1006:
             _logger.error("Token is invalid.")
             return
 
-        _logger.info("Disconnected from BotiCord. Reconnecting...")
+        _logger.info("Disconnected from BotiCord. Reconnecting in 1 second...")
+        await asyncio.sleep(1)
 
         await self.connect()
 
     async def _send_ping(self) -> None:
         if not self.ws.closed:
             await asyncio.sleep(45)
             await self.ws.send_json({"event": "ping"})
```

### Comparing `boticordpy-3.0.1/boticordpy.egg-info/PKG-INFO` & `boticordpy-3.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,9 @@
-Metadata-Version: 2.1
-Name: boticordpy
-Version: 3.0.1
-Summary: A Python wrapper for BotiCord API
-Home-page: https://github.com/boticord/boticordpy
-Author: Marakarka
-Author-email: support@kerdoku.top
-License: MIT
-Project-URL: Documentation, https://py.boticord.top/en/stable
-Project-URL: Issue tracker, https://github.com/boticord/boticordpy/issues
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >= 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <p align="center">
-<img width="520" src="https://media.discordapp.net/attachments/929108234709639208/943873379809787964/boticordpylogo.png" alt="">
+<img width="560" src="https://github.com/boticord/boticordpy/assets/61203964/87393a07-2afa-4568-a324-500d1940b4fc" alt="">
 </p>
 
 <p align="center">
   <b>
     The easiest way to use BotiCord API in Python.
     <span> · </span>
     <a href="https://py.boticord.top/">Docs</a>
@@ -71,15 +52,15 @@
 from boticordpy import BoticordClient
 
 bot = commands.Bot(command_prefix="!")
 
 
 # Function that will return the current bot's stats.
 async def get_stats():
-    return {"servers": len(bot.guilds), "shards": 0, "members": len(bot.users)}
+    return {"servers": len(bot.guilds), "shards": None, "members": len(bot.users)}
 
 
 # Function that will be called if stats are posted successfully.
 async def on_success_posting():
     print("wow stats posting works")
```

#### html2text {}

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1 Name: boticordpy Version: 3.0.1 Summary: A Python wrapper
-for BotiCord API Home-page: https://github.com/boticord/boticordpy Author:
-Marakarka Author-email: support@kerdoku.top License: MIT Project-URL:
-Documentation, https://py.boticord.top/en/stable Project-URL: Issue tracker,
-https://github.com/boticord/boticordpy/issues Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >= 3.8 Description-Content-Type: text/markdown License-File:
-LICENSE.txt
            The easiest way to use BotiCord API in Python.  Â·  Docs
 
 ***** Features *****
 * Object-oriented * Full BotiCord API Coverage * Modern Pythonic API using
 `async`/`await` syntax * BotiCord Websocket * It is not necessary to use any
 particular library used to interact with the Discord API.
 ***** Installation *****
@@ -19,17 +9,17 @@
 library: ``` pip install boticordpy ``` ``` python3 -m pip install boticordpy
 ``` Or just clone the repo: https://github.com/boticord/boticordpy
 ***** Examples *****
 You can find other examples in an examples folder. **Discord.py Autopost
 example** ```py from discord.ext import commands from boticordpy import
 BoticordClient bot = commands.Bot(command_prefix="!") # Function that will
 return the current bot's stats. async def get_stats(): return {"servers": len
-(bot.guilds), "shards": 0, "members": len(bot.users)} # Function that will be
-called if stats are posted successfully. async def on_success_posting(): print
-("wow stats posting works") boticord_client = BoticordClient
+(bot.guilds), "shards": None, "members": len(bot.users)} # Function that will
+be called if stats are posted successfully. async def on_success_posting():
+print("wow stats posting works") boticord_client = BoticordClient
 ( "your_boticord_api_token", version=3 ) # <--- BotiCord API token autopost =
 ( boticord_client.autopost() .init_stats(get_stats) .on_success
 (on_success_posting) .start("id_of_your_bot") # <--- ID of your bot ) bot.run
 ("bot token") # <--- Discord bot's token ```
 ***** Links *****
 * [PyPi](https://pypi.org/project/boticordpy) * [Documentation](https://
 py.boticord.top) * [Github](https://github.com/boticord/boticordpy) *
```

### Comparing `boticordpy-3.0.1/setup.py` & `boticordpy-3.0.2/setup.py`

 * *Files identical despite different names*

