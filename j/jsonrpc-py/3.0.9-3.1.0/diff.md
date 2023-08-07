# Comparing `tmp/jsonrpc-py-3.0.9.tar.gz` & `tmp/jsonrpc-py-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-3.0.9.tar", last modified: Sun May 28 11:12:51 2023, max compression
+gzip compressed data, was "jsonrpc-py-3.1.0.tar", last modified: Mon Aug  7 19:04:30 2023, max compression
```

## Comparing `jsonrpc-py-3.0.9.tar` & `jsonrpc-py-3.1.0.tar`

### file list

```diff
@@ -1,90 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.009646 jsonrpc-py-3.0.9/
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/.flake8
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/Makefile
--rw-r--r--   0 root         (0) root         (0)     2921 2023-05-28 11:12:51.008646 jsonrpc-py-3.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:50.996646 jsonrpc-py-3.0.9/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:50.993646 jsonrpc-py-3.0.9/docs/changelog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:50.997646 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.1.0.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.002646 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.1.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.2.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.2.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.2.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.2.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.3.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.4.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.5.1.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.004646 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/deployment.rst
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/docs/reference.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.006646 jsonrpc-py-3.0.9/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9422 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5994 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/request.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/response.py
--rw-rw-rw-   0 root         (0) root         (0)     2032 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     3300 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/typedefs.py
--rw-rw-rw-   0 root         (0) root         (0)     4098 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/jsonrpc/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.007646 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2921 2023-05-28 11:12:50.000000 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2087 2023-05-28 11:12:50.000000 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 11:12:50.000000 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-28 11:12:50.000000 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-28 11:12:50.000000 jsonrpc-py-3.0.9/jsonrpc_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1885 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 11:12:51.009646 jsonrpc-py-3.0.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 11:12:51.008646 jsonrpc-py-3.0.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13819 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1917 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     5630 2023-05-28 11:12:33.000000 jsonrpc-py-3.0.9/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:04:30.069139 jsonrpc-py-3.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-08-07 19:04:30.069139 jsonrpc-py-3.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:04:30.054140 jsonrpc-py-3.1.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:04:30.051140 jsonrpc-py-3.1.0/docs/changelog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:04:30.056140 jsonrpc-py-3.1.0/docs/changelog/v1.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v1.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v1.x.x/v1.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v1.x.x/v1.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v1.x.x/v1.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v1.x.x/v1.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v1.x.x/v1.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v1.x.x/v1.1.0.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:04:30.060140 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.2.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.2.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.2.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.2.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.3.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.4.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.4.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.5.1.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:04:30.063140 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.10.rst
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.11.rst
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.12.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.13.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/deployment.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/docs/reference.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:04:30.066140 jsonrpc-py-3.1.0/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10073 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3597 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/jsonrpc/lifespan.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/jsonrpc/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/jsonrpc/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2032 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/jsonrpc/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3300 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5034 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:04:30.067139 jsonrpc-py-3.1.0/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-08-07 19:04:30.000000 jsonrpc-py-3.1.0/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-08-07 19:04:30.000000 jsonrpc-py-3.1.0/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 19:04:30.000000 jsonrpc-py-3.1.0/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-07 19:04:30.000000 jsonrpc-py-3.1.0/jsonrpc_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-07 19:04:30.000000 jsonrpc-py-3.1.0/jsonrpc_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 19:04:30.069139 jsonrpc-py-3.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 19:04:30.069139 jsonrpc-py-3.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13688 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3591 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/tests/test_lifespan.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/tests/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/tests/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/tests/test_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2023-08-07 19:04:12.000000 jsonrpc-py-3.1.0/tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.0.9/.gitlab-ci.yml` & `jsonrpc-py-3.1.0/.gitlab-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-image: python:3.11-bullseye
+image: python:3.11-bookworm
 
 variables:
   PIP_CACHE_DIR: "$CI_PROJECT_DIR/.pip_cache"
   PIP_PROGRESS_BAR: "off"
   PIP_TIMEOUT: "300"
   PYTHONDONTWRITEBYTECODE: "1"
```

### Comparing `jsonrpc-py-3.0.9/LICENSE` & `jsonrpc-py-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/Makefile` & `jsonrpc-py-3.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/PKG-INFO` & `jsonrpc-py-3.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.9
+Version: 3.1.0
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Homepage, https://docs.jsonrpc.ru
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
@@ -27,46 +27,46 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: ujson
 License-File: LICENSE
 
-JSON-RPC Python
-===============
+# JSON-RPC Python
+
 [![pipeline status][pipeline]][homepage]
 [![coverage report][coverage]][homepage]
 [![latest release][version]][pypi]
 [![pypi downloads][downloads]][pypi]
 
 **JSON-RPC Python** is a lightweight ASGI micro framework for building web applications.
 
-Features
---------
+## Features
+
 * Pure zero-dependency JSON-RPC 2.0 implementation.
 * Simple and user-friendly API interface.
 * 100% type annotated codebase.
 * 100% test coverage, so it's production-ready.
 
-Requirements
-------------
+## Requirements
+
 Python 3.11 and above.
 
-Installation
-------------
+## Installation
+
 ```
 $ pip install jsonrpc-py
 ```
 
