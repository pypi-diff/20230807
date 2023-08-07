# Comparing `tmp/vector_vault-2.1.9.tar.gz` & `tmp/vector_vault-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.1.9.tar", last modified: Mon Aug  7 02:55:57 2023, max compression
+gzip compressed data, was "vector_vault-2.2.0.tar", last modified: Mon Aug  7 16:29:30 2023, max compression
```

## Comparing `vector_vault-2.1.9.tar` & `vector_vault-2.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:55:57.891199 vector_vault-2.1.9/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.9/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 02:55:57.891058 vector_vault-2.1.9/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    27408 2023-08-06 20:06:54.000000 vector_vault-2.1.9/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-07 02:55:57.891233 vector_vault-2.1.9/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1046 2023-08-07 02:55:34.000000 vector_vault-2.1.9/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:55:57.886866 vector_vault-2.1.9/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 02:55:57.000000 vector_vault-2.1.9/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-07 02:55:57.000000 vector_vault-2.1.9/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-07 02:55:57.000000 vector_vault-2.1.9/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-07 02:55:57.000000 vector_vault-2.1.9/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-07 02:55:57.000000 vector_vault-2.1.9/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 02:55:57.890665 vector_vault-2.1.9/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.9/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    14352 2023-08-07 01:04:28.000000 vector_vault-2.1.9/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.9/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.9/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.9/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.9/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.9/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16787 2023-08-06 19:45:14.000000 vector_vault-2.1.9/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    37058 2023-08-07 02:55:28.000000 vector_vault-2.1.9/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.9/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.9/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 16:29:30.604033 vector_vault-2.2.0/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.2.0/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 16:29:30.603851 vector_vault-2.2.0/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    27408 2023-08-06 20:06:54.000000 vector_vault-2.2.0/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-07 16:29:30.604072 vector_vault-2.2.0/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1046 2023-08-07 16:29:24.000000 vector_vault-2.2.0/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 16:29:30.599551 vector_vault-2.2.0/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 16:29:30.000000 vector_vault-2.2.0/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-07 16:29:30.000000 vector_vault-2.2.0/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-07 16:29:30.000000 vector_vault-2.2.0/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-07 16:29:30.000000 vector_vault-2.2.0/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-07 16:29:30.000000 vector_vault-2.2.0/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 16:29:30.603432 vector_vault-2.2.0/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.2.0/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    14352 2023-08-07 01:04:28.000000 vector_vault-2.2.0/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.2.0/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.2.0/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.2.0/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.2.0/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.2.0/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16787 2023-08-06 19:45:14.000000 vector_vault-2.2.0/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    37296 2023-08-07 16:29:14.000000 vector_vault-2.2.0/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.2.0/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.2.0/vectorvault/wrap.py
```

### Comparing `vector_vault-2.1.9/LICENSE` & `vector_vault-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.9/PKG-INFO` & `vector_vault-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.1.9
+Version: 2.2.0
 Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-2.1.9/README.md` & `vector_vault-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.9/setup.py` & `vector_vault-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.1.9",
+    version="2.2.0",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Customize ChatGPT and unleash the full potential of generative AI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.1.9/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.2.0/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.1.9
+Version: 2.2.0
 Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-2.1.9/vectorvault/ai.py` & `vector_vault-2.2.0/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.9/vectorvault/cloud_api.py` & `vector_vault-2.2.0/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.9/vectorvault/cloudmanager.py` & `vector_vault-2.2.0/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.9/vectorvault/creds.py` & `vector_vault-2.2.0/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.9/vectorvault/download.py` & `vector_vault-2.2.0/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.9/vectorvault/itemize.py` & `vector_vault-2.2.0/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.9/vectorvault/tools_gpt.py` & `vector_vault-2.2.0/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.9/vectorvault/vault.py` & `vector_vault-2.2.0/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,15 +545,18 @@
             else:
                 inputs = [text]
         else:
             inputs = [text]
         response = ''
         for segment in inputs:
             start_time = time.time()
-            seg_len = self.ai.get_tokens(segment)
+            if text:
+                seg_len = self.ai.get_tokens(segment)
+            else:
+                seg_len = len(custom_prompt)
             # max 90,000 tokens per minute | max requests per minute = 3500
             trip_time = float(start_time - self.last_chat_time)
             req_min = 60 / trip_time # 1 min (60) / time between requests (trip_time)
             projected_tokens_per_min = req_min * seg_len
             rate_ratio = projected_tokens_per_min / 90000
             if self.verbose == True:
                 print(f'Projected Tokens per min:{projected_tokens_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {seg_len}')
@@ -566,15 +569,15 @@
             if self.verbose == True:
                 print(f"Time calc'd to sleep: {self.needed_sleep_time}")
             exceptions = 0
             while True:
                 try:
                     if summary and not get_context:
                         response += self.ai.summarize(segment, model=model, custom_prompt=custom_prompt)
-                    elif get_context and not summary:
+                    elif text and get_context and not summary:
                         user_input = segment + history if history_search else segment
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-16000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-14000:]
@@ -583,15 +586,15 @@
                             input_ = str(context)
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                             for text in context:
                                 input_ += text['data']
                         response = self.ai.llm_w_context(segment, input_, history, model=model, custom_prompt=custom_prompt)
-                    else:
+                    else: # Custom prompt only
                         response = self.ai.llm(segment, history, model=model, custom_prompt=custom_prompt)
                     break
                 except Exception as e:
                     exceptions += 1
                     print(traceback.format_exc())
                     print(f"API Error: {e}. Sleeping 5 seconds")
                     if exceptions >= 5:
@@ -699,15 +702,18 @@
             else:
                 inputs = [text]
         else:
             inputs = [text]
         response = ''
         for segment in inputs:
             start_time = time.time()
-            seg_len = self.ai.get_tokens(segment)
+            if text:
+                seg_len = self.ai.get_tokens(segment)
+            else:
+                seg_len = len(custom_prompt)
             # max 90,000 tokens per minute | max requests per minute = 3500
             trip_time = float(start_time - self.last_chat_time)
             req_min = 60 / trip_time # 1 min (60) / time between requests (trip_time)
             projected_tokens_per_min = req_min * seg_len
             rate_ratio = projected_tokens_per_min / 90000
             if self.verbose == True:
                 print(f'Projected Tokens per min:{projected_tokens_per_min} | Rate Limit Ratio: {rate_ratio} | Text Length: {seg_len}')
@@ -722,15 +728,15 @@
             exceptions = 0
             while True:
                 try:
                     if summary and get_context == False:
                         for word in self.ai.summarize_stream(segment, model=model, custom_prompt=custom_prompt):
                             yield word
                         yield '!END'
-                    elif get_context and not summary:
+                    elif text and get_context and not summary:
                         user_input = segment + history if history_search else segment
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-16000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-14000:]
@@ -760,15 +766,15 @@
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
                                 yield item['data']
                             yield '!END'
                         else: # No context return and just send back the ai stream only 
                             for word in self.ai.llm_w_context_stream(segment, input_, history, model=model, custom_prompt=custom_prompt):
                                 yield word
                             yield '!END'
-                    else:
+                    else: # Just a custom prompt
                         for word in self.ai.llm_stream(segment, history, model=model, custom_prompt=custom_prompt):
                             yield word
                         yield '!END'
                     break
                 except Exception as e:
                     exceptions += 1
                     print(f"API Error: {e}. Sleeping 5 seconds")
```

### Comparing `vector_vault-2.1.9/vectorvault/vecreq.py` & `vector_vault-2.2.0/vectorvault/vecreq.py`

 * *Files identical despite different names*

