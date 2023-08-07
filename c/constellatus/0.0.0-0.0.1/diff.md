# Comparing `tmp/constellatus-0.0.0.tar.gz` & `tmp/constellatus-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constellatus-0.0.0.tar", last modified: Sat Jul 29 05:06:14 2023, max compression
+gzip compressed data, was "constellatus-0.0.1.tar", last modified: Mon Aug  7 00:21:07 2023, max compression
```

## Comparing `constellatus-0.0.0.tar` & `constellatus-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2023-07-29 05:06:14.826509 constellatus-0.0.0/
--rw-rw-r--   0 eons      (1000) eons      (1000)      557 2023-07-29 05:06:14.826509 constellatus-0.0.0/PKG-INFO
--rw-rw-r--   0 eons      (1000) eons      (1000)       38 2023-07-29 05:05:46.000000 constellatus-0.0.0/README.md
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2023-07-29 05:06:14.790510 constellatus-0.0.0/pkg/
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2023-07-29 05:06:14.806509 constellatus-0.0.0/pkg/constellatus/
--rw-rw-r--   0 eons      (1000) eons      (1000)       28 2023-07-29 05:05:53.000000 constellatus-0.0.0/pkg/constellatus/__init__.py
--rw-rw-r--   0 eons      (1000) eons      (1000)       34 2023-07-29 05:05:53.000000 constellatus-0.0.0/pkg/constellatus/constellatus.py
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2023-07-29 05:06:14.822509 constellatus-0.0.0/pkg/constellatus.egg-info/
--rw-rw-r--   0 eons      (1000) eons      (1000)      557 2023-07-29 05:06:14.000000 constellatus-0.0.0/pkg/constellatus.egg-info/PKG-INFO
--rw-rw-r--   0 eons      (1000) eons      (1000)      256 2023-07-29 05:06:14.000000 constellatus-0.0.0/pkg/constellatus.egg-info/SOURCES.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)        1 2023-07-29 05:06:14.000000 constellatus-0.0.0/pkg/constellatus.egg-info/dependency_links.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)       13 2023-07-29 05:06:14.000000 constellatus-0.0.0/pkg/constellatus.egg-info/top_level.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)      104 2023-07-29 05:05:53.000000 constellatus-0.0.0/pyproject.toml
--rw-rw-r--   0 eons      (1000) eons      (1000)      704 2023-07-29 05:06:14.830510 constellatus-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:21:07.149932 constellatus-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-07 00:21:07.149932 constellatus-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-08-07 00:20:50.000000 constellatus-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:21:07.145932 constellatus-0.0.1/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:21:07.145932 constellatus-0.0.1/pkg/constellatus/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-07 00:20:58.000000 constellatus-0.0.1/pkg/constellatus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 00:20:58.000000 constellatus-0.0.1/pkg/constellatus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-08-07 00:20:58.000000 constellatus-0.0.1/pkg/constellatus/constellatus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:21:07.149932 constellatus-0.0.1/pkg/constellatus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-07 00:21:07.000000 constellatus-0.0.1/pkg/constellatus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-07 00:21:07.000000 constellatus-0.0.1/pkg/constellatus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:21:07.000000 constellatus-0.0.1/pkg/constellatus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 00:21:07.000000 constellatus-0.0.1/pkg/constellatus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 00:21:07.000000 constellatus-0.0.1/pkg/constellatus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 00:21:07.000000 constellatus-0.0.1/pkg/constellatus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-07 00:20:58.000000 constellatus-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-07 00:21:07.149932 constellatus-0.0.1/setup.cfg
```

### Comparing `constellatus-0.0.0/setup.cfg` & `constellatus-0.0.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = constellatus
-version = v0.0.0
+version = 0.0.1
 author = eons
 author_email = support@eons.llc
 description = Elder data composition
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/constellatus/constellatus
@@ -18,15 +18,22 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
+	eons
+	flask
+	apie
 
 [options.packages.find]
 where = pkg
 
+[options.entry_points]
+console_scripts = 
+	constellatus = constellatus:constellatus
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

