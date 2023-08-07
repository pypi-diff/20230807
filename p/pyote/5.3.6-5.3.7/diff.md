# Comparing `tmp/pyote-5.3.6.tar.gz` & `tmp/pyote-5.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyote-5.3.6.tar", last modified: Sat Jul 29 17:48:16 2023, max compression
+gzip compressed data, was "pyote-5.3.7.tar", last modified: Mon Aug  7 16:29:15 2023, max compression
```

## Comparing `pyote-5.3.6.tar` & `pyote-5.3.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 17:48:16.956109 pyote-5.3.6/
--rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.3.6/LICENSE
--rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1190 2023-07-29 17:48:16.956109 pyote-5.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.3.6/README.rst
--rw-rw-rw-   0        0        0       81 2023-07-29 17:48:16.957108 pyote-5.3.6/setup.cfg
--rw-rw-rw-   0        0        0     2945 2023-07-22 13:57:05.000000 pyote-5.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:48:16.787407 pyote-5.3.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 17:48:16.810635 pyote-5.3.6/src/pyote.egg-info/
--rw-rw-rw-   0        0        0     1190 2023-07-29 17:48:16.000000 pyote-5.3.6/src/pyote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1789 2023-07-29 17:48:16.000000 pyote-5.3.6/src/pyote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 17:48:16.000000 pyote-5.3.6/src/pyote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.3.6/src/pyote.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      268 2023-07-29 17:48:16.000000 pyote-5.3.6/src/pyote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-29 17:48:16.000000 pyote-5.3.6/src/pyote.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-29 17:48:16.923769 pyote-5.3.6/src/pyoteapp/
--rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.3.6/src/pyoteapp/PYOTE.bat
--rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.3.6/src/pyoteapp/SER.py
--rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.3.6/src/pyoteapp/__init__.py
--rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.3.6/src/pyoteapp/autocorrtools.py
--rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.3.6/src/pyoteapp/blockIntegrateUtils.py
--rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.3.6/src/pyoteapp/checkForNewerVersion.py
--rw-rw-rw-   0        0        0    12525 2023-06-30 14:42:34.000000 pyote-5.3.6/src/pyoteapp/csvreader.py
--rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.3.6/src/pyoteapp/diffraction-table.p
--rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.3.6/src/pyoteapp/errorBarUtils.py
--rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.3.6/src/pyoteapp/example-penumbral.csv
--rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.3.6/src/pyoteapp/exponentialEdgeUtilities.py
--rw-rw-rw-   0        0        0     6835 2023-07-16 03:05:04.000000 pyote-5.3.6/src/pyoteapp/false_positive.py
--rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.3.6/src/pyoteapp/fixedPrecision.py
--rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.3.6/src/pyoteapp/genDiffraction.py
--rw-rw-rw-   0        0        0   386867 2023-07-29 17:27:02.000000 pyote-5.3.6/src/pyoteapp/gui.py
--rw-rw-rw-   0        0        0     1907 2023-06-17 17:37:29.000000 pyote-5.3.6/src/pyoteapp/helpDialog.py
--rw-rw-rw-   0        0        0    25723 2023-07-07 20:15:46.000000 pyote-5.3.6/src/pyoteapp/iterative_logl_functions.py
--rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.3.6/src/pyoteapp/likelihood_calculations.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:48:16.955116 pyote-5.3.6/src/pyoteapp/model-examples/
--rw-rw-rw-   0        0        0     1209 2023-05-29 17:45:05.000000 pyote-5.3.6/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p
--rw-rw-rw-   0        0        0     1204 2023-05-29 18:25:21.000000 pyote-5.3.6/src/pyoteapp/model-examples/LCP_penumbral.p
--rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.3.6/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.3.6/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.3.6/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.3.6/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
--rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.3.6/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.3.6/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.3.6/src/pyoteapp/model-help.pdf
--rw-rw-rw-   0        0        0     1926 2023-05-11 18:15:42.000000 pyote-5.3.6/src/pyoteapp/noiseUtils.py
--rw-rw-rw-   0        0        0   397985 2023-07-29 17:35:24.000000 pyote-5.3.6/src/pyoteapp/pyote-info.pdf
--rw-rw-rw-   0        0        0   452150 2023-07-29 17:17:45.000000 pyote-5.3.6/src/pyoteapp/pyote.py
--rw-rw-rw-   0        0        0    79636 2023-06-17 20:42:15.000000 pyote-5.3.6/src/pyoteapp/pyote_modelling_utility_functions.py
--rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.3.6/src/pyoteapp/run-pyote-mac.bat
--rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.3.6/src/pyoteapp/showVideoFrames.py
--rw-rw-rw-   0        0        0    23501 2023-07-07 02:06:56.000000 pyote-5.3.6/src/pyoteapp/solverUtils.py
--rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.3.6/src/pyoteapp/subframe_timing_utilities.py
--rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.3.6/src/pyoteapp/timestampDialog.py
--rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.3.6/src/pyoteapp/timestampUtils.py
--rw-rw-rw-   0        0        0       34 2023-07-29 17:45:54.000000 pyote-5.3.6/src/pyoteapp/version.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:29:15.190222 pyote-5.3.7/
+-rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.3.7/LICENSE
+-rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1190 2023-08-07 16:29:15.190222 pyote-5.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.3.7/README.rst
+-rw-rw-rw-   0        0        0       81 2023-08-07 16:29:15.191240 pyote-5.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     2945 2023-07-22 13:57:05.000000 pyote-5.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:29:15.019595 pyote-5.3.7/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 16:29:15.031686 pyote-5.3.7/src/pyote.egg-info/
+-rw-rw-rw-   0        0        0     1190 2023-08-07 16:29:15.000000 pyote-5.3.7/src/pyote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1789 2023-08-07 16:29:15.000000 pyote-5.3.7/src/pyote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 16:29:15.000000 pyote-5.3.7/src/pyote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.3.7/src/pyote.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      268 2023-08-07 16:29:15.000000 pyote-5.3.7/src/pyote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 16:29:15.000000 pyote-5.3.7/src/pyote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 16:29:15.156224 pyote-5.3.7/src/pyoteapp/
+-rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.3.7/src/pyoteapp/PYOTE.bat
+-rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.3.7/src/pyoteapp/SER.py
+-rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.3.7/src/pyoteapp/__init__.py
+-rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.3.7/src/pyoteapp/autocorrtools.py
+-rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.3.7/src/pyoteapp/blockIntegrateUtils.py
+-rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.3.7/src/pyoteapp/checkForNewerVersion.py
+-rw-rw-rw-   0        0        0    12525 2023-06-30 14:42:34.000000 pyote-5.3.7/src/pyoteapp/csvreader.py
+-rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.3.7/src/pyoteapp/diffraction-table.p
+-rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.3.7/src/pyoteapp/errorBarUtils.py
+-rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.3.7/src/pyoteapp/example-penumbral.csv
+-rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.3.7/src/pyoteapp/exponentialEdgeUtilities.py
+-rw-rw-rw-   0        0        0     6835 2023-07-16 03:05:04.000000 pyote-5.3.7/src/pyoteapp/false_positive.py
+-rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.3.7/src/pyoteapp/fixedPrecision.py
+-rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.3.7/src/pyoteapp/genDiffraction.py
+-rw-rw-rw-   0        0        0   386867 2023-07-29 17:27:02.000000 pyote-5.3.7/src/pyoteapp/gui.py
+-rw-rw-rw-   0        0        0     1907 2023-06-17 17:37:29.000000 pyote-5.3.7/src/pyoteapp/helpDialog.py
+-rw-rw-rw-   0        0        0    25723 2023-07-07 20:15:46.000000 pyote-5.3.7/src/pyoteapp/iterative_logl_functions.py
+-rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.3.7/src/pyoteapp/likelihood_calculations.py
+drwxrwxrwx   0        0        0        0 2023-08-07 16:29:15.189222 pyote-5.3.7/src/pyoteapp/model-examples/
+-rw-rw-rw-   0        0        0     1209 2023-05-29 17:45:05.000000 pyote-5.3.7/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p
+-rw-rw-rw-   0        0        0     1204 2023-05-29 18:25:21.000000 pyote-5.3.7/src/pyoteapp/model-examples/LCP_penumbral.p
+-rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.3.7/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.3.7/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.3.7/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.3.7/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
+-rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.3.7/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.3.7/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.3.7/src/pyoteapp/model-help.pdf
+-rw-rw-rw-   0        0        0     1926 2023-05-11 18:15:42.000000 pyote-5.3.7/src/pyoteapp/noiseUtils.py
+-rw-rw-rw-   0        0        0   398170 2023-08-07 16:26:51.000000 pyote-5.3.7/src/pyoteapp/pyote-info.pdf
+-rw-rw-rw-   0        0        0   453284 2023-08-07 16:19:25.000000 pyote-5.3.7/src/pyoteapp/pyote.py
+-rw-rw-rw-   0        0        0    79636 2023-06-17 20:42:15.000000 pyote-5.3.7/src/pyoteapp/pyote_modelling_utility_functions.py
+-rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.3.7/src/pyoteapp/run-pyote-mac.bat
+-rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.3.7/src/pyoteapp/showVideoFrames.py
+-rw-rw-rw-   0        0        0    23501 2023-07-07 02:06:56.000000 pyote-5.3.7/src/pyoteapp/solverUtils.py
+-rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.3.7/src/pyoteapp/subframe_timing_utilities.py
+-rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.3.7/src/pyoteapp/timestampDialog.py
+-rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.3.7/src/pyoteapp/timestampUtils.py
+-rw-rw-rw-   0        0        0       34 2023-08-07 16:15:33.000000 pyote-5.3.7/src/pyoteapp/version.py
```

### Comparing `pyote-5.3.6/LICENSE` & `pyote-5.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/PKG-INFO` & `pyote-5.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.3.6
+Version: 5.3.7
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.3.6/setup.py` & `pyote-5.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyote.egg-info/PKG-INFO` & `pyote-5.3.7/src/pyote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.3.6
+Version: 5.3.7
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.3.6/src/pyote.egg-info/SOURCES.txt` & `pyote-5.3.7/src/pyote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/SER.py` & `pyote-5.3.7/src/pyoteapp/SER.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/autocorrtools.py` & `pyote-5.3.7/src/pyoteapp/autocorrtools.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/blockIntegrateUtils.py` & `pyote-5.3.7/src/pyoteapp/blockIntegrateUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/checkForNewerVersion.py` & `pyote-5.3.7/src/pyoteapp/checkForNewerVersion.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/csvreader.py` & `pyote-5.3.7/src/pyoteapp/csvreader.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/diffraction-table.p` & `pyote-5.3.7/src/pyoteapp/diffraction-table.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/errorBarUtils.py` & `pyote-5.3.7/src/pyoteapp/errorBarUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/example-penumbral.csv` & `pyote-5.3.7/src/pyoteapp/example-penumbral.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/exponentialEdgeUtilities.py` & `pyote-5.3.7/src/pyoteapp/exponentialEdgeUtilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/false_positive.py` & `pyote-5.3.7/src/pyoteapp/false_positive.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/fixedPrecision.py` & `pyote-5.3.7/src/pyoteapp/fixedPrecision.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/genDiffraction.py` & `pyote-5.3.7/src/pyoteapp/genDiffraction.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/gui.py` & `pyote-5.3.7/src/pyoteapp/gui.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/helpDialog.py` & `pyote-5.3.7/src/pyoteapp/helpDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/iterative_logl_functions.py` & `pyote-5.3.7/src/pyoteapp/iterative_logl_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/likelihood_calculations.py` & `pyote-5.3.7/src/pyoteapp/likelihood_calculations.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p` & `pyote-5.3.7/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/model-examples/LCP_penumbral.p` & `pyote-5.3.7/src/pyoteapp/model-examples/LCP_penumbral.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.7/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.7/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.7/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv` & `pyote-5.3.7/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.3.7/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.3.7/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/model-help.pdf` & `pyote-5.3.7/src/pyoteapp/model-help.pdf`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/noiseUtils.py` & `pyote-5.3.7/src/pyoteapp/noiseUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/pyote-info.pdf` & `pyote-5.3.7/src/pyoteapp/pyote-info.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,8 +1,11 @@
 Version history (PyOTE description – out of date - is at end)
+Version 5.3.7
+7 August 2023
+• Adds csv source file information to fit metrics xlsx file
 Version 5.3.6
 29 July 2023
 • Colors a FP FAILED metric log entry red
 Version 5.3.5
 22 July 2023
 • Fixes Mac filepath issues
 Version 5.3.4
@@ -37,19 +40,18 @@
 due to noise and so we can loosen up the initial test.
 •
 
 Fixed some issues around removing and adding data sets on the light curve tab. Now
 the data grid at the lower left tracks the deletes and adds properly and the entire list of
 light curves can be cleared.
 
-Version 5.2.8
+Version 5.2.8
 30 June 2023
 • Added detection of duplicate column names (only possible in a csv file from PyMovie).
-
-Duplicate names cause the column data to be concatenated and this cannot be
+Duplicate names cause the column data to be concatenated and this cannot be
 tolerated, so when this error is found, the data import is aborted.
 The user will need to edit the csv file to resolve the name duplication.
 •
 
 Added a warning message that will only appear if a user manually calculates baseline
 statistics and then does a find event. Sometimes that is exactly what is wanted, but
 those statistics become fixed and will be used for all subsequent find event clicks.
@@ -100,24 +102,20 @@
 Changed snr to dnr (drop to noise ratio) in the places where that is the actual
 calculation being performed.
 
 Version 5.2.4
 11 May 2023
 • Fixes an edge case – when only two points were in the event bottom, sigmaA was
 being set to 0.0 (causing an assertion error) rather than setting it to the value
-previously determined for sigmaB.
-Version 5.2.3
 
+previously determined for sigmaB.
+Version 5.2.3
 2 May 2023
-
-•
-
-Restores the calculation of timeDelta to 6 digit precision (it had been inadvertently
+• Restores the calculation of timeDelta to 6 digit precision (it had been inadvertently
 limited to 4 digits by a previous change)
-
 •
 
 Fixes a bug in the calculation of flash edge times that was discovered when very high
 SNR recording was attempted
 
 Version 5.2.2
 13 April 2023
@@ -157,18 +155,17 @@
 • Fixes VizieR file preparation code to detect when lat or long is given with a + sign
 (common when input comes from reading a .xlsx file)and avoid adding a redundant +
 (double) character.
 •
 
 Reverts to using pyqtgraph 0.12.4
 
-Version 5.1.0 7 February 2023
+Version 5.1.0 7 February 2023
 • Changed the way data sets (lightcurves) read from a PyMovie csv file are selected for
-
-viewing. Whereas previously it was possible to specify a ‘prefix’ to be used when
+viewing. Whereas previously it was possible to specify a ‘prefix’ to be used when
 reading PyMovie csv files (such as ‘signal’ or ‘appsum’), it was not possible to mix-andmatch data sets with different prefixes. With this version, that now becomes possible.
 With this feature, it now becomes possible to demonstrate for yourself that there is no
 reason to process a target lightcurve in ‘aperture sum’ mode (no background
 subtraction) versus the regular ‘signal’ mode (where background subtraction is
 performed). Simply display the ‘signal’ and ‘appsum’ versions of a target lightcurve and
 use the y position spinBox on one of the curves until they overlap. This should show
 that during the event, the points almost exactly overlap, so event timing will be the
@@ -204,19 +201,18 @@
 • model-examples folder is now being placed in the Documents folder rather than the
 Desktop folder.
 •
 
 Launch from python3 or python or py now detected and dealt with when checking PyPI
 repository for latest version.
 
-Version 5.0.2 8 January 2023
+Version 5.0.2 8 January 2023
 • Added timing problem report – counts of dropped readings; duplicated readings;
 cadence error. These appear in the log box (lower right corner) and are written to the
-
-log file.
+log file.
 •
 
 Made D and R edge time calculations work properly even when there are dropped
 readings in the observation
 
 Version 5.0.0 6 January 2023
 • Added ability to specify a block size to be used during automatic block integration.
@@ -248,23 +244,20 @@
 Cadence jitter happens when high frame rates create a situation where frame recording cannot keep up and the traffic control implemented by the computer changes the
 arrival/timestamp time of frames so that some appear a little earlier and others a little
 late.
 Cadence jitter is defined as a timing discrepancy of between 20% and 80% of a frame
 time and is represented by a yellow line.
 Timing discrepancies greater than 80% of a frame time continue to be shown as a red
 line and are assumed to come from dropped frames. In any case, they deserve
-attention.
-Version 4.8.8 7 August 2022
 
-•
-
-Added message at normal program close to the effect that QBasicTimer messages
+attention.
+Version 4.8.8 7 August 2022
+• Added message at normal program close to the effect that QBasicTimer messages
 that appear after the program has closed are harmless artifacts of the order in which
 QUI elements are closed.
-
 Version 4.8.7 29 July 2022
 • changed numpy version requirement to match that of PyMovie so that ultimately the
 two programs can share a virtual environment, thus saving much space.
 Version 4.8.6 23 July 2022
 • added instructions telling the user how to install a new version when one is found.
 There are instructions for pip based installations and pipenv installations
 Version 4.8.4
@@ -294,19 +287,19 @@
 removes the writing of the startup batch file as a different method will be used in
 conjunction with pipenv.
 
 Version 4.7.9
 • disables the compiling to C code (which was done to increase execution speed) of
 routines used for finding an event using min/max size. There is compelling (but
 indirect) evidence that the C compiler on Win11 (and maybe only for the i5 processor)
-is generating incorrect code. This issue showed up recently with 2 users who had
+
+is generating incorrect code. This issue showed up recently with 2 users who had
 installed Win11 on i5 processor-based computer. On those machines, finding an event
 using min/max would always hang at 99% completion. Allowing the original Python
-
-code to be used instead of compiling to C-code resolved that issue. As finding an event
+code to be used instead of compiling to C-code resolved that issue. As finding an event
 using min/max size minimizes the number of candidate solutions naturally, the loss of
 speed is not so important – it’s fast enough.
 version 4.6.4
 • made the 'camera response' checkbox (in the Settings/misc tab) sticky
 •
 
 corrected the log messaging about Donly, Ronly, DandR, and min/max directions to the
@@ -340,18 +333,17 @@
 change when hovering over a splitter. As this is confusing, the busy cursor feature has
 been removed.
 version 4.5.5
 • fixes a bug where, if a full D and R light-curve was split (trimmed) into a D-only and an
 R-only light-curve, the R-only result did not apply subframe timing adjustments
 version 4.5.4
 • cleans up the the first bin of the False-Positive histogram
-version 4.5.3
-• adds an option to validate a single point event to the Analysis tab. It uses the false-
 
-positive test procedure to determine if the selected point had a non-zero chance to
+version 4.5.3
+• adds an option to validate a single point event to the Analysis tab. It uses the falsepositive test procedure to determine if the selected point had a non-zero chance to
 have been caused by baseline noise alone.
 version 4.5.2
 • fixes a bug where transition points (only present in high SNR light-curves) were not
 properly ignored during calculation of event noise. This manifested itself most clearly in
 too large error bars for magDrop
 version 4.5.0
 • fixes a bug introduced with the NE3 code changes that inhibited sub-frame timing
@@ -380,19 +372,19 @@
 •
 
 made it possible to select the points of the normalized target lightcurve to be included
 in the std metric
 
 version 4.3.6
 • added a simple metric as an aid to selecting an appropriate number of readings to use
-to smooth the reference curve used for normalization. It is printed in green whenever
+
+to smooth the reference curve used for normalization. It is printed in green whenever
 normalization is active. It is simply the standard deviation of the normalized target
 lightcurve. Although it is quite simple, it is a value that is minimized the more level and
-
-the less bumpy the normalized target curve is.
+the less bumpy the normalized target curve is.
 When normalization is active, at each change, a pair of metrics are printed in the log
 panel.
 The red metric is the Pearson R value of the correlation between the target lightcurve
 and the reference lightcurve; it should be maximized (using the X offset spinbox of the
 reference curve) at the point where the two curves are properly time-aligned. It is also
 affected by the smoothing interval, but this connection should be ignored.
 The green metric is the standard deviation of the target lightcurve – it is lowered when
@@ -423,20 +415,21 @@
 • fixes an error message that occurs during the initial installation of a version that has a
 change to the number of tabs in the GUI
 version 4.3.0
 • minor cosmetic cleanup to deal with Windows GUI differences (I hope it works – this is
 always a frustrating and mysterious area)
 version 4.2.9
 • adds the lightcurve used to the report generated during the detectability analysis
-•
+
+•
 
 automatically clears the effect of previous normailzation when the reference lightcurve
 is changed (or deselected)
 
-version 4.2.8
+version 4.2.8
 • fixes 'trim problem'
 •
 
 adds 'step by' buttons that change the smoothing interval spinbox step size.
 
 version 4.2.6
 • tidies up the lightcurve panel a bit and changes color samples for target and reference
@@ -477,18 +470,18 @@
 version 4.2.2
 • adds a new tab/panel for controlling the display of lightcurves. From the 'help button'
 on that tab:
 This panel allows up to 10 lightcurves to be displayed at the same time. If the csv file has
 more than 10 lightcurves, the first 10 are displayed.
 The target lightcurve is always drawn with bright blue dots.
 If a lightcurve is selected as a reference to be used for normalization, it is always
-drawn with bright green dots.
-Unless a lightcurve is designated as a target (curve to be analyzed for an event) or is
 
-designated as a reference lightcurve, its dot color depends on the row it is in - every
+drawn with bright green dots.
+Unless a lightcurve is designated as a target (curve to be analyzed for an event) or is
+designated as a reference lightcurve, its dot color depends on the row it is in - every
 row has a unique color other than blue or green.
 Lightcurves can be displaced up or down using the Y offset spinner to control the
 displacement. This affects the display position only; the underlying values are not
 affected. This facility was added to allow the separation of lightcurves that would
 otherwise overlap in a confusing manner.
 There can only be one lightcurve selected as target.
 There can be either 0 or 1 lightcurve selected as a reference for normalization.
@@ -524,20 +517,21 @@
 Win 10 accepts / as a separator – Win 11 apparently does not (unless there is some
 setting that will persuade Win 11 to accept either separator.
 version 4.1.8
 • adds option to write sample light-curve from detectability analysis to a csv file that be
 imported to PyOTE.
 version 4.1.7
 • adds the requirement to specify an observation duration when doing a detectability test
-•
+
+•
 
 during a detectability test, if a detectable event was found, a sample light-curve
 showing such an event is plotted, otherwise the normal False-Positive plot will be
+shown.
 
-shown.
 version 4.1.6
 • reenables Cholesky failure messages (disabled for testing)
 •
 
 Adds test to detectability routine so that the user cannot give an event duration that
 requires more points than are available in the observation.
 
@@ -586,19 +580,19 @@
 your NE3 at a gamma of 0.75 (1.0 gamma is not available) AND that you use PyMovie
 to linearize the recording (i.e., invert the 0.75 gamma curve of the camera).
 
 •
 
 The D and R exponential curves each have their own time constant, measured in
 frames, that control the frame rate of exponential curve growth. The default values
-provided are usually enough to provide the starting point for a good fit. This starting
+
+provided are usually enough to provide the starting point for a good fit. This starting
 point is used by PyOTE during a least-squares driven search for better time constant
 values. If the starting point given is too far from 'correct', the least-squares search may
-
-settle in a local minimum that produces a fit that is visually bad. In this case, change
+settle in a local minimum that produces a fit that is visually bad. In this case, change
 the starting value to something closer to 'correct' and try again.
 •
 
 When the exponential curve fit algorithm is in use, the light-curve plot PyOTE displays
 will be changed. Gone is the blue 'camera response' curve, replaced by brown dotted
 'theoretical' exponential edge curves that you can use to judge for yourself the
 goodness of a 'fit'.
@@ -634,19 +628,19 @@
 version 4.0.8
 • fixes bug (introduced by a misspelling in version 4.0.7) that kept csv files with more
 than four apertures from runnig.
 version 4.0.7
 • adds the ability to select the PyMovie data column type to be analyzed. There are two
 main column types that are likely to be used: signal, which has background subtracted
 and appsum, which has no background subtracted – it's the raw mask pixels summed.
-Some others are available: avgbkd (shows the average pixel value in the aperture);
+
+Some others are available: avgbkd (shows the average pixel value in the aperture);
 stdbkg (shows the pixel noise in the background pixels in the aperture); nmaskpx
 (which shows the nuber of pixels in the sampling mask – there are times when this
-
-curve can be used to extrat event times).
+curve can be used to extrat event times).
 Note: this only applies to csv files generated by PyMovie.
 version 4.0.6
 • minor GUI changes
 version 4.0.5
 • if you click outside the light-curve, the closest point will be toggled (so you don't have
 to zoom in to select the leftmost or rightmost point in a light-curve.
 •
@@ -682,18 +676,18 @@
 version 4.0.2
 • removed a debug print statement that was inadvertently left in. It is responsible for the
 “mouse event” messages polluting the log file.
 version 4.0.1
 • increased width of detectibility plots to (hopefully) deal with Windows tendency to
 truncate the plots. If this doesn't work, then this will be a permanent feature (not a bug)
 for Win10 installations.
-version 4.0.0
-• detectibility graphics plots are now being being put in their own folder. The root folder is
 
-that of the directory where the light-curve came from. The plots will be found in
+version 4.0.0
+• detectibility graphics plots are now being being put in their own folder. The root folder is
+that of the directory where the light-curve came from. The plots will be found in
 lightCurveDirectory\DetectibilityPlots\
 In addition, if you supply a duration step size, which is the way to ask the detectibilty
 calculator to step from the given duration down until an event of that duration fails the
 False-positive test, only the final plot (where False-positive became non-zero) will be
 plotted.
 All of the above is just to cut down on clutter in the light-curve directory and to only plot
 meaningful graphics generated during the minimum duration search.
@@ -721,19 +715,18 @@
 sticky stuff.
 This version also removes the 'scrunch' of the lefthand button panel.
 version 3.9.6
 • another attempt fix the startup gui size issue on smaller legacy monitors. This version
 has a design size of 1900x1000. It may be necessary to delete the simple-ote.ini file
 that 'remembers' size and position settings. It is located in whatever directory PyOTE
 starts up in.
-version 3.9.5
-• adds automation to the 'detectibility' calculator. If a duration step size is entered, a
-series of 'detectibility' calculations will be made at decreasing durations until the false-
 
-positive probability becomes non-zero. A unique .png (incorporates duration and
+version 3.9.5
+• adds automation to the 'detectibility' calculator. If a duration step size is entered, a
+series of 'detectibility' calculations will be made at decreasing durations until the falsepositive probability becomes non-zero. A unique .png (incorporates duration and
 magDrop in the file name) will be written to the directory of the light-curve and the final
 plot where detection failed will be left on-screen.
 If the duration step size is left unfilled or is zero, a single 'detectibility' calculation will be
 made as before.
 version 3.9.4
 • attempts to fix over-size initial gui.
 version 3.9.3
@@ -762,18 +755,18 @@
 producing a report.
 version 3.8.7
 • changed the way curve to analyze and normalization curve are selected to make it less
 confusing. Now, if there is a conflict (same curve selected for analysis and
 normalization) the other one is set to 0 (a new value) to 'get it out of the way'. It may
 still be a little bit confusing when you need to crossover, but if you set the higher
 numbered curve first, it will be easy.
-version 3.8.6
-• checks for only a single light-curve in the csv file which was causing a 'list index out of
 
-range' error message
+version 3.8.6
+• checks for only a single light-curve in the csv file which was causing a 'list index out of
+range' error message
 version 3.8.5
 • changed the way QGridLayout was referenced.
 version 3.8.4
 • changed the way QTableWidgetItem and QApplication were referenced to
 accommodate the latest Anaconda version, which has reorganized where those
 modules are stored. A similar change was made in version 3.7.6 and I do not know
 how this has gone uncorrected for so long – I hope that I have not missed something.
@@ -803,18 +796,21 @@
 the baseline that are outside the 'flash-zone' can be specified. Look for a button
 labelled Mark baseline region located near the bottom-left of the GUI panel.
 This tool may also be useful for wind-gust situations, headlights from passing cars,
 bumping the telescope, etc. In the past, such accidents might have required extensive
 'clipping' of the light-curve to avoid the affected areas, with a consequent loss of
 information. Hopefully this tool will alleviate those situations.
 version 3.7.8
-• added visible left, top, and bottom axes to main plot (with ticks to make easier to
+
+•
+
+added visible left, top, and bottom axes to main plot (with ticks to make easier to
 associate timestamp with point).
 
-version 3.7.7
+version 3.7.7
 • if timestamps are available in the csv file, they are used as x axis labels in the main
 plot.
 version 3.7.6
 • changed the way QMainWindow and Qapplication were referenced to accommodate
 the latest Anaconda version, which has reorganized where those modules are stored.
 This was causing a fatal startup error.
 version 3.7.5
@@ -843,20 +839,21 @@
 version 3.7.2
 • fixes bug that caused all analysis attempts to 'stall'
 version 3.7.1
 • fixed a bug in the r limb angle entry
 version 3.7.0
 • adds right-click help to ast speed label giving the equation to use if asteroid
 speed is not available but asteroid diameter and maximum duration are
-specified
+
+specified
 •
 
 adds suggestion to right-click help on penumbral fit checkbox for how to find the
+penumbral curve csv file that is provided for practice purposes.
 
-penumbral curve csv file that is provided for practice purposes.
 version 3.6.8
 • adds modeling of off centerline observations to lightcurve calibration curve
 generation
 version 3.6.7
 • clarified the location of the Enable Manual Timestamp Entry checkbox in the
 pop-up message appears when there are no timestamps in the csv file.
 version 3.6.6
@@ -882,20 +879,18 @@
 formatting to control rounding, etc
 … if I can't write to the selected file, I ask whether you might have it open
 somewhere else already
 version 3.6.1
 • reduced number of digits in the error bar numbers to 2 written to the Asteroid
 Occultation Report Form so that the resulting number fits within the allotted cell
 size. (I'm told that Occult only uses 2 digits anyway.) I also updated the context
-help associated with the … fill Excel report button
-version 3.6.0
-
-•
 
-provides the ability to fill entries in the Excel spreadsheet Asteroid Occultation
+help associated with the … fill Excel report button
+version 3.6.0
+• provides the ability to fill entries in the Excel spreadsheet Asteroid Occultation
 Report Form from PyOTE results, thus eliminating transcription errors.
 A button to allow the user to activate this 'fill' has been added just to the right of
 
 the … write report button
 NOTE: the normal .xls report form that OccultWatcher creates and prefills (when
 requested) during your report to OccultWatcher ...
 … MUST BE CONVERTED to .xlsx for use by PyOTE!
@@ -916,19 +911,19 @@
 that it is ready for submission.
 version 3.5.9
 • fixed another bug in penumbral curve fit and removed diagnostic printouts.
 version 3.5.8
 • fixed a number of bugs in the penumbral curve fit code
 version 3.5.7
 • automatically turns off the display of the normalizing lightcurve when a
-normalization is performed. It was a source of confusion to leave the normalizing
+
+normalization is performed. It was a source of confusion to leave the normalizing
 lightcurve visible because it was sometimes the case that the normalization
 appeared not to have occurred (when the normalization effect was
-
-subtle/minor).
+subtle/minor).
 version 3.5.6
 • fixed a bug that kept a user from selecting a new file to read if PyOTE had been
 started from PyMovie. Previously, it had only reopened the same file instead of
 giving the user a file select dialog to choose from.
 version 3.5.5
 • fixed a bug that kept occultations from being extracted from lightcurves 5 and
 up. The lightcurves above 4 could be viewed --- they just couldn't be processed
@@ -958,18 +953,18 @@
 without requiring in-depth understanding of the internal workings of the program,
 we have decided to make the end-point smoothing issue very apparent by doing
 an automatic 'trim' of the points affected by extrapolation.
 version 3.5.1
 • Added additional references to the North American Excel Spreadsheet report in
 the new section of the final report that bangs on about the start-of-exposure
 timing convention.
-version 3.5.0
-• When PyMovie files are read, the aperture names are now being used in the
 
-data table (lower left panel) as column headings and used during the 'write csv'
+version 3.5.0
+• When PyMovie files are read, the aperture names are now being used in the
+data table (lower left panel) as column headings and used during the 'write csv'
 process. This makes the format of the PyOTE csv file match the PyMovie
 format so that AOTA can read both PyMovie csv files AND PyOTE csv files.
 •
 
 NEW: when 'trims' have been placed, a 'write csv' process will honor those
 values and produce a 'trimmed' output file.
 
@@ -1003,22 +998,22 @@
 The above observation suggests that reliable estimates of magDrop require that A be greater
 than std(A) --- that is the ad hoc reason that we have defined limMagDrop as we have.
 This value is substituted for a calculated magDrop whenever A is less than std(A), i.e.,
 whenever A is at or below std(A).
 limMagDrop values are reported with a leading > symbol to signify that that value is a
 limMagDrop value. They are easy to spot in the report.
 version 3.4.7
-• Automatically loads the correct version of Adv2
-version 3.4.6
 
 •
 
-Adds AAV Version 2 file as a type that can be read (important when Do OCR
-check is enabled)
+Automatically loads the correct version of Adv2
 
+version 3.4.6
+• Adds AAV Version 2 file as a type that can be read (important when Do OCR
+check is enabled)
 version 3.4.5
 • Fixes block integration which was failing when more than 4 lightcurves were
 being processed.
 •
 
 Made use diff and Do OCR checkboxes sticky.
 
@@ -1049,28 +1044,28 @@
 plotted, or edges are plotted --- a cleaner plot is the major result and you have
 better control over the 'look'
 •
 
 Added a checkbox to disable the automatic display of D and R frames from the
 video for OCR quality control checks. When there are no concerns about OCR
 reliability (true for me nearly all the time), it can be annoying to have to close the
-frames all the time.
 
+frames all the time.
 •
 
 The BIG change is the addition of a penumbral curve fit procedure. It's a bit
-
-fiddly, so I included a test lightcurve with the download. I can't give you a
+fiddly, so I included a test lightcurve with the download. I can't give you a
 specific location for the file because it depends on details of your particular
 installation. Find where it is by searching for example-penumbral.csv When
 you find it, copy or move it to some other folder because if you process it where
 it resides, other files will get added in your installation directory --- we really don't
 want extraneous non-program files floating around in your installation directory.
 To learn how to use the new procedure (which is a bit 'fiddly'), right-click on the
 penumbral fit checkbox --- be patient; play around.
+
 version 3.4.0
 • Adds the ability to specify a diffraction lightcurve for use in timing the event. A
 new panel with edit boxes for asteroid/occulting body distance (in AU --astronomical units) and asteroid/shadow speed (in km per second) has been
 added. These values are needed in order to calculate a diffraction light curve.
 In addition to modeling diffraction effects, one can add the effect of a finite star
 disk to produce a penumbral curve. NOTE: PyOTE does not yet have the ability
 to correctly analyze a penumbral curve where it takes more than 1 or 2 readings
@@ -1091,19 +1086,19 @@
 this manner as well as .fits files inside a FITS folder.
 If this button is disabled, it is because the .csv file did not come from PyMovie or
 Limovie or simply cannot be found/opened.
 This feature can/should be used as a final quality control check for a video that
 contains timestamps extracted using OCR. It is possible for OCR to fail in manner that
 is not detected by PyOTE because the program only verifies that there is a consistent
 step (delta time) between frames. If a high order digit in the timestamp has been
-consistently misread, substituting a 8 for a 9 in the minutes field for example, the steps
+
+consistently misread, substituting a 8 for a 9 in the minutes field for example, the steps
 can be consistent while the reported time of the event will be seriously in error.
 ALL time reporting is derived from the timestamp(s) associated with D and/or R (the
-
-integer values, not the sub-frame values). If those timestamps are correct, the reported
+integer values, not the sub-frame values). If those timestamps are correct, the reported
 times will be correct even when there may be a few missing or duplicated frames. So
 best practice is to enter the D frame value in the spin box and visually confirm that the
 timestamp that you can see is the same as that extracted by the OCR procedure.
 Repeat for R.
 Another use for this feature is to handle the case where there is a visual timestamp, but
 either OCR was not activated during the .csv preparation, or the timestamp overlay
 came from an unsupported VTI type. The workflow would be to let PyOTE find the D
@@ -1131,19 +1126,19 @@
 the size (duration) extracted from the actual observation, but with only correlated
 noise in the sample (the number of points in this sample is equal to the number
 of points used in the lightcurve extraction). 50,000 attempts are made to find
 the deepest event that appears (falsely) when there is only noise being
 analyzed. If the drop from the actual observation is greater than the maximum
 size of a 'false drop', we have some assurance that the event extracted from the
 actual observation did not happen 'by chance'.
-version 3.2.9
+
+version 3.2.9
 • Changed main plot so that the scroll wheel only zooms the x axis.
 • Changed lightcurve plot so that it conforms properly to 'start-of-exposure'.
-
-version 3.2.8
+version 3.2.8
 • Changed font size in help files --- it was fine for Mac but too big for Win10
 version 3.2.7
 • Removed the 'hover-for-help' and replaced it with a 'right-click-on-item' to get
 help. This scheme was introduced in PyMovie and I found it easier to use than
 the 'hover' scheme. In practice, the 'hover' popped up when it was not needed,
 so most users eventually disabled it. As a result, it became so tedious to look at
 help --- enable hover; hover; read; disable hover --- that the help system was
@@ -1175,20 +1170,19 @@
 LC3 == LC4 whenever there was an actual LC4. It was correct in the lightcurves
 themselves, so no observation analyses have been affected by this bug. It was
 cosmetic only.
 •
 
 Added support for the PyMovie csv format
 
-version 3.2.1
+version 3.2.1
 • this version makes PyOTE more robust to a common 'cockpit error' that users
 have been making with Tangra files. Specifically, if a Tangra csv file is opened
 in a spreadsheet program, then saved from that spreadsheet program, the
-
-original csv file gets modified and overwritten by the addition of empty fields at
+original csv file gets modified and overwritten by the addition of empty fields at
 every row sufficient to match the number of columns in the longest
 header/comment row --- the spreadsheet program did this to satisfy its internal
 requirement that every row have an equal number of columns. The result is
 superfluous commas at the end of data lines (that Tangra did NOT put there).
 Until this version, that 'butchered' file could not be read. This version adds code
 to parse data lines only up to the first non-empty column. Hopefully this will not
 have ramifications in the future (like a format change that has empty fields
@@ -1218,20 +1212,20 @@
 Also trapped is the case where a user has entered a custom frame time but failed to click the
 radio button indicating that it is to be used.
 version 3.1.5:
 • Added additional tests of candidate solutions against a straight line so that there
 should always be agreement between a solution found by a min/max event size
 search and a marked D and R region search of the same area.
 Previously it was possible for the min/max search, which searches the entire
-light curve, to be tripped up by what we call a 'competitor'. A 'competitor' is an
+
+light curve, to be tripped up by what we call a 'competitor'. A 'competitor' is an
 'event' with good statistics. However, that 'competitor' may have a small
 magDrop and so later be rejected when we compare with a straight line solution.
 That 'competitor' would thus mask an event with slightly worse statistics but a
-
-larger magDrop. The change was to test every candidate against a straight line
+larger magDrop. The change was to test every candidate against a straight line
 during the search. This does make the search time longer, but not too much
 longer.
 version 3.1.4:
 • Fixed error in new dropped reading detection logic when light curve was
 processed in field mode.
 •
 
@@ -1270,23 +1264,23 @@
 artificially constrained and thus be wrong. This situation is now detected and a
 log entry as well as a pop-up alert will tell the user to change the limits and try
 again.
 •
 
 Three magDrop values are now calculated for each confidence level: the largest
 magDrop calculated using B + err(B) along with A – err(A); the nominal
-magDrop calculated using B and A; the minimum magDrop calculated using
-B – err(b) along with A + err(A)
 
+magDrop calculated using B and A; the minimum magDrop calculated using
+B – err(b) along with A + err(A)
 •
 
 The labels on the Find Event button and the Calc Err Bar button were changed
-
-to more clearly suggest that after finding an 'event', one should then press the
+to more clearly suggest that after finding an 'event', one should then press the
 'report' button to the right in order to complete the process.
+
 version 3.1.0:
 • Added a Mac version of a pyote startup file. It is automatically placed on the
 Desktop the first time pyote is run. Double-clicking on that Desktop file icon will
 start pyote thereafter.
 version 3.0.8:
 • Added a Windows batch file to the distribution that, when executed, will startup
 pyote. The file is called PYOTE.bat and is automatically copied to
@@ -1313,24 +1307,24 @@
 block integration analysis, it seems intuitive to disable the Accept integration
 button at that time as well.
 version 2.1.5:
 • Disable the Accept integration button when user overrides an automatic block
 analysis with a manual block selection followed by a click on the Block integrate
 button.
 version 2.1.4:
-• Corrected a bug that kept manual selection of block integration from being
-performed after a refusal to accept the automatic block analysis results.
-version 2.1.3:
 
 •
 
-A minor change to how color bars are plotted when the automatic block
+Corrected a bug that kept manual selection of block integration from being
+performed after a refusal to accept the automatic block analysis results.
+
+version 2.1.3:
+• A minor change to how color bars are plotted when the automatic block
 integration feature is employed. The edges now appear between data points so
 the bands are easier to see, particularly for 2 point block sizes.
-
 version 2.1.2:
 • To ease usage of the automatic block integration feature, accepting the
 automatically determined block integration parameters no longer uses a modal
 query box, which interfered with the ability to explore/expand the light curve plot.
 Now there is separate button which gets enabled after an automatic block
 integration completes.
 version 2.1.1
@@ -1360,23 +1354,23 @@
 timed with LED flashes from iPhones (John Grismore's AstroFlashTimer) or Android
 phones (Eric Couto's Occult Flash) rather than VTI timestamped files
 •
 •
 
 Adds a button to calculate the edge position of an LED timing flash.
 Adds a checkbox to enable/disable the tooltip messages that appear when a
-control is hovered over. Tooltip display defaults to 'enabled' because tooltips are
-an important aid for guiding users initially. Later, when such help is no longer
-needed, the user can turn them off (they are annoying when you don't need
-them).
 
 •
 •
 •
 
+control is hovered over. Tooltip display defaults to 'enabled' because tooltips are
+an important aid for guiding users initially. Later, when such help is no longer
+needed, the user can turn them off (they are annoying when you don't need
+them).
 Adds the ability to select which light curve is to be analyzed. Previous versions
 would only analyze the first light curve for D and R events. This flexibility is
 useful in general, but was particularly needed to support LED flash timing.
 Adds a checkbox to force manual entry of timestamp info. This is useful when
 OCR on a VTI timed light curve has catastrophic errors. It is always employed
 when using LED flash timing.
 During the error bar calculation, it is possible for the Cholesky decomposition
@@ -1408,20 +1402,21 @@
 available for calculation of correlated noise coefficients. When fewer than 14
 points are available, the correlation coefficients are set to: [1, 0, …] (i.e.,
 coefficients are set to 'no correlated noise')
 version 2.0.2
 • Note: this version has many significant changes. If you lose confidence in this
 version, remember that you can always go back to version 1.47 by typing --pip install pyote==1.47
 in an Anaconda console. (Be sure to use double == signs in the command.)
-•
+
+•
 
 improved handling of D and R region selection so that one cannot enter an
 invalid configuration --- automatic corrections/changes are applied.
 
-•
+•
 
 incorporates a new 'solver' that no longer requires an initial estimation of
 baseline noise. This 'solver' is also much faster. With this 'solver', the two-pass
 modification added in version 1.46 is no longer needed.
 
 •
```

