# Comparing `tmp/zj_utils_zjj421-0.0.11.tar.gz` & `tmp/zj_utils_zjj421-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/zj/work_projects/private/zj_utils/dist/.tmp-hneq5sm3/zj_utils_zjj421-0.0.11.tar", last modified: Mon Aug  7 07:51:39 2023, max compression
+gzip compressed data, was "/home/zj/work_projects/zj_utils/dist/.tmp-mdv322wf/zj_utils_zjj421-0.0.9.tar", last modified: Thu Jul 13 05:54:52 2023, max compression
```

## Comparing `zj_utils_zjj421-0.0.11.tar` & `zj_utils_zjj421-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 zj        (1000) zj        (1000)        0 2023-08-07 07:51:39.000000 zj_utils_zjj421-0.0.11/
--rw-rw-r--   0 zj        (1000) zj        (1000)     1073 2023-03-20 07:29:22.000000 zj_utils_zjj421-0.0.11/LICENSE
--rw-rw-r--   0 zj        (1000) zj        (1000)      539 2023-08-07 07:51:39.000000 zj_utils_zjj421-0.0.11/PKG-INFO
--rw-rw-r--   0 zj        (1000) zj        (1000)       47 2023-07-13 02:06:49.000000 zj_utils_zjj421-0.0.11/README.md
--rw-rw-r--   0 zj        (1000) zj        (1000)      564 2023-08-07 07:50:47.000000 zj_utils_zjj421-0.0.11/pyproject.toml
--rw-rw-r--   0 zj        (1000) zj        (1000)       38 2023-08-07 07:51:39.000000 zj_utils_zjj421-0.0.11/setup.cfg
-drwxrwxr-x   0 zj        (1000) zj        (1000)        0 2023-08-07 07:51:39.000000 zj_utils_zjj421-0.0.11/src/
-drwxrwxr-x   0 zj        (1000) zj        (1000)        0 2023-08-07 07:51:39.000000 zj_utils_zjj421-0.0.11/src/zj_utils/
--rw-rw-r--   0 zj        (1000) zj        (1000)      245 2023-08-07 07:50:47.000000 zj_utils_zjj421-0.0.11/src/zj_utils/__init__.py
--rw-rw-r--   0 zj        (1000) zj        (1000)     3603 2023-03-20 07:29:22.000000 zj_utils_zjj421-0.0.11/src/zj_utils/concurrency.py
--rw-rw-r--   0 zj        (1000) zj        (1000)     4088 2023-03-20 09:47:52.000000 zj_utils_zjj421-0.0.11/src/zj_utils/files.py
--rw-rw-r--   0 zj        (1000) zj        (1000)     4789 2023-07-13 03:02:22.000000 zj_utils_zjj421-0.0.11/src/zj_utils/helper.py
--rw-rw-r--   0 zj        (1000) zj        (1000)     3872 2023-08-07 07:20:58.000000 zj_utils_zjj421-0.0.11/src/zj_utils/timer.py
--rw-rw-r--   0 zj        (1000) zj        (1000)     5102 2023-08-07 07:26:29.000000 zj_utils_zjj421-0.0.11/src/zj_utils/video_reader.py
-drwxrwxr-x   0 zj        (1000) zj        (1000)        0 2023-08-07 07:51:39.000000 zj_utils_zjj421-0.0.11/src/zj_utils_zjj421.egg-info/
--rw-rw-r--   0 zj        (1000) zj        (1000)      539 2023-08-07 07:51:39.000000 zj_utils_zjj421-0.0.11/src/zj_utils_zjj421.egg-info/PKG-INFO
--rw-rw-r--   0 zj        (1000) zj        (1000)      353 2023-08-07 07:51:39.000000 zj_utils_zjj421-0.0.11/src/zj_utils_zjj421.egg-info/SOURCES.txt
--rw-rw-r--   0 zj        (1000) zj        (1000)        1 2023-08-07 07:51:39.000000 zj_utils_zjj421-0.0.11/src/zj_utils_zjj421.egg-info/dependency_links.txt
--rw-rw-r--   0 zj        (1000) zj        (1000)        9 2023-08-07 07:51:39.000000 zj_utils_zjj421-0.0.11/src/zj_utils_zjj421.egg-info/top_level.txt
+drwxrwxr-x   0 zj        (1000) zj        (1000)        0 2023-07-13 05:54:52.000000 zj_utils_zjj421-0.0.9/
+-rw-rw-r--   0 zj        (1000) zj        (1000)     1073 2023-03-20 07:29:22.000000 zj_utils_zjj421-0.0.9/LICENSE
+-rw-rw-r--   0 zj        (1000) zj        (1000)      538 2023-07-13 05:54:52.000000 zj_utils_zjj421-0.0.9/PKG-INFO
+-rw-rw-r--   0 zj        (1000) zj        (1000)       47 2023-07-13 02:06:49.000000 zj_utils_zjj421-0.0.9/README.md
+-rw-rw-r--   0 zj        (1000) zj        (1000)      563 2023-07-13 05:54:03.000000 zj_utils_zjj421-0.0.9/pyproject.toml
+-rw-rw-r--   0 zj        (1000) zj        (1000)       38 2023-07-13 05:54:52.000000 zj_utils_zjj421-0.0.9/setup.cfg
+drwxrwxr-x   0 zj        (1000) zj        (1000)        0 2023-07-13 05:54:52.000000 zj_utils_zjj421-0.0.9/src/
+drwxrwxr-x   0 zj        (1000) zj        (1000)        0 2023-07-13 05:54:52.000000 zj_utils_zjj421-0.0.9/src/zj_utils/
+-rw-rw-r--   0 zj        (1000) zj        (1000)      244 2023-07-13 03:02:22.000000 zj_utils_zjj421-0.0.9/src/zj_utils/__init__.py
+-rw-rw-r--   0 zj        (1000) zj        (1000)     3603 2023-03-20 07:29:22.000000 zj_utils_zjj421-0.0.9/src/zj_utils/concurrency.py
+-rw-rw-r--   0 zj        (1000) zj        (1000)     4088 2023-03-20 09:47:52.000000 zj_utils_zjj421-0.0.9/src/zj_utils/files.py
+-rw-rw-r--   0 zj        (1000) zj        (1000)     4789 2023-07-13 03:02:22.000000 zj_utils_zjj421-0.0.9/src/zj_utils/helper.py
+-rw-rw-r--   0 zj        (1000) zj        (1000)     3802 2023-07-13 02:08:47.000000 zj_utils_zjj421-0.0.9/src/zj_utils/timer.py
+-rw-rw-r--   0 zj        (1000) zj        (1000)     3664 2023-07-13 02:32:27.000000 zj_utils_zjj421-0.0.9/src/zj_utils/video_reader.py
+drwxrwxr-x   0 zj        (1000) zj        (1000)        0 2023-07-13 05:54:52.000000 zj_utils_zjj421-0.0.9/src/zj_utils_zjj421.egg-info/
+-rw-rw-r--   0 zj        (1000) zj        (1000)      538 2023-07-13 05:54:52.000000 zj_utils_zjj421-0.0.9/src/zj_utils_zjj421.egg-info/PKG-INFO
+-rw-rw-r--   0 zj        (1000) zj        (1000)      353 2023-07-13 05:54:52.000000 zj_utils_zjj421-0.0.9/src/zj_utils_zjj421.egg-info/SOURCES.txt
+-rw-rw-r--   0 zj        (1000) zj        (1000)        1 2023-07-13 05:54:52.000000 zj_utils_zjj421-0.0.9/src/zj_utils_zjj421.egg-info/dependency_links.txt
+-rw-rw-r--   0 zj        (1000) zj        (1000)        9 2023-07-13 05:54:52.000000 zj_utils_zjj421-0.0.9/src/zj_utils_zjj421.egg-info/top_level.txt
```

### Comparing `zj_utils_zjj421-0.0.11/LICENSE` & `zj_utils_zjj421-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zj_utils_zjj421-0.0.11/PKG-INFO` & `zj_utils_zjj421-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zj_utils_zjj421
-Version: 0.0.11
+Version: 0.0.9
 Summary: A personal kit
 Author-email: zjj421 <zhangjian421wo@outlook.com>
 Project-URL: Homepage, https://github.com/zjj421/zj_utils
 Project-URL: Bug Tracker, https://github.com/zjj421/zj_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zj_utils_zjj421-0.0.11/pyproject.toml` & `zj_utils_zjj421-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "zj_utils_zjj421"
