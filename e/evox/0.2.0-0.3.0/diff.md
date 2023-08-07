# Comparing `tmp/evox-0.2.0.tar.gz` & `tmp/evox-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evox-0.2.0.tar", last modified: Tue Jun 13 07:04:20 2023, max compression
+gzip compressed data, was "evox-0.3.0.tar", last modified: Mon Aug  7 07:41:11 2023, max compression
```

## Comparing `evox-0.2.0.tar` & `evox-0.3.0.tar`

### file list

```diff
@@ -1,119 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.348936 evox-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-13 07:04:09.000000 evox-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-13 07:04:20.348936 evox-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-13 07:04:09.000000 evox-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-13 07:04:09.000000 evox-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:04:20.348936 evox-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.324936 evox-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.328935 evox-0.2.0/src/evox/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.328935 evox-0.2.0/src/evox/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.332936 evox-0.2.0/src/evox/algorithms/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/containers/clustered_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/containers/coevolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/containers/tree_algorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.332936 evox-0.2.0/src/evox/algorithms/mo/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/mo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/mo/ibea.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/mo/moead.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/mo/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/mo/rvea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.332936 evox-0.2.0/src/evox/algorithms/so/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/cma_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/cso.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/de.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/nes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/open_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/pgpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/pso.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/sort_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.336936 evox-0.2.0/src/evox/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/core/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/core/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/core/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.336936 evox-0.2.0/src/evox/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/metrics/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/metrics/igd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.336936 evox-0.2.0/src/evox/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/population.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/std_mo_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/std_so_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.336936 evox-0.2.0/src/evox/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.336936 evox-0.2.0/src/evox/operators/crossover/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/differential_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/one_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/sbx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/simulated_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crowding_distance_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.340936 evox-0.2.0/src/evox/operators/mutation/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/mutation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/mutation/bitflip.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/mutation/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/mutation/pm_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/non_dominated_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.340936 evox-0.2.0/src/evox/operators/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/sampling/latin_hypercude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/sampling/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.340936 evox-0.2.0/src/evox/operators/selection/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/selection/rvea_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/selection/tournament.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/selection/uniform_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.340936 evox-0.2.0/src/evox/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/pipelines/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/pipelines/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/pipelines/multidevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/pipelines/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.340936 evox-0.2.0/src/evox/problems/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.344936 evox-0.2.0/src/evox/problems/classic/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/ackley.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/dtlz.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/griewank.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/rastrigin.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/zdt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.344936 evox-0.2.0/src/evox/problems/neuroevolution/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/neuroevolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/neuroevolution/torchvision_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.344936 evox-0.2.0/src/evox/problems/rl/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/rl/brax.py
--rw-r--r--   0 runner    (1001) docker     (123)    12332 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/rl/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/rl/gym_mo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.328935 evox-0.2.0/src/evox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-13 07:04:20.000000 evox-0.2.0/src/evox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-13 07:04:20.000000 evox-0.2.0/src/evox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:04:20.000000 evox-0.2.0/src/evox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-13 07:04:20.000000 evox-0.2.0/src/evox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 07:04:20.000000 evox-0.2.0/src/evox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.348936 evox-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_classic_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_crowding_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_distributed_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_multi_objective_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_neuroevolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_non_dominated_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_single_objective_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.903773 evox-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-07 07:40:59.000000 evox-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-08-07 07:41:11.903773 evox-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-07 07:40:59.000000 evox-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-07 07:40:59.000000 evox-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 07:41:11.903773 evox-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.883773 evox-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.887773 evox-0.3.0/src/evox/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.887773 evox-0.3.0/src/evox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.891773 evox-0.3.0/src/evox/algorithms/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/containers/clustered_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/containers/coevolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/containers/tree_algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.891773 evox-0.3.0/src/evox/algorithms/mo/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/mo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/mo/eagmoead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/mo/hype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/mo/ibea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/mo/moead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/mo/moeaddra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/mo/moeadm2m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/mo/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/mo/nsga3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/mo/rvea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/mo/spea2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.891773 evox-0.3.0/src/evox/algorithms/so/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/so/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/so/cma_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/so/cso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/so/de.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/so/nes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/so/open_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/so/pgpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/so/pso.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/algorithms/so/sort_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.895773 evox-0.3.0/src/evox/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/core/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/core/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.895773 evox-0.3.0/src/evox/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/metrics/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/metrics/igd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.895773 evox-0.3.0/src/evox/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/monitors/evoxvis_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/monitors/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/monitors/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/monitors/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/monitors/std_mo_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/monitors/std_so_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.895773 evox-0.3.0/src/evox/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.895773 evox-0.3.0/src/evox/operators/crossover/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/crossover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/crossover/differential_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/crossover/one_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/crossover/sbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/crossover/simulated_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/crossover/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/crowding_distance_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.895773 evox-0.3.0/src/evox/operators/mutation/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/mutation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/mutation/bitflip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/mutation/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/mutation/pm_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/non_dominated_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.899773 evox-0.3.0/src/evox/operators/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/sampling/latin_hypercude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/sampling/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.899773 evox-0.3.0/src/evox/operators/selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/selection/non_dominate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/selection/roulette_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/selection/rvea_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/selection/topk_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/selection/tournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/operators/selection/uniform_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.899773 evox-0.3.0/src/evox/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/pipelines/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/pipelines/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/pipelines/multidevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/pipelines/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/pipelines/uni_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.899773 evox-0.3.0/src/evox/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.899773 evox-0.3.0/src/evox/problems/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/classic/ackley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/classic/dtlz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/classic/griewank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/classic/rastrigin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/classic/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/classic/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/classic/zdt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.899773 evox-0.3.0/src/evox/problems/neuroevolution/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/neuroevolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/neuroevolution/torchvision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.903773 evox-0.3.0/src/evox/problems/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/rl/brax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12332 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/rl/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/problems/rl/gym_mo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-08-07 07:40:59.000000 evox-0.3.0/src/evox/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.887773 evox-0.3.0/src/evox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-08-07 07:41:11.000000 evox-0.3.0/src/evox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-07 07:41:11.000000 evox-0.3.0/src/evox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:41:11.000000 evox-0.3.0/src/evox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-07 07:41:11.000000 evox-0.3.0/src/evox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 07:41:11.000000 evox-0.3.0/src/evox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:41:11.903773 evox-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_classic_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_crowding_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_distributed_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_multi_objective_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_neuroevolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_non_dominated_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_single_objective_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_uni_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-07 07:40:59.000000 evox-0.3.0/tests/test_utils.py
```

### Comparing `evox-0.2.0/LICENSE` & `evox-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/PKG-INFO` & `evox-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evox
-Version: 0.2.0
+Version: 0.3.0
 Summary: evox
 Author-email: Bill Huang <bill.huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang <zhenyuliang97@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, EMI-Group
         All rights reserved.
         
@@ -45,15 +45,15 @@
 Provides-Extra: gym
 Provides-Extra: neuroevolution
 Provides-Extra: distributed
 Provides-Extra: full
 License-File: LICENSE
 
 <h1 align="center">
-  <img src=./logo.png alt="Logo" height="24em"/>
+  <img src=./docs/source/_static/evox_logo.png alt="Logo" height="24em"/>
   <strong>EvoX</strong>
   <br>
   A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
 </h1>
 
 <div align="center">
   <a href="https://evox.readthedocs.io/">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evox Version: 0.2.0 Summary: evox Author-email:
+Metadata-Version: 2.1 Name: evox Version: 0.3.0 Summary: evox Author-email:
 Bill Huang
 huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang
 gmail.com> License: BSD 3-Clause License Copyright (c) 2022, EMI-Group All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
```

### Comparing `evox-0.2.0/README.md` & `evox-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align="center">
-  <img src=./logo.png alt="Logo" height="24em"/>
+  <img src=./docs/source/_static/evox_logo.png alt="Logo" height="24em"/>
   <strong>EvoX</strong>
   <br>
   A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
 </h1>
 
 <div align="center">
   <a href="https://evox.readthedocs.io/">
```

### Comparing `evox-0.2.0/pyproject.toml` & `evox-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "evox"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name = "Bill Huang", email = "bill.huang2001@gmail.com" },
   { name = "Christina Lee", email = "1315552992@qq.com" },
   { name = "Zhenyu Liang", email = "zhenyuliang97@gmail.com" },
 ]
 description = "evox"
 readme = "README.md"
