# Comparing `tmp/t_val-0.0.2.tar.gz` & `tmp/t_val-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\t_val-0.0.2.tar", last modified: Fri Aug  4 11:42:08 2023, max compression
+gzip compressed data, was "dist\t_val-0.0.3.tar", last modified: Mon Aug  7 07:25:04 2023, max compression
```

## Comparing `t_val-0.0.2.tar` & `t_val-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 11:42:08.000000 t_val-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-08-04 11:42:08.000000 t_val-0.0.2/libname/
--rw-rw-rw-   0        0        0      405 2023-08-04 11:17:21.000000 t_val-0.0.2/libname/t_val.py
--rw-rw-rw-   0        0        0       26 2023-08-04 09:59:35.000000 t_val-0.0.2/libname/__init__.py
--rw-rw-rw-   0        0        0      269 2023-08-04 11:42:08.000000 t_val-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-04 11:42:08.000000 t_val-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      386 2023-08-04 11:36:56.000000 t_val-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:42:08.000000 t_val-0.0.2/t_val.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-04 11:42:08.000000 t_val-0.0.2/t_val.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      269 2023-08-04 11:42:08.000000 t_val-0.0.2/t_val.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-08-04 11:42:08.000000 t_val-0.0.2/t_val.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-08-04 11:42:08.000000 t_val-0.0.2/t_val.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 07:25:04.000000 t_val-0.0.3/
+-rw-rw-rw-   0        0        0      200 2023-08-07 07:25:04.000000 t_val-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-07 07:25:04.000000 t_val-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      224 2023-08-07 06:07:01.000000 t_val-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:25:04.000000 t_val-0.0.3/t_val/
+-rw-rw-rw-   0        0        0      409 2023-08-07 06:04:30.000000 t_val-0.0.3/t_val/t_val.py
+-rw-rw-rw-   0        0        0        0 2023-08-07 06:03:07.000000 t_val-0.0.3/t_val/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 07:25:04.000000 t_val-0.0.3/t_val.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-07 07:25:04.000000 t_val-0.0.3/t_val.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      200 2023-08-07 07:25:04.000000 t_val-0.0.3/t_val.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-08-07 07:25:04.000000 t_val-0.0.3/t_val.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 07:25:04.000000 t_val-0.0.3/t_val.egg-info/top_level.txt
```

