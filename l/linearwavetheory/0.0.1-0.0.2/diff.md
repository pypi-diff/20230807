# Comparing `tmp/linearwavetheory-0.0.1.tar.gz` & `tmp/linearwavetheory-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linearwavetheory-0.0.1.tar", last modified: Sun Aug  6 03:52:47 2023, max compression
+gzip compressed data, was "linearwavetheory-0.0.2.tar", last modified: Mon Aug  7 03:08:36 2023, max compression
```

## Comparing `linearwavetheory-0.0.1.tar` & `linearwavetheory-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-06 03:52:47.302376 linearwavetheory-0.0.1/
--rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-06 02:37:22.000000 linearwavetheory-0.0.1/LICENSE
--rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-06 03:52:47.302153 linearwavetheory-0.0.1/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)      532 2023-08-06 03:43:57.000000 linearwavetheory-0.0.1/README.md
--rw-r--r--   0 pietersmit   (502) staff       (20)       38 2023-08-06 03:52:47.302454 linearwavetheory-0.0.1/setup.cfg
--rw-r--r--   0 pietersmit   (502) staff       (20)     1055 2023-08-06 03:43:57.000000 linearwavetheory-0.0.1/setup.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-06 03:52:47.298411 linearwavetheory-0.0.1/src/
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-06 03:52:47.300382 linearwavetheory-0.0.1/src/linearwavetheory/
--rw-r--r--   0 pietersmit   (502) staff       (20)      249 2023-08-06 03:43:57.000000 linearwavetheory-0.0.1/src/linearwavetheory/__init__.py
--rw-r--r--   0 pietersmit   (502) staff       (20)      260 2023-08-06 03:43:57.000000 linearwavetheory-0.0.1/src/linearwavetheory/_constants.py
--rw-r--r--   0 pietersmit   (502) staff       (20)      381 2023-07-18 23:20:42.000000 linearwavetheory-0.0.1/src/linearwavetheory/_numba_settings.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     2265 2023-08-06 03:43:57.000000 linearwavetheory-0.0.1/src/linearwavetheory/_tools.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    31708 2023-08-06 03:43:58.000000 linearwavetheory-0.0.1/src/linearwavetheory/dispersion.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-06 03:52:47.301808 linearwavetheory-0.0.1/src/linearwavetheory.egg-info/
--rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-06 03:52:47.000000 linearwavetheory-0.0.1/src/linearwavetheory.egg-info/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)      419 2023-08-06 03:52:47.000000 linearwavetheory-0.0.1/src/linearwavetheory.egg-info/SOURCES.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)        1 2023-08-06 03:52:47.000000 linearwavetheory-0.0.1/src/linearwavetheory.egg-info/dependency_links.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)       12 2023-08-06 03:52:47.000000 linearwavetheory-0.0.1/src/linearwavetheory.egg-info/requires.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)       17 2023-08-06 03:52:47.000000 linearwavetheory-0.0.1/src/linearwavetheory.egg-info/top_level.txt
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 03:08:36.253462 linearwavetheory-0.0.2/
+-rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-06 02:37:22.000000 linearwavetheory-0.0.2/LICENSE
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-07 03:08:36.253233 linearwavetheory-0.0.2/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)      532 2023-08-06 03:43:57.000000 linearwavetheory-0.0.2/README.md
+-rw-r--r--   0 pietersmit   (502) staff       (20)       38 2023-08-07 03:08:36.253548 linearwavetheory-0.0.2/setup.cfg
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1055 2023-08-07 03:08:22.000000 linearwavetheory-0.0.2/setup.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 03:08:36.249368 linearwavetheory-0.0.2/src/
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 03:08:36.251500 linearwavetheory-0.0.2/src/linearwavetheory/
+-rw-r--r--   0 pietersmit   (502) staff       (20)      249 2023-08-06 03:43:57.000000 linearwavetheory-0.0.2/src/linearwavetheory/__init__.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)      260 2023-08-06 03:43:57.000000 linearwavetheory-0.0.2/src/linearwavetheory/_constants.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)      381 2023-07-18 23:20:42.000000 linearwavetheory-0.0.2/src/linearwavetheory/_numba_settings.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     2195 2023-08-07 03:01:04.000000 linearwavetheory-0.0.2/src/linearwavetheory/_tools.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    38239 2023-08-07 03:08:05.000000 linearwavetheory-0.0.2/src/linearwavetheory/dispersion.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 03:08:36.252892 linearwavetheory-0.0.2/src/linearwavetheory.egg-info/
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-07 03:08:36.000000 linearwavetheory-0.0.2/src/linearwavetheory.egg-info/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)      419 2023-08-07 03:08:36.000000 linearwavetheory-0.0.2/src/linearwavetheory.egg-info/SOURCES.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)        1 2023-08-07 03:08:36.000000 linearwavetheory-0.0.2/src/linearwavetheory.egg-info/dependency_links.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)       12 2023-08-07 03:08:36.000000 linearwavetheory-0.0.2/src/linearwavetheory.egg-info/requires.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)       17 2023-08-07 03:08:36.000000 linearwavetheory-0.0.2/src/linearwavetheory.egg-info/top_level.txt
```

### Comparing `linearwavetheory-0.0.1/LICENSE` & `linearwavetheory-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.1/PKG-INFO` & `linearwavetheory-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearwavetheory
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package that implements linear wave theory for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/linearwavetheory.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linearwavetheory-0.0.1/README.md` & `linearwavetheory-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.1/setup.py` & `linearwavetheory-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme_contents = file.read()
 
 setuptools.setup(
     name="linearwavetheory",
-    version="0.0.1",
+    version="0.0.2",
     license="Apache 2 License",
     install_requires=[
         "numpy",
         "numba",
     ],
     description="Python package that implements linear wave theory for ocean surface gravity waves",
     long_description=readme_contents,
```

### Comparing `linearwavetheory-0.0.1/src/linearwavetheory/_tools.py` & `linearwavetheory-0.0.2/src/linearwavetheory/_tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,16 +47,14 @@
 
     Special cases:
     - If the input is None, return an array of zeros with the specified number of rows.
     - If no target rows are specified (=0), the number of rows is determined by the input array.
 
     """
     target_cols = 2
-    if x is None:
-        return np.zeros((target_rows, target_cols))
 
     x = atleast_2d(x)
     if target_rows == 0:
         target_rows = x.shape[0]
 
     out = np.zeros((target_rows, target_cols))
```

### Comparing `linearwavetheory-0.0.1/src/linearwavetheory/dispersion.py` & `linearwavetheory-0.0.2/src/linearwavetheory/dispersion.py`

 * *Files 14% similar despite different names*

```diff
@@ -478,15 +478,15 @@
         w[j] is calculated for k[j] and d[j].
 
     :param kinematic_surface_tension: kinematic surface tension in m^3/s^2. Per default set to 0.0728 N/m (water at 20C)
         divided by density of seawater (1025 kg/m^3).
 
     :param grav: gravitational acceleration in m/s^2. Default is 9.81 m/s^2.
 
-    :return: The intrinsic angular frequency as a 1 dimensional numpy array.
+    :return: The intrinsic phase speed as a 1 dimensional numpy array.
     """
     wavenumber_magnitude = atleast_1d(wavenumber_magnitude)
     _intrinsic_phase_speed = np.zeros(wavenumber_magnitude.shape)
 
     if grav <= 0:
         raise ValueError("Gravitational acceleration must be positive")
 
@@ -569,15 +569,17 @@
 
     intrinsic_wavenumber_vector = _to_2d_array(intrinsic_wavenumber_vector)
     relative_velocity = _to_2d_array(
         ambient_current_velocity, target_rows=intrinsic_wavenumber_vector.shape[0]
     ) - _to_2d_array(
         observer_velocity, target_rows=intrinsic_wavenumber_vector.shape[0]
     )
-    wavenumber_magnitude = np.linalg.norm(intrinsic_wavenumber_vector, axis=-1)
+    wavenumber_magnitude = np.sqrt(
+        np.sum(intrinsic_wavenumber_vector * intrinsic_wavenumber_vector, axis=-1)
+    )
     _intrinsic_phase_speed = intrinsic_phase_speed(
         wavenumber_magnitude,
         depth,
         kinematic_surface_tension=kinematic_surface_tension,
         grav=grav,
     )
 
@@ -601,16 +603,16 @@
     return _encounter_phase_velocity
 
 
 @jit(**numba_default)
 def encounter_phase_speed(
     intrinsic_wavenumber_vector,
     depth=np.inf,
-    ambient_current_velocity=None,
-    observer_velocity=None,
+    ambient_current_velocity=(0.0, 0.0),
+    observer_velocity=(0.0, 0.0),
     kinematic_surface_tension: float = KINEMATIC_SURFACE_TENSION,
     grav=GRAV,
 ) -> np.ndarray:
     """
     The phase SPEED of a wave moving through an ambient current field with velocity ambient_current_velocity
     (defauly 0) as observed by an observer moving with velocity observer_velocity (default 0) relative to the
     earth reference frame.
@@ -640,128 +642,235 @@
     :param kinematic_surface_tension: Kinematic surface tension parameter. Per default set to 0.0728 N/m (water at 20C)
     divided by density of seawater (1025 kg/m^3).
 
     :param grav: Gravitational acceleration (m/s^2). Default 9.81 m/s^2.
 
     :return: A 1D numpy array with shape (N,) where N is the number of wavenumbers.
     """
-    c = encounter_phase_velocity(
+    _encounter_phase_velocity = encounter_phase_velocity(
         intrinsic_wavenumber_vector,
         depth,
         ambient_current_velocity=ambient_current_velocity,
         observer_velocity=observer_velocity,
         kinematic_surface_tension=kinematic_surface_tension,
         grav=grav,
     )
-    return np.linalg.norm(c, axis=-1)
+    return np.sqrt(
+        np.sum(_encounter_phase_velocity * _encounter_phase_velocity, axis=-1)
+    )
 
 
 @jit(**numba_default)
 def intrinsic_group_speed(
     wavenumber_magnitude: Union[float, np.ndarray],
     depth: Union[float, np.ndarray] = np.inf,
     kinematic_surface_tension: float = KINEMATIC_SURFACE_TENSION,
     grav=GRAV,
 ) -> np.ndarray:
     """
-    :param wavenumber: Wavenumber (rad/m)
-    :param depth: Depth (m)
-    :param grav: Gravitational acceleration (m/s^2)
-    :return:
-    """
-    wavenumber_magnitude = np.atleast_1d(wavenumber_magnitude)
-
-    kd = wavenumber_magnitude * depth
-    intrinsic_angular_frequency = np.sqrt(grav * wavenumber_magnitude * np.tanh(kd))
-    cg = (
-        (1 / 2 + kd / np.sinh(2 * kd))
-        * intrinsic_angular_frequency
-        / wavenumber_magnitude
-    )
+    The intrinsic group speed for linear gravity-capillary waves. I.e.
+
+        cg = dw / dk
+
+    NOTE:
+        - if the wavenumber magnitude is zero, the group speed is defined as it's limiting value as k-> 0
+            (the shallow water group speed).
+        - if the depth is smaller or equal to zero, the group speed is undefined and np.nan is returned.
+        - if the wavenumber magnitude is negative, we return an error (undefined).
+
+    :param  wavenumber_magnitude: The wavenumber_magnitude. Can be a scalar or a 1 dimensional numpy array.
+
+    :param depth: depth in meters. Can be a scalar or a 1 dimensional numpy array. If a 1d array is provided, it must
+        have the same length as the wavenumber_magnitude array, and calculation is performed pairwise. I.e.
+        w[j] is calculated for k[j] and d[j].
+
+    :param kinematic_surface_tension: kinematic surface tension in m^3/s^2. Per default set to 0.0728 N/m (water at 20C)
+        divided by density of seawater (1025 kg/m^3).
+
+    :param grav: gravitational acceleration in m/s^2. Default is 9.81 m/s^2.
+
+    :return: The intrinsic group speed as a 1 dimensional numpy array.
+    """
+    wavenumber_magnitude = atleast_1d(wavenumber_magnitude)
+    _intrinsic_group_speed = np.zeros(wavenumber_magnitude.shape)
+
+    if grav <= 0:
+        raise ValueError("Gravitational acceleration must be positive")
+
+    if kinematic_surface_tension <= 0:
+        raise ValueError("Kinematic surface tension must be positive")
+
+    depth = atleast_1d(depth)
+    if len(depth) == 1:
+        depth = np.full_like(wavenumber_magnitude, depth[0], dtype=depth.dtype)
+
+    if not len(wavenumber_magnitude) == len(depth):
+        raise ValueError("wavenumber_magnitude and depth must have the same length.")
 
-    if not (kinematic_surface_tension > 0.0):
-        return cg
+    for jj in range(0, len(wavenumber_magnitude)):
+        if wavenumber_magnitude[jj] < 0:
+            raise ValueError("Negative wavenumber encountered")
+
+        if depth[jj] <= 0:
+            _intrinsic_group_speed[jj] = np.nan
+            continue
+
+        if wavenumber_magnitude[jj] == 0:
+            _intrinsic_group_speed[jj] = np.sqrt(grav * depth[jj])
+            continue
 
-    else:
         surface_tension_term = np.sqrt(
-            1 + kinematic_surface_tension * wavenumber_magnitude**2 / grav
+            1 + kinematic_surface_tension * wavenumber_magnitude[jj] ** 2 / grav
         )
-
-        return (
-            cg * surface_tension_term
-            + intrinsic_angular_frequency
-            * wavenumber_magnitude
+        kd = wavenumber_magnitude[jj] * depth[jj]
+        n = 1 / 2 + kd / np.sinh(2 * kd)
+        c = np.sqrt(grav / wavenumber_magnitude[jj] * np.tanh(kd))
+        w = wavenumber_magnitude[jj] * c
+
+        _intrinsic_group_speed[jj] = (
+            n * c * surface_tension_term
+            + w
+            * wavenumber_magnitude[jj]
             * kinematic_surface_tension
             / grav
             / surface_tension_term
         )
+    return _intrinsic_group_speed
 
 
 @jit(**numba_default)
 def encounter_group_velocity(
-    wavenumber,
+    intrinsic_wavenumber_vector,
     depth=np.inf,
-    ambient_current_velocity=None,
-    observer_velocity=None,
+    ambient_current_velocity=(0.0, 0.0),
+    observer_velocity=(0.0, 0.0),
     kinematic_surface_tension: float = KINEMATIC_SURFACE_TENSION,
     grav=GRAV,
 ) -> np.ndarray:
     """
-    :param wavenumber: Wavenumber (rad/m)
-    :param depth: Depth (m)
-    :param grav: Gravitational acceleration (m/s^2)
-    :return:
-    """
-    wavenumber = _to_2d_array(wavenumber)
-    ambient_current_velocity = _to_2d_array(
-        ambient_current_velocity, target_rows=wavenumber.shape[0]
-    )
-    observer_velocity = _to_2d_array(observer_velocity, target_rows=wavenumber.shape[0])
-    relative_velocity = ambient_current_velocity - observer_velocity
+    The group VELOCITY of a wave moving through an ambient current field with velocity ambient_current_velocity
+    (defauly 0) as observed by an observer moving with velocity observer_velocity (default 0) relative to the
+    earth reference frame.
+
+    We calculate the result as a function of the intrinsic wavenumber, with magnitude and direction such that the
+    wavenumber points in the direction of wave propagation in the intrinsic frame of reference. Depending on the
+    magnitude of the ambient current and the wavenumber, this wavenumber may differ in sign -
+    though magnitude is preserved for all observers.
+
+    Input
+    -----
+    :param intrinsic_wavenumber_vector: Wavenumber (rad/m) in the intrinsic frame of reference of the wave specified as a 1D
+    numpy array (kx,ky), or as a 2D numpy array with shape (N,2) where N is the number of wavenumbers.
+
+    :param depth: Depth (m). May be a scalar or a numpy array. If a numpy array, must have the same number of rows as
+    the number of wavenumbers in intrinsic_wavenumber.
+
+    :param ambient_current_velocity: current (m/s) in the earth reference frame specified as a 1D numpy array (u,v),
+    which will be broadcast to an array of the same shape as the wavenumber array, or as a 2D numpy array with the same
+    shape as the wavenumber array, in which case the j^th row will be used for the j^th wavenumber. Default (0,0).
+
+    :param observer_velocity: velocity (m/s) of the observer in the earth reference frame specified as a 1D numpy array
+    (u,v), which will be broadcast to an array of the same shape as the wavenumber array, or as a 2D numpy array with
+    the same shape as the wavenumber array, in which case the j^th row will be used for the j^th wavenumber.
+    Default (0,0).
+
+    :param kinematic_surface_tension: Kinematic surface tension parameter. Per default set to 0.0728 N/m (water at 20C)
+    divided by density of seawater (1025 kg/m^3).
+
+    :param grav: Gravitational acceleration (m/s^2). Default 9.81 m/s^2.
+
+    :return: A 2D numpy array with shape (N,2) where N is the number of wavenumbers.
+    """
 
-    wavenumber_magnitude = np.linalg.norm(wavenumber, axis=-1)
-    cg_int = intrinsic_group_speed(
+    intrinsic_wavenumber_vector = _to_2d_array(intrinsic_wavenumber_vector)
+    relative_velocity = _to_2d_array(
+        ambient_current_velocity, target_rows=intrinsic_wavenumber_vector.shape[0]
+    ) - _to_2d_array(
+        observer_velocity, target_rows=intrinsic_wavenumber_vector.shape[0]
+    )
+    wavenumber_magnitude = np.sqrt(
+        np.sum(intrinsic_wavenumber_vector * intrinsic_wavenumber_vector, axis=-1)
+    )
+    _intrinsic_group_speed = intrinsic_group_speed(
         wavenumber_magnitude,
         depth,
         kinematic_surface_tension=kinematic_surface_tension,
         grav=grav,
     )
 
-    cg = np.zeros(wavenumber.shape)
+    _encounter_group_velocity = np.zeros(intrinsic_wavenumber_vector.shape)
     for jj in range(0, len(wavenumber_magnitude)):
         if wavenumber_magnitude[jj] > 0:
-            cg[jj, 0] = (
-                cg_int[jj] * wavenumber[jj, 0] / wavenumber_magnitude[jj]
+            _encounter_group_velocity[jj, 0] = (
+                _intrinsic_group_speed[jj]
+                * intrinsic_wavenumber_vector[jj, 0]
+                / wavenumber_magnitude[jj]
                 + relative_velocity[jj, 0]
             )
-            cg[jj, 1] = (
-                cg_int[jj] * wavenumber[jj, 1] / wavenumber_magnitude[jj]
+
+            _encounter_group_velocity[jj, 1] = (
+                _intrinsic_group_speed[jj]
+                * intrinsic_wavenumber_vector[jj, 1]
+                / wavenumber_magnitude[jj]
                 + relative_velocity[jj, 1]
             )
-
-    return cg
+        else:
+            # group velocity is undefined for zero wavenumber.
+            _encounter_group_velocity[jj, 0] = np.nan
+            _encounter_group_velocity[jj, 1] = np.nan
+    return _encounter_group_velocity
 
 
 @jit(**numba_default)
 def encounter_group_speed(
     wavenumber,
     depth=np.inf,
-    ambient_current_velocity=None,
-    relative_velocity=None,
+    ambient_current_velocity=(0.0, 0.0),
+    relative_velocity=(0.0, 0.0),
     kinematic_surface_tension: float = KINEMATIC_SURFACE_TENSION,
     grav=GRAV,
 ) -> np.ndarray:
     """
-    :param wavenumber: Wavenumber (rad/m)
-    :param depth: Depth (m)
-    :param grav: Gravitational acceleration (m/s^2)
-    :return:
+    The group SPEED of a wave moving through an ambient current field with velocity ambient_current_velocity
+    (defauly 0) as observed by an observer moving with velocity observer_velocity (default 0) relative to the
+    earth reference frame.
+
+    We calculate the result as a function of the intrinsic wavenumber, with magnitude and direction such that the
+    wavenumber points in the direction of wave propagation in the intrinsic frame of reference. Depending on the
+    magnitude of the ambient current and the wavenumber, this wavenumber may differ in sign -
+    though magnitude is preserved for all observers.
+
+    Input
+    -----
+    :param intrinsic_wavenumber: Wavenumber (rad/m) in the intrinsic frame of reference of the wave specified as a 1D
+    numpy array (kx,ky), or as a 2D numpy array with shape (N,2) where N is the number of wavenumbers.
+
+    :param depth: Depth (m). May be a scalar or a numpy array. If a numpy array, must have the same number of rows as
+    the number of wavenumbers in intrinsic_wavenumber.
+
+    :param ambient_current_velocity: current (m/s) in the earth reference frame specified as a 1D numpy array (u,v),
+    which will be broadcast to an array of the same shape as the wavenumber array, or as a 2D numpy array with the same
+    shape as the wavenumber array, in which case the j^th row will be used for the j^th wavenumber. Default (0,0).
+
+    :param observer_velocity: velocity (m/s) of the observer in the earth reference frame specified as a 1D numpy array
+    (u,v), which will be broadcast to an array of the same shape as the wavenumber array, or as a 2D numpy array with
+    the same shape as the wavenumber array, in which case the j^th row will be used for the j^th wavenumber.
+    Default (0,0).
+
+    :param kinematic_surface_tension: Kinematic surface tension parameter. Per default set to 0.0728 N/m (water at 20C)
+    divided by density of seawater (1025 kg/m^3).
+
+    :param grav: Gravitational acceleration (m/s^2). Default 9.81 m/s^2.
+
+    :return: A 1D numpy array with shape (N,) where N is the number of wavenumbers.
     """
-    cg = encounter_group_velocity(
+    _encounter_group_velocity = encounter_group_velocity(
         wavenumber,
         depth,
         ambient_current_velocity,
         relative_velocity,
         kinematic_surface_tension=kinematic_surface_tension,
         grav=grav,
     )
-    return np.linalg.norm(cg, axis=-1)
+    return np.sqrt(
+        np.sum(_encounter_group_velocity * _encounter_group_velocity, axis=-1)
+    )
```

### Comparing `linearwavetheory-0.0.1/src/linearwavetheory.egg-info/PKG-INFO` & `linearwavetheory-0.0.2/src/linearwavetheory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearwavetheory
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package that implements linear wave theory for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/linearwavetheory.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

