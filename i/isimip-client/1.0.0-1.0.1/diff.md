# Comparing `tmp/isimip-client-1.0.0.tar.gz` & `tmp/isimip-client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isimip-client-1.0.0.tar", last modified: Wed Aug  2 14:56:18 2023, max compression
+gzip compressed data, was "isimip-client-1.0.1.tar", last modified: Mon Aug  7 08:06:36 2023, max compression
```

## Comparing `isimip-client-1.0.0.tar` & `isimip-client-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-08-02 14:56:18.705223 isimip-client-1.0.0/
--rw-r--r--   0 jochen    (1000) staff       (20)     1102 2023-02-27 15:38:48.000000 isimip-client-1.0.0/LICENSE
--rw-r--r--   0 jochen    (1000) staff       (20)     4330 2023-08-02 14:56:18.705110 isimip-client-1.0.0/PKG-INFO
--rw-r--r--   0 jochen    (1000) staff       (20)     2318 2023-08-02 14:53:14.000000 isimip-client-1.0.0/README.md
-drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-08-02 14:56:18.704199 isimip-client-1.0.0/isimip_client/
--rw-r--r--   0 jochen    (1000) staff       (20)       32 2023-07-31 16:03:57.000000 isimip-client-1.0.0/isimip_client/__init__.py
--rw-r--r--   0 jochen    (1000) staff       (20)     7650 2022-06-12 17:04:53.000000 isimip-client-1.0.0/isimip_client/client.py
-drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-08-02 14:56:18.704968 isimip-client-1.0.0/isimip_client.egg-info/
--rw-r--r--   0 jochen    (1000) staff       (20)     4330 2023-08-02 14:56:18.000000 isimip-client-1.0.0/isimip_client.egg-info/PKG-INFO
--rw-r--r--   0 jochen    (1000) staff       (20)      266 2023-08-02 14:56:18.000000 isimip-client-1.0.0/isimip_client.egg-info/SOURCES.txt
--rw-r--r--   0 jochen    (1000) staff       (20)        1 2023-08-02 14:56:18.000000 isimip-client-1.0.0/isimip_client.egg-info/dependency_links.txt
--rw-r--r--   0 jochen    (1000) staff       (20)       42 2023-08-02 14:56:18.000000 isimip-client-1.0.0/isimip_client.egg-info/requires.txt
--rw-r--r--   0 jochen    (1000) staff       (20)       14 2023-08-02 14:56:18.000000 isimip-client-1.0.0/isimip_client.egg-info/top_level.txt
--rw-r--r--   0 jochen    (1000) staff       (20)      994 2023-08-02 14:50:42.000000 isimip-client-1.0.0/pyproject.toml
--rw-r--r--   0 jochen    (1000) staff       (20)       38 2023-08-02 14:56:18.705253 isimip-client-1.0.0/setup.cfg
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-08-07 08:06:36.358692 isimip-client-1.0.1/
+-rw-r--r--   0 jochen    (1000) staff       (20)     1102 2023-02-27 15:38:48.000000 isimip-client-1.0.1/LICENSE
+-rw-r--r--   0 jochen    (1000) staff       (20)     4777 2023-08-07 08:06:36.358587 isimip-client-1.0.1/PKG-INFO
+-rw-r--r--   0 jochen    (1000) staff       (20)     2765 2023-08-07 07:51:12.000000 isimip-client-1.0.1/README.md
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-08-07 08:06:36.357913 isimip-client-1.0.1/isimip_client/
+-rw-r--r--   0 jochen    (1000) staff       (20)       32 2023-08-07 07:42:01.000000 isimip-client-1.0.1/isimip_client/__init__.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     7155 2023-08-07 08:02:19.000000 isimip-client-1.0.1/isimip_client/client.py
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-08-07 08:06:36.358443 isimip-client-1.0.1/isimip_client.egg-info/
+-rw-r--r--   0 jochen    (1000) staff       (20)     4777 2023-08-07 08:06:36.000000 isimip-client-1.0.1/isimip_client.egg-info/PKG-INFO
+-rw-r--r--   0 jochen    (1000) staff       (20)      266 2023-08-07 08:06:36.000000 isimip-client-1.0.1/isimip_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)        1 2023-08-07 08:06:36.000000 isimip-client-1.0.1/isimip_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)       68 2023-08-07 08:06:36.000000 isimip-client-1.0.1/isimip_client.egg-info/requires.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)       14 2023-08-07 08:06:36.000000 isimip-client-1.0.1/isimip_client.egg-info/top_level.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)     1041 2023-08-07 07:50:44.000000 isimip-client-1.0.1/pyproject.toml
+-rw-r--r--   0 jochen    (1000) staff       (20)       38 2023-08-07 08:06:36.358725 isimip-client-1.0.1/setup.cfg
```

### Comparing `isimip-client-1.0.0/LICENSE` & `isimip-client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `isimip-client-1.0.0/PKG-INFO` & `isimip-client-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isimip-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: A thin client library to use the API of the ISIMIP repository using Python.
 Author-email: Jochen Klar <jochen.klar@pik-potsdam.de>
 Maintainer-email: Jochen Klar <jochen.klar@pik-potsdam.de>
 License: MIT License
         
         Copyright (c) 2022 Potsdam Institute for Climate Impact Research
         
@@ -37,14 +37,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: jupyter
 License-File: LICENSE
 
 isimip-client
 =============
 
+[![Latest release](https://shields.io/github/v/release/ISI-MIP/isimip-client)](https://github.com/ISI-MIP/isimip-client/releases)
+[![PyPI release](https://img.shields.io/pypi/v/isimip-client)](https://pypi.org/project/isimip-client/)
+[![Python Version](https://img.shields.io/badge/python->=3.8-blue)](https://www.python.org/)
+[![License](https://img.shields.io/badge/License-MIT-green)](https://github.com/ISI-MIP/isimip-qc/blob/master/LICENSE)
+
 A *thin* client library to use the API of the [ISIMIP repository](https://data.isimip.org) using Python.
 
 Setup
 -----
 
 The library is written in Python (> 3.6) uses only dependencies, which can be installed without administrator priviledges. The installation of Python (and its developing packages), however differs from operating system to operating system. Optional Git is needed if the application is installed directly from GitHub. The installation of Python 3 and Git for different plattforms is documented [here](https://github.com/ISI-MIP/isimip-utils/blob/master/docs/prerequisites.md).
```

