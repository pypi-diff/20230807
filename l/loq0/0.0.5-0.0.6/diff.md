# Comparing `tmp/loq0-0.0.5.tar.gz` & `tmp/loq0-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loq0-0.0.5.tar", last modified: Mon Aug  7 06:09:30 2023, max compression
+gzip compressed data, was "loq0-0.0.6.tar", last modified: Mon Aug  7 06:27:43 2023, max compression
```

## Comparing `loq0-0.0.5.tar` & `loq0-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,13 @@
-drwxr-xr-x   0 seo_hyun   (501) staff       (20)        0 2023-08-07 06:09:30.109263 loq0-0.0.5/
--rw-r--r--   0 seo_hyun   (501) staff       (20)      429 2023-08-07 06:09:30.109089 loq0-0.0.5/PKG-INFO
-drwxr-xr-x   0 seo_hyun   (501) staff       (20)        0 2023-08-07 06:09:30.108823 loq0-0.0.5/loq0.egg-info/
--rw-r--r--   0 seo_hyun   (501) staff       (20)      429 2023-08-07 06:09:30.000000 loq0-0.0.5/loq0.egg-info/PKG-INFO
--rw-r--r--   0 seo_hyun   (501) staff       (20)      120 2023-08-07 06:09:30.000000 loq0-0.0.5/loq0.egg-info/SOURCES.txt
--rw-r--r--   0 seo_hyun   (501) staff       (20)        1 2023-08-07 06:09:30.000000 loq0-0.0.5/loq0.egg-info/dependency_links.txt
--rw-r--r--   0 seo_hyun   (501) staff       (20)        1 2023-08-07 06:09:30.000000 loq0-0.0.5/loq0.egg-info/top_level.txt
--rw-r--r--   0 seo_hyun   (501) staff       (20)       38 2023-08-07 06:09:30.109339 loq0-0.0.5/setup.cfg
--rw-r--r--   0 seo_hyun   (501) staff       (20)      595 2023-08-07 06:05:02.000000 loq0-0.0.5/setup.py
+drwxr-xr-x   0 seo_hyun   (501) staff       (20)        0 2023-08-07 06:27:43.760267 loq0-0.0.6/
+-rw-r--r--   0 seo_hyun   (501) staff       (20)      429 2023-08-07 06:27:43.760097 loq0-0.0.6/PKG-INFO
+drwxr-xr-x   0 seo_hyun   (501) staff       (20)        0 2023-08-07 06:27:43.759079 loq0-0.0.6/loq0/
+-rw-r--r--   0 seo_hyun   (501) staff       (20)       98 2023-08-07 06:24:59.000000 loq0-0.0.6/loq0/__init__.py
+-rw-r--r--   0 seo_hyun   (501) staff       (20)       95 2023-07-11 12:12:01.000000 loq0-0.0.6/loq0/const.py
+-rw-r--r--   0 seo_hyun   (501) staff       (20)      983 2023-07-22 16:46:33.000000 loq0-0.0.6/loq0/game.py
+drwxr-xr-x   0 seo_hyun   (501) staff       (20)        0 2023-08-07 06:27:43.759858 loq0-0.0.6/loq0.egg-info/
+-rw-r--r--   0 seo_hyun   (501) staff       (20)      429 2023-08-07 06:27:43.000000 loq0-0.0.6/loq0.egg-info/PKG-INFO
+-rw-r--r--   0 seo_hyun   (501) staff       (20)      164 2023-08-07 06:27:43.000000 loq0-0.0.6/loq0.egg-info/SOURCES.txt
+-rw-r--r--   0 seo_hyun   (501) staff       (20)        1 2023-08-07 06:27:43.000000 loq0-0.0.6/loq0.egg-info/dependency_links.txt
+-rw-r--r--   0 seo_hyun   (501) staff       (20)        5 2023-08-07 06:27:43.000000 loq0-0.0.6/loq0.egg-info/top_level.txt
+-rw-r--r--   0 seo_hyun   (501) staff       (20)       38 2023-08-07 06:27:43.760328 loq0-0.0.6/setup.cfg
+-rw-r--r--   0 seo_hyun   (501) staff       (20)      574 2023-08-07 06:27:39.000000 loq0-0.0.6/setup.py
```