-version = "0.0.11"
+version = "0.0.9"
 authors = [
   { name="zjj421", email="zhangjian421wo@outlook.com" },
 ]
 description = "A personal kit"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `zj_utils_zjj421-0.0.11/src/zj_utils/concurrency.py` & `zj_utils_zjj421-0.0.9/src/zj_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `zj_utils_zjj421-0.0.11/src/zj_utils/files.py` & `zj_utils_zjj421-0.0.9/src/zj_utils/files.py`

 * *Files identical despite different names*

### Comparing `zj_utils_zjj421-0.0.11/src/zj_utils/helper.py` & `zj_utils_zjj421-0.0.9/src/zj_utils/helper.py`

 * *Files identical despite different names*

### Comparing `zj_utils_zjj421-0.0.11/src/zj_utils/timer.py` & `zj_utils_zjj421-0.0.9/src/zj_utils/timer.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,32 +3,30 @@
 # Created by zj on 2020/10/13 
 # Task:
 from collections import deque
 from datetime import datetime
 import time
 import cv2
 
-__all__ = ['FPSRealTime', 'FPS', 'MyTimer', 'runtime']
-
 
 class FPSRealTime(object):
     def __init__(self, buffer_len=10):
         self._start_tick = cv2.getTickCount()
         self._freq = 1000.0 / cv2.getTickFrequency()
         self._difftimes = deque(maxlen=buffer_len)
 
