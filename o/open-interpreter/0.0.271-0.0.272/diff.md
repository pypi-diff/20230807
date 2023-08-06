# Comparing `tmp/open_interpreter-0.0.271.tar.gz` & `tmp/open_interpreter-0.0.272.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.271.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.272.tar", max compression
```

## Comparing `open_interpreter-0.0.271.tar` & `open_interpreter-0.0.272.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.271/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.271/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.271/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.271/interpreter/cli.py
--rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.271/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.271/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13559 2023-08-06 20:58:45.519021 open_interpreter-0.0.271/interpreter/interpreter.py
--rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.271/interpreter/llama_2.py
--rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.271/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.271/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.271/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-06 21:28:19.437777 open_interpreter-0.0.271/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.271/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.272/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.272/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.272/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.272/interpreter/cli.py
+-rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.272/interpreter/code_block.py
+-rw-r--r--   0        0        0     7495 2023-08-06 21:49:50.770126 open_interpreter-0.0.272/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13570 2023-08-06 21:52:01.375917 open_interpreter-0.0.272/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.272/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.272/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.272/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.272/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-06 21:53:41.426481 open_interpreter-0.0.272/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.272/PKG-INFO
```

### Comparing `open_interpreter-0.0.271/LICENSE` & `open_interpreter-0.0.272/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.271/README.md` & `open_interpreter-0.0.272/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.271/interpreter/__init__.py` & `open_interpreter-0.0.272/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.271/interpreter/cli.py` & `open_interpreter-0.0.272/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.271/interpreter/code_block.py` & `open_interpreter-0.0.272/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.271/interpreter/code_interpreter.py` & `open_interpreter-0.0.272/interpreter/code_interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,16 @@
       # Check if it's a message we added (like ACTIVE_LINE)
       # Or if we should save it to self.output
       if line.startswith("ACTIVE_LINE:"):
         self.active_line = int(line.split(":")[1])
       elif line == "END_OF_EXECUTION":
         self.done.set()
         self.active_line = None
+      elif "KeyboardInterrupt" in line:
+        raise KeyboardInterrupt
       else:
         self.output += "\n" + line
         self.output = self.output.strip()
 
       # Strip then truncate the output if necessary
       self.output = truncate_output(self.output)
```

### Comparing `open_interpreter-0.0.271/interpreter/interpreter.py` & `open_interpreter-0.0.272/interpreter/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
               self.messages[-1]["function_call"][
                 "parsed_arguments"] = new_parsed_arguments
 
         elif self.local:
           # Llama-2
           # Get contents of current code block and save to parsed_arguments, under function_call
           if "content" in self.messages[-1]:
-            current_code_block = self.messages[-1]["content"].split("```")[-1]
+            current_code_block = self.messages[-1]["content"].split("```python")[-1]
             arguments = {"language": "python", "code": current_code_block}
             
             # Llama-2 won't make a "function_call" property for us to store this under, so:
             if "function_call" not in self.messages[-1]:
               self.messages[-1]["function_call"] = {}
               
             self.messages[-1]["function_call"]["parsed_arguments"] = arguments
@@ -374,15 +374,15 @@
           # Create or retrieve a Code Interpreter for this language
           language = self.messages[-1]["function_call"]["parsed_arguments"][
             "language"]
           if language not in self.code_interpreters:
             self.code_interpreters[language] = CodeInterpreter(language)
           code_interpreter = self.code_interpreters[language]
 
-          # Let Code Interpreter control the active_block
+          # Let this Code Interpreter control the active_block
           code_interpreter.active_block = self.active_block
           code_interpreter.run()
 
           # End the active_block
           self.active_block.end()
 
           # Append the output to messages
```

### Comparing `open_interpreter-0.0.271/interpreter/llama_2.py` & `open_interpreter-0.0.272/interpreter/llama_2.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.271/interpreter/message_block.py` & `open_interpreter-0.0.272/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.271/interpreter/system_message.txt` & `open_interpreter-0.0.272/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.271/interpreter/utils.py` & `open_interpreter-0.0.272/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.271/pyproject.toml` & `open_interpreter-0.0.272/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.271"
+version = "0.0.272"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.271/PKG-INFO` & `open_interpreter-0.0.272/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.271
+Version: 0.0.272
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

