# Comparing `tmp/atksh-utils-0.4.1.tar.gz` & `tmp/atksh-utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.4.1.tar", last modified: Mon Aug  7 01:24:59 2023, max compression
+gzip compressed data, was "atksh-utils-0.4.2.tar", last modified: Mon Aug  7 01:47:36 2023, max compression
```

## Comparing `atksh-utils-0.4.1.tar` & `atksh-utils-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.124282 atksh-utils-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.124282 atksh-utils-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.124282 atksh-utils-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.124282 atksh-utils-0.4.1/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1763 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/askgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/src/atksh_utils/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 01:24:58.000000 atksh-utils-0.4.1/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 01:24:59.000000 atksh-utils-0.4.1/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.124282 atksh-utils-0.4.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:24:59.128282 atksh-utils-0.4.1/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-07 01:24:46.000000 atksh-utils-0.4.1/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:47:36.117096 atksh-utils-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:47:36.117096 atksh-utils-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:47:36.117096 atksh-utils-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-07 01:47:36.117096 atksh-utils-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 01:47:36.117096 atksh-utils-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:47:36.117096 atksh-utils-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:47:36.117096 atksh-utils-0.4.2/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:47:36.117096 atksh-utils-0.4.2/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/src/atksh_utils/openai/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1763 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/src/atksh_utils/openai/askgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 01:47:36.000000 atksh-utils-0.4.2/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:47:36.117096 atksh-utils-0.4.2/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-07 01:47:36.000000 atksh-utils-0.4.2/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-07 01:47:36.000000 atksh-utils-0.4.2/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 01:47:36.000000 atksh-utils-0.4.2/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 01:47:36.000000 atksh-utils-0.4.2/src/atksh_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-07 01:47:36.000000 atksh-utils-0.4.2/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 01:47:36.000000 atksh-utils-0.4.2/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:47:36.117096 atksh-utils-0.4.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 01:47:36.117096 atksh-utils-0.4.2/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-07 01:47:21.000000 atksh-utils-0.4.2/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.4.1/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.4.2/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.1/.gitignore` & `atksh-utils-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.1/LICENSE` & `atksh-utils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.1/PKG-INFO` & `atksh-utils-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.4.1/README.md` & `atksh-utils-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.1/pyproject.toml` & `atksh-utils-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 [project]
 dependencies = [
   "openai>=0.27.8",
   "beautifulsoup4>=4.12.2,<5.0.0",
   "requests>=2.26.0,<3.0.0",
   "duckduckgo_search>=3.8.3,<4.0.0",
+  "dill>=0.3.7,<0.4.0",
 ]
 description = "atksh's utils"
 dynamic = ["version"]
 license = {file = "LICENSE"}
 name = "atksh-utils"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `atksh-utils-0.4.1/src/atksh_utils/openai/api.py` & `atksh-utils-0.4.2/src/atksh_utils/openai/api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.1/src/atksh_utils/openai/askgpt.py` & `atksh-utils-0.4.2/src/atksh_utils/openai/askgpt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.1/src/atksh_utils/openai/functional.py` & `atksh-utils-0.4.2/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.1/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.4.2/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.1/src/atksh_utils/openai/tool.py` & `atksh-utils-0.4.2/src/atksh_utils/openai/tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 import subprocess
 import tempfile
 import time
+from code import InteractiveConsole
 from itertools import islice
+from typing import Any
 
 import requests
 from bs4 import BeautifulSoup as bs4
 from duckduckgo_search import DDGS
 
 from .prompt import SEARCH_RESULT_SUMMARIZE_PROMPT, VISIT_PAGE_SUMMARIZE_PROMPT
 
@@ -70,15 +72,15 @@
             ret = f"Error: {e}.\nPlease try again or try another url."
         return ret
 
     return web_search, visit_page
 
 
 def exec_python_code(code: str) -> str:
-    """This is a function that executes Python code and returns the stdout. Don't forget to print the result.
+    """This is a function that executes Python code and returns the stdout. Don't forget to print the result. Note that the session is not saved. So, you must import the modules you need every time.
 
     :param code: Python code of multiple lines. You must print the result. For example, `value = 2 + 3; print(value)`.
     :type code: str
     :return: The result of the execution of the Python code (stdout by print)
     :rtype: str
     """
     with tempfile.NamedTemporaryFile(mode="w", suffix=".py") as f:
```

### Comparing `atksh-utils-0.4.1/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.4.2/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.4.1/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.4.2/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.1/tests/openai/test_api.py` & `atksh-utils-0.4.2/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.4.1/tests/openai/test_functional.py` & `atksh-utils-0.4.2/tests/openai/test_functional.py`

 * *Files identical despite different names*

