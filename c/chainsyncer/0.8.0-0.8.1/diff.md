# Comparing `tmp/chainsyncer-0.8.0.tar.gz` & `tmp/chainsyncer-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainsyncer-0.8.0.tar", last modified: Sun Aug  6 13:04:36 2023, max compression
+gzip compressed data, was "chainsyncer-0.8.1.tar", last modified: Sun Aug  6 18:26:59 2023, max compression
```

## Comparing `chainsyncer-0.8.0.tar` & `chainsyncer-0.8.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-06-07 09:45:06.000000 chainsyncer-0.8.0/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-07 09:45:06.000000 chainsyncer-0.8.0/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      695 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      871 2023-06-07 09:45:06.000000 chainsyncer-0.8.0/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2023-06-07 09:45:06.000000 chainsyncer-0.8.0/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.003570 chainsyncer-0.8.0/chainsyncer/
--rw-r--r--   0 lash      (1000) lash      (1000)       31 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.003570 chainsyncer-0.8.0/chainsyncer/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      697 2023-08-06 11:56:37.000000 chainsyncer-0.8.0/chainsyncer/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)       90 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/cli/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      618 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/cli/config.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.003570 chainsyncer-0.8.0/chainsyncer/data/
--rw-r--r--   0 lash      (1000) lash      (1000)      132 2022-05-13 06:47:02.000000 chainsyncer-0.8.0/chainsyncer/data/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.003570 chainsyncer-0.8.0/chainsyncer/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       44 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/data/config/syncer.ini
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/chainsyncer/driver/
--rw-r--r--   0 lash      (1000) lash      (1000)       29 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/driver/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4274 2023-04-22 20:26:06.000000 chainsyncer-0.8.0/chainsyncer/driver/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3071 2023-08-06 13:01:13.000000 chainsyncer-0.8.0/chainsyncer/driver/chain_interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2848 2023-08-06 12:22:53.000000 chainsyncer-0.8.0/chainsyncer/driver/chain_interface_new.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1814 2023-02-26 19:42:52.000000 chainsyncer-0.8.0/chainsyncer/driver/chain_interface_race.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1145 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3582 2023-04-22 20:26:06.000000 chainsyncer-0.8.0/chainsyncer/filter.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/chainsyncer/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     3308 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/runnable/unlock.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1163 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/session.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1424 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/settings.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/chainsyncer/store/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/store/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)    13085 2023-06-07 09:45:06.000000 chainsyncer-0.8.0/chainsyncer/store/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3010 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/store/fs.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1001 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/store/mem.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2070 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/store/rocksdb.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/chainsyncer/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/chainsyncer/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7016 2023-08-06 12:44:01.000000 chainsyncer-0.8.0/chainsyncer/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7544 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/chainsyncer/unittest/store.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.003570 chainsyncer-0.8.0/chainsyncer.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      695 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1079 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      176 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-08-06 13:04:35.000000 chainsyncer-0.8.0/chainsyncer.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       74 2023-08-06 12:57:18.000000 chainsyncer-0.8.0/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      889 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      592 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       35 2021-10-14 03:38:11.000000 chainsyncer-0.8.0/sql_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:04:36.006904 chainsyncer-0.8.0/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     1670 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/tests/test_basic.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1426 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/tests/test_driver.py
--rw-r--r--   0 lash      (1000) lash      (1000)    10649 2022-10-13 07:54:43.000000 chainsyncer-0.8.0/tests/test_filter.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4622 2022-08-13 18:16:03.000000 chainsyncer-0.8.0/tests/test_session.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:26:59.556609 chainsyncer-0.8.1/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-06-07 09:45:06.000000 chainsyncer-0.8.1/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       78 2023-06-07 09:45:06.000000 chainsyncer-0.8.1/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      695 2023-08-06 18:26:59.556609 chainsyncer-0.8.1/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      871 2023-06-07 09:45:06.000000 chainsyncer-0.8.1/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2023-06-07 09:45:06.000000 chainsyncer-0.8.1/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:26:59.553276 chainsyncer-0.8.1/chainsyncer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       31 2022-10-13 07:54:43.000000 chainsyncer-0.8.1/chainsyncer/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:26:59.553276 chainsyncer-0.8.1/chainsyncer/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      697 2023-08-06 11:56:37.000000 chainsyncer-0.8.1/chainsyncer/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       90 2022-08-13 18:16:03.000000 chainsyncer-0.8.1/chainsyncer/cli/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      618 2022-10-13 07:54:43.000000 chainsyncer-0.8.1/chainsyncer/cli/config.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:26:59.553276 chainsyncer-0.8.1/chainsyncer/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)      132 2022-05-13 06:47:02.000000 chainsyncer-0.8.1/chainsyncer/data/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:26:59.553276 chainsyncer-0.8.1/chainsyncer/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       44 2022-08-13 18:16:03.000000 chainsyncer-0.8.1/chainsyncer/data/config/syncer.ini
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:26:59.556609 chainsyncer-0.8.1/chainsyncer/driver/
+-rw-r--r--   0 lash      (1000) lash      (1000)       29 2022-08-13 18:16:03.000000 chainsyncer-0.8.1/chainsyncer/driver/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4370 2023-08-06 17:32:33.000000 chainsyncer-0.8.1/chainsyncer/driver/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3071 2023-08-06 13:01:13.000000 chainsyncer-0.8.1/chainsyncer/driver/chain_interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2848 2023-08-06 12:22:53.000000 chainsyncer-0.8.1/chainsyncer/driver/chain_interface_new.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1814 2023-02-26 19:42:52.000000 chainsyncer-0.8.1/chainsyncer/driver/chain_interface_race.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1145 2022-10-13 07:54:43.000000 chainsyncer-0.8.1/chainsyncer/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3582 2023-08-06 16:02:22.000000 chainsyncer-0.8.1/chainsyncer/filter.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:26:59.556609 chainsyncer-0.8.1/chainsyncer/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3308 2022-10-13 07:54:43.000000 chainsyncer-0.8.1/chainsyncer/runnable/unlock.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1351 2023-08-06 17:43:35.000000 chainsyncer-0.8.1/chainsyncer/session.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1424 2022-10-13 07:54:43.000000 chainsyncer-0.8.1/chainsyncer/settings.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:26:59.556609 chainsyncer-0.8.1/chainsyncer/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-08-13 18:16:03.000000 chainsyncer-0.8.1/chainsyncer/store/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    13085 2023-06-07 09:45:06.000000 chainsyncer-0.8.1/chainsyncer/store/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3010 2022-10-13 07:54:43.000000 chainsyncer-0.8.1/chainsyncer/store/fs.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1001 2022-08-13 18:16:03.000000 chainsyncer-0.8.1/chainsyncer/store/mem.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2070 2022-08-13 18:16:03.000000 chainsyncer-0.8.1/chainsyncer/store/rocksdb.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:26:59.556609 chainsyncer-0.8.1/chainsyncer/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-08-13 18:16:03.000000 chainsyncer-0.8.1/chainsyncer/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7026 2023-08-06 18:25:31.000000 chainsyncer-0.8.1/chainsyncer/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7544 2022-10-13 07:54:43.000000 chainsyncer-0.8.1/chainsyncer/unittest/store.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:26:59.553276 chainsyncer-0.8.1/chainsyncer.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      695 2023-08-06 18:26:59.000000 chainsyncer-0.8.1/chainsyncer.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1079 2023-08-06 18:26:59.000000 chainsyncer-0.8.1/chainsyncer.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 18:26:59.000000 chainsyncer-0.8.1/chainsyncer.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-08-06 18:26:59.000000 chainsyncer-0.8.1/chainsyncer.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      176 2023-08-06 18:26:59.000000 chainsyncer-0.8.1/chainsyncer.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-08-06 18:26:59.000000 chainsyncer-0.8.1/chainsyncer.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       74 2023-08-06 12:57:18.000000 chainsyncer-0.8.1/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      889 2023-08-06 18:26:59.556609 chainsyncer-0.8.1/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      592 2022-08-13 18:16:03.000000 chainsyncer-0.8.1/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       35 2021-10-14 03:38:11.000000 chainsyncer-0.8.1/sql_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:26:59.556609 chainsyncer-0.8.1/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1670 2022-08-13 18:16:03.000000 chainsyncer-0.8.1/tests/test_basic.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1426 2022-08-13 18:16:03.000000 chainsyncer-0.8.1/tests/test_driver.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    10649 2022-10-13 07:54:43.000000 chainsyncer-0.8.1/tests/test_filter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4622 2022-08-13 18:16:03.000000 chainsyncer-0.8.1/tests/test_session.py
```

### Comparing `chainsyncer-0.8.0/LICENSE` & `chainsyncer-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/PKG-INFO` & `chainsyncer-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainsyncer
-Version: 0.8.0
+Version: 0.8.1
 Summary: Generic blockchain syncer driver
 Home-page: https://git.defalsify.org/chainsyncer
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: cryptocurrency
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chainsyncer-0.8.0/WAIVER` & `chainsyncer-0.8.1/WAIVER`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/WAIVER.asc` & `chainsyncer-0.8.1/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/cli/arg.py` & `chainsyncer-0.8.1/chainsyncer/cli/arg.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/cli/config.py` & `chainsyncer-0.8.1/chainsyncer/cli/config.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/driver/base.py` & `chainsyncer-0.8.1/chainsyncer/driver/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         self.post_callback = post_callback
         self.block_callback = block_callback
         self.idle_callback = idle_callback
         self.last_start = 0
         self.clock_id = time.CLOCK_MONOTONIC_RAW
         self.store.connect()
         self.store.start(offset=offset, target=target)
+        self.item = None
         if not SyncDriver.signal_set:
             for sig in SyncDriver.signal_request:
                 signal.signal(sig, self.__sig_terminate)
             SyncDriver.signal_set = True
 
 
     def __sig_terminate(self, sig, frame):
@@ -53,25 +54,26 @@
 
     def terminate(self):
         """Set syncer to terminate as soon as possible.
         """
         logg.info('termination requested!')
         SyncDriver.running_global = False
         self.running = False
+        self.session.stop(self.item)
 
 
-    def run(self, conn, interval=1):
+    def run(self, conn, interval=1, ctx=None):
         while self.running_global:
-            self.session = SyncSession(self.store)
-            item = self.session.start()
-            if item == None:
+            self.session = SyncSession(self.store, ctx=ctx)
+            self.item = self.session.start()
+            if self.item == None:
                 self.running = False
                 self.running_global = False
                 break
-            self.loop(conn, item, interval=interval)
+            self.loop(conn, self.item, interval=interval)
 
 
     def idle(self, interval):
         interval *= NS_DIV
         idle_start = time.clock_gettime_ns(self.clock_id)
         delta = idle_start - self.last_start
         if delta > interval:
```

