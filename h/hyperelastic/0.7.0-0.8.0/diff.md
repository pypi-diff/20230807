# Comparing `tmp/hyperelastic-0.7.0.tar.gz` & `tmp/hyperelastic-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperelastic-0.7.0.tar", last modified: Sun Aug  6 20:46:57 2023, max compression
+gzip compressed data, was "hyperelastic-0.8.0.tar", last modified: Mon Aug  7 10:05:59 2023, max compression
```

## Comparing `hyperelastic-0.7.0.tar` & `hyperelastic-0.8.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.809732 hyperelastic-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-08-06 20:46:57.809732 hyperelastic-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 20:46:57.809732 hyperelastic-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.801732 hyperelastic-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.801732 hyperelastic-0.7.0/src/hyperelastic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/frameworks/_generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/frameworks/_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/frameworks/_stretches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/lab/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_curve_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_load_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/math/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27718 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/math/_voigt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/models/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/models/generalized/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/generalized/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/generalized/_stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/models/invariants/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/invariants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/invariants/_third_order_deformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/models/stretches/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/stretches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/stretches/_generalized_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/stretches/_ogden.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/spaces/_deformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/spaces/_dilatational.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/spaces/_distortional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.801732 hyperelastic-0.7.0/src/hyperelastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-08-06 20:46:57.000000 hyperelastic-0.7.0/src/hyperelastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-06 20:46:57.000000 hyperelastic-0.7.0/src/hyperelastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:46:57.000000 hyperelastic-0.7.0/src/hyperelastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 20:46:57.000000 hyperelastic-0.7.0/src/hyperelastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 20:46:57.000000 hyperelastic-0.7.0/src/hyperelastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_lab_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_sympy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.623826 hyperelastic-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50629 2023-08-07 10:05:59.623826 hyperelastic-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:05:59.623826 hyperelastic-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.619826 hyperelastic-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.619826 hyperelastic-0.8.0/src/hyperelastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.619826 hyperelastic-0.8.0/src/hyperelastic/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/frameworks/_generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/frameworks/_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/frameworks/_stretches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.623826 hyperelastic-0.8.0/src/hyperelastic/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/lab/_curve_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/lab/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/lab/_load_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/lab/_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/lab/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/lab/_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.623826 hyperelastic-0.8.0/src/hyperelastic/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27718 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/math/_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.623826 hyperelastic-0.8.0/src/hyperelastic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.623826 hyperelastic-0.8.0/src/hyperelastic/models/generalized/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/models/generalized/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/models/generalized/_stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.623826 hyperelastic-0.8.0/src/hyperelastic/models/invariants/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/models/invariants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/models/invariants/_third_order_deformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.623826 hyperelastic-0.8.0/src/hyperelastic/models/stretches/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/models/stretches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/models/stretches/_generalized_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/models/stretches/_ogden.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.623826 hyperelastic-0.8.0/src/hyperelastic/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/spaces/_deformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/spaces/_dilatational.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/src/hyperelastic/spaces/_distortional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.619826 hyperelastic-0.8.0/src/hyperelastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50629 2023-08-07 10:05:59.000000 hyperelastic-0.8.0/src/hyperelastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-07 10:05:59.000000 hyperelastic-0.8.0/src/hyperelastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:05:59.000000 hyperelastic-0.8.0/src/hyperelastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 10:05:59.000000 hyperelastic-0.8.0/src/hyperelastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 10:05:59.000000 hyperelastic-0.8.0/src/hyperelastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:05:59.623826 hyperelastic-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/tests/test_generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/tests/test_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/tests/test_lab_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/tests/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-07 10:05:50.000000 hyperelastic-0.8.0/tests/test_sympy.py
```

### Comparing `hyperelastic-0.7.0/LICENSE` & `hyperelastic-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/PKG-INFO` & `hyperelastic-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.7.0
+Version: 0.8.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -775,15 +775,15 @@
 
 model = MyInvariantsModel()
 framework = hel.InvariantsFramework(model)
 umat = hel.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic invariant-based material formulations
