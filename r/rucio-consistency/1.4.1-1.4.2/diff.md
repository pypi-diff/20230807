# Comparing `tmp/rucio-consistency-1.4.1.tar.gz` & `tmp/rucio-consistency-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-consistency-1.4.1.tar", last modified: Sat Aug  5 15:53:49 2023, max compression
+gzip compressed data, was "dist/rucio-consistency-1.4.2.tar", last modified: Mon Aug  7 18:20:21 2023, max compression
```

## Comparing `rucio-consistency-1.4.1.tar` & `rucio-consistency-1.4.2.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-05 15:53:49.161091 rucio-consistency-1.4.1/
--rw-r--r--   0 ivm        (503) staff       (20)    11357 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/LICENSE
--rw-r--r--   0 ivm        (503) staff       (20)      350 2023-08-05 15:53:49.160776 rucio-consistency-1.4.1/PKG-INFO
--rw-r--r--   0 ivm        (503) staff       (20)    12399 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/README.rst
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-05 15:53:49.153785 rucio-consistency-1.4.1/rucio_consistency/
--rw-r--r--   0 ivm        (503) staff       (20)      378 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/__init__.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4635 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/cmplib.py
--rw-r--r--   0 ivm        (503) staff       (20)    11469 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/config.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     5417 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/part.py
--rwxr-xr-x   0 ivm        (503) staff       (20)      372 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/py3.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-05 15:53:49.159147 rucio-consistency-1.4.1/rucio_consistency/scripts/
--rwxr-xr-x   0 ivm        (503) staff       (20)     3532 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/scripts/cmp2.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     3596 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/scripts/cmp3.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     4317 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/scripts/cmp5.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    10323 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/scripts/db_dump.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2737 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/scripts/partition.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     1069 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/scripts/update_stats.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     2523 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/stats.py
--rw-r--r--   0 ivm        (503) staff       (20)      125 2023-08-05 15:53:07.000000 rucio-consistency-1.4.1/rucio_consistency/version.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-05 15:53:49.160278 rucio-consistency-1.4.1/rucio_consistency/xrootd/
--rw-r--r--   0 ivm        (503) staff       (20)       39 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/xrootd/__init__.py
--rwxr-xr-x   0 ivm        (503) staff       (20)     9449 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/rucio_consistency/xrootd/xrootd_client.py
--rwxr-xr-x   0 ivm        (503) staff       (20)    29117 2023-08-05 15:52:56.000000 rucio-consistency-1.4.1/rucio_consistency/xrootd/xrootd_scanner.py
-drwxr-xr-x   0 ivm        (503) staff       (20)        0 2023-08-05 15:53:49.156579 rucio-consistency-1.4.1/rucio_consistency.egg-info/
--rw-r--r--   0 ivm        (503) staff       (20)      350 2023-08-05 15:53:49.000000 rucio-consistency-1.4.1/rucio_consistency.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (503) staff       (20)      850 2023-08-05 15:53:49.000000 rucio-consistency-1.4.1/rucio_consistency.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (503) staff       (20)        1 2023-08-05 15:53:49.000000 rucio-consistency-1.4.1/rucio_consistency.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (503) staff       (20)      388 2023-08-05 15:53:49.000000 rucio-consistency-1.4.1/rucio_consistency.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (503) staff       (20)        1 2023-08-05 15:53:49.000000 rucio-consistency-1.4.1/rucio_consistency.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (503) staff       (20)       22 2023-08-05 15:53:49.000000 rucio-consistency-1.4.1/rucio_consistency.egg-info/requires.txt
--rw-r--r--   0 ivm        (503) staff       (20)       18 2023-08-05 15:53:49.000000 rucio-consistency-1.4.1/rucio_consistency.egg-info/top_level.txt
--rw-r--r--   0 ivm        (503) staff       (20)       38 2023-08-05 15:53:49.161315 rucio-consistency-1.4.1/setup.cfg
--rw-r--r--   0 ivm        (503) staff       (20)     1391 2023-06-27 13:17:59.000000 rucio-consistency-1.4.1/setup.py
+drwxr-xr-x   0 ivm        (502) staff       (20)        0 2023-08-07 18:20:21.000000 rucio-consistency-1.4.2/
+-rw-r--r--   0 ivm        (502) staff       (20)      358 2023-08-07 18:20:21.000000 rucio-consistency-1.4.2/PKG-INFO
+-rw-r--r--   0 ivm        (502) staff       (20)    12399 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/README.rst
+drwxr-xr-x   0 ivm        (502) staff       (20)        0 2023-08-07 18:20:21.000000 rucio-consistency-1.4.2/rucio_consistency/
+-rw-r--r--   0 ivm        (502) staff       (20)      378 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/__init__.py
+-rwxr-xr-x   0 ivm        (502) staff       (20)     4635 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/cmplib.py
+-rw-r--r--   0 ivm        (502) staff       (20)    11469 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/config.py
+-rwxr-xr-x   0 ivm        (502) staff       (20)     5417 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/part.py
+-rwxr-xr-x   0 ivm        (502) staff       (20)      372 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/py3.py
+drwxr-xr-x   0 ivm        (502) staff       (20)        0 2023-08-07 18:20:21.000000 rucio-consistency-1.4.2/rucio_consistency/scripts/
+-rwxr-xr-x   0 ivm        (502) staff       (20)     3532 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/scripts/cmp2.py
+-rwxr-xr-x   0 ivm        (502) staff       (20)     3596 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/scripts/cmp3.py
+-rwxr-xr-x   0 ivm        (502) staff       (20)     4317 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/scripts/cmp5.py
+-rwxr-xr-x   0 ivm        (502) staff       (20)    10323 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/scripts/db_dump.py
+-rwxr-xr-x   0 ivm        (502) staff       (20)     2737 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/scripts/partition.py
+-rwxr-xr-x   0 ivm        (502) staff       (20)     1069 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/scripts/update_stats.py
+-rwxr-xr-x   0 ivm        (502) staff       (20)     2523 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/stats.py
+-rw-r--r--   0 ivm        (502) staff       (20)      125 2023-08-07 18:19:47.000000 rucio-consistency-1.4.2/rucio_consistency/version.py
+drwxr-xr-x   0 ivm        (502) staff       (20)        0 2023-08-07 18:20:21.000000 rucio-consistency-1.4.2/rucio_consistency/xrootd/
+-rw-r--r--   0 ivm        (502) staff       (20)       39 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/xrootd/__init__.py
+-rwxr-xr-x   0 ivm        (502) staff       (20)     9449 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/rucio_consistency/xrootd/xrootd_client.py
+-rwxr-xr-x   0 ivm        (502) staff       (20)    29194 2023-08-07 18:15:48.000000 rucio-consistency-1.4.2/rucio_consistency/xrootd/xrootd_scanner.py
+drwxr-xr-x   0 ivm        (502) staff       (20)        0 2023-08-07 18:20:21.000000 rucio-consistency-1.4.2/rucio_consistency.egg-info/
+-rw-r--r--   0 ivm        (502) staff       (20)      358 2023-08-07 18:20:20.000000 rucio-consistency-1.4.2/rucio_consistency.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (502) staff       (20)      842 2023-08-07 18:20:20.000000 rucio-consistency-1.4.2/rucio_consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (502) staff       (20)        1 2023-08-07 18:20:20.000000 rucio-consistency-1.4.2/rucio_consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (502) staff       (20)      389 2023-08-07 18:20:20.000000 rucio-consistency-1.4.2/rucio_consistency.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (502) staff       (20)        1 2023-08-07 18:20:20.000000 rucio-consistency-1.4.2/rucio_consistency.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (502) staff       (20)       22 2023-08-07 18:20:20.000000 rucio-consistency-1.4.2/rucio_consistency.egg-info/requires.txt
+-rw-r--r--   0 ivm        (502) staff       (20)       18 2023-08-07 18:20:20.000000 rucio-consistency-1.4.2/rucio_consistency.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (502) staff       (20)       38 2023-08-07 18:20:21.000000 rucio-consistency-1.4.2/setup.cfg
+-rw-r--r--   0 ivm        (502) staff       (20)     1391 2023-08-07 16:52:41.000000 rucio-consistency-1.4.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `rucio-consistency-1.4.1/README.rst` & `rucio-consistency-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/cmplib.py` & `rucio-consistency-1.4.2/rucio_consistency/cmplib.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/config.py` & `rucio-consistency-1.4.2/rucio_consistency/config.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/part.py` & `rucio-consistency-1.4.2/rucio_consistency/part.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/scripts/cmp2.py` & `rucio-consistency-1.4.2/rucio_consistency/scripts/cmp2.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/scripts/cmp3.py` & `rucio-consistency-1.4.2/rucio_consistency/scripts/cmp3.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/scripts/cmp5.py` & `rucio-consistency-1.4.2/rucio_consistency/scripts/cmp5.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/scripts/db_dump.py` & `rucio-consistency-1.4.2/rucio_consistency/scripts/db_dump.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/scripts/partition.py` & `rucio-consistency-1.4.2/rucio_consistency/scripts/partition.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/scripts/update_stats.py` & `rucio-consistency-1.4.2/rucio_consistency/scripts/update_stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/stats.py` & `rucio-consistency-1.4.2/rucio_consistency/stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/xrootd/xrootd_client.py` & `rucio-consistency-1.4.2/rucio_consistency/xrootd/xrootd_client.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.4.1/rucio_consistency/xrootd/xrootd_scanner.py` & `rucio-consistency-1.4.2/rucio_consistency/xrootd/xrootd_scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
             self.Master.scanner_succeeded(self, location, self.WasRecursive, files, dirs, empty_dir_count, empty_dirs)
 
 class ScannerMaster(PyThread):
     
     MAX_RECURSION_FAILED_COUNT = 5
     REPORT_INTERVAL = 10.0
     RESULTS_BUFFER_SISZE = 100
-    HEARTBEAT_INTERVAL = 300
+    HEARTBEAT_INTERVAL = None
     
     def __init__(self, client, path_converter, root, root_expected, recursive_threshold, max_scanners, timeout, quiet, display_progress, 
                 stats=None, my_stats=None, max_files=None,
                 include_sizes=True, ignore_list=[], list_empty_dirs=False):
         PyThread.__init__(self)
         self.RecursiveThreshold = recursive_threshold
         self.PathConverter = path_converter
@@ -275,21 +275,22 @@
         #
         # scan Root non-recursovely first, if failed, return immediarely
         #
         #server, location, recursive, timeout
         scanner_task = Scanner(self, self.Client, self.Timeout, self.Root, self.RecursiveThreshold == 0, include_sizes=self.IncludeSizes, 
                 report_empty_top=False, list_empty_dirs=self.ListEmptyDirs)
         self.ScannerQueue.addTask(scanner_task)
-        while not self.ScannerQueue.isEmpty():
-            self.sleep(self.HEARTBEAT_INTERVAL)
-            if self.MyStats is not None:
-                t = time.time()
-                self.MyStats["heartbeat"] = t
-                self.MyStats["heartbeat_utc"] = str(datetime.utcfromtimestamp(t))
-                self.Stats.save()
+        if self.HEARTBEAT_INTERVAL is not None:
+            while not self.ScannerQueue.isEmpty():
+                self.sleep(self.HEARTBEAT_INTERVAL)
+                if self.MyStats is not None:
+                    t = time.time()
+                    self.MyStats["heartbeat"] = t
+                    self.MyStats["heartbeat_utc"] = str(datetime.utcfromtimestamp(t))
+                    self.Stats.save()
         self.ScannerQueue.waitUntilEmpty()
         self.Results.close()
         self.ScannerQueue.Delegate = None       # detach for garbage collection
         self.ScannerQueue = None
         
     def dir_ignored(self, logpath):
         # path is expected to be canonic here
```

### Comparing `rucio-consistency-1.4.1/rucio_consistency.egg-info/SOURCES.txt` & `rucio-consistency-1.4.2/rucio_consistency.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.rst
 setup.py
 rucio_consistency/__init__.py
 rucio_consistency/cmplib.py
 rucio_consistency/config.py
 rucio_consistency/part.py
 rucio_consistency/py3.py
```

### Comparing `rucio-consistency-1.4.1/setup.py` & `rucio-consistency-1.4.2/setup.py`

 * *Files identical despite different names*

