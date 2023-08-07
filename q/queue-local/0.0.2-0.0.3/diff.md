# Comparing `tmp/queue-local-0.0.2.tar.gz` & `tmp/queue-local-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue-local-0.0.2.tar", last modified: Sun Aug  6 15:19:59 2023, max compression
+gzip compressed data, was "queue-local-0.0.3.tar", last modified: Mon Aug  7 16:16:21 2023, max compression
```

## Comparing `queue-local-0.0.2.tar` & `queue-local-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:19:59.726187 queue-local-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-06 15:19:59.726187 queue-local-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-06 15:19:28.000000 queue-local-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-06 15:19:28.000000 queue-local-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:19:59.726187 queue-local-0.0.2/queue_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-06 15:19:59.000000 queue-local-0.0.2/queue_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-06 15:19:59.000000 queue-local-0.0.2/queue_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 15:19:59.000000 queue-local-0.0.2/queue_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 15:19:59.000000 queue-local-0.0.2/queue_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 15:19:59.726187 queue-local-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-06 15:19:28.000000 queue-local-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:16:21.939103 queue-local-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-07 16:16:21.939103 queue-local-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-07 16:15:54.000000 queue-local-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-07 16:15:54.000000 queue-local-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:16:21.939103 queue-local-0.0.3/queue_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-07 16:16:21.000000 queue-local-0.0.3/queue_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-07 16:16:21.000000 queue-local-0.0.3/queue_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:16:21.000000 queue-local-0.0.3/queue_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:16:21.000000 queue-local-0.0.3/queue_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 16:16:21.939103 queue-local-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-07 16:15:54.000000 queue-local-0.0.3/setup.py
```

### Comparing `queue-local-0.0.2/README.md` & `queue-local-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `queue-local-0.0.2/setup.py` & `queue-local-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 setuptools.setup(
      name='queue-local',
-     version='0.0.2',  # https://pypi.org/project/queue-local-python-package/
+     version='0.0.3',  # https://pypi.org/project/queue-local-python-package/
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles queue Local Python",
      long_description="This is a package for sharing common Queue function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/circles",
      packages=setuptools.find_packages(),
```