@@ -21,14 +21,15 @@
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
 dependencies = [
   "jax >= 0.3.0",
   "jaxlib >= 0.3.0",
   "optax >= 0.1.0",
+  "pyarrow >= 10.0.0",
 ]
 
 [project.optional-dependencies]
 test = [
   "chex >= 0.1.0",
   "flax >= 0.5.0",
   "pytest >= 6.0.0",
```

### Comparing `evox-0.2.0/src/evox/algorithms/containers/clustered_algorithm.py` & `evox-0.3.0/src/evox/algorithms/containers/clustered_algorithm.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/algorithms/containers/coevolution.py` & `evox-0.3.0/src/evox/algorithms/containers/coevolution.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/algorithms/containers/tree_algorithm.py` & `evox-0.3.0/src/evox/algorithms/containers/tree_algorithm.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/algorithms/mo/ibea.py` & `evox-0.3.0/src/evox/algorithms/mo/nsga2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,102 @@
-import evox as ex
 import jax
 import jax.numpy as jnp
 
-from evox.operators.selection import TournamentSelection
-from evox.operators.mutation import PmMutation
-from evox.operators.crossover import SimulatedBinaryCrossover
-from evox.utils import cal_fitness
+from evox.operators import (
+    non_dominated_sort,
+    crowding_distance,
+    selection,
+    mutation,
+    crossover,
+)
+from evox import Algorithm, jit_class, State
 
 
-@ex.jit_class
-class IBEA(ex.Algorithm):
-    """IBEA algorithm
+@jit_class
+class NSGA2(Algorithm):
+    """NSGA-II algorithm
 
-    link:
+    link: https://ieeexplore.ieee.org/document/996017
     """
 
     def __init__(
         self,
         lb,
         ub,
         n_objs,
         pop_size,
-        kappa=0.05,
-        mutation=PmMutation(),
-        crossover=SimulatedBinaryCrossover(),
+        selection_op=None,
+        mutation_op=None,
+        crossover_op=None,
     ):
         self.lb = lb
         self.ub = ub
         self.n_objs = n_objs
         self.dim = lb.shape[0]
         self.pop_size = pop_size
-        self.kappa = kappa
 
-        self.selection = TournamentSelection(num_round=self.pop_size)
-        self.mutation = mutation
-        self.crossover = crossover
+        self.selection = selection_op
+        self.mutation = mutation_op
+        self.crossover = crossover_op
+
+        if self.selection is None:
+            self.selection = selection.UniformRand(1)
+        if self.mutation is None:
+            self.mutation = mutation.Polynomial((self.lb, self.ub))
+        if self.crossover is None:
+            self.crossover = crossover.SimulatedBinary()
 
     def setup(self, key):
         key, subkey = jax.random.split(key)
         population = (
             jax.random.uniform(subkey, shape=(self.pop_size, self.dim))
             * (self.ub - self.lb)
             + self.lb
         )
-        return ex.State(
+        return State(
             population=population,
             fitness=jnp.zeros((self.pop_size, self.n_objs)),
             next_generation=population,
             is_init=True,
+            key=key,
         )
 
-    @ex.jit_method
     def ask(self, state):
         return jax.lax.cond(state.is_init, self._ask_init, self._ask_normal, state)
 
     def tell(self, state, fitness):
         return jax.lax.cond(
             state.is_init, self._tell_init, self._tell_normal, state, fitness
         )
 
     def _ask_init(self, state):
         return state.population, state
 
     def _ask_normal(self, state):
-        population = state.population
-        pop_obj = state.fitness
-        fitness = cal_fitness(pop_obj, self.kappa)[0]
-
-        selected, state = self.selection(state, population, fitness)
-        crossovered, state = self.crossover(state, selected)
-        mutated, state = self.mutation(state, crossovered, (self.lb, self.ub))
+        key, sel_key1, x_key, mut_key = jax.random.split(state.key, 4)
+        # crossovered = self.selection(sel_key1, state.population)
+        crossovered = self.crossover(x_key, state.population)
+        next_generation = self.mutation(mut_key, crossovered)
 
-        next_generation = jnp.clip(mutated, self.lb, self.ub)
-        return next_generation, state.update(next_generation=next_generation)
+        next_generation = jnp.clip(next_generation, self.lb, self.ub)
+
+        return next_generation, state.update(next_generation=next_generation, key=key)
 
     def _tell_init(self, state, fitness):
         state = state.update(fitness=fitness, is_init=False)
         return state
 
-    # @profile
     def _tell_normal(self, state, fitness):
         merged_pop = jnp.concatenate([state.population, state.next_generation], axis=0)
-        merged_obj = jnp.concatenate([state.fitness, fitness], axis=0)
-
-        n = jnp.shape(merged_pop)[0]
-        merged_fitness, I, C = cal_fitness(merged_obj, self.kappa)
-
-        next_ind = jnp.arange(n)
-        vals = (next_ind, merged_fitness)
-
-        def body_fun(i, vals):
-            next_ind, merged_fitness = vals
-            x = jnp.argmin(merged_fitness)
-            merged_fitness += jnp.exp(-I[x, :] / C[x] / self.kappa)
-            merged_fitness = merged_fitness.at[x].set(jnp.max(merged_fitness))
-            next_ind = next_ind.at[x].set(-1)
-            return (next_ind, merged_fitness)
-
-        next_ind, merged_fitness = jax.lax.fori_loop(0, self.pop_size, body_fun, vals)
-
-        ind = jnp.where(next_ind != -1, size=n, fill_value=-1)[0]
-        ind_n = ind[0 : self.pop_size]
-
-        survivor = merged_pop[ind_n]
-        survivor_fitness = merged_obj[ind_n]
+        merged_fitness = jnp.concatenate([state.fitness, fitness], axis=0)
 
+        rank = non_dominated_sort(merged_fitness)
+        order = jnp.argsort(rank)
+        worst_rank = rank[order[self.pop_size]]
+        mask = rank == worst_rank
+        crowding_dis = crowding_distance(merged_fitness, mask)
+
+        combined_order = jnp.lexsort((-crowding_dis, rank))[: self.pop_size]
+        survivor = merged_pop[combined_order]
+        survivor_fitness = merged_fitness[combined_order]
         state = state.update(population=survivor, fitness=survivor_fitness)
-
         return state
```

### Comparing `evox-0.2.0/src/evox/algorithms/mo/moead.py` & `evox-0.3.0/src/evox/algorithms/mo/moead.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,94 @@
-import evox as ex
 import jax
 import jax.numpy as jnp
 
-from evox.operators.mutation import PmMutation
-from evox.operators.crossover import SimulatedBinaryCrossover
+from evox.operators import mutation, crossover
 from evox.operators.sampling import UniformSampling, LatinHypercubeSampling
 from evox.utils import euclidean_dis
+from evox import Algorithm, State, jit_class
 
 
-@ex.jit_class
-class MOEAD(ex.Algorithm):
+@jit_class
+class MOEAD(Algorithm):
     """MOEA/D algorithm
 
     link: https://ieeexplore.ieee.org/document/4358754
     """
 
     def __init__(
         self,
         lb,
         ub,
         n_objs,
         pop_size,
         type=1,
-        mutation=PmMutation(),
-        crossover=SimulatedBinaryCrossover(type=2),
+        mutation_op=None,
+        crossover_op=None,
     ):
         self.lb = lb
         self.ub = ub
         self.n_objs = n_objs
         self.dim = lb.shape[0]
         self.pop_size = pop_size
         self.type = type
         self.T = jnp.ceil(self.pop_size / 10).astype(int)
 
-        self.mutation = mutation
-        self.crossover = crossover
+        self.mutation = mutation_op
+        self.crossover = crossover_op
+
+        if self.mutation is None:
+            self.mutation = mutation.Polynomial((lb, ub))
+        if self.crossover is None:
+            self.crossover = crossover.SimulatedBinary(type=2)
+        self.sample = LatinHypercubeSampling(self.pop_size, self.n_objs)
 
     def setup(self, key):
         key, subkey1, subkey2 = jax.random.split(key, 3)
         population = (
             jax.random.uniform(subkey1, shape=(self.pop_size, self.dim))
             * (self.ub - self.lb)
             + self.lb
         )
-        # w = UniformSampling(self.pop_size, self.n_objs).random()[0]
-        w = LatinHypercubeSampling(self.pop_size, self.n_objs).random(subkey2)[0]
+        w, _ = self.sample(subkey2)
         B = euclidean_dis(w, w)
         B = jnp.argsort(B, axis=1)
         B = B[:, : self.T]
-        return ex.State(
+        return State(
             population=population,
             fitness=jnp.zeros((self.pop_size, self.n_objs)),
             next_generation=population,
             weight_vector=w,
             B=B,
             Z=jnp.zeros(shape=self.n_objs),
             parent=jnp.zeros((self.pop_size, self.T)).astype(int),
             is_init=True,
             key=key,
         )
 
-    @ex.jit_method
     def ask(self, state):
         return jax.lax.cond(state.is_init, self._ask_init, self._ask_normal, state)
 
     def tell(self, state, fitness):
         return jax.lax.cond(
             state.is_init, self._tell_init, self._tell_normal, state, fitness
         )
 
     def _ask_init(self, state):
         return state.population, state
 
     def _ask_normal(self, state):
-        key, subkey = jax.random.split(state.key)
+        key, subkey, sel_key, mut_key = jax.random.split(state.key, 4)
         parent = jax.random.permutation(
             subkey, state.B, axis=1, independent=True
         ).astype(int)
         population = state.population
         selected_p = jnp.r_[population[parent[:, 0]], population[parent[:, 1]]]
 
-        crossovered, state = self.crossover(state, selected_p)
-        next_generation, state = self.mutation(state, crossovered, (self.lb, self.ub))
-        # next_generation = jnp.clip(mutated, self.lb, self.ub)
+        crossovered = self.crossover(sel_key, selected_p)
+        next_generation = self.mutation(mut_key, crossovered)
 
         return next_generation, state.update(
             next_generation=next_generation, parent=parent, key=key
         )
 
     def _tell_init(self, state, fitness):
         Z = jnp.min(fitness, axis=0)
```

### Comparing `evox-0.2.0/src/evox/algorithms/mo/rvea.py` & `evox-0.3.0/src/evox/algorithms/mo/ibea.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,144 +1,130 @@
-import evox as ex
 import jax
 import jax.numpy as jnp
 
-from evox.operators.selection import ReferenceVectorGuidedSelection
-from evox.operators.mutation import PmMutation
-from evox.operators.crossover import SimulatedBinaryCrossover
-from evox.operators.sampling import UniformSampling, LatinHypercubeSampling
+from evox.operators import selection, mutation, crossover
+from evox.utils import cal_max
+from evox import Algorithm, State, jit_class
 
 
-@ex.jit_class
-class RVEA(ex.Algorithm):
-    """RVEA algorithms
+@jax.jit
+def cal_fitness(pop_obj, kappa):
+    n = jnp.shape(pop_obj)[0]
+    pop_obj = (pop_obj - jnp.tile(jnp.min(pop_obj), (n, 1))) / (
+        jnp.tile(jnp.max(pop_obj) - jnp.min(pop_obj), (n, 1))
+    )
+    I = cal_max(pop_obj, pop_obj)
 
-    link: https://ieeexplore.ieee.org/document/7386636
+    C = jnp.max(jnp.abs(I), axis=0)
+
+    fitness = jnp.sum(-jnp.exp(-I / jnp.tile(C, (n, 1)) / kappa), axis=0) + 1
+
+    return fitness, I, C
+
+
+@jit_class
+class IBEA(Algorithm):
+    """IBEA algorithm
+
+    link: https://link.springer.com/chapter/10.1007/978-3-540-30217-9_84
     """
 
     def __init__(
         self,
         lb,
         ub,
         n_objs,
         pop_size,
-        alpha=2,
-        fr=0.1,
-        max_gen=100,
-        selection=ReferenceVectorGuidedSelection(),
-        mutation=PmMutation(),
-        crossover=SimulatedBinaryCrossover(),
+        kappa=0.05,
+        mutation_op=None,
+        crossover_op=None,
     ):
         self.lb = lb
         self.ub = ub
         self.n_objs = n_objs
         self.dim = lb.shape[0]
         self.pop_size = pop_size
-        self.alpha = alpha
-        self.fr = fr
-        self.max_gen = max_gen
-
-        self.selection = selection
-        self.mutation = mutation
-        self.crossover = crossover
-        # self.sampling = UniformSampling(self.pop_size, self.n_objs)
-        self.sampling = LatinHypercubeSampling(self.pop_size, self.n_objs)
+        self.kappa = kappa
+
+        self.selection = selection.Tournament(n_round=self.pop_size)
+        self.mutation = mutation_op
+        self.crossover = crossover_op
+
+        if self.mutation is None:
+            self.mutation = mutation.Polynomial((lb, ub))
+        if self.crossover is None:
+            self.crossover = crossover.SimulatedBinary()
 
     def setup(self, key):
-        key, subkey1, subkey2 = jax.random.split(key, 3)
+        key, subkey = jax.random.split(key)
         population = (
-            jax.random.uniform(subkey1, shape=(self.pop_size, self.dim))
+            jax.random.uniform(subkey, shape=(self.pop_size, self.dim))
             * (self.ub - self.lb)
             + self.lb
         )
-        v = self.sampling.random(subkey2)[0]
-        v = v / jnp.linalg.norm(v, axis=0)
-        mask = jnp.full((self.pop_size, 1), False)
-
-        return ex.State(
+        return State(
             population=population,
             fitness=jnp.zeros((self.pop_size, self.n_objs)),
             next_generation=population,
-            reference_vector=v,
             is_init=True,
             key=key,
-            gen=0,
-            mask=mask,
         )
 
-    @ex.jit_method
     def ask(self, state):
         return jax.lax.cond(state.is_init, self._ask_init, self._ask_normal, state)
 
     def tell(self, state, fitness):
         return jax.lax.cond(
             state.is_init, self._tell_init, self._tell_normal, state, fitness
         )
 
     def _ask_init(self, state):
         return state.population, state
 
     def _ask_normal(self, state):
-        mask = state.mask
-        key = state.key
-        key, subkey = jax.random.split(key)
-        r = (
-            jax.random.uniform(subkey, shape=(self.pop_size, self.dim))
-            * (self.ub - self.lb)
-            + self.lb
-        )
-
-        crossovered, state = self.crossover(state, state.population)
-        next_generation, state = self.mutation(state, crossovered, (self.lb, self.ub))
-        next_generation = jnp.where(mask, r, next_generation)
+        key, sel_key, x_key, mut_key = jax.random.split(state.key, 4)
+        population = state.population
+        pop_obj = state.fitness
+        fitness = cal_fitness(pop_obj, self.kappa)[0]
+
+        # selected = self.selection(sel_key, population, fitness)
+        selected, _ = self.selection(sel_key, population, -fitness)
+        crossovered = self.crossover(x_key, selected)
+        next_generation = self.mutation(mut_key, crossovered)
 
+        # next_generation = jnp.clip(mutated, self.lb, self.ub)
         return next_generation, state.update(next_generation=next_generation, key=key)
 
     def _tell_init(self, state, fitness):
         state = state.update(fitness=fitness, is_init=False)
         return state
 
+    # @profile
     def _tell_normal(self, state, fitness):
-        current_gen = state.gen + 1
-        v = state.reference_vector
         merged_pop = jnp.concatenate([state.population, state.next_generation], axis=0)
-        merged_fitness = jnp.concatenate([state.fitness, fitness], axis=0)
+        merged_obj = jnp.concatenate([state.fitness, fitness], axis=0)
 
-        rank, state = self.selection(
-            state, merged_fitness, v, (current_gen / self.max_gen) ** self.alpha
-        )
+        n = jnp.shape(merged_pop)[0]
+        merged_fitness, I, C = cal_fitness(merged_obj, self.kappa)
 
-        mask = (rank == -1)[:, jnp.newaxis]
+        next_ind = jnp.arange(n)
+        vals = (next_ind, merged_fitness)
 
-        survivor = merged_pop[rank]
-        survivor_fitness = merged_fitness[rank]
+        def body_fun(i, vals):
+            next_ind, merged_fitness = vals
+            x = jnp.argmin(merged_fitness)
+            merged_fitness += jnp.exp(-I[x, :] / C[x] / self.kappa)
+            merged_fitness = merged_fitness.at[x].set(jnp.max(merged_fitness))
+            next_ind = next_ind.at[x].set(-1)
+            return (next_ind, merged_fitness)
 
-        def rv_adaptation(pop_obj, v):
-            v_temp = v * jnp.tile((pop_obj.max(0) - pop_obj.min(0)), (len(v), 1))
-            next_v = v.astype(float)
-
-            next_v = v_temp / jnp.tile(
-                jnp.sqrt(jnp.sum(v_temp**2, axis=1)).reshape(len(v), 1),
-                (1, jnp.shape(v)[1]),
-            )
-
-            return next_v
-
-        def no_update(pop_obj, v):
-            return v
-
-        v = jax.lax.cond(
-            current_gen % (1 / self.fr) == 0,
-            rv_adaptation,
-            no_update,
-            survivor_fitness,
-            v,
-        )
+        next_ind, merged_fitness = jax.lax.fori_loop(0, self.pop_size, body_fun, vals)
+
+        ind = jnp.where(next_ind != -1, size=n, fill_value=-1)[0]
+        ind_n = ind[0 : self.pop_size]
+
+        survivor = merged_pop[ind_n]
+        survivor_fitness = merged_obj[ind_n]
+
+        state = state.update(population=survivor, fitness=survivor_fitness)
 
-        state = state.update(
-            population=survivor,
-            fitness=survivor_fitness,
-            reference_vector=v,
-            gen=current_gen,
-            mask=mask,
-        )
         return state
```

### Comparing `evox-0.2.0/src/evox/algorithms/so/cma_es.py` & `evox-0.3.0/src/evox/algorithms/so/cma_es.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/algorithms/so/cso.py` & `evox-0.3.0/src/evox/algorithms/so/cso.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/algorithms/so/de.py` & `evox-0.3.0/src/evox/algorithms/so/de.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/algorithms/so/nes.py` & `evox-0.3.0/src/evox/algorithms/so/nes.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/algorithms/so/open_es.py` & `evox-0.3.0/src/evox/algorithms/so/open_es.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/algorithms/so/pgpe.py` & `evox-0.3.0/src/evox/algorithms/so/pgpe.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/algorithms/so/pso.py` & `evox-0.3.0/src/evox/algorithms/so/pso.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/core/algorithm.py` & `evox-0.3.0/src/evox/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/core/module.py` & `evox-0.3.0/src/evox/core/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     err_msg = "Expect last return value must be State, got {}"
 
     @wraps(func)
     def wrapper(self, state: State, *args, **kwargs):
         assert isinstance(self, Stateful) and isinstance(state, State)
         # find the state that match the current module
-        path, matched_state = state.find_path_to(self._node_id)
+        path, matched_state = state.find_path_to(self._node_id, self._module_name)
 
         return_value = func(self, matched_state, *args, **kwargs)
 
         # single return value, the value must be a State
         if not isinstance(return_value, tuple):
             assert isinstance(return_value, State), err_msg.format(type(return_value))
             aux, new_state = None, return_value
@@ -180,21 +180,22 @@
         Returns
         -------
         State
             The state of this module.
         """
         return State()
 
-    def _recursive_init(self, key, node_id) -> Tuple[State, int]:
+    def _recursive_init(self, key, node_id, module_name) -> Tuple[State, int]:
         if hasattr(self, "_node_id") and self._node_id is not None:
             warnings.warn(
                 "Trying to re-initialize a Stateful module that is already initialized"
             )
 
         self._node_id = node_id
+        self._module_name = module_name
 
         child_states = {}
 
         # Find all submodules and sort them according to their name.
         # Sorting is important because it makes sure that the node_id
         # is deterministic across different runs.
         submodules = []
@@ -205,15 +206,15 @@
         submodules.sort()
 
         for attr_name, attr in submodules:
             if key is None:
                 subkey = None
             else:
                 key, subkey = jax.random.split(key)
-            submodule_state, node_id = attr._recursive_init(subkey, node_id + 1)
+            submodule_state, node_id = attr._recursive_init(subkey, node_id + 1, attr_name)
             assert isinstance(
                 submodule_state, State
             ), "setup method must return a State"
             child_states[attr_name] = submodule_state
 
         return (
             self.setup(key)
@@ -233,9 +234,9 @@
             A PRNGKey.
 
         Returns
         -------
         State
             The state of this module and all submodules combined.
         """
-        state, _node_id = self._recursive_init(key, 0)
+        state, _node_id = self._recursive_init(key, 0, None)
         return state
```

### Comparing `evox-0.2.0/src/evox/core/problem.py` & `evox-0.3.0/src/evox/core/problem.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/core/state.py` & `evox-0.3.0/src/evox/core/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,18 +102,24 @@
         return self._child_states[name]
 
     def update_child(self, name: str, child_state: dict) -> State:
         return copy(self)._set_child_states_mut(
             {**self._child_states, name: self._child_states[name].update(child_state)}
         )
 
-    def find_path_to(self, node_id) -> Optional[Tuple[Union[Tuple, int], State]]:
+    def find_path_to(self, node_id: int, hint: Optional[str] = None) -> Optional[Tuple[Union[Tuple, int], State]]:
+        """Find the state with node_id matching the state_id
+        A hint can be given with the module_name
+        """
         if node_id == self._state_id:
             return node_id, self
 
+        if node_id == self._child_states[hint]._state_id:
+            return (hint, node_id), self._child_states[hint]
+
         for child_id, child_state in self._child_states.items():
             result = child_state.find_path_to(node_id)
             if result is not None:
                 path, state = result
                 return (child_id, path), state
 
         return None
```

### Comparing `evox-0.2.0/src/evox/metrics/hypervolume.py` & `evox-0.3.0/src/evox/metrics/hypervolume.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/monitors/fitness.py` & `evox-0.3.0/src/evox/monitors/fitness.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/monitors/gym.py` & `evox-0.3.0/src/evox/monitors/gym.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/monitors/population.py` & `evox-0.3.0/src/evox/monitors/population.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/monitors/std_mo_monitor.py` & `evox-0.3.0/src/evox/monitors/std_mo_monitor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import chex
 import jax.numpy as jnp
 import numpy as np
 from ..operators.non_dominated_sort import non_dominated_sort
 
 
 class StdMOMonitor:
     """Standard multi-objective monitor
     Used for multi-objective workflow,
     can monitor fitness and record the pareto front.
+
     Parameters
     ----------
     record_pf
         Whether to record the pareto front during the run.
         Default to False.
         Setting it to True will cause the monitor to
         maintain a pareto front of all the solutions with unlimited size,
@@ -25,19 +25,19 @@
         self.record_pf = record_pf
         self.record_fit_history = record_fit_history
         self.fitness_history = []
         self.current_population = None
         self.pf_solutions = None
         self.pf_fitness = None
 
-    def record_pop(self, pop):
+    def record_pop(self, pop, tranform=None):
         self.current_population = pop
         return pop
 
-    def record_fit(self, fitness):
+    def record_fit(self, fitness, tranform=None):
         if self.record_fit_history:
             self.fitness_history.append(fitness)
 
         if self.record_pf:
             if self.pf_fitness is None:
                 self.pf_fitness = fitness
             else:
@@ -64,7 +64,13 @@
         return self.pf_fitness
 
     def get_pf_solutions(self):
         return self.pf_solutions
 
     def get_history(self):
         return self.fitness_history
+
+    def flush(self):
+        hcb.barrier_wait()
+
+    def close(self):
+        self.flush()
```

### Comparing `evox-0.2.0/src/evox/monitors/std_so_monitor.py` & `evox-0.3.0/src/evox/monitors/std_so_monitor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import jax.numpy as jnp
 import warnings
+import jax.experimental.host_callback as hcb
 
 
 class StdSOMonitor:
     """Standard single-objective monitor
     Used for single-objective workflow,
     can monitor fitness and the population.
 
@@ -21,19 +22,19 @@
         self.record_fit_history = record_fit_history
         self.fitness_history = []
         self.record_topk = record_topk
         self.current_population = None
         self.topk_solutions = None
         self.topk_fitness = None
 
-    def record_pop(self, pop):
+    def record_pop(self, pop, tranform=None):
         self.current_population = pop
         return pop
 
-    def record_fit(self, fitness):
+    def record_fit(self, fitness, transform=None):
         if self.record_fit_history:
             self.fitness_history.append(fitness)
         if self.record_topk == 1:
             # handle the case where topk = 1
             # don't need argsort / top_k, which are slower
             current_min_fit = jnp.min(fitness, keepdims=True)
             if self.topk_fitness is None or self.topk_fitness > current_min_fit:
@@ -86,7 +87,13 @@
         if self.topk_solutions is None:
             warnings.warn("trying to get info from a monitor with no recorded data")
             return None
         return self.topk_solutions[0]
 
     def get_history(self):
         return self.fitness_history
+
+    def flush(self):
+        hcb.barrier_wait()
+
+    def close(self):
+        self.flush()
```

### Comparing `evox-0.2.0/src/evox/operators/crossover/one_point.py` & `evox-0.3.0/src/evox/operators/crossover/one_point.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-import evox as ex
-import jax
 import jax.numpy as jnp
+from jax import random, jit, vmap
+from evox import jit_class
 
 
 def _random_pairing(key, x):
     batch, dim = x.shape
-    x = jax.random.permutation(key, x, axis=0)
+    x = random.permutation(key, x, axis=0)
     return x.reshape(batch // 2, 2, dim)
 
 
 def _unpair(x):
     batch, _, dim = x.shape
     return x.reshape(batch * 2, dim)
 
 
 def _one_point_crossover(key, parents):
     _, dim = parents.shape
-    point = jax.random.choice(key, dim) + 1
-    mask = jnp.ones((point,))
-    mask = jnp.pad(mask, (0, dim - point), 'constant', constant_values=(0, 0))
+    point = random.choice(key, dim) + 1
+    mask = jnp.arange(dim) < point
     c1 = jnp.where(mask, parents[0], parents[1])
     c2 = jnp.where(mask, parents[1], parents[0])
     return jnp.stack([c1, c2])
 
 
-@ex.jit_class
-class OnePointCrossover(ex.Operator):
-    def __init__(self, stdvar=1.0):
-        self.stdvar = stdvar
-
-    def setup(self, key):
-        return ex.State(key=key)
-
-    def __call__(self, state, x):
-        key = state.key
-        key, pairing_key, crossover_key = jax.random.split(key, 3)
-        paired = _random_pairing(pairing_key, x)
-        crossover_keys = jax.random.split(crossover_key, paired.shape[0])
-        children = jax.vmap(_one_point_crossover)(crossover_keys, paired)
-        return _unpair(children), ex.State(key=key)
+@jit
+def one_point(key, x):
+    pairing_key, crossover_key = random.split(key, 2)
+    paired = _random_pairing(pairing_key, x)
+    crossover_keys = random.split(crossover_key, paired.shape[0])
+    children = vmap(_one_point_crossover)(crossover_keys, paired)
+    return _unpair(children)
+
+
+@jit_class
+class OnePoint:
+    def __call__(self, key, x):
+        return one_point(key, x)
```

### Comparing `evox-0.2.0/src/evox/operators/crossover/sbx.py` & `evox-0.3.0/src/evox/operators/crossover/sbx.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,60 @@
-import evox as ex
-import jax
 import jax.numpy as jnp
+from jax import random, jit, vmap
+from evox import jit_class
+from functools import partial
+
+
+@partial(jit, static_argnums=[4])
+def simulated_binary(key, x, pro_c, dis_c, type):
+    mu_key, beta1_key, beta2_key, beta3_key = random.split(key, 4)
+    n, _ = jnp.shape(x)
+    parent1_dec = x[: n // 2, :]
+    parent2_dec = x[n // 2: n // 2 * 2, :]
+    n_p, d = jnp.shape(parent1_dec)
+    beta = jnp.zeros((n_p, d))
+    mu = random.uniform(mu_key, shape=(n_p, d))
+    beta = jnp.where(mu <= 0.5, jnp.power(2 * mu, 1 / (dis_c + 1)), beta)
+    beta = jnp.where(mu > 0.5, jnp.power(2 - 2 * mu, -1 / (dis_c + 1)), beta)
+    beta = beta * (
+        (-1) ** random.randint(beta1_key, shape=(n_p, d), minval=0, maxval=2)
+    )
+    beta = jnp.where(random.uniform(beta2_key, shape=(n_p, d)) < 0.5, 1, beta)
+    beta = jnp.where(
+        jnp.tile(random.uniform(beta3_key, shape=(n_p, 1)) > pro_c, (1, d)), 1, beta
+    )
+    if type == 1:
+        offspring_dec = jnp.vstack(
+            (
+                (parent1_dec + parent2_dec) / 2
+                + beta * (parent1_dec - parent2_dec) / 2,
+                (parent1_dec + parent2_dec) / 2
+                - beta * (parent1_dec - parent2_dec) / 2,
+            )
+        )
+        if n % 2 != 0:
+            offspring_dec = jnp.r_[offspring_dec, x[-1:, :]]
+    if type == 2:
+        offspring_dec = (parent1_dec + parent2_dec) / 2 + beta * (
+            parent1_dec - parent2_dec
+        ) / 2
+    return offspring_dec
 
 
-@ex.jit_class
-class SimulatedBinaryCrossover(ex.Operator):
+@jit_class
+class SimulatedBinary:
     """Simulated binary crossover(SBX)
 
     Args:
         pro_c: the probabilities of doing crossover.
         dis_c: the distribution index of SBX.
-        type: the type is that generate the number of individuals. Type 1 generate offspring of the same size as the parent. 
-        Type 2 generate offspring of half of the population size of the parent. 
+        type: the type is that generate the number of individuals. Type 1 generate offspring of the same size as the parent.
+        Type 2 generate offspring of half of the population size of the parent.
     """
 
     def __init__(self, pro_c=1, dis_c=20, type=1):
         self.pro_c = pro_c
         self.dis_c = dis_c
         self.type = type
 
-    def setup(self, key):
-        return ex.State(key=key)
-
-    def __call__(self, state, x):
-        key = state.key
-        key, mu_key, beta1_key, beta2_key, beta3_key = jax.random.split(key, 5)
-        n, _ = jnp.shape(x)
-        parent1_dec = x[:n // 2, :]
-        parent2_dec = x[n // 2:n // 2 * 2, :]
-        n_p, d = jnp.shape(parent1_dec)
-        beta = jnp.zeros((n_p, d))
-        mu = jax.random.uniform(mu_key, shape=(n_p, d))
-        beta = jnp.where(mu <= 0.5, jnp.power(
-            2 * mu, 1 / (self.dis_c + 1)), beta)
-        beta = jnp.where(mu > 0.5, jnp.power(
-            2 - 2 * mu, -1 / (self.dis_c + 1)), beta)
-        beta = beta * ((-1) ** jax.random.randint(beta1_key,
-                       shape=(n_p, d), minval=0, maxval=2))
-        beta = jnp.where(jax.random.uniform(
-            beta2_key, shape=(n_p, d)) < 0.5, 1, beta)
-        beta = jnp.where(jnp.tile(jax.random.uniform(
-            beta3_key, shape=(n_p, 1)) > self.pro_c, (1, d)), 1, beta)
-        if self.type == 1:
-            offspring_dec = jnp.vstack(((parent1_dec + parent2_dec) / 2 + beta * (parent1_dec - parent2_dec) / 2,
-                                        (parent1_dec + parent2_dec) / 2 - beta * (parent1_dec - parent2_dec) / 2))
-            if n % 2 != 0:
-                offspring_dec = jnp.r_[offspring_dec, x[-1:, :]]
-        if self.type == 2:
-            offspring_dec = (parent1_dec + parent2_dec) / 2 + \
-                beta * (parent1_dec - parent2_dec) / 2
-        return offspring_dec, ex.State(key=key)
+    def __call__(self, key, x):
+        return simulated_binary(key, x, self.pro_c, self.dis_c, self.type)
```

### Comparing `evox-0.2.0/src/evox/operators/crossover/uniform.py` & `evox-0.3.0/src/evox/operators/crossover/uniform.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-import evox as ex
-import jax
 import jax.numpy as jnp
+from jax import random, jit, vmap, lax
+from evox import jit_class
 
 
 def _random_pairing(key, x):
     batch, dim = x.shape
-    x = jax.random.permutation(key, x, axis=0)
+    x = random.permutation(key, x, axis=0)
     return x.reshape(batch // 2, 2, dim)
 
 
 def _unpair(x):
     batch, _, dim = x.shape
     return x.reshape(batch * 2, dim)
 
 
 def _uniform_crossover(key, parents):
     _, dim = parents.shape
-    mask = jax.random.choice(key, 2, (dim,))
+    mask = random.choice(key, 2, (dim,))
     c1 = jnp.where(mask, parents[0], parents[1])
     c2 = jnp.where(mask, parents[1], parents[0])
     return jnp.stack([c1, c2])
 
 
-@ex.jit_class
-class UniformCrossover(ex.Operator):
-    def __init__(self, stdvar=1.0):
-        self.stdvar = stdvar
-
-    def setup(self, key):
-        return ex.State(key=key)
-
-    def __call__(self, state, x):
-        key = state.key
-        key, pairing_key, crossover_key = jax.random.split(key, 3)
-        paired = _random_pairing(pairing_key, x)
-        crossover_keys = jax.random.split(crossover_key, paired.shape[0])
-        children = jax.vmap(_uniform_crossover)(crossover_keys, paired)
-        return _unpair(children), ex.State(key=key)
+@jit
+def uniform_rand(key, x):
+    key, pairing_key, crossover_key = random.split(key, 3)
+    paired = _random_pairing(pairing_key, x)
+    crossover_keys = random.split(crossover_key, paired.shape[0])
+    children = vmap(_uniform_crossover)(crossover_keys, paired)
+    return _unpair(children)
+
+
+@jit_class
+class UniformRand:
+    def __call__(self, key, x):
+        return uniform_rand(key, x)
```

### Comparing `evox-0.2.0/src/evox/operators/crowding_distance_sort.py` & `evox-0.3.0/src/evox/operators/crowding_distance_sort.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/operators/mutation/pm_mutation.py` & `evox-0.3.0/src/evox/operators/mutation/pm_mutation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,72 @@
-import evox as ex
-import jax
+from evox import jit_class
+from jax import jit, random
 import jax.numpy as jnp
 
 
-@ex.jit_class
-class PmMutation(ex.Operator):
+@jit
+def polynomial(key, x, boundary, pro_m, dis_m):
+    subkey1, subkey2 = random.split(key)
+    if jnp.shape(x)[0] == 1:
+        pop_dec = x
+    else:
+        pop_dec = x[: (len(x) // 2) * 2, :]
+    n, d = jnp.shape(pop_dec)
+    site = random.uniform(subkey1, shape=(n, d)) < pro_m / d
+    mu = random.uniform(subkey2, shape=(n, d))
+
+    temp = site & (mu <= 0.5)
+    lower, upper = jnp.tile(boundary[0], (n, 1)), jnp.tile(boundary[1], (n, 1))
+    pop_dec = jnp.maximum(jnp.minimum(pop_dec, upper), lower)
+    norm = jnp.where(temp, (pop_dec - lower) / (upper - lower), 0)
+    pop_dec = jnp.where(
+        temp,
+        pop_dec
+        + (upper - lower)
+        * (
+            jnp.power(
+                2.0 * mu + (1.0 - 2.0 * mu) * jnp.power(1.0 - norm, dis_m + 1.0),
+                1.0 / (dis_m + 1),
+            )
+            - 1.0
+        ),
+        pop_dec,
+    )
+
+    temp = site & (mu > 0.5)
+    norm = jnp.where(temp, (upper - pop_dec) / (upper - lower), 0)
+    pop_dec = jnp.where(
+        temp,
+        pop_dec
+        + (upper - lower)
+        * (
+            1.0
+            - jnp.power(
+                2.0 * (1.0 - mu)
+                + 2.0 * (mu - 0.5) * jnp.power(1.0 - norm, dis_m + 1.0),
+                1.0 / (dis_m + 1.0),
+            )
+        ),
+        pop_dec,
+    )
+    if jnp.shape(x)[0] % 2 != 0:
+        pop_dec = jnp.r_[pop_dec, x[-1:, :]]
+
+    return pop_dec
+
+
+@jit_class
+class Polynomial:
     """Polynomial mutation
 
     Args:
         pro_m: the expectation of number of bits doing mutation.
         dis_m: the distribution index of polynomial mutation.
     """
 
-    def __init__(self, pro_m=1, dis_m=20):
+    def __init__(self, boundary, pro_m=1, dis_m=20):
+        self.boundary = boundary
         self.pro_m = pro_m
         self.dis_m = dis_m
 
-    def setup(self, key):
-        return ex.State(key=key)
-
-    def __call__(self, state, x, boundary=None):
-        key, subkey1, subkey2 = jax.random.split(state.key, 3)
-        if jnp.shape(x)[0] == 1:
-            pop_dec = x
-        else:
-            pop_dec = x[:(len(x)//2)*2, :]
-        n, d = jnp.shape(pop_dec)
-        site = jax.random.uniform(subkey1, shape=(n, d)) < self.pro_m / d
-        mu = jax.random.uniform(subkey2, shape=(n, d))
-
-        temp = site & (mu <= 0.5)
-        lower, upper = jnp.tile(
-            boundary[0], (n, 1)), jnp.tile(boundary[1], (n, 1))
-        pop_dec = jnp.maximum(jnp.minimum(pop_dec, upper), lower)
-        norm = jnp.where(temp, (pop_dec-lower)/(upper-lower), 0)
-        pop_dec = jnp.where(temp, pop_dec+(upper - lower) *
-                            (jnp.power(2. * mu + (1. - 2. * mu) * jnp.power(1. - norm, self.dis_m + 1.),
-                                       1. / (self.dis_m + 1)) - 1.), pop_dec)
-
-        temp = site & (mu > 0.5)
-        norm = jnp.where(temp, (upper-pop_dec) / (upper - lower), 0)
-        pop_dec = jnp.where(temp, pop_dec+(upper - lower) *
-                            (1. - jnp.power(
-                                2. * (1. - mu) + 2. * (mu - 0.5) *
-                                jnp.power(1. - norm, self.dis_m + 1.),
-                                1. / (self.dis_m + 1.))), pop_dec)
-        if jnp.shape(x)[0] % 2 != 0:
-            pop_dec = jnp.r_[pop_dec, x[-1:, :]]
-
-        return pop_dec, ex.State(key=key)
+    def __call__(self, key, x):
+        return polynomial(key, x, self.boundary, self.pro_m, self.dis_m)
```

### Comparing `evox-0.2.0/src/evox/operators/non_dominated_sort.py` & `evox-0.3.0/src/evox/operators/non_dominated_sort.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/operators/sampling/latin_hypercude.py` & `evox-0.3.0/src/evox/operators/sampling/latin_hypercude.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import jax
 import jax.numpy as jnp
+from evox import jit_class
 
 
+@jit_class
 class LatinHypercubeSampling:
     """Latin hypercube sampling"""
 
     def __init__(self, n=None, m=None):
         self.n = n
         self.m = m
 
-    def random(self, key):
-        key, subkey = jax.random.split(key)
-        subkeys = jax.random.split(subkey, self.m)
-        w = jax.random.uniform(subkey, shape=(self.n, self.m))
+    def __call__(self, key):
+        subkeys = jax.random.split(key, self.m)
+        w = jax.random.uniform(key, shape=(self.n, self.m))
         parm = jnp.tile(jnp.arange(1, self.n+1), (self.m, 1))
         parm = jax.vmap(jax.random.permutation, in_axes=(0, 0), out_axes=1)(subkeys, parm)
         w = (parm - w) / self.n
         n = self.n
-        return  w, n
+        return w, n
+
```

### Comparing `evox-0.2.0/src/evox/operators/sampling/uniform.py` & `evox-0.3.0/src/evox/operators/sampling/uniform.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import evox as ex
 import jax
 import jax.numpy as jnp
 from itertools import combinations as n_choose_k
-# from evox.utils import comb
 from scipy.special import comb
 
+import evox
 
+
+@evox.jit_class
 class UniformSampling:
     """Uniform sampling use Das and Dennis's method, Deb and Jain's method."""
 
     def __init__(self, n=None, m=None):
         self.n = n
         self.m = m
 
-
-    def random(self):
+    def __call__(self):
         h1 = 1
         while comb(h1 + self.m, self.m - 1) <= self.n:
             h1 += 1
 
         w = jnp.array(list(n_choose_k(range(1, h1 + self.m), self.m-1))) - \
             jnp.tile(jnp.array(range(self.m-1)), (comb(h1+self.m-1, self.m-1).astype(int), 1)) - 1
         w = (jnp.c_[w, jnp.zeros((jnp.shape(w)[0], 1)) + h1] -
@@ -31,8 +31,9 @@
                 w2 = jnp.array(list(n_choose_k(range(1, h2+self.m), self.m-1))) - \
                     jnp.tile(jnp.array(range(self.m - 1)), (comb(h2+self.m-1, self.m-1).astype(int), 1)) - 1
                 w2 = (jnp.c_[w2, jnp.zeros((jnp.shape(w2)[0], 1))+h2] -
                     jnp.c_[jnp.zeros((jnp.shape(w2)[0], 1)), w2]) / h2
                 w = jnp.r_[w, w2/2. + 1./(2.*self.m)]
         w = jnp.maximum(w, 1e-6)
         n = jnp.shape(w)[0]
-        return  w, n
+        return w, n
+
```

### Comparing `evox-0.2.0/src/evox/operators/selection/rvea_selection.py` & `evox-0.3.0/src/evox/operators/selection/rvea_selection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,55 @@
-import evox as ex
-import jax
 import jax.numpy as jnp
-import jax.experimental.host_callback as hcb
+from jax import jit, lax
 from evox.utils import cos_dist
+from evox import jit_class
 
 
-@ex.jit_class
-class ReferenceVectorGuidedSelection(ex.Operator):
-    """Reference vector guided environmental selection.
+@jit
+def ref_vec_guided(x, v, theta):
+    n, m = jnp.shape(x)
+    nv = jnp.shape(v)[0]
+    obj = x
 
-    """
+    obj -= jnp.tile(jnp.min(obj, axis=0), (n, 1))
 
-    def __init__(self, x=None, v=None, theta=None):
-        self.x = x
-        self.v = v
-        self.theta = theta
+    cosine = cos_dist(v, v)
+    cosine = jnp.where(jnp.eye(jnp.shape(cosine)[0], dtype=bool), 0, cosine)
+    gamma = jnp.min(jnp.arccos(cosine), axis=1)
 
-    def setup(self, key):
-        return ex.State(key=key)
+    angle = jnp.arccos(cos_dist(obj, v))
 
-    def __call__(self, state, x, v, theta):
-        self.x = x
-        self.v = v
-        self.theta = theta
-        key, subkey = jax.random.split(state.key)
-        n, m = jnp.shape(self.x)
-        nv = jnp.shape(self.v)[0]
-        obj = self.x
+    associate = jnp.argmin(angle, axis=1)
 
-        obj -= jnp.tile(jnp.min(obj, axis=0), (n, 1))
+    next_ind = jnp.full(nv, -1)
+    is_null = jnp.sum(next_ind)
 
-        cosine = cos_dist(self.v, self.v)
-        cosine = jnp.where(jnp.eye(jnp.shape(cosine)[0], dtype=bool), 0, cosine) 
-        gamma = jnp.min(jnp.arccos(cosine), axis=1)
+    def update_next(i, sub_index, next_ind):
+        apd = (1 + m * theta * angle[sub_index, i] / gamma[i]) * jnp.sqrt(
+            jnp.sum(obj[sub_index, :] ** 2, axis=1)
+        )
+        apd_max = jnp.max(apd)
+        noise = jnp.where(sub_index == -1, apd_max, 0)
+        best = jnp.argmin(apd + noise)
+        next_ind = next_ind.at[i].set(sub_index[best.astype(int)])
+        return next_ind
 
-        angle = jnp.arccos(cos_dist(obj, self.v))
+    def no_update(_i, _sub_index, next_ind):
+        return next_ind
 
-        associate = jnp.argmin(angle, axis=1)
+    def body_fun(i, val):
+        sub_index = jnp.where(associate == i, size=nv, fill_value=-1)[0]
+        next_ind = lax.cond(
+            jnp.sum(sub_index) != is_null, update_next, no_update, i, sub_index, val
+        )
+        return next_ind
 
-        next_ind = jnp.full(nv, -1)
-        is_null = jnp.sum(next_ind)
-
-
-        def update_next(i, sub_index ,next_ind):
-            apd = (1+m*theta*angle[sub_index, i]/gamma[i]) * jnp.sqrt(jnp.sum(obj[sub_index, :]**2, axis=1))
-            apd_max = jnp.max(apd)
-            noise = jnp.where(sub_index==-1, apd_max, 0)
-            best = jnp.argmin(apd+noise)
-            next_ind = next_ind.at[i].set(sub_index[best.astype(int)])
-            return next_ind
-
-        def no_update(i, sub_index ,next_ind):
-            return next_ind
-
-        def body_fun(i, val):
-            sub_index = jnp.where(associate == i, size=nv, fill_value=-1)[0]
-            next_ind = jax.lax.cond(jnp.sum(sub_index) != is_null, update_next, no_update, i, sub_index, val)
-            return next_ind
-
-        next_ind = jax.lax.fori_loop(0, nv, body_fun, next_ind)
-
-        return next_ind, ex.State(key=key)
+    next_ind = lax.fori_loop(0, nv, body_fun, next_ind)
 
+    return next_ind
 
 
+@jit_class
+class ReferenceVectorGuided:
+    """Reference vector guided environmental selection."""
+    def __call__(self, x, v, theta):
+        return ref_vec_guided(x, v, theta)
```

### Comparing `evox-0.2.0/src/evox/operators/selection/tournament.py` & `evox-0.3.0/src/evox/operators/selection/tournament.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,69 @@
 from typing import Callable
 
-import evox as ex
-import jax
 import jax.numpy as jnp
+from jax import random, jit, vmap
+from evox import jit_class
 
+from functools import partial
 
-@ex.jit_class
-class TournamentSelection(ex.Operator):
+
+@partial(jit, static_argnums=[3, 4, 5])
+def tournament_single_fit(key, pop, fit, n_round, tournament_func, tournament_size):
+
+    chosen = random.choice(key, n_round, shape=(n_round, tournament_size))
+    candidates_fitness = fit[chosen, ...]
+    winner_indices = vmap(tournament_func)(candidates_fitness)
+    index = chosen[jnp.arange(n_round), winner_indices]
+    return pop[index], index
+
+
+@partial(jit, static_argnums=[3, 4, 5])
+def tournament_multi_fit(key, pop, fit, n_round, tournament_func, tournament_size):
+
+    chosen = random.choice(key, n_round, shape=(n_round, tournament_size))
+    candidates_fitness = fit[chosen, ...]
+    winner_indices = vmap(jnp.lexsort)(jnp.transpose(candidates_fitness, (0, 2, 1)))
+    index = chosen[jnp.arange(n_round), winner_indices[:, 0]]
+    return pop[index], index
+
+
+@jit_class
+class Tournament:
     """Tournament selection"""
 
     def __init__(
-        self, num_round: int, tournament_func: Callable = jnp.argmax, tournament_size: int = 2
+        self,
+        n_round: int,
+        tournament_func: Callable = jnp.argmin,
+        tournament_size: int = 2,
     ):
         """
         Parameters
         ----------
         num_round
             Number of time the tournament will hold.
         tournament_func
             A function used to determine the winner of the tournament.
             The function must accept a array of shape (N, ) or (N, K),
             where N is the number of individuals and K is the number of objectives,
             and return a single integer indicating the index of the winner.
         tournament_size
             Number of individuals in one tournament
         """
-        self.num_round = num_round
+        self.n_round = n_round
         self.tournament_func = tournament_func
         self.tournament_size = tournament_size
 
-    def setup(self, key):
-        return ex.State(key=key)
+    def __call__(self, key, pop, *args):
+
+        if len(args) == 1:
+            fit = args[0]
+            return tournament_single_fit(
+            key, pop, fit, self.n_round, self.tournament_func, self.tournament_size
+            )
+        else:
+            fit = jnp.c_[args]
+            return tournament_multi_fit(
+            key, pop, fit, self.n_round, self.tournament_func, self.tournament_size
+            )
 
-    def __call__(self, state, x, fitness):
-        key, subkey = jax.random.split(state.key)
-        # select num_round times and each time
-        # k individuals to form candidates
-        chosen = jax.random.choice(subkey, self.num_round, shape=(
-            self.num_round, self.tournament_size))
-        # candidates = x[chosen, ...]
-        candidates_fitness = fitness[chosen, ...]
-        winner_indices = jax.vmap(self.tournament_func)(candidates_fitness)
-        index = jnp.diagonal(chosen[:, winner_indices])
-        return x[index], ex.State(key=key)
```

### Comparing `evox-0.2.0/src/evox/pipelines/distributed.py` & `evox-0.3.0/src/evox/pipelines/distributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         leaves0, _treedef = tree_flatten(states[0])
         for state in states:
             leaves, _treedef = tree_flatten(state)
             chex.assert_trees_all_close(leaves0, leaves)
         return True
 
 
-class DistributedPipeline(Stateful):
+class RayDistributedWorkflow(Stateful):
     def __init__(
         self,
         algorithm: Algorithm,
         problem: Problem,
         pop_size: int,
         num_workers: int,
         options: dict = {},
```

### Comparing `evox-0.2.0/src/evox/pipelines/gym.py` & `evox-0.3.0/src/evox/pipelines/gym.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/pipelines/multidevice.py` & `evox-0.3.0/src/evox/pipelines/multidevice.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/pipelines/standard.py` & `evox-0.3.0/src/evox/pipelines/standard.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/problems/classic/ackley.py` & `evox-0.3.0/src/evox/problems/classic/ackley.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/problems/classic/dtlz.py` & `evox-0.3.0/src/evox/problems/classic/dtlz.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import jax
 import jax.numpy as jnp
-import evox as ex
+from evox import Problem, State, jit_class
 from evox.operators.sampling import UniformSampling, LatinHypercubeSampling
 import chex
-from functools import partial
+import pkgutil, json
 
 
-class DTLZ(ex.Problem):
+@jit_class
+class DTLZ(Problem):
     """DTLZ"""
 
-    def __init__(self, d=None, m=None, ref_num=1000,):
+    def __init__(self, d=None, m=None, ref_num=1000):
         self.d = d
         self.m = m
         self._dtlz = None
         self.ref_num = ref_num
+        self.sample = UniformSampling(self.ref_num * self.m, self.m)
 
     def setup(self, key):
-        return ex.State(key=key)
+        return State(key=key)
 
     def evaluate(self, state: chex.PyTreeDef, X: chex.Array):
         chex.assert_type(X, float)
-        chex.assert_shape(X, (None, self.n))
+        chex.assert_shape(X, (None, self.d))
         return jax.jit(jax.vmap(self._dtlz))(X), state
 
     def pf(self, state: chex.PyTreeDef):
-        f = UniformSampling(self.ref_num * self.m, self.m).random()[0] / 2
-        # f = LatinHypercubeSampling(self.ref_num * self.m, self.m).random(state.key)[0] / 2
+        f = self.sample()[0] / 2
         return f, state
 
 
 class DTLZ1(DTLZ):
     def __init__(self, d=None, m=None, ref_num=100):
         if m is None:
             self.m = 3
@@ -67,23 +68,23 @@
             self.d = d
         super().__init__(d, m, ref_num)
 
     def evaluate(self, state: chex.PyTreeDef, X: chex.Array):
         m = self.m
         g = jnp.sum((X[:, m - 1:] - 0.5) ** 2, axis=1, keepdims=True)
         f = jnp.tile(1 + g, (1, m)) * jnp.fliplr(jnp.cumprod(jnp.c_[jnp.ones((jnp.shape(g)[0], 1)),
-                                                                    jnp.cos(X[:, :m - 1] * jnp.pi / 2)], axis=1)) * jnp.c_[jnp.ones((jnp.shape(g)[0], 1)), jnp.sin(
-                                                                        X[:, m - 2::-1] * jnp.pi / 2)]
+        jnp.cos(X[:, :m - 1] * jnp.pi / 2)], axis=1)) * jnp.c_[jnp.ones((jnp.shape(g)[0], 1)), jnp.sin(
+            X[:, m - 2::-1] * jnp.pi / 2)]
 
         return f, state
 
     def pf(self, state: chex.PyTreeDef):
-        f = UniformSampling(self.ref_num * self.m, self.m).random()[0]
+        f = self.sample()[0]
         f /= jnp.tile(jnp.sqrt(jnp.sum(f ** 2, axis=1,
-                      keepdims=True)), (1, self.m))
+                                       keepdims=True)), (1, self.m))
         return f, state
 
 
 class DTLZ3(DTLZ2):
     def __init__(self, d=None, m=None, ref_num=1000):
         super().__init__(d, m, ref_num)
 
@@ -91,31 +92,29 @@
         n, d = jnp.shape(X)
         m = self.m
         g = 100 * (d - m + 1 + jnp.sum(
             ((X[:, m - 1:] - 0.5) ** 2 -
              jnp.cos(20 * jnp.pi * (X[:, m - 1:] - 0.5))),
             axis=1, keepdims=True))
         f = jnp.tile(1 + g, (1, m)) * jnp.fliplr(jnp.cumprod(jnp.c_[jnp.ones((n, 1)),
-                                                                    jnp.cos(X[:, :m - 1] * jnp.pi / 2)],
-                                                             axis=1)) * \
-            jnp.c_[jnp.ones((n, 1)), jnp.sin(X[:, m - 2::-1] * jnp.pi / 2)]
+        jnp.cos(X[:, :m - 1] * jnp.pi / 2)], axis=1)) * jnp.c_[jnp.ones((n, 1)), jnp.sin(X[:, m - 2::-1] * jnp.pi / 2)]
 
         return f, state
 
 
 class DTLZ4(DTLZ2):
     def __init__(self, d=None, m=None, ref_num=1000):
         super().__init__(d, m, ref_num)
 
     def evaluate(self, state: chex.PyTreeDef, X: chex.Array):
         m = self.m
         X = X.at[:, :m - 1].power(100)
         g = jnp.sum((X[:, m - 1:] - 0.5) ** 2, axis=1, keepdims=True)
         f = jnp.tile(1 + g, (1, m)) * jnp.fliplr(jnp.cumprod(jnp.c_[jnp.ones((jnp.shape(g)[0], 1)),
-                                                                    jnp.cos(X[:, :m - 1] * jnp.pi / 2)],
+        jnp.cos(X[:, :m - 1] * jnp.pi / 2)],
                                                              axis=1)) * \
             jnp.c_[jnp.ones((jnp.shape(g)[0], 1)), jnp.sin(
                 X[:, m - 2::-1] * jnp.pi / 2)]
 
         return f, state
 
 
@@ -133,28 +132,28 @@
         super().__init__(d, m, ref_num)
 
     def evaluate(self, state: chex.PyTreeDef, X: chex.Array):
         m = self.m
         g = jnp.sum((X[:, m - 1:] - 0.5) ** 2, axis=1, keepdims=True)
         temp = jnp.tile(g, (1, m - 2))
         X = X.at[:, 1:m - 1].set((1 + 2 * temp *
-                                 X[:, 1:m - 1]) / (2 + 2 * temp))
+                                  X[:, 1:m - 1]) / (2 + 2 * temp))
         f = jnp.tile(1 + g, (1, m)) * jnp.fliplr(jnp.cumprod(jnp.c_[jnp.ones((jnp.shape(g)[0], 1)),
-                                                                    jnp.cos(X[:, :m - 1] * jnp.pi / 2)],
+        jnp.cos(X[:, :m - 1] * jnp.pi / 2)],
                                                              axis=1)) * \
             jnp.c_[jnp.ones((jnp.shape(g)[0], 1)), jnp.sin(
                 X[:, m - 2::-1] * jnp.pi / 2)]
         return f, state
 
     def pf(self, state: chex.PyTreeDef):
         n = self.ref_num * self.m
         f = jnp.vstack((jnp.hstack(((jnp.arange(0, 1, 1. / (n - 1))), 1.)),
-                       jnp.hstack(((jnp.arange(1, 0, -1. / (n - 1))), 0.)))).T
+                        jnp.hstack(((jnp.arange(1, 0, -1. / (n - 1))), 0.)))).T
         f /= jnp.tile(jnp.sqrt(jnp.sum(f ** 2, axis=1,
-                      keepdims=True)), (1, jnp.shape(f)[1]))
+                                       keepdims=True)), (1, jnp.shape(f)[1]))
 
         for i in range(self.m - 2):
             f = jnp.c_[f[:, 0], f]
 
         f = f / jnp.sqrt(2) * jnp.tile(jnp.hstack((self.m - 2,
                                                    jnp.arange(self.m - 2, -1, -1))), (jnp.shape(f)[0], 1))
         return f, state
