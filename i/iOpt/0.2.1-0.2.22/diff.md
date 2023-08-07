# Comparing `tmp/iOpt-0.2.1.tar.gz` & `tmp/iOpt-0.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iOpt-0.2.1.tar", last modified: Thu Jun 29 07:15:58 2023, max compression
+gzip compressed data, was "iOpt-0.2.22.tar", last modified: Mon Aug  7 05:26:34 2023, max compression
```

## Comparing `iOpt-0.2.1.tar` & `iOpt-0.2.22.tar`

### file list

```diff
@@ -1,181 +1,182 @@
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.250923 iOpt-0.2.1/
--rw-r--r--   0 anton      (501) staff       (20)     1543 2023-04-21 14:01:15.000000 iOpt-0.2.1/LICENSE
--rw-r--r--   0 anton      (501) staff       (20)     7406 2023-06-29 07:15:58.250511 iOpt-0.2.1/PKG-INFO
--rw-r--r--   0 anton      (501) staff       (20)     6867 2023-04-25 16:30:22.000000 iOpt-0.2.1/README.md
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.177737 iOpt-0.2.1/examples/
--rw-r--r--   0 anton      (501) staff       (20)     1380 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/GKLS_example.py
--rw-r--r--   0 anton      (501) staff       (20)     1002 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/GKLS_timeout_example.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.178161 iOpt-0.2.1/examples/Genetic_algorithm/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.178451 iOpt-0.2.1/examples/Genetic_algorithm/TSP/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.179031 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/
--rw-r--r--   0 anton      (501) staff       (20)     1687 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Example_GA_TSP_Vary_Mutation.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.179476 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Problems/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Problems/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     3554 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Problems/ga_tsp_vary_mutation.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.180591 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/
--rw-r--r--   0 anton      (501) staff       (20)     1798 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Example_GA_TSP_Vary_Mutation_Population_Size.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.181042 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Problems/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Problems/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     4587 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Problems/ga_tsp_2d.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/TSP/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:15.000000 iOpt-0.2.1/examples/Genetic_algorithm/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     1288 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Grishagin_example.py
--rw-r--r--   0 anton      (501) staff       (20)     1210 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Hill_example.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.181369 iOpt-0.2.1/examples/Machine_learning/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.181673 iOpt-0.2.1/examples/Machine_learning/SVC/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.182616 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/
--rw-r--r--   0 anton      (501) staff       (20)     1509 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_kernel_coefficient.py
--rw-r--r--   0 anton      (501) staff       (20)     1548 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_regularization.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.183660 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/
--rw-r--r--   0 anton      (501) staff       (20)     3032 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Kernel.py
--rw-r--r--   0 anton      (501) staff       (20)     3108 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Regularization.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_1D/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.186064 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/
--rw-r--r--   0 anton      (501) staff       (20)     1482 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Example_2D_SVC.py
--rw-r--r--   0 anton      (501) staff       (20)     1563 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Example_2D_SVC_Industrial.py
--rw-r--r--   0 anton      (501) staff       (20)     1240 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Example_SVC_Float_Discrete.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.187239 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Problems/
--rw-r--r--   0 anton      (501) staff       (20)     3031 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Problems/SVC_2D_Float_Discrete.py
--rw-r--r--   0 anton      (501) staff       (20)     3065 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Problems/SVC_2d.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Problems/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_2D/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.195050 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/
--rw-r--r--   0 anton      (501) staff       (20)     1379 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/Example_SVC_Discrete_Param.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.195561 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/Problem/
--rw-r--r--   0 anton      (501) staff       (20)     3366 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/Problem/SVC_3D.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/Problem/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Machine_learning/SVC/_3D/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/SVC/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/Machine_learning/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     1238 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/RastriginInt_example.py
--rw-r--r--   0 anton      (501) staff       (20)     1462 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Rastrigin_example.py
--rw-r--r--   0 anton      (501) staff       (20)      894 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Shekel4_example.py
--rw-r--r--   0 anton      (501) staff       (20)     1245 2023-06-29 05:54:18.000000 iOpt-0.2.1/examples/Shekel_example.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.197132 iOpt-0.2.1/examples/console_output/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/console_output/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      607 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/console_output/example_custom_output.py
--rw-r--r--   0 anton      (501) staff       (20)      595 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/console_output/example_full_output.py
--rw-r--r--   0 anton      (501) staff       (20)      596 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/console_output/example_only_result_output.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.197442 iOpt-0.2.1/examples/dynamic_painters/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.197910 iOpt-0.2.1/examples/dynamic_painters/1D_examples/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/dynamic_painters/1D_examples/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      620 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/dynamic_painters/1D_examples/example_1D_with_objective_function.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.198452 iOpt-0.2.1/examples/dynamic_painters/2D_examples/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/dynamic_painters/2D_examples/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      778 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/dynamic_painters/2D_examples/example_2D_with_level_lines.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/dynamic_painters/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.199010 iOpt-0.2.1/examples/static_painters/
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.200788 iOpt-0.2.1/examples/static_painters/1D_examples/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/1D_examples/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      639 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_approximation.py
--rw-r--r--   0 anton      (501) staff       (20)      639 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_interpolation.py
--rw-r--r--   0 anton      (501) staff       (20)      636 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_objective_function_pointsInBottom_mode.py
--rw-r--r--   0 anton      (501) staff       (20)      637 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_only_points.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.202890 iOpt-0.2.1/examples/static_painters/2D_examples/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      774 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_1-dimension_section.py
--rw-r--r--   0 anton      (501) staff       (20)      666 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_approximation.py
--rw-r--r--   0 anton      (501) staff       (20)      666 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_interpolation.py
--rw-r--r--   0 anton      (501) staff       (20)      638 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_level_lines.py
--rw-r--r--   0 anton      (501) staff       (20)      670 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_level_lines_by_interpolation.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/examples/static_painters/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.212153 iOpt-0.2.1/iOpt/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.214550 iOpt-0.2.1/iOpt/evolvent/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/evolvent/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)    11432 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/evolvent/evolvent.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.219657 iOpt-0.2.1/iOpt/method/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/method/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     3291 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/calculator.py
--rw-r--r--   0 anton      (501) staff       (20)      359 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/icriterion_evaluate_method.py
--rw-r--r--   0 anton      (501) staff       (20)     7340 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/index_method.py
--rw-r--r--   0 anton      (501) staff       (20)     2194 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/index_method_calculator.py
--rw-r--r--   0 anton      (501) staff       (20)      577 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/method/listener.py
--rw-r--r--   0 anton      (501) staff       (20)    17783 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/method.py
--rw-r--r--   0 anton      (501) staff       (20)    12978 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/mixed_integer_method.py
--rw-r--r--   0 anton      (501) staff       (20)     1493 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/optim_task.py
--rw-r--r--   0 anton      (501) staff       (20)     3614 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/parallel_process.py
--rw-r--r--   0 anton      (501) staff       (20)     9748 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/process.py
--rw-r--r--   0 anton      (501) staff       (20)    24759 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/search_data.py
--rw-r--r--   0 anton      (501) staff       (20)      368 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/method/sol_value.py
--rw-r--r--   0 anton      (501) staff       (20)     3676 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/method/solverFactory.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.220071 iOpt-0.2.1/iOpt/output_system/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.221534 iOpt-0.2.1/iOpt/output_system/listeners/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/listeners/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     4695 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/listeners/animate_painters.py
--rw-r--r--   0 anton      (501) staff       (20)     2351 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/listeners/console_outputers.py
--rw-r--r--   0 anton      (501) staff       (20)    10166 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/listeners/static_painters.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.222069 iOpt-0.2.1/iOpt/output_system/outputers/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/outputers/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     8761 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/outputers/console_outputer.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.230116 iOpt-0.2.1/iOpt/output_system/painters/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/painters/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     5164 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/painters/animate_painters.py
--rw-r--r--   0 anton      (501) staff       (20)      389 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/painters/painter.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.230721 iOpt-0.2.1/iOpt/output_system/painters/plotters/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/iOpt/output_system/painters/plotters/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)    19460 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/painters/plotters/plotters.py
--rw-r--r--   0 anton      (501) staff       (20)    12090 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/output_system/painters/static_painters.py
--rw-r--r--   0 anton      (501) staff       (20)     1661 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/problem.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.231305 iOpt-0.2.1/iOpt/routine/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/routine/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      843 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/routine/timeout.py
--rw-r--r--   0 anton      (501) staff       (20)     1424 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/solution.py
--rw-r--r--   0 anton      (501) staff       (20)     9049 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/solver.py
--rw-r--r--   0 anton      (501) staff       (20)     3159 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/solver_parametrs.py
--rw-r--r--   0 anton      (501) staff       (20)      906 2023-06-29 05:54:18.000000 iOpt-0.2.1/iOpt/trial.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.214026 iOpt-0.2.1/iOpt.egg-info/
--rw-r--r--   0 anton      (501) staff       (20)     7406 2023-06-29 07:15:58.000000 iOpt-0.2.1/iOpt.egg-info/PKG-INFO
--rw-r--r--   0 anton      (501) staff       (20)     5506 2023-06-29 07:15:58.000000 iOpt-0.2.1/iOpt.egg-info/SOURCES.txt
--rw-r--r--   0 anton      (501) staff       (20)        1 2023-06-29 07:15:58.000000 iOpt-0.2.1/iOpt.egg-info/dependency_links.txt
--rw-r--r--   0 anton      (501) staff       (20)      153 2023-06-29 07:15:58.000000 iOpt-0.2.1/iOpt.egg-info/requires.txt
--rw-r--r--   0 anton      (501) staff       (20)       23 2023-06-29 07:15:58.000000 iOpt-0.2.1/iOpt.egg-info/top_level.txt
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.242588 iOpt-0.2.1/problems/
--rw-r--r--   0 anton      (501) staff       (20)     3299 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/GKLS.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.243858 iOpt-0.2.1/problems/GKLS_function/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/GKLS_function/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)    34141 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/GKLS_function/gkls_function.py
--rw-r--r--   0 anton      (501) staff       (20)     5230 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/GKLS_function/gkls_random.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.244702 iOpt-0.2.1/problems/Hill/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Hill/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)   418174 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Hill/hill_generation.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.245906 iOpt-0.2.1/problems/Shekel/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Shekel/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)   355176 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Shekel/shekel_generation.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.248030 iOpt-0.2.1/problems/Shekel4/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Shekel4/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)      407 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/Shekel4/shekel4_generation.py
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     2631 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/g2c.py
--rw-r--r--   0 anton      (501) staff       (20)     2564 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/g8c.py
--rw-r--r--   0 anton      (501) staff       (20)     3053 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/grishagin.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.248934 iOpt-0.2.1/problems/grishagin_function/
--rw-r--r--   0 anton      (501) staff       (20)        0 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/grishagin_function/__init__.py
--rw-r--r--   0 anton      (501) staff       (20)     3968 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/grishagin_function/grishagin_function.py
--rw-r--r--   0 anton      (501) staff       (20)     6176 2023-04-21 14:01:16.000000 iOpt-0.2.1/problems/grishagin_function/grishagin_generation.py
--rw-r--r--   0 anton      (501) staff       (20)     3168 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/hill.py
--rw-r--r--   0 anton      (501) staff       (20)     2677 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/rastrigin.py
--rw-r--r--   0 anton      (501) staff       (20)     5378 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/rastriginInt.py
--rw-r--r--   0 anton      (501) staff       (20)     3034 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/rastrigin_hidden_constraint.py
--rw-r--r--   0 anton      (501) staff       (20)     5684 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/rastrigin_int_hidden_constraint.py
--rw-r--r--   0 anton      (501) staff       (20)     2391 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/romeijn1c.py
--rw-r--r--   0 anton      (501) staff       (20)     2913 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/romeijn2c.py
--rw-r--r--   0 anton      (501) staff       (20)     2949 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/romeijn3c.py
--rw-r--r--   0 anton      (501) staff       (20)     2637 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/romeijn5c.py
--rw-r--r--   0 anton      (501) staff       (20)     3200 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/shekel.py
--rw-r--r--   0 anton      (501) staff       (20)     3173 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/shekel4.py
--rw-r--r--   0 anton      (501) staff       (20)     2938 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/stronginc2.py
--rw-r--r--   0 anton      (501) staff       (20)     3150 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/stronginc3.py
--rw-r--r--   0 anton      (501) staff       (20)     3407 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/stronginc5.py
--rw-r--r--   0 anton      (501) staff       (20)     2212 2023-06-29 05:54:18.000000 iOpt-0.2.1/problems/xsquared.py
--rw-r--r--   0 anton      (501) staff       (20)       38 2023-06-29 07:15:58.251011 iOpt-0.2.1/setup.cfg
--rw-r--r--   0 anton      (501) staff       (20)     1359 2023-06-29 07:15:09.000000 iOpt-0.2.1/setup.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-06-29 07:15:58.250050 iOpt-0.2.1/test/
--rw-r--r--   0 anton      (501) staff       (20)     3795 2023-06-29 05:54:18.000000 iOpt-0.2.1/test/test_evolvent.py
--rw-r--r--   0 anton      (501) staff       (20)     1865 2023-04-21 14:01:16.000000 iOpt-0.2.1/test/test_optim_task.py
--rw-r--r--   0 anton      (501) staff       (20)     6617 2023-06-29 05:54:18.000000 iOpt-0.2.1/test/test_solving_test_problems.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.703890 iOpt-0.2.22/
+-rw-r--r--   0 anton      (501) staff       (20)     1543 2023-08-07 05:25:30.000000 iOpt-0.2.22/LICENSE
+-rw-r--r--   0 anton      (501) staff       (20)     7423 2023-08-07 05:26:34.703579 iOpt-0.2.22/PKG-INFO
+-rw-r--r--   0 anton      (501) staff       (20)     6883 2023-08-07 05:25:30.000000 iOpt-0.2.22/README.md
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.629008 iOpt-0.2.22/examples/
+-rw-r--r--   0 anton      (501) staff       (20)     1391 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/GKLS_example.py
+-rw-r--r--   0 anton      (501) staff       (20)     1007 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/GKLS_timeout_example.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.629315 iOpt-0.2.22/examples/Genetic_algorithm/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.629636 iOpt-0.2.22/examples/Genetic_algorithm/TSP/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.630249 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_1D/
+-rw-r--r--   0 anton      (501) staff       (20)     1697 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_1D/Example_GA_TSP_Vary_Mutation.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.630954 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_1D/Problems/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_1D/Problems/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     3579 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_1D/Problems/ga_tsp_vary_mutation.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_1D/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.632146 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_2D/
+-rw-r--r--   0 anton      (501) staff       (20)     1853 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_2D/Example_GA_TSP_Vary_Mutation_Population_Size.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.632781 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_2D/Problems/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_2D/Problems/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     4613 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_2D/Problems/ga_tsp_2d.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Genetic_algorithm/TSP/_2D/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Genetic_algorithm/TSP/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Genetic_algorithm/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     1295 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Grishagin_example.py
+-rw-r--r--   0 anton      (501) staff       (20)     1217 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Hill_example.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.633241 iOpt-0.2.22/examples/Machine_learning/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.633803 iOpt-0.2.22/examples/Machine_learning/SVC/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.635382 iOpt-0.2.22/examples/Machine_learning/SVC/_1D/
+-rw-r--r--   0 anton      (501) staff       (20)     1525 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_kernel_coefficient.py
+-rw-r--r--   0 anton      (501) staff       (20)     1565 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_regularization.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.636517 iOpt-0.2.22/examples/Machine_learning/SVC/_1D/Problems/
+-rw-r--r--   0 anton      (501) staff       (20)     3058 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Kernel.py
+-rw-r--r--   0 anton      (501) staff       (20)     3134 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Regularization.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_1D/Problems/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_1D/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.644815 iOpt-0.2.22/examples/Machine_learning/SVC/_2D/
+-rw-r--r--   0 anton      (501) staff       (20)     1491 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_2D/Example_2D_SVC.py
+-rw-r--r--   0 anton      (501) staff       (20)     1573 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_2D/Example_2D_SVC_Industrial.py
+-rw-r--r--   0 anton      (501) staff       (20)     1243 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_2D/Example_SVC_Float_Discrete.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.646085 iOpt-0.2.22/examples/Machine_learning/SVC/_2D/Problems/
+-rw-r--r--   0 anton      (501) staff       (20)     3061 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_2D/Problems/SVC_2D_Float_Discrete.py
+-rw-r--r--   0 anton      (501) staff       (20)     3091 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_2D/Problems/SVC_2d.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_2D/Problems/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_2D/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.646733 iOpt-0.2.22/examples/Machine_learning/SVC/_3D/
+-rw-r--r--   0 anton      (501) staff       (20)     1385 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_3D/Example_SVC_Discrete_Param.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.647552 iOpt-0.2.22/examples/Machine_learning/SVC/_3D/Problem/
+-rw-r--r--   0 anton      (501) staff       (20)     3397 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_3D/Problem/SVC_3D.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_3D/Problem/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/_3D/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/SVC/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Machine_learning/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     1250 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/RastriginInt_example.py
+-rw-r--r--   0 anton      (501) staff       (20)     1474 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Rastrigin_example.py
+-rw-r--r--   0 anton      (501) staff       (20)      897 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Shekel4_example.py
+-rw-r--r--   0 anton      (501) staff       (20)     1255 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/Shekel_example.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.649095 iOpt-0.2.22/examples/console_output/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/console_output/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      608 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/console_output/example_custom_output.py
+-rw-r--r--   0 anton      (501) staff       (20)      596 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/console_output/example_full_output.py
+-rw-r--r--   0 anton      (501) staff       (20)      597 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/console_output/example_only_result_output.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.649433 iOpt-0.2.22/examples/dynamic_painters/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.650013 iOpt-0.2.22/examples/dynamic_painters/1D_examples/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/dynamic_painters/1D_examples/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      621 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/dynamic_painters/1D_examples/example_1D_with_objective_function.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.650682 iOpt-0.2.22/examples/dynamic_painters/2D_examples/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/dynamic_painters/2D_examples/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      780 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/dynamic_painters/2D_examples/example_2D_with_level_lines.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/dynamic_painters/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.651065 iOpt-0.2.22/examples/static_painters/
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.667376 iOpt-0.2.22/examples/static_painters/1D_examples/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/1D_examples/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      640 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/1D_examples/example_1D_with_approximation.py
+-rw-r--r--   0 anton      (501) staff       (20)      640 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/1D_examples/example_1D_with_interpolation.py
+-rw-r--r--   0 anton      (501) staff       (20)      640 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/1D_examples/example_1D_with_objective_function_pointsInBottom_mode.py
+-rw-r--r--   0 anton      (501) staff       (20)      638 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/1D_examples/example_1D_with_only_points.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.669528 iOpt-0.2.22/examples/static_painters/2D_examples/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/2D_examples/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      776 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/2D_examples/example_2D_with_1-dimension_section.py
+-rw-r--r--   0 anton      (501) staff       (20)      667 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/2D_examples/example_2D_with_approximation.py
+-rw-r--r--   0 anton      (501) staff       (20)      667 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/2D_examples/example_2D_with_interpolation.py
+-rw-r--r--   0 anton      (501) staff       (20)      639 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/2D_examples/example_2D_with_level_lines.py
+-rw-r--r--   0 anton      (501) staff       (20)      671 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/2D_examples/example_2D_with_level_lines_by_interpolation.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/examples/static_painters/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.671619 iOpt-0.2.22/iOpt/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.678903 iOpt-0.2.22/iOpt/evolvent/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/evolvent/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)    11704 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/evolvent/evolvent.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.684184 iOpt-0.2.22/iOpt/method/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     3424 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/calculator.py
+-rw-r--r--   0 anton      (501) staff       (20)      360 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/icriterion_evaluate_method.py
+-rw-r--r--   0 anton      (501) staff       (20)     7424 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/index_method.py
+-rw-r--r--   0 anton      (501) staff       (20)     2213 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/index_method_calculator.py
+-rw-r--r--   0 anton      (501) staff       (20)      586 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/listener.py
+-rw-r--r--   0 anton      (501) staff       (20)     6260 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/local_optimizer.py
+-rw-r--r--   0 anton      (501) staff       (20)    17778 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/method.py
+-rw-r--r--   0 anton      (501) staff       (20)    13488 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/mixed_integer_method.py
+-rw-r--r--   0 anton      (501) staff       (20)     1569 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/optim_task.py
+-rw-r--r--   0 anton      (501) staff       (20)     3643 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/parallel_process.py
+-rw-r--r--   0 anton      (501) staff       (20)     9378 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/process.py
+-rw-r--r--   0 anton      (501) staff       (20)    25178 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/search_data.py
+-rw-r--r--   0 anton      (501) staff       (20)      376 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/sol_value.py
+-rw-r--r--   0 anton      (501) staff       (20)     3705 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/method/solverFactory.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.684471 iOpt-0.2.22/iOpt/output_system/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.685490 iOpt-0.2.22/iOpt/output_system/listeners/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/listeners/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     4807 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/listeners/animate_painters.py
+-rw-r--r--   0 anton      (501) staff       (20)     2374 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/listeners/console_outputers.py
+-rw-r--r--   0 anton      (501) staff       (20)    10285 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/listeners/static_painters.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.688870 iOpt-0.2.22/iOpt/output_system/outputers/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/outputers/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     9591 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/outputers/console_outputer.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.690126 iOpt-0.2.22/iOpt/output_system/painters/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/painters/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     5338 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/painters/animate_painters.py
+-rw-r--r--   0 anton      (501) staff       (20)      395 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/painters/painter.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.690877 iOpt-0.2.22/iOpt/output_system/painters/plotters/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/painters/plotters/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)    19664 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/painters/plotters/plotters.py
+-rw-r--r--   0 anton      (501) staff       (20)    12399 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/output_system/painters/static_painters.py
+-rw-r--r--   0 anton      (501) staff       (20)     1690 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/problem.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.691511 iOpt-0.2.22/iOpt/routine/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/routine/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      843 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/routine/timeout.py
+-rw-r--r--   0 anton      (501) staff       (20)     1459 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/solution.py
+-rw-r--r--   0 anton      (501) staff       (20)     9607 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/solver.py
+-rw-r--r--   0 anton      (501) staff       (20)     3565 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/solver_parametrs.py
+-rw-r--r--   0 anton      (501) staff       (20)      917 2023-08-07 05:25:30.000000 iOpt-0.2.22/iOpt/trial.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.678358 iOpt-0.2.22/iOpt.egg-info/
+-rw-r--r--   0 anton      (501) staff       (20)     7423 2023-08-07 05:26:34.000000 iOpt-0.2.22/iOpt.egg-info/PKG-INFO
+-rw-r--r--   0 anton      (501) staff       (20)     5537 2023-08-07 05:26:34.000000 iOpt-0.2.22/iOpt.egg-info/SOURCES.txt
+-rw-r--r--   0 anton      (501) staff       (20)        1 2023-08-07 05:26:34.000000 iOpt-0.2.22/iOpt.egg-info/dependency_links.txt
+-rw-r--r--   0 anton      (501) staff       (20)      160 2023-08-07 05:26:34.000000 iOpt-0.2.22/iOpt.egg-info/requires.txt
+-rw-r--r--   0 anton      (501) staff       (20)       23 2023-08-07 05:26:34.000000 iOpt-0.2.22/iOpt.egg-info/top_level.txt
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.697675 iOpt-0.2.22/problems/
+-rw-r--r--   0 anton      (501) staff       (20)     3325 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/GKLS.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.698722 iOpt-0.2.22/problems/GKLS_function/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/GKLS_function/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)    34141 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/GKLS_function/gkls_function.py
+-rw-r--r--   0 anton      (501) staff       (20)     5230 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/GKLS_function/gkls_random.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.699336 iOpt-0.2.22/problems/Hill/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/Hill/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)   418174 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/Hill/hill_generation.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.700474 iOpt-0.2.22/problems/Shekel/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/Shekel/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)   355176 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/Shekel/shekel_generation.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.701459 iOpt-0.2.22/problems/Shekel4/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/Shekel4/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)      407 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/Shekel4/shekel4_generation.py
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     2670 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/g2c.py
+-rw-r--r--   0 anton      (501) staff       (20)     2604 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/g8c.py
+-rw-r--r--   0 anton      (501) staff       (20)     3090 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/grishagin.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.702284 iOpt-0.2.22/problems/grishagin_function/
+-rw-r--r--   0 anton      (501) staff       (20)        0 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/grishagin_function/__init__.py
+-rw-r--r--   0 anton      (501) staff       (20)     3968 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/grishagin_function/grishagin_function.py
+-rw-r--r--   0 anton      (501) staff       (20)     6176 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/grishagin_function/grishagin_generation.py
+-rw-r--r--   0 anton      (501) staff       (20)     3206 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/hill.py
+-rw-r--r--   0 anton      (501) staff       (20)     2717 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/rastrigin.py
+-rw-r--r--   0 anton      (501) staff       (20)     5489 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/rastriginInt.py
+-rw-r--r--   0 anton      (501) staff       (20)     3076 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/rastrigin_hidden_constraint.py
+-rw-r--r--   0 anton      (501) staff       (20)     5808 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/rastrigin_int_hidden_constraint.py
+-rw-r--r--   0 anton      (501) staff       (20)     2429 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/romeijn1c.py
+-rw-r--r--   0 anton      (501) staff       (20)     2953 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/romeijn2c.py
+-rw-r--r--   0 anton      (501) staff       (20)     2990 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/romeijn3c.py
+-rw-r--r--   0 anton      (501) staff       (20)     2677 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/romeijn5c.py
+-rw-r--r--   0 anton      (501) staff       (20)     3239 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/shekel.py
+-rw-r--r--   0 anton      (501) staff       (20)     3212 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/shekel4.py
+-rw-r--r--   0 anton      (501) staff       (20)     2978 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/stronginc2.py
+-rw-r--r--   0 anton      (501) staff       (20)     3192 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/stronginc3.py
+-rw-r--r--   0 anton      (501) staff       (20)     3450 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/stronginc5.py
+-rw-r--r--   0 anton      (501) staff       (20)     2253 2023-08-07 05:25:30.000000 iOpt-0.2.22/problems/xsquared.py
+-rw-r--r--   0 anton      (501) staff       (20)       38 2023-08-07 05:26:34.703979 iOpt-0.2.22/setup.cfg
+-rw-r--r--   0 anton      (501) staff       (20)     1360 2023-08-07 05:25:59.000000 iOpt-0.2.22/setup.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-08-07 05:26:34.703186 iOpt-0.2.22/test/
+-rw-r--r--   0 anton      (501) staff       (20)     3809 2023-08-07 05:25:30.000000 iOpt-0.2.22/test/test_evolvent.py
+-rw-r--r--   0 anton      (501) staff       (20)     1875 2023-08-07 05:25:30.000000 iOpt-0.2.22/test/test_optim_task.py
+-rw-r--r--   0 anton      (501) staff       (20)     6568 2023-08-07 05:25:30.000000 iOpt-0.2.22/test/test_solving_test_problems.py
```

### Comparing `iOpt-0.2.1/LICENSE` & `iOpt-0.2.22/LICENSE`

 * *Files identical despite different names*

### Comparing `iOpt-0.2.1/PKG-INFO` & `iOpt-0.2.22/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iOpt
-Version: 0.2.1
+Version: 0.2.22
 Summary: Фреймворк для автоматического выбора значений параметров для математических моделей, ИИ и МО.
 Home-page: https://github.com/aimclub/iOpt
 Author: UNN Team
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -102,35 +102,34 @@
 
 from subprocess import Popen, PIPE, STDOUT
 
 if __name__ == "__main__":
     """
     Minimization of the Rastrigin test function with visualization
     """
-    #Create a test task
+    # Create a test task
     problem = Rastrigin(2)
-    #Setup a solver options
-    params = SolverParameters(r=2.5, eps=0.01, itersLimit=300, refineSolution=True)
-    #Create the solver
+    # Setup a solver options
+    params = SolverParameters(r=2.5, eps=0.01, iters_limit=300, refine_solution=True)
+    # Create the solver
     solver = Solver(problem, parameters=params)
-    #Print results to console while solving
+    # Print results to console while solving
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
-    #3D visualization at the end of the solution
-    spl = StaticPainterNDListener("rastrigin.png", "output", varsIndxs=[0,1], mode="surface", calc="interpolation")
-    solver.AddListener(spl)
-    #Run problem solution
-    sol = solver.Solve()
+    solver.add_listener(cfol)
+    # 3D visualization at the end of the solution
+    spl = StaticPainterNDListener("rastrigin.png", "output", vars_indxs=[0, 1], mode="surface", calc="interpolation")
+    solver.add_listener(spl)
+    # Run problem solution
+    sol = solver.solve()
 ```
 
 # **Examples**
 
 Let’s demonstrate the use of the iOpt framework when tuning the hyperparameters of one of the machine learning methods. In the support vector machine ([SVC](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)), we find the optimal hyperparameters (the regularization parameter **C**, the kernel coefficient **gamma**) in the problem of breast cancer classification ([detailed description of the data](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))).
 
-
 ```python
 import numpy as np
 from sklearn.utils import shuffle
 from sklearn.datasets import load_breast_cancer
 
 from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
@@ -150,27 +149,27 @@
 if __name__ == "__main__":
     x, y = load_breast_cancer_data()
     regularization_value_bound = {'low': 1, 'up': 6}
     kernel_coefficient_bound = {'low': -7, 'up': -3}
 
     problem = SVC_2d.SVC_2D(x, y, regularization_value_bound, kernel_coefficient_bound)
 
-    method_params = SolverParameters(r=np.double(3.0), itersLimit=100)
+    method_params = SolverParameters(r=np.double(3.0), iters_limit=100)
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimatePainterNDListener("svc2d_anim.png", "output", varsIndxs=[0, 1], toPaintObjFunc=False)
-    solver.AddListener(apl)
+    apl = AnimatePainterNDListener("svc2d_anim.png", "output", vars_indxs=[0, 1], to_paint_obj_func=False)
+    solver.add_listener(apl)
+
+    spl = StaticPainterNDListener("svc2d_stat.png", "output", vars_indxs=[0, 1], mode="surface", calc="interpolation")
+    solver.add_listener(spl)
 
-    spl = StaticPainterNDListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
-    solver.AddListener(spl)
-    
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
-    solver_info = solver.Solve()
+    solver_info = solver.solve()
 
 ```
 
 # **Project Structure**
 
 The latest stable release of iOpt is in the [main](https://github.com/UNN-ITMM-Software/iOpt/tree/main) branch. The repository includes the following directories:
 - The [iOpt](https://github.com/UNN-ITMM-Software/iOpt/tree/main/iOpt) directory contains the framework core in the form of Python classes.
```

### Comparing `iOpt-0.2.1/README.md` & `iOpt-0.2.22/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -88,35 +88,34 @@
 
 from subprocess import Popen, PIPE, STDOUT
 
 if __name__ == "__main__":
     """
     Minimization of the Rastrigin test function with visualization
     """
-    #Create a test task
+    # Create a test task
     problem = Rastrigin(2)
-    #Setup a solver options
-    params = SolverParameters(r=2.5, eps=0.01, itersLimit=300, refineSolution=True)
-    #Create the solver
+    # Setup a solver options
+    params = SolverParameters(r=2.5, eps=0.01, iters_limit=300, refine_solution=True)
+    # Create the solver
     solver = Solver(problem, parameters=params)
-    #Print results to console while solving
+    # Print results to console while solving
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
-    #3D visualization at the end of the solution
-    spl = StaticPainterNDListener("rastrigin.png", "output", varsIndxs=[0,1], mode="surface", calc="interpolation")
-    solver.AddListener(spl)
-    #Run problem solution
-    sol = solver.Solve()
+    solver.add_listener(cfol)
+    # 3D visualization at the end of the solution
+    spl = StaticPainterNDListener("rastrigin.png", "output", vars_indxs=[0, 1], mode="surface", calc="interpolation")
+    solver.add_listener(spl)
+    # Run problem solution
+    sol = solver.solve()
 ```
 
 # **Examples**
 
 Let’s demonstrate the use of the iOpt framework when tuning the hyperparameters of one of the machine learning methods. In the support vector machine ([SVC](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)), we find the optimal hyperparameters (the regularization parameter **C**, the kernel coefficient **gamma**) in the problem of breast cancer classification ([detailed description of the data](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))).
 
-
 ```python
 import numpy as np
 from sklearn.utils import shuffle
 from sklearn.datasets import load_breast_cancer
 
 from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
@@ -136,27 +135,27 @@
 if __name__ == "__main__":
     x, y = load_breast_cancer_data()
     regularization_value_bound = {'low': 1, 'up': 6}
     kernel_coefficient_bound = {'low': -7, 'up': -3}
 
     problem = SVC_2d.SVC_2D(x, y, regularization_value_bound, kernel_coefficient_bound)
 
-    method_params = SolverParameters(r=np.double(3.0), itersLimit=100)
+    method_params = SolverParameters(r=np.double(3.0), iters_limit=100)
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimatePainterNDListener("svc2d_anim.png", "output", varsIndxs=[0, 1], toPaintObjFunc=False)
-    solver.AddListener(apl)
+    apl = AnimatePainterNDListener("svc2d_anim.png", "output", vars_indxs=[0, 1], to_paint_obj_func=False)
+    solver.add_listener(apl)
+
+    spl = StaticPainterNDListener("svc2d_stat.png", "output", vars_indxs=[0, 1], mode="surface", calc="interpolation")
+    solver.add_listener(spl)
 
-    spl = StaticPainterNDListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
-    solver.AddListener(spl)
-    
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
-    solver_info = solver.Solve()
+    solver_info = solver.solve()
 
 ```
 
 # **Project Structure**
 
 The latest stable release of iOpt is in the [main](https://github.com/UNN-ITMM-Software/iOpt/tree/main) branch. The repository includes the following directories:
 - The [iOpt](https://github.com/UNN-ITMM-Software/iOpt/tree/main/iOpt) directory contains the framework core in the form of Python classes.
```

### Comparing `iOpt-0.2.1/examples/GKLS_example.py` & `iOpt-0.2.22/examples/Grishagin_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-from problems.GKLS import GKLS
+from problems.grishagin import Grishagin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
 
 from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
-
-def SolveSingleGKLS():
+if __name__ == "__main__":
     """
-    Минимизация тестовой функции из GKLS генератора с номером 39
+    Минимизация тестовой функции Гришагина с визуализацией
     """
 
     # создание объекта задачи
-    problem = GKLS(dimension=2, functionNumber=39)
+    problem = Grishagin(function_number=1)
 
     # Формируем параметры решателя
-    params = SolverParameters(r=3.5, eps=0.01, itersLimit=300, refineSolution=True, numberOfParallelPoints=4)
+    params = SolverParameters(r=2.5, eps=0.01, iters_limit=300, refine_solution=True)
 
     # Создаем решатель
     solver = Solver(problem=problem, parameters=params)
 
-    # Добавляем вывод резултатов в консоль
+    # Добавляем вывод результатов в консоль
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
     # Добавляем построение 3D визуализации после решения задачи
-    spl = StaticPainterNDListener(fileName="GKLS.png", pathForSaves="output", varsIndxs=[0, 1], mode="lines layers",
+    spl = StaticPainterNDListener("grishagin.png", "output", vars_indxs=[0, 1], mode="lines layers",
                                   calc="objective function")
-    solver.AddListener(spl)
+    solver.add_listener(spl)
 
     # Решение задачи
-    sol = solver.Solve()
-
-
-if __name__ == "__main__":
-    SolveSingleGKLS()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/GKLS_timeout_example.py` & `iOpt-0.2.22/examples/GKLS_timeout_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,23 @@
     Минимизация тестовой функции из GKLS генератора с номером 39
     """
 
     # создание объекта задачи
     problem = GKLS(dimension=6, functionNumber=39)
 
     # Формируем параметры решателя
-    params = SolverParameters(r=7, eps=0.01, itersLimit=3000000,
-                              numberOfParallelPoints=4, timeout=1)
+    params = SolverParameters(r=7, eps=0.01, iters_limit=3000000,
+                              number_of_parallel_points=4, timeout=1)
 
     # Создаем решатель
     solver = Solver(problem=problem, parameters=params)
 
     # Добавляем вывод резултатов в консоль
     cfol = ConsoleOutputListener(mode='result')
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
     # Решение задачи
-    sol = solver.Solve()
+    sol = solver.solve()
 
 
 if __name__ == "__main__":
     SolveSingleGKLS()
```

### Comparing `iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Example_GA_TSP_Vary_Mutation.py` & `iOpt-0.2.22/examples/Genetic_algorithm/TSP/_2D/Example_GA_TSP_Vary_Mutation_Population_Size.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-from iOpt.output_system.listeners.static_painters import StaticPainterListener
-from iOpt.output_system.listeners.animate_painters import AnimatePainterListener
-from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
+from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
 
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from examples.Genetic_algorithm.TSP._1D.Problems import ga_tsp_vary_mutation
+from examples.Genetic_algorithm.TSP._2D.Problems import ga_tsp_2d
 import numpy as np
 import xml.etree.ElementTree as ET
 
-def load_TSPs_matrix(filename):
-    root = ET.parse(filename).getroot()
+
+def load_TSPs_matrix(file_name):
+    root = ET.parse(file_name).getroot()
     columns = root.findall('graph/vertex')
     num_cols = len(columns)
     trans_matrix = np.zeros((num_cols, num_cols))
     for i, v in enumerate(columns):
         for e in v:
             j = int(e.text)
             trans_matrix[i, j] = float(e.get('cost'))
     return trans_matrix
 
 
 if __name__ == "__main__":
     tsp_matrix = load_TSPs_matrix('../TSPs_matrices/a280.xml')
     num_iteration = 200
-    population_size = 100
     mutation_probability_bound = {'low': 0.0, 'up': 1.0}
-    problem = ga_tsp_vary_mutation.GA_TSP_Vary_Mutation(tsp_matrix, num_iteration,
-                                                        population_size, mutation_probability_bound)
+    population_size_bound = {'low': 10.0, 'up': 100.0}
+    problem = ga_tsp_2d.GA_TSP_2D(tsp_matrix, num_iteration,
+                                  mutation_probability_bound, population_size_bound)
 
-    method_params = SolverParameters(r=np.double(3.0), itersLimit=40)
+    method_params = SolverParameters(r=np.double(2.0), iters_limit=300)
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimatePainterListener("gatsp_1d_anim_vary_mutation.png", "output", toPaintObjFunc=False)
-    solver.AddListener(apl)
-
-    spl = StaticPainterListener("gatsp_1d_stat_vary_mutation.png", "output", mode="interpolation")
-    solver.AddListener(spl)
-
-    cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
+    apl = AnimatePainterNDListener("gatsp_2d_anim_vary_mutation.png", "output", vars_indxs=[0, 1],
+                                   to_paint_obj_func=True)
+    solver.add_listener(apl)
+
+    spl = StaticPainterNDListener("gatsp_2d_stat_vary_mutation.png", "output", vars_indxs=[0, 1], mode="interpolation")
+    solver.add_listener(spl)
+
+    solver_info = solver.solve()
+    print(solver_info.number_of_global_trials)
+    print(solver_info.number_of_local_trials)
+    print(solver_info.solving_time)
 
-    solver_info = solver.Solve()
+    print(solver_info.best_trials[0].point.float_variables)
+    print(solver_info.best_trials[0].function_values[0].value)
```

### Comparing `iOpt-0.2.1/examples/Genetic_algorithm/TSP/_1D/Problems/ga_tsp_vary_mutation.py` & `iOpt-0.2.22/examples/Genetic_algorithm/TSP/_1D/Problems/ga_tsp_vary_mutation.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,47 +21,47 @@
         :param cost_matrix: Матрица расстояний
         :param num_iteration: Максимальное число итераций генетического алгоритма
         :param population_size: Размер популяции
         :param mutation_probability_bound: Границы изменения вероятности мутации (low - нижняя граница, up - верхняя)
         """
         super(GA_TSP_Vary_Mutation, self).__init__()
         self.dimension = 1
-        self.numberOfFloatVariables = 1
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        self.number_of_float_variables = 1
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
         self.costMatrix = cost_matrix
         if num_iteration <= 0:
             raise ValueError('The number of iterations cannot be zero or negative.')
         if population_size <= 0:
             raise ValueError('Population size cannot be negative or zero')
         self.populationSize = population_size
         self.numberOfIterations = num_iteration
-        self.floatVariableNames = np.array(["Mutation probability"], dtype=str)
-        self.lowerBoundOfFloatVariables = np.array([mutation_probability_bound['low']], dtype=np.double)
-        self.upperBoundOfFloatVariables = np.array([mutation_probability_bound['up']], dtype=np.double)
+        self.float_variable_names = np.array(["Mutation probability"], dtype=str)
+        self.lower_bound_of_float_variables = np.array([mutation_probability_bound['low']], dtype=np.double)
+        self.upper_bound_of_float_variables = np.array([mutation_probability_bound['up']], dtype=np.double)
         self.n_dim = cost_matrix.shape[0]
 
     def calc_total_distance(self, routine):
         """
         Метод расчёта расстояния
 
         :param routine: массив вершин для подсчёта расстояния
         """
         num_points, = routine.shape
         return sum([self.costMatrix[routine[i % num_points], routine[(i + 1) % num_points]] for i in range(num_points)])
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Метод расчёта значения целевой функции в точке
 
         :param point: Точка испытания
-        :param functionValue: объект хранения значения целевой функции в точке
+        :param function_value: объект хранения значения целевой функции в точке
         """
-        mutation_prob = point.floatVariables[0]
+        mutation_prob = point.float_variables[0]
         ga_tsp = GA_TSP(func=self.calc_total_distance,
                         n_dim=self.n_dim, size_pop=self.populationSize,
                         max_iter=self.numberOfIterations, prob_mut=mutation_prob)
         best_points, best_distance = ga_tsp.run()
-        functionValue.value = best_distance[0]
+        function_value.value = best_distance[0]
         #        print(best_distance[0])
-        return functionValue
+        return function_value
```

### Comparing `iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Example_GA_TSP_Vary_Mutation_Population_Size.py` & `iOpt-0.2.22/examples/Genetic_algorithm/TSP/_1D/Example_GA_TSP_Vary_Mutation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
-from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
+from iOpt.output_system.listeners.static_painters import StaticPainterListener
+from iOpt.output_system.listeners.animate_painters import AnimatePainterListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from examples.Genetic_algorithm.TSP._2D.Problems import ga_tsp_2d
+from examples.Genetic_algorithm.TSP._1D.Problems import ga_tsp_vary_mutation
 import numpy as np
 import xml.etree.ElementTree as ET
 
 
-def load_TSPs_matrix(filename):
-    root = ET.parse(filename).getroot()
+def load_TSPs_matrix(file_name):
+    root = ET.parse(file_name).getroot()
     columns = root.findall('graph/vertex')
     num_cols = len(columns)
     trans_matrix = np.zeros((num_cols, num_cols))
     for i, v in enumerate(columns):
         for e in v:
             j = int(e.text)
             trans_matrix[i, j] = float(e.get('cost'))
     return trans_matrix
 
 
 if __name__ == "__main__":
     tsp_matrix = load_TSPs_matrix('../TSPs_matrices/a280.xml')
     num_iteration = 200
+    population_size = 100
     mutation_probability_bound = {'low': 0.0, 'up': 1.0}
-    population_size_bound = {'low': 10.0, 'up': 100.0}
-    problem = ga_tsp_2d.GA_TSP_2D(tsp_matrix, num_iteration,
-                                  mutation_probability_bound, population_size_bound)
+    problem = ga_tsp_vary_mutation.GA_TSP_Vary_Mutation(tsp_matrix, num_iteration,
+                                                        population_size, mutation_probability_bound)
 
-    method_params = SolverParameters(r=np.double(2.0), itersLimit=300)
+    method_params = SolverParameters(r=np.double(3.0), iters_limit=40)
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimatePainterNDListener("gatsp_2d_anim_vary_mutation.png", "output",  varsIndxs=[0, 1], toPaintObjFunc=True)
-    solver.AddListener(apl)
+    apl = AnimatePainterListener("gatsp_1d_anim_vary_mutation.png", "output", to_paint_obj_func=False)
+    solver.add_listener(apl)
 
-    spl = StaticPainterNDListener("gatsp_2d_stat_vary_mutation.png", "output", varsIndxs=[0, 1], mode="interpolation")
-    solver.AddListener(spl)
+    spl = StaticPainterListener("gatsp_1d_stat_vary_mutation.png", "output", mode="interpolation")
+    solver.add_listener(spl)
 
-    solver_info = solver.Solve()
-    print(solver_info.numberOfGlobalTrials)
-    print(solver_info.numberOfLocalTrials)
-    print(solver_info.solvingTime)
+    cfol = ConsoleOutputListener(mode='full')
+    solver.add_listener(cfol)
 
-    print(solver_info.bestTrials[0].point.floatVariables)
-    print(solver_info.bestTrials[0].functionValues[0].value)
+    solver_info = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/Genetic_algorithm/TSP/_2D/Problems/ga_tsp_2d.py` & `iOpt-0.2.22/examples/Genetic_algorithm/TSP/_2D/Problems/ga_tsp_2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,18 @@
         :param cost_matrix: Матрица расстояний
         :param num_iteration: Максимальное число итераций генетического алгоритма
         :param population_size_bound: Границы изменения размера популяции (low - нижняя граница, up - верхняя)
         :param mutation_probability_bound: Границы изменения вероятности мутации (low - нижняя граница, up - верхняя)
         """
         super(GA_TSP_2D, self).__init__()
         self.dimension = 2
-        self.numberOfFloatVariables = 2
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        self.number_of_float_variables = 2
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
         self.costMatrix = cost_matrix
         # Проверка корректности числа итераций метода
         if num_iteration <= 0:
             raise ValueError('The number of iterations cannot be zero or negative.')
         # Проверка валидности интервала вероятностей мутации
         if mutation_probability_bound['low'] > mutation_probability_bound['up'] or \
                 mutation_probability_bound['low'] < 0.0 or \
@@ -43,40 +43,40 @@
                 mutation_probability_bound['up'] > 1.0:
             raise ValueError('Invalid mutation probability interval')
         # Проверка валидности размера популяции
         if population_size_bound['low'] < 2 or population_size_bound['low'] > population_size_bound['up']:
             raise ValueError('Incorrect population sizes were established')
 
         self.numberOfIterations = num_iteration
-        self.floatVariableNames = np.array(["mutation probability", "population size"], dtype=str)
-        self.lowerBoundOfFloatVariables = np.array([mutation_probability_bound['low'], population_size_bound['low']])
-        self.upperBoundOfFloatVariables = np.array([mutation_probability_bound['up'], population_size_bound['up'] / 2])
+        self.float_variable_names = np.array(["mutation probability", "population size"], dtype=str)
+        self.lower_bound_of_float_variables = np.array([mutation_probability_bound['low'], population_size_bound['low']])
+        self.upper_bound_of_float_variables = np.array([mutation_probability_bound['up'], population_size_bound['up'] / 2])
         self.n_dim = cost_matrix.shape[0]
 
     def calc_total_distance(self, routine):
         """
         Метод расчёта расстояния
 
         :param routine: массив вершин для подсчёта расстояния
         """
         num_points, = routine.shape
         return sum([self.costMatrix[routine[i % num_points], routine[(i + 1) % num_points]] for i in range(num_points)])
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Метод расчёта значения целевой функции в точке
 
         :param point: Точка испытания
-        :param functionValue: объект хранения значения целевой функции в точке
+        :param function_value: объект хранения значения целевой функции в точке
         """
-        mutation_prob, num_population = point.floatVariables[0], int(point.floatVariables[1])
+        mutation_prob, num_population = point.float_variables[0], int(point.float_variables[1])
         # Контроль чётности осыбей популяции
         if num_population % 2 != 0:
             num_population -= 1
 
         ga_tsp = GA_TSP(func=self.calc_total_distance,
                         n_dim=self.n_dim, size_pop=num_population,
                         max_iter=int(self.numberOfIterations), prob_mut=mutation_prob)
         best_points, best_distance = ga_tsp.run()
-        functionValue.value = best_distance[0]
+        function_value.value = best_distance[0]
         print(best_distance[0])
-        return functionValue
+        return function_value
```

### Comparing `iOpt-0.2.1/examples/Grishagin_example.py` & `iOpt-0.2.22/examples/Shekel4_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,25 @@
-from problems.grishagin import Grishagin
+from problems.shekel4 import Shekel4
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-
-from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 if __name__ == "__main__":
     """
-    Минимизация тестовой функции Гришагина с визуализацией
+    Минимизация тестовой функции Шекеля (размерность = 4)
     """
 
     # создание объекта задачи
-    problem = Grishagin(function_number=1)
+    problem = Shekel4(function_number=1)
 
     # Формируем параметры решателя
-    params = SolverParameters(r=2.5, eps=0.01, itersLimit=300, refineSolution=True)
+    params = SolverParameters(r=2.5, eps=0.01, iters_limit=10000, refine_solution=True)
 
     # Создаем решатель
     solver = Solver(problem=problem, parameters=params)
 
     # Добавляем вывод результатов в консоль
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
-
-    # Добавляем построение 3D визуализации после решения задачи
-    spl = StaticPainterNDListener("grishagin.png", "output", varsIndxs=[0, 1], mode="lines layers",
-                                calc="objective function")
-    solver.AddListener(spl)
+    solver.add_listener(cfol)
 
     # Решение задачи
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/Hill_example.py` & `iOpt-0.2.22/examples/Hill_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     Минимизация тестовой функции Хилла c визуализацией
     """
 
     # создание объекта задачи
     problem = Hill(function_number=5)
 
     # Формируем параметры решателя
-    params = SolverParameters(r=3, eps=0.01, itersLimit=300, refineSolution=True)
+    params = SolverParameters(r=3, eps=0.01, iters_limit=300, refine_solution=True)
 
     # Создаем решатель
     solver = Solver(problem=problem, parameters=params)
 
     # Добавляем вывод результатов в консоль
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
     # Добавляем построение визуализации после решения задачи
-    spl = StaticPainterListener("hill.png", "output", indx=0, isPointsAtBottom=False, mode="objective function")
-    solver.AddListener(spl)
+    spl = StaticPainterListener("hill.png", "output", indx=0, is_points_at_bottom=False, mode="objective function")
+    solver.add_listener(spl)
 
     # Решение задачи
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_kernel_coefficient.py` & `iOpt-0.2.22/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_kernel_coefficient.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     kernel_coefficient = -5
     regularization_value_bound = {'low': 1, 'up': 6}
     problem = SVC_Fixed_Kernel.SVC_Fixed_Kernel(x, y, kernel_coefficient, regularization_value_bound)
 
     method_params = SolverParameters(r=np.double(3.0), eps=np.double(0.05))
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimatePainterListener("svc1d_anim.png", "output", toPaintObjFunc=True)
-    solver.AddListener(apl)
+    apl = AnimatePainterListener("svc1d_anim.png", "output", to_paint_obj_func=True)
+    solver.add_listener(apl)
 
     spl = StaticPainterListener("svc1d_stat.png", "output", mode="interpolation")
-    solver.AddListener(spl)
+    solver.add_listener(spl)
 
-    solver_info = solver.Solve()
-    print(solver_info.numberOfGlobalTrials)
-    print(solver_info.numberOfLocalTrials)
-    print(solver_info.solvingTime)
+    solver_info = solver.solve()
+    print(solver_info.number_of_global_trials)
+    print(solver_info.number_of_local_trials)
+    print(solver_info.solving_time)
 
-    print(solver_info.bestTrials[0].point.floatVariables)
-    print(solver_info.bestTrials[0].functionValues[0].value)
+    print(solver_info.best_trials[0].point.float_variables)
+    print(solver_info.best_trials[0].function_values[0].value)
```

### Comparing `iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_regularization.py` & `iOpt-0.2.22/examples/Machine_learning/SVC/_1D/Example_SVC_Fixed_regularization.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
 if __name__ == "__main__":
     x, y = load_breast_cancer_data()
     regularization_value = 6
     kernel_coefficient_bound = {'low': -7, 'up': -3}
     problem = SVC_Fixed_Regularization.SVC_Fixed_Regularization(x, y, regularization_value, kernel_coefficient_bound)
 
-    method_params = SolverParameters(r=np.double(3.0), itersLimit=10, eps=np.double(0.05))
+    method_params = SolverParameters(r=np.double(3.0), iters_limit=10, eps=np.double(0.05))
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimatePainterListener("svc1d_anim.png", "output", toPaintObjFunc=True)
-    solver.AddListener(apl)
+    apl = AnimatePainterListener("svc1d_anim.png", "output", to_paint_obj_func=True)
+    solver.add_listener(apl)
 
     spl = StaticPainterListener("svc1d_stat.png", "output", mode="interpolation")
-    solver.AddListener(spl)
+    solver.add_listener(spl)
 
-    solver_info = solver.Solve()
-    print(solver_info.numberOfGlobalTrials)
-    print(solver_info.numberOfLocalTrials)
-    print(solver_info.solvingTime)
+    solver_info = solver.solve()
+    print(solver_info.number_of_global_trials)
+    print(solver_info.number_of_local_trials)
+    print(solver_info.solving_time)
 
-    print(solver_info.bestTrials[0].point.floatVariables)
-    print(solver_info.bestTrials[0].functionValues[0].value)
+    print(solver_info.best_trials[0].point.float_variables)
+    print(solver_info.best_trials[0].function_values[0].value)
```

### Comparing `iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Kernel.py` & `iOpt-0.2.22/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Kernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,33 +24,33 @@
         :param x_dataset: входные данные обучающе выборки метода SVC
         :param y_dataset: выходные данные обучающе выборки метода SVC
         :param kernel_coefficient_value: Значение коэфицента ядра
         :param regularization_bound: Границы изменения параметра регуляризации (low - нижняя граница, up - верхняя)
         """
         super(SVC_Fixed_Kernel, self).__init__()
         self.dimension = 1
-        self.numberOfFloatVariables = 1
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        self.number_of_float_variables = 1
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
         if x_dataset.shape[0] != y_dataset.shape[0]:
             raise ValueError('The input and output sample sizes do not match.')
         self.x = x_dataset
         self.y = y_dataset
         self.kernelCoefficient = kernel_coefficient_value
-        self.floatVariableNames = np.array(["Regularization parameter"], dtype=str)
-        self.lowerBoundOfFloatVariables = np.array([regularization_bound['low']], dtype=np.double)
-        self.upperBoundOfFloatVariables = np.array([regularization_bound['up']], dtype=np.double)
+        self.float_variable_names = np.array(["Regularization parameter"], dtype=str)
+        self.lower_bound_of_float_variables = np.array([regularization_bound['low']], dtype=np.double)
+        self.upper_bound_of_float_variables = np.array([regularization_bound['up']], dtype=np.double)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Метод расчёта значения целевой функции в точке
 
         :param point: Точка испытания
-        :param functionValue: объект хранения значения целевой функции в точке
+        :param function_value: объект хранения значения целевой функции в точке
         """
-        cs = point.floatVariables[0]
+        cs = point.float_variables[0]
         clf = SVC(C=10 ** cs, gamma=10 ** self.kernelCoefficient)
         clf.fit(self.x, self.y)
-        functionValue.value = -cross_val_score(clf, self.x, self.y,
-                                               scoring=lambda model, x, y: f1_score(y, model.predict(x))).mean()
-        return functionValue
+        function_value.value = -cross_val_score(clf, self.x, self.y,
+                                                scoring=lambda model, x, y: f1_score(y, model.predict(x))).mean()
+        return function_value
```

### Comparing `iOpt-0.2.1/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Regularization.py` & `iOpt-0.2.22/examples/Machine_learning/SVC/_1D/Problems/SVC_Fixed_Regularization.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,34 +24,34 @@
         :param x_dataset: входные данные обучающе выборки метода SVC
         :param y_dataset: выходные данные обучающе выборки метода SVC
         :param regularization_value: Значение параметра регуляризации
         :param kernel_coefficient_bound: Границы изменения значений коэфицента ядра (low - нижняя граница, up - верхняя)
         """
         super(SVC_Fixed_Regularization, self).__init__()
         self.dimension = 1
-        self.numberOfFloatVariables = 1
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        self.number_of_float_variables = 1
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
         if x_dataset.shape[0] != y_dataset.shape[0]:
             raise ValueError('The input and output sample sizes do not match.')
         self.x = x_dataset
         self.y = y_dataset
         self.regularizationValue = regularization_value
-        self.floatVariableNames = np.array(["Kernel coefficient"], dtype=str)
-        self.lowerBoundOfFloatVariables = np.array([kernel_coefficient_bound['low']], dtype=np.double)
-        self.upperBoundOfFloatVariables = np.array([kernel_coefficient_bound['up']], dtype=np.double)
+        self.float_variable_names = np.array(["Kernel coefficient"], dtype=str)
+        self.lower_bound_of_float_variables = np.array([kernel_coefficient_bound['low']], dtype=np.double)
+        self.upper_bound_of_float_variables = np.array([kernel_coefficient_bound['up']], dtype=np.double)
         s = 0
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Метод расчёта значения целевой функции в точке
 
         :param point: Точка испытания
-        :param functionValue: объект хранения значения целевой функции в точке
+        :param function_value: объект хранения значения целевой функции в точке
         """
-        kernel_coefficient = point.floatVariables[0]
+        kernel_coefficient = point.float_variables[0]
         clf = SVC(C=10 ** self.regularizationValue, gamma=10 ** kernel_coefficient)
         clf.fit(self.x, self.y)
-        functionValue.value = -cross_val_score(clf, self.x, self.y,
-                                               scoring=lambda model, x, y: f1_score(y, model.predict(x))).mean()
-        return functionValue
+        function_value.value = -cross_val_score(clf, self.x, self.y,
+                                                scoring=lambda model, x, y: f1_score(y, model.predict(x))).mean()
+        return function_value
```

### Comparing `iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Example_2D_SVC.py` & `iOpt-0.2.22/examples/Machine_learning/SVC/_2D/Example_2D_SVC.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 if __name__ == "__main__":
     x, y = load_breast_cancer_data()
     regularization_value_bound = {'low': 1, 'up': 6}
     kernel_coefficient_bound = {'low': -7, 'up': -3}
 
     problem = SVC_2d.SVC_2D(x, y, regularization_value_bound, kernel_coefficient_bound)
 
-    method_params = SolverParameters(r=np.double(3.0), itersLimit=100)
+    method_params = SolverParameters(r=np.double(3.0), iters_limit=100)
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimatePainterNDListener("svc2d_anim.png", "output", varsIndxs=[0, 1], toPaintObjFunc=False)
-    solver.AddListener(apl)
+    apl = AnimatePainterNDListener("svc2d_anim.png", "output", vars_indxs=[0, 1], to_paint_obj_func=False)
+    solver.add_listener(apl)
 
-    spl = StaticPainterNDListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
-    solver.AddListener(spl)
+    spl = StaticPainterNDListener("svc2d_stat.png", "output", vars_indxs=[0, 1], mode="surface", calc="interpolation")
+    solver.add_listener(spl)
 
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
-    solver_info = solver.Solve()
+    solver_info = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Example_2D_SVC_Industrial.py` & `iOpt-0.2.22/examples/Machine_learning/SVC/_2D/Example_SVC_Float_Discrete.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
 from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
+from sklearn.datasets import load_breast_cancer
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from examples.Machine_learning.SVC._2D.Problems import SVC_2d
+from examples.Machine_learning.SVC._2D.Problems import SVC_2D_Float_Discrete
 from sklearn.utils import shuffle
 import numpy as np
-import pandas as pd
 
-def get_SCANIA_dataset():
-    xls = pd.read_excel(r"../Datasets/aps_failure_training_set1.xls", header=None)
-    data = xls.values[1:]
-    row, col = data.shape
-    _x = data[:, 1:col]
-    _y = data[:, 0]
-    y = np.array(_y, dtype=np.double)
-    x = np.array(_x, dtype=np.double)
-    return shuffle(x, y, random_state=42)
+
+def load_breast_cancer_data():
+    dataset = load_breast_cancer()
+    x_raw, y_raw = dataset['data'], dataset['target']
+    inputs, outputs = shuffle(x_raw, y_raw ^ 1, random_state=42)
+    return inputs, outputs
+
+
 if __name__ == "__main__":
-    X, Y = get_SCANIA_dataset()
-    x = X[:2000]
-    y = Y[:2000]
-    regularization_value_bound = {'low': 1, 'up': 10}
-    kernel_coefficient_bound = {'low': -8, 'up': -1}
-    problem = SVC_2d.SVC_2D(x, y, regularization_value_bound, kernel_coefficient_bound)
-    method_params = SolverParameters(r=np.double(2.0), itersLimit=200)
+    x, y = load_breast_cancer_data()
+    regularization_value_bound = {'low': 1, 'up': 6}
+    kernel_type = {'kernel': ['linear', 'rbf', 'sigmoid']}
+
+    problem = SVC_2D_Float_Discrete.SVC_2D_Float_Discrete(x, y, regularization_value_bound, kernel_type)
+
+    method_params = SolverParameters(r=np.double(3.0), iters_limit=100)
     solver = Solver(problem, parameters=method_params)
-    apl = AnimatePainterNDListener("svc2d_anim.png", "output", varsIndxs=[0, 1])
-    solver.AddListener(apl)
-    spl = StaticPainterNDListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
-    solver.AddListener(spl)
+
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
-    solver_info = solver.Solve()
+    solver.add_listener(cfol)
+
+    solver_info = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Example_SVC_Float_Discrete.py` & `iOpt-0.2.22/examples/Machine_learning/SVC/_2D/Example_2D_SVC_Industrial.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
 from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
-from sklearn.datasets import load_breast_cancer
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from examples.Machine_learning.SVC._2D.Problems import SVC_2D_Float_Discrete
+from examples.Machine_learning.SVC._2D.Problems import SVC_2d
 from sklearn.utils import shuffle
 import numpy as np
+import pandas as pd
 
 
-def load_breast_cancer_data():
-    dataset = load_breast_cancer()
-    x_raw, y_raw = dataset['data'], dataset['target']
-    inputs, outputs = shuffle(x_raw, y_raw ^ 1, random_state=42)
-    return inputs, outputs
+def get_SCANIA_dataset():
+    xls = pd.read_excel(r"../Datasets/aps_failure_training_set1.xls", header=None)
+    data = xls.values[1:]
+    row, col = data.shape
+    _x = data[:, 1:col]
+    _y = data[:, 0]
+    y = np.array(_y, dtype=np.double)
+    x = np.array(_x, dtype=np.double)
+    return shuffle(x, y, random_state=42)
 
 
 if __name__ == "__main__":
-    x, y = load_breast_cancer_data()
-    regularization_value_bound = {'low': 1, 'up': 6}
-    kernel_type = {'kernel': ['linear', 'rbf', 'sigmoid']}
-
-    problem = SVC_2D_Float_Discrete.SVC_2D_Float_Discrete(x, y, regularization_value_bound, kernel_type)
-
-    method_params = SolverParameters(r=np.double(3.0), itersLimit=100)
+    X, Y = get_SCANIA_dataset()
+    x = X[:2000]
+    y = Y[:2000]
+    regularization_value_bound = {'low': 1, 'up': 10}
+    kernel_coefficient_bound = {'low': -8, 'up': -1}
+    problem = SVC_2d.SVC_2D(x, y, regularization_value_bound, kernel_coefficient_bound)
+    method_params = SolverParameters(r=np.double(2.0), iters_limit=200)
     solver = Solver(problem, parameters=method_params)
-
+    apl = AnimatePainterNDListener("svc2d_anim.png", "output", vars_indxs=[0, 1])
+    solver.add_listener(apl)
+    spl = StaticPainterNDListener("svc2d_stat.png", "output", vars_indxs=[0, 1], mode="surface", calc="interpolation")
+    solver.add_listener(spl)
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
-
-    solver_info = solver.Solve()
+    solver.add_listener(cfol)
+    solver_info = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Problems/SVC_2D_Float_Discrete.py` & `iOpt-0.2.22/examples/Machine_learning/SVC/_3D/Problem/SVC_3D.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 import numpy as np
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.problem import Problem
 from sklearn.svm import SVC
 from sklearn.model_selection import cross_val_score
-from typing import Dict
-from sklearn.pipeline import Pipeline
-from sklearn.preprocessing import StandardScaler
+from typing import Dict, List
 
-class SVC_2D_Float_Discrete(Problem):
+class SVC_3D(Problem):
     """
-    Класс SVC_2D представляет возможность поиска оптимального набора гиперпараметров алгоритма
+    Класс SVC_3D представляет возможность поиска оптимального набора гиперпараметров алгоритма
       C-Support Vector Classification.
       Найденные параметры являются оптимальными при варьировании параматра регуляризации
-      (Regularization parameter С) и типа ядра (kernel)
+      (Regularization parameter С) значения коэфицента ядра (gamma) и типа ядра (kernel)
     """
 
     def __init__(self, x_dataset: np.ndarray, y_dataset: np.ndarray,
                  regularization_bound: Dict[str, float],
-                 kernel_type: Dict[str, list[str]]
+                 kernel_coefficient_bound: Dict[str, float],
+                 kernel_type: Dict[str, List[str]]
                  ):
         """
-        Конструктор класса SVC_2D_Float_Discrete
+        Конструктор класса SVC_3D
 
         :param x_dataset: входные данные обучающе выборки метода SVC
         :param y_dataset: выходные данные обучающе выборки метода SVC
+        :param kernel_coefficient_bound: Значение параметра регуляризации
         :param regularization_bound: Границы изменения значений коэфицента ядра (low - нижняя граница, up - верхняя)
         :param kernel_type: Тип ядра, используемый в алгоритме SVC
         """
-        super(SVC_2D_Float_Discrete, self).__init__()
-        self.dimension = 2
-        self.numberOfFloatVariables = 1
-        self.numberOfDiscreteVariables = 1
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        super(SVC_3D, self).__init__()
+        self.dimension = 3
+        self.number_of_float_variables = 2
+        self.number_of_discrete_variables = 1
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
         if x_dataset.shape[0] != y_dataset.shape[0]:
             raise ValueError('The input and output sample sizes do not match.')
         self.x = x_dataset
         self.y = y_dataset
-        self.floatVariableNames = np.array(["Regularization parameter"], dtype=str)
-        self.lowerBoundOfFloatVariables = np.array([regularization_bound['low']], dtype=np.double)
-        self.upperBoundOfFloatVariables = np.array([regularization_bound['up']], dtype=np.double)
+        self.float_variable_names = np.array(["Regularization parameter", "Kernel coefficient"], dtype=str)
+        self.lower_bound_of_float_variables = np.array([regularization_bound['low'], kernel_coefficient_bound['low']],
+                                                   dtype=np.double)
+        self.upper_bound_of_float_variables = np.array([regularization_bound['up'], kernel_coefficient_bound['up']],
+                                                   dtype=np.double)
+        self.discrete_variable_names.append('kernel')
+        self.discrete_variable_values.append(kernel_type['kernel'])
 
-        self.discreteVariableNames.append('kernel')
-        self.discreteVariableValues.append(kernel_type['kernel'])
 
-
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Метод расчёта значения целевой функции в точке
 
         :param point: Точка испытания
-        :param functionValue: объект хранения значения целевой функции в точке
+        :param function_value: объект хранения значения целевой функции в точке
         """
-        cs = point.floatVariables[0]
-        kernel_type = point.discreteVariables[0]
-        clf = SVC(C=10 ** cs, kernel=kernel_type)
-        functionValue.value = -cross_val_score(clf, self.x, self.y, scoring='f1').mean()
-        return functionValue
+        cs, gammas = point.float_variables[0], point.float_variables[1]
+        kernel_type = point.discrete_variables[0]
+        clf = SVC(C=10 ** cs, gamma=10 ** gammas, kernel=kernel_type)
+        function_value.value = -cross_val_score(clf, self.x, self.y, scoring='f1').mean()
+        return function_value
```

### Comparing `iOpt-0.2.1/examples/Machine_learning/SVC/_2D/Problems/SVC_2d.py` & `iOpt-0.2.22/examples/Machine_learning/SVC/_2D/Problems/SVC_2d.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,34 +25,34 @@
         :param x_dataset: входные данные обучающе выборки метода SVC
         :param y_dataset: выходные данные обучающе выборки метода SVC
         :param kernel_coefficient_bound: Значение параметра регуляризации
         :param regularization_bound: Границы изменения значений коэфицента ядра (low - нижняя граница, up - верхняя)
         """
         super(SVC_2D, self).__init__()
         self.dimension = 2
-        self.numberOfFloatVariables = 2
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        self.number_of_float_variables = 2
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
         if x_dataset.shape[0] != y_dataset.shape[0]:
             raise ValueError('The input and output sample sizes do not match.')
         self.x = x_dataset
         self.y = y_dataset
-        self.floatVariableNames = np.array(["Regularization parameter", "Kernel coefficient"], dtype=str)
-        self.lowerBoundOfFloatVariables = np.array([regularization_bound['low'], kernel_coefficient_bound['low']],
+        self.float_variable_names = np.array(["Regularization parameter", "Kernel coefficient"], dtype=str)
+        self.lower_bound_of_float_variables = np.array([regularization_bound['low'], kernel_coefficient_bound['low']],
                                                    dtype=np.double)
-        self.upperBoundOfFloatVariables = np.array([regularization_bound['up'], kernel_coefficient_bound['up']],
+        self.upper_bound_of_float_variables = np.array([regularization_bound['up'], kernel_coefficient_bound['up']],
                                                    dtype=np.double)
 
 
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Метод расчёта значения целевой функции в точке
 
         :param point: Точка испытания
-        :param functionValue: объект хранения значения целевой функции в точке
+        :param function_value: объект хранения значения целевой функции в точке
         """
-        cs, gammas = point.floatVariables[0], point.floatVariables[1]
+        cs, gammas = point.float_variables[0], point.float_variables[1]
         clf = SVC(C=10 ** cs, gamma=10 ** gammas)
-        functionValue.value = -cross_val_score(clf, self.x, self.y, scoring='f1').mean()
-        return functionValue
+        function_value.value = -cross_val_score(clf, self.x, self.y, scoring='f1').mean()
+        return function_value
```

### Comparing `iOpt-0.2.1/examples/Machine_learning/SVC/_3D/Example_SVC_Discrete_Param.py` & `iOpt-0.2.22/examples/Machine_learning/SVC/_3D/Example_SVC_Discrete_Param.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 from iOpt.output_system.listeners.static_painters import StaticDiscreteListener
 from sklearn.datasets import load_breast_cancer
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
 from examples.Machine_learning.SVC._3D.Problem import SVC_3D
 from sklearn.utils import shuffle
 
+
 def load_breast_cancer_data():
     dataset = load_breast_cancer()
     x_raw, y_raw = dataset['data'], dataset['target']
     inputs, outputs = shuffle(x_raw, y_raw ^ 1, random_state=42)
     return inputs, outputs
 
+
 if __name__ == "__main__":
     x, y = load_breast_cancer_data()
     regularization_value_bound = {'low': 1, 'up': 10}
     kernel_coefficient_bound = {'low': -9, 'up': -6.7}
     kernel_type = {'kernel': ['rbf', 'sigmoid', 'poly']}
     problem = SVC_3D.SVC_3D(x, y, regularization_value_bound, kernel_coefficient_bound, kernel_type)
-    method_params = SolverParameters(itersLimit=400)
+    method_params = SolverParameters(iters_limit=400)
     solver = Solver(problem, parameters=method_params)
     apl = StaticDiscreteListener("experiment1.png", mode='analysis')
-    solver.AddListener(apl)
+    solver.add_listener(apl)
     apl = StaticDiscreteListener("experiment2.png", mode='bestcombination', calc='interpolation', mrkrs=4)
-    solver.AddListener(apl)
+    solver.add_listener(apl)
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
-    solver_info = solver.Solve()
+    solver.add_listener(cfol)
+    solver_info = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/Machine_learning/SVC/_3D/Problem/SVC_3D.py` & `iOpt-0.2.22/problems/shekel4.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 import numpy as np
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
+from iOpt.trial import Trial
 from iOpt.problem import Problem
-from sklearn.svm import SVC
-from sklearn.model_selection import cross_val_score
-from typing import Dict, List
+import problems.Shekel4.shekel4_generation as shekelGen
 
-class SVC_3D(Problem):
+
+class Shekel4(Problem):
     """
-    Класс SVC_3D представляет возможность поиска оптимального набора гиперпараметров алгоритма
-      C-Support Vector Classification.
-      Найденные параметры являются оптимальными при варьировании параматра регуляризации
-      (Regularization parameter С) значения коэфицента ядра (gamma) и типа ядра (kernel)
+    Функция Шекеля - это многомерная, мультимодальная, непрерывная, детерминированная функция, задана формулой:
+       :math:`f(x) = \sum_{i=1}^{m}(c_{i}+\sum_{j=1}^{n}(x-a_{i})^{2})^{-1}`,
+       где :math:`m` – количество максимумов функции,
+       :math:`a, c` - параметры, генерируемые случайным образом.
+       В генераторе размерность задачи равна 4.
     """
 
-    def __init__(self, x_dataset: np.ndarray, y_dataset: np.ndarray,
-                 regularization_bound: Dict[str, float],
-                 kernel_coefficient_bound: Dict[str, float],
-                 kernel_type: Dict[str, List[str]]
-                 ):
+    def __init__(self, function_number: int):
         """
-        Конструктор класса SVC_3D
+        Конструктор класса Shekel problem.
 
-        :param x_dataset: входные данные обучающе выборки метода SVC
-        :param y_dataset: выходные данные обучающе выборки метода SVC
-        :param kernel_coefficient_bound: Значение параметра регуляризации
-        :param regularization_bound: Границы изменения значений коэфицента ядра (low - нижняя граница, up - верхняя)
-        :param kernel_type: Тип ядра, используемый в алгоритме SVC
+        :param functionNumber: номер задачи в наборе, :math:`1 <= functionNumber <= 3`
         """
-        super(SVC_3D, self).__init__()
-        self.dimension = 3
-        self.numberOfFloatVariables = 2
-        self.numberOfDiscreteVariables = 1
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
-        if x_dataset.shape[0] != y_dataset.shape[0]:
-            raise ValueError('The input and output sample sizes do not match.')
-        self.x = x_dataset
-        self.y = y_dataset
-        self.floatVariableNames = np.array(["Regularization parameter", "Kernel coefficient"], dtype=str)
-        self.lowerBoundOfFloatVariables = np.array([regularization_bound['low'], kernel_coefficient_bound['low']],
-                                                   dtype=np.double)
-        self.upperBoundOfFloatVariables = np.array([regularization_bound['up'], kernel_coefficient_bound['up']],
-                                                   dtype=np.double)
-        self.discreteVariableNames.append('kernel')
-        self.discreteVariableValues.append(kernel_type['kernel'])
-
+        super(Shekel4, self).__init__()
+        self.name = "Shekel4"
+        self.dimension = 4
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
+        self.fn = function_number
+
+        self.float_variable_names = np.ndarray(shape=(self.dimension,), dtype=str)
+        for i in range(self.dimension):
+            self.float_variable_names[i] = i
+
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension,), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(0)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension,), dtype=np.double)
+        self.upper_bound_of_float_variables.fill(10)
+
+        self.known_optimum = np.ndarray(shape=(1,), dtype=Trial)
+
+        pointfv = np.ndarray(shape=(self.dimension,), dtype=np.double)
+        pointfv.fill(4)
+        KOpoint = Point(pointfv, [])
+        KOfunV = np.ndarray(shape=(1,), dtype=FunctionValue)
+        KOfunV[0] = FunctionValue()
+        KOfunV[0] = self.calculate(KOpoint, KOfunV[0])
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
-        Метод расчёта значения целевой функции в точке
+        Вычисление значения выбранной функции в заданной точке.
 
-        :param point: Точка испытания
-        :param functionValue: объект хранения значения целевой функции в точке
+        :param point: координаты точки испытания, в которой будет вычислено значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
+        :return: Вычисленное значение функции в точке point
         """
-        cs, gammas = point.floatVariables[0], point.floatVariables[1]
-        kernel_type = point.discreteVariables[0]
-        clf = SVC(C=10 ** cs, gamma=10 ** gammas, kernel=kernel_type)
-        functionValue.value = -cross_val_score(clf, self.x, self.y, scoring='f1').mean()
-        return functionValue
+        res: np.double = 0
+        for i in range(shekelGen.maxI[self.fn - 1]):
+            den: np.double = 0
+            for j in range(self.dimension):
+                den = den + pow((point.float_variables[j] - shekelGen.a[i][j]), 2.0)
+            res = res - 1 / (den + shekelGen.c[i])
+
+        function_value.value = res
+        return function_value
```

### Comparing `iOpt-0.2.1/examples/RastriginInt_example.py` & `iOpt-0.2.22/examples/Rastrigin_example.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
+from iOpt.trial import Point
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.trial import Point
-from problems.rastriginInt import RastriginInt
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 
 if __name__ == "__main__":
     """
     Минимизация тестовой функции Растригина с визуализацией
     """
 
     # Создание тестовой задачи
-    problem = RastriginInt(dimension=5, numberOfDiscreteVariables=3)
+    problem = Rastrigin(dimension=2)
     # Начальная точка
-    startPoint: Point = Point(floatVariables=[0.5, 0.5], discreteVariables=['A', 'B', 'A'])
+    start_point: Point = Point(float_variables=[0.5, 0.5], discrete_variables=None)
     # Параметры решателя
-    params = SolverParameters(r=2.5, eps=0.01, itersLimit=10000, startPoint=startPoint, numberOfParallelPoints=16)
+    params = SolverParameters(r=2.5, eps=0.01, iters_limit=300, refine_solution=True, start_point=start_point)
     # Создание решателя
     solver = Solver(problem=problem, parameters=params)
     # Вывод результатов в консоль в процессе решения задачи
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
     # 3D визуализация по окончании решения задачи
-
+    spl = StaticPainterNDListener(file_name="rastrigin.png", path_for_saves="output", vars_indxs=[0, 1], mode="surface",
+                                  calc="interpolation")
+    solver.add_listener(spl)
     # Запуск решения задачи
-    sol = solver.Solve()
-
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/Rastrigin_example.py` & `iOpt-0.2.22/examples/RastriginInt_example.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-from iOpt.trial import Point
-from problems.rastrigin import Rastrigin
+from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
-from iOpt.output_system.listeners.console_outputers import ConsoleOutputListener
+from iOpt.trial import Point
+from problems.rastriginInt import RastriginInt
 
 if __name__ == "__main__":
     """
     Минимизация тестовой функции Растригина с визуализацией
     """
 
     # Создание тестовой задачи
-    problem = Rastrigin(dimension=2)
+    problem = RastriginInt(dimension=5, number_of_discrete_variables=3)
     # Начальная точка
-    startPoint: Point = Point(floatVariables=[0.5, 0.5], discreteVariables=None)
+    start_point: Point = Point(float_variables=[0.5, 0.5], discrete_variables=['A', 'B', 'A'])
     # Параметры решателя
-    params = SolverParameters(r=2.5, eps=0.01, itersLimit=300, refineSolution=True, startPoint=startPoint)
+    params = SolverParameters(r=2.5, eps=0.01, iters_limit=10000, start_point=start_point, number_of_parallel_points=16)
     # Создание решателя
     solver = Solver(problem=problem, parameters=params)
     # Вывод результатов в консоль в процессе решения задачи
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
     # 3D визуализация по окончании решения задачи
-    spl = StaticPainterNDListener(fileName="rastrigin.png", pathForSaves="output", varsIndxs=[0, 1], mode="surface",
-                                  calc="interpolation")
-    solver.AddListener(spl)
-    # Запуск решения задачи
-    sol = solver.Solve()
 
+    # Запуск решения задачи
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/Shekel_example.py` & `iOpt-0.2.22/examples/Shekel_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,23 @@
     Минимизация тестовой функции Шекеля
     """
 
     # создание объекта задачи
     problem = Shekel(function_number=0)
 
     # Формируем параметры решателя
-    params = SolverParameters(r=3, eps=0.01, itersLimit=300, refineSolution=True)
+    params = SolverParameters(r=3, eps=0.01, iters_limit=300, refine_solution=True)
 
     # Создаем решатель
     solver = Solver(problem=problem, parameters=params)
 
     # Добавляем вывод результатов в консоль
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
     # Добавляем построение визуализации после решения задачи
-    spl = StaticPainterListener(fileName="shekel.png", pathForSaves="output", indx=0, isPointsAtBottom=False,
+    spl = StaticPainterListener(file_name="shekel.png", path_for_saves="output", indx=0, is_points_at_bottom=False,
                                 mode="objective function")
-    solver.AddListener(spl)
+    solver.add_listener(spl)
 
     # Решение задачи
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/console_output/example_custom_output.py` & `iOpt-0.2.22/examples/console_output/example_custom_output.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     params = SolverParameters(r=3.5, eps=0.001)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
     cfol = ConsoleOutputListener(mode="custom", iters=400)
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/console_output/example_full_output.py` & `iOpt-0.2.22/examples/console_output/example_full_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     params = SolverParameters(r=3.5, eps=0.001)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
     cfol = ConsoleOutputListener(mode="full")
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/console_output/example_only_result_output.py` & `iOpt-0.2.22/examples/console_output/example_only_result_output.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     params = SolverParameters(r=3.5, eps=0.001)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
     cfol = ConsoleOutputListener(mode="result")
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/dynamic_painters/1D_examples/example_1D_with_objective_function.py` & `iOpt-0.2.22/examples/dynamic_painters/1D_examples/example_1D_with_objective_function.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
     apl = AnimatePainterListener("rastrigin_1_2.5_0.01.png")
-    solver.AddListener(apl)
+    solver.add_listener(apl)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/dynamic_painters/2D_examples/example_2D_with_level_lines.py` & `iOpt-0.2.22/examples/dynamic_painters/2D_examples/example_2D_with_level_lines.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     cfol = ConsoleOutputListener(mode="full")
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
     # add needed listeners for solver
     apl = AnimatePainterNDListener("xsquared_1_2.5_0.01.png")
-    solver.AddListener(apl)
+    solver.add_listener(apl)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_approximation.py` & `iOpt-0.2.22/examples/static_painters/2D_examples/example_2D_with_interpolation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.output_system.listeners.static_painters import StaticPainterListener
+from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 
 if __name__ == "__main__":
-    # create the problem 1D dimension
-    problem = Rastrigin(1)
+    # create the problem 2D dimension
+    problem = Rastrigin(2)
 
     # add solver parameters
-    params = SolverParameters(r=3, eps=0.01)
+    params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticPainterListener("rastrigin_1_3_0.01.png", mode="approximation")
-    solver.AddListener(apl)
+    apl = StaticPainterNDListener("rastrigin_2_2.5_0.01_interp.png", mode='surface', calc='interpolation')
+    solver.add_listener(apl)
 
     # solve the problem
-    sol = solver.Solve()
-    
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_interpolation.py` & `iOpt-0.2.22/examples/static_painters/1D_examples/example_1D_with_interpolation.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
     apl = StaticPainterListener("rastrigin_1_2.5_0.01.png", mode="interpolation")
-    solver.AddListener(apl)
+    solver.add_listener(apl)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_objective_function_pointsInBottom_mode.py` & `iOpt-0.2.22/examples/static_painters/1D_examples/example_1D_with_objective_function_pointsInBottom_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,12 +10,12 @@
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticPainterListener("xsquared_1_2.5_0.01.png", isPointsAtBottom=True)
-    solver.AddListener(apl)
+    apl = StaticPainterListener("xsquared_1_2.5_0.01.png", is_points_at_bottom=True)
+    solver.add_listener(apl)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/static_painters/1D_examples/example_1D_with_only_points.py` & `iOpt-0.2.22/examples/static_painters/1D_examples/example_1D_with_only_points.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
     apl = StaticPainterListener("rastrigin_1_2.5_0.01.png", mode="only points")
-    solver.AddListener(apl)
+    solver.add_listener(apl)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_1-dimension_section.py` & `iOpt-0.2.22/examples/static_painters/2D_examples/example_2D_with_1-dimension_section.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
     apl_0 = StaticPainterListener("rastrigin_2_3.5_0.001_static1D_0.png", "output", indx=0)
     apl_1 = StaticPainterListener("rastrigin_2_3.5_0.001_static1D_1.png", "output", indx=1)
-    solver.AddListener(apl_0)
-    solver.AddListener(apl_1)
+    solver.add_listener(apl_0)
+    solver.add_listener(apl_1)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_approximation.py` & `iOpt-0.2.22/examples/static_painters/1D_examples/example_1D_with_approximation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
-from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
+from iOpt.output_system.listeners.static_painters import StaticPainterListener
 
 if __name__ == "__main__":
-    # create the problem 2D dimension
-    problem = Rastrigin(2)
+    # create the problem 1D dimension
+    problem = Rastrigin(1)
 
     # add solver parameters
-    params = SolverParameters(r=2.5, eps=0.01)
+    params = SolverParameters(r=3, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticPainterNDListener("rastrigin_2_2.5_0.01_approx.png", mode='surface', calc='approximation')
-    solver.AddListener(apl)
+    apl = StaticPainterListener("rastrigin_1_3_0.01.png", mode="approximation")
+    solver.add_listener(apl)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
+
```

### Comparing `iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_interpolation.py` & `iOpt-0.2.22/examples/static_painters/2D_examples/example_2D_with_level_lines.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from problems.rastrigin import Rastrigin
+from problems.xsquared import XSquared
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
 from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 
 if __name__ == "__main__":
     # create the problem 2D dimension
-    problem = Rastrigin(2)
+    problem = XSquared(2)
 
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticPainterNDListener("rastrigin_2_2.5_0.01_interp.png", mode='surface', calc='interpolation')
-    solver.AddListener(apl)
+    apl = StaticPainterNDListener("xsquared_2_2.5_0.01.png", mode='lines layers')
+    solver.add_listener(apl)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_level_lines.py` & `iOpt-0.2.22/examples/static_painters/2D_examples/example_2D_with_level_lines_by_interpolation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from problems.xsquared import XSquared
+from problems.rastrigin import Rastrigin
 from iOpt.solver import Solver
 from iOpt.solver_parametrs import SolverParameters
 from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 
 if __name__ == "__main__":
     # create the problem 2D dimension
-    problem = XSquared(2)
+    problem = Rastrigin(2)
 
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticPainterNDListener("xsquared_2_2.5_0.01.png", mode='lines layers')
-    solver.AddListener(apl)
+    apl = StaticPainterNDListener("xsquared_2_2.5_0.01_interp.png", mode='lines layers', calc='interpolation')
+    solver.add_listener(apl)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/examples/static_painters/2D_examples/example_2D_with_level_lines_by_interpolation.py` & `iOpt-0.2.22/examples/static_painters/2D_examples/example_2D_with_approximation.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,12 +10,12 @@
     # add solver parameters
     params = SolverParameters(r=2.5, eps=0.01)
 
     # create solver
     solver = Solver(problem, parameters=params)
 
     # add needed listeners for solver
-    apl = StaticPainterNDListener("xsquared_2_2.5_0.01_interp.png", mode='lines layers', calc='interpolation')
-    solver.AddListener(apl)
+    apl = StaticPainterNDListener("rastrigin_2_2.5_0.01_approx.png", mode='surface', calc='approximation')
+    solver.add_listener(apl)
 
     # solve the problem
-    sol = solver.Solve()
+    sol = solver.solve()
```

### Comparing `iOpt-0.2.1/iOpt/method/calculator.py` & `iOpt-0.2.22/iOpt/method/calculator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,89 @@
 from __future__ import annotations
 
 import copy
-from multiprocessing import Pool
+from pathos.multiprocessing import _ProcessPool
 
 from iOpt.method.icriterion_evaluate_method import ICriterionEvaluateMethod
 from iOpt.method.search_data import SearchDataItem
 from iOpt.solver_parametrs import SolverParameters
 
 import sys
 
-#возможно стоит удалить
+# возможно стоит удалить
 sys.setrecursionlimit(10000)
 
 
 class Calculator:
-    pool: Pool = None
-    evaluateMethod: ICriterionEvaluateMethod = None
+    pool: _ProcessPool = None
+    evaluate_method: ICriterionEvaluateMethod = None
 
     def __init__(self,
-                 evaluateMethod: ICriterionEvaluateMethod,
+                 evaluate_method: ICriterionEvaluateMethod,
                  parameters: SolverParameters
                  ):
         r"""
         Конструктор класса Calculator
 
-        :param evaluateMethod: метод вычислений, проводящий поисковые испытания по заданным правилам.
+        :param evaluate_method: метод вычислений, проводящий поисковые испытания по заданным правилам.
         :param parameters: параметры решения задачи оптимизации.
         """
-        self.evaluateMethod = evaluateMethod
+        self.evaluate_method = evaluate_method
         self.parameters = parameters
-        Calculator.pool = Pool(parameters.numberOfParallelPoints,
-                               initializer=Calculator.worker_init,
-                               initargs=(self.evaluateMethod,))
+        Calculator.worker_init(self.evaluate_method)
+        Calculator.pool = _ProcessPool(parameters.number_of_parallel_points,
+                                       initializer=Calculator.worker_init,
+                                       initargs=(self.evaluate_method,))
 
     r"""
     Инициализация метода вычислений в каждом процессе из пула процессов Calculator.Pool
 
-    :param evaluateMethod: метод вычислений, проводящий поисковые испытания по заданным правилам.
+    :param evaluate_method: метод вычислений, проводящий поисковые испытания по заданным правилам.
     """
+
     @staticmethod
-    def worker_init(evaluateMethod: ICriterionEvaluateMethod):
-        Calculator.evaluateMethod = evaluateMethod
+    def worker_init(evaluate_method: ICriterionEvaluateMethod):
+        Calculator.evaluate_method = evaluate_method
 
     r"""
     Метод проведения испытаний в процессе из пула процессов Calculator.Pool
 
     :param point: точка проведения испытания
     """
+
     @staticmethod
     def worker(point: SearchDataItem) -> SearchDataItem:
         try:
-            Calculator.evaluateMethod.CalculateFunctionals(point)
+            Calculator.evaluate_method.calculate_functionals(point)
         except Exception:
-            point.SetZ(sys.float_info.max)
-            point.SetIndex(-10)
+            point.set_z(sys.float_info.max)
+            point.set_index(-10)
         return point
 
     r"""
     Метод проведения испытаний для множества точек
 
     :param points: точки проведения испытаний
     """
 
-    def CalculateFunctionalsForItems(self, points: list[SearchDataItem]) -> list[SearchDataItem]:
+    def calculate_functionals_for_items(self, points: list[SearchDataItem]) -> list[SearchDataItem]:
         # пока оставленно на случай отладки
         # for point in points:
         #     self.worker(point, self.method)
 
         # Ниже реализация цикла через пулл процессов
         points_copy = []
         for point in points:
-            sd = SearchDataItem(y=copy.deepcopy(point.point), x=copy.deepcopy(point.GetX()),
-                                functionValues=copy.deepcopy(point.functionValues),
-                                discreteValueIndex=point.GetDiscreteValueIndex())
+            sd = SearchDataItem(y=copy.deepcopy(point.point), x=copy.deepcopy(point.get_x()),
+                                function_values=copy.deepcopy(point.function_values),
+                                discrete_value_index=point.get_discrete_value_index())
             points_copy.append(sd)
 
         points_res = Calculator.pool.map(Calculator.worker, points_copy)
 
         for point, point_r in zip(points, points_res):
-            self.evaluateMethod.CopyFunctionals(point, point_r)
+            self.evaluate_method.copy_functionals(point, point_r)
 
         return points
 
     def __del__(self):
         self.pool.close()
```

### Comparing `iOpt-0.2.1/iOpt/method/index_method.py` & `iOpt-0.2.22/iOpt/method/index_method.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,141 +19,140 @@
     Класс Method содержит реализацию Алгоритма Глобального Поиска
     """
 
     def __init__(self,
                  parameters: SolverParameters,
                  task: OptimizationTask,
                  evolvent: Evolvent,
-                 searchData: SearchData
+                 search_data: SearchData
                  ):
-        super(IndexMethod, self).__init__(parameters, task, evolvent, searchData)
+        super(IndexMethod, self).__init__(parameters, task, evolvent, search_data)
 
-    def CalculateFunctionals(self, point: SearchDataItem) -> SearchDataItem:
+    def calculate_functionals(self, point: SearchDataItem) -> SearchDataItem:
         r"""
         Проведение поискового испытания в заданной точке.
 
         :param point: точка, в которой надо провести испытание.
 
         :return: точка, в которой сохранены результаты испытания.
         """
         try:
-            number_of_constraints = self.task.problem.numberOfConstraints
+            number_of_constraints = self.task.problem.number_of_constraints
             for i in range(number_of_constraints):
-                point.functionValues[i] = FunctionValue(FunctionType.CONSTRAINT, i)  # ???
-                point = self.task.Calculate(point, i)
-                point.SetZ(point.functionValues[i].value)
-                point.SetIndex(i)
-                if point.GetZ() > 0:
+                point.function_values[i] = FunctionValue(FunctionType.CONSTRAINT, i)  # ???
+                point = self.task.calculate(point, i)
+                point.set_z(point.function_values[i].value)
+                point.set_index(i)
+                if point.get_z() > 0:
                     return point
-            point.functionValues[number_of_constraints] = FunctionValue(FunctionType.OBJECTIV, number_of_constraints)
-            point = self.task.Calculate(point, number_of_constraints)
-            point.SetZ(point.functionValues[number_of_constraints].value)
-            point.SetIndex(number_of_constraints)
+            point.function_values[number_of_constraints] = FunctionValue(FunctionType.OBJECTIV, number_of_constraints)
+            point = self.task.calculate(point, number_of_constraints)
+            point.set_z(point.function_values[number_of_constraints].value)
+            point.set_index(number_of_constraints)
         except Exception:
-            point.SetZ(sys.float_info.max)
-            point.SetIndex(-10)
-
+            point.set_z(sys.float_info.max)
+            point.set_index(-10)
 
         return point
 
-    def CalculateM(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
+    def calculate_m(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
         r"""
         Вычисление оценки константы Гельдера между между curr_point и left_point.
 
         :param curr_point: правая точка интервала
         :param left_point: левая точка интервала
         """
         # Обратить внимание на вычисление расстояния, должен использоваться метод CalculateDelta
         if curr_point is None:
             print("CalculateM: curr_point is None")
             raise RuntimeError("CalculateM: curr_point is None")
         if left_point is None:
             return
-        index = curr_point.GetIndex()
+        index = curr_point.get_index()
         if index < 0:
             return
         m = 0.0
-        if left_point.GetIndex() == index:  # А если не равны, то надо искать ближайший левый/правый с таким индексом
-            m = abs(left_point.GetZ() - curr_point.GetZ()) / curr_point.delta
+        if left_point.get_index() == index:  # А если не равны, то надо искать ближайший левый/правый с таким индексом
+            m = abs(left_point.get_z() - curr_point.get_z()) / curr_point.delta
         else:
             # Ищем слева
             other_point = left_point
-            while (other_point is not None) and (other_point.GetIndex() < curr_point.GetIndex()):
-                other_point = other_point.GetLeft()
-            if other_point is not None and other_point.GetIndex() >= 0:
+            while (other_point is not None) and (other_point.get_index() < curr_point.get_index()):
+                other_point = other_point.get_left()
+            if other_point is not None and other_point.get_index() >= 0:
                 # print(index)
-                m = abs(other_point.functionValues[index].value - curr_point.GetZ()) / \
-                    self.CalculateDelta(other_point, curr_point, self.dimension)
+                m = abs(other_point.function_values[index].value - curr_point.get_z()) / \
+                    self.calculate_delta(other_point, curr_point, self.dimension)
             # Ищем справа
-            other_point = left_point.GetRight()
+            other_point = left_point.get_right()
             if other_point is not None and other_point is curr_point:  # возможно только при пересчёте M
-                other_point = other_point.GetRight()
-            while (other_point is not None) and (other_point.GetIndex() < curr_point.GetIndex()):
-                other_point = other_point.GetRight()
-            if other_point is not None and other_point.GetIndex() >= 0:
-                m = max(m, abs(curr_point.GetZ() - other_point.functionValues[index].value) / \
-                        self.CalculateDelta(curr_point, other_point, self.dimension))
+                other_point = other_point.get_right()
+            while (other_point is not None) and (other_point.get_index() < curr_point.get_index()):
+                other_point = other_point.get_right()
+            if other_point is not None and other_point.get_index() >= 0:
+                m = max(m, abs(curr_point.get_z() - other_point.function_values[index].value) / \
+                        self.calculate_delta(curr_point, other_point, self.dimension))
 
         if m > self.M[index] or (self.M[index] == 1.0 and m > 1e-12):
             self.M[index] = m
             self.recalcR = True
 
-    def CalculateGlobalR(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
+    def calculate_global_r(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
         r"""
         Вычисление глобальной характеристики интервала [left_point, curr_point].
 
         :param curr_point: правая точка интервала.
         :param left_point: левая точка интервала.
         """
 
-        # Сюда переедет целиком CalculateGlobalR из Method, а там останется только случай с равными индексами
+        # Сюда переедет целиком calculate_global_r из Method, а там останется только случай с равными индексами
         if curr_point is None:
-            print("CalculateGlobalR: Curr point is NONE")
-            raise Exception("CalculateGlobalR: Curr point is NONE")
+            print("calculate_global_r: Curr point is NONE")
+            raise Exception("calculate_global_r: Curr point is NONE")
         if left_point is None:
             curr_point.globalR = -np.infty
             return None
-        zl = left_point.GetZ()
-        zr = curr_point.GetZ()
+        zl = left_point.get_z()
+        zr = curr_point.get_z()
         r = self.parameters.r
         deltax = curr_point.delta
 
-        if left_point.GetIndex() < 0 and curr_point.GetIndex() < 0:
-            globalR = 2 * deltax - 4 * math.fabs(self.Z[0]) / (r * self.M[0])
-        elif left_point.GetIndex() == curr_point.GetIndex():
-            v = curr_point.GetIndex()
-            globalR = deltax + (zr - zl) * (zr - zl) / (deltax * self.M[v] * self.M[v] * r * r) - \
-                      2 * (zr + zl - 2 * self.Z[v]) / (r * self.M[v])
-        elif left_point.GetIndex() < curr_point.GetIndex():
-            v = curr_point.GetIndex()
-            globalR = 2 * deltax - 4 * (zr - self.Z[v]) / (r * self.M[v])
+        if left_point.get_index() < 0 and curr_point.get_index() < 0:
+            global_r = 2 * deltax - 4 * math.fabs(self.Z[0]) / (r * self.M[0])
+        elif left_point.get_index() == curr_point.get_index():
+            v = curr_point.get_index()
+            global_r = deltax + (zr - zl) * (zr - zl) / (deltax * self.M[v] * self.M[v] * r * r) - \
+                       2 * (zr + zl - 2 * self.Z[v]) / (r * self.M[v])
+        elif left_point.get_index() < curr_point.get_index():
+            v = curr_point.get_index()
+            global_r = 2 * deltax - 4 * (zr - self.Z[v]) / (r * self.M[v])
         else:
-            v = left_point.GetIndex()
-            globalR = 2 * deltax - 4 * (zl - self.Z[v]) / (r * self.M[v])
-        curr_point.globalR = globalR
-
-    def UpdateZ(self, point: SearchDataItem) -> None:
-        for i in range(point.GetIndex()):
-            if self.Z[i] > point.functionValues[i].value:
-                self.Z[i] = point.functionValues[i].value
+            v = left_point.get_index()
+            global_r = 2 * deltax - 4 * (zl - self.Z[v]) / (r * self.M[v])
+        curr_point.globalR = global_r
+
+    def update_z(self, point: SearchDataItem) -> None:
+        for i in range(point.get_index()):
+            if self.Z[i] > point.function_values[i].value:
+                self.Z[i] = point.function_values[i].value
                 self.recalcR = True
 
-    def RecalcAllCharacteristics(self) -> None:
-        for i in range(self.best.GetIndex()):
-            self.Z[i] = -self.M[i] * self.parameters.epsR
-        self.Z[self.best.GetIndex()] = self.best.GetZ()
-        super().RecalcAllCharacteristics()
+    def recalc_all_characteristics(self) -> None:
+        for i in range(self.best.get_index()):
+            self.Z[i] = -self.M[i] * self.parameters.eps_r
+        self.Z[self.best.get_index()] = self.best.get_z()
+        super().recalc_all_characteristics()
 
-    def UpdateOptimum(self, point: SearchDataItem) -> None:
+    def update_optimum(self, point: SearchDataItem) -> None:
         r"""
         Обновляет оценку оптимума.
 
         :param point: точка нового испытания.
         """
 
-        if self.best is None or self.best.GetIndex() < point.GetIndex() or (
-                self.best.GetIndex() == point.GetIndex() and point.GetZ() < self.best.GetZ()):
+        if self.best is None or self.best.get_index() < point.get_index() or (
+                self.best.get_index() == point.get_index() and point.get_z() < self.best.get_z()):
             self.best = point
             self.recalcR = True
-            self.Z[point.GetIndex()] = point.GetZ()
+            self.Z[point.get_index()] = point.get_z()
         # self.UpdateZ(point)
-        self.searchData.solution.bestTrials[0] = self.best
+        self.search_data.solution.best_trials[0] = self.best
```

### Comparing `iOpt-0.2.1/iOpt/method/index_method_calculator.py` & `iOpt-0.2.22/iOpt/method/index_method_calculator.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,40 +12,40 @@
     """
 
     def __init__(self,
                  task: OptimizationTask
                  ):
         self.task = task
 
-    def CalculateFunctionals(self, point: SearchDataItem) -> SearchDataItem:
+    def calculate_functionals(self, point: SearchDataItem) -> SearchDataItem:
         r"""
         Проведение поискового испытания в заданной точке.
 
         :param point: точка, в которой надо провести испытание.
 
         :return: точка, в которой сохранены результаты испытания.
         """
-        number_of_constraints = self.task.problem.numberOfConstraints
+        number_of_constraints = self.task.problem.number_of_constraints
         for i in range(number_of_constraints):
-            point.functionValues[i] = FunctionValue(FunctionType.CONSTRAINT, i)
-            point = self.task.Calculate(point, i)
-            point.SetZ(point.functionValues[i].value)
-            point.SetIndex(i)
-            if point.GetZ() < 0:
+            point.function_values[i] = FunctionValue(FunctionType.CONSTRAINT, i)
+            point = self.task.calculate(point, i)
+            point.set_z(point.function_values[i].value)
+            point.set_index(i)
+            if point.get_z() < 0:
                 return point
-        point.functionValues[number_of_constraints] = FunctionValue(FunctionType.OBJECTIV, 0)
-        point = self.task.Calculate(point, number_of_constraints)
-        point.SetZ(point.functionValues[number_of_constraints].value)
-        point.SetIndex(number_of_constraints)
+        point.function_values[number_of_constraints] = FunctionValue(FunctionType.OBJECTIV, 0)
+        point = self.task.calculate(point, number_of_constraints)
+        point.set_z(point.function_values[number_of_constraints].value)
+        point.set_index(number_of_constraints)
         return point
 
-    def CopyFunctionals(self, dist_point: SearchDataItem, src_point: SearchDataItem):
+    def copy_functionals(self, dist_point: SearchDataItem, src_point: SearchDataItem):
         r"""
         Копирование поискового испытания.
 
         :param dist_point: точка, в которую копируются значения испытаний.
         :param src_point: точка c результатами испытаний.
         """
 
-        dist_point.functionValues = copy.deepcopy(src_point.functionValues)
-        dist_point.SetZ(src_point.GetZ())
-        dist_point.SetIndex(src_point.GetIndex())
+        dist_point.function_values = copy.deepcopy(src_point.function_values)
+        dist_point.set_z(src_point.get_z())
+        dist_point.set_index(src_point.get_index())
```

### Comparing `iOpt-0.2.1/iOpt/method/listener.py` & `iOpt-0.2.22/iOpt/method/listener.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import numpy as np
 
 class Listener:
     """
     Базовый класс слушателя событий.
     """
 
-    def BeforeMethodStart(self, method: Method):
+    def before_method_start(self, method: Method):
         pass
 
-    def OnEndIteration(self, currPoints : np.ndarray(shape=(1), dtype=SearchDataItem), solution: Solution):
+    def on_end_iteration(self, curr_points : np.ndarray(shape=(1), dtype=SearchDataItem), solution: Solution):
         pass
 
-    def OnMethodStop(self, searchData: SearchData, solution: Solution, status: bool):
+    def on_method_stop(self, search_data: SearchData, solution: Solution, status: bool):
         pass
 
-    def OnRefrash(self):
+    def on_refrash(self):
         pass
```

### Comparing `iOpt-0.2.1/iOpt/method/method.py` & `iOpt-0.2.22/iOpt/method/method.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,48 +21,48 @@
     Класс Method содержит реализацию Алгоритма Глобального Поиска
     """
 
     def __init__(self,
                  parameters: SolverParameters,
                  task: OptimizationTask,
                  evolvent: Evolvent,
-                 searchData: SearchData
+                 search_data: SearchData
                  ):
         r"""
         Конструктор класса Method
 
         :param parameters: параметры решения задачи оптимизации.
         :param task: обёртка решаемой задачи.
         :param evolvent: развертка Пеано-Гильберта, отображающая отрезок [0,1] на многомерную область D.
-        :param searchData: структура данных для хранения накопленной поисковой информации.
+        :param search_data: структура данных для хранения накопленной поисковой информации.
         """
         self.stop: bool = False
         self.recalcR: bool = True
         self.recalcM: bool = True
-        self.iterationsCount: int = 0
+        self.iterations_count: int = 0
         self.best: SearchDataItem = None
 
         self.parameters = parameters
         self.task = task
         self.evolvent = evolvent
-        self.searchData = searchData
-        # change to np.array, but indexing np is slower
-        self.M = [1.0 for _ in range(task.problem.numberOfObjectives + task.problem.numberOfConstraints)]
-        self.Z = [np.infty for _ in range(task.problem.numberOfObjectives + task.problem.numberOfConstraints)]
-        self.dimension = task.problem.numberOfFloatVariables  # А ДЛЯ ДИСКРЕТНЫХ?
-        self.searchData.solution.solutionAccuracy = np.infty
-        self.numberOfAllFunctions = task.problem.numberOfObjectives + task.problem.numberOfConstraints
+        self.search_data = search_data
+
+        self.M = [1.0 for _ in range(task.problem.number_of_objectives + task.problem.number_of_constraints)]
+        self.Z = [np.infty for _ in range(task.problem.number_of_objectives + task.problem.number_of_constraints)]
+        self.dimension = task.problem.number_of_float_variables
+        self.search_data.solution.solution_accuracy = np.infty
+        self.numberOfAllFunctions = task.problem.number_of_objectives + task.problem.number_of_constraints
 
     @property
     def min_delta(self):
-        return self.searchData.solution.solutionAccuracy
+        return self.search_data.solution.solution_accuracy
 
     @min_delta.setter
     def min_delta(self, val):
-        self.searchData.solution.solutionAccuracy = val
+        self.search_data.solution.solution_accuracy = val
 
     # @staticmethod
     # def CalculateDelta(lx: float, rx: float, dimension: int) -> float:
     #     """
     #     Вычисляет гельдерово расстояние в метрике Гельдера между двумя точками на отрезке [0,1],
     #       полученными при редукции размерности.
     #
@@ -70,337 +70,335 @@
     #     :param rx: правая точка
     #     :param dimension: размерность исходного пространства
     #
     #     :return: гельдерово расстояние между lx и rx.
     #     """
     #     return pow(rx - lx, 1.0 / dimension)
 
-    def CalculateDelta(self, lPoint: SearchDataItem, rPoint: SearchDataItem, dimension: int) -> float:
+    def calculate_delta(self, l_point: SearchDataItem, r_point: SearchDataItem, dimension: int) -> float:
         """
         Вычисляет гельдерово расстояние в метрике Гельдера между двумя точками на отрезке [0,1],
           полученными при редукции размерности.
 
-        :param lPoint: левая точка
-        :param rPoint: правая точка
+        :param l_point: левая точка
+        :param r_point: правая точка
         :param dimension: размерность исходного пространства
 
         :return: гельдерово расстояние между lx и rx.
         """
-        return pow(rPoint.GetX() - lPoint.GetX(), 1.0 / dimension)
+        return pow(r_point.get_x() - l_point.get_x(), 1.0 / dimension)
 
-    def FirstIteration(self, calculator: Calculator = None) -> list[SearchDataItem]:
+    def first_iteration(self, calculator: Calculator = None) -> list[SearchDataItem]:
         r"""
         Метод выполняет первую итерацию Алгоритма Глобального Поиска.
         """
 
         # Генерация 3х точек 0, 0.5, 1. Значение функции будет вычисляться только в точке 0.5.
         # Интервал задаётся правой точкой, т.е. будут интервалы только для 0.5 и 1
-        left = SearchDataItem(Point(self.evolvent.GetImage(0.0), None), 0.,
-                              functionValues=[FunctionValue()] * self.numberOfAllFunctions)
-        right = SearchDataItem(Point(self.evolvent.GetImage(1.0), None), 1.0,
-                               functionValues=[FunctionValue()] * self.numberOfAllFunctions)
+        left = SearchDataItem(Point(self.evolvent.get_image(0.0), None), 0.,
+                              function_values=[FunctionValue()] * self.numberOfAllFunctions)
+        right = SearchDataItem(Point(self.evolvent.get_image(1.0), None), 1.0,
+                               function_values=[FunctionValue()] * self.numberOfAllFunctions)
 
         items: list[SearchDataItem] = []
 
-        if self.parameters.startPoint:
-            numberOfPoint: int = self.parameters.numberOfParallelPoints - 1
-            h: float = 1.0 / (numberOfPoint + 1)
+        if self.parameters.start_point:
+            number_of_point: int = self.parameters.number_of_parallel_points - 1
+            h: float = 1.0 / (number_of_point + 1)
 
-            yStartPoint = Point(copy.copy(self.parameters.startPoint.floatVariables), None)
-            xStartPoint = self.evolvent.GetInverseImage(self.parameters.startPoint.floatVariables)
+            ystart_point = Point(copy.copy(self.parameters.start_point.float_variables), None)
+            xstart_point = self.evolvent.get_inverse_image(self.parameters.start_point.float_variables)
 
-            itemStartPoint = SearchDataItem(yStartPoint, xStartPoint,
-                                  functionValues=[FunctionValue()] * self.numberOfAllFunctions)
+            itemstart_point = SearchDataItem(ystart_point, xstart_point,
+                                             function_values=[FunctionValue()] * self.numberOfAllFunctions)
 
-            isAddStartPoint: bool = False
+            is_add_start_point: bool = False
 
-            for i in range(numberOfPoint):
+            for i in range(number_of_point):
                 x = h * (i + 1)
-                y = Point(self.evolvent.GetImage(x), None)
+                y = Point(self.evolvent.get_image(x), None)
                 item = SearchDataItem(y, x,
-                                      functionValues=[FunctionValue()] * self.numberOfAllFunctions)
-                if x < xStartPoint < h * (i + 2):
+                                      function_values=[FunctionValue()] * self.numberOfAllFunctions)
+                if x < xstart_point < h * (i + 2):
                     items.append(item)
-                    items.append(itemStartPoint)
-                    isAddStartPoint = True
+                    items.append(itemstart_point)
+                    is_add_start_point = True
                 else:
                     items.append(item)
 
-            if not isAddStartPoint:
-                items.append(itemStartPoint)
+            if not is_add_start_point:
+                items.append(itemstart_point)
         else:
 
-            numberOfPoint: int = self.parameters.numberOfParallelPoints
-            h: float = 1.0 / (numberOfPoint + 1)
+            number_of_point: int = self.parameters.number_of_parallel_points
+            h: float = 1.0 / (number_of_point + 1)
 
-            for i in range(numberOfPoint):
+            for i in range(number_of_point):
                 x = h * (i + 1)
-                y = Point(self.evolvent.GetImage(x), None)
+                y = Point(self.evolvent.get_image(x), None)
                 item = SearchDataItem(y, x,
-                                      functionValues=[FunctionValue()] * self.numberOfAllFunctions)
+                                      function_values=[FunctionValue()] * self.numberOfAllFunctions)
                 items.append(item)
 
         if calculator is None:
             for item in items:
-                self.CalculateFunctionals(item)
+                self.calculate_functionals(item)
+                self.update_optimum(item)
         else:
-            calculator.CalculateFunctionalsForItems(items)
+            calculator.calculate_functionals_for_items(items)
 
         for item in items:
-            self.UpdateOptimum(item)
+            self.update_optimum(item)
 
         left.delta = 0
-        self.CalculateGlobalR(left, None)
+        self.calculate_global_r(left, None)
 
-        items[0].delta = self.CalculateDelta(left, items[0], self.dimension)
-        self.CalculateGlobalR(items[0], left)
+        items[0].delta = self.calculate_delta(left, items[0], self.dimension)
+        self.calculate_global_r(items[0], left)
         for id_item, item in enumerate(items):
             if id_item > 0:
-                items[id_item].delta = self.CalculateDelta(items[id_item - 1], items[id_item], self.dimension)
-                self.CalculateGlobalR(items[id_item], items[id_item - 1])
-                self.CalculateM(items[id_item], items[id_item - 1])
+                items[id_item].delta = self.calculate_delta(items[id_item - 1], items[id_item], self.dimension)
+                self.calculate_global_r(items[id_item], items[id_item - 1])
+                self.calculate_m(items[id_item], items[id_item - 1])
 
-        right.delta = self.CalculateDelta(items[-1], right, self.dimension)
-        self.CalculateGlobalR(right, items[-1])
+        right.delta = self.calculate_delta(items[-1], right, self.dimension)
+        self.calculate_global_r(right, items[-1])
 
         # вставить left  и right, потом middle
-        self.searchData.InsertFirstDataItem(left, right)
-        # self.searchData.InsertDataItem(middle, right)
+        self.search_data.insert_first_data_item(left, right)
+        # self.search_data.InsertDataItem(middle, right)
 
         for item in items:
-            self.searchData.InsertDataItem(item, right)
+            self.search_data.insert_data_item(item, right)
 
         self.recalcR = True
         self.recalcM = True
 
-        self.iterationsCount = len(items)
-        self.searchData.solution.numberOfGlobalTrials = len(items)
+        self.iterations_count = len(items)
+        self.search_data.solution.number_of_global_trials = len(items)
 
         return items
 
-    def CheckStopCondition(self) -> bool:
+    def check_stop_condition(self) -> bool:
         r"""
         Проверка условия остановки.
         Алгоритм должен завершить работу, когда достигнута точность eps или превышен лимит итераций.
 
         :return: True, если выполнен критерий остановки; False - в противном случае.
         """
-        if self.min_delta < self.parameters.eps or self.iterationsCount >= self.parameters.globalMethodIterationCount:
+        if self.min_delta < self.parameters.eps or self.iterations_count >= self.parameters.global_method_iteration_count:
             self.stop = True
         else:
             self.stop = False
 
         return self.stop
 
-    def RecalcM(self) -> None:
+    def recalc_m(self) -> None:
         r"""
         Пересчёт оценки константы Липшица.
         """
         if self.recalcM is not True:
             return
-        for item in self.searchData:
-            self.CalculateM(item, item.GetLeft())
+        for item in self.search_data:
+            self.calculate_m(item, item.get_left())
         self.recalcM = False
 
-    def RecalcAllCharacteristics(self) -> None:
+    def recalc_all_characteristics(self) -> None:
         r"""
         Пересчёт характеристик для всех поисковых интервалов.
         """
         if self.recalcR is not True:
             return
-        self.searchData.ClearQueue()
-        for item in self.searchData:  # Должно работать...
-            self.CalculateGlobalR(item, item.GetLeft())
+        self.search_data.clear_queue()
+        for item in self.search_data:  # Должно работать...
+            self.calculate_global_r(item, item.get_left())
             # self.CalculateLocalR(item)
-        self.searchData.RefillQueue()
+        self.search_data.refill_queue()
         self.recalcR = False
 
-    def CalculateNextPointCoordinate(self, point: SearchDataItem) -> float:
+    def calculate_next_point_coordinate(self, point: SearchDataItem) -> float:
         r"""
         Вычисление точки нового испытания :math:`x^{k+1}` в заданном интервале :math:`[x_{t-1},x_t]`.
 
         :param point: интервал, заданный его правой точкой :math:`x_t`.
 
         :return: точка нового испытания :math:`x^{k+1}` в этом интервале.
         """
         # https://github.com/MADZEROPIE/ags_nlp_solver/blob/cedcbcc77aa08ef1ba591fc7400c3d558f65a693/solver/src/solver.cpp#L420
-        left = point.GetLeft()
+        left = point.get_left()
         if left is None:
             print("CalculateNextPointCoordinate: Left point is NONE")
             raise Exception("CalculateNextPointCoordinate: Left point is NONE")
-        xl = left.GetX()
-        xr = point.GetX()
-        idl = left.GetIndex()
-        idr = point.GetIndex()
+        xl = left.get_x()
+        xr = point.get_x()
+        idl = left.get_index()
+        idr = point.get_index()
         if idl == idr and idl >= 0:
             v = idr
-            dif = point.GetZ() - left.GetZ()
+            dif = point.get_z() - left.get_z()
             dg = -1.0
             if dif > 0:
                 dg = 1.0
 
             x = 0.5 * (xl + xr)
-            x -= 0.5 * dg * pow(abs(dif) / self.M[v], self.task.problem.numberOfFloatVariables) / self.parameters.r
+            x -= 0.5 * dg * pow(abs(dif) / self.M[v], self.task.problem.number_of_float_variables) / self.parameters.r
 
         else:
             x = 0.5 * (xl + xr)
         if x <= xl or x >= xr:
             print(f"CalculateNextPointCoordinate: x is outside of interval {x} {xl} {xr}")
             raise Exception("CalculateNextPointCoordinate: x is outside of interval")
         return x
 
-    def CalculateIterationPoint(self) -> Tuple[SearchDataItem, SearchDataItem]:  # return  (new, old)
+    def calculate_iteration_point(self) -> Tuple[SearchDataItem, SearchDataItem]:  # return  (new, old)
         r"""
         Вычисление точки нового испытания :math:`x^{k+1}`.
 
         :return: :math:`x^{k+1}` - точка нового испытания, и :math:`x_t` - левая точка интервала :math:`[x_{t-1},x_t]`,
           которому принадлежит :math:`x^{k+1}`, т.е. :math:`x^{k+1} \in [x_{t-1},x_t]`.
         """
         if self.recalcM is True:
-            self.RecalcM()
+            self.recalc_m()
         if self.recalcR is True:
-            self.RecalcAllCharacteristics()
+            self.recalc_all_characteristics()
 
-        old = self.searchData.GetDataItemWithMaxGlobalR()
+        old = self.search_data.get_data_item_with_max_global_r()
         self.min_delta = min(old.delta, self.min_delta)
-        newx = self.CalculateNextPointCoordinate(old)
-        newy = self.evolvent.GetImage(newx)
+        newx = self.calculate_next_point_coordinate(old)
+        newy = self.evolvent.get_image(newx)
         new = copy.deepcopy(SearchDataItem(Point(newy, []), newx,
-                                           functionValues=[FunctionValue()] * self.numberOfAllFunctions))
+                                           function_values=[FunctionValue()] * self.numberOfAllFunctions))
 
         # Обновление числа испытаний
-        self.searchData.solution.numberOfGlobalTrials += 1
+        self.search_data.solution.number_of_global_trials += 1
 
         return new, old
 
-    def CalculateFunctionals(self, point: SearchDataItem) -> SearchDataItem:
+    def calculate_functionals(self, point: SearchDataItem) -> SearchDataItem:
         r"""
         Проведение поискового испытания в заданной точке.
 
         :param point: точка, в которой надо провести испытание.
 
         :return: точка, в которой сохранены результаты испытания.
         """
         try:
-            point = self.task.Calculate(point, 0)
-            point.SetZ(point.functionValues[0].value)
-            point.SetIndex(0)
+            point = self.task.calculate(point, 0)
+            point.set_z(point.function_values[0].value)
+            point.set_index(0)
         except Exception:
-            point.SetZ(sys.float_info.max)
-            point.SetIndex(-10)
+            point.set_z(sys.float_info.max)
+            point.set_index(-10)
 
         return point
 
-    def CalculateM(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
+    def calculate_m(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
         r"""
         Вычисление оценки константы Гельдера между между curr_point и left_point.
 
         :param curr_point: правая точка интервала
         :param left_point: левая точка интервала
         """
         if curr_point is None:
             print("CalculateM: curr_point is None")
             raise RuntimeError("CalculateM: curr_point is None")
         if left_point is None:
             return
-        index = curr_point.GetIndex()
-        if left_point.GetIndex() == index and index >= 0:  # А если не равны, то надо искать ближайший левый/правый с таким индексом
-            m = abs(left_point.GetZ() - curr_point.GetZ()) / curr_point.delta
+        index = curr_point.get_index()
+        if left_point.get_index() == index and index >= 0:  # А если не равны, то надо искать ближайший левый/правый с таким индексом
+            m = abs(left_point.get_z() - curr_point.get_z()) / curr_point.delta
             if m > self.M[index]:
                 self.M[index] = m
                 self.recalcR = True
 
-    # def CalculateM(self, point: SearchDataItem):  # В python нет такой перегрузки функций, надо менять название
-    #     self.CalculateM(point, point.GetLeft())
-
-    def CalculateGlobalR(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
+    def calculate_global_r(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
         r"""
         Вычисление глобальной характеристики интервала [left_point, curr_point].
 
         :param curr_point: правая точка интервала.
         :param left_point: левая точка интервала.
         """
         if curr_point is None:
-            print("CalculateGlobalR: Curr point is NONE")
-            raise Exception("CalculateGlobalR: Curr point is NONE")
+            print("calculate_global_r: Curr point is NONE")
+            raise Exception("calculate_global_r: Curr point is NONE")
         if left_point is None:
             curr_point.globalR = -np.infty
             return None
-        zl = left_point.GetZ()
-        zr = curr_point.GetZ()
+        zl = left_point.get_z()
+        zr = curr_point.get_z()
         r = self.parameters.r
         deltax = curr_point.delta
 
-        if left_point.GetIndex() < 0 and curr_point.GetIndex() < 0:
-            globalR = 2 * deltax - 4 * math.fabs(self.Z[0]) / (r * self.M[0])
-        elif left_point.GetIndex() == curr_point.GetIndex():
-            v = curr_point.GetIndex()
-            globalR = deltax + (zr - zl) * (zr - zl) / (deltax * self.M[v] * self.M[v] * r * r) - \
-                      2 * (zr + zl - 2 * self.Z[v]) / (r * self.M[v])
-        elif left_point.GetIndex() < curr_point.GetIndex():
-            v = curr_point.GetIndex()
-            globalR = 2 * deltax - 4 * (zr - self.Z[v]) / (r * self.M[v])
+        if left_point.get_index() < 0 and curr_point.get_index() < 0:
+            global_r = 2 * deltax - 4 * math.fabs(self.Z[0]) / (r * self.M[0])
+        elif left_point.get_index() == curr_point.get_index():
+            v = curr_point.get_index()
+            global_r = deltax + (zr - zl) * (zr - zl) / (deltax * self.M[v] * self.M[v] * r * r) - \
+                       2 * (zr + zl - 2 * self.Z[v]) / (r * self.M[v])
+        elif left_point.get_index() < curr_point.get_index():
+            v = curr_point.get_index()
+            global_r = 2 * deltax - 4 * (zr - self.Z[v]) / (r * self.M[v])
         else:
-            v = left_point.GetIndex()
-            globalR = 2 * deltax - 4 * (zl - self.Z[v]) / (r * self.M[v])
-        curr_point.globalR = globalR
+            v = left_point.get_index()
+            global_r = 2 * deltax - 4 * (zl - self.Z[v]) / (r * self.M[v])
+        curr_point.globalR = global_r
 
-    def RenewSearchData(self, newpoint: SearchDataItem, oldpoint: SearchDataItem) -> None:
+    def renew_search_data(self, newpoint: SearchDataItem, oldpoint: SearchDataItem) -> None:
         """
         Метод обновляет всю поисковую информацию: длины интервалов, константы Гёльдера, все характеристики и вставляет
           новую точку в хранилище.
 
         :param newpoint: новая точка
         :param oldpoint: правая точка интервала, которому принадлежит новая точка
         """
 
         # oldpoint.delta = Method.CalculateDelta(newpoint.GetX(), oldpoint.GetX(), self.dimension)
         # newpoint.delta = Method.CalculateDelta(oldpoint.GetLeft().GetX(), newpoint.GetX(), self.dimension)
 
-        oldpoint.delta = self.CalculateDelta(newpoint, oldpoint, self.dimension)
-        newpoint.delta = self.CalculateDelta(oldpoint.GetLeft(), newpoint, self.dimension)
+        oldpoint.delta = self.calculate_delta(newpoint, oldpoint, self.dimension)
+        newpoint.delta = self.calculate_delta(oldpoint.get_left(), newpoint, self.dimension)
 
-        self.CalculateM(newpoint, oldpoint.GetLeft())
-        self.CalculateM(oldpoint, newpoint)
+        self.calculate_m(newpoint, oldpoint.get_left())
+        self.calculate_m(oldpoint, newpoint)
 
-        self.CalculateGlobalR(newpoint, oldpoint.GetLeft())
-        self.CalculateGlobalR(oldpoint, newpoint)
+        self.calculate_global_r(newpoint, oldpoint.get_left())
+        self.calculate_global_r(oldpoint, newpoint)
 
-        self.searchData.InsertDataItem(newpoint, oldpoint)
+        self.search_data.insert_data_item(newpoint, oldpoint)
 
-    def UpdateOptimum(self, point: SearchDataItem) -> None:
+    def update_optimum(self, point: SearchDataItem) -> None:
         r"""
         Обновляет оценку оптимума.
 
         :param point: точка нового испытания.
         """
-        if self.best is None or self.best.GetIndex() < point.GetIndex():
+        if self.best is None or self.best.get_index() < point.get_index():
             self.best = point
             self.recalcR = True
-            self.Z[point.GetIndex()] = point.GetZ()
-        elif self.best.GetIndex() == point.GetIndex() and point.GetZ() < self.best.GetZ():
+            self.Z[point.get_index()] = point.get_z()
+        elif self.best.get_index() == point.get_index() and point.get_z() < self.best.get_z():
             self.best = point
             self.recalcR = True
-            self.Z[point.GetIndex()] = point.GetZ()
-        self.searchData.solution.bestTrials[0] = self.best
+            self.Z[point.get_index()] = point.get_z()
+        self.search_data.solution.best_trials[0] = self.best
 
-    def FinalizeIteration(self) -> None:
+    def finalize_iteration(self) -> None:
         r"""
         Заканчивает итерацию, обновляет счётчик итераций.
         """
-        self.iterationsCount += 1
+        self.iterations_count += 1
 
-    def GetIterationsCount(self) -> int:
+    def get_iterations_count(self) -> int:
         r"""
         Возвращает число выполненных итераций.
 
         :return:  число выполненных итераций.
         """
-        return self.iterationsCount
+        return self.iterations_count
 
-    def GetOptimumEstimation(self) -> SearchDataItem:
+    def get_optimum_estimation(self) -> SearchDataItem:
         r"""
         Возвращает оценку оптимума.
 
         :return: текущая оценка оптимума.
         """
         return self.best
```

### Comparing `iOpt-0.2.1/iOpt/method/mixed_integer_method.py` & `iOpt-0.2.22/iOpt/method/mixed_integer_method.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,247 +25,248 @@
     Класс Method содержит реализацию Алгоритма Глобального Поиска
     """
 
     def __init__(self,
                  parameters: SolverParameters,
                  task: OptimizationTask,
                  evolvent: Evolvent,
-                 searchData: SearchData
+                 search_data: SearchData
                  ):
-        super(MixedIntegerMethod, self).__init__(parameters, task, evolvent, searchData)
+        super(MixedIntegerMethod, self).__init__(parameters, task, evolvent, search_data)
 
         # u = {i, j, k}, i = {0, 1, 2}, j = {0, 1}, k = {0, 1, 2, 3, 4} -> 3*2*4=24
 
-        list_discreteValues = list(task.problem.discreteVariableValues)
-        self.discreteParameters = list(itertools.product(*list_discreteValues))
+        list_discrete_values = list(task.problem.discrete_variable_values)
+        self.discreteParameters = list(itertools.product(*list_discrete_values))
         # определяем количество сочетаний параметров
         self.numberOfParameterCombinations = len(self.discreteParameters)
         # 0 0.5 1  1.5 2   2.5  3    3.5 4
 
-    def FirstIteration(self, calculator: Calculator = None) -> list[SearchDataItem]:
+    def first_iteration(self, calculator: Calculator = None) -> list[SearchDataItem]:
         r"""
         Метод выполняет первую итерацию Алгоритма Глобального Поиска.
         """
-        self.iterationsCount = 1
+        self.iterations_count = 1
         # Генерация 3х точек 0, 0.5, 1. Значение функции будет вычисляться только в точке 0.5.
         # Интервал задаётся правой точкой, т.е. будут интервалы только для 0.5 и 1
-        left = SearchDataItem(Point(self.evolvent.GetImage(0.0), self.discreteParameters[0]), 0.0,
-                              functionValues=[FunctionValue()] * self.numberOfAllFunctions)
-        image_right = self.evolvent.GetImage(1.0)
+        left = SearchDataItem(Point(self.evolvent.get_image(0.0), self.discreteParameters[0]), 0.0,
+                              function_values=[FunctionValue()] * self.numberOfAllFunctions)
+        image_right = self.evolvent.get_image(1.0)
         right: list[SearchDataItem] = []
 
         # [(x + y - 1)/y]
 
         items: list[SearchDataItem] = []
         image_x: list = []
         is_init_image_x: bool = False
 
-        numberOfPointsInOneInterval = \
-            int(math.modf((self.parameters.numberOfParallelPoints + self.numberOfParameterCombinations - 1)
+        number_of_points_in_one_interval = \
+            int(math.modf((self.parameters.number_of_parallel_points + self.numberOfParameterCombinations - 1)
                           / self.numberOfParameterCombinations)[1])
 
-        h: float = 1.0 / (numberOfPointsInOneInterval + 1)
-
-        if self.parameters.startPoint:
+        h: float = 1.0 / (number_of_points_in_one_interval + 1)
 
+        if self.parameters.start_point:
             for id_comb in range(self.numberOfParameterCombinations):
+                if np.array_equal(self.parameters.start_point.discrete_variables, self.discreteParameters[id_comb]):
+                    num_temp = number_of_points_in_one_interval - 1
 
-                if np.array_equal(self.parameters.startPoint.discreteVariables, self.discreteParameters[id_comb]):
-                    numTemp = numberOfPointsInOneInterval - 1
-
-                    yStartPoint = Point(copy.copy(self.parameters.startPoint.floatVariables),
-                                        self.discreteParameters[id_comb])
-                    xStartPoint = id_comb + self.evolvent.GetInverseImage(self.parameters.startPoint.floatVariables)
-                    itemStartPoint = SearchDataItem(yStartPoint, xStartPoint, discreteValueIndex=id_comb,
-                                          functionValues=[FunctionValue()] * self.numberOfAllFunctions)
+                    ystart_point = Point(copy.copy(self.parameters.start_point.float_variables),
+                                         self.discreteParameters[id_comb])
+                    xstart_point = id_comb + self.evolvent.get_inverse_image(
+                        self.parameters.start_point.float_variables)
+                    itemstart_point = SearchDataItem(ystart_point, xstart_point, discrete_value_index=id_comb,
+                                                     function_values=[FunctionValue()] * self.numberOfAllFunctions)
 
-                    isAddStartPoint: bool = False
+                    is_add_start_point: bool = False
 
-                    for i in range(numTemp):
+                    for i in range(num_temp):
                         x = id_comb + h * (i + 1)
 
-                        y_temp = self.evolvent.GetImage(x)
+                        y_temp = self.evolvent.get_image(x)
 
                         y = Point(copy.copy(y_temp), self.discreteParameters[id_comb])
-                        item = SearchDataItem(y, x, discreteValueIndex=id_comb,
-                                              functionValues=[FunctionValue()] * self.numberOfAllFunctions)
-                        if x < xStartPoint < id_comb + h * (i + 1):
+                        item = SearchDataItem(y, x, discrete_value_index=id_comb,
+                                              function_values=[FunctionValue()] * self.numberOfAllFunctions)
+                        if x < xstart_point < id_comb + h * (i + 1):
                             items.append(item)
-                            items.append(itemStartPoint)
-                            isAddStartPoint = True
+                            items.append(itemstart_point)
+                            is_add_start_point = True
                         else:
                             items.append(item)
 
-                    if not isAddStartPoint:
-                        items.append(itemStartPoint)
+                    if not is_add_start_point:
+                        items.append(itemstart_point)
 
                 else:
-
-                    for i in range(numberOfPointsInOneInterval):
+                    for i in range(number_of_points_in_one_interval):
                         x = id_comb + h * (i + 1)
                         if not is_init_image_x:
-                            image_x.append(self.evolvent.GetImage(x))
+                            image_x.append(self.evolvent.get_image(x))
 
                         y = Point(copy.copy(image_x[i]), self.discreteParameters[id_comb])
-                        item = SearchDataItem(y, x, discreteValueIndex=id_comb,
-                                              functionValues=[FunctionValue()] * self.numberOfAllFunctions)
+                        item = SearchDataItem(y, x, discrete_value_index=id_comb,
+                                              function_values=[FunctionValue()] * self.numberOfAllFunctions)
                         items.append(item)
 
                 right.append(SearchDataItem(Point(copy.copy(image_right), self.discreteParameters[id_comb]),
                                             float(id_comb + 1),
-                                            functionValues=[FunctionValue()] * self.numberOfAllFunctions,
-                                            discreteValueIndex=id_comb))
+                                            function_values=[FunctionValue()] * self.numberOfAllFunctions,
+                                            discrete_value_index=id_comb))
 
                 if not is_init_image_x:
                     is_init_image_x = True
         else:
             for id_comb in range(self.numberOfParameterCombinations):
-                for i in range(numberOfPointsInOneInterval):
+                for i in range(number_of_points_in_one_interval):
                     x = id_comb + h * (i + 1)
                     if not is_init_image_x:
-                        image_x.append(self.evolvent.GetImage(x))
+                        image_x.append(self.evolvent.get_image(x))
 
                     y = Point(copy.copy(image_x[i]), self.discreteParameters[id_comb])
-                    item = SearchDataItem(y, x, discreteValueIndex=id_comb,
-                                          functionValues=[FunctionValue()] * self.numberOfAllFunctions)
+                    item = SearchDataItem(y, x, discrete_value_index=id_comb,
+                                          function_values=[FunctionValue()] * self.numberOfAllFunctions)
                     items.append(item)
 
                 right.append(SearchDataItem(Point(copy.copy(image_right), self.discreteParameters[id_comb]),
                                             float(id_comb + 1),
-                                            functionValues=[FunctionValue()] * self.numberOfAllFunctions,
-                                            discreteValueIndex=id_comb))
+                                            function_values=[FunctionValue()] * self.numberOfAllFunctions,
+                                            discrete_value_index=id_comb))
 
                 if not is_init_image_x:
                     is_init_image_x = True
 
         if calculator is None:
             for item in items:
-                self.CalculateFunctionals(item)
+                self.calculate_functionals(item)
+                self.update_optimum(item)
         else:
-            calculator.CalculateFunctionalsForItems(items)
+            calculator.calculate_functionals_for_items(items)
 
         for item in items:
-            self.UpdateOptimum(item)
+            self.update_optimum(item)
 
         left.delta = 0
         # left надо для всех считать
-        self.CalculateGlobalR(left, None)
+        self.calculate_global_r(left, None)
 
-        items[0].delta = self.CalculateDelta(left, items[0], self.dimension)
-        self.CalculateGlobalR(items[0], left)
+        items[0].delta = self.calculate_delta(left, items[0], self.dimension)
+        self.calculate_global_r(items[0], left)
 
         for id_comb in range(self.numberOfParameterCombinations):
             if id_comb > 0:
                 # вычисление left
-                index = id_comb * numberOfPointsInOneInterval
-                items[index].delta = self.CalculateDelta(right[id_comb - 1], items[index], self.dimension)
-                self.CalculateGlobalR(items[index], right[id_comb - 1])
-
-            for id_item in range(1, numberOfPointsInOneInterval):
-                index = id_comb * numberOfPointsInOneInterval + id_item
-                items[index].delta = self.CalculateDelta(items[index - 1], items[index], self.dimension)
-                self.CalculateGlobalR(items[index], items[index - 1])
-                self.CalculateM(items[index], items[index - 1])
-
-            left_index = id_comb * numberOfPointsInOneInterval + numberOfPointsInOneInterval - 1
-            right[id_comb].delta = self.CalculateDelta(items[left_index], right[id_comb], self.dimension)
-            self.CalculateGlobalR(right[id_comb], items[left_index])
+                index = id_comb * number_of_points_in_one_interval
+                items[index].delta = self.calculate_delta(right[id_comb - 1], items[index], self.dimension)
+                self.calculate_global_r(items[index], right[id_comb - 1])
+
+            for id_item in range(1, number_of_points_in_one_interval):
+                index = id_comb * number_of_points_in_one_interval + id_item
+                items[index].delta = self.calculate_delta(items[index - 1], items[index], self.dimension)
+                self.calculate_global_r(items[index], items[index - 1])
+                self.calculate_m(items[index], items[index - 1])
+
+            left_index = id_comb * number_of_points_in_one_interval + number_of_points_in_one_interval - 1
+            right[id_comb].delta = self.calculate_delta(items[left_index], right[id_comb], self.dimension)
+            self.calculate_global_r(right[id_comb], items[left_index])
 
         # вставить left  и right, потом middle
-        self.searchData.InsertFirstDataItem(left, right[-1])
+        self.search_data.insert_first_data_item(left, right[-1])
 
         for right_item in range(self.numberOfParameterCombinations):
             if right_item < self.numberOfParameterCombinations - 1:
-                self.searchData.InsertDataItem(right[right_item], right[-1])
+                self.search_data.insert_data_item(right[right_item], right[-1])
 
-            for id_item in range(numberOfPointsInOneInterval):
-                index = right_item * numberOfPointsInOneInterval + id_item
-                self.searchData.InsertDataItem(items[index], right[right_item])
+            for id_item in range(number_of_points_in_one_interval):
+                index = right_item * number_of_points_in_one_interval + id_item
+                self.search_data.insert_data_item(items[index], right[right_item])
 
         self.recalcR = True
         self.recalcM = True
-        self.iterationsCount = len(items)
-        self.searchData.solution.numberOfGlobalTrials = len(items)
+        self.iterations_count = len(items)
+        self.search_data.solution.number_of_global_trials = len(items)
 
         return items
 
-    def CalculateIterationPoint(self) -> Tuple[SearchDataItem, SearchDataItem]:  # return  (new, old)
+    def calculate_iteration_point(self) -> Tuple[SearchDataItem, SearchDataItem]:  # return  (new, old)
         r"""
         Вычисление точки нового испытания :math:`x^{k+1}`.
 
         :return: :math:`x^{k+1}` - точка нового испытания, и :math:`x_t` - левая точка интервала :math:`[x_{t-1},x_t]`,
           которому принадлежит :math:`x^{k+1}`, т.е. :math:`x^{k+1} \in [x_{t-1},x_t]`.
         """
 
         if self.recalcM is True:
-            self.RecalcM()
+            self.recalc_m()
         if self.recalcR is True:
-            self.RecalcAllCharacteristics()
+            self.recalc_all_characteristics()
 
-        old = self.searchData.GetDataItemWithMaxGlobalR()
+        old = self.search_data.get_data_item_with_max_global_r()
         self.min_delta = min(old.delta, self.min_delta)
-        newx = self.CalculateNextPointCoordinate(old)
-        newy = self.evolvent.GetImage(newx - math.modf(newx)[1])
-        new = copy.deepcopy(SearchDataItem(Point(newy, old.point.discreteVariables),
-                                           newx, discreteValueIndex=old.GetDiscreteValueIndex(),
-                                           functionValues=[FunctionValue()] * self.numberOfAllFunctions))
+        newx = self.calculate_next_point_coordinate(old)
+        newy = self.evolvent.get_image(newx - math.modf(newx)[1])
+        new = copy.deepcopy(SearchDataItem(Point(newy, old.point.discrete_variables),
+                                           newx, discrete_value_index=old.get_discrete_value_index(),
+                                           function_values=[FunctionValue()] * self.numberOfAllFunctions))
         # Обновление числа испытаний
-        self.searchData.solution.numberOfGlobalTrials += 1
+        self.search_data.solution.number_of_global_trials += 1
 
         return new, old
 
     @staticmethod
     def GetDiscreteParameters(problem: Problem) -> list:
-        list_discreteValues = list(problem.discreteVariableValues)
-        return list(itertools.product(*list_discreteValues))
+        list_discrete_values = list(problem.discrete_variable_values)
+        return list(itertools.product(*list_discrete_values))
 
-    def CalculateM(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
+    def calculate_m(self, curr_point: SearchDataItem, left_point: SearchDataItem) -> None:
         r"""
         Вычисление оценки константы Гельдера между между curr_point и left_point.
 
         :param curr_point: правая точка интервала
         :param left_point: левая точка интервала
         """
         # Обратить внимание на вычисление расстояния, должен использоваться метод CalculateDelta
         if curr_point is None:
             print("CalculateM: curr_point is None")
             raise RuntimeError("CalculateM: curr_point is None")
         if left_point is None:
             return
-        index = curr_point.GetIndex()
+        index = curr_point.get_index()
         if index < 0:
             return
         m = 0.0
-        if left_point.GetIndex() == index:  # А если не равны, то надо искать ближайший левый/правый с таким индексом
-            m = abs(left_point.GetZ() - curr_point.GetZ()) / curr_point.delta
+        if left_point.get_index() == index:  # А если не равны, то надо искать ближайший левый/правый с таким индексом
+            m = abs(left_point.get_z() - curr_point.get_z()) / curr_point.delta
         else:
             # Ищем слева
             other_point = left_point
-            while (other_point is not None) and (other_point.GetIndex() < curr_point.GetIndex()):
-                if other_point.GetDiscreteValueIndex() == curr_point.GetDiscreteValueIndex():
-                    other_point = other_point.GetLeft()
+            while (other_point is not None) and (other_point.get_index() < curr_point.get_index()):
+                if other_point.get_discrete_value_index() == curr_point.get_discrete_value_index():
+                    other_point = other_point.get_left()
                 else:
                     other_point = None
                     break
-            if other_point is not None and other_point.GetIndex() >= 0:
+            if other_point is not None and other_point.get_index() >= 0 \
+                    and other_point.get_discrete_value_index() == curr_point.get_discrete_value_index():
                 # print(index)
-                m = abs(other_point.functionValues[index].value - curr_point.GetZ()) / \
-                    self.CalculateDelta(other_point, curr_point, self.dimension)
+                m = abs(other_point.function_values[index].value - curr_point.get_z()) / \
+                    self.calculate_delta(other_point, curr_point, self.dimension)
 
             # Ищем справа
-            other_point = left_point.GetRight()
+            other_point = left_point.get_right()
             if other_point is not None and other_point is curr_point:  # возможно только при пересчёте M
-                other_point = other_point.GetRight()
-            while (other_point is not None) and (other_point.GetIndex() < curr_point.GetIndex()):
-                if other_point.GetDiscreteValueIndex() == curr_point.GetDiscreteValueIndex():
-                    other_point = other_point.GetRight()
+                other_point = other_point.get_right()
+            while (other_point is not None) and (other_point.get_index() < curr_point.get_index()):
+                if other_point.get_discrete_value_index() == curr_point.get_discrete_value_index():
+                    other_point = other_point.get_right()
                 else:
                     other_point = None
                     break
 
-            if other_point is not None and other_point.GetIndex() >= 0:
-                m = max(m, abs(curr_point.GetZ() - other_point.functionValues[index].value) / \
-                        self.CalculateDelta(curr_point, other_point, self.dimension))
+            if other_point is not None and other_point.get_index() >= 0 \
+                    and other_point.get_discrete_value_index() == curr_point.get_discrete_value_index():
+                m = max(m, abs(curr_point.get_z() - other_point.function_values[index].value) / \
+                        self.calculate_delta(curr_point, other_point, self.dimension))
 
         if m > self.M[index] or (self.M[index] == 1.0 and m > 1e-12):
             self.M[index] = m
             self.recalcR = True
```

### Comparing `iOpt-0.2.1/iOpt/method/optim_task.py` & `iOpt-0.2.22/iOpt/method/optim_task.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,28 +15,29 @@
     def __init__(self,
                  problem: Problem,
                  perm: np.ndarray(shape=(1), dtype=int) = None
                  ):
         self.problem = problem
 
         if perm is None:
-            self.perm = np.ndarray(shape=(self.problem.numberOfObjectives + self.problem.numberOfConstraints),
+            self.perm = np.ndarray(shape=(self.problem.number_of_objectives +
+                                          self.problem.number_of_constraints),
                                    dtype=int)
             for i in range(self.perm.size):
                 self.perm[i] = i
         else:
             self.perm = perm
 
-    def Calculate(self,
-                  dataItem: SearchDataItem,
-                  functionIndex: int,
-                  type: TypeOfCalculation = TypeOfCalculation.FUNCTION
+    def calculate(self,
+                  data_item: SearchDataItem,
+                  function_index: int,
+                  calculation_type: TypeOfCalculation = TypeOfCalculation.FUNCTION
                   ) -> SearchDataItem:
         """Compute selected function by number."""
         # ???
-        dataItem.functionValues[self.perm[functionIndex]] = self.problem.Calculate(dataItem.point,
-                                                                                   dataItem.functionValues[
-                                                                                       self.perm[functionIndex]])
-        if not(np.isfinite(dataItem.functionValues[self.perm[functionIndex]].value)):
+        data_item.function_values[self.perm[function_index]] = self.problem.calculate(data_item.point,
+                                                                                      data_item.function_values[
+                                                                                          self.perm[function_index]])
+        if not np.isfinite(data_item.function_values[self.perm[function_index]].value):
             raise Exception("Infinity values")
 
-        return dataItem
+        return data_item
```

### Comparing `iOpt-0.2.1/iOpt/method/parallel_process.py` & `iOpt-0.2.22/iOpt/method/solverFactory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 from typing import List
 
 from iOpt.evolvent.evolvent import Evolvent
-from iOpt.method.calculator import Calculator
+from iOpt.method.index_method import IndexMethod
 from iOpt.method.listener import Listener
 from iOpt.method.method import Method
-from iOpt.method.index_method_calculator import IndexMethodCalculator
+from iOpt.method.mixed_integer_method import MixedIntegerMethod
 from iOpt.method.optim_task import OptimizationTask
+from iOpt.method.parallel_process import ParallelProcess
 from iOpt.method.process import Process
-from iOpt.method.search_data import SearchData, SearchDataItem
+from iOpt.method.search_data import SearchData
 from iOpt.solver_parametrs import SolverParameters
 
 
-class ParallelProcess(Process):
+class SolverFactory:
     """
-    Класс ParallelProcess реализует распараллеливание на уровне потоков (процессов python).
+    Класс SolverFactory создает подходящие классы метода решения и процесса по заданным параметрам
     """
 
-    def __init__(self,
-                 parameters: SolverParameters,
-                 task: OptimizationTask,
-                 evolvent: Evolvent,
-                 searchData: SearchData,
-                 method: Method,
-                 listeners: List[Listener]
-                 ):
+    def __init__(self):
+        pass
+
+    @staticmethod
+    def create_method(parameters: SolverParameters,
+                      task: OptimizationTask,
+                      evolvent: Evolvent,
+                      search_data: SearchData) -> Method:
+        """
+        Создает подходящий класс метода решения по заданным параметрам
+
+        :param parameters: параметры решения задачи оптимизации.
+        :param task: обёртка решаемой задачи.
+        :param evolvent: развертка Пеано-Гильберта, отображающая отрезок [0,1] на многомерную область D.
+        :param search_data: структура данных для хранения накопленной поисковой информации.
+
+        :return: созданный метод
+        """
+
+        if task.problem.number_of_discrete_variables > 0:
+            return MixedIntegerMethod(parameters, task, evolvent, search_data)
+        elif task.problem.number_of_constraints > 0:
+            return IndexMethod(parameters, task, evolvent, search_data)
+        else:
+            return Method(parameters, task, evolvent, search_data)
+
+    @staticmethod
+    def create_process(parameters: SolverParameters,
+                       task: OptimizationTask,
+                       evolvent: Evolvent,
+                       search_data: SearchData,
+                       method: Method,
+                       listeners: List[Listener]) -> Process:
         """
-        Конструктор класса ParallelProcess
+        Создает подходящий класс процесса по заданным параметрам
 
         :param parameters: Параметры решения задачи оптимизации.
         :param task: Обёртка решаемой задачи.
         :param evolvent: Развертка Пеано-Гильберта, отображающая отрезок [0,1] на многомерную область D.
-        :param searchData: Структура данных для хранения накопленной поисковой информации.
+        :param search_data: Структура данных для хранения накопленной поисковой информации.
         :param method: Метод оптимизации, проводящий поисковые испытания по заданным правилам.
         :param listeners: Список "наблюдателей" (используется для вывода текущей информации).
-        """
-        super(ParallelProcess, self).__init__(parameters, task, evolvent, searchData, method, listeners)
-
-        self.indexMethodCalculator = IndexMethodCalculator(task)
-        self.calculator = Calculator(self.indexMethodCalculator, parameters)
 
-    def DoGlobalIteration(self, number: int = 1):
+        :return: созданный процесс
         """
-        Метод позволяет выполнить несколько итераций глобального поиска
-
-        :param number: Количество итераций глобального поиска
-        """
-        number_ = number
-        doneTrials = []
-        if self._first_iteration is True:
-            for listener in self._listeners:
-                listener.BeforeMethodStart(self.method)
-            doneTrials = self.method.FirstIteration(self.calculator)
-            self._first_iteration = False
-            number = number - 1
-
-        for _ in range(number):
-            list_newpoint: list[SearchDataItem] = []
-            list_oldpoint: list[SearchDataItem] = []
-
-            for _ in range(self.parameters.numberOfParallelPoints):
-                newpoint, oldpoint = self.method.CalculateIterationPoint()
-                list_newpoint.append(newpoint)
-                list_oldpoint.append(oldpoint)
-            self.calculator.CalculateFunctionalsForItems(list_newpoint)
-
-            for newpoint, oldpoint in zip(list_newpoint, list_oldpoint):
-                self.method.UpdateOptimum(newpoint)
-                self.method.RenewSearchData(newpoint, oldpoint)
-                self.method.FinalizeIteration()
-                doneTrials = self.searchData.GetLastItems(self.parameters.numberOfParallelPoints * number_)
-
-        for listener in self._listeners:
-            listener.OnEndIteration(doneTrials, self.GetResults())
+        if parameters.number_of_parallel_points == 1:
+            return Process(parameters=parameters, task=task, evolvent=evolvent,
+                           search_data=search_data, method=method, listeners=listeners)
+        else:
+            return ParallelProcess(parameters=parameters, task=task, evolvent=evolvent,
+                                   search_data=search_data, method=method, listeners=listeners)
```

### Comparing `iOpt-0.2.1/iOpt/method/process.py` & `iOpt-0.2.22/iOpt/method/process.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import sys
 from datetime import datetime
 from typing import List
 
 import traceback
 
-import scipy
-from scipy.optimize import Bounds
-
 from iOpt.evolvent.evolvent import Evolvent
 from iOpt.method.listener import Listener
+from iOpt.method.local_optimizer import local_optimize
 from iOpt.method.method import Method
 from iOpt.method.optim_task import OptimizationTask
 from iOpt.method.search_data import SearchData, SearchDataItem
 from iOpt.solution import Solution
 from iOpt.solver_parametrs import SolverParameters
 from iOpt.trial import FunctionValue, FunctionType
 from iOpt.trial import Point
@@ -23,203 +21,185 @@
     Класс Process скрывает внутреннюю имплементацию класса Solver.
     """
 
     def __init__(self,
                  parameters: SolverParameters,
                  task: OptimizationTask,
                  evolvent: Evolvent,
-                 searchData: SearchData,
+                 search_data: SearchData,
                  method: Method,
                  listeners: List[Listener]
                  ):
         """
         Конструктор класса Process
 
         :param parameters: Параметры решения задачи оптимизации.
         :param task: Обёртка решаемой задачи.
         :param evolvent: Развертка Пеано-Гильберта, отображающая отрезок [0,1] на многомерную область D.
-        :param searchData: Структура данных для хранения накопленной поисковой информации.
+        :param search_data: Структура данных для хранения накопленной поисковой информации.
         :param method: Метод оптимизации, проводящий поисковые испытания по заданным правилам.
         :param listeners: Список "наблюдателей" (используется для вывода текущей информации).
         """
         self.parameters = parameters
         self.task = task
         self.evolvent = evolvent
-        self.searchData = searchData
+        self.search_data = search_data
         self.method = method
         self._listeners = listeners
         self._first_iteration = True
 
-    def Solve(self) -> Solution:
+    def solve(self) -> Solution:
         """
         Метод позволяет решить задачу оптимизации. Остановка поиска выполняется согласно критерию,
         заданному при создании класса Solver.
 
         :return: Текущая оценка решения задачи оптимизации
         """
 
-        startTime = datetime.now()
+        start_time = datetime.now()
 
         try:
-            while not self.method.CheckStopCondition():
-                self.DoGlobalIteration()
+            while not self.method.check_stop_condition():
+                self.do_global_iteration()
 
         except Exception:
             print('Exception was thrown')
             print(traceback.format_exc())
 
-        if self.parameters.refineSolution:
-            self.DoLocalRefinement(self.parameters.localMethodIterationCount)
+        if self.parameters.refine_solution:
+            self.do_local_refinement(self.parameters.local_method_iteration_count)
 
-        result = self.GetResults()
-        result.solvingTime = (datetime.now() - startTime).total_seconds()
+        result = self.get_results()
+        result.solving_time = (datetime.now() - start_time).total_seconds()
 
         for listener in self._listeners:
-            status = self.method.CheckStopCondition()
-            listener.OnMethodStop(self.searchData, self.GetResults(), status)
+            status = self.method.check_stop_condition()
+            listener.on_method_stop(self.search_data, self.get_results(), status)
 
         return result
 
-    def DoGlobalIteration(self, number: int = 1):
+    def do_global_iteration(self, number: int = 1):
         """
         Метод позволяет выполнить несколько итераций глобального поиска
 
         :param number: Количество итераций глобального поиска
         """
         number_ = number
-        doneTrials = []
+        done_trials = []
         if self._first_iteration is True:
             for listener in self._listeners:
-                listener.BeforeMethodStart(self.method)
-            doneTrials = self.method.FirstIteration()
+                listener.before_method_start(self.method)
+            done_trials = self.method.first_iteration()
             self._first_iteration = False
-            number = number - 1
+            number -= 1
 
         for _ in range(number):
-            newpoint, oldpoint = self.method.CalculateIterationPoint()
-            self.method.CalculateFunctionals(newpoint)
-            self.method.UpdateOptimum(newpoint)
-            self.method.RenewSearchData(newpoint, oldpoint)
-            self.method.FinalizeIteration()
-            doneTrials = self.searchData.GetLastItems(self.parameters.numberOfParallelPoints * number_)
+            newpoint, oldpoint = self.method.calculate_iteration_point()
+            self.method.calculate_functionals(newpoint)
+            self.method.update_optimum(newpoint)
+            self.method.renew_search_data(newpoint, oldpoint)
+            self.method.finalize_iteration()
+            done_trials = self.search_data.get_last_items(self.parameters.number_of_parallel_points * number_)
 
         for listener in self._listeners:
-            listener.OnEndIteration(doneTrials, self.GetResults())
-
-    def problemCalculate(self, y):
-        result = self.GetResults()
-        point = Point(y, result.bestTrials[0].point.discreteVariables)
-        functionValue = FunctionValue(FunctionType.OBJECTIV)
-
-        for i in range(self.task.problem.dimension):
-            if (y[i] < self.task.problem.lowerBoundOfFloatVariables[i]) \
-                    or (y[i] > self.task.problem.upperBoundOfFloatVariables[i]):
-                functionValue.value = sys.float_info.max
-                return functionValue.value
-
-        try:
-            for i in range(self.task.problem.numberOfConstraints):
-                functionConstraintValue = FunctionValue(FunctionType.CONSTRAINT, i)
-                functionConstraintValue = self.task.problem.Calculate(point, functionConstraintValue)
-                if functionConstraintValue.value > 0:
-                    functionValue.value = sys.float_info.max
-                    return functionValue.value
+            listener.on_end_iteration(done_trials, self.get_results())
 
-            functionValue = self.task.problem.Calculate(point, functionValue)
-        except Exception:
-            functionValue.value = sys.float_info.max
-
-        return functionValue.value
-
-    def DoLocalRefinement(self, number: int = 1):
+    def do_local_refinement(self, number: int = 1):
         """
         Метод позволяет выполнить несколько итераций локального поиска
 
         :param number: Количество итераций локального поиска
         """
         try:
-            localMethodIterationCount = number
+            local_method_iteration_count = number
             if number == -1:
-                localMethodIterationCount = self.parameters.localMethodIterationCount
-
-            result = self.GetResults()
-            startPoint = result.bestTrials[0].point.floatVariables
+                local_method_iteration_count = int(self.parameters.local_method_iteration_count)
 
-            nelder_mead = scipy.optimize.minimize(self.problemCalculate, x0=startPoint, method='Nelder-Mead',
-                                                  options={'maxiter': localMethodIterationCount})
+            result = self.get_results()
+            # start_point = result.bestTrials[0].point.floatVariables
 
-            if localMethodIterationCount > 0:
-                result.bestTrials[0].point.floatVariables = nelder_mead.x
-
-                point: SearchDataItem = SearchDataItem(result.bestTrials[0].point,
-                                                       self.evolvent.GetInverseImage(
-                                                           result.bestTrials[0].point.floatVariables),
-                                                       functionValues=[FunctionValue()] *
-                                                                      (self.task.problem.numberOfConstraints +
-                                                                       self.task.problem.numberOfObjectives)
+            local_solution = local_optimize(self.task,
+                                            method="Hooke-Jeeves", start_point=result.best_trials[0].point,
+                                            max_calcs=local_method_iteration_count,
+                                            args={"eps": self.parameters.eps / 100, "step_mult": 2,
+                                                  "max_iter": local_method_iteration_count}
+                                            )
+            # scipy.optimize.minimize(self.problemCalculate, x0=start_point, method='Nelder-Mead',
+            #                        options={'maxiter': local_method_iteration_count})
+            # local_solution = LocalOptimize(LocalTaskWrapper(self.task, result.bestTrials[0].point.discreteVariables),
+            #                               method="Nelder-Mead", start_point=start_point,
+            #                               args={"options": {'maxiter': local_method_iteration_count}})
+
+            if local_method_iteration_count > 0:
+                result.best_trials[0].point.float_variables = local_solution["x"]
+
+                point: SearchDataItem = SearchDataItem(result.best_trials[0].point,
+                                                       self.evolvent.get_inverse_image(
+                                                           result.best_trials[0].point.float_variables),
+                                                       function_values=[FunctionValue()] *
+                                                                       (self.task.problem.number_of_constraints +
+                                                                        self.task.problem.number_of_objectives)
                                                        )
 
-                number_of_constraints = self.task.problem.numberOfConstraints
+                number_of_constraints = self.task.problem.number_of_constraints
                 for i in range(number_of_constraints):
-                    point.functionValues[i] = FunctionValue(FunctionType.CONSTRAINT, i)
-                    point.functionValues[i] = self.task.problem.Calculate(point.point, point.functionValues[i])
-                    point.SetZ(point.functionValues[i].value)
-                    point.SetIndex(i)
-                    if point.GetZ() > 0:
+                    point.function_values[i] = FunctionValue(FunctionType.CONSTRAINT, i)
+                    point.function_values[i] = self.task.problem.calculate(point.point, point.function_values[i])
+                    point.set_z(point.function_values[i].value)
+                    point.set_index(i)
+                    if point.get_z() > 0:
                         break
-                point.functionValues[number_of_constraints] = FunctionValue(FunctionType.OBJECTIV,
-                                                                            number_of_constraints)
-                point.functionValues[number_of_constraints] = \
-                    self.task.problem.Calculate(point.point, point.functionValues[number_of_constraints])
-                point.SetZ(point.functionValues[number_of_constraints].value)
-                point.SetIndex(number_of_constraints)
+                point.function_values[number_of_constraints] = FunctionValue(FunctionType.OBJECTIV,
+                                                                             number_of_constraints)
+                point.function_values[number_of_constraints] = \
+                    self.task.problem.calculate(point.point, point.function_values[number_of_constraints])
+                point.set_z(point.function_values[number_of_constraints].value)
+                point.set_index(number_of_constraints)
 
-                result.bestTrials[0].functionValues = point.functionValues
+                result.best_trials[0].function_values = point.function_values
 
-            result.numberOfLocalTrials = nelder_mead.nfev
+            result.number_of_local_trials = local_solution["fev"]
         except Exception:
             print("Local Refinement is not possible")
 
-    def GetResults(self) -> Solution:
+    def get_results(self) -> Solution:
         """
         Метод возвращает лучшее найденное решение задачи оптимизации
 
         :return: Решение задачи оптимизации
         """
-        # ДА, ЭТО КОСТЫЛЬ. т.к. solution хранит trial
-        # self.searchData.solution.bestTrials[0] = self.method.GetOptimumEstimation()
-        return self.searchData.solution
+        return self.search_data.solution
 
-    def SaveProgress(self, fileName: str) -> None:
+    def save_progress(self, file_name: str) -> None:
         """
         Сохранение процесса оптимизации из файла
 
-        :param fileName: имя файла
+        :param file_name: имя файла
         """
-        self.searchData.SaveProgress(fileName=fileName)
+        self.search_data.save_progress(file_name=file_name)
 
-    def LoadProgress(self, fileName: str) -> None:
+    def load_progress(self, file_name: str) -> None:
         """
         Загрузка процесса оптимизации из файла
 
-        :param fileName: имя файла
+        :param file_name: имя файла
         """
-        self.searchData.LoadProgress(fileName=fileName)
-        self.method.iterationsCount = self.searchData.GetCount() - 2
+        self.search_data.load_progress(file_name=file_name)
+        self.method.iterations_count = self.search_data.get_count() - 2
 
-        for ditem in self.searchData:
-            if ditem.GetIndex() >= 0:
-                self.method.UpdateOptimum(ditem)
+        for ditem in self.search_data:
+            if ditem.get_index() >= 0:
+                self.method.update_optimum(ditem)
 
-        self.method.RecalcM()
-        self.method.RecalcAllCharacteristics()
+        self.method.recalc_m()
+        self.method.recalc_all_characteristics()
         self._first_iteration = False
 
         for listener in self._listeners:
-            listener.BeforeMethodStart(self.method)
+            listener.before_method_start(self.method)
 
     '''
     def RefreshListener(self):
         pass
 
     def AddListener(self, listener: Listener):
         #self.__listeners.append(listener)
```

### Comparing `iOpt-0.2.1/iOpt/method/search_data.py` & `iOpt-0.2.22/iOpt/method/search_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,136 +21,135 @@
     """
         Класс SearchDataItem предназначен для хранения поисковой информации, представляющей собой
         интервал с включенной правой точкой, а так же ссылками на соседние интервалы. SearchDataItem
         является наследником от класса Trial.
     """
 
     def __init__(self, y: Point, x: np.double,
-                 functionValues: np.ndarray(shape=(1), dtype=FunctionValue) = [FunctionValue()],
-                 discreteValueIndex: int = 0):
+                 function_values: np.ndarray(shape=(1), dtype=FunctionValue) = [FunctionValue()],
+                 discrete_value_index: int = 0):
         """
         Конструктор класса SearchDataItem
 
         :param y: Точка испытания в исходной N-мерной области поиска
         :param x: Отображении точки испытания y на отрезок [0, 1]
-        :param functionValues: Вектор значений функций (целевой функции и функций ограничений)
-        :param discreteValueIndex: Дискретный параметр
+        :param function_values: Вектор значений функций (целевой функции и функций ограничений)
+        :param discrete_value_index: Дискретный параметр
         """
-        super().__init__(point=y, functionValues=copy.deepcopy(functionValues))
+        super().__init__(point=y, function_values=copy.deepcopy(function_values))
         self.point = y
         self.__x = x
-        self.__discreteValueIndex = discreteValueIndex
+        self.__discrete_value_index = discrete_value_index
         self.__index: int = -2
         self.__z: np.double = sys.float_info.max
         self.__leftPoint: SearchDataItem = None
         self.__rightPoint: SearchDataItem = None
         self.delta: np.double = -1.0
         self.globalR: np.double = -1.0
         self.localR: np.double = -1.0
         self.iterationNumber: int = -1
 
-
-    def GetX(self) -> np.double:
+    def get_x(self) -> np.double:
         """
         Метод позволяет получить правую точку поискового интервала, где :math:`x\in[0, 1]`.
 
         :return: Значение правой точки интервала
         """
         return self.__x
 
-    def GetY(self) -> Point:
+    def get_y(self) -> Point:
         """
         Метод позволяет получить N-мерную точку испытания исходной области поиска.
 
         :return: Значение N-мерной точки испытания
         """
         return self.point
 
-    def GetDiscreteValueIndex(self) -> int:
+    def get_discrete_value_index(self) -> int:
         """
         Метод позволяет получить дискретный параметр.
 
         :return: Значение дискретного параметра
         """
-        return self.__discreteValueIndex
+        return self.__discrete_value_index
 
-    def SetIndex(self, index: int):
+    def set_index(self, index: int):
         """
         Метод позволяет задать значение индекса последнего выполненного ограничения
         для индексной схемы.
 
         :param index: Индекс ограничения
         """
         self.__index = index
 
-    def GetIndex(self) -> int:
+    def get_index(self) -> int:
         """
         Метод позволяет получить значение индекса последнего выполненного ограничения
         для индексной схемы.
 
         :return: Значение индекса
         """
         return self.__index
 
-    def SetZ(self, z: np.double):
+    def set_z(self, z: np.double):
         """
         Метод позволяет задать значение функции для заданного индекса.
 
         :param z: Значение функции
         """
         self.__z = z
 
-    def GetZ(self) -> np.double:
+    def get_z(self) -> np.double:
         """
         Метод позволяет получить значение функции для заданного индекса.
 
         :return: Значение функции для index
         """
         return self.__z
 
-    def SetLeft(self, point: SearchDataItem):
+    def set_left(self, point: SearchDataItem):
         """
         Метод позволяет задать левый интервал для исходного.
 
         :param point: Левый интервал
         """
         self.__leftPoint = point
 
-    def GetLeft(self) -> SearchDataItem:
+    def get_left(self) -> SearchDataItem:
         """
         Метод позволяет получить левый интервал для исходного.
 
         :return: Значение левого интервала
         """
         return self.__leftPoint
 
-    def SetRight(self, point: SearchDataItem):
+    def set_right(self, point: SearchDataItem):
         """
         Метод позволяет задать правый интервал для исходного.
 
         :param point: Правый интервал
         """
         self.__rightPoint = point
 
-    def GetRight(self) -> SearchDataItem:
+    def get_right(self) -> SearchDataItem:
         """
        Метод позволяет получить правый интервал для исходного.
 
        :return: Значение правого интервала
        """
         return self.__rightPoint
 
     def __lt__(self, other) -> bool:
         """
         Метод переопределяет оператор сравнения < для двух интервалов.
         :param other: Второй интервал
         :return: Значение true - если правая точка исходного интервала меньше
         правой точки второго, иначе - false.
         """
-        return self.GetX() < other.GetX()
+        return self.get_x() < other.get_x()
 
 
 class CharacteristicsQueue:
     """
     Класс CharacteristicsQueue предназначен для хранения приоритетной очереди
     характеристик с вытеснением.
     """
@@ -165,49 +164,49 @@
 
     def Clear(self):
         """
         Метод позволяет очистить очередь
         """
         self.__baseQueue.clear()
 
-    def Insert(self, key: np.double, dataItem: SearchDataItem):
+    def insert(self, key: np.double, data_item: SearchDataItem):
         """
         Метод добавляет поисковый интервал с указанным приоритетом.
         Приоритетом является значение характеристики на данном интервале.
 
         :param key: Приоритет поискового интервала
-        :param dataItem: Вставляемый интервал
+        :param data_item: Вставляемый интервал
         """
-        self.__baseQueue.insert(dataItem, key)
+        self.__baseQueue.insert(data_item, key)
 
-    def GetBestItem(self) -> (SearchDataItem, np.double):
+    def get_best_item(self) -> (SearchDataItem, np.double):
         """
         Метод позволяет получить интервал с лучшей характеристикой
 
         :return: Кортеж: интервал с лучшей характеристикой, приоритет интервала в очереди
         """
         return self.__baseQueue.popfirst()
 
-    def IsEmpty(self):
+    def is_empty(self):
         """
         Метод позволяет сделать проверку на пустоту очереди.
 
         :return: Значение true если очередь пуста, иначе false
         """
         return self.__baseQueue.is_empty()
 
-    def GetMaxLen(self) -> int:
+    def get_max_len(self) -> int:
         """
         Метод позволяет получить максимальный размер очереди.
 
         :return: Значение максимального размера очереди
         """
         return self.__baseQueue.maxlen
 
-    def GetLen(self) -> int:
+    def get_len(self) -> int:
         """
         Метод позволяет получить текущий размер очереди.
 
         :return: Значение текущего размера очереди
         """
         return len(self.__baseQueue)
 
@@ -235,258 +234,258 @@
         :param maxlen: Максимальный размер очереди
         """
         self.solution = Solution(problem)
         self._allTrials = []
         self._RGlobalQueue = CharacteristicsQueue(maxlen)
         self.__firstDataItem: SearchDataItem = None
 
-    def ClearQueue(self):
+    def clear_queue(self):
         """
         Метод позволяет очистить очередь характеристик
         """
         self._RGlobalQueue.Clear()
 
     # вставка точки если знает правую точку
     # в качестве интервала используем [i-1, i]
-    # если rightDataItem == None то его необходимо найти по дереву _allTrials
-    def InsertDataItem(self, newDataItem: SearchDataItem,
-                       rightDataItem: SearchDataItem = None):
+    # если right_data_item == None то его необходимо найти по дереву _allTrials
+    def insert_data_item(self, new_data_item: SearchDataItem,
+                         right_data_item: SearchDataItem = None):
         """
         Метод позволяет добавить новый интервал испытаний в список всех проведенных испытаний
         и приоритетную очередь характеристик.
 
-        :param newDataItem: Новый интервал испытаний
-        :param rightDataItem: Покрывающий интервал, является правым интервалом для newDataItem
+        :param new_data_item: Новый интервал испытаний
+        :param right_data_item: Покрывающий интервал, является правым интервалом для newDataItem
         """
         flag = True
-        if rightDataItem is None:
-            rightDataItem = self.FindDataItemByOneDimensionalPoint(newDataItem.GetX())
+        if right_data_item is None:
+            right_data_item = self.find_data_item_by_one_dimensional_point(new_data_item.get_x())
             flag = False
-        newDataItem.SetLeft(rightDataItem.GetLeft())
-        rightDataItem.SetLeft(newDataItem)
-        newDataItem.SetRight(rightDataItem)
-        newDataItem.GetLeft().SetRight(newDataItem)
+        new_data_item.set_left(right_data_item.get_left())
+        right_data_item.set_left(new_data_item)
+        new_data_item.set_right(right_data_item)
+        new_data_item.get_left().set_right(new_data_item)
 
-        self._allTrials.append(newDataItem)
+        self._allTrials.append(new_data_item)
 
-        self._RGlobalQueue.Insert(newDataItem.globalR, newDataItem)
+        self._RGlobalQueue.insert(new_data_item.globalR, new_data_item)
         if flag:
-            self._RGlobalQueue.Insert(rightDataItem.globalR, rightDataItem)
+            self._RGlobalQueue.insert(right_data_item.globalR, right_data_item)
 
-    def InsertFirstDataItem(self, leftDataItem: SearchDataItem,
-                            rightDataItem: SearchDataItem):
+    def insert_first_data_item(self, left_data_item: SearchDataItem,
+                               right_data_item: SearchDataItem):
         """
         Метод позволяет добавить пару интервалов испытаний на первой итерации AGP.
 
-        :param leftDataItem: Левый интервал для rightDataItem
-        :param rightDataItem: Правый интервал для leftDataItem
+        :param left_data_item: Левый интервал для right_data_item
+        :param right_data_item: Правый интервал для leftDataItem
         """
-        leftDataItem.SetRight(rightDataItem)
-        rightDataItem.SetLeft(leftDataItem)
+        left_data_item.set_right(right_data_item)
+        right_data_item.set_left(left_data_item)
 
-        self._allTrials.append(leftDataItem)
-        self._allTrials.append(rightDataItem)
+        self._allTrials.append(left_data_item)
+        self._allTrials.append(right_data_item)
 
-        self.__firstDataItem = leftDataItem
+        self.__firstDataItem = left_data_item
 
     # поиск покрывающего интервала
     # возвращает правую точку
-    def FindDataItemByOneDimensionalPoint(self, x: np.double) -> SearchDataItem:
+    def find_data_item_by_one_dimensional_point(self, x: np.double) -> SearchDataItem:
         """
         Метод позволяет найти покрывающий интервал для полученной точки x.
 
         :param x: Правая точка интервала
         :return: Правая точка покрывающего интервала
         """
         # итерируемся по rightPoint от минимального элемента
         for item in self:
-            if item.GetX() > x:
+            if item.get_x() > x:
                 return item
         return None
 
-    def GetDataItemWithMaxGlobalR(self) -> SearchDataItem:
+    def get_data_item_with_max_global_r(self) -> SearchDataItem:
         """
         Метод позволяет получить интервал с лучшим значением глобальной характеристики.
 
         :return: Значение интервала с лучшей глобальной характеристикой
         """
-        if self._RGlobalQueue.IsEmpty():
-            self.RefillQueue()
-        return self._RGlobalQueue.GetBestItem()[0]
+        if self._RGlobalQueue.is_empty():
+            self.refill_queue()
+        return self._RGlobalQueue.get_best_item()[0]
 
     # Перезаполнение очереди (при ее опустошении или при смене оценки константы Липшица)
-    def RefillQueue(self):
+    def refill_queue(self):
         """
         Метод позволяет перезаполнить очередь глобальных характеристик, например, при ее опустошении
         или при смене оценки константы Липшица.
 
         """
         self._RGlobalQueue.Clear()
         for itr in self:
-            self._RGlobalQueue.Insert(itr.globalR, itr)
+            self._RGlobalQueue.insert(itr.globalR, itr)
 
     # Возвращает текущее число интервалов в дереве
-    def GetCount(self) -> int:
+    def get_count(self) -> int:
         """
         Метод позволяет получить текущее число интервалов в списке.
 
         :return: Значение числа интервалов в списке
         """
         return len(self._allTrials)
 
-    def GetLastItem(self) -> SearchDataItem:
+    def get_last_item(self) -> SearchDataItem:
         """
         Метод позволяет получить последний добавленный интервал в список.
 
         :return: Значение последнего добавленного интервала
         """
         try:
             return self._allTrials[-1]
         except Exception:
             print("GetLastItem: List is empty")
 
-    def GetLastItems(self, N: int = 1) -> list[SearchDataItem]:
+    def get_last_items(self, N: int = 1) -> list[SearchDataItem]:
         """
         Метод позволяет получить последние добавленные интервалы в список.
 
         :return: Значения последней серии добавленных интервалов
         """
         try:
             return self._allTrials[-N:]
         except Exception:
             print("GetLastItems: List is empty")
 
-    def SaveProgress(self, fileName: str):
+    def save_progress(self, file_name: str):
         """
         Сохранение процесса оптимизации в файл
 
-        :param fileName: имя файла
+        :param file_name: имя файла
         """
         data = {}
         data['SearchDataItem'] = []
         for dataItem in self._allTrials:
 
             fvs = []
-            for fv in dataItem.functionValues:
+            for fv in dataItem.function_values:
                 fvs.append({
                     'value': fv.value,
                     'type': 1 if fv.type == FunctionType.OBJECTIV else 2,
                     'functionID': str(fv.functionID),
                 })
 
             data['SearchDataItem'].append({
-                'floatVariables': list(dataItem.GetY().floatVariables),
-                'discreteVariables': [] if dataItem.GetY().discreteVariables is None else list(
-                    dataItem.GetY().discreteVariables),
-                'functionValues': list(fvs),
-                'x': dataItem.GetX(),
+                'float_variables': list(dataItem.get_y().float_variables),
+                'discrete_variables': [] if dataItem.get_y().discrete_variables is None else list(
+                    dataItem.get_y().discrete_variables),
+                'function_values': list(fvs),
+                'x': dataItem.get_x(),
                 'delta': dataItem.delta,
                 'globalR': dataItem.globalR,
                 'localR': dataItem.localR,
-                'index': dataItem.GetIndex(),
-                'discreteValueIndex': dataItem.GetDiscreteValueIndex(),
-                '__z': dataItem.GetZ()
+                'index': dataItem.get_index(),
+                'discrete_value_index': dataItem.get_discrete_value_index(),
+                '__z': dataItem.get_z()
             })
 
-        data['BestTrials'] = []  # создаем список
-        dataItem = self.solution.bestTrials[0]
+        data['best_trials'] = []  # создаем список
+        dataItem = self.solution.best_trials[0]
         fvs = []  # пустой список для словарей со значениями функций
-        for fv in dataItem.functionValues:
+        for fv in dataItem.function_values:
             fvs.append({
                 'value': fv.value,
                 'type': 1 if fv.type == FunctionType.OBJECTIV else 2,
                 'functionID': str(fv.functionID),
             })
 
-        data['BestTrials'].append({
-            'floatVariables': list(dataItem.GetY().floatVariables),
-            'discreteVariables': [] if dataItem.GetY().discreteVariables is None else list(
-                dataItem.GetY().discreteVariables),
-            'functionValues': list(fvs),
-            'x': dataItem.GetX(),
+        data['best_trials'].append({
+            'float_variables': list(dataItem.get_y().float_variables),
+            'discrete_variables': [] if dataItem.get_y().discrete_variables is None else list(
+                dataItem.get_y().discrete_variables),
+            'function_values': list(fvs),
+            'x': dataItem.get_x(),
             'delta': dataItem.delta,
             'globalR': dataItem.globalR,
             'localR': dataItem.localR,
-            'index': dataItem.GetIndex(),
-            'discreteValueIndex': dataItem.GetDiscreteValueIndex(),
-            '__z': dataItem.GetZ()
+            'index': dataItem.get_index(),
+            'discrete_value_index': dataItem.get_discrete_value_index(),
+            '__z': dataItem.get_z()
         })
 
-        with open(fileName, 'w') as f:
+        with open(file_name, 'w') as f:
             json.dump(data, f, indent='\t', separators=(',', ':'))
 
-    def LoadProgress(self, fileName: str):
+    def load_progress(self, file_name: str):
         """
         Загрузка процесса оптимизации из файла
 
-        :param fileName: имя файла
+        :param file_name: имя файла
         """
 
-        with open(fileName) as json_file:
+        with open(file_name) as json_file:
             data = json.load(json_file)
 
-            functionValues = []
-            for p in data['BestTrials']:
+            function_values = []
+            for p in data['best_trials']:
 
-                for fv in p['functionValues']:
-                    functionValues.append(FunctionValue(
+                for fv in p['function_values']:
+                    function_values.append(FunctionValue(
                         (FunctionType.OBJECTIV if fv['type'] == 1 else FunctionType.CONSTRAINT),
                         str(fv['functionID'])))
-                    functionValues[-1].value = np.double(fv['value'])
+                    function_values[-1].value = np.double(fv['value'])
 
-                dataItem = SearchDataItem(Point(p['floatVariables'], p['discreteVariables']), p['x'], functionValues,
-                                          p['discreteValueIndex'])
-                dataItem.delta = p['delta']  # [-1] - обращение к последнему элементу
-                dataItem.globalR = p['globalR']
-                dataItem.localR = p['localR']
-                dataItem.SetZ(p['__z'])
-                dataItem.SetIndex(p['index'])
+                data_item = SearchDataItem(Point(p['float_variables'], p['discrete_variables']), p['x'],
+                                           function_values,
+                                           p['discrete_value_index'])
+                data_item.delta = p['delta']  # [-1] - обращение к последнему элементу
+                data_item.globalR = p['globalR']
+                data_item.localR = p['localR']
+                data_item.set_z(p['__z'])
+                data_item.set_index(p['index'])
 
-                self.solution.bestTrials[0] = dataItem
+                self.solution.best_trials[0] = data_item
 
-            firstDataItem = []
+            first_data_item = []
 
             for p in data['SearchDataItem'][:2]:
-                functionValues = []
+                function_values = []
 
-                for fv in p['functionValues']:
-                    functionValues.append(FunctionValue(
+                for fv in p['function_values']:
+                    function_values.append(FunctionValue(
                         (FunctionType.OBJECTIV if fv['type'] == 1 else FunctionType.CONSTRAINT),
                         str(fv['functionID'])))
-                    functionValues[-1].value = np.double(fv['value'])
+                    function_values[-1].value = np.double(fv['value'])
 
-                firstDataItem.append(
-                    SearchDataItem(Point(p['floatVariables'], p['discreteVariables']), p['x'], functionValues,
-                                   p['discreteValueIndex']))
-                firstDataItem[-1].delta = p['delta']
-                firstDataItem[-1].globalR = p['globalR']
-                firstDataItem[-1].localR = p['localR']
-                firstDataItem[-1].SetIndex(p['index'])
+                first_data_item.append(
+                    SearchDataItem(Point(p['float_variables'], p['discrete_variables']), p['x'], function_values,
+                                   p['discrete_value_index']))
+                first_data_item[-1].delta = p['delta']
+                first_data_item[-1].globalR = p['globalR']
+                first_data_item[-1].localR = p['localR']
+                first_data_item[-1].set_index(p['index'])
 
-            self.InsertFirstDataItem(firstDataItem[0], firstDataItem[1])
+            self.insert_first_data_item(first_data_item[0], first_data_item[1])
 
             for p in data['SearchDataItem'][2:]:
-                functionValues = []
+                function_values = []
 
-                for fv in p['functionValues']:
-                    functionValues.append(FunctionValue(
+                for fv in p['function_values']:
+                    function_values.append(FunctionValue(
                         (FunctionType.OBJECTIV if fv['type'] == 1 else FunctionType.CONSTRAINT),
                         str(fv['functionID'])))
-                    functionValues[-1].value = np.double(fv['value'])
-
-                dataItem = SearchDataItem(Point(p['floatVariables'], p['discreteVariables']), p['x'], functionValues,
-                                          p['discreteValueIndex'])
-                dataItem.delta = p['delta']
-                dataItem.globalR = p['globalR']
-                dataItem.localR = p['localR']
-                dataItem.SetZ(p['__z'])
-                dataItem.SetIndex(p['index'])
+                    function_values[-1].value = np.double(fv['value'])
 
-                self.InsertDataItem(dataItem)
+                data_item = SearchDataItem(Point(p['float_variables'], p['discrete_variables']),
+                                           p['x'], function_values, p['discrete_value_index'])
+                data_item.delta = p['delta']
+                data_item.globalR = p['globalR']
+                data_item.localR = p['localR']
+                data_item.set_z(p['__z'])
+                data_item.set_index(p['index'])
 
+                self.insert_data_item(data_item)
 
     def __iter__(self):
         # вернуть самую левую точку из дерева (ниже код проверить!)
         # return self._allTrials.min_item()[1]
         self.curIter = self.__firstDataItem
         if self.curIter is None:
             raise StopIteration
@@ -494,15 +493,15 @@
             return self
 
     def __next__(self):
         if self.curIter is None:
             raise StopIteration
         else:
             tmp = self.curIter
-            self.curIter = self.curIter.GetRight()
+            self.curIter = self.curIter.get_right()
             return tmp
 
 
 class SearchDataDualQueue(SearchData):
     """
     Класс SearchDataDualQueue является наследником класса SearchData. Предназначен
       для хранения множества всех интервалов, исходной задачи и двух приоритетных очередей
@@ -516,81 +515,81 @@
 
         :param problem: Информация об исходной задаче
         :param maxlen: Максимальный размер очереди
         """
         super().__init__(problem, maxlen)
         self.__RLocalQueue = CharacteristicsQueue(maxlen)
 
-    def ClearQueue(self):
+    def clear_queue(self):
         """
         Метод позволяет очистить очереди характеристик
         """
         self._RGlobalQueue.Clear()
         self.__RLocalQueue.Clear()
 
-    def InsertDataItem(self, newDataItem: SearchDataItem,
-                       rightDataItem: SearchDataItem = None):
+    def insert_data_item(self, new_data_item: SearchDataItem,
+                         right_data_item: SearchDataItem = None):
         """
         Метод позволяет добавить новый интервал испытаний в список всех проведенных испытаний
           и приоритетные очереди глобальных и локальных характеристик.
 
-        :param newDataItem: Новый интервал испытаний
-        :param rightDataItem: Покрывающий интервал, является правым интервалом для newDataItem
+        :param new_data_item: Новый интервал испытаний
+        :param right_data_item: Покрывающий интервал, является правым интервалом для newDataItem
         """
         flag = True
-        if rightDataItem is None:
-            rightDataItem = self.FindDataItemByOneDimensionalPoint(newDataItem.GetX())
+        if right_data_item is None:
+            right_data_item = self.find_data_item_by_one_dimensional_point(new_data_item.get_x())
             flag = False
 
-        newDataItem.SetLeft(rightDataItem.GetLeft())
-        rightDataItem.SetLeft(newDataItem)
-        newDataItem.SetRight(rightDataItem)
-        newDataItem.GetLeft().SetRight(newDataItem)
+        new_data_item.set_left(right_data_item.get_left())
+        right_data_item.set_left(new_data_item)
+        new_data_item.set_right(right_data_item)
+        new_data_item.get_left().set_right(new_data_item)
 
-        self._allTrials.append(newDataItem)
+        self._allTrials.append(new_data_item)
 
-        self._RGlobalQueue.Insert(newDataItem.globalR, newDataItem)
-        self.__RLocalQueue.Insert(newDataItem.localR, newDataItem)
+        self._RGlobalQueue.insert(new_data_item.globalR, new_data_item)
+        self.__RLocalQueue.insert(new_data_item.localR, new_data_item)
         if flag:
-            self._RGlobalQueue.Insert(rightDataItem.globalR, rightDataItem)
-            self.__RLocalQueue.Insert(rightDataItem.localR, rightDataItem)
+            self._RGlobalQueue.insert(right_data_item.globalR, right_data_item)
+            self.__RLocalQueue.insert(right_data_item.localR, right_data_item)
 
-    def GetDataItemWithMaxGlobalR(self) -> SearchDataItem:
+    def get_data_item_with_max_global_r(self) -> SearchDataItem:
         """
        Метод позволяет получить интервал с лучшим значением глобальной характеристики.
 
        :return: Значение интервала с лучшей глобальной характеристикой
        """
-        if self._RGlobalQueue.IsEmpty():
-            self.RefillQueue()
-        bestItem = self._RGlobalQueue.GetBestItem()
-        while bestItem[1] != bestItem[0].globalR:
-            if self._RGlobalQueue.IsEmpty():
-                self.RefillQueue()
-            bestItem = self._RGlobalQueue.GetBestItem()
-        return bestItem[0]
+        if self._RGlobalQueue.is_empty():
+            self.refill_queue()
+        best_item = self._RGlobalQueue.get_best_item()
+        while best_item[1] != best_item[0].globalR:
+            if self._RGlobalQueue.is_empty():
+                self.refill_queue()
+            best_item = self._RGlobalQueue.get_best_item()
+        return best_item[0]
 
-    def GetDataItemWithMaxLocalR(self) -> SearchDataItem:
+    def get_data_item_with_max_local_r(self) -> SearchDataItem:
         """
        Метод позволяет получить интервал с лучшим значением локальной характеристики.
 
        :return: Значение интервала с лучшей локальной характеристикой
        """
-        if self.__RLocalQueue.IsEmpty():
-            self.RefillQueue()
-        bestItem = self.__RLocalQueue.GetBestItem()
-        while bestItem[1] != bestItem[0].localR:
-            if self.__RLocalQueue.IsEmpty():
-                self.RefillQueue()
-            bestItem = self.__RLocalQueue.GetBestItem()
-        return bestItem[0]
+        if self.__RLocalQueue.is_empty():
+            self.refill_queue()
+        best_item = self.__RLocalQueue.get_best_item()
+        while best_item[1] != best_item[0].localR:
+            if self.__RLocalQueue.is_empty():
+                self.refill_queue()
+            best_item = self.__RLocalQueue.get_best_item()
+        return best_item[0]
 
-    def RefillQueue(self):
+    def refill_queue(self):
         """
        Метод позволяет перезаполнить очереди глобальных и локальных характеристик, например,
          при их опустошении или при смене оценки константы Липшица.
 
        """
-        self.ClearQueue()
+        self.clear_queue()
         for itr in self:
-            self._RGlobalQueue.Insert(itr.globalR, itr)
-            self.__RLocalQueue.Insert(itr.localR, itr)
+            self._RGlobalQueue.insert(itr.globalR, itr)
+            self.__RLocalQueue.insert(itr.localR, itr)
```

### Comparing `iOpt-0.2.1/iOpt/output_system/listeners/animate_painters.py` & `iOpt-0.2.22/iOpt/output_system/listeners/animate_painters.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,76 +3,78 @@
 from iOpt.solution import Solution
 from iOpt.method.method import Method
 
 from iOpt.output_system.painters.animate_painters import AnimatePainter, AnimatePainterND
 
 import numpy as np
 
+
 class AnimatePainterListener(Listener):
     """
     Класс AnimationPaintListener - слушатель событий. Содержит методы-обработчики, выдающие в качестве
       реакции на события динамически обновляющееся изображение процесса оптимизации.
       Используется для одномерной оптимизации.
     """
 
-    def __init__(self, fileName: str, pathForSaves="", isPointsAtBottom=False, toPaintObjFunc=True):
+    def __init__(self, file_name: str, path_for_saves="", is_points_at_bottom=False, to_paint_obj_func=True):
         """
         Конструктор класса AnimationPaintListener
 
-        :param fileName: Название файла с указанием формата для сохранения изображения. Обязательный параметр.
-        :param pathForSaves: Директория для сохранения изображения. В случае, если параметр не указан, изображение
+        :param file_name: Название файла с указанием формата для сохранения изображения. Обязательный параметр.
+        :param path_for_saves: Директория для сохранения изображения. В случае, если параметр не указан, изображение
            сохраняется в текущей рабочей директории.
-        :param isPointsAtBottom: Должны ли точки поисковой информации ставиться под графиком или нет. Если False,
+        :param is_points_at_bottom: Должны ли точки поисковой информации ставиться под графиком или нет. Если False,
            точки ставятся на графике.
-        :param toPaintObjFunc: Должна ли отрисовываться целевая функция или нет.
+        :param to_paint_obj_func: Должна ли отрисовываться целевая функция или нет.
         """
-        self.fileName = fileName
-        self.pathForSaves = pathForSaves
-        self.isPointsAtBottom = isPointsAtBottom
-        self.toPaintObjFunc = toPaintObjFunc
-        self.__painter = AnimatePainter(self.isPointsAtBottom, 0, self.pathForSaves, self.fileName)
-
-    def BeforeMethodStart(self, method: Method):
-        self.__painter.SetProblem(method.task.problem)
-        if self.toPaintObjFunc:
-            self.__painter.PaintObjectiveFunc()
-
-    def OnEndIteration(self, savedNewPoints : np.ndarray(shape=(1), dtype=SearchDataItem), solution: Solution):
-        self.__painter.PaintPoints(savedNewPoints)
-
-    def OnMethodStop(self, searchData: SearchData, solution: Solution, status: bool):
-        self.__painter.PaintOptimum(solution)
-        self.__painter.SaveImage()
+        self.file_name = file_name
+        self.path_for_saves = path_for_saves
+        self.is_points_at_bottom = is_points_at_bottom
+        self.to_paint_obj_func = to_paint_obj_func
+        self.__painter = AnimatePainter(self.is_points_at_bottom, 0, self.path_for_saves, self.file_name)
+
+    def before_method_start(self, method: Method):
+        self.__painter.set_problem(method.task.problem)
+        if self.to_paint_obj_func:
+            self.__painter.paint_objective_func()
+
+    def on_end_iteration(self, saved_new_points: np.ndarray(shape=(1), dtype=SearchDataItem), solution: Solution):
+        self.__painter.paint_points(saved_new_points)
+
+    def on_method_stop(self, search_data: SearchData, solution: Solution, status: bool):
+        self.__painter.paint_optimum(solution)
+        self.__painter.save_image()
+
 
 class AnimatePainterNDListener(Listener):
     """
     Класс AnimationPaintListener - слушатель событий. Содержит методы-обработчики, выдающие в качестве
       реакции на события динамически обновляющееся изображение процесса оптимизации.
       Используется для многомерной оптимизации.
     """
 
-    def __init__(self, fileName: str, pathForSaves="", varsIndxs=[0, 1], toPaintObjFunc=True):
+    def __init__(self, file_name: str, path_for_saves="", vars_indxs=[0, 1], to_paint_obj_func=True):
         """
         Конструктор класса AnimationNDPaintListener
 
-        :param fileName: Название файла с указанием формата для сохранения изображения. Обязательный параметр.
-        :param pathForSaves: Директория для сохранения изображения. В случае, если параметр не указан, изображение
+        :param file_name: Название файла с указанием формата для сохранения изображения. Обязательный параметр.
+        :param path_for_saves: Директория для сохранения изображения. В случае, если параметр не указан, изображение
            сохраняется в текущей рабочей директории.
-        :param varsIndxs: Пара индексов переменных оптимизационной задачи, для которых будет построен рисунок.
-        :param toPaintObjFunc: Должна ли отрисовываться целевая функция или нет.
+        :param vars_indxs: Пара индексов переменных оптимизационной задачи, для которых будет построен рисунок.
+        :param to_paint_obj_func: Должна ли отрисовываться целевая функция или нет.
         """
-        self.fileName = fileName
-        self.pathForSaves = pathForSaves
-        self.toPaintObjFunc = toPaintObjFunc
-        self.__painter = AnimatePainterND(varsIndxs, self.pathForSaves, self.fileName)
-
-    def BeforeMethodStart(self, method: Method):
-        self.__painter.SetProblem(method.task.problem)
-
-    def OnEndIteration(self, savedNewPoints : np.ndarray(shape=(1), dtype=SearchDataItem), solution: Solution):
-        self.__painter.PaintPoints(savedNewPoints)
-
-    def OnMethodStop(self, searchData: SearchData, solution: Solution, status: bool):
-        self.__painter.PaintOptimum(solution)
-        if self.toPaintObjFunc:
-            self.__painter.PaintObjectiveFunc()
-        self.__painter.SaveImage()
+        self.file_name = file_name
+        self.path_for_saves = path_for_saves
+        self.to_paint_obj_func = to_paint_obj_func
+        self.__painter = AnimatePainterND(vars_indxs, self.path_for_saves, self.file_name)
+
+    def before_method_start(self, method: Method):
+        self.__painter.set_problem(method.task.problem)
+
+    def on_end_iteration(self, saved_new_points: np.ndarray(shape=(1), dtype=SearchDataItem), solution: Solution):
+        self.__painter.paint_points(saved_new_points)
+
+    def on_method_stop(self, search_data: SearchData, solution: Solution, status: bool):
+        self.__painter.paint_optimum(solution)
+        if self.to_paint_obj_func:
+            self.__painter.paint_objective_func()
+        self.__painter.save_image()
```

### Comparing `iOpt-0.2.1/iOpt/output_system/listeners/console_outputers.py` & `iOpt-0.2.22/iOpt/output_system/listeners/console_outputers.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from iOpt.method.search_data import SearchData, SearchDataItem
 from iOpt.solution import Solution
 from iOpt.method.method import Method
 from iOpt.output_system.outputers.console_outputer import ConsoleOutputer
 
 import numpy as np
 
+
 class ConsoleOutputListener(Listener):
     """
     Класс ConsoleFullOutputListener - слушатель событий. Содержит методы-обработчики, выдающие в качестве
       реакции на событие консольный вывод.
     """
 
     def __init__(self, mode='full', iters=100):
@@ -24,21 +25,21 @@
            выводит в консоль только финальный результат процесса оптимизации.
         :param iters: Частота вывода в консоль. Используется совместно с режимом вывода 'custom'.
         """
         self.__outputer: ConsoleOutputer = None
         self.mode = mode
         self.iters = iters
 
-    def BeforeMethodStart(self, method: Method):
+    def before_method_start(self, method: Method):
         self.__outputer = ConsoleOutputer(method.task.problem, method.parameters)
-        self.__outputer.PrintInitInfo()
+        self.__outputer.print_init_info()
 
-    def OnEndIteration(self, currPoints: List[SearchDataItem], currSolution: Solution):
+    def on_end_iteration(self, curr_points: List[SearchDataItem], curr_solution: Solution):
         if self.mode == 'full':
-            self.__outputer.PrintIterPointInfo(currPoints)
+            self.__outputer.print_iter_point_info(curr_points)
         elif self.mode == 'custom':
-            self.__outputer.PrintBestPointInfo(currSolution, self.iters)
+            self.__outputer.print_best_point_info(curr_solution, self.iters)
         elif self.mode == 'result':
             pass
 
-    def OnMethodStop(self, searchData: SearchData, solution: Solution, status: bool):
-        self.__outputer.PrintFinalResultInfo(solution, status)
+    def on_method_stop(self, search_data: SearchData, solution: Solution, status: bool):
+        self.__outputer.print_final_result_info(solution, status)
```

### Comparing `iOpt-0.2.1/iOpt/output_system/listeners/static_painters.py` & `iOpt-0.2.22/iOpt/output_system/listeners/static_painters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from iOpt.method.listener import Listener
-from iOpt.method.search_data import SearchData, SearchDataItem
-from iOpt.solution import Solution
 from iOpt.method.method import Method
-
+from iOpt.method.search_data import SearchData
 from iOpt.output_system.painters.static_painters import StaticPainter, StaticPainterND, DiscretePainter
+from iOpt.solution import Solution
 
-import numpy as np
 
 class StaticDiscreteListener(Listener):
     """
     """
-    def __init__(self, fileName: str, pathForSaves="", mode='analysis', calc='objective function', type='lines layers',
-                 numpoints=150, mrkrs=3):
+
+    def __init__(self, file_name: str, path_for_saves="", mode='analysis', calc='objective function',
+                 type='lines layers', numpoints=150, mrkrs=3):
         """
         """
         if mode != 'analysis' and mode != 'bestcombination':
             raise Exception(
                 "StaticDiscreteListener mode is incorrect, mode can take values 'analysis' or 'bestcombination'")
         if type != 'lines layers':
             raise Exception(
@@ -26,134 +25,136 @@
         if numpoints <= 0:
             raise Exception(
                 "StaticDiscreteListener numpoints is incorrect, numpoints > 0")
         if mrkrs <= 0:
             raise Exception(
                 "StaticDiscreteListener mrkrs is incorrect, mrkrs > 0")
 
-        self.fileName = fileName
-        self.pathForSaves = pathForSaves
+        self.file_name = file_name
+        self.path_for_saves = path_for_saves
         self.subparameters = [1, 2]
         self.mode = mode
         self.type = type
         self.calc = calc
         self.numpoints = numpoints
         self.mrkrs = mrkrs
-        self.searchDataSorted = []
+        self.search_dataSorted = []
         self.bestValueSorted = []
-        self.numberOfParallelPoints = 1
+        self.number_of_parallel_points = 1
 
-    def BeforeMethodStart(self, method: Method):
-        if method.task.problem.numberOfFloatVariables > 2 and self.calc == 'interpolation':
+    def before_method_start(self, method: Method):
+        if method.task.problem.number_of_float_variables > 2 and self.calc == 'interpolation':
             raise Exception(
                 "StaticDiscreteListener with calc 'interpolation' supported with dimension <= 2")
-        self.numberOfParallelPoints = method.parameters.numberOfParallelPoints
+        self.number_of_parallel_points = method.parameters.number_of_parallel_points
 
-    def OnEndIteration(self, newPoints, solution: Solution):
-        for newPoint in newPoints:
-            self.searchDataSorted.append(newPoint)
-            self.bestValueSorted.append(solution.bestTrials[0].functionValues[0].value)
-
-    def OnMethodStop(self, searchData: SearchData,
-                     solution: Solution, status: bool):
-        painter = DiscretePainter(self.searchDataSorted, self.bestValueSorted,
-                                  solution.problem.numberOfDiscreteVariables,
-                                  solution.problem.numberOfFloatVariables,
-                                  solution.bestTrials[0].point,
-                                  solution.problem.discreteVariableValues,
-                                  solution.problem.discreteVariableNames,
+    def on_end_iteration(self, new_points, solution: Solution):
+        for newPoint in new_points:
+            self.search_dataSorted.append(newPoint)
+            self.bestValueSorted.append(solution.best_trials[0].function_values[0].value)
+
+    def on_method_stop(self, search_data: SearchData,
+                       solution: Solution, status: bool):
+        painter = DiscretePainter(self.search_dataSorted, self.bestValueSorted,
+                                  solution.problem.number_of_discrete_variables,
+                                  solution.problem.number_of_float_variables,
+                                  solution.best_trials[0].point,
+                                  solution.problem.discrete_variable_values,
+                                  solution.problem.discrete_variable_names,
                                   self.mode, self.calc, self.subparameters,
-                                  solution.problem.lowerBoundOfFloatVariables,
-                                  solution.problem.upperBoundOfFloatVariables,
-                                  self.fileName, self.pathForSaves, solution.problem.Calculate,
-                                  solution.bestTrials[0].functionValues[0].value,
-                                  searchData, self.numberOfParallelPoints)
+                                  solution.problem.lower_bound_of_float_variables,
+                                  solution.problem.upper_bound_of_float_variables,
+                                  self.file_name, self.path_for_saves, solution.problem.calculate,
+                                  solution.best_trials[0].function_values[0].value,
+                                  search_data, self.number_of_parallel_points)
         if self.mode == 'analysis':
-            painter.PaintAnalisys(mrks=2)
+            painter.paint_analisys(mrks=2)
         elif self.mode == 'bestcombination':
             if self.type == 'lines layers':
-                painter.PaintObjectiveFunc(self.numpoints)
-                painter.PaintPoints(self.mrkrs)
+                painter.paint_objective_func(self.numpoints)
+                painter.paint_points(self.mrkrs)
+
+        painter.save_image()
 
-        painter.SaveImage()
 
 # mode: objective function, approximation, only points
 class StaticPainterListener(Listener):
     """
     Класс StaticPaintListener - слушатель событий. Содержит метод-обработчик, выдающий в качестве
       реакции на завершение работы метода изображение.
     """
 
-    def __init__(self, fileName: str, pathForSaves="", indx=0, isPointsAtBottom=False, mode='objective function'):
+    def __init__(self, file_name: str, path_for_saves="", indx=0, is_points_at_bottom=False, mode='objective function'):
         """
         Конструктор класса StaticPaintListener
 
-        :param fileName: Название файла с указанием формата для сохранения изображения. Обязательный параметр.
-        :param pathForSaves: Директория для сохранения изображения. В случае, если параметр не указан, изображение
+        :param file_name: Название файла с указанием формата для сохранения изображения. Обязательный параметр.
+        :param path_for_saves: Директория для сохранения изображения. В случае, если параметр не указан, изображение
            сохраняется в текущей рабочей директории.
         :param indx: Индекс переменной оптимизационной задачи. Используется в многомерной оптимизации.
            Позволяет отобразить в сечении найденного минимума процесс оптимизации по одной выбранной переменной.
-        :param isPointsAtBottom: Отрисовать точки поисковой информации под графиком. Если False, точки ставятся на графике.
+        :param is_points_at_bottom: Отрисовать точки поисковой информации под графиком. Если False, точки ставятся на графике.
         :param mode: Способ вычислений для отрисовки графика целевой функции, который будет использован. Возможные
            режимы: 'objective function', 'only points', 'approximation' и 'interpolation'. Режим 'objective function'
            строит график, вычисляя значения целевой функции на равномерной сетке. Режим 'approximation' строит
            нейроаппроксимацию для целевой функции на основе полученной поисковой информации.
            Режим 'interpolation' строит интерполяцию для целевой функции на основе полученной поисковой информации.
            Режим 'only points' не строит график целевой функции.
         """
-        self.fileName = fileName
-        self.pathForSaves = pathForSaves
+        self.file_name = file_name
+        self.path_for_saves = path_for_saves
         self.parameterInNDProblem = indx
-        self.isPointsAtBottom = isPointsAtBottom
+        self.is_points_at_bottom = is_points_at_bottom
         self.mode = mode
 
-    def OnMethodStop(self, searchData: SearchData,
-                     solution: Solution, status: bool):
-        painter = StaticPainter(searchData, solution, self.mode, self.isPointsAtBottom,
-                           self.parameterInNDProblem, self.pathForSaves, self.fileName)
-        painter.PaintObjectiveFunc()
-        painter.PaintPoints()
-        painter.PaintOptimum()
-        painter.SaveImage()
+    def on_method_stop(self, search_data: SearchData,
+                       solution: Solution, status: bool):
+        painter = StaticPainter(search_data, solution, self.mode, self.is_points_at_bottom,
+                                self.parameterInNDProblem, self.path_for_saves, self.file_name)
+        painter.paint_objective_func()
+        painter.paint_points()
+        painter.paint_optimum()
+        painter.save_image()
+
 
 # mode: surface, lines layers, approximation
 class StaticPainterNDListener(Listener):
     """
     Класс StaticNDPaintListener - слушатель событий. Содержит метод-обработчик, выдающий в качестве
       реакции на завершение работы метода изображение.
       Используется для многомерной оптимизации.
     """
 
-    def __init__(self, fileName: str, pathForSaves="", varsIndxs=[0, 1], mode='lines layers',
+    def __init__(self, file_name: str, path_for_saves="", vars_indxs=[0, 1], mode='lines layers',
                  calc='objective function'):
         """
         Конструктор класса StaticNDPaintListener
 
-        :param fileName: Название файла с указанием формата для сохранения изображения. Обязательный параметр.
-        :param pathForSaves: Директория для сохранения изображения. В случае, если параметр не указан, изображение
+        :param file_name: Название файла с указанием формата для сохранения изображения. Обязательный параметр.
+        :param path_for_saves: Директория для сохранения изображения. В случае, если параметр не указан, изображение
            сохраняется в текущей рабочей директории.
-        :param varsIndxs: Пара индексов переменных оптимизационной задачи, для которых будет построен рисунок.
+        :param vars_indxs: Пара индексов переменных оптимизационной задачи, для которых будет построен рисунок.
         :param mode_: Режим отрисовки графика целевой функции, который будет использован.
            Возможные режимы:'lines layers', 'surface'.
            Режим 'lines layers' рисует линии уровня в сечении найденного методом решения.
            Режим 'surface' строит поверхность в сечении найденного методом решения.
         :param calc: Способ вычислений для отрисовки графика целевой функции, который будет использован. Возможные
            режимы: 'objective function' (только в режиме 'lines layers'), 'approximation' (только в режиме 'surface')
            и 'interpolation'. Режим 'objective function' строит график, вычисляя значения целевой функции на равномерной
            сетке. Режим 'approximation' строит нейроаппроксимацию для целевой функции на основе полученной поисковой
            информации. Режим 'interpolation' строит интерполяцию для целевой функции на основе полученной поисковой
            информации.
         """
-        self.fileName = fileName
-        self.pathForSaves = pathForSaves
-        self.parameters = varsIndxs
+        self.file_name = file_name
+        self.path_for_saves = path_for_saves
+        self.parameters = vars_indxs
         self.mode = mode
         self.calc = calc
 
-    def OnMethodStop(self, searchData: SearchData,
-                     solution: Solution, status: bool, ):
-        painter = StaticPainterND(searchData, solution, self.parameters, self.mode, self.calc,
-                           self.fileName, self.pathForSaves)
-        painter.PaintObjectiveFunc()
-        painter.PaintPoints()
-        painter.PaintOptimum()
-        painter.SaveImage()
+    def on_method_stop(self, search_data: SearchData,
+                       solution: Solution, status: bool, ):
+        painter = StaticPainterND(search_data, solution, self.parameters, self.mode, self.calc,
+                                  self.file_name, self.path_for_saves)
+        painter.paint_objective_func()
+        painter.paint_points()
+        painter.paint_optimum()
+        painter.save_image()
```

### Comparing `iOpt-0.2.1/iOpt/output_system/outputers/console_outputer.py` & `iOpt-0.2.22/iOpt/output_system/outputers/console_outputer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,173 +1,187 @@
 from typing import List
 
 from iOpt.method.search_data import SearchDataItem
 from iOpt.problem import Problem
 from iOpt.solution import Solution
 from iOpt.solver_parametrs import SolverParameters
 
+
 class ConsoleOutputer:
     def __init__(self, problem: Problem, parameters: SolverParameters):
         self.problem = problem
         self.parameters = parameters
         self.__functions = OutputFunctions()
         self.iterNum = 1
-        self.ndv = self.problem.numberOfDiscreteVariables
+        self.ndv = self.problem.number_of_discrete_variables
 
-    def PrintInitInfo(self):
-        self.__functions.printInit(
+    def print_init_info(self):
+        self.__functions.print_init(
             self.parameters.eps,
             self.parameters.r,
-            self.parameters.epsR,
-            self.parameters.itersLimit,
-            self.problem.numberOfFloatVariables,
-            self.problem.numberOfObjectives,
-            self.problem.numberOfConstraints,
-            self.problem.lowerBoundOfFloatVariables,
-            self.problem.upperBoundOfFloatVariables,
-            self.problem.numberOfDiscreteVariables,
-            self.parameters.numberOfParallelPoints
+            self.parameters.eps_r,
+            self.parameters.iters_limit,
+            self.problem.number_of_float_variables,
+            self.problem.number_of_objectives,
+            self.problem.number_of_constraints,
+            self.problem.lower_bound_of_float_variables,
+            self.problem.upper_bound_of_float_variables,
+            self.problem.number_of_discrete_variables,
+            self.parameters.number_of_parallel_points
         )
 
-    def PrintIterPointInfo(self, savedNewPoints: List[SearchDataItem]):
-        if self.parameters.numberOfParallelPoints > 1:
+    def print_iter_point_info(self, saved_new_points: List[SearchDataItem]):
+        if self.parameters.number_of_parallel_points > 1:
             isFirst = True
         else:
             isFirst = False
 
-        for i in range(len(savedNewPoints)):
-            point = savedNewPoints[i].GetY().floatVariables
-            dpoint = savedNewPoints[i].GetY().discreteVariables
-            value = savedNewPoints[i].GetZ()
+        for i in range(len(saved_new_points)):
+            point = saved_new_points[i].get_y().float_variables
+            dpoint = saved_new_points[i].get_y().discrete_variables
+            value = saved_new_points[i].get_z()
 
-            self.__functions.printIter(
+            self.__functions.print_iter(
                 point,
                 dpoint,
                 value,
                 self.iterNum, self.ndv,
                 isFirst
             )
             isFirst = False
 
             self.iterNum += 1
 
-    def PrintBestPointInfo(self, solution, iters):
+    def print_best_point_info(self, solution, iters):
         if self.iterNum % iters != 0:
             pass
         else:
-            bestTrialPoint = solution.bestTrials[0].point.floatVariables
-            bestTrialDPoint = solution.bestTrials[0].point.discreteVariables
-            bestTrialValue = solution.bestTrials[0].functionValues[0].value
-            self.__functions.printBest(
-                solution.numberOfGlobalTrials,
-                solution.numberOfLocalTrials,
-                solution.solutionAccuracy,
-                bestTrialPoint,
-                bestTrialDPoint,
-                bestTrialValue,
+            best_trial_point = solution.best_trials[0].point.float_variables
+            best_trial_d_point = solution.best_trials[0].point.discrete_variables
+            best_trial_value = solution.best_trials[0].function_values[0].value
+            self.__functions.print_best(
+                solution.number_of_global_trials,
+                solution.number_of_local_trials,
+                solution.solution_accuracy,
+                best_trial_point,
+                best_trial_d_point,
+                best_trial_value,
                 self.iterNum, self.ndv
             )
         self.iterNum += 1
 
-    def PrintFinalResultInfo(self, solution: Solution, status: bool):
-        bestTrialPoint = solution.bestTrials[0].point.floatVariables
-        bestTrialDPoint = solution.bestTrials[0].point.discreteVariables
-        bestTrialValue = solution.bestTrials[0].functionValues[0].value
-        self.__functions.printResult(
+    def print_final_result_info(self, solution: Solution, status: bool):
+        best_trial_point = solution.best_trials[0].point.float_variables
+        best_trial_d_point = solution.best_trials[0].point.discrete_variables
+        best_trial_value = solution.best_trials[0].function_values[0].value
+        self.__functions.print_result(
             status,
-            solution.numberOfGlobalTrials,
-            solution.numberOfLocalTrials,
-            solution.solvingTime,
-            solution.solutionAccuracy,
-            bestTrialPoint,
-            bestTrialDPoint,
-            bestTrialValue, self.ndv
+            solution.number_of_global_trials,
+            solution.number_of_local_trials,
+            solution.solving_time,
+            solution.solution_accuracy,
+            best_trial_point,
+            best_trial_d_point,
+            best_trial_value, self.ndv
         )
 
 
 class OutputFunctions:
 
-    def printInit(self, eps, r, epsR, itersLimit, floatdim, numberOfObjectives, numberOfConstraints,
-                  lowerBoundOfFloatVariables, upperBoundOfFloatVariables, numberOfDiscreteVariables,
-                  numberOfParallelPoints):
-        dim = floatdim + numberOfDiscreteVariables
+    def print_init(self, eps, r, eps_r, iters_limit, floatdim, number_of_objectives, number_of_constraints,
+                   lower_bound_of_float_variables, upper_bound_of_float_variables, number_of_discrete_variables,
+                   number_of_parallel_points):
+        dim = floatdim + number_of_discrete_variables
         size_max_one_output = 15
         print()
         print("-" * (30 + size_max_one_output * dim + 2))
         print("|{:^{width}}|".format("Task Description", width=30 + size_max_one_output * dim))
         print("-" * (30 + size_max_one_output * dim + 2))
         print("|{:>29} {:<{width}}|".format("dimension: ", floatdim, width=size_max_one_output * dim))
         tempstr = "["
         for i in range(floatdim):
             tempstr += "["
-            tempstr += str(lowerBoundOfFloatVariables[i])
+            tempstr += str(lower_bound_of_float_variables[i])
             tempstr += ", "
-            tempstr += str(upperBoundOfFloatVariables[i])
+            tempstr += str(upper_bound_of_float_variables[i])
             tempstr += "], "
         tempstr = tempstr[:-2]
         tempstr += "]"
         print("|{:>29} {:<{width}}|".format("bounds: ", tempstr, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}}|".format("objective-function count: ", numberOfObjectives, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}}|".format("constraint-function count: ", numberOfConstraints, width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("objective-function count: ", number_of_objectives,
+                                            width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("constraint-function count: ", number_of_constraints,
+                                            width=size_max_one_output * dim))
         print("-" * (30 + size_max_one_output * dim + 2))
         print("|{:^{width}}|".format("Method Parameters", width=30 + size_max_one_output * dim))
         print("-" * (30 + size_max_one_output * dim + 2))
         print("|{:>29} {:<{width}}|".format("eps: ", eps, width=size_max_one_output * dim))
         print("|{:>29} {:<{width}}|".format("r: ", r, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}}|".format("epsR: ", epsR, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}}|".format("itersLimit: ", itersLimit, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}}|".format("numberOfParallelPoints: ", numberOfParallelPoints, width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("eps_r: ", eps_r, width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("iters_limit: ", iters_limit, width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("number_of_parallel_points: ", number_of_parallel_points,
+                                            width=size_max_one_output * dim))
         print("-" * (30 + size_max_one_output * dim + 2))
         print("|{:^{width}}|".format("Iterations", width=30 + size_max_one_output * dim))
         print("-" * (30 + size_max_one_output * dim + 2))
         print("|{:^{width}}|".format("", width=30 + size_max_one_output * dim))
 
-    def printIter(self, point, dpoint, value, iter, ndv, flag):
+    def print_iter(self, point, dpoint, value, iter, ndv, flag):
         size_max_one_output = 15
         dim1 = len(point)
         if dpoint:
             dim2 = len(dpoint)
         else:
             dim2 = 0
         print("|", end=' ')
         # print("\033[A|", end=' ')
         if flag:
             print("*{:>4}:".format(iter), end=' ')
         else:
             print("{:>5}:".format(iter), end=' ')
         print("{:>19.8f}".format(value), end='   ')
         if ndv > 0:
-            print("{:<{width}}|".format(str(point) + " with " + str(dpoint), width = size_max_one_output * (dim1 + dim2)))
+            print("{:<{width}}|".format(str(point) + " with " + str(dpoint), width=size_max_one_output * (dim1 + dim2)))
         else:
             print("{:<{width}}|".format(str(point), width=size_max_one_output * dim1))
 
-    def printResult(self, solved, numberOfGlobalTrials, numberOfLocalTrials, solvingTime, solutionAccuracy,
-                    bestTrialPoint, bestTrialDPoint, bestTrialValue, ndv):
+    def print_result(self, solved, number_of_global_trials, number_of_local_trials, solving_time,
+                     solution_accuracy, best_trial_point, best_trial_d_point, best_trial_value, ndv):
         size_max_one_output = 15
-        dim = len(bestTrialPoint) + len(bestTrialDPoint)
+        dim = len(best_trial_point) + len(best_trial_d_point)
         print("-" * (30 + size_max_one_output * dim + 2))
         print("|{:^{width}}|".format("Result", width=30 + size_max_one_output * dim))
         print("-" * (30 + size_max_one_output * dim + 2))
         # print("|{:>29} {:<{width}}|".format("is solved: ", str(solved), width=20*dim))
-        print("|{:>29} {:<{width}}|".format("global iteration count: ", numberOfGlobalTrials, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}}|".format("local iteration count: ", numberOfLocalTrials, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}}|".format("solving time: ", solvingTime, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}}|".format("solution point: ", str(bestTrialPoint), width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("global iteration count: ", number_of_global_trials,
+                                            width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("local iteration count: ", number_of_local_trials,
+                                            width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("solving time: ", solving_time, width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("solution point: ", str(best_trial_point), width=size_max_one_output * dim))
         if ndv > 0:
-            print("|{:>29} {:<{width}}|".format("best disrete combination: ", str(bestTrialDPoint), width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}.8f}|".format("solution value: ", bestTrialValue, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}.8f}|".format("accuracy: ", solutionAccuracy, width=size_max_one_output * dim))
+            print("|{:>29} {:<{width}}|".format("best disrete combination: ", str(best_trial_d_point),
+                                                width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}.8f}|".format("solution value: ", best_trial_value, width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}.8f}|".format("accuracy: ", solution_accuracy, width=size_max_one_output * dim))
         print("-" * (30 + size_max_one_output * dim + 2))
 
-    def printBest(self, numberOfGlobalTrials, numberOfLocalTrials, solutionAccuracy,
-                  bestTrialPoint, bestTrialDPoint, bestTrialValue, iter, ndv):
+    def print_best(self, number_of_global_trials, number_of_local_trials, solution_accuracy,
+                   best_trial_point, best_trial_d_point, best_trial_value, curr_iter, ndv):
         size_max_one_output = 15
-        dim = len(bestTrialPoint) + len(bestTrialDPoint)
-        print("|{:>29} {:<{width}}|".format("current iteration # ", iter, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}}|".format("global iteration count: ", numberOfGlobalTrials, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}}|".format("local iteration count: ", numberOfLocalTrials, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}}|".format("current best point: ", str(bestTrialPoint), width=size_max_one_output * dim))
+        dim = len(best_trial_point) + len(best_trial_d_point)
+        print("|{:>29} {:<{width}}|".format("current iteration # ", curr_iter,
+                                            width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("global iteration count: ", number_of_global_trials,
+                                            width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("local iteration count: ", number_of_local_trials,
+                                            width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}}|".format("current best point: ", str(best_trial_point),
+                                            width=size_max_one_output * dim))
         if ndv > 0:
-            print("|{:>29} {:<{width}}|".format("with discrete combination: ", str(bestTrialDPoint), width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}.8f}|".format("current best value: ", bestTrialValue, width=size_max_one_output * dim))
-        print("|{:>29} {:<{width}.8f}|".format("currant accuracy: ", solutionAccuracy, width=size_max_one_output * dim))
+            print("|{:>29} {:<{width}}|".format("with discrete combination: ", str(best_trial_d_point),
+                                                width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}.8f}|".format("current best value: ", best_trial_value,
+                                               width=size_max_one_output * dim))
+        print("|{:>29} {:<{width}.8f}|".format("currant accuracy: ", solution_accuracy,
+                                               width=size_max_one_output * dim))
         print("." * (30 + size_max_one_output * dim + 2))
```

### Comparing `iOpt-0.2.1/iOpt/output_system/painters/animate_painters.py` & `iOpt-0.2.22/iOpt/output_system/painters/animate_painters.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,124 +5,124 @@
 from iOpt.output_system.painters.painter import Painter
 from iOpt.output_system.painters.plotters.plotters import AnimatePlotter2D, AnimatePlotter3D
 
 import matplotlib.pyplot as plt
 import os
 
 class AnimatePainter(Painter):
-    def __init__(self, isPointsAtBottom, parameterInNDProblem, pathForSaves, fileName):
-        self.pathForSaves = pathForSaves
-        self.fileName = fileName
-        self.isPointsAtBottom = isPointsAtBottom
+    def __init__(self, is_points_at_bottom, parameter_in_nd_problem, path_for_saves, file_name):
+        self.path_for_saves = path_for_saves
+        self.file_name = file_name
+        self.is_points_at_bottom = is_points_at_bottom
         self.objFunc = None
-        self.parameterInNDProblem = parameterInNDProblem
+        self.parameterInNDProblem = parameter_in_nd_problem
         self.section = []
 
         # настройки графика
-        self.plotter = AnimatePlotter2D(parameterInNDProblem, 0, 1)
+        self.plotter = AnimatePlotter2D(parameter_in_nd_problem, 0, 1)
 
-    def SetProblem(self, problem: Problem):
-        self.objFunc = problem.Calculate
+    def set_problem(self, problem: Problem):
+        self.objFunc = problem.calculate
 
-        for i in range(problem.numberOfFloatVariables):
-            self.section.append(float(problem.upperBoundOfFloatVariables[i]) - float(problem.lowerBoundOfFloatVariables[i]))
+        for i in range(problem.number_of_float_variables):
+            self.section.append(float(problem.upper_bound_of_float_variables[i]) - float(problem.lower_bound_of_float_variables[i]))
 
         # настройки графика
-        self.plotter.SetBounds(float(problem.lowerBoundOfFloatVariables[self.parameterInNDProblem]),
-                                 float(problem.upperBoundOfFloatVariables[self.parameterInNDProblem]))
+        self.plotter.set_bounds(float(problem.lower_bound_of_float_variables[self.parameterInNDProblem]),
+                                float(problem.upper_bound_of_float_variables[self.parameterInNDProblem]))
 
-    def PaintObjectiveFunc(self):
-        self.plotter.PlotByGrid(self.CalculateFunc, self.section.copy(), pointsCount=150)
+    def paint_objective_func(self):
+        self.plotter.plot_by_grid(self.calculate_func, self.section.copy(), points_count=150)
 
-    def PaintPoints(self, currPoints):
-        x = [currPoint.GetY().floatVariables[self.parameterInNDProblem] for currPoint in currPoints]
-        fv = [currPoint.GetZ() for currPoint in currPoints]
-        if self.isPointsAtBottom:
-            fv = [currPoint.GetZ() * 0.7 for currPoint in currPoints]
+    def paint_points(self, curr_points):
+        x = [currPoint.get_y().float_variables[self.parameterInNDProblem] for currPoint in curr_points]
+        fv = [currPoint.get_z() for currPoint in curr_points]
+        if self.is_points_at_bottom:
+            fv = [currPoint.get_z() * 0.7 for currPoint in curr_points]
         else:
-            fv = [currPoint.GetZ() for currPoint in currPoints]
-        self.plotter.PlotPoints(x, fv, 'blue', 'o', 4)
+            fv = [currPoint.get_z() for currPoint in curr_points]
+        self.plotter.plot_points(x, fv, 'blue', 'o', 4)
 
-    def PaintOptimum(self, solution: Solution):
-        optimum = solution.bestTrials[0].point.floatVariables[self.parameterInNDProblem]
-        optimumVal = solution.bestTrials[0].functionValues[0].value
+    def paint_optimum(self, solution: Solution):
+        optimum = solution.best_trials[0].point.float_variables[self.parameterInNDProblem]
+        optimumVal = solution.best_trials[0].function_values[0].value
 
         value = optimumVal
 
-        if self.isPointsAtBottom:
+        if self.is_points_at_bottom:
             value = value * 0.7
 
-        self.plotter.PlotPoints([optimum], [value], 'red', 'o', 4)
+        self.plotter.plot_points([optimum], [value], 'red', 'o', 4)
 
-    def SaveImage(self):
-        if not os.path.isdir(self.pathForSaves):
-            if self.pathForSaves == "":
-                plt.savefig(self.fileName)
+    def save_image(self):
+        if not os.path.isdir(self.path_for_saves):
+            if self.path_for_saves == "":
+                plt.savefig(self.file_name)
             else:
-                os.mkdir(self.pathForSaves)
-                plt.savefig(self.pathForSaves + "/" + self.fileName)
+                os.mkdir(self.path_for_saves)
+                plt.savefig(self.path_for_saves + "/" + self.file_name)
         else:
-            plt.savefig(self.pathForSaves + "/" + self.fileName)
+            plt.savefig(self.path_for_saves + "/" + self.file_name)
         plt.ioff()
         plt.show()
 
-    def CalculateFunc(self, x):
+    def calculate_func(self, x):
         point = Point(x, [])
         fv = FunctionValue()
         fv = self.objFunc(point, fv)
         return fv.value
 
 
 class AnimatePainterND(Painter):
-    def __init__(self, parametersInNDProblem, pathForSaves, fileName):
-        self.pathForSaves = pathForSaves
-        self.fileName = fileName
+    def __init__(self, parameters_in_nd_problem, path_for_saves, file_name):
+        self.path_for_saves = path_for_saves
+        self.file_name = file_name
         self.objFunc = None
-        self.parametersInNDProblem = parametersInNDProblem
+        self.parametersInNDProblem = parameters_in_nd_problem
         self.section = []
 
         # настройки графика
-        self.plotter = AnimatePlotter3D(parametersInNDProblem)
+        self.plotter = AnimatePlotter3D(parameters_in_nd_problem)
 
-    def SetProblem(self, problem: Problem):
-        self.objFunc = problem.Calculate
+    def set_problem(self, problem: Problem):
+        self.objFunc = problem.calculate
 
         # настройки графика
-        self.plotter.SetBounds([float(problem.lowerBoundOfFloatVariables[self.parametersInNDProblem[0]]),
-                               float(problem.lowerBoundOfFloatVariables[self.parametersInNDProblem[1]])],
-                               [float(problem.upperBoundOfFloatVariables[self.parametersInNDProblem[0]]),
-                               float(problem.upperBoundOfFloatVariables[self.parametersInNDProblem[1]])])
-
-    def PaintObjectiveFunc(self):
-        self.plotter.PlotByGrid(self.CalculateFunc, self.section, pointsCount=150)
-
-    def PaintPoints(self, currPoints):
-        x = [[currPoint.GetY().floatVariables[self.parametersInNDProblem[0]] for currPoint in currPoints],
-        [currPoint.GetY().floatVariables[self.parametersInNDProblem[1]] for currPoint in currPoints]]
-        self.plotter.PlotPoints(x, [], 'blue', 'o', 4)
-
-    def PaintOptimum(self, solution: Solution):
-        optimum = [solution.bestTrials[0].point.floatVariables[self.parametersInNDProblem[0]],
-                   solution.bestTrials[0].point.floatVariables[self.parametersInNDProblem[1]]]
-        optimumVal = solution.bestTrials[0].functionValues[0].value
+        self.plotter.set_bounds([float(problem.lower_bound_of_float_variables[self.parametersInNDProblem[0]]),
+                                 float(problem.lower_bound_of_float_variables[self.parametersInNDProblem[1]])],
+                                [float(problem.upper_bound_of_float_variables[self.parametersInNDProblem[0]]),
+                               float(problem.upper_bound_of_float_variables[self.parametersInNDProblem[1]])])
+
+    def paint_objective_func(self):
+        self.plotter.plot_by_grid(self.calculate_func, self.section, points_count=150)
+
+    def paint_points(self, curr_points):
+        x = [[currPoint.get_y().float_variables[self.parametersInNDProblem[0]] for currPoint in curr_points],
+             [currPoint.get_y().float_variables[self.parametersInNDProblem[1]] for currPoint in curr_points]]
+        self.plotter.plot_points(x, [], 'blue', 'o', 4)
+
+    def paint_optimum(self, solution: Solution):
+        optimum = [solution.best_trials[0].point.float_variables[self.parametersInNDProblem[0]],
+                   solution.best_trials[0].point.float_variables[self.parametersInNDProblem[1]]]
+        optimumVal = solution.best_trials[0].function_values[0].value
 
-        self.plotter.PlotPoints(optimum, [], 'red', 'o', 4)
+        self.plotter.plot_points(optimum, [], 'red', 'o', 4)
 
         self.section = optimum
 
-    def SaveImage(self):
-        if not os.path.isdir(self.pathForSaves):
-            if self.pathForSaves == "":
-                plt.savefig(self.fileName)
+    def save_image(self):
+        if not os.path.isdir(self.path_for_saves):
+            if self.path_for_saves == "":
+                plt.savefig(self.file_name)
             else:
-                os.mkdir(self.pathForSaves)
-                plt.savefig(self.pathForSaves + "/" + self.fileName)
+                os.mkdir(self.path_for_saves)
+                plt.savefig(self.path_for_saves + "/" + self.file_name)
         else:
-            plt.savefig(self.pathForSaves + "/" + self.fileName)
+            plt.savefig(self.path_for_saves + "/" + self.file_name)
         plt.ioff()
         plt.show()
 
-    def CalculateFunc(self, x):
+    def calculate_func(self, x):
         point = Point(x, [])
         fv = FunctionValue()
         fv = self.objFunc(point, fv)
         return fv.value
```

### Comparing `iOpt-0.2.1/iOpt/output_system/painters/plotters/plotters.py` & `iOpt-0.2.22/iOpt/output_system/painters/plotters/plotters.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 
 from sklearn.neural_network import MLPRegressor
 from scipy import interpolate
 from matplotlib.cm import ScalarMappable
 from textwrap import wrap
 
 class DisretePlotter:
-    def __init__(self, mode, pcount, floatdim, parametersvals, parametersnames, subparameters, lb, rb, bestsvalues, numberOfParallelPoints):
+    def __init__(self, mode, pcount, floatdim, parametersvals, parametersnames, subparameters, lb, rb, bestsvalues,
+                 number_of_parallel_points):
         plt.style.use('fivethirtyeight')
         plt.rcParams['contour.negative_linestyle'] = 'solid'
         plt.rcParams['figure.figsize'] = (12, 6)
         plt.rcParams['font.size'] = 6
 
-        self.numberOfParallelPoints = numberOfParallelPoints
+        self.number_of_parallel_points = number_of_parallel_points
         self.subparameters = subparameters
         self.lb = lb
         self.rb = rb
         self.floatdim = floatdim
         self.bestsvalues=bestsvalues
 
         self.discreteParamsCombinations = [list(x) for x in np.array(np.meshgrid(*parametersvals)).T.reshape(-1,
@@ -70,31 +71,31 @@
             self.axes[1].grid(False)
             self.axes[1].set_xticks([])
             self.axes[1].set_yticks([])
             plt.tight_layout()
 
         self.name = ['' + parametersnames[i] + '' for i in range(len(parametersnames))]
 
-    def PlotAnalisysSubplotsFigure(self, allpoints, allvalues, combinations, optimum, mrkrs=3):
+    def plot_analisys_subplots_figure(self, allpoints, allvalues, combinations, optimum, mrkrs=3):
             for j in range(self.count):
-                self.axes[j].scatter([x.discreteVariables[0] for x in allpoints],
+                self.axes[j].scatter([x.discrete_variables[0] for x in allpoints],
                                      [item[0] for item in allvalues],
                                      s=mrkrs ** 2, color='black')
-                self.axes[j].scatter([optimum.discreteVariables[j]],
+                self.axes[j].scatter([optimum.discrete_variables[j]],
                                      [self.bestsvalues[-1]],
                                      s=(mrkrs+2) ** 2, color='red', marker='*')
                 self.axes[j].set_xlim([self.axes[j].get_xlim()[0] - 1, self.axes[j].get_xlim()[1] + 1])
 
             id = -1
             for i in range(1, len(self.bestsvalues)):
                 if self.bestsvalues[-1] < self.bestsvalues[-i]:
                     id = i
                     break
-            best_iter = int(len(self.bestsvalues) - id + self.numberOfParallelPoints +
-                            (self.numberOfParallelPoints == 1))
+            best_iter = int(len(self.bestsvalues) - id + self.number_of_parallel_points +
+                            (self.number_of_parallel_points == 1))
 
             self.axes[self.count].plot([int(item[1]) for item in allvalues],
                                        [item[0] for item in allvalues],
                                        color='black', linewidth=1, alpha=1)
             self.axes[self.count].scatter([best_iter], [self.bestsvalues[-1]],
                                           s=(mrkrs+2) ** 2, color='red', marker='*')
 
@@ -111,43 +112,43 @@
                 for i in x:
                     str_ += i + ', '
                 str_ = str_[:-2]
                 str_ += ']'
                 combinations.append(str_)
             self.axes[self.count + 1].scatter([allvalues[0][0]] * self.combcount, combinations, alpha=0)
 
-            text = "best value "+ str(self.bestsvalues[-1]) + " in point " + str(optimum.floatVariables)
-            text += ' with ' + str(optimum.discreteVariables)
+            text = "best value "+ str(self.bestsvalues[-1]) + " in point " + str(optimum.float_variables)
+            text += ' with ' + str(optimum.discrete_variables)
             text = '\n'.join(wrap(text, 90))
 
             iters = list(range(1, len(self.bestsvalues) + 1))
             self.axes[self.count + 2].plot(iters, self.bestsvalues, color='black', linewidth=1, alpha=1)
             l1 = self.axes[self.count + 2].scatter([best_iter], [self.bestsvalues[-1]],
                                                    label=text, s=(mrkrs+2) ** 2, color='red', marker='*')
 
             self.axes[self.count + 3].legend(handles =[l1] , labels=[text],
                                                           numpoints=1, ncol=1,
                                                           fontsize=10, loc='lower left')
             plt.tight_layout()
 
-    def PlotPoints(self, best, other, optimum, optimumPoint, mrkrs):
+    def plot_points(self, best, other, optimum, optimum_point, mrkrs):
             '''
             self.ax.scatter(other[0], other[1], s=mrkrs ** 2, color='grey',
                             label='points with another discrete parameters combinations')
             '''
             self.axes[0].scatter(best[0], best[1], s=mrkrs ** 2, color='blue',
-                            label='points with discrete parameters combination ' + str(optimum.discreteVariables))
+                            label='points with discrete parameters combination ' + str(optimum.discrete_variables))
 
-            text = 'optimum point ' + str(optimum.floatVariables) + ' with '+ str(optimum.discreteVariables) + ' and optimum value ' + str(self.bestsvalues[-1])
+            text = 'optimum point ' + str(optimum.float_variables) + ' with '+ str(optimum.discrete_variables) + ' and optimum value ' + str(self.bestsvalues[-1])
             text = '\n'.join(wrap(text, 90))
 
-            l1 = self.axes[0].scatter(optimumPoint[0],
-                            optimumPoint[1],
-                            s=mrkrs ** 2, color='red',
-                            label= text)
+            l1 = self.axes[0].scatter(optimum_point[0],
+                                      optimum_point[1],
+                                      s=mrkrs ** 2, color='red',
+                                      label= text)
 
             if self.floatdim > 1:
                 self.axes[0].set_title(
                 'Lines layers of objective function in section of optimum point',
                 fontsize=12)
             else:
                 self.axes[0].set_title(
@@ -156,266 +157,267 @@
 
             legend_obj = self.axes[1].legend(handles =[l1] , labels=[text], loc='upper left', prop={'size': 10},
                                              bbox_to_anchor=(0, -0.4), fancybox=True,
                                              shadow=True, ncol=1)
             legend_obj.set_draggable(True)
             plt.tight_layout()
 
-    def PlotByGrid(self, calculate, section, pointsCount):
+    def plot_by_grid(self, calculate, section, points_count):
             if self.floatdim > 1:
                 i = self.subparameters[0]
                 j = self.subparameters[1]
 
-                xi = np.linspace(self.lb[i - 1], self.rb[i - 1], pointsCount)
-                xj = np.linspace(self.lb[j - 1], self.rb[j - 1], pointsCount)
+                xi = np.linspace(self.lb[i - 1], self.rb[i - 1], points_count)
+                xj = np.linspace(self.lb[j - 1], self.rb[j - 1], points_count)
                 xv, yv = np.meshgrid(xi, xj)
 
                 z = []
-                fv = section.floatVariables.copy()
-                for k in range(pointsCount):
+                fv = section.float_variables.copy()
+                for k in range(points_count):
                     z_ = []
-                    for t in range(pointsCount):
+                    for t in range(points_count):
                         fv[i - 1] = xv[k, t]
                         fv[j - 1] = yv[k, t]
-                        z_.append(calculate(fv, section.discreteVariables))
+                        z_.append(calculate(fv, section.discrete_variables))
                     z.append(z_)
 
 
                 self.axes[0].set_xlabel('x' + str(i))
                 self.axes[0].set_ylabel('x' + str(j))
 
                 xx = self.axes[0].contour(xi, xj, z, linewidths=1, levels=10, cmap='plasma')
 
                 self.fig.colorbar(ScalarMappable(norm=xx.norm, cmap=xx.cmap), ax=self.axes[0], orientation='vertical')
 
             else:
-                x = np.linspace(self.lb[0], self.rb[0], pointsCount)
+                x = np.linspace(self.lb[0], self.rb[0], points_count)
                 z = []
-                fv = section.floatVariables.copy()
-                for k in range(pointsCount):
+                fv = section.float_variables.copy()
+                for k in range(points_count):
                     fv[0] = x[k]
-                    z.append(calculate(fv, section.discreteVariables))
+                    z.append(calculate(fv, section.discrete_variables))
 
                 self.axes[0].set_xlabel('trial point')
                 self.axes[0].set_ylabel('objective function value')
 
                 self.axes[0].plot(x, z, linewidth=1, color='black', alpha=0.7)
 
-    def PlotInterpolation(self, points, values, pointsCount=100):
+    def plot_interpolation(self, points, values, points_count=100):
             if self.floatdim > 1:
                 i = self.subparameters[0] - 1
                 j = self.subparameters[1] - 1
                 interp = interpolate.Rbf(np.array(points)[:, 0], np.array(points)[:, 1], values)
-                x1 = np.linspace(self.lb[i], self.rb[i], pointsCount)
-                x2 = np.linspace(self.lb[j], self.rb[j], pointsCount)
+                x1 = np.linspace(self.lb[i], self.rb[i], points_count)
+                x2 = np.linspace(self.lb[j], self.rb[j], points_count)
                 x1, x2 = np.meshgrid(x1, x2)
                 z = interp(x1, x2)
                 xx=self.axes[0].contour(x1, x2, z, levels=10, linewidths=1, cmap='plasma')
                 self.fig.colorbar(ScalarMappable(norm=xx.norm, cmap=xx.cmap))
             else:
                 f = interpolate.interp1d(np.array(points), np.array(values), kind=3)
-                x_plot = np.linspace(min(np.array(points)), max(np.array(points)), pointsCount)
+                x_plot = np.linspace(min(np.array(points)), max(np.array(points)), points_count)
                 plt.plot(x_plot, f(x_plot), color='black', linewidth=1, alpha=0.7)
 
 class Plotter:
     """
     Базовый класс вызовов функций стандартного плоттера matplotlib.pyplot.
     """
-    def PlotByGrid(self):
+    def plot_by_grid(self):
         pass
-    def PlotApproximation(self):
+    def plot_approximation(self):
         pass
-    def PlotInterpolation(self):
+    def plot_interpolation(self):
         pass
-    def PlotPoints(self):
+    def plot_points(self):
         pass
 
 class Plotter2D(Plotter):
-    def __init__(self, parameterInNDProblem, leftBound, rightBound):
+    def __init__(self, parameter_in_nd_problem, left_bound, right_bound):
         plt.style.use('fivethirtyeight')
         plt.rcParams['contour.negative_linestyle'] = 'solid'
         plt.rcParams["figure.figsize"] = (8, 6)
 
-        self.index = parameterInNDProblem
-        self.leftBound = leftBound
-        self.rightBound = rightBound
+        self.index = parameter_in_nd_problem
+        self.leftBound = left_bound
+        self.rightBound = right_bound
 
         self.fig, self.ax = plt.subplots(1, 1)
         self.ax.tick_params(axis='both', labelsize=8)
         self.ax.set_xlim([self.leftBound, self.rightBound])
 
-    def PlotByGrid(self, calculate, section, pointsCount=100):
-        x = np.arange(self.leftBound, self.rightBound, (self.rightBound - self.leftBound) / pointsCount)
+    def plot_by_grid(self, calculate, section, points_count=100):
+        x = np.arange(self.leftBound, self.rightBound, (self.rightBound - self.leftBound) / points_count)
         z = []
-        for i in range(pointsCount):
+        for i in range(points_count):
             section[self.index] = x[i]
             z.append(calculate(section))
         plt.plot(x, z, linewidth=1, color='black', alpha=0.7)
 
-    def PlotApproximation(self, points, values, pointsCount=100):
+    def plot_approximation(self, points, values, points_count=100):
         nn = MLPRegressor(activation='logistic',  # can be tanh, identity, logistic, relu
                           solver='lbfgs',  # can be lbfgs, sgd , adam
                           alpha=0.001,
                           hidden_layer_sizes=(50,),
                           max_iter=5000,
                           tol=10e-8,
                           random_state=None)
         nn.fit(np.array(points)[:, np.newaxis], np.array(values))
-        x_plot = np.linspace(self.leftBound, self.rightBound, pointsCount)
+        x_plot = np.linspace(self.leftBound, self.rightBound, points_count)
         z = nn.predict(x_plot[:, np.newaxis])
         plt.plot(x_plot, z, color='black', linewidth=1, alpha=0.7)
 
-    def PlotInterpolation(self, points, values, pointsCount=100):
+    def plot_interpolation(self, points, values, points_count=100):
         f = interpolate.interp1d(np.array(points), np.array(values), kind=3)
-        x_plot = np.linspace(min(np.array(points)), max(np.array(points)), pointsCount)
+        x_plot = np.linspace(min(np.array(points)), max(np.array(points)), points_count)
         plt.plot(x_plot, f(x_plot), color='black', linewidth=1, alpha=0.7)
 
-    def PlotPoints(self, points, values, clr='blue', mrkr='o', mrkrs=4):
+    def plot_points(self, points, values, clr='blue', mrkr='o', mrkrs=4):
         self.ax.scatter(points, values, color=clr, marker=mrkr, s=mrkrs)
 
 class Plotter3D(Plotter):
-    def __init__(self, parametersInNDProblem, leftBounds, rightBounds, objFunc, plotterType):
+    def __init__(self, parameters_in_nd_problem, left_bounds, right_bounds, obj_func, plotter_type):
         plt.style.use('fivethirtyeight')
         plt.rcParams['contour.negative_linestyle'] = 'solid'
         plt.rcParams["figure.figsize"] = (8, 6)
 
-        self.indexes = parametersInNDProblem
-        self.leftBounds = leftBounds
-        self.rightBounds = rightBounds
-        self.objFunc = objFunc
+        self.indexes = parameters_in_nd_problem
+        self.leftBounds = left_bounds
+        self.rightBounds = right_bounds
+        self.objFunc = obj_func
 
-        self.plotterType = plotterType
+        self.plotterType = plotter_type
 
         self.fig = plt.subplot()
         if self.plotterType == 'surface':
             self.ax = plt.subplot(projection='3d')
         elif self.plotterType == 'lines layers':
             self.ax = plt.subplot()
         self.ax.set_xlim([self.leftBounds[0], self.rightBounds[0]])
         self.ax.set_ylim([self.leftBounds[1], self.rightBounds[1]])
         self.ax.tick_params(axis='both', labelsize=8)
 
-    def PlotByGrid(self, calculate, section, pointsCount=100):
-        x1 = np.arange(self.leftBounds[0], self.rightBounds[0], (self.rightBounds[0] - self.leftBounds[0]) / pointsCount)
-        x2 = np.arange(self.leftBounds[1], self.rightBounds[1], (self.rightBounds[1] - self.leftBounds[1]) / pointsCount)
+    def plot_by_grid(self, calculate, section, points_count=100):
+        x1 = np.arange(self.leftBounds[0], self.rightBounds[0], (self.rightBounds[0] - self.leftBounds[0]) / points_count)
+        x2 = np.arange(self.leftBounds[1], self.rightBounds[1], (self.rightBounds[1] - self.leftBounds[1]) / points_count)
         xv, yv = np.meshgrid(x1, x2)
         z = []
 
-        for i in range(pointsCount):
+        for i in range(points_count):
             z_ = []
-            for j in range(pointsCount):
+            for j in range(points_count):
                 section[self.indexes[0]] = xv[i, j]
                 section[self.indexes[1]] = yv[i, j]
                 z_.append(calculate(section))
             z.append(z_)
 
         self.ax.contour(x1, x2, z, linewidths=1, levels=25, cmap=plt.cm.viridis)
 
-    def PlotApproximation(self, points, values, pointsCount=100):
+    def plot_approximation(self, points, values, points_count=100):
         nn = MLPRegressor(activation='logistic',  # can be tanh, identity, logistic, relu
                           solver='lbfgs',  # can be lbfgs, sgd , adam
                           alpha=0.001,
                           hidden_layer_sizes=(40,),
                           max_iter=10000,
                           tol=10e-6,
                           random_state=10)
 
         nn.fit(points, values)
-        x1 = np.linspace(self.leftBounds[0], self.rightBounds[0], pointsCount)
-        x2 = np.linspace(self.leftBounds[1], self.rightBounds[1], pointsCount)
+        x1 = np.linspace(self.leftBounds[0], self.rightBounds[0], points_count)
+        x2 = np.linspace(self.leftBounds[1], self.rightBounds[1], points_count)
         x1, x2 = np.meshgrid(x1, x2)
 
         # np.c - cлияние осей X и Y в точки
         # ravel - развернуть (к одномерному массиву)
         xy = np.c_[x1.ravel(), x2.ravel()]
 
         # делаем предсказание значений
         z = nn.predict(xy)
-        z = z.reshape(pointsCount, pointsCount)
+        z = z.reshape(points_count, points_count)
 
         # полученная аппроксимация
         self.ax.plot_surface(x1, x2, z, cmap=plt.cm.viridis, alpha=0.6)
 
-    def PlotInterpolation(self, points, values, pointsCount=100):
+    def plot_interpolation(self, points, values, points_count=100):
         if self.plotterType == 'lines layers':
             interp = interpolate.Rbf(np.array(points)[:, 0], np.array(points)[:, 1], values)
-            x1 = np.linspace(self.leftBounds[0], self.rightBounds[0], pointsCount)
-            x2 = np.linspace(self.leftBounds[1], self.rightBounds[1], pointsCount)
+            x1 = np.linspace(self.leftBounds[0], self.rightBounds[0], points_count)
+            x2 = np.linspace(self.leftBounds[1], self.rightBounds[1], points_count)
             x1, x2 = np.meshgrid(x1, x2)
             z = interp(x1, x2)
             self.ax.contour(x1, x2, z, linewidths=1, cmap=plt.cm.viridis)
         elif self.plotterType == 'surface':
             interp = interpolate.Rbf(np.array(points)[:, 0], np.array(points)[:, 1], values)
-            x1 = np.linspace(self.leftBounds[0], self.rightBounds[0], pointsCount)
-            x2 = np.linspace(self.leftBounds[1], self.rightBounds[1], pointsCount)
+            x1 = np.linspace(self.leftBounds[0], self.rightBounds[0], points_count)
+            x2 = np.linspace(self.leftBounds[1], self.rightBounds[1], points_count)
             x1, x2 = np.meshgrid(x1, x2)
             z = interp(x1, x2)
             self.ax.plot_surface(x1, x2, z, cmap=plt.cm.viridis, alpha=0.6)
 
-    def PlotPoints(self, points, values, clr='blue', mrkr='o', mrkrs=3):
+    def plot_points(self, points, values, clr='blue', mrkr='o', mrkrs=3):
         if self.plotterType == 'lines layers':
             self.ax.scatter(np.array(points)[:, 0], np.array(points)[:, 1], color=clr, marker=mrkr, s=mrkrs)
         elif self.plotterType == 'surface':
             self.ax.scatter(np.array(points)[:, 0], np.array(points)[:, 1], values, s=mrkrs, color=clr, marker=mrkr, alpha=1.0)
 
 class AnimatePlotter2D(Plotter2D):
-    def __init__(self, parametersInNDProblem, leftBounds, rightBounds, objFunc=None, plotterType='lines layers'):
+    def __init__(self, parameters_in_nd_problem, left_bounds, right_bounds, obj_func=None,
+                 plotter_type='lines layers'):
         plt.ion()
         plt.style.use('fivethirtyeight')
         plt.rcParams['contour.negative_linestyle'] = 'solid'
         plt.rcParams["figure.figsize"] = (8, 6)
 
-        self.index = parametersInNDProblem
+        self.index = parameters_in_nd_problem
         self.leftBound = 0
         self.rightBound = 0
-        self.objFunc = objFunc
+        self.objFunc = obj_func
 
-        self.plotterType = plotterType
+        self.plotterType = plotter_type
 
         self.fig, self.ax = plt.subplots()
         self.ax.tick_params(axis='both', labelsize=8)
         self.ax.set_autoscaley_on(True)
 
-    def SetBounds(self, leftBound, rightBound):
-        self.leftBound = leftBound
-        self.rightBound = rightBound
+    def set_bounds(self, left_bound, right_bound):
+        self.leftBound = left_bound
+        self.rightBound = right_bound
 
         self.ax.set_xlim(self.leftBound, self.rightBound)
 
-    def PlotPoints(self, points, values, clr='blue', mrkr='o', mrkrs=4):
+    def plot_points(self, points, values, clr='blue', mrkr='o', mrkrs=4):
         self.ax.plot(points[0], values[0], color=clr, marker=mrkr, markersize=mrkrs)
         self.ax.relim()
         self.ax.autoscale_view()
         self.fig.canvas.draw()
         self.fig.canvas.flush_events()
 
 
 class AnimatePlotter3D(Plotter3D):
-    def __init__(self, parametersInNDProblem, objFunc=None, plotterType='lines layers'):
+    def __init__(self, parameters_in_nd_problem, obj_func=None, plotter_type='lines layers'):
         plt.ion()
         plt.style.use('fivethirtyeight')
         plt.rcParams['contour.negative_linestyle'] = 'solid'
         plt.rcParams["figure.figsize"] = (8, 6)
 
-        self.indexes = parametersInNDProblem
+        self.indexes = parameters_in_nd_problem
         self.leftBounds = [0, 0]
         self.rightBounds = [1, 1]
         self.objFunc = None
 
         self.fig, self.ax = plt.subplots()
 
         self.ax.tick_params(axis='both', labelsize=8)
         self.ax.set_autoscaley_on(True)
 
-    def SetBounds(self, leftBounds, rightBounds):
-        self.leftBounds = leftBounds
-        self.rightBounds = rightBounds
+    def set_bounds(self, left_bounds, right_bounds):
+        self.leftBounds = left_bounds
+        self.rightBounds = right_bounds
 
         self.ax.set_xlim(self.leftBounds[0], self.rightBounds[0])
         self.ax.set_ylim(self.leftBounds[1], self.rightBounds[1])
 
-    def PlotPoints(self, points, values, clr='blue', mrkr='o', mrkrs=4):
+    def plot_points(self, points, values, clr='blue', mrkr='o', mrkrs=4):
         self.ax.scatter(points[0], points[1], color=clr, marker=mrkr, s=mrkrs)
         self.ax.relim()
         self.ax.autoscale_view()
         self.fig.canvas.draw()
         self.fig.canvas.flush_events()
```

### Comparing `iOpt-0.2.1/iOpt/output_system/painters/static_painters.py` & `iOpt-0.2.22/iOpt/output_system/painters/static_painters.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,267 +6,268 @@
 from iOpt.output_system.painters.plotters.plotters import Plotter2D, Plotter3D, DisretePlotter
 from iOpt.output_system.painters.painter import Painter
 
 import matplotlib.pyplot as plt
 import os
 
 class DiscretePainter(Painter):
-    def __init__(self, searchDataSorted, bestsvalues, pcount, floatdim, optimumPoint, discreteValues,
-                 discreteName, mode, calc, subparameters, lb, rb, fileName, pathForSaves, calculate, optimumValue, searchData, numberOfParallelPoints):
-        self.pathForSaves = pathForSaves
-        self.fileName = fileName
+    def __init__(self, search_data_sorted, bestsvalues, pcount, floatdim, optimumPoint, discreteValues,
+                 discrete_name, mode, calc, subparameters, lb, rb, file_name, path_for_saves, calculate,
+                 optimum_value, search_data, number_of_parallel_points):
+        self.path_for_saves = path_for_saves
+        self.file_name = file_name
         self.calc = calc
         self.calculate = calculate
         self.optimum = optimumPoint
-        self.optimumVal = optimumValue
-        self.numberOfParallelPoints = numberOfParallelPoints
+        self.optimumVal = optimum_value
+        self.number_of_parallel_points = number_of_parallel_points
 
         self.values = []
         self.points = []
 
         self.combination = []
 
         self.pointsWithBestComb = [[], []]
         self.otherPoints = [[], []]
         self.optimumPoint = [[], []]
 
         if mode == 'bestcombination':
-            for x in searchData:
-                if x.GetZ() > 1.7e+308:
+            for x in search_data:
+                if x.get_z() > 1.7e+308:
                     continue
-                if x.GetY().discreteVariables != self.optimum.discreteVariables:
+                if x.get_y().discrete_variables != self.optimum.discrete_variables:
                     if floatdim > 1:
-                        self.otherPoints[0].append(x.GetY().floatVariables[subparameters[0] - 1])
-                        self.otherPoints[1].append(x.GetY().floatVariables[subparameters[1] - 1])
+                        self.otherPoints[0].append(x.get_y().float_variables[subparameters[0] - 1])
+                        self.otherPoints[1].append(x.get_y().float_variables[subparameters[1] - 1])
                     else:
-                        self.otherPoints[0].append(x.GetY().floatVariables[0])
+                        self.otherPoints[0].append(x.get_y().float_variables[0])
                         self.otherPoints[1].append(self.optimumVal - 5)
                     continue
                 else:
                     if floatdim > 1:
                         '''
                         ok = True
                         for k in range(floatdim):
-                            if (x.GetY().floatVariables[k] != self.optimum.floatVariables[k] and
+                            if (x.GetY().float_variables[k] != self.optimum.float_variables[k] and
                             k != subparameters[0] - 1 and k != subparameters[1] - 1):
                                 ok = False
                                 break
                         if ok:
                             self.values2.append(x.GetZ())
-                            self.points2.append([x.GetY().floatVariables[subparameters[0] - 1],
-                                                 x.GetY().floatVariables[subparameters[1] - 1]])
+                            self.points2.append([x.GetY().float_variables[subparameters[0] - 1],
+                                                 x.GetY().float_variables[subparameters[1] - 1]])
                         '''
-                        self.points.append([x.GetY().floatVariables[subparameters[0] - 1],
-                                       x.GetY().floatVariables[subparameters[1] - 1]])
-                        self.values.append(x.GetZ())
-                        self.pointsWithBestComb[0].append(x.GetY().floatVariables[subparameters[0] - 1])
-                        self.pointsWithBestComb[1].append(x.GetY().floatVariables[subparameters[1] - 1])
+                        self.points.append([x.get_y().float_variables[subparameters[0] - 1],
+                                            x.get_y().float_variables[subparameters[1] - 1]])
+                        self.values.append(x.get_z())
+                        self.pointsWithBestComb[0].append(x.get_y().float_variables[subparameters[0] - 1])
+                        self.pointsWithBestComb[1].append(x.get_y().float_variables[subparameters[1] - 1])
                     else:
-                        self.points.append(x.GetY().floatVariables[0])
-                        self.values.append(x.GetZ())
-                        self.pointsWithBestComb[0].append(x.GetY().floatVariables[0])
+                        self.points.append(x.get_y().float_variables[0])
+                        self.values.append(x.get_z())
+                        self.pointsWithBestComb[0].append(x.get_y().float_variables[0])
                         self.pointsWithBestComb[1].append(self.optimumVal - 5)
 
             if floatdim > 1:
-                self.optimumPoint[0].append(self.optimum.floatVariables[subparameters[0] - 1])
-                self.optimumPoint[1].append(self.optimum.floatVariables[subparameters[1] - 1])
+                self.optimumPoint[0].append(self.optimum.float_variables[subparameters[0] - 1])
+                self.optimumPoint[1].append(self.optimum.float_variables[subparameters[1] - 1])
             else:
-                self.optimumPoint[0].append(self.optimum.floatVariables[0])
+                self.optimumPoint[0].append(self.optimum.float_variables[0])
                 self.optimumPoint[1].append(self.optimumVal - 5)
 
         elif mode == 'analysis':
             i = 0
-            for item in searchDataSorted:
+            for item in search_data_sorted:
                 i += 1
-                if item.GetZ() > 1.7e+308:
+                if item.get_z() > 1.7e+308:
                     continue
-                self.points.append(item.GetY())
-                self.values.append([item.GetZ(), i])
+                self.points.append(item.get_y())
+                self.values.append([item.get_z(), i])
                 str = '['
-                for j in range(len(item.GetY().discreteVariables)):
-                    str += item.GetY().discreteVariables[j] + ', '
+                for j in range(len(item.get_y().discrete_variables)):
+                    str += item.get_y().discrete_variables[j] + ', '
                 str = str[:-2]
                 str += ']'
                 self.combination.append([str, i])
 
-        self.plotter = DisretePlotter(mode, pcount, floatdim, discreteValues, discreteName,
-                                      subparameters, lb, rb, bestsvalues, self.numberOfParallelPoints)
+        self.plotter = DisretePlotter(mode, pcount, floatdim, discreteValues, discrete_name,
+                                      subparameters, lb, rb, bestsvalues, self.number_of_parallel_points)
 
-    def PaintObjectiveFunc(self, numpoints):
+    def paint_objective_func(self, numpoints):
         if self.calc == 'objective function':
             section = self.optimum
-            self.plotter.PlotByGrid(self.CalculateFunc, section, numpoints)
+            self.plotter.plot_by_grid(self.calculate_func, section, numpoints)
         elif self.calc == 'interpolation':
-            self.plotter.PlotInterpolation(self.points, self.values)
+            self.plotter.plot_interpolation(self.points, self.values)
 
-    def PaintPoints(self, mrks):
-        self.plotter.PlotPoints(self.pointsWithBestComb, self.otherPoints, self.optimum, self.optimumPoint, mrks)
+    def paint_points(self, mrks):
+        self.plotter.plot_points(self.pointsWithBestComb, self.otherPoints, self.optimum, self.optimumPoint, mrks)
 
-    def PaintAnalisys(self, mrks):
-        self.plotter.PlotAnalisysSubplotsFigure(self.points, self.values,  self.combination, self.optimum, mrks)
-    def PaintOptimum(self, solution: Solution = None):
+    def paint_analisys(self, mrks):
+        self.plotter.plot_analisys_subplots_figure(self.points, self.values, self.combination, self.optimum, mrks)
+    def paint_optimum(self, solution: Solution = None):
         pass
 
-    def SaveImage(self):
-        if not os.path.isdir(self.pathForSaves):
-            if self.pathForSaves == "":
-                plt.savefig(self.fileName)
+    def save_image(self):
+        if not os.path.isdir(self.path_for_saves):
+            if self.path_for_saves == "":
+                plt.savefig(self.file_name)
             else:
-                os.mkdir(self.pathForSaves)
-                plt.savefig(self.pathForSaves + "/" + self.fileName)
+                os.mkdir(self.path_for_saves)
+                plt.savefig(self.path_for_saves + "/" + self.file_name)
         else:
-            plt.savefig(self.pathForSaves + "/" + self.fileName)
+            plt.savefig(self.path_for_saves + "/" + self.file_name)
         plt.show()
 
-    def CalculateFunc(self, x, d):
+    def calculate_func(self, x, d):
         point = Point(x, d)
         fv = FunctionValue()
         fv = self.calculate(point, fv)
         return fv.value
 class StaticPainter(Painter):
-    def __init__(self, searchData: SearchData,
+    def __init__(self, search_data: SearchData,
                  solution: Solution,
                  mode,
-                 isPointsAtBottom,
-                 parameterInNDProblem,
-                 pathForSaves,
-                 fileName
-    ):
-        self.pathForSaves = pathForSaves
-        self.fileName = fileName
+                 is_points_at_bottom,
+                 parameter_in_nd_problem,
+                 path_for_saves,
+                 file_name
+                 ):
+        self.path_for_saves = path_for_saves
+        self.file_name = file_name
 
         self.objectFunctionPainterType = mode
-        self.isPointsAtBottom = isPointsAtBottom
+        self.is_points_at_bottom = is_points_at_bottom
 
-        self.objFunc = solution.problem.Calculate
+        self.objFunc = solution.problem.calculate
 
         # формируем массив точек итераций для графика
         self.points = []
         self.values = []
 
-        for item in searchData:
-            self.points.append(item.GetY().floatVariables[parameterInNDProblem])
-            self.values.append(item.GetZ())
+        for item in search_data:
+            self.points.append(item.get_y().float_variables[parameter_in_nd_problem])
+            self.values.append(item.get_z())
 
         self.points = self.points[1:-1]
         self.values = self.values[1:-1]
 
-        self.optimum = solution.bestTrials[0].point.floatVariables
-        self.optimumC = solution.bestTrials[0].point.floatVariables[parameterInNDProblem]
-        self.optimumValue = solution.bestTrials[0].functionValues[0].value
+        self.optimum = solution.best_trials[0].point.float_variables
+        self.optimumC = solution.best_trials[0].point.float_variables[parameter_in_nd_problem]
+        self.optimumValue = solution.best_trials[0].function_values[0].value
 
         # настройки графика
-        self.plotter = Plotter2D(parameterInNDProblem,
-                        float(solution.problem.lowerBoundOfFloatVariables[parameterInNDProblem]),
-                        float(solution.problem.upperBoundOfFloatVariables[parameterInNDProblem]))
+        self.plotter = Plotter2D(parameter_in_nd_problem,
+                                 float(solution.problem.lower_bound_of_float_variables[parameter_in_nd_problem]),
+                                 float(solution.problem.upper_bound_of_float_variables[parameter_in_nd_problem]))
 
-    def PaintObjectiveFunc(self):
+    def paint_objective_func(self):
         if self.objectFunctionPainterType == 'objective function':
             section = self.optimum.copy()
-            self.plotter.PlotByGrid(self.CalculateFunc, section, pointsCount=150)
+            self.plotter.plot_by_grid(self.calculate_func, section, points_count=150)
         elif self.objectFunctionPainterType == 'approximation':
-            self.plotter.PlotApproximation(self.points, self.values, pointsCount=100)
+            self.plotter.plot_approximation(self.points, self.values, points_count=100)
         elif self.objectFunctionPainterType == 'interpolation':
-            self.plotter.PlotInterpolation(self.points, self.values, pointsCount=100)
+            self.plotter.plot_interpolation(self.points, self.values, points_count=100)
         elif self.objectFunctionPainterType == 'only points':
             pass
 
-    def PaintPoints(self, currPoint: SearchDataItem = None):
-        if self.isPointsAtBottom:
+    def paint_points(self, curr_point: SearchDataItem = None):
+        if self.is_points_at_bottom:
             values = [self.optimumValue - (max(self.values) - min(self.values)) * 0.3] * len(self.values)
-            self.plotter.PlotPoints(self.points, values, 'blue', 'o', 4)
+            self.plotter.plot_points(self.points, values, 'blue', 'o', 4)
         else:
-            self.plotter.PlotPoints(self.points, self.values, 'blue', 'o', 4)
+            self.plotter.plot_points(self.points, self.values, 'blue', 'o', 4)
 
-    def PaintOptimum(self, solution: Solution = None):
+    def paint_optimum(self, solution: Solution = None):
         value = self.optimumValue
-        if self.isPointsAtBottom:
+        if self.is_points_at_bottom:
             value = value - (max(self.values) - min(self.values)) * 0.3
-        self.plotter.PlotPoints([self.optimumC], [value], 'red', 'o', 4)
+        self.plotter.plot_points([self.optimumC], [value], 'red', 'o', 4)
 
-    def SaveImage(self):
-        if not os.path.isdir(self.pathForSaves):
-            if self.pathForSaves == "":
-                plt.savefig(self.fileName)
+    def save_image(self):
+        if not os.path.isdir(self.path_for_saves):
+            if self.path_for_saves == "":
+                plt.savefig(self.file_name)
             else:
-                os.mkdir(self.pathForSaves)
-                plt.savefig(self.pathForSaves + "/" + self.fileName)
+                os.mkdir(self.path_for_saves)
+                plt.savefig(self.path_for_saves + "/" + self.file_name)
         else:
-            plt.savefig(self.pathForSaves + "/" + self.fileName)
+            plt.savefig(self.path_for_saves + "/" + self.file_name)
         plt.show()
 
-    def CalculateFunc(self, x):
+    def calculate_func(self, x):
         point = Point(x)
         fv = FunctionValue()
         fv = self.objFunc(point, fv)
         return fv.value
 
 class StaticPainterND(Painter):
-    def __init__(self, searchData, solution, parameters, mode, calc, fileName, pathForSaves):
-        self.pathForSaves = pathForSaves
-        self.fileName = fileName
+    def __init__(self, search_data, solution, parameters, mode, calc, file_name, path_for_saves):
+        self.path_for_saves = path_for_saves
+        self.file_name = file_name
 
         self.objectFunctionPainterType = mode
         self.objectFunctionCalculatorType = calc
 
-        self.objFunc = solution.problem.Calculate
+        self.objFunc = solution.problem.calculate
 
         # формируем массив точек итераций для графика
         self.points = []
         self.values = []
 
-        for item in searchData:
-            self.points.append([item.GetY().floatVariables[parameters[0]], item.GetY().floatVariables[parameters[1]]])
-            self.values.append(item.GetZ())
+        for item in search_data:
+            self.points.append([item.get_y().float_variables[parameters[0]], item.get_y().float_variables[parameters[1]]])
+            self.values.append(item.get_z())
 
         self.points = self.points[1:-1]
         self.values = self.values[1:-1]
 
-        self.optimum = solution.bestTrials[0].point.floatVariables
-        self.optimumValue = solution.bestTrials[0].functionValues[0].value
+        self.optimum = solution.best_trials[0].point.float_variables
+        self.optimumValue = solution.best_trials[0].function_values[0].value
 
-        self.leftBounds = [float(solution.problem.lowerBoundOfFloatVariables[parameters[0]]),
-                           float(solution.problem.lowerBoundOfFloatVariables[parameters[1]])]
-        self.rightBounds = [float(solution.problem.upperBoundOfFloatVariables[parameters[0]]),
-                            float(solution.problem.upperBoundOfFloatVariables[parameters[1]])]
+        self.leftBounds = [float(solution.problem.lower_bound_of_float_variables[parameters[0]]),
+                           float(solution.problem.lower_bound_of_float_variables[parameters[1]])]
+        self.rightBounds = [float(solution.problem.upper_bound_of_float_variables[parameters[0]]),
+                            float(solution.problem.upper_bound_of_float_variables[parameters[1]])]
 
         # настройки графика
-        self.plotter = Plotter3D(parameters, self.leftBounds, self.rightBounds, solution.problem.Calculate, self.objectFunctionPainterType)
+        self.plotter = Plotter3D(parameters, self.leftBounds, self.rightBounds, solution.problem.calculate, self.objectFunctionPainterType)
 
-    def PaintObjectiveFunc(self):
+    def paint_objective_func(self):
         if self.objectFunctionPainterType == 'lines layers':
             if self.objectFunctionCalculatorType == 'objective function':
-                self.plotter.PlotByGrid(self.CalculateFunc, self.optimum, pointsCount=100)
+                self.plotter.plot_by_grid(self.calculate_func, self.optimum, points_count=100)
             elif self.objectFunctionCalculatorType == 'interpolation':
-                self.plotter.PlotInterpolation(self.points, self.values, pointsCount=100)
+                self.plotter.plot_interpolation(self.points, self.values, points_count=100)
             elif self.objectFunctionCalculatorType == "approximation":
                 pass
         elif self.objectFunctionPainterType == 'surface':
             if self.objectFunctionCalculatorType == 'approximation':
-                self.plotter.PlotApproximation(self.points, self.values, pointsCount=50)
+                self.plotter.plot_approximation(self.points, self.values, points_count=50)
             elif self.objectFunctionCalculatorType == 'interpolation':
-                self.plotter.PlotInterpolation(self.points, self.values, pointsCount=50)
+                self.plotter.plot_interpolation(self.points, self.values, points_count=50)
             elif self.objectFunctionCalculatorType == "objective function":
                 pass
 
-    def PaintPoints(self, currPoint: SearchDataItem = None):
-        self.plotter.PlotPoints(self.points, self.values, 'blue', 'o', 4)
+    def paint_points(self, curr_point: SearchDataItem = None):
+        self.plotter.plot_points(self.points, self.values, 'blue', 'o', 4)
 
-    def PaintOptimum(self, solution: Solution = None):
-        self.plotter.PlotPoints([self.optimum], [self.optimumValue], 'red', 'o', 4)
+    def paint_optimum(self, solution: Solution = None):
+        self.plotter.plot_points([self.optimum], [self.optimumValue], 'red', 'o', 4)
 
-    def SaveImage(self):
-        if not os.path.isdir(self.pathForSaves):
-            if self.pathForSaves == "":
-                plt.savefig(self.fileName)
+    def save_image(self):
+        if not os.path.isdir(self.path_for_saves):
+            if self.path_for_saves == "":
+                plt.savefig(self.file_name)
             else:
-                os.mkdir(self.pathForSaves)
-                plt.savefig(self.pathForSaves + "/" + self.fileName)
+                os.mkdir(self.path_for_saves)
+                plt.savefig(self.path_for_saves + "/" + self.file_name)
         else:
-            plt.savefig(self.pathForSaves + "/" + self.fileName)
+            plt.savefig(self.path_for_saves + "/" + self.file_name)
         plt.show()
 
-    def CalculateFunc(self, x):
+    def calculate_func(self, x):
         point = Point(x, [])
         fv = FunctionValue()
         fv = self.objFunc(point, fv)
         return fv.value
```

### Comparing `iOpt-0.2.1/iOpt/problem.py` & `iOpt-0.2.22/iOpt/problem.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 
 class Problem(ABC):
     """Базовый класс для задач оптимизации"""
 
     def __init__(self):
         self.name: str = ''
         self.dimension = 0
-        self.numberOfFloatVariables: int = 0
-        self.numberOfDiscreteVariables: int = 0
-        self.numberOfObjectives: int = 0
-        self.numberOfConstraints: int = 0
-
-        self.floatVariableNames: np.ndarray(shape=(1), dtype=str) = []
-        self.discreteVariableNames: np.ndarray(shape=(1), dtype=str) = []
-
-        self.lowerBoundOfFloatVariables: np.ndarray(shape=(1), dtype=np.double) = []
-        self.upperBoundOfFloatVariables: np.ndarray(shape=(1), dtype=np.double) = []
-        self.discreteVariableValues: np.ndarray(shape=(1, 1), dtype=str) = []
+        self.number_of_float_variables: int = 0
+        self.number_of_discrete_variables: int = 0
+        self.number_of_objectives: int = 0
+        self.number_of_constraints: int = 0
+
+        self.float_variable_names: np.ndarray(shape=(1), dtype=str) = []
+        self.discrete_variable_names: np.ndarray(shape=(1), dtype=str) = []
+
+        self.lower_bound_of_float_variables: np.ndarray(shape=(1), dtype=np.double) = []
+        self.upper_bound_of_float_variables: np.ndarray(shape=(1), dtype=np.double) = []
+        self.discrete_variable_values: np.ndarray(shape=(1, 1), dtype=str) = []
 
-        self.knownOptimum: np.ndarray(shape=(1), dtype=Trial) = []
+        self.known_optimum: np.ndarray(shape=(1), dtype=Trial) = []
 
     @abstractmethod
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Метод вычисления функции в заданной точке.
           Для любой новой постановки задачи, которая наследуется от :class:`Problem`, этот метод следует перегрузить.
 
         :return: Вычисленное значение функции."""
         pass
 
-   # @abstractmethod
-    def GetName(self):
+    # @abstractmethod
+    def get_name(self):
         """
         Метод позволяет получить имя задачи
 
         :return: self.name."""
         return self.name
-        #pass
+        # pass
```

### Comparing `iOpt-0.2.1/iOpt/routine/timeout.py` & `iOpt-0.2.22/iOpt/routine/timeout.py`

 * *Files identical despite different names*

### Comparing `iOpt-0.2.1/iOpt/solution.py` & `iOpt-0.2.22/iOpt/solution.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 
 class Solution:
     """
     Класс описания решения задачи оптимизации
     """
     def __init__(self,
                  problem: Problem,
-                 bestTrials: np.ndarray(shape=(1), dtype=Trial) = [Trial([], [])],
-
-                 numberOfGlobalTrials: int = 1,
-                 numberOfLocalTrials: int = 0,
-                 solvingTime: np.double = 0.0,
-                 solutionAccuracy: np.double = 0.0
+                 best_trials: np.ndarray(shape=(1), dtype=Trial) = [Trial([], [])],
+                 number_of_global_trials: int = 1,
+                 number_of_local_trials: int = 0,
+                 solving_time: np.double = 0.0,
+                 solution_accuracy: np.double = 0.0
                  ):
         """
         Конструктор класса
 
         :param problem: Задача оптимизации
-        :param bestTrials: Решение задачи оптимизации
-        :param numberOfGlobalTrials: Число выполненных глобальных итераций поиска
-        :param numberOfLocalTrials: Число выполненных локальных итераций поиска
-        :param solvingTime: Время решения задачи
-        :param solutionAccuracy: Точность найденного решения
+        :param best_trials: Решение задачи оптимизации
+        :param number_of_global_trials: Число выполненных глобальных итераций поиска
+        :param number_of_local_trials: Число выполненных локальных итераций поиска
+        :param solving_time: Время решения задачи
+        :param solution_accuracy: Точность найденного решения
         """
 
         self.problem = problem
-        self.bestTrials = bestTrials
+        self.best_trials = best_trials
 
-        self.numberOfGlobalTrials = numberOfGlobalTrials
-        self.numberOfLocalTrials = numberOfLocalTrials
-        self.solvingTime = solvingTime
-        self.solutionAccuracy = solutionAccuracy
+        self.number_of_global_trials = number_of_global_trials
+        self.number_of_local_trials = number_of_local_trials
+        self.solving_time = solving_time
+        self.solution_accuracy = solution_accuracy
```

### Comparing `iOpt-0.2.1/iOpt/solver.py` & `iOpt-0.2.22/iOpt/solver.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,168 +28,173 @@
         :param problem: Постановка задачи оптимизации
         :param parameters: Параметры поиска оптимальных решений
         """
 
         self.problem = problem
         self.parameters = parameters
 
-        Solver.ChackParameters(self.problem, self.parameters)
+        Solver.check_parameters(self.problem, self.parameters)
 
         self.__listeners: List[Listener] = []
 
-        self.searchData = SearchData(problem)
-        self.evolvent = Evolvent(problem.lowerBoundOfFloatVariables, problem.upperBoundOfFloatVariables,
-                                 problem.numberOfFloatVariables)
+        self.search_data = SearchData(problem)
+        self.evolvent = Evolvent(problem.lower_bound_of_float_variables, problem.upper_bound_of_float_variables,
+                                 problem.number_of_float_variables)
         self.task = OptimizationTask(problem)
-        self.method = SolverFactory.CreateMethod(parameters, self.task, self.evolvent, self.searchData)
-        self.process = SolverFactory.CreateProcess(parameters=parameters, task=self.task, evolvent=self.evolvent,
-                                                   searchData=self.searchData, method=self.method,
-                                                   listeners=self.__listeners)
+        self.method = SolverFactory.create_method(parameters, self.task, self.evolvent, self.search_data)
+        self.process = SolverFactory.create_process(parameters=parameters, task=self.task, evolvent=self.evolvent,
+                                                    search_data=self.search_data, method=self.method,
+                                                    listeners=self.__listeners)
 
-    def Solve(self) -> Solution:
+    def solve(self) -> Solution:
         """
         Метод позволяет решить задачу оптимизации. Остановка поиска выполняется согласно критерию,
         заданному при создании класса Solver.
 
         :return: решение задачи оптимизации
         """
-        Solver.ChackParameters(self.problem, self.parameters)
-        sol: Solution = None;
+        Solver.check_parameters(self.problem, self.parameters)
         if self.parameters.timeout < 0:
-            sol = self.process.Solve()
+            sol = self.process.solve()
         else:
-            solv_with_timeout = timeout(seconds=self.parameters.timeout * 60)(self.process.Solve)
+            solv_with_timeout = timeout(seconds=self.parameters.timeout * 60)(self.process.solve)
             try:
                 solv_with_timeout()
+                sol = self.get_results()
             except Exception as exc:
                 print(exc)
-                sol = self.GetResults()
-                sol.solvingTime = self.parameters.timeout * 60
+                sol = self.get_results()
+                sol.solving_time = self.parameters.timeout * 60
                 self.method.recalcR = True
                 self.method.recalcM = True
-                status = self.method.CheckStopCondition()
+                status = self.method.check_stop_condition()
                 for listener in self.__listeners:
-                    listener.OnMethodStop(self.searchData, self.GetResults(), status)
+                    listener.on_method_stop(self.search_data, self.get_results(), status)
         return sol
 
-    def DoGlobalIteration(self, number: int = 1):
+    def do_global_iteration(self, number: int = 1):
         """
         Метод позволяет выполнить несколько итераций глобального поиска
 
         :param number: число итераций глобального поиска
         """
-        Solver.ChackParameters(self.problem, self.parameters)
-        self.process.DoGlobalIteration(number)
+        Solver.check_parameters(self.problem, self.parameters)
+        self.process.do_global_iteration(number)
 
-    def DoLocalRefinement(self, number: int = 1):
+    def do_local_refinement(self, number: int = 1):
         """
         Метод позволяет выполнить несколько итераций локального поиска
 
         :param number: число итераций локального поиска
         """
-        Solver.ChackParameters(self.problem, self.parameters)
-        self.process.DoLocalRefinement(number)
+        Solver.check_parameters(self.problem, self.parameters)
+        self.process.do_local_refinement(number)
 
-    def GetResults(self) -> Solution:
+    def get_results(self) -> Solution:
         """
         Метод позволяет получить текущую оценку решения задачи оптимизации
 
         :return: решение задачи оптимизации
         """
-        return self.process.GetResults()
+        return self.process.get_results()
 
-    def SaveProgress(self, fileName: str) -> None:
+    def save_progress(self, file_name: str) -> None:
         """
         Сохранение процесса оптимизации в файл
 
-        :param fileName: имя файла
+        :param file_name: имя файла
         """
-        self.process.SaveProgress(fileName=fileName)
+        self.process.save_progress(file_name=file_name)
 
-    def LoadProgress(self, fileName: str) -> None:
+    def load_progress(self, file_name: str) -> None:
         """
         Загрузка процесса оптимизации из файла
 
-        :param fileName: имя файла
+        :param file_name: имя файла
         """
-        Solver.ChackParameters(self.problem, self.parameters)
-        self.process.LoadProgress(fileName=fileName)
+        Solver.check_parameters(self.problem, self.parameters)
+        self.process.load_progress(file_name=file_name)
 
-    def RefreshListener(self) -> None:
+        if (self.problem.number_of_discrete_variables > 0):
+            self.process.method.iterations_count = self.process.search_data.get_count() - (len(self.method.GetDiscreteParameters(self.problem)) + 1 ) #-2
+        else: self.process.method.iterations_count = self.process.search_data.get_count() - 2
+
+    def refresh_listener(self) -> None:
         """
         Метод оповещения наблюдателей о произошедшем событии
         """
 
         pass
 
-    def AddListener(self, listener: Listener) -> None:
+    def add_listener(self, listener: Listener) -> None:
         """
         Добавления наблюдателя за процессом оптимизации
 
         :param listener: объект класса реализующий методы наблюдения
         """
 
         self.__listeners.append(listener)
 
     @staticmethod
-    def ChackParameters(problem: Problem,
-                        parameters: SolverParameters = SolverParameters()) -> None:
+    def check_parameters(problem: Problem,
+                         parameters: SolverParameters = SolverParameters()) -> None:
         """
         Проверяет параметры решателя
 
         :param problem: Постановка задачи оптимизации
         :param parameters: Параметры поиска оптимальных решений
 
         """
 
         if parameters.eps <= 0:
             raise Exception("search precision is incorrect, parameters.eps <= 0")
         if parameters.r <= 1:
             raise Exception("The reliability parameter should be greater 1. r>1")
-        if parameters.itersLimit < 1:
-            raise Exception("The number of iterations must not be negative. itersLimit>0")
-        if parameters.evolventDensity < 2 or parameters.evolventDensity > 20:
+        if parameters.iters_limit < 1:
+            raise Exception("The number of iterations must not be negative. iters_limit>0")
+        if parameters.evolvent_density < 2 or parameters.evolvent_density > 20:
             raise Exception("Evolvent density should be within [2,20]")
-        if parameters.epsR < 0 or parameters.epsR >= 1:
+        if parameters.eps_r < 0 or parameters.eps_r >= 1:
             raise Exception("The epsilon redundancy parameter must be within [0, 1)")
 
-        if problem.numberOfFloatVariables < 1:
+        if problem.number_of_float_variables < 1:
             raise Exception("Must have at least one float variable")
-        if problem.numberOfDiscreteVariables < 0:
+        if problem.number_of_discrete_variables < 0:
             raise Exception("The number of discrete parameters must not be negative")
-        if problem.numberOfObjectives < 1:
+        if problem.number_of_objectives < 1:
             raise Exception("At least one criterion must be defined")
-        if problem.numberOfConstraints < 0:
+        if problem.number_of_constraints < 0:
             raise Exception("The number of сonstraints must not be negative")
 
-        if len(problem.floatVariableNames) != problem.numberOfFloatVariables:
+        if len(problem.float_variable_names) != problem.number_of_float_variables:
             raise Exception("Floaf parameter names are not defined")
 
-        if len(problem.lowerBoundOfFloatVariables) != problem.numberOfFloatVariables:
+        if len(problem.lower_bound_of_float_variables) != problem.number_of_float_variables:
             raise Exception("List of lower bounds for float search variables defined incorrectly")
-        if len(problem.upperBoundOfFloatVariables) != problem.numberOfFloatVariables:
+        if len(problem.upper_bound_of_float_variables) != problem.number_of_float_variables:
             raise Exception("List of upper bounds for float search variables defined incorrectly")
 
-        for lowerBound, upperBound in zip(problem.lowerBoundOfFloatVariables, problem.upperBoundOfFloatVariables):
-            if lowerBound >= upperBound:
+        for lower_bound, upper_bound in zip(problem.lower_bound_of_float_variables,
+                                            problem.upper_bound_of_float_variables):
+            if lower_bound >= upper_bound:
                 raise Exception("For floating point search variables, "
                                 "the upper search bound must be greater than the lower.")
 
-        if problem.numberOfDiscreteVariables > 0:
-            if len(problem.discreteVariableNames) != problem.numberOfDiscreteVariables:
+        if problem.number_of_discrete_variables > 0:
+            if len(problem.discrete_variable_names) != problem.number_of_discrete_variables:
                 raise Exception("Discrete parameter names are not defined")
 
-            for discreteValues in problem.discreteVariableValues:
+            for discreteValues in problem.discrete_variable_values:
                 if len(discreteValues) < 1:
                     raise Exception("Discrete variable values not defined")
 
-        if parameters.startPoint:
-            if len(parameters.startPoint.floatVariables) != problem.numberOfFloatVariables:
+        if parameters.start_point:
+            if len(parameters.start_point.float_variables) != problem.number_of_float_variables:
                 raise Exception("Incorrect start point size")
-            if parameters.startPoint.discreteVariables:
-                if len(parameters.startPoint.discreteVariables) != problem.numberOfDiscreteVariables:
+            if parameters.start_point.discrete_variables:
+                if len(parameters.start_point.discrete_variables) != problem.number_of_discrete_variables:
                     raise Exception("Incorrect start point discrete variables")
-            for lowerBound, upperBound, y in zip(problem.lowerBoundOfFloatVariables, problem.upperBoundOfFloatVariables,
-                                                 parameters.startPoint.floatVariables):
-                if y < lowerBound or y > upperBound:
+            for lower_bound, upper_bound, y in zip(problem.lower_bound_of_float_variables,
+                                                   problem.upper_bound_of_float_variables,
+                                                   parameters.start_point.float_variables):
+                if y < lower_bound or y > upper_bound:
                     raise Exception("Incorrect start point coordinate")
-
```

### Comparing `iOpt-0.2.1/iOpt/trial.py` & `iOpt-0.2.22/iOpt/trial.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 class FunctionType(Enum):
     OBJECTIV = 1
     CONSTRAINT = 2
 
 
 class Point:
     def __init__(self,
-                 floatVariables: np.ndarray(shape=(1), dtype=np.double),
-                 discreteVariables: np.ndarray(shape=(1), dtype=str)=None,
+                 float_variables: np.ndarray(shape=(1), dtype=np.double),
+                 discrete_variables: np.ndarray(shape=(1), dtype=str) = None,
                  ):
-        self.floatVariables = floatVariables
-        self.discreteVariables = discreteVariables
+        self.float_variables = float_variables
+        self.discrete_variables = discrete_variables
 
 
 class FunctionValue:
     def __init__(self,
                  type: FunctionType = FunctionType.OBJECTIV,
                  functionID: int = 0
                  ):
@@ -25,11 +25,11 @@
         self.functionID = functionID
         self.value: np.double = 0.0
 
 
 class Trial:
     def __init__(self,
                  point: Point,
-                 functionValues: np.ndarray(shape=(1), dtype=FunctionValue)
+                 function_values: np.ndarray(shape=(1), dtype=FunctionValue)
                  ):
         self.point = point
-        self.functionValues = functionValues
+        self.function_values = function_values
```

### Comparing `iOpt-0.2.1/iOpt.egg-info/PKG-INFO` & `iOpt-0.2.22/iOpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iOpt
-Version: 0.2.1
+Version: 0.2.22
 Summary: Фреймворк для автоматического выбора значений параметров для математических моделей, ИИ и МО.
 Home-page: https://github.com/aimclub/iOpt
 Author: UNN Team
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -102,35 +102,34 @@
 
 from subprocess import Popen, PIPE, STDOUT
 
 if __name__ == "__main__":
     """
     Minimization of the Rastrigin test function with visualization
     """
-    #Create a test task
+    # Create a test task
     problem = Rastrigin(2)
-    #Setup a solver options
-    params = SolverParameters(r=2.5, eps=0.01, itersLimit=300, refineSolution=True)
-    #Create the solver
+    # Setup a solver options
+    params = SolverParameters(r=2.5, eps=0.01, iters_limit=300, refine_solution=True)
+    # Create the solver
     solver = Solver(problem, parameters=params)
-    #Print results to console while solving
+    # Print results to console while solving
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
-    #3D visualization at the end of the solution
-    spl = StaticPainterNDListener("rastrigin.png", "output", varsIndxs=[0,1], mode="surface", calc="interpolation")
-    solver.AddListener(spl)
-    #Run problem solution
-    sol = solver.Solve()
+    solver.add_listener(cfol)
+    # 3D visualization at the end of the solution
+    spl = StaticPainterNDListener("rastrigin.png", "output", vars_indxs=[0, 1], mode="surface", calc="interpolation")
+    solver.add_listener(spl)
+    # Run problem solution
+    sol = solver.solve()
 ```
 
 # **Examples**
 
 Let’s demonstrate the use of the iOpt framework when tuning the hyperparameters of one of the machine learning methods. In the support vector machine ([SVC](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)), we find the optimal hyperparameters (the regularization parameter **C**, the kernel coefficient **gamma**) in the problem of breast cancer classification ([detailed description of the data](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))).
 
-
 ```python
 import numpy as np
 from sklearn.utils import shuffle
 from sklearn.datasets import load_breast_cancer
 
 from iOpt.output_system.listeners.static_painters import StaticPainterNDListener
 from iOpt.output_system.listeners.animate_painters import AnimatePainterNDListener
@@ -150,27 +149,27 @@
 if __name__ == "__main__":
     x, y = load_breast_cancer_data()
     regularization_value_bound = {'low': 1, 'up': 6}
     kernel_coefficient_bound = {'low': -7, 'up': -3}
 
     problem = SVC_2d.SVC_2D(x, y, regularization_value_bound, kernel_coefficient_bound)
 
-    method_params = SolverParameters(r=np.double(3.0), itersLimit=100)
+    method_params = SolverParameters(r=np.double(3.0), iters_limit=100)
     solver = Solver(problem, parameters=method_params)
 
-    apl = AnimatePainterNDListener("svc2d_anim.png", "output", varsIndxs=[0, 1], toPaintObjFunc=False)
-    solver.AddListener(apl)
+    apl = AnimatePainterNDListener("svc2d_anim.png", "output", vars_indxs=[0, 1], to_paint_obj_func=False)
+    solver.add_listener(apl)
+
+    spl = StaticPainterNDListener("svc2d_stat.png", "output", vars_indxs=[0, 1], mode="surface", calc="interpolation")
+    solver.add_listener(spl)
 
-    spl = StaticPainterNDListener("svc2d_stat.png", "output", varsIndxs=[0, 1], mode="surface", calc="interpolation")
-    solver.AddListener(spl)
-    
     cfol = ConsoleOutputListener(mode='full')
-    solver.AddListener(cfol)
+    solver.add_listener(cfol)
 
-    solver_info = solver.Solve()
+    solver_info = solver.solve()
 
 ```
 
 # **Project Structure**
 
 The latest stable release of iOpt is in the [main](https://github.com/UNN-ITMM-Software/iOpt/tree/main) branch. The repository includes the following directories:
 - The [iOpt](https://github.com/UNN-ITMM-Software/iOpt/tree/main/iOpt) directory contains the framework core in the form of Python classes.
```

### Comparing `iOpt-0.2.1/iOpt.egg-info/SOURCES.txt` & `iOpt-0.2.22/iOpt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 iOpt/evolvent/evolvent.py
 iOpt/method/__init__.py
 iOpt/method/calculator.py
 iOpt/method/icriterion_evaluate_method.py
 iOpt/method/index_method.py
 iOpt/method/index_method_calculator.py
 iOpt/method/listener.py
+iOpt/method/local_optimizer.py
 iOpt/method/method.py
 iOpt/method/mixed_integer_method.py
 iOpt/method/optim_task.py
 iOpt/method/parallel_process.py
 iOpt/method/process.py
 iOpt/method/search_data.py
 iOpt/method/sol_value.py
```

### Comparing `iOpt-0.2.1/problems/GKLS.py` & `iOpt-0.2.22/problems/GKLS.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
         :param dimension: Размерность задачи, :math:`2 <= dimension <= 5`
         :param functionNumber: номер задачи в наборе, :math:`1 <= functionNumber <= 100`
         """
         super(GKLS, self).__init__()
         self.dimension = dimension
         self.name = "GKLS"
-        self.numberOfFloatVariables = dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        self.number_of_float_variables = dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
 
-        self.floatVariableNames = [str(x) for x in range(self.dimension)]
+        self.float_variable_names = [str(x) for x in range(self.dimension)]
 
-        self.lowerBoundOfFloatVariables = dimension * [-1]
-        self.upperBoundOfFloatVariables = dimension * [1]
+        self.lower_bound_of_float_variables = dimension * [-1]
+        self.upper_bound_of_float_variables = dimension * [1]
 
         self.function: GKLSFunction = GKLSFunction()
 
         self.mMaxDimension: int = 5
         self.mMinDimension: int = 2
 
         self.function_number: int = functionNumber
@@ -57,20 +57,20 @@
         self.function.SetFunctionNumber(self.function_number)
 
         KOfunV = FunctionValue()
         KOfunV.value = self.function.GetOptimumValue()
 
         KOpoint = Point(self.function.GetOptimumPoint(), [])
 
-        self.knownOptimum = [Trial(KOpoint, [KOfunV])]
+        self.known_optimum = [Trial(KOpoint, [KOfunV])]
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения функции в заданной точке
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
 
         :return: Вычисленное значение функции в точке point
         """
-        functionValue.value = self.function.Calculate(point.floatVariables)
-        return functionValue
+        function_value.value = self.function.Calculate(point.float_variables)
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/GKLS_function/gkls_function.py` & `iOpt-0.2.22/problems/GKLS_function/gkls_function.py`

 * *Files identical despite different names*

### Comparing `iOpt-0.2.1/problems/GKLS_function/gkls_random.py` & `iOpt-0.2.22/problems/GKLS_function/gkls_random.py`

 * *Files identical despite different names*

### Comparing `iOpt-0.2.1/problems/Hill/hill_generation.py` & `iOpt-0.2.22/problems/Hill/hill_generation.py`

 * *Files identical despite different names*

### Comparing `iOpt-0.2.1/problems/Shekel/shekel_generation.py` & `iOpt-0.2.22/problems/Shekel/shekel_generation.py`

 * *Files identical despite different names*

### Comparing `iOpt-0.2.1/problems/g2c.py` & `iOpt-0.2.22/problems/g2c.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,56 +11,56 @@
     def __init__(self):
         """
         Конструктор класса gC2 problem.
         """
         super(g2c, self).__init__()
         self.name = "g2c"
         self.dimension: int = 20
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 2
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 2
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(0)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables.fill(10)
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(0)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables.fill(10)
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
         # Optimum is UNDEFINED
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
         result: np.double = 0
-        x = point.floatVariables
+        x = point.float_variables
         sum1 = 0
         sum2 = 0
         prod = 1
 
-        if functionValue.type == FunctionType.OBJECTIV:
+        if function_value.type == FunctionType.OBJECTIV:
             for i in range(0, self.dimension):
                 sum1 += pow(math.cos(x[i]), 4)
                 sum2 += (i + 1) * pow(x[i], 2)
                 prod = prod * pow(x[i], 2)
             result = - abs((sum1 - 2 * prod) / math.sqrt(sum2))
-        elif functionValue.functionID == 0:  # constraint 1
+        elif function_value.functionID == 0:  # constraint 1
             for i in range(0, self.dimension):
                 prod = prod * x[i]
             result = np.double(-prod + 0.75)
-        elif functionValue.functionID == 1:  # constraint 2
+        elif function_value.functionID == 1:  # constraint 2
             for i in range(0, self.dimension):
                 sum1 += x[i]
             result = np.double(sum1 - 7.5*self.dimension)
 
-        functionValue.value = result
-        return functionValue
+        function_value.value = result
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/g8c.py` & `iOpt-0.2.22/problems/romeijn3c.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,70 @@
 import numpy as np
 from iOpt.trial import FunctionType
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
-import math
 
+a = np.array([0.5, 0.25, 1.0, 1.0 / 12.0, 2])
+c = np.array([0.125, 0.25, 0.1, 0.2, 1.0 / 12.0])
+p = np.array([[0, 5], [2, 5], [3, 2], [4, 4], [5, 1]])
 
-class g8c(Problem):
+
+class Romeijn3c(Problem):
     def __init__(self):
         """
-        Конструктор класса gC8 problem.
+        Конструктор класса Romeijn3c problem.
         """
-        super(g8c, self).__init__()
-        self.name = "g8c"
+        super(Romeijn3c, self).__init__()
+        self.name = "Romeijn3c"
         self.dimension: int = 2
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 2
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 3
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(0)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables.fill(10)
+        self.lower_bound_of_float_variables = np.ndarray(shape=(1, self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables = [-3, -4]
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables = [10, 7]
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
-        pointfv = [1.2279713, 4.2453733]
+        pointfv = [-3, -4]
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
-        KOfunV[0] = self.Calculate(KOpoint, KOfunV[0])
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        KOfunV[0] = self.calculate(KOpoint, KOfunV[0])
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
         result: np.double = 0
-        x = point.floatVariables
+        x = point.float_variables
 
-        if functionValue.type == FunctionType.OBJECTIV:
-            result = np.double(-pow(math.sin(2 * math.pi*x[0]), 3)*math.sin(2 * math.pi*x[1]) / (pow(x[0], 3)*(x[0] + x[1])))
-        elif functionValue.functionID == 0:  # constraint 1
-            result = np.double(pow(x[0], 2) - x[1] + 1)
-        elif functionValue.functionID == 1:  # constraint 2
-            result = np.double(1 - x[0] + pow(x[1] - 4, 4))
+        if function_value.type == FunctionType.OBJECTIV:
+            for i in range(0, 5):
+                temp = 0
+                for j in range(0, self.dimension):
+                    temp += pow(x[j] - p[i][j], 2)
+                temp = a[i] * temp + c[i]
+                result += 1 / temp
+        elif function_value.functionID == 0:  # constraint 1
+            result = np.double(x[0] + x[1] - 5)
+        elif function_value.functionID == 1:  # constraint 2
+            result = np.double(x[0] - pow(x[1], 2))
+        elif function_value.functionID == 2:  # constraint 3
+            result = np.double(5 * pow(x[0], 3) - 8 / 5 * pow(x[1], 2))
 
-        functionValue.value = result
-        return functionValue
+        function_value.value = result
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/grishagin.py` & `iOpt-0.2.22/problems/grishagin.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,43 +22,43 @@
         Конструктор класса Grishagin problem.
 
         :param functionNumber: номер задачи в наборе, :math:`1 <= functionNumber <= 100`
         """
         super(Grishagin, self).__init__()
         self.name = "Grishagin"
         self.dimension = 2
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
-        self.floatVariableNames = np.ndarray(shape=(self.dimension,), dtype=str)
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
+        self.float_variable_names = np.ndarray(shape=(self.dimension,), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension,), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(0)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension,), dtype=np.double)
-        self.upperBoundOfFloatVariables.fill(1)
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension,), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(0)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension,), dtype=np.double)
+        self.upper_bound_of_float_variables.fill(1)
 
         self.functionNumber = function_number
         self.function: GrishaginFunction = GrishaginFunction(self.functionNumber)
         self.function.SetFunctionNumber()
 
-        self.knownOptimum = np.ndarray(shape=(1,), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1,), dtype=Trial)
         pointfv = self.function.GetOptimumPoint()
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1,), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
-        KOfunV[0] = self.Calculate(KOpoint, KOfunV[0])
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        KOfunV[0] = self.calculate(KOpoint, KOfunV[0])
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
-        functionValue.value = self.function.Calculate(point.floatVariables)
+        function_value.value = self.function.Calculate(point.float_variables)
 
-        return functionValue
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/grishagin_function/grishagin_function.py` & `iOpt-0.2.22/problems/grishagin_function/grishagin_function.py`

 * *Files identical despite different names*

### Comparing `iOpt-0.2.1/problems/grishagin_function/grishagin_generation.py` & `iOpt-0.2.22/problems/grishagin_function/grishagin_generation.py`

 * *Files identical despite different names*

### Comparing `iOpt-0.2.1/problems/hill.py` & `iOpt-0.2.22/problems/hill.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,46 +21,46 @@
         Конструктор класса Hill problem.
 
         :param functionNumber: номер задачи в наборе, :math:`1 <= functionNumber <= 1000`
         """
         super(Hill, self).__init__()
         self.name = "Hill"
         self.dimension = 1
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
         self.fn = function_number
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(0)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables.fill(1)
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(0)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables.fill(1)
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
         pointfv = np.ndarray(shape=(self.dimension), dtype=np.double)
         pointfv[0] = hillGen.minHill[self.fn][1]
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
         KOfunV[0].value = hillGen.minHill[self.fn][0]
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
         res: np.double = 0
         for i in range(hillGen.NUM_HILL_COEFF):
-            res = res + hillGen.aHill[self.fn][i] * math.sin(2 * i * math.pi * point.floatVariables[0]) + \
-                  hillGen.bHill[self.fn][i] * math.cos(2 * i * math.pi * point.floatVariables[0])
-        functionValue.value = res
-        return functionValue
+            res = res + hillGen.aHill[self.fn][i] * math.sin(2 * i * math.pi * point.float_variables[0]) + \
+                  hillGen.bHill[self.fn][i] * math.cos(2 * i * math.pi * point.float_variables[0])
+        function_value.value = res
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/rastrigin.py` & `iOpt-0.2.22/problems/romeijn5c.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,61 @@
 import numpy as np
+from iOpt.trial import FunctionType
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
 import math
 
 
-class Rastrigin(Problem):
-    """
-    Функция  Растригина задана формулой:
-       :math:`f(y)=(\sum_{i=1}^{N}[x_{i}^{2}-10*cos(2\pi x_{i})])`,
-       где :math:`x\in [-2.2, 1.8], N` – размерность задачи.
-    """
-
-    def __init__(self, dimension: int):
+class Romeijn5c(Problem):
+    def __init__(self):
         """
-        Конструктор класса Rastrigin problem.
-
-        :param dimension: Размерность задачи.
+        Конструктор класса Romeijn5c problem.
         """
-        super(Rastrigin, self).__init__()
-        self.name = "Rastrigin"
-        self.dimension = dimension
-        self.numberOfFloatVariables = dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        super(Romeijn5c, self).__init__()
+        self.name = "Romeijn5c"
+        self.dimension: int = 2
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 2
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(-2.2)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables.fill(1.8)
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables = [-1.5, 0]
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables = [3.5, 15]
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
-        pointfv = np.ndarray(shape=(self.dimension), dtype=np.double)
-        pointfv.fill(0)
+        pointfv = [2.4656, 15]
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
-        KOfunV[0].value = 0
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        KOfunV[0] = self.calculate(KOpoint, KOfunV[0])  # -195.37
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
-        sum: np.double = 0
-        for i in range(self.dimension):
-            sum += point.floatVariables[i] * point.floatVariables[i] - 10 * math.cos(
-                2 * math.pi * point.floatVariables[i]) + 10
+        result: np.double = 0
+        x = point.float_variables
 
-        functionValue.value = sum
-        return functionValue
+        if function_value.type == FunctionType.OBJECTIV:
+            temp = x[1] - 1.275 * pow(x[0], 2) + 5.0 * x[0] - 6.0
+            result = np.double(-pow(temp, 2) - 10.0 * (1 - 1 / (8.0 * math.pi)) * math.cos(math.pi * x[0]) - 10.0)
+        elif function_value.functionID == 0:  # constraint 1
+            result = -math.pi * x[0] - x[1]
+        elif function_value.functionID == 1:  # constraint 2
+            result = -pow(math.pi * x[0], 2) + 4.0 * x[1]
 
-    def GetName(self):
-        return self.name
+        function_value.value = result
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/rastriginInt.py` & `iOpt-0.2.22/problems/rastrigin_int_hidden_constraint.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,129 +2,138 @@
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
 import math
 
 
-class RastriginInt(Problem):
+class RastriginIntHiddenConstraint(Problem):
     """
     Функция  Растригина задана формулой:
        :math:`f(y)=(\sum_{i=1}^{N}[x_{i}^{2}-10*cos(2\pi x_{i})])`,
        где :math:`x\in [-2.2, 1.8], N` – размерность задачи.
     """
 
-    def __init__(self, dimension: int, numberOfDiscreteVariables: int):
+    def __init__(self, dimension: int, number_of_discrete_variables: int):
         """
         Конструктор класса RastriginInt problem.
 
         :param dimension: Размерность задачи.
         """
-        super(RastriginInt, self).__init__()
-        self.name = "RastriginInt"
+        super(RastriginIntHiddenConstraint, self).__init__()
+        self.name = "RastriginIntHiddenConstraint"
         self.dimension = dimension
-        self.numberOfFloatVariables = dimension - numberOfDiscreteVariables
-        self.numberOfDiscreteVariables = numberOfDiscreteVariables
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        self.number_of_float_variables = dimension - number_of_discrete_variables
+        self.number_of_discrete_variables = number_of_discrete_variables
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
 
-        self.floatVariableNames = np.ndarray(shape=(self.numberOfFloatVariables), dtype=object)
-        for i in range(self.numberOfFloatVariables):
-            self.floatVariableNames[i] = str(i)
+        self.float_variable_names = np.ndarray(shape=(self.number_of_float_variables), dtype=object)
+        for i in range(self.number_of_float_variables):
+            self.float_variable_names[i] = str(i)
 
-        self.discreteVariableNames = np.ndarray(shape=(self.numberOfDiscreteVariables), dtype=object)
-        for i in range(self.numberOfDiscreteVariables):
-            self.discreteVariableNames[i] = str(i)
+        self.discrete_variable_names = np.ndarray(shape=(self.number_of_discrete_variables), dtype=object)
+        for i in range(self.number_of_discrete_variables):
+            self.discrete_variable_names[i] = str(i)
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.numberOfFloatVariables), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(-2.2)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.numberOfFloatVariables), dtype=np.double)
-        self.upperBoundOfFloatVariables.fill(1.8)
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.number_of_float_variables), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(-2.2)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.number_of_float_variables), dtype=np.double)
+        self.upper_bound_of_float_variables.fill(1.8)
 
-        self.discreteVariableValues = [["A", "B"] for i in range(self.numberOfDiscreteVariables)]
+        self.discrete_variable_values = [["A", "B"] for i in range(self.number_of_discrete_variables)]
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
-        pointfv = np.ndarray(shape=(self.numberOfFloatVariables), dtype=np.double)
+        pointfv = np.ndarray(shape=(self.number_of_float_variables), dtype=np.double)
         pointfv.fill(0)
 
-        pointdv = np.ndarray(shape=(self.numberOfDiscreteVariables), dtype=object)
+        pointdv = np.ndarray(shape=(self.number_of_discrete_variables), dtype=object)
         pointdv.fill("B")
 
         KOpoint = Point(pointfv, pointdv)
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
         KOfunV[0].value = 0
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
         self.A = np.ndarray(shape=(self.dimension), dtype=np.double)
         self.A.fill(-2.2)
 
         self.B = np.ndarray(shape=(self.dimension), dtype=np.double)
         self.B.fill(1.8)
 
         self.optPoint = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.optPoint = np.append([[0] for i in range(self.numberOfFloatVariables)],
-                                  [[1.8] for i in range(self.numberOfDiscreteVariables)])
+        self.optPoint = np.append([[0] for i in range(self.number_of_float_variables)],
+                                  [[1.8] for i in range(self.number_of_discrete_variables)])
 
         self.multKoef = 0
 
         x = np.ndarray(shape=(self.dimension), dtype=np.double)
         count =math.pow(2, self.dimension)
         for i in range(int(count)):
             for j in range(self.dimension):
                 x[j] = self.A[j] if (((i >> j) & 1) == 0) else self.B[j]
-            v = abs(self.MultFunc(x))
+            v = abs(self.mult_func(x))
             if v > self.multKoef:  self.multKoef = v
 
         self.multKoef += 4
-        self.optMultKoef = (self.MultFunc(self.optPoint)+self.multKoef)
+        self.optMultKoef = (self.mult_func(self.optPoint) + self.multKoef)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
+
+        isInf: bool = True
+        for i in range(self.number_of_float_variables):
+            if point.float_variables[i] <= 0.5 or point.float_variables[i] > 1.5:
+                isInf = False
+
+        if isInf:
+            raise Exception("Infinity values")
+
         sum: np.double = 0
-        x = point.floatVariables
-        for i in range(self.numberOfFloatVariables):
+        x = point.float_variables
+        for i in range(self.number_of_float_variables):
             sum += x[i] * x[i] - 10 * math.cos(2 * math.pi * x[i]) + 10
 
-        dx = point.discreteVariables
-        for i in range(self.numberOfDiscreteVariables):
+        dx = point.discrete_variables
+        for i in range(self.number_of_discrete_variables):
             if dx[i] == "A":
                 sum += 2.2
             elif dx[i] == "B":
                 sum -= 1.8
             else:
                 raise ValueError
 
-        x_arr = self.PointToArray(point)
-        sum = sum * (self.MultFunc(x_arr)+self.multKoef)
+        x_arr = self.point_to_array(point)
+        sum = sum * (self.mult_func(x_arr) + self.multKoef)
 
-        functionValue.value = sum
-        return functionValue
+        function_value.value = sum
+        return function_value
 
-    def PointToArray(self, point: Point) -> np.ndarray:
+    def point_to_array(self, point: Point) -> np.ndarray:
         arr = np.ndarray(shape=(self.dimension), dtype=np.double)
 
-        for i in range(0, self.numberOfFloatVariables):
-            arr[i] = point.floatVariables[i]
+        for i in range(0, self.number_of_float_variables):
+            arr[i] = point.float_variables[i]
 
-        for i in range(0, self.numberOfDiscreteVariables):
-            if point.discreteVariables[i] == "A":
-                arr[self.numberOfFloatVariables+i] = -2.2
-            elif point.discreteVariables[i] == "B":
-                arr[self.numberOfFloatVariables+i] = 1.8
+        for i in range(0, self.number_of_discrete_variables):
+            if point.discrete_variables[i] == "A":
+                arr[self.number_of_float_variables+i] = -2.2
+            elif point.discrete_variables[i] == "B":
+                arr[self.number_of_float_variables+i] = 1.8
         return arr
 
-    def MultFunc(self, x: np.ndarray) -> np.double:
+    def mult_func(self, x: np.ndarray) -> np.double:
         result: np.double = 0
         a: np.double
         d: np.double
 
         for i in range(self.dimension):
             d = (self.B[i]-self.A[i])/2
             a = (x[i]-self.optPoint[i])/d
```

### Comparing `iOpt-0.2.1/problems/rastrigin_hidden_constraint.py` & `iOpt-0.2.22/problems/rastrigin.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,74 +2,65 @@
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
 import math
 
 
-class RastriginHiddenConstraint(Problem):
+class Rastrigin(Problem):
     """
-    Функция Растригина со скрытими ограничениями задана формулой:
+    Функция  Растригина задана формулой:
        :math:`f(y)=(\sum_{i=1}^{N}[x_{i}^{2}-10*cos(2\pi x_{i})])`,
        где :math:`x\in [-2.2, 1.8], N` – размерность задачи.
     """
 
     def __init__(self, dimension: int):
         """
-        Конструктор класса RastriginHiddenConstraint problem.
+        Конструктор класса Rastrigin problem.
 
         :param dimension: Размерность задачи.
         """
-        super(RastriginHiddenConstraint, self).__init__()
-        self.name = "RastriginHiddenConstraint"
+        super(Rastrigin, self).__init__()
+        self.name = "Rastrigin"
         self.dimension = dimension
-        self.numberOfFloatVariables = dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        self.number_of_float_variables = dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(-2.2)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables.fill(1.8)
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(-2.2)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables.fill(1.8)
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
         pointfv = np.ndarray(shape=(self.dimension), dtype=np.double)
         pointfv.fill(0)
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
         KOfunV[0].value = 0
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
-
-        isInf: bool = True
-        for i in range(self.dimension):
-            if point.floatVariables[i] <= 0.5 or point.floatVariables[i] > 1.5:
-                isInf = False
-
-        if isInf:
-            raise Exception("Infinity values")
-
         sum: np.double = 0
         for i in range(self.dimension):
-            sum += point.floatVariables[i] * point.floatVariables[i] - 10 * math.cos(
-                2 * math.pi * point.floatVariables[i]) + 10
+            sum += point.float_variables[i] * point.float_variables[i] - 10 * math.cos(
+                2 * math.pi * point.float_variables[i]) + 10
 
-        functionValue.value = sum
-        return functionValue
+        function_value.value = sum
+        return function_value
 
-    def GetName(self):
+    def get_name(self):
         return self.name
```

### Comparing `iOpt-0.2.1/problems/romeijn1c.py` & `iOpt-0.2.22/problems/romeijn1c.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,45 +10,45 @@
     def __init__(self):
         """
         Конструктор класса RomeijnC1 problem.
         """
         super(Romeijn1c, self).__init__()
         self.name = "Romeijn1c"
         self.dimension: int = 3
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 1
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 1
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(0)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables = [0.18745, 0.16230, 0.42846]
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(0)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables = [0.18745, 0.16230, 0.42846]
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
         # Optimum is UNDEFINED
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
         result: np.double = 0
-        x = point.floatVariables
+        x = point.float_variables
 
-        if functionValue.type == FunctionType.OBJECTIV:
+        if function_value.type == FunctionType.OBJECTIV:
             result = -1 / (pow(x[0], 2) * x[1] * x[2])
-        elif functionValue.functionID == 0:  # constraint 1
+        elif function_value.functionID == 0:  # constraint 1
             result = 0.44098 * x[0] + 28.46 * pow(x[0], 2) + 6158.4 * pow(x[0], 2) * x[1] + 0.0037018 * x[2] + \
                      5.4474 * pow(x[2], 2) + 0.032236 * x[0] * x[2] + 2.92 * x[1] * x[2] + 0.44712 * x[1] \
                      + 37.964 * pow(x[1], 2) + 42.876 * x[0] * x[1] - 1
 
-        functionValue.value = result
-        return functionValue
+        function_value.value = result
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/romeijn2c.py` & `iOpt-0.2.22/problems/romeijn2c.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,55 +10,55 @@
     def __init__(self):
         """
         Конструктор класса Romeijn2c problem.
         """
         super(Romeijn2c, self).__init__()
         self.name = "Romeijn2c"
         self.dimension: int = 6
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 2
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 2
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(0)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables = [10, 10, 15, 15, 1, 1]
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(0)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables = [10, 10, 15, 15, 1, 1]
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
         pointfv = [10, 10, 15, 4.609, 0.78511, 0.384]
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
-        KOfunV[0] = self.Calculate(KOpoint, KOfunV[0])
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        KOfunV[0] = self.calculate(KOpoint, KOfunV[0])
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
         result: np.double = 1
-        x = point.floatVariables
+        x = point.float_variables
 
-        if functionValue.type == FunctionType.OBJECTIV:
+        if function_value.type == FunctionType.OBJECTIV:
             result = np.double(-(0.0204 + 0.0607 * pow(x[4], 2)) * x[0] * x[3] * (x[0] + x[1] + x[2]) - \
                                (0.0187 + 0.0437 * pow(x[5], 2)) * x[1] * x[2] * (x[0] + 1.57 * x[1] + x[3]))
-        elif functionValue.functionID == 0:  # constraint 1
+        elif function_value.functionID == 0:  # constraint 1
             for i in range(0, self.dimension):
                 result = result / x[i]
             result = np.double(2070 * result - 1)
 
-        elif functionValue.functionID == 1:  # constraint 2
+        elif function_value.functionID == 1:  # constraint 2
             result = np.double(0.00062 * x[0] * x[3] * pow(x[4], 2) * (x[0] + x[1] + x[2]) + \
                                0.00058 * x[1] * x[2] * pow(x[5], 2) * (x[0] + 1.57 * x[1] + x[3]) - 1)
 
-        functionValue.value = result
-        return functionValue
+        function_value.value = result
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/romeijn3c.py` & `iOpt-0.2.22/problems/stronginc5.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 import numpy as np
 from iOpt.trial import FunctionType
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
+import math
 
-a = np.array([0.5, 0.25, 1.0, 1.0 / 12.0, 2])
-c = np.array([0.125, 0.25, 0.1, 0.2, 1.0 / 12.0])
-p = np.array([[0, 5], [2, 5], [3, 2], [4, 4], [5, 1]])
 
-
-class Romeijn3c(Problem):
+class Stronginc5(Problem):
     def __init__(self):
         """
-        Конструктор класса Romeijn3c problem.
+        Конструктор класса Stronginc5 problem.
         """
-        super(Romeijn3c, self).__init__()
-        self.name = "Romeijn3c"
-        self.dimension: int = 2
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 3
+        super(Stronginc5, self).__init__()
+        self.name = "Stronginc5"
+        self.dimension: int = 5
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 5
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(1, self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables = [-3, -4]
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables = [10, 7]
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables = [-3, -3, -3, -10, -10]
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables = [3, 3, 3, 10, 10]
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
-        pointfv = [-3, -4]
+        pointfv = [-0.0679, 1.9434, 2.4512, 9.9013, 9.9008]
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
-        KOfunV[0] = self.Calculate(KOpoint, KOfunV[0])
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        KOfunV[0] = self.calculate(KOpoint, KOfunV[0]) # -43.298677;
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
-        result: np.double = 0
-        x = point.floatVariables
+        res: np.double = 0
+        x = point.float_variables
 
-        if functionValue.type == FunctionType.OBJECTIV:
-            for i in range(0, 5):
-                temp = 0
-                for j in range(0, self.dimension):
-                    temp += pow(x[j] - p[i][j], 2)
-                temp = a[i] * temp + c[i]
-                result += 1 / temp
-        elif functionValue.functionID == 0:  # constraint 1
-            result = np.double(x[0] + x[1] - 5)
-        elif functionValue.functionID == 1:  # constraint 2
-            result = np.double(x[0] - pow(x[1], 2))
-        elif functionValue.functionID == 2:  # constraint 3
-            result = np.double(5 * pow(x[0], 3) - 8 / 5 * pow(x[1], 2))
+        if function_value.type == FunctionType.OBJECTIV:
+            res = np.double(math.sin(x[0] * x[2]) - (x[1] * x[4] + x[2] * x[3])*math.cos(x[0] * x[1]))
+        elif function_value.functionID == 0:  # constraint 1
+            res = np.double(-(x[0] + x[1] + x[2] + x[3] + x[4]))
+        elif function_value.functionID == 1:  # constraint 2
+            res = np.double(x[1] * x[1] / 9 + x[3] * x[3] / 100 - 1.4)
+        elif function_value.functionID == 2:  # constraint 3
+            res = np.double(3 - pow(x[0] + 1, 2) - pow(x[1] + 2, 2) - pow(x[2] - 2, 2) - pow(x[4] + 5, 2))
+        elif function_value.functionID == 3:  # constraint 4
+            res = np.double(4 * x[0] * x[0] * math.sin(x[0]) + x[1] * x[1] * math.cos(x[1] + x[3]) +
+                            x[2] * x[2] * (math.sin(x[2] + x[4]) + math.sin(10 * (x[2] - x[3]) / 3)) - 4)
+        elif function_value.functionID == 4:  # constraint 5
+            res = np.double(x[0] * x[0] + x[1] * x[1] * pow(math.sin((x[0] + x[3]) / 3 + 6.6) +
+                                                            math.sin((x[1] + x[4]) / 2 + 0.9), 2) - 17 *
+                            pow(math.cos(x[0] + x[2] + 1), 2) + 16)
 
-        functionValue.value = result
-        return functionValue
+        function_value.value = res
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/romeijn5c.py` & `iOpt-0.2.22/problems/g8c.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,59 +3,58 @@
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
 import math
 
 
-class Romeijn5c(Problem):
+class g8c(Problem):
     def __init__(self):
         """
-        Конструктор класса Romeijn5c problem.
+        Конструктор класса gC8 problem.
         """
-        super(Romeijn5c, self).__init__()
-        self.name = "Romeijn5c"
+        super(g8c, self).__init__()
+        self.name = "g8c"
         self.dimension: int = 2
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 2
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 2
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables = [-1.5, 0]
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables = [3.5, 15]
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(0)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables.fill(10)
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
-        pointfv = [2.4656, 15]
+        pointfv = [1.2279713, 4.2453733]
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
-        KOfunV[0] = self.Calculate(KOpoint, KOfunV[0])  # -195.37
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        KOfunV[0] = self.calculate(KOpoint, KOfunV[0])
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
         result: np.double = 0
-        x = point.floatVariables
+        x = point.float_variables
 
-        if functionValue.type == FunctionType.OBJECTIV:
-            temp = x[1] - 1.275 * pow(x[0], 2) + 5.0 * x[0] - 6.0
-            result = np.double(-pow(temp, 2) - 10.0 * (1 - 1 / (8.0 * math.pi)) * math.cos(math.pi * x[0]) - 10.0)
-        elif functionValue.functionID == 0:  # constraint 1
-            result = -math.pi * x[0] - x[1]
-        elif functionValue.functionID == 1:  # constraint 2
-            result = -pow(math.pi * x[0], 2) + 4.0 * x[1]
+        if function_value.type == FunctionType.OBJECTIV:
+            result = np.double(-pow(math.sin(2 * math.pi*x[0]), 3)*math.sin(2 * math.pi*x[1]) / (pow(x[0], 3)*(x[0] + x[1])))
+        elif function_value.functionID == 0:  # constraint 1
+            result = np.double(pow(x[0], 2) - x[1] + 1)
+        elif function_value.functionID == 1:  # constraint 2
+            result = np.double(1 - x[0] + pow(x[1] - 4, 4))
 
-        functionValue.value = result
-        return functionValue
+        function_value.value = result
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/shekel.py` & `iOpt-0.2.22/problems/shekel.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,50 +18,50 @@
     def __init__(self, function_number: int):
         """
         Конструктор класса Shekel problem.
 
         :param functionNumber: номер задачи в наборе, :math:`1 <= functionNumber <= 1000`
         """
         super(Shekel, self).__init__()
-        self.name = Shekel
+        self.name = "Shekel"
         self.dimension = 1
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
         self.fn = function_number
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension,), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension,), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension,), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(0)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension,), dtype=np.double)
-        self.upperBoundOfFloatVariables.fill(10)
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension,), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(0)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension,), dtype=np.double)
+        self.upper_bound_of_float_variables.fill(10)
 
-        self.knownOptimum = np.ndarray(shape=(1,), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1,), dtype=Trial)
 
         pointfv = np.ndarray(shape=(self.dimension,), dtype=np.double)
         pointfv[0] = shekelGen.minShekel[self.fn][1]
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1,), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
         KOfunV[0].value = shekelGen.minShekel[self.fn][0]
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
         res: np.double = 0
         for i in range(shekelGen.NUM_SHEKEL_COEFF):
             res = res - 1 / (
-                        shekelGen.kShekel[self.fn][i] * pow(point.floatVariables[0] - shekelGen.aShekel[self.fn][i], 2)
+                        shekelGen.kShekel[self.fn][i] * pow(point.float_variables[0] - shekelGen.aShekel[self.fn][i], 2)
                         + shekelGen.cShekel[self.fn][i])
 
-        functionValue.value = res
-        return functionValue
+        function_value.value = res
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/shekel4.py` & `iOpt-0.2.22/problems/stronginc3.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 import numpy as np
+from iOpt.trial import FunctionType
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
-import problems.Shekel4.shekel4_generation as shekelGen
+import math
 
 
-class Shekel4(Problem):
-    """
-    Функция Шекеля - это многомерная, мультимодальная, непрерывная, детерминированная функция, задана формулой:
-       :math:`f(x) = \sum_{i=1}^{m}(c_{i}+\sum_{j=1}^{n}(x-a_{i})^{2})^{-1}`,
-       где :math:`m` – количество максимумов функции,
-       :math:`a, c` - параметры, генерируемые случайным образом.
-       В генераторе размерность задачи равна 4.
-    """
-
-    def __init__(self, function_number: int):
+class Stronginc3(Problem):
+    def __init__(self):
         """
-        Конструктор класса Shekel problem.
-
-        :param functionNumber: номер задачи в наборе, :math:`1 <= functionNumber <= 3`
+        Конструктор класса Stronginc3 problem.
         """
-        super(Shekel4, self).__init__()
-        self.name = Shekel4
-        self.dimension = 4
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
-        self.fn = function_number
+        super(Stronginc3, self).__init__()
+        self.name = "Stronginc3"
+        self.dimension: int = 2
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 3
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension,), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension,), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(0)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension,), dtype=np.double)
-        self.upperBoundOfFloatVariables.fill(10)
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables = [0, -1]
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables = [4, 3]
 
-        self.knownOptimum = np.ndarray(shape=(1,), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
-        pointfv = np.ndarray(shape=(self.dimension,), dtype=np.double)
-        pointfv.fill(4)
+        pointfv = np.ndarray(shape=(self.dimension), dtype=np.double)
+        pointfv = [0.941176, 0.941176]
         KOpoint = Point(pointfv, [])
-        KOfunV = np.ndarray(shape=(1,), dtype=FunctionValue)
+        KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
-        KOfunV[0] = self.Calculate(KOpoint, KOfunV[0])
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        KOfunV[0].value = -1.489444
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
         res: np.double = 0
-        for i in range(shekelGen.maxI[self.fn - 1]):
-            den: np.double = 0
-            for j in range(self.dimension):
-                den = den + pow((point.floatVariables[j] - shekelGen.a[i][j]), 2.0)
-            res = res - 1 / (den + shekelGen.c[i])
+        x: np.double = point.float_variables
+
+        if function_value.type == FunctionType.OBJECTIV:
+            t1: np.double = pow(0.5 * x[0] - 0.5, 4.0)
+            t2: np.double = pow(x[1] - 1.0, 4.0)
+            res = np.double(1.5 * x[0] * x[0] * math.exp(1.0 - x[0] * x[0] - 20.25 * (x[0] - x[1]) * (x[0] - x[1])))
+            res = np.double(res + t1 * t2 * math.exp(2.0 - t1 - t2))
+            res = np.double(-res)
+        elif function_value.functionID == 0:  # constraint 1
+            res = np.double(0.01 * ((x[0] - 2.2) * (x[0] - 2.2) + (x[1] - 1.2) * (x[1] - 1.2) - 2.25))
+        elif function_value.functionID == 1:  # constraint 2
+            res = np.double(100.0 * (1.0 - ((x[0] - 2.0) / 1.2) * ((x[0] - 2.0) / 1.2) - (x[1] / 2.0) * (x[1] / 2.0)))
+        elif function_value.functionID == 2:  # constraint 3
+            res = np.double(10.0 * (x[1] - 1.5 - 1.5 * math.sin(6.283 * (x[0] - 1.75))))
+
+        function_value.value = res
+        return function_value
 
-        functionValue.value = res
-        return functionValue
+    def get_name(self):
+        return self.name
```

### Comparing `iOpt-0.2.1/problems/stronginc2.py` & `iOpt-0.2.22/problems/stronginc2.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,56 +11,56 @@
     def __init__(self):
         """
         Конструктор класса Stronginc2 problem.
         """
         super(Stronginc2, self).__init__()
         self.name = 'Stronginc2'
         self.dimension: int = 2
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 2
+        self.number_of_float_variables = self.dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 2
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables = [0, -1]
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables = [4, 3]
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables = [0, -1]
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables = [4, 3]
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
         pointfv = np.ndarray(shape=(self.dimension), dtype=np.double)
         pointfv.fill(1.088)
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
-        KOfunV[0] = self.Calculate(KOpoint, KOfunV[0])  # -1.477
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        KOfunV[0] = self.calculate(KOpoint, KOfunV[0])  # -1.477
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
         res: np.double = 0
-        x: np.double = point.floatVariables
+        x: np.double = point.float_variables
 
-        if functionValue.type == FunctionType.OBJECTIV:
+        if function_value.type == FunctionType.OBJECTIV:
             t1: np.double = pow(0.5 * x[0] - 0.5, 4.0)
             t2: np.double = pow(x[1] - 1.0, 4.0)
             res = np.double(1.5 * x[0] * x[0] * math.exp(1.0 - x[0] * x[0] - 20.25 * (x[0] - x[1]) * (x[0] - x[1])))
             res = np.double(res + t1 * t2 * math.exp(2.0 - t1 - t2))
             res = np.double(-res)
-        elif functionValue.functionID == 0:  # constraint 1
+        elif function_value.functionID == 0:  # constraint 1
             res = np.double(((x[0]- 2.2) * (x[0] - 2.2) + (x[1] - 1.2) * (x[1] - 1.2) - 1.25))
-        elif functionValue.functionID == 1:  # constraint 2
+        elif function_value.functionID == 1:  # constraint 2
             res = np.double(1.21 - (x[0] - 2.2) * (x[0] - 2.2) - (x[1] - 1.2) * (x[1] - 1.2))
 
-        functionValue.value = res
-        return functionValue
+        function_value.value = res
+        return function_value
```

### Comparing `iOpt-0.2.1/problems/stronginc3.py` & `iOpt-0.2.22/problems/rastrigin_hidden_constraint.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,75 @@
 import numpy as np
-from iOpt.trial import FunctionType
 from iOpt.trial import Point
 from iOpt.trial import FunctionValue
 from iOpt.trial import Trial
 from iOpt.problem import Problem
 import math
 
 
-class Stronginc3(Problem):
-    def __init__(self):
+class RastriginHiddenConstraint(Problem):
+    """
+    Функция Растригина со скрытими ограничениями задана формулой:
+       :math:`f(y)=(\sum_{i=1}^{N}[x_{i}^{2}-10*cos(2\pi x_{i})])`,
+       где :math:`x\in [-2.2, 1.8], N` – размерность задачи.
+    """
+
+    def __init__(self, dimension: int):
         """
-        Конструктор класса Stronginc3 problem.
+        Конструктор класса RastriginHiddenConstraint problem.
+
+        :param dimension: Размерность задачи.
         """
-        super(Stronginc3, self).__init__()
-        self.name = "Stronginc3"
-        self.dimension: int = 2
-        self.numberOfFloatVariables = self.dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 3
+        super(RastriginHiddenConstraint, self).__init__()
+        self.name = "RastriginHiddenConstraint"
+        self.dimension = dimension
+        self.number_of_float_variables = dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables = [0, -1]
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables = [4, 3]
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(-2.2)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables.fill(1.8)
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
         pointfv = np.ndarray(shape=(self.dimension), dtype=np.double)
-        pointfv = [0.941176, 0.941176]
+        pointfv.fill(0)
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
-        KOfunV[0].value = -1.489444
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        KOfunV[0].value = 0
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения выбранной функции в заданной точке.
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
-        res: np.double = 0
-        x: np.double = point.floatVariables
 
-        if functionValue.type == FunctionType.OBJECTIV:
-            t1: np.double = pow(0.5 * x[0] - 0.5, 4.0)
-            t2: np.double = pow(x[1] - 1.0, 4.0)
-            res = np.double(1.5 * x[0] * x[0] * math.exp(1.0 - x[0] * x[0] - 20.25 * (x[0] - x[1]) * (x[0] - x[1])))
-            res = np.double(res + t1 * t2 * math.exp(2.0 - t1 - t2))
-            res = np.double(-res)
-        elif functionValue.functionID == 0:  # constraint 1
-            res = np.double(0.01 * ((x[0] - 2.2) * (x[0] - 2.2) + (x[1] - 1.2) * (x[1] - 1.2) - 2.25))
-        elif functionValue.functionID == 1:  # constraint 2
-            res = np.double(100.0 * (1.0 - ((x[0] - 2.0) / 1.2) * ((x[0] - 2.0) / 1.2) - (x[1] / 2.0) * (x[1] / 2.0)))
-        elif functionValue.functionID == 2:  # constraint 3
-            res = np.double(10.0 * (x[1] - 1.5 - 1.5 * math.sin(6.283 * (x[0] - 1.75))))
+        isInf: bool = True
+        for i in range(self.dimension):
+            if point.float_variables[i] <= 0.5 or point.float_variables[i] > 1.5:
+                isInf = False
+
+        if isInf:
+            raise Exception("Infinity values")
+
+        sum: np.double = 0
+        for i in range(self.dimension):
+            sum += point.float_variables[i] * point.float_variables[i] - 10 * math.cos(
+                2 * math.pi * point.float_variables[i]) + 10
 
-        functionValue.value = res
-        return functionValue
+        function_value.value = sum
+        return function_value
 
-    def GetName(self):
+    def get_name(self):
         return self.name
```

### Comparing `iOpt-0.2.1/problems/xsquared.py` & `iOpt-0.2.22/problems/xsquared.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,50 +8,50 @@
 class XSquared(Problem):
     """
     Функция критерия :math:`f(x) = x^2`.
     """
 
     def __init__(self, dimension: int):
         super(XSquared, self).__init__()
-        self.name = XSquared
+        self.name = "XSquared"
         self.dimension = dimension
-        self.numberOfFloatVariables = dimension
-        self.numberOfDiscreteVariables = 0
-        self.numberOfObjectives = 1
-        self.numberOfConstraints = 0
+        self.number_of_float_variables = dimension
+        self.number_of_discrete_variables = 0
+        self.number_of_objectives = 1
+        self.number_of_constraints = 0
 
-        self.floatVariableNames = np.ndarray(shape=(self.dimension), dtype=str)
+        self.float_variable_names = np.ndarray(shape=(self.dimension), dtype=str)
         for i in range(self.dimension):
-            self.floatVariableNames[i] = i
+            self.float_variable_names[i] = i
 
-        self.lowerBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.lowerBoundOfFloatVariables.fill(-1)
-        self.upperBoundOfFloatVariables = np.ndarray(shape=(self.dimension), dtype=np.double)
-        self.upperBoundOfFloatVariables.fill(1)
+        self.lower_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.lower_bound_of_float_variables.fill(-1)
+        self.upper_bound_of_float_variables = np.ndarray(shape=(self.dimension), dtype=np.double)
+        self.upper_bound_of_float_variables.fill(1)
 
-        self.knownOptimum = np.ndarray(shape=(1), dtype=Trial)
+        self.known_optimum = np.ndarray(shape=(1), dtype=Trial)
 
         pointfv = np.ndarray(shape=(self.dimension), dtype=np.double)
         pointfv.fill(0)
         KOpoint = Point(pointfv, [])
         KOfunV = np.ndarray(shape=(1), dtype=FunctionValue)
         KOfunV[0] = FunctionValue()
         KOfunV[0].value = 0
-        self.knownOptimum[0] = Trial(KOpoint, KOfunV)
+        self.known_optimum[0] = Trial(KOpoint, KOfunV)
 
-    def Calculate(self, point: Point, functionValue: FunctionValue) -> FunctionValue:
+    def calculate(self, point: Point, function_value: FunctionValue) -> FunctionValue:
         """
         Вычисление значения критерия
 
         :param point: координаты точки испытания, в которой будет вычислено значение функции
-        :param functionValue: объект определяющий номер функции в задаче и хранящий значение функции
+        :param function_value: объект определяющий номер функции в задаче и хранящий значение функции
         :return: Вычисленное значение функции в точке point
         """
         sum: np.double = 0
         for i in range(self.dimension):
-            sum += point.floatVariables[i] * point.floatVariables[i]
+            sum += point.float_variables[i] * point.float_variables[i]
 
-        functionValue.value = sum
-        return functionValue
+        function_value.value = sum
+        return function_value
 
-    def GetName(self):
+    def get_name(self):
         return self.name
```

### Comparing `iOpt-0.2.1/setup.py` & `iOpt-0.2.22/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 def _get_requirements(req_name: str):
     requirements = _extract_requirements(req_name)
     return requirements
 
 setup(
    name='iOpt',
-   version='0.2.1',
+   version='0.2.22',
    description='Фреймворк для автоматического выбора значений параметров для математических моделей, ИИ и МО.',
    author='UNN Team',
    author_email='',
    long_description=read_me_description,
    long_description_content_type="text/markdown",
    url="https://github.com/aimclub/iOpt",
    python_requires='>=3.8',
```

### Comparing `iOpt-0.2.1/test/test_evolvent.py` & `iOpt-0.2.22/test/test_evolvent.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 class TestEvolvent(unittest.TestCase):
     def setUp(self):
         self.ev1 = Evolvent([-1], [1])  # N = 1
         self.ev2 = Evolvent([-1, -1], [1, 1], 2, 10)  # N = 2, m = 10
 
     def test_Preimages_N1(self):
         y = [0]
-        self.assertEqual(self.ev1.GetPreimages(y), 0.5)
+        self.assertEqual(self.ev1.get_preimages(y), 0.5)
 
     def test_XtoYandBack_N1(self):
         x1 = 0.5
-        y = self.ev1.GetImage(x1)
-        x2 = self.ev1.GetInverseImage(y)
+        y = self.ev1.get_image(x1)
+        x2 = self.ev1.get_inverse_image(y)
         self.assertEqual(x1, x2)
 
     def test_Preimages_N2(self):
         y = [0.5, 0.5]
-        self.assertEqual(self.ev2.GetPreimages(y), 0.625)
+        self.assertEqual(self.ev2.get_preimages(y), 0.625)
 
     def test_XtoYandBack_N2(self):
         x1 = 0.625
-        y = self.ev2.GetImage(x1)
-        x2 = self.ev2.GetInverseImage(y)
+        y = self.ev2.get_image(x1)
+        x2 = self.ev2.get_inverse_image(y)
         self.assertEqual(x1, x2)
 
     def test_YtoXandBack_N2(self):
         y1 = np.array([0.5, 0.5])
-        x = self.ev2.GetInverseImage(y1)
-        y2 = self.ev2.GetImage(x)
+        x = self.ev2.get_inverse_image(y1)
+        y2 = self.ev2.get_image(x)
         np.testing.assert_array_almost_equal(y1, y2, decimal=3)
         # self.assertAlmostEqual(y1.tolist(), y2.tolist())
 
     def test_fileGetInverseImage(self):
 
         with open('test/evolventTestData/evolventGetInverseImage.txt') as file:
             for line in file:
@@ -60,15 +60,15 @@
                         y.append(np.double(yValue.split('=')[1]))
 
                     # [-0.5, 0.5]
                     lower = - np.ones(N, dtype=np.int32) / 2
                     upper = np.ones(N, dtype=np.int32) / 2
 
                     evolvent = Evolvent(lower, upper, N, m)
-                    xx = evolvent.GetInverseImage(y)
+                    xx = evolvent.get_inverse_image(y)
 
                     self.assertAlmostEqual(x, xx, 5)
 
     def test_fileGetImage(self):
 
         with open('test/evolventTestData/evolventGetImage.txt') as file:
             for line in file:
@@ -92,15 +92,15 @@
                         y.append(np.double(yValue.split('=')[1]))
 
                     # [-0.5, 0.5]
                     lower = - np.ones(N, dtype=np.int32) / 2
                     upper = np.ones(N, dtype=np.int32) / 2
 
                     evolvent = Evolvent(lower, upper, N, m)
-                    yy = evolvent.GetImage(x)
+                    yy = evolvent.get_image(x)
 
                     np.testing.assert_array_almost_equal(y, yy, decimal=10)
 
 
 # Executing the tests in the above test case class
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `iOpt-0.2.1/test/test_optim_task.py` & `iOpt-0.2.22/test/test_optim_task.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """setUp method is overridden from the parent class OptimizationTask"""
 
     def setUp(self):
         self.problem = Rastrigin(3)
         self.optimizationTask = OptimizationTask(self.problem)
 
         self.problemPerm = Rastrigin(3)
-        self.perm = np.ndarray(shape=(self.problemPerm.numberOfObjectives + self.problemPerm.numberOfConstraints),
+        self.perm = np.ndarray(shape=(self.problemPerm.number_of_objectives + self.problemPerm.number_of_constraints),
                                dtype=np.int32)
         for i in range(self.perm.size):
             self.perm[i] = self.perm.size - 1 - i
         self.optimizationTaskPerm = OptimizationTask(self.problem, self.perm)
 
     def test_InitWithoutPermRastrigin3(self):
         self.assertEqual(self.optimizationTask.perm.tolist(), [0])
@@ -28,22 +28,22 @@
 
     def test_InitWithPermRastrigin3(self):
         self.assertEqual(self.optimizationTaskPerm.perm.tolist(), [0])
 
     def test_CalculateRastrigin3(self):
         point = Point([0.5, 0.1, 0.3], [])
         sdi = SearchDataItem(point, -1, 0)
-        sdi.functionValues = np.ndarray(shape=(1), dtype=FunctionValue)
-        sdi.functionValues[0] = FunctionValue()
-        sdi = self.optimizationTask.Calculate(sdi, 0)
+        sdi.function_values = np.ndarray(shape=(1), dtype=FunctionValue)
+        sdi.function_values[0] = FunctionValue()
+        sdi = self.optimizationTask.calculate(sdi, 0)
 
         sum: np.double = 0
         for i in range(self.problem.dimension):
-            sum += point.floatVariables[i] * point.floatVariables[i] - 10 * math.cos(
-                2 * math.pi * point.floatVariables[i]) + 10
+            sum += point.float_variables[i] * point.float_variables[i] - 10 * math.cos(
+                2 * math.pi * point.float_variables[i]) + 10
 
-        self.assertEqual(sdi.functionValues[0].value, sum)
+        self.assertEqual(sdi.function_values[0].value, sum)
 
 
 """Executing the tests in the above test case class"""
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `iOpt-0.2.1/test/test_solving_test_problems.py` & `iOpt-0.2.22/test/test_solving_test_problems.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,26 +22,26 @@
         self.epsVal = 0.01
 
     def checkIsSolved(self, problem: Problem, params: SolverParameters, number_of_global_trials: int):
         # Создаем решатель
         solver = Solver(problem, parameters=params)
 
         # Решение задачи
-        sol = solver.Solve()
+        sol = solver.solve()
 
         # Проверяем что найденный АГП минимумом соответствуйте априори известному, для этой задачи, с точностью eps
         for j in range(problem.dimension):
-            fabsx = np.abs(problem.knownOptimum[0].point.floatVariables[j] -
-                           sol.bestTrials[0].point.floatVariables[j])
-            fm = params.eps * (problem.upperBoundOfFloatVariables[j] -
-                               problem.lowerBoundOfFloatVariables[j])
+            fabsx = np.abs(problem.known_optimum[0].point.float_variables[j] -
+                           sol.best_trials[0].point.float_variables[j])
+            fm = params.eps * (problem.upper_bound_of_float_variables[j] -
+                               problem.lower_bound_of_float_variables[j])
             self.assertLessEqual(fabsx, fm)
 
         # Проверяем что на решение потребовалось правильное число итераций АГП
-        self.assertEqual(sol.numberOfGlobalTrials, number_of_global_trials)
+        self.assertEqual(sol.number_of_global_trials, number_of_global_trials)
 
     def test_Rastrigin_Solve(self):
         r = 3.5
         problem = Rastrigin(1)
         params = SolverParameters(r=r, eps=self.epsVal)
         number_of_global_trials = 44
 
@@ -94,68 +94,66 @@
 
     def test_Solve_100_GKLS_2D_problem(self):
         # Необходимое число итераций алгоритма, для каждой из 100 задач, с заданными параметрами решателя
         number_of_global_trials = [883, 1441, 1061, 723, 732, 687, 684, 775, 754, 1053, 1165, 1361, 465, 760, 701, 887,
                                    1070, 1673, 1576, 744, 392, 878, 1176, 525, 1175, 856, 898, 649, 885, 771, 972, 1042,
                                    1042, 619, 796, 544, 647, 1071, 591, 833, 605, 458, 527, 1003, 473, 988, 1277, 649,
                                    531, 730, 1108, 828, 648, 221, 1502, 849, 632, 641, 609, 749, 922, 693, 991, 894,
-                                   716,
-                                   575, 952, 1287, 231, 1052, 625, 516, 732, 757, 617, 1455, 490, 1118, 786, 1273, 533,
-                                   683,
-                                   278, 1456, 1091, 1171, 974, 777, 1227, 700, 767, 728, 962, 1198, 445, 809, 946, 288,
-                                   927, 903]
+                                   716, 575, 952, 1287, 231, 1052, 625, 516, 732, 757, 617, 1455, 490, 1118, 786, 1273,
+                                   533, 683, 278, 1456, 1091, 1171, 974, 777, 1227, 700, 767, 728, 962, 1198, 445, 809,
+                                   946, 288, 927, 903]
 
         for i in range(100):
             # создание объекта задачи, двухмерная задача с номером i+1
             problem = GKLS(2, i + 1)
             # Формируем параметры решателя, параметр надежности метода r=5.1, точность поиска eps=0.01
             params = SolverParameters(r=5.1, eps=0.01)
 
             self.checkIsSolved(problem, params, number_of_global_trials[i])
 
     def test_GKLS_4D_Solve(self):
         r = 3.5
         problem = GKLS(4, 3)
-        params = SolverParameters(r=r, eps=self.epsVal, refineSolution=False, itersLimit=5000)
+        params = SolverParameters(r=r, eps=self.epsVal, refine_solution=False, iters_limit=5000)
 
         number_of_global_trials = 2830
 
         self.checkIsSolved(problem, params, number_of_global_trials)
 
     def test_StronginC2_Solve(self):
         r = 4
         problem = Stronginc2()
-        params = SolverParameters(r=r, eps=self.epsVal, epsR=0.01)
+        params = SolverParameters(r=r, eps=self.epsVal, eps_r=0.01)
 
         number_of_global_trials = 437
 
         self.checkIsSolved(problem, params, number_of_global_trials)
 
     def test_StronginC3_Solve(self):
         r = 4
         problem = Stronginc3()
-        params = SolverParameters(r=r, eps=self.epsVal, epsR=0.01)
+        params = SolverParameters(r=r, eps=self.epsVal, eps_r=0.01)
 
         number_of_global_trials = 512
 
         self.checkIsSolved(problem, params, number_of_global_trials)
 
     def test_Romeijn3c_Solve(self):
         r = 4
         problem = Romeijn3c()
-        params = SolverParameters(r=r, eps=self.epsVal, epsR=0.01)
+        params = SolverParameters(r=r, eps=self.epsVal, eps_r=0.01)
 
         number_of_global_trials = 702
 
         self.checkIsSolved(problem, params, number_of_global_trials)
 
     def test_Romeijn5c_Solve(self):
         r = 4
         problem = Romeijn5c()
-        params = SolverParameters(r=r, eps=self.epsVal, epsR=0.01)
+        params = SolverParameters(r=r, eps=self.epsVal, eps_r=0.01)
 
         number_of_global_trials = 193
 
         self.checkIsSolved(problem, params, number_of_global_trials)
 
 
 """Executing the tests in the above test case class"""
```

