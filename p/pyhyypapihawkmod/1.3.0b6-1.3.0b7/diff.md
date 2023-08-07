# Comparing `tmp/pyhyypapihawkmod-1.3.0b6.tar.gz` & `tmp/pyhyypapihawkmod-1.3.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.3.0b6.tar", last modified: Fri Aug  4 08:49:03 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.3.0b7.tar", last modified: Mon Aug  7 11:18:23 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.3.0b6.tar` & `pyhyypapihawkmod-1.3.0b7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 08:49:03.981857 pyhyypapihawkmod-1.3.0b6/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b6/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b6/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-08-04 08:49:03.980848 pyhyypapihawkmod-1.3.0b6/PKG-INFO
--rw-rw-rw-   0        0        0     3348 2023-08-04 08:48:12.000000 pyhyypapihawkmod-1.3.0b6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 08:49:03.878562 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      410 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      162 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0    12602 2023-08-01 16:50:47.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2780 2023-08-01 17:13:20.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2825 2023-08-01 17:14:02.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    32743 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4114 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     1999 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/imei.py
--rw-rw-rw-   0        0        0     7584 2023-08-01 17:13:20.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    19095 2023-08-04 08:46:43.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-08-04 08:49:03.978828 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-08-04 08:49:03.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2023-08-04 08:49:03.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 08:49:03.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-08-04 08:49:03.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-04 08:49:03.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 08:49:03.981857 pyhyypapihawkmod-1.3.0b6/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-08-01 19:51:24.000000 pyhyypapihawkmod-1.3.0b6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:18:23.542315 pyhyypapihawkmod-1.3.0b7/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b7/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b7/MANIFEST.in
+-rw-rw-rw-   0        0        0      422 2023-08-07 11:18:23.541306 pyhyypapihawkmod-1.3.0b7/PKG-INFO
+-rw-rw-rw-   0        0        0     3610 2023-08-07 11:16:30.000000 pyhyypapihawkmod-1.3.0b7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 11:18:23.526107 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      410 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    12602 2023-08-01 16:50:47.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2780 2023-08-01 17:13:20.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2825 2023-08-01 17:14:02.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    32743 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4114 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     1999 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/imei.py
+-rw-rw-rw-   0        0        0     7584 2023-08-01 17:13:20.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    19549 2023-08-07 11:14:55.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:18:23.538270 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      422 2023-08-07 11:18:23.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-08-07 11:18:23.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 11:18:23.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-07 11:18:23.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-07 11:18:23.000000 pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 11:18:23.542315 pyhyypapihawkmod-1.3.0b7/setup.cfg
+-rw-rw-rw-   0        0        0      826 2023-08-07 11:17:06.000000 pyhyypapihawkmod-1.3.0b7/setup.py
```

### Comparing `pyhyypapihawkmod-1.3.0b6/LICENSE.md` & `pyhyypapihawkmod-1.3.0b7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b6/README.md` & `pyhyypapihawkmod-1.3.0b7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -34,18 +34,25 @@
 3. Get site/partition/user/zone info:
 
 ```
 print(json.dumps(client.get_sync_info(),indent=2))
 
 ```
 
+
+Todo:
+- Look into v1 of the FCM API, may have to rewrite the entire push_received system.
+
 Changelog 
 
+1.3.0b7
+- Fixed HeartbeatPing and HeartbeatPingAck packets. Should now provide hearbeat and ack correctly.
+
 1.3.0b6
-- Added 30 min ping (Ping is broken ...)
+- Added 30 min ping (Ping is from initial implementation, to investigate). Currently reconnects
 
 1.3.0b5
 - Added reconnect for timeouts
 
 1.3.0b4
 - Minor Refactoring
