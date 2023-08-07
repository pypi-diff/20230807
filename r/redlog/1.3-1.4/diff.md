# Comparing `tmp/redlog-1.3-py3-none-any.whl.zip` & `tmp/redlog-1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 10928 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1066 b- defN 23-Aug-07 12:32 LICENCE
--rw-r--r--  2.0 unx      544 b- defN 23-Aug-07 12:32 README.md
--rw-r--r--  2.0 unx     5823 b- defN 23-Aug-07 12:32 test.py
--rw-r--r--  2.0 unx    10202 b- defN 23-Aug-07 12:32 redlog/__init__.py
--rwxr-xr-x  2.0 unx     4044 b- defN 23-Aug-07 12:32 redlog/__main__.py
--rw-r--r--  2.0 unx      836 b- defN 23-Aug-07 12:33 redlog.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      221 b- defN 23-Aug-07 12:33 redlog.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 12:33 redlog.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Aug-07 12:33 redlog.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 12:33 redlog.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1066 b- defN 23-Aug-07 12:33 redlog-1.3.dist-info/LICENCE
--rw-r--r--  2.0 unx      882 b- defN 23-Aug-07 12:33 redlog-1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 12:33 redlog-1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 12:33 redlog-1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1132 b- defN 23-Aug-07 12:33 redlog-1.3.dist-info/RECORD
-15 files, 25927 bytes uncompressed, 9072 bytes compressed:  65.0%
+Zip file size: 10945 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     1066 b- defN 23-Aug-07 14:43 LICENCE
+-rw-r--r--  2.0 unx      544 b- defN 23-Aug-07 14:43 README.md
+-rw-r--r--  2.0 unx     5823 b- defN 23-Aug-07 14:43 test.py
+-rw-r--r--  2.0 unx    10260 b- defN 23-Aug-07 14:43 redlog/__init__.py
+-rwxr-xr-x  2.0 unx     4044 b- defN 23-Aug-07 14:43 redlog/__main__.py
+-rw-r--r--  2.0 unx      836 b- defN 23-Aug-07 14:44 redlog.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      221 b- defN 23-Aug-07 14:44 redlog.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 14:44 redlog.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Aug-07 14:44 redlog.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 14:44 redlog.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1066 b- defN 23-Aug-07 14:44 redlog-1.4.dist-info/LICENCE
+-rw-r--r--  2.0 unx      882 b- defN 23-Aug-07 14:44 redlog-1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 14:44 redlog-1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-07 14:44 redlog-1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1132 b- defN 23-Aug-07 14:44 redlog-1.4.dist-info/RECORD
+15 files, 25985 bytes uncompressed, 9089 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: redlog.egg-info/requires.txt
 Comment: 
 
 Filename: redlog.egg-info/top_level.txt
 Comment: 
 
-Filename: redlog-1.3.dist-info/LICENCE
+Filename: redlog-1.4.dist-info/LICENCE
 Comment: 
 
-Filename: redlog-1.3.dist-info/METADATA
+Filename: redlog-1.4.dist-info/METADATA
 Comment: 
 
-Filename: redlog-1.3.dist-info/WHEEL
+Filename: redlog-1.4.dist-info/WHEEL
 Comment: 
 
-Filename: redlog-1.3.dist-info/top_level.txt
+Filename: redlog-1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: redlog-1.3.dist-info/RECORD
+Filename: redlog-1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## redlog/__init__.py

