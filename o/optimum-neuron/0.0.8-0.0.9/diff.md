# Comparing `tmp/optimum-neuron-0.0.8.tar.gz` & `tmp/optimum-neuron-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-neuron-0.0.8.tar", last modified: Mon Jul 24 15:59:54 2023, max compression
+gzip compressed data, was "optimum-neuron-0.0.9.tar", last modified: Mon Aug  7 18:41:47 2023, max compression
```

## Comparing `optimum-neuron-0.0.8.tar` & `optimum-neuron-0.0.9.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.509668 optimum-neuron-0.0.8/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    11357 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/LICENSE
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      651 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/MANIFEST.in
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    10778 2023-07-24 15:59:54.509976 optimum-neuron-0.0.8/PKG-INFO
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     9523 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/README.md
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.411312 optimum-neuron-0.0.8/optimum/
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.410793 optimum-neuron-0.0.8/optimum/commands/
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.423614 optimum-neuron-0.0.8/optimum/commands/export/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     5451 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/export/neuron.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     5327 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/export/neuronx.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.426373 optimum-neuron-0.0.8/optimum/commands/neuron/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1428 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/neuron/base.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     8808 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/neuron/cache.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2214 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/neuron/subcommands.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.428052 optimum-neuron-0.0.8/optimum/commands/register/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1270 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/register/register_export.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      755 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/commands/register/register_neuron.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.411122 optimum-neuron-0.0.8/optimum/exporters/
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.436245 optimum-neuron-0.0.8/optimum/exporters/neuron/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      998 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/__init__.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    11479 2023-07-24 15:26:45.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/__main__.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    14853 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/base.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1810 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/config.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    22613 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/convert.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     9979 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/model_configs.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    11140 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/exporters/neuron/utils.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.447655 optimum-neuron-0.0.8/optimum/neuron/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2993 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/__init__.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.455206 optimum-neuron-0.0.8/optimum/neuron/accelerate/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      785 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/__init__.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    23071 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/accelerator.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     4637 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/optimizer.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2212 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/scheduler.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    16801 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/state.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.459670 optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      789 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/__init__.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     7899 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/dataclasses.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1076 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/misc.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.467890 optimum-neuron-0.0.8/optimum/neuron/distributed/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      902 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/__init__.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    16900 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/base.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     4041 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/checkpointing.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     5459 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/decoder_models.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2844 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/encoder_models.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    11929 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/parallel_layers.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     3364 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/parallelizers_manager.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    23651 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/distributed/utils.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.470228 optimum-neuron-0.0.8/optimum/neuron/generation/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      668 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/generation/__init__.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    70566 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/generation/utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2337 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/hf_argparser.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    38265 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/modeling.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    19850 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/modeling_base.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    10917 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/modeling_decoder.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    21219 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/modeling_diffusion.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.473454 optimum-neuron-0.0.8/optimum/neuron/pipelines/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      666 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/pipelines/__init__.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.474301 optimum-neuron-0.0.8/optimum/neuron/pipelines/diffusers/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    12432 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/pipelines/diffusers/pipeline_stable_diffusion.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.475990 optimum-neuron-0.0.8/optimum/neuron/pipelines/transformers/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      658 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/pipelines/transformers/__init__.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     9124 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/pipelines/transformers/base.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    14102 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/trainer_callback.py
--rwxr-xr-x   0 michaelbenayoun   (501) staff       (20)    20239 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/trainers.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     9419 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/training_args.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.494068 optimum-neuron-0.0.8/optimum/neuron/utils/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1491 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/__init__.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     6793 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/argument_utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    34728 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/cache_utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    16574 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/compilation_utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      885 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/constant.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2002 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/import_utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    22030 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/misc.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1994 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/optimization_utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     7766 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/patching.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1734 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/require_utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1644 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/testing_utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    10602 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/training_utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     3102 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/optimum/neuron/utils/version_utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      639 2023-07-24 15:27:59.000000 optimum-neuron-0.0.8/optimum/neuron/version.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.498348 optimum-neuron-0.0.8/optimum_neuron.egg-info/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    10778 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/PKG-INFO
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     2801 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/SOURCES.txt
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)       39 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/dependency_links.txt
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)       66 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/entry_points.txt
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)        1 2023-07-24 14:56:07.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/not-zip-safe
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      507 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/requires.txt
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)        8 2023-07-24 15:59:54.000000 optimum-neuron-0.0.8/optimum_neuron.egg-info/top_level.txt
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     1161 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/pyproject.toml
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)      430 2023-07-24 15:59:54.511131 optimum-neuron-0.0.8/setup.cfg
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     3060 2023-07-24 15:59:45.000000 optimum-neuron-0.0.8/setup.py
-drwxr-xr-x   0 michaelbenayoun   (501) staff       (20)        0 2023-07-24 15:59:54.508808 optimum-neuron-0.0.8/tests/
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    35375 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_cache_utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     3415 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_compilation_utils.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    27302 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_examples.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     4696 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_generate.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    49320 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_modeling.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     5994 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_modeling_decoder.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     9277 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_trainer_callback.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)    17847 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_trainers.py
--rw-r--r--   0 michaelbenayoun   (501) staff       (20)     8584 2023-07-24 14:49:15.000000 optimum-neuron-0.0.8/tests/test_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.070421 optimum-neuron-0.0.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10778 2023-08-07 18:41:47.070421 optimum-neuron-0.0.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9523 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.058421 optimum-neuron-0.0.9/optimum/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.058421 optimum-neuron-0.0.9/optimum/commands/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.062421 optimum-neuron-0.0.9/optimum/commands/export/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5451 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/commands/export/neuron.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5327 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/commands/export/neuronx.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.062421 optimum-neuron-0.0.9/optimum/commands/neuron/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1428 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/commands/neuron/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8808 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/commands/neuron/cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2214 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/commands/neuron/subcommands.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.062421 optimum-neuron-0.0.9/optimum/commands/register/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1270 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/commands/register/register_export.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      755 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/commands/register/register_neuron.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.058421 optimum-neuron-0.0.9/optimum/exporters/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.062421 optimum-neuron-0.0.9/optimum/exporters/neuron/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      998 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/exporters/neuron/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11617 2023-08-05 21:24:05.000000 optimum-neuron-0.0.9/optimum/exporters/neuron/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14853 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/exporters/neuron/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1810 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/exporters/neuron/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23755 2023-08-05 21:24:05.000000 optimum-neuron-0.0.9/optimum/exporters/neuron/convert.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9979 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/exporters/neuron/model_configs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11354 2023-08-05 21:24:05.000000 optimum-neuron-0.0.9/optimum/exporters/neuron/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.066421 optimum-neuron-0.0.9/optimum/neuron/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2993 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.066421 optimum-neuron-0.0.9/optimum/neuron/accelerate/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      785 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/accelerate/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23071 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/accelerate/accelerator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4637 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/accelerate/optimizer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2212 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/accelerate/scheduler.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16801 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/accelerate/state.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.066421 optimum-neuron-0.0.9/optimum/neuron/accelerate/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      789 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/accelerate/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7899 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/accelerate/utils/dataclasses.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1076 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/accelerate/utils/misc.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.066421 optimum-neuron-0.0.9/optimum/neuron/distributed/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      902 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/distributed/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16900 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/distributed/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4041 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/distributed/checkpointing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4909 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/distributed/decoder_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3698 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/distributed/encoder_decoder_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2844 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/distributed/encoder_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17598 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/distributed/parallel_layers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3426 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/distributed/parallelizers_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24106 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/distributed/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.066421 optimum-neuron-0.0.9/optimum/neuron/generation/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      668 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/generation/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    70566 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/generation/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2337 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/hf_argparser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    38265 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/modeling.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19850 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/modeling_base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10917 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/modeling_decoder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21875 2023-08-07 16:38:42.000000 optimum-neuron-0.0.9/optimum/neuron/modeling_diffusion.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.066421 optimum-neuron-0.0.9/optimum/neuron/pipelines/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      666 2023-08-07 14:48:16.000000 optimum-neuron-0.0.9/optimum/neuron/pipelines/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.066421 optimum-neuron-0.0.9/optimum/neuron/pipelines/diffusers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14193 2023-08-05 21:48:14.000000 optimum-neuron-0.0.9/optimum/neuron/pipelines/diffusers/pipeline_stable_diffusion.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.066421 optimum-neuron-0.0.9/optimum/neuron/pipelines/transformers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/pipelines/transformers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9124 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/pipelines/transformers/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14102 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/trainer_callback.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    20239 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/trainers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9419 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/training_args.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.070421 optimum-neuron-0.0.9/optimum/neuron/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1491 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6793 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/utils/argument_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34728 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/utils/cache_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16574 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/utils/compilation_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/utils/constant.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/utils/import_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22048 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/utils/misc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1994 2023-07-19 22:10:56.000000 optimum-neuron-0.0.9/optimum/neuron/utils/optimization_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7766 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/utils/patching.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1734 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/utils/require_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1644 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/optimum/neuron/utils/testing_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10602 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/optimum/neuron/utils/training_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3102 2023-07-19 16:08:29.000000 optimum-neuron-0.0.9/optimum/neuron/utils/version_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      639 2023-08-07 16:41:49.000000 optimum-neuron-0.0.9/optimum/neuron/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.070421 optimum-neuron-0.0.9/optimum_neuron.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10778 2023-08-07 18:41:47.000000 optimum-neuron-0.0.9/optimum_neuron.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2854 2023-08-07 18:41:47.000000 optimum-neuron-0.0.9/optimum_neuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-08-07 18:41:47.000000 optimum-neuron-0.0.9/optimum_neuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       66 2023-08-07 18:41:47.000000 optimum-neuron-0.0.9/optimum_neuron.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-20 13:54:06.000000 optimum-neuron-0.0.9/optimum_neuron.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-08-07 18:41:47.000000 optimum-neuron-0.0.9/optimum_neuron.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-08-07 18:41:47.000000 optimum-neuron-0.0.9/optimum_neuron.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1161 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-08-07 18:41:47.070421 optimum-neuron-0.0.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3004 2023-08-07 18:41:15.000000 optimum-neuron-0.0.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-07 18:41:47.070421 optimum-neuron-0.0.9/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35375 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/tests/test_cache_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3415 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/tests/test_compilation_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27302 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/tests/test_examples.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4696 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/tests/test_generate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    49320 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/tests/test_modeling.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5994 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/tests/test_modeling_decoder.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9277 2023-08-04 15:19:06.000000 optimum-neuron-0.0.9/tests/test_trainer_callback.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17847 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/tests/test_trainers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8584 2023-07-19 14:52:33.000000 optimum-neuron-0.0.9/tests/test_utils.py
```

### Comparing `optimum-neuron-0.0.8/LICENSE` & `optimum-neuron-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/MANIFEST.in` & `optimum-neuron-0.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/PKG-INFO` & `optimum-neuron-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.8
+Version: 0.0.9
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `optimum-neuron-0.0.8/README.md` & `optimum-neuron-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/commands/export/neuron.py` & `optimum-neuron-0.0.9/optimum/commands/export/neuron.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/commands/export/neuronx.py` & `optimum-neuron-0.0.9/optimum/commands/export/neuronx.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/commands/neuron/base.py` & `optimum-neuron-0.0.9/optimum/commands/neuron/base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/commands/neuron/cache.py` & `optimum-neuron-0.0.9/optimum/commands/neuron/cache.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/commands/neuron/subcommands.py` & `optimum-neuron-0.0.9/optimum/commands/neuron/subcommands.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/commands/register/register_export.py` & `optimum-neuron-0.0.9/optimum/commands/register/register_export.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/commands/register/register_neuron.py` & `optimum-neuron-0.0.9/optimum/commands/register/register_neuron.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/exporters/neuron/__init__.py` & `optimum-neuron-0.0.9/optimum/exporters/neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/exporters/neuron/__main__.py` & `optimum-neuron-0.0.9/optimum/exporters/neuron/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,21 +104,25 @@
     )
     mandatory_axes = neuron_config_constructor.func.get_mandatory_axes_for_task(task)
     input_shapes = {name: getattr(args, name) for name in mandatory_axes}
     return input_shapes
 
 
 def normalize_stable_diffusion_input_shapes(
-    task: str,
     args: argparse.Namespace,
 ) -> Dict[str, Dict[str, int]]:
     args = vars(args) if isinstance(args, argparse.Namespace) else args
     mandatory_axes = set(getattr(inspect.getfullargspec(build_stable_diffusion_components_mandatory_shapes), "args"))
     # Remove `sequence_length` as diffusers will pad it to the max and remove number of channels .
-    mandatory_axes = mandatory_axes - {"sequence_length", "unet_num_channels", "vae_num_channels"}
+    mandatory_axes = mandatory_axes - {
+        "sequence_length",
+        "unet_num_channels",
+        "vae_encoder_num_channels",
+        "vae_decoder_num_channels",
+    }
     if not mandatory_axes.issubset(set(args.keys())):
         raise AttributeError(
             f"Shape of {mandatory_axes} are mandatory for neuron compilation, while {mandatory_axes.difference(args.keys())} are not given."
         )
     mandatory_shapes = {name: args[name] for name in mandatory_axes}
     input_shapes = build_stable_diffusion_components_mandatory_shapes(**mandatory_shapes)
     return input_shapes
@@ -126,28 +130,29 @@
 
 def infer_stable_diffusion_shapes_from_diffusers(
     input_shapes: Dict[str, Dict[str, int]],
     model: "StableDiffusionPipeline",
 ):
     sequence_length = model.tokenizer.model_max_length
     unet_num_channels = model.unet.config.in_channels
-    vae_num_channels = model.vae.config.latent_channels
+    vae_encoder_num_channels = model.vae.config.in_channels
+    vae_decoder_num_channels = model.vae.config.latent_channels
     vae_scale_factor = 2 ** (len(model.vae.config.block_out_channels) - 1) or 8
     height = input_shapes["unet_input_shapes"]["height"] // vae_scale_factor
     width = input_shapes["unet_input_shapes"]["width"] // vae_scale_factor
 
     input_shapes["text_encoder_input_shapes"].update({"sequence_length": sequence_length})
     input_shapes["unet_input_shapes"].update(
         {"sequence_length": sequence_length, "num_channels": unet_num_channels, "height": height, "width": width}
     )
     input_shapes["vae_encoder_input_shapes"].update(
-        {"num_channels": vae_num_channels, "height": height, "width": width}
+        {"num_channels": vae_encoder_num_channels, "height": height, "width": width}
     )
     input_shapes["vae_decoder_input_shapes"].update(
-        {"num_channels": vae_num_channels, "height": height, "width": width}
+        {"num_channels": vae_decoder_num_channels, "height": height, "width": width}
     )
 
 
 def main_export(
     model_name_or_path: str,
     output: Union[str, Path],
     compiler_kwargs: Dict[str, Any],
@@ -269,15 +274,15 @@
     # Retrieve CLI arguments
     args = parser.parse_args()
 
     task = infer_task(args.task, args.model)
     compiler_kwargs = infer_compiler_kwargs(args)
 
     if task == "stable-diffusion":
-        input_shapes = normalize_stable_diffusion_input_shapes(task, args)
+        input_shapes = normalize_stable_diffusion_input_shapes(args)
     else:
         input_shapes = normalize_input_shapes(task, args)
 
     main_export(
         model_name_or_path=args.model,
         output=args.output,
         compiler_kwargs=compiler_kwargs,
```

