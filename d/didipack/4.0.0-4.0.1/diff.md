# Comparing `tmp/didipack-4.0.0.tar.gz` & `tmp/didipack-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "didipack-4.0.0.tar", last modified: Mon Aug  7 04:56:15 2023, max compression
+gzip compressed data, was "didipack-4.0.1.tar", last modified: Mon Aug  7 04:58:59 2023, max compression
```

## Comparing `didipack-4.0.0.tar` & `didipack-4.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:56:15.826395 didipack-4.0.0/
--rw-r--r--   0 adidishe   (503) staff       (20)     1061 2020-05-30 14:27:33.000000 didipack-4.0.0/LICENSE.txt
--rw-r--r--   0 adidishe   (503) staff       (20)      853 2023-08-07 04:56:15.826686 didipack-4.0.0/PKG-INFO
--rw-r--r--   0 adidishe   (503) staff       (20)     1055 2021-02-13 12:52:32.000000 didipack-4.0.0/README.md
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:56:15.821482 didipack-4.0.0/create_rf/
--rwxr--r--   0 adidishe   (503) staff       (20)    20378 2023-08-03 03:16:13.000000 didipack-4.0.0/create_rf/RandomFeaturesGenerator.py
--rw-r--r--   0 adidishe   (503) staff       (20)      174 2023-08-07 04:25:53.000000 didipack-4.0.0/create_rf/__init__.py
--rw-r--r--   0 adidishe   (503) staff       (20)      984 2023-01-30 08:07:41.000000 didipack-4.0.0/create_rf/aux.py
--rw-r--r--   0 adidishe   (503) staff       (20)     5223 2023-08-03 02:18:39.000000 didipack-4.0.0/create_rf/gen_rf_factors.py
--rw-r--r--   0 adidishe   (503) staff       (20)     4431 2023-01-30 11:02:36.000000 didipack-4.0.0/create_rf/pre_process_130.py
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:56:15.823164 didipack-4.0.0/didipack/
--rw-r--r--   0 adidishe   (503) staff       (20)      184 2023-08-07 04:46:58.000000 didipack-4.0.0/didipack/__init__.py
--rw-r--r--   0 adidishe   (503) staff       (20)     5707 2021-06-23 07:26:52.000000 didipack-4.0.0/didipack/latex_paper.py
--rw-r--r--   0 adidishe   (503) staff       (20)    18383 2021-02-12 21:49:54.000000 didipack-4.0.0/didipack/latex_ressource.py
--rw-r--r--   0 adidishe   (503) staff       (20)    10138 2023-08-07 04:10:35.000000 didipack-4.0.0/didipack/latex_table.py
--rw-r--r--   0 adidishe   (503) staff       (20)     5122 2023-08-07 04:46:58.000000 didipack-4.0.0/didipack/parameters.py
--rw-r--r--   0 adidishe   (503) staff       (20)      610 2021-02-13 11:17:35.000000 didipack-4.0.0/didipack/plot_function.py
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:56:15.823944 didipack-4.0.0/didipack.egg-info/
--rw-r--r--   0 adidishe   (503) staff       (20)      853 2023-08-07 04:56:15.000000 didipack-4.0.0/didipack.egg-info/PKG-INFO
--rw-r--r--   0 adidishe   (503) staff       (20)      684 2023-08-07 04:56:15.000000 didipack-4.0.0/didipack.egg-info/SOURCES.txt
--rw-r--r--   0 adidishe   (503) staff       (20)        1 2023-08-07 04:56:15.000000 didipack-4.0.0/didipack.egg-info/dependency_links.txt
--rw-r--r--   0 adidishe   (503) staff       (20)       48 2023-08-07 04:56:15.000000 didipack-4.0.0/didipack.egg-info/requires.txt
--rw-r--r--   0 adidishe   (503) staff       (20)       33 2023-08-07 04:56:15.000000 didipack-4.0.0/didipack.egg-info/top_level.txt
--rw-r--r--   0 adidishe   (503) staff       (20)       79 2023-08-07 04:56:15.827000 didipack-4.0.0/setup.cfg
--rw-r--r--   0 adidishe   (503) staff       (20)     1325 2023-08-07 04:54:41.000000 didipack-4.0.0/setup.py
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:56:15.824752 didipack-4.0.0/trainer/
--rw-r--r--   0 adidishe   (503) staff       (20)        2 2023-08-07 04:44:31.000000 didipack-4.0.0/trainer/__init__.py
--rw-r--r--   0 adidishe   (503) staff       (20)     5571 2023-08-07 04:46:58.000000 didipack-4.0.0/trainer/train_splitter.py
--rw-r--r--   0 adidishe   (503) staff       (20)     3622 2023-08-07 04:46:58.000000 didipack-4.0.0/trainer/trainer_abstract.py
--rw-r--r--   0 adidishe   (503) staff       (20)     1924 2023-08-07 04:46:58.000000 didipack-4.0.0/trainer/trainer_ridge.py
-drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:56:15.826094 didipack-4.0.0/utils/
--rw-r--r--   0 adidishe   (503) staff       (20)        2 2023-08-07 04:44:31.000000 didipack-4.0.0/utils/__init__.py
--rw-r--r--   0 adidishe   (503) staff       (20)     1585 2023-08-07 04:48:13.000000 didipack-4.0.0/utils/general.py
--rw-r--r--   0 adidishe   (503) staff       (20)     1230 2023-08-07 04:48:13.000000 didipack-4.0.0/utils/pandasplus.py
--rw-r--r--   0 adidishe   (503) staff       (20)      772 2023-07-21 00:00:42.000000 didipack-4.0.0/utils/plot.py
--rw-r--r--   0 adidishe   (503) staff       (20)     3694 2023-08-01 04:41:03.000000 didipack-4.0.0/utils/ridge.py
--rw-r--r--   0 adidishe   (503) staff       (20)      837 2023-01-31 16:53:40.000000 didipack-4.0.0/utils/smart_algebra.py
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:58:59.453517 didipack-4.0.1/
+-rw-r--r--   0 adidishe   (503) staff       (20)     1061 2020-05-30 14:27:33.000000 didipack-4.0.1/LICENSE.txt
+-rw-r--r--   0 adidishe   (503) staff       (20)      853 2023-08-07 04:58:59.453582 didipack-4.0.1/PKG-INFO
+-rw-r--r--   0 adidishe   (503) staff       (20)     1055 2021-02-13 12:52:32.000000 didipack-4.0.1/README.md
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:58:59.448851 didipack-4.0.1/create_rf/
+-rwxr--r--   0 adidishe   (503) staff       (20)    20378 2023-08-03 03:16:13.000000 didipack-4.0.1/create_rf/RandomFeaturesGenerator.py
+-rw-r--r--   0 adidishe   (503) staff       (20)      174 2023-08-07 04:25:53.000000 didipack-4.0.1/create_rf/__init__.py
+-rw-r--r--   0 adidishe   (503) staff       (20)      984 2023-01-30 08:07:41.000000 didipack-4.0.1/create_rf/aux.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     5223 2023-08-03 02:18:39.000000 didipack-4.0.1/create_rf/gen_rf_factors.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     4431 2023-01-30 11:02:36.000000 didipack-4.0.1/create_rf/pre_process_130.py
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:58:59.450699 didipack-4.0.1/didipack/
+-rw-r--r--   0 adidishe   (503) staff       (20)      184 2023-08-07 04:46:58.000000 didipack-4.0.1/didipack/__init__.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     5707 2021-06-23 07:26:52.000000 didipack-4.0.1/didipack/latex_paper.py
+-rw-r--r--   0 adidishe   (503) staff       (20)    18383 2021-02-12 21:49:54.000000 didipack-4.0.1/didipack/latex_ressource.py
+-rw-r--r--   0 adidishe   (503) staff       (20)    10138 2023-08-07 04:10:35.000000 didipack-4.0.1/didipack/latex_table.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     5122 2023-08-07 04:46:58.000000 didipack-4.0.1/didipack/parameters.py
+-rw-r--r--   0 adidishe   (503) staff       (20)      610 2021-02-13 11:17:35.000000 didipack-4.0.1/didipack/plot_function.py
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:58:59.451511 didipack-4.0.1/didipack.egg-info/
+-rw-r--r--   0 adidishe   (503) staff       (20)      853 2023-08-07 04:58:59.000000 didipack-4.0.1/didipack.egg-info/PKG-INFO
+-rw-r--r--   0 adidishe   (503) staff       (20)      684 2023-08-07 04:58:59.000000 didipack-4.0.1/didipack.egg-info/SOURCES.txt
+-rw-r--r--   0 adidishe   (503) staff       (20)        1 2023-08-07 04:58:59.000000 didipack-4.0.1/didipack.egg-info/dependency_links.txt
+-rw-r--r--   0 adidishe   (503) staff       (20)       48 2023-08-07 04:58:59.000000 didipack-4.0.1/didipack.egg-info/requires.txt
+-rw-r--r--   0 adidishe   (503) staff       (20)       33 2023-08-07 04:58:59.000000 didipack-4.0.1/didipack.egg-info/top_level.txt
+-rw-r--r--   0 adidishe   (503) staff       (20)       79 2023-08-07 04:58:59.453794 didipack-4.0.1/setup.cfg
+-rw-r--r--   0 adidishe   (503) staff       (20)     1325 2023-08-07 04:58:40.000000 didipack-4.0.1/setup.py
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:58:59.452258 didipack-4.0.1/trainer/
+-rw-r--r--   0 adidishe   (503) staff       (20)        2 2023-08-07 04:44:31.000000 didipack-4.0.1/trainer/__init__.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     5571 2023-08-07 04:46:58.000000 didipack-4.0.1/trainer/train_splitter.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     3622 2023-08-07 04:46:58.000000 didipack-4.0.1/trainer/trainer_abstract.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     1924 2023-08-07 04:46:58.000000 didipack-4.0.1/trainer/trainer_ridge.py
+drwxr-xr-x   0 adidishe   (503) staff       (20)        0 2023-08-07 04:58:59.453377 didipack-4.0.1/utils/
+-rw-r--r--   0 adidishe   (503) staff       (20)       52 2023-08-07 04:58:40.000000 didipack-4.0.1/utils/__init__.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     1585 2023-08-07 04:48:13.000000 didipack-4.0.1/utils/general.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     1230 2023-08-07 04:48:13.000000 didipack-4.0.1/utils/pandasplus.py
+-rw-r--r--   0 adidishe   (503) staff       (20)      772 2023-07-21 00:00:42.000000 didipack-4.0.1/utils/plot.py
+-rw-r--r--   0 adidishe   (503) staff       (20)     3694 2023-08-01 04:41:03.000000 didipack-4.0.1/utils/ridge.py
+-rw-r--r--   0 adidishe   (503) staff       (20)      837 2023-01-31 16:53:40.000000 didipack-4.0.1/utils/smart_algebra.py
```

### Comparing `didipack-4.0.0/LICENSE.txt` & `didipack-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/PKG-INFO` & `didipack-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didipack
-Version: 4.0.0
+Version: 4.0.1
 Summary: Usefull time saver for data-science and finance with python
 Home-page: https://github.com/AntoineDidisheim
 Author: Antoine Didisheim
 Author-email: antoinedidisheim@gmail.com
 License: MIT
 Download-URL: https://github.com/AntoineDidisheim/didipack/archive/v0.1.1.tar.gz
 Keywords: LaTex,Finance
