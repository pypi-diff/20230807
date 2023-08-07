# Comparing `tmp/kioss-0.2.8.tar.gz` & `tmp/kioss-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.2.8.tar", last modified: Tue Aug  1 13:26:03 2023, max compression
+gzip compressed data, was "kioss-0.2.9.tar", last modified: Tue Aug  1 13:48:29 2023, max compression
```

## Comparing `kioss-0.2.8.tar` & `kioss-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:26:03.347831 kioss-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 13:25:52.000000 kioss-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 13:26:03.347831 kioss-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-01 13:25:52.000000 kioss-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:26:03.347831 kioss-0.2.8/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 13:25:52.000000 kioss-0.2.8/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-08-01 13:25:52.000000 kioss-0.2.8/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-01 13:25:52.000000 kioss-0.2.8/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:26:03.347831 kioss-0.2.8/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 13:26:03.000000 kioss-0.2.8/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 13:26:03.000000 kioss-0.2.8/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:26:03.000000 kioss-0.2.8/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 13:26:03.000000 kioss-0.2.8/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:26:03.347831 kioss-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 13:25:52.000000 kioss-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:26:03.347831 kioss-0.2.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-08-01 13:25:52.000000 kioss-0.2.8/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 13:25:52.000000 kioss-0.2.8/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:48:29.498540 kioss-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 13:48:20.000000 kioss-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 13:48:29.498540 kioss-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-01 13:48:20.000000 kioss-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:48:29.498540 kioss-0.2.9/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 13:48:20.000000 kioss-0.2.9/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19800 2023-08-01 13:48:20.000000 kioss-0.2.9/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-01 13:48:20.000000 kioss-0.2.9/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:48:29.498540 kioss-0.2.9/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-01 13:48:29.000000 kioss-0.2.9/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 13:48:29.000000 kioss-0.2.9/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:48:29.000000 kioss-0.2.9/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 13:48:29.000000 kioss-0.2.9/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:48:29.498540 kioss-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 13:48:20.000000 kioss-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:48:29.498540 kioss-0.2.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-08-01 13:48:20.000000 kioss-0.2.9/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-01 13:48:20.000000 kioss-0.2.9/test/test_util.py
```

### Comparing `kioss-0.2.8/LICENSE` & `kioss-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.2.8/README.md` & `kioss-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `kioss-0.2.8/kioss/pipe.py` & `kioss-0.2.9/kioss/pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,31 +335,35 @@
         super().__init__(iterator)
         logging.getLogger().setLevel(logging.INFO)
         self.what = what
         self.yields_count = 0
         self.errors_count = 0
         self.last_log_at_yields_count = 0
         self.start_time = time.time()
+        self._is_exhausted = False
 
     def _log(self) -> None:
         logging.info(
             "%s `%s` have been yielded in elapsed time '%s', with %s errors produced.",
             self.yields_count,
             self.what,
             str(
                 datetime.fromtimestamp(time.time())
                 - datetime.fromtimestamp(self.start_time)
             ),
             self.errors_count,
         )
 
     def __next__(self) -> T:
+        if self._is_exhausted:
+            raise StopIteration
         try:
             elem = super().__next__()
         except StopIteration:
+            self._is_exhausted = True
             if self.yields_count != self.last_log_at_yields_count:
                 self._log()
             raise
 
         self.yields_count += 1
         if isinstance(elem, Exception):
             self.errors_count += 1
@@ -421,35 +425,39 @@
     - the next element reception thrown an exception (it is stored in self.to_be_raised and will be raised during the next call to self.__next__)
     """
 
     def __init__(self, iterator: Iterator[T], size: int, secs: float) -> None:
         super().__init__(iterator)
         self.size = size
         self.secs = secs
-        self.to_be_raised: Exception = None
+        self._to_be_raised: Exception = None
+        self._is_exhausted = False
 
     def __next__(self) -> List[T]:
-        if self.to_be_raised:
-            e = self.to_be_raised
-            self.to_be_raised = None
+        if self._is_exhausted:
+            raise StopIteration
+        if self._to_be_raised:
+            e = self._to_be_raised
+            self._to_be_raised = None
             raise e
         start_time = time.time()
         batch = None
         try:
             batch = [super().__next__()]
             while len(batch) < self.size and (time.time() - start_time) < self.secs:
                 batch.append(super().__next__())
             return batch
         except StopIteration:
+            self._is_exhausted = True
             if batch:
                 return batch
             raise
         except Exception as e:
             if batch:
-                self.to_be_raised = e
+                self._to_be_raised = e
                 return batch
             raise
 
 
 class _ConcurrentlyMergingPipe(Pipe[T]):
     MAX_NUM_WAITING_ELEMS_PER_THREAD = 16
```

### Comparing `kioss-0.2.8/kioss/util.py` & `kioss-0.2.9/kioss/util.py`

 * *Files identical despite different names*

### Comparing `kioss-0.2.8/test/test_pipe.py` & `kioss-0.2.9/test/test_pipe.py`

 * *Files identical despite different names*

### Comparing `kioss-0.2.8/test/test_util.py` & `kioss-0.2.9/test/test_util.py`

 * *Files identical despite different names*

