# Comparing `tmp/python2verilog-0.1.0.tar.gz` & `tmp/python2verilog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python2verilog-0.1.0.tar", last modified: Sun Aug  6 19:57:27 2023, max compression
+gzip compressed data, was "python2verilog-0.1.1.tar", last modified: Sun Aug  6 20:29:24 2023, max compression
```

## Comparing `python2verilog-0.1.0.tar` & `python2verilog-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:57:27.766492 python2verilog-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-06 19:57:27.766492 python2verilog-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-08-06 19:57:17.000000 python2verilog-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-06 19:57:17.000000 python2verilog-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:57:27.766492 python2verilog-0.1.0/python2verilog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-06 19:57:27.000000 python2verilog-0.1.0/python2verilog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-06 19:57:27.000000 python2verilog-0.1.0/python2verilog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:57:27.000000 python2verilog-0.1.0/python2verilog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 19:57:27.000000 python2verilog-0.1.0/python2verilog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 19:57:27.766492 python2verilog-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:29:24.869988 python2verilog-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-06 20:29:24.869988 python2verilog-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-08-06 20:29:11.000000 python2verilog-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-06 20:29:11.000000 python2verilog-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:29:24.869988 python2verilog-0.1.1/python2verilog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-06 20:29:24.000000 python2verilog-0.1.1/python2verilog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-06 20:29:24.000000 python2verilog-0.1.1/python2verilog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:29:24.000000 python2verilog-0.1.1/python2verilog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 20:29:24.000000 python2verilog-0.1.1/python2verilog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 20:29:24.869988 python2verilog-0.1.1/setup.cfg
```

### Comparing `python2verilog-0.1.0/PKG-INFO` & `python2verilog-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.1.0
+Version: 0.1.1
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `python2verilog-0.1.0/README.md` & `python2verilog-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python2verilog-0.1.0/pyproject.toml` & `python2verilog-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python2verilog"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Kerry Wang", email = "kerrywang369@gmail.com" }]
 description = "Converts a subset of python generator functions into synthesizable sequential SystemVerilog"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `python2verilog-0.1.0/python2verilog.egg-info/PKG-INFO` & `python2verilog-0.1.1/python2verilog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.1.0
+Version: 0.1.1
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

