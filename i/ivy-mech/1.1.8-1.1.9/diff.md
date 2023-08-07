# Comparing `tmp/ivy-mech-1.1.8.tar.gz` & `tmp/ivy-mech-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivy-mech-1.1.8.tar", last modified: Wed Dec  1 08:47:53 2021, max compression
+gzip compressed data, was "ivy-mech-1.1.9.tar", last modified: Wed Dec  1 16:06:57 2021, max compression
```

## Comparing `ivy-mech-1.1.8.tar` & `ivy-mech-1.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:47:53.655079 ivy-mech-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11411 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7131 2021-12-01 08:47:53.655079 ivy-mech-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18975 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:47:53.655079 ivy-mech-1.1.8/ivy_mech/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:47:53.655079 ivy-mech-1.1.8/ivy_mech/orientation/
--rw-r--r--   0 runner    (1001) docker     (121)      218 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/orientation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5573 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/orientation/axis_angle.py
--rw-r--r--   0 runner    (1001) docker     (121)    14648 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/orientation/euler_angles.py
--rw-r--r--   0 runner    (1001) docker     (121)    10270 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/orientation/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (121)     9279 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/orientation/rotation_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:47:53.655079 ivy-mech-1.1.8/ivy_mech/pose/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2953 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/pose/axis_angle_pose.py
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/pose/euler_pose.py
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/pose/matrix_pose.py
--rw-r--r--   0 runner    (1001) docker     (121)     3798 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/pose/quaternion_pose.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:47:53.655079 ivy-mech-1.1.8/ivy_mech/position/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/position/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/position/coordinate_conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/ivy_mech/position/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:47:53.655079 ivy-mech-1.1.8/ivy_mech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7131 2021-12-01 08:47:53.000000 ivy-mech-1.1.8/ivy_mech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      676 2021-12-01 08:47:53.000000 ivy-mech-1.1.8/ivy_mech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 08:47:53.000000 ivy-mech-1.1.8/ivy_mech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-01 08:47:53.000000 ivy-mech-1.1.8/ivy_mech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-01 08:47:53.000000 ivy-mech-1.1.8/ivy_mech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-01 08:47:53.655079 ivy-mech-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2207 2021-12-01 08:47:39.000000 ivy-mech-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:06:57.888652 ivy-mech-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11411 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7789 2021-12-01 16:06:57.888652 ivy-mech-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    18951 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:06:57.888652 ivy-mech-1.1.9/ivy_mech/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:06:57.888652 ivy-mech-1.1.9/ivy_mech/orientation/
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/orientation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5573 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/orientation/axis_angle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14648 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/orientation/euler_angles.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10270 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/orientation/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9279 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/orientation/rotation_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:06:57.888652 ivy-mech-1.1.9/ivy_mech/pose/
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2953 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/pose/axis_angle_pose.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2768 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/pose/euler_pose.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3372 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/pose/matrix_pose.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3798 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/pose/quaternion_pose.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:06:57.888652 ivy-mech-1.1.9/ivy_mech/position/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/position/coordinate_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/ivy_mech/position/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:06:57.888652 ivy-mech-1.1.9/ivy_mech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7789 2021-12-01 16:06:57.000000 ivy-mech-1.1.9/ivy_mech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2021-12-01 16:06:57.000000 ivy-mech-1.1.9/ivy_mech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 16:06:57.000000 ivy-mech-1.1.9/ivy_mech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-01 16:06:57.000000 ivy-mech-1.1.9/ivy_mech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-01 16:06:57.000000 ivy-mech-1.1.9/ivy_mech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-01 16:06:57.888652 ivy-mech-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4123 2021-12-01 16:06:35.000000 ivy-mech-1.1.9/setup.py
```

### Comparing `ivy-mech-1.1.8/LICENSE` & `ivy-mech-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ivy-mech-1.1.8/PKG-INFO` & `ivy-mech-1.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: ivy-mech
-Version: 1.1.8
+Version: 1.1.9
 Summary: Mechanics functions with end-to-end support for machine learning developers, written in Ivy
 Home-page: https://ivy-dl.org/mech
 Author: Ivy Team
 Author-email: ivydl.team@gmail.com
 License: Apache 2.0
 Project-URL: Docs, https://ivy-dl.org/mech/
 Project-URL: Source, https://github.com/ivy-dl/mech
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
+.. image:: https://github.com/ivy-dl/mech/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 
 
 **Mechanics functions with end-to-end support for machine learning developers, written in Ivy.**
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/logos/supported/frameworks.png?raw=true
+   :width: 100%
+
 Contents
 --------
 
 * `Overview`_
 * `Run Through`_
 * `Interactive Demos`_
 * `Get Involed`_
