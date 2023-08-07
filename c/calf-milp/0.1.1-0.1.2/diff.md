# Comparing `tmp/calf_milp-0.1.1.tar.gz` & `tmp/calf_milp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calf_milp-0.1.1.tar", last modified: Mon Aug  7 18:20:01 2023, max compression
+gzip compressed data, was "calf_milp-0.1.2.tar", last modified: Mon Aug  7 18:34:00 2023, max compression
```

## Comparing `calf_milp-0.1.1.tar` & `calf_milp-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:20:01.404865 calf_milp-0.1.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2023-08-07 18:17:50.000000 calf_milp-0.1.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-07 18:17:50.000000 calf_milp-0.1.1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2632 2023-08-07 18:20:01.404865 calf_milp-0.1.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1791 2023-08-07 18:17:50.000000 calf_milp-0.1.1/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:20:01.404865 calf_milp-0.1.1/calf_milp/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13219 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/calf_milp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:20:01.404865 calf_milp-0.1.1/calf_milp/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/tests/test_common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/tests/test_template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:20:01.404865 calf_milp-0.1.1/calf_milp.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2632 2023-08-07 18:20:01.000000 calf_milp-0.1.1/calf_milp.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      421 2023-08-07 18:20:01.000000 calf_milp-0.1.1/calf_milp.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 18:20:01.000000 calf_milp-0.1.1/calf_milp.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 18:18:40.000000 calf_milp-0.1.1/calf_milp.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-08-07 18:20:01.000000 calf_milp-0.1.1/calf_milp.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-08-07 18:20:01.000000 calf_milp-0.1.1/calf_milp.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-08-07 18:17:50.000000 calf_milp-0.1.1/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-08-07 18:20:01.404865 calf_milp-0.1.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-08-07 18:17:50.000000 calf_milp-0.1.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:34:00.365724 calf_milp-0.1.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2023-08-07 18:31:46.000000 calf_milp-0.1.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-07 18:31:46.000000 calf_milp-0.1.2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2632 2023-08-07 18:34:00.365724 calf_milp-0.1.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1791 2023-08-07 18:31:46.000000 calf_milp-0.1.2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:34:00.361724 calf_milp-0.1.2/calf_milp/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13268 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/calf_milp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:34:00.365724 calf_milp-0.1.2/calf_milp/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/tests/test_common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-08-07 18:31:46.000000 calf_milp-0.1.2/calf_milp/tests/test_template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:34:00.365724 calf_milp-0.1.2/calf_milp.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2632 2023-08-07 18:34:00.000000 calf_milp-0.1.2/calf_milp.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      421 2023-08-07 18:34:00.000000 calf_milp-0.1.2/calf_milp.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 18:34:00.000000 calf_milp-0.1.2/calf_milp.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 18:32:36.000000 calf_milp-0.1.2/calf_milp.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-08-07 18:34:00.000000 calf_milp-0.1.2/calf_milp.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-08-07 18:34:00.000000 calf_milp-0.1.2/calf_milp.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-08-07 18:31:46.000000 calf_milp-0.1.2/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-08-07 18:34:00.365724 calf_milp-0.1.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-08-07 18:31:46.000000 calf_milp-0.1.2/setup.py
```

### Comparing `calf_milp-0.1.1/LICENSE` & `calf_milp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calf_milp-0.1.1/PKG-INFO` & `calf_milp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calf_milp
-Version: 0.1.1
+Version: 0.1.2
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/calf-milp
 Download-URL: https://github.com/hrolfrc/calf-milp
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `calf_milp-0.1.1/README.rst` & `calf_milp-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `calf_milp-0.1.1/calf_milp/calf_milp.py` & `calf_milp-0.1.2/calf_milp/calf_milp.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,14 +397,15 @@
         """ Fit to the data, then reduce X to the features that contribute positive AUC.
 
             Arguments:
                 X : array-like, shape (n_samples, n_features)
                     The training input features and samples
 
                 y : array-like of shape (n_samples,)
+                    Target vector relative to X.
 
             Returns:
                 X_r : array of shape [n_samples, n_selected_features]
                 The input samples with only the selected features.
 
             """
         return self.fit(X, y).transform(X)
```

### Comparing `calf_milp-0.1.1/calf_milp.egg-info/PKG-INFO` & `calf_milp-0.1.2/calf_milp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calf-milp
-Version: 0.1.1
+Version: 0.1.2
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/calf-milp
 Download-URL: https://github.com/hrolfrc/calf-milp
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `calf_milp-0.1.1/setup.py` & `calf_milp-0.1.2/setup.py`

 * *Files identical despite different names*

