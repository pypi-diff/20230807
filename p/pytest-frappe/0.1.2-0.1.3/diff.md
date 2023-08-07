# Comparing `tmp/pytest-frappe-0.1.2.tar.gz` & `tmp/pytest-frappe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-frappe-0.1.2.tar", last modified: Wed May  3 17:08:09 2023, max compression
+gzip compressed data, was "pytest-frappe-0.1.3.tar", last modified: Mon Aug  7 13:32:27 2023, max compression
```

## Comparing `pytest-frappe-0.1.2.tar` & `pytest-frappe-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.1.2/.gitignore
--rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.1.2/LICENSE
--rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.1.2/Makefile
--rw-r--r--   0        0        0     1501 2023-04-17 15:11:03.689905 pytest-frappe-0.1.2/README.md
--rw-r--r--   0        0        0     1411 2023-04-17 14:28:42.325679 pytest-frappe-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      119 2023-05-03 17:07:20.190671 pytest-frappe-0.1.2/pytest_frappe/__init__.py
--rw-r--r--   0        0        0     1186 2023-05-03 16:59:23.590048 pytest-frappe-0.1.2/pytest_frappe/fixtures.py
--rw-r--r--   0        0        0      399 2023-05-03 17:07:19.774674 pytest-frappe-0.1.2/pytest_frappe/plugin.py
--rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.1.2/setup.cfg
--rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 pytest-frappe-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-04-14 11:50:24.300726 pytest-frappe-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1066 2023-04-14 11:37:30.475170 pytest-frappe-0.1.3/LICENSE
+-rw-r--r--   0        0        0      356 2023-04-14 12:07:20.818247 pytest-frappe-0.1.3/Makefile
+-rw-r--r--   0        0        0     1501 2023-04-17 15:11:03.689905 pytest-frappe-0.1.3/README.md
+-rw-r--r--   0        0        0     1411 2023-04-17 14:28:42.325679 pytest-frappe-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      171 2023-08-07 13:30:14.677286 pytest-frappe-0.1.3/pytest_frappe/__init__.py
+-rw-r--r--   0        0        0     1186 2023-05-03 16:59:23.590048 pytest-frappe-0.1.3/pytest_frappe/fixtures.py
+-rw-r--r--   0        0        0      234 2023-08-07 13:30:14.825285 pytest-frappe-0.1.3/pytest_frappe/mock_utils.py
+-rw-r--r--   0        0        0      399 2023-05-03 17:07:19.774674 pytest-frappe-0.1.3/pytest_frappe/plugin.py
+-rw-r--r--   0        0        0      279 2023-04-14 12:07:08.826506 pytest-frappe-0.1.3/setup.cfg
+-rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 pytest-frappe-0.1.3/PKG-INFO
```

### Comparing `pytest-frappe-0.1.2/.gitignore` & `pytest-frappe-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.1.2/LICENSE` & `pytest-frappe-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.1.2/README.md` & `pytest-frappe-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.1.2/pyproject.toml` & `pytest-frappe-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.1.2/pytest_frappe/fixtures.py` & `pytest-frappe-0.1.3/pytest_frappe/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-frappe-0.1.2/PKG-INFO` & `pytest-frappe-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-frappe
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pytest Frappe Plugin - A set of pytest fixtures to test Frappe applications
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

