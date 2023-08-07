# Comparing `tmp/swh.perfecthash-1.0.0.tar.gz` & `tmp/swh.perfecthash-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.perfecthash-1.0.0.tar", last modified: Mon Aug  7 10:11:56 2023, max compression
+gzip compressed data, was "swh.perfecthash-1.0.0rc1.tar", last modified: Fri Jun 23 16:27:25 2023, max compression
```

## Comparing `swh.perfecthash-1.0.0.tar` & `swh.perfecthash-1.0.0rc1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:56.593915 swh.perfecthash-1.0.0/
--rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      279 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      147 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1096 2023-08-07 10:11:56.593915 swh.perfecthash-1.0.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      172 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/README.rst
--rwxr-xr-x   0 jenkins    (115) docker     (999)      350 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/build_cmph.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      733 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:56.589915 swh.perfecthash-1.0.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:56.593915 swh.perfecthash-1.0.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:56.593915 swh.perfecthash-1.0.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)     3696 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/docs/benchmarks.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      628 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/docs/format.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      470 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      317 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      487 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       66 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        7 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      231 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-08-07 10:11:56.593915 swh.perfecthash-1.0.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2393 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:56.593915 swh.perfecthash-1.0.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:56.593915 swh.perfecthash-1.0.0/swh/perfecthash/
--rw-r--r--   0 jenkins    (115) docker     (999)       19 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/swh/perfecthash/.clang-format
--rw-r--r--   0 jenkins    (115) docker     (999)      552 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/swh/perfecthash/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     3583 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/swh/perfecthash/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1751 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/swh/perfecthash/build.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13776 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/swh/perfecthash/hash.c
--rw-r--r--   0 jenkins    (115) docker     (999)     1618 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/swh/perfecthash/hash.h
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/swh/perfecthash/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     5635 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/swh/perfecthash/test_hash.cpp
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:56.593915 swh.perfecthash-1.0.0/swh/perfecthash/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/swh/perfecthash/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4654 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/swh/perfecthash/tests/test_hash.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-08-07 10:11:56.593915 swh.perfecthash-1.0.0/swh.perfecthash.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1096 2023-08-07 10:11:56.000000 swh.perfecthash-1.0.0/swh.perfecthash.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      922 2023-08-07 10:11:56.000000 swh.perfecthash-1.0.0/swh.perfecthash.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-08-07 10:11:56.000000 swh.perfecthash-1.0.0/swh.perfecthash.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       23 2023-08-07 10:11:56.000000 swh.perfecthash-1.0.0/swh.perfecthash.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-08-07 10:11:56.000000 swh.perfecthash-1.0.0/swh.perfecthash.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1623 2023-08-07 10:11:50.000000 swh.perfecthash-1.0.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.581641 swh.perfecthash-1.0.0rc1/
+-rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      279 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      147 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1099 2023-06-23 16:27:25.581641 swh.perfecthash-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      172 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/README.rst
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      350 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/build_cmph.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      733 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)     3696 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/benchmarks.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      628 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/format.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      470 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      317 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      487 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       66 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        7 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      231 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-23 16:27:25.581641 swh.perfecthash-1.0.0rc1/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2393 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/swh/perfecthash/
+-rw-r--r--   0 jenkins    (115) docker     (999)       19 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/.clang-format
+-rw-r--r--   0 jenkins    (115) docker     (999)      552 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     3583 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1751 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/build.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13776 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/hash.c
+-rw-r--r--   0 jenkins    (115) docker     (999)     1618 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/hash.h
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     5635 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/test_hash.cpp
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/swh/perfecthash/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4654 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/tests/test_hash.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1099 2023-06-23 16:27:25.000000 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      922 2023-06-23 16:27:25.000000 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-23 16:27:25.000000 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       23 2023-06-23 16:27:25.000000 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-23 16:27:25.000000 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1623 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/tox.ini
```

### Comparing `swh.perfecthash-1.0.0/.pre-commit-config.yaml` & `swh.perfecthash-1.0.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/CODE_OF_CONDUCT.md` & `swh.perfecthash-1.0.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/LICENSE` & `swh.perfecthash-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/PKG-INFO` & `swh.perfecthash-1.0.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.perfecthash
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Software Heritage Perfect Hash
 Home-page: https://forge.softwareheritage.org/source/swh-perfecthash
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-perfecthash
```

### Comparing `swh.perfecthash-1.0.0/conftest.py` & `swh.perfecthash-1.0.0rc1/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/docs/benchmarks.rst` & `swh.perfecthash-1.0.0rc1/docs/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/docs/format.rst` & `swh.perfecthash-1.0.0rc1/docs/format.rst`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/setup.py` & `swh.perfecthash-1.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/swh/perfecthash/Makefile` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/Makefile`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/swh/perfecthash/__init__.py` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/swh/perfecthash/build.py` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/build.py`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/swh/perfecthash/hash.c` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/hash.c`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/swh/perfecthash/hash.h` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/hash.h`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/swh/perfecthash/test_hash.cpp` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/test_hash.cpp`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/swh/perfecthash/tests/test_hash.py` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/swh.perfecthash.egg-info/PKG-INFO` & `swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.perfecthash
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Software Heritage Perfect Hash
 Home-page: https://forge.softwareheritage.org/source/swh-perfecthash
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-perfecthash
```

### Comparing `swh.perfecthash-1.0.0/swh.perfecthash.egg-info/SOURCES.txt` & `swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-1.0.0/tox.ini` & `swh.perfecthash-1.0.0rc1/tox.ini`

 * *Files identical despite different names*

