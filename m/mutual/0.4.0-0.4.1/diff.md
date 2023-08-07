# Comparing `tmp/mutual-0.4.0.tar.gz` & `tmp/mutual-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.4.0.tar", last modified: Sun Aug  6 15:45:03 2023, max compression
+gzip compressed data, was "mutual-0.4.1.tar", last modified: Mon Aug  7 16:14:30 2023, max compression
```

## Comparing `mutual-0.4.0.tar` & `mutual-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-06 15:45:03.581399 mutual-0.4.0/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.4.0/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)    10128 2023-08-06 15:45:03.581136 mutual-0.4.0/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     9701 2023-08-06 15:41:03.000000 mutual-0.4.0/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-06 15:45:03.576717 mutual-0.4.0/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)     4365 2023-08-06 15:33:15.000000 mutual-0.4.0/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-06 15:45:03.580787 mutual-0.4.0/mutual/api_resources/
--rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-08-02 06:46:48.000000 mutual-0.4.0/mutual/api_resources/APIKey.py
--rw-r--r--   0 alexbetita   (501) staff       (20)    14003 2023-08-06 15:33:02.000000 mutual-0.4.0/mutual/api_resources/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4988 2023-08-04 07:23:14.000000 mutual-0.4.0/mutual/api_resources/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.4.0/mutual/api_resources/Dev.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.4.0/mutual/api_resources/Judge.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.4.0/mutual/api_resources/JudgeMessage.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.4.0/mutual/api_resources/Material.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     2995 2023-07-30 03:48:40.000000 mutual-0.4.0/mutual/api_resources/Memory.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.4.0/mutual/api_resources/Prompt.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      358 2023-08-04 02:43:31.000000 mutual-0.4.0/mutual/api_resources/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-06 15:45:03.577632 mutual-0.4.0/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)    10128 2023-08-06 15:45:03.000000 mutual-0.4.0/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      509 2023-08-06 15:45:03.000000 mutual-0.4.0/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-08-06 15:45:03.000000 mutual-0.4.0/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-08-06 15:45:03.000000 mutual-0.4.0/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-08-06 15:45:03.000000 mutual-0.4.0/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-08-06 15:45:03.581450 mutual-0.4.0/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-08-06 15:45:00.000000 mutual-0.4.0/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-07 16:14:30.394468 mutual-0.4.1/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.4.1/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)    10128 2023-08-07 16:14:30.394061 mutual-0.4.1/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     9701 2023-08-06 15:41:03.000000 mutual-0.4.1/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-07 16:14:30.389680 mutual-0.4.1/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4365 2023-08-07 16:14:05.000000 mutual-0.4.1/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-07 16:14:30.393735 mutual-0.4.1/mutual/api_resources/
+-rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-08-02 06:46:48.000000 mutual-0.4.1/mutual/api_resources/APIKey.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)    14259 2023-08-07 16:11:03.000000 mutual-0.4.1/mutual/api_resources/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4988 2023-08-04 07:23:14.000000 mutual-0.4.1/mutual/api_resources/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.4.1/mutual/api_resources/Dev.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.4.1/mutual/api_resources/Judge.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.4.1/mutual/api_resources/JudgeMessage.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.4.1/mutual/api_resources/Material.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3109 2023-08-07 16:11:47.000000 mutual-0.4.1/mutual/api_resources/Memory.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.4.1/mutual/api_resources/Prompt.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      358 2023-08-04 02:43:31.000000 mutual-0.4.1/mutual/api_resources/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-08-07 16:14:30.390670 mutual-0.4.1/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)    10128 2023-08-07 16:14:30.000000 mutual-0.4.1/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      509 2023-08-07 16:14:30.000000 mutual-0.4.1/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-08-07 16:14:30.000000 mutual-0.4.1/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-08-07 16:14:30.000000 mutual-0.4.1/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-08-07 16:14:30.000000 mutual-0.4.1/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-08-07 16:14:30.394519 mutual-0.4.1/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-08-07 16:07:33.000000 mutual-0.4.1/setup.py
```

### Comparing `mutual-0.4.0/LICENSE.txt` & `mutual-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.4.0/PKG-INFO` & `mutual-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutual-0.4.0/README.md` & `mutual-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mutual-0.4.0/mutual/__init__.py` & `mutual-0.4.1/mutual/__init__.py`

 * *Files identical despite different names*

### Comparing `mutual-0.4.0/mutual/api_resources/APIKey.py` & `mutual-0.4.1/mutual/api_resources/APIKey.py`

 * *Files identical despite different names*

### Comparing `mutual-0.4.0/mutual/api_resources/Bot.py` & `mutual-0.4.1/mutual/api_resources/Bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,51 +37,53 @@
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
 
 def create_bot(bot_name=None, prompt=None, prompt_id = "default", judge_id="default", 
-            judge_message_id="default", materiald_id="default", template=None):
+            judge_message_id="default", materiald_id="default", template=None, subject=None):
     
     url = f"{mutual.endpoint}/bots"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "bot_name": bot_name,
         "prompt": prompt,
         "prompt_id": prompt_id or "default",
         "judge_id": judge_id or "default",
         "judge_message_id": judge_message_id or "default",
         "material_id": materiald_id or "default",
