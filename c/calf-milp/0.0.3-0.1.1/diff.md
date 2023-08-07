# Comparing `tmp/calf_milp-0.0.3.tar.gz` & `tmp/calf_milp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calf_milp-0.0.3.tar", last modified: Sat Aug  5 04:28:44 2023, max compression
+gzip compressed data, was "calf_milp-0.1.1.tar", last modified: Mon Aug  7 18:20:01 2023, max compression
```

## Comparing `calf_milp-0.0.3.tar` & `calf_milp-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:28:44.296071 calf_milp-0.0.3/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-08-02 13:53:45.000000 calf_milp-0.0.3/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-08-02 13:53:45.000000 calf_milp-0.0.3/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2476 2023-08-05 04:28:44.296071 calf_milp-0.0.3/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1630 2023-08-05 04:27:42.000000 calf_milp-0.0.3/README.rst
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:28:44.292071 calf_milp-0.0.3/calf_milp/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      167 2023-08-02 14:23:44.000000 calf_milp-0.0.3/calf_milp/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-05 04:27:42.000000 calf_milp-0.0.3/calf_milp/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     4222 2023-08-02 14:44:06.000000 calf_milp-0.0.3/calf_milp/calf_milp.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8277 2023-07-25 20:07:15.000000 calf_milp-0.0.3/calf_milp/calf_sat.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:28:44.296071 calf_milp-0.0.3/calf_milp/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-08-02 13:53:45.000000 calf_milp-0.0.3/calf_milp/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      243 2023-08-02 14:24:00.000000 calf_milp-0.0.3/calf_milp/tests/test_common.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      402 2023-08-02 14:44:06.000000 calf_milp-0.0.3/calf_milp/tests/test_template.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-05 04:28:44.296071 calf_milp-0.0.3/calf_milp.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2476 2023-08-05 04:28:44.000000 calf_milp-0.0.3/calf_milp.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      443 2023-08-05 04:28:44.000000 calf_milp-0.0.3/calf_milp.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 04:28:44.000000 calf_milp-0.0.3/calf_milp.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-05 04:20:13.000000 calf_milp-0.0.3/calf_milp.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-05 04:28:44.000000 calf_milp-0.0.3/calf_milp.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       10 2023-08-05 04:28:44.000000 calf_milp-0.0.3/calf_milp.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      142 2023-08-02 13:53:45.000000 calf_milp-0.0.3/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-05 04:28:44.296071 calf_milp-0.0.3/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2641 2023-08-02 14:41:03.000000 calf_milp-0.0.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:20:01.404865 calf_milp-0.1.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2023-08-07 18:17:50.000000 calf_milp-0.1.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-07 18:17:50.000000 calf_milp-0.1.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2632 2023-08-07 18:20:01.404865 calf_milp-0.1.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1791 2023-08-07 18:17:50.000000 calf_milp-0.1.1/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:20:01.404865 calf_milp-0.1.1/calf_milp/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13219 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/calf_milp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:20:01.404865 calf_milp-0.1.1/calf_milp/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/tests/test_common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-08-07 18:17:50.000000 calf_milp-0.1.1/calf_milp/tests/test_template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-07 18:20:01.404865 calf_milp-0.1.1/calf_milp.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2632 2023-08-07 18:20:01.000000 calf_milp-0.1.1/calf_milp.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      421 2023-08-07 18:20:01.000000 calf_milp-0.1.1/calf_milp.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 18:20:01.000000 calf_milp-0.1.1/calf_milp.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-07 18:18:40.000000 calf_milp-0.1.1/calf_milp.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-08-07 18:20:01.000000 calf_milp-0.1.1/calf_milp.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-08-07 18:20:01.000000 calf_milp-0.1.1/calf_milp.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-08-07 18:17:50.000000 calf_milp-0.1.1/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      148 2023-08-07 18:20:01.404865 calf_milp-0.1.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-08-07 18:17:50.000000 calf_milp-0.1.1/setup.py
```

### Comparing `calf_milp-0.0.3/LICENSE` & `calf_milp-0.1.1/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2016, Vighnesh Birodkar and scikit-learn-contrib contributors
+Copyright (c) 2023, Carlson Research, LLC
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `calf_milp-0.0.3/PKG-INFO` & `calf_milp-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: calf_milp
-Version: 0.0.3
+Version: 0.1.1
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/calf-milp
 Download-URL: https://github.com/hrolfrc/calf-milp
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
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calf-milp.svg?style=shield
+.. _CircleCI: https://circleci.com/gh/hrolfrc/calf-milp
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calf-milp/badge/?version=latest
 .. _ReadTheDocs: https://calf-milp.readthedocs.io/en/latest/?badge=latest
 
-CalfMilp - A classifier with integer weights
-=============================================
+CalfMilp
+#####################################
 
-A binomial classifier that fits using mixed integer linear programming.
+CalfMilp is a binomial classifier that implements a course approximation linear function by mixed integer linear programming.
 
 Contact
 ------------------
 Rolf Carlson hrolfrc@gmail.com
 
 Install
 ------------------
@@ -47,24 +50,24 @@
 CalfMilp provides classification and prediction for two classes, the binomial case.  Small problems are supported.  This is research code and a work in progress.
 
 CalfMilp is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
 Example
-------------------
+===========
 
 .. code:: ipython2
 
-    from calf-milp import CalfMilp
+    from calf_milp import CalfMilp
     from sklearn.datasets import make_classification
     from sklearn.model_selection import train_test_split
 
 Make a classification problem
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     seed = 42
     X, y = make_classification(
         n_samples=30,
         n_features=5,
@@ -86,10 +89,14 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     cls.score(X_test, y_test)
 
 
+
+
 .. parsed-literal::
 
-    1.0
+    0.875
+
+
```

