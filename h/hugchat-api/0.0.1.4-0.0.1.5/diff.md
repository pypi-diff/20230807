# Comparing `tmp/hugchat_api-0.0.1.4.tar.gz` & `tmp/hugchat_api-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat_api-0.0.1.4.tar", last modified: Sat Jul  1 05:02:09 2023, max compression
+gzip compressed data, was "hugchat_api-0.0.1.5.tar", last modified: Mon Aug  7 13:22:59 2023, max compression
```

## Comparing `hugchat_api-0.0.1.4.tar` & `hugchat_api-0.0.1.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 05:02:09.620181 hugchat_api-0.0.1.4/
--rw-rw-rw-   0        0        0    35823 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/LICENSE
--rw-rw-rw-   0        0        0     6237 2023-07-01 05:02:09.619180 hugchat_api-0.0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5397 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 05:02:09.600170 hugchat_api-0.0.1.4/hugchat_api/
--rw-rw-rw-   0        0        0      296 2023-07-01 05:01:45.000000 hugchat_api-0.0.1.4/hugchat_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 05:02:09.616181 hugchat_api-0.0.1.4/hugchat_api/core/
--rw-rw-rw-   0        0        0    13732 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/Bot.py
--rw-rw-rw-   0        0        0       55 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/Exceptions.py
--rw-rw-rw-   0        0        0     1641 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/Message.py
--rw-rw-rw-   0        0        0     7133 2023-07-01 05:01:45.000000 hugchat_api-0.0.1.4/hugchat_api/core/Sign.py
--rw-rw-rw-   0        0        0     1278 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/ThreadPool.py
--rw-rw-rw-   0        0        0     4247 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/WebSearch.py
--rw-rw-rw-   0        0        0      758 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/__init__.py
--rw-rw-rw-   0        0        0     6737 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.4/hugchat_api/terminal_cli.py
-drwxrwxrwx   0        0        0        0 2023-07-01 05:02:09.618170 hugchat_api-0.0.1.4/hugchat_api/utils/
--rw-rw-rw-   0        0        0     1726 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 05:02:09.606183 hugchat_api-0.0.1.4/hugchat_api.egg-info/
--rw-rw-rw-   0        0        0     6237 2023-07-01 05:02:09.000000 hugchat_api-0.0.1.4/hugchat_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-07-01 05:02:09.000000 hugchat_api-0.0.1.4/hugchat_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 05:02:09.000000 hugchat_api-0.0.1.4/hugchat_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-01 05:02:09.000000 hugchat_api-0.0.1.4/hugchat_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 05:02:09.000000 hugchat_api-0.0.1.4/hugchat_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 05:02:09.620181 hugchat_api-0.0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1193 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 13:22:59.863009 hugchat_api-0.0.1.5/
+-rw-rw-rw-   0        0        0    35823 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6483 2023-08-07 13:22:59.862009 hugchat_api-0.0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5612 2023-08-07 13:08:44.000000 hugchat_api-0.0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 13:22:59.840004 hugchat_api-0.0.1.5/hugchat_api/
+-rw-rw-rw-   0        0        0      327 2023-08-07 13:08:44.000000 hugchat_api-0.0.1.5/hugchat_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 13:22:59.860011 hugchat_api-0.0.1.5/hugchat_api/core/
+-rw-rw-rw-   0        0        0    13749 2023-08-07 13:08:44.000000 hugchat_api-0.0.1.5/hugchat_api/core/Bot.py
+-rw-rw-rw-   0        0        0       55 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.5/hugchat_api/core/Exceptions.py
+-rw-rw-rw-   0        0        0      115 2023-08-07 13:08:44.000000 hugchat_api-0.0.1.5/hugchat_api/core/ListBots.py
+-rw-rw-rw-   0        0        0     1641 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.5/hugchat_api/core/Message.py
+-rw-rw-rw-   0        0        0     7133 2023-07-01 05:01:45.000000 hugchat_api-0.0.1.5/hugchat_api/core/Sign.py
+-rw-rw-rw-   0        0        0     1278 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.5/hugchat_api/core/ThreadPool.py
+-rw-rw-rw-   0        0        0     4247 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.5/hugchat_api/core/WebSearch.py
+-rw-rw-rw-   0        0        0      774 2023-08-07 13:08:44.000000 hugchat_api-0.0.1.5/hugchat_api/core/__init__.py
+-rw-rw-rw-   0        0        0     6790 2023-08-07 13:08:44.000000 hugchat_api-0.0.1.5/hugchat_api/terminal_cli.py
+drwxrwxrwx   0        0        0        0 2023-08-07 13:22:59.861009 hugchat_api-0.0.1.5/hugchat_api/utils/
+-rw-rw-rw-   0        0        0     1726 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.5/hugchat_api/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 13:22:59.846006 hugchat_api-0.0.1.5/hugchat_api.egg-info/
+-rw-rw-rw-   0        0        0     6483 2023-08-07 13:22:59.000000 hugchat_api-0.0.1.5/hugchat_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-08-07 13:22:59.000000 hugchat_api-0.0.1.5/hugchat_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 13:22:59.000000 hugchat_api-0.0.1.5/hugchat_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-08-07 13:22:59.000000 hugchat_api-0.0.1.5/hugchat_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-07 13:22:59.000000 hugchat_api-0.0.1.5/hugchat_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 13:22:59.863009 hugchat_api-0.0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-08-07 13:22:12.000000 hugchat_api-0.0.1.5/setup.py
```

### Comparing `hugchat_api-0.0.1.4/LICENSE` & `hugchat_api-0.0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.4/PKG-INFO` & `hugchat_api-0.0.1.5/hugchat_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: hugchat_api
-Version: 0.0.1.4
-Summary: Chat using huggingchat, 'stream' response and 'Search Web' supported.
+Name: hugchat-api
+Version: 0.0.1.5
+Summary: Chat using huggingchat, 'stream' response and 'Search Web' supported. (MetaAI's new model supported)
 Home-page: https://github.com/ogios/huggingchat-api
 Author: ogios
 Author-email: 2134692955@qq.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -62,15 +62,15 @@
 ## API Usage
 
 </summary>
 
 
 - Create Bot
 ```python
-bot = HUG.getBot(email=EMAIL, cookies=cookies)
+bot = HUG.getBot(email=EMAIL, cookies=cookies, model=ListBots.<model name>)
 ```
 - Get all conversations & Print title
 ```python
 conversations = bot.getConversations()
 conv_id = list(conversations.keys())[0]
 print(conversations[conv_id])
 ```
@@ -109,57 +109,74 @@
 print(message.getText())
 ```
 
 **Code:**
 
 ```python
 import os, time
+
 from hugchat_api import HuggingChat
+from hugchat_api.core import ListBots
 from hugchat_api.utils import formatHistory, formatConversations
 
-EMAIL = os.getenv("EMAIL_QQ")
-PASSWD = ""
+EMAIL = os.getenv("EMAIL")
+PASSWD = os.getenv("PASSWD")
 COOKIE_STORE_PATH = "./usercookies"
 
-# create ThreadPool
-HUG = HuggingChat(max_thread=1)       
+'''create ThreadPool'''
+HUG = HuggingChat(max_thread=1)
 
-# initialize sign in funciton
-sign = HUG.getSign(EMAIL, PASSWD)   
-# sign in or...
+
+'''initialize sign in funciton'''
+sign = HUG.getSign(EMAIL, PASSWD)
+
+'''sign in or...'''
 cookies = sign.login(save=True, cookie_dir_path=COOKIE_STORE_PATH)
-# create bot
-bot = HUG.getBot(email=EMAIL, cookies=cookies)
-# get all conversations and see one's title
+# cookies = sign.loadCookiesFromDir()
+
+
+
+'''create bot with MetaAI's model'''
+bot = HUG.getBot(email=EMAIL, cookies=cookies, model=ListBots.META_70B_HF)
+
+'''get all conversations and see one's title'''
 conversations = bot.getConversations()
 conv_id = list(conversations.keys())[0]
 print(conversations[conv_id])
-# get all chat histories by conversation_id
+
+'''get all chat histories by conversation_id'''
 histories = bot.getHistoriesByID(conversation_id=conv_id)
 print(formatHistory(histories))
-# delete a conversation
+
+'''delete a conversation'''
 bot.removeConversation(conversation_id=conv_id)
-# create a new conversation
+
+'''create a new conversation'''
 conversation_id = bot.createConversation()
-# chat
+
+'''chat'''
 message = bot.chat(
     text="hi",
     conversation_id=conversation_id,
     web_search=True,
     max_tries=2,
     # callback=(bot.updateTitle, (conversation_id,))
 )
-# wait the full text or...
+
+
+
+'''wait the full text or...'''
 while not message.web_search_done:
     time.sleep(0.1)
 print(message.getWebSearchSteps())
 while not message.isDone():
     time.sleep(0.1)
 print(message.getFinalText())
-# get the stream text instantly
+
+'''get the stream text instantly'''
 print(message.getWebSearchSteps())
 print(message.getText())
 ```
 
 </details>
 
 
@@ -205,20 +222,20 @@
 #
 #       0. [649471fa525d2d2474973871] - Hello there! How can I help you? Let me know if you need something specific done.
 #       1. [64946fb2525d2d247497382c] - Hi there! How can I assist you?
 
 (None) > /cd 0
 (647e09ccabd9de3d82d6fba0) > hi
 #(user): hi
-#(Open-Assistant): ...
+#(HFBot): ...
 (647e09ccabd9de3d82d6fba0) > /web
 #WEB_SEARCH is set to `True`
 (647e09ccabd9de3d82d6fba0) > hi
 # ...(steps about web search)
-#(Open-Assistant): ...
+#(HFBot): ...
 ```
 
 </details>
 
 ## Download status
 seperated in regions(country_code). powered by bigquery and mermaid.
 ![test](http://47.94.146.109:8000/.md)
```

### Comparing `hugchat_api-0.0.1.4/README.md` & `hugchat_api-0.0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 ## API Usage
 
 </summary>
 
 
 - Create Bot
 ```python
-bot = HUG.getBot(email=EMAIL, cookies=cookies)
+bot = HUG.getBot(email=EMAIL, cookies=cookies, model=ListBots.<model name>)
 ```
 - Get all conversations & Print title
 ```python
 conversations = bot.getConversations()
 conv_id = list(conversations.keys())[0]
 print(conversations[conv_id])
 ```
@@ -88,57 +88,74 @@
 print(message.getText())
 ```
 
 **Code:**
 
 ```python
 import os, time
+
 from hugchat_api import HuggingChat
+from hugchat_api.core import ListBots
 from hugchat_api.utils import formatHistory, formatConversations
 
-EMAIL = os.getenv("EMAIL_QQ")
-PASSWD = ""
+EMAIL = os.getenv("EMAIL")
+PASSWD = os.getenv("PASSWD")
 COOKIE_STORE_PATH = "./usercookies"
 
-# create ThreadPool
-HUG = HuggingChat(max_thread=1)       
+'''create ThreadPool'''
+HUG = HuggingChat(max_thread=1)
+
+
+'''initialize sign in funciton'''
+sign = HUG.getSign(EMAIL, PASSWD)
 
-# initialize sign in funciton
-sign = HUG.getSign(EMAIL, PASSWD)   
-# sign in or...
+'''sign in or...'''
 cookies = sign.login(save=True, cookie_dir_path=COOKIE_STORE_PATH)
-# create bot
-bot = HUG.getBot(email=EMAIL, cookies=cookies)
-# get all conversations and see one's title
+# cookies = sign.loadCookiesFromDir()
+
+
+
+'''create bot with MetaAI's model'''
+bot = HUG.getBot(email=EMAIL, cookies=cookies, model=ListBots.META_70B_HF)
+
+'''get all conversations and see one's title'''
 conversations = bot.getConversations()
 conv_id = list(conversations.keys())[0]
 print(conversations[conv_id])
-# get all chat histories by conversation_id
+
+'''get all chat histories by conversation_id'''
 histories = bot.getHistoriesByID(conversation_id=conv_id)
 print(formatHistory(histories))
-# delete a conversation
+
+'''delete a conversation'''
 bot.removeConversation(conversation_id=conv_id)
-# create a new conversation
+
+'''create a new conversation'''
 conversation_id = bot.createConversation()
-# chat
+
+'''chat'''
 message = bot.chat(
     text="hi",
     conversation_id=conversation_id,
     web_search=True,
     max_tries=2,
     # callback=(bot.updateTitle, (conversation_id,))
 )
-# wait the full text or...
+
+
+
+'''wait the full text or...'''
 while not message.web_search_done:
     time.sleep(0.1)
 print(message.getWebSearchSteps())
 while not message.isDone():
     time.sleep(0.1)
 print(message.getFinalText())
-# get the stream text instantly
+
+'''get the stream text instantly'''
 print(message.getWebSearchSteps())
 print(message.getText())
 ```
 
 </details>
 
 
@@ -184,20 +201,20 @@
 #
 #       0. [649471fa525d2d2474973871] - Hello there! How can I help you? Let me know if you need something specific done.
 #       1. [64946fb2525d2d247497382c] - Hi there! How can I assist you?
 
 (None) > /cd 0
 (647e09ccabd9de3d82d6fba0) > hi
 #(user): hi
-#(Open-Assistant): ...
+#(HFBot): ...
 (647e09ccabd9de3d82d6fba0) > /web
 #WEB_SEARCH is set to `True`
 (647e09ccabd9de3d82d6fba0) > hi
 # ...(steps about web search)
-#(Open-Assistant): ...
+#(HFBot): ...
 ```
 
 </details>
 
 ## Download status
 seperated in regions(country_code). powered by bigquery and mermaid.
 ![test](http://47.94.146.109:8000/.md)
```

### Comparing `hugchat_api-0.0.1.4/hugchat_api/core/Bot.py` & `hugchat_api-0.0.1.5/hugchat_api/core/Bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,26 @@
 from typing import Callable, Tuple
 
 from .WebSearch import WebSearch
 from .Message import Message
 from .ThreadPool import ThreadPool
 from ..utils import getTime
 from .Exceptions import *
+from . import ListBots
+
+
 
 
 class Bot:
     def __init__(
             self,
             email: str,
             cookies: requests.sessions.RequestsCookieJar,
             thread_pool: ThreadPool,
-            model: str = "OpenAssistant/oasst-sft-6-llama-30b-xor",
+            model: str = ListBots.OPENASSISTENT_30B_XOR,
     ):
         self.thread_pool: ThreadPool = thread_pool
         self.email = email
         self.model = model
         self.default_params = {
             "temperature": 0.9,
             "top_p": 0.95,
```

### Comparing `hugchat_api-0.0.1.4/hugchat_api/core/Message.py` & `hugchat_api-0.0.1.5/hugchat_api/core/Message.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.4/hugchat_api/core/Sign.py` & `hugchat_api-0.0.1.5/hugchat_api/core/Sign.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.4/hugchat_api/core/ThreadPool.py` & `hugchat_api-0.0.1.5/hugchat_api/core/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.4/hugchat_api/core/WebSearch.py` & `hugchat_api-0.0.1.5/hugchat_api/core/WebSearch.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.4/hugchat_api/core/__init__.py` & `hugchat_api-0.0.1.5/hugchat_api/core/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from concurrent.futures import ThreadPoolExecutor
 from requests.sessions import RequestsCookieJar
-from requests import sessions
+
 
 from .Bot import Bot
 from .Sign import Sign
 from .ThreadPool import ThreadPool
+from . import ListBots
 
 
 class HuggingChat:
     def __init__(self, max_thread: int = 5):
         # self.thread_pool = ThreadPoolExecutor(max_workers=max_thread)
         self.thread_pool = ThreadPool(max_thread)
     
-    def getBot(self, email: str, cookies: RequestsCookieJar):
+    def getBot(self, email: str, cookies: RequestsCookieJar, model: str = ListBots.OPENASSISTENT_30B_XOR):
         bot = Bot(
             email=email,
             cookies=cookies,
-            thread_pool=self.thread_pool
+            thread_pool=self.thread_pool,
+            model=model,
         )
         return bot
     
     def getSign(self, email, passwd):
         return Sign(
             email=email,
             passwd=passwd
```

### Comparing `hugchat_api-0.0.1.4/hugchat_api/terminal_cli.py` & `hugchat_api-0.0.1.5/hugchat_api/terminal_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # from rich.markdown import Markdown
 
 from .core import HuggingChat
 from .core.Message import Message
 from .core.Sign import Sign
 from .core.Bot import Bot
 from .utils import color, formatHistory, formatConversations, getTextFromInput, getIdByIndex
+from .core import ListBots
 
 # COOKIE_DIR_PATH = os.path.abspath(os.path.dirname(__file__)) + "/usercookies"
 # CONSOLE = Console()
 hug = HuggingChat()
 
 # FLAG = False
 WEB_SEARCH = False
@@ -53,15 +54,15 @@
     while not message.done:
         if message.error:
             logging.error(str(message.error))
             return
         time.sleep(0.5)
         
     msg = message.getFinalText()
-    string = f"({color('Open-Assistant', 'blue')}): {msg}"
+    string = f"({color('HFBot: ', 'blue')}): {msg}"
     print(string)
     # try:
     #     markdown = Markdown(string)
     #     CONSOLE.print(markdown)
     # except:
     #     print(string)
 
@@ -129,15 +130,15 @@
     elif not checkCookies(u):
         p = getpass.getpass() if not PASSWD else PASSWD
     else:
         p = None
     
     cookies = login(u, p, force)
     print(f"You are now logged in as <{u}>")
-    bot: Bot = hug.getBot(u, cookies=cookies)
+    bot: Bot.Bot = hug.getBot(u, cookies=cookies, model=ListBots.META_70B_HF)
     gc.collect()
     while 1:
         try:
             gc.collect()
             # while FLAG:
             #     time.sleep(0.1)
             #     continue
```

### Comparing `hugchat_api-0.0.1.4/hugchat_api/utils/__init__.py` & `hugchat_api-0.0.1.5/hugchat_api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.4/hugchat_api.egg-info/PKG-INFO` & `hugchat_api-0.0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: hugchat-api
-Version: 0.0.1.4
-Summary: Chat using huggingchat, 'stream' response and 'Search Web' supported.
+Name: hugchat_api
+Version: 0.0.1.5
+Summary: Chat using huggingchat, 'stream' response and 'Search Web' supported. (MetaAI's new model supported)
 Home-page: https://github.com/ogios/huggingchat-api
 Author: ogios
 Author-email: 2134692955@qq.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -62,15 +62,15 @@
 ## API Usage
 
 </summary>
 
 
 - Create Bot
 ```python
-bot = HUG.getBot(email=EMAIL, cookies=cookies)
+bot = HUG.getBot(email=EMAIL, cookies=cookies, model=ListBots.<model name>)
 ```
 - Get all conversations & Print title
 ```python
 conversations = bot.getConversations()
 conv_id = list(conversations.keys())[0]
 print(conversations[conv_id])
 ```
@@ -109,57 +109,74 @@
 print(message.getText())
 ```
 
 **Code:**
 
 ```python
 import os, time
+
 from hugchat_api import HuggingChat
+from hugchat_api.core import ListBots
 from hugchat_api.utils import formatHistory, formatConversations
 
-EMAIL = os.getenv("EMAIL_QQ")
-PASSWD = ""
+EMAIL = os.getenv("EMAIL")
+PASSWD = os.getenv("PASSWD")
 COOKIE_STORE_PATH = "./usercookies"
 
-# create ThreadPool
-HUG = HuggingChat(max_thread=1)       
+'''create ThreadPool'''
+HUG = HuggingChat(max_thread=1)
 
-# initialize sign in funciton
-sign = HUG.getSign(EMAIL, PASSWD)   
-# sign in or...
+
+'''initialize sign in funciton'''
+sign = HUG.getSign(EMAIL, PASSWD)
+
+'''sign in or...'''
 cookies = sign.login(save=True, cookie_dir_path=COOKIE_STORE_PATH)
-# create bot
-bot = HUG.getBot(email=EMAIL, cookies=cookies)
-# get all conversations and see one's title
+# cookies = sign.loadCookiesFromDir()
+
+
+
+'''create bot with MetaAI's model'''
+bot = HUG.getBot(email=EMAIL, cookies=cookies, model=ListBots.META_70B_HF)
+
+'''get all conversations and see one's title'''
 conversations = bot.getConversations()
 conv_id = list(conversations.keys())[0]
 print(conversations[conv_id])
-# get all chat histories by conversation_id
+
+'''get all chat histories by conversation_id'''
 histories = bot.getHistoriesByID(conversation_id=conv_id)
 print(formatHistory(histories))
-# delete a conversation
+
+'''delete a conversation'''
 bot.removeConversation(conversation_id=conv_id)
-# create a new conversation
+
+'''create a new conversation'''
 conversation_id = bot.createConversation()
-# chat
+
+'''chat'''
 message = bot.chat(
     text="hi",
     conversation_id=conversation_id,
     web_search=True,
     max_tries=2,
     # callback=(bot.updateTitle, (conversation_id,))
 )
-# wait the full text or...
+
+
+
+'''wait the full text or...'''
 while not message.web_search_done:
     time.sleep(0.1)
 print(message.getWebSearchSteps())
 while not message.isDone():
     time.sleep(0.1)
 print(message.getFinalText())
-# get the stream text instantly
+
+'''get the stream text instantly'''
 print(message.getWebSearchSteps())
 print(message.getText())
 ```
 
 </details>
 
 
@@ -205,20 +222,20 @@
 #
 #       0. [649471fa525d2d2474973871] - Hello there! How can I help you? Let me know if you need something specific done.
 #       1. [64946fb2525d2d247497382c] - Hi there! How can I assist you?
 
 (None) > /cd 0
 (647e09ccabd9de3d82d6fba0) > hi
 #(user): hi
-#(Open-Assistant): ...
+#(HFBot): ...
 (647e09ccabd9de3d82d6fba0) > /web
 #WEB_SEARCH is set to `True`
 (647e09ccabd9de3d82d6fba0) > hi
 # ...(steps about web search)
-#(Open-Assistant): ...
+#(HFBot): ...
 ```
 
 </details>
 
 ## Download status
 seperated in regions(country_code). powered by bigquery and mermaid.
 ![test](http://47.94.146.109:8000/.md)
```

### Comparing `hugchat_api-0.0.1.4/setup.py` & `hugchat_api-0.0.1.5/setup.py`

 * *Files identical despite different names*

