# Comparing `tmp/tensorflow-ml-1.1.3.tar.gz` & `tmp/tensorflow-ml-1.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow-ml-1.1.3.tar", last modified: Mon Aug  7 09:20:10 2023, max compression
+gzip compressed data, was "tensorflow-ml-1.1.3.1.tar", last modified: Mon Aug  7 10:21:48 2023, max compression
```

## Comparing `tensorflow-ml-1.1.3.tar` & `tensorflow-ml-1.1.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.708810 tensorflow-ml-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-08-07 09:20:10.708810 tensorflow-ml-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:20:10.708810 tensorflow-ml-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.700810 tensorflow-ml-1.1.3/tensorflow_ml/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.700810 tensorflow-ml-1.1.3/tensorflow_ml/classification/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15715 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    20472 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/logistic_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.704810 tensorflow-ml-1.1.3/tensorflow_ml/classification/naive_bayes/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/naive_bayes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/naive_bayes/bernoulli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/naive_bayes/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.708810 tensorflow-ml-1.1.3/tensorflow_ml/regression/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/regression/lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/regression/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/regression/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/regression/ridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.700810 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-08-07 09:20:10.000000 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-07 09:20:10.000000 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:20:10.000000 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-07 09:20:10.000000 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 09:20:10.000000 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:21:48.269519 tensorflow-ml-1.1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-08-07 10:21:48.269519 tensorflow-ml-1.1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:21:48.269519 tensorflow-ml-1.1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:21:48.265519 tensorflow-ml-1.1.3.1/tensorflow_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:21:48.265519 tensorflow-ml-1.1.3.1/tensorflow_ml/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15715 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/classification/decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20472 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/classification/logistic_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:21:48.269519 tensorflow-ml-1.1.3.1/tensorflow_ml/classification/naive_bayes/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/classification/naive_bayes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/classification/naive_bayes/bernoulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/classification/naive_bayes/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:21:48.269519 tensorflow-ml-1.1.3.1/tensorflow_ml/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/regression/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/regression/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/regression/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-08-07 10:19:55.000000 tensorflow-ml-1.1.3.1/tensorflow_ml/regression/ridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:21:48.265519 tensorflow-ml-1.1.3.1/tensorflow_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-08-07 10:21:48.000000 tensorflow-ml-1.1.3.1/tensorflow_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-07 10:21:48.000000 tensorflow-ml-1.1.3.1/tensorflow_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:21:48.000000 tensorflow-ml-1.1.3.1/tensorflow_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-07 10:21:48.000000 tensorflow-ml-1.1.3.1/tensorflow_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 10:21:48.000000 tensorflow-ml-1.1.3.1/tensorflow_ml.egg-info/top_level.txt
```

### Comparing `tensorflow-ml-1.1.3/LICENSE` & `tensorflow-ml-1.1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.3/PKG-INFO` & `tensorflow-ml-1.1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-ml
-Version: 1.1.3
+Version: 1.1.3.1
 Summary: Tensorflow ML
 Author: Siddhant Pathak
 Author-email: siddhantpathak2@gmail.com
 Keywords: python,tensorflow,ml,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `tensorflow-ml-1.1.3/README.md` & `tensorflow-ml-1.1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.3/setup.py` & `tensorflow-ml-1.1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '1.1.3' 
+VERSION = '1.1.3.1' 
 
 DESCRIPTION = 'Tensorflow ML'
 
 with open("README.md", 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 lib_folder = os.path.dirname(os.path.realpath(__file__))
```