@@ -47,14 +51,17 @@
 
 There are a host of derived libraries written in Ivy, in the areas of mechanics, 3D vision, robotics, gym environments,
 neural memory, pre-trained models + implementations, and builder tools with trainers, data loaders and more. Click on
 the icons below to learn more!
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_libraries.png?raw=true
+   :width: 100%
+
 
 
 
 
 
 
 
@@ -215,22 +222,28 @@
 **Target Facing Rotation Matrix**
 
 The first demo uses the method ``ivy_mech.target_facing_rotation_matrix`` to dynamically
 track a moving target plant pot with a camera, as shown below:
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_mech/demo_a.png?raw=true
+   :width: 100%
+
 **Polar to Cartesian Co-ordinates**
 
 The second demo uses the method ``ivy_mech.polar_to_cartesian_coords`` to convert a polar depth image
 acquired from an omni-directional camera into cartesian co-ordinates,
 enabling the surrounding geometry to be represented as a point cloud, for interactive visualization.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_mech/demo_b.png?raw=true
+   :width: 100%
+
 Get Involed
 -----------
 
 We hope the functions in this library are useful to a wide range of machine learning developers.
 However, there are many more areas of mechanics which could be covered by this library.
 
 If there are any particular mechanics functions you feel are missing,
```

### Comparing `ivy-mech-1.1.8/README.rst` & `ivy-mech-1.1.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-.. raw:: html
-
-    <p align="center">
-        <img width="75%" style="display: block;" src='docs/partial_source/logos/logo.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/mech/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 .. raw:: html
 
     <br/>
     <a href="https://pypi.org/project/ivy-mech">
         <img style="float: left; padding-right: 4px; padding-bottom: 4px;" src="https://badge.fury.io/py/ivy-mech.svg">
     </a>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-.. raw:: html
