# Comparing `tmp/brainchain-0.4.3.tar.gz` & `tmp/brainchain-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.4.3.tar", max compression
+gzip compressed data, was "brainchain-0.4.4.tar", max compression
```

## Comparing `brainchain-0.4.3.tar` & `brainchain-0.4.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6082 2023-07-28 02:29:35.545159 brainchain-0.4.3/brainchain/.aider.chat.history.md
--rw-r--r--   0        0        0     1874 2023-07-28 02:29:35.545374 brainchain-0.4.3/brainchain/.aider.input.history
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.4.3/brainchain/README.md
--rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.4.3/brainchain/__init__.py
--rw-r--r--   0        0        0    12291 2023-08-07 19:42:48.123115 brainchain-0.4.3/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.4.3/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.4.3/brainchain/coredata.py
--rw-r--r--   0        0        0      665 2023-07-20 04:24:18.860063 brainchain-0.4.3/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.4.3/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.4.3/brainchain/sales_intel.py
--rw-r--r--   0        0        0      532 2023-08-07 19:42:54.298079 brainchain-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     6082 2023-07-28 02:29:35.545159 brainchain-0.4.4/brainchain/.aider.chat.history.md
+-rw-r--r--   0        0        0     1874 2023-07-28 02:29:35.545374 brainchain-0.4.4/brainchain/.aider.input.history
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.4.4/brainchain/README.md
+-rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.4.4/brainchain/__init__.py
+-rw-r--r--   0        0        0    12265 2023-08-07 20:24:16.580273 brainchain-0.4.4/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.4.4/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.4.4/brainchain/coredata.py
+-rw-r--r--   0        0        0      665 2023-07-20 04:24:18.860063 brainchain-0.4.4/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.4.4/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.4.4/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      532 2023-08-07 20:24:19.346496 brainchain-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.4.4/PKG-INFO
```

### Comparing `brainchain-0.4.3/brainchain/.aider.chat.history.md` & `brainchain-0.4.4/brainchain/.aider.chat.history.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.3/brainchain/.aider.input.history` & `brainchain-0.4.4/brainchain/.aider.input.history`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.3/brainchain/README.md` & `brainchain-0.4.4/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.3/brainchain/brainchain.py` & `brainchain-0.4.4/brainchain/brainchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,25 +84,25 @@
         params = {"user_prompt": user_prompt, "system_prompt": system_prompt, "backend": "azure", "model": "gpt-4-32k", "max_tokens": max_tokens }
         response = requests.post(endpoint, headers=headers, json=params)
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
-    def prompt(self, q, history=[], top_p=0.0, system="You are a multi-disciplinary research assistant who formulates, validates, and figures out correct answers. Your insights are ferocious and undeniable. You expand and digest new concepts and relate them to what you already know.", model="gpt-3.5-turbo-16k", backend="azure", presence_penalty=0.0, frequency_penalty=0.0, n=1):
+    def prompt(self, q, history=[], top_p=0.0, system="You are a multi-disciplinary research assistant who formulates, validates, and figures out correct answers. Your insights are ferocious and undeniable. You expand and digest new concepts and relate them to what you already know.", model="gpt-4-32k", backend="azure", presence_penalty=0.0, frequency_penalty=0.0, n=1):
         endpoint = self.services["prompt-completion-service"]["prompting"]
         headers = {"Authorization": f"Bearer {self.api_key}"}
         payload = {"user_prompt": q, "history": history, "system_prompt": system, "model": model, "presence_penalty": float(
             presence_penalty), "frequency_penalty": float(frequency_penalty), "top_p": float(top_p)}
         response = requests.post(endpoint, headers=headers, json=payload)
 
         if response.status_code == 200:
             return response.json()
         else:
-            response.raise_for_status()
+            return {}
 
     def ingest(self, url: str):
         """
         Ingest a document into Weaviate, via URL. For now, this only works with PDFs. URL has to be publicly
         accessible and point directly to the document, e.g. https://www.example.com/document.pdf.
 
         Note: if you want to monitor the status of your doc's ingestion, look at the Modal logs for the
```

### Comparing `brainchain-0.4.3/brainchain/carnivore.py` & `brainchain-0.4.4/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.3/brainchain/coredata.py` & `brainchain-0.4.4/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.3/brainchain/factcheck.py` & `brainchain-0.4.4/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.3/brainchain/requirements.txt` & `brainchain-0.4.4/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.3/brainchain/sales_intel.py` & `brainchain-0.4.4/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.4.3/pyproject.toml` & `brainchain-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.4.3"
+version = "0.4.4"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
 promptlayer = "0.1.92"
```

### Comparing `brainchain-0.4.3/PKG-INFO` & `brainchain-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.4.3
+Version: 0.4.4
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

