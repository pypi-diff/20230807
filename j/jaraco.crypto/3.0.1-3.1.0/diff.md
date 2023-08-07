# Comparing `tmp/jaraco.crypto-3.0.1.tar.gz` & `tmp/jaraco.crypto-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.crypto-3.0.1.tar", last modified: Mon Mar 15 01:58:19 2021, max compression
+gzip compressed data, was "jaraco.crypto-3.1.0.tar", last modified: Mon Aug  7 00:22:16 2023, max compression
```

## Comparing `jaraco.crypto-3.0.1.tar` & `jaraco.crypto-3.1.0.tar`

### file list

```diff
@@ -1,52 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:58:19.754257 jaraco.crypto-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:58:19.750257 jaraco.crypto-3.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:58:19.750257 jaraco.crypto-3.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/.github/workflows/automerge.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      798 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2021-03-15 01:58:19.754257 jaraco.crypto-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/certutil.py
--rw-r--r--   0 runner    (1001) docker     (121)      305 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:58:19.750257 jaraco.crypto-3.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      756 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      870 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:58:19.750257 jaraco.crypto-3.0.1/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:58:19.754257 jaraco.crypto-3.0.1/jaraco/crypto/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    39912 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/blowfish.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/cert.py
--rw-r--r--   0 runner    (1001) docker     (121)     4441 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/cipher.py
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/digest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3466 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/evp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:58:19.754257 jaraco.crypto-3.0.1/jaraco/crypto/itsdangerous/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/itsdangerous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/itsdangerous/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/rand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/support.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:58:19.754257 jaraco.crypto-3.0.1/jaraco/crypto/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/tests/test_cipher.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/tests/test_digest.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/tests/test_rand.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/jaraco/crypto/tests/test_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 01:58:19.754257 jaraco.crypto-3.0.1/jaraco.crypto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2021-03-15 01:58:19.000000 jaraco.crypto-3.0.1/jaraco.crypto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      928 2021-03-15 01:58:19.000000 jaraco.crypto-3.0.1/jaraco.crypto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-15 01:58:19.000000 jaraco.crypto-3.0.1/jaraco.crypto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      280 2021-03-15 01:58:19.000000 jaraco.crypto-3.0.1/jaraco.crypto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-15 01:58:19.000000 jaraco.crypto-3.0.1/jaraco.crypto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-03-15 01:58:19.754257 jaraco.crypto-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10139 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/skeleton.md
--rw-r--r--   0 runner    (1001) docker     (121)      707 2021-03-15 01:57:53.000000 jaraco.crypto-3.0.1/tox.ini
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.053395 jaraco.crypto-3.1.0/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      133 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/.coveragerc
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      246 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/.editorconfig
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.047963 jaraco.crypto-3.1.0/.github/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      148 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/.github/dependabot.yml
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.048155 jaraco.crypto-3.1.0/.github/workflows/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3146 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/.github/workflows/main.yml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       81 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      188 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/.readthedocs.yaml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1023 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/LICENSE
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      927 2023-08-07 00:22:03.000000 jaraco.crypto-3.1.0/NEWS.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2031 2023-08-07 00:22:16.053497 jaraco.crypto-3.1.0/PKG-INFO
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1481 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/README.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1504 2023-08-06 23:57:22.000000 jaraco.crypto-3.1.0/certutil.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      261 2023-08-07 00:13:38.000000 jaraco.crypto-3.1.0/conftest.py
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.048797 jaraco.crypto-3.1.0/docs/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1203 2023-08-07 00:07:21.000000 jaraco.crypto-3.1.0/docs/conf.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       78 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/docs/history.rst
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      910 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/docs/index.rst
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.043575 jaraco.crypto-3.1.0/jaraco/
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.051658 jaraco.crypto-3.1.0/jaraco/crypto/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)        0 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/__init__.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)    39889 2023-08-06 23:56:39.000000 jaraco.crypto-3.1.0/jaraco/crypto/blowfish.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2178 2023-08-07 00:10:08.000000 jaraco.crypto-3.1.0/jaraco/crypto/cert.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4785 2023-08-06 23:56:39.000000 jaraco.crypto-3.1.0/jaraco/crypto/cipher.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1835 2023-08-06 23:56:39.000000 jaraco.crypto-3.1.0/jaraco/crypto/digest.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3647 2023-08-07 00:12:12.000000 jaraco.crypto-3.1.0/jaraco/crypto/evp.py
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.052068 jaraco.crypto-3.1.0/jaraco/crypto/itsdangerous/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)        0 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/itsdangerous/__init__.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2260 2023-08-06 23:56:39.000000 jaraco.crypto-3.1.0/jaraco/crypto/itsdangerous/compat.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1167 2023-08-06 23:56:39.000000 jaraco.crypto-3.1.0/jaraco/crypto/rand.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1395 2023-08-07 00:03:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/support.py
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.053199 jaraco.crypto-3.1.0/jaraco/crypto/tests/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)        0 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/tests/__init__.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1207 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/tests/test_cipher.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      804 2023-08-06 23:52:24.000000 jaraco.crypto-3.1.0/jaraco/crypto/tests/test_digest.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      561 2023-08-06 23:52:24.000000 jaraco.crypto-3.1.0/jaraco/crypto/tests/test_rand.py
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      715 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/tests/test_threads.py
+drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.049704 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2031 2023-08-07 00:22:16.000000 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/PKG-INFO
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      903 2023-08-07 00:22:16.000000 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/SOURCES.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)        1 2023-08-07 00:22:16.000000 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/dependency_links.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      275 2023-08-07 00:22:16.000000 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/requires.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)        7 2023-08-07 00:22:16.000000 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/top_level.txt
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      154 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/mypy.ini
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      186 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/pyproject.toml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      842 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/pytest.ini
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1023 2023-08-07 00:22:16.053855 jaraco.crypto-3.1.0/setup.cfg
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)       44 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/towncrier.toml
+-rw-r--r--   0 jaraco   (697332) primarygroup (89939)      771 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/tox.ini
```

### Comparing `jaraco.crypto-3.0.1/CHANGES.rst` & `jaraco.crypto-3.1.0/NEWS.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v3.1.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
+Bugfixes
+--------
+
+- Fixed context initialization fix. (#3)
+
+
 v3.0.1
 ======
 
 Rely on PEP 420 for namespace package.
 
 v3.0.0
 ======
```

### Comparing `jaraco.crypto-3.0.1/LICENSE` & `jaraco.crypto-3.1.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.crypto-3.0.1/PKG-INFO` & `jaraco.crypto-3.1.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,38 @@
-Metadata-Version: 2.1
-Name: jaraco.crypto
-Version: 3.0.1
-Summary: Cryptography support by jaraco
-Home-page: https://github.com/jaraco/jaraco.crypto
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/pypi/v/jaraco.crypto.svg
-           :target: `PyPI link`_
-        
-        .. image:: https://img.shields.io/pypi/pyversions/jaraco.crypto.svg
-           :target: `PyPI link`_
-        
-        .. _PyPI link: https://pypi.org/project/jaraco.crypto
-        
-        .. image:: https://github.com/jaraco/jaraco.crypto/workflows/tests/badge.svg
-           :target: https://github.com/jaraco/jaraco.crypto/actions?query=workflow%3A%22tests%22
-           :alt: tests
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-           :alt: Code style: Black
-        
-        .. image:: https://readthedocs.org/projects/jaracocrypto/badge/?version=latest
-           :target: https://jaracocrypto.readthedocs.io/en/latest/?badge=latest
-        
-        A set of cryptographic routines and utilities
-        implemented in pure Python.
-        
-        ================
-        Acknowledgements
-        ================
-        
-        Many of the ideas and much of the code has been adapted from or inspired by
-        several other projects, including:
-        
-        - The code repository was originally a fork of the `ctypescrypto project
-          <http://code.google.com/p/ctypescrypto/>`_. The code history includes the
-          full history of the ancestral project.
-        - The blowfish code was adapted from a module contributed to the community
-          by Michael Gilfix.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Provides-Extra: testing
-Provides-Extra: docs
+.. image:: https://img.shields.io/pypi/v/jaraco.crypto.svg
+   :target: https://pypi.org/project/jaraco.crypto
+
+.. image:: https://img.shields.io/pypi/pyversions/jaraco.crypto.svg
+
+.. image:: https://github.com/jaraco/jaraco.crypto/workflows/tests/badge.svg
+   :target: https://github.com/jaraco/jaraco.crypto/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: Black
+
+.. image:: https://readthedocs.org/projects/jaracocrypto/badge/?version=latest
+   :target: https://jaracocrypto.readthedocs.io/en/latest/?badge=latest
+
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
+   :target: https://blog.jaraco.com/skeleton
+
+A set of cryptographic routines and utilities
+implemented in pure Python.
+
+================
+Acknowledgements
+================
+
+Many of the ideas and much of the code has been adapted from or inspired by
+several other projects, including:
+
+- The code repository was originally a fork of the `ctypescrypto project
+  <http://code.google.com/p/ctypescrypto/>`_. The code history includes the
+  full history of the ancestral project.
+- The blowfish code was adapted from a module contributed to the community
+  by Michael Gilfix.
```

### Comparing `jaraco.crypto-3.0.1/certutil.py` & `jaraco.crypto-3.1.0/certutil.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from win32com.client import gencache, Dispatch
-import win32com.client
-
-clsid = '884e2049-217d-11da-b2a4-000e7bbb2b09'
-gencache.EnsureModule('{%s}' % clsid, 0, 1, 0)
-
-class_factory = Dispatch("X509Enrollment.CX509EnrollmentWebClassFactory")
-enrollment = class_factory.CreateObject("X509Enrollment.CX509Enrollment")
-pkcs10_request = class_factory.CreateObject(
-    "X509Enrollment.CX509CertificateRequestPkcs10"
-)
-private_key = class_factory.CreateObject("X509Enrollment.CX509privateKey")
-distinguished_name = class_factory.CreateObject("X509Enrollment.CX500DistinguishedName")
-
-
-def generate_request():
-    generate_key(length=2048)
-
-    CONTEXT_USER = 1
-    CONEXT_MACHINE = 2
-    XCN_CERT_NAME_STR_NONE = 0
-
-    hresult = pkcs10_request.InitializeFromPrivateKey(CONTEXT_USER, private_key, "")
-    name = 'CN=StartCom Free Certificate Member'
-    distinguished_name.Encode(name, XCN_CERT_NAME_STR_NONE)
-    pkcs10_request.Subject = distinguished_name
-
-
-def generate_key(length):
-    key = private_key
-
-    XCN_NCRYPT_ALLOW_EXPORT_FLAG = 1
-    XCN_NCRYPT_UI_NO_PROTECTION_FLAG = 0
-    XCN_NCRYPT_UI_PROTECT_KEY_FLAG = 1
-
-    key.ProviderName = "Microsoft Enhanced RSA and AES Cryptographic Provider"
-    key.ProviderType = "24"
-    key.KeySpec = "1"
-    key.KeyProtection = XCN_NCRYPT_UI_NO_PROTECTION_FLAG
-    key.ExportPolicy = XCN_NCRYPT_ALLOW_EXPORT_FLAG
-    key.Length = length
-
-
-generate_request()
-enrollment.InitializeFromRequest(pkcs10_request)
-print 'Request'
-print enrollment.createRequest(1)
+from win32com.client import gencache, Dispatch
+import win32com.client
+
+clsid = '884e2049-217d-11da-b2a4-000e7bbb2b09'
+gencache.EnsureModule('{%s}' % clsid, 0, 1, 0)
+
+class_factory = Dispatch("X509Enrollment.CX509EnrollmentWebClassFactory")
+enrollment = class_factory.CreateObject("X509Enrollment.CX509Enrollment")
+pkcs10_request = class_factory.CreateObject(
+    "X509Enrollment.CX509CertificateRequestPkcs10"
+)
+private_key = class_factory.CreateObject("X509Enrollment.CX509privateKey")
+distinguished_name = class_factory.CreateObject("X509Enrollment.CX500DistinguishedName")
+
+
+def generate_request():
+    generate_key(length=2048)
+
+    CONTEXT_USER = 1
+    CONEXT_MACHINE = 2
+    XCN_CERT_NAME_STR_NONE = 0
+
+    hresult = pkcs10_request.InitializeFromPrivateKey(CONTEXT_USER, private_key, "")
+    name = 'CN=StartCom Free Certificate Member'
+    distinguished_name.Encode(name, XCN_CERT_NAME_STR_NONE)
+    pkcs10_request.Subject = distinguished_name
+
+
+def generate_key(length):
+    key = private_key
+
+    XCN_NCRYPT_ALLOW_EXPORT_FLAG = 1
+    XCN_NCRYPT_UI_NO_PROTECTION_FLAG = 0
+    XCN_NCRYPT_UI_PROTECT_KEY_FLAG = 1
+
+    key.ProviderName = "Microsoft Enhanced RSA and AES Cryptographic Provider"
+    key.ProviderType = "24"
+    key.KeySpec = "1"
+    key.KeyProtection = XCN_NCRYPT_UI_NO_PROTECTION_FLAG
+    key.ExportPolicy = XCN_NCRYPT_ALLOW_EXPORT_FLAG
+    key.Length = length
+
+
+generate_request()
+enrollment.InitializeFromRequest(pkcs10_request)
+print('Request')
+print(enrollment.createRequest(1))
```

### Comparing `jaraco.crypto-3.0.1/docs/conf.py` & `jaraco.crypto-3.1.0/docs/conf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,47 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
                 pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
-                url='https://www.python.org/dev/peps/pep-{pep_number:0>4}/',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
+
+# Be strict about any broken references
+nitpicky = True
+nitpick_ignore = []
+
+# Include Python intersphinx mapping to prevent failures
+# jaraco/skeleton#51
+extensions += ['sphinx.ext.intersphinx']
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+}
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
+
+nitpick_ignore = [
+    ('py:class', '_ctypes.Structure'),
+]
```

### Comparing `jaraco.crypto-3.0.1/docs/index.rst` & `jaraco.crypto-3.1.0/docs/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Welcome to |project| documentation!
 ===================================
 
