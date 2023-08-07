# Comparing `tmp/rpy_symmetry-0.0.1.tar.gz` & `tmp/rpy_symmetry-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpy_symmetry-0.0.1.tar", last modified: Fri Aug  4 16:34:43 2023, max compression
+gzip compressed data, was "rpy_symmetry-0.0.2.tar", last modified: Mon Aug  7 10:31:20 2023, max compression
```

## Comparing `rpy_symmetry-0.0.1.tar` & `rpy_symmetry-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:34:43.616250 rpy_symmetry-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-04 16:34:43.616250 rpy_symmetry-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-04 16:34:28.000000 rpy_symmetry-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-04 16:34:28.000000 rpy_symmetry-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:34:43.616250 rpy_symmetry-0.0.1/rpy_symmetry/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 16:34:28.000000 rpy_symmetry-0.0.1/rpy_symmetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-04 16:34:28.000000 rpy_symmetry-0.0.1/rpy_symmetry/rpy_symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:34:43.616250 rpy_symmetry-0.0.1/rpy_symmetry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-04 16:34:43.000000 rpy_symmetry-0.0.1/rpy_symmetry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-04 16:34:43.000000 rpy_symmetry-0.0.1/rpy_symmetry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:34:43.000000 rpy_symmetry-0.0.1/rpy_symmetry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 16:34:43.000000 rpy_symmetry-0.0.1/rpy_symmetry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 16:34:43.000000 rpy_symmetry-0.0.1/rpy_symmetry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:34:43.616250 rpy_symmetry-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:34:43.616250 rpy_symmetry-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-04 16:34:28.000000 rpy_symmetry-0.0.1/tests/test_basics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:20.485591 rpy_symmetry-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-07 10:31:20.481591 rpy_symmetry-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-07 10:31:04.000000 rpy_symmetry-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-07 10:31:04.000000 rpy_symmetry-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:20.481591 rpy_symmetry-0.0.2/rpy_symmetry/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 10:31:04.000000 rpy_symmetry-0.0.2/rpy_symmetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-08-07 10:31:04.000000 rpy_symmetry-0.0.2/rpy_symmetry/rpy_symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:20.481591 rpy_symmetry-0.0.2/rpy_symmetry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-07 10:31:20.000000 rpy_symmetry-0.0.2/rpy_symmetry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-07 10:31:20.000000 rpy_symmetry-0.0.2/rpy_symmetry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:31:20.000000 rpy_symmetry-0.0.2/rpy_symmetry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 10:31:20.000000 rpy_symmetry-0.0.2/rpy_symmetry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 10:31:20.000000 rpy_symmetry-0.0.2/rpy_symmetry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:31:20.485591 rpy_symmetry-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:20.481591 rpy_symmetry-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-07 10:31:04.000000 rpy_symmetry-0.0.2/tests/test_basics.py
```

### Comparing `rpy_symmetry-0.0.1/README.md` & `rpy_symmetry-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 
 
 By default, the Symmetry test uses the one from:
 
     Mira A (1999) Distribution-free test for symmetry based on Bonferroni's measure. J Appl Stat 26(8):959–972. https://doi.org/10.1080/02664769921963
 
 ## Requirements
-`R` needs to be installed (`conda install -c conda-forge r-base r-essentials`). The python interface is built on [`rpy2`](https://rpy2.github.io/).
+`R` needs to be installed (`conda install -c conda-forge r-essentials`). The python interface is built on [`rpy2`](https://rpy2.github.io/).
 
 ## Examples
 See example notebook
```

### Comparing `rpy_symmetry-0.0.1/pyproject.toml` & `rpy_symmetry-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "rpy_symmetry"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
     "numpy",
     "rpy2",
 ]
 
 [metadata]
 author ='Joran R. Angevaare'
```

### Comparing `rpy_symmetry-0.0.1/rpy_symmetry/rpy_symmetry.py` & `rpy_symmetry-0.0.2/rpy_symmetry/rpy_symmetry.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,19 +54,25 @@
                 f'_install_package_on_the_fly(\'{name}\')"'
             )
     return rpackages.importr(name)
 
 
 def _install_package_on_the_fly(package: str) -> None:
     from rpy2.robjects.vectors import StrVector
+    from rpy2.rinterface_lib.embedded import RRuntimeError
 
     utils = rpackages.importr('utils')
     packnames = (package,)
     utils.chooseCRANmirror(ind=1)
-    utils.install_packages(StrVector(packnames))
+    try:
+        utils.install_packages(StrVector(packnames))
+    except RRuntimeError as e:
+        raise RuntimeError(
+            f'Cannot install {package} on the fly, please make sure that R is properly installed'
+        ) from e
 
 
 def _float_or_str(x) -> ty.Union[str, float]:
     """Try making x a float, or a string otherwise"""
     try:
         return float(x)
     except ValueError:
```

