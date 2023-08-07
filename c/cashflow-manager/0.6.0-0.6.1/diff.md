# Comparing `tmp/cashflow_manager-0.6.0.tar.gz` & `tmp/cashflow_manager-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashflow_manager-0.6.0.tar", max compression
+gzip compressed data, was "cashflow_manager-0.6.1.tar", max compression
```

## Comparing `cashflow_manager-0.6.0.tar` & `cashflow_manager-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        6 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/VERSION
--rw-r--r--   0        0        0        0 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/budget/__init__.py
--rw-r--r--   0        0        0     1430 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/budget/cli.py
--rw-r--r--   0        0        0     1163 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/budget/processor.py
--rw-r--r--   0        0        0     1562 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/days/main.py
--rw-r--r--   0        0        0        0 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/statement/__init__.py
--rw-r--r--   0        0        0      922 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/statement/budget.py
--rw-r--r--   0        0        0      857 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/statement/category.py
--rw-r--r--   0        0        0     2131 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/statement/cli.py
--rw-r--r--   0        0        0     8325 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/statement/processor.py
--rw-r--r--   0        0        0      377 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/cashflow/statement/vocab.py
--rw-r--r--   0        0        0      613 2023-04-02 19:19:32.346850 cashflow_manager-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 cashflow_manager-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/VERSION
+-rw-r--r--   0        0        0        0 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/budget/__init__.py
+-rw-r--r--   0        0        0     1430 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/budget/cli.py
+-rw-r--r--   0        0        0     1163 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/budget/processor.py
+-rw-r--r--   0        0        0     1562 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/days/main.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/statement/__init__.py
+-rw-r--r--   0        0        0      922 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/statement/budget.py
+-rw-r--r--   0        0        0      857 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/statement/category.py
+-rw-r--r--   0        0        0     2131 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/statement/cli.py
+-rw-r--r--   0        0        0     8325 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/statement/processor.py
+-rw-r--r--   0        0        0      377 2023-08-07 09:48:21.576400 cashflow_manager-0.6.1/cashflow/statement/vocab.py
+-rw-r--r--   0        0        0      613 2023-08-07 09:48:21.580400 cashflow_manager-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 cashflow_manager-0.6.1/PKG-INFO
```

### Comparing `cashflow_manager-0.6.0/cashflow/budget/cli.py` & `cashflow_manager-0.6.1/cashflow/budget/cli.py`

 * *Files identical despite different names*

### Comparing `cashflow_manager-0.6.0/cashflow/budget/processor.py` & `cashflow_manager-0.6.1/cashflow/budget/processor.py`

 * *Files identical despite different names*

### Comparing `cashflow_manager-0.6.0/cashflow/days/main.py` & `cashflow_manager-0.6.1/cashflow/days/main.py`

 * *Files identical despite different names*

### Comparing `cashflow_manager-0.6.0/cashflow/statement/budget.py` & `cashflow_manager-0.6.1/cashflow/statement/budget.py`

 * *Files identical despite different names*

### Comparing `cashflow_manager-0.6.0/cashflow/statement/category.py` & `cashflow_manager-0.6.1/cashflow/statement/category.py`

 * *Files identical despite different names*

### Comparing `cashflow_manager-0.6.0/cashflow/statement/cli.py` & `cashflow_manager-0.6.1/cashflow/statement/cli.py`

 * *Files identical despite different names*

### Comparing `cashflow_manager-0.6.0/cashflow/statement/processor.py` & `cashflow_manager-0.6.1/cashflow/statement/processor.py`

 * *Files identical despite different names*

### Comparing `cashflow_manager-0.6.0/pyproject.toml` & `cashflow_manager-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cashflow-manager"
-version = "0.6.0"
+version = "0.6.1"
 description = "Import transaction in Notion cashflow and budget manager"
 authors = ["lparolari <luca.parolari23@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "cashflow" },
 ]
```

### Comparing `cashflow_manager-0.6.0/PKG-INFO` & `cashflow_manager-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflow-manager
-Version: 0.6.0
+Version: 0.6.1
 Summary: Import transaction in Notion cashflow and budget manager
 License: MIT
 Author: lparolari
 Author-email: luca.parolari23@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

