# Comparing `tmp/moscot-0.3.1.tar.gz` & `tmp/moscot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moscot-0.3.1.tar", last modified: Sun Jul 30 08:10:08 2023, max compression
+gzip compressed data, was "moscot-0.3.2.tar", last modified: Mon Aug  7 15:36:27 2023, max compression
```

## Comparing `moscot-0.3.1.tar` & `moscot-0.3.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.389801 moscot-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-30 08:08:45.000000 moscot-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-30 08:08:45.000000 moscot-0.3.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-30 08:08:45.000000 moscot-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-30 08:08:45.000000 moscot-0.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-30 08:08:45.000000 moscot-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-30 08:08:45.000000 moscot-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-30 08:10:08.385801 moscot-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-30 08:08:45.000000 moscot-0.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-30 08:08:45.000000 moscot-0.3.1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-30 08:08:45.000000 moscot-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 08:10:08.389801 moscot-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.377802 moscot-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot/backends/ott/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/ott/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/ott/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/ott/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/ott/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/backends/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot/base/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot/base/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25371 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/birth_death.py
--rw-r--r--   0 runner    (1001) docker     (123)    21112 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/compound_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    31320 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/problems/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/base/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/costs/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/costs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/costs/_costs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/costs/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13977 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/plotting/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/plotting/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/cross_modality/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/cross_modality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/cross_modality/_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/cross_modality/_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21399 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/generic/_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/generic/_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/space/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/space/_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/space/_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    25427 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/space/_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/spatiotemporal/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/spatiotemporal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/spatiotemporal/_spatio_temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/problems/time/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22380 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/time/_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    39311 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/problems/time/_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.385801 moscot-0.3.1/src/moscot/utils/_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/allTFs_dmel.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/allTFs_hg38.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/allTFs_mm.txt
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/human_apoptosis.txt
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/human_proliferation.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/mouse_apoptosis.txt
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/_data/mouse_proliferation.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/subset_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-30 08:08:45.000000 moscot-0.3.1/src/moscot/utils/tagged_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 08:10:08.381801 moscot-0.3.1/src/moscot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-30 08:10:08.000000 moscot-0.3.1/src/moscot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-30 08:10:08.000000 moscot-0.3.1/src/moscot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 08:10:08.000000 moscot-0.3.1/src/moscot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-30 08:10:08.000000 moscot-0.3.1/src/moscot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 08:10:08.000000 moscot-0.3.1/src/moscot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.159469 moscot-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-07 15:34:49.000000 moscot-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-07 15:34:49.000000 moscot-0.3.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-07 15:34:49.000000 moscot-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-07 15:34:49.000000 moscot-0.3.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-07 15:34:49.000000 moscot-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-07 15:34:49.000000 moscot-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-08-07 15:36:27.159469 moscot-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-08-07 15:34:49.000000 moscot-0.3.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-07 15:34:49.000000 moscot-0.3.2/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-08-07 15:34:49.000000 moscot-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:36:27.159469 moscot-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.127467 moscot-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.139468 moscot-0.3.2/src/moscot/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.139468 moscot-0.3.2/src/moscot/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.139468 moscot-0.3.2/src/moscot/backends/ott/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/backends/ott/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/backends/ott/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/backends/ott/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/backends/ott/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/backends/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.139468 moscot-0.3.2/src/moscot/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/base/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/base/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.139468 moscot-0.3.2/src/moscot/base/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/base/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/base/problems/_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25371 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/base/problems/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/base/problems/birth_death.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21112 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/base/problems/compound_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/base/problems/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31320 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/base/problems/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/base/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.139468 moscot-0.3.2/src/moscot/costs/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/costs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/costs/_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/costs/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.143468 moscot-0.3.2/src/moscot/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13977 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/plotting/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/plotting/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.143468 moscot-0.3.2/src/moscot/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.147468 moscot-0.3.2/src/moscot/problems/cross_modality/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/cross_modality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/cross_modality/_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/cross_modality/_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.147468 moscot-0.3.2/src/moscot/problems/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21379 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/generic/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/generic/_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.151469 moscot-0.3.2/src/moscot/problems/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/space/_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/space/_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25427 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/space/_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.151469 moscot-0.3.2/src/moscot/problems/spatiotemporal/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/spatiotemporal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/spatiotemporal/_spatio_temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.151469 moscot-0.3.2/src/moscot/problems/time/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/time/_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39311 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/problems/time/_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.155469 moscot-0.3.2/src/moscot/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.155469 moscot-0.3.2/src/moscot/utils/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/utils/_data/allTFs_dmel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/utils/_data/allTFs_hg38.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/utils/_data/allTFs_mm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/utils/_data/human_apoptosis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/utils/_data/human_proliferation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/utils/_data/mouse_apoptosis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/utils/_data/mouse_proliferation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/utils/subset_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-08-07 15:34:49.000000 moscot-0.3.2/src/moscot/utils/tagged_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:36:27.139468 moscot-0.3.2/src/moscot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-08-07 15:36:27.000000 moscot-0.3.2/src/moscot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-08-07 15:36:27.000000 moscot-0.3.2/src/moscot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:36:27.000000 moscot-0.3.2/src/moscot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-07 15:36:27.000000 moscot-0.3.2/src/moscot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 15:36:27.000000 moscot-0.3.2/src/moscot.egg-info/top_level.txt
```

### Comparing `moscot-0.3.1/.gitignore` & `moscot-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/.pre-commit-config.yaml` & `moscot-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/LICENSE` & `moscot-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/PKG-INFO` & `moscot-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moscot
-Version: 0.3.1
+Version: 0.3.2
 Summary: Multi-omic single-cell optimal transport tools
 Author: Dominik Klein, Giovanni Palla, Michal Klein, Zoe Piran, Marius Lange
 Maintainer-email: Dominik Klein <dominik.klein@helmholtz-muenchen.de>, Giovanni Palla <giovanni.palla@helmholtz-muenchen.de>, Michal Klein <michal.klein@helmholtz-muenchen.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Theis Lab
         All rights reserved.
