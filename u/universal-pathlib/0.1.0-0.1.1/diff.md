# Comparing `tmp/universal_pathlib-0.1.0.tar.gz` & `tmp/universal_pathlib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal_pathlib-0.1.0.tar", last modified: Thu Aug  3 08:08:15 2023, max compression
+gzip compressed data, was "universal_pathlib-0.1.1.tar", last modified: Mon Aug  7 21:04:14 2023, max compression
```

## Comparing `universal_pathlib-0.1.0.tar` & `universal_pathlib-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.088260 universal_pathlib-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-03 08:08:15.088260 universal_pathlib-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.080260 universal_pathlib-0.1.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/notebooks/examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-03 08:08:15.088260 universal_pathlib-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.080260 universal_pathlib-0.1.0/universal_pathlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:08:14.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/universal_pathlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.080260 universal_pathlib-0.1.0/upath/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 08:08:15.000000 universal_pathlib-0.1.0/upath/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23978 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.084260 universal_pathlib-0.1.0/upath/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/hdfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/implementations/webdav.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.084260 universal_pathlib-0.1.0/upath/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.084260 universal_pathlib-0.1.0/upath/tests/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_hdfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/implementations/test_webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.088260 universal_pathlib-0.1.0/upath/tests/pathlib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/_test_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   104167 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_310.py
--rw-r--r--   0 runner    (1001) docker     (123)   109314 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_311.py
--rw-r--r--   0 runner    (1001) docker     (123)   138582 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_312.py
--rw-r--r--   0 runner    (1001) docker     (123)    91139 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_38.py
--rw-r--r--   0 runner    (1001) docker     (123)    98727 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_39.py
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:08:15.088260 universal_pathlib-0.1.0/upath/tests/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/third_party/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 08:07:47.000000 universal_pathlib-0.1.0/upath/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:04:14.334421 universal_pathlib-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-07 21:04:14.334421 universal_pathlib-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:04:14.330421 universal_pathlib-0.1.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/notebooks/examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-07 21:04:14.338421 universal_pathlib-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:04:14.330421 universal_pathlib-0.1.1/universal_pathlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-07 21:04:14.000000 universal_pathlib-0.1.1/universal_pathlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-07 21:04:14.000000 universal_pathlib-0.1.1/universal_pathlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:04:14.000000 universal_pathlib-0.1.1/universal_pathlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:04:14.000000 universal_pathlib-0.1.1/universal_pathlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-07 21:04:14.000000 universal_pathlib-0.1.1/universal_pathlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 21:04:14.000000 universal_pathlib-0.1.1/universal_pathlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:04:14.330421 universal_pathlib-0.1.1/upath/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 21:04:14.000000 universal_pathlib-0.1.1/upath/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24016 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:04:14.330421 universal_pathlib-0.1.1/upath/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/implementations/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/implementations/hdfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/implementations/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/implementations/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/implementations/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/implementations/webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:04:14.334421 universal_pathlib-0.1.1/upath/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:04:14.334421 universal_pathlib-0.1.1/upath/tests/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/implementations/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/implementations/test_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/implementations/test_hdfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/implementations/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/implementations/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/implementations/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/implementations/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/implementations/test_webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:04:14.334421 universal_pathlib-0.1.1/upath/tests/pathlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/pathlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/pathlib/_test_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/pathlib/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104167 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/pathlib/test_pathlib_310.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109314 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/pathlib/test_pathlib_311.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138582 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/pathlib/test_pathlib_312.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91139 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/pathlib/test_pathlib_38.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98727 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/pathlib/test_pathlib_39.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:04:14.334421 universal_pathlib-0.1.1/upath/tests/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/third_party/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-07 21:03:52.000000 universal_pathlib-0.1.1/upath/tests/utils.py
```

### Comparing `universal_pathlib-0.1.0/.flake8` & `universal_pathlib-0.1.1/.flake8`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/.pre-commit-config.yaml` & `universal_pathlib-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/CHANGELOG.md` & `universal_pathlib-0.1.1/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.1]
+### Fixed
+- restore `._kwargs` and `._url` on `PosixUPath` and `WindowsUPath` subclasses (#131).
+- tests: fixed and refactored core tests (#130).
+
 ## [0.1.0]
 ### Changed
 - updated past changelog entries.
 - changed `UPath.__new__` behavior to return `UPath` subclasses for local paths (#125).
 
 ### Fixed
 - improved azure test separation (#123).
@@ -62,15 +67,16 @@
 ### Changed
 - Use `NotADirectoryError` instead of custom error (#74).
 
 ## [0.0.19] - 2022-06-22
 ### Added
 - started a changelog to keep track of significant changes
 
-[Unreleased]: https://github.com/fsspec/universal_pathlib/compare/v0.1.0...HEAD
+[Unreleased]: https://github.com/fsspec/universal_pathlib/compare/v0.1.1...HEAD
+[0.1.1]: https://github.com/fsspec/universal_pathlib/compare/v0.1.0...v0.1.1
 [0.1.0]: https://github.com/fsspec/universal_pathlib/compare/v0.0.24...v0.1.0
 [0.0.24]: https://github.com/fsspec/universal_pathlib/compare/v0.0.23...v0.0.24
 [0.0.23]: https://github.com/fsspec/universal_pathlib/compare/v0.0.22...v0.0.23
 [0.0.22]: https://github.com/fsspec/universal_pathlib/compare/v0.0.21...v0.0.22
 [0.0.21]: https://github.com/fsspec/universal_pathlib/compare/v0.0.20...v0.0.21
 [0.0.20]: https://github.com/fsspec/universal_pathlib/compare/v0.0.19...v0.0.20
 [0.0.19]: https://github.com/fsspec/universal_pathlib/tree/v0.0.19
```

