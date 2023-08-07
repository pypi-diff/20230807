# Comparing `tmp/cleanlab-studio-1.1.0.tar.gz` & `tmp/cleanlab-studio-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-1.1.0.tar", last modified: Thu Aug  3 00:01:10 2023, max compression
+gzip compressed data, was "cleanlab-studio-1.1.1.tar", last modified: Mon Aug  7 18:44:16 2023, max compression
```

## Comparing `cleanlab-studio-1.1.0.tar` & `cleanlab-studio-1.1.1.tar`

### file list

```diff
@@ -1,84 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.026109 cleanlab-studio-1.1.0/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.026109 cleanlab-studio-1.1.0/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.026109 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/schema_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/studio/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/studio/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/studio/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.026109 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/test_excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/test_json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.020507 cleanlab-studio-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-08-07 18:44:16.020507 cleanlab-studio-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.008507 cleanlab-studio-1.1.1/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.012507 cleanlab-studio-1.1.1/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.012507 cleanlab-studio-1.1.1/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.012507 cleanlab-studio-1.1.1/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.016507 cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/schema_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/upload_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.016507 cleanlab-studio-1.1.1/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.016507 cleanlab-studio-1.1.1/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.016507 cleanlab-studio-1.1.1/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.020507 cleanlab-studio-1.1.1/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/clean_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.020507 cleanlab-studio-1.1.1/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.020507 cleanlab-studio-1.1.1/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/studio/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.008507 cleanlab-studio-1.1.1/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-08-07 18:44:15.000000 cleanlab-studio-1.1.1/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-08-07 18:44:16.000000 cleanlab-studio-1.1.1/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:44:15.000000 cleanlab-studio-1.1.1/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-07 18:44:15.000000 cleanlab-studio-1.1.1/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-07 18:44:15.000000 cleanlab-studio-1.1.1/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 18:44:15.000000 cleanlab-studio-1.1.1/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 18:44:16.020507 cleanlab-studio-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.020507 cleanlab-studio-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:16.020507 cleanlab-studio-1.1.1/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/tests/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/tests/datasets/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/tests/datasets/test_excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/tests/datasets/test_json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-08-07 18:44:00.000000 cleanlab-studio-1.1.1/tests/datasets/utils.py
```

### Comparing `cleanlab-studio-1.1.0/LICENSE` & `cleanlab-studio-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/PKG-INFO` & `cleanlab-studio-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.1.0
+Version: 1.1.1
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
```

### Comparing `cleanlab-studio-1.1.0/README.md` & `cleanlab-studio-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/helpers.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/image_utils.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/image_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/schema_types.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/schema_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload_helpers.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload_types.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/dataset/upload_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/main.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/types.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/cli/util.py` & `cleanlab-studio-1.1.1/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/errors.py` & `cleanlab-studio-1.1.1/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-1.1.1/cleanlab_studio/internal/api/api.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-1.1.1/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-1.1.1/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-1.1.1/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-1.1.1/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/internal/settings.py` & `cleanlab-studio-1.1.1/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-1.1.1/cleanlab_studio/internal/upload_helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,48 @@
 
 import aiohttp
 from multidict import CIMultiDictProxy
 import requests
 
 from .api import api
 from .dataset_source import DatasetSource
-from .types import JSONDict
+from .types import FieldSchemaDict, JSONDict
+
+
+def upload_dataset(
+    api_key: str,
+    dataset_source: DatasetSource,
+    *,
+    schema_overrides: Optional[FieldSchemaDict] = None,
+    modality: Optional[str] = None,
+    id_column: Optional[str] = None,
+) -> str:
+    upload_id = upload_dataset_file(api_key, dataset_source)
+    schema = get_proposed_schema(api_key, upload_id)
+
+    if (schema is None or schema.get("immutable", False)) and (
+        schema_overrides is not None or modality is not None or id_column is not None
+    ):
+        raise ValueError(
+            "Schema_overrides, modality, and id_column parameters cannot be provided for simple zip uploads"
+        )
+
+    if schema is not None and not schema.get("immutable", False):
+        schema["metadata"]["name"] = dataset_source.dataset_name
+        if schema_overrides is not None:
+            for field in schema_overrides:
+                schema["fields"][field] = schema_overrides[field]
+        if modality is not None:
+            schema["metadata"]["modality"] = modality
+        if id_column is not None:
+            schema["metadata"]["id_column"] = id_column
+
+    api.confirm_schema(api_key, schema, upload_id)
+    dataset_id = get_ingestion_result(api_key, upload_id)
+    return dataset_id
 
 
 async def _upload_file_chunk_async(
     session: aiohttp.ClientSession,
     chunk: bytes,
     presigned_post: str,
 ) -> CIMultiDictProxy[str]:
@@ -54,15 +87,18 @@
         {"ETag": json.loads(res.headers["etag"]), "PartNumber": i + 1}
         for i, res in enumerate(responses)
     ]
 
 
 def upload_dataset_file(api_key: str, dataset_source: DatasetSource) -> str:
     upload_id, part_sizes, presigned_posts = api.initialize_upload(
-        api_key, dataset_source.get_filename(), dataset_source.file_type, dataset_source.file_size
+        api_key,
+        dataset_source.get_filename(),
+        dataset_source.file_type,
+        dataset_source.file_size,
     )
     upload_parts = upload_file_parts(dataset_source, part_sizes, presigned_posts)
     api.complete_file_upload(api_key, upload_id, upload_parts)
     return upload_id
 
 
 def get_proposed_schema(api_key: str, upload_id: str) -> Optional[JSONDict]:
```

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/internal/util.py` & `cleanlab-studio-1.1.1/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/studio/clean.py` & `cleanlab-studio-1.1.1/cleanlab_studio/internal/clean_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/studio/inference.py` & `cleanlab-studio-1.1.1/cleanlab_studio/studio/inference.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio/studio/studio.py` & `cleanlab-studio-1.1.1/cleanlab_studio/studio/studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 """
 from typing import Any, List, Literal, Optional, Union
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
-from . import clean, upload, inference
+from . import inference
+from cleanlab_studio.internal import clean_helpers, upload_helpers
 from cleanlab_studio.internal.api import api
 from cleanlab_studio.internal.util import (
     init_dataset_source,
     check_none,
     check_not_none,
 )
 from cleanlab_studio.internal.settings import CleanlabSettings
@@ -64,15 +65,15 @@
             modality: Optional parameter to override the modality of your dataset. If not provided, modality will be inferred.
             id_column: Optional parameter to override the ID column of your dataset. If not provided, a monotonically increasing ID column will be generated.
 
         Returns:
             ID of uploaded dataset.
         """
         ds = init_dataset_source(dataset, dataset_name)
-        return upload.upload_dataset(
+        return upload_helpers.upload_dataset(
             self._api_key,
             ds,
             schema_overrides=schema_overrides,
             modality=modality,
             id_column=id_column,
         )
 
@@ -262,15 +263,15 @@
         Args:
             cleanset_id: ID of cleanset to check status of.
             timeout: Optional timeout after which to stop polling for progress. If not provided, will block until cleanset is ready.
 
         Returns:
             After cleanset is done being generated, returns `True` if cleanset is ready to use, `False` otherwise.
         """
-        return clean.poll_cleanset_status(self._api_key, cleanset_id, timeout)
+        return clean_helpers.poll_cleanset_status(self._api_key, cleanset_id, timeout)
 
     def get_latest_cleanset_id(self, project_id: str) -> str:
         """
         Gets latest cleanset ID for a project.
 
         Args:
             project_id: ID of project.
@@ -294,15 +295,15 @@
         """
         Gets a model deployed by Cleanlab Studio.
 
         Args:
             model_id: ID of model to get. This ID should be fetched in the deployments page of the app UI.
 
         Returns:
-            Model object with methods to run predictions on new input data
+            [Model](inference#class-model) object with methods to run predictions on new input data.
         """
         return inference.Model(self._api_key, model_id)
 
     class Experimental:
         def __init__(self, outer):  # type: ignore
             self._outer = outer
```

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-1.1.1/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.1.0
+Version: 1.1.1
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
```

### Comparing `cleanlab-studio-1.1.0/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-1.1.1/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -37,31 +37,30 @@
 cleanlab_studio/cli/dataset/upload_types.py
 cleanlab_studio/cli/decorators/__init__.py
 cleanlab_studio/cli/decorators/auth_config.py
 cleanlab_studio/cli/decorators/previous_state.py
 cleanlab_studio/cli/login/__init__.py
 cleanlab_studio/cli/login/login.py
 cleanlab_studio/internal/__init__.py
+cleanlab_studio/internal/clean_helpers.py
 cleanlab_studio/internal/settings.py
 cleanlab_studio/internal/types.py
 cleanlab_studio/internal/upload_helpers.py
 cleanlab_studio/internal/util.py
 cleanlab_studio/internal/api/__init__.py
 cleanlab_studio/internal/api/api.py
 cleanlab_studio/internal/dataset_source/__init__.py
 cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
 cleanlab_studio/internal/dataset_source/dataset_source.py
 cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
 cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
 cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
 cleanlab_studio/studio/__init__.py
-cleanlab_studio/studio/clean.py
 cleanlab_studio/studio/inference.py
 cleanlab_studio/studio/studio.py
-cleanlab_studio/studio/upload.py
 tests/__init__.py
 tests/datasets/__init__.py
 tests/datasets/constants.py
 tests/datasets/test_csv_dataset.py
 tests/datasets/test_excel_dataset.py
 tests/datasets/test_json_dataset.py
 tests/datasets/utils.py
```

### Comparing `cleanlab-studio-1.1.0/setup.py` & `cleanlab-studio-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/tests/datasets/test_csv_dataset.py` & `cleanlab-studio-1.1.1/tests/datasets/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/tests/datasets/test_excel_dataset.py` & `cleanlab-studio-1.1.1/tests/datasets/test_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/tests/datasets/test_json_dataset.py` & `cleanlab-studio-1.1.1/tests/datasets/test_json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.1.0/tests/datasets/utils.py` & `cleanlab-studio-1.1.1/tests/datasets/utils.py`

 * *Files identical despite different names*

