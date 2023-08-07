# Comparing `tmp/jinaai-0.2.4.tar.gz` & `tmp/jinaai-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinaai-0.2.4.tar", last modified: Fri Jul 28 04:29:40 2023, max compression
+gzip compressed data, was "jinaai-0.2.5.tar", last modified: Mon Aug  7 10:26:05 2023, max compression
```

## Comparing `jinaai-0.2.4.tar` & `jinaai-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-28 04:29:40.627063 jinaai-0.2.4/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.2.4/LICENSE
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14695 2023-07-28 04:29:40.626874 jinaai-0.2.4/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14446 2023-07-25 06:20:32.000000 jinaai-0.2.4/README.md
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-28 04:29:40.624660 jinaai-0.2.4/jinaai/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     3411 2023-07-28 04:12:19.000000 jinaai-0.2.4/jinaai/__init__.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-28 04:29:40.626705 jinaai-0.2.4/jinaai/clients/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1670 2023-07-28 03:49:43.000000 jinaai-0.2.4/jinaai/clients/BestBannerClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1261 2023-07-28 04:07:41.000000 jinaai-0.2.4/jinaai/clients/HTTPClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1986 2023-07-28 04:17:10.000000 jinaai-0.2.4/jinaai/clients/JinaChatClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2125 2023-07-28 03:50:10.000000 jinaai-0.2.4/jinaai/clients/PromptPerfectClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1965 2023-07-28 03:51:28.000000 jinaai-0.2.4/jinaai/clients/RationaleClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2051 2023-07-28 03:51:56.000000 jinaai-0.2.4/jinaai/clients/SceneXClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.2.4/jinaai/clients/__init__.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.2.4/jinaai/utils.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-28 04:29:40.625311 jinaai-0.2.4/jinaai.egg-info/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14695 2023-07-28 04:29:40.000000 jinaai-0.2.4/jinaai.egg-info/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      437 2023-07-28 04:29:40.000000 jinaai-0.2.4/jinaai.egg-info/SOURCES.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-07-28 04:29:40.000000 jinaai-0.2.4/jinaai.egg-info/dependency_links.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        9 2023-07-28 04:29:40.000000 jinaai-0.2.4/jinaai.egg-info/requires.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-07-28 04:29:40.000000 jinaai-0.2.4/jinaai.egg-info/top_level.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-07-28 04:29:40.627107 jinaai-0.2.4/setup.cfg
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      508 2023-07-28 04:29:30.000000 jinaai-0.2.4/setup.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-08-07 10:26:05.816016 jinaai-0.2.5/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.2.5/LICENSE
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14856 2023-08-07 10:26:05.815820 jinaai-0.2.5/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14607 2023-08-07 09:55:26.000000 jinaai-0.2.5/README.md
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-08-07 10:26:05.813528 jinaai-0.2.5/jinaai/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     3411 2023-07-28 04:12:19.000000 jinaai-0.2.5/jinaai/__init__.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-08-07 10:26:05.815646 jinaai-0.2.5/jinaai/clients/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1670 2023-07-28 03:49:43.000000 jinaai-0.2.5/jinaai/clients/BestBannerClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1261 2023-07-28 04:07:41.000000 jinaai-0.2.5/jinaai/clients/HTTPClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2180 2023-08-07 10:24:45.000000 jinaai-0.2.5/jinaai/clients/JinaChatClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2125 2023-07-28 03:50:10.000000 jinaai-0.2.5/jinaai/clients/PromptPerfectClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1965 2023-07-28 03:51:28.000000 jinaai-0.2.5/jinaai/clients/RationaleClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2051 2023-07-28 03:51:56.000000 jinaai-0.2.5/jinaai/clients/SceneXClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.2.5/jinaai/clients/__init__.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1057 2023-08-07 10:20:49.000000 jinaai-0.2.5/jinaai/utils.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-08-07 10:26:05.814109 jinaai-0.2.5/jinaai.egg-info/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    14856 2023-08-07 10:26:05.000000 jinaai-0.2.5/jinaai.egg-info/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      437 2023-08-07 10:26:05.000000 jinaai-0.2.5/jinaai.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-08-07 10:26:05.000000 jinaai-0.2.5/jinaai.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        9 2023-08-07 10:26:05.000000 jinaai-0.2.5/jinaai.egg-info/requires.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-08-07 10:26:05.000000 jinaai-0.2.5/jinaai.egg-info/top_level.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-08-07 10:26:05.816061 jinaai-0.2.5/setup.cfg
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      508 2023-08-07 10:25:34.000000 jinaai-0.2.5/setup.py
```

### Comparing `jinaai-0.2.4/LICENSE` & `jinaai-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.4/PKG-INFO` & `jinaai-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinaai
-Version: 0.2.4
+Version: 0.2.5
 Summary: Jina AI Python SDK
 Home-page: https://github.com/jina-ai/jinaai-py.git
 Author: Jina AI
 Author-email: guillaume.roncari@jina.ai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -303,14 +303,15 @@
 >| options['top_p']                       | None / str             | Default: 1
 >| options['stop']                        | None / str / str array | Up to 4 sequences where the API will stop generating further tokens
 >| options['max_tokens']                  | None / number          | Default: infinite
 >| options['presence_penalty']            | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['frequency_penalty']           | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['logit_bias']                  | None / dict            | The likelihood for a token to appear in the completion
 >| ...logit_bias['tokenId']               | number                 | Bias value from -100 to 100
