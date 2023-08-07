# Comparing `tmp/calf_milp-0.0.2.tar.gz` & `tmp/calf_milp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calf_milp-0.0.2.tar", last modified: Sat Aug  5 04:20:13 2023, max compression
+gzip compressed data, was "calf_milp-0.0.3.tar", last modified: Sat Aug  5 04:28:44 2023, max compression
```

## Comparing `calf_milp-0.0.2.tar` & `calf_milp-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:20:13.753589 calf_milp-0.0.2/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-08-02 13:53:45.000000 calf_milp-0.0.2/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-08-02 13:53:45.000000 calf_milp-0.0.2/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2951 2023-08-05 04:20:13.753589 calf_milp-0.0.2/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2106 2023-08-02 14:44:06.000000 calf_milp-0.0.2/README.rst
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:20:13.753589 calf_milp-0.0.2/calf_milp/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      167 2023-08-02 14:23:44.000000 calf_milp-0.0.2/calf_milp/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-05 04:18:55.000000 calf_milp-0.0.2/calf_milp/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4222 2023-08-02 14:44:06.000000 calf_milp-0.0.2/calf_milp/calf_milp.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8277 2023-07-25 20:07:15.000000 calf_milp-0.0.2/calf_milp/calf_sat.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:20:13.753589 calf_milp-0.0.2/calf_milp/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-08-02 13:53:45.000000 calf_milp-0.0.2/calf_milp/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      243 2023-08-02 14:24:00.000000 calf_milp-0.0.2/calf_milp/tests/test_common.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      402 2023-08-02 14:44:06.000000 calf_milp-0.0.2/calf_milp/tests/test_template.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:20:13.753589 calf_milp-0.0.2/calf_milp.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2951 2023-08-05 04:20:13.000000 calf_milp-0.0.2/calf_milp.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      443 2023-08-05 04:20:13.000000 calf_milp-0.0.2/calf_milp.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 04:20:13.000000 calf_milp-0.0.2/calf_milp.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 04:20:13.000000 calf_milp-0.0.2/calf_milp.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-05 04:20:13.000000 calf_milp-0.0.2/calf_milp.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       10 2023-08-05 04:20:13.000000 calf_milp-0.0.2/calf_milp.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      142 2023-08-02 13:53:45.000000 calf_milp-0.0.2/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-05 04:20:13.753589 calf_milp-0.0.2/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2641 2023-08-02 14:41:03.000000 calf_milp-0.0.2/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:28:44.296071 calf_milp-0.0.3/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-08-02 13:53:45.000000 calf_milp-0.0.3/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-08-02 13:53:45.000000 calf_milp-0.0.3/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2476 2023-08-05 04:28:44.296071 calf_milp-0.0.3/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1630 2023-08-05 04:27:42.000000 calf_milp-0.0.3/README.rst
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:28:44.292071 calf_milp-0.0.3/calf_milp/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      167 2023-08-02 14:23:44.000000 calf_milp-0.0.3/calf_milp/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-05 04:27:42.000000 calf_milp-0.0.3/calf_milp/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     4222 2023-08-02 14:44:06.000000 calf_milp-0.0.3/calf_milp/calf_milp.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     8277 2023-07-25 20:07:15.000000 calf_milp-0.0.3/calf_milp/calf_sat.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:28:44.296071 calf_milp-0.0.3/calf_milp/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-08-02 13:53:45.000000 calf_milp-0.0.3/calf_milp/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      243 2023-08-02 14:24:00.000000 calf_milp-0.0.3/calf_milp/tests/test_common.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      402 2023-08-02 14:44:06.000000 calf_milp-0.0.3/calf_milp/tests/test_template.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:28:44.296071 calf_milp-0.0.3/calf_milp.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2476 2023-08-05 04:28:44.000000 calf_milp-0.0.3/calf_milp.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      443 2023-08-05 04:28:44.000000 calf_milp-0.0.3/calf_milp.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 04:28:44.000000 calf_milp-0.0.3/calf_milp.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 04:20:13.000000 calf_milp-0.0.3/calf_milp.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-05 04:28:44.000000 calf_milp-0.0.3/calf_milp.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       10 2023-08-05 04:28:44.000000 calf_milp-0.0.3/calf_milp.egg-info/top_level.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      142 2023-08-02 13:53:45.000000 calf_milp-0.0.3/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-05 04:28:44.296071 calf_milp-0.0.3/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2641 2023-08-02 14:41:03.000000 calf_milp-0.0.3/setup.py
```

### Comparing `calf_milp-0.0.2/LICENSE` & `calf_milp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calf_milp-0.0.2/PKG-INFO` & `calf_milp-0.0.3/calf_milp.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calf_milp
-Version: 0.0.2
+Name: calf-milp
+Version: 0.0.3
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/calf-milp
 Download-URL: https://github.com/hrolfrc/calf-milp
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -23,41 +23,37 @@
 .. -*- mode: rst -*-
 
 |ReadTheDocs|_
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calf-milp/badge/?version=latest
 .. _ReadTheDocs: https://calf-milp.readthedocs.io/en/latest/?badge=latest
 
-CalfMilp - Saddle point problem for AUC maximization
-============================================================
+CalfMilp - A classifier with integer weights
+=============================================
 
-An AUC optimizing binomial classifier.
+A binomial classifier that fits using mixed integer linear programming.
 
 Contact
 ------------------
 Rolf Carlson hrolfrc@gmail.com
 
 Install
 ------------------
 Use pip to install calf-milp.
 
 ``pip install calf-milp``
 
 Introduction
 ------------------
