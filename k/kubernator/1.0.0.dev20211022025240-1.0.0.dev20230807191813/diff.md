# Comparing `tmp/kubernator-1.0.0.dev20211022025240.tar.gz` & `tmp/kubernator-1.0.0.dev20230807191813.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubernator-1.0.0.dev20211022025240.tar", last modified: Fri Oct 22 02:53:23 2021, max compression
+gzip compressed data, was "kubernator-1.0.0.dev20230807191813.tar", last modified: Mon Aug  7 19:18:55 2023, max compression
```

## Comparing `kubernator-1.0.0.dev20211022025240.tar` & `kubernator-1.0.0.dev20230807191813.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 02:53:23.650814 kubernator-1.0.0.dev20211022025240/
--rw-rw-r--   0 runner    (1001) docker     (121)       27 2021-10-22 02:53:18.000000 kubernator-1.0.0.dev20211022025240/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9475 2021-10-22 02:53:23.650814 kubernator-1.0.0.dev20211022025240/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 02:53:23.646814 kubernator-1.0.0.dev20211022025240/kubernator/
--rw-r--r--   0 runner    (1001) docker     (121)    11387 2021-10-22 02:53:18.000000 kubernator-1.0.0.dev20211022025240/kubernator/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-10-22 02:52:27.000000 kubernator-1.0.0.dev20211022025240/kubernator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15522 2021-10-22 02:52:27.000000 kubernator-1.0.0.dev20211022025240/kubernator/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    15518 2021-10-22 02:52:27.000000 kubernator-1.0.0.dev20211022025240/kubernator/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     8757 2021-10-22 02:52:27.000000 kubernator-1.0.0.dev20211022025240/kubernator/helm.py
--rw-r--r--   0 runner    (1001) docker     (121)     7622 2021-10-22 02:52:27.000000 kubernator-1.0.0.dev20211022025240/kubernator/istio.py
--rw-r--r--   0 runner    (1001) docker     (121)    18588 2021-10-22 02:52:27.000000 kubernator-1.0.0.dev20211022025240/kubernator/k8s.py
--rw-r--r--   0 runner    (1001) docker     (121)    25906 2021-10-22 02:52:27.000000 kubernator-1.0.0.dev20211022025240/kubernator/k8s_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     9430 2021-10-22 02:52:27.000000 kubernator-1.0.0.dev20211022025240/kubernator/kops.py
--rw-r--r--   0 runner    (1001) docker     (121)     5131 2021-10-22 02:52:27.000000 kubernator-1.0.0.dev20211022025240/kubernator/proc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8045 2021-10-22 02:52:27.000000 kubernator-1.0.0.dev20211022025240/kubernator/template.py
--rw-r--r--   0 runner    (1001) docker     (121)     2449 2021-10-22 02:52:27.000000 kubernator-1.0.0.dev20211022025240/kubernator/tf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 02:53:23.650814 kubernator-1.0.0.dev20211022025240/kubernator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9475 2021-10-22 02:53:23.000000 kubernator-1.0.0.dev20211022025240/kubernator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      533 2021-10-22 02:53:23.000000 kubernator-1.0.0.dev20211022025240/kubernator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 02:53:23.000000 kubernator-1.0.0.dev20211022025240/kubernator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-10-22 02:53:23.000000 kubernator-1.0.0.dev20211022025240/kubernator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 02:53:23.000000 kubernator-1.0.0.dev20211022025240/kubernator.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)      221 2021-10-22 02:53:23.000000 kubernator-1.0.0.dev20211022025240/kubernator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-10-22 02:53:23.000000 kubernator-1.0.0.dev20211022025240/kubernator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 02:53:23.000000 kubernator-1.0.0.dev20211022025240/kubernator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-22 02:53:23.650814 kubernator-1.0.0.dev20211022025240/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)    11223 2021-10-22 02:53:18.000000 kubernator-1.0.0.dev20211022025240/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:18:55.889252 kubernator-1.0.0.dev20230807191813/
+-rw-rw-r--   0 runner    (1001) docker     (123)       27 2023-08-07 19:18:51.000000 kubernator-1.0.0.dev20230807191813/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-08-07 19:18:55.885252 kubernator-1.0.0.dev20230807191813/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:18:55.885252 kubernator-1.0.0.dev20230807191813/kubernator/
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-08-07 19:18:51.000000 kubernator-1.0.0.dev20230807191813/kubernator/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/istio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25906 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/k8s_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/kops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-07 19:17:59.000000 kubernator-1.0.0.dev20230807191813/kubernator/tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:18:55.885252 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:18:55.000000 kubernator-1.0.0.dev20230807191813/kubernator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 19:18:55.889252 kubernator-1.0.0.dev20230807191813/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11276 2023-08-07 19:18:51.000000 kubernator-1.0.0.dev20230807191813/setup.py
```

### Comparing `kubernator-1.0.0.dev20211022025240/PKG-INFO` & `kubernator-1.0.0.dev20230807191813/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kubernator
-Version: 1.0.0.dev20211022025240
+Version: 1.0.0.dev20230807191813
 Summary: Kubernator is the a pluggable framework for K8S provisioning
 Home-page: https://github.com/karellen/kubernator
 Author: Express Systems USA, Inc.
 Author-email: 
 Maintainer: Karellen, Inc., Arcadiy Ivanov
 Maintainer-email: supervisor@karellen.co,arcadiy@karellen.co
 License: Apache License, Version 2.0
 Project-URL: Bug Tracker, https://github.com/karellen/kubernator/issues
 Project-URL: Documentation, https://github.com/karellen/kubernator/
 Project-URL: Source Code, https://github.com/karellen/kubernator/
 Keywords: kubernetes k8s kube top provisioning kOps terraform tf AWS
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Distributed Computing
@@ -211,9 +211,7 @@
         logger.warning("Resource %s in %s contains `replica` specification that will be removed. Use HPA!!!",
                        r, r.source)
         del r.manifest["spec"]["replicas"]
 
 
 ktor.k8s.add_transformer(remove_replicas)
 ```
-
-
```

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/LICENSE` & `kubernator-1.0.0.dev20230807191813/kubernator/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/__init__.py` & `kubernator-1.0.0.dev20230807191813/kubernator/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/api.py` & `kubernator-1.0.0.dev20230807191813/kubernator/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 import requests
 import yaml
 from appdirs import user_config_dir
 from jinja2 import (Environment,
                     ChainableUndefined,
                     make_logging_undefined,
                     Template as JinjaTemplate,
-                    contextfunction)
+                    pass_context)
 from jsonschema import validators
 
 _CACHE_HEADER_TRANSLATION = {"etag": "if-none-match",
                              "last-modified": "if-modified-since"}
 _CACHE_HEADERS = ("etag", "last-modified")
 
 
