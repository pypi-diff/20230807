# Comparing `tmp/open_interpreter-0.0.277.tar.gz` & `tmp/open_interpreter-0.0.278.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.277.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.278.tar", max compression
```

## Comparing `open_interpreter-0.0.277.tar` & `open_interpreter-0.0.278.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.277/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.277/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.277/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.277/interpreter/cli.py
--rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.277/interpreter/code_block.py
--rw-r--r--   0        0        0     8132 2023-08-07 02:36:30.664804 open_interpreter-0.0.277/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13860 2023-08-07 17:21:10.873094 open_interpreter-0.0.277/interpreter/interpreter.py
--rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.277/interpreter/llama_2.py
--rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.277/interpreter/message_block.py
--rw-r--r--   0        0        0     1915 2023-08-07 17:40:06.855841 open_interpreter-0.0.277/interpreter/system_message.txt
--rw-r--r--   0        0        0     3535 2023-08-06 21:56:51.302530 open_interpreter-0.0.277/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-07 17:40:32.961742 open_interpreter-0.0.277/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.277/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.278/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.278/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.278/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.278/interpreter/cli.py
+-rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.278/interpreter/code_block.py
+-rw-r--r--   0        0        0     8410 2023-08-07 19:48:01.908489 open_interpreter-0.0.278/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13860 2023-08-07 17:21:10.873094 open_interpreter-0.0.278/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.278/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.278/interpreter/message_block.py
+-rw-r--r--   0        0        0     1915 2023-08-07 17:40:06.855841 open_interpreter-0.0.278/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3535 2023-08-06 21:56:51.302530 open_interpreter-0.0.278/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-07 21:19:31.840224 open_interpreter-0.0.278/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.278/PKG-INFO
```

### Comparing `open_interpreter-0.0.277/LICENSE` & `open_interpreter-0.0.278/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.277/README.md` & `open_interpreter-0.0.278/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.277/interpreter/__init__.py` & `open_interpreter-0.0.278/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.277/interpreter/cli.py` & `open_interpreter-0.0.278/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.277/interpreter/code_block.py` & `open_interpreter-0.0.278/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.277/interpreter/code_interpreter.py` & `open_interpreter-0.0.278/interpreter/code_interpreter.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,27 +161,36 @@
     indicating the active line number during execution. The print statements respect
     the indentation of the original code, using the indentation of the next non-blank line.
 
     Note: This doesn't work on shell if:
     1) Any line starts with whitespace and
     2) Sometimes, doesn't even work for regular loops with newlines between lines
     We return in those cases.
+
+    In python it doesn't work if:
+    1) Try/Except clause
+    2) Triple quote multiline strings
     """
 
     # Split the original code into lines
     code_lines = code.strip().split('\n')
 
     # If it's shell, check for breaking cases
     if self.language == "shell":
       if "for" in code or "do" in code or "done" in code:
         return code
       for line in code_lines:
         if line.startswith(" "):
           return code
 
+    # If it's Python, check for breaking cases
+    if self.language == "python":
+      if "try" in code or "except" in code or "'''" in code or "'''" in code:
+        return code
+
     # Initialize an empty list to hold the modified lines of code
     modified_code_lines = []
 
     # Iterate over each line in the original code
     for i, line in enumerate(code_lines):
       # Initialize a variable to hold the leading whitespace of the next non-empty line
       leading_whitespace = ""
```

### Comparing `open_interpreter-0.0.277/interpreter/interpreter.py` & `open_interpreter-0.0.278/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.277/interpreter/llama_2.py` & `open_interpreter-0.0.278/interpreter/llama_2.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.277/interpreter/message_block.py` & `open_interpreter-0.0.278/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.277/interpreter/system_message.txt` & `open_interpreter-0.0.278/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.277/interpreter/utils.py` & `open_interpreter-0.0.278/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.277/pyproject.toml` & `open_interpreter-0.0.278/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.277"
+version = "0.0.278"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.277/PKG-INFO` & `open_interpreter-0.0.278/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.277
+Version: 0.0.278
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

