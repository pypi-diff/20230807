# Comparing `tmp/vector_vault-2.1.8.tar.gz` & `tmp/vector_vault-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.1.8.tar", last modified: Mon Aug  7 02:46:54 2023, max compression
+gzip compressed data, was "vector_vault-2.1.9.tar", last modified: Mon Aug  7 02:55:57 2023, max compression
```

## Comparing `vector_vault-2.1.8.tar` & `vector_vault-2.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:46:54.773221 vector_vault-2.1.8/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.8/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 02:46:54.773059 vector_vault-2.1.8/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    27408 2023-08-06 20:06:54.000000 vector_vault-2.1.8/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-07 02:46:54.773260 vector_vault-2.1.8/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1046 2023-08-07 02:46:28.000000 vector_vault-2.1.8/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:46:54.769273 vector_vault-2.1.8/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 02:46:54.000000 vector_vault-2.1.8/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-07 02:46:54.000000 vector_vault-2.1.8/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-07 02:46:54.000000 vector_vault-2.1.8/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-07 02:46:54.000000 vector_vault-2.1.8/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-07 02:46:54.000000 vector_vault-2.1.8/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:46:54.772690 vector_vault-2.1.8/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.8/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    14352 2023-08-07 01:04:28.000000 vector_vault-2.1.8/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.8/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.8/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.8/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.8/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.8/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16787 2023-08-06 19:45:14.000000 vector_vault-2.1.8/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    36861 2023-08-06 17:13:56.000000 vector_vault-2.1.8/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.8/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.8/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:55:57.891199 vector_vault-2.1.9/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.9/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 02:55:57.891058 vector_vault-2.1.9/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    27408 2023-08-06 20:06:54.000000 vector_vault-2.1.9/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-07 02:55:57.891233 vector_vault-2.1.9/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1046 2023-08-07 02:55:34.000000 vector_vault-2.1.9/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:55:57.886866 vector_vault-2.1.9/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 02:55:57.000000 vector_vault-2.1.9/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-07 02:55:57.000000 vector_vault-2.1.9/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-07 02:55:57.000000 vector_vault-2.1.9/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-07 02:55:57.000000 vector_vault-2.1.9/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-07 02:55:57.000000 vector_vault-2.1.9/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:55:57.890665 vector_vault-2.1.9/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.9/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    14352 2023-08-07 01:04:28.000000 vector_vault-2.1.9/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.9/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.9/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.9/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.9/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.9/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16787 2023-08-06 19:45:14.000000 vector_vault-2.1.9/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    37058 2023-08-07 02:55:28.000000 vector_vault-2.1.9/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.9/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.9/vectorvault/wrap.py
```

### Comparing `vector_vault-2.1.8/LICENSE` & `vector_vault-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.8/PKG-INFO` & `vector_vault-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.1.8
+Version: 2.1.9
 Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-2.1.8/README.md` & `vector_vault-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.8/setup.py` & `vector_vault-2.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.1.8",
+    version="2.1.9",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Customize ChatGPT and unleash the full potential of generative AI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.1.8/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.1.9/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.1.8
+Version: 2.1.9
 Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-2.1.8/vectorvault/ai.py` & `vector_vault-2.1.9/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.8/vectorvault/cloud_api.py` & `vector_vault-2.1.9/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.8/vectorvault/cloudmanager.py` & `vector_vault-2.1.9/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.8/vectorvault/creds.py` & `vector_vault-2.1.9/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.8/vectorvault/download.py` & `vector_vault-2.1.9/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.8/vectorvault/itemize.py` & `vector_vault-2.1.9/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.8/vectorvault/tools_gpt.py` & `vector_vault-2.1.9/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.8/vectorvault/vault.py` & `vector_vault-2.1.9/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,15 @@
                 current_item_index += 1
 
         self.last_time = start_time
         self.first_run = False
         if self.verbose == True:
             print("get vectors time --- %s seconds ---" % (time.time() - start_time))
 
-    def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, custom_prompt=False):
+    def get_chat(self, text: str = None, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, custom_prompt=False):
         '''
             Chat get response from OpenAI's ChatGPT. 
             Models: ChatGPT = "gpt-3.5-turbo" • GPT4 = "gpt-4" 
             Large Context Models: ChatGPT 16k = "gpt-3.5-turbo-16k" • GPT4 32k = "gpt-4-32k"
             Best Versions: "gpt-3.5-turbo-0301" is March 2023 ChatGPT (best version) - "gpt-4-0314" (best version)
 
             Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
@@ -532,19 +532,22 @@
         if not history:
             history = ''
         
         deduction = self.needed_sleep_time - (time.time() - self.last_chat_time)
         self.needed_sleep_time = deduction if deduction > 0 else 0
         time.sleep(self.needed_sleep_time)
 
-        if self.ai.get_tokens(text) > 4000:
-            if summary:
-                inputs = self.split_text(text, 14500)
+        if text: 
+            if self.ai.get_tokens(text) > 4000:
+                if summary:
+                    inputs = self.split_text(text, 14500)
+                else:
+                    inputs = text[-16000:]
             else:
-                inputs = text[-16000:]
+                inputs = [text]
         else:
             inputs = [text]
         response = ''
         for segment in inputs:
             start_time = time.time()
             seg_len = self.ai.get_tokens(segment)
             # max 90,000 tokens per minute | max requests per minute = 3500
@@ -602,15 +605,15 @@
             print("get chat time --- %s seconds ---" % (time.time() - start_time))
 
         if return_context == False:
             return response
         elif return_context == True:
             return {'response': response, 'context': context}
         
-    def get_chat_stream(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, metatag=False, metatag_prefixes=False, metatag_suffixes=False, custom_prompt=False):
+    def get_chat_stream(self, text: str = None, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False, metatag=False, metatag_prefixes=False, metatag_suffixes=False, custom_prompt=False):
         '''
             Always use this get_chat_stream() wrapped by either print_stream(), or cloud_stream().
             cloud_stream() is for cloud functions, like a flask app serving a front end elsewhere.
             print_stream() is for local console printing
 
             - Example Signle Usage: 
             `response = vault.print_stream(vault.get_chat_stream(text))`
@@ -682,20 +685,23 @@
         
         if not history:
             history = ''
         
         deduction = self.needed_sleep_time - (time.time() - self.last_chat_time)
         self.needed_sleep_time = deduction if deduction > 0 else 0
         time.sleep(self.needed_sleep_time)
-
-        if self.ai.get_tokens(text) > 4000:
-            if summary:
-                inputs = self.split_text(text, 14500)
+        
+        if text:
+            if self.ai.get_tokens(text) > 4000:
+                if summary:
+                    inputs = self.split_text(text, 14500)
+                else:
+                    inputs = text[-16000:]
             else:
-                inputs = text[-16000:]
+                inputs = [text]
         else:
             inputs = [text]
         response = ''
         for segment in inputs:
             start_time = time.time()
             seg_len = self.ai.get_tokens(segment)
             # max 90,000 tokens per minute | max requests per minute = 3500
```

### Comparing `vector_vault-2.1.8/vectorvault/vecreq.py` & `vector_vault-2.1.9/vectorvault/vecreq.py`

 * *Files identical despite different names*

