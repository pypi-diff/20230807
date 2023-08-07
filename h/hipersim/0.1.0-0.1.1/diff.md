# Comparing `tmp/hipersim-0.1.0.tar.gz` & `tmp/hipersim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipersim-0.1.0.tar", last modified: Fri Jun 23 14:39:35 2023, max compression
+gzip compressed data, was "C:\Users\nkdi\Documents\Programs\hipersim\release\dist\.tmp-6f2r5jb0\hipersim-0.1.1.tar", last modified: Mon Aug  7 21:21:41 2023, max compression
```

## Comparing `hipersim-0.1.0.tar` & `hipersim-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 14:39:34.981090 hipersim-0.1.0/
--rw-rw-rw-   0        0        0     1086 2021-06-22 12:13:11.000000 hipersim-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       47 2021-10-01 12:38:50.000000 hipersim-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1348 2023-06-23 14:39:34.982602 hipersim-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      907 2021-09-27 21:27:22.000000 hipersim-0.1.0/README.md
--rw-rw-rw-   0        0        0      108 2021-06-22 09:04:30.000000 hipersim-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      678 2023-06-23 14:39:34.997015 hipersim-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 14:39:33.603843 hipersim-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 14:39:33.673322 hipersim-0.1.0/src/hipersim/
--rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.1.0/src/hipersim/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 14:39:34.201674 hipersim-0.1.0/src/hipersim/surrogates/
--rw-rw-rw-   0        0        0    33135 2021-09-30 23:02:13.000000 hipersim-0.1.0/src/hipersim/surrogates/AutoencoderModel_20Farms_10outputs.sav
--rw-rw-rw-   0        0        0    31911 2021-10-01 05:42:56.000000 hipersim-0.1.0/src/hipersim/surrogates/PyWake_Surrogate_10Farms_Power_Autoencoder.sav
--rw-rw-rw-   0        0        0    41997 2021-09-30 20:57:49.000000 hipersim-0.1.0/src/hipersim/surrogates/PyWake_Surrogate_10Farms_Power_RelativeLocation.sav
--rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.1.0/src/hipersim/surrogates/__init__.py
--rw-rw-rw-   0        0        0     8179 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/surrogates/farm_utils.py
--rw-rw-rw-   0        0        0     2006 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/surrogates/math_utils.py
--rw-rw-rw-   0        0        0    21250 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/surrogates/neuralnets.py
--rw-rw-rw-   0        0        0      604 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/surrogates/os_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-23 14:39:34.828119 hipersim-0.1.0/src/hipersim/turbgen/
--rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.1.0/src/hipersim/turbgen/__init__.py
--rw-rw-rw-   0        0        0    19408 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/turbgen/constrain_field.py
--rw-rw-rw-   0        0        0    17771 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/turbgen/constrain_field_1d.py
--rw-rw-rw-   0        0        0    31003 2023-06-23 14:34:21.000000 hipersim-0.1.0/src/hipersim/turbgen/generate_field.py
--rw-rw-rw-   0        0        0   457165 2023-06-23 13:55:19.000000 hipersim-0.1.0/src/hipersim/turbgen/mannspectrum.py
--rw-rw-rw-   0        0        0    26539 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/turbgen/manntensor.py
--rw-rw-rw-   0        0        0      490 2023-06-23 13:55:19.000000 hipersim-0.1.0/src/hipersim/turbgen/trapezoidal_sum_2d.py
--rw-rw-rw-   0        0        0     8810 2023-06-23 13:55:19.000000 hipersim-0.1.0/src/hipersim/turbgen/turb_utils.py
--rw-rw-rw-   0        0        0     8042 2023-06-23 13:55:19.000000 hipersim-0.1.0/src/hipersim/turbgen/turbgen.py
-drwxrwxrwx   0        0        0        0 2023-06-23 14:39:33.790183 hipersim-0.1.0/src/hipersim.egg-info/
--rw-rw-rw-   0        0        0     1348 2023-06-23 14:39:33.000000 hipersim-0.1.0/src/hipersim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1061 2023-06-23 14:39:33.000000 hipersim-0.1.0/src/hipersim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 14:39:33.000000 hipersim-0.1.0/src/hipersim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-23 14:39:33.000000 hipersim-0.1.0/src/hipersim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 14:39:33.000000 hipersim-0.1.0/src/hipersim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-23 14:39:34.973166 hipersim-0.1.0/tests/
--rw-rw-rw-   0        0        0     1454 2023-06-23 13:55:19.000000 hipersim-0.1.0/tests/test_manntensor.py
--rw-rw-rw-   0        0        0     9278 2023-06-23 14:34:22.000000 hipersim-0.1.0/tests/test_spectra.py
--rw-rw-rw-   0        0        0     6278 2023-06-23 14:34:22.000000 hipersim-0.1.0/tests/test_turb_gen.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:21:41.463208 hipersim-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2021-06-22 12:13:11.000000 hipersim-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       47 2021-10-01 12:38:50.000000 hipersim-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1348 2023-08-07 21:21:41.464206 hipersim-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      907 2021-09-27 21:27:22.000000 hipersim-0.1.1/README.md
+-rw-rw-rw-   0        0        0      108 2021-06-22 09:04:30.000000 hipersim-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      678 2023-08-07 21:21:41.479817 hipersim-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 21:21:41.032722 hipersim-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 21:21:41.068172 hipersim-0.1.1/src/hipersim/
+-rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.1.1/src/hipersim/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:21:41.241331 hipersim-0.1.1/src/hipersim/surrogates/
+-rw-rw-rw-   0        0        0    33135 2021-09-30 23:02:13.000000 hipersim-0.1.1/src/hipersim/surrogates/AutoencoderModel_20Farms_10outputs.sav
+-rw-rw-rw-   0        0        0    31911 2021-10-01 05:42:56.000000 hipersim-0.1.1/src/hipersim/surrogates/PyWake_Surrogate_10Farms_Power_Autoencoder.sav
+-rw-rw-rw-   0        0        0    41997 2021-09-30 20:57:49.000000 hipersim-0.1.1/src/hipersim/surrogates/PyWake_Surrogate_10Farms_Power_RelativeLocation.sav
+-rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.1.1/src/hipersim/surrogates/__init__.py
+-rw-rw-rw-   0        0        0     8179 2023-03-28 12:05:04.000000 hipersim-0.1.1/src/hipersim/surrogates/farm_utils.py
+-rw-rw-rw-   0        0        0     2006 2023-03-28 12:05:04.000000 hipersim-0.1.1/src/hipersim/surrogates/math_utils.py
+-rw-rw-rw-   0        0        0    21250 2023-03-28 12:05:04.000000 hipersim-0.1.1/src/hipersim/surrogates/neuralnets.py
+-rw-rw-rw-   0        0        0      604 2023-03-28 12:05:04.000000 hipersim-0.1.1/src/hipersim/surrogates/os_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:21:41.397695 hipersim-0.1.1/src/hipersim/turbgen/
+-rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.1.1/src/hipersim/turbgen/__init__.py
+-rw-rw-rw-   0        0        0    19408 2023-03-28 12:05:04.000000 hipersim-0.1.1/src/hipersim/turbgen/constrain_field.py
+-rw-rw-rw-   0        0        0    17771 2023-03-28 12:05:04.000000 hipersim-0.1.1/src/hipersim/turbgen/constrain_field_1d.py
+-rw-rw-rw-   0        0        0    30995 2023-08-07 21:14:51.000000 hipersim-0.1.1/src/hipersim/turbgen/generate_field.py
+-rw-rw-rw-   0        0        0   457165 2023-06-23 13:55:19.000000 hipersim-0.1.1/src/hipersim/turbgen/mannspectrum.py
+-rw-rw-rw-   0        0        0    26539 2023-03-28 12:05:04.000000 hipersim-0.1.1/src/hipersim/turbgen/manntensor.py
+-rw-rw-rw-   0        0        0      490 2023-06-23 13:55:19.000000 hipersim-0.1.1/src/hipersim/turbgen/trapezoidal_sum_2d.py
+-rw-rw-rw-   0        0        0     8810 2023-06-23 13:55:19.000000 hipersim-0.1.1/src/hipersim/turbgen/turb_utils.py
+-rw-rw-rw-   0        0        0     8042 2023-06-23 13:55:19.000000 hipersim-0.1.1/src/hipersim/turbgen/turbgen.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:21:41.120864 hipersim-0.1.1/src/hipersim.egg-info/
+-rw-rw-rw-   0        0        0     1348 2023-08-07 21:21:40.000000 hipersim-0.1.1/src/hipersim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1061 2023-08-07 21:21:41.000000 hipersim-0.1.1/src/hipersim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 21:21:40.000000 hipersim-0.1.1/src/hipersim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-08-07 21:21:40.000000 hipersim-0.1.1/src/hipersim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 21:21:40.000000 hipersim-0.1.1/src/hipersim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 21:21:41.458381 hipersim-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1454 2023-06-23 13:55:19.000000 hipersim-0.1.1/tests/test_manntensor.py
+-rw-rw-rw-   0        0        0     9278 2023-06-23 14:34:22.000000 hipersim-0.1.1/tests/test_spectra.py
+-rw-rw-rw-   0        0        0     6278 2023-06-23 14:34:22.000000 hipersim-0.1.1/tests/test_turb_gen.py
```

### Comparing `hipersim-0.1.0/LICENSE` & `hipersim-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/PKG-INFO` & `hipersim-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipersim
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of wind energy simulation tools
 Home-page: https://gitlab.windenergy.dtu.dk/HiperSim/hipersim
 Author: Nikolay Dimitrov
 Author-email: nkdi@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hipersim-0.1.0/README.md` & `hipersim-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/setup.cfg` & `hipersim-0.1.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 6970 6572 7369 6d0d 0a76 6572   = hipersim..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e30 0d0a 6175  sion = 0.1.0..au
