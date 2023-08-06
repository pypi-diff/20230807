# Comparing `tmp/phxsocket-0.1.2.tar.gz` & `tmp/phxsocket-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phxsocket-0.1.2.tar", last modified: Wed Oct 20 05:51:31 2021, max compression
+gzip compressed data, was "phxsocket-0.1.3.tar", last modified: Sun Aug  6 23:00:45 2023, max compression
```

## Comparing `phxsocket-0.1.2.tar` & `phxsocket-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0 w         (1000) w         (1000)        0 2021-10-20 05:51:31.992246 phxsocket-0.1.2/
--rwxrwxrwx   0 w         (1000) w         (1000)     2721 2021-10-20 05:51:31.970247 phxsocket-0.1.2/PKG-INFO
--rwxrwxrwx   0 w         (1000) w         (1000)     1619 2021-10-20 04:40:32.000000 phxsocket-0.1.2/README.md
-drwxrwxrwx   0 w         (1000) w         (1000)        0 2021-10-20 05:51:31.851252 phxsocket-0.1.2/phxsocket/
--rwxrwxrwx   0 w         (1000) w         (1000)      129 2020-10-30 14:39:40.000000 phxsocket-0.1.2/phxsocket/__init__.py
--rwxrwxrwx   0 w         (1000) w         (1000)     2044 2021-10-20 05:49:49.000000 phxsocket-0.1.2/phxsocket/channel.py
--rwxrwxrwx   0 w         (1000) w         (1000)     5673 2021-10-20 05:49:49.000000 phxsocket-0.1.2/phxsocket/client.py
--rwxrwxrwx   0 w         (1000) w         (1000)      590 2021-10-20 05:49:49.000000 phxsocket-0.1.2/phxsocket/message.py
-drwxrwxrwx   0 w         (1000) w         (1000)        0 2021-10-20 05:51:31.948247 phxsocket-0.1.2/phxsocket.egg-info/
--rwxrwxrwx   0 w         (1000) w         (1000)     2721 2021-10-20 05:51:31.000000 phxsocket-0.1.2/phxsocket.egg-info/PKG-INFO
--rwxrwxrwx   0 w         (1000) w         (1000)      266 2021-10-20 05:51:31.000000 phxsocket-0.1.2/phxsocket.egg-info/SOURCES.txt
--rwxrwxrwx   0 w         (1000) w         (1000)        1 2021-10-20 05:51:31.000000 phxsocket-0.1.2/phxsocket.egg-info/dependency_links.txt
--rwxrwxrwx   0 w         (1000) w         (1000)       16 2021-10-20 05:51:31.000000 phxsocket-0.1.2/phxsocket.egg-info/requires.txt
--rwxrwxrwx   0 w         (1000) w         (1000)       10 2021-10-20 05:51:31.000000 phxsocket-0.1.2/phxsocket.egg-info/top_level.txt
--rwxrwxrwx   0 w         (1000) w         (1000)       38 2021-10-20 05:51:31.993746 phxsocket-0.1.2/setup.cfg
--rwxrwxrwx   0 w         (1000) w         (1000)      748 2021-10-20 05:51:21.000000 phxsocket-0.1.2/setup.py
+drwxrwxrwx   0 w         (1000) w         (1000)        0 2023-08-06 23:00:45.980731 phxsocket-0.1.3/
+-rwxrwxrwx   0 w         (1000) w         (1000)    35149 2020-10-30 14:37:35.000000 phxsocket-0.1.3/LICENSE
+-rwxrwxrwx   0 w         (1000) w         (1000)     2117 2023-08-06 23:00:45.978781 phxsocket-0.1.3/PKG-INFO
+-rwxrwxrwx   0 w         (1000) w         (1000)     1619 2021-10-20 04:40:32.000000 phxsocket-0.1.3/README.md
+drwxrwxrwx   0 w         (1000) w         (1000)        0 2023-08-06 23:00:45.860849 phxsocket-0.1.3/phxsocket/
+-rwxrwxrwx   0 w         (1000) w         (1000)      129 2020-10-30 14:39:40.000000 phxsocket-0.1.3/phxsocket/__init__.py
+-rwxrwxrwx   0 w         (1000) w         (1000)     2044 2021-10-20 05:49:49.000000 phxsocket-0.1.3/phxsocket/channel.py
+-rwxrwxrwx   0 w         (1000) w         (1000)     5637 2021-10-20 07:32:16.000000 phxsocket-0.1.3/phxsocket/client.py
+-rwxrwxrwx   0 w         (1000) w         (1000)      590 2021-10-20 05:49:49.000000 phxsocket-0.1.3/phxsocket/message.py
+drwxrwxrwx   0 w         (1000) w         (1000)        0 2023-08-06 23:00:45.957198 phxsocket-0.1.3/phxsocket.egg-info/
+-rwxrwxrwx   0 w         (1000) w         (1000)     2117 2023-08-06 23:00:45.000000 phxsocket-0.1.3/phxsocket.egg-info/PKG-INFO
+-rwxrwxrwx   0 w         (1000) w         (1000)      274 2023-08-06 23:00:45.000000 phxsocket-0.1.3/phxsocket.egg-info/SOURCES.txt
+-rwxrwxrwx   0 w         (1000) w         (1000)        1 2023-08-06 23:00:45.000000 phxsocket-0.1.3/phxsocket.egg-info/dependency_links.txt
+-rwxrwxrwx   0 w         (1000) w         (1000)       16 2023-08-06 23:00:45.000000 phxsocket-0.1.3/phxsocket.egg-info/requires.txt
+-rwxrwxrwx   0 w         (1000) w         (1000)       10 2023-08-06 23:00:45.000000 phxsocket-0.1.3/phxsocket.egg-info/top_level.txt
+-rwxrwxrwx   0 w         (1000) w         (1000)       38 2023-08-06 23:00:45.981732 phxsocket-0.1.3/setup.cfg
+-rwxrwxrwx   0 w         (1000) w         (1000)      749 2023-08-06 22:59:50.000000 phxsocket-0.1.3/setup.py
```

### Comparing `phxsocket-0.1.2/PKG-INFO` & `phxsocket-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,95 @@
 Metadata-Version: 2.1
 Name: phxsocket