@@ -173,29 +172,29 @@
         super().__init__(d, m, ref_num)
 
     def evaluate(self, state: chex.PyTreeDef, X: chex.Array):
         m = self.m
         g = jnp.sum((X[:, m - 1:] ** 0.1), axis=1, keepdims=True)
         temp = jnp.tile(g, (1, m - 2))
         X = X.at[:, 1:m - 1].set((1 + 2 * temp *
-                                 X[:, 1:m - 1]) / (2 + 2 * temp))
+                                  X[:, 1:m - 1]) / (2 + 2 * temp))
 
         f = jnp.tile(1 + g, (1, m)) * jnp.fliplr(jnp.cumprod(jnp.c_[jnp.ones((jnp.shape(g)[0], 1)),
-                                                                    jnp.cos(X[:, :m - 1] * jnp.pi / 2)],
+        jnp.cos(X[:, :m - 1] * jnp.pi / 2)],
                                                              axis=1)) * \
             jnp.c_[jnp.ones((jnp.shape(g)[0], 1)), jnp.sin(
                 X[:, m - 2::-1] * jnp.pi / 2)]
         return f, state
 
     def pf(self, state: chex.PyTreeDef):
         n = self.ref_num * self.m
         f = jnp.vstack((jnp.hstack(((jnp.arange(0, 1, 1. / (n - 1))), 1.)),
-                       jnp.hstack(((jnp.arange(1, 0, -1. / (n - 1))), 0.)))).T
+                        jnp.hstack(((jnp.arange(1, 0, -1. / (n - 1))), 0.)))).T
         f /= jnp.tile(jnp.sqrt(jnp.sum(f ** 2, axis=1,
-                      keepdims=True)), (1, jnp.shape(f)[1]))
+                                       keepdims=True)), (1, jnp.shape(f)[1]))
 
         for i in range(self.m - 2):
             f = jnp.c_[f[:, 0], f]
 
         f = f / jnp.sqrt(2) * jnp.tile(jnp.hstack((self.m - 2,
                                                    jnp.arange(self.m - 2, -1, -1))), (jnp.shape(f)[0], 1))
         return f, state
