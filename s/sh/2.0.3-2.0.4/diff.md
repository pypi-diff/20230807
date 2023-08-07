# Comparing `tmp/sh-2.0.3.tar.gz` & `tmp/sh-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-2.0.3.tar", max compression
+gzip compressed data, was "sh-2.0.4.tar", max compression
```

## Comparing `sh-2.0.3.tar` & `sh-2.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    16832 2023-03-20 19:58:54.699480 sh-2.0.3/CHANGELOG.md
--rw-r--r--   0        0        0     1065 2023-03-20 19:58:54.699480 sh-2.0.3/LICENSE.txt
--rw-r--r--   0        0        0     2564 2023-03-20 19:58:54.699480 sh-2.0.3/MIGRATION.md
--rw-r--r--   0        0        0      452 2023-03-20 19:58:54.699480 sh-2.0.3/Makefile
--rw-r--r--   0        0        0     2423 2023-03-20 19:58:54.699480 sh-2.0.3/README.rst
--rw-r--r--   0        0        0    32464 2023-03-20 19:58:54.699480 sh-2.0.3/images/logo-230.png
--rw-r--r--   0        0        0   246823 2023-03-20 19:58:54.703480 sh-2.0.3/images/logo-big.png
--rw-r--r--   0        0        0     1767 2023-03-20 19:58:54.703480 sh-2.0.3/pyproject.toml
--rw-r--r--   0        0        0   127296 2023-03-20 19:58:54.703480 sh-2.0.3/sh.py
--rw-r--r--   0        0        0      973 2023-03-20 19:58:54.703480 sh-2.0.3/tests/Dockerfile
--rw-r--r--   0        0        0        0 2023-03-20 19:58:54.703480 sh-2.0.3/tests/__init__.py
--rw-r--r--   0        0        0    90334 2023-03-20 19:58:54.703480 sh-2.0.3/tests/test.py
--rw-r--r--   0        0        0      539 2023-03-20 19:58:54.703480 sh-2.0.3/tox.ini
--rw-r--r--   0        0        0     3821 1970-01-01 00:00:00.000000 sh-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0    17061 2023-05-15 15:25:18.729174 sh-2.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1065 2023-05-15 15:25:18.729174 sh-2.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     2564 2023-05-15 15:25:18.729174 sh-2.0.4/MIGRATION.md
+-rw-r--r--   0        0        0      452 2023-05-15 15:25:18.729174 sh-2.0.4/Makefile
+-rw-r--r--   0        0        0     2423 2023-05-15 15:25:18.729174 sh-2.0.4/README.rst
+-rw-r--r--   0        0        0    32464 2023-05-15 15:25:18.729174 sh-2.0.4/images/logo-230.png
+-rw-r--r--   0        0        0   246823 2023-05-15 15:25:18.729174 sh-2.0.4/images/logo-big.png
+-rw-r--r--   0        0        0     1767 2023-05-15 15:25:18.729174 sh-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0   127311 2023-05-15 15:25:18.729174 sh-2.0.4/sh.py
+-rw-r--r--   0        0        0      973 2023-05-15 15:25:18.729174 sh-2.0.4/tests/Dockerfile
+-rw-r--r--   0        0        0        0 2023-05-15 15:25:18.729174 sh-2.0.4/tests/__init__.py
+-rw-r--r--   0        0        0    90334 2023-05-15 15:25:18.733173 sh-2.0.4/tests/test.py
+-rw-r--r--   0        0        0      539 2023-05-15 15:25:18.733173 sh-2.0.4/tox.ini
+-rw-r--r--   0        0        0     3669 1970-01-01 00:00:00.000000 sh-2.0.4/PKG-INFO
```

### Comparing `sh-2.0.3/CHANGELOG.md` & `sh-2.0.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Changelog
 
-## 2.0.2 - 2/13/22
+## 2.0.4 - 5/13/22
+
+- Allow `ok_code` to be used with `fg` [#655](https://github.com/amoffat/sh/pull/655)
+- Make sure `new_group` never creates a new session [#675](https://github.com/amoffat/sh/pull/675)
+
+## 2.0.2 / 2.0.3 (misversioned) - 2/13/22
 
 - Performance regression when using a generator with `_in` [#650](https://github.com/amoffat/sh/pull/650)
 - Adding test support for python 3.11
 
 ## 2.0.0 - 2/9/22
 
 - Executed commands now return a unicode string by default
```

### Comparing `sh-2.0.3/LICENSE.txt` & `sh-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sh-2.0.3/MIGRATION.md` & `sh-2.0.4/MIGRATION.md`

 * *Files identical despite different names*

### Comparing `sh-2.0.3/README.rst` & `sh-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `sh-2.0.3/images/logo-230.png` & `sh-2.0.4/images/logo-230.png`

 * *Files identical despite different names*

### Comparing `sh-2.0.3/images/logo-big.png` & `sh-2.0.4/images/logo-big.png`

 * *Files identical despite different names*

### Comparing `sh-2.0.3/pyproject.toml` & `sh-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sh"
-version = "2.0.3"
+version = "2.0.4"
 description = "Python subprocess replacement"
 authors = ["Andrew Moffat <arwmoffat@gmail.com>"]
 readme = "README.rst"
 maintainers = [
     "Andrew Moffat <arwmoffat@gmail.com>",
     "Erik Cederstrand <erik@cederstrand.dk>"
 ]
```

### Comparing `sh-2.0.3/sh.py` & `sh-2.0.4/sh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1112,15 +1112,15 @@
     """fg is not valid with basically every other option"""
 
     invalid = []
     msg = """\
 _fg is invalid with nearly every other option, see warning and workaround here:
 
     https://amoffat.github.io/sh/sections/special_arguments.html#fg"""
-    allowlist = {"env", "fg", "cwd"}
+    allowlist = {"env", "fg", "cwd", "ok_code"}
     offending = set(passed_kwargs.keys()) - allowlist
 
     if "fg" in passed_kwargs and passed_kwargs["fg"] and offending:
         invalid.append(("fg", msg))
     return invalid
 
 
@@ -2033,15 +2033,15 @@
 
                 # put our forked process in a new session?  this will relinquish
                 # any control of our inherited CTTY and also make our parent
                 # process init
                 if new_session:
                     os.setsid()
                 elif new_group:
-                    os.setpgrp()
+                    os.setpgid(0, 0)
 
                 sid = os.getsid(0)
                 pgid = os.getpgid(0)
                 payload = ("%d,%d" % (sid, pgid)).encode(DEFAULT_ENCODING)
                 os.write(session_pipe_write, payload)
 
                 if ca["tty_out"] and not stdout_is_fd_based and not single_tty:
```

### Comparing `sh-2.0.3/tests/Dockerfile` & `sh-2.0.4/tests/Dockerfile`

 * *Files identical despite different names*

### Comparing `sh-2.0.3/tests/test.py` & `sh-2.0.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `sh-2.0.3/tox.ini` & `sh-2.0.4/tox.ini`

 * *Files identical despite different names*

### Comparing `sh-2.0.3/PKG-INFO` & `sh-2.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sh
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python subprocess replacement
 Home-page: https://amoffat.github.io/sh/
 License: MIT
 Author: Andrew Moffat
 Author-email: arwmoffat@gmail.com
 Maintainer: Andrew Moffat
 Maintainer-email: arwmoffat@gmail.com
@@ -15,18 +15,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Documentation, https://amoffat.github.io/sh/
 Project-URL: Repository, https://github.com/amoffat/sh
 Description-Content-Type: text/x-rst
```

