# Comparing `tmp/tensorflow-ml-1.1.2.tar.gz` & `tmp/tensorflow-ml-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow-ml-1.1.2.tar", last modified: Sun Aug  6 22:39:36 2023, max compression
+gzip compressed data, was "tensorflow-ml-1.1.3.tar", last modified: Mon Aug  7 09:20:10 2023, max compression
```

## Comparing `tensorflow-ml-1.1.2.tar` & `tensorflow-ml-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:39:36.160218 tensorflow-ml-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-06 22:37:39.000000 tensorflow-ml-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-08-06 22:39:36.160218 tensorflow-ml-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-08-06 22:37:39.000000 tensorflow-ml-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 22:39:36.160218 tensorflow-ml-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-06 22:37:39.000000 tensorflow-ml-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:39:36.160218 tensorflow-ml-1.1.2/tensorflow_ml/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-06 22:37:39.000000 tensorflow-ml-1.1.2/tensorflow_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:39:36.160218 tensorflow-ml-1.1.2/tensorflow_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-08-06 22:39:36.000000 tensorflow-ml-1.1.2/tensorflow_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-06 22:39:36.000000 tensorflow-ml-1.1.2/tensorflow_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 22:39:36.000000 tensorflow-ml-1.1.2/tensorflow_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-06 22:39:36.000000 tensorflow-ml-1.1.2/tensorflow_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-06 22:39:36.000000 tensorflow-ml-1.1.2/tensorflow_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.708810 tensorflow-ml-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-08-07 09:20:10.708810 tensorflow-ml-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:20:10.708810 tensorflow-ml-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.700810 tensorflow-ml-1.1.3/tensorflow_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.700810 tensorflow-ml-1.1.3/tensorflow_ml/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15715 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20472 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/logistic_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.704810 tensorflow-ml-1.1.3/tensorflow_ml/classification/naive_bayes/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/naive_bayes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/naive_bayes/bernoulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/classification/naive_bayes/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.708810 tensorflow-ml-1.1.3/tensorflow_ml/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/regression/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/regression/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/regression/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-08-07 09:17:51.000000 tensorflow-ml-1.1.3/tensorflow_ml/regression/ridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:20:10.700810 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-08-07 09:20:10.000000 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-07 09:20:10.000000 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:20:10.000000 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-07 09:20:10.000000 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 09:20:10.000000 tensorflow-ml-1.1.3/tensorflow_ml.egg-info/top_level.txt
```

### Comparing `tensorflow-ml-1.1.2/LICENSE` & `tensorflow-ml-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.1.2/PKG-INFO` & `tensorflow-ml-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: tensorflow-ml
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tensorflow ML
 Author: Siddhant Pathak
 Author-email: siddhantpathak2@gmail.com
 Keywords: python,tensorflow,ml,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tensorflow-ml
 
 ![Keras](https://img.shields.io/badge/Keras-FF0000?style=for-the-badge&logo=keras&logoColor=white) ![Tensorflow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white) ![PyPI](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white) ![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue) ![Dependabot](https://img.shields.io/badge/dependabot-025E8C?style=for-the-badge&logo=dependabot&logoColor=white)
 
-[![Upload Python Package](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml)
+[![Upload Python Package](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml) [![docs](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/pages/pages-build-deployment)
+
 
 ## Introduction
 
 TensorFlow ML is a project that aims to provide an abstract implementation of commonly used machine learning algorithms using TensorFlow, without relying on external libraries like scikit-learn. This project is designed to offer a comprehensive and flexible set of machine learning models that can be used for various tasks, such as classification, regression, clustering, and more.
 
 The TensorFlow ML project is useful for several reasons and can overcome the needs of scikit-learn in various scenarios:
```

### Comparing `tensorflow-ml-1.1.2/README.md` & `tensorflow-ml-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # tensorflow-ml
 
 ![Keras](https://img.shields.io/badge/Keras-FF0000?style=for-the-badge&logo=keras&logoColor=white) ![Tensorflow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white) ![PyPI](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white) ![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue) ![Dependabot](https://img.shields.io/badge/dependabot-025E8C?style=for-the-badge&logo=dependabot&logoColor=white)
 
-[![Upload Python Package](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml)
+[![Upload Python Package](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml) [![docs](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/pages/pages-build-deployment)
+
 
 ## Introduction
 
 TensorFlow ML is a project that aims to provide an abstract implementation of commonly used machine learning algorithms using TensorFlow, without relying on external libraries like scikit-learn. This project is designed to offer a comprehensive and flexible set of machine learning models that can be used for various tasks, such as classification, regression, clustering, and more.
 
 The TensorFlow ML project is useful for several reasons and can overcome the needs of scikit-learn in various scenarios:
```

### Comparing `tensorflow-ml-1.1.2/setup.py` & `tensorflow-ml-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '1.1.2' 
+VERSION = '1.1.3' 
 
 DESCRIPTION = 'Tensorflow ML'
 
 with open("README.md", 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 lib_folder = os.path.dirname(os.path.realpath(__file__))
```

### Comparing `tensorflow-ml-1.1.2/tensorflow_ml.egg-info/PKG-INFO` & `tensorflow-ml-1.1.3/tensorflow_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: tensorflow-ml
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tensorflow ML
 Author: Siddhant Pathak
 Author-email: siddhantpathak2@gmail.com
 Keywords: python,tensorflow,ml,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tensorflow-ml
 
 ![Keras](https://img.shields.io/badge/Keras-FF0000?style=for-the-badge&logo=keras&logoColor=white) ![Tensorflow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white) ![PyPI](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white) ![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue) ![Dependabot](https://img.shields.io/badge/dependabot-025E8C?style=for-the-badge&logo=dependabot&logoColor=white)
 
-[![Upload Python Package](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml)
+[![Upload Python Package](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml/badge.svg?branch=main)](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/python-publish.yml) [![docs](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/siddhantpathakk/tensorflow-ml/actions/workflows/pages/pages-build-deployment)
+
 
 ## Introduction
 
 TensorFlow ML is a project that aims to provide an abstract implementation of commonly used machine learning algorithms using TensorFlow, without relying on external libraries like scikit-learn. This project is designed to offer a comprehensive and flexible set of machine learning models that can be used for various tasks, such as classification, regression, clustering, and more.
 
 The TensorFlow ML project is useful for several reasons and can overcome the needs of scikit-learn in various scenarios:
```

### Comparing `tensorflow-ml-1.1.2/tensorflow_ml.egg-info/requires.txt` & `tensorflow-ml-1.1.3/tensorflow_ml.egg-info/requires.txt`

 * *Files identical despite different names*