```

### Comparing `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/alarm_info.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/imei.py` & `pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/imei.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod/push_receiver.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,15 @@
 REGISTER_URL = "https://android.clients.google.com/c2dm/register3"
 CHECKIN_URL = "https://android.clients.google.com/checkin"
 FCM_SUBSCRIBE = "https://fcm.googleapis.com/fcm/connect/subscribe"
 FCM_ENDPOINT = "https://fcm.googleapis.com/fcm/send"
 GOOGLE_MTALK_ENDPOINT = "mtalk.google.com"
 READ_TIMEOUT_SECS = 60 * 60
 MIN_RESET_INTERVAL_SECS = 60 * 5
-MAX_SILENT_INTERVAL_SECS = 60 * 30
-STATUS_TIMEOUT = 1
+MAX_SILENT_INTERVAL_SECS = 60 * 15
 
 MCS_VERSION = 41
 PACKET_BY_TAG = [
     HeartbeatPing,
     HeartbeatAck,
     LoginRequest,
     LoginResponse,
@@ -250,17 +249,17 @@
     
     def __init__(
         self,
     ) -> None:
         self.fcm_registration = FCMRegistration()
         self.received_persistent_ids = []
         self.time_of_last_reset = 0
-        self.last_stream_id_received = 0
         self.time_of_last_receive = time.time()
         self.current_ping_thread = 0
+        self.awaiting_ack = False 
 
 
     def __read(self, sock, size):
         buf = b""
         while len(buf) < size:
             buf += sock.recv(size - len(buf))
         return buf
@@ -335,15 +334,14 @@
             if version < MCS_VERSION and version != 38:
                 raise RuntimeError("protocol version {} unsupported".format(version))
         else:
             (tag,) = struct.unpack("B", self.__read(data, 1))
         _LOGGER.debug("tag %s (%s)", tag, PACKET_BY_TAG[tag])
         size = self.__read_varint32(data)
         _LOGGER.debug("size %s", size)
-        self.last_stream_id_received += 1
         self.time_of_last_receive = time.time()
         if size >= 0:
             buf = self.__read(data, size)
             _LOGGER.debug(hexlify(buf))
             packet = PACKET_BY_TAG[tag]
             payload = packet()
             payload.ParseFromString(buf)
@@ -387,15 +385,17 @@
         req.user = credentials["gcm"]["androidId"]
         req.use_rmq2 = True
         req.setting.add(name="new_vc", value="1")  # pylint: disable=maybe-no-member
         req.received_persistent_id.extend(persistent_ids)  # pylint: disable=maybe-no-member
         self.__send(google_socket, req)
         login_response = self.__recv(google_socket, first=True)
         _LOGGER.debug("Received login response: %s", login_response)
-        thread.Thread(target=self.__ping_scheduler, args=(google_socket,)).start()
+        thread.Thread(target=self.__ping_scheduler, args=(google_socket,
+                                                          credentials,
+                                                          persistent_ids)).start()
         return google_socket
 
 
     def __reset(self, google_socket, credentials, persistent_ids):
         now = time.time()
         if now - self.time_of_last_reset < MIN_RESET_INTERVAL_SECS:
             raise Exception("Too many connection reset attempts.")
@@ -405,40 +405,71 @@
             google_socket.shutdown(2)
             google_socket.close()
         except OSError as err:
             _LOGGER.debug("Unable to close connection %f", err)
         return self.__login(credentials, persistent_ids)
 
 
-    def __ping_scheduler(self, google_socket):
+    def __ping_scheduler(self, google_socket, credentials, persistent_ids):
         self.current_ping_thread += 1
         if self.current_ping_thread > 10000:
             self.current_ping_thread = 1
         mythread = self.current_ping_thread
         while mythread == self.current_ping_thread:
+            if self.awaiting_ack:
+                self.awaiting_ack = False
+                self.__reset(google_socket=google_socket,
+                                credentials=credentials,
+                                persistent_ids=persistent_ids)
+                break
             if time.time() - self.time_of_last_receive > MAX_SILENT_INTERVAL_SECS:
                 _LOGGER.debug("Sending PING now==========================")
                 self.__send_ping(google_socket=google_socket)
-                time.sleep(60)
             time.sleep(60)
+
         _LOGGER.debug("Closing PING thread : " + str(mythread))
                 
-        
-
+                    
+    def __send_ping(self, google_socket):
+        self.awaiting_ack = True
+        header = bytearray([0, 0])
+        buf = bytes(header)
+        total = 0
+        while total < len(buf):
+            sent = google_socket.send(buf[total:])
+            if sent == 0:
+                raise RuntimeError("socket connection broken")
+            total += sent
+     
+     
+    def __handle_ping(self, google_socket):
+        header = bytearray([0, 2])
+        buf = bytes(header)
+        total = 0
+        while total < len(buf):
+            sent = google_socket.send(buf[total:])
+            if sent == 0:
+                raise RuntimeError("socket connection broken")
+            total += sent
+  
+     
+     
 
     def __listen(self, credentials, callback, persistent_ids, obj):
         google_socket = self.__login(credentials, persistent_ids)
         while True:
             try:
                 data = self.__recv(google_socket)
                 if isinstance(data, DataMessageStanza):
                     msg_id = self.__handle_data_message(data, credentials, callback, obj)
                     persistent_ids.append(msg_id)
                 elif isinstance(data, HeartbeatPing):
-                    self.__handle_ping(google_socket, data)
+                    self.__handle_ping(google_socket)
+                elif isinstance(data, HeartbeatAck):
+                    self.awaiting_ack = False
                 elif data is None or isinstance(data, Close):
                     google_socket = self.__reset(google_socket, credentials, persistent_ids)
                 else:
                     _LOGGER.debug("Unexpected message type %s", type(data))
             except ConnectionResetError:
                 _LOGGER.debug("Connection Reset: Reconnecting")
                 google_socket = self.__login(credentials, persistent_ids)
@@ -473,35 +504,14 @@
             auth_secret=secret,
         )
         _LOGGER.debug("Received data message %s: %s", data.persistent_id, decrypted)
         callback(obj, json.loads(decrypted.decode("utf-8")), data)
         return data.persistent_id
 
 
