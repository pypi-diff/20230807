# Comparing `tmp/Nabilkz-1.1.tar.gz` & `tmp/Nabilkz-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nabilkz-1.1.tar", last modified: Thu Aug  3 18:38:20 2023, max compression
+gzip compressed data, was "Nabilkz-1.2.tar", last modified: Mon Aug  7 18:42:04 2023, max compression
```

## Comparing `Nabilkz-1.1.tar` & `Nabilkz-1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:20.920293 Nabilkz-1.1/
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:20.900794 Nabilkz-1.1/Nabilkz/
--rw-rw-rw-   0        0        0     1891 2023-08-03 18:28:06.000000 Nabilkz-1.1/Nabilkz/Nabil.py
--rw-rw-rw-   0        0        0        0 2023-08-03 17:43:26.000000 Nabilkz-1.1/Nabilkz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 18:38:20.917291 Nabilkz-1.1/Nabilkz.egg-info/
--rw-rw-rw-   0        0        0      131 2023-08-03 18:38:20.000000 Nabilkz-1.1/Nabilkz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-08-03 18:38:20.000000 Nabilkz-1.1/Nabilkz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 18:38:20.000000 Nabilkz-1.1/Nabilkz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-03 18:38:20.000000 Nabilkz-1.1/Nabilkz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-03 18:38:20.000000 Nabilkz-1.1/Nabilkz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      131 2023-08-03 18:38:20.918295 Nabilkz-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-03 18:38:20.920293 Nabilkz-1.1/setup.cfg
--rw-rw-rw-   0        0        0      310 2023-08-03 18:38:14.000000 Nabilkz-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:42:04.905616 Nabilkz-1.2/
+drwxrwxrwx   0        0        0        0 2023-08-07 18:42:04.877733 Nabilkz-1.2/Nabilkz/
+-rw-rw-rw-   0        0        0     1891 2023-08-07 18:36:55.000000 Nabilkz-1.2/Nabilkz/Nabil.py
+-rw-rw-rw-   0        0        0     3201 2023-08-07 18:37:47.000000 Nabilkz-1.2/Nabilkz/Nabili2c.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 17:43:26.000000 Nabilkz-1.2/Nabilkz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 18:42:04.902699 Nabilkz-1.2/Nabilkz.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-08-07 18:42:04.000000 Nabilkz-1.2/Nabilkz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-08-07 18:42:04.000000 Nabilkz-1.2/Nabilkz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 18:42:04.000000 Nabilkz-1.2/Nabilkz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 18:42:04.000000 Nabilkz-1.2/Nabilkz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 18:42:04.000000 Nabilkz-1.2/Nabilkz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2023-08-07 18:42:04.904608 Nabilkz-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-07 18:42:04.905616 Nabilkz-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      340 2023-08-07 18:41:07.000000 Nabilkz-1.2/setup.py
```

### Comparing `Nabilkz-1.1/Nabilkz/Nabil.py` & `Nabilkz-1.2/Nabilkz/Nabil.py`

 * *Files identical despite different names*

