# Comparing `tmp/sppam-0.0.9.tar.gz` & `tmp/sppam-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sppam-0.0.9.tar", last modified: Wed Aug  2 02:45:14 2023, max compression
+gzip compressed data, was "sppam-0.1.0.tar", last modified: Mon Aug  7 20:21:32 2023, max compression
```

## Comparing `sppam-0.0.9.tar` & `sppam-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:45:14.484481 sppam-0.0.9/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-07-30 01:58:42.000000 sppam-0.0.9/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-30 01:58:42.000000 sppam-0.0.9/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2904 2023-08-02 02:45:14.484481 sppam-0.0.9/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2071 2023-08-01 23:51:40.000000 sppam-0.0.9/README.rst
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      142 2023-08-01 20:18:30.000000 sppam-0.0.9/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-02 02:45:14.484481 sppam-0.0.9/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2617 2023-08-01 23:57:37.000000 sppam-0.0.9/setup.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:45:14.480481 sppam-0.0.9/sppam/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      145 2023-08-01 18:31:29.000000 sppam-0.0.9/sppam/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-02 02:42:13.000000 sppam-0.0.9/sppam/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8291 2023-08-02 02:34:31.000000 sppam-0.0.9/sppam/sppam.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:45:14.484481 sppam-0.0.9/sppam/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-30 01:58:42.000000 sppam-0.0.9/sppam/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      239 2023-08-01 18:32:49.000000 sppam-0.0.9/sppam/tests/test_common.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      389 2023-08-01 20:08:16.000000 sppam-0.0.9/sppam/tests/test_template.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 02:45:14.484481 sppam-0.0.9/sppam.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2904 2023-08-02 02:45:14.000000 sppam-0.0.9/sppam.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      369 2023-08-02 02:45:14.000000 sppam-0.0.9/sppam.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-02 02:45:14.000000 sppam-0.0.9/sppam.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-01 22:53:39.000000 sppam-0.0.9/sppam.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-02 02:45:14.000000 sppam-0.0.9/sppam.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        6 2023-08-02 02:45:14.000000 sppam-0.0.9/sppam.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 20:21:32.364461 sppam-0.1.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1529 2023-08-07 20:20:27.000000 sppam-0.1.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-07 20:20:27.000000 sppam-0.1.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2982 2023-08-07 20:21:32.364461 sppam-0.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2153 2023-08-07 20:20:27.000000 sppam-0.1.0/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-08-07 20:20:27.000000 sppam-0.1.0/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-08-07 20:21:32.364461 sppam-0.1.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-08-07 20:20:27.000000 sppam-0.1.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 20:21:32.364461 sppam-0.1.0/sppam/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      145 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11206 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/sppam.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 20:21:32.364461 sppam-0.1.0/sppam/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      239 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/tests/test_common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/tests/test_template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 20:21:32.364461 sppam-0.1.0/sppam.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2982 2023-08-07 20:21:32.000000 sppam-0.1.0/sppam.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      369 2023-08-07 20:21:32.000000 sppam-0.1.0/sppam.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 20:21:32.000000 sppam-0.1.0/sppam.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 20:21:16.000000 sppam-0.1.0/sppam.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-08-07 20:21:32.000000 sppam-0.1.0/sppam.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-08-07 20:21:32.000000 sppam-0.1.0/sppam.egg-info/top_level.txt
```

### Comparing `sppam-0.0.9/LICENSE` & `sppam-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sppam-0.0.9/PKG-INFO` & `sppam-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 Metadata-Version: 2.1
 Name: sppam
-Version: 0.0.9
+Version: 0.1.0
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/sppam
 Download-URL: https://github.com/hrolfrc/sppam
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
-|ReadTheDocs|_
+|CircleCI|_ |ReadTheDocs|_
+
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/sppam.svg?style=shield
+.. _CircleCI: https://circleci.com/gh/hrolfrc/sppam
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/sppam/badge/?version=latest
 .. _ReadTheDocs: https://sppam.readthedocs.io/en/latest/?badge=latest
 
-SPPAM - Saddle point problem for AUC maximization
-============================================================
+SPPAM
+#####################################
 
 An AUC optimizing binomial classifier.
 
 Contact
 ------------------
+
 Rolf Carlson hrolfrc@gmail.com
 
 Install
 ------------------
 Use pip to install sppam.
 
 ``pip install sppam``
 
 Introduction
 ------------------
-This is a python implementation of a classifier that endeavors to solve the `saddle point problem for AUC maximization`_. [1]
+This is a python implementation of a classifier that approximates the solution to the `saddle point problem for AUC maximization`_. [1]
 
 SPPAM provides classification and prediction for two classes, the binomial case.  Small to medium problems are supported.  This is research code and a work in progress.
 
 SPPAM is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
 .. _`saddle point problem for AUC maximization`: https://www.frontiersin.org/articles/10.3389/fams.2019.00030/full
 
 Example
