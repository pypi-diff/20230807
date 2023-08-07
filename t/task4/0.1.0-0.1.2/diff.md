# Comparing `tmp/task4-0.1.0.tar.gz` & `tmp/task4-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task4-0.1.0.tar", max compression
+gzip compressed data, was "task4-0.1.2.tar", max compression
```

## Comparing `task4-0.1.0.tar` & `task4-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task4-0.1.0/LICENSE
--rw-r--r--   0        0        0      259 2023-08-04 21:17:25.582564 task4-0.1.0/log_parser/__init__.py
--rw-r--r--   0        0        0      117 2023-08-04 21:17:25.586547 task4-0.1.0/log_parser/__main__.py
--rw-r--r--   0        0        0       23 2023-07-26 00:59:21.000035 task4-0.1.0/log_parser/__version__.py
--rw-r--r--   0        0        0      151 2023-08-04 21:17:25.566551 task4-0.1.0/log_parser/cli/__init__.py
--rw-r--r--   0        0        0      117 2023-08-04 21:17:25.571572 task4-0.1.0/log_parser/cli/__main__.py
--rw-r--r--   0        0        0    12491 2023-08-07 12:48:30.719050 task4-0.1.0/log_parser/cli/cli.py
--rw-r--r--   0        0        0     7817 2023-08-04 19:51:24.232095 task4-0.1.0/log_parser/cli/patterns.py
--rw-r--r--   0        0        0    15604 2023-08-07 02:18:32.532814 task4-0.1.0/log_parser/log_parser.py
--rw-r--r--   0        0        0       98 2023-08-07 10:54:47.910859 task4-0.1.0/log_parser/showcase/__init__.py
--rw-r--r--   0        0        0      139 2023-08-07 10:54:47.915859 task4-0.1.0/log_parser/showcase/__main__.py
--rw-r--r--   0        0        0 36936434 2017-07-27 13:29:20.000000 task4-0.1.0/log_parser/showcase/access.log
--rw-r--r--   0        0        0    27128 2023-08-07 12:19:50.128825 task4-0.1.0/log_parser/showcase/showcase.py
--rw-r--r--   0        0        0      396 2023-08-07 00:04:13.095451 task4-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    26052 2023-07-26 00:57:10.559780 task4-0.1.0/README.md
--rw-r--r--   0        0        0    26197 1970-01-01 00:00:00.000000 task4-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task4-0.1.2/LICENSE
+-rw-r--r--   0        0        0      259 2023-08-04 21:17:25.582564 task4-0.1.2/log_parser/__init__.py
+-rw-r--r--   0        0        0      117 2023-08-04 21:17:25.586547 task4-0.1.2/log_parser/__main__.py
+-rw-r--r--   0        0        0       23 2023-08-07 13:17:09.089703 task4-0.1.2/log_parser/__version__.py
+-rw-r--r--   0        0        0      151 2023-08-04 21:17:25.566551 task4-0.1.2/log_parser/cli/__init__.py
+-rw-r--r--   0        0        0      117 2023-08-04 21:17:25.571572 task4-0.1.2/log_parser/cli/__main__.py
+-rw-r--r--   0        0        0    12491 2023-08-07 12:48:30.719050 task4-0.1.2/log_parser/cli/cli.py
+-rw-r--r--   0        0        0     7817 2023-08-04 19:51:24.232095 task4-0.1.2/log_parser/cli/patterns.py
+-rw-r--r--   0        0        0    15604 2023-08-07 02:18:32.532814 task4-0.1.2/log_parser/log_parser.py
+-rw-r--r--   0        0        0       98 2023-08-07 10:54:47.910859 task4-0.1.2/log_parser/showcase/__init__.py
+-rw-r--r--   0        0        0      139 2023-08-07 10:54:47.915859 task4-0.1.2/log_parser/showcase/__main__.py
+-rw-r--r--   0        0        0 36936434 2017-07-27 13:29:20.000000 task4-0.1.2/log_parser/showcase/access.log
+-rw-r--r--   0        0        0    27128 2023-08-07 12:19:50.128825 task4-0.1.2/log_parser/showcase/showcase.py
+-rw-r--r--   0        0        0      518 2023-08-07 13:17:09.085705 task4-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    26052 2023-07-26 00:57:10.559780 task4-0.1.2/README.md
+-rw-r--r--   0        0        0    26197 1970-01-01 00:00:00.000000 task4-0.1.2/PKG-INFO
```

### Comparing `task4-0.1.0/log_parser/cli/cli.py` & `task4-0.1.2/log_parser/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task4-0.1.0/log_parser/cli/patterns.py` & `task4-0.1.2/log_parser/cli/patterns.py`

 * *Files identical despite different names*

### Comparing `task4-0.1.0/log_parser/log_parser.py` & `task4-0.1.2/log_parser/log_parser.py`

 * *Files identical despite different names*

### Comparing `task4-0.1.0/log_parser/showcase/access.log` & `task4-0.1.2/log_parser/showcase/access.log`

 * *Files identical despite different names*

### Comparing `task4-0.1.0/log_parser/showcase/showcase.py` & `task4-0.1.2/log_parser/showcase/showcase.py`

 * *Files identical despite different names*

### Comparing `task4-0.1.0/README.md` & `task4-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `task4-0.1.0/PKG-INFO` & `task4-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task4
-Version: 0.1.0
+Version: 0.1.2
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
-Metadata-Version: 2.1 Name: task4 Version: 0.1.0 Summary: Log file parser CLI
+Metadata-Version: 2.1 Name: task4 Version: 0.1.2 Summary: Log file parser CLI
 and library License: MIT Author: Bill.Avramenko Author-email:
 billavramenko@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: questionary
 (>=1.10.0,<2.0.0) Description-Content-Type: text/markdown
```

