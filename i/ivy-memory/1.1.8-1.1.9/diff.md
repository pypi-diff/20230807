# Comparing `tmp/ivy-memory-1.1.8.tar.gz` & `tmp/ivy-memory-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivy-memory-1.1.8.tar", last modified: Wed Dec  1 08:50:01 2021, max compression
+gzip compressed data, was "ivy-memory-1.1.9.tar", last modified: Wed Dec  1 16:23:02 2021, max compression
```

## Comparing `ivy-memory-1.1.8.tar` & `ivy-memory-1.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:50:01.107317 ivy-memory-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11411 2021-12-01 08:49:40.000000 ivy-memory-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-01 08:49:40.000000 ivy-memory-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9913 2021-12-01 08:50:01.107317 ivy-memory-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21782 2021-12-01 08:49:40.000000 ivy-memory-1.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:50:01.103317 ivy-memory-1.1.8/ivy_memory/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-12-01 08:49:40.000000 ivy-memory-1.1.8/ivy_memory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:50:01.107317 ivy-memory-1.1.8/ivy_memory/geometric/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-12-01 08:49:40.000000 ivy-memory-1.1.8/ivy_memory/geometric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7039 2021-12-01 08:49:40.000000 ivy-memory-1.1.8/ivy_memory/geometric/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)    33024 2021-12-01 08:49:40.000000 ivy-memory-1.1.8/ivy_memory/geometric/esm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:50:01.107317 ivy-memory-1.1.8/ivy_memory/learnt/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-12-01 08:49:40.000000 ivy-memory-1.1.8/ivy_memory/learnt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13349 2021-12-01 08:49:40.000000 ivy-memory-1.1.8/ivy_memory/learnt/ntm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 08:50:01.103317 ivy-memory-1.1.8/ivy_memory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9913 2021-12-01 08:50:01.000000 ivy-memory-1.1.8/ivy_memory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      399 2021-12-01 08:50:01.000000 ivy-memory-1.1.8/ivy_memory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 08:50:01.000000 ivy-memory-1.1.8/ivy_memory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-12-01 08:50:01.000000 ivy-memory-1.1.8/ivy_memory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-01 08:50:01.000000 ivy-memory-1.1.8/ivy_memory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-12-01 08:49:40.000000 ivy-memory-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-01 08:50:01.107317 ivy-memory-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2021-12-01 08:49:40.000000 ivy-memory-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:23:02.923319 ivy-memory-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11411 2021-12-01 16:22:48.000000 ivy-memory-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-01 16:22:48.000000 ivy-memory-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    10577 2021-12-01 16:23:02.923319 ivy-memory-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    21760 2021-12-01 16:22:48.000000 ivy-memory-1.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:23:02.923319 ivy-memory-1.1.9/ivy_memory/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-12-01 16:22:48.000000 ivy-memory-1.1.9/ivy_memory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:23:02.923319 ivy-memory-1.1.9/ivy_memory/geometric/
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2021-12-01 16:22:48.000000 ivy-memory-1.1.9/ivy_memory/geometric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7039 2021-12-01 16:22:48.000000 ivy-memory-1.1.9/ivy_memory/geometric/containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33024 2021-12-01 16:22:48.000000 ivy-memory-1.1.9/ivy_memory/geometric/esm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:23:02.923319 ivy-memory-1.1.9/ivy_memory/learnt/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-12-01 16:22:48.000000 ivy-memory-1.1.9/ivy_memory/learnt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13349 2021-12-01 16:22:48.000000 ivy-memory-1.1.9/ivy_memory/learnt/ntm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 16:23:02.923319 ivy-memory-1.1.9/ivy_memory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10577 2021-12-01 16:23:02.000000 ivy-memory-1.1.9/ivy_memory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2021-12-01 16:23:02.000000 ivy-memory-1.1.9/ivy_memory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 16:23:02.000000 ivy-memory-1.1.9/ivy_memory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-12-01 16:23:02.000000 ivy-memory-1.1.9/ivy_memory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-01 16:23:02.000000 ivy-memory-1.1.9/ivy_memory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2021-12-01 16:22:48.000000 ivy-memory-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-01 16:23:02.923319 ivy-memory-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4115 2021-12-01 16:22:48.000000 ivy-memory-1.1.9/setup.py
```

### Comparing `ivy-memory-1.1.8/LICENSE` & `ivy-memory-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ivy-memory-1.1.8/PKG-INFO` & `ivy-memory-1.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: ivy-memory
-Version: 1.1.8
+Version: 1.1.9
 Summary: End-to-end memory modules for machine learning developers, written in Ivy.
 Home-page: https://ivy-dl.org/memory
 Author: Ivy Team
 Author-email: ivydl.team@gmail.com
 License: Apache 2.0
 Project-URL: Docs, https://ivy-dl.org/memory/
 Project-URL: Source, https://github.com/ivy-dl/memory
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
+.. image:: https://github.com/ivy-dl/memory/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 
 
 **End-to-end memory modules for machine learning developers, written in Ivy.**
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/logos/supported/frameworks.png?raw=true
+   :width: 100%
+
 Contents
 --------
 
 * `Overview`_
 * `Run Through`_
 * `Interactive Demos`_
 * `Get Involed`_
@@ -49,14 +53,17 @@
 
 There are a host of derived libraries written in Ivy, in the areas of mechanics, 3D vision, robotics, gym environments,
 neural memory, pre-trained models + implementations, and builder tools with trainers, data loaders and more. Click on
 the icons below to learn more!
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_libraries.png?raw=true
+   :width: 100%
+
 
 
 
 
 
 
 
