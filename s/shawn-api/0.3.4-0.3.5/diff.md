# Comparing `tmp/shawn_api-0.3.4.tar.gz` & `tmp/shawn_api-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shawn_api-0.3.4.tar", last modified: Fri Aug  4 09:53:11 2023, max compression
+gzip compressed data, was "shawn_api-0.3.5.tar", last modified: Mon Aug  7 07:28:22 2023, max compression
```

## Comparing `shawn_api-0.3.4.tar` & `shawn_api-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 09:53:11.987006 shawn_api-0.3.4/
--rw-rw-rw-   0        0        0      651 2023-08-04 09:53:11.986006 shawn_api-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-04 09:53:11.987006 shawn_api-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      901 2023-08-04 09:53:09.000000 shawn_api-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 09:53:11.974006 shawn_api-0.3.4/shawn_api/
--rw-rw-rw-   0        0        0        0 2023-08-04 09:49:32.000000 shawn_api-0.3.4/shawn_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 09:53:11.985006 shawn_api-0.3.4/shawn_api/models/
--rw-rw-rw-   0        0        0       33 2023-08-04 08:38:38.000000 shawn_api-0.3.4/shawn_api/models/__init__.py
--rw-rw-rw-   0        0        0     1469 2023-08-04 08:58:38.000000 shawn_api-0.3.4/shawn_api/models/chat.py
--rw-rw-rw-   0        0        0      148 2023-08-04 08:38:38.000000 shawn_api-0.3.4/shawn_api/models/model.py
-drwxrwxrwx   0        0        0        0 2023-08-04 09:53:11.981006 shawn_api-0.3.4/shawn_api.egg-info/
--rw-rw-rw-   0        0        0      651 2023-08-04 09:53:11.000000 shawn_api-0.3.4/shawn_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-08-04 09:53:11.000000 shawn_api-0.3.4/shawn_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 09:53:11.000000 shawn_api-0.3.4/shawn_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-08-04 09:53:11.000000 shawn_api-0.3.4/shawn_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-04 09:53:11.000000 shawn_api-0.3.4/shawn_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 07:28:22.520354 shawn_api-0.3.5/
+-rw-rw-rw-   0        0        0      651 2023-08-07 07:28:22.519352 shawn_api-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-07 07:28:22.520354 shawn_api-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-08-07 07:28:21.000000 shawn_api-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:28:22.506354 shawn_api-0.3.5/shawn_api/
+-rw-rw-rw-   0        0        0        0 2023-08-04 09:49:32.000000 shawn_api-0.3.5/shawn_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:28:22.518376 shawn_api-0.3.5/shawn_api/models/
+-rw-rw-rw-   0        0        0       33 2023-08-04 08:38:38.000000 shawn_api-0.3.5/shawn_api/models/__init__.py
+-rw-rw-rw-   0        0        0     1416 2023-08-07 07:26:58.000000 shawn_api-0.3.5/shawn_api/models/chat.py
+-rw-rw-rw-   0        0        0      148 2023-08-04 08:38:38.000000 shawn_api-0.3.5/shawn_api/models/model.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:28:22.514388 shawn_api-0.3.5/shawn_api.egg-info/
+-rw-rw-rw-   0        0        0      651 2023-08-07 07:28:22.000000 shawn_api-0.3.5/shawn_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-08-07 07:28:22.000000 shawn_api-0.3.5/shawn_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:28:22.000000 shawn_api-0.3.5/shawn_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-07 07:28:22.000000 shawn_api-0.3.5/shawn_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-07 07:28:22.000000 shawn_api-0.3.5/shawn_api.egg-info/top_level.txt
```

### Comparing `shawn_api-0.3.4/PKG-INFO` & `shawn_api-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shawn_api
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python library for shawn test api
 Author: Shawn-Tam
 Author-email: shawn@dcoean.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `shawn_api-0.3.4/setup.py` & `shawn_api-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from setuptools import setup
 
-
 setup(
     name="shawn_api",
-    version="0.3.4",
+    version="0.3.5",
     description="A Python library for shawn test api",
     author="Shawn-Tam",
     author_email="shawn@dcoean.ai",
     packages=["shawn_api", "shawn_api.models"],
     install_requires=[
         "requests",
-        "aiohttp",
+        "httpx",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",  # or "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

### Comparing `shawn_api-0.3.4/shawn_api/models/chat.py` & `shawn_api-0.3.5/shawn_api/models/chat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-import aiohttp
 import requests
 from typing import Optional
+from ..utils.http_request import post_request
+
 
 class Chat:
     headers: Optional[dict] = {}
-    base_url: Optional[str] = "https://test.api.anyask.ai.:8888"
+    base_url: Optional[str] = "https://test.api.anyask.ai"
     path_messages: Optional[str] = "/chat/messages"
 
     def messages(self, data) -> str:
         if data.get('stream'):
             raise Exception("Don't support stream'")
         resp = requests.post(
             url=self.base_url + self.path_messages,
             headers=self.headers,
             json=data
         )
-        if resp.status_code >= 200 and resp.status_code < 300:
+        if 200 <= resp.status_code < 300:
             resp = resp.json()
             content = resp.get("choices")[0].get("message", {}).get("content", "")
             if content == "":
                 content = resp.get("choices")[0].get("delta", {}).get("content", "")
             return content
         else:
             return resp.text
 
     async def amessages(self, data: dict) -> str:
         if data.get('stream'):
             raise Exception("Don't support stream'")
-        async with aiohttp.ClientSession(self.base_url) as session:
-            async with session.post(self.path_messages, json=data) as resp:
-                chat_msg: dict = await resp.json()
-                content = chat_msg.get("choices")[0].get("message", {}).get("content", "")
-                if content == "":
-                    content = chat_msg.get("choices")[0].get("delta", {}).get("content", "")
-                return content
+        url = f"{self.base_url}{self.path_messages}"
+        resp = await post_request(url, headers=self.headers, data=data)
+        chat_msg: dict = await resp.json()
+        content = chat_msg.get("choices")[0].get("message", {}).get("content", "")
+        if content == "":
+            content = chat_msg.get("choices")[0].get("delta", {}).get("content", "")
+        return content
```

### Comparing `shawn_api-0.3.4/shawn_api.egg-info/PKG-INFO` & `shawn_api-0.3.5/shawn_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shawn-api
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python library for shawn test api
 Author: Shawn-Tam
 Author-email: shawn@dcoean.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

