# Comparing `tmp/dgarbsutils-1.6.0.tar.gz` & `tmp/dgarbsutils-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgarbsutils-1.6.0.tar", last modified: Mon Aug  7 12:30:46 2023, max compression
+gzip compressed data, was "dgarbsutils-1.6.2.tar", last modified: Mon Aug  7 12:43:51 2023, max compression
```

## Comparing `dgarbsutils-1.6.0.tar` & `dgarbsutils-1.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:30:46.684533 dgarbsutils-1.6.0/
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1072 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      913 2023-08-07 12:30:46.688533 dgarbsutils-1.6.0/PKG-INFO
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      419 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/README.md
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       84 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/pyproject.toml
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      693 2023-08-07 12:30:46.688533 dgarbsutils-1.6.0/setup.cfg
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:30:46.684533 dgarbsutils-1.6.0/src/
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:30:46.684533 dgarbsutils-1.6.0/src/dgarbsutils/
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     2311 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/Cloudwatch.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5604 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/DynamoDB.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2069 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/EventBridge.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6879 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/GraphMail.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/__init__.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     7118 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/awsUtils.py
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5839 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/src/dgarbsutils/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:30:46.684533 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      913 2023-08-07 12:30:46.000000 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      455 2023-08-07 12:30:46.000000 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-08-07 12:30:46.000000 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       31 2023-08-07 12:30:46.000000 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       12 2023-08-07 12:30:46.000000 dgarbsutils-1.6.0/src/dgarbsutils.egg-info/top_level.txt
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:30:46.684533 dgarbsutils-1.6.0/tests/
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1782 2023-08-07 12:19:54.000000 dgarbsutils-1.6.0/tests/test_utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:43:51.023655 dgarbsutils-1.6.2/
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1072 2023-08-07 12:19:54.000000 dgarbsutils-1.6.2/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      913 2023-08-07 12:43:51.023655 dgarbsutils-1.6.2/PKG-INFO
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      419 2023-08-07 12:19:54.000000 dgarbsutils-1.6.2/README.md
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)       84 2023-08-07 12:19:54.000000 dgarbsutils-1.6.2/pyproject.toml
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)      693 2023-08-07 12:43:51.023655 dgarbsutils-1.6.2/setup.cfg
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:43:51.019656 dgarbsutils-1.6.2/src/
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:43:51.019656 dgarbsutils-1.6.2/src/dgarbsutils/
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     2311 2023-08-07 12:19:54.000000 dgarbsutils-1.6.2/src/dgarbsutils/Cloudwatch.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5604 2023-08-07 12:19:54.000000 dgarbsutils-1.6.2/src/dgarbsutils/DynamoDB.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2069 2023-08-07 12:19:54.000000 dgarbsutils-1.6.2/src/dgarbsutils/EventBridge.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6879 2023-08-07 12:19:54.000000 dgarbsutils-1.6.2/src/dgarbsutils/GraphMail.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:19:54.000000 dgarbsutils-1.6.2/src/dgarbsutils/__init__.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     7118 2023-08-07 12:19:54.000000 dgarbsutils-1.6.2/src/dgarbsutils/awsUtils.py
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     5839 2023-08-07 12:19:54.000000 dgarbsutils-1.6.2/src/dgarbsutils/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:43:51.023655 dgarbsutils-1.6.2/src/dgarbsutils.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      913 2023-08-07 12:43:51.000000 dgarbsutils-1.6.2/src/dgarbsutils.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      455 2023-08-07 12:43:51.000000 dgarbsutils-1.6.2/src/dgarbsutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-08-07 12:43:51.000000 dgarbsutils-1.6.2/src/dgarbsutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       31 2023-08-07 12:43:51.000000 dgarbsutils-1.6.2/src/dgarbsutils.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       12 2023-08-07 12:43:51.000000 dgarbsutils-1.6.2/src/dgarbsutils.egg-info/top_level.txt
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-07 12:43:51.023655 dgarbsutils-1.6.2/tests/
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1782 2023-08-07 12:19:54.000000 dgarbsutils-1.6.2/tests/test_utils.py
```

### Comparing `dgarbsutils-1.6.0/LICENSE` & `dgarbsutils-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.6.0/PKG-INFO` & `dgarbsutils-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgarbsutils
-Version: 1.6.0
+Version: 1.6.2
 Summary: A set of curated utils
 Home-page: https://github.com/dgarbalo/py-utils
 Author: Devon Garbalosa
 Author-email: dgarbalo@gmail.com
 Project-URL: Bug Tracker, https://github.com/dgarbalo/py-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dgarbsutils-1.6.0/setup.cfg` & `dgarbsutils-1.6.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dgarbsutils
-version = 1.6.0
+version = 1.6.2
 author = Devon Garbalosa
 author_email = dgarbalo@gmail.com
 description = A set of curated utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/dgarbalo/py-utils
 project_urls =
```

### Comparing `dgarbsutils-1.6.0/src/dgarbsutils/Cloudwatch.py` & `dgarbsutils-1.6.2/src/dgarbsutils/Cloudwatch.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.6.0/src/dgarbsutils/DynamoDB.py` & `dgarbsutils-1.6.2/src/dgarbsutils/DynamoDB.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.6.0/src/dgarbsutils/EventBridge.py` & `dgarbsutils-1.6.2/src/dgarbsutils/EventBridge.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.6.0/src/dgarbsutils/GraphMail.py` & `dgarbsutils-1.6.2/src/dgarbsutils/GraphMail.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.6.0/src/dgarbsutils/awsUtils.py` & `dgarbsutils-1.6.2/src/dgarbsutils/awsUtils.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.6.0/src/dgarbsutils/utils.py` & `dgarbsutils-1.6.2/src/dgarbsutils/utils.py`

 * *Files identical despite different names*

### Comparing `dgarbsutils-1.6.0/src/dgarbsutils.egg-info/PKG-INFO` & `dgarbsutils-1.6.2/src/dgarbsutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgarbsutils
-Version: 1.6.0
+Version: 1.6.2
 Summary: A set of curated utils
 Home-page: https://github.com/dgarbalo/py-utils
 Author: Devon Garbalosa
 Author-email: dgarbalo@gmail.com
 Project-URL: Bug Tracker, https://github.com/dgarbalo/py-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dgarbsutils-1.6.0/tests/test_utils.py` & `dgarbsutils-1.6.2/tests/test_utils.py`

 * *Files identical despite different names*

