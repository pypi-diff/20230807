# Comparing `tmp/pysubgroup-0.7.3.tar.gz` & `tmp/pysubgroup-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysubgroup-0.7.3.tar", last modified: Fri Jun 17 21:40:23 2022, max compression
+gzip compressed data, was "pysubgroup-0.7.6.tar", last modified: Mon Aug  7 11:13:41 2023, max compression
```

## Comparing `pysubgroup-0.7.3.tar` & `pysubgroup-0.7.6.tar`

### file list

```diff
@@ -1,53 +1,96 @@
-drwxr-xr-x   0 mgbckr    (1000) mgbckr    (1000)        0 2022-06-17 21:40:23.337668 pysubgroup-0.7.3/
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)    11347 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/LICENSE
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)      989 2022-06-17 21:40:23.337668 pysubgroup-0.7.3/PKG-INFO
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     8630 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/README.md
-drwxr-xr-x   0 mgbckr    (1000) mgbckr    (1000)        0 2022-06-17 21:40:23.327668 pysubgroup-0.7.3/pysubgroup/
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)      440 2021-08-15 18:49:27.000000 pysubgroup-0.7.3/pysubgroup/__init__.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)    21506 2022-06-14 21:59:04.000000 pysubgroup-0.7.3/pysubgroup/algorithms.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)    14663 2022-06-14 21:59:04.000000 pysubgroup-0.7.3/pysubgroup/binary_target.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)      548 2021-08-15 18:49:27.000000 pysubgroup-0.7.3/pysubgroup/constraints.py
-drwxr-xr-x   0 mgbckr    (1000) mgbckr    (1000)        0 2022-06-17 21:40:23.329667 pysubgroup-0.7.3/pysubgroup/data/
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)   162249 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/pysubgroup/data/credit-g.arff
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)    10303 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/pysubgroup/data/titanic.csv
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)     3041 2021-08-15 18:49:27.000000 pysubgroup-0.7.3/pysubgroup/fi_target.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)    15281 2021-08-15 18:49:27.000000 pysubgroup-0.7.3/pysubgroup/gp_growth.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)     9124 2021-08-15 18:49:27.000000 pysubgroup-0.7.3/pysubgroup/measures.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)     4233 2021-08-15 18:49:27.000000 pysubgroup-0.7.3/pysubgroup/model_target.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)    25967 2022-06-14 21:59:04.000000 pysubgroup-0.7.3/pysubgroup/numeric_target.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)     1279 2021-08-15 18:49:27.000000 pysubgroup-0.7.3/pysubgroup/refinement_operator.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)     6299 2021-08-15 18:49:27.000000 pysubgroup-0.7.3/pysubgroup/representations.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)    20344 2022-06-14 21:19:24.000000 pysubgroup-0.7.3/pysubgroup/subgroup_description.py
-drwxr-xr-x   0 mgbckr    (1000) mgbckr    (1000)        0 2022-06-17 21:40:23.337668 pysubgroup-0.7.3/pysubgroup/tests/
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)      441 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/pysubgroup/tests/DataSets.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)        0 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/pysubgroup/tests/__init__.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     1444 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/algorithms_testing.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)      541 2021-08-15 18:49:27.000000 pysubgroup-0.7.3/pysubgroup/tests/t_combined_im.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)      483 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/t_numeric_targets.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)      549 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/t_numeric_targets2.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)      654 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/pysubgroup/tests/t_simple_dfs.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)      451 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/t_titanic.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)      645 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/pysubgroup/tests/test_ChiSquaredQF.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     2628 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/test_SubgroupDiscoveryResult.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)    14294 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/test_algorithms_boolean.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     9452 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/test_algorithms_boolean_constraints.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     6677 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/test_algorithms_numeric.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     2839 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/pysubgroup/tests/test_boolean_expressions.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     5447 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/test_fi_target.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     5951 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/test_generalisation_aware.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     6373 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/pysubgroup/tests/test_generalisations.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     1708 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/test_qf_input.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     4135 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/pysubgroup/tests/test_representations.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     5025 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/tests/test_subgroup.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)      537 2022-06-14 21:19:44.000000 pysubgroup-0.7.3/pysubgroup/tests/test_subgroup_description.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)      665 2020-07-17 00:40:31.000000 pysubgroup-0.7.3/pysubgroup/tests/test_visualization.py
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)     8515 2021-01-05 23:38:25.000000 pysubgroup-0.7.3/pysubgroup/utils.py
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)     5478 2021-08-15 18:49:27.000000 pysubgroup-0.7.3/pysubgroup/visualization.py
-drwxr-xr-x   0 mgbckr    (1000) mgbckr    (1000)        0 2022-06-17 21:40:23.327668 pysubgroup-0.7.3/pysubgroup.egg-info/
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)      989 2022-06-17 21:40:22.000000 pysubgroup-0.7.3/pysubgroup.egg-info/PKG-INFO
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)     1502 2022-06-17 21:40:23.000000 pysubgroup-0.7.3/pysubgroup.egg-info/SOURCES.txt
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)        1 2022-06-17 21:40:22.000000 pysubgroup-0.7.3/pysubgroup.egg-info/dependency_links.txt
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)       38 2022-06-17 21:40:23.000000 pysubgroup-0.7.3/pysubgroup.egg-info/requires.txt
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)       11 2022-06-17 21:40:23.000000 pysubgroup-0.7.3/pysubgroup.egg-info/top_level.txt
--rw-rw-r--   0 mgbckr    (1000) mgbckr    (1000)       79 2022-06-17 21:40:23.338667 pysubgroup-0.7.3/setup.cfg
--rw-r--r--   0 mgbckr    (1000) mgbckr    (1000)     1461 2022-06-17 21:21:20.000000 pysubgroup-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.968055 pysubgroup-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.928054 pysubgroup-0.7.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.940055 pysubgroup-0.7.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    15918 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-08-07 11:13:41.968055 pysubgroup-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.944055 pysubgroup-0.7.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.944055 pysubgroup-0.7.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.944055 pysubgroup-0.7.6/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.944055 pysubgroup-0.7.6/docs/sections/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/sections/components/gp_growth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/sections/components/selectors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/sections/components/targets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/sections/index_components.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.944055 pysubgroup-0.7.6/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/docs/tutorials/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-07 11:13:41.968055 pysubgroup-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.932054 pysubgroup-0.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.952055 pysubgroup-0.7.6/src/pysubgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23450 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16434 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/binary_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.956055 pysubgroup-0.7.6/src/pysubgroup/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   161620 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/data/credit-g.arff
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/data/titanic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/fi_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20040 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/gp_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/model_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28185 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/numeric_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/refinement_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/subgroup_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/src/pysubgroup/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.956055 pysubgroup-0.7.6/src/pysubgroup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-08-07 11:13:41.000000 pysubgroup-0.7.6/src/pysubgroup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-07 11:13:41.000000 pysubgroup-0.7.6/src/pysubgroup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:13:41.000000 pysubgroup-0.7.6/src/pysubgroup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:13:41.000000 pysubgroup-0.7.6/src/pysubgroup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-07 11:13:41.000000 pysubgroup-0.7.6/src/pysubgroup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 11:13:41.000000 pysubgroup-0.7.6/src/pysubgroup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:13:41.968055 pysubgroup-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/algorithms_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/t_combined_im.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/t_gp_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/t_numeric_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/t_numeric_targets2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/t_simple_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/t_titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/t_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_ChiSquaredQF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_SubgroupDiscoveryResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_algorithms_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_algorithms_boolean_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_algorithms_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_binary_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_boolean_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_fi_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_generalisation_aware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_generalisations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_gp_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_model_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_qf_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_subgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_subgroup_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_utils_dataconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-07 11:12:56.000000 pysubgroup-0.7.6/tox.ini
```

### Comparing `pysubgroup-0.7.3/LICENSE` & `pysubgroup-0.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysubgroup-0.7.3/README.md` & `pysubgroup-0.7.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,81 @@
-# Pysubgroup
+<!-- These are examples of badges you might want to add to your README:
+     please update the URLs accordingly
+
+[![Built Status](https://api.cirrus-ci.com/github/<USER>/pysubgroup.svg?branch=main)](https://cirrus-ci.com/github/<USER>/pysubgroup)
+[![ReadTheDocs](https://readthedocs.org/projects/pysubgroup/badge/?version=latest)](https://pysubgroup.readthedocs.io/en/stable/)
+[![Coveralls](https://img.shields.io/coveralls/github/<USER>/pysubgroup/main.svg)](https://coveralls.io/r/<USER>/pysubgroup)
+[![PyPI-Server](https://img.shields.io/pypi/v/pysubgroup.svg)](https://pypi.org/project/pysubgroup/)
+[![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/pysubgroup.svg)](https://anaconda.org/conda-forge/pysubgroup)
+[![Monthly Downloads](https://pepy.tech/badge/pysubgroup/month)](https://pepy.tech/project/pysubgroup)
+[![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/pysubgroup)
+-->
+
+
+# pysubgroup
 
 **pysubgroup** is a Python package that enables subgroup discovery in Python+pandas (scipy stack) data analysis environment. It provides for a lightweight, easy-to-use, extensible and freely available implementation of state-of-the-art algorithms, interestingness measures and presentation options.
 
-As of 2020, this library is still in a prototype phase. It has, however, been already succeesfully employed in active application projects.
+This library is still in a prototype phase. It has, however, been already successfully employed in active application projects.
 
-### Subgroup Discovery
+## Subgroup Discovery
 
 Subgroup Discovery is a well established data mining technique that allows you to identify patterns in your data.
 More precisely, the goal of subgroup discovery is to identify descriptions of data subsets that show an interesting distribution with respect to a pre-specified target concept.
 For example, given a dataset of patients in a hospital, we could be interested in subgroups of patients, for which a certain treatment X was successful.
 One example result could then be stated as:
 
 _"While in general the operation is successful in only 60% of the cases", for the subgroup
-of female patients under 50 that also have been treated with drug d, the successrate was 82%."_
+of female patients under 50 that also have been treated with drug d, the success rate was 82%."_
 
 Here, a variable _operation success_ is the target concept, the identified subgroup has the interpretable description _female=True AND age<50 AND drug_D = True_. We call these single conditions (such as _female=True_) selection expressions or short _selectors_.
 The interesting behavior for this subgroup is that the distribution of the target concept differs significantly from the distribution in the overall general dataset.
 A discovered subgroup could also be seen as a rule:
 ```
 female=True AND age<50 AND drug_D = True ==> Operation_outcome=SUCCESS
 ```
-Computationally, subgroup discovery is challenging since a large number of such conjunctive subgroup descriptions have to be considered. Of course, finding computable criteria, which subgroups are likely interesting to a user is also an eternal struggle. 
+Computationally, subgroup discovery is challenging since a large number of such conjunctive subgroup descriptions have to be considered. Of course, finding computable criteria, which subgroups are likely interesting to a user is also an eternal struggle.
 Therefore, a lot of literature has been devoted to the topic of subgroup discovery (including some of my own work). Recent overviews on the topic are for example:
 
 * Herrera, Franciso, et al. ["An overview on subgroup discovery: foundations and applications."](https://scholar.google.de/scholar?q=Herrera%2C+Franciso%2C+et+al.+%E2%80%9CAn+overview+on+subgroup+discovery%3A+foundations+and+applications.%E2%80%9D+Knowledge+and+information+systems+29.3+(2011)%3A+495-525.) Knowledge and information systems 29.3 (2011): 495-525.
 * Atzmueller, Martin. ["Subgroup discovery."](https://scholar.google.de/scholar?q=Atzmueller%2C+Martin.+%E2%80%9CSubgroup+discovery.%E2%80%9D+Wiley+Interdisciplinary+Reviews%3A+Data+Mining+and+Knowledge+Discovery+5.1+(2015)%3A+35-49.) Wiley Interdisciplinary Reviews: Data Mining and Knowledge Discovery 5.1 (2015): 35-49.
 * And of course, my point of view on the topic is [summarized in my dissertation](https://opus.bibliothek.uni-wuerzburg.de/files/9781/Dissertation-Lemmerich.pdf):
 
 ### Prerequisites and Installation
 pysubgroup is built to fit in the standard Python data analysis environment from the scipy-stack.
 Thus, it can be used just having pandas (including its dependencies numpy, scipy, and matplotlib) installed. Visualizations are carried out with the matplotlib library.
 
 pysubgroup consists of pure Python code. Thus, you can simply download the code from the repository and copy it in your `site-packages` directory.
-pysubgroup is also on PyPI and should be installable using:  
+pysubgroup is also on PyPI and should be installable using:
 `pip install pysubgroup`
 
 **Note**: Some users complained about the **pip installation not working**.
 If, after the installation, it still doesn't find the package, then do the following steps:
  1. Find where the directory `site-packages` is.
  2. Copy the folder `pysubgroup`, which contains the source code, into the `site-packages` directory. (WARNING: This is not the main repository folder. The `pysubgroup` folder is inside the main repository folder, at the same level as `doc`)
  3. Now you can import the module with `import pysubgroup`.
 
-### How to use:
+## How to use:
 A simple use case (here using the well known _titanic_ data) can be created in just a few lines of code:
 
 ```python
 import pysubgroup as ps
 
 # Load the example dataset
-from pysubgroup.tests.DataSets import get_titanic_data
+from pysubgroup.datasets import get_titanic_data
 data = get_titanic_data()
 
 target = ps.BinaryTarget ('Survived', True)
 searchspace = ps.create_selectors(data, ignore=['Survived'])
 task = ps.SubgroupDiscoveryTask (
-    data, 
-    target, 
-    searchspace, 
-    result_set_size=5, 
-    depth=2, 
+    data,
+    target,
+    searchspace,
+    result_set_size=5,
+    depth=2,
     qf=ps.WRAccQF())
 result = ps.BeamSearch().execute(task)
 ```
 The first line imports _pysubgroup_ package.
 The following lines load an example dataset (the popular titanic dataset).
 
 Therafter, we define a target, i.e., the property we are mainly interested in (_'survived'}.
@@ -87,50 +100,53 @@
     <tr>      <th>1</th>      <td>0.101331</td>      <td>Parch==0 AND Sex==female</td>    </tr>
     <tr>      <th>2</th>      <td>0.079142</td>      <td>Sex==female AND SibSp: [0:1[</td>    </tr>
     <tr>      <th>3</th>      <td>0.077663</td>      <td>Cabin.isnull() AND Sex==female</td>    </tr>
     <tr>      <th>4</th>      <td>0.071746</td>      <td>Embarked==S AND Sex==female</td>    </tr>
 </tbody></table>
 
 
-### Key classes
+## Key classes
 Here is an outline on the most important classes:
 * Selector: A Selector represents an atomic condition over the data, e.g., _age < 50_. There several subtypes of Selectors, i.e., NominalSelector (color==BLUE), NumericSelector (age < 50) and NegatedSelector (a wrapper such as not selector1)
 * SubgroupDiscoveryTask: As mentioned before, encapsulates the specification of how an algorithm should search for interesting subgroups
 * SubgroupDicoveryResult: These are the main outcome of a subgroup disovery run. You can obtain a list of subgroups using the `to_subgroups()` or to a dataframe using `to_dataframe()`
 * Conjunction: A conjunction is the most widely used SubgroupDescription, and indicates which data instances are covered by the subgroup. It can be seen as the left hand side of a rule.
 
 
-
-
-
-### License
-I am happy about anyone using this software. Thus, this work is put under an Apache license. However, if this constitutes
-any hindrance to your application, please feel free to contact me, I am sure that we can work something out.
+## License
+We are happy about anyone using this software. Thus, this work is put under an Apache license. However, if this constitutes
+any hindrance to your application, please feel free to contact us, we am sure that we can work something out.
 
     Copyright 2016-2019 Florian Lemmerich
-        
+
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
-    
-### Cite
+
+## Cite
 If you are using pysubgroup for your research, please consider citing our demo paper:
-        
+
     Lemmerich, F., & Becker, M. (2018, September). pysubgroup: Easy-to-use subgroup discovery in python. In Joint European Conference on Machine Learning and Knowledge Discovery in Databases (ECMLPKDD). pp. 658-662.
-    
+
 bibtex:
-  
+
     @inproceedings{lemmerich2018pysubgroup,
       title={pysubgroup: Easy-to-use subgroup discovery in python},
       author={Lemmerich, Florian and Becker, Martin},
       booktitle={Joint European Conference on Machine Learning and Knowledge Discovery in Databases},
       pages={658--662},
       year={2018}
     }
+
+
+## Note
+
+This project has been set up using PyScaffold 4.5. For details and usage
+information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `pysubgroup-0.7.3/pysubgroup/algorithms.py` & `pysubgroup-0.7.6/src/pysubgroup/algorithms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,182 +1,235 @@
-'''
+"""
 Created on 29.04.2016
 
 @author: lemmerfn
-'''
+"""
 import copy
-from math import factorial
-from itertools import combinations, chain
-from heapq import heappush, heappop
-from collections import Counter, namedtuple
 import warnings
+from collections import Counter, defaultdict, namedtuple
+from heapq import heappop, heappush
+from itertools import chain, combinations
+from math import factorial
+
 import numpy as np
+
 import pysubgroup as ps
 
 
 class SubgroupDiscoveryTask:
-    '''
+    """
     Capsulates all parameters required to perform standard subgroup discovery
-    '''
+    """
 
-    def __init__(self, data, target, search_space, qf, result_set_size=10, depth=3, min_quality=0, constraints=None):
+    def __init__(
+        self,
+        data,
+        target,
+        search_space,
+        qf,
+        result_set_size=10,
+        depth=3,
+        min_quality=float("-inf"),
+        constraints=None,
+    ):
         self.data = data
         self.target = target
         self.search_space = search_space
         self.qf = qf
         self.result_set_size = result_set_size
         self.depth = depth
         self.min_quality = min_quality
         if constraints is None:
             constraints = []
         self.constraints = constraints
-        self.constraints_monotone = [constr for constr in constraints if constr.is_monotone]
-        self.constraints_other = [constr for constr in constraints if not constr.is_monotone]
+        self.constraints_monotone = [
+            constr for constr in constraints if constr.is_monotone
+        ]
+        self.constraints_other = [
+            constr for constr in constraints if not constr.is_monotone
+        ]
 
 
 def constraints_satisfied(constraints, subgroup, statistics=None, data=None):
-    return all(constr.is_satisfied(subgroup, statistics, data) for constr in constraints)
-
+    return all(
+        constr.is_satisfied(subgroup, statistics, data) for constr in constraints
+    )
 
 
 class Apriori:
-    def __init__(self, representation_type=None, combination_name='Conjunction', use_numba=True):
+    def __init__(
+        self, representation_type=None, combination_name="Conjunction", use_numba=True
+    ):
         self.combination_name = combination_name
 
         if representation_type is None:
             representation_type = ps.BitSetRepresentation
         self.representation_type = representation_type
         self.use_vectorization = True
-        self.use_repruning = False
-        self.optimistic_estimate_name = 'optimistic_estimate'
+        self.optimistic_estimate_name = "optimistic_estimate"
         self.next_level = self.get_next_level
         self.compiled_func = None
         if use_numba:
             try:
-                import numba # pylint: disable=unused-import, import-outside-toplevel
+                # TODO: used?
+                import numba  # pylint: disable=unused-import, import-outside-toplevel # noqa: F401, E501
+
                 self.next_level = self.get_next_level_numba
-                print('Apriori: Using numba for speedup')
+                print("Apriori: Using numba for speedup")
             except ImportError:
                 pass
 
-
     def get_next_level_candidates(self, task, result, next_level_candidates):
         promising_candidates = []
         optimistic_estimate_function = getattr(task.qf, self.optimistic_estimate_name)
         for sg in next_level_candidates:
             statistics = task.qf.calculate_statistics(sg, task.target, task.data)
-            ps.add_if_required(result, sg, task.qf.evaluate(sg, statistics, task.target, task.data), task, statistics=statistics)
-            optimistic_estimate = optimistic_estimate_function(sg, task.target, task.data, statistics)
+            ps.add_if_required(
+                result,
+                sg,
+                task.qf.evaluate(sg, statistics, task.target, task.data),
+                task,
+                statistics=statistics,
+            )
+            optimistic_estimate = optimistic_estimate_function(
+                sg, task.target, task.data, statistics
+            )
 
             if optimistic_estimate >= ps.minimum_required_quality(result, task):
-                if ps.constraints_hold(task.constraints_monotone, sg, statistics, task.data):
+                if ps.constraints_satisfied(
+                    task.constraints_monotone, sg, statistics, task.data
+                ):
                     promising_candidates.append((optimistic_estimate, sg.selectors))
         min_quality = ps.minimum_required_quality(result, task)
-        promising_candidates = [selectors for estimate, selectors in promising_candidates if estimate > min_quality]
+        promising_candidates = [
+            selectors
+            for estimate, selectors in promising_candidates
+            if estimate > min_quality
+        ]
         return promising_candidates
 
-
     def get_next_level_candidates_vectorized(self, task, result, next_level_candidates):
         promising_candidates = []
         statistics = []
         optimistic_estimate_function = getattr(task.qf, self.optimistic_estimate_name)
         for sg in next_level_candidates:
             statistics.append(task.qf.calculate_statistics(sg, task.target, task.data))
         tpl_class = statistics[0].__class__
         vec_statistics = tpl_class._make(np.array(tpl) for tpl in zip(*statistics))
         qualities = task.qf.evaluate(None, task.target, task.data, vec_statistics)
-        optimistic_estimates = optimistic_estimate_function(None, None, None, vec_statistics)
+        optimistic_estimates = optimistic_estimate_function(
+            None, None, None, vec_statistics
+        )
 
         for sg, quality, stats in zip(next_level_candidates, qualities, statistics):
             ps.add_if_required(result, sg, quality, task, statistics=stats)
 
         min_quality = ps.minimum_required_quality(result, task)
         for sg, optimistic_estimate in zip(next_level_candidates, optimistic_estimates):
             if optimistic_estimate >= min_quality:
                 promising_candidates.append(sg.selectors)
         return promising_candidates
 
-    def reprune_lower_levels(self, promising_candidates, depth):
-        for k in range(1, depth):
-            promising_candidates_k = (combinations(selectors, k) for selectors in promising_candidates)
-            combination_counter = Counter(chain.from_iterable(promising_candidates_k))
-            d = depth + 1 - k
-            unpromising_combinations = set(frozenset(sel) for sel, count in combination_counter.items() if count < d)
-            promising_candidates = list(selectors for selectors in promising_candidates
-                                        if all(frozenset(comb) not in unpromising_combinations for comb in combinations(selectors, k)))
-        return promising_candidates
-
     def get_next_level_numba(self, promising_candidates):
-        from numba import jit # pylint: disable=import-error, import-outside-toplevel
-        if not hasattr(self, 'compiled_func') or self.compiled_func is None:
-            @jit
-            def getNewCandidates(l, hashes):
+        from numba import njit  # pylint: disable=import-error, import-outside-toplevel
+
+        if not hasattr(self, "compiled_func") or self.compiled_func is None:
+
+            @njit
+            def getNewCandidates(candidates, hashes):  # pragma: no cover
                 result = []
-                for i in range(len(l)-1):
-                    for j in range(i + 1, len(l)):
+                for i in range(len(candidates) - 1):
+                    for j in range(i + 1, len(candidates)):
                         if hashes[i] == hashes[j]:
-                            if np.all(l[i, :-1] == l[j, :-1]):
+                            if np.all(candidates[i, :-1] == candidates[j, :-1]):
                                 result.append((i, j))
                 return result
+
             self.compiled_func = getNewCandidates
 
         all_selectors = Counter(chain.from_iterable(promising_candidates))
-        d = {selector:i for i, selector in enumerate(all_selectors)}
-        l = [tuple(d[sel] for sel in selectors) for selectors in promising_candidates]
-        arr = np.array(l, dtype=int)
+        all_selectors_ids = {selector: i for i, selector in enumerate(all_selectors)}
+        promising_candidates_selector_ids = [
+            tuple(all_selectors_ids[sel] for sel in selectors)
+            for selectors in promising_candidates
+        ]
+        arr = np.array(promising_candidates_selector_ids, dtype=int)
 
         print(len(arr))
-        hashes = np.array([hash(tuple(x[:-1])) for x in l], dtype=np.int64)
+        hashes = np.array(
+            [hash(tuple(x[:-1])) for x in promising_candidates_selector_ids],
+            dtype=np.int64,
+        )
         candidates_int = self.compiled_func(arr, hashes)
-        return list((*promising_candidates[i], promising_candidates[j][-1])  for i, j in candidates_int)
+        return list(
+            (*promising_candidates[i], promising_candidates[j][-1])
+            for i, j in candidates_int
+        )
 
     def get_next_level(self, promising_candidates):
-        precomputed_list = list((tuple(sg), sg[-1], hash(tuple(sg[:-1])), tuple(sg[:-1])) for sg in promising_candidates)
-        return list((*sg1, new_selector) for (sg1, _, hash_l, selectors_l), (_, new_selector, hash_r, selectors_r) in combinations(precomputed_list, 2)
-                    if (hash_l == hash_r) and (selectors_l == selectors_r))
+        by_prefix_dict = defaultdict(list)
+        for sg in promising_candidates:
+            by_prefix_dict[tuple(sg[:-1])].append(sg[-1])
+        return [
+            prefix + real_suffix
+            for prefix, suffixes in by_prefix_dict.items()
+            for real_suffix in combinations(sorted(suffixes), 2)
+        ]
 
     def execute(self, task):
         if not isinstance(task.qf, ps.BoundedInterestingnessMeasure):
             raise RuntimeWarning("Quality function is unbounded, long runtime expected")
 
         task.qf.calculate_constant_statistics(task.data, task.target)
 
         with self.representation_type(task.data, task.search_space) as representation:
             combine_selectors = getattr(representation.__class__, self.combination_name)
             result = []
             # init the first level
             next_level_candidates = []
             for sel in task.search_space:
-                next_level_candidates.append(combine_selectors([sel]))
+                sg = combine_selectors([sel])
+                if ps.constraints_satisfied(
+                    task.constraints_monotone, sg, None, task.data
+                ):
+                    next_level_candidates.append(sg)
 
             # level-wise search
             depth = 1
             while next_level_candidates:
                 # check sgs from the last level
                 if self.use_vectorization:
-                    promising_candidates = self.get_next_level_candidates_vectorized(task, result, next_level_candidates)
+                    promising_candidates = self.get_next_level_candidates_vectorized(
+                        task, result, next_level_candidates
+                    )
                 else:
-                    promising_candidates = self.get_next_level_candidates(task, result, next_level_candidates)
+                    promising_candidates = self.get_next_level_candidates(
+                        task, result, next_level_candidates
+                    )
 
                 if depth == task.depth:
                     break
 
-                if self.use_repruning:
-                    promising_candidates = self.reprune_lower_levels(promising_candidates, depth)
-
                 next_level_candidates_no_pruning = self.next_level(promising_candidates)
 
                 # select those selectors and build a subgroup from them
-                #   for which all subsets of length depth (=candidate length -1) are in the set of promising candidates
+                #   for which all subsets of length depth (=candidate length -1)
+                #   are in the set of promising candidates
                 set_promising_candidates = set(tuple(p) for p in promising_candidates)
-                next_level_candidates = [combine_selectors(selectors) for selectors in next_level_candidates_no_pruning
-                                         if all((subset in set_promising_candidates) for subset in combinations(selectors, depth))]
+                next_level_candidates = [
+                    combine_selectors(selectors)
+                    for selectors in next_level_candidates_no_pruning
+                    if all(
+                        (subset in set_promising_candidates)
+                        for subset in combinations(selectors, depth)
+                    )
+                ]
                 depth = depth + 1
 
-        result.sort(key=lambda x: x[0], reverse=True)
+        result = ps.prepare_subgroup_discovery_result(result, task)
         return ps.SubgroupDiscoveryResult(result, task)
 
 
 class BestFirstSearch:
     def execute(self, task):
         result = []
         queue = [(float("-inf"), ps.Conjunction([]))]
@@ -186,28 +239,43 @@
             q, old_description = heappop(queue)
             q = -q
             if not q > ps.minimum_required_quality(result, task):
                 break
             for candidate_description in operator.refinements(old_description):
                 sg = candidate_description
                 statistics = task.qf.calculate_statistics(sg, task.target, task.data)
-                ps.add_if_required(result, sg, task.qf.evaluate(sg, task.target, task.data, statistics), task, statistics=statistics)
+                ps.add_if_required(
+                    result,
+                    sg,
+                    task.qf.evaluate(sg, task.target, task.data, statistics),
+                    task,
+                    statistics=statistics,
+                )
                 if len(candidate_description) < task.depth:
-                    optimistic_estimate = task.qf.optimistic_estimate(sg, task.target, task.data, statistics)
+                    optimistic_estimate = task.qf.optimistic_estimate(
+                        sg, task.target, task.data, statistics
+                    )
 
                     # compute refinements and fill the queue
                     if optimistic_estimate >= ps.minimum_required_quality(result, task):
-                        if ps.constraints_satisfied(task.constraints_monotone, candidate_description, statistics, task.data):
-                            heappush(queue, (-optimistic_estimate, candidate_description))
+                        if ps.constraints_satisfied(
+                            task.constraints_monotone,
+                            candidate_description,
+                            statistics,
+                            task.data,
+                        ):
+                            heappush(
+                                queue, (-optimistic_estimate, candidate_description)
+                            )
 
-        result.sort(key=lambda x: x[0], reverse=True)
+        result = ps.prepare_subgroup_discovery_result(result, task)
         return ps.SubgroupDiscoveryResult(result, task)
 
 
-class GeneralisingBFS:
+class GeneralisingBFS:  # pragma: no cover
     def __init__(self):
         self.alpha = 1.10
         self.discarded = [0, 0, 0, 0, 0, 0, 0]
         self.refined = [0, 0, 0, 0, 0, 0, 0]
 
     def execute(self, task):
         result = []
@@ -233,216 +301,281 @@
 
             if (quality, sg) in result:
                 new_queue = []
                 for q_tmp, c_tmp in queue:
                     if (-q_tmp) > qual:
                         heappush(new_queue, (q_tmp, c_tmp))
                 queue = new_queue
-            optimistic_estimate = task.qf.optimistic_estimate(sg, task.target, task.data, statistics)
+            optimistic_estimate = task.qf.optimistic_estimate(
+                sg, task.target, task.data, statistics
+            )
             # else:
-            #    ps.add_if_required(result, sg, task.qf.evaluate_from_dataset(task.data, sg), task)
-            #    optimistic_estimate = task.qf.optimistic_generalisation_from_dataset(task.data, sg) if qf_is_bounded else float("inf")
+            #    ps.add_if_required(
+            #       result, sg, task.qf.evaluate_from_dataset(task.data, sg), task)
+            #    optimistic_estimate = task.qf.optimistic_generalisation_from_dataset(
+            #       task.data, sg) if qf_is_bounded else float("inf")
 
             # compute refinements and fill the queue
-            if len(candidate_description) < task.depth and (optimistic_estimate / self.alpha ** (len(candidate_description) + 1)) >= ps.minimum_required_quality(result, task):
+            if len(candidate_description) < task.depth and (
+                optimistic_estimate / self.alpha ** (len(candidate_description) + 1)
+            ) >= ps.minimum_required_quality(result, task):
                 # print(qual)
                 # print(optimistic_estimate)
                 self.refined[len(candidate_description)] += 1
                 # print(str(candidate_description))
                 for new_description in operator.refinements(candidate_description):
                     heappush(queue, (-optimistic_estimate, new_description))
             else:
                 self.discarded[len(candidate_description)] += 1
 
         result.sort(key=lambda x: x[0], reverse=True)
         for qual, sg in result:
-            print("{} {}".format(qual, sg))
+            print(f"{qual} {sg}")
         print("discarded " + str(self.discarded))
         return ps.SubgroupDiscoveryResult(result, task)
 
 
 class BeamSearch:
-    '''
+    """
     Implements the BeamSearch algorithm. Its a basic implementation
-    '''
+    """
 
     def __init__(self, beam_width=20, beam_width_adaptive=False):
         self.beam_width = beam_width
         self.beam_width_adaptive = beam_width_adaptive
 
     def execute(self, task):
         # adapt beam width to the result set size if desired
         if self.beam_width_adaptive:
             self.beam_width = task.result_set_size
 
         # check if beam size is to small for result set
         if self.beam_width < task.result_set_size:
-            raise RuntimeError('Beam width in the beam search algorithm is smaller than the result set size!')
+            raise RuntimeError(
+                "Beam width in the beam search algorithm "
+                "is smaller than the result set size!"
+            )
 
         task.qf.calculate_constant_statistics(task.data, task.target)
 
         # init
-        beam = [(0, ps.Conjunction([]), task.qf.calculate_statistics(slice(None), task.target, task.data))]
+        beam = [
+            (
+                0,
+                ps.Conjunction([]),
+                task.qf.calculate_statistics(slice(None), task.target, task.data),
+            )
+        ]
         last_beam = None
 
         depth = 0
         while beam != last_beam and depth < task.depth:
             last_beam = beam.copy()
-            for (_, last_sg, _) in last_beam:
-                if not getattr(last_sg, 'visited', False):
-                    setattr(last_sg, 'visited', True)
+            for _, last_sg, _ in last_beam:
+                if not getattr(last_sg, "visited", False):
+                    setattr(last_sg, "visited", True)
                     for sel in task.search_space:
                         # create a clone
                         new_selectors = list(last_sg.selectors)
                         if sel not in new_selectors:
                             new_selectors.append(sel)
                             sg = ps.Conjunction(new_selectors)
-                            statistics = task.qf.calculate_statistics(sg, task.target, task.data)
-                            quality = task.qf.evaluate(sg, task.target, task.data, statistics)
-                            ps.add_if_required(beam, sg, quality, task, check_for_duplicates=True, statistics=statistics)
+                            statistics = task.qf.calculate_statistics(
+                                sg, task.target, task.data
+                            )
+                            quality = task.qf.evaluate(
+                                sg, task.target, task.data, statistics
+                            )
+                            ps.add_if_required(
+                                beam,
+                                sg,
+                                quality,
+                                task,
+                                check_for_duplicates=True,
+                                statistics=statistics,
+                            )
             depth += 1
-# TODO make sure there is no bug here
-        result = beam[:task.result_set_size]
-        result.sort(key=lambda x: x[0], reverse=True)
+        # TODO make sure there is no bug here
+        result = beam[: task.result_set_size]
+        result = ps.prepare_subgroup_discovery_result(result, task)
         return ps.SubgroupDiscoveryResult(result, task)
 
 
 class SimpleSearch:
     def __init__(self, show_progress=True):
         self.show_progress = show_progress
+
     def execute(self, task):
         task.qf.calculate_constant_statistics(task.data, task.target)
         result = []
-        all_selectors = chain.from_iterable(combinations(task.search_space, r) for r in range(1, task.depth + 1))
+        all_selectors = chain.from_iterable(
+            combinations(task.search_space, r) for r in range(1, task.depth + 1)
+        )
         if self.show_progress:
             try:
-                from tqdm import tqdm   # pylint: disable=import-outside-toplevel
+                from tqdm.auto import tqdm  # pylint: disable=import-outside-toplevel
+
                 def binomial(x, y):
                     try:
                         binom = factorial(x) // factorial(y) // factorial(x - y)
-                    except ValueError:
+                    except ValueError:  # pragma: no cover
                         binom = 0
                     return binom
-                total = sum(binomial(len(task.search_space), k) for k in range(1, task.depth + 1))
+
+                total = sum(
+                    binomial(len(task.search_space), k)
+                    for k in range(1, task.depth + 1)
+                )
                 all_selectors = tqdm(all_selectors, total=total)
             except ImportError:
-                pass
+                warnings.warn(
+                    "tqdm not installed but show_progress=True", ImportWarning
+                )
         for selectors in all_selectors:
             sg = ps.Conjunction(selectors)
             statistics = task.qf.calculate_statistics(sg, task.target, task.data)
             quality = task.qf.evaluate(sg, task.target, task.data, statistics)
             ps.add_if_required(result, sg, quality, task, statistics=statistics)
-        result.sort(key=lambda x: x[0], reverse=True)
+        result = ps.prepare_subgroup_discovery_result(result, task)
         return ps.SubgroupDiscoveryResult(result, task)
 
 
 class SimpleDFS:
     def execute(self, task, use_optimistic_estimates=True):
         task.qf.calculate_constant_statistics(task.data, task.target)
-        result = self.search_internal(task, [], task.search_space, [], use_optimistic_estimates)
-        result.sort(key=lambda x: x[0], reverse=True)
+        result = self.search_internal(
+            task, [], task.search_space, [], use_optimistic_estimates
+        )
+        result = ps.prepare_subgroup_discovery_result(result, task)
         return ps.SubgroupDiscoveryResult(result, task)
 
-    def search_internal(self, task, prefix, modification_set, result, use_optimistic_estimates):
+    def search_internal(
+        self, task, prefix, modification_set, result, use_optimistic_estimates
+    ):
         sg = ps.Conjunction(copy.copy(prefix))
 
         statistics = task.qf.calculate_statistics(sg, task.target, task.data)
-        if use_optimistic_estimates and len(prefix) < task.depth and isinstance(task.qf, ps.BoundedInterestingnessMeasure):
-            optimistic_estimate = task.qf.optimistic_estimate(sg, task.target, task.data, statistics)
+        if (
+            use_optimistic_estimates
+            and len(prefix) < task.depth
+            and isinstance(task.qf, ps.BoundedInterestingnessMeasure)
+        ):
+            optimistic_estimate = task.qf.optimistic_estimate(
+                sg, task.target, task.data, statistics
+            )
             if not optimistic_estimate > ps.minimum_required_quality(result, task):
                 return result
 
         quality = task.qf.evaluate(sg, task.target, task.data, statistics)
         ps.add_if_required(result, sg, quality, task, statistics=statistics)
-        if not ps.constraints_satisfied(task.constraints_monotone, sg, statistics=statistics, data=task.data):
-            return
+        if not ps.constraints_satisfied(
+            task.constraints_monotone, sg, statistics=statistics, data=task.data
+        ):
+            return result
         if len(prefix) < task.depth:
             new_modification_set = copy.copy(modification_set)
             for sel in modification_set:
                 prefix.append(sel)
                 new_modification_set.pop(0)
-                self.search_internal(task, prefix, new_modification_set, result, use_optimistic_estimates)
+                self.search_internal(
+                    task, prefix, new_modification_set, result, use_optimistic_estimates
+                )
                 # remove the sel again
                 prefix.pop(-1)
         return result
 
 
 class DFS:
     """
-    Implementation of a depth-first-search with look-ahead using a provided datastructure.
+    Implementation of a depth-first-search
+    with look-ahead using a provided datastructure.
     """
 
     def __init__(self, apply_representation):
         self.target_bitset = None
         self.apply_representation = apply_representation
         self.operator = None
-        self.params_tpl = namedtuple('StandardQF_parameters', ('size_sg', 'positives_count'))
+        self.params_tpl = namedtuple(
+            "StandardQF_parameters", ("size_sg", "positives_count")
+        )
 
     def execute(self, task):
         self.operator = ps.StaticSpecializationOperator(task.search_space)
         task.qf.calculate_constant_statistics(task.data, task.target)
         result = []
         with self.apply_representation(task.data, task.search_space) as representation:
             self.search_internal(task, result, representation.Conjunction([]))
-        result.sort(key=lambda x: x[0], reverse=True)
+        result = ps.prepare_subgroup_discovery_result(result, task)
         return ps.SubgroupDiscoveryResult(result, task)
 
     def search_internal(self, task, result, sg):
         statistics = task.qf.calculate_statistics(sg, task.target, task.data)
-        if not constraints_satisfied(task.constraints_monotone, sg, statistics, task.data):
+        if not constraints_satisfied(
+            task.constraints_monotone, sg, statistics, task.data
+        ):
             return
-        optimistic_estimate = task.qf.optimistic_estimate(sg, task.target, task.data, statistics)
+        optimistic_estimate = task.qf.optimistic_estimate(
+            sg, task.target, task.data, statistics
+        )
         if not optimistic_estimate > ps.minimum_required_quality(result, task):
             return
         quality = task.qf.evaluate(sg, task.target, task.data, statistics)
         ps.add_if_required(result, sg, quality, task, statistics=statistics)
 
         if sg.depth < task.depth:
             for new_sg in self.operator.refinements(sg):
                 self.search_internal(task, result, new_sg)
 
 
 class DFSNumeric:
-    tpl = namedtuple('size_mean_parameters', ('size_sg', 'mean'))
+    tpl = namedtuple("size_mean_parameters", ("size_sg", "mean"))
+
     def __init__(self):
         self.pop_size = 0
         self.f = None
         self.target_values = None
         self.bitsets = {}
         self.num_calls = 0
+        self.evaluate = None
 
     def execute(self, task):
         if not isinstance(task.qf, ps.StandardQFNumeric):
-            warnings.warn("BSD_numeric so far is only implemented for StandardQFNumeric")
+            raise RuntimeError(
+                "BSD_numeric so far is only implemented for StandardQFNumeric"
+            )
         self.pop_size = len(task.data)
-        sorted_data = task.data.sort_values(task.target.get_attributes(), ascending=False)
+        sorted_data = task.data.sort_values(
+            task.target.get_attributes()[0], ascending=False
+        )
 
         # generate target bitset
         self.target_values = sorted_data[task.target.get_attributes()[0]].to_numpy()
 
         task.qf.calculate_constant_statistics(task.data, task.target)
 
         # generate selector bitsets
         self.bitsets = {}
         for sel in task.search_space:
             # generate bitset
             self.bitsets[sel] = sel.covers(sorted_data)
-        result = self.search_internal(task, [], task.search_space, [], np.ones(len(sorted_data), dtype=bool))
-        result.sort(key=lambda x: x[0], reverse=True)
-
+        result = self.search_internal(
+            task, [], task.search_space, [], np.ones(len(sorted_data), dtype=bool)
+        )
+        result = ps.prepare_subgroup_discovery_result(result, task)
         return ps.SubgroupDiscoveryResult(result, task)
 
     def search_internal(self, task, prefix, modification_set, result, bitset):
         self.num_calls += 1
         sg_size = bitset.sum()
         if sg_size == 0:
             return result
         target_values_sg = self.target_values[bitset]
 
-        target_values_cs = np.cumsum(target_values_sg)
+        target_values_cs = np.cumsum(target_values_sg, dtype=np.float64)
+
         sizes = np.arange(1, len(target_values_cs) + 1)
         mean_values_cs = target_values_cs / sizes
         tpl = DFSNumeric.tpl(sizes, mean_values_cs)
         qualities = task.qf.evaluate(None, None, None, tpl)
         optimistic_estimate = np.max(qualities)
 
         if optimistic_estimate <= ps.minimum_required_quality(result, task):
@@ -455,11 +588,13 @@
 
         if len(prefix) < task.depth:
             new_modification_set = copy.copy(modification_set)
             for sel in modification_set:
                 prefix.append(sel)
                 new_bitset = bitset & self.bitsets[sel]
                 new_modification_set.pop(0)
-                self.search_internal(task, prefix, new_modification_set, result, new_bitset)
+                self.search_internal(
+                    task, prefix, new_modification_set, result, new_bitset
+                )
                 # remove the sel again
                 prefix.pop(-1)
         return result
```

### Comparing `pysubgroup-0.7.3/pysubgroup/binary_target.py` & `pysubgroup-0.7.6/src/pysubgroup/binary_target.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,60 @@
-'''
+"""
 Created on 29.09.2017
 
 @author: lemmerfn
-'''
+"""
 from collections import namedtuple
 from functools import total_ordering
+
 import numpy as np
-import scipy.stats
 
-import pysubgroup as ps
+from pysubgroup.measures import (
+    AbstractInterestingnessMeasure,
+    BoundedInterestingnessMeasure,
+    GeneralizationAwareQF_stats,
+)
 
-from pysubgroup.subgroup_description import EqualitySelector
+from .subgroup_description import EqualitySelector, get_cover_array_and_size
+from .utils import BaseTarget, derive_effective_sample_size
 
 
 @total_ordering
-class BinaryTarget:
-
-    statistic_types = ('size_sg', 'size_dataset', 'positives_sg', 'positives_dataset', 'size_complement',
-                      'relative_size_sg', 'relative_size_complement', 'coverage_sg', 'coverage_complement',
-                      'target_share_sg', 'target_share_complement', 'target_share_dataset', 'lift')
+class BinaryTarget(BaseTarget):
+    statistic_types = (
+        "size_sg",
+        "size_dataset",
+        "positives_sg",
+        "positives_dataset",
+        "size_complement",
+        "relative_size_sg",
+        "relative_size_complement",
+        "coverage_sg",
+        "coverage_complement",
+        "target_share_sg",
+        "target_share_complement",
+        "target_share_dataset",
+        "lift",
+    )
 
     def __init__(self, target_attribute=None, target_value=None, target_selector=None):
         """
         Creates a new target for the boolean model class (classic subgroup discovery).
-        If target_attribute and target_value are given, the target_selector is computed using attribute and value
+        If target_attribute and target_value are given, the target_selector is computed
+        using attribute and value
         """
         if target_attribute is not None and target_value is not None:
             if target_selector is not None:
-                raise BaseException("BinaryTarget is to be constructed EITHER by a selector OR by attribute/value pair")
+                raise ValueError(
+                    "BinaryTarget is to be constructed"
+                    "EITHER by a selector OR by attribute/value pair"
+                )
             target_selector = EqualitySelector(target_attribute, target_value)
         if target_selector is None:
-            raise BaseException("No target selector given")
+            raise ValueError("No target selector given")
         self.target_selector = target_selector
 
     def __repr__(self):
         return "T: " + str(self.target_selector)
 
     def __eq__(self, other):
         return self.__dict__ == other.__dict__
@@ -42,201 +62,305 @@
     def __lt__(self, other):
         return str(self) < str(other)
 
     def covers(self, instance):
         return self.target_selector.covers(instance)
 
     def get_attributes(self):
-        return [self.target_selector.get_attribute_name()]
+        return (self.target_selector.attribute_name,)
 
     def get_base_statistics(self, subgroup, data):
-        cover_arr, size_sg = ps.get_cover_array_and_size(subgroup, len(data), data)
+        cover_arr, size_sg = get_cover_array_and_size(subgroup, len(data), data)
         positives = self.covers(data)
         instances_subgroup = size_sg
         positives_dataset = np.sum(positives)
         instances_dataset = len(data)
         positives_subgroup = np.sum(positives[cover_arr])
-        return instances_dataset, positives_dataset, instances_subgroup, positives_subgroup
+        return (
+            instances_dataset,
+            positives_dataset,
+            instances_subgroup,
+            positives_subgroup,
+        )
 
     def calculate_statistics(self, subgroup, data, cached_statistics=None):
-        if cached_statistics is None or not isinstance(cached_statistics, dict):
-            statistics = dict()
-        elif all(k in cached_statistics for k in BinaryTarget.statistic_types):
+        if self.all_statistics_present(cached_statistics):
             return cached_statistics
-        else:
-            statistics = cached_statistics
 
-        (instances_dataset, positives_dataset, instances_subgroup, positives_subgroup) = \
-            self.get_base_statistics(subgroup, data)
-        statistics['size_sg'] = instances_subgroup
-        statistics['size_dataset'] = instances_dataset
-        statistics['positives_sg'] = positives_subgroup
-        statistics['positives_dataset'] = positives_dataset
-        statistics['size_complement'] = instances_dataset - instances_subgroup
-        statistics['relative_size_sg'] = instances_subgroup / instances_dataset
-        statistics['relative_size_complement'] = (instances_dataset - instances_subgroup) / instances_dataset
-        statistics['coverage_sg'] = positives_subgroup / positives_dataset
-        statistics['coverage_complement'] = (positives_dataset - positives_subgroup) / positives_dataset
-        statistics['target_share_sg'] = positives_subgroup / instances_subgroup
-        statistics['target_share_complement'] = (positives_dataset - positives_subgroup) / (instances_dataset - instances_subgroup)
-        statistics['target_share_dataset'] = positives_dataset / instances_dataset
-        statistics['lift'] = statistics['target_share_sg'] / statistics['target_share_dataset']
+        (
+            instances_dataset,
+            positives_dataset,
+            instances_subgroup,
+            positives_subgroup,
+        ) = self.get_base_statistics(subgroup, data)
+        statistics = {}
+        statistics["size_sg"] = instances_subgroup
+        statistics["size_dataset"] = instances_dataset
+        statistics["positives_sg"] = positives_subgroup
+        statistics["positives_dataset"] = positives_dataset
+        statistics["size_complement"] = instances_dataset - instances_subgroup
+        statistics["relative_size_sg"] = instances_subgroup / instances_dataset
+        statistics["relative_size_complement"] = (
+            instances_dataset - instances_subgroup
+        ) / instances_dataset
+        statistics["coverage_sg"] = positives_subgroup / positives_dataset
+        statistics["coverage_complement"] = (
+            positives_dataset - positives_subgroup
+        ) / positives_dataset
+        statistics["target_share_sg"] = positives_subgroup / instances_subgroup
+        if instances_dataset == instances_subgroup:
+            statistics["target_share_complement"] = float("nan")
+        else:
+            statistics["target_share_complement"] = (
+                positives_dataset - positives_subgroup
+            ) / (instances_dataset - instances_subgroup)
+        statistics["target_share_dataset"] = positives_dataset / instances_dataset
+        statistics["lift"] = (
+            statistics["target_share_sg"] / statistics["target_share_dataset"]
+        )
         return statistics
 
 
-class SimplePositivesQF(ps.AbstractInterestingnessMeasure):  # pylint: disable=abstract-method
-    tpl = namedtuple('PositivesQF_parameters', ('size_sg', 'positives_count'))
+class SimplePositivesQF(
+    AbstractInterestingnessMeasure
+):  # pylint: disable=abstract-method
+    tpl = namedtuple("PositivesQF_parameters", ("size_sg", "positives_count"))
 
     def __init__(self):
         self.dataset_statistics = None
         self.positives = None
         self.has_constant_statistics = False
-        self.required_stat_attrs = ('size_sg', 'positives_count')
+        self.required_stat_attrs = ("size_sg", "positives_count")
 
     def calculate_constant_statistics(self, data, target):
         assert isinstance(target, BinaryTarget)
         self.positives = target.covers(data)
-        self.dataset_statistics = SimplePositivesQF.tpl(len(data), np.sum(self.positives))
+        self.dataset_statistics = SimplePositivesQF.tpl(
+            len(data), np.sum(self.positives)
+        )
         self.has_constant_statistics = True
 
-    def calculate_statistics(self, subgroup, target, data, statistics=None):
-        cover_arr, size_sg = ps.get_cover_array_and_size(subgroup, len(self.positives), data)
-        return SimplePositivesQF.tpl(size_sg, np.count_nonzero(self.positives[cover_arr]))
-
-    def evaluate(self, subgroup, target, data, statistics=None):
-        statistics = self.ensure_statistics(subgroup, target, data, statistics)
-        dataset = self.dataset_statistics
-        return (statistics.positives_count / dataset.positives_count)
-
+    def calculate_statistics(
+        self, subgroup, target, data, statistics=None
+    ):  # pylint: disable=unused-argument
+        cover_arr, size_sg = get_cover_array_and_size(
+            subgroup, len(self.positives), data
+        )
+        return SimplePositivesQF.tpl(
+            size_sg, np.count_nonzero(self.positives[cover_arr])
+        )
+
+    # <<< GpGrowth >>>
+    def gp_get_stats(self, row_index):
+        return np.array([1, self.positives[row_index]], dtype=int)
+
+    def gp_get_null_vector(self):
+        return np.zeros(2)
+
+    def gp_merge(self, left, right):
+        left += right
+
+    def gp_get_params(self, _cover_arr, v):
+        return SimplePositivesQF.tpl(v[0], v[1])
+
+    def gp_to_str(self, stats):
+        return " ".join(map(str, stats))
+
+    def gp_size_sg(self, stats):
+        return stats[0]
+
+    @property
+    def gp_requires_cover_arr(self):
+        return False
 
-        
 
 # TODO Make ChiSquared useful for real nominal data not just binary
-# TODO Introduce Enum for direction
-# TODO Maybe it is possible to give a optimistic estimate for ChiSquared
-class ChiSquaredQF(SimplePositivesQF):
+#      Introduce Enum for direction
+#      Maybe it is possible to give a optimistic estimate for ChiSquared
+class ChiSquaredQF(SimplePositivesQF):  # pragma: no cover
     """
-    ChiSquaredQF which test for statistical independence of a subgroup against it's complement
+    ChiSquaredQF which test for statistical independence
+    of a subgroup against it's complement
 
     ...
 
     """
 
     @staticmethod
-    def chi_squared_qf(instances_dataset, positives_dataset, instances_subgroup, positives_subgroup, min_instances=5, bidirect=True, direction_positive=True, index=0):
+    def chi_squared_qf(
+        instances_dataset,
+        positives_dataset,
+        instances_subgroup,
+        positives_subgroup,
+        min_instances=5,
+        bidirect=True,
+        direction_positive=True,
+        index=0,
+    ):
         """
         Performs chi2 test of statistical independence
 
-        Test whether a subgroup is statistically independent from it's complement (see scipy.stats.chi2_contingency).
+        Test whether a subgroup is statistically independent
+        from it's complement (see scipy.stats.chi2_contingency).
 
 
         Parameters
         ----------
-        instances_dataset, positives_dataset, instances_subgroup, positives_subgroup : int
+        instances_dataset,
+                positives_dataset,
+                instances_subgroup,
+                positives_subgroup : int
             counts of subgroup and dataset
         min_instances : int, optional
             number of required instances, if less -inf is returned for that subgroup
         bidirect : bool, optional
-            If true both directions are considered interesting else direction_positive decides which direction is interesting
+            If true both directions are considered interesting
+            else direction_positive decides which direction is interesting
         direction_positive: bool, optional
-            Only used if bidirect=False; specifies whether you are interested in positive (True) or negative deviations
+            Only used if bidirect=False; specifies whether you are interested
+            in positive (True) or negative deviations
         index : {0, 1}, optional
             decides whether the test statistic (0) or the p-value (1) should be used
         """
+        import scipy.stats  # pylint:disable=import-outside-toplevel
 
-        if (instances_subgroup < min_instances) or ((instances_dataset - instances_subgroup) < min_instances):
+        if (instances_subgroup < min_instances) or (
+            (instances_dataset - instances_subgroup) < min_instances
+        ):
             return float("-inf")
 
-        negatives_subgroup = instances_subgroup - positives_subgroup # pylint: disable=bad-whitespace
-        negatives_dataset = instances_dataset - positives_dataset # pylint: disable=bad-whitespace
+        negatives_subgroup = instances_subgroup - positives_subgroup
+        negatives_dataset = instances_dataset - positives_dataset
         negatives_complement = negatives_dataset - negatives_subgroup
         positives_complement = positives_dataset - positives_subgroup
 
-        val = scipy.stats.chi2_contingency([[positives_subgroup, positives_complement],
-                                            [negatives_subgroup, negatives_complement]], correction=False)[index]
+        val = scipy.stats.chi2_contingency(
+            [
+                [positives_subgroup, positives_complement],
+                [negatives_subgroup, negatives_complement],
+            ],
+            correction=False,
+        )[index]
         if bidirect:
             return val
         p_subgroup = positives_subgroup / instances_subgroup
         p_dataset = positives_dataset / instances_dataset
         if direction_positive and p_subgroup > p_dataset:
             return val
-        elif not direction_positive and p_subgroup < p_dataset:
+        if not direction_positive and p_subgroup < p_dataset:
             return val
         return -val
 
     @staticmethod
-    def chi_squared_qf_weighted(subgroup, data, weighting_attribute, effective_sample_size=0, min_instances=5, ):
-        (instancesDataset, positivesDataset, instancesSubgroup, positivesSubgroup) = subgroup.get_base_statistics(data, weighting_attribute)
-        if (instancesSubgroup < min_instances) or ((instancesDataset - instancesSubgroup) < 5):
+    def chi_squared_qf_weighted(
+        subgroup,
+        data,
+        weighting_attribute,
+        effective_sample_size=0,
+        min_instances=5,
+    ):
+        import scipy.stats  # pylint:disable=import-outside-toplevel
+
+        (
+            instancesDataset,
+            positivesDataset,
+            instancesSubgroup,
+            positivesSubgroup,
+        ) = subgroup.get_base_statistics(data, weighting_attribute)
+        if (instancesSubgroup < min_instances) or (
+            (instancesDataset - instancesSubgroup) < 5
+        ):
             return float("inf")
         if effective_sample_size == 0:
-            effective_sample_size = ps.effective_sample_size(data[weighting_attribute])
+            effective_sample_size = derive_effective_sample_size(
+                data[weighting_attribute]
+            )
         # p_subgroup = positivesSubgroup / instancesSubgroup
         # p_dataset = positivesDataset / instancesDataset
 
         negatives_subgroup = instancesSubgroup - positivesSubgroup
         negatives_dataset = instancesDataset - positivesDataset
         positives_complement = positivesDataset - positivesSubgroup
         negatives_complement = negatives_dataset - negatives_subgroup
-        val = scipy.stats.chi2_contingency([[positivesSubgroup, positives_complement],
-                                            [negatives_subgroup, negatives_complement]], correction=True)[0]
+        val = scipy.stats.chi2_contingency(
+            [
+                [positivesSubgroup, positives_complement],
+                [negatives_subgroup, negatives_complement],
+            ],
+            correction=True,
+        )[0]
         return scipy.stats.chi2.sf(val * effective_sample_size / instancesDataset, 1)
 
-    def __init__(self, direction='both', min_instances=5, stat='chi2'):
+    def __init__(self, direction="both", min_instances=5, stat="chi2"):
         """
         Parameters
         ----------
         direction : {'both', 'positive', 'negative'}
             direction of deviation that is of interest
         min_instances : int, optional
             number of required instances, if less -inf is returned for that subgroup
         stat : {'chi2', 'p'}
-            whether to report the test statistic or the p-value (see scipy.stats.chi2_contingency)
+            whether to report the test statistic
+            or the p-value (see scipy.stats.chi2_contingency)
         """
-        if direction == 'both':
+        if direction == "both":
             self.bidirect = True
             self.direction_positive = True
-        if direction == 'positive':
+        if direction == "positive":
             self.bidirect = False
             self.direction_positive = True
-        if direction == 'negative':
+        if direction == "negative":
             self.bidirect = False
             self.direction_positive = False
         self.min_instances = min_instances
-        self.index = {'chi2' : 0, 'p': 1}[stat]
+        self.index = {"chi2": 0, "p": 1}[stat]
         super().__init__()
 
     def evaluate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
         dataset = self.dataset_statistics
-        return ChiSquaredQF.chi_squared_qf(dataset.size_sg, dataset.positives_count, statistics.size_sg, statistics.positives_count, self.min_instances, self.bidirect, self.direction_positive, self.index)
+        return ChiSquaredQF.chi_squared_qf(
+            dataset.size_sg,
+            dataset.positives_count,
+            statistics.size_sg,
+            statistics.positives_count,
+            self.min_instances,
+            self.bidirect,
+            self.direction_positive,
+            self.index,
+        )
 
 
-class StandardQF(SimplePositivesQF, ps.BoundedInterestingnessMeasure):
+class StandardQF(SimplePositivesQF, BoundedInterestingnessMeasure):
     """
     StandardQF which weights the relative size against the difference in averages
 
-    The StandardQF is a general form of quality function which for different values of a is order equivalen to
+    The StandardQF is a general form of quality function
+    which for different values of a is order equivalen to
     many popular quality measures.
 
     Attributes
     ----------
     a : float
         used as an exponent to scale the relative size to the difference in averages
 
     """
 
     @staticmethod
-    def standard_qf(a, instances_dataset, positives_dataset, instances_subgroup, positives_subgroup):
-        if not hasattr(instances_subgroup, '__array_interface__') and (instances_subgroup == 0):
+    def standard_qf(
+        a, instances_dataset, positives_dataset, instances_subgroup, positives_subgroup
+    ):
+        if not hasattr(instances_subgroup, "__array_interface__") and (
+            instances_subgroup == 0
+        ):
             return np.nan
         p_subgroup = np.divide(positives_subgroup, instances_subgroup)
-        #if instances_subgroup == 0:
+        # if instances_subgroup == 0:
         #    return 0
-        #p_subgroup = positives_subgroup / instances_subgroup
+        # p_subgroup = positives_subgroup / instances_subgroup
         p_dataset = positives_dataset / instances_dataset
         return (instances_subgroup / instances_dataset) ** a * (p_subgroup - p_dataset)
 
     def __init__(self, a):
         """
         Parameters
         ----------
@@ -245,79 +369,97 @@
         """
         self.a = a
         super().__init__()
 
     def evaluate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
         dataset = self.dataset_statistics
-        return StandardQF.standard_qf(self.a, dataset.size_sg, dataset.positives_count, statistics.size_sg, statistics.positives_count)
+        return StandardQF.standard_qf(
+            self.a,
+            dataset.size_sg,
+            dataset.positives_count,
+            statistics.size_sg,
+            statistics.positives_count,
+        )
 
     def optimistic_estimate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
         dataset = self.dataset_statistics
-        return StandardQF.standard_qf(self.a, dataset.size_sg, dataset.positives_count, statistics.positives_count, statistics.positives_count)
+        return StandardQF.standard_qf(
+            self.a,
+            dataset.size_sg,
+            dataset.positives_count,
+            statistics.positives_count,
+            statistics.positives_count,
+        )
 
     def optimistic_generalisation(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
         dataset = self.dataset_statistics
         pos_remaining = dataset.positives_count - statistics.positives_count
-        return StandardQF.standard_qf(self.a, dataset.size_sg, dataset.positives_count, statistics.size_sg + pos_remaining, dataset.positives_count)
+        return StandardQF.standard_qf(
+            self.a,
+            dataset.size_sg,
+            dataset.positives_count,
+            statistics.size_sg + pos_remaining,
+            dataset.positives_count,
+        )
 
 
 class LiftQF(StandardQF):
     """
     Lift Quality Function
 
     LiftQF is a StandardQF with a=0.
-    Thus it treats the difference in ratios as the quality without caring about the relative size of a subgroup.
+    Thus it treats the difference in ratios as the quality
+    without caring about the relative size of a subgroup.
     """
 
     def __init__(self):
-        """
-        """
+        """ """
 
         super().__init__(0.0)
 
 
-
-# TODO add true binomial quality function as in https://opus.bibliothek.uni-wuerzburg.de/opus4-wuerzburg/frontdoor/index/index/docId/1786
+# TODO add true binomial quality function as in
+# https://opus.bibliothek.uni-wuerzburg.de/opus4-wuerzburg/frontdoor/index/index/docId/1786 # noqa: E501
 class SimpleBinomialQF(StandardQF):
     """
     Simple Binomial Quality Function
 
     SimpleBinomialQF is a StandardQF with a=0.5.
-    It is an order equivalent approximation of the full binomial test if the subgroup size is much smaller than the size of the entire dataset.
+    It is an order equivalent approximation of the full binomial test
+    if the subgroup size is much smaller than the size of the entire dataset.
     """
 
     def __init__(self):
-        """
-        """
+        """ """
 
         super().__init__(0.5)
 
 
 class WRAccQF(StandardQF):
     """
     Weighted Relative Accuracy Quality Function
 
     WRAccQF is a StandardQF with a=1.
-    It is order equivalent to the difference in the observed and expected number of positive instances.
+    It is order equivalent to the difference in the observed
+    and expected number of positive instances.
     """
 
     def __init__(self):
-        """
-        """
+        """ """
 
         super().__init__(1.0)
 
 
 #####
 # GeneralizationAware Interestingness Measures
 #####
-class GeneralizationAware_StandardQF(ps.GeneralizationAwareQF_stats):
+class GeneralizationAware_StandardQF(GeneralizationAwareQF_stats):
     def __init__(self, a):
         super().__init__(StandardQF(0))
         self.a = a
 
     def get_max(self, *args):
         max_ratio = 0.0
         max_stats = None
@@ -334,8 +476,10 @@
         sg_stats = statistics.subgroup_stats
         general_stats = statistics.generalisation_stats
         if sg_stats.size_sg == 0 or general_stats.size_sg == 0:
             return np.nan
 
         sg_ratio = sg_stats.positives_count / sg_stats.size_sg
         general_ratio = general_stats.positives_count / general_stats.size_sg
-        return (sg_stats.size_sg / self.stats0.size_sg) ** self.a * (sg_ratio - general_ratio)
+        return (sg_stats.size_sg / self.stats0.size_sg) ** self.a * (
+            sg_ratio - general_ratio
+        )
```

### Comparing `pysubgroup-0.7.3/pysubgroup/data/credit-g.arff` & `pysubgroup-0.7.6/src/pysubgroup/data/credit-g.arff`

 * *Files 1% similar despite different names*

```diff
@@ -1,284 +1,284 @@
 % Description of the German credit dataset.
-% 
+%
 % 1. Title: German Credit data
-% 
+%
 % 2. Source Information
-% 
-% Professor Dr. Hans Hofmann  
-% Institut f"ur Statistik und "Okonometrie  
-% Universit"at Hamburg  
-% FB Wirtschaftswissenschaften  
-% Von-Melle-Park 5    
-% 2000 Hamburg 13 
-% 
+%
+% Professor Dr. Hans Hofmann
+% Institut f"ur Statistik und "Okonometrie
+% Universit"at Hamburg
+% FB Wirtschaftswissenschaften
+% Von-Melle-Park 5
+% 2000 Hamburg 13
+%
 % 3. Number of Instances:  1000
-% 
+%
 % Two datasets are provided.  the original dataset, in the form provided
 % by Prof. Hofmann, contains categorical/symbolic attributes and
-% is in the file "german.data".   
-%  
-% For algorithms that need numerical attributes, Strathclyde University 
-% produced the file "german.data-numeric".  This file has been edited 
-% and several indicator variables added to make it suitable for 
+% is in the file "german.data".
+%
+% For algorithms that need numerical attributes, Strathclyde University
+% produced the file "german.data-numeric".  This file has been edited
+% and several indicator variables added to make it suitable for
 % algorithms which cannot cope with categorical variables.   Several
 % attributes that are ordered categorical (such as attribute 17) have
 % been coded as integer.    This was the form used by StatLog.
-% 
-% 
+%
+%
 % 6. Number of Attributes german: 20 (7 numerical, 13 categorical)
 %    Number of Attributes german.numer: 24 (24 numerical)
-% 
-% 
+%
+%
 % 7.  Attribute description for german
-% 
+%
 % Attribute 1:  (qualitative)
 % 	       Status of existing checking account
 %                A11 :      ... <    0 DM
 % 	       A12 : 0 <= ... <  200 DM
 % 	       A13 :      ... >= 200 DM /
 % 		     salary assignments for at least 1 year
 %                A14 : no checking account
-% 
+%
 % Attribute 2:  (numerical)
 % 	      Duration in month
-% 
+%
 % Attribute 3:  (qualitative)
 % 	      Credit history
 % 	      A30 : no credits taken/
 % 		    all credits paid back duly
 %               A31 : all credits at this bank paid back duly
 % 	      A32 : existing credits paid back duly till now
 %               A33 : delay in paying off in the past
 % 	      A34 : critical account/
 % 		    other credits existing (not at this bank)
-% 
+%
 % Attribute 4:  (qualitative)
 % 	      Purpose
 % 	      A40 : car (new)
 % 	      A41 : car (used)
 % 	      A42 : furniture/equipment
 % 	      A43 : radio/television
 % 	      A44 : domestic appliances
 % 	      A45 : repairs
 % 	      A46 : education
 % 	      A47 : (vacation - does not exist?)
 % 	      A48 : retraining
 % 	      A49 : business
 % 	      A410 : others
-% 
+%
 % Attribute 5:  (numerical)
 % 	      Credit amount
-% 
+%
 % Attibute 6:  (qualitative)
 % 	      Savings account/bonds
 % 	      A61 :          ... <  100 DM
 % 	      A62 :   100 <= ... <  500 DM
 % 	      A63 :   500 <= ... < 1000 DM
 % 	      A64 :          .. >= 1000 DM
 %               A65 :   unknown/ no savings account
-% 
+%
 % Attribute 7:  (qualitative)
 % 	      Present employment since
 % 	      A71 : unemployed
 % 	      A72 :       ... < 1 year
-% 	      A73 : 1  <= ... < 4 years  
+% 	      A73 : 1  <= ... < 4 years
 % 	      A74 : 4  <= ... < 7 years
 % 	      A75 :       .. >= 7 years
-% 
+%
 % Attribute 8:  (numerical)
 % 	      Installment rate in percentage of disposable income
-% 
+%
 % Attribute 9:  (qualitative)
 % 	      Personal status and sex
 % 	      A91 : male   : divorced/separated
 % 	      A92 : female : divorced/separated/married
 %               A93 : male   : single
 % 	      A94 : male   : married/widowed
 % 	      A95 : female : single
-% 
+%
 % Attribute 10: (qualitative)
 % 	      Other debtors / guarantors
 % 	      A101 : none
 % 	      A102 : co-applicant
 % 	      A103 : guarantor
-% 
+%
 % Attribute 11: (numerical)
 % 	      Present residence since
-% 
+%
 % Attribute 12: (qualitative)
 % 	      Property
 % 	      A121 : real estate
 % 	      A122 : if not A121 : building society savings agreement/
 % 				   life insurance
 %               A123 : if not A121/A122 : car or other, not in attribute 6
 % 	      A124 : unknown / no property
-% 
+%
 % Attribute 13: (numerical)
 % 	      Age in years
-% 
+%
 % Attribute 14: (qualitative)
-% 	      Other installment plans 
+% 	      Other installment plans
 % 	      A141 : bank
 % 	      A142 : stores
 % 	      A143 : none
-% 
+%
 % Attribute 15: (qualitative)
 % 	      Housing
 % 	      A151 : rent
 % 	      A152 : own
 % 	      A153 : for free
-% 
+%
 % Attribute 16: (numerical)
 %               Number of existing credits at this bank
-% 
+%
 % Attribute 17: (qualitative)
 % 	      Job
 % 	      A171 : unemployed/ unskilled  - non-resident
 % 	      A172 : unskilled - resident
 % 	      A173 : skilled employee / official
 % 	      A174 : management/ self-employed/
 % 		     highly qualified employee/ officer
-% 
+%
 % Attribute 18: (numerical)
 % 	      Number of people being liable to provide maintenance for
-% 
+%
 % Attribute 19: (qualitative)
 % 	      Telephone
 % 	      A191 : none
 % 	      A192 : yes, registered under the customers name
-% 
+%
 % Attribute 20: (qualitative)
 % 	      foreign worker
 % 	      A201 : yes
 % 	      A202 : no
-% 
-% 
-% 
+%
+%
+%
 % 8.  Cost Matrix
-% 
+%
 % This dataset requires use of a cost matrix (see below)
-% 
-% 
+%
+%
 %       1        2
 % ----------------------------
 %   1   0        1
 % -----------------------
 %   2   5        0
-% 
+%
 % (1 = Good,  2 = Bad)
-% 
+%
 % the rows represent the actual classification and the columns
 % the predicted classification.
-% 
-% It is worse to class a customer as good when they are bad (5), 
+%
+% It is worse to class a customer as good when they are bad (5),
 % than it is to class a customer as bad when they are good (1).
-% 
+%
 %
 %
 %
 %
 % Relabeled values in attribute checking_status
-%    From: A11                     To: '<0'                
-%    From: A12                     To: '0<=X<200'          
-%    From: A13                     To: '>=200'             
-%    From: A14                     To: 'no checking'       
+%    From: A11                     To: '<0'
+%    From: A12                     To: '0<=X<200'
+%    From: A13                     To: '>=200'
+%    From: A14                     To: 'no checking'
 %
 %
 % Relabeled values in attribute credit_history
 %    From: A30                     To: 'no credits/all paid'
-%    From: A31                     To: 'all paid'          
-%    From: A32                     To: 'existing paid'     
+%    From: A31                     To: 'all paid'
+%    From: A32                     To: 'existing paid'
 %    From: A33                     To: 'delayed previously'
 %    From: A34                     To: 'critical/other existing credit'
 %
 %
 % Relabeled values in attribute purpose
-%    From: A40                     To: 'new car'           
-%    From: A41                     To: 'used car'          
-%    From: A42                     To: furniture/equipment 
-%    From: A43                     To: radio/tv            
+%    From: A40                     To: 'new car'
+%    From: A41                     To: 'used car'
+%    From: A42                     To: furniture/equipment
+%    From: A43                     To: radio/tv
 %    From: A44                     To: 'domestic appliance'
-%    From: A45                     To: repairs             
-%    From: A46                     To: education           
-%    From: A47                     To: vacation            
-%    From: A48                     To: retraining          
-%    From: A49                     To: business            
-%    From: A410                    To: other               
+%    From: A45                     To: repairs
+%    From: A46                     To: education
+%    From: A47                     To: vacation
+%    From: A48                     To: retraining
+%    From: A49                     To: business
+%    From: A410                    To: other
 %
 %
 % Relabeled values in attribute savings_status
-%    From: A61                     To: '<100'              
-%    From: A62                     To: '100<=X<500'        
-%    From: A63                     To: '500<=X<1000'       
-%    From: A64                     To: '>=1000'            
-%    From: A65                     To: 'no known savings'  
+%    From: A61                     To: '<100'
+%    From: A62                     To: '100<=X<500'
+%    From: A63                     To: '500<=X<1000'
+%    From: A64                     To: '>=1000'
+%    From: A65                     To: 'no known savings'
 %
 %
 % Relabeled values in attribute employment
-%    From: A71                     To: unemployed          
-%    From: A72                     To: '<1'                
-%    From: A73                     To: '1<=X<4'            
-%    From: A74                     To: '4<=X<7'            
-%    From: A75                     To: '>=7'               
+%    From: A71                     To: unemployed
+%    From: A72                     To: '<1'
+%    From: A73                     To: '1<=X<4'
+%    From: A74                     To: '4<=X<7'
+%    From: A75                     To: '>=7'
 %
 %
 % Relabeled values in attribute personal_status
-%    From: A91                     To: 'male div/sep'      
+%    From: A91                     To: 'male div/sep'
 %    From: A92                     To: 'female div/dep/mar'
-%    From: A93                     To: 'male single'       
-%    From: A94                     To: 'male mar/wid'      
-%    From: A95                     To: 'female single'     
+%    From: A93                     To: 'male single'
+%    From: A94                     To: 'male mar/wid'
+%    From: A95                     To: 'female single'
 %
 %
 % Relabeled values in attribute other_parties
-%    From: A101                    To: none                
-%    From: A102                    To: 'co applicant'      
-%    From: A103                    To: guarantor           
+%    From: A101                    To: none
+%    From: A102                    To: 'co applicant'
+%    From: A103                    To: guarantor
 %
 %
 % Relabeled values in attribute property_magnitude
-%    From: A121                    To: 'real estate'       
-%    From: A122                    To: 'life insurance'    
-%    From: A123                    To: car                 
-%    From: A124                    To: 'no known property' 
+%    From: A121                    To: 'real estate'
+%    From: A122                    To: 'life insurance'
+%    From: A123                    To: car
+%    From: A124                    To: 'no known property'
 %
 %
 % Relabeled values in attribute other_payment_plans
-%    From: A141                    To: bank                
-%    From: A142                    To: stores              
-%    From: A143                    To: none                
+%    From: A141                    To: bank
+%    From: A142                    To: stores
+%    From: A143                    To: none
 %
 %
 % Relabeled values in attribute housing
-%    From: A151                    To: rent                
-%    From: A152                    To: own                 
-%    From: A153                    To: 'for free'          
+%    From: A151                    To: rent
+%    From: A152                    To: own
+%    From: A153                    To: 'for free'
 %
 %
 % Relabeled values in attribute job
 %    From: A171                    To: 'unemp/unskilled non res'
 %    From: A172                    To: 'unskilled resident'
-%    From: A173                    To: skilled             
+%    From: A173                    To: skilled
 %    From: A174                    To: 'high qualif/self emp/mgmt'
 %
 %
 % Relabeled values in attribute own_telephone
-%    From: A191                    To: none                
-%    From: A192                    To: yes                 
+%    From: A191                    To: none
+%    From: A192                    To: yes
 %
 %
 % Relabeled values in attribute foreign_worker
-%    From: A201                    To: yes                 
-%    From: A202                    To: no                  
+%    From: A201                    To: yes
+%    From: A202                    To: no
 %
 %
 % Relabeled values in attribute class
-%    From: 1                       To: good                
-%    From: 2                       To: bad                 
+%    From: 1                       To: good
+%    From: 2                       To: bad
 %
 @relation german_credit
 @attribute checking_status { '<0', '0<=X<200', '>=200', 'no checking'}
 @attribute duration real
 @attribute credit_history { 'no credits/all paid', 'all paid', 'existing paid', 'delayed previously', 'critical/other existing credit'}
 @attribute purpose { 'new car', 'used car', furniture/equipment, radio/tv, 'domestic appliance', repairs, education, vacation, retraining, business, other}
 @attribute credit_amount real
```

### Comparing `pysubgroup-0.7.3/pysubgroup/data/titanic.csv` & `pysubgroup-0.7.6/src/pysubgroup/data/titanic.csv`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -150,8 +150,8 @@
 149	0	2	Navratil, Mr. Michel ("Louis M Hoffman")	male	36.5	0	2	230080	26	F2	S
 150	0	2	Byles, Rev. Thomas Roussel Davids	male	42	0	0	244310	13		S
 151	0	2	Bateman, Rev. Robert James	male	51	0	0	S.O.P. 1166	12.525		S
 152	1	1	Pears, Mrs. Thomas (Edith Wearne)	female	22	1	0	113776	66.6	C2	S
 153	0	3	Meo, Mr. Alfonzo	male	55.5	0	0	A.5. 11206	8.05		S
 154	0	3	van Billiard, Mr. Austin Blyler	male	40.5	0	2	A/5. 851	14.5		S
 155	0	3	Olsen, Mr. Ole Martin	male		0	0	Fa 265302	7.3125		S
-156	0	1	Williams, Mr. Charles Duane	male	51	0	1	PC 17597	61.3792		C
+156	0	1	Williams, Mr. Charles Duane	male	51	0	1	PC 17597	61.3792		C
```

### Comparing `pysubgroup-0.7.3/pysubgroup/fi_target.py` & `pysubgroup-0.7.6/src/pysubgroup/fi_target.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-'''
+"""
 Created on 29.09.2017
 
 @author: lemmerfn
-'''
+"""
 from collections import namedtuple
 from functools import total_ordering
-import pysubgroup as ps
 
+import pysubgroup as ps
 
 
 @total_ordering
-class FITarget:
-    statistic_types = ('size_sg', 'size_dataset')
+class FITarget(ps.BaseTarget):
+    statistic_types = ("size_sg", "size_dataset")
 
     def __repr__(self):
         return "T: Frequent Itemsets"
 
     def __eq__(self, other):
         return self.__dict__ == other.__dict__
 
@@ -26,71 +26,72 @@
         return []
 
     def get_base_statistics(self, subgroup, data):
         _, size = ps.get_cover_array_and_size(subgroup, len(data), data)
         return size
 
     def calculate_statistics(self, subgroup_description, data, cached_statistics=None):
-        if cached_statistics is None or not isinstance(cached_statistics, dict):
-            statistics = dict()
-        elif all(k in cached_statistics for k in FITarget.statistic_types):
+        if self.all_statistics_present(cached_statistics):
             return cached_statistics
-        else:
-            statistics = cached_statistics
 
         _, size = ps.get_cover_array_and_size(subgroup_description, len(data), data)
-
-        statistics['size_sg'] = size
-        statistics['size_dataset'] = len(data)
+        statistics = {}
+        statistics["size_sg"] = size
+        statistics["size_dataset"] = len(data)
         return statistics
 
 
 class SimpleCountQF(ps.AbstractInterestingnessMeasure):
-    tpl = namedtuple('CountQF_parameters', ('subgroup_size'))
+    tpl = namedtuple("CountQF_parameters", ("size_sg"))
+    gp_requires_cover_arr = False
 
     def __init__(self):
-        self.required_stat_attrs = ('subgroup_size',)
+        self.required_stat_attrs = ("size_sg",)
         self.has_constant_statistics = True
         self.size_dataset = None
 
-    def calculate_constant_statistics(self, data, target):
+    def calculate_constant_statistics(
+        self, data, target
+    ):  # pylint: disable=unused-argument
         self.size_dataset = len(data)
 
-    def calculate_statistics(self, subgroup_description, target, data, statistics=None):
-        _, size = ps.get_cover_array_and_size(subgroup_description, self.size_dataset, data)
+    def calculate_statistics(
+        self, subgroup_description, target, data, statistics=None
+    ):  # pylint: disable=unused-argument
+        _, size = ps.get_cover_array_and_size(
+            subgroup_description, self.size_dataset, data
+        )
         return SimpleCountQF.tpl(size)
 
     def gp_get_stats(self, _):
-        return {"subgroup_size" : 1}
+        return {"size_sg": 1}
 
     def gp_get_null_vector(self):
-        return {"subgroup_size":0}
+        return {"size_sg": 0}
 
-    def gp_merge(self, l, r):
-        l["subgroup_size"] += r["subgroup_size"]
+    def gp_merge(self, left, right):
+        left["size_sg"] += right["size_sg"]
 
     def gp_get_params(self, _cover_arr, v):
-        return SimpleCountQF.tpl(v['subgroup_size'])
+        return SimpleCountQF.tpl(v["size_sg"])
 
     def gp_to_str(self, stats):
-        return str(stats['subgroup_size'])
+        return str(stats["size_sg"])
 
-    @property
-    def gp_requires_cover_arr(self):
-        return False
+    def gp_size_sg(self, stats):
+        return stats["size_sg"]
 
 
 class CountQF(SimpleCountQF, ps.BoundedInterestingnessMeasure):
     def evaluate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
-        return statistics.subgroup_size
+        return statistics.size_sg
 
     def optimistic_estimate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
-        return statistics.subgroup_size
-
+        return statistics.size_sg
 
 
 class AreaQF(SimpleCountQF):
     def evaluate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
-        return statistics.subgroup_size * subgroup.depth
+        return statistics.size_sg * subgroup.depth
```

### Comparing `pysubgroup-0.7.3/pysubgroup/gp_growth.py` & `pysubgroup-0.7.6/src/pysubgroup/gp_growth.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,288 +1,471 @@
-from collections import  namedtuple, defaultdict
-from itertools import combinations
+import itertools
+import warnings
+from collections import defaultdict, namedtuple
+from pathlib import Path
+
 import numpy as np
+
 import pysubgroup as ps
-from tqdm import tqdm
-from copy import copy
-import itertools
-class GpGrowth:
 
-    def __init__(self, mode='b_u' ):
-        self.GP_node = namedtuple('GP_node', ['cls', 'id', 'parent', 'children', 'stats'])
+
+def identity(x, *args, **kwargs):  # pylint: disable=unused-argument
+    return x
+
+
+class GpGrowth:
+    def __init__(self, mode="b_u"):
+        self.GP_node = namedtuple(
+            "GP_node", ["cls", "id", "parent", "children", "stats"]
+        )
         self.minSupp = 10
-        self.tqdm = tqdm
+        self.tqdm = identity
         self.depth = 0
-        self.mode = mode  #specify eihther b_u (bottom up) or t_d (top down)
-        # Future: There also is the option of a stable mode which never creates the prefix trees
-
-    def prepare_selectors(self, search_space):
-        
-        self.get_stats = task.qf.gp_get_stats
-        self.get_null_vector = task.qf.gp_get_null_vector
-        self.merge = task.qf.gp_merge
-        l = []
+        self.mode = mode  # specify eihther b_u (bottom up) or t_d (top down)
+        self.constraints_monotone = []
+        self.results = []
+        self.task = []
+        # Future: There also is the option of a stable mode
+        # which never creates the prefix trees
+
+    def prepare_selectors(self, search_space, data):
+        selectors = []
+        assert len(search_space) > 0, "Provided searchspace was empty"
         for selector in search_space:
             cov_arr = selector.covers(data)
-            l.append((np.count_nonzero(cov_arr), selector, cov_arr))
-        l = [(size, selector, arr) for size, selector, arr in l if size > self.minSupp]
+            selectors.append((np.count_nonzero(cov_arr), selector, cov_arr))
 
-        s = sorted(l, reverse=True)
-        selectors_sorted = [selector for size, selector, arr in s]
-        arrs = np.vstack([arr for size, selector, arr in s]).T
+        selectors = [
+            (size, selector, arr)
+            for size, selector, arr in selectors
+            if all(
+                constraint.is_satisfied(arr, slice(None), data)
+                for constraint in self.constraints_monotone
+            )
+        ]
+        sorted_selectors = sorted(selectors, reverse=True)
+        self.remove_selectors_with_low_optimistic_estimate(
+            sorted_selectors, len(search_space)
+        )
+
+        selectors_sorted = [selector for size, selector, arr in sorted_selectors]
+        if len(selectors_sorted) == 0:
+            arrs = np.empty((0, 0), dtype=np.bool_)
+        else:
+            arrs = np.vstack([arr for size, selector, arr in sorted_selectors]).T
+        # print(selectors_sorted)
         return selectors_sorted, arrs
 
+    def remove_selectors_with_low_optimistic_estimate(self, s, search_space_size):
+        if not hasattr(self.task.qf, "optimistic_estimate"):
+            return
+        if search_space_size > self.task.result_set_size:
+            # remove selectors which have to lo of an optimistic estimate
+            # selectors_map = {selector : i for i,(_, selector, _) in enumerate(s)}
+            stats = []
+            for _, _, cov_arr in s:
+                statistics = self.task.qf.calculate_statistics(
+                    cov_arr, self.task.target, self.task.data
+                )
+                stats.append(statistics)
+                quality = self.task.qf.evaluate(
+                    cov_arr, self.task.target, self.task.data, statistics
+                )
+                ps.add_if_required(
+                    self.results, None, quality, self.task, statistics=statistics
+                )
+            del statistics
+            to_pop = []
+            min_quality = ps.minimum_required_quality(self.results, self.task)
+            for i, ((_, _, cov_arr), statistics) in enumerate(zip(s, stats)):
+                if (
+                    not self.task.qf.optimistic_estimate(
+                        cov_arr, self.task.target, self.task.data, statistics
+                    )
+                    > min_quality
+                ):
+                    to_pop.append(i)
+            self.task.min_quality = np.nextafter(
+                float(min_quality), self.task.min_quality
+            )
+            for i in reversed(to_pop):
+                s.pop(i)
+            self.results.clear()
+
     def nodes_to_cls_nodes(self, nodes):
         cls_nodes = defaultdict(list)
         for node in nodes:
             cls_nodes[node.cls].append(node)
         return cls_nodes
 
-
-    def execute(self, task):
-        assert(self.mode in ('b_u', 't_d'))
-        task.qf.calculate_constant_statistics(task)
+    def setup_from_quality_function(self, qf):
+        # pylint: disable=attribute-defined-outside-init
+        self.get_stats = qf.gp_get_stats
+        self.get_null_vector = qf.gp_get_null_vector
+        self.merge = qf.gp_merge
+        self.requires_cover_arr = qf.gp_requires_cover_arr
+        # pylint: enable=attribute-defined-outside-init
+
+    def setup_constraints(self, constraints, qf):
+        self.constraints_monotone = constraints
+        for constraint in self.constraints_monotone:
+            constraint.gp_prepare(qf)
+
+        if self.mode == "t_d" and len(self.constraints_monotone) == 0:
+            warnings.warn(
+                """Poor runtime expected: Top down method does not use
+                optimistic estimates and no constraints were provided""",
+                UserWarning,
+            )
+
+        if len(constraints) == 1:
+            self.check_constraints = constraints[0].gp_is_satisfied
+
+    def check_constraints(self, node):  # pylint: disable=method-hidden
+        return all(
+            constraint.gp_is_satisfied(node) for constraint in self.constraints_monotone
+        )
+
+    def setup(self, task):
+        self.task = task
+        task.qf.calculate_constant_statistics(task.data, task.target)
         self.depth = task.depth
-        selectors_sorted, arrs = self.prepare_selectors(task.search_space)
-        self.requires_cover_arr = task.qf.gp_requires_cover_arr
+        self.setup_constraints(task.constraints_monotone, task.qf)
 
+        self.setup_from_quality_function(task.qf)
+
+    def create_initial_tree(self, arrs):
         # Create tree
         root = self.GP_node(-1, -1, None, {}, self.get_null_vector())
         nodes = []
-        for row_index, row in self.tqdm(enumerate(arrs), 'creating tree', total=len(arrs)):
-            self.normal_insert(root, nodes, self.get_stats(row_index), np.nonzero(row)[0])
+        for row_index, row in self.tqdm(
+            enumerate(arrs), "creating tree", total=len(arrs)
+        ):
+            self.normal_insert(
+                root, nodes, self.get_stats(row_index), np.nonzero(row)[0]
+            )
         nodes.append(root)
+        return root, nodes
+
+    def execute(self, task):
+        assert self.mode in ("b_u", "t_d"), "mode needs to be either b_u or t_d"
+        self.setup(task)
+
+        selectors_sorted, arrs = self.prepare_selectors(task.search_space, task.data)
+        root, nodes = self.create_initial_tree(arrs)
 
         # mine tree
         cls_nodes = self.nodes_to_cls_nodes(nodes)
-        if self.mode == 'b_u':
-            patterns = self.recurse(cls_nodes, [])
-        elif self.mode == 't_d':
-            patterns = self.recurse_top_down(cls_nodes, root)
-        else:
-            raise RuntimeError('mode needs to be either b_u or t_d')
+        if self.mode == "b_u":
+            self.recurse(cls_nodes, tuple())
+        elif self.mode == "t_d":
+            results = self.recurse_top_down(cls_nodes, root)
+            results = self.calculate_quality_function_for_patterns(task, results, arrs)
+            for quality, sg, stats in results:
+                ps.add_if_required(
+                    self.results, sg, quality, self.task, statistics=stats
+                )
+        self.results = self.convert_results_to_subgroups(self.results, selectors_sorted)
+
+        self.results = ps.prepare_subgroup_discovery_result(self.results, task)
+        return ps.SubgroupDiscoveryResult(self.results, task)
+
+    def convert_results_to_subgroups(self, results, selectors_sorted):
+        new_result = []
+        for quality, indices, stats in results:
+            selectors = [selectors_sorted[i] for i in indices]
+            sg = ps.Conjunction(selectors)
+            new_result.append((quality, sg, stats))
+        return new_result
 
-        # compute quality functions
-        return self.calculate_quality_function_for_patterns(patterns, selectors_sorted, arrs)
-
-    def calculate_quality_function_for_patterns(self, patterns, selectors_sorted, arrs):
+    def calculate_quality_function_for_patterns(self, task, results, arrs):
         out = []
-        for indices, gp_params in self.tqdm(patterns, 'computing quality function',):
-            if len(indices) > 0:
-                selectors = [selectors_sorted[i] for i in indices]
-                #print(selectors, stats)
-                sg = ps.Conjunction(selectors)
-                if self.requires_cover_arr:
-                    statistics = task.qf.gp_get_params(np.all([arrs[i] for i in indices]), gp_params)
+        for indices, gp_params in self.tqdm(
+            results,
+            "computing quality function",
+        ):
+            if self.requires_cover_arr:
+                if len(indices) == 1:
+                    cover_arr = arrs[:, indices[0]]
                 else:
-                    statistics = task.qf.gp_get_params(None, gp_params)
-                #qual1 = task.qf.evaluate(sg, task.qf.calculate_statistics(sg, task.data))
-                qual2 = task.qf.evaluate(sg, statistics)
-                out.append((qual2, sg))
+                    cover_arr = np.all([arrs[:, i] for i in indices])
+                statistics = task.qf.gp_get_params(cover_arr, gp_params)
+                sg = cover_arr
+            else:
+                statistics = task.qf.gp_get_params(None, gp_params)
+                sg = None
+            # qual1 = task.qf.evaluate(sg, task.qf.calculate_statistics(sg, task.data))
+            qual2 = task.qf.evaluate(sg, task.target, task.data, statistics)
+            out.append((qual2, indices, statistics))
         return out
 
     def normal_insert(self, root, nodes, new_stats, classes):
         node = root
         for cls in classes:
             if cls not in node.children:
-                new_child = self.GP_node(cls, len(nodes), node, {}, self.get_null_vector())
+                new_child = self.GP_node(
+                    cls, len(nodes), node, {}, self.get_null_vector()
+                )
                 nodes.append(new_child)
                 node.children[cls] = new_child
             self.merge(node.stats, new_stats)
             node = node.children[cls]
         self.merge(node.stats, new_stats)
         return node
 
-    def insert_into_tree(self, root, nodes, new_stats, classes, max_depth):
-        ''' Creates a tree of a maximum depth = depth
-        '''
-        if len(classes) <= max_depth:
-            self.normal_insert(root, nodes, new_stats, classes)
-            return
-        for prefix in combinations(classes, max_depth -1):
-            node = self.normal_insert(root, nodes, new_stats, classes)
-            # do normal insert for prefix
-            index_for_remaining = classes.index(prefix) + 1
-            for cls in classes[index_for_remaining:]:
-                if cls not in node.children:
-                    new_child = self.GP_node(cls, len(nodes), node, {}, self.get_null_vector())
-                    nodes.append(new_child)
-                    node.children[cls] = new_child
-                    self.merge(node.stats, new_stats)
-
-
-    def check_constraints(self, node):
-        #return node[0] >= self.minSupp
-        return node['size'] >= self.minSupp
+    def add_if_required(self, prefix, gp_stats):
+        statistics = self.task.qf.gp_get_params(None, gp_stats)
+        quality = self.task.qf.evaluate(None, None, None, statistics)
+        ps.add_if_required(
+            self.results, prefix, quality, self.task, statistics=statistics
+        )
 
     def recurse(self, cls_nodes, prefix, is_single_path=False):
         if len(cls_nodes) == 0:
-            raise RuntimeError
-        results = []
-
-        results.append((prefix, cls_nodes[-1][0].stats))
+            raise RuntimeError  # pragma: no cover
+        self.add_if_required(prefix, cls_nodes[-1][0].stats)
         if len(prefix) >= self.depth:
-            return results
-        
+            return  # pragma: no cover
+
         stats_dict = self.get_stats_for_class(cls_nodes)
+        if not self.requires_cover_arr:
+            statistics = self.task.qf.gp_get_params(None, cls_nodes[-1][0].stats)
+            optimistic_estimate = self.task.qf.optimistic_estimate(
+                None, self.task.target, self.task.data, statistics
+            )
+            if not optimistic_estimate >= ps.minimum_required_quality(
+                self.results, self.task
+            ):
+                return
         if is_single_path:
-            root_stats = cls_nodes[-1][0].stats
-            del stats_dict[-1]
-            all_combinations = ps.powerset(stats_dict.keys(), max_length=self.depth - len(prefix))
-            
+            if len(cls_nodes) == 1 and -1 in cls_nodes:
+                return
+            del stats_dict[-1]  # remove root node
+            all_combinations = ps.powerset(
+                stats_dict.keys(), max_length=self.depth - len(prefix) + 1
+            )
+
             for comb in all_combinations:
-                results.append((prefix+comb, root_stats))
+                # it might still be, that stats_dict[comb[-1]] is wrong
+                # if that is the case then
+                # stats_dict[comb[0]] is correct
+                if len(comb) > 0:
+                    self.add_if_required(prefix + comb, stats_dict[comb[-1]])
         else:
             for cls, nodes in cls_nodes.items():
                 if cls >= 0:
                     if self.check_constraints(stats_dict[cls]):
                         if len(prefix) == (self.depth - 1):
-                            results.append(((*prefix, cls), stats_dict[cls]))
+                            self.add_if_required((*prefix, cls), stats_dict[cls])
                         else:
                             is_single_path_now = len(nodes) == 1
                             new_tree = self.create_new_tree_from_nodes(nodes)
                             if len(new_tree) > 0:
-                                results.extend(self.recurse(new_tree, (*prefix, cls), is_single_path_now))
-        return results
-
-    def get_prefixes_top_down(self, alpha, max_length):
-        if len(alpha) == 0:
-            return [()]
-        if len(alpha) == 1 or max_length == 1:
-            return [(alpha[0],)]
-        prefixes = [(alpha[0],)]
-        prefixes.extend([(alpha[0], *suffix) for suffix in self.get_prefixes_top_down(alpha[1:], max_length-1)])
-        return prefixes
-
+                                self.recurse(
+                                    new_tree, (*prefix, cls), is_single_path_now
+                                )
 
     def recurse_top_down(self, cls_nodes, root, depth_in=0):
+        # print(f"{depth_in}"+"\t"*depth_in+str(root.cls))
+        # print("init root", root.cls)
+        # print(depth_in)
+        # self.check_tree_is_ordered(root)
+        results = []
 
-        alpha = []
         curr_depth = depth_in
+        stats_dict = self.get_stats_for_class(cls_nodes)
+        is_valid_class = {
+            key: self.check_constraints(gp_stats)
+            for key, gp_stats in stats_dict.items()
+        }
+        # init_class = root.cls
+        # direct_child = None
+        init_root = root
+        alpha = []
         while True:
             if root.cls == -1:
-               pass
+                pass
             else:
                 alpha.append(root.cls)
             if len(root.children) == 1 and curr_depth <= self.depth:
-                curr_depth += 1
-                root = next(iter(root.children.values()))
+                # print(f"Path optmization {len(root.children)}")
+                #    curr_depth += 1
+
+                potential_root = next(iter(root.children.values()))
+                if is_valid_class[potential_root.cls]:
+                    root = potential_root
+                else:
+                    break
             else:
                 break
-        prefixes = self.get_prefixes_top_down(alpha, max_length=self.depth - depth_in + 1)
-
-        # Bug: If we have a longer path that branches. eg. consider the tree from items A - B - C and A - B - D
-        # and depth - depth_in == 2 then prefixes = [(A), (A, B)] but the sets
-        # (A, C) and (A, D) are also valid
-        # basically if we have prefixes of diffrent length this does not work properly
-        if len(root.children) == 0 or curr_depth >= self.depth:
-            results = []
-            stats_dict = self.get_stats_for_class(cls_nodes)
-            for prefix in prefixes:
-                cls = max(prefix)
-                if self.check_constraints(stats_dict[cls]):
-                    results.append((prefix, stats_dict[cls]))
-            return results
+        # self.get_prefixes_top_down(alpha,  max_length=self.depth - depth_in + 1) #
+        # assert len(alpha) > 0
+        prefixes = list(ps.powerset(alpha, max_length=self.depth - depth_in + 1))[1:]
+
+        # prefixes = list(map(lambda x: sum(x, tuple()), prefixes))
+        # print(root.cls, list(root.children), prefixes)
+        # print("AAA", list(cls_nodes.keys()))
+
+        if init_root.cls == -1:
+            prefixes.append(tuple())
+        for prefix in prefixes:
+            if len(prefix) == 0:
+                if is_valid_class[init_root.cls]:
+                    results.append((prefix, stats_dict[init_root.cls]))
+                continue
+            cls = prefix[-1]
+            if is_valid_class[cls]:
+                results.append((prefix, stats_dict[cls]))
+
+        # suffixes = [((), root.stats)]
+
+        suffixes = []
+        if curr_depth == (self.depth - 1):
+            # print(f"{depth_in}"+"\t"*depth_in+"B")
+            for cls, stats in stats_dict.items():
+                if cls < 0 or cls in alpha:
+                    continue
+                assert cls > max(
+                    alpha
+                ), f"{cls} {max(alpha)}, {alpha}, {list(stats_dict.keys())}"
+                suffixes.append(((cls,), stats))
         else:
-            suffixes = [((), root.stats)]
-            stats_dict = self.get_stats_for_class(cls_nodes)
-            for cls in cls_nodes:
-                if cls >= 0 and cls not in alpha:
-                    if self.check_constraints(stats_dict[cls]):
-                        # Future: There is also the possibility to compute the stats_dict of the prefix tree
-                        # without creating the prefix tree first
-                        # This might be useful if curr_depth == self.depth - 2
-                        # as we need not recreate the tree
-
-                        if curr_depth == (self.depth - 1):
-                            suffixes.append(((cls,), stats_dict[cls]))
-                        else:
-                            new_root, nodes = self.get_top_down_tree_for_class(cls_nodes, cls)
-                            if len(nodes) > 0:
-                                new_cls_nodes = self.nodes_to_cls_nodes(nodes)
-                                print("  " * curr_depth, cls, curr_depth, len(new_cls_nodes))
-                                suffixes.extend(self.recurse_top_down(new_cls_nodes, new_root, curr_depth+1))
-
-        return [((*pre, *(suf[0])), suf[1]) for pre, suf in itertools.product(prefixes, suffixes)]
-
-    def remove_infrequent_class(self, nodes, cls_nodes, stats_dict):
-        # returns cleaned tree
-
-        infrequent_classes = []
-        for cls in cls_nodes:
-            if not self.check_constraints(stats_dict[cls]):
-                infrequent_classes.append(cls)
-        infrequent_classes = sorted(infrequent_classes, reverse=True)
-        for cls in infrequent_classes:
-            for node_to_remove in cls_nodes[cls]:
-                self.merge_trees_top_down(nodes, node_to_remove.parent, node_to_remove)
-
-
+            # print(f"{depth_in}"+"\t"*depth_in+"A")
+            for cls in stats_dict:
+                if cls < 0 or cls in alpha:
+                    continue
+                if is_valid_class[cls]:
+                    # Future: There is also the possibility
+                    # to compute the stats_dict of the prefix tree
+                    # without creating the prefix tree first
+                    # This might be useful if curr_depth == self.depth - 2
+                    # as we need not recreate the tree
+                    new_root, nodes = self.get_top_down_tree_for_class(
+                        cls_nodes, cls, is_valid_class
+                    )
+                    # self.check_tree_is_ordered(new_root)
+                    # self.check_tree_is_ordered(init_root)
+                    if len(nodes) > 0:
+                        new_cls_nodes = self.nodes_to_cls_nodes(nodes)
+                        # new_dict = self.get_stats_for_class(new_cls_nodes)
+                        # for key, value in new_dict.items():
+                        #    if isinstance(stats_dict[key], dict):
+                        #        continue
+                        #    assert stats_dict[key][0]>=value[0], \
+                        #       f"{stats_dict[key][0]} {value[0]}"
+                        #    assert stats_dict[key][1]>=value[1], \
+                        #       f"{stats_dict[key][1]} {value[1]}"
+                        # print("  " * curr_depth, cls, curr_depth, len(new_cls_nodes))
+                        suffixes.extend(
+                            self.recurse_top_down(
+                                new_cls_nodes, new_root, curr_depth + 1
+                            )
+                        )
+        # if prefixes == [(12,), (13,)]:
+        #    print(f"{depth_in}"+"\t"*depth_in+ "pre, suf", prefixes)
+
+        # the combination below can be optimized to avoid the if
+        # by first grouping them by length
+        results.extend(
+            [
+                ((*pre, *suf), gp_stats)
+                for pre, (suf, gp_stats) in itertools.product(prefixes, suffixes)
+                if len(pre) + len(suf) <= self.depth
+                and (len(pre) == 0 or pre[-1] < suf[0])
+            ]
+        )
+        # if prefixes == [(12,), (13,)]:
+        #    print(f"{depth_in}"+"\t"*depth_in+ "results", results)
+        # print()
+        return results
 
-    def get_top_down_tree_for_class(self, cls_nodes, cls):
-        # Future: Can eventually also remove infrequent nodes already during tree creation
+    def check_tree_is_ordered(self, root, prefix=None):  # pragma: no cover
+        """Verify that the nodes of a tree are sorted in ascending order"""
+        if prefix is None:
+            prefix = []
+        s = {root.cls}
+        for cls, child in root.children.items():
+            assert child.cls > root.cls, f"{prefix} , {cls}"
+            s2 = self.check_tree_is_ordered(child, prefix + [cls])
+            s = s.union(s2)
+        return s
+
+    def get_top_down_tree_for_class(self, cls_nodes, cls, is_valid_class):
+        # Future: Can eventually also remove infrequent nodes already
+        # during tree creation
         base_root = None
         nodes = []
-        if len(cls_nodes[cls]) > 0:
-            base_root = self.create_copy_of_tree_top_down(cls_nodes[cls][0], nodes)
-            for other_root in cls_nodes[cls][1:]:
-                self.merge_trees_top_down(nodes, base_root, other_root)
+        if len(cls_nodes[cls]) > 0 and is_valid_class[cls]:
+            base_root = self.create_copy_of_tree_top_down(
+                cls_nodes[cls][0], nodes, is_valid_class=is_valid_class
+            )
+            for from_root in cls_nodes[cls][1:]:
+                self.merge_trees_top_down(nodes, base_root, from_root, is_valid_class)
         return base_root, nodes
 
-    def create_copy_of_tree_top_down(self, root, nodes=None, parent=None):
+    def create_copy_of_tree_top_down(
+        self, from_root, nodes=None, parent=None, is_valid_class=None
+    ):
         if nodes is None:
-            nodes = []
-        #if len(nodes) == 0:
+            nodes = []  # pragma: no cover
+        # if len(nodes) == 0:
         #    root_cls = -1
         children = {}
-        new_root = self.GP_node(root.cls, len(nodes), parent, children, root.stats.copy())
+        new_root = self.GP_node(
+            from_root.cls, len(nodes), parent, children, from_root.stats.copy()
+        )
         nodes.append(new_root)
-        for child_cls, child in root.children.items():
-            new_child = self.create_copy_of_tree_top_down(child, nodes, new_root)
-            children[child_cls] = new_child
+        for child_cls, child in from_root.children.items():
+            if is_valid_class is None or child_cls in is_valid_class:
+                new_child = self.create_copy_of_tree_top_down(
+                    child, nodes, new_root, is_valid_class=is_valid_class
+                )
+                children[child_cls] = new_child
         return new_root
 
-    def merge_trees_top_down(self, nodes, mutable_root, other_root):
-        self.merge(mutable_root.stats, other_root.stats)
-        for cls in other_root.children:
+    def merge_trees_top_down(self, nodes, mutable_root, from_root, is_valid_class):
+        self.merge(mutable_root.stats, from_root.stats)
+        for cls in from_root.children:
             if cls not in mutable_root.children:
-                self.create_copy_of_tree_top_down(other_root.children[cls], nodes, mutable_root)
+                new_child = self.create_copy_of_tree_top_down(
+                    from_root.children[cls],
+                    nodes,
+                    mutable_root,
+                    is_valid_class=is_valid_class,
+                )
+                mutable_root.children[cls] = new_child
             else:
-                self.merge_trees_top_down(nodes, mutable_root.children[cls], other_root.children[cls])
-        
+                self.merge_trees_top_down(
+                    nodes,
+                    mutable_root.children[cls],
+                    from_root.children[cls],
+                    is_valid_class=is_valid_class,
+                )
 
     def get_stats_for_class(self, cls_nodes):
         out = {}
         for key, nodes in cls_nodes.items():
             s = self.get_null_vector()
             for node in nodes:
                 self.merge(s, node.stats)
             out[key] = s
         return out
 
-
     def create_new_tree_from_nodes(self, nodes):
         new_nodes = {}
         for node in nodes:
             nodes_upwards = self.get_nodes_upwards(node)
             self.create_copy_of_path(nodes_upwards[1:], new_nodes, node.stats)
 
-        #self.remove_infrequent_nodes(new_nodes)
+        # self.remove_infrequent_nodes(new_nodes)
         cls_nodes = defaultdict(list)
         for new_node in new_nodes.values():
             cls_nodes[new_node.cls].append(new_node)
         return cls_nodes
 
-    def remove_infrequent_nodes(self, new_nodes):
-        keys = list(new_nodes.keys())
-        for key in keys:
-            node = new_nodes[key]
-            if node.stats["size"] < self.minSupp:
-                del new_nodes[key]
-
     def create_copy_of_path(self, nodes, new_nodes, stats):
         parent = None
         for node in reversed(nodes):
             if node.id not in new_nodes:
                 new_node = self.GP_node(node.cls, node.id, parent, {}, stats.copy())
                 new_nodes[node.id] = new_node
             else:
@@ -299,77 +482,24 @@
             path.append(ref)
             ref = ref.parent
             if ref is None:
                 break
         return path
 
     def to_file(self, task, path):
-        task.qf.calculate_constant_statistics(task)
-        self.depth = task.depth
-        selectors_sorted, arrs = self.prepare_selectors(task.search_space)
+        self.setup(task)
+        _, arrs = self.prepare_selectors(task.search_space, task.data)
 
         # Create tree
-        root = self.GP_node(-1, -1, None, {}, self.get_null_vector())
-        nodes = []
-        with open(path, 'w') as f:
-            for row_index, row in self.tqdm(enumerate(arrs), 'creating tree', total=len(arrs)):
-                #print(np.nonzero(row)[0])
-                f.write(" ".join(map(str, np.nonzero(row)[0])) + " "+ task.qf.gp_to_str(self.get_stats(row_index))+"\r\n")
-        
-
-if __name__ == '__main__':
-    from pysubgroup.tests.DataSets import get_credit_data
-    from pysubgroup import model_target
-
-    data = get_credit_data()
-    #warnings.filterwarnings("error")
-    print(data.columns)
-    searchSpace_Nominal = ps.create_nominal_selectors(data, ignore=['duration', 'credit_amount'])
-    searchSpace_Numeric = ps.create_numeric_selectors(data, ignore=['duration', 'credit_amount'])
-    searchSpace = searchSpace_Nominal + searchSpace_Numeric
-    target = ps.FITarget()
-    #QF=model_target.EMM_Likelihood(model_target.PolyRegression_ModelClass(x_name='duration', y_name='credit_amount'))
-    QF=ps.CountQF()
-    task = ps.SubgroupDiscoveryTask(data, target, searchSpace, result_set_size=200, depth=4, qf=QF)
-    GpGrowth(mode='b_u').to_file(task,'E:/tmp/gp_credit.txt')
-
-    import time
-    start_time = time.time()
-    gp = GpGrowth(mode='b_u').execute(task)
-    print("--- %s seconds ---" % (time.time() - start_time))
-    #gp = [(qual, sg) for qual, sg in gp if sg.depth <= task.depth]
-    gp = sorted(gp)
-    quit()
-
-    start_time = time.time()
-    dfs1 = ps.SimpleDFS().execute(task)
-    print("--- %s seconds ---" % (time.time() - start_time))
-    dfs = [(qual, sg.subgroup_description) for qual, sg in dfs1]
-    dfs = sorted(dfs, reverse=True)
-    gp = sorted(gp, reverse=True)
-
-    def better_sorted(l):
-        the_dict=defaultdict(list)
-        prev_key=l[0][0]
-        for key, val in l:
-            
-            if abs(prev_key-key)<10**-11:
-                the_dict[prev_key].append(val)
-            else:
-                the_dict[key].append(val)
-                prev_key = key
-        print(len(the_dict))
-        result = []
-        for key, vals in the_dict.items():
-            for val in sorted(vals):
-                result.append((key, val))
-        return result
-    dfs = better_sorted(dfs)
-    gp = better_sorted(gp)
-    gp = gp[:task.result_set_size]
-
-    for i, (l, r) in enumerate(zip(gp, dfs)):
-        print(i)
-        print('gp:', l)
-        print('df:', r)
-        assert(abs(l[0]-r[0]) < 10 ** -7)
-        assert(l[1] == r[1])
+        to_str = task.qf.gp_to_str
+        path = Path(path).absolute()
+        print(path)
+        with open(path, "w", encoding="utf-8") as f:
+            for row_index, row in self.tqdm(
+                enumerate(arrs), "creating tree", total=len(arrs)
+            ):
+                f.write(
+                    " ".join(map(str, np.nonzero(row)[0]))
+                    + " "
+                    + to_str(self.get_stats(row_index))
+                    + "\n"
+                )
```

### Comparing `pysubgroup-0.7.3/pysubgroup/measures.py` & `pysubgroup-0.7.6/src/pysubgroup/measures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,49 @@
-'''
+"""
 Created on 28.04.2016
 
 @author: lemmerfn
-'''
-from abc import ABC, abstractmethod
+"""
+from abc import ABC
 from collections import namedtuple
 from itertools import combinations
+
 import numpy as np
+
 import pysubgroup as ps
 
 
 class AbstractInterestingnessMeasure(ABC):
-
     # pylint: disable=no-member
     def ensure_statistics(self, subgroup, target, data, statistics=None):
         if not self.has_constant_statistics:
             self.calculate_constant_statistics(data, target)
         if any(not hasattr(statistics, attr) for attr in self.required_stat_attrs):
-            if getattr(subgroup, 'statistics', False):
+            if getattr(subgroup, "statistics", False):
                 return subgroup.statistics
-            else:
-                return self.calculate_statistics(subgroup, target, data, statistics)
+            return self.calculate_statistics(subgroup, target, data, statistics)
         return statistics
+
     # pylint: enable=no-member
-    #def optimistic_estimate_from_dataset(self, data, subgroup, weighting_attribute=None): #pylint: disable=unused-argument
+    # def optimistic_estimate_from_dataset(
+    #       self,
+    #       data,
+    #       subgroup,
+    #       weighting_attribute=None): #pylint: disable=unused-argument
     #    return float("inf")
 
 
 class BoundedInterestingnessMeasure(AbstractInterestingnessMeasure):
     pass
-    #@abstractmethod
-    #def optimistic_estimate_from_dataset(self, data, subgroup, weighting_attribute=None):
+    # @abstractmethod
+    # def optimistic_estimate_from_dataset(
+    #       self, data, subgroup, weighting_attribute=None):
     #    pass
 
 
-
 #####
 # FIX ME: This is currently not working anymore
 #####
 class CombinedInterestingnessMeasure(BoundedInterestingnessMeasure):
     def __init__(self, measures, weights=None):
         self.measures = measures
 
@@ -50,74 +55,112 @@
     def calculate_constant_statistics(self, data, target):
         pass
 
     def calculate_statistics(self, subgroup, target, data, cached_statistics=None):
         pass
 
     def evaluate(self, subgroup, target, data, statistics=None):
-        #FIX USE of constant statistics
-        return np.dot([m.evaluate(subgroup, target, data, None) for m in self.measures], self.weights)
+        # FIX USE of constant statistics
+        return np.dot(
+            [m.evaluate(subgroup, target, data, None) for m in self.measures],
+            self.weights,
+        )
 
     def optimistic_estimate(self, subgroup, target, data, statistics=None):
         # FIX USE of constant statistics
-        return np.dot([m.optimistic_estimate(subgroup, target, data, None) for m in self.measures], self.weights)
-
-    def evaluate_from_statistics(self, instances_dataset, positives_dataset, instances_subgroup, positives_subgroup):
-        return np.dot([m.evaluate_from_statistics(instances_dataset, positives_dataset, instances_subgroup, positives_subgroup) for m in self.measures], self.weights)
-
-    #def optimistic_estimate_from_statistics(self, instances_dataset, positives_dataset, instances_subgroup, positives_subgroup):
+        return np.dot(
+            [
+                m.optimistic_estimate(subgroup, target, data, None)
+                for m in self.measures
+            ],
+            self.weights,
+        )
+
+    def evaluate_from_statistics(
+        self,
+        instances_dataset,
+        positives_dataset,
+        instances_subgroup,
+        positives_subgroup,
+    ):
+        return np.dot(
+            [
+                m.evaluate_from_statistics(
+                    instances_dataset,
+                    positives_dataset,
+                    instances_subgroup,
+                    positives_subgroup,
+                )
+                for m in self.measures
+            ],
+            self.weights,
+        )
+
+    # def optimistic_estimate_from_statistics(
+    #       self,
+    #       instances_dataset,
+    #       positives_dataset,
+    #       instances_subgroup,
+    #       positives_subgroup):
     #    return np.dot(
-    #        [m.evaluate_from_statistics(instances_dataset, positives_dataset, instances_subgroup, positives_subgroup) for m in self.measures],
+    #        [m.evaluate_from_statistics(
+    #           instances_dataset,
+    #           positives_dataset,
+    #           instances_subgroup,
+    #           positives_subgroup)
+    #               for m in self.measures],
     #        self.weights)
 
 
 ##########
 # Filter
 ##########
 def unique_attributes(result_set, data):
     result = []
     used_attributes = []
-    for (q, sg) in result_set:
+    for q, sg in result_set:
         atts = sg.subgroup_description.get_attributes()
-        if atts not in used_attributes or all([ps.is_categorical_attribute(data, x) for x in atts]):
+        if atts not in used_attributes or all(
+            ps.is_categorical_attribute(data, x) for x in atts
+        ):
             result.append((q, sg))
             used_attributes.append(atts)
     return result
 
 
 def minimum_statistic_filter(result_set, statistic, minimum, data):
     result = []
-    for (q, sg) in result_set:
+    for q, sg in result_set:
         if len(sg.statistics) == 0:
             sg.calculate_statistics(data)
         if sg.statistics[statistic] >= minimum:
             result.append((q, sg))
     return result
 
 
 def minimum_quality_filter(result_set, minimum):
     result = []
-    for (q, sg) in result_set:
+    for q, sg in result_set:
         if q >= minimum:
             result.append((q, sg))
     return result
 
 
 def maximum_statistic_filter(result_set, statistic, maximum):
     result = []
-    for (q, sg) in result_set:
+    for q, sg in result_set:
         if sg.statistics[statistic] <= maximum:
             result.append((q, sg))
     return result
 
 
 def overlap_filter(result_set, data, similarity_level=0.9):
     result = []
     result_sgs = []
-    for (q, sg) in result_set:
+    for q, sg in result_set:
         if not overlaps_list(sg, result_sgs, data, similarity_level):
             result_sgs.append(sg)
             result.append((q, sg))
     return result
 
 
 def overlaps_list(sg, list_of_sgs, data, similarity_level=0.9):
@@ -143,48 +186,49 @@
         return hasattr(self.qf, name)
 
 
 #####
 # GeneralizationAware Interestingness Measures
 #####
 class GeneralizationAwareQF(AbstractInterestingnessMeasure):
-    ga_tuple = namedtuple('ga_tuple', ['subgroup_quality', 'generalisation_quality'])
+    ga_tuple = namedtuple("ga_tuple", ["subgroup_quality", "generalisation_quality"])
+
     def __init__(self, qf):
         self.qf = qf
 
         # this cache maps the representation of descriptions to tuples
         # the first entry is the quality and the second one is
         # the largest quality of all its predessors
         self.cache = {}
         self.has_constant_statistics = False
-        self.required_stat_attrs = ['subgroup_quality', 'generalisation_quality']
+        self.required_stat_attrs = ["subgroup_quality", "generalisation_quality"]
         self.q0 = 0
 
     def calculate_constant_statistics(self, data, target):
         self.cache = {}
         self.qf.calculate_constant_statistics(data, target)
         self.q0 = self.qf.evaluate(slice(None), target, data)
         self.has_constant_statistics = self.qf.has_constant_statistics
 
     def calculate_statistics(self, subgroup, target, data, statistics=None):
         sg_repr = repr(subgroup)
         if sg_repr in self.cache:
             return GeneralizationAwareQF.ga_tuple(*self.cache[sg_repr])
-        else:
-            (q_sg, q_prev) = self.get_qual_and_previous_qual(subgroup, target, data)
-            self.cache[sg_repr] = (q_sg, q_prev)
-            return GeneralizationAwareQF.ga_tuple(q_sg, q_prev)
+
+        (q_sg, q_prev) = self.get_qual_and_previous_qual(subgroup, target, data)
+        self.cache[sg_repr] = (q_sg, q_prev)
+        return GeneralizationAwareQF.ga_tuple(q_sg, q_prev)
 
     def get_qual_and_previous_qual(self, subgroup, target, data):
         q_subgroup = self.qf.evaluate(subgroup, target, data)
         max_q = 0
         selectors = subgroup.selectors
         if len(selectors) > 0:
             # compute quality of all generalizations
-            generalizations = combinations(selectors, len(selectors)-1)
+            generalizations = combinations(selectors, len(selectors) - 1)
 
             for sels in generalizations:
                 sgd = ps.Conjunction(list(sels))
                 (q_sg, q_prev) = self.calculate_statistics(sgd, target, data)
                 max_q = max(max_q, q_sg, q_prev)
         return (q_subgroup, max_q)
 
@@ -193,15 +237,16 @@
         return statistics.subgroup_quality - statistics.generalisation_quality
 
 
 #####
 # GeneralizationAware Interestingness Measures
 #####
 class GeneralizationAwareQF_stats(AbstractInterestingnessMeasure):
-    ga_tuple = namedtuple('ga_stats_tuple', ['subgroup_stats', 'generalisation_stats'])
+    ga_tuple = namedtuple("ga_stats_tuple", ["subgroup_stats", "generalisation_stats"])
+
     def __init__(self, qf):
         self.qf = qf
 
         # this cache maps the representation of descriptions to tuples
         # the first entry is the quality and the second one is
         # the largest quality of all its predecessors
         self.cache = {}
@@ -215,31 +260,33 @@
         self.stats0 = self.qf.calculate_statistics(slice(None), target, data)
         self.has_constant_statistics = self.qf.has_constant_statistics
 
     def calculate_statistics(self, subgroup, target, data, statistics=None):
         sg_repr = repr(subgroup)
         if sg_repr in self.cache:
             return GeneralizationAwareQF_stats.ga_tuple(*self.cache[sg_repr])
-        else:
-            (stats_sg, stats_prev) = self.get_stats_and_previous_stats(subgroup, target, data)
-            self.cache[sg_repr] = (stats_sg, stats_prev)
-            return GeneralizationAwareQF_stats.ga_tuple(stats_sg, stats_prev)
+
+        (stats_sg, stats_prev) = self.get_stats_and_previous_stats(
+            subgroup, target, data
+        )
+        self.cache[sg_repr] = (stats_sg, stats_prev)
+        return GeneralizationAwareQF_stats.ga_tuple(stats_sg, stats_prev)
 
     def get_stats_and_previous_stats(self, subgroup, target, data):
         stats_subgroup = self.qf.calculate_statistics(subgroup, target, data)
         max_stats = self.stats0
         selectors = subgroup.selectors
         if len(selectors) > 0:
             # compute quality of all generalizations
-            generalizations = combinations(selectors, len(selectors)-1)
+            generalizations = combinations(selectors, len(selectors) - 1)
 
             for sels in generalizations:
                 sgd = ps.Conjunction(list(sels))
                 (stats_sg, stats_prev) = self.calculate_statistics(sgd, target, data)
                 max_stats = self.get_max(max_stats, stats_sg, stats_prev)
         return (stats_subgroup, max_stats)
 
-    def evaluate(self, subgroup, statistics_or_data=None):
+    def evaluate(self, subgroup, target, data, statistics=None):
         raise NotImplementedError
 
     def get_max(self, *args):
-        raise NotImplementedError
+        raise NotImplementedError
```

### Comparing `pysubgroup-0.7.3/pysubgroup/model_target.py` & `pysubgroup-0.7.6/src/pysubgroup/model_target.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,117 +1,143 @@
 from collections import namedtuple
-from scipy.stats import norm
+
 import numpy as np
+
 import pysubgroup as ps
-beta_tuple = namedtuple('beta_tuple', ['beta', 'size'])
+
+beta_tuple = namedtuple("beta_tuple", ["beta", "size_sg"])
 
 
 class EMM_Likelihood(ps.AbstractInterestingnessMeasure):
-    tpl = namedtuple('EMM_Likelihood', ['model_params', 'subgroup_likelihood', 'inverse_likelihood', 'size'])
+    tpl = namedtuple(
+        "EMM_Likelihood",
+        ["model_params", "subgroup_likelihood", "inverse_likelihood", "size"],
+    )
+
     def __init__(self, model):
         self.model = model
         self.has_constant_statistics = False
         self.required_stat_attrs = EMM_Likelihood.tpl._fields
         self.data_size = None
 
-    def calculate_constant_statistics(self, task):
-        self.model.calculate_constant_statistics(task)
-        self.data_size = len(task.data)
+    def calculate_constant_statistics(self, data, target):
+        self.model.calculate_constant_statistics(data, target)
+        self.data_size = len(data)
         self.has_constant_statistics = True
 
-    def calculate_statistics(self, subgroup, data=None):
+    def calculate_statistics(
+        self, subgroup, target, data, statistics=None
+    ):  # pylint: disable=unused-argument
         cover_arr, sg_size = ps.get_cover_array_and_size(subgroup, self.data_size, data)
-
         params = self.model.fit(cover_arr, data)
         return self.get_tuple(sg_size, params, cover_arr)
 
     def get_tuple(self, sg_size, params, cover_arr):
-        #numeric stability?
-        all_likelihood = self.model.likelihood(params, np.ones(self.data_size, dtype=bool))
+        # numeric stability?
+        all_likelihood = self.model.likelihood(
+            params, np.ones(self.data_size, dtype=bool)
+        )
         sg_likelihood_sum = np.sum(all_likelihood[cover_arr])
         total_likelihood_sum = np.sum(all_likelihood)
         dataset_average = np.nan
         if (self.data_size - sg_size) > 0:
-            dataset_average = (total_likelihood_sum - sg_likelihood_sum)/(self.data_size - sg_size)
+            dataset_average = (total_likelihood_sum - sg_likelihood_sum) / (
+                self.data_size - sg_size
+            )
         sg_average = np.nan
         if sg_size > 0:
-            sg_average = sg_likelihood_sum/sg_size
+            sg_average = sg_likelihood_sum / sg_size
         return EMM_Likelihood.tpl(params, sg_average, dataset_average, sg_size)
 
-    def evaluate(self, subgroup, statistics=None):
-        statistics = self.ensure_statistics(subgroup, statistics)
-        #numeric stability?
+    def evaluate(self, subgroup, target, data, statistics=None):
+        statistics = self.ensure_statistics(subgroup, target, data, statistics)
+        # numeric stability?
         return statistics.subgroup_likelihood - statistics.inverse_likelihood
 
     def gp_get_params(self, cover_arr, v):
         params = self.model.gp_get_params(v)
-        sg_size = params.size
+        sg_size = params.size_sg
         return self.get_tuple(sg_size, params, cover_arr)
 
-
-    def supports_weights(self):
-        return False
-
-    def is_applicable(self, _):
+    @property
+    def gp_requires_cover_arr(self):
         return True
 
     def __getattr__(self, name):
         return getattr(self.model, name)
 
+
 class PolyRegression_ModelClass:
-    def __init__(self, x_name='x', y_name='y', degree=1):
+    def __init__(self, x_name="x", y_name="y", degree=1):
         self.x_name = x_name
         self.y_name = y_name
         if degree != 1:
-            raise ValueError('Currently only degree == 1 is supported')
+            raise ValueError("Currently only degree == 1 is supported")
         self.degree = degree
         self.x = None
         self.y = None
         self.has_constant_statistics = True
         super().__init__()
 
-    def calculate_constant_statistics(self, task):
-        data = task.data
+    def calculate_constant_statistics(
+        self, data, target
+    ):  # pylint: disable=unused-argument
         self.x = data[self.x_name].to_numpy()
         self.y = data[self.y_name].to_numpy()
         self.has_constant_statistics = True
 
     @staticmethod
     def gp_merge(u, v):
         v0 = v[0]
         u0 = u[0]
         if v0 == 0 or u0 == 0:
             d = 0
         else:
-            d = v0 * u0/(v0 + u0)*(v[1]/v0 - u[1]/u0)*(v[2]/v0 - u[2]/u0)
+            d = v0 * u0 / (v0 + u0) * (v[1] / v0 - u[1] / u0) * (v[2] / v0 - u[2] / u0)
         u += v
         u[3] += d
 
     def gp_get_null_vector(self):
         return np.zeros(5)
 
     def gp_get_stats(self, row_index):
         x = self.x[row_index]
-        return np.array([1, x, self.y[row_index], 0, x*x])
+        return np.array([1, x, self.y[row_index], 0, x * x])
 
     def gp_get_params(self, v):
         size = v[0]
         if size < self.degree:
             return beta_tuple(np.full(self.degree + 1, np.nan), size)
         v1 = v[1]
-        slope = v[0] * v[3] / (v[0]*v[4] - v1 * v1)
-        intersept = v[2]/v[0] - slope * v[1]/v[0]
+        slope = v[0] * v[3] / (v[0] * v[4] - v1 * v1)
+        intersept = v[2] / v[0] - slope * v[1] / v[0]
         return beta_tuple(np.array([slope, intersept]), v[0])
 
+    def gp_to_str(self, stats):
+        return " ".join(map(str, stats))
+
+    def gp_size_sg(self, stats):
+        return stats[0]
+
+    @property
+    def gp_requires_cover_arr(self):
+        return False
+
     def fit(self, subgroup, data=None):
         cover_arr, size = ps.get_cover_array_and_size(subgroup, len(self.x), data)
         if size <= self.degree + 1:
             return beta_tuple(np.full(self.degree + 1, np.nan), size)
-        return beta_tuple(np.polyfit(self.x[cover_arr], self.y[cover_arr], deg=self.degree), size)
+        return beta_tuple(
+            np.polyfit(self.x[cover_arr], self.y[cover_arr], deg=self.degree), size
+        )
 
     def likelihood(self, stats, sg):
+        from scipy.stats import norm  # pylint: disable=import-outside-toplevel
+
         if any(np.isnan(stats.beta)):
             return np.full(self.x[sg].shape, np.nan)
         return norm.pdf(np.polyval(stats.beta, self.x[sg]) - self.y[sg])
 
     def loglikelihood(self, stats, sg):
+        from scipy.stats import norm  # pylint: disable=import-outside-toplevel
+
         return norm.logpdf(np.polyval(stats.beta, self.x[sg]) - self.y[sg])
```

### Comparing `pysubgroup-0.7.3/pysubgroup/numeric_target.py` & `pysubgroup-0.7.6/src/pysubgroup/numeric_target.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,39 @@
-'''
+"""
 Created on 29.09.2017
 
 @author: lemmerfn
-'''
+"""
 import numbers
 from collections import namedtuple
 from functools import total_ordering
+
 import numpy as np
+
 import pysubgroup as ps
 
 
 @total_ordering
 class NumericTarget:
-
     statistic_types = (
-        'size_sg', 'size_dataset', 'mean_sg', 'mean_dataset', 'std_sg', 'std_dataset', 'median_sg', 'median_dataset',
-        'max_sg', 'max_dataset', 'min_sg', 'min_dataset', 'mean_lift', 'median_lift')
+        "size_sg",
+        "size_dataset",
+        "mean_sg",
+        "mean_dataset",
+        "std_sg",
+        "std_dataset",
+        "median_sg",
+        "median_dataset",
+        "max_sg",
+        "max_dataset",
+        "min_sg",
+        "min_dataset",
+        "mean_lift",
+        "median_lift",
+    )
 
     def __init__(self, target_variable):
         self.target_variable = target_variable
 
     def __repr__(self):
         return "T: " + str(self.target_variable)
 
@@ -40,518 +54,656 @@
         instances_subgroup = size_sg
         mean_sg = np.mean(sg_target_values)
         mean_dataset = np.mean(all_target_values)
         return (instances_dataset, mean_dataset, instances_subgroup, mean_sg)
 
     def calculate_statistics(self, subgroup, data, cached_statistics=None):
         if cached_statistics is None or not isinstance(cached_statistics, dict):
-            statistics = dict()
+            statistics = {}
         elif all(k in cached_statistics for k in NumericTarget.statistic_types):
             return cached_statistics
         else:
             statistics = cached_statistics
 
         cover_arr, _ = ps.get_cover_array_and_size(subgroup, len(data), data)
         all_target_values = data[self.target_variable].to_numpy()
         sg_target_values = all_target_values[cover_arr]
 
-        statistics['size_sg'] = len(sg_target_values)
-        statistics['size_dataset'] = len(data)
-        statistics['mean_sg'] = np.mean(sg_target_values)
-        statistics['mean_dataset'] = np.mean(all_target_values)
-        statistics['std_sg'] = np.std(sg_target_values)
-        statistics['std_dataset'] = np.std(all_target_values)
-        statistics['median_sg'] = np.median(sg_target_values)
-        statistics['median_dataset'] = np.median(all_target_values)
-        statistics['max_sg'] = np.max(sg_target_values)
-        statistics['max_dataset'] = np.max(all_target_values)
-        statistics['min_sg'] = np.min(sg_target_values)
-        statistics['min_dataset'] = np.min(all_target_values)
-        statistics['mean_lift'] = statistics['mean_sg'] / statistics['mean_dataset']
-        statistics['median_lift'] = statistics['median_sg'] / statistics['median_dataset']
+        statistics["size_sg"] = len(sg_target_values)
+        statistics["size_dataset"] = len(data)
+        statistics["mean_sg"] = np.mean(sg_target_values)
+        statistics["mean_dataset"] = np.mean(all_target_values)
+        statistics["std_sg"] = np.std(sg_target_values)
+        statistics["std_dataset"] = np.std(all_target_values)
+        statistics["median_sg"] = np.median(sg_target_values)
+        statistics["median_dataset"] = np.median(all_target_values)
+        statistics["max_sg"] = np.max(sg_target_values)
+        statistics["max_dataset"] = np.max(all_target_values)
+        statistics["min_sg"] = np.min(sg_target_values)
+        statistics["min_dataset"] = np.min(all_target_values)
+        statistics["mean_lift"] = statistics["mean_sg"] / statistics["mean_dataset"]
+        statistics["median_lift"] = (
+            statistics["median_sg"] / statistics["median_dataset"]
+        )
         return statistics
 
 
 class StandardQFNumeric(ps.BoundedInterestingnessMeasure):
-    tpl = namedtuple('StandardQFNumeric_parameters', ('size_sg', 'mean', 'estimate'))
+    tpl = namedtuple("StandardQFNumeric_parameters", ("size_sg", "mean", "estimate"))
+
     @staticmethod
     def standard_qf_numeric(a, _, mean_dataset, instances_subgroup, mean_sg):
-        return instances_subgroup ** a * (mean_sg - mean_dataset)
+        return instances_subgroup**a * (mean_sg - mean_dataset)
 
-    def __init__(self, a, invert=False, estimator='sum'):
+    def __init__(self, a, invert=False, estimator="sum"):
         if not isinstance(a, numbers.Number):
-            raise ValueError(f'a is not a number. Received a={a}')
+            raise ValueError(f"a is not a number. Received a={a}")
         self.a = a
         self.invert = invert
-        self.required_stat_attrs = ('size_sg', 'mean')
+        self.required_stat_attrs = ("size_sg", "mean")
         self.dataset_statistics = None
         self.all_target_values = None
         self.has_constant_statistics = False
-        if estimator == 'sum':
+        if estimator == "sum":
             self.estimator = StandardQFNumeric.Summation_Estimator(self)
-        elif estimator == 'average':
+        elif estimator == "average":
             self.estimator = StandardQFNumeric.Average_Estimator(self)
-        elif estimator == 'order':
+        elif estimator == "order":
             self.estimator = StandardQFNumeric.Ordering_Estimator(self)
         else:
-            raise ValueError('estimator is not one of the following: ' + str(['sum', 'average', 'order']))
+            raise ValueError(
+                "estimator is not one of the following: "
+                + str(["sum", "average", "order"])
+            )
 
     def calculate_constant_statistics(self, data, target):
         data = self.estimator.get_data(data, target)
         self.all_target_values = data[target.target_variable].to_numpy()
         target_mean = np.mean(self.all_target_values)
         data_size = len(data)
         self.dataset_statistics = StandardQFNumeric.tpl(data_size, target_mean, None)
         self.estimator.calculate_constant_statistics(data, target)
         self.has_constant_statistics = True
 
     def evaluate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
         dataset = self.dataset_statistics
-        return StandardQFNumeric.standard_qf_numeric(self.a, dataset.size_sg, dataset.mean, statistics.size_sg, statistics.mean)
+        return StandardQFNumeric.standard_qf_numeric(
+            self.a, dataset.size_sg, dataset.mean, statistics.size_sg, statistics.mean
+        )
 
     def calculate_statistics(self, subgroup, target, data, statistics=None):
-        cover_arr, sg_size = ps.get_cover_array_and_size(subgroup, len(self.all_target_values), data)
-        sg_mean = np.array([0])
+        cover_arr, sg_size = ps.get_cover_array_and_size(
+            subgroup, len(self.all_target_values), data
+        )
+        sg_mean = 0
         sg_target_values = 0
         if sg_size > 0:
             sg_target_values = self.all_target_values[cover_arr]
             sg_mean = np.mean(sg_target_values)
-            estimate = self.estimator.get_estimate(subgroup, sg_size, sg_mean, cover_arr, sg_target_values)
+            estimate = self.estimator.get_estimate(
+                subgroup, sg_size, sg_mean, cover_arr, sg_target_values
+            )
         else:
-            estimate = float('-inf')
+            estimate = float("-inf")
         return StandardQFNumeric.tpl(sg_size, sg_mean, estimate)
 
-
     def optimistic_estimate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
         return statistics.estimate
 
-
     class Summation_Estimator:
         def __init__(self, qf):
             self.qf = qf
             self.indices_greater_mean = None
             self.target_values_greater_mean = None
 
         def get_data(self, data, target):
             return data
 
-        def calculate_constant_statistics(self, data, target):  # pylint: disable=unused-argument
-            self.indices_greater_mean = self.qf.all_target_values > self.qf.dataset_statistics.mean
-            self.target_values_greater_mean = self.qf.all_target_values#[self.indices_greater_mean]
-
-        def get_estimate(self, subgroup, sg_size, sg_mean, cover_arr, _):  # pylint: disable=unused-argument
-            larger_than_mean = self.target_values_greater_mean[cover_arr][self.indices_greater_mean[cover_arr]]
+        def calculate_constant_statistics(
+            self, data, target
+        ):  # pylint: disable=unused-argument
+            self.indices_greater_mean = (
+                self.qf.all_target_values > self.qf.dataset_statistics.mean
+            )
+            self.target_values_greater_mean = (
+                self.qf.all_target_values
+            )  # [self.indices_greater_mean]
+
+        def get_estimate(
+            self, subgroup, sg_size, sg_mean, cover_arr, _
+        ):  # pylint: disable=unused-argument
+            larger_than_mean = self.target_values_greater_mean[cover_arr][
+                self.indices_greater_mean[cover_arr]
+            ]
             size_greater_mean = len(larger_than_mean)
             sum_greater_mean = np.sum(larger_than_mean)
 
-            return sum_greater_mean - size_greater_mean * self.qf.dataset_statistics.mean
+            return (
+                sum_greater_mean - size_greater_mean * self.qf.dataset_statistics.mean
+            )
 
     class Average_Estimator:
         def __init__(self, qf):
             self.qf = qf
             self.indices_greater_mean = None
             self.target_values_greater_mean = None
 
         def get_data(self, data, target):
             return data
 
-        def calculate_constant_statistics(self, data, target): # pylint: disable=unused-argument
-            self.indices_greater_mean = self.qf.all_target_values > self.qf.dataset_statistics.mean
+        def calculate_constant_statistics(
+            self, data, target
+        ):  # pylint: disable=unused-argument
+            self.indices_greater_mean = (
+                self.qf.all_target_values > self.qf.dataset_statistics.mean
+            )
             self.target_values_greater_mean = self.qf.all_target_values
 
-        def get_estimate(self, subgroup, sg_size, sg_mean, cover_arr, _): # pylint: disable=unused-argument
-            larger_than_mean = self.target_values_greater_mean[cover_arr][self.indices_greater_mean[cover_arr]]
+        def get_estimate(
+            self, subgroup, sg_size, sg_mean, cover_arr, _
+        ):  # pylint: disable=unused-argument
+            larger_than_mean = self.target_values_greater_mean[cover_arr][
+                self.indices_greater_mean[cover_arr]
+            ]
             size_greater_mean = len(larger_than_mean)
             max_greater_mean = np.sum(larger_than_mean)
 
-            return size_greater_mean ** self.qf.a * (max_greater_mean - self.qf.dataset_statistics.mean)
-
-
+            return size_greater_mean**self.qf.a * (
+                max_greater_mean - self.qf.dataset_statistics.mean
+            )
 
     class Ordering_Estimator:
         def __init__(self, qf):
             self.qf = qf
             self.indices_greater_mean = None
             self._get_estimate = self.get_estimate_numpy
             self.use_numba = True
             self.numba_in_place = False
 
         def get_data(self, data, target):
-            data.sort_values(target.get_attributes(), ascending=False, inplace=True)
+            data.sort_values(target.get_attributes()[0], ascending=False, inplace=True)
             return data
 
         def calculate_constant_statistics(self, data, target):
             if self.use_numba and not self.numba_in_place:
                 try:
-                    from numba import njit # pylint: disable=unused-import, import-outside-toplevel
-                    #print('StandardQf_Numeric: Using numba for speedup')
+                    from numba import (
+                        njit,  # pylint: disable=unused-import, import-outside-toplevel
+                    )
+
+                    # print('StandardQf_Numeric: Using numba for speedup')
                 except ImportError:
                     return
+
                 @njit
                 def estimate_numba(values_sg, a, mean_dataset):
                     n = 1
                     sum_values = 0
-                    max_value = -10 ** 10
+                    max_value = -(10**10)
                     for val in values_sg:
                         sum_values += val
                         mean_sg = sum_values / n
-                        quality = n ** a * (mean_sg - mean_dataset)
+                        quality = n**a * (mean_sg - mean_dataset)
                         if quality > max_value:
                             max_value = quality
                         n += 1
                     return max_value
+
                 self._get_estimate = estimate_numba
                 self.numba_in_place = True
 
-        def get_estimate(self, subgroup, sg_size, sg_mean, cover_arr, target_values_sg):  # pylint: disable=unused-argument
+        def get_estimate(
+            self, subgroup, sg_size, sg_mean, cover_arr, target_values_sg
+        ):  # pylint: disable=unused-argument
             if self.numba_in_place:
-                return self._get_estimate(target_values_sg, self.qf.a, self.qf.dataset_statistics.mean)
+                return self._get_estimate(
+                    target_values_sg, self.qf.a, self.qf.dataset_statistics.mean
+                )
             else:
-                return self._get_estimate(target_values_sg, self.qf.a, self.qf.dataset_statistics.mean)
+                return self._get_estimate(
+                    target_values_sg, self.qf.a, self.qf.dataset_statistics.mean
+                )
 
         def get_estimate_numpy(self, values_sg, _, mean_dataset):
             target_values_cs = np.cumsum(values_sg)
             sizes = np.arange(1, len(target_values_cs) + 1)
             mean_values = target_values_cs / sizes
             stats = StandardQFNumeric.tpl(sizes, mean_values, mean_dataset)
             qualities = self.qf.evaluate(None, None, None, stats)
             optimistic_estimate = np.max(qualities)
             return optimistic_estimate
 
 
-
 class StandardQFNumericMedian(ps.BoundedInterestingnessMeasure):
-    tpl = namedtuple('StandardQFNumericMedian_parameters', ('size_sg', 'median', 'estimate'))
+    tpl = namedtuple(
+        "StandardQFNumericMedian_parameters", ("size_sg", "median", "estimate")
+    )
+
     @staticmethod
     def standard_qf_numeric(a, _, median_dataset, instances_subgroup, median_sg):
-        return instances_subgroup ** a * (median_sg - median_dataset)
+        return instances_subgroup**a * (median_sg - median_dataset)
 
-    def __init__(self, a, invert=False, estimator='sum'):
+    def __init__(self, a, invert=False, estimator="sum"):
         if not isinstance(a, numbers.Number):
-            raise ValueError(f'a is not a number. Received a={a}')
+            raise ValueError(f"a is not a number. Received a={a}")
         self.a = a
         self.invert = invert
-        self.required_stat_attrs = ('size_sg', 'median')
+        self.required_stat_attrs = ("size_sg", "median")
         self.dataset_statistics = None
         self.all_target_values = None
         self.has_constant_statistics = False
-        if estimator == 'sum':
+        if estimator == "sum":
             self.estimator = StandardQFNumericMedian.Summation_Estimator(self)
-        elif estimator == 'average':
+        elif estimator == "average":
             self.estimator = StandardQFNumericMedian.Average_Estimator(self)
-        elif estimator == 'order':
+        elif estimator == "order":
             self.estimator = StandardQFNumericMedian.Ordering_Estimator(self)
         else:
-            raise ValueError('estimator is not one of the following: ' + str(['sum', 'average', 'order']))
+            raise ValueError(
+                "estimator is not one of the following: "
+                + str(["sum", "average", "order"])
+            )
 
     def calculate_constant_statistics(self, data, target):
         data = self.estimator.get_data(data, target)
         self.all_target_values = data[target.target_variable].to_numpy()
         target_median = np.median(self.all_target_values)
         data_size = len(data)
-        self.dataset_statistics = StandardQFNumericMedian.tpl(data_size, target_median, None)
+        self.dataset_statistics = StandardQFNumericMedian.tpl(
+            data_size, target_median, None
+        )
         self.estimator.calculate_constant_statistics(data, target)
         self.has_constant_statistics = True
 
     def evaluate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
         dataset = self.dataset_statistics
-        return StandardQFNumericMedian.standard_qf_numeric(self.a, dataset.size_sg, dataset.median, statistics.size_sg, statistics.median)
+        return StandardQFNumericMedian.standard_qf_numeric(
+            self.a,
+            dataset.size_sg,
+            dataset.median,
+            statistics.size_sg,
+            statistics.median,
+        )
 
     def calculate_statistics(self, subgroup, target, data, statistics=None):
-        cover_arr, sg_size = ps.get_cover_array_and_size(subgroup, len(self.all_target_values), data)
+        cover_arr, sg_size = ps.get_cover_array_and_size(
+            subgroup, len(self.all_target_values), data
+        )
         sg_median = np.array([0])
         sg_target_values = 0
         if sg_size > 0:
             sg_target_values = self.all_target_values[cover_arr]
             sg_median = np.median(sg_target_values)
-            estimate = self.estimator.get_estimate(subgroup, sg_size, sg_median, cover_arr, sg_target_values)
+            estimate = self.estimator.get_estimate(
+                subgroup, sg_size, sg_median, cover_arr, sg_target_values
+            )
         else:
-            estimate = float('-inf')
+            estimate = float("-inf")
         return StandardQFNumericMedian.tpl(sg_size, sg_median, estimate)
 
-
     def optimistic_estimate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
         return statistics.estimate
 
-
     class Summation_Estimator:
         def __init__(self, qf):
             self.qf = qf
             self.indices_greater_median = None
             self.target_values_greater_median = None
 
         def get_data(self, data, target):
             return data
 
-        def calculate_constant_statistics(self, data, target):  # pylint: disable=unused-argument
-            self.indices_greater_median = self.qf.all_target_values > self.qf.dataset_statistics.median
-            self.target_values_greater_median = self.qf.all_target_values#[self.indices_greater_median]
-
-        def get_estimate(self, subgroup, sg_size, sg_median, cover_arr, _):  # pylint: disable=unused-argument
-            larger_than_median = self.target_values_greater_median[cover_arr][self.indices_greater_median[cover_arr]]
+        def calculate_constant_statistics(
+            self, data, target
+        ):  # pylint: disable=unused-argument
+            self.indices_greater_median = (
+                self.qf.all_target_values > self.qf.dataset_statistics.median
+            )
+            self.target_values_greater_median = (
+                self.qf.all_target_values
+            )  # [self.indices_greater_median]
+
+        def get_estimate(
+            self, subgroup, sg_size, sg_median, cover_arr, _
+        ):  # pylint: disable=unused-argument
+            larger_than_median = self.target_values_greater_median[cover_arr][
+                self.indices_greater_median[cover_arr]
+            ]
             size_greater_median = len(larger_than_median)
             sum_greater_median = np.sum(larger_than_median)
 
-            return sum_greater_median - size_greater_median * self.qf.dataset_statistics.median
+            return (
+                sum_greater_median
+                - size_greater_median * self.qf.dataset_statistics.median
+            )
 
     class Average_Estimator:
         def __init__(self, qf):
             self.qf = qf
             self.indices_greater_mean = None
             self.target_values_greater_mean = None
 
         def get_data(self, data, target):
             return data
 
-        def calculate_constant_statistics(self, data, target): # pylint: disable=unused-argument
-            self.indices_greater_mean = self.qf.all_target_values > self.qf.dataset_statistics.mean
+        def calculate_constant_statistics(
+            self, data, target
+        ):  # pylint: disable=unused-argument
+            self.indices_greater_mean = (
+                self.qf.all_target_values > self.qf.dataset_statistics.mean
+            )
             self.target_values_greater_mean = self.qf.all_target_values
 
-        def get_estimate(self, subgroup, sg_size, sg_mean, cover_arr, _): # pylint: disable=unused-argument
-            larger_than_mean = self.target_values_greater_mean[cover_arr][self.indices_greater_mean[cover_arr]]
+        def get_estimate(
+            self, subgroup, sg_size, sg_mean, cover_arr, _
+        ):  # pylint: disable=unused-argument
+            larger_than_mean = self.target_values_greater_mean[cover_arr][
+                self.indices_greater_mean[cover_arr]
+            ]
             size_greater_mean = len(larger_than_mean)
             max_greater_mean = np.sum(larger_than_mean)
 
-            return size_greater_mean ** self.qf.a * (max_greater_mean - self.qf.dataset_statistics.mean)
-
-
+            return size_greater_mean**self.qf.a * (
+                max_greater_mean - self.qf.dataset_statistics.mean
+            )
 
     class Ordering_Estimator:
         def __init__(self, qf):
             self.qf = qf
             self.indices_greater_mean = None
             self._get_estimate = self.get_estimate_numpy
             self.use_numba = True
             self.numba_in_place = False
 
         def get_data(self, data, target):
-            data.sort_values(target.get_attributes(), ascending=False, inplace=True)
+            data.sort_values(target.get_attributes()[0], ascending=False, inplace=True)
             return data
 
         def calculate_constant_statistics(self, data, target):
             if self.use_numba and not self.numba_in_place:
                 try:
-                    from numba import njit # pylint: disable=unused-import, import-outside-toplevel
-                    #print('StandardQf_Numeric: Using numba for speedup')
+                    from numba import (
+                        njit,  # pylint: disable=unused-import, import-outside-toplevel
+                    )
+
+                    # print('StandardQf_Numeric: Using numba for speedup')
                 except ImportError:
                     return
+
                 @njit
                 def estimate_numba(values_sg, a, mean_dataset):
                     n = 1
                     sum_values = 0
-                    max_value = -10 ** 10
+                    max_value = -(10**10)
                     for val in values_sg:
                         sum_values += val
                         mean_sg = sum_values / n
-                        quality = n ** a * (mean_sg - mean_dataset)
+                        quality = n**a * (mean_sg - mean_dataset)
                         if quality > max_value:
                             max_value = quality
                         n += 1
                     return max_value
+
                 self._get_estimate = estimate_numba
                 self.numba_in_place = True
 
-        def get_estimate(self, subgroup, sg_size, sg_mean, cover_arr, target_values_sg):  # pylint: disable=unused-argument
+        def get_estimate(
+            self, subgroup, sg_size, sg_mean, cover_arr, target_values_sg
+        ):  # pylint: disable=unused-argument
             if self.numba_in_place:
-                return self._get_estimate(target_values_sg, self.qf.a, self.qf.dataset_statistics.mean)
+                return self._get_estimate(
+                    target_values_sg, self.qf.a, self.qf.dataset_statistics.mean
+                )
             else:
-                return self._get_estimate(target_values_sg, self.qf.a, self.qf.dataset_statistics.mean)
+                return self._get_estimate(
+                    target_values_sg, self.qf.a, self.qf.dataset_statistics.mean
+                )
 
         def get_estimate_numpy(self, values_sg, _, mean_dataset):
             target_values_cs = np.cumsum(values_sg)
             sizes = np.arange(1, len(target_values_cs) + 1)
             mean_values = target_values_cs / sizes
             stats = StandardQFNumericMedian.tpl(sizes, mean_values, mean_dataset)
             qualities = self.qf.evaluate(None, None, None, stats)
             optimistic_estimate = np.max(qualities)
             return optimistic_estimate
 
 
 class StandardQFNumericTscore(ps.BoundedInterestingnessMeasure):
-    tpl = namedtuple('StandardQFNumericTscore_parameters', ('size_sg', 'mean', 'std' , 'estimate'))
+    tpl = namedtuple(
+        "StandardQFNumericTscore_parameters", ("size_sg", "mean", "std", "estimate")
+    )
+
     @staticmethod
     def standard_qf_numeric(a, _, mean_dataset, instances_subgroup, mean_sg, std_sg):
-        if std_sg == 0 :
+        if std_sg == 0:
             return 0
-        else :
-            return (instances_subgroup ** 0.5 * (mean_sg - mean_dataset)) / std_sg 
+        else:
+            return (instances_subgroup**0.5 * (mean_sg - mean_dataset)) / std_sg
 
-    def __init__(self, a, invert=False, estimator='sum'):
+    def __init__(self, a, invert=False, estimator="sum"):
         if not isinstance(a, numbers.Number):
-            raise ValueError(f'a is not a number. Received a={a}')
+            raise ValueError(f"a is not a number. Received a={a}")
         self.a = a
         self.invert = invert
-        self.required_stat_attrs = ('size_sg', 'mean', 'std')
+        self.required_stat_attrs = ("size_sg", "mean", "std")
         self.dataset_statistics = None
         self.all_target_values = None
         self.has_constant_statistics = False
-        if estimator == 'sum':
+        if estimator == "sum":
             self.estimator = StandardQFNumericTscore.Summation_Estimator(self)
-        elif estimator == 'average':
+        elif estimator == "average":
             self.estimator = StandardQFNumericTscore.Average_Estimator(self)
-        elif estimator == 'order':
+        elif estimator == "order":
             self.estimator = StandardQFNumericTscore.Ordering_Estimator(self)
         else:
-            raise ValueError('estimator is not one of the following: ' + str(['sum', 'average', 'order']))
+            raise ValueError(
+                "estimator is not one of the following: "
+                + str(["sum", "average", "order"])
+            )
 
     def calculate_constant_statistics(self, data, target):
         data = self.estimator.get_data(data, target)
         self.all_target_values = data[target.target_variable].to_numpy()
         target_mean = np.mean(self.all_target_values)
         target_std = np.std(self.all_target_values)
         data_size = len(data)
-        self.dataset_statistics = StandardQFNumericTscore.tpl(data_size, target_mean, target_std, None)
+        self.dataset_statistics = StandardQFNumericTscore.tpl(
+            data_size, target_mean, target_std, None
+        )
         self.estimator.calculate_constant_statistics(data, target)
         self.has_constant_statistics = True
 
     def evaluate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
         dataset = self.dataset_statistics
-        return StandardQFNumericTscore.standard_qf_numeric(self.a, dataset.size_sg, dataset.mean, statistics.size_sg, statistics.mean, statistics.std)
+        return StandardQFNumericTscore.standard_qf_numeric(
+            self.a,
+            dataset.size_sg,
+            dataset.mean,
+            statistics.size_sg,
+            statistics.mean,
+            statistics.std,
+        )
 
     def calculate_statistics(self, subgroup, target, data, statistics=None):
-        cover_arr, sg_size = ps.get_cover_array_and_size(subgroup, len(self.all_target_values), data)
+        cover_arr, sg_size = ps.get_cover_array_and_size(
+            subgroup, len(self.all_target_values), data
+        )
         sg_mean = np.array([0])
         sg_std = np.array([0])
         sg_target_values = 0
         if sg_size > 0:
             sg_target_values = self.all_target_values[cover_arr]
             sg_mean = np.mean(sg_target_values)
             sg_std = np.std(sg_target_values)
-            estimate = self.estimator.get_estimate(subgroup, sg_size, sg_mean, cover_arr, sg_target_values)
+            estimate = self.estimator.get_estimate(
+                subgroup, sg_size, sg_mean, cover_arr, sg_target_values
+            )
         else:
-            estimate = float('-inf')
+            estimate = float("-inf")
         return StandardQFNumericTscore.tpl(sg_size, sg_mean, sg_std, estimate)
 
-
     def optimistic_estimate(self, subgroup, target, data, statistics=None):
         statistics = self.ensure_statistics(subgroup, target, data, statistics)
         return statistics.estimate
 
-
     class Summation_Estimator:
         def __init__(self, qf):
             self.qf = qf
             self.indices_greater_mean = None
             self.target_values_greater_mean = None
 
         def get_data(self, data, target):
             return data
 
-        def calculate_constant_statistics(self, data, target):  # pylint: disable=unused-argument
-            self.indices_greater_mean = self.qf.all_target_values > self.qf.dataset_statistics.mean
-            self.target_values_greater_mean = self.qf.all_target_values#[self.indices_greater_mean]
-
-        def get_estimate(self, subgroup, sg_size, sg_mean, cover_arr, _):  # pylint: disable=unused-argument
-            larger_than_mean = self.target_values_greater_mean[cover_arr][self.indices_greater_mean[cover_arr]]
+        def calculate_constant_statistics(
+            self, data, target
+        ):  # pylint: disable=unused-argument
+            self.indices_greater_mean = (
+                self.qf.all_target_values > self.qf.dataset_statistics.mean
+            )
+            self.target_values_greater_mean = (
+                self.qf.all_target_values
+            )  # [self.indices_greater_mean]
+
+        def get_estimate(
+            self, subgroup, sg_size, sg_mean, cover_arr, _
+        ):  # pylint: disable=unused-argument
+            larger_than_mean = self.target_values_greater_mean[cover_arr][
+                self.indices_greater_mean[cover_arr]
+            ]
             size_greater_mean = len(larger_than_mean)
             sum_greater_mean = np.sum(larger_than_mean)
 
-            return sum_greater_mean - size_greater_mean * self.qf.dataset_statistics.mean
+            return (
+                sum_greater_mean - size_greater_mean * self.qf.dataset_statistics.mean
+            )
 
     class Average_Estimator:
         def __init__(self, qf):
             self.qf = qf
             self.indices_greater_mean = None
             self.target_values_greater_mean = None
 
         def get_data(self, data, target):
             return data
 
-        def calculate_constant_statistics(self, data, target): # pylint: disable=unused-argument
-            self.indices_greater_mean = self.qf.all_target_values > self.qf.dataset_statistics.mean
+        def calculate_constant_statistics(
+            self, data, target
+        ):  # pylint: disable=unused-argument
+            self.indices_greater_mean = (
+                self.qf.all_target_values > self.qf.dataset_statistics.mean
+            )
             self.target_values_greater_mean = self.qf.all_target_values
 
-        def get_estimate(self, subgroup, sg_size, sg_mean, cover_arr, _): # pylint: disable=unused-argument
-            larger_than_mean = self.target_values_greater_mean[cover_arr][self.indices_greater_mean[cover_arr]]
+        def get_estimate(
+            self, subgroup, sg_size, sg_mean, cover_arr, _
+        ):  # pylint: disable=unused-argument
+            larger_than_mean = self.target_values_greater_mean[cover_arr][
+                self.indices_greater_mean[cover_arr]
+            ]
             size_greater_mean = len(larger_than_mean)
             max_greater_mean = np.sum(larger_than_mean)
 
-            return size_greater_mean ** self.qf.a * (max_greater_mean - self.qf.dataset_statistics.mean)
-
-
+            return size_greater_mean**self.qf.a * (
+                max_greater_mean - self.qf.dataset_statistics.mean
+            )
 
     class Ordering_Estimator:
         def __init__(self, qf):
             self.qf = qf
             self.indices_greater_mean = None
             self._get_estimate = self.get_estimate_numpy
             self.use_numba = True
             self.numba_in_place = False
 
         def get_data(self, data, target):
-            data.sort_values(target.get_attributes(), ascending=False, inplace=True)
+            data.sort_values(target.get_attributes()[0], ascending=False, inplace=True)
             return data
 
         def calculate_constant_statistics(self, data, target):
             if self.use_numba and not self.numba_in_place:
                 try:
-                    from numba import njit # pylint: disable=unused-import, import-outside-toplevel
-                    #print('StandardQf_Numeric: Using numba for speedup')
+                    from numba import (
+                        njit,  # pylint: disable=unused-import, import-outside-toplevel
+                    )
+
+                    # print('StandardQf_Numeric: Using numba for speedup')
                 except ImportError:
                     return
+
                 @njit
                 def estimate_numba(values_sg, a, mean_dataset):
                     n = 1
                     sum_values = 0
-                    max_value = -10 ** 10
+                    max_value = -(10**10)
                     for val in values_sg:
                         sum_values += val
                         mean_sg = sum_values / n
-                        quality = n ** a * (mean_sg - mean_dataset)
+                        quality = n**a * (mean_sg - mean_dataset)
                         if quality > max_value:
                             max_value = quality
                         n += 1
                     return max_value
+
                 self._get_estimate = estimate_numba
                 self.numba_in_place = True
 
-        def get_estimate(self, subgroup, sg_size, sg_mean, cover_arr, target_values_sg):  # pylint: disable=unused-argument
+        def get_estimate(
+            self, subgroup, sg_size, sg_mean, cover_arr, target_values_sg
+        ):  # pylint: disable=unused-argument
             if self.numba_in_place:
-                return self._get_estimate(target_values_sg, self.qf.a, self.qf.dataset_statistics.mean)
+                return self._get_estimate(
+                    target_values_sg, self.qf.a, self.qf.dataset_statistics.mean
+                )
             else:
-                return self._get_estimate(target_values_sg, self.qf.a, self.qf.dataset_statistics.mean)
+                return self._get_estimate(
+                    target_values_sg, self.qf.a, self.qf.dataset_statistics.mean
+                )
 
         def get_estimate_numpy(self, values_sg, _, mean_dataset):
             target_values_cs = np.cumsum(values_sg)
             sizes = np.arange(1, len(target_values_cs) + 1)
             mean_values = target_values_cs / sizes
             stats = StandardQFNumericTscore.tpl(sizes, mean_values, mean_dataset)
             qualities = self.qf.evaluate(None, None, None, stats)
             optimistic_estimate = np.max(qualities)
             return optimistic_estimate
 
 
 # TODO Update to new format
-#class GAStandardQFNumeric(ps.AbstractInterestingnessMeasure):
+# class GAStandardQFNumeric(ps.AbstractInterestingnessMeasure):
 #    def __init__(self, a, invert=False):
 #        self.a = a
 #        self.invert = invert
 #
 #    def evaluate_from_dataset(self, data, subgroup, weighting_attribute=None):
-#        (instances_dataset, _, instances_subgroup, mean_sg) = subgroup.get_base_statistics(data, weighting_attribute)
+#        (instances_dataset, _, instances_subgroup, mean_sg) = \
+#           subgroup.get_base_statistics(data, weighting_attribute)
 #        if instances_subgroup in (0, instances_dataset):
 #            return 0
 #        max_mean = get_max_generalization_mean(data, subgroup, weighting_attribute)
 #        relative_size = (instances_subgroup / instances_dataset)
-#        return ps.conditional_invert(relative_size ** self.a * (mean_sg - max_mean), self.invert)
+#        return ps.conditional_invert(
+#           relative_size ** self.a * (mean_sg - max_mean), self.invert)
 
 #    def supports_weights(self):
 #        return True
 
 #    def is_applicable(self, subgroup):
 #        return isinstance(subgroup.target, NumericTarget)
 
 
-#def get_max_generalization_mean(data, subgroup, weighting_attribute=None):
+# def get_max_generalization_mean(data, subgroup, weighting_attribute=None):
 #    selectors = subgroup.subgroup_description.selectors
 #    generalizations = ps.powerset(selectors)
 #    max_mean = 0
 #    for sels in generalizations:
 #        sg = ps.Subgroup(subgroup.target, ps.Conjunction(list(sels)))
 #        mean_sg = sg.get_base_statistics(data, weighting_attribute)[3]
 #        max_mean = max(max_mean, mean_sg)
-#    return max_mean
+#    return max_mean
```

### Comparing `pysubgroup-0.7.3/pysubgroup/refinement_operator.py` & `pysubgroup-0.7.6/src/pysubgroup/refinement_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-import pysubgroup as ps
 from collections import defaultdict
 from itertools import chain
-import random
+
+
 class RefinementOperator:
     pass
 
 
 class StaticSpecializationOperator:
     def __init__(self, selectors):
         search_space_dict = defaultdict(list)
         for selector in selectors:
             search_space_dict[selector.attribute_name].append(selector)
         self.search_space = list(search_space_dict.values())
-        self.search_space_index = {key: i for i, key in enumerate(search_space_dict.keys())}
+        self.search_space_index = {
+            key: i for i, key in enumerate(search_space_dict.keys())
+        }
 
     def refinements(self, subgroup):
         if subgroup.depth > 0:
-            index_of_last = self.search_space_index[subgroup._selectors[-1].attribute_name]
-            new_selectors = chain.from_iterable(self.search_space[index_of_last + 1:])
+            index_of_last = self.search_space_index[
+                subgroup._selectors[-1].attribute_name
+            ]
+            new_selectors = chain.from_iterable(self.search_space[index_of_last + 1 :])
         else:
             new_selectors = chain.from_iterable(self.search_space)
 
         return (subgroup & sel for sel in new_selectors)
 
 
 class StaticGeneralizationOperator:
     def __init__(self, selectors):
         self.search_space = selectors
 
     def refinements(self, sG):
-        index_of_last_selector = min(self.search_space.index(sG._selectors[-1]), len(self.search_space) - 1)
-        new_selectors = self.search_space[index_of_last_selector + 1:]
+        index_of_last_selector = min(
+            self.search_space.index(sG._selectors[-1]), len(self.search_space) - 1
+        )
+        new_selectors = self.search_space[index_of_last_selector + 1 :]
 
         return (sG | sel for sel in new_selectors)
```

### Comparing `pysubgroup-0.7.3/pysubgroup/representations.py` & `pysubgroup-0.7.6/src/pysubgroup/representations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,199 +1,193 @@
 import numpy as np
-import pysubgroup as ps
 
+from pysubgroup.subgroup_description import Conjunction, Disjunction
 
 
-
-class RepresentationBase():
+class RepresentationBase:
     def __init__(self, new_conjunction, selectors_to_patch):
         self._new_conjunction = new_conjunction
         self.previous_conjunction = None
         self.selectors_to_patch = selectors_to_patch
 
     def patch_all_selectors(self):
         for sel in self.selectors_to_patch:
             self.patch_selector(sel)
 
-    def patch_selector(self, sel):
-        raise NotImplementedError
+    def patch_selector(self, sel):  # pragma: no cover
+        raise NotImplementedError()  # pragma: no cover
 
     def patch_classes(self):
         pass
 
     def undo_patch_classes(self):
         pass
 
     def __enter__(self):
         self.patch_classes()
         self.patch_all_selectors()
         return self
 
-
-    def __exit__(self, * args):
+    def __exit__(self, *args):
         self.undo_patch_classes()
 
 
-
-class BitSet_Conjunction(ps.Conjunction):
+class BitSet_Conjunction(Conjunction):
     n_instances = 0
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.representation = self.compute_representation()
 
     def compute_representation(self):
-                # empty description ==> return a list of all '1's
+        # empty description ==> return a list of all '1's
         if not self._selectors:
             return np.full(BitSet_Conjunction.n_instances, True, dtype=bool)
         # non-empty description
         return np.all([sel.representation for sel in self._selectors], axis=0)
 
     @property
     def size_sg(self):
         return np.count_nonzero(self.representation)
 
     def append_and(self, to_append):
         super().append_and(to_append)
-        self.representation = np.logical_and(self.representation, to_append.representation)
+        self.representation = np.logical_and(
+            self.representation, to_append.representation
+        )
 
     @property
     def __array_interface__(self):
         return self.representation.__array_interface__
 
 
-
-class BitSet_Disjunction(ps.Disjunction):
+class BitSet_Disjunction(Disjunction):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.representation = self.compute_representation()
 
     def compute_representation(self):
-                # empty description ==> return a list of all '1's
+        # empty description ==> return a list of all '1's
         if not self._selectors:
             return np.full(BitSet_Conjunction.n_instances, False, dtype=bool)
         # non-empty description
         return np.any([sel.representation for sel in self._selectors], axis=0)
 
     @property
     def size_sg(self):
         return np.count_nonzero(self.representation)
 
     def append_or(self, to_append):
         super().append_or(to_append)
-        self.representation = np.logical_or(self.representation, to_append.representation)
+        self.representation = np.logical_or(
+            self.representation, to_append.representation
+        )
 
     @property
     def __array_interface__(self):
         return self.representation.__array_interface__
 
 
-
-
 class BitSetRepresentation(RepresentationBase):
     Conjunction = BitSet_Conjunction
     Disjunction = BitSet_Disjunction
+
     def __init__(self, df, selectors_to_patch):
         self.df = df
         super().__init__(BitSet_Conjunction, selectors_to_patch)
 
     def patch_selector(self, sel):
         sel.representation = sel.covers(self.df)
         sel.size_sg = np.count_nonzero(sel.representation)
 
     def patch_classes(self):
         BitSet_Conjunction.n_instances = len(self.df)
         super().patch_classes()
 
 
-class Set_Conjunction(ps.Conjunction):
+class Set_Conjunction(Conjunction):
     all_set = set()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.representation = self.compute_representation()
         self.arr_for_interface = np.array(list(self.representation), dtype=int)
 
     def compute_representation(self):
-                # empty description ==> return a list of all '1's
+        # empty description ==> return a list of all '1's
         if not self._selectors:
             return Set_Conjunction.all_set
         # non-empty description
         return set.intersection(*[sel.representation for sel in self._selectors])
 
     @property
     def size_sg(self):
         return len(self.representation)
 
-    #def __copy__(self):
-    #    tmp = super().__copy__()
-    #    tmp.representation = self.representation.copy()
-    #    return tmp
-
     def append_and(self, to_append):
         super().append_and(to_append)
         self.representation = self.representation.intersection(to_append.representation)
         self.arr_for_interface = np.array(list(self.representation), dtype=int)
 
     @property
     def __array_interface__(self):
-        return self.arr_for_interface.__array_interface__ # pylint: disable=no-member
+        return self.arr_for_interface.__array_interface__  # pylint: disable=no-member
 
 
 class SetRepresentation(RepresentationBase):
     Conjunction = Set_Conjunction
+
     def __init__(self, df, selectors_to_patch):
         self.df = df
         super().__init__(Set_Conjunction, selectors_to_patch)
 
     def patch_selector(self, sel):
         sel.representation = set(*np.nonzero(sel.covers(self.df)))
         sel.size_sg = len(sel.representation)
 
     def patch_classes(self):
         Set_Conjunction.all_set = set(self.df.index)
         super().patch_classes()
 
 
-class NumpySet_Conjunction(ps.Conjunction):
+class NumpySet_Conjunction(Conjunction):
     all_set = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.representation = self.compute_representation()
 
     def compute_representation(self):
-                # empty description ==> return a list of all '1's
+        # empty description ==> return a list of all '1's
         if not self._selectors:
             return NumpySet_Conjunction.all_set
         start = self._selectors[0].representation
         for sel in self._selectors[1:]:
             start = np.intersect1d(start, sel.representation, assume_unique=True)
         return start
 
     @property
     def size_sg(self):
         return len(self.representation)
 
-    #def __copy__(self):
-    #    tmp = super().__copy__()
-    #    tmp.representation = self.representation.copy()
-    #    return tmp
-
     def append_and(self, to_append):
         super().append_and(to_append)
-        #self._selectors.append(to_append)
-        self.representation = np.intersect1d(self.representation, to_append.representation, True)
+        # self._selectors.append(to_append)
+        self.representation = np.intersect1d(
+            self.representation, to_append.representation, True
+        )
 
     @property
     def __array_interface__(self):
         return self.representation.__array_interface__
 
 
 class NumpySetRepresentation(RepresentationBase):
     Conjunction = NumpySet_Conjunction
+
     def __init__(self, df, selectors_to_patch):
         self.df = df
         super().__init__(NumpySet_Conjunction, selectors_to_patch)
 
     def patch_selector(self, sel):
         sel.representation = np.nonzero(sel.covers(self.df))[0]
         sel.size_sg = len(sel.representation)
```

### Comparing `pysubgroup-0.7.3/pysubgroup/subgroup_description.py` & `pysubgroup-0.7.6/src/pysubgroup/subgroup_description.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,159 +1,178 @@
-'''
+"""
 Created on 28.04.2016
 
 @author: lemmerfn
-'''
-from abc import ABC, abstractmethod
+"""
+import copy
 import weakref
+from abc import ABC, abstractmethod
 from functools import total_ordering
-import pandas as pd
-import pysubgroup as ps
 from itertools import chain
-import copy
+
 import numpy as np
 
+import pysubgroup as ps
+
 
 @total_ordering
 class SelectorBase(ABC):
-
     # selector cache
     __refs__ = weakref.WeakSet()
 
     def __new__(cls, *args, **kwargs):
         """Ensures that each selector only exists once."""
 
         # create temporary selector
         tmp = super().__new__(cls)
         tmp.set_descriptions(*args, **kwargs)
 
         # save original arguments
-        # NOTE: this is a fix for pickle; so we can call `__getnewargs_ex__` with the right arguments
-        # TODO: this may have unintended side effects if args, kwargs are large or volatile (I don't think we have that yet though)
+        # NOTE: this is a fix for pickle
+        #       so we can call `__getnewargs_ex__` with the right arguments
+        # TODO: this may have unintended side effects if args,
+        #       kwargs are large or volatile (I don't think we have that yet though)
         tmp.__new_args__ = args, kwargs
 
         # check if selector is already in cache (__refs__)
         # if so, return cached instance
         if tmp in SelectorBase.__refs__:
-            for ref in SelectorBase. __refs__:
+            for ref in SelectorBase.__refs__:
                 if ref == tmp:
                     return ref
         # if not return
         return tmp
 
-    def __getnewargs_ex__(self):
-        return self.__new_args__
+    def __getnewargs_ex__(self):  # pylint: disable=invalid-getnewargs-ex-returned
+        tmp_args = self.__new_args__
+        del self.__new_args__
+        return tmp_args
 
     def __init__(self):
         # add selector to cache
-        # TODO: why not do this in `__new__`, then it would be all together in one function?
+        # TODO: why not do this in `__new__`,
+        # then it would be all together in one function?
         SelectorBase.__refs__.add(self)
 
     def __eq__(self, other):
         if other is None:
             return False
         return repr(self) == repr(other)
 
     def __lt__(self, other):
         return repr(self) < repr(other)
 
     def __hash__(self):
-        return self._hash #pylint: disable=no-member
+        return self._hash  # pylint: disable=no-member
 
     @abstractmethod
     def set_descriptions(self, *args, **kwargs):
-        pass
+        pass  # pragma: no-cover
 
 
 def get_cover_array_and_size(subgroup, data_len=None, data=None):
     if hasattr(subgroup, "representation"):
         cover_arr = subgroup
         size = subgroup.size_sg
     elif isinstance(subgroup, slice):
         cover_arr = subgroup
         if data_len is None:
-            if isinstance(data, pd.DataFrame):
+            if type(data).__name__ == "DataFrame":
                 data_len = len(data)
             else:
-                raise ValueError("if you pass a slice, you need to pass either data_len or data")
+                raise ValueError(
+                    "if you pass a slice, you need to pass either data_len or data"
+                )
         # https://stackoverflow.com/questions/36188429/retrieve-length-of-slice-from-slice-object-in-python
         size = len(range(*subgroup.indices(data_len)))
-    elif hasattr(subgroup, '__array_interface__'):
+    elif hasattr(subgroup, "__array_interface__"):
         cover_arr = subgroup
-        type_char = subgroup.__array_interface__['typestr'][1]
-        if type_char == 'b': # boolean indexing is used
+        type_char = subgroup.__array_interface__["typestr"][1]
+        if type_char == "b":  # boolean indexing is used
             size = np.count_nonzero(cover_arr)
-        elif type_char == 'u' or type_char == 'i': # integer indexing
-            size = subgroup.__array_interface__['shape'][0]
+        elif type_char in ("u", "i"):  # integer indexing
+            size = subgroup.__array_interface__["shape"][0]
         else:
-            print(type_char)
-            raise NotImplementedError(f"Currently a typechar of {type_char} is not supported.")
+            raise NotImplementedError(
+                f"Currently a typechar of {type_char} is not supported."
+            )
     else:
-        assert isinstance(data, pd.DataFrame)
+        assert type(data).__name__ == "DataFrame"
         cover_arr = subgroup.covers(data)
         size = np.count_nonzero(cover_arr)
     return cover_arr, size
 
 
 def get_size(subgroup, data_len=None, data=None):
     if hasattr(subgroup, "representation"):
         size = subgroup.size_sg
     elif isinstance(subgroup, slice):
         if data_len is None:
-            if isinstance(data, pd.DataFrame):
+            if type(data).__name__ == "DataFrame":
                 data_len = len(data)
             else:
-                raise ValueError("if you pass a slice, you need to pass either data_len or data")
+                raise ValueError(
+                    "if you pass a slice, you need to pass either data_len or data"
+                )
         # https://stackoverflow.com/questions/36188429/retrieve-length-of-slice-from-slice-object-in-python
         size = len(range(*subgroup.indices(data_len)))
-    elif hasattr(subgroup, '__array_interface__'):
-        type_char = subgroup.__array_interface__['typestr'][1]
-        if type_char == 'b': # boolean indexing is used
+    elif hasattr(subgroup, "__array_interface__"):
+        type_char = subgroup.__array_interface__["typestr"][1]
+        if type_char == "b":  # boolean indexing is used
             size = np.count_nonzero(subgroup)
-        elif type_char == 'u' or type_char == 'i': # integer indexing
-            size = subgroup.__array_interface__['shape'][0]
+        elif type_char == "u" or type_char == "i":  # integer indexing
+            size = subgroup.__array_interface__["shape"][0]
         else:
-            print(type_char)
-            raise NotImplementedError(f"Currently a typechar of {type_char} is not supported.")
+            raise NotImplementedError(
+                f"Currently a typechar of {type_char} is not supported."
+            )
     else:
-        assert isinstance(data, pd.DataFrame)
+        assert type(data).__name__ == "DataFrame"
         size = np.count_nonzero(subgroup.covers(data))
     return size
 
 
 class EqualitySelector(SelectorBase):
     def __init__(self, attribute_name, attribute_value, selector_name=None):
         if attribute_name is None:
             raise TypeError()
         if attribute_value is None:
             raise TypeError()
-        
+
         # TODO: this is redundant due to `__new__` and `set_descriptions`
         self._attribute_name = attribute_name
         self._attribute_value = attribute_value
         self._selector_name = selector_name
-        self.set_descriptions(self._attribute_name, self._attribute_value, self._selector_name)
-        
+        self.set_descriptions(
+            self._attribute_name, self._attribute_value, self._selector_name
+        )
+
         super().__init__()
 
     @property
     def attribute_name(self):
         return self._attribute_name
 
     @property
     def attribute_value(self):
         return self._attribute_value
 
-    def set_descriptions(self, attribute_name, attribute_value, selector_name=None): # pylint: disable=arguments-differ
-        self._hash, self._query, self._string = EqualitySelector.compute_descriptions(attribute_name, attribute_value, selector_name=selector_name)
+    def set_descriptions(
+        self, attribute_name, attribute_value, selector_name=None
+    ):  # pylint: disable=arguments-differ
+        self._hash, self._query, self._string = EqualitySelector.compute_descriptions(
+            attribute_name, attribute_value, selector_name=selector_name
+        )
 
     @classmethod
     def compute_descriptions(cls, attribute_name, attribute_value, selector_name):
         if isinstance(attribute_value, (str, bytes)):
             query = str(attribute_name) + "==" + "'" + str(attribute_value) + "'"
+        elif attribute_value is None:
+            query = str(attribute_name) + " is None"
         elif np.isnan(attribute_value):
             query = attribute_name + ".isnull()"
         else:
             query = str(attribute_name) + "==" + str(attribute_value)
         if selector_name is not None:
             string_ = selector_name
         else:
@@ -161,34 +180,53 @@
         hash_value = hash(query)
         return (hash_value, query, string_)
 
     def __repr__(self):
         return self._query
 
     def covers(self, data):
+        import pandas as pd  # pylint: disable=import-outside-toplevel
+
         row = data[self.attribute_name].to_numpy()
         if pd.isnull(self.attribute_value):
             return pd.isnull(row)
         return row == self.attribute_value
 
     def __str__(self, open_brackets="", closing_brackets=""):
         return open_brackets + self._string + closing_brackets
 
     @property
     def selectors(self):
         return (self,)
 
+    @staticmethod
+    def from_str(s):
+        s = s.strip()
+        attribute_name, attribute_value = s.split("==")
+        if attribute_value[0] == "'" and attribute_value[-1] == "'":
+            if attribute_value.startswith("'b'") and attribute_value.endswith("''"):
+                attribute_value = str.encode(attribute_value[3:-2])
+            else:
+                attribute_value = attribute_value[1:-1]
+        try:
+            attribute_value = int(attribute_value)
+        except ValueError:
+            try:
+                attribute_value = float(attribute_value)
+            except ValueError:
+                pass
+        return ps.EqualitySelector(attribute_name, attribute_value)
+
 
 class NegatedSelector(SelectorBase):
     def __init__(self, selector):
-        
         # TODO: this is redundant due to `__new__` and `set_descriptions`
         self._selector = selector
         self.set_descriptions(selector)
-        
+
         super().__init__()
 
     def covers(self, data_instance):
         return np.logical_not(self._selector.covers(data_instance))
 
     def __repr__(self):
         return self._query
@@ -202,28 +240,28 @@
 
     @property
     def attribute_name(self):
         return self._selector.attribute_name
 
     @property
     def selectors(self):
-        return self._selector.selectors
+        return (self,)
 
 
 # Including the lower bound, excluding the upper_bound
 class IntervalSelector(SelectorBase):
     def __init__(self, attribute_name, lower_bound, upper_bound, selector_name=None):
-        
+        assert lower_bound < upper_bound
         # TODO: this is redundant due to `__new__` and `set_descriptions`
         self._attribute_name = attribute_name
         self._lower_bound = lower_bound
         self._upper_bound = upper_bound
         self.selector_name = selector_name
         self.set_descriptions(attribute_name, lower_bound, upper_bound, selector_name)
-        
+
         super().__init__()
 
     @property
     def attribute_name(self):
         return self._attribute_name
 
     @property
@@ -244,25 +282,35 @@
     def __hash__(self):
         return self._hash
 
     def __str__(self):
         return self._string
 
     @classmethod
-    def compute_descriptions(cls, attribute_name, lower_bound, upper_bound, selector_name=None):
+    def compute_descriptions(
+        cls, attribute_name, lower_bound, upper_bound, selector_name=None
+    ):
         if selector_name is None:
-            _string = cls.compute_string(attribute_name, lower_bound, upper_bound, rounding_digits=2)
+            _string = cls.compute_string(
+                attribute_name, lower_bound, upper_bound, rounding_digits=2
+            )
         else:
             _string = selector_name
-        _query = cls.compute_string(attribute_name, lower_bound, upper_bound, rounding_digits=None)
-        _hash = _query.__hash__()
+        _query = cls.compute_string(
+            attribute_name, lower_bound, upper_bound, rounding_digits=None
+        )
+        _hash = hash(_query)
         return (_hash, _query, _string)
 
-    def set_descriptions(self, attribute_name, lower_bound, upper_bound, selector_name=None):  # pylint: disable=arguments-differ
-        self._hash, self._query, self._string = IntervalSelector.compute_descriptions(attribute_name, lower_bound, upper_bound, selector_name=selector_name)
+    def set_descriptions(
+        self, attribute_name, lower_bound, upper_bound, selector_name=None
+    ):  # pylint: disable=arguments-differ
+        self._hash, self._query, self._string = IntervalSelector.compute_descriptions(
+            attribute_name, lower_bound, upper_bound, selector_name=selector_name
+        )
 
     @classmethod
     def compute_string(cls, attribute_name, lower_bound, upper_bound, rounding_digits):
         if rounding_digits is None:
             formatter = "{}"
         else:
             formatter = "{0:." + str(rounding_digits) + "f}"
@@ -270,23 +318,55 @@
         lb = lower_bound
         if ub % 1:
             ub = formatter.format(ub)
         if lb % 1:
             lb = formatter.format(lb)
 
         if lower_bound == float("-inf") and upper_bound == float("inf"):
-            repre = attribute_name + "= anything"
+            repre = attribute_name + " = anything"
         elif lower_bound == float("-inf"):
             repre = attribute_name + "<" + str(ub)
         elif upper_bound == float("inf"):
             repre = attribute_name + ">=" + str(lb)
         else:
             repre = attribute_name + ": [" + str(lb) + ":" + str(ub) + "["
         return repre
 
+    @staticmethod
+    def from_str(s):
+        s = s.strip()
+        if s.endswith(" = anything"):
+            return IntervalSelector(
+                s[: -len(" = anything")], float("-inf"), float("+inf")
+            )
+        if "<" in s:
+            attribute_name, ub = s.split("<")
+            try:
+                return IntervalSelector(attribute_name.strip(), float("-inf"), int(ub))
+            except ValueError:
+                return IntervalSelector(
+                    attribute_name.strip(), float("-inf"), float(ub)
+                )
+        if ">=" in s:
+            attribute_name, lb = s.split(">=")
+            try:
+                return IntervalSelector(attribute_name.strip(), int(lb), float("inf"))
+            except ValueError:
+                return IntervalSelector(attribute_name.strip(), float(lb), float("inf"))
+        if s.count(":") == 2:
+            attribute_name, lb, ub = s.split(":")
+            lb = lb.strip()[1:]
+            ub = ub.strip()[:-1]
+            try:
+                return IntervalSelector(attribute_name.strip(), int(lb), int(ub))
+            except ValueError:
+                return IntervalSelector(attribute_name.strip(), float(lb), float(ub))
+        else:
+            raise ValueError(f"string {s} could not be converted to IntervalSelector")
+
     @property
     def selectors(self):
         return (self,)
 
 
 def create_selectors(data, nbins=5, intervals_only=True, ignore=None):
     if ignore is None:
@@ -296,93 +376,113 @@
     return sels
 
 
 def create_nominal_selectors(data, ignore=None):
     if ignore is None:
         ignore = []
     nominal_selectors = []
-    # for attr_name in [x for x in data.select_dtypes(exclude=['number']).columns.values if x not in ignore]:
-    #    nominal_selectors.extend(create_nominal_selectors_for_attribute(data, attr_name))
-    nominal_dtypes = data.select_dtypes(exclude=['number'])
+    # for attr_name in [
+    #       x for x in data.select_dtypes(exclude=['number']).columns.values
+    #       if x not in ignore]:
+    #    nominal_selectors.extend(
+    #       create_nominal_selectors_for_attribute(data, attr_name))
+    nominal_dtypes = data.select_dtypes(exclude=["number"])
     dtypes = data.dtypes
     # print(dtypes)
     for attr_name in [x for x in nominal_dtypes.columns.values if x not in ignore]:
-        nominal_selectors.extend(create_nominal_selectors_for_attribute(data, attr_name, dtypes))
+        nominal_selectors.extend(
+            create_nominal_selectors_for_attribute(data, attr_name, dtypes)
+        )
     return nominal_selectors
 
 
 def create_nominal_selectors_for_attribute(data, attribute_name, dtypes=None):
+    import pandas as pd  # pylint: disable=import-outside-toplevel
+
     nominal_selectors = []
     for val in pd.unique(data[attribute_name]):
         nominal_selectors.append(EqualitySelector(attribute_name, val))
     # setting the is_bool flag for selector
     if dtypes is None:
         dtypes = data.dtypes
-    if dtypes[attribute_name] == 'bool':
+    if dtypes[attribute_name] == "bool":
         for s in nominal_selectors:
             s.is_bool = True
     return nominal_selectors
 
 
-def create_numeric_selectors(data, nbins=5, intervals_only=True, weighting_attribute=None, ignore=None):
+def create_numeric_selectors(
+    data, nbins=5, intervals_only=True, weighting_attribute=None, ignore=None
+):
     if ignore is None:
-        ignore = []
+        ignore = []  # pragma: no cover
     numeric_selectors = []
-    for attr_name in [x for x in data.select_dtypes(include=['number']).columns.values if x not in ignore]:
-        numeric_selectors.extend(create_numeric_selectors_for_attribute(
-            data, attr_name, nbins, intervals_only, weighting_attribute))
+    for attr_name in [
+        x
+        for x in data.select_dtypes(include=["number"]).columns.values
+        if x not in ignore
+    ]:
+        numeric_selectors.extend(
+            create_numeric_selectors_for_attribute(
+                data, attr_name, nbins, intervals_only, weighting_attribute
+            )
+        )
     return numeric_selectors
 
 
-def create_numeric_selectors_for_attribute(data, attr_name, nbins=5, intervals_only=True, weighting_attribute=None):
+def create_numeric_selectors_for_attribute(
+    data, attr_name, nbins=5, intervals_only=True, weighting_attribute=None
+):
     numeric_selectors = []
     data_not_null = data[data[attr_name].notnull()]
 
     uniqueValues = np.unique(data_not_null[attr_name])
     if len(data_not_null.index) < len(data.index):
         numeric_selectors.append(EqualitySelector(attr_name, np.nan))
 
     if len(uniqueValues) <= nbins:
         for val in uniqueValues:
             numeric_selectors.append(EqualitySelector(attr_name, val))
     else:
-        cutpoints = ps.equal_frequency_discretization(data, attr_name, nbins, weighting_attribute)
+        cutpoints = ps.equal_frequency_discretization(
+            data, attr_name, nbins, weighting_attribute
+        )
         if intervals_only:
             old_cutpoint = float("-inf")
             for c in cutpoints:
                 numeric_selectors.append(IntervalSelector(attr_name, old_cutpoint, c))
                 old_cutpoint = c
-            numeric_selectors.append(IntervalSelector(attr_name, old_cutpoint, float("inf")))
+            numeric_selectors.append(
+                IntervalSelector(attr_name, old_cutpoint, float("inf"))
+            )
         else:
             for c in cutpoints:
                 numeric_selectors.append(IntervalSelector(attr_name, c, float("inf")))
                 numeric_selectors.append(IntervalSelector(attr_name, float("-inf"), c))
 
     return numeric_selectors
 
 
 def remove_target_attributes(selectors, target):
-    result = []
-    for sel in selectors:
-        if not sel.get_attribute_name() in target.get_attributes():
-            result.append(sel)
-    return result
+    return [
+        sel for sel in selectors if sel.attribute_name not in target.get_attributes()
+    ]
 
 
 ##############
 # Boolean expressions
 ##############
 class BooleanExpressionBase(ABC):
     def __or__(self, other):
         tmp = copy.copy(self)
         tmp.append_or(other)
         return tmp
 
     def __and__(self, other):
-        tmp = self.__copy__()
+        tmp = copy.copy(self)
         tmp.append_and(other)
         return tmp
 
     @abstractmethod
     def append_and(self, to_append):
         pass
 
@@ -390,17 +490,20 @@
     def append_or(self, to_append):
         pass
 
     @abstractmethod
     def __copy__(self):
         pass
 
+
 @total_ordering
 class Conjunction(BooleanExpressionBase):
     def __init__(self, selectors):
+        self._repr = None
+        self._hash = None
         try:
             it = iter(selectors)
             self._selectors = list(it)
         except TypeError:
             self._selectors = [selectors]
 
     def covers(self, instance):
@@ -416,72 +519,67 @@
     def __str__(self, open_brackets="", closing_brackets="", and_term=" AND "):
         if not self._selectors:
             return "Dataset"
         attrs = sorted(str(sel) for sel in self._selectors)
         return "".join((open_brackets, and_term.join(attrs), closing_brackets))
 
     def __repr__(self):
-        if hasattr(self, "_repr"):
+        if self._repr is not None:
             return self._repr
         else:
             self._repr = self._compute_repr()
             return self._repr
 
     def __eq__(self, other):
         return repr(self) == repr(other)
 
     def __lt__(self, other):
         return repr(self) < repr(other)
 
     def __hash__(self):
-        if hasattr(self, "_hash"):
+        if self._hash is not None:
             return self._hash
         else:
             self._hash = self._compute_hash()
             return self._hash
 
-    def _compute_representations(self):
-        self._repr = self._compute_repr()
-        self._hash = self._compute_hash()
-
     def _compute_repr(self):
         if not self._selectors:
             return "True"
         reprs = sorted(repr(sel) for sel in self._selectors)
         return "".join(("(", " and ".join(reprs), ")"))
 
     def _compute_hash(self):
         return hash(repr(self))
 
     def _invalidate_representations(self):
-        if hasattr(self, '_repr'):
-            delattr(self, '_repr')
-        if hasattr(self, '_hash'):
-            delattr(self, '_hash')
+        self._repr = None
+        self._hash = None
 
     def append_and(self, to_append):
         if isinstance(to_append, SelectorBase):
             self._selectors.append(to_append)
         elif isinstance(to_append, Conjunction):
             self._selectors.extend(to_append.selectors)
         else:
-            try:
-                self._selectors.extend(to_append)
-            except TypeError:
-                self._selectors.append(to_append)
+            self._selectors.extend(to_append)
         self._invalidate_representations()
 
     def append_or(self, to_append):
-        raise RuntimeError("Or operations are not supported by a pure Conjunction. Consider using DNF.")
+        raise RuntimeError(
+            "Or operations are not supported by a pure Conjunction. Consider using DNF."
+        )
 
     def pop_and(self):
         return self._selectors.pop()
 
     def pop_or(self):
-        raise RuntimeError("Or operations are not supported by a pure Conjunction. Consider using DNF.")
+        raise RuntimeError(
+            "Or operations are not supported by a pure Conjunction. Consider using DNF."
+        )
 
     def __copy__(self):
         cls = self.__class__
         result = cls.__new__(cls)
         result.__dict__.update(self.__dict__)
         result._selectors = list(self._selectors)
         return result
@@ -490,20 +588,36 @@
     def depth(self):
         return len(self._selectors)
 
     @property
     def selectors(self):
         return tuple(chain.from_iterable(sel.selectors for sel in self._selectors))
 
+    @staticmethod
+    def from_str(s):
+        if s.strip() == "Dataset":
+            return Conjunction([])
+        selector_strings = s.split(" AND ")
+        selectors = []
+        for selector_string in selector_strings:
+            selector_string = selector_string.strip()
+            if "==" in selector_string:
+                selectors.append(EqualitySelector.from_str(selector_string))
+            else:
+                selectors.append(IntervalSelector.from_str(selector_string))
+        return Conjunction(selectors)
+
 
 @total_ordering
 class Disjunction(BooleanExpressionBase):
-    def __init__(self, selectors):
+    def __init__(self, selectors=None):
         if isinstance(selectors, (list, tuple)):
             self._selectors = selectors
+        elif selectors is None:
+            self._selectors = []
         else:
             self._selectors = [selectors]
 
     def covers(self, instance):
         # empty description ==> return a list of all '1's
         if not self._selectors:
             return np.full(len(instance), False, dtype=bool)
@@ -511,15 +625,15 @@
         return np.any([sel.covers(instance) for sel in self._selectors], axis=0)
 
     def __len__(self):
         return len(self._selectors)
 
     def __str__(self, open_brackets="", closing_brackets="", or_term=" OR "):
         if not self._selectors:
-            return "Dataset"
+            return "Empty"  # pragma: no cover
         attrs = sorted(str(sel) for sel in self._selectors)
         return "".join((open_brackets, or_term.join(attrs), closing_brackets))
 
     def __repr__(self):
         if not self._selectors:
             return "True"
         reprs = sorted(repr(sel) for sel in self._selectors)
@@ -531,17 +645,23 @@
     def __lt__(self, other):
         return repr(self) < repr(other)
 
     def __hash__(self):
         return hash(repr(self))
 
     def append_and(self, to_append):
-        raise RuntimeError("And operations are not supported by a pure Conjunction. Consider using DNF.")
+        raise RuntimeError(
+            "And operations are not supported by a pure Conjunction. "
+            "Consider using DNF."
+        )
 
     def append_or(self, to_append):
+        if isinstance(to_append, Disjunction):
+            self._selectors.extend(to_append.selectors)
+            return
         try:
             self._selectors.extend(to_append)
         except TypeError:
             self._selectors.append(to_append)
 
     def __copy__(self):
         cls = self.__class__
@@ -569,32 +689,43 @@
         elif isinstance(to_append, SelectorBase):
             return Conjunction(to_append)
         else:
             it = iter(to_append)
             if all(isinstance(sel, SelectorBase) for sel in to_append):
                 return Conjunction(it)
             else:
-                raise ValueError("DNFs only accept an iterable of pure Selectors")
+                raise ValueError(
+                    "DNFs only accept an iterable of Selectors"
+                )  # pragma: no cover
 
     def append_or(self, to_append):
+        if isinstance(to_append, ps.Disjunction):
+            to_append = to_append.selectors
         try:
             it = iter(to_append)
             conjunctions = [DNF._ensure_pure_conjunction(part) for part in it]
         except TypeError:
             conjunctions = DNF._ensure_pure_conjunction(to_append)
         super().append_or(conjunctions)
 
     def append_and(self, to_append):
+        if isinstance(to_append, Disjunction):
+            raise NotImplementedError(
+                "Appeding a disjunction to DNF is not implemented"
+            )
         conj = DNF._ensure_pure_conjunction(to_append)
         if len(self._selectors) > 0:
             for conjunction in self._selectors:
                 conjunction.append_and(conj)
         else:
             self._selectors.append(conj)
 
     def pop_and(self):
         out_list = [s.pop_and() for s in self._selectors]
         return_val = out_list[0]
         if all(x == return_val for x in out_list):
             return return_val
         else:
+            for to_append, conj in zip(out_list, self._selectors):
+                conj.append_and(to_append)
+
             raise RuntimeError("pop_and failed as the result was inconsistent")
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/algorithms_testing.py` & `pysubgroup-0.7.6/tests/algorithms_testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-from timeit import default_timer as timer
 import abc
+from timeit import default_timer as timer
+
 import pysubgroup as ps
 
-class TestAlgorithmsBase(abc.ABC):
 
+class TestAlgorithmsBase(abc.ABC):
     # pylint: disable=no-member
     def evaluate_result(self, algorithm_result, result, qualities):
         self.assertTrue(isinstance(algorithm_result, ps.SubgroupDiscoveryResult))
         algorithm_result.to_dataframe()
         algorithm_result = algorithm_result.to_descriptions()
-        for (q, sg) in algorithm_result:
+        for q, sg in algorithm_result:
             print("   " + str(q) + ":\t" + str(sg))
         # compare length such that zip works correctly
         self.assertEqual(len(algorithm_result), len(result))
         self.assertEqual(len(algorithm_result), len(qualities))
 
-        for (algorithm_q, algorithm_SG), expected_q, expected_SGD in zip(algorithm_result, qualities, result):
+        for (algorithm_q, algorithm_SG), expected_q, expected_SGD in zip(
+            algorithm_result, qualities, result
+        ):
             self.assertEqual(repr(algorithm_SG), repr(expected_SGD))
             self.assertEqual(algorithm_q, expected_q)
 
-
     def runAlgorithm(self, algorithm, name, result, qualities, task):
         print()
         print("Running " + name)
         start = timer()
         algorithm_result = algorithm.execute(task)
         end = timer()
         print("   Runtime for {}: {}".format(name, end - start))
 
-        if hasattr(self.task.qf, 'calls'):
-            print('   Number of call to qf:', self.task.qf.calls)
+        if hasattr(self.task.qf, "calls"):
+            print("   Number of call to qf:", self.task.qf.calls)
         print()
         self.evaluate_result(algorithm_result, result, qualities)
         return algorithm_result
+
     # pylint: enable=no-member
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/t_numeric_targets2.py` & `pysubgroup-0.7.6/tests/t_numeric_targets2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import pprint
+
 import numpy as np
 import pandas as pd
-import pysubgroup as ps
 
+import pysubgroup as ps
 
 pp = pprint.PrettyPrinter(indent=4)
 
 data = np.array([[1, 2, 3, 4, 5], ["F", "F", "F", "Tr", "Tr"]]).T
 data = pd.DataFrame(data, columns=["Target", "A"])
 data["Target"] = pd.to_numeric(data["Target"])
 
 
-target = ps.NumericTarget('Target')
+target = ps.NumericTarget("Target")
 print(data[target.target_variable])
 sgd = ps.EqualitySelector("A", "Tr")
 target.calculate_statistics(sgd, data)
 
 qf = ps.StandardQFNumeric(1.0)
 print(qf.evaluate(sgd, target, data))
 print(qf.optimistic_estimate(sgd, target, data))
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_ChiSquaredQF.py` & `pysubgroup-0.7.6/tests/test_ChiSquaredQF.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from timeit import default_timer as timer
+
 import pysubgroup as ps
-from pysubgroup.tests.DataSets import get_credit_data
+from pysubgroup.datasets import get_credit_data
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     data = get_credit_data()
 
-    target = ps.BinaryTarget('class', b'bad')
-    searchSpace = ps.create_nominal_selectors(data, ignore=['class'])
-    task = ps.SubgroupDiscoveryTask(data, target, searchSpace, result_set_size=10, depth=4, qf=ps.ChiSquaredQF())
+    target = ps.BinaryTarget("class", b"bad")
+    searchSpace = ps.create_nominal_selectors(data, ignore=["class"])
+    task = ps.SubgroupDiscoveryTask(
+        data, target, searchSpace, result_set_size=10, depth=4, qf=ps.ChiSquaredQF()
+    )
 
     print("running DFS")
     start = timer()
     result = ps.SimpleDFS().execute(task)
     end = timer()
     print("Time elapsed: ", (end - start))
-    for (q, sg) in result:
+    for q, sg in result:
         print(str(q) + ":\t" + str(sg.subgroup_description))
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_SubgroupDiscoveryResult.py` & `pysubgroup-0.7.6/tests/test_SubgroupDiscoveryResult.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,87 @@
 import unittest
-import matplotlib.pyplot as plt
+
+from algorithms_testing import TestAlgorithmsBase
 
 import pysubgroup as ps
-from pysubgroup.tests.DataSets import get_credit_data
-from pysubgroup.tests.algorithms_testing import TestAlgorithmsBase
+from pysubgroup.datasets import get_credit_data
 
 show_plots = False
+
+
 class TestNominalTarget_to_result(unittest.TestCase, TestAlgorithmsBase):
     @classmethod
     def setUpClass(cls):
         data = get_credit_data()
-        target = ps.BinaryTarget('class', b'bad')
-        searchSpace = ps.create_nominal_selectors(data, ignore=['class'])
-        cls.task = ps.SubgroupDiscoveryTask(data, target, searchSpace, result_set_size=10, depth=5, qf=ps.StandardQF(1.0))
+        target = ps.BinaryTarget("class", b"bad")
+        searchSpace = ps.create_nominal_selectors(data, ignore=["class"])
+        cls.task = ps.SubgroupDiscoveryTask(
+            data,
+            target,
+            searchSpace,
+            result_set_size=10,
+            depth=5,
+            qf=ps.StandardQF(1.0),
+        )
         cls.result = ps.SimpleDFS().execute(cls.task)
 
     def test_to_dataframe(self):
         df = self.__class__.result.to_dataframe()
         self.assertEqual(len(df), 10)
         self.assertEqual(len(df.columns), 15)
 
     def test_to_descriptions(self):
-        l = self.__class__.result.to_descriptions()
-        self.assertEqual(len(l), 10)
-        for tpl in l:
+        descriptions = self.__class__.result.to_descriptions()
+        self.assertEqual(len(descriptions), 10)
+        for tpl in descriptions:
             self.assertEqual(len(tpl), 2)
             self.assertTrue(isinstance(tpl[0], float))
             self.assertTrue(isinstance(tpl[1], ps.Conjunction))
 
-    #def test_supportSetVisualization(self):
+    # def test_supportSetVisualization(self):
     #    img = self.__class__.result.supportSetVisualization()
     #    self.assertEqual(img.shape, (10, 274))
     #    if show_plots:
     #        plt.matshow(img)
     #        plt.show()
 
+
 class TestNumericTarget_to_result(unittest.TestCase, TestAlgorithmsBase):
     @classmethod
     def setUpClass(cls):
         data = get_credit_data()
-        target = ps.NumericTarget('credit_amount')
-        searchSpace = ps.create_nominal_selectors(data, ignore=['credit_amount'])
-        cls.task = ps.SubgroupDiscoveryTask(data, target, searchSpace, result_set_size=10, depth=3, qf=ps.StandardQFNumeric(1.0))
+        target = ps.NumericTarget("credit_amount")
+        searchSpace = ps.create_nominal_selectors(data, ignore=["credit_amount"])
+        cls.task = ps.SubgroupDiscoveryTask(
+            data,
+            target,
+            searchSpace,
+            result_set_size=10,
+            depth=3,
+            qf=ps.StandardQFNumeric(1.0),
+        )
         cls.result = ps.SimpleDFS().execute(cls.task)
 
     def test_to_dataframe(self):
         df = self.__class__.result.to_dataframe()
         self.assertEqual(len(df), 10)
         self.assertEqual(len(df.columns), 16)
 
     def test_to_descriptions(self):
-        l = self.__class__.result.to_descriptions()
-        self.assertEqual(len(l), 10)
-        for tpl in l:
+        descriptions = self.__class__.result.to_descriptions()
+        self.assertEqual(len(descriptions), 10)
+        for tpl in descriptions:
             self.assertEqual(len(tpl), 2)
             self.assertTrue(isinstance(tpl[0], float))
             self.assertTrue(isinstance(tpl[1], ps.Conjunction))
 
-
-    #def test_supportSetVisualization(self):
+    # def test_supportSetVisualization(self):
     #    img = self.__class__.result.supportSetVisualization()
     #    self.assertEqual(img.shape, (10, 425))
     #    if show_plots:
     #        plt.matshow(img)
     #        plt.show()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     show_plots = False
     unittest.main()
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_algorithms_boolean.py` & `pysubgroup-0.7.6/tests/test_algorithms_boolean.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,218 +1,354 @@
+# flake8: noqa: E501
+
 import unittest
+
 import pytest
+from algorithms_testing import TestAlgorithmsBase
+
 import pysubgroup as ps
-from pysubgroup.tests.DataSets import get_credit_data
+from pysubgroup.datasets import get_credit_data
 
-from pysubgroup.tests.algorithms_testing import TestAlgorithmsBase
 
 class TestSettings:
     All = True
     Apriori = False
     SimpleDFS = False
     BestFirstSearch = False
     BeamSearch = False
     DFS_bitset = False
     DFS_set = False
     DFS_numpyset = False
     SimpleSearch = False
+    GpGrowth = False
+
 
 skip_long_running = True
-class BooleanTargetBase():
 
+
+class BooleanTargetBase:
     # pylint: disable=no-member
-    @unittest.skipUnless(TestSettings.All or TestSettings.Apriori, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.Apriori, "flag not set")
     def test_Apriori(self):
-        self.runAlgorithm(ps.Apriori(), "Apriori", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.Apriori(), "Apriori", self.result, self.qualities, self.task
+        )
+
+    @unittest.skipUnless(TestSettings.All or TestSettings.Apriori, "flag not set")
+    def test_Apriori_no_numba(self):
+        self.runAlgorithm(
+            ps.Apriori(use_numba=False),
+            "Apriori",
+            self.result,
+            self.qualities,
+            self.task,
+        )
+
+    @unittest.skipUnless(TestSettings.All or TestSettings.Apriori, "flag not set")
+    def test_Apriori_no_vector(self):
+        alg = ps.Apriori()
+        alg.use_vectorization = False
+        self.runAlgorithm(alg, "Apriori", self.result, self.qualities, self.task)
 
-    @unittest.skipUnless(TestSettings.All or TestSettings.SimpleDFS, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.SimpleDFS, "flag not set")
     def test_SimpleDFS(self):
-        self.runAlgorithm(ps.SimpleDFS(), "SimpleDFS", self.result, self.qualities, self.task)
-
-    @unittest.skipUnless(TestSettings.All or TestSettings.BestFirstSearch, 'flag not set')
+        self.runAlgorithm(
+            ps.SimpleDFS(), "SimpleDFS", self.result, self.qualities, self.task
+        )
+
+    @unittest.skipUnless(
+        TestSettings.All or TestSettings.BestFirstSearch, "flag not set"
+    )
     def test_BestFirstSearch(self):
-        self.runAlgorithm(ps.BestFirstSearch(), "BestFirstSearch", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.BestFirstSearch(),
+            "BestFirstSearch",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
-    @unittest.skipUnless(TestSettings.All or TestSettings.BeamSearch, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.BeamSearch, "flag not set")
     def test_BeamSearch(self):
-        self.runAlgorithm(ps.BeamSearch(beam_width=12), "BeamSearch", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.BeamSearch(beam_width=12),
+            "BeamSearch",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
-    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_bitset, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_bitset, "flag not set")
     def test_DFS_bitset(self):
-        self.runAlgorithm(ps.DFS(ps.BitSetRepresentation), "DFS bitset", self.result, self.qualities, self.task)
-
-
-
+        self.runAlgorithm(
+            ps.DFS(ps.BitSetRepresentation),
+            "DFS bitset",
+            self.result,
+            self.qualities,
+            self.task,
+        )
+
+    @unittest.skipUnless(TestSettings.All or TestSettings.GpGrowth, "flag not set")
+    def test_gp_growth(self):
+        self.task.constraints_monotone.append(
+            ps.MinSupportConstraint(100)
+        )  # constraint added to speed up tests
+        self.runAlgorithm(
+            ps.GpGrowth(), "GpGrowth", self.result, self.qualities, self.task
+        )
+        self.task.constraints_monotone.pop(-1)
+
+    @unittest.skipUnless(TestSettings.All or TestSettings.GpGrowth, "flag not set")
+    def test_gp_growth_long(self):
+        self.runAlgorithm(
+            ps.GpGrowth(), "GpGrowth", self.result, self.qualities, self.task
+        )
+
+    @unittest.skipUnless(TestSettings.All or TestSettings.GpGrowth, "flag not set")
+    def test_gp_growth_top_down(self):
+        self.task.constraints_monotone.append(ps.MinSupportConstraint(100))
+        self.runAlgorithm(
+            ps.GpGrowth(mode="t_d"), "GpGrowth", self.result, self.qualities, self.task
+        )
+        self.task.constraints_monotone.pop(-1)
 
     @pytest.mark.slow
-    @unittest.skipUnless(TestSettings.All or TestSettings.SimpleSearch, 'flag not set')
-    def test_SimpleSearch(self):
-        self.runAlgorithm(ps.SimpleSearch(), "SimpleSearch", self.result, self.qualities, self.task)
+    @unittest.skipUnless(TestSettings.SimpleSearch, "flag not set")
+    def test_SimpleSearch_slow(self):
+        self.runAlgorithm(
+            ps.SimpleSearch(), "SimpleSearch", self.result, self.qualities, self.task
+        )
 
-    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_set, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_set, "flag not set")
     def test_DFS_set(self):
-        self.runAlgorithm(ps.DFS(ps.SetRepresentation), "DFS set", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.DFS(ps.SetRepresentation),
+            "DFS set",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
-    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_numpyset, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_numpyset, "flag not set")
     def test_DFS_numpy_sets(self):
-        self.runAlgorithm(ps.DFS(ps.NumpySetRepresentation), "DFS numpyset", self.result, self.qualities, self.task)
-    # pylint: enable=no-member
+        self.runAlgorithm(
+            ps.DFS(ps.NumpySetRepresentation),
+            "DFS numpyset",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
+    # pylint: enable=no-member
 
 
 class TestAlgorithms(TestAlgorithmsBase, BooleanTargetBase, unittest.TestCase):
     def setUp(self):
         NS_checking = ps.EqualitySelector("checking_status", b"<0")
         NS_foreign_worker = ps.EqualitySelector("foreign_worker", b"yes")
         NS_other_parties = ps.EqualitySelector("other_parties", b"none")
         NS_savings_status = ps.EqualitySelector("savings_status", b"<100")
         NS_job = ps.EqualitySelector("job", b"skilled")
-        self.result = [ps.Conjunction([NS_checking, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking]),
-                       ps.Conjunction([NS_checking, NS_other_parties, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_other_parties]),
-                       ps.Conjunction([NS_checking, NS_savings_status, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_savings_status]),
-                       ps.Conjunction([NS_checking, NS_savings_status, NS_other_parties, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_job, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_savings_status, NS_other_parties]),
-                       ps.Conjunction([NS_checking, NS_job]),
-                       ]
-        self.qualities = [0.055299999999999995,
-                          0.05280000000000001,
-                          0.052300000000000006,
-                          0.05059999999999999,
-                          0.04959999999999999,
-                          0.048299999999999996,
-                          0.04660000000000001,
-                          0.04550000000000001,
-                          0.0452,
-                          0.044399999999999995]
+        self.result = [
+            ps.Conjunction([NS_checking, NS_foreign_worker]),
+            ps.Conjunction([NS_checking]),
+            ps.Conjunction([NS_checking, NS_other_parties, NS_foreign_worker]),
+            ps.Conjunction([NS_checking, NS_other_parties]),
+            ps.Conjunction([NS_checking, NS_savings_status, NS_foreign_worker]),
+            ps.Conjunction([NS_checking, NS_savings_status]),
+            ps.Conjunction(
+                [NS_checking, NS_savings_status, NS_other_parties, NS_foreign_worker]
+            ),
+            ps.Conjunction([NS_checking, NS_job, NS_foreign_worker]),
+            ps.Conjunction([NS_checking, NS_savings_status, NS_other_parties]),
+            ps.Conjunction([NS_checking, NS_job]),
+        ]
+        self.qualities = [
+            0.055299999999999995,
+            0.05280000000000001,
+            0.052300000000000006,
+            0.05059999999999999,
+            0.04959999999999999,
+            0.048299999999999996,
+            0.04660000000000001,
+            0.04550000000000001,
+            0.0452,
+            0.044399999999999995,
+        ]
         data = get_credit_data()
-        target = ps.BinaryTarget('class', b'bad')
-        searchSpace = ps.create_nominal_selectors(data, ignore=['class'])
-        self.task = ps.SubgroupDiscoveryTask(data, target, searchSpace, result_set_size=10, depth=5, qf=ps.StandardQF(1.0))
+        target = ps.BinaryTarget("class", b"bad")
+        searchSpace = ps.create_nominal_selectors(data, ignore=["class"])
+        self.task = ps.SubgroupDiscoveryTask(
+            data,
+            target,
+            searchSpace,
+            result_set_size=10,
+            depth=5,
+            qf=ps.StandardQF(1.0),
+        )
+
 
 # also includes numeric attributes and has 12 targets
 
 
 class TestAlgorithms2(TestAlgorithmsBase, BooleanTargetBase, unittest.TestCase):
     def setUp(self):
         NS_checking = ps.EqualitySelector("checking_status", b"<0")
         NS_foreign_worker = ps.EqualitySelector("foreign_worker", b"yes")
         NS_other_parties = ps.EqualitySelector("other_parties", b"none")
         NS_savings_status = ps.EqualitySelector("savings_status", b"<100")
         NS_job = ps.EqualitySelector("job", b"skilled")
         NS_dependents = ps.EqualitySelector("num_dependents", 1.0)
-        self.result = [ps.Conjunction([NS_checking, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking]),
-                       ps.Conjunction([NS_checking, NS_other_parties, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_other_parties]),
-                       ps.Conjunction([NS_checking, NS_savings_status, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_foreign_worker, NS_dependents]),
-                       ps.Conjunction([NS_checking, NS_savings_status]),
-                       ps.Conjunction([NS_checking, NS_dependents]),
-                       ps.Conjunction([NS_checking, NS_savings_status, NS_other_parties, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_job, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_savings_status, NS_other_parties]),
-                       ps.Conjunction([NS_checking, NS_job]),
-                       ]
-        self.qualities = [0.055299999999999995,
-                          0.05280000000000001,
-                          0.052300000000000006,
-                          0.05059999999999999,
-                          0.04959999999999999,
-                          0.04870000000000001,
-                          0.048299999999999996,
-                          0.0474,
-                          0.04660000000000001,
-                          0.04550000000000001,
-                          0.0452,
-                          0.044399999999999995
-                          ]
+        self.result = [
+            ps.Conjunction([NS_checking, NS_foreign_worker]),
+            ps.Conjunction([NS_checking]),
+            ps.Conjunction([NS_checking, NS_other_parties, NS_foreign_worker]),
+            ps.Conjunction([NS_checking, NS_other_parties]),
+            ps.Conjunction([NS_checking, NS_savings_status, NS_foreign_worker]),
+            ps.Conjunction([NS_checking, NS_foreign_worker, NS_dependents]),
+            ps.Conjunction([NS_checking, NS_savings_status]),
+            ps.Conjunction([NS_checking, NS_dependents]),
+            ps.Conjunction(
+                [NS_checking, NS_savings_status, NS_other_parties, NS_foreign_worker]
+            ),
+            ps.Conjunction([NS_checking, NS_job, NS_foreign_worker]),
+            ps.Conjunction([NS_checking, NS_savings_status, NS_other_parties]),
+            ps.Conjunction([NS_checking, NS_job]),
+        ]
+        self.qualities = [
+            0.055299999999999995,
+            0.05280000000000001,
+            0.052300000000000006,
+            0.05059999999999999,
+            0.04959999999999999,
+            0.04870000000000001,
+            0.048299999999999996,
+            0.0474,
+            0.04660000000000001,
+            0.04550000000000001,
+            0.0452,
+            0.044399999999999995,
+        ]
         data = get_credit_data()
-        target = ps.BinaryTarget('class', b'bad')
-        searchSpace_Nominal = ps.create_nominal_selectors(data, ignore=['class'])
-        searchSpace_Numeric = ps.create_numeric_selectors(data, ignore=['class'])
+        target = ps.BinaryTarget("class", b"bad")
+        searchSpace_Nominal = ps.create_nominal_selectors(data, ignore=["class"])
+        searchSpace_Numeric = ps.create_numeric_selectors(data, ignore=["class"])
         searchSpace = searchSpace_Nominal + searchSpace_Numeric
-        self.task = ps.SubgroupDiscoveryTask(data, target, searchSpace, result_set_size=12, depth=5, qf=ps.StandardQF(1.0))
+        self.task = ps.SubgroupDiscoveryTask(
+            data,
+            target,
+            searchSpace,
+            result_set_size=12,
+            depth=5,
+            qf=ps.StandardQF(1.0),
+        )
 
-    @pytest.mark.slow
     def test_DFS_numpy_sets(self):
-        super.test_DFS_numpy_sets()
+        super().test_DFS_numpy_sets()
+
 
 # uses an a=0.5 and result_set_size = 12, is much faster because of that
 
 
 class TestAlgorithms3(TestAlgorithmsBase, BooleanTargetBase, unittest.TestCase):
     def setUp(self):
         NS_checking = ps.EqualitySelector("checking_status", b"<0")
         NS_foreign_worker = ps.EqualitySelector("foreign_worker", b"yes")
         NS_other_parties = ps.EqualitySelector("other_parties", b"none")
         NS_savings_status = ps.EqualitySelector("savings_status", b"<100")
         NS_job = ps.EqualitySelector("job", b"skilled")
         NS_dependents = ps.EqualitySelector("num_dependents", 1.0)
-        self.result = [ps.Conjunction([NS_checking, NS_foreign_worker, NS_job, NS_other_parties, NS_savings_status]),  # AND job=='b'skilled'' AND other_parties=='b'none'' AND savings_status=='b'<100'
-                       # 0.113713540226172:    checking_status=='b'<0'' AND foreign_worker=='b'yes'' AND job=='b'skilled'' AND savings_status=='b'<100''
-                       ps.Conjunction([NS_checking, NS_foreign_worker, NS_job, NS_savings_status]),
-                       ps.Conjunction([NS_checking, NS_foreign_worker, NS_job]),  # checking_status=='b'<0'' AND foreign_worker=='b'yes'' AND job=='b'skilled''
-                       # checking_status=='b'<0'' AND job=='b'skilled'' AND other_parties=='b'none'' AND savings_status=='b'<100''
-                       ps.Conjunction([NS_checking, NS_job, NS_other_parties, NS_savings_status]),
-                       ps.Conjunction([NS_checking, NS_foreign_worker, NS_job, NS_other_parties]),
-                       ps.Conjunction([NS_checking, NS_job, NS_savings_status]),
-                       ps.Conjunction([NS_checking, NS_foreign_worker, NS_other_parties, NS_savings_status]),
-                       ps.Conjunction([NS_checking, NS_foreign_worker, NS_other_parties]),
-                       ps.Conjunction([NS_checking, NS_foreign_worker, NS_savings_status]),
-                       ps.Conjunction([NS_checking, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_foreign_worker, NS_job, NS_dependents, NS_savings_status]),
-                       ps.Conjunction([NS_checking, NS_job, NS_other_parties])]
-
-        self.qualities = [0.11457431093955019,
-                          0.113713540226172,
-                          0.11201325679119281,
-                          0.1117538749727658,
-                          0.11161046793076415,
-                          0.11145710640046322,
-                          0.11045259291161472,
-                          0.10929088624672183,
-                          0.10875519439407161,
-                          0.10866138825404954,
-                          0.10832735026213287,
-                          0.10813405094128754]
+        self.result = [
+            ps.Conjunction(
+                [
+                    NS_checking,
+                    NS_foreign_worker,
+                    NS_job,
+                    NS_other_parties,
+                    NS_savings_status,
+                ]
+            ),  # AND job=='b'skilled'' AND other_parties=='b'none'' AND savings_status=='b'<100'
+            # 0.113713540226172:    checking_status=='b'<0'' AND foreign_worker=='b'yes'' AND job=='b'skilled'' AND savings_status=='b'<100''
+            ps.Conjunction([NS_checking, NS_foreign_worker, NS_job, NS_savings_status]),
+            ps.Conjunction(
+                [NS_checking, NS_foreign_worker, NS_job]
+            ),  # checking_status=='b'<0'' AND foreign_worker=='b'yes'' AND job=='b'skilled''
+            # checking_status=='b'<0'' AND job=='b'skilled'' AND other_parties=='b'none'' AND savings_status=='b'<100''
+            ps.Conjunction([NS_checking, NS_job, NS_other_parties, NS_savings_status]),
+            ps.Conjunction([NS_checking, NS_foreign_worker, NS_job, NS_other_parties]),
+            ps.Conjunction([NS_checking, NS_job, NS_savings_status]),
+            ps.Conjunction(
+                [NS_checking, NS_foreign_worker, NS_other_parties, NS_savings_status]
+            ),
+            ps.Conjunction([NS_checking, NS_foreign_worker, NS_other_parties]),
+            ps.Conjunction([NS_checking, NS_foreign_worker, NS_savings_status]),
+            ps.Conjunction([NS_checking, NS_foreign_worker]),
+            ps.Conjunction(
+                [
+                    NS_checking,
+                    NS_foreign_worker,
+                    NS_job,
+                    NS_dependents,
+                    NS_savings_status,
+                ]
+            ),
+            ps.Conjunction([NS_checking, NS_job, NS_other_parties]),
+        ]
+
+        self.qualities = [
+            0.11457431093955019,
+            0.113713540226172,
+            0.11201325679119281,
+            0.1117538749727658,
+            0.11161046793076415,
+            0.11145710640046322,
+            0.11045259291161472,
+            0.10929088624672183,
+            0.10875519439407161,
+            0.10866138825404954,
+            0.10832735026213287,
+            0.10813405094128754,
+        ]
         data = get_credit_data()
-        target = ps.BinaryTarget('class', b'bad')
-        searchSpace_Nominal = ps.create_nominal_selectors(data, ignore=['class'])
-        searchSpace_Numeric = ps.create_numeric_selectors(data, ignore=['class'])
+        target = ps.BinaryTarget("class", b"bad")
+        searchSpace_Nominal = ps.create_nominal_selectors(data, ignore=["class"])
+        searchSpace_Numeric = ps.create_numeric_selectors(data, ignore=["class"])
         searchSpace = searchSpace_Nominal + searchSpace_Numeric
-        self.task = ps.SubgroupDiscoveryTask(data, target, searchSpace, result_set_size=12, depth=5, qf=ps.StandardQF(0.5))
+        self.task = ps.SubgroupDiscoveryTask(
+            data,
+            target,
+            searchSpace,
+            result_set_size=12,
+            depth=5,
+            qf=ps.StandardQF(0.5),
+        )
 
-    @pytest.mark.slow
+    # @pytest.mark.slow  # not really that slow (< 1 min)
     def test_BestFirstSearch(self):
-        super.test_BestFirstSearch()
+        super().test_BestFirstSearch()
 
-    @pytest.mark.slow
-    def test_SimpleDFS(self):
-        super.test_SimpleDFS()
-
-    @pytest.mark.slow
-    def test_DFS_numpy_sets(self):
-        super.test_DFS_numpy_sets()
+    @pytest.mark.slow  #  (< 2 min)
+    def test_SimpleDFS_slow(self):
+        super().test_SimpleDFS()
 
+    @pytest.mark.slow  # (< 1 min)
+    def test_DFS_numpy_sets_slow(self):
+        super().test_DFS_numpy_sets()
 
-if __name__ == '__main__':
 
-    #unittest.main()
+if __name__ == "__main__":
+    # unittest.main()
     suites = []
     suites.append(unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms))
     suites.append(unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms2))
-    suites.append(unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms3))
+    # suites.append(unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms3))
     complete_suite = unittest.TestSuite(suites)
     unittest.TextTestRunner(verbosity=2).run(complete_suite)
 
-    #import cProfile
+    # import cProfile
     # p=cProfile.Profile()
     # p.enable()
     # t=TestAlgorithms()
     # t.setUp()
     # t.test_BSD()
 
     # p.disable()
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_algorithms_boolean_constraints.py` & `pysubgroup-0.7.6/tests/test_algorithms_boolean_constraints.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,200 @@
+# flake8: noqa: E501
+
 import unittest
+
 import pytest
+from algorithms_testing import TestAlgorithmsBase
+
 import pysubgroup as ps
-from pysubgroup.tests.DataSets import get_credit_data
+from pysubgroup.datasets import get_credit_data
 
-from pysubgroup.tests.algorithms_testing import TestAlgorithmsBase
 
 class TestSettings:
     All = True
     Apriori = False
     SimpleDFS = False
     BestFirstSearch = False
     BeamSearch = False
     DFS_bitset = False
     DFS_set = False
     DFS_numpyset = False
     SimpleSearch = False
 
+
 skip_long_running = True
-class BooleanTargetBase(TestAlgorithmsBase):
 
+
+class BooleanTargetBase(TestAlgorithmsBase):
     # pylint: disable=no-member
-    @unittest.skipUnless(TestSettings.All or TestSettings.Apriori, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.Apriori, "flag not set")
     def test_Apriori(self):
-        self.runAlgorithm(ps.Apriori(), "Apriori", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.Apriori(), "Apriori", self.result, self.qualities, self.task
+        )
 
-    @unittest.skipUnless(TestSettings.SimpleDFS, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.SimpleDFS, "flag not set")
     def test_SimpleDFS(self):
-        self.runAlgorithm(ps.SimpleDFS(), "SimpleDFS", self.result, self.qualities, self.task)
-
-    @unittest.skipUnless(TestSettings.All or TestSettings.BestFirstSearch, 'flag not set')
+        self.runAlgorithm(
+            ps.SimpleDFS(), "SimpleDFS", self.result, self.qualities, self.task
+        )
+
+    @unittest.skipUnless(
+        TestSettings.All or TestSettings.BestFirstSearch, "flag not set"
+    )
     def test_BestFirstSearch(self):
-        self.runAlgorithm(ps.BestFirstSearch(), "BestFirstSearch", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.BestFirstSearch(),
+            "BestFirstSearch",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
-    @unittest.skipUnless(TestSettings.All or TestSettings.BeamSearch, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.BeamSearch, "flag not set")
     def test_BeamSearch(self):
-        self.runAlgorithm(ps.BeamSearch(beam_width=12), "BeamSearch", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.BeamSearch(beam_width=12),
+            "BeamSearch",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
-    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_bitset, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_bitset, "flag not set")
     def test_DFS_bitset(self):
-        self.runAlgorithm(ps.DFS(ps.BitSetRepresentation), "DFS bitset", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.DFS(ps.BitSetRepresentation),
+            "DFS bitset",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
     @pytest.mark.slow
-    @unittest.skipUnless(TestSettings.SimpleSearch, 'flag not set')
-    def test_SimpleSearch(self):
-        self.runAlgorithm(ps.SimpleSearch(), "SimpleSearch", self.result, self.qualities, self.task)
+    @unittest.skipUnless(TestSettings.SimpleSearch, "flag not set")
+    def test_SimpleSearch_slow(self):
+        self.runAlgorithm(
+            ps.SimpleSearch(), "SimpleSearch", self.result, self.qualities, self.task
+        )
 
-    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_set, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_set, "flag not set")
     def test_DFS_set(self):
-        self.runAlgorithm(ps.DFS(ps.SetRepresentation), "DFS set", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.DFS(ps.SetRepresentation),
+            "DFS set",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
-    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_numpyset, 'flag not set')
+    @unittest.skipUnless(TestSettings.All or TestSettings.DFS_numpyset, "flag not set")
     def test_DFS_numpy_sets(self):
-        self.runAlgorithm(ps.DFS(ps.NumpySetRepresentation), "DFS numpyset", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.DFS(ps.NumpySetRepresentation),
+            "DFS numpyset",
+            self.result,
+            self.qualities,
+            self.task,
+        )
+
+    @unittest.skipUnless(TestSettings.All or TestSettings.GpGrowth, "flag not set")
+    def test_gp_growth(self):
+        self.runAlgorithm(
+            ps.GpGrowth(), "GpGrowth", self.result, self.qualities, self.task
+        )
 
     def evaluate_result(self, algorithm_result, result, qualities):
         df = algorithm_result.to_dataframe()
-        self.assertTrue(all(algorithm_result.task.constraints[0].min_support <= df['size_sg']))
+        self.assertTrue(
+            all(algorithm_result.task.constraints[0].min_support <= df["size_sg"])
+        )
         TestAlgorithmsBase.evaluate_result(self, algorithm_result, result, qualities)
+
     # pylint: enable=no-member
+
+
 class TestAlgorithms(BooleanTargetBase, unittest.TestCase):
     def setUp(self):
         NS_checking = ps.EqualitySelector("checking_status", b"<0")
         NS_foreign_worker = ps.EqualitySelector("foreign_worker", b"yes")
         NS_other_parties = ps.EqualitySelector("other_parties", b"none")
         NS_savings_status = ps.EqualitySelector("savings_status", b"<100")
         NS_payment_plans = ps.EqualitySelector("other_payment_plans", b"none")
-        self.result = [ps.Conjunction([NS_checking, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking]),
-                       ps.Conjunction([NS_checking, NS_other_parties, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_other_parties]),
-                       ps.Conjunction([NS_checking, NS_savings_status, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_savings_status]),
-                       ps.Conjunction([NS_checking, NS_foreign_worker, NS_payment_plans]),
-                       ps.Conjunction([NS_checking, NS_payment_plans]),
-                       ps.Conjunction([NS_foreign_worker, NS_savings_status]),
-                       ps.Conjunction([NS_foreign_worker, NS_other_parties, NS_savings_status]),
-                       ]
-        self.qualities = [0.055299999999999995,
-                          0.05280000000000001,
-                          0.052300000000000006,
-                          0.05059999999999999,
-                          0.04959999999999999,
-                          0.048299999999999996,
-                          0.0426,
-                          0.04,
-                          0.03869999999999999,
-                          0.03750000000000001]
+        self.result = [
+            ps.Conjunction([NS_checking, NS_foreign_worker]),
+            ps.Conjunction([NS_checking]),
+            ps.Conjunction([NS_checking, NS_other_parties, NS_foreign_worker]),
+            ps.Conjunction([NS_checking, NS_other_parties]),
+            ps.Conjunction([NS_checking, NS_savings_status, NS_foreign_worker]),
+            ps.Conjunction([NS_checking, NS_savings_status]),
+            ps.Conjunction([NS_checking, NS_foreign_worker, NS_payment_plans]),
+            ps.Conjunction([NS_checking, NS_payment_plans]),
+            ps.Conjunction([NS_foreign_worker, NS_savings_status]),
+            ps.Conjunction([NS_foreign_worker, NS_other_parties, NS_savings_status]),
+        ]
+        self.qualities = [
+            0.055299999999999995,
+            0.05280000000000001,
+            0.052300000000000006,
+            0.05059999999999999,
+            0.04959999999999999,
+            0.048299999999999996,
+            0.0426,
+            0.04,
+            0.03869999999999999,
+            0.03750000000000001,
+        ]
         data = get_credit_data()
-        target = ps.BinaryTarget('class', b'bad')
-        searchSpace = ps.create_nominal_selectors(data, ignore=['class'])
-        self.task = ps.SubgroupDiscoveryTask(data, target, searchSpace, result_set_size=10, depth=5, qf=ps.StandardQF(1.0), constraints=[ps.MinSupportConstraint(200)])
+        target = ps.BinaryTarget("class", b"bad")
+        searchSpace = ps.create_nominal_selectors(data, ignore=["class"])
+        self.task = ps.SubgroupDiscoveryTask(
+            data,
+            target,
+            searchSpace,
+            result_set_size=10,
+            depth=5,
+            qf=ps.StandardQF(1.0),
+            constraints=[ps.MinSupportConstraint(200)],
+        )
+
+
+# class TestAlgorithms2(BooleanTargetBase, unittest.TestCase):
+#     def setUp(self):
+#         NS_checking = ps.EqualitySelector("checking_status", b"<0")
+#         NS_foreign_worker = ps.EqualitySelector("foreign_worker", b"yes")
+#         NS_other_parties = ps.EqualitySelector("other_parties", b"none")
+#         NS_savings_status = ps.EqualitySelector("savings_status", b"<100")
+#         NS_payment_plans = ps.EqualitySelector("other_payment_plans", b"none")
+#         NS_job = ps.EqualitySelector("job", b"skilled")
+#         self.result = [
+#             ps.Conjunction([NS_savings_status]),
+#             ps.Conjunction([NS_foreign_worker]),
+#             ps.Conjunction([NS_foreign_worker, NS_other_parties]),
+#             ps.Conjunction([NS_foreign_worker, NS_job]),
+#         ]
+#         self.qualities = [
+#             0.03610000000000002,
+#             0.0071000000000000256,
+#             0.004999999999999996,
+#             0.0006999999999999932,
+#         ]
+#         data = get_credit_data()
+#         target = ps.BinaryTarget("class", b"bad")
+#         searchSpace = ps.create_nominal_selectors(data, ignore=["class"])
+#         self.task = ps.SubgroupDiscoveryTask(
+#             data,
+#             target,
+#             searchSpace,
+#             result_set_size=10,
+#             depth=5,
+#             qf=ps.StandardQF(1.0),
+#             constraints=[ps.MinSupportConstraint(600)],
+#         )
+
 
 #   0.055299999999999995:        checking_status=='b'<0'' AND foreign_worker=='b'yes''
 #   0.05280000000000001: checking_status=='b'<0''
 #   0.052300000000000006:        checking_status=='b'<0'' AND foreign_worker=='b'yes'' AND other_parties=='b'none''
 #   0.05059999999999999: checking_status=='b'<0'' AND other_parties=='b'none''
 #   0.04959999999999999: checking_status=='b'<0'' AND foreign_worker=='b'yes'' AND savings_status=='b'<100''
 #   0.048299999999999996:        checking_status=='b'<0'' AND savings_status=='b'<100''
@@ -102,26 +203,25 @@
 #   0.03869999999999999: foreign_worker=='b'yes'' AND savings_status=='b'<100''
 #   0.03750000000000001: foreign_worker=='b'yes'' AND other_parties=='b'none'' AND savings_status=='b'<100''
 
 
 # also includes numeric attributes and has 12 targets
 
 
-
-if __name__ == '__main__':
-
-    #unittest.main()
+if __name__ == "__main__":
+    # unittest.main()
     suites = []
     suites.append(unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms))
-    #suites.append(unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms2))
-    #suites.append( unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms3))
+    # suites.append(unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms2))
+    # suites.append(unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms2))
+    # suites.append( unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms3))
     complete_suite = unittest.TestSuite(suites)
     unittest.TextTestRunner(verbosity=2).run(complete_suite)
 
-    #import cProfile
+    # import cProfile
     # p=cProfile.Profile()
     # p.enable()
     # t=TestAlgorithms()
     # t.setUp()
     # t.test_BSD()
 
     # p.disable()
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_algorithms_numeric.py` & `pysubgroup-0.7.6/tests/test_algorithms_numeric.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,132 +1,191 @@
+# flake8: noqa: E501
+
 # 383476.7679999999:      own_telephone=='b'yes''
 # 361710.05800000014:     foreign_worker=='b'yes'' and own_telephone=='b'yes''
 # 345352.9920000001:      other_parties=='b'none'' and own_telephone=='b'yes''
 # 338205.08:      foreign_worker=='b'yes'' and own_telephone=='b'yes'' and personal_status=='b'male single''
 # 336857.8220000001:      own_telephone=='b'yes'' and personal_status=='b'male single''
 # 323586.28200000006:     foreign_worker=='b'yes'' and other_parties=='b'none'' and own_telephone=='b'yes''
 # 320306.81600000005:     job=='b'high qualif/self emp/mgmt''
 # 300963.84599999996:     class=='b'bad'' and own_telephone=='b'yes''
 # 299447.332:     foreign_worker=='b'yes'' and job=='b'high qualif/self emp/mgmt''
 # 297422.98200000013:     foreign_worker=='b'yes'' and other_parties=='b'none'' and own_telephone=='b'yes'' and personal_status=='b'male single''
 
 import unittest
-import pysubgroup as ps
 
+from algorithms_testing import TestAlgorithmsBase
+
+import pysubgroup as ps
+from pysubgroup.datasets import get_credit_data
 
-from pysubgroup.tests.DataSets import get_credit_data
-from pysubgroup.tests.algorithms_testing import TestAlgorithmsBase
 
 class TestStandardQFNumeric(unittest.TestCase):
     def test_constructor(self):
         ps.StandardQFNumeric(0)
         ps.StandardQFNumeric(1.0)
         ps.StandardQFNumeric(0, invert=True)
         ps.StandardQFNumeric(0, invert=False)
 
         with self.assertRaises(ValueError):
-            ps.StandardQFNumeric('test')
+            ps.StandardQFNumeric("test")
 
-        ps.StandardQFNumeric(0, estimator='sum')
-        ps.StandardQFNumeric(0, estimator='average')
-        ps.StandardQFNumeric(0, estimator='order')
+        ps.StandardQFNumeric(0, estimator="sum")
+        ps.StandardQFNumeric(0, estimator="average")
+        ps.StandardQFNumeric(0, estimator="order")
 
         with self.assertRaises(ValueError):
-            ps.StandardQFNumeric(0, estimator='bla')
+            ps.StandardQFNumeric(0, estimator="bla")
 
 
 class TestAlgorithmsWithNumericTarget(TestAlgorithmsBase, unittest.TestCase):
     def setUp(self):
         NS_telephone = ps.EqualitySelector("own_telephone", b"yes")
         NS_foreign_worker = ps.EqualitySelector("foreign_worker", b"yes")
         NS_other_parties = ps.EqualitySelector("other_parties", b"none")
-        NS_personal = ps.EqualitySelector("personal_status", b'male single')
-        NS_job = ps.EqualitySelector("job", b'high qualif/self emp/mgmt')
+        NS_personal = ps.EqualitySelector("personal_status", b"male single")
+        NS_job = ps.EqualitySelector("job", b"high qualif/self emp/mgmt")
         NS_class = ps.EqualitySelector("class", b"bad")
 
-        o = [[NS_telephone],
-             [NS_foreign_worker, NS_telephone],
-             [NS_other_parties, NS_telephone],
-             [NS_foreign_worker, NS_telephone, NS_personal],
-             [NS_telephone, NS_personal],
-             [NS_foreign_worker, NS_other_parties, NS_telephone],
-             [NS_job],
-             [NS_class, NS_telephone],
-             [NS_foreign_worker, NS_job],
-             [NS_foreign_worker, NS_other_parties, NS_telephone, NS_personal]
-             ]
+        o = [
+            [NS_telephone],
+            [NS_foreign_worker, NS_telephone],
+            [NS_other_parties, NS_telephone],
+            [NS_foreign_worker, NS_telephone, NS_personal],
+            [NS_telephone, NS_personal],
+            [NS_foreign_worker, NS_other_parties, NS_telephone],
+            [NS_job],
+            [NS_class, NS_telephone],
+            [NS_foreign_worker, NS_job],
+            [NS_foreign_worker, NS_other_parties, NS_telephone, NS_personal],
+        ]
         self.result = list(map(ps.Conjunction, o))
         self.qualities = [
             383476.7679999999,
             361710.05800000014,
             345352.9920000001,
             338205.08,
             336857.8220000001,
             323586.28200000006,
             320306.81600000005,
             300963.84599999996,
             299447.332,
-            297422.98200000013]
+            297422.98200000013,
+        ]
 
         data = get_credit_data()
-        target = ps.NumericTarget('credit_amount')
-        searchSpace_Nominal = ps.create_nominal_selectors(data, ignore=['credit_amount'])
-        searchSpace_Numeric = [] #ps.create_numeric_selectors(data, ignore=['credit_amount'], nbins=10)
+        target = ps.NumericTarget("credit_amount")
+        searchSpace_Nominal = ps.create_nominal_selectors(
+            data, ignore=["credit_amount"]
+        )
+        searchSpace_Numeric = (
+            []
+        )  # ps.create_numeric_selectors(data, ignore=['credit_amount'], nbins=10)
         searchSpace = searchSpace_Nominal + searchSpace_Numeric
-        self.task = ps.SubgroupDiscoveryTask(data, target, searchSpace, result_set_size=10, depth=5, qf=ps.CountCallsInterestingMeasure(ps.StandardQFNumeric(1, False, 'sum')))
+        self.task = ps.SubgroupDiscoveryTask(
+            data,
+            target,
+            searchSpace,
+            result_set_size=10,
+            depth=5,
+            qf=ps.StandardQFNumeric(1, False, "sum"),
+        )
 
     def test_SimpleDFS(self):
-        self.runAlgorithm(ps.SimpleDFS(), "SimpleDFS", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.SimpleDFS(), "SimpleDFS", self.result, self.qualities, self.task
+        )
 
     def test_DFS_average(self):
-        self.task.qf = ps.CountCallsInterestingMeasure(ps.StandardQFNumeric(self.task.qf.a, False, 'average'))
-        self.runAlgorithm(ps.DFS(ps.BitSetRepresentation), "DFS average", self.result, self.qualities, self.task)
+        self.task.qf = ps.StandardQFNumeric(self.task.qf.a, False, "average")
+        self.runAlgorithm(
+            ps.DFS(ps.BitSetRepresentation),
+            "DFS average",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
     def test_DFS_order(self):
-        self.task.qf = ps.CountCallsInterestingMeasure(ps.StandardQFNumeric(self.task.qf.a, False, 'order'))
-        self.runAlgorithm(ps.DFS(ps.BitSetRepresentation), "DFS order", self.result, self.qualities, self.task)
+        self.task.qf = ps.StandardQFNumeric(self.task.qf.a, False, "order")
+        self.runAlgorithm(
+            ps.DFS(ps.BitSetRepresentation),
+            "DFS order",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
     def test_DFS_sum(self):
-        self.task.qf = ps.CountCallsInterestingMeasure(ps.StandardQFNumeric(self.task.qf.a, False, 'sum'))
-        self.runAlgorithm(ps.DFS(ps.BitSetRepresentation), "DFS sum", self.result, self.qualities, self.task)
+        self.task.qf = ps.StandardQFNumeric(self.task.qf.a, False, "sum")
+        self.runAlgorithm(
+            ps.DFS(ps.BitSetRepresentation),
+            "DFS sum",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
     def test_BeamSearch_sum(self):
-        self.task.qf = ps.CountCallsInterestingMeasure(ps.StandardQFNumeric(self.task.qf.a, False, 'sum'))
-        self.runAlgorithm(ps.BeamSearch(), "BeamSearch sum", self.result, self.qualities, self.task)
+        self.task.qf = ps.StandardQFNumeric(self.task.qf.a, False, "sum")
+        self.runAlgorithm(
+            ps.BeamSearch(), "BeamSearch sum", self.result, self.qualities, self.task
+        )
 
     def test_BeamSearch_average(self):
-        self.task.qf = ps.CountCallsInterestingMeasure(ps.StandardQFNumeric(self.task.qf.a, False, 'average'))
-        self.runAlgorithm(ps.BeamSearch(), "BeamSearch average", self.result, self.qualities, self.task)
+        self.task.qf = ps.StandardQFNumeric(self.task.qf.a, False, "average")
+        self.runAlgorithm(
+            ps.BeamSearch(),
+            "BeamSearch average",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
     def test_BeamSearch_order(self):
-        self.task.qf = ps.CountCallsInterestingMeasure(ps.StandardQFNumeric(self.task.qf.a, False, 'order'))
-        self.runAlgorithm(ps.BeamSearch(), "BeamSearch order", self.result, self.qualities, self.task)
+        self.task.qf = ps.StandardQFNumeric(self.task.qf.a, False, "order")
+        self.runAlgorithm(
+            ps.BeamSearch(), "BeamSearch order", self.result, self.qualities, self.task
+        )
 
     def test_Apriori_no_numba(self):
-        self.runAlgorithm(ps.Apriori(use_numba=False), "Apriori use_numba=False", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.Apriori(use_numba=False),
+            "Apriori use_numba=False",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
     def test_Apriori_with_numba(self):
-        self.runAlgorithm(ps.Apriori(use_numba=True), "Apriori use_numba=True", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.Apriori(use_numba=True),
+            "Apriori use_numba=True",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
     def test_DFSNumeric(self):
-        algo = ps.DFSNumeric()
-        self.runAlgorithm(algo, "DFS_numeric", self.result, self.qualities, self.task)
-        print('   Number of call to qf:', algo.num_calls)
+        self.runAlgorithm(
+            ps.DFSNumeric(), "DFS_numeric", self.result, self.qualities, self.task
+        )
+        # print('   Number of call to qf:', algo.num_calls)
 
-    #def test_SimpleSearch(self):
+    # def test_SimpleSearch(self):
     #   self.runAlgorithm(ps.SimpleSearch(), "SimpleSearch", self.result, self.qualities, self.task)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
 
 
-   # 639577.0460000001:   duration>=30.0
-   # 624424.3040000001:   duration>=30.0 AND foreign_worker=='b'yes''
-   # 579219.206:  duration>=30.0 AND other_parties=='b'none''
-   # 564066.4640000002:   duration>=30.0 AND foreign_worker=='b'yes'' AND other_parties=='b'none''
-   # 547252.302:  duration>=30.0 AND num_dependents==1.0
-   # 532099.56:   duration>=30.0 AND foreign_worker=='b'yes'' AND num_dependents==1.0
-   # 491104.688:  duration>=30.0 AND num_dependents==1.0 AND other_parties=='b'none''
-   # 490633.1400000001:   duration>=30.0 AND foreign_worker=='b'yes'' AND other_payment_plans=='b'none''
-   # 490633.1400000001:   duration>=30.0 AND other_payment_plans=='b'none''
-   # 475951.94600000005:  duration>=30.0 AND foreign_worker=='b'yes'' AND num_dependents==1.0 AND other_parties=='b'none''
+# 639577.0460000001:   duration>=30.0
+# 624424.3040000001:   duration>=30.0 AND foreign_worker=='b'yes''
+# 579219.206:  duration>=30.0 AND other_parties=='b'none''
+# 564066.4640000002:   duration>=30.0 AND foreign_worker=='b'yes'' AND other_parties=='b'none''
+# 547252.302:  duration>=30.0 AND num_dependents==1.0
+# 532099.56:   duration>=30.0 AND foreign_worker=='b'yes'' AND num_dependents==1.0
+# 491104.688:  duration>=30.0 AND num_dependents==1.0 AND other_parties=='b'none''
+# 490633.1400000001:   duration>=30.0 AND foreign_worker=='b'yes'' AND other_payment_plans=='b'none''
+# 490633.1400000001:   duration>=30.0 AND other_payment_plans=='b'none''
+# 475951.94600000005:  duration>=30.0 AND foreign_worker=='b'yes'' AND num_dependents==1.0 AND other_parties=='b'none''
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_boolean_expressions.py` & `pysubgroup-0.7.6/tests/test_boolean_expressions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 import unittest
 
 import numpy as np
 import pandas as pd
+
 import pysubgroup as ps
 
 
 class TestRelationsMethods(unittest.TestCase):
-
     def check_dataframe_query(self, selector, result):
         result1 = np.array(result, dtype=bool)
         np.testing.assert_array_equal(selector.covers(self.df), result1)
         np.testing.assert_array_equal(self.df.query(repr(selector)), self.df[result1])
 
+    def test_Disjunction(self):
+        dis1 = ps.Disjunction(ps.EqualitySelector("A1", 1))
+        dis2 = ps.Disjunction(ps.EqualitySelector("A2", 1))
+        dis_test = dis1 | dis2
+        dis12 = ps.Disjunction(
+            [ps.EqualitySelector("A1", 1), ps.EqualitySelector("A2", 1)]
+        )
+        self.assertEqual(dis_test, dis12)
+
+    def test_Conjunction(self):
+        conj = ps.Conjunction(ps.EqualitySelector("A1", 1))
+        conj.append_and([ps.EqualitySelector("A1", 1)])
+
     def test_DNF(self):
         A1 = ps.EqualitySelector("A1", 1)
         A2 = ps.EqualitySelector("A2", 1, "AA")
         B1 = ps.EqualitySelector("B1", 1)
         B2 = ps.EqualitySelector("B2", "1")
 
         dnf1 = ps.DNF()
@@ -33,23 +46,48 @@
         self.assertTrue(dnf4 == dnf5)
 
         dnf6 = ps.DNF([])
         dnf6.append_and([B1, B2])
         dnf7 = ps.DNF([])
         dnf7.append_and([A1, A2])
         dnf7.append_or(ps.Conjunction([B1, B2]))
-        self.df = pd.DataFrame.from_dict({"A1": [1, 1, 1, 2, 2, 2, 2, 0, 0, 0], #pylint: disable=attribute-defined-outside-init
-                                          "A2": [0, 1, 1, 1, 2, 2, 2, 0, 0, 0],
-                                          "B1": [0, 0, 0, 0, 1, 1, 1, 0, 1, 1],
-                                          "B2": ["0", "0", "0", "0", "1", "1", "2", "0", "0", "1"]})
+        with self.assertRaises(RuntimeError):
+            dnf7.pop_and()
+        self.df = pd.DataFrame.from_dict(
+            {
+                "A1": [
+                    1,
+                    1,
+                    1,
+                    2,
+                    2,
+                    2,
+                    2,
+                    0,
+                    0,
+                    0,
+                ],  # pylint: disable=attribute-defined-outside-init
+                "A2": [0, 1, 1, 1, 2, 2, 2, 0, 0, 0],
+                "B1": [0, 0, 0, 0, 1, 1, 1, 0, 1, 1],
+                "B2": ["0", "0", "0", "0", "1", "1", "2", "0", "0", "1"],
+            }
+        )
         self.check_dataframe_query(dnf1, [1, 1, 1, 1, 0, 0, 0, 0, 0, 0])
         self.check_dataframe_query(dnf3, [0, 1, 1, 0, 0, 0, 0, 0, 0, 0])
         self.check_dataframe_query(dnf6, [0, 0, 0, 0, 1, 1, 0, 0, 0, 1])
         self.check_dataframe_query(dnf7, [0, 1, 1, 0, 1, 1, 0, 0, 0, 1])
 
+        dnf8 = ps.DNF([])
+        dnf8.append_and([A1, A2])
+        dnf8.append_or(ps.Conjunction([B1, A2]))
+        self.assertEqual(dnf8.pop_and(), A2)
+        dnf8.append_or(ps.Disjunction([A2]))
+        with self.assertRaises(NotImplementedError):
+            dnf8.append_and(ps.Disjunction([A2]))
+
     def test_equality_expressions(self):
         A1 = ps.EqualitySelector("A", 1)
         A2 = ps.EqualitySelector("A", 2, "AA")
         B1 = ps.EqualitySelector("B", 1)
 
         D1 = ps.Disjunction([A1, A2])
         D1_clone = ps.Disjunction([A1, A2])
@@ -71,9 +109,9 @@
         self.assertTrue(C_all == C1_clone)
         self.assertTrue(hash(C_all) == hash(C1_clone))
 
         self.assertFalse(C1 == D1)
         self.assertFalse(hash(C1) == hash(D1))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_fi_target.py` & `pysubgroup-0.7.6/tests/test_fi_target.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,190 @@
 import unittest
+
 import numpy as np
+from algorithms_testing import TestAlgorithmsBase
+
 import pysubgroup as ps
-from pysubgroup.tests.DataSets import get_titanic_data
-from pysubgroup.tests.algorithms_testing import TestAlgorithmsBase
+from pysubgroup.datasets import get_titanic_data
 
+# data=get_titanic_data()
+# search_space = ps.create_selectors(data, ignore="survived")
+# dt = data.dtypes
 
+# task = ps.SubgroupDiscoveryTask(
+#     data, ps.FITarget, search_space, result_set_size=10, depth=5, qf=ps.CountQF())
+# result = ps.SimpleDFS().execute(task)
 
-#data=get_titanic_data()
-#search_space = ps.create_selectors(data, ignore="survived")
-#dt = data.dtypes
+# for (q, sg) in result:
+#    print(str(q) + ":\t" + str(sg.subgroup_description))
 
-#task = ps.SubgroupDiscoveryTask(data, ps.FITarget, search_space, result_set_size=10, depth=5, qf=ps.CountQF())
-#result = ps.SimpleDFS().execute(task)
+# task = ps.SubgroupDiscoveryTask(
+#     data, ps.FITarget, search_space, result_set_size=10, depth=2, qf=ps.AreaQF())
+# result = ps.SimpleDFS().execute(task)
 
-#for (q, sg) in result:
+# for (q, sg) in result:
 #    print(str(q) + ":\t" + str(sg.subgroup_description))
 
-#task = ps.SubgroupDiscoveryTask(data, ps.FITarget, search_space, result_set_size=10, depth=2, qf=ps.AreaQF())
-#result = ps.SimpleDFS().execute(task)
+# df_test1 = pd.DataFrame.from_records(
+#   [[1,1,1],[0,0,1],[0,0,1]], columns=["A", "B", "C"])
+
+
+class TestFITarget(TestAlgorithmsBase, unittest.TestCase):
+    def test_fi_target(self):
+        target = ps.FITarget()
+        self.assertEqual(target.get_attributes(), [])
+
+        df = get_titanic_data()
+        NS_embarked = ps.EqualitySelector("Embarked", "S")
+        self.assertEqual(target.get_base_statistics(NS_embarked, df), 110)
+
+        statistics = target.calculate_statistics(NS_embarked, df)
+        self.assertDictEqual(statistics, {"size_sg": 110, "size_dataset": 156})
+        statistics2 = target.calculate_statistics(
+            NS_embarked, df, cached_statistics=statistics
+        )
+        self.assertIs(statistics2, statistics)
 
-#for (q, sg) in result:
-#    print(str(q) + ":\t" + str(sg.subgroup_description))
 
 class TestCountQF(TestAlgorithmsBase, unittest.TestCase):
     def test_Apriori(self):
-        self.runAlgorithm(ps.Apriori(), "Apriori", self.result[1:], self.qualities[1:], self.task)
+        self.runAlgorithm(
+            ps.Apriori(), "Apriori", self.result[1:], self.qualities[1:], self.task
+        )
 
     def test_DFS(self):
-        self.runAlgorithm(ps.SimpleDFS(), "DFS", self.result[:-1], self.qualities[:-1], self.task)
+        self.runAlgorithm(
+            ps.SimpleDFS(), "DFS", self.result[:-1], self.qualities[:-1], self.task
+        )
+
+    def test_gp_growth(self):
+        self.task.constraints_monotone.append(ps.MinSupportConstraint(20))
+        self.runAlgorithm(
+            ps.GpGrowth(), "GpGrowth", self.result[:-1], self.qualities[:-1], self.task
+        )
+        self.task.constraints_monotone.pop(-1)
+
+    def test_gp_growth_top_down(self):
+        self.task.constraints_monotone.append(ps.MinSupportConstraint(20))
+        self.runAlgorithm(
+            ps.GpGrowth(mode="t_d"),
+            "GpGrowth",
+            self.result[:-1],
+            self.qualities[:-1],
+            self.task,
+        )
+        self.task.constraints_monotone.pop(-1)
 
     def setUp(self):
         NS_cabin = ps.EqualitySelector("Cabin", np.nan)
-        NS_embarked = ps.EqualitySelector("Embarked", 'S')
-        NS_male = ps.EqualitySelector("Sex", 'male')
-        NS_female = ps.EqualitySelector("Sex", 'female')
-        #NS_other_parties = ps.EqualitySelector("other_parties", b"none")
-        #NS_savings_status = ps.EqualitySelector("savings_status", b"<100")
-        #NS_job = ps.EqualitySelector("job", b"skilled")
-        self.result = [ps.Conjunction([]),
-                       ps.Conjunction([NS_cabin]),
-                       ps.Conjunction([NS_embarked]),
-                       ps.Conjunction([NS_male]),
-                       ps.Conjunction([NS_cabin, NS_embarked]),
-                       ps.Conjunction([NS_cabin, NS_male]),
-                       ps.Conjunction([NS_embarked, NS_male]),
-                       ps.Conjunction([NS_cabin, NS_embarked, NS_male]),
-                       ps.Conjunction([NS_female]),
-                       ps.Conjunction([NS_cabin, NS_female]),
-                       ps.Conjunction([NS_embarked, NS_female])]
+        NS_embarked = ps.EqualitySelector("Embarked", "S")
+        NS_male = ps.EqualitySelector("Sex", "male")
+        NS_female = ps.EqualitySelector("Sex", "female")
+        # NS_other_parties = ps.EqualitySelector("other_parties", b"none")
+        # NS_savings_status = ps.EqualitySelector("savings_status", b"<100")
+        # NS_job = ps.EqualitySelector("job", b"skilled")
+        self.result = [
+            ps.Conjunction([]),
+            ps.Conjunction([NS_cabin]),
+            ps.Conjunction([NS_embarked]),
+            ps.Conjunction([NS_male]),
+            ps.Conjunction([NS_cabin, NS_embarked]),
+            ps.Conjunction([NS_cabin, NS_male]),
+            ps.Conjunction([NS_embarked, NS_male]),
+            ps.Conjunction([NS_cabin, NS_embarked, NS_male]),
+            ps.Conjunction([NS_female]),
+            ps.Conjunction([NS_cabin, NS_female]),
+            ps.Conjunction([NS_embarked, NS_female]),
+        ]
 
         self.qualities = [156, 125, 110, 100, 89, 82, 73, 60, 56, 43, 37]
 
         data = get_titanic_data()
         self.qualities2 = [np.count_nonzero(conj.covers(data)) for conj in self.result]
         self.assertEqual(self.qualities, self.qualities2)
         searchSpace = ps.create_nominal_selectors(data)
-        self.task = ps.SubgroupDiscoveryTask(data, ps.FITarget(), searchSpace, result_set_size=10, depth=5, qf=ps.CountQF())
-
-
+        self.task = ps.SubgroupDiscoveryTask(
+            data,
+            ps.FITarget(),
+            searchSpace,
+            result_set_size=10,
+            depth=5,
+            qf=ps.CountQF(),
+        )
 
 
 class TestAreaQF(TestAlgorithmsBase, unittest.TestCase):
     def test_SimpleSearch(self):
-        self.runAlgorithm(ps.SimpleSearch(), "SimpleSearch", self.result, self.qualities, self.task)
-   # 178: Cabin.isnull() AND Embarked=='S'
-   #164: Cabin.isnull() AND Sex=='male'
-   #146: Embarked=='S' AND Sex=='male'
-   #125: Cabin.isnull()
-   #110: Embarked=='S'
-   #100: Sex=='male'
-   #86:  Cabin.isnull() AND Sex=='female'
-   #74:  Embarked=='S' AND Sex=='female'
-   #56:  Sex=='female'
-   #46:  Cabin.isnull() AND Embarked=='C'
+        self.runAlgorithm(
+            ps.SimpleSearch(), "SimpleSearch", self.result, self.qualities, self.task
+        )
+
+    # 178: Cabin.isnull() AND Embarked=='S'
+    # 164: Cabin.isnull() AND Sex=='male'
+    # 146: Embarked=='S' AND Sex=='male'
+    # 125: Cabin.isnull()
+    # 110: Embarked=='S'
+    # 100: Sex=='male'
+    # 86:  Cabin.isnull() AND Sex=='female'
+    # 74:  Embarked=='S' AND Sex=='female'
+    # 56:  Sex=='female'
+    # 46:  Cabin.isnull() AND Embarked=='C'
     def setUp(self):
         NS_cabin = ps.EqualitySelector("Cabin", np.nan)
-        NS_embarked = ps.EqualitySelector("Embarked", 'S')
-        NS_embarked2 = ps.EqualitySelector("Embarked", 'C')
-        NS_male = ps.EqualitySelector("Sex", 'male')
-        NS_female = ps.EqualitySelector("Sex", 'female')
-        #NS_other_parties = ps.EqualitySelector("other_parties", b"none")
-        #NS_savings_status = ps.EqualitySelector("savings_status", b"<100")
-        #NS_job = ps.EqualitySelector("job", b"skilled")
-        self.result = [ps.Conjunction([NS_cabin, NS_embarked]),
-                       ps.Conjunction([NS_cabin, NS_male]),
-                       ps.Conjunction([NS_embarked, NS_male]),
-                       ps.Conjunction([NS_cabin]),
-                       ps.Conjunction([NS_embarked]),
-                       ps.Conjunction([NS_male]),
-                       ps.Conjunction([NS_cabin, NS_female]),
-                       ps.Conjunction([NS_embarked, NS_female]),
-                       ps.Conjunction([NS_female]),
-                       ps.Conjunction([NS_cabin, NS_embarked2]),
-                       ]
+        NS_embarked = ps.EqualitySelector("Embarked", "S")
+        NS_embarked2 = ps.EqualitySelector("Embarked", "C")
+        NS_male = ps.EqualitySelector("Sex", "male")
+        NS_female = ps.EqualitySelector("Sex", "female")
+        # NS_other_parties = ps.EqualitySelector("other_parties", b"none")
+        # NS_savings_status = ps.EqualitySelector("savings_status", b"<100")
+        # NS_job = ps.EqualitySelector("job", b"skilled")
+        self.result = [
+            ps.Conjunction([NS_cabin, NS_embarked]),
+            ps.Conjunction([NS_cabin, NS_male]),
+            ps.Conjunction([NS_embarked, NS_male]),
+            ps.Conjunction([NS_cabin]),
+            ps.Conjunction([NS_embarked]),
+            ps.Conjunction([NS_male]),
+            ps.Conjunction([NS_cabin, NS_female]),
+            ps.Conjunction([NS_embarked, NS_female]),
+            ps.Conjunction([NS_female]),
+            ps.Conjunction([NS_cabin, NS_embarked2]),
+        ]
 
         self.qualities = [178, 164, 146, 125, 110, 100, 86, 74, 56, 46]
 
         data = get_titanic_data()
-        self.qualities2 = [np.count_nonzero(conj.covers(data))*conj.depth for conj in self.result]
+        self.qualities2 = [
+            np.count_nonzero(conj.covers(data)) * conj.depth for conj in self.result
+        ]
         self.assertEqual(self.qualities, self.qualities2)
         searchSpace = ps.create_nominal_selectors(data)
-        self.task = ps.SubgroupDiscoveryTask(data, ps.FITarget(), searchSpace, result_set_size=10, depth=2, qf=ps.AreaQF())
-
- #  156: True
- #  125: Cabin.isnull()
- #  110: Embarked=='S'
- #  100: Sex=='male'
- #  89:  Cabin.isnull() AND Embarked=='S'
- #  82:  Cabin.isnull() AND Sex=='male'
- #  73:  Embarked=='S' AND Sex=='male'
- #  60:  Cabin.isnull() AND Embarked=='S' AND Sex=='male'
- #  56:  Sex=='female'
- #  43:  Cabin.isnull() AND Sex=='female'
- #  37:  Embarked=='S' AND Sex=='female'
+        self.task = ps.SubgroupDiscoveryTask(
+            data,
+            ps.FITarget(),
+            searchSpace,
+            result_set_size=10,
+            depth=2,
+            qf=ps.AreaQF(),
+        )
+
+
+#  156: True
+#  125: Cabin.isnull()
+#  110: Embarked=='S'
+#  100: Sex=='male'
+#  89:  Cabin.isnull() AND Embarked=='S'
+#  82:  Cabin.isnull() AND Sex=='male'
+#  73:  Embarked=='S' AND Sex=='male'
+#  60:  Cabin.isnull() AND Embarked=='S' AND Sex=='male'
+#  56:  Sex=='female'
+#  43:  Cabin.isnull() AND Sex=='female'
+#  37:  Embarked=='S' AND Sex=='female'
 
-if __name__ == '__main__':
-    #unittest.main()
+if __name__ == "__main__":
+    # unittest.main()
     suite1 = unittest.TestLoader().loadTestsFromTestCase(TestCountQF)
     suite2 = unittest.TestLoader().loadTestsFromTestCase(TestAreaQF)
-    #suite3 = unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms3)
-    complete_suite = unittest.TestSuite([suite1, suite2])
+    suite3 = unittest.TestLoader().loadTestsFromTestCase(TestFITarget)
+    # suite3 = unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms3)
+    complete_suite = unittest.TestSuite([suite1, suite2, suite3])
     unittest.TextTestRunner(verbosity=2).run(complete_suite)
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_generalisation_aware.py` & `pysubgroup-0.7.6/tests/test_generalisation_aware.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,137 +1,176 @@
 import unittest
-from collections import namedtuple
+
 import numpy as np
 import pandas as pd
+from algorithms_testing import TestAlgorithmsBase
+
 import pysubgroup as ps
-from pysubgroup.tests.DataSets import get_credit_data
-from pysubgroup.tests.algorithms_testing import TestAlgorithmsBase
+from pysubgroup.datasets import get_credit_data
+
 
 class TestGeneralisationAwareQf(unittest.TestCase):
     def setUp(self):
         self.qf = ps.CountQF()
         self.ga_qf = ps.GeneralizationAwareQF(self.qf)
         self.prepare_df()
-    
 
     def prepare_df(self):
         A = np.array([0, 0, 1, 1, 0, 0, 1, 1, 1, 1], dtype=bool)
         self.A1 = ps.EqualitySelector("columnA", True)
         self.A0 = ps.EqualitySelector("columnA", False)
 
         B = np.array(["A", "B", "C", "C", "B", "A", "D", "A", "A", "A"])
         self.BA = ps.EqualitySelector("columnB", "A")
         self.BC = ps.EqualitySelector("columnB", "C")
-        self.df = pd.DataFrame.from_dict({'columnA': A, 'columnB':B, 'columnC': np.array([[0, 1] for _ in range(5)]).flatten()})
-
+        self.BD = ps.EqualitySelector("columnB", "D")
+        self.df = pd.DataFrame.from_dict(
+            {
+                "columnA": A,
+                "columnB": B,
+                "columnC": np.array([[0, 1] for _ in range(5)]).flatten(),
+            }
+        )
 
     def test_CountTarget1(self):
         df = self.df
         target = ps.FITarget()
         self.ga_qf.calculate_constant_statistics(df, target)
 
         ga_score = self.ga_qf.evaluate(ps.Conjunction([self.A1]), target, df)
 
         A1_score = self.qf.evaluate(ps.Conjunction([self.A1]), target, df)
         zero_score = self.qf.evaluate(ps.Conjunction([]), target, df)
 
-        self.assertEqual(ga_score, A1_score-zero_score)
+        self.assertEqual(ga_score, A1_score - zero_score)
 
         ga2_score = self.ga_qf.evaluate(ps.Conjunction([self.A1]), target, df)
 
         self.assertEqual(ga2_score, ga_score)
 
-
     def test_CountTarget2(self):
         df = self.df
         target = ps.FITarget()
         self.ga_qf.calculate_constant_statistics(df, None)
 
-        ga_score = self.ga_qf.evaluate(ps.Conjunction([self.A1, self.BA]), target,  df)
+        ga_score = self.ga_qf.evaluate(ps.Conjunction([self.A1, self.BA]), target, df)
 
         A_B_score = self.qf.evaluate(ps.Conjunction([self.A1, self.BA]), target, df)
         zero_score = self.qf.evaluate(ps.Conjunction([]), target, df)
 
-        self.assertEqual(ga_score, A_B_score-zero_score)
-
+        self.assertEqual(ga_score, A_B_score - zero_score)
 
 
 class TestGeneralisationAware_StandardQf(unittest.TestCase):
     def setUp(self):
         self.df = None
         self.A1 = None
         self.BA = None
+        self.A0 = None
+        self.BD = None
         TestGeneralisationAwareQf.prepare_df(self)
         self.ga_qf = ps.GeneralizationAware_StandardQF(0)
 
     def test_simple(self):
-        target = ps.BinaryTarget('columnC', 1)
+        target = ps.BinaryTarget("columnC", 1)
         qf = ps.StandardQF(0)
         qf.calculate_constant_statistics(self.df, target)
 
         self.ga_qf.calculate_constant_statistics(self.df, target)
 
-        #print(qf.calculate_statistics(self.A1, self.df))
-        #print(qf.calculate_statistics(self.BA, self.df))
-        #print(qf.calculate_statistics(ps.Conjunction([self.A1, self.BA]), self.df))
-        #print(qf.calculate_statistics(slice(None), self.df))
-        ga_stat = self.ga_qf.calculate_statistics(ps.Conjunction([self.A1, self.BA]), target, self.df)
+        # print(qf.calculate_statistics(self.A1, self.df))
+        # print(qf.calculate_statistics(self.BA, self.df))
+        # print(qf.calculate_statistics(ps.Conjunction([self.A1, self.BA]), self.df))
+        # print(qf.calculate_statistics(slice(None), self.df))
+        ga_stat = self.ga_qf.calculate_statistics(
+            ps.Conjunction([self.A1, self.BA]), target, self.df
+        )
 
         self.assertEqual(ga_stat.subgroup_stats, ps.SimplePositivesQF.tpl(3, 2))
         self.assertEqual(ga_stat.generalisation_stats, ps.SimplePositivesQF.tpl(5, 3))
-        # Ensure cache works properly
-        self.assertEqual(ga_stat, self.ga_qf.calculate_statistics(ps.Conjunction([self.A1, self.BA]), target, self.df))
 
-        ga_score = self.ga_qf.evaluate(ps.Conjunction([self.A1, self.BA]), target, self.df)
-        ga_score2 = self.ga_qf.evaluate(ps.Conjunction([self.A1, self.BA]), target, self.df)
+        # Ensure cache works properly
+        self.assertEqual(
+            ga_stat,
+            self.ga_qf.calculate_statistics(
+                ps.Conjunction([self.A1, self.BA]), target, self.df
+            ),
+        )
+
+        ga_score = self.ga_qf.evaluate(
+            ps.Conjunction([self.A1, self.BA]), target, self.df
+        )
+        ga_score2 = self.ga_qf.evaluate(
+            ps.Conjunction([self.A1, self.BA]), target, self.df
+        )
+        ga_score3 = self.ga_qf.evaluate(
+            ps.Conjunction([self.A0, self.BD]), target, self.df
+        )
 
         self.assertEqual(ga_score, ga_score2)
         self.assertAlmostEqual(ga_score, 0.06666666666666)
+        self.assertTrue(np.isnan(ga_score3))
 
 
 class TestAlgorithms(TestAlgorithmsBase, unittest.TestCase):
     # TODO properly specify desired result
     def setUp(self):
         NS_checking = ps.EqualitySelector("checking_status", b"<0")
         NS_foreign_worker = ps.EqualitySelector("foreign_worker", b"yes")
         NS_other_parties = ps.EqualitySelector("other_parties", b"none")
         NS_savings_status = ps.EqualitySelector("savings_status", b"<100")
         NS_job = ps.EqualitySelector("job", b"skilled")
-        self.result = [ps.Conjunction([NS_checking, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking]),
-                       ps.Conjunction([NS_checking, NS_other_parties, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_other_parties]),
-                       ps.Conjunction([NS_checking, NS_savings_status, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_savings_status]),
-                       ps.Conjunction([NS_checking, NS_savings_status, NS_other_parties, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_job, NS_foreign_worker]),
-                       ps.Conjunction([NS_checking, NS_savings_status, NS_other_parties]),
-                       ps.Conjunction([NS_checking, NS_job]),
-                       ]
-        self.qualities = [0.055299999999999995,
-                          0.05280000000000001,
-                          0.052300000000000006,
-                          0.05059999999999999,
-                          0.04959999999999999,
-                          0.048299999999999996,
-                          0.04660000000000001,
-                          0.04550000000000001,
-                          0.0452,
-                          0.044399999999999995]
+        self.result = [
+            ps.Conjunction([NS_checking, NS_foreign_worker]),
+            ps.Conjunction([NS_checking]),
+            ps.Conjunction([NS_checking, NS_other_parties, NS_foreign_worker]),
+            ps.Conjunction([NS_checking, NS_other_parties]),
+            ps.Conjunction([NS_checking, NS_savings_status, NS_foreign_worker]),
+            ps.Conjunction([NS_checking, NS_savings_status]),
+            ps.Conjunction(
+                [NS_checking, NS_savings_status, NS_other_parties, NS_foreign_worker]
+            ),
+            ps.Conjunction([NS_checking, NS_job, NS_foreign_worker]),
+            ps.Conjunction([NS_checking, NS_savings_status, NS_other_parties]),
+            ps.Conjunction([NS_checking, NS_job]),
+        ]
+        self.qualities = [
+            0.055299999999999995,
+            0.05280000000000001,
+            0.052300000000000006,
+            0.05059999999999999,
+            0.04959999999999999,
+            0.048299999999999996,
+            0.04660000000000001,
+            0.04550000000000001,
+            0.0452,
+            0.044399999999999995,
+        ]
         data = get_credit_data()
-        target = ps.BinaryTarget('class', b'bad')
-        searchSpace = ps.create_nominal_selectors(data, ignore=['class'])
-        self.task = ps.SubgroupDiscoveryTask(data, target, searchSpace, result_set_size=10, depth=3, qf=ps.GeneralizationAwareQF(ps.StandardQF(1.0)))
+        target = ps.BinaryTarget("class", b"bad")
+        searchSpace = ps.create_nominal_selectors(data, ignore=["class"])
+        self.task = ps.SubgroupDiscoveryTask(
+            data,
+            target,
+            searchSpace,
+            result_set_size=10,
+            depth=3,
+            qf=ps.GeneralizationAwareQF(ps.StandardQF(1.0)),
+        )
 
     @unittest.skip
     def test_GA_SimpleDFS(self):
-        self.runAlgorithm(ps.SimpleDFS(), "SimpleDFS", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.SimpleDFS(), "SimpleDFS", self.result, self.qualities, self.task
+        )
 
     @unittest.skip
     def test_StandardQF_GA_SimpleDFS(self):
         self.task.qf = ps.GeneralizationAware_StandardQF(0.5)
-        self.runAlgorithm(ps.SimpleDFS(), "Standard_SimpleDFS", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.SimpleDFS(), "Standard_SimpleDFS", self.result, self.qualities, self.task
+        )
         print(self.task.qf.cache)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_generalisations.py` & `pysubgroup-0.7.6/tests/test_generalisations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,88 +1,114 @@
 import unittest
+
+from algorithms_testing import TestAlgorithmsBase
+
 import pysubgroup as ps
-from pysubgroup.tests.DataSets import get_credit_data
-from pysubgroup.tests.algorithms_testing import TestAlgorithmsBase
+from pysubgroup.datasets import get_credit_data
 
 skip_long_running = True
 
+
 class BooleanTargetBase(TestAlgorithmsBase):
     # pylint: disable=no-member
     @unittest.skipIf(skip_long_running, "as skip_long_running flag is True")
     def test_GeneralisingBFS(self):
-        self.runAlgorithm(ps.GeneralisingBFS(), "GeneralisingBFS", self.result, self.qualities, self.task)
+        self.runAlgorithm(
+            ps.GeneralisingBFS(),
+            "GeneralisingBFS",
+            self.result,
+            self.qualities,
+            self.task,
+        )
 
     def test_GeneralisingApriori(self):
-        algorithm = ps.Apriori(combination_name='Disjunction')
-        algorithm.optimistic_estimate_name = 'optimistic_generalisation'
-        self.runAlgorithm(algorithm, "GeneralisingApriori", self.result, self.qualities, self.task)
+        algorithm = ps.Apriori(combination_name="Disjunction")
+        algorithm.optimistic_estimate_name = "optimistic_generalisation"
+        self.runAlgorithm(
+            algorithm, "GeneralisingApriori", self.result, self.qualities, self.task
+        )
+
     # pylint: enable=no-member
 
+
 class TestAlgorithms(BooleanTargetBase, unittest.TestCase):
     def setUp(self):
         NS_checking = ps.EqualitySelector("checking_status", b"<0")
         NS_checking2 = ps.EqualitySelector("checking_status", b"0<=X<200")
         NS_other_parties = ps.EqualitySelector("other_parties", b"co applicant")
-        NS_other = ps.EqualitySelector("purpose", b'other')
-        NS_repairs = ps.EqualitySelector("purpose", b'repairs')
-        NS_purpose = ps.EqualitySelector("purpose", b'business')
+        NS_other = ps.EqualitySelector("purpose", b"other")
+        NS_repairs = ps.EqualitySelector("purpose", b"repairs")
+        NS_purpose = ps.EqualitySelector("purpose", b"business")
 
         NS_history = ps.EqualitySelector("credit_history", b"no credits/all paid")
         NS_history2 = ps.EqualitySelector("credit_history", b"all paid")
         NS_empl = ps.EqualitySelector("employment", b"unemployed")
         NS_job = ps.EqualitySelector("job", b"unemp/unskilled non res")
         NS_bank = ps.EqualitySelector("other_payment_plans", b"bank")
-        self.result = [ps.Disjunction([NS_checking, NS_checking2, NS_bank]),
-                       ps.Disjunction([NS_checking, NS_checking2, NS_history]),
-                       ps.Disjunction([NS_checking, NS_checking2]),
-                       ps.Disjunction([NS_checking, NS_checking2, NS_other]),
-                       ps.Disjunction([NS_checking, NS_checking2, NS_repairs]),
-                       ps.Disjunction([NS_checking, NS_checking2, NS_empl]),
-                       ps.Disjunction([NS_checking, NS_checking2, NS_other_parties]),
-                       ps.Disjunction([NS_checking, NS_checking2, NS_history2]),
-                       ps.Disjunction([NS_checking, NS_checking2, NS_purpose]),
-                       ps.Disjunction([NS_checking, NS_checking2, NS_job]),
-                       ]
-        self.qualities = [0.0779,
-                          0.07740000000000002,
-                          0.0771,
-                          0.07680000000000001,
-                          0.07670000000000002,
-                          0.0767,
-                          0.07660000000000003,
-                          0.07650000000000003,
-                          0.07650000000000001,
-                          0.07600000000000001]
+        self.result = [
+            ps.Disjunction([NS_checking, NS_checking2, NS_bank]),
+            ps.Disjunction([NS_checking, NS_checking2, NS_history]),
+            ps.Disjunction([NS_checking, NS_checking2]),
+            ps.Disjunction([NS_checking, NS_checking2, NS_other]),
+            ps.Disjunction([NS_checking, NS_checking2, NS_repairs]),
+            ps.Disjunction([NS_checking, NS_checking2, NS_empl]),
+            ps.Disjunction([NS_checking, NS_checking2, NS_other_parties]),
+            ps.Disjunction([NS_checking, NS_checking2, NS_history2]),
+            ps.Disjunction([NS_checking, NS_checking2, NS_purpose]),
+            ps.Disjunction([NS_checking, NS_checking2, NS_job]),
+        ]
+        self.qualities = [
+            0.0779,
+            0.07740000000000002,
+            0.0771,
+            0.07680000000000001,
+            0.07670000000000002,
+            0.0767,
+            0.07660000000000003,
+            0.07650000000000003,
+            0.07650000000000001,
+            0.07600000000000001,
+        ]
         data = get_credit_data()
-        target = ps.BinaryTarget('class', b'bad')
-        searchSpace = ps.create_nominal_selectors(data, ignore=['class'])
-        self.task = ps.SubgroupDiscoveryTask(data, target, searchSpace, result_set_size=10, depth=3, qf=ps.StandardQF(1.0))
+        target = ps.BinaryTarget("class", b"bad")
+        searchSpace = ps.create_nominal_selectors(data, ignore=["class"])
+        self.task = ps.SubgroupDiscoveryTask(
+            data,
+            target,
+            searchSpace,
+            result_set_size=10,
+            depth=3,
+            qf=ps.StandardQF(1.0),
+        )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     suite1 = unittest.TestLoader().loadTestsFromTestCase(TestAlgorithms)
     complete_suite = unittest.TestSuite([suite1])
     unittest.TextTestRunner(verbosity=2).run(complete_suite)
-#depth = 5, a=1.0
+
+# flake8: noqa: E501
+
+# depth = 5, a=1.0
 #   0.07800000000000001: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR other_parties=='b'co applicant'' OR other_payment_plans=='b'bank''
 #   0.07800000000000001: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR other_parties=='b'co applicant'' OR other_payment_plans=='b'bank'' OR purpose=='b'other''
 #   0.07790000000000001: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR credit_history=='b'no credits/all paid'' OR other_parties=='b'co applicant'' OR other_payment_plans=='b'bank''
 #   0.0779:              checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR other_payment_plans=='b'bank''
 #   0.0779:              checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR other_payment_plans=='b'bank'' OR purpose=='b'other''
 #   0.07780000000000002: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR credit_history=='b'no credits/all paid'' OR other_payment_plans=='b'bank''
 #   0.07780000000000002: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR credit_history=='b'no credits/all paid'' OR other_payment_plans=='b'bank'' OR purpose=='b'other''
 #   0.07770000000000002: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR credit_history=='b'no credits/all paid'' OR other_payment_plans=='b'bank'' OR purpose=='b'repairs''
 #   0.0776:              checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR other_parties=='b'co applicant'' OR other_payment_plans=='b'bank'' OR purpose=='b'repairs''
 #   0.07750000000000001: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR other_payment_plans=='b'bank'' OR purpose=='b'repairs''
 #   0.07750000000000001: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR credit_history=='b'all paid'' OR other_parties=='b'co applicant'' OR other_payment_plans=='b'bank''
 
-#depth = 3, a=1.0
+# depth = 3, a=1.0
 #  0.0779:              checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR other_payment_plans=='b'bank''
 #  0.07740000000000002: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR credit_history=='b'no credits/all paid''
 #  0.0771:              checking_status=='b'0<=X<200'' OR checking_status=='b'<0''
 #  0.07680000000000001: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR purpose=='b'other''
 #  0.07670000000000002: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR purpose=='b'repairs''
 #  0.0767:              checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR employment=='b'unemployed''
 #  0.07660000000000003: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR other_parties=='b'co applicant''
 #  0.07650000000000003: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR credit_history=='b'all paid''
 #  0.07650000000000001: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR purpose=='b'business''
-#  0.07600000000000001: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR job=='b'unemp/unskilled non res''
+#  0.07600000000000001: checking_status=='b'0<=X<200'' OR checking_status=='b'<0'' OR job=='b'unemp/unskilled non res''
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_qf_input.py` & `pysubgroup-0.7.6/tests/test_qf_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import unittest
+
 import numpy as np
+
 import pysubgroup as ps
-from pysubgroup.tests.DataSets import get_credit_data
+from pysubgroup.datasets import get_credit_data
+
 
 class TestQFInputs(unittest.TestCase):
     def setUp(self):
         self.data = get_credit_data()
 
     def test_get_cover_array_and_size(self):
-        sel = ps.EqualitySelector('checking_status', b'no checking')
+        sel = ps.EqualitySelector("checking_status", b"no checking")
         _, size = ps.get_cover_array_and_size(sel, None, self.data)
         self.assertEqual(size, 394)
         _, size = ps.get_cover_array_and_size(slice(None), len(self.data), None)
         self.assertEqual(size, len(self.data))
         _, size = ps.get_cover_array_and_size(slice(0, 10), len(self.data))
         self.assertEqual(size, 10)
         _, size = ps.get_cover_array_and_size(np.array([1, 3, 5, 7, 11], dtype=int))
         self.assertEqual(size, 5)
 
-# TODO Need to test other qf as well
-#    def test_AreaQf(self):
-#        pass
+    # TODO Need to test other qf as well
+    #    def test_AreaQf(self):
+    #        pass
 
     def test_CountQf(self):
         target = ps.FITarget()
-        #task = ps.SubgroupDiscoveryTask(self.data, ps.FITarget(), None, None)
+        # task = ps.SubgroupDiscoveryTask(self.data, ps.FITarget(), None, None)
 
         qf = ps.CountQF()
         qf.calculate_constant_statistics(self.data, target)
-        sel = ps.EqualitySelector('checking_status', b'no checking')
+        sel = ps.EqualitySelector("checking_status", b"no checking")
         print(self.data.columns)
         print(self.data.checking_status.value_counts())
         size = qf.evaluate(sel, target, self.data)
         self.assertEqual(size, 394)
         size = qf.evaluate(slice(None), target, self.data)
         self.assertEqual(size, len(self.data))
         size = qf.evaluate(slice(0, 10), target, self.data)
         self.assertEqual(size, 10)
         size = qf.evaluate(np.array([1, 3, 5, 7, 11], dtype=int), target, self.data)
         self.assertEqual(size, 5)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_subgroup.py` & `pysubgroup-0.7.6/tests/test_subgroup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import unittest
+
 import numpy as np
 import pandas as pd
+
 import pysubgroup as ps
 
 
 class TestRelationsMethods(unittest.TestCase):
     def test_EqualitySelector_ordering(self):
         A1 = ps.EqualitySelector("A", 1)
         A1_clone = ps.EqualitySelector("A", 1)
@@ -22,18 +24,18 @@
 
         C1 = ps.EqualitySelector("checking_status", b"<0")
         C2 = ps.EqualitySelector("checking_status", b"<0")
 
         self.assertTrue(C1 == C2)
         self.assertTrue(hash(C1) == hash(C2))
 
-        l = [A1, A2, B1]
-        self.assertEqual(l.index(A1), 0)
-        self.assertEqual(l.index(A2), 1)
-        self.assertEqual(l.index(B1), 2)
+        selectors = [A1, A2, B1]
+        self.assertEqual(selectors.index(A1), 0)
+        self.assertEqual(selectors.index(A2), 1)
+        self.assertEqual(selectors.index(B1), 2)
 
     def test_IntervalSelector_ordering(self):
         S1 = ps.IntervalSelector("A", 1.2345, 2.0)
         S1_clone = ps.IntervalSelector("A", 1.2345, 2.0)
         S1_clone = ps.IntervalSelector("A", 1.2345, 2.0)
         S2 = ps.IntervalSelector("A", 1.2345, 3.0)
         S3 = ps.IntervalSelector("A", 1.2346, 3.0)
@@ -115,22 +117,27 @@
         I1 = ps.IntervalSelector("test", 10, 15)
         self.assertEqual(str(I1), "test: [10:15[")
         self.assertEqual(repr(I1), "test: [10:15[")
 
         I2 = ps.IntervalSelector("test2", np.sqrt(2), np.sqrt(3))
         self.assertEqual(str(I2), "test2: [1.41:1.73[")
         self.assertEqual(repr(I2), "test2: [1.4142135623730951:1.7320508075688772[")
-        #self.assertEqual(repr(NegC), "(not CCC==True)")
+        # self.assertEqual(repr(NegC), "(not CCC==True)")
 
     def test_create_selectors_with_nan(self):
-        df = pd.DataFrame.from_dict({'A' : np.array([np.nan, np.nan, np.nan]), 'B' : np.array([10, np.nan, np.nan])})
+        df = pd.DataFrame.from_dict(
+            {
+                "A": np.array([np.nan, np.nan, np.nan]),
+                "B": np.array([10, np.nan, np.nan]),
+            }
+        )
         result = ps.create_selectors(df)
-        A_null = ps.EqualitySelector('A', np.nan)
-        B_null = ps.EqualitySelector('B', np.nan)
-        B_10 = ps.EqualitySelector('B', 10.)
+        A_null = ps.EqualitySelector("A", np.nan)
+        B_null = ps.EqualitySelector("B", np.nan)
+        B_10 = ps.EqualitySelector("B", 10.0)
         assert A_null in result
         assert B_null in result
         assert B_10 in result
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `pysubgroup-0.7.3/pysubgroup/tests/test_visualization.py` & `pysubgroup-0.7.6/tests/test_visualization.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import matplotlib.pyplot as plt
+
 import pysubgroup as ps
-from pysubgroup.tests.DataSets import get_titanic_data
+from pysubgroup.datasets import get_titanic_data
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     plt.interactive(False)
 
-
     data = get_titanic_data()
-    target = ps.BinaryTarget('Survived', 0)
-    search_space = ps.create_selectors(data, ignore=['Survived'])
-    task = ps.SubgroupDiscoveryTask(data, target, search_space,
-                                    result_set_size=5, depth=2,
-                                    qf=ps.ChiSquaredQF())
+    target = ps.BinaryTarget("Survived", 0)
+    search_space = ps.create_selectors(data, ignore=["Survived"])
+    task = ps.SubgroupDiscoveryTask(
+        data, target, search_space, result_set_size=5, depth=2, qf=ps.ChiSquaredQF()
+    )
 
     result = ps.SimpleDFS().execute(task)
 
-    #dfs = ps.results_as_df(data, result)
-    #fig = ps.plot_roc(dfs, data, ps.ChiSquaredQF())
-    #fig.show()
-    #plt.show()
+    # dfs = ps.results_as_df(data, result)
+    # fig = ps.plot_roc(dfs, data, ps.ChiSquaredQF())
+    # fig.show()
+    # plt.show()
```

### Comparing `pysubgroup-0.7.3/pysubgroup/utils.py` & `pysubgroup-0.7.6/src/pysubgroup/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-'''
+"""
 Created on 02.05.2016
 
 @author: lemmerfn
-'''
+"""
 import itertools
-from functools import partial
-from heapq import heappush, heappop
 from collections.abc import Iterable
+from functools import partial
+from heapq import heappop, heappush
 
 import numpy as np
-import pandas as pd
+
 import pysubgroup as ps
 
 
-def add_if_required(result, sg, quality, task, check_for_duplicates=False, statistics=None):
+def add_if_required(
+    result, sg, quality, task, check_for_duplicates=False, statistics=None
+):
     if quality > task.min_quality:
         if not ps.constraints_satisfied(task.constraints, sg, statistics, task.data):
             return
         if check_for_duplicates and (quality, sg, statistics) in result:
             return
         if len(result) < task.result_set_size:
             heappush(result, (quality, sg, statistics))
@@ -29,16 +31,25 @@
 def minimum_required_quality(result, task):
     if len(result) < task.result_set_size:
         return task.min_quality
     else:
         return result[0][0]
 
 
+def prepare_subgroup_discovery_result(result, task):
+    result_filtered = [tpl for tpl in result if tpl[0] > task.min_quality]
+    result_filtered.sort(key=lambda x: x[0], reverse=True)
+    result_filtered = result_filtered[: task.result_set_size]
+    return result_filtered
+
+
 # Returns the cutpoints for discretization
-def equal_frequency_discretization(data, attribute_name, nbins=5, weighting_attribute=None):
+def equal_frequency_discretization(
+    data, attribute_name, nbins=5, weighting_attribute=None
+):
     cutpoints = []
     if weighting_attribute is None:
         cleaned_data = data[attribute_name]
         cleaned_data = cleaned_data[~np.isnan(cleaned_data)]
         sorted_data = sorted(cleaned_data)
         number_instances = len(sorted_data)
         for i in range(1, nbins):
@@ -71,82 +82,86 @@
                     if remaining_weights < 1.5 * (bin_size):
                         break
                     sum_of_weights = 0
     return cutpoints
 
 
 def conditional_invert(val, invert):
-    return - 2 * (invert - 0.5) * val
+    return -2 * (invert - 0.5) * val
 
 
 def results_df_autoround(df):
-    return df.round({
-        'quality': 3,
-        'size_sg': 0,
-        'size_dataset': 0,
-        'positives_sg': 0,
-        'positives_dataset': 0,
-        'size_complement': 0,
-        'relative_size_sg': 3,
-        'relative_size_complement': 3,
-        'coverage_sg': 3,
-        'coverage_complement': 3,
-        'target_share_sg': 3,
-        'target_share_complement': 3,
-        'target_share_dataset': 3,
-        'lift': 3,
-
-        'size_sg_weighted': 1,
-        'size_dataset_weighted': 1,
-        'positives_sg_weighted': 1,
-        'positives_dataset_weighted': 1,
-        'size_complement_weighted': 1,
-        'relative_size_sg_weighted': 3,
-        'relative_size_complement_weighted': 3,
-        'coverage_sg_weighted': 3,
-        'coverage_complement_weighted': 3,
-        'target_share_sg_weighted': 3,
-        'target_share_complement_weighted': 3,
-        'target_share_dataset_weighted': 3,
-        'lift_weighted': 3})
+    return df.round(
+        {
+            "quality": 3,
+            "size_sg": 0,
+            "size_dataset": 0,
+            "positives_sg": 0,
+            "positives_dataset": 0,
+            "size_complement": 0,
+            "relative_size_sg": 3,
+            "relative_size_complement": 3,
+            "coverage_sg": 3,
+            "coverage_complement": 3,
+            "target_share_sg": 3,
+            "target_share_complement": 3,
+            "target_share_dataset": 3,
+            "lift": 3,
+            "size_sg_weighted": 1,
+            "size_dataset_weighted": 1,
+            "positives_sg_weighted": 1,
+            "positives_dataset_weighted": 1,
+            "size_complement_weighted": 1,
+            "relative_size_sg_weighted": 3,
+            "relative_size_complement_weighted": 3,
+            "coverage_sg_weighted": 3,
+            "coverage_complement_weighted": 3,
+            "target_share_sg_weighted": 3,
+            "target_share_complement_weighted": 3,
+            "target_share_dataset_weighted": 3,
+            "lift_weighted": 3,
+        }
+    )
 
 
 def perc_formatter(x):
     return "{0:.1f}%".format(x * 100)
 
 
 def float_formatter(x, digits=2):
     return ("{0:." + str(digits) + "f}").format(x)
 
 
 def is_categorical_attribute(data, attribute_name):
-    return attribute_name in data.select_dtypes(exclude=['number']).columns.values
+    return attribute_name in data.select_dtypes(exclude=["number"]).columns.values
 
 
 def is_numerical_attribute(data, attribute_name):
-    return attribute_name in data.select_dtypes(include=['number']).columns.values
+    return attribute_name in data.select_dtypes(include=["number"]).columns.values
 
 
 def remove_selectors_with_attributes(selector_list, attribute_list):
     return [x for x in selector_list if x.attributeName not in attribute_list]
 
 
-def effective_sample_size(weights):
-    return sum(weights) ** 2 / sum(weights ** 2)
+def derive_effective_sample_size(weights):
+    return sum(weights) ** 2 / sum(weights**2)
 
 
 # from https://docs.python.org/3/library/itertools.html#recipes
 def powerset(iterable, max_length=None):
     "powerset([1,2,3]) --> () (1,) (2,) (3,) (1,2) (1,3) (2,3) (1,2,3)"
     s = list(iterable)
     if max_length is None:
         max_length = len(s)
     if max_length < len(s):
         max_length = len(s)
-    return itertools.chain.from_iterable(itertools.combinations(s, r) for r in range(max_length))
+    return itertools.chain.from_iterable(
+        itertools.combinations(s, r) for r in range(max_length)
+    )
 
 
 def overlap(sg, another_sg, data):
     cover_sg = sg.covers(data)
     cover_another_sg = another_sg.covers(data)
     union = np.logical_or(cover_sg, cover_another_sg)
     intercept = np.logical_and(cover_sg, cover_another_sg)
@@ -194,66 +209,92 @@
         else:
             result.append(list_1[i])
             j += 1
             i += 1
     return result
 
 
+class BaseTarget:
+    def all_statistics_present(self, cached_statistics):
+        if isinstance(cached_statistics, dict) and all(
+            expected_value in cached_statistics
+            for expected_value in self.__class__.statistic_types
+        ):  # pylint: disable=no-member
+            return True
+        return False
+
+
 class SubgroupDiscoveryResult:
     def __init__(self, results, task):
         self.task = task
         self.results = results
         assert isinstance(results, Iterable)
 
-    def to_descriptions(self):
-        return [(qual, sgd) for qual, sgd, stats in self.results]
+    def to_descriptions(self, include_stats=False):
+        if include_stats:
+            return list(self.results)
+        else:
+            return [(qual, sgd) for qual, sgd, stats in self.results]
 
-    def to_table(self, statistics_to_show=None, print_header=True, include_target=False):
+    def to_table(
+        self, statistics_to_show=None, print_header=True, include_target=False
+    ):
         if statistics_to_show is None:
             statistics_to_show = type(self.task.target).statistic_types
         table = []
         if print_header:
             row = ["quality", "subgroup"]
+            if include_target:
+                row.append("target")
             for stat in statistics_to_show:
                 row.append(stat)
             table.append(row)
-        for (q, sg, stats) in self.results:
+        for q, sg, stats in self.results:
             stats = self.task.target.calculate_statistics(sg, self.task.data, stats)
-            row = [str(q), str(sg)]
+            row = [q, sg]
             if include_target:
-                row.append(str(self.task.target))
+                row.append(self.task.target)
             for stat in statistics_to_show:
-                row.append(str(stats[stat]))
+                row.append(stats[stat])
             table.append(row)
         return table
 
-    def to_dataframe(self, statistics_to_show=None, autoround=False, include_target=False):
+    def to_dataframe(
+        self, statistics_to_show=None, autoround=False, include_target=False
+    ):
+        import pandas as pd  # pylint: disable=import-outside-toplevel
+
         if statistics_to_show is None:
             statistics_to_show = type(self.task.target).statistic_types
         res = self.to_table(statistics_to_show, True, include_target)
         headers = res.pop(0)
-        df = pd.DataFrame(res, columns=headers, dtype=np.float64)
+        df = pd.DataFrame(res, columns=headers)
         if autoround:
             df = results_df_autoround(df)
         return df
 
     def to_latex(self, statistics_to_show=None):
         if statistics_to_show is None:
             statistics_to_show = type(self.task.target).statistic_types
         df = self.to_dataframe(statistics_to_show)
-        latex = df.to_latex(index=False, col_space=10, formatters={
-            'quality': partial(float_formatter, digits=3),
-            'size_sg': partial(float_formatter, digits=0),
-            'size_dataset': partial(float_formatter, digits=0),
-            'positives_sg': partial(float_formatter, digits=0),
-            'positives_dataset': partial(float_formatter, digits=0),
-            'size_complement': partial(float_formatter, digits=0),
-            'relative_size_sg': perc_formatter,
-            'relative_size_complement': perc_formatter,
-            'coverage_sg': perc_formatter,
-            'coverage_complement': perc_formatter,
-            'target_share_sg': perc_formatter,
-            'target_share_complement': perc_formatter,
-            'target_share_dataset': perc_formatter,
-            'lift': partial(float_formatter, digits=1)})
-        latex = latex.replace(' AND ', r' $\wedge$ ')
+        latex = df.to_latex(
+            index=False,
+            col_space=10,
+            formatters={
+                "quality": partial(float_formatter, digits=3),
+                "size_sg": partial(float_formatter, digits=0),
+                "size_dataset": partial(float_formatter, digits=0),
+                "positives_sg": partial(float_formatter, digits=0),
+                "positives_dataset": partial(float_formatter, digits=0),
+                "size_complement": partial(float_formatter, digits=0),
+                "relative_size_sg": perc_formatter,
+                "relative_size_complement": perc_formatter,
+                "coverage_sg": perc_formatter,
+                "coverage_complement": perc_formatter,
+                "target_share_sg": perc_formatter,
+                "target_share_complement": perc_formatter,
+                "target_share_dataset": perc_formatter,
+                "lift": partial(float_formatter, digits=1),
+            },
+        )
+        latex = latex.replace(" AND ", r" $\wedge$ ")
         return latex
```

### Comparing `pysubgroup-0.7.3/pysubgroup/visualization.py` & `pysubgroup-0.7.6/src/pysubgroup/visualization.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,140 +1,183 @@
 from functools import partial
 
-import pandas as pd
 import numpy as np
-from scipy.cluster.hierarchy import dendrogram, linkage
-from scipy.spatial.distance import squareform
-from matplotlib import pyplot as plt
 
 import pysubgroup as ps
 
 
-def plot_sgbars(result_df, _, ylabel="target share", title="Discovered Subgroups", dynamic_widths=False, _suffix=""):
+def plot_sgbars(
+    result_df,
+    _,
+    ylabel="target share",
+    title="Discovered Subgroups",
+    dynamic_widths=False,
+    _suffix="",
+):
+    from matplotlib import pyplot as plt  # pylint: disable=import-outside-toplevel
+
     shares_sg = result_df["target_share_sg"]
     shares_compl = result_df["target_share_complement"]
     sg_relative_sizes = result_df["relative_size_sg"]
     x = np.arange(len(result_df))
 
     base_width = 0.8
     if dynamic_widths:
         width_sg = 0.02 + base_width * sg_relative_sizes
         width_compl = base_width - width_sg
     else:
         width_sg = base_width / 2
         width_compl = base_width / 2
 
     fig, ax = plt.subplots()
-    rects1 = ax.bar(x, shares_sg, width_sg, align='edge')
-    rects2 = ax.bar(x + width_sg, shares_compl, width_compl, align='edge', color='#61b76f')
+    rects1 = ax.bar(x, shares_sg, width_sg, align="edge")
+    rects2 = ax.bar(
+        x + width_sg, shares_compl, width_compl, align="edge", color="#61b76f"
+    )
 
     ax.set_ylabel(ylabel)
     ax.set_title(title)
     ax.set_xticks(x + base_width / 2)
     ax.set_xticklabels(result_df.index, rotation=90)
 
-    ax.legend((rects1[0], rects2[0]), ('subgroup', 'complement'))
+    ax.legend((rects1[0], rects2[0]), ("subgroup", "complement"))
     fig.set_size_inches(12, len(result_df))
 
     return fig
 
 
 def plot_roc(result_df, data, qf=ps.StandardQF(0.5), levels=40, annotate=False):
+    from matplotlib import pyplot as plt  # pylint: disable=import-outside-toplevel
+
     instances_dataset = len(data)
-    positives_dataset = np.max(result_df['positives_dataset'])
+    positives_dataset = np.max(result_df["positives_dataset"])
     negatives_dataset = instances_dataset - positives_dataset
 
     xlist = np.linspace(0.01, 0.99, 100)
     ylist = np.linspace(0.01, 0.99, 100)
     X, Y = np.meshgrid(xlist, ylist)
-    f = np.vectorize(partial(qf.evaluate, instances_dataset, positives_dataset), otypes=[np.float])
+    f = np.vectorize(
+        partial(qf.evaluate, instances_dataset, positives_dataset), otypes=[np.float]
+    )
     Z = f(X * negatives_dataset + Y * positives_dataset, Y * positives_dataset)
     max_val = np.max([np.max(Z), -np.min(Z)])
 
     fig, ax = plt.subplots()
     cm = plt.cm.get_cmap("bwr")
 
     plt.contourf(X, Y, Z, levels, cmap=cm, vmin=-max_val, vmax=max_val)
 
     for i, sg in result_df.iterrows():
-        rel_positives_sg = sg['positives_sg'] / positives_dataset
-        rel_negatives_sg = (sg['size_sg'] - sg['positives_sg']) / negatives_dataset
-        ax.plot(rel_negatives_sg, rel_positives_sg, 'ro', color='black')
+        rel_positives_sg = sg["positives_sg"] / positives_dataset
+        rel_negatives_sg = (sg["size_sg"] - sg["positives_sg"]) / negatives_dataset
+        ax.plot(rel_negatives_sg, rel_positives_sg, "ro", color="black")
         if annotate:
             label_margin = 0.01
-            ax.annotate(str(i), (rel_negatives_sg + label_margin, rel_positives_sg + label_margin))
+            ax.annotate(
+                str(i),
+                (rel_negatives_sg + label_margin, rel_positives_sg + label_margin),
+            )
 
     # plt.colorbar(cp)
-    plt.title('Discovered subgroups')
-    plt.xlabel('False Positive Rate')
-    plt.ylabel('True Positive Rate')
+    plt.title("Discovered subgroups")
+    plt.xlabel("False Positive Rate")
+    plt.ylabel("True Positive Rate")
 
     return fig
 
 
 def plot_npspace(result_df, data, annotate=True, fixed_limits=False):
+    from matplotlib import pyplot as plt  # pylint: disable=import-outside-toplevel
 
     fig, ax = plt.subplots()
 
     for i, sg in result_df.iterrows():
-        target_share_sg = sg['target_share_sg']
-        size_sg = sg['size_sg']
-        ax.plot(size_sg, target_share_sg, 'ro', color='black')
+        target_share_sg = sg["target_share_sg"]
+        size_sg = sg["size_sg"]
+        ax.plot(size_sg, target_share_sg, "ro", color="black")
         if annotate:
             ax.annotate(str(i), (size_sg + 5, target_share_sg + 0.001))
 
     if fixed_limits:
         plt.xlim((0, len(data)))
         plt.ylim((0, 1))
 
-    plt.title('Discovered subgroups')
-    plt.xlabel('Size of Subgroup')
-    plt.ylabel('Target Share Subgroup')
+    plt.title("Discovered subgroups")
+    plt.xlabel("Size of Subgroup")
+    plt.ylabel("Target Share Subgroup")
 
     return fig
 
 
 def plot_distribution_numeric(sg, data, bins):
+    from matplotlib import pyplot as plt  # pylint: disable=import-outside-toplevel
+
     fig, _ = plt.subplots()
     target_values_sg = data[sg.covers(data)][sg.target.get_attributes()].values
     target_values_data = data[sg.target.get_attributes()].values
-    plt.hist(target_values_sg, bins, alpha=0.5, label=str(sg.subgroup_description), density=True)
+    plt.hist(
+        target_values_sg,
+        bins,
+        alpha=0.5,
+        label=str(sg.subgroup_description),
+        density=True,
+    )
     plt.hist(target_values_data, bins, alpha=0.5, label="Overall Data", density=True)
-    plt.legend(loc='upper right')
+    plt.legend(loc="upper right")
     return fig
 
 
 def compare_distributions_numeric(sgs, data, bins):
+    from matplotlib import pyplot as plt  # pylint: disable=import-outside-toplevel
+
     fig, _ = plt.subplots()
     for sg in sgs:
         target_values_sg = data[sg.covers(data)][sg.target.get_attributes()].values
-        plt.hist(target_values_sg, bins, alpha=0.3, label=str(sg.subgroup_description), density=True)
-    plt.legend(loc='upper right')
+        plt.hist(
+            target_values_sg,
+            bins,
+            alpha=0.3,
+            label=str(sg.subgroup_description),
+            density=True,
+        )
+    plt.legend(loc="upper right")
     return fig
 
 
 def similarity_sgs(sgd_results, data, color=True):
+    import pandas as pd  # pylint:disable=import-outside-toplevel
+
     sgs = [x[1] for x in sgd_results]
-    #sgNames = [str(sg.subgroup_description) for sg in sgs]
+    # sgNames = [str(sg.subgroup_description) for sg in sgs]
     dists = [[ps.overlap(sg, sg2, data) for sg2 in sgs] for sg in sgs]
     dist_df = pd.DataFrame(dists)
     if color:
         dist_df = dist_df.style.background_gradient()
     return dist_df
 
 
 def similarity_dendrogram(result, data):
+    from matplotlib import pyplot as plt  # pylint: disable=import-outside-toplevel
+    from scipy.cluster.hierarchy import (  # pylint: disable=import-outside-toplevel
+        dendrogram,
+        linkage,
+    )
+    from scipy.spatial.distance import (
+        squareform,  # pylint: disable=import-outside-toplevel
+    )
+
     fig, _ = plt.subplots()
     dist_df = similarity_sgs(result, data, color=False)
     mat = 1 - dist_df.values
     dists = squareform(mat)
     linkage_matrix = linkage(dists, "single")
     dendrogram(linkage_matrix, labels=dist_df.index)
     return fig
 
+
 def supportSetVisualization(result, in_order=True, drop_empty=True):
     df = result.task.data
     n_items = len(result.task.data)
     n_SGDs = len(result.results)
     covs = np.zeros((n_items, n_SGDs), dtype=bool)
     for i, (_, r, _) in enumerate(result.to_subgroups):
         covs[:, i] = r.covers(df)
@@ -144,10 +187,13 @@
     sort_inds_x = np.argsort(np.sum(covs, axis=1))[::-1]
     img_arr = img_arr[sort_inds_x, :]
     if not in_order:
         sort_inds_y = np.argsort(np.sum(covs, axis=0))
         img_arr = img_arr[:, sort_inds_y]
     if drop_empty:
         keep_entities = np.sum(img_arr, axis=1) > 0
-        print("Discarding {} entities that are not covered".format(n_items - np.count_nonzero(keep_entities)))
+        print(
+            f"Discarding {n_items - np.count_nonzero(keep_entities)} "
+            "entities that are not covered"
+        )
         img_arr = img_arr[keep_entities, :]
     return img_arr.T
```

