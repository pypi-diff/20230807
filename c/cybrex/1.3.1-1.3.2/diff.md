# Comparing `tmp/cybrex-1.3.1.tar.gz` & `tmp/cybrex-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.3.1.tar", last modified: Mon Aug  7 13:54:20 2023, max compression
+gzip compressed data, was "cybrex-1.3.2.tar", last modified: Mon Aug  7 14:45:56 2023, max compression
```

## Comparing `cybrex-1.3.1.tar` & `cybrex-1.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.930799 cybrex-1.3.1/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.3.1/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 13:54:20.930512 cybrex-1.3.1/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.3.1/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.924952 cybrex-1.3.1/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.3.1/cybrex/__init__.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.928617 cybrex-1.3.1/cybrex/chains/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.1/cybrex/chains/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.3.1/cybrex/chains/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2381 2023-08-07 13:01:11.000000 cybrex-1.3.1/cybrex/chains/map_reduce.py
--rw-r--r--   0 pasha      (501) staff       (20)     5564 2023-08-07 13:54:06.000000 cybrex-1.3.1/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    10794 2023-08-07 13:42:48.000000 cybrex-1.3.1/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)     1676 2023-08-05 19:44:06.000000 cybrex-1.3.1/cybrex/document_chunker.py
--rw-r--r--   0 pasha      (501) staff       (20)     4830 2023-08-07 11:07:40.000000 cybrex-1.3.1/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.929139 cybrex-1.3.1/cybrex/prompts/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.1/cybrex/prompts/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     9756 2023-08-07 13:43:38.000000 cybrex-1.3.1/cybrex/prompts/base.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.930033 cybrex-1.3.1/cybrex/vector_storage/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.1/cybrex/vector_storage/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)      206 2023-08-07 13:42:48.000000 cybrex-1.3.1/cybrex/vector_storage/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2987 2023-08-07 12:50:10.000000 cybrex-1.3.1/cybrex/vector_storage/chroma.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 13:54:20.927754 cybrex-1.3.1/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      554 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-07 13:54:20.000000 cybrex-1.3.1/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-07 13:54:09.000000 cybrex-1.3.1/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.3.1/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-07 13:54:20.930904 cybrex-1.3.1/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 14:45:56.831986 cybrex-1.3.2/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.3.2/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 14:45:56.831694 cybrex-1.3.2/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.3.2/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 14:45:56.827313 cybrex-1.3.2/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.3.2/cybrex/__init__.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 14:45:56.829977 cybrex-1.3.2/cybrex/chains/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.2/cybrex/chains/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.3.2/cybrex/chains/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2389 2023-08-07 14:15:31.000000 cybrex-1.3.2/cybrex/chains/map_reduce.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5564 2023-08-07 13:54:06.000000 cybrex-1.3.2/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    10855 2023-08-07 14:38:25.000000 cybrex-1.3.2/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1676 2023-08-05 19:44:06.000000 cybrex-1.3.2/cybrex/document_chunker.py
+-rw-r--r--   0 pasha      (501) staff       (20)     4843 2023-08-07 14:38:25.000000 cybrex-1.3.2/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 14:45:56.830468 cybrex-1.3.2/cybrex/prompts/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.2/cybrex/prompts/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     9984 2023-08-07 14:45:37.000000 cybrex-1.3.2/cybrex/prompts/base.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 14:45:56.831269 cybrex-1.3.2/cybrex/vector_storage/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.2/cybrex/vector_storage/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)      219 2023-08-07 14:38:25.000000 cybrex-1.3.2/cybrex/vector_storage/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2987 2023-08-07 12:50:10.000000 cybrex-1.3.2/cybrex/vector_storage/chroma.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 14:45:56.829239 cybrex-1.3.2/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 14:45:56.000000 cybrex-1.3.2/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      554 2023-08-07 14:45:56.000000 cybrex-1.3.2/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-07 14:45:56.000000 cybrex-1.3.2/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-07 14:45:56.000000 cybrex-1.3.2/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-07 14:45:56.000000 cybrex-1.3.2/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-07 14:45:56.000000 cybrex-1.3.2/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-07 14:37:24.000000 cybrex-1.3.2/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.3.2/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-07 14:45:56.832081 cybrex-1.3.2/setup.cfg
```

### Comparing `cybrex-1.3.1/PKG-INFO` & `cybrex-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.3.1
+Version: 1.3.2
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.3.1/README.md` & `cybrex-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.1/cybrex/chains/map_reduce.py` & `cybrex-1.3.2/cybrex/chains/map_reduce.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 llm_output = self.llm.process(input_chunk)
                 logging.getLogger('statbox').info({
                     'action': 'intermediate_map_reduce_step',
                     'output': llm_output,
                 })
                 outputs.append(llm_output)
             if len(outputs) == 1:
-                return outputs[0]
+                return outputs[0].strip()
             chunks = list(map(self.output_processor, outputs))
 
 
 class ChunkAccumulator:
     def __init__(self, prompter):
         self.prompter = prompter
         self.chunks = []
```

### Comparing `cybrex-1.3.1/cybrex/cli.py` & `cybrex-1.3.2/cybrex/cli.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.1/cybrex/cybrex_ai.py` & `cybrex-1.3.2/cybrex/cybrex_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import asyncio
 import base64
 import io
 import json
 import logging
 import os.path
 from gzip import GzipFile
-from typing import List, Optional
+from typing import (
+    List,
+    Optional,
+)
 
 import numpy as np
 import pypdf
 import yaml
 from aiokit import AioThing
 from izihawa_configurator import Configurator
 from izihawa_utils.exceptions import BaseError
 from izihawa_utils.file import mkdir_p
 from stc_geck.advices import get_documents_on_topic
 from stc_geck.client import StcGeck
 
-from .chains.map_reduce import QAChain, SummarizeChain
+from .chains.map_reduce import (
+    QAChain,
+    SummarizeChain,
+)
 from .document_chunker import DocumentChunker
 from .models import CybrexModel
 from .vector_storage.chroma import ChromaVectorStorage
 
 
 class DocumentNotFoundError(BaseError):
     pass
@@ -74,15 +80,18 @@
         if not self.geck:
             self.geck = StcGeck(
                 ipfs_http_base_url=config['ipfs']['http']['base_url'],
                 grpc_api_endpoint=config['summa']['endpoint']
             )
             self.starts.append(self.geck)
 
-        self.vector_storage = ChromaVectorStorage(path=os.path.join(self.home_path, 'chroma'), collection_name=self.model.get_embeddings_id())
+        self.vector_storage = ChromaVectorStorage(
+            path=os.path.join(self.home_path, 'chroma'),
+            collection_name=self.model.get_embeddings_id(),
+        )
 
     async def resolve_document_content(self, document: dict) -> Optional[str]:
         if 'content' in document:
             return document['content']
         elif 'links' in document:
             primary_link = document['links'][0]
             file_content = await self.geck.download(document['links'][0]['cid'])
```

### Comparing `cybrex-1.3.1/cybrex/document_chunker.py` & `cybrex-1.3.2/cybrex/document_chunker.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.1/cybrex/models.py` & `cybrex-1.3.2/cybrex/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 from typing import List
 
 from ctransformers import AutoModelForCausalLM
 from keybert import KeyBERT
 from langchain import OpenAI
-from langchain.embeddings import HuggingFaceInstructEmbeddings, OpenAIEmbeddings
+from langchain.embeddings import (
+    HuggingFaceInstructEmbeddings,
+    OpenAIEmbeddings,
+)
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from lazy import lazy
 
 from .prompts.base import BasePrompter
 
 
 class LLM:
```

### Comparing `cybrex-1.3.1/cybrex/prompts/base.py` & `cybrex-1.3.2/cybrex/prompts/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             'openai': OpenAIPrompter()
         }[type_]
 
     def qa_prompt(self, question, chunks: List[dict]):
         if len(chunks) >= 1:
             return '''
 You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document and a question, create a final answer.
-ALWAYS add references using DOIs near corresponding statements in your answer.
+ALWAYS add references using DOIs from extracted parts near corresponding statements in your answer.
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
 
 USER:
 Extracted parts:
 {summary}
 
 Question:
@@ -64,15 +64,15 @@
 
 class Llama27bPrompter(BasePrompter):
     def qa_prompt(self, question: str, chunks: List[dict]):
         if len(chunks) >= 1:
             return '''
 <s><<SYS>>
 You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document and a question, create a final answer.
-ALWAYS add references to extracted parts using template "DOI: 10.1038/s41576-022-00477-6" near corresponding statements.
+ALWAYS add references using DOIs from extracted parts near corresponding statements in your answer.
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
 <</SYS>>
 [INST]
 Extracted parts:
 {summary}
 
 Question:
@@ -132,7 +132,15 @@
 DOIs:
 
 QUESTION: {question}
 =========
 {summary}
 =========
 FINAL ANSWER:""".format(question=question, summary=self.generate_summary(chunks))
+
+    def summarize_prompt(self, chunks: List[dict]):
+        return '''
+Given the following extracted parts of a long document, summarize its content
+
+Extracted parts:
+{summary}
+'''.format(summary=self.generate_summary(chunks))
```

### Comparing `cybrex-1.3.1/cybrex/vector_storage/chroma.py` & `cybrex-1.3.2/cybrex/vector_storage/chroma.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.1/cybrex.egg-info/PKG-INFO` & `cybrex-1.3.2/cybrex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.3.1
+Version: 1.3.2
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.3.1/cybrex.egg-info/SOURCES.txt` & `cybrex-1.3.2/cybrex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.1/pyproject.toml` & `cybrex-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.3.1"
+version = "1.3.2"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

