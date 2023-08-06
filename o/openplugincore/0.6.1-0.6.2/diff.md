# Comparing `tmp/openplugincore-0.6.1.tar.gz` & `tmp/openplugincore-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugincore-0.6.1.tar", last modified: Sun Jul 30 02:24:33 2023, max compression
+gzip compressed data, was "openplugincore-0.6.2.tar", last modified: Sun Aug  6 23:57:27 2023, max compression
```

## Comparing `openplugincore-0.6.1.tar` & `openplugincore-0.6.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:33.622072 openplugincore-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 02:24:33.622072 openplugincore-0.6.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:33.622072 openplugincore-0.6.1/openplugincore/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/openplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/openplugin_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/openplugin_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:33.622072 openplugincore-0.6.1/openplugincore/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-30 02:24:19.000000 openplugincore-0.6.1/openplugincore/utils/prompting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:33.622072 openplugincore-0.6.1/openplugincore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 02:24:33.000000 openplugincore-0.6.1/openplugincore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-30 02:24:33.000000 openplugincore-0.6.1/openplugincore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:24:33.000000 openplugincore-0.6.1/openplugincore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-30 02:24:33.000000 openplugincore-0.6.1/openplugincore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-30 02:24:33.000000 openplugincore-0.6.1/openplugincore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 02:24:33.622072 openplugincore-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-30 02:24:19.000000 openplugincore-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:33.622072 openplugincore-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/test_openplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/test_openplugin_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-30 02:24:19.000000 openplugincore-0.6.1/tests/test_openplugin_memo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:57:27.087191 openplugincore-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-06 23:57:27.087191 openplugincore-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-08-06 23:57:14.000000 openplugincore-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:57:27.083191 openplugincore-0.6.2/openplugincore/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-06 23:57:14.000000 openplugincore-0.6.2/openplugincore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-08-06 23:57:14.000000 openplugincore-0.6.2/openplugincore/openplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-06 23:57:14.000000 openplugincore-0.6.2/openplugincore/openplugin_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-06 23:57:14.000000 openplugincore-0.6.2/openplugincore/openplugin_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-06 23:57:14.000000 openplugincore-0.6.2/openplugincore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:57:27.083191 openplugincore-0.6.2/openplugincore/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 23:57:14.000000 openplugincore-0.6.2/openplugincore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-06 23:57:14.000000 openplugincore-0.6.2/openplugincore/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-08-06 23:57:14.000000 openplugincore-0.6.2/openplugincore/utils/prompting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:57:27.083191 openplugincore-0.6.2/openplugincore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-06 23:57:26.000000 openplugincore-0.6.2/openplugincore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 23:57:27.000000 openplugincore-0.6.2/openplugincore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 23:57:26.000000 openplugincore-0.6.2/openplugincore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-06 23:57:26.000000 openplugincore-0.6.2/openplugincore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-06 23:57:26.000000 openplugincore-0.6.2/openplugincore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 23:57:27.087191 openplugincore-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-06 23:57:14.000000 openplugincore-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:57:27.087191 openplugincore-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 23:57:14.000000 openplugincore-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-06 23:57:14.000000 openplugincore-0.6.2/tests/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-08-06 23:57:14.000000 openplugincore-0.6.2/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-08-06 23:57:14.000000 openplugincore-0.6.2/tests/test_openplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-06 23:57:14.000000 openplugincore-0.6.2/tests/test_openplugin_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-06 23:57:14.000000 openplugincore-0.6.2/tests/test_openplugin_memo.py
```

### Comparing `openplugincore-0.6.1/PKG-INFO` & `openplugincore-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugincore
-Version: 0.6.1
+Version: 0.6.2
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugincore-0.6.1/openplugincore/openplugin.py` & `openplugincore-0.6.2/openplugincore/openplugin.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.1/openplugincore/openplugin_completion.py` & `openplugincore-0.6.2/openplugincore/openplugin_completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import openai
 from dotenv import load_dotenv
 from .openplugin import OpenPlugin
 load_dotenv()
 
 OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
 
-def openplugin_completion(openai_api_key: str, messages: list[dict], plugin_name: str = None, root_url: str = None, **chatgpt_args):
+def openplugin_completion(openai_api_key: str, messages: list[dict], truncate: bool = True, plugin_name: str = None, root_url: str = None, **chatgpt_args):
     # set environment variable to 
     os.environ["OPENAI_API_KEY"] = openai_api_key
     openai.api_key = openai_api_key
     if not plugin_name and not root_url:
         return openai.ChatCompletion.create(
             **chatgpt_args,
             messages=messages
         )
     plugin = OpenPlugin(plugin_name=plugin_name, root_url=root_url, openai_api_key=openai_api_key)
     try:
         function_response = plugin.fetch_plugin(
             messages=messages,
+            truncate=truncate,
             **chatgpt_args
         )
     except ValueError as e:
         if "Not a plugin function" in str(e):
             return openai.ChatCompletion.create(
                 **chatgpt_args,
                 messages=messages
```

### Comparing `openplugincore-0.6.1/openplugincore/openplugin_memo.py` & `openplugincore-0.6.2/openplugincore/openplugin_memo.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.1/openplugincore/types.py` & `openplugincore-0.6.2/openplugincore/types.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.1/openplugincore/utils/prompting.py` & `openplugincore-0.6.2/openplugincore/utils/prompting.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.1/openplugincore.egg-info/PKG-INFO` & `openplugincore-0.6.2/openplugincore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugincore
-Version: 0.6.1
+Version: 0.6.2
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugincore-0.6.1/openplugincore.egg-info/SOURCES.txt` & `openplugincore-0.6.2/openplugincore.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 openplugincore/__init__.py
 openplugincore/openplugin.py
 openplugincore/openplugin_completion.py
 openplugincore/openplugin_memo.py
 openplugincore/types.py
 openplugincore.egg-info/PKG-INFO
```

### Comparing `openplugincore-0.6.1/setup.py` & `openplugincore-0.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name='openplugincore', 
-        version="0.6.1",
+        version="0.6.2",
         author="Sebastian Sosa",
         author_email="1sebastian1sosa1@gmail.com",
         description='Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         long_description='Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         packages=find_packages(),
         package_data={
             "openplugincore": ["*.json"],  # include all .json files in the openplugin package
```

### Comparing `openplugincore-0.6.1/tests/mock_data.py` & `openplugincore-0.6.2/tests/mock_data.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.1/tests/test_e2e.py` & `openplugincore-0.6.2/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.1/tests/test_openplugin.py` & `openplugincore-0.6.2/tests/test_openplugin.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.1/tests/test_openplugin_completion.py` & `openplugincore-0.6.2/tests/test_openplugin_completion.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.6.1/tests/test_openplugin_memo.py` & `openplugincore-0.6.2/tests/test_openplugin_memo.py`

 * *Files identical despite different names*

