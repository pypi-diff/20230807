# Comparing `tmp/nspektr-0.4.0.tar.gz` & `tmp/nspektr-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nspektr-0.4.0.tar", last modified: Thu Jun  9 20:33:37 2022, max compression
+gzip compressed data, was "nspektr-0.5.0.tar", last modified: Mon Aug  7 00:34:22 2023, max compression
```

## Comparing `nspektr-0.4.0.tar` & `nspektr-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 20:33:37.041132 nspektr-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-06-09 20:33:11.000000 nspektr-0.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-06-09 20:33:11.000000 nspektr-0.4.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-06-09 20:33:11.000000 nspektr-0.4.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 20:33:37.041132 nspektr-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-06-09 20:33:11.000000 nspektr-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 20:33:37.041132 nspektr-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-06-09 20:33:11.000000 nspektr-0.4.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-09 20:33:11.000000 nspektr-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-09 20:33:11.000000 nspektr-0.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-06-09 20:33:11.000000 nspektr-0.4.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-06-09 20:33:11.000000 nspektr-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1911 2022-06-09 20:33:37.045132 nspektr-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-06-09 20:33:11.000000 nspektr-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 20:33:37.041132 nspektr-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-06-09 20:33:11.000000 nspektr-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-09 20:33:11.000000 nspektr-0.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-06-09 20:33:11.000000 nspektr-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-09 20:33:11.000000 nspektr-0.4.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 20:33:37.041132 nspektr-0.4.0/nspektr/
--rw-r--r--   0 runner    (1001) docker     (121)     3952 2022-06-09 20:33:11.000000 nspektr-0.4.0/nspektr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-06-09 20:33:11.000000 nspektr-0.4.0/nspektr/_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 20:33:37.041132 nspektr-0.4.0/nspektr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1911 2022-06-09 20:33:36.000000 nspektr-0.4.0/nspektr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-06-09 20:33:37.000000 nspektr-0.4.0/nspektr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 20:33:36.000000 nspektr-0.4.0/nspektr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-06-09 20:33:36.000000 nspektr-0.4.0/nspektr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-09 20:33:36.000000 nspektr-0.4.0/nspektr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-06-09 20:33:11.000000 nspektr-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-06-09 20:33:11.000000 nspektr-0.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-06-09 20:33:37.045132 nspektr-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-06-09 20:33:11.000000 nspektr-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:34:22.436790 nspektr-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-07 00:33:54.000000 nspektr-0.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-07 00:33:54.000000 nspektr-0.5.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:34:22.436790 nspektr-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-07 00:33:54.000000 nspektr-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:34:22.436790 nspektr-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-07 00:33:54.000000 nspektr-0.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-07 00:33:54.000000 nspektr-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-07 00:33:54.000000 nspektr-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-07 00:33:54.000000 nspektr-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-07 00:33:54.000000 nspektr-0.5.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-07 00:34:22.436790 nspektr-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-07 00:33:54.000000 nspektr-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:34:22.436790 nspektr-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-07 00:33:54.000000 nspektr-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 00:33:54.000000 nspektr-0.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-07 00:33:54.000000 nspektr-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 00:33:54.000000 nspektr-0.5.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:34:22.436790 nspektr-0.5.0/nspektr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-08-07 00:33:54.000000 nspektr-0.5.0/nspektr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-07 00:33:54.000000 nspektr-0.5.0/nspektr/_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:34:22.436790 nspektr-0.5.0/nspektr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-07 00:34:22.000000 nspektr-0.5.0/nspektr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-07 00:34:22.000000 nspektr-0.5.0/nspektr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:34:22.000000 nspektr-0.5.0/nspektr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-07 00:34:22.000000 nspektr-0.5.0/nspektr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 00:34:22.000000 nspektr-0.5.0/nspektr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 00:33:54.000000 nspektr-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-07 00:33:54.000000 nspektr-0.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 00:34:22.436790 nspektr-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 00:33:54.000000 nspektr-0.5.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-07 00:33:54.000000 nspektr-0.5.0/tox.ini
```

### Comparing `nspektr-0.4.0/CHANGES.rst` & `nspektr-0.5.0/NEWS.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v0.5.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v0.4.0
 ======
 
 #1: doctest on ``check()`` uses ``pytest`` instead of ``pip`` for
 broader compatibility.
 
 v0.3.0
