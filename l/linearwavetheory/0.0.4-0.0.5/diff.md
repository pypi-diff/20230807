# Comparing `tmp/linearwavetheory-0.0.4.tar.gz` & `tmp/linearwavetheory-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linearwavetheory-0.0.4.tar", last modified: Mon Aug  7 18:53:40 2023, max compression
+gzip compressed data, was "linearwavetheory-0.0.5.tar", last modified: Mon Aug  7 19:39:20 2023, max compression
```

## Comparing `linearwavetheory-0.0.4.tar` & `linearwavetheory-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 18:53:40.732535 linearwavetheory-0.0.4/
--rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-06 02:37:22.000000 linearwavetheory-0.0.4/LICENSE
--rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-07 18:53:40.732419 linearwavetheory-0.0.4/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)      532 2023-08-06 03:43:57.000000 linearwavetheory-0.0.4/README.md
--rw-r--r--   0 pietersmit   (502) staff       (20)       38 2023-08-07 18:53:40.732577 linearwavetheory-0.0.4/setup.cfg
--rw-r--r--   0 pietersmit   (502) staff       (20)     1055 2023-08-07 18:53:29.000000 linearwavetheory-0.0.4/setup.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 18:53:40.730119 linearwavetheory-0.0.4/src/
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 18:53:40.731476 linearwavetheory-0.0.4/src/linearwavetheory/
--rw-r--r--   0 pietersmit   (502) staff       (20)      249 2023-08-06 03:43:57.000000 linearwavetheory-0.0.4/src/linearwavetheory/__init__.py
--rw-r--r--   0 pietersmit   (502) staff       (20)      260 2023-08-06 03:43:57.000000 linearwavetheory-0.0.4/src/linearwavetheory/_constants.py
--rw-r--r--   0 pietersmit   (502) staff       (20)      381 2023-07-18 23:20:42.000000 linearwavetheory-0.0.4/src/linearwavetheory/_numba_settings.py
--rw-r--r--   0 pietersmit   (502) staff       (20)     2195 2023-08-07 03:01:04.000000 linearwavetheory-0.0.4/src/linearwavetheory/_tools.py
--rw-r--r--   0 pietersmit   (502) staff       (20)    39174 2023-08-07 18:53:19.000000 linearwavetheory-0.0.4/src/linearwavetheory/dispersion.py
-drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 18:53:40.732244 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/
--rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-07 18:53:40.000000 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/PKG-INFO
--rw-r--r--   0 pietersmit   (502) staff       (20)      419 2023-08-07 18:53:40.000000 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/SOURCES.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)        1 2023-08-07 18:53:40.000000 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/dependency_links.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)       12 2023-08-07 18:53:40.000000 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/requires.txt
--rw-r--r--   0 pietersmit   (502) staff       (20)       17 2023-08-07 18:53:40.000000 linearwavetheory-0.0.4/src/linearwavetheory.egg-info/top_level.txt
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 19:39:20.125198 linearwavetheory-0.0.5/
+-rw-r--r--   0 pietersmit   (502) staff       (20)    11357 2023-08-06 02:37:22.000000 linearwavetheory-0.0.5/LICENSE
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-07 19:39:20.125085 linearwavetheory-0.0.5/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)      532 2023-08-06 03:43:57.000000 linearwavetheory-0.0.5/README.md
+-rw-r--r--   0 pietersmit   (502) staff       (20)       38 2023-08-07 19:39:20.125237 linearwavetheory-0.0.5/setup.cfg
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1055 2023-08-07 19:38:50.000000 linearwavetheory-0.0.5/setup.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 19:39:20.123120 linearwavetheory-0.0.5/src/
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 19:39:20.124194 linearwavetheory-0.0.5/src/linearwavetheory/
+-rw-r--r--   0 pietersmit   (502) staff       (20)      249 2023-08-06 03:43:57.000000 linearwavetheory-0.0.5/src/linearwavetheory/__init__.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)      260 2023-08-06 03:43:57.000000 linearwavetheory-0.0.5/src/linearwavetheory/_constants.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)      381 2023-07-18 23:20:42.000000 linearwavetheory-0.0.5/src/linearwavetheory/_numba_settings.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)     2195 2023-08-07 03:01:04.000000 linearwavetheory-0.0.5/src/linearwavetheory/_tools.py
+-rw-r--r--   0 pietersmit   (502) staff       (20)    44907 2023-08-07 19:39:05.000000 linearwavetheory-0.0.5/src/linearwavetheory/dispersion.py
+drwxr-xr-x   0 pietersmit   (502) staff       (20)        0 2023-08-07 19:39:20.124902 linearwavetheory-0.0.5/src/linearwavetheory.egg-info/
+-rw-r--r--   0 pietersmit   (502) staff       (20)     1169 2023-08-07 19:39:20.000000 linearwavetheory-0.0.5/src/linearwavetheory.egg-info/PKG-INFO
+-rw-r--r--   0 pietersmit   (502) staff       (20)      419 2023-08-07 19:39:20.000000 linearwavetheory-0.0.5/src/linearwavetheory.egg-info/SOURCES.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)        1 2023-08-07 19:39:20.000000 linearwavetheory-0.0.5/src/linearwavetheory.egg-info/dependency_links.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)       12 2023-08-07 19:39:20.000000 linearwavetheory-0.0.5/src/linearwavetheory.egg-info/requires.txt
+-rw-r--r--   0 pietersmit   (502) staff       (20)       17 2023-08-07 19:39:20.000000 linearwavetheory-0.0.5/src/linearwavetheory.egg-info/top_level.txt
```

### Comparing `linearwavetheory-0.0.4/LICENSE` & `linearwavetheory-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.4/PKG-INFO` & `linearwavetheory-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearwavetheory
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package that implements linear wave theory for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/linearwavetheory.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linearwavetheory-0.0.4/README.md` & `linearwavetheory-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.4/setup.py` & `linearwavetheory-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme_contents = file.read()
 
 setuptools.setup(
     name="linearwavetheory",
-    version="0.0.4",
+    version="0.0.5",
     license="Apache 2 License",
     install_requires=[
         "numpy",
         "numba",
     ],
     description="Python package that implements linear wave theory for ocean surface gravity waves",
     long_description=readme_contents,
```

### Comparing `linearwavetheory-0.0.4/src/linearwavetheory/_tools.py` & `linearwavetheory-0.0.5/src/linearwavetheory/_tools.py`

 * *Files identical despite different names*

### Comparing `linearwavetheory-0.0.4/src/linearwavetheory/dispersion.py` & `linearwavetheory-0.0.5/src/linearwavetheory/dispersion.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,33 +165,190 @@
     ```
     """
 
     # Numba does not recognize "atleast_1d" for scalars
     intrinsic_angular_frequency = atleast_1d(intrinsic_angular_frequency)
     depth = atleast_1d(depth)
 
-    if len(depth) == 1:
-        depth = np.full_like(intrinsic_angular_frequency, depth[0], dtype=depth.dtype)
+    if kinematic_surface_tension < 0:
+        raise ValueError("kinematic_surface_tension must be non-negative.")
 
-    if len(intrinsic_angular_frequency) != len(depth):
-        raise ValueError(
-            "intrinsic_angular_frequency and depth must have the same length."
+    if grav <= 0:
+        raise ValueError("grav must be positive.")
+
+    if maximum_number_of_iterations < 1:
+        raise ValueError("maximum_number_of_iterations must be at least 1.")
+
+    if relative_tolerance <= 0:
+        raise ValueError("relative_tolerance must be positive.")
+
+    if absolute_tolerance <= 0:
+        raise ValueError("absolute_tolerance must be positive.")
+
+    _limit = 0
+    # Passing as a number because numba vectorize does not support strings (it seems? - not well tested other than
+    # the naive approach of just passing a string fails.)
+    if limit == "deep":
+        _limit = 1
+    elif limit == "shallow":
+        _limit = 2
+    elif limit == "capillary":
+        _limit = 3
+    elif limit == "gravity":
+        _limit = 4
+
+    return _inverse_intrinsic_dispersion_relation_ufunc(
+        intrinsic_angular_frequency,
+        depth,
+        kinematic_surface_tension,
+        grav,
+        maximum_number_of_iterations,
+        relative_tolerance,
+        absolute_tolerance,
+        _limit,
+    )
+
+
+@vectorize()
+def _inverse_intrinsic_dispersion_relation_ufunc(
+    intrinsic_angular_frequency,
+    depth,
+    kinematic_surface_tension: float,
+    grav: float,
+    maximum_number_of_iterations: int,
+    relative_tolerance: float,
+    absolute_tolerance: float,
+    _limit: int,
+):
+    limit = "none"
+    """
+    ** Internal function. Call inverse_intrinsic_dispersion_relation instead. **
+
+    Find the wavenumber magnitude for a given intrinsic radial frequency through inversion of the dispersion relation
+    for linear gravity waves including suface tension effects, i.e. solve for wavenumber k in:
+
+        w = sqrt( ( ( g * k + tau * k**3 ) * tanh(k*d) )
+
+    with g gravitational acceleration, tau kinematice surface tension, k wavenumber and d depth. The dispersion relation
+    is solved using Newton Iteration with a first guess based on the dispersion relation for deep or shallow water
+    waves.
+
+    Notes:
+    - We only solve for real roots (no evanescent waves)
+    - For negative depths or zero depths we reduce nan (undefined)
+    - For zero frequency we return zero wavenumber
+    - Stopping criterium is based on relative and absolute tolerance:
+
+            | w - w_est | / w < relative_tolerance  (default 1e-3)
+
+            and
+
+            | w - w_est |  < absolute_tolerance  (default np.inf
+
+        where w is the intrinsic angular frequency and w_est is the estimated intrinsic angular frequency based on the
+        current estimate of the wavenumber. Per default we do not use the absolute stopping criterium.
+
+    - We exit when either maximum number of iterations (default 10 is reached, or tolerance is achieved.
+      Typically only 1 to 2 iterations are needed.
+
+    :param  intrinsic_angular_frequency: The radial frequency in rad/s as observed from a frame of reference moving with the
+        wave. Scalar.
+
+    :param depth: depth in meters. Scalar.
+
+    :param kinematic_surface_tension: kinematic surface tension in m^3/s^2. Per default set to 0.0728 N/m (water at 20C)
+        divided by density of seawater (1025 kg/m^3).
+
+    :param grav: gravitational acceleration in m/s^2. Default is 9.81 m/s^2.
+
+    :param maximum_number_of_iterations: Maximum number of iterations. Default is 10.
+
+    :param relative_tolerance: Relative accuracy used in the stopping criterium. Default is 1e-3.
+
+    :param absolute_tolerance: Absolute accuracy used in the stopping criterium. Default is np.inf.
+
+    :return: The wavenumber. Scalar.
+    """
+
+    # == Input Validation ==
+
+    # Since we can try to solve for the negative intrinsic frequency branch of the dispersion relation, we allow
+    # negative intrinsic frequencies. In this case the wavenumber magnitude is the same as for the positive branch.
+    intrinsic_angular_frequency = np.abs(intrinsic_angular_frequency)
+
+    # For zero or negative depths the solution is undefined.
+    if depth <= 0:
+        return np.nan
+
+    # For zero intrinsic frequency the wavenumber is zero
+    if intrinsic_angular_frequency == 0:
+        return 0.0
+
+    if limit == 0:
+        return intrinsic_angular_frequency**2 / grav
+    elif limit == 1:
+        return intrinsic_angular_frequency / np.sqrt(grav * depth)
+    elif limit == 2:
+        return (intrinsic_angular_frequency**2 / kinematic_surface_tension) ** (1 / 3)
+    elif limit == 3:
+        kinematic_surface_tension = 0.0
+
+    # == Initial Estimate ==
+    if intrinsic_angular_frequency > np.sqrt(grav / depth):
+        # use the deep water relation
+        wavenumber_estimate = intrinsic_angular_frequency**2 / grav
+    else:
+        # use the shallow water relation
+        wavenumber_estimate = intrinsic_angular_frequency / np.sqrt(grav * depth)
+
+    # If the initial estimate turns out to be in the capillary range- use the pure capillary dispersion relation for
+    # the initial estimate.
+    if wavenumber_estimate**3 * kinematic_surface_tension / grav > 5:
+        wavenumber_estimate = (
+            intrinsic_angular_frequency**2 / kinematic_surface_tension
+        ) ** (1 / 3)
+
+    # == Newton Iteration ==
+    for ii in range(0, maximum_number_of_iterations):
+        surface_tension_term = np.sqrt(
+            1 + kinematic_surface_tension * wavenumber_estimate**2 / grav
+        )
+
+        error = (
+            np.sqrt(grav * wavenumber_estimate * np.tanh(wavenumber_estimate * depth))
+            * surface_tension_term
+            - intrinsic_angular_frequency
+        )
+
+        if (
+            np.abs(error) < absolute_tolerance
+            and np.abs(error / intrinsic_angular_frequency) < relative_tolerance
+        ):
+            break
+
+        kd = wavenumber_estimate * depth
+
+        # Group speed in the absence of surface tension
+        cg = (1 / 2 + kd / np.sinh(2 * kd)) * np.sqrt(
+            grav / wavenumber_estimate * np.tanh(kd)
+        )
+
+        # Calculate the derivative of the error function with respect to wavenumber.
+        error_derivative_to_wavenumber = (
+            cg * surface_tension_term
+            + np.sqrt(grav * wavenumber_estimate * np.tanh(kd))
+            * wavenumber_estimate
+            * kinematic_surface_tension
+            / grav
+            / surface_tension_term
         )
 
-    wavenumber_estimate = np.empty_like(intrinsic_angular_frequency)
-    for jj in range(0, len(intrinsic_angular_frequency)):
-        wavenumber_estimate[jj] = _inverse_intrinsic_dispersion_relation_scalar(
-            intrinsic_angular_frequency[jj],
-            depth[jj],
-            kinematic_surface_tension,
-            grav,
-            maximum_number_of_iterations,
-            relative_tolerance,
-            absolute_tolerance,
-            limit,
+        # Newton Iteration
+        wavenumber_estimate = (
+            wavenumber_estimate - error / error_derivative_to_wavenumber
         )
 
     return wavenumber_estimate
 
 
 @jit(**numba_default)
 def _inverse_intrinsic_dispersion_relation_scalar(
```

### Comparing `linearwavetheory-0.0.4/src/linearwavetheory.egg-info/PKG-INFO` & `linearwavetheory-0.0.5/src/linearwavetheory.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearwavetheory
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package that implements linear wave theory for ocean surface gravity waves
 Home-page: https://github.com/sofarocean/linearwavetheory.git
 Author: Pieter Bart Smit
 Author-email: sofaroceangithubbot@gmail.com
 License: Apache 2 License
 Project-URL: Sofar Ocean Site, https://www.sofarocean.com
 Classifier: Programming Language :: Python :: 3
```

