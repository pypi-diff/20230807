# Comparing `tmp/python-define-1.1.2.tar.gz` & `tmp/python-define-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-define-1.1.2.tar", last modified: Thu Jul 20 11:55:25 2023, max compression
+gzip compressed data, was "python-define-1.1.3.tar", last modified: Mon Aug  7 01:21:08 2023, max compression
```

## Comparing `python-define-1.1.2.tar` & `python-define-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-07-20 11:55:25.898506 python-define-1.1.2/
--rw-r--r--   0 grant     (1000) grant     (1000)    34523 2023-06-29 07:50:39.000000 python-define-1.1.2/LICENSE
--rw-r--r--   0 grant     (1000) grant     (1000)    44847 2023-07-20 11:55:25.898506 python-define-1.1.2/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)     4368 2023-07-18 02:55:31.000000 python-define-1.1.2/README.md
--rwxr-xr-x   0 grant     (1000) grant     (1000)     5620 2023-07-20 11:52:42.000000 python-define-1.1.2/define.py
--rw-r--r--   0 grant     (1000) grant     (1000)      775 2023-07-20 11:54:08.000000 python-define-1.1.2/pyproject.toml
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-07-20 11:55:25.898506 python-define-1.1.2/python_define.egg-info/
--rw-r--r--   0 grant     (1000) grant     (1000)    44847 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)      266 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/SOURCES.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        1 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/dependency_links.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/entry_points.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       13 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/requires.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        7 2023-07-20 11:55:25.000000 python-define-1.1.2/python_define.egg-info/top_level.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-07-20 11:55:25.898506 python-define-1.1.2/setup.cfg
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-08-07 01:21:08.742864 python-define-1.1.3/
+-rw-r--r--   0 grant     (1000) grant     (1000)    34523 2023-06-29 07:50:39.000000 python-define-1.1.3/LICENSE
+-rw-r--r--   0 grant     (1000) grant     (1000)    44890 2023-08-07 01:21:08.742864 python-define-1.1.3/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)     4411 2023-08-07 01:18:14.000000 python-define-1.1.3/README.md
+-rwxr-xr-x   0 grant     (1000) grant     (1000)     5620 2023-07-20 11:52:42.000000 python-define-1.1.3/define.py
+-rw-r--r--   0 grant     (1000) grant     (1000)      775 2023-08-07 01:19:02.000000 python-define-1.1.3/pyproject.toml
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-08-07 01:21:08.742864 python-define-1.1.3/python_define.egg-info/
+-rw-r--r--   0 grant     (1000) grant     (1000)    44890 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)      266 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/SOURCES.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        1 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/dependency_links.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/entry_points.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       13 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/requires.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        7 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/top_level.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-08-07 01:21:08.742864 python-define-1.1.3/setup.cfg
```

### Comparing `python-define-1.1.2/LICENSE` & `python-define-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-define-1.1.2/PKG-INFO` & `python-define-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.1.2
+Version: 1.1.3
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -691,18 +691,20 @@
 
 - A general purpose OpenAI client
 - A free tool to use, you will need an [OpenAI API Key](https://platform.openai.com/account/api-keys)
 - Always perfect in its response
 
 ## Installation
 
+First install [pipx](https://pypa.github.io/pipx/)
+
 ```shell
 export OPENAI_API_KEY="<your-openai-api-key>"
 # echo 'export OPENAI_API_KEY="<your-openai-api-key>"' >> "${HOME}/.bashrc"
-python -m pip install python-define
+pipx install python-define
 ```
 
 Package Address: https://pypi.org/project/python-define/
 
 ## Examples
 
 ```markdown
```

### Comparing `python-define-1.1.2/README.md` & `python-define-1.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 
 - A general purpose OpenAI client
 - A free tool to use, you will need an [OpenAI API Key](https://platform.openai.com/account/api-keys)
 - Always perfect in its response
 
 ## Installation
 
+First install [pipx](https://pypa.github.io/pipx/)
+
 ```shell
 export OPENAI_API_KEY="<your-openai-api-key>"
 # echo 'export OPENAI_API_KEY="<your-openai-api-key>"' >> "${HOME}/.bashrc"
-python -m pip install python-define
+pipx install python-define
 ```
 
 Package Address: https://pypi.org/project/python-define/
 
 ## Examples
 
 ```markdown
```

### Comparing `python-define-1.1.2/define.py` & `python-define-1.1.3/define.py`

 * *Files identical despite different names*

### Comparing `python-define-1.1.2/pyproject.toml` & `python-define-1.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-define"
-version = "1.1.2"
+version = "1.1.3"
 description = "An OpenAI powered command-line linguistics assistant"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Grant Carthew", email = "grant@carthew.net"},
 ]
```

### Comparing `python-define-1.1.2/python_define.egg-info/PKG-INFO` & `python-define-1.1.3/python_define.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.1.2
+Version: 1.1.3
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -691,18 +691,20 @@
 
 - A general purpose OpenAI client
 - A free tool to use, you will need an [OpenAI API Key](https://platform.openai.com/account/api-keys)
 - Always perfect in its response
 
 ## Installation
 
+First install [pipx](https://pypa.github.io/pipx/)
+
 ```shell
 export OPENAI_API_KEY="<your-openai-api-key>"
 # echo 'export OPENAI_API_KEY="<your-openai-api-key>"' >> "${HOME}/.bashrc"
-python -m pip install python-define
+pipx install python-define
 ```
 
 Package Address: https://pypi.org/project/python-define/
 
 ## Examples
 
 ```markdown
```

