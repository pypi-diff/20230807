# Comparing `tmp/ecr-scan-notifier-0.0.8.tar.gz` & `tmp/ecr-scan-notifier-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecr-scan-notifier-0.0.8.tar", last modified: Mon Jul 24 06:58:55 2023, max compression
+gzip compressed data, was "ecr-scan-notifier-0.0.9.tar", last modified: Mon Jul 31 17:14:12 2023, max compression
```

## Comparing `ecr-scan-notifier-0.0.8.tar` & `ecr-scan-notifier-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:55.704112 ecr-scan-notifier-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-24 06:58:38.000000 ecr-scan-notifier-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 06:58:38.000000 ecr-scan-notifier-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-24 06:58:55.704112 ecr-scan-notifier-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-24 06:58:38.000000 ecr-scan-notifier-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 06:58:38.000000 ecr-scan-notifier-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:58:55.704112 ecr-scan-notifier-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-24 06:58:38.000000 ecr-scan-notifier-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:55.700112 ecr-scan-notifier-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:55.704112 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier/
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-24 06:58:38.000000 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:55.704112 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 06:58:38.000000 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-07-24 06:58:38.000000 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier/_jsii/ecr-scan-notifier@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:58:38.000000 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:58:55.704112 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-24 06:58:55.000000 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-24 06:58:55.000000 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:58:55.000000 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 06:58:55.000000 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 06:58:55.000000 ecr-scan-notifier-0.0.8/src/ecr_scan_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:14:12.666937 ecr-scan-notifier-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-31 17:13:55.000000 ecr-scan-notifier-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 17:13:55.000000 ecr-scan-notifier-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-31 17:14:12.666937 ecr-scan-notifier-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-31 17:13:55.000000 ecr-scan-notifier-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 17:13:55.000000 ecr-scan-notifier-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 17:14:12.666937 ecr-scan-notifier-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-31 17:13:55.000000 ecr-scan-notifier-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:14:12.662937 ecr-scan-notifier-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:14:12.666937 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-31 17:13:55.000000 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:14:12.666937 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-31 17:13:55.000000 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23676 2023-07-31 17:13:55.000000 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier/_jsii/ecr-scan-notifier@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:13:55.000000 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:14:12.666937 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-31 17:14:12.000000 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-31 17:14:12.000000 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:14:12.000000 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-31 17:14:12.000000 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 17:14:12.000000 ecr-scan-notifier-0.0.9/src/ecr_scan_notifier.egg-info/top_level.txt
```

### Comparing `ecr-scan-notifier-0.0.8/LICENSE` & `ecr-scan-notifier-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ecr-scan-notifier-0.0.8/PKG-INFO` & `ecr-scan-notifier-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecr-scan-notifier
-Version: 0.0.8
+Version: 0.0.9
 Summary: Notifies on new AWS ECR scan results
 Home-page: https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Author: Stefan Freitag<stefan.freitag@rwe.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `ecr-scan-notifier-0.0.8/README.md` & `ecr-scan-notifier-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ecr-scan-notifier-0.0.8/setup.py` & `ecr-scan-notifier-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ecr-scan-notifier",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "Notifies on new AWS ECR scan results",
     "license": "Apache-2.0",
     "url": "https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@rwe.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "ecr_scan_notifier",
         "ecr_scan_notifier._jsii"
     ],
     "package_data": {
         "ecr_scan_notifier._jsii": [
-            "ecr-scan-notifier@0.0.8.jsii.tgz"
+            "ecr-scan-notifier@0.0.9.jsii.tgz"
         ],
         "ecr_scan_notifier": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ecr-scan-notifier-0.0.8/src/ecr_scan_notifier/__init__.py` & `ecr-scan-notifier-0.0.9/src/ecr_scan_notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `ecr-scan-notifier-0.0.8/src/ecr_scan_notifier.egg-info/PKG-INFO` & `ecr-scan-notifier-0.0.9/src/ecr_scan_notifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecr-scan-notifier
-Version: 0.0.8
+Version: 0.0.9
 Summary: Notifies on new AWS ECR scan results
 Home-page: https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Author: Stefan Freitag<stefan.freitag@rwe.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/cdk-ecr-scan-notifier.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

