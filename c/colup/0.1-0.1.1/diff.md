# Comparing `tmp/colup-0.1.tar.gz` & `tmp/colup-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\colup-0.1.tar", last modified: Sat Aug  5 13:55:56 2023, max compression
+gzip compressed data, was "dist\colup-0.1.1.tar", last modified: Mon Aug  7 20:09:37 2023, max compression
```

## Comparing `colup-0.1.tar` & `colup-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 13:55:56.011528 colup-0.1/
--rw-rw-rw-   0        0        0      187 2023-08-05 13:55:56.010005 colup-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-05 13:55:56.007493 colup-0.1/colup.egg-info/
--rw-rw-rw-   0        0        0      187 2023-08-05 13:55:55.000000 colup-0.1/colup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2023-08-05 13:55:55.000000 colup-0.1/colup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 13:55:55.000000 colup-0.1/colup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-05 13:55:55.000000 colup-0.1/colup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 13:55:55.000000 colup-0.1/colup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      734 2023-08-05 13:46:43.000000 colup-0.1/file_uploader.py
--rw-rw-rw-   0        0        0       42 2023-08-05 13:55:56.012111 colup-0.1/setup.cfg
--rw-rw-rw-   0        0        0      233 2023-08-05 13:43:38.000000 colup-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:09:37.893316 colup-0.1.1/
+-rw-rw-rw-   0        0        0      298 2023-08-07 20:09:37.880330 colup-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 20:09:37.873135 colup-0.1.1/colup.egg-info/
+-rw-rw-rw-   0        0        0      298 2023-08-07 20:09:37.000000 colup-0.1.1/colup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-08-07 20:09:37.000000 colup-0.1.1/colup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 20:09:37.000000 colup-0.1.1/colup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-08-07 20:09:37.000000 colup-0.1.1/colup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 20:09:37.000000 colup-0.1.1/colup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 20:09:37.000000 colup-0.1.1/colup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      734 2023-08-07 11:47:05.000000 colup-0.1.1/file_uploader.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 20:09:37.895919 colup-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      594 2023-08-07 20:07:46.000000 colup-0.1.1/setup.py
```

### Comparing `colup-0.1/file_uploader.py` & `colup-0.1.1/file_uploader.py`

 * *Files identical despite different names*

