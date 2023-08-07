# Comparing `tmp/unipolator-0.3.0.tar.gz` & `tmp/unipolator-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipolator-0.3.0.tar", last modified: Fri Jul  7 15:04:35 2023, max compression
+gzip compressed data, was "unipolator-0.3.2.tar", last modified: Mon Aug  7 16:06:03 2023, max compression
```

## Comparing `unipolator-0.3.0.tar` & `unipolator-0.3.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 15:04:35.140015 unipolator-0.3.0/
--rw-rw-rw-   0        0        0     1096 2023-07-04 08:51:45.000000 unipolator-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       86 2023-07-04 08:51:45.000000 unipolator-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4984 2023-07-07 15:04:35.140015 unipolator-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4261 2023-07-07 14:54:26.000000 unipolator-0.3.0/README.md
--rw-rw-rw-   0        0        0       30 2023-07-04 08:51:45.000000 unipolator-0.3.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       26 2023-07-04 08:51:45.000000 unipolator-0.3.0/requirements.txt
--rw-rw-rw-   0        0        0      979 2023-07-07 15:04:35.154133 unipolator-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     3705 2023-07-04 08:51:45.000000 unipolator-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:04:34.914975 unipolator-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 15:04:35.074550 unipolator-0.3.0/src/unipolator/
--rw-rw-rw-   0        0        0      540 2023-06-23 17:24:42.000000 unipolator-0.3.0/src/unipolator/__init__.py
--rw-rw-rw-   0        0        0  1034336 2023-07-04 16:40:53.000000 unipolator-0.3.0/src/unipolator/blas_functions.c
--rw-rw-rw-   0        0        0     3529 2023-06-20 17:16:13.000000 unipolator-0.3.0/src/unipolator/blas_functions.pxd
--rw-rw-rw-   0        0        0    12966 2023-06-20 17:16:14.000000 unipolator-0.3.0/src/unipolator/blas_functions.pyx
--rw-rw-rw-   0        0        0   939774 2023-07-04 16:40:55.000000 unipolator-0.3.0/src/unipolator/blas_functions_vectors.c
--rw-rw-rw-   0        0        0     1996 2023-06-21 11:45:33.000000 unipolator-0.3.0/src/unipolator/blas_functions_vectors.pxd
--rw-rw-rw-   0        0        0    10315 2023-06-21 14:22:37.000000 unipolator-0.3.0/src/unipolator/blas_functions_vectors.pyx
--rw-rw-rw-   0        0        0  1169151 2023-07-07 15:04:01.000000 unipolator-0.3.0/src/unipolator/caching.c
--rw-rw-rw-   0        0        0      327 2023-03-14 14:26:20.000000 unipolator-0.3.0/src/unipolator/caching.pxd
--rw-rw-rw-   0        0        0    16121 2023-03-14 14:26:20.000000 unipolator-0.3.0/src/unipolator/caching.pyx
--rw-rw-rw-   0        0        0  1117308 2023-07-07 15:04:03.000000 unipolator-0.3.0/src/unipolator/exp_and_log.c
--rw-rw-rw-   0        0        0     4322 2023-05-14 09:49:40.000000 unipolator-0.3.0/src/unipolator/exp_and_log.pxd
--rw-rw-rw-   0        0        0    16395 2023-05-14 10:14:00.000000 unipolator-0.3.0/src/unipolator/exp_and_log.pyx
--rw-rw-rw-   0        0        0  1071936 2023-07-07 15:04:06.000000 unipolator-0.3.0/src/unipolator/hamiltonian_system.c
--rw-rw-rw-   0        0        0    12369 2023-06-20 08:33:21.000000 unipolator-0.3.0/src/unipolator/hamiltonian_system.pyx
--rw-rw-rw-   0        0        0   972905 2023-07-07 15:04:08.000000 unipolator-0.3.0/src/unipolator/hamiltonian_system_vector.c
--rw-rw-rw-   0        0        0     6556 2023-06-22 14:33:53.000000 unipolator-0.3.0/src/unipolator/hamiltonian_system_vector.pyx
--rw-rw-rw-   0        0        0  1176137 2023-07-07 15:04:11.000000 unipolator-0.3.0/src/unipolator/indexing.c
--rw-rw-rw-   0        0        0     1918 2023-03-14 14:26:20.000000 unipolator-0.3.0/src/unipolator/indexing.pxd
--rw-rw-rw-   0        0        0    11597 2023-03-14 14:26:21.000000 unipolator-0.3.0/src/unipolator/indexing.pyx
--rw-rw-rw-   0        0        0   996203 2023-07-07 15:04:15.000000 unipolator-0.3.0/src/unipolator/sym_trotter_system.c
--rw-rw-rw-   0        0        0    13791 2023-05-03 10:17:56.000000 unipolator-0.3.0/src/unipolator/sym_trotter_system.pyx
--rw-rw-rw-   0        0        0  1010843 2023-07-07 15:04:18.000000 unipolator-0.3.0/src/unipolator/sym_trotter_system_vector.c
--rw-rw-rw-   0        0        0    14805 2023-06-22 14:33:38.000000 unipolator-0.3.0/src/unipolator/sym_trotter_system_vector.pyx
--rw-rw-rw-   0        0        0  1085385 2023-07-07 15:04:20.000000 unipolator-0.3.0/src/unipolator/symmetric_unitary_interpolation.c
--rw-rw-rw-   0        0        0    11483 2023-06-23 21:07:25.000000 unipolator-0.3.0/src/unipolator/symmetric_unitary_interpolation.pyx
--rw-rw-rw-   0        0        0  1099315 2023-07-07 15:04:23.000000 unipolator-0.3.0/src/unipolator/symmetric_unitary_interpolation_vector.c
--rw-rw-rw-   0        0        0    14996 2023-06-23 21:07:25.000000 unipolator-0.3.0/src/unipolator/symmetric_unitary_interpolation_vector.pyx
--rw-rw-rw-   0        0        0   980859 2023-07-07 15:04:25.000000 unipolator-0.3.0/src/unipolator/trotter_system.c
--rw-rw-rw-   0        0        0    15625 2023-06-20 09:36:37.000000 unipolator-0.3.0/src/unipolator/trotter_system.pyx
--rw-rw-rw-   0        0        0   992953 2023-07-07 15:04:27.000000 unipolator-0.3.0/src/unipolator/trotter_system_vector.c
--rw-rw-rw-   0        0        0    14375 2023-06-22 14:33:15.000000 unipolator-0.3.0/src/unipolator/trotter_system_vector.pyx
--rw-rw-rw-   0        0        0      220 2023-04-24 11:56:46.000000 unipolator-0.3.0/src/unipolator/unipolator.pyx
--rw-rw-rw-   0        0        0  1203106 2023-07-07 15:04:30.000000 unipolator-0.3.0/src/unipolator/unitary_interpolation.c
--rw-rw-rw-   0        0        0    22136 2023-06-20 08:44:04.000000 unipolator-0.3.0/src/unipolator/unitary_interpolation.pyx
--rw-rw-rw-   0        0        0  1174908 2023-07-07 15:04:32.000000 unipolator-0.3.0/src/unipolator/unitary_interpolation_vector.c
--rw-rw-rw-   0        0        0    21484 2023-06-22 17:41:14.000000 unipolator-0.3.0/src/unipolator/unitary_interpolation_vector.pyx
--rw-rw-rw-   0        0        0    21740 2023-05-14 14:16:58.000000 unipolator-0.3.0/src/unipolator/unitary_interpolation_vector_old.pyx
-drwxrwxrwx   0        0        0        0 2023-07-07 15:04:35.122268 unipolator-0.3.0/src/unipolator.egg-info/
--rw-rw-rw-   0        0        0     4984 2023-07-07 15:04:33.000000 unipolator-0.3.0/src/unipolator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1779 2023-07-07 15:04:34.000000 unipolator-0.3.0/src/unipolator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 15:04:33.000000 unipolator-0.3.0/src/unipolator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-04 08:52:35.000000 unipolator-0.3.0/src/unipolator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       85 2023-07-07 15:04:33.000000 unipolator-0.3.0/src/unipolator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-07 15:04:33.000000 unipolator-0.3.0/src/unipolator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 15:04:34.923184 unipolator-0.3.0/test/
-drwxrwxrwx   0        0        0        0 2023-07-07 15:04:35.140015 unipolator-0.3.0/test/Outlook/
--rw-rw-rw-   0        0        0     4771 2023-06-12 12:51:11.000000 unipolator-0.3.0/test/Outlook/expm_v.pyx
+drwxrwxrwx   0        0        0        0 2023-08-07 16:06:03.268130 unipolator-0.3.2/
+-rw-rw-rw-   0        0        0     1096 2023-08-07 15:58:43.000000 unipolator-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0       86 2023-08-07 15:58:43.000000 unipolator-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5441 2023-08-07 16:06:03.268130 unipolator-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4718 2023-08-07 15:58:43.000000 unipolator-0.3.2/README.md
+-rw-rw-rw-   0        0        0       30 2023-08-07 15:58:43.000000 unipolator-0.3.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       26 2023-08-07 15:58:43.000000 unipolator-0.3.2/requirements.txt
+-rw-rw-rw-   0        0        0      985 2023-08-07 16:06:03.270753 unipolator-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     3740 2023-08-07 16:05:13.000000 unipolator-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:06:03.138759 unipolator-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 16:06:03.243263 unipolator-0.3.2/src/unipolator/
+-rw-rw-rw-   0        0        0      579 2023-08-04 19:01:02.000000 unipolator-0.3.2/src/unipolator/__init__.py
+-rw-rw-rw-   0        0        0    18415 2023-08-07 15:23:06.000000 unipolator-0.3.2/src/unipolator/autobinning.py
+-rw-rw-rw-   0        0        0  1034341 2023-08-07 15:58:51.000000 unipolator-0.3.2/src/unipolator/blas_functions.c
+-rw-rw-rw-   0        0        0     3529 2023-06-20 17:16:13.000000 unipolator-0.3.2/src/unipolator/blas_functions.pxd
+-rw-rw-rw-   0        0        0    12966 2023-06-20 17:16:14.000000 unipolator-0.3.2/src/unipolator/blas_functions.pyx
+-rw-rw-rw-   0        0        0   939770 2023-08-07 15:58:52.000000 unipolator-0.3.2/src/unipolator/blas_functions_vectors.c
+-rw-rw-rw-   0        0        0     1996 2023-06-21 11:45:33.000000 unipolator-0.3.2/src/unipolator/blas_functions_vectors.pxd
+-rw-rw-rw-   0        0        0    10315 2023-06-21 14:22:37.000000 unipolator-0.3.2/src/unipolator/blas_functions_vectors.pyx
+-rw-rw-rw-   0        0        0  1169151 2023-08-07 15:58:53.000000 unipolator-0.3.2/src/unipolator/caching.c
+-rw-rw-rw-   0        0        0      327 2023-03-14 14:26:20.000000 unipolator-0.3.2/src/unipolator/caching.pxd
+-rw-rw-rw-   0        0        0    16121 2023-03-14 14:26:20.000000 unipolator-0.3.2/src/unipolator/caching.pyx
+-rw-rw-rw-   0        0        0  1117317 2023-08-07 15:58:56.000000 unipolator-0.3.2/src/unipolator/exp_and_log.c
+-rw-rw-rw-   0        0        0     4322 2023-05-14 09:49:40.000000 unipolator-0.3.2/src/unipolator/exp_and_log.pxd
+-rw-rw-rw-   0        0        0    16395 2023-05-14 10:14:00.000000 unipolator-0.3.2/src/unipolator/exp_and_log.pyx
+-rw-rw-rw-   0        0        0  1071945 2023-08-07 15:58:59.000000 unipolator-0.3.2/src/unipolator/hamiltonian_system.c
+-rw-rw-rw-   0        0        0    12369 2023-06-20 08:33:21.000000 unipolator-0.3.2/src/unipolator/hamiltonian_system.pyx
+-rw-rw-rw-   0        0        0   972905 2023-08-07 15:59:01.000000 unipolator-0.3.2/src/unipolator/hamiltonian_system_vector.c
+-rw-rw-rw-   0        0        0     6556 2023-06-22 14:33:53.000000 unipolator-0.3.2/src/unipolator/hamiltonian_system_vector.pyx
+-rw-rw-rw-   0        0        0  1176137 2023-08-07 15:59:02.000000 unipolator-0.3.2/src/unipolator/indexing.c
+-rw-rw-rw-   0        0        0     1918 2023-03-14 14:26:20.000000 unipolator-0.3.2/src/unipolator/indexing.pxd
+-rw-rw-rw-   0        0        0    11597 2023-03-14 14:26:21.000000 unipolator-0.3.2/src/unipolator/indexing.pyx
+-rw-rw-rw-   0        0        0   996212 2023-08-07 15:59:05.000000 unipolator-0.3.2/src/unipolator/sym_trotter_system.c
+-rw-rw-rw-   0        0        0    13791 2023-05-03 10:17:56.000000 unipolator-0.3.2/src/unipolator/sym_trotter_system.pyx
+-rw-rw-rw-   0        0        0  1010843 2023-08-07 15:59:06.000000 unipolator-0.3.2/src/unipolator/sym_trotter_system_vector.c
+-rw-rw-rw-   0        0        0    14805 2023-06-22 14:33:38.000000 unipolator-0.3.2/src/unipolator/sym_trotter_system_vector.pyx
+-rw-rw-rw-   0        0        0  1085385 2023-08-07 15:59:08.000000 unipolator-0.3.2/src/unipolator/symmetric_unitary_interpolation.c
+-rw-rw-rw-   0        0        0    11483 2023-06-23 21:07:25.000000 unipolator-0.3.2/src/unipolator/symmetric_unitary_interpolation.pyx
+-rw-rw-rw-   0        0        0  1099315 2023-08-07 15:59:09.000000 unipolator-0.3.2/src/unipolator/symmetric_unitary_interpolation_vector.c
+-rw-rw-rw-   0        0        0    14996 2023-06-23 21:07:25.000000 unipolator-0.3.2/src/unipolator/symmetric_unitary_interpolation_vector.pyx
+-rw-rw-rw-   0        0        0   980859 2023-08-07 15:59:11.000000 unipolator-0.3.2/src/unipolator/trotter_system.c
+-rw-rw-rw-   0        0        0    15625 2023-06-20 09:36:37.000000 unipolator-0.3.2/src/unipolator/trotter_system.pyx
+-rw-rw-rw-   0        0        0   992953 2023-08-07 15:59:12.000000 unipolator-0.3.2/src/unipolator/trotter_system_vector.c
+-rw-rw-rw-   0        0        0    14375 2023-06-22 14:33:15.000000 unipolator-0.3.2/src/unipolator/trotter_system_vector.pyx
+-rw-rw-rw-   0        0        0  1230559 2023-08-07 15:59:13.000000 unipolator-0.3.2/src/unipolator/unitary_interpolation.c
+-rw-rw-rw-   0        0        0    22553 2023-08-07 15:50:55.000000 unipolator-0.3.2/src/unipolator/unitary_interpolation.pyx
+-rw-rw-rw-   0        0        0  1192860 2023-08-07 15:59:15.000000 unipolator-0.3.2/src/unipolator/unitary_interpolation_vector.c
+-rw-rw-rw-   0        0        0    21804 2023-08-07 15:42:28.000000 unipolator-0.3.2/src/unipolator/unitary_interpolation_vector.pyx
+-rw-rw-rw-   0        0        0    21740 2023-05-14 14:16:58.000000 unipolator-0.3.2/src/unipolator/unitary_interpolation_vector_old.pyx
+drwxrwxrwx   0        0        0        0 2023-08-07 16:06:03.265044 unipolator-0.3.2/src/unipolator.egg-info/
+-rw-rw-rw-   0        0        0     5441 2023-08-07 16:06:02.000000 unipolator-0.3.2/src/unipolator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1779 2023-08-07 16:06:03.000000 unipolator-0.3.2/src/unipolator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 16:06:02.000000 unipolator-0.3.2/src/unipolator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 15:59:16.000000 unipolator-0.3.2/src/unipolator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       85 2023-08-07 16:06:02.000000 unipolator-0.3.2/src/unipolator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 16:06:02.000000 unipolator-0.3.2/src/unipolator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 16:06:03.138759 unipolator-0.3.2/test/
+drwxrwxrwx   0        0        0        0 2023-08-07 16:06:03.267130 unipolator-0.3.2/test/Outlook/
+-rw-rw-rw-   0        0        0     4771 2023-06-12 12:51:11.000000 unipolator-0.3.2/test/Outlook/expm_v.pyx
```

### Comparing `unipolator-0.3.0/LICENSE` & `unipolator-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/PKG-INFO` & `unipolator-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: unipolator
-Version: 0.3.0
+Version: 0.3.2
 Summary: Unipolator allows for n dimensional unitary interpolation, and the calculation of propagators using unitary interpolation. Speeds up your propagators for linear quantum systems.
 Home-page: https://github.com/Ntropic/unipolator
-Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.3.0.tar.gz
+Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.3.2.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
@@ -36,14 +36,29 @@
 Equivalently if we wish to propagate only wavevectors $\ket{\psi(t)} = U(t) \ket{\psi(0)}$ we initialize the unitary interpolation cache via
 ```
 ui_vector = UI_vector(H_s, c_mins, c_maxs, c_bins, m)  
 ```
 where `m` is the number of wavevectors that are calculated in parallel.
 The package contains further methods listed at the bottom of this document.
 
+## Automatic Binning
+The method `UI_bins` automatically calculates the optimal binning for a target infidelity (default `I_tar=1e-10`). Use via
+```
+bins = UI_bins(H_s, c_mins, c_maxs, I_tar=1e-10)
+```
+By calling 
+```
+ui = UI_auto(H_s, c_mins, c_maxs, I_tar=1e-10)
+```
+or
+```
+ui_vector = UI_vector_auto(H_s, c_mins, c_maxs, I_tar=1e-10, m)
+```
+this method is called automatically during the initialization of the unitary interpolation cache.
+
 ## Calculate:
 We can now use `ui` to calculate matrix exponentials, their derivatives, pulse sequences, and their gradients via the following methods:
 1. `expmH` calculates the unitary $U = \exp(-i H(c) \Delta t)$ for a given set of coefficients `c` (double array of length $n$), pass `U_ui` to the method to store the result (this avoids allocating new memory for every call, and allows reusing the same arrays)
     ```
     ui.expmH( c, U_ui)  
     ``` 
     Similarly we pass two $d \times m$ arrays `V_in` and `V_out`, with the $m$ input wavevectors and for the propagated wavevectors, via
```

### Comparing `unipolator-0.3.0/README.md` & `unipolator-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,29 @@
 Equivalently if we wish to propagate only wavevectors $\ket{\psi(t)} = U(t) \ket{\psi(0)}$ we initialize the unitary interpolation cache via
 ```
 ui_vector = UI_vector(H_s, c_mins, c_maxs, c_bins, m)  
 ```
 where `m` is the number of wavevectors that are calculated in parallel.
 The package contains further methods listed at the bottom of this document.
 
+## Automatic Binning
+The method `UI_bins` automatically calculates the optimal binning for a target infidelity (default `I_tar=1e-10`). Use via
+```
+bins = UI_bins(H_s, c_mins, c_maxs, I_tar=1e-10)
+```
+By calling 
+```
+ui = UI_auto(H_s, c_mins, c_maxs, I_tar=1e-10)
+```
+or
+```
+ui_vector = UI_vector_auto(H_s, c_mins, c_maxs, I_tar=1e-10, m)
+```
+this method is called automatically during the initialization of the unitary interpolation cache.
+
 ## Calculate:
 We can now use `ui` to calculate matrix exponentials, their derivatives, pulse sequences, and their gradients via the following methods:
 1. `expmH` calculates the unitary $U = \exp(-i H(c) \Delta t)$ for a given set of coefficients `c` (double array of length $n$), pass `U_ui` to the method to store the result (this avoids allocating new memory for every call, and allows reusing the same arrays)
     ```
     ui.expmH( c, U_ui)  
     ``` 
     Similarly we pass two $d \times m$ arrays `V_in` and `V_out`, with the $m$ input wavevectors and for the propagated wavevectors, via
```

### Comparing `unipolator-0.3.0/setup.cfg` & `unipolator-0.3.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6e69 706f 6c61 746f 720d 0a76   = unipolator..v
-00000020: 6572 7369 6f6e 203d 2030 2e33 2e30 0d0a  ersion = 0.3.0..
+00000020: 6572 7369 6f6e 203d 2030 2e33 2e32 0d0a  ersion = 0.3.2..
 00000030: 6175 7468 6f72 203d 204d 6963 6861 656c  author = Michael
 00000040: 2053 6368 696c 6c69 6e67 0d0a 6175 7468   Schilling..auth
 00000050: 6f72 5f65 6d61 696c 203d 206d 6963 6861  or_email = micha
 00000060: 656c 406e 7472 6f70 6963 2e64 650d 0a64  el@ntropic.de..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2055 6e69  escription = Uni
 00000080: 706f 6c61 746f 7220 616c 6c6f 7773 2066  polator allows f
 00000090: 6f72 206e 2064 696d 656e 7369 6f6e 616c  or n dimensional
@@ -25,17 +25,17 @@
 00000180: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
 00000190: 2f67 6974 6875 622e 636f 6d2f 4e74 726f  /github.com/Ntro
 000001a0: 7069 632f 756e 6970 6f6c 6174 6f72 0d0a  pic/unipolator..
 000001b0: 646f 776e 6c6f 6164 5f75 726c 203d 2068  download_url = h
 000001c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 000001d0: 6d2f 4e74 726f 7069 632f 756e 6970 6f6c  m/Ntropic/unipol
 000001e0: 6174 6f72 2f61 7263 6869 7665 2f72 6566  ator/archive/ref
-000001f0: 732f 7461 6773 2f76 302e 332e 302e 7461  s/tags/v0.3.0.ta
-00000200: 722e 677a 0d0a 5072 6f67 7261 6d6d 696e  r.gz..Programmin
-00000210: 6720 4c61 6e67 7561 6765 203d 203a 2050  g Language = : P
+000001f0: 732f 7461 6773 2f76 302e 332e 322e 7461  s/tags/v0.3.2.ta
+00000200: 722e 677a 0d0a 0950 726f 6772 616d 6d69  r.gz...Programmi
+00000210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 00000220: 7974 686f 6e20 3a3a 2033 0d0a 0950 726f  ython :: 3...Pro
 00000230: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000240: 6520 3a3a 2050 7974 686f 6e20 3a3a 2049  e :: Python :: I
 00000250: 6d70 6c65 6d65 6e74 6174 696f 6e20 3a3a  mplementation ::
 00000260: 2043 5079 7468 6f6e 0d0a 0949 6e74 656e   CPython...Inten
 00000270: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
 00000280: 5363 6965 6e63 652f 5265 7365 6172 6368  Science/Research
