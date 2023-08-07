# Comparing `tmp/corals-0.1.5.tar.gz` & `tmp/corals-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corals-0.1.5.tar", last modified: Mon Mar  6 15:44:43 2023, max compression
+gzip compressed data, was "corals-0.1.6.tar", last modified: Mon Aug  7 07:52:24 2023, max compression
```

## Comparing `corals-0.1.5.tar` & `corals-0.1.6.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.819286 corals-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-06 15:44:18.000000 corals-0.1.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.803285 corals-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.807286 corals-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-03-06 15:44:18.000000 corals-0.1.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-06 15:44:18.000000 corals-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-06 15:44:18.000000 corals-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-06 15:44:18.000000 corals-0.1.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-03-06 15:44:43.819286 corals-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-03-06 15:44:18.000000 corals-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.807286 corals-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-06 15:44:18.000000 corals-0.1.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.811286 corals-0.1.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-06 15:44:18.000000 corals-0.1.5/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 15:44:18.000000 corals-0.1.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-06 15:44:18.000000 corals-0.1.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-03-06 15:44:18.000000 corals-0.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-03-06 15:44:18.000000 corals-0.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-06 15:44:18.000000 corals-0.1.5/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.811286 corals-0.1.5/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-03-06 15:44:18.000000 corals-0.1.5/docs/notebooks/full.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-03-06 15:44:18.000000 corals-0.1.5/docs/notebooks/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-06 15:44:18.000000 corals-0.1.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-06 15:44:18.000000 corals-0.1.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-06 15:44:18.000000 corals-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-06 15:44:43.823286 corals-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-06 15:44:18.000000 corals-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.803285 corals-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.811286 corals-0.1.5/src/corals/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.811286 corals-0.1.5/src/corals/_experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/_experimental/test_correlation_topk.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/_experimental/test_joblib_context_size_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/_experimental/test_joblib_context_size_large_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/_experimental/test_presorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/_experimental/test_topk_reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.811286 corals-0.1.5/src/corals/correlation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.811286 corals-0.1.5/src/corals/correlation/full/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.811286 corals-0.1.5/src/corals/correlation/full/_deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/full/_deprecated/original.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/full/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/full/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/full/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/full/matmul.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.815286 corals-0.1.5/src/corals/correlation/threshold/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.815286 corals-0.1.5/src/corals/correlation/threshold/_deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/threshold/_deprecated/original.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/threshold/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/threshold/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.815286 corals-0.1.5/src/corals/correlation/topk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.815286 corals-0.1.5/src/corals/correlation/topk/_deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/_deprecated/batched_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/_deprecated/batched_joblib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/_deprecated/batched_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/_deprecated/batched_memmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/_deprecated/batched_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/_deprecated/nmslib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/_deprecated/original.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.815286 corals-0.1.5/src/corals/correlation/topk/_experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/_experimental/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/_experimental/nndescent.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/baselines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.819286 corals-0.1.5/src/corals/correlation/topk/batched/
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/batched/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/batched/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/batched/nearest_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/batched/nearest_neighbors_ann_ngt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/batched/nearest_neighbors_ann_nmslib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/batched/nearest_neighbors_balltree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/batched/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/batched/result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topk/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.819286 corals-0.1.5/src/corals/correlation/topkdiff/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topkdiff/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topkdiff/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/topkdiff/original.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/correlation/utils_numba.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.819286 corals-0.1.5/src/corals/sorting/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/sorting/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-03-06 15:44:18.000000 corals-0.1.5/src/corals/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.811286 corals-0.1.5/src/corals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-03-06 15:44:43.000000 corals-0.1.5/src/corals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-03-06 15:44:43.000000 corals-0.1.5/src/corals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 15:44:43.000000 corals-0.1.5/src/corals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 15:44:43.000000 corals-0.1.5/src/corals.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-06 15:44:43.000000 corals-0.1.5/src/corals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-06 15:44:43.000000 corals-0.1.5/src/corals.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:44:43.819286 corals-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-06 15:44:18.000000 corals-0.1.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-06 15:44:18.000000 corals-0.1.5/tests/test_correlation_full.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-06 15:44:18.000000 corals-0.1.5/tests/test_correlation_nearest_neighbors_ngt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-06 15:44:18.000000 corals-0.1.5/tests/test_correlation_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-06 15:44:18.000000 corals-0.1.5/tests/test_correlation_threshold2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-03-06 15:44:18.000000 corals-0.1.5/tests/test_correlation_topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-06 15:44:18.000000 corals-0.1.5/tests/test_correlation_topk_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-03-06 15:44:18.000000 corals-0.1.5/tests/test_correlation_topkdiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-03-06 15:44:18.000000 corals-0.1.5/tests/test_correlation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-06 15:44:18.000000 corals-0.1.5/tests/test_correlation_utils_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-06 15:44:18.000000 corals-0.1.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-06 15:44:18.000000 corals-0.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.085960 corals-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-07 07:51:55.000000 corals-0.1.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.073959 corals-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.077959 corals-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-08-07 07:51:55.000000 corals-0.1.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-07 07:51:55.000000 corals-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-08-07 07:51:55.000000 corals-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-07 07:51:55.000000 corals-0.1.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-07 07:51:55.000000 corals-0.1.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-08-07 07:52:24.085960 corals-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-07 07:51:55.000000 corals-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.077959 corals-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-07 07:51:55.000000 corals-0.1.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.077959 corals-0.1.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 07:51:55.000000 corals-0.1.6/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-07 07:51:55.000000 corals-0.1.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 07:51:55.000000 corals-0.1.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-08-07 07:51:55.000000 corals-0.1.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-07 07:51:55.000000 corals-0.1.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-07 07:51:55.000000 corals-0.1.6/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.077959 corals-0.1.6/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-08-07 07:51:55.000000 corals-0.1.6/docs/notebooks/full.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-08-07 07:51:55.000000 corals-0.1.6/docs/notebooks/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-07 07:51:55.000000 corals-0.1.6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-07 07:51:55.000000 corals-0.1.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-07 07:51:55.000000 corals-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-08-07 07:52:24.085960 corals-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-07 07:51:55.000000 corals-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.073959 corals-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.077959 corals-0.1.6/src/corals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.077959 corals-0.1.6/src/corals/_experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/_experimental/test_correlation_topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/_experimental/test_joblib_context_size_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/_experimental/test_joblib_context_size_large_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/_experimental/test_presorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/_experimental/test_topk_reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.081959 corals-0.1.6/src/corals/correlation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.081959 corals-0.1.6/src/corals/correlation/full/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.081959 corals-0.1.6/src/corals/correlation/full/_deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/full/_deprecated/original.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/full/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/full/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/full/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/full/matmul.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.081959 corals-0.1.6/src/corals/correlation/threshold/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.081959 corals-0.1.6/src/corals/correlation/threshold/_deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/threshold/_deprecated/original.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/threshold/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/threshold/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.081959 corals-0.1.6/src/corals/correlation/topk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.081959 corals-0.1.6/src/corals/correlation/topk/_deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/_deprecated/batched_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/_deprecated/batched_joblib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/_deprecated/batched_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/_deprecated/batched_memmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/_deprecated/batched_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/_deprecated/nmslib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/_deprecated/original.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.081959 corals-0.1.6/src/corals/correlation/topk/_experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/_experimental/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/_experimental/nndescent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/baselines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.081959 corals-0.1.6/src/corals/correlation/topk/batched/
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/batched/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/batched/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/batched/nearest_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/batched/nearest_neighbors_ann_ngt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/batched/nearest_neighbors_ann_nmslib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/batched/nearest_neighbors_balltree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/batched/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/batched/result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topk/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.085960 corals-0.1.6/src/corals/correlation/topkdiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topkdiff/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topkdiff/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/topkdiff/original.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/correlation/utils_numba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.085960 corals-0.1.6/src/corals/sorting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/sorting/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-07 07:51:55.000000 corals-0.1.6/src/corals/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.077959 corals-0.1.6/src/corals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-08-07 07:52:24.000000 corals-0.1.6/src/corals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-07 07:52:24.000000 corals-0.1.6/src/corals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:52:24.000000 corals-0.1.6/src/corals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:52:23.000000 corals-0.1.6/src/corals.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-07 07:52:24.000000 corals-0.1.6/src/corals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 07:52:24.000000 corals-0.1.6/src/corals.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.085960 corals-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-07 07:51:55.000000 corals-0.1.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-07 07:51:55.000000 corals-0.1.6/tests/test_correlation_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-07 07:51:55.000000 corals-0.1.6/tests/test_correlation_nearest_neighbors_ngt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-08-07 07:51:55.000000 corals-0.1.6/tests/test_correlation_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-07 07:51:55.000000 corals-0.1.6/tests/test_correlation_threshold2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-08-07 07:51:55.000000 corals-0.1.6/tests/test_correlation_topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-07 07:51:55.000000 corals-0.1.6/tests/test_correlation_topk_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-07 07:51:55.000000 corals-0.1.6/tests/test_correlation_topkdiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-08-07 07:51:55.000000 corals-0.1.6/tests/test_correlation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-08-07 07:51:55.000000 corals-0.1.6/tests/test_correlation_utils_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 07:51:55.000000 corals-0.1.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-07 07:51:55.000000 corals-0.1.6/tox.ini
```

### Comparing `corals-0.1.5/.coveragerc` & `corals-0.1.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/.github/workflows/ci.yml` & `corals-0.1.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/.gitignore` & `corals-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/.pre-commit-config.yaml` & `corals-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/PKG-INFO` & `corals-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: corals
-Version: 0.1.5
+Version: 0.1.6
 Summary: CorALS is an open-source software package for the construction and analysis of large-scale correlation networks for high-dimensional data.
 Home-page: https://github.com/mgbckr/corals-python
 Author: Martin Becker
 Author-email: mgbckr@stanford.edu
 License: MIT
 Project-URL: Documentation, https://github.com/mgbckr/corals-python
 Project-URL: Source, https://github.com/mgbckr/corals-python
 Project-URL: Tracker, https://github.com/mgbckr/corals-python/issues
 Project-URL: Download, https://pypi.org/project/corals/#files
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Requires-Python: <3.11,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 
 # CorALS
 
 *CorALS* is an open-source software package for the construction and analysis of large-scale correlation networks for high-dimensional data.
 
 If you use *CorALS* for a scientific publication, please cite:
 
 ```plain
-TO BE PUBLISHED
+Becker, M., Nassar, H., Espinosa, C. et al. 
+Large-scale correlation network construction for unraveling the coordination of complex biological systems. 
+Nat Comput Sci (2023). 
+https://doi.org/10.1038/s43588-023-00429-y
 ```
 
 ## Install
 
 ```bash
 pip install corals
 ```