### Comparing `universal_pathlib-0.1.0/CODE_OF_CONDUCT.rst` & `universal_pathlib-0.1.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/CONTRIBUTING.rst` & `universal_pathlib-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/LICENSE` & `universal_pathlib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/PKG-INFO` & `universal_pathlib-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: universal_pathlib
-Version: 0.1.0
+Version: 0.1.1
 Summary: pathlib api extended to use fsspec backends
 Home-page: https://github.com/fsspec/universal_pathlib
 Maintainer-email: andrewfulton9@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `universal_pathlib-0.1.0/README.md` & `universal_pathlib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/notebooks/examples.ipynb` & `universal_pathlib-0.1.1/notebooks/examples.ipynb`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/noxfile.py` & `universal_pathlib-0.1.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/pyproject.toml` & `universal_pathlib-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/setup.cfg` & `universal_pathlib-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/universal_pathlib.egg-info/PKG-INFO` & `universal_pathlib-0.1.1/universal_pathlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: universal-pathlib
-Version: 0.1.0
+Version: 0.1.1
 Summary: pathlib api extended to use fsspec backends
 Home-page: https://github.com/fsspec/universal_pathlib
 Maintainer-email: andrewfulton9@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `universal_pathlib-0.1.0/universal_pathlib.egg-info/SOURCES.txt` & `universal_pathlib-0.1.1/universal_pathlib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 upath/tests/test_core.py
 upath/tests/utils.py
 upath/tests/implementations/__init__.py
 upath/tests/implementations/test_azure.py
 upath/tests/implementations/test_gcs.py
 upath/tests/implementations/test_hdfs.py
 upath/tests/implementations/test_http.py
+upath/tests/implementations/test_local.py
 upath/tests/implementations/test_memory.py
 upath/tests/implementations/test_s3.py
 upath/tests/implementations/test_webdav.py
 upath/tests/pathlib/__init__.py
 upath/tests/pathlib/_test_support.py
 upath/tests/pathlib/conftest.py
 upath/tests/pathlib/test_pathlib_310.py
```

### Comparing `universal_pathlib-0.1.0/upath/core.py` & `universal_pathlib-0.1.1/upath/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 
 
 class _FSSpecAccessor:
     __slots__ = ("_fs",)
 
     def __init__(self, parsed_url: SplitResult | None, **kwargs: Any) -> None:
-        if parsed_url:
+        if parsed_url and parsed_url.scheme:
             cls = get_filesystem_class(parsed_url.scheme)
             url_kwargs = cls._get_kwargs_from_urls(urlunsplit(parsed_url))
         else:
             cls = get_filesystem_class(None)
             url_kwargs = {}
         url_kwargs.update(kwargs)
         self._fs = cls(**url_kwargs)
@@ -162,15 +162,15 @@
             drv, root, parts = _cls._flavour.join_parsed_parts(
                 other._drv, other._root, other._parts, drv, root, parts  # type: ignore # noqa: E501
             )
 
             _kwargs = getattr(other, "_kwargs", {})
             _url = getattr(other, "_url", None)
             other_kwargs = _kwargs.copy()
-            if _url:
+            if _url and _url.scheme:
                 other_kwargs["url"] = _url
             new_kwargs = _kwargs.copy()
             new_kwargs.update(kwargs)
 
             return _cls(
                 _cls._format_parsed_parts(drv, root, parts, **other_kwargs),
                 **new_kwargs,
```

### Comparing `universal_pathlib-0.1.0/upath/implementations/cloud.py` & `universal_pathlib-0.1.1/upath/implementations/cloud.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/implementations/hdfs.py` & `universal_pathlib-0.1.1/upath/implementations/hdfs.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/implementations/http.py` & `universal_pathlib-0.1.1/upath/implementations/http.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/implementations/local.py` & `universal_pathlib-0.1.1/upath/implementations/local.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import os
 from pathlib import Path
 from pathlib import PosixPath
 from pathlib import WindowsPath
 from typing import Any
 from typing import Iterable
+from urllib.parse import SplitResult
 
 from fsspec.implementations.local import LocalFileSystem
 
 from upath.core import UPath
 
 __all__ = [
     "LocalPath",
@@ -45,27 +46,26 @@
     # assign all PosixPath methods/attrs to prevent multi inheritance issues
     for attr, func_or_attr in _iterate_class_attrs(PosixPath):
         locals()[attr] = func_or_attr
     del attr, func_or_attr
 
     @property
     def fs(self):
-        try:
-            return self._cached_fs
-        except AttributeError:
-            self._cached_fs = fs = LocalFileSystem()
-            return fs
+        return LocalFileSystem()
 
     @property
     def path(self) -> str:
         return str(self)
 
     @classmethod
     def _from_parts(cls, args, *, url=None, **kw):
-        return super(UPath, cls)._from_parts(args)
+        obj = super(UPath, cls)._from_parts(args)
+        obj._kwargs = {}
+        obj._url = SplitResult("", "", str(obj), "", "")
+        return obj
 
 
 class WindowsUPath(WindowsPath, UPath):
     __slots__ = ()
 
     if os.name != "nt":
         __new__ = WindowsPath.__new__
@@ -73,20 +73,19 @@
     # assign all WindowsPath methods/attrs to prevent multi inheritance issues
     for attr, func_or_attr in _iterate_class_attrs(WindowsPath):
         locals()[attr] = func_or_attr
     del attr, func_or_attr
 
     @property
     def fs(self):
-        try:
-            return self._cached_fs
-        except AttributeError:
-            self._cached_fs = fs = LocalFileSystem()
-            return fs
+        return LocalFileSystem()
 
     @property
     def path(self) -> str:
         return str(self)
 
     @classmethod
     def _from_parts(cls, args, *, url=None, **kw):
-        return super(UPath, cls)._from_parts(args)
+        obj = super(UPath, cls)._from_parts(args)
+        obj._kwargs = {}
+        obj._url = SplitResult("", "", str(obj), "", "")
+        return obj
```

### Comparing `universal_pathlib-0.1.0/upath/implementations/memory.py` & `universal_pathlib-0.1.1/upath/implementations/memory.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/implementations/webdav.py` & `universal_pathlib-0.1.1/upath/implementations/webdav.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/registry.py` & `universal_pathlib-0.1.1/upath/registry.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/cases.py` & `universal_pathlib-0.1.1/upath/tests/cases.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/conftest.py` & `universal_pathlib-0.1.1/upath/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/implementations/test_azure.py` & `universal_pathlib-0.1.1/upath/tests/implementations/test_azure.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/implementations/test_gcs.py` & `universal_pathlib-0.1.1/upath/tests/implementations/test_gcs.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/implementations/test_hdfs.py` & `universal_pathlib-0.1.1/upath/tests/implementations/test_hdfs.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/implementations/test_http.py` & `universal_pathlib-0.1.1/upath/tests/implementations/test_http.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/implementations/test_memory.py` & `universal_pathlib-0.1.1/upath/tests/implementations/test_memory.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/implementations/test_s3.py` & `universal_pathlib-0.1.1/upath/tests/implementations/test_s3.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/pathlib/_test_support.py` & `universal_pathlib-0.1.1/upath/tests/pathlib/_test_support.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/pathlib/conftest.py` & `universal_pathlib-0.1.1/upath/tests/pathlib/conftest.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_310.py` & `universal_pathlib-0.1.1/upath/tests/pathlib/test_pathlib_310.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_311.py` & `universal_pathlib-0.1.1/upath/tests/pathlib/test_pathlib_311.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_312.py` & `universal_pathlib-0.1.1/upath/tests/pathlib/test_pathlib_312.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_38.py` & `universal_pathlib-0.1.1/upath/tests/pathlib/test_pathlib_38.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/pathlib/test_pathlib_39.py` & `universal_pathlib-0.1.1/upath/tests/pathlib/test_pathlib_39.py`

 * *Files identical despite different names*

### Comparing `universal_pathlib-0.1.0/upath/tests/test_core.py` & `universal_pathlib-0.1.1/upath/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import pathlib
 import pickle
 import sys
 import warnings
+from urllib.parse import SplitResult
 
 import pytest
 
 from upath import UPath
 from upath.implementations.cloud import GCSPath
 from upath.implementations.cloud import S3Path
 
@@ -63,23 +64,20 @@
     def test_home(self):
         pth = type(self.path).home()
         assert str(pth) == os.path.expanduser("~")
         assert isinstance(pth, pathlib.Path)
         assert isinstance(pth, UPath)
 
 
-@pytest.mark.hdfs
-def test_multiple_backend_paths(local_testdir, s3_fixture, hdfs):
-    _, anon, s3so = s3_fixture
+def test_multiple_backend_paths(local_testdir):
     path = f"s3:{local_testdir}"
-    s3_path = UPath(path, anon=anon, **s3so)
+    s3_path = UPath(path, anon=True)
     assert s3_path.joinpath("text.txt")._url.scheme == "s3"
-    host, user, port = hdfs
-    path = f"hdfs:{local_testdir}"
-    UPath(path, host=host, user=user, port=port)
+    path = f"file://{local_testdir}"
+    UPath(path)
     assert s3_path.joinpath("text1.txt")._url.scheme == "s3"
 
 
 def test_constructor_accept_path(local_testdir):
     path = UPath(pathlib.Path(local_testdir))
     assert str(path) == str(pathlib.Path(local_testdir))
 
@@ -121,49 +119,41 @@
 def test_new_method(local_testdir):
     path = UPath.__new__(pathlib.Path, local_testdir)
     assert str(path) == str(pathlib.Path(local_testdir))
     assert isinstance(path, pathlib.Path)
     assert isinstance(path, UPath)
 
 
-@skip_on_windows
-class TestFSSpecLocal(BaseTests):
-    @pytest.fixture(autouse=True)
-    def path(self, local_testdir):
-        path = f"file://{local_testdir}"
-        self.path = UPath(path)
-
-
 PATHS = (
     ("path", "storage_options", "module", "object_type"),
     (
-        ("/tmp/abc", (), None, pathlib.Path),
-        ("s3://bucket/folder", ({"anon": True}), "s3fs", S3Path),
-        ("gs://bucket/folder", ({"token": "anon"}), "gcsfs", GCSPath),
+        ("/tmp/abc", {}, None, pathlib.Path),
+        ("s3://bucket/folder", {"anon": True}, "s3fs", S3Path),
+        ("gs://bucket/folder", {"token": "anon"}, "gcsfs", GCSPath),
     ),
 )
 
 
 @pytest.mark.parametrize(*PATHS)
 def test_create_from_type(path, storage_options, module, object_type):
     """Test that derived paths use same fs instance."""
     if module:
         # skip if module cannot be imported
         pytest.importorskip(module)
     try:
-        upath = UPath(path, storage_options=storage_options)
+        upath = UPath(path, **storage_options)
         # test expected object type
         assert isinstance(upath, object_type)
         cast = type(upath)
         parent = upath.parent
         # test derived object is same type
         assert isinstance(parent, cast)
         # test that created fs uses fsspec instance cache
         assert not hasattr(upath, "fs") or upath.fs is parent.fs
-        new = cast(str(parent))
+        new = cast(str(parent), **storage_options)
         # test that object cast is same type
         assert isinstance(new, cast)
     except ImportError:
         # fs failed to import
         pass
 
 
@@ -186,38 +176,38 @@
     assert path_a._root == path_b._root
     assert path_a._drv == path_b._drv
     assert path_a._parts == path_b._parts
     assert path_a._url == path_b._url
 
 
 def test_pickling():
-    path = UPath("gcs://bucket/folder", storage_options={"anon": True})
+    path = UPath("gcs://bucket/folder", token="anon")
     pickled_path = pickle.dumps(path)
     recovered_path = pickle.loads(pickled_path)
 
     assert type(path) == type(recovered_path)
     assert str(path) == str(recovered_path)
     assert path.fs.storage_options == recovered_path.fs.storage_options
 
 
 def test_pickling_child_path():
-    path = UPath("gcs://bucket", anon=True) / "subfolder" / "subsubfolder"
+    path = UPath("gcs://bucket", token="anon") / "subfolder" / "subsubfolder"
     pickled_path = pickle.dumps(path)
     recovered_path = pickle.loads(pickled_path)
 
     assert type(path) == type(recovered_path)
     assert str(path) == str(recovered_path)
     assert path._drv == recovered_path._drv
     assert path._root == recovered_path._root
     assert path._parts == recovered_path._parts
     assert path.fs.storage_options == recovered_path.fs.storage_options
 
 
 def test_copy_path():
-    path = UPath("gcs://bucket/folder", anon=True)
+    path = UPath("gcs://bucket/folder", token="anon")
     copy_path = UPath(path)
 
     assert type(path) == type(copy_path)
     assert str(path) == str(copy_path)
     assert path._drv == copy_path._drv
     assert path._root == copy_path._root
     assert path._parts == copy_path._parts
@@ -249,14 +239,32 @@
 
     path = UPath("/tmp/folder")
     copy_path = UPath(path, "folder2", "folder3")
 
     assert str(path / "folder2" / "folder3") == str(copy_path)
 
 
+@pytest.mark.parametrize(
+    "urlpath",
+    [
+        os.getcwd(),
+        pathlib.Path.cwd().as_uri(),
+        "mock:///abc",
+    ],
+)
+def test_access_to_private_kwargs_and_url(urlpath):
+    # fixme: this should be deprecated...
+    pth = UPath(urlpath)
+    assert isinstance(pth._kwargs, dict)
+    assert pth._kwargs == {}
+    assert isinstance(pth._url, SplitResult)
+    assert pth._url.scheme == "" or pth._url.scheme in pth.fs.protocol
+    assert pth._url.path == pth.path
+
+
 def test_copy_path_append_kwargs():
     path = UPath("gcs://bucket/folder", anon=True)
     copy_path = UPath(path, anon=False)
 
     assert type(path) == type(copy_path)
     assert str(path) == str(copy_path)
     assert not copy_path._kwargs["anon"]
```

