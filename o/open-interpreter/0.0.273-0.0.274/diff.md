# Comparing `tmp/open_interpreter-0.0.273.tar.gz` & `tmp/open_interpreter-0.0.274.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.273.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.274.tar", max compression
```

## Comparing `open_interpreter-0.0.273.tar` & `open_interpreter-0.0.274.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.273/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.273/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.273/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.273/interpreter/cli.py
--rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.273/interpreter/code_block.py
--rw-r--r--   0        0        0     7495 2023-08-06 21:49:50.770126 open_interpreter-0.0.273/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13800 2023-08-06 22:01:09.577801 open_interpreter-0.0.273/interpreter/interpreter.py
--rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.273/interpreter/llama_2.py
--rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.273/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.273/interpreter/system_message.txt
--rw-r--r--   0        0        0     3535 2023-08-06 21:56:51.302530 open_interpreter-0.0.273/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-06 22:02:05.643720 open_interpreter-0.0.273/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.273/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.274/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.274/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.274/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.274/interpreter/cli.py
+-rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.274/interpreter/code_block.py
+-rw-r--r--   0        0        0     7927 2023-08-07 01:02:09.806356 open_interpreter-0.0.274/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13800 2023-08-06 22:01:09.577801 open_interpreter-0.0.274/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.274/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.274/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.274/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3535 2023-08-06 21:56:51.302530 open_interpreter-0.0.274/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-07 01:04:22.177484 open_interpreter-0.0.274/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.274/PKG-INFO
```

### Comparing `open_interpreter-0.0.273/LICENSE` & `open_interpreter-0.0.274/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.273/README.md` & `open_interpreter-0.0.274/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.273/interpreter/__init__.py` & `open_interpreter-0.0.274/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.273/interpreter/cli.py` & `open_interpreter-0.0.274/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.273/interpreter/code_block.py` & `open_interpreter-0.0.274/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.273/interpreter/code_interpreter.py` & `open_interpreter-0.0.274/interpreter/code_interpreter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import subprocess
 import threading
+import traceback
 import time
 import ast
 import astor
 import sys
 import os
 
 # Mapping of languages to their start and print commands
@@ -94,15 +95,35 @@
 
     # Add print commands that tell us what the active line is
     code = self.add_active_line_prints(code)
 
     # If it's Python, we also need to normalize
     # and fix indentation (so it works with `python -i`)
     if self.language == "python":
-      code = normalize(code)
+
+      # Normalize code by parsing then unparsing it
+      try:
+        parsed_ast = ast.parse(code)
+        code = astor.to_source(parsed_ast)
+      except:
+        # If this failed, it means the code didn't compile
+        # This traceback will be our output.
+        
+        traceback_string = traceback.format_exc()
+        self.output = traceback_string
+
+        # Strip then truncate the output if necessary
+        self.output = truncate_output(self.output)
+
+        # Display it
+        self.active_block.output = self.output
+        self.active_block.refresh()
+
+        return self.output
+        
       code = fix_code_indentation(code)
 
     # Add end command (we'll be listening for this so we know when it ends)
     code += "\n\n" + self.print_cmd.format('END_OF_EXECUTION') + "\n"
     """
     # Debug
     print("Running code:")
@@ -199,23 +220,14 @@
       self.output = truncate_output(self.output)
 
       # Update the active block
       self.active_block.active_line = self.active_line
       self.active_block.output = self.output
       self.active_block.refresh()
 
-
-def normalize(code):
-  # Parse the code into an AST
-  parsed_ast = ast.parse(code)
-
-  # Convert the AST back to source code
-  return astor.to_source(parsed_ast)
-
-
 def fix_code_indentation(code):
   lines = code.split("\n")
   fixed_lines = []
   was_indented = False
   for line in lines:
     current_indent = len(line) - len(line.lstrip())
     if current_indent == 0 and was_indented:
```

### Comparing `open_interpreter-0.0.273/interpreter/interpreter.py` & `open_interpreter-0.0.274/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.273/interpreter/llama_2.py` & `open_interpreter-0.0.274/interpreter/llama_2.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.273/interpreter/message_block.py` & `open_interpreter-0.0.274/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.273/interpreter/system_message.txt` & `open_interpreter-0.0.274/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.273/interpreter/utils.py` & `open_interpreter-0.0.274/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.273/pyproject.toml` & `open_interpreter-0.0.274/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.273"
+version = "0.0.274"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.273/PKG-INFO` & `open_interpreter-0.0.274/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.273
+Version: 0.0.274
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

