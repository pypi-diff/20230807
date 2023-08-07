# Comparing `tmp/CheeseAPI-0.0.5.tar.gz` & `tmp/CheeseAPI-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheeseAPI-0.0.5.tar", last modified: Wed Aug  2 15:37:54 2023, max compression
+gzip compressed data, was "CheeseAPI-0.0.6.tar", last modified: Mon Aug  7 02:21:39 2023, max compression
```

## Comparing `CheeseAPI-0.0.5.tar` & `CheeseAPI-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 15:37:54.390228 CheeseAPI-0.0.5/
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 15:37:54.387680 CheeseAPI-0.0.5/CheeseAPI/
--rw-r--r--   0 cheese     (501) staff       (20)      255 2023-08-01 09:51:10.000000 CheeseAPI-0.0.5/CheeseAPI/__init__.py
--rw-r--r--   0 cheese     (501) staff       (20)    16971 2023-08-02 15:14:07.000000 CheeseAPI-0.0.5/CheeseAPI/app.py
--rw-r--r--   0 cheese     (501) staff       (20)     1636 2023-08-01 09:45:24.000000 CheeseAPI-0.0.5/CheeseAPI/cSignal.py
--rw-r--r--   0 cheese     (501) staff       (20)     8370 2023-08-02 15:37:10.000000 CheeseAPI-0.0.5/CheeseAPI/command.py
--rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.5/CheeseAPI/exception.py
--rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.5/CheeseAPI/file.py
--rw-r--r--   0 cheese     (501) staff       (20)     2287 2023-08-01 09:12:11.000000 CheeseAPI-0.0.5/CheeseAPI/module.py
--rw-r--r--   0 cheese     (501) staff       (20)     3675 2023-08-01 08:04:57.000000 CheeseAPI-0.0.5/CheeseAPI/request.py
--rw-r--r--   0 cheese     (501) staff       (20)    12440 2023-08-01 08:05:03.000000 CheeseAPI-0.0.5/CheeseAPI/response.py
--rw-r--r--   0 cheese     (501) staff       (20)     4317 2023-08-01 06:17:09.000000 CheeseAPI-0.0.5/CheeseAPI/route.py
--rw-r--r--   0 cheese     (501) staff       (20)     3709 2023-08-02 09:26:09.000000 CheeseAPI-0.0.5/CheeseAPI/server.py
--rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.5/CheeseAPI/system.py
--rw-r--r--   0 cheese     (501) staff       (20)     1345 2023-08-01 07:01:25.000000 CheeseAPI-0.0.5/CheeseAPI/websocket.py
--rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.5/CheeseAPI/workspace.py
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-02 15:37:54.389349 CheeseAPI-0.0.5/CheeseAPI.egg-info/
--rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)      516 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/SOURCES.txt
--rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/dependency_links.txt
--rw-r--r--   0 cheese     (501) staff       (20)       56 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/entry_points.txt
--rw-r--r--   0 cheese     (501) staff       (20)       57 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/requires.txt
--rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-02 15:37:54.000000 CheeseAPI-0.0.5/CheeseAPI.egg-info/top_level.txt
--rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.5/LICENSE
--rw-r--r--   0 cheese     (501) staff       (20)     7909 2023-08-02 15:37:54.389937 CheeseAPI-0.0.5/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)     7458 2023-08-02 01:58:40.000000 CheeseAPI-0.0.5/README.md
--rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-02 15:37:54.390357 CheeseAPI-0.0.5/setup.cfg
--rw-r--r--   0 cheese     (501) staff       (20)      984 2023-08-02 15:37:32.000000 CheeseAPI-0.0.5/setup.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-07 02:21:39.410232 CheeseAPI-0.0.6/
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-07 02:21:39.409062 CheeseAPI-0.0.6/CheeseAPI/
+-rw-r--r--   0 cheese     (501) staff       (20)      263 2023-08-07 02:05:19.000000 CheeseAPI-0.0.6/CheeseAPI/__init__.py
+-rw-r--r--   0 cheese     (501) staff       (20)    16870 2023-08-07 02:05:09.000000 CheeseAPI-0.0.6/CheeseAPI/app.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1636 2023-08-01 09:45:24.000000 CheeseAPI-0.0.6/CheeseAPI/cSignal.py
+-rw-r--r--   0 cheese     (501) staff       (20)     8402 2023-08-03 06:20:30.000000 CheeseAPI-0.0.6/CheeseAPI/command.py
+-rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.6/CheeseAPI/exception.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.6/CheeseAPI/file.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2287 2023-08-01 09:12:11.000000 CheeseAPI-0.0.6/CheeseAPI/module.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3332 2023-08-03 08:02:48.000000 CheeseAPI-0.0.6/CheeseAPI/request.py
+-rw-r--r--   0 cheese     (501) staff       (20)    12440 2023-08-01 08:05:03.000000 CheeseAPI-0.0.6/CheeseAPI/response.py
+-rw-r--r--   0 cheese     (501) staff       (20)     4317 2023-08-01 06:17:09.000000 CheeseAPI-0.0.6/CheeseAPI/route.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3709 2023-08-02 09:26:09.000000 CheeseAPI-0.0.6/CheeseAPI/server.py
+-rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.6/CheeseAPI/system.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1345 2023-08-01 07:01:25.000000 CheeseAPI-0.0.6/CheeseAPI/websocket.py
+-rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.6/CheeseAPI/workspace.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-07 02:21:39.409841 CheeseAPI-0.0.6/CheeseAPI.egg-info/
+-rw-r--r--   0 cheese     (501) staff       (20)     7964 2023-08-07 02:21:39.000000 CheeseAPI-0.0.6/CheeseAPI.egg-info/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)      516 2023-08-07 02:21:39.000000 CheeseAPI-0.0.6/CheeseAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-07 02:21:39.000000 CheeseAPI-0.0.6/CheeseAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       56 2023-08-07 02:21:39.000000 CheeseAPI-0.0.6/CheeseAPI.egg-info/entry_points.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       57 2023-08-07 02:21:39.000000 CheeseAPI-0.0.6/CheeseAPI.egg-info/requires.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-07 02:21:39.000000 CheeseAPI-0.0.6/CheeseAPI.egg-info/top_level.txt
+-rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.6/LICENSE
+-rw-r--r--   0 cheese     (501) staff       (20)     7964 2023-08-07 02:21:39.410025 CheeseAPI-0.0.6/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)     7513 2023-08-03 09:30:51.000000 CheeseAPI-0.0.6/README.md
+-rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-07 02:21:39.410278 CheeseAPI-0.0.6/setup.cfg
+-rw-r--r--   0 cheese     (501) staff       (20)      984 2023-08-07 02:20:03.000000 CheeseAPI-0.0.6/setup.py
```

### Comparing `CheeseAPI-0.0.5/CheeseAPI/app.py` & `CheeseAPI-0.0.6/CheeseAPI/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,25 @@
 from .request import Request
 from .response import Response, BaseResponse, FileResponse
 from .file import File
 from .websocket import websocket
 from .module import LocalModule, Module
 from .cSignal import signal
 
