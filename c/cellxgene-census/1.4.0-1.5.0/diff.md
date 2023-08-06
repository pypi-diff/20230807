# Comparing `tmp/cellxgene_census-1.4.0.tar.gz` & `tmp/cellxgene_census-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-1.4.0.tar", last modified: Fri Jul 28 18:35:37 2023, max compression
+gzip compressed data, was "cellxgene_census-1.5.0.tar", last modified: Sun Aug  6 21:56:55 2023, max compression
```

## Comparing `cellxgene_census-1.4.0.tar` & `cellxgene_census-1.5.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/release_process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.658118 cellxgene_census-1.4.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.654118 cellxgene_census-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.658118 cellxgene_census-1.4.0/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.658118 cellxgene_census-1.4.0/src/cellxgene_census/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.662118 cellxgene_census-1.4.0/src/cellxgene_census/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25110 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/ml/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.662118 cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.662118 cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/_csr_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/_eager_iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.658118 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-28 18:35:37.000000 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-28 18:35:37.000000 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:35:37.000000 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-28 18:35:37.000000 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 18:35:37.000000 cellxgene_census-1.4.0/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.662118 cellxgene_census-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    56048 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.662118 cellxgene_census-1.4.0/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/tests/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/ml/test_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/tests/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/pp/test_hvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/pp/test_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/pp/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:35:37.666118 cellxgene_census-1.4.0/tests/experimental/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/experimental/util/test_csr_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-28 18:35:22.000000 cellxgene_census-1.4.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/release_process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.310281 cellxgene_census-1.5.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.306281 cellxgene_census-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.310281 cellxgene_census-1.5.0/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.310281 cellxgene_census-1.5.0/src/cellxgene_census/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.310281 cellxgene_census-1.5.0/src/cellxgene_census/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26112 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/ml/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/_csr_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/_eager_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.310281 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-06 21:56:55.000000 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-06 21:56:55.000000 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 21:56:55.000000 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-06 21:56:55.000000 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 21:56:55.000000 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    56048 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/tests/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/ml/test_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/tests/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/pp/test_hvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/pp/test_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/pp/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/tests/experimental/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/util/test_csr_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_util.py
```

### Comparing `cellxgene_census-1.4.0/LICENSE` & `cellxgene_census-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/PKG-INFO` & `cellxgene_census-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene_census
-Version: 1.4.0
+Version: 1.5.0
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.4.0/README.md` & `cellxgene_census-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/pyproject.toml` & `cellxgene_census-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
 [project.optional-dependencies]
 experimental = [
     "torch==2.0.1",
     "torchdata==0.6.1",
     "scikit-learn==1.2.2",
     "scikit-misc==0.2.0",
+    "psutil==5.9.5",
 ]
 
 [project.urls]
 homepage = "https://github.com/chanzuckerberg/cellxgene-census"
 repository = "https://github.com/chanzuckerberg/cellxgene-census"
 
 [tool.setuptools.packages.find]
```

### Comparing `cellxgene_census-1.4.0/release_process.md` & `cellxgene_census-1.5.0/release_process.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/__init__.py` & `cellxgene_census-1.5.0/src/cellxgene_census/__init__.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.5.0/src/cellxgene_census/_experiment.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.5.0/src/cellxgene_census/_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/_open.py` & `cellxgene_census-1.5.0/src/cellxgene_census/_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.5.0/src/cellxgene_census/_presence_matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.5.0/src/cellxgene_census/_release_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/experimental/ml/pytorch.py` & `cellxgene_census-1.5.0/src/cellxgene_census/experimental/ml/pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import gc
 import logging
 import os
 from contextlib import contextmanager
 from datetime import timedelta
 from time import time
 from typing import Any, Dict, Iterator, Optional, Sequence, Tuple
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
+import psutil
 import pyarrow as pa
 import scipy
 import somacore
 import tiledbsoma as soma
 import torch
 import torchdata.datapipes.iter as pipes
 from attr import define
@@ -149,14 +151,27 @@
         stats.elapsed += int(time() - start_time)
         stats.n_soma_batches += 1
 
         pytorch_logger.debug(f"Retrieved SOMA batch: {stats}")
         return _ObsAndXSOMABatch(obs=obs_batch, X=X_batch, stats=stats)
 
 