+.. sidebar-links::
+   :home:
+   :pypi:
+
 .. toctree::
    :maxdepth: 1
 
    history
 
 
 .. automodule:: jaraco.crypto.blowfish
```

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/blowfish.py` & `jaraco.crypto-3.1.0/jaraco/crypto/blowfish.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,20 +90,19 @@
 True
 
 """
 
 import struct
 import types
 
-import six
 
 __author__ = "Michael Gilfix <mgilfix@eecs.tufts.edu>"
 
 
-long = six.integer_types[0]
+long = (int,)[0]
 
 
 class Blowfish:
 
     """Blowfish encryption Scheme
 
     This class implements the encryption and decryption
@@ -163,15 +162,14 @@
     ENCRYPT = 0
     DECRYPT = 1
 
     # For the __round_func
     modulus = long(2) ** 32
 
     def __init__(self, key):
-
         if not key or len(key) < 8 or len(key) > 56:
             raise RuntimeError(
                 "Attempted to initialize Blowfish cipher with "
                 "key of invalid length: %s" % len(key)
             )
 
         self.p_boxes = [
```

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/cert.py` & `jaraco.crypto-3.1.0/jaraco/crypto/cert.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import ctypes
 
+from .support import find_library
+
 
 class Stack(ctypes.Structure):
     _fields_ = [
         ('num', ctypes.c_int),
         ('data', ctypes.POINTER(ctypes.c_char_p)),
         ('sorted', ctypes.c_int),
         ('num_alloc', ctypes.c_int),
@@ -37,42 +39,44 @@
         ('ex_data', CRYPTO_EX_DATA),
     ]
 
 
 FILETYPE_PEM = 1
 FILETYPE_ASN1 = 2
 
