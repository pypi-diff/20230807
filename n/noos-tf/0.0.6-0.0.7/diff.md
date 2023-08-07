# Comparing `tmp/noos-tf-0.0.6.tar.gz` & `tmp/noos_tf-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noos-tf-0.0.6.tar", last modified: Tue Jan  5 19:13:25 2021, max compression
+gzip compressed data, was "noos_tf-0.0.7.tar", max compression
```

## Comparing `noos-tf-0.0.6.tar` & `noos_tf-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1077 2021-01-05 19:12:16.143013 noos-tf-0.0.6/LICENSE
--rw-r--r--   0        0        0     2496 2021-01-05 19:12:16.143013 noos-tf-0.0.6/README.md
--rw-r--r--   0        0        0     1331 2021-01-05 19:12:16.143013 noos-tf-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      149 2021-01-05 19:12:16.143013 noos-tf-0.0.6/src/noos_tf/__init__.py
--rw-r--r--   0        0        0     1380 2021-01-05 19:12:16.143013 noos-tf-0.0.6/src/noos_tf/api.py
--rw-r--r--   0        0        0     1325 2021-01-05 19:12:16.143013 noos-tf-0.0.6/src/noos_tf/cli.py
--rw-r--r--   0        0        0     2783 2021-01-05 19:12:16.143013 noos-tf-0.0.6/src/noos_tf/client.py
--rw-r--r--   0        0        0     3419 2021-01-05 19:13:25.297153 noos-tf-0.0.6/setup.py
--rw-r--r--   0        0        0     3156 2021-01-05 19:13:25.297487 noos-tf-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-08-07 17:11:16.997265 noos_tf-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2496 2023-08-07 17:11:16.997265 noos_tf-0.0.7/README.md
+-rw-r--r--   0        0        0     1849 2023-08-07 17:11:16.997265 noos_tf-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-08-07 17:11:16.997265 noos_tf-0.0.7/src/noos_tf/__init__.py
+-rw-r--r--   0        0        0     1380 2023-08-07 17:11:16.997265 noos_tf-0.0.7/src/noos_tf/api.py
+-rw-r--r--   0        0        0     1343 2023-08-07 17:11:16.997265 noos_tf-0.0.7/src/noos_tf/cli.py
+-rw-r--r--   0        0        0     2783 2023-08-07 17:11:16.997265 noos_tf-0.0.7/src/noos_tf/client.py
+-rw-r--r--   0        0        0     3158 1970-01-01 00:00:00.000000 noos_tf-0.0.7/PKG-INFO
```

### Comparing `noos-tf-0.0.6/LICENSE` & `noos_tf-0.0.7/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Noos Energy Limited.
+Copyright (c) 2022 Noos Energy Limited.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `noos-tf-0.0.6/README.md` & `noos_tf-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `noos-tf-0.0.6/src/noos_tf/api.py` & `noos_tf-0.0.7/src/noos_tf/api.py`

 * *Files identical despite different names*

### Comparing `noos-tf-0.0.6/src/noos_tf/cli.py` & `noos_tf-0.0.7/src/noos_tf/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Using `invoke` as library
 # http://docs.pyinvoke.org/en/stable/concepts/library.html
 import os
 
-from invoke import Collection, Program, task
+from invoke import Collection, Program, Task, task
 
 from . import __version__, api
 
 
 @task
 def update(ctx, variable="", value="", workspace="", organisation=None, token=None):
     """Update variable in Terraform cloud."""
@@ -26,12 +26,12 @@
     assert organisation is not None, "Missing Terraform Cloud organisation."
     assert token is not None, "Missing Terraform Cloud token."
     url = api.run_workspace_plan(organisation, workspace, token, message)
     print(f"Running Terraform plan for {workspace}: {url}")
 
 
 ns = Collection()
-ns.add_task(update)
-ns.add_task(run)
+ns.add_task(Task(update))
+ns.add_task(Task(run))
 
 
 main = Program(namespace=ns, version=__version__)
```

### Comparing `noos-tf-0.0.6/src/noos_tf/client.py` & `noos_tf-0.0.7/src/noos_tf/client.py`

 * *Files identical despite different names*

### Comparing `noos-tf-0.0.6/PKG-INFO` & `noos_tf-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: noos-tf
-Version: 0.0.6
+Version: 0.0.7
 Summary: HashiCorp Terraform Cloud API client
 Home-page: https://github.com/noosenergy/noos-terraform
 License: MIT
 Author: Noos Energy
 Author-email: contact@noos.energy
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: invoke
 Requires-Dist: noos-pyk
 Description-Content-Type: text/markdown
 
 [![CircleCI](https://circleci.com/gh/noosenergy/noos-terraform.svg?style=svg&circle-token=5d70bf41e76bbad2a187da8db5c0c39f691db452)](https://circleci.com/gh/noosenergy/noos-terraform)
```

