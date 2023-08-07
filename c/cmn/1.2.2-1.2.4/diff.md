# Comparing `tmp/cmn-1.2.2.tar.gz` & `tmp/cmn-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmn-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cmn-1.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cmn-1.2.2.tar` & `cmn-1.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1005 2023-07-31 22:03:09.378237 cmn-1.2.2/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1127 2023-08-07 18:53:04.536799 cmn-1.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       88 2023-08-07 19:14:41.930601 cmn-1.2.2/.gitignore
--rw-r--r--   0        0        0     9229 2023-08-06 00:34:24.799239 cmn-1.2.2/LICENSE
--rw-r--r--   0        0        0     2649 2023-08-03 22:44:06.242819 cmn-1.2.2/README.md
--rw-r--r--   0        0        0      547 2023-08-07 19:46:55.577860 cmn-1.2.2/pyproject.toml
--rw-r--r--   0        0        0       15 2023-08-03 22:48:42.765195 cmn-1.2.2/requirements.txt
--rw-r--r--   0        0        0     4726 2023-08-07 19:02:33.161717 cmn-1.2.2/src/ChangeMediaName/ChangeMediaName.py
--rw-r--r--   0        0        0     1104 2023-08-06 01:09:25.634489 cmn-1.2.2/src/ColoredLogger/ColoredLogger.py
--rw-r--r--   0        0        0     2860 2023-08-06 01:09:25.666374 cmn-1.2.2/src/OutputFormatter/OutputFormatter.py
--rw-r--r--   0        0        0     2301 2023-08-07 19:01:17.007069 cmn-1.2.2/src/OutputFormatter/test_OutputFormatter.py
--rw-r--r--   0        0        0      132 2023-08-07 19:51:25.393052 cmn-1.2.2/src/cmn/__init__.py
--rw-r--r--   0        0        0     6480 2023-08-07 19:49:32.274293 cmn-1.2.2/src/cmn/__main__.py
--rw-r--r--   0        0        0     7046 2023-08-07 19:49:08.829047 cmn-1.2.2/src/test_main.py
--rw-r--r--   0        0        0     3048 1970-01-01 00:00:00.000000 cmn-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1005 2023-07-31 22:03:09.378237 cmn-1.2.4/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1127 2023-08-07 18:53:04.536799 cmn-1.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       88 2023-08-07 19:14:41.930601 cmn-1.2.4/.gitignore
+-rw-r--r--   0        0        0     9229 2023-08-06 00:34:24.799239 cmn-1.2.4/LICENSE
+-rw-r--r--   0        0        0     2649 2023-08-03 22:44:06.242819 cmn-1.2.4/README.md
+-rw-r--r--   0        0        0      552 2023-08-07 19:52:54.320230 cmn-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0       15 2023-08-03 22:48:42.765195 cmn-1.2.4/requirements.txt
+-rw-r--r--   0        0        0     4726 2023-08-07 19:02:33.161717 cmn-1.2.4/src/ChangeMediaName/ChangeMediaName.py
+-rw-r--r--   0        0        0     1104 2023-08-06 01:09:25.634489 cmn-1.2.4/src/ColoredLogger/ColoredLogger.py
+-rw-r--r--   0        0        0     2860 2023-08-06 01:09:25.666374 cmn-1.2.4/src/OutputFormatter/OutputFormatter.py
+-rw-r--r--   0        0        0     2301 2023-08-07 19:01:17.007069 cmn-1.2.4/src/OutputFormatter/test_OutputFormatter.py
+-rw-r--r--   0        0        0     3767 2023-08-07 19:58:00.913373 cmn-1.2.4/src/cmn/__init__.py
+-rw-r--r--   0        0        0     3071 2023-08-07 19:57:45.827010 cmn-1.2.4/src/cmn/__main__.py
+-rw-r--r--   0        0        0     7046 2023-08-07 19:49:08.829047 cmn-1.2.4/src/test_main.py
+-rw-r--r--   0        0        0     3048 1970-01-01 00:00:00.000000 cmn-1.2.4/PKG-INFO
```

### Comparing `cmn-1.2.2/.github/workflows/python-app.yml` & `cmn-1.2.4/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `cmn-1.2.2/.github/workflows/python-publish.yml` & `cmn-1.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cmn-1.2.2/LICENSE` & `cmn-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cmn-1.2.2/README.md` & `cmn-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cmn-1.2.2/pyproject.toml` & `cmn-1.2.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     "colorama >= 0.4.6"
 ]
 
 [project.urls]
 Home = "https://github.com/Henrique-190/ChangeMediaName"
 
 [project.scripts]
-cmn = "cmn.__init__"
+cmn = "cmn.__main__:main"
```

### Comparing `cmn-1.2.2/src/ChangeMediaName/ChangeMediaName.py` & `cmn-1.2.4/src/ChangeMediaName/ChangeMediaName.py`

 * *Files identical despite different names*

### Comparing `cmn-1.2.2/src/ColoredLogger/ColoredLogger.py` & `cmn-1.2.4/src/ColoredLogger/ColoredLogger.py`

 * *Files identical despite different names*

### Comparing `cmn-1.2.2/src/OutputFormatter/OutputFormatter.py` & `cmn-1.2.4/src/OutputFormatter/OutputFormatter.py`

 * *Files identical despite different names*

### Comparing `cmn-1.2.2/src/OutputFormatter/test_OutputFormatter.py` & `cmn-1.2.4/src/OutputFormatter/test_OutputFormatter.py`

 * *Files identical despite different names*

### Comparing `cmn-1.2.2/src/test_main.py` & `cmn-1.2.4/src/test_main.py`

 * *Files identical despite different names*

### Comparing `cmn-1.2.2/PKG-INFO` & `cmn-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmn
-Version: 1.2.2
+Version: 1.2.4
 Summary: Main - Module responsible for the main program. Parses the arguments and calls the other modules.
 Author-email: Henrique Alvelos <henriquealvelos@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: colorama >= 0.4.6
 Project-URL: Home, https://github.com/Henrique-190/ChangeMediaName
```