@@ -52,11 +52,11 @@
 00000330: 6167 6573 203d 2066 696e 643a 0d0a 0d0a  ages = find:....
 00000340: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
 00000350: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
 00000360: 2073 7263 0d0a 6578 636c 7564 6520 3d20   src..exclude = 
 00000370: 7465 7374 0d0a 0d0a 5b6f 7074 696f 6e73  test....[options
 00000380: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
 00000390: 2a20 3d20 2a2e 7078 642c 202a 2e68 2c20  * = *.pxd, *.h, 
-000003a0: 2a2e 7079 780d 0a0d 0a5b 6567 675f 696e  *.pyx....[egg_in
-000003b0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000003c0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000003d0: 0a0d 0a                                  ...
+000003a0: 2a2e 7079 782c 202a 2e70 790d 0a0d 0a5b  *.pyx, *.py....[
+000003b0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000003c0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000003d0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `unipolator-0.3.0/setup.py` & `unipolator-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,17 @@
             sources.append(sfile)
         extension.sources[:] = sources
     return extensions
 
 # make a list of the .pyx files in the os.join.path("src",name) directory
 #pyx_files = [os.path.splitext(fn)[0] for fn in os.listdir(os.path.join('src', name)) if fn.endswith(".pyx")] 
 pyx_files = ['blas_functions', 'blas_functions_vectors', 'exp_and_log', 'indexing', 'caching', 'unitary_interpolation',  'symmetric_unitary_interpolation', 'hamiltonian_system', 'trotter_system', 'sym_trotter_system']
+#pyx_files += ['autobinning']
 pyx_files += ['unitary_interpolation_vector', 'symmetric_unitary_interpolation_vector', 'trotter_system_vector', 'sym_trotter_system_vector', 'hamiltonian_system_vector']
+
 # check which operating system we are on
 # Linux?
 if os.name == 'posix':   # Linux or Mac OSX
     extra_compile_args = ["-O3", "-ffast-math", "-march=native", "-fopenmp"]
 else:  # Windows?
     extra_compile_args = ["/O2", "/openmp"]
     
@@ -58,22 +60,22 @@
 
 with open("requirements-dev.txt") as fp:
     dev_requires = fp.read().strip().split("\n")
 
 setup(   
     name = "unipolator",
     #zip_safe = False,
-    version    = "0.3.0",
+    version      = "0.3.2",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "Unipolator allows for n dimensional unitary interpolation, and the calculation of propagators using unitary interpolation. Speeds up your propagators for linear quantum systems.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/Ntropic/unipolator",
-    download_url = "https://github.com/Ntropic/unipolator/archive/refs/tags/v0.3.0.tar.gz",
+    download_url = "https://github.com/Ntropic/unipolator/archive/refs/tags/v0.3.2.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     ext_modules = extensions,
     install_requires = install_requires,
```

### Comparing `unipolator-0.3.0/src/unipolator/__init__.py` & `unipolator-0.3.2/src/unipolator/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+#from unipolator.autobinning import *
 from unipolator.hamiltonian_system import *
 
 from unipolator.unitary_interpolation import *
 from unipolator.symmetric_unitary_interpolation import *
 from unipolator.trotter_system import *
 from unipolator.sym_trotter_system import *
```

### Comparing `unipolator-0.3.0/src/unipolator/blas_functions.c` & `unipolator-0.3.2/src/unipolator/blas_functions.c`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "/O2",
             "/openmp"
         ],
         "include_dirs": [
-            "C:\\Users\\schilling\\anaconda3\\envs\\mypy\\lib\\site-packages\\numpy\\core\\include"
+            "C:\\Users\\micha\\anaconda3\\envs\\mypy\\lib\\site-packages\\numpy\\core\\include"
         ],
         "name": "unipolator.blas_functions",
         "sources": [
             "src\\unipolator\\blas_functions.pyx"
         ]
     },
     "module_name": "unipolator.blas_functions"
@@ -1240,15 +1240,15 @@
 typedef int __pyx_t_5scipy_6linalg_13cython_lapack_zselect1(__pyx_t_double_complex *);
 
 /* "scipy/linalg/cython_lapack.pxd":29
  * ctypedef bint sselect3(s*, s*, s*)
  * ctypedef bint zselect1(z*)
  * ctypedef bint zselect2(z*, z*)             # <<<<<<<<<<<<<<
  * 
- * cdef void cbbcsd(char *jobu1, char *jobu2, char *jobv1t, char *jobv2t, char *trans, int *m, int *p, int *q, s *theta, s *phi, c *u1, int *ldu1, c *u2, int *ldu2, c *v1t, int *ldv1t, c *v2t, int *ldv2t, s *b11d, s *b11e, s *b12d, s *b12e, s *b21d, s *b21e, s *b22d, s *b22e, s *rwork, int *lrwork, int *info) nogil
+ * cdef void cbbcsd(char *jobu1, char *jobu2, char *jobv1t, char *jobv2t, char *trans, int *m, int *p, int *q, s *theta, s *phi, c *u1, int *ldu1, c *u2, int *ldu2, c *v1t, int *ldv1t, c *v2t, int *ldv2t, s *b11d, s *b11e, s *b12d, s *b12e, s *b21d, s *b21e, s *b22d, s *b22e, s *rwork, int *lrwork, int *info) noexcept nogil
  */
 typedef int __pyx_t_5scipy_6linalg_13cython_lapack_zselect2(__pyx_t_double_complex *, __pyx_t_double_complex *);
 struct __pyx_ctuple_int__and_int__and_int;
 typedef struct __pyx_ctuple_int__and_int__and_int __pyx_ctuple_int__and_int__and_int;
 
 /* "unipolator/blas_functions.pxd":30
  * cdef double complex target_indexes_trace_pointer(double complex *v0, int n, int[::1] target_indexes) nogil
```

### Comparing `unipolator-0.3.0/src/unipolator/blas_functions.pxd` & `unipolator-0.3.2/src/unipolator/blas_functions.pxd`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/blas_functions.pyx` & `unipolator-0.3.2/src/unipolator/blas_functions.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/blas_functions_vectors.c` & `unipolator-0.3.2/src/unipolator/blas_functions_vectors.c`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "/O2",
             "/openmp"
         ],
         "include_dirs": [
-            "C:\\Users\\schilling\\anaconda3\\envs\\mypy\\lib\\site-packages\\numpy\\core\\include"
+            "C:\\Users\\micha\\anaconda3\\envs\\mypy\\lib\\site-packages\\numpy\\core\\include"
         ],
         "name": "unipolator.blas_functions_vectors",
         "sources": [
             "src\\unipolator\\blas_functions_vectors.pyx"
         ]
     },
     "module_name": "unipolator.blas_functions_vectors"
```

### Comparing `unipolator-0.3.0/src/unipolator/blas_functions_vectors.pxd` & `unipolator-0.3.2/src/unipolator/blas_functions_vectors.pxd`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/blas_functions_vectors.pyx` & `unipolator-0.3.2/src/unipolator/blas_functions_vectors.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/caching.c` & `unipolator-0.3.2/src/unipolator/caching.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/caching.pyx` & `unipolator-0.3.2/src/unipolator/caching.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/exp_and_log.c` & `unipolator-0.3.2/src/unipolator/exp_and_log.c`

 * *Files 0% similar despite different names*

```diff
@@ -1240,15 +1240,15 @@
 typedef int __pyx_t_5scipy_6linalg_13cython_lapack_zselect1(__pyx_t_double_complex *);
 
 /* "scipy/linalg/cython_lapack.pxd":29
  * ctypedef bint sselect3(s*, s*, s*)
  * ctypedef bint zselect1(z*)
  * ctypedef bint zselect2(z*, z*)             # <<<<<<<<<<<<<<
  * 
- * cdef void cbbcsd(char *jobu1, char *jobu2, char *jobv1t, char *jobv2t, char *trans, int *m, int *p, int *q, s *theta, s *phi, c *u1, int *ldu1, c *u2, int *ldu2, c *v1t, int *ldv1t, c *v2t, int *ldv2t, s *b11d, s *b11e, s *b12d, s *b12e, s *b21d, s *b21e, s *b22d, s *b22e, s *rwork, int *lrwork, int *info) nogil
+ * cdef void cbbcsd(char *jobu1, char *jobu2, char *jobv1t, char *jobv2t, char *trans, int *m, int *p, int *q, s *theta, s *phi, c *u1, int *ldu1, c *u2, int *ldu2, c *v1t, int *ldv1t, c *v2t, int *ldv2t, s *b11d, s *b11e, s *b12d, s *b12e, s *b21d, s *b21e, s *b22d, s *b22e, s *rwork, int *lrwork, int *info) noexcept nogil
  */
 typedef int __pyx_t_5scipy_6linalg_13cython_lapack_zselect2(__pyx_t_double_complex *, __pyx_t_double_complex *);
 struct __pyx_ctuple_int__and_int__and_int;
 typedef struct __pyx_ctuple_int__and_int__and_int __pyx_ctuple_int__and_int__and_int;
 
 /* "blas_functions.pxd":30
  * cdef double complex target_indexes_trace_pointer(double complex *v0, int n, int[::1] target_indexes) nogil
```

### Comparing `unipolator-0.3.0/src/unipolator/exp_and_log.pxd` & `unipolator-0.3.2/src/unipolator/exp_and_log.pxd`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/exp_and_log.pyx` & `unipolator-0.3.2/src/unipolator/exp_and_log.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/hamiltonian_system.c` & `unipolator-0.3.2/src/unipolator/hamiltonian_system.c`

 * *Files 0% similar despite different names*

```diff
@@ -1478,15 +1478,15 @@
 typedef int __pyx_t_5scipy_6linalg_13cython_lapack_zselect1(__pyx_t_double_complex *);
 
 /* "scipy/linalg/cython_lapack.pxd":29
  * ctypedef bint sselect3(s*, s*, s*)
  * ctypedef bint zselect1(z*)
  * ctypedef bint zselect2(z*, z*)             # <<<<<<<<<<<<<<
  * 
- * cdef void cbbcsd(char *jobu1, char *jobu2, char *jobv1t, char *jobv2t, char *trans, int *m, int *p, int *q, s *theta, s *phi, c *u1, int *ldu1, c *u2, int *ldu2, c *v1t, int *ldv1t, c *v2t, int *ldv2t, s *b11d, s *b11e, s *b12d, s *b12e, s *b21d, s *b21e, s *b22d, s *b22e, s *rwork, int *lrwork, int *info) nogil
+ * cdef void cbbcsd(char *jobu1, char *jobu2, char *jobv1t, char *jobv2t, char *trans, int *m, int *p, int *q, s *theta, s *phi, c *u1, int *ldu1, c *u2, int *ldu2, c *v1t, int *ldv1t, c *v2t, int *ldv2t, s *b11d, s *b11e, s *b12d, s *b12e, s *b21d, s *b21e, s *b22d, s *b22e, s *rwork, int *lrwork, int *info) noexcept nogil
  */
 typedef int __pyx_t_5scipy_6linalg_13cython_lapack_zselect2(__pyx_t_double_complex *, __pyx_t_double_complex *);
 struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_dexpmH_pointer;
 struct __pyx_opt_args_10unipolator_18hamiltonian_system_18Hamiltonian_System_expmH_pulse_pointer;
 
 /* "unipolator/hamiltonian_system.pyx":125
  *             u0 += self.d2
```

### Comparing `unipolator-0.3.0/src/unipolator/hamiltonian_system.pyx` & `unipolator-0.3.2/src/unipolator/hamiltonian_system.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/hamiltonian_system_vector.c` & `unipolator-0.3.2/src/unipolator/hamiltonian_system_vector.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/hamiltonian_system_vector.pyx` & `unipolator-0.3.2/src/unipolator/hamiltonian_system_vector.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/indexing.c` & `unipolator-0.3.2/src/unipolator/indexing.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/indexing.pxd` & `unipolator-0.3.2/src/unipolator/indexing.pxd`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/indexing.pyx` & `unipolator-0.3.2/src/unipolator/indexing.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/sym_trotter_system.c` & `unipolator-0.3.2/src/unipolator/sym_trotter_system.c`

 * *Files 0% similar despite different names*

```diff
@@ -1478,15 +1478,15 @@
 typedef int __pyx_t_5scipy_6linalg_13cython_lapack_zselect1(__pyx_t_double_complex *);
 
 /* "scipy/linalg/cython_lapack.pxd":29
  * ctypedef bint sselect3(s*, s*, s*)
  * ctypedef bint zselect1(z*)
  * ctypedef bint zselect2(z*, z*)             # <<<<<<<<<<<<<<
  * 
- * cdef void cbbcsd(char *jobu1, char *jobu2, char *jobv1t, char *jobv2t, char *trans, int *m, int *p, int *q, s *theta, s *phi, c *u1, int *ldu1, c *u2, int *ldu2, c *v1t, int *ldv1t, c *v2t, int *ldv2t, s *b11d, s *b11e, s *b12d, s *b12e, s *b21d, s *b21e, s *b22d, s *b22e, s *rwork, int *lrwork, int *info) nogil
+ * cdef void cbbcsd(char *jobu1, char *jobu2, char *jobv1t, char *jobv2t, char *trans, int *m, int *p, int *q, s *theta, s *phi, c *u1, int *ldu1, c *u2, int *ldu2, c *v1t, int *ldv1t, c *v2t, int *ldv2t, s *b11d, s *b11e, s *b12d, s *b12e, s *b21d, s *b21e, s *b22d, s *b22e, s *rwork, int *lrwork, int *info) noexcept nogil
  */
 typedef int __pyx_t_5scipy_6linalg_13cython_lapack_zselect2(__pyx_t_double_complex *, __pyx_t_double_complex *);
 
 /* "unipolator/sym_trotter_system.pyx":11
  * 
  * # Unitary Interpolation
  * cdef class Sym_Trotter_System:             # <<<<<<<<<<<<<<
```

### Comparing `unipolator-0.3.0/src/unipolator/sym_trotter_system.pyx` & `unipolator-0.3.2/src/unipolator/sym_trotter_system.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/sym_trotter_system_vector.c` & `unipolator-0.3.2/src/unipolator/sym_trotter_system_vector.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/sym_trotter_system_vector.pyx` & `unipolator-0.3.2/src/unipolator/sym_trotter_system_vector.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/symmetric_unitary_interpolation.c` & `unipolator-0.3.2/src/unipolator/symmetric_unitary_interpolation.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/symmetric_unitary_interpolation.pyx` & `unipolator-0.3.2/src/unipolator/symmetric_unitary_interpolation.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/symmetric_unitary_interpolation_vector.c` & `unipolator-0.3.2/src/unipolator/symmetric_unitary_interpolation_vector.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/symmetric_unitary_interpolation_vector.pyx` & `unipolator-0.3.2/src/unipolator/symmetric_unitary_interpolation_vector.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/trotter_system.c` & `unipolator-0.3.2/src/unipolator/trotter_system.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/trotter_system.pyx` & `unipolator-0.3.2/src/unipolator/trotter_system.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/trotter_system_vector.c` & `unipolator-0.3.2/src/unipolator/trotter_system_vector.c`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/trotter_system_vector.pyx` & `unipolator-0.3.2/src/unipolator/trotter_system_vector.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator/unitary_interpolation.c` & `unipolator-0.3.2/src/unipolator/unitary_interpolation.c`

 * *Files 1% similar despite different names*

```diff
@@ -2537,80 +2537,90 @@
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_H_s[] = "H_s";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
+static const char __pyx_k_long[] = "long";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ASCII[] = "ASCII";
+static const char __pyx_k_I_tar[] = "I_tar";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dI_dj[] = "dI_dj";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_arange[] = "arange";
 static const char __pyx_k_c_bins[] = "c_bins";
+static const char __pyx_k_c_maxs[] = "c_maxs";
+static const char __pyx_k_c_mins[] = "c_mins";
+static const char __pyx_k_compat[] = "compat";
 static const char __pyx_k_double[] = "double";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
+static const char __pyx_k_UI_auto[] = "UI_auto";
+static const char __pyx_k_UI_bins[] = "UI_bins";
 static const char __pyx_k_asarray[] = "asarray";
 static const char __pyx_k_c_max_s[] = "c_max_s";
 static const char __pyx_k_c_min_s[] = "c_min_s";
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_U_target[] = "U_target";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
+static const char __pyx_k_opt_bins[] = "opt_bins";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_complex128[] = "complex128";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
+static const char __pyx_k_autobinning[] = "autobinning";
 static const char __pyx_k_which_diffs[] = "which_diffs";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_target_indexes[] = "target_indexes";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
+static const char __pyx_k_optimal_binning[] = "optimal_binning";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
@@ -2641,26 +2651,30 @@
 static const char __pyx_k_The_derivative_dU_must_be_of_siz[] = "The derivative dU must be of size [d,d].";
 static const char __pyx_k_The_unitaries_U_and_U_target_mus[] = "The unitaries U and U_target must be of size [d,d].";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_Warning_These_parameters_lie_out[] = "Warning: These parameters lie outside of interpolation grid!";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
+static const char __pyx_k_self_c_self_du1_self_ei_self_ur0[] = "self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling";
+static const char __pyx_k_src_unipolator_unitary_interpola[] = "src\\unipolator\\unitary_interpolation.pyx";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
+static const char __pyx_k_unipolator_unitary_interpolation[] = "unipolator.unitary_interpolation";
 static const char __pyx_k_Inputs_must_fulfill_which_diffs_2[] = "Inputs must fulfill: which_diffs.shape[0] = cs.shape[1].";
 static const char __pyx_k_The_derivative_dU_must_be_of_siz_2[] = "The derivative dU must be of size [n_d_di,d,d].";
 static PyObject *__pyx_n_s_ASCII;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
 static PyObject *__pyx_n_s_H_s;
+static PyObject *__pyx_n_s_I_tar;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_u_Inputs_must_fulfill_cs_shape_0_d;
 static PyObject *__pyx_kp_u_Inputs_must_fulfill_which_diffs;
 static PyObject *__pyx_kp_u_Inputs_must_fulfill_which_diffs_2;
@@ -2678,31 +2692,37 @@
 static PyObject *__pyx_kp_u_The_derivative_dU_must_be_of_siz;
 static PyObject *__pyx_kp_u_The_derivative_dU_must_be_of_siz_2;
 static PyObject *__pyx_kp_u_The_unitaries_U_and_U_target_mus;
 static PyObject *__pyx_kp_u_The_unitary_U_must_be_of_size_d;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_U;
 static PyObject *__pyx_n_s_UI;
+static PyObject *__pyx_n_s_UI_auto;
+static PyObject *__pyx_n_s_UI_bins;
 static PyObject *__pyx_n_s_U_target;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_kp_u_Warning_These_parameters_lie_out;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_arange;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_asarray;
+static PyObject *__pyx_n_s_autobinning;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_n_s_c_bins;
 static PyObject *__pyx_n_s_c_max_s;
+static PyObject *__pyx_n_s_c_maxs;
 static PyObject *__pyx_n_s_c_min_s;
+static PyObject *__pyx_n_s_c_mins;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
+static PyObject *__pyx_n_s_compat;
 static PyObject *__pyx_n_s_complex128;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
 static PyObject *__pyx_n_s_cs;
 static PyObject *__pyx_n_s_dI_dj;
 static PyObject *__pyx_n_s_dU;
 static PyObject *__pyx_n_s_dict;
@@ -2719,27 +2739,30 @@
 static PyObject *__pyx_n_u_fortran;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_kp_s_got_differing_extents_in_dimensi;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
+static PyObject *__pyx_n_s_long;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_obj;
+static PyObject *__pyx_n_s_opt_bins;
+static PyObject *__pyx_n_s_optimal_binning;
 static PyObject *__pyx_n_s_pack;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_print;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
 static PyObject *__pyx_n_s_pyx_result;
@@ -2747,44 +2770,49 @@
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_Enum;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
+static PyObject *__pyx_kp_s_self_c_self_du1_self_ei_self_ur0;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_size;
+static PyObject *__pyx_kp_s_src_unipolator_unitary_interpola;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_kp_s_strided_and_direct;
 static PyObject *__pyx_kp_s_strided_and_direct_or_indirect;
 static PyObject *__pyx_kp_s_strided_and_indirect;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_target_indexes;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
+static PyObject *__pyx_n_s_unipolator_unitary_interpolation;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_which_diffs;
-static int __pyx_pf_10unipolator_21unitary_interpolation_2UI___cinit__(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_H_s, __Pyx_memviewslice __pyx_v_c_min_s, __Pyx_memviewslice __pyx_v_c_max_s, __Pyx_memviewslice __pyx_v_c_bins, __Pyx_memviewslice __pyx_v_which_diffs); /* proto */
+static int __pyx_pf_10unipolator_21unitary_interpolation_2UI___init__(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_H_s, __Pyx_memviewslice __pyx_v_c_min_s, __Pyx_memviewslice __pyx_v_c_max_s, __Pyx_memviewslice __pyx_v_c_bins, __Pyx_memviewslice __pyx_v_which_diffs); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_2set_which_diffs(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_which_diffs); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_4get_single_param(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_c); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_6get_cache(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_8expmH(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_10dexpmH(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_12expmH_pulse(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_14expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_16grape(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_U_target, __Pyx_memviewslice __pyx_v_target_indexes, __Pyx_memviewslice __pyx_v_U, __Pyx_memviewslice __pyx_v_dU, __Pyx_memviewslice __pyx_v_dI_dj); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_UI_auto(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_H_s, PyObject *__pyx_v_c_min_s, PyObject *__pyx_v_c_max_s, PyObject *__pyx_v_I_tar, PyObject *__pyx_v_which_diffs); /* proto */
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_bins(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_H_s, PyObject *__pyx_v_c_min_s, PyObject *__pyx_v_c_max_s, PyObject *__pyx_v_I_tar); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2824,36 +2852,37 @@
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_10unipolator_21unitary_interpolation_UI(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_float_1eneg_10;
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_112105877;
 static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static __Pyx_memviewslice __pyx_k_;
+static PyObject *__pyx_k__15;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_slice__31;
+static PyObject *__pyx_slice__32;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
@@ -2861,49 +2890,54 @@
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__30;
-static PyObject *__pyx_tuple__32;
+static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
 static PyObject *__pyx_tuple__35;
 static PyObject *__pyx_tuple__36;
 static PyObject *__pyx_tuple__37;
-static PyObject *__pyx_tuple__38;
 static PyObject *__pyx_tuple__39;
-static PyObject *__pyx_tuple__40;
 static PyObject *__pyx_tuple__41;
-static PyObject *__pyx_codeobj__42;
+static PyObject *__pyx_tuple__42;
+static PyObject *__pyx_tuple__43;
+static PyObject *__pyx_tuple__44;
+static PyObject *__pyx_tuple__45;
+static PyObject *__pyx_tuple__46;
+static PyObject *__pyx_codeobj__38;
+static PyObject *__pyx_codeobj__40;
+static PyObject *__pyx_codeobj__47;
 /* Late includes */
 
 /* "unipolator/unitary_interpolation.pyx":37
  *     cdef long[::1] first_elements_E, first_elements_C, L
  *     cdef long[::1] d_di
- *     def __cinit__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long)):             # <<<<<<<<<<<<<<
+ *     def __init__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long)):             # <<<<<<<<<<<<<<
  *         # Construct parameters
  *         self.n_dims = c_min_s.shape[0]
  */
 
 /* Python wrapper */
-static int __pyx_pw_10unipolator_21unitary_interpolation_2UI_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_10unipolator_21unitary_interpolation_2UI_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_10unipolator_21unitary_interpolation_2UI_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_10unipolator_21unitary_interpolation_2UI_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_H_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_c_min_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_c_max_s = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_c_bins = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_which_diffs = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
+  __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_H_s,&__pyx_n_s_c_min_s,&__pyx_n_s_c_max_s,&__pyx_n_s_c_bins,&__pyx_n_s_which_diffs,0};
     PyObject* values[5] = {0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
@@ -2925,37 +2959,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_H_s)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_min_s)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 1); __PYX_ERR(0, 37, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, 1); __PYX_ERR(0, 37, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_max_s)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 2); __PYX_ERR(0, 37, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, 2); __PYX_ERR(0, 37, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_bins)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 3); __PYX_ERR(0, 37, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, 3); __PYX_ERR(0, 37, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_which_diffs);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 37, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 37, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -2974,28 +3008,28 @@
     } else {
       __pyx_v_which_diffs = __pyx_k_;
       __PYX_INC_MEMVIEW(&__pyx_v_which_diffs, 1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 37, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 37, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("unipolator.unitary_interpolation.UI.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("unipolator.unitary_interpolation.UI.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10unipolator_21unitary_interpolation_2UI___cinit__(((struct __pyx_obj_10unipolator_21unitary_interpolation_UI *)__pyx_v_self), __pyx_v_H_s, __pyx_v_c_min_s, __pyx_v_c_max_s, __pyx_v_c_bins, __pyx_v_which_diffs);
+  __pyx_r = __pyx_pf_10unipolator_21unitary_interpolation_2UI___init__(((struct __pyx_obj_10unipolator_21unitary_interpolation_UI *)__pyx_v_self), __pyx_v_H_s, __pyx_v_c_min_s, __pyx_v_c_max_s, __pyx_v_c_bins, __pyx_v_which_diffs);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_10unipolator_21unitary_interpolation_2UI___cinit__(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_H_s, __Pyx_memviewslice __pyx_v_c_min_s, __Pyx_memviewslice __pyx_v_c_max_s, __Pyx_memviewslice __pyx_v_c_bins, __Pyx_memviewslice __pyx_v_which_diffs) {
+static int __pyx_pf_10unipolator_21unitary_interpolation_2UI___init__(struct __pyx_obj_10unipolator_21unitary_interpolation_UI *__pyx_v_self, __Pyx_memviewslice __pyx_v_H_s, __Pyx_memviewslice __pyx_v_c_min_s, __Pyx_memviewslice __pyx_v_c_max_s, __Pyx_memviewslice __pyx_v_c_bins, __Pyx_memviewslice __pyx_v_which_diffs) {
   int __pyx_v_i;
   PyObject *__pyx_v_U_grid = NULL;
   PyObject *__pyx_v_cum_prod = NULL;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -3033,18 +3067,18 @@
   __Pyx_memviewslice __pyx_t_34 = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_t_35 = { 0, 0, { 0 }, { 0 }, { 0 } };
   Py_ssize_t __pyx_t_36;
   __Pyx_memviewslice __pyx_t_37 = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__cinit__", 0);
+  __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "unipolator/unitary_interpolation.pyx":39
- *     def __cinit__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long)):
+ *     def __init__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long)):
  *         # Construct parameters
  *         self.n_dims = c_min_s.shape[0]             # <<<<<<<<<<<<<<
  *         self.n_dims_1 = self.n_dims - 1
  *         self.d = H_s.shape[1]
  */
   __pyx_v_self->n_dims = (__pyx_v_c_min_s.shape[0]);
 
@@ -4240,15 +4274,15 @@
   __pyx_v_self->L = __pyx_t_35;
   __pyx_t_35.memview = NULL;
   __pyx_t_35.data = NULL;
 
   /* "unipolator/unitary_interpolation.pyx":37
  *     cdef long[::1] first_elements_E, first_elements_C, L
  *     cdef long[::1] d_di
- *     def __cinit__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long)):             # <<<<<<<<<<<<<<
+ *     def __init__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long)):             # <<<<<<<<<<<<<<
  *         # Construct parameters
  *         self.n_dims = c_min_s.shape[0]
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
@@ -4278,15 +4312,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_t_30, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_t_31, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_t_32, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_t_33, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_t_34, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_t_35, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_t_37, 1);
-  __Pyx_AddTraceback("unipolator.unitary_interpolation.UI.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("unipolator.unitary_interpolation.UI.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_U_grid);
   __Pyx_XDECREF(__pyx_v_cum_prod);
   __PYX_XDEC_MEMVIEW(&__pyx_v_H_s, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_c_min_s, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_c_max_s, 1);
@@ -9058,14 +9092,15 @@
   }
 
   /* "unipolator/unitary_interpolation.pyx":424
  *             new_p0, p0 = p0, new_p0
  *             new_q0, q0 = q0, new_q0
  *         return I0             # <<<<<<<<<<<<<<
  * 
+ * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_6 = PyFloat_FromDouble(__pyx_v_I0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
@@ -9094,15 +9129,15 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static char __pyx_doc_10unipolator_21unitary_interpolation_2UI_18__reduce_cython__[] = "UI.__reduce_cython__(self)";
 static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
@@ -9123,27 +9158,27 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")
  */
   __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("unipolator.unitary_interpolation.UI.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -9151,17 +9186,17 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
 static char __pyx_doc_10unipolator_21unitary_interpolation_2UI_20__setstate_cython__[] = "UI.__setstate_cython__(self, __pyx_state)";
 static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_2UI_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
@@ -9180,41 +9215,411 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("unipolator.unitary_interpolation.UI.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "unipolator/unitary_interpolation.pyx":427
+ * 
+ * 
+ * def UI_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long)):             # <<<<<<<<<<<<<<
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ *     return UI(H_s, c_min_s, c_max_s, opt_bins, which_diffs)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_1UI_auto(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_21unitary_interpolation_UI_auto[] = "UI_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs=np.array([], dtype=np.compat.long))";
+static PyMethodDef __pyx_mdef_10unipolator_21unitary_interpolation_1UI_auto = {"UI_auto", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_21unitary_interpolation_1UI_auto, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_21unitary_interpolation_UI_auto};
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_1UI_auto(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_H_s = 0;
+  PyObject *__pyx_v_c_min_s = 0;
+  PyObject *__pyx_v_c_max_s = 0;
+  PyObject *__pyx_v_I_tar = 0;
+  PyObject *__pyx_v_which_diffs = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("UI_auto (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_H_s,&__pyx_n_s_c_min_s,&__pyx_n_s_c_max_s,&__pyx_n_s_I_tar,&__pyx_n_s_which_diffs,0};
+    PyObject* values[5] = {0,0,0,0,0};
+    values[3] = ((PyObject *)__pyx_float_1eneg_10);
+    values[4] = __pyx_k__15;
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_H_s)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_min_s)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("UI_auto", 0, 3, 5, 1); __PYX_ERR(0, 427, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_max_s)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("UI_auto", 0, 3, 5, 2); __PYX_ERR(0, 427, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_I_tar);
+          if (value) { values[3] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_which_diffs);
+          if (value) { values[4] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "UI_auto") < 0)) __PYX_ERR(0, 427, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_H_s = values[0];
+    __pyx_v_c_min_s = values[1];
+    __pyx_v_c_max_s = values[2];
+    __pyx_v_I_tar = values[3];
+    __pyx_v_which_diffs = values[4];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("UI_auto", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 427, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("unipolator.unitary_interpolation.UI_auto", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_10unipolator_21unitary_interpolation_UI_auto(__pyx_self, __pyx_v_H_s, __pyx_v_c_min_s, __pyx_v_c_max_s, __pyx_v_I_tar, __pyx_v_which_diffs);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_UI_auto(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_H_s, PyObject *__pyx_v_c_min_s, PyObject *__pyx_v_c_max_s, PyObject *__pyx_v_I_tar, PyObject *__pyx_v_which_diffs) {
+  PyObject *__pyx_v_opt_bins = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("UI_auto", 0);
+
+  /* "unipolator/unitary_interpolation.pyx":428
+ * 
+ * def UI_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long)):
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)             # <<<<<<<<<<<<<<
+ *     return UI(H_s, c_min_s, c_max_s, opt_bins, which_diffs)
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_optimal_binning); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_v_H_s);
+  __Pyx_GIVEREF(__pyx_v_H_s);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_H_s);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_c_mins, __pyx_v_c_min_s) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_c_maxs, __pyx_v_c_max_s) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_I_tar, __pyx_v_I_tar) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_opt_bins = __pyx_t_4;
+  __pyx_t_4 = 0;
+
+  /* "unipolator/unitary_interpolation.pyx":429
+ * def UI_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long)):
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ *     return UI(H_s, c_min_s, c_max_s, opt_bins, which_diffs)             # <<<<<<<<<<<<<<
+ * 
+ * def UI_bins(H_s, c_min_s, c_max_s, I_tar=1e-10):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_INCREF(__pyx_v_H_s);
+  __Pyx_GIVEREF(__pyx_v_H_s);
+  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_H_s);
+  __Pyx_INCREF(__pyx_v_c_min_s);
+  __Pyx_GIVEREF(__pyx_v_c_min_s);
+  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_c_min_s);
+  __Pyx_INCREF(__pyx_v_c_max_s);
+  __Pyx_GIVEREF(__pyx_v_c_max_s);
+  PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_v_c_max_s);
+  __Pyx_INCREF(__pyx_v_opt_bins);
+  __Pyx_GIVEREF(__pyx_v_opt_bins);
+  PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_v_opt_bins);
+  __Pyx_INCREF(__pyx_v_which_diffs);
+  __Pyx_GIVEREF(__pyx_v_which_diffs);
+  PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_v_which_diffs);
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10unipolator_21unitary_interpolation_UI), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* "unipolator/unitary_interpolation.pyx":427
+ * 
+ * 
+ * def UI_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long)):             # <<<<<<<<<<<<<<
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ *     return UI(H_s, c_min_s, c_max_s, opt_bins, which_diffs)
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("unipolator.unitary_interpolation.UI_auto", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_opt_bins);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "unipolator/unitary_interpolation.pyx":431
+ *     return UI(H_s, c_min_s, c_max_s, opt_bins, which_diffs)
+ * 
+ * def UI_bins(H_s, c_min_s, c_max_s, I_tar=1e-10):             # <<<<<<<<<<<<<<
+ *     return optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_3UI_bins(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_21unitary_interpolation_2UI_bins[] = "UI_bins(H_s, c_min_s, c_max_s, I_tar=1e-10)";
+static PyMethodDef __pyx_mdef_10unipolator_21unitary_interpolation_3UI_bins = {"UI_bins", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_21unitary_interpolation_3UI_bins, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_21unitary_interpolation_2UI_bins};
+static PyObject *__pyx_pw_10unipolator_21unitary_interpolation_3UI_bins(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_H_s = 0;
+  PyObject *__pyx_v_c_min_s = 0;
+  PyObject *__pyx_v_c_max_s = 0;
+  PyObject *__pyx_v_I_tar = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("UI_bins (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_H_s,&__pyx_n_s_c_min_s,&__pyx_n_s_c_max_s,&__pyx_n_s_I_tar,0};
+    PyObject* values[4] = {0,0,0,0};
+    values[3] = ((PyObject *)__pyx_float_1eneg_10);
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_H_s)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_min_s)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("UI_bins", 0, 3, 4, 1); __PYX_ERR(0, 431, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_max_s)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("UI_bins", 0, 3, 4, 2); __PYX_ERR(0, 431, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_I_tar);
+          if (value) { values[3] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "UI_bins") < 0)) __PYX_ERR(0, 431, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_H_s = values[0];
+    __pyx_v_c_min_s = values[1];
+    __pyx_v_c_max_s = values[2];
+    __pyx_v_I_tar = values[3];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("UI_bins", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 431, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("unipolator.unitary_interpolation.UI_bins", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_10unipolator_21unitary_interpolation_2UI_bins(__pyx_self, __pyx_v_H_s, __pyx_v_c_min_s, __pyx_v_c_max_s, __pyx_v_I_tar);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10unipolator_21unitary_interpolation_2UI_bins(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_H_s, PyObject *__pyx_v_c_min_s, PyObject *__pyx_v_c_max_s, PyObject *__pyx_v_I_tar) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("UI_bins", 0);
+
+  /* "unipolator/unitary_interpolation.pyx":432
+ * 
+ * def UI_bins(H_s, c_min_s, c_max_s, I_tar=1e-10):
+ *     return optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_optimal_binning); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_v_H_s);
+  __Pyx_GIVEREF(__pyx_v_H_s);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_H_s);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_c_mins, __pyx_v_c_min_s) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_c_maxs, __pyx_v_c_max_s) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_I_tar, __pyx_v_I_tar) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_4;
+  __pyx_t_4 = 0;
+  goto __pyx_L0;
+
+  /* "unipolator/unitary_interpolation.pyx":431
+ *     return UI(H_s, c_min_s, c_max_s, opt_bins, which_diffs)
+ * 
+ * def UI_bins(H_s, c_min_s, c_max_s, I_tar=1e-10):             # <<<<<<<<<<<<<<
+ *     return optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("unipolator.unitary_interpolation.UI_bins", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
@@ -9739,15 +10144,15 @@
       /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -9871,15 +10276,15 @@
       /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -10003,15 +10408,15 @@
       /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -10427,15 +10832,15 @@
     /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 134, __pyx_L1_error)
 
     /* "View.MemoryView":133
  *         self.itemsize = itemsize
@@ -10459,15 +10864,15 @@
     /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 137, __pyx_L1_error)
 
     /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -10586,15 +10991,15 @@
     /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 149, __pyx_L1_error)
 
     /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
@@ -10860,15 +11265,15 @@
       /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(1, 177, __pyx_L1_error)
 
       /* "View.MemoryView":176
  * 
@@ -11104,15 +11509,15 @@
     /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 193, __pyx_L1_error)
 
     /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
@@ -11838,15 +12243,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -11894,15 +12299,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -13623,15 +14028,15 @@
     /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 420, __pyx_L1_error)
 
     /* "View.MemoryView":419
  * 
@@ -14671,15 +15076,15 @@
       /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(1, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -15033,15 +15438,15 @@
     /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 522, __pyx_L1_error)
 
     /* "View.MemoryView":521
  *     @cname('getbuffer')
@@ -15582,15 +15987,15 @@
     /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 572, __pyx_L1_error)
 
     /* "View.MemoryView":570
  *     @property
@@ -15699,15 +16104,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__28, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__29, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":578
@@ -16737,15 +17142,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -16793,15 +17198,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -17150,17 +17555,17 @@
  *             else:
  */
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice__31);
-            __Pyx_GIVEREF(__pyx_slice__31);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__31);
+            __Pyx_INCREF(__pyx_slice__32);
+            __Pyx_GIVEREF(__pyx_slice__32);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__32);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":685
  *             if not seen_ellipsis:
@@ -17185,15 +17590,15 @@
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__31); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__32); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -17325,17 +17730,17 @@
  * 
  *     return have_slices or nslices, tuple(result)
  */
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice__31);
-        __Pyx_GIVEREF(__pyx_slice__31);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__31);
+        __Pyx_INCREF(__pyx_slice__32);
+        __Pyx_GIVEREF(__pyx_slice__32);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__32);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":697
  * 
@@ -17454,15 +17859,15 @@
       /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(1, 705, __pyx_L1_error)
 
       /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -19638,15 +20043,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -19694,15 +20099,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -22971,15 +23376,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__35, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__36, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
@@ -23266,15 +23671,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static struct __pyx_vtabstruct_10unipolator_21unitary_interpolation_UI __pyx_vtable_10unipolator_21unitary_interpolation_UI;
 
-static PyObject *__pyx_tp_new_10unipolator_21unitary_interpolation_UI(PyTypeObject *t, PyObject *a, PyObject *k) {
+static PyObject *__pyx_tp_new_10unipolator_21unitary_interpolation_UI(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_10unipolator_21unitary_interpolation_UI *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
@@ -23335,19 +23740,15 @@
   p->first_elements_E.memview = NULL;
   p->first_elements_C.data = NULL;
   p->first_elements_C.memview = NULL;
   p->L.data = NULL;
   p->L.memview = NULL;
   p->d_di.data = NULL;
   p->d_di.memview = NULL;
-  if (unlikely(__pyx_pw_10unipolator_21unitary_interpolation_2UI_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
-  bad:
-  Py_DECREF(o); o = 0;
-  return NULL;
 }
 
 static void __pyx_tp_dealloc_10unipolator_21unitary_interpolation_UI(PyObject *o) {
   struct __pyx_obj_10unipolator_21unitary_interpolation_UI *p = (struct __pyx_obj_10unipolator_21unitary_interpolation_UI *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
@@ -23426,30 +23827,30 @@
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
-  0, /*tp_doc*/
+  "UI(double complex[:, :, ::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs=np.array([], dtype=long))", /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_10unipolator_21unitary_interpolation_UI, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
-  0, /*tp_init*/
+  __pyx_pw_10unipolator_21unitary_interpolation_2UI_1__init__, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_10unipolator_21unitary_interpolation_UI, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
@@ -24249,14 +24650,15 @@
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
   {&__pyx_n_s_H_s, __pyx_k_H_s, sizeof(__pyx_k_H_s), 0, 0, 1, 1},
+  {&__pyx_n_s_I_tar, __pyx_k_I_tar, sizeof(__pyx_k_I_tar), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_u_Inputs_must_fulfill_cs_shape_0_d, __pyx_k_Inputs_must_fulfill_cs_shape_0_d, sizeof(__pyx_k_Inputs_must_fulfill_cs_shape_0_d), 0, 1, 0, 0},
   {&__pyx_kp_u_Inputs_must_fulfill_which_diffs, __pyx_k_Inputs_must_fulfill_which_diffs, sizeof(__pyx_k_Inputs_must_fulfill_which_diffs), 0, 1, 0, 0},
   {&__pyx_kp_u_Inputs_must_fulfill_which_diffs_2, __pyx_k_Inputs_must_fulfill_which_diffs_2, sizeof(__pyx_k_Inputs_must_fulfill_which_diffs_2), 0, 1, 0, 0},
@@ -24274,31 +24676,37 @@
   {&__pyx_kp_u_The_derivative_dU_must_be_of_siz, __pyx_k_The_derivative_dU_must_be_of_siz, sizeof(__pyx_k_The_derivative_dU_must_be_of_siz), 0, 1, 0, 0},
   {&__pyx_kp_u_The_derivative_dU_must_be_of_siz_2, __pyx_k_The_derivative_dU_must_be_of_siz_2, sizeof(__pyx_k_The_derivative_dU_must_be_of_siz_2), 0, 1, 0, 0},
   {&__pyx_kp_u_The_unitaries_U_and_U_target_mus, __pyx_k_The_unitaries_U_and_U_target_mus, sizeof(__pyx_k_The_unitaries_U_and_U_target_mus), 0, 1, 0, 0},
   {&__pyx_kp_u_The_unitary_U_must_be_of_size_d, __pyx_k_The_unitary_U_must_be_of_size_d, sizeof(__pyx_k_The_unitary_U_must_be_of_size_d), 0, 1, 0, 0},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_U, __pyx_k_U, sizeof(__pyx_k_U), 0, 0, 1, 1},
   {&__pyx_n_s_UI, __pyx_k_UI, sizeof(__pyx_k_UI), 0, 0, 1, 1},
+  {&__pyx_n_s_UI_auto, __pyx_k_UI_auto, sizeof(__pyx_k_UI_auto), 0, 0, 1, 1},
+  {&__pyx_n_s_UI_bins, __pyx_k_UI_bins, sizeof(__pyx_k_UI_bins), 0, 0, 1, 1},
   {&__pyx_n_s_U_target, __pyx_k_U_target, sizeof(__pyx_k_U_target), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_kp_u_Warning_These_parameters_lie_out, __pyx_k_Warning_These_parameters_lie_out, sizeof(__pyx_k_Warning_These_parameters_lie_out), 0, 1, 0, 0},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_arange, __pyx_k_arange, sizeof(__pyx_k_arange), 0, 0, 1, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_asarray, __pyx_k_asarray, sizeof(__pyx_k_asarray), 0, 0, 1, 1},
+  {&__pyx_n_s_autobinning, __pyx_k_autobinning, sizeof(__pyx_k_autobinning), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_n_s_c_bins, __pyx_k_c_bins, sizeof(__pyx_k_c_bins), 0, 0, 1, 1},
   {&__pyx_n_s_c_max_s, __pyx_k_c_max_s, sizeof(__pyx_k_c_max_s), 0, 0, 1, 1},
+  {&__pyx_n_s_c_maxs, __pyx_k_c_maxs, sizeof(__pyx_k_c_maxs), 0, 0, 1, 1},
   {&__pyx_n_s_c_min_s, __pyx_k_c_min_s, sizeof(__pyx_k_c_min_s), 0, 0, 1, 1},
+  {&__pyx_n_s_c_mins, __pyx_k_c_mins, sizeof(__pyx_k_c_mins), 0, 0, 1, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+  {&__pyx_n_s_compat, __pyx_k_compat, sizeof(__pyx_k_compat), 0, 0, 1, 1},
   {&__pyx_n_s_complex128, __pyx_k_complex128, sizeof(__pyx_k_complex128), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
   {&__pyx_n_s_cs, __pyx_k_cs, sizeof(__pyx_k_cs), 0, 0, 1, 1},
   {&__pyx_n_s_dI_dj, __pyx_k_dI_dj, sizeof(__pyx_k_dI_dj), 0, 0, 1, 1},
   {&__pyx_n_s_dU, __pyx_k_dU, sizeof(__pyx_k_dU), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
@@ -24315,27 +24723,30 @@
   {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 0, 1, 0},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
+  {&__pyx_n_s_long, __pyx_k_long, sizeof(__pyx_k_long), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
+  {&__pyx_n_s_opt_bins, __pyx_k_opt_bins, sizeof(__pyx_k_opt_bins), 0, 0, 1, 1},
+  {&__pyx_n_s_optimal_binning, __pyx_k_optimal_binning, sizeof(__pyx_k_optimal_binning), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_print, __pyx_k_print, sizeof(__pyx_k_print), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
@@ -24343,30 +24754,33 @@
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
+  {&__pyx_kp_s_self_c_self_du1_self_ei_self_ur0, __pyx_k_self_c_self_du1_self_ei_self_ur0, sizeof(__pyx_k_self_c_self_du1_self_ei_self_ur0), 0, 0, 1, 0},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
+  {&__pyx_kp_s_src_unipolator_unitary_interpola, __pyx_k_src_unipolator_unitary_interpola, sizeof(__pyx_k_src_unipolator_unitary_interpola), 0, 0, 1, 0},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_kp_s_strided_and_direct, __pyx_k_strided_and_direct, sizeof(__pyx_k_strided_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_direct_or_indirect, __pyx_k_strided_and_direct_or_indirect, sizeof(__pyx_k_strided_and_direct_or_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_target_indexes, __pyx_k_target_indexes, sizeof(__pyx_k_target_indexes), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
+  {&__pyx_n_s_unipolator_unitary_interpolation, __pyx_k_unipolator_unitary_interpolation, sizeof(__pyx_k_unipolator_unitary_interpolation), 0, 0, 1, 1},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_which_diffs, __pyx_k_which_diffs, sizeof(__pyx_k_which_diffs), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 44, __pyx_L1_error)
@@ -24507,321 +24921,346 @@
  */
   __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_The_derivative_dU_must_be_of_siz_2); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 387, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_self_c_self_du1_self_ei_self_ur0); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "(tree fragment)":4
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
+ *     raise TypeError("self.c,self.du1,self.ei,self.ur0,self.ur1,self.ur2,self.ur3,self.ur4,self.ur5,self.vl,self.vr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_self_c_self_du1_self_ei_self_ur0); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 944, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 950, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 522, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 572, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__28 = PyTuple_New(1); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 579, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
+  __pyx_tuple__29 = PyTuple_New(1); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__28, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__28);
+  PyTuple_SET_ITEM(__pyx_tuple__29, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__29);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__31 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__31)) __PYX_ERR(1, 684, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__31);
-  __Pyx_GIVEREF(__pyx_slice__31);
+  __pyx_slice__32 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__32)) __PYX_ERR(1, 684, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__32);
+  __Pyx_GIVEREF(__pyx_slice__32);
 
   /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_tuple__35 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_tuple__36 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
+
+  /* "unipolator/unitary_interpolation.pyx":427
+ * 
+ * 
+ * def UI_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long)):             # <<<<<<<<<<<<<<
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ *     return UI(H_s, c_min_s, c_max_s, opt_bins, which_diffs)
+ */
+  __pyx_tuple__37 = PyTuple_Pack(6, __pyx_n_s_H_s, __pyx_n_s_c_min_s, __pyx_n_s_c_max_s, __pyx_n_s_I_tar, __pyx_n_s_which_diffs, __pyx_n_s_opt_bins); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(5, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_unipolator_unitary_interpola, __pyx_n_s_UI_auto, 427, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 427, __pyx_L1_error)
+
+  /* "unipolator/unitary_interpolation.pyx":431
+ *     return UI(H_s, c_min_s, c_max_s, opt_bins, which_diffs)
+ * 
+ * def UI_bins(H_s, c_min_s, c_max_s, I_tar=1e-10):             # <<<<<<<<<<<<<<
+ *     return optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ * 
+ */
+  __pyx_tuple__39 = PyTuple_Pack(4, __pyx_n_s_H_s, __pyx_n_s_c_min_s, __pyx_n_s_c_max_s, __pyx_n_s_I_tar); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 431, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_unipolator_unitary_interpola, __pyx_n_s_UI_bins, 431, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 431, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_tuple__41 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__37);
-  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_tuple__42 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__42);
+  __Pyx_GIVEREF(__pyx_tuple__42);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(1, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__38);
-  __Pyx_GIVEREF(__pyx_tuple__38);
+  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__39);
-  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_tuple__44 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__44);
+  __Pyx_GIVEREF(__pyx_tuple__44);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(1, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__40);
-  __Pyx_GIVEREF(__pyx_tuple__40);
+  __pyx_tuple__45 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__45);
+  __Pyx_GIVEREF(__pyx_tuple__45);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__41 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__41);
-  __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__46 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__46);
+  __Pyx_GIVEREF(__pyx_tuple__46);
+  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_float_1eneg_10 = PyFloat_FromDouble(1e-10); if (unlikely(!__pyx_float_1eneg_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -25140,15 +25579,16 @@
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_memviewslice __pyx_t_5 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  static PyThread_type_lock __pyx_t_6[8];
+  PyObject *__pyx_t_6 = NULL;
+  static PyThread_type_lock __pyx_t_7[8];
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -25257,139 +25697,216 @@
  * from libc.math cimport fabs
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
+  /* "unipolator/unitary_interpolation.pyx":9
+ * from .caching cimport *
+ * from .blas_functions cimport *
+ * from .autobinning import optimal_binning             # <<<<<<<<<<<<<<
+ * 
+ * # Unitary Interpolation
+ */
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_n_s_optimal_binning);
+  __Pyx_GIVEREF(__pyx_n_s_optimal_binning);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_optimal_binning);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_autobinning, __pyx_t_1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_optimal_binning); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_optimal_binning, __pyx_t_1) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
   /* "unipolator/unitary_interpolation.pyx":37
  *     cdef long[::1] first_elements_E, first_elements_C, L
  *     cdef long[::1] d_di
- *     def __cinit__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long)):             # <<<<<<<<<<<<<<
+ *     def __init__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long)):             # <<<<<<<<<<<<<<
  *         # Construct parameters
  *         self.n_dims = c_min_s.shape[0]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_k_ = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
+  /* "unipolator/unitary_interpolation.pyx":427
+ * 
+ * 
+ * def UI_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long)):             # <<<<<<<<<<<<<<
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ *     return UI(H_s, c_min_s, c_max_s, opt_bins, which_diffs)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_compat); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_long); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_k__15 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10unipolator_21unitary_interpolation_1UI_auto, NULL, __pyx_n_s_unipolator_unitary_interpolation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UI_auto, __pyx_t_1) < 0) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "unipolator/unitary_interpolation.pyx":431
+ *     return UI(H_s, c_min_s, c_max_s, opt_bins, which_diffs)
+ * 
+ * def UI_bins(H_s, c_min_s, c_max_s, I_tar=1e-10):             # <<<<<<<<<<<<<<
+ *     return optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ * 
+ */
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10unipolator_21unitary_interpolation_3UI_bins, NULL, __pyx_n_s_unipolator_unitary_interpolation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 431, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UI_bins, __pyx_t_1) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
   /* "unipolator/unitary_interpolation.pyx":1
  * #cython: language_level=3             # <<<<<<<<<<<<<<
  * import numpy as np
  * cimport numpy as npc
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_4) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "View.MemoryView":210
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(array self):
  */
-  __pyx_t_4 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_4) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_array_type);
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__41, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
-  __Pyx_DECREF_SET(generic, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
+  __Pyx_DECREF_SET(generic, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__42, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
-  __Pyx_DECREF_SET(strided, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
+  __Pyx_DECREF_SET(strided, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__43, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
-  __Pyx_DECREF_SET(indirect, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
+  __Pyx_DECREF_SET(indirect, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__44, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
-  __Pyx_DECREF_SET(contiguous, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
+  __Pyx_DECREF_SET(contiguous, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__45, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
-  __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
+  __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":317
  * 
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0             # <<<<<<<<<<<<<<
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [
  *     PyThread_allocate_lock(),
@@ -25399,59 +25916,59 @@
   /* "View.MemoryView":318
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [             # <<<<<<<<<<<<<<
  *     PyThread_allocate_lock(),
  *     PyThread_allocate_lock(),
  */
-  __pyx_t_6[0] = PyThread_allocate_lock();
-  __pyx_t_6[1] = PyThread_allocate_lock();
-  __pyx_t_6[2] = PyThread_allocate_lock();
-  __pyx_t_6[3] = PyThread_allocate_lock();
-  __pyx_t_6[4] = PyThread_allocate_lock();
-  __pyx_t_6[5] = PyThread_allocate_lock();
-  __pyx_t_6[6] = PyThread_allocate_lock();
-  __pyx_t_6[7] = PyThread_allocate_lock();
-  memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_6, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
+  __pyx_t_7[0] = PyThread_allocate_lock();
+  __pyx_t_7[1] = PyThread_allocate_lock();
+  __pyx_t_7[2] = PyThread_allocate_lock();
+  __pyx_t_7[3] = PyThread_allocate_lock();
+  __pyx_t_7[4] = PyThread_allocate_lock();
+  __pyx_t_7[5] = PyThread_allocate_lock();
+  __pyx_t_7[6] = PyThread_allocate_lock();
+  __pyx_t_7[7] = PyThread_allocate_lock();
+  memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_7, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
 
   /* "View.MemoryView":551
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 551, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_4) < 0) __PYX_ERR(1, 551, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 551, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 551, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryview_type);
 
   /* "View.MemoryView":997
  *         return self.from_object
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 997, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_4) < 0) __PYX_ERR(1, 997, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 997, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 997, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryviewslice_type);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum, NULL, __pyx_n_s_View_MemoryView); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Enum, __pyx_t_4) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum, NULL, __pyx_n_s_View_MemoryView); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Enum, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.name = __pyx_state[0]
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
@@ -25462,14 +25979,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __PYX_XDEC_MEMVIEW(&__pyx_t_5, 1);
+  __Pyx_XDECREF(__pyx_t_6);
   if (__pyx_m) {
     if (__pyx_d) {
       __Pyx_AddTraceback("init unipolator.unitary_interpolation", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init unipolator.unitary_interpolation");
```

### Comparing `unipolator-0.3.0/src/unipolator/unitary_interpolation.pyx` & `unipolator-0.3.2/src/unipolator/unitary_interpolation.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 cimport numpy as npc
 from libc.math cimport fabs
 from .exp_and_log cimport *
 from .indexing cimport *
 from .caching cimport *
 from .blas_functions cimport *
-
+from .autobinning import optimal_binning
 
 # Unitary Interpolation
 cdef class UI:
     # Initialize variables, to quickly calculate interpolations while minimizing memmory allocation overheads
     cdef double[::1] c_mins, c_maxs, dcs, das
     cdef long[::1] c_bins
     cdef int n_dims, d, d2, n_dims_1, n_d_di_1, n_d_di
@@ -30,15 +30,15 @@
     cdef double complex *du1
     cdef long[::1] strides_L, strides_R,
     cdef long[:,::1] strides_E, strides_C
     cdef long[::1] location, d_location
     cdef double[::1] abs_alpha_rest, alpha
     cdef long[::1] first_elements_E, first_elements_C, L
     cdef long[::1] d_di
-    def __cinit__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long)):
+    def __init__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long)):
         # Construct parameters
         self.n_dims = c_min_s.shape[0]
         self.n_dims_1 = self.n_dims - 1
         self.d = H_s.shape[1]
         self.d2 = self.d * self.d
         if not H_s.shape[0] == self.n_dims + 1:
             print('Requires n+1 Hamiltonians for n dimensional interpolation. Check lenths of Hs, c_mins, c_maxs, c_bins')