@@ -323,15 +323,15 @@
                 return super().__str__()
 
         logging_undefined = make_logging_undefined(
             logger=logger,
             base=CollectingUndefined
         )
 
-        @contextfunction
+        @pass_context
         def variable_finalizer(ctx, value):
             normalized_value = str(value)
             if self.VARIABLE_START_STRING in normalized_value and self.VARIABLE_END_STRING in normalized_value:
                 value_template_content = sys.intern(normalized_value)
                 env: Environment = ctx.environment
                 value_template = self.templates.get(value_template_content)
                 if not value_template:
```

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/app.py` & `kubernator-1.0.0.dev20230807191813/kubernator/app.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/helm.py` & `kubernator-1.0.0.dev20230807191813/kubernator/helm.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/istio.py` & `kubernator-1.0.0.dev20230807191813/kubernator/istio.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/k8s.py` & `kubernator-1.0.0.dev20230807191813/kubernator/k8s.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/k8s_api.py` & `kubernator-1.0.0.dev20230807191813/kubernator/k8s_api.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/kops.py` & `kubernator-1.0.0.dev20230807191813/kubernator/kops.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/proc.py` & `kubernator-1.0.0.dev20230807191813/kubernator/proc.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/template.py` & `kubernator-1.0.0.dev20230807191813/kubernator/template.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator/tf.py` & `kubernator-1.0.0.dev20230807191813/kubernator/tf.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator.egg-info/PKG-INFO` & `kubernator-1.0.0.dev20230807191813/kubernator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kubernator
-Version: 1.0.0.dev20211022025240
+Version: 1.0.0.dev20230807191813
 Summary: Kubernator is the a pluggable framework for K8S provisioning
 Home-page: https://github.com/karellen/kubernator
 Author: Express Systems USA, Inc.
 Author-email: 
 Maintainer: Karellen, Inc., Arcadiy Ivanov
 Maintainer-email: supervisor@karellen.co,arcadiy@karellen.co
 License: Apache License, Version 2.0
 Project-URL: Bug Tracker, https://github.com/karellen/kubernator/issues
 Project-URL: Documentation, https://github.com/karellen/kubernator/
 Project-URL: Source Code, https://github.com/karellen/kubernator/
 Keywords: kubernetes k8s kube top provisioning kOps terraform tf AWS
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Distributed Computing
@@ -211,9 +211,7 @@
         logger.warning("Resource %s in %s contains `replica` specification that will be removed. Use HPA!!!",
                        r, r.source)
         del r.manifest["spec"]["replicas"]
 
 
 ktor.k8s.add_transformer(remove_replicas)
 ```