-------------------
+===========
 
 .. code:: ipython2
 
     from sppam import SPPAM
     from sklearn.datasets import make_classification
     from sklearn.model_selection import train_test_split
 
@@ -90,16 +94,19 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     cls.score(X_test, y_test)
 
 
+
+
 .. parsed-literal::
 
     1.0
 
+
 References
 ------------------
 [1] Natole Jr, Michael & Ying, Yiming & Lyu, Siwei. (2019).
 Stochastic AUC Optimization Algorithms With Linear Convergence.
 Frontiers in Applied Mathematics and Statistics. 5. 10.3389/fams.2019.00030.
```

### Comparing `sppam-0.0.9/README.rst` & `sppam-0.1.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 .. -*- mode: rst -*-
 
-|ReadTheDocs|_
+|CircleCI|_ |ReadTheDocs|_
+
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/sppam.svg?style=shield
+.. _CircleCI: https://circleci.com/gh/hrolfrc/sppam
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/sppam/badge/?version=latest
 .. _ReadTheDocs: https://sppam.readthedocs.io/en/latest/?badge=latest
 
-SPPAM - Saddle point problem for AUC maximization
-============================================================
+SPPAM
+#####################################
 
 An AUC optimizing binomial classifier.
 
 Contact
 ------------------
+
 Rolf Carlson hrolfrc@gmail.com
 
 Install
 ------------------
 Use pip to install sppam.
 
 ``pip install sppam``
 
 Introduction
 ------------------
-This is a python implementation of a classifier that endeavors to solve the `saddle point problem for AUC maximization`_. [1]
+This is a python implementation of a classifier that approximates the solution to the `saddle point problem for AUC maximization`_. [1]
 
 SPPAM provides classification and prediction for two classes, the binomial case.  Small to medium problems are supported.  This is research code and a work in progress.
 
 SPPAM is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
 .. _`saddle point problem for AUC maximization`: https://www.frontiersin.org/articles/10.3389/fams.2019.00030/full
 
 Example
-------------------
+===========
 
 .. code:: ipython2
 
     from sppam import SPPAM
     from sklearn.datasets import make_classification
     from sklearn.model_selection import train_test_split
 
@@ -68,16 +72,19 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     cls.score(X_test, y_test)
 
 
+
+
 .. parsed-literal::
 
     1.0
 
+
 References
 ------------------
 [1] Natole Jr, Michael & Ying, Yiming & Lyu, Siwei. (2019).
 Stochastic AUC Optimization Algorithms With Linear Convergence.
 Frontiers in Applied Mathematics and Statistics. 5. 10.3389/fams.2019.00030.