@@ -419,7 +419,15 @@
             # flip pointers
             self.ur0, self.ur4 = self.ur4, self.ur0
             self.ur1, self.ur5 = self.ur5, self.ur1
             new_p0, p0 = p0, new_p0
             new_q0, q0 = q0, new_q0
         return I0
 
+
+def UI_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long)):
+    opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+    return UI(H_s, c_min_s, c_max_s, opt_bins, which_diffs)
+
+def UI_bins(H_s, c_min_s, c_max_s, I_tar=1e-10):
+    return optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+
```

### Comparing `unipolator-0.3.0/src/unipolator/unitary_interpolation_vector.c` & `unipolator-0.3.2/src/unipolator/unitary_interpolation_vector.c`

 * *Files 0% similar despite different names*

```diff
@@ -1393,15 +1393,15 @@
  */
 struct __pyx_ctuple_int__and_int__and_int {
   int f0;
   int f1;
   int f2;
 };
 
-/* "unipolator/unitary_interpolation_vector.pyx":13
+/* "unipolator/unitary_interpolation_vector.pyx":14
  * 
  * # Unitary Interpolation
  * cdef class UI_vector:             # <<<<<<<<<<<<<<
  *     # Initialize variables, to quickly calculate interpolations while minimizing memmory allocation overheads
  *     cdef double[::1] c_mins, c_maxs, dcs, das
  */
 struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector {
@@ -1528,15 +1528,15 @@
   PyObject *from_object;
   PyObject *(*to_object_func)(char *);
   int (*to_dtype_func)(char *, PyObject *);
 };
 
 
 
-/* "unipolator/unitary_interpolation_vector.pyx":13
+/* "unipolator/unitary_interpolation_vector.pyx":14
  * 
  * # Unitary Interpolation
  * cdef class UI_vector:             # <<<<<<<<<<<<<<
  *     # Initialize variables, to quickly calculate interpolations while minimizing memmory allocation overheads
  *     cdef double[::1] c_mins, c_maxs, dcs, das
  */
 
@@ -2533,38 +2533,43 @@
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_H_s[] = "H_s";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_V_in[] = "V_in";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
+static const char __pyx_k_long[] = "long";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ASCII[] = "ASCII";
+static const char __pyx_k_I_tar[] = "I_tar";
 static const char __pyx_k_V_out[] = "V_out";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_arange[] = "arange";
 static const char __pyx_k_c_bins[] = "c_bins";
+static const char __pyx_k_c_maxs[] = "c_maxs";
+static const char __pyx_k_c_mins[] = "c_mins";
+static const char __pyx_k_compat[] = "compat";
 static const char __pyx_k_double[] = "double";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
@@ -2576,14 +2581,15 @@
 static const char __pyx_k_c_min_s[] = "c_min_s";
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_change_m[] = "change_m";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
+static const char __pyx_k_opt_bins[] = "opt_bins";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_UI_vector[] = "UI_vector";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
@@ -2591,22 +2597,25 @@
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_complex128[] = "complex128";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
+static const char __pyx_k_autobinning[] = "autobinning";
 static const char __pyx_k_which_diffs[] = "which_diffs";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_UI_vector_auto[] = "UI_vector_auto";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
+static const char __pyx_k_optimal_binning[] = "optimal_binning";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
@@ -2641,26 +2650,29 @@
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_V_in_shape_0_needs_to_be_equal_t[] = "V_in.shape[0] needs to be equal to H_s[0].shape[0].";
 static const char __pyx_k_Warning_These_parameters_lie_out[] = "Warning: These parameters lie outside of interpolation grid!";
 static const char __pyx_k_c_shape_0_needs_to_be_equal_to_H[] = "c.shape[0] needs to be equal to H_s[0].shape[0]-1.";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
+static const char __pyx_k_src_unipolator_unitary_interpola[] = "src\\unipolator\\unitary_interpolation_vector.pyx";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
+static const char __pyx_k_unipolator_unitary_interpolation[] = "unipolator.unitary_interpolation_vector";
 static const char __pyx_k_The_input_derivative_vector_must_2[] = "The input derivative vector must have the same number of columns as the input and output vectors, and equal to m.";
 static const char __pyx_k_The_input_derivative_vector_must_3[] = "The input derivative vector must have the same number of rows as the number of derivatives to calculate.";
 static PyObject *__pyx_n_s_ASCII;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
 static PyObject *__pyx_n_s_H_s;
+static PyObject *__pyx_n_s_I_tar;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_u_Inputs_must_fulfill_which_diffs;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
@@ -2677,37 +2689,42 @@
 static PyObject *__pyx_kp_u_The_input_derivative_vector_must;
 static PyObject *__pyx_kp_u_The_input_derivative_vector_must_2;
 static PyObject *__pyx_kp_u_The_input_derivative_vector_must_3;
 static PyObject *__pyx_kp_u_The_input_vector_must_be_of_size;
 static PyObject *__pyx_kp_u_The_output_vector_must_be_of_siz;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_UI_vector;
+static PyObject *__pyx_n_s_UI_vector_auto;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_V_in;
 static PyObject *__pyx_kp_u_V_in_shape_0_needs_to_be_equal_t;
 static PyObject *__pyx_n_s_V_out;
 static PyObject *__pyx_kp_u_V_out_shape_0_needs_to_be_equal;
 static PyObject *__pyx_kp_u_V_out_shape_1_needs_to_be_equal;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_kp_u_Warning_These_parameters_lie_out;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_arange;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_asarray;
+static PyObject *__pyx_n_s_autobinning;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_n_s_c_bins;
 static PyObject *__pyx_n_s_c_max_s;
+static PyObject *__pyx_n_s_c_maxs;
 static PyObject *__pyx_n_s_c_min_s;
+static PyObject *__pyx_n_s_c_mins;
 static PyObject *__pyx_kp_u_c_shape_0_needs_to_be_equal_to_H;
 static PyObject *__pyx_n_s_change_m;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
+static PyObject *__pyx_n_s_compat;
 static PyObject *__pyx_n_s_complex128;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
 static PyObject *__pyx_n_s_cs;
 static PyObject *__pyx_n_s_dU;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_double;
@@ -2723,28 +2740,31 @@
 static PyObject *__pyx_n_u_fortran;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_kp_s_got_differing_extents_in_dimensi;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
+static PyObject *__pyx_n_s_long;
 static PyObject *__pyx_n_s_m;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_obj;
+static PyObject *__pyx_n_s_opt_bins;
+static PyObject *__pyx_n_s_optimal_binning;
 static PyObject *__pyx_n_s_pack;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_print;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
 static PyObject *__pyx_n_s_pyx_result;
@@ -2756,39 +2776,42 @@
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_size;
+static PyObject *__pyx_kp_s_src_unipolator_unitary_interpola;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_kp_s_strided_and_direct;
 static PyObject *__pyx_kp_s_strided_and_direct_or_indirect;
 static PyObject *__pyx_kp_s_strided_and_indirect;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
+static PyObject *__pyx_n_s_unipolator_unitary_interpolation;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_which_diffs;
 static int __pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector___cinit__(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self, __Pyx_memviewslice __pyx_v_H_s, __Pyx_memviewslice __pyx_v_c_min_s, __Pyx_memviewslice __pyx_v_c_max_s, __Pyx_memviewslice __pyx_v_c_bins, __Pyx_memviewslice __pyx_v_which_diffs, int __pyx_v_m); /* proto */
 static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_2change_m(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self, int __pyx_v_m); /* proto */
 static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_4set_which_diffs(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self, __Pyx_memviewslice __pyx_v_which_diffs); /* proto */
 static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_6get_single_param(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self, __Pyx_memviewslice __pyx_v_c); /* proto */
 static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_8get_cache(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_10expmH(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_V_in, __Pyx_memviewslice __pyx_v_V_out); /* proto */
 static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_12dexpmH(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self, __Pyx_memviewslice __pyx_v_c, __Pyx_memviewslice __pyx_v_V_in, __Pyx_memviewslice __pyx_v_V_out, __Pyx_memviewslice __pyx_v_dU); /* proto */
 static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_14expmH_pulse(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_V_in, __Pyx_memviewslice __pyx_v_V_out); /* proto */
 static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_16expmH_pulse_no_multiply(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self, __Pyx_memviewslice __pyx_v_cs, __Pyx_memviewslice __pyx_v_V_in, __Pyx_memviewslice __pyx_v_V_out); /* proto */
 static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_UI_vector_auto(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_H_s, PyObject *__pyx_v_c_min_s, PyObject *__pyx_v_c_max_s, PyObject *__pyx_v_I_tar, PyObject *__pyx_v_which_diffs, CYTHON_UNUSED PyObject *__pyx_v_m); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2828,40 +2851,41 @@
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_10unipolator_28unitary_interpolation_vector_UI_vector(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_float_1eneg_10;
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_112105877;
 static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static __Pyx_memviewslice __pyx_k_;
+static PyObject *__pyx_k__19;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_slice__35;
+static PyObject *__pyx_slice__36;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
@@ -2869,28 +2893,31 @@
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__30;
 static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__32;
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
-static PyObject *__pyx_tuple__36;
+static PyObject *__pyx_tuple__35;
 static PyObject *__pyx_tuple__37;
 static PyObject *__pyx_tuple__38;
 static PyObject *__pyx_tuple__39;
 static PyObject *__pyx_tuple__40;
 static PyObject *__pyx_tuple__41;
-static PyObject *__pyx_tuple__42;
 static PyObject *__pyx_tuple__43;
 static PyObject *__pyx_tuple__44;
 static PyObject *__pyx_tuple__45;
-static PyObject *__pyx_codeobj__46;
+static PyObject *__pyx_tuple__46;
+static PyObject *__pyx_tuple__47;
+static PyObject *__pyx_tuple__48;
+static PyObject *__pyx_codeobj__42;
+static PyObject *__pyx_codeobj__49;
 /* Late includes */
 
-/* "unipolator/unitary_interpolation_vector.pyx":37
+/* "unipolator/unitary_interpolation_vector.pyx":38
  *     cdef long[::1] first_elements_E, first_elements_C, L
  *     cdef long[::1] d_di
  *     def __cinit__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long), int m = 1):             # <<<<<<<<<<<<<<
  *         # Construct parameters
  *         self.n_dims = c_min_s.shape[0]
  */
 
@@ -2936,27 +2963,27 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_H_s)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_min_s)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 6, 1); __PYX_ERR(0, 37, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 6, 1); __PYX_ERR(0, 38, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_max_s)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 6, 2); __PYX_ERR(0, 37, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 6, 2); __PYX_ERR(0, 38, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_bins)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 6, 3); __PYX_ERR(0, 37, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 6, 3); __PYX_ERR(0, 38, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_which_diffs);
           if (value) { values[4] = value; kw_args--; }
         }
@@ -2964,15 +2991,15 @@
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_m);
           if (value) { values[5] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 37, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 38, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
@@ -2980,33 +3007,33 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_H_s = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_H_s.memview)) __PYX_ERR(0, 37, __pyx_L3_error)
-    __pyx_v_c_min_s = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c_min_s.memview)) __PYX_ERR(0, 37, __pyx_L3_error)
-    __pyx_v_c_max_s = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c_max_s.memview)) __PYX_ERR(0, 37, __pyx_L3_error)
-    __pyx_v_c_bins = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c_bins.memview)) __PYX_ERR(0, 37, __pyx_L3_error)
+    __pyx_v_H_s = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_H_s.memview)) __PYX_ERR(0, 38, __pyx_L3_error)
+    __pyx_v_c_min_s = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c_min_s.memview)) __PYX_ERR(0, 38, __pyx_L3_error)
+    __pyx_v_c_max_s = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c_max_s.memview)) __PYX_ERR(0, 38, __pyx_L3_error)
+    __pyx_v_c_bins = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c_bins.memview)) __PYX_ERR(0, 38, __pyx_L3_error)
     if (values[4]) {
-      __pyx_v_which_diffs = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_which_diffs.memview)) __PYX_ERR(0, 37, __pyx_L3_error)
+      __pyx_v_which_diffs = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_which_diffs.memview)) __PYX_ERR(0, 38, __pyx_L3_error)
     } else {
       __pyx_v_which_diffs = __pyx_k_;
       __PYX_INC_MEMVIEW(&__pyx_v_which_diffs, 1);
     }
     if (values[5]) {
-      __pyx_v_m = __Pyx_PyInt_As_int(values[5]); if (unlikely((__pyx_v_m == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 37, __pyx_L3_error)
+      __pyx_v_m = __Pyx_PyInt_As_int(values[5]); if (unlikely((__pyx_v_m == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L3_error)
     } else {
       __pyx_v_m = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 37, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 38, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.unitary_interpolation_vector.UI_vector.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector___cinit__(((struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self), __pyx_v_H_s, __pyx_v_c_min_s, __pyx_v_c_max_s, __pyx_v_c_bins, __pyx_v_which_diffs, __pyx_v_m);
 
@@ -3058,164 +3085,164 @@
   __Pyx_memviewslice __pyx_t_35 = { 0, 0, { 0 }, { 0 }, { 0 } };
   Py_ssize_t __pyx_t_36;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":39
+  /* "unipolator/unitary_interpolation_vector.pyx":40
  *     def __cinit__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long), int m = 1):
  *         # Construct parameters
  *         self.n_dims = c_min_s.shape[0]             # <<<<<<<<<<<<<<
  *         self.n_dims_1 = self.n_dims - 1
  *         self.d = H_s.shape[1]
  */
   __pyx_v_self->n_dims = (__pyx_v_c_min_s.shape[0]);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":40
+  /* "unipolator/unitary_interpolation_vector.pyx":41
  *         # Construct parameters
  *         self.n_dims = c_min_s.shape[0]
  *         self.n_dims_1 = self.n_dims - 1             # <<<<<<<<<<<<<<
  *         self.d = H_s.shape[1]
  *         self.d2 = self.d * self.d
  */
   __pyx_v_self->n_dims_1 = (__pyx_v_self->n_dims - 1);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":41
+  /* "unipolator/unitary_interpolation_vector.pyx":42
  *         self.n_dims = c_min_s.shape[0]
  *         self.n_dims_1 = self.n_dims - 1
  *         self.d = H_s.shape[1]             # <<<<<<<<<<<<<<
  *         self.d2 = self.d * self.d
  *         if not H_s.shape[0] == self.n_dims + 1:
  */
   __pyx_v_self->d = (__pyx_v_H_s.shape[1]);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":42
+  /* "unipolator/unitary_interpolation_vector.pyx":43
  *         self.n_dims_1 = self.n_dims - 1
  *         self.d = H_s.shape[1]
  *         self.d2 = self.d * self.d             # <<<<<<<<<<<<<<
  *         if not H_s.shape[0] == self.n_dims + 1:
  *             print('Requires n+1 Hamiltonians for n dimensional interpolation. Check lenths of Hs, c_mins, c_maxs, c_bins')
  */
   __pyx_v_self->d2 = (__pyx_v_self->d * __pyx_v_self->d);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":43
+  /* "unipolator/unitary_interpolation_vector.pyx":44
  *         self.d = H_s.shape[1]
  *         self.d2 = self.d * self.d
  *         if not H_s.shape[0] == self.n_dims + 1:             # <<<<<<<<<<<<<<
  *             print('Requires n+1 Hamiltonians for n dimensional interpolation. Check lenths of Hs, c_mins, c_maxs, c_bins')
  *             raise ValueError
  */
   __pyx_t_1 = ((!(((__pyx_v_H_s.shape[0]) == (__pyx_v_self->n_dims + 1)) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":44
+    /* "unipolator/unitary_interpolation_vector.pyx":45
  *         self.d2 = self.d * self.d
  *         if not H_s.shape[0] == self.n_dims + 1:
  *             print('Requires n+1 Hamiltonians for n dimensional interpolation. Check lenths of Hs, c_mins, c_maxs, c_bins')             # <<<<<<<<<<<<<<
  *             raise ValueError
  *         self.c_bins = np.empty(self.n_dims, dtype=long)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":45
+    /* "unipolator/unitary_interpolation_vector.pyx":46
  *         if not H_s.shape[0] == self.n_dims + 1:
  *             print('Requires n+1 Hamiltonians for n dimensional interpolation. Check lenths of Hs, c_mins, c_maxs, c_bins')
  *             raise ValueError             # <<<<<<<<<<<<<<
  *         self.c_bins = np.empty(self.n_dims, dtype=long)
  *         for i in range(self.n_dims):
  */
     __Pyx_Raise(__pyx_builtin_ValueError, 0, 0, 0);
-    __PYX_ERR(0, 45, __pyx_L1_error)
+    __PYX_ERR(0, 46, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":43
+    /* "unipolator/unitary_interpolation_vector.pyx":44
  *         self.d = H_s.shape[1]
  *         self.d2 = self.d * self.d
  *         if not H_s.shape[0] == self.n_dims + 1:             # <<<<<<<<<<<<<<
  *             print('Requires n+1 Hamiltonians for n dimensional interpolation. Check lenths of Hs, c_mins, c_maxs, c_bins')
  *             raise ValueError
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":46
+  /* "unipolator/unitary_interpolation_vector.pyx":47
  *             print('Requires n+1 Hamiltonians for n dimensional interpolation. Check lenths of Hs, c_mins, c_maxs, c_bins')
  *             raise ValueError
  *         self.c_bins = np.empty(self.n_dims, dtype=long)             # <<<<<<<<<<<<<<
  *         for i in range(self.n_dims):
  *             self.c_bins[i] = c_bins[i]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 46, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->c_bins, 0);
   __pyx_v_self->c_bins = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":47
+  /* "unipolator/unitary_interpolation_vector.pyx":48
  *             raise ValueError
  *         self.c_bins = np.empty(self.n_dims, dtype=long)
  *         for i in range(self.n_dims):             # <<<<<<<<<<<<<<
  *             self.c_bins[i] = c_bins[i]
  *         self.c_mins, self.c_maxs, self.dcs, self.das = Bin_Parameters(c_min_s, c_max_s, self.c_bins)
  */
   __pyx_t_7 = __pyx_v_self->n_dims;
   __pyx_t_8 = __pyx_t_7;
   for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
     __pyx_v_i = __pyx_t_9;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":48
+    /* "unipolator/unitary_interpolation_vector.pyx":49
  *         self.c_bins = np.empty(self.n_dims, dtype=long)
  *         for i in range(self.n_dims):
  *             self.c_bins[i] = c_bins[i]             # <<<<<<<<<<<<<<
  *         self.c_mins, self.c_maxs, self.dcs, self.das = Bin_Parameters(c_min_s, c_max_s, self.c_bins)
  *         # Single Step Indexing Parameters  --> Add multiple indexes later
  */
     __pyx_t_10 = __pyx_v_i;
     __pyx_t_11 = __pyx_v_i;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->c_bins.data) + __pyx_t_11)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_c_bins.data) + __pyx_t_10)) )));
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":49
+  /* "unipolator/unitary_interpolation_vector.pyx":50
  *         for i in range(self.n_dims):
  *             self.c_bins[i] = c_bins[i]
  *         self.c_mins, self.c_maxs, self.dcs, self.das = Bin_Parameters(c_min_s, c_max_s, self.c_bins)             # <<<<<<<<<<<<<<
  *         # Single Step Indexing Parameters  --> Add multiple indexes later
  *         self.location = np.empty(self.n_dims, dtype=long)
  */
-  __pyx_t_5 = __pyx_f_10unipolator_8indexing_Bin_Parameters(__pyx_v_c_min_s, __pyx_v_c_max_s, __pyx_v_self->c_bins, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_5 = __pyx_f_10unipolator_8indexing_Bin_Parameters(__pyx_v_c_min_s, __pyx_v_c_max_s, __pyx_v_self->c_bins, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if ((likely(PyTuple_CheckExact(__pyx_t_5))) || (PyList_CheckExact(__pyx_t_5))) {
     PyObject* sequence = __pyx_t_5;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 4)) {
       if (size > 4) __Pyx_RaiseTooManyValuesError(4);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 49, __pyx_L1_error)
+      __PYX_ERR(0, 50, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 2); 
       __pyx_t_12 = PyTuple_GET_ITEM(sequence, 3); 
@@ -3230,51 +3257,51 @@
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_12);
     #else
     {
       Py_ssize_t i;
       PyObject** temps[4] = {&__pyx_t_2,&__pyx_t_4,&__pyx_t_3,&__pyx_t_12};
       for (i=0; i < 4; i++) {
-        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 49, __pyx_L1_error)
+        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 50, __pyx_L1_error)
         __Pyx_GOTREF(item);
         *(temps[i]) = item;
       }
     }
     #endif
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else {
     Py_ssize_t index = -1;
     PyObject** temps[4] = {&__pyx_t_2,&__pyx_t_4,&__pyx_t_3,&__pyx_t_12};
-    __pyx_t_13 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_13 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 50, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_14 = Py_TYPE(__pyx_t_13)->tp_iternext;
     for (index=0; index < 4; index++) {
       PyObject* item = __pyx_t_14(__pyx_t_13); if (unlikely(!item)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(item);
       *(temps[index]) = item;
     }
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_14(__pyx_t_13), 4) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_14(__pyx_t_13), 4) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
     __pyx_t_14 = NULL;
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     goto __pyx_L7_unpacking_done;
     __pyx_L6_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     __pyx_t_14 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 49, __pyx_L1_error)
+    __PYX_ERR(0, 50, __pyx_L1_error)
     __pyx_L7_unpacking_done:;
   }
-  __pyx_t_15 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_15.memview)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_15.memview)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_16.memview)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_3, PyBUF_WRITABLE); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_3, PyBUF_WRITABLE); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_12, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_12, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->c_mins, 0);
   __pyx_v_self->c_mins = __pyx_t_15;
   __pyx_t_15.memview = NULL;
   __pyx_t_15.data = NULL;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->c_maxs, 0);
   __pyx_v_self->c_maxs = __pyx_t_16;
@@ -3285,326 +3312,326 @@
   __pyx_t_17.memview = NULL;
   __pyx_t_17.data = NULL;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->das, 0);
   __pyx_v_self->das = __pyx_t_18;
   __pyx_t_18.memview = NULL;
   __pyx_t_18.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":51
+  /* "unipolator/unitary_interpolation_vector.pyx":52
  *         self.c_mins, self.c_maxs, self.dcs, self.das = Bin_Parameters(c_min_s, c_max_s, self.c_bins)
  *         # Single Step Indexing Parameters  --> Add multiple indexes later
  *         self.location = np.empty(self.n_dims, dtype=long)             # <<<<<<<<<<<<<<
  *         self.abs_alpha_rest = np.empty(self.n_dims, dtype=np.double)
  *         self.d_location = np.empty(self.n_dims, dtype=long)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->location, 0);
   __pyx_v_self->location = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":52
+  /* "unipolator/unitary_interpolation_vector.pyx":53
  *         # Single Step Indexing Parameters  --> Add multiple indexes later
  *         self.location = np.empty(self.n_dims, dtype=long)
  *         self.abs_alpha_rest = np.empty(self.n_dims, dtype=np.double)             # <<<<<<<<<<<<<<
  *         self.d_location = np.empty(self.n_dims, dtype=long)
  *         self.alpha = np.empty(self.n_dims, dtype=np.double)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_double); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_double); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->abs_alpha_rest, 0);
   __pyx_v_self->abs_alpha_rest = __pyx_t_18;
   __pyx_t_18.memview = NULL;
   __pyx_t_18.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":53
+  /* "unipolator/unitary_interpolation_vector.pyx":54
  *         self.location = np.empty(self.n_dims, dtype=long)
  *         self.abs_alpha_rest = np.empty(self.n_dims, dtype=np.double)
  *         self.d_location = np.empty(self.n_dims, dtype=long)             # <<<<<<<<<<<<<<
  *         self.alpha = np.empty(self.n_dims, dtype=np.double)
  *         if which_diffs.shape[0] == 0:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->d_location, 0);
   __pyx_v_self->d_location = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":54
+  /* "unipolator/unitary_interpolation_vector.pyx":55
  *         self.abs_alpha_rest = np.empty(self.n_dims, dtype=np.double)
  *         self.d_location = np.empty(self.n_dims, dtype=long)
  *         self.alpha = np.empty(self.n_dims, dtype=np.double)             # <<<<<<<<<<<<<<
  *         if which_diffs.shape[0] == 0:
  *             self.d_di = np.arange(self.n_dims)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_12, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_12, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->alpha, 0);
   __pyx_v_self->alpha = __pyx_t_18;
   __pyx_t_18.memview = NULL;
   __pyx_t_18.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":55
+  /* "unipolator/unitary_interpolation_vector.pyx":56
  *         self.d_location = np.empty(self.n_dims, dtype=long)
  *         self.alpha = np.empty(self.n_dims, dtype=np.double)
  *         if which_diffs.shape[0] == 0:             # <<<<<<<<<<<<<<
  *             self.d_di = np.arange(self.n_dims)
  *         else:
  */
   __pyx_t_1 = (((__pyx_v_which_diffs.shape[0]) == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":56
+    /* "unipolator/unitary_interpolation_vector.pyx":57
  *         self.alpha = np.empty(self.n_dims, dtype=np.double)
  *         if which_diffs.shape[0] == 0:
  *             self.d_di = np.arange(self.n_dims)             # <<<<<<<<<<<<<<
  *         else:
  *             self.d_di = which_diffs
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_12 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 56, __pyx_L1_error)
+    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_12, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_12, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 57, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __PYX_XDEC_MEMVIEW(&__pyx_v_self->d_di, 0);
     __pyx_v_self->d_di = __pyx_t_6;
     __pyx_t_6.memview = NULL;
     __pyx_t_6.data = NULL;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":55
+    /* "unipolator/unitary_interpolation_vector.pyx":56
  *         self.d_location = np.empty(self.n_dims, dtype=long)
  *         self.alpha = np.empty(self.n_dims, dtype=np.double)
  *         if which_diffs.shape[0] == 0:             # <<<<<<<<<<<<<<
  *             self.d_di = np.arange(self.n_dims)
  *         else:
  */
     goto __pyx_L8;
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":58
+  /* "unipolator/unitary_interpolation_vector.pyx":59
  *             self.d_di = np.arange(self.n_dims)
  *         else:
  *             self.d_di = which_diffs             # <<<<<<<<<<<<<<
  *         self.n_d_di = self.d_di.shape[0]
  * 
  */
   /*else*/ {
     __PYX_XDEC_MEMVIEW(&__pyx_v_self->d_di, 0);
     __PYX_INC_MEMVIEW(&__pyx_v_which_diffs, 0);
     __pyx_v_self->d_di = __pyx_v_which_diffs;
   }
   __pyx_L8:;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":59
+  /* "unipolator/unitary_interpolation_vector.pyx":60
  *         else:
  *             self.d_di = which_diffs
  *         self.n_d_di = self.d_di.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         # Construct interpolation grid points
  */
   __pyx_v_self->n_d_di = (__pyx_v_self->d_di.shape[0]);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":62
+  /* "unipolator/unitary_interpolation_vector.pyx":63
  * 
  *         # Construct interpolation grid points
  *         U_grid, cum_prod = Unitary_Grid(H_s, self.c_mins, self.dcs, self.c_bins)             # <<<<<<<<<<<<<<
  *         ## Construct interpolation cache
  *         self.E, self.Vl, self.Vr, self.CL, self.CH, self.strides_E, self.strides_L, self.strides_R, self.strides_C, self.first_elements_E, self.first_elements_C = Create_Interpolation_Cache( U_grid, cum_prod, self.c_bins)
  */
-  __pyx_t_12 = __pyx_f_10unipolator_7caching_Unitary_Grid(__pyx_v_H_s, __pyx_v_self->c_mins, __pyx_v_self->dcs, __pyx_v_self->c_bins, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_12 = __pyx_f_10unipolator_7caching_Unitary_Grid(__pyx_v_H_s, __pyx_v_self->c_mins, __pyx_v_self->dcs, __pyx_v_self->c_bins, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   if ((likely(PyTuple_CheckExact(__pyx_t_12))) || (PyList_CheckExact(__pyx_t_12))) {
     PyObject* sequence = __pyx_t_12;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 62, __pyx_L1_error)
+      __PYX_ERR(0, 63, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_3 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_5);
     #else
-    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_2 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
+    __pyx_t_2 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __pyx_t_14 = Py_TYPE(__pyx_t_2)->tp_iternext;
     index = 0; __pyx_t_3 = __pyx_t_14(__pyx_t_2); if (unlikely(!__pyx_t_3)) goto __pyx_L9_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
     index = 1; __pyx_t_5 = __pyx_t_14(__pyx_t_2); if (unlikely(!__pyx_t_5)) goto __pyx_L9_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_5);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_14(__pyx_t_2), 2) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_14(__pyx_t_2), 2) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
     __pyx_t_14 = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L10_unpacking_done;
     __pyx_L9_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_14 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 62, __pyx_L1_error)
+    __PYX_ERR(0, 63, __pyx_L1_error)
     __pyx_L10_unpacking_done:;
   }
   __pyx_v_U_grid = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_cum_prod = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":64
+  /* "unipolator/unitary_interpolation_vector.pyx":65
  *         U_grid, cum_prod = Unitary_Grid(H_s, self.c_mins, self.dcs, self.c_bins)
  *         ## Construct interpolation cache
  *         self.E, self.Vl, self.Vr, self.CL, self.CH, self.strides_E, self.strides_L, self.strides_R, self.strides_C, self.first_elements_E, self.first_elements_C = Create_Interpolation_Cache( U_grid, cum_prod, self.c_bins)             # <<<<<<<<<<<<<<
  *         self.ei = &self.E[0, 0]
  *         self.vl = &self.Vl[0, 0, 0]
  */
-  __pyx_t_19 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_v_U_grid, PyBUF_WRITABLE); if (unlikely(!__pyx_t_19.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_cum_prod, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __pyx_t_12 = __pyx_f_10unipolator_7caching_Create_Interpolation_Cache(__pyx_t_19, __pyx_t_6, __pyx_v_self->c_bins, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_19 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_v_U_grid, PyBUF_WRITABLE); if (unlikely(!__pyx_t_19.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_cum_prod, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_12 = __pyx_f_10unipolator_7caching_Create_Interpolation_Cache(__pyx_t_19, __pyx_t_6, __pyx_v_self->c_bins, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __PYX_XDEC_MEMVIEW(&__pyx_t_19, 1);
   __pyx_t_19.memview = NULL;
   __pyx_t_19.data = NULL;
   __PYX_XDEC_MEMVIEW(&__pyx_t_6, 1);
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
   if ((likely(PyTuple_CheckExact(__pyx_t_12))) || (PyList_CheckExact(__pyx_t_12))) {
     PyObject* sequence = __pyx_t_12;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 11)) {
       if (size > 11) __Pyx_RaiseTooManyValuesError(11);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 64, __pyx_L1_error)
+      __PYX_ERR(0, 65, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_5 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 2); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 3); 
@@ -3640,65 +3667,65 @@
     __Pyx_INCREF(__pyx_t_24);
     __Pyx_INCREF(__pyx_t_25);
     #else
     {
       Py_ssize_t i;
       PyObject** temps[11] = {&__pyx_t_5,&__pyx_t_3,&__pyx_t_2,&__pyx_t_4,&__pyx_t_13,&__pyx_t_20,&__pyx_t_21,&__pyx_t_22,&__pyx_t_23,&__pyx_t_24,&__pyx_t_25};
       for (i=0; i < 11; i++) {
-        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 64, __pyx_L1_error)
+        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 65, __pyx_L1_error)
         __Pyx_GOTREF(item);
         *(temps[i]) = item;
       }
     }
     #endif
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   } else {
     Py_ssize_t index = -1;
     PyObject** temps[11] = {&__pyx_t_5,&__pyx_t_3,&__pyx_t_2,&__pyx_t_4,&__pyx_t_13,&__pyx_t_20,&__pyx_t_21,&__pyx_t_22,&__pyx_t_23,&__pyx_t_24,&__pyx_t_25};
-    __pyx_t_26 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __pyx_t_26 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_26)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_26);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __pyx_t_14 = Py_TYPE(__pyx_t_26)->tp_iternext;
     for (index=0; index < 11; index++) {
       PyObject* item = __pyx_t_14(__pyx_t_26); if (unlikely(!item)) goto __pyx_L11_unpacking_failed;
       __Pyx_GOTREF(item);
       *(temps[index]) = item;
     }
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_14(__pyx_t_26), 11) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_14(__pyx_t_26), 11) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
     __pyx_t_14 = NULL;
     __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
     goto __pyx_L12_unpacking_done;
     __pyx_L11_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_26); __pyx_t_26 = 0;
     __pyx_t_14 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 64, __pyx_L1_error)
+    __PYX_ERR(0, 65, __pyx_L1_error)
     __pyx_L12_unpacking_done:;
   }
-  __pyx_t_27 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_27.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_27 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_27.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_19 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_3, PyBUF_WRITABLE); if (unlikely(!__pyx_t_19.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_19 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_3, PyBUF_WRITABLE); if (unlikely(!__pyx_t_19.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_28 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_28.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_28 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_28.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_29 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_29.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_29 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_29.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_30 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_13, PyBUF_WRITABLE); if (unlikely(!__pyx_t_30.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_30 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_13, PyBUF_WRITABLE); if (unlikely(!__pyx_t_30.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  __pyx_t_31 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_long(__pyx_t_20, PyBUF_WRITABLE); if (unlikely(!__pyx_t_31.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_31 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_long(__pyx_t_20, PyBUF_WRITABLE); if (unlikely(!__pyx_t_31.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_21, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_21, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
-  __pyx_t_32 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_22, PyBUF_WRITABLE); if (unlikely(!__pyx_t_32.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_32 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_22, PyBUF_WRITABLE); if (unlikely(!__pyx_t_32.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-  __pyx_t_33 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_long(__pyx_t_23, PyBUF_WRITABLE); if (unlikely(!__pyx_t_33.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_33 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_long(__pyx_t_23, PyBUF_WRITABLE); if (unlikely(!__pyx_t_33.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_23); __pyx_t_23 = 0;
-  __pyx_t_34 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_24, PyBUF_WRITABLE); if (unlikely(!__pyx_t_34.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_34 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_24, PyBUF_WRITABLE); if (unlikely(!__pyx_t_34.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
-  __pyx_t_35 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_25, PyBUF_WRITABLE); if (unlikely(!__pyx_t_35.memview)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_35 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_25, PyBUF_WRITABLE); if (unlikely(!__pyx_t_35.memview)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->E, 0);
   __pyx_v_self->E = __pyx_t_27;
   __pyx_t_27.memview = NULL;
   __pyx_t_27.data = NULL;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->Vl, 0);
   __pyx_v_self->Vl = __pyx_t_19;
@@ -3737,125 +3764,125 @@
   __pyx_t_34.memview = NULL;
   __pyx_t_34.data = NULL;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->first_elements_C, 0);
   __pyx_v_self->first_elements_C = __pyx_t_35;
   __pyx_t_35.memview = NULL;
   __pyx_t_35.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":65
+  /* "unipolator/unitary_interpolation_vector.pyx":66
  *         ## Construct interpolation cache
  *         self.E, self.Vl, self.Vr, self.CL, self.CH, self.strides_E, self.strides_L, self.strides_R, self.strides_C, self.first_elements_E, self.first_elements_C = Create_Interpolation_Cache( U_grid, cum_prod, self.c_bins)
  *         self.ei = &self.E[0, 0]             # <<<<<<<<<<<<<<
  *         self.vl = &self.Vl[0, 0, 0]
  *         self.vr = &self.Vr[0, 0, 0]
  */
   __pyx_t_10 = 0;
   __pyx_t_11 = 0;
   __pyx_v_self->ei = (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_self->E.data + __pyx_t_10 * __pyx_v_self->E.strides[0]) )) + __pyx_t_11)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":66
+  /* "unipolator/unitary_interpolation_vector.pyx":67
  *         self.E, self.Vl, self.Vr, self.CL, self.CH, self.strides_E, self.strides_L, self.strides_R, self.strides_C, self.first_elements_E, self.first_elements_C = Create_Interpolation_Cache( U_grid, cum_prod, self.c_bins)
  *         self.ei = &self.E[0, 0]
  *         self.vl = &self.Vl[0, 0, 0]             # <<<<<<<<<<<<<<
  *         self.vr = &self.Vr[0, 0, 0]
  *         self.c = &self.CH[0, 0, 0]
  */
   __pyx_t_11 = 0;
   __pyx_t_10 = 0;
   __pyx_t_36 = 0;
   __pyx_v_self->vl = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->Vl.data + __pyx_t_11 * __pyx_v_self->Vl.strides[0]) ) + __pyx_t_10 * __pyx_v_self->Vl.strides[1]) )) + __pyx_t_36)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":67
+  /* "unipolator/unitary_interpolation_vector.pyx":68
  *         self.ei = &self.E[0, 0]
  *         self.vl = &self.Vl[0, 0, 0]
  *         self.vr = &self.Vr[0, 0, 0]             # <<<<<<<<<<<<<<
  *         self.c = &self.CH[0, 0, 0]
  *         self.L = np.empty(self.n_dims, dtype=long)
  */
   __pyx_t_36 = 0;
   __pyx_t_10 = 0;
   __pyx_t_11 = 0;
   __pyx_v_self->vr = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->Vr.data + __pyx_t_36 * __pyx_v_self->Vr.strides[0]) ) + __pyx_t_10 * __pyx_v_self->Vr.strides[1]) )) + __pyx_t_11)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":68
+  /* "unipolator/unitary_interpolation_vector.pyx":69
  *         self.vl = &self.Vl[0, 0, 0]
  *         self.vr = &self.Vr[0, 0, 0]
  *         self.c = &self.CH[0, 0, 0]             # <<<<<<<<<<<<<<
  *         self.L = np.empty(self.n_dims, dtype=long)
  *         self.change_m(m)
  */
   __pyx_t_11 = 0;
   __pyx_t_10 = 0;
   __pyx_t_36 = 0;
   __pyx_v_self->c = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->CH.data + __pyx_t_11 * __pyx_v_self->CH.strides[0]) ) + __pyx_t_10 * __pyx_v_self->CH.strides[1]) )) + __pyx_t_36)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":69
+  /* "unipolator/unitary_interpolation_vector.pyx":70
  *         self.vr = &self.Vr[0, 0, 0]
  *         self.c = &self.CH[0, 0, 0]
  *         self.L = np.empty(self.n_dims, dtype=long)             # <<<<<<<<<<<<<<
  *         self.change_m(m)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_25 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_25 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_25)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_25);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyInt_From_int(__pyx_v_self->n_dims); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_24 = PyTuple_New(1); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_24 = PyTuple_New(1); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_24);
   __Pyx_GIVEREF(__pyx_t_12);
   PyTuple_SET_ITEM(__pyx_t_24, 0, __pyx_t_12);
   __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
-  __pyx_t_23 = __Pyx_PyObject_Call(__pyx_t_25, __pyx_t_24, __pyx_t_12); if (unlikely(!__pyx_t_23)) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_23 = __Pyx_PyObject_Call(__pyx_t_25, __pyx_t_24, __pyx_t_12); if (unlikely(!__pyx_t_23)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_23);
   __Pyx_DECREF(__pyx_t_25); __pyx_t_25 = 0;
   __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_35 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_23, PyBUF_WRITABLE); if (unlikely(!__pyx_t_35.memview)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_35 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_23, PyBUF_WRITABLE); if (unlikely(!__pyx_t_35.memview)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_23); __pyx_t_23 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->L, 0);
   __pyx_v_self->L = __pyx_t_35;
   __pyx_t_35.memview = NULL;
   __pyx_t_35.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":70
+  /* "unipolator/unitary_interpolation_vector.pyx":71
  *         self.c = &self.CH[0, 0, 0]
  *         self.L = np.empty(self.n_dims, dtype=long)
  *         self.change_m(m)             # <<<<<<<<<<<<<<
  * 
  *     def change_m(self, int m):
  */
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_change_m); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_change_m); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_24 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_24 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_24)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_24);
   __pyx_t_25 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
     __pyx_t_25 = PyMethod_GET_SELF(__pyx_t_12);
     if (likely(__pyx_t_25)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
       __Pyx_INCREF(__pyx_t_25);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_12, function);
     }
   }
   __pyx_t_23 = (__pyx_t_25) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_25, __pyx_t_24) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_24);
   __Pyx_XDECREF(__pyx_t_25); __pyx_t_25 = 0;
   __Pyx_DECREF(__pyx_t_24); __pyx_t_24 = 0;