@@ -213,79 +212,19 @@
             self.d = d
         super().__init__(d, m, ref_num)
 
     def evaluate(self, state: chex.PyTreeDef, X: chex.Array):
         n, d = jnp.shape(X)
         m = self.m
         f = jnp.zeros((n, m))
-        g = 1 + jnp.mean(X[:, m-1:], axis=1, keepdims=True)
-        f = f.at[:, m-1].set((1 + g) * (m - jnp.sum(X[:, :m-1] / (1 + jnp.tile(g, (1, m-1)))
-                                                    * (1 + jnp.sin(3 * jnp.pi * X[:, :m-1])), axis=1, keepdims=True)))
-
+        g = 1 + 9 * jnp.mean(X[:, m - 1:], axis=1, keepdims=True)
+        f = f.at[:, :m - 1].set(X[:, :m - 1])
+        f = f.at[:, m - 1:].set((1 + g) * (m - jnp.sum(f[:, :m - 1] / (1 + jnp.tile(g, (1, m - 1)))
+                                                       * (1 + jnp.sin(3 * jnp.pi * f[:, :m - 1])), axis=1,
+                                                       keepdims=True)))
         return f, state
 
     def pf(self, state: chex.PyTreeDef):
-        intervel = jnp.array([0, 0.251412, 0.631627, 0.859401])
-        median = (intervel[1] - intervel[0]) / (intervel[3] -
-                                                intervel[2] + intervel[1] - intervel[0])
-        # ReplicatePoint function
-        return super().pf(state)
-
-
-class DTLZ8(DTLZ):
-    def __init__(self, d=None, m=None, ref_num=1000):
-        if m is None:
-            self.m = 2
-        else:
-            self.m = m
-
-        if d is None:
-            self.d = self.m*10
-        else:
-            self.d = d
-        super().__init__(d, m, ref_num)
-
-    def evaluate(self, state: chex.PyTreeDef, X: chex.Array):
-        n, d = jnp.shape(X)
-        m = self.m
-        f = jnp.zeros((n, m))
-        for i in range(m):
-            f = f.at[:, i].set(
-                jnp.mean(X[:, int(i*d/m):int((i+1)*d/m)], axis=1, keepdims=True))
-
-        return f, state
-
-    def pf(self, state: chex.PyTreeDef):
-        return super().pf(state)
-
-
-class DTLZ9(DTLZ):
-    def __init__(self, d=None, m=None, ref_num=1000):
-        if m is None:
-            self.m = 2
-        else:
-            self.m = m
-
-        if d is None:
-            self.d = self.m*10
-        else:
-            self.d = d
-        self.d = int(jnp.ceil(self.d/self.m)*self.m)
-        super().__init__(d, m, ref_num)
-
-    def evaluate(self, state: chex.PyTreeDef, X: chex.Array):
-        n, d = jnp.shape(X)
-        X = X**0.1
-        m = self.m
-        f = jnp.zeros([n, m])
-        for i in range(m):
-            f = f.at[:, i].set(jnp.sum(X[:, int(i*d/m):int((i+1)*d/m)],
-                                       axis=1, keepdims=True))
-        return f, state
-
-    def pf(self, state: chex.PyTreeDef):
-        n = self.ref_num * self.m
-        temp = jnp.vstack(
-            (jnp.hstack(((jnp.arange(0, 1, 1. / (n - 1))), 1.)))).T
-        f = jnp.c_[jnp.tile(jnp.cos(0.5*jnp.pi*temp),
-                            (1, self.m-1)), jnp.sin(0.5*jnp.pi*temp)]
-        return f, state
+        data_bytes = pkgutil.get_data('evox', 'problems/classic/data/dtlz7_pf.json')
+        data = data_bytes.decode()
+        pf = json.loads(data)
+        return jnp.array(pf), state
```

### Comparing `evox-0.2.0/src/evox/problems/classic/zdt.py` & `evox-0.3.0/src/evox/problems/classic/zdt.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import jax
 import jax.numpy as jnp
 from functools import partial