-
-
```

### Comparing `kubernator-1.0.0.dev20211022025240/kubernator.egg-info/SOURCES.txt` & `kubernator-1.0.0.dev20230807191813/kubernator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.0.dev20211022025240/setup.py` & `kubernator-1.0.0.dev20230807191813/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,23 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'kubernator',
-        version = '1.0.0.dev20211022025240',
+        version = '1.0.0.dev20230807191813',
         description = 'Kubernator is the a pluggable framework for K8S provisioning',
         long_description = '# Kubernator\n\nKubernator™ (Ktor™) is an integrated solution for the Kubernetes state management. It operates on directories,\nprocessing their content via a collection of plugins, generating Kubernetes resources in the process, validating them,\ntransforming them and then applying against the Kubernetes cluster.\n\n[![Gitter](https://img.shields.io/gitter/room/karellen/lobby?logo=gitter)](https://gitter.im/karellen/Lobby)\n[![Build Status](https://img.shields.io/github/workflow/status/karellen/kubernator/kubernator/master)](https://github.com/karellen/kubernator/actions/workflows/kubernator.yml)\n[![Coverage Status](https://img.shields.io/coveralls/github/karellen/kubernator/master?logo=coveralls)](https://coveralls.io/r/karellen/kubernator?branch=master)\n\n[![Kubernator Version](https://img.shields.io/pypi/v/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Python Versions](https://img.shields.io/pypi/pyversions/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Day](https://img.shields.io/pypi/dd/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Week](https://img.shields.io/pypi/dw/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Month](https://img.shields.io/pypi/dm/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n\n## Notices\n\n### Beta Software\n\nWhile fully functional in the current state and used in production, this software is in **EARLY BETA**. A lot of things\nare expected to change rapidly, including main APIs, initialization procedures and some core features. Documentation at\nthis stage is basically non-existent.\n\n### License\n\nThe product is licensed under the Apache License, Version 2.0. Please see LICENSE for further details.\n\n### Warranties and Liability\n\nKubernator and its plugins are provided on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either\nexpress or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT,\nMERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of\nusing or redistributing Kubernator and assume any risks associated with doing so.\n\n### Trademarks\n\n"Kubernator" and "Ktor" are trademarks or registered trademarks of Express Systems USA, Inc and Karellen, Inc. All other\ntrademarks are property of their respective owners.\n\n## Problem Statement\n\n## Solution\n\n## Mode of Operation\n\nKubernator is a command line utility. Upon startup and processing of the command line arguments and initializing\nlogging, Kubernator initializes plugins. Current plugins include:\n\n0. Kubernator App\n1. Terraform\n2. kOps\n3. Kubernetes\n4. Helm\n5. Template\n\nThe order of initialization matters as it\'s the order the plugin handlers are executed!\n\nThe entire application operates in the following stages by invoking each plugin\'s stage handler in sequence:\n\n1. Plugin Init Stage\n2. Pre-start script (if specified)\n3. Plugin Start Stage\n4. For each directory in the pipeline:\n    1. Plugin Before Directory Stage\n    2. If `.kubernator.py` is present in the directory:\n        1. Plugin Before Script Stage\n        2. `.kubernator.py` script\n        3. Plugin After Script Stage\n    3. Plugin After Directory Stage\n5. Plugin End Stage\n\nEach plugin individually plays a specific role and performs a specific function which will be described in a later\nsection.\n\n## State/Context\n\nThere is a global state that is carried through as the application is running. It is a hierarchy of objects (`context`)\nthat follows the parent-child relationship as the application traverses the directory structure. For example, given the\ndirectory structure `/a/b`, `/a/c`, and `/a/c/d` any value of the context set or modified in context scoped to\ndirectory `/a` is visible in directories `/a/b`, `/a/c` and `/a/c/d`, while the same modified or set in `/a/b` is only\nvisible there, while one in `/a/c` is visible in `/a/c` and in `/a/c/d` but not `/a` or `/a/b`.\n\nAdditionally, there is a `context.globals` which is the top-most context that is available in all stages that are not\nassociated with the directory structure.\n\nNote, that in cases where the directory structure traversal moves to remote directories (that are actualized by local\ntemporary directories), such remote directory structure enters the context hierarchy as a child of the directory in\nwhich remote was registered.\n\nAlso note, that context carries not just data by references to essential functions.\n\nIn pre-start and `.kubernator.py` scripts the context is fully available as a global variable `ktor`.\n\n### Plugins\n\n#### Kubernator App Plugin\n\nThe role of the Kubernator App Plugin is to traverse the directory structure, expose essential functions through context\nand to run Kubernator scripts.\n\nIn the *After Directory Stage* Kubernator app scans the directories immediately available in the current, sorts them in\nthe alphabetic order, excludes those matching any of the patterns in `context.app.excludes` and then queues up the\nremaining directories in the order the match the patterns in `context.app.includes`.\n\nThus, for a directory content `/a/foo`, `/a/bal`, `/a/bar`, `/a/baz`, excludes `f*`, and includes `baz` and `*`, the\nresulting queue of directories to traverse will be `/a/baz`, `/a/bal`, `/a/bar`.\n\nNotice, that user can further interfere with processing order of the directory queue by asking Kubernator to walk\narbitrary paths, both local and remote.\n\n##### Context\n\n* `ktor.app.args`\n  > Namespace containing command line argument values\n* `ktor.app.walk_local(*paths: Union[Path, str, bytes])`\n  > Immediately schedules the paths to be traversed after the current directory by adding them to the queue\n  > Relative path is relative to the current directory\n* `ktor.app.walk_remote(repo, *path_prefixes: Union[Path, str, bytes])`\n  > Immediately schedules the path prefixes under the remote repo URL to be traversed after the current directory by\n  > adding them to the queue. Only Git URLs are currently supported.\n  > All absolute path prefixes are relativized based on the repository.\n* `ktor.app.repository_credentials_provider(func: Callable)`\n  > Sets a repository credentials provider function `func` that sets/overwrites credentials for URLs being specified by\n  > `walk_remote`. The callable `func` accepts a single argument containing a parsed URL in a form of tuple. The `func`\n  > is expected to return a tuple of three elements representing URL schema, username and password. If the value should\n  > not be changed it should be None. To convert from `git://repo.com/hello` to HTTPS authentication one should write\n  > a function returning `("https", "username", "password")`. The best utility is achieved by logic that allows running\n  > the plan both in CI and local environments using different authentication mechanics in different environments.\n\n#### Terraform\n\nThis is exclusively designed to pull the configuration options out of Terraform and to allow scripts and plugins to\nutilize that data.\n\n##### Context\n\n* `ktor.tf`\n  > A dictionary containing the values from Terraform output\n\n#### Kops\n\n##### Context\n\n#### Kubernetes\n\n##### Context\n\n#### Helm\n\n##### Context\n\n#### Templates\n\n##### Context\n\n## Examples\n\n### Adding Remote Directory\n\n```python\nktor.app.repository_credentials_provider(lambda r: ("ssh", "git", None))\nktor.app.walk_remote("git://repo.example.com/org/project?ref=dev", "/project")\n```\n\n### Adding Local Directory\n\n```python\nktor.app.walk_local("/home/username/local-dir")\n```\n\n### Using Transformers\n\n```python\ndef remove_replicas(resources, r: "K8SResource"):\n    if (r.group == "apps" and r.kind in ("StatefulSet", "Deployment")\n            and "replicas" in r.manifest["spec"]):\n        logger.warning("Resource %s in %s contains `replica` specification that will be removed. Use HPA!!!",\n                       r, r.source)\n        del r.manifest["spec"]["replicas"]\n\n\nktor.k8s.add_transformer(remove_replicas)\n```\n',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
             'Operating System :: MacOS :: MacOS X',
             'Operating System :: POSIX',
             'Operating System :: POSIX :: Linux',
             'Environment :: Console',
             'Topic :: Utilities',
             'Topic :: System :: Monitoring',
             'Topic :: System :: Distributed Computing',
@@ -69,15 +70,15 @@
         package_data = {
             'kubernator': ['LICENSE']
         },
         install_requires = [
             'appdirs~=1.4',
             'coloredlogs~=15.0',
             'gevent>=21.1.2',
-            'jinja2~=2.11',
+            'jinja2~=3.1',
             'json-log-formatter~=0.3',
             'jsonpatch~=1.32',
             'jsonpath-ng~=1.5',
             'jsonschema<4.0',
             'kubernetes~=17.0',
             'openapi-schema-validator~=0.1',
             'openapi-spec-validator~=0.3',
```