```

### Comparing `corals-0.1.5/README.md` & `corals-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # CorALS
 
 *CorALS* is an open-source software package for the construction and analysis of large-scale correlation networks for high-dimensional data.
 
 If you use *CorALS* for a scientific publication, please cite:
 
 ```plain
-TO BE PUBLISHED
+Becker, M., Nassar, H., Espinosa, C. et al. 
+Large-scale correlation network construction for unraveling the coordination of complex biological systems. 
+Nat Comput Sci (2023). 
+https://doi.org/10.1038/s43588-023-00429-y
 ```
 
 ## Install
 
 ```bash
 pip install corals
 ```
```

### Comparing `corals-0.1.5/docs/Makefile` & `corals-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/docs/conf.py` & `corals-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/docs/index.rst` & `corals-0.1.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/docs/notebooks/full.ipynb` & `corals-0.1.6/docs/notebooks/full.ipynb`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/docs/notebooks/quickstart.ipynb` & `corals-0.1.6/docs/notebooks/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/setup.cfg` & `corals-0.1.6/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
-python_requires = >=3.9,<3.11
+python_requires = >=3.9
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	numba>=0.52.0
 	numpy>=1.20.3,<2.0.0
 	joblib>=1.0.0,<2.0.0
 	scipy>=1.6.3,<2.0.0
 	scikit-learn>=0.24.2,<2.0.0
```