-The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model) are all available as submodels of the third order deformation material formulation.
+The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model)) are all available as submodels of the third order deformation material formulation.
 
 - [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/invariants/_third_order_deformation.py))
 
 ## Principal stretch-based material formulations
 A minimal template for a principal stretch-based material formulation applied on the distortional space:
 
 ```python
```

### Comparing `hyperelastic-0.7.0/README.md` & `hyperelastic-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 model = MyInvariantsModel()
 framework = hel.InvariantsFramework(model)
 umat = hel.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic invariant-based material formulations
-The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model) are all available as submodels of the third order deformation material formulation.
+The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model)) are all available as submodels of the third order deformation material formulation.
 
 - [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/invariants/_third_order_deformation.py))
 
 ## Principal stretch-based material formulations
 A minimal template for a principal stretch-based material formulation applied on the distortional space:
 
 ```python
```

### Comparing `hyperelastic-0.7.0/pyproject.toml` & `hyperelastic-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/__init__.py` & `hyperelastic-0.8.0/src/hyperelastic/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/frameworks/_generalized.py` & `hyperelastic-0.8.0/src/hyperelastic/frameworks/_generalized.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/frameworks/_invariants.py` & `hyperelastic-0.8.0/src/hyperelastic/frameworks/_invariants.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/frameworks/_stretches.py` & `hyperelastic-0.8.0/src/hyperelastic/frameworks/_stretches.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/lab/_curve_fit.py` & `hyperelastic-0.8.0/src/hyperelastic/lab/_curve_fit.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/lab/_experiment.py` & `hyperelastic-0.8.0/src/hyperelastic/lab/_experiment.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/lab/_load_case.py` & `hyperelastic-0.8.0/src/hyperelastic/lab/_load_case.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,24 @@
         \boldsymbol{P} = J \boldsymbol{\sigma} \boldsymbol{F}^{-T}
 
     The deformation gradient and its determinant are evaluated for the
     homogeneous incompressible deformation.
 
     ..  math::
         \boldsymbol{F} &= \text{diag} \left(\begin{bmatrix}
-        \lambda_1 & \lambda_2 & \frac{1}{\lambda_1 \lambda_2} \end{bmatrix} \right)
+            \lambda_1 & \lambda_2 & \lambda_3 \end{bmatrix} \right)
 
-        J &= 1
+        J &= \lambda_1 \lambda_2 \lambda_3 = 1
 
-    This enables the evaluation of the normal force per undeformed area.
+    This enables the evaluation of the normal force per undeformed area, where
+    quantities in the traction-free transverse direction are denoted with a subscript
+    :math:`(\bullet)_t`.
 
     ..  math::
-        \frac{N_i}{A_i} = P_{(ii)} - P_{(jj)} \frac{\lambda_j}{\lambda_i}
+        \frac{N}{A} = P - P_t \frac{\lambda_t}{\lambda}
 
     """
 
     def stress(self, F, P, axis=0, traction_free=-1):
         r"""Normal force per undeformed area for a given deformation gradient of an
         incompressible deformation and the first Piola-Kirchhoff stress tensor.
 
@@ -74,15 +76,16 @@
             \lambda & \frac{1}{\sqrt{\lambda}} & \frac{1}{\sqrt{\lambda}} \end{bmatrix}
             \right)
 
     """
 
     def __init__(self, label=None):
         if label is None:
-            self.label = "Uniaxial Tension"
+            label = "Uniaxial Tension"
+        self.label = label
 
     def defgrad(self, stretch):
         "Return the Deformation Gradient tensor from given stretches."
 
         x = stretch
         y = 1 / np.sqrt(stretch)
         z = np.zeros_like(stretch)
@@ -98,15 +101,16 @@
             \lambda & \lambda & \frac{1}{\lambda^2} \end{bmatrix}
             \right)
 
     """
 
     def __init__(self, label=None):
         if label is None:
-            self.label = "Biaxial Tension"
+            label = "Biaxial Tension"
+        self.label = label
 
     def defgrad(self, stretch):
         "Return the Deformation Gradient tensor from given stretches."
 
         x = stretch
         y = 1 / stretch**2
         z = np.zeros_like(stretch)
