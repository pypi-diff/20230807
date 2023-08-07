# Comparing `tmp/hyperx-0.1.9.tar.gz` & `tmp/hyperx-2023.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperx-0.1.9.tar", last modified: Wed Aug  2 19:18:24 2023, max compression
+gzip compressed data, was "hyperx-2023.2.6.tar", last modified: Mon Aug  7 20:04:22 2023, max compression
```

## Comparing `hyperx-0.1.9.tar` & `hyperx-2023.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.777074 hyperx-0.1.9/
--rw-rw-rw-   0        0        0      535 2023-08-02 19:18:24.776074 hyperx-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.742698 hyperx-0.1.9/hyperx/
--rw-rw-rw-   0        0        0      747 2023-07-17 20:06:12.000000 hyperx-0.1.9/hyperx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.760774 hyperx-0.1.9/hyperx/api/
--rw-rw-rw-   0        0        0   161428 2023-08-02 19:09:25.000000 hyperx-0.1.9/hyperx/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.762774 hyperx-0.1.9/hyperx/api/types/
--rw-rw-rw-   0        0        0    23328 2023-08-02 18:26:00.000000 hyperx-0.1.9/hyperx/api/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.770074 hyperx-0.1.9/hyperx/library/
--rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.9/hyperx/library/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.9/hyperx/library/find.py
--rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.9/hyperx/library/library.py
-drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.774074 hyperx-0.1.9/hyperx/utils/
--rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.9/hyperx/utils/__init__.py
--rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.9/hyperx/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 19:18:24.758779 hyperx-0.1.9/hyperx.egg-info/
--rw-rw-rw-   0        0        0      535 2023-08-02 19:18:24.000000 hyperx-0.1.9/hyperx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-08-02 19:18:24.000000 hyperx-0.1.9/hyperx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 19:18:24.000000 hyperx-0.1.9/hyperx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-08-02 19:18:24.000000 hyperx-0.1.9/hyperx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-02 19:18:24.000000 hyperx-0.1.9/hyperx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      660 2023-08-02 19:18:07.000000 hyperx-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-02 19:18:24.777074 hyperx-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 20:04:22.086880 hyperx-2023.2.6/
+-rw-rw-rw-   0        0        0      538 2023-08-07 20:04:22.086880 hyperx-2023.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-2023.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 20:04:22.042971 hyperx-2023.2.6/hyperx/
+-rw-rw-rw-   0        0        0      747 2023-07-17 20:06:12.000000 hyperx-2023.2.6/hyperx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:04:22.071288 hyperx-2023.2.6/hyperx/api/
+-rw-rw-rw-   0        0        0   161428 2023-08-07 20:03:30.000000 hyperx-2023.2.6/hyperx/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:04:22.074288 hyperx-2023.2.6/hyperx/api/types/
+-rw-rw-rw-   0        0        0    23328 2023-08-07 20:03:11.000000 hyperx-2023.2.6/hyperx/api/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:04:22.080880 hyperx-2023.2.6/hyperx/library/
+-rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-2023.2.6/hyperx/library/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-2023.2.6/hyperx/library/find.py
+-rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-2023.2.6/hyperx/library/library.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:04:22.084880 hyperx-2023.2.6/hyperx/utils/
+-rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-2023.2.6/hyperx/utils/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-2023.2.6/hyperx/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:04:22.069292 hyperx-2023.2.6/hyperx.egg-info/
+-rw-rw-rw-   0        0        0      538 2023-08-07 20:04:21.000000 hyperx-2023.2.6/hyperx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-08-07 20:04:22.000000 hyperx-2023.2.6/hyperx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 20:04:21.000000 hyperx-2023.2.6/hyperx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-07 20:04:21.000000 hyperx-2023.2.6/hyperx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 20:04:21.000000 hyperx-2023.2.6/hyperx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      663 2023-08-07 19:59:10.000000 hyperx-2023.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 20:04:22.088268 hyperx-2023.2.6/setup.cfg
```

### Comparing `hyperx-0.1.9/PKG-INFO` & `hyperx-2023.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.9
+Version: 2023.2.6
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.9/hyperx/__init__.py` & `hyperx-2023.2.6/hyperx/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.9/hyperx/api/__init__.py` & `hyperx-2023.2.6/hyperx/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.9/hyperx/api/types/__init__.py` & `hyperx-2023.2.6/hyperx/api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.9/hyperx/library/find.py` & `hyperx-2023.2.6/hyperx/library/find.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.9/hyperx/library/library.py` & `hyperx-2023.2.6/hyperx/library/library.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.9/hyperx/utils/utils.py` & `hyperx-2023.2.6/hyperx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.9/hyperx.egg-info/PKG-INFO` & `hyperx-2023.2.6/hyperx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.9
+Version: 2023.2.6
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.9/pyproject.toml` & `hyperx-2023.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hyperx"
-version = "0.1.9"
+version = "2023.2.6"
 authors = [
   { name="Kelly Ann Smith", email="kellyann.smith@collieraerospace.com" },
   { name="Noah Prezant", email="noah.prezant@collieraerospace.com" },
 ]
 description = "HyperX scripting for Python"
 readme = "README.md"
 requires-python = ">=3.10"
```

