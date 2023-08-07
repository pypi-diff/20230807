# Comparing `tmp/myllm-1.2.3.tar.gz` & `tmp/myllm-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myllm-1.2.3.tar", max compression
+gzip compressed data, was "myllm-1.2.4.tar", max compression
```

## Comparing `myllm-1.2.3.tar` & `myllm-1.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-08-07 12:06:31.950397 myllm-1.2.3/LICENSE
--rw-r--r--   0        0        0     2230 2023-08-07 12:06:31.950397 myllm-1.2.3/README.md
--rw-r--r--   0        0        0       96 2023-08-07 12:06:33.350397 myllm-1.2.3/myllm/__init__.py
--rw-r--r--   0        0        0      701 2023-08-07 12:06:31.950397 myllm-1.2.3/myllm/config.py
--rw-r--r--   0        0        0     1313 2023-08-07 12:06:31.950397 myllm-1.2.3/myllm/default_settings.toml
--rw-r--r--   0        0        0     1731 2023-08-07 12:06:31.950397 myllm-1.2.3/myllm/main.py
--rw-r--r--   0        0        0     3039 2023-08-07 12:06:33.342397 myllm-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 myllm-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-07 14:02:18.161261 myllm-1.2.4/LICENSE
+-rw-r--r--   0        0        0     2230 2023-08-07 14:02:18.161261 myllm-1.2.4/README.md
+-rw-r--r--   0        0        0       96 2023-08-07 14:02:19.173269 myllm-1.2.4/myllm/__init__.py
+-rw-r--r--   0        0        0      701 2023-08-07 14:02:18.161261 myllm-1.2.4/myllm/config.py
+-rw-r--r--   0        0        0     1313 2023-08-07 14:02:18.161261 myllm-1.2.4/myllm/default_settings.toml
+-rw-r--r--   0        0        0     1731 2023-08-07 14:02:18.161261 myllm-1.2.4/myllm/main.py
+-rw-r--r--   0        0        0     3039 2023-08-07 14:02:19.165269 myllm-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 myllm-1.2.4/PKG-INFO
```

### Comparing `myllm-1.2.3/LICENSE` & `myllm-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `myllm-1.2.3/README.md` & `myllm-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `myllm-1.2.3/myllm/config.py` & `myllm-1.2.4/myllm/config.py`

 * *Files identical despite different names*

### Comparing `myllm-1.2.3/myllm/default_settings.toml` & `myllm-1.2.4/myllm/default_settings.toml`

 * *Files identical despite different names*

### Comparing `myllm-1.2.3/myllm/main.py` & `myllm-1.2.4/myllm/main.py`

 * *Files identical despite different names*

### Comparing `myllm-1.2.3/pyproject.toml` & `myllm-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "MyLLM"
-version = "1.2.3"
+version = "1.2.4"
 description = "A python package to interact with llm model supported by g4f"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["chatgpt","llm","ai","llama","ai", "g4f", "freegpt"]
 packages = [
     {include = "myllm"}
```

### Comparing `myllm-1.2.3/PKG-INFO` & `myllm-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myllm
-Version: 1.2.3
+Version: 1.2.4
 Summary: A python package to interact with llm model supported by g4f
 License: MIT
 Keywords: chatgpt,llm,ai,llama,ai,g4f,freegpt
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: myllm Version: 1.2.3 Summary: A python package to
+Metadata-Version: 2.1 Name: myllm Version: 1.2.4 Summary: A python package to
 interact with llm model supported by g4f License: MIT Keywords:
 chatgpt,llm,ai,llama,ai,g4f,freegpt Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: g4f (>=0.0.1,<0.0.2) Requires-Dist: langchain
```