@@ -122,15 +126,16 @@
             \lambda & 1 & \frac{1}{\lambda} \end{bmatrix}
             \right)
 
     """
 
     def __init__(self, label=None):
         if label is None:
-            self.label = "Planar Tension"
+            label = "Planar Tension"
+        self.label = label
 
     def defgrad(self, stretch):
         "Return the Deformation Gradient tensor from given stretches."
 
         x = stretch
         y = 1 / stretch
         o = np.ones_like(stretch)
```

### Comparing `hyperelastic-0.7.0/src/hyperelastic/lab/_optimize.py` & `hyperelastic-0.8.0/src/hyperelastic/lab/_optimize.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/lab/_plotting.py` & `hyperelastic-0.8.0/src/hyperelastic/lab/_plotting.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/lab/_simulation.py` & `hyperelastic-0.8.0/src/hyperelastic/lab/_simulation.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,62 @@
     material : class
         A class with a method for evaluating the gradient of the strain energy function
         w.r.t. the deformation gradient, e.g.
         :class:`DistortionalSpace <.DistortionalSpace>`.
     parameters : array_like
         The material parameters.
 
+
+    Examples
+    --------
+    The material model response behaviour of a hyperelastic material model formulation
+    is evaluated for a :class:`uniaxial tension <.lab.Uniaxial>` load case. A given
+    stretch data is used to create the :class:`Simulation <.lab.Simulation>` object.
+
+    >>> import numpy as np
+    >>> import hyperelastic
+    >>> from hyperelastic import lab
+    >>>
+    >>> stretch = np.linspace(0.7, 2.5, 181)
+
+    A function which takes the material parameters and returns the hyperelastic
+    constitutive material formulation has to be provided for the simulation objects.
+    Here, we use an isotropic invariant-based
+    :class:`third-order deformation <.models.invariants.ThirdOrderDeformation>`
+    material formulation.
+
+    >>> def material(**kwargs):
+    >>>     "A third-order deformation material formulation."
+    >>>
+    >>>     tod = hyperelastic.models.invariants.ThirdOrderDeformation(**kwargs)
+    >>>     framework = hyperelastic.InvariantsFramework(tod)
+    >>>
+    >>>     return hyperelastic.DeformationSpace(framework)
+
+    A list of (string) labels is used to apply the list or array of parameter values to
+    the material formulation.
+
+    >>> simulation = lab.Simulation(
+    >>>     loadcase=lab.Uniaxial(),
+    >>>     stretch=stretch,
+    >>>     material=material,
+    >>>     labels=["C10", "C01", "C11", "C20", "C30"],
+    >>>     parameters=[0.4, 0.1, 0.02, -0.04, 0.01],
+    >>> )
+
+    The stress-stretch plot returns a figure which visualizes the force per undeformed
+    area vs. the ratio of the undeformed and deformed length.
+
+    >>> fig, ax = simulation.plot_stress_stretch()
+    >>>
+    >>> ax.legend()
+    >>> ax.set_title("Third-Order Deformation")
+
+    ..  image:: images/fig_simulation-tod.png
+
     """
 
     def __init__(self, loadcase, stretch, labels, material, parameters=None):
         """Initialize the results of a simulation.
 
         Parameters
         ----------
@@ -40,58 +88,14 @@
         material : class
             A class with a method for evaluating the gradient of the strain energy
             function w.r.t. the deformation gradient, e.g.
             :class:`DistortionalSpace <.DistortionalSpace>`.
         parameters : array_like or None, optional
             The material parameters (default is None).
 
-        Examples
-        --------
-        A test specimen is subjected to uniaxial tension. The stretch and force per
-        undeformed area data are used to create the
-        :class:`Simulation <.lab.Simulation>`.
-
-        >>> import numpy as np
-        >>> import hyperelastic
-        >>> from hyperelastic import lab
-        >>>
-        >>> stretch = np.linspace(0.7, 2.5, 181)
-
-        A function which takes the material parameters and returns the hyperelastic
-        constitutive material formulation has to be provided for the simulation objects.
-        Here, we use an isotropic invariant-based
-        :class:`third-order deformation <.models.invariants.ThirdOrderDeformation>`
-        material formulation.
-
-        >>> def material(**kwargs):
-        >>>     "A third-order deformation material formulation."
-        >>>
-        >>>     tod = hyperelastic.models.invariants.ThirdOrderDeformation(**kwargs)
-        >>>     framework = hyperelastic.InvariantsFramework(tod)
-        >>>
-        >>>     return hyperelastic.DeformationSpace(framework)
-
-        The list of labels is used to apply the parameter values to the material
-        parameters.
-
-        >>> simulation = lab.Simulation(
-        >>>     loadcase=lab.Uniaxial(),
-        >>>     stretch=stretch,
-        >>>     material=material,
-        >>>     labels=["C10", "C01", "C11", "C20", "C30"],
-        >>>     parameters=[0.4, 0.1, 0.02, -0.04, 0.01],
-        >>> )
-
-        >>> fig, ax = simulation.plot_stress_stretch()
-        >>>
-        >>> ax.legend()
-        >>> ax.set_title("Third-Order Deformation")
-
-        ..  image:: images/fig_simulation-tod.png
-
         """
 
         super().__init__()
 
         self.loadcase = loadcase
         self.stretch = stretch
         self.labels = labels
