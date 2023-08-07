# Comparing `tmp/ms2query-1.2.1.tar.gz` & `tmp/ms2query-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ms2query-1.2.1.tar", last modified: Tue Jun 20 14:43:37 2023, max compression
+gzip compressed data, was "dist/ms2query-1.2.2.tar", last modified: Mon Aug  7 15:32:23 2023, max compression
```

## Comparing `ms2query-1.2.1.tar` & `ms2query-1.2.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-06-20 14:43:37.000000 ms2query-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20873 2023-06-20 14:43:25.000000 ms2query-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/k_fold_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/visualize_mass_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/clean_and_filter_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query/create_new_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/add_classifire_classifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/create_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/train_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/create_new_library/train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22515 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/ms2library.py
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/old_query_from_sqlite_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/query_from_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/results_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-06-20 14:43:25.000000 ms2query-1.2.1/ms2query/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 14:43:37.000000 ms2query-1.2.1/ms2query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-20 14:43:37.000000 ms2query-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-20 14:43:25.000000 ms2query-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:37.000000 ms2query-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/test_add_classifier_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/test_calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/test_clean_and_filter_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-06-20 14:43:25.000000 ms2query-1.2.1/tests/test_collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_ms2library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_results_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_train_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-20 14:43:26.000000 ms2query-1.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:32:23.000000 ms2query-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    24180 2023-08-07 15:32:23.000000 ms2query-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20876 2023-08-07 15:32:09.000000 ms2query-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:32:23.000000 ms2query-1.2.2/ms2query/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:32:23.000000 ms2query-1.2.2/ms2query/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/benchmarking/collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/benchmarking/k_fold_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/benchmarking/visualize_mass_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/clean_and_filter_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:32:23.000000 ms2query-1.2.2/ms2query/create_new_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/create_new_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/create_new_library/add_classifire_classifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/create_new_library/calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/create_new_library/create_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/create_new_library/library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/create_new_library/split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/create_new_library/train_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/create_new_library/train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/create_new_library/train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22515 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/old_query_from_sqlite_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/query_from_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/results_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-08-07 15:32:09.000000 ms2query-1.2.2/ms2query/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:32:23.000000 ms2query-1.2.2/ms2query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24180 2023-08-07 15:32:22.000000 ms2query-1.2.2/ms2query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-08-07 15:32:22.000000 ms2query-1.2.2/ms2query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:32:22.000000 ms2query-1.2.2/ms2query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 15:32:22.000000 ms2query-1.2.2/ms2query.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:32:22.000000 ms2query-1.2.2/ms2query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-07 15:32:22.000000 ms2query-1.2.2/ms2query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-07 15:32:22.000000 ms2query-1.2.2/ms2query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-07 15:32:23.000000 ms2query-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-08-07 15:32:09.000000 ms2query-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:32:23.000000 ms2query-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_add_classifier_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_clean_and_filter_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_results_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_train_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-07 15:32:09.000000 ms2query-1.2.2/tests/test_utils.py
```

### Comparing `ms2query-1.2.1/PKG-INFO` & `ms2query-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
@@ -118,15 +118,15 @@
           --library LIBRARY_FOLDER
                                 The directory containing the library spectra, to download add --download
           --ionmode {positive,negative}
                                 Specify the ionization mode used
           --download            This will download the most up to date model and library.The model will be stored in the folder given as the second argumentThe model will be downloaded in the in the ionization mode specified under --mode
           --results RESULTS     The folder in which the results should be stored. The default is a new results folder in the folder with the spectra
           --filter_ionmode      Filter out all spectra that are not in the specified ion-mode. The ion mode can be specified by using --ionmode
-          --addional_metadata   Return additional metadata columns in the results, for example --additional_metadata rtinseconds feature_id
+          --addional_metadata   Return additional metadata columns in the results, for example --additional_metadata retention_time feature_id
         ```
         
         ## Build MS2Query into other tools
         If you want to incorporate MS2Query into another tool it might be easier to run MS2Query from a python script, 
         instead of running from the command line. The guide below can be used as a starting point. 
         
         Below you can find an example script for running MS2Query.
```