-                     [docs/partial_source/logos/logo.png]
-.. raw:: html
+.. image:: https://github.com/ivy-dl/mech/blob/master/docs/partial_source/
+logos/logo.png?raw=true :width: 100% .. raw:: html
 [https://badge.fury.io/py/ivy-mech.svg] [https://img.shields.io/github/
 workflow/status/ivy-dl/mech/docs?label=docs] [https://img.shields.io/github/
 workflow/status/ivy-dl/mech/nightly-tests?label=tests] [https://img.shields.io/
 discord/799879767196958751?color=blue&label=%20&logo=discord&logoColor=white]
 **Mechanics functions with end-to-end support for machine learning developers,
 written in Ivy.** .. raw:: html
 [https://raw.githubusercontent.com/ivy-dl/ivy-dl.github.io/master/img/
```

### Comparing `ivy-mech-1.1.8/ivy_mech/orientation/axis_angle.py` & `ivy-mech-1.1.9/ivy_mech/orientation/axis_angle.py`

 * *Files identical despite different names*

### Comparing `ivy-mech-1.1.8/ivy_mech/orientation/euler_angles.py` & `ivy-mech-1.1.9/ivy_mech/orientation/euler_angles.py`

 * *Files identical despite different names*

### Comparing `ivy-mech-1.1.8/ivy_mech/orientation/quaternion.py` & `ivy-mech-1.1.9/ivy_mech/orientation/quaternion.py`

 * *Files identical despite different names*

### Comparing `ivy-mech-1.1.8/ivy_mech/orientation/rotation_matrix.py` & `ivy-mech-1.1.9/ivy_mech/orientation/rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `ivy-mech-1.1.8/ivy_mech/pose/axis_angle_pose.py` & `ivy-mech-1.1.9/ivy_mech/pose/axis_angle_pose.py`

 * *Files identical despite different names*

### Comparing `ivy-mech-1.1.8/ivy_mech/pose/euler_pose.py` & `ivy-mech-1.1.9/ivy_mech/pose/euler_pose.py`

 * *Files identical despite different names*

### Comparing `ivy-mech-1.1.8/ivy_mech/pose/matrix_pose.py` & `ivy-mech-1.1.9/ivy_mech/pose/matrix_pose.py`

 * *Files identical despite different names*

### Comparing `ivy-mech-1.1.8/ivy_mech/pose/quaternion_pose.py` & `ivy-mech-1.1.9/ivy_mech/pose/quaternion_pose.py`

 * *Files identical despite different names*

### Comparing `ivy-mech-1.1.8/ivy_mech/position/coordinate_conversions.py` & `ivy-mech-1.1.9/ivy_mech/position/coordinate_conversions.py`

 * *Files identical despite different names*

### Comparing `ivy-mech-1.1.8/ivy_mech/position/transformations.py` & `ivy-mech-1.1.9/ivy_mech/position/transformations.py`

 * *Files identical despite different names*

### Comparing `ivy-mech-1.1.8/ivy_mech.egg-info/PKG-INFO` & `ivy-mech-1.1.9/ivy_mech.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: ivy-mech
-Version: 1.1.8
+Version: 1.1.9
 Summary: Mechanics functions with end-to-end support for machine learning developers, written in Ivy
 Home-page: https://ivy-dl.org/mech
 Author: Ivy Team
 Author-email: ivydl.team@gmail.com
 License: Apache 2.0
 Project-URL: Docs, https://ivy-dl.org/mech/
 Project-URL: Source, https://github.com/ivy-dl/mech
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
+.. image:: https://github.com/ivy-dl/mech/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 
 
 **Mechanics functions with end-to-end support for machine learning developers, written in Ivy.**
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/logos/supported/frameworks.png?raw=true
+   :width: 100%
+
 Contents
 --------
 
 * `Overview`_
 * `Run Through`_
 * `Interactive Demos`_
 * `Get Involed`_
@@ -47,14 +51,17 @@
 
 There are a host of derived libraries written in Ivy, in the areas of mechanics, 3D vision, robotics, gym environments,
 neural memory, pre-trained models + implementations, and builder tools with trainers, data loaders and more. Click on
 the icons below to learn more!
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_libraries.png?raw=true
+   :width: 100%
+
 
 
 
 
 
 
 
@@ -215,22 +222,28 @@
 **Target Facing Rotation Matrix**
 
 The first demo uses the method ``ivy_mech.target_facing_rotation_matrix`` to dynamically
 track a moving target plant pot with a camera, as shown below:
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_mech/demo_a.png?raw=true
+   :width: 100%
+
 **Polar to Cartesian Co-ordinates**
 
 The second demo uses the method ``ivy_mech.polar_to_cartesian_coords`` to convert a polar depth image
 acquired from an omni-directional camera into cartesian co-ordinates,
 enabling the surrounding geometry to be represented as a point cloud, for interactive visualization.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_mech/demo_b.png?raw=true
+   :width: 100%
+
 Get Involed
 -----------
 
 We hope the functions in this library are useful to a wide range of machine learning developers.
 However, there are many more areas of mechanics which could be covered by this library.
 
 If there are any particular mechanics functions you feel are missing,
```

### Comparing `ivy-mech-1.1.8/ivy_mech.egg-info/SOURCES.txt` & `ivy-mech-1.1.9/ivy_mech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