-    def get_fps(self, number=2):
+    def get_fps(self):
         current_tick = cv2.getTickCount()
         different_time = (current_tick - self._start_tick) * self._freq
         self._start_tick = current_tick
 
         self._difftimes.append(different_time)
 
         fps = 1000.0 / (sum(self._difftimes) / len(self._difftimes))
-        fps_rounded = round(fps, number)
+        fps_rounded = round(fps, 2)
 
         return fps_rounded
 
 
 class FPS:
     def __init__(self):
         # store the start time, end time, and total number of frames
@@ -86,14 +84,15 @@
 
     def log(self, tip='Elapsed time', unit='ms', reset=False):
         duration = round(self.elapsed(reset, unit), 3)
         print('{}: {}{}'.format(tip, duration, unit))
         return duration
 
     def rlog(self, tip='Elapsed time'):
+
         return self.log(unit='ms', reset=True, tip=tip)
 
     def total_elapsed(self, unit='ms'):
         assert unit in ('us', 'ms', 's', 'min')
         duration = (time.time() - self.first_start_time)
         if unit == 'us':
             duration = duration * 1e6
```

### Comparing `zj_utils_zjj421-0.0.11/src/zj_utils_zjj421.egg-info/PKG-INFO` & `zj_utils_zjj421-0.0.9/src/zj_utils_zjj421.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zj-utils-zjj421
-Version: 0.0.11
+Version: 0.0.9
 Summary: A personal kit
 Author-email: zjj421 <zhangjian421wo@outlook.com>
 Project-URL: Homepage, https://github.com/zjj421/zj_utils
 Project-URL: Bug Tracker, https://github.com/zjj421/zj_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