### Comparing `ms2query-1.2.1/README.md` & `ms2query-1.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
   --library LIBRARY_FOLDER
                         The directory containing the library spectra, to download add --download
   --ionmode {positive,negative}
                         Specify the ionization mode used
   --download            This will download the most up to date model and library.The model will be stored in the folder given as the second argumentThe model will be downloaded in the in the ionization mode specified under --mode
   --results RESULTS     The folder in which the results should be stored. The default is a new results folder in the folder with the spectra
   --filter_ionmode      Filter out all spectra that are not in the specified ion-mode. The ion mode can be specified by using --ionmode
-  --addional_metadata   Return additional metadata columns in the results, for example --additional_metadata rtinseconds feature_id
+  --addional_metadata   Return additional metadata columns in the results, for example --additional_metadata retention_time feature_id
 ```
 
 ## Build MS2Query into other tools
 If you want to incorporate MS2Query into another tool it might be easier to run MS2Query from a python script, 
 instead of running from the command line. The guide below can be used as a starting point. 
 
 Below you can find an example script for running MS2Query.
```

### Comparing `ms2query-1.2.1/ms2query/__init__.py` & `ms2query-1.2.2/ms2query/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,18 @@
     parser.add_argument("--results", action="store",
                         help="The folder in which the results should be stored. "
                              "The default is a new results folder in the folder with the spectra")
     parser.add_argument("--filter_ionmode", action="store_true",
                         help="Filter out all spectra that are not in the specified ion-mode. "
                              "The ion mode can be specified by using --ionmode")
     parser.add_argument("--additional_metadata", action="store",
-                        default=("rtinseconds", "feature_id",),
+                        default=("retention_time", "feature_id",),
                         nargs="+",
                         type=str,
-                        help="Return additional metadata columns in the results, for example --additional_metadata rtinseconds feature_id")
+                        help="Return additional metadata columns in the results, for example --additional_metadata retention_time feature_id")
     args = parser.parse_args()
     ms2query_library_files_directory = args.library
     ms2_spectra_location = args.spectra
     ion_mode = args.ionmode
     results_folder = args.results
     additional_columns = tuple(args.additional_metadata)
     if args.filter_ionmode:
```

### Comparing `ms2query-1.2.1/ms2query/benchmarking/collect_test_data_results.py` & `ms2query-1.2.2/ms2query/benchmarking/collect_test_data_results.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/benchmarking/create_accuracy_vs_recall_plot.py` & `ms2query-1.2.2/ms2query/benchmarking/create_accuracy_vs_recall_plot.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/benchmarking/k_fold_cross_validation.py` & `ms2query-1.2.2/ms2query/benchmarking/k_fold_cross_validation.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/benchmarking/visualize_mass_distribution.py` & `ms2query-1.2.2/ms2query/benchmarking/visualize_mass_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/benchmarking/visualize_tanimoto_score_distribution.py` & `ms2query-1.2.2/ms2query/benchmarking/visualize_tanimoto_score_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/clean_and_filter_spectra.py` & `ms2query-1.2.2/ms2query/clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/create_new_library/add_classifire_classifications.py` & `ms2query-1.2.2/ms2query/create_new_library/add_classifire_classifications.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/create_new_library/calculate_tanimoto_scores.py` & `ms2query-1.2.2/ms2query/create_new_library/calculate_tanimoto_scores.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/create_new_library/create_sqlite_database.py` & `ms2query-1.2.2/ms2query/create_new_library/create_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/create_new_library/library_files_creator.py` & `ms2query-1.2.2/ms2query/create_new_library/library_files_creator.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/create_new_library/split_data_for_training.py` & `ms2query-1.2.2/ms2query/create_new_library/split_data_for_training.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/create_new_library/train_models.py` & `ms2query-1.2.2/ms2query/create_new_library/train_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 This script is not needed for normally running MS2Query, it is only needed to to train
 new models
 """
 
 import os
 from spec2vec.model_building import train_new_word2vec_model
 from ms2query.create_new_library.train_ms2deepscore import train_ms2deepscore_wrapper
-from ms2query.create_new_library.train_ms2query_model import train_ms2query_model
+from ms2query.create_new_library.train_ms2query_model import train_ms2query_model, convert_to_onnx_model
 from ms2query.create_new_library.library_files_creator import LibraryFilesCreator
-from ms2query.utils import load_matchms_spectrum_objects_from_file, convert_to_onnx_model
+from ms2query.utils import load_matchms_spectrum_objects_from_file
 from ms2query.clean_and_filter_spectra import create_spectrum_documents, clean_normalize_and_split_annotated_spectra
 
 
 class SettingsTrainingModels:
     def __init__(self,
                  settings):
         default_settings = {"ms2ds_fraction_validation_spectra": 30,
```

### Comparing `ms2query-1.2.1/ms2query/create_new_library/train_ms2deepscore.py` & `ms2query-1.2.2/ms2query/create_new_library/train_ms2deepscore.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/create_new_library/train_ms2query_model.py` & `ms2query-1.2.2/ms2query/create_new_library/train_ms2query_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 This script is not needed for normally running MS2Query, it is only needed to to train
 new models
 """
 
 import os
 from typing import List
 import pandas as pd
