# Comparing `tmp/ivy-builder-1.1.8.tar.gz` & `tmp/ivy-builder-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivy-builder-1.1.8.tar", last modified: Wed Dec  1 08:48:37 2021, max compression
+gzip compressed data, was "ivy-builder-1.1.9.tar", last modified: Wed Dec  1 16:17:53 2021, max compression
```

## Comparing `ivy-builder-1.1.8.tar` & `ivy-builder-1.1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:37.054328 ivy-builder-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11411 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-12-01 08:48:37.054328 ivy-builder-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12845 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:37.050328 ivy-builder-1.1.8/ivy_builder/
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:37.050328 ivy-builder-1.1.8/ivy_builder/abstract/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/abstract/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/abstract/network.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/abstract/network_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    25719 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/abstract/trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)    21619 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/abstract/tuner.py
--rw-r--r--   0 runner    (1001) docker     (121)    36832 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2048 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/checkpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:37.050328 ivy-builder-1.1.8/ivy_builder/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30857 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/data_loaders/seq_data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:37.050328 ivy-builder-1.1.8/ivy_builder/data_loaders/specs/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/data_loaders/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4150 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/data_loaders/specs/seq_data_loader_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    26374 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:37.054328 ivy-builder-1.1.8/ivy_builder/empty/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      714 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/empty/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/empty/network.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/empty/trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5316 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:37.054328 ivy-builder-1.1.8/ivy_builder/specs/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/specs/data_loader_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/specs/dataset_dirs.py
--rw-r--r--   0 runner    (1001) docker     (121)      557 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/specs/dataset_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2531 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/specs/network_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/specs/spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     4387 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/specs/trainer_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder/specs/tuner_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:37.050328 ivy-builder-1.1.8/ivy_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-12-01 08:48:37.000000 ivy-builder-1.1.8/ivy_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2021-12-01 08:48:37.000000 ivy-builder-1.1.8/ivy_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 08:48:37.000000 ivy-builder-1.1.8/ivy_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-01 08:48:37.000000 ivy-builder-1.1.8/ivy_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-12-01 08:48:37.000000 ivy-builder-1.1.8/ivy_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:37.054328 ivy-builder-1.1.8/ivy_builder_demos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7104 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder_demos/full_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/ivy_builder_demos/simple_example.py
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:48:37.054328 ivy-builder-1.1.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2116 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/scripts/format_dataset_containers.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      124 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/scripts/print_json_args.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2596 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/scripts/remove_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2481 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/scripts/reset_to_defaults.sh
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-01 08:48:37.054328 ivy-builder-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2021-12-01 08:48:20.000000 ivy-builder-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:17:53.672113 ivy-builder-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11411 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1607 2021-12-01 16:17:53.672113 ivy-builder-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    12824 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:17:53.668113 ivy-builder-1.1.9/ivy_builder/
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:17:53.668113 ivy-builder-1.1.9/ivy_builder/abstract/
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/abstract/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/abstract/network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/abstract/network_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25719 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/abstract/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21619 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/abstract/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36832 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2048 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/checkpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:17:53.668113 ivy-builder-1.1.9/ivy_builder/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30857 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/data_loaders/seq_data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:17:53.668113 ivy-builder-1.1.9/ivy_builder/data_loaders/specs/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/data_loaders/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4150 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/data_loaders/specs/seq_data_loader_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26374 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:17:53.672113 ivy-builder-1.1.9/ivy_builder/empty/
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/empty/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/empty/network.py
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/empty/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5316 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:17:53.672113 ivy-builder-1.1.9/ivy_builder/specs/
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/specs/data_loader_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/specs/dataset_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/specs/dataset_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2531 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/specs/network_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/specs/spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4387 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/specs/trainer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder/specs/tuner_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:17:53.668113 ivy-builder-1.1.9/ivy_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1607 2021-12-01 16:17:53.000000 ivy-builder-1.1.9/ivy_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2021-12-01 16:17:53.000000 ivy-builder-1.1.9/ivy_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 16:17:53.000000 ivy-builder-1.1.9/ivy_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-01 16:17:53.000000 ivy-builder-1.1.9/ivy_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-12-01 16:17:53.000000 ivy-builder-1.1.9/ivy_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:17:53.672113 ivy-builder-1.1.9/ivy_builder_demos/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7104 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder_demos/full_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3161 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/ivy_builder_demos/simple_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:17:53.672113 ivy-builder-1.1.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2116 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/scripts/format_dataset_containers.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      124 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/scripts/print_json_args.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2596 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/scripts/remove_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2481 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/scripts/reset_to_defaults.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-01 16:17:53.672113 ivy-builder-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4300 2021-12-01 16:17:39.000000 ivy-builder-1.1.9/setup.py
```

### Comparing `ivy-builder-1.1.8/LICENSE` & `ivy-builder-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/PKG-INFO` & `ivy-builder-1.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 Metadata-Version: 2.1
 Name: ivy-builder
-Version: 1.1.8
+Version: 1.1.9
 Summary: Build custom Ivy training tasks with clear, hierarchical and robust user specifications.
 Home-page: https://ivy-dl.org/builder
 Author: Ivy Team
 Author-email: ivydl.team@gmail.com
 License: Apache 2.0
 Project-URL: Docs, https://ivy-dl.org/builder/
 Project-URL: Source, https://github.com/ivy-dl/builder
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
+.. image:: https://github.com/ivy-dl/builder/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 
 
 **Build custom Ivy training tasks with clear, hierarchical and robust user specifications.**
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/logos/supported/frameworks.png?raw=true
+   :width: 100%
+
 **Ivy Libraries**
 
 There are a host of derived libraries written in Ivy, in the areas of mechanics, 3D vision, robotics, gym environments,
 neural memory, pre-trained models + implementations, and builder tools with trainers, data loaders and more. Click on
 the icons below to learn more!
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_libraries.png?raw=true
+   :width: 100%
+
```

### Comparing `ivy-builder-1.1.8/README.rst` & `ivy-builder-1.1.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-.. raw:: html
-
-    <p align="center">
-        <img width="75%" style="display: block;" src='docs/partial_source/logos/logo.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/builder/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 .. raw:: html
 
     <br/>
     <a href="https://pypi.org/project/ivy-builder">
         <img style="float: left; padding-right: 4px; padding-bottom: 4px;" src="https://badge.fury.io/py/ivy-builder.svg">
     </a>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-.. raw:: html
