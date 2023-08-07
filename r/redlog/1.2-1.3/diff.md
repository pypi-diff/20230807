# Comparing `tmp/redlog-1.2-py3-none-any.whl.zip` & `tmp/redlog-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 11131 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1066 b- defN 23-Mar-04 11:23 LICENCE
--rw-r--r--  2.0 unx      544 b- defN 23-Mar-04 11:23 README.md
--rw-r--r--  2.0 unx     6086 b- defN 23-Mar-04 11:23 test.py
--rw-r--r--  2.0 unx    10614 b- defN 23-Mar-04 11:23 redlog/__init__.py
--rwxr-xr-x  2.0 unx     4043 b- defN 23-Mar-04 11:23 redlog/__main__.py
--rw-r--r--  2.0 unx      836 b- defN 23-Mar-04 11:24 redlog.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      221 b- defN 23-Mar-04 11:24 redlog.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-04 11:24 redlog.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Mar-04 11:24 redlog.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-04 11:24 redlog.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1066 b- defN 23-Mar-04 11:24 redlog-1.2.dist-info/LICENCE
--rw-r--r--  2.0 unx      882 b- defN 23-Mar-04 11:24 redlog-1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-04 11:24 redlog-1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-04 11:24 redlog-1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1132 b- defN 23-Mar-04 11:24 redlog-1.2.dist-info/RECORD
-15 files, 26601 bytes uncompressed, 9275 bytes compressed:  65.1%
+Zip file size: 10928 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     1066 b- defN 23-Aug-07 12:32 LICENCE
+-rw-r--r--  2.0 unx      544 b- defN 23-Aug-07 12:32 README.md
+-rw-r--r--  2.0 unx     5823 b- defN 23-Aug-07 12:32 test.py
+-rw-r--r--  2.0 unx    10202 b- defN 23-Aug-07 12:32 redlog/__init__.py
+-rwxr-xr-x  2.0 unx     4044 b- defN 23-Aug-07 12:32 redlog/__main__.py
+-rw-r--r--  2.0 unx      836 b- defN 23-Aug-07 12:33 redlog.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      221 b- defN 23-Aug-07 12:33 redlog.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 12:33 redlog.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Aug-07 12:33 redlog.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 12:33 redlog.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1066 b- defN 23-Aug-07 12:33 redlog-1.3.dist-info/LICENCE
+-rw-r--r--  2.0 unx      882 b- defN 23-Aug-07 12:33 redlog-1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 12:33 redlog-1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 12:33 redlog-1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1132 b- defN 23-Aug-07 12:33 redlog-1.3.dist-info/RECORD
+15 files, 25927 bytes uncompressed, 9072 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: redlog.egg-info/requires.txt
 Comment: 
 
 Filename: redlog.egg-info/top_level.txt
 Comment: 
 
-Filename: redlog-1.2.dist-info/LICENCE
+Filename: redlog-1.3.dist-info/LICENCE
 Comment: 
 
-Filename: redlog-1.2.dist-info/METADATA
+Filename: redlog-1.3.dist-info/METADATA
 Comment: 
 
-Filename: redlog-1.2.dist-info/WHEEL
+Filename: redlog-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: redlog-1.2.dist-info/top_level.txt
+Filename: redlog-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: redlog-1.2.dist-info/RECORD
+Filename: redlog-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## test.py

