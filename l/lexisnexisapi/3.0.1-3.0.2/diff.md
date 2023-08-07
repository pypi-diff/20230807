# Comparing `tmp/lexisnexisapi-3.0.1.tar.gz` & `tmp/lexisnexisapi-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexisnexisapi-3.0.1.tar", last modified: Fri Aug  4 20:31:44 2023, max compression
+gzip compressed data, was "lexisnexisapi-3.0.2.tar", last modified: Mon Aug  7 17:24:38 2023, max compression
```

## Comparing `lexisnexisapi-3.0.1.tar` & `lexisnexisapi-3.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-04 20:31:44.505852 lexisnexisapi-3.0.1/
--rw-r--r--   0 rwcuffney   (501) staff       (20)      466 2023-08-02 01:16:32.000000 lexisnexisapi-3.0.1/LICENSE.txt
--rw-r--r--   0 rwcuffney   (501) staff       (20)     6033 2023-08-04 20:31:44.505639 lexisnexisapi-3.0.1/PKG-INFO
--rw-r--r--   0 rwcuffney   (501) staff       (20)     5659 2023-08-03 15:24:28.000000 lexisnexisapi-3.0.1/README.md
--rw-r--r--   0 rwcuffney   (501) staff       (20)      618 2023-08-04 20:30:10.000000 lexisnexisapi-3.0.1/pyproject.toml
--rw-r--r--   0 rwcuffney   (501) staff       (20)       38 2023-08-04 20:31:44.505918 lexisnexisapi-3.0.1/setup.cfg
--rw-r--r--   0 rwcuffney   (501) staff       (20)      767 2023-08-04 20:29:23.000000 lexisnexisapi-3.0.1/setup.py
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-04 20:31:44.499226 lexisnexisapi-3.0.1/src/
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-04 20:31:44.502993 lexisnexisapi-3.0.1/src/lexisnexisapi/
--rw-r--r--   0 rwcuffney   (501) staff       (20)        0 2023-08-02 01:16:32.000000 lexisnexisapi-3.0.1/src/lexisnexisapi/__init__.py
--rw-r--r--   0 rwcuffney   (501) staff       (20)     2338 2023-08-02 20:21:18.000000 lexisnexisapi-3.0.1/src/lexisnexisapi/credentials.py
--rw-r--r--   0 rwcuffney   (501) staff       (20)     9718 2023-08-04 19:52:06.000000 lexisnexisapi-3.0.1/src/lexisnexisapi/metabase.py
--rw-r--r--   0 rwcuffney   (501) staff       (20)     2963 2023-08-04 20:27:36.000000 lexisnexisapi-3.0.1/src/lexisnexisapi/webservices.py
-drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-04 20:31:44.505197 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/
--rw-r--r--   0 rwcuffney   (501) staff       (20)     6148 2023-08-04 20:10:21.000000 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/.DS_Store
--rw-r--r--   0 rwcuffney   (501) staff       (20)     6033 2023-08-04 20:31:44.000000 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/PKG-INFO
--rw-r--r--   0 rwcuffney   (501) staff       (20)      372 2023-08-04 20:31:44.000000 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/SOURCES.txt
--rw-r--r--   0 rwcuffney   (501) staff       (20)        1 2023-08-04 20:31:44.000000 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/dependency_links.txt
--rw-r--r--   0 rwcuffney   (501) staff       (20)       14 2023-08-04 20:31:44.000000 lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/top_level.txt
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-07 17:24:38.170228 lexisnexisapi-3.0.2/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      466 2023-08-02 01:16:32.000000 lexisnexisapi-3.0.2/LICENSE.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     6033 2023-08-07 17:24:38.169875 lexisnexisapi-3.0.2/PKG-INFO
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     5659 2023-08-03 15:24:28.000000 lexisnexisapi-3.0.2/README.md
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      618 2023-08-07 17:11:46.000000 lexisnexisapi-3.0.2/pyproject.toml
+-rw-r--r--   0 rwcuffney   (501) staff       (20)       38 2023-08-07 17:24:38.170292 lexisnexisapi-3.0.2/setup.cfg
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      767 2023-08-07 17:12:03.000000 lexisnexisapi-3.0.2/setup.py
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-07 17:24:38.164360 lexisnexisapi-3.0.2/src/
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-07 17:24:38.167551 lexisnexisapi-3.0.2/src/lexisnexisapi/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)        0 2023-08-02 01:16:32.000000 lexisnexisapi-3.0.2/src/lexisnexisapi/__init__.py
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     2338 2023-08-02 20:21:18.000000 lexisnexisapi-3.0.2/src/lexisnexisapi/credentials.py
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     9718 2023-08-07 17:11:29.000000 lexisnexisapi-3.0.2/src/lexisnexisapi/metabase.py
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     3015 2023-08-07 17:14:51.000000 lexisnexisapi-3.0.2/src/lexisnexisapi/webservices.py
+drwxr-xr-x   0 rwcuffney   (501) staff       (20)        0 2023-08-07 17:24:38.169565 lexisnexisapi-3.0.2/src/lexisnexisapi.egg-info/
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     6148 2023-08-04 20:10:21.000000 lexisnexisapi-3.0.2/src/lexisnexisapi.egg-info/.DS_Store
+-rw-r--r--   0 rwcuffney   (501) staff       (20)     6033 2023-08-07 17:24:38.000000 lexisnexisapi-3.0.2/src/lexisnexisapi.egg-info/PKG-INFO
+-rw-r--r--   0 rwcuffney   (501) staff       (20)      372 2023-08-07 17:24:38.000000 lexisnexisapi-3.0.2/src/lexisnexisapi.egg-info/SOURCES.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)        1 2023-08-07 17:24:38.000000 lexisnexisapi-3.0.2/src/lexisnexisapi.egg-info/dependency_links.txt
+-rw-r--r--   0 rwcuffney   (501) staff       (20)       14 2023-08-07 17:24:38.000000 lexisnexisapi-3.0.2/src/lexisnexisapi.egg-info/top_level.txt
```

### Comparing `lexisnexisapi-3.0.1/PKG-INFO` & `lexisnexisapi-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexisnexisapi
-Version: 3.0.1
+Version: 3.0.2
 Summary: A module to support the lexisnexis metabase search api
 Home-page: 
 Author: Robert Cuffney
 Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
 License: MIT
 Keywords: example project
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lexisnexisapi-3.0.1/README.md` & `lexisnexisapi-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-3.0.1/pyproject.toml` & `lexisnexisapi-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexisnexisapi"
-version = "3.0.1"
+version = "3.0.2"
 authors = [{ name = "Robert Cuffney", email = "robert.cuffney@lexisnexis.com" },
 		   { name = "Ozgur Aycan", email = "ozgur.aycan@lexisnexis.co.uk" }
 ]
 description = "A module to support the lexisnexis metabase search api"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lexisnexisapi-3.0.1/setup.py` & `lexisnexisapi-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="lexisnexisapi",
