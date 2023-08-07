# Comparing `tmp/myllm-1.2.6.tar.gz` & `tmp/myllm-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myllm-1.2.6.tar", max compression
+gzip compressed data, was "myllm-1.2.7.tar", max compression
```

## Comparing `myllm-1.2.6.tar` & `myllm-1.2.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-08-07 17:06:56.330047 myllm-1.2.6/LICENSE
--rw-r--r--   0        0        0     2230 2023-08-07 17:06:56.330047 myllm-1.2.6/README.md
--rw-r--r--   0        0        0       96 2023-08-07 17:06:57.786044 myllm-1.2.6/myllm/__init__.py
--rw-r--r--   0        0        0      701 2023-08-07 17:06:56.330047 myllm-1.2.6/myllm/config.py
--rw-r--r--   0        0        0     1313 2023-08-07 17:06:56.330047 myllm-1.2.6/myllm/default_settings.toml
--rw-r--r--   0        0        0     3203 2023-08-07 17:06:56.330047 myllm-1.2.6/myllm/main.py
--rw-r--r--   0        0        0     3033 2023-08-07 17:06:57.774044 myllm-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 myllm-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-07 17:58:51.017628 myllm-1.2.7/LICENSE
+-rw-r--r--   0        0        0     2230 2023-08-07 17:58:51.017628 myllm-1.2.7/README.md
+-rw-r--r--   0        0        0       96 2023-08-07 17:58:52.505621 myllm-1.2.7/myllm/__init__.py
+-rw-r--r--   0        0        0      701 2023-08-07 17:58:51.021628 myllm-1.2.7/myllm/config.py
+-rw-r--r--   0        0        0     1313 2023-08-07 17:58:51.021628 myllm-1.2.7/myllm/default_settings.toml
+-rw-r--r--   0        0        0     3208 2023-08-07 17:58:51.021628 myllm-1.2.7/myllm/main.py
+-rw-r--r--   0        0        0     3051 2023-08-07 17:58:52.497621 myllm-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3116 1970-01-01 00:00:00.000000 myllm-1.2.7/PKG-INFO
```

### Comparing `myllm-1.2.6/LICENSE` & `myllm-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `myllm-1.2.6/README.md` & `myllm-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `myllm-1.2.6/myllm/config.py` & `myllm-1.2.7/myllm/config.py`

 * *Files identical despite different names*

### Comparing `myllm-1.2.6/myllm/default_settings.toml` & `myllm-1.2.7/myllm/default_settings.toml`

 * *Files identical despite different names*

### Comparing `myllm-1.2.6/myllm/main.py` & `myllm-1.2.7/myllm/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-MYLLM Main
+MYLLM Main 🤖
 
 """
 
 import asyncio
 import importlib
 from typing import Any, List, Mapping, Optional
```

### Comparing `myllm-1.2.6/pyproject.toml` & `myllm-1.2.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "MyLLM"
-version = "1.2.6"
+version = "1.2.7"
 description = "A python package to interact with llm model supported by g4f"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["chatgpt","llm","ai","llama","ai", "g4f", "freegpt"]
 packages = [
     {include = "myllm"}
@@ -22,15 +22,16 @@
 "Issues" =  "https://github.com/mraniki/MyLLM/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 loguru = "^0.7.0"
-g4f = "^0.0.1"
+g4f = "^0.0.1.4"
+js2py = "^0.74"
 # langchain = "^0.0.255"
 # libre-chat = "^0.0.4"
 # huggingface_hub = "^v0.16.4"
 # google-search-results = "^2.4.2"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `myllm-1.2.6/PKG-INFO` & `myllm-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: myllm
-Version: 1.2.6
+Version: 1.2.7
 Summary: A python package to interact with llm model supported by g4f
 License: MIT
 Keywords: chatgpt,llm,ai,llama,ai,g4f,freegpt
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
-Requires-Dist: g4f (>=0.0.1,<0.0.2)
+Requires-Dist: g4f (>=0.0.1.4,<0.0.2.0)
+Requires-Dist: js2py (>=0.74,<0.75)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Project-URL: Changelog, https://github.com/mraniki/MyLLM/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/MyLLM/issues
 Project-URL: Support, https://github.com/mraniki/MyLLM/discussions
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: myllm Version: 1.2.6 Summary: A python package to
+Metadata-Version: 2.1 Name: myllm Version: 1.2.7 Summary: A python package to
 interact with llm model supported by g4f License: MIT Keywords:
 chatgpt,llm,ai,llama,ai,g4f,freegpt Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
-(>=3.1.12,<4.0.0) Requires-Dist: g4f (>=0.0.1,<0.0.2) Requires-Dist: loguru
-(>=0.7.0,<0.8.0) Project-URL: Changelog, https://github.com/mraniki/MyLLM/blob/
-dev/CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/MyLLM/issues
-Project-URL: Support, https://github.com/mraniki/MyLLM/discussions Description-
-Content-Type: text/markdown
+(>=3.1.12,<4.0.0) Requires-Dist: g4f (>=0.0.1.4,<0.0.2.0) Requires-Dist: js2py
+(>=0.74,<0.75) Requires-Dist: loguru (>=0.7.0,<0.8.0) Project-URL: Changelog,
+https://github.com/mraniki/MyLLM/blob/dev/CHANGELOG.rst Project-URL: Issues,
+https://github.com/mraniki/MyLLM/issues Project-URL: Support, https://
+github.com/mraniki/MyLLM/discussions Description-Content-Type: text/markdown
 [https://img.shields.io/badge/Wiki-
 %23000000.svg?style=for-the-
 badge&logo=wikipedia&logoColor=white] [https:/
 /img.shields.io/badge/github-                                     [Logo]
 %23000000.svg?style=for-the-
 badge&logo=github&logoColor=white]
 [https://img.shields.io/docker/pulls/mraniki/
```