-libeay32 = ctypes.windll.libeay32
-libeay32.BN_bn2hex.restype = ctypes.c_char_p
+lib = find_library('libeay32') or find_library('libssl')
+assert lib, "Couldn't find OpenSSL"
+
+lib.BN_bn2hex.restype = ctypes.c_char_p
 
 
 class X509(ctypes.Structure):
     _fields_ = []
 
     def get_serial_number(self):
-        asn1_i = libeay32.X509_get_serialNumber(ctypes.byref(self))
-        bignum = libeay32.ASN1_INTEGER_to_BN(asn1_i, None)
+        asn1_i = lib.X509_get_serialNumber(ctypes.byref(self))
+        bignum = lib.ASN1_INTEGER_to_BN(asn1_i, None)
         try:
-            hex = libeay32.BN_bn2hex(bignum)
+            hex = lib.BN_bn2hex(bignum)
             result = int(hex, 16)
         finally:
-            libeay32.BN_free(bignum)
+            lib.BN_free(bignum)
         return result
 
 
 def load_certificate(type, data):
-    bio = libeay32.BIO_new_mem_buf(data, len(data))
+    bio = lib.BIO_new_mem_buf(data, len(data))
 
     try:
         if type == FILETYPE_PEM:
-            cert = libeay32.PEM_read_bio_X509(bio, None, None, None)
+            cert = lib.PEM_read_bio_X509(bio, None, None, None)
         else:
             raise ValueError("Unsupported type")
     finally:
