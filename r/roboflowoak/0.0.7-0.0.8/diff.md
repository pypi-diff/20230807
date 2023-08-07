# Comparing `tmp/roboflowoak-0.0.7.tar.gz` & `tmp/roboflowoak-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/roboflowoak-0.0.7.tar", last modified: Thu Nov  3 02:53:24 2022, max compression
+gzip compressed data, was "roboflowoak-0.0.8.tar", last modified: Mon Nov  7 00:03:14 2022, max compression
```

## Comparing `roboflowoak-0.0.7.tar` & `roboflowoak-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 maxwellstone   (501) staff       (20)        0 2022-11-03 02:53:24.185613 roboflowoak-0.0.7/
--rw-r--r--   0 maxwellstone   (501) staff       (20)    35127 2022-09-05 03:44:08.000000 roboflowoak-0.0.7/LICENSE
--rw-r--r--   0 maxwellstone   (501) staff       (20)      454 2022-11-03 02:53:24.185495 roboflowoak-0.0.7/PKG-INFO
--rw-r--r--   0 maxwellstone   (501) staff       (20)     1149 2022-09-05 03:44:08.000000 roboflowoak-0.0.7/README.md
-drwxr-xr-x   0 maxwellstone   (501) staff       (20)        0 2022-11-03 02:53:24.184594 roboflowoak-0.0.7/roboflowoak/
--rw-r--r--   0 maxwellstone   (501) staff       (20)     5726 2022-11-03 02:45:55.000000 roboflowoak-0.0.7/roboflowoak/__init__.py
--rw-r--r--   0 maxwellstone   (501) staff       (20)     1263 2022-09-05 03:44:08.000000 roboflowoak-0.0.7/roboflowoak/api.py
--rw-r--r--   0 maxwellstone   (501) staff       (20)    10922 2022-10-08 21:18:31.000000 roboflowoak-0.0.7/roboflowoak/pipe.py
--rw-r--r--   0 maxwellstone   (501) staff       (20)     4207 2022-09-19 21:59:44.000000 roboflowoak-0.0.7/roboflowoak/postprocs.py
-drwxr-xr-x   0 maxwellstone   (501) staff       (20)        0 2022-11-03 02:53:24.185348 roboflowoak-0.0.7/roboflowoak.egg-info/
--rw-r--r--   0 maxwellstone   (501) staff       (20)      454 2022-11-03 02:53:24.000000 roboflowoak-0.0.7/roboflowoak.egg-info/PKG-INFO
--rw-r--r--   0 maxwellstone   (501) staff       (20)      288 2022-11-03 02:53:24.000000 roboflowoak-0.0.7/roboflowoak.egg-info/SOURCES.txt
--rw-r--r--   0 maxwellstone   (501) staff       (20)        1 2022-11-03 02:53:24.000000 roboflowoak-0.0.7/roboflowoak.egg-info/dependency_links.txt
--rw-r--r--   0 maxwellstone   (501) staff       (20)       17 2022-11-03 02:53:24.000000 roboflowoak-0.0.7/roboflowoak.egg-info/requires.txt
--rw-r--r--   0 maxwellstone   (501) staff       (20)       12 2022-11-03 02:53:24.000000 roboflowoak-0.0.7/roboflowoak.egg-info/top_level.txt
--rw-r--r--   0 maxwellstone   (501) staff       (20)       38 2022-11-03 02:53:24.185653 roboflowoak-0.0.7/setup.cfg
--rw-r--r--   0 maxwellstone   (501) staff       (20)      773 2022-11-03 02:53:00.000000 roboflowoak-0.0.7/setup.py
+drwxr-xr-x   0 jacobsolawetz   (501) staff       (20)        0 2022-11-07 00:03:14.473943 roboflowoak-0.0.8/
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)    35127 2022-11-06 23:57:57.000000 roboflowoak-0.0.8/LICENSE
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)      473 2022-11-07 00:03:14.473802 roboflowoak-0.0.8/PKG-INFO
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)     1149 2022-11-06 23:57:57.000000 roboflowoak-0.0.8/README.md
+drwxr-xr-x   0 jacobsolawetz   (501) staff       (20)        0 2022-11-07 00:03:14.473059 roboflowoak-0.0.8/roboflowoak/
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)     5828 2022-11-06 23:58:59.000000 roboflowoak-0.0.8/roboflowoak/__init__.py
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)     1238 2022-11-06 23:58:59.000000 roboflowoak-0.0.8/roboflowoak/api.py
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)    10886 2022-11-06 23:57:57.000000 roboflowoak-0.0.8/roboflowoak/pipe.py
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)     4207 2022-11-06 23:57:57.000000 roboflowoak-0.0.8/roboflowoak/postprocs.py
+drwxr-xr-x   0 jacobsolawetz   (501) staff       (20)        0 2022-11-07 00:03:14.473621 roboflowoak-0.0.8/roboflowoak.egg-info/
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)      473 2022-11-07 00:03:14.000000 roboflowoak-0.0.8/roboflowoak.egg-info/PKG-INFO
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)      288 2022-11-07 00:03:14.000000 roboflowoak-0.0.8/roboflowoak.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)        1 2022-11-07 00:03:14.000000 roboflowoak-0.0.8/roboflowoak.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)       17 2022-11-07 00:03:14.000000 roboflowoak-0.0.8/roboflowoak.egg-info/requires.txt
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)       12 2022-11-07 00:03:14.000000 roboflowoak-0.0.8/roboflowoak.egg-info/top_level.txt
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)       38 2022-11-07 00:03:14.473984 roboflowoak-0.0.8/setup.cfg
+-rw-r--r--   0 jacobsolawetz   (501) staff       (20)      773 2022-11-06 23:59:08.000000 roboflowoak-0.0.8/setup.py
```

### Comparing `roboflowoak-0.0.7/LICENSE` & `roboflowoak-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `roboflowoak-0.0.7/README.md` & `roboflowoak-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `roboflowoak-0.0.7/roboflowoak/__init__.py` & `roboflowoak-0.0.8/roboflowoak/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import threading
 from pip._internal.utils.appdirs import user_cache_dir
 import shutil
 
 cache_dir = user_cache_dir('pip') + "/roboflow"
 
 class RoboflowOak:
