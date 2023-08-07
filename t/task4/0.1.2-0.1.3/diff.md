# Comparing `tmp/task4-0.1.2.tar.gz` & `tmp/task4-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task4-0.1.2.tar", max compression
+gzip compressed data, was "task4-0.1.3.tar", max compression
```

## Comparing `task4-0.1.2.tar` & `task4-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task4-0.1.2/LICENSE
--rw-r--r--   0        0        0      259 2023-08-04 21:17:25.582564 task4-0.1.2/log_parser/__init__.py
--rw-r--r--   0        0        0      117 2023-08-04 21:17:25.586547 task4-0.1.2/log_parser/__main__.py
--rw-r--r--   0        0        0       23 2023-08-07 13:17:09.089703 task4-0.1.2/log_parser/__version__.py
--rw-r--r--   0        0        0      151 2023-08-04 21:17:25.566551 task4-0.1.2/log_parser/cli/__init__.py
--rw-r--r--   0        0        0      117 2023-08-04 21:17:25.571572 task4-0.1.2/log_parser/cli/__main__.py
--rw-r--r--   0        0        0    12491 2023-08-07 12:48:30.719050 task4-0.1.2/log_parser/cli/cli.py
--rw-r--r--   0        0        0     7817 2023-08-04 19:51:24.232095 task4-0.1.2/log_parser/cli/patterns.py
--rw-r--r--   0        0        0    15604 2023-08-07 02:18:32.532814 task4-0.1.2/log_parser/log_parser.py
--rw-r--r--   0        0        0       98 2023-08-07 10:54:47.910859 task4-0.1.2/log_parser/showcase/__init__.py
--rw-r--r--   0        0        0      139 2023-08-07 10:54:47.915859 task4-0.1.2/log_parser/showcase/__main__.py
--rw-r--r--   0        0        0 36936434 2017-07-27 13:29:20.000000 task4-0.1.2/log_parser/showcase/access.log
--rw-r--r--   0        0        0    27128 2023-08-07 12:19:50.128825 task4-0.1.2/log_parser/showcase/showcase.py
--rw-r--r--   0        0        0      518 2023-08-07 13:17:09.085705 task4-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    26052 2023-07-26 00:57:10.559780 task4-0.1.2/README.md
--rw-r--r--   0        0        0    26197 1970-01-01 00:00:00.000000 task4-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task4-0.1.3/LICENSE
+-rw-r--r--   0        0        0      259 2023-08-04 21:17:25.582564 task4-0.1.3/log_parser/__init__.py
+-rw-r--r--   0        0        0      117 2023-08-04 21:17:25.586547 task4-0.1.3/log_parser/__main__.py
+-rw-r--r--   0        0        0       23 2023-08-07 13:45:20.243648 task4-0.1.3/log_parser/__version__.py
+-rw-r--r--   0        0        0      151 2023-08-04 21:17:25.566551 task4-0.1.3/log_parser/cli/__init__.py
+-rw-r--r--   0        0        0      117 2023-08-04 21:17:25.571572 task4-0.1.3/log_parser/cli/__main__.py
+-rw-r--r--   0        0        0    12491 2023-08-07 12:48:30.719050 task4-0.1.3/log_parser/cli/cli.py
+-rw-r--r--   0        0        0     7817 2023-08-04 19:51:24.232095 task4-0.1.3/log_parser/cli/patterns.py
+-rw-r--r--   0        0        0    15604 2023-08-07 02:18:32.532814 task4-0.1.3/log_parser/log_parser.py
+-rw-r--r--   0        0        0       98 2023-08-07 10:54:47.910859 task4-0.1.3/log_parser/showcase/__init__.py
+-rw-r--r--   0        0        0      139 2023-08-07 10:54:47.915859 task4-0.1.3/log_parser/showcase/__main__.py
+-rw-r--r--   0        0        0 36936434 2017-07-27 13:29:20.000000 task4-0.1.3/log_parser/showcase/access.log
+-rw-r--r--   0        0        0    23944 2023-08-07 13:43:41.071387 task4-0.1.3/log_parser/showcase/showcase.py
+-rw-r--r--   0        0        0      518 2023-08-07 13:45:20.238692 task4-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    26052 2023-07-26 00:57:10.559780 task4-0.1.3/README.md
+-rw-r--r--   0        0        0    26197 1970-01-01 00:00:00.000000 task4-0.1.3/PKG-INFO
```

### Comparing `task4-0.1.2/log_parser/cli/cli.py` & `task4-0.1.3/log_parser/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task4-0.1.2/log_parser/cli/patterns.py` & `task4-0.1.3/log_parser/cli/patterns.py`

 * *Files identical despite different names*

### Comparing `task4-0.1.2/log_parser/log_parser.py` & `task4-0.1.3/log_parser/log_parser.py`

 * *Files identical despite different names*

### Comparing `task4-0.1.2/log_parser/showcase/access.log` & `task4-0.1.3/log_parser/showcase/access.log`

 * *Files identical despite different names*

### Comparing `task4-0.1.2/log_parser/showcase/showcase.py` & `task4-0.1.3/log_parser/showcase/showcase.py`

 * *Files 7% similar despite different names*

```diff
@@ -176,37 +176,34 @@
 
 # Determine the platform
 current_platform = platform.system()
 
 # Set the Python command based on the platform
 if current_platform == 'Windows':
     python_command = 'python -m'
