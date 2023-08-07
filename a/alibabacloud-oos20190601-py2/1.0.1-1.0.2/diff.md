# Comparing `tmp/alibabacloud_oos20190601_py2-1.0.1.tar.gz` & `tmp/alibabacloud_oos20190601_py2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oos20190601_py2-1.0.1.tar", last modified: Fri Jul 28 03:47:56 2023, max compression
+gzip compressed data, was "dist/alibabacloud_oos20190601_py2-1.0.2.tar", last modified: Mon Aug  7 07:36:32 2023, max compression
```

## Comparing `alibabacloud_oos20190601_py2-1.0.1.tar` & `alibabacloud_oos20190601_py2-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:47:56.000000 alibabacloud_oos20190601_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-28 03:47:55.000000 alibabacloud_oos20190601_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-28 03:47:55.000000 alibabacloud_oos20190601_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-28 03:47:55.000000 alibabacloud_oos20190601_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2500 2023-07-28 03:47:56.000000 alibabacloud_oos20190601_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-28 03:47:55.000000 alibabacloud_oos20190601_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-07-28 03:47:55.000000 alibabacloud_oos20190601_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:47:56.000000 alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 03:47:55.000000 alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135538 2023-07-28 03:47:55.000000 alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601/client.py
--rw-r--r--   0 root         (0) root         (0)   739464 2023-07-28 03:47:55.000000 alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 03:47:56.000000 alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2500 2023-07-28 03:47:56.000000 alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-28 03:47:56.000000 alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 03:47:56.000000 alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-28 03:47:56.000000 alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-28 03:47:56.000000 alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 03:47:56.000000 alibabacloud_oos20190601_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2931 2023-07-28 03:47:55.000000 alibabacloud_oos20190601_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 07:36:32.000000 alibabacloud_oos20190601_py2-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-08-07 07:36:32.000000 alibabacloud_oos20190601_py2-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 07:36:32.000000 alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135538 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601/client.py
+-rw-r--r--   0 root         (0) root         (0)   739464 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 07:36:32.000000 alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-07 07:36:32.000000 alibabacloud_oos20190601_py2-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2931 2023-08-07 07:36:31.000000 alibabacloud_oos20190601_py2-1.0.2/setup.py
```

### Comparing `alibabacloud_oos20190601_py2-1.0.1/LICENSE` & `alibabacloud_oos20190601_py2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601_py2-1.0.1/PKG-INFO` & `alibabacloud_oos20190601_py2-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_oos20190601_py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud Operation Orchestration Service (20190601) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oos20190601_py2-1.0.1/README-CN.md` & `alibabacloud_oos20190601_py2-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601_py2-1.0.1/README.md` & `alibabacloud_oos20190601_py2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601/client.py` & `alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601/models.py` & `alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_oos20190601_py2-1.0.1/alibabacloud_oos20190601_py2.egg-info/PKG-INFO` & `alibabacloud_oos20190601_py2-1.0.2/alibabacloud_oos20190601_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-oos20190601-py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud Operation Orchestration Service (20190601) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oos20190601_py2-1.0.1/setup.py` & `alibabacloud_oos20190601_py2-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_oos20190601_py2.
 
-Created on 28/07/2023
+Created on 07/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_oos20190601"
 NAME = "alibabacloud_oos20190601_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Operation Orchestration Service (20190601) SDK Library for Python2"
```

