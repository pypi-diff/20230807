# Comparing `tmp/ott-jax-0.4.2.tar.gz` & `tmp/ott-jax-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ott-jax-0.4.2.tar", last modified: Thu Jul  6 22:25:50 2023, max compression
+gzip compressed data, was "ott-jax-0.4.3.tar", last modified: Mon Aug  7 09:41:03 2023, max compression
```

## Comparing `ott-jax-0.4.2.tar` & `ott-jax-0.4.3.tar`

### file list

```diff
@@ -1,112 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.612058 ott-jax-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-06 22:24:34.000000 ott-jax-0.4.2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-06 22:24:34.000000 ott-jax-0.4.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-06 22:24:34.000000 ott-jax-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-06 22:24:34.000000 ott-jax-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-06 22:24:34.000000 ott-jax-0.4.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-06 22:24:34.000000 ott-jax-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 22:24:34.000000 ott-jax-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-07-06 22:25:50.612058 ott-jax-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-06 22:24:34.000000 ott-jax-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 22:24:34.000000 ott-jax-0.4.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-06 22:24:34.000000 ott-jax-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 22:25:50.612058 ott-jax-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-06 22:24:34.000000 ott-jax-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.588058 ott-jax-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.592058 ott-jax-0.4.2/src/ott/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.592058 ott-jax-0.4.2/src/ott/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/costs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/epsilon_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32238 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/low_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/geometry/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.592058 ott-jax-0.4.2/src/ott/initializers/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.592058 ott-jax-0.4.2/src/ott/initializers/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/linear/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/linear/initializers_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/initializers/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/nn/initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/initializers/quadratic/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/initializers/quadratic/initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/math/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/math/fixed_point_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/math/matrix_square_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/math/unbalanced_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/problems/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/linear/barycenter_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/linear/linear_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/linear/potentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.596058 ott-jax-0.4.2/src/ott/problems/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/nn/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.600058 ott-jax-0.4.2/src/ott/problems/quadratic/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/quadratic/gw_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/quadratic/quadratic_costs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20108 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/problems/quadratic/quadratic_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.600058 ott-jax-0.4.2/src/ott/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.600058 ott-jax-0.4.2/src/ott/solvers/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/acceleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/continuous_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/discrete_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/implicit_differentiation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/lineax_implicit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/lr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51767 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    28038 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/linear/sinkhorn_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.604058 ott-jax-0.4.2/src/ott/solvers/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/conjugate_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/nn/neuraldual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.604058 ott-jax-0.4.2/src/ott/solvers/quadratic/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/quadratic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19738 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/quadratic/gromov_wasserstein.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/quadratic/gw_barycenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/solvers/was_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.608058 ott-jax-0.4.2/src/ott/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.608058 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/fit_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/fit_gmm_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/gaussian_mixture/scale_tril.py
--rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/k_means.py
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/map_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/segment_sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/sinkhorn_divergence.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/tools/soft_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-06 22:24:34.000000 ott-jax-0.4.2/src/ott/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:25:50.612058 ott-jax-0.4.2/src/ott_jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-07-06 22:25:50.000000 ott-jax-0.4.2/src/ott_jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-06 22:25:50.000000 ott-jax-0.4.2/src/ott_jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:25:50.000000 ott-jax-0.4.2/src/ott_jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 22:25:50.000000 ott-jax-0.4.2/src/ott_jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 22:25:50.000000 ott-jax-0.4.2/src/ott_jax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.224658 ott-jax-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-07 09:39:54.000000 ott-jax-0.4.3/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-07 09:39:54.000000 ott-jax-0.4.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-08-07 09:39:54.000000 ott-jax-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-07 09:39:54.000000 ott-jax-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-07 09:39:54.000000 ott-jax-0.4.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-07 09:39:54.000000 ott-jax-0.4.3/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-08-07 09:39:54.000000 ott-jax-0.4.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-08-07 09:39:54.000000 ott-jax-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-07 09:39:54.000000 ott-jax-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 09:39:54.000000 ott-jax-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-08-07 09:41:03.224658 ott-jax-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-08-07 09:39:54.000000 ott-jax-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-07 09:39:54.000000 ott-jax-0.4.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-08-07 09:39:54.000000 ott-jax-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 09:41:03.224658 ott-jax-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-07 09:39:54.000000 ott-jax-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.188658 ott-jax-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.188658 ott-jax-0.4.3/src/ott/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.188658 ott-jax-0.4.3/src/ott/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35276 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/geometry/costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/geometry/epsilon_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32238 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/geometry/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/geometry/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/geometry/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/geometry/low_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/geometry/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/geometry/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.192658 ott-jax-0.4.3/src/ott/initializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.192658 ott-jax-0.4.3/src/ott/initializers/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/initializers/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/initializers/linear/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/initializers/linear/initializers_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.192658 ott-jax-0.4.3/src/ott/initializers/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/initializers/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/initializers/nn/initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.192658 ott-jax-0.4.3/src/ott/initializers/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/initializers/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/initializers/quadratic/initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.196658 ott-jax-0.4.3/src/ott/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/math/fixed_point_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/math/matrix_square_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/math/unbalanced_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.196658 ott-jax-0.4.3/src/ott/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.200658 ott-jax-0.4.3/src/ott/problems/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/problems/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/problems/linear/barycenter_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/problems/linear/linear_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/problems/linear/potentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.200658 ott-jax-0.4.3/src/ott/problems/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/problems/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/problems/nn/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.200658 ott-jax-0.4.3/src/ott/problems/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/problems/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/problems/quadratic/gw_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/problems/quadratic/quadratic_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19303 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/problems/quadratic/quadratic_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.204658 ott-jax-0.4.3/src/ott/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.208658 ott-jax-0.4.3/src/ott/solvers/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/linear/acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/linear/continuous_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/linear/discrete_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/linear/implicit_differentiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/linear/lineax_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/linear/lr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51795 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/linear/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28038 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/linear/sinkhorn_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.212658 ott-jax-0.4.3/src/ott/solvers/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/nn/conjugate_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/nn/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/nn/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/nn/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/nn/neuraldual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.212658 ott-jax-0.4.3/src/ott/solvers/quadratic/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/quadratic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/quadratic/gromov_wasserstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/quadratic/gw_barycenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/solvers/was_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.216658 ott-jax-0.4.3/src/ott/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.220658 ott-jax-0.4.3/src/ott/tools/gaussian_mixture/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/gaussian_mixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/gaussian_mixture/fit_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/gaussian_mixture/fit_gmm_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/gaussian_mixture/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/gaussian_mixture/gaussian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/gaussian_mixture/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/gaussian_mixture/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/gaussian_mixture/scale_tril.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/k_means.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/map_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/segment_sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/sinkhorn_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/tools/soft_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-07 09:39:54.000000 ott-jax-0.4.3/src/ott/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 09:41:03.224658 ott-jax-0.4.3/src/ott_jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-08-07 09:41:02.000000 ott-jax-0.4.3/src/ott_jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-07 09:41:03.000000 ott-jax-0.4.3/src/ott_jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 09:41:02.000000 ott-jax-0.4.3/src/ott_jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-07 09:41:02.000000 ott-jax-0.4.3/src/ott_jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-07 09:41:02.000000 ott-jax-0.4.3/src/ott_jax.egg-info/top_level.txt
```

### Comparing `ott-jax-0.4.2/.gitignore` & `ott-jax-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/.pre-commit-config.yaml` & `ott-jax-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/LICENSE` & `ott-jax-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/PKG-INFO` & `ott-jax-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ott-jax
-Version: 0.4.2
+Version: 0.4.3
 Summary: Optimal Transport Tools in JAX.
 Author-email: OTT team <optimal.transport.tools@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ott-jax-0.4.2/README.md` & `ott-jax-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/pyproject.toml` & `ott-jax-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 authors = [
     {name = "OTT team", email = "optimal.transport.tools@gmail.com"}
 ]
 dependencies = [
     "jax>=0.1.67",
     "jaxlib>=0.1.47",
     "jaxopt>=0.5.5",
-    # numba/numpy compatibility issue
-    "numpy>=1.18.4, !=1.25.0",
-    "flax>=0.5.2",
+    # numba/numpy compatibility issue in JAXOPT.
+    "numpy>=1.18.4, <1.25.0",
+    "flax>=0.6.6",
     "optax>=0.1.1",
     "lineax>=0.0.1; python_version >= '3.9'"
 ]
 keywords = [
     "optimal transport",
     "gromov wasserstein",
     "sinkhorn",
@@ -71,14 +71,15 @@
     "coverage[toml]",
     "chex",
     "networkx>=2.5",
     "scikit-learn>=1.0",
     # tslearn needs numba, which isn't supported for 3.11
     "tslearn>=0.5; python_version < '3.11'",
     "lineax; python_version >= '3.9'",
+    "matplotlib",
 ]
 docs = [
     "sphinx>=4.0",
     "sphinx-book-theme>=1.0.1",
     "sphinx_autodoc_typehints>=1.12.0",
     "sphinx-copybutton>=0.5.1",
     "sphinxcontrib-bibtex>=2.5.0",
@@ -119,14 +120,15 @@
 
 [tool.coverage.run]
 branch = true
 source = ["src/"]
 omit = [
     "*/__init__.py",
     "*/_version.py",
+    "*/types.py",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     '\#.*pragma:\s*no.?cover',
     "^if __name__ == .__main__.:$",
     '^\s*raise AssertionError\b',
@@ -145,14 +147,15 @@
 split_before_named_assigns = true
 spaces_around_power_operator = true
 dedent_closing_brackets = true
 coalesce_brackets = true
 
 [tool.rstcheck]
 ignore_directives = [
+    "include",
     "toctree",
     "module",
     "currentmodule",
     "autosummary",
     "automodule",
     "autoclass",
     "bibliography"
@@ -162,15 +165,16 @@
     "doc",
     "mod",
     "cite",
 ]
 
 [tool.doc8]
 max_line_length = 80
-ignore_path = ['docs/**/_autosummary']
+# Parser "myst_parser.sphinx_" not found. No module named 'myst_parser'.
+ignore_path = ["docs/**/_autosummary", "docs/contributing.rst"]
 
 [tool.tox]
 legacy_tox_ini = """
     [tox]
     min_version = 4.0
     env_list = lint-code,py{3.8,3.9,3.10,3.11}
     skip_missing_interpreters = true
```

### Comparing `ott-jax-0.4.2/setup.py` & `ott-jax-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/__init__.py` & `ott-jax-0.4.3/src/ott/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/_version.py` & `ott-jax-0.4.3/src/ott/_version.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/geometry/__init__.py` & `ott-jax-0.4.3/src/ott/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/geometry/costs.py` & `ott-jax-0.4.3/src/ott/geometry/costs.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,18 @@
   def pairwise(self, x: jnp.ndarray, y: jnp.ndarray) -> float:
     """Compute Euclidean norm."""
     return jnp.linalg.norm(x - y)
 
 
 @jax.tree_util.register_pytree_node_class
 class SqEuclidean(TICost):
-  """Squared Euclidean distance."""
+  r"""Squared Euclidean distance.
+
+  Implemented as a translation invariant cost, :math:`h(z) = \|z\|^2`.
+  """
 
   def norm(self, x: jnp.ndarray) -> Union[float, jnp.ndarray]:
     """Compute squared Euclidean norm for vector."""
     return jnp.sum(x ** 2, axis=-1)
 
   def pairwise(self, x: jnp.ndarray, y: jnp.ndarray) -> float:
     """Compute minus twice the dot-product between vectors."""
@@ -308,21 +311,22 @@
     return jnp.ones((1, dim))
 
 
 class RegTICost(TICost, abc.ABC):
   r"""Base class for regularized translation-invariant costs.
 
   .. math::
-    \frac{1}{2} \|\cdot\|_2^2 + \text{scaling_reg} reg\left(\cdot\right)
+    \frac{1}{2} \|\cdot\|_2^2 + \text{scaling_reg} reg\left(matrix \cdot\right)
 
   where :func:`reg` is the regularization function.
 
   Args:
     scaling_reg: Strength of the :meth:`regularization <reg>`.
-    matrix: :math:`p \times d` projection matrix with **orthogonal rows**.
+    matrix: :math:`p \times d` projection matrix in the Stiefel manifold,
+      namely with **orthonormalized rows**.
     orthogonal: Whether to regularize in the orthogonal complement
       to promote displacements in the span of ``matrix``.
   """
 
   def __init__(
       self,
       scaling_reg: float = 1.0,
```

### Comparing `ott-jax-0.4.2/src/ott/geometry/epsilon_scheduler.py` & `ott-jax-0.4.3/src/ott/geometry/epsilon_scheduler.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/geometry/geometry.py` & `ott-jax-0.4.3/src/ott/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/geometry/graph.py` & `ott-jax-0.4.3/src/ott/geometry/graph.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/geometry/grid.py` & `ott-jax-0.4.3/src/ott/geometry/grid.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/geometry/low_rank.py` & `ott-jax-0.4.3/src/ott/geometry/low_rank.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/geometry/pointcloud.py` & `ott-jax-0.4.3/src/ott/geometry/pointcloud.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/geometry/segment.py` & `ott-jax-0.4.3/src/ott/geometry/segment.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/initializers/__init__.py` & `ott-jax-0.4.3/src/ott/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/initializers/linear/__init__.py` & `ott-jax-0.4.3/src/ott/initializers/linear/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/initializers/linear/initializers.py` & `ott-jax-0.4.3/src/ott/initializers/linear/initializers.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/initializers/linear/initializers_lr.py` & `ott-jax-0.4.3/src/ott/initializers/linear/initializers_lr.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/initializers/nn/__init__.py` & `ott-jax-0.4.3/src/ott/initializers/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/initializers/nn/initializers.py` & `ott-jax-0.4.3/src/ott/initializers/nn/initializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,17 @@
       f_pred = self._compute_f(a, b, params)
       g_pred = self.geom.update_potential(
           f_pred, jnp.zeros_like(b), jnp.log(b), 0, axis=0
       )
       g_pred = jnp.where(jnp.isfinite(g_pred), g_pred, 0.)
 
       ot_prob = linear_problem.LinearProblem(geom=self.geom, a=a, b=b)
-      dual_obj = sinkhorn.ent_reg_cost(f_pred, g_pred, ot_prob, lse_mode=True)
+      dual_obj = sinkhorn.compute_kl_reg_cost(
+          f_pred, g_pred, ot_prob, lse_mode=True
+      )
       loss = -dual_obj
       return loss, f_pred
 
     def loss_batch(params, a, b):
       loss_fn = functools.partial(dual_obj_loss_single, params=params)
       loss, f_pred = jax.vmap(loss_fn)(a=a, b=b)
       return jnp.mean(loss), f_pred
```

### Comparing `ott-jax-0.4.2/src/ott/initializers/quadratic/__init__.py` & `ott-jax-0.4.3/src/ott/initializers/quadratic/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/initializers/quadratic/initializers.py` & `ott-jax-0.4.3/src/ott/initializers/quadratic/initializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import abc
-from typing import TYPE_CHECKING, Any, Dict, Sequence, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, Tuple
 
 import jax
 import jax.numpy as jnp
 
 from ott.geometry import geometry
 
 if TYPE_CHECKING:
@@ -117,23 +117,28 @@
      \text{right}_y(\text{cost_yy}) + \text{unbalanced_correction}
 
   When working with the fused problem, a linear term is added to the cost
   matrix: `cost_matrix` += `fused_penalty` * `geom_xy.cost_matrix`
   """
 
   def _create_geometry(
-      self, quad_prob: "quadratic_problem.QuadraticProblem", *, epsilon: float,
+      self,
+      quad_prob: "quadratic_problem.QuadraticProblem",
+      *,
+      epsilon: float,
+      relative_epsilon: Optional[bool] = None,
       **kwargs: Any
   ) -> geometry.Geometry:
     """Compute initial geometry for linearization.
 
     Args:
       quad_prob: Quadratic OT problem.
       epsilon: Epsilon regularization.
-      kwargs: Additional keyword arguments, unused.
+      relative_epsilon: Flag, use `relative_epsilon` or not in geometry.
+      kwargs: Keyword arguments for :class:`~ott.geometry.geometry.Geometry`.
 
     Returns:
       The initial geometry used to initialize the linearized problem.
     """
     from ott.problems.quadratic import quadratic_problem
     del kwargs
 
@@ -156,36 +161,44 @@
           epsilon=epsilon, transport_mass=marginal_1.sum()
       )
       unbalanced_correction = quad_prob.cost_unbalanced_correction(
           init_transport, marginal_1, marginal_2, epsilon=epsilon
       )
       cost_matrix = marginal_cost.cost_matrix - tmp + unbalanced_correction
 
-    cost_matrix += quad_prob.fused_penalty * quad_prob._fused_cost_matrix()
-    return geometry.Geometry(cost_matrix=cost_matrix, epsilon=epsilon)
+    cost_matrix += quad_prob.fused_penalty * quad_prob._fused_cost_matrix
+    return geometry.Geometry(
+        cost_matrix=cost_matrix,
+        epsilon=epsilon,
+        relative_epsilon=relative_epsilon
+    )
 
 
 class LRQuadraticInitializer(BaseQuadraticInitializer):
   """Wrapper that wraps low-rank Sinkhorn initializers.
 
   Args:
     lr_linear_initializer: Low-rank linear initializer.
   """
 
   def __init__(self, lr_linear_initializer: "initializers_lr.LRInitializer"):
     super().__init__()
     self._linear_lr_initializer = lr_linear_initializer
 
   def _create_geometry(
-      self, quad_prob: "quadratic_problem.QuadraticProblem", **kwargs: Any
+      self,
+      quad_prob: "quadratic_problem.QuadraticProblem",
+      relative_epsilon: Optional[bool] = False,
+      **kwargs: Any
   ) -> geometry.Geometry:
     """Compute initial geometry for linearization.
 
     Args:
       quad_prob: Quadratic OT problem.
+      relative_epsilon: Whether to use relative epsilon in the geometry.
       kwargs: Keyword arguments for
         :meth:`~ott.initializers.linear.initializers_lr.LRInitializer.__call__`.
 
     Returns:
       The initial geometry used to initialize a linear problem.
     """
     from ott.solvers.linear import sinkhorn_lr
@@ -197,15 +210,15 @@
         g=g,
         costs=None,
         errors=None,
         ot_prob=None,
         epsilon=None,
     )
 
