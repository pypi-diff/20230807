# Comparing `tmp/fyers_sdk-2.1.5.tar.gz` & `tmp/fyers_sdk-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-2.1.5.tar", last modified: Fri Aug  4 14:07:50 2023, max compression
+gzip compressed data, was "fyers_sdk-2.1.6.tar", last modified: Mon Aug  7 07:00:32 2023, max compression
```

## Comparing `fyers_sdk-2.1.5.tar` & `fyers_sdk-2.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-04 14:07:50.501531 fyers_sdk-2.1.5/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.1.5/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-04 14:07:50.501531 fyers_sdk-2.1.5/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.1.5/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-04 14:07:50.473531 fyers_sdk-2.1.5/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-04 14:07:50.501531 fyers_sdk-2.1.5/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.1.5/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    61782 2023-08-04 13:39:41.000000 fyers_sdk-2.1.5/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1140 2023-08-01 06:21:10.000000 fyers_sdk-2.1.5/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     9833 2023-08-02 11:15:05.000000 fyers_sdk-2.1.5/fyers_sdk/FyersWebsocket/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15350 2023-08-04 05:44:36.000000 fyers_sdk-2.1.5/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.1.5/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27346 2023-08-04 10:33:40.000000 fyers_sdk-2.1.5/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.1.5/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-04 14:07:50.497532 fyers_sdk-2.1.5/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-04 14:07:50.000000 fyers_sdk-2.1.5/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-04 14:07:50.000000 fyers_sdk-2.1.5/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-04 14:07:50.000000 fyers_sdk-2.1.5/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-08-04 14:07:50.000000 fyers_sdk-2.1.5/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-04 14:07:50.000000 fyers_sdk-2.1.5/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-04 14:07:50.501531 fyers_sdk-2.1.5/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1031 2023-08-04 14:07:33.000000 fyers_sdk-2.1.5/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-07 07:00:32.074876 fyers_sdk-2.1.6/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.1.6/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-07 07:00:32.074876 fyers_sdk-2.1.6/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.1.6/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-07 07:00:32.038876 fyers_sdk-2.1.6/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-07 07:00:32.074876 fyers_sdk-2.1.6/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.1.6/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    63507 2023-08-07 06:59:04.000000 fyers_sdk-2.1.6/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1140 2023-08-01 06:21:10.000000 fyers_sdk-2.1.6/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     9833 2023-08-02 11:15:05.000000 fyers_sdk-2.1.6/fyers_sdk/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15350 2023-08-04 05:44:36.000000 fyers_sdk-2.1.6/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.1.6/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27374 2023-08-07 04:47:57.000000 fyers_sdk-2.1.6/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.1.6/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-07 07:00:32.062876 fyers_sdk-2.1.6/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-07 07:00:31.000000 fyers_sdk-2.1.6/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-07 07:00:31.000000 fyers_sdk-2.1.6/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-07 07:00:31.000000 fyers_sdk-2.1.6/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-08-07 07:00:31.000000 fyers_sdk-2.1.6/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-07 07:00:31.000000 fyers_sdk-2.1.6/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-07 07:00:32.078876 fyers_sdk-2.1.6/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1031 2023-08-07 06:57:21.000000 fyers_sdk-2.1.6/setup.py
```

### Comparing `fyers_sdk-2.1.5/LICENSE.txt` & `fyers_sdk-2.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.5/PKG-INFO` & `fyers_sdk-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 2.1.5
+Version: 2.1.6
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.1.5/README.md` & `fyers_sdk-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.5/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-2.1.6/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files 4% similar despite different names*

