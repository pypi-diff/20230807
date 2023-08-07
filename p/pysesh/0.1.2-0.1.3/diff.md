# Comparing `tmp/pysesh-0.1.2.tar.gz` & `tmp/pysesh-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysesh-0.1.2.tar", last modified: Mon Aug  7 05:24:52 2023, max compression
+gzip compressed data, was "pysesh-0.1.3.tar", last modified: Mon Aug  7 05:33:45 2023, max compression
```

## Comparing `pysesh-0.1.2.tar` & `pysesh-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:24:52.791092 pysesh-0.1.2/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      265 2023-08-07 05:24:52.791092 pysesh-0.1.2/PKG-INFO
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:24:52.791092 pysesh-0.1.2/pysesh/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     1226 2023-08-07 05:23:47.000000 pysesh-0.1.2/pysesh/__init__.py
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2217 2023-08-07 05:01:49.000000 pysesh-0.1.2/pysesh/env.py
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2501 2023-08-07 05:20:37.000000 pysesh-0.1.2/pysesh/main.py
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2919 2023-08-07 05:12:49.000000 pysesh-0.1.2/pysesh/session.py
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:24:52.791092 pysesh-0.1.2/pysesh.egg-info/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      265 2023-08-07 05:24:52.000000 pysesh-0.1.2/pysesh.egg-info/PKG-INFO
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      256 2023-08-07 05:24:52.000000 pysesh-0.1.2/pysesh.egg-info/SOURCES.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)        1 2023-08-07 05:24:52.000000 pysesh-0.1.2/pysesh.egg-info/dependency_links.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       44 2023-08-07 05:24:52.000000 pysesh-0.1.2/pysesh.egg-info/entry_points.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       28 2023-08-07 05:24:52.000000 pysesh-0.1.2/pysesh.egg-info/requires.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)        7 2023-08-07 05:24:52.000000 pysesh-0.1.2/pysesh.egg-info/top_level.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       38 2023-08-07 05:24:52.791092 pysesh-0.1.2/setup.cfg
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      565 2023-08-07 05:24:47.000000 pysesh-0.1.2/setup.py
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:33:45.287604 pysesh-0.1.3/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      265 2023-08-07 05:33:45.287604 pysesh-0.1.3/PKG-INFO
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:33:45.287604 pysesh-0.1.3/pysesh/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     1239 2023-08-07 05:33:33.000000 pysesh-0.1.3/pysesh/__init__.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2217 2023-08-07 05:01:49.000000 pysesh-0.1.3/pysesh/env.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2501 2023-08-07 05:20:37.000000 pysesh-0.1.3/pysesh/main.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2919 2023-08-07 05:12:49.000000 pysesh-0.1.3/pysesh/session.py
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-08-07 05:33:45.287604 pysesh-0.1.3/pysesh.egg-info/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      265 2023-08-07 05:33:45.000000 pysesh-0.1.3/pysesh.egg-info/PKG-INFO
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      256 2023-08-07 05:33:45.000000 pysesh-0.1.3/pysesh.egg-info/SOURCES.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)        1 2023-08-07 05:33:45.000000 pysesh-0.1.3/pysesh.egg-info/dependency_links.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       44 2023-08-07 05:33:45.000000 pysesh-0.1.3/pysesh.egg-info/entry_points.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       28 2023-08-07 05:33:45.000000 pysesh-0.1.3/pysesh.egg-info/requires.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)        7 2023-08-07 05:33:45.000000 pysesh-0.1.3/pysesh.egg-info/top_level.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       38 2023-08-07 05:33:45.287604 pysesh-0.1.3/setup.cfg
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      565 2023-08-07 05:33:39.000000 pysesh-0.1.3/setup.py
```

### Comparing `pysesh-0.1.2/pysesh/__init__.py` & `pysesh-0.1.3/pysesh/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,9 +35,9 @@
 delete_parser.add_argument('name', type=str, help='Name of the session to delete.')
 
 list_parser = subparsers.add_parser('list', help='List all available sessions.')
 
 args = parser.parse_args()
 
 
-DIRECTORY = os.path.join('/tmp', 'pysesh')
+DIRECTORY = os.path.abspath(os.path.dirname(__file__)))
 REPOSITORY = os.path.join(DIRECTORY, 'sessions.pickle')
```

### Comparing `pysesh-0.1.2/pysesh/env.py` & `pysesh-0.1.3/pysesh/env.py`

 * *Files identical despite different names*

### Comparing `pysesh-0.1.2/pysesh/main.py` & `pysesh-0.1.3/pysesh/main.py`

 * *Files identical despite different names*

### Comparing `pysesh-0.1.2/pysesh/session.py` & `pysesh-0.1.3/pysesh/session.py`

 * *Files identical despite different names*

### Comparing `pysesh-0.1.2/setup.py` & `pysesh-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pysesh',
-    version='0.1.2',
+    version='0.1.3',
     description='A Python Session Manager and Multiplexer, allowing you to manage multiple sessions and their respective states, and switch between them with ease.',
     author='Connor Etherington',
     author_email='connor@concise.cc',
     packages=find_packages(),
     install_requires=[
         'colr',
         'argparse',
```

