# Comparing `tmp/urlincode2-0.5.4.tar.gz` & `tmp/urlincode2-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlincode2-0.5.4.tar", last modified: Mon Aug  7 11:37:03 2023, max compression
+gzip compressed data, was "urlincode2-0.5.5.tar", last modified: Mon Aug  7 11:52:59 2023, max compression
```

## Comparing `urlincode2-0.5.4.tar` & `urlincode2-0.5.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-07 11:37:03.776313 urlincode2-0.5.4/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      300 2023-08-07 11:37:03.776313 urlincode2-0.5.4/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-08-07 11:37:03.776313 urlincode2-0.5.4/setup.cfg
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      472 2023-08-07 11:36:57.000000 urlincode2-0.5.4/setup.py
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-07 11:37:03.776313 urlincode2-0.5.4/urlincode2.egg-info/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      300 2023-08-07 11:37:03.000000 urlincode2-0.5.4/urlincode2.egg-info/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      144 2023-08-07 11:37:03.000000 urlincode2-0.5.4/urlincode2.egg-info/SOURCES.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-07 11:37:03.000000 urlincode2-0.5.4/urlincode2.egg-info/dependency_links.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-07 11:37:03.000000 urlincode2-0.5.4/urlincode2.egg-info/top_level.txt
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-07 11:52:59.182190 urlincode2-0.5.5/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      412 2023-08-07 11:52:59.182190 urlincode2-0.5.5/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-08-07 11:52:59.182190 urlincode2-0.5.5/setup.cfg
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      584 2023-08-07 11:52:46.000000 urlincode2-0.5.5/setup.py
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-07 11:52:59.182190 urlincode2-0.5.5/urlincode2.egg-info/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      412 2023-08-07 11:52:59.000000 urlincode2-0.5.5/urlincode2.egg-info/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      144 2023-08-07 11:52:59.000000 urlincode2-0.5.5/urlincode2.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-07 11:52:59.000000 urlincode2-0.5.5/urlincode2.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-07 11:52:59.000000 urlincode2-0.5.5/urlincode2.egg-info/top_level.txt
```