-  if (unlikely(!__pyx_t_23)) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (unlikely(!__pyx_t_23)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_23);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __Pyx_DECREF(__pyx_t_23); __pyx_t_23 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":37
+  /* "unipolator/unitary_interpolation_vector.pyx":38
  *     cdef long[::1] first_elements_E, first_elements_C, L
  *     cdef long[::1] d_di
  *     def __cinit__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long), int m = 1):             # <<<<<<<<<<<<<<
  *         # Construct parameters
  *         self.n_dims = c_min_s.shape[0]
  */
 
@@ -3901,15 +3928,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_c_max_s, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_c_bins, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_which_diffs, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":72
+/* "unipolator/unitary_interpolation_vector.pyx":73
  *         self.change_m(m)
  * 
  *     def change_m(self, int m):             # <<<<<<<<<<<<<<
  *         self.m = m
  *         self.dm = self.d * m
  */
 
@@ -3921,15 +3948,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("change_m (wrapper)", 0);
   assert(__pyx_arg_m); {
-    __pyx_v_m = __Pyx_PyInt_As_int(__pyx_arg_m); if (unlikely((__pyx_v_m == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
+    __pyx_v_m = __Pyx_PyInt_As_int(__pyx_arg_m); if (unlikely((__pyx_v_m == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.unitary_interpolation_vector.UI_vector.change_m", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -3955,339 +3982,339 @@
   Py_ssize_t __pyx_t_10;
   __Pyx_memviewslice __pyx_t_11 = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("change_m", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":73
+  /* "unipolator/unitary_interpolation_vector.pyx":74
  * 
  *     def change_m(self, int m):
  *         self.m = m             # <<<<<<<<<<<<<<
  *         self.dm = self.d * m
  *         # also change self.vi's
  */
   __pyx_v_self->m = __pyx_v_m;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":74
+  /* "unipolator/unitary_interpolation_vector.pyx":75
  *     def change_m(self, int m):
  *         self.m = m
  *         self.dm = self.d * m             # <<<<<<<<<<<<<<
  *         # also change self.vi's
  *         self.Ur = np.empty([self.d, self.m], dtype=np.complex128)
  */
   __pyx_v_self->dm = (__pyx_v_self->d * __pyx_v_m);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":76
+  /* "unipolator/unitary_interpolation_vector.pyx":77
  *         self.dm = self.d * m
  *         # also change self.vi's
  *         self.Ur = np.empty([self.d, self.m], dtype=np.complex128)             # <<<<<<<<<<<<<<
  *         self.ur0 = &self.Ur[0, 0]
  *         self.Ur1 = np.empty([self.d, self.m], dtype=np.complex128)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->d); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->d); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->m); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->m); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_complex128); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_complex128); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->Ur, 0);
   __pyx_v_self->Ur = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":77
+  /* "unipolator/unitary_interpolation_vector.pyx":78
  *         # also change self.vi's
  *         self.Ur = np.empty([self.d, self.m], dtype=np.complex128)
  *         self.ur0 = &self.Ur[0, 0]             # <<<<<<<<<<<<<<
  *         self.Ur1 = np.empty([self.d, self.m], dtype=np.complex128)
  *         self.ur1 = &self.Ur1[0, 0]
  */
   __pyx_t_7 = 0;
   __pyx_t_8 = 0;
   __pyx_v_self->ur0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_self->Ur.data + __pyx_t_7 * __pyx_v_self->Ur.strides[0]) )) + __pyx_t_8)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":78
+  /* "unipolator/unitary_interpolation_vector.pyx":79
  *         self.Ur = np.empty([self.d, self.m], dtype=np.complex128)
  *         self.ur0 = &self.Ur[0, 0]
  *         self.Ur1 = np.empty([self.d, self.m], dtype=np.complex128)             # <<<<<<<<<<<<<<
  *         self.ur1 = &self.Ur1[0, 0]
  *         self.dU1 = np.empty([self.n_d_di, self.d, self.m], dtype=np.complex128)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->d); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->d); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->m); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->m); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_5);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_3);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_5 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_complex128); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_complex128); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->Ur1, 0);
   __pyx_v_self->Ur1 = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":79
+  /* "unipolator/unitary_interpolation_vector.pyx":80
  *         self.ur0 = &self.Ur[0, 0]
  *         self.Ur1 = np.empty([self.d, self.m], dtype=np.complex128)
  *         self.ur1 = &self.Ur1[0, 0]             # <<<<<<<<<<<<<<
  *         self.dU1 = np.empty([self.n_d_di, self.d, self.m], dtype=np.complex128)
  *         self.du1 = &self.dU1[0, 0, 0]
  */
   __pyx_t_8 = 0;
   __pyx_t_7 = 0;
   __pyx_v_self->ur1 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_self->Ur1.data + __pyx_t_8 * __pyx_v_self->Ur1.strides[0]) )) + __pyx_t_7)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":80
+  /* "unipolator/unitary_interpolation_vector.pyx":81
  *         self.Ur1 = np.empty([self.d, self.m], dtype=np.complex128)
  *         self.ur1 = &self.Ur1[0, 0]
  *         self.dU1 = np.empty([self.n_d_di, self.d, self.m], dtype=np.complex128)             # <<<<<<<<<<<<<<
  *         self.du1 = &self.dU1[0, 0, 0]
  *         self.dU2 = np.empty([self.n_d_di, self.d, self.m], dtype=np.complex128)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->n_d_di); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->n_d_di); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->d); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->d); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->m); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->m); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyList_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_complex128); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_complex128); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->dU1, 0);
   __pyx_v_self->dU1 = __pyx_t_9;
   __pyx_t_9.memview = NULL;
   __pyx_t_9.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":81
+  /* "unipolator/unitary_interpolation_vector.pyx":82
  *         self.ur1 = &self.Ur1[0, 0]
  *         self.dU1 = np.empty([self.n_d_di, self.d, self.m], dtype=np.complex128)
  *         self.du1 = &self.dU1[0, 0, 0]             # <<<<<<<<<<<<<<
  *         self.dU2 = np.empty([self.n_d_di, self.d, self.m], dtype=np.complex128)
  *         self.du2 = &self.dU2[0, 0, 0]
  */
   __pyx_t_7 = 0;
   __pyx_t_8 = 0;
   __pyx_t_10 = 0;
   __pyx_v_self->du1 = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->dU1.data + __pyx_t_7 * __pyx_v_self->dU1.strides[0]) ) + __pyx_t_8 * __pyx_v_self->dU1.strides[1]) )) + __pyx_t_10)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":82
+  /* "unipolator/unitary_interpolation_vector.pyx":83
  *         self.dU1 = np.empty([self.n_d_di, self.d, self.m], dtype=np.complex128)
  *         self.du1 = &self.dU1[0, 0, 0]
  *         self.dU2 = np.empty([self.n_d_di, self.d, self.m], dtype=np.complex128)             # <<<<<<<<<<<<<<
  *         self.du2 = &self.dU2[0, 0, 0]
  *         self.Es = np.empty(self.d, dtype=np.complex128)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->n_d_di); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->n_d_di); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->d); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->d); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->m); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->m); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyList_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyList_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyList_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_4 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_complex128); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_complex128); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->dU2, 0);
   __pyx_v_self->dU2 = __pyx_t_9;
   __pyx_t_9.memview = NULL;
   __pyx_t_9.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":83
+  /* "unipolator/unitary_interpolation_vector.pyx":84
  *         self.du1 = &self.dU1[0, 0, 0]
  *         self.dU2 = np.empty([self.n_d_di, self.d, self.m], dtype=np.complex128)
  *         self.du2 = &self.dU2[0, 0, 0]             # <<<<<<<<<<<<<<
  *         self.Es = np.empty(self.d, dtype=np.complex128)
  *         self.es0 = &self.Es[0]
  */
   __pyx_t_10 = 0;
   __pyx_t_8 = 0;
   __pyx_t_7 = 0;
   __pyx_v_self->du2 = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->dU2.data + __pyx_t_10 * __pyx_v_self->dU2.strides[0]) ) + __pyx_t_8 * __pyx_v_self->dU2.strides[1]) )) + __pyx_t_7)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":84
+  /* "unipolator/unitary_interpolation_vector.pyx":85
  *         self.dU2 = np.empty([self.n_d_di, self.d, self.m], dtype=np.complex128)
  *         self.du2 = &self.dU2[0, 0, 0]
  *         self.Es = np.empty(self.d, dtype=np.complex128)             # <<<<<<<<<<<<<<
  *         self.es0 = &self.Es[0]
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->d); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->d); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_complex128); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_complex128); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_dc___pyx_t_double_complex(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->Es, 0);
   __pyx_v_self->Es = __pyx_t_11;
   __pyx_t_11.memview = NULL;
   __pyx_t_11.data = NULL;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":85
+  /* "unipolator/unitary_interpolation_vector.pyx":86
  *         self.du2 = &self.dU2[0, 0, 0]
  *         self.Es = np.empty(self.d, dtype=np.complex128)
  *         self.es0 = &self.Es[0]             # <<<<<<<<<<<<<<
  * 
  *     cdef single_parameters2oddgrid(self, double[::1] c):
  */
   __pyx_t_7 = 0;
   __pyx_v_self->es0 = (&(*((__pyx_t_double_complex *) ( /* dim=0 */ ((char *) (((__pyx_t_double_complex *) __pyx_v_self->Es.data) + __pyx_t_7)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":72
+  /* "unipolator/unitary_interpolation_vector.pyx":73
  *         self.change_m(m)
  * 
  *     def change_m(self, int m):             # <<<<<<<<<<<<<<
  *         self.m = m
  *         self.dm = self.d * m
  */
 
@@ -4307,15 +4334,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":87
+/* "unipolator/unitary_interpolation_vector.pyx":88
  *         self.es0 = &self.Es[0]
  * 
  *     cdef single_parameters2oddgrid(self, double[::1] c):             # <<<<<<<<<<<<<<
  *         cdef int sum_location = 0
  *         cdef double alpha_max = 0.0
  */
 
@@ -4340,162 +4367,162 @@
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("single_parameters2oddgrid", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":88
+  /* "unipolator/unitary_interpolation_vector.pyx":89
  * 
  *     cdef single_parameters2oddgrid(self, double[::1] c):
  *         cdef int sum_location = 0             # <<<<<<<<<<<<<<
  *         cdef double alpha_max = 0.0
  *         cdef double alpha_rest
  */
   __pyx_v_sum_location = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":89
+  /* "unipolator/unitary_interpolation_vector.pyx":90
  *     cdef single_parameters2oddgrid(self, double[::1] c):
  *         cdef int sum_location = 0
  *         cdef double alpha_max = 0.0             # <<<<<<<<<<<<<<
  *         cdef double alpha_rest
  *         cdef Py_ssize_t i
  */
   __pyx_v_alpha_max = 0.0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":92
+  /* "unipolator/unitary_interpolation_vector.pyx":93
  *         cdef double alpha_rest
  *         cdef Py_ssize_t i
  *         cdef int max_alpha_ind = 0             # <<<<<<<<<<<<<<
  *         cdef int max_vals
  *         for i in range(self.n_dims):
  */
   __pyx_v_max_alpha_ind = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":94
+  /* "unipolator/unitary_interpolation_vector.pyx":95
  *         cdef int max_alpha_ind = 0
  *         cdef int max_vals
  *         for i in range(self.n_dims):             # <<<<<<<<<<<<<<
  *             # Transform
  *             self.alpha[i] = (c[i] - self.c_mins[i]) / self.dcs[i]
  */
   __pyx_t_1 = __pyx_v_self->n_dims;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":96
+    /* "unipolator/unitary_interpolation_vector.pyx":97
  *         for i in range(self.n_dims):
  *             # Transform
  *             self.alpha[i] = (c[i] - self.c_mins[i]) / self.dcs[i]             # <<<<<<<<<<<<<<
  *             # Round
  *             self.location[i] = <int> self.alpha[i]     # floor ->
  */
     __pyx_t_4 = __pyx_v_i;
     __pyx_t_5 = __pyx_v_i;
     __pyx_t_6 = __pyx_v_i;
     __pyx_t_7 = __pyx_v_i;
     *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->alpha.data) + __pyx_t_7)) )) = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_c.data) + __pyx_t_4)) ))) - (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->c_mins.data) + __pyx_t_5)) )))) / (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->dcs.data) + __pyx_t_6)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":98
+    /* "unipolator/unitary_interpolation_vector.pyx":99
  *             self.alpha[i] = (c[i] - self.c_mins[i]) / self.dcs[i]
  *             # Round
  *             self.location[i] = <int> self.alpha[i]     # floor ->             # <<<<<<<<<<<<<<
  *             alpha_rest = self.alpha[i] - self.location[i]
  *             if alpha_rest > 0.5:
  */
     __pyx_t_6 = __pyx_v_i;
     __pyx_t_5 = __pyx_v_i;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_5)) )) = ((int)(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->alpha.data) + __pyx_t_6)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":99
+    /* "unipolator/unitary_interpolation_vector.pyx":100
  *             # Round
  *             self.location[i] = <int> self.alpha[i]     # floor ->
  *             alpha_rest = self.alpha[i] - self.location[i]             # <<<<<<<<<<<<<<
  *             if alpha_rest > 0.5:
  *                 self.location[i] += 1
  */
     __pyx_t_6 = __pyx_v_i;
     __pyx_t_5 = __pyx_v_i;
     __pyx_v_alpha_rest = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->alpha.data) + __pyx_t_6)) ))) - (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_5)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":100
+    /* "unipolator/unitary_interpolation_vector.pyx":101
  *             self.location[i] = <int> self.alpha[i]     # floor ->
  *             alpha_rest = self.alpha[i] - self.location[i]
  *             if alpha_rest > 0.5:             # <<<<<<<<<<<<<<
  *                 self.location[i] += 1
  *                 alpha_rest -= 1
  */
     __pyx_t_8 = ((__pyx_v_alpha_rest > 0.5) != 0);
     if (__pyx_t_8) {
 
-      /* "unipolator/unitary_interpolation_vector.pyx":101
+      /* "unipolator/unitary_interpolation_vector.pyx":102
  *             alpha_rest = self.alpha[i] - self.location[i]
  *             if alpha_rest > 0.5:
  *                 self.location[i] += 1             # <<<<<<<<<<<<<<
  *                 alpha_rest -= 1
  *             sum_location += self.location[i]
  */
       __pyx_t_5 = __pyx_v_i;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_5)) )) += 1;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":102
+      /* "unipolator/unitary_interpolation_vector.pyx":103
  *             if alpha_rest > 0.5:
  *                 self.location[i] += 1
  *                 alpha_rest -= 1             # <<<<<<<<<<<<<<
  *             sum_location += self.location[i]
  * 
  */
       __pyx_v_alpha_rest = (__pyx_v_alpha_rest - 1.0);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":100
+      /* "unipolator/unitary_interpolation_vector.pyx":101
  *             self.location[i] = <int> self.alpha[i]     # floor ->
  *             alpha_rest = self.alpha[i] - self.location[i]
  *             if alpha_rest > 0.5:             # <<<<<<<<<<<<<<
  *                 self.location[i] += 1
  *                 alpha_rest -= 1
  */
     }
 
-    /* "unipolator/unitary_interpolation_vector.pyx":103
+    /* "unipolator/unitary_interpolation_vector.pyx":104
  *                 self.location[i] += 1
  *                 alpha_rest -= 1
  *             sum_location += self.location[i]             # <<<<<<<<<<<<<<
  * 
  *             self.abs_alpha_rest[i] = fabs(alpha_rest)
  */
     __pyx_t_5 = __pyx_v_i;
     __pyx_v_sum_location = (__pyx_v_sum_location + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_5)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":105
+    /* "unipolator/unitary_interpolation_vector.pyx":106
  *             sum_location += self.location[i]
  * 
  *             self.abs_alpha_rest[i] = fabs(alpha_rest)             # <<<<<<<<<<<<<<
  *             self.d_location[i] = 1 if alpha_rest >= 0 else -1
  *             if self.alpha[i] < 0 or self.alpha[i] > self.c_bins[i]:
  */
     __pyx_t_5 = __pyx_v_i;
     *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_5)) )) = fabs(__pyx_v_alpha_rest);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":106
+    /* "unipolator/unitary_interpolation_vector.pyx":107
  * 
  *             self.abs_alpha_rest[i] = fabs(alpha_rest)
  *             self.d_location[i] = 1 if alpha_rest >= 0 else -1             # <<<<<<<<<<<<<<
  *             if self.alpha[i] < 0 or self.alpha[i] > self.c_bins[i]:
  *                 print('Warning: These parameters lie outside of interpolation grid!')
  */
     if (((__pyx_v_alpha_rest >= 0.0) != 0)) {
       __pyx_t_9 = 1;
     } else {
       __pyx_t_9 = -1L;
     }
     __pyx_t_5 = __pyx_v_i;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_5)) )) = __pyx_t_9;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":107
+    /* "unipolator/unitary_interpolation_vector.pyx":108
  *             self.abs_alpha_rest[i] = fabs(alpha_rest)
  *             self.d_location[i] = 1 if alpha_rest >= 0 else -1
  *             if self.alpha[i] < 0 or self.alpha[i] > self.c_bins[i]:             # <<<<<<<<<<<<<<
  *                 print('Warning: These parameters lie outside of interpolation grid!')
  *                 break
  */
     __pyx_t_5 = __pyx_v_i;
@@ -4508,226 +4535,226 @@
     __pyx_t_5 = __pyx_v_i;
     __pyx_t_6 = __pyx_v_i;
     __pyx_t_10 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->alpha.data) + __pyx_t_5)) ))) > (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->c_bins.data) + __pyx_t_6)) )))) != 0);
     __pyx_t_8 = __pyx_t_10;
     __pyx_L7_bool_binop_done:;
     if (__pyx_t_8) {
 
-      /* "unipolator/unitary_interpolation_vector.pyx":108
+      /* "unipolator/unitary_interpolation_vector.pyx":109
  *             self.d_location[i] = 1 if alpha_rest >= 0 else -1
  *             if self.alpha[i] < 0 or self.alpha[i] > self.c_bins[i]:
  *                 print('Warning: These parameters lie outside of interpolation grid!')             # <<<<<<<<<<<<<<
  *                 break
  *         if is_even(sum_location):
  */
-      __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 108, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 109, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":109
+      /* "unipolator/unitary_interpolation_vector.pyx":110
  *             if self.alpha[i] < 0 or self.alpha[i] > self.c_bins[i]:
  *                 print('Warning: These parameters lie outside of interpolation grid!')
  *                 break             # <<<<<<<<<<<<<<
  *         if is_even(sum_location):
  *             max_alpha_ind = c_argmax(self.abs_alpha_rest, max_alpha_ind, alpha_max, self.n_dims)
  */
       goto __pyx_L4_break;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":107
+      /* "unipolator/unitary_interpolation_vector.pyx":108
  *             self.abs_alpha_rest[i] = fabs(alpha_rest)
  *             self.d_location[i] = 1 if alpha_rest >= 0 else -1
  *             if self.alpha[i] < 0 or self.alpha[i] > self.c_bins[i]:             # <<<<<<<<<<<<<<
  *                 print('Warning: These parameters lie outside of interpolation grid!')
  *                 break
  */
     }
   }
   __pyx_L4_break:;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":110
+  /* "unipolator/unitary_interpolation_vector.pyx":111
  *                 print('Warning: These parameters lie outside of interpolation grid!')
  *                 break
  *         if is_even(sum_location):             # <<<<<<<<<<<<<<
  *             max_alpha_ind = c_argmax(self.abs_alpha_rest, max_alpha_ind, alpha_max, self.n_dims)
  *             if self.location[max_alpha_ind] + self.d_location[max_alpha_ind] > self.c_bins[max_alpha_ind]:
  */
   __pyx_t_8 = (__pyx_f_10unipolator_8indexing_is_even(__pyx_v_sum_location, 0) != 0);
   if (__pyx_t_8) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":111
+    /* "unipolator/unitary_interpolation_vector.pyx":112
  *                 break
  *         if is_even(sum_location):
  *             max_alpha_ind = c_argmax(self.abs_alpha_rest, max_alpha_ind, alpha_max, self.n_dims)             # <<<<<<<<<<<<<<
  *             if self.location[max_alpha_ind] + self.d_location[max_alpha_ind] > self.c_bins[max_alpha_ind]:
  *                 self.d_location[max_alpha_ind] = -1
  */
     __pyx_v_max_alpha_ind = __pyx_f_10unipolator_8indexing_c_argmax(__pyx_v_self->abs_alpha_rest, __pyx_v_max_alpha_ind, __pyx_v_alpha_max, __pyx_v_self->n_dims, 0);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":112
+    /* "unipolator/unitary_interpolation_vector.pyx":113
  *         if is_even(sum_location):
  *             max_alpha_ind = c_argmax(self.abs_alpha_rest, max_alpha_ind, alpha_max, self.n_dims)
  *             if self.location[max_alpha_ind] + self.d_location[max_alpha_ind] > self.c_bins[max_alpha_ind]:             # <<<<<<<<<<<<<<
  *                 self.d_location[max_alpha_ind] = -1
  *             self.location[max_alpha_ind] += self.d_location[max_alpha_ind]
  */
     __pyx_t_6 = __pyx_v_max_alpha_ind;
     __pyx_t_5 = __pyx_v_max_alpha_ind;
     __pyx_t_4 = __pyx_v_max_alpha_ind;
     __pyx_t_8 = ((((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_6)) ))) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_5)) )))) > (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->c_bins.data) + __pyx_t_4)) )))) != 0);
     if (__pyx_t_8) {
 
-      /* "unipolator/unitary_interpolation_vector.pyx":113
+      /* "unipolator/unitary_interpolation_vector.pyx":114
  *             max_alpha_ind = c_argmax(self.abs_alpha_rest, max_alpha_ind, alpha_max, self.n_dims)
  *             if self.location[max_alpha_ind] + self.d_location[max_alpha_ind] > self.c_bins[max_alpha_ind]:
  *                 self.d_location[max_alpha_ind] = -1             # <<<<<<<<<<<<<<
  *             self.location[max_alpha_ind] += self.d_location[max_alpha_ind]
  *             self.d_location[max_alpha_ind] = - self.d_location[max_alpha_ind]
  */
       __pyx_t_4 = __pyx_v_max_alpha_ind;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_4)) )) = -1L;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":112
+      /* "unipolator/unitary_interpolation_vector.pyx":113
  *         if is_even(sum_location):
  *             max_alpha_ind = c_argmax(self.abs_alpha_rest, max_alpha_ind, alpha_max, self.n_dims)
  *             if self.location[max_alpha_ind] + self.d_location[max_alpha_ind] > self.c_bins[max_alpha_ind]:             # <<<<<<<<<<<<<<
  *                 self.d_location[max_alpha_ind] = -1
  *             self.location[max_alpha_ind] += self.d_location[max_alpha_ind]
  */
     }
 
-    /* "unipolator/unitary_interpolation_vector.pyx":114
+    /* "unipolator/unitary_interpolation_vector.pyx":115
  *             if self.location[max_alpha_ind] + self.d_location[max_alpha_ind] > self.c_bins[max_alpha_ind]:
  *                 self.d_location[max_alpha_ind] = -1
  *             self.location[max_alpha_ind] += self.d_location[max_alpha_ind]             # <<<<<<<<<<<<<<
  *             self.d_location[max_alpha_ind] = - self.d_location[max_alpha_ind]
  *             self.abs_alpha_rest[max_alpha_ind] = 1-self.abs_alpha_rest[max_alpha_ind]
  */
     __pyx_t_4 = __pyx_v_max_alpha_ind;
     __pyx_t_5 = __pyx_v_max_alpha_ind;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_5)) )) += (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_4)) )));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":115
+    /* "unipolator/unitary_interpolation_vector.pyx":116
  *                 self.d_location[max_alpha_ind] = -1
  *             self.location[max_alpha_ind] += self.d_location[max_alpha_ind]
  *             self.d_location[max_alpha_ind] = - self.d_location[max_alpha_ind]             # <<<<<<<<<<<<<<
  *             self.abs_alpha_rest[max_alpha_ind] = 1-self.abs_alpha_rest[max_alpha_ind]
  *         for i in range(self.n_dims):
  */
     __pyx_t_4 = __pyx_v_max_alpha_ind;
     __pyx_t_5 = __pyx_v_max_alpha_ind;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_5)) )) = (-(*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_4)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":116
+    /* "unipolator/unitary_interpolation_vector.pyx":117
  *             self.location[max_alpha_ind] += self.d_location[max_alpha_ind]
  *             self.d_location[max_alpha_ind] = - self.d_location[max_alpha_ind]
  *             self.abs_alpha_rest[max_alpha_ind] = 1-self.abs_alpha_rest[max_alpha_ind]             # <<<<<<<<<<<<<<
  *         for i in range(self.n_dims):
  *             self.d_location[i] -= 1
  */
     __pyx_t_4 = __pyx_v_max_alpha_ind;
     __pyx_t_5 = __pyx_v_max_alpha_ind;
     *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_5)) )) = (1.0 - (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_4)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":110
+    /* "unipolator/unitary_interpolation_vector.pyx":111
  *                 print('Warning: These parameters lie outside of interpolation grid!')
  *                 break
  *         if is_even(sum_location):             # <<<<<<<<<<<<<<
  *             max_alpha_ind = c_argmax(self.abs_alpha_rest, max_alpha_ind, alpha_max, self.n_dims)
  *             if self.location[max_alpha_ind] + self.d_location[max_alpha_ind] > self.c_bins[max_alpha_ind]:
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":117
+  /* "unipolator/unitary_interpolation_vector.pyx":118
  *             self.d_location[max_alpha_ind] = - self.d_location[max_alpha_ind]
  *             self.abs_alpha_rest[max_alpha_ind] = 1-self.abs_alpha_rest[max_alpha_ind]
  *         for i in range(self.n_dims):             # <<<<<<<<<<<<<<
  *             self.d_location[i] -= 1
  *             self.d_location[i] >>= 1 # via bitshift operation
  */
   __pyx_t_1 = __pyx_v_self->n_dims;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":118
+    /* "unipolator/unitary_interpolation_vector.pyx":119
  *             self.abs_alpha_rest[max_alpha_ind] = 1-self.abs_alpha_rest[max_alpha_ind]
  *         for i in range(self.n_dims):
  *             self.d_location[i] -= 1             # <<<<<<<<<<<<<<
  *             self.d_location[i] >>= 1 # via bitshift operation
  *             #d_location[i] /= 2 #(d_location[i]-1)/2 ### in two steps with optimized in-place operations
  */
     __pyx_t_4 = __pyx_v_i;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_4)) )) -= 1;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":119
+    /* "unipolator/unitary_interpolation_vector.pyx":120
  *         for i in range(self.n_dims):
  *             self.d_location[i] -= 1
  *             self.d_location[i] >>= 1 # via bitshift operation             # <<<<<<<<<<<<<<
  *             #d_location[i] /= 2 #(d_location[i]-1)/2 ### in two steps with optimized in-place operations
  *         for i in range(self.n_dims):
  */
     __pyx_t_4 = __pyx_v_i;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_4)) )) >>= 1;
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":121
+  /* "unipolator/unitary_interpolation_vector.pyx":122
  *             self.d_location[i] >>= 1 # via bitshift operation
  *             #d_location[i] /= 2 #(d_location[i]-1)/2 ### in two steps with optimized in-place operations
  *         for i in range(self.n_dims):             # <<<<<<<<<<<<<<
  *             max_vals = self.location[i]+self.d_location[i]
  *             if max_vals > self.c_bins[i]-1:
  */
   __pyx_t_1 = __pyx_v_self->n_dims;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":122
+    /* "unipolator/unitary_interpolation_vector.pyx":123
  *             #d_location[i] /= 2 #(d_location[i]-1)/2 ### in two steps with optimized in-place operations
  *         for i in range(self.n_dims):
  *             max_vals = self.location[i]+self.d_location[i]             # <<<<<<<<<<<<<<
  *             if max_vals > self.c_bins[i]-1:
  *                 self.d_location[i] = -1
  */
     __pyx_t_4 = __pyx_v_i;
     __pyx_t_5 = __pyx_v_i;
     __pyx_v_max_vals = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_4)) ))) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_5)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":123
+    /* "unipolator/unitary_interpolation_vector.pyx":124
  *         for i in range(self.n_dims):
  *             max_vals = self.location[i]+self.d_location[i]
  *             if max_vals > self.c_bins[i]-1:             # <<<<<<<<<<<<<<
  *                 self.d_location[i] = -1
  * 
  */
     __pyx_t_5 = __pyx_v_i;
     __pyx_t_8 = ((__pyx_v_max_vals > ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->c_bins.data) + __pyx_t_5)) ))) - 1)) != 0);
     if (__pyx_t_8) {
 
-      /* "unipolator/unitary_interpolation_vector.pyx":124
+      /* "unipolator/unitary_interpolation_vector.pyx":125
  *             max_vals = self.location[i]+self.d_location[i]
  *             if max_vals > self.c_bins[i]-1:
  *                 self.d_location[i] = -1             # <<<<<<<<<<<<<<
  * 
  *     def set_which_diffs(self, long[::1] which_diffs):
  */
       __pyx_t_5 = __pyx_v_i;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_5)) )) = -1L;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":123
+      /* "unipolator/unitary_interpolation_vector.pyx":124
  *         for i in range(self.n_dims):
  *             max_vals = self.location[i]+self.d_location[i]
  *             if max_vals > self.c_bins[i]-1:             # <<<<<<<<<<<<<<
  *                 self.d_location[i] = -1
  * 
  */
     }
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":87
+  /* "unipolator/unitary_interpolation_vector.pyx":88
  *         self.es0 = &self.Es[0]
  * 
  *     cdef single_parameters2oddgrid(self, double[::1] c):             # <<<<<<<<<<<<<<
  *         cdef int sum_location = 0
  *         cdef double alpha_max = 0.0
  */
 
@@ -4740,15 +4767,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":126
+/* "unipolator/unitary_interpolation_vector.pyx":127
  *                 self.d_location[i] = -1
  * 
  *     def set_which_diffs(self, long[::1] which_diffs):             # <<<<<<<<<<<<<<
  *         self.d_di = which_diffs
  *         self.n_d_di_1 = self.d_di.shape[0] - 1
  */
 
@@ -4760,15 +4787,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_which_diffs (wrapper)", 0);
   assert(__pyx_arg_which_diffs); {
-    __pyx_v_which_diffs = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_arg_which_diffs, PyBUF_WRITABLE); if (unlikely(!__pyx_v_which_diffs.memview)) __PYX_ERR(0, 126, __pyx_L3_error)
+    __pyx_v_which_diffs = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_arg_which_diffs, PyBUF_WRITABLE); if (unlikely(!__pyx_v_which_diffs.memview)) __PYX_ERR(0, 127, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.unitary_interpolation_vector.UI_vector.set_which_diffs", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -4780,44 +4807,44 @@
 }
 
 static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_4set_which_diffs(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *__pyx_v_self, __Pyx_memviewslice __pyx_v_which_diffs) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_which_diffs", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":127
+  /* "unipolator/unitary_interpolation_vector.pyx":128
  * 
  *     def set_which_diffs(self, long[::1] which_diffs):
  *         self.d_di = which_diffs             # <<<<<<<<<<<<<<
  *         self.n_d_di_1 = self.d_di.shape[0] - 1
  *         self.n_d_di = self.d_di.shape[0]
  */
   __PYX_XDEC_MEMVIEW(&__pyx_v_self->d_di, 0);
   __PYX_INC_MEMVIEW(&__pyx_v_which_diffs, 0);
   __pyx_v_self->d_di = __pyx_v_which_diffs;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":128
+  /* "unipolator/unitary_interpolation_vector.pyx":129
  *     def set_which_diffs(self, long[::1] which_diffs):
  *         self.d_di = which_diffs
  *         self.n_d_di_1 = self.d_di.shape[0] - 1             # <<<<<<<<<<<<<<
  *         self.n_d_di = self.d_di.shape[0]
  * 
  */
   __pyx_v_self->n_d_di_1 = ((__pyx_v_self->d_di.shape[0]) - 1);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":129
+  /* "unipolator/unitary_interpolation_vector.pyx":130
  *         self.d_di = which_diffs
  *         self.n_d_di_1 = self.d_di.shape[0] - 1
  *         self.n_d_di = self.d_di.shape[0]             # <<<<<<<<<<<<<<
  * 
  *     def get_single_param(self, double[::1] c): # To verify interpolation grid
  */
   __pyx_v_self->n_d_di = (__pyx_v_self->d_di.shape[0]);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":126
+  /* "unipolator/unitary_interpolation_vector.pyx":127
  *                 self.d_location[i] = -1
  * 
  *     def set_which_diffs(self, long[::1] which_diffs):             # <<<<<<<<<<<<<<
  *         self.d_di = which_diffs
  *         self.n_d_di_1 = self.d_di.shape[0] - 1
  */
 
@@ -4825,15 +4852,15 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __PYX_XDEC_MEMVIEW(&__pyx_v_which_diffs, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":131
+/* "unipolator/unitary_interpolation_vector.pyx":132
  *         self.n_d_di = self.d_di.shape[0]
  * 
  *     def get_single_param(self, double[::1] c): # To verify interpolation grid             # <<<<<<<<<<<<<<
  *         self.single_parameters2oddgrid(c)
  *         return np.asarray(self.location), np.asarray(self.d_location), np.asarray(self.abs_alpha_rest)
  */
 
@@ -4845,15 +4872,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_single_param (wrapper)", 0);
   assert(__pyx_arg_c); {
-    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_arg_c, PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 131, __pyx_L3_error)
+    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_arg_c, PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 132, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.unitary_interpolation_vector.UI_vector.get_single_param", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -4874,118 +4901,118 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_single_param", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":132
+  /* "unipolator/unitary_interpolation_vector.pyx":133
  * 
  *     def get_single_param(self, double[::1] c): # To verify interpolation grid
  *         self.single_parameters2oddgrid(c)             # <<<<<<<<<<<<<<
  *         return np.asarray(self.location), np.asarray(self.d_location), np.asarray(self.abs_alpha_rest)
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_v_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_v_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":133
+  /* "unipolator/unitary_interpolation_vector.pyx":134
  *     def get_single_param(self, double[::1] c): # To verify interpolation grid
  *         self.single_parameters2oddgrid(c)
  *         return np.asarray(self.location), np.asarray(self.d_location), np.asarray(self.abs_alpha_rest)             # <<<<<<<<<<<<<<
  * 
  *     def get_cache(self): # To verify interpolation grid
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->location, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->location, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->d_location, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->d_location, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->abs_alpha_rest, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->abs_alpha_rest, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":131
+  /* "unipolator/unitary_interpolation_vector.pyx":132
  *         self.n_d_di = self.d_di.shape[0]
  * 
  *     def get_single_param(self, double[::1] c): # To verify interpolation grid             # <<<<<<<<<<<<<<
  *         self.single_parameters2oddgrid(c)
  *         return np.asarray(self.location), np.asarray(self.d_location), np.asarray(self.abs_alpha_rest)
  */
 
@@ -5002,15 +5029,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_c, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":135
+/* "unipolator/unitary_interpolation_vector.pyx":136
  *         return np.asarray(self.location), np.asarray(self.d_location), np.asarray(self.abs_alpha_rest)
  * 
  *     def get_cache(self): # To verify interpolation grid             # <<<<<<<<<<<<<<
  *         return np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL), np.asarray(self.CH), np.asarray(self.strides_E), np.asarray(self.strides_L), np.asarray(self.strides_R), np.asarray(self.strides_C)
  * 
  */
 
@@ -5044,230 +5071,230 @@
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_cache", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":136
+  /* "unipolator/unitary_interpolation_vector.pyx":137
  * 
  *     def get_cache(self): # To verify interpolation grid
  *         return np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL), np.asarray(self.CH), np.asarray(self.strides_E), np.asarray(self.strides_L), np.asarray(self.strides_R), np.asarray(self.strides_C)             # <<<<<<<<<<<<<<
  * 
  *     cdef interpolate_single_u(self, double complex *u0, double complex *v0): #u0 => input vectors, v0 => output vectors
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->E, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->E, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->Vl, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->Vl, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->Vr, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->Vr, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CL, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CL, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CH, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->CH, 3, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_E, 2, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_E, 2, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
   __pyx_t_7 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_L, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_L, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_10 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_10);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_9, function);
     }
   }
   __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_R, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_R, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_11 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_11);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_10, function);
     }
   }
   __pyx_t_9 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_11, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_C, 2, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_self->strides_C, 2, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_12 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
     if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
       __Pyx_INCREF(__pyx_t_12);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_11, function);
     }
   }
   __pyx_t_10 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_12, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 136, __pyx_L1_error)
+  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = PyTuple_New(9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_11 = PyTuple_New(9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_t_4);
@@ -5292,15 +5319,15 @@
   __pyx_t_8 = 0;
   __pyx_t_9 = 0;
   __pyx_t_10 = 0;
   __pyx_r = __pyx_t_11;
   __pyx_t_11 = 0;
   goto __pyx_L0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":135
+  /* "unipolator/unitary_interpolation_vector.pyx":136
  *         return np.asarray(self.location), np.asarray(self.d_location), np.asarray(self.abs_alpha_rest)
  * 
  *     def get_cache(self): # To verify interpolation grid             # <<<<<<<<<<<<<<
  *         return np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL), np.asarray(self.CH), np.asarray(self.strides_E), np.asarray(self.strides_L), np.asarray(self.strides_R), np.asarray(self.strides_C)
  * 
  */
 
@@ -5322,15 +5349,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":138
+/* "unipolator/unitary_interpolation_vector.pyx":139
  *         return np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL), np.asarray(self.CH), np.asarray(self.strides_E), np.asarray(self.strides_L), np.asarray(self.strides_R), np.asarray(self.strides_C)
  * 
  *     cdef interpolate_single_u(self, double complex *u0, double complex *v0): #u0 => input vectors, v0 => output vectors             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i, j
  *         cdef Py_ssize_t ind
  */
 
@@ -5348,146 +5375,146 @@
   int __pyx_t_6;
   Py_ssize_t __pyx_t_7;
   __Pyx_memviewslice __pyx_t_8 = { 0, 0, { 0 }, { 0 }, { 0 } };
   __pyx_t_double_complex *__pyx_t_9;
   __pyx_t_double_complex *__pyx_t_10;
   __Pyx_RefNannySetupContext("interpolate_single_u", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":141
+  /* "unipolator/unitary_interpolation_vector.pyx":142
  *         cdef Py_ssize_t i, j
  *         cdef Py_ssize_t ind
  *         if self.n_dims == 1:             # <<<<<<<<<<<<<<
  *             ind = self.location[0] + self.d_location[0]
  *             self.vr = &self.Vr[ind,0,0] # In 1D strides are 1
  */
   __pyx_t_1 = ((__pyx_v_self->n_dims == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":142
+    /* "unipolator/unitary_interpolation_vector.pyx":143
  *         cdef Py_ssize_t ind
  *         if self.n_dims == 1:
  *             ind = self.location[0] + self.d_location[0]             # <<<<<<<<<<<<<<
  *             self.vr = &self.Vr[ind,0,0] # In 1D strides are 1
  *             self.vl = &self.Vl[ind,0,0]
  */
     __pyx_t_2 = 0;
     __pyx_t_3 = 0;
     __pyx_v_ind = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_2)) ))) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_3)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":143
