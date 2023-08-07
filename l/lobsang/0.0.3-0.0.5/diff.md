# Comparing `tmp/lobsang-0.0.3.tar.gz` & `tmp/lobsang-0.0.5.tar.gz`

## Comparing `lobsang-0.0.3.tar` & `lobsang-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 lobsang-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 lobsang-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 lobsang-0.0.3/examples/.env
--rw-r--r--   0        0        0    34218 2020-02-02 00:00:00.000000 lobsang-0.0.3/examples/1_basics.ipynb
--rw-r--r--   0        0        0    18604 2020-02-02 00:00:00.000000 lobsang-0.0.3/examples/2_directives.ipynb
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/__init__.py
--rw-r--r--   0        0        0    16192 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/chat.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/messages.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/directives/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/directives/base.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/directives/json.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/directives/text.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/llms/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/llms/base.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/llms/fake.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 lobsang-0.0.3/lobsang/llms/openai.py
--rw-r--r--   0        0        0    18287 2020-02-02 00:00:00.000000 lobsang-0.0.3/tests/test_chat.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 lobsang-0.0.3/tests/test_directives.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 lobsang-0.0.3/tests/test_llms.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 lobsang-0.0.3/tests/test_messages.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 lobsang-0.0.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 lobsang-0.0.3/LICENSE
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 lobsang-0.0.3/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 lobsang-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 lobsang-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 lobsang-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 lobsang-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 lobsang-0.0.5/examples/.env
+-rw-r--r--   0        0        0    34218 2020-02-02 00:00:00.000000 lobsang-0.0.5/examples/1_basics.ipynb
+-rw-r--r--   0        0        0    18604 2020-02-02 00:00:00.000000 lobsang-0.0.5/examples/2_directives.ipynb
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 lobsang-0.0.5/lobsang/__init__.py
+-rw-r--r--   0        0        0    16192 2020-02-02 00:00:00.000000 lobsang-0.0.5/lobsang/chat.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 lobsang-0.0.5/lobsang/messages.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 lobsang-0.0.5/lobsang/directives/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 lobsang-0.0.5/lobsang/directives/base.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 lobsang-0.0.5/lobsang/directives/json.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 lobsang-0.0.5/lobsang/directives/text.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 lobsang-0.0.5/lobsang/llms/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 lobsang-0.0.5/lobsang/llms/base.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 lobsang-0.0.5/lobsang/llms/fake.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 lobsang-0.0.5/lobsang/llms/openai.py
+-rw-r--r--   0        0        0    18287 2020-02-02 00:00:00.000000 lobsang-0.0.5/tests/test_chat.py
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 lobsang-0.0.5/tests/test_directives.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 lobsang-0.0.5/tests/test_llms.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 lobsang-0.0.5/tests/test_messages.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 lobsang-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 lobsang-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 lobsang-0.0.5/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lobsang-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 lobsang-0.0.5/PKG-INFO
```

### Comparing `lobsang-0.0.3/CHANGELOG.md` & `lobsang-0.0.5/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
-and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+and this project adh
+## [0.0.5] 2023-08-07
+
+### Fixed
+- Fix version specifier in pyproject.toml
+
+## [0.0.4] 2023-08-07
+
+### Changed
+- Switched from 'ast.literal_eval' to 'json.loads' in JSONDirective
+
+### Removed
+- Remove trailing newline from JOSONDirective.instructions
 
 ## [0.0.3] 2023-08-06
 
 ### Added
 
 - Add abstract `instructions` property to abstract base class `Directive`
 - Add _info method to easily create info dict for directive
```

### Comparing `lobsang-0.0.3/.github/workflows/python-publish.yml` & `lobsang-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/examples/1_basics.ipynb` & `lobsang-0.0.5/examples/1_basics.ipynb`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/examples/2_directives.ipynb` & `lobsang-0.0.5/examples/2_directives.ipynb`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/lobsang/__init__.py` & `lobsang-0.0.5/lobsang/__init__.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/lobsang/chat.py` & `lobsang-0.0.5/lobsang/chat.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/lobsang/messages.py` & `lobsang-0.0.5/lobsang/messages.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/lobsang/directives/__init__.py` & `lobsang-0.0.5/lobsang/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/lobsang/directives/base.py` & `lobsang-0.0.5/lobsang/directives/base.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/lobsang/directives/json.py` & `lobsang-0.0.5/lobsang/directives/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     """
     instructions = """\
     {message}
     
     Create a JSON object with the following schema:
     ```json
     {schema}
-    ```
-    """
+    ```"""
 
     def __init__(self, schema: dict, prune=True, instructions: str = None):
         """
         Initializes the JSONDirective with the provided schema.
 
         **Note:** Replacing the original response helps to keep a clean chat history, hinting that
          i.e. any
@@ -85,17 +84,17 @@
         # Stop early if no JSON block was found
         if not json_block:
             return res, info | {"error": "No JSON block found.", **kwargs}
 
         # Try to parse JSON block
         try:
             # We use ast instead of json because ast is less strict (e.g. allows single quotes)
-            json_object = ast.literal_eval(json_block)
-        except SyntaxError as e:
-            return res, info | {"error": f"Not valid JSON. Syntax Error: {e}", **kwargs}
+            json_object = json.loads(json_block)
+        except json.JSONDecodeError as e:
+            return res, info | {"error": f"Not valid JSON. Decode Error: {e}", **kwargs}
 
         # Validate JSON object
         try:
             validate(json_object, schema=self.schema)
         except jsonschema.exceptions.ValidationError as e:
             return res, info | {"error": f"Does not match schema. Schema Error: {e}", **kwargs}
```

### Comparing `lobsang-0.0.3/lobsang/directives/text.py` & `lobsang-0.0.5/lobsang/directives/text.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/lobsang/llms/base.py` & `lobsang-0.0.5/lobsang/llms/base.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/lobsang/llms/fake.py` & `lobsang-0.0.5/lobsang/llms/fake.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/lobsang/llms/openai.py` & `lobsang-0.0.5/lobsang/llms/openai.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/tests/test_chat.py` & `lobsang-0.0.5/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/tests/test_directives.py` & `lobsang-0.0.5/tests/test_directives.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,16 +103,15 @@
         'test2': "Hello, world"
     }
     ```
     This is some text after the JSON block.
     """
     parsed, info = json_directive.parse(response)
     assert parsed == response
