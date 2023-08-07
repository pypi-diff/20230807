# Comparing `tmp/neurosity-2.0.1.tar.gz` & `tmp/neurosity-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurosity-2.0.1.tar", last modified: Mon Aug  7 01:16:16 2023, max compression
+gzip compressed data, was "neurosity-2.1.0.tar", last modified: Mon Aug  7 01:40:15 2023, max compression
```

## Comparing `neurosity-2.0.1.tar` & `neurosity-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 01:16:16.857097 neurosity-2.0.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1071 2023-08-07 00:20:59.000000 neurosity-2.0.1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)    30612 2023-08-07 01:16:16.850298 neurosity-2.0.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)    30192 2023-08-07 01:15:58.000000 neurosity-2.0.1/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 01:16:16.819628 neurosity-2.0.1/neurosity/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       60 2023-08-07 00:20:59.000000 neurosity-2.0.1/neurosity/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      651 2023-08-07 00:20:59.000000 neurosity-2.0.1/neurosity/config.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8093 2023-08-07 00:20:59.000000 neurosity-2.0.1/neurosity/neurosity.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 01:16:16.845697 neurosity-2.0.1/neurosity.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    30612 2023-08-07 01:16:16.000000 neurosity-2.0.1/neurosity.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-08-07 01:16:16.000000 neurosity-2.0.1/neurosity.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-08-07 01:16:16.000000 neurosity-2.0.1/neurosity.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       18 2023-08-07 01:16:16.000000 neurosity-2.0.1/neurosity.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-08-07 01:16:16.000000 neurosity-2.0.1/neurosity.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-08-07 01:16:16.857988 neurosity-2.0.1/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      714 2023-08-07 01:03:23.000000 neurosity-2.0.1/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 01:40:15.150667 neurosity-2.1.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1071 2023-08-07 00:20:59.000000 neurosity-2.1.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    30612 2023-08-07 01:40:15.149013 neurosity-2.1.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    30192 2023-08-07 01:33:47.000000 neurosity-2.1.0/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 01:40:14.963940 neurosity-2.1.0/neurosity/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       60 2023-08-07 00:20:59.000000 neurosity-2.1.0/neurosity/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      651 2023-08-07 00:20:59.000000 neurosity-2.1.0/neurosity/config.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8137 2023-08-07 01:38:08.000000 neurosity-2.1.0/neurosity/neurosity.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 01:40:15.143783 neurosity-2.1.0/neurosity.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    30612 2023-08-07 01:40:14.000000 neurosity-2.1.0/neurosity.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-08-07 01:40:14.000000 neurosity-2.1.0/neurosity.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-08-07 01:40:14.000000 neurosity-2.1.0/neurosity.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       18 2023-08-07 01:40:14.000000 neurosity-2.1.0/neurosity.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-08-07 01:40:14.000000 neurosity-2.1.0/neurosity.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-08-07 01:40:15.151367 neurosity-2.1.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      714 2023-08-07 01:37:02.000000 neurosity-2.1.0/setup.py
```

### Comparing `neurosity-2.0.1/LICENSE` & `neurosity-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neurosity-2.0.1/PKG-INFO` & `neurosity-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurosity
-Version: 2.0.1
+Version: 2.1.0
 Summary: Official Neurosity Python SDK
 Home-page: https://github.com/neurosity/neurosity-python-sdk
 Author: Alex Castillo
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neurosity-2.0.1/README.md` & `neurosity-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `neurosity-2.0.1/neurosity/config.py` & `neurosity-2.1.0/neurosity/config.py`

 * *Files identical despite different names*

### Comparing `neurosity-2.0.1/neurosity/neurosity.py` & `neurosity-2.1.0/neurosity/neurosity.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
     def exit_handler(self, signum=None, frame=None):
         self.remove_client()
         self.remove_all_subscriptions()
         signal.signal(signal.SIGTERM, signal.SIG_DFL)
         signal.signal(signal.SIGINT, signal.SIG_DFL)
         signal.signal(signal.SIGHUP, signal.SIG_DFL)
-        print("exit h")
         os.kill(os.getpid(), signal.SIGTERM)
         
     def get_server_timestamp(self):
         return {".sv": "timestamp"}
 
     def login(self, credentials):
         if (hasattr(self, "user") and hasattr(self, "token")):
@@ -141,14 +140,16 @@
 
         initial_message = {}
 
         def stream_handler(message):
             if (message["path"] == "/"):
                 initial_message[message["stream_id"]] = message
                 full_payload = message["data"]
+                if full_payload == None:
+                    return
             else:
                 child = message["path"][1:]
                 full_payload = initial_message[message["stream_id"]]["data"]
                 if (message["data"] == None):
                     # delete key is value is `None`
                     full_payload.pop(child, None)
                 else:
```

### Comparing `neurosity-2.0.1/neurosity.egg-info/PKG-INFO` & `neurosity-2.1.0/neurosity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurosity
-Version: 2.0.1
+Version: 2.1.0
 Summary: Official Neurosity Python SDK
 Home-page: https://github.com/neurosity/neurosity-python-sdk
 Author: Alex Castillo
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neurosity-2.0.1/setup.py` & `neurosity-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='neurosity',
     py_modules=['neurosity'],
     packages=find_packages(),
-    version='2.0.1',
+    version='2.1.0',
     url='https://github.com/neurosity/neurosity-python-sdk',
     python_requires='>=3.8',
     description='Official Neurosity Python SDK',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alex Castillo',
     license='MIT',
```