+from onnxconverter_common import FloatTensorType
+from skl2onnx import convert_sklearn
 from tqdm import tqdm
 from matchms import Spectrum
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.metrics import mean_squared_error
 from ms2query import MS2Library
 from ms2query.query_from_sqlite_database import SqliteLibrary
 from ms2query.create_new_library.library_files_creator import LibraryFilesCreator
 from ms2query.create_new_library.split_data_for_training import split_spectra_on_inchikeys, split_training_and_validation_spectra
 from ms2query.create_new_library.calculate_tanimoto_scores import calculate_tanimoto_scores_from_smiles
-from ms2query.utils import save_pickled_file
+from ms2query.utils import save_pickled_file, return_non_existing_file_name
 
 
 class DataCollectorForTraining():
     """Class to collect data needed to train a ms2query random forest"""
     def __init__(self,
                  ms2library: MS2Library,
                  preselection_cut_off: int = 100):
@@ -138,7 +140,21 @@
 
     save_pickled_file(training_scores, os.path.join(library_files_folder, "training_scores_ms2query"))
     save_pickled_file(training_labels, os.path.join(library_files_folder, "training_labels_ms2query"))
 
     # Train MS2Query model
     ms2query_model = train_random_forest(training_scores, training_labels)
     return ms2query_model
+
+
+def convert_to_onnx_model(random_forest_model, file_name = None):
+    """The randomforest model is stored as an onnx model for backwards compatability"""
+    FloatTensorType([None, 5])
+    onnx = convert_sklearn(random_forest_model, initial_types=[("input",
+                                                        FloatTensorType([None, random_forest_model.n_features_in_]))],
+                   target_opset=12)
+    if file_name is not None:
+        file_name = return_non_existing_file_name(file_name)
+
+        with open(file_name, "wb") as file:
+            file.write(onnx.SerializeToString())
+    return onnx
```

### Comparing `ms2query-1.2.1/ms2query/ms2library.py` & `ms2query-1.2.2/ms2query/ms2library.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/old_query_from_sqlite_functions.py` & `ms2query-1.2.2/ms2query/old_query_from_sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/query_from_sqlite_database.py` & `ms2query-1.2.2/ms2query/query_from_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/results_table.py` & `ms2query-1.2.2/ms2query/results_table.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/run_ms2query.py` & `ms2query-1.2.2/ms2query/run_ms2query.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/ms2query/utils.py` & `ms2query-1.2.2/ms2query/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import os
 import sys
 import json
 from typing import List, Union, Tuple, Optional
 import numpy as np
 from matchms import importing
 from spec2vec.Spec2Vec import Spectrum