+async def doFunc(func: Callable, kwargs: Dict[str, Any] = {}):
+    _kwargs = {}
+    sig = inspect.signature(func)
+    for key, value in kwargs.items():
+        if key in sig.parameters or 'kwargs' in sig.parameters:
+            _kwargs[key] = value
+    if inspect.iscoroutinefunction(func):
+        return await func(**_kwargs)
+    else:
+        return func(**_kwargs)
+
 class App:
     def __init__(self):
         self.startTimer: float = time.time()
 
         from .system import System
         from .workspace import Workspace
         from .server import Server
@@ -124,62 +135,62 @@
                     # 404
                     requestFunc, kwargs = matchPath(request.path)
                     kwargs['request'] = request
                     if not isinstance(requestFunc, dict):
                         if signal.receiver('http_response404Handle'):
                             await signal.send_async('http_response404Handle', kwargs)
                         for http_response404Handle in self.http_response404Handles:
-                            _response = await self.doFunc(http_response404Handle, kwargs)
+                            _response = await doFunc(http_response404Handle, kwargs)
                             if isinstance(_response, BaseResponse):
                                 response = _response
                         if not isinstance(response, BaseResponse):
                             response = Response(status = 404)
 
                     # 405
                     elif request.method not in requestFunc:
                         if signal.receiver('http_response405Handle'):
                             await signal.send_async('http_response405Handle', kwargs)
                         for http_response405Handle in self.http_response405Handles:
-                            _response = await self.doFunc(http_response405Handle, kwargs)
+                            _response = await doFunc(http_response405Handle, kwargs)
                             if isinstance(_response, BaseResponse):
                                 response = _response
                         if not isinstance(response, BaseResponse):
                             response = Response(status = 405)
 
                     # Other...
                     else:
                         if signal.receiver('http_beforeRequestHandle'):
                             await signal.send_async('http_beforeRequestHandle', kwargs)
                         for http_beforeRequestHandle in self.http_beforeRequestHandles:
-                            _response = await self.doFunc(http_beforeRequestHandle, kwargs)
+                            _response = await doFunc(http_beforeRequestHandle, kwargs)
                             if isinstance(_response, BaseResponse):
                                 response = _response
 
                         if not isinstance(response, BaseResponse):
                             requestFunc = requestFunc[request.method]
-                            response = await self.doFunc(requestFunc, kwargs)
+                            response = await doFunc(requestFunc, kwargs)
 
                         if isinstance(response, BaseResponse):
                             if signal.receiver('http_afterResponseHandle'):
                                 await signal.send_async('http_afterResponseHandle', kwargs)
                             for http_afterResponseHandle in self.http_afterResponseHandles:
                                 kwargs['response'] = response
-                                _response = await self.doFunc(http_afterResponseHandle, kwargs)
+                                _response = await doFunc(http_afterResponseHandle, kwargs)
                                 if isinstance(_response, BaseResponse):
                                     response = _response
                         else:
                             CheeseLog.danger(f'The error occured while accessing the {request.method} {request.fullPath}\nTraceback (most recent call last):\n  File "{inspect.getsourcefile(requestFunc)}", line {inspect.getsourcelines(requestFunc)[1]}, in <module>\n    Function {requestFunc.__name__} needs to return Response, not {response.__class__.__name__}')
                             response = Response(status = 500)
             except Exception as e:
                 CheeseLog.danger(f'The error occured while accessing the {request.method} {request.fullPath}\n{traceback.format_exc()}'[:-1], f'The error occured while accessing the \033[36m{request.method} {request.fullPath}\033[0m\n{traceback.format_exc()}'[:-1])
                 if signal.receiver('http_response500Handle'):
                     await signal.send_async('http_response500Handle', kwargs)
                 for http_response500Handle in self.http_response500Handles:
                     kwargs['exception'] = e
-                    _response = await self.doFunc(http_response500Handle, kwargs)
+                    _response = await doFunc(http_response500Handle, kwargs)
                     if isinstance(_response, BaseResponse):
                         response = _response
                 if not isinstance(response, BaseResponse):
                     response = Response(status = 500)
 
             headers = []
             for key, value in response.headers.items():
@@ -232,22 +243,22 @@
         if scope['type'] in [ 'websocket', 'websockets' ]:
             try:
                 request = Request(scope)
                 requestFunc, kwargs = matchPath(request.path)
                 kwargs['request'] = request
                 if requestFunc is None or 'WEBSOCKET' not in requestFunc:
                     for websocket_notFoundHandle in self.websocket_notFoundHandles:
-                        await self.doFunc(websocket_notFoundHandle, kwargs)
+                        await doFunc(websocket_notFoundHandle, kwargs)
                     return
                 requestFunc = requestFunc['WEBSOCKET']
 
                 if signal.receiver('websocket_beforeConnectionHandle'):
                     await signal.send_async('websocket_beforeConnectionHandle', kwargs)
                 for websocket_beforeConnectionHandle in self.websocket_beforeConnectionHandles:
-                    await self.doFunc(websocket_beforeConnectionHandle, kwargs)
+                    await doFunc(websocket_beforeConnectionHandle, kwargs)
 
                 await send({
                     'type': 'websocket.accept'
                 })
 
                 if (await receive())['type'] == 'websocket.connect':
                     CheeseLog.websocket(f'{request.ip} connected {request.path}', f'{request.ip} connected \033[36m{request.path}\033[0m')