-        "template": template
+        "template": template,
+        "subject": subject
     }
     response = requests.post(url, data=json.dumps(data), headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
 
 def update_bot(bot_id=None, bot_name=None, prompt_id=None, judge_id=None, 
-               judge_message_id=None, material_id=None):
+               judge_message_id=None, material_id=None, subject=None):
     
     url = f"{mutual.endpoint}/bots/{str(bot_id)}"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "bot_name": bot_name,
         "prompt_id": prompt_id,
         "judge_id": judge_id,
         "judge_message_id": judge_message_id,
-        "material_id": material_id
+        "material_id": material_id,
+        "subject": subject
     }
     # remove keys with None value
     data = {k: v for k, v in data.items() if v is not None}
     response = requests.patch(url, data=json.dumps(data), headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
@@ -124,28 +126,29 @@
                             "user_data": {
                                 "username": None,
                                 "tokens_used" : None
                             }
                         },
                     }
 
-    def update_bot(self,  bot_name=None, prompt=None, prompt_id=None, judge_id=None, judge_message_id=None, material_id=None):
+    def update_bot(self,  bot_name=None, prompt=None, prompt_id=None, judge_id=None, judge_message_id=None, material_id=None, subject=None):
         url = f"{mutual.endpoint}/bots/{str(self.bot_id)}"
 
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}"
         }
         data = {
             "bot_name": bot_name,
             "prompt": prompt,
             "prompt_id": prompt_id,
             "judge_id" : judge_id,
             "judge_message_id" : judge_message_id,
-            "material_id": material_id
+            "material_id": material_id,
+            "subject": subject
         }
         # remove keys with None value
         data = {k: v for k, v in data.items() if v is not None}
         response = requests.patch(url, data=json.dumps(data), headers=headers)
         if response.status_code < 300:
             return response.json()
         else:
@@ -255,47 +258,50 @@
         response = requests.get(url, headers=headers)
 
         if response.status_code < 300:
             return response.json()
         else:
             return f"Request failed with status code {response.status_code}, with an Error Message: {response.text}"
 