```

### Comparing `didipack-4.0.0/README.md` & `didipack-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/create_rf/RandomFeaturesGenerator.py` & `didipack-4.0.1/create_rf/RandomFeaturesGenerator.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/create_rf/aux.py` & `didipack-4.0.1/create_rf/aux.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/create_rf/gen_rf_factors.py` & `didipack-4.0.1/create_rf/gen_rf_factors.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/create_rf/pre_process_130.py` & `didipack-4.0.1/create_rf/pre_process_130.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/didipack/latex_paper.py` & `didipack-4.0.1/didipack/latex_paper.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/didipack/latex_ressource.py` & `didipack-4.0.1/didipack/latex_ressource.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/didipack/latex_table.py` & `didipack-4.0.1/didipack/latex_table.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/didipack/parameters.py` & `didipack-4.0.1/didipack/parameters.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/didipack/plot_function.py` & `didipack-4.0.1/didipack/plot_function.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/didipack.egg-info/PKG-INFO` & `didipack-4.0.1/didipack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didipack
-Version: 4.0.0
+Version: 4.0.1
 Summary: Usefull time saver for data-science and finance with python
 Home-page: https://github.com/AntoineDidisheim
 Author: Antoine Didisheim
 Author-email: antoinedidisheim@gmail.com
 License: MIT
 Download-URL: https://github.com/AntoineDidisheim/didipack/archive/v0.1.1.tar.gz
 Keywords: LaTex,Finance