-    assert info['error'] == ('Not valid JSON. Syntax Error: invalid syntax. Perhaps you forgot a comma? '
-                             '(<unknown>, line 2)')
+    assert info['error'] == "Not valid JSON. Decode Error: Expecting ',' delimiter: line 3 column 9 (char 30)"
 
     # Does not adhere to schema
     response = """
     This is some text around the JSON block.
     ```json
     {
         "test": 123
```

### Comparing `lobsang-0.0.3/tests/test_messages.py` & `lobsang-0.0.5/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/LICENSE` & `lobsang-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lobsang-0.0.3/README.md` & `lobsang-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -37,22 +37,22 @@
     # Call the chat with one message
     chat("Hello!")
     chat("How are you?")
     print("Chat history:")  
     print(chat)
     
     # Call the chat with multiple messages
-    res = chat("What is 1+1?", "What is 2+2?")
+    res = chat.run(["What is 1+1?", "What is 2+2?"])
     print("Chat Snippet:")
     print(res)
     print("Full chat history:")
     print(chat)
     ```
   - **Directives**: Directives are used to guide the LLM to generate a specific response by embedding instructions
       in a corresponding message. For example, you can use the JSON directive to instruct the LLM to generate a JSON
-      response (see [examples/utilize_directives.py](./examples/utilize_directives.py) for more details).
+      response (see [examples/2_directives.ipynb](./examples/2_directives.ipynb) for more details).
 
 ## Examples
 We provide a few examples to get you started. You can find them in the [examples](./examples) folder.
 The examples use the openai package, make sure to install it before running the examples (`pip install openai`).
 You will also need an OpenAI API key, which you can get here: https://platform.openai.com/account/api-keys.
```

### Comparing `lobsang-0.0.3/pyproject.toml` & `lobsang-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name="lobsang"
 description="A simple framework to interact with conversational LLMs"
 keywords =['llm', 'chat', 'framework']
-version="0.0.3"
+version="0.0.5"
 authors = []
 readme="README.md"
 requires-python=">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = []
+dependencies = [
+    "openai >= 0.27.8, < 1",
+    "jsonschema >=4.18.6, < 5",
+]
 
 [project.optional-dependencies]
 dev = ["black==23.3.0", "pylint==2.8.2"]
 
 [project.urls]
 "Homepage" = "https://github.com/cereisen/lobsang"
```

### Comparing `lobsang-0.0.3/PKG-INFO` & `lobsang-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: lobsang
-Version: 0.0.3
+Version: 0.0.5
 Summary: A simple framework to interact with conversational LLMs
 Project-URL: Homepage, https://github.com/cereisen/lobsang
 License-File: LICENSE
 Keywords: chat,framework,llm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
+Requires-Dist: jsonschema<5,>=4.18.6
+Requires-Dist: openai<1,>=0.27.8
 Provides-Extra: dev
 Requires-Dist: black==23.3.0; extra == 'dev'
 Requires-Dist: pylint==2.8.2; extra == 'dev'
 Description-Content-Type: text/markdown
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/lobsang)
 ![GitHub](https://img.shields.io/github/license/cereisen/lobsang)
@@ -53,22 +55,22 @@
     # Call the chat with one message
     chat("Hello!")
     chat("How are you?")
     print("Chat history:")  
     print(chat)
     
     # Call the chat with multiple messages
-    res = chat("What is 1+1?", "What is 2+2?")
+    res = chat.run(["What is 1+1?", "What is 2+2?"])
     print("Chat Snippet:")
     print(res)
     print("Full chat history:")
     print(chat)
     ```
   - **Directives**: Directives are used to guide the LLM to generate a specific response by embedding instructions
       in a corresponding message. For example, you can use the JSON directive to instruct the LLM to generate a JSON
-      response (see [examples/utilize_directives.py](./examples/utilize_directives.py) for more details).
+      response (see [examples/2_directives.ipynb](./examples/2_directives.ipynb) for more details).
 
 ## Examples
 We provide a few examples to get you started. You can find them in the [examples](./examples) folder.
 The examples use the openai package, make sure to install it before running the examples (`pip install openai`).
 You will also need an OpenAI API key, which you can get here: https://platform.openai.com/account/api-keys.
```

