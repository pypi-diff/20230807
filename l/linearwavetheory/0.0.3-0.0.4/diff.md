# Comparing `tmp/linearwavetheory-0.0.3.tar.gz` & `tmp/linearwavetheory-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linearwavetheory-0.0.3.tar", last modified: Mon Aug  7 03:40:42 2023, max compression
+gzip compressed data, was "linearwavetheory-0.0.4.tar", last modified: Mon Aug  7 18:53:40 2023, max compression
```

## Comparing `linearwavetheory-0.0.3.tar` & `linearwavetheory-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 03:40:42.506393 linearwavetheory-0.0.3/
--rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-06 02:37:22.000000 linearwavetheory-0.0.3/LICENSE
--rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-07 03:40:42.506133 linearwavetheory-0.0.3/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)      532 2023-08-06 03:43:57.000000 linearwavetheory-0.0.3/README.md
--rw-r--r--   0 pietersmit   (502) staff       (20)       38 2023-08-07 03:40:42.506483 linearwavetheory-0.0.3/setup.cfg
--rw-r--r--   0 pietersmit   (502) staff       (20)     1055 2023-08-07 03:40:25.000000 linearwavetheory-0.0.3/setup.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 03:40:42.501707 linearwavetheory-0.0.3/src/
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 03:40:42.503981 linearwavetheory-0.0.3/src/linearwavetheory/
--rw-r--r--   0 pietersmit   (502) staff       (20)      249 2023-08-06 03:43:57.000000 linearwavetheory-0.0.3/src/linearwavetheory/__init__.py
--rw-r--r--   0 pietersmit   (502) staff       (20)      260 2023-08-06 03:43:57.000000 linearwavetheory-0.0.3/src/linearwavetheory/_constants.py
--rw-r--r--   0 pietersmit   (502) staff       (20)      381 2023-07-18 23:20:42.000000 linearwavetheory-0.0.3/src/linearwavetheory/_numba_settings.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     2195 2023-08-07 03:01:04.000000 linearwavetheory-0.0.3/src/linearwavetheory/_tools.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    40107 2023-08-07 03:40:29.000000 linearwavetheory-0.0.3/src/linearwavetheory/dispersion.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 03:40:42.505652 linearwavetheory-0.0.3/src/linearwavetheory.egg-info/
--rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-07 03:40:42.000000 linearwavetheory-0.0.3/src/linearwavetheory.egg-info/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)      419 2023-08-07 03:40:42.000000 linearwavetheory-0.0.3/src/linearwavetheory.egg-info/SOURCES.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)        1 2023-08-07 03:40:42.000000 linearwavetheory-0.0.3/src/linearwavetheory.egg-info/dependency_links.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)       12 2023-08-07 03:40:42.000000 linearwavetheory-0.0.3/src/linearwavetheory.egg-info/requires.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)       17 2023-08-07 03:40:42.000000 linearwavetheory-0.0.3/src/linearwavetheory.egg-info/top_level.txt
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 18:53:40.732535 linearwavetheory-0.0.4/
+-rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-06 02:37:22.000000 linearwavetheory-0.0.4/LICENSE
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-07 18:53:40.732419 linearwavetheory-0.0.4/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)      532 2023-08-06 03:43:57.000000 linearwavetheory-0.0.4/README.md
+-rw-r--r--   0 pietersmit   (502) staff       (20)       38 2023-08-07 18:53:40.732577 linearwavetheory-0.0.4/setup.cfg
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1055 2023-08-07 18:53:29.000000 linearwavetheory-0.0.4/setup.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 18:53:40.730119 linearwavetheory-0.0.4/src/
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 18:53:40.731476 linearwavetheory-0.0.4/src/linearwavetheory/
+-rw-r--r--   0 pietersmit   (502) staff       (20)      249 2023-08-06 03:43:57.000000 linearwavetheory-0.0.4/src/linearwavetheory/__init__.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)      260 2023-08-06 03:43:57.000000 linearwavetheory-0.0.4/src/linearwavetheory/_constants.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)      381 2023-07-18 23:20:42.000000 linearwavetheory-0.0.4/src/linearwavetheory/_numba_settings.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     2195 2023-08-07 03:01:04.000000 linearwavetheory-0.0.4/src/linearwavetheory/_tools.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    39174 2023-08-07 18:53:19.000000 linearwavetheory-0.0.4/src/linearwavetheory/dispersion.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 18:53:40.732244 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-07 18:53:40.000000 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)      419 2023-08-07 18:53:40.000000 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/SOURCES.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)        1 2023-08-07 18:53:40.000000 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/dependency_links.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)       12 2023-08-07 18:53:40.000000 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/requires.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)       17 2023-08-07 18:53:40.000000 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/top_level.txt
```

### Comparing `linearwavetheory-0.0.3/LICENSE` & `linearwavetheory-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.3/PKG-INFO` & `linearwavetheory-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearwavetheory
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package that implements linear wave theory for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/linearwavetheory.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linearwavetheory-0.0.3/README.md` & `linearwavetheory-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.3/setup.py` & `linearwavetheory-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme_contents = file.read()
 
 setuptools.setup(
     name="linearwavetheory",
-    version="0.0.3",
+    version="0.0.4",
     license="Apache 2 License",
     install_requires=[
         "numpy",
         "numba",
     ],
     description="Python package that implements linear wave theory for ocean surface gravity waves",
     long_description=readme_contents,
```

### Comparing `linearwavetheory-0.0.3/src/linearwavetheory/_tools.py` & `linearwavetheory-0.0.4/src/linearwavetheory/_tools.py`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.3/src/linearwavetheory/dispersion.py` & `linearwavetheory-0.0.4/src/linearwavetheory/dispersion.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 Authors: Pieter Bart Smit
 ======================
 
 """
 
 import numpy as np
-from numba import jit
+from numba import jit, vectorize
 from ._tools import atleast_1d, _to_2d_array
 from ._constants import (
     GRAV,
     KINEMATIC_SURFACE_TENSION,
     MAXIMUM_NUMBER_OF_ITERATIONS,
     RELATIVE_TOLERANCE,
     ABSOLUTE_TOLERANCE,
@@ -382,50 +382,47 @@
     :param kinematic_surface_tension: kinematic surface tension in m^3/s^2. Per default set to 0.0728 N/m (water at 20C)
         divided by density of seawater (1025 kg/m^3).
 
     :param grav: gravitational acceleration in m/s^2. Default is 9.81 m/s^2.
 
     :return: The intrinsic angular frequency as a 1 dimensional numpy array.
     """
-    wavenumber_magnitude = atleast_1d(wavenumber_magnitude)
-
-    depth = atleast_1d(depth)
-    if len(depth) == 1:
-        depth = np.full_like(wavenumber_magnitude, depth[0], dtype=depth.dtype)
-
-    if not len(wavenumber_magnitude) == len(depth):
-        raise ValueError("wavenumber_magnitude and depth must have the same length.")
 
     if kinematic_surface_tension < 0:
         raise ValueError("kinematic_surface_tension must be non-negative.")
 
     if grav < 0:
         raise ValueError("grav must be positive.")
 
-    intrinsic_angular_frequency = np.empty_like(wavenumber_magnitude)
-    for jj in range(0, len(wavenumber_magnitude)):
-        if wavenumber_magnitude[jj] == 0:
-            intrinsic_angular_frequency[jj] = 0
-            continue
-
-        if wavenumber_magnitude[jj] < 0:
-            raise ValueError("wavenumber_magnitude must be non-negative.")
-
-        if depth[jj] <= 0:
-            intrinsic_angular_frequency[jj] = np.nan
-            continue
-
-        intrinsic_angular_frequency[jj] = np.sqrt(
-            (
-                grav * wavenumber_magnitude[jj]
-                + kinematic_surface_tension * wavenumber_magnitude[jj] ** 3
-            )
-            * np.tanh(wavenumber_magnitude[jj] * depth[jj])
+    wavenumber_magnitude = atleast_1d(wavenumber_magnitude)
+    if np.any(wavenumber_magnitude < 0.0):
+        raise ValueError("wavenumber_magnitude must be non-negative.")
+
+    return _intrinsic_dispersion_relation_ufunc(
+        wavenumber_magnitude, depth, kinematic_surface_tension, grav
+    )
+
+
+@vectorize()
+def _intrinsic_dispersion_relation_ufunc(
+    wavenumber_magnitude, depth, kinematic_surface_tension, grav
+):
+    if wavenumber_magnitude == 0.0:
+        return 0.0
+
+    if depth <= 0:
+        return np.nan
+
+    return np.sqrt(
+        (
+            grav * wavenumber_magnitude
+            + kinematic_surface_tension * wavenumber_magnitude**3
         )
-    return intrinsic_angular_frequency
+        * np.tanh(wavenumber_magnitude * depth)
+    )
 
 
 @jit(**numba_default)
 def encounter_dispersion_relation(
     intrinsic_wavenumber_vector: np.ndarray,
     depth=np.inf,
     ambient_current_velocity=(0, 0),
@@ -527,50 +524,44 @@
         divided by density of seawater (1025 kg/m^3).
 
     :param grav: gravitational acceleration in m/s^2. Default is 9.81 m/s^2.
 
     :return: The intrinsic phase speed as a 1 dimensional numpy array.
     """
     wavenumber_magnitude = atleast_1d(wavenumber_magnitude)
-    _intrinsic_phase_speed = np.zeros(wavenumber_magnitude.shape)
+    depth = atleast_1d(depth)
 
     if grav <= 0:
         raise ValueError("Gravitational acceleration must be positive")
 
     if kinematic_surface_tension <= 0:
         raise ValueError("Kinematic surface tension must be positive")
 
-    depth = atleast_1d(depth)
-    if len(depth) == 1:
-        depth = np.full_like(wavenumber_magnitude, depth[0], dtype=depth.dtype)
+    if np.any(wavenumber_magnitude < 0):
+        raise ValueError("Wavenumber magnitude must be positive")
 
-    if not len(wavenumber_magnitude) == len(depth):
-        raise ValueError("wavenumber_magnitude and depth must have the same length.")
+    return _intrinsic_phase_speed_ufunc(
+        wavenumber_magnitude, depth, kinematic_surface_tension, grav
+    )
 
-    for jj in range(0, len(wavenumber_magnitude)):
-        if wavenumber_magnitude[jj] < 0:
-            raise ValueError("Negative wavenumber encountered")
 
-        if depth[jj] <= 0:
-            _intrinsic_phase_speed[jj] = np.nan
-            continue
-
-        if wavenumber_magnitude[jj] == 0:
-            _intrinsic_phase_speed[jj] = np.sqrt(grav * depth[jj])
-            continue
-
-        _intrinsic_phase_speed[jj] = np.sqrt(
-            (
-                grav / wavenumber_magnitude[jj]
-                + kinematic_surface_tension * wavenumber_magnitude[jj]
-            )
-            * np.tanh(wavenumber_magnitude[jj] * depth[jj])
-        )
+@vectorize()
+def _intrinsic_phase_speed_ufunc(
+    wavenumber_magnitude, depth, kinematic_surface_tension, grav
+):
+    if depth <= 0:
+        return np.nan
 
-    return _intrinsic_phase_speed
+    if wavenumber_magnitude == 0:
+        return np.sqrt(grav * depth)
+
+    return np.sqrt(
+        (grav / wavenumber_magnitude + kinematic_surface_tension * wavenumber_magnitude)
+        * np.tanh(wavenumber_magnitude * depth)
+    )
 
 
 @jit(**numba_default)
 def encounter_phase_velocity(
     intrinsic_wavenumber_vector: np.ndarray,
     depth: Union[float, np.ndarray] = np.inf,
     ambient_current_velocity=(0.0, 0.0),
@@ -733,57 +724,65 @@
         divided by density of seawater (1025 kg/m^3).
 
     :param grav: gravitational acceleration in m/s^2. Default is 9.81 m/s^2.
 
     :return: The intrinsic group speed as a 1 dimensional numpy array.
     """
     wavenumber_magnitude = atleast_1d(wavenumber_magnitude)
-    _intrinsic_group_speed = np.zeros(wavenumber_magnitude.shape)
+    depth = atleast_1d(depth)
 
     if grav <= 0:
         raise ValueError("Gravitational acceleration must be positive")
 
     if kinematic_surface_tension <= 0:
         raise ValueError("Kinematic surface tension must be positive")
 
-    depth = atleast_1d(depth)
-    if len(depth) == 1:
-        depth = np.full_like(wavenumber_magnitude, depth[0], dtype=depth.dtype)
+    if np.any(wavenumber_magnitude < 0):
+        raise ValueError("Wavenumber magnitude must be positive")
 
-    if not len(wavenumber_magnitude) == len(depth):
-        raise ValueError("wavenumber_magnitude and depth must have the same length.")
+    return _intrinsic_group_speed_ufunc(
+        wavenumber_magnitude, depth, kinematic_surface_tension, grav
+    )
 
-    for jj in range(0, len(wavenumber_magnitude)):
-        if wavenumber_magnitude[jj] < 0:
-            raise ValueError("Negative wavenumber encountered")
 
-        if depth[jj] <= 0:
-            _intrinsic_group_speed[jj] = np.nan
-            continue
-
-        if wavenumber_magnitude[jj] == 0:
-            _intrinsic_group_speed[jj] = np.sqrt(grav * depth[jj])
-            continue
+@vectorize()
+def _intrinsic_group_speed_ufunc(
+    wavenumber_magnitude,
+    depth,
+    kinematic_surface_tension,
+    grav,
+) -> np.ndarray:
+    """
+    The intrinsic group speed for linear gravity-capillary waves. I.e.
 
-        surface_tension_term = np.sqrt(
-            1 + kinematic_surface_tension * wavenumber_magnitude[jj] ** 2 / grav
-        )
-        kd = wavenumber_magnitude[jj] * depth[jj]
-        n = 1 / 2 + kd / np.sinh(2 * kd)
-        c = np.sqrt(grav / wavenumber_magnitude[jj] * np.tanh(kd))
-        w = wavenumber_magnitude[jj] * c
-
-        _intrinsic_group_speed[jj] = (
-            n * c * surface_tension_term
-            + w
-            * wavenumber_magnitude[jj]
-            * kinematic_surface_tension
-            / grav
-            / surface_tension_term
-        )
+        cg = dw / dk
+
+    """
+    if depth <= 0:
+        return np.nan
+
+    if wavenumber_magnitude == 0:
+        return np.sqrt(grav * depth)
+
+    surface_tension_term = np.sqrt(
+        1 + kinematic_surface_tension * wavenumber_magnitude**2 / grav
+    )
+    kd = wavenumber_magnitude * depth
+    n = 1 / 2 + kd / np.sinh(2 * kd)
+    c = np.sqrt(grav / wavenumber_magnitude * np.tanh(kd))
+    w = wavenumber_magnitude * c
+
+    _intrinsic_group_speed = (
+        n * c * surface_tension_term
+        + w
+        * wavenumber_magnitude
+        * kinematic_surface_tension
+        / grav
+        / surface_tension_term
+    )
     return _intrinsic_group_speed
 
 
 @jit(**numba_default)
 def encounter_group_velocity(
     intrinsic_wavenumber_vector,
     depth=np.inf,
```

### Comparing `linearwavetheory-0.0.3/src/linearwavetheory.egg-info/PKG-INFO` & `linearwavetheory-0.0.4/src/linearwavetheory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearwavetheory
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package that implements linear wave theory for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/linearwavetheory.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