```diff
@@ -21,38 +21,38 @@
         log = Log(DB_HOST, DB_PORT, db=DB_INDEX, retention_time=1)
         # push
         test_messages = ["Yeah!", "", "qwerty"]
         for msg in test_messages:
             log.info(msg)
         # pop and compare
         msg = None
-        for msg in log.read_day():
+        for msg in log.fetch():
             now = time.time()
             self.assertTrue(now - 1 < msg.timestamp <= now)
             self.assertEqual(msg.tag, Tag.INFO)
             self.assertEqual(msg.content, test_messages.pop(0))
             self.assertTrue(msg.is_last)
             self.assertIsNone(msg.pred)
         self.assertIsNotNone(msg)   # to make sure we ever enter the loop
         # expiration
         time.sleep(1.1)
-        for _ in log.read_day():
+        for _ in log.fetch():
             self.fail("Some messages are not expired in the log")
 
     def test_chaining(self):
         """ Log message updating """
         self.db.flushdb()
         log = Log(DB_HOST, DB_PORT, db=DB_INDEX)
         # push
         msg = log.info("info")
         msg.warning("warn")
         log.info("another info!")
         msg.error("error")
         # check
-        messages = list(log.read_day())
+        messages = list(log.fetch())
         self.assertEqual(len(messages), 4)
         # - content
         self.assertEqual(messages[0].content, "info")
         self.assertEqual(messages[1].content, "warn")
         self.assertEqual(messages[2].content, "another info!")
         self.assertEqual(messages[3].content, "error")
         # - tag
@@ -80,86 +80,82 @@
         """ Log message updating across dates """
         self.db.flushdb()
         log = Log(DB_HOST, DB_PORT, db=DB_INDEX)
         # push
         msg = log.info("info")
         # cheat: change the date to past
         self.assertTrue(hasattr(msg, 'key'))
-        newkey, _ = Thread._get_key(time.time() - 1234567)
+        now = time.time()
+        newkey, _ = Thread._get_key(now - 1234567)
         self.db.rename(msg.key, newkey)
         msg.key = newkey
         # push more
+        time.sleep(0.001)
         msg.info("another info!")
         log.warning("warn")
         msg.error("error")
         # check
-        messages = list(log.read_day())
+        messages = list(log.fetch(now, now + 123))
         self.assertEqual(len(messages), 3)
         # - predecessors
-        self.assertIsNone(messages[0].pred.pred)
-        self.assertIsNotNone(messages[0].pred)
+        self.assertTrue(messages[0].pred)
         self.assertIsNone(messages[1].pred)
         self.assertEqual(messages[2].pred, messages[0])
         # - content
-        self.assertEqual(messages[0].pred.content, "info")
         self.assertEqual(messages[0].content, "another info!")
         self.assertEqual(messages[1].content, "warn")
         self.assertEqual(messages[2].content, "error")
         # - tag
-        self.assertEqual(messages[0].pred.tag, Tag.INFO)
         self.assertEqual(messages[0].tag, Tag.INFO)
         self.assertEqual(messages[1].tag, Tag.WARNING)
         self.assertEqual(messages[2].tag, Tag.ERROR)
         # - update number
-        self.assertEqual(messages[0].pred.update_number, 0)
         self.assertEqual(messages[0].update_number, 1)
         self.assertEqual(messages[1].update_number, 0)
         self.assertEqual(messages[2].update_number, 2)
         # - is last
-        self.assertFalse(messages[0].pred.is_last)
         self.assertFalse(messages[0].is_last)
         self.assertTrue(messages[1].is_last)
         self.assertTrue(messages[2].is_last)
 
     def test_flushed_logs_before_update(self):
         """ Flushing logs before updating a message """
         # push
         self.db.flushdb()
         log = Log(DB_HOST, DB_PORT, db=DB_INDEX)
         msg = log.info("info")
         self.db.flushdb()
         msg.info("new info")
         # check
-        for n, msg in enumerate(log.read_day()):
+        for n, msg in enumerate(log.fetch()):
             self.assertEqual(n, 0)
             self.assertIsNone(msg.pred)
             self.assertEqual(msg.content, "new info")
             self.assertEqual(msg.tag, Tag.INFO)
             self.assertEqual(msg.update_number, 0)
             self.assertTrue(msg.is_last)
 
     def test_long_thread(self):
         """ Making a long thread of messages """
         self.db.flushdb()
         log = Log(DB_HOST, DB_PORT, db=DB_INDEX)
         thread = log.info("start")
         for i in range(12345):
             thread.info(f"message #{i}")
-        messages = list(log.read(0, time.time()))
+        messages = list(log.fetch(0, time.time()))
         self.assertEqual(len(messages), 12345 + 1)
 
     def test_range_filter(self):
         """ Picking messages in a given time range """
         self.db.flushdb()
         log = Log(DB_HOST, DB_PORT, db=DB_INDEX)
         # push
         log.error("First message").debug("Thread to the first message")
         start_time = time.time()
         time.sleep(0.01)
         log.warning("Second message")
         # check
-        rng = (start_time, time.time())
-        messages = list(log.read_day(0, rng))
+        messages = list(log.fetch(start_time, time.time()))
         self.assertEqual(len(messages), 1)
         self.assertEqual(messages[0].content, "Second message")
         self.assertEqual(messages[0].tag, Tag.WARNING)
         self.assertIsNone(messages[0].pred)
```

## redlog/__init__.py