+00000020: 7369 6f6e 203d 2030 2e31 2e31 0d0a 6175  sion = 0.1.1..au
 00000030: 7468 6f72 203d 204e 696b 6f6c 6179 2044  thor = Nikolay D
 00000040: 696d 6974 726f 760d 0a61 7574 686f 725f  imitrov..author_
 00000050: 656d 6169 6c20 3d20 6e6b 6469 4064 7475  email = nkdi@dtu
 00000060: 2e64 6b0d 0a64 6573 6372 6970 7469 6f6e  .dk..description
 00000070: 203d 2041 2063 6f6c 6c65 6374 696f 6e20   = A collection 
 00000080: 6f66 2077 696e 6420 656e 6572 6779 2073  of wind energy s
 00000090: 696d 756c 6174 696f 6e20 746f 6f6c 730d  imulation tools.
```

### Comparing `hipersim-0.1.0/src/hipersim/surrogates/AutoencoderModel_20Farms_10outputs.sav` & `hipersim-0.1.1/src/hipersim/surrogates/AutoencoderModel_20Farms_10outputs.sav`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/surrogates/PyWake_Surrogate_10Farms_Power_Autoencoder.sav` & `hipersim-0.1.1/src/hipersim/surrogates/PyWake_Surrogate_10Farms_Power_Autoencoder.sav`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/surrogates/PyWake_Surrogate_10Farms_Power_RelativeLocation.sav` & `hipersim-0.1.1/src/hipersim/surrogates/PyWake_Surrogate_10Farms_Power_RelativeLocation.sav`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/surrogates/farm_utils.py` & `hipersim-0.1.1/src/hipersim/surrogates/farm_utils.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/surrogates/math_utils.py` & `hipersim-0.1.1/src/hipersim/surrogates/math_utils.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/surrogates/neuralnets.py` & `hipersim-0.1.1/src/hipersim/surrogates/neuralnets.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/surrogates/os_utils.py` & `hipersim-0.1.1/src/hipersim/surrogates/os_utils.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/turbgen/constrain_field.py` & `hipersim-0.1.1/src/hipersim/turbgen/constrain_field.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/turbgen/constrain_field_1d.py` & `hipersim-0.1.1/src/hipersim/turbgen/constrain_field_1d.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/turbgen/generate_field.py` & `hipersim-0.1.1/src/hipersim/turbgen/generate_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 """
 Created on Sat Apr 24 12:23:07 2021
 
 @author: nkdi, mmpe, astah
 """
 import numpy as np
 import time
-from src.hipersim.turbgen.manntensor import manntensorcomponents
-from src.hipersim.turbgen.trapezoidal_sum_2d import trapezoidal_sum_2d
+from hipersim.turbgen.manntensor import manntensorcomponents
+from hipersim.turbgen.trapezoidal_sum_2d import trapezoidal_sum_2d
 
 
 class SpectralTensor():
     def __init__(self, alphaepsilon, L, Gamma, Nx, Ny, Nz, dx, dy, dz,
                  HighFreqComp=0, double_x=False, double_y=True, double_z=True):
         self.alphaepsilon = alphaepsilon
         self.L = L
```

### Comparing `hipersim-0.1.0/src/hipersim/turbgen/mannspectrum.py` & `hipersim-0.1.1/src/hipersim/turbgen/mannspectrum.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/turbgen/manntensor.py` & `hipersim-0.1.1/src/hipersim/turbgen/manntensor.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/turbgen/turb_utils.py` & `hipersim-0.1.1/src/hipersim/turbgen/turb_utils.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim/turbgen/turbgen.py` & `hipersim-0.1.1/src/hipersim/turbgen/turbgen.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/src/hipersim.egg-info/PKG-INFO` & `hipersim-0.1.1/src/hipersim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipersim
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of wind energy simulation tools
 Home-page: https://gitlab.windenergy.dtu.dk/HiperSim/hipersim
 Author: Nikolay Dimitrov
 Author-email: nkdi@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hipersim-0.1.0/src/hipersim.egg-info/SOURCES.txt` & `hipersim-0.1.1/src/hipersim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/tests/test_manntensor.py` & `hipersim-0.1.1/tests/test_manntensor.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/tests/test_spectra.py` & `hipersim-0.1.1/tests/test_spectra.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.1.0/tests/test_turb_gen.py` & `hipersim-0.1.1/tests/test_turb_gen.py`

 * *Files identical despite different names*