### Comparing `calf_milp-0.0.3/README.rst` & `calf_milp-0.1.1/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 .. -*- mode: rst -*-
 
-|ReadTheDocs|_
+|CircleCI|_ |ReadTheDocs|_
+
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calf-milp.svg?style=shield
+.. _CircleCI: https://circleci.com/gh/hrolfrc/calf-milp
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calf-milp/badge/?version=latest
 .. _ReadTheDocs: https://calf-milp.readthedocs.io/en/latest/?badge=latest
 
-CalfMilp - A classifier with integer weights
-=============================================
+CalfMilp
+#####################################
 
-A binomial classifier that fits using mixed integer linear programming.
+CalfMilp is a binomial classifier that implements a course approximation linear function by mixed integer linear programming.
 
 Contact
 ------------------
 Rolf Carlson hrolfrc@gmail.com
 
 Install
 ------------------
@@ -25,24 +28,24 @@
 CalfMilp provides classification and prediction for two classes, the binomial case.  Small problems are supported.  This is research code and a work in progress.
 
 CalfMilp is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
 Example
-------------------
+===========
 
 .. code:: ipython2
 
-    from calf-milp import CalfMilp
+    from calf_milp import CalfMilp
     from sklearn.datasets import make_classification
     from sklearn.model_selection import train_test_split
 
 Make a classification problem
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     seed = 42
     X, y = make_classification(
         n_samples=30,
         n_features=5,
@@ -64,10 +67,14 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     cls.score(X_test, y_test)
 
 
+
+
 .. parsed-literal::
 
-    1.0
+    0.875
+
+
```

### Comparing `calf_milp-0.0.3/calf_milp.egg-info/PKG-INFO` & `calf_milp-0.1.1/calf_milp.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: calf-milp
-Version: 0.0.3
+Version: 0.1.1
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/calf-milp
 Download-URL: https://github.com/hrolfrc/calf-milp
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
+.. |CircleCI| image:: https://circleci.com/gh/hrolfrc/calf-milp.svg?style=shield
+.. _CircleCI: https://circleci.com/gh/hrolfrc/calf-milp
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/calf-milp/badge/?version=latest
 .. _ReadTheDocs: https://calf-milp.readthedocs.io/en/latest/?badge=latest
 
-CalfMilp - A classifier with integer weights
-=============================================
+CalfMilp
+#####################################
 
-A binomial classifier that fits using mixed integer linear programming.
+CalfMilp is a binomial classifier that implements a course approximation linear function by mixed integer linear programming.
 
 Contact
 ------------------
 Rolf Carlson hrolfrc@gmail.com
 
 Install
 ------------------
@@ -47,24 +50,24 @@
 CalfMilp provides classification and prediction for two classes, the binomial case.  Small problems are supported.  This is research code and a work in progress.
 
 CalfMilp is designed for use with scikit-learn_ pipelines and composite estimators.
 
 .. _scikit-learn: https://scikit-learn.org
 
 Example
-------------------
+===========
 
 .. code:: ipython2
 
-    from calf-milp import CalfMilp
+    from calf_milp import CalfMilp
     from sklearn.datasets import make_classification
     from sklearn.model_selection import train_test_split
 
 Make a classification problem
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     seed = 42
     X, y = make_classification(
         n_samples=30,
         n_features=5,
@@ -86,10 +89,14 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: ipython2
 
     cls.score(X_test, y_test)
 
 
+
+
 .. parsed-literal::
 
-    1.0
+    0.875
+
+
```

### Comparing `calf_milp-0.0.3/setup.py` & `calf_milp-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 DOWNLOAD_URL = 'https://github.com/hrolfrc/calf-milp'
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