@@ -266,23 +273,29 @@
 **Learning to Copy with NTM**
 
 The first demo trains a Neural Turing Machine to copy a sequence from one memory bank to another.
 NTM can overfit to a single copy sequence very quickly, as show in the real-time visualization below.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_memory/demo_a.png?raw=true
+   :width: 100%
+
 **Mapping a Room with ESM**
 
 The second demo creates an egocentric map of a room, from a rotating camera.
 The raw image observations are shown on the left,
 and the incrementally constructed omni-directional ESM feature and depth images are shown on the right.
 While this example only projects color values into the memory, arbitrary neural network features can also be projected, for end-to-end training.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_memory/demo_b.png?raw=true
+   :width: 100%
+
 Get Involed
 -----------
 
 We hope the memory classes in this library are useful to a wide range of machine learning developers.
 However, there are many more areas of differentiable memory which could be covered by this library.
 
 If there are any particular functions or classes you feel are missing,
```

### Comparing `ivy-memory-1.1.8/README.rst` & `ivy-memory-1.1.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-.. raw:: html
-
-    <p align="center">
-        <img width="75%" style="display: block;" src='docs/partial_source/logos/logo.png'>
-    </p>
+.. image:: https://github.com/ivy-dl/memory/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 .. raw:: html
 
     <br/>
     <a href="https://pypi.org/project/ivy-memory">
         <img style="float: left; padding-right: 4px; padding-bottom: 4px;" src="https://badge.fury.io/py/ivy-memory.svg">
     </a>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-.. raw:: html
-                     [docs/partial_source/logos/logo.png]
-.. raw:: html
+.. image:: https://github.com/ivy-dl/memory/blob/master/docs/partial_source/
+logos/logo.png?raw=true :width: 100% .. raw:: html
 [https://badge.fury.io/py/ivy-memory.svg] [https://img.shields.io/github/
 workflow/status/ivy-dl/memory/docs?label=docs] [https://img.shields.io/github/
 workflow/status/ivy-dl/memory/nightly-tests?label=tests] [https://
 img.shields.io/discord/
 799879767196958751?color=blue&label=%20&logo=discord&logoColor=white]
 **End-to-end memory modules for machine learning developers, written in Ivy.**
 .. raw:: html
```

### Comparing `ivy-memory-1.1.8/ivy_memory/geometric/containers.py` & `ivy-memory-1.1.9/ivy_memory/geometric/containers.py`

 * *Files identical despite different names*

### Comparing `ivy-memory-1.1.8/ivy_memory/geometric/esm.py` & `ivy-memory-1.1.9/ivy_memory/geometric/esm.py`

 * *Files identical despite different names*

### Comparing `ivy-memory-1.1.8/ivy_memory/learnt/ntm.py` & `ivy-memory-1.1.9/ivy_memory/learnt/ntm.py`

 * *Files identical despite different names*

### Comparing `ivy-memory-1.1.8/ivy_memory.egg-info/PKG-INFO` & `ivy-memory-1.1.9/ivy_memory.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: ivy-memory
-Version: 1.1.8
+Version: 1.1.9
 Summary: End-to-end memory modules for machine learning developers, written in Ivy.
 Home-page: https://ivy-dl.org/memory
 Author: Ivy Team
 Author-email: ivydl.team@gmail.com
 License: Apache 2.0
 Project-URL: Docs, https://ivy-dl.org/memory/
 Project-URL: Source, https://github.com/ivy-dl/memory
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
+.. image:: https://github.com/ivy-dl/memory/blob/master/docs/partial_source/logos/logo.png?raw=true
+   :width: 100%
 
 
 
 **End-to-end memory modules for machine learning developers, written in Ivy.**
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/logos/supported/frameworks.png?raw=true
+   :width: 100%
+
 Contents
 --------
 
 * `Overview`_
 * `Run Through`_
 * `Interactive Demos`_
 * `Get Involed`_
@@ -49,14 +53,17 @@
 
 There are a host of derived libraries written in Ivy, in the areas of mechanics, 3D vision, robotics, gym environments,
 neural memory, pre-trained models + implementations, and builder tools with trainers, data loaders and more. Click on
 the icons below to learn more!
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_libraries.png?raw=true
+   :width: 100%
+
 
 
 
 
 
 
 
@@ -266,23 +273,29 @@
 **Learning to Copy with NTM**
 
 The first demo trains a Neural Turing Machine to copy a sequence from one memory bank to another.
 NTM can overfit to a single copy sequence very quickly, as show in the real-time visualization below.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_memory/demo_a.png?raw=true
+   :width: 100%
+
 **Mapping a Room with ESM**
 
 The second demo creates an egocentric map of a room, from a rotating camera.
 The raw image observations are shown on the left,
 and the incrementally constructed omni-directional ESM feature and depth images are shown on the right.
 While this example only projects color values into the memory, arbitrary neural network features can also be projected, for end-to-end training.
 
 
 
+.. image:: https://github.com/ivy-dl/ivy-dl.github.io/blob/master/img/externally_linked/ivy_memory/demo_b.png?raw=true
+   :width: 100%
+
 Get Involed
 -----------
 
 We hope the memory classes in this library are useful to a wide range of machine learning developers.
 However, there are many more areas of differentiable memory which could be covered by this library.
 
 If there are any particular functions or classes you feel are missing,
```

