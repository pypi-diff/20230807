# Comparing `tmp/pyacaia_async-0.0.6.tar.gz` & `tmp/pyacaia_async-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacaia_async-0.0.6.tar", last modified: Mon Jul 17 05:47:52 2023, max compression
+gzip compressed data, was "pyacaia_async-0.0.7.tar", last modified: Mon Aug  7 11:16:40 2023, max compression
```

## Comparing `pyacaia_async-0.0.6.tar` & `pyacaia_async-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:47:52.834052 pyacaia_async-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-17 05:47:52.834052 pyacaia_async-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:47:52.834052 pyacaia_async-0.0.6/pyacaia_async/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/acaiascale.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/pyacaia_async/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 05:47:52.834052 pyacaia_async-0.0.6/pyacaia_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-17 05:47:52.000000 pyacaia_async-0.0.6/pyacaia_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-17 05:47:52.000000 pyacaia_async-0.0.6/pyacaia_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 05:47:52.000000 pyacaia_async-0.0.6/pyacaia_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 05:47:52.000000 pyacaia_async-0.0.6/pyacaia_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 05:47:52.000000 pyacaia_async-0.0.6/pyacaia_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 05:47:52.834052 pyacaia_async-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-17 05:47:37.000000 pyacaia_async-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:40.113750 pyacaia_async-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 11:16:23.000000 pyacaia_async-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-07 11:16:40.113750 pyacaia_async-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-08-07 11:16:23.000000 pyacaia_async-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:40.113750 pyacaia_async-0.0.7/pyacaia_async/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-07 11:16:23.000000 pyacaia_async-0.0.7/pyacaia_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-08-07 11:16:23.000000 pyacaia_async-0.0.7/pyacaia_async/acaiascale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-07 11:16:23.000000 pyacaia_async-0.0.7/pyacaia_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-08-07 11:16:23.000000 pyacaia_async-0.0.7/pyacaia_async/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-07 11:16:23.000000 pyacaia_async-0.0.7/pyacaia_async/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-08-07 11:16:23.000000 pyacaia_async-0.0.7/pyacaia_async/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:16:40.113750 pyacaia_async-0.0.7/pyacaia_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-07 11:16:40.000000 pyacaia_async-0.0.7/pyacaia_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-07 11:16:40.000000 pyacaia_async-0.0.7/pyacaia_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:16:40.000000 pyacaia_async-0.0.7/pyacaia_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 11:16:40.000000 pyacaia_async-0.0.7/pyacaia_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 11:16:40.000000 pyacaia_async-0.0.7/pyacaia_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 11:16:40.113750 pyacaia_async-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-07 11:16:23.000000 pyacaia_async-0.0.7/setup.py
```

### Comparing `pyacaia_async-0.0.6/LICENSE` & `pyacaia_async-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.6/PKG-INFO` & `pyacaia_async-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacaia_async
-Version: 0.0.6
+Version: 0.0.7
 Summary: An async implementation of PyAcaia
 Home-page: https://github.com/zweckj/pyacaia_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyacaia_async-0.0.6/README.md` & `pyacaia_async-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.6/pyacaia_async/acaiascale.py` & `pyacaia_async-0.0.7/pyacaia_async/acaiascale.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
         self._msg_types = {
             "tare": encode(4, [0]),
             "startTimer": encode(13, [0,0]),
             "stopTimer": encode(13, [0,2]),
             "resetTimer": encode(13, [0,1]),
             "heartbeat": encode(0, [2,0]),
+            "getSettings": encode(6, [0]*16),
             "auth": encodeId(isPyxisStyle=is_new_style_scale),
             "notificationRequest": encodeNotificationRequest(),
         }
 
         if not is_new_style_scale:
             # for old style scales, the default char id is the same as the notify char id
             DEFAULT_CHAR_ID = NOTIFY_CHAR_ID = OLD_STYLE_CHAR_ID
@@ -57,15 +58,15 @@
             self._client = BleakClient(bleDevice)
         elif mac:
             self._client = BleakClient(mac)
         else:
             raise ValueError("Either mac or bleDevice must be specified")
         
         await self.connect(callback)
