# Comparing `tmp/pysesh-0.1.0.tar.gz` & `tmp/pysesh-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysesh-0.1.0.tar", last modified: Mon Aug  7 05:02:56 2023, max compression
+gzip compressed data, was "pysesh-0.1.1.tar", last modified: Mon Aug  7 05:13:22 2023, max compression
```

## Comparing `pysesh-0.1.0.tar` & `pysesh-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:02:56.727201 pysesh-0.1.0/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      109 2023-08-07 05:02:56.727201 pysesh-0.1.0/PKG-INFO
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:02:56.727201 pysesh-0.1.0/pysesh/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     1273 2023-08-07 05:01:49.000000 pysesh-0.1.0/pysesh/__init__.py
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2217 2023-08-07 05:01:49.000000 pysesh-0.1.0/pysesh/env.py
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2428 2023-08-07 05:01:49.000000 pysesh-0.1.0/pysesh/main.py
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2949 2023-08-07 05:01:49.000000 pysesh-0.1.0/pysesh/session.py
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:02:56.727201 pysesh-0.1.0/pysesh.egg-info/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      109 2023-08-07 05:02:56.000000 pysesh-0.1.0/pysesh.egg-info/PKG-INFO
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      256 2023-08-07 05:02:56.000000 pysesh-0.1.0/pysesh.egg-info/SOURCES.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)        1 2023-08-07 05:02:56.000000 pysesh-0.1.0/pysesh.egg-info/dependency_links.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       44 2023-08-07 05:02:56.000000 pysesh-0.1.0/pysesh.egg-info/entry_points.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       28 2023-08-07 05:02:56.000000 pysesh-0.1.0/pysesh.egg-info/requires.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)        7 2023-08-07 05:02:56.000000 pysesh-0.1.0/pysesh.egg-info/top_level.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       38 2023-08-07 05:02:56.727201 pysesh-0.1.0/setup.cfg
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      419 2023-08-07 05:01:49.000000 pysesh-0.1.0/setup.py
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:13:22.590475 pysesh-0.1.1/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      265 2023-08-07 05:13:22.590475 pysesh-0.1.1/PKG-INFO
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:13:22.590475 pysesh-0.1.1/pysesh/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     1322 2023-08-07 05:12:05.000000 pysesh-0.1.1/pysesh/__init__.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2217 2023-08-07 05:01:49.000000 pysesh-0.1.1/pysesh/env.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2428 2023-08-07 05:01:49.000000 pysesh-0.1.1/pysesh/main.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2919 2023-08-07 05:12:49.000000 pysesh-0.1.1/pysesh/session.py
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:13:22.590475 pysesh-0.1.1/pysesh.egg-info/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      265 2023-08-07 05:13:22.000000 pysesh-0.1.1/pysesh.egg-info/PKG-INFO
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      256 2023-08-07 05:13:22.000000 pysesh-0.1.1/pysesh.egg-info/SOURCES.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)        1 2023-08-07 05:13:22.000000 pysesh-0.1.1/pysesh.egg-info/dependency_links.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       44 2023-08-07 05:13:22.000000 pysesh-0.1.1/pysesh.egg-info/entry_points.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       28 2023-08-07 05:13:22.000000 pysesh-0.1.1/pysesh.egg-info/requires.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)        7 2023-08-07 05:13:22.000000 pysesh-0.1.1/pysesh.egg-info/top_level.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       38 2023-08-07 05:13:22.590475 pysesh-0.1.1/setup.cfg
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      565 2023-08-07 05:10:35.000000 pysesh-0.1.1/setup.py
```

### Comparing `pysesh-0.1.0/pysesh/__init__.py` & `pysesh-0.1.1/pysesh/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ('s', '#00fc03'),
     ('l', '#F0F0F0'),
 ])
 
 def cpr(text: str):
     console.print(text)
 
-parser = argparse.ArgumentParser(description='Python Multiplexer (pysesh) - A CLI to handle Python sessions.')
+parser = argparse.ArgumentParser(description='Python Multiplex - A Session Management Utility for Python.')
 subparsers = parser.add_subparsers(dest='command')
 
 new_parser = subparsers.add_parser('new', help='Create a new session.')
 new_parser.add_argument('name', type=str, help='Name of the new session.')
 
 load_parser = subparsers.add_parser('load', help='Load an existing session.')
 load_parser.add_argument('name', type=str, help='Name of the session to load.')
@@ -35,10 +35,12 @@
 delete_parser.add_argument('name', type=str, help='Name of the session to delete.')
 
 list_parser = subparsers.add_parser('list', help='List all available sessions.')
 
 args = parser.parse_args()
 
 
-REPOSITORY = os.path.join(os.path.dirname(__file__), 'state', 'sessions.pickle')
+REPOSITORY = os.path.join(os.path.dirname(__file__), 'sessions.pickle')
 DIRECTORY = os.path.join(os.path.dirname(__file__), 'state')
 
+if not os.path.exists(DIRECTORY):
+    os.makedirs(DIRECTORY)
```

### Comparing `pysesh-0.1.0/pysesh/env.py` & `pysesh-0.1.1/pysesh/env.py`

 * *Files identical despite different names*

### Comparing `pysesh-0.1.0/pysesh/main.py` & `pysesh-0.1.1/pysesh/main.py`

 * *Files identical despite different names*

### Comparing `pysesh-0.1.0/pysesh/session.py` & `pysesh-0.1.1/pysesh/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import inquirer  # add this import at the top
+import inquirer
 from pysesh import os, pickle, console, color, col, sys, inquirer, REPOSITORY, cpr
 
 
 def load_sessions():
     try:
         with open(REPOSITORY, 'rb') as f:
             return pickle.load(f)
```

