# Comparing `tmp/rand-omata-0.0.3.tar.gz` & `tmp/rand-omata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rand-omata-0.0.3.tar", last modified: Mon Aug  7 15:35:57 2023, max compression
+gzip compressed data, was "rand-omata-0.0.4.tar", last modified: Mon Aug  7 16:54:35 2023, max compression
```

## Comparing `rand-omata-0.0.3.tar` & `rand-omata-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 15:35:57.487817 rand-omata-0.0.3/
--rw-rw-rw-   0        0        0       84 2023-08-07 15:34:14.000000 rand-omata-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0       25 2023-08-07 15:34:04.000000 rand-omata-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      639 2023-08-07 15:35:57.486818 rand-omata-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       87 2023-08-07 15:33:36.000000 rand-omata-0.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-08-07 15:35:57.462818 rand-omata-0.0.3/rand_omata/
--rw-rw-rw-   0        0        0        0 2023-08-07 15:31:28.000000 rand-omata-0.0.3/rand_omata/__init__.py
--rw-rw-rw-   0        0        0     1498 2023-08-07 15:34:38.000000 rand-omata-0.0.3/rand_omata/rand_omata.py
-drwxrwxrwx   0        0        0        0 2023-08-07 15:35:57.485824 rand-omata-0.0.3/rand_omata.egg-info/
--rw-rw-rw-   0        0        0      639 2023-08-07 15:35:57.000000 rand-omata-0.0.3/rand_omata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-08-07 15:35:57.000000 rand-omata-0.0.3/rand_omata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 15:35:57.000000 rand-omata-0.0.3/rand_omata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-07 15:35:57.000000 rand-omata-0.0.3/rand_omata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-07 15:35:57.000000 rand-omata-0.0.3/rand_omata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 15:35:57.487817 rand-omata-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      706 2023-08-07 15:33:19.000000 rand-omata-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:54:35.597980 rand-omata-0.0.4/
+-rw-rw-rw-   0        0        0       85 2023-08-07 16:50:49.000000 rand-omata-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0       25 2023-08-07 15:34:04.000000 rand-omata-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      988 2023-08-07 16:54:35.597980 rand-omata-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-08-07 16:50:21.000000 rand-omata-0.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 16:54:35.597980 rand-omata-0.0.4/rand_omata/
+-rw-rw-rw-   0        0        0        0 2023-08-07 16:51:31.000000 rand-omata-0.0.4/rand_omata/__init__.py
+-rw-rw-rw-   0        0        0     1498 2023-08-07 16:51:34.000000 rand-omata-0.0.4/rand_omata/rand_omata.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:54:35.597980 rand-omata-0.0.4/rand_omata.egg-info/
+-rw-rw-rw-   0        0        0      988 2023-08-07 16:54:35.000000 rand-omata-0.0.4/rand_omata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-08-07 16:54:35.000000 rand-omata-0.0.4/rand_omata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 16:54:35.000000 rand-omata-0.0.4/rand_omata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 16:54:35.000000 rand-omata-0.0.4/rand_omata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 16:54:35.613602 rand-omata-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-08-07 16:54:15.000000 rand-omata-0.0.4/setup.py
```

### Comparing `rand-omata-0.0.3/rand_omata/rand_omata.py` & `rand-omata-0.0.4/rand_omata/rand_omata.py`

 * *Files identical despite different names*