```diff
@@ -201,74 +201,68 @@
 
     def report_exception(self, message: str, exception: Exception, tag: Tag=None) -> Thread:
         return self.__call__(
             tag or Tag.CRITICAL,
             f'{message}: {exception}\n' + '\n'.join(traceback.format_tb(exception.__traceback__))
         )
 
-    def read_day(self, date: Union[str, int] = 0, time_range: Optional[Tuple[float, float]] = None) -> Generator[Message, None, None]:
-        """ Retrieves all messages at a single given day. Optionally filters by a given time range.
-                date: date in `DATE_FORMAT` format, or integer (0=today, 1=yesterday, etc.)
-                time_range: absolute timestamp range (two-tuple) to pick messages in; can be none
+    def fetch(self, from_ts: Optional[float] = None, to_ts: Optional[float] = None) -> Generator[Message, None, None]:
+        """ Retrieves messages between two given timestamps.
         """
-        # get key in string format
-        if isinstance(date, int):
-            ts = time.time() - date * SECONDS_PER_DAY
-            date = datetime.utcfromtimestamp(ts).strftime(DATE_FORMAT)
-        midnight = datetime.strptime(date, DATE_FORMAT).timestamp()
+        if from_ts is None and to_ts is not None:
+            marks = range(math.floor(from_ts), math.floor(to_ts) + 1, SECONDS_PER_DAY)
+            dates = map(lambda t: datetime.utcfromtimestamp(t).strftime(DATE_FORMAT), marks)
+        else:
+            dates = sorted(map(bytes.decode, self.db.keys()))
 
-        # loop raw messages
         daily_cache = {}   # index => message for messages having predecessors
-        raw_messages = self.db.lrange(date, 0, -1)
-        for idx, raw in enumerate(raw_messages):
-            # parse message
-            message = Message(raw, midnight)
-
-            # check if within the time_range
-            if time_range:
-                if message.timestamp < time_range[0]:
+
+        # loop dates
+        for date in dates:
+            midnight = datetime.strptime(date, DATE_FORMAT).timestamp()
+
+            # loop raw messages
+            raw_messages = self.db.lrange(date, 0, -1)
+            for idx, raw in enumerate(raw_messages):
+                # parse message
+                message = Message(raw, midnight)
+
+                # check if within the time_range
+                if from_ts is not None and message.timestamp < from_ts:
                     continue
-                if time_range[1] <= message.timestamp:
+                if to_ts is not None and to_ts <= message.timestamp:
                     break
 
-            # resolve the thread
-            thread = message
-            while thread is not None and thread.pred is not None:
-                pred_date, pred_idx = thread.pred
-
-                # check for the preceding message in the cache
-                if pred_date == date and pred_idx in daily_cache:
-                    thread.pred = daily_cache.pop(pred_idx)
-                    break
-                else:
-                    # not found in the cache; get from the DB
-                    pred_db_record = self.db.lrange(pred_date, pred_idx, pred_idx)
-
-                    # create the preceding message if `pred_db_record` exists (may disappear due to its TTL)
-                    thread.pred = Message(
-                        pred_db_record[0],
-                        datetime.strptime(pred_date, DATE_FORMAT).timestamp(),
-                    ) if pred_db_record else None
-
-                    # check if within the time_range
-                    if time_range and thread.pred.timestamp < time_range[0]:
-                        # if out of bounds, mark the predecessor as existing one but do not keep
-                        thread.pred = True
+                # resolve the thread
+                thread = message
+                while thread is not None and thread.pred is not None:
+                    pred_date, pred_idx = thread.pred
+
+                    # check for the preceding message in the cache
+                    if pred_idx in daily_cache:
+                        thread.pred = daily_cache.pop(pred_idx)
                         break
+                    else:
+                        # not found in the cache; get from the DB
+                        pred_db_record = self.db.lrange(pred_date, pred_idx, pred_idx)
+
+                        # create the preceding message if `pred_db_record` exists (may disappear due to its TTL)
+                        thread.pred = Message(
+                            pred_db_record[0],
+                            datetime.strptime(pred_date, DATE_FORMAT).timestamp()
+                        ) if pred_db_record else None
+
+                        # check if within the time_range
+                        if from_ts is not None and thread.pred.timestamp < from_ts:
+                            # if out of bounds, mark the predecessor as existing one but do not keep
+                            thread.pred = True
+                            break
+
+                    # loop
+                    thread = thread.pred
+
+                # put to cache if the current message precedes another one
+                if not message.is_last:
+                    daily_cache[idx] = message
 
-                # loop
-                thread = thread.pred
-
-            # put to cache if the current message preceeds another one
-            if not message.is_last:
-                daily_cache[idx] = message
-
-            yield message
-
-    def read(self, from_ts: float, to_ts: float) -> Generator[Message, None, None]:
-        """ Retrieves messages between two given timestamps.
-        """
-        marks = range(math.floor(from_ts), math.floor(to_ts) + 1, SECONDS_PER_DAY)
-        dates = map(lambda t: datetime.utcfromtimestamp(t).strftime(DATE_FORMAT), marks)
-        for day in dates:
-            for message in self.read_day(day, (from_ts, to_ts)):
                 yield message
+
```

