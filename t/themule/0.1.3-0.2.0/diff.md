# Comparing `tmp/themule-0.1.3.tar.gz` & `tmp/themule-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themule-0.1.3.tar", last modified: Tue Jun 13 21:25:14 2023, max compression
+gzip compressed data, was "themule-0.2.0.tar", last modified: Mon Aug  7 06:21:04 2023, max compression
```

## Comparing `themule-0.1.3.tar` & `themule-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:25:14.644984 themule-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 21:25:04.000000 themule-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 21:25:14.640984 themule-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 21:25:04.000000 themule-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 21:25:04.000000 themule-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:25:14.640984 themule-0.1.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 21:25:04.000000 themule-0.1.3/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 21:25:04.000000 themule-0.1.3/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:25:04.000000 themule-0.1.3/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:25:14.644984 themule-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-13 21:25:04.000000 themule-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:25:14.640984 themule-0.1.3/themule/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 21:25:07.000000 themule-0.1.3/themule/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 21:25:04.000000 themule-0.1.3/themule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 21:25:04.000000 themule-0.1.3/themule/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-13 21:25:04.000000 themule-0.1.3/themule/boto_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 21:25:04.000000 themule-0.1.3/themule/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 21:25:04.000000 themule-0.1.3/themule/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-13 21:25:04.000000 themule-0.1.3/themule/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-13 21:25:04.000000 themule-0.1.3/themule/import_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-13 21:25:04.000000 themule-0.1.3/themule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 21:25:04.000000 themule-0.1.3/themule/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:25:14.640984 themule-0.1.3/themule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 21:25:14.000000 themule-0.1.3/themule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:21:04.597481 themule-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-07 06:20:52.000000 themule-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-07 06:21:04.597481 themule-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-08-07 06:20:52.000000 themule-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-07 06:20:52.000000 themule-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:21:04.597481 themule-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 06:20:52.000000 themule-0.2.0/requirements/base.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:21:04.597481 themule-0.2.0/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 06:20:52.000000 themule-0.2.0/requirements/extras/aws_batch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 06:20:52.000000 themule-0.2.0/requirements/extras/docker.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 06:20:52.000000 themule-0.2.0/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:20:52.000000 themule-0.2.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 06:21:04.597481 themule-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-08-07 06:20:52.000000 themule-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:21:04.597481 themule-0.2.0/themule/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 06:20:56.000000 themule-0.2.0/themule/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-07 06:20:52.000000 themule-0.2.0/themule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-07 06:20:52.000000 themule-0.2.0/themule/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-08-07 06:20:52.000000 themule-0.2.0/themule/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-07 06:20:52.000000 themule-0.2.0/themule/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-07 06:20:52.000000 themule-0.2.0/themule/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-07 06:20:52.000000 themule-0.2.0/themule/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-07 06:20:52.000000 themule-0.2.0/themule/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-07 06:20:52.000000 themule-0.2.0/themule/import_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-07 06:20:52.000000 themule-0.2.0/themule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-07 06:20:52.000000 themule-0.2.0/themule/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:21:04.597481 themule-0.2.0/themule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-07 06:21:04.000000 themule-0.2.0/themule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-07 06:21:04.000000 themule-0.2.0/themule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:21:04.000000 themule-0.2.0/themule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 06:21:04.000000 themule-0.2.0/themule.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:21:04.000000 themule-0.2.0/themule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-07 06:21:04.000000 themule-0.2.0/themule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 06:21:04.000000 themule-0.2.0/themule.egg-info/top_level.txt
```

### Comparing `themule-0.1.3/setup.py` & `themule-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,27 +47,43 @@
         about["__version__"] = f.read().strip()
 
     return about
 
 about = get_about()
 
 
+BUNDLES = (
+    "aws_batch",
+    "docker",
+)
+
+
+def extras(*p):
+    """Parse requirement in the requirements/extras/ directory."""
+    return reqs("extras", *p)
+
+def extras_require():
+    """Get map of all extra requirements."""
+    return {x: extras(x + ".txt") for x in BUNDLES}
+
+
 setup(
     name="themule",
     version=about["__version__"],
     description="The Mule - run arbitrary python function on AWS Batch",
     url="http://github.com/wlatanowicz/themule",
     author=about["__author__"],
     author_email="wiktor@latanowicz.com",
     license="MIT",
     long_description=long_description(),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=["tests*",]),
     zip_safe=False,
     install_requires=reqs("base.txt"),
+    extras_require=extras_require(),
     tests_require=reqs("tests.txt"),
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
```

### Comparing `themule-0.1.3/themule/cli.py` & `themule-0.2.0/themule/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from typing import Type
 
 import click
 
+from .conf import settings
 from .executor import execute_job
 from .import_helpers import import_by_path
 from .serializers import DEFAULT_SERIALIZER, BaseSerializer
 
 
 @click.group()
 def cli():
@@ -19,21 +20,20 @@
     "--serializer",
     "serializer_path",
     type=str,
     help="Path to serializer's class",
 )
 @click.argument("job-spec", type=str)
 def execute_job_cli(serializer_path, job_spec):
-    setup = os.environ.get("THEMULE_SETUP_CALLBACK")
-    if setup:
-        setup_func = import_by_path(setup)
-        setup_func()
+    bootstrap = settings.BOOTSTRAP_CALLBACK
+    if bootstrap:
+        bootstrap_func = import_by_path(bootstrap)
+        bootstrap_func()
 
     if not serializer_path:
-        serializer_path = os.environ.get(
-            "THEMULE_JOB_SERIALIZER", default=DEFAULT_SERIALIZER
-        )
+        serializer_path = settings.JOB_SERIALIZER
+
     serializer_class: Type[BaseSerializer] = import_by_path(serializer_path)
     serializer = serializer_class()
     job = serializer.unserialize(job_spec)
 
     execute_job(job)
```