-import evox as ex
+from evox import jit_class, Problem
 import chex
 
 
 def _generic_zdt(f1, g, h, x):
     f1_x = f1(x)
     g_x = g(x)
     return jnp.array([f1_x, g_x * h(f1(x), g_x)])
 
 
-@ex.jit_class
-class ZDT(ex.Problem):
+@jit_class
+class ZDT(Problem):
     def __init__(self, n, ref_num=100):
         self.n = n
         self._zdt = None
         self.ref_num = ref_num
 
     def evaluate(self, state: chex.PyTreeDef, X: jax.Array):
         chex.assert_type(X, float)
@@ -33,46 +33,63 @@
         super().__init__(n)
         f1 = lambda x: x[0]
         g = lambda x: 1 + 9 * jnp.mean(x[1:])
         h = lambda f1, g: 1 - jnp.sqrt(f1 / g)
         self._zdt = partial(_generic_zdt, f1, g, h)
 
 
-
 class ZDT2(ZDT):
     def __init__(self, n):
         super().__init__(n)
         f1 = lambda x: x[0]
         g = lambda x: 1 + 9 * jnp.mean(x[1:])
         h = lambda f1, g: 1 - (f1 / g) ** 2
         self._zdt = partial(_generic_zdt, f1, g, h)
 
     def pf(self, state: chex.PyTreeDef):
         x = jnp.linspace(0, 1, self.ref_num)
         return jnp.c_[x, 1 - x**2], state
 
 
