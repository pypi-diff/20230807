# Comparing `tmp/mapillary-1.0.8.tar.gz` & `tmp/mapillary-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapillary-1.0.8.tar", last modified: Wed Aug 10 16:41:56 2022, max compression
+gzip compressed data, was "mapillary-1.0.9.tar", last modified: Sat Aug 13 11:43:44 2022, max compression
```

## Comparing `mapillary-1.0.8.tar` & `mapillary-1.0.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.910520 mapillary-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     3541 2022-08-10 16:41:42.000000 mapillary-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-08-10 16:41:42.000000 mapillary-1.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-08-10 16:41:42.000000 mapillary-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-08-10 16:41:42.000000 mapillary-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-08-10 16:41:42.000000 mapillary-1.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     9932 2022-08-10 16:41:56.910520 mapillary-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-08-10 16:41:42.000000 mapillary-1.0.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)    73847 2022-08-10 16:41:42.000000 mapillary-1.0.8/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (121)     7907 2022-08-10 16:41:42.000000 mapillary-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-10 16:41:42.000000 mapillary-1.0.8/mapillary.toml
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-10 16:41:56.910520 mapillary-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-08-10 16:41:42.000000 mapillary-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.902520 mapillary-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.902520 mapillary-1.0.8/src/mapillary/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.906520 mapillary-1.0.8/src/mapillary/config/
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.906520 mapillary-1.0.8/src/mapillary/config/api/
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/config/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12581 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/config/api/entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/config/api/general.py
--rw-r--r--   0 runner    (1001) docker     (121)     8163 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/config/api/vector_tiles.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.906520 mapillary-1.0.8/src/mapillary/controller/
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/controller/detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4679 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/controller/feature.py
--rw-r--r--   0 runner    (1001) docker     (121)    31458 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/controller/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     4856 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/controller/save.py
--rw-r--r--   0 runner    (1001) docker     (121)    33785 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.906520 mapillary-1.0.8/src/mapillary/models/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.906520 mapillary-1.0.8/src/mapillary/models/api/
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/models/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8104 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/models/api/entities.py
--rw-r--r--   0 runner    (1001) docker     (121)    14360 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/models/api/general.py
--rw-r--r--   0 runner    (1001) docker     (121)    19230 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/models/api/vector_tiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     8257 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/models/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9597 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14586 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/models/geojson.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.910520 mapillary-1.0.8/src/mapillary/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/utils/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)    16122 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/utils/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    21713 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     9928 2022-08-10 16:41:42.000000 mapillary-1.0.8/src/mapillary/utils/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.906520 mapillary-1.0.8/src/mapillary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9932 2022-08-10 16:41:56.000000 mapillary-1.0.8/src/mapillary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-08-10 16:41:56.000000 mapillary-1.0.8/src/mapillary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 16:41:56.000000 mapillary-1.0.8/src/mapillary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-08-10 16:41:56.000000 mapillary-1.0.8/src/mapillary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-10 16:41:56.000000 mapillary-1.0.8/src/mapillary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-08-10 16:41:42.000000 mapillary-1.0.8/test.env
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.910520 mapillary-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:42.000000 mapillary-1.0.8/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-08-10 16:41:42.000000 mapillary-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4876 2022-08-10 16:41:42.000000 mapillary-1.0.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.910520 mapillary-1.0.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:42.000000 mapillary-1.0.8/tests/data/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.910520 mapillary-1.0.8/tests/helper/
--rw-r--r--   0 runner    (1001) docker     (121)     4301 2022-08-10 16:41:42.000000 mapillary-1.0.8/tests/helper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.910520 mapillary-1.0.8/tests/helper/data/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-10 16:41:42.000000 mapillary-1.0.8/tests/helper/data/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)     2273 2022-08-10 16:41:42.000000 mapillary-1.0.8/tests/helper/fetch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4073 2022-08-10 16:41:42.000000 mapillary-1.0.8/tests/test_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 16:41:56.910520 mapillary-1.0.8/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-08-10 16:41:42.000000 mapillary-1.0.8/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-08-10 16:41:42.000000 mapillary-1.0.8/tests/utils/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     2816 2022-08-10 16:41:42.000000 mapillary-1.0.8/tests/utils/test_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.706812 mapillary-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     3541 2022-08-13 11:43:34.000000 mapillary-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-08-13 11:43:34.000000 mapillary-1.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-08-13 11:43:34.000000 mapillary-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-08-13 11:43:34.000000 mapillary-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-08-13 11:43:34.000000 mapillary-1.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     9932 2022-08-13 11:43:44.706812 mapillary-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-08-13 11:43:34.000000 mapillary-1.0.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (121)    73847 2022-08-13 11:43:34.000000 mapillary-1.0.9/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (121)     7907 2022-08-13 11:43:34.000000 mapillary-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-08-13 11:43:34.000000 mapillary-1.0.9/mapillary.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-13 11:43:44.706812 mapillary-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     6133 2022-08-13 11:43:34.000000 mapillary-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.694812 mapillary-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.698812 mapillary-1.0.9/src/mapillary/
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.698812 mapillary-1.0.9/src/mapillary/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.702812 mapillary-1.0.9/src/mapillary/config/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/config/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12581 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/config/api/entities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/config/api/general.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8163 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/config/api/vector_tiles.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.702812 mapillary-1.0.9/src/mapillary/controller/
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/controller/detection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4679 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/controller/feature.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31458 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/controller/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4856 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/controller/save.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33785 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.702812 mapillary-1.0.9/src/mapillary/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.702812 mapillary-1.0.9/src/mapillary/models/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/models/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8104 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/models/api/entities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14360 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/models/api/general.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19230 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/models/api/vector_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8257 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9597 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14586 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/models/geojson.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.702812 mapillary-1.0.9/src/mapillary/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/utils/extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16122 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/utils/filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21713 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9928 2022-08-13 11:43:34.000000 mapillary-1.0.9/src/mapillary/utils/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.698812 mapillary-1.0.9/src/mapillary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9932 2022-08-13 11:43:44.000000 mapillary-1.0.9/src/mapillary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-08-13 11:43:44.000000 mapillary-1.0.9/src/mapillary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-13 11:43:44.000000 mapillary-1.0.9/src/mapillary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2022-08-13 11:43:44.000000 mapillary-1.0.9/src/mapillary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-13 11:43:44.000000 mapillary-1.0.9/src/mapillary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-08-13 11:43:34.000000 mapillary-1.0.9/test.env
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.706812 mapillary-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:34.000000 mapillary-1.0.9/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-08-13 11:43:34.000000 mapillary-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4876 2022-08-13 11:43:34.000000 mapillary-1.0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.706812 mapillary-1.0.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:34.000000 mapillary-1.0.9/tests/data/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.706812 mapillary-1.0.9/tests/helper/
+-rw-r--r--   0 runner    (1001) docker     (121)     4301 2022-08-13 11:43:34.000000 mapillary-1.0.9/tests/helper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.706812 mapillary-1.0.9/tests/helper/data/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-13 11:43:34.000000 mapillary-1.0.9/tests/helper/data/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)     2273 2022-08-13 11:43:34.000000 mapillary-1.0.9/tests/helper/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4073 2022-08-13 11:43:34.000000 mapillary-1.0.9/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 11:43:44.706812 mapillary-1.0.9/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-08-13 11:43:34.000000 mapillary-1.0.9/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-08-13 11:43:34.000000 mapillary-1.0.9/tests/utils/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2816 2022-08-13 11:43:34.000000 mapillary-1.0.9/tests/utils/test_filter.py
```

### Comparing `mapillary-1.0.8/CODE_OF_CONDUCT.md` & `mapillary-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/CONTRIBUTING.md` & `mapillary-1.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/LICENSE` & `mapillary-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/Makefile` & `mapillary-1.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/PKG-INFO` & `mapillary-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapillary
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python 3 library built on the Mapillary API v4 to facilitate retrieving and working with Mapillary data
 Home-page: https://github.com/mapillary/mapillary-python-sdk
 Author: Christopher Beddow
 Author-email: support@mapillary.zendesk.com
 License: MIT
 Project-URL: Download, https://pypi.org/project/mapillary/#files
 Project-URL: Release Notes, https://github.com/mapillary/mapillary-python-sdk/releases
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapillary Version: 1.0.8 Summary: A Python 3
+Metadata-Version: 2.1 Name: mapillary Version: 1.0.9 Summary: A Python 3
 library built on the Mapillary API v4 to facilitate retrieving and working with
 Mapillary data Home-page: https://github.com/mapillary/mapillary-python-sdk
 Author: Christopher Beddow Author-email: support@mapillary.zendesk.com License:
 MIT Project-URL: Download, https://pypi.org/project/mapillary/#files Project-
 URL: Release Notes, https://github.com/mapillary/mapillary-python-sdk/releases
 Project-URL: Bug Tracker, https://github.com/mapillary/mapillary-python-sdk/
 issues Project-URL: Source, https://github.com/mapillary/mapillary-python-sdk
