# Comparing `tmp/myllm-1.2.5.tar.gz` & `tmp/myllm-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myllm-1.2.5.tar", max compression
+gzip compressed data, was "myllm-1.2.6.tar", max compression
```

## Comparing `myllm-1.2.5.tar` & `myllm-1.2.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-08-07 14:45:11.598017 myllm-1.2.5/LICENSE
--rw-r--r--   0        0        0     2230 2023-08-07 14:45:11.598017 myllm-1.2.5/README.md
--rw-r--r--   0        0        0       96 2023-08-07 14:45:12.822035 myllm-1.2.5/myllm/__init__.py
--rw-r--r--   0        0        0      701 2023-08-07 14:45:11.598017 myllm-1.2.5/myllm/config.py
--rw-r--r--   0        0        0     1313 2023-08-07 14:45:11.598017 myllm-1.2.5/myllm/default_settings.toml
--rw-r--r--   0        0        0     1731 2023-08-07 14:45:11.598017 myllm-1.2.5/myllm/main.py
--rw-r--r--   0        0        0     3039 2023-08-07 14:45:12.814035 myllm-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 myllm-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-07 17:06:56.330047 myllm-1.2.6/LICENSE
+-rw-r--r--   0        0        0     2230 2023-08-07 17:06:56.330047 myllm-1.2.6/README.md
+-rw-r--r--   0        0        0       96 2023-08-07 17:06:57.786044 myllm-1.2.6/myllm/__init__.py
+-rw-r--r--   0        0        0      701 2023-08-07 17:06:56.330047 myllm-1.2.6/myllm/config.py
+-rw-r--r--   0        0        0     1313 2023-08-07 17:06:56.330047 myllm-1.2.6/myllm/default_settings.toml
+-rw-r--r--   0        0        0     3203 2023-08-07 17:06:56.330047 myllm-1.2.6/myllm/main.py
+-rw-r--r--   0        0        0     3033 2023-08-07 17:06:57.774044 myllm-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 myllm-1.2.6/PKG-INFO
```

### Comparing `myllm-1.2.5/LICENSE` & `myllm-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `myllm-1.2.5/README.md` & `myllm-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `myllm-1.2.5/myllm/config.py` & `myllm-1.2.6/myllm/config.py`

 * *Files identical despite different names*

### Comparing `myllm-1.2.5/myllm/default_settings.toml` & `myllm-1.2.6/myllm/default_settings.toml`

 * *Files identical despite different names*

### Comparing `myllm-1.2.5/pyproject.toml` & `myllm-1.2.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "MyLLM"
-version = "1.2.5"
+version = "1.2.6"
 description = "A python package to interact with llm model supported by g4f"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["chatgpt","llm","ai","llama","ai", "g4f", "freegpt"]
 packages = [
     {include = "myllm"}
@@ -23,19 +23,19 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 loguru = "^0.7.0"
 g4f = "^0.0.1"
-langchain = "^0.0.255"
+# langchain = "^0.0.255"
 # libre-chat = "^0.0.4"
 # huggingface_hub = "^v0.16.4"
 # google-search-results = "^2.4.2"
-# cohere
+
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^8.0.2"
 ruff = ">=0.0.280,<0.0.283"
 
 [tool.ruff]
 select = [
```

### Comparing `myllm-1.2.5/PKG-INFO` & `myllm-1.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: myllm
-Version: 1.2.5
+Version: 1.2.6
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
 Requires-Dist: g4f (>=0.0.1,<0.0.2)
-Requires-Dist: langchain (>=0.0.255,<0.0.256)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Project-URL: Changelog, https://github.com/mraniki/MyLLM/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/MyLLM/issues
 Project-URL: Support, https://github.com/mraniki/MyLLM/discussions
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: myllm Version: 1.2.5 Summary: A python package to
+Metadata-Version: 2.1 Name: myllm Version: 1.2.6 Summary: A python package to
 interact with llm model supported by g4f License: MIT Keywords:
 chatgpt,llm,ai,llama,ai,g4f,freegpt Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
-(>=3.1.12,<4.0.0) Requires-Dist: g4f (>=0.0.1,<0.0.2) Requires-Dist: langchain
-(>=0.0.255,<0.0.256) Requires-Dist: loguru (>=0.7.0,<0.8.0) Project-URL:
-Changelog, https://github.com/mraniki/MyLLM/blob/dev/CHANGELOG.rst Project-URL:
-Issues, https://github.com/mraniki/MyLLM/issues Project-URL: Support, https://
-github.com/mraniki/MyLLM/discussions Description-Content-Type: text/markdown
+(>=3.1.12,<4.0.0) Requires-Dist: g4f (>=0.0.1,<0.0.2) Requires-Dist: loguru
+(>=0.7.0,<0.8.0) Project-URL: Changelog, https://github.com/mraniki/MyLLM/blob/
+dev/CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/MyLLM/issues
+Project-URL: Support, https://github.com/mraniki/MyLLM/discussions Description-
+Content-Type: text/markdown
 [https://img.shields.io/badge/Wiki-
 %23000000.svg?style=for-the-
 badge&logo=wikipedia&logoColor=white] [https:/
 /img.shields.io/badge/github-                                     [Logo]
 %23000000.svg?style=for-the-
 badge&logo=github&logoColor=white]
 [https://img.shields.io/docker/pulls/mraniki/
```

