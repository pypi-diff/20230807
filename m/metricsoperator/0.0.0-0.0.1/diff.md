# Comparing `tmp/metricsoperator-0.0.0.tar.gz` & `tmp/metricsoperator-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricsoperator-0.0.0.tar", last modified: Sun Aug  6 22:06:51 2023, max compression
+gzip compressed data, was "metricsoperator-0.0.1.tar", last modified: Sun Aug  6 22:28:27 2023, max compression
```

## Comparing `metricsoperator-0.0.0.tar` & `metricsoperator-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-06 22:06:51.289982 metricsoperator-0.0.0/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      169 2023-08-06 22:03:40.000000 metricsoperator-0.0.0/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1953 2023-08-06 22:06:51.289982 metricsoperator-0.0.0/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1099 2023-08-06 22:06:46.000000 metricsoperator-0.0.0/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-06 22:06:51.289982 metricsoperator-0.0.0/metricsoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       44 2023-08-06 22:03:40.000000 metricsoperator-0.0.0/metricsoperator/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1535 2023-08-06 22:03:40.000000 metricsoperator-0.0.0/metricsoperator/client.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-06 22:06:51.289982 metricsoperator-0.0.0/metricsoperator/metrics/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      375 2023-08-06 22:03:40.000000 metricsoperator-0.0.0/metricsoperator/metrics/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6678 2023-08-06 22:03:40.000000 metricsoperator-0.0.0/metricsoperator/metrics/base.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      930 2023-08-06 22:03:40.000000 metricsoperator-0.0.0/metricsoperator/metrics/storage.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      372 2023-08-06 22:03:40.000000 metricsoperator-0.0.0/metricsoperator/utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-06 22:06:51.289982 metricsoperator-0.0.0/metricsoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1953 2023-08-06 22:06:51.000000 metricsoperator-0.0.0/metricsoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      459 2023-08-06 22:06:51.000000 metricsoperator-0.0.0/metricsoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-08-06 22:06:51.000000 metricsoperator-0.0.0/metricsoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-08-06 04:14:56.000000 metricsoperator-0.0.0/metricsoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       27 2023-08-06 22:06:51.000000 metricsoperator-0.0.0/metricsoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       16 2023-08-06 22:06:51.000000 metricsoperator-0.0.0/metricsoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-08-06 22:03:40.000000 metricsoperator-0.0.0/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       38 2023-08-06 22:06:51.289982 metricsoperator-0.0.0/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2256 2023-08-06 22:03:40.000000 metricsoperator-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:28:27.380470 metricsoperator-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-06 22:28:27.380470 metricsoperator-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:28:27.376469 metricsoperator-0.0.1/metricsoperator/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:28:27.380470 metricsoperator-0.0.1/metricsoperator/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/metrics/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:28:27.380470 metricsoperator-0.0.1/metricsoperator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 22:28:27.380470 metricsoperator-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/setup.py
```

### Comparing `metricsoperator-0.0.0/PKG-INFO` & `metricsoperator-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: metricsoperator
-Version: 0.0.0
+Version: 0.0.1
 Summary: Python helpers for the Metrics Operator
 Home-page: https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: metrics-operator,hpc,kubernetes,metrics,storage,applications
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -38,8 +37,7 @@
 See [LICENSE](https://github.com/converged-computing/cloud-select/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/cloud-select/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/cloud-select/blob/main/NOTICE) for details.
 
 SPDX-License-Identifier: (MIT)
 
 LLNL-CODE- 842614
-
```

### Comparing `metricsoperator-0.0.0/README.md` & `metricsoperator-0.0.1/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 
 See [LICENSE](https://github.com/converged-computing/cloud-select/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/cloud-select/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/cloud-select/blob/main/NOTICE) for details.
 
 SPDX-License-Identifier: (MIT)
 
-LLNL-CODE- 842614
+LLNL-CODE- 842614
```

### Comparing `metricsoperator-0.0.0/metricsoperator/client.py` & `metricsoperator-0.0.1/metricsoperator/client.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.0/metricsoperator/metrics/base.py` & `metricsoperator-0.0.1/metricsoperator/metrics/base.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.0/metricsoperator/metrics/storage.py` & `metricsoperator-0.0.1/metricsoperator/metrics/storage.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.0/metricsoperator.egg-info/PKG-INFO` & `metricsoperator-0.0.1/metricsoperator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: metricsoperator
-Version: 0.0.0
+Version: 0.0.1
 Summary: Python helpers for the Metrics Operator
 Home-page: https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: metrics-operator,hpc,kubernetes,metrics,storage,applications
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -38,8 +37,7 @@
 See [LICENSE](https://github.com/converged-computing/cloud-select/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/cloud-select/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/cloud-select/blob/main/NOTICE) for details.
 
 SPDX-License-Identifier: (MIT)
 
 LLNL-CODE- 842614
-
```

### Comparing `metricsoperator-0.0.0/setup.py` & `metricsoperator-0.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="metricsoperator",
-        version="0.0.0",
+        version="0.0.1",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1",
```