-        libeay32.BIO_free(bio)
+        lib.BIO_free(bio)
     if not cert:
         raise Exception("Exception loading cert")
     return ctypes.cast(cert, ctypes.POINTER(X509)).contents
 
 
 if __name__ == '__main__':
     with open('server.pem', 'rb') as certfile:
```

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/cipher.py` & `jaraco.crypto-3.1.0/jaraco/crypto/cipher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import ctypes
 
-import six
 
 from . import evp
 
 CIPHER_ALGORITHMS = ("DES", "DES-EDE3", "BF", "AES-128", "AES-192", "AES-256")
 CIPHER_MODES = ("CBC", "CFB", "OFB", "ECB")
 
 
@@ -40,14 +39,20 @@
 evp.get_cipherbyname.restype = ctypes.POINTER(CipherType)  # type: ignore
 
 
 class Cipher(ctypes.Structure):
     _fields_ = evp._cipher_context_fields
     finalized = False
 
+    def __new__(cls, *a, **kw):
+        return evp.lib.EVP_CIPHER_CTX_new().contents
+
+    def __del__(self):
+        evp.lib.EVP_CIPHER_CTX_free(self)
+
     def __init__(self, type, key, iv, encrypt=True):
         key = key.encode('ascii')
         iv = iv.encode('ascii')
         engine = None
         type = self.interpret_type(type)
         res = evp.CipherInit_ex(self, type, engine, key, iv, encrypt)
         if res == 0:
@@ -77,15 +82,15 @@
         written may be anything from zero bytes to
         (inl + cipher_block_size - 1) so outl should
         contain sufficient room. The actual number of
         bytes written is placed in outl.
         """
         if self.finalized:
             raise CipherError("No updates allowed")
-        if isinstance(data, six.text_type):
+        if isinstance(data, str):
             data = data.encode()
         out = ctypes.create_string_buffer(len(data) + evp.MAX_BLOCK_LENGTH - 1)
         out_len = ctypes.c_int()
 
         res = evp.CipherUpdate(self, out, out_len, data, len(data))
         if res != 1:
             raise CipherError("Error updating cipher")
@@ -129,7 +134,13 @@
 ) = evp.CipherInit_ex.argtypes = _init_args  # type: ignore
 evp.EncryptUpdate.argtypes = (  # type: ignore
     evp.DecryptUpdate.argtypes  # type: ignore
 ) = evp.CipherUpdate.argtypes = _update_args  # type: ignore
 evp.EncryptFinal_ex.argtypes = (  # type: ignore
     evp.DecryptFinal_ex.argtypes  # type: ignore
 ) = evp.CipherFinal_ex.argtypes = _final_args  # type: ignore
+
+evp.lib.EVP_CIPHER_CTX_new.argtypes = None
+evp.lib.EVP_CIPHER_CTX_new.restype = ctypes.POINTER(Cipher)
+
+evp.lib.EVP_CIPHER_CTX_free.argtypes = (ctypes.POINTER(Cipher),)
+evp.lib.EVP_CIPHER_CTX_free.restype = None
```

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/digest.py` & `jaraco.crypto-3.1.0/jaraco/crypto/digest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import ctypes
 