+>| options['image']                       | str                    | The attached image of the message. The image can be either a URL or a base64-encoded string
 
 - Output
 
 >| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['output']                       | str               | The generated answer
```

### Comparing `jinaai-0.2.4/README.md` & `jinaai-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -293,14 +293,15 @@
 >| options['top_p']                       | None / str             | Default: 1
 >| options['stop']                        | None / str / str array | Up to 4 sequences where the API will stop generating further tokens
 >| options['max_tokens']                  | None / number          | Default: infinite
 >| options['presence_penalty']            | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['frequency_penalty']           | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['logit_bias']                  | None / dict            | The likelihood for a token to appear in the completion
 >| ...logit_bias['tokenId']               | number                 | Bias value from -100 to 100
+>| options['image']                       | str                    | The attached image of the message. The image can be either a URL or a base64-encoded string
 
 - Output
 
 >| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['output']                       | str               | The generated answer
```

### Comparing `jinaai-0.2.4/jinaai/__init__.py` & `jinaai-0.2.5/jinaai/__init__.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.4/jinaai/clients/BestBannerClient.py` & `jinaai-0.2.5/jinaai/clients/BestBannerClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.4/jinaai/clients/HTTPClient.py` & `jinaai-0.2.5/jinaai/clients/HTTPClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.4/jinaai/clients/JinaChatClient.py` & `jinaai-0.2.5/jinaai/clients/SceneXClient.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 from .HTTPClient import HTTPClient
-from ..utils import is_base64, is_url
 
+def autoFillFeatures(options=None):
+    features = options.get('features', []) if options else []
+    if options and 'question' in options and 'question_answer' not in features:
+        features.append('question_answer')
+    return features
 
-class JinaChatClient(HTTPClient):
+class SceneXClient(HTTPClient):
     def __init__(self, headers=None, options=None):
-        baseUrl = 'https://api.chat.jina.ai/v1/chat'
+        baseUrl = 'https://api.scenex.jina.ai/v1'
         defaultHeaders = { 
             'Content-Type': 'application/json',
         }
         mergedHeaders = defaultHeaders.update(headers)
         super().__init__(baseUrl=baseUrl, headers=defaultHeaders, options=options)
 
     def from_array(self, input, options=None):
         return {
-            'messages': [
+            'data': [
                 {
-                    'content': i,
-                    **(((is_url(i) or is_base64(i)) and { 'image': i }) or {}),
-                    'role': 'user',
+                    'image': i,
+                    'features': autoFillFeatures(options),
                     **(options or {})
                 }
                 for i in input
-            ],
-            **(options or {})
+            ]
         }
 
     def from_string(self, input, options=None):
         return {
-            'messages': [
+            'data': [
                 {
-                    'content': input,
-                    **(((is_url(input) or is_base64(input)) and { 'image': input }) or {}),
-                    'role': 'user',
+                    'image': input,
+                    'features': autoFillFeatures(options),
                     **(options or {})
                 }
-            ],
-            **(options or {})
+            ]
         }
 
     def to_simplified_output(self, output):