```

### Comparing `didipack-4.0.0/didipack.egg-info/SOURCES.txt` & `didipack-4.0.1/didipack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/setup.py` & `didipack-4.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='didipack',
     packages=setuptools.find_packages(),  # Automatically discover and include all packages in the package directory
-    version='4.0.0',
+    version='4.0.1',
     license='MIT',
     setup_requires=['wheel'],
     description='Usefull time saver for data-science and finance with python',
     author='Antoine Didisheim',
     author_email='antoinedidisheim@gmail.com',
     url='https://github.com/AntoineDidisheim',
     download_url='https://github.com/AntoineDidisheim/didipack/archive/v0.1.1.tar.gz',
```

### Comparing `didipack-4.0.0/trainer/train_splitter.py` & `didipack-4.0.1/trainer/train_splitter.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/trainer/trainer_abstract.py` & `didipack-4.0.1/trainer/trainer_abstract.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/trainer/trainer_ridge.py` & `didipack-4.0.1/trainer/trainer_ridge.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/utils/general.py` & `didipack-4.0.1/utils/general.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/utils/pandasplus.py` & `didipack-4.0.1/utils/pandasplus.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/utils/plot.py` & `didipack-4.0.1/utils/plot.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/utils/ridge.py` & `didipack-4.0.1/utils/ridge.py`

 * *Files identical despite different names*

### Comparing `didipack-4.0.0/utils/smart_algebra.py` & `didipack-4.0.1/utils/smart_algebra.py`

 * *Files identical despite different names*