### Comparing `chainsyncer-0.8.0/chainsyncer/driver/chain_interface.py` & `chainsyncer-0.8.1/chainsyncer/driver/chain_interface.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/driver/chain_interface_new.py` & `chainsyncer-0.8.1/chainsyncer/driver/chain_interface_new.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/driver/chain_interface_race.py` & `chainsyncer-0.8.1/chainsyncer/driver/chain_interface_race.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/error.py` & `chainsyncer-0.8.1/chainsyncer/error.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/filter.py` & `chainsyncer-0.8.1/chainsyncer/filter.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/runnable/unlock.py` & `chainsyncer-0.8.1/chainsyncer/runnable/unlock.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/session.py` & `chainsyncer-0.8.1/chainsyncer/session.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,40 +6,45 @@
 from chainsyncer.error import FilterDone
 
 logg = logging.getLogger(__name__)
 
 
 class SyncSession:
 
-    def __init__(self, session_store):
+    def __init__(self, session_store, ctx=None):
         self.session_store = session_store
         self.started = self.session_store.started
         self.next = self.session_store.next_item
         self.item = None
         self.filters = self.session_store.filters
+        self.ctx = ctx
 
 
     def get(self, k):
         return self.session_store.get(str(k))
    
 
     def start(self, offset=0, target=-1):
         self.session_store.start(offset=offset, target=target)
         self.item = self.session_store.next_item()
         return self.item
 
 
     def stop(self, item):
         self.session_store.stop(item)