-    return quad_prob.update_lr_geom(tmp_out)
+    return quad_prob.update_lr_geom(tmp_out, relative_epsilon=relative_epsilon)
 
   @property
   def rank(self) -> int:
     """Rank of the transport matrix factorization."""
     return self._linear_lr_initializer.rank
 
   def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
```

### Comparing `ott-jax-0.4.2/src/ott/math/__init__.py` & `ott-jax-0.4.3/src/ott/math/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/math/fixed_point_loop.py` & `ott-jax-0.4.3/src/ott/math/fixed_point_loop.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/math/matrix_square_root.py` & `ott-jax-0.4.3/src/ott/math/matrix_square_root.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/math/unbalanced_functions.py` & `ott-jax-0.4.3/src/ott/math/unbalanced_functions.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/math/utils.py` & `ott-jax-0.4.3/src/ott/math/utils.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/problems/__init__.py` & `ott-jax-0.4.3/src/ott/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/problems/linear/__init__.py` & `ott-jax-0.4.3/src/ott/problems/linear/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/problems/linear/barycenter_problem.py` & `ott-jax-0.4.3/src/ott/problems/linear/barycenter_problem.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,20 +36,14 @@
       ``[num_measures, max_measure_size]`` can be passed.
       If ``y`` is already pre-segmented, this array must be always specified.
     weights: Array of shape ``[num_measures,]`` containing the weights of the
       measures.
     cost_fn: Cost function used. If `None`,
       use the :class:`~ott.geometry.costs.SqEuclidean` cost.
     epsilon: Epsilon regularization used to solve reg-OT problems.
-    debiased: **Currently not implemented.**
-      Whether the problem is debiased, in the sense that
-      the regularized transportation cost of barycenter to itself will
-      be considered when computing gradient. Note that if the debiased option
-      is used, the barycenter size needs to be smaller than the maximum measure
-      size for parallelization to operate efficiently.
     kwargs: Keyword arguments :func:`~ott.geometry.segment.segment_point_cloud`.
       Only used when ``y`` is not already segmented. When passing
       ``segment_ids``, 2 arguments must be specified for jitting to work:
 
         - ``num_segments`` - the total number of measures.
         - ``max_measure_size`` -  maximum of support sizes of these measures.
   """
@@ -57,25 +51,23 @@
   def __init__(
       self,
       y: jnp.ndarray,
       b: Optional[jnp.ndarray] = None,
       weights: Optional[jnp.ndarray] = None,
       cost_fn: Optional[costs.CostFn] = None,
       epsilon: Optional[float] = None,
-      debiased: bool = False,
       **kwargs: Any,
   ):
     self._y = y
     if y.ndim == 3 and b is None:
       raise ValueError("Specify weights if `y` is already segmented.")
     self._b = b
     self._weights = weights
     self.cost_fn = costs.SqEuclidean() if cost_fn is None else cost_fn
     self.epsilon = epsilon
-    self.debiased = debiased
     self._kwargs = kwargs
 
     if self._is_segmented:
       # (num_measures, max_measure_size, ndim)
       # (num_measures, max_measure_size)
       assert self._y.shape[:2] == self._b.shape
     else:
@@ -83,42 +75,26 @@
       # (num_total_points,)
       assert self._b is None or self._y.shape[0] == self._b.shape[0]
 
   @property
   def segmented_y_b(self) -> Tuple[jnp.ndarray, jnp.ndarray]:
     """Tuple of arrays containing the segmented measures and weights.
 
