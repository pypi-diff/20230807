# Comparing `tmp/python-define-1.1.3.tar.gz` & `tmp/python-define-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-define-1.1.3.tar", last modified: Mon Aug  7 01:21:08 2023, max compression
+gzip compressed data, was "python-define-1.1.4.tar", last modified: Mon Aug  7 01:46:28 2023, max compression
```

## Comparing `python-define-1.1.3.tar` & `python-define-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-08-07 01:21:08.742864 python-define-1.1.3/
--rw-r--r--   0 grant     (1000) grant     (1000)    34523 2023-06-29 07:50:39.000000 python-define-1.1.3/LICENSE
--rw-r--r--   0 grant     (1000) grant     (1000)    44890 2023-08-07 01:21:08.742864 python-define-1.1.3/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)     4411 2023-08-07 01:18:14.000000 python-define-1.1.3/README.md
--rwxr-xr-x   0 grant     (1000) grant     (1000)     5620 2023-07-20 11:52:42.000000 python-define-1.1.3/define.py
--rw-r--r--   0 grant     (1000) grant     (1000)      775 2023-08-07 01:19:02.000000 python-define-1.1.3/pyproject.toml
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-08-07 01:21:08.742864 python-define-1.1.3/python_define.egg-info/
--rw-r--r--   0 grant     (1000) grant     (1000)    44890 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)      266 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/SOURCES.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        1 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/dependency_links.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/entry_points.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       13 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/requires.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        7 2023-08-07 01:21:08.000000 python-define-1.1.3/python_define.egg-info/top_level.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-08-07 01:21:08.742864 python-define-1.1.3/setup.cfg
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-08-07 01:46:28.467297 python-define-1.1.4/
+-rw-r--r--   0 grant     (1000) grant     (1000)    34523 2023-06-29 07:50:39.000000 python-define-1.1.4/LICENSE
+-rw-r--r--   0 grant     (1000) grant     (1000)    44890 2023-08-07 01:46:28.467297 python-define-1.1.4/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)     4411 2023-08-07 01:18:14.000000 python-define-1.1.4/README.md
+-rwxr-xr-x   0 grant     (1000) grant     (1000)     5605 2023-08-07 01:42:49.000000 python-define-1.1.4/define.py
+-rw-r--r--   0 grant     (1000) grant     (1000)      775 2023-08-07 01:45:16.000000 python-define-1.1.4/pyproject.toml
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-08-07 01:46:28.467297 python-define-1.1.4/python_define.egg-info/
+-rw-r--r--   0 grant     (1000) grant     (1000)    44890 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)      266 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/SOURCES.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        1 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/dependency_links.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/entry_points.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       13 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/requires.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        7 2023-08-07 01:46:28.000000 python-define-1.1.4/python_define.egg-info/top_level.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-08-07 01:46:28.467297 python-define-1.1.4/setup.cfg
```

### Comparing `python-define-1.1.3/LICENSE` & `python-define-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-define-1.1.3/PKG-INFO` & `python-define-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.1.3
+Version: 1.1.4
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `python-define-1.1.3/README.md` & `python-define-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `python-define-1.1.3/define.py` & `python-define-1.1.4/define.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,30 +62,30 @@
 
 I will ask you questions about the **English Language**, and you will provide the answers.
 
 Your answers will be **short and concise**.
 
 If I supply you with a **single word**, I want you to **correct spelling mistakes** and **define that word**.
 
-Expect me to be supplying you will spelling mistakes. Do your best to determine what word I am trying to understand.
+Expect me to be supplying you with spelling mistakes. Do your best to determine what word I am trying to understand.
 
 Use the **phonetic sound** of the letters to try and determine what word I am trying to learn.
 
 ## Requirements
 
 - **Correct mistakes** such as spelling, grammar, and others.
 - Keep your answers **short** unless asked to expand.
 - **Single words** are a **request for an answer**, not a statement.
 - **I will never complement you**, I need you to define the words.
 
 ## Constraints
 
 - Your answers will be for the **English Language**.
-- The users locale value is: **{{locale}}**.
-- Ensure you answer with the users **locale** values in mind.
+- My locale value is: **{{locale}}**.
+- Ensure you answer with my **locale** value in mind.
 - **State the differences between English locale spellings**.
 - If it looks like I am commenting to you or complementing you, I am not, I am asking for an answer.
 
 ## Answer Format
 
 Spelling <locale>: <correct-spelling>
 <list-of-alternate-spellings-if-they-exist-for-different-locales-omit-if-there-is-no-difference>
```

### Comparing `python-define-1.1.3/pyproject.toml` & `python-define-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-define"
-version = "1.1.3"
+version = "1.1.4"
 description = "An OpenAI powered command-line linguistics assistant"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Grant Carthew", email = "grant@carthew.net"},
 ]
```

### Comparing `python-define-1.1.3/python_define.egg-info/PKG-INFO` & `python-define-1.1.4/python_define.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.1.3
+Version: 1.1.4
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

