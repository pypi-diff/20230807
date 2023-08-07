# Comparing `tmp/rsplan-1.0.5.tar.gz` & `tmp/rsplan-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsplan-1.0.5.tar", last modified: Mon Jul 31 17:37:07 2023, max compression
+gzip compressed data, was "rsplan-1.0.6.tar", last modified: Mon Aug  7 19:50:27 2023, max compression
```

## Comparing `rsplan-1.0.5.tar` & `rsplan-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-31 17:37:07.410989 rsplan-1.0.5/
--rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.5/LICENSE
--rw-rw-r--   0 built     (1000) built     (1000)     5740 2023-07-31 17:37:07.410989 rsplan-1.0.5/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)     4083 2023-07-25 20:27:37.000000 rsplan-1.0.5/README.md
--rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-07-31 17:37:00.000000 rsplan-1.0.5/pyproject.toml
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-31 17:37:07.410989 rsplan-1.0.5/rsplan/
--rw-rw-r--   0 built     (1000) built     (1000)      113 2023-07-31 17:32:15.000000 rsplan-1.0.5/rsplan/__init__.py
--rw-rw-r--   0 built     (1000) built     (1000)    28387 2023-07-25 20:19:49.000000 rsplan-1.0.5/rsplan/curves.py
--rw-rw-r--   0 built     (1000) built     (1000)     2650 2023-07-31 17:34:37.000000 rsplan-1.0.5/rsplan/demo.py
--rw-rw-r--   0 built     (1000) built     (1000)     2981 2023-07-25 02:02:07.000000 rsplan-1.0.5/rsplan/helpers.py
--rw-rw-r--   0 built     (1000) built     (1000)     6597 2023-07-25 20:19:52.000000 rsplan-1.0.5/rsplan/planner.py
--rw-rw-r--   0 built     (1000) built     (1000)    12043 2023-07-25 01:56:11.000000 rsplan-1.0.5/rsplan/primitives.py
--rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-25 19:46:23.000000 rsplan-1.0.5/rsplan/py.typed
--rw-rw-r--   0 built     (1000) built     (1000)     5121 2023-07-24 00:19:18.000000 rsplan-1.0.5/rsplan/unit_tests.py
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-31 17:37:07.410989 rsplan-1.0.5/rsplan.egg-info/
--rw-rw-r--   0 built     (1000) built     (1000)     5740 2023-07-31 17:37:07.000000 rsplan-1.0.5/rsplan.egg-info/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)      335 2023-07-31 17:37:07.000000 rsplan-1.0.5/rsplan.egg-info/SOURCES.txt
--rw-rw-r--   0 built     (1000) built     (1000)        1 2023-07-31 17:37:07.000000 rsplan-1.0.5/rsplan.egg-info/dependency_links.txt
--rw-rw-r--   0 built     (1000) built     (1000)       39 2023-07-31 17:37:07.000000 rsplan-1.0.5/rsplan.egg-info/requires.txt
--rw-rw-r--   0 built     (1000) built     (1000)        7 2023-07-31 17:37:07.000000 rsplan-1.0.5/rsplan.egg-info/top_level.txt
--rw-rw-r--   0 built     (1000) built     (1000)       38 2023-07-31 17:37:07.410989 rsplan-1.0.5/setup.cfg
--rw-rw-r--   0 built     (1000) built     (1000)      686 2023-07-31 17:36:44.000000 rsplan-1.0.5/setup.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-08-07 19:50:27.593753 rsplan-1.0.6/
+-rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.6/LICENSE
+-rw-rw-r--   0 built     (1000) built     (1000)     5740 2023-08-07 19:50:27.589752 rsplan-1.0.6/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)     4083 2023-07-25 20:27:37.000000 rsplan-1.0.6/README.md
+-rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-08-07 19:50:18.000000 rsplan-1.0.6/pyproject.toml
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-08-07 19:50:27.589752 rsplan-1.0.6/rsplan/
+-rw-rw-r--   0 built     (1000) built     (1000)       73 2023-08-07 04:56:29.000000 rsplan-1.0.6/rsplan/__init__.py
+-rw-rw-r--   0 built     (1000) built     (1000)    28387 2023-07-25 20:19:49.000000 rsplan-1.0.6/rsplan/curves.py
+-rw-rw-r--   0 built     (1000) built     (1000)     2552 2023-08-07 04:58:52.000000 rsplan-1.0.6/rsplan/demo.py
+-rw-rw-r--   0 built     (1000) built     (1000)     2981 2023-07-25 02:02:07.000000 rsplan-1.0.6/rsplan/helpers.py
+-rw-rw-r--   0 built     (1000) built     (1000)     6597 2023-07-25 20:19:52.000000 rsplan-1.0.6/rsplan/planner.py
+-rw-rw-r--   0 built     (1000) built     (1000)    12043 2023-07-25 01:56:11.000000 rsplan-1.0.6/rsplan/primitives.py
+-rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-25 19:46:23.000000 rsplan-1.0.6/rsplan/py.typed
+-rw-rw-r--   0 built     (1000) built     (1000)     5121 2023-07-24 00:19:18.000000 rsplan-1.0.6/rsplan/unit_tests.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-08-07 19:50:27.589752 rsplan-1.0.6/rsplan.egg-info/
+-rw-rw-r--   0 built     (1000) built     (1000)     5740 2023-08-07 19:50:27.000000 rsplan-1.0.6/rsplan.egg-info/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)      335 2023-08-07 19:50:27.000000 rsplan-1.0.6/rsplan.egg-info/SOURCES.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        1 2023-08-07 19:50:27.000000 rsplan-1.0.6/rsplan.egg-info/dependency_links.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       39 2023-08-07 19:50:27.000000 rsplan-1.0.6/rsplan.egg-info/requires.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        7 2023-08-07 19:50:27.000000 rsplan-1.0.6/rsplan.egg-info/top_level.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       38 2023-08-07 19:50:27.593753 rsplan-1.0.6/setup.cfg
+-rw-rw-r--   0 built     (1000) built     (1000)      686 2023-08-07 19:50:11.000000 rsplan-1.0.6/setup.py
```

### Comparing `rsplan-1.0.5/LICENSE` & `rsplan-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.5/PKG-INFO` & `rsplan-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.5
+Version: 1.0.6
 Summary: Reeds-Shepp algorithm implementation in Python
 Home-page: https://github.com/builtrobotics/rs
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
```

### Comparing `rsplan-1.0.5/README.md` & `rsplan-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.5/pyproject.toml` & `rsplan-1.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rsplan"
-version = "1.0.5"
+version = "1.0.6"
 description = "Reeds-Shepp algorithm implementation in Python"
 readme = "README.md"
 authors = [{ name = "Built Robotics", email = "tarakapoor9@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rsplan-1.0.5/rsplan/curves.py` & `rsplan-1.0.6/rsplan/curves.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.5/rsplan/demo.py` & `rsplan-1.0.6/rsplan/demo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from typing import List, Tuple
 
 import matplotlib.pyplot as plt  # type: ignore[import]
 import numpy as np
 
-# from rsplan import planner, primitives
 import rsplan
 
 # List of path end poses to visualize Reeds-Shepp paths for with matplotlib.
 # Format: (end x, end y, end yaw, turn radius, runway length)
 _END_POSES: List[Tuple[float, float, float, int, float]] = [
     (5, 6, np.pi, 1, 0),
     (15, 3, np.pi / 2.0, 2, 6),
@@ -43,15 +42,15 @@
         length * np.sin(yaw),
         head_width=width,
         head_length=width,
     )
     plt.plot(x, y, marker="s", label=label)
 
 
-def _viz_path(rs_path: rsplan.Path, path_num: int) -> None: #primitives.Path, path_num: int) -> None:
+def _viz_path(rs_path: rsplan.Path, path_num: int) -> None:
     """Visualizes the given path in the plot."""
     x_coords, y_coords, _ = rs_path.coordinates_tuple()
 
     path_plt = plt.subplot(111)
     path_plt.plot(x_coords, y_coords, label=(f"Path ix: {path_num}"))
 
     # Shrink current axis's height by 10% on the bottom
@@ -79,15 +78,15 @@
         end_coords = _END_POSES[i]
         x, y, yaw, turn_radius, runway_length = end_coords
         step_size = 0.05
 
         _plot_arrow(*start)  # Start arrow same for all paths starting at origin
 
         # Passing in yaw angles in radians
-        rs_path = rsplan.path( #planner.path(
+        rs_path = rsplan.path(
             start, (x, y, yaw), turn_radius, runway_length, step_size
         )
         _viz_path(rs_path, i + 1)
         _plot_arrow(x, y, yaw)  # End of path arrow to show direction
 
     plt.show()
```

### Comparing `rsplan-1.0.5/rsplan/helpers.py` & `rsplan-1.0.6/rsplan/helpers.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.5/rsplan/planner.py` & `rsplan-1.0.6/rsplan/planner.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.5/rsplan/primitives.py` & `rsplan-1.0.6/rsplan/primitives.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.5/rsplan/unit_tests.py` & `rsplan-1.0.6/rsplan/unit_tests.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.5/rsplan.egg-info/PKG-INFO` & `rsplan-1.0.6/rsplan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.5
+Version: 1.0.6
 Summary: Reeds-Shepp algorithm implementation in Python
 Home-page: https://github.com/builtrobotics/rs
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
```

### Comparing `rsplan-1.0.5/setup.py` & `rsplan-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "rsplan",
-    version = "1.0.5",
+    version = "1.0.6",
     author = "Built Robotics",
     author_email = "tarakapoor9@gmail.com",
     description = ("Reeds-Shepp algorithm implementation in Python."),
     license = "MIT",
     keywords = "reeds-shepp path planning",
     url = "https://github.com/builtrobotics/rs",
     packages=['rsplan'],
```