```

### Comparing `moscot-0.3.1/README.rst` & `moscot-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/pyproject.toml` & `moscot-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     "pandas>=2.0.1",
     "networkx>=2.6.3",
     # https://github.com/scverse/scanpy/issues/2411
     "matplotlib>=3.5.0",
     "anndata>=0.9.1",
     "scanpy>=1.9.3",
     "wrapt>=1.13.2",
-    "ott-jax==0.4.0",
+    "docrep>=0.3.2",
+    "ott-jax>=0.4.3",
     "cloudpickle>=2.2.0",
 ]
 
 [project.optional-dependencies]
 spatial = [
     "squidpy>=1.2.3"
 ]
```

### Comparing `moscot-0.3.1/src/moscot/_logging.py` & `moscot-0.3.2/src/moscot/_logging.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/_registry.py` & `moscot-0.3.2/src/moscot/_registry.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/_types.py` & `moscot-0.3.2/src/moscot/_types.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/backends/ott/__init__.py` & `moscot-0.3.2/src/moscot/backends/ott/__init__.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/backends/ott/_utils.py` & `moscot-0.3.2/src/moscot/backends/ott/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
 import jax
 import jax.numpy as jnp
 import scipy.sparse as sp
-from ott.geometry import geometry, pointcloud
+from ott.geometry import epsilon_scheduler, geometry, pointcloud
 from ott.tools import sinkhorn_divergence as sdiv
 
 from moscot._logging import logger
 from moscot._types import ArrayLike, ScaleCost_t
 
 __all__ = ["sinkhorn_divergence"]
 
 
 def sinkhorn_divergence(
     point_cloud_1: ArrayLike,
     point_cloud_2: ArrayLike,
     a: Optional[ArrayLike] = None,
     b: Optional[ArrayLike] = None,
-    epsilon: Optional[float] = 1e-1,
+    epsilon: Union[float, epsilon_scheduler.Epsilon] = 1e-1,
     scale_cost: ScaleCost_t = 1.0,
     **kwargs: Any,
 ) -> float:
     point_cloud_1 = jnp.asarray(point_cloud_1)
     point_cloud_2 = jnp.asarray(point_cloud_2)
     a = None if a is None else jnp.asarray(a)
     b = None if b is None else jnp.asarray(b)
```

### Comparing `moscot-0.3.1/src/moscot/backends/ott/output.py` & `moscot-0.3.2/src/moscot/backends/ott/output.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/backends/ott/solver.py` & `moscot-0.3.2/src/moscot/backends/ott/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self._solver: Optional[OTTSolver_t] = None
         self._problem: Optional[OTTProblem_t] = None
         self._jit = jit
 
     def _create_geometry(
         self,
         x: TaggedArray,
-        epsilon: Optional[Union[float, epsilon_scheduler.Epsilon]] = None,
+        epsilon: Union[float, epsilon_scheduler.Epsilon] = None,
         relative_epsilon: Optional[bool] = None,
         scale_cost: Scale_t = 1.0,
         batch_size: Optional[int] = None,
         **kwargs: Any,
     ) -> geometry.Geometry:
         if x.is_point_cloud:
             cost_fn = x.cost
