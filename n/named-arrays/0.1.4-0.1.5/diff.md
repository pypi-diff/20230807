# Comparing `tmp/named_arrays-0.1.4.tar.gz` & `tmp/named_arrays-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "named_arrays-0.1.4.tar", last modified: Wed Mar 15 01:22:04 2023, max compression
+gzip compressed data, was "named_arrays-0.1.5.tar", last modified: Mon Aug  7 03:07:20 2023, max compression
```

## Comparing `named_arrays-0.1.4.tar` & `named_arrays-0.1.5.tar`

### file list

```diff
@@ -1,67 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.548843 named_arrays-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.536843 named_arrays-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.540843 named_arrays-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-15 01:21:50.000000 named_arrays-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-03-15 01:21:50.000000 named_arrays-0.1.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-15 01:21:50.000000 named_arrays-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-15 01:21:50.000000 named_arrays-0.1.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-03-15 01:22:04.548843 named_arrays-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-03-15 01:21:50.000000 named_arrays-0.1.4/README.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-15 01:21:50.000000 named_arrays-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.540843 named_arrays-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-15 01:21:50.000000 named_arrays-0.1.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.540843 named_arrays-0.1.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 01:21:50.000000 named_arrays-0.1.4/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.540843 named_arrays-0.1.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-15 01:21:50.000000 named_arrays-0.1.4/docs/_templates/class_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-15 01:21:50.000000 named_arrays-0.1.4/docs/_templates/function_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-15 01:21:50.000000 named_arrays-0.1.4/docs/_templates/module_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-15 01:21:50.000000 named_arrays-0.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-15 01:21:50.000000 named_arrays-0.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-15 01:21:50.000000 named_arrays-0.1.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.540843 named_arrays-0.1.4/named_arrays/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_core_array_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_named_array_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.544843 named_arrays-0.1.4/named_arrays/_vectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_vectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.544843 named_arrays-0.1.4/named_arrays/_vectors/cartesian/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_vectors/cartesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_vectors/cartesian/cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_vectors/cartesian/cartesian_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.544843 named_arrays-0.1.4/named_arrays/_vectors/cartesian/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_vectors/cartesian/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_vectors/cartesian/tests/test_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_vectors/cartesian/tests/test_cartesian_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.544843 named_arrays-0.1.4/named_arrays/_vectors/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_vectors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20888 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_vectors/tests/test_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17823 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_vectors/vector_array_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/_vectors/vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    28362 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.544843 named_arrays-0.1.4/named_arrays/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18998 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/scalars/array_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    40500 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/scalars/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.544843 named_arrays-0.1.4/named_arrays/scalars/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/scalars/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44467 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/scalars/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.544843 named_arrays-0.1.4/named_arrays/scalars/uncertainties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/scalars/uncertainties/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.548843 named_arrays-0.1.4/named_arrays/scalars/uncertainties/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/scalars/uncertainties/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26513 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/scalars/uncertainties/tests/test_uncertainties.py
--rw-r--r--   0 runner    (1001) docker     (123)    20731 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/scalars/uncertainties/uncertainties.py
--rw-r--r--   0 runner    (1001) docker     (123)    18090 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/scalars/uncertainties/uncertainties_array_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.548843 named_arrays-0.1.4/named_arrays/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35437 2023-03-15 01:21:50.000000 named_arrays-0.1.4/named_arrays/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 01:22:04.544843 named_arrays-0.1.4/named_arrays.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-03-15 01:22:04.000000 named_arrays-0.1.4/named_arrays.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-15 01:22:04.000000 named_arrays-0.1.4/named_arrays.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 01:22:04.000000 named_arrays-0.1.4/named_arrays.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-15 01:22:04.000000 named_arrays-0.1.4/named_arrays.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-15 01:22:04.000000 named_arrays-0.1.4/named_arrays.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-15 01:21:50.000000 named_arrays-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-15 01:21:50.000000 named_arrays-0.1.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 01:22:04.548843 named_arrays-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.933718 named_arrays-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.917717 named_arrays-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.921717 named_arrays-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-07 03:07:06.000000 named_arrays-0.1.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-07 03:07:06.000000 named_arrays-0.1.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 03:07:06.000000 named_arrays-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-07 03:07:06.000000 named_arrays-0.1.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-08-07 03:07:20.933718 named_arrays-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-08-07 03:07:06.000000 named_arrays-0.1.5/README.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-08-07 03:07:06.000000 named_arrays-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.921717 named_arrays-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.921717 named_arrays-0.1.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.921717 named_arrays-0.1.5/docs/_static/favicon_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_static/favicon_io/about.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_static/favicon_io/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_static/favicon_io/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_static/favicon_io/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_static/favicon_io/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_static/favicon_io/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_static/favicon_io/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_static/favicon_io/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.921717 named_arrays-0.1.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_templates/class_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_templates/function_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/_templates/module_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-07 03:07:06.000000 named_arrays-0.1.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.925717 named_arrays-0.1.5/named_arrays/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34651 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_core_array_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.925717 named_arrays-0.1.5/named_arrays/_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_functions/function_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21194 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_functions/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.925717 named_arrays-0.1.5/named_arrays/_functions/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_functions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23362 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_functions/tests/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.925717 named_arrays-0.1.5/named_arrays/_matrices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.925717 named_arrays-0.1.5/named_arrays/_matrices/cartesian/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/cartesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/cartesian/matrices_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/cartesian/matrices_cartesian_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/cartesian/matrices_cartesian_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/cartesian/matrices_cartesian_nd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.925717 named_arrays-0.1.5/named_arrays/_matrices/cartesian/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/cartesian/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/cartesian/tests/test_matrices_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/cartesian/tests/test_matrices_cartesian_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/matrices_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/matrices_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/matrices_spectral_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.925717 named_arrays-0.1.5/named_arrays/_matrices/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_matrices/tests/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_named_array_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.929717 named_arrays-0.1.5/named_arrays/_scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/scalar_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/scalar_named_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37923 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/scalars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.929717 named_arrays-0.1.5/named_arrays/_scalars/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39228 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/tests/test_scalars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.929717 named_arrays-0.1.5/named_arrays/_scalars/uncertainties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/uncertainties/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.929717 named_arrays-0.1.5/named_arrays/_scalars/uncertainties/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/uncertainties/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33896 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/uncertainties/tests/test_uncertainties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28317 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/uncertainties/uncertainties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/uncertainties/uncertainties_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_scalars/uncertainties/uncertainties_named_array_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.929717 named_arrays-0.1.5/named_arrays/_vectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.929717 named_arrays-0.1.5/named_arrays/_vectors/cartesian/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/cartesian/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.933718 named_arrays-0.1.5/named_arrays/_vectors/cartesian/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/cartesian/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/cartesian/vectors_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/cartesian/vectors_cartesian_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/cartesian/vectors_cartesian_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/cartesian/vectors_cartesian_nd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.933718 named_arrays-0.1.5/named_arrays/_vectors/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/tests/test_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/vector_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/vector_named_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25894 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/vectors_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/vectors_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/_vectors/vectors_spectral_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/plt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.933718 named_arrays-0.1.5/named_arrays/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42405 2023-08-07 03:07:06.000000 named_arrays-0.1.5/named_arrays/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 03:07:20.925717 named_arrays-0.1.5/named_arrays.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-08-07 03:07:20.000000 named_arrays-0.1.5/named_arrays.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-07 03:07:20.000000 named_arrays-0.1.5/named_arrays.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 03:07:20.000000 named_arrays-0.1.5/named_arrays.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-07 03:07:20.000000 named_arrays-0.1.5/named_arrays.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 03:07:20.000000 named_arrays-0.1.5/named_arrays.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-07 03:07:06.000000 named_arrays-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-07 03:07:06.000000 named_arrays-0.1.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 03:07:20.933718 named_arrays-0.1.5/setup.cfg
```

### Comparing `named_arrays-0.1.4/.github/workflows/publish.yml` & `named_arrays-0.1.5/.github/workflows/publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 name: Publish to PyPI and TestPyPI
 
-on: push
+on:
+  release:
+    types: [published]
 
 jobs:
   publish:
     name: Build and publish to PyPI and TestPyPI
