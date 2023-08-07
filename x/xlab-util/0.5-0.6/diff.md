# Comparing `tmp/xlab-util-0.5.tar.gz` & `tmp/xlab-util-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlab-util-0.5.tar", last modified: Mon Aug  7 11:10:27 2023, max compression
+gzip compressed data, was "xlab-util-0.6.tar", last modified: Mon Aug  7 11:12:21 2023, max compression
```

## Comparing `xlab-util-0.5.tar` & `xlab-util-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-07 11:10:27.351083 xlab-util-0.5/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-07 11:10:27.351083 xlab-util-0.5/PKG-INFO
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       11 2023-08-01 07:16:54.000000 xlab-util-0.5/README.md
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       38 2023-08-07 11:10:27.351083 xlab-util-0.5/setup.cfg
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      203 2023-08-07 11:08:41.000000 xlab-util-0.5/setup.py
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-07 11:10:27.347083 xlab-util-0.5/xlab_util.egg-info/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-07 11:10:27.000000 xlab-util-0.5/xlab_util.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      263 2023-08-07 11:10:27.000000 xlab-util-0.5/xlab_util.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        1 2023-08-07 11:10:27.000000 xlab-util-0.5/xlab_util.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        9 2023-08-07 11:10:27.000000 xlab-util-0.5/xlab_util.egg-info/top_level.txt
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-07 11:10:27.351083 xlab-util-0.5/xlabutil/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      210 2023-08-04 07:31:18.000000 xlab-util-0.5/xlabutil/__init__.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      407 2023-08-01 07:32:55.000000 xlab-util-0.5/xlabutil/base.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1560 2023-08-07 07:01:15.000000 xlab-util-0.5/xlabutil/inference.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1870 2023-08-07 11:07:20.000000 xlab-util-0.5/xlabutil/result.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       83 2023-08-04 07:12:05.000000 xlab-util-0.5/xlabutil/type.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      749 2023-08-01 07:33:04.000000 xlab-util-0.5/xlabutil/util.py
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-07 11:12:21.592330 xlab-util-0.6/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-07 11:12:21.592330 xlab-util-0.6/PKG-INFO
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       11 2023-08-01 07:16:54.000000 xlab-util-0.6/README.md
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       38 2023-08-07 11:12:21.592330 xlab-util-0.6/setup.cfg
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      203 2023-08-07 11:12:16.000000 xlab-util-0.6/setup.py
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-07 11:12:21.592330 xlab-util-0.6/xlab_util.egg-info/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-07 11:12:21.000000 xlab-util-0.6/xlab_util.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      263 2023-08-07 11:12:21.000000 xlab-util-0.6/xlab_util.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        1 2023-08-07 11:12:21.000000 xlab-util-0.6/xlab_util.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        9 2023-08-07 11:12:21.000000 xlab-util-0.6/xlab_util.egg-info/top_level.txt
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-07 11:12:21.592330 xlab-util-0.6/xlabutil/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      232 2023-08-07 11:12:10.000000 xlab-util-0.6/xlabutil/__init__.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      407 2023-08-01 07:32:55.000000 xlab-util-0.6/xlabutil/base.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1560 2023-08-07 07:01:15.000000 xlab-util-0.6/xlabutil/inference.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1870 2023-08-07 11:07:20.000000 xlab-util-0.6/xlabutil/result.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       83 2023-08-04 07:12:05.000000 xlab-util-0.6/xlabutil/type.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      749 2023-08-01 07:33:04.000000 xlab-util-0.6/xlabutil/util.py
```

### Comparing `xlab-util-0.5/xlabutil/inference.py` & `xlab-util-0.6/xlabutil/inference.py`

 * *Files identical despite different names*

### Comparing `xlab-util-0.5/xlabutil/result.py` & `xlab-util-0.6/xlabutil/result.py`

 * *Files identical despite different names*

### Comparing `xlab-util-0.5/xlabutil/util.py` & `xlab-util-0.6/xlabutil/util.py`

 * *Files identical despite different names*