### Comparing `tensorflow-ml-1.1.3/tensorflow_ml/classification/decision_tree.py` & `tensorflow-ml-1.1.3.1/tensorflow_ml/classification/decision_tree.py`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.3/tensorflow_ml/classification/logistic_regression.py` & `tensorflow-ml-1.1.3.1/tensorflow_ml/classification/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.3/tensorflow_ml/classification/naive_bayes/bernoulli.py` & `tensorflow-ml-1.1.3.1/tensorflow_ml/classification/naive_bayes/bernoulli.py`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.3/tensorflow_ml/classification/naive_bayes/gaussian.py` & `tensorflow-ml-1.1.3.1/tensorflow_ml/classification/naive_bayes/gaussian.py`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.3/tensorflow_ml/regression/lasso.py` & `tensorflow-ml-1.1.3.1/tensorflow_ml/regression/lasso.py`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.3/tensorflow_ml/regression/linear.py` & `tensorflow-ml-1.1.3.1/tensorflow_ml/regression/linear.py`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.3/tensorflow_ml/regression/polynomial.py` & `tensorflow-ml-1.1.3.1/tensorflow_ml/regression/polynomial.py`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.3/tensorflow_ml/regression/ridge.py` & `tensorflow-ml-1.1.3.1/tensorflow_ml/regression/ridge.py`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.3/tensorflow_ml.egg-info/PKG-INFO` & `tensorflow-ml-1.1.3.1/tensorflow_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-ml
-Version: 1.1.3
+Version: 1.1.3.1
 Summary: Tensorflow ML
 Author: Siddhant Pathak
 Author-email: siddhantpathak2@gmail.com
 Keywords: python,tensorflow,ml,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `tensorflow-ml-1.1.3/tensorflow_ml.egg-info/SOURCES.txt` & `tensorflow-ml-1.1.3.1/tensorflow_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.3/tensorflow_ml.egg-info/requires.txt` & `tensorflow-ml-1.1.3.1/tensorflow_ml.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -29,44 +29,44 @@
 contourpy==1.1.0
 cryptography==41.0.3
 cufflinks==0.17.3
 cycler==0.11.0
 Cython==3.0.0b3
 DateTime==5.1
 debugpy==1.6.7
-decorator==5.1.1
+decorator<5.0
 defusedxml==0.7.1
 deprecation==2.1.0
 dm-tree==0.1.8
 eikon==1.1.16
 entrypoints==0.4
 et-xmlfile==1.1.0
 executing==1.2.0
 fastjsonschema==2.18.0
 flatbuffers==23.5.26
 fonttools==4.25.0
 fqdn==1.5.1
 frozendict==2.3.8
 gast==0.4.0
-google-auth==2.21.0
+google-auth
 google-auth-oauthlib==1.0.0
 google-pasta==0.2.0
 grpcio==1.56.0
 h11==0.14.0
 h2==3.2.0
 h5py==3.9.0
 hpack==3.0.0
 html5lib==1.1
 httpcore==0.17.3
 httpx==0.24.1
 hyperframe==5.2.0
 idna==2.10
 inflection==0.5.1
-ipykernel==6.25.0
-ipython==8.14.0
+ipykernel
+ipython
 ipython-genutils==0.2.0
 ipywidgets==8.1.0
 isoduration==20.11.0
 jax==0.4.13
 jedi==0.19.0
 Jinja2==3.1.2
 joblib==1.3.1
@@ -101,15 +101,15 @@
 multitasking==0.0.11
 munkres==1.1.4
 nbclassic==1.0.0
 nbclient==0.8.0
 nbconvert==7.7.3
 nbformat==5.9.2
 nest-asyncio==1.5.7
-notebook==7.0.2
+notebook
 notebook_shim==0.2.3
 numexpr==2.8.4
 numpy==1.23.5
 oauthlib==3.2.2
 openpyxl==3.0.10
 opt-einsum==3.3.0
 overrides==7.3.1
@@ -121,15 +121,15 @@
 patsy==0.5.3
 pexpect==4.8.0
 pickleshare==0.7.5
 Pillow==9.4.0
 platformdirs==3.10.0
 plotly==5.15.0
 ply==3.11
-pooch==1.7.0
+pooch<1.7
 prometheus-client==0.17.1
 prompt-toolkit==3.0.39
 protobuf==4.23.3
 psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
 py-cpuinfo==9.0.0
@@ -146,15 +146,15 @@
 python-json-logger==2.0.7
 pytz==2023.3
 PyYAML==6.0.1
 pyzmq==25.1.0
 qtconsole==5.4.3
 QtPy==2.3.1
 referencing==0.30.2
-requests==2.31.0
+requests
 requests-oauthlib==1.3.1
 rfc3339-validator==0.1.4
 rfc3986==1.5.0
 rfc3986-validator==0.1.1
 rpds-py==0.9.2
 rsa==4.9
 scipy==1.11.1
```