+    /* "unipolator/unitary_interpolation_vector.pyx":144
  *         if self.n_dims == 1:
  *             ind = self.location[0] + self.d_location[0]
  *             self.vr = &self.Vr[ind,0,0] # In 1D strides are 1             # <<<<<<<<<<<<<<
  *             self.vl = &self.Vl[ind,0,0]
  *             self.ei = &self.E[ind,0]
  */
     __pyx_t_3 = __pyx_v_ind;
     __pyx_t_2 = 0;
     __pyx_t_4 = 0;
     __pyx_v_self->vr = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->Vr.data + __pyx_t_3 * __pyx_v_self->Vr.strides[0]) ) + __pyx_t_2 * __pyx_v_self->Vr.strides[1]) )) + __pyx_t_4)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":144
+    /* "unipolator/unitary_interpolation_vector.pyx":145
  *             ind = self.location[0] + self.d_location[0]
  *             self.vr = &self.Vr[ind,0,0] # In 1D strides are 1
  *             self.vl = &self.Vl[ind,0,0]             # <<<<<<<<<<<<<<
  *             self.ei = &self.E[ind,0]
  *             MM_cdot_pointer_v(self.vr, u0, self.ur0, self.d, self.m)
  */
     __pyx_t_4 = __pyx_v_ind;
     __pyx_t_2 = 0;
     __pyx_t_3 = 0;
     __pyx_v_self->vl = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->Vl.data + __pyx_t_4 * __pyx_v_self->Vl.strides[0]) ) + __pyx_t_2 * __pyx_v_self->Vl.strides[1]) )) + __pyx_t_3)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":145
+    /* "unipolator/unitary_interpolation_vector.pyx":146
  *             self.vr = &self.Vr[ind,0,0] # In 1D strides are 1
  *             self.vl = &self.Vl[ind,0,0]
  *             self.ei = &self.E[ind,0]             # <<<<<<<<<<<<<<
  *             MM_cdot_pointer_v(self.vr, u0, self.ur0, self.d, self.m)
  *             v_exp_pointer_v(self.ei, self.ur0, self.abs_alpha_rest[0], self.d, self.m)
  */
     __pyx_t_3 = __pyx_v_ind;
     __pyx_t_2 = 0;
     __pyx_v_self->ei = (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_self->E.data + __pyx_t_3 * __pyx_v_self->E.strides[0]) )) + __pyx_t_2)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":146
+    /* "unipolator/unitary_interpolation_vector.pyx":147
  *             self.vl = &self.Vl[ind,0,0]
  *             self.ei = &self.E[ind,0]
  *             MM_cdot_pointer_v(self.vr, u0, self.ur0, self.d, self.m)             # <<<<<<<<<<<<<<
  *             v_exp_pointer_v(self.ei, self.ur0, self.abs_alpha_rest[0], self.d, self.m)
  *             MM_cdot_pointer_v(self.vl, self.ur0, v0, self.d, self.m)
  */
     __pyx_f_10unipolator_22blas_functions_vectors_MM_cdot_pointer_v(__pyx_v_self->vr, __pyx_v_u0, __pyx_v_self->ur0, __pyx_v_self->d, __pyx_v_self->m);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":147
+    /* "unipolator/unitary_interpolation_vector.pyx":148
  *             self.ei = &self.E[ind,0]
  *             MM_cdot_pointer_v(self.vr, u0, self.ur0, self.d, self.m)
  *             v_exp_pointer_v(self.ei, self.ur0, self.abs_alpha_rest[0], self.d, self.m)             # <<<<<<<<<<<<<<
  *             MM_cdot_pointer_v(self.vl, self.ur0, v0, self.d, self.m)
  *         else:
  */
     __pyx_t_2 = 0;
     __pyx_f_10unipolator_22blas_functions_vectors_v_exp_pointer_v(__pyx_v_self->ei, __pyx_v_self->ur0, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_2)) ))), __pyx_v_self->d, __pyx_v_self->m);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":148
+    /* "unipolator/unitary_interpolation_vector.pyx":149
  *             MM_cdot_pointer_v(self.vr, u0, self.ur0, self.d, self.m)
  *             v_exp_pointer_v(self.ei, self.ur0, self.abs_alpha_rest[0], self.d, self.m)
  *             MM_cdot_pointer_v(self.vl, self.ur0, v0, self.d, self.m)             # <<<<<<<<<<<<<<
  *         else:
  *             # Right side first
  */
     __pyx_f_10unipolator_22blas_functions_vectors_MM_cdot_pointer_v(__pyx_v_self->vl, __pyx_v_self->ur0, __pyx_v_v0, __pyx_v_self->d, __pyx_v_self->m);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":141
+    /* "unipolator/unitary_interpolation_vector.pyx":142
  *         cdef Py_ssize_t i, j
  *         cdef Py_ssize_t ind
  *         if self.n_dims == 1:             # <<<<<<<<<<<<<<
  *             ind = self.location[0] + self.d_location[0]
  *             self.vr = &self.Vr[ind,0,0] # In 1D strides are 1
  */
     goto __pyx_L3;
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":151
+  /* "unipolator/unitary_interpolation_vector.pyx":152
  *         else:
  *             # Right side first
  *             self.L[0] = self.location[0] + self.d_location[0]             # <<<<<<<<<<<<<<
  *             for i in range(1, self.n_dims):
  *                 self.L[i] = self.location[i]
  */
   /*else*/ {
     __pyx_t_2 = 0;
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_4)) )) = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_2)) ))) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_3)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":152
+    /* "unipolator/unitary_interpolation_vector.pyx":153
  *             # Right side first
  *             self.L[0] = self.location[0] + self.d_location[0]
  *             for i in range(1, self.n_dims):             # <<<<<<<<<<<<<<
  *                 self.L[i] = self.location[i]
  *             ind = findex_0(self.L, self.strides_E[0,:], self.n_dims)
  */
     __pyx_t_5 = __pyx_v_self->n_dims;
     __pyx_t_6 = __pyx_t_5;
     for (__pyx_t_7 = 1; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
       __pyx_v_i = __pyx_t_7;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":153
+      /* "unipolator/unitary_interpolation_vector.pyx":154
  *             self.L[0] = self.location[0] + self.d_location[0]
  *             for i in range(1, self.n_dims):
  *                 self.L[i] = self.location[i]             # <<<<<<<<<<<<<<
  *             ind = findex_0(self.L, self.strides_E[0,:], self.n_dims)
  *             self.vr = &self.Vr[ind, 0, 0]  # In 1D strides are 1
  */
       __pyx_t_3 = __pyx_v_i;
       __pyx_t_2 = __pyx_v_i;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_2)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_3)) )));
     }
 
-    /* "unipolator/unitary_interpolation_vector.pyx":154
+    /* "unipolator/unitary_interpolation_vector.pyx":155
  *             for i in range(1, self.n_dims):
  *                 self.L[i] = self.location[i]
  *             ind = findex_0(self.L, self.strides_E[0,:], self.n_dims)             # <<<<<<<<<<<<<<
  *             self.vr = &self.Vr[ind, 0, 0]  # In 1D strides are 1
  *             MM_cdot_pointer_v(self.vr, u0, self.ur0, self.d, self.m)
  */
     __pyx_t_8.data = __pyx_v_self->strides_E.data;
@@ -5504,100 +5531,100 @@
     __pyx_t_8.suboffsets[0] = -1;
 
 __pyx_v_ind = __pyx_f_10unipolator_8indexing_findex_0(__pyx_v_self->L, __pyx_t_8, __pyx_v_self->n_dims, 0);
     __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
     __pyx_t_8.memview = NULL;
     __pyx_t_8.data = NULL;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":155
+    /* "unipolator/unitary_interpolation_vector.pyx":156
  *                 self.L[i] = self.location[i]
  *             ind = findex_0(self.L, self.strides_E[0,:], self.n_dims)
  *             self.vr = &self.Vr[ind, 0, 0]  # In 1D strides are 1             # <<<<<<<<<<<<<<
  *             MM_cdot_pointer_v(self.vr, u0, self.ur0, self.d, self.m)
  *             self.ei = &self.E[ind, 0]
  */
     __pyx_t_3 = __pyx_v_ind;
     __pyx_t_2 = 0;
     __pyx_t_4 = 0;
     __pyx_v_self->vr = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->Vr.data + __pyx_t_3 * __pyx_v_self->Vr.strides[0]) ) + __pyx_t_2 * __pyx_v_self->Vr.strides[1]) )) + __pyx_t_4)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":156
+    /* "unipolator/unitary_interpolation_vector.pyx":157
  *             ind = findex_0(self.L, self.strides_E[0,:], self.n_dims)
  *             self.vr = &self.Vr[ind, 0, 0]  # In 1D strides are 1
  *             MM_cdot_pointer_v(self.vr, u0, self.ur0, self.d, self.m)             # <<<<<<<<<<<<<<
  *             self.ei = &self.E[ind, 0]
  *             v_exp_pointer_v(self.ei, self.ur0, self.abs_alpha_rest[0], self.d, self.m)
  */
     __pyx_f_10unipolator_22blas_functions_vectors_MM_cdot_pointer_v(__pyx_v_self->vr, __pyx_v_u0, __pyx_v_self->ur0, __pyx_v_self->d, __pyx_v_self->m);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":157
+    /* "unipolator/unitary_interpolation_vector.pyx":158
  *             self.vr = &self.Vr[ind, 0, 0]  # In 1D strides are 1
  *             MM_cdot_pointer_v(self.vr, u0, self.ur0, self.d, self.m)
  *             self.ei = &self.E[ind, 0]             # <<<<<<<<<<<<<<
  *             v_exp_pointer_v(self.ei, self.ur0, self.abs_alpha_rest[0], self.d, self.m)
  *             self.L[0] = self.location[0]
  */
     __pyx_t_4 = __pyx_v_ind;
     __pyx_t_2 = 0;
     __pyx_v_self->ei = (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_self->E.data + __pyx_t_4 * __pyx_v_self->E.strides[0]) )) + __pyx_t_2)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":158
+    /* "unipolator/unitary_interpolation_vector.pyx":159
  *             MM_cdot_pointer_v(self.vr, u0, self.ur0, self.d, self.m)
  *             self.ei = &self.E[ind, 0]
  *             v_exp_pointer_v(self.ei, self.ur0, self.abs_alpha_rest[0], self.d, self.m)             # <<<<<<<<<<<<<<
  *             self.L[0] = self.location[0]
  *             # Center multiplications
  */
     __pyx_t_2 = 0;
     __pyx_f_10unipolator_22blas_functions_vectors_v_exp_pointer_v(__pyx_v_self->ei, __pyx_v_self->ur0, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_2)) ))), __pyx_v_self->d, __pyx_v_self->m);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":159
+    /* "unipolator/unitary_interpolation_vector.pyx":160
  *             self.ei = &self.E[ind, 0]
  *             v_exp_pointer_v(self.ei, self.ur0, self.abs_alpha_rest[0], self.d, self.m)
  *             self.L[0] = self.location[0]             # <<<<<<<<<<<<<<
  *             # Center multiplications
  *             for i in range(self.n_dims_1):
  */
     __pyx_t_2 = 0;
     __pyx_t_4 = 0;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_4)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_2)) )));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":161
+    /* "unipolator/unitary_interpolation_vector.pyx":162
  *             self.L[0] = self.location[0]
  *             # Center multiplications
  *             for i in range(self.n_dims_1):             # <<<<<<<<<<<<<<
  *                 j = i + 1
  *                 self.L[j] += self.d_location[j]
  */
     __pyx_t_5 = __pyx_v_self->n_dims_1;
     __pyx_t_6 = __pyx_t_5;
     for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
       __pyx_v_i = __pyx_t_7;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":162
+      /* "unipolator/unitary_interpolation_vector.pyx":163
  *             # Center multiplications
  *             for i in range(self.n_dims_1):
  *                 j = i + 1             # <<<<<<<<<<<<<<
  *                 self.L[j] += self.d_location[j]
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]
  */
       __pyx_v_j = (__pyx_v_i + 1);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":163
+      /* "unipolator/unitary_interpolation_vector.pyx":164
  *             for i in range(self.n_dims_1):
  *                 j = i + 1
  *                 self.L[j] += self.d_location[j]             # <<<<<<<<<<<<<<
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]
  *                 self.ei = &self.E[ind, 0]
  */
       __pyx_t_2 = __pyx_v_j;
       __pyx_t_4 = __pyx_v_j;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_4)) )) += (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_2)) )));
 
-      /* "unipolator/unitary_interpolation_vector.pyx":164
+      /* "unipolator/unitary_interpolation_vector.pyx":165
  *                 j = i + 1
  *                 self.L[j] += self.d_location[j]
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]             # <<<<<<<<<<<<<<
  *                 self.ei = &self.E[ind, 0]
  *                 if self.d_location[i]:  ### Higher
  */
       __pyx_t_8.data = __pyx_v_self->strides_E.data;
@@ -5615,47 +5642,47 @@
 
 __pyx_t_2 = __pyx_v_j;
       __pyx_v_ind = (__pyx_f_10unipolator_8indexing_findex_0(__pyx_v_self->L, __pyx_t_8, __pyx_v_self->n_dims, 0) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->first_elements_E.data) + __pyx_t_2)) ))));
       __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
       __pyx_t_8.memview = NULL;
       __pyx_t_8.data = NULL;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":165
+      /* "unipolator/unitary_interpolation_vector.pyx":166
  *                 self.L[j] += self.d_location[j]
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]
  *                 self.ei = &self.E[ind, 0]             # <<<<<<<<<<<<<<
  *                 if self.d_location[i]:  ### Higher
  *                     self.L[i] += -1
  */
       __pyx_t_2 = __pyx_v_ind;
       __pyx_t_4 = 0;
       __pyx_v_self->ei = (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_self->E.data + __pyx_t_2 * __pyx_v_self->E.strides[0]) )) + __pyx_t_4)) ))));
 
-      /* "unipolator/unitary_interpolation_vector.pyx":166
+      /* "unipolator/unitary_interpolation_vector.pyx":167
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]
  *                 self.ei = &self.E[ind, 0]
  *                 if self.d_location[i]:  ### Higher             # <<<<<<<<<<<<<<
  *                     self.L[i] += -1
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  */
       __pyx_t_4 = __pyx_v_i;
       __pyx_t_1 = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_4)) ))) != 0);
       if (__pyx_t_1) {
 
-        /* "unipolator/unitary_interpolation_vector.pyx":167
+        /* "unipolator/unitary_interpolation_vector.pyx":168
  *                 self.ei = &self.E[ind, 0]
  *                 if self.d_location[i]:  ### Higher
  *                     self.L[i] += -1             # <<<<<<<<<<<<<<
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  *                     self.c = &self.CL[ind, 0, 0]
  */
         __pyx_t_4 = __pyx_v_i;
         *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_4)) )) += -1L;
 
-        /* "unipolator/unitary_interpolation_vector.pyx":168
+        /* "unipolator/unitary_interpolation_vector.pyx":169
  *                 if self.d_location[i]:  ### Higher
  *                     self.L[i] += -1
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]             # <<<<<<<<<<<<<<
  *                     self.c = &self.CL[ind, 0, 0]
  *                     self.L[i] += 1  # Restore value
  */
         __pyx_t_8.data = __pyx_v_self->strides_C.data;
@@ -5673,47 +5700,47 @@
 
 __pyx_t_4 = __pyx_v_i;
         __pyx_v_ind = (__pyx_f_10unipolator_8indexing_findex_0(__pyx_v_self->L, __pyx_t_8, __pyx_v_self->n_dims, 0) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->first_elements_C.data) + __pyx_t_4)) ))));
         __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
         __pyx_t_8.memview = NULL;
         __pyx_t_8.data = NULL;
 
-        /* "unipolator/unitary_interpolation_vector.pyx":169
+        /* "unipolator/unitary_interpolation_vector.pyx":170
  *                     self.L[i] += -1
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  *                     self.c = &self.CL[ind, 0, 0]             # <<<<<<<<<<<<<<
  *                     self.L[i] += 1  # Restore value
  *                 else:                        ### Lower
  */
         __pyx_t_4 = __pyx_v_ind;
         __pyx_t_2 = 0;
         __pyx_t_3 = 0;
         __pyx_v_self->c = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->CL.data + __pyx_t_4 * __pyx_v_self->CL.strides[0]) ) + __pyx_t_2 * __pyx_v_self->CL.strides[1]) )) + __pyx_t_3)) ))));
 
-        /* "unipolator/unitary_interpolation_vector.pyx":170
+        /* "unipolator/unitary_interpolation_vector.pyx":171
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  *                     self.c = &self.CL[ind, 0, 0]
  *                     self.L[i] += 1  # Restore value             # <<<<<<<<<<<<<<
  *                 else:                        ### Lower
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims)+self.first_elements_C[i]
  */
         __pyx_t_3 = __pyx_v_i;
         *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_3)) )) += 1;
 
-        /* "unipolator/unitary_interpolation_vector.pyx":166
+        /* "unipolator/unitary_interpolation_vector.pyx":167
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]
  *                 self.ei = &self.E[ind, 0]
  *                 if self.d_location[i]:  ### Higher             # <<<<<<<<<<<<<<
  *                     self.L[i] += -1
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  */
         goto __pyx_L8;
       }
 
-      /* "unipolator/unitary_interpolation_vector.pyx":172
+      /* "unipolator/unitary_interpolation_vector.pyx":173
  *                     self.L[i] += 1  # Restore value
  *                 else:                        ### Lower
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims)+self.first_elements_C[i]             # <<<<<<<<<<<<<<
  *                     self.c = &self.CH[ind,0,0]
  *                 self.L[j] = self.location[j]
  */
       /*else*/ {
@@ -5732,130 +5759,130 @@
 
 __pyx_t_3 = __pyx_v_i;
         __pyx_v_ind = (__pyx_f_10unipolator_8indexing_findex_0(__pyx_v_self->L, __pyx_t_8, __pyx_v_self->n_dims, 0) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->first_elements_C.data) + __pyx_t_3)) ))));
         __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
         __pyx_t_8.memview = NULL;
         __pyx_t_8.data = NULL;
 
-        /* "unipolator/unitary_interpolation_vector.pyx":173
+        /* "unipolator/unitary_interpolation_vector.pyx":174
  *                 else:                        ### Lower
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims)+self.first_elements_C[i]
  *                     self.c = &self.CH[ind,0,0]             # <<<<<<<<<<<<<<
  *                 self.L[j] = self.location[j]
  *                 MM_cdot_pointer_v(self.c, self.ur0, self.ur1, self.d, self.m)
  */
         __pyx_t_3 = __pyx_v_ind;
         __pyx_t_2 = 0;
         __pyx_t_4 = 0;
         __pyx_v_self->c = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->CH.data + __pyx_t_3 * __pyx_v_self->CH.strides[0]) ) + __pyx_t_2 * __pyx_v_self->CH.strides[1]) )) + __pyx_t_4)) ))));
       }
       __pyx_L8:;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":174
+      /* "unipolator/unitary_interpolation_vector.pyx":175
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims)+self.first_elements_C[i]
  *                     self.c = &self.CH[ind,0,0]
  *                 self.L[j] = self.location[j]             # <<<<<<<<<<<<<<
  *                 MM_cdot_pointer_v(self.c, self.ur0, self.ur1, self.d, self.m)
  *                 v_exp_pointer_v(self.ei, self.ur1, self.abs_alpha_rest[j], self.d, self.m)
  */
       __pyx_t_4 = __pyx_v_j;
       __pyx_t_2 = __pyx_v_j;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_2)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_4)) )));
 
-      /* "unipolator/unitary_interpolation_vector.pyx":175
+      /* "unipolator/unitary_interpolation_vector.pyx":176
  *                     self.c = &self.CH[ind,0,0]
  *                 self.L[j] = self.location[j]
  *                 MM_cdot_pointer_v(self.c, self.ur0, self.ur1, self.d, self.m)             # <<<<<<<<<<<<<<
  *                 v_exp_pointer_v(self.ei, self.ur1, self.abs_alpha_rest[j], self.d, self.m)
  *                 self.ur1, self.ur0 = self.ur0, self.ur1
  */
       __pyx_f_10unipolator_22blas_functions_vectors_MM_cdot_pointer_v(__pyx_v_self->c, __pyx_v_self->ur0, __pyx_v_self->ur1, __pyx_v_self->d, __pyx_v_self->m);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":176
+      /* "unipolator/unitary_interpolation_vector.pyx":177
  *                 self.L[j] = self.location[j]
  *                 MM_cdot_pointer_v(self.c, self.ur0, self.ur1, self.d, self.m)
  *                 v_exp_pointer_v(self.ei, self.ur1, self.abs_alpha_rest[j], self.d, self.m)             # <<<<<<<<<<<<<<
  *                 self.ur1, self.ur0 = self.ur0, self.ur1
  *             # Left side multiplication
  */
       __pyx_t_4 = __pyx_v_j;
       __pyx_f_10unipolator_22blas_functions_vectors_v_exp_pointer_v(__pyx_v_self->ei, __pyx_v_self->ur1, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_4)) ))), __pyx_v_self->d, __pyx_v_self->m);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":177
+      /* "unipolator/unitary_interpolation_vector.pyx":178
  *                 MM_cdot_pointer_v(self.c, self.ur0, self.ur1, self.d, self.m)
  *                 v_exp_pointer_v(self.ei, self.ur1, self.abs_alpha_rest[j], self.d, self.m)
  *                 self.ur1, self.ur0 = self.ur0, self.ur1             # <<<<<<<<<<<<<<
  *             # Left side multiplication
  *             self.L[self.n_dims_1] += self.d_location[self.n_dims_1]
  */
       __pyx_t_9 = __pyx_v_self->ur0;
       __pyx_t_10 = __pyx_v_self->ur1;
       __pyx_v_self->ur1 = __pyx_t_9;
       __pyx_v_self->ur0 = __pyx_t_10;
     }
 
-    /* "unipolator/unitary_interpolation_vector.pyx":179
+    /* "unipolator/unitary_interpolation_vector.pyx":180
  *                 self.ur1, self.ur0 = self.ur0, self.ur1
  *             # Left side multiplication
  *             self.L[self.n_dims_1] += self.d_location[self.n_dims_1]             # <<<<<<<<<<<<<<
  *             ind = findex_0(self.L, self.strides_L, self.n_dims)
  *             self.vl = &self.Vl[ind,0,0]
  */
     __pyx_t_4 = __pyx_v_self->n_dims_1;
     __pyx_t_2 = __pyx_v_self->n_dims_1;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_2)) )) += (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_4)) )));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":180
+    /* "unipolator/unitary_interpolation_vector.pyx":181
  *             # Left side multiplication
  *             self.L[self.n_dims_1] += self.d_location[self.n_dims_1]
  *             ind = findex_0(self.L, self.strides_L, self.n_dims)             # <<<<<<<<<<<<<<
  *             self.vl = &self.Vl[ind,0,0]
  *             MM_cdot_pointer_v(self.vl, self.ur0, v0, self.d, self.m)
  */
     __pyx_v_ind = __pyx_f_10unipolator_8indexing_findex_0(__pyx_v_self->L, __pyx_v_self->strides_L, __pyx_v_self->n_dims, 0);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":181
+    /* "unipolator/unitary_interpolation_vector.pyx":182
  *             self.L[self.n_dims_1] += self.d_location[self.n_dims_1]
  *             ind = findex_0(self.L, self.strides_L, self.n_dims)
  *             self.vl = &self.Vl[ind,0,0]             # <<<<<<<<<<<<<<
  *             MM_cdot_pointer_v(self.vl, self.ur0, v0, self.d, self.m)
  * 
  */
     __pyx_t_4 = __pyx_v_ind;
     __pyx_t_2 = 0;
     __pyx_t_3 = 0;
     __pyx_v_self->vl = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->Vl.data + __pyx_t_4 * __pyx_v_self->Vl.strides[0]) ) + __pyx_t_2 * __pyx_v_self->Vl.strides[1]) )) + __pyx_t_3)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":182
+    /* "unipolator/unitary_interpolation_vector.pyx":183
  *             ind = findex_0(self.L, self.strides_L, self.n_dims)
  *             self.vl = &self.Vl[ind,0,0]
  *             MM_cdot_pointer_v(self.vl, self.ur0, v0, self.d, self.m)             # <<<<<<<<<<<<<<
  * 
  *     cdef interpolate_single_u_du(self, double complex *u0, double complex *v0, double complex *du0): #u0, du0 => input the matrices for output   ##int[::1] d_di, -> define earlier
  */
     __pyx_f_10unipolator_22blas_functions_vectors_MM_cdot_pointer_v(__pyx_v_self->vl, __pyx_v_self->ur0, __pyx_v_v0, __pyx_v_self->d, __pyx_v_self->m);
   }
   __pyx_L3:;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":138
+  /* "unipolator/unitary_interpolation_vector.pyx":139
  *         return np.asarray(self.E), np.asarray(self.Vl), np.asarray(self.Vr), np.asarray(self.CL), np.asarray(self.CH), np.asarray(self.strides_E), np.asarray(self.strides_L), np.asarray(self.strides_R), np.asarray(self.strides_C)
  * 
  *     cdef interpolate_single_u(self, double complex *u0, double complex *v0): #u0 => input vectors, v0 => output vectors             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i, j
  *         cdef Py_ssize_t ind
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":184
+/* "unipolator/unitary_interpolation_vector.pyx":185
  *             MM_cdot_pointer_v(self.vl, self.ur0, v0, self.d, self.m)
  * 
  *     cdef interpolate_single_u_du(self, double complex *u0, double complex *v0, double complex *du0): #u0, du0 => input the matrices for output   ##int[::1] d_di, -> define earlier             # <<<<<<<<<<<<<<
  *         # d_di contains the indexes of the derivatives that we want to calculate
  *         cdef Py_ssize_t i, j, ind, curr_d_di
  */
 
@@ -5880,255 +5907,255 @@
   int __pyx_t_6;
   int __pyx_t_7;
   Py_ssize_t __pyx_t_8;
   __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
   __pyx_t_double_complex *__pyx_t_10;
   __Pyx_RefNannySetupContext("interpolate_single_u_du", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":187
+  /* "unipolator/unitary_interpolation_vector.pyx":188
  *         # d_di contains the indexes of the derivatives that we want to calculate
  *         cdef Py_ssize_t i, j, ind, curr_d_di
  *         cdef int curr_d_ind = 0             # <<<<<<<<<<<<<<
  *         cdef double complex *du1 = self.du1 #.copy()
  *         cdef double complex *du2 = self.du2 #.copy()
  */
   __pyx_v_curr_d_ind = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":188
+  /* "unipolator/unitary_interpolation_vector.pyx":189
  *         cdef Py_ssize_t i, j, ind, curr_d_di
  *         cdef int curr_d_ind = 0
  *         cdef double complex *du1 = self.du1 #.copy()             # <<<<<<<<<<<<<<
  *         cdef double complex *du2 = self.du2 #.copy()
  *         cdef double complex *ur0 = self.ur0
  */
   __pyx_t_1 = __pyx_v_self->du1;
   __pyx_v_du1 = __pyx_t_1;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":189
+  /* "unipolator/unitary_interpolation_vector.pyx":190
  *         cdef int curr_d_ind = 0
  *         cdef double complex *du1 = self.du1 #.copy()
  *         cdef double complex *du2 = self.du2 #.copy()             # <<<<<<<<<<<<<<
  *         cdef double complex *ur0 = self.ur0
  *         cdef double complex *ur1 = self.ur1
  */
   __pyx_t_1 = __pyx_v_self->du2;
   __pyx_v_du2 = __pyx_t_1;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":190
+  /* "unipolator/unitary_interpolation_vector.pyx":191
  *         cdef double complex *du1 = self.du1 #.copy()
  *         cdef double complex *du2 = self.du2 #.copy()
  *         cdef double complex *ur0 = self.ur0             # <<<<<<<<<<<<<<
  *         cdef double complex *ur1 = self.ur1
  *         cdef double complex *es0 = self.es0
  */
   __pyx_t_1 = __pyx_v_self->ur0;
   __pyx_v_ur0 = __pyx_t_1;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":191
+  /* "unipolator/unitary_interpolation_vector.pyx":192
  *         cdef double complex *du2 = self.du2 #.copy()
  *         cdef double complex *ur0 = self.ur0
  *         cdef double complex *ur1 = self.ur1             # <<<<<<<<<<<<<<
  *         cdef double complex *es0 = self.es0
  *         if self.n_dims == 1:
  */
   __pyx_t_1 = __pyx_v_self->ur1;
   __pyx_v_ur1 = __pyx_t_1;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":192
+  /* "unipolator/unitary_interpolation_vector.pyx":193
  *         cdef double complex *ur0 = self.ur0
  *         cdef double complex *ur1 = self.ur1
  *         cdef double complex *es0 = self.es0             # <<<<<<<<<<<<<<
  *         if self.n_dims == 1:
  *             ind = self.location[0] + self.d_location[0]
  */
   __pyx_t_1 = __pyx_v_self->es0;
   __pyx_v_es0 = __pyx_t_1;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":193
+  /* "unipolator/unitary_interpolation_vector.pyx":194
  *         cdef double complex *ur1 = self.ur1
  *         cdef double complex *es0 = self.es0
  *         if self.n_dims == 1:             # <<<<<<<<<<<<<<
  *             ind = self.location[0] + self.d_location[0]
  *             self.vr = &self.Vr[ind, 0, 0] # In 1D strides are 1
  */
   __pyx_t_2 = ((__pyx_v_self->n_dims == 1) != 0);
   if (__pyx_t_2) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":194
+    /* "unipolator/unitary_interpolation_vector.pyx":195
  *         cdef double complex *es0 = self.es0
  *         if self.n_dims == 1:
  *             ind = self.location[0] + self.d_location[0]             # <<<<<<<<<<<<<<
  *             self.vr = &self.Vr[ind, 0, 0] # In 1D strides are 1
  *             self.vl = &self.Vl[ind, 0, 0]
  */
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_v_ind = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_3)) ))) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_4)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":195
+    /* "unipolator/unitary_interpolation_vector.pyx":196
  *         if self.n_dims == 1:
  *             ind = self.location[0] + self.d_location[0]
  *             self.vr = &self.Vr[ind, 0, 0] # In 1D strides are 1             # <<<<<<<<<<<<<<
  *             self.vl = &self.Vl[ind, 0, 0]
  *             self.ei = &self.E[ind, 0]
  */
     __pyx_t_4 = __pyx_v_ind;
     __pyx_t_3 = 0;
     __pyx_t_5 = 0;
     __pyx_v_self->vr = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->Vr.data + __pyx_t_4 * __pyx_v_self->Vr.strides[0]) ) + __pyx_t_3 * __pyx_v_self->Vr.strides[1]) )) + __pyx_t_5)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":196
+    /* "unipolator/unitary_interpolation_vector.pyx":197
  *             ind = self.location[0] + self.d_location[0]
  *             self.vr = &self.Vr[ind, 0, 0] # In 1D strides are 1
  *             self.vl = &self.Vl[ind, 0, 0]             # <<<<<<<<<<<<<<
  *             self.ei = &self.E[ind, 0]
  *             MM_cdot_pointer_v(self.vr, u0, ur0,  self.d, self.m)
  */
     __pyx_t_5 = __pyx_v_ind;
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_v_self->vl = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->Vl.data + __pyx_t_5 * __pyx_v_self->Vl.strides[0]) ) + __pyx_t_3 * __pyx_v_self->Vl.strides[1]) )) + __pyx_t_4)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":197
+    /* "unipolator/unitary_interpolation_vector.pyx":198
  *             self.vr = &self.Vr[ind, 0, 0] # In 1D strides are 1
  *             self.vl = &self.Vl[ind, 0, 0]
  *             self.ei = &self.E[ind, 0]             # <<<<<<<<<<<<<<
  *             MM_cdot_pointer_v(self.vr, u0, ur0,  self.d, self.m)
  *             if self.d_di[curr_d_ind] == 0:
  */
     __pyx_t_4 = __pyx_v_ind;
     __pyx_t_3 = 0;
     __pyx_v_self->ei = (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_self->E.data + __pyx_t_4 * __pyx_v_self->E.strides[0]) )) + __pyx_t_3)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":198
+    /* "unipolator/unitary_interpolation_vector.pyx":199
  *             self.vl = &self.Vl[ind, 0, 0]
  *             self.ei = &self.E[ind, 0]
  *             MM_cdot_pointer_v(self.vr, u0, ur0,  self.d, self.m)             # <<<<<<<<<<<<<<
  *             if self.d_di[curr_d_ind] == 0:
  *                 copy_pointer(ur0, du1, self.dm)
  */
     __pyx_f_10unipolator_22blas_functions_vectors_MM_cdot_pointer_v(__pyx_v_self->vr, __pyx_v_u0, __pyx_v_ur0, __pyx_v_self->d, __pyx_v_self->m);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":199
+    /* "unipolator/unitary_interpolation_vector.pyx":200
  *             self.ei = &self.E[ind, 0]
  *             MM_cdot_pointer_v(self.vr, u0, ur0,  self.d, self.m)
  *             if self.d_di[curr_d_ind] == 0:             # <<<<<<<<<<<<<<
  *                 copy_pointer(ur0, du1, self.dm)
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)
  */
     __pyx_t_3 = __pyx_v_curr_d_ind;
     __pyx_t_2 = (((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_di.data) + __pyx_t_3)) ))) == 0) != 0);
     if (__pyx_t_2) {
 
-      /* "unipolator/unitary_interpolation_vector.pyx":200
+      /* "unipolator/unitary_interpolation_vector.pyx":201
  *             MM_cdot_pointer_v(self.vr, u0, ur0,  self.d, self.m)
  *             if self.d_di[curr_d_ind] == 0:
  *                 copy_pointer(ur0, du1, self.dm)             # <<<<<<<<<<<<<<
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)
  *                 MM_cdot_pointer_v(self.vl, self.du1, du0, self.d, self.m)
  */
       __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_ur0, __pyx_v_du1, __pyx_v_self->dm);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":201
+      /* "unipolator/unitary_interpolation_vector.pyx":202
  *             if self.d_di[curr_d_ind] == 0:
  *                 copy_pointer(ur0, du1, self.dm)
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)             # <<<<<<<<<<<<<<
  *                 MM_cdot_pointer_v(self.vl, self.du1, du0, self.d, self.m)
  *             v_exp_pointer_v(self.ei, ur0, self.abs_alpha_rest[0], self.d, self.m)
  */
       __pyx_t_3 = 0;
       __pyx_t_4 = 0;
       __pyx_t_5 = 0;
       __pyx_f_10unipolator_22blas_functions_vectors_v_exp_v_pointer_v(((((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_3)) ))) * 2) + 1) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->das.data) + __pyx_t_4)) )))), __pyx_v_self->ei, __pyx_v_du1, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_5)) ))), __pyx_v_self->d, __pyx_v_self->m);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":202
+      /* "unipolator/unitary_interpolation_vector.pyx":203
  *                 copy_pointer(ur0, du1, self.dm)
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)
  *                 MM_cdot_pointer_v(self.vl, self.du1, du0, self.d, self.m)             # <<<<<<<<<<<<<<
  *             v_exp_pointer_v(self.ei, ur0, self.abs_alpha_rest[0], self.d, self.m)
  *             MM_cdot_pointer_v(self.vl, ur0, v0, self.d, self.m)
  */
       __pyx_f_10unipolator_22blas_functions_vectors_MM_cdot_pointer_v(__pyx_v_self->vl, __pyx_v_self->du1, __pyx_v_du0, __pyx_v_self->d, __pyx_v_self->m);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":199
+      /* "unipolator/unitary_interpolation_vector.pyx":200
  *             self.ei = &self.E[ind, 0]
  *             MM_cdot_pointer_v(self.vr, u0, ur0,  self.d, self.m)
  *             if self.d_di[curr_d_ind] == 0:             # <<<<<<<<<<<<<<
  *                 copy_pointer(ur0, du1, self.dm)
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)
  */
     }
 
-    /* "unipolator/unitary_interpolation_vector.pyx":203
+    /* "unipolator/unitary_interpolation_vector.pyx":204
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)
  *                 MM_cdot_pointer_v(self.vl, self.du1, du0, self.d, self.m)
  *             v_exp_pointer_v(self.ei, ur0, self.abs_alpha_rest[0], self.d, self.m)             # <<<<<<<<<<<<<<
  *             MM_cdot_pointer_v(self.vl, ur0, v0, self.d, self.m)
  *         else:
  */
     __pyx_t_5 = 0;
     __pyx_f_10unipolator_22blas_functions_vectors_v_exp_pointer_v(__pyx_v_self->ei, __pyx_v_ur0, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_5)) ))), __pyx_v_self->d, __pyx_v_self->m);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":204
+    /* "unipolator/unitary_interpolation_vector.pyx":205
  *                 MM_cdot_pointer_v(self.vl, self.du1, du0, self.d, self.m)
  *             v_exp_pointer_v(self.ei, ur0, self.abs_alpha_rest[0], self.d, self.m)
  *             MM_cdot_pointer_v(self.vl, ur0, v0, self.d, self.m)             # <<<<<<<<<<<<<<
  *         else:
  *             # Track the number of performed derivatives via curr_d_ind, the indexes to perform with self.d_di and the next derivative to perform with self.d_di[curr_d_ind] == curr_d_di
  */
     __pyx_f_10unipolator_22blas_functions_vectors_MM_cdot_pointer_v(__pyx_v_self->vl, __pyx_v_ur0, __pyx_v_v0, __pyx_v_self->d, __pyx_v_self->m);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":193
+    /* "unipolator/unitary_interpolation_vector.pyx":194
  *         cdef double complex *ur1 = self.ur1
  *         cdef double complex *es0 = self.es0
  *         if self.n_dims == 1:             # <<<<<<<<<<<<<<
  *             ind = self.location[0] + self.d_location[0]
  *             self.vr = &self.Vr[ind, 0, 0] # In 1D strides are 1
  */
     goto __pyx_L3;
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":208
+  /* "unipolator/unitary_interpolation_vector.pyx":209
  *             # Track the number of performed derivatives via curr_d_ind, the indexes to perform with self.d_di and the next derivative to perform with self.d_di[curr_d_ind] == curr_d_di
  *             # Right side first
  *             self.L[0] = self.location[0] + self.d_location[0]             # <<<<<<<<<<<<<<
  *             for i in range(1, self.n_dims):
  *                 self.L[i] = self.location[i]
  */
   /*else*/ {
     __pyx_t_5 = 0;
     __pyx_t_4 = 0;
     __pyx_t_3 = 0;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_3)) )) = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_5)) ))) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_4)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":209
