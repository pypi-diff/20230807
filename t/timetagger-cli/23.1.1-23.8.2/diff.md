# Comparing `tmp/timetagger_cli-23.1.1.tar.gz` & `tmp/timetagger_cli-23.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timetagger_cli-23.1.1.tar", last modified: Tue Jan 24 08:32:21 2023, max compression
+gzip compressed data, was "timetagger_cli-23.8.2.tar", last modified: Mon Aug  7 15:14:38 2023, max compression
```

## Comparing `timetagger_cli-23.1.1.tar` & `timetagger_cli-23.8.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-01-24 08:32:21.486199 timetagger_cli-23.1.1/
--rw-r--r--   0 almar      (501) staff       (20)     1068 2023-01-24 08:13:00.000000 timetagger_cli-23.1.1/LICENSE
--rw-r--r--   0 almar      (501) staff       (20)     1509 2023-01-24 08:32:21.485838 timetagger_cli-23.1.1/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)     2542 2023-01-24 08:13:00.000000 timetagger_cli-23.1.1/README.md
--rw-r--r--   0 almar      (501) staff       (20)       38 2023-01-24 08:32:21.486323 timetagger_cli-23.1.1/setup.cfg
--rw-r--r--   0 almar      (501) staff       (20)     2110 2023-01-24 08:30:47.000000 timetagger_cli-23.1.1/setup.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-01-24 08:32:21.401208 timetagger_cli-23.1.1/timetagger_cli/
--rw-r--r--   0 almar      (501) staff       (20)      220 2023-01-24 08:31:36.000000 timetagger_cli-23.1.1/timetagger_cli/__init__.py
--rw-r--r--   0 almar      (501) staff       (20)     2063 2023-01-24 08:13:00.000000 timetagger_cli-23.1.1/timetagger_cli/__main__.py
--rw-r--r--   0 almar      (501) staff       (20)     2170 2023-01-24 08:13:00.000000 timetagger_cli-23.1.1/timetagger_cli/config.py
--rw-r--r--   0 almar      (501) staff       (20)     6373 2023-01-24 08:13:00.000000 timetagger_cli-23.1.1/timetagger_cli/core.py
--rw-r--r--   0 almar      (501) staff       (20)     2594 2023-01-24 08:13:00.000000 timetagger_cli-23.1.1/timetagger_cli/utils.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-01-24 08:32:21.485031 timetagger_cli-23.1.1/timetagger_cli.egg-info/
--rw-r--r--   0 almar      (501) staff       (20)     1509 2023-01-24 08:32:21.000000 timetagger_cli-23.1.1/timetagger_cli.egg-info/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)      415 2023-01-24 08:32:21.000000 timetagger_cli-23.1.1/timetagger_cli.egg-info/SOURCES.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2023-01-24 08:32:21.000000 timetagger_cli-23.1.1/timetagger_cli.egg-info/dependency_links.txt
--rw-r--r--   0 almar      (501) staff       (20)       60 2023-01-24 08:32:21.000000 timetagger_cli-23.1.1/timetagger_cli.egg-info/entry_points.txt
--rw-r--r--   0 almar      (501) staff       (20)       14 2023-01-24 08:32:21.000000 timetagger_cli-23.1.1/timetagger_cli.egg-info/requires.txt
--rw-r--r--   0 almar      (501) staff       (20)       15 2023-01-24 08:32:21.000000 timetagger_cli-23.1.1/timetagger_cli.egg-info/top_level.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2023-01-24 08:32:21.000000 timetagger_cli-23.1.1/timetagger_cli.egg-info/zip-safe
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-08-07 15:14:38.885054 timetagger_cli-23.8.2/
+-rw-r--r--   0 almar      (501) staff       (20)     1068 2023-01-24 08:13:00.000000 timetagger_cli-23.8.2/LICENSE
+-rw-r--r--   0 almar      (501) staff       (20)     1509 2023-08-07 15:14:38.884928 timetagger_cli-23.8.2/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     2542 2023-01-24 08:13:00.000000 timetagger_cli-23.8.2/README.md
+-rw-r--r--   0 almar      (501) staff       (20)       38 2023-08-07 15:14:38.885110 timetagger_cli-23.8.2/setup.cfg
+-rw-r--r--   0 almar      (501) staff       (20)     2110 2023-01-24 08:30:47.000000 timetagger_cli-23.8.2/setup.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-08-07 15:14:38.882372 timetagger_cli-23.8.2/timetagger_cli/
+-rw-r--r--   0 almar      (501) staff       (20)      228 2023-08-07 15:14:28.000000 timetagger_cli-23.8.2/timetagger_cli/__init__.py
+-rw-r--r--   0 almar      (501) staff       (20)     2089 2023-08-07 15:13:20.000000 timetagger_cli-23.8.2/timetagger_cli/__main__.py
+-rw-r--r--   0 almar      (501) staff       (20)     2170 2023-01-24 08:13:00.000000 timetagger_cli-23.8.2/timetagger_cli/config.py
+-rw-r--r--   0 almar      (501) staff       (20)     7856 2023-08-07 15:13:20.000000 timetagger_cli-23.8.2/timetagger_cli/core.py
+-rw-r--r--   0 almar      (501) staff       (20)     2594 2023-01-24 08:13:00.000000 timetagger_cli-23.8.2/timetagger_cli/utils.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-08-07 15:14:38.884599 timetagger_cli-23.8.2/timetagger_cli.egg-info/
+-rw-r--r--   0 almar      (501) staff       (20)     1509 2023-08-07 15:14:38.000000 timetagger_cli-23.8.2/timetagger_cli.egg-info/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)      415 2023-08-07 15:14:38.000000 timetagger_cli-23.8.2/timetagger_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2023-08-07 15:14:38.000000 timetagger_cli-23.8.2/timetagger_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 almar      (501) staff       (20)       60 2023-08-07 15:14:38.000000 timetagger_cli-23.8.2/timetagger_cli.egg-info/entry_points.txt
+-rw-r--r--   0 almar      (501) staff       (20)       14 2023-08-07 15:14:38.000000 timetagger_cli-23.8.2/timetagger_cli.egg-info/requires.txt
+-rw-r--r--   0 almar      (501) staff       (20)       15 2023-08-07 15:14:38.000000 timetagger_cli-23.8.2/timetagger_cli.egg-info/top_level.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2023-01-24 08:32:21.000000 timetagger_cli-23.8.2/timetagger_cli.egg-info/zip-safe
```

### Comparing `timetagger_cli-23.1.1/LICENSE` & `timetagger_cli-23.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timetagger_cli-23.1.1/PKG-INFO` & `timetagger_cli-23.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetagger_cli
-Version: 23.1.1
+Version: 23.8.2
 Summary: Track your time from the command-line.
 Home-page: https://github.com/almarklein/timetagger_cli
 Author: Almar Klein
 Author-email: 
 License: MIT
 Keywords: time,tracker,CLI,terminal
 Platform: any