-    def feed(self, source: Union[str, List[str], Tuple[str, bytes]] = None):
+    def feed(self, source: Union[str, List[str], Tuple[str, bytes]] = None, subject=None):
         url = f"{mutual.endpoint}/memories/{self.bot_id}"
         url_text = f"{mutual.endpoint}/memories/{self.bot_id}/text"
         headers = {
             "Authorization": f"Bearer {mutual.api_key}"
         }
         # Check if the source is a file or a list of strings
  
         if isinstance(source, str):  # Source is a file path
             # Open the file in binary mode
             with open(source, 'rb') as file:
                 # Prepare the data payload
                 data = {
-                    'file': file
+                    'file': file,
+                    'subject': subject
                 }
                 # Send the POST request
                 response = requests.post(url, files=data, headers=headers)
 
         elif isinstance(source, list):  # Source is a list of strings
             # Prepare the data payload
             data = {
-                'data': source
+                'data': source,
+                'subject': subject
             }
             # Convert data to json format
             data = json.dumps(data)
             # Send the POST request
             response = requests.post(url_text, data=data, headers=headers)
 
         elif isinstance(source, tuple):  # Source is (filename, file content)
             filename, file_content = source
             # Prepare the data payload
             data = {
-                'file': (filename, io.BytesIO(file_content))  # Create a tuple (filename, file-like object)
+                'file': (filename, io.BytesIO(file_content)),  # Create a tuple (filename, file-like object)
+                'subject': subject
             }
             # Send the POST request
             response = requests.post(url, files=data, headers=headers)
 
         else:
             return "The source type is not supported"
```

### Comparing `mutual-0.4.0/mutual/api_resources/Chat.py` & `mutual-0.4.1/mutual/api_resources/Chat.py`

 * *Files identical despite different names*

### Comparing `mutual-0.4.0/mutual/api_resources/Dev.py` & `mutual-0.4.1/mutual/api_resources/Dev.py`

 * *Files identical despite different names*

### Comparing `mutual-0.4.0/mutual/api_resources/Judge.py` & `mutual-0.4.1/mutual/api_resources/Judge.py`

 * *Files identical despite different names*

### Comparing `mutual-0.4.0/mutual/api_resources/JudgeMessage.py` & `mutual-0.4.1/mutual/api_resources/JudgeMessage.py`

 * *Files identical despite different names*

### Comparing `mutual-0.4.0/mutual/api_resources/Material.py` & `mutual-0.4.1/mutual/api_resources/Material.py`

 * *Files identical despite different names*

### Comparing `mutual-0.4.0/mutual/api_resources/Memory.py` & `mutual-0.4.1/mutual/api_resources/Memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import requests
 import json
 import mutual
 import io
 from typing import List, Union, Tuple
 
-def feed(self, source: Union[str, List[str], Tuple[str, bytes]] = None):
+def feed(self, source: Union[str, List[str], Tuple[str, bytes]] = None, subject=None):
     url = f"{mutual.endpoint}/memories/{self.bot_id}"
     url_text = f"{mutual.endpoint}/memories/{self.bot_id}/text"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     # Check if the source is a file or a list of strings
     if isinstance(source, str):  # Source is a file path
         # Open the file in binary mode
         with open(source, 'rb') as file:
             # Prepare the data payload
             data = {
-                'file': file
+                'file': file,
+                'subject': subject
             }
             # Send the POST request
             response = requests.post(url, files=data, headers=headers)
 
     elif isinstance(source, list):  # Source is a list of strings
         # Prepare the data payload
         data = {
-            'data': source
+            'data': source,
+            'subject': subject
         }
         # Convert data to json format
         data = json.dumps(data)
         # Send the POST request
         response = requests.post(url_text, data=data, headers=headers)
 
     elif isinstance(source, tuple):  # Source is (filename, file content)
         filename, file_content = source
         # Prepare the data payload
         data = {
-            'file': (filename, io.BytesIO(file_content))  # Create a tuple (filename, file-like object)
+            'file': (filename, io.BytesIO(file_content)),  # Create a tuple (filename, file-like object)
+            'subject': subject
         }
         # Send the POST request
         response = requests.post(url, files=data, headers=headers)
 
     else:
         return "The source type is not supported"
```

### Comparing `mutual-0.4.0/mutual/api_resources/Prompt.py` & `mutual-0.4.1/mutual/api_resources/Prompt.py`

 * *Files identical despite different names*

### Comparing `mutual-0.4.0/mutual.egg-info/PKG-INFO` & `mutual-0.4.1/mutual.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutual-0.4.0/setup.py` & `mutual-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.4.0',  # beta
+    version='0.4.1',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