### Comparing `pyote-5.3.6/src/pyoteapp/pyote.py` & `pyote-5.3.7/src/pyoteapp/pyote.py`

 * *Files 0% similar despite different names*

```diff
@@ -4856,16 +4856,16 @@
                           f'so there is no fit metrics file to remove.')
             return
 
         lightCurveDir = os.path.dirname(self.csvFilePath)  # This gets the folder where the light-curve.csv is located
         metric_file_path = os.path.join(lightCurveDir, 'fit_metrics.txt')
         if os.path.exists(metric_file_path):
             os.remove(metric_file_path)
-            self.showInfo(f'The fit metrics file has been cleared.')
-        return
+            self.showInfo(f'The fit metrics file has been restarted.')
+            self.addSourceFileToFitMetricTxtFile()
 
     def renameFitMetricFile(self):
         if self.csvFilePath is None:
             self.showInfo('No lightcurve file selected yet.')
             return
 
         lightCurveDir = os.path.dirname(self.csvFilePath)
@@ -7259,14 +7259,34 @@
         self.showMsg("")
 
         self.updateFitMetricTxtFile()
 
         if error_bar_plots_available:
             self.showHelp(self.helpLabelForFalsePositive)
 
+    def addSourceFileToFitMetricTxtFile(self):
+        lightCurveDir = os.path.dirname(self.csvFilePath)  # This gets the folder where the light-curve.csv is located
+        metric_file_path = os.path.join(lightCurveDir, 'fit_metrics.txt')
+
+        if os.path.exists(metric_file_path):
+            # We will append the new metric_file_path to an existing fit_metric.csv file
+            pass
+        else:
+            # Here we will create a new fit_metric.csv file' with a header line
+            with open(metric_file_path, 'w') as fileObject:
+                fileObject.writelines('aperture name,time err +/-secs,DNR,FP metric,magDrop,'
+                                      'percent drop,duration (secs),D time,'
+                                      'R time,D frame,R frame,B,A,sigmaB,sigmaA,'
+                                      'observed drop,FP drop,FP margin\n')
+
+        with open(metric_file_path, 'a') as fileObject:
+            fileObject.writelines(f'\n')
+            fileObject.writelines(f'Source file is {metric_file_path}\n')
+            fileObject.writelines(f'\n')
+
     def updateFitMetricTxtFile(self):
         lightCurveDir = os.path.dirname(self.csvFilePath)  # This gets the folder where the light-curve.csv is located
         metric_file_path = os.path.join(lightCurveDir, 'fit_metrics.txt')
 
         if os.path.exists(metric_file_path):
             # self.showInfo('We will append to an existing fit_metric.csv file')
             pass
@@ -9010,15 +9030,15 @@
                 "Csv files (*.csv)")
         else:
             self.csvFilePath = self.externalCsvFilePath
             self.externalCsvFilePath = None
 
         if self.csvFilePath:
             self.targetKey = ''
-            # self.clearFitMetricTxtFile()
+            self.addSourceFileToFitMetricTxtFile()
             self.firstLightCurveDisplayed = False
             self.availableLightCurvesForDisplay = []
             self.curveSelectionComboBox.clear()
 
             # These are used to (try to) avoid exception when a new file is read while a reference curve is active
             self.smoothingIntervalSpinBox.setValue(0)
             self.yRefStar = []
```

### Comparing `pyote-5.3.6/src/pyoteapp/pyote_modelling_utility_functions.py` & `pyote-5.3.7/src/pyoteapp/pyote_modelling_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/showVideoFrames.py` & `pyote-5.3.7/src/pyoteapp/showVideoFrames.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/solverUtils.py` & `pyote-5.3.7/src/pyoteapp/solverUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/subframe_timing_utilities.py` & `pyote-5.3.7/src/pyoteapp/subframe_timing_utilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/timestampDialog.py` & `pyote-5.3.7/src/pyoteapp/timestampDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.6/src/pyoteapp/timestampUtils.py` & `pyote-5.3.7/src/pyoteapp/timestampUtils.py`

 * *Files identical despite different names*

