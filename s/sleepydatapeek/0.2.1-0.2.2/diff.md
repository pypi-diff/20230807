# Comparing `tmp/sleepydatapeek-0.2.1.tar.gz` & `tmp/sleepydatapeek-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepydatapeek-0.2.1.tar", max compression
+gzip compressed data, was "sleepydatapeek-0.2.2.tar", max compression
```

## Comparing `sleepydatapeek-0.2.1.tar` & `sleepydatapeek-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-07-30 21:27:14.923251 sleepydatapeek-0.2.1/LICENSE
--rw-r--r--   0        0        0     1817 2023-08-01 22:30:32.920527 sleepydatapeek-0.2.1/README.md
--rw-r--r--   0        0        0      621 2023-08-02 17:58:03.679036 sleepydatapeek-0.2.1/pyproject.toml
--rwxr-xr-x   0        0        0      929 2023-08-02 17:53:04.431941 sleepydatapeek-0.2.1/sleepydatapeek.py
--rw-r--r--   0        0        0     1907 2023-08-02 17:53:14.924276 sleepydatapeek-0.2.1/toolchain/commands.py
--rw-r--r--   0        0        0      247 2023-08-02 17:52:32.204969 sleepydatapeek-0.2.1/toolchain/utils.py
--rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 sleepydatapeek-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-30 21:27:14.923251 sleepydatapeek-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1817 2023-08-01 22:30:32.920527 sleepydatapeek-0.2.2/README.md
+-rw-r--r--   0        0        0      621 2023-08-07 02:45:05.923835 sleepydatapeek-0.2.2/pyproject.toml
+-rwxr-xr-x   0        0        0      929 2023-08-02 17:53:04.431941 sleepydatapeek-0.2.2/sleepydatapeek.py
+-rw-r--r--   0        0        0     1907 2023-08-02 17:53:14.924276 sleepydatapeek-0.2.2/toolchain/commands.py
+-rw-r--r--   0        0        0      247 2023-08-02 17:52:32.204969 sleepydatapeek-0.2.2/toolchain/utils.py
+-rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 sleepydatapeek-0.2.2/PKG-INFO
```

### Comparing `sleepydatapeek-0.2.1/LICENSE` & `sleepydatapeek-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.2.1/README.md` & `sleepydatapeek-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.2.1/pyproject.toml` & `sleepydatapeek-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepydatapeek"
-version = "0.2.1"
+version = "0.2.2"
 description = "Peek at local datafiles fast!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 repository = "https://github.com/anthonybench/datapeek"
 keywords = ["pandas", "data"]
 packages = [
```

### Comparing `sleepydatapeek-0.2.1/sleepydatapeek.py` & `sleepydatapeek-0.2.2/sleepydatapeek.py`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.2.1/toolchain/commands.py` & `sleepydatapeek-0.2.2/toolchain/commands.py`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.2.1/PKG-INFO` & `sleepydatapeek-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepydatapeek
-Version: 0.2.1
+Version: 0.2.2
 Summary: Peek at local datafiles fast!
 Home-page: https://github.com/anthonybench/datapeek
 License: GNU GPL
 Keywords: pandas,data
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```

