# Comparing `tmp/listcolouring-0.1.0.tar.gz` & `tmp/listcolouring-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "listcolouring-0.1.0.tar", max compression
+gzip compressed data, was "listcolouring-0.1.1.tar", max compression
```

## Comparing `listcolouring-0.1.0.tar` & `listcolouring-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2023-08-07 16:07:13.596807 listcolouring-0.1.0/LICENSE
--rw-r--r--   0        0        0      579 2023-08-07 16:07:13.596807 listcolouring-0.1.0/README.md
--rw-r--r--   0        0        0     1829 2023-08-07 16:07:13.596807 listcolouring-0.1.0/listcolouring/__init__.py
--rw-r--r--   0        0        0      405 2023-08-07 16:07:13.600807 listcolouring-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1112 1970-01-01 00:00:00.000000 listcolouring-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-07 16:07:13.596807 listcolouring-0.1.1/LICENSE
+-rw-r--r--   0        0        0      579 2023-08-07 16:07:13.596807 listcolouring-0.1.1/README.md
+-rw-r--r--   0        0        0     1829 2023-08-07 16:07:13.596807 listcolouring-0.1.1/listcolouring/__init__.py
+-rw-r--r--   0        0        0      405 2023-08-07 16:13:33.860779 listcolouring-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1163 1970-01-01 00:00:00.000000 listcolouring-0.1.1/PKG-INFO
```

### Comparing `listcolouring-0.1.0/LICENSE` & `listcolouring-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `listcolouring-0.1.0/README.md` & `listcolouring-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `listcolouring-0.1.0/listcolouring/__init__.py` & `listcolouring-0.1.1/listcolouring/__init__.py`

 * *Files identical despite different names*

### Comparing `listcolouring-0.1.0/PKG-INFO` & `listcolouring-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: listcolouring
-Version: 0.1.0
+Version: 0.1.1
 Summary: List colouring in Python with NetworkX.
 License: MIT
 Author: Matthew Henderson
 Author-email: matthew.james.henderson@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Description-Content-Type: text/markdown
 
 # list-colouring
```