-    def __send_ping(self, google_socket):
-        req = HeartbeatPing()
-        #req.stream_id = data.stream_id + 1
-        req.last_stream_id_received = self.last_stream_id_received
-        #req.status = data.status
-        self.__send(google_socket, req)
-        
-
-    def __handle_ping(self, google_socket, data):
-        _LOGGER.debug(
-            "Responding to ping: Stream ID: %s, Last: %s, Status: %s",
-            data.stream_id,
-            data.last_stream_id_received,
-            data.status,
-        )
-        req = HeartbeatAck()
-        req.stream_id = data.stream_id + 1
-        req.last_stream_id_received = data.stream_id
-        req.status = data.status
-        self.__send(google_socket, req)
-
 
     def listen(self, credentials, callback, received_persistent_ids=None, obj=None):
         """
         listens for push notifications
 
         credentials: credentials object returned by register()
         callback(obj, notification, data_message): called on notifications
@@ -514,15 +524,15 @@
             received_persistent_ids = []
 
         self.__listen(credentials, callback, received_persistent_ids, obj)
 
 
     def runner(self, callback, credentials = None, persistent_ids = None):
         """sample that registers a token and waits for notifications"""
-        #_LOGGER.setLevel(logging.DEBUG)
+        _LOGGER.setLevel(logging.DEBUG)
         if persistent_ids is None:
             persistent_ids = []
             
         if credentials is None:
             credentials = self.fcm_registration.register(sender_id=int(GCF_SENDER_ID))
             _credentials = {"credentials" : credentials}
             callback(_credentials) #doesn't do anything for now. Using a different method currently
```

### Comparing `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.3.0b7/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b6/setup.py` & `pyhyypapihawkmod-1.3.0b7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.3.0b6",
+    version="1.3.0b7",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
-    long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
+    long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others.",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
     setup_requires=[
         'requests',
         'setuptools'
     ],
     install_requires=[
```