-    def __init__(self, model, version, api_key, confidence=0.2, overlap=0.5, advanced_config={}, rgb=False, depth=False, device=None, device_name="device", blocking=True, legacy=False):
+    def __init__(self, model, version, api_key, confidence=0.2, overlap=0.5, advanced_config={}, rgb=False, depth=False, device=None, device_name="device", blocking=True, legacy=False, api_endpoint="https://api.roboflow.com"):
         self.project = model
         self.version = version
         self.api_key = api_key
         self.blocking = blocking
         self.depth = depth
         self.confidence = confidence
         self.overlap = overlap
         self.device_name = device_name
         self.dev = device
+        self.api_endpoint = api_endpoint
         self.advanced_config = advanced_config
         self.fast = not len(self.advanced_config.keys()) > 0
         self.sensor_mode = "THE_1080_P"
         self.wide_fov = False
         if "sensor_mode" in self.advanced_config.keys():
             self.sensor_mode = advanced_config["sensor_mode"]
         if "wide_fov" in self.advanced_config.keys():
@@ -39,15 +40,15 @@
         self.cache_path = self.find_weights()
         with open(os.path.join(self.cache_path, 'config.txt'), 'r') as f:
             self.model_objects = json.loads(f.read())
             self.size = (int(self.model_objects["environment"]["RESOLUTION"]), int(self.model_objects["environment"]["RESOLUTION"]))
             self.resolution = self.size
             self.class_names = self.model_objects["class_names"]
             self.colors = self.model_objects["colors"]
-            print("Size",self.size,"Resolution",self.resolution)
+            #print("Size",self.size,"Resolution",self.resolution)
         try:
             self.dai_pipe = DepthAIPipeline(self.cache_path+"/roboflow.blob", self.size, self.resolution, self.class_names, rgb, self.colors, self.fast, self.confidence, self.overlap, self.sensor_mode, self.wide_fov, depth, device, legacy)
         except:
             try:
                 shutil.rmtree(cache_dir)
                 self.cache_path = self.find_weights()
                 with open(os.path.join(self.cache_path, 'config.txt'), 'r') as f:
@@ -61,15 +62,15 @@
                 raise Exception("Failure while retrying load weights - does this model, version, api key exist? can you curl api.roboflow.com, and can your device download files from google cloud storage? have you hit your device limit?")
 
     def find_weights(self):
         if os.path.exists(os.path.join(cache_dir, self.project, self.version, "roboflow.blob")) and os.path.exists(
                         os.path.join(cache_dir, self.project, self.version, "config.txt")):
             return os.path.join(cache_dir, self.project, self.version)
 
-        return download_blob(self.project, self.version, self.api_key, self.dev)
+        return download_blob(self.project, self.version, self.api_key, self.dev, self.api_endpoint)
 
     def detect(self):
         ret = self.dai_pipe.get()
 
         predictions = []
         dets = ret[0]
         for det in dets:
```

### Comparing `roboflowoak-0.0.7/roboflowoak/api.py` & `roboflowoak-0.0.8/roboflowoak/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import requests
 import os
 import json
 from pip._internal.utils.appdirs import user_cache_dir
 
-api_endpoint = "https://api.roboflow.com/oak/"
 cache_dir = user_cache_dir('pip') + "/roboflow"
 
-def download_blob(project, version, api_key, device_id):
+def download_blob(project, version, api_key, device_id, api_endpoint):
 
-    endpoint = api_endpoint+project+"/"+version+"?api_key="+api_key+"&device="+device_id
+    endpoint = api_endpoint+"/oak/"+project+"/"+version+"?api_key="+api_key+"&device="+device_id
     api_data = requests.get(endpoint)
 
     if api_data.status_code != 200:
         raise Exception(str(api_data.json()))
     api_data = api_data.json()
     if 'warning' in api_data.keys():
         print(api_data['warning'], flush=True)
```

### Comparing `roboflowoak-0.0.7/roboflowoak/pipe.py` & `roboflowoak-0.0.8/roboflowoak/pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,14 @@
     def get(self):
         if self.depth:
             in_depth = self.q_depth.get()
 
         #in_manip = self.q_manip.get()
 
         in_det = self.q_det.get()
-        print("getting detections")
         detections = self.post_processing(in_det)
 
         depth = None
 
         if self.depth:
             depth = in_depth.getFrame()
```

### Comparing `roboflowoak-0.0.7/roboflowoak/postprocs.py` & `roboflowoak-0.0.8/roboflowoak/postprocs.py`

 * *Files identical despite different names*

### Comparing `roboflowoak-0.0.7/setup.py` & `roboflowoak-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 from setuptools import find_packages
 
 long_description = "https://docs.roboflow.com/inference/luxonis-oak"
 
 setuptools.setup(
     name="roboflowoak",  # Replace with your own username
-    version="0.0.7",
+    version="0.0.8",
     author="Roboflow",
     license='GPLv3+',
     author_email="jacob@roboflow.com",
     description="python client for deploying Roboflow models to OAK devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.roboflow.com",
```