## redlog/__main__.py

```diff
@@ -64,15 +64,15 @@
             raise ValueError(f"Cannot interpret time range: {args.last}")
 
     # instantiate the database connection
     log = redlog.Log(host=args.host, port=args.port, db=args.db)
     threads = []
 
     # loop the messages
-    for message in log.read(*time_range):
+    for message in log.fetch(*time_range):
         millisec = (message.timestamp % 1) * 1000
         time_mark = datetime.fromtimestamp(message.timestamp).strftime(args.time_format) + ".%03d" % (millisec)
 
         prefix = ""
         indent = "\n" + " " * (len(time_mark) + 1)
         stroke = False
         for i, msg in enumerate(threads):
```

## redlog.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redlog
-Version: 1.2
+Version: 1.3
 Summary: Python logger to Redis database with threading support
 Home-page: https://github.com/lnstadrum/redlog
 Author: lnstadrum
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `redlog-1.2.dist-info/LICENCE` & `redlog-1.3.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `redlog-1.2.dist-info/METADATA` & `redlog-1.3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redlog
-Version: 1.2
+Version: 1.3
 Summary: Python logger to Redis database with threading support
 Home-page: https://github.com/lnstadrum/redlog
 Author: lnstadrum
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `redlog-1.2.dist-info/RECORD` & `redlog-1.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENCE,sha256=FHBeqzNhoBKNclRLw_EUEWrAGGoUKp_-j2sQ5fsJ2uw,1066
 README.md,sha256=auqpQzwFKF0u7UWg2DI8s4XjKnJRHCyunKgPl5rhGlI,544
-test.py,sha256=mYNWLrEchdQX5Nzm0e1orCYPsj2UscaefZfchCLVz-Q,6086
-redlog/__init__.py,sha256=N3H12YVhoJAai-sJdiQiGAn8XzW4znDwQPr4eXGD9Sc,10614
-redlog/__main__.py,sha256=BxRa-Ckc3dzrpu617qbLyioN54YvFveK0PwfPPfDvwc,4043
-redlog.egg-info/PKG-INFO,sha256=LEw6_XyJDq8tk263bZV5EJkwXd0yY51Kc9FDv-pSz_A,836
+test.py,sha256=f6XHAcXZrqYcIsYVMiwagO0uhvIXj0HLogP26MGSbQs,5823
+redlog/__init__.py,sha256=5Bo2sWaQOP8TqRRTTTT8VtQwBkFE_BvLwoYfpVAjg8M,10202
+redlog/__main__.py,sha256=m7NMOsbWFMEcfP8WDdAv6cmbxWF79zyRWjXJKTH8rYQ,4044
+redlog.egg-info/PKG-INFO,sha256=8EhSMgB4H2XZPicKwrWn0EaKaYMZvum_sZ5u56DAJt4,836
 redlog.egg-info/SOURCES.txt,sha256=OZSrHua32CABstt6mXpL4xd7OnyC0_buKNXz_GiZeoU,221
 redlog.egg-info/dependency_links.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 redlog.egg-info/requires.txt,sha256=zvPRrr65sUJqZwdA2PC64piJMhKcZUFGdQ8jAnVfIt8,16
 redlog.egg-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-redlog-1.2.dist-info/LICENCE,sha256=FHBeqzNhoBKNclRLw_EUEWrAGGoUKp_-j2sQ5fsJ2uw,1066
-redlog-1.2.dist-info/METADATA,sha256=4_CtU8AkjVyhBEEOMN1oGGu7vHXUNqcP8Vf0-1aVZ8M,882
-redlog-1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-redlog-1.2.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-redlog-1.2.dist-info/RECORD,,
+redlog-1.3.dist-info/LICENCE,sha256=FHBeqzNhoBKNclRLw_EUEWrAGGoUKp_-j2sQ5fsJ2uw,1066
+redlog-1.3.dist-info/METADATA,sha256=dpPhv5_u33zU_3o42dKWj2jbk9Uv0OSjheCX49X1npQ,882
+redlog-1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+redlog-1.3.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+redlog-1.3.dist-info/RECORD,,
```