### Comparing `corals-0.1.5/setup.py` & `corals-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/__init__.py` & `corals-0.1.6/src/corals/__init__.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/_experimental/test_correlation_topk.py` & `corals-0.1.6/src/corals/_experimental/test_correlation_topk.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/_experimental/test_joblib_context_size_large_small.py` & `corals-0.1.6/src/corals/_experimental/test_joblib_context_size_large_small.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/_experimental/test_presorting.py` & `corals-0.1.6/src/corals/_experimental/test_presorting.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/_experimental/test_topk_reduce.py` & `corals-0.1.6/src/corals/_experimental/test_topk_reduce.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/full/_deprecated/original.py` & `corals-0.1.6/src/corals/correlation/full/_deprecated/original.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/full/matmul.py` & `corals-0.1.6/src/corals/correlation/full/matmul.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/threshold/_deprecated/original.py` & `corals-0.1.6/src/corals/correlation/threshold/_deprecated/original.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/threshold/loop.py` & `corals-0.1.6/src/corals/correlation/threshold/loop.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/_deprecated/batched_generic.py` & `corals-0.1.6/src/corals/correlation/topk/_deprecated/batched_generic.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/_deprecated/batched_joblib.py` & `corals-0.1.6/src/corals/correlation/topk/_deprecated/batched_joblib.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/_deprecated/batched_loop.py` & `corals-0.1.6/src/corals/correlation/topk/_deprecated/batched_loop.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/_deprecated/batched_memmap.py` & `corals-0.1.6/src/corals/correlation/topk/_deprecated/batched_memmap.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/_deprecated/batched_old.py` & `corals-0.1.6/src/corals/correlation/topk/_deprecated/batched_old.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/_deprecated/nmslib.py` & `corals-0.1.6/src/corals/correlation/topk/_deprecated/nmslib.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/_deprecated/original.py` & `corals-0.1.6/src/corals/correlation/topk/_deprecated/original.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/_experimental/distributed.py` & `corals-0.1.6/src/corals/correlation/topk/_experimental/distributed.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/_experimental/nndescent.py` & `corals-0.1.6/src/corals/correlation/topk/_experimental/nndescent.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/baselines.py` & `corals-0.1.6/src/corals/correlation/topk/baselines.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/batched/base.py` & `corals-0.1.6/src/corals/correlation/topk/batched/base.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/batched/matmul.py` & `corals-0.1.6/src/corals/correlation/topk/batched/matmul.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/batched/nearest_neighbors.py` & `corals-0.1.6/src/corals/correlation/topk/batched/nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/batched/nearest_neighbors_ann_ngt.py` & `corals-0.1.6/src/corals/correlation/topk/batched/nearest_neighbors_ann_ngt.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/batched/nearest_neighbors_ann_nmslib.py` & `corals-0.1.6/src/corals/correlation/topk/batched/nearest_neighbors_ann_nmslib.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/batched/nearest_neighbors_balltree.py` & `corals-0.1.6/src/corals/correlation/topk/batched/nearest_neighbors_balltree.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/batched/reduce.py` & `corals-0.1.6/src/corals/correlation/topk/batched/reduce.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/batched/result_handler.py` & `corals-0.1.6/src/corals/correlation/topk/batched/result_handler.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topk/helper.py` & `corals-0.1.6/src/corals/correlation/topk/helper.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/topkdiff/original.py` & `corals-0.1.6/src/corals/correlation/topkdiff/original.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/utils.py` & `corals-0.1.6/src/corals/correlation/utils.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/correlation/utils_numba.py` & `corals-0.1.6/src/corals/correlation/utils_numba.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/sorting/parallel.py` & `corals-0.1.6/src/corals/sorting/parallel.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals/threads.py` & `corals-0.1.6/src/corals/threads.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/src/corals.egg-info/PKG-INFO` & `corals-0.1.6/src/corals.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: corals
-Version: 0.1.5
+Version: 0.1.6
 Summary: CorALS is an open-source software package for the construction and analysis of large-scale correlation networks for high-dimensional data.
 Home-page: https://github.com/mgbckr/corals-python
 Author: Martin Becker
 Author-email: mgbckr@stanford.edu
 License: MIT
 Project-URL: Documentation, https://github.com/mgbckr/corals-python
 Project-URL: Source, https://github.com/mgbckr/corals-python
 Project-URL: Tracker, https://github.com/mgbckr/corals-python/issues
 Project-URL: Download, https://pypi.org/project/corals/#files
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Requires-Python: <3.11,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 
 # CorALS
 
 *CorALS* is an open-source software package for the construction and analysis of large-scale correlation networks for high-dimensional data.
 
 If you use *CorALS* for a scientific publication, please cite:
 
 ```plain
-TO BE PUBLISHED
+Becker, M., Nassar, H., Espinosa, C. et al. 
+Large-scale correlation network construction for unraveling the coordination of complex biological systems. 
+Nat Comput Sci (2023). 
+https://doi.org/10.1038/s43588-023-00429-y
 ```
 
 ## Install
 
 ```bash
 pip install corals
 ```