-
 class ZDT3(ZDT):
     def __init__(self, n):
         super().__init__(n)
         f1 = lambda x: x[0]
         g = lambda x: 1 + 9 * jnp.mean(x[1:])
         h = lambda f1, g: 1 - jnp.sqrt(f1 / g) - (f1 / g) * jnp.sin(10 * jnp.pi * f1)
         self._zdt = partial(_generic_zdt, f1, g, h)
 
     def pf(self, state: chex.PyTreeDef):
-        pass
+        r = jnp.array([[0, 0.0830], [0.1822, 0.2577], [0.4093, 0.4538], [0.6183, 0.6525], [0.8233, 0.8518]])
+
+        f1 = jnp.linspace(r[:, 0], r[:, 1], int(self.ref_num / len(r)))
+        f2 = 1 - jnp.sqrt(f1) - f1 * jnp.sin(10 * jnp.pi * f1)
+        pf = jnp.array([f1, f2]).T
+        pf = jnp.row_stack(pf)
+        return pf, state
 
 
 class ZDT4(ZDT):
     def __init__(self, n):
         super().__init__(n)
         f1 = lambda x: x[0]
         g = (
             lambda x: 1
             + 10 * (self.n - 1)
             + jnp.sum(x[1:] ** 2 - 10 * jnp.cos(4 * jnp.pi * x[1:]))
         )
         h = lambda f1, g: 1 - jnp.sqrt(f1 / g)
         self._zdt = partial(_generic_zdt, f1, g, h)
 