+def run_gc() -> Tuple[Tuple[Any, Any, Any], Tuple[Any, Any, Any]]:
+    proc = psutil.Process(os.getpid())
+
+    pre_gc = proc.memory_full_info(), psutil.virtual_memory(), psutil.swap_memory()
+    gc.collect()
+    post_gc = proc.memory_full_info(), psutil.virtual_memory(), psutil.swap_memory()
+
+    pytorch_logger.debug(f"gc:  pre={pre_gc}")
+    pytorch_logger.debug(f"gc: post={post_gc}")
+
+    return pre_gc, post_gc
+
+
 class _ObsAndXIterator(Iterator[ObsAndXDatum]):
     """
     Iterates through a set of ``obs`` and corresponding ``X`` rows, where the rows to be returned are specified by
     the ``obs_tables_iter`` argument. For the specified ``obs` rows, the corresponding ``X`` data is loaded and
     joined together. It is returned from this iterator as 2-tuples of ``X`` and obs Tensors.
 
     Internally manages the retrieval of data in SOMA-sized batches, fetching the next batch of SOMA data as needed.
@@ -189,14 +204,15 @@
             self.soma_batch_iter = _EagerIterator(self.soma_batch_iter)
         self.soma_batch = None
         self.var_joinids = var_joinids
         self.batch_size = batch_size
         self.return_sparse_X = return_sparse_X
         self.encoders = encoders
         self.stats = stats
+        self.max_process_mem_usage_bytes = 0
 
     def __next__(self) -> ObsAndXDatum:
         """Read the next torch batch, possibly across multiple soma batches"""
 
         obs: pd.DataFrame = pd.DataFrame()
         X: sparse.csr_matrix = sparse.csr_matrix((0, len(self.var_joinids)))
 
@@ -241,14 +257,19 @@
 
     def _read_partial_torch_batch(self, batch_size: int) -> ObsAndXDatum:
         """Reads a torch-size batch of data from the current SOMA batch, returning a torch-size batch whose size may
         contain fewer rows than the requested ``batch_size``. This can happen when the remaining rows in the current
         SOMA batch are fewer than the requested ``batch_size``."""
 
         if self.soma_batch is None or not (0 <= self.i < len(self.soma_batch)):
+            # GC memory from previous soma_batch
+            self.soma_batch = None
+            mem_info = run_gc()
+            self.max_process_mem_usage_bytes = max(self.max_process_mem_usage_bytes, mem_info[0][0].uss)
+
             self.soma_batch: _ObsAndXSOMABatch = next(self.soma_batch_iter)
             self.stats += self.soma_batch.stats
             self.i = 0
 
             pytorch_logger.debug(f"Retrieved SOMA batch totals: {self.stats}")
 
         obs_batch = self.soma_batch.obs
@@ -464,14 +485,15 @@
                 "torch does not work with sparse tensors in multi-processing mode "
                 "(see https://github.com/pytorch/pytorch/issues/20248)"
             )
 
         with _open_experiment(self.exp_uri, self.aws_region, soma_buffer_bytes=self.soma_buffer_bytes) as exp:
             X: soma.SparseNDArray = exp.ms[self.measurement_name].X[self.layer_name]
 
+            # TODO: Get all IDs, close experiment. Iterate through obs IDs using custom stride, not based upon soma_buffer_bytes
             obs_tables_iter = exp.obs.read(
                 coords=(self._partition_obs_joinids(self._obs_joinids),),
                 batch_size=somacore.BatchSize(),
                 column_names=self.obs_column_names,
             )
 
             obs_and_x_iter = _ObsAndXIterator(
@@ -484,14 +506,18 @@
                 return_sparse_X=self.return_sparse_X,
                 use_eager_fetch=self.use_eager_fetch,
             )
 
             for datum_ in obs_and_x_iter:
                 yield datum_
 
+            pytorch_logger.debug(
+                "max process memory usage=" f"{obs_and_x_iter.max_process_mem_usage_bytes / (1024 ** 3):.3f} GiB"
+            )
+
     def __len__(self) -> int:
         self._init()
         assert self._obs_joinids is not None
 
         return len(self._obs_joinids)
 
     def __getitem__(self, index: int) -> ObsAndXDatum:
```

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py` & `cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/_online.py` & `cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_online.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/experimental/pp/_stats.py` & `cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_stats.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/_csr_iter.py` & `cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/_csr_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census/experimental/util/_eager_iter.py` & `cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/_eager_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.5.0/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-census
-Version: 1.4.0
+Version: 1.5.0
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.4.0/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.5.0/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/README.md` & `cellxgene_census-1.5.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/conftest.py` & `cellxgene_census-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/experimental/ml/test_pytorch.py` & `cellxgene_census-1.5.0/tests/experimental/ml/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/experimental/pp/test_hvg.py` & `cellxgene_census-1.5.0/tests/experimental/pp/test_hvg.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/experimental/pp/test_online.py` & `cellxgene_census-1.5.0/tests/experimental/pp/test_online.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/experimental/pp/test_stats.py` & `cellxgene_census-1.5.0/tests/experimental/pp/test_stats.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/experimental/util/test_csr_iter.py` & `cellxgene_census-1.5.0/tests/experimental/util/test_csr_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/test_acceptance.py` & `cellxgene_census-1.5.0/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/test_directory.py` & `cellxgene_census-1.5.0/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/test_get_anndata.py` & `cellxgene_census-1.5.0/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/test_get_helpers.py` & `cellxgene_census-1.5.0/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/test_open.py` & `cellxgene_census-1.5.0/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.4.0/tests/test_util.py` & `cellxgene_census-1.5.0/tests/test_util.py`

 * *Files identical despite different names*

