# Comparing `tmp/switchinglogfilehandlers-0.0.3.tar.gz` & `tmp/switchinglogfilehandlers-0.0.4.tar.gz`

## Comparing `switchinglogfilehandlers-0.0.3.tar` & `switchinglogfilehandlers-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.3/foo.2022-12-10-21-31.log
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.3/foo.2022-12-10-21-32.log
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.3/foo.2022-12-10-21-33.log
--rwxr-xr-x   0        0        0     1650 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.3/testit
--rwxr-xr-x   0        0        0     1605 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.3/testit2
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.3/src/switchinglogfilehandlers/__init__.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.3/LICENSE
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.3/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-31.log
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-32.log
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-33.log
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo.2023-08-07-12-22.log
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo.2023-08-07-12-23.log
+-rwxr-xr-x   0        0        0     1650 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/testit
+-rwxr-xr-x   0        0        0     1613 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/testit2
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/testit3
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo/bar/baz.2023-08-07-12-31.log
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/foo/bar/baz.2023-08-07-12-32.log
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/src/switchinglogfilehandlers/__init__.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 switchinglogfilehandlers-0.0.4/PKG-INFO
```

### Comparing `switchinglogfilehandlers-0.0.3/foo.2022-12-10-21-31.log` & `switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-31.log`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.3/foo.2022-12-10-21-32.log` & `switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-32.log`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.3/foo.2022-12-10-21-33.log` & `switchinglogfilehandlers-0.0.4/foo.2022-12-10-21-33.log`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.3/testit` & `switchinglogfilehandlers-0.0.4/testit`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.3/testit2` & `switchinglogfilehandlers-0.0.4/testit2`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                 "formatter": "standard",
                 "stream": "ext://sys.stdout"
             },
             "file": {
                 "class":
                 "switchinglogfilehandlers.TimedSwitchingFileHandler",
                 "formatter": "standard",
-                "filename": "foo.",
+                "filename": "foo/bar/baz.",
                 "when": "m",
             },
         },
         "loggers": {
             "": {
                 "handlers": ["file"],
                 "level": "DEBUG"
```

### Comparing `switchinglogfilehandlers-0.0.3/src/switchinglogfilehandlers/__init__.py` & `switchinglogfilehandlers-0.0.4/src/switchinglogfilehandlers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import logging
+import os
+import os.path
 import threading
 import time
 
 class TimeoutSwitchingFileHandler(logging.Handler):
-    def __init__(self, filename, min_timeout=60, max_timeout=3600):
+    def __init__(self, filename, min_timeout=60, max_timeout=3600, create_directory=False):
         super().__init__()
         self.basename = filename
         self.min_timeout = min_timeout
         self.max_timeout = max_timeout
+        self.create_directory = create_directory
         self.fh = None
         self.last_emit = 0
         self.first_emit = 0
         self.last_emit = 0
         cleanup = threading.Thread(target=self.cleanup_loop, daemon=True)
         cleanup.start()
 
     def emit(self, record):
         msg = self.format(record)
         now = time.time()
         if not self.fh:
             now_tm = time.localtime(now)
             filename = self.basename + time.strftime("%Y-%m-%d-%H-%M-%S", now_tm) + "-%06d" % (now % 1 * 1000000) + ".log"
+            if self.create_directory:
+                dirname = os.path.dirname(filename)
+                os.makedirs(dirname, exist_ok=True)
             self.fh = open(filename, "a")
             self.first_emit = now
         self.fh.write(msg)
         self.fh.write("\n")
         self.fh.flush()
         self.last_emit = now
 
@@ -38,15 +44,15 @@
                 self.fh = None
             if self.fh and now - self.first_emit > self.max_timeout:
                 self.fh.close()
                 self.fh = None
             self.release()
 
 class TimedSwitchingFileHandler(logging.Handler):
-    def __init__(self, filename, when='h', utc=False):
+    def __init__(self, filename, when='h', utc=False, create_directory=False):
         super().__init__()
         self.basename = filename
         when = when.lower()
         if when == 's':
             self.timestamp_format = "%Y-%m-%d-%H-%M-%S"
         elif when == 'm':
             self.timestamp_format = "%Y-%m-%d-%H-%M"
@@ -55,27 +61,31 @@
         elif when == 'd':
             self.timestamp_format = "%Y-%m-%d"
         elif when == 'w':
             self.timestamp_format = "%Gw%V"
         else:
             raise ValueError(f"Unknown value “{when}” for when")
         self.utc = utc
+        self.create_directory = create_directory
         self.current_filename = None
         self.fh = None
 
     def emit(self, record):
         msg = self.format(record)
         now = time.time()
         if self.utc:
             now_tm = time.gmtime(now)
         else:
             now_tm = time.localtime(now)
         new_filename =  self.basename + time.strftime(self.timestamp_format, now_tm) + ".log"
         if new_filename != self.current_filename:
             if self.fh:
                 self.fh.close()
+            if self.create_directory:
+                new_dirname = os.path.dirname(new_filename)
+                os.makedirs(new_dirname, exist_ok=True)
             self.fh = open(new_filename, "a")
             self.current_filename = new_filename
         self.fh.write(msg)
         self.fh.write("\n")
         self.fh.flush()
```

### Comparing `switchinglogfilehandlers-0.0.3/LICENSE` & `switchinglogfilehandlers-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.3/README.md` & `switchinglogfilehandlers-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `switchinglogfilehandlers-0.0.3/pyproject.toml` & `switchinglogfilehandlers-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "switchinglogfilehandlers"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Peter J. Holzer", email="hjp@hjp.at" },
 ]
 description = "A collection of switching log file handlers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `switchinglogfilehandlers-0.0.3/PKG-INFO` & `switchinglogfilehandlers-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switchinglogfilehandlers
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of switching log file handlers
 Project-URL: Homepage, https://git.hjp.at:3000/hjp/switchinglogfilehandlers
 Project-URL: Bug Tracker, https://git.hjp.at:3000/hjp/switchinglogfilehandlers/issues
 Author-email: "Peter J. Holzer" <hjp@hjp.at>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

