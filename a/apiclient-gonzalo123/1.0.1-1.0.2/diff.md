# Comparing `tmp/apiclient-gonzalo123-1.0.1.tar.gz` & `tmp/apiclient-gonzalo123-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiclient-gonzalo123-1.0.1.tar", last modified: Fri Aug  4 13:00:17 2023, max compression
+gzip compressed data, was "apiclient-gonzalo123-1.0.2.tar", last modified: Mon Aug  7 08:05:09 2023, max compression
```

## Comparing `apiclient-gonzalo123-1.0.1.tar` & `apiclient-gonzalo123-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-04 13:00:17.031298 apiclient-gonzalo123-1.0.1/
--rw-r--r--   0 gonzalo    (501) staff       (20)     1045 2023-08-04 13:00:17.031103 apiclient-gonzalo123-1.0.1/PKG-INFO
--rw-r--r--   0 gonzalo    (501) staff       (20)      610 2023-08-03 12:22:33.000000 apiclient-gonzalo123-1.0.1/README.md
-drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-04 13:00:17.029707 apiclient-gonzalo123-1.0.1/apiclient/
--rw-r--r--   0 gonzalo    (501) staff       (20)       52 2023-08-03 09:53:01.000000 apiclient-gonzalo123-1.0.1/apiclient/__init__.py
--rw-r--r--   0 gonzalo    (501) staff       (20)     1288 2023-08-04 12:58:12.000000 apiclient-gonzalo123-1.0.1/apiclient/apiclient.py
-drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-04 13:00:17.030868 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/
--rw-r--r--   0 gonzalo    (501) staff       (20)     1045 2023-08-04 13:00:17.000000 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/PKG-INFO
--rw-r--r--   0 gonzalo    (501) staff       (20)      282 2023-08-04 13:00:17.000000 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/SOURCES.txt
--rw-r--r--   0 gonzalo    (501) staff       (20)        1 2023-08-04 13:00:17.000000 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/dependency_links.txt
--rw-r--r--   0 gonzalo    (501) staff       (20)       16 2023-08-04 13:00:17.000000 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/requires.txt
--rw-r--r--   0 gonzalo    (501) staff       (20)       10 2023-08-04 13:00:17.000000 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/top_level.txt
--rw-r--r--   0 gonzalo    (501) staff       (20)       38 2023-08-04 13:00:17.031338 apiclient-gonzalo123-1.0.1/setup.cfg
--rw-r--r--   0 gonzalo    (501) staff       (20)      816 2023-08-04 12:58:24.000000 apiclient-gonzalo123-1.0.1/setup.py
+drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-07 08:05:09.401669 apiclient-gonzalo123-1.0.2/
+-rw-r--r--   0 gonzalo    (501) staff       (20)     1045 2023-08-07 08:05:09.401513 apiclient-gonzalo123-1.0.2/PKG-INFO
+-rw-r--r--   0 gonzalo    (501) staff       (20)      610 2023-08-03 12:22:33.000000 apiclient-gonzalo123-1.0.2/README.md
+drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-07 08:05:09.400189 apiclient-gonzalo123-1.0.2/apiclient/
+-rw-r--r--   0 gonzalo    (501) staff       (20)       52 2023-08-03 09:53:01.000000 apiclient-gonzalo123-1.0.2/apiclient/__init__.py
+-rw-r--r--   0 gonzalo    (501) staff       (20)     1442 2023-08-07 08:03:05.000000 apiclient-gonzalo123-1.0.2/apiclient/apiclient.py
+drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-07 08:05:09.401305 apiclient-gonzalo123-1.0.2/apiclient_gonzalo123.egg-info/
+-rw-r--r--   0 gonzalo    (501) staff       (20)     1045 2023-08-07 08:05:09.000000 apiclient-gonzalo123-1.0.2/apiclient_gonzalo123.egg-info/PKG-INFO
+-rw-r--r--   0 gonzalo    (501) staff       (20)      282 2023-08-07 08:05:09.000000 apiclient-gonzalo123-1.0.2/apiclient_gonzalo123.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzalo    (501) staff       (20)        1 2023-08-07 08:05:09.000000 apiclient-gonzalo123-1.0.2/apiclient_gonzalo123.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzalo    (501) staff       (20)       16 2023-08-07 08:05:09.000000 apiclient-gonzalo123-1.0.2/apiclient_gonzalo123.egg-info/requires.txt
+-rw-r--r--   0 gonzalo    (501) staff       (20)       10 2023-08-07 08:05:09.000000 apiclient-gonzalo123-1.0.2/apiclient_gonzalo123.egg-info/top_level.txt
+-rw-r--r--   0 gonzalo    (501) staff       (20)       38 2023-08-07 08:05:09.401707 apiclient-gonzalo123-1.0.2/setup.cfg
+-rw-r--r--   0 gonzalo    (501) staff       (20)      816 2023-08-07 08:03:14.000000 apiclient-gonzalo123-1.0.2/setup.py
```

### Comparing `apiclient-gonzalo123-1.0.1/PKG-INFO` & `apiclient-gonzalo123-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiclient-gonzalo123
-Version: 1.0.1
+Version: 1.0.2
 Summary: apiclient
 Home-page: https://github.com/gonzalo123/apiclient
 Author: Gonzalo Ayuso
 Author-email: gonzalo123@gmail.com
 License: MIT
 Keywords: apiclient
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apiclient-gonzalo123-1.0.1/README.md` & `apiclient-gonzalo123-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `apiclient-gonzalo123-1.0.1/apiclient/apiclient.py` & `apiclient-gonzalo123-1.0.2/apiclient/apiclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import requests
 
 
 class ApiClientException(Exception):
     pass
 
 
+class ApiClientAuthException(Exception):
+    pass
+
+
 class ApiClient:
     def __init__(self, token, base):
         self.token = token
         self.base = base
 
     @staticmethod
     def _zip(columns, rows):
@@ -28,14 +32,16 @@
     def _process_response(self, response):
         if response.ok:
             data = response.json()
             if response.headers['x-recordset'] == 'compact':
                 return self._zip(*data)
             else:
                 return data
+        elif response.status_code == 401:
+            raise ApiClientAuthException('not valid token')
         else:
             raise ApiClientException(response.json())
 
     def get(self, uri, params):
         return self._process_response(requests.get(
             url=self._get_url(uri),
             params=params,
```

### Comparing `apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/PKG-INFO` & `apiclient-gonzalo123-1.0.2/apiclient_gonzalo123.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiclient-gonzalo123
-Version: 1.0.1
+Version: 1.0.2
 Summary: apiclient
 Home-page: https://github.com/gonzalo123/apiclient
 Author: Gonzalo Ayuso
 Author-email: gonzalo123@gmail.com
 License: MIT
 Keywords: apiclient
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apiclient-gonzalo123-1.0.1/setup.py` & `apiclient-gonzalo123-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup_args = dict(
     name="apiclient-gonzalo123",
-    version="1.0.1",
+    version="1.0.2",
     author="Gonzalo Ayuso",
     author_email="gonzalo123@gmail.com",
     description="apiclient",
     long_description=long_description,
     license='MIT',
     long_description_content_type="text/markdown",
     keywords=['apiclient'],
```