```

### Comparing `mapillary-1.0.8/Pipfile` & `mapillary-1.0.9/Pipfile`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 future = "==0.18.2"
 hypothesis = "==6.14.0"
 idna = "==2.10"
 iniconfig = "==1.1.1"
 mapbox-vector-tile = "==1.2.1"
 mercantile = "==1.2.1"
 munch = "==2.5.0"
-numpy = "==1.22"
+numpy = "==1.21.0"
 scipy = "==1.7.3"
 pkginfo = "==1.7.0"
 pluggy = "==0.13.1"
 protobuf = "==3.17.3"
 psutil = "==5.8.0"
 py = "==1.10.0"
 pyparsing = "==2.4.7"
```

### Comparing `mapillary-1.0.8/Pipfile.lock` & `mapillary-1.0.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/README.md` & `mapillary-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/setup.py` & `mapillary-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 import sys
 import json
 import shutil
 
 # Setup variables. Change as needed
 NAME = "mapillary"  
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 AUTHOR = "Christopher Beddow"
 AUTHOR_EMAIL = "support@mapillary.zendesk.com"
 LICENSE = "MIT"
 PLATFORM = ["POSIX", "MacOS X", "Linux", "Windows"]
 DESCRIPTION = (
     "A Python 3 library built on the Mapillary API v4 to facilitate retrieving and "
     "working with Mapillary data"
```

### Comparing `mapillary-1.0.8/src/mapillary/__init__.py` & `mapillary-1.0.9/src/mapillary/__init__.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/config/__init__.py` & `mapillary-1.0.9/src/mapillary/config/__init__.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/config/api/entities.py` & `mapillary-1.0.9/src/mapillary/config/api/entities.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/config/api/general.py` & `mapillary-1.0.9/src/mapillary/config/api/general.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/config/api/vector_tiles.py` & `mapillary-1.0.9/src/mapillary/config/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/controller/detection.py` & `mapillary-1.0.9/src/mapillary/controller/detection.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/controller/feature.py` & `mapillary-1.0.9/src/mapillary/controller/feature.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/controller/image.py` & `mapillary-1.0.9/src/mapillary/controller/image.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/controller/save.py` & `mapillary-1.0.9/src/mapillary/controller/save.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/interface.py` & `mapillary-1.0.9/src/mapillary/interface.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/models/api/entities.py` & `mapillary-1.0.9/src/mapillary/models/api/entities.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/models/api/general.py` & `mapillary-1.0.9/src/mapillary/models/api/general.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/models/api/vector_tiles.py` & `mapillary-1.0.9/src/mapillary/models/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/models/client.py` & `mapillary-1.0.9/src/mapillary/models/client.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/models/exceptions.py` & `mapillary-1.0.9/src/mapillary/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/models/geojson.py` & `mapillary-1.0.9/src/mapillary/models/geojson.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/utils/auth.py` & `mapillary-1.0.9/src/mapillary/utils/auth.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/utils/extract.py` & `mapillary-1.0.9/src/mapillary/utils/extract.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/utils/filter.py` & `mapillary-1.0.9/src/mapillary/utils/filter.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/utils/format.py` & `mapillary-1.0.9/src/mapillary/utils/format.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/utils/time.py` & `mapillary-1.0.9/src/mapillary/utils/time.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary/utils/verify.py` & `mapillary-1.0.9/src/mapillary/utils/verify.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary.egg-info/PKG-INFO` & `mapillary-1.0.9/src/mapillary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapillary
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python 3 library built on the Mapillary API v4 to facilitate retrieving and working with Mapillary data
 Home-page: https://github.com/mapillary/mapillary-python-sdk
 Author: Christopher Beddow
 Author-email: support@mapillary.zendesk.com
 License: MIT
 Project-URL: Download, https://pypi.org/project/mapillary/#files
 Project-URL: Release Notes, https://github.com/mapillary/mapillary-python-sdk/releases
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapillary Version: 1.0.8 Summary: A Python 3
+Metadata-Version: 2.1 Name: mapillary Version: 1.0.9 Summary: A Python 3
 library built on the Mapillary API v4 to facilitate retrieving and working with
 Mapillary data Home-page: https://github.com/mapillary/mapillary-python-sdk
 Author: Christopher Beddow Author-email: support@mapillary.zendesk.com License:
 MIT Project-URL: Download, https://pypi.org/project/mapillary/#files Project-
 URL: Release Notes, https://github.com/mapillary/mapillary-python-sdk/releases
 Project-URL: Bug Tracker, https://github.com/mapillary/mapillary-python-sdk/
 issues Project-URL: Source, https://github.com/mapillary/mapillary-python-sdk
```

### Comparing `mapillary-1.0.8/src/mapillary.egg-info/SOURCES.txt` & `mapillary-1.0.9/src/mapillary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/src/mapillary.egg-info/requires.txt` & `mapillary-1.0.9/src/mapillary.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/test.env` & `mapillary-1.0.9/test.env`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/tests/conftest.py` & `mapillary-1.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/tests/helper/client.py` & `mapillary-1.0.9/tests/helper/client.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/tests/helper/fetch.py` & `mapillary-1.0.9/tests/helper/fetch.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/tests/test_interface.py` & `mapillary-1.0.9/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/tests/utils/test_extract.py` & `mapillary-1.0.9/tests/utils/test_extract.py`

 * *Files identical despite different names*

### Comparing `mapillary-1.0.8/tests/utils/test_filter.py` & `mapillary-1.0.9/tests/utils/test_filter.py`

 * *Files identical despite different names*