-import six
 
 from . import evp
 
 
 class DigestError(Exception):
     pass
 
@@ -20,24 +19,30 @@
         return res.contents
 
 
 class Digest(ctypes.Structure):
     _fields_ = evp._digest_context_fields
     finalized = False
 
+    def __new__(cls, *a, **kw):
+        return evp.lib.EVP_MD_CTX_new().contents
+
+    def __del__(self):
+        evp.lib.EVP_MD_CTX_free(self)
+
     def __init__(self, digest_type):
         self.digest_type = digest_type
         result = evp.DigestInit_ex(self, digest_type, None)
         if result == 0:
             raise DigestError("Unable to initialize digest")
 
     def update(self, data):
         if self.finalized:
             raise DigestError("Digest is finalized; no updates allowed")
-        if isinstance(data, six.text_type):
+        if isinstance(data, str):
             data = data.encode()
         result = evp.DigestUpdate(self, data, len(data))
         if result != 1:
             raise DigestError("Unable to update digest")
 
     def digest(self, data=None):
         if data is not None:
```

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/evp.py` & `jaraco.crypto-3.1.0/jaraco/crypto/evp.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     ('update', c_void_p),
     ('final', c_void_p),
     ('copy', c_void_p),
     ('cleanup', c_void_p),
     ('sign', c_void_p),
     ('verify', c_void_p),
     ('required_pkey_type', c_int * 5),
-    ('block size', c_int),
+    ('block_size', c_int),
     ('ctx_size', c_int),
     ('md_ctrl', c_void_p),
 ]
 
 _digest_context_fields = [
     ('p_type', c_void_p),  # POINTER(DigestType)
     ('engine', c_void_p),  # todo, POINTER(ENGINE)
@@ -84,14 +84,18 @@
     DigestUpdate.restype = c_int
     DigestFinal_ex.argtypes = (
         POINTER(Digest),
         c_char_p,
         POINTER(c_uint),
     )
     DigestFinal_ex.restype = c_int
+    lib.EVP_MD_CTX_new.restype = POINTER(Digest)
+    lib.EVP_MD_CTX_new.argtypes = None
+    lib.EVP_MD_CTX_free.restype = None
+    lib.EVP_MD_CTX_free.argtypes = (POINTER(Digest),)
 
 
 _reg('get_cipherbyname')
 get_cipherbyname.argtypes = (c_char_p,)  # type: ignore
 
 _cipher_fields = [
     ('nid', c_int),
```

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/itsdangerous/compat.py` & `jaraco.crypto-3.1.0/jaraco/crypto/itsdangerous/compat.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Compatibility shim for timestamp compatibility between
 itsdangerous 0.24 and 1.x. See `itsdangerous 120
 <https://github.com/pallets/itsdangerous/issues/120>`_
 for motivation and details.
 """
 
 import time
-import sys
 import datetime
 
 import itsdangerous
 
 
 class EpochOffsetSigner(itsdangerous.TimestampSigner):
     """