+
+class ZDT6(ZDT):
+    def __init__(self, n):
+        super().__init__(n)
+        f1 = lambda x: 1 - jnp.exp(-4 * x[0]) * jnp.sin(6 * jnp.pi * x[0])**6
+        g = lambda x: 1 + 9 * (jnp.sum(x[1:]) / 9)**0.25
+        h = lambda f1, g: 1 - (f1 / g)**2
+        self._zdt = partial(_generic_zdt, f1, g, h)
+
+    def pf(self, state: chex.PyTreeDef):
+        min_f1 = 0.280775
+        f1 = jnp.linspace(min_f1, 1, self.ref_num)
+        return jnp.c_[f1, 1 - f1**2], state
```

### Comparing `evox-0.2.0/src/evox/problems/neuroevolution/torchvision_dataset.py` & `evox-0.3.0/src/evox/problems/neuroevolution/torchvision_dataset.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/problems/rl/__init__.py` & `evox-0.3.0/src/evox/problems/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/problems/rl/gym.py` & `evox-0.3.0/src/evox/problems/rl/gym.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/problems/rl/gym_mo.py` & `evox-0.3.0/src/evox/problems/rl/gym_mo.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/src/evox/utils.py` & `evox-0.3.0/src/evox/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections.abc import Iterable
 from functools import partial
 from typing import Union, List
 