-        if 'choices' not in output or len(output['choices']) < 1 or output['choices'][0]['message']['content'] == '':
-            raise Exception('Remote API Error, bad output: ' + str(output))
+        if not output.get('result') or any(x.get('text') and x.get('text') != '' for x in output['result']) is False:
+            raise Exception('Remote API Error, bad output: {}'.format(json.dumps(output)))
         return {
-            'output': output['choices'][0]['message']['content'],
-            'chatId': output['chatId']
+            'results': [
+                {
+                    'output': r['answer'] if 'answer' in r and r['answer'] is not None else r['text'],
+                    'i18n': r['i18n']
+                }
+                for r in output['result']
+            ]
         }
 
-    def generate(self, data, options = None):
-        raw_output = self.post('/completions', data)
+    def describe(self, data, options = None):
+        raw_output = self.post('/describe', data)
         simplified_output = self.to_simplified_output(raw_output)
         if options and 'raw' in options:
             simplified_output['raw'] = raw_output
         return simplified_output
 
-    def stream(self, data, options = None):
-        return self.post('/completions', data, False)
```

### Comparing `jinaai-0.2.4/jinaai/clients/PromptPerfectClient.py` & `jinaai-0.2.5/jinaai/clients/PromptPerfectClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.4/jinaai/clients/RationaleClient.py` & `jinaai-0.2.5/jinaai/clients/RationaleClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.4/jinaai/utils.py` & `jinaai-0.2.5/jinaai/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 import mimetypes
 import os
 import re
+from typing import List, Dict, Optional
 
 def is_url(string):
     url_pattern = r'^(?:\w+:)?\/\/([^\s.]+\.\S{2}|localhost[:?\d]*)\S*$'
     return bool(re.match(url_pattern, string))
 
 def is_base64(string):
     base64_pattern = r'^data:[A-Za-z0-9+/]+;base64,'
@@ -22,7 +23,12 @@
     except Exception as error:
         raise Exception(f"Image to base64 error: {str(error)}")
 
 def get_mime_type(file_path):
     mime_type, _ = mimetypes.guess_type(file_path)
     return mime_type or 'application/octet-stream'
 
+def omit(d: Dict, key: str) -> Dict:
+    if d is None:
+        return {}
+    return {k: v for k, v in d.items() if k != key}
+
```

### Comparing `jinaai-0.2.4/jinaai.egg-info/PKG-INFO` & `jinaai-0.2.5/jinaai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinaai
-Version: 0.2.4
+Version: 0.2.5
 Summary: Jina AI Python SDK
 Home-page: https://github.com/jina-ai/jinaai-py.git
 Author: Jina AI
 Author-email: guillaume.roncari@jina.ai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -303,14 +303,15 @@
 >| options['top_p']                       | None / str             | Default: 1
 >| options['stop']                        | None / str / str array | Up to 4 sequences where the API will stop generating further tokens
 >| options['max_tokens']                  | None / number          | Default: infinite
 >| options['presence_penalty']            | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['frequency_penalty']           | None / number          | Number between -2.0 and 2.0, Default: 0
 >| options['logit_bias']                  | None / dict            | The likelihood for a token to appear in the completion
 >| ...logit_bias['tokenId']               | number                 | Bias value from -100 to 100
+>| options['image']                       | str                    | The attached image of the message. The image can be either a URL or a base64-encoded string
 
 - Output
 
 >| VARIABLE                               | TYPE              | VALUE 
 >|----------------------------------------|-------------------|----------
 >| output                                 | dict              | 
 >| output['output']                       | str               | The generated answer
```

