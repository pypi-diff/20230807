# Comparing `tmp/sllim-0.1.8.tar.gz` & `tmp/sllim-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sllim-0.1.8.tar", max compression
+gzip compressed data, was "sllim-0.1.9.tar", max compression
```

## Comparing `sllim-0.1.8.tar` & `sllim-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1060 2023-05-15 16:22:10.877704 sllim-0.1.8/LICENSE
--rw-r--r--   0        0        0     1383 2023-05-29 12:04:13.123988 sllim-0.1.8/README.md
--rw-r--r--   0        0        0      322 2023-07-19 21:19:53.213680 sllim-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    12393 2023-07-19 21:19:30.443426 sllim-0.1.8/sllim/__init__.py
--rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 sllim-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-05-15 16:22:10.877704 sllim-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1383 2023-05-29 12:04:13.123988 sllim-0.1.9/README.md
+-rw-r--r--   0        0        0      322 2023-07-26 20:48:03.660772 sllim-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    12399 2023-07-26 20:47:57.327418 sllim-0.1.9/sllim/__init__.py
+-rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 sllim-0.1.9/PKG-INFO
```

### Comparing `sllim-0.1.8/LICENSE` & `sllim-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sllim-0.1.8/README.md` & `sllim-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sllim-0.1.8/sllim/__init__.py` & `sllim-0.1.9/sllim/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     # Load from cache
     if local_cache:
         with open(cache_file) as w:
             cache = json.load(w)
 
     def wrapper(*args, **kwargs):
         if kwargs.get("nocache", False) or not local_cache:
-            kwargs.pop("nocache")
+            kwargs.pop("nocache", None)
             return fn(*args, **kwargs)
 
         key = str(args + tuple(kwargs.items()))
         if key not in cache:
             res = fn(*args, **kwargs)
             cache[key] = res
             with open(cache_file, "w") as w:
```

### Comparing `sllim-0.1.8/PKG-INFO` & `sllim-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sllim
-Version: 0.1.8
+Version: 0.1.9
 Summary: Fixing the openai api
 Author: Kaiser Pister
 Author-email: kaiser@pister.dev
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