-        asyncio.create_task(self._send_heartbeats())
+        asyncio.create_task(self._send_heartbeats(interval=HEARTBEAT_INTERVAL if is_new_style_scale else 1, new_style_heartbeat=is_new_style_scale))
         asyncio.create_task(self._process_queue())
         return self
 
     @property
     def msg_types(self) -> dict:
         return self._msg_types
     
@@ -112,16 +113,17 @@
                         self._queue.task_done()
                     return
                 
                 if self._disconnecting and self._queue.empty():
                     return
                 
                 char_id, payload = await self._queue.get()
-                await self._write_msg(char_id, payload)   
+                await self._write_msg(char_id, payload)
                 self._queue.task_done()
+                await asyncio.sleep(0.1)
 
             except asyncio.CancelledError:
                 return
             except Exception as ex:
                 _LOGGER.debug("Error writing to device: %s", ex)
                 return
 
@@ -160,26 +162,38 @@
 
         await self._queue.put((
                 DEFAULT_CHAR_ID,
                 self.msg_types["notificationRequest"]
         ))
 
 
-    async def _send_heartbeats(self, interval:int=HEARTBEAT_INTERVAL) -> None:
+    async def _send_heartbeats(self, interval:int=HEARTBEAT_INTERVAL, new_style_heartbeat:bool=False) -> None:
         """ Task to send heartbeats in the background. """
         while True:
             try:
                 if not self._connected or self._disconnecting:
                     return
                 
                 _LOGGER.debug("Sending heartbeat.")
+                if new_style_heartbeat:
+                    await self._queue.put((
+                        DEFAULT_CHAR_ID, 
+                        self.msg_types["auth"]
+                    ))
+
                 await self._queue.put((
                         DEFAULT_CHAR_ID, 
                         self.msg_types["heartbeat"]
                     ))
+                
+                if new_style_heartbeat:
+                    await self._queue.put((
+                        DEFAULT_CHAR_ID, 
+                        self.msg_types["getSettings"]
+                    ))
                 await asyncio.sleep(interval)
             except asyncio.CancelledError:
                 return
             except Exception as ex:
                 _LOGGER.debug("Error sending heartbeat: %s", ex)
                 return
 
@@ -193,42 +207,41 @@
             self._connected = False
             _LOGGER.debug("Disconnected from Acaia Scale.")
         except Exception as ex:
             _LOGGER.debug("Error disconnecting from device: %s", ex)
 
 
     async def tare(self) -> None:
-        await self.auth()
         await self._queue.put((
                 DEFAULT_CHAR_ID, 
                 self.msg_types["tare"]
             ))
 
 
     async def startStopTimer(self) -> None:
-        await self.auth()
         if not self._timer_running:
+            _LOGGER.debug('Sending "start" message.')
             await self._queue.put((      
                     DEFAULT_CHAR_ID, 
                     self.msg_types["startTimer"]
                 ))
             self._timer_running = True
             if not self._timer_start:
                 self._timer_start = time.time()
         else:
+            _LOGGER.debug('Sending "stop" message.')
             await self._queue.put((
                     DEFAULT_CHAR_ID, 
                     self.msg_types["stopTimer"]
                 ))
             self._timer_running = False
             self._timer_stop = time.time()
 
 
     async def resetTimer(self) -> None:
-        await self.auth()
         await self._queue.put((
                 DEFAULT_CHAR_ID, 
                 self.msg_types["resetTimer"]
             ))
         self._timer_start = None
         self._timer_stop = None
```

### Comparing `pyacaia_async-0.0.6/pyacaia_async/decode.py` & `pyacaia_async-0.0.7/pyacaia_async/decode.py`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.6/pyacaia_async/helpers.py` & `pyacaia_async-0.0.7/pyacaia_async/helpers.py`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.6/pyacaia_async.egg-info/PKG-INFO` & `pyacaia_async-0.0.7/pyacaia_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacaia-async
-Version: 0.0.6
+Version: 0.0.7
 Summary: An async implementation of PyAcaia
 Home-page: https://github.com/zweckj/pyacaia_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyacaia_async-0.0.6/setup.py` & `pyacaia_async-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="pyacaia_async",
-    version="0.0.6",
+    version="0.0.7",
     description="An async implementation of PyAcaia",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pyacaia_async",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

