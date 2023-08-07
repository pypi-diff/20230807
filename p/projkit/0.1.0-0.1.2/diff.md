# Comparing `tmp/projkit-0.1.0.tar.gz` & `tmp/projkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projkit-0.1.0.tar", last modified: Mon Aug  7 12:10:28 2023, max compression
+gzip compressed data, was "projkit-0.1.2.tar", last modified: Mon Aug  7 12:36:01 2023, max compression
```

## Comparing `projkit-0.1.0.tar` & `projkit-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:10:28.723318 projkit-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 12:10:16.000000 projkit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-08-07 12:10:28.723318 projkit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-08-07 12:10:16.000000 projkit-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:10:28.719318 projkit-0.1.0/projkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 12:10:16.000000 projkit-0.1.0/projkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-08-07 12:10:16.000000 projkit-0.1.0/projkit/camops.py
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-08-07 12:10:16.000000 projkit-0.1.0/projkit/imutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-07 12:10:16.000000 projkit-0.1.0/projkit/pyutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:10:28.723318 projkit-0.1.0/projkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-08-07 12:10:28.000000 projkit-0.1.0/projkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-07 12:10:28.000000 projkit-0.1.0/projkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:10:28.000000 projkit-0.1.0/projkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 12:10:28.000000 projkit-0.1.0/projkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 12:10:28.000000 projkit-0.1.0/projkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 12:10:28.723318 projkit-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-08-07 12:10:16.000000 projkit-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:36:01.261457 projkit-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 12:35:50.000000 projkit-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-07 12:36:01.257456 projkit-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-08-07 12:35:50.000000 projkit-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:36:01.257456 projkit-0.1.2/projkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 12:35:50.000000 projkit-0.1.2/projkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-08-07 12:35:50.000000 projkit-0.1.2/projkit/camops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-08-07 12:35:50.000000 projkit-0.1.2/projkit/imutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-07 12:35:50.000000 projkit-0.1.2/projkit/pyutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:36:01.257456 projkit-0.1.2/projkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-07 12:36:01.000000 projkit-0.1.2/projkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-07 12:36:01.000000 projkit-0.1.2/projkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:36:01.000000 projkit-0.1.2/projkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 12:36:01.000000 projkit-0.1.2/projkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 12:36:01.000000 projkit-0.1.2/projkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 12:36:01.261457 projkit-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-07 12:35:50.000000 projkit-0.1.2/setup.py
```

### Comparing `projkit-0.1.0/LICENSE` & `projkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `projkit-0.1.0/PKG-INFO` & `projkit-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: projkit
-Version: 0.1.0
+Version: 0.1.2
 Summary: Library designed to simplify camera projection tasks and calculations, particularly when working with image predictions and 3D point cloud data. This library provides functions to effectively incorporate point cloud data with image predictions.
 Home-page: https://github.com/fuzailpalnak/projkit
 Author: Fuzail Palnak
 Author-email: fuzailpalnak@gmail.com
 Keywords: Camera Projections,3d Projections,2d projections,point cloud
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # projkit
 
 Welcome to **projkit**, a Python library designed to simplify camera projection tasks and calculations,
 particularly when working with image predictions and 3D point cloud data. 
 This library provides functions to effectively incorporate point cloud data with image predictions.
 
+## Installation
+
+```sh
+pip install projkit
+```
 
 ## Features
 
 - **Camera Projection to Image Coordinates**: Easily project point cloud data onto image coordinates using provided camera parameters.
   
   ```python
   from projkit.camops import project_in_2d_with_K_R_t_dist_coeff
```

### Comparing `projkit-0.1.0/README.md` & `projkit-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # projkit
 
 Welcome to **projkit**, a Python library designed to simplify camera projection tasks and calculations,
 particularly when working with image predictions and 3D point cloud data. 
 This library provides functions to effectively incorporate point cloud data with image predictions.
 
+## Installation
+
+```sh
+pip install projkit
+```
 
 ## Features
 
 - **Camera Projection to Image Coordinates**: Easily project point cloud data onto image coordinates using provided camera parameters.
   
   ```python
   from projkit.camops import project_in_2d_with_K_R_t_dist_coeff
```

### Comparing `projkit-0.1.0/projkit/camops.py` & `projkit-0.1.2/projkit/camops.py`

 * *Files identical despite different names*

### Comparing `projkit-0.1.0/projkit/imutils.py` & `projkit-0.1.2/projkit/imutils.py`

 * *Files identical despite different names*

### Comparing `projkit-0.1.0/projkit/pyutils.py` & `projkit-0.1.2/projkit/pyutils.py`

 * *Files identical despite different names*

### Comparing `projkit-0.1.0/projkit.egg-info/PKG-INFO` & `projkit-0.1.2/projkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: projkit
-Version: 0.1.0
+Version: 0.1.2
 Summary: Library designed to simplify camera projection tasks and calculations, particularly when working with image predictions and 3D point cloud data. This library provides functions to effectively incorporate point cloud data with image predictions.
 Home-page: https://github.com/fuzailpalnak/projkit
 Author: Fuzail Palnak
 Author-email: fuzailpalnak@gmail.com
 Keywords: Camera Projections,3d Projections,2d projections,point cloud
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # projkit
 
 Welcome to **projkit**, a Python library designed to simplify camera projection tasks and calculations,
 particularly when working with image predictions and 3D point cloud data. 
 This library provides functions to effectively incorporate point cloud data with image predictions.
 
+## Installation
+
+```sh
+pip install projkit
+```
 
 ## Features
 
 - **Camera Projection to Image Coordinates**: Easily project point cloud data onto image coordinates using provided camera parameters.
   
   ```python
   from projkit.camops import project_in_2d_with_K_R_t_dist_coeff
```

### Comparing `projkit-0.1.0/setup.py` & `projkit-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,33 +10,33 @@
         install_requires = f.read().split("\n")
 except FileNotFoundError:
     install_requires = []
 
 
 setup(
     name="projkit",
-    version="0.1.0",
+    version="0.1.2",
     author="Fuzail Palnak",
     author_email="fuzailpalnak@gmail.com",
     url="https://github.com/fuzailpalnak/projkit",
     description="Library designed to simplify camera projection tasks and calculations, "
                 "particularly when working with image predictions and 3D point cloud data."
                 " This library provides functions to effectively incorporate point cloud data with image predictions.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    python_requires=">=3.8",
+    python_requires=">=3.6",
     install_requires=install_requires,
     keywords=[
         "Camera Projections",
         "3d Projections",
         "2d projections",
         "point cloud",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
     ],
-)
+)
```