+    if: startsWith(github.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@master
       - name: Set up Python 3.10
         uses: actions/setup-python@v3
         with:
           python-version: "3.10"
@@ -27,11 +30,10 @@
           --outdir dist/
       - name: Publish to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.TEST_PYPI_API_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
       - name: Publish to PyPI
-        if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `named_arrays-0.1.4/.github/workflows/tests.yml` & `named_arrays-0.1.5/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install package
         run: |
           python -m pip install --upgrade pip
           pip install setuptools wheel
-          pip install git+https://github.com/astropy/astropy.git
+          pip install git+https://github.com/byrdie/astropy.git@bugfix/scalar-power
           pip install -e .[test]
       - name: Test with pytest
         run: |
           pip install pytest pytest-cov
           pytest --doctest-modules --junitxml=junit/test-results.xml --cov=. --cov-report=xml --cov-report=html
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v3
```

### Comparing `named_arrays-0.1.4/PKG-INFO` & `named_arrays-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: named_arrays
-Version: 0.1.4
+Version: 0.1.5
 Summary: Numpy arrays with labeled axes, similar to xarray but with support for uncertainties
 Author-email: "Roy T. Smart" <roytsmart@gmail.com>, "Jacob D. Parker" <jacobdparker@gmail.com>
 Project-URL: Homepage, https://github.com/Kankelborg-Group/named_arrays
 Project-URL: Documentation, https://named-arrays.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -12,14 +12,15 @@
 Provides-Extra: doc
 
 # named_arrays
 
 ![tests](https://github.com/Kankelborg-Group/named_arrays/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/Kankelborg-Group/named_arrays/branch/main/graph/badge.svg?token=x8K7SLx4UB)](https://codecov.io/gh/Kankelborg-Group/named_arrays)
 [![Documentation Status](https://readthedocs.org/projects/named-arrays/badge/?version=latest)](https://named-arrays.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/named-arrays.svg)](https://badge.fury.io/py/named-arrays)
 
 `named_arrays` is an implementation of a [named tensor](https://nlp.seas.harvard.edu/NamedTensor), which assigns names to each axis of an n-dimensional array such as a numpy array.
 
 When using a numpy array, we often have to insert singleton dimensions to align axes before using binary operators etc.
 This is not necessary when using a named tensor implementation such as `xarray` or `named_arrays`, axes are aligned automatically using their names.
 
 ## Installation
```

### Comparing `named_arrays-0.1.4/README.ipynb` & `named_arrays-0.1.5/README.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998737373737374%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(5, '[![PyPI "*

 * *            "version](https://badge.fury.io/py/named-arrays.svg)](https://badge.fury.io/py/named-arrays)\\n')]}}}"}*

```diff
@@ -7,14 +7,15 @@
             },
             "source": [
                 "# named_arrays\n",
                 "\n",
                 "![tests](https://github.com/Kankelborg-Group/named_arrays/actions/workflows/tests.yml/badge.svg)\n",
                 "[![codecov](https://codecov.io/gh/Kankelborg-Group/named_arrays/branch/main/graph/badge.svg?token=x8K7SLx4UB)](https://codecov.io/gh/Kankelborg-Group/named_arrays)\n",
                 "[![Documentation Status](https://readthedocs.org/projects/named-arrays/badge/?version=latest)](https://named-arrays.readthedocs.io/en/latest/?badge=latest)\n",
+                "[![PyPI version](https://badge.fury.io/py/named-arrays.svg)](https://badge.fury.io/py/named-arrays)\n",
                 "\n",
                 "`named_arrays` is an implementation of a [named tensor](https://nlp.seas.harvard.edu/NamedTensor), which assigns names to each axis of an n-dimensional array such as a numpy array.\n",
                 "\n",
                 "When using a numpy array, we often have to insert singleton dimensions to align axes before using binary operators etc.\n",
                 "This is not necessary when using a named tensor implementation such as `xarray` or `named_arrays`, axes are aligned automatically using their names."
             ]
         },
```

### Comparing `named_arrays-0.1.4/README.md` & `named_arrays-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # named_arrays
 
 ![tests](https://github.com/Kankelborg-Group/named_arrays/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/Kankelborg-Group/named_arrays/branch/main/graph/badge.svg?token=x8K7SLx4UB)](https://codecov.io/gh/Kankelborg-Group/named_arrays)
 [![Documentation Status](https://readthedocs.org/projects/named-arrays/badge/?version=latest)](https://named-arrays.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/named-arrays.svg)](https://badge.fury.io/py/named-arrays)
 
 `named_arrays` is an implementation of a [named tensor](https://nlp.seas.harvard.edu/NamedTensor), which assigns names to each axis of an n-dimensional array such as a numpy array.
 
 When using a numpy array, we often have to insert singleton dimensions to align axes before using binary operators etc.
 This is not necessary when using a named tensor implementation such as `xarray` or `named_arrays`, axes are aligned automatically using their names.
 
 ## Installation
```

### Comparing `named_arrays-0.1.4/docs/Makefile` & `named_arrays-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `named_arrays-0.1.4/docs/_templates/class_custom.rst` & `named_arrays-0.1.5/docs/_templates/class_custom.rst`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 .. autoclass:: {{ fullname }}
     :members:
     :show-inheritance:
     :inherited-members:
     :undoc-members:
     :member-order: groupwise
 
-    .. automethod:: __init__
-
     {% block attributes %}
     {% if attributes %}
     .. rubric:: {{ _('Attributes') }}
 
     .. autosummary::
     {% for item in attributes %}
       ~{{ name }}.{{ item }}
@@ -33,9 +31,10 @@
     {% endif %}
     {% endblock %}
 
     {% block dia %}
     .. rubric:: {{ _('Inheritance Diagram') }}
 
     .. inheritance-diagram:: {{ fullname }}
+        :parts: 1
     {% endblock %}
```

### Comparing `named_arrays-0.1.4/docs/_templates/module_custom.rst` & `named_arrays-0.1.5/docs/_templates/module_custom.rst`

 * *Files identical despite different names*

### Comparing `named_arrays-0.1.4/docs/conf.py` & `named_arrays-0.1.5/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,19 +33,20 @@
     'sphinx.ext.autodoc',
     # "sphinx.ext.autodoc.typehints",
     # 'sphinx_autodoc_typehints',
     'sphinx.ext.autosummary',
     'sphinx.ext.intersphinx',
     'sphinx.ext.inheritance_diagram',
     'jupyter_sphinx',
+    'sphinx_favicon'
 ]
 autosummary_generate = True  # Turn on sphinx.ext.autosummary
 autosummary_imported_members = True
 # autoclass_content = 'both'
-# autodoc_typehints = "description"
+autodoc_typehints = "description"
 
 # autosummary_filename_map = {
 #     'kgpy.optics.Surface': 'kgpy.optics.Surface_cls',
 # }
 
 # typehints_fully_qualified = True
 
@@ -68,14 +69,39 @@
 html_theme = 'pydata_sphinx_theme'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
+html_theme_options = {
+    "icon_links": [
+        {
+            "name": "GitHub",
+            "url": "https://github.com/Kankelborg-Group/named_arrays",
+            "icon": "fa-brands fa-github",
+            "type": "fontawesome",
+        },
+        {
+            "name": "PyPI",
+            "url": "https://pypi.org/project/named-arrays/",
+            "icon": "fa-brands fa-python",
+        },
+    ],
+}
+
+favicons = [
+    dict(href="favicon_io/favicon-16x16.png"),
+    dict(href="favicon_io/favicon-32x32.png"),
+    dict(
+        rel="apple-touch-icon",
+        href="favicon_io/apple-touch-icon.png"
+    )
+]
+
 # https://github.com/readthedocs/readthedocs.org/issues/2569
 master_doc = 'index'
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/', None),
```

### Comparing `named_arrays-0.1.4/docs/make.bat` & `named_arrays-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `named_arrays-0.1.4/named_arrays/_core_array_functions.py` & `named_arrays-0.1.5/named_arrays/_core_array_functions.py`

 * *Files identical despite different names*

### Comparing `named_arrays-0.1.4/named_arrays/_vectors/cartesian/cartesian.py` & `named_arrays-0.1.5/named_arrays/_vectors/cartesian/vectors_cartesian.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,51 +26,52 @@
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractCartesianVectorArray(
     na.AbstractVectorArray
 ):
     @property
     @abc.abstractmethod
-    def type_array(self: Self) -> Type[AbstractExplicitCartesianVectorArray]:
+    def type_explicit(self: Self) -> Type[AbstractExplicitCartesianVectorArray]:
         pass
 
+
     @property
     def length(self: Self) -> na.AbstractScalar:
         result = 0
-        components = self.components
-        for c in components:
-            if components[c] is not None:
-                result = result + np.square(components[c])
+        entries = self.cartesian_nd.entries
+        for e in entries:
+            if entries[e] is not None:
+                result = result + np.square(np.abs(entries[e]))
         result = np.sqrt(result)
         return result
 
     def __mul__(self: Self, other: na.ArrayLike | u.Unit) -> AbstractExplicitCartesianVectorArray:
         if isinstance(other, u.UnitBase):
             components = self.components
-            result = self.type_array()
+            result = self.prototype_vector
             for c in components:
                 result.components[c] = components[c] * other
             return result
         else:
             return super().__mul__(other)
 
     def __lshift__(self: Self, other: na.ArrayLike | u.UnitBase) -> AbstractExplicitCartesianVectorArray:
         if isinstance(other, u.UnitBase):
             components= self.components
-            result = self.type_array()
+            result = self.prototype_vector
             for c in components:
                 result.components[c] = components[c] << other
             return result
         else:
             return super().__lshift__(other)
 
     def __truediv__(self: Self, other: na.ArrayLike | u.UnitBase) -> AbstractExplicitCartesianVectorArray:
         if isinstance(other, u.UnitBase):
             components = self.components
-            result = self.type_array()
+            result = self.prototype_vector
             for c in components:
                 result.components[c] = components[c] / other
             return result
         else:
             return super().__truediv__(other)
 
     def __array_ufunc__(
@@ -81,20 +82,23 @@
             **kwargs,
     ) -> None | AbstractExplicitCartesianVectorArray | tuple[AbstractExplicitCartesianVectorArray, ...]:
 
         result = super().__array_ufunc__(function, method, *inputs, **kwargs)
         if result is not NotImplemented:
             return result
 
+        if function is np.matmul:
+            return NotImplemented
+
         components = self.components
 
         components_inputs = []
         for inp in inputs:
             if isinstance(inp, na.AbstractArray):
-                if inp.type_array_abstract == self.type_array_abstract:
+                if inp.type_abstract == self.type_abstract:
                     components_inp = inp.components
                 elif isinstance(inp, na.AbstractScalar):
                     components_inp = {c: inp for c in components}
                 else:
                     return NotImplemented
             else:
                 components_inp = {c: inp for c in components}
@@ -109,20 +113,20 @@
         else:
             out = (None, ) * function.nout
             components_out = {c: (None, ) * function.nout for c in components}
 
         if "where" in kwargs:
             where = kwargs.pop("where")
             if isinstance(where, na.AbstractArray):
-                if where.type_array_abstract == self.type_array_abstract:
+                if where.type_abstract == self.type_abstract:
                     components_where = where.components
-                elif isinstance(where, na.ScalarArray):
+                elif isinstance(where, na.AbstractScalar):
                     components_where = {c: where for c in components}
                 else:
-                    return where.__array_ufunc__(function, method, *inputs, **kwargs)
+                    return NotImplemented
             else:
                 components_where = {c: where for c in components}
         else:
             components_where = {c: True for c in components}
 
         components_result = tuple(dict() for _ in range(function.nout))
         for c in components:
@@ -132,15 +136,15 @@
                 where=components_where[c],
                 **kwargs,
             )
             if function.nout == 1:
                 component_result = (component_result, )
             for i in range(function.nout):
                 components_result[i][c] = component_result[i]
-        result = list(self.type_array.from_components(components_result[i]) for i in range(function.nout))
+        result = list(self.type_explicit.from_components(components_result[i]) for i in range(function.nout))
 
         for i in range(function.nout):
             if out[i] is not None:
                 out[i].components = result[i].components
                 result[i] = out[i]
 
         if function.nout == 1:
@@ -177,125 +181,45 @@
 StartT = TypeVar('StartT', bound=float | complex | u.Quantity | na.AbstractScalar | AbstractCartesianVectorArray)
 StopT = TypeVar('StopT', bound=float | complex | u.Quantity | na.AbstractScalar | AbstractCartesianVectorArray)
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractCartesianVectorUniformRandomSample(
     AbstractCartesianVectorRandomSample,
-    na.AbstractVectorUniformRandomSample,
-    Generic[StartT, StopT],
+    na.AbstractVectorUniformRandomSample[StartT, StopT],
 ):
-    start: StartT = dataclasses.MISSING
-    stop: StopT = dataclasses.MISSING
-    shape_random: dict[str, int] = None
-    seed: None | int = None
-
-    @property
-    def array(self) -> AbstractExplicitCartesianVectorArray:
-        start = self.start
-        if not isinstance(start, na.AbstractVectorArray):
-            start = self.type_array.from_scalar(start)
-
-        stop = self.stop
-        if not isinstance(stop, na.AbstractVectorArray):
-            stop = self.type_array.from_scalar(stop)
-
-        seed = self.seed
-
-        result = self.type_array()
-        components_start = start.components
-        components_stop = stop.components
-
-        for c in result.components:
-            result.components[c] = na.ScalarUniformRandomSample(
-                start=components_start[c],
-                stop=components_stop[c],
-                shape_random=self.shape_random,
-                seed=seed,
-            ).array
-            seed += 1
-
-        return result
+    pass
 
 
 CenterT = TypeVar('CenterT', bound=float | complex | u.Quantity | na.AbstractScalar | AbstractCartesianVectorArray)
 WidthT = TypeVar('WidthT', bound=float | complex | u.Quantity | na.AbstractScalar | AbstractCartesianVectorArray)
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractCartesianVectorNormalRandomSample(
     AbstractCartesianVectorRandomSample,
-    na.AbstractVectorNormalRandomSample,
-    Generic[CenterT, WidthT],
+    na.AbstractVectorNormalRandomSample[CenterT, WidthT],
 ):
-    center: StartT = dataclasses.MISSING
-    width: StopT = dataclasses.MISSING
-    shape_random: dict[str, int] = None
-    seed: None | int = None
-
-    @property
-    def array(self) -> AbstractExplicitCartesianVectorArray:
-        center = self.center
-        if not isinstance(center, na.AbstractVectorArray):
-            center = self.type_array.from_scalar(center)
-
-        width = self.width
-        if not isinstance(width, na.AbstractVectorArray):
-            width = self.type_array.from_scalar(width)
-
-        seed = self.seed
-
-        result = self.type_array()
-        components_center = center.components
-        components_width = width.components
-
-        for c in result.components:
-            result.components[c] = na.ScalarNormalRandomSample(
-                center=components_center[c],
-                width=components_width[c],
-                shape_random=self.shape_random,
-                seed=seed,
-            ).array
-            seed += 1
-
-        return result
+    pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractParameterizedCartesianVectorArray(
     AbstractImplicitCartesianVectorArray,
     na.AbstractParameterizedVectorArray,
 ):
     pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractCartesianVectorArrayRange(
     AbstractParameterizedCartesianVectorArray,
-    na.AbstractVectorArrayRange,
-    Generic[StartT, StopT]
+    na.AbstractVectorArrayRange[StartT, StopT],
 ):
-    @property
-    def array(self) -> AbstractExplicitCartesianVectorArray:
-        start = self.start
-        if not isinstance(start, na.AbstractVectorArray):
-            start = self.type_array.from_scalar(start)
-
-        stop = self.stop
-        if not isinstance(stop, na.AbstractVectorArray):
-            stop = self.type_array.from_scalar(stop)
-
-        result = self.type_array()
-        components_start = start.components
-        components_stop = stop.components
-
-        # for c in result.components:
-        #     result.components[c] = na.
-        #
-        # return
+    pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractCartesianVectorSpace(
     AbstractParameterizedCartesianVectorArray,
     na.AbstractVectorSpace,
 ):
```

### Comparing `named_arrays-0.1.4/named_arrays/_vectors/cartesian/tests/test_cartesian.py` & `named_arrays-0.1.5/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import astropy.units as u
 import named_arrays as na
 import named_arrays._vectors.tests.test_vectors
 
 __all__ = [
     'AbstractTestAbstractCartesianVectorArray',
     'AbstractTestAbstractExplicitCartesianVectorArray',
-    'AbstractTestAbstractExplicitCartesianVectorArrayCreation',
     'AbstractTestAbstractImplicitCartesianVectorArray',
     'AbstractTestAbstractCartesianVectorRandomSample',
     'AbstractTestAbstractCartesianVectorUniformRandomSample',
     'AbstractTestAbstractCartesianVectorNormalRandomSample',
     'AbstractTestAbstractParameterizedCartesianVectorArray',
     'AbstractTestAbstractCartesianVectorArrayRange',
     'AbstractTestAbstractCartesianVectorSpace',
@@ -61,49 +60,49 @@
 
             try:
                 if ufunc in [np.log, np.log2, np.log10, np.sqrt]:
                     kwargs["where"] = array > 0
                 elif ufunc in [np.log1p]:
                     kwargs["where"] = array >= -1
                 elif ufunc in [np.arcsin, np.arccos, np.arctanh]:
-                    kwargs["where"] = (-1< array) & (array < 1)
+                    kwargs["where"] = (-1 < array) & (array < 1)
                 elif ufunc in [np.arccosh]:
                     kwargs["where"] = array >= 1
                 elif ufunc in [np.reciprocal]:
                     kwargs["where"] = array != 0
             except u.UnitConversionError:
                 pass
 
             for c in components:
                 for k in kwargs:
                     if isinstance(kwargs[k], na.AbstractVectorArray):
                         kwargs_components[c][k] = kwargs[k].components[c]
                     else:
                         kwargs_components[c][k] = kwargs[k]
 
-            result_expected = tuple(array.type_array() for _ in range(ufunc.nout))
+            result_expected = tuple(array.prototype_vector for _ in range(ufunc.nout))
             try:
                 for c in components:
                     result_c = ufunc(components[c], **kwargs_components[c])
                     if ufunc.nout == 1:
-                        result_c = (result_c, )
+                        result_c = (result_c,)
                     for i in range(ufunc.nout):
                         result_expected[i].components[c] = result_c[i]
 
             except Exception as e:
                 with pytest.raises(type(e)):
                     ufunc(array, **kwargs)
                 return
 
             result = ufunc(array, **kwargs)
 
             if ufunc.nout == 1:
-                out = 0 * result
+                out = 0 * np.nan_to_num(result)
             else:
-                out = tuple(0 * r for r in result)
+                out = tuple(0 * np.nan_to_num(r) for r in result)
 
             result_out = ufunc(array, out=out, **kwargs)
 
             if ufunc.nout == 1:
                 out = (out,)
                 result = (result,)
                 result_out = (result_out,)
@@ -126,18 +125,18 @@
             super().test_ufunc_binary(ufunc, array, array_2)
 
             if isinstance(array, na.AbstractVectorArray):
                 array_normalized = array
                 if isinstance(array_2, na.AbstractVectorArray):
                     array_2_normalized = array_2
                 else:
-                    array_2_normalized = array.type_array.from_scalar(array_2)
+                    array_2_normalized = array.type_explicit.from_scalar(array_2, like=array)
             else:
                 if isinstance(array_2, na.AbstractVectorArray):
-                    array_normalized = array_2.type_array.from_scalar(array)
+                    array_normalized = array_2.type_explicit.from_scalar(array, like=array_2)
                     array_2_normalized = array_2
                 else:
                     raise ValueError("One of the test arrays should be vectors")
 
             components = array_normalized.components
             components_2 = array_2_normalized.components
 
@@ -145,26 +144,25 @@
             kwargs_components = {c: dict() for c in components}
 
             try:
                 if ufunc in [np.power, np.float_power]:
                     kwargs["where"] = (array_2 >= 1) & (array >= 0)
                 elif ufunc in [np.divide, np.floor_divide, np.remainder, np.fmod, np.divmod]:
                     kwargs["where"] = array_2 != 0
-            except u.UnitConversionError:
+            except (u.UnitConversionError, TypeError):
                 pass
 
             for c in components:
                 for k in kwargs:
                     if isinstance(kwargs[k], na.AbstractVectorArray):
                         kwargs_components[c][k] = kwargs[k].components[c]
                     else:
                         kwargs_components[c][k] = kwargs[k]
 
-
-            result_expected = tuple(array_normalized.type_array() for _ in range(ufunc.nout))
+            result_expected = tuple(array_normalized.prototype_vector for _ in range(ufunc.nout))
             try:
                 for c in components:
                     result_c = ufunc(components[c], components_2[c], **kwargs_components[c])
                     if ufunc.nout == 1:
                         result_c = (result_c,)
                     for i in range(ufunc.nout):
                         result_expected[i].components[c] = result_c[i]
@@ -172,17 +170,17 @@
                 with pytest.raises(type(e)):
                     ufunc(array, array_2, **kwargs)
                 return
 
             result = ufunc(array, array_2, **kwargs)
 
             if ufunc.nout == 1:
-                out = 0 * result
+                out = 0 * np.nan_to_num(result)
             else:
-                out = tuple(0 * r for r in result)
+                out = tuple(0 * np.nan_to_num(r) for r in result)
 
             result_out = ufunc(array, array_2, out=out, **kwargs)
 
             if ufunc.nout == 1:
                 out = (out,)
                 result = (result,)
                 result_out = (result_out,)
@@ -196,22 +194,15 @@
 class AbstractTestAbstractExplicitCartesianVectorArray(
     AbstractTestAbstractCartesianVectorArray,
     named_arrays._vectors.tests.test_vectors.AbstractTestAbstractExplicitVectorArray,
 ):
     pass
 
 
-class AbstractTestAbstractExplicitCartesianVectorArrayCreation(
-    named_arrays._vectors.tests.test_vectors.AbstractTestAbstractExplicitVectorArrayCreation,
-):
-    pass
-
-
 class AbstractTestAbstractImplicitCartesianVectorArray(
-    AbstractTestAbstractCartesianVectorArray,
     named_arrays._vectors.tests.test_vectors.AbstractTestAbstractImplicitVectorArray,
 ):
     pass
 
 
 class AbstractTestAbstractCartesianVectorRandomSample(
     AbstractTestAbstractImplicitCartesianVectorArray,
```

### Comparing `named_arrays-0.1.4/named_arrays/_vectors/cartesian/tests/test_cartesian_2d.py` & `named_arrays-0.1.5/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_2d.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from typing import Type, Callable, Sequence
-
 import pytest
 import numpy as np
 import astropy.units as u
-
 import named_arrays as na
 import named_arrays.tests.test_core
-import named_arrays.scalars.uncertainties.tests.test_uncertainties
-from . import test_cartesian
+import named_arrays._vectors.tests.test_vectors
+from . import test_vectors_cartesian
 
 __all__ = [
     'AbstractTestAbstractCartesian2dVectorArray',
     'TestCartesian2dVectorArray',
-    'TestCartesian2dVectorArrayCreation',
     'AbstractTestAbstractImplicitCartesian2dVectorArray',
     'AbstractTestAbstractCartesian2dVectorRandomSample',
     'TestCartesian2dVectorUniformRandomSample',
     'TestCartesian2dVectorNormalRandomSample',
     'AbstractTestAbstractParameterizedCartesian2dVectorArray',
     'TestCartesian2dVectorArrayRange',
     'AbstractTestAbstractCartesian2dVectorSpace',
@@ -24,47 +21,54 @@
     'TestCartesian2dVectorStratifiedRandomSpace',
     'TestCartesian2dVectorLogarithmicSpace',
     'TestCartesian2dVectorGeometricSpace',
 ]
 
 _num_x = named_arrays.tests.test_core.num_x
 _num_y = named_arrays.tests.test_core.num_y
-_num_distribution = named_arrays.scalars.uncertainties.tests.test_uncertainties._num_distribution
+_num_distribution = named_arrays.tests.test_core.num_distribution
 
 
 def _cartesian2d_arrays():
     arrays_numeric_x = [
         4,
         na.ScalarUniformRandomSample(-4, 4, shape_random=dict(y=_num_y)),
+        na.Cartesian2dVectorArray(x=2, y=3)
     ]
     units_x = [1, u.mm]
     arrays_numeric_x = [a * unit for a in arrays_numeric_x for unit in units_x]
 
     arrays_numeric_y = [
         5.,
         na.ScalarUniformRandomSample(-5, 5, shape_random=dict(x=_num_x, y=_num_y)),
         na.UniformUncertainScalarArray(
             nominal=na.ScalarUniformRandomSample(-5, 5, shape_random=dict(x=_num_x, y=_num_y)),
             width=1,
             num_distribution=_num_distribution
-        )
+        ),
+        na.Cartesian2dVectorArray(x=4, y=8)
     ]
     units_y = [1, u.mm]
     arrays_numeric_y = [a * unit for a in arrays_numeric_y for unit in units_y]
 
     arrays = [na.Cartesian2dVectorArray(x=ax, y=ay) for ax in arrays_numeric_x for ay in arrays_numeric_y]
     return arrays
 
 
 def _cartesian2d_arrays_2():
     units = [1, u.mm]
     arrays_scalar = [
         6,
         na.ScalarArray(6),
         na.ScalarUniformRandomSample(-6, 6, shape_random=dict(y=_num_y, x=_num_x)),
+        na.UniformUncertainScalarArray(
+            nominal=na.ScalarUniformRandomSample(-6, 6, shape_random=dict(y=_num_y, x=_num_x)),
+            width=1,
+            num_distribution=_num_distribution
+        )
     ]
     arrays_scalar = [a * unit for a in arrays_scalar for unit in units]
     arrays_vector_x = [
         7,
         na.ScalarUniformRandomSample(-7, 7, shape_random=dict(y=_num_y)),
     ]
     arrays_vector_x = [a * unit for a in arrays_vector_x for unit in units]
@@ -74,21 +78,16 @@
     ]
     arrays_vector_y = [a * unit for a in arrays_vector_y for unit in units]
     arrays_vector = [na.Cartesian2dVectorArray(x=ax, y=ay) for ax in arrays_vector_x for ay in arrays_vector_y]
     arrays = arrays_scalar + arrays_vector
     return arrays
 
 
-class AbstractTestAbstractCartesian2dVectorArray(
-    test_cartesian.AbstractTestAbstractCartesianVectorArray,
-):
-
-    @pytest.mark.parametrize(
-        argnames='item',
-        argvalues=[
+def _cartesian2d_items() -> list[na.AbstractArray | dict[str, int, slice, na.AbstractArray]]:
+    return [
             dict(y=0),
             dict(y=slice(0, 1)),
             dict(y=na.ScalarArrayRange(0, 2, axis='y')),
             dict(
                 y=na.Cartesian2dVectorArray(
                     x=na.ScalarArrayRange(0, 2, axis='y'),
                     y=na.ScalarArrayRange(0, 2, axis='y'),
@@ -117,36 +116,44 @@
                 num_distribution=_num_distribution,
             ) > 0.5,
             na.Cartesian2dVectorArray(
                 x=na.ScalarLinearSpace(0, 1, axis='y', num=_num_y) > 0.3,
                 y=na.ScalarLinearSpace(0, 1, axis='y', num=_num_y) > 0.5,
             ),
         ]
+
+class AbstractTestAbstractCartesian2dVectorArray(
+    test_vectors_cartesian.AbstractTestAbstractCartesianVectorArray,
+):
+
+    @pytest.mark.parametrize(
+        argnames='item',
+        argvalues=_cartesian2d_items()
     )
     def test__getitem__(
             self,
             array: na.AbstractCartesian2dVectorArray,
             item: dict[str, int | slice | na.AbstractArray] | na.AbstractArray
     ):
         super().test__getitem__(array=array, item=item)
 
     @pytest.mark.parametrize('array_2', _cartesian2d_arrays_2())
     class TestUfuncBinary(
-        test_cartesian.AbstractTestAbstractCartesianVectorArray.TestUfuncBinary
+        test_vectors_cartesian.AbstractTestAbstractCartesianVectorArray.TestUfuncBinary
     ):
         pass
 
     @pytest.mark.parametrize('array_2', _cartesian2d_arrays_2())
     class TestMatmul(
-        test_cartesian.AbstractTestAbstractCartesianVectorArray.TestMatmul
+        test_vectors_cartesian.AbstractTestAbstractCartesianVectorArray.TestMatmul
     ):
         pass
 
     class TestArrayFunctions(
-        test_cartesian.AbstractTestAbstractCartesianVectorArray.TestArrayFunctions
+        test_vectors_cartesian.AbstractTestAbstractCartesianVectorArray.TestArrayFunctions
     ):
 
         @pytest.mark.parametrize(
             argnames='where',
             argvalues=[
                 np._NoValue,
                 True,
@@ -155,15 +162,15 @@
                 na.Cartesian2dVectorArray(
                     x=(na.ScalarLinearSpace(-1, 1, 'x', _num_x) >= 0) | (na.ScalarLinearSpace(-1, 1, 'y', _num_y) >= 0),
                     y=(na.ScalarLinearSpace(-1, 1, 'x', _num_x) <= 0) | (na.ScalarLinearSpace(-1, 1, 'y', _num_y) <= 0),
                 )
             ]
         )
         class TestReductionFunctions(
-            test_cartesian.AbstractTestAbstractCartesianVectorArray.TestArrayFunctions.TestReductionFunctions,
+            test_vectors_cartesian.AbstractTestAbstractCartesianVectorArray.TestArrayFunctions.TestReductionFunctions,
         ):
             pass
 
         @pytest.mark.parametrize(
             argnames='q',
             argvalues=[
                 .25,
@@ -173,60 +180,85 @@
                 na.Cartesian2dVectorArray(
                     x=na.ScalarLinearSpace(.25, .50, axis='q', num=3, endpoint=True),
                     y=na.ScalarLinearSpace(50 * u.percent, 75 * u.percent, axis='q', num=3, endpoint=True)
                 )
             ]
         )
         class TestPercentileLikeFunctions(
-            test_cartesian.AbstractTestAbstractCartesianVectorArray.TestArrayFunctions.TestPercentileLikeFunctions,
+            test_vectors_cartesian.AbstractTestAbstractCartesianVectorArray.TestArrayFunctions.
+            TestPercentileLikeFunctions,
         ):
             pass
 
 
 @pytest.mark.parametrize('array', _cartesian2d_arrays())
 class TestCartesian2dVectorArray(
     AbstractTestAbstractCartesian2dVectorArray,
-    test_cartesian.AbstractTestAbstractExplicitCartesianVectorArray,
+    test_vectors_cartesian.AbstractTestAbstractExplicitCartesianVectorArray,
 ):
-    pass
 
-
-class TestCartesian2dVectorArrayCreation(
-    test_cartesian.AbstractTestAbstractExplicitCartesianVectorArrayCreation,
-):
-    @property
-    def type_array(self) -> Type[na.Cartesian2dVectorArray]:
-        return na.Cartesian2dVectorArray
+    @pytest.mark.parametrize(
+        argnames="item",
+        argvalues=[
+            dict(y=0),
+            dict(x=0, y=0),
+            dict(y=slice(None)),
+            dict(y=na.ScalarArrayRange(0, _num_y, axis='y')),
+            dict(x=na.ScalarArrayRange(0, _num_x, axis='x'), y=na.ScalarArrayRange(0, _num_y, axis='y')),
+            dict(
+                y=na.Cartesian2dVectorArray(
+                    x=na.ScalarArrayRange(0, _num_y, axis='y'),
+                    y=na.ScalarArrayRange(0, _num_y, axis='y'),
+                )
+            ),
+            na.ScalarArray.ones(shape=dict(y=_num_y), dtype=bool),
+            np.ones_like(na.Cartesian2dVectorArray(), dtype=bool, shape=dict(y=_num_y)),
+        ],
+    )
+    @pytest.mark.parametrize(
+        argnames="value",
+        argvalues=[
+            0,
+            na.ScalarUniformRandomSample(-5, 5, dict(y=_num_y)),
+            na.Cartesian2dVectorUniformRandomSample(-5, 5, shape_random=dict(y=_num_y)),
+        ]
+    )
+    def test__setitem__(
+            self,
+            array: na.ScalarArray,
+            item: dict[str, int | slice | na.ScalarArray] | na.ScalarArray,
+            value: float | na.ScalarArray
+    ):
+        super().test__setitem__(array=array, item=item, value=value)
 
 
 class AbstractTestAbstractImplicitCartesian2dVectorArray(
-    AbstractTestAbstractCartesian2dVectorArray,
-    test_cartesian.AbstractTestAbstractImplicitCartesianVectorArray,
+    test_vectors_cartesian.AbstractTestAbstractImplicitCartesianVectorArray,
 ):
     pass
 
 
 class AbstractTestAbstractCartesian2dVectorRandomSample(
     AbstractTestAbstractImplicitCartesian2dVectorArray,
-    test_cartesian.AbstractTestAbstractCartesianVectorRandomSample,
+    test_vectors_cartesian.AbstractTestAbstractCartesianVectorRandomSample,
 ):
     pass
 
 
 def _cartesian_2d_uniform_random_samples() -> list[na.Cartesian2dVectorUniformRandomSample]:
     starts = [
         0,
-        na.Cartesian2dVectorArray(x=0, y=1),
         na.Cartesian2dVectorArray(
             x=na.ScalarLinearSpace(0, 1, axis='x', num=_num_x),
             y=na.ScalarLinearSpace(1, 2, axis='x', num=_num_x)
         )
     ]
     stops = [
         10,
+        na.UniformUncertainScalarArray(10, width=1, num_distribution=_num_distribution),
         na.Cartesian2dVectorArray(x=10, y=11),
         na.Cartesian2dVectorArray(
             x=na.ScalarLinearSpace(10, 11, axis='x', num=_num_x),
             y=na.ScalarLinearSpace(11, 12, axis='x', num=_num_x)
         ),
     ]
     units = [None, u.mm]
@@ -236,72 +268,139 @@
             start=start << unit if unit is not None else start,
             stop=stop << unit if unit is not None else stop,
             shape_random=shape_random,
         ) for start in starts for stop in stops for unit in units for shape_random in shapes_random
     ]
 
 
-@pytest.mark.skip
 @pytest.mark.parametrize('array', _cartesian_2d_uniform_random_samples())
 class TestCartesian2dVectorUniformRandomSample(
     AbstractTestAbstractCartesian2dVectorRandomSample,
-    test_cartesian.AbstractTestAbstractCartesianVectorUniformRandomSample,
+    test_vectors_cartesian.AbstractTestAbstractCartesianVectorUniformRandomSample,
 ):
     pass
 
 
-@pytest.mark.skip
+def _cartesian_2d_normal_random_samples() -> list[na.Cartesian2dVectorNormalRandomSample]:
+    centers = [
+        0,
+        na.Cartesian2dVectorArray(
+            x=na.ScalarLinearSpace(0, 1, axis='x', num=_num_x),
+            y=na.ScalarLinearSpace(1, 2, axis='x', num=_num_x)
+        )
+    ]
+    widths = [
+        10,
+        na.UniformUncertainScalarArray(10, width=1, num_distribution=_num_distribution),
+        na.Cartesian2dVectorArray(x=10, y=11),
+        na.Cartesian2dVectorArray(
+            x=na.ScalarLinearSpace(10, 11, axis='x', num=_num_x),
+            y=na.ScalarLinearSpace(11, 12, axis='x', num=_num_x)
+        ),
+    ]
+    units = [None, u.mm]
+    shapes_random = [dict(y=_num_y)]
+    return [
+        na.Cartesian2dVectorNormalRandomSample(
+            center=center << unit if unit is not None else center,
+            width=width << unit if unit is not None else width,
+            shape_random=shape_random,
+        ) for center in centers for width in widths for unit in units for shape_random in shapes_random
+    ]
+
+
+@pytest.mark.parametrize('array', _cartesian_2d_normal_random_samples())
 class TestCartesian2dVectorNormalRandomSample(
     AbstractTestAbstractCartesian2dVectorRandomSample,
-    test_cartesian.AbstractTestAbstractCartesianVectorNormalRandomSample,
+    test_vectors_cartesian.AbstractTestAbstractCartesianVectorNormalRandomSample,
 ):
     pass
 
 
 class AbstractTestAbstractParameterizedCartesian2dVectorArray(
     AbstractTestAbstractImplicitCartesian2dVectorArray,
-    test_cartesian.AbstractTestAbstractParameterizedCartesianVectorArray,
+    test_vectors_cartesian.AbstractTestAbstractParameterizedCartesianVectorArray,
 ):
     pass
 
 
-@pytest.mark.skip
+
+def _cartesian_2d_vector_array_ranges() -> tuple[na.Cartesian2dVectorArrayRange, ...]:
+    starts = (
+        0,
+        na.Cartesian2dVectorArray(0, 1),
+    )
+    stops = (
+        5,
+        na.Cartesian2dVectorArray(5, 5)
+    )
+    axes = (
+        na.Cartesian2dVectorArray('x', 'y'),
+    )
+    _num = na.Cartesian2dVectorArray(_num_x, _num_y)
+    return tuple(
+        na.Cartesian2dVectorArrayRange(
+            start=start,
+            stop=stop,
+            axis=axis,
+            step=(stop - start) / _num,
+        )
+        for start in starts
+        for stop in stops
+        for axis in axes
+    )
+
+
+@pytest.mark.parametrize("array", _cartesian_2d_vector_array_ranges())
 class TestCartesian2dVectorArrayRange(
     AbstractTestAbstractParameterizedCartesian2dVectorArray,
-    test_cartesian.AbstractTestAbstractCartesianVectorArrayRange,
+    test_vectors_cartesian.AbstractTestAbstractCartesianVectorArrayRange,
 ):
     pass
 
 
 class AbstractTestAbstractCartesian2dVectorSpace(
     AbstractTestAbstractParameterizedCartesian2dVectorArray,
-    test_cartesian.AbstractTestAbstractCartesianVectorSpace,
+    test_vectors_cartesian.AbstractTestAbstractCartesianVectorSpace,
 ):
     pass
 
-@pytest.mark.skip
-class TestCartesian2dVectorLinearSpace(
-    AbstractTestAbstractCartesian2dVectorSpace,
-    test_cartesian.AbstractTestAbstractCartesianVectorLinearSpace,
-):
-    pass
 
-@pytest.mark.skip
-class TestCartesian2dVectorStratifiedRandomSpace(
-    TestCartesian2dVectorLinearSpace,
-    test_cartesian.AbstractTestAbstractCartesianVectorStratifiedRandomSpace,
-):
-    pass
+def _cartesian_2d_vector_linear_spaces() -> tuple[na.Cartesian2dVectorLinearSpace, ...]:
+    starts = (
+        0,
+        na.Cartesian2dVectorArray(0, 1),
+    )
+    stops = (
+        5,
+        na.Cartesian2dVectorArray(5, 5)
+    )
+    axes = (
+        na.Cartesian2dVectorArray('x', 'y'),
+    )
+    nums = (
+        na.Cartesian2dVectorArray(_num_x, _num_y),
+    )
+    return tuple(
+        na.Cartesian2dVectorLinearSpace(
+            start=start,
+            stop=stop,
+            axis=axis,
+            num=num,
+        )
+        for start in starts
+        for stop in stops
+        for axis in axes
+        for num in nums
+    )
 
-@pytest.mark.skip
-class TestCartesian2dVectorLogarithmicSpace(
-    AbstractTestAbstractCartesian2dVectorSpace,
-    test_cartesian.AbstractTestAbstractCartesianVectorLogarithmicSpace,
-):
-    pass
 
-@pytest.mark.skip
-class TestCartesian2dVectorGeometricSpace(
+@pytest.mark.parametrize("array", _cartesian_2d_vector_linear_spaces())
+class TestCartesian2dVectorLinearSpace(
     AbstractTestAbstractCartesian2dVectorSpace,
-    test_cartesian.AbstractTestAbstractCartesianVectorGeometricSpace,
+    AbstractTestAbstractCartesian2dVectorArray,
+    test_vectors_cartesian.AbstractTestAbstractCartesianVectorLinearSpace,
+    test_vectors_cartesian.AbstractTestAbstractCartesianVectorArray,
+    named_arrays._vectors.tests.test_vectors.AbstractTestAbstractVectorArray,
+    named_arrays.tests.test_core.AbstractTestAbstractArray,
 ):
     pass
```

### Comparing `named_arrays-0.1.4/named_arrays/_vectors/tests/test_vectors.py` & `named_arrays-0.1.5/named_arrays/_vectors/tests/test_vectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,38 @@
     'AbstractTestAbstractVectorSpace',
     'AbstractTestAbstractVectorLinearSpace',
     'AbstractTestAbstractVectorStratifiedRandomSpace',
     'AbstractTestAbstractVectorLogarithmicSpace',
     'AbstractTestAbstractVectorGeometricSpace',
 ]
 
+
 class AbstractTestAbstractVectorArray(
     named_arrays.tests.test_core.AbstractTestAbstractArray,
 ):
+    def test_cartesian_nd(self, array: na.AbstractVectorArray):
+        cartesian_nd = array.cartesian_nd
+        assert isinstance(cartesian_nd, na.AbstractCartesianNdVectorArray)
+        for c in cartesian_nd.components:
+            assert isinstance(na.as_named_array(cartesian_nd.components[c]), na.AbstractScalar)
+
+    def test_from_cartesian_nd(self, array: na.AbstractVectorArray):
+        assert np.all(array.type_explicit.from_cartesian_nd(array.cartesian_nd, like=array) == array)
+
+    def test_matrix(self, array: na.AbstractVectorArray):
+        def _recursive_test(array: na.AbstractMatrixArray):
+            assert isinstance(array, na.AbstractMatrixArray)
+            components = array.components
+            for c in components:
+                component = components[c]
+                if isinstance(component, na.AbstractVectorArray):
+                    _recursive_test(component)
+                else:
+                    assert isinstance(na.as_named_array(component), na.AbstractScalar)
+        _recursive_test(array.matrix)
 
     def test_components(self, array: na.AbstractVectorArray):
         components = array.components
         assert isinstance(components, dict)
         for component in components:
             assert isinstance(component, str)
             assert isinstance(components[component], (int, float, complex, np.ndarray, na.AbstractArray))
@@ -41,35 +62,36 @@
         for c in components:
             assert array.axes == components[c].axes
 
     @pytest.mark.parametrize('dtype', [int, float])
     def test_astype(self, array: na.AbstractVectorArray, dtype: Type):
         super().test_astype(array=array, dtype=dtype)
         array_new = array.astype(dtype)
-        for c in array_new.components:
-            assert array_new.components[c].dtype == dtype
+        for e in array_new.entries:
+            entry = array_new.entries[e]
+            assert entry.dtype == dtype
 
     @pytest.mark.parametrize('unit', [u.mm, u.s])
     def test_to(self, array: na.AbstractVectorArray, unit: None | u.UnitBase):
         super().test_to(array=array, unit=unit)
-        components = array.components
-        if all(unit.is_equivalent(na.unit_normalized(components[c])) for c in components):
+        entries = array.cartesian_nd.entries
+        if all(unit.is_equivalent(na.unit_normalized(entries[e])) for e in entries):
             array_new = array.to(unit)
-            assert array_new.type_array_abstract == array.type_array_abstract
-            assert all(array_new.components[c].unit == unit for c in array_new.components)
+            assert array_new.type_abstract == array.type_abstract
+            assert all(array_new.cartesian_nd.entries[e].unit == unit for e in array_new.cartesian_nd.entries)
         else:
             with pytest.raises(u.UnitConversionError):
                 array.to(unit)
 
     def test_length(self, array: na.AbstractVectorArray):
         super().test_length(array=array)
-        components = array.components
-        components_iter = iter(components)
-        comp_0 = components[next(components_iter)]
-        if all(na.unit_normalized(comp_0).is_equivalent(na.unit_normalized(components[c])) for c in components_iter):
+        entries = array.cartesian_nd.entries
+        entries_iter = iter(entries)
+        entry_0 = entries[next(entries_iter)]
+        if all(na.unit_normalized(entry_0).is_equivalent(na.unit_normalized(entries[e])) for e in entries_iter):
             length = array.length
             assert isinstance(length, (int, float, np.ndarray, na.AbstractScalar))
             assert np.all(length >= 0)
         else:
             with pytest.raises(u.UnitConversionError):
                 array.length
 
@@ -87,47 +109,47 @@
 
         components = array.broadcasted.components
         components_expected = dict()
 
         if isinstance(item, dict):
             components_item = {c: dict() for c in components}
             for ax in item:
-                if isinstance(item[ax], na.AbstractArray) and item[ax].type_array_abstract == array.type_array_abstract:
+                if isinstance(item[ax], na.AbstractArray) and item[ax].type_abstract == array.type_abstract:
                     components_item_ax = item[ax].components
                 else:
-                    components_item_ax = array.type_array.from_scalar(item[ax]).components
+                    components_item_ax = array.type_explicit.from_scalar(item[ax], like=array).components
                 for c in components:
                     components_item[c][ax] = components_item_ax[c]
 
         else:
-            if not item.type_array_abstract == array.type_array_abstract:
-                components_item = array.type_array.from_scalar(item).components
+            if not item.type_abstract == array.type_abstract:
+                components_item = array.type_explicit.from_scalar(item, like=array).components
             else:
                 components_item = item.components
                 item_accumulated = True
                 for c in components_item:
                     item_accumulated = item_accumulated & components_item[c]
-                components_item = item.type_array.from_scalar(item_accumulated).components
+                components_item = item.type_explicit.from_scalar(item_accumulated, like=array).components
 
         for c in components:
             components_expected[c] = na.as_named_array(components[c])[components_item[c]]
 
-        result_expected = array.type_array.from_components(components_expected)
+        result_expected = array.type_explicit.from_components(components_expected)
 
         result = array[item]
 
         assert isinstance(result.shape, dict)
         assert np.all(result == result_expected)
 
     def test__bool__(self, array: na.AbstractVectorArray):
-        if array.shape or any(na.unit(array.components[c]) is not None for c in array.components):
+        if array.shape or any(na.unit(array.cartesian_nd.entries[e]) is not None for e in array.cartesian_nd.entries):
             with pytest.raises(
-                expected_exception=ValueError,
-                match=r"(Quantity truthiness is ambiguous, .*)"
-                      r"|(The truth value of an array with more than one element is ambiguous. .*)"
+                    expected_exception=ValueError,
+                    match=r"(Quantity truthiness is ambiguous, .*)"
+                          r"|(The truth value of an array with more than one element is ambiguous. .*)"
             ):
                 bool(array)
             return
 
         result = bool(array)
         assert isinstance(result, bool)
 
@@ -139,19 +161,22 @@
                 self,
                 array: None | bool | int | float | complex | str | na.AbstractArray,
                 array_2: None | bool | int | float | complex | str | na.AbstractArray,
         ):
 
             try:
                 if isinstance(array, na.AbstractVectorArray) and isinstance(array_2, na.AbstractVectorArray):
-                    components_1 = array.components
-                    components_2 = array_2.components
-                    result_expected = 0
-                    for c in components_1:
-                        result_expected = result_expected + components_1[c] * components_2[c]
+                    components_1 = array.cartesian_nd.components
+                    components_2 = array_2.cartesian_nd.components
+                    if np.all(components_2.keys() == components_1.keys()):
+                        result_expected = 0
+                        for c in components_1:
+                            result_expected = result_expected + components_1[c] * components_2[c]
+                    else:
+                        raise TypeError
                 else:
                     result_expected = np.multiply(array, array_2)
             except (ValueError, TypeError) as e:
                 with pytest.raises(type(e)):
                     np.matmul(array, array_2)
                 return
 
@@ -212,17 +237,16 @@
                             kwargs_components[c][k] = kwargs[k].components[c]
                         else:
                             kwargs_components[c][k] = kwargs[k]
 
                         if isinstance(kwargs_components[c][k], na.AbstractArray):
                             kwargs_components[c][k] = kwargs_components[c][k].broadcast_to(shape)
 
-
                 try:
-                    result_expected = array.type_array()
+                    result_expected = array.prototype_vector
                     for c in components:
                         component = na.as_named_array(array.components[c]).broadcast_to(shape)
                         result_expected.components[c] = func(component, **kwargs_components[c])
                 except (ValueError, TypeError, u.UnitsError) as e:
                     with pytest.raises(type(e)):
                         func(array, **kwargs)
                     return
@@ -247,15 +271,15 @@
                     array: na.AbstractVectorArray,
                     q: float | u.Quantity | na.AbstractArray,
                     axis: None | str | Sequence[str],
                     keepdims: bool,
             ):
                 super().test_percentile_like_functions(
                     func=func,
-                    array=array.array,
+                    array=array.explicit,
                     q=q,
                     axis=axis,
                     keepdims=keepdims,
                 )
 
                 shape = array.shape
                 components = array.components
@@ -272,15 +296,15 @@
                     kwargs_components[c] = dict(
                         q=components_q[c],
                         axis=axis,
                         keepdims=keepdims,
                     )
 
                 try:
-                    result_expected = array.type_array()
+                    result_expected = array.prototype_vector
                     for c in components:
                         component = na.as_named_array(array.components[c]).broadcast_to(shape)
                         result_expected.components[c] = func(component, **kwargs_components[c])
                 except (ValueError, TypeError) as e:
                     with pytest.raises(type(e)):
                         func(array, **kwargs)
                     return
@@ -314,15 +338,15 @@
                 if axis[0] not in array.shape:
                     with pytest.raises(ValueError, match="`axis` .* not in array with shape .*"):
                         func(array, axis=axis)
                     return
 
                 result = func(array, axis=axis)
 
-                result_expected = array.type_array()
+                result_expected = array.prototype_vector
                 for c in array.components:
                     result_expected.components[c] = func(array.broadcasted.components[c], axis=axis)
 
                 assert np.all(result == result_expected)
 
         class TestFFTNLikeFunctions(
             named_arrays.tests.test_core.AbstractTestAbstractArray.TestArrayFunctions.TestFFTNLikeFunctions,
@@ -350,15 +374,15 @@
                 if s is not None and axes.keys() != s.keys():
                     with pytest.raises(ValueError):
                         func(a=array, axes=axes, s=s)
                     return
 
                 result = func(array, axes=axes, s=s)
 
-                result_expected = array.type_array()
+                result_expected = array.prototype_vector
                 for c in array.components:
                     result_expected.components[c] = func(
                         array.broadcasted.components[c],
                         axes=axes,
                         s=s,
                     )
 
@@ -383,28 +407,28 @@
 
             result = np.sort(array, axis=axis)
 
             array_broadcasted = na.broadcast_to(array, array.shape)
             components_broadcasted = array_broadcasted.components
 
             if axis_normalized:
-                result_expected = array.type_array()
+                result_expected = array.prototype_vector
                 for c in components_broadcasted:
                     result_expected.components[c] = np.sort(components_broadcasted[c], axis=axis_normalized)
             else:
                 result_expected = array
 
             assert np.all(result == result_expected)
 
         @pytest.mark.parametrize('copy', [False, True])
         def test_nan_to_num(self, array: na.AbstractVectorArray, copy: bool):
             components = array.components
 
             components_expected = {c: np.nan_to_num(components[c], copy=copy) for c in components}
-            result_expected = array.type_array.from_components(components_expected)
+            result_expected = array.type_explicit.from_components(components_expected)
 
             if not copy and isinstance(array, na.AbstractImplicitArray):
                 with pytest.raises(ValueError, match=r"can\'t write to an array that is not an instance of .*"):
                     np.nan_to_num(array, copy=copy)
                 return
 
             result = np.nan_to_num(array, copy=copy)
@@ -418,89 +442,33 @@
     def test_broadcasted(self, array: na.AbstractVectorArray):
         array_broadcasted = array.broadcasted
         shape = array.shape
         components = array_broadcasted.components
         for component in components:
             assert components[component].shape == shape
 
-    def test_ptp(
-            self,
-            array: na.AbstractVectorArray,
+    class TestNamedArrayFunctions(
+        named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions
     ):
-        super().test_ptp(array=array)
-        if any(np.issubdtype(na.get_dtype(array.components[c]), bool) for c in array.components):
-            with pytest.raises(TypeError, match='numpy boolean subtract, .*'):
-                array.ptp()
-            return
-
-        assert np.all(array.ptp() == np.ptp(array))
 
-    def test_all(
-            self,
-            array: na.AbstractVectorArray,
-    ):
-        super().test_all(array=array)
-        components = array.components
-        if any(na.unit(components[c]) is not None for c in components):
-            with pytest.raises(TypeError, match="no implementation found for .*"):
-                array.all()
-            return
-
-        assert np.all(array.all() == np.all(array))
-
-    def test_any(
-            self,
-            array: na.AbstractVectorArray,
-    ):
-        super().test_any(array=array)
-        components = array.components
-        if any(na.unit(components[c]) is not None for c in components):
-            with pytest.raises(TypeError, match="no implementation found for .*"):
-                array.any()
-            return
-
-        assert np.all(array.any() == np.any(array))
+        @pytest.mark.xfail
+        class TestPltPlotLikeFunctions(
+            named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestPltPlotLikeFunctions
+        ):
+            pass
 
 
 class AbstractTestAbstractExplicitVectorArray(
     AbstractTestAbstractVectorArray,
     named_arrays.tests.test_core.AbstractTestAbstractExplicitArray,
 ):
     pass
 
 
-class AbstractTestAbstractExplicitVectorArrayCreation(
-    named_arrays.tests.test_core.AbstractTestAbstractExplicitArrayCreation,
-):
-    @property
-    @abc.abstractmethod
-    def type_array(self) -> Type[na.AbstractExplicitVectorArray]:
-        pass
-
-    def test_empty(self, shape: dict[str, int], dtype: Type):
-        super().test_empty(shape=shape, dtype=dtype)
-        result = self.type_array.empty(shape, dtype=dtype)
-        for c in result.components:
-            assert result.components[c].dtype == dtype
-
-    def test_zeros(self, shape: dict[str, int], dtype: Type):
-        super().test_zeros(shape=shape, dtype=dtype)
-        result = self.type_array.zeros(shape, dtype=dtype)
-        for c in result.components:
-            assert result.components[c].dtype == dtype
-
-    def test_ones(self, shape: dict[str, int], dtype: Type):
-        super().test_ones(shape=shape, dtype=dtype)
-        result = self.type_array.ones(shape, dtype=dtype)
-        for c in result.components:
-            assert result.components[c].dtype == dtype
-
-
 class AbstractTestAbstractImplicitVectorArray(
-    AbstractTestAbstractVectorArray,
     named_arrays.tests.test_core.AbstractTestAbstractImplicitArray,
 ):
     pass
 
 
 class AbstractTestAbstractVectorRandomSample(
     AbstractTestAbstractImplicitVectorArray,
```

### Comparing `named_arrays-0.1.4/named_arrays/_vectors/vector_array_functions.py` & `named_arrays-0.1.5/named_arrays/_vectors/vector_array_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from typing import Callable, Sequence, Type
 import numpy as np
 import astropy.units as u
 import named_arrays as na
+import named_arrays._scalars.scalar_array_functions
+from . import vectors
 
 __all__ = [
+    'ARRAY_CREATION_LIKE_FUNCTIONS',
+    'SEQUENCE_FUNCTIONS',
     'DEFAULT_FUNCTIONS',
     'PERCENTILE_LIKE_FUNCTIONS',
     'ARG_REDUCE_FUNCTIONS',
     'FFT_LIKE_FUNCTIONS',
     'FFTN_LIKE_FUNCTIONS',
     'HANDLED_FUNCTIONS',
     'STACK_LIKE_FUNCTIONS',
 ]
 
-
+ARRAY_CREATION_LIKE_FUNCTIONS = named_arrays._scalars.scalar_array_functions.ARRAY_CREATION_LIKE_FUNCTIONS
+SEQUENCE_FUNCTIONS = named_arrays._scalars.scalar_array_functions.SEQUENCE_FUNCTIONS
 DEFAULT_FUNCTIONS = [
     np.ndim,
     np.min,
     np.nanmin,
     np.max,
     np.nanmax,
     np.sum,
@@ -68,26 +73,89 @@
 STACK_LIKE_FUNCTIONS = [
     np.stack,
     np.concatenate,
 ]
 HANDLED_FUNCTIONS = dict()
 
 
+def array_function_array_creation_like(
+        func: Callable,
+        prototype: na.AbstractVectorArray,
+        dtype: None | type | np.dtype = None,
+        order: str = "K",
+        subok: bool = True,
+        shape: dict[str, int] = None,
+) -> na.AbstractVectorArray:
+
+    components = prototype.components
+
+    components_result = dict()
+    for c in components:
+        components_result[c] = func(
+            na.as_named_array(components[c]),
+            dtype=dtype,
+            order=order,
+            subok=subok,
+            shape=shape,
+        )
+
+    return prototype.type_explicit.from_components(components_result)
+
+
+def array_function_sequence(
+        func: Callable,
+        *args: float | u.Quantity | na.AbstractScalar | na.AbstractVectorArray,
+        axis: str | na.AbstractVectorArray,
+        num: int | na.AbstractVectorArray = 50,
+        endpoint: bool = True,
+        dtype: None | type | np.dtype = None,
+        **kwargs: float | u.Quantity | na.AbstractScalar | na.AbstractVectorArray,
+) -> na.AbstractVectorArray:
+
+    try:
+        prototype = vectors._prototype(*args, *kwargs.values())
+        args = tuple(vectors._normalize(arg, prototype) for arg in args)
+        axis = vectors._normalize(axis, prototype)
+        num = vectors._normalize(num, prototype)
+        kwargs = {k: vectors._normalize(kwargs[k], prototype) for k in kwargs}
+    except na.VectorTypeError:
+        return NotImplemented
+
+    components_args = tuple(arg.components for arg in args)
+    components_axis = axis.components
+    components_num = num.components
+    components_kwargs = {k: kwargs[k].components for k in kwargs}
+
+    components = {
+        c: func(
+            *tuple(na.as_named_array(components_arg[c]) for components_arg in components_args),
+            axis=components_axis[c],
+            num=components_num[c],
+            endpoint=endpoint,
+            dtype=dtype,
+            **{k: na.as_named_array(components_kwargs[k][c]) for k in components_kwargs},
+        )
+        for c in prototype.components
+    }
+
+    return prototype.type_explicit.from_components(components)
+
+
 def array_function_default(
         func: Callable,
         a: na.AbstractVectorArray,
         axis: None | str | Sequence[str] = None,
         dtype: None | type | np.dtype = np._NoValue,
         out: None | na.AbstractExplicitVectorArray = None,
         keepdims: bool = False,
         initial: None | bool | int | float | complex | u.Quantity = np._NoValue,
         where: na.AbstractScalarArray | na.AbstractVectorArray = np._NoValue,
 ) -> na.AbstractExplicitVectorArray:
 
-    a = a.array
+    a = a.explicit
     shape = na.shape_broadcasted(a, where)
 
     axis_normalized = tuple(shape) if axis is None else (axis, ) if isinstance(axis, str) else axis
 
     if axis is not None:
         if not set(axis_normalized).issubset(shape):
             raise ValueError(
@@ -107,15 +175,15 @@
     )
 
     if dtype is not np._NoValue:
         kwargs_base["dtype"] = dtype
     if initial is not np._NoValue:
         kwargs_base["initial"] = initial
 
-    result = a.type_array()
+    result = a.prototype_vector
     for c in components:
         component = na.as_named_array(components[c])
         where_c = components_where[c]
         shape_c = na.broadcast_shapes(component.shape, na.shape(where_c), shape_base)
         kwargs = dict()
         if where_c is not np._NoValue:
             kwargs["where"] = where_c.broadcast_to(shape_c) if isinstance(where_c, na.AbstractArray) else where_c
@@ -139,15 +207,15 @@
         axis: None | str | Sequence[str] = None,
         out: None | na.AbstractExplicitVectorArray = None,
         overwrite_input: bool = False,
         method: str = 'linear',
         keepdims: bool = False,
 ) -> na.AbstractExplicitVectorArray:
 
-    a = a.array
+    a = a.explicit
     shape = a.shape
 
     axis_normalized = na.axis_normalized(a, axis)
 
     if axis is not None:
         if not set(axis_normalized).issubset(shape):
             raise ValueError(
@@ -163,15 +231,15 @@
     kwargs_base = dict(
         axis=axis,
         overwrite_input=overwrite_input,
         method=method,
         keepdims=keepdims,
     )
 
-    result = a.type_array()
+    result = a.prototype_vector
     for c in components:
         component = na.as_named_array(components[c])
         shape_c = na.broadcast_shapes(component.shape, shape_base)
         result.components[c] = func(
             component.broadcast_to(shape_c),
             q=components_q[c],
             out=components_out[c],
@@ -186,15 +254,15 @@
 
 def array_function_arg_reduce(
         func: Callable,
         a: na.AbstractVectorArray,
         axis: None | str | Sequence[str] = None,
 ) -> dict[str, na.AbstractVectorArray]:
 
-    a = a.array
+    a = a.explicit
     components = a.components
 
     if axis is not None:
         if isinstance(axis, str):
             axis = (axis, )
         if not set(axis).issubset(a.axes):
             raise ValueError(f"Reduction axes {axis} are not a subset of the array axes {a.axes}")
@@ -204,56 +272,57 @@
 
     axis_normalized = na.axis_normalized(a, axis)
 
     components_result = dict()
     for c in components:
         component = na.as_named_array(components[c])
         shape_c = component.shape
-        if shape_c:
+        axis_c = tuple(ax for ax in axis_normalized if ax in shape_c)
+        if axis_c:
             components_result[c] = func(
                 a=component,
-                axis=tuple(ax for ax in axis_normalized if ax in shape_c),
+                axis=axis_c,
             )
         else:
             components_result[c] = dict()
 
     axes_result = tuple(set(ax for c in components_result for ax in components_result[c]))
 
     result = dict()
     for ax in axes_result:
-        result[ax] = a.type_array()
+        result[ax] = a.prototype_vector
         for c in components:
             result[ax].components[c] = components_result[c].get(ax, None)
 
     return result
 
 
 def array_function_fft_like(
         func: Callable,
         a: na.AbstractVectorArray,
         axis: tuple[str, str],
         n: None | int = None,
         norm: str = "backward"
 ) -> na.AbstractExplicitVectorArray:
 
-    a = a.array
+    a = a.explicit
     components = a.components
     shape = a.shape
 
     if axis[0] not in shape:
         raise ValueError(f"`axis` {axis[0]} not in array with shape {shape}")
 
     shape_axis = {axis[0]: shape[axis[0]]}
 
     components = {
         c: na.broadcast_to(components[c], na.broadcast_shapes(na.shape(components[c]), shape_axis))
         for c in components
     }
 
-    result = a.type_array()
+    result = a.prototype_vector
     for c in components:
         result.components[c] = func(
             a=components[c],
             axis=axis,
             n=n,
             norm=norm,
         )
@@ -265,24 +334,24 @@
         func: Callable,
         a: na.AbstractVectorArray,
         axes: dict[str, str],
         s: None | dict[str, int] = None,
         norm: str = "backward",
 ) -> na.AbstractExplicitVectorArray:
 
-    a = a.array
+    a = a.explicit
     components = a.components
     shape_a = a.shape
 
     if not set(axes).issubset(shape_a):
         raise ValueError(f"`axes`, {tuple(axes)}, not a subset of array axes, {tuple(shape_a)}")
 
     shape_base = {ax: shape_a[ax] for ax in axes}
 
-    result = a.type_array()
+    result = a.prototype_vector
     for c in components:
         component = na.as_named_array(components[c])
         result.components[c] = func(
             a=na.broadcast_to(component, na.broadcast_shapes(component.shape, shape_base)),
             axes=axes,
             s=s,
             norm=norm,
@@ -295,32 +364,82 @@
     """Register an ``__array_function__`` implementation for :class:`AbstractVectorArray` objects."""
     def decorator(func):
         HANDLED_FUNCTIONS[numpy_function] = func
         return func
     return decorator
 
 
+@implements(np.copyto)
+def copyto(
+        dst: na.AbstractExplicitVectorArray,
+        src: na.AbstractScalar | na.AbstractVectorArray,
+        casting: str = "same_kind",
+        where: bool | na.AbstractScalar | na.AbstractVectorArray = True,
+) -> None:
+    if not isinstance(dst, na.AbstractExplicitVectorArray):
+        return NotImplemented
+
+    components_dst = dst.components
+
+    if isinstance(src, na.AbstractArray):
+        if isinstance(src, na.AbstractVectorArray):
+            if src.type_abstract == dst.type_abstract:
+                components_src = src.components
+            else:
+                return NotImplemented
+        elif isinstance(src, na.AbstractScalar):
+            components_src = {c: src for c in components_dst}
+        else:
+            return NotImplemented
+    else:
+        components_src = {c: src for c in components_dst}
+
+    if isinstance(where, na.AbstractArray):
+        if isinstance(where, na.AbstractVectorArray):
+            if where.type_abstract == where.type_explicit:
+                components_where = where.components
+            else:
+                return NotImplemented
+        elif isinstance(where, na.AbstractScalar):
+            components_where = {c: where for c in components_dst}
+        else:
+            return NotImplemented
+    else:
+        components_where = {c: where for c in components_dst}
+
+    for c in components_dst:
+        try:
+            np.copyto(
+                dst=components_dst[c],
+                src=components_src[c],
+                casting=casting,
+                where=components_where[c],
+            )
+        except TypeError:
+            components_dst[c] = components_src[c]
+
+
 @implements(np.broadcast_to)
 def broadcast_to(
         array: na.AbstractVectorArray,
         shape: dict[str, int],
 ) -> na.AbstractExplicitVectorArray:
     components = array.components
     components_result = {c: na.broadcast_to(array=components[c], shape=shape) for c in components}
-    return array.type_array.from_components(components_result)
+    return array.type_explicit.from_components(components_result)
 
 
 @implements(np.transpose)
 def transpose(
         a: na.AbstractVectorArray,
         axes: None | Sequence[str] = None,
 ) -> na.AbstractExplicitVectorArray:
 
     components = a.broadcasted.components
-    return a.type_array.from_components({c: np.transpose(a=components[c], axes=axes) for c in components})
+    return a.type_explicit.from_components({c: np.transpose(a=components[c], axes=axes) for c in components})
 
 
 @implements(np.moveaxis)
 def moveaxis(
         a: na.AbstractVectorArray,
         source: str | Sequence[str],
         destination: str | Sequence[str],
@@ -343,28 +462,21 @@
         shape_c = na.shape(components[c])
         source_and_destination = tuple((src, dest) for src, dest in zip(source, destination) if src in shape_c)
         components_result[c] = np.moveaxis(
             a=components[c],
             source=tuple(src_and_dest[0] for src_and_dest in source_and_destination),
             destination=tuple(src_and_dest[1] for src_and_dest in source_and_destination),
         )
-    return a.type_array.from_components(components_result)
+    return a.type_explicit.from_components(components_result)
 
 
 @implements(np.reshape)
 def reshape(a: na.AbstractVectorArray, newshape: dict[str, int]) -> na.AbstractExplicitVectorArray:
     components = a.broadcasted.components
-    return a.type_array.from_components({c: np.reshape(a=components[c], newshape=newshape) for c in components})
-
-
-@implements(np.linalg.inv)
-def linalg_inv(a: na.AbstractVectorArray,):
-    raise NotImplementedError(
-        "np.linalg.inv not supported for instances of 'named_arrays.AbstractVectorArray'"
-    )
+    return a.type_explicit.from_components({c: np.reshape(a=components[c], newshape=newshape) for c in components})
 
 
 def array_function_stack_like(
         func: Callable,
         arrays: Sequence[bool | int | float | complex | str | u.Quantity | na.AbstractScalar | na.AbstractVectorArray],
         axis: str,
         out: None | na.AbstractExplicitVectorArray = None,
@@ -374,51 +486,51 @@
 ) -> na.AbstractExplicitVectorArray:
 
     for array in arrays:
         if isinstance(array, na.AbstractVectorArray):
             vector_prototype = array
             break
 
-    arrays = [vector_prototype.type_array.from_scalar(a) if not isinstance(a, na.AbstractVectorArray) else a
+    arrays = [vector_prototype.type_explicit.from_scalar(a) if not isinstance(a, na.AbstractVectorArray) else a
               for a in arrays]
     shape = na.shape_broadcasted(*arrays)
     arrays = [a.broadcast_to(shape) for a in arrays]
 
     components_arrays = [a.components for a in arrays]
 
     if out is None:
-        components_out = vector_prototype.type_array.from_scalar(out).components
+        components_out = vector_prototype.type_explicit.from_scalar(out, like=vector_prototype).components
     else:
         components_out = out.components
 
     components_result = dict()
     for c in components_arrays[0]:
         components_result[c] = func(
             arrays=[components[c] for components in components_arrays],
             axis=axis,
             out=components_out[c],
             dtype=dtype,
             casting=casting,
         )
 
     if out is None:
-        return vector_prototype.type_array.from_components(components_result)
+        return vector_prototype.type_explicit.from_components(components_result)
     else:
         return out
 
 
 @implements(np.sort)
 def sort(
         a: na.AbstractVectorArray,
         axis: None | str | Sequence[str],
         kind: None | str = None,
         order: None | str | list[str] = None,
 ) -> na.AbstractExplicitVectorArray:
 
-    a = a.array
+    a = a.explicit
     shape_a = a.shape
     components = a.components
 
     if axis is None:
         axis = tuple(shape_a)
         if not axis:
             return a
@@ -429,15 +541,15 @@
             raise ValueError(f"if `axis` is a sequence, it must not be empty, got {axis}")
 
     if not set(axis).issubset(shape_a):
         raise ValueError(f"`axis`, {axis} is not a subset of `a.axes`, {a.axes}")
 
     shape_base = {ax: shape_a[ax] for ax in axis}
 
-    result = a.type_array()
+    result = a.prototype_vector
     for c in components:
         component = na.as_named_array(components[c])
         if any(ax in axis for ax in component.axes):
             component = component.broadcast_to(na.broadcast_shapes(component.shape, shape_base))
             result.components[c] = np.sort(component, axis=axis, kind=kind, order=order)
         else:
             result.components[c] = components[c]
@@ -449,15 +561,15 @@
 def argsort(
         a: na.AbstractVectorArray,
         axis: None | str | Sequence[str],
         kind: None | str = None,
         order: None | str | list[str] = None,
 ) -> dict[str, na.AbstractExplicitVectorArray]:
 
-    a = a.array
+    a = a.explicit
     shape_a = a.shape
     components = a.components
 
     if axis is None:
         axis = tuple(shape_a)
         if not axis:
             return dict()
@@ -468,15 +580,15 @@
             raise ValueError(f"if `axis` is a sequence, it must not be empty, got {axis}")
 
     if not set(axis).issubset(shape_a):
         raise ValueError(f"`axis`, {axis} is not a subset of `a.axes`, {a.axes}")
 
     shape_base = {ax: shape_a[ax] for ax in axis}
 
-    result = {ax: a.type_array() for ax in shape_a}
+    result = {ax: a.prototype_vector for ax in shape_a}
     for c in components:
         component = na.as_named_array(components[c])
         if any(ax in axis for ax in component.axes):
             component = component.broadcast_to(na.broadcast_shapes(component.shape, shape_base))
             result_c = np.argsort(component, axis=axis, kind=kind, order=order)
         else:
             result_c = dict()
@@ -488,38 +600,38 @@
 
 @implements(np.unravel_index)
 def unravel_index(
         indices: na.AbstractVectorArray,
         shape: dict[str, int],
 ) -> dict[str, na.AbstractExplicitVectorArray]:
 
-    indices = indices.array
+    indices = indices.explicit
     components = indices.components
     result = {ax: dict() for ax in indices.axes}
 
     for c in components:
         result_c = np.unravel_index(
             indices=components[c],
             shape=shape,
         )
         for ax in result_c:
             result[ax][c] = result_c[ax]
 
-    result = {ax: indices.type_array.from_components(result[ax]) for ax in result}
+    result = {ax: indices.type_explicit.from_components(result[ax]) for ax in result}
     return result
 
 
 @implements(np.array_equal)
 def array_equal(
         a1: na.AbstractVectorArray,
         a2: na.AbstractVectorArray,
         equal_nan: bool = False,
 ) -> bool:
 
-    if not a1.type_array_abstract == a2.type_array_abstract:
+    if not a1.type_abstract == a2.type_abstract:
         return False
 
     components_a1 = a1.components
     components_a2 = a2.components
 
     result = True
     for c in components_a1:
@@ -534,15 +646,15 @@
 
 @implements(np.array_equiv)
 def array_equiv(
         a1: na.AbstractVectorArray,
         a2: na.AbstractVectorArray,
 ) -> bool:
 
-    if not a1.type_array_abstract == a2.type_array_abstract:
+    if not a1.type_abstract == a2.type_abstract:
         return False
 
     components_a1 = a1.components
     components_a2 = a2.components
 
     result = True
     for c in components_a1:
@@ -561,15 +673,15 @@
         rtol: float = 1e-05,
         atol: float = 1e-08,
         equal_nan: bool = False,
 ):
     if isinstance(a, na.AbstractVectorArray):
         components_a = a.components
         if isinstance(b, na.AbstractVectorArray):
-            if a.type_array_abstract == b.type_array_abstract:
+            if a.type_abstract == b.type_abstract:
                 components_b = b.components
             else:
                 return NotImplemented
         else:
             components_b = {c: b for c in components_a}
     else:
         if isinstance(b, na.AbstractVectorArray):
@@ -589,15 +701,15 @@
         )
 
     return result
 
 
 @implements(np.nonzero)
 def nonzero(a: na.AbstractVectorArray):
-    a = a.array
+    a = a.explicit
     components = a.components
 
     components_accumulated = True
     for c in components:
         components_accumulated = components_accumulated & components[c]
 
     return np.nonzero(components_accumulated)
@@ -620,12 +732,12 @@
             copy=copy,
             nan=nan,
             posinf=posinf,
             neginf=neginf,
         )
 
     if copy:
-        return x.type_array.from_components(components_result)
+        return x.type_explicit.from_components(components_result)
     else:
         if not isinstance(x, na.AbstractExplicitArray):
             raise ValueError("can't write to an array that is not an instance of `named_array.AbstractExplictArray`")
         return x
```

### Comparing `named_arrays-0.1.4/named_arrays/core.py` & `named_arrays-0.1.5/named_arrays/_core.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 import numpy as np
 import numpy.typing as npt
 import astropy.units as u
 import named_arrays as na
 
 __all__ = [
     'QuantityLike',
+    'StartT',
+    'StopT',
     'get_dtype',
+    'value',
     'unit',
     'unit_normalized',
     'type_array',
     'broadcast_shapes',
     'shape_broadcasted',
     'ndindex',
     'indices',
     'flatten_axes',
     'axis_normalized',
+    'explicit',
     'AbstractArray',
     'ArrayLike',
     'AbstractExplicitArray',
     'AbstractImplicitArray',
     'AbstractRandomMixin',
     'AbstractRangeMixin',
     'AbstractSymmetricRangeMixin',
@@ -41,14 +45,24 @@
     'AbstractUniformRandomSample',
     'AbstractNormalRandomSample',
     'AbstractPoissonRandomSample',
 ]
 
 QuantityLike = Union[int, float, complex, np.ndarray, u.Quantity]
 
+AxisT = TypeVar("AxisT", bound="str | AbstractArray")
+NumT = TypeVar("NumT", bound="int | AbstractArray")
+StartT = TypeVar("StartT", bound="QuantityLike | AbstractArray")
+StopT = TypeVar("StopT", bound="QuantityLike | AbstractArray")
+CenterT = TypeVar("CenterT", bound="QuantityLike | AbstractArray")
+WidthT = TypeVar("WidthT", bound="QuantityLike | AbstractArray")
+StartExponentT = TypeVar("StartExponentT", bound="QuantityLike | AbstractArray")
+StopExponentT = TypeVar("StopExponentT", bound="QuantityLike | AbstractArray")
+BaseT = TypeVar("BaseT", bound="QuantityLike | AbstractArray")
+
 
 def get_dtype(
         value: bool | int | float | complex | str | np.ndarray | AbstractArray,
 ) -> np.dtype:
     """
     Get the equivalent :attr:`numpy.ndarray.dtype` of the argument.
 
@@ -72,14 +86,35 @@
             return value.dtype
         else:
             raise ValueError("non-scalar instances of `na.AbstractArray` may not be represented by a single dtype")
     else:
         return np.array(value).dtype
 
 
+def value(a: float | u.Quantity | AbstractArray):
+    """
+    Remove the units (if they exist) from the input.
+
+    Parameters
+    ----------
+    a
+        A numeric value that may or may not have associated units
+
+    Returns
+    -------
+        The same numeric value, but guaranteed to be dimensionless.
+    """
+
+    if isinstance(a, AbstractArray):
+        return a.value
+    elif isinstance(a, u.Quantity):
+        return a.value
+    else:
+        return a
+
 def unit(
         value: float | complex | np.ndarray | u.UnitBase | u.Quantity | AbstractArray
 ) -> None | u.UnitBase:
     if isinstance(value, u.UnitBase):
         return value
     elif isinstance(value, u.Quantity):
         return value.unit
@@ -105,15 +140,15 @@
 def type_array(
         *values: bool | int | float | complex | str | np.ndarray | u.Quantity | AbstractArray,
 ) -> Type[AbstractExplicitArray]:
     cls = None
     priority_max = 0
     for value in values:
         if isinstance(value, AbstractArray):
-            cls_tmp = value.type_array
+            cls_tmp = value.type_explicit
             priority_tmp = cls_tmp.__named_array_priority__
             if priority_tmp > priority_max:
                 priority_max = priority_tmp
                 cls = cls_tmp
     return cls
 
 
@@ -188,14 +223,34 @@
     elif isinstance(axis, str):
         result = axis,
     else:
         result = tuple(axis)
     return result
 
 
+def explicit(value: Any | AbstractArray):
+    """
+    Converts an array to its explicit version if possible.
+
+    Parameters
+    ----------
+    value
+        any value or an instance of :class:`AbstractArray`
+
+    Returns
+    -------
+        If an instance of :class:`AbstractArray`, returns :attr:`AbstractArray.explicit` otherwise just returns the
+        input value.
+    """
+    if isinstance(value, AbstractArray):
+        return value.explicit
+    else:
+        return value
+
+
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractArray(
     np.lib.mixins.NDArrayOperatorsMixin,
     abc.ABC,
 ):
     """
     The ultimate parent class for all array types defined in this package.
@@ -210,22 +265,22 @@
         Similar to :attr:`numpy.class.__array_priority__`
 
         :return: :type:`int` describing this class's array priority
         """
 
     @property
     @abc.abstractmethod
-    def type_array_abstract(self: Self) -> Type[AbstractArray]:
+    def type_abstract(self: Self) -> Type[AbstractArray]:
         """
         The :class:`AbstractArray` type corresponding to this array
         """
 
     @property
     @abc.abstractmethod
-    def type_array(self: Self) -> Type[AbstractExplicitArray]:
+    def type_explicit(self: Self) -> Type[AbstractExplicitArray]:
         """
         The :class:`AbstractExplicitArray` type corresponding to this array
         """
 
     @property
     @abc.abstractmethod
     def axes(self: Self) -> tuple[str, ...]:
@@ -264,15 +319,22 @@
     def size(self: Self) -> int:
         """
         Total number of elements in the array. Equivalent to :attr:`numpy.ndarray.size`
         """
 
     @property
     @abc.abstractmethod
-    def array(self: Self) -> AbstractExplicitArray:
+    def value(self: Self) -> Self:
+        """
+        Returns a new array with its units removed, if they exist
+        """
+
+    @property
+    @abc.abstractmethod
+    def explicit(self: Self) -> AbstractExplicitArray:
         """
         Converts this array to an instance of :class:`named_arrays.AbstractExplicitArray`
         """
 
     @property
     @abc.abstractmethod
     def centers(self: Self) -> AbstractArray:
@@ -365,38 +427,73 @@
             The name of the new axis
 
         Returns
         -------
         Array with the specified axes combined
         """
 
-    def to_string(self, prefix: None | str = None):
-        pre = " " * len(prefix) if prefix is not None else ""
-        tab = " " * 4
+    def to_string(
+            self,
+            prefix: None | str = None,
+            multiline: None | bool = None,
+    ):
+        """
+        Convert this array instance to a string representation.
+
+        Parameters
+        ----------
+        prefix
+            the length of this string is used to align the output
+        multiline
+            flag which controls if the output should be spread over multiple
+            lines.
+
+        Returns
+        -------
+        array represented as a :class:`str`
+        """
         fields = dataclasses.fields(self)
-        result = f"{pre}{self.__class__.__qualname__}(\n"
-        for f in fields:
-            line = f"{pre}{tab}{f.name}="
+
+        if multiline is None:
+            multiline_normalized = any(isinstance(getattr(self, f.name), (np.ndarray, na.AbstractArray)) for f in fields)
+        else:
+            multiline_normalized = multiline
+
+        if multiline_normalized:
+            delim_field = "\n"
+            pre = " " * len(prefix) if prefix is not None else ""
+            tab = " " * 4
+        else:
+            delim_field = " "
+            pre = tab = ""
+
+        result = f"{self.__class__.__qualname__}("
+        if multiline_normalized:
+            result += "\n"
+
+        for i, f in enumerate(fields):
+            field_str = f"{pre}{tab}{f.name}="
             val = getattr(self, f.name)
             if isinstance(val, AbstractArray):
-                val_str = val.to_string(prefix=line)
+                val_str = val.to_string(prefix=f"{pre}{tab}", multiline=multiline)
             elif isinstance(val, np.ndarray):
                 val_str = np.array2string(
                     a=val,
                     separator=", ",
-                    prefix=line,
+                    prefix=field_str,
                 )
                 if isinstance(val, u.Quantity):
                     val_str = f"{val_str} {val.unit}"
             else:
                 val_str = repr(val)
-            line += val_str
-            line += ",\n"
-            result += line
-        result += ")"
+            field_str += val_str
+            if multiline_normalized or i < (len(fields) - 1):
+                field_str += f",{delim_field}"
+            result += field_str
+        result += f"{pre})"
         return result
 
     def __repr__(self):
         return self.to_string()
 
     def copy_shallow(self: Self) -> Self:
         return copy.copy(self)
@@ -509,14 +606,20 @@
         from . import _core_array_functions
 
         if func in _core_array_functions.HANDLED_FUNCTIONS:
             return _core_array_functions.HANDLED_FUNCTIONS[func](*args, **kwargs)
 
         return NotImplemented
 
+    def __named_array_function__(self, func, *args, **kwargs):
+        """
+        Method used to dispatch custom named array functions
+        """
+        return NotImplemented
+
     def broadcast_to(
             self: Self,
             shape: dict[str, int],
     ) -> Self:
         return np.broadcast_to(self, shape=shape)
 
     def reshape(
@@ -726,88 +829,53 @@
 ArrayLike = Union[QuantityLike, AbstractArray]
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractExplicitArray(
     AbstractArray,
 ):
-    @classmethod
-    @abc.abstractmethod
-    def empty(cls: Type[Self], shape: dict[str, int], dtype: Type = float) -> Self:
-        """
-        Create a new empty array
-
-        Parameters
-        ----------
-        shape
-            shape of the new array
-        dtype
-            data type of the new array
-
-        Returns
-        -------
-            A new empty array with the specified shape and data type
-        """
-
-    @classmethod
-    @abc.abstractmethod
-    def zeros(cls: Type[Self], shape: dict[str, int], dtype: Type = float) -> Self:
-        """
-        Create a new array of zeros
 
-        Parameters
-        ----------
-        shape
-            shape of the new array
-        dtype
-            data type of the new array
-
-        Returns
-        -------
-            A new array of zeros with the specified shape and data type
-        """
-
-    @classmethod
     @abc.abstractmethod
-    def ones(cls: Type[Self], shape: dict[str, int], dtype: Type = float) -> Self:
-        """
-        Create a new array of ones
-
-        Parameters
-        ----------
-        shape
-            shape of the new array
-        dtype
-            data type of the new array
-
-        Returns
-        -------
-            A new array of ones with the specified shape and data type
-        """
+    def __setitem__(
+            self,
+            item,
+            value,
+    ) -> None:
+        pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractImplicitArray(
     AbstractArray,
 ):
     @property
     def axes(self: Self) -> tuple[str, ...]:
-        return self.array.axes
+        return self.explicit.axes
 
     @property
     def ndim(self: Self) -> int:
-        return self.array.ndim
+        return self.explicit.ndim
 
     @property
     def size(self: Self) -> int:
-        return self.array.size
+        return self.explicit.size
+
+    @property
+    def value(self: Self) -> Self:
+        return self.explicit.value
 
     @property
     def shape(self: Self) -> dict[str, int]:
-        return self.array.shape
+        return self.explicit.shape
+
+    @abc.abstractmethod
+    def _attr_normalized(self, name: str) -> AbstractExplicitArray:
+        """
+        Similar to :func:`getattr`, but normalizes it to an instance of :class:`AbstractExplicitArray`
+        """
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractRandomMixin(
     abc.ABC,
 ):
 
@@ -897,36 +965,89 @@
         """
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractUniformRandomSample(
     AbstractRangeMixin,
     AbstractRandomSample,
+    Generic[StartT, StopT],
 ):
-    pass
+    start: StartT = dataclasses.MISSING
+    stop: StopT = dataclasses.MISSING
+    shape_random: None | dict[str, int] = None
+    seed: None | int = None
+
+    @property
+    def explicit(self) -> AbstractExplicitArray:
+
+        start = self._attr_normalized("start")
+        stop = self._attr_normalized("stop")
+
+        return na.random.uniform(
+            low=start,
+            high=stop,
+            shape_random=self.shape_random,
+            seed=self.seed,
+        )
+
+    @property
+    def centers(self: Self) -> Self:
+        return self
 
 
 @dataclasses.dataclass
 class AbstractNormalRandomSample(
     AbstractSymmetricRangeMixin,
     AbstractRandomSample,
+    Generic[CenterT, WidthT],
 ):
-    pass
+    center: CenterT = dataclasses.MISSING
+    width: WidthT = dataclasses.MISSING
+    shape_random: None | dict[str, int] = None
+    seed: None | int = None
+
+    @property
+    def explicit(self) -> AbstractExplicitArray:
+        center = self._attr_normalized("center")
+        width = self._attr_normalized("width")
+
+        return na.random.normal(
+            loc=center,
+            scale=width,
+            shape_random=self.shape_random,
+            seed=self.seed,
+        )
+
+    @property
+    def centers(self: Self) -> Self:
+        return self
+
 
 @dataclasses.dataclass
 class AbstractPoissonRandomSample(
     AbstractRandomSample,
+    Generic[CenterT],
 ):
+    center: CenterT = dataclasses.MISSING
+    shape_random: None | dict[str, int] = None
+    seed: None | int = None
 
     @property
-    @abc.abstractmethod
-    def center(self: Self) -> ArrayLike:
-        """
-        Center value of the range.
-        """
+    def explicit(self) -> AbstractExplicitArray:
+        center = self._attr_normalized("center")
+
+        return na.random.poisson(
+            lam=center,
+            shape_random=self.shape_random,
+            seed=self.seed,
+        )
+
+    @property
+    def centers(self: Self) -> Self:
+        return self
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractParameterizedArray(
     AbstractImplicitArray,
 ):
 
@@ -958,16 +1079,40 @@
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractArrayRange(
     AbstractLinearParameterizedArrayMixin,
     AbstractRangeMixin,
     AbstractParameterizedArray,
+    Generic[StartT, StopT]
 ):
-    pass
+    start: StartT = dataclasses.MISSING
+    stop: StopT = dataclasses.MISSING
+    axis: str | na.AbstractArray= dataclasses.MISSING
+    step: int | float | na.AbstractArray = 1
+
+    @property
+    def explicit(self: Self) -> AbstractExplicitArray:
+        start = self._attr_normalized("start")
+        stop = self._attr_normalized("stop")
+
+        return na.arange(
+            start=start,
+            stop=stop,
+            axis=self.axis,
+            step=self.step,
+        )
+
+    @property
+    def centers(self: Self) -> Self:
+        return self
+
+    @property
+    def num(self: Self) -> int:
+        return np.ceil((self.stop - self.start) / self.step).astype(int)
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractSpace(
     AbstractParameterizedArray,
 ):
     @property
@@ -978,68 +1123,133 @@
         """
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractLinearSpace(
     AbstractLinearParameterizedArrayMixin,
     AbstractRangeMixin,
-    AbstractSpace
+    AbstractSpace,
+    Generic[StartT, StopT, AxisT, NumT],
 ):
+    start: StartT = dataclasses.MISSING
+    stop: StopT = dataclasses.MISSING
+    axis: AxisT = dataclasses.MISSING
+    num: NumT = 11
+    endpoint: bool = True
+
+    @property
+    def explicit(self: Self) -> AbstractExplicitArray:
+        return na.linspace(
+            start=self._attr_normalized("start"),
+            stop=self._attr_normalized("stop"),
+            axis=self.axis,
+            num=self.num,
+            endpoint=self.endpoint
+        )
+
+    @property
+    def centers(self: Self) -> Self:
+        return self
 
     @property
     def step(self: Self) -> AbstractArray:
         if self.endpoint:
             return self.range / (self.num - 1)
         else:
             return self.range / self.num
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractStratifiedRandomSpace(
     AbstractRandomMixin,
-    AbstractLinearSpace,
+    AbstractLinearSpace[StartT, StopT, AxisT, NumT],
 ):
-    pass
+    seed: None | int = None
+
+    @property
+    def explicit(self: Self) -> AbstractExplicitArray:
+        result = self.centers
+
+        step_size = self.step
+
+        delta = na.random.uniform(
+            low=-step_size / 2,
+            high=step_size / 2,
+            shape_random=result.shape,
+            seed=self.seed,
+        )
+
+        return result + delta
+
+    @property
+    def centers(self: Self) -> AbstractExplicitArray:
+        return na.linspace(
+            start=self._attr_normalized("start"),
+            stop=self._attr_normalized("stop"),
+            num=self.num,
+            endpoint=self.endpoint,
+            axis=self.axis,
+        )
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractLogarithmicSpace(
     AbstractRangeMixin,
     AbstractSpace,
+    Generic[StartExponentT, StopExponentT, BaseT, AxisT, NumT]
 ):
+    start_exponent: StartExponentT = dataclasses.MISSING
+    stop_exponent: StopExponentT = dataclasses.MISSING
+    base: BaseT = dataclasses.MISSING
+    axis: AxisT = dataclasses.MISSING
+    num: NumT = 11
+    endpoint: bool = True
+
+    @property
+    def explicit(self: Self) -> AbstractExplicitArray:
+        return na.logspace(
+            start=self._attr_normalized("start_exponent"),
+            stop=self._attr_normalized("stop_exponent"),
+            axis=self.axis,
+            num=self.num,
+            endpoint=self.endpoint,
+            base=self.base,
+        )
 
     @property
-    @abc.abstractmethod
-    def start_exponent(self: Self) -> ArrayLike:
-        """
-        Exponent of the starting value of the sequence.
-        """
-
-    @property
-    @abc.abstractmethod
-    def stop_exponent(self: Self) -> ArrayLike:
-        """
-        Exponent of the ending value of the sequence.
-        """
-
-    @property
-    @abc.abstractmethod
-    def base(self: Self) -> ArrayLike:
-        """
-        Base which is exponentiated by :attr:`start_exponent` and :attr:`stop_exponent`.
-        """
+    def centers(self: Self) -> Self:
+        return self
 
     @property
     def start(self: Self) -> ArrayLike:
         return self.base ** self.start_exponent
 
     @property
     def stop(self: Self) -> ArrayLike:
         return self.base ** self.stop_exponent
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractGeometricSpace(
     AbstractRangeMixin,
     AbstractSpace,
+    Generic[StartT, StopT, AxisT, NumT]
 ):
-    pass
+    start: StartT = dataclasses.MISSING
+    stop: StopT = dataclasses.MISSING
+    axis: AxisT = dataclasses.MISSING
+    num: NumT = 11
+    endpoint: bool = True
+
+    @property
+    def explicit(self: Self) -> AbstractExplicitArray:
+        return na.geomspace(
+            start=self._attr_normalized("start"),
+            stop=self._attr_normalized("stop"),
+            axis=self.axis,
+            num=self.num,
+            endpoint=self.endpoint,
+        )
+
+    @property
+    def centers(self: Self) -> Self:
+        return self
```

### Comparing `named_arrays-0.1.4/named_arrays/scalars/array_functions.py` & `named_arrays-0.1.5/named_arrays/_scalars/scalar_array_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 from __future__ import annotations
 from typing import Sequence, Callable, Type
 import numpy as np
 import astropy.units as u
 import named_arrays as na
+from . import scalars
 
 __all__ = [
+    'ARRAY_CREATION_LIKE_FUNCTIONS',
     'DEFAULT_FUNCTIONS',
     'PERCENTILE_LIKE_FUNCTIONS',
     'ARG_REDUCE_FUNCTIONS',
     'FFT_LIKE_FUNCTIONS',
     'FFTN_LIKE_FUNCTIONS',
     'HANDLED_FUNCTIONS',
 ]
-
+ARRAY_CREATION_LIKE_FUNCTIONS = [
+    np.empty_like,
+    np.zeros_like,
+    np.ones_like,
+]
+SEQUENCE_FUNCTIONS = [
+    np.linspace,
+    np.logspace,
+    np.geomspace,
+]
 DEFAULT_FUNCTIONS = [
     np.ndim,
     np.min,
     np.nanmin,
     np.max,
     np.nanmax,
     np.sum,
@@ -63,39 +74,101 @@
     np.fft.ifftn,
     np.fft.rfftn,
     np.fft.irfftn,
 ]
 HANDLED_FUNCTIONS = dict()
 
 
+def array_function_array_creation_like(
+        func: Callable,
+        prototype: na.AbstractScalarArray,
+        dtype: None | type | np.dtype = None,
+        order: str = "K",
+        subok: bool = True,
+        shape: dict[str, int] = None,
+):
+    if shape is None:
+        shape = prototype.shape
+
+    return prototype.type_explicit(
+        ndarray=func(
+            prototype.ndarray,
+            dtype=dtype,
+            order=order,
+            subok=subok,
+            shape=tuple(shape.values()),
+        ),
+        axes=tuple(shape.keys()),
+    )
+
+
+def array_function_sequence(
+        func: Callable,
+        *args: float | u.Quantity | na.AbstractScalarArray,
+        axis: str,
+        num: int = 50,
+        endpoint: bool = True,
+        dtype: None | type | np.dtype = None,
+        **kwargs: float | u.Quantity | na.AbstractScalarArray,
+):
+    try:
+        args = tuple(scalars._normalize(arg) for arg in args)
+        kwargs = {k: scalars._normalize(kwargs[k]) for k in kwargs}
+    except na.ScalarTypeError:
+        return NotImplemented
+
+    shape = na.shape_broadcasted(*args, *kwargs.values())
+
+    args = tuple(arg.ndarray_aligned(shape) for arg in args)
+    kwargs = {k: kwargs[k].ndarray_aligned(shape) for k in kwargs}
+
+    if isinstance(axis, na.AbstractArray):
+        if isinstance(axis, na.AbstractScalarArray):
+            axis = axis.ndarray
+        else:
+            return NotImplemented
+
+    return na.ScalarArray(
+        ndarray=func(
+            *args,
+            num=num,
+            endpoint=endpoint,
+            dtype=dtype,
+            axis=~0,
+            **kwargs,
+        ),
+        axes=tuple(shape) + (axis, ),
+    )
+
+
 def array_function_default(
         func: Callable,
         a: na.AbstractScalarArray,
         axis: None | str | Sequence[str] = None,
         dtype: type | np.dtype = np._NoValue,
         out: None | na.ScalarArray = None,
         keepdims: bool = False,
         initial: bool | int | float | complex | u.Quantity = np._NoValue,
         where: bool | na.AbstractScalarArray = np._NoValue,
 ):
-    a = a.array
+    a = a.explicit
     shape = na.shape_broadcasted(a, where)
 
     axis_normalized = na.axis_normalized(a, axis=axis)
 
     if axis is not None:
         if not set(axis_normalized).issubset(shape):
             raise ValueError(
                 f"the `axis` argument must be `None` or a subset of the broadcasted shape of `a` and `where`, "
                 f"got {axis} for `axis`, but `{shape} for `shape`"
             )
 
     if out is not None:
         if not isinstance(out, na.ScalarArray):
-            raise ValueError(f"`out` should be `None` or an instance of `{a.type_array}`, got `{type(out)}`")
+            raise ValueError(f"`out` should be `None` or an instance of `{a.type_explicit}`, got `{type(out)}`")
         axes_ndarray = out.axes
         if not keepdims:
             axes_ndarray = axes_ndarray + tuple(ax for ax in shape if ax not in out.axes)
     else:
         axes_ndarray = tuple(shape)
 
     kwargs = dict()
@@ -140,27 +213,41 @@
         axis: None | str | Sequence[str] = None,
         out: None | na.ScalarArray = None,
         overwrite_input: bool = np._NoValue,
         method: str = np._NoValue,
         keepdims: bool = False,
 ) -> na.ScalarArray:
 
-    a = a.array
+    if isinstance(a, na.AbstractArray):
+        if isinstance(a, na.AbstractScalarArray):
+            a = a.explicit
+        else:
+            return NotImplemented
+    else:
+        a = na.ScalarArray(a)
+
     axes_a = a.axes
 
     axis_normalized = na.axis_normalized(a, axis=axis)
 
     if axis is not None:
         if not set(axis_normalized).issubset(axes_a):
             raise ValueError(
                 f"the `axis` argument must be `None` or a subset of `a.axes`, "
                 f"got {axis} for `axis`, but `{a.axes} for `a.axes`"
             )
 
-    q = q.array if isinstance(q, na.AbstractArray) else na.ScalarArray(q)
+    if isinstance(q, na.AbstractArray):
+        if isinstance(q, na.AbstractScalarArray):
+            q = q.explicit
+        else:
+            return NotImplemented
+    else:
+        q = na.ScalarArray(q)
+
     axes_q = q.axes
 
     axis_union = set(a.axes) & set(q.axes)
     if axis_union:
         raise ValueError(f"'q' must not have any shared axes with 'a', but axes {axis_union} are shared")
 
     axes_result = axes_q + (tuple(ax for ax in axes_a if ax not in axis_normalized) if not keepdims else axes_a)
@@ -196,15 +283,15 @@
 
 def array_function_arg_reduce(
         func: Callable,
         a: na.AbstractScalarArray,
         axis: None | str | Sequence[str] = None,
 ) -> dict[str, na.ScalarArray]:
 
-    a = a.array
+    a = a.explicit
     shape_a = a.shape
 
     if axis is not None:
         if isinstance(axis, str):
             axis = (axis, )
         if not set(axis).issubset(a.axes):
             raise ValueError(f"Reduction axes {axis} are not a subset of the array axes {a.axes}")
@@ -257,15 +344,15 @@
         func: Callable,
         a: na.AbstractScalarArray,
         axes: dict[str, str],
         s: None | dict[str, int] = None,
         norm: str = "backward",
 ) -> na.ScalarArray:
 
-    a = a.array
+    a = a.explicit
     shape = a.shape
 
     if not all(ax in shape for ax in axes):
         raise ValueError(f"Not all transform axes {axes} are in input array shape {shape}")
 
     if s is None:
         s = {ax: shape[ax] for ax in axes}
@@ -288,14 +375,54 @@
     """Register an __array_function__ implementation for AbstractScalarArray objects."""
     def decorator(func):
         HANDLED_FUNCTIONS[numpy_function] = func
         return func
     return decorator
 
 
+@implements(np.copyto)
+def copyto(
+        dst: na.ScalarArray,
+        src: na.AbstractScalarArray,
+        casting: str = "same_kind",
+        where: bool | na.AbstractScalarArray = True,
+):
+
+    if not isinstance(dst, na.ScalarArray):
+        return NotImplemented
+
+    shape = dst.shape
+
+    if isinstance(src, na.AbstractArray):
+        if isinstance(src, na.AbstractScalarArray):
+            src_ndarray = src.ndarray_aligned(shape)
+        else:
+            return NotImplemented
+    else:
+        src_ndarray = src
+
+    if isinstance(where, na.AbstractArray):
+        if isinstance(where, na.AbstractScalarArray):
+            where_ndarray = where.ndarray_aligned(shape)
+        else:
+            return NotImplemented
+    else:
+        where_ndarray = where
+
+    try:
+        np.copyto(
+            dst=dst.ndarray,
+            src=src_ndarray,
+            casting=casting,
+            where=where_ndarray,
+        )
+    except TypeError:
+        dst.ndarray = src.ndarray
+
+
 @implements(np.broadcast_to)
 def broadcast_to(
         array: na.AbstractScalarArray,
         shape: dict[str, int],
 ):
     return na.ScalarArray(
         ndarray=np.broadcast_to(array.ndarray_aligned(shape), tuple(shape.values()), subok=True),
@@ -352,21 +479,14 @@
 def reshape(a: na.AbstractScalarArray, newshape: dict[str, int]) -> na.ScalarArray:
     return na.ScalarArray(
         ndarray=np.reshape(a.ndarray, tuple(newshape.values())),
         axes=tuple(newshape.keys()),
     )
 
 
-@implements(np.linalg.inv)
-def linalg_inv(a: na.AbstractScalarArray,):
-    raise NotImplementedError(
-        "np.linalg.inv not supported, use 'named_arrays.AbstractScalarArray.matrix_inverse()' instead"
-    )
-
-
 @implements(np.stack)
 def stack(
         arrays: Sequence[bool | int | float | complex | str | u.Quantity | na.AbstractScalarArray],
         axis: str,
         out: None | na.ScalarArray = None,
         *,
         dtype: str | np.dtype | Type = None,
@@ -411,19 +531,22 @@
         arrays: Sequence[bool | int | float | complex | str | u.Quantity | na.AbstractScalarArray],
         axis: str,
         out: None | na.ScalarArray = None,
         dtype: None | str | Type | np.dtype = None,
         casting: str = "same_kind",
 ) -> na.ScalarArray:
 
-    arrays = [na.ScalarArray(arr) if not isinstance(arr, na.AbstractArray) else arr for arr in arrays]
+    arrays = [na.ScalarArray(arr) if not isinstance(arr, na.AbstractArray) else arr.explicit for arr in arrays]
     for array in arrays:
         if not isinstance(array, na.AbstractScalarArray):
             return NotImplemented
 
+    if any(axis not in array.shape for array in arrays):
+        raise ValueError(f"axis '{axis}' must be present in all the input arrays, got {[a.axes for a in arrays]}")
+
     shapes = []
     for array in arrays:
         shape = array.shape
         shape[axis] = 1
         shapes.append(shape)
 
     shape_prototype = na.broadcast_shapes(*shapes)
@@ -464,15 +587,15 @@
 def sort(
         a: na.AbstractScalarArray,
         axis: None | str | Sequence[str],
         kind: None | str = None,
         order: None | str | list[str] = None,
 ) -> na.ScalarArray:
 
-    a = a.array
+    a = a.explicit
 
     if axis is not None:
         if isinstance(axis, str):
             axis = (axis, )
         else:
             axis = tuple(axis)
 
@@ -505,15 +628,15 @@
 def argsort(
         a: na.AbstractScalarArray,
         axis: None | str,
         kind: None | str = None,
         order: None | str | list[str] = None,
 ) -> dict[str, na.ScalarArray]:
 
-    a = a.array
+    a = a.explicit
     shape_a = a.shape
 
     if axis is not None:
         if isinstance(axis, str):
             axis = (axis, )
         else:
             axis = tuple(axis)
@@ -622,15 +745,15 @@
         atol=atol,
         equal_nan=equal_nan,
     )
 
 
 @implements(np.nonzero)
 def nonzero(a: na.AbstractScalarArray):
-    a = a.array
+    a = a.explicit
     if not a.shape:
         return dict()
     axes = a.axes
     axes_flattened = a.axes_flattened
     result = np.nonzero(a.ndarray)
     return {axes[r]: na.ScalarArray(result[r], axes=(axes_flattened, )) for r, _ in enumerate(result)}
```

### Comparing `named_arrays-0.1.4/named_arrays/scalars/core.py` & `named_arrays-0.1.5/named_arrays/_scalars/scalars.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import numpy as np
 import numpy.typing as npt
 import scipy.ndimage
 import astropy.units as u
 import named_arrays as na
 
 __all__ = [
+    'ScalarStartT',
+    'ScalarStopT',
+    'ScalarTypeError',
     'as_named_array',
     'AbstractScalar',
     'AbstractScalarArray',
     'ScalarLike',
     'ScalarArray',
     'AbstractImplicitScalarArray',
     'ScalarUniformRandomSample',
@@ -27,21 +30,40 @@
     'ScalarLogarithmicSpace',
     'ScalarGeometricSpace',
 ]
 
 NDArrayT = TypeVar('NDArrayT', bound=npt.ArrayLike)
 StartT = TypeVar('StartT', bound='ScalarLike')
 StopT = TypeVar('StopT', bound='ScalarLike')
+ScalarStartT = TypeVar('ScalarStartT', bound='ScalarLike')
+ScalarStopT = TypeVar('ScalarStopT', bound='ScalarLike')
 CenterT = TypeVar('CenterT', bound='ScalarLike')
 WidthT = TypeVar('WidthT', bound='ScalarLike')
 StartExponentT = TypeVar('StartExponentT', bound='ScalarLike')
 StopExponentT = TypeVar('StopExponentT', bound='ScalarLike')
 BaseT = TypeVar('BaseT', bound='ScalarLike')
 
 
+class ScalarTypeError(TypeError):
+    pass
+
+
+def _normalize(a: float | u.Quantity | na.AbstractScalarArray) -> na.AbstractScalarArray:
+
+    if isinstance(a, na.AbstractArray):
+        if isinstance(a, na.AbstractScalarArray):
+            result = a
+        else:
+            raise ScalarTypeError
+    else:
+        result = na.ScalarArray(a)
+
+    return result
+
+
 def as_named_array(value: bool | int | float | complex | str | u.Quantity | na.AbstractArray):
     if not isinstance(value, na.AbstractArray):
         return ScalarArray(value)
     else:
         return value
 
 
@@ -106,31 +128,38 @@
     AbstractScalar,
     Generic[NDArrayT],
 ):
 
     __named_array_priority__: ClassVar[int] = 1
 
     @property
-    def type_array_abstract(self: Self) -> Type[AbstractScalarArray]:
+    def type_abstract(self: Self) -> Type[AbstractScalarArray]:
         return AbstractScalarArray
 
     @property
-    def type_array(self: Self) -> Type[ScalarArray]:
+    def type_explicit(self: Self) -> Type[ScalarArray]:
         return ScalarArray
 
     @property
     @abc.abstractmethod
     def ndarray(self: Self) -> bool | int | float | complex | str | np.ndarray | u.Quantity:
         """
         Underlying data that is wrapped by this class.
 
         This is usually an instance of :class:`numpy.ndarray` or :class:`astropy.units.Quantity`, but it can also be a
         built-in python type such as a :class:`int`, :class:`float`, or :class:`bool`
         """
 
+    @property
+    def value(self: Self) -> ScalarArray:
+        return self.type_explicit(
+            ndarray=na.value(self.ndarray),
+            axes=self.axes,
+        )
+
     def astype(
             self: Self,
             dtype: str | np.dtype | Type,
             order: str = 'K',
             casting='unsafe',
             subok: bool = True,
             copy: bool = True,
@@ -372,14 +401,17 @@
             method,
             *inputs,
             **kwargs,
         )
         if result is not NotImplemented:
             return result
 
+        if function is np.matmul:
+            return NotImplemented
+
         nout = function.nout
 
         kwargs_ndarray = kwargs.copy()
 
         if "out" in kwargs_ndarray:
             out = kwargs_ndarray["out"]
             out_normalized = list()
@@ -449,33 +481,57 @@
             args: tuple,
             kwargs: dict[str, Any],
     ):
         result = super().__array_function__(func=func, types=types, args=args, kwargs=kwargs)
         if result is not NotImplemented:
             return result
 
-        from . import array_functions
+        from . import scalar_array_functions
+
+        if func in scalar_array_functions.ARRAY_CREATION_LIKE_FUNCTIONS:
+            return scalar_array_functions.array_function_array_creation_like(func, *args, **kwargs)
+
+        if func in scalar_array_functions.SEQUENCE_FUNCTIONS:
+            return scalar_array_functions.array_function_sequence(func, *args, **kwargs)
+
+        if func in scalar_array_functions.DEFAULT_FUNCTIONS:
+            return scalar_array_functions.array_function_default(func, *args, **kwargs)
+
+        if func in scalar_array_functions.PERCENTILE_LIKE_FUNCTIONS:
+            return scalar_array_functions.array_function_percentile_like(func, *args, **kwargs)
+
+        if func in scalar_array_functions.ARG_REDUCE_FUNCTIONS:
+            return scalar_array_functions.array_function_arg_reduce(func, *args, **kwargs)
+
+        if func in scalar_array_functions.FFT_LIKE_FUNCTIONS:
+            return scalar_array_functions.array_function_fft_like(func, *args, **kwargs)
+
+        if func in scalar_array_functions.FFTN_LIKE_FUNCTIONS:
+            return scalar_array_functions.array_function_fftn_like(func, *args, **kwargs)
+
+        if func in scalar_array_functions.HANDLED_FUNCTIONS:
+            return scalar_array_functions.HANDLED_FUNCTIONS[func](*args, **kwargs)
 
-        if func in array_functions.DEFAULT_FUNCTIONS:
-            return array_functions.array_function_default(func, *args, **kwargs)
+        return NotImplemented
 
-        if func in array_functions.PERCENTILE_LIKE_FUNCTIONS:
-            return array_functions.array_function_percentile_like(func, *args, **kwargs)
+    def __named_array_function__(self, func, *args, **kwargs):
+        result = super().__named_array_function__(func, *args, **kwargs)
+        if result is not NotImplemented:
+            return result
 
-        if func in array_functions.ARG_REDUCE_FUNCTIONS:
-            return array_functions.array_function_arg_reduce(func, *args, **kwargs)
+        from . import scalar_named_array_functions
 
-        if func in array_functions.FFT_LIKE_FUNCTIONS:
-            return array_functions.array_function_fft_like(func, *args, **kwargs)
+        if func in scalar_named_array_functions.RANDOM_FUNCTIONS:
+            return scalar_named_array_functions.random(func=func, *args, **kwargs)
 
-        if func in array_functions.FFTN_LIKE_FUNCTIONS:
-            return array_functions.array_function_fftn_like(func, *args, **kwargs)
+        if func in scalar_named_array_functions.PLT_PLOT_LIKE_FUNCTIONS:
+            return scalar_named_array_functions.plt_plot_like(func, *args, **kwargs)
 
-        if func in array_functions.HANDLED_FUNCTIONS:
-            return array_functions.HANDLED_FUNCTIONS[func](*args, **kwargs)
+        if func in scalar_named_array_functions.HANDLED_FUNCTIONS:
+            return scalar_named_array_functions.HANDLED_FUNCTIONS[func](*args, **kwargs)
 
         return NotImplemented
 
     def matrix_multiply(
             self: Self,
             other: AbstractScalar,
             axis_rows: str,
@@ -569,15 +625,15 @@
             d = self[{axis_rows: 1, axis_columns: 0}]
             e = self[{axis_rows: 1, axis_columns: 1}]
             f = self[{axis_rows: 1, axis_columns: 2}]
             g = self[{axis_rows: 2, axis_columns: 0}]
             h = self[{axis_rows: 2, axis_columns: 1}]
             i = self[{axis_rows: 2, axis_columns: 2}]
 
-            result = ScalarArray(ndarray=self.array.copy(), axes=self.axes.copy())
+            result = ScalarArray(ndarray=self.explicit.copy(), axes=self.axes.copy())
             result[{axis_rows_inverse: 0, axis_columns_inverse: 0}] = (e * i - f * h)
             result[{axis_rows_inverse: 0, axis_columns_inverse: 1}] = -(b * i - c * h)
             result[{axis_rows_inverse: 0, axis_columns_inverse: 2}] = (b * f - c * e)
             result[{axis_rows_inverse: 1, axis_columns_inverse: 0}] = -(d * i - f * g)
             result[{axis_rows_inverse: 1, axis_columns_inverse: 1}] = (a * i - c * g)
             result[{axis_rows_inverse: 1, axis_columns_inverse: 2}] = -(a * f - c * d)
             result[{axis_rows_inverse: 2, axis_columns_inverse: 0}] = (d * h - e * g)
@@ -701,28 +757,70 @@
         if getattr(self.ndarray, 'ndim', 0) != len(self.axes):
             raise ValueError('The number of axis names must match the number of dimensions.')
         if len(self.axes) != len(set(self.axes)):
             raise ValueError(f'Each axis name must be unique, got {self.axes}.')
 
     @classmethod
     def empty(cls: Type[Self], shape: dict[str, int], dtype: Type | np.dtype = float) -> Self:
+        """
+        Create a new empty array
+
+        Parameters
+        ----------
+        shape
+            shape of the new array
+        dtype
+            data type of the new array
+
+        Returns
+        -------
+            A new empty array with the specified shape and data type
+        """
         return cls(
             ndarray=np.empty(shape=tuple(shape.values()), dtype=dtype),
             axes=tuple(shape.keys()),
         )
 
     @classmethod
     def zeros(cls: Type[Self], shape: dict[str, int], dtype: Type | np.dtype = float) -> Self:
+        """
+        Create a new array of zeros
+
+        Parameters
+        ----------
+        shape
+            shape of the new array
+        dtype
+            data type of the new array
+
+        Returns
+        -------
+            A new array of zeros with the specified shape and data type
+        """
         return cls(
             ndarray=np.zeros(shape=tuple(shape.values()), dtype=dtype),
             axes=tuple(shape.keys()),
         )
 
     @classmethod
     def ones(cls: Type[Self], shape: dict[str, int], dtype: Type | np.dtype = float) -> Self:
+        """
+        Create a new array of ones
+
+        Parameters
+        ----------
+        shape
+            shape of the new array
+        dtype
+            data type of the new array
+
+        Returns
+        -------
+            A new array of ones with the specified shape and data type
+        """
         return cls(
             ndarray=np.ones(shape=tuple(shape.values()), dtype=dtype),
             axes=tuple(shape.keys()),
         )
 
     @property
     def shape(self: Self) -> dict[str, int]:
@@ -741,305 +839,223 @@
         return na.get_dtype(self.ndarray)
 
     @property
     def unit(self: Self) -> None | u.UnitBase:
         return na.unit(self.ndarray)
 
     @property
-    def array(self: Self) -> Self:
+    def explicit(self: Self) -> Self:
         return self
 
     @property
     def centers(self: Self) -> Self:
         return self
 
     def __setitem__(
             self: Self,
-            key: dict[str, int | slice | AbstractScalar] | AbstractScalar,
-            value: int | float | u.Quantity | AbstractScalar,
+            item: dict[str, int | slice | AbstractScalarArray] | AbstractScalarArray,
+            value: int | float | u.Quantity | AbstractScalarArray,
     ) -> None:
 
-        if not isinstance(value, AbstractScalar):
+        shape_self = self.shape
+
+        if isinstance(value, na.AbstractArray):
+            if isinstance(value, na.AbstractScalarArray):
+                value = value.explicit
+            else:
+                raise TypeError(
+                    f"if `value` is an instance of `AbstractArray`, it must be an instance of `AbstractScalarArray`, "
+                    f"got {type(value)}"
+                )
+        else:
             value = ScalarArray(value)
 
-        if isinstance(key, ScalarArray):
-            shape = self.shape_broadcasted(key)
-            self.ndarray_aligned(shape)[key.ndarray_aligned(shape)] = value.ndarray
+        if isinstance(item, AbstractScalarArray):
+
+            item = item.explicit
+            shape_item = item.shape
+
+            if not set(item.shape).issubset(shape_self):
+                raise ValueError(
+                    f"if `item` is an instance of `{na.AbstractArray.__name__}`, "
+                    f"`item.axes`, {item.axes}, should be a subset of `self.axes`, {self.axes}"
+                )
+
+            if shape_item:
+                axis_new = item.axes_flattened
+            else:
+                axis_new = "boolean"
+
+            axes_untouched = tuple(ax for ax in shape_self if ax not in shape_item)
+            axes_value = (axis_new, ) + axes_untouched
+            axes_self = tuple(shape_item) + axes_untouched
+
+            self.ndarray_aligned(axes_self)[item.ndarray] = value.ndarray_aligned(axes_value)
+
+        elif isinstance(item, dict):
+
+            if not set(item).issubset(shape_self):
+                raise ValueError(
+                    f"if `item` is a `{dict.__name__}`, the keys in `item`, {tuple(item)}, "
+                    f"must be a subset of `self.axes`, {self.axes}"
+                )
+
+            item_advanced = {ax: item[ax] for ax in item if na.shape(item[ax])}
+
+            shape_advanced = na.shape_broadcasted(*item_advanced.values())
+
+            axes_self = tuple(shape_advanced) + tuple(ax for ax in shape_self if ax not in shape_advanced)
+            axes_value = list(axes_self)
 
-        else:
-            key_casted = cast(dict[str, Union[int, slice, AbstractScalar]], key)
             index = [slice(None)] * self.ndim   # type: list[Union[int, slice, AbstractScalar]]
-            axes = list(self.axes)
-            for axis in key_casted:
-                item_axis = key_casted[axis]
-                if isinstance(item_axis, int):
-                    axes.remove(axis)
-                if isinstance(item_axis, ScalarArray):
-                    item_axis = item_axis.ndarray_aligned(self.shape_broadcasted(item_axis))
-                index[self.axes.index(axis)] = item_axis
+            for axis in item:
+                item_axis = item[axis]
+                if isinstance(item_axis, na.AbstractScalarArray):
+                    item_axis = item_axis.ndarray_aligned(shape_advanced)
+                elif isinstance(item_axis, slice):
+                    pass
+                elif isinstance(item_axis, int):
+                    if axis in value.shape:
+                        raise ValueError(f"`value` has an axis, '{axis}', that is set to an `int` in `item`")
+                    axes_value.remove(axis)
+                else:
+                    raise TypeError(
+                        f"if `item` is a `{dict}`, all its values must be an instance of an `{int}`, a `{slice}`,"
+                        f"or an {na.AbstractScalarArray.__name__}, got {type(item_axis).__name__} for key '{axis}'"
+                    )
+                index[axes_self.index(axis)] = item_axis
 
             if value.shape:
-                value = value.ndarray_aligned({axis: 1 for axis in axes})
+                value = value.ndarray_aligned(axes_value)
             else:
                 value = value.ndarray
 
-            self.ndarray[tuple(index)] = value
+            self.ndarray_aligned(axes_self)[tuple(index)] = value
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractImplicitScalarArray(
     AbstractScalarArray,
     na.AbstractImplicitArray,
 ):
 
     @property
     def ndarray(self: Self) -> na.QuantityLike:
-        return self.array.ndarray
+        return self.explicit.ndarray
 
     @property
     def dtype(self: Self) -> np.dtype:
-        return self.array.dtype
+        return self.explicit.dtype
 
     @property
     def unit(self: Self) -> None | u.Unit:
-        return self.array.unit
+        return self.explicit.unit
+
+    def _attr_normalized(self, name: str) -> ScalarArray:
+
+        attr = getattr(self, name)
+
+        if isinstance(attr, na.AbstractArray):
+            if isinstance(attr, na.AbstractScalarArray):
+                result = attr
+            else:
+                raise TypeError(
+                    f"if `{name}` is an instance of `AbstractArray`, it must be an instance of `AbstractScalarArray`, "
+                    f"got {type(attr)}"
+                )
+        else:
+            result = ScalarArray(attr)
+
+        return result
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractScalarRandomSample(
     AbstractImplicitScalarArray,
     na.AbstractRandomSample,
 ):
     pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class ScalarUniformRandomSample(
     AbstractScalarRandomSample,
-    na.AbstractUniformRandomSample,
-    Generic[StartT, StopT],
+    na.AbstractUniformRandomSample[ScalarStartT, ScalarStopT],
 ):
-    start: StartT = dataclasses.MISSING
-    stop: StopT = dataclasses.MISSING
-    shape_random: dict[str, int] = None
-    seed: None | int = None
-
-    @property
-    def array(self: Self) -> ScalarArray:
-        start = self.start
-        if not isinstance(start, na.AbstractArray):
-            start = ScalarArray(start)
-
-        stop = self.stop
-        if not isinstance(stop, na.AbstractArray):
-            stop = ScalarArray(stop)
-
-        shape_random = self.shape_random if self.shape_random is not None else dict()
-        shape = na.shape_broadcasted(start, stop) | shape_random
-
-        start = start.ndarray_aligned(shape)
-        stop = stop.ndarray_aligned(shape)
-
-        unit = None
-        if isinstance(start, u.Quantity):
-            unit = start.unit
-            start = start.value
-            stop = stop.to(unit).value
-
-        value = self._rng.uniform(
-            low=start,
-            high=stop,
-            size=tuple(shape.values()),
-        )
-
-        if unit is not None:
-            value = value << unit
-
-        return ScalarArray(
-            ndarray=value,
-            axes=tuple(shape.keys())
-        )
-
-    @property
-    def centers(self: Self) -> Self:
-        return self
+    pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class ScalarNormalRandomSample(
     AbstractScalarRandomSample,
-    na.AbstractNormalRandomSample,
-    Generic[CenterT, WidthT],
+    na.AbstractNormalRandomSample[CenterT, WidthT],
 ):
-    center: CenterT = dataclasses.MISSING
-    width: WidthT = dataclasses.MISSING
-    shape_random: None | dict[str, int] = None
-    seed: None | int = None
-
-    @property
-    def array(self: Self) -> ScalarArray:
-        center = self.center
-        if not isinstance(center, na.AbstractArray):
-            center = ScalarArray(center)
-
-        width = self.width
-        if not isinstance(width, na.AbstractArray):
-            width = ScalarArray(width)
-
-        shape_random = self.shape_random if self.shape_random is not None else dict()
-        shape = na.shape_broadcasted(center, width) | shape_random
-
-        center = center.ndarray_aligned(shape)
-        width = width.ndarray_aligned(shape)
-
-        unit = None
-        if isinstance(center, u.Quantity):
-            unit = center.unit
-            center = center.value
-            width = width.to(unit).value
-
-        value = self._rng.normal(
-            loc=center,
-            scale=width,
-            size=tuple(shape.values()),
-        )
-
-        if unit is not None:
-            value = value << unit
-
-        return ScalarArray(
-            ndarray=value,
-            axes=tuple(shape.keys())
-        )
-
-    @property
-    def centers(self: Self) -> Self:
-        return self
+    pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class ScalarPoissonRandomSample(
     AbstractScalarRandomSample,
-    na.AbstractPoissonRandomSample,
-    Generic[CenterT],
+    na.AbstractPoissonRandomSample[CenterT],
 ):
-    center: CenterT = dataclasses.MISSING
-    shape_random: None | dict[str, int] = None
-    seed: None | int = None
-
-    @property
-    def array(self: Self) -> ScalarArray:
-        center = self.center
-        if not isinstance(center, na.AbstractArray):
-            center = ScalarArray(center)
-
-        shape_random = self.shape_random if self.shape_random is not None else dict()
-        shape = na.shape_broadcasted(center) | shape_random
-
-        center = center.ndarray_aligned(shape)
-
-        unit = None
-        if isinstance(center, u.Quantity):
-            unit = center.unit
-            center = center.value
-
-        value = self._rng.poisson(
-            lam=center,
-            size=tuple(shape.values()),
-        )
-
-        if unit is not None:
-            value = value << unit
-
-        return ScalarArray(
-            ndarray=value,
-            axes=tuple(shape.keys())
-        )
-
-    @property
-    def centers(self: Self) -> Self:
-        return self
+    pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractParameterizedScalarArray(
     AbstractImplicitScalarArray,
     na.AbstractParameterizedArray,
 ):
     pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class ScalarArrayRange(
     AbstractParameterizedScalarArray,
-    na.AbstractArrayRange,
-    Generic[StartT, StopT],
+    na.AbstractArrayRange[ScalarStartT, ScalarStopT],
 ):
     """
     An :class:`AbstractScalarArray` over the range [:attr:`start`, :attr:`stop`) incremented by :attr:`step`.
     An analog to :func:`numpy.arange`.
 
     :class:`ScalarArrayRange` can be used to create a :class:`ScalarArray` of integers.
 
     .. jupyter-execute::
 
         import named_arrays as na
         x = na.ScalarArrayRange(1, 8, axis = "x")
-        print(x.array)
+        print(x.explicit)
         print(x.shape)
 
     Note above that ``x`` does not include :attr:`stop`, and won't in almost all cases.  :class:`ScalarArrayRange` can be used to
     create an increasing :class:`ScalarArray` of floats, even with non integer steps.
 
     .. jupyter-execute::
 
         x = na.ScalarArrayRange(-0.5, 3, "x", 0.25)
-        print(x.array)
+        print(x.explicit)
 
     For the above, and more complicated uses, it is recommended to use :class:`ScalarLinearSpace` instead.  See numpy
     documentation of :func:`numpy.arange` for more info.
     """
-    start: StartT = dataclasses.MISSING
-    stop: StopT = dataclasses.MISSING
-    axis: str = dataclasses.MISSING
-    step: int = 1
-
-    @property
-    def array(self: Self) -> ScalarArray:
-        return ScalarArray(
-            ndarray=np.arange(
-                start=self.start,
-                stop=self.stop,
-                step=self.step,
-            ),
-            axes=(self.axis, ),
-        )
-
-    @property
-    def centers(self: Self) -> Self:
-        return self
-
-    @property
-    def num(self: Self) -> int:
-        return int(np.ceil((self.stop - self.start) / self.step))
+    pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractScalarSpace(
     AbstractParameterizedScalarArray,
     na.AbstractSpace,
 ):
     pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class ScalarLinearSpace(
     AbstractScalarSpace,
-    na.AbstractLinearSpace,
-    Generic[StartT, StopT],
+    na.AbstractLinearSpace[StartT, StopT, str, int],
 ):
     """
     An evenly spaced :class:`ScalarArray` ranging from start to stop with num elements.
 
     Most often, instances of :class:`ScalarArray` won't be formed directly from a :class:`numpy.ndarray`, but through
     more useful routines like :class:`ScalarLinearSpace`, a named_arrays equivalent to :func:`numpy.linspace`.
     For example, one can quickly create an evenly spaced coordinate (or axis) array with units.
@@ -1056,43 +1072,14 @@
     Then easily convert that into a wavelength.
 
     .. jupyter-execute::
 
         wavelength = (1240 * u.eV * u.nm / photon_energy).to(u.nm)
         print(wavelength)
     """
-    start: StartT = dataclasses.MISSING
-    stop: StopT = dataclasses.MISSING
-    axis: str = dataclasses.MISSING
-    num: int = 11
-    endpoint: bool = True
-
-    @property
-    def array(self: Self) -> ScalarArray:
-        start = self.start
-        if not isinstance(start, AbstractScalar):
-            start = ScalarArray(start)
-        stop = self.stop
-        if not isinstance(stop, AbstractScalar):
-            stop = ScalarArray(stop)
-        shape = na.shape_broadcasted(start, stop)
-        return ScalarArray(
-            ndarray=np.linspace(
-                start=start.ndarray_aligned(shape),
-                stop=stop.ndarray_aligned(shape),
-                num=self.num,
-                endpoint=self.endpoint,
-                axis=~0,
-            ),
-            axes=tuple(shape.keys()) + (self.axis, )
-        )
-
-    @property
-    def centers(self: Self) -> Self:
-        return self
 
     # def index(
     #         self: ScalarLinearSpaceT,
     #         value: ScalarLinearSpaceT,
     #         axis: None | str | Sequence[str] = None,
     # ) -> dict[str, ScalarArrayT]:
     #     result = super().index(
@@ -1132,132 +1119,30 @@
                 start=self.start.interp_linear(item),
                 stop=self.stop.interp_linear(item),
                 num=self.num,
                 endpoint=self.endpoint,
                 axis=self.axis,
             )
 
-#
-# @dataclasses.dataclass(eq=False, repr=False)
-# class _RandomSpaceMixin(_SpaceMixin):
-#
-#     seed: typ.Optional[int] = None
-#
-#     def __post_init__(self):
-#         if self.seed is None:
-#             self.seed = random.randint(0, 10 ** 12)
-#
-#     @property
-#     def _rng(self: _RandomSpaceMixinT) -> np.random.Generator:
-#         return np.random.default_rng(seed=self.seed)
-
 
 @dataclasses.dataclass(eq=False, repr=False)
 class ScalarStratifiedRandomSpace(
     ScalarLinearSpace[StartT, StopT],
-    na.AbstractStratifiedRandomSpace,
+    na.AbstractStratifiedRandomSpace[StartT, StopT, str, int],
 ):
-    seed: None | int = None
-
-    @property
-    def array(self: Self) -> ScalarArray:
-        result = self.centers
-
-        step_size = self.step
-
-        delta = ScalarUniformRandomSample(
-            start=-step_size / 2,
-            stop=step_size / 2,
-            shape_random=result.shape,
-            seed=self.seed,
-        )
-
-        return result + delta
-
-    @property
-    def centers(self: Self) -> ScalarLinearSpace:
-        return ScalarLinearSpace(
-            start=self.start,
-            stop=self.stop,
-            num=self.num,
-            endpoint=self.endpoint,
-            axis=self.axis,
-        )
+    pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class ScalarLogarithmicSpace(
     AbstractScalarSpace,
-    na.AbstractLogarithmicSpace,
-    Generic[StartExponentT, StopExponentT, BaseT]
+    na.AbstractLogarithmicSpace[StartExponentT, StopExponentT, BaseT, str, int],
 ):
-    start_exponent: StartExponentT = dataclasses.MISSING
-    stop_exponent: StopExponentT = dataclasses.MISSING
-    base: BaseT = dataclasses.MISSING
-    axis: str = dataclasses.MISSING
-    num: int = 11
-    endpoint: bool = True
-
-    @property
-    def array(self: Self) -> ScalarArray:
-        start_exponent = self.start_exponent
-        if not isinstance(start_exponent, AbstractScalar):
-            start_exponent = ScalarArray(start_exponent)
-        stop_exponent = self.stop_exponent
-        if not isinstance(stop_exponent, AbstractScalar):
-            stop_exponent = ScalarArray(stop_exponent)
-        base = self.base
-        if not isinstance(base, AbstractScalar):
-            base = ScalarArray(base)
-        shape = na.shape_broadcasted(start_exponent, stop_exponent, base)
-        return ScalarArray(
-            ndarray=np.logspace(
-                start=start_exponent.ndarray_aligned(shape),
-                stop=stop_exponent.ndarray_aligned(shape),
-                num=self.num,
-                endpoint=self.endpoint,
-                base=base.ndarray_aligned(shape | {self.axis: 1}),
-                axis=~0,
-            ),
-            axes=tuple(shape.keys()) + (self.axis, )
-        )
-
-    @property
-    def centers(self: Self) -> Self:
-        return self
+    pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class ScalarGeometricSpace(
     AbstractScalarSpace,
-    na.AbstractGeometricSpace,
-    Generic[StartT, StopT],
+    na.AbstractGeometricSpace[StartT, StopT, str, int],
 ):
-    start: StartT = dataclasses.MISSING
-    stop: StopT = dataclasses.MISSING
-    axis: str = dataclasses.MISSING
-    num: int = 11
-    endpoint: bool = True
-
-    @property
-    def array(self: Self) -> ScalarArray:
-        start = self.start
-        if not isinstance(start, AbstractScalar):
-            start = ScalarArray(start)
-        stop = self.stop
-        if not isinstance(stop, AbstractScalar):
-            stop = ScalarArray(stop)
-        shape = na.shape_broadcasted(start, stop)
-        return ScalarArray(
-            ndarray=np.geomspace(
-                start=start.ndarray_aligned(shape),
-                stop=stop.ndarray_aligned(shape),
-                num=self.num,
-                endpoint=self.endpoint,
-                axis=~0,
-            ),
-            axes=tuple(shape.keys()) + (self.axis, )
-        )
-
-    @property
-    def centers(self: Self) -> Self:
-        return self
+    pass
```

### Comparing `named_arrays-0.1.4/named_arrays/scalars/tests/test_core.py` & `named_arrays-0.1.5/named_arrays/_scalars/tests/test_scalars.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,25 +60,25 @@
 
 
 class AbstractTestAbstractScalar(
     tests.test_core.AbstractTestAbstractArray,
 ):
 
     def test_dtype(self, array: na.AbstractScalar):
-        assert array.dtype == array.array.dtype
+        assert array.dtype == array.explicit.dtype
         assert isinstance(array.dtype, np.dtype)
 
     def test_unit(self, array: na.AbstractScalar):
-        assert array.unit == array.array.unit
+        assert array.unit == array.explicit.unit
         unit = array.unit
         if unit is not None:
             assert isinstance(unit, u.UnitBase)
 
     def test_unit_normalized(self, array: na.AbstractScalar):
-        assert array.unit_normalized == array.array.unit_normalized
+        assert array.unit_normalized == array.explicit.unit_normalized
         if array.unit is None:
             assert array.unit_normalized == u.dimensionless_unscaled
         else:
             assert array.unit_normalized == array.unit
 
     @pytest.mark.parametrize('dtype', [int, float])
     def test_astype(self, array: na.AbstractScalar, dtype: Type):
@@ -140,50 +140,14 @@
             out = 0 * result
             result_out = np.matmul(array, array_2, out=out)
 
             assert np.all(result == result_expected)
             assert np.all(result == result_out)
             assert result_out is out
 
-    def test_ptp(
-            self,
-            array: na.AbstractScalar,
-    ):
-        super().test_ptp(array=array)
-        if np.issubdtype(array.dtype, bool):
-            with pytest.raises(TypeError, match='numpy boolean subtract, .*'):
-                array.ptp()
-            return
-
-        assert np.all(array.ptp() == np.ptp(array))
-
-    def test_all(
-            self,
-            array: na.AbstractScalar,
-    ):
-        super().test_all(array=array)
-        if array.unit is not None:
-            with pytest.raises(TypeError, match="no implementation found for .*"):
-                array.all()
-            return
-
-        assert np.all(array.all() == np.all(array))
-
-    def test_any(
-            self,
-            array: na.AbstractScalar,
-    ):
-        super().test_any(array=array)
-        if array.unit is not None:
-            with pytest.raises(TypeError, match="no implementation found for .*"):
-                array.any()
-            return
-
-        assert np.all(array.any() == np.any(array))
-
 
 class AbstractTestAbstractScalarArray(
     AbstractTestAbstractScalar,
 ):
 
     def test_ndarray(self, array: na.AbstractScalarArray):
         assert isinstance(array.ndarray, (int, float, complex, str, np.ndarray))
@@ -192,14 +156,24 @@
         super().test_axes(array)
         assert len(array.axes) == np.ndim(array.ndarray)
 
     def test_size(self, array: na.AbstractScalarArray):
         super().test_size(array)
         assert array.size == np.size(array.ndarray)
 
+    @pytest.mark.parametrize('index', [1, ~0])
+    def test_change_axis_index(self, array: na.ScalarArray, index: int):
+        axis = 'x'
+        if axis in array.axes:
+            result = array.change_axis_index(axis, index)
+            assert result.axes.index(axis) == (index % array.ndim)
+        else:
+            with pytest.raises(KeyError):
+                array.change_axis_index(axis, index)
+
     @pytest.mark.parametrize(
         argnames='item',
         argvalues=[
             dict(y=0),
             dict(y=slice(0,1)),
             dict(y=na.ScalarArray(np.array([0, 1]), axes=('y', ))),
             na.ScalarLinearSpace(0, 1, axis='y', num=_num_y) > 0.5,
@@ -357,17 +331,17 @@
                     ufunc(array, **kwargs)
                 return
 
             result = ufunc(array, **kwargs)
             result_ndarray = ufunc(array.ndarray, **kwargs_ndarray)
 
             if ufunc.nout == 1:
-                out = 0 * result
+                out = 0 * np.nan_to_num(result)
             else:
-                out = tuple(0 * r for r in result)
+                out = tuple(0 * np.nan_to_num(r) for r in result)
 
             result_out = ufunc(array, out=out, **kwargs)
 
             if ufunc.nout == 1:
                 out = (out, )
                 result_ndarray = (result_ndarray, )
                 result = (result, )
@@ -522,37 +496,37 @@
                 out = 0 * result
                 result_out = func(array, out=out, **kwargs)
 
                 assert np.all(result.ndarray == result_ndarray)
                 assert np.allclose(result, result_out)
                 assert result_out is out
 
-        @pytest.mark.parametrize(
-            argnames='q',
-            argvalues=[
-                .25,
-                25 * u.percent,
-                na.ScalarLinearSpace(.25, .75, axis='q', num=3, endpoint=True),
-            ]
-        )
         class TestPercentileLikeFunctions(
             AbstractTestAbstractScalar.TestArrayFunctions.TestPercentileLikeFunctions
         ):
 
+            @pytest.mark.parametrize(
+                argnames='q',
+                argvalues=[
+                    .25,
+                    25 * u.percent,
+                    na.ScalarLinearSpace(.25, .75, axis='q', num=3, endpoint=True),
+                ]
+            )
             def test_percentile_like_functions(
                     self,
                     func: Callable,
                     array: na.AbstractScalarArray,
                     q: float | u.Quantity | na.AbstractArray,
                     axis: None | str | Sequence[str],
                     keepdims: bool,
             ):
                 super().test_percentile_like_functions(
                     func=func,
-                    array=array.array,
+                    array=array.explicit,
                     q=q,
                     axis=axis,
                     keepdims=keepdims,
                 )
 
                 kwargs = dict(
                     q=q,
@@ -588,14 +562,52 @@
                 out = 0 * result
                 result_out = func(array, out=out, **kwargs)
 
                 assert np.all(result.ndarray == result_ndarray)
                 assert np.allclose(result, result_out)
                 assert result_out is out
 
+            @pytest.mark.parametrize(
+                argnames="q",
+                argvalues=[
+                    na.UncertainScalarArray(
+                        nominal=25 * u.percent,
+                        distribution=na.ScalarNormalRandomSample(
+                            center=25 * u.percent,
+                            width=1 * u.percent,
+                            shape_random=dict(_distribution=_num_distribution)
+                        )
+                    ),
+                    na.NormalUncertainScalarArray(
+                        nominal=na.ScalarLinearSpace(25 * u.percent, 75 * u.percent, axis='y', num=_num_y),
+                        width=1 * u.percent,
+                        num_distribution=_num_distribution,
+                    )
+                ]
+            )
+            def test_percentile_like_functions_q_uncertain(
+                    self,
+                    func: Callable,
+                    array: na.AbstractScalarArray,
+                    q: float | u.Quantity | na.AbstractArray,
+                    axis: None | str | Sequence[str],
+                    keepdims: bool,
+            ):
+                from named_arrays._scalars.uncertainties.tests.test_uncertainties import (
+                    AbstractTestAbstractUncertainScalarArray
+                )
+                other = AbstractTestAbstractUncertainScalarArray.TestArrayFunctions.TestPercentileLikeFunctions()
+                other.test_percentile_like_functions(
+                    func=func,
+                    array=array,
+                    q=q,
+                    axis=axis,
+                    keepdims=keepdims,
+                )
+
         class TestFFTLikeFunctions(
             AbstractTestAbstractScalar.TestArrayFunctions.TestFFTLikeFunctions
         ):
 
             def test_fft_like_functions(
                     self,
                     func: Callable,
@@ -778,57 +790,102 @@
                 v.ndarray if isinstance(v, na.AbstractArray) else v,
                 mode=mode,
             )
 
             assert result.axes == tuple(shape_broadcasted.keys())
             assert np.all(result.ndarray == result_expected)
 
+    class TestNamedArrayFunctions(
+        tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions
+    ):
+        @pytest.mark.parametrize(
+            argnames="array_2",
+            argvalues=_scalar_arrays_2(),
+        )
+        @pytest.mark.parametrize(
+            argnames="where",
+            argvalues=[
+                np._NoValue,
+                True,
+                na.linspace(0, 1, axis="x", num=_num_x) > 0.5,
+            ]
+        )
+        @pytest.mark.parametrize(
+            argnames="alpha",
+            argvalues=[
+                np._NoValue,
+                na.linspace(0, 1, axis="x", num=_num_x),
+            ]
+        )
+        class TestPltPlotLikeFunctions(
+            tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestPltPlotLikeFunctions,
+        ):
+            pass
+
 
 @pytest.mark.parametrize('array', _scalar_arrays())
 class TestScalarArray(
     AbstractTestAbstractScalarArray,
     tests.test_core.AbstractTestAbstractExplicitArray,
 ):
-    @pytest.mark.parametrize('index', [1, ~0])
-    def test_change_axis_index(self, array: na.ScalarArray, index: int):
-        axis = 'x'
-        if axis in array.axes:
-            result = array.change_axis_index(axis, index)
-            assert result.axes.index(axis) == (index % array.ndim)
-        else:
-            with pytest.raises(KeyError):
-                array.change_axis_index(axis, index)
 
+    @pytest.mark.parametrize(
+        argnames="item",
+        argvalues=[
+            dict(y=0),
+            dict(x=0, y=0),
+            dict(y=slice(None)),
+            dict(y=na.ScalarArrayRange(0, _num_y, axis='y')),
+            dict(x=na.ScalarArrayRange(0, _num_x, axis='x'), y=na.ScalarArrayRange(0, _num_y, axis='y')),
+            na.ScalarArray.ones(shape=dict(y=_num_y), dtype=bool),
+        ],
+    )
+    @pytest.mark.parametrize(
+        argnames="value",
+        argvalues=[
+            0,
+            na.ScalarUniformRandomSample(-5, 5, dict(y=_num_y)),
+        ]
+    )
+    def test__setitem__(
+            self,
+            array: na.ScalarArray,
+            item: dict[str, int | slice | na.ScalarArray] | na.ScalarArray,
+            value: float | na.ScalarArray
+    ):
+        super().test__setitem__(array=array, item=item, value=value)
 
-class TestScalarArrayCreation(
-    tests.test_core.AbstractTestAbstractExplicitArrayCreation
-):
+
+@pytest.mark.parametrize('shape', [dict(x=3), dict(x=4, y=5)])
+@pytest.mark.parametrize('dtype', [int, float, complex])
+class TestScalarArrayCreation:
 
     @property
     def type_array(self) -> Type[na.ScalarArray]:
         return na.ScalarArray
 
     def test_empty(self, shape: dict[str, int], dtype: Type):
-        super().test_empty(shape=shape, dtype=dtype)
         result = self.type_array.empty(shape, dtype=dtype)
+        assert result.shape == shape
         assert result.dtype == dtype
 
     def test_zeros(self, shape: dict[str, int], dtype: Type):
-        super().test_zeros(shape=shape, dtype=dtype)
         result = self.type_array.zeros(shape, dtype=dtype)
+        assert result.shape == shape
+        assert np.all(result == 0)
         assert result.dtype == dtype
 
     def test_ones(self, shape: dict[str, int], dtype: Type):
-        super().test_ones(shape=shape, dtype=dtype)
         result = self.type_array.ones(shape, dtype=dtype)
+        assert result.shape == shape
+        assert np.all(result == 1)
         assert result.dtype == dtype
 
 
 class AbstractTestAbstractImplicitScalarArray(
-    AbstractTestAbstractScalarArray,
     tests.test_core.AbstractTestAbstractImplicitArray,
 ):
     pass
 
 
 class AbstractTestAbstractScalarRandomSample(
     AbstractTestAbstractImplicitScalarArray,
@@ -975,15 +1032,17 @@
         ) for start in starts for stop in stops for unit in units for endpoint in endpoints
     ]
 
 
 @pytest.mark.parametrize('array', _scalar_linear_spaces())
 class TestScalarLinearSpace(
     AbstractTestAbstractScalarSpace,
+    AbstractTestAbstractScalarArray,
     tests.test_core.AbstractTestAbstractLinearSpace,
+    tests.test_core.AbstractTestAbstractArray,
 ):
     pass
 
 def _scalar_stratified_random_spaces():
     starts = [
         0,
         na.ScalarArray(np.random.random(_num_x), axes=('x', )),
@@ -1023,15 +1082,14 @@
     ]
     stop_exponents = [
         2,
         na.ScalarArray(np.random.random(_num_x) + 2, axes=('x', )),
     ]
     bases = [
         2,
-        na.ScalarArray(np.random.random(_num_x) + 1, axes=('x',)),
     ]
     endpoints = [
         False,
         True,
     ]
     return [
         na.ScalarLogarithmicSpace(
@@ -1079,206 +1137,7 @@
 
 @pytest.mark.parametrize('array', _scalar_geometric_spaces())
 class TestScalarGeometricSpace(
     AbstractTestAbstractScalarSpace,
     tests.test_core.AbstractTestAbstractGeometricSpace,
 ):
     pass
-
-
-# class OldTestScalarArray:
-#     def test__post_init__(self):
-#         with pytest.raises(ValueError):
-#             na.ScalarArray(ndarray=np.empty((2, 3)) * u.dimensionless_unscaled, axes=['x'])
-#
-#     def test_shape(self):
-#         shape = dict(x=2, y=3)
-#         a = na.ScalarArray(
-#             ndarray=np.random.random(tuple(shape.values())) * u.dimensionless_unscaled,
-#             axes=['x', 'y'],
-#         )
-#         assert a.shape == shape
-#
-#     def test_shape_broadcasted(self):
-#         shape = dict(x=5, y=6)
-#         d1 = na.ScalarArray.empty(dict(x=shape['x'], y=1))
-#         d2 = na.ScalarArray.empty(dict(y=shape['y'], x=1))
-#         assert d1.shape_broadcasted(d2) == shape
-#
-#     def test_ndarray_aligned(self):
-#         shape = dict(x=5, y=6, z=7)
-#         d = na.ScalarArray.empty(dict(z=shape['z']))
-#         assert d.ndarray_aligned(shape).shape == (1, 1, shape['z'])
-#
-#     def test_combine_axes(self):
-#         shape = dict(x=5, y=6, z=7)
-#         a = na.ScalarArray.zeros(shape).combine_axes(['x', 'y'])
-#         assert a.shape == dict(z=shape['z'], xy=shape['x'] * shape['y'])
-#
-#     def test__array_ufunc__(self):
-#         shape = dict(x=100, y=101)
-#         a = na.ScalarArray(
-#             ndarray=np.random.random(shape['x']),
-#             axes=['x'],
-#         )
-#         b = na.ScalarArray(
-#             ndarray=np.random.random(shape['y']),
-#             axes=['y'],
-#         )
-#         c = a + b
-#         assert c.shape == shape
-#         assert (c.ndarray == a.ndarray[..., np.newaxis] + b.ndarray).all()
-#
-#     def test__array_ufunc__incompatible_dims(self):
-#         a = na.ScalarArray(
-#             ndarray=np.random.random(10),
-#             axes=['x'],
-#         )
-#         b = na.ScalarArray(
-#             ndarray=np.random.random(11),
-#             axes=['x'],
-#         )
-#         with pytest.raises(ValueError):
-#             a + b
-#
-#     @pytest.mark.parametrize(
-#         argnames='a,b',
-#         argvalues=[
-#             (na.ScalarArray(5), 6),
-#             (na.ScalarArray(5 * u.mm), 6 * u.mm),
-#
-#             (na.ScalarLinearSpace(0, 1, num=11, axis='x'), 6),
-#             (na.ScalarLinearSpace(0, 1, num=11, axis='x') * u.mm, 6 * u.mm),
-#             (na.ScalarLinearSpace(0, 1, num=11, axis='x') * u.mm, na.ScalarLinearSpace(0, 1, num=11, axis='x') * u.mm),
-#         ],
-#     )
-#     def test__add__(self, a: na.ScalarLike, b: na.ScalarLike):
-#         c = a + b
-#         d = b + a
-#         b_normalized = b
-#         if not isinstance(b, na.AbstractArray):
-#             b_normalized = na.ScalarArray(b)
-#         assert isinstance(c, na.AbstractArray)
-#         assert isinstance(d, na.AbstractArray)
-#         assert np.all(c.ndarray == a.ndarray + b_normalized.ndarray)
-#         assert np.all(d.ndarray == b_normalized.ndarray + a.ndarray)
-#         assert np.all(c == d)
-#
-#     def test__mul__unit(self):
-#         a = na.ScalarUniformRandomSpace(0, 1, axis='x', num=10,) * u.mm
-#         assert isinstance(a, na.AbstractArray)
-#         assert isinstance(a.ndarray, u.Quantity)
-#
-#     def test__mul__float(self):
-#         a = na.ScalarUniformRandomSpace(0, 1, axis='x', num=10,)
-#         b = 2.
-#         c = a * b
-#         assert isinstance(c, na.Array)
-#         assert c.ndarray.mean() > a.ndarray.mean()
-#
-#     def test__mul__ndarray(self):
-#         shape = dict(x=10)
-#         a = na.ScalarUniformRandomSpace(0, 1, axis='x', num=shape['x'])
-#         b = np.ones(shape['x'])
-#         with pytest.raises(ValueError):
-#             a * b
-#
-#     def test__array_function__broadcast_to(self):
-#         shape = dict(x=5, y=6)
-#         a = na.ScalarLinearSpace(1, 5, axis='y', num=shape['y'])
-#         b = np.broadcast_to(a, shape)
-#         c = np.broadcast_to(a, shape=shape)
-#         d = np.broadcast_to(array=a, shape=shape)
-#         assert np.all(b == c)
-#         assert np.all(b == d)
-#
-#     def test__array_function__stack(self):
-#         a = na.ScalarLinearSpace(0, 1, num=11, axis='x')
-#         b = na.ScalarLinearSpace(2, 3, num=11, axis='x')
-#         c = na.ScalarLinearSpace(3, 4, num=11, axis='x')
-#         result = np.stack([a, b, c], axis='y')
-#         assert np.all(result.ndarray == np.stack([a.ndarray, b.ndarray, c.ndarray]))
-#
-#     def test__array_function__sum(self):
-#         shape = dict(x=4, y=7)
-#         a = np.sum(na.ScalarArray.ones(shape))
-#         assert a.ndarray == shape['x'] * shape['y']
-#         assert a.shape == dict()
-#
-#     def test__array_function__sum_axis(self):
-#         shape = dict(x=4, y=7)
-#         a = np.sum(na.ScalarArray.ones(shape), axis='x')
-#         assert (a.ndarray == shape['x']).all()
-#         assert a.shape == dict(y=shape['y'])
-#
-#     def test__array_function__sum_keepdims(self):
-#         shape = dict(x=4, y=7)
-#         a = np.sum(na.ScalarArray.ones(shape), keepdims=True)
-#         assert a.ndarray[0, 0] == shape['x'] * shape['y']
-#         assert a.shape == dict(x=1, y=1)
-#
-#     @pytest.mark.parametrize(
-#         argnames='a, shift',
-#         argvalues=[
-#             (na.ScalarLinearSpace(0, 1, num=11, axis='x'), 1),
-#             (na.ScalarLinearSpace(0, 1, num=11, axis='x') * na.ScalarLinearSpace(0, 1, num=11, axis='y'), 1),
-#         ],
-#     )
-#     def test__array_function__roll(self, a: na.AbstractScalarArray, shift: int):
-#         b = np.roll(a, shift, axis='x')
-#         assert np.all(b.ndarray == np.roll(a.ndarray, shift, axis=0))
-#
-#     def test__getitem__int(self):
-#         a = na.ScalarRange(stop=10, axis='x')
-#         b = na.ScalarRange(stop=11, axis='y')
-#         c = na.ScalarRange(stop=5, axis='z')
-#         d = a * b * c
-#         index = dict(x=1, y=1)
-#         assert (d[index].ndarray == c.ndarray).all()
-#         assert d[index].shape == c.shape
-#
-#     def test__getitem__slice(self):
-#         a = na.ScalarRange(stop=10, axis='x')
-#         b = na.ScalarRange(stop=11, axis='y')
-#         c = na.ScalarRange(stop=5, axis='z')
-#         d = a * b * c
-#         index = dict(x=slice(1, 2), y=slice(1, 2))
-#         assert (d[index].ndarray == c.ndarray).all()
-#         assert d[index].shape == dict(x=1, y=1, z=d.shape['z'])
-#
-#     def test__getitem__advanced_bool(self):
-#         a = na.ScalarRange(stop=10, axis='x')
-#         b = na.ScalarRange(stop=11, axis='y')
-#         c = na.ScalarRange(stop=5, axis='z')
-#         d = a * b * c
-#         assert d[a > 5].shape == {**b.shape, **c.shape, **d[a > 5].shape}
-#
-#     def test_ndindex(self):
-#         shape = dict(x=2, y=2)
-#         result_expected = [{'x': 0, 'y': 0}, {'x': 0, 'y': 1}, {'x': 1, 'y': 0}, {'x': 1, 'y': 1}]
-#         a = na.ScalarArray.empty(shape)
-#         assert list(a.ndindex()) == result_expected
-#
-#     # def test_index_nearest_brute(self):
-#     #
-#     #     x = kgpy.labeled.LinearSpace(0, 1, num=5, axis='x')
-#     #     y = kgpy.labeled.LinearSpace(0, 1, num=5, axis='y')
-#     #     z = kgpy.labeled.LinearSpace(0, 1, num=5, axis='z')
-#     #     a = x + 10 * y + 100 * z
-#     #     index_nearest = a.index_nearest_brute(a, axis=('x', 'y'))
-#     #     indices = a.indices
-#     #
-#     #     for ax in indices:
-#     #         assert np.all(index_nearest[ax] == indices[ax])
-#     #
-#     # def test_index_nearest_secant(self):
-#     #
-#     #     x = na.ScalarLinearSpace(0, 1, num=5, axis='x')
-#     #     y = na.ScalarLinearSpace(0, 1, num=5, axis='y')
-#     #     # z = kgpy.labeled.LinearSpace(0, 1, num=5, axis='z')
-#     #     a = x + 10*y
-#     #     index_nearest = a.index_nearest_secant(a, axis='x')
-#     #     indices = a.indices
-#     #
-#     #     for ax in indices:
-#     #         assert np.all(index_nearest[ax] == indices[ax])
-
```

### Comparing `named_arrays-0.1.4/named_arrays/scalars/uncertainties/tests/test_uncertainties.py` & `named_arrays-0.1.5/named_arrays/_scalars/uncertainties/tests/test_uncertainties.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Type, Sequence, Callable
 import numpy as np
 import pytest
 import astropy.units as u
 import named_arrays as na
 import named_arrays.tests.test_core
-import named_arrays.scalars.tests.test_core
+import named_arrays._scalars.tests.test_scalars
 
 __all__ = [
     'AbstractTestAbstractUncertainScalarArray',
     'TestUncertainScalarArray',
-    'TestUncertainScalarArrayCreation',
     'AbstractTestAbstractImplicitUncertainScalarArray',
     'TestUniformUncertainScalarArray',
     'TestNormalUncertainScalarArray',
 ]
 
 _num_x = named_arrays.tests.test_core.num_x
 _num_y = named_arrays.tests.test_core.num_y
@@ -66,15 +65,15 @@
         for unit in units
     ]
     arrays = arrays_exact + arrays_uncertain
     return arrays
 
 
 class AbstractTestAbstractUncertainScalarArray(
-    named_arrays.scalars.tests.test_core.AbstractTestAbstractScalar,
+    named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar,
 ):
 
     def test_nominal(self, array: na.AbstractUncertainScalarArray):
         assert np.sum(array.nominal) != 0
         assert array.axis_distribution not in na.shape(array.nominal)
 
     def test_distribution(self, array: na.AbstractUncertainScalarArray):
@@ -194,15 +193,15 @@
         result = array / unit
         result_nominal = array.nominal / unit
         result_distribution = array.distribution / unit
         assert np.all(result.nominal == result_nominal)
         assert np.all(result.distribution == result_distribution)
 
     class TestUfuncUnary(
-        named_arrays.scalars.tests.test_core.AbstractTestAbstractScalar.TestUfuncUnary
+        named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestUfuncUnary
     ):
 
         def test_ufunc_unary(
                 self,
                 ufunc: np.ufunc,
                 array: na.AbstractUncertainScalarArray,
         ):
@@ -214,15 +213,15 @@
 
             unit = array.unit_normalized
             if ufunc in [np.log, np.log2, np.log10, np.sqrt]:
                 kwargs["where"] = array > 0
             elif ufunc in [np.log1p]:
                 kwargs["where"] = array >= (-1 * unit)
             elif ufunc in [np.arcsin, np.arccos, np.arctanh]:
-                kwargs["where"] = ((-1 * unit) <= array) & (array <= (1 * unit))
+                kwargs["where"] = ((-1 * unit) < array) & (array < (1 * unit))
             elif ufunc in [np.arccosh]:
                 kwargs["where"] = array >= (1 * unit)
             elif ufunc in [np.reciprocal]:
                 kwargs["where"] = array != 0
 
             if "where" in kwargs:
                 kwargs_nominal["where"] = kwargs["where"].nominal
@@ -258,15 +257,15 @@
                 assert np.all(result[i].nominal == result_nominal[i], **kwargs_nominal)
                 assert np.all(result[i].distribution == result_distribution[i], **kwargs_distribution)
                 assert np.all(result[i] == result_out[i], **kwargs)
                 assert result_out[i] is out[i]
 
     @pytest.mark.parametrize('array_2', _uncertain_scalar_arrays_2())
     class TestUfuncBinary(
-        named_arrays.scalars.tests.test_core.AbstractTestAbstractScalar.TestUfuncBinary
+        named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestUfuncBinary
     ):
 
         def test_ufunc_binary(
                 self,
                 ufunc: np.ufunc,
                 array: None | bool | int | float | complex | na.AbstractUncertainScalarArray,
                 array_2: None | bool | int | float | complex | na.AbstractUncertainScalarArray,
@@ -313,17 +312,17 @@
 
             result = ufunc(array, array_2, **kwargs)
             result_nominal = ufunc(array_normalized.nominal, array_2_normalized.nominal, **kwargs_nominal)
             result_distribution = ufunc(
                 array_normalized.distribution, array_2_normalized.distribution, **kwargs_distribution)
 
             if ufunc.nout == 1:
-                out = 0 * result
+                out = 0 * np.nan_to_num(result)
             else:
-                out = tuple(0 * r for r in result)
+                out = tuple(0 * np.nan_to_num(r) for r in result)
 
             result_out = ufunc(array, array_2, out=out, **kwargs)
 
             if ufunc.nout == 1:
                 out = (out, )
                 result = (result, )
                 result_nominal = (result_nominal, )
@@ -334,20 +333,20 @@
                 assert np.all(result[i].nominal == result_nominal[i], **kwargs_nominal)
                 assert np.all(result[i].distribution == result_distribution[i], **kwargs_distribution)
                 assert np.all(result[i] == result_out[i], **kwargs)
                 assert result_out[i] is out[i]
 
     @pytest.mark.parametrize('array_2', _uncertain_scalar_arrays_2())
     class TestMatmul(
-        named_arrays.scalars.tests.test_core.AbstractTestAbstractScalar.TestMatmul
+        named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestMatmul
     ):
         pass
 
     class TestArrayFunctions(
-        named_arrays.scalars.tests.test_core.AbstractTestAbstractScalar.TestArrayFunctions,
+        named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestArrayFunctions,
     ):
 
         @pytest.mark.parametrize(
             argnames='where',
             argvalues=[
                 np._NoValue,
                 True,
@@ -359,15 +358,16 @@
                     distribution=(na.ScalarLinearSpace(-1, 1, 'x', _num_x) >= 0)
                                  | (na.ScalarLinearSpace(-1, 1, 'y', _num_y) >= 0)
                                  | (na.ScalarLinearSpace(-1, 1, '_distribution', _num_distribution) >= 0)
                 ),
             ]
         )
         class TestReductionFunctions(
-            named_arrays.scalars.tests.test_core.AbstractTestAbstractScalar.TestArrayFunctions.TestReductionFunctions,
+            named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestArrayFunctions.
+            TestReductionFunctions,
         ):
 
             def test_reduction_functions(
                     self,
                     func: Callable,
                     array: na.AbstractUncertainScalarArray,
                     axis: None | str | Sequence[str],
@@ -436,15 +436,16 @@
                         width=1 * u.percent,
                         shape_random=dict(_distribution=_num_distribution)
                     )
                 )
             ]
         )
         class TestPercentileLikeFunctions(
-            named_arrays.scalars.tests.test_core.AbstractTestAbstractScalar.TestArrayFunctions.TestPercentileLikeFunctions
+            named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestArrayFunctions.
+            TestPercentileLikeFunctions
         ):
 
             def test_percentile_like_functions(
                     self,
                     func: Callable,
                     array: na.AbstractUncertainScalarArray,
                     q: float | u.Quantity | na.AbstractArray,
@@ -455,14 +456,20 @@
                     func=func,
                     array=array,
                     q=q,
                     axis=axis,
                     keepdims=keepdims,
                 )
 
+                array_normalized = array
+                if isinstance(array, na.AbstractArray):
+                    if isinstance(array, na.AbstractScalar):
+                        if isinstance(array, na.AbstractScalarArray):
+                            array_normalized = na.UncertainScalarArray(array, array)
+
                 kwargs = dict(
                     q=q,
                     axis=axis,
                     keepdims=keepdims,
                 )
 
                 kwargs_nominal = kwargs.copy()
@@ -476,16 +483,16 @@
 
                 if axis is None:
                     axis_normalized = na.axis_normalized(array, axis)
                     kwargs_nominal["axis"] = axis_normalized
                     kwargs_distribution["axis"] = axis_normalized
 
                 try:
-                    result_nominal = func(array.broadcasted.nominal, **kwargs_nominal)
-                    result_distribution = func(array.broadcasted.distribution, **kwargs_distribution)
+                    result_nominal = func(array_normalized.broadcasted.nominal, **kwargs_nominal)
+                    result_distribution = func(array_normalized.broadcasted.distribution, **kwargs_distribution)
                 except (ValueError, TypeError) as e:
                     with pytest.raises(type(e)):
                         func(array, **kwargs)
                     return
 
                 result = func(array, **kwargs)
 
@@ -494,15 +501,15 @@
 
                 assert np.all(result.nominal == result_nominal)
                 assert np.all(result.distribution == result_distribution)
                 assert np.all(result == result_out)
                 assert result_out is out
 
         class TestFFTLikeFunctions(
-            named_arrays.scalars.tests.test_core.AbstractTestAbstractScalar.TestArrayFunctions.TestFFTLikeFunctions,
+            named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestArrayFunctions.TestFFTLikeFunctions,
         ):
 
             def test_fft_like_functions(
                     self,
                     func: Callable,
                     array: na.AbstractUncertainScalarArray,
                     axis: tuple[str, str],
@@ -516,15 +523,15 @@
                 result_nominal = func(array.broadcasted.nominal, axis=axis)
                 result_distribution = func(array.broadcasted.distribution, axis=axis)
 
                 assert np.all(result.nominal == result_nominal)
                 assert np.all(result.distribution == result_distribution)
 
         class TestFFTNLikeFunctions(
-            named_arrays.scalars.tests.test_core.AbstractTestAbstractScalar.TestArrayFunctions.TestFFTNLikeFunctions
+            named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestArrayFunctions.TestFFTNLikeFunctions
         ):
             def test_fftn_like_functions(
                     self,
                     func: Callable,
                     array: na.AbstractUncertainScalarArray,
                     axes: dict[str, str],
                     s: None | dict[str, int],
@@ -599,34 +606,81 @@
         @pytest.mark.parametrize('v', _uncertain_scalar_arrays_2())
         @pytest.mark.parametrize('mode', ['full', 'same', 'valid'])
         def test_convolve(self, array: na.AbstractArray, v: na.AbstractArray, mode: str):
             super().test_convolve(array=array, v=v, mode=mode)
             with pytest.raises(ValueError, match="`numpy.convolve` is not supported .*"):
                 np.convolve(array, v=v, mode=mode)
 
+    class TestNamedArrayFunctions(
+        named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions
+    ):
+        @pytest.mark.parametrize(
+            argnames="array_2",
+            argvalues=_uncertain_scalar_arrays_2(),
+        )
+        @pytest.mark.parametrize(
+            argnames="where",
+            argvalues=[
+                np._NoValue,
+                True,
+                na.linspace(0, 1, axis="x", num=_num_x) > 0.5,
+            ]
+        )
+        @pytest.mark.parametrize(
+            argnames="alpha",
+            argvalues=[
+                np._NoValue,
+                na.linspace(0, 1, axis="x", num=_num_x),
+            ]
+        )
+        class TestPltPlotLikeFunctions(
+            named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestPltPlotLikeFunctions,
+        ):
+            pass
+
 
 @pytest.mark.parametrize('array', _uncertain_scalar_arrays())
 class TestUncertainScalarArray(
     AbstractTestAbstractUncertainScalarArray,
     named_arrays.tests.test_core.AbstractTestAbstractExplicitArray
 ):
-    pass
-
 
-class TestUncertainScalarArrayCreation(
-    named_arrays.tests.test_core.AbstractTestAbstractExplicitArrayCreation,
-):
-
-    @property
-    def type_array(self) -> Type[na.UncertainScalarArray]:
-        return na.UncertainScalarArray
+    @pytest.mark.parametrize(
+        argnames="item",
+        argvalues=[
+            dict(y=0),
+            dict(x=0, y=0),
+            dict(y=slice(None)),
+            dict(y=na.ScalarArrayRange(0, _num_y, axis='y')),
+            dict(x=na.ScalarArrayRange(0, _num_x, axis='x'), y=na.ScalarArrayRange(0, _num_y, axis='y')),
+            na.ScalarArray.ones(shape=dict(y=_num_y), dtype=bool),
+        ],
+    )
+    @pytest.mark.parametrize(
+        argnames="value",
+        argvalues=[
+            0,
+            na.ScalarUniformRandomSample(-5, 5, dict(y=_num_y)),
+            na.UncertainScalarUniformRandomSample(
+                start=na.UniformUncertainScalarArray(-5, 0, num_distribution=_num_distribution),
+                stop=5,
+                shape_random=dict(y=_num_y),
+            )
+        ]
+    )
+    def test__setitem__(
+            self,
+            array: na.ScalarArray,
+            item: dict[str, int | slice | na.ScalarArray] | na.ScalarArray,
+            value: float | na.ScalarArray
+    ):
+        super().test__setitem__(array=array, item=item, value=value)
 
 
 class AbstractTestAbstractImplicitUncertainScalarArray(
-    AbstractTestAbstractUncertainScalarArray,
     named_arrays.tests.test_core.AbstractTestAbstractImplicitArray,
 ):
     pass
 
 
 def _uniform_uncertain_scalar_arrays():
     arrays_exact = [
@@ -651,14 +705,17 @@
     ]
     return arrays
 
 
 @pytest.mark.parametrize('array', _uniform_uncertain_scalar_arrays())
 class TestUniformUncertainScalarArray(
     AbstractTestAbstractImplicitUncertainScalarArray,
+    AbstractTestAbstractUncertainScalarArray,
+    named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar,
+    named_arrays.tests.test_core.AbstractTestAbstractArray,
 ):
     pass
 
 
 def _normal_uncertain_scalar_arrays():
     arrays_exact = [
         4,
@@ -684,7 +741,190 @@
 
 
 @pytest.mark.parametrize('array', _normal_uncertain_scalar_arrays())
 class TestNormalUncertainScalarArray(
     AbstractTestAbstractImplicitUncertainScalarArray,
 ):
     pass
+
+
+class AbstractTestAbstractUncertainScalarRandomSample(
+    AbstractTestAbstractImplicitUncertainScalarArray,
+    named_arrays.tests.test_core.AbstractTestAbstractRandomSample,
+):
+    pass
+
+
+def _uncertain_scalar_uniform_random_samples() -> tuple[na.UncertainScalarUniformRandomSample, ...]:
+
+    starts = (
+        na.UniformUncertainScalarArray(
+            na.ScalarLinearSpace(0, 1, axis='x', num=_num_x),
+            width=0.2,
+            num_distribution=_num_distribution,
+        ),
+    )
+    stops = (
+        2,
+        na.ScalarArray(2),
+        na.ScalarLinearSpace(2, 3, axis='x', num=_num_x),
+        na.UniformUncertainScalarArray(
+            na.ScalarLinearSpace(2, 3, axis='x', num=_num_x),
+            width=0.1,
+            num_distribution=_num_distribution,
+        ),
+    )
+    units = (1, u.mm)
+    arrays = tuple(
+        na.UncertainScalarUniformRandomSample(
+            start=start * unit,
+            stop=stop * unit,
+            shape_random=dict(y=_num_y),
+        )
+        for start in starts
+        for stop in stops
+        for unit in units
+    )
+    return arrays
+
+
+@pytest.mark.parametrize("array", _uncertain_scalar_uniform_random_samples())
+class TestUncertainScalarUniformRandomSample(
+    AbstractTestAbstractUncertainScalarRandomSample,
+    named_arrays.tests.test_core.AbstractTestAbstractUniformRandomSample,
+):
+    pass
+
+
+def _uncertain_scalar_normal_random_samples() -> tuple[na.UncertainScalarNormalRandomSample, ...]:
+
+    centers = (
+        na.UniformUncertainScalarArray(
+            na.ScalarLinearSpace(0, 1, axis='x', num=_num_x),
+            width=0.2,
+            num_distribution=_num_distribution,
+        ),
+    )
+    widths = (
+        2,
+        na.ScalarArray(2),
+        na.ScalarLinearSpace(2, 3, axis='x', num=_num_x),
+        na.UniformUncertainScalarArray(
+            na.ScalarLinearSpace(2, 3, axis='x', num=_num_x),
+            width=0.1,
+            num_distribution=_num_distribution,
+        ),
+    )
+    units = (1, u.mm)
+    arrays = tuple(
+        na.UncertainScalarNormalRandomSample(
+            center=center * unit,
+            width=width * unit,
+            shape_random=dict(y=_num_y),
+        )
+        for center in centers
+        for width in widths
+        for unit in units
+    )
+    return arrays
+
+
+@pytest.mark.parametrize("array", _uncertain_scalar_normal_random_samples())
+class TestUncertainScalarNormalmRandomSample(
+    AbstractTestAbstractUncertainScalarRandomSample,
+    named_arrays.tests.test_core.AbstractTestAbstractNormalRandomSample,
+):
+    pass
+
+
+def _uncertain_scalar_poisson_random_samples() -> tuple[na.UncertainScalarPoissionRandomSample, ...]:
+
+    centers = (
+        na.UniformUncertainScalarArray(2, width=0.1, num_distribution=_num_distribution),
+        na.UniformUncertainScalarArray(
+            na.ScalarLinearSpace(2, 3, axis='x', num=_num_x),
+            width=0.1,
+            num_distribution=_num_distribution,
+        ),
+    )
+    units = (1, u.mm)
+    arrays = tuple(
+        na.UncertainScalarPoissionRandomSample(
+            center=center * unit,
+            shape_random=dict(y=_num_y),
+        )
+        for center in centers
+        for unit in units
+    )
+    return arrays
+
+
+@pytest.mark.parametrize("array", _uncertain_scalar_poisson_random_samples())
+class TestUncertainScalarPoissonRandomSample(
+    AbstractTestAbstractUncertainScalarRandomSample,
+    named_arrays.tests.test_core.AbstractTestAbstractPoissonRandomSample,
+):
+    pass
+
+
+
+class AbstractTestAbstractParameterizedUncertainScalarArray(
+    AbstractTestAbstractImplicitUncertainScalarArray,
+    named_arrays.tests.test_core.AbstractTestAbstractParameterizedArray,
+):
+    pass
+
+
+class TestUncertainScalarLinearSpace(
+    AbstractTestAbstractUncertainScalarRandomSample,
+    named_arrays.tests.test_core.AbstractTestAbstractPoissonRandomSample,
+):
+    pass
+
+
+class AbstractTestAbstractScalarSpace(
+    AbstractTestAbstractParameterizedUncertainScalarArray,
+    named_arrays.tests.test_core.AbstractTestAbstractSpace,
+):
+    pass
+
+
+def _uncertain_scalar_linear_spaces() -> tuple[na.UncertainScalarLinearSpace, ...]:
+
+    starts = (
+        na.UniformUncertainScalarArray(
+            na.ScalarLinearSpace(0, 1, axis='x', num=_num_x),
+            width=0.2,
+            num_distribution=_num_distribution,
+        ),
+    )
+    stops = (
+        2,
+        na.ScalarArray(2),
+        na.ScalarLinearSpace(2, 3, axis='x', num=_num_x),
+        na.UniformUncertainScalarArray(
+            na.ScalarLinearSpace(2, 3, axis='x', num=_num_x),
+            width=0.1,
+            num_distribution=_num_distribution,
+        ),
+    )
+    units = (1, u.mm)
+    arrays = tuple(
+        na.UncertainScalarLinearSpace(
+            start=start * unit,
+            stop=stop * unit,
+            axis='y',
+            num=_num_y,
+        )
+        for start in starts
+        for stop in stops
+        for unit in units
+    )
+    return arrays
+
+
+@pytest.mark.parametrize("array", _uncertain_scalar_linear_spaces())
+class TestUncertainScalarLinearSpace(
+    AbstractTestAbstractScalarSpace,
+    named_arrays.tests.test_core.AbstractTestAbstractLinearSpace,
+):
+    pass
```

### Comparing `named_arrays-0.1.4/named_arrays/scalars/uncertainties/uncertainties.py` & `named_arrays-0.1.5/named_arrays/_scalars/uncertainties/uncertainties.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,48 +6,83 @@
 import dataclasses
 import numpy as np
 import astropy.units as u
 
 import named_arrays as na
 
 __all__ = [
+    'UncertainScalarStartT',
+    'UncertainScalarStopT',
+    'UncertainScalarTypeError',
     'AbstractUncertainScalarArray',
     'UncertainScalarArray',
     'UniformUncertainScalarArray',
     'NormalUncertainScalarArray',
+    'UncertainScalarUniformRandomSample',
+    'UncertainScalarNormalRandomSample',
+    'UncertainScalarPoissionRandomSample',
+    'AbstractParameterizedUncertainScalarArray',
+    'AbstractUncertainScalarSpace',
+    'UncertainScalarLinearSpace',
+    'UncertainScalarStratifiedRandomSpace',
+    'UncertainScalarLogarithmicSpace',
+    'UncertainScalarGeometricSpace',
 ]
 
 NominalArrayT = TypeVar(
     'NominalArrayT',
     bound=None | float | complex | np.ndarray | u.Quantity | na.AbstractScalarArray,
 )
 DistributionArrayT = TypeVar(
     'DistributionArrayT',
     bound=None | float | complex | np.ndarray | u.Quantity | na.AbstractScalarArray,
 )
 WidthT = TypeVar('WidthT', bound=int | float | np.ndarray | u.Quantity | na.AbstractScalarArray)
+UncertainScalarStartT = TypeVar("UncertainScalarStartT", bound=float | u.Quantity | na.AbstractScalar)
+UncertainScalarStopT = TypeVar("UncertainScalarStopT", bound=float | u.Quantity | na.AbstractScalar)
+UncertainScalarCenterT = TypeVar("UncertainScalarCenterT", bound=float | u.Quantity | na.AbstractScalar)
+UncertainScalarWidthT = TypeVar("UncertainScalarWidthT", bound=float | u.Quantity | na.AbstractScalar)
 
 _axis_distribution_default = "_distribution"
 _num_distribution_default = 11
 
 
+class UncertainScalarTypeError(TypeError):
+    pass
+
+
+def _normalize(a: float | u.Quantity | na.AbstractScalar):
+    if isinstance(a, na.AbstractArray):
+        if isinstance(a, na.AbstractScalar):
+            if isinstance(a, na.AbstractUncertainScalarArray):
+                result = a
+            else:
+                result = na.UncertainScalarArray(a, a)
+        else:
+            return UncertainScalarTypeError
+    else:
+        result = na.UncertainScalarArray(a, a)
+
+    return result
+
+
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractUncertainScalarArray(
     na.AbstractScalar
 ):
     __named_array_priority__: ClassVar[int] = 10 * na.AbstractScalarArray.__named_array_priority__
 
     axis_distribution: ClassVar[str] = "_distribution"
 
     @property
-    def type_array(self) -> Type[UncertainScalarArray]:
+    def type_explicit(self) -> Type[UncertainScalarArray]:
         return UncertainScalarArray
 
     @property
-    def type_array_abstract(self) -> Type[AbstractUncertainScalarArray]:
+    def type_abstract(self) -> Type[AbstractUncertainScalarArray]:
         return AbstractUncertainScalarArray
 
     @property
     @abc.abstractmethod
     def nominal(self) -> float | complex | u.Quantity | na.AbstractScalarArray:
         """
         Nominal value of the array.
@@ -75,21 +110,23 @@
     def dtype(self) -> np.dtype:
         return np.promote_types(
             na.get_dtype(self.nominal),
             na.get_dtype(self.distribution),
         )
 
     @property
-    def unit(self: Self) -> None | u.Unit:
-        return na.unit(self.nominal)
+    def value(self) -> UncertainScalarArray:
+        return self.type_explicit(
+            nominal=na.value(self.nominal),
+            distribution=na.value(self.distribution),
+        )
 
     @property
-    @abc.abstractmethod
-    def array(self) -> UncertainScalarArray[na.ScalarArray, na.ScalarArray]:
-        pass
+    def unit(self: Self) -> None | u.Unit:
+        return na.unit(self.nominal)
 
     def astype(
             self,
             dtype: str | np.dtype | Type,
             order: str = 'K',
             casting='unsafe',
             subok: bool = True,
@@ -145,23 +182,23 @@
             distribution=distribution.combine_axes(axes=axes, axis_new=axis_new),
         )
 
     def _getitem(
             self,
             item: dict[str, int | slice | na.AbstractScalar] | na.AbstractScalar,
     ):
-        array = self.array
+        array = self.explicit
         shape_array = array.shape
         shape_array_distribution = array.shape_distribution
 
         nominal = na.as_named_array(array.nominal)
         distribution = na.as_named_array(array.distribution)
 
         if isinstance(item, na.AbstractArray):
-            item = item.array
+            item = item.explicit
             if isinstance(item, AbstractUncertainScalarArray):
                 item_nominal = item_distribution = item.nominal & np.all(item.distribution, axis=self.axis_distribution)
             elif isinstance(item, na.AbstractScalarArray):
                 item_nominal = item_distribution = item
             else:
                 return NotImplemented
 
@@ -289,14 +326,30 @@
 
         result = super().__array_ufunc__(function, method, *inputs, **kwargs)
         if result is not NotImplemented:
             return result
 
         nout = function.nout
 
+        inputs_nominal = []
+        inputs_distribution = []
+        for inp in inputs:
+            if isinstance(inp, na.AbstractArray):
+                if isinstance(inp, AbstractUncertainScalarArray):
+                    inp_nominal = inp.nominal
+                    inp_distribution = inp.distribution
+                elif isinstance(inp, na.AbstractScalarArray):
+                    inp_nominal = inp_distribution = inp
+                else:
+                    return NotImplemented
+            else:
+                inp_nominal = inp_distribution = inp
+            inputs_nominal.append(inp_nominal)
+            inputs_distribution.append(inp_distribution)
+
         kwargs_nominal = dict()
         kwargs_distribution = dict()
 
         if "where" in kwargs:
             where = kwargs.pop("where")
             if isinstance(where, na.AbstractArray):
                 if isinstance(where, na.AbstractScalar):
@@ -320,15 +373,15 @@
                 if o is not None:
                     if isinstance(o, UncertainScalarArray):
                         types = (np.ndarray, na.AbstractArray)
                         o_nominal = o.nominal if isinstance(o.nominal, types) else None
                         o_distribution = o.distribution if isinstance(o.distribution, types) else None
                     else:
                         raise ValueError(
-                            f"`out` must be `None` or an instance of `{self.type_array}`, "
+                            f"`out` must be `None` or an instance of `{self.type_explicit}`, "
                             f"got {tuple(type(x) for x in out)}"
                         )
                 else:
                     o_nominal = o_distribution = None
                 out_nominal.append(o_nominal)
                 out_distribution.append(o_distribution)
             if nout == 1:
@@ -338,30 +391,14 @@
                 out_nominal = tuple(out_nominal)
                 out_distribution = tuple(out_distribution)
             kwargs_nominal["out"] = out_nominal
             kwargs_distribution["out"] = out_distribution
         else:
             out = (None, ) * nout
 
-        inputs_nominal = []
-        inputs_distribution = []
-        for inp in inputs:
-            if isinstance(inp, na.AbstractArray):
-                if isinstance(inp, AbstractUncertainScalarArray):
-                    inp_nominal = inp.nominal
-                    inp_distribution = inp.distribution
-                elif isinstance(inp, na.AbstractScalarArray):
-                    inp_nominal = inp_distribution = inp
-                else:
-                    return NotImplemented
-            else:
-                inp_nominal = inp_distribution = inp
-            inputs_nominal.append(inp_nominal)
-            inputs_distribution.append(inp_distribution)
-
         result_nominal = getattr(function, method)(*inputs_nominal, **kwargs_nominal, **kwargs)
         result_distribution = getattr(function, method)(*inputs_distribution, **kwargs_distribution, **kwargs)
 
         if nout == 1:
             result_nominal = (result_nominal, )
             result_distribution = (result_distribution, )
 
@@ -391,14 +428,20 @@
     ):
         result = super().__array_function__(func=func, types=types, args=args, kwargs=kwargs)
         if result is not NotImplemented:
             return result
 
         from . import uncertainties_array_functions
 
+        if func in uncertainties_array_functions.ARRAY_CREATION_LIKE_FUNCTIONS:
+            return uncertainties_array_functions.array_function_array_creation_like(func, *args, **kwargs)
+
+        if func in uncertainties_array_functions.SEQUENCE_FUNCTIONS:
+            return uncertainties_array_functions.array_function_sequence(func, *args, **kwargs)
+
         if func in uncertainties_array_functions.DEFAULT_FUNCTIONS:
             return uncertainties_array_functions.array_function_default(func, *args, **kwargs)
 
         if func in uncertainties_array_functions.PERCENTILE_LIKE_FUNCTIONS:
             return uncertainties_array_functions.array_function_percentile_like(func, *args, **kwargs)
 
         if func in uncertainties_array_functions.ARG_REDUCE_FUNCTIONS:
@@ -414,17 +457,35 @@
             return uncertainties_array_functions.array_function_stack_like(func, *args, **kwargs)
 
         if func in uncertainties_array_functions.HANDLED_FUNCTIONS:
             return uncertainties_array_functions.HANDLED_FUNCTIONS[func](*args, **kwargs)
 
         return NotImplemented
 
+    def __named_array_function__(self, func, *args, **kwargs):
+        result = super().__named_array_function__(func, *args, **kwargs)
+        if result is not NotImplemented:
+            return result
+
+        from . import uncertainties_named_array_functions
+
+        if func in uncertainties_named_array_functions.RANDOM_FUNCTIONS:
+            return uncertainties_named_array_functions.random(func=func, *args, **kwargs)
+
+        if func in uncertainties_named_array_functions.PLT_PLOT_LIKE_FUNCTIONS:
+            return uncertainties_named_array_functions.plt_plot_like(func, *args, **kwargs)
+
+        if func in uncertainties_named_array_functions.HANDLED_FUNCTIONS:
+            return uncertainties_named_array_functions.HANDLED_FUNCTIONS[func](*args, **kwargs)
+
+        return NotImplemented
+
     @property
     def broadcasted(self) -> na.UncertainScalarArray:
-        a = self.array
+        a = self.explicit
         return na.UncertainScalarArray(
             nominal=na.broadcast_to(a.nominal, a.shape),
             distribution=na.broadcast_to(a.distribution, a.shape_distribution),
         )
 
 
 @dataclasses.dataclass(eq=False, repr=False)
@@ -433,99 +494,155 @@
     na.AbstractExplicitArray,
     Generic[NominalArrayT, DistributionArrayT],
 ):
     nominal: NominalArrayT = dataclasses.MISSING
     distribution: DistributionArrayT = dataclasses.MISSING
 
     def __post_init__(self):
-        if self.axis_distribution not in na.shape(self.distribution):
+        if self.axis_distribution in na.shape(self.nominal):
             raise ValueError(
-                f"`axis_distribution`, '{self.axis_distribution}' not in `distribution` array with "
-                f"shape {na.shape(self.distribution)}"
+                f"`axis_distribution`, '{self.axis_distribution}' should not be in `nominal` array with "
+                f"shape {na.shape(self.nominal)}"
             )
 
-    @classmethod
-    def empty(
-            cls: Type[Self],
-            shape: dict[str, int],
-            dtype: Type = float,
-            axis_distribution: str = _axis_distribution_default,
-            num_distribution: int = _num_distribution_default,
-    ) -> Self:
-        shape_distribution = shape | {axis_distribution: num_distribution}
-        return UncertainScalarArray(
-            nominal=na.ScalarArray.empty(shape=shape, dtype=dtype),
-            distribution=na.ScalarArray.empty(shape=shape_distribution, dtype=dtype),
-        )
-
-    @classmethod
-    def zeros(
-            cls: Type[Self],
-            shape: dict[str, int],
-            dtype: Type = float,
-            axis_distribution: str = _axis_distribution_default,
-            num_distribution: int = _num_distribution_default,
-    ) -> Self:
-        shape_distribution = shape | {axis_distribution: num_distribution}
-        return UncertainScalarArray(
-            nominal=na.ScalarArray.zeros(shape=shape, dtype=dtype),
-            distribution=na.ScalarArray.zeros(shape=shape_distribution, dtype=dtype),
-        )
-
-    @classmethod
-    def ones(
-            cls: Type[Self],
-            shape: dict[str, int],
-            dtype: Type = float,
-            axis_distribution: str = _axis_distribution_default,
-            num_distribution: int = _num_distribution_default,
-    ) -> Self:
-        shape_distribution = shape | {axis_distribution: num_distribution}
-        return UncertainScalarArray(
-            nominal=na.ScalarArray.ones(shape=shape, dtype=dtype),
-            distribution=na.ScalarArray.ones(shape=shape_distribution, dtype=dtype),
-        )
-
     @property
     def num_distribution(self: Self) -> int:
         return self.distribution.shape[self.axis_distribution]
 
     @property
     def axes(self: Self) -> tuple[str, ...]:
         return tuple(self.shape.keys())
 
     @property
     def shape(self) -> dict[str, int]:
         shape = self.shape_distribution
-        shape.pop(self.axis_distribution)
+        if self.axis_distribution in shape:
+            shape.pop(self.axis_distribution)
         return shape
 
     @property
     def ndim(self: Self) -> int:
         return len(self.shape)
 
     @property
     def size(self: Self) -> int:
         return int(np.array(tuple(self.shape.values())).prod())
 
     @property
-    def array(self) -> Self:
+    def explicit(self) -> Self:
         return self.copy_shallow()
 
     @property
     def centers(self) -> Self:
         return self
 
+    def __setitem__(
+            self,
+            item: dict[str, int | slice | na.AbstractScalar] | na.AbstractScalar,
+            value: int | float | u.Quantity | na.AbstractScalar,
+    ):
+        shape_self = self.shape
+
+        if isinstance(item, na.AbstractArray):
+
+            item = item.explicit
+            if not set(item.shape).issubset(shape_self):
+                raise ValueError(
+                    f"if `item` is an instance of `{na.AbstractArray.__name__}`, "
+                    f"`item.axes`, {item.axes}, should be a subset of `self.axes`, {self.axes}"
+                )
+
+            if isinstance(item, na.AbstractUncertainScalarArray):
+                item_nominal = item.nominal
+                item_distribution = item.distribution
+            elif isinstance(item, na.AbstractScalarArray):
+                item_nominal = item_distribution = item
+            else:
+                raise TypeError(
+                    f"if `item` is an instance of `{na.AbstractArray.__name__}`, "
+                    f"it must be an instance of `{na.AbstractScalar.__name__}`, "
+                    f"got `{type(item)}`"
+                )
+        elif isinstance(item, dict):
+
+            if not set(item).issubset(shape_self):
+                raise ValueError(
+                    f"if `item` is a `{dict.__name__}`, the keys in `item`, {tuple(item)}, "
+                    f"must be a subset of `self.axes`, {self.axes}"
+                )
+
+            item_nominal = dict()
+            item_distribution = dict()
+            for axis in item:
+                item_axis = item[axis]
+                if isinstance(item_axis, na.AbstractArray):
+                    if isinstance(item_axis, na.AbstractUncertainScalarArray):
+                        item_nominal[axis] = item_axis.nominal
+                        item_distribution[axis] = item_axis.distribution
+                    elif isinstance(item_axis, na.AbstractScalarArray):
+                        item_nominal[axis] = item_distribution[axis] = item_axis
+                    else:
+                        raise TypeError(
+                            f"if a value in `item` is an instance of `{na.AbstractArray.__name__}`, "
+                            f"it must be an instance of `{na.AbstractScalar.__name__}`, "
+                            f"got `{type(item_axis)}`"
+                        )
+                else:
+                    item_nominal[axis] = item_distribution[axis] = item_axis
+
+        else:
+            raise TypeError(
+                f"`item` must be an instance of `{na.AbstractArray.__name__}` or {dict.__name__}, "
+                f"got `{type(item)}`"
+            )
+
+        if isinstance(value, na.AbstractArray):
+            if isinstance(value, na.AbstractUncertainScalarArray):
+                value_nominal = value.nominal
+                value_distribution = value.distribution
+            elif isinstance(value, na.AbstractScalarArray):
+                value_nominal = value_distribution = value
+            else:
+                raise TypeError(
+                    f"if `value` is an instance of `{na.AbstractArray.__name__}`, "
+                    f"it must be an instance of `{na.AbstractScalar.__name__}`, "
+                    f"got {type(value)}"
+                )
+        else:
+            value_nominal = value_distribution = value
+
+        self.nominal[item_nominal] = value_nominal
+        self.distribution[item_distribution] = value_distribution
+
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractImplicitUncertainScalarArray(
     AbstractUncertainScalarArray,
     na.AbstractImplicitArray,
 ):
-    pass
+
+    def _attr_normalized(self, name: str) -> UncertainScalarArray:
+
+        attr = getattr(self, name)
+
+        if isinstance(attr, na.AbstractArray):
+            if isinstance(attr, na.AbstractScalar):
+                if isinstance(attr, na.AbstractUncertainScalarArray):
+                    result = attr
+                else:
+                    result = UncertainScalarArray(attr, attr)
+            else:
+                raise TypeError(
+                    f"if `{name}` is an instance of `AbstractArray`, it must be an instance of `AbstractScalar`, "
+                    f"got {type(attr)}"
+                )
+        else:
+            result = UncertainScalarArray(attr, attr)
+
+        return result
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class UniformUncertainScalarArray(
     AbstractImplicitUncertainScalarArray,
     na.AbstractRandomMixin,
     Generic[NominalArrayT, WidthT],
@@ -541,18 +658,18 @@
             start=self.nominal - self.width,
             stop=self.nominal + self.width,
             shape_random={self.axis_distribution: self.num_distribution},
             seed=self.seed,
         )
 
     @property
-    def array(self) -> UncertainScalarArray:
+    def explicit(self) -> UncertainScalarArray:
         return UncertainScalarArray(
-            nominal=na.as_named_array(self.nominal).array,
-            distribution=na.as_named_array(self.distribution).array,
+            nominal=na.explicit(self.nominal),
+            distribution=na.explicit(self.distribution),
         )
 
     @property
     def centers(self) -> Self:
         return self
 
 
@@ -573,17 +690,116 @@
             center=self.nominal,
             width=self.width,
             shape_random={self.axis_distribution: self.num_distribution},
             seed=self.seed,
         )
 
     @property
-    def array(self) -> UncertainScalarArray:
+    def explicit(self) -> UncertainScalarArray:
         return UncertainScalarArray(
-            nominal=na.as_named_array(self.nominal).array,
-            distribution=na.as_named_array(self.distribution).array,
+            nominal=na.explicit(self.nominal),
+            distribution=na.explicit(self.distribution),
         )
 
     @property
     def centers(self) -> Self:
         return self
 
+
+@dataclasses.dataclass(eq=False, repr=False)
+class AbstractUncertainScalarRandomSample(
+    AbstractImplicitUncertainScalarArray,
+    na.AbstractRandomSample,
+):
+    @property
+    def nominal(self) -> float | u.Quantity | na.AbstractScalarArray:
+        return self.explicit.nominal
+
+    @property
+    def distribution(self) -> na.AbstractScalarArray:
+        return self.explicit.distribution
+
+    @property
+    def num_distribution(self) -> int:
+        return self.explicit.num_distribution
+
+
+@dataclasses.dataclass(eq=False, repr=False)
+class UncertainScalarUniformRandomSample(
+    AbstractUncertainScalarRandomSample,
+    na.AbstractUniformRandomSample[UncertainScalarStartT, UncertainScalarStopT],
+):
+    pass
+
+
+@dataclasses.dataclass(eq=False, repr=False)
+class UncertainScalarNormalRandomSample(
+    AbstractUncertainScalarRandomSample,
+    na.AbstractNormalRandomSample[UncertainScalarCenterT, UncertainScalarWidthT],
+):
+    pass
+
+
+@dataclasses.dataclass(eq=False, repr=False)
+class UncertainScalarPoissionRandomSample(
+    AbstractUncertainScalarRandomSample,
+    na.AbstractPoissonRandomSample[UncertainScalarCenterT],
+):
+    pass
+
+
+@dataclasses.dataclass(eq=False, repr=False)
+class AbstractParameterizedUncertainScalarArray(
+    AbstractImplicitUncertainScalarArray,
+    na.AbstractParameterizedArray,
+):
+    @property
+    def nominal(self) -> float | u.Quantity | na.AbstractScalarArray:
+        return self.explicit.nominal
+
+    @property
+    def distribution(self) -> na.AbstractScalarArray:
+        return self.explicit.distribution
+
+    @property
+    def num_distribution(self) -> int:
+        return self.explicit.num_distribution
+
+
+@dataclasses.dataclass(eq=False, repr=False)
+class AbstractUncertainScalarSpace(
+    AbstractParameterizedUncertainScalarArray,
+    na.AbstractSpace,
+):
+    pass
+
+
+@dataclasses.dataclass(eq=False, repr=False)
+class UncertainScalarLinearSpace(
+    AbstractUncertainScalarSpace,
+    na.AbstractLinearSpace,
+):
+    pass
+
+
+@dataclasses.dataclass(eq=False, repr=False)
+class UncertainScalarStratifiedRandomSpace(
+    UncertainScalarLinearSpace,
+    na.AbstractStratifiedRandomSpace,
+):
+    pass
+
+
+@dataclasses.dataclass(eq=False, repr=False)
+class UncertainScalarLogarithmicSpace(
+    AbstractUncertainScalarSpace,
+    na.AbstractLogarithmicSpace,
+):
+    pass
+
+
+@dataclasses.dataclass(eq=False, repr=False)
+class UncertainScalarGeometricSpace(
+    AbstractUncertainScalarSpace,
+    na.AbstractGeometricSpace,
+):
+    pass
```

### Comparing `named_arrays-0.1.4/named_arrays/scalars/uncertainties/uncertainties_array_functions.py` & `named_arrays-0.1.5/named_arrays/_scalars/uncertainties/uncertainties_array_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,106 @@
 from typing import Callable, Sequence
 import numpy as np
 import astropy.units as u
 import named_arrays as na
-import named_arrays.scalars.array_functions
+import named_arrays._scalars.scalar_array_functions
+from . import uncertainties
 
 __all__ = [
+    'ARRAY_CREATION_LIKE_FUNCTIONS',
+    'SEQUENCE_FUNCTIONS',
     'DEFAULT_FUNCTIONS',
     'PERCENTILE_LIKE_FUNCTIONS',
     'ARG_REDUCE_FUNCTIONS',
     'FFT_LIKE_FUNCTIONS',
     'FFTN_LIKE_FUNCTIONS',
     'STACK_LIKE_FUNCTIONS',
     'HANDLED_FUNCTIONS',
 ]
 
-DEFAULT_FUNCTIONS = named_arrays.scalars.array_functions.DEFAULT_FUNCTIONS
-PERCENTILE_LIKE_FUNCTIONS = named_arrays.scalars.array_functions.PERCENTILE_LIKE_FUNCTIONS
-ARG_REDUCE_FUNCTIONS = named_arrays.scalars.array_functions.ARG_REDUCE_FUNCTIONS
-FFT_LIKE_FUNCTIONS = named_arrays.scalars.array_functions.FFT_LIKE_FUNCTIONS
-FFTN_LIKE_FUNCTIONS = named_arrays.scalars.array_functions.FFTN_LIKE_FUNCTIONS
+ARRAY_CREATION_LIKE_FUNCTIONS = named_arrays._scalars.scalar_array_functions.ARRAY_CREATION_LIKE_FUNCTIONS
+SEQUENCE_FUNCTIONS = named_arrays._scalars.scalar_array_functions.SEQUENCE_FUNCTIONS
+DEFAULT_FUNCTIONS = named_arrays._scalars.scalar_array_functions.DEFAULT_FUNCTIONS
+PERCENTILE_LIKE_FUNCTIONS = named_arrays._scalars.scalar_array_functions.PERCENTILE_LIKE_FUNCTIONS
+ARG_REDUCE_FUNCTIONS = named_arrays._scalars.scalar_array_functions.ARG_REDUCE_FUNCTIONS
+FFT_LIKE_FUNCTIONS = named_arrays._scalars.scalar_array_functions.FFT_LIKE_FUNCTIONS
+FFTN_LIKE_FUNCTIONS = named_arrays._scalars.scalar_array_functions.FFTN_LIKE_FUNCTIONS
 STACK_LIKE_FUNCTIONS = [np.stack, np.concatenate]
 HANDLED_FUNCTIONS = dict()
 
+
+def array_function_array_creation_like(
+        func: Callable,
+        prototype: na.AbstractUncertainScalarArray,
+        dtype: None | type | np.dtype = None,
+        order: str = "K",
+        subok: bool = True,
+        shape: dict[str, int] = None,
+):
+    prototype = prototype.explicit
+
+    if shape is not None:
+        shape_distribution = shape | {prototype.axis_distribution: prototype.num_distribution}
+    else:
+        shape_distribution = None
+
+    return prototype.type_explicit(
+        nominal=func(
+            na.as_named_array(prototype.nominal),
+            dtype=dtype,
+            order=order,
+            subok=subok,
+            shape=shape,
+        ),
+        distribution=func(
+            na.as_named_array(prototype.distribution),
+            dtype=dtype,
+            order=order,
+            subok=subok,
+            shape=shape_distribution,
+        ),
+    )
+
+
+def array_function_sequence(
+        func: Callable,
+        *args: float | u.Quantity | na.AbstractScalarArray | na.AbstractUncertainScalarArray,
+        axis: str,
+        num: int = 50,
+        endpoint: bool = True,
+        dtype: None | type | np.dtype = None,
+        **kwargs: float | u.Quantity | na.AbstractScalarArray,
+) -> na.AbstractUncertainScalarArray:
+
+    try:
+        args = tuple(uncertainties._normalize(arg) for arg in args)
+        kwargs = {k: uncertainties._normalize(kwargs[k]) for k in kwargs}
+    except na.ScalarTypeError:
+        return NotImplemented
+
+    return na.UncertainScalarArray(
+        nominal=func(
+            *tuple(na.as_named_array(arg.nominal) for arg in args),
+            axis=axis,
+            num=num,
+            endpoint=endpoint,
+            dtype=dtype,
+            **{k: na.as_named_array(kwargs[k].nominal) for k in kwargs},
+        ),
+        distribution=func(
+            *tuple(na.as_named_array(arg.distribution) for arg in args),
+            axis=axis,
+            num=num,
+            endpoint=endpoint,
+            dtype=dtype,
+            **{k: na.as_named_array(kwargs[k].distribution) for k in kwargs},
+        ),
+    )
+
+
 def array_function_default(
         func: Callable,
         a: na.AbstractUncertainScalarArray,
         axis: None | str | Sequence[str] = None,
         dtype: type | np.dtype = np._NoValue,
         out: None | na.UncertainScalarArray = None,
         keepdims: bool = False,
@@ -43,15 +118,15 @@
     kwargs["axis"] = tuple(shape_a.keys()) if axis is None else axis
 
     if dtype is not np._NoValue:
         kwargs["dtype"] = dtype
 
     if out is not None:
         if not isinstance(out, na.UncertainScalarArray):
-            raise ValueError(f"`out` must be `None or an instance of `{a.type_array}`, got `{type(out)}`")
+            raise ValueError(f"`out` must be `None or an instance of `{a.type_explicit}`, got `{type(out)}`")
         kwargs_nominal["out"] = out.nominal
         kwargs_distribution["out"] = out.distribution
     else:
         kwargs["out"] = out
 
     kwargs["keepdims"] = keepdims
 
@@ -87,56 +162,95 @@
         out.distribution = result_distribution
         result = out
     return result
 
 
 def array_function_percentile_like(
         func: Callable,
-        a: na.AbstractUncertainScalarArray,
+        a: float | u.Quantity | na.AbstractScalarArray | na.AbstractUncertainScalarArray,
         q: float | u.Quantity | na.AbstractScalarArray | na.AbstractUncertainScalarArray,
         axis: None | str | Sequence[str] = None,
         out: None | na.ScalarArray = None,
         overwrite_input: bool = np._NoValue,
         method: str = np._NoValue,
         keepdims: bool = False,
 ):
-    a = a.broadcasted
-    shape_a = a.shape
+    if isinstance(a, na.AbstractArray):
+        if isinstance(a, na.AbstractScalar):
+            if isinstance(a, na.AbstractScalarArray):
+                a = na.UncertainScalarArray(a, a)
+            elif isinstance(a, na.AbstractUncertainScalarArray):
+                pass
+            else:
+                return NotImplemented
+        else:
+            return NotImplemented
+    else:
+        a = na.UncertainScalarArray(a, a)
 
-    if isinstance(q, na.AbstractUncertainScalarArray):
-        q_nominal = q.nominal
-        q_distribution = q.distribution
+    if isinstance(q, na.AbstractArray):
+        if isinstance(q, na.AbstractScalar):
+            if isinstance(q, na.AbstractScalarArray):
+                q_nominal = q_distribution = q
+            elif isinstance(q, na.AbstractUncertainScalarArray):
+                q_nominal = q.nominal
+                q_distribution = q.distribution
+            else:
+                return NotImplemented
+        else:
+            return NotImplemented
     else:
         q_nominal = q_distribution = q
 
+    shape_a = a.shape
+
+    axis_normalized = na.axis_normalized(a, axis)
+
+    if axis is not None:
+        if not set(axis_normalized).issubset(shape_a):
+            raise ValueError(
+                f"the `axis` argument must be `None` or a subset of `a.axes`, "
+                f"got {axis} for `axis`, but `{a.axes} for `a.axes`"
+            )
+
+    shape_base = {ax: shape_a[ax] for ax in axis_normalized}
+
     kwargs = dict()
     kwargs_nominal = dict()
     kwargs_distribution = dict()
 
-    kwargs["axis"] = tuple(shape_a.keys()) if axis is None else axis
+    kwargs["axis"] = axis_normalized
 
     if out is not None:
         if not isinstance(out, na.UncertainScalarArray):
-            raise ValueError(f"`out` must be an instance of `{a.type_array}`, got `{type(out)}`")
+            raise ValueError(f"`out` must be an instance of `{a.type_explicit}`, got `{type(out)}`")
         kwargs_nominal["out"] = out.nominal
         kwargs_distribution["out"] = out.distribution
     else:
         kwargs["out"] = out
 
     if overwrite_input is not np._NoValue:
         kwargs["overwrite_input"] = overwrite_input
     if method is not np._NoValue:
         kwargs["method"] = method
     kwargs["keepdims"] = keepdims
 
     kwargs_nominal = kwargs | kwargs_nominal
     kwargs_distribution = kwargs | kwargs_distribution
 
-    result_nominal = func(a.nominal, q_nominal, **kwargs_nominal)
-    result_distribution = func(a.distribution, q_distribution, **kwargs_distribution)
+    result_nominal = func(
+        a=na.broadcast_to(a.nominal, na.broadcast_shapes(na.shape(a.nominal), shape_base)),
+        q=q_nominal,
+        **kwargs_nominal,
+    )
+    result_distribution = func(
+        a=na.broadcast_to(a.distribution, na.broadcast_shapes(na.shape(a.distribution), shape_base)),
+        q=q_distribution,
+        **kwargs_distribution,
+    )
 
     if out is None:
         result = na.UncertainScalarArray(
             nominal=result_nominal,
             distribution=result_distribution,
         )
     else:
@@ -189,15 +303,15 @@
         func: Callable,
         a: na.AbstractUncertainScalarArray,
         axis: tuple[str, str],
         n: None | int = None,
         norm: str = "backward"
 ) -> na.UncertainScalarArray:
 
-    a = a.array
+    a = a.explicit
     shape_a = a.shape
 
     if axis[0] not in shape_a:
         raise ValueError(f"`axis` {axis[0]} not in array with shape {shape_a}")
 
     nominal = a.nominal
     distribution = a.distribution
@@ -222,15 +336,15 @@
         func: Callable,
         a: na.AbstractUncertainScalarArray,
         axes: dict[str, str],
         s: None | dict[str, int] = None,
         norm: str = "backward",
 ) -> na.UncertainScalarArray:
 
-    a = a.array
+    a = a.explicit
     shape_a = a.shape
 
     if not set(axes).issubset(shape_a):
         raise ValueError(f"`axes`, {tuple(axes)}, not a subset of array axes, {tuple(shape_a)}")
 
     nominal = a.nominal
     distribution = a.distribution
@@ -255,22 +369,71 @@
     """Register an __array_function__ implementation for :class:`named_arrays.AbstractUncertainScalarArray` objects."""
     def decorator(func):
         HANDLED_FUNCTIONS[numpy_function] = func
         return func
     return decorator
 
 
+@implements(np.copyto)
+def copyto(
+        dst: na.UncertainScalarArray,
+        src: na.AbstractScalarArray | na.AbstractUncertainScalarArray,
+        casting: str = "same_kind",
+        where: bool | na.AbstractScalarArray | na.AbstractUncertainScalarArray = True,
+):
+    if not isinstance(dst, na.UncertainScalarArray):
+        return NotImplemented
+
+    if isinstance(src, na.AbstractArray):
+        if isinstance(src, na.AbstractScalar):
+            if isinstance(src, na.AbstractScalarArray):
+                src_nominal = src_distribution = src
+            elif isinstance(src, na.AbstractUncertainScalarArray):
+                src_nominal = src.nominal
+                src_distribution = src.distribution
+            else:
+                return NotImplemented
+        else:
+            return NotImplemented
+    else:
+        src_nominal = src_distribution = src
+
+    if isinstance(where, na.AbstractArray):
+        if isinstance(where, na.AbstractScalar):
+            if isinstance(where, na.AbstractScalarArray):
+                where_nominal = where_distribution = where
+            elif isinstance(src, na.AbstractUncertainScalarArray):
+                where_nominal = src.nominal
+                where_distribution = src.distribution
+            else:
+                return NotImplemented
+        else:
+            return NotImplemented
+    else:
+        where_nominal = where_distribution = where
+
+    try:
+        np.copyto(dst=dst.nominal, src=src_nominal, casting=casting, where=where_nominal)
+    except TypeError:
+        dst.nominal = src_nominal
+
+    try:
+        np.copyto(dst=dst.distribution, src=src_distribution, casting=casting, where=where_distribution)
+    except TypeError:
+        dst.distribution = src_distribution
+
+
 @implements(np.broadcast_to)
 def broadcast_to(
         array: na.AbstractUncertainScalarArray,
         shape: dict[str, int]
 ) -> na.UncertainScalarArray:
 
-    array = array.array
-    shape_distribution = shape | {array.axis_distribution: array.num_distribution}
+    array = array.explicit
+    shape_distribution = na.broadcast_shapes(shape, array.shape_distribution)
 
     return na.UncertainScalarArray(
         nominal=na.broadcast_to(array.nominal, shape=shape),
         distribution=na.broadcast_to(array.distribution, shape=shape_distribution)
     )
 
 
@@ -299,15 +462,15 @@
         source: str | Sequence[str],
         destination: str | Sequence[str],
 ) -> na.UncertainScalarArray:
 
     source = (source,) if isinstance(source, str) else source
     destination = (destination,) if isinstance(destination, str) else destination
 
-    a = a.array
+    a = a.explicit
 
     set_axis_diff = set(source) - set(a.axes)
     if set_axis_diff:
         raise ValueError(f"source axes {tuple(set_axis_diff)} not in array axes {a.axes}")
 
     nominal = na.as_named_array(a.nominal)
     distribution = na.as_named_array(a.distribution)
@@ -339,15 +502,15 @@
 
 @implements(np.reshape)
 def reshape(
         a: na.AbstractUncertainScalarArray,
         newshape: dict[str, int],
 ) -> na.UncertainScalarArray:
 
-    a = a.array
+    a = a.explicit
     a.nominal = na.broadcast_to(a.nominal, shape=a.shape)
     a.distribution = na.broadcast_to(a.distribution, shape=a.shape_distribution)
     a.distribution.change_axis_index(axis=a.axis_distribution, index=~0)
 
     newshape_distribution = newshape | {a.axis_distribution: a.num_distribution}
 
     return na.UncertainScalarArray(
@@ -471,15 +634,15 @@
         indices: na.AbstractUncertainScalarArray,
         shape: dict[str, int],
 ) -> dict[str, na.AbstractUncertainScalarArray]:
 
     if not shape:
         return dict()
 
-    indices = indices.array
+    indices = indices.explicit
 
     result_nominal = np.unravel_index(na.as_named_array(indices.nominal), shape=shape)
     result_distribution = np.unravel_index(na.as_named_array(indices.distribution), shape=shape)
 
     result = {ax: na.UncertainScalarArray(result_nominal[ax], result_distribution[ax]) for ax in shape}
 
     return result
@@ -569,15 +732,15 @@
     )
 
     return result_nominal and result_distribution
 
 
 @implements(np.nonzero)
 def nonzero(a: na.AbstractUncertainScalarArray) -> dict[str, na.UncertainScalarArray]:
-    a = a.array
+    a = a.explicit
 
     result = np.nonzero(a.nominal * np.prod(a.distribution, axis=a.axis_distribution))
 
     return result
 
 
 @implements(np.nan_to_num)
```

### Comparing `named_arrays-0.1.4/named_arrays/tests/test_core.py` & `named_arrays-0.1.5/named_arrays/tests/test_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 from typing import Sequence, Type, Callable
 import pytest
 import abc
 import dataclasses
 import numpy as np
+import matplotlib.axes
+import matplotlib.artist
+import matplotlib.pyplot as plt
 import astropy.units as u
 import named_arrays as na
 
 num_x = 3
 num_y = 4
 num_z = 5
 num_distribution = 3
@@ -170,24 +173,30 @@
     def test_ndim(self, array: na.AbstractArray):
         assert isinstance(array.ndim, int)
 
     def test_size(self, array: na.AbstractArray):
         size = array.size
         assert isinstance(size, int)
 
+    def test_value(self, array: na.AbstractArray):
+        result = array.value
+        assert isinstance(result, array.type_abstract)
+        assert isinstance(result + 1, array.type_abstract)
+
+
     def test_array(self, array: na.AbstractArray):
-        assert isinstance(array.array, na.AbstractExplicitArray)
+        assert isinstance(array.explicit, na.AbstractExplicitArray)
 
     def test_type_array(self, array: na.AbstractArray):
-        assert issubclass(array.type_array, na.AbstractExplicitArray)
+        assert issubclass(array.type_explicit, na.AbstractExplicitArray)
 
     def test_type_array_abstract(self, array: na.AbstractArray):
-        assert issubclass(array.type_array_abstract, na.AbstractArray)
-        assert not issubclass(array.type_array_abstract, na.AbstractExplicitArray)
-        assert not issubclass(array.type_array_abstract, na.AbstractImplicitArray)
+        assert issubclass(array.type_abstract, na.AbstractArray)
+        assert not issubclass(array.type_abstract, na.AbstractExplicitArray)
+        assert not issubclass(array.type_abstract, na.AbstractImplicitArray)
 
     def test_centers(self, array: na.AbstractArray):
         assert isinstance(array.centers, na.AbstractArray)
 
     @abc.abstractmethod
     def test_astype(self, array: na.AbstractArray, dtype: type):
         pass
@@ -253,15 +262,20 @@
             assert getattr(array, field.name) is getattr(array_copy, field.name)
 
     def test_copy(self, array: na.AbstractArray):
         array_copy = array.copy()
         assert isinstance(array_copy, na.AbstractArray)
         assert dataclasses.is_dataclass(array_copy)
         for field in dataclasses.fields(array_copy):
-            assert np.all(getattr(array, field.name) == getattr(array_copy, field.name))
+            attr = getattr(array, field.name)
+            attr_copy = getattr(array_copy, field.name)
+            if isinstance(attr, dict):
+                assert [np.all(attr[key] == attr_copy[key] for key in attr)]
+            else:
+                assert np.all(attr == attr_copy)
 
     @abc.abstractmethod
     def test__getitem__(
             self,
             array: na.AbstractArray,
             item: dict[str, int | slice | na.AbstractArray] | na.AbstractArray
     ):
@@ -434,14 +448,55 @@
             if array_2 is not None:
                 array_2 = np.transpose(array_2)
             self.test_matmul(array_2, array)
 
     class TestArrayFunctions(abc.ABC):
 
         @pytest.mark.parametrize(
+            argnames="func",
+            argvalues=[
+                np.empty_like,
+                np.zeros_like,
+                np.ones_like,
+            ]
+        )
+        @pytest.mark.parametrize(
+            argnames="shape",
+            argvalues=[
+                None,
+                dict(y=num_y),
+                dict(x=num_x, y=num_y)
+            ]
+        )
+        @pytest.mark.parametrize("dtype", [None, int, float])
+        class TestArrayCreationLikeFunctions(abc.ABC):
+
+            def test_array_creation_like_functions(
+                    self,
+                    func: Callable,
+                    array: na.AbstractArray,
+                    shape: dict[str, int],
+                    dtype: type
+            ):
+                result = func(array, dtype=dtype, shape=shape)
+
+                if shape is None:
+                    shape_normalized = array.shape
+                else:
+                    shape_normalized = shape
+
+                assert result.shape == shape_normalized
+                assert type(result) == array.type_explicit
+
+                if func is np.zeros_like:
+                    assert np.all(result.value == 0)
+                elif func is np.ones_like:
+                    assert np.all(result.value == 1)
+
+        @pytest.mark.parametrize(
             argnames='func',
             argvalues=[
                 np.all,
                 np.any,
                 np.max,
                 np.nanmax,
                 np.min,
@@ -586,14 +641,20 @@
                     func: Callable,
                     array: na.AbstractArray,
                     axes: dict[str, str],
                     s: None | dict[str, int],
             ):
                 pass
 
+        def test_copyto(self, array: na.AbstractArray):
+            dst = 0 * array
+            np.copyto(dst=dst, src=array)
+            assert np.all(array == dst)
+
+
         @pytest.mark.parametrize(
             argnames='shape',
             argvalues=[
                 dict(x=num_x, y=num_y),
                 dict(x=num_x, y=num_y, z=num_z),
             ]
         )
@@ -640,31 +701,27 @@
             if any(ax not in array.axes for ax in source_normalized):
                 with pytest.raises(ValueError, match=r"source axes .* not in array axes .*"):
                     np.moveaxis(a=array, source=source, destination=destination)
                 return
 
             result = np.moveaxis(a=array, source=source, destination=destination)
 
-            assert np.all(array.sum() == result.sum())
+            assert np.all(array == np.moveaxis(a=result, source=destination, destination=source))
             assert len(array.axes) == len(result.axes)
             assert not any(ax in result.axes for ax in source_normalized)
             assert all(ax in result.axes for ax in destination_normalized)
 
         @pytest.mark.parametrize('newshape', [dict(r=-1)])
         def test_reshape(self, array: na.AbstractArray, newshape: dict[str, int]):
 
             result = np.reshape(a=array, newshape=newshape)
 
             assert result.size == array.size
             assert result.axes == tuple(newshape.keys())
 
-        def test_linalg_inv(self, array: na.AbstractArray):
-            with pytest.raises(NotImplementedError):
-                np.linalg.inv(array)
-
         @pytest.mark.parametrize('axis', ['y', 'z'])
         @pytest.mark.parametrize('use_out', [False, True])
         def test_stack(
                 self,
                 array: na.AbstractArray,
                 axis: str,
                 use_out: bool,
@@ -686,41 +743,36 @@
             assert np.all(result[{axis: 0}] == array)
             assert np.all(result[{axis: 1}] == array)
 
             if use_out:
                 assert result is out
 
         @pytest.mark.parametrize('axis', ['x', 'y'])
-        @pytest.mark.parametrize('use_out', [False, True])
         def test_concatenate(
                 self,
                 array: na.AbstractArray,
                 axis: str,
-                use_out: bool,
         ):
             arrays = [array, array]
 
-            shape_out = array.shape
-            if axis not in shape_out:
-                shape_out[axis] = 1
-            shape_out[axis] = 2 * shape_out[axis]
+            if axis not in array.shape:
+                with pytest.raises(ValueError, match="axis .* must be present in all the input arrays, got .*"):
+                    np.concatenate(arrays, axis=axis)
+                return
 
-            if use_out:
-                out = 0 * np.concatenate(arrays=arrays, axis=axis)
-            else:
-                out = None
+            result = np.concatenate(arrays, axis=axis)
 
-            result = np.concatenate(arrays, axis=axis, out=out)
+            out = 0 * result
 
-            assert result.shape == shape_out
-            assert np.all(result[{axis: slice(None, shape_out[axis] // 2)}] == array)
-            assert np.all(result[{axis: slice(shape_out[axis] // 2, None)}] == array)
+            result_out = np.concatenate(arrays, axis=axis, out=out)
 
-            if use_out:
-                assert result is out
+            assert np.all(result[{axis: slice(None, array.shape[axis])}] == array)
+            assert np.all(result[{axis: slice(array.shape[axis], None)}] == array)
+            assert np.all(result == result_out)
+            assert result_out is out
 
         @abc.abstractmethod
         def test_sort(self, array: na.AbstractArray, axis: None | str | Sequence[str]):
             pass
 
         @pytest.mark.parametrize('axis', [None, 'x', 'y', ('x', 'y'), ()])
         def test_argsort(self, array: na.AbstractArray, axis: None | str | Sequence[str]):
@@ -743,15 +795,15 @@
 
             sorted = array[result]
             sorted_expected = np.sort(a=array, axis=axis)
             assert np.all(sorted == sorted_expected)
 
         def test_unravel_index(self, array: na.AbstractArray):
             indices_raveled = na.ScalarArrayRange(0, array.size, axis='raveled').reshape(array.shape)
-            indices_raveled = indices_raveled * array.type_array.ones(shape=dict(), dtype=int)
+            indices_raveled = indices_raveled * np.ones_like(array.value, shape=dict(), dtype=int)
             result = np.unravel_index(
                 indices=indices_raveled,
                 shape=array.shape,
             )
             expected = array.indices
             for ax in result:
                 assert np.all(result[ax] == expected[ax])
@@ -777,29 +829,27 @@
                 array_2 = array.copy().broadcast_to(shape_new)
                 assert np.array_equiv(array, array_2)
 
             elif array_2 == "zeros":
                 array_2 = 0 * array
                 assert not np.array_equiv(array, array_2)
 
-        @pytest.mark.parametrize("array_2", ["copy", "broadcast", "zeros"])
+        @pytest.mark.parametrize("array_2", ["copy", "zeros"])
         def test_allclose(self, array: na.AbstractArray, array_2: str):
             if array_2 == "copy":
-                array_2 = array + array.mean() * na.ScalarUniformRandomSample(-1e-10, 1e-10, shape_random=array.shape)
-                assert np.allclose(array, array_2)
-
-            elif array_2 == "broadcast":
-                shape_new = array.shape | dict(extra_axis=5)
-                array_2 = array + array.mean() * na.ScalarUniformRandomSample(-1e-10, 1e-10, shape_random=shape_new)
+                array_2 = array + array.mean() * na.ScalarUniformRandomSample(-1e-10, 1e-10)
                 assert np.allclose(array, array_2)
 
             elif array_2 == "zeros":
                 array_2 = 0 * array
                 assert not np.allclose(array, array_2)
 
+            else:
+                raise NotImplementedError
+
         def test_nonzero(self, array: na.AbstractArray):
             mask = array > array.mean()
             result = array[np.nonzero(mask)]
             result_expected = array[mask]
             assert np.all(result == result_expected)
 
         @abc.abstractmethod
@@ -846,20 +896,28 @@
 
     def test_sum(
             self,
             array: na.AbstractArray,
     ):
         assert np.array_equal(array.sum(), np.sum(array))
 
-    @abc.abstractmethod
     def test_ptp(
             self,
             array: na.AbstractArray,
     ):
-        pass
+        try:
+            result_expected = np.ptp(array)
+        except Exception as e:
+            with pytest.raises(type(e)):
+                array.ptp()
+            return
+
+        result = array.ptp()
+
+        assert np.all(result == result_expected)
 
     def test_mean(
             self,
             array: na.AbstractArray,
     ):
         assert np.array_equal(array.mean(), np.mean(array))
 
@@ -873,76 +931,219 @@
             self,
             array: na.AbstractArray,
     ):
         q = 25 * u.percent
         kwargs = dict(method='closest_observation')
         assert np.array_equal(array.percentile(q, **kwargs), np.percentile(array, q, **kwargs))
 
-    @abc.abstractmethod
     def test_all(
             self,
             array: na.AbstractArray,
     ):
-        pass
+        try:
+            result_expected = np.all(array)
+        except Exception as e:
+            with pytest.raises(type(e)):
+                array.all()
+            return
+
+        result = array.all()
+
+        assert np.all(result == result_expected)
 
-    @abc.abstractmethod
     def test_any(
             self,
             array: na.AbstractArray
     ):
-        pass
+        try:
+            result_expected = np.any(array)
+        except Exception as e:
+            with pytest.raises(type(e)):
+                array.any()
+            return
+
+        result = array.any()
+
+        assert np.all(result == result_expected)
 
     def test_rms(
             self,
             array: na.AbstractArray,
     ):
         assert np.array_equal(array.rms(), np.sqrt(np.mean(np.square(array))))
 
     def test_transpose(
             self,
             array: na.AbstractArray,
     ):
         assert np.array_equal(array.transpose(), np.transpose(array))
 
+    class TestNamedArrayFunctions(abc.ABC):
+
+        @pytest.mark.parametrize(
+            argnames="func",
+            argvalues=[
+                na.plt.plot,
+            ]
+        )
+        @pytest.mark.parametrize(
+            argnames="ax",
+            argvalues=[
+                np._NoValue,
+                None,
+                plt.subplots()[1],
+                na.plt.subplots(axis_cols="x", ncols=num_x)[1],
+            ]
+        )
+        @pytest.mark.parametrize(
+            argnames="axis",
+            argvalues=[
+                np._NoValue,
+                None,
+                "y",
+            ]
+        )
+        class TestPltPlotLikeFunctions(abc.ABC):
+
+            def test_plt_plot_like(
+                    self,
+                    func: Callable,
+                    array: na.AbstractArray,
+                    array_2: na.ArrayLike,
+                    ax: None | matplotlib.axes.Axes,
+                    axis: None | str,
+                    where: bool | na.AbstractScalar,
+                    alpha: None | str | na.AbstractScalar,
+            ):
+                args = (array_2, array)
+                args = tuple(a for a in args if a is not None)
+
+                kwargs = dict()
+                if ax is not np._NoValue:
+                    kwargs["ax"] = ax
+                if axis is not np._NoValue:
+                    kwargs["axis"] = axis
+                if where is not np._NoValue:
+                    kwargs["where"] = where
+                if alpha is not np._NoValue:
+                    kwargs["alpha"] = alpha
+
+                shape = na.shape_broadcasted(*args)
+
+                axis_normalized = axis
+                if axis_normalized is np._NoValue:
+                    axis_normalized = None
+
+                if axis_normalized is None:
+                    if len(shape) != 1:
+                        with pytest.raises(
+                            expected_exception=ValueError,
+                            match="if `axis` is `None`, the broadcasted shape of .* should have one element"
+                        ):
+                            func(*args, **kwargs)
+                        return
+                    axis_normalized = next(iter(shape))
+
+                shape_orthogonal = {a: shape[a] for a in shape if a != axis_normalized}
+
+                if ax is None or ax is np._NoValue:
+                    ax_normalized = plt.gca()
+                else:
+                    ax_normalized = ax
+                ax_normalized = na.as_named_array(ax_normalized)
+
+                if not set(ax_normalized.shape).issubset(shape_orthogonal):
+                    with pytest.raises(
+                            expected_exception=ValueError,
+                            match="the shape of .* should be a subset of .*"
+                    ):
+                        func(*args, **kwargs)
+                    return
+
+                for k in kwargs:
+                    if not set(na.shape(kwargs[k])).issubset(shape_orthogonal):
+                        with pytest.raises(
+                            expected_exception=ValueError,
+                            match="the shape of .* should be a subset of .*"
+                        ):
+                            func(*args, **kwargs)
+                        return
+
+                result = func(*args, **kwargs)
+
+                assert isinstance(result, na.AbstractArray)
+                assert result.dtype == matplotlib.artist.Artist
+
+                for index in ax_normalized.ndindex():
+                    assert ax_normalized[index].ndarray.has_data()
 
 
 class AbstractTestAbstractExplicitArray(
     AbstractTestAbstractArray,
 ):
-    pass
 
+    @abc.abstractmethod
+    def test__setitem__(
+            self,
+            array: na.AbstractArray,
+            item: dict[str, int | slice | na.AbstractArray] | na.AbstractArray,
+            value: na.AbstractArray
+    ):
+        result = na.broadcast_to(array, array.shape).astype(float).copy()
+
+        if isinstance(item, na.AbstractArray):
+            if not set(item.shape).issubset(array.axes):
+                with pytest.raises(
+                    expected_exception=ValueError,
+                    match="if `item` is an instance of .*, `item.axes`, .*, "
+                          "should be a subset of `self.axes`, .*"
+                ):
+                    result[item] = value
+                return
 
-@pytest.mark.parametrize('shape', [dict(x=3), dict(x=4, y=5)])
-@pytest.mark.parametrize('dtype', [int, float, complex])
-class AbstractTestAbstractExplicitArrayCreation(abc.ABC):
+        elif isinstance(item, dict):
+            if not set(item).issubset(array.axes):
+                with pytest.raises(
+                    expected_exception=ValueError,
+                    match="if `item` is a .*, the keys in `item`, .*, "
+                          "must be a subset of `self.axes`, .*"
+                ):
+                    result[item] = value
+                return
 
-    @property
-    @abc.abstractmethod
-    def type_array(self) -> Type[na.AbstractExplicitArray]:
-        pass
+            for axis in item:
+                if isinstance(item[axis], int):
+                    if axis in na.shape(value):
+                        with pytest.raises(
+                            expected_exception=ValueError,
+                            match="`value` has an axis, .*, that is set to an `int` in `item`"
+                        ):
+                            result[item] = value
+                        return
+
+        try:
+            value_0 = na.as_named_array(value).reshape(dict(dummy=-1))[dict(dummy=0)]
+            result_0 = result.reshape(dict(dummy=-1))[dict(dummy=0)]
+            value_0 + result_0
+        except u.UnitConversionError as e:
+            with pytest.raises((TypeError, u.UnitConversionError)):
+                result[item] = value
+            return
 
-    def test_empty(self, shape: dict[str, int], dtype: Type):
-        result = self.type_array.empty(shape, dtype=dtype)
-        assert result.shape == shape
-
-    def test_zeros(self, shape: dict[str, int], dtype: Type):
-        result = self.type_array.zeros(shape, dtype=dtype)
-        assert result.shape == shape
-        assert np.all(result == 0)
-
-    def test_ones(self, shape: dict[str, int], dtype: Type):
-        result = self.type_array.ones(shape, dtype=dtype)
-        assert result.shape == shape
-        assert np.all(result == 1)
+        result[item] = value
+        assert np.all(result[item] == value)
 
 
 class AbstractTestAbstractImplicitArray(
-    AbstractTestAbstractArray,
+    abc.ABC,
 ):
-    pass
+    def test_explicit(self, array: na.AbstractArray):
+        result = array.explicit
+        assert isinstance(result, na.AbstractExplicitArray)
+        assert np.abs(result.sum()) > 0
 
 
 class AbstractTestAbstractRandomMixin(
     abc.ABC,
 ):
 
     def test_seed(self, array: na.AbstractRandomMixin):
@@ -1019,16 +1220,15 @@
     AbstractTestAbstractImplicitArray,
 ):
 
     def test_axis(self, array: na.AbstractParameterizedArray):
         assert isinstance(array.axis, (str, na.AbstractArray))
 
     def test_num(self, array: na.AbstractParameterizedArray):
-        assert isinstance(array.num, (int, na.AbstractArray))
-        assert array.num == array.shape[array.axis]
+        assert isinstance(array.num, (int, np.integer, na.AbstractArray))
 
 
 class AbstractTestAbstractLinearParametrizedArrayMixin:
 
     def test_step(self, array: na.AbstractLinearParameterizedArrayMixin):
         assert isinstance(array.step, (int, float, complex, u.Quantity, na.AbstractArray))
         assert np.all(np.abs(array.step) > 0)
```

### Comparing `named_arrays-0.1.4/named_arrays.egg-info/PKG-INFO` & `named_arrays-0.1.5/named_arrays.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: named-arrays
-Version: 0.1.4
+Version: 0.1.5
 Summary: Numpy arrays with labeled axes, similar to xarray but with support for uncertainties
 Author-email: "Roy T. Smart" <roytsmart@gmail.com>, "Jacob D. Parker" <jacobdparker@gmail.com>
 Project-URL: Homepage, https://github.com/Kankelborg-Group/named_arrays
 Project-URL: Documentation, https://named-arrays.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -12,14 +12,15 @@
 Provides-Extra: doc
 
 # named_arrays
 
 ![tests](https://github.com/Kankelborg-Group/named_arrays/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/Kankelborg-Group/named_arrays/branch/main/graph/badge.svg?token=x8K7SLx4UB)](https://codecov.io/gh/Kankelborg-Group/named_arrays)
 [![Documentation Status](https://readthedocs.org/projects/named-arrays/badge/?version=latest)](https://named-arrays.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/named-arrays.svg)](https://badge.fury.io/py/named-arrays)
 
 `named_arrays` is an implementation of a [named tensor](https://nlp.seas.harvard.edu/NamedTensor), which assigns names to each axis of an n-dimensional array such as a numpy array.
 
 When using a numpy array, we often have to insert singleton dimensions to align axes before using binary operators etc.
 This is not necessary when using a named tensor implementation such as `xarray` or `named_arrays`, axes are aligned automatically using their names.
 
 ## Installation
```

### Comparing `named_arrays-0.1.4/pyproject.toml` & `named_arrays-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -21,20 +21,27 @@
     "scipy",
     'astropy',
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
-    "pytest"
+    "pytest",
 ]
 doc = [
+    "pytest",
+    "graphviz",
     "sphinx-autodoc-typehints",
     "pydata-sphinx-theme",
+    "ipykernel",
     "jupyter-sphinx",
+    "sphinx-favicon",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Kankelborg-Group/named_arrays"
 Documentation = "https://named-arrays.readthedocs.io/en/latest"
 
 [tool.setuptools_scm]
+
+[tool.setuptools.package-data]
+named_arrays = ["py.typed"]
```