+        for fltr in self.filters:
+            stopper = getattr(fltr, 'stop', None)
+            if stopper != None:
+               stopper()
 
 
     def filter(self, conn, block, tx):
         self.session_store.connect()
         for fltr in self.filters:
             logg.debug('executing filter {}'.format(fltr))
             self.item.advance()
-            interrupt = fltr.filter(conn, block, tx)
+            interrupt = fltr.filter(conn, block, tx, ctx=self.ctx)
             if not self.item.release(interrupt=interrupt):
                 break
         self.item.reset()
         self.next()
         self.session_store.disconnect()
```

### Comparing `chainsyncer-0.8.0/chainsyncer/settings.py` & `chainsyncer-0.8.1/chainsyncer/settings.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/store/base.py` & `chainsyncer-0.8.1/chainsyncer/store/base.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/store/fs.py` & `chainsyncer-0.8.1/chainsyncer/store/fs.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/store/mem.py` & `chainsyncer-0.8.1/chainsyncer/store/mem.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/store/rocksdb.py` & `chainsyncer-0.8.1/chainsyncer/store/rocksdb.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer/unittest/base.py` & `chainsyncer-0.8.1/chainsyncer/unittest/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         return self.z
 
 
     def common_name(self):
         return self.name 
 
 
-    def filter(self, conn, block, tx):
+    def filter(self, conn, block, tx, ctx=None):
         r = False
         if self.brk_hard != None:
             r = True
             if self.brk_hard > 0:
                 r = True
             self.brk_hard -= 1
             if r:
```

### Comparing `chainsyncer-0.8.0/chainsyncer/unittest/store.py` & `chainsyncer-0.8.1/chainsyncer/unittest/store.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/chainsyncer.egg-info/PKG-INFO` & `chainsyncer-0.8.1/chainsyncer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainsyncer
-Version: 0.8.0
+Version: 0.8.1
 Summary: Generic blockchain syncer driver
 Home-page: https://git.defalsify.org/chainsyncer
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: cryptocurrency
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chainsyncer-0.8.0/chainsyncer.egg-info/SOURCES.txt` & `chainsyncer-0.8.1/chainsyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/setup.cfg` & `chainsyncer-0.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chainsyncer
-version = 0.8.0
+version = 0.8.1
 description = Generic blockchain syncer driver
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/chainsyncer
 keywords = 
 	cryptocurrency
 classifiers =
```

### Comparing `chainsyncer-0.8.0/setup.py` & `chainsyncer-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/tests/test_basic.py` & `chainsyncer-0.8.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/tests/test_driver.py` & `chainsyncer-0.8.1/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/tests/test_filter.py` & `chainsyncer-0.8.1/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `chainsyncer-0.8.0/tests/test_session.py` & `chainsyncer-0.8.1/tests/test_session.py`

 * *Files identical despite different names*