@@ -23,15 +22,15 @@
     except AttributeError:
         EPOCH = 1293840000.0
 
     def get_timestamp(self):
         return int(time.time() - self.EPOCH)
 
     def timestamp_to_datetime(self, ts):
-        return super(EpochOffsetSigner, self).timestamp_to_datetime(ts + self.EPOCH)
+        return super().timestamp_to_datetime(ts + self.EPOCH)
 
 
 def unsign(signer, blob, **kwargs):
     """
     Prepare to freeze time; create frozen decorator
 
     >>> from freezegun import freeze_time
@@ -71,11 +70,7 @@
     """
     try:
         return signer.unsign(blob, **kwargs)
     except itsdangerous.exc.SignatureExpired:
         compat_signer = EpochOffsetSigner(None)
         vars(compat_signer).update(vars(signer))
         return compat_signer.unsign(blob, **kwargs)
-
-
-if sys.version_info < (3,):
-    unsign.__doc__ = unsign.__doc__.replace('itsdangerous.exc.', '')
```

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/rand.py` & `jaraco.crypto-3.1.0/jaraco/crypto/rand.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import ctypes
 
-import six
 
 from .evp import lib
 
 
 class RandError(Exception):
     pass
 
@@ -33,15 +32,15 @@
 
 
 lib.RAND_seed.argtypes = ctypes.c_char_p, ctypes.c_int
 lib.RAND_add.argtypes = ctypes.c_char_p, ctypes.c_int, ctypes.c_double
 
 
 def seed(data, entropy=None):
-    if not isinstance(data, six.string_types):
+    if not isinstance(data, str):
         raise TypeError("data must be a string")
     params = [data, len(data)]
     if entropy:
         func = lib.RAND_add
         params.append(entropy)
     else:
         func = lib.RAND_seed
```

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/support.py` & `jaraco.crypto-3.1.0/jaraco/crypto/support.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import ctypes
 import os
 import platform
 import subprocess
 
-from six.moves import filter
-
 
 def find_lib_Linux(lib_name):
     try:
         lines = subprocess.check_output(['ldconfig', '-p'], text=True)
     except TypeError:
-        lines = subprocess.check_output(['ldconfig', '-p'], universal_newlines=True)
+        lines = subprocess.check_output(['ldconfig', '-p'], text=True)
 
     for line in lines.splitlines():
         lib, _, rest = line.strip().partition(' ')
         _, _, path = rest.rpartition(' ')
         found_name, _, _ = lib.partition('.')
         if lib_name == found_name:
             return path
@@ -31,14 +29,15 @@
     Given a name like libeay32, find the best match.
     """
     # todo, allow the target environment to customize this behavior
     roots = [
         'c:\\Program Files\\OpenSSL\\',
         '\\OpenSSL-Win64',
         '/usr/local/opt/openssl/lib/',
+        '/opt/homebrew/lib/',
     ]
     ext = (
         '.dll'
         if platform.system() == 'Windows'
         else '.dylib'
         if platform.system() == 'Darwin'
         else '.so'
```

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/tests/test_cipher.py` & `jaraco.crypto-3.1.0/jaraco/crypto/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/tests/test_digest.py` & `jaraco.crypto-3.1.0/jaraco/crypto/tests/test_digest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import binascii
 
-import py.test
+import pytest
 
 from jaraco.crypto import digest
 
 
 def test_load_valid_digest_type_by_name():
     digest.DigestType.from_name('SHA256')
 
 
 def test_load_invalid_digest_type_by_name():
     # dne is Does Not Exist
-    py.test.raises(digest.DigestError, digest.DigestType.from_name, 'sha-dne')
+    pytest.raises(digest.DigestError, digest.DigestType.from_name, 'sha-dne')
 
 
 def test_digest():
     digest_type = digest.DigestType.from_name('SHA512')
     sha512 = digest.Digest(digest_type)
     sha512.update("test")
     assert not sha512.finalized
```

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/tests/test_rand.py` & `jaraco.crypto-3.1.0/jaraco/crypto/tests/test_rand.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import py.test
+import pytest
 
 from jaraco.crypto import rand
 
 
 def test_bytes():
     bytes = rand.bytes(100)
     assert len(bytes) == 100
@@ -12,15 +12,15 @@
 def test_pseudo_bytes():
     bytes = rand.pseudo_bytes(100)
     assert len(bytes) == 100
     assert bytes != rand.pseudo_bytes(100)
 
 
 def test_seed():
-    py.test.skip("This fails, why?")
+    pytest.skip("This fails, why?")
     seed = 'bunch of bytes' * 1000
     rand.cleanup()
     rand.seed(seed)
     bytes1 = rand.pseudo_bytes(100)
     rand.cleanup()
     rand.seed(seed)
     bytes2 = rand.pseudo_bytes(100)
```

### Comparing `jaraco.crypto-3.0.1/jaraco/crypto/tests/test_threads.py` & `jaraco.crypto-3.1.0/jaraco/crypto/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.0.1/jaraco.crypto.egg-info/SOURCES.txt` & `jaraco.crypto-3.1.0/jaraco.crypto.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
-.readthedocs.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
 certutil.py
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
-setup.py
-skeleton.md
+towncrier.toml
 tox.ini
-.github/workflows/automerge.yml
+.github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 jaraco.crypto.egg-info/PKG-INFO
 jaraco.crypto.egg-info/SOURCES.txt
 jaraco.crypto.egg-info/dependency_links.txt
```

### Comparing `jaraco.crypto-3.0.1/setup.cfg` & `jaraco.crypto-3.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 [metadata]
-license_files = 
-	LICENSE
 name = jaraco.crypto
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
 description = Cryptography support by jaraco
 long_description = file:README.rst
 url = https://github.com/jaraco/jaraco.crypto
 classifiers = 
@@ -13,41 +11,44 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
-setup_requires = setuptools_scm[toml] >= 3.4.1
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
-	pytest >= 4.6
+	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
-	pytest-black >= 0.3.7; python_implementation != "PyPy" and python_version < "3.10"
+	pytest-black >= 0.3.7; \
+	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy; python_implementation != "PyPy" and python_version < "3.10"
-	pytest-enabler >= 1.0.1
+	pytest-mypy >= 0.9.1; \
+	python_implementation != "PyPy"
+	pytest-enabler >= 2.2
+	pytest-ruff
 	
 	itsdangerous
 	freezegun
 docs = 
-	sphinx
-	jaraco.packaging >= 8.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