-    Additional segment may be added when the problem is debiased.
-
-      - Segmented measures of shape ``[num_measures, max_measure_size, ndim]``.
-      - Segmented weights of shape ``[num_measures, max_measure_size]``.
+    - Segmented measures of shape ``[num_measures, max_measure_size, ndim]``.
+    - Segmented weights of shape ``[num_measures, max_measure_size]``.
     """
     if self._is_segmented:
       y, b = self._y, self._b
     else:
       y, b = segment.segment_point_cloud(
           x=self._y,
           a=self._b,
           padding_vector=self.cost_fn._padder(self.ndim),
           **self._kwargs
       )
-
-    if self.debiased:
-      return self._add_slice_for_debiased(y, b)
-    return y, b
-
-  @staticmethod
-  def _add_slice_for_debiased(
-      y: jnp.ndarray, b: jnp.ndarray
-  ) -> Tuple[jnp.ndarray, jnp.ndarray]:
-    _, n, ndim = y.shape  # (num_measures, max_measure_size, ndim)
-    # yapf: disable
-    y = jnp.concatenate((y, jnp.zeros((1, n, ndim))), axis=0)
-    b = jnp.concatenate((b, jnp.zeros((1, n))), axis=0)
-    # yapf: enable
     return y, b
 
   @property
   def flattened_y(self) -> jnp.ndarray:
     """Array of shape ``[num_measures * (N_1 + N_2 + ...), ndim]``."""
     if self._is_segmented:
       return self._y.reshape((-1, self._y.shape[-1]))
@@ -144,33 +120,28 @@
     """Number of dimensions of ``y``."""
     return self._y.shape[-1]
 
   @property
   def weights(self) -> jnp.ndarray:
     """Barycenter weights of shape ``[num_measures,]`` that sum to 1."""
     if self._weights is None:
-      weights = jnp.ones((self.num_measures,)) / self.num_measures
-    else:
-      # Check that the number of measures coincides with the weights' size.
-      assert self._weights.shape[0] == self.num_measures
-      # By default, we assume that weights sum to 1, and enforce this if needed.
-      weights = self._weights / jnp.sum(self._weights)
-    if self.debiased:
-      return jnp.concatenate((weights, jnp.array([-0.5])))
-    return weights
+      return jnp.ones((self.num_measures,)) / self.num_measures
+    # Check that the number of measures coincides with the weights' size.
+    assert self._weights.shape[0] == self.num_measures
+    # By default, we assume that weights sum to 1, and enforce this if needed.
+    return self._weights / jnp.sum(self._weights)
 
   @property
   def _is_segmented(self) -> bool:
     return self._y.ndim == 3
 
   def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     return ([self._y, self._b, self._weights], {
         "cost_fn": self.cost_fn,
         "epsilon": self.epsilon,
-        "debiased": self.debiased,
         **self._kwargs,
     })
 
   @classmethod
   def tree_unflatten(  # noqa: D102
       cls, aux_data: Dict[str, Any], children: Sequence[Any]
   ) -> "FreeBarycenterProblem":
```

### Comparing `ott-jax-0.4.2/src/ott/problems/linear/linear_problem.py` & `ott-jax-0.4.3/src/ott/problems/linear/linear_problem.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/problems/linear/potentials.py` & `ott-jax-0.4.3/src/ott/problems/linear/potentials.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import (
-    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Literal,
     Optional,
     Sequence,
     Tuple,
@@ -24,19 +23,17 @@
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
 import jax.tree_util as jtu
 import numpy as np
 
+from ott.geometry import costs
 from ott.problems.linear import linear_problem
 
-if TYPE_CHECKING:
-  from ott.geometry import costs
-
 try:
   import matplotlib as mpl
   import matplotlib.pyplot as plt
 except ImportError:
   mpl = plt = None
 
 __all__ = ["DualPotentials", "EntropicPotentials"]
@@ -60,19 +57,22 @@
   """
 
   def __init__(
       self,
       f: Potential_t,
       g: Potential_t,
       *,
-      cost_fn: "costs.CostFn",
+      cost_fn: costs.CostFn,
       corr: bool = False
   ):
     self._f = f
     self._g = g
+    assert (
+        not corr or type(cost_fn) == costs.SqEuclidean
+    ), "Duals in `corr` form can only be used with a squared-Euclidean cost."
     self.cost_fn = cost_fn
     self._corr = corr
 
   def transport(self, vec: jnp.ndarray, forward: bool = True) -> jnp.ndarray:
     r"""Transport ``vec`` according to Brenier formula :cite:`brenier:91`.
 
     Uses Theorem 1.17 from :cite:`santambrogio:15` to compute an OT map when
@@ -102,40 +102,42 @@
     if self._corr and isinstance(self.cost_fn, costs.SqEuclidean):
       return self._grad_f(vec) if forward else self._grad_g(vec)
     if forward:
       return vec - self._grad_h_inv(self._grad_f(vec))
     return vec - self._grad_h_inv(self._grad_g(vec))
 
   def distance(self, src: jnp.ndarray, tgt: jnp.ndarray) -> float:
-    """Evaluate 2-Wasserstein distance between samples using dual potentials.
+    r"""Evaluate Wasserstein distance between samples using dual potentials.
 
-    Uses Eq. 5 from :cite:`makkuva:20` when given in `corr` form, direct
-    estimation by integrating dual function against points when using dual form.
+    This uses direct estimation of potentials against measures when dual
+    functions are provided in usual form. This expression is valid for any
+    cost function.
+
+    When potentials are given in correlation form, as specified by the flag
+    ``corr``, the dual potentials solve the dual problem corresponding to the
+    minimization of the primal OT problem where the ground cost is
+    :math:`-2\langle x,y\rangle`. To recover the (squared) 2-Wasserstein
+    distance, terms are re-arranged and contributions from squared norms are
+    taken into account.
 
     Args:
       src: Samples from the source distribution, array of shape ``[n, d]``.
       tgt: Samples from the target distribution, array of shape ``[m, d]``.
 
     Returns:
-      Wasserstein distance.
+      Wasserstein distance using specified cost function.
     """
     src, tgt = jnp.atleast_2d(src), jnp.atleast_2d(tgt)
     f = jax.vmap(self.f)
-
-    if self._corr:
-      grad_g_y = self._grad_g(tgt)
-      term1 = -jnp.mean(f(src))
-      term2 = -jnp.mean(jnp.sum(tgt * grad_g_y, axis=-1) - f(grad_g_y))
-
-      C = jnp.mean(jnp.sum(src ** 2, axis=-1))
-      C += jnp.mean(jnp.sum(tgt ** 2, axis=-1))
-      return 2. * (term1 + term2) + C
-
     g = jax.vmap(self.g)
-    return jnp.mean(f(src)) + jnp.mean(g(tgt))
+    out = jnp.mean(f(src)) + jnp.mean(g(tgt))
+    if self._corr:
+      out = -2.0 * out + jnp.mean(jnp.sum(src ** 2, axis=-1))
+      out += jnp.mean(jnp.sum(tgt ** 2, axis=-1))
+    return out
 
   @property
   def f(self) -> Potential_t:
     """The first dual potential function."""
     return self._f
 
   @property
@@ -177,26 +179,29 @@
   ) -> "DualPotentials":
     return cls(*children, **aux_data)
 
   def plot_ot_map(
       self,
       source: jnp.ndarray,
       target: jnp.ndarray,
+      samples: Optional[jnp.ndarray] = None,
       forward: bool = True,
       ax: Optional["plt.Axes"] = None,
       legend_kwargs: Optional[Dict[str, Any]] = None,
       scatter_kwargs: Optional[Dict[str, Any]] = None,
   ) -> Tuple["plt.Figure", "plt.Axes"]:
     """Plot data and learned optimal transport map.
 
     Args:
       source: samples from the source measure
       target: samples from the target measure
-      forward: use the forward map from the potentials
-        if ``True``, otherwise use the inverse map
+      samples: extra samples to transport, either ``source`` (if ``forward``) or
+        ``target`` (if not ``forward``) by default.
+      forward: use the forward map from the potentials if ``True``,
+        otherwise use the inverse map.
       ax: axis to add the plot to
       scatter_kwargs: additional kwargs passed into
         :meth:`~matplotlib.axes.Axes.scatter`
       legend_kwargs: additional kwargs passed into
         :meth:`~matplotlib.axes.Axes.legend`
 
     Returns:
@@ -241,30 +246,30 @@
         target[:, 1],
         color=target_color,
         label="target",
         **scatter_kwargs,
     )
 
     # plot the transported samples
-    base_samples = source if forward else target
-    transported_samples = self.transport(base_samples, forward=forward)
+    samples = (source if forward else target) if samples is None else samples
+    transported_samples = self.transport(samples, forward=forward)
     ax.scatter(
         transported_samples[:, 0],
         transported_samples[:, 1],
         color="#F2545B",
         label=label_transport,
         **scatter_kwargs,
     )
 
-    for i in range(base_samples.shape[0]):
+    for i in range(samples.shape[0]):
       ax.arrow(
-          base_samples[i, 0],
-          base_samples[i, 1],
-          transported_samples[i, 0] - base_samples[i, 0],
-          transported_samples[i, 1] - base_samples[i, 1],
+          samples[i, 0],
+          samples[i, 1],
+          transported_samples[i, 0] - samples[i, 0],
+          transported_samples[i, 1] - samples[i, 1],
           color=[0.5, 0.5, 1],
           alpha=0.3
       )
 
     ax.legend(**legend_kwargs)
     return fig, ax
```

### Comparing `ott-jax-0.4.2/src/ott/problems/nn/__init__.py` & `ott-jax-0.4.3/src/ott/problems/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/problems/nn/dataset.py` & `ott-jax-0.4.3/src/ott/problems/nn/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,16 @@
     """
     return self._create_sample_generators()
 
   def _create_sample_generators(self) -> Iterator[jnp.array]:
     rng = self.init_rng
     while True:
       rng1, rng2, rng = jax.random.split(rng, 3)