```

### Comparing `sppam-0.0.9/setup.py` & `sppam-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 DOWNLOAD_URL = 'https://github.com/hrolfrc/sppam'
 VERSION = _version.__version__
 INSTALL_REQUIRES = ['numpy', 'scipy', 'scikit-learn']
 CLASSIFIERS = ['Intended Audience :: Science/Research',
                'Intended Audience :: Developers',
                'Topic :: Scientific/Engineering :: Artificial Intelligence',
                'Topic :: Scientific/Engineering :: Mathematics',
-               'Development Status :: 2 - Pre-Alpha',
+               'Development Status :: 3 - Alpha',
                'License :: OSI Approved',
                'Topic :: Scientific/Engineering',
                'Operating System :: OS Independent',
                'Programming Language :: Python :: 3']
 
 EXTRAS_REQUIRE = {
     'tests': [
```

### Comparing `sppam-0.0.9/sppam/sppam.py` & `sppam-0.1.0/sppam/sppam.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Natole Jr, Michael & Ying, Yiming & Lyu, Siwei. (2019).
 Stochastic AUC Optimization Algorithms With Linear Convergence.
 Frontiers in Applied Mathematics and Statistics. 5. 10.3389/fams.2019.00030.
 https://www.frontiersin.org/articles/10.3389/fams.2019.00030/full#B5
 
 """
-
+import time
 from collections import Counter
 
 import numpy as np
 from ortools.linear_solver.pywraplp import Solver
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.datasets import make_classification
 from sklearn.metrics import roc_auc_score
@@ -53,14 +53,17 @@
         1.  Classification of patterns using LP
         https://www.stat.cmu.edu/~ryantibs/convexopt-F13/scribes/lec2.pdf
 
         2.  LP formulation evolving to regularization and SVM
         Calf looks similar to dual problem on slide 14
         https://people.eecs.berkeley.edu/~russell/classes/cs194/f11/lectures/CS194%20Fall%202011%20Lecture%2005.pdf
 
+        3. Natole Jr, Michael & Ying, Yiming & Lyu, Siwei. (2019).
+        Stochastic AUC Optimization Algorithms With Linear Convergence.
+        Frontiers in Applied Mathematics and Statistics. 5. 10.3389/fams.2019.00030.
 
     Examples:
         >>> from sklearn.datasets import make_classification
         >>> from sklearn.metrics import roc_auc_score
 
         # Make a classification problem
         >>> X_d, y_d = make_classification(
@@ -90,27 +93,30 @@
         0.99
 
     """
 
     feature_range = list(range(X.shape[1]))
     sample_range = list(range(X.shape[0]))
 
-    # solver = Solver.CreateSolver('GLOP')
     solver = Solver.CreateSolver('GLOP')
 
     # The following recommendation to improve GLOP performance degrades the AUC.
     # https: https://developers.google.com/optimization/lp/lp_advanced#choice_of_solvers_and_algorithms
     # uncomment to see the relative performance in calf_lp.ipynb
     # solver.use_dual_simplex = True
 
     if not solver:
         raise RuntimeError("GLOP solver unavailable")
+    solver.SetTimeLimit(1000)
+
+    # n_plus and n_minus are the numbers of samples of the positive and negative cases.
+    # protect against division by zero.
+    n_plus = max(Counter(y)[1], 1)
+    n_minus = max(Counter(y)[0], 1)
 
-    n_plus = Counter(y)[1]
-    n_minus = Counter(y)[0]
     # w[i] is 0 if feature i is excluded
     # otherwise the weight is 1 or -1
     w = {}
     for j in feature_range:
         w[j] = solver.NumVar(-1, 1, 'w[%i]' % j)
 
     pos = (1 / n_plus) * sum([X[i][j] * w[j] for j in feature_range for i in sample_range if y[i] == 1])
@@ -147,25 +153,64 @@
 # noinspection PyAttributeOutsideInit
 class SPPAM(ClassifierMixin, BaseEstimator):
     """ The SPPAM (Saddle Point Problem for AUC Maximization) classifier
 
         Attributes
         ----------
 
-        classes_ : ndarray of shape (n_classes, )
-            A list of class labels known to the classifier.
-
-        coef_ : feature weights of shape (1, n_features).
+        coef_ : array of shape (n_features, )
+            Estimated coefficients for the linear fit problem.  Only
+            one target should be passed, and this is a 1D array of length
+            n_features.
 
         n_features_in_ : int
-            The number of features of the data passed to :meth:`fit`.
+            Number of features seen during :term:`fit`.
 
-    """
+        classes_ : list
+            The unique class labels
+
+        fit_time_ : float
+            The number of seconds to fit X to y
+
+        Examples
+        --------
+            >>> import numpy
+            >>> from sklearn.datasets import make_classification as mc
+            >>> X, y = mc(n_features=2, n_redundant=0, n_informative=2, n_clusters_per_class=1, random_state=42)
+            >>> numpy.round(X[0:3, :], 2)
+            array([[ 1.23, -0.76],
+                   [ 0.7 , -1.38],
+                   [ 2.55,  2.5 ]])
+
+            >>> y[0:3]
+            array([0, 0, 1])
+
+            >>> cls = SPPAM().fit(X, y)
+            >>> cls.score(X, y)
+            0.95
+
+            >>> np.round(cls.coef_, 4)
+            array([-0.2463,  1.    ])
+
+            >>> numpy.round(cls.score(X, y), 2)
+            0.95
+
+            >>> cls.fit_time_ > 0
+            True
+
+            >>> cls.predict(np.array([[3, 5]]))
+            array([0])
+
+            >>> cls.predict_proba(np.array([[3, 5]]))
+            array([[1., 0.]])
+
+        """
 
     def __init__(self):
+        """ Initialize SPPAM """
         pass
 
     def fit(self, X, y):
         """ Fit the model according to the given training data.
 
         Parameters
         ----------
@@ -185,20 +230,33 @@
             raise ValueError('requires y to be passed, but the target y is None')
 
         X, y = check_X_y(X, y)
         self.n_features_in_ = X.shape[1]
         self.classes_ = unique_labels(y)
         self.X_ = X
         self.y_ = y
+
+        start = time.time()
         self.w_, self.status_ = lp_weights(X, y)
-        self.is_fitted_ = True
+        self.fit_time_ = time.time() - start
         self.coef_ = self.w_
+        self.is_fitted_ = True
         return self
 
     def decision_function(self, X):
+        """ Identify confidence scores for the samples
+
+        Arguments:
+            X : array-like, shape (n_samples, n_features)
+                The training input features and samples
+
+        Returns:
+            the decision vector (n_samples)
+
+        """
         check_is_fitted(self, ['is_fitted_', 'X_', 'y_'])
 
         X = self._validate_data(X, accept_sparse="csr", reset=False)
         scores = np.array(
             minmax_scale(
                 predict(X, self.w_),
                 feature_range=(-1, 1)
@@ -206,20 +264,18 @@
         )
         return scores
 
     def predict(self, X):
         """Predict class labels for samples in X.
 
         Parameters:
-
             X : {array-like, sparse matrix} of shape (n_samples, n_features)
                 The data matrix for which we want to get the predictions.
 
         Returns:
-
             y_pred : ndarray of shape (n_samples,)
                 Vector containing the class labels for each sample.
         """
         check_is_fitted(self, ['is_fitted_', 'X_', 'y_'])
         X = check_array(X)
 
         if len(self.classes_) < 2:
@@ -231,37 +287,69 @@
             y_class = [self.classes_[x] for x in y_class]
         return np.array(y_class)
 
     def predict_proba(self, X):
         """Probability estimates for samples in X.
 
         Parameters:
-
             X : array-like of shape (n_samples, n_features)
                 Vector to be scored, where n_samples is the number of samples and
                 n_features is the number of features.
 
         Returns:
-
             T: array-like of shape (n_samples, n_classes)
                 Returns the probability of the sample for each class in the model,
                 where classes are ordered as they are in `self.classes_`.
 
-            """
+        """
         check_is_fitted(self, ['is_fitted_', 'X_', 'y_'])
         X = check_array(X)
 
         y_proba = np.array(
             minmax_scale(
                 self.decision_function(X),
                 feature_range=(0, 1)
             )
         )
         class_prob = np.column_stack((1 - y_proba, y_proba))
         return class_prob
 
+    def transform(self, X):
+        """ Reduce X to the features that contribute positive AUC.
+
+        Arguments:
+            X : array-like, shape (n_samples, n_features)
+                The training input features and samples
+
+        Returns:
+            X_r : array of shape [n_samples, n_selected_features]
+            The input samples with only the selected features.
+
+        """
+        check_is_fitted(self, ['is_fitted_', 'X_', 'y_'])
+        X = check_array(X)
+
+        return X[:, np.asarray(self.coef_).nonzero()]
+
+    def fit_transform(self, X, y):
+        """ Fit to the data, then reduce X to the features that contribute positive AUC.
+
+            Arguments:
+                X : array-like, shape (n_samples, n_features)
+                    The training input features and samples
+
+                y : array-like of shape (n_samples,)
+                    Target vector relative to X.
+
+            Returns:
+                X_r : array of shape [n_samples, n_selected_features]
+                The input samples with only the selected features.
+
+            """
+        return self.fit(X, y).transform(X)
+
     def _more_tags(self):
         return {
             'poor_score': True,
             'non_deterministic': True,
             'binary_only': True
         }
```

### Comparing `sppam-0.0.9/sppam.egg-info/PKG-INFO` & `sppam-0.1.0/sppam.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 Metadata-Version: 2.1
 Name: sppam
-Version: 0.0.9
+Version: 0.1.0
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/sppam
 Download-URL: https://github.com/hrolfrc/sppam
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
-|ReadTheDocs|_
+|CircleCI|_ |ReadTheDocs|_
+
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/sppam.svg?style=shield
+.. _CircleCI: https://circleci.com/gh/hrolfrc/sppam
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/sppam/badge/?version=latest
 .. _ReadTheDocs: https://sppam.readthedocs.io/en/latest/?badge=latest
 
-SPPAM - Saddle point problem for AUC maximization
-============================================================
+SPPAM
+#####################################
 
 An AUC optimizing binomial classifier.
 
 Contact
 ------------------
+
 Rolf Carlson hrolfrc@gmail.com
 
 Install
 ------------------
 Use pip to install sppam.
 
 ``pip install sppam``
 
 Introduction
 ------------------
-This is a python implementation of a classifier that endeavors to solve the `saddle point problem for AUC maximization`_. [1]
+This is a python implementation of a classifier that approximates the solution to the `saddle point problem for AUC maximization`_. [1]
 
 SPPAM provides classification and prediction for two classes, the binomial case.  Small to medium problems are supported.  This is research code and a work in progress.
 
 SPPAM is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
 .. _`saddle point problem for AUC maximization`: https://www.frontiersin.org/articles/10.3389/fams.2019.00030/full
 
 Example
-------------------
+===========
 
 .. code:: ipython2
 
     from sppam import SPPAM
     from sklearn.datasets import make_classification
     from sklearn.model_selection import train_test_split
 
@@ -90,16 +94,19 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     cls.score(X_test, y_test)
 
 
+
+
 .. parsed-literal::
 
     1.0
 
+
 References
 ------------------
 [1] Natole Jr, Michael & Ying, Yiming & Lyu, Siwei. (2019).
 Stochastic AUC Optimization Algorithms With Linear Convergence.
 Frontiers in Applied Mathematics and Statistics. 5. 10.3389/fams.2019.00030.
```

