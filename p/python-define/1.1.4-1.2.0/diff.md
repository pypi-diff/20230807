# Comparing `tmp/python-define-1.1.4.tar.gz` & `tmp/python-define-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-define-1.1.4.tar", last modified: Mon Aug  7 01:46:28 2023, max compression
+gzip compressed data, was "python-define-1.2.0.tar", last modified: Mon Aug  7 02:00:44 2023, max compression
```

## Comparing `python-define-1.1.4.tar` & `python-define-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-08-07 01:46:28.467297 python-define-1.1.4/
--rw-r--r--   0 grant     (1000) grant     (1000)    34523 2023-06-29 07:50:39.000000 python-define-1.1.4/LICENSE
--rw-r--r--   0 grant     (1000) grant     (1000)    44890 2023-08-07 01:46:28.467297 python-define-1.1.4/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)     4411 2023-08-07 01:18:14.000000 python-define-1.1.4/README.md
--rwxr-xr-x   0 grant     (1000) grant     (1000)     5605 2023-08-07 01:42:49.000000 python-define-1.1.4/define.py
--rw-r--r--   0 grant     (1000) grant     (1000)      775 2023-08-07 01:45:16.000000 python-define-1.1.4/pyproject.toml
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-08-07 01:46:28.467297 python-define-1.1.4/python_define.egg-info/
--rw-r--r--   0 grant     (1000) grant     (1000)    44890 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)      266 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/SOURCES.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        1 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/dependency_links.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/entry_points.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       13 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/requires.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        7 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/top_level.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-08-07 01:46:28.467297 python-define-1.1.4/setup.cfg
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-08-07 02:00:44.726953 python-define-1.2.0/
+-rw-r--r--   0 grant     (1000) grant     (1000)    34523 2023-06-29 07:50:39.000000 python-define-1.2.0/LICENSE
+-rw-r--r--   0 grant     (1000) grant     (1000)    44890 2023-08-07 02:00:44.726953 python-define-1.2.0/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)     4411 2023-08-07 01:18:14.000000 python-define-1.2.0/README.md
+-rwxr-xr-x   0 grant     (1000) grant     (1000)     5692 2023-08-07 01:59:16.000000 python-define-1.2.0/define.py
+-rw-r--r--   0 grant     (1000) grant     (1000)      775 2023-08-07 01:59:47.000000 python-define-1.2.0/pyproject.toml
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-08-07 02:00:44.726953 python-define-1.2.0/python_define.egg-info/
+-rw-r--r--   0 grant     (1000) grant     (1000)    44890 2023-08-07 02:00:44.000000 python-define-1.2.0/python_define.egg-info/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)      266 2023-08-07 02:00:44.000000 python-define-1.2.0/python_define.egg-info/SOURCES.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        1 2023-08-07 02:00:44.000000 python-define-1.2.0/python_define.egg-info/dependency_links.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-08-07 02:00:44.000000 python-define-1.2.0/python_define.egg-info/entry_points.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       13 2023-08-07 02:00:44.000000 python-define-1.2.0/python_define.egg-info/requires.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        7 2023-08-07 02:00:44.000000 python-define-1.2.0/python_define.egg-info/top_level.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-08-07 02:00:44.726953 python-define-1.2.0/setup.cfg
```

### Comparing `python-define-1.1.4/LICENSE` & `python-define-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-define-1.1.4/PKG-INFO` & `python-define-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.1.4
+Version: 1.2.0
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `python-define-1.1.4/README.md` & `python-define-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python-define-1.1.4/define.py` & `python-define-1.2.0/define.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 
+from importlib.metadata import version
 from typing import List, Dict
 import click
 import locale
 import openai
 import os
 import sys
 
@@ -180,14 +181,15 @@
         'role': 'user',
         'content': user_content
     }
     ]
 
 
 @click.command()
+@click.version_option(version('python-define'))
 @click.argument('query')
 def cli(query: str) -> None:
     """An OpenAI-powered command-line linguistics assistant."""
 
     # Fetch the OpenAI API key from the environment variables
     openai.api_key = os.getenv('OPENAI_API_KEY')
     if not openai.api_key:
```

### Comparing `python-define-1.1.4/pyproject.toml` & `python-define-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-define"
-version = "1.1.4"
+version = "1.2.0"
 description = "An OpenAI powered command-line linguistics assistant"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Grant Carthew", email = "grant@carthew.net"},
 ]
```

### Comparing `python-define-1.1.4/python_define.egg-info/PKG-INFO` & `python-define-1.2.0/python_define.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.1.4
+Version: 1.2.0
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