-import jax
+from jax import vmap
 import jax.numpy as jnp
 from jax.tree_util import tree_flatten, tree_leaves, tree_unflatten
 
 from .core.module import *
 
 
 def min_by(
@@ -32,15 +32,15 @@
 @jax.jit
 def pair_distance(a, b):
     return jnp.linalg.norm(a - b, axis=0)
 
 
 @jax.jit
 def euclidean_dis(x, y):
-    return jax.vmap(lambda _x: jax.vmap(lambda _y: pair_distance(_x, _y))(y))(x)
+    return vmap(lambda _x: vmap(lambda _y: pair_distance(_x, _y))(y))(x)
 
 
 @jax.jit
 def pair_max(a, b):
     return jnp.max(a - b, axis=0)
 
 
@@ -49,31 +49,38 @@
     return jnp.dot(
         x / jnp.linalg.norm(x, axis=-1, keepdims=True),
         (y / jnp.linalg.norm(y, axis=-1, keepdims=True)).T,
     )
 
 
 @jax.jit
-def cal_indicator(x, y):
-    return jax.vmap(lambda _x: jax.vmap(lambda _y: pair_max(_x, _y))(y))(x)
+def cal_max(x, y):
+    return vmap(lambda _x: vmap(lambda _y: pair_max(_x, _y))(y))(x)
 
 
 @jax.jit
-def cal_fitness(pop_obj, kappa):
-    n = jnp.shape(pop_obj)[0]
-    pop_obj = (pop_obj - jnp.tile(jnp.min(pop_obj), (n, 1))) / (
-        jnp.tile(jnp.max(pop_obj) - jnp.min(pop_obj), (n, 1))
-    )
-    I = cal_indicator(pop_obj, pop_obj)
+def _dominate(x, y):
+    """return true if x dominate y (x < y) and false elsewise."""
+    return jnp.all(x <= y) & jnp.any(x < y)
+
 
-    C = jnp.max(jnp.abs(I), axis=0)
+@jax.jit
+def _dominate_relation(x, y):
+    """return a matrix A, where A_{ij} is True if x_i donminate y_j"""
+    return vmap(lambda _x: vmap(lambda _y: _dominate(_x, _y))(y))(x)
 
-    fitness = jnp.sum(-jnp.exp(-I / jnp.tile(C, (n, 1)) / kappa), axis=0) + 1
 
-    return fitness, I, C
+@jax.jit
+def new_dist_mat(xs : jax.Array) -> jax.Array:
+    assert len(xs.shape) == 2
+    xx = jax.vmap(lambda x: jnp.dot(x, x))(xs)
+    x2 = jnp.broadcast_to(xx[:, jnp.newaxis], (xx.shape[0], xx.shape[0]))
+    y2 = jnp.broadcast_to(xx[jnp.newaxis, :], (xx.shape[0], xx.shape[0]))
+    xy = jnp.matmul(xs, xs.T)
+    return jnp.sqrt(jnp.maximum(x2 + y2 - 2 * xy, 0))
 
 
 def compose(*functions):
     # if argument is a single Iterable like list or tuple,
     # treat it as a list of functions
     if len(functions) == 1 and isinstance(functions[0], Iterable):
         functions = functions[0]
```

### Comparing `evox-0.2.0/src/evox.egg-info/PKG-INFO` & `evox-0.3.0/src/evox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evox
-Version: 0.2.0
+Version: 0.3.0
 Summary: evox
 Author-email: Bill Huang <bill.huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang <zhenyuliang97@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, EMI-Group
         All rights reserved.
         
@@ -45,15 +45,15 @@
 Provides-Extra: gym
 Provides-Extra: neuroevolution
 Provides-Extra: distributed
 Provides-Extra: full
 License-File: LICENSE
 
 <h1 align="center">
-  <img src=./logo.png alt="Logo" height="24em"/>
+  <img src=./docs/source/_static/evox_logo.png alt="Logo" height="24em"/>
   <strong>EvoX</strong>
   <br>
   A Distributed GPU-accelerated Library towards Scalable Evolutionary Computation
 </h1>
 
 <div align="center">
   <a href="https://evox.readthedocs.io/">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evox Version: 0.2.0 Summary: evox Author-email:
+Metadata-Version: 2.1 Name: evox Version: 0.3.0 Summary: evox Author-email:
 Bill Huang
 huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang
 gmail.com> License: BSD 3-Clause License Copyright (c) 2022, EMI-Group All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
```

### Comparing `evox-0.2.0/src/evox.egg-info/SOURCES.txt` & `evox-0.3.0/src/evox.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,24 @@
 src/evox.egg-info/top_level.txt
 src/evox/algorithms/__init__.py
 src/evox/algorithms/containers/__init__.py
 src/evox/algorithms/containers/clustered_algorithm.py
 src/evox/algorithms/containers/coevolution.py
 src/evox/algorithms/containers/tree_algorithm.py
 src/evox/algorithms/mo/__init__.py
+src/evox/algorithms/mo/eagmoead.py
+src/evox/algorithms/mo/hype.py
 src/evox/algorithms/mo/ibea.py
 src/evox/algorithms/mo/moead.py
+src/evox/algorithms/mo/moeaddra.py
+src/evox/algorithms/mo/moeadm2m.py
 src/evox/algorithms/mo/nsga2.py
+src/evox/algorithms/mo/nsga3.py
 src/evox/algorithms/mo/rvea.py
+src/evox/algorithms/mo/spea2.py
 src/evox/algorithms/so/__init__.py
 src/evox/algorithms/so/cma_es.py
 src/evox/algorithms/so/cso.py
 src/evox/algorithms/so/de.py
 src/evox/algorithms/so/nes.py
 src/evox/algorithms/so/open_es.py
 src/evox/algorithms/so/pgpe.py
@@ -32,14 +38,15 @@
 src/evox/core/operator.py
 src/evox/core/problem.py
 src/evox/core/state.py
 src/evox/metrics/__init__.py
 src/evox/metrics/hypervolume.py
 src/evox/metrics/igd.py
 src/evox/monitors/__init__.py
+src/evox/monitors/evoxvis_monitor.py
 src/evox/monitors/fitness.py
 src/evox/monitors/gym.py
 src/evox/monitors/population.py
 src/evox/monitors/std_mo_monitor.py
 src/evox/monitors/std_so_monitor.py
 src/evox/operators/__init__.py
 src/evox/operators/crowding_distance_sort.py
@@ -54,22 +61,26 @@
 src/evox/operators/mutation/bitflip.py
 src/evox/operators/mutation/gaussian.py
 src/evox/operators/mutation/pm_mutation.py
 src/evox/operators/sampling/__init__.py
 src/evox/operators/sampling/latin_hypercude.py
 src/evox/operators/sampling/uniform.py
 src/evox/operators/selection/__init__.py
+src/evox/operators/selection/non_dominate.py
+src/evox/operators/selection/roulette_wheel.py
 src/evox/operators/selection/rvea_selection.py
+src/evox/operators/selection/topk_fit.py
 src/evox/operators/selection/tournament.py
 src/evox/operators/selection/uniform_random.py
 src/evox/pipelines/__init__.py
 src/evox/pipelines/distributed.py
 src/evox/pipelines/gym.py
 src/evox/pipelines/multidevice.py
 src/evox/pipelines/standard.py
+src/evox/pipelines/uni_workflow.py
 src/evox/problems/__init__.py
 src/evox/problems/classic/__init__.py
 src/evox/problems/classic/ackley.py
 src/evox/problems/classic/dtlz.py
 src/evox/problems/classic/griewank.py
 src/evox/problems/classic/rastrigin.py
 src/evox/problems/classic/rosenbrock.py
@@ -88,8 +99,9 @@
 tests/test_gym.py
 tests/test_monitors.py
 tests/test_multi_objective_algorithms.py
 tests/test_neuroevolution.py
 tests/test_non_dominated_sort.py
 tests/test_single_objective_algorithms.py
 tests/test_state.py
+tests/test_uni_workflow.py
 tests/test_utils.py
```

### Comparing `evox-0.2.0/tests/test_classic_problems.py` & `evox-0.3.0/tests/test_classic_problems.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/tests/test_containers.py` & `evox-0.3.0/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/tests/test_crowding_distance.py` & `evox-0.3.0/tests/test_crowding_distance.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/tests/test_distributed_pipeline.py` & `evox-0.3.0/tests/test_uni_workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,30 @@
 import jax.numpy as jnp
 import pytest
 
 
 def test_distributed_cso():
     monitor = StdSOMonitor()
     # create a pipeline
-    pipeline = pipelines.DistributedPipeline(
+    pipeline = pipelines.UniWorkflow(
         algorithm=algorithms.CSO(
             lb=jnp.full(shape=(2,), fill_value=-32),
             ub=jnp.full(shape=(2,), fill_value=32),
             pop_size=20,
         ),
         problem=problems.classic.Ackley(),
-        pop_size=10,
-        num_workers=2,
-        global_fitness_transform=monitor.record_fit,
-        options={"num_cpus": 0.5, "num_gpus": 0},  # just for testing purpose
+        monitor=monitor
     )
     # init the pipeline
     key = jax.random.PRNGKey(42)
     state = pipeline.init(key)
+    state = pipeline.enable_multi_devices(state)
 
     # run the pipeline for 100 steps
     for i in range(100):
         state = pipeline.step(state)
 
     # the result should be close to 0
+    monitor.close()
     min_fitness = monitor.get_min_fitness()
     print(min_fitness)
     assert min_fitness < 1e-4
-    pipeline.health_check(state)
```

### Comparing `evox-0.2.0/tests/test_gym.py` & `evox-0.3.0/tests/test_gym.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/tests/test_monitors.py` & `evox-0.3.0/tests/test_monitors.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/tests/test_neuroevolution.py` & `evox-0.3.0/tests/test_neuroevolution.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/tests/test_non_dominated_sort.py` & `evox-0.3.0/tests/test_non_dominated_sort.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/tests/test_single_objective_algorithms.py` & `evox-0.3.0/tests/test_single_objective_algorithms.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/tests/test_state.py` & `evox-0.3.0/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `evox-0.2.0/tests/test_utils.py` & `evox-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

