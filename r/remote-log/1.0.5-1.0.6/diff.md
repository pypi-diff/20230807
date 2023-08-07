# Comparing `tmp/remote-log-1.0.5.tar.gz` & `tmp/remote-log-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote-log-1.0.5.tar", last modified: Sat Aug  5 14:09:26 2023, max compression
+gzip compressed data, was "remote-log-1.0.6.tar", last modified: Mon Aug  7 20:44:31 2023, max compression
```

## Comparing `remote-log-1.0.5.tar` & `remote-log-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:09:26.581902 remote-log-1.0.5/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1046 2023-08-05 14:09:26.581790 remote-log-1.0.5/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      824 2023-08-05 14:09:03.000000 remote-log-1.0.5/README.md
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:09:26.580639 remote-log-1.0.5/remote_log/
--rw-r--r--   0 brainspoof   (501) staff       (20)       25 2023-08-04 20:15:20.000000 remote-log-1.0.5/remote_log/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       34 2023-08-05 13:41:02.000000 remote-log-1.0.5/remote_log/__main__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2540 2023-08-05 13:16:24.000000 remote-log-1.0.5/remote_log/remote_log.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2180 2023-08-05 11:12:34.000000 remote-log-1.0.5/remote_log/sysinfo.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       28 2023-08-04 20:15:20.000000 remote-log-1.0.5/remote_log/tests.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-05 14:09:26.581397 remote-log-1.0.5/remote_log.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1046 2023-08-05 14:09:26.000000 remote-log-1.0.5/remote_log.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      300 2023-08-05 14:09:26.000000 remote-log-1.0.5/remote_log.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-08-05 14:09:26.000000 remote-log-1.0.5/remote_log.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       27 2023-08-05 14:09:26.000000 remote-log-1.0.5/remote_log.egg-info/requires.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       11 2023-08-05 14:09:26.000000 remote-log-1.0.5/remote_log.egg-info/top_level.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-08-05 14:09:26.581945 remote-log-1.0.5/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      644 2023-08-05 14:09:24.000000 remote-log-1.0.5/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-07 20:44:31.488026 remote-log-1.0.6/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1046 2023-08-07 20:44:31.487872 remote-log-1.0.6/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      824 2023-08-05 14:09:03.000000 remote-log-1.0.6/README.md
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-07 20:44:31.486790 remote-log-1.0.6/remote_log/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       25 2023-08-04 20:15:20.000000 remote-log-1.0.6/remote_log/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       34 2023-08-05 13:41:02.000000 remote-log-1.0.6/remote_log/__main__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2540 2023-08-05 13:16:24.000000 remote-log-1.0.6/remote_log/remote_log.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1976 2023-08-07 20:43:27.000000 remote-log-1.0.6/remote_log/sysinfo.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       28 2023-08-04 20:15:20.000000 remote-log-1.0.6/remote_log/tests.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-08-07 20:44:31.487626 remote-log-1.0.6/remote_log.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1046 2023-08-07 20:44:31.000000 remote-log-1.0.6/remote_log.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      300 2023-08-07 20:44:31.000000 remote-log-1.0.6/remote_log.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-08-07 20:44:31.000000 remote-log-1.0.6/remote_log.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       27 2023-08-07 20:44:31.000000 remote-log-1.0.6/remote_log.egg-info/requires.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       11 2023-08-07 20:44:31.000000 remote-log-1.0.6/remote_log.egg-info/top_level.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-08-07 20:44:31.488092 remote-log-1.0.6/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      644 2023-08-07 20:43:08.000000 remote-log-1.0.6/setup.py
```

### Comparing `remote-log-1.0.5/PKG-INFO` & `remote-log-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remote-log
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple function to send logging data to a remote server.
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 Description-Content-Type: text/markdown
 
 ```python
 import remote_log
```

### Comparing `remote-log-1.0.5/README.md` & `remote-log-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `remote-log-1.0.5/remote_log/remote_log.py` & `remote-log-1.0.6/remote_log/remote_log.py`

 * *Files identical despite different names*

### Comparing `remote-log-1.0.5/remote_log/sysinfo.py` & `remote-log-1.0.6/remote_log/sysinfo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import psutil
 import platform
 import uuid
 import datetime
 import sysconfig
 import hashlib
-import cpuinfo
 import time
 
 # Function to convert large number of bytes into a readable format
 def get_size(bytes, suffix="B"):
     factor = 1024
     for unit in ["", "K", "M", "G", "T", "P"]:
         if bytes < factor:
             return f"{bytes:.2f}{unit}{suffix}"
         bytes /= factor
 
 def get_system_info():
-    cpu = cpuinfo.get_cpu_info()
     
     # Get system info
     info = {}
 
     # System
     info["system"] = platform.system()
 
@@ -34,17 +32,14 @@
     info["platform"] = sysconfig.get_platform()
 
     # Machine
     info["machine"] = platform.machine()
 
     # Processor Info
     info["processor_type"] = platform.processor()
-    info["processor_name"] = cpu["brand_raw"]
-    info["processor_architecture"] = cpu["arch"]
-    info["processor_version"]= cpu["cpuinfo_version_string"]
     
     info["physical_cores"] = psutil.cpu_count(logical=False)
     info["total_cores"] = psutil.cpu_count(logical=True)
 
     # Current Time
     current_time = datetime.datetime.now().astimezone()
     info["current_time"] = current_time.strftime("%Y-%m-%d %H:%M:%S") + " " + time.tzname[1]
```

### Comparing `remote-log-1.0.5/remote_log.egg-info/PKG-INFO` & `remote-log-1.0.6/remote_log.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remote-log
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple function to send logging data to a remote server.
 Author: Shubham Gupta
 Author-email: shubhastro2@gmail.com
 Description-Content-Type: text/markdown
 
 ```python
 import remote_log
```

### Comparing `remote-log-1.0.5/setup.py` & `remote-log-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='remote-log',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     description = 'A simple function to send logging data to a remote server.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Shubham Gupta',
     author_email = 'shubhastro2@gmail.com',
     install_requires=[
```