-from skl2onnx import convert_sklearn
-from skl2onnx.common.data_types import FloatTensorType
 from onnxruntime import InferenceSession
 
 
 if sys.version_info < (3, 8):
     import pickle5 as pickle
 else:
     import pickle
@@ -212,28 +210,14 @@
         self.minimal_ms2query_metascore = minimal_ms2query_metascore
         self.additional_metadata_columns = additional_metadata_columns
         self.additional_ms2query_score_columns = additional_ms2query_score_columns
         self.preselection_cut_off = preselection_cut_off
         self.filter_on_ion_mode = filter_on_ion_mode
 
 
-def convert_to_onnx_model(random_forest_model, file_name = None):
-    """The randomforest model is stored as an onnx model for backwards compatability"""
-    FloatTensorType([None, 5])
-    onnx = convert_sklearn(random_forest_model, initial_types=[("input",
-                                                        FloatTensorType([None, random_forest_model.n_features_in_]))],
-                   target_opset=12)
-    if file_name is not None:
-        file_name = return_non_existing_file_name(file_name)
-
-        with open(file_name, "wb") as file:
-            file.write(onnx.SerializeToString())
-    return onnx
-
-
 def predict_onnx_model(random_forest_onnx_model: InferenceSession, input_values):
     """Makes predictions for an onnx model"""
     # input_name = random_forest_onnx_model.get_inputs()[0].name
     predictions = random_forest_onnx_model.run(None, {"input": input_values.astype(np.float32)})
     # Converts np array of shape (n,1) to a 1D numpy array.
     predictions = predictions[0].ravel()
     return predictions
```

### Comparing `ms2query-1.2.1/ms2query.egg-info/PKG-INFO` & `ms2query-1.2.2/ms2query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
@@ -118,15 +118,15 @@
           --library LIBRARY_FOLDER
                                 The directory containing the library spectra, to download add --download
           --ionmode {positive,negative}
                                 Specify the ionization mode used
           --download            This will download the most up to date model and library.The model will be stored in the folder given as the second argumentThe model will be downloaded in the in the ionization mode specified under --mode
           --results RESULTS     The folder in which the results should be stored. The default is a new results folder in the folder with the spectra
           --filter_ionmode      Filter out all spectra that are not in the specified ion-mode. The ion mode can be specified by using --ionmode
-          --addional_metadata   Return additional metadata columns in the results, for example --additional_metadata rtinseconds feature_id
+          --addional_metadata   Return additional metadata columns in the results, for example --additional_metadata retention_time feature_id
         ```
         
         ## Build MS2Query into other tools
         If you want to incorporate MS2Query into another tool it might be easier to run MS2Query from a python script, 
         instead of running from the command line. The guide below can be used as a starting point. 
         
         Below you can find an example script for running MS2Query.
```

### Comparing `ms2query-1.2.1/ms2query.egg-info/SOURCES.txt` & `ms2query-1.2.2/ms2query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/setup.py` & `ms2query-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         "tensorflow-macos<2.9;platform_machine=='arm64'", #Add for Macos M1 chip compatability
         "tensorflow-metal==0.5.0;platform_machine=='arm64'",
         "tensorflow<2.9;platform_machine!='arm64'", #tensorflow <2.9 for change in error bar plotting
         "scikit-learn",
         "ms2deepscore",
         "gensim>=4.0.0",
         "pandas>=1.2.5,<2.0.0",
