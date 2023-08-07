# Comparing `tmp/sppam-0.1.0.tar.gz` & `tmp/sppam-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sppam-0.1.0.tar", last modified: Mon Aug  7 20:21:32 2023, max compression
+gzip compressed data, was "sppam-0.1.2.tar", last modified: Mon Aug  7 21:40:24 2023, max compression
```

## Comparing `sppam-0.1.0.tar` & `sppam-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 20:21:32.364461 sppam-0.1.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1529 2023-08-07 20:20:27.000000 sppam-0.1.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-07 20:20:27.000000 sppam-0.1.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2982 2023-08-07 20:21:32.364461 sppam-0.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2153 2023-08-07 20:20:27.000000 sppam-0.1.0/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-08-07 20:20:27.000000 sppam-0.1.0/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-08-07 20:21:32.364461 sppam-0.1.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-08-07 20:20:27.000000 sppam-0.1.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 20:21:32.364461 sppam-0.1.0/sppam/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      145 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11206 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/sppam.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 20:21:32.364461 sppam-0.1.0/sppam/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      239 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/tests/test_common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-08-07 20:20:27.000000 sppam-0.1.0/sppam/tests/test_template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 20:21:32.364461 sppam-0.1.0/sppam.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2982 2023-08-07 20:21:32.000000 sppam-0.1.0/sppam.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      369 2023-08-07 20:21:32.000000 sppam-0.1.0/sppam.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 20:21:32.000000 sppam-0.1.0/sppam.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 20:21:16.000000 sppam-0.1.0/sppam.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-08-07 20:21:32.000000 sppam-0.1.0/sppam.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-08-07 20:21:32.000000 sppam-0.1.0/sppam.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 21:40:24.228765 sppam-0.1.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1529 2023-08-07 21:39:24.000000 sppam-0.1.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-07 21:39:24.000000 sppam-0.1.2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2982 2023-08-07 21:40:24.228765 sppam-0.1.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2153 2023-08-07 21:39:24.000000 sppam-0.1.2/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-08-07 21:39:24.000000 sppam-0.1.2/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-08-07 21:40:24.232765 sppam-0.1.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2613 2023-08-07 21:39:24.000000 sppam-0.1.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 21:40:24.228765 sppam-0.1.2/sppam/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      145 2023-08-07 21:39:24.000000 sppam-0.1.2/sppam/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-08-07 21:39:24.000000 sppam-0.1.2/sppam/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11383 2023-08-07 21:39:24.000000 sppam-0.1.2/sppam/sppam.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 21:40:24.228765 sppam-0.1.2/sppam/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-07 21:39:24.000000 sppam-0.1.2/sppam/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      239 2023-08-07 21:39:24.000000 sppam-0.1.2/sppam/tests/test_common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-08-07 21:39:24.000000 sppam-0.1.2/sppam/tests/test_template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 21:40:24.228765 sppam-0.1.2/sppam.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2982 2023-08-07 21:40:24.000000 sppam-0.1.2/sppam.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      369 2023-08-07 21:40:24.000000 sppam-0.1.2/sppam.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 21:40:24.000000 sppam-0.1.2/sppam.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 21:40:09.000000 sppam-0.1.2/sppam.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-08-07 21:40:24.000000 sppam-0.1.2/sppam.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-08-07 21:40:24.000000 sppam-0.1.2/sppam.egg-info/top_level.txt
```

### Comparing `sppam-0.1.0/LICENSE` & `sppam-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sppam-0.1.0/PKG-INFO` & `sppam-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sppam
-Version: 0.1.0
+Version: 0.1.2
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/sppam
 Download-URL: https://github.com/hrolfrc/sppam
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sppam-0.1.0/README.rst` & `sppam-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `sppam-0.1.0/setup.py` & `sppam-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `sppam-0.1.0/sppam/sppam.py` & `sppam-0.1.2/sppam/sppam.py`

 * *Files 5% similar despite different names*

```diff
@@ -169,14 +169,15 @@
             The unique class labels
 
         fit_time_ : float
             The number of seconds to fit X to y
 
         Examples
         --------
+
             >>> import numpy
             >>> from sklearn.datasets import make_classification as mc
             >>> X, y = mc(n_features=2, n_redundant=0, n_informative=2, n_clusters_per_class=1, random_state=42)
             >>> numpy.round(X[0:3, :], 2)
             array([[ 1.23, -0.76],
                    [ 0.7 , -1.38],
                    [ 2.55,  2.5 ]])
