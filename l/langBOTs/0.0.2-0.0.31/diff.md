# Comparing `tmp/langBOTs-0.0.2.tar.gz` & `tmp/langBOTs-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langBOTs-0.0.2.tar", last modified: Wed Aug  2 14:22:42 2023, max compression
+gzip compressed data, was "langBOTs-0.0.31.tar", last modified: Mon Aug  7 09:17:04 2023, max compression
```

## Comparing `langBOTs-0.0.2.tar` & `langBOTs-0.0.31.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:22:42.498839 langBOTs-0.0.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1061 2023-08-02 14:04:38.000000 langBOTs-0.0.2/LICENSE.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2023-08-02 14:22:42.498839 langBOTs-0.0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      846 2023-08-02 13:25:09.000000 langBOTs-0.0.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:22:42.494839 langBOTs-0.0.2/langBOTs/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 06:40:02.000000 langBOTs-0.0.2/langBOTs/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1964 2023-08-02 13:39:54.000000 langBOTs-0.0.2/langBOTs/api.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1509 2023-08-02 11:12:34.000000 langBOTs-0.0.2/langBOTs/chain.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      239 2023-08-02 06:39:00.000000 langBOTs-0.0.2/langBOTs/main.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1941 2023-08-02 13:10:25.000000 langBOTs-0.0.2/langBOTs/query.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3725 2023-08-02 10:21:08.000000 langBOTs-0.0.2/langBOTs/scrapsplitvec.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 14:22:42.498839 langBOTs-0.0.2/langBOTs.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2023-08-02 14:22:42.000000 langBOTs-0.0.2/langBOTs.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      315 2023-08-02 14:22:42.000000 langBOTs-0.0.2/langBOTs.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-02 14:22:42.000000 langBOTs-0.0.2/langBOTs.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      110 2023-08-02 14:22:42.000000 langBOTs-0.0.2/langBOTs.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-08-02 14:22:42.000000 langBOTs-0.0.2/langBOTs.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       79 2023-08-02 14:22:42.498839 langBOTs-0.0.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1155 2023-08-02 14:22:35.000000 langBOTs-0.0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-07 09:17:04.625028 langBOTs-0.0.31/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1061 2023-08-02 14:04:38.000000 langBOTs-0.0.31/LICENSE.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1910 2023-08-07 09:17:04.625028 langBOTs-0.0.31/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1331 2023-08-07 09:15:34.000000 langBOTs-0.0.31/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-07 09:17:04.621028 langBOTs-0.0.31/langBOTs/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 06:40:02.000000 langBOTs-0.0.31/langBOTs/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2272 2023-08-03 20:16:11.000000 langBOTs-0.0.31/langBOTs/api.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1556 2023-08-03 20:26:08.000000 langBOTs-0.0.31/langBOTs/chain.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      239 2023-08-02 06:39:00.000000 langBOTs-0.0.31/langBOTs/main.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1118 2023-08-03 20:24:24.000000 langBOTs-0.0.31/langBOTs/query.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3725 2023-08-02 10:21:08.000000 langBOTs-0.0.31/langBOTs/scrapsplitvec.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-07 09:17:04.625028 langBOTs-0.0.31/langBOTs.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1910 2023-08-07 09:17:04.000000 langBOTs-0.0.31/langBOTs.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      315 2023-08-07 09:17:04.000000 langBOTs-0.0.31/langBOTs.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-07 09:17:04.000000 langBOTs-0.0.31/langBOTs.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      110 2023-08-07 09:17:04.000000 langBOTs-0.0.31/langBOTs.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-08-07 09:17:04.000000 langBOTs-0.0.31/langBOTs.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      805 2023-08-07 09:17:04.625028 langBOTs-0.0.31/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1156 2023-08-07 09:16:09.000000 langBOTs-0.0.31/setup.py
```

### Comparing `langBOTs-0.0.2/LICENSE.txt` & `langBOTs-0.0.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langBOTs-0.0.2/langBOTs/chain.py` & `langBOTs-0.0.31/langBOTs/chain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+"""Initialising huggingface model aswell as langchain"""
 from langchain import HuggingFacePipeline
 from langchain.chains import RetrievalQA
 from pydantic import BaseModel
-from typing import Optional, Any
+from typing import Any
 
 
 class MDL(BaseModel):
     retriever: Any
     model_id: str = "bigscience/bloom-560m"
     task: str = "text-generation"
     model_kwargs: Any = {"temperature": 0, "max_length": 512}
```

### Comparing `langBOTs-0.0.2/langBOTs/scrapsplitvec.py` & `langBOTs-0.0.31/langBOTs/scrapsplitvec.py`

 * *Files identical despite different names*

### Comparing `langBOTs-0.0.2/setup.py` & `langBOTs-0.0.31/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='langBOTs',
-    version='0.0.2',
+    version='0.0.31',
     author='Rajat S',
     description='Scrape, Langchain, Deploy !',
     url = 'https://github.com/gapirajat/langBOTs',
     packages=find_packages(),
     install_requires=[
         # List any dependencies your package requires here
         'langchain',
```