-        "matchmsextras>=0.4.0",
+        "matchmsextras==0.4.0",
         "pubchempy", #This is a dependency for matchmsextras, which is missing in setup
         "tqdm",
         "matplotlib",
         "skl2onnx",
         "onnxruntime",
     ],
     extras_require={':python_version < "3.8"': ["pickle5",],
```

### Comparing `ms2query-1.2.1/tests/conftest.py` & `ms2query-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_add_classifier_annotations.py` & `ms2query-1.2.2/tests/test_add_classifier_annotations.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_calculate_tanimoto_scores.py` & `ms2query-1.2.2/tests/test_calculate_tanimoto_scores.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_clean_and_filter_spectra.py` & `ms2query-1.2.2/tests/test_clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_collect_test_data_results.py` & `ms2query-1.2.2/tests/test_collect_test_data_results.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_library_files_creator.py` & `ms2query-1.2.2/tests/test_library_files_creator.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_ms2library.py` & `ms2query-1.2.2/tests/test_ms2library.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_results_table.py` & `ms2query-1.2.2/tests/test_results_table.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_run_ms2query.py` & `ms2query-1.2.2/tests/test_run_ms2query.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_split_data_for_training.py` & `ms2query-1.2.2/tests/test_split_data_for_training.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_sqlite.py` & `ms2query-1.2.2/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_train_models.py` & `ms2query-1.2.2/tests/test_train_models.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_train_ms2deepscore.py` & `ms2query-1.2.2/tests/test_train_ms2deepscore.py`

 * *Files identical despite different names*

### Comparing `ms2query-1.2.1/tests/test_train_ms2query_model.py` & `ms2query-1.2.2/tests/test_train_ms2query_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import os
+
+import numpy as np
 import pytest
 import sys
 import pandas as pd
 from ms2query.create_new_library.train_ms2query_model import \
-    DataCollectorForTraining, calculate_tanimoto_scores_with_library, train_random_forest, train_ms2query_model
-from ms2query.utils import load_pickled_file, load_matchms_spectrum_objects_from_file, convert_to_onnx_model
+    DataCollectorForTraining, calculate_tanimoto_scores_with_library, train_random_forest, train_ms2query_model, \
+    convert_to_onnx_model
+from ms2query.utils import load_pickled_file, load_matchms_spectrum_objects_from_file, load_ms2query_model, \
+    predict_onnx_model
 from onnxruntime import InferenceSession
 from ms2query.utils import predict_onnx_model
 from ms2query.ms2library import MS2Library
 
 
 if sys.version_info < (3, 8):
     pass
@@ -72,23 +76,27 @@
     expected_result = pd.DataFrame([0.199695, 0.177669, 0.192504],
                                    index=spectra_ids_list,
                                    columns=["Tanimoto_score"])
     assert isinstance(result, pd.DataFrame), "Expected a pd.Dataframe"
     pd.testing.assert_frame_equal(result, expected_result, check_dtype=False)
 
 
-def test_train_random_forest():
+def test_train_and_save_random_forest():
     training_scores, training_labels = load_pickled_file(os.path.join(
         os.path.split(os.path.dirname(__file__))[0],
         "tests/test_files/test_files_train_ms2query_nn",
         "expected_train_and_val_data.pickle"))[:2]
     ms2query_model = train_random_forest(training_scores, training_labels)
     onnx_model = convert_to_onnx_model(ms2query_model)
     onnx_model_session = InferenceSession(onnx_model.SerializeToString())
-    predictions = predict_onnx_model(onnx_model_session, training_scores.values)
+    predictions_onnx_model = predict_onnx_model(onnx_model_session, training_scores.values)
+
+    # check if saving onnx model works
+    predictions_sklearn_model = ms2query_model.predict(training_scores.values.astype(np.float32))
+    assert np.allclose(predictions_onnx_model, predictions_sklearn_model)
 
 
 @pytest.mark.integration
 def test_train_ms2query_model(path_to_general_test_files, tmp_path, hundred_test_spectra):
     models_folder = os.path.join(tmp_path, "models")
     ms2query_model = train_ms2query_model(
         training_spectra=hundred_test_spectra,
```

### Comparing `ms2query-1.2.1/tests/test_utils.py` & `ms2query-1.2.2/tests/test_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import os
 from io import StringIO
 from typing import List
 
-import numpy as np
 import pandas as pd
 import pytest
 from matchms import Spectrum
 from ms2query.utils import (add_unknown_charges_to_spectra,
-                            load_matchms_spectrum_objects_from_file,
-                            load_pickled_file,
-                            convert_to_onnx_model, load_ms2query_model, predict_onnx_model)
+                            load_matchms_spectrum_objects_from_file)
 
 
 def test_convert_files_to_matchms_spectrum_objects_unknown_file(tmp_path):
     """Tests if unknown file raises an Assertion error"""
     with pytest.raises(AssertionError):
         load_matchms_spectrum_objects_from_file(os.path.join(tmp_path, "file_that_does_not_exist.json"))
 
@@ -47,32 +44,14 @@
         assert spectrum.get("charge") == 1, "The charge is expected to be 1"
     for spectrum in spectra_with_charge[20:30]:
         assert spectrum.get("charge") == -1, "The charge is expected to be -1"
     for spectrum in spectra_with_charge[30:]:
         assert spectrum.get("charge") == 2, "The charge is expected to be 2"
 
 
-def test_save_as_onnx_model(tmp_path):
-    path_to_test_dir = os.path.join(
-        os.path.split(os.path.dirname(__file__))[0],
-        'tests/test_files/')
-    rf_model_file = os.path.join(path_to_test_dir, 'general_test_files', "test_ms2q_rf_model.pickle")
-    rf_model = load_pickled_file(rf_model_file)
-    expected_result = load_pickled_file(os.path.join(
-        os.path.split(os.path.dirname(__file__))[0],
-        "tests/test_files/test_files_train_ms2query_nn",
-        "expected_train_and_val_data.pickle"))[0]
-    new_model = os.path.join(tmp_path, "rf_model.onnx")
-    convert_to_onnx_model(rf_model, new_model)
-    ms2query_model = load_ms2query_model(new_model)
-    result = predict_onnx_model(ms2query_model, expected_result.values)
-    original_result = rf_model.predict(expected_result.values.astype(np.float32))
-    assert np.allclose(result, original_result)
-
-
 def check_correct_results_csv_file(dataframe_found: pd.DataFrame,
                                    expected_headers: List[str],
                                    nr_of_rows_to_check=2):
     # Define expected results
     csv_format_expected_results ="""query_spectrum_nr,ms2query_model_prediction,precursor_mz_difference,precursor_mz_query_spectrum,precursor_mz_analog,inchikey,spectrum_id,analog_compound_name,charge,s2v_score,ms2ds_score,retention_time,retention_index,smiles,cf_kingdom,cf_superclass,cf_class,cf_subclass,cf_direct_parent,npc_class_results,npc_superclass_results,npc_pathway_results\n
         1,0.5645,33.2500,907.0000,940.2500,KNGPFNUOXXLKCN,CCMSLIB00000001760,Hoiamide B,1,0.9996,0.9232,,,CCC[C@@H](C)[C@@H]([C@H](C)[C@@H]1[C@H]([C@H](Cc2nc(cs2)C3=N[C@](CS3)(C4=N[C@](CS4)(C(=O)N[C@H]([C@H]([C@H](C(=O)O[C@H](C(=O)N[C@H](C(=O)O1)[C@@H](C)O)[C@@H](C)CC)C)O)[C@@H](C)CC)C)C)OC)C)O,b,c,d,e,f,g,h,i\n
         2,0.4090,61.3670,928.0000,866.6330,GRJSOZDXIUZXEW,CCMSLIB00000001761,Halovir A,0,0.9621,0.4600,,,CCCCCCCCCCCCCC(=O)NC(C)(C)C(=O)N1C[C@H](O)C[C@H]1C(=O)NC(CC(C)C)C(=O)N[C@@H](C(C)C)C(=O)N[C@@H](CCC(N)=O)C(=O)N[C@H](CO)CC(C)C,b,c,d,e,f,g,h,i\n"""
```

