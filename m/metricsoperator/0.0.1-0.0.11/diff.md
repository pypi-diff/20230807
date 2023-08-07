# Comparing `tmp/metricsoperator-0.0.1.tar.gz` & `tmp/metricsoperator-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricsoperator-0.0.1.tar", last modified: Sun Aug  6 22:28:27 2023, max compression
+gzip compressed data, was "metricsoperator-0.0.11.tar", last modified: Mon Aug  7 05:12:33 2023, max compression
```

## Comparing `metricsoperator-0.0.1.tar` & `metricsoperator-0.0.11.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:28:27.380470 metricsoperator-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-06 22:28:27.380470 metricsoperator-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:28:27.376469 metricsoperator-0.0.1/metricsoperator/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:28:27.380470 metricsoperator-0.0.1/metricsoperator/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/metrics/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/metricsoperator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:28:27.380470 metricsoperator-0.0.1/metricsoperator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 22:28:27.000000 metricsoperator-0.0.1/metricsoperator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 22:28:27.380470 metricsoperator-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-08-06 22:27:44.000000 metricsoperator-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/metricsoperator/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/metricsoperator/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/metrics/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/metrics/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/metricsoperator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/metricsoperator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 05:12:33.000000 metricsoperator-0.0.11/metricsoperator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 05:12:33.733519 metricsoperator-0.0.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-08-07 05:12:02.000000 metricsoperator-0.0.11/setup.py
```

### Comparing `metricsoperator-0.0.1/PKG-INFO` & `metricsoperator-0.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metricsoperator
-Version: 0.0.1
+Version: 0.0.11
 Summary: Python helpers for the Metrics Operator
 Home-page: https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: metrics-operator,hpc,kubernetes,metrics,storage,applications
```

### Comparing `metricsoperator-0.0.1/README.md` & `metricsoperator-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.1/metricsoperator/client.py` & `metricsoperator-0.0.11/metricsoperator/client.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.1/metricsoperator/metrics/base.py` & `metricsoperator-0.0.11/metricsoperator/metrics/base.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.1/metricsoperator/metrics/storage.py` & `metricsoperator-0.0.11/metricsoperator/metrics/storage.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.1/metricsoperator.egg-info/PKG-INFO` & `metricsoperator-0.0.11/metricsoperator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metricsoperator
-Version: 0.0.1
+Version: 0.0.11
 Summary: Python helpers for the Metrics Operator
 Home-page: https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: metrics-operator,hpc,kubernetes,metrics,storage,applications
```

### Comparing `metricsoperator-0.0.1/setup.py` & `metricsoperator-0.0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="metricsoperator",
-        version="0.0.1",
+        version="0.0.11",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1",
```