### Comparing `isimip-client-1.0.0/README.md` & `isimip-client-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 isimip-client
 =============
 
+[![Latest release](https://shields.io/github/v/release/ISI-MIP/isimip-client)](https://github.com/ISI-MIP/isimip-client/releases)
+[![PyPI release](https://img.shields.io/pypi/v/isimip-client)](https://pypi.org/project/isimip-client/)
+[![Python Version](https://img.shields.io/badge/python->=3.8-blue)](https://www.python.org/)
+[![License](https://img.shields.io/badge/License-MIT-green)](https://github.com/ISI-MIP/isimip-qc/blob/master/LICENSE)
+
 A *thin* client library to use the API of the [ISIMIP repository](https://data.isimip.org) using Python.
 
 Setup
 -----
 
 The library is written in Python (> 3.6) uses only dependencies, which can be installed without administrator priviledges. The installation of Python (and its developing packages), however differs from operating system to operating system. Optional Git is needed if the application is installed directly from GitHub. The installation of Python 3 and Git for different plattforms is documented [here](https://github.com/ISI-MIP/isimip-utils/blob/master/docs/prerequisites.md).
```

### Comparing `isimip-client-1.0.0/isimip_client/client.py` & `isimip-client-1.0.1/isimip_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,38 +161,28 @@
             payload['country'] = country
         elif bbox is not None:
             payload['task'] = 'mask_bbox'
             payload['bbox'] = bbox
         elif landonly is not None:
             payload['task'] = 'mask_landonly'
 
-        response = requests.post(self.files_api_url, json=payload, auth=self.auth, headers=self.headers)
-        job = self.parse_response(response)
-        if poll:
-            return self.poll(job, self.mask, [paths, country, bbox, landonly, poll], poll)
-        else:
-            return job
+        return self.post_job(payload, poll)
 
     def cutout(self, paths, bbox, poll=None):
         payload = {
             'task': 'cutout_bbox',
             'bbox': bbox
         }
 
         if isinstance(paths, list):
             payload['paths'] = paths
         else:
             payload['paths'] = [paths]
 
-        response = requests.post(self.files_api_url, json=payload, auth=self.auth, headers=self.headers)
-        job = self.parse_response(response)
-        if poll:
-            return self.poll(job, self.cutout, [paths, bbox, poll], poll)
-        else:
-            return job
+        return self.post_job(payload, poll)
 
     def select(self, paths, country=None, bbox=None, point=None, poll=None):
         payload = {}
 
         if isinstance(paths, list):
             payload['paths'] = paths
         else:
@@ -204,21 +194,21 @@
         elif bbox is not None:
             payload['task'] = 'select_bbox'
             payload['bbox'] = bbox
         elif point is not None:
             payload['task'] = 'select_point'
             payload['point'] = point
 
-        response = requests.post(self.files_api_url, json=payload, auth=self.auth, headers=self.headers)
-        job = self.parse_response(response)
-        if poll:
-            return self.poll(job, self.select, [paths, country, bbox, point, poll], poll)
-        else:
-            return job
+        return self.post_job(payload, poll)
 
-    def poll(self, job, method, args, poll_sleep):
-        print('job', job['id'], job['status'], job['meta'] if job['meta'] else '')
-        if job['status'] in ['queued', 'started']:
-            time.sleep(poll_sleep)
-            return method(*args)
-        else:
-            return job
+    def post_job(self, payload, poll=None):
+        while True:
+            response = requests.post(self.files_api_url, json=payload, auth=self.auth, headers=self.headers)
+            job = self.parse_response(response)
+            if poll:
+                print('job', job['id'], job['status'], job['meta'] if job['meta'] else '')
+                if job['status'] in ['queued', 'started']:
+                    time.sleep(poll)
+                else:
+                    return job
+            else:
+                return job
```

### Comparing `isimip-client-1.0.0/isimip_client.egg-info/PKG-INFO` & `isimip-client-1.0.1/isimip_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isimip-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: A thin client library to use the API of the ISIMIP repository using Python.
 Author-email: Jochen Klar <jochen.klar@pik-potsdam.de>
 Maintainer-email: Jochen Klar <jochen.klar@pik-potsdam.de>
 License: MIT License
         
         Copyright (c) 2022 Potsdam Institute for Climate Impact Research
         
@@ -37,14 +37,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: jupyter
 License-File: LICENSE
 
 isimip-client
 =============
 
+[![Latest release](https://shields.io/github/v/release/ISI-MIP/isimip-client)](https://github.com/ISI-MIP/isimip-client/releases)
+[![PyPI release](https://img.shields.io/pypi/v/isimip-client)](https://pypi.org/project/isimip-client/)
+[![Python Version](https://img.shields.io/badge/python->=3.8-blue)](https://www.python.org/)
+[![License](https://img.shields.io/badge/License-MIT-green)](https://github.com/ISI-MIP/isimip-qc/blob/master/LICENSE)
+
 A *thin* client library to use the API of the [ISIMIP repository](https://data.isimip.org) using Python.
 
 Setup
 -----
 
 The library is written in Python (> 3.6) uses only dependencies, which can be installed without administrator priviledges. The installation of Python (and its developing packages), however differs from operating system to operating system. Optional Git is needed if the application is installed directly from GitHub. The installation of Python 3 and Git for different plattforms is documented [here](https://github.com/ISI-MIP/isimip-utils/blob/master/docs/prerequisites.md).
```

### Comparing `isimip-client-1.0.0/pyproject.toml` & `isimip-client-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 jupyter = [
     "jupyter",
     "jupyterlab",
+    "matplotlib",
+    "netCDF4",
+    "pandas",
 ]
 
 [project.urls]
 Repository = "https://github.com/ISI-MIP/isimip-client"
 
 [tool.setuptools]
 packages = ["isimip_client"]
```