+    /* "unipolator/unitary_interpolation_vector.pyx":210
  *             # Right side first
  *             self.L[0] = self.location[0] + self.d_location[0]
  *             for i in range(1, self.n_dims):             # <<<<<<<<<<<<<<
  *                 self.L[i] = self.location[i]
  *             ind = findex_0(self.L, self.strides_E[0,:], self.n_dims)
  */
     __pyx_t_6 = __pyx_v_self->n_dims;
     __pyx_t_7 = __pyx_t_6;
     for (__pyx_t_8 = 1; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
       __pyx_v_i = __pyx_t_8;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":210
+      /* "unipolator/unitary_interpolation_vector.pyx":211
  *             self.L[0] = self.location[0] + self.d_location[0]
  *             for i in range(1, self.n_dims):
  *                 self.L[i] = self.location[i]             # <<<<<<<<<<<<<<
  *             ind = findex_0(self.L, self.strides_E[0,:], self.n_dims)
  *             self.vr = &self.Vr[ind, 0, 0]  # In 1D strides are 1
  */
       __pyx_t_4 = __pyx_v_i;
       __pyx_t_5 = __pyx_v_i;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_5)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_4)) )));
     }
 
-    /* "unipolator/unitary_interpolation_vector.pyx":211
+    /* "unipolator/unitary_interpolation_vector.pyx":212
  *             for i in range(1, self.n_dims):
  *                 self.L[i] = self.location[i]
  *             ind = findex_0(self.L, self.strides_E[0,:], self.n_dims)             # <<<<<<<<<<<<<<
  *             self.vr = &self.Vr[ind, 0, 0]  # In 1D strides are 1
  *             self.ei = &self.E[ind, 0]
  */
     __pyx_t_9.data = __pyx_v_self->strides_E.data;
@@ -6145,169 +6172,169 @@
     __pyx_t_9.suboffsets[0] = -1;
 
 __pyx_v_ind = __pyx_f_10unipolator_8indexing_findex_0(__pyx_v_self->L, __pyx_t_9, __pyx_v_self->n_dims, 0);
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":212
+    /* "unipolator/unitary_interpolation_vector.pyx":213
  *                 self.L[i] = self.location[i]
  *             ind = findex_0(self.L, self.strides_E[0,:], self.n_dims)
  *             self.vr = &self.Vr[ind, 0, 0]  # In 1D strides are 1             # <<<<<<<<<<<<<<
  *             self.ei = &self.E[ind, 0]
  * 
  */
     __pyx_t_4 = __pyx_v_ind;
     __pyx_t_5 = 0;
     __pyx_t_3 = 0;
     __pyx_v_self->vr = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->Vr.data + __pyx_t_4 * __pyx_v_self->Vr.strides[0]) ) + __pyx_t_5 * __pyx_v_self->Vr.strides[1]) )) + __pyx_t_3)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":213
+    /* "unipolator/unitary_interpolation_vector.pyx":214
  *             ind = findex_0(self.L, self.strides_E[0,:], self.n_dims)
  *             self.vr = &self.Vr[ind, 0, 0]  # In 1D strides are 1
  *             self.ei = &self.E[ind, 0]             # <<<<<<<<<<<<<<
  * 
  *             MM_cdot_pointer_v(self.vr, u0, ur0, self.d, self.m) # now ur0 and du1
  */
     __pyx_t_3 = __pyx_v_ind;
     __pyx_t_5 = 0;
     __pyx_v_self->ei = (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_self->E.data + __pyx_t_3 * __pyx_v_self->E.strides[0]) )) + __pyx_t_5)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":215
+    /* "unipolator/unitary_interpolation_vector.pyx":216
  *             self.ei = &self.E[ind, 0]
  * 
  *             MM_cdot_pointer_v(self.vr, u0, ur0, self.d, self.m) # now ur0 and du1             # <<<<<<<<<<<<<<
  *             curr_d_di = self.d_di[curr_d_ind]
  *             if curr_d_di == 0:
  */
     __pyx_f_10unipolator_22blas_functions_vectors_MM_cdot_pointer_v(__pyx_v_self->vr, __pyx_v_u0, __pyx_v_ur0, __pyx_v_self->d, __pyx_v_self->m);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":216
+    /* "unipolator/unitary_interpolation_vector.pyx":217
  * 
  *             MM_cdot_pointer_v(self.vr, u0, ur0, self.d, self.m) # now ur0 and du1
  *             curr_d_di = self.d_di[curr_d_ind]             # <<<<<<<<<<<<<<
  *             if curr_d_di == 0:
  *                 copy_pointer(ur0, du1, self.dm)
  */
     __pyx_t_5 = __pyx_v_curr_d_ind;
     __pyx_v_curr_d_di = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_di.data) + __pyx_t_5)) )));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":217
+    /* "unipolator/unitary_interpolation_vector.pyx":218
  *             MM_cdot_pointer_v(self.vr, u0, ur0, self.d, self.m) # now ur0 and du1
  *             curr_d_di = self.d_di[curr_d_ind]
  *             if curr_d_di == 0:             # <<<<<<<<<<<<<<
  *                 copy_pointer(ur0, du1, self.dm)
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)
  */
     __pyx_t_2 = ((__pyx_v_curr_d_di == 0) != 0);
     if (__pyx_t_2) {
 
-      /* "unipolator/unitary_interpolation_vector.pyx":218
+      /* "unipolator/unitary_interpolation_vector.pyx":219
  *             curr_d_di = self.d_di[curr_d_ind]
  *             if curr_d_di == 0:
  *                 copy_pointer(ur0, du1, self.dm)             # <<<<<<<<<<<<<<
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)
  *                 curr_d_ind += 1
  */
       __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_ur0, __pyx_v_du1, __pyx_v_self->dm);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":219
+      /* "unipolator/unitary_interpolation_vector.pyx":220
  *             if curr_d_di == 0:
  *                 copy_pointer(ur0, du1, self.dm)
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)             # <<<<<<<<<<<<<<
  *                 curr_d_ind += 1
  *                 curr_d_di = self.d_di[curr_d_ind]
  */
       __pyx_t_5 = 0;
       __pyx_t_3 = 0;
       __pyx_t_4 = 0;
       __pyx_f_10unipolator_22blas_functions_vectors_v_exp_v_pointer_v(((((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_5)) ))) * 2) + 1) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->das.data) + __pyx_t_3)) )))), __pyx_v_self->ei, __pyx_v_du1, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_4)) ))), __pyx_v_self->d, __pyx_v_self->m);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":220
+      /* "unipolator/unitary_interpolation_vector.pyx":221
  *                 copy_pointer(ur0, du1, self.dm)
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)
  *                 curr_d_ind += 1             # <<<<<<<<<<<<<<
  *                 curr_d_di = self.d_di[curr_d_ind]
  *             v_exp_pointer_v(self.ei, ur0, self.abs_alpha_rest[0], self.d, self.m) # still ur0 and du1
  */
       __pyx_v_curr_d_ind = (__pyx_v_curr_d_ind + 1);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":221
+      /* "unipolator/unitary_interpolation_vector.pyx":222
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)
  *                 curr_d_ind += 1
  *                 curr_d_di = self.d_di[curr_d_ind]             # <<<<<<<<<<<<<<
  *             v_exp_pointer_v(self.ei, ur0, self.abs_alpha_rest[0], self.d, self.m) # still ur0 and du1
  * 
  */
       __pyx_t_4 = __pyx_v_curr_d_ind;
       __pyx_v_curr_d_di = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_di.data) + __pyx_t_4)) )));
 
-      /* "unipolator/unitary_interpolation_vector.pyx":217
+      /* "unipolator/unitary_interpolation_vector.pyx":218
  *             MM_cdot_pointer_v(self.vr, u0, ur0, self.d, self.m) # now ur0 and du1
  *             curr_d_di = self.d_di[curr_d_ind]
  *             if curr_d_di == 0:             # <<<<<<<<<<<<<<
  *                 copy_pointer(ur0, du1, self.dm)
  *                 v_exp_v_pointer_v( (self.d_location[0]*2+1)*self.das[0], self.ei, du1, self.abs_alpha_rest[0], self.d, self.m) # -i*E*amp*exp(-i*E*t)
  */
     }
 
-    /* "unipolator/unitary_interpolation_vector.pyx":222
+    /* "unipolator/unitary_interpolation_vector.pyx":223
  *                 curr_d_ind += 1
  *                 curr_d_di = self.d_di[curr_d_ind]
  *             v_exp_pointer_v(self.ei, ur0, self.abs_alpha_rest[0], self.d, self.m) # still ur0 and du1             # <<<<<<<<<<<<<<
  * 
  *             self.L[0] = self.location[0]
  */
     __pyx_t_4 = 0;
     __pyx_f_10unipolator_22blas_functions_vectors_v_exp_pointer_v(__pyx_v_self->ei, __pyx_v_ur0, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_4)) ))), __pyx_v_self->d, __pyx_v_self->m);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":224
+    /* "unipolator/unitary_interpolation_vector.pyx":225
  *             v_exp_pointer_v(self.ei, ur0, self.abs_alpha_rest[0], self.d, self.m) # still ur0 and du1
  * 
  *             self.L[0] = self.location[0]             # <<<<<<<<<<<<<<
  *             # Center multiplications
  *             for i in range(self.n_dims_1):
  */
     __pyx_t_4 = 0;
     __pyx_t_3 = 0;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_3)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_4)) )));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":226
+    /* "unipolator/unitary_interpolation_vector.pyx":227
  *             self.L[0] = self.location[0]
  *             # Center multiplications
  *             for i in range(self.n_dims_1):             # <<<<<<<<<<<<<<
  *                 j = i + 1
  *                 self.L[j] += self.d_location[j]
  */
     __pyx_t_6 = __pyx_v_self->n_dims_1;
     __pyx_t_7 = __pyx_t_6;
     for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
       __pyx_v_i = __pyx_t_8;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":227
+      /* "unipolator/unitary_interpolation_vector.pyx":228
  *             # Center multiplications
  *             for i in range(self.n_dims_1):
  *                 j = i + 1             # <<<<<<<<<<<<<<
  *                 self.L[j] += self.d_location[j]
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]
  */
       __pyx_v_j = (__pyx_v_i + 1);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":228
+      /* "unipolator/unitary_interpolation_vector.pyx":229
  *             for i in range(self.n_dims_1):
  *                 j = i + 1
  *                 self.L[j] += self.d_location[j]             # <<<<<<<<<<<<<<
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]
  *                 self.ei = &self.E[ind, 0]
  */
       __pyx_t_4 = __pyx_v_j;
       __pyx_t_3 = __pyx_v_j;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_3)) )) += (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_4)) )));
 
-      /* "unipolator/unitary_interpolation_vector.pyx":229
+      /* "unipolator/unitary_interpolation_vector.pyx":230
  *                 j = i + 1
  *                 self.L[j] += self.d_location[j]
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]             # <<<<<<<<<<<<<<
  *                 self.ei = &self.E[ind, 0]
  *                 if self.d_location[i]:  ### Higher
  */
       __pyx_t_9.data = __pyx_v_self->strides_E.data;
@@ -6325,47 +6352,47 @@
 
 __pyx_t_4 = __pyx_v_j;
       __pyx_v_ind = (__pyx_f_10unipolator_8indexing_findex_0(__pyx_v_self->L, __pyx_t_9, __pyx_v_self->n_dims, 0) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->first_elements_E.data) + __pyx_t_4)) ))));
       __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
       __pyx_t_9.memview = NULL;
       __pyx_t_9.data = NULL;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":230
+      /* "unipolator/unitary_interpolation_vector.pyx":231
  *                 self.L[j] += self.d_location[j]
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]
  *                 self.ei = &self.E[ind, 0]             # <<<<<<<<<<<<<<
  *                 if self.d_location[i]:  ### Higher
  *                     self.L[i] += -1
  */
       __pyx_t_4 = __pyx_v_ind;
       __pyx_t_3 = 0;
       __pyx_v_self->ei = (&(*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_self->E.data + __pyx_t_4 * __pyx_v_self->E.strides[0]) )) + __pyx_t_3)) ))));
 
-      /* "unipolator/unitary_interpolation_vector.pyx":231
+      /* "unipolator/unitary_interpolation_vector.pyx":232
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]
  *                 self.ei = &self.E[ind, 0]
  *                 if self.d_location[i]:  ### Higher             # <<<<<<<<<<<<<<
  *                     self.L[i] += -1
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  */
       __pyx_t_3 = __pyx_v_i;
       __pyx_t_2 = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_3)) ))) != 0);
       if (__pyx_t_2) {
 
-        /* "unipolator/unitary_interpolation_vector.pyx":232
+        /* "unipolator/unitary_interpolation_vector.pyx":233
  *                 self.ei = &self.E[ind, 0]
  *                 if self.d_location[i]:  ### Higher
  *                     self.L[i] += -1             # <<<<<<<<<<<<<<
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  *                     self.c = &self.CL[ind, 0, 0]
  */
         __pyx_t_3 = __pyx_v_i;
         *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_3)) )) += -1L;
 
-        /* "unipolator/unitary_interpolation_vector.pyx":233
+        /* "unipolator/unitary_interpolation_vector.pyx":234
  *                 if self.d_location[i]:  ### Higher
  *                     self.L[i] += -1
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]             # <<<<<<<<<<<<<<
  *                     self.c = &self.CL[ind, 0, 0]
  *                     self.L[i] += 1  # Restore value
  */
         __pyx_t_9.data = __pyx_v_self->strides_C.data;
@@ -6383,47 +6410,47 @@
 
 __pyx_t_3 = __pyx_v_i;
         __pyx_v_ind = (__pyx_f_10unipolator_8indexing_findex_0(__pyx_v_self->L, __pyx_t_9, __pyx_v_self->n_dims, 0) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->first_elements_C.data) + __pyx_t_3)) ))));
         __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
         __pyx_t_9.memview = NULL;
         __pyx_t_9.data = NULL;
 
-        /* "unipolator/unitary_interpolation_vector.pyx":234
+        /* "unipolator/unitary_interpolation_vector.pyx":235
  *                     self.L[i] += -1
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  *                     self.c = &self.CL[ind, 0, 0]             # <<<<<<<<<<<<<<
  *                     self.L[i] += 1  # Restore value
  *                 else:                        ### Lower
  */
         __pyx_t_3 = __pyx_v_ind;
         __pyx_t_4 = 0;
         __pyx_t_5 = 0;
         __pyx_v_self->c = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->CL.data + __pyx_t_3 * __pyx_v_self->CL.strides[0]) ) + __pyx_t_4 * __pyx_v_self->CL.strides[1]) )) + __pyx_t_5)) ))));
 
-        /* "unipolator/unitary_interpolation_vector.pyx":235
+        /* "unipolator/unitary_interpolation_vector.pyx":236
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  *                     self.c = &self.CL[ind, 0, 0]
  *                     self.L[i] += 1  # Restore value             # <<<<<<<<<<<<<<
  *                 else:                        ### Lower
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims)+self.first_elements_C[i]
  */
         __pyx_t_5 = __pyx_v_i;
         *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_5)) )) += 1;
 
-        /* "unipolator/unitary_interpolation_vector.pyx":231
+        /* "unipolator/unitary_interpolation_vector.pyx":232
  *                 ind = findex_0(self.L, self.strides_E[j, :], self.n_dims) + self.first_elements_E[j]
  *                 self.ei = &self.E[ind, 0]
  *                 if self.d_location[i]:  ### Higher             # <<<<<<<<<<<<<<
  *                     self.L[i] += -1
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims) + self.first_elements_C[i]
  */
         goto __pyx_L10;
       }
 
-      /* "unipolator/unitary_interpolation_vector.pyx":237
+      /* "unipolator/unitary_interpolation_vector.pyx":238
  *                     self.L[i] += 1  # Restore value
  *                 else:                        ### Lower
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims)+self.first_elements_C[i]             # <<<<<<<<<<<<<<
  *                     self.c = &self.CH[ind,0,0]
  *                 self.L[j] = self.location[j]
  */
       /*else*/ {
@@ -6442,197 +6469,197 @@
 
 __pyx_t_5 = __pyx_v_i;
         __pyx_v_ind = (__pyx_f_10unipolator_8indexing_findex_0(__pyx_v_self->L, __pyx_t_9, __pyx_v_self->n_dims, 0) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->first_elements_C.data) + __pyx_t_5)) ))));
         __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
         __pyx_t_9.memview = NULL;
         __pyx_t_9.data = NULL;
 
-        /* "unipolator/unitary_interpolation_vector.pyx":238
+        /* "unipolator/unitary_interpolation_vector.pyx":239
  *                 else:                        ### Lower
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims)+self.first_elements_C[i]
  *                     self.c = &self.CH[ind,0,0]             # <<<<<<<<<<<<<<
  *                 self.L[j] = self.location[j]
  *                 # Batch matrix multiply
  */
         __pyx_t_5 = __pyx_v_ind;
         __pyx_t_4 = 0;
         __pyx_t_3 = 0;
         __pyx_v_self->c = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->CH.data + __pyx_t_5 * __pyx_v_self->CH.strides[0]) ) + __pyx_t_4 * __pyx_v_self->CH.strides[1]) )) + __pyx_t_3)) ))));
       }
       __pyx_L10:;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":239
+      /* "unipolator/unitary_interpolation_vector.pyx":240
  *                     ind = findex_0(self.L, self.strides_C[i, :], self.n_dims)+self.first_elements_C[i]
  *                     self.c = &self.CH[ind,0,0]
  *                 self.L[j] = self.location[j]             # <<<<<<<<<<<<<<
  *                 # Batch matrix multiply
  *                 MM_cdot_pointer_batch_v(self.c, ur0, ur1, du1, du2, self.d, self.m, self.dm, curr_d_ind) # now ur1 and du2
  */
       __pyx_t_3 = __pyx_v_j;
       __pyx_t_4 = __pyx_v_j;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_4)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_3)) )));
 
-      /* "unipolator/unitary_interpolation_vector.pyx":241
+      /* "unipolator/unitary_interpolation_vector.pyx":242
  *                 self.L[j] = self.location[j]
  *                 # Batch matrix multiply
  *                 MM_cdot_pointer_batch_v(self.c, ur0, ur1, du1, du2, self.d, self.m, self.dm, curr_d_ind) # now ur1 and du2             # <<<<<<<<<<<<<<
  *                 # Perform the row wise complex scaling, with potential derivative
  *                 if curr_d_di == j: # Add derivative here
  */
       __pyx_f_10unipolator_22blas_functions_vectors_MM_cdot_pointer_batch_v(__pyx_v_self->c, __pyx_v_ur0, __pyx_v_ur1, __pyx_v_du1, __pyx_v_du2, __pyx_v_self->d, __pyx_v_self->m, __pyx_v_self->dm, __pyx_v_curr_d_ind);
 
-      /* "unipolator/unitary_interpolation_vector.pyx":243
+      /* "unipolator/unitary_interpolation_vector.pyx":244
  *                 MM_cdot_pointer_batch_v(self.c, ur0, ur1, du1, du2, self.d, self.m, self.dm, curr_d_ind) # now ur1 and du2
  *                 # Perform the row wise complex scaling, with potential derivative
  *                 if curr_d_di == j: # Add derivative here             # <<<<<<<<<<<<<<
  *                     v_exp_v_and_v_exp_pointer_v_batch_increment((self.d_location[curr_d_di]*2+1)*self.das[curr_d_di], self.ei, es0, ur1, du2, self.abs_alpha_rest[j], self.d, self.m, self.dm, curr_d_ind)
  *                     curr_d_ind += 1
  */
       __pyx_t_2 = ((__pyx_v_curr_d_di == __pyx_v_j) != 0);
       if (__pyx_t_2) {
 
-        /* "unipolator/unitary_interpolation_vector.pyx":244
+        /* "unipolator/unitary_interpolation_vector.pyx":245
  *                 # Perform the row wise complex scaling, with potential derivative
  *                 if curr_d_di == j: # Add derivative here
  *                     v_exp_v_and_v_exp_pointer_v_batch_increment((self.d_location[curr_d_di]*2+1)*self.das[curr_d_di], self.ei, es0, ur1, du2, self.abs_alpha_rest[j], self.d, self.m, self.dm, curr_d_ind)             # <<<<<<<<<<<<<<
  *                     curr_d_ind += 1
  *                     curr_d_di = self.d_di[curr_d_ind]
  */
         __pyx_t_3 = __pyx_v_curr_d_di;
         __pyx_t_4 = __pyx_v_curr_d_di;
         __pyx_t_5 = __pyx_v_j;
         __pyx_f_10unipolator_22blas_functions_vectors_v_exp_v_and_v_exp_pointer_v_batch_increment(((((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_3)) ))) * 2) + 1) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->das.data) + __pyx_t_4)) )))), __pyx_v_self->ei, __pyx_v_es0, __pyx_v_ur1, __pyx_v_du2, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_5)) ))), __pyx_v_self->d, __pyx_v_self->m, __pyx_v_self->dm, __pyx_v_curr_d_ind);
 
-        /* "unipolator/unitary_interpolation_vector.pyx":245
+        /* "unipolator/unitary_interpolation_vector.pyx":246
  *                 if curr_d_di == j: # Add derivative here
  *                     v_exp_v_and_v_exp_pointer_v_batch_increment((self.d_location[curr_d_di]*2+1)*self.das[curr_d_di], self.ei, es0, ur1, du2, self.abs_alpha_rest[j], self.d, self.m, self.dm, curr_d_ind)
  *                     curr_d_ind += 1             # <<<<<<<<<<<<<<
  *                     curr_d_di = self.d_di[curr_d_ind]
  *                 else:
  */
         __pyx_v_curr_d_ind = (__pyx_v_curr_d_ind + 1);
 
-        /* "unipolator/unitary_interpolation_vector.pyx":246
+        /* "unipolator/unitary_interpolation_vector.pyx":247
  *                     v_exp_v_and_v_exp_pointer_v_batch_increment((self.d_location[curr_d_di]*2+1)*self.das[curr_d_di], self.ei, es0, ur1, du2, self.abs_alpha_rest[j], self.d, self.m, self.dm, curr_d_ind)
  *                     curr_d_ind += 1
  *                     curr_d_di = self.d_di[curr_d_ind]             # <<<<<<<<<<<<<<
  *                 else:
  *                     v_exp_v_and_v_exp_pointer_v_batch(self.ei, self.es0, ur1, du2, self.abs_alpha_rest[j], self.d, self.m, curr_d_ind)
  */
         __pyx_t_5 = __pyx_v_curr_d_ind;
         __pyx_v_curr_d_di = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_di.data) + __pyx_t_5)) )));
 
-        /* "unipolator/unitary_interpolation_vector.pyx":243
+        /* "unipolator/unitary_interpolation_vector.pyx":244
  *                 MM_cdot_pointer_batch_v(self.c, ur0, ur1, du1, du2, self.d, self.m, self.dm, curr_d_ind) # now ur1 and du2
  *                 # Perform the row wise complex scaling, with potential derivative
  *                 if curr_d_di == j: # Add derivative here             # <<<<<<<<<<<<<<
  *                     v_exp_v_and_v_exp_pointer_v_batch_increment((self.d_location[curr_d_di]*2+1)*self.das[curr_d_di], self.ei, es0, ur1, du2, self.abs_alpha_rest[j], self.d, self.m, self.dm, curr_d_ind)
  *                     curr_d_ind += 1
  */
         goto __pyx_L11;
       }
 
-      /* "unipolator/unitary_interpolation_vector.pyx":248
+      /* "unipolator/unitary_interpolation_vector.pyx":249
  *                     curr_d_di = self.d_di[curr_d_ind]
  *                 else:
  *                     v_exp_v_and_v_exp_pointer_v_batch(self.ei, self.es0, ur1, du2, self.abs_alpha_rest[j], self.d, self.m, curr_d_ind)             # <<<<<<<<<<<<<<
  *                 ur1, ur0 = ur0, ur1 # now flip them
  *                 du2, du1 = du1, du2
  */
       /*else*/ {
         __pyx_t_5 = __pyx_v_j;
         __pyx_f_10unipolator_22blas_functions_vectors_v_exp_v_and_v_exp_pointer_v_batch(__pyx_v_self->ei, __pyx_v_self->es0, __pyx_v_ur1, __pyx_v_du2, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_self->abs_alpha_rest.data) + __pyx_t_5)) ))), __pyx_v_self->d, __pyx_v_self->m, __pyx_v_curr_d_ind);
       }
       __pyx_L11:;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":249
+      /* "unipolator/unitary_interpolation_vector.pyx":250
  *                 else:
  *                     v_exp_v_and_v_exp_pointer_v_batch(self.ei, self.es0, ur1, du2, self.abs_alpha_rest[j], self.d, self.m, curr_d_ind)
  *                 ur1, ur0 = ur0, ur1 # now flip them             # <<<<<<<<<<<<<<
  *                 du2, du1 = du1, du2
  *             # Left side multiplication
  */
       __pyx_t_1 = __pyx_v_ur0;
       __pyx_t_10 = __pyx_v_ur1;
       __pyx_v_ur1 = __pyx_t_1;
       __pyx_v_ur0 = __pyx_t_10;
 
-      /* "unipolator/unitary_interpolation_vector.pyx":250
+      /* "unipolator/unitary_interpolation_vector.pyx":251
  *                     v_exp_v_and_v_exp_pointer_v_batch(self.ei, self.es0, ur1, du2, self.abs_alpha_rest[j], self.d, self.m, curr_d_ind)
  *                 ur1, ur0 = ur0, ur1 # now flip them
  *                 du2, du1 = du1, du2             # <<<<<<<<<<<<<<
  *             # Left side multiplication
  *             self.L[self.n_dims_1] = self.location[self.n_dims_1] + self.d_location[self.n_dims_1]
  */
       __pyx_t_10 = __pyx_v_du1;
       __pyx_t_1 = __pyx_v_du2;
       __pyx_v_du2 = __pyx_t_10;
       __pyx_v_du1 = __pyx_t_1;
     }
 
-    /* "unipolator/unitary_interpolation_vector.pyx":252
+    /* "unipolator/unitary_interpolation_vector.pyx":253
  *                 du2, du1 = du1, du2
  *             # Left side multiplication
  *             self.L[self.n_dims_1] = self.location[self.n_dims_1] + self.d_location[self.n_dims_1]             # <<<<<<<<<<<<<<
  *             ind = findex_0(self.L, self.strides_L, self.n_dims)
  *             self.vl = &self.Vl[ind,0,0]
  */
     __pyx_t_5 = __pyx_v_self->n_dims_1;
     __pyx_t_4 = __pyx_v_self->n_dims_1;
     __pyx_t_3 = __pyx_v_self->n_dims_1;
     *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->L.data) + __pyx_t_3)) )) = ((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->location.data) + __pyx_t_5)) ))) + (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_self->d_location.data) + __pyx_t_4)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":253
+    /* "unipolator/unitary_interpolation_vector.pyx":254
  *             # Left side multiplication
  *             self.L[self.n_dims_1] = self.location[self.n_dims_1] + self.d_location[self.n_dims_1]
  *             ind = findex_0(self.L, self.strides_L, self.n_dims)             # <<<<<<<<<<<<<<
  *             self.vl = &self.Vl[ind,0,0]
  *             MM_cdot_pointer_batch_v(self.vl, ur0, v0, du1, du0, self.d, self.m, self.dm, curr_d_ind) # now ur1 and du2
  */
     __pyx_v_ind = __pyx_f_10unipolator_8indexing_findex_0(__pyx_v_self->L, __pyx_v_self->strides_L, __pyx_v_self->n_dims, 0);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":254
+    /* "unipolator/unitary_interpolation_vector.pyx":255
  *             self.L[self.n_dims_1] = self.location[self.n_dims_1] + self.d_location[self.n_dims_1]
  *             ind = findex_0(self.L, self.strides_L, self.n_dims)
  *             self.vl = &self.Vl[ind,0,0]             # <<<<<<<<<<<<<<
  *             MM_cdot_pointer_batch_v(self.vl, ur0, v0, du1, du0, self.d, self.m, self.dm, curr_d_ind) # now ur1 and du2
  * 
  */
     __pyx_t_4 = __pyx_v_ind;
     __pyx_t_5 = 0;
     __pyx_t_3 = 0;
     __pyx_v_self->vl = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_self->Vl.data + __pyx_t_4 * __pyx_v_self->Vl.strides[0]) ) + __pyx_t_5 * __pyx_v_self->Vl.strides[1]) )) + __pyx_t_3)) ))));
 
-    /* "unipolator/unitary_interpolation_vector.pyx":255
+    /* "unipolator/unitary_interpolation_vector.pyx":256
  *             ind = findex_0(self.L, self.strides_L, self.n_dims)
  *             self.vl = &self.Vl[ind,0,0]
  *             MM_cdot_pointer_batch_v(self.vl, ur0, v0, du1, du0, self.d, self.m, self.dm, curr_d_ind) # now ur1 and du2             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_f_10unipolator_22blas_functions_vectors_MM_cdot_pointer_batch_v(__pyx_v_self->vl, __pyx_v_ur0, __pyx_v_v0, __pyx_v_du1, __pyx_v_du0, __pyx_v_self->d, __pyx_v_self->m, __pyx_v_self->dm, __pyx_v_curr_d_ind);
   }
   __pyx_L3:;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":184
+  /* "unipolator/unitary_interpolation_vector.pyx":185
  *             MM_cdot_pointer_v(self.vl, self.ur0, v0, self.d, self.m)
  * 
  *     cdef interpolate_single_u_du(self, double complex *u0, double complex *v0, double complex *du0): #u0, du0 => input the matrices for output   ##int[::1] d_di, -> define earlier             # <<<<<<<<<<<<<<
  *         # d_di contains the indexes of the derivatives that we want to calculate
  *         cdef Py_ssize_t i, j, ind, curr_d_di
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":258
+/* "unipolator/unitary_interpolation_vector.pyx":259
  * 
  * 
  *     cdef expmH_pointer(self, double[::1] c, double complex *u0, double complex *v0):             # <<<<<<<<<<<<<<
  *         self.single_parameters2oddgrid(c)
  *         self.interpolate_single_u(u0, v0)
  */
 
@@ -6641,37 +6668,37 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expmH_pointer", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":259
+  /* "unipolator/unitary_interpolation_vector.pyx":260
  * 
  *     cdef expmH_pointer(self, double[::1] c, double complex *u0, double complex *v0):
  *         self.single_parameters2oddgrid(c)             # <<<<<<<<<<<<<<
  *         self.interpolate_single_u(u0, v0)
  *     def expmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_v_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_v_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":260
+  /* "unipolator/unitary_interpolation_vector.pyx":261
  *     cdef expmH_pointer(self, double[::1] c, double complex *u0, double complex *v0):
  *         self.single_parameters2oddgrid(c)
  *         self.interpolate_single_u(u0, v0)             # <<<<<<<<<<<<<<
  *     def expmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out):
  *         if not c.shape[0] == self.n_dims:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->interpolate_single_u(__pyx_v_self, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->interpolate_single_u(__pyx_v_self, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":258
+  /* "unipolator/unitary_interpolation_vector.pyx":259
  * 
  * 
  *     cdef expmH_pointer(self, double[::1] c, double complex *u0, double complex *v0):             # <<<<<<<<<<<<<<
  *         self.single_parameters2oddgrid(c)
  *         self.interpolate_single_u(u0, v0)
  */
 
@@ -6684,15 +6711,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":261
+/* "unipolator/unitary_interpolation_vector.pyx":262
  *         self.single_parameters2oddgrid(c)
  *         self.interpolate_single_u(u0, v0)
  *     def expmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out):             # <<<<<<<<<<<<<<
  *         if not c.shape[0] == self.n_dims:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  */
 
@@ -6730,40 +6757,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_V_in)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("expmH", 1, 3, 3, 1); __PYX_ERR(0, 261, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("expmH", 1, 3, 3, 1); __PYX_ERR(0, 262, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_V_out)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("expmH", 1, 3, 3, 2); __PYX_ERR(0, 261, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("expmH", 1, 3, 3, 2); __PYX_ERR(0, 262, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH") < 0)) __PYX_ERR(0, 261, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH") < 0)) __PYX_ERR(0, 262, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 261, __pyx_L3_error)
-    __pyx_v_V_in = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_in.memview)) __PYX_ERR(0, 261, __pyx_L3_error)
-    __pyx_v_V_out = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_out.memview)) __PYX_ERR(0, 261, __pyx_L3_error)
+    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 262, __pyx_L3_error)
+    __pyx_v_V_in = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_in.memview)) __PYX_ERR(0, 262, __pyx_L3_error)
+    __pyx_v_V_out = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_out.memview)) __PYX_ERR(0, 262, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("expmH", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 261, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("expmH", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 262, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.unitary_interpolation_vector.UI_vector.expmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_10expmH(((struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self), __pyx_v_c, __pyx_v_V_in, __pyx_v_V_out);
 
@@ -6785,224 +6812,224 @@
   Py_ssize_t __pyx_t_6;
   Py_ssize_t __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expmH", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":262
+  /* "unipolator/unitary_interpolation_vector.pyx":263
  *         self.interpolate_single_u(u0, v0)
  *     def expmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out):
  *         if not c.shape[0] == self.n_dims:             # <<<<<<<<<<<<<<
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         # check V_in size
  */
   __pyx_t_1 = ((!(((__pyx_v_c.shape[0]) == __pyx_v_self->n_dims) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":263
+    /* "unipolator/unitary_interpolation_vector.pyx":264
  *     def expmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out):
  *         if not c.shape[0] == self.n_dims:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')             # <<<<<<<<<<<<<<
  *         # check V_in size
  *         if not V_in.shape[0] == self.d:
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 263, __pyx_L1_error)
+    __PYX_ERR(0, 264, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":262
+    /* "unipolator/unitary_interpolation_vector.pyx":263
  *         self.interpolate_single_u(u0, v0)
  *     def expmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out):
  *         if not c.shape[0] == self.n_dims:             # <<<<<<<<<<<<<<
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         # check V_in size
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":265
+  /* "unipolator/unitary_interpolation_vector.pyx":266
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         # check V_in size
  *         if not V_in.shape[0] == self.d:             # <<<<<<<<<<<<<<
  *             raise ValueError('V_in.shape[0] needs to be equal to H_s[0].shape[0].')
  *         if not V_in.shape[1] == self.m:
  */
   __pyx_t_1 = ((!(((__pyx_v_V_in.shape[0]) == __pyx_v_self->d) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":266
+    /* "unipolator/unitary_interpolation_vector.pyx":267
  *         # check V_in size
  *         if not V_in.shape[0] == self.d:
  *             raise ValueError('V_in.shape[0] needs to be equal to H_s[0].shape[0].')             # <<<<<<<<<<<<<<
  *         if not V_in.shape[1] == self.m:
  *             # change m
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 266, __pyx_L1_error)
+    __PYX_ERR(0, 267, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":265
+    /* "unipolator/unitary_interpolation_vector.pyx":266
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  *         # check V_in size
  *         if not V_in.shape[0] == self.d:             # <<<<<<<<<<<<<<
  *             raise ValueError('V_in.shape[0] needs to be equal to H_s[0].shape[0].')
  *         if not V_in.shape[1] == self.m:
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":267
+  /* "unipolator/unitary_interpolation_vector.pyx":268
  *         if not V_in.shape[0] == self.d:
  *             raise ValueError('V_in.shape[0] needs to be equal to H_s[0].shape[0].')
  *         if not V_in.shape[1] == self.m:             # <<<<<<<<<<<<<<
  *             # change m
  *             self.change_m(V_in.shape[1])
  */
   __pyx_t_1 = ((!(((__pyx_v_V_in.shape[1]) == __pyx_v_self->m) != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":269
+    /* "unipolator/unitary_interpolation_vector.pyx":270
  *         if not V_in.shape[1] == self.m:
  *             # change m
  *             self.change_m(V_in.shape[1])             # <<<<<<<<<<<<<<
  *         # check V_out size
  *         if not V_out.shape[0] == self.d:
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_change_m); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_change_m); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 270, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_V_in.shape[1])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_V_in.shape[1])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 270, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 270, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":267
+    /* "unipolator/unitary_interpolation_vector.pyx":268
  *         if not V_in.shape[0] == self.d:
  *             raise ValueError('V_in.shape[0] needs to be equal to H_s[0].shape[0].')
  *         if not V_in.shape[1] == self.m:             # <<<<<<<<<<<<<<
  *             # change m
  *             self.change_m(V_in.shape[1])
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":271
+  /* "unipolator/unitary_interpolation_vector.pyx":272
  *             self.change_m(V_in.shape[1])
  *         # check V_out size
  *         if not V_out.shape[0] == self.d:             # <<<<<<<<<<<<<<
  *             raise ValueError('V_out.shape[0] needs to be equal to H_s[0].shape[0].')
  *         if not V_out.shape[1] == self.m:
  */
   __pyx_t_1 = ((!(((__pyx_v_V_out.shape[0]) == __pyx_v_self->d) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":272
+    /* "unipolator/unitary_interpolation_vector.pyx":273
  *         # check V_out size
  *         if not V_out.shape[0] == self.d:
  *             raise ValueError('V_out.shape[0] needs to be equal to H_s[0].shape[0].')             # <<<<<<<<<<<<<<
  *         if not V_out.shape[1] == self.m:
  *             raise ValueError('V_out.shape[1] needs to be equal to V_in.shape[1].')
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 272, __pyx_L1_error)
+    __PYX_ERR(0, 273, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":271
+    /* "unipolator/unitary_interpolation_vector.pyx":272
  *             self.change_m(V_in.shape[1])
  *         # check V_out size
  *         if not V_out.shape[0] == self.d:             # <<<<<<<<<<<<<<
  *             raise ValueError('V_out.shape[0] needs to be equal to H_s[0].shape[0].')
  *         if not V_out.shape[1] == self.m:
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":273
+  /* "unipolator/unitary_interpolation_vector.pyx":274
  *         if not V_out.shape[0] == self.d:
  *             raise ValueError('V_out.shape[0] needs to be equal to H_s[0].shape[0].')
  *         if not V_out.shape[1] == self.m:             # <<<<<<<<<<<<<<
  *             raise ValueError('V_out.shape[1] needs to be equal to V_in.shape[1].')
  *         cdef double complex *u0 = &V_in[0, 0]
  */
   __pyx_t_1 = ((!(((__pyx_v_V_out.shape[1]) == __pyx_v_self->m) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":274
+    /* "unipolator/unitary_interpolation_vector.pyx":275
  *             raise ValueError('V_out.shape[0] needs to be equal to H_s[0].shape[0].')
  *         if not V_out.shape[1] == self.m:
  *             raise ValueError('V_out.shape[1] needs to be equal to V_in.shape[1].')             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &V_in[0, 0]
  *         cdef double complex *v0 = &V_out[0, 0]
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 274, __pyx_L1_error)
+    __PYX_ERR(0, 275, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":273
+    /* "unipolator/unitary_interpolation_vector.pyx":274
  *         if not V_out.shape[0] == self.d:
  *             raise ValueError('V_out.shape[0] needs to be equal to H_s[0].shape[0].')
  *         if not V_out.shape[1] == self.m:             # <<<<<<<<<<<<<<
  *             raise ValueError('V_out.shape[1] needs to be equal to V_in.shape[1].')
  *         cdef double complex *u0 = &V_in[0, 0]
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":275
+  /* "unipolator/unitary_interpolation_vector.pyx":276
  *         if not V_out.shape[1] == self.m:
  *             raise ValueError('V_out.shape[1] needs to be equal to V_in.shape[1].')
  *         cdef double complex *u0 = &V_in[0, 0]             # <<<<<<<<<<<<<<
  *         cdef double complex *v0 = &V_out[0, 0]
  *         self.expmH_pointer(c, u0, v0)
  */
   __pyx_t_6 = 0;
   __pyx_t_7 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_V_in.data + __pyx_t_6 * __pyx_v_V_in.strides[0]) )) + __pyx_t_7)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":276
+  /* "unipolator/unitary_interpolation_vector.pyx":277
  *             raise ValueError('V_out.shape[1] needs to be equal to V_in.shape[1].')
  *         cdef double complex *u0 = &V_in[0, 0]
  *         cdef double complex *v0 = &V_out[0, 0]             # <<<<<<<<<<<<<<
  *         self.expmH_pointer(c, u0, v0)
  * 
  */
   __pyx_t_7 = 0;
   __pyx_t_6 = 0;
   __pyx_v_v0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_V_out.data + __pyx_t_7 * __pyx_v_V_out.strides[0]) )) + __pyx_t_6)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":277
+  /* "unipolator/unitary_interpolation_vector.pyx":278
  *         cdef double complex *u0 = &V_in[0, 0]
  *         cdef double complex *v0 = &V_out[0, 0]
  *         self.expmH_pointer(c, u0, v0)             # <<<<<<<<<<<<<<
  * 
  *     cdef dexpmH_pointer(self, double[::1] c, double complex *u0, double complex *v0, double complex *du0):  #int[::1] d_di,
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":261
+  /* "unipolator/unitary_interpolation_vector.pyx":262
  *         self.single_parameters2oddgrid(c)
  *         self.interpolate_single_u(u0, v0)
  *     def expmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out):             # <<<<<<<<<<<<<<
  *         if not c.shape[0] == self.n_dims:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')
  */
 
@@ -7021,15 +7048,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_V_in, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_V_out, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":279
+/* "unipolator/unitary_interpolation_vector.pyx":280
  *         self.expmH_pointer(c, u0, v0)
  * 
  *     cdef dexpmH_pointer(self, double[::1] c, double complex *u0, double complex *v0, double complex *du0):  #int[::1] d_di,             # <<<<<<<<<<<<<<
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         self.single_parameters2oddgrid(c)
  */
 
@@ -7038,37 +7065,37 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dexpmH_pointer", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":281
+  /* "unipolator/unitary_interpolation_vector.pyx":282
  *     cdef dexpmH_pointer(self, double[::1] c, double complex *u0, double complex *v0, double complex *du0):  #int[::1] d_di,
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         self.single_parameters2oddgrid(c)             # <<<<<<<<<<<<<<
  *         self.interpolate_single_u_du(u0, v0, du0)
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_v_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_v_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":282
+  /* "unipolator/unitary_interpolation_vector.pyx":283
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         self.single_parameters2oddgrid(c)
  *         self.interpolate_single_u_du(u0, v0, du0)             # <<<<<<<<<<<<<<
  * 
  *     def dexpmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out, double complex[:,:,::1] dU):  #int[::1] d_di,
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->interpolate_single_u_du(__pyx_v_self, __pyx_v_u0, __pyx_v_v0, __pyx_v_du0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->interpolate_single_u_du(__pyx_v_self, __pyx_v_u0, __pyx_v_v0, __pyx_v_du0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":279
+  /* "unipolator/unitary_interpolation_vector.pyx":280
  *         self.expmH_pointer(c, u0, v0)
  * 
  *     cdef dexpmH_pointer(self, double[::1] c, double complex *u0, double complex *v0, double complex *du0):  #int[::1] d_di,             # <<<<<<<<<<<<<<
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         self.single_parameters2oddgrid(c)
  */
 
@@ -7081,15 +7108,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":284
+/* "unipolator/unitary_interpolation_vector.pyx":285
  *         self.interpolate_single_u_du(u0, v0, du0)
  * 
  *     def dexpmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out, double complex[:,:,::1] dU):  #int[::1] d_di,             # <<<<<<<<<<<<<<
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         cdef double complex *u0 = &V_in[0,0]
  */
 
@@ -7130,48 +7157,48 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_V_in)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("dexpmH", 1, 4, 4, 1); __PYX_ERR(0, 284, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dexpmH", 1, 4, 4, 1); __PYX_ERR(0, 285, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_V_out)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("dexpmH", 1, 4, 4, 2); __PYX_ERR(0, 284, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dexpmH", 1, 4, 4, 2); __PYX_ERR(0, 285, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dU)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("dexpmH", 1, 4, 4, 3); __PYX_ERR(0, 284, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dexpmH", 1, 4, 4, 3); __PYX_ERR(0, 285, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dexpmH") < 0)) __PYX_ERR(0, 284, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dexpmH") < 0)) __PYX_ERR(0, 285, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
-    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 284, __pyx_L3_error)
-    __pyx_v_V_in = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_in.memview)) __PYX_ERR(0, 284, __pyx_L3_error)
-    __pyx_v_V_out = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_out.memview)) __PYX_ERR(0, 284, __pyx_L3_error)
-    __pyx_v_dU = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dU.memview)) __PYX_ERR(0, 284, __pyx_L3_error)
+    __pyx_v_c = __Pyx_PyObject_to_MemoryviewSlice_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_c.memview)) __PYX_ERR(0, 285, __pyx_L3_error)
+    __pyx_v_V_in = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_in.memview)) __PYX_ERR(0, 285, __pyx_L3_error)
+    __pyx_v_V_out = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_out.memview)) __PYX_ERR(0, 285, __pyx_L3_error)
+    __pyx_v_dU = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dU.memview)) __PYX_ERR(0, 285, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dexpmH", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 284, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dexpmH", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 285, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.unitary_interpolation_vector.UI_vector.dexpmH", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_12dexpmH(((struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self), __pyx_v_c, __pyx_v_V_in, __pyx_v_V_out, __pyx_v_dU);
 
@@ -7193,320 +7220,320 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dexpmH", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":286
+  /* "unipolator/unitary_interpolation_vector.pyx":287
  *     def dexpmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out, double complex[:,:,::1] dU):  #int[::1] d_di,
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         cdef double complex *u0 = &V_in[0,0]             # <<<<<<<<<<<<<<
  *         cdef double complex *v0 = &V_out[0,0]
  *         cdef double complex *du0 = &dU[0,0,0]
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_V_in.data + __pyx_t_1 * __pyx_v_V_in.strides[0]) )) + __pyx_t_2)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":287
+  /* "unipolator/unitary_interpolation_vector.pyx":288
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         cdef double complex *u0 = &V_in[0,0]
  *         cdef double complex *v0 = &V_out[0,0]             # <<<<<<<<<<<<<<
  *         cdef double complex *du0 = &dU[0,0,0]
  *         if not c.shape[0] == self.n_dims:
  */
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
   __pyx_v_v0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_V_out.data + __pyx_t_2 * __pyx_v_V_out.strides[0]) )) + __pyx_t_1)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":288
