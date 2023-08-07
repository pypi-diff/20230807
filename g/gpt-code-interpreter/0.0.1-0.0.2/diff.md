# Comparing `tmp/gpt_code_interpreter-0.0.1.tar.gz` & `tmp/gpt_code_interpreter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_code_interpreter-0.0.1.tar", max compression
+gzip compressed data, was "gpt_code_interpreter-0.0.2.tar", max compression
```

## Comparing `gpt_code_interpreter-0.0.1.tar` & `gpt_code_interpreter-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2023-08-04 04:23:37.688355 gpt_code_interpreter-0.0.1/LICENSE
--rw-r--r--   0        0        0     4556 2023-08-04 04:23:37.688473 gpt_code_interpreter-0.0.1/README.md
--rw-r--r--   0        0        0      109 2023-08-07 00:57:39.236766 gpt_code_interpreter-0.0.1/gpt_code_interpreter/__init__.py
--rw-r--r--   0        0        0       50 2023-08-07 01:03:01.758108 gpt_code_interpreter-0.0.1/gpt_code_interpreter/agents/__init__.py
--rw-r--r--   0        0        0      101 2023-08-04 04:53:06.486250 gpt_code_interpreter-0.0.1/gpt_code_interpreter/agents/custom_agent.py
--rw-r--r--   0        0        0     9989 2023-08-04 04:53:06.486351 gpt_code_interpreter-0.0.1/gpt_code_interpreter/agents/functions_agent.py
--rw-r--r--   0        0        0      147 2023-08-04 04:53:06.486432 gpt_code_interpreter-0.0.1/gpt_code_interpreter/chains/__init__.py
--rw-r--r--   0        0        0     1002 2023-08-07 00:57:53.882274 gpt_code_interpreter-0.0.1/gpt_code_interpreter/chains/extract_code.py
--rw-r--r--   0        0        0     1459 2023-08-07 00:57:55.199190 gpt_code_interpreter-0.0.1/gpt_code_interpreter/chains/modifications_check.py
--rw-r--r--   0        0        0      979 2023-08-07 00:57:57.252365 gpt_code_interpreter-0.0.1/gpt_code_interpreter/chains/rm_dl_link.py
--rw-r--r--   0        0        0      390 2023-08-04 04:53:06.486666 gpt_code_interpreter-0.0.1/gpt_code_interpreter/config.py
--rw-r--r--   0        0        0      191 2023-08-04 04:53:06.486735 gpt_code_interpreter-0.0.1/gpt_code_interpreter/prompts/__init__.py
--rw-r--r--   0        0        0     1869 2023-08-04 04:53:06.486789 gpt_code_interpreter-0.0.1/gpt_code_interpreter/prompts/modifications_check.py
--rw-r--r--   0        0        0      959 2023-08-04 04:53:06.486841 gpt_code_interpreter-0.0.1/gpt_code_interpreter/prompts/remove_dl_link.py
--rw-r--r--   0        0        0     1600 2023-08-04 04:53:06.486896 gpt_code_interpreter-0.0.1/gpt_code_interpreter/prompts/system_message.py
--rw-r--r--   0        0        0      122 2023-08-04 04:53:06.486970 gpt_code_interpreter-0.0.1/gpt_code_interpreter/schema/__init__.py
--rw-r--r--   0        0        0     2403 2023-08-07 00:57:58.759502 gpt_code_interpreter-0.0.1/gpt_code_interpreter/schema/file.py
--rw-r--r--   0        0        0      123 2023-08-04 04:53:06.487091 gpt_code_interpreter-0.0.1/gpt_code_interpreter/schema/input.py
--rw-r--r--   0        0        0      752 2023-08-04 04:53:06.487145 gpt_code_interpreter-0.0.1/gpt_code_interpreter/schema/response.py
--rw-r--r--   0        0        0    11327 2023-08-07 01:28:26.619979 gpt_code_interpreter-0.0.1/gpt_code_interpreter/session.py
--rw-r--r--   0        0        0      112 2023-08-04 04:53:06.487335 gpt_code_interpreter-0.0.1/gpt_code_interpreter/utils/__init__.py
--rw-r--r--   0        0        0      931 2023-08-07 00:57:59.636030 gpt_code_interpreter-0.0.1/gpt_code_interpreter/utils/callbacks.py
--rw-r--r--   0        0        0     2478 2023-08-07 00:58:00.263001 gpt_code_interpreter-0.0.1/gpt_code_interpreter/utils/parser.py
--rw-r--r--   0        0        0      803 2023-08-07 00:56:39.116528 gpt_code_interpreter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5482 1970-01-01 00:00:00.000000 gpt_code_interpreter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-04 04:23:37.688355 gpt_code_interpreter-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4556 2023-08-04 04:23:37.688473 gpt_code_interpreter-0.0.2/README.md
+-rw-r--r--   0        0        0      109 2023-08-07 00:57:39.236766 gpt_code_interpreter-0.0.2/gpt_code_interpreter/__init__.py
+-rw-r--r--   0        0        0       50 2023-08-07 01:03:01.758108 gpt_code_interpreter-0.0.2/gpt_code_interpreter/agents/__init__.py
+-rw-r--r--   0        0        0      101 2023-08-04 04:53:06.486250 gpt_code_interpreter-0.0.2/gpt_code_interpreter/agents/custom_agent.py
+-rw-r--r--   0        0        0     9989 2023-08-04 04:53:06.486351 gpt_code_interpreter-0.0.2/gpt_code_interpreter/agents/functions_agent.py
+-rw-r--r--   0        0        0      147 2023-08-04 04:53:06.486432 gpt_code_interpreter-0.0.2/gpt_code_interpreter/chains/__init__.py
+-rw-r--r--   0        0        0     1002 2023-08-07 00:57:53.882274 gpt_code_interpreter-0.0.2/gpt_code_interpreter/chains/extract_code.py
+-rw-r--r--   0        0        0     1459 2023-08-07 00:57:55.199190 gpt_code_interpreter-0.0.2/gpt_code_interpreter/chains/modifications_check.py
+-rw-r--r--   0        0        0      979 2023-08-07 00:57:57.252365 gpt_code_interpreter-0.0.2/gpt_code_interpreter/chains/rm_dl_link.py
+-rw-r--r--   0        0        0      390 2023-08-04 04:53:06.486666 gpt_code_interpreter-0.0.2/gpt_code_interpreter/config.py
+-rw-r--r--   0        0        0      191 2023-08-04 04:53:06.486735 gpt_code_interpreter-0.0.2/gpt_code_interpreter/prompts/__init__.py
+-rw-r--r--   0        0        0     1869 2023-08-04 04:53:06.486789 gpt_code_interpreter-0.0.2/gpt_code_interpreter/prompts/modifications_check.py
+-rw-r--r--   0        0        0      959 2023-08-04 04:53:06.486841 gpt_code_interpreter-0.0.2/gpt_code_interpreter/prompts/remove_dl_link.py
+-rw-r--r--   0        0        0     1600 2023-08-04 04:53:06.486896 gpt_code_interpreter-0.0.2/gpt_code_interpreter/prompts/system_message.py
+-rw-r--r--   0        0        0      122 2023-08-04 04:53:06.486970 gpt_code_interpreter-0.0.2/gpt_code_interpreter/schema/__init__.py
+-rw-r--r--   0        0        0     2403 2023-08-07 00:57:58.759502 gpt_code_interpreter-0.0.2/gpt_code_interpreter/schema/file.py
+-rw-r--r--   0        0        0      123 2023-08-04 04:53:06.487091 gpt_code_interpreter-0.0.2/gpt_code_interpreter/schema/input.py
+-rw-r--r--   0        0        0      752 2023-08-04 04:53:06.487145 gpt_code_interpreter-0.0.2/gpt_code_interpreter/schema/response.py
+-rw-r--r--   0        0        0    11327 2023-08-07 01:28:26.619979 gpt_code_interpreter-0.0.2/gpt_code_interpreter/session.py
+-rw-r--r--   0        0        0      112 2023-08-04 04:53:06.487335 gpt_code_interpreter-0.0.2/gpt_code_interpreter/utils/__init__.py
+-rw-r--r--   0        0        0      931 2023-08-07 00:57:59.636030 gpt_code_interpreter-0.0.2/gpt_code_interpreter/utils/callbacks.py
+-rw-r--r--   0        0        0     2478 2023-08-07 00:58:00.263001 gpt_code_interpreter-0.0.2/gpt_code_interpreter/utils/parser.py
+-rw-r--r--   0        0        0      803 2023-08-07 07:31:16.493634 gpt_code_interpreter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5482 1970-01-01 00:00:00.000000 gpt_code_interpreter-0.0.2/PKG-INFO
```

### Comparing `gpt_code_interpreter-0.0.1/LICENSE` & `gpt_code_interpreter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/README.md` & `gpt_code_interpreter-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/agents/functions_agent.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/agents/functions_agent.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/chains/extract_code.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/chains/extract_code.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/chains/modifications_check.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/chains/modifications_check.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/chains/rm_dl_link.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/chains/rm_dl_link.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/prompts/modifications_check.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/prompts/modifications_check.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/prompts/remove_dl_link.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/prompts/remove_dl_link.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/prompts/system_message.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/prompts/system_message.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/schema/file.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/schema/file.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/schema/response.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/schema/response.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/session.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/session.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/utils/callbacks.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/gpt_code_interpreter/utils/parser.py` & `gpt_code_interpreter-0.0.2/gpt_code_interpreter/utils/parser.py`

 * *Files identical despite different names*

### Comparing `gpt_code_interpreter-0.0.1/pyproject.toml` & `gpt_code_interpreter-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "gpt-code-interpreter"
-version = "0.0.1"
+version = "0.0.2"
 description = "CodeInterpreterAPI is an (unofficial) open source python interface for the ChatGPT CodeInterpreter."
 authors = ["Shroominic <contact@shroominic.com>", "Sangwoo Han <swhan0906@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 python-dotenv = "^1.0.0"
 openai = "^0.27.8"
-langchain = "^0.0.242"
+langchain = "^0.0.238"
 codeboxapi = "^0.0.14"
 
 [tool.poetry.extras]
 all = ["jupyter-kernel-gateway", "streamlit", "Pillow"]
 localbox = ["jupyter-kernel-gateway"]
 frontend = ["streamlit"]
 image_support = ["Pillow"]
```

### Comparing `gpt_code_interpreter-0.0.1/PKG-INFO` & `gpt_code_interpreter-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-code-interpreter
-Version: 0.0.1
+Version: 0.0.2
 Summary: CodeInterpreterAPI is an (unofficial) open source python interface for the ChatGPT CodeInterpreter.
 License: MIT
 Author: Shroominic
 Author-email: contact@shroominic.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: frontend
 Provides-Extra: image-support
 Provides-Extra: localbox
 Requires-Dist: codeboxapi (>=0.0.14,<0.0.15)
-Requires-Dist: langchain (>=0.0.242,<0.0.243)
+Requires-Dist: langchain (>=0.0.238,<0.0.239)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Code Interpreter API
 
 A LangChain implementation of the ChatGPT Code Interpreter.
```

