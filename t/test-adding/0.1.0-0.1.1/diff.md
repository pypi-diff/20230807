# Comparing `tmp/test-adding-0.1.0.tar.gz` & `tmp/test-adding-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-adding-0.1.0.tar", last modified: Mon Aug  7 14:10:11 2023, max compression
+gzip compressed data, was "test-adding-0.1.1.tar", last modified: Mon Aug  7 14:23:55 2023, max compression
```

## Comparing `test-adding-0.1.0.tar` & `test-adding-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 14:10:11.896035 test-adding-0.1.0/
--rw-rw-rw-   0        0        0       58 2023-08-07 14:10:11.895034 test-adding-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-07 14:07:09.000000 test-adding-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 14:10:11.887035 test-adding-0.1.0/adding/
--rw-rw-rw-   0        0        0       33 2023-08-07 14:05:34.000000 test-adding-0.1.0/adding/__init__.py
--rw-rw-rw-   0        0        0      206 2023-08-07 13:59:29.000000 test-adding-0.1.0/adding/addition.py
--rw-rw-rw-   0        0        0       42 2023-08-07 14:10:11.896035 test-adding-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      284 2023-08-07 14:08:00.000000 test-adding-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-07 14:10:11.894034 test-adding-0.1.0/test_adding.egg-info/
--rw-rw-rw-   0        0        0       58 2023-08-07 14:10:11.000000 test-adding-0.1.0/test_adding.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-08-07 14:10:11.000000 test-adding-0.1.0/test_adding.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 14:10:11.000000 test-adding-0.1.0/test_adding.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-08-07 14:10:11.000000 test-adding-0.1.0/test_adding.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-08-07 14:10:11.000000 test-adding-0.1.0/test_adding.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 14:23:55.591033 test-adding-0.1.1/
+-rw-rw-rw-   0        0        0       58 2023-08-07 14:23:55.590033 test-adding-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-07 14:07:09.000000 test-adding-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 14:23:55.582033 test-adding-0.1.1/adding/
+-rw-rw-rw-   0        0        0       33 2023-08-07 14:05:34.000000 test-adding-0.1.1/adding/__init__.py
+-rw-rw-rw-   0        0        0      206 2023-08-07 13:59:29.000000 test-adding-0.1.1/adding/addition.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 14:23:55.591033 test-adding-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      284 2023-08-07 14:23:10.000000 test-adding-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:23:55.589034 test-adding-0.1.1/test_adding.egg-info/
+-rw-rw-rw-   0        0        0       58 2023-08-07 14:23:55.000000 test-adding-0.1.1/test_adding.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-08-07 14:23:55.000000 test-adding-0.1.1/test_adding.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 14:23:55.000000 test-adding-0.1.1/test_adding.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-08-07 14:23:55.000000 test-adding-0.1.1/test_adding.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 14:23:55.000000 test-adding-0.1.1/test_adding.egg-info/top_level.txt
```