+  /* "unipolator/unitary_interpolation_vector.pyx":289
  *         cdef double complex *u0 = &V_in[0,0]
  *         cdef double complex *v0 = &V_out[0,0]
  *         cdef double complex *du0 = &dU[0,0,0]             # <<<<<<<<<<<<<<
  *         if not c.shape[0] == self.n_dims:
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_v_du0 = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_dU.data + __pyx_t_1 * __pyx_v_dU.strides[0]) ) + __pyx_t_2 * __pyx_v_dU.strides[1]) )) + __pyx_t_3)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":289
+  /* "unipolator/unitary_interpolation_vector.pyx":290
  *         cdef double complex *v0 = &V_out[0,0]
  *         cdef double complex *du0 = &dU[0,0,0]
  *         if not c.shape[0] == self.n_dims:             # <<<<<<<<<<<<<<
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.n_d_di == dU.shape[0]:
  */
   __pyx_t_4 = ((!(((__pyx_v_c.shape[0]) == __pyx_v_self->n_dims) != 0)) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":290
+    /* "unipolator/unitary_interpolation_vector.pyx":291
  *         cdef double complex *du0 = &dU[0,0,0]
  *         if not c.shape[0] == self.n_dims:
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')             # <<<<<<<<<<<<<<
  *         if not self.n_d_di == dU.shape[0]:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 291, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 290, __pyx_L1_error)
+    __PYX_ERR(0, 291, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":289
+    /* "unipolator/unitary_interpolation_vector.pyx":290
  *         cdef double complex *v0 = &V_out[0,0]
  *         cdef double complex *du0 = &dU[0,0,0]
  *         if not c.shape[0] == self.n_dims:             # <<<<<<<<<<<<<<
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.n_d_di == dU.shape[0]:
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":291
+  /* "unipolator/unitary_interpolation_vector.pyx":292
  *         if not c.shape[0] == self.n_dims:
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.n_d_di == dU.shape[0]:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  *         if not V_in.shape[0] == self.d:
  */
   __pyx_t_4 = ((!((__pyx_v_self->n_d_di == (__pyx_v_dU.shape[0])) != 0)) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":292
+    /* "unipolator/unitary_interpolation_vector.pyx":293
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.n_d_di == dU.shape[0]:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')             # <<<<<<<<<<<<<<
  *         if not V_in.shape[0] == self.d:
  *             raise ValueError('The input vector must be of size [d].')
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 292, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 293, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 292, __pyx_L1_error)
+    __PYX_ERR(0, 293, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":291
+    /* "unipolator/unitary_interpolation_vector.pyx":292
  *         if not c.shape[0] == self.n_dims:
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.n_d_di == dU.shape[0]:             # <<<<<<<<<<<<<<
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  *         if not V_in.shape[0] == self.d:
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":293
+  /* "unipolator/unitary_interpolation_vector.pyx":294
  *         if not self.n_d_di == dU.shape[0]:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  *         if not V_in.shape[0] == self.d:             # <<<<<<<<<<<<<<
  *             raise ValueError('The input vector must be of size [d].')
  *         if not V_out.shape[0] == self.d:
  */
   __pyx_t_4 = ((!(((__pyx_v_V_in.shape[0]) == __pyx_v_self->d) != 0)) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":294
+    /* "unipolator/unitary_interpolation_vector.pyx":295
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  *         if not V_in.shape[0] == self.d:
  *             raise ValueError('The input vector must be of size [d].')             # <<<<<<<<<<<<<<
  *         if not V_out.shape[0] == self.d:
  *             raise ValueError('The output vector must be of size [d].')
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 294, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 295, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 294, __pyx_L1_error)
+    __PYX_ERR(0, 295, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":293
+    /* "unipolator/unitary_interpolation_vector.pyx":294
  *         if not self.n_d_di == dU.shape[0]:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  *         if not V_in.shape[0] == self.d:             # <<<<<<<<<<<<<<
  *             raise ValueError('The input vector must be of size [d].')
  *         if not V_out.shape[0] == self.d:
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":295
+  /* "unipolator/unitary_interpolation_vector.pyx":296
  *         if not V_in.shape[0] == self.d:
  *             raise ValueError('The input vector must be of size [d].')
  *         if not V_out.shape[0] == self.d:             # <<<<<<<<<<<<<<
  *             raise ValueError('The output vector must be of size [d].')
  *         if not V_in.shape[1] == V_out.shape[1] == self.m:
  */
   __pyx_t_4 = ((!(((__pyx_v_V_out.shape[0]) == __pyx_v_self->d) != 0)) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":296
+    /* "unipolator/unitary_interpolation_vector.pyx":297
  *             raise ValueError('The input vector must be of size [d].')
  *         if not V_out.shape[0] == self.d:
  *             raise ValueError('The output vector must be of size [d].')             # <<<<<<<<<<<<<<
  *         if not V_in.shape[1] == V_out.shape[1] == self.m:
  *             raise ValueError('The input and output vectors must have the same number of columns, and equal to m.')
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 296, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 297, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 296, __pyx_L1_error)
+    __PYX_ERR(0, 297, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":295
+    /* "unipolator/unitary_interpolation_vector.pyx":296
  *         if not V_in.shape[0] == self.d:
  *             raise ValueError('The input vector must be of size [d].')
  *         if not V_out.shape[0] == self.d:             # <<<<<<<<<<<<<<
  *             raise ValueError('The output vector must be of size [d].')
  *         if not V_in.shape[1] == V_out.shape[1] == self.m:
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":297
+  /* "unipolator/unitary_interpolation_vector.pyx":298
  *         if not V_out.shape[0] == self.d:
  *             raise ValueError('The output vector must be of size [d].')
  *         if not V_in.shape[1] == V_out.shape[1] == self.m:             # <<<<<<<<<<<<<<
  *             raise ValueError('The input and output vectors must have the same number of columns, and equal to m.')
  *         if not dU.shape[1] == self.d:
  */
   __pyx_t_4 = ((__pyx_v_V_in.shape[1]) == (__pyx_v_V_out.shape[1]));
   if (__pyx_t_4) {
     __pyx_t_4 = ((__pyx_v_V_out.shape[1]) == __pyx_v_self->m);
   }
   __pyx_t_6 = ((!(__pyx_t_4 != 0)) != 0);
   if (unlikely(__pyx_t_6)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":298
+    /* "unipolator/unitary_interpolation_vector.pyx":299
  *             raise ValueError('The output vector must be of size [d].')
  *         if not V_in.shape[1] == V_out.shape[1] == self.m:
  *             raise ValueError('The input and output vectors must have the same number of columns, and equal to m.')             # <<<<<<<<<<<<<<
  *         if not dU.shape[1] == self.d:
  *             raise ValueError('The input derivative vector must be of size [d].')
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 298, __pyx_L1_error)
+    __PYX_ERR(0, 299, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":297
+    /* "unipolator/unitary_interpolation_vector.pyx":298
  *         if not V_out.shape[0] == self.d:
  *             raise ValueError('The output vector must be of size [d].')
  *         if not V_in.shape[1] == V_out.shape[1] == self.m:             # <<<<<<<<<<<<<<
  *             raise ValueError('The input and output vectors must have the same number of columns, and equal to m.')
  *         if not dU.shape[1] == self.d:
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":299
+  /* "unipolator/unitary_interpolation_vector.pyx":300
  *         if not V_in.shape[1] == V_out.shape[1] == self.m:
  *             raise ValueError('The input and output vectors must have the same number of columns, and equal to m.')
  *         if not dU.shape[1] == self.d:             # <<<<<<<<<<<<<<
  *             raise ValueError('The input derivative vector must be of size [d].')
  *         if not dU.shape[2] == self.m:
  */
   __pyx_t_6 = ((!(((__pyx_v_dU.shape[1]) == __pyx_v_self->d) != 0)) != 0);
   if (unlikely(__pyx_t_6)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":300
+    /* "unipolator/unitary_interpolation_vector.pyx":301
  *             raise ValueError('The input and output vectors must have the same number of columns, and equal to m.')
  *         if not dU.shape[1] == self.d:
  *             raise ValueError('The input derivative vector must be of size [d].')             # <<<<<<<<<<<<<<
  *         if not dU.shape[2] == self.m:
  *             raise ValueError('The input derivative vector must have the same number of columns as the input and output vectors, and equal to m.')
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 301, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 300, __pyx_L1_error)
+    __PYX_ERR(0, 301, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":299
+    /* "unipolator/unitary_interpolation_vector.pyx":300
  *         if not V_in.shape[1] == V_out.shape[1] == self.m:
  *             raise ValueError('The input and output vectors must have the same number of columns, and equal to m.')
  *         if not dU.shape[1] == self.d:             # <<<<<<<<<<<<<<
  *             raise ValueError('The input derivative vector must be of size [d].')
  *         if not dU.shape[2] == self.m:
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":301
+  /* "unipolator/unitary_interpolation_vector.pyx":302
  *         if not dU.shape[1] == self.d:
  *             raise ValueError('The input derivative vector must be of size [d].')
  *         if not dU.shape[2] == self.m:             # <<<<<<<<<<<<<<
  *             raise ValueError('The input derivative vector must have the same number of columns as the input and output vectors, and equal to m.')
  *         if not self.n_d_di == dU.shape[0]:
  */
   __pyx_t_6 = ((!(((__pyx_v_dU.shape[2]) == __pyx_v_self->m) != 0)) != 0);
   if (unlikely(__pyx_t_6)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":302
+    /* "unipolator/unitary_interpolation_vector.pyx":303
  *             raise ValueError('The input derivative vector must be of size [d].')
  *         if not dU.shape[2] == self.m:
  *             raise ValueError('The input derivative vector must have the same number of columns as the input and output vectors, and equal to m.')             # <<<<<<<<<<<<<<
  *         if not self.n_d_di == dU.shape[0]:
  *             raise ValueError('The input derivative vector must have the same number of rows as the number of derivatives to calculate.')
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 302, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 302, __pyx_L1_error)
+    __PYX_ERR(0, 303, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":301
+    /* "unipolator/unitary_interpolation_vector.pyx":302
  *         if not dU.shape[1] == self.d:
  *             raise ValueError('The input derivative vector must be of size [d].')
  *         if not dU.shape[2] == self.m:             # <<<<<<<<<<<<<<
  *             raise ValueError('The input derivative vector must have the same number of columns as the input and output vectors, and equal to m.')
  *         if not self.n_d_di == dU.shape[0]:
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":303
+  /* "unipolator/unitary_interpolation_vector.pyx":304
  *         if not dU.shape[2] == self.m:
  *             raise ValueError('The input derivative vector must have the same number of columns as the input and output vectors, and equal to m.')
  *         if not self.n_d_di == dU.shape[0]:             # <<<<<<<<<<<<<<
  *             raise ValueError('The input derivative vector must have the same number of rows as the number of derivatives to calculate.')
  *         self.dexpmH_pointer(c, u0, v0, du0)
  */
   __pyx_t_6 = ((!((__pyx_v_self->n_d_di == (__pyx_v_dU.shape[0])) != 0)) != 0);
   if (unlikely(__pyx_t_6)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":304
+    /* "unipolator/unitary_interpolation_vector.pyx":305
  *             raise ValueError('The input derivative vector must have the same number of columns as the input and output vectors, and equal to m.')
  *         if not self.n_d_di == dU.shape[0]:
  *             raise ValueError('The input derivative vector must have the same number of rows as the number of derivatives to calculate.')             # <<<<<<<<<<<<<<
  *         self.dexpmH_pointer(c, u0, v0, du0)
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 304, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 305, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 304, __pyx_L1_error)
+    __PYX_ERR(0, 305, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":303
+    /* "unipolator/unitary_interpolation_vector.pyx":304
  *         if not dU.shape[2] == self.m:
  *             raise ValueError('The input derivative vector must have the same number of columns as the input and output vectors, and equal to m.')
  *         if not self.n_d_di == dU.shape[0]:             # <<<<<<<<<<<<<<
  *             raise ValueError('The input derivative vector must have the same number of rows as the number of derivatives to calculate.')
  *         self.dexpmH_pointer(c, u0, v0, du0)
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":305
+  /* "unipolator/unitary_interpolation_vector.pyx":306
  *         if not self.n_d_di == dU.shape[0]:
  *             raise ValueError('The input derivative vector must have the same number of rows as the number of derivatives to calculate.')
  *         self.dexpmH_pointer(c, u0, v0, du0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0, __pyx_v_v0, __pyx_v_du0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 305, __pyx_L1_error)
+  __pyx_t_5 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->dexpmH_pointer(__pyx_v_self, __pyx_v_c, __pyx_v_u0, __pyx_v_v0, __pyx_v_du0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":284
+  /* "unipolator/unitary_interpolation_vector.pyx":285
  *         self.interpolate_single_u_du(u0, v0, du0)
  * 
  *     def dexpmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out, double complex[:,:,::1] dU):  #int[::1] d_di,             # <<<<<<<<<<<<<<
  *         # d_di contains the indexes of the derivatives that we want to calculate (needs to be in ascending order with a negative value at the end)
  *         cdef double complex *u0 = &V_in[0,0]
  */
 
@@ -7523,15 +7550,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_V_out, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_dU, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":308
+/* "unipolator/unitary_interpolation_vector.pyx":309
  * 
  * 
  *     cdef expmH_pulse_pointer(self, double[:,::1] cs, double complex *u0, double complex *v0):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i = 0
  *         cdef int steps = cs.shape[0]
  */
 
@@ -7549,95 +7576,95 @@
   Py_ssize_t __pyx_t_5;
   __Pyx_memviewslice __pyx_t_6 = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expmH_pulse_pointer", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":309
+  /* "unipolator/unitary_interpolation_vector.pyx":310
  * 
  *     cdef expmH_pulse_pointer(self, double[:,::1] cs, double complex *u0, double complex *v0):
  *         cdef Py_ssize_t i = 0             # <<<<<<<<<<<<<<
  *         cdef int steps = cs.shape[0]
  *         cdef int steps_2 = steps >> 1  # floor (steps/2)
  */
   __pyx_v_i = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":310
+  /* "unipolator/unitary_interpolation_vector.pyx":311
  *     cdef expmH_pulse_pointer(self, double[:,::1] cs, double complex *u0, double complex *v0):
  *         cdef Py_ssize_t i = 0
  *         cdef int steps = cs.shape[0]             # <<<<<<<<<<<<<<
  *         cdef int steps_2 = steps >> 1  # floor (steps/2)
  *         cdef int is_odd_steps = steps % 2
  */
   __pyx_v_steps = (__pyx_v_cs.shape[0]);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":311
+  /* "unipolator/unitary_interpolation_vector.pyx":312
  *         cdef Py_ssize_t i = 0
  *         cdef int steps = cs.shape[0]
  *         cdef int steps_2 = steps >> 1  # floor (steps/2)             # <<<<<<<<<<<<<<
  *         cdef int is_odd_steps = steps % 2
  *         if not cs.shape[1] == self.n_dims:
  */
   __pyx_v_steps_2 = (__pyx_v_steps >> 1);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":312
+  /* "unipolator/unitary_interpolation_vector.pyx":313
  *         cdef int steps = cs.shape[0]
  *         cdef int steps_2 = steps >> 1  # floor (steps/2)
  *         cdef int is_odd_steps = steps % 2             # <<<<<<<<<<<<<<
  *         if not cs.shape[1] == self.n_dims:
  *             raise ValueError('The coefficient matrix must be of size [n_time_steps, interpolation_dimensions].')
  */
   __pyx_v_is_odd_steps = (__pyx_v_steps % 2);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":313
+  /* "unipolator/unitary_interpolation_vector.pyx":314
  *         cdef int steps_2 = steps >> 1  # floor (steps/2)
  *         cdef int is_odd_steps = steps % 2
  *         if not cs.shape[1] == self.n_dims:             # <<<<<<<<<<<<<<
  *             raise ValueError('The coefficient matrix must be of size [n_time_steps, interpolation_dimensions].')
  *         for i in range(0, steps_2, 2):
  */
   __pyx_t_1 = ((!(((__pyx_v_cs.shape[1]) == __pyx_v_self->n_dims) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":314
+    /* "unipolator/unitary_interpolation_vector.pyx":315
  *         cdef int is_odd_steps = steps % 2
  *         if not cs.shape[1] == self.n_dims:
  *             raise ValueError('The coefficient matrix must be of size [n_time_steps, interpolation_dimensions].')             # <<<<<<<<<<<<<<
  *         for i in range(0, steps_2, 2):
  *             self.single_parameters2oddgrid(cs[i,:])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 315, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 314, __pyx_L1_error)
+    __PYX_ERR(0, 315, __pyx_L1_error)
 
-    /* "unipolator/unitary_interpolation_vector.pyx":313
+    /* "unipolator/unitary_interpolation_vector.pyx":314
  *         cdef int steps_2 = steps >> 1  # floor (steps/2)
  *         cdef int is_odd_steps = steps % 2
  *         if not cs.shape[1] == self.n_dims:             # <<<<<<<<<<<<<<
  *             raise ValueError('The coefficient matrix must be of size [n_time_steps, interpolation_dimensions].')
  *         for i in range(0, steps_2, 2):
  */
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":315
+  /* "unipolator/unitary_interpolation_vector.pyx":316
  *         if not cs.shape[1] == self.n_dims:
  *             raise ValueError('The coefficient matrix must be of size [n_time_steps, interpolation_dimensions].')
  *         for i in range(0, steps_2, 2):             # <<<<<<<<<<<<<<
  *             self.single_parameters2oddgrid(cs[i,:])
  *             self.interpolate_single_u(u0, v0)
  */
   __pyx_t_3 = __pyx_v_steps_2;
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=2) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":316
+    /* "unipolator/unitary_interpolation_vector.pyx":317
  *             raise ValueError('The coefficient matrix must be of size [n_time_steps, interpolation_dimensions].')
  *         for i in range(0, steps_2, 2):
  *             self.single_parameters2oddgrid(cs[i,:])             # <<<<<<<<<<<<<<
  *             self.interpolate_single_u(u0, v0)
  *             self.single_parameters2oddgrid(cs[i+1,:])
  */
     __pyx_t_6.data = __pyx_v_cs.data;
@@ -7649,33 +7676,33 @@
         __pyx_t_6.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
 __pyx_t_6.shape[0] = __pyx_v_cs.shape[1];
 __pyx_t_6.strides[0] = __pyx_v_cs.strides[1];
     __pyx_t_6.suboffsets[0] = -1;
 
-__pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 316, __pyx_L1_error)
+__pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 317, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __PYX_XDEC_MEMVIEW(&__pyx_t_6, 1);
     __pyx_t_6.memview = NULL;
     __pyx_t_6.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":317
+    /* "unipolator/unitary_interpolation_vector.pyx":318
  *         for i in range(0, steps_2, 2):
  *             self.single_parameters2oddgrid(cs[i,:])
  *             self.interpolate_single_u(u0, v0)             # <<<<<<<<<<<<<<
  *             self.single_parameters2oddgrid(cs[i+1,:])
  *             self.interpolate_single_u(v0, u0)
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->interpolate_single_u(__pyx_v_self, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 317, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->interpolate_single_u(__pyx_v_self, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":318
+    /* "unipolator/unitary_interpolation_vector.pyx":319
  *             self.single_parameters2oddgrid(cs[i,:])
  *             self.interpolate_single_u(u0, v0)
  *             self.single_parameters2oddgrid(cs[i+1,:])             # <<<<<<<<<<<<<<
  *             self.interpolate_single_u(v0, u0)
  *         if is_odd_steps:
  */
     __pyx_t_6.data = __pyx_v_cs.data;
@@ -7687,44 +7714,44 @@
         __pyx_t_6.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
 __pyx_t_6.shape[0] = __pyx_v_cs.shape[1];
 __pyx_t_6.strides[0] = __pyx_v_cs.strides[1];
     __pyx_t_6.suboffsets[0] = -1;
 
-__pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 318, __pyx_L1_error)
+__pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __PYX_XDEC_MEMVIEW(&__pyx_t_6, 1);
     __pyx_t_6.memview = NULL;
     __pyx_t_6.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":319
+    /* "unipolator/unitary_interpolation_vector.pyx":320
  *             self.interpolate_single_u(u0, v0)
  *             self.single_parameters2oddgrid(cs[i+1,:])
  *             self.interpolate_single_u(v0, u0)             # <<<<<<<<<<<<<<
  *         if is_odd_steps:
  *             self.single_parameters2oddgrid(cs[steps_2,:])
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->interpolate_single_u(__pyx_v_self, __pyx_v_v0, __pyx_v_u0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->interpolate_single_u(__pyx_v_self, __pyx_v_v0, __pyx_v_u0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":320
+  /* "unipolator/unitary_interpolation_vector.pyx":321
  *             self.single_parameters2oddgrid(cs[i+1,:])
  *             self.interpolate_single_u(v0, u0)
  *         if is_odd_steps:             # <<<<<<<<<<<<<<
  *             self.single_parameters2oddgrid(cs[steps_2,:])
  *             self.interpolate_single_u(u0, v0)
  */
   __pyx_t_1 = (__pyx_v_is_odd_steps != 0);
   if (__pyx_t_1) {
 
-    /* "unipolator/unitary_interpolation_vector.pyx":321
+    /* "unipolator/unitary_interpolation_vector.pyx":322
  *             self.interpolate_single_u(v0, u0)
  *         if is_odd_steps:
  *             self.single_parameters2oddgrid(cs[steps_2,:])             # <<<<<<<<<<<<<<
  *             self.interpolate_single_u(u0, v0)
  *         else:  # copy to v0
  */
     __pyx_t_6.data = __pyx_v_cs.data;
@@ -7736,55 +7763,55 @@
         __pyx_t_6.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
 __pyx_t_6.shape[0] = __pyx_v_cs.shape[1];
 __pyx_t_6.strides[0] = __pyx_v_cs.strides[1];
     __pyx_t_6.suboffsets[0] = -1;
 
-__pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 321, __pyx_L1_error)
+__pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->single_parameters2oddgrid(__pyx_v_self, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 322, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __PYX_XDEC_MEMVIEW(&__pyx_t_6, 1);
     __pyx_t_6.memview = NULL;
     __pyx_t_6.data = NULL;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":322
+    /* "unipolator/unitary_interpolation_vector.pyx":323
  *         if is_odd_steps:
  *             self.single_parameters2oddgrid(cs[steps_2,:])
  *             self.interpolate_single_u(u0, v0)             # <<<<<<<<<<<<<<
  *         else:  # copy to v0
  *             copy_pointer(u0, v0, self.dm)
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->interpolate_single_u(__pyx_v_self, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 322, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->interpolate_single_u(__pyx_v_self, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":320
+    /* "unipolator/unitary_interpolation_vector.pyx":321
  *             self.single_parameters2oddgrid(cs[i+1,:])
  *             self.interpolate_single_u(v0, u0)
  *         if is_odd_steps:             # <<<<<<<<<<<<<<
  *             self.single_parameters2oddgrid(cs[steps_2,:])
  *             self.interpolate_single_u(u0, v0)
  */
     goto __pyx_L6;
   }
 
-  /* "unipolator/unitary_interpolation_vector.pyx":324
+  /* "unipolator/unitary_interpolation_vector.pyx":325
  *             self.interpolate_single_u(u0, v0)
  *         else:  # copy to v0
  *             copy_pointer(u0, v0, self.dm)             # <<<<<<<<<<<<<<
  * 
  *     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] V_in, double complex[:,::1] V_out):
  */
   /*else*/ {
     __pyx_f_10unipolator_11exp_and_log_copy_pointer(__pyx_v_u0, __pyx_v_v0, __pyx_v_self->dm);
   }
   __pyx_L6:;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":308
+  /* "unipolator/unitary_interpolation_vector.pyx":309
  * 
  * 
  *     cdef expmH_pulse_pointer(self, double[:,::1] cs, double complex *u0, double complex *v0):             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t i = 0
  *         cdef int steps = cs.shape[0]
  */
 
@@ -7798,15 +7825,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":326
+/* "unipolator/unitary_interpolation_vector.pyx":327
  *             copy_pointer(u0, v0, self.dm)
  * 
  *     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] V_in, double complex[:,::1] V_out):             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &V_in[0, 0]
  *         cdef double complex *v0 = &V_out[0, 0]
  */
 
@@ -7844,40 +7871,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cs)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_V_in)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("expmH_pulse", 1, 3, 3, 1); __PYX_ERR(0, 326, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("expmH_pulse", 1, 3, 3, 1); __PYX_ERR(0, 327, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_V_out)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("expmH_pulse", 1, 3, 3, 2); __PYX_ERR(0, 326, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("expmH_pulse", 1, 3, 3, 2); __PYX_ERR(0, 327, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH_pulse") < 0)) __PYX_ERR(0, 326, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH_pulse") < 0)) __PYX_ERR(0, 327, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 326, __pyx_L3_error)
-    __pyx_v_V_in = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_in.memview)) __PYX_ERR(0, 326, __pyx_L3_error)
-    __pyx_v_V_out = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_out.memview)) __PYX_ERR(0, 326, __pyx_L3_error)
+    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 327, __pyx_L3_error)
+    __pyx_v_V_in = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_in.memview)) __PYX_ERR(0, 327, __pyx_L3_error)
+    __pyx_v_V_out = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_out.memview)) __PYX_ERR(0, 327, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("expmH_pulse", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 326, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("expmH_pulse", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 327, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.unitary_interpolation_vector.UI_vector.expmH_pulse", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_14expmH_pulse(((struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self), __pyx_v_cs, __pyx_v_V_in, __pyx_v_V_out);
 
@@ -7895,48 +7922,48 @@
   Py_ssize_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expmH_pulse", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":327
+  /* "unipolator/unitary_interpolation_vector.pyx":328
  * 
  *     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] V_in, double complex[:,::1] V_out):
  *         cdef double complex *u0 = &V_in[0, 0]             # <<<<<<<<<<<<<<
  *         cdef double complex *v0 = &V_out[0, 0]
  *         self.expmH_pulse_pointer(cs, u0, v0)
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_V_in.data + __pyx_t_1 * __pyx_v_V_in.strides[0]) )) + __pyx_t_2)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":328
+  /* "unipolator/unitary_interpolation_vector.pyx":329
  *     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] V_in, double complex[:,::1] V_out):
  *         cdef double complex *u0 = &V_in[0, 0]
  *         cdef double complex *v0 = &V_out[0, 0]             # <<<<<<<<<<<<<<
  *         self.expmH_pulse_pointer(cs, u0, v0)
  * 
  */
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
   __pyx_v_v0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_V_out.data + __pyx_t_2 * __pyx_v_V_out.strides[0]) )) + __pyx_t_1)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":329
+  /* "unipolator/unitary_interpolation_vector.pyx":330
  *         cdef double complex *u0 = &V_in[0, 0]
  *         cdef double complex *v0 = &V_out[0, 0]
  *         self.expmH_pulse_pointer(cs, u0, v0)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->expmH_pulse_pointer(__pyx_v_self, __pyx_v_cs, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_3 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->expmH_pulse_pointer(__pyx_v_self, __pyx_v_cs, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":326
+  /* "unipolator/unitary_interpolation_vector.pyx":327
  *             copy_pointer(u0, v0, self.dm)
  * 
  *     def expmH_pulse(self, double[:,::1] cs, double complex[:,::1] V_in, double complex[:,::1] V_out):             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &V_in[0, 0]
  *         cdef double complex *v0 = &V_out[0, 0]
  */
 
@@ -7952,15 +7979,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_V_in, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_V_out, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "unipolator/unitary_interpolation_vector.pyx":332
+/* "unipolator/unitary_interpolation_vector.pyx":333
  * 
  * 
  *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,::1] V_in, double complex[:,:,::1] V_out):             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &V_in[0,0]
  *         cdef double complex *v0 = &V_out[0,0,0]
  */
 
@@ -7998,40 +8025,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cs)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_V_in)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 3, 3, 1); __PYX_ERR(0, 332, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 3, 3, 1); __PYX_ERR(0, 333, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_V_out)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 3, 3, 2); __PYX_ERR(0, 332, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 3, 3, 2); __PYX_ERR(0, 333, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH_pulse_no_multiply") < 0)) __PYX_ERR(0, 332, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "expmH_pulse_no_multiply") < 0)) __PYX_ERR(0, 333, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 332, __pyx_L3_error)
-    __pyx_v_V_in = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_in.memview)) __PYX_ERR(0, 332, __pyx_L3_error)
-    __pyx_v_V_out = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_out.memview)) __PYX_ERR(0, 332, __pyx_L3_error)
+    __pyx_v_cs = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_cs.memview)) __PYX_ERR(0, 333, __pyx_L3_error)
+    __pyx_v_V_in = __Pyx_PyObject_to_MemoryviewSlice_d_dc___pyx_t_double_complex(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_in.memview)) __PYX_ERR(0, 333, __pyx_L3_error)
+    __pyx_v_V_out = __Pyx_PyObject_to_MemoryviewSlice_d_d_dc___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_V_out.memview)) __PYX_ERR(0, 333, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 332, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("expmH_pulse_no_multiply", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 333, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("unipolator.unitary_interpolation_vector.UI_vector.expmH_pulse_no_multiply", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10unipolator_28unitary_interpolation_vector_9UI_vector_16expmH_pulse_no_multiply(((struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self), __pyx_v_cs, __pyx_v_V_in, __pyx_v_V_out);
 
@@ -8057,149 +8084,149 @@
   Py_ssize_t __pyx_t_8;
   __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expmH_pulse_no_multiply", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":333
+  /* "unipolator/unitary_interpolation_vector.pyx":334
  * 
  *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,::1] V_in, double complex[:,:,::1] V_out):
  *         cdef double complex *u0 = &V_in[0,0]             # <<<<<<<<<<<<<<
  *         cdef double complex *v0 = &V_out[0,0,0]
  *         cdef n = cs.shape[0]
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_v_u0 = (&(*((__pyx_t_double_complex *) ( /* dim=1 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_V_in.data + __pyx_t_1 * __pyx_v_V_in.strides[0]) )) + __pyx_t_2)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":334
+  /* "unipolator/unitary_interpolation_vector.pyx":335
  *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,::1] V_in, double complex[:,:,::1] V_out):
  *         cdef double complex *u0 = &V_in[0,0]
  *         cdef double complex *v0 = &V_out[0,0,0]             # <<<<<<<<<<<<<<
  *         cdef n = cs.shape[0]
  *         for i in range(n):
  */
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_v_v0 = (&(*((__pyx_t_double_complex *) ( /* dim=2 */ ((char *) (((__pyx_t_double_complex *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_V_out.data + __pyx_t_2 * __pyx_v_V_out.strides[0]) ) + __pyx_t_1 * __pyx_v_V_out.strides[1]) )) + __pyx_t_3)) ))));
 
-  /* "unipolator/unitary_interpolation_vector.pyx":335
+  /* "unipolator/unitary_interpolation_vector.pyx":336
  *         cdef double complex *u0 = &V_in[0,0]
  *         cdef double complex *v0 = &V_out[0,0,0]
  *         cdef n = cs.shape[0]             # <<<<<<<<<<<<<<
  *         for i in range(n):
  *             self.expmH_pointer(cs[i,:], u0, v0)
  */
-  __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_cs.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_v_cs.shape[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_v_n = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":336
+  /* "unipolator/unitary_interpolation_vector.pyx":337
  *         cdef double complex *v0 = &V_out[0,0,0]
  *         cdef n = cs.shape[0]
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             self.expmH_pointer(cs[i,:], u0, v0)
  *             v0 += self.dm
  */
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
     __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 337, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 337, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_5))) {
         if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 337, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 337, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 337, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 337, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_7(__pyx_t_5);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 336, __pyx_L1_error)
+          else __PYX_ERR(0, 337, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":337
+    /* "unipolator/unitary_interpolation_vector.pyx":338
  *         cdef n = cs.shape[0]
  *         for i in range(n):
  *             self.expmH_pointer(cs[i,:], u0, v0)             # <<<<<<<<<<<<<<
  *             v0 += self.dm
  *     """
  */
-    __pyx_t_8 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_8 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 337, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_8 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 338, __pyx_L1_error)
     __pyx_t_9.data = __pyx_v_cs.data;
     __pyx_t_9.memview = __pyx_v_cs.memview;
     __PYX_INC_MEMVIEW(&__pyx_t_9, 0);
     {
     Py_ssize_t __pyx_tmp_idx = __pyx_t_8;
     Py_ssize_t __pyx_tmp_stride = __pyx_v_cs.strides[0];
         __pyx_t_9.data += __pyx_tmp_idx * __pyx_tmp_stride;
 }
 
 __pyx_t_9.shape[0] = __pyx_v_cs.shape[1];
 __pyx_t_9.strides[0] = __pyx_v_cs.strides[1];
     __pyx_t_9.suboffsets[0] = -1;
 