-This is a python implementation of a classifier that endeavors to solve the `saddle point problem for AUC maximization`_. [1]
-
-CalfMilp provides classification and prediction for two classes, the binomial case.  Small to medium problems are supported.  This is research code and a work in progress.
+CalfMilp provides classification and prediction for two classes, the binomial case.  Small problems are supported.  This is research code and a work in progress.
 
 CalfMilp is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
-.. _`saddle point problem for AUC maximization`: https://www.frontiersin.org/articles/10.3389/fams.2019.00030/full
-
 Example
 ------------------
 
 .. code:: ipython2
 
     from calf-milp import CalfMilp
     from sklearn.datasets import make_classification
@@ -93,13 +89,7 @@
 
     cls.score(X_test, y_test)
 
 
 .. parsed-literal::
 
     1.0
-
-References
-------------------
-[1] Natole Jr, Michael & Ying, Yiming & Lyu, Siwei. (2019).
-Stochastic AUC Optimization Algorithms With Linear Convergence.
-Frontiers in Applied Mathematics and Statistics. 5. 10.3389/fams.2019.00030.
```

### Comparing `calf_milp-0.0.2/README.rst` & `calf_milp-0.0.3/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 .. -*- mode: rst -*-
 
 |ReadTheDocs|_
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calf-milp/badge/?version=latest
 .. _ReadTheDocs: https://calf-milp.readthedocs.io/en/latest/?badge=latest
 
-CalfMilp - Saddle point problem for AUC maximization
-============================================================
+CalfMilp - A classifier with integer weights
+=============================================
 
-An AUC optimizing binomial classifier.
+A binomial classifier that fits using mixed integer linear programming.
 
 Contact
 ------------------
 Rolf Carlson hrolfrc@gmail.com
 
 Install
 ------------------
 Use pip to install calf-milp.
 
 ``pip install calf-milp``
 
 Introduction
 ------------------
-This is a python implementation of a classifier that endeavors to solve the `saddle point problem for AUC maximization`_. [1]
-
-CalfMilp provides classification and prediction for two classes, the binomial case.  Small to medium problems are supported.  This is research code and a work in progress.
+CalfMilp provides classification and prediction for two classes, the binomial case.  Small problems are supported.  This is research code and a work in progress.
 
 CalfMilp is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
-.. _`saddle point problem for AUC maximization`: https://www.frontiersin.org/articles/10.3389/fams.2019.00030/full
-
 Example
 ------------------
 
 .. code:: ipython2
 
     from calf-milp import CalfMilp
     from sklearn.datasets import make_classification
@@ -70,14 +66,8 @@
 .. code:: ipython2
 
     cls.score(X_test, y_test)
 
 
 .. parsed-literal::
 
-    1.0
-
-References
-------------------
-[1] Natole Jr, Michael & Ying, Yiming & Lyu, Siwei. (2019).
-Stochastic AUC Optimization Algorithms With Linear Convergence.
-Frontiers in Applied Mathematics and Statistics. 5. 10.3389/fams.2019.00030.
+    1.0
```

### Comparing `calf_milp-0.0.2/calf_milp/calf_milp.py` & `calf_milp-0.0.3/calf_milp/calf_milp.py`

 * *Files identical despite different names*

### Comparing `calf_milp-0.0.2/calf_milp/calf_sat.py` & `calf_milp-0.0.3/calf_milp/calf_sat.py`

 * *Files identical despite different names*

### Comparing `calf_milp-0.0.2/calf_milp.egg-info/PKG-INFO` & `calf_milp-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calf-milp
-Version: 0.0.2
+Name: calf_milp
+Version: 0.0.3
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/calf-milp
 Download-URL: https://github.com/hrolfrc/calf-milp
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -23,41 +23,37 @@
 .. -*- mode: rst -*-
 
 |ReadTheDocs|_
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calf-milp/badge/?version=latest
 .. _ReadTheDocs: https://calf-milp.readthedocs.io/en/latest/?badge=latest
 
-CalfMilp - Saddle point problem for AUC maximization
-============================================================
+CalfMilp - A classifier with integer weights
+=============================================
 
-An AUC optimizing binomial classifier.
+A binomial classifier that fits using mixed integer linear programming.
 
 Contact
 ------------------
 Rolf Carlson hrolfrc@gmail.com
 
 Install
 ------------------
 Use pip to install calf-milp.
 
 ``pip install calf-milp``
 
 Introduction
 ------------------
-This is a python implementation of a classifier that endeavors to solve the `saddle point problem for AUC maximization`_. [1]
-
-CalfMilp provides classification and prediction for two classes, the binomial case.  Small to medium problems are supported.  This is research code and a work in progress.
+CalfMilp provides classification and prediction for two classes, the binomial case.  Small problems are supported.  This is research code and a work in progress.
 
 CalfMilp is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
-.. _`saddle point problem for AUC maximization`: https://www.frontiersin.org/articles/10.3389/fams.2019.00030/full
-
 Example
 ------------------
 
 .. code:: ipython2
 
     from calf-milp import CalfMilp
     from sklearn.datasets import make_classification
@@ -93,13 +89,7 @@
 
     cls.score(X_test, y_test)
 
 
 .. parsed-literal::
 
     1.0
-
-References
-------------------
-[1] Natole Jr, Michael & Ying, Yiming & Lyu, Siwei. (2019).
-Stochastic AUC Optimization Algorithms With Linear Convergence.
-Frontiers in Applied Mathematics and Statistics. 5. 10.3389/fams.2019.00030.
```

### Comparing `calf_milp-0.0.2/setup.py` & `calf_milp-0.0.3/setup.py`

 * *Files identical despite different names*