-                     [docs/partial_source/logos/logo.png]
-.. raw:: html
+.. image:: https://github.com/ivy-dl/builder/blob/master/docs/partial_source/
+logos/logo.png?raw=true :width: 100% .. raw:: html
 [https://badge.fury.io/py/ivy-builder.svg] [https://img.shields.io/pypi/l/ivy-
 builder] [https://img.shields.io/github/workflow/status/ivy-dl/builder/
 docs?label=docs] [https://img.shields.io/github/workflow/status/ivy-dl/builder/
 nightly-tests?label=nightly] [https://img.shields.io/discord/
 799879767196958751?color=blue&label=%20&logo=discord&logoColor=white]
 **Build custom Ivy training tasks with clear, hierarchical and robust user
 specifications.** .. raw:: html
```

### Comparing `ivy-builder-1.1.8/ivy_builder/abstract/data_loader.py` & `ivy-builder-1.1.9/ivy_builder/abstract/data_loader.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/abstract/network.py` & `ivy-builder-1.1.9/ivy_builder/abstract/network.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/abstract/network_group.py` & `ivy-builder-1.1.9/ivy_builder/abstract/network_group.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/abstract/trainer.py` & `ivy-builder-1.1.9/ivy_builder/abstract/trainer.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/abstract/tuner.py` & `ivy-builder-1.1.9/ivy_builder/abstract/tuner.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/builder.py` & `ivy-builder-1.1.9/ivy_builder/builder.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/checkpoints.py` & `ivy-builder-1.1.9/ivy_builder/checkpoints.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/data_loaders/seq_data_loader.py` & `ivy-builder-1.1.9/ivy_builder/data_loaders/seq_data_loader.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/data_loaders/specs/seq_data_loader_spec.py` & `ivy-builder-1.1.9/ivy_builder/data_loaders/specs/seq_data_loader_spec.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/dataset.py` & `ivy-builder-1.1.9/ivy_builder/dataset.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/empty/data_loader.py` & `ivy-builder-1.1.9/ivy_builder/empty/data_loader.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/empty/network.py` & `ivy-builder-1.1.9/ivy_builder/empty/network.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/empty/trainer.py` & `ivy-builder-1.1.9/ivy_builder/empty/trainer.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/scheduler.py` & `ivy-builder-1.1.9/ivy_builder/scheduler.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/specs/data_loader_spec.py` & `ivy-builder-1.1.9/ivy_builder/specs/data_loader_spec.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/specs/dataset_spec.py` & `ivy-builder-1.1.9/ivy_builder/specs/dataset_spec.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/specs/network_spec.py` & `ivy-builder-1.1.9/ivy_builder/specs/network_spec.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/specs/spec.py` & `ivy-builder-1.1.9/ivy_builder/specs/spec.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/specs/trainer_spec.py` & `ivy-builder-1.1.9/ivy_builder/specs/trainer_spec.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder/specs/tuner_spec.py` & `ivy-builder-1.1.9/ivy_builder/specs/tuner_spec.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder.egg-info/PKG-INFO` & `ivy-builder-1.1.9/ivy_builder.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 Metadata-Version: 2.1
 Name: ivy-builder
-Version: 1.1.8
+Version: 1.1.9
 Summary: Build custom Ivy training tasks with clear, hierarchical and robust user specifications.
 Home-page: https://ivy-dl.org/builder
 Author: Ivy Team
 Author-email: ivydl.team@gmail.com
 License: Apache 2.0
 Project-URL: Docs, https://ivy-dl.org/builder/
 Project-URL: Source, https://github.com/ivy-dl/builder
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
+.. image:: https://github.com/ivy-dl/builder/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 
 
 **Build custom Ivy training tasks with clear, hierarchical and robust user specifications.**
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/logos/supported/frameworks.png?raw=true
+   :width: 100%
+
 **Ivy Libraries**
 
 There are a host of derived libraries written in Ivy, in the areas of mechanics, 3D vision, robotics, gym environments,
 neural memory, pre-trained models + implementations, and builder tools with trainers, data loaders and more. Click on
 the icons below to learn more!
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_libraries.png?raw=true
+   :width: 100%
+
```

### Comparing `ivy-builder-1.1.8/ivy_builder.egg-info/SOURCES.txt` & `ivy-builder-1.1.9/ivy_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder_demos/full_example.py` & `ivy-builder-1.1.9/ivy_builder_demos/full_example.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/ivy_builder_demos/simple_example.py` & `ivy-builder-1.1.9/ivy_builder_demos/simple_example.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/scripts/format_dataset_containers.py` & `ivy-builder-1.1.9/scripts/format_dataset_containers.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/scripts/remove_checkpoints.py` & `ivy-builder-1.1.9/scripts/remove_checkpoints.py`

 * *Files identical despite different names*

### Comparing `ivy-builder-1.1.8/scripts/reset_to_defaults.sh` & `ivy-builder-1.1.9/scripts/reset_to_defaults.sh`

 * *Files identical despite different names*