```diff
@@ -73,15 +73,15 @@
         # increase conter, get new key
         self.upd_ctr += 1
         newkey, delta = Thread._get_key(time.time())
 
         # form the value to store in the DB:
         #   | num updates > 0[31] | has next[1] | ms since midnight[4*8] | prev msg key[48] | prev msg idx[32] | tag[8] | message[...]
         self.value = bytearray((self.upd_ctr * 2).to_bytes(4, 'big')            # num updates and 'has next' bit (=0)
-                                + delta.to_bytes(4, 'big')                      # ms since bidnight
+                                + delta.to_bytes(4, 'big')                      # ms since midnight
                                 + self.key.encode()                             # predecessor key
                                 + self.idx.to_bytes(4, 'big')                   # predecessor index
                                 + tag[0].encode() + message.encode('utf-8'))    # tag + message content
 
         # push to a list
         self.idx = self._push(newkey, bytes(self.value))
         self.key = newkey
@@ -204,21 +204,21 @@
             tag or Tag.CRITICAL,
             f'{message}: {exception}\n' + '\n'.join(traceback.format_tb(exception.__traceback__))
         )
 
     def fetch(self, from_ts: Optional[float] = None, to_ts: Optional[float] = None) -> Generator[Message, None, None]:
         """ Retrieves messages between two given timestamps.
         """
-        if from_ts is None and to_ts is not None:
+        if from_ts is not None and to_ts is not None:
             marks = range(math.floor(from_ts), math.floor(to_ts) + 1, SECONDS_PER_DAY)
             dates = map(lambda t: datetime.utcfromtimestamp(t).strftime(DATE_FORMAT), marks)
         else:
             dates = sorted(map(bytes.decode, self.db.keys()))
 
-        daily_cache = {}   # index => message for messages having predecessors
+        cache = {}   # 'date/index' => message for messages having predecessors
 
         # loop dates
         for date in dates:
             midnight = datetime.strptime(date, DATE_FORMAT).timestamp()
 
             # loop raw messages
             raw_messages = self.db.lrange(date, 0, -1)
@@ -234,16 +234,17 @@
 
                 # resolve the thread
                 thread = message
                 while thread is not None and thread.pred is not None:
                     pred_date, pred_idx = thread.pred
 
                     # check for the preceding message in the cache
-                    if pred_idx in daily_cache:
-                        thread.pred = daily_cache.pop(pred_idx)
+                    cache_key = f"{pred_date}/{pred_idx}"
+                    if cache_key in cache:
+                        thread.pred = cache.pop(cache_key)
                         break
                     else:
                         # not found in the cache; get from the DB
                         pred_db_record = self.db.lrange(pred_date, pred_idx, pred_idx)
 
                         # create the preceding message if `pred_db_record` exists (may disappear due to its TTL)
                         thread.pred = Message(
@@ -258,11 +259,10 @@
                             break
 
                     # loop
                     thread = thread.pred
 
                 # put to cache if the current message precedes another one
                 if not message.is_last:
-                    daily_cache[idx] = message
+                    cache[f"{date}/{idx}"] = message
 
                 yield message
-
```

## redlog.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redlog
-Version: 1.3
+Version: 1.4
 Summary: Python logger to Redis database with threading support
 Home-page: https://github.com/lnstadrum/redlog
 Author: lnstadrum
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `redlog-1.3.dist-info/LICENCE` & `redlog-1.4.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `redlog-1.3.dist-info/METADATA` & `redlog-1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redlog
-Version: 1.3
+Version: 1.4
 Summary: Python logger to Redis database with threading support
 Home-page: https://github.com/lnstadrum/redlog
 Author: lnstadrum
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `redlog-1.3.dist-info/RECORD` & `redlog-1.4.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENCE,sha256=FHBeqzNhoBKNclRLw_EUEWrAGGoUKp_-j2sQ5fsJ2uw,1066
 README.md,sha256=auqpQzwFKF0u7UWg2DI8s4XjKnJRHCyunKgPl5rhGlI,544
 test.py,sha256=f6XHAcXZrqYcIsYVMiwagO0uhvIXj0HLogP26MGSbQs,5823
-redlog/__init__.py,sha256=5Bo2sWaQOP8TqRRTTTT8VtQwBkFE_BvLwoYfpVAjg8M,10202
+redlog/__init__.py,sha256=-m5RJTxjv5SP5VxN6Y7TBw4ufelhG5DdBew5S8nx0i8,10260
 redlog/__main__.py,sha256=m7NMOsbWFMEcfP8WDdAv6cmbxWF79zyRWjXJKTH8rYQ,4044
-redlog.egg-info/PKG-INFO,sha256=8EhSMgB4H2XZPicKwrWn0EaKaYMZvum_sZ5u56DAJt4,836
+redlog.egg-info/PKG-INFO,sha256=tYpSxnj4pYrBD18JBx6P4CCl4JenyUT4jnD9q7h2yzs,836
 redlog.egg-info/SOURCES.txt,sha256=OZSrHua32CABstt6mXpL4xd7OnyC0_buKNXz_GiZeoU,221
 redlog.egg-info/dependency_links.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 redlog.egg-info/requires.txt,sha256=zvPRrr65sUJqZwdA2PC64piJMhKcZUFGdQ8jAnVfIt8,16
 redlog.egg-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-redlog-1.3.dist-info/LICENCE,sha256=FHBeqzNhoBKNclRLw_EUEWrAGGoUKp_-j2sQ5fsJ2uw,1066
-redlog-1.3.dist-info/METADATA,sha256=dpPhv5_u33zU_3o42dKWj2jbk9Uv0OSjheCX49X1npQ,882
-redlog-1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-redlog-1.3.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-redlog-1.3.dist-info/RECORD,,
+redlog-1.4.dist-info/LICENCE,sha256=FHBeqzNhoBKNclRLw_EUEWrAGGoUKp_-j2sQ5fsJ2uw,1066
+redlog-1.4.dist-info/METADATA,sha256=lIp3E5YnwteSJbKwCFuxeUm-hySfAeTSd1PLmdKbO-U,882
+redlog-1.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+redlog-1.4.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+redlog-1.4.dist-info/RECORD,,
```

