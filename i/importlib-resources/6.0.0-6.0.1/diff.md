# Comparing `tmp/importlib_resources-6.0.0.tar.gz` & `tmp/importlib_resources-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_resources-6.0.0.tar", last modified: Fri Jul  7 18:27:18 2023, max compression
+gzip compressed data, was "importlib_resources-6.0.1.tar", last modified: Mon Aug  7 05:09:22 2023, max compression
```

## Comparing `importlib_resources-6.0.0.tar` & `importlib_resources-6.0.1.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/docs/using.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/importlib_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/importlib_resources/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data01/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/binary.file
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data01/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/subdirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/subdirectory/binary.file
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/utf-16.file
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/utf-8.file
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data02/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data02/one/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/one/resource1.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.857378 importlib_resources-6.0.0/importlib_resources/tests/data02/subdirectory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data02/subdirectory/subsubdir/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/subdirectory/subsubdir/resource.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data02/two/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/two/resource2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/namespacedata01/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/namespacedata01/binary.file
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/namespacedata01/utf-16.file
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/namespacedata01/utf-8.file
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_compatibilty_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_resource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1417 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/update-zips.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/zipdata01/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/zipdata01/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/zipdata01/ziptestdata.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/zipdata02/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/zipdata02/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/zipdata02/ziptestdata.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/importlib_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-07 18:27:18.000000 importlib_resources-6.0.0/importlib_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-07 18:27:18.000000 importlib_resources-6.0.0/importlib_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:27:18.000000 importlib_resources-6.0.0/importlib_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-07 18:27:18.000000 importlib_resources-6.0.0/importlib_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 18:27:18.000000 importlib_resources-6.0.0/importlib_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.647300 importlib_resources-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.627300 importlib_resources-6.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.627300 importlib_resources-6.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-07 05:09:22.651300 importlib_resources-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.631300 importlib_resources-6.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/docs/using.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.635300 importlib_resources-6.0.1/importlib_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.643300 importlib_resources-6.0.1/importlib_resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.643300 importlib_resources-6.0.1/importlib_resources/tests/data01/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data01/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data01/binary.file
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.643300 importlib_resources-6.0.1/importlib_resources/tests/data01/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data01/subdirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data01/subdirectory/binary.file
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data01/utf-16.file
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data01/utf-8.file
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.643300 importlib_resources-6.0.1/importlib_resources/tests/data02/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data02/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.643300 importlib_resources-6.0.1/importlib_resources/tests/data02/one/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data02/one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data02/one/resource1.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.619300 importlib_resources-6.0.1/importlib_resources/tests/data02/subdirectory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.647300 importlib_resources-6.0.1/importlib_resources/tests/data02/subdirectory/subsubdir/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data02/subdirectory/subsubdir/resource.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.647300 importlib_resources-6.0.1/importlib_resources/tests/data02/two/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data02/two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/data02/two/resource2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.647300 importlib_resources-6.0.1/importlib_resources/tests/namespacedata01/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/namespacedata01/binary.file
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/namespacedata01/utf-16.file
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/namespacedata01/utf-8.file
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/test_compatibilty_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/test_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/test_resource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1417 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/update-zips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.647300 importlib_resources-6.0.1/importlib_resources/tests/zipdata01/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/zipdata01/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/zipdata01/ziptestdata.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.647300 importlib_resources-6.0.1/importlib_resources/tests/zipdata02/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/zipdata02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/importlib_resources/tests/zipdata02/ziptestdata.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 05:09:22.635300 importlib_resources-6.0.1/importlib_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-07 05:09:22.000000 importlib_resources-6.0.1/importlib_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-07 05:09:22.000000 importlib_resources-6.0.1/importlib_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 05:09:22.000000 importlib_resources-6.0.1/importlib_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-07 05:09:22.000000 importlib_resources-6.0.1/importlib_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 05:09:22.000000 importlib_resources-6.0.1/importlib_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-07 05:09:22.651300 importlib_resources-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-07 05:08:57.000000 importlib_resources-6.0.1/tox.ini
```

### Comparing `importlib_resources-6.0.0/.github/workflows/main.yml` & `importlib_resources-6.0.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/.gitignore` & `importlib_resources-6.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/NEWS.rst` & `importlib_resources-6.0.1/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v6.0.1
+======
+
+Bugfixes
+--------
+
+- Restored Apache license. (#285)
+
+
 v6.0.0
 ======
 
 Deprecations and Removals
 -------------------------
 
 - Removed legacy functions deprecated in 5.3. (#80)
```

### Comparing `importlib_resources-6.0.0/PKG-INFO` & `importlib_resources-6.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib_resources
-Version: 6.0.0
+Version: 6.0.1
 Summary: Read resources from Python packages
 Home-page: https://github.com/python/importlib_resources
 Author: Barry Warsaw
 Author-email: barry@python.org
 Project-URL: Documentation, https://importlib-resources.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -82,14 +82,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-importlib-resources?utm_source=pypi-importlib-resources&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `importlib_resources-6.0.0/README.rst` & `importlib_resources-6.0.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-importlib-resources?utm_source=pypi-importlib-resources&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `importlib_resources-6.0.0/docs/conf.py` & `importlib_resources-6.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/docs/index.rst` & `importlib_resources-6.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/docs/migration.rst` & `importlib_resources-6.0.1/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/docs/using.rst` & `importlib_resources-6.0.1/docs/using.rst`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/_adapters.py` & `importlib_resources-6.0.1/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/_common.py` & `importlib_resources-6.0.1/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/_compat.py` & `importlib_resources-6.0.1/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/_itertools.py` & `importlib_resources-6.0.1/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/abc.py` & `importlib_resources-6.0.1/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/readers.py` & `importlib_resources-6.0.1/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/simple.py` & `importlib_resources-6.0.1/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/_compat.py` & `importlib_resources-6.0.1/importlib_resources/tests/_compat.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/_path.py` & `importlib_resources-6.0.1/importlib_resources/tests/_path.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/test_compatibilty_files.py` & `importlib_resources-6.0.1/importlib_resources/tests/test_compatibilty_files.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/test_contents.py` & `importlib_resources-6.0.1/importlib_resources/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/test_custom.py` & `importlib_resources-6.0.1/importlib_resources/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/test_files.py` & `importlib_resources-6.0.1/importlib_resources/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/test_open.py` & `importlib_resources-6.0.1/importlib_resources/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/test_path.py` & `importlib_resources-6.0.1/importlib_resources/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/test_read.py` & `importlib_resources-6.0.1/importlib_resources/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/test_reader.py` & `importlib_resources-6.0.1/importlib_resources/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/test_resource.py` & `importlib_resources-6.0.1/importlib_resources/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/update-zips.py` & `importlib_resources-6.0.1/importlib_resources/tests/update-zips.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/util.py` & `importlib_resources-6.0.1/importlib_resources/tests/util.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/zipdata01/ziptestdata.zip` & `importlib_resources-6.0.1/importlib_resources/tests/zipdata01/ziptestdata.zip`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources/tests/zipdata02/ziptestdata.zip` & `importlib_resources-6.0.1/importlib_resources/tests/zipdata02/ziptestdata.zip`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/importlib_resources.egg-info/PKG-INFO` & `importlib_resources-6.0.1/importlib_resources.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib-resources
-Version: 6.0.0
+Version: 6.0.1
 Summary: Read resources from Python packages
 Home-page: https://github.com/python/importlib_resources
 Author: Barry Warsaw
 Author-email: barry@python.org
 Project-URL: Documentation, https://importlib-resources.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -82,14 +82,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-importlib-resources?utm_source=pypi-importlib-resources&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `importlib_resources-6.0.0/importlib_resources.egg-info/SOURCES.txt` & `importlib_resources-6.0.1/importlib_resources.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE
 NEWS.rst
 README.rst
+SECURITY.md
 codecov.yml
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
 towncrier.toml
 tox.ini
```

### Comparing `importlib_resources-6.0.0/pytest.ini` & `importlib_resources-6.0.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/setup.cfg` & `importlib_resources-6.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `importlib_resources-6.0.0/tox.ini` & `importlib_resources-6.0.1/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-[tox]
-toxworkdir={env:TOX_WORK_DIR:.tox}
-
-
 [testenv]
 deps =
 setenv =
 	PYTHONWARNDEFAULTENCODING = 1
 commands =
 	pytest {posargs}
 usedevelop = True
```