-Version: 0.1.2
+Version: 0.1.3
 Summary: Websocket client for Phoenix Elixir
 Home-page: https://github.com/wwww-wwww/phxsocket
 Author: wwwwwwww
 Author-email: wvvwvvvvwvvw@gmail.com
 License: UNKNOWN
-Description: # phxsocket
-        ### Synchronous phoenix websocket client using callbacks
-        [Phoenix channels](https://hexdocs.pm/phoenix/channels.html)
-        ## Requirements
-        `websockets`
-        
-        ## Usage
-        Import the package
-        ```python
-        import phxsocket
-        ```
-        
-        Create socket client
-        ```python
-        socket = phxsocket.Client("wss://target.url/channel/websocket", {"options": "something"})
-        ```
-        
-        Connect and join a channel
-        ```python
-        if socket.connect(): # blocking, raises exception on failure
-          channel = socket.channel("room:roomname", {"more options": "something else"})
-          resp = channel.join() # also blocking, raises exception on failure
-        ```
-        
-        Alternatively
-        ```python
-        def connect_to_channel(socket):
-          channel = socket.channel("room:roomname", {"more options": "something else"})
-          resp = channel.join()
-          
-        socket.on_open = connect_to_channel
-        connection = socket.connect(blocking=False)
-        
-        connection.wait() # blocking, raises exception on failure
-        ```
-        
-        Reconnect on disconnection
-        ```python
-        socket.on_close = lambda socket: socket.connect()
-        ```
-        
-        Subscribe to events
-        ```python
-        def do_something(payload):
-          thing = payload["thing"]
-        
-        channel.on("eventname", do_something)
-        ```
-        
-        Push data to a channel
-        ```python
-        channel.push("eventname", {"some": "data"})
-        ```
-        
-        Push data and wait for a response
-        ```python
-        message = channel.push("eventname", {"some": "data"}, reply=True)
-        response = message.wait_for_response() # blocking
-        ```
-        
-        Push data and react to the response with a callback
-        ```python
-        def respond(payload):
-          print(payload)
-        
-        channel.push("eventname", {"some": "data"}, respond)
-        ```
-        
-        Leave a channel
-        ```python
-        channel.leave()
-        ```
-        
-        Disconnect
-        ```python
-        socket.close()
-        ```
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# phxsocket
+### Synchronous phoenix websocket client using callbacks
+[Phoenix channels](https://hexdocs.pm/phoenix/channels.html)
+## Requirements
+`websockets`
+
+## Usage
+Import the package
+```python
+import phxsocket
+```
+
+Create socket client
+```python
+socket = phxsocket.Client("wss://target.url/channel/websocket", {"options": "something"})
+```
+
+Connect and join a channel
+```python
+if socket.connect(): # blocking, raises exception on failure
+  channel = socket.channel("room:roomname", {"more options": "something else"})
+  resp = channel.join() # also blocking, raises exception on failure
+```
+
+Alternatively
+```python
+def connect_to_channel(socket):
+  channel = socket.channel("room:roomname", {"more options": "something else"})
+  resp = channel.join()
+  
+socket.on_open = connect_to_channel
+connection = socket.connect(blocking=False)
+
+connection.wait() # blocking, raises exception on failure
+```
+
+Reconnect on disconnection
+```python
+socket.on_close = lambda socket: socket.connect()
+```
+
+Subscribe to events
+```python
+def do_something(payload):
+  thing = payload["thing"]
+
+channel.on("eventname", do_something)
+```
+
+Push data to a channel
+```python
+channel.push("eventname", {"some": "data"})
+```
+
+Push data and wait for a response
+```python
+message = channel.push("eventname", {"some": "data"}, reply=True)
+response = message.wait_for_response() # blocking
+```
+
+Push data and react to the response with a callback
+```python
+def respond(payload):
+  print(payload)
+
+channel.push("eventname", {"some": "data"}, respond)
+```
+
+Leave a channel
+```python
+channel.leave()
+```
+
+Disconnect
+```python
+socket.close()
+```
+
+
```

### Comparing `phxsocket-0.1.2/README.md` & `phxsocket-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `phxsocket-0.1.2/phxsocket/channel.py` & `phxsocket-0.1.3/phxsocket/channel.py`

 * *Files identical despite different names*

### Comparing `phxsocket-0.1.2/phxsocket/client.py` & `phxsocket-0.1.3/phxsocket/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,16 +91,15 @@
   async def _run(self, loop, send_queue, connect_evt, shutdown_evt):
     async with websockets.connect(self.url) as websocket:
       connect_evt.respond(None)
       broadcast = loop.create_task(self._broadcast(websocket, send_queue))
       listen = loop.create_task(self._listen(websocket))
       shutdown = loop.create_task(shutdown_evt.wait())
       await asyncio.wait({listen, shutdown, broadcast},
-                         return_when=asyncio.FIRST_COMPLETED,
-                         loop=loop)
+                         return_when=asyncio.FIRST_COMPLETED)
 
   def run(self, connect_evt):
     self._loop = loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
 
     self._send_queue = asyncio.Queue()
     self._shutdown_evt = asyncio.Event()
```

### Comparing `phxsocket-0.1.2/phxsocket/message.py` & `phxsocket-0.1.3/phxsocket/message.py`

 * *Files identical despite different names*

### Comparing `phxsocket-0.1.2/phxsocket.egg-info/PKG-INFO` & `phxsocket-0.1.3/phxsocket.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,95 @@
 Metadata-Version: 2.1
 Name: phxsocket
-Version: 0.1.2
+Version: 0.1.3
 Summary: Websocket client for Phoenix Elixir
 Home-page: https://github.com/wwww-wwww/phxsocket
 Author: wwwwwwww
 Author-email: wvvwvvvvwvvw@gmail.com
 License: UNKNOWN
-Description: # phxsocket
-        ### Synchronous phoenix websocket client using callbacks
-        [Phoenix channels](https://hexdocs.pm/phoenix/channels.html)
-        ## Requirements
-        `websockets`
-        
-        ## Usage
-        Import the package
-        ```python
-        import phxsocket
-        ```
-        
-        Create socket client
-        ```python
-        socket = phxsocket.Client("wss://target.url/channel/websocket", {"options": "something"})
-        ```
-        
-        Connect and join a channel
-        ```python
-        if socket.connect(): # blocking, raises exception on failure
-          channel = socket.channel("room:roomname", {"more options": "something else"})
-          resp = channel.join() # also blocking, raises exception on failure
-        ```
-        
-        Alternatively
-        ```python
-        def connect_to_channel(socket):
-          channel = socket.channel("room:roomname", {"more options": "something else"})
-          resp = channel.join()
-          
-        socket.on_open = connect_to_channel
-        connection = socket.connect(blocking=False)
-        
-        connection.wait() # blocking, raises exception on failure
-        ```
-        
-        Reconnect on disconnection
-        ```python
-        socket.on_close = lambda socket: socket.connect()
-        ```
-        
-        Subscribe to events
-        ```python
-        def do_something(payload):
-          thing = payload["thing"]
-        
-        channel.on("eventname", do_something)
-        ```
-        
-        Push data to a channel
-        ```python
-        channel.push("eventname", {"some": "data"})
-        ```
-        
-        Push data and wait for a response
-        ```python
-        message = channel.push("eventname", {"some": "data"}, reply=True)
-        response = message.wait_for_response() # blocking
-        ```
-        
-        Push data and react to the response with a callback
-        ```python
-        def respond(payload):
-          print(payload)
-        
-        channel.push("eventname", {"some": "data"}, respond)
-        ```
-        
-        Leave a channel
-        ```python
-        channel.leave()
-        ```
-        
-        Disconnect
-        ```python
-        socket.close()
-        ```
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# phxsocket
+### Synchronous phoenix websocket client using callbacks
+[Phoenix channels](https://hexdocs.pm/phoenix/channels.html)
+## Requirements
+`websockets`
+
+## Usage
+Import the package
+```python
+import phxsocket
+```
+
+Create socket client
+```python
+socket = phxsocket.Client("wss://target.url/channel/websocket", {"options": "something"})
+```
+
+Connect and join a channel
+```python
+if socket.connect(): # blocking, raises exception on failure
+  channel = socket.channel("room:roomname", {"more options": "something else"})
+  resp = channel.join() # also blocking, raises exception on failure
+```
+
+Alternatively
+```python
+def connect_to_channel(socket):
+  channel = socket.channel("room:roomname", {"more options": "something else"})
+  resp = channel.join()
+  
+socket.on_open = connect_to_channel
+connection = socket.connect(blocking=False)
+
+connection.wait() # blocking, raises exception on failure
+```
+
+Reconnect on disconnection
+```python
+socket.on_close = lambda socket: socket.connect()
+```
+
+Subscribe to events
+```python
+def do_something(payload):
+  thing = payload["thing"]
+
+channel.on("eventname", do_something)
+```
+
+Push data to a channel
+```python
+channel.push("eventname", {"some": "data"})
+```
+
+Push data and wait for a response
+```python
+message = channel.push("eventname", {"some": "data"}, reply=True)
+response = message.wait_for_response() # blocking
+```
+
+Push data and react to the response with a callback
+```python
+def respond(payload):
+  print(payload)
+
+channel.push("eventname", {"some": "data"}, respond)
+```
+
+Leave a channel
+```python
+channel.leave()
+```
+
+Disconnect
+```python
+socket.close()
+```
+
+
```

### Comparing `phxsocket-0.1.2/setup.py` & `phxsocket-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
   long_description = fh.read()
 
 with open("requirements.txt") as fh:
   install_requires = fh.read()
 
 setup(
   name="phxsocket",
-  version="0.1.2",
+  version="0.1.3",
   author="wwwwwwww",
   author_email="wvvwvvvvwvvw@gmail.com",
   description="Websocket client for Phoenix Elixir",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/wwww-wwww/phxsocket",
   install_requires=install_requires,
   packages=find_packages(),
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
   ],
-  python_requires=">=3.7",
+  python_requires=">=3.10",
 )
```

