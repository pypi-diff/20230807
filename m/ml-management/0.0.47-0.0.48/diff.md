# Comparing `tmp/ml-management-0.0.47.tar.gz` & `tmp/ml-management-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.47.tar", last modified: Mon Jul 31 18:02:28 2023, max compression
+gzip compressed data, was "ml-management-0.0.48.tar", last modified: Mon Aug  7 11:17:10 2023, max compression
```

## Comparing `ml-management-0.0.47.tar` & `ml-management-0.0.48.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.660085 ml-management-0.0.47/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       18 2023-06-29 11:52:32.000000 ml-management-0.0.47/MANIFEST.in
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.656085 ml-management-0.0.47/ML_management/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/__init__.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.656085 ml-management-0.0.47/ML_management/collectors/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      120 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/collectors/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1092 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      456 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1318 2023-07-11 12:32:50.000000 ml-management-0.0.47/ML_management/collectors/collectors.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.656085 ml-management-0.0.47/ML_management/collectors/dummy/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      463 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.656085 ml-management-0.0.47/ML_management/collectors/s3/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9711 2023-07-10 10:35:03.000000 ml-management-0.0.47/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.656085 ml-management-0.0.47/ML_management/collectors/topic_markers/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)   331440 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3167 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.656085 ml-management-0.0.47/ML_management/dataset_loader_template/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4373 2023-07-19 11:55:30.000000 ml-management-0.0.47/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.656085 ml-management-0.0.47/ML_management/executor_template/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.656085 ml-management-0.0.47/ML_management/executor_template/default_executors/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      895 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      843 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      869 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     6505 2023-07-19 11:55:30.000000 ml-management-0.0.47/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      402 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      334 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.660085 ml-management-0.0.47/ML_management/mlmanagement/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      694 2023-07-31 17:52:51.000000 ml-management-0.0.47/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2639 2023-07-24 14:01:37.000000 ml-management-0.0.47/ML_management/mlmanagement/abstract_mlflow_client.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      380 2023-07-20 08:59:05.000000 ml-management-0.0.47/ML_management/mlmanagement/base_exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3392 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5054 2023-07-11 12:32:50.000000 ml-management-0.0.47/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    16629 2023-07-31 17:52:51.000000 ml-management-0.0.47/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    10945 2023-07-31 17:52:51.000000 ml-management-0.0.47/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      201 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2751 2023-07-31 17:58:01.000000 ml-management-0.0.47/ML_management/mlmanagement/module_finder.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5121 2023-07-20 08:59:05.000000 ml-management-0.0.47/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      371 2023-07-24 14:01:37.000000 ml-management-0.0.47/ML_management/mlmanagement/singleton_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      269 2023-07-26 12:02:49.000000 ml-management-0.0.47/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.660085 ml-management-0.0.47/ML_management/models/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/models/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      949 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.660085 ml-management-0.0.47/ML_management/models/patterns/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4865 2023-07-19 11:55:30.000000 ml-management-0.0.47/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      561 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      445 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.660085 ml-management-0.0.47/ML_management/registry/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/registry/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3362 2023-07-24 14:01:37.000000 ml-management-0.0.47/ML_management/registry/abstract_registry_manager.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2765 2023-07-24 14:01:37.000000 ml-management-0.0.47/ML_management/registry/exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4264 2023-07-24 14:01:37.000000 ml-management-0.0.47/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.660085 ml-management-0.0.47/ML_management/tests/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/tests/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3361 2023-07-11 12:32:50.000000 ml-management-0.0.47/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9858 2023-07-11 12:32:50.000000 ml-management-0.0.47/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.660085 ml-management-0.0.47/ML_management/uploader_data/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.47/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1914 2023-07-10 10:35:03.000000 ml-management-0.0.47/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1430 2023-07-10 10:35:03.000000 ml-management-0.0.47/ML_management/uploader_data/utils.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-07-31 18:02:28.660085 ml-management-0.0.47/PKG-INFO
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       56 2023-06-29 11:52:32.000000 ml-management-0.0.47/README.md
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        7 2023-07-31 18:00:31.000000 ml-management-0.0.47/VERSION
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-31 18:02:28.660085 ml-management-0.0.47/ml_management.egg-info/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-07-31 18:02:28.000000 ml-management-0.0.47/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2729 2023-07-31 18:02:28.000000 ml-management-0.0.47/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        1 2023-07-31 18:02:28.000000 ml-management-0.0.47/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      166 2023-07-31 18:02:28.000000 ml-management-0.0.47/ml_management.egg-info/requires.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       14 2023-07-31 18:02:28.000000 ml-management-0.0.47/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       38 2023-07-31 18:02:28.660085 ml-management-0.0.47/setup.cfg
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1076 2023-07-31 17:34:33.000000 ml-management-0.0.47/setup.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.773285 ml-management-0.0.48/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       18 2023-06-29 11:52:32.000000 ml-management-0.0.48/MANIFEST.in
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.765285 ml-management-0.0.48/ML_management/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/__init__.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.769285 ml-management-0.0.48/ML_management/collectors/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      120 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/collectors/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1092 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      456 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1318 2023-07-11 12:32:50.000000 ml-management-0.0.48/ML_management/collectors/collectors.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.769285 ml-management-0.0.48/ML_management/collectors/dummy/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      463 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.769285 ml-management-0.0.48/ML_management/collectors/s3/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9711 2023-07-10 10:35:03.000000 ml-management-0.0.48/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.769285 ml-management-0.0.48/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)   331440 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3167 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.769285 ml-management-0.0.48/ML_management/dataset_loader_template/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4373 2023-07-19 11:55:30.000000 ml-management-0.0.48/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.769285 ml-management-0.0.48/ML_management/executor_template/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.769285 ml-management-0.0.48/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      895 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      843 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      869 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     6505 2023-07-19 11:55:30.000000 ml-management-0.0.48/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      402 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      334 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.769285 ml-management-0.0.48/ML_management/mlmanagement/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      694 2023-08-01 08:58:20.000000 ml-management-0.0.48/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2639 2023-07-24 14:01:37.000000 ml-management-0.0.48/ML_management/mlmanagement/abstract_mlflow_client.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      380 2023-07-20 08:59:05.000000 ml-management-0.0.48/ML_management/mlmanagement/base_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3392 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5054 2023-07-11 12:32:50.000000 ml-management-0.0.48/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    16629 2023-08-01 08:58:20.000000 ml-management-0.0.48/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    10945 2023-08-01 08:58:20.000000 ml-management-0.0.48/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      201 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2751 2023-08-01 08:58:20.000000 ml-management-0.0.48/ML_management/mlmanagement/module_finder.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5121 2023-07-20 08:59:05.000000 ml-management-0.0.48/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      371 2023-07-24 14:01:37.000000 ml-management-0.0.48/ML_management/mlmanagement/singleton_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      269 2023-07-26 12:02:49.000000 ml-management-0.0.48/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.769285 ml-management-0.0.48/ML_management/models/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/models/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      949 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.769285 ml-management-0.0.48/ML_management/models/patterns/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4865 2023-07-19 11:55:30.000000 ml-management-0.0.48/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      561 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      445 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.769285 ml-management-0.0.48/ML_management/registry/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/registry/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3362 2023-07-24 14:01:37.000000 ml-management-0.0.48/ML_management/registry/abstract_registry_manager.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2765 2023-07-24 14:01:37.000000 ml-management-0.0.48/ML_management/registry/exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4264 2023-07-24 14:01:37.000000 ml-management-0.0.48/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.773285 ml-management-0.0.48/ML_management/tests/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/tests/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3361 2023-07-11 12:32:50.000000 ml-management-0.0.48/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9858 2023-07-11 12:32:50.000000 ml-management-0.0.48/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.773285 ml-management-0.0.48/ML_management/uploader_data/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.48/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1914 2023-07-10 10:35:03.000000 ml-management-0.0.48/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1430 2023-07-10 10:35:03.000000 ml-management-0.0.48/ML_management/uploader_data/utils.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-08-07 11:17:10.773285 ml-management-0.0.48/PKG-INFO
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       56 2023-06-29 11:52:32.000000 ml-management-0.0.48/README.md
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        7 2023-08-07 10:51:00.000000 ml-management-0.0.48/VERSION
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-08-07 11:17:10.773285 ml-management-0.0.48/ml_management.egg-info/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-08-07 11:17:10.000000 ml-management-0.0.48/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2729 2023-08-07 11:17:10.000000 ml-management-0.0.48/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        1 2023-08-07 11:17:10.000000 ml-management-0.0.48/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      102 2023-08-07 11:17:10.000000 ml-management-0.0.48/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       14 2023-08-07 11:17:10.000000 ml-management-0.0.48/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       38 2023-08-07 11:17:10.773285 ml-management-0.0.48/setup.cfg
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      918 2023-08-07 10:46:45.000000 ml-management-0.0.48/setup.py
```

### Comparing `ml-management-0.0.47/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.48/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/collectors/collectors.py` & `ml-management-0.0.48/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.48/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.48/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.48/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.48/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.48/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.48/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.48/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.48/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.48/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/mlmanagement/abstract_mlflow_client.py` & `ml-management-0.0.48/ML_management/mlmanagement/abstract_mlflow_client.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.48/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.48/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.48/ML_management/mlmanagement/mlmanagement.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.48/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/mlmanagement/module_finder.py` & `ml-management-0.0.48/ML_management/mlmanagement/module_finder.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.48/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.48/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.48/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.48/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/registry/abstract_registry_manager.py` & `ml-management-0.0.48/ML_management/registry/abstract_registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/registry/exceptions.py` & `ml-management-0.0.48/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/registry/registry_manager.py` & `ml-management-0.0.48/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.48/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.48/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.48/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ML_management/uploader_data/utils.py` & `ml-management-0.0.48/ML_management/uploader_data/utils.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.48/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.47/setup.py` & `ml-management-0.0.48/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,18 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ISPRAS MODIS",
     author_email="modis@ispras.ru",
     maintainer="Maxim Ryndin",
     packages=find_packages(include=["ML_management", "ML_management.*"]),
     include_package_data=True,
-    # jsonschema 2.6.0 is the last one to support python 3.6
     install_requires=[
         "sgqlc==16.1",
         "mlflow==2.4.0",
-        "pandas>=0.20.1,<=1.5.2",
-        "numpy>=1.8.1,<=1.23.5",
-        "jsonschema==2.6.0",
-        "requests_toolbelt>=0.9.1,<=0.10.1",
-        "boto3==1.21.21",
-        "protobuf<4.0.0",
+        "boto3==1.28.15",
+        "jsonschema==4.18.4",
+        "requests_toolbelt>=0.9.1,<=1",
         "tqdm==4.65.0",
     ],
     data_files=[("", ["VERSION"])],
     python_requires=">=3.8",
 )
```