+    quoting = r'""'
 else:
     python_command = 'python3 -m'
+    quoting = r'\"'
 
 select_style = questionary.Style([
     #     ('default', "bg:#ffffff fg:#000000"),
     # ('selected', 'bg:#336699 fg:#ffffff'),
     ('highlighted', '#008888'),
     ('pointer', '#008888'),
     # ('question', 'fg:#009b06'),
     ('qmark', 'fg:#009b06'),
     ('instruction', "#008888"),
     ('answer', "#009b06"),
 ])
 
-# extractor = r'IP4\ \((?P<IP4_LIST>(?:(?:IP4|.*?),\ )*(?:IP4|.*?))\)' \
-#             r'\ -\ -\ \[DATE_TIME_SEC\]\ \"(?:REQUEST|-)\"\ (?P<STATUS>\d{3})' \
-#             r'\ (?P<BYTES>\d+|-)\ (?P<MINUTES>\d+|-)\ (?P<SECONDS>\d+|-)\ \"(?:URL|-|.*?)\"' \
-#             r'\ \"(?:USER_AGENT|-|.*?)\"\ \"(?:URI|-)\"'
-
-extractor = r'IP4\ \((?P<IP4_LIST>(?:(?:IP4|.*?),\ )*(?:IP4|.*?))\)' \
-            r'\ -\ -\ \[DATE_TIME_SEC\]\ ""(?:REQUEST|-)""\ (?P<STATUS>\d{3})' \
-            r'\ (?P<BYTES>\d+|-)\ (?P<MINUTES>\d+|-)\ (?P<SECONDS>\d+|-)\ ""(?:URL|-|.*?)""' \
-            r'\ ""(?:USER_AGENT|-|.*?)""\ ""(?:URI|-)""'
+extractor = fr'IP4\ \((?P<IP4_LIST>(?:(?:IP4|.*?),\ )*(?:IP4|.*?))\)' \
+            fr'\ -\ -\ \[DATE_TIME_SEC\]\ {quoting}(?:REQUEST|-){quoting}\ (?P<STATUS>\d{{3}})' \
+            fr'\ (?P<BYTES>\d+|-)\ (?P<MINUTES>\d+|-)\ (?P<SECONDS>\d+|-)\ {quoting}(?:URL|-|.*?){quoting}' \
+            fr'\ {quoting}(?:USER_AGENT|-|.*?){quoting}\ {quoting}(?:URI|-){quoting}'
 
 OPTIONS_ARGUMENTS = {
     'r': {
         'descr': 'r',
         'type': 'text',
         'message': 'Provide row range (row1 row2 ... rowN) (row1-rowN) (from the beginning: -row) (to the end: row-)',
         'default': '1-',
@@ -341,85 +338,14 @@
         'descr': 'file',
         'type': 'path',
         'message': 'Which log file would you like to parse?',
         'validation': lambda val: True if val else 'Please, provide a path to a file',
         'default': f'{os.path.dirname(os.path.abspath(__file__))}/access.log',
         'filter': lambda val: f'"{val}"' if val else val,
     },
-    # 're': {
-    #     'descr': 're',
-    #     'type': 'select',
-    #     'name': 'regex',
-    #     'message': 'Which regular expression would you like to choose?',
-    #     'choices': [Choice(title=val.name, value=val.name) for val in RegexPatterns],
-    #     'instruction': '(Use arrow keys to navigate through the menu)',
-    #     'pointer': '>',
-    #     'filter': lambda val: val if val else 'IP4',
-    #     'use_shortcuts': True,
-    # },
-    # 'j': {
-    #     'descr': 'j',
-    #     'type': 'confirm',
-    #     'message': 'Would you like to output in JSON format?',
-    #     'default': False,
-    #     'filter': lambda val: '-j' if val else '',
-    # },
-    # 'j_true': {
-    #     'descr': 'j_true',
-    #     'type': 'confirm',
-    #     'message': 'Would you like to output in JSON format?',
-    #     'default': True,
-    #     'filter': lambda val: '-j' if val else '',
-    # },
-    # 'n': {
-    #     'descr': 'n',
-    #     'type': 'confirm',
-    #     'message': 'Does not the parsed file contain a header on the first line?',
-    #     'default': False,
-    #     'filter': lambda val: '--no-header' if val else '',
-    # },
-    # 'n_true': {
-    #     'descr': 'n_true',
-    #     'type': 'confirm',
-    #     'message': 'Does not the parsed file contain a header on the first line?',
-    #     'default': True,
-    #     'filter': lambda val: '--no-header' if val else '',
-    # },
-    # 'f_tsv': {
-    #     'descr': 'f_tsv',
-    #     'type': 'path',
-    #     'message': 'Which file would you like to use?',
-    #     'validation': lambda val: True if val else 'Please, provide a path to a file',
-    #     'default': f'{os.path.dirname(os.path.abspath(__file__))}/sample.tsv',
-    #     'filter': lambda val: f'"{val}"' if val else val,
-    # },
-    # 'f_out': {
-    #     'descr': 'f_out',
-    #     'type': 'path',
-    #     'message': 'In which file would you like to write generated passwords (it may be new)?',
-    #     'validation': lambda val: True if val else 'Please specify the path to the file',
-    #     'default': './sample_output.csv',
-    #     'filter': lambda val: f'"{val}"' if val else val,
-    # },
-    # 'f_log': {
-    #     'descr': 'f_log',
-    #     'type': 'path',
-    #     'message': 'In which file would you like to write log messages (it may be new)?',
-    #     'validation': lambda val: True if val else 'Please specify the path to the file',
-    #     'default': './parse_xsv.log',
-    #     'filter': lambda val: f'"{val}"' if val else val,
-    # },
-    # 'f_err': {
-    #     'descr': 'f_err',
-    #     'type': 'path',
-    #     'message': 'Which file would you like to use?',
-    #     'validation': lambda val: True if val else 'Please, provide a path to a file',
-    #     'default': f'{os.path.dirname(os.path.abspath(__file__))}/corrupted_sample.csv',
-    #     'filter': lambda val: f'"{val}"' if val else val,
-    # },
     'v': {
         'descr': 'v',
         'type': 'text',
         'message': 'What logging level would you like to set?',
         'default': '2',
         'validation': lambda val: True if val.isdigit() else 'Please, provide a number',
         'filter': lambda val: f'{"-" if int(val) > 0 else ""}{"v" * (int(val) if int(val) <= 4 else 4)}',
```

### Comparing `task4-0.1.2/pyproject.toml` & `task4-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "task4"
-version = "0.1.2"
+version = "0.1.3"
 description = "Log file parser CLI and library"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "log_parser"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `task4-0.1.2/README.md` & `task4-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `task4-0.1.2/PKG-INFO` & `task4-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task4
-Version: 0.1.2
+Version: 0.1.3
 Summary: Log file parser CLI and library
 License: MIT
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: task4 Version: 0.1.2 Summary: Log file parser CLI
+Metadata-Version: 2.1 Name: task4 Version: 0.1.3 Summary: Log file parser CLI
 and library License: MIT Author: Bill.Avramenko Author-email:
 billavramenko@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: questionary
 (>=1.10.0,<2.0.0) Description-Content-Type: text/markdown
```

