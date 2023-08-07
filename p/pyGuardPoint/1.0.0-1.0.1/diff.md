# Comparing `tmp/pyGuardPoint-1.0.0.tar.gz` & `tmp/pyGuardPoint-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-1.0.0.tar", last modified: Fri Aug  4 12:40:39 2023, max compression
+gzip compressed data, was "pyGuardPoint-1.0.1.tar", last modified: Mon Aug  7 09:56:05 2023, max compression
```

## Comparing `pyGuardPoint-1.0.0.tar` & `pyGuardPoint-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 12:40:39.113928 pyGuardPoint-1.0.0/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     6116 2023-08-04 12:40:39.113928 pyGuardPoint-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5857 2023-07-26 10:18:05.000000 pyGuardPoint-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-04 12:40:39.103820 pyGuardPoint-1.0.0/pyGuardPoint/
--rw-rw-rw-   0        0        0      290 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0     1229 2023-08-04 12:11:20.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    12153 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     1415 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cardholdertypes.py
--rw-rw-rw-   0        0        0     6900 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1385 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1408 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2648 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1500 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5584 2023-08-02 09:21:03.000000 pyGuardPoint-1.0.0/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-1.0.0/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2988 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0    10663 2023-07-31 14:11:21.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    17658 2023-05-12 10:58:18.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0      105 2023-08-04 12:11:20.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3140 2023-05-04 10:22:18.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 12:40:39.113928 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     6116 2023-08-04 12:40:39.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2023-08-04 12:40:39.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 12:40:39.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-08-04 12:40:39.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-04 12:40:39.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 12:40:39.113928 pyGuardPoint-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      565 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:56:05.144372 pyGuardPoint-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     6116 2023-08-07 09:56:05.144372 pyGuardPoint-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5857 2023-07-26 10:18:05.000000 pyGuardPoint-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-07 09:56:05.135373 pyGuardPoint-1.0.1/pyGuardPoint/
+-rw-rw-rw-   0        0        0      290 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.1/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0     1229 2023-08-04 12:11:20.000000 pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    12245 2023-08-07 09:55:49.000000 pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     1415 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_cardholdertypes.py
+-rw-rw-rw-   0        0        0     6900 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1385 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1408 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2648 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1500 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5584 2023-08-02 09:21:03.000000 pyGuardPoint-1.0.1/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-1.0.1/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2988 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.1/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-1.0.1/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0    10663 2023-07-31 14:11:21.000000 pyGuardPoint-1.0.1/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    17658 2023-05-12 10:58:18.000000 pyGuardPoint-1.0.1/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0      105 2023-08-04 12:11:20.000000 pyGuardPoint-1.0.1/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3140 2023-05-04 10:22:18.000000 pyGuardPoint-1.0.1/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:56:05.142376 pyGuardPoint-1.0.1/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0     6116 2023-08-07 09:56:05.000000 pyGuardPoint-1.0.1/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2023-08-07 09:56:05.000000 pyGuardPoint-1.0.1/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:56:05.000000 pyGuardPoint-1.0.1/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-1.0.1/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-08-07 09:56:05.000000 pyGuardPoint-1.0.1/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-07 09:56:05.000000 pyGuardPoint-1.0.1/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 09:56:05.144372 pyGuardPoint-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      565 2023-08-07 09:55:49.000000 pyGuardPoint-1.0.1/setup.py
```

### Comparing `pyGuardPoint-1.0.0/LICENSE.txt` & `pyGuardPoint-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/PKG-INFO` & `pyGuardPoint-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-1.0.0/README.rst` & `pyGuardPoint-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,27 @@
 
         code, json_body = self.gp_json_query("DELETE", url=(url + url_query_params))
         # Check response body is formatted correctly
         if json_body:
             GuardPointResponse.check_odata_body_structure(json_body)
 
         if code != 204:  # HTTP NO_CONTENT
-            if "errorMessages" in json_body:
-                raise GuardPointError(json_body["errorMessages"][0]["other"])
-            if 'error' in json_body:
-                raise GuardPointError(json_body['error'])
+            error_msg = ""
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    error_msg = json_body['error']
+                elif 'message' in json_body:
+                    error_msg = json_body['message']
+                else:
+                    error_msg = str(code)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             else:
-                raise GuardPointError(str(code))
+                raise GuardPointError(f"No body - ({code})")
 
 
         return True
 
     def update_card_holder_area(self, cardholder_uid: str, area: Area):
         if not validators.uuid(cardholder_uid):
             raise ValueError(f'Malformed Cardholder UID {cardholder_uid}')
@@ -79,17 +86,14 @@
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
             # 'IgnoreNonEditable': ''
         }
 
         code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
-        # Check response body is formatted correctly
-        if json_body:
-            GuardPointResponse.check_odata_body_structure(json_body)
 
         if code != 204:  # HTTP NO_CONTENT
             error_msg = ""
             if isinstance(json_body, dict):
                 if 'error' in json_body:
                     error_msg = json_body['error']
                 elif 'message' in json_body:
@@ -180,16 +184,16 @@
             raise ValueError(f'Malformed UID {uid}')
 
         url = "/odata/API_Cardholders"
         url_query_params = "(" + uid + ")?$select=photo"
 
         code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
         # Check response body is formatted correctly
-        if json_body:
-            GuardPointResponse.check_odata_body_structure(json_body)
+        #if json_body:
+        #    GuardPointResponse.check_odata_body_structure(json_body)
 
         if code != 200:
             error_msg = ""
             if isinstance(json_body, dict):
                 if 'error' in json_body:
                     error_msg = json_body['error']
 
@@ -212,16 +216,16 @@
                                        "cardholderCustomizedField," \
                                        "cardholderPersonalDetail," \
                                        "securityGroup," \
                                        "insideArea"
 
         code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
         # Check response body is formatted correctly
-        if json_body:
-            GuardPointResponse.check_odata_body_structure(json_body)
+        #if json_body:
+        #    GuardPointResponse.check_odata_body_structure(json_body)
 
         if code == 404: # Not Found
             return None
 
         if code != 200:
             error_msg = ""
             if isinstance(json_body, dict):
@@ -268,16 +272,16 @@
             url_query_params += "$count=true&$top=0"
         else:
             url_query_params += "$orderby=fromDateValid%20desc&"
             url_query_params += "$top=" + str(limit) + "&$skip=" + str(offset)
 
         code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
         # Check response body is formatted correctly
-        if json_body:
-            GuardPointResponse.check_odata_body_structure(json_body)
+        #if json_body:
+        #    GuardPointResponse.check_odata_body_structure(json_body)
 
         if code != 200:
             error_msg = ""
             if isinstance(json_body, dict):
                 if 'error' in json_body:
                     error_msg = json_body['error']
```

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cardholdertypes.py` & `pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_cardholdertypes.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-1.0.1/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-1.0.1/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-1.0.1/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/guardpoint.py` & `pyGuardPoint-1.0.1/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-1.0.1/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-1.0.1/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-1.0.1/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-1.0.1/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint.egg-info/PKG-INFO` & `pyGuardPoint-1.0.1/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-1.0.0/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-1.0.1/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-1.0.0/setup.py` & `pyGuardPoint-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
-      version="1.0.0",
+      version="1.0.1",
       author="John Owen",
       description="Python wrapper for GuardPoint 10 Access Control System",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'Levenshtein', 'cryptography'],
       packages=['pyGuardPoint'],
```