```

### Comparing `nspektr-0.4.0/LICENSE` & `nspektr-0.5.0/LICENSE`

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

### Comparing `nspektr-0.4.0/PKG-INFO` & `nspektr-0.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: nspektr
-Version: 0.4.0
+Version: 0.5.0
 Summary: package inspector
 Home-page: https://github.com/jaraco/nspektr
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/nspektr.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/nspektr
 
 .. image:: https://img.shields.io/pypi/pyversions/nspektr.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/nspektr
 
 .. image:: https://github.com/jaraco/nspektr/workflows/tests/badge.svg
    :target: https://github.com/jaraco/nspektr/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/nspektr/badge/?version=latest
    :target: https://nspektr.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 
 nspektr is a distribution package dependency inspector.
 
 It combines functionality from ``importlib.metadata`` and ``packaging``
 to provide routines to resolve and validate dependencies for a package
```

### Comparing `nspektr-0.4.0/README.rst` & `nspektr-0.5.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 .. image:: https://img.shields.io/pypi/v/nspektr.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/nspektr
 
 .. image:: https://img.shields.io/pypi/pyversions/nspektr.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/nspektr
 
 .. image:: https://github.com/jaraco/nspektr/workflows/tests/badge.svg
    :target: https://github.com/jaraco/nspektr/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/nspektr/badge/?version=latest
    :target: https://nspektr.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 
 nspektr is a distribution package dependency inspector.
 
 It combines functionality from ``importlib.metadata`` and ``packaging``
 to provide routines to resolve and validate dependencies for a package
```

### Comparing `nspektr-0.4.0/docs/conf.py` & `nspektr-0.5.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
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
@@ -21,16 +24,26 @@
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
                 url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
 
-# Be strict about any broken references:
+# Be strict about any broken references
 nitpicky = True
+nitpick_ignore = []
 
 # Include Python intersphinx mapping to prevent failures
 # jaraco/skeleton#51
 extensions += ['sphinx.ext.intersphinx']
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
 }
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
+
+intersphinx_mapping.update(
+    packaging=('https://packaging.pypa.io/en/stable/', None),
+)
+
+nitpick_ignore.append(('py:class', 'importlib.metadata.Distribution'))
```

### Comparing `nspektr-0.4.0/nspektr/__init__.py` & `nspektr-0.5.0/nspektr/__init__.py`

 * *Files identical despite different names*

### Comparing `nspektr-0.4.0/nspektr/_compat.py` & `nspektr-0.5.0/nspektr/_compat.py`

 * *Files identical despite different names*

### Comparing `nspektr-0.4.0/nspektr.egg-info/PKG-INFO` & `nspektr-0.5.0/nspektr.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: nspektr
-Version: 0.4.0
+Version: 0.5.0
 Summary: package inspector
 Home-page: https://github.com/jaraco/nspektr
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/nspektr.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/nspektr
 
 .. image:: https://img.shields.io/pypi/pyversions/nspektr.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/nspektr
 
 .. image:: https://github.com/jaraco/nspektr/workflows/tests/badge.svg
    :target: https://github.com/jaraco/nspektr/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/nspektr/badge/?version=latest
    :target: https://nspektr.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 
 nspektr is a distribution package dependency inspector.
 
 It combines functionality from ``importlib.metadata`` and ``packaging``
 to provide routines to resolve and validate dependencies for a package
```

### Comparing `nspektr-0.4.0/setup.cfg` & `nspektr-0.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	jaraco.context
 	jaraco.functools
 	more_itertools
 	packaging
 	importlib_metadata>=3.6; python_version < "3.10"
 
@@ -30,25 +30,27 @@
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.0.1
+	pytest-enabler >= 2.2
+	pytest-ruff
 docs = 
-	sphinx
-	jaraco.packaging >= 9
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

