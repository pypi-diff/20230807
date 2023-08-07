# Comparing `tmp/brainchain-0.4.2.tar.gz` & `tmp/brainchain-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.4.2.tar", max compression
+gzip compressed data, was "brainchain-0.4.3.tar", max compression
```

## Comparing `brainchain-0.4.2.tar` & `brainchain-0.4.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6082 2023-07-28 02:29:35.545159 brainchain-0.4.2/brainchain/.aider.chat.history.md
--rw-r--r--   0        0        0     1874 2023-07-28 02:29:35.545374 brainchain-0.4.2/brainchain/.aider.input.history
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.4.2/brainchain/README.md
--rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.4.2/brainchain/__init__.py
--rw-r--r--   0        0        0    11485 2023-07-28 02:36:23.299632 brainchain-0.4.2/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.4.2/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.4.2/brainchain/coredata.py
--rw-r--r--   0        0        0      665 2023-07-20 04:24:18.860063 brainchain-0.4.2/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.4.2/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.4.2/brainchain/sales_intel.py
--rw-r--r--   0        0        0      532 2023-07-28 02:32:49.415048 brainchain-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     6082 2023-07-28 02:29:35.545159 brainchain-0.4.3/brainchain/.aider.chat.history.md
+-rw-r--r--   0        0        0     1874 2023-07-28 02:29:35.545374 brainchain-0.4.3/brainchain/.aider.input.history
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.4.3/brainchain/README.md
+-rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.4.3/brainchain/__init__.py
+-rw-r--r--   0        0        0    12291 2023-08-07 19:42:48.123115 brainchain-0.4.3/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.4.3/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.4.3/brainchain/coredata.py
+-rw-r--r--   0        0        0      665 2023-07-20 04:24:18.860063 brainchain-0.4.3/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.4.3/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.4.3/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      532 2023-08-07 19:42:54.298079 brainchain-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.4.3/PKG-INFO
```

### Comparing `brainchain-0.4.2/brainchain/.aider.chat.history.md` & `brainchain-0.4.3/brainchain/.aider.chat.history.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.2/brainchain/.aider.input.history` & `brainchain-0.4.3/brainchain/.aider.input.history`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.2/brainchain/README.md` & `brainchain-0.4.3/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.2/brainchain/brainchain.py` & `brainchain-0.4.3/brainchain/brainchain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 import json
 import requests
+import tiktoken
 from urllib.parse import quote
 import aiohttp
 from . import SalesIntel, FactCheck
 
 class Brainchain:
     def __init__(self, env: str = "prod", api_key: str = os.environ["BRAINCHAIN_API_KEY"],
                  service_url="https://brainchain--agent.modal.run/", salesintel_api_key=os.environ[
@@ -20,17 +21,17 @@
                 "prod": "https://brainchain--agent.modal.run/",
                 "dev": "https://brainchain--agent-dev.modal.run/"
             },
             "agent-service": {
                 "agent": "https://brainchain--agent-service.modal.run/agent"
             },
             "prompt-completion-service": {
-                "prompting": "https://brainchain--prompt-completion-service-fastapi-app.modal.run/prompting",
-                "get_pdf_title": "https://brainchain--prompt-completion-service-fastapi-app.modal.run/get_pdf_title",
-                "get_pdf_authors": "https://brainchain--prompt-completion-service-fastapi-app.modal.run/get_pdf_authors"
+                "prompting": "https://brainchain--prompt-completion-service.modal.run/prompting",
+                "pdf-title": "https://brainchain--prompt-completion-service.modal.run/pdf-title",
+                "pdf-authors": "https://brainchain--prompt-completion-service.modal.run/pdf-authors"
             },
             "search": {
                 "prod": "https://brainchain--search.modal.run/",
                 "dev":  "https://brainchain--search-dev.modal.run/"
             },
             "electrolaser": {
                 "prod": "https://brainchain--electrolaser.modal.run/",
@@ -66,25 +67,32 @@
         params = {"query": query, "additional_pages": additional_pages}
         response = requests.get(endpoint, headers=headers, params=params)
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
-    def bullet_point_summarizer(self, text: str, prompt=""):
-        endpoint = self.services["electrolaser"][self.env]
+    def bullet_point_summarizer(self, content: str, model="gpt-4-32k"):
+        enc = tiktoken.encoding_for_model(model)
+        endpoint = self.services["prompt-completion-service"]["prompting"]
+        system_prompt = f"Write a concise summary of the user input in the form of numbered bullet points. Please output in JSON format, with a key named 'title' (corresponding to a title that you come up with based on the user input), as well as a key named 'description' of the overall text input, and then please have a key called 'bullet_points' which is an array of the bullet point summaries of the content."
+        user_prompt = content
+        content = content.replace("\n\n", "")
+        total_tokens_used = len(enc.encode(content) + enc.encode(system_prompt))
+        buffer = 512
+        max_tokens = 32768 - (total_tokens_used + buffer)
         headers = {"Authorization": f"Bearer {self.api_key}"}
-        params = {"query": query, "additional_pages": additional_pages}
-        response = requests.get(endpoint, headers=headers, params=params)
+        params = {"user_prompt": user_prompt, "system_prompt": system_prompt, "backend": "azure", "model": "gpt-4-32k", "max_tokens": max_tokens }
+        response = requests.post(endpoint, headers=headers, json=params)
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
-    def prompt(self, q, history=[], top_p=0.0, system="You are a multi-disciplinary research assistant who formulates, validates, and figures out correct answers. Your insights are ferocious and undeniable. You expand and digest new concepts and relate them to what you already know.", model="gpt-3.5-turbo-16k", presence_penalty=0.0, frequency_penalty=0.0, n=1):
+    def prompt(self, q, history=[], top_p=0.0, system="You are a multi-disciplinary research assistant who formulates, validates, and figures out correct answers. Your insights are ferocious and undeniable. You expand and digest new concepts and relate them to what you already know.", model="gpt-3.5-turbo-16k", backend="azure", presence_penalty=0.0, frequency_penalty=0.0, n=1):
         endpoint = self.services["prompt-completion-service"]["prompting"]
         headers = {"Authorization": f"Bearer {self.api_key}"}
         payload = {"user_prompt": q, "history": history, "system_prompt": system, "model": model, "presence_penalty": float(
             presence_penalty), "frequency_penalty": float(frequency_penalty), "top_p": float(top_p)}
         response = requests.post(endpoint, headers=headers, json=payload)
 
         if response.status_code == 200:
@@ -178,38 +186,38 @@
         response = requests.get(endpoint, headers=headers)
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
     def obtain_title(self, text_first_page: str = None):
-        endpoint = self.services["prompt-completion-service"]["get_pdf_title"]
+        endpoint = self.services["prompt-completion-service"]["pdf-title"]
         payload = {}
 
         if text_first_page:
             payload["document_text"] = text_first_page
     
         headers = {"Authorization": f"Bearer {self.api_key}"}
         response = requests.post(endpoint, headers=headers, json=payload)
         content = response.content.decode('utf-8')
         return json.loads(content)
 
     def obtain_authors(self, text_first_page: str = None):
-        endpoint =  self.services["prompt-completion-service"]["get_pdf_authors"]
+        endpoint =  self.services["prompt-completion-service"]["pdf-authors"]
         payload = {}
 
         if text_first_page:
             payload["document_text"] = text_first_page
 
         headers = {"Authorization": f"Bearer {self.api_key}"}
         response = requests.post(endpoint, headers=headers, json=payload)
         content = response.content.decode('utf-8')
         return json.loads(content)
 
-    def summon(self, prompt, agent_type="OAMF", model="gpt-4-0613", max_tokens=2048, temperature=0, top_p=0, top_k=0.0, presence_penalty=0.0, frequency_penalty=0.0, chat_history: list = []):
+    def summon(self, prompt, agent_type="OAMF", model="gpt-4-32k", backend="azure", max_tokens=8000, temperature=0, top_p=0, top_k=0.0, presence_penalty=0.0, frequency_penalty=0.0, chat_history: list = []):
         endpoint = self.services["agent-service"]["agent"]
         headers = {"Authorization": f"Bearer {self.api_key}"}
         params = {
             "prompt": prompt,
             "env": self.env,
             "agent_type": agent_type,
             "model": model,
@@ -224,15 +232,15 @@
         response = requests.post(endpoint, headers=headers, json=params)
 
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
-    async def asummon(self, prompt, agent_type="OAMF", model="gpt-4-0613", max_tokens=2048, temperature=0, top_p=0, top_k=0.0, presence_penalty=0.0, frequency_penalty=0.0, chat_history: list = []):
+    async def asummon(self, prompt, agent_type="OAMF", model="gpt-4-32k", backend="azure", max_tokens=8192, temperature=0, top_p=0, top_k=0.0, presence_penalty=0.0, frequency_penalty=0.0, chat_history: list = []):
         endpoint = self.services["agent-service"]["agent"]
         headers = {"Authorization": f"Bearer {self.api_key}"}
         params = {
             "prompt": prompt,
             "env": self.env,
             "agent_type": agent_type,
             "model": model,
```

### Comparing `brainchain-0.4.2/brainchain/carnivore.py` & `brainchain-0.4.3/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.2/brainchain/coredata.py` & `brainchain-0.4.3/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.2/brainchain/factcheck.py` & `brainchain-0.4.3/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.2/brainchain/requirements.txt` & `brainchain-0.4.3/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.2/brainchain/sales_intel.py` & `brainchain-0.4.3/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.2/pyproject.toml` & `brainchain-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.4.2"
+version = "0.4.3"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
 promptlayer = "0.1.92"
 openai = "0.27.8"
-modal-client = "0.50.2627"
+modal-client = "0.50.2932"
 tiktoken = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `brainchain-0.4.2/PKG-INFO` & `brainchain-0.4.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.4.2
+Version: 0.4.3
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: modal-client (==0.50.2627)
+Requires-Dist: modal-client (==0.50.2932)
 Requires-Dist: openai (==0.27.8)
 Requires-Dist: promptlayer (==0.1.92)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
```