-      means = jax.random.choice(rng1, self.centers, [self.batch_size])
-      normal_samples = jax.random.normal(rng2, [self.batch_size, 2])
+      means = jax.random.choice(rng1, self.centers, (self.batch_size,))
+      normal_samples = jax.random.normal(rng2, (self.batch_size, 2))
       samples = self.scale * means + self.variance ** 2 * normal_samples
       yield samples
 
 
 def create_gaussian_mixture_samplers(
     name_source: Name_t,
     name_target: Name_t,
```

### Comparing `ott-jax-0.4.2/src/ott/problems/quadratic/__init__.py` & `ott-jax-0.4.3/src/ott/problems/quadratic/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/problems/quadratic/gw_barycenter.py` & `ott-jax-0.4.3/src/ott/problems/quadratic/gw_barycenter.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/problems/quadratic/quadratic_costs.py` & `ott-jax-0.4.3/src/ott/problems/quadratic/quadratic_costs.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/problems/quadratic/quadratic_problem.py` & `ott-jax-0.4.3/src/ott/problems/quadratic/quadratic_problem.py`

 * *Files 12% similar despite different names*

```diff
@@ -130,16 +130,14 @@
     else:
       self.loss = loss
 
   def marginal_dependent_cost(
       self,
       marginal_1: jnp.ndarray,
       marginal_2: jnp.ndarray,
-      *,
-      remove_scale: bool = False,
   ) -> low_rank.LRCGeometry:
     r"""Initialize cost term that depends on the marginals of the transport.
 
     Uses the first term in eq. 6, p. 1 of :cite:`peyre:16`.
 
     Let :math:`p` be the `[n,]` marginal of the transport matrix for samples
     from :attr:`geom_xx` and :math:`q` the `[m,]` marginal of the
@@ -156,25 +154,19 @@
 
     This helper function instantiates these two low-rank matrices and groups
     them into a single low-rank cost geometry object.
 
     Args:
       marginal_1: [n,], first marginal of transport matrix.
       marginal_2: [m,], second marginal of transport matrix.
-      remove_scale: Whether to remove any scaling from the cost matrices before
-        computing the linearization.
 
     Returns:
       Low-rank geometry of rank 2, storing normalization constants.
     """
     geom_xx, geom_yy = self.geom_xx, self.geom_yy
-    if remove_scale:
-      geom_xx = geom_xx.set_scale_cost(1.0)
-      geom_yy = geom_yy.set_scale_cost(1.0)
-
     if self._loss_name == "sqeucl":  # quadratic apply, efficient for LR
       tmp1 = geom_xx.apply_square_cost(marginal_1, axis=1)
       tmp2 = geom_yy.apply_square_cost(marginal_2, axis=1)
     else:
       f1, f2 = self.linear_loss
       tmp1 = apply_cost(geom_xx, marginal_1, axis=1, fn=f1)
       tmp2 = apply_cost(geom_yy, marginal_2, axis=1, fn=f2)
@@ -247,53 +239,51 @@
     a = jax.lax.stop_gradient(self.a)
     b = jax.lax.stop_gradient(self.b)
     return a.sum() * b.sum()
 
   def update_lr_geom(
       self,
       lr_sink: "sinkhorn_lr.LRSinkhornOutput",
-      remove_scale: bool = False,
+      relative_epsilon: Optional[bool] = None,
   ) -> geometry.Geometry:
     """Recompute (possibly LRC) linearization using LR Sinkhorn output."""
     marginal_1 = lr_sink.marginal(1)
     marginal_2 = lr_sink.marginal(0)
-    marginal_cost = self.marginal_dependent_cost(
-        marginal_1, marginal_2, remove_scale=remove_scale
-    )
+    marginal_cost = self.marginal_dependent_cost(marginal_1, marginal_2)
 
     # Extract factors from LR Sinkhorn output
     q, r, inv_sqg = lr_sink.q, lr_sink.r, 1.0 / jnp.sqrt(lr_sink.g)
     # Distribute middle marginal evenly across both factors.
     q, r = q * inv_sqg[None, :], r * inv_sqg[None, :]
 
     # Handle LRC Geometry case.
     h1, h2 = self.quad_loss
     geom_xx, geom_yy, geom_xy = self.geom_xx, self.geom_yy, self.geom_xy
-    if remove_scale:
-      geom_xx = geom_xx.set_scale_cost(1.0)
-      geom_yy = geom_yy.set_scale_cost(1.0)
-      geom_xy = geom_xy.set_scale_cost(1.0) if self.is_fused else None
     tmp1 = apply_cost(geom_xx, q, axis=1, fn=h1)
     tmp2 = apply_cost(geom_yy, r, axis=1, fn=h2)
     if self.is_low_rank:
-      geom = low_rank.LRCGeometry(cost_1=tmp1, cost_2=-tmp2) + marginal_cost
+      geom = low_rank.LRCGeometry(
+          cost_1=tmp1, cost_2=-tmp2, relative_epsilon=relative_epsilon
+      ) + marginal_cost
       if self.is_fused:
         geom = geom + geom_xy
     else:
       cost_matrix = marginal_cost.cost_matrix - jnp.dot(tmp1, tmp2.T)
-      cost_matrix += self.fused_penalty * self._fused_cost_matrix(remove_scale)
-      geom = geometry.Geometry(cost_matrix=cost_matrix)
+      cost_matrix += self.fused_penalty * self._fused_cost_matrix
+      geom = geometry.Geometry(
+          cost_matrix=cost_matrix, relative_epsilon=relative_epsilon
+      )
     return geom  # noqa: RET504
 
   def update_linearization(
       self,
       transport: Transport,
       epsilon: Optional[Union[epsilon_scheduler.Epsilon, float]] = None,
       old_transport_mass: float = 1.0,
-      remove_scale: bool = False,
+      relative_epsilon: Optional[bool] = None,
   ) -> linear_problem.LinearProblem:
     """Update linearization of GW problem by updating cost matrix.
 
     If the problem is balanced (``tau_a = 1.0 and tau_b = 1.0``), the equation
     follows eq. 6, p. 1 of :cite:`peyre:16`.
 
     If the problem is unbalanced (``tau_a < 1.0 or tau_b < 1.0``), two cases are
@@ -303,88 +293,81 @@
     :meth:`init_linearization`.
 
     Args:
       transport: Solution of the linearization of the quadratic problem.
       epsilon: An epsilon scheduler or a float passed on to the linearization.
       old_transport_mass: Sum of the elements of the transport matrix at the
         previous iteration.
-      remove_scale: Whether to remove any scaling from the cost matrices when
-        computing the linearization of the quadratic cost. At the moment, this
-        is only used when doing this update at the last outer iteration of the
-        :class:`~ott.solvers.quadratic.gromov_wasserstein.GromovWasserstein`
-        solver.
+      relative_epsilon: Whether to use relative epsilon in the linearized
+        geometry.
 
     Returns:
       Updated linear OT problem, a new local linearization of GW problem.
     """
     rescale_factor = 1.0
     unbalanced_correction = 0.0
 
     if not self.is_balanced:
       marginal_1 = transport.marginal(axis=1)
       transport_mass = jax.lax.stop_gradient(marginal_1.sum())
       rescale_factor = jnp.sqrt(old_transport_mass / transport_mass)
 
     marginal_1 = transport.marginal(axis=1) * rescale_factor
     marginal_2 = transport.marginal(axis=0) * rescale_factor
-    marginal_cost = self.marginal_dependent_cost(
-        marginal_1, marginal_2, remove_scale=remove_scale
-    )
+    marginal_cost = self.marginal_dependent_cost(marginal_1, marginal_2)
 
     transport_matrix = transport.matrix * rescale_factor
 
     if not self.is_balanced:
       # Rescales transport for Unbalanced GW according to Sejourne et al. (2021)
       transport_mass = jax.lax.stop_gradient(marginal_1.sum())
       epsilon = update_epsilon_unbalanced(epsilon, transport_mass)
       unbalanced_correction = self.cost_unbalanced_correction(
           transport_matrix, marginal_1, marginal_2, epsilon
       )
 
     h1, h2 = self.quad_loss
     geom_xx, geom_yy = self.geom_xx, self.geom_yy
-    if remove_scale:
-      geom_xx = geom_xx.set_scale_cost(1.0)
-      geom_yy = geom_yy.set_scale_cost(1.0)
 
     tmp = apply_cost(geom_xx, transport_matrix, axis=1, fn=h1)
     tmp = apply_cost(geom_yy, tmp.T, axis=1, fn=h2).T
 
     cost_matrix = marginal_cost.cost_matrix - tmp + unbalanced_correction
-    cost_matrix += self.fused_penalty * rescale_factor * \
-                   self._fused_cost_matrix(remove_scale)
+    cost_matrix += self.fused_penalty * rescale_factor * self._fused_cost_matrix
 
-    geom = geometry.Geometry(cost_matrix=cost_matrix, epsilon=epsilon)
+    geom = geometry.Geometry(
+        cost_matrix=cost_matrix,
+        epsilon=epsilon,
+        relative_epsilon=relative_epsilon
+    )
 
     return linear_problem.LinearProblem(
         geom, self.a, self.b, tau_a=self.tau_a, tau_b=self.tau_b
     )
 
   def update_lr_linearization(
       self,
       lr_sink: "sinkhorn_lr.LRSinkhornOutput",
       *,
-      remove_scale: bool = False,
+      relative_epsilon: Optional[bool] = None,
   ) -> linear_problem.LinearProblem:
     """Update a Quad problem linearization using a LR Sinkhorn."""
     return linear_problem.LinearProblem(
-        self.update_lr_geom(lr_sink, remove_scale=remove_scale),
+        self.update_lr_geom(lr_sink, relative_epsilon=relative_epsilon),
         self.a,
         self.b,
         tau_a=self.tau_a,
         tau_b=self.tau_b
     )
 
-  def _fused_cost_matrix(self,
-                         unscale: bool = False) -> Union[float, jnp.ndarray]:
+  @property
+  def _fused_cost_matrix(self) -> Union[float, jnp.ndarray]:
     if not self.is_fused:
       return 0.0
     geom_xy = self.geom_xy
-    if unscale:
-      geom_xy = geom_xy.set_scale_cost(1.0)
 
     if isinstance(geom_xy, pointcloud.PointCloud) and geom_xy.is_online:
       return geom_xy._compute_cost_matrix() * geom_xy.inv_scale_cost
     return geom_xy.cost_matrix
 
   @property
   def _is_low_rank_convertible(self) -> bool:
```

### Comparing `ott-jax-0.4.2/src/ott/solvers/__init__.py` & `ott-jax-0.4.3/src/ott/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/linear/__init__.py` & `ott-jax-0.4.3/src/ott/solvers/linear/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/linear/acceleration.py` & `ott-jax-0.4.3/src/ott/solvers/linear/acceleration.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/linear/continuous_barycenter.py` & `ott-jax-0.4.3/src/ott/solvers/linear/continuous_barycenter.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,20 +85,14 @@
           )
       )
       return (
           out.reg_ot_cost, out.converged, out.matrix,
           out.errors if store_errors else None
       )
 
-    if bar_prob.debiased:
-      raise NotImplementedError(
-          "Debiased version of continuous Wasserstein barycenter "
-          "not yet implemented."
-      )
-
     reg_ot_costs, convergeds, matrices, errors = solve_linear_ot(
         self.a, self.x, seg_b, seg_y
     )
 
     cost = jnp.sum(reg_ot_costs * bar_prob.weights)
     updated_costs = self.costs.at[iteration].set(cost)
     converged = jnp.all(convergeds)
```

### Comparing `ott-jax-0.4.2/src/ott/solvers/linear/discrete_barycenter.py` & `ott-jax-0.4.3/src/ott/solvers/linear/discrete_barycenter.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/linear/implicit_differentiation.py` & `ott-jax-0.4.3/src/ott/solvers/linear/implicit_differentiation.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/linear/lineax_implicit.py` & `ott-jax-0.4.3/src/ott/solvers/linear/lineax_implicit.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/linear/lr_utils.py` & `ott-jax-0.4.3/src/ott/solvers/linear/lr_utils.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/linear/sinkhorn.py` & `ott-jax-0.4.3/src/ott/solvers/linear/sinkhorn.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,18 +81,18 @@
         gv,
         ot_prob,
         norm_error=norm_error,
         lse_mode=lse_mode,
         parallel_dual_updates=parallel_dual_updates
     )
 
