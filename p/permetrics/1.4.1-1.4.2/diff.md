# Comparing `tmp/permetrics-1.4.1.tar.gz` & `tmp/permetrics-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permetrics-1.4.1.tar", last modified: Fri Aug  4 04:25:06 2023, max compression
+gzip compressed data, was "permetrics-1.4.2.tar", last modified: Mon Aug  7 10:13:25 2023, max compression
```

## Comparing `permetrics-1.4.1.tar` & `permetrics-1.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:25:06.795924 permetrics-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-04 04:24:44.000000 permetrics-1.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-08-04 04:24:44.000000 permetrics-1.4.1/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 04:24:44.000000 permetrics-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-04 04:24:44.000000 permetrics-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-08-04 04:25:06.795924 permetrics-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   340278 2023-08-04 04:24:44.000000 permetrics-1.4.1/R-R2-Rsquared.docx
--rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-08-04 04:24:44.000000 permetrics-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:25:06.791924 permetrics-1.4.1/permetrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37300 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    72219 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    97099 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:25:06.795924 permetrics-1.4.1/permetrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/classifier_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/cluster_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/data_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/regressor_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:25:06.791924 permetrics-1.4.1/permetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-08-04 04:25:06.000000 permetrics-1.4.1/permetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-04 04:25:06.000000 permetrics-1.4.1/permetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 04:25:06.000000 permetrics-1.4.1/permetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-04 04:25:06.000000 permetrics-1.4.1/permetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 04:25:06.000000 permetrics-1.4.1/permetrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 04:25:06.795924 permetrics-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-08-04 04:24:44.000000 permetrics-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:25:06.795924 permetrics-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-04 04:24:44.000000 permetrics-1.4.1/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-04 04:24:44.000000 permetrics-1.4.1/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-08-04 04:24:44.000000 permetrics-1.4.1/tests/test_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:13:25.344230 permetrics-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-07 10:12:49.000000 permetrics-1.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-08-07 10:12:49.000000 permetrics-1.4.2/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 10:12:49.000000 permetrics-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-07 10:12:49.000000 permetrics-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24253 2023-08-07 10:13:25.344230 permetrics-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   340278 2023-08-07 10:12:49.000000 permetrics-1.4.2/R-R2-Rsquared.docx
+-rw-r--r--   0 runner    (1001) docker     (123)    21551 2023-08-07 10:12:49.000000 permetrics-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:13:25.344230 permetrics-1.4.2/permetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-07 10:12:49.000000 permetrics-1.4.2/permetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37315 2023-08-07 10:12:49.000000 permetrics-1.4.2/permetrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72234 2023-08-07 10:12:49.000000 permetrics-1.4.2/permetrics/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-08-07 10:12:49.000000 permetrics-1.4.2/permetrics/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97095 2023-08-07 10:12:49.000000 permetrics-1.4.2/permetrics/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:13:25.344230 permetrics-1.4.2/permetrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 10:12:49.000000 permetrics-1.4.2/permetrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-08-07 10:12:49.000000 permetrics-1.4.2/permetrics/utils/classifier_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-08-07 10:12:49.000000 permetrics-1.4.2/permetrics/utils/cluster_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-08-07 10:12:49.000000 permetrics-1.4.2/permetrics/utils/data_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-07 10:12:49.000000 permetrics-1.4.2/permetrics/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-08-07 10:12:49.000000 permetrics-1.4.2/permetrics/utils/regressor_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:13:25.344230 permetrics-1.4.2/permetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24253 2023-08-07 10:13:25.000000 permetrics-1.4.2/permetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-07 10:13:25.000000 permetrics-1.4.2/permetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:13:25.000000 permetrics-1.4.2/permetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 10:13:25.000000 permetrics-1.4.2/permetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 10:13:25.000000 permetrics-1.4.2/permetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:13:25.344230 permetrics-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-08-07 10:12:49.000000 permetrics-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:13:25.344230 permetrics-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-07 10:12:49.000000 permetrics-1.4.2/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-07 10:12:49.000000 permetrics-1.4.2/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-08-07 10:12:49.000000 permetrics-1.4.2/tests/test_regression.py
```

### Comparing `permetrics-1.4.1/CODE_OF_CONDUCT.md` & `permetrics-1.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/ChangeLog.md` & `permetrics-1.4.2/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# Version 1.4.2
++ Fix bug in get_support() function
++ Fix bug rounding number in ClassificationMetric 
++ Update logo and docs
+
+---------------------------------------------------------------------
+
 # Version 1.4.1
 + Remove all lowercase shortname of all metrics
 + Fix bugs in GINI function belongs to ClassificationMetric
 + Fix bugs in some functions belong to ClusteringMetric
 + Update characteristics of most of the functions (valid ranges and best value)
 + Add metrics to ClusteringMetrics
   + Entropy Score (ES)
