# Comparing `tmp/recon_lw-2.0.0.dev5762896093.tar.gz` & `tmp/recon_lw-2.0.0.dev5787337974.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5762896093.tar", last modified: Fri Aug  4 13:42:54 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5787337974.tar", last modified: Mon Aug  7 16:03:58 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5762896093.tar` & `recon_lw-2.0.0.dev5787337974.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-08-04 13:42:27.000000 recon_lw-2.0.0.dev5762896093/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14303 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    35231 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23883 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6405 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    18015 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/recon_lw/recon_oe_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:42:54.000000 recon_lw-2.0.0.dev5762896093/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-08-04 13:42:00.000000 recon_lw-2.0.0.dev5762896093/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 16:03:58.000000 recon_lw-2.0.0.dev5787337974/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-08-07 16:03:58.000000 recon_lw-2.0.0.dev5787337974/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-08-07 16:03:36.000000 recon_lw-2.0.0.dev5787337974/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 16:03:58.000000 recon_lw-2.0.0.dev5787337974/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14303 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35231 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23883 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6405 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/recon_ob_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18419 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/recon_lw/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 16:03:58.000000 recon_lw-2.0.0.dev5787337974/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-08-07 16:03:58.000000 recon_lw-2.0.0.dev5787337974/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-08-07 16:03:58.000000 recon_lw-2.0.0.dev5787337974/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-07 16:03:58.000000 recon_lw-2.0.0.dev5787337974/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-08-07 16:03:58.000000 recon_lw-2.0.0.dev5787337974/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-08-07 16:03:58.000000 recon_lw-2.0.0.dev5787337974/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-07 16:03:58.000000 recon_lw-2.0.0.dev5787337974/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 16:03:58.000000 recon_lw-2.0.0.dev5787337974/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-08-07 16:03:13.000000 recon_lw-2.0.0.dev5787337974/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5787337974/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5787337974/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5787337974/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5787337974/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5787337974/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5787337974/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5787337974/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5787337974/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5787337974/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5787337974/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw/recon_oe_ob.py` & `recon_lw-2.0.0.dev5787337974/recon_lw/recon_oe_ob.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 from recon_lw.EventsSaver import EventsSaver
 from recon_lw import recon_ob_cross_stream
 from recon_lw.TimeCacheMatcher import TimeCacheMatcher
 from th2_data_services.utils.message_utils import message_utils
 from recon_lw.StateSequenceGenerator import StateSequenceGenerator
 
 
-def process_order_states(message_pickle_path, sessions_list, result_events_path, settings):
+def process_order_states(message_pickle_path, sessions_list, result_events_path, settings, data_objects=None):
     events_saver = EventsSaver(result_events_path)
     root_event = events_saver.create_event("recon_lw_oe_ob_order_states_images " + datetime.now().isoformat(), "Microservice")
     events_saver.save_events([root_event])
 
-    if sessions_list is not None and len(sessions_list):
-        sessions_set = set(sessions_list)
-        streams = recon_lw.open_streams(message_pickle_path,
-                               lambda n: n[:n.rfind('_')] in sessions_set)
+    if data_objects:
+        streams = recon_lw.open_streams(None, data_objects=data_objects)
     else:
-        streams = recon_lw.open_streams(message_pickle_path)
+        if sessions_list is not None and len(sessions_list):
+            sessions_set = set(sessions_list)
+            streams = recon_lw.open_streams(message_pickle_path,
+                                lambda n: n[:n.rfind('_')] in sessions_set)
+        else:
+            streams = recon_lw.open_streams(message_pickle_path)
 
     create_event = lambda n, t, ok, b: events_saver.create_event(n, t, ok, b, parentId=root_event["eventId"])
     save_events = lambda ev_batch: events_saver.save_events(ev_batch)
     seq_gen = StateSequenceGenerator(settings["horizon_delay_seconds"],
                                      settings["stream_sequence_timestamp_extract"],
                                      settings["key_ts_new_key_extract"],
                                      oe_er_state_update,
@@ -49,28 +52,28 @@
 
 def oe_er_state_update(er, current_state, create_event, send_events):
     current_state["no_state"] = False
     current_state["last_er"] = er
 
 
 def process_oe_md_comparison(ob_events_path, oe_images_events_path, md_sessions_list, result_events_path,
-                              horizon_delay_seconds, is_book_open):
+                              horizon_delay_seconds, is_book_open, keeper):
     events_saver = EventsSaver(result_events_path)
     root_event = events_saver.create_event("recon_lw_oe_ob_compare" + datetime.now().isoformat(), "Microservice")
     events_saver.save_events([root_event])
     
     def create_event(n, t, ok, b, am=None):
         return events_saver.create_event(n, t, ok, b, parentId=root_event["eventId"], attached_messages=am)
 
     #create_event = lambda n, t, ok, b: events_saver.create_event(n, t, ok, b, parentId=root_event["eventId"])
     save_events = lambda ev_batch: events_saver.save_events(ev_batch)
     processor = TimeCacheMatcher(horizon_delay_seconds,
                                  oe_ob_get_timestamp_key1_key2,
                                  oe_ob_interpret_func,
-                                 {"is_book_open": is_book_open},
+                                 {"is_book_open": is_book_open, "orders_keeper": keeper},
                                  create_event,
                                  save_events)
     
     data_filter = lambda e: e['body'] and e['body'].get("timestamp", -1) != -1
     streams = recon_lw.open_scoped_events_streams(ob_events_path, lambda n: any(s in n for s in md_sessions_list))
     streams2 = recon_lw.open_scoped_events_streams(oe_images_events_path, data_filter=data_filter)
     for elem in streams2:
@@ -86,19 +89,24 @@
         processor.process_objects_batch(buffer_to_process)
 
     processor.flush_all()
     events_saver.flush()
 
 
 def oe_ob_get_timestamp_key1_key2(o, custom_settings):
+    keeper = custom_settings['orders_keeper']
     if o["eventType"] == "OrderBook":
         if "order_id" in o["body"]["operation_params"]:
+            order_id = o["body"]["operation_params"]["order_id"]
+            if order_id and int(order_id) not in keeper:
+                # Exclude orders from unknown users
+                return None, None, None
             str_toe = o["body"]["operation_params"]["str_time_of_event"]
             ts = recon_lw.epoch_nano_str_to_ts(str_toe)
-            return ts, f'{str_toe}.{o["body"]["operation_params"]["order_id"]}.{o["body"]["otv"]}', None
+            return ts, f'{str_toe}.{order_id}.{o["body"]["otv"]}', None
         else:
             return None, None, None
     elif o["eventType"] == "OEMDImage":
         is_book_open = custom_settings["is_book_open"]
         str_toe = o["body"]["operation_params"]["str_time_of_event"]
         ts = recon_lw.epoch_nano_str_to_ts(str_toe)
         if not is_book_open(o["body"]["operation_params"]["instr"],ts):
```

### Comparing `recon_lw-2.0.0.dev5762896093/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5787337974/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/setup.py` & `recon_lw-2.0.0.dev5787337974/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5762896093/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5787337974/test/test_recon_ob.py`

 * *Files identical despite different names*

