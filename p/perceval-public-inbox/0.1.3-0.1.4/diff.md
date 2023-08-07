# Comparing `tmp/perceval_public_inbox-0.1.3.tar.gz` & `tmp/perceval_public_inbox-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_public_inbox-0.1.3.tar", max compression
+gzip compressed data, was "perceval_public_inbox-0.1.4.tar", max compression
```

## Comparing `perceval_public_inbox-0.1.3.tar` & `perceval_public_inbox-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       50 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/AUTHORS
--rw-r--r--   0        0        0    35149 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/LICENSE
--rw-r--r--   0        0        0      384 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/NEWS
--rw-r--r--   0        0        0     2291 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/perceval/backends/public_inbox/__init__.py
--rw-r--r--   0        0        0       86 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/perceval/backends/public_inbox/_version.py
--rw-r--r--   0        0        0    12428 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/perceval/backends/public_inbox/public_inbox.py
--rw-r--r--   0        0        0     1375 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    53248 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/tests/.coverage
--rw-r--r--   0        0        0        0 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0    77686 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/tests/data/public_inbox/alternate-repos.tar.gz
--rw-r--r--   0        0        0    18463 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/tests/data/public_inbox/example-repo.git.tar.gz
--rwxr-xr-x   0        0        0     1017 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/tests/run_tests.py
--rw-r--r--   0        0        0    18717 2023-07-24 09:31:54.526466 perceval_public_inbox-0.1.3/tests/test_public_inbox.py
--rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 perceval_public_inbox-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-08-07 09:45:57.630587 perceval_public_inbox-0.1.4/AUTHORS
+-rw-r--r--   0        0        0    35149 2023-08-07 09:45:57.630587 perceval_public_inbox-0.1.4/LICENSE
+-rw-r--r--   0        0        0      540 2023-08-07 09:45:57.630587 perceval_public_inbox-0.1.4/NEWS
+-rw-r--r--   0        0        0     2291 2023-08-07 09:45:57.630587 perceval_public_inbox-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-08-07 09:45:57.630587 perceval_public_inbox-0.1.4/perceval/backends/public_inbox/__init__.py
+-rw-r--r--   0        0        0       86 2023-08-07 09:45:57.630587 perceval_public_inbox-0.1.4/perceval/backends/public_inbox/_version.py
+-rw-r--r--   0        0        0    12428 2023-08-07 09:45:57.630587 perceval_public_inbox-0.1.4/perceval/backends/public_inbox/public_inbox.py
+-rw-r--r--   0        0        0     1375 2023-08-07 09:45:57.630587 perceval_public_inbox-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    53248 2023-08-07 09:45:57.630587 perceval_public_inbox-0.1.4/tests/.coverage
+-rw-r--r--   0        0        0        0 2023-08-07 09:45:57.630587 perceval_public_inbox-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0    77686 2023-08-07 09:45:57.634587 perceval_public_inbox-0.1.4/tests/data/public_inbox/alternate-repos.tar.gz
+-rw-r--r--   0        0        0    18463 2023-08-07 09:45:57.634587 perceval_public_inbox-0.1.4/tests/data/public_inbox/example-repo.git.tar.gz
+-rwxr-xr-x   0        0        0     1017 2023-08-07 09:45:57.634587 perceval_public_inbox-0.1.4/tests/run_tests.py
+-rw-r--r--   0        0        0    18717 2023-08-07 09:45:57.634587 perceval_public_inbox-0.1.4/tests/test_public_inbox.py
+-rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 perceval_public_inbox-0.1.4/PKG-INFO
```

### Comparing `perceval_public_inbox-0.1.3/LICENSE` & `perceval_public_inbox-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.3/README.md` & `perceval_public_inbox-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.3/perceval/backends/public_inbox/public_inbox.py` & `perceval_public_inbox-0.1.4/perceval/backends/public_inbox/public_inbox.py`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.3/pyproject.toml` & `perceval_public_inbox-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-public-inbox"
-version = "0.1.3"
+version = "0.1.4"
 description = "Perceval backend for public-inbox."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval_public_inbox-0.1.3/tests/.coverage` & `perceval_public_inbox-0.1.4/tests/.coverage`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.3/tests/data/public_inbox/alternate-repos.tar.gz` & `perceval_public_inbox-0.1.4/tests/data/public_inbox/alternate-repos.tar.gz`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.3/tests/data/public_inbox/example-repo.git.tar.gz` & `perceval_public_inbox-0.1.4/tests/data/public_inbox/example-repo.git.tar.gz`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.3/tests/run_tests.py` & `perceval_public_inbox-0.1.4/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.3/tests/test_public_inbox.py` & `perceval_public_inbox-0.1.4/tests/test_public_inbox.py`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.3/PKG-INFO` & `perceval_public_inbox-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-public-inbox
-Version: 0.1.3
+Version: 0.1.4
 Summary: Perceval backend for public-inbox.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