-  def ent_reg_cost(  # noqa: D102
+  def compute_kl_reg_cost(  # noqa: D102
       self, ot_prob: linear_problem.LinearProblem, lse_mode: bool
   ) -> float:
-    return ent_reg_cost(self.fu, self.gv, ot_prob, lse_mode)
+    return compute_kl_reg_cost(self.fu, self.gv, ot_prob, lse_mode)
 
   def recenter(
       self,
       f: jnp.ndarray,
       g: jnp.ndarray,
       ot_prob: linear_problem.LinearProblem,
   ) -> Tuple[jnp.ndarray, jnp.ndarray]:
@@ -224,15 +224,15 @@
     marginal = geom.marginal_from_scalings(f_u, g_v, axis=axis)
   norm_error = jnp.asarray(norm_error)
   return jnp.sum(
       jnp.abs(marginal - target) ** norm_error[:, jnp.newaxis], axis=1
   ) ** (1.0 / norm_error)
 
 
-def ent_reg_cost(
+def compute_kl_reg_cost(
     f: jnp.ndarray, g: jnp.ndarray, ot_prob: linear_problem.LinearProblem,
     lse_mode: bool
 ) -> float:
   r"""Compute objective of Sinkhorn for OT problem given dual solutions.
 
   The objective is evaluated for dual solution ``f`` and ``g``, using
   information contained in  ``ot_prob``. The objective is the regularized
@@ -332,15 +332,15 @@
 
   def set_cost(  # noqa: D102
       self, ot_prob: linear_problem.LinearProblem, lse_mode: bool,
       use_danskin: bool
   ) -> "SinkhornOutput":
     f = jax.lax.stop_gradient(self.f) if use_danskin else self.f
     g = jax.lax.stop_gradient(self.g) if use_danskin else self.g
-    return self.set(reg_ot_cost=ent_reg_cost(f, g, ot_prob, lse_mode))
+    return self.set(reg_ot_cost=compute_kl_reg_cost(f, g, ot_prob, lse_mode))
 
   @property
   def dual_cost(self) -> jnp.ndarray:
     """Return dual transport cost, without considering regularizer."""
     a, b = self.ot_prob.a, self.ot_prob.b
     dual_cost = jnp.sum(jnp.where(a > 0.0, a * self.f, 0))
     dual_cost += jnp.sum(jnp.where(b > 0.0, b * self.g, 0))
```

### Comparing `ott-jax-0.4.2/src/ott/solvers/linear/sinkhorn_lr.py` & `ott-jax-0.4.3/src/ott/solvers/linear/sinkhorn_lr.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/nn/__init__.py` & `ott-jax-0.4.3/src/ott/solvers/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/nn/conjugate_solvers.py` & `ott-jax-0.4.3/src/ott/solvers/nn/conjugate_solvers.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/nn/layers.py` & `ott-jax-0.4.3/src/ott/solvers/nn/layers.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/nn/losses.py` & `ott-jax-0.4.3/src/ott/solvers/nn/losses.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/nn/models.py` & `ott-jax-0.4.3/src/ott/solvers/nn/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -160,25 +160,27 @@
     init_fn: choice of initialization method for weight matrices (default:
       :func:`jax.nn.initializers.normal`).
     act_fn: choice of activation function used in network architecture
       (needs to be convex, default: :obj:`jax.nn.relu`).
     pos_weights: Enforce positive weights with a projection.
       If ``False``, the positive weights should be enforced with clipping
       or regularization in the loss.
-    gaussian_map: data inputs of source and target measures for
-      initialization scheme based on Gaussian approximation of input and
-      target measure (if ``None``, identity initialization is used).
+    gaussian_map_samples: Tuple of source and target points, used to initialize
+      the ICNN to mimic the linear Bures map that morphs the (Gaussian
+      approximation) of the input measure to that of the target measure. If
+      ``None``, the identity initialization is used, and ICNN mimics half the
+      squared Euclidean norm.
   """
   dim_data: int
   dim_hidden: Sequence[int]
   init_std: float = 1e-2
   init_fn: Callable = jax.nn.initializers.normal
   act_fn: Callable[[jnp.ndarray], jnp.ndarray] = nn.relu
   pos_weights: bool = True
-  gaussian_map: Optional[Tuple[jnp.ndarray, jnp.ndarray]] = None
+  gaussian_map_samples: Optional[Tuple[jnp.ndarray, jnp.ndarray]] = None
 
   @property
   def is_potential(self) -> bool:  # noqa: D102
     return True
 
   def setup(self) -> None:  # noqa: D102
     self.num_hidden = len(self.dim_hidden)
@@ -189,18 +191,20 @@
       # used in PositiveDense layers
       rescale = hid_dense.inv_rectifier_fn
     else:
       hid_dense = nn.Dense
       rescale = lambda x: x
     self.use_init = False
     # check if Gaussian map was provided
-    if self.gaussian_map is not None:
-      factor, mean = self._compute_gaussian_map(self.gaussian_map)
+    if self.gaussian_map_samples is not None:
+      factor, mean = self._compute_gaussian_map_params(
+          self.gaussian_map_samples
+      )
     else:
-      factor, mean = self._compute_identity_map(self.dim_data)
+      factor, mean = self._compute_identity_map_params(self.dim_data)
 
     w_zs = []
     # keep track of previous size to normalize accordingly
     normalization = 1
 
     for i in range(1, self.num_hidden):
       w_zs.append(
@@ -249,49 +253,32 @@
             bias_init=initializers.constant(0.),
             use_bias=True,
         )
     )
     self.w_xs = w_xs
 
   @staticmethod
-  def _compute_gaussian_map(
-      inputs: Tuple[jnp.ndarray, jnp.ndarray]
+  def _compute_gaussian_map_params(
+      samples: Tuple[jnp.ndarray, jnp.ndarray]
   ) -> Tuple[jnp.ndarray, jnp.ndarray]:
-
-    def compute_moments(x, reg=1e-4, sqrt_inv=False):
-      shape = x.shape
-      z = x.reshape(shape[0], -1)
-      mu = jnp.expand_dims(jnp.mean(z, axis=0), 0)
-      z = z - mu
-      matmul = lambda a, b: jnp.matmul(a, b)
-      sigma = jax.vmap(matmul)(jnp.expand_dims(z, 2), jnp.expand_dims(z, 1))
-      # unbiased estimate
-      sigma = jnp.sum(sigma, axis=0) / (shape[0] - 1)
-      # regularize
-      sigma = sigma + reg * jnp.eye(shape[1])
-
-      if sqrt_inv:
-        sigma_sqrt, sigma_inv_sqrt, _ = matrix_square_root.sqrtm(sigma)
-        return sigma, sigma_sqrt, sigma_inv_sqrt, mu
-      return sigma, mu
-
-    source, target = inputs
-    _, covs_sqrt, covs_inv_sqrt, mus = compute_moments(source, sqrt_inv=True)
-    covt, mut = compute_moments(target, sqrt_inv=False)
-
-    mo = matrix_square_root.sqrtm_only(
-        jnp.dot(jnp.dot(covs_sqrt, covt), covs_sqrt)
-    )
-    A = jnp.dot(jnp.dot(covs_inv_sqrt, mo), covs_inv_sqrt)
-    b = jnp.squeeze(mus) - jnp.linalg.solve(A, jnp.squeeze(mut))
-    A = matrix_square_root.sqrtm_only(A)
-    return jnp.expand_dims(A, 0), jnp.expand_dims(b, 0)
+    from ott.tools.gaussian_mixture import gaussian
+    source, target = samples
+    # print(source)
+    # print(type(source))
+    g_s = gaussian.Gaussian.from_samples(source)
+    g_t = gaussian.Gaussian.from_samples(target)
+    lin_op = g_s.scale.gaussian_map(g_t.scale)
+    b = jnp.squeeze(g_t.loc) - jnp.linalg.solve(lin_op, jnp.squeeze(g_t.loc))
+    lin_op = matrix_square_root.sqrtm_only(lin_op)
+    return jnp.expand_dims(lin_op, 0), jnp.expand_dims(b, 0)
 
   @staticmethod
-  def _compute_identity_map(input_dim: int) -> Tuple[jnp.ndarray, jnp.ndarray]:
+  def _compute_identity_map_params(
+      input_dim: int
+  ) -> Tuple[jnp.ndarray, jnp.ndarray]:
     A = jnp.eye(input_dim).reshape((1, input_dim, input_dim))
     b = jnp.zeros((1, input_dim))
     return A, b
 
   @nn.compact
   def __call__(self, x: jnp.ndarray) -> float:  # noqa: D102
     z = self.act_fn(self.w_xs[0](x))
```

### Comparing `ott-jax-0.4.2/src/ott/solvers/nn/neuraldual.py` & `ott-jax-0.4.3/src/ott/solvers/nn/neuraldual.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/quadratic/__init__.py` & `ott-jax-0.4.3/src/ott/solvers/quadratic/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/quadratic/gromov_wasserstein.py` & `ott-jax-0.4.3/src/ott/solvers/quadratic/gromov_wasserstein.py`

 * *Files 6% similar despite different names*

```diff
@@ -160,21 +160,16 @@
 
   Args:
     args: Positional arguments for
       :class:`~ott.solvers.was_solver.WassersteinSolver`.
     warm_start: Whether to initialize (low-rank) Sinkhorn calls using values
       from the previous iteration. If `None`, warm starts are not used for
       standard Sinkhorn, but used for low-rank Sinkhorn.
-    unscale_last_linearization: Whether to remove any scaling from the
-      cost matrices of the last linearization stored in
-      :attr:`~ott.solvers.quadratic.gromov_wasserstein.GWOutput.geom`.
-      This has the practical benefit that, while the OT coupling matrices
-      obtained with GW might have been computed by re-scaling cost matrices for
-      numerical stability, the last linearization stored in the geometry will be
-      unscaled and recomputed with the original cost values.
+    relative_epsilon: Whether to use relative epsilon in the linearized
+      geometry.
     quad_initializer: Quadratic initializer. If the solver is entropic,
       :class:`~ott.initializers.quadratic.initializers.QuadraticInitializer`
       is always used. Otherwise, the quadratic initializer wraps the low-rank
       Sinkhorn initializers. If `None`, the low-rank initializer will be
       selected in a problem-specific manner. If both ``geom_xx`` and ``geom_yy``
       are :class:`~ott.geometry.pointcloud.PointCloud` or
       :class:`~ott.geometry.low_rank.LRCGeometry`, use
@@ -190,25 +185,25 @@
       :class:`~ott.solvers.was_solver.WassersteinSolver`.
   """
 
   def __init__(
       self,
       *args: Any,
       warm_start: Optional[bool] = None,
-      unscale_last_linearization: bool = False,
+      relative_epsilon: Optional[bool] = None,
       quad_initializer: Optional[
           Union[Literal["random", "rank2", "k-means", "generalized-k-means"],
                 quad_initializers.BaseQuadraticInitializer]] = None,
       progress_fn: Optional[ProgressCallbackFn_t] = None,
       kwargs_init: Optional[Mapping[str, Any]] = None,
       **kwargs: Any
   ):
     super().__init__(*args, **kwargs)
     self._warm_start = warm_start
-    self.unscale_last_linearization = unscale_last_linearization
+    self.relative_epsilon = relative_epsilon
     self.quad_initializer = quad_initializer
     self.progress_fn = progress_fn
     self.kwargs_init = {} if kwargs_init is None else kwargs_init
 
   def __call__(
       self,
       prob: quadratic_problem.QuadraticProblem,
@@ -232,29 +227,35 @@
     rng1, rng2 = jax.random.split(rng, 2)
 
     if prob._is_low_rank_convertible:
       prob = prob.to_low_rank()
 
     if init is None:
       initializer = self.create_initializer(prob)
-      init = initializer(prob, epsilon=self.epsilon, rng=rng1, **kwargs)
+      init = initializer(
+          prob,
+          epsilon=self.epsilon,
+          rng=rng1,
+          relative_epsilon=self.relative_epsilon,
+          **kwargs
+      )
 
     out = iterations(self, prob, init, rng2)
     # TODO(lpapaxanthoos): remove stop_gradient when using backprop
     if self.is_low_rank:
       linearization = prob.update_lr_linearization(
           jax.lax.stop_gradient(out.linear_state),
-          remove_scale=self.unscale_last_linearization
+          relative_epsilon=self.relative_epsilon,
       )
     else:
       linearization = prob.update_linearization(
           jax.lax.stop_gradient(out.linear_state),
           epsilon=self.epsilon,
           old_transport_mass=jax.lax.stop_gradient(out.old_transport_mass),
-          remove_scale=self.unscale_last_linearization,
+          relative_epsilon=self.relative_epsilon,
       )
 
     linear_state = out.linear_state.set_cost(linearization, True, True)
     iteration = jnp.sum(out.costs != -1)
     converged = jnp.logical_and(
         iteration < self.max_iterations, jnp.all(out.linear_convergence)
     )
@@ -362,15 +363,15 @@
     """Whether to initialize (low-rank) Sinkhorn using previous solutions."""
     return self.is_low_rank if self._warm_start is None else self._warm_start
 
   def tree_flatten(self) -> Tuple[Sequence[Any], Dict[str, Any]]:  # noqa: D102
     children, aux_data = super().tree_flatten()
     aux_data["warm_start"] = self._warm_start
     aux_data["progress_fn"] = self.progress_fn
-    aux_data["unscale_last_linearization"] = self.unscale_last_linearization
+    aux_data["relative_epsilon"] = self.relative_epsilon
     aux_data["quad_initializer"] = self.quad_initializer
     aux_data["kwargs_init"] = self.kwargs_init
     return children, aux_data
 
 
 def iterations(
     solver: GromovWasserstein,
@@ -392,20 +393,25 @@
     del compute_error  # always assumed true for the outer loop of GW
 
     lin_state = state.linear_state
     if solver.is_low_rank:
       rng = state.rngs[iteration]
       init = (lin_state.q, lin_state.r,
               lin_state.g) if solver.warm_start else (None, None, None)
-      linear_pb = prob.update_lr_linearization(state.linear_state)
+      linear_pb = prob.update_lr_linearization(
+          state.linear_state, relative_epsilon=solver.relative_epsilon
+      )
       out = solver.linear_ot_solver(linear_pb, init=init, rng=rng)
     else:
       init = (lin_state.f, lin_state.g) if solver.warm_start else (None, None)
       linear_pb = prob.update_linearization(
-          lin_state, solver.epsilon, state.old_transport_mass
+          lin_state,
+          solver.epsilon,
+          state.old_transport_mass,
+          relative_epsilon=solver.relative_epsilon,
       )
       out = solver.linear_ot_solver(linear_pb, init=init)
 
     old_transport_mass = jax.lax.stop_gradient(
         state.linear_state.transport_mass
     )
     new_state = state.update(
```

### Comparing `ott-jax-0.4.2/src/ott/solvers/quadratic/gw_barycenter.py` & `ott-jax-0.4.3/src/ott/solvers/quadratic/gw_barycenter.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/solvers/was_solver.py` & `ott-jax-0.4.3/src/ott/solvers/was_solver.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/__init__.py` & `ott-jax-0.4.3/src/ott/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/__init__.py` & `ott-jax-0.4.3/src/ott/tools/gaussian_mixture/__init__.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/fit_gmm.py` & `ott-jax-0.4.3/src/ott/tools/gaussian_mixture/fit_gmm.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/fit_gmm_pair.py` & `ott-jax-0.4.3/src/ott/tools/gaussian_mixture/fit_gmm_pair.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian.py` & `ott-jax-0.4.3/src/ott/tools/gaussian_mixture/gaussian.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian_mixture.py` & `ott-jax-0.4.3/src/ott/tools/gaussian_mixture/gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py` & `ott-jax-0.4.3/src/ott/tools/gaussian_mixture/gaussian_mixture_pair.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/linalg.py` & `ott-jax-0.4.3/src/ott/tools/gaussian_mixture/linalg.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/probabilities.py` & `ott-jax-0.4.3/src/ott/tools/gaussian_mixture/probabilities.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/gaussian_mixture/scale_tril.py` & `ott-jax-0.4.3/src/ott/tools/gaussian_mixture/scale_tril.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/k_means.py` & `ott-jax-0.4.3/src/ott/tools/k_means.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/map_estimator.py` & `ott-jax-0.4.3/src/ott/tools/map_estimator.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/plot.py` & `ott-jax-0.4.3/src/ott/tools/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 from typing import List, Optional, Sequence, Tuple, Union
 
 import jax.numpy as jnp
 import numpy as np
 import scipy
 
-from ott import utils
 from ott.geometry import pointcloud
 from ott.solvers.linear import sinkhorn, sinkhorn_lr
 from ott.solvers.quadratic import gromov_wasserstein
 
 try:
   import matplotlib.pyplot as plt
   from matplotlib import animation
@@ -35,43 +34,62 @@
 
 def bidimensional(x: jnp.ndarray,
                   y: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
   """Apply PCA to reduce to bi-dimensional data."""
   if x.shape[1] < 3:
     return x, y
 
-  u, s, _ = scipy.sparse.linalg.svds(jnp.concatenate([x, y], axis=0), k=2)
+  u, s, _ = scipy.sparse.linalg.svds(
+      np.array(jnp.concatenate([x, y], axis=0)), k=2
+  )
   proj = u * s
   k = x.shape[0]
   return proj[:k], proj[k:]
 
 
 class Plot:
   """Plot an optimal transport map between two point clouds.
 
-  It enables to either plot or update a plot in a single object, offering the
-  possibilities to create animations as a
+  This object can either plot or update a plot, to create animations as a
   :class:`~matplotlib.animation.FuncAnimation`, which can in turned be saved to
   disk at will. There are two design principles here:
 
   #. we do not rely on saving to/loading from disk to create animations
   #. we try as much as possible to disentangle the transport problem from
      its visualization.
+
+  We use 2D scatter plots by default, relying on PCA visualization for d>3 data.
+  This step requires a conversion to a numpy array, in order to compute leading
+  singular values. This tool is therefore not designed having performance in
+  mind.
+
+  Args:
+    fig: Specify figure object. Created by default
+    ax: Specify axes objects. Created by default
+    threshold: value below which links in transportation matrix won't be
+      plotted. This value should be negative when using animations.
+    scale: scale used for marker plots.
+    show_lines: whether to show OT lines, as described in ``ot.matrix`` argument
+    cmap: color map used to plot line colors.
+    scale_alpha_by_coupling: use or not the coupling's value as proxy for alpha
+    alpha: default alpha value for lines.
+    title: title of the plot.
   """
 
   def __init__(
       self,
       fig: Optional["plt.Figure"] = None,
       ax: Optional["plt.Axes"] = None,
-      cost_threshold: float = -1.0,  # should be negative for animations.
+      threshold: float = -1.0,
       scale: int = 200,
       show_lines: bool = True,
       cmap: str = "cool",
       scale_alpha_by_coupling: bool = False,
       alpha: float = 0.7,
+      title: Optional[str] = None
   ):
     if plt is None:
       raise RuntimeError("Please install `matplotlib` first.")
 
     if ax is None and fig is None:
       fig, ax = plt.subplots()
     elif fig is None:
@@ -80,19 +98,20 @@
       ax = plt.gca()
     self.fig = fig
     self.ax = ax
     self._show_lines = show_lines
     self._lines = []
     self._points_x = None
     self._points_y = None
-    self._threshold = cost_threshold
+    self._threshold = threshold
     self._scale = scale
     self._cmap = cmap
     self._scale_alpha_by_coupling = scale_alpha_by_coupling
     self._alpha = alpha
+    self._title = title
 
   def _scatter(self, ot: Transport):
     """Compute the position and scales of the points on a 2D plot."""
     if not isinstance(ot.geom, pointcloud.PointCloud):
       raise ValueError("So far we only plot PointCloud geometry.")
 
     x, y = ot.geom.x, ot.geom.y
@@ -131,15 +150,15 @@
 
       start, end = xy[i, [0, 2]], xy[i, [1, 3]]
       result.append((start, end, strength, alpha))
 
     return result
 
   def __call__(self, ot: Transport) -> List["plt.Artist"]:
-    """Plot 2-D couplings. Projects via PCA if data is higher dimensional."""
+    """Plot couplings in 2-D, using PCA if data is higher dimensional."""
     x, y, sx, sy = self._scatter(ot)
     self._points_x = self.ax.scatter(
         *x.T, s=sx, edgecolors="k", marker="o", label="x"
     )
     self._points_y = self.ax.scatter(
         *y.T, s=sy, edgecolors="k", marker="X", label="y"
     )
@@ -156,17 +175,21 @@
           end,
           linewidth=0.5 + 4 * strength,
           color=cmap(strength),
           zorder=0,
           alpha=alpha
       )
       self._lines.append(line)
+    if self._title is not None:
+      self.ax.set_title(self._title)
     return [self._points_x, self._points_y] + self._lines
 
-  def update(self, ot: Transport) -> List["plt.Artist"]:
+  def update(self,
+             ot: Transport,
+             title: Optional[str] = None) -> List["plt.Artist"]:
     """Update a plot with a transport instance."""
     x, y, _, _ = self._scatter(ot)
     self._points_x.set_offsets(x)
     self._points_y.set_offsets(y)
     if not self._show_lines:
       return []
 
@@ -193,68 +216,32 @@
           color=cmap(strength),
           zorder=0,
           alpha=alpha
       )
       self._lines.append(line)
 
     self._lines = self._lines[:num_to_plot]  # Maybe remove some
+    if title is not None:
+      self.ax.set_title(title)
     return [self._points_x, self._points_y] + self._lines
 
   def animate(
       self,
       transports: Sequence[Transport],
+      titles: Optional[Sequence[str]] = None,
       frame_rate: float = 10.0
   ) -> "animation.FuncAnimation":
     """Make an animation from several transports."""
     _ = self(transports[0])
+    if titles is None:
+      titles = [None for _ in np.arange(0, len(transports))]
+    assert len(titles) == len(transports), (
+        f"titles/transports lengths differ `{len(titles)}`/`{len(transports)}`."
+    )
     return animation.FuncAnimation(
         self.fig,
-        lambda i: self.update(transports[i]),
+        lambda i: self.update(transports[i], titles[i]),
         np.arange(0, len(transports)),
-        init_func=lambda: self.update(transports[0]),
+        init_func=lambda: self.update(transports[0], titles[0]),
         interval=1000 / frame_rate,
         blit=True
     )
-
-
-def _barycenters(
-    ax: "plt.Axes",
-    y: jnp.ndarray,
-    a: jnp.ndarray,
-    b: jnp.ndarray,
-    matrix: jnp.ndarray,
-    scale: int = 200
-) -> None:
-  """Plot 2-D sinkhorn barycenters."""
-  sa, sb = jnp.min(a) / scale, jnp.min(b) / scale
-  ax.scatter(*y.T, s=b / sb, edgecolors="k", marker="X", label="y")
-  tx = 1 / a[:, None] * jnp.matmul(matrix, y)
-  ax.scatter(*tx.T, s=a / sa, edgecolors="k", marker="X", label="T(x)")
-  ax.legend(fontsize=15)
-
-
-def barycentric_projections(
-    arg: Union[Transport, jnp.ndarray],
-    a: jnp.ndarray = None,
-    b: jnp.ndarray = None,
-    matrix: jnp.ndarray = None,
-    ax: Optional["plt.Axes"] = None,
-    **kwargs
-):
-  """Plot the barycenters, from the Transport object or from arguments."""
-  if ax is None:
-    _, ax = plt.subplots(1, 1, figsize=(8, 5))
-
-  if utils.is_jax_array(arg):
-    if matrix is None:
-      raise ValueError("The `matrix` argument cannot be None.")
-
-    a = jnp.ones(matrix.shape[0]) / matrix.shape[0] if a is None else a
-    b = jnp.ones(matrix.shape[1]) / matrix.shape[1] if b is None else b
-    return _barycenters(ax, arg, a, b, matrix, **kwargs)
-
-  if isinstance(arg, gromov_wasserstein.GWOutput):
-    geom = arg.linear_state.geom
-  else:
-    geom = arg.geom
-
-  return _barycenters(ax, geom.y, arg.a, arg.b, arg.matrix, **kwargs)
```

### Comparing `ott-jax-0.4.2/src/ott/tools/segment_sinkhorn.py` & `ott-jax-0.4.3/src/ott/tools/segment_sinkhorn.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/sinkhorn_divergence.py` & `ott-jax-0.4.3/src/ott/tools/sinkhorn_divergence.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/tools/soft_sort.py` & `ott-jax-0.4.3/src/ott/tools/soft_sort.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import functools
-from typing import Any, Callable, Optional, Union
+from typing import Any, Callable, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 from ott.geometry import pointcloud
 from ott.problems.linear import linear_problem
 from ott.solvers.linear import sinkhorn
 
-__all__ = ["sort", "ranks", "quantile"]
+__all__ = [
+    "sort", "ranks", "sort_with", "quantile", "quantile_normalization",
+    "quantize", "topk_mask"
+]
 
 
 def transport_for_sort(
     inputs: jnp.ndarray,
     weights: Optional[jnp.ndarray] = None,
     target_weights: Optional[jnp.ndarray] = None,
     squashing_fun: Optional[Callable[[jnp.ndarray], jnp.ndarray]] = None,
@@ -78,15 +81,15 @@
 def apply_on_axis(op, inputs, axis, *args, **kwargs: Any) -> jnp.ndarray:
   """Apply a differentiable operator on a given axis of the input.
 
   Args:
     op: a differentiable operator (can be ranks, quantile, etc.)
     inputs: Array of any shape.
     axis: the axis (int) or tuple of ints on which to apply the operator. If
-      several axes are passed the operator, those are merged as a single
+      several axes are passed to the operator, those are merged as a single
       dimension.
     args: other positional arguments to the operator.
     kwargs: other positional arguments to the operator.
 
   Returns:
     An Array holding the output of the differentiable operator on the given
     axis.
@@ -148,139 +151,205 @@
   For instance:
 
   .. code-block:: python
 
     x = jax.random.uniform(rng, (100,))
     x_sorted = sort(x)
 
-
   will output sorted convex-combinations of values contained in ``x``, that are
   differentiable approximations to the sorted vector of entries in ``x``.
   These can be compared with the values produced by :func:`jax.numpy.sort`,
 
   .. code-block:: python
 
     x_sorted = jax.numpy.sort(x)
 
-
   Args:
     inputs: Array of any shape.
     axis: the axis on which to apply the soft-sorting operator.
     topk: if set to a positive value, the returned vector will only contain
       the top-k values. This also reduces the complexity of soft-sorting, since
       the number of target points to which the slice of the ``inputs`` tensor
-      will be mapped to will be equal to ``topk+1``.
-    num_targets: if ``topk`` is not specified, ``num_targets`` defines the
-      number of (composite) sorted values computed from the inputs (each value
-      is a convex combination of values recorded in the inputs, provided in
-      increasing order). If neither ``topk`` nor ``num_targets`` are specified,
-      ``num_targets`` defaults to the size of the slices of the input that are
-      sorted, i.e. ``inputs.shape[axis]``, and the number of composite sorted
-      values is equal to the slice of the inputs that are sorted.
+      will be mapped to will be equal to ``topk + 1``.
+    num_targets: if ``topk`` is not specified, a vector of size``num_targets``
+      is returned. This defines the number of (composite) sorted values computed
+      from the inputs (each value is a convex combination of values recorded in
+      the inputs, provided in increasing order). If neither ``topk`` nor
+      ``num_targets`` are specified, ``num_targets`` defaults to the size of the
+      slices of the input that are sorted, i.e. ``inputs.shape[axis]``, and the
+      number of composite sorted values is equal to the slice of the inputs that
+      are sorted. As a result, the output is of the same size as ``inputs``.
     kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
       ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
       to solve the optimal transport problem;
-      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
+      :class:`cost_fn <ott.geometry.costs.CostFn>` object of
       :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
-      cost function to transport from ``inputs`` to the ``num_targets`` target
-      values ; ``epsilon`` regularization
-      parameter. Remaining ``kwargs`` are passed on to defined the
+      1D cost function to transport from ``inputs`` to the ``num_targets``
+      target values; ``epsilon`` regularization parameter. Remaining ``kwargs``
+      are passed on to parameterize the
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
   Returns:
-    An Array of the same shape as the input with soft-sorted values on the
-    given axis.
+    An Array of the same shape as the input, except on ``axis``, where that size
+    will be equal to ``topk`` or ``num_targets``, with soft-sorted values on the
+    given axis. Same size as ``inputs`` if both these parameters are ``None``.
   """
   return apply_on_axis(_sort, inputs, axis, topk, num_targets, **kwargs)
 
 
-def _ranks(inputs: jnp.ndarray, num_targets, **kwargs: Any) -> jnp.ndarray:
+def _ranks(
+    inputs: jnp.ndarray, num_targets, target_weights, **kwargs: Any
+) -> jnp.ndarray:
   """Apply the soft ranks operator on a one dimensional array."""
   num_points = inputs.shape[0]
-  num_targets = num_points if num_targets is None else num_targets
+  if target_weights is None:
+    num_targets = num_points if num_targets is None else num_targets
+    target_weights = jnp.ones((num_targets,)) / num_targets
+  else:
+    num_targets = target_weights.shape[0]
   a = jnp.ones((num_points,)) / num_points
-  b = jnp.ones((num_targets,)) / num_targets
-  ot = transport_for_sort(inputs, a, b, **kwargs)
+  ot = transport_for_sort(inputs, a, target_weights, **kwargs)
   out = 1.0 / a * ot.apply(jnp.arange(num_targets), axis=1)
+  out *= (num_points - 1.0) / (num_targets - 1.0)
   return jnp.reshape(out, inputs.shape)
 
 
 def ranks(
     inputs: jnp.ndarray,
     axis: int = -1,
     num_targets: Optional[int] = None,
+    target_weights: Optional[jnp.ndarray] = None,
     **kwargs: Any,
 ) -> jnp.ndarray:
   r"""Apply the soft rank operator on input tensor.
 
   For instance:
 
   .. code-block:: python
 
     x = jax.random.uniform(rng, (100,))
     x_ranks = ranks(x)
 
-  will output fractional values, between 0 and 1, that are differentiable
-  approximations to the normalized ranks of entries in ``x``. These should be
-  compared to the non-differentiable rank vectors, namely the normalized inverse
-  permutation produced by :func:`jax.numpy.argsort`, which can be obtained as:
+  will output values that are differentiable approximations to the ranks of
+  entries in ``x``. These should be compared to the non-differentiable rank
+  vectors, namely the normalized inverse permutation produced by
+  :func:`jax.numpy.argsort`, which can be obtained as:
 
   .. code-block:: python
 
-    x_ranks = jax.numpy.argsort(jax.numpy.argsort(x)) / x.shape[0]
+    x_ranks = jax.numpy.argsort(jax.numpy.argsort(x))
 
   Args:
     inputs: Array of any shape.
     axis: the axis on which to apply the soft-sorting operator.
-    topk: if set to a positive value, the returned vector will only contain
-      the top-k values. This also reduces the complexity of soft-sorting, since
-      the number of target points to which the slice of the ``inputs`` tensor
-      will be mapped to will be equal to ``topk+1``.
-    num_targets: if ``topk`` is not specified, ``num_targets`` defines the
-      number of (composite) sorted values computed from the inputs (each value
-      is a convex combination of values recorded in the inputs, provided in
-      increasing order). If neither ``topk`` nor ``num_targets`` are specified,
-      ``num_targets`` defaults to the size of the slices of the input that are
-      sorted, i.e. ``inputs.shape[axis]``, and the number of composite sorted
-      values is equal to the slice of the inputs that are sorted.
+    target_weights: This vector contains weights (summing to 1) that describe
+      amount of mass shipped to targets.
+    num_targets: If ``target_weights`  is ``None``, ``num_targets`` is
+      considered to define the number of targets used to rank inputs. Each
+      rank in the output will be a convex combination of
+      ``{1, .., num_targets}``. The weight of each of these points
+      is assumed to be uniform. If neither ``num_targets`` nor
+      ``target_weights`` are specified, ``num_targets`` defaults to the size
+      of the slices of the input that are sorted, i.e. ``inputs.shape[axis]``.
     kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
       ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
       to solve the optimal transport problem;
-      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
+      :class:`cost_fn <ott.geometry.costs.CostFn>` object of
       :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
-      cost function to transport from ``inputs`` to the ``num_targets`` target
-      values ; ``epsilon`` regularization
-      parameter. Remaining ``kwargs`` are passed on to defined the
+      1D cost function to transport from ``inputs`` to the ``num_targets``
+      target values; ``epsilon`` regularization parameter. Remaining ``kwargs``
+      are passed on to parameterize the
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
   Returns:
     An Array of the same shape as the input with soft-rank values
-    normalized to be in :math:`[0,1]`, replacing the original ones.
+    normalized to be in :math:`[0, n-1]` where :math:`n` is
+    ``inputs.shape[axis]``.
+  """
+  return apply_on_axis(
+      _ranks, inputs, axis, num_targets, target_weights, **kwargs
+  )
+
 
+def topk_mask(
+    inputs: jnp.ndarray,
+    axis: int = -1,
+    k: int = 1,
+    **kwargs: Any,
+) -> jnp.ndarray:
+  r"""Soft :math:`\text{top-}k` selection mask.
+
+  For instance:
+
+  .. code-block:: python
+
+    k = 5
+    x = jax.random.uniform(rng, (100,))
+    mask = topk_mask(x, k=k)
+
+  will output a vector of shape ``x.shape``, with values in :math:`[0,1]`, that
+  are differentiable approximations to the binary mask selecting the top $k$
+  entries in ``x``. These should be compared to the non-differentiable mask
+  obtained with :func:`jax.numpy.sort`, which can be obtained as:
+
+  .. code-block:: python
+
+    mask = x >= jax.numpy.sort(x).flip()[k-1]
+
+  Args:
+    inputs: Array of any shape.
+    axis: the axis on which to apply the soft-sorting operator.
+    k: topk parameter. Should be smaller than ``inputs.shape[axis]``.
+    kwargs: keyword arguments passed on to lower level functions. Of interest
+      to the user are ``squashing_fun``, which will redistribute the values in
+      ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
+      to solve the optimal transport problem;
+      :class:`cost_fn <ott.geometry.costs.CostFn>` object of
+      :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
+      1D cost function to transport from ``inputs`` to the ``num_targets``
+      target values; ``epsilon`` regularization parameter. Remaining ``kwargs``
+      are passed on to parameterize the
+      :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
+
+  Returns:
+    The soft :math:`\text{top-}k` selection mask.
   """
-  return apply_on_axis(_ranks, inputs, axis, num_targets, **kwargs)
+  num_points = inputs.shape[axis]
+  assert k < num_points, (
+      f"`k` must be smaller than `inputs.shape[axis]`, yet {k} >= {num_points}."
+  )
+  target_weights = jnp.array([1.0 - k / num_points, k / num_points])
+  out = apply_on_axis(
+      _ranks,
+      inputs,
+      axis,
+      num_targets=None,
+      target_weights=target_weights,
+      **kwargs
+  )
+  return out / (num_points - 1)
 
 
 def quantile(
     inputs: jnp.ndarray,
-    q: jnp.ndarray,
-    axis: int = -1,
+    q: Optional[Union[float, jnp.ndarray]],
+    axis: Union[int, Tuple[int, ...]] = -1,
     weight: Optional[Union[float, jnp.ndarray]] = None,
     **kwargs: Any,
 ) -> jnp.ndarray:
   r"""Apply the soft quantiles operator on the input tensor.
 
   For instance:
 
   .. code-block:: python
 
     x = jax.random.uniform(rng, (100,))
-    x_quantiles = quantiles(x, q=jnp.array([0.2, 0.8]))
+    x_quantiles = quantile(x, q=jnp.array([0.2, 0.8]))
 
   ``x_quantiles`` will hold an approximation to the 20 and 80 percentiles in
   ``x``, computed as a convex combination (a weighted mean, with weights summing
   to 1) of all values in ``x`` (and not, as for standard quantiles, the
   values ``x_sorted[20]`` and ``x_sorted[80]`` if ``x_sorted=jnp.sort(x)``).
   These values offer a trade-off between accuracy (closeness to the true
   percentiles) and gradient (the Jacobian of ``x_quantiles`` w.r.t ``x`` will
@@ -288,36 +357,35 @@
 
   The non-differentiable version is given by :func:`jax.numpy.quantile`, e.g.
 
   .. code-block:: python
 
     x_quantiles = jax.numpy.quantile(x, q=jnp.array([0.2, 0.8]))
 
-
   Args:
    inputs: an Array of any shape.
    q: values of the quantile level to be computed, e.g. [0.5] for median.
      These values should all lie in :math:`[0,1]`.
    axis: the axis on which to apply the operator.
    weight: the weight assigned to each quantile target value in the OT problem.
-    This weight should be small, typically of the order of ``1/n``, where ``n``
-    is the size of ``x``. Note: Since the size of ``q`` times ``weight``
-    must be strictly smaller than ``1``, in order to leave enough mass to set
-    other target values in the transport problem, the algorithm might ensure
-    this by setting, when needed, a lower value.
+     This weight should be small, typically of the order of ``1/n``, where ``n``
+     is the size of ``x``. Note: Since the size of ``q`` times ``weight``
+     must be strictly smaller than ``1``, in order to leave enough mass to set
+     other target values in the transport problem, the algorithm might ensure
+     this by setting, when needed, a lower value.
    kwargs: keyword arguments passed on to lower level functions. Of interest
-      to the user are ``squashing_fun``, which will redistribute the values in
-      ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
-      to solve the optimal transport problem;
-      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
-      :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
-      cost function to transport from ``inputs`` to the ``num_targets`` target
-      values ; ``epsilon`` regularization
-      parameter. Remaining ``kwargs`` are passed on to defined the
-      :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
+     to the user are ``squashing_fun``, which will redistribute the values in
+     ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
+     to solve the optimal transport problem;
+     :class:`cost_fn <ott.geometry.costs.CostFn>` object of
+     :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
+     1D cost function to transport from ``inputs`` to the ``num_targets``
+     target values; ``epsilon`` regularization parameter. Remaining ``kwargs``
+     are passed on to parameterize the
+     :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
   Returns:
     An Array, which has the same shape as ``inputs``, except on the ``axis``
     that is passed, which has size ``q.shape[0]``, to collect soft-quantile
     values.
   """
 
@@ -368,19 +436,19 @@
         jnp.stack([filler_weights, quantile_weights], axis=1), (-1,)
     )[:-1]
 
     ot = transport_for_sort(inputs, a, weights, **kwargs)
     out = 1.0 / weights * ot.apply(jnp.squeeze(inputs), axis=0)
 
     # Recover odd indices corresponding to the desired quantiles.
-    odds = jnp.concatenate([
-        jnp.zeros((num_quantiles + 1, 1), dtype=bool),
-        jnp.ones((num_quantiles + 1, 1), dtype=bool)
+    odds = np.concatenate([
+        np.zeros((num_quantiles + 1, 1), dtype=bool),
+        np.ones((num_quantiles + 1, 1), dtype=bool)
     ],
-                           axis=1).ravel()[:-1]
+                          axis=1).ravel()[:-1]
     return out[odds][idx]
 
   return apply_on_axis(_quantile, inputs, axis, q, weight, **kwargs)
 
 
 def _quantile_normalization(
     inputs: jnp.ndarray, targets: jnp.ndarray, weights: float, **kwargs: Any
@@ -393,42 +461,42 @@
 
 
 def quantile_normalization(
     inputs: jnp.ndarray,
     targets: jnp.ndarray,
     weights: Optional[jnp.ndarray] = None,
     axis: int = -1,
-    **kwargs
+    **kwargs: Any,
 ) -> jnp.ndarray:
-  r"""Renormalize inputs so that its quantiles match those of targets/weights.
+  r"""Re-normalize inputs so that its quantiles match those of targets/weights.
 
   Quantile normalization rearranges the values in inputs to values that match
   the distribution of values described in the discrete distribution ``targets``
   weighted by ``weights``. This transformation preserves the order of values
   in ``inputs`` along the specified ``axis``.
 
   Args:
     inputs: array of any shape whose values will be changed to match those in
       ``targets``.
     targets: sorted array (in ascending order) of dimension 1 describing a
       discrete distribution. Note: the ``targets`` values must be provided as
       a sorted vector.
-    weights: vector of nonnegative weights, summing to :math:`1`, of the same
+    weights: vector of non-negative weights, summing to :math:`1`, of the same
       size as ``targets``. When not set, this defaults to the uniform
       distribution.
     axis: the axis along which the quantile transformation is applied.
     kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
       ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
       to solve the optimal transport problem;
-      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
+      :class:`cost_fn <ott.geometry.costs.CostFn>` object of
       :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
-      cost function to transport from ``inputs`` to the ``num_targets`` target
-      values ; ``epsilon`` regularization
-      parameter. Remaining ``kwargs`` are passed on to defined the
+      1D cost function to transport from ``inputs`` to the ``num_targets``
+      target values; ``epsilon`` regularization parameter. Remaining ``kwargs``
+      are passed on to parameterize the
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
   Returns:
     An array, which has the same shape as the input, except on the give axis on
     which the dimension is 1.
 
   Raises:
@@ -469,19 +537,19 @@
     criterion: the values according to which to sort the inputs. It has shape
       [batch, 1].
     topk: The number of outputs to keep.
     kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
       ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
       to solve the optimal transport problem;
-      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
+      :class:`cost_fn <ott.geometry.costs.CostFn>` object of
       :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
-      cost function to transport from ``inputs`` to the ``num_targets`` target
-      values ; ``epsilon`` regularization
-      parameter. Remaining ``kwargs`` are passed on to defined the
+      1D cost function to transport from ``inputs`` to the ``num_targets``
+      target values; ``epsilon`` regularization parameter. Remaining ``kwargs``
+      are passed on to parameterize the
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
   Returns:
     An Array of size [batch | topk, dim].
   """
   num_points = criterion.shape[0]
   weights = jnp.ones(num_points, dtype=criterion.dtype) / num_points
@@ -515,15 +583,15 @@
 
 def quantize(
     inputs: jnp.ndarray,
     num_levels: int = 10,
     axis: int = -1,
     **kwargs: Any,
 ) -> jnp.ndarray:
-  r"""Soft quantizes an input according using num_levels values along axis.
+  r"""Soft quantizes an input according using ``num_levels`` values along axis.
 
   The quantization operator consists in concentrating several values around
   a few predefined ``num_levels``. The soft quantization operator proposed here
   does so by carrying out a `soft` concentration that is differentiable. The
   ``inputs`` values are first soft-sorted, resulting in ``num_levels`` values.
   In a second step, the ``inputs`` values are then provided again a composite
   value that is equal (for each) to a convex combination of those soft-sorted
@@ -537,19 +605,18 @@
     inputs: an Array of size [batch, dim].
     num_levels: number of quantiles available to quantize the signal.
     axis: axis along which quantization is carried out.
     kwargs: keyword arguments passed on to lower level functions. Of interest
       to the user are ``squashing_fun``, which will redistribute the values in
       ``inputs`` to lie in :math:`[0,1]` (sigmoid of whitened values by default)
       to solve the optimal transport problem;
-      attribute :class:`cost_fn <ott.geometry.costs.CostFn>` of
+      :class:`cost_fn <ott.geometry.costs.CostFn>` object of
       :class:`~ott.geometry.pointcloud.PointCloud`, which defines the ground
-      cost function to transport from ``inputs`` to the ``num_targets`` target
-      values ; ``epsilon`` regularization
-      parameter. Remaining ``kwargs`` are passed on to defined the
+      1D cost function to transport from ``inputs`` to the ``num_targets``
+      target values; ``epsilon`` regularization parameter. Remaining ``kwargs``
+      are passed on to parameterize the
       :class:`~ott.solvers.linear.sinkhorn.Sinkhorn` solver.
 
-
   Returns:
     An Array of the same size as ``inputs``.
   """
   return apply_on_axis(_quantize, inputs, axis, num_levels, **kwargs)
```

### Comparing `ott-jax-0.4.2/src/ott/types.py` & `ott-jax-0.4.3/src/ott/types.py`

 * *Files identical despite different names*

### Comparing `ott-jax-0.4.2/src/ott/utils.py` & `ott-jax-0.4.3/src/ott/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from typing import Any, Callable, NamedTuple, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 __all__ = [
-    "register_pytree_node", "deprecate", "is_jax_array", "default_progress_fn"
+    "register_pytree_node", "deprecate", "is_jax_array", "default_prng_key",
+    "default_progress_fn"
 ]
 
 
 def register_pytree_node(cls: type) -> type:
   """Register dataclasses as pytree_nodes."""
   cls = dataclasses.dataclass()(cls)
   flatten = lambda obj: jax.tree_flatten(dataclasses.asdict(obj))
@@ -56,26 +57,25 @@
   return functools.wraps(func)(wrapper)
 
 
 def is_jax_array(obj: Any) -> bool:
   """Check if an object is a Jax array."""
   if hasattr(jax, "Array"):
     # https://jax.readthedocs.io/en/latest/jax_array_migration.html
-    return isinstance(obj, (jax.Array, jnp.DeviceArray))
+    return isinstance(obj, jax.Array)
   return isinstance(obj, jnp.DeviceArray)
 
 
 def default_prng_key(
     rng: Optional[jax.random.PRNGKeyArray] = None,
 ) -> jax.random.PRNGKeyArray:
   """Get the default PRNG key.
 
   Args:
-    rng:
-      PRNG key.
+    rng: PRNG key.
 
   Returns:
     If ``rng = None``, returns the default PRNG key.
     Otherwise, it returns the unmodified ``rng`` key.
   """
   return jax.random.PRNGKey(0) if rng is None else rng
```

### Comparing `ott-jax-0.4.2/src/ott_jax.egg-info/PKG-INFO` & `ott-jax-0.4.3/src/ott_jax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ott-jax
-Version: 0.4.2
+Version: 0.4.3
 Summary: Optimal Transport Tools in JAX.
 Author-email: OTT team <optimal.transport.tools@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ott-jax-0.4.2/src/ott_jax.egg-info/SOURCES.txt` & `ott-jax-0.4.3/src/ott_jax.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 .codecov.yml
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
+CITATION.bib
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 environment.yml
 pyproject.toml
 setup.py
 src/ott/__init__.py
```

### Comparing `ott-jax-0.4.2/src/ott_jax.egg-info/requires.txt` & `ott-jax-0.4.3/src/ott_jax.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 jax>=0.1.67
 jaxlib>=0.1.47
 jaxopt>=0.5.5
-numpy!=1.25.0,>=1.18.4
-flax>=0.5.2
+numpy<1.25.0,>=1.18.4
+flax>=0.6.6
 optax>=0.1.1
 
 [:python_version >= "3.9"]
 lineax>=0.0.1
 
 [dev]
 pre-commit>=2.16.0
@@ -26,13 +26,14 @@
 pytest-xdist
 pytest-cov
 pytest-memray
 coverage[toml]
 chex
 networkx>=2.5
 scikit-learn>=1.0
+matplotlib
 
 [test:python_version < "3.11"]
 tslearn>=0.5
 
 [test:python_version >= "3.9"]
 lineax
```