```

### Comparing `permetrics-1.4.1/LICENSE` & `permetrics-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/PKG-INFO` & `permetrics-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permetrics
-Version: 1.4.1
+Version: 1.4.2
 Summary: PerMetrics: A Framework of Performance Metrics for Machine Learning Models
 Home-page: https://github.com/thieu1995/permetrics
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/permetrics
@@ -38,20 +38,24 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-<p align="center"><img src=".github/assets/logo2.png" alt="PERMETRICS" title="PERMETRICS"/></p>
+<p align="center">
+<img style="max-width:100%;" 
+src="https://thieu1995.github.io/post/2023-08/permetrics-01.png" 
+alt="PERMETRICS"/>
+</p>
 
 
 ---
 
-[![GitHub release](https://img.shields.io/badge/release-1.4.1-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
+[![GitHub release](https://img.shields.io/badge/release-1.4.2-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/permetrics) 
 [![PyPI version](https://badge.fury.io/py/permetrics.svg)](https://badge.fury.io/py/permetrics)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/permetrics.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/permetrics.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/permetrics.svg)
 [![Downloads](https://pepy.tech/badge/permetrics)](https://pepy.tech/project/permetrics)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/permetrics/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/permetrics/actions/workflows/publish-package.yaml)
@@ -67,15 +71,15 @@
 PerMetrics is a python library for performance metrics of machine learning models. We aim to implement all 
 performance metrics for problems such as regression, classification, clustering, ... problems. Helping users in all 
 field access metrics as fast as possible
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total metrics**: 103 (47 regression metrics, 16 classification metrics, 40 clustering metrics)
 * **Documentation:** https://permetrics.readthedocs.io/en/latest/
-* **Python versions:** > 3.7.x
+* **Python versions:** >= 3.7.x
 * **Dependencies:** numpy, scipy
 
 
 # Notification
 
 * **Currently, there is a huge misunderstanding among frameworks around the world about the notation of R, R2, and R^2.** 
 * Please read the file [R-R2-Rsquared.docx](https://github.com/thieu1995/permetrics/blob/master/R-R2-Rsquared.docx) to understand the differences between them and why there is such confusion.
@@ -87,32 +91,29 @@
 
 
 # Installation
 
 ### Install with pip
 Install the [current PyPI release](https://pypi.python.org/pypi/permetrics):
 ```sh 
-$ pip install permetrics==1.4.1
+$ pip install permetrics==1.4.2
 ```
 
 Or installing from the source code, use:
 ```sh 
 $ git clone https://github.com/thieu1995/permetrics.git
 $ cd permetrics
 $ python setup.py install
 ```
 
 Or install the development version from GitHub:
 ```bash
 pip install git+https://github.com/thieu1995/permetrics
 ```
 
-
-# Usage
-
 After installation, you can import Permetrics as any other Python module:
 
 ```sh
 $ python
 >>> import permetrics
 >>> permetrics.__version__
 ```
```

### Comparing `permetrics-1.4.1/R-R2-Rsquared.docx` & `permetrics-1.4.2/R-R2-Rsquared.docx`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/README.md` & `permetrics-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 
-<p align="center"><img src=".github/assets/logo2.png" alt="PERMETRICS" title="PERMETRICS"/></p>
+<p align="center">
+<img style="max-width:100%;" 
+src="https://thieu1995.github.io/post/2023-08/permetrics-01.png" 
+alt="PERMETRICS"/>
+</p>
 
 
 ---
 
-[![GitHub release](https://img.shields.io/badge/release-1.4.1-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
+[![GitHub release](https://img.shields.io/badge/release-1.4.2-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/permetrics) 
 [![PyPI version](https://badge.fury.io/py/permetrics.svg)](https://badge.fury.io/py/permetrics)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/permetrics.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/permetrics.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/permetrics.svg)
 [![Downloads](https://pepy.tech/badge/permetrics)](https://pepy.tech/project/permetrics)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/permetrics/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/permetrics/actions/workflows/publish-package.yaml)
@@ -24,15 +28,15 @@
 PerMetrics is a python library for performance metrics of machine learning models. We aim to implement all 
 performance metrics for problems such as regression, classification, clustering, ... problems. Helping users in all 
 field access metrics as fast as possible
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total metrics**: 103 (47 regression metrics, 16 classification metrics, 40 clustering metrics)
 * **Documentation:** https://permetrics.readthedocs.io/en/latest/
-* **Python versions:** > 3.7.x
+* **Python versions:** >= 3.7.x
 * **Dependencies:** numpy, scipy
 
 
 # Notification
 
 * **Currently, there is a huge misunderstanding among frameworks around the world about the notation of R, R2, and R^2.** 
 * Please read the file [R-R2-Rsquared.docx](https://github.com/thieu1995/permetrics/blob/master/R-R2-Rsquared.docx) to understand the differences between them and why there is such confusion.
@@ -44,32 +48,29 @@
 
 
 # Installation
 
 ### Install with pip
 Install the [current PyPI release](https://pypi.python.org/pypi/permetrics):
 ```sh 
-$ pip install permetrics==1.4.1
+$ pip install permetrics==1.4.2
 ```
 
 Or installing from the source code, use:
 ```sh 
 $ git clone https://github.com/thieu1995/permetrics.git
 $ cd permetrics
 $ python setup.py install
 ```
 
 Or install the development version from GitHub:
 ```bash
 pip install git+https://github.com/thieu1995/permetrics
 ```
 
-
-# Usage
-
 After installation, you can import Permetrics as any other Python module:
 
 ```sh
 $ python
 >>> import permetrics
 >>> permetrics.__version__
 ```
```

### Comparing `permetrics-1.4.1/permetrics/__init__.py` & `permetrics-1.4.2/permetrics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 # print(external_evaluator.MIS())
 #
 # internal_evaluator = ClusteringMetric(y_pred=y_pred, X=X, decimal=5)
 # print(internal_evaluator.banfeld_raftery_index())
 # print(internal_evaluator.BRI())
 
 
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 
 from .evaluator import Evaluator
 from .classification import ClassificationMetric
 from .regression import RegressionMetric
 from .clustering import ClusteringMetric
```

### Comparing `permetrics-1.4.1/permetrics/classification.py` & `permetrics-1.4.2/permetrics/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     @staticmethod
     def get_support(name=None, verbose=True):
         if name == "all":
             if verbose:
                 for key, value in ClassificationMetric.SUPPORT.items():
                     print(f"Metric {key} : {value}")
-                return ClassificationMetric.SUPPORT
+            return ClassificationMetric.SUPPORT
         if name not in list(ClassificationMetric.SUPPORT.keys()):
             raise ValueError(f"ClassificationMetric doesn't support metric named: {name}")
         else:
             if verbose:
                 print(f"Metric {name}: {ClassificationMetric.SUPPORT[name]}")
             return ClassificationMetric.SUPPORT[name]
 
@@ -325,23 +325,23 @@
 
         list_f1 = np.array([item["f1"] for item in metrics.values()])
         list_weights = np.array([item["n_true"] for item in metrics.values()])
 
         if average == "micro":
             tp_global = np.sum(np.diag(matrix))
             fp_global = fn_global = np.sum(matrix) - tp_global
-            precision = np.round(tp_global / (tp_global + fp_global), decimal)
+            precision = tp_global / (tp_global + fp_global)
             recall = tp_global / (tp_global + fn_global)
             f1 = (2 * precision * recall) / (precision + recall)
         elif average == "macro":
             f1 = np.mean(list_f1)
         elif average == "weighted":
             f1 = np.dot(list_weights, list_f1) / np.sum(list_weights)
         else:
-            f1 = dict([(label, item["f1"]) for label, item in metrics.items()])
+            f1 = dict([(label, np.round(item["f1"], decimal)) for label, item in metrics.items()])
         return f1 if type(f1) == dict else np.round(f1, decimal)
 
     def f2_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
         """
         Generate f2 score for multiple classification problem
         Higher is better (Best = 1), Range = [0, 1]
 
@@ -361,23 +361,23 @@
 
         list_f2 = np.array([item["f1"] for item in metrics.values()])
         list_weights = np.array([item["n_true"] for item in metrics.values()])
 
         if average == "micro":
             tp_global = np.sum(np.diag(matrix))
             fp_global = fn_global = np.sum(matrix) - tp_global
-            precision = np.round(tp_global / (tp_global + fp_global), decimal)
+            precision = tp_global / (tp_global + fp_global)
             recall = tp_global / (tp_global + fn_global)
             f2 = (5 * precision * recall) / (4 * precision + recall)
         elif average == "macro":
             f2 = np.mean(list_f2)
         elif average == "weighted":
             f2 = np.dot(list_weights, list_f2) / np.sum(list_weights)
         else:
-            f2 = dict([(label, item["f2"]) for label, item in metrics.items()])
+            f2 = dict([(label, np.round(item["f2"], decimal)) for label, item in metrics.items()])
         return f2 if type(f2) == dict else np.round(f2, decimal)
 
     def fbeta_score(self, y_true=None, y_pred=None, beta=1.0, labels=None, average="macro", decimal=None, **kwargs):
         """
         The beta parameter determines the weight of recall in the combined score.
         beta < 1 lends more weight to precision, while beta > 1 favors recall
         (beta -> 0 considers only precision, beta -> +inf only recall).
@@ -400,23 +400,23 @@
 
         list_fbeta = np.array([item["f1"] for item in metrics.values()])
         list_weights = np.array([item["n_true"] for item in metrics.values()])
 
         if average == "micro":
             tp_global = np.sum(np.diag(matrix))
             fp_global = fn_global = np.sum(matrix) - tp_global
-            precision = np.round(tp_global / (tp_global + fp_global), decimal)
+            precision = tp_global / (tp_global + fp_global)
             recall = tp_global / (tp_global + fn_global)
             fbeta = ((1 + beta ** 2) * precision * recall) / (beta ** 2 * precision + recall)
         elif average == "macro":
             fbeta = np.mean(list_fbeta)
         elif average == "weighted":
             fbeta = np.dot(list_weights, list_fbeta) / np.sum(list_weights)
         else:
-            fbeta = dict([(label, item["fbeta"]) for label, item in metrics.items()])
+            fbeta = dict([(label, np.round(item["fbeta"], decimal)) for label, item in metrics.items()])
         return fbeta if type(fbeta) == dict else np.round(fbeta, decimal)
 
     def matthews_correlation_coefficient(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
         """
         Generate Matthews Correlation Coefficient
         Higher is better (Best = 1), Range = [-1, +1]
 
@@ -442,15 +442,15 @@
             fp = fn = np.sum(matrix) - tp
             mcc = (tp * tn - fp * fn) / np.sqrt(((tp + fp) * (tp + fn) * (tn + fp) * (tn + fn)))
         elif average == "macro":
             mcc = np.mean(list_mcc)
         elif average == "weighted":
             mcc = np.dot(list_weights, list_mcc) / np.sum(list_weights)
         else:
-            mcc = dict([(label, item["mcc"]) for label, item in metrics.items()])
+            mcc = dict([(label, np.round(item["mcc"], decimal)) for label, item in metrics.items()])
         return mcc if type(mcc) == dict else np.round(mcc, decimal)
 
     def hamming_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
         """
         Generate hamming score for multiple classification problem
         Higher is better (Best = 1), Range = [0, 1]
```

### Comparing `permetrics-1.4.1/permetrics/clustering.py` & `permetrics-1.4.2/permetrics/clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     @staticmethod
     def get_support(name=None, verbose=True):
         if name == "all":
             if verbose:
                 for key, value in ClusteringMetric.SUPPORT.items():
                     print(f"Metric {key} : {value}")
-                return ClusteringMetric.SUPPORT
+            return ClusteringMetric.SUPPORT
         if name not in list(ClusteringMetric.SUPPORT.keys()):
             raise ValueError(f"ClusteringMetric doesn't support metric named: {name}")
         else:
             if verbose:
                 print(f"Metric {name}: {ClusteringMetric.SUPPORT[name]}")
             return ClusteringMetric.SUPPORT[name]
 
@@ -265,15 +265,15 @@
         centroids = cu.get_centroids(X, y_pred)
         euc_distance_to_centroids = cu.get_min_dist(X, centroids)
         WGSS = np.sum(euc_distance_to_centroids**2)
         # Computing the minimum squared distance to the centroids:
         MinSqDist = np.min(cu.pdist(centroids, metric='sqeuclidean'))
         # Computing the XB index:
         xb = (1 / X.shape[0]) * (WGSS / MinSqDist)
-        return xb
+        return np.round(xb, decimal)
 
     def banfeld_raftery_index(self, X=None, y_pred=None, decimal=None, **kwargs):
         """
         Computes the Banfeld-Raftery Index.
         Smaller is better (No best value), Range=(-inf, inf)
         This index is the weighted sum of the logarithms of the traces of the variance covariance matrix of each cluster
```

### Comparing `permetrics-1.4.1/permetrics/evaluator.py` & `permetrics-1.4.2/permetrics/evaluator.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/permetrics/regression.py` & `permetrics-1.4.2/permetrics/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     @staticmethod
     def get_support(name=None, verbose=True):
         if name == "all":
             if verbose:
                 for key, value in RegressionMetric.SUPPORT.items():
                     print(f"Metric {key} : {value}")
-                return RegressionMetric.SUPPORT
+            return RegressionMetric.SUPPORT
         if name not in list(RegressionMetric.SUPPORT.keys()):
             raise ValueError(f"RegressionMetric doesn't support metric named: {name}")
         else:
             if verbose:
                 print(f"Metric {name}: {RegressionMetric.SUPPORT[name]}")
             return RegressionMetric.SUPPORT[name]
```

### Comparing `permetrics-1.4.1/permetrics/utils/classifier_util.py` & `permetrics-1.4.2/permetrics/utils/classifier_util.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/permetrics/utils/cluster_util.py` & `permetrics-1.4.2/permetrics/utils/cluster_util.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/permetrics/utils/data_util.py` & `permetrics-1.4.2/permetrics/utils/data_util.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/permetrics/utils/encoder.py` & `permetrics-1.4.2/permetrics/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/permetrics/utils/regressor_util.py` & `permetrics-1.4.2/permetrics/utils/regressor_util.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/permetrics.egg-info/PKG-INFO` & `permetrics-1.4.2/permetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permetrics
-Version: 1.4.1
+Version: 1.4.2
 Summary: PerMetrics: A Framework of Performance Metrics for Machine Learning Models
 Home-page: https://github.com/thieu1995/permetrics
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/permetrics
@@ -38,20 +38,24 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-<p align="center"><img src=".github/assets/logo2.png" alt="PERMETRICS" title="PERMETRICS"/></p>
+<p align="center">
+<img style="max-width:100%;" 
+src="https://thieu1995.github.io/post/2023-08/permetrics-01.png" 
+alt="PERMETRICS"/>
+</p>
 
 
 ---
 
-[![GitHub release](https://img.shields.io/badge/release-1.4.1-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
+[![GitHub release](https://img.shields.io/badge/release-1.4.2-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/permetrics) 
 [![PyPI version](https://badge.fury.io/py/permetrics.svg)](https://badge.fury.io/py/permetrics)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/permetrics.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/permetrics.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/permetrics.svg)
 [![Downloads](https://pepy.tech/badge/permetrics)](https://pepy.tech/project/permetrics)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/permetrics/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/permetrics/actions/workflows/publish-package.yaml)
@@ -67,15 +71,15 @@
 PerMetrics is a python library for performance metrics of machine learning models. We aim to implement all 
 performance metrics for problems such as regression, classification, clustering, ... problems. Helping users in all 
 field access metrics as fast as possible
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total metrics**: 103 (47 regression metrics, 16 classification metrics, 40 clustering metrics)
 * **Documentation:** https://permetrics.readthedocs.io/en/latest/
-* **Python versions:** > 3.7.x
+* **Python versions:** >= 3.7.x
 * **Dependencies:** numpy, scipy
 
 
 # Notification
 
 * **Currently, there is a huge misunderstanding among frameworks around the world about the notation of R, R2, and R^2.** 
 * Please read the file [R-R2-Rsquared.docx](https://github.com/thieu1995/permetrics/blob/master/R-R2-Rsquared.docx) to understand the differences between them and why there is such confusion.
@@ -87,32 +91,29 @@
 
 
 # Installation
 
 ### Install with pip
 Install the [current PyPI release](https://pypi.python.org/pypi/permetrics):
 ```sh 
-$ pip install permetrics==1.4.1
+$ pip install permetrics==1.4.2
 ```
 
 Or installing from the source code, use:
 ```sh 
 $ git clone https://github.com/thieu1995/permetrics.git
 $ cd permetrics
 $ python setup.py install
 ```
 
 Or install the development version from GitHub:
 ```bash
 pip install git+https://github.com/thieu1995/permetrics
 ```
 
-
-# Usage
-
 After installation, you can import Permetrics as any other Python module:
 
 ```sh
 $ python
 >>> import permetrics
 >>> permetrics.__version__
 ```
```

### Comparing `permetrics-1.4.1/permetrics.egg-info/SOURCES.txt` & `permetrics-1.4.2/permetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/setup.py` & `permetrics-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="permetrics",
-    version="1.4.1",
+    version="1.4.2",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="PerMetrics: A Framework of Performance Metrics for Machine Learning Models",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["regression", "classification", "clustering", "metrics", "performance metrics",
               "rmse", "mae", "mape", "nse", "nash-sutcliffe-efficiency", "willmott-index",
```

### Comparing `permetrics-1.4.1/tests/test_classification.py` & `permetrics-1.4.2/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/tests/test_clustering.py` & `permetrics-1.4.2/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.4.1/tests/test_regression.py` & `permetrics-1.4.2/tests/test_regression.py`

 * *Files identical despite different names*

