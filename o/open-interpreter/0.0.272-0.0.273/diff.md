# Comparing `tmp/open_interpreter-0.0.272.tar.gz` & `tmp/open_interpreter-0.0.273.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.272.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.273.tar", max compression
```

## Comparing `open_interpreter-0.0.272.tar` & `open_interpreter-0.0.273.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.272/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.272/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.272/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.272/interpreter/cli.py
--rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.272/interpreter/code_block.py
--rw-r--r--   0        0        0     7495 2023-08-06 21:49:50.770126 open_interpreter-0.0.272/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13570 2023-08-06 21:52:01.375917 open_interpreter-0.0.272/interpreter/interpreter.py
--rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.272/interpreter/llama_2.py
--rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.272/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.272/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.272/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-06 21:53:41.426481 open_interpreter-0.0.272/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.272/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.273/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.273/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.273/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.273/interpreter/cli.py
+-rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.273/interpreter/code_block.py
+-rw-r--r--   0        0        0     7495 2023-08-06 21:49:50.770126 open_interpreter-0.0.273/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13800 2023-08-06 22:01:09.577801 open_interpreter-0.0.273/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.273/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.273/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.273/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3535 2023-08-06 21:56:51.302530 open_interpreter-0.0.273/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-06 22:02:05.643720 open_interpreter-0.0.273/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.273/PKG-INFO
```

### Comparing `open_interpreter-0.0.272/LICENSE` & `open_interpreter-0.0.273/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.272/README.md` & `open_interpreter-0.0.273/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.272/interpreter/__init__.py` & `open_interpreter-0.0.273/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.272/interpreter/cli.py` & `open_interpreter-0.0.273/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.272/interpreter/code_block.py` & `open_interpreter-0.0.273/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.272/interpreter/code_interpreter.py` & `open_interpreter-0.0.273/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.272/interpreter/interpreter.py` & `open_interpreter-0.0.273/interpreter/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,16 +225,23 @@
         messages=tt.trim(self.messages, model, system_message=system_message),
         functions=[function_schema],
         stream=True,
         temperature=self.temperature,
       )
     elif self.local:
       # Llama-2
+      
+      # Turn function messages -> system messages for llama compatability
+      messages = self.messages
+      for message in messages:
+        if message['role'] == 'function':
+            message['role'] = 'system'
+          
       response = self.llama_instance.create_chat_completion(
-        messages=tt.trim(self.messages,
+        messages=tt.trim(messages,
                          "gpt-3.5-turbo",
                          system_message=system_message),
         stream=True,
         temperature=self.temperature,
       )
 
     # Initialize message, function call trackers, and active block
```

### Comparing `open_interpreter-0.0.272/interpreter/llama_2.py` & `open_interpreter-0.0.273/interpreter/llama_2.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.272/interpreter/message_block.py` & `open_interpreter-0.0.273/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.272/interpreter/system_message.txt` & `open_interpreter-0.0.273/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.272/interpreter/utils.py` & `open_interpreter-0.0.273/interpreter/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import json
 
 def merge_deltas(original, delta):
+    """
+    Pushes the delta into the original and returns that.
+
+    Great for reconstructing OpenAI streaming responses -> complete message objects.
+    """
     for key, value in delta.items():
         if isinstance(value, dict):
             if key not in original:
                 original[key] = value
             else:
                 merge_deltas(original[key], value)
         else:
```

### Comparing `open_interpreter-0.0.272/pyproject.toml` & `open_interpreter-0.0.273/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.272"
+version = "0.0.273"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.272/PKG-INFO` & `open_interpreter-0.0.273/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.272
+Version: 0.0.273
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

