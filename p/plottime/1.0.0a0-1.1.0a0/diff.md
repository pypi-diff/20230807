# Comparing `tmp/plottime-1.0.0a0.tar.gz` & `tmp/plottime-1.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plottime-1.0.0a0.tar", last modified: Tue May 16 15:19:18 2023, max compression
+gzip compressed data, was "plottime-1.1.0a0.tar", last modified: Mon Aug  7 08:43:48 2023, max compression
```

## Comparing `plottime-1.0.0a0.tar` & `plottime-1.1.0a0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 francesco   (501) staff       (20)        0 2023-05-16 15:19:18.532010 plottime-1.0.0a0/
--rw-r--r--   0 francesco   (501) staff       (20)      104 2023-05-16 15:19:18.532064 plottime-1.0.0a0/PKG-INFO
--rw-r--r--   0 francesco   (501) staff       (20)       10 2023-03-16 13:43:47.000000 plottime-1.0.0a0/README.md
-drwxr-xr-x   0 francesco   (501) staff       (20)        0 2023-05-16 15:19:18.531372 plottime-1.0.0a0/plottime/
--rw-r--r--   0 francesco   (501) staff       (20)     2926 2023-05-16 14:53:47.000000 plottime-1.0.0a0/plottime/plot.py
-drwxr-xr-x   0 francesco   (501) staff       (20)        0 2023-05-16 15:19:18.531909 plottime-1.0.0a0/plottime.egg-info/
--rw-r--r--   0 francesco   (501) staff       (20)      104 2023-05-16 15:19:18.000000 plottime-1.0.0a0/plottime.egg-info/PKG-INFO
--rw-r--r--   0 francesco   (501) staff       (20)      204 2023-05-16 15:19:18.000000 plottime-1.0.0a0/plottime.egg-info/SOURCES.txt
--rw-r--r--   0 francesco   (501) staff       (20)        1 2023-05-16 15:19:18.000000 plottime-1.0.0a0/plottime.egg-info/dependency_links.txt
--rw-r--r--   0 francesco   (501) staff       (20)       25 2023-05-16 15:19:18.000000 plottime-1.0.0a0/plottime.egg-info/requires.txt
--rw-r--r--   0 francesco   (501) staff       (20)        9 2023-05-16 15:19:18.000000 plottime-1.0.0a0/plottime.egg-info/top_level.txt
--rw-r--r--   0 francesco   (501) staff       (20)      220 2023-05-16 15:19:18.532251 plottime-1.0.0a0/setup.cfg
--rw-r--r--   0 francesco   (501) staff       (20)       69 2022-12-29 21:08:12.000000 plottime-1.0.0a0/setup.py
+drwxr-xr-x   0 francesco   (501) staff       (20)        0 2023-08-07 08:43:48.878613 plottime-1.1.0a0/
+-rw-r--r--   0 francesco   (501) staff       (20)      104 2023-08-07 08:43:48.878656 plottime-1.1.0a0/PKG-INFO
+-rw-r--r--   0 francesco   (501) staff       (20)       10 2023-03-16 13:43:47.000000 plottime-1.1.0a0/README.md
+drwxr-xr-x   0 francesco   (501) staff       (20)        0 2023-08-07 08:43:48.878000 plottime-1.1.0a0/plottime/
+-rw-r--r--   0 francesco   (501) staff       (20)     2926 2023-05-31 07:33:28.000000 plottime-1.1.0a0/plottime/plot.py
+-rw-r--r--   0 francesco   (501) staff       (20)      357 2023-05-31 07:33:44.000000 plottime-1.1.0a0/plottime/utils.py
+drwxr-xr-x   0 francesco   (501) staff       (20)        0 2023-08-07 08:43:48.878521 plottime-1.1.0a0/plottime.egg-info/
+-rw-r--r--   0 francesco   (501) staff       (20)      104 2023-08-07 08:43:48.000000 plottime-1.1.0a0/plottime.egg-info/PKG-INFO
+-rw-r--r--   0 francesco   (501) staff       (20)      222 2023-08-07 08:43:48.000000 plottime-1.1.0a0/plottime.egg-info/SOURCES.txt
+-rw-r--r--   0 francesco   (501) staff       (20)        1 2023-08-07 08:43:48.000000 plottime-1.1.0a0/plottime.egg-info/dependency_links.txt
+-rw-r--r--   0 francesco   (501) staff       (20)       25 2023-08-07 08:43:48.000000 plottime-1.1.0a0/plottime.egg-info/requires.txt
+-rw-r--r--   0 francesco   (501) staff       (20)        9 2023-08-07 08:43:48.000000 plottime-1.1.0a0/plottime.egg-info/top_level.txt
+-rw-r--r--   0 francesco   (501) staff       (20)      220 2023-08-07 08:43:48.878981 plottime-1.1.0a0/setup.cfg
+-rw-r--r--   0 francesco   (501) staff       (20)       69 2022-12-29 21:08:12.000000 plottime-1.1.0a0/setup.py
```

### Comparing `plottime-1.0.0a0/plottime/plot.py` & `plottime-1.1.0a0/plottime/plot.py`

 * *Files identical despite different names*