```

### Comparing `timetagger_cli-23.1.1/README.md` & `timetagger_cli-23.8.2/README.md`

 * *Files identical despite different names*

### Comparing `timetagger_cli-23.1.1/setup.py` & `timetagger_cli-23.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `timetagger_cli-23.1.1/timetagger_cli/__main__.py` & `timetagger_cli-23.8.2/timetagger_cli/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,19 +48,19 @@
     version,
     help,
     timetagger_cli.app,
     timetagger_cli.setup,
     timetagger_cli.status,
     timetagger_cli.start,
     timetagger_cli.stop,
+    timetagger_cli.resume,
 )
 
 
 def main(argv=None):
-
     assert sys.version_info.major == 3, "This script needs to run with Python 3."
 
     # Get CLI args
     if argv is None:
         argv = sys.argv[1:]
     if not argv:
         argv = ["help"]
```

### Comparing `timetagger_cli-23.1.1/timetagger_cli/config.py` & `timetagger_cli-23.8.2/timetagger_cli/config.py`

 * *Files identical despite different names*

### Comparing `timetagger_cli-23.1.1/timetagger_cli/core.py` & `timetagger_cli-23.8.2/timetagger_cli/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -150,14 +150,73 @@
     else:
         print("Stopping running records.")
         request("PUT", "records", running_records)
         print()
         print_records(running_records)
 
 
+def resume():
+    """Start a timer with the same description as previous."""
+
+    now = int(time.time())
+    d = datetime.datetime.fromtimestamp(now)
+
+    today = datetime.datetime(d.year, d.month, d.day)
+    tomorrow = today + datetime.timedelta(1)
+
+    t1 = int(today.timestamp())
+    t2 = int(tomorrow.timestamp())
+
+    # Get records from today
+    records = request("GET", f"records?timerange={t1}-{t2}")["records"]
+
+    if len(records) == 0:
+        print("No records earlier today.")
+        return
+
+    # Remove HIDDEN records
+    filtered_records = [r for r in records if "HIDDEN" not in r["ds"]]
+
+    # Get last record
+    last_record = filtered_records[-1]
+
+    # Get running records, to stop them
+    running_records = get_running_records()
+    for r in running_records:
+        if r.get("ds", "") == last_record["ds"]:
+            print("Timer with this description is already running.")
+            print()
+            print_records([r])
+            return
+        r["t2"] = now
+
+    # Create new record
+    r = {
+        "key": generate_uid(),
+        "t1": now,
+        "t2": now,
+        "mt": time.time(),
+        "st": 0,
+        "ds": last_record["ds"],
+    }
+
+    # Push
+    records = running_records + [r]
+    request("PUT", "records", records)
+
+    # Report
+    if not running_records:
+        print("Timer started ...")
+    else:
+        print(f"Timer started ... and stopped {len(running_records)} running records.")
+
+    print()
+    print_records(records)
+
+
 def status():
     """Get an overview of today and this week. The exact content may change."""
 
     now = int(time.time())
     d = datetime.datetime.fromtimestamp(now)
 
     # Get important dates
```

### Comparing `timetagger_cli-23.1.1/timetagger_cli/utils.py` & `timetagger_cli-23.8.2/timetagger_cli/utils.py`

 * *Files identical despite different names*

### Comparing `timetagger_cli-23.1.1/timetagger_cli.egg-info/PKG-INFO` & `timetagger_cli-23.8.2/timetagger_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetagger-cli
-Version: 23.1.1
+Version: 23.8.2
 Summary: Track your time from the command-line.
 Home-page: https://github.com/almarklein/timetagger_cli
 Author: Almar Klein
 Author-email: 
 License: MIT
 Keywords: time,tracker,CLI,terminal
 Platform: any
```

