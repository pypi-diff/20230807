# Comparing `tmp/composipy-1.0.2.tar.gz` & `tmp/composipy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composipy-1.0.2.tar", last modified: Sat May  6 17:07:07 2023, max compression
+gzip compressed data, was "composipy-1.1.0.tar", last modified: Sun Aug  6 22:39:42 2023, max compression
```

## Comparing `composipy-1.0.2.tar` & `composipy-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.984605 composipy-1.0.2/
--rw-rw-rw-   0        0        0     1092 2023-05-05 22:53:36.000000 composipy-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4021 2023-05-06 17:07:07.984605 composipy-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3532 2023-05-05 22:53:36.000000 composipy-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.949596 composipy-1.0.2/composipy/
--rw-rw-rw-   0        0        0      213 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.968600 composipy-1.0.2/composipy/core/
--rw-rw-rw-   0        0        0        0 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/core/__init__.py
--rw-rw-rw-   0        0        0     9276 2023-05-06 16:51:15.000000 composipy-1.0.2/composipy/core/material.py
--rw-rw-rw-   0        0        0     9433 2023-05-06 16:55:57.000000 composipy-1.0.2/composipy/core/property.py
--rw-rw-rw-   0        0        0    13254 2023-05-06 00:02:25.000000 composipy-1.0.2/composipy/core/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.969601 composipy-1.0.2/composipy/nastranapi/
--rw-rw-rw-   0        0        0       58 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/nastranapi/__init__.py
--rw-rw-rw-   0        0        0     6325 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/nastranapi/pcomp_generator.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.978603 composipy-1.0.2/composipy/pre_integrated_component/
--rw-rw-rw-   0        0        0  2270468 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/_S.py
--rw-rw-rw-   0        0        0        0 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/__init__.py
--rw-rw-rw-   0        0        0   119327 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/_ii_F.py
--rw-rw-rw-   0        0        0     6377 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/build_k.py
--rw-rw-rw-   0        0        0     1203 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/functions.py
--rw-rw-rw-   0        0        0     3552 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/write_pre_integrated_terms.py
--rw-rw-rw-   0        0        0     2340 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/write_shape_function.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.979604 composipy-1.0.2/composipy/utils/
--rw-rw-rw-   0        0        0       42 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/utils/__init__.py
--rw-rw-rw-   0        0        0     1283 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/utils/validators.py
--rw-rw-rw-   0        0        0       21 2023-05-06 12:05:21.000000 composipy-1.0.2/composipy/version.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.964600 composipy-1.0.2/composipy.egg-info/
--rw-rw-rw-   0        0        0     4021 2023-05-06 17:07:07.000000 composipy-1.0.2/composipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      964 2023-05-06 17:07:07.000000 composipy-1.0.2/composipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 17:07:07.000000 composipy-1.0.2/composipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-06 17:07:07.000000 composipy-1.0.2/composipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-06 17:07:07.000000 composipy-1.0.2/composipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 17:07:07.985605 composipy-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1012 2023-05-05 22:53:36.000000 composipy-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.983604 composipy-1.0.2/tests/
--rw-rw-rw-   0        0        0     1870 2023-05-05 22:53:36.000000 composipy-1.0.2/tests/test_ABD.py
--rw-rw-rw-   0        0        0      864 2023-05-05 22:53:36.000000 composipy-1.0.2/tests/test_Material_Q0.py
--rw-rw-rw-   0        0        0     1185 2023-05-05 22:53:36.000000 composipy-1.0.2/tests/test_lamination_parameters.py
--rw-rw-rw-   0        0        0     1614 2023-05-05 22:53:36.000000 composipy-1.0.2/tests/test_plate_buckling.py
--rw-rw-rw-   0        0        0     1948 2023-05-06 16:45:59.000000 composipy-1.0.2/tests/test_plate_buckling_LP.py
+drwxrwxrwx   0        0        0        0 2023-08-06 22:39:42.961478 composipy-1.1.0/
+-rw-rw-rw-   0        0        0     1092 2023-05-06 17:21:18.000000 composipy-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4117 2023-08-06 22:39:42.961478 composipy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3628 2023-07-29 16:31:56.000000 composipy-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 22:39:42.926470 composipy-1.1.0/composipy/
+-rw-rw-rw-   0        0        0      213 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 22:39:42.944474 composipy-1.1.0/composipy/core/
+-rw-rw-rw-   0        0        0        0 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/core/__init__.py
+-rw-rw-rw-   0        0        0     9276 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/core/material.py
+-rw-rw-rw-   0        0        0     9433 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/core/property.py
+-rw-rw-rw-   0        0        0    13254 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/core/structure.py
+drwxrwxrwx   0        0        0        0 2023-08-06 22:39:42.946475 composipy-1.1.0/composipy/nastranapi/
+-rw-rw-rw-   0        0        0       58 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/nastranapi/__init__.py
+-rw-rw-rw-   0        0        0     6325 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/nastranapi/pcomp_generator.py
+drwxrwxrwx   0        0        0        0 2023-08-06 22:39:42.947475 composipy-1.1.0/composipy/optimize/
+-rw-rw-rw-   0        0        0      171 2023-08-06 22:35:35.000000 composipy-1.1.0/composipy/optimize/__init__.py
+-rw-rw-rw-   0        0        0     6374 2023-08-06 22:35:35.000000 composipy-1.1.0/composipy/optimize/_maximize_buckling.py
+-rw-rw-rw-   0        0        0     6301 2023-08-06 22:35:35.000000 composipy-1.1.0/composipy/optimize/_minimize_panel_weight.py
+drwxrwxrwx   0        0        0        0 2023-08-06 22:39:42.955477 composipy-1.1.0/composipy/pre_integrated_component/
+-rw-rw-rw-   0        0        0  2270468 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/pre_integrated_component/_S.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/pre_integrated_component/__init__.py
+-rw-rw-rw-   0        0        0   119327 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/pre_integrated_component/_ii_F.py
+-rw-rw-rw-   0        0        0     6377 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/pre_integrated_component/build_k.py
+-rw-rw-rw-   0        0        0     1203 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/pre_integrated_component/functions.py
+-rw-rw-rw-   0        0        0     3552 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/pre_integrated_component/write_pre_integrated_terms.py
+-rw-rw-rw-   0        0        0     2340 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/pre_integrated_component/write_shape_function.py
+drwxrwxrwx   0        0        0        0 2023-08-06 22:39:42.956477 composipy-1.1.0/composipy/utils/
+-rw-rw-rw-   0        0        0       42 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1283 2023-05-06 17:21:18.000000 composipy-1.1.0/composipy/utils/validators.py
+-rw-rw-rw-   0        0        0       21 2023-08-06 22:35:35.000000 composipy-1.1.0/composipy/version.py
+drwxrwxrwx   0        0        0        0 2023-08-06 22:39:42.941473 composipy-1.1.0/composipy.egg-info/
+-rw-rw-rw-   0        0        0     4117 2023-08-06 22:39:42.000000 composipy-1.1.0/composipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1081 2023-08-06 22:39:42.000000 composipy-1.1.0/composipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 22:39:42.000000 composipy-1.1.0/composipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-08-06 22:39:42.000000 composipy-1.1.0/composipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 22:39:42.000000 composipy-1.1.0/composipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 22:39:42.961478 composipy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2023-05-06 17:21:18.000000 composipy-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 22:39:42.960478 composipy-1.1.0/tests/
+-rw-rw-rw-   0        0        0     1870 2023-05-06 17:21:18.000000 composipy-1.1.0/tests/test_ABD.py
+-rw-rw-rw-   0        0        0      864 2023-05-06 17:21:18.000000 composipy-1.1.0/tests/test_Material_Q0.py
+-rw-rw-rw-   0        0        0     1185 2023-05-06 17:21:18.000000 composipy-1.1.0/tests/test_lamination_parameters.py
+-rw-rw-rw-   0        0        0     1614 2023-05-06 17:21:18.000000 composipy-1.1.0/tests/test_plate_buckling.py
+-rw-rw-rw-   0        0        0     1948 2023-05-06 17:21:18.000000 composipy-1.1.0/tests/test_plate_buckling_LP.py
```

### Comparing `composipy-1.0.2/LICENSE` & `composipy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/PKG-INFO` & `composipy-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: composipy
-Version: 1.0.2
+Version: 1.1.0
 Summary: This package intends to perform composite material calculations
 Home-page: https://github.com/rafaelpsilva07/composipy
 Author: Rafael Pereira
 Author-email: rafaelpsilva07@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Downloads](https://static.pepy.tech/badge/composipy)](https://pepy.tech/project/composipy)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rafaelpsilva07/composipy/pypi.yml)
 ![PyPI](https://img.shields.io/pypi/v/composipy)
+[![DOI](https://zenodo.org/badge/332543985.svg)](https://zenodo.org/badge/latestdoi/332543985)
 
 
 # Composipy
 
 ## What it is
 
 **composipy** is a python library to calculate composite plates using the classical laminate theory. This library is designed to be simple, userfriendly and helpfull.
```

### Comparing `composipy-1.0.2/README.md` & `composipy-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [![Downloads](https://static.pepy.tech/badge/composipy)](https://pepy.tech/project/composipy)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rafaelpsilva07/composipy/pypi.yml)
 ![PyPI](https://img.shields.io/pypi/v/composipy)
+[![DOI](https://zenodo.org/badge/332543985.svg)](https://zenodo.org/badge/latestdoi/332543985)
 
 
 # Composipy
 
 ## What it is
 
 **composipy** is a python library to calculate composite plates using the classical laminate theory. This library is designed to be simple, userfriendly and helpfull.
```

### Comparing `composipy-1.0.2/composipy/core/material.py` & `composipy-1.1.0/composipy/core/material.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/composipy/core/property.py` & `composipy-1.1.0/composipy/core/property.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/composipy/core/structure.py` & `composipy-1.1.0/composipy/core/structure.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/composipy/nastranapi/pcomp_generator.py` & `composipy-1.1.0/composipy/nastranapi/pcomp_generator.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/composipy/pre_integrated_component/_S.py` & `composipy-1.1.0/composipy/pre_integrated_component/_S.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/composipy/pre_integrated_component/_ii_F.py` & `composipy-1.1.0/composipy/pre_integrated_component/_ii_F.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/composipy/pre_integrated_component/build_k.py` & `composipy-1.1.0/composipy/pre_integrated_component/build_k.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/composipy/pre_integrated_component/functions.py` & `composipy-1.1.0/composipy/pre_integrated_component/functions.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/composipy/pre_integrated_component/write_pre_integrated_terms.py` & `composipy-1.1.0/composipy/pre_integrated_component/write_pre_integrated_terms.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/composipy/pre_integrated_component/write_shape_function.py` & `composipy-1.1.0/composipy/pre_integrated_component/write_shape_function.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/composipy/utils/validators.py` & `composipy-1.1.0/composipy/utils/validators.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/composipy.egg-info/PKG-INFO` & `composipy-1.1.0/composipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: composipy
-Version: 1.0.2
+Version: 1.1.0
 Summary: This package intends to perform composite material calculations
 Home-page: https://github.com/rafaelpsilva07/composipy
 Author: Rafael Pereira
 Author-email: rafaelpsilva07@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Downloads](https://static.pepy.tech/badge/composipy)](https://pepy.tech/project/composipy)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rafaelpsilva07/composipy/pypi.yml)
 ![PyPI](https://img.shields.io/pypi/v/composipy)
+[![DOI](https://zenodo.org/badge/332543985.svg)](https://zenodo.org/badge/latestdoi/332543985)
 
 
 # Composipy
 
 ## What it is
 
 **composipy** is a python library to calculate composite plates using the classical laminate theory. This library is designed to be simple, userfriendly and helpfull.
```

### Comparing `composipy-1.0.2/composipy.egg-info/SOURCES.txt` & `composipy-1.1.0/composipy.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 composipy.egg-info/top_level.txt
 composipy/core/__init__.py
 composipy/core/material.py
 composipy/core/property.py
 composipy/core/structure.py
 composipy/nastranapi/__init__.py
 composipy/nastranapi/pcomp_generator.py
+composipy/optimize/__init__.py
+composipy/optimize/_maximize_buckling.py
+composipy/optimize/_minimize_panel_weight.py
 composipy/pre_integrated_component/_S.py
 composipy/pre_integrated_component/__init__.py
 composipy/pre_integrated_component/_ii_F.py
 composipy/pre_integrated_component/build_k.py
 composipy/pre_integrated_component/functions.py
 composipy/pre_integrated_component/write_pre_integrated_terms.py
 composipy/pre_integrated_component/write_shape_function.py
```

### Comparing `composipy-1.0.2/setup.py` & `composipy-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/tests/test_ABD.py` & `composipy-1.1.0/tests/test_ABD.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/tests/test_Material_Q0.py` & `composipy-1.1.0/tests/test_Material_Q0.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/tests/test_lamination_parameters.py` & `composipy-1.1.0/tests/test_lamination_parameters.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/tests/test_plate_buckling.py` & `composipy-1.1.0/tests/test_plate_buckling.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.2/tests/test_plate_buckling_LP.py` & `composipy-1.1.0/tests/test_plate_buckling_LP.py`

 * *Files identical despite different names*