### Comparing `optimum-neuron-0.0.8/optimum/exporters/neuron/base.py` & `optimum-neuron-0.0.9/optimum/exporters/neuron/base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/exporters/neuron/config.py` & `optimum-neuron-0.0.9/optimum/exporters/neuron/config.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/exporters/neuron/convert.py` & `optimum-neuron-0.0.9/optimum/exporters/neuron/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import copy
 from collections import OrderedDict
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
+from packaging import version
 from transformers import PretrainedConfig
 
 from ...exporters.error_utils import OutputMatchError, ShapeError
 from ...neuron.utils import (
     convert_neuronx_compiler_args_to_neuron,
     is_neuron_available,
     is_neuronx_available,
@@ -336,15 +337,15 @@
             logger.error(
                 f"An error occured when trying to trace {model_name} with the error message: {e}.\n"
                 f"The export is failed and {model_name} neuron model won't be stored."
             )
 
     # remove models failed to export
     for i, model_name in failed_models:
-        output_file_names.pop(i)
+        output_file_names.pop(model_name)
         models_and_neuron_configs.pop(model_name)
 
     outputs = list(map(list, zip(*outputs)))
     return outputs
 
 
 def export(
@@ -422,28 +423,52 @@
 
         logger.info(f"Using Neuron: --auto-cast-type {auto_cast_type}")
         compiler_args.extend(["--auto-cast-type", auto_cast_type])
     else:
         compiler_args = ["--auto-cast", "none"]
 
     # diffusers specific
-    if hasattr(config._config, "_class_name") and "unet" in config._config._class_name.lower():
-        compiler_args.extend(["--model-type", "unet-inference"])
+    compiler_args = add_stable_diffusion_compiler_args(config, compiler_args)
 
     neuron_model = neuronx.trace(checked_model, dummy_inputs_tuple, compiler_args=compiler_args)
 
     if config.dynamic_batch_size is True:
         neuron_model = neuronx.dynamic_batch(neuron_model)
 
+    # diffusers specific
+    improve_stable_diffusion_loading(config, neuron_model)
+
     torch.jit.save(neuron_model, output)
     del neuron_model
 
     return config.inputs, config.outputs
 
 
+def add_stable_diffusion_compiler_args(config, compiler_args):
+    if hasattr(config._config, "_name_or_path"):
+        sd_components = ["text_encoder", "unet", "vae", "vae_encoder", "vae_decoder"]
+        if any(component in config._config._name_or_path.lower() for component in sd_components):
+            compiler_args.extend(["--enable-fast-loading-neuron-binaries"])
+        # unet
+        if "unet" in config._config._name_or_path.lower():
+            compiler_args.extend(["--model-type=unet-inference"])
+    return compiler_args
+
+
+def improve_stable_diffusion_loading(config, neuron_model):
+    if version.parse(neuronx.__version__) >= version.parse("1.13.1.1.9.0"):
+        if hasattr(config._config, "_name_or_path"):
+            sd_components = ["text_encoder", "unet", "vae", "vae_encoder", "vae_decoder"]
+            if any(component in config._config._name_or_path.lower() for component in sd_components):
+                neuronx.async_load(neuron_model)
+            # unet
+            if "unet" in config._config._name_or_path.lower():
+                neuronx.lazy_load(neuron_model)
+
+
 def export_neuron(
     model: "PreTrainedModel",
     config: "NeuronConfig",
     output: Path,
     auto_cast: Optional[str] = None,
     auto_cast_type: str = "bf16",
     disable_fast_relayout: bool = False,
```

### Comparing `optimum-neuron-0.0.8/optimum/exporters/neuron/model_configs.py` & `optimum-neuron-0.0.9/optimum/exporters/neuron/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/exporters/neuron/utils.py` & `optimum-neuron-0.0.9/optimum/exporters/neuron/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,22 +81,29 @@
         return output
 
 
 def build_stable_diffusion_components_mandatory_shapes(
     batch_size: Optional[int] = None,
     sequence_length: Optional[int] = None,
     unet_num_channels: Optional[int] = None,
-    vae_num_channels: Optional[int] = None,
+    vae_encoder_num_channels: Optional[int] = None,
+    vae_decoder_num_channels: Optional[int] = None,
     height: Optional[int] = None,
     width: Optional[int] = None,
 ):
     text_encoder_input_shapes = {"batch_size": batch_size, "sequence_length": sequence_length}
-    vae_encoder_input_shapes = vae_decoder_input_shapes = {
+    vae_encoder_input_shapes = {
         "batch_size": batch_size,
-        "num_channels": vae_num_channels,
+        "num_channels": vae_encoder_num_channels,
+        "height": height,
+        "width": width,
+    }
+    vae_decoder_input_shapes = {
+        "batch_size": batch_size,
+        "num_channels": vae_decoder_num_channels,
         "height": height,
         "width": width,
     }
     unet_input_shapes = {
         "batch_size": batch_size,
         "sequence_length": sequence_length,
         "num_channels": unet_num_channels,
```

### Comparing `optimum-neuron-0.0.8/optimum/neuron/__init__.py` & `optimum-neuron-0.0.9/optimum/neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/accelerate/__init__.py` & `optimum-neuron-0.0.9/optimum/neuron/accelerate/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/accelerate/accelerator.py` & `optimum-neuron-0.0.9/optimum/neuron/accelerate/accelerator.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/accelerate/optimizer.py` & `optimum-neuron-0.0.9/optimum/neuron/accelerate/optimizer.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/accelerate/scheduler.py` & `optimum-neuron-0.0.9/optimum/neuron/accelerate/scheduler.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/accelerate/state.py` & `optimum-neuron-0.0.9/optimum/neuron/accelerate/state.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/__init__.py` & `optimum-neuron-0.0.9/optimum/neuron/accelerate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/dataclasses.py` & `optimum-neuron-0.0.9/optimum/neuron/accelerate/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/accelerate/utils/misc.py` & `optimum-neuron-0.0.9/optimum/neuron/accelerate/utils/misc.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/distributed/__init__.py` & `optimum-neuron-0.0.9/optimum/neuron/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/distributed/base.py` & `optimum-neuron-0.0.9/optimum/neuron/distributed/base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/distributed/checkpointing.py` & `optimum-neuron-0.0.9/optimum/neuron/distributed/checkpointing.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/distributed/decoder_models.py` & `optimum-neuron-0.0.9/optimum/neuron/distributed/decoder_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,48 +13,65 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Classes related to `neuronx-distributed` to perform parallelism."""
 
 from typing import TYPE_CHECKING, Dict, Optional
 
 from .base import Parallelizer
-from .parallel_layers import ParallelMLP, ParallelSelfAttention
-from .utils import WeightInformation, embedding_to_parallel_embedding, linear_to_parallel_linear
+from .parallel_layers import ParallelEmbedding, ParallelMLP, ParallelSelfAttention
+from .utils import linear_to_parallel_linear
 
 
 if TYPE_CHECKING:
     import torch
     from transformers import PreTrainedModel
 
 
+class GPTNeoParallelEmbedding(ParallelEmbedding):
+    EMBEDDING_NAME = "transformer.wte"
+    LM_HEAD_NAME = "lm_head"
+
+
 class GPTNeoParallelSelfAttention(ParallelSelfAttention):
     QUERIES_NAME = "q_proj"
     KEYS_NAME = "k_proj"
     VALUES_NAME = "v_proj"
     OUTPUT_PROJECTION_NAME = "out_proj"
     ALL_HEAD_SIZE_NAME = "embed_dim"
 
 
+class GPTNeoParallelMLP(ParallelMLP):
+    FIRST_LINEAR_NAME = "c_fc"
+    SECOND_LINEAR_NAME = "c_proj"
+
+
 class GPTNeoParallelizer(Parallelizer):
     @classmethod
     def _parallelize(
         cls,
         model: "PreTrainedModel",
         orig_to_parallel: Optional[Dict[int, "torch.nn.Parameter"]],
         device: Optional["torch.device"] = None,
     ) -> "PreTrainedModel":
+        model = GPTNeoParallelEmbedding.transform(model, model, device=device)
         for block in model.transformer.h:
             block.attn.attention = GPTNeoParallelSelfAttention.transform(
                 model,
                 block.attn.attention,
                 device=device,
             )
+            block.mlp = GPTNeoParallelMLP.transform(model, block.mlp, device=device)
         return model
 
 
+class LlamaParallelEmbedding(ParallelEmbedding):
+    EMBEDDING_NAME = "model.embed_tokens"
+    LM_HEAD_NAME = "lm_head"
+
+
 class LlamaParallelSelfAttention(ParallelSelfAttention):
     QUERIES_NAME = "q_proj"
     KEYS_NAME = "k_proj"
     VALUES_NAME = "v_proj"
     OUTPUT_PROJECTION_NAME = "o_proj"
     NUM_ATTENTION_HEADS_NAME = "num_heads"
     ALL_HEAD_SIZE_NAME = "hidden_size"
@@ -110,34 +127,12 @@
     @classmethod
     def _parallelize(
         cls,
         model: "PreTrainedModel",
         orig_to_parallel: Optional[Dict[int, "torch.nn.Parameter"]],
         device: Optional["torch.device"] = None,
     ) -> "PreTrainedModel":
-        embedding_weight_info = None
-        lm_head_weight_info = None
-        lm_head_bias_weight_info = None
-        weight_map = getattr(model, "_weight_map", None)
-        if weight_map is not None:
-            embedding_weight_info = WeightInformation(
-                weight_map["model.embed_tokens.weight"],
-                "model.embed_tokens.weight",
-                device=device,
-            )
-            lm_head_weight_info = WeightInformation(weight_map["lm_head.weight"], "lm_head.weight", device=device)
-            if "lm_head.bias" in weight_map:
-                lm_head_bias_weight_info = WeightInformation(weight_map["lm_head.bias"], "lm_head.bias", device=device)
-
-        model.model.embed_tokens, model.lm_head = embedding_to_parallel_embedding(
-            model.model.embed_tokens,
-            lm_head_layer=model.lm_head,
-            embedding_weight_info=embedding_weight_info,
-            lm_head_weight_info=lm_head_weight_info,
-            lm_head_bias_weight_info=lm_head_bias_weight_info,
-            orig_to_parallel=orig_to_parallel,
-            device=device,
-        )
+        model = LlamaParallelEmbedding.transform(model, model, device=device)
         for layer in model.model.layers:
             layer.self_attn = LlamaParallelSelfAttention.transform(model, layer.self_attn, device=device)
             layer.mlp = LLamaParallelMLP.transform(model, layer.mlp, device=device)
         return model
```

### Comparing `optimum-neuron-0.0.8/optimum/neuron/distributed/encoder_models.py` & `optimum-neuron-0.0.9/optimum/neuron/distributed/encoder_models.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/distributed/parallelizers_manager.py` & `optimum-neuron-0.0.9/optimum/neuron/distributed/parallelizers_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import Dict, List, Type, Union
 
 from transformers import PreTrainedModel
 
 from .base import Parallelizer
 
 
-_PARALLELIZER_CLASSES_MODULE_NAMES = ["encoder_models", "decoder_models"]
+_PARALLELIZER_CLASSES_MODULE_NAMES = ["encoder_models", "decoder_models", "encoder_decoder_models"]
 
 
 def parallelizer_classes_resolver(
     model_type_to_parallelizer_class_name: Dict[str, str]
 ) -> Dict[str, Type[Parallelizer]]:
     modules = []
     for module_name in _PARALLELIZER_CLASSES_MODULE_NAMES:
@@ -51,14 +51,15 @@
 class ParallelizersManager:
     _MODEL_TYPE_TO_PARALLEL_MODEL_CLASS = parallelizer_classes_resolver(
         {
             "bert": "BertParallelizer",
             "roberta": "RobertaParallelizer",
             "gpt_neo": "GPTNeoParallelizer",
             "llama": "LlamaParallelizer",
+            "t5": "T5Parallelizer",
         }
     )
 
     @classmethod
     def get_supported_model_types(cls) -> List[str]:
         return list(cls._MODEL_TYPE_TO_PARALLEL_MODEL_CLASS.keys())
```

### Comparing `optimum-neuron-0.0.8/optimum/neuron/distributed/utils.py` & `optimum-neuron-0.0.9/optimum/neuron/distributed/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,33 +22,26 @@
 from typing import Any, Dict, Iterator, Literal, Optional, Tuple, Type, Union
 
 import torch
 from transformers import PretrainedConfig
 
 from ..utils import DynamicPatch, Patcher, is_neuronx_distributed_available, is_torch_xla_available
 from ..utils.misc import download_checkpoints_in_cache
-from ..utils.require_utils import requires_safetensors, requires_torch_xla
+from ..utils.require_utils import requires_neuronx_distributed, requires_safetensors, requires_torch_xla
 
 
 if is_torch_xla_available():
     import torch_xla.core.xla_model as xm
     from torch_xla.distributed.zero_redundancy_optimizer import ZeroRedundancyOptimizer
 else:
     ZeroRedundancyOptimizer = object
 
 
 if is_neuronx_distributed_available():
     from neuronx_distributed.parallel_layers import layers
-    from neuronx_distributed.parallel_layers.parallel_state import (
-        get_data_parallel_group,
-        get_data_parallel_rank,
-        get_data_parallel_size,
-        get_tensor_model_parallel_rank,
-        model_parallel_is_initialized,
-    )
 
 TENSOR_PARALLEL_SHARDS_DIR_NAME = "tensor_parallel_shards"
 
 
 @dataclass
 class WeightInformation:
     """
@@ -111,14 +104,15 @@
     if device != weight_info.device:
         raise ValueError(
             f"The specfified device must match the device in the `WeightInformation` but got {device} and "
             f"{weight_info.device}, the `WeightInformation` object is: {weight_info}."
         )
 
 
+@requires_neuronx_distributed
 def embedding_to_parallel_embedding(
     embedding_layer: "torch.nn.Embedding",
     lm_head_layer: Optional["torch.nn.Linear"] = None,
     embedding_weight_info: Optional[WeightInformation] = None,
     lm_head_weight_info: Optional[WeightInformation] = None,
     lm_head_bias_weight_info: Optional[WeightInformation] = None,
     orig_to_parallel: Optional[Dict[int, "torch.nn.Parameter"]] = None,
@@ -147,14 +141,19 @@
         device (`Optional[torch.device]`, defaults to `None`):
             The device where the new parallel layer should be put.
 
     Returns:
         `Union[ParallelEmbedding, Tuple[ParallelEmbedding", ColumnParallelLinear]]`: The parallel embedding and the
         parallel linear projection if specified.
     """
+    from neuronx_distributed.parallel_layers import layers
+    from neuronx_distributed.parallel_layers.parallel_state import (
+        get_tensor_model_parallel_rank,
+    )
+
     device = device if device is not None else torch.device("cpu")
 
     for weight_info in [embedding_weight_info, lm_head_weight_info, lm_head_bias_weight_info]:
         if weight_info is None:
             continue
         _validate_weight_info_device_matches_specified_device(device, weight_info)
 
@@ -208,14 +207,15 @@
 
     if lm_head_layer is None:
         return parallel_embedding_layer
 
     return parallel_embedding_layer, parallel_lm_head_layer
 
 
+@requires_neuronx_distributed
 def linear_to_parallel_linear(
     linear_layer: "torch.nn.Linear",
     axis: Union[Literal["row"], Literal["column"]],
     input_is_parallel: bool = False,
     gather_output: bool = True,
     linear_layer_weight_info: Optional[WeightInformation] = None,
     linear_layer_bias_weight_info: Optional[WeightInformation] = None,
@@ -249,14 +249,19 @@
             It might be deprecated soon.
         device (`Optional[torch.device]`, defaults to `None`):
             The device where the new parallel layer should be put.
 
     Returns:
         `Union[RowParallelLinear, ColumnParallelLinear]`: The parallel linear layer.
     """
+    from neuronx_distributed.parallel_layers import layers
+    from neuronx_distributed.parallel_layers.parallel_state import (
+        get_tensor_model_parallel_rank,
+    )
+
     if axis not in ["row", "column"]:
         raise ValueError(f'axis must either be "row" or "column", but {axis} was given here.')
 
     device = device if device is not None else torch.device("cpu")
     for weight_info in [linear_layer_weight_info, linear_layer_bias_weight_info]:
         if weight_info is None:
             continue
@@ -509,25 +514,33 @@
         optimizer_with_no_parameters._args_to_recreate = (args, kwargs)
         return optimizer_with_no_parameters
 
     return optimizer_constructor
 
 
 @requires_torch_xla
+@requires_neuronx_distributed
 class ZeroRedundancyOptimizerCompatibleWithTensorParallelism(ZeroRedundancyOptimizer):
     def __init__(
         self,
         params: Iterator[torch.Tensor],
         optimizer_class: Type[torch.optim.Optimizer],
         optimizer_dtype: Optional[Any] = None,
         grad_clipping: bool = True,
         max_norm: Optional[float] = None,
         pin_layout: bool = True,
         **defaults: Any,
     ):
+        from neuronx_distributed.parallel_layers.parallel_state import (
+            get_data_parallel_group,
+            get_data_parallel_rank,
+            get_data_parallel_size,
+            model_parallel_is_initialized,
+        )
+
         if not is_neuronx_distributed_available() or not model_parallel_is_initialized():
             return super().__init__(
                 params,
                 optimizer_class,
                 optimizer_dtype=optimizer_dtype,
                 grad_clipping=grad_clipping,
                 max_norm=max_norm,
```

### Comparing `optimum-neuron-0.0.8/optimum/neuron/generation/__init__.py` & `optimum-neuron-0.0.9/optimum/neuron/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/generation/utils.py` & `optimum-neuron-0.0.9/optimum/neuron/generation/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/hf_argparser.py` & `optimum-neuron-0.0.9/optimum/neuron/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/modeling.py` & `optimum-neuron-0.0.9/optimum/neuron/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/modeling_base.py` & `optimum-neuron-0.0.9/optimum/neuron/modeling_base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/modeling_decoder.py` & `optimum-neuron-0.0.9/optimum/neuron/modeling_decoder.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/modeling_diffusion.py` & `optimum-neuron-0.0.9/optimum/neuron/modeling_diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,22 @@
     config_name = "model_index.json"
     sub_component_config_name = "config.json"
 
     def __init__(
         self,
         text_encoder: torch.jit._script.ScriptModule,
         unet: torch.jit._script.ScriptModule,
-        vae_encoder: torch.jit._script.ScriptModule,
+        # TODO: Fix vae encoder export
+        # vae_encoder: torch.jit._script.ScriptModule,
         vae_decoder: torch.jit._script.ScriptModule,
         config: Dict[str, Any],
         tokenizer: CLIPTokenizer,
         scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
         feature_extractor: Optional[CLIPFeatureExtractor] = None,
+        device_ids: Optional[List[int]] = [],
         configs: Optional[Dict[str, "PretrainedConfig"]] = None,
         neuron_configs: Optional[Dict[str, "NeuronConfig"]] = None,
         model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
         model_and_config_save_paths: Optional[Dict[str, Tuple[str, Path]]] = None,
     ):
         """
         Args:
@@ -98,58 +100,65 @@
             tokenizer (`CLIPTokenizer`):
                 Tokenizer of class
                 [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
             scheduler (`Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]`):
                 A scheduler to be used in combination with the U-NET component to denoise the encoded image latents.
             feature_extractor (`Optional[CLIPFeatureExtractor]`, defaults to `None`):
                 A model extracting features from generated images to be used as inputs for the `safety_checker`
+            device_ids (Optional[List[int]], defaults to `[]`):
+                A list of integers that specify the NeuronCores to use for parallelization
             configs (Optional[Dict[str, "PretrainedConfig"]], defaults to `None`):
                 A dictionary configurations for components of the pipeline.
             neuron_configs (Optional["NeuronConfig"], defaults to `None`):
                 A list of Neuron configurations.
             model_save_dir (`Optional[Union[str, Path, TemporaryDirectory]]`, defaults to `None`):
                 The directory under which the exported Neuron models were saved.
             model_and_config_save_paths (`Optional[Dict[str, Tuple[str, Path]]]`, defaults to `None`):
                 The paths where exported Neuron models were saved.
         """
 
         self._internal_dict = config
+        self.device_ids = device_ids
         self.configs = configs
         self.neuron_configs = neuron_configs
+        self.dynamic_batch_size = all(
+            neuron_config._config.neuron["dynamic_batch_size"] for neuron_config in self.neuron_configs.values()
+        )
 
         self.text_encoder = NeuronModelTextEncoder(
             text_encoder,
             self,
             self.configs[DIFFUSION_MODEL_TEXT_ENCODER_NAME],
             self.neuron_configs[DIFFUSION_MODEL_TEXT_ENCODER_NAME],
         )
         self.unet = NeuronModelUnet(
             unet, self, self.configs[DIFFUSION_MODEL_UNET_NAME], self.neuron_configs[DIFFUSION_MODEL_UNET_NAME]
         )
-        self.vae_encoder = NeuronModelVaeEncoder(
-            vae_encoder,
-            self,
-            self.configs[DIFFUSION_MODEL_VAE_ENCODER_NAME],
-            self.neuron_configs[DIFFUSION_MODEL_VAE_ENCODER_NAME],
-        )
+        # TODO: Fix vae encoder export
+        # self.vae_encoder = NeuronModelVaeEncoder(
+        #     vae_encoder,
+        #     self,
+        #     self.configs[DIFFUSION_MODEL_VAE_ENCODER_NAME],
+        #     self.neuron_configs[DIFFUSION_MODEL_VAE_ENCODER_NAME],
+        # )
         self.vae_decoder = NeuronModelVaeDecoder(
             vae_decoder,
             self,
             self.configs[DIFFUSION_MODEL_VAE_DECODER_NAME],
             self.neuron_configs[DIFFUSION_MODEL_VAE_DECODER_NAME],
         )
 
         self.tokenizer = tokenizer
         self.scheduler = scheduler
         self.feature_extractor = feature_extractor
         self.safety_checker = None
         sub_models = {
             DIFFUSION_MODEL_TEXT_ENCODER_NAME: self.text_encoder,
             DIFFUSION_MODEL_UNET_NAME: self.unet,
-            DIFFUSION_MODEL_VAE_ENCODER_NAME: self.vae_encoder,
+            # DIFFUSION_MODEL_VAE_ENCODER_NAME: self.vae_encoder,
             DIFFUSION_MODEL_VAE_DECODER_NAME: self.vae_decoder,
         }
         for name in sub_models.keys():
             self._internal_dict[name] = ("optimum", sub_models[name].__class__.__name__)
         self._internal_dict.pop("vae", None)
 
         self._attributes_init(model_save_dir)
@@ -222,15 +231,15 @@
         cache_dir: Optional[str] = None,
         text_encoder_file_name: Optional[str] = NEURON_FILE_NAME,
         unet_file_name: Optional[str] = NEURON_FILE_NAME,
         vae_encoder_file_name: Optional[str] = NEURON_FILE_NAME,
         vae_decoder_file_name: Optional[str] = NEURON_FILE_NAME,
         local_files_only: bool = False,
         model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
-        device_ids: Optional[List[int]] = None,
+        device_ids: Optional[List[int]] = [],
         **kwargs,  # To share kwargs only available for `_from_transformers`
     ):
         model_id = str(model_id)
         sub_models_to_load, _, _ = cls.extract_init_dict(config)
         sub_models_names = set(sub_models_to_load.keys()).intersection({"feature_extractor", "tokenizer", "scheduler"})
         sub_models = {}
 
@@ -278,18 +287,19 @@
                 new_model_save_dir / DIFFUSION_MODEL_TEXT_ENCODER_NAME / text_encoder_file_name,
                 new_model_save_dir / DIFFUSION_MODEL_TEXT_ENCODER_NAME / cls.sub_component_config_name,
             ),
             "unet": (
                 new_model_save_dir / DIFFUSION_MODEL_UNET_NAME / unet_file_name,
                 new_model_save_dir / DIFFUSION_MODEL_UNET_NAME / cls.sub_component_config_name,
             ),
-            "vae_encoder": (
-                new_model_save_dir / DIFFUSION_MODEL_VAE_ENCODER_NAME / vae_encoder_file_name,
-                new_model_save_dir / DIFFUSION_MODEL_VAE_ENCODER_NAME / cls.sub_component_config_name,
-            ),
+            # TODO: Fix vae encoder export
+            # "vae_encoder": (
+            #     new_model_save_dir / DIFFUSION_MODEL_VAE_ENCODER_NAME / vae_encoder_file_name,
+            #     new_model_save_dir / DIFFUSION_MODEL_VAE_ENCODER_NAME / cls.sub_component_config_name,
+            # ),
             "vae_decoder": (
                 new_model_save_dir / DIFFUSION_MODEL_VAE_DECODER_NAME / vae_decoder_file_name,
                 new_model_save_dir / DIFFUSION_MODEL_VAE_DECODER_NAME / cls.sub_component_config_name,
             ),
         }
 
         # Re-build pretrained configs and neuron configs
@@ -305,29 +315,32 @@
             unet = torch_neuronx.DataParallel(
                 torch.jit.load(model_and_config_save_paths["unet"][0]),
                 device_ids,
                 set_dynamic_batching=neuron_configs[DIFFUSION_MODEL_UNET_NAME].dynamic_batch_size,
             )
         else:
             unet = cls.load_model(model_and_config_save_paths["unet"][0])
-        vae_encoder = cls.load_model(model_and_config_save_paths["vae_encoder"][0])
+        # TODO: Fix vae encoder export
+        # vae_encoder = cls.load_model(model_and_config_save_paths["vae_encoder"][0])
         vae_decoder = cls.load_model(model_and_config_save_paths["vae_decoder"][0])
 
         if model_save_dir is None:
             model_save_dir = new_model_save_dir
 
         return cls(
             text_encoder=text_encoder,
             unet=unet,
-            vae_encoder=vae_encoder,
+            # TODO: Fix vae encoder export
+            # vae_encoder=vae_encoder,
             vae_decoder=vae_decoder,
             config=config,
             tokenizer=sub_models["tokenizer"],
             scheduler=sub_models["scheduler"],
             feature_extractor=sub_models.pop("feature_extractor", None),
+            device_ids=device_ids,
             configs=configs,
             neuron_configs=neuron_configs,
             model_save_dir=model_save_dir,
             model_and_config_save_paths=model_and_config_save_paths,
         )
 
     @classmethod
@@ -344,22 +357,22 @@
         trust_remote_code: bool = False,
         task: Optional[str] = None,
         auto_cast: Optional[str] = None,
         auto_cast_type: Optional[str] = None,
         disable_fast_relayout: Optional[bool] = False,
         disable_fallback: bool = False,
         dynamic_batch_size: bool = False,
-        device_ids: Optional[List[int]] = None,
+        device_ids: Optional[List[int]] = [],
         **kwargs_shapes,
     ) -> "NeuronStableDiffusionPipelineBase":
         if task is None:
             task = TasksManager.infer_task_from_model(cls.auto_model_class)
 
         # mandatory shapes
-        input_shapes = normalize_stable_diffusion_input_shapes(task, kwargs_shapes)
+        input_shapes = normalize_stable_diffusion_input_shapes(kwargs_shapes)
 
         # Get compilation arguments
         auto_cast_type = None if auto_cast is None else auto_cast_type
         compiler_kwargs = {
             "auto_cast": auto_cast,
             "auto_cast_type": auto_cast_type,
             "disable_fast_relayout": disable_fast_relayout,
```

### Comparing `optimum-neuron-0.0.8/optimum/neuron/pipelines/__init__.py` & `optimum-neuron-0.0.9/optimum/neuron/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/pipelines/diffusers/pipeline_stable_diffusion.py` & `optimum-neuron-0.0.9/optimum/neuron/pipelines/diffusers/pipeline_stable_diffusion.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import torch
 from diffusers import StableDiffusionPipeline
 from diffusers.loaders import LoraLoaderMixin, TextualInversionLoaderMixin
 from diffusers.pipelines.stable_diffusion import StableDiffusionPipelineOutput
 from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion import rescale_noise_cfg
+from diffusers.utils import randn_tensor
 
 
 logger = logging.getLogger(__name__)
 
 
 class StableDiffusionPipelineMixin(StableDiffusionPipeline):
     # Adapted from https://github.com/huggingface/diffusers/blob/v0.18.2/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py#L302
     def _encode_prompt(
         self,
         prompt,
-        device,
         num_images_per_prompt,
         do_classifier_free_guidance,
         negative_prompt=None,
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
         lora_scale: Optional[float] = None,
     ):
@@ -132,14 +132,32 @@
             # For classifier free guidance, we need to do two forward passes.
             # Here we concatenate the unconditional and text embeddings into a single batch
             # to avoid doing two forward passes
             prompt_embeds = torch.cat([negative_prompt_embeds, prompt_embeds])
 
         return prompt_embeds
 
+    # Adapted from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
+    def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, generator, latents=None):
+        shape = (batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
+        if isinstance(generator, list) and len(generator) != batch_size:
+            raise ValueError(
+                f"You have passed a list of generators of length {len(generator)}, but requested an effective batch"
+                f" size of {batch_size}. Make sure the batch size matches the length of the generators."
+            )
+
+        if latents is None:
+            latents = randn_tensor(shape, generator=generator, dtype=dtype)
+        elif latents.shape != shape:
+            raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {shape}")
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
+        return latents
+
     # Adapted from https://github.com/huggingface/diffusers/blob/v0.18.2/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py#L566
     def __call__(
         self,
         prompt: Union[str, List[str]] = None,
         height: Optional[int] = None,
         width: Optional[int] = None,
         num_inference_steps: int = 50,
@@ -171,48 +189,45 @@
         if prompt is not None and isinstance(prompt, str):
             batch_size = 1
         elif prompt is not None and isinstance(prompt, list):
             batch_size = len(prompt)
         else:
             batch_size = prompt_embeds.shape[0]
 
-        device = self._execution_device
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
-        do_classifier_free_guidance = guidance_scale > 1.0
+        do_classifier_free_guidance = guidance_scale > 1.0 and (self.dynamic_batch_size or len(self.device_ids) == 2)
 
         # 3. Encode input prompt
         text_encoder_lora_scale = (
             cross_attention_kwargs.get("scale", None) if cross_attention_kwargs is not None else None
         )
         prompt_embeds = self._encode_prompt(
             prompt,
-            device,
             num_images_per_prompt,
             do_classifier_free_guidance,
             negative_prompt,
             prompt_embeds=prompt_embeds,
             negative_prompt_embeds=negative_prompt_embeds,
             lora_scale=text_encoder_lora_scale,
         )
 
         # 4. Prepare timesteps
-        self.scheduler.set_timesteps(num_inference_steps, device=device)
+        self.scheduler.set_timesteps(num_inference_steps)
         timesteps = self.scheduler.timesteps
 
         # 5. Prepare latent variables
         num_channels_latents = self.unet.config.in_channels
         latents = self.prepare_latents(
             batch_size * num_images_per_prompt,
             num_channels_latents,
             height,
             width,
             prompt_embeds.dtype,
-            device,
             generator,
             latents,
         )
 
         # 6. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
         extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
@@ -249,15 +264,15 @@
                     progress_bar.update()
                     if callback is not None and i % callback_steps == 0:
                         callback(i, t, latents)
 
         if not output_type == "latent":
             # [Modified] Replace with pre-compiled
             image = self.vae_decoder(latents / getattr(self.vae_decoder.config, "scaling_factor", 0.18215))[0]
-            image, has_nsfw_concept = self.run_safety_checker(image, device, prompt_embeds.dtype)
+            image, has_nsfw_concept = self.run_safety_checker(image, prompt_embeds.dtype)
         else:
             image = latents
             has_nsfw_concept = None
 
         if has_nsfw_concept is None:
             do_denormalize = [True] * image.shape[0]
         else:
@@ -269,7 +284,21 @@
         if hasattr(self, "final_offload_hook") and self.final_offload_hook is not None:
             self.final_offload_hook.offload()
 
         if not return_dict:
             return (image, has_nsfw_concept)
 
         return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
+
+    def run_safety_checker(self, image, dtype):
+        if self.safety_checker is None:
+            has_nsfw_concept = None
+        else:
+            if torch.is_tensor(image):
+                feature_extractor_input = self.image_processor.postprocess(image, output_type="pil")
+            else:
+                feature_extractor_input = self.image_processor.numpy_to_pil(image)
+            safety_checker_input = self.feature_extractor(feature_extractor_input, return_tensors="pt")
+            image, has_nsfw_concept = self.safety_checker(
+                images=image, clip_input=safety_checker_input.pixel_values.to(dtype)
+            )
+        return image, has_nsfw_concept
```

### Comparing `optimum-neuron-0.0.8/optimum/neuron/pipelines/transformers/__init__.py` & `optimum-neuron-0.0.9/optimum/neuron/pipelines/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/pipelines/transformers/base.py` & `optimum-neuron-0.0.9/optimum/neuron/pipelines/transformers/base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/trainer_callback.py` & `optimum-neuron-0.0.9/optimum/neuron/trainer_callback.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/trainers.py` & `optimum-neuron-0.0.9/optimum/neuron/trainers.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/training_args.py` & `optimum-neuron-0.0.9/optimum/neuron/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/__init__.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/argument_utils.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/argument_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/cache_utils.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/compilation_utils.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/compilation_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/constant.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/import_utils.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/misc.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,16 @@
         if log:
             logger.info(f"Converting {weight_file} to safetensors")
         checkpoint = torch.load(weight_file)
         data_pointers = set()
         for k, v in checkpoint.items():
             if id(v.data) in data_pointers:
                 v = v.clone()
-            checkpoint[k] = v.contiguous()
+            v = v.contiguous()
+            checkpoint[k] = v
             data_pointers.add(id(v.data))
         save_file(checkpoint, safetensors_path)
         del checkpoint
 
     return safetensors_path
```

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/optimization_utils.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/patching.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/patching.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/require_utils.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/require_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/testing_utils.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/training_utils.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/training_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/utils/version_utils.py` & `optimum-neuron-0.0.9/optimum/neuron/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/optimum/neuron/version.py` & `optimum-neuron-0.0.9/optimum/neuron/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

### Comparing `optimum-neuron-0.0.8/optimum_neuron.egg-info/PKG-INFO` & `optimum-neuron-0.0.9/optimum_neuron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.8
+Version: 0.0.9
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `optimum-neuron-0.0.8/optimum_neuron.egg-info/SOURCES.txt` & `optimum-neuron-0.0.9/optimum_neuron.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 optimum/neuron/accelerate/utils/__init__.py
 optimum/neuron/accelerate/utils/dataclasses.py
 optimum/neuron/accelerate/utils/misc.py
 optimum/neuron/distributed/__init__.py
 optimum/neuron/distributed/base.py
 optimum/neuron/distributed/checkpointing.py
 optimum/neuron/distributed/decoder_models.py
+optimum/neuron/distributed/encoder_decoder_models.py
 optimum/neuron/distributed/encoder_models.py
 optimum/neuron/distributed/parallel_layers.py
 optimum/neuron/distributed/parallelizers_manager.py
 optimum/neuron/distributed/utils.py
 optimum/neuron/generation/__init__.py
 optimum/neuron/generation/utils.py
 optimum/neuron/pipelines/__init__.py
```

### Comparing `optimum-neuron-0.0.8/pyproject.toml` & `optimum-neuron-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/setup.py` & `optimum-neuron-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "safetensors",
 ]
 
 QUALITY_REQUIRES = [
     "black",
     "ruff",
     "isort",
-#    "hf_doc_builder @ git+https://github.com/huggingface/doc-builder.git",
+    "hf_doc_builder",
 ]
 
 EXTRAS_REQUIRE = {
     "tests": TESTS_REQUIRE,
     "quality": QUALITY_REQUIRES,
     "neuron": [
         "wheel",
@@ -49,15 +49,15 @@
         "torch==1.13.1.*",
         "neuron-cc[tensorflow]==1.15.*",
         "protobuf",
         "torchvision",
     ],
     "neuronx": [
         "wheel",
-        "neuronx-cc==2.6.*",
+        "neuronx-cc==2.*",
         "torch-neuronx",
         "transformers-neuronx",
         "torch==1.13.1.*",
         "torchvision==0.14.*",
         "neuronx_distributed",
     ],
     "diffusers": ["diffusers"],
```

### Comparing `optimum-neuron-0.0.8/tests/test_cache_utils.py` & `optimum-neuron-0.0.9/tests/test_cache_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/tests/test_compilation_utils.py` & `optimum-neuron-0.0.9/tests/test_compilation_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/tests/test_examples.py` & `optimum-neuron-0.0.9/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/tests/test_generate.py` & `optimum-neuron-0.0.9/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/tests/test_modeling.py` & `optimum-neuron-0.0.9/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/tests/test_modeling_decoder.py` & `optimum-neuron-0.0.9/tests/test_modeling_decoder.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/tests/test_trainer_callback.py` & `optimum-neuron-0.0.9/tests/test_trainer_callback.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/tests/test_trainers.py` & `optimum-neuron-0.0.9/tests/test_trainers.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.8/tests/test_utils.py` & `optimum-neuron-0.0.9/tests/test_utils.py`

 * *Files identical despite different names*