@@ -210,24 +211,24 @@
         pass
 
     def fit(self, X, y):
         """ Fit the model according to the given training data.
 
         Parameters
         ----------
-        X : {array-like, sparse matrix} of shape (n_samples, n_features)
-            Training vector, where n_samples is the number of samples and n_features is the number of features.
+            X : {array-like, sparse matrix} of shape (n_samples, n_features)
+                Training vector, where n_samples is the number of samples and n_features is the number of features.
 
-        y : array-like of shape (n_samples,)
-            Target vector relative to X.
+            y : array-like of shape (n_samples,)
+                Target vector relative to X.
 
         Returns
         -------
-        self
-            Fitted estimator.
+            self
+                Fitted estimator.
 
         """
         if y is None:
             raise ValueError('requires y to be passed, but the target y is None')
 
         X, y = check_X_y(X, y)
         self.n_features_in_ = X.shape[1]
@@ -241,20 +242,22 @@
         self.coef_ = self.w_
         self.is_fitted_ = True
         return self
 
     def decision_function(self, X):
         """ Identify confidence scores for the samples
 
-        Arguments:
+        Parameters
+        ----------
             X : array-like, shape (n_samples, n_features)
                 The training input features and samples
 
-        Returns:
-            the decision vector (n_samples)
+        Returns
+        -------
+            y_d : the decision vector (n_samples)
 
         """
         check_is_fitted(self, ['is_fitted_', 'X_', 'y_'])
 
         X = self._validate_data(X, accept_sparse="csr", reset=False)
         scores = np.array(
             minmax_scale(
@@ -263,21 +266,24 @@
             )
         )
         return scores
 
     def predict(self, X):
         """Predict class labels for samples in X.
 
-        Parameters:
+        Parameters
+        ----------
             X : {array-like, sparse matrix} of shape (n_samples, n_features)
                 The data matrix for which we want to get the predictions.
 
-        Returns:
+        Returns
+        -------
             y_pred : ndarray of shape (n_samples,)
                 Vector containing the class labels for each sample.
+
         """
         check_is_fitted(self, ['is_fitted_', 'X_', 'y_'])
         X = check_array(X)
 
         if len(self.classes_) < 2:
             y_class = self.y_
         else:
@@ -286,21 +292,23 @@
             # get the class labels
             y_class = [self.classes_[x] for x in y_class]
         return np.array(y_class)
 
     def predict_proba(self, X):
         """Probability estimates for samples in X.
 
-        Parameters:
+        Parameters
+        ----------
             X : array-like of shape (n_samples, n_features)
                 Vector to be scored, where n_samples is the number of samples and
                 n_features is the number of features.
 
-        Returns:
-            T: array-like of shape (n_samples, n_classes)
+        Returns
+        -------
+            T : array-like of shape (n_samples, n_classes)
                 Returns the probability of the sample for each class in the model,
                 where classes are ordered as they are in `self.classes_`.
 
         """
         check_is_fitted(self, ['is_fitted_', 'X_', 'y_'])
         X = check_array(X)
 
@@ -312,40 +320,44 @@
         )
         class_prob = np.column_stack((1 - y_proba, y_proba))
         return class_prob
 
     def transform(self, X):
         """ Reduce X to the features that contribute positive AUC.
 
-        Arguments:
+        Parameters
+        ----------
             X : array-like, shape (n_samples, n_features)
                 The training input features and samples
 
-        Returns:
+        Returns
+        -------
             X_r : array of shape [n_samples, n_selected_features]
-            The input samples with only the selected features.
+                The input samples with only the selected features.
 
         """
         check_is_fitted(self, ['is_fitted_', 'X_', 'y_'])
         X = check_array(X)
 
         return X[:, np.asarray(self.coef_).nonzero()]
 
     def fit_transform(self, X, y):
         """ Fit to the data, then reduce X to the features that contribute positive AUC.
 
-            Arguments:
-                X : array-like, shape (n_samples, n_features)
-                    The training input features and samples
+        Parameters
+        ----------
+            X : array-like, shape (n_samples, n_features)
+                The training input features and samples
 
-                y : array-like of shape (n_samples,)
-                    Target vector relative to X.
+            y : array-like of shape (n_samples,)
+                Target vector relative to X.
 
-            Returns:
-                X_r : array of shape [n_samples, n_selected_features]
+        Returns
+        -------
+            X_r : array of shape [n_samples, n_selected_features]
                 The input samples with only the selected features.
 
             """
         return self.fit(X, y).transform(X)
 
     def _more_tags(self):
         return {
```

### Comparing `sppam-0.1.0/sppam.egg-info/PKG-INFO` & `sppam-0.1.2/sppam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sppam
-Version: 0.1.0
+Version: 0.1.2
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/sppam
 Download-URL: https://github.com/hrolfrc/sppam
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