-__pyx_t_4 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_t_9, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 337, __pyx_L1_error)
+__pyx_t_4 = ((struct __pyx_vtabstruct_10unipolator_28unitary_interpolation_vector_UI_vector *)__pyx_v_self->__pyx_vtab)->expmH_pointer(__pyx_v_self, __pyx_t_9, __pyx_v_u0, __pyx_v_v0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
     __pyx_t_9.memview = NULL;
     __pyx_t_9.data = NULL;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "unipolator/unitary_interpolation_vector.pyx":338
+    /* "unipolator/unitary_interpolation_vector.pyx":339
  *         for i in range(n):
  *             self.expmH_pointer(cs[i,:], u0, v0)
  *             v0 += self.dm             # <<<<<<<<<<<<<<
  *     """
  *     def grape(self, double[:,::1] cs, double complex[:,::1] U_target, int[::1] target_indexes, double complex[:,::1] U, double complex[:,:,::1] dU, double[:,::1] dI_dj):
  */
     __pyx_v_v0 = (__pyx_v_v0 + __pyx_v_self->dm);
 
-    /* "unipolator/unitary_interpolation_vector.pyx":336
+    /* "unipolator/unitary_interpolation_vector.pyx":337
  *         cdef double complex *v0 = &V_out[0,0,0]
  *         cdef n = cs.shape[0]
  *         for i in range(n):             # <<<<<<<<<<<<<<
  *             self.expmH_pointer(cs[i,:], u0, v0)
  *             v0 += self.dm
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":332
+  /* "unipolator/unitary_interpolation_vector.pyx":333
  * 
  * 
  *     def expmH_pulse_no_multiply(self, double[:,::1] cs, double complex[:,::1] V_in, double complex[:,:,::1] V_out):             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &V_in[0,0]
  *         cdef double complex *v0 = &V_out[0,0,0]
  */
 
@@ -8334,14 +8361,236 @@
   __Pyx_AddTraceback("unipolator.unitary_interpolation_vector.UI_vector.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "unipolator/unitary_interpolation_vector.pyx":406
+ * 
+ * 
+ * def UI_vector_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long), m = 1):             # <<<<<<<<<<<<<<
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ *     return UI_vector(H_s, c_min_s, c_max_s, opt_bins, which_diffs, m = 1)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10unipolator_28unitary_interpolation_vector_1UI_vector_auto(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10unipolator_28unitary_interpolation_vector_UI_vector_auto[] = "UI_vector_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs=np.array([], dtype=np.compat.long), m=1)";
+static PyMethodDef __pyx_mdef_10unipolator_28unitary_interpolation_vector_1UI_vector_auto = {"UI_vector_auto", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10unipolator_28unitary_interpolation_vector_1UI_vector_auto, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10unipolator_28unitary_interpolation_vector_UI_vector_auto};
+static PyObject *__pyx_pw_10unipolator_28unitary_interpolation_vector_1UI_vector_auto(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_H_s = 0;
+  PyObject *__pyx_v_c_min_s = 0;
+  PyObject *__pyx_v_c_max_s = 0;
+  PyObject *__pyx_v_I_tar = 0;
+  PyObject *__pyx_v_which_diffs = 0;
+  CYTHON_UNUSED PyObject *__pyx_v_m = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("UI_vector_auto (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_H_s,&__pyx_n_s_c_min_s,&__pyx_n_s_c_max_s,&__pyx_n_s_I_tar,&__pyx_n_s_which_diffs,&__pyx_n_s_m,0};
+    PyObject* values[6] = {0,0,0,0,0,0};
+    values[3] = ((PyObject *)__pyx_float_1eneg_10);
+    values[4] = __pyx_k__19;
+    values[5] = ((PyObject *)__pyx_int_1);
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_H_s)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_min_s)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("UI_vector_auto", 0, 3, 6, 1); __PYX_ERR(0, 406, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_c_max_s)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("UI_vector_auto", 0, 3, 6, 2); __PYX_ERR(0, 406, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_I_tar);
+          if (value) { values[3] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_which_diffs);
+          if (value) { values[4] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_m);
+          if (value) { values[5] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "UI_vector_auto") < 0)) __PYX_ERR(0, 406, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_H_s = values[0];
+    __pyx_v_c_min_s = values[1];
+    __pyx_v_c_max_s = values[2];
+    __pyx_v_I_tar = values[3];
+    __pyx_v_which_diffs = values[4];
+    __pyx_v_m = values[5];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("UI_vector_auto", 0, 3, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 406, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("unipolator.unitary_interpolation_vector.UI_vector_auto", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_10unipolator_28unitary_interpolation_vector_UI_vector_auto(__pyx_self, __pyx_v_H_s, __pyx_v_c_min_s, __pyx_v_c_max_s, __pyx_v_I_tar, __pyx_v_which_diffs, __pyx_v_m);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10unipolator_28unitary_interpolation_vector_UI_vector_auto(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_H_s, PyObject *__pyx_v_c_min_s, PyObject *__pyx_v_c_max_s, PyObject *__pyx_v_I_tar, PyObject *__pyx_v_which_diffs, CYTHON_UNUSED PyObject *__pyx_v_m) {
+  PyObject *__pyx_v_opt_bins = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("UI_vector_auto", 0);
+
+  /* "unipolator/unitary_interpolation_vector.pyx":407
+ * 
+ * def UI_vector_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long), m = 1):
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)             # <<<<<<<<<<<<<<
+ *     return UI_vector(H_s, c_min_s, c_max_s, opt_bins, which_diffs, m = 1)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_optimal_binning); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_v_H_s);
+  __Pyx_GIVEREF(__pyx_v_H_s);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_H_s);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_c_mins, __pyx_v_c_min_s) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_c_maxs, __pyx_v_c_max_s) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_I_tar, __pyx_v_I_tar) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_opt_bins = __pyx_t_4;
+  __pyx_t_4 = 0;
+
+  /* "unipolator/unitary_interpolation_vector.pyx":408
+ * def UI_vector_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long), m = 1):
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ *     return UI_vector(H_s, c_min_s, c_max_s, opt_bins, which_diffs, m = 1)             # <<<<<<<<<<<<<<
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_INCREF(__pyx_v_H_s);
+  __Pyx_GIVEREF(__pyx_v_H_s);
+  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_H_s);
+  __Pyx_INCREF(__pyx_v_c_min_s);
+  __Pyx_GIVEREF(__pyx_v_c_min_s);
+  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_c_min_s);
+  __Pyx_INCREF(__pyx_v_c_max_s);
+  __Pyx_GIVEREF(__pyx_v_c_max_s);
+  PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_v_c_max_s);
+  __Pyx_INCREF(__pyx_v_opt_bins);
+  __Pyx_GIVEREF(__pyx_v_opt_bins);
+  PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_v_opt_bins);
+  __Pyx_INCREF(__pyx_v_which_diffs);
+  __Pyx_GIVEREF(__pyx_v_which_diffs);
+  PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_v_which_diffs);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_m, __pyx_int_1) < 0) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10unipolator_28unitary_interpolation_vector_UI_vector), __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "unipolator/unitary_interpolation_vector.pyx":406
+ * 
+ * 
+ * def UI_vector_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long), m = 1):             # <<<<<<<<<<<<<<
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ *     return UI_vector(H_s, c_min_s, c_max_s, opt_bins, which_diffs, m = 1)
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("unipolator.unitary_interpolation_vector.UI_vector_auto", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_opt_bins);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
@@ -8866,15 +9115,15 @@
       /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -8998,15 +9247,15 @@
       /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -9130,15 +9379,15 @@
       /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -9554,15 +9803,15 @@
     /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 134, __pyx_L1_error)
 
     /* "View.MemoryView":133
  *         self.itemsize = itemsize
@@ -9586,15 +9835,15 @@
     /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 137, __pyx_L1_error)
 
     /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -9713,15 +9962,15 @@
     /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 149, __pyx_L1_error)
 
     /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
@@ -9987,15 +10236,15 @@
       /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(1, 177, __pyx_L1_error)
 
       /* "View.MemoryView":176
  * 
@@ -10231,15 +10480,15 @@
     /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 193, __pyx_L1_error)
 
     /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
@@ -10965,15 +11214,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -11021,15 +11270,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -12750,15 +12999,15 @@
     /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 420, __pyx_L1_error)
 
     /* "View.MemoryView":419
  * 
@@ -13798,15 +14047,15 @@
       /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(1, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -14160,15 +14409,15 @@
     /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 522, __pyx_L1_error)
 
     /* "View.MemoryView":521
  *     @cname('getbuffer')
@@ -14709,15 +14958,15 @@
     /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 572, __pyx_L1_error)
 
     /* "View.MemoryView":570
  *     @property
@@ -14826,15 +15075,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__32, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__33, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":578
@@ -15864,15 +16113,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -15920,15 +16169,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -16277,17 +16526,17 @@
  *             else:
  */
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice__35);
-            __Pyx_GIVEREF(__pyx_slice__35);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__35);
+            __Pyx_INCREF(__pyx_slice__36);
+            __Pyx_GIVEREF(__pyx_slice__36);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__36);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":685
  *             if not seen_ellipsis:
@@ -16312,15 +16561,15 @@
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__35); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__36); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -16452,17 +16701,17 @@
  * 
  *     return have_slices or nslices, tuple(result)
  */
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice__35);
-        __Pyx_GIVEREF(__pyx_slice__35);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__35);
+        __Pyx_INCREF(__pyx_slice__36);
+        __Pyx_GIVEREF(__pyx_slice__36);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__36);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":697
  * 
@@ -16581,15 +16830,15 @@
       /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(1, 705, __pyx_L1_error)
 
       /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -18765,15 +19014,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -18821,15 +19070,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -22098,15 +22347,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__39, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__40, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
@@ -23370,14 +23619,15 @@
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
   {&__pyx_n_s_H_s, __pyx_k_H_s, sizeof(__pyx_k_H_s), 0, 0, 1, 1},
+  {&__pyx_n_s_I_tar, __pyx_k_I_tar, sizeof(__pyx_k_I_tar), 0, 0, 1, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_u_Inputs_must_fulfill_which_diffs, __pyx_k_Inputs_must_fulfill_which_diffs, sizeof(__pyx_k_Inputs_must_fulfill_which_diffs), 0, 1, 0, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
@@ -23394,37 +23644,42 @@
   {&__pyx_kp_u_The_input_derivative_vector_must, __pyx_k_The_input_derivative_vector_must, sizeof(__pyx_k_The_input_derivative_vector_must), 0, 1, 0, 0},
   {&__pyx_kp_u_The_input_derivative_vector_must_2, __pyx_k_The_input_derivative_vector_must_2, sizeof(__pyx_k_The_input_derivative_vector_must_2), 0, 1, 0, 0},
   {&__pyx_kp_u_The_input_derivative_vector_must_3, __pyx_k_The_input_derivative_vector_must_3, sizeof(__pyx_k_The_input_derivative_vector_must_3), 0, 1, 0, 0},
   {&__pyx_kp_u_The_input_vector_must_be_of_size, __pyx_k_The_input_vector_must_be_of_size, sizeof(__pyx_k_The_input_vector_must_be_of_size), 0, 1, 0, 0},
   {&__pyx_kp_u_The_output_vector_must_be_of_siz, __pyx_k_The_output_vector_must_be_of_siz, sizeof(__pyx_k_The_output_vector_must_be_of_siz), 0, 1, 0, 0},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_UI_vector, __pyx_k_UI_vector, sizeof(__pyx_k_UI_vector), 0, 0, 1, 1},
+  {&__pyx_n_s_UI_vector_auto, __pyx_k_UI_vector_auto, sizeof(__pyx_k_UI_vector_auto), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_V_in, __pyx_k_V_in, sizeof(__pyx_k_V_in), 0, 0, 1, 1},
   {&__pyx_kp_u_V_in_shape_0_needs_to_be_equal_t, __pyx_k_V_in_shape_0_needs_to_be_equal_t, sizeof(__pyx_k_V_in_shape_0_needs_to_be_equal_t), 0, 1, 0, 0},
   {&__pyx_n_s_V_out, __pyx_k_V_out, sizeof(__pyx_k_V_out), 0, 0, 1, 1},
   {&__pyx_kp_u_V_out_shape_0_needs_to_be_equal, __pyx_k_V_out_shape_0_needs_to_be_equal, sizeof(__pyx_k_V_out_shape_0_needs_to_be_equal), 0, 1, 0, 0},
   {&__pyx_kp_u_V_out_shape_1_needs_to_be_equal, __pyx_k_V_out_shape_1_needs_to_be_equal, sizeof(__pyx_k_V_out_shape_1_needs_to_be_equal), 0, 1, 0, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_kp_u_Warning_These_parameters_lie_out, __pyx_k_Warning_These_parameters_lie_out, sizeof(__pyx_k_Warning_These_parameters_lie_out), 0, 1, 0, 0},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_arange, __pyx_k_arange, sizeof(__pyx_k_arange), 0, 0, 1, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_asarray, __pyx_k_asarray, sizeof(__pyx_k_asarray), 0, 0, 1, 1},
+  {&__pyx_n_s_autobinning, __pyx_k_autobinning, sizeof(__pyx_k_autobinning), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_n_s_c_bins, __pyx_k_c_bins, sizeof(__pyx_k_c_bins), 0, 0, 1, 1},
   {&__pyx_n_s_c_max_s, __pyx_k_c_max_s, sizeof(__pyx_k_c_max_s), 0, 0, 1, 1},
+  {&__pyx_n_s_c_maxs, __pyx_k_c_maxs, sizeof(__pyx_k_c_maxs), 0, 0, 1, 1},
   {&__pyx_n_s_c_min_s, __pyx_k_c_min_s, sizeof(__pyx_k_c_min_s), 0, 0, 1, 1},
+  {&__pyx_n_s_c_mins, __pyx_k_c_mins, sizeof(__pyx_k_c_mins), 0, 0, 1, 1},
   {&__pyx_kp_u_c_shape_0_needs_to_be_equal_to_H, __pyx_k_c_shape_0_needs_to_be_equal_to_H, sizeof(__pyx_k_c_shape_0_needs_to_be_equal_to_H), 0, 1, 0, 0},
   {&__pyx_n_s_change_m, __pyx_k_change_m, sizeof(__pyx_k_change_m), 0, 0, 1, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+  {&__pyx_n_s_compat, __pyx_k_compat, sizeof(__pyx_k_compat), 0, 0, 1, 1},
   {&__pyx_n_s_complex128, __pyx_k_complex128, sizeof(__pyx_k_complex128), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
   {&__pyx_n_s_cs, __pyx_k_cs, sizeof(__pyx_k_cs), 0, 0, 1, 1},
   {&__pyx_n_s_dU, __pyx_k_dU, sizeof(__pyx_k_dU), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_double, __pyx_k_double, sizeof(__pyx_k_double), 0, 0, 1, 1},
@@ -23440,28 +23695,31 @@
   {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 0, 1, 0},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
+  {&__pyx_n_s_long, __pyx_k_long, sizeof(__pyx_k_long), 0, 0, 1, 1},
   {&__pyx_n_s_m, __pyx_k_m, sizeof(__pyx_k_m), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
+  {&__pyx_n_s_opt_bins, __pyx_k_opt_bins, sizeof(__pyx_k_opt_bins), 0, 0, 1, 1},
+  {&__pyx_n_s_optimal_binning, __pyx_k_optimal_binning, sizeof(__pyx_k_optimal_binning), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_print, __pyx_k_print, sizeof(__pyx_k_print), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
@@ -23473,34 +23731,36 @@
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
+  {&__pyx_kp_s_src_unipolator_unitary_interpola, __pyx_k_src_unipolator_unitary_interpola, sizeof(__pyx_k_src_unipolator_unitary_interpola), 0, 0, 1, 0},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_kp_s_strided_and_direct, __pyx_k_strided_and_direct, sizeof(__pyx_k_strided_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_direct_or_indirect, __pyx_k_strided_and_direct_or_indirect, sizeof(__pyx_k_strided_and_direct_or_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
+  {&__pyx_n_s_unipolator_unitary_interpolation, __pyx_k_unipolator_unitary_interpolation, sizeof(__pyx_k_unipolator_unitary_interpolation), 0, 0, 1, 1},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_which_diffs, __pyx_k_which_diffs, sizeof(__pyx_k_which_diffs), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 44, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 45, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 48, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 944, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 152, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 834, __pyx_L1_error)
@@ -23509,176 +23769,176 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":44
+  /* "unipolator/unitary_interpolation_vector.pyx":45
  *         self.d2 = self.d * self.d
  *         if not H_s.shape[0] == self.n_dims + 1:
  *             print('Requires n+1 Hamiltonians for n dimensional interpolation. Check lenths of Hs, c_mins, c_maxs, c_bins')             # <<<<<<<<<<<<<<
  *             raise ValueError
  *         self.c_bins = np.empty(self.n_dims, dtype=long)
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Requires_n_1_Hamiltonians_for_n); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Requires_n_1_Hamiltonians_for_n); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":108
+  /* "unipolator/unitary_interpolation_vector.pyx":109
  *             self.d_location[i] = 1 if alpha_rest >= 0 else -1
  *             if self.alpha[i] < 0 or self.alpha[i] > self.c_bins[i]:
  *                 print('Warning: These parameters lie outside of interpolation grid!')             # <<<<<<<<<<<<<<
  *                 break
  *         if is_even(sum_location):
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Warning_These_parameters_lie_out); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Warning_These_parameters_lie_out); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":263
+  /* "unipolator/unitary_interpolation_vector.pyx":264
  *     def expmH(self, double[::1] c, double complex[:,::1] V_in, double complex[:,::1] V_out):
  *         if not c.shape[0] == self.n_dims:
  *             raise ValueError('c.shape[0] needs to be equal to H_s[0].shape[0]-1.')             # <<<<<<<<<<<<<<
  *         # check V_in size
  *         if not V_in.shape[0] == self.d:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_c_shape_0_needs_to_be_equal_to_H); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_c_shape_0_needs_to_be_equal_to_H); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":266
+  /* "unipolator/unitary_interpolation_vector.pyx":267
  *         # check V_in size
  *         if not V_in.shape[0] == self.d:
  *             raise ValueError('V_in.shape[0] needs to be equal to H_s[0].shape[0].')             # <<<<<<<<<<<<<<
  *         if not V_in.shape[1] == self.m:
  *             # change m
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_V_in_shape_0_needs_to_be_equal_t); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_V_in_shape_0_needs_to_be_equal_t); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":272
+  /* "unipolator/unitary_interpolation_vector.pyx":273
  *         # check V_out size
  *         if not V_out.shape[0] == self.d:
  *             raise ValueError('V_out.shape[0] needs to be equal to H_s[0].shape[0].')             # <<<<<<<<<<<<<<
  *         if not V_out.shape[1] == self.m:
  *             raise ValueError('V_out.shape[1] needs to be equal to V_in.shape[1].')
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_V_out_shape_0_needs_to_be_equal); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_V_out_shape_0_needs_to_be_equal); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":274
+  /* "unipolator/unitary_interpolation_vector.pyx":275
  *             raise ValueError('V_out.shape[0] needs to be equal to H_s[0].shape[0].')
  *         if not V_out.shape[1] == self.m:
  *             raise ValueError('V_out.shape[1] needs to be equal to V_in.shape[1].')             # <<<<<<<<<<<<<<
  *         cdef double complex *u0 = &V_in[0, 0]
  *         cdef double complex *v0 = &V_out[0, 0]
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_V_out_shape_1_needs_to_be_equal); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_V_out_shape_1_needs_to_be_equal); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 275, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":290
+  /* "unipolator/unitary_interpolation_vector.pyx":291
  *         cdef double complex *du0 = &dU[0,0,0]
  *         if not c.shape[0] == self.n_dims:
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')             # <<<<<<<<<<<<<<
  *         if not self.n_d_di == dU.shape[0]:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_The_coefficient_c_must_be_of_siz); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_The_coefficient_c_must_be_of_siz); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":292
+  /* "unipolator/unitary_interpolation_vector.pyx":293
  *             raise ValueError('The coefficient c must be of size [interpolation_dimensions].')
  *         if not self.n_d_di == dU.shape[0]:
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')             # <<<<<<<<<<<<<<
  *         if not V_in.shape[0] == self.d:
  *             raise ValueError('The input vector must be of size [d].')
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 292, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Inputs_must_fulfill_which_diffs); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":294
+  /* "unipolator/unitary_interpolation_vector.pyx":295
  *             raise ValueError('Inputs must fulfill: which_diffs.shape[0] = dU.shape[0].')
  *         if not V_in.shape[0] == self.d:
  *             raise ValueError('The input vector must be of size [d].')             # <<<<<<<<<<<<<<
  *         if not V_out.shape[0] == self.d:
  *             raise ValueError('The output vector must be of size [d].')
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_The_input_vector_must_be_of_size); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_The_input_vector_must_be_of_size); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 295, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":296
+  /* "unipolator/unitary_interpolation_vector.pyx":297
  *             raise ValueError('The input vector must be of size [d].')
  *         if not V_out.shape[0] == self.d:
  *             raise ValueError('The output vector must be of size [d].')             # <<<<<<<<<<<<<<
  *         if not V_in.shape[1] == V_out.shape[1] == self.m:
  *             raise ValueError('The input and output vectors must have the same number of columns, and equal to m.')
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_The_output_vector_must_be_of_siz); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_The_output_vector_must_be_of_siz); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":298
+  /* "unipolator/unitary_interpolation_vector.pyx":299
  *             raise ValueError('The output vector must be of size [d].')
  *         if not V_in.shape[1] == V_out.shape[1] == self.m:
  *             raise ValueError('The input and output vectors must have the same number of columns, and equal to m.')             # <<<<<<<<<<<<<<
  *         if not dU.shape[1] == self.d:
  *             raise ValueError('The input derivative vector must be of size [d].')
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_The_input_and_output_vectors_mus); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_The_input_and_output_vectors_mus); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":300
+  /* "unipolator/unitary_interpolation_vector.pyx":301
  *             raise ValueError('The input and output vectors must have the same number of columns, and equal to m.')
  *         if not dU.shape[1] == self.d:
  *             raise ValueError('The input derivative vector must be of size [d].')             # <<<<<<<<<<<<<<
  *         if not dU.shape[2] == self.m:
  *             raise ValueError('The input derivative vector must have the same number of columns as the input and output vectors, and equal to m.')
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_The_input_derivative_vector_must); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_The_input_derivative_vector_must); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":302
+  /* "unipolator/unitary_interpolation_vector.pyx":303
  *             raise ValueError('The input derivative vector must be of size [d].')
  *         if not dU.shape[2] == self.m:
  *             raise ValueError('The input derivative vector must have the same number of columns as the input and output vectors, and equal to m.')             # <<<<<<<<<<<<<<
  *         if not self.n_d_di == dU.shape[0]:
  *             raise ValueError('The input derivative vector must have the same number of rows as the number of derivatives to calculate.')
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_The_input_derivative_vector_must_2); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_The_input_derivative_vector_must_2); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":304
+  /* "unipolator/unitary_interpolation_vector.pyx":305
  *             raise ValueError('The input derivative vector must have the same number of columns as the input and output vectors, and equal to m.')
  *         if not self.n_d_di == dU.shape[0]:
  *             raise ValueError('The input derivative vector must have the same number of rows as the number of derivatives to calculate.')             # <<<<<<<<<<<<<<
  *         self.dexpmH_pointer(c, u0, v0, du0)
  * 
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_The_input_derivative_vector_must_3); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_The_input_derivative_vector_must_3); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 305, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "unipolator/unitary_interpolation_vector.pyx":314
+  /* "unipolator/unitary_interpolation_vector.pyx":315
  *         cdef int is_odd_steps = steps % 2
  *         if not cs.shape[1] == self.n_dims:
  *             raise ValueError('The coefficient matrix must be of size [n_time_steps, interpolation_dimensions].')             # <<<<<<<<<<<<<<
  *         for i in range(0, steps_2, 2):
  *             self.single_parameters2oddgrid(cs[i,:])
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_The_coefficient_matrix_must_be_o); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_The_coefficient_matrix_must_be_o); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 315, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -23700,297 +23960,310 @@
   /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 944, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "../../../../../../anaconda3/envs/mypy/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 950, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
 
   /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
 
   /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 522, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 572, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
 
   /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__32 = PyTuple_New(1); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 579, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
+  __pyx_tuple__33 = PyTuple_New(1); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__32, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__32);
+  PyTuple_SET_ITEM(__pyx_tuple__33, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__33);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
 
   /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__35 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__35)) __PYX_ERR(1, 684, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__35);
-  __Pyx_GIVEREF(__pyx_slice__35);
+  __pyx_slice__36 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__36)) __PYX_ERR(1, 684, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__36);
+  __Pyx_GIVEREF(__pyx_slice__36);
 
   /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__37);
-  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__38);
+  __Pyx_GIVEREF(__pyx_tuple__38);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__38);
-  __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_tuple__39 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_tuple__40 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__40);
+  __Pyx_GIVEREF(__pyx_tuple__40);
+
+  /* "unipolator/unitary_interpolation_vector.pyx":406
+ * 
+ * 
+ * def UI_vector_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long), m = 1):             # <<<<<<<<<<<<<<
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ *     return UI_vector(H_s, c_min_s, c_max_s, opt_bins, which_diffs, m = 1)
+ */
+  __pyx_tuple__41 = PyTuple_Pack(7, __pyx_n_s_H_s, __pyx_n_s_c_min_s, __pyx_n_s_c_max_s, __pyx_n_s_I_tar, __pyx_n_s_which_diffs, __pyx_n_s_m, __pyx_n_s_opt_bins); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(6, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_unipolator_unitary_interpola, __pyx_n_s_UI_vector_auto, 406, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 406, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(1, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__40);
-  __Pyx_GIVEREF(__pyx_tuple__40);
+  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__41 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__41);
-  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_tuple__44 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__44);
+  __Pyx_GIVEREF(__pyx_tuple__44);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__42 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(1, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__42);
-  __Pyx_GIVEREF(__pyx_tuple__42);
+  __pyx_tuple__45 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__45);
+  __Pyx_GIVEREF(__pyx_tuple__45);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(1, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__43);
-  __Pyx_GIVEREF(__pyx_tuple__43);
+  __pyx_tuple__46 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__46);
+  __Pyx_GIVEREF(__pyx_tuple__46);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__44 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(1, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__44);
-  __Pyx_GIVEREF(__pyx_tuple__44);
+  __pyx_tuple__47 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__47);
+  __Pyx_GIVEREF(__pyx_tuple__47);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__45 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__45);
-  __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__48 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__48);
+  __Pyx_GIVEREF(__pyx_tuple__48);
+  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_float_1eneg_10 = PyFloat_FromDouble(1e-10); if (unlikely(!__pyx_float_1eneg_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -24045,24 +24318,24 @@
   __pyx_vtabptr_10unipolator_28unitary_interpolation_vector_UI_vector = &__pyx_vtable_10unipolator_28unitary_interpolation_vector_UI_vector;
   __pyx_vtable_10unipolator_28unitary_interpolation_vector_UI_vector.single_parameters2oddgrid = (PyObject *(*)(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *, __Pyx_memviewslice))__pyx_f_10unipolator_28unitary_interpolation_vector_9UI_vector_single_parameters2oddgrid;
   __pyx_vtable_10unipolator_28unitary_interpolation_vector_UI_vector.interpolate_single_u = (PyObject *(*)(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *, __pyx_t_double_complex *, __pyx_t_double_complex *))__pyx_f_10unipolator_28unitary_interpolation_vector_9UI_vector_interpolate_single_u;
   __pyx_vtable_10unipolator_28unitary_interpolation_vector_UI_vector.interpolate_single_u_du = (PyObject *(*)(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *, __pyx_t_double_complex *, __pyx_t_double_complex *, __pyx_t_double_complex *))__pyx_f_10unipolator_28unitary_interpolation_vector_9UI_vector_interpolate_single_u_du;
   __pyx_vtable_10unipolator_28unitary_interpolation_vector_UI_vector.expmH_pointer = (PyObject *(*)(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *, __Pyx_memviewslice, __pyx_t_double_complex *, __pyx_t_double_complex *))__pyx_f_10unipolator_28unitary_interpolation_vector_9UI_vector_expmH_pointer;
   __pyx_vtable_10unipolator_28unitary_interpolation_vector_UI_vector.dexpmH_pointer = (PyObject *(*)(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *, __Pyx_memviewslice, __pyx_t_double_complex *, __pyx_t_double_complex *, __pyx_t_double_complex *))__pyx_f_10unipolator_28unitary_interpolation_vector_9UI_vector_dexpmH_pointer;
   __pyx_vtable_10unipolator_28unitary_interpolation_vector_UI_vector.expmH_pulse_pointer = (PyObject *(*)(struct __pyx_obj_10unipolator_28unitary_interpolation_vector_UI_vector *, __Pyx_memviewslice, __pyx_t_double_complex *, __pyx_t_double_complex *))__pyx_f_10unipolator_28unitary_interpolation_vector_9UI_vector_expmH_pulse_pointer;
-  if (PyType_Ready(&__pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector.tp_dictoffset && __pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector.tp_dict, __pyx_vtabptr_10unipolator_28unitary_interpolation_vector_UI_vector) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_UI_vector, (PyObject *)&__pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector.tp_dict, __pyx_vtabptr_10unipolator_28unitary_interpolation_vector_UI_vector) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_UI_vector, (PyObject *)&__pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
   __pyx_ptype_10unipolator_28unitary_interpolation_vector_UI_vector = &__pyx_type_10unipolator_28unitary_interpolation_vector_UI_vector;
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
@@ -24306,15 +24579,16 @@
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_memviewslice __pyx_t_5 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  static PyThread_type_lock __pyx_t_6[8];
+  PyObject *__pyx_t_6 = NULL;
+  static PyThread_type_lock __pyx_t_7[8];
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -24423,139 +24697,204 @@
  * from libc.math cimport fabs
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "unipolator/unitary_interpolation_vector.pyx":37
+  /* "unipolator/unitary_interpolation_vector.pyx":10
+ * from .blas_functions cimport *
+ * from .blas_functions_vectors cimport *
+ * from .autobinning import optimal_binning             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_n_s_optimal_binning);
+  __Pyx_GIVEREF(__pyx_n_s_optimal_binning);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_optimal_binning);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_autobinning, __pyx_t_1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_optimal_binning); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_optimal_binning, __pyx_t_1) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "unipolator/unitary_interpolation_vector.pyx":38
  *     cdef long[::1] first_elements_E, first_elements_C, L
  *     cdef long[::1] d_di
  *     def __cinit__(self, double complex[:,:,::1] H_s, double[::1] c_min_s, double[::1] c_max_s, long[::1] c_bins, long[::1] which_diffs = np.array([], dtype=long), int m = 1):             # <<<<<<<<<<<<<<
  *         # Construct parameters
  *         self.n_dims = c_min_s.shape[0]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, ((PyObject *)(&PyLong_Type))) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_k_ = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
+  /* "unipolator/unitary_interpolation_vector.pyx":406
+ * 
+ * 
+ * def UI_vector_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long), m = 1):             # <<<<<<<<<<<<<<
+ *     opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+ *     return UI_vector(H_s, c_min_s, c_max_s, opt_bins, which_diffs, m = 1)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_compat); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_long); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_k__19 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10unipolator_28unitary_interpolation_vector_1UI_vector_auto, NULL, __pyx_n_s_unipolator_unitary_interpolation); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UI_vector_auto, __pyx_t_1) < 0) __PYX_ERR(0, 406, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
   /* "unipolator/unitary_interpolation_vector.pyx":1
  * #cython: language_level=3             # <<<<<<<<<<<<<<
  * import numpy as np
  * cimport numpy as npc
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_4) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "View.MemoryView":210
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(array self):
  */
-  __pyx_t_4 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 210, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_4) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 210, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_array_type);
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__43, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
-  __Pyx_DECREF_SET(generic, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
+  __Pyx_DECREF_SET(generic, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__41, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__44, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
-  __Pyx_DECREF_SET(strided, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
+  __Pyx_DECREF_SET(strided, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__42, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__45, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
-  __Pyx_DECREF_SET(indirect, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
+  __Pyx_DECREF_SET(indirect, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__43, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__46, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
-  __Pyx_DECREF_SET(contiguous, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
+  __Pyx_DECREF_SET(contiguous, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__44, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__47, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
-  __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
+  __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":317
  * 
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0             # <<<<<<<<<<<<<<
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [
  *     PyThread_allocate_lock(),
@@ -24565,59 +24904,59 @@
   /* "View.MemoryView":318
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [             # <<<<<<<<<<<<<<
  *     PyThread_allocate_lock(),
  *     PyThread_allocate_lock(),
  */
-  __pyx_t_6[0] = PyThread_allocate_lock();
-  __pyx_t_6[1] = PyThread_allocate_lock();
-  __pyx_t_6[2] = PyThread_allocate_lock();
-  __pyx_t_6[3] = PyThread_allocate_lock();
-  __pyx_t_6[4] = PyThread_allocate_lock();
-  __pyx_t_6[5] = PyThread_allocate_lock();
-  __pyx_t_6[6] = PyThread_allocate_lock();
-  __pyx_t_6[7] = PyThread_allocate_lock();
-  memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_6, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
+  __pyx_t_7[0] = PyThread_allocate_lock();
+  __pyx_t_7[1] = PyThread_allocate_lock();
+  __pyx_t_7[2] = PyThread_allocate_lock();
+  __pyx_t_7[3] = PyThread_allocate_lock();
+  __pyx_t_7[4] = PyThread_allocate_lock();
+  __pyx_t_7[5] = PyThread_allocate_lock();
+  __pyx_t_7[6] = PyThread_allocate_lock();
+  __pyx_t_7[7] = PyThread_allocate_lock();
+  memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_7, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
 
   /* "View.MemoryView":551
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 551, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_4) < 0) __PYX_ERR(1, 551, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 551, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 551, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryview_type);
 
   /* "View.MemoryView":997
  *         return self.from_object
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 997, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_4) < 0) __PYX_ERR(1, 997, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 997, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 997, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryviewslice_type);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum, NULL, __pyx_n_s_View_MemoryView); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Enum, __pyx_t_4) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum, NULL, __pyx_n_s_View_MemoryView); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Enum, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.name = __pyx_state[0]
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
@@ -24628,14 +24967,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __PYX_XDEC_MEMVIEW(&__pyx_t_5, 1);
+  __Pyx_XDECREF(__pyx_t_6);
   if (__pyx_m) {
     if (__pyx_d) {
       __Pyx_AddTraceback("init unipolator.unitary_interpolation_vector", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init unipolator.unitary_interpolation_vector");
```

### Comparing `unipolator-0.3.0/src/unipolator/unitary_interpolation_vector.pyx` & `unipolator-0.3.2/src/unipolator/unitary_interpolation_vector.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 cimport numpy as npc
 from libc.math cimport fabs
 from .exp_and_log cimport *
 from .indexing cimport *
 from .caching cimport *
 from .blas_functions cimport *
 from .blas_functions_vectors cimport *
+from .autobinning import optimal_binning
 
 
 # Unitary Interpolation
 cdef class UI_vector:
     # Initialize variables, to quickly calculate interpolations while minimizing memmory allocation overheads
     cdef double[::1] c_mins, c_maxs, dcs, das
     cdef long[::1] c_bins
@@ -395,8 +396,13 @@
             #copy_pointer(new_q0, q0, self.d2)
             # flip pointers
             self.ur0, self.ur4 = self.ur4, self.ur0
             self.ur1, self.ur5 = self.ur5, self.ur1
             new_p0, p0 = p0, new_p0
             new_q0, q0 = q0, new_q0
         return I0
-    """
+    """
+
+
+def UI_vector_auto(H_s, c_min_s, c_max_s, I_tar=1e-10, which_diffs = np.array([], dtype=np.compat.long), m = 1):
+    opt_bins  = optimal_binning(H_s, c_mins=c_min_s, c_maxs=c_max_s, I_tar=I_tar)
+    return UI_vector(H_s, c_min_s, c_max_s, opt_bins, which_diffs, m = 1)
```

### Comparing `unipolator-0.3.0/src/unipolator/unitary_interpolation_vector_old.pyx` & `unipolator-0.3.2/src/unipolator/unitary_interpolation_vector_old.pyx`

 * *Files identical despite different names*

### Comparing `unipolator-0.3.0/src/unipolator.egg-info/PKG-INFO` & `unipolator-0.3.2/src/unipolator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: unipolator
-Version: 0.3.0
+Version: 0.3.2
 Summary: Unipolator allows for n dimensional unitary interpolation, and the calculation of propagators using unitary interpolation. Speeds up your propagators for linear quantum systems.
 Home-page: https://github.com/Ntropic/unipolator
-Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.3.0.tar.gz
+Download-URL: https://github.com/Ntropic/unipolator/archive/refs/tags/v0.3.2.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
@@ -36,14 +36,29 @@
 Equivalently if we wish to propagate only wavevectors $\ket{\psi(t)} = U(t) \ket{\psi(0)}$ we initialize the unitary interpolation cache via
 ```
 ui_vector = UI_vector(H_s, c_mins, c_maxs, c_bins, m)  
 ```
 where `m` is the number of wavevectors that are calculated in parallel.
 The package contains further methods listed at the bottom of this document.
 
+## Automatic Binning
+The method `UI_bins` automatically calculates the optimal binning for a target infidelity (default `I_tar=1e-10`). Use via
+```
+bins = UI_bins(H_s, c_mins, c_maxs, I_tar=1e-10)
+```
+By calling 
+```
+ui = UI_auto(H_s, c_mins, c_maxs, I_tar=1e-10)
+```
+or
+```
+ui_vector = UI_vector_auto(H_s, c_mins, c_maxs, I_tar=1e-10, m)
+```
+this method is called automatically during the initialization of the unitary interpolation cache.
+
 ## Calculate:
 We can now use `ui` to calculate matrix exponentials, their derivatives, pulse sequences, and their gradients via the following methods:
 1. `expmH` calculates the unitary $U = \exp(-i H(c) \Delta t)$ for a given set of coefficients `c` (double array of length $n$), pass `U_ui` to the method to store the result (this avoids allocating new memory for every call, and allows reusing the same arrays)
     ```
     ui.expmH( c, U_ui)  
     ``` 
     Similarly we pass two $d \times m$ arrays `V_in` and `V_out`, with the $m$ input wavevectors and for the propagated wavevectors, via
```

### Comparing `unipolator-0.3.0/src/unipolator.egg-info/SOURCES.txt` & `unipolator-0.3.2/src/unipolator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 src/unipolator/__init__.py
+src/unipolator/autobinning.py
 src/unipolator/blas_functions.c
 src/unipolator/blas_functions.pxd
 src/unipolator/blas_functions.pyx
 src/unipolator/blas_functions_vectors.c
 src/unipolator/blas_functions_vectors.pxd
 src/unipolator/blas_functions_vectors.pyx
 src/unipolator/caching.c
@@ -33,15 +34,14 @@
 src/unipolator/symmetric_unitary_interpolation.pyx
 src/unipolator/symmetric_unitary_interpolation_vector.c
 src/unipolator/symmetric_unitary_interpolation_vector.pyx
 src/unipolator/trotter_system.c
 src/unipolator/trotter_system.pyx
 src/unipolator/trotter_system_vector.c
 src/unipolator/trotter_system_vector.pyx
-src/unipolator/unipolator.pyx
 src/unipolator/unitary_interpolation.c
 src/unipolator/unitary_interpolation.pyx
 src/unipolator/unitary_interpolation_vector.c
 src/unipolator/unitary_interpolation_vector.pyx
 src/unipolator/unitary_interpolation_vector_old.pyx
 src/unipolator.egg-info/PKG-INFO
 src/unipolator.egg-info/SOURCES.txt
```

### Comparing `unipolator-0.3.0/test/Outlook/expm_v.pyx` & `unipolator-0.3.2/test/Outlook/expm_v.pyx`

 * *Files identical despite different names*

