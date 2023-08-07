# Comparing `tmp/alibabacloud_oos20190601-1.0.6.tar.gz` & `tmp/alibabacloud_oos20190601-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oos20190601-1.0.6.tar", last modified: Fri Jul 28 03:48:23 2023, max compression
+gzip compressed data, was "dist/alibabacloud_oos20190601-1.0.7.tar", last modified: Mon Aug  7 07:37:11 2023, max compression
```

## Comparing `alibabacloud_oos20190601-1.0.6.tar` & `alibabacloud_oos20190601-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      544 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2356 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316523 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601/client.py
--rw-r--r--   0 root         (0) root         (0)   735938 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2356 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2639 2023-07-28 03:48:23.000000 alibabacloud_oos20190601-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      601 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316523 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601/client.py
+-rw-r--r--   0 root         (0) root         (0)   735938 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-08-07 07:37:11.000000 alibabacloud_oos20190601-1.0.7/setup.py
```

### Comparing `alibabacloud_oos20190601-1.0.6/ChangeLog.md` & `alibabacloud_oos20190601-1.0.7/ChangeLog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-28 Version: 1.0.6
+- PatchBaseline Support Tags.
+
 2022-11-07 Version: 1.0.5
 - Update StartExecution add Parameter TemplateURL.
    Update StartExecution Parameter TemplateName to optional.
    Update ValidateTemplateContent add Parameter TemplateURL.
    Update ValidateTemplateContent Parameter TemplateConten to optional.
 
 2022-09-15 Version: 1.0.4
```

### Comparing `alibabacloud_oos20190601-1.0.6/LICENSE` & `alibabacloud_oos20190601-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601-1.0.6/PKG-INFO` & `alibabacloud_oos20190601-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_oos20190601
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud Operation Orchestration Service (20190601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oos20190601-1.0.6/README-CN.md` & `alibabacloud_oos20190601-1.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601-1.0.6/README.md` & `alibabacloud_oos20190601-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601/client.py` & `alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601/models.py` & `alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601-1.0.6/alibabacloud_oos20190601.egg-info/PKG-INFO` & `alibabacloud_oos20190601-1.0.7/alibabacloud_oos20190601.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-oos20190601
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud Operation Orchestration Service (20190601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oos20190601-1.0.6/setup.py` & `alibabacloud_oos20190601-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_oos20190601.
 
-Created on 28/07/2023
+Created on 07/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_oos20190601"
 NAME = "alibabacloud_oos20190601" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Operation Orchestration Service (20190601) SDK Library for Python"
```

