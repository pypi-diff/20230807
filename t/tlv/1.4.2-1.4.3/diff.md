# Comparing `tmp/tlv-1.4.2.tar.gz` & `tmp/tlv-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlv-1.4.2.tar", last modified: Wed Aug  2 09:47:16 2023, max compression
+gzip compressed data, was "tlv-1.4.3.tar", last modified: Mon Aug  7 11:42:16 2023, max compression
```

## Comparing `tlv-1.4.2.tar` & `tlv-1.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:47:16.759681 tlv-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-02 09:46:58.000000 tlv-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 09:46:58.000000 tlv-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-08-02 09:47:16.763681 tlv-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-08-02 09:46:58.000000 tlv-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 09:46:58.000000 tlv-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 09:47:16.763681 tlv-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-02 09:47:16.000000 tlv-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:47:16.759681 tlv-1.4.2/tlv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/cls_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/src_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-02 09:46:58.000000 tlv-1.4.2/tlv/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:47:16.759681 tlv-1.4.2/tlv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 09:47:16.000000 tlv-1.4.2/tlv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:42:16.498504 tlv-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-07 11:41:57.000000 tlv-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 11:41:57.000000 tlv-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-08-07 11:42:16.498504 tlv-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-08-07 11:41:57.000000 tlv-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 11:41:57.000000 tlv-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-07 11:42:16.498504 tlv-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-07 11:42:16.000000 tlv-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:42:16.494504 tlv-1.4.3/tlv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:41:57.000000 tlv-1.4.3/tlv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-07 11:41:57.000000 tlv-1.4.3/tlv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-07 11:41:57.000000 tlv-1.4.3/tlv/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-08-07 11:41:57.000000 tlv-1.4.3/tlv/cls_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-07 11:41:57.000000 tlv-1.4.3/tlv/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-08-07 11:41:57.000000 tlv-1.4.3/tlv/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-08-07 11:41:57.000000 tlv-1.4.3/tlv/src_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-07 11:41:57.000000 tlv-1.4.3/tlv/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:42:16.498504 tlv-1.4.3/tlv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-08-07 11:42:16.000000 tlv-1.4.3/tlv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-07 11:42:16.000000 tlv-1.4.3/tlv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:42:16.000000 tlv-1.4.3/tlv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 11:42:16.000000 tlv-1.4.3/tlv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-07 11:42:16.000000 tlv-1.4.3/tlv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-07 11:42:16.000000 tlv-1.4.3/tlv.egg-info/top_level.txt
```

### Comparing `tlv-1.4.2/LICENSE` & `tlv-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tlv-1.4.2/PKG-INFO` & `tlv-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlv
-Version: 1.4.2
+Version: 1.4.3
 Summary: -- Too less variation -- Find duplicates in source code for various languages
 Home-page: https://github.com/priv-kweihmann/tlv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tlv-1.4.2/README.md` & `tlv-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `tlv-1.4.2/setup.py` & `tlv-1.4.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="tlv",
-    version="1.4.2",
+    version="1.4.3",
     author="Konrad Weihmann",
     author_email="kweihmann@outlook.com",
     description="-- Too less variation -- Find duplicates in source code for various languages",
     long_description=_long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/priv-kweihmann/tlv",
     packages=setuptools.find_packages(),
```

### Comparing `tlv-1.4.2/tlv/arg_parser.py` & `tlv-1.4.3/tlv/arg_parser.py`

 * *Files identical despite different names*

### Comparing `tlv-1.4.2/tlv/cls_ast.py` & `tlv-1.4.3/tlv/cls_ast.py`

 * *Files identical despite different names*

### Comparing `tlv-1.4.2/tlv/lexer.py` & `tlv-1.4.3/tlv/lexer.py`

 * *Files identical despite different names*

### Comparing `tlv-1.4.2/tlv/src_parser.py` & `tlv-1.4.3/tlv/src_parser.py`

 * *Files identical despite different names*

### Comparing `tlv-1.4.2/tlv/tokens.py` & `tlv-1.4.3/tlv/tokens.py`

 * *Files identical despite different names*

### Comparing `tlv-1.4.2/tlv.egg-info/PKG-INFO` & `tlv-1.4.3/tlv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlv
-Version: 1.4.2
+Version: 1.4.3
 Summary: -- Too less variation -- Find duplicates in source code for various languages
 Home-page: https://github.com/priv-kweihmann/tlv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