@@ -264,42 +275,31 @@
                     while True:
                         message = await receive()
                         if message['type'] == 'websocket.receive':
                             if 'text' in message:
                                 kwargs['value'] = message['text']
                             elif 'bytes' in message:
                                 kwargs['value'] = message['bytes']
-                            await self.doFunc(requestFunc, kwargs)
+                            await doFunc(requestFunc, kwargs)
                         elif message['type'] == 'websocket.disconnect':
                             del websocket._CLIENTS[request.sid]
                             task.cancel()
                             await task
                             CheeseLog.websocket(f'{request.ip} disconnected {request.path}', f'{request.ip} disconnected \033[36m{request.path}\033[0m')
                             break
 
                 if signal.receiver('websocket_afterDisconnectHandle'):
                     await signal.send_async('websocket_afterDisconnectHandle', kwargs)
                 for websocket_afterDisconnectHandle in self.websocket_afterDisconnectHandles:
-                    await self.doFunc(websocket_afterDisconnectHandle, kwargs)
+                    await doFunc(websocket_afterDisconnectHandle, kwargs)
             except Exception as e:
                 CheeseLog.danger(f'The error occured while accessing the WEBSOCKET {request.fullPath}\n{traceback.format_exc()}'[:-1], f'The error occured while accessing the \033[36mWEBSOCKET {request.fullPath}\033[0m\n{traceback.format_exc()}'[:-1])
                 for websocket_errorHandle in self.websocket_errorHandles:
                     kwargs['exception'] = e
-                    await self.doFunc(websocket_errorHandle, kwargs)
-
-    async def doFunc(self, func: Callable, kwargs: Dict[str, Any] = {}):
-        _kwargs = {}
-        sig = inspect.signature(func)
-        for key, value in kwargs.items():
-            if key in sig.parameters or 'kwargs' in sig.parameters:
-                _kwargs[key] = value
-        if inspect.iscoroutinefunction(func):
-            return await func(**_kwargs)
-        else:
-            return func(**_kwargs)
+                    await doFunc(websocket_errorHandle, kwargs)
 
     def server_startingHandle(self, func: Callable):
         self.server_startingHandles.append(func)
 
     def server_endingHandle(self, func: Callable):
         self.server_endingHandles.append(func)