```

### Comparing `hyperelastic-0.7.0/src/hyperelastic/math/_voigt.py` & `hyperelastic-0.8.0/src/hyperelastic/math/_voigt.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/models/generalized/_stretch.py` & `hyperelastic-0.8.0/src/hyperelastic/models/generalized/_stretch.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/models/invariants/_third_order_deformation.py` & `hyperelastic-0.8.0/src/hyperelastic/models/invariants/_third_order_deformation.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/models/stretches/_generalized_invariants.py` & `hyperelastic-0.8.0/src/hyperelastic/models/stretches/_generalized_invariants.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/models/stretches/_ogden.py` & `hyperelastic-0.8.0/src/hyperelastic/models/stretches/_ogden.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/spaces/_deformation.py` & `hyperelastic-0.8.0/src/hyperelastic/spaces/_deformation.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/spaces/_dilatational.py` & `hyperelastic-0.8.0/src/hyperelastic/spaces/_dilatational.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic/spaces/_distortional.py` & `hyperelastic-0.8.0/src/hyperelastic/spaces/_distortional.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/src/hyperelastic.egg-info/PKG-INFO` & `hyperelastic-0.8.0/src/hyperelastic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.7.0
+Version: 0.8.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -775,15 +775,15 @@
 
 model = MyInvariantsModel()
 framework = hel.InvariantsFramework(model)
 umat = hel.DistortionalSpace(framework)
 ```
 
 ### Available isotropic hyperelastic invariant-based material formulations
-The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model) are all available as submodels of the third order deformation material formulation.
+The typical polynomial-based material formulations ([Neo-Hooke](https://en.wikipedia.org/wiki/Neo-Hookean_solid), [Mooney-Rivlin](https://en.wikipedia.org/wiki/Mooney%E2%80%93Rivlin_solid), [Yeoh](https://en.wikipedia.org/wiki/Yeoh_hyperelastic_model)) are all available as submodels of the third order deformation material formulation.
 
 - [Third-Order-Deformation (James-Green-Simpson)](https://onlinelibrary.wiley.com/doi/abs/10.1002/app.1975.070190723) ([code](https://github.com/adtzlr/hyperelastic/blob/main/src/hyperelastic/models/invariants/_third_order_deformation.py))
 
 ## Principal stretch-based material formulations
 A minimal template for a principal stretch-based material formulation applied on the distortional space:
 
 ```python
```

### Comparing `hyperelastic-0.7.0/src/hyperelastic.egg-info/SOURCES.txt` & `hyperelastic-0.8.0/src/hyperelastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/tests/test_generalized.py` & `hyperelastic-0.8.0/tests/test_generalized.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/tests/test_lab.py` & `hyperelastic-0.8.0/tests/test_lab.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/tests/test_lab_simple.py` & `hyperelastic-0.8.0/tests/test_lab_simple.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/tests/test_math.py` & `hyperelastic-0.8.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/tests/test_simulation.py` & `hyperelastic-0.8.0/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/tests/test_space.py` & `hyperelastic-0.8.0/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.7.0/tests/test_sympy.py` & `hyperelastic-0.8.0/tests/test_sympy.py`

 * *Files identical despite different names*

