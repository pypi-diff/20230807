# Comparing `tmp/calf_milp-0.1.2.tar.gz` & `tmp/calf_milp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calf_milp-0.1.2.tar", last modified: Mon Aug  7 18:34:00 2023, max compression
+gzip compressed data, was "calf_milp-0.1.3.tar", last modified: Mon Aug  7 21:43:42 2023, max compression
```

## Comparing `calf_milp-0.1.2.tar` & `calf_milp-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:34:00.365724 calf_milp-0.1.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2023-08-07 18:31:46.000000 calf_milp-0.1.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-07 18:31:46.000000 calf_milp-0.1.2/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2632 2023-08-07 18:34:00.365724 calf_milp-0.1.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1791 2023-08-07 18:31:46.000000 calf_milp-0.1.2/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:34:00.361724 calf_milp-0.1.2/calf_milp/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13268 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/calf_milp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:34:00.365724 calf_milp-0.1.2/calf_milp/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/tests/test_common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/tests/test_template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:34:00.365724 calf_milp-0.1.2/calf_milp.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2632 2023-08-07 18:34:00.000000 calf_milp-0.1.2/calf_milp.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      421 2023-08-07 18:34:00.000000 calf_milp-0.1.2/calf_milp.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 18:34:00.000000 calf_milp-0.1.2/calf_milp.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 18:32:36.000000 calf_milp-0.1.2/calf_milp.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-08-07 18:34:00.000000 calf_milp-0.1.2/calf_milp.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-08-07 18:34:00.000000 calf_milp-0.1.2/calf_milp.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-08-07 18:31:46.000000 calf_milp-0.1.2/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-08-07 18:34:00.365724 calf_milp-0.1.2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-08-07 18:31:46.000000 calf_milp-0.1.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 21:43:42.040400 calf_milp-0.1.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2023-08-07 21:41:27.000000 calf_milp-0.1.3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-07 21:41:27.000000 calf_milp-0.1.3/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2632 2023-08-07 21:43:42.040400 calf_milp-0.1.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1791 2023-08-07 21:41:27.000000 calf_milp-0.1.3/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 21:43:42.040400 calf_milp-0.1.3/calf_milp/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2023-08-07 21:41:27.000000 calf_milp-0.1.3/calf_milp/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-08-07 21:41:27.000000 calf_milp-0.1.3/calf_milp/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13264 2023-08-07 21:41:27.000000 calf_milp-0.1.3/calf_milp/calf_milp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 21:43:42.040400 calf_milp-0.1.3/calf_milp/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-07 21:41:27.000000 calf_milp-0.1.3/calf_milp/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-08-07 21:41:27.000000 calf_milp-0.1.3/calf_milp/tests/test_common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-08-07 21:41:27.000000 calf_milp-0.1.3/calf_milp/tests/test_template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 21:43:42.040400 calf_milp-0.1.3/calf_milp.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2632 2023-08-07 21:43:42.000000 calf_milp-0.1.3/calf_milp.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      421 2023-08-07 21:43:42.000000 calf_milp-0.1.3/calf_milp.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 21:43:42.000000 calf_milp-0.1.3/calf_milp.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 21:42:20.000000 calf_milp-0.1.3/calf_milp.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-08-07 21:43:42.000000 calf_milp-0.1.3/calf_milp.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-08-07 21:43:42.000000 calf_milp-0.1.3/calf_milp.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-08-07 21:41:27.000000 calf_milp-0.1.3/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-08-07 21:43:42.040400 calf_milp-0.1.3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-08-07 21:41:27.000000 calf_milp-0.1.3/setup.py
```

### Comparing `calf_milp-0.1.2/LICENSE` & `calf_milp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calf_milp-0.1.2/PKG-INFO` & `calf_milp-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calf_milp
-Version: 0.1.2
+Version: 0.1.3
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/calf-milp
 Download-URL: https://github.com/hrolfrc/calf-milp
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `calf_milp-0.1.2/README.rst` & `calf_milp-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `calf_milp-0.1.2/calf_milp/calf_milp.py` & `calf_milp-0.1.3/calf_milp/calf_milp.py`

 * *Files identical despite different names*

```diff
@@ -295,16 +295,16 @@
         self.X_ = X
         self.y_ = y
 
         # fit and time the fit
         start = time.time()
         self.w_, self.status_ = sat_weights(X, y)
         self.fit_time_ = time.time() - start
-        self.is_fitted_ = True
         self.coef_ = self.w_
+        self.is_fitted_ = True
         return self
 
     def decision_function(self, X):
         """ Identify confidence scores for the samples
 
         Arguments:
             X : array-like, shape (n_samples, n_features)
@@ -359,15 +359,15 @@
 
         Returns:
 
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
```

### Comparing `calf_milp-0.1.2/calf_milp.egg-info/PKG-INFO` & `calf_milp-0.1.3/calf_milp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calf-milp
-Version: 0.1.2
+Version: 0.1.3
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/calf-milp
 Download-URL: https://github.com/hrolfrc/calf-milp
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `calf_milp-0.1.2/setup.py` & `calf_milp-0.1.3/setup.py`

 * *Files identical despite different names*

