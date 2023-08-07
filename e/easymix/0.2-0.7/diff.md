# Comparing `tmp/easymix-0.2.tar.gz` & `tmp/easymix-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymix-0.2.tar", last modified: Sun Aug  6 18:40:49 2023, max compression
+gzip compressed data, was "easymix-0.7.tar", last modified: Sun Aug  6 22:23:06 2023, max compression
```

## Comparing `easymix-0.2.tar` & `easymix-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 18:40:49.770185 easymix-0.2/
--rw-r--r--   0 ze        (1000) ze        (1000)    26526 2023-07-17 08:23:51.000000 easymix-0.2/LICENSE
--rw-r--r--   0 ze        (1000) ze        (1000)       59 2023-08-06 18:23:42.000000 easymix-0.2/MANIFEST.in
--rw-r--r--   0 ze        (1000) ze        (1000)      115 2023-08-06 18:40:49.770185 easymix-0.2/PKG-INFO
--rw-r--r--   0 ze        (1000) ze        (1000)        0 2023-08-06 18:22:11.000000 easymix-0.2/README.md
-drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 18:40:49.770185 easymix-0.2/easymix.egg-info/
--rw-r--r--   0 ze        (1000) ze        (1000)      115 2023-08-06 18:40:49.000000 easymix-0.2/easymix.egg-info/PKG-INFO
--rw-r--r--   0 ze        (1000) ze        (1000)      195 2023-08-06 18:40:49.000000 easymix-0.2/easymix.egg-info/SOURCES.txt
--rw-r--r--   0 ze        (1000) ze        (1000)        1 2023-08-06 18:40:49.000000 easymix-0.2/easymix.egg-info/dependency_links.txt
--rw-r--r--   0 ze        (1000) ze        (1000)        4 2023-08-06 18:40:49.000000 easymix-0.2/easymix.egg-info/top_level.txt
--rw-r--r--   0 ze        (1000) ze        (1000)       13 2023-08-06 18:23:00.000000 easymix-0.2/requirements.txt
--rw-r--r--   0 ze        (1000) ze        (1000)       38 2023-08-06 18:40:49.770185 easymix-0.2/setup.cfg
--rw-r--r--   0 ze        (1000) ze        (1000)      178 2023-08-06 18:39:46.000000 easymix-0.2/setup.py
-drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 18:40:49.770185 easymix-0.2/src/
--rw-r--r--   0 ze        (1000) ze        (1000)     1899 2023-08-02 16:46:13.000000 easymix-0.2/src/__init__.py
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 22:23:06.813834 easymix-0.7/
+-rw-r--r--   0 ze        (1000) ze        (1000)    26526 2023-07-17 08:23:51.000000 easymix-0.7/LICENSE
+-rw-r--r--   0 ze        (1000) ze        (1000)      322 2023-08-06 22:23:06.813834 easymix-0.7/PKG-INFO
+-rw-r--r--   0 ze        (1000) ze        (1000)      870 2023-08-06 22:22:28.000000 easymix-0.7/README.md
+-rw-r--r--   0 ze        (1000) ze        (1000)       38 2023-08-06 22:23:06.813834 easymix-0.7/setup.cfg
+-rw-r--r--   0 ze        (1000) ze        (1000)      582 2023-08-06 22:22:50.000000 easymix-0.7/setup.py
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 22:23:06.813834 easymix-0.7/src/
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 22:23:06.813834 easymix-0.7/src/easymix/
+-rw-r--r--   0 ze        (1000) ze        (1000)     1899 2023-08-02 16:46:13.000000 easymix-0.7/src/easymix/__init__.py
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 22:23:06.813834 easymix-0.7/src/easymix.egg-info/
+-rw-r--r--   0 ze        (1000) ze        (1000)      322 2023-08-06 22:23:06.000000 easymix-0.7/src/easymix.egg-info/PKG-INFO
+-rw-r--r--   0 ze        (1000) ze        (1000)      224 2023-08-06 22:23:06.000000 easymix-0.7/src/easymix.egg-info/SOURCES.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)        1 2023-08-06 22:23:06.000000 easymix-0.7/src/easymix.egg-info/dependency_links.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)       14 2023-08-06 22:23:06.000000 easymix-0.7/src/easymix.egg-info/requires.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)        8 2023-08-06 22:23:06.000000 easymix-0.7/src/easymix.egg-info/top_level.txt
```

### Comparing `easymix-0.2/LICENSE` & `easymix-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easymix-0.2/src/__init__.py` & `easymix-0.7/src/easymix/__init__.py`

 * *Files identical despite different names*