@@ -160,15 +160,15 @@
 
     def _prepare(
         self,
         xy: Optional[TaggedArray] = None,
         x: Optional[TaggedArray] = None,
         y: Optional[TaggedArray] = None,
         # geometry
-        epsilon: Optional[Union[float, epsilon_scheduler.Epsilon]] = None,
+        epsilon: Union[float, epsilon_scheduler.Epsilon] = None,
         relative_epsilon: Optional[bool] = None,
         batch_size: Optional[int] = None,
         scale_cost: Scale_t = 1.0,
         cost_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         cost_matrix_rank: Optional[int] = None,
         # problem
         **kwargs: Any,
@@ -261,15 +261,15 @@
 
     def _prepare(
         self,
         xy: Optional[TaggedArray] = None,
         x: Optional[TaggedArray] = None,
         y: Optional[TaggedArray] = None,
         # geometry
-        epsilon: Optional[Union[float, epsilon_scheduler.Epsilon]] = None,
+        epsilon: Union[float, epsilon_scheduler.Epsilon] = None,
         relative_epsilon: Optional[bool] = None,
         batch_size: Optional[int] = None,
         scale_cost: Scale_t = 1.0,
         cost_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         cost_matrix_rank: Optional[int] = None,
         # problem
         alpha: float = 0.5,
```

### Comparing `moscot-0.3.1/src/moscot/backends/utils.py` & `moscot-0.3.2/src/moscot/backends/utils.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/base/cost.py` & `moscot-0.3.2/src/moscot/base/cost.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/base/output.py` & `moscot-0.3.2/src/moscot/base/output.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/base/problems/__init__.py` & `moscot-0.3.2/src/moscot/base/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/base/problems/_mixins.py` & `moscot-0.3.2/src/moscot/base/problems/_mixins.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/base/problems/_utils.py` & `moscot-0.3.2/src/moscot/base/problems/_utils.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/base/problems/birth_death.py` & `moscot-0.3.2/src/moscot/base/problems/birth_death.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/base/problems/compound_problem.py` & `moscot-0.3.2/src/moscot/base/problems/compound_problem.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/base/problems/manager.py` & `moscot-0.3.2/src/moscot/base/problems/manager.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/base/problems/problem.py` & `moscot-0.3.2/src/moscot/base/problems/problem.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/base/solver.py` & `moscot-0.3.2/src/moscot/base/solver.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/costs/_costs.py` & `moscot-0.3.2/src/moscot/costs/_costs.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/costs/_utils.py` & `moscot-0.3.2/src/moscot/costs/_utils.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/datasets.py` & `moscot-0.3.2/src/moscot/datasets.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/plotting/_plotting.py` & `moscot-0.3.2/src/moscot/plotting/_plotting.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/plotting/_utils.py` & `moscot-0.3.2/src/moscot/plotting/_utils.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/problems/_utils.py` & `moscot-0.3.2/src/moscot/problems/_utils.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/problems/cross_modality/_mixins.py` & `moscot-0.3.2/src/moscot/problems/cross_modality/_mixins.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/problems/cross_modality/_translation.py` & `moscot-0.3.2/src/moscot/problems/cross_modality/_translation.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         if xy:
             kwargs["xy"] = xy
         return super().prepare(x=x, y=y, policy="external_star", key=batch_key, cost=cost, a=a, b=b, **kwargs)  # type: ignore[return-value] # noqa: E501
 
     def solve(  # type: ignore[override]
         self,
         alpha: Optional[float] = 1.0,
-        epsilon: Optional[float] = 1e-2,
+        epsilon: float = 1e-2,
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: QuadInitializer_t = None,
```

### Comparing `moscot-0.3.1/src/moscot/problems/generic/_generic.py` & `moscot-0.3.2/src/moscot/problems/generic/_generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             a=a,
             b=b,
             **kwargs,
         )
 
     def solve(
         self,
-        epsilon: Optional[float] = 1e-3,
+        epsilon: float = 1e-3,
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: SinkhornInitializer_t = None,
@@ -370,15 +370,15 @@
             b=b,
             **kwargs,
         )
 
     def solve(
         self,
         alpha: float = 1.0,
-        epsilon: Optional[float] = 1e-3,
+        epsilon: float = 1e-3,
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: QuadInitializer_t = None,
```

### Comparing `moscot-0.3.1/src/moscot/problems/generic/_mixins.py` & `moscot-0.3.2/src/moscot/problems/generic/_mixins.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/problems/space/_alignment.py` & `moscot-0.3.2/src/moscot/problems/space/_alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         return super().prepare(  # type: ignore[return-value]
             x=x, y=y, xy=xy, policy=policy, key=batch_key, reference=reference, cost=cost, a=a, b=b, **kwargs
         )
 
     def solve(
         self,
         alpha: float = 0.5,
-        epsilon: Optional[float] = 1e-2,
+        epsilon: float = 1e-2,
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: QuadInitializer_t = None,
```

### Comparing `moscot-0.3.1/src/moscot/problems/space/_mapping.py` & `moscot-0.3.2/src/moscot/problems/space/_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         return super().prepare(  # type: ignore[return-value]
             x=x, y=y, policy="external_star", key=batch_key, cost=cost, a=a, b=b, **kwargs
         )
 
     def solve(
         self,
         alpha: float = 0.5,
-        epsilon: Optional[float] = 1e-2,
+        epsilon: float = 1e-2,
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: QuadInitializer_t = None,
```

### Comparing `moscot-0.3.1/src/moscot/problems/space/_mixins.py` & `moscot-0.3.2/src/moscot/problems/space/_mixins.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/problems/spatiotemporal/_spatio_temporal.py` & `moscot-0.3.2/src/moscot/problems/spatiotemporal/_spatio_temporal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import types
 from typing import Any, Literal, Mapping, Optional, Tuple, Type, Union
 
+from ott.geometry import epsilon_scheduler
+
 from anndata import AnnData
 
 from moscot import _constants
 from moscot._types import (
     CostKwargs_t,
     Numeric_t,
     OttCostFnMap_t,
@@ -153,15 +155,15 @@
             marginal_kwargs=marginal_kwargs,
             **kwargs,
         )
 
     def solve(
         self,
         alpha: float = 0.5,
-        epsilon: Optional[float] = 1e-3,
+        epsilon: Union[float, epsilon_scheduler.Epsilon] = 1e-3,
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: QuadInitializer_t = None,
```

### Comparing `moscot-0.3.1/src/moscot/problems/time/_lineage.py` & `moscot-0.3.2/src/moscot/problems/time/_lineage.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             a=a,
             b=b,
             **kwargs,
         )
 
     def solve(
         self,
-        epsilon: Optional[float] = 1e-3,
+        epsilon: float = 1e-3,
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: SinkhornInitializer_t = None,
@@ -391,15 +391,15 @@
             marginal_kwargs=marginal_kwargs,
             **kwargs,
         )
 
     def solve(
         self,
         alpha: float = 0.5,
-        epsilon: Optional[float] = 1e-3,
+        epsilon: float = 1e-3,
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: QuadInitializer_t = None,
```

### Comparing `moscot-0.3.1/src/moscot/problems/time/_mixins.py` & `moscot-0.3.2/src/moscot/problems/time/_mixins.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/utils/_data/allTFs_dmel.txt` & `moscot-0.3.2/src/moscot/utils/_data/allTFs_dmel.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/utils/_data/allTFs_hg38.txt` & `moscot-0.3.2/src/moscot/utils/_data/allTFs_hg38.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/utils/_data/allTFs_mm.txt` & `moscot-0.3.2/src/moscot/utils/_data/allTFs_mm.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/utils/_data/human_apoptosis.txt` & `moscot-0.3.2/src/moscot/utils/_data/human_apoptosis.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/utils/_data/human_proliferation.txt` & `moscot-0.3.2/src/moscot/utils/_data/human_proliferation.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/utils/_data/mouse_apoptosis.txt` & `moscot-0.3.2/src/moscot/utils/_data/mouse_apoptosis.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/utils/_data/mouse_proliferation.txt` & `moscot-0.3.2/src/moscot/utils/_data/mouse_proliferation.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/utils/data.py` & `moscot-0.3.2/src/moscot/utils/data.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/utils/subset_policy.py` & `moscot-0.3.2/src/moscot/utils/subset_policy.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot/utils/tagged_array.py` & `moscot-0.3.2/src/moscot/utils/tagged_array.py`

 * *Files identical despite different names*

### Comparing `moscot-0.3.1/src/moscot.egg-info/PKG-INFO` & `moscot-0.3.2/src/moscot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moscot
-Version: 0.3.1
+Version: 0.3.2
 Summary: Multi-omic single-cell optimal transport tools
 Author: Dominik Klein, Giovanni Palla, Michal Klein, Zoe Piran, Marius Lange
 Maintainer-email: Dominik Klein <dominik.klein@helmholtz-muenchen.de>, Giovanni Palla <giovanni.palla@helmholtz-muenchen.de>, Michal Klein <michal.klein@helmholtz-muenchen.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Theis Lab
         All rights reserved.
```

### Comparing `moscot-0.3.1/src/moscot.egg-info/SOURCES.txt` & `moscot-0.3.2/src/moscot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

