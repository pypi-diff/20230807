# Comparing `tmp/prelude-sdk-1.3.4.tar.gz` & `tmp/prelude-sdk-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.3.4.tar", last modified: Tue Aug  1 15:17:51 2023, max compression
+gzip compressed data, was "prelude-sdk-1.3.5.tar", last modified: Mon Aug  7 20:23:04 2023, max compression
```

## Comparing `prelude-sdk-1.3.4.tar` & `prelude-sdk-1.3.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.503397 prelude-sdk-1.3.4/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.3.4/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-08-01 15:17:51.503448 prelude-sdk-1.3.4/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.3.4/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.497575 prelude-sdk-1.3.4/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.4/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.500501 prelude-sdk-1.3.4/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2484 2023-07-26 15:41:33.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5566 2023-07-26 15:41:33.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3731 2023-07-26 15:41:33.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     2113 2023-07-31 17:07:15.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.3.4/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.501308 prelude-sdk-1.3.4/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.4/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude-sdk-1.3.4/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     3627 2023-08-01 15:12:48.000000 prelude-sdk-1.3.4/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.498106 prelude-sdk-1.3.4/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-08-01 15:17:51.000000 prelude-sdk-1.3.4/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      773 2023-08-01 15:17:51.000000 prelude-sdk-1.3.4/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-08-01 15:17:51.000000 prelude-sdk-1.3.4/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-08-01 15:17:51.000000 prelude-sdk-1.3.4/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-08-01 15:17:51.000000 prelude-sdk-1.3.4/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.3.4/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2023-08-01 15:17:51.503663 prelude-sdk-1.3.4/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.503075 prelude-sdk-1.3.4/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.4/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.3.4/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-01 15:17:51.503295 prelude-sdk-1.3.4/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.4/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2075 2023-06-06 22:22:58.000000 prelude-sdk-1.3.4/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5045 2023-06-06 22:22:58.000000 prelude-sdk-1.3.4/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3350 2023-06-07 19:10:37.000000 prelude-sdk-1.3.4/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.3.4/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:23:04.454424 prelude-sdk-1.3.5/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.3.5/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-08-07 20:23:04.454495 prelude-sdk-1.3.5/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.3.5/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:23:04.450376 prelude-sdk-1.3.5/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.5/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:23:04.452301 prelude-sdk-1.3.5/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.5/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2484 2023-07-26 15:41:33.000000 prelude-sdk-1.3.5/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5694 2023-08-07 19:56:56.000000 prelude-sdk-1.3.5/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3731 2023-07-26 15:41:33.000000 prelude-sdk-1.3.5/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     2113 2023-07-31 17:07:15.000000 prelude-sdk-1.3.5/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.3.5/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:23:04.452874 prelude-sdk-1.3.5/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.3.5/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude-sdk-1.3.5/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     3627 2023-08-01 15:12:48.000000 prelude-sdk-1.3.5/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:23:04.450941 prelude-sdk-1.3.5/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-08-07 20:23:04.000000 prelude-sdk-1.3.5/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      773 2023-08-07 20:23:04.000000 prelude-sdk-1.3.5/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-08-07 20:23:04.000000 prelude-sdk-1.3.5/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-08-07 20:23:04.000000 prelude-sdk-1.3.5/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-08-07 20:23:04.000000 prelude-sdk-1.3.5/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.3.5/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2023-08-07 20:23:04.454746 prelude-sdk-1.3.5/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:23:04.454124 prelude-sdk-1.3.5/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.5/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.3.5/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-08-07 20:23:04.454335 prelude-sdk-1.3.5/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.3.5/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2075 2023-06-06 22:22:58.000000 prelude-sdk-1.3.5/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5045 2023-06-06 22:22:58.000000 prelude-sdk-1.3.5/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3350 2023-06-07 19:10:37.000000 prelude-sdk-1.3.5/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.3.5/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-1.3.4/LICENSE` & `prelude-sdk-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/PKG-INFO` & `prelude-sdk-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.3.4
+Version: 1.3.5
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.3.4/README.md` & `prelude-sdk-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-1.3.5/prelude_sdk/controllers/build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.3.5/prelude_sdk/controllers/detect_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,38 +5,40 @@
 
 class DetectController:
 
     def __init__(self, account):
         self.account = account
 
     @verify_credentials
-    def register_endpoint(self, host, serial_num, edr_id='', tags=None):
+    def register_endpoint(self, host, serial_num, edr_id='', partner_code=0, tags=None):
         """ Register (or re-register) an endpoint to your account """
-        body = dict(id=f'{host}:{serial_num}:{edr_id}')
+        body = dict(id=f'{host}:{serial_num}:{edr_id}:{partner_code}')
         if tags:
             body['tags'] = tags
 
         res = requests.post(
             f'{self.account.hq}/detect/endpoint',
             headers=self.account.headers,
             json=body,
             timeout=10
         )
         if res.status_code == 200:
             return res.text
         raise Exception(res.text)
 
     @verify_credentials
-    def update_endpoint(self, endpoint_id, host=None, edr_id=None, tags=None):
+    def update_endpoint(self, endpoint_id, host=None, edr_id=None, partner_code=0, tags=None):
         """ Update an endpoint in your account """
         body = dict()
         if host:
             body['host'] = host
         if edr_id is not None:
-            body['edr_id'] = edr_id
+            body['edr_id'] = edr_id or None
+        if partner_code != 0:
+            body['control'] = partner_code
         if tags is not None:
             body['tags'] = tags
 
         res = requests.post(
             f'{self.account.hq}/detect/endpoint/{endpoint_id}',
             headers=self.account.headers,
             json=body,
```

### Comparing `prelude-sdk-1.3.4/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-1.3.5/prelude_sdk/controllers/iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/prelude_sdk/controllers/partner_controller.py` & `prelude-sdk-1.3.5/prelude_sdk/controllers/partner_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/prelude_sdk/models/account.py` & `prelude-sdk-1.3.5/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/prelude_sdk/models/codes.py` & `prelude-sdk-1.3.5/prelude_sdk/models/codes.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.3.5/prelude_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.3.4
+Version: 1.3.5
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.3.4/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.3.5/prelude_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/setup.cfg` & `prelude-sdk-1.3.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.3.4
+version = 1.3.5
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.3.4/tests/conftest.py` & `prelude-sdk-1.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/tests/test_build_controller.py` & `prelude-sdk-1.3.5/tests/test_build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/tests/test_detect_controller.py` & `prelude-sdk-1.3.5/tests/test_detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/tests/test_iam_controller.py` & `prelude-sdk-1.3.5/tests/test_iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.3.4/tests/test_probe_controller.py` & `prelude-sdk-1.3.5/tests/test_probe_controller.py`

 * *Files identical despite different names*