-Distribution
-------------
+## Distribution
+
 This project is licensed under the terms of the [BSD 3-Clause License](LICENSE).
 
-Links
------
+## Links
+
 * Documentation: <https://docs.jsonrpc.ru>
 * PyPI Releases: <https://pypi.org/project/jsonrpc-py>
 * Source Code: <https://gitlab.com/jsonrpc/jsonrpc-py>
 
 [homepage]: <https://gitlab.com/jsonrpc/jsonrpc-py>
 [pipeline]: <https://img.shields.io/gitlab/pipeline-status/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
 [coverage]: <https://img.shields.io/gitlab/pipeline-coverage/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
```

### Comparing `jsonrpc-py-3.0.9/README.md` & `jsonrpc-py-3.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-JSON-RPC Python
-===============
+# JSON-RPC Python
+
 [![pipeline status][pipeline]][homepage]
 [![coverage report][coverage]][homepage]
 [![latest release][version]][pypi]
 [![pypi downloads][downloads]][pypi]
 
 **JSON-RPC Python** is a lightweight ASGI micro framework for building web applications.
 
-Features
---------
+## Features
+
 * Pure zero-dependency JSON-RPC 2.0 implementation.
 * Simple and user-friendly API interface.
 * 100% type annotated codebase.
 * 100% test coverage, so it's production-ready.
 
-Requirements
-------------
+## Requirements
+
 Python 3.11 and above.
 
-Installation
-------------
+## Installation
+
 ```
 $ pip install jsonrpc-py
 ```
 
-Distribution
-------------
+## Distribution
+
 This project is licensed under the terms of the [BSD 3-Clause License](LICENSE).
 
-Links
------
+## Links
+
 * Documentation: <https://docs.jsonrpc.ru>
 * PyPI Releases: <https://pypi.org/project/jsonrpc-py>
 * Source Code: <https://gitlab.com/jsonrpc/jsonrpc-py>
 
 [homepage]: <https://gitlab.com/jsonrpc/jsonrpc-py>
 [pipeline]: <https://img.shields.io/gitlab/pipeline-status/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
 [coverage]: <https://img.shields.io/gitlab/pipeline-coverage/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
```

### Comparing `jsonrpc-py-3.0.9/docs/changelog/v1.x.x/v1.1.0.rst` & `jsonrpc-py-3.1.0/docs/changelog/v1.x.x/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.0.1.rst` & `jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.0.1.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/docs/changelog/v2.x.x/v2.3.0.rst` & `jsonrpc-py-3.1.0/docs/changelog/v2.x.x/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/docs/changelog/v3.x.x/v3.0.0.rst` & `jsonrpc-py-3.1.0/docs/changelog/v3.x.x/v3.0.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/docs/changelog.rst` & `jsonrpc-py-3.1.0/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/docs/conf.py` & `jsonrpc-py-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/docs/deployment.rst` & `jsonrpc-py-3.1.0/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/docs/index.rst` & `jsonrpc-py-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/docs/quickstart.rst` & `jsonrpc-py-3.1.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/docs/reference.rst` & `jsonrpc-py-3.1.0/docs/reference.rst`

 * *Files 6% similar despite different names*

```diff
@@ -49,7 +49,13 @@
   :members:
 
 Data Serialization
 ------------------
 
 .. autoclass:: JSONSerializer
   :members:
+
+Lifespan
+--------
+
+.. autoclass:: LifespanEvents
+  :members:
```

### Comparing `jsonrpc-py-3.0.9/jsonrpc/__init__.py` & `jsonrpc-py-3.1.0/jsonrpc/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 """
 
 from typing import Final
 
 from .asgi import ASGIHandler
 from .dispatcher import AsyncDispatcher
 from .errors import Error, ErrorEnum
+from .lifespan import LifespanEvents
 from .request import BatchRequest, Request
 from .response import BatchResponse, Response
 from .serializer import JSONSerializer
 
 __all__: Final[tuple[str, ...]] = (
     "ASGIHandler",
     "AsyncDispatcher",
     "BatchRequest",
     "BatchResponse",
     "Error",
     "ErrorEnum",
     "JSONSerializer",
+    "LifespanEvents",
     "Request",
     "Response",
 )
```

### Comparing `jsonrpc-py-3.0.9/jsonrpc/asgi.py` & `jsonrpc-py-3.1.0/jsonrpc/asgi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,78 @@
 import re
 from asyncio import CancelledError, Task, create_task, shield
 from collections import UserDict
 from collections.abc import Generator, MutableSequence
 from http import HTTPMethod, HTTPStatus
 from io import DEFAULT_BUFFER_SIZE, BytesIO
-from typing import Any, ClassVar, Final, TypeAlias
+from typing import Any, ClassVar, Final, Generic, TypeAlias, TypeVar
 
 from .dispatcher import AsyncDispatcher
 from .errors import Error
+from .lifespan import LifespanEvents, LifespanManager
 from .request import BatchRequest, Request
 from .response import BatchResponse, Response
 from .serializer import JSONSerializer
 from .typedefs import ASGIReceiveCallable, ASGISendCallable, HTTPConnectionScope, Scope
-from .utilities import multiple_coroutines
+from .utilities import CancellableGather
 
 __all__: Final[tuple[str, ...]] = ("ASGIHandler",)
 
+KT = TypeVar("KT")
+VT = TypeVar("VT")
+
+
+class ASGIHandler(UserDict[KT, VT], Generic[KT, VT]):
+    """
+    Base class representing the ``ASGI`` entry point.
+    Its subclassing the :py:class:`collections.UserDict` object
+    for providing the user-defined data storage.
+
+    For example::
+
+        >>> app = ASGIHandler()
+        >>> app["my_private_key"] = "foobar"
+        >>> app["my_private_key"]
+        "foobar"
+    """
+
+    __slots__: tuple[str, ...] = ()
+
+    #: The default content type of the responses.
+    content_type: ClassVar[str] = "application/json"
+
+    #: Class variable representing the :class:`jsonrpc.AsyncDispatcher` object
+    #: used by this class for routing user-defined functions by default.
+    dispatcher: Final[AsyncDispatcher] = AsyncDispatcher()
+
+    #: Class variable representing the :class:`jsonrpc.JSONSerializer` object
+    #: used by this class for data serialization by default.
+    serializer: Final[JSONSerializer] = JSONSerializer()
+
+    #: Class variable representing the :class:`jsonrpc.LifespanEvents` object
+    #: used by this class for storing the user-defined functions that running
+    #: when application is initiated and shutting down.
+    events: Final[LifespanEvents] = LifespanEvents()
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__qualname__}({self.data!r})"
+
+    async def __call__(self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable) -> None:
+        match scope:
+            case {"type": "http", **kwargs}:  # noqa: F841
+                await HTTPHandler(scope, receive, send, self.__class__)  # type: ignore[arg-type]
+            case {"type": "lifespan", **kwargs}:  # noqa: F841
+                await LifespanManager(receive, send, self.events)
+            case _:
+                raise ValueError("Only ASGI/HTTP connections are allowed.")
+
+
+#: ---
+#: Useful typing aliases, such as too generic objects.
+AnyASGIHandler: TypeAlias = ASGIHandler[Any, Any]
 AnyTask: TypeAlias = Task[Any]
 AnyRequest: TypeAlias = Request | Error | BatchRequest
 AnyResponse: TypeAlias = Response | BatchResponse | None
 
 #: ---
 #: Ensure that "Content-Type" is a valid JSON header.
 JSON_CTYPE_REGEXB: Final[re.Pattern[bytes]] = re.compile(
@@ -53,20 +106,20 @@
     background_tasks: Final[set[AnyTask]] = set()
 
     def __init__(
         self,
         scope: HTTPConnectionScope,
         receive: ASGIReceiveCallable,
         send: ASGISendCallable,
-        app: type["ASGIHandler"],
+        app: type[AnyASGIHandler],
     ) -> None:
         self.scope: Final[HTTPConnectionScope] = scope
         self.receive: Final[ASGIReceiveCallable] = receive
         self.send: Final[ASGISendCallable] = send
-        self.app: type[ASGIHandler] = app
+        self.app: type[AnyASGIHandler] = app
 
     def __await__(self) -> Generator[Any, None, None]:
         #: ---
         #: Create a suitable iterator by calling __await__ on a coroutine.
         return self.__await_impl__().__await__()
 
     async def __await_impl__(self) -> None:
@@ -154,15 +207,15 @@
 
         try:
             obj: Any = self.app.serializer.deserialize(payload)
         except Error as error:
             return write_error(error)
 
         is_batch_request: bool = isinstance(obj, MutableSequence) and len(obj) >= 1
-        request: AnyRequest = BatchRequest.from_json(obj) if is_batch_request else Request.from_json(obj)
+        request: AnyRequest = (BatchRequest if is_batch_request else Request).from_json(obj)  # type: ignore[attr-defined]
 
         if not (response := await self.process_request(request)):
             return b""
 
         try:
             return self.app.serializer.serialize(response.json)
         except Error as error:
@@ -197,54 +250,16 @@
             try:
                 result: Any = await shield(task)
                 return Response(body=result, response_id=request.request_id)
             except Error as error:
                 return Response(error=error, response_id=request.request_id)
 
         async def on_batch_request(request: BatchRequest) -> BatchResponse:
-            responses: tuple[AnyResponse, ...] = await multiple_coroutines(map(self.process_request, request))
+            responses: tuple[AnyResponse, ...] = await CancellableGather(map(self.process_request, request))
             return BatchResponse([response for response in responses if isinstance(response, Response)])
 
         if isinstance(obj, Error):
             return on_error(obj)
         elif isinstance(obj, Request):
             return await on_request(obj)
         else:
             return await on_batch_request(obj)
-
-
-class ASGIHandler(UserDict[str, Any]):
-    """
-    Base class representing the ``ASGI`` entry point.
-    Its subclassing the :py:class:`collections.UserDict` object
-    for providing the user-defined data storage.
-
-    For example::
-
-        >>> app = ASGIHandler()
-        >>> app["my_private_key"] = "foobar"
-        >>> app["my_private_key"]
-        "foobar"
-    """
-
-    __slots__: tuple[str, ...] = ()
-
-    #: The default content type of the responses.
-    content_type: ClassVar[str] = "application/json"
-
-    #: Class variable representing the :class:`jsonrpc.AsyncDispatcher` object
-    #: used by this class for routing user-defined functions by default.
-    dispatcher: Final[AsyncDispatcher] = AsyncDispatcher()
-
-    #: Class variable representing the :class:`jsonrpc.JSONSerializer` object
-    #: used by this class for data serialization by default.
-    serializer: Final[JSONSerializer] = JSONSerializer()
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__qualname__}({self.data!r})"
-
-    async def __call__(self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable) -> None:
-        match scope:
-            case {"type": "http", **kwargs}:  # noqa: F841
-                await HTTPHandler(scope, receive, send, self.__class__)  # type: ignore[arg-type]
-            case _:
-                raise ValueError("Only ASGI/HTTP connections are allowed.")
```

### Comparing `jsonrpc-py-3.0.9/jsonrpc/dispatcher.py` & `jsonrpc-py-3.1.0/jsonrpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/jsonrpc/errors.py` & `jsonrpc-py-3.1.0/jsonrpc/errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/jsonrpc/request.py` & `jsonrpc-py-3.1.0/jsonrpc/request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/jsonrpc/response.py` & `jsonrpc-py-3.1.0/jsonrpc/response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/jsonrpc/serializer.py` & `jsonrpc-py-3.1.0/jsonrpc/serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/jsonrpc/typedefs.py` & `jsonrpc-py-3.1.0/jsonrpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/jsonrpc/utilities.py` & `jsonrpc-py-3.1.0/jsonrpc/utilities.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,114 +1,147 @@
-from asyncio import AbstractEventLoop, Future, Task, TaskGroup, get_running_loop
-from collections.abc import Callable, Coroutine, Generator, Iterable, Iterator, MutableMapping
+from asyncio import AbstractEventLoop, Task, TaskGroup, get_running_loop
+from collections.abc import Awaitable, Callable, Coroutine, Generator, Iterable, Iterator, MutableMapping
 from contextvars import Context, copy_context
 from dataclasses import dataclass, field
-from functools import partial
+from functools import partial, total_ordering
 from heapq import heappop, heappush
 from inspect import iscoroutinefunction
-from typing import Any, Final, Generic, Literal, ParamSpec, TypeAlias, TypeGuard, TypeVar, final
+from typing import Any, Final, Generic, Literal, ParamSpec, TypeAlias, TypeGuard, TypeVar, final, overload
 
 __all__: Final[tuple[str, ...]] = (
+    "CancellableGather",
     "ensure_async",
     "is_iterable",
     "make_hashable",
-    "multiple_coroutines",
+    "PrioritizedItem",
     "Undefined",
     "UndefinedType",
 )
 
 T = TypeVar("T")
 P = ParamSpec("P")
 CoroutineLike: TypeAlias = Generator[Any, None, T] | Coroutine[Any, Any, T]
 
 
-def ensure_async(user_function: Callable[P, Any], /, *args: P.args, **kwargs: P.kwargs) -> Future[Any]:
-    loop: AbstractEventLoop = get_running_loop()
-    context: Context = copy_context()
-
-    if iscoroutinefunction(callback := partial(user_function, *args, **kwargs)):
-        return loop.create_task(callback(), context=context)
-    else:
-        return loop.run_in_executor(None, context.run, callback)
-
-
-def is_iterable(obj: Any, /) -> TypeGuard[Iterable[Any]]:
-    try:
-        iter(obj)
-    except TypeError:
-        return False
-    else:
-        return True
-
-
-def make_hashable(obj: Any, /) -> Any:
-    if isinstance(obj, MutableMapping):
-        return tuple((key, make_hashable(value)) for key, value in sorted(obj.items()))
-    #: ---
-    #: Try hash to avoid converting a hashable iterable (e.g. string, frozenset)
-    #: to a tuple:
-    try:
-        hash(obj)
-    except TypeError:
-        if is_iterable(obj):
-            return tuple(map(make_hashable, obj))
-        #: ---
-        #: Non-hashable, non-iterable:
-        raise
-
-    return obj
+@total_ordering
+@dataclass(eq=False, slots=True)
+class PrioritizedItem(Generic[T]):
+    priority: int
+    item: T
+
+    def __eq__(self, obj: Any) -> bool:
+        if not isinstance(obj, self.__class__):
+            return NotImplemented
+        return self.priority == obj.priority
+
+    def __lt__(self, obj: Any) -> bool:
+        if not isinstance(obj, self.__class__):
+            return NotImplemented
+        return self.priority < obj.priority
 
 
-@dataclass(repr=False, eq=False, slots=True)
-class multiple_coroutines(Generic[T]):
+@dataclass(slots=True)
+class CancellableGather(Generic[T]):
     coroutines: Iterable[CoroutineLike[T]]
-    queue: list[tuple[int, T]] = field(default_factory=list, init=False)
+    results: list[PrioritizedItem[T]] = field(default_factory=list, init=False)
 
     def __await__(self) -> Generator[Any, None, tuple[T, ...]]:
         #: ---
         #: Create a suitable iterator by calling __await__ on a coroutine.
         return self.__await_impl__().__await__()
 
     async def __await_impl__(self) -> tuple[T, ...]:
         context: Final[Context] = copy_context()
         try:
-            async with TaskGroup() as tg:
-                for task_id, coroutine in enumerate(self.coroutines):
-                    task: Task[T] = tg.create_task(coroutine, context=context)
-                    callback: partial[None] = partial(self.populate_results, task_id=task_id)
+            async with TaskGroup() as group:
+                for priority, coroutine in enumerate(self.coroutines):
+                    task: Task[T] = group.create_task(coroutine, context=context)
+                    callback: partial[None] = partial(self.populate_results, priority=priority)
                     task.add_done_callback(callback, context=context)
         except BaseExceptionGroup as exc_group:
             #: ---
             #: Propagate the first raised exception from exception group:
             for exc in self.exception_from_group(exc_group):
                 raise exc from None
 
         return tuple(self.iter_results())
 
-    def populate_results(self, task: Task[T], *, task_id: int) -> None:
+    def populate_results(self, task: Task[T], *, priority: int) -> None:
         if not task.cancelled() and task.exception() is None:
-            result: Final[T] = task.result()
-            heappush(self.queue, (task_id, result))
+            result: PrioritizedItem[T] = PrioritizedItem(priority, task.result())
+            heappush(self.results, result)
 
     def exception_from_group(self, exc: BaseException) -> Iterator[BaseException]:
         if isinstance(exc, BaseExceptionGroup):
             for nested in exc.exceptions:
                 yield from self.exception_from_group(nested)
         else:
             yield exc
 
     def iter_results(self) -> Iterator[T]:
         while True:
             try:
-                _, result = heappop(self.queue)
-                yield result
+                result: PrioritizedItem[T] = heappop(self.results)
+                yield result.item
             except IndexError:
                 break
 
 
+@overload
+async def ensure_async(user_function: Callable[P, Awaitable[T]], /, *args: P.args, **kwargs: P.kwargs) -> T:
+    ...
+
+
+@overload
+async def ensure_async(user_function: Callable[P, CoroutineLike[T]], /, *args: P.args, **kwargs: P.kwargs) -> T:
+    ...
+
+
+@overload
+async def ensure_async(user_function: Callable[P, T], /, *args: P.args, **kwargs: P.kwargs) -> T:
+    ...
+
+
+async def ensure_async(user_function: Callable[P, Any], /, *args: P.args, **kwargs: P.kwargs) -> Any:
+    loop: AbstractEventLoop = get_running_loop()
+    context: Context = copy_context()
+
+    if iscoroutinefunction(callback := partial(user_function, *args, **kwargs)):
+        return await loop.create_task(callback(), context=context)
+    else:
+        return await loop.run_in_executor(None, context.run, callback)
+
+
+def is_iterable(obj: Any, /) -> TypeGuard[Iterable[Any]]:
+    try:
+        iter(obj)
+    except TypeError:
+        return False
+    else:
+        return True
+
+
+def make_hashable(obj: Any, /) -> Any:
+    if isinstance(obj, MutableMapping):
+        return tuple((key, make_hashable(value)) for key, value in sorted(obj.items()))
+    #: ---
+    #: Try hash to avoid converting a hashable iterable (e.g. string, frozenset)
+    #: to a tuple:
+    try:
+        hash(obj)
+    except TypeError:
+        if is_iterable(obj):
+            return tuple(map(make_hashable, obj))
+        #: ---
+        #: Non-hashable, non-iterable:
+        raise
+
+    return obj
+
+
 @final
 class UndefinedType:
     __slots__: tuple[str, ...] = ()
 
     def __repr__(self) -> Literal["Undefined"]:
         return "Undefined"
```

### Comparing `jsonrpc-py-3.0.9/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc-py-3.1.0/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.9
+Version: 3.1.0
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Homepage, https://docs.jsonrpc.ru
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
@@ -27,46 +27,46 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: ujson
 License-File: LICENSE
 
-JSON-RPC Python
-===============
+# JSON-RPC Python
+
 [![pipeline status][pipeline]][homepage]
 [![coverage report][coverage]][homepage]
 [![latest release][version]][pypi]
 [![pypi downloads][downloads]][pypi]
 
 **JSON-RPC Python** is a lightweight ASGI micro framework for building web applications.
 
-Features
---------
+## Features
+
 * Pure zero-dependency JSON-RPC 2.0 implementation.
 * Simple and user-friendly API interface.
 * 100% type annotated codebase.
 * 100% test coverage, so it's production-ready.
 
-Requirements
-------------
+## Requirements
+
 Python 3.11 and above.
 
-Installation
-------------
+## Installation
+
 ```
 $ pip install jsonrpc-py
 ```
 
-Distribution
-------------
+## Distribution
+
 This project is licensed under the terms of the [BSD 3-Clause License](LICENSE).
 
-Links
------
+## Links
+
 * Documentation: <https://docs.jsonrpc.ru>
 * PyPI Releases: <https://pypi.org/project/jsonrpc-py>
 * Source Code: <https://gitlab.com/jsonrpc/jsonrpc-py>
 
 [homepage]: <https://gitlab.com/jsonrpc/jsonrpc-py>
 [pipeline]: <https://img.shields.io/gitlab/pipeline-status/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
 [coverage]: <https://img.shields.io/gitlab/pipeline-coverage/jsonrpc/jsonrpc-py?branch=development&logo=gitlab&style=flat-square>
```

### Comparing `jsonrpc-py-3.0.9/jsonrpc_py.egg-info/SOURCES.txt` & `jsonrpc-py-3.1.0/jsonrpc_py.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -42,26 +42,32 @@
 docs/changelog/v2.x.x/v2.4.8.rst
 docs/changelog/v2.x.x/v2.4.9.rst
 docs/changelog/v2.x.x/v2.5.0.rst
 docs/changelog/v2.x.x/v2.5.1.rst
 docs/changelog/v3.x.x/index.rst
 docs/changelog/v3.x.x/v3.0.0.rst
 docs/changelog/v3.x.x/v3.0.1.rst
+docs/changelog/v3.x.x/v3.0.10.rst
+docs/changelog/v3.x.x/v3.0.11.rst
+docs/changelog/v3.x.x/v3.0.12.rst
+docs/changelog/v3.x.x/v3.0.13.rst
 docs/changelog/v3.x.x/v3.0.2.rst
 docs/changelog/v3.x.x/v3.0.3.rst
 docs/changelog/v3.x.x/v3.0.4.rst
 docs/changelog/v3.x.x/v3.0.5.rst
 docs/changelog/v3.x.x/v3.0.6.rst
 docs/changelog/v3.x.x/v3.0.7.rst
 docs/changelog/v3.x.x/v3.0.8.rst
 docs/changelog/v3.x.x/v3.0.9.rst
+docs/changelog/v3.x.x/v3.1.0.rst
 jsonrpc/__init__.py
 jsonrpc/asgi.py
 jsonrpc/dispatcher.py
 jsonrpc/errors.py
+jsonrpc/lifespan.py
 jsonrpc/py.typed
 jsonrpc/request.py
 jsonrpc/response.py
 jsonrpc/serializer.py
 jsonrpc/typedefs.py
 jsonrpc/utilities.py
 jsonrpc_py.egg-info/PKG-INFO
@@ -69,11 +75,12 @@
 jsonrpc_py.egg-info/dependency_links.txt
 jsonrpc_py.egg-info/requires.txt
 jsonrpc_py.egg-info/top_level.txt
 tests/__init__.py
 tests/test_asgi.py
 tests/test_dispatcher.py
 tests/test_errors.py
+tests/test_lifespan.py
 tests/test_request.py
 tests/test_response.py
 tests/test_serializer.py
 tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.0.9/pyproject.toml` & `jsonrpc-py-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
-    "Typing :: Typed"
+    "Typing :: Typed",
 ]
 requires-python = ">=3.11"
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Andrew Malchuk"
 email = "andrew.malchuk@yandex.ru"
```

### Comparing `jsonrpc-py-3.0.9/tests/test_asgi.py` & `jsonrpc-py-3.1.0/tests/test_asgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from asyncio import Event, Queue, get_running_loop, sleep, wait_for
 from collections.abc import MutableMapping
 from http import HTTPMethod, HTTPStatus
 from typing import Any, Final, Literal
-from unittest import IsolatedAsyncioTestCase, TestCase
+from unittest import IsolatedAsyncioTestCase as AsyncioTestCase, TestCase
 from unittest.mock import AsyncMock
 from uuid import UUID, uuid4
 
 from httpx import AsyncClient, Response
 
 from jsonrpc import ASGIHandler, ErrorEnum
 
@@ -19,35 +19,33 @@
 
     def __eq__(self, string: str) -> Literal[True]:
         self.test_case.assertIsInstance(string, str)
         self.test_case.assertGreater(len(string), 0)
         return True
 
 
-class TestASGIHandler(IsolatedAsyncioTestCase):
+class TestASGIHandler(AsyncioTestCase):
     def setUp(self) -> None:
         self.app: ASGIHandler = ASGIHandler()
         self.receive_channel: AsyncMock = AsyncMock()
         self.send_channel: AsyncMock = AsyncMock()
 
     def test_inheritance(self) -> None:
         self.assertIsInstance(self.app, MutableMapping)
 
     async def test_supported_scopes(self) -> None:
-        for scope in {"type": "websocket"}, {"type": "lifespan"}:
-            with self.subTest(scope=scope):
-                with self.assertRaises(ValueError) as context:
-                    await self.app(scope, self.receive_channel, self.send_channel)
+        with self.assertRaises(ValueError) as context:
+            await self.app({"type": "websocket"}, self.receive_channel, self.send_channel)
 
-                self.assertEqual(str(context.exception), "Only ASGI/HTTP connections are allowed.")
-                self.receive_channel.assert_not_called()
-                self.send_channel.assert_not_called()
+        self.assertEqual(str(context.exception), "Only ASGI/HTTP connections are allowed.")
+        self.receive_channel.assert_not_called()
+        self.send_channel.assert_not_called()
 
 
-class TestHTTPHandler(IsolatedAsyncioTestCase):
+class TestHTTPHandler(AsyncioTestCase):
     @property
     def random_id(self) -> str:
         uuid: Final[UUID] = uuid4()
         return str(uuid)
 
     def setUp(self) -> None:
         self.app: ASGIHandler = ASGIHandler()
```

### Comparing `jsonrpc-py-3.0.9/tests/test_dispatcher.py` & `jsonrpc-py-3.1.0/tests/test_dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from collections.abc import Callable, MutableMapping
 from types import FunctionType, LambdaType
 from typing import NoReturn, TypeVar
-from unittest import IsolatedAsyncioTestCase
+from unittest import IsolatedAsyncioTestCase as AsyncioTestCase
 
 from jsonrpc import AsyncDispatcher, Error, ErrorEnum
 
 T = TypeVar("T")
 
 
-class TestDispatcher(IsolatedAsyncioTestCase):
+class TestDispatcher(AsyncioTestCase):
     def setUp(self) -> None:
         self.dispatcher: AsyncDispatcher = AsyncDispatcher()
 
     def test_inheritance(self) -> None:
         self.assertIsInstance(self.dispatcher, MutableMapping)
 
     def test_register_not_function(self) -> None:
```

### Comparing `jsonrpc-py-3.0.9/tests/test_errors.py` & `jsonrpc-py-3.1.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/tests/test_request.py` & `jsonrpc-py-3.1.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/tests/test_response.py` & `jsonrpc-py-3.1.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/tests/test_serializer.py` & `jsonrpc-py-3.1.0/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.9/tests/test_utilities.py` & `jsonrpc-py-3.1.0/tests/test_utilities.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,125 +1,78 @@
 from asyncio import create_task, sleep, wait_for
+from dataclasses import is_dataclass
 from typing import Any, Literal, NoReturn
-from unittest import IsolatedAsyncioTestCase, TestCase
+from unittest import IsolatedAsyncioTestCase as AsyncioTestCase, TestCase
 from unittest.mock import AsyncMock, MagicMock, sentinel
 
-from jsonrpc.utilities import Undefined, UndefinedType, ensure_async, make_hashable, multiple_coroutines
+from jsonrpc.utilities import CancellableGather, PrioritizedItem, Undefined, UndefinedType, ensure_async, make_hashable
 
 
-class TestHashable(TestCase):
-    def test_equality(self) -> None:
-        tests: tuple[tuple[Any, Any], ...] = (
-            ([], ()),
-            (["a", 1], ("a", 1)),
-            ({}, ()),
-            ({"a"}, ("a",)),
-            (frozenset({"a"}), {"a"}),
-            ({"a": 1, "b": 2}, (("a", 1), ("b", 2))),
-            ({"b": 2, "a": 1}, (("a", 1), ("b", 2))),
-            (("a", ["b", 1]), ("a", ("b", 1))),
-            (("a", {"b": 1}), ("a", (("b", 1),))),
-        )
-        for actual, expected in tests:
-            with self.subTest(actual=actual):
-                self.assertEqual(make_hashable(actual), expected)
-
-    def test_count_equality(self) -> None:
-        tests: tuple[tuple[Any, Any], ...] = (
-            ({"a": 1, "b": ["a", 1]}, (("a", 1), ("b", ("a", 1)))),
-            ({"a": 1, "b": ("a", [1, 2])}, (("a", 1), ("b", ("a", (1, 2))))),
-        )
-        for actual, expected in tests:
-            with self.subTest(actual=actual):
-                self.assertCountEqual(make_hashable(actual), expected)
-
-    def test_unhashable(self) -> None:
-        class Unhashable:
-            __hash__: Literal[None] = None
+class TestCancellableGather(AsyncioTestCase):
+    def test_prioritized_item(self) -> None:
+        self.assertTrue(is_dataclass(prioritized_item := PrioritizedItem(0, "for testing purposes")))
+        self.assertEqual(prioritized_item, PrioritizedItem(0, b"for testing purposes"))
+        self.assertNotEqual(prioritized_item, PrioritizedItem(123, "for testing purposes"))
+        self.assertLess(prioritized_item, PrioritizedItem(1, "the other one"))
+        self.assertNotEqual(prioritized_item, "for testing purposes")
 
-        with self.assertRaises(TypeError) as context:
-            make_hashable(Unhashable())
-
-        self.assertIn("unhashable type", str(context.exception))
+        with self.assertRaises(TypeError):
+            prioritized_item < "for testing purposes"  # noqa: B015
 
-
-class TestUndefined(TestCase):
-    def test_hash(self) -> None:
-        self.assertEqual(hash(Undefined), 0xBAADF00D)
-
-    def test_equality(self) -> None:
-        self.assertEqual(Undefined, UndefinedType())
-        self.assertNotEqual(Undefined, None)
-
-    def test_is_truth(self) -> None:
-        self.assertFalse(Undefined)
-
-
-class TestAsyncioUtilities(IsolatedAsyncioTestCase):
-    async def test_ensure_async(self) -> None:
-        for mock in (
-            MagicMock(return_value=sentinel.sync_def),
-            AsyncMock(return_value=sentinel.async_def),
-        ):
-            with self.subTest(mock=mock):
-                result: Any = await ensure_async(mock, 1, 2, 3, key="value")
-                self.assertIs(result, mock.return_value)
-                mock.assert_called_once_with(1, 2, 3, key="value")
-
-    async def test_multiple_coroutines(self) -> None:
+    async def test_awaited_once(self) -> None:
         mocks: set[AsyncMock] = {AsyncMock(return_value=i) for i in ("a", "b", "c")}
 
         async def inner(mock: AsyncMock) -> Any:
             return await mock()
 
-        results: tuple[str, ...] = await multiple_coroutines(map(inner, mocks))
+        results: tuple[str, ...] = await CancellableGather(map(inner, mocks))
         self.assertCountEqual(results, ("a", "b", "c"))
 
         for mock in mocks:
             with self.subTest(mock=mock):
                 mock.assert_awaited_once()
 
-    async def test_multiple_coroutines_preserved_order(self) -> None:
-        results: tuple[str, ...] = await multiple_coroutines(
+    async def test_preserved_order(self) -> None:
+        results: tuple[str, ...] = await CancellableGather(
             (
                 sleep(0.04, "a"),  # <-- accepted latest but should be first in results
                 sleep(0.02, "b"),  # <-- accepted second and should be second in results
                 sleep(0.01, "c"),  # <-- accepted first but should be third in results
                 sleep(0.03, "d"),  # <-- accepted third but should be latest in results
             )
         )
         self.assertTupleEqual(results, ("a", "b", "c", "d"))
 
-    async def test_multiple_coroutines_exception(self) -> None:
+    async def test_exception(self) -> None:
         first_exception_mock: AsyncMock = AsyncMock(side_effect=Exception("first exception"))
         second_exception_mock: AsyncMock = AsyncMock(side_effect=Exception("second exception"))
 
         async def inner(mock: AsyncMock) -> Any:
             return await mock()
 
         with self.assertRaises(Exception) as context:
-            await multiple_coroutines(map(inner, (first_exception_mock, second_exception_mock)))
+            await CancellableGather(map(inner, (first_exception_mock, second_exception_mock)))
 
         self.assertRegex(str(context.exception), r"(?:first|second) exception")
         first_exception_mock.assert_awaited_once()
         second_exception_mock.assert_awaited_once()
 
-    async def test_multiple_coroutines_timeout_error(self) -> None:
+    async def test_timeout_error(self) -> None:
         hello_task, world_task = create_task(sleep(3600.0, "hello")), create_task(sleep(3600.0, "world"))
         with self.assertRaises(TimeoutError):
-            await multiple_coroutines(
+            await CancellableGather(
                 [
                     wait_for(hello_task, timeout=0.001),
                     wait_for(world_task, timeout=0.002),
                 ]
             )
         self.assertTrue(hello_task.cancelled())
         self.assertTrue(world_task.cancelled())
 
-    async def test_multiple_coroutines_exception_group(self) -> None:
+    async def test_exception_group(self) -> None:
         async def inner() -> NoReturn:
             raise ExceptionGroup(
                 "one",
                 (
                     Exception("for testing purposes"),  # <-- this should be raised first
                     ExceptionGroup(
                         "two",
@@ -135,10 +88,70 @@
                             Exception("5"),
                         ),
                     ),
                 ),
             )
 
         with self.assertRaises(Exception) as context:
-            await multiple_coroutines([inner()])
+            await CancellableGather([inner()])
 
         self.assertEqual(str(context.exception), "for testing purposes")
+
+
+class TestAsyncioUtilities(AsyncioTestCase):
+    async def test_ensure_async(self) -> None:
+        for mock in (
+            MagicMock(return_value=sentinel.sync_def),
+            AsyncMock(return_value=sentinel.async_def),
+        ):
+            with self.subTest(mock=mock):
+                result: Any = await ensure_async(mock, 1, 2, 3, key="value")
+                self.assertIs(result, mock.return_value)
+                mock.assert_called_once_with(1, 2, 3, key="value")
+
+
+class TestHashable(TestCase):
+    def test_equality(self) -> None:
+        tests: tuple[tuple[Any, Any], ...] = (
+            ([], ()),
+            (["a", 1], ("a", 1)),
+            ({}, ()),
+            ({"a"}, ("a",)),
+            (frozenset({"a"}), {"a"}),
+            ({"a": 1, "b": 2}, (("a", 1), ("b", 2))),
+            ({"b": 2, "a": 1}, (("a", 1), ("b", 2))),
+            (("a", ["b", 1]), ("a", ("b", 1))),
+            (("a", {"b": 1}), ("a", (("b", 1),))),
+        )
+        for actual, expected in tests:
+            with self.subTest(actual=actual):
+                self.assertEqual(make_hashable(actual), expected)
+
+    def test_count_equality(self) -> None:
+        tests: tuple[tuple[Any, Any], ...] = (
+            ({"a": 1, "b": ["a", 1]}, (("a", 1), ("b", ("a", 1)))),
+            ({"a": 1, "b": ("a", [1, 2])}, (("a", 1), ("b", ("a", (1, 2))))),
+        )
+        for actual, expected in tests:
+            with self.subTest(actual=actual):
+                self.assertCountEqual(make_hashable(actual), expected)
+
+    def test_unhashable(self) -> None:
+        class Unhashable:
+            __hash__: Literal[None] = None
+
+        with self.assertRaises(TypeError) as context:
+            make_hashable(Unhashable())
+
+        self.assertIn("unhashable type", str(context.exception))
+
+
+class TestUndefined(TestCase):
+    def test_hash(self) -> None:
+        self.assertEqual(hash(Undefined), 0xBAADF00D)
+
+    def test_equality(self) -> None:
+        self.assertEqual(Undefined, UndefinedType())
+        self.assertNotEqual(Undefined, None)
+
+    def test_is_truth(self) -> None:
+        self.assertFalse(Undefined)
```