```

### Comparing `corals-0.1.5/src/corals.egg-info/SOURCES.txt` & `corals-0.1.6/src/corals.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .coveragerc
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
+CHANGELOG.md
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/ci.yml
 docs/Makefile
```

### Comparing `corals-0.1.5/tests/test_correlation_full.py` & `corals-0.1.6/tests/test_correlation_full.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/tests/test_correlation_nearest_neighbors_ngt.py` & `corals-0.1.6/tests/test_correlation_nearest_neighbors_ngt.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/tests/test_correlation_threshold.py` & `corals-0.1.6/tests/test_correlation_threshold.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/tests/test_correlation_threshold2.py` & `corals-0.1.6/tests/test_correlation_threshold2.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/tests/test_correlation_topk.py` & `corals-0.1.6/tests/test_correlation_topk.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/tests/test_correlation_topk_general.py` & `corals-0.1.6/tests/test_correlation_topk_general.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/tests/test_correlation_topkdiff.py` & `corals-0.1.6/tests/test_correlation_topkdiff.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/tests/test_correlation_utils.py` & `corals-0.1.6/tests/test_correlation_utils.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/tests/test_correlation_utils_numba.py` & `corals-0.1.6/tests/test_correlation_utils_numba.py`

 * *Files identical despite different names*

### Comparing `corals-0.1.5/tox.ini` & `corals-0.1.6/tox.ini`

 * *Files identical despite different names*