```diff
@@ -921,50 +921,53 @@
                         response[val] = data_resp[val]
             else:
                 if data_type == "depth":
 
                     for i, val in enumerate(self.depthvalue):
                         if val in data_resp and i < 10:
                             response[val] = data_resp[val] / (
-                                10 ** data_resp["precision"] * data_resp["multiplier"])
+                                10 ** data_resp["precision"] ) * data_resp["multiplier"]
 
                         elif val in data_resp:
                             response[val] = data_resp[val]
                 elif data_type == "scrips":
                     for i, val in enumerate(self.data_val):
                         if val in data_resp and val in precision_calcu_value and val not in ["upper_ckt", "lower_ckt"]:
                             response[val] = data_resp[val] / (
-                                10 ** (data_resp["precision"] * data_resp["multiplier"])
+                                (10 ** data_resp["precision"] )* data_resp["multiplier"]
                             )
                             # response[val] = data_resp[val] / (
 
                         elif val in data_resp:
                             response[val] = data_resp[val]
-                    if "prev_close_price" in response and "ltp" in response:
+
+                    response["lower_ckt"] = 0
+                    response["upper_ckt"] = 0
+                    if "prev_close_price" in response and "ltp" in response and response["prev_close_price"] != 0:
                         response["ch"] = round((response['ltp']  - response['prev_close_price']),2) 
                         response["chp"] = round((response["ch"]  / response['prev_close_price'] * 100) , 2)
                     if "OI" in response:
                         response.pop("OI")
                     if "Yhigh" in response:
                         response.pop("Yhigh")
                     if "Ylow" in response:
                         response.pop("Ylow")
                 else:
                     for i, val in enumerate(self.index_val):
                         if val in data_resp and i in [0, 1, 3, 4, 5]:
                             response[val] = data_resp[val] / (
-                                10 ** (data_resp["precision"] * data_resp["multiplier"])
+                                (10 ** data_resp["precision"] ) * data_resp["multiplier"]
                             )
                         elif val in data_resp:
                             response[val] = data_resp[val]
                         if "prev_close_price" in response and "ltp" in response:
                             response["ch"] = round((response['ltp']  - response['prev_close_price']),2) 
                             response["chp"] = round((response["ch"]  / response['prev_close_price'] * 100) , 2)
-            response["lower_ckt"] = 0
-            response["upper_ckt"] = 0
+                        response["lower_ckt"] = 0
+                        response["upper_ckt"] = 0
             
             self.On_message(response)
 
         except Exception as e:
             self.data_logger.exception(e)
 
     def __datafeed_resp(self, data: bytearray):
@@ -1009,19 +1012,21 @@
 
                         self.resp[self.dp_sym[topic_id]] = {}
 
                         field_count = struct.unpack("B", data[offset : offset + 1])[0]
                         offset += 1
 
                         for index in range(field_count):
-                            value = struct.unpack(">I", data[offset : offset + 4])[0]
+                            value = struct.unpack(">i", data[offset : offset + 4])[0]
                             offset += 4
-                            self.resp[self.dp_sym[topic_id]][
-                                self.depthvalue[index]
-                            ] = value
+
+                            if value != -2147483648:
+                                self.resp[self.dp_sym[topic_id]][
+                                    self.depthvalue[index]
+                                ] = value
 
                         offset += 2
 
                         multiplier = struct.unpack(">H", data[offset : offset + 2])[0]
                         self.resp[self.dp_sym[topic_id]]["multiplier"] = multiplier
                         offset += 2
                         precision = struct.unpack("B", data[offset : offset + 1])[0]
@@ -1051,20 +1056,22 @@
                         self.resp[self.index_sym[topic_id]] = {}
 
                         # field_count - 21 in scrips , 25 in depth , 6 in index
                         field_count = struct.unpack("B", data[offset : offset + 1])[0]
                         offset += 1
 
                         for index in range(field_count):
-                            value = struct.unpack(">I", data[offset : offset + 4])[0]
+
+                            value = struct.unpack(">i", data[offset : offset + 4])[0]
                             offset += 4
-                            print(struct.unpack(">I", data[offset : offset + 4]))
-                            self.resp[self.index_sym[topic_id]][
-                                self.index_val[index]
-                            ] = value
+
+                            if value != -2147483648:
+                                self.resp[self.index_sym[topic_id]][
+                                    self.index_val[index]
+                                ] = value
 
                         offset += 2
 
                         multiplier = struct.unpack(">H", data[offset : offset + 2])[0]
                         self.resp[self.index_sym[topic_id]]["multiplier"] = multiplier
                         offset += 2
 
@@ -1094,27 +1101,26 @@
                         self.resp[self.scrips_sym[topic_id]] = {}
 
                         # field_count - 21 in scrips , 25 in depth , 6 in index
                         field_count = struct.unpack("B", data[offset : offset + 1])[0]
                         offset += 1
 
                         for index in range(field_count):
-                            value = struct.unpack(">I", data[offset : offset + 4])[0]
+                            value = struct.unpack(">i", data[offset : offset + 4])[0]
                             offset += 4
-                            self.resp[self.scrips_sym[topic_id]][
-                                self.data_val[index]
-                            ] = value
+                            if value != -2147483648:
+                                self.resp[self.scrips_sym[topic_id]][
+                                    self.data_val[index]
+                                ] = value
 
                         offset += 2
 
                         multiplier = struct.unpack(">H", data[offset : offset + 2])[0]
                         self.resp[self.scrips_sym[topic_id]]["multiplier"] = multiplier
                         offset += 2
-                        print("multiplier : ", multiplier)
-
 
                         precision = struct.unpack("B", data[offset : offset + 1])[0]
                         self.resp[self.scrips_sym[topic_id]]["precision"] = precision
                         offset += 1
                         val = ["exchange", "exchange_token", "symbol"]
                         for i in range(3):
                             string_len = struct.unpack("B", data[offset : offset + 1])[
@@ -1138,42 +1144,56 @@
                     offset += 2
 
                     field_count = struct.unpack("B", data[offset : offset + 1])[0]
                     offset += 1
                     sf_flag, idx_flag, dp_flag = False, False, False
                     self.UpdateTick = False
                     for index in range(field_count):
-                        value = struct.unpack(">I", data[offset : offset + 4])[0]
+                        value = struct.unpack(">i", data[offset : offset + 4])[0]
                         offset += 4
                         # if field_count == 20 or field_count == 21:
                         if topic_id in self.scrips_sym:
-                            if self.resp[self.scrips_sym[topic_id]][
-                                self.data_val[index]] != value and value != "2147483648":
+                            if self.data_val[index] in self.resp[self.scrips_sym[topic_id]] and self.resp[self.scrips_sym[topic_id]][
+                                self.data_val[index]] != value and value != -2147483648:
                                 self.resp[self.scrips_sym[topic_id]][
                                     self.data_val[index]
                                 ] = value
                                 self.UpdateTick = True
+                            elif value != -2147483648:
+                                self.resp[self.scrips_sym[topic_id]][
+                                    self.data_val[index]
+                                ] = value
+                                self.UpdateTick = True
+
                             sf_flag = True
                         elif topic_id in self.index_sym:
-                            if self.resp[self.index_sym[topic_id]][
-                                self.index_val[index]] != value:
+                            if self.index_val[index] in self.resp[self.index_sym[topic_id]] and  self.resp[self.index_sym[topic_id]][self.index_val[index]] != value and value != "-2147483648":
 
                                 self.resp[self.index_sym[topic_id]][
                                     self.index_val[index]
                                 ] = value
                                 self.UpdateTick = True
+                            elif value != -2147483648:
+                                self.resp[self.index_sym[topic_id]][
+                                    self.index_val[index]
+                                ] = value
+                                self.UpdateTick = True
                             idx_flag = True
                         elif topic_id in self.dp_sym:
-                            if self.resp[self.dp_sym[topic_id]][
-                                self.depthvalue[index]] != value:
+                            if self.depthvalue[index] in self.resp[self.dp_sym[topic_id]] and self.resp[self.dp_sym[topic_id]][
+                                self.depthvalue[index]] != value and value != "-2147483648":
                                 self.resp[self.dp_sym[topic_id]][
                                     self.depthvalue[index]
                                 ] = value
                                 self.UpdateTick = True
-
+                            elif value != -2147483648:
+                                self.resp[self.dp_sym[topic_id]][
+                                    self.depthvalue[index]
+                                ] = value
+                                self.UpdateTick = True                                
                             dp_flag = True
                     if self.UpdateTick:
                         if sf_flag:
                             self.__response_output(
                                 self.resp[self.scrips_sym[topic_id]], "scrips"
                             )
                         elif idx_flag:
@@ -1190,33 +1210,41 @@
                     offset += 1
                     topic_id = struct.unpack("H", data[offset : offset + 2])[0]
                     offset += 2
                     sf_flag, idx_flag = False, False
                     if topic_id in self.scrips_sym:
 
                         # for index in range(3):
-                        value = struct.unpack(">I", data[offset : offset + 4])[0]
+                        value = struct.unpack(">i", data[offset : offset + 4])[0]
                         offset += 4
+                        if value != self.resp[self.scrips_sym[topic_id]][self.data_val[0]] and value != 2147483648:
+                            self.resp[self.scrips_sym[topic_id]][self.data_val[0]] = value
+                            sf_flag = True
 
-                        self.resp[self.scrips_sym[topic_id]][self.data_val[0]] = value
-                        sf_flag = True
-
+                            self.__response_output(
+                                self.resp[self.scrips_sym[topic_id]], "scrips"
+                            )
                     elif topic_id in self.index_sym:
                         value = struct.unpack(">I", data[offset : offset + 4])[0]
                         offset += 4
-                        self.resp[self.index_sym[topic_id]][self.index_val[0]] = value
-                        idx_flag = True
-                    if sf_flag:
-                        self.__response_output(
-                            self.resp[self.scrips_sym[topic_id]], "scrips"
-                        )
-                    elif idx_flag:
-                        self.__response_output(
-                            self.resp[self.index_sym[topic_id]], "index"
-                        )
+                        if value != self.resp[self.index_sym[topic_id]][self.index_val[0]] and value != 2147483648:
+                            self.resp[self.index_sym[topic_id]][self.index_val[0]] = value
+                            idx_flag = True
+                            self.__response_output(
+                                self.resp[self.index_sym[topic_id]], "index"
+                            )
+                        
+                    # if sf_flag:
+                    #     self.__response_output(
+                    #         self.resp[self.scrips_sym[topic_id]], "scrips"
+                    #     )
+                    # elif idx_flag:
+                    #     self.__response_output(
+                    #         self.resp[self.index_sym[topic_id]], "index"
+                    #     )
 
         except Exception as e:
             self.data_logger.exception(e)
 
 
     def __response_msg(self, data: bytearray):
         """
@@ -1404,20 +1432,19 @@
             if self.write_to_file:
                 self.data_logger.debug(f"ERROR Response:{message}")
             else:
                 print(f"Response: {message}")
 
     def on_open(self) -> None:
         """
-        Performs initialization and waits before executing further actions.
+        Handles the open action.
         """
-        if self.__ws_object is None:
-            self.__init_connection()
-            time.sleep(2)
-
+        # if self.__ws_object is None:
+        #     self.__init_connection()
+        #     time.sleep(2)
         if self.OnOpen:
             self.OnOpen()
 
 
     def connect(self) -> None:
         """
         Establishes a connection to the WebSocket.
@@ -1525,31 +1552,30 @@
         """
         Initializes the WebSocket connection and starts the WebSocketApp.
 
         The method creates a WebSocketApp object with the specified URL and sets the appropriate event handlers.
         It then starts the WebSocketApp in a separate thread.
         """
         try:
-            if self.__ws_object is None:
-                if self.access_token_to_hsmtoken():
-                    if self.write_to_file:
-                        self.background_flag = True
-
-                    ws = websocket.WebSocketApp(
-                        self.__url,
-                        on_message=lambda ws, msg: self.__response_msg(msg),
-                        on_error=lambda ws, msg: self.On_error(msg),
-                        on_close=lambda ws, close_code, close_reason: self.__on_close(
-                            ws, close_code, close_reason
-                        ),
-                        on_open=lambda ws: self.__on_open(ws),
-                    )
-                    self.ws_thread = Thread(target=ws.run_forever)
-                    self.ws_thread.daemon = self.background_flag
-                    self.ws_thread.start()
+            if self.access_token_to_hsmtoken():
+                if self.write_to_file:
+                    self.background_flag = True
+
+                ws = websocket.WebSocketApp(
+                    self.__url,
+                    on_message=lambda ws, msg: self.__response_msg(msg),
+                    on_error=lambda ws, msg: self.On_error(msg),
+                    on_close=lambda ws, close_code, close_reason: self.__on_close(
+                        ws, close_code, close_reason
+                    ),
+                    on_open=lambda ws: self.__on_open(ws),
+                )
+                self.ws_thread = Thread(target=ws.run_forever)
+                self.ws_thread.daemon = self.background_flag
+                self.ws_thread.start()
 
         except Exception as e:
             self.data_logger.exception(e)
 
     def close_connection(self) -> None:
         """
         Closes the WebSocket connection 
@@ -1640,15 +1666,14 @@
 
         Args:
             symbols (list): A list of symbols to subscribe to.
             data_type (str, optional): The type of data to subscribe to. Defaults to "SymbolUpdate".
             channel (int, optional): The channel to use for subscription. Defaults to 1.
         """
         try:
-            # self.__init_connection()
             time.sleep(2)
             self.data_type = data_type
             self.symbols = symbols
             self.channel_num = channel
             self.__channel_resume_pause()
             self.channel_symbol = self.__symbol_conversion(symbols)
             if self.channel_symbol is None:
@@ -1667,11 +1692,12 @@
             total_symbols = len(self.scrips_count[self.channel_num])
             symbol_chunks = [
                 self.scrips_count[self.channel_num][i : i + 100]
                 for i in range(0, total_symbols, 100)
             ]
             for symbols in symbol_chunks:
                 message = self.__subscription_msg(symbols)
+
                 self.message.append(message)
 
         except Exception as e:
             self.data_logger.exception(e)
```

### Comparing `fyers_sdk-2.1.5/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-2.1.6/fyers_sdk/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.5/fyers_sdk/FyersWebsocket/map.json` & `fyers_sdk-2.1.6/fyers_sdk/FyersWebsocket/map.json`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.5/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-2.1.6/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.5/fyers_sdk/fyersModel.py` & `fyers_sdk-2.1.6/fyers_sdk/fyersModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,15 @@
         """
         try:
             response = requests.patch(
                 url=Config.API + api,
                 data=json.dumps(data),
                 headers={"Authorization": header, "Content-Type": self.content ,"version": "3"},
             )
+            print(response)
             return response.json()
         except Exception as e:
             self.api_logger.error(e)
 
 
 class FyersServiceAsync:
     def __init__(self, logger):
```

### Comparing `fyers_sdk-2.1.5/fyers_sdk/fyers_logger.py` & `fyers_sdk-2.1.6/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.5/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-2.1.6/fyers_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 2.1.5
+Version: 2.1.6
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.1.5/setup.py` & `fyers_sdk-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='2.1.5',
+     version='2.1.6',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
```