```

### Comparing `CheeseAPI-0.0.5/CheeseAPI/cSignal.py` & `CheeseAPI-0.0.6/CheeseAPI/cSignal.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.5/CheeseAPI/command.py` & `CheeseAPI-0.0.6/CheeseAPI/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 static path: \033[34m{app.server.STATIC_PATH}\033[0m''' if app.server.STATIC_PATH is not False else '') + (f'''
 current log file path: \033[4;36m.{app.logger.filePath[len(app.workspace.BASE_PATH):]}\033[0m''' if app.server.LOG_FILENAME is not False else ''))
 
     CheeseLog.starting(f'The server running on http://{app.server.HOST}:{app.server.PORT}', f'The server running on \033[4;36mhttp://{app.server.HOST}:{app.server.PORT}\033[0m')
 
     import sys
     sys.path.append(os.getcwd())
-    app = __import__(_app.split(':')[0]).app
+    app = eval(f'__import__(\'{_app.split(":")[0]}\').{_app.split(":")[1]}')
 
     _modules = set()
     if len(app.modules):
         CheeseLog.starting(f'Modules:\n{" | ".join(app.modules)}')
     for module in app.modules:
         _modules.add(Module(_modules, module))
     app.modules = _modules
```

### Comparing `CheeseAPI-0.0.5/CheeseAPI/file.py` & `CheeseAPI-0.0.6/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.5/CheeseAPI/module.py` & `CheeseAPI-0.0.6/CheeseAPI/module.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.5/CheeseAPI/request.py` & `CheeseAPI-0.0.6/CheeseAPI/request.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,86 +12,60 @@
         self._values: Dict[str, str] = {}
 
     def get(self, key: str, default: T = None) -> str | File | T:
         if key not in self._values:
             return default
         return self._values[key]
 
-class Args(BaseItem):
-    def __init__(self, query: str):
-        super().__init__()
-
-        for q in query.split('&'):
-            q = q.split('=')
-            self._values[q[0]] = q[1] if len(q) > 1 else None
-
-class Form(BaseItem):
-    @overload
-    def __init__(self):
-        ...
-
-    @overload
-    def __init__(self, body: str):
-        ...
-
-    @overload
-    def __init__(self, body: bytes, spliter: bytes):
-        ...
-
-    def __init__(self, body: str | bytes | None = None, spliter: bytes | None = None):
-        super().__init__()
-
-        if body and not spliter:
-            for s in body.split('&'):
-                s = s.split('=')
-                self._values[s[0]] = s[1]
-
-        elif body and spliter:
-            body = body[2:-4].split(spliter)[1:-1]
-            for s in body:
-                key = re.findall(rb'\bname="(.*?)"', s)[0].decode()
-                value = s.split(b'\r\n\r\n')[1][:-4]
-                filename = re.findall(rb'\bfilename="(.*?)"', s)
-                if len(filename):
-                    self._values[key] = File(filename[0].decode(), value)
-                else:
-                    self._values[key] = value.decode()
-
 class Request:
     def __init__(self, scope, body: bytes | None = None):
         query_string = scope['query_string'].decode()
 
         self.ip: CheeseType.network.IPv4 = scope['client'][0]
         self.path: str = scope['path']
         self.fullPath: str = self.path + '?' + query_string if query_string else self.path
         self.scheme = scope['scheme']
 
         self.headers: Dict[str, str] = {}
 
         if scope['type'] in [ 'http', 'https' ]:
             self.method: str = scope['method']
-            self.args = Args(query_string)
+            self.args: Dict[str, str] = {}
+            for q in query_string.split('&'):
+                q = q.split('=')
+                self.args[q[0]] = q[1] if len(q) > 1 else None
             self.body = None
-            self.form: Form = Form()
+            self.form: Dict[str, str] = {}
             for header in scope['headers']:
                 key = header[0].decode()
                 value = header[1].decode()
                 self.headers[key] = value
                 if key == 'content-type':
                     try:
                         if value in [ 'application/json', 'application/javascript' ]:
                             self.body = json.loads(body)
                         elif value == 'application/xml':
                             self.body = xmltodict.parse(body)
                         elif value in [ 'text/plain', 'text/html' ]:
                             self.body = body.decode()
                         elif value.startswith('multipart/form-data;'):
-                            self.form = Form(body, header[1].split(b'boundary=')[1].split(b';')[0])
+                            spliter = header[1].split(b'boundary=')[1].split(b';')[0]
+                            body = body[2:-4].split(spliter)[1:-1]
+                            for s in body:
+                                key = re.findall(rb'\bname="(.*?)"', s)[0].decode()
+                                value = s.split(b'\r\n\r\n')[1][:-4]
+                                filename = re.findall(rb'\bfilename="(.*?)"', s)
+                                if len(filename):
+                                    self.form[key] = File(filename[0].decode(), value)
+                                else:
+                                    self.form[key] = value.decode()
                         elif value == 'application/x-www-form-urlencoded':
-                            self.form = Form(body.decode())
+                            for s in body.decode().split('&'):
+                                s = s.split('=')
+                                self.form[s[0]] = s[1]
                     except:
                         CheeseLog.danger(f'{self.method} {self.fullPath} cannot parse request.body correctly:\n{traceback.format_exc()}'[:-1], f'\033[36m{self.method} {self.fullPath}\033[0m cannot parse request.body correctly:\n{traceback.format_exc()}'[:-1])
         else:
             for header in scope['headers']:
                 key = header[0].decode()
                 value = header[1].decode()
                 self.headers[key] = value
```

### Comparing `CheeseAPI-0.0.5/CheeseAPI/response.py` & `CheeseAPI-0.0.6/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.5/CheeseAPI/route.py` & `CheeseAPI-0.0.6/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.5/CheeseAPI/server.py` & `CheeseAPI-0.0.6/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.5/CheeseAPI/system.py` & `CheeseAPI-0.0.6/CheeseAPI/system.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.5/CheeseAPI/websocket.py` & `CheeseAPI-0.0.6/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.5/CheeseAPI.egg-info/PKG-INFO` & `CheeseAPI-0.0.6/CheeseAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.5
+Version: 0.0.6
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **CheeseAPI**
 
-请注意，该文档是最新的beta版，如果你想要查看最新的发布版内容，请查看最新的tag。
+目前项目仍处于开发阶段，无法保证稳定性。
+
+该文档是最新的beta版，如果你想要查看最新的发布版内容，请查看最新的tag。
 
 ## **介绍**
 
 一款基于uvicorn的web协程框架，目前仍处于开发阶段，一些基础功能已经可以使用。
 
 目前仅保证支持python3.11。
 
@@ -213,15 +215,15 @@
 
 route = Route('/User', app.route)
 
 @route.post('/register')
 def register(request: Request):
     nickname = request.form.get('nickname')
     password = request.form.get('password')
-    gender = Gender(request.form.get('gender', 2))
+    gender = Gender(int(request.form.get('gender', 2)))
     service.register(nickname, password, gender)
     return Response('注册成功！')
 
 @route.post('/login')
 def login(request: Request):
     nickname = request.form.get('nickname')
     password = request.form.get('password')
```

### Comparing `CheeseAPI-0.0.5/CheeseAPI.egg-info/SOURCES.txt` & `CheeseAPI-0.0.6/CheeseAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.5/LICENSE` & `CheeseAPI-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.5/PKG-INFO` & `CheeseAPI-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.5
+Version: 0.0.6
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **CheeseAPI**
 
-请注意，该文档是最新的beta版，如果你想要查看最新的发布版内容，请查看最新的tag。
+目前项目仍处于开发阶段，无法保证稳定性。
+
+该文档是最新的beta版，如果你想要查看最新的发布版内容，请查看最新的tag。
 
 ## **介绍**
 
 一款基于uvicorn的web协程框架，目前仍处于开发阶段，一些基础功能已经可以使用。
 
 目前仅保证支持python3.11。
 
@@ -213,15 +215,15 @@
 
 route = Route('/User', app.route)
 
 @route.post('/register')
 def register(request: Request):
     nickname = request.form.get('nickname')
     password = request.form.get('password')
-    gender = Gender(request.form.get('gender', 2))
+    gender = Gender(int(request.form.get('gender', 2)))
     service.register(nickname, password, gender)
     return Response('注册成功！')
 
 @route.post('/login')
 def login(request: Request):
     nickname = request.form.get('nickname')
     password = request.form.get('password')
```

### Comparing `CheeseAPI-0.0.5/README.md` & `CheeseAPI-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # **CheeseAPI**
 
-请注意，该文档是最新的beta版，如果你想要查看最新的发布版内容，请查看最新的tag。
+目前项目仍处于开发阶段，无法保证稳定性。
+
+该文档是最新的beta版，如果你想要查看最新的发布版内容，请查看最新的tag。
 
 ## **介绍**
 
 一款基于uvicorn的web协程框架，目前仍处于开发阶段，一些基础功能已经可以使用。
 
 目前仅保证支持python3.11。
 
@@ -198,15 +200,15 @@
 
 route = Route('/User', app.route)
 
 @route.post('/register')
 def register(request: Request):
     nickname = request.form.get('nickname')
     password = request.form.get('password')
-    gender = Gender(request.form.get('gender', 2))
+    gender = Gender(int(request.form.get('gender', 2)))
     service.register(nickname, password, gender)
     return Response('注册成功！')
 
 @route.post('/login')
 def login(request: Request):
     nickname = request.form.get('nickname')
     password = request.form.get('password')
```

### Comparing `CheeseAPI-0.0.5/setup.py` & `CheeseAPI-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('./README.md', 'r', encoding = 'utf-8') as f:
     longDescription = f.read()
 
 setuptools.setup(
     name = 'CheeseAPI',
-    version = '0.0.5',
+    version = '0.0.6',
     author = 'Cheese Unknown',
     author_email = 'cheese@cheese.ren',
     description = '一款基于uvicorn的web协程框架',
     long_description = longDescription,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/CheeseUnknown/CheeseAPI',
     license = 'MIT',
```