-    version='3.0.1',
+    version='3.0.2',
     license='MIT',
     author="Robert Cuffney",
     author_email='robert.cuffney@lexisnexis.com',
     description = 'a module to support the lexisnexis metabase search api',
     long_description = ' module provides a Python interface to interact with the Metabase API. It allows you to perform searches and retrieve articles using the Metabase API. The module facilitates the creation of Python objects representing the API response, making it easy to work with the data.',
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `lexisnexisapi-3.0.1/src/lexisnexisapi/credentials.py` & `lexisnexisapi-3.0.2/src/lexisnexisapi/credentials.py`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-3.0.1/src/lexisnexisapi/metabase.py` & `lexisnexisapi-3.0.2/src/lexisnexisapi/metabase.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 from datetime import datetime
 from lexisnexisapi import credentials as cred
 import time
 import ast
 
 
-__version__ = '2.0'
+__version__ = '3.0.2'
 __author__ = "Robert Cuffney & Ozgur Aycan, CS Integration Consultants @ LexisNexis"
 
 #Constants are usually defined on a module level and written in all capital letters with underscores separating words. 
 #Examples include MAX_OVERFLOW and TOTAL.
 
 #url = 'http://metabase.moreover.com/api/v10/searchArticles?'
 
@@ -68,15 +68,15 @@
         creates a json file
         '''
         if self.totalResults != 0:
             with open(file, "w") as my_file:
                 my_file.write(json.dumps(self.articles, indent=4))
                 print(f'{len(self.articles)} article(s) successfully written to a file:{file}')
         else:
-            print("no articles to write to file!") =
+            print("no articles to write to file!")
 
 #### Below Functions, within this class, used only for FullDataSet
     @error_handler 
     def get_fulldataset(self):
         self.parameters.pop('sequence_id',"")                 #get rid of 'sequence_id' if it's there
         #self.parameters['limit']='1000'                       #This will set the limit to the maximum allowed per their key  
         t_lst =[]                                             #this will be the list of all articles
```

### Comparing `lexisnexisapi-3.0.1/src/lexisnexisapi/webservices.py` & `lexisnexisapi-3.0.2/src/lexisnexisapi/webservices.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,34 +5,40 @@
 import json
 import xmltodict
 import base64
 
 from lexisnexisapi import credentials as cred
 
 class APIEndpoints():
+    '''
+    Class of constants that stores the API endpoints
+    '''
     COMPANYANDFINANCIAL = 'https://services-api.lexisnexis.com/v1/CompanyAndFinancial?'
     COMPANYDOSSIERS = 'https://services-api.lexisnexis.com/v1/CompanyDossiers?'
     NEWS = 'https://services-api.lexisnexis.com/v1/News?'
     SOURCES = 'https://services-api.lexisnexis.com/v1/Sources?'
     DOCKETS = 'https://services-api.lexisnexis.com/v1/Dockets?'
     JURYVERDICTSANDSETTLEMENTS = 'https://services-api.lexisnexis.com/v1/JuryVerdictsSettlements?'
 
 def error_handler(func):
+    '''
+    generic error handling
+    '''
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Exception as e:
             print(f"Error occurred in function: '{func.__name__}'")
             print("error: {e}")
             print(f"args:{args}")
             print(f"kwargs:{kwargs}")
             raise  # Re-raise the exception to propagate it further
     return wrapper
 
-#@error_handler
+
 def token():
     """Gets Authorization token to use in other requests."""
     client_id = cred.get_Key('WSAPI_CLIENT_ID')
     secret = cred.get_Key('WSAPI_SECRET')
     auth_url = 'https://auth-api.lexisnexis.com/oauth/v2/token'
     payload = {
         'grant_type': 'client_credentials',
@@ -42,35 +48,35 @@
     headers = {'Content-Type': 'application/x-www-form-urlencoded'}
     
     response = requests.post(auth_url, auth=auth, headers=headers, data=payload)
     response.raise_for_status()  # Raise exception for bad status codes
     json_data = response.json()
     return json_data['access_token']
 
-#@error_handler
+@error_handler
 def call_api(access_token,endpoint, **kwargs):
-    """Call the API with the provided token in the Authorization header."""
+    """Call the API with the provided token and endpoint"""
     headers = {
         'Authorization': f'Bearer {access_token}',
         'Accept': 'application/json'
     }
     url =getattr(APIEndpoints(), endpoint)
     with requests.Session() as session:
         response = session.get(headers=headers,url=url,**kwargs)
         response.raise_for_status()  # Raise exception for bad status codes
         api_data = response.json()
         return api_data
 
-@error_handler
+
 def get_base64(message):
     base64_message = base64.b64encode(message.encode('ascii')).decode('ascii')
     return base64_message
 
 
-@error_handler
+
 def convert_xml_content(data):
     '''
     conversts the content section of the document to a 
     python dictionary
     '''
     for c in data['value']:
         myDoc = c['Document']['Content']
```

### Comparing `lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/.DS_Store` & `lexisnexisapi-3.0.2/src/lexisnexisapi.egg-info/.DS_Store`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-3.0.1/src/lexisnexisapi.egg-info/PKG-INFO` & `lexisnexisapi-3.0.2/src/lexisnexisapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexisnexisapi
-Version: 3.0.1
+Version: 3.0.2
 Summary: A module to support the lexisnexis metabase search api
 Home-page: 
 Author: Robert Cuffney
 Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
 License: MIT
 Keywords: example project
 Classifier: Programming Language :: Python :: 3
```

