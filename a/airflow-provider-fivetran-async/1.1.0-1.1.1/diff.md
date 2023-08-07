# Comparing `tmp/airflow-provider-fivetran-async-1.1.0.tar.gz` & `tmp/airflow-provider-fivetran-async-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-fivetran-async-1.1.0.tar", last modified: Fri Jun 16 16:27:05 2023, max compression
+gzip compressed data, was "airflow-provider-fivetran-async-1.1.1.tar", last modified: Mon Aug  7 12:00:38 2023, max compression
```

## Comparing `airflow-provider-fivetran-async-1.1.0.tar` & `airflow-provider-fivetran-async-1.1.1.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.422975 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 16:27:05.000000 airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/example_dags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/example_dags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/example_dags/example_fivetran_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/utils/operator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/common/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.426975 airflow-provider-fivetran-async-1.1.0/tests/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/hooks/test_fivetran.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/tests/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/operators/test_fivetran.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/tests/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/sensors/test_fivetran.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/tests/triggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/triggers/test_fivetran.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:27:05.430976 airflow-provider-fivetran-async-1.1.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-16 16:26:48.000000 airflow-provider-fivetran-async-1.1.0/tests/utils/test_operator_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.291629 airflow-provider-fivetran-async-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-08-07 12:00:38.291629 airflow-provider-fivetran-async-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.287629 airflow-provider-fivetran-async-1.1.1/airflow_provider_fivetran_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-08-07 12:00:38.000000 airflow-provider-fivetran-async-1.1.1/airflow_provider_fivetran_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-07 12:00:38.000000 airflow-provider-fivetran-async-1.1.1/airflow_provider_fivetran_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:00:38.000000 airflow-provider-fivetran-async-1.1.1/airflow_provider_fivetran_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-07 12:00:38.000000 airflow-provider-fivetran-async-1.1.1/airflow_provider_fivetran_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-07 12:00:38.000000 airflow-provider-fivetran-async-1.1.1/airflow_provider_fivetran_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-07 12:00:38.000000 airflow-provider-fivetran-async-1.1.1/airflow_provider_fivetran_async.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.287629 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.287629 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/example_dags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/example_dags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/example_dags/example_fivetran.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/example_dags/example_fivetran_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/example_dags/example_fivetran_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/example_dags/example_fivetran_bqml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/example_dags/example_fivetran_dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/example_dags/example_fivetran_xcom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29201 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.287629 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/utils/operator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-07 12:00:38.291629 airflow-provider-fivetran-async-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.287629 airflow-provider-fivetran-async-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.291629 airflow-provider-fivetran-async-1.1.1/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/common/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.291629 airflow-provider-fivetran-async-1.1.1/tests/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24562 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/hooks/test_fivetran.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.291629 airflow-provider-fivetran-async-1.1.1/tests/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/operators/test_fivetran.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.291629 airflow-provider-fivetran-async-1.1.1/tests/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/sensors/test_fivetran.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.291629 airflow-provider-fivetran-async-1.1.1/tests/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/triggers/test_fivetran.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:38.291629 airflow-provider-fivetran-async-1.1.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-08-07 12:00:17.000000 airflow-provider-fivetran-async-1.1.1/tests/utils/test_operator_utils.py
```

### Comparing `airflow-provider-fivetran-async-1.1.0/PKG-INFO` & `airflow-provider-fivetran-async-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-fivetran-async
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Fivetran async provider for Apache Airflow
 Home-page: https://github.com/astronomer/airflow-provider-fivetran-async
 Author: Astronomer & Fivetran
 Author-email: humans@astronomer.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/astronomer/airflow-provider-fivetran-async
 Project-URL: Changelog, https://github.com/astronomer/airflow-provider-fivetran-async/blob/main/CHANGELOG.md
@@ -15,25 +15,26 @@
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: openlineage
 Provides-Extra: all
 
 # Fivetran Async Provider for Apache Airflow
 
 This package provides an async operator, sensor and hook that integrates [Fivetran](https://fivetran.com) into Apache Airflow.
-`FivetranSensorAsync` allows you to monitor a Fivetran sync job for completion before running downstream processes.
-`FivetranOperatorAsync` submits a Fivetran sync job and polls for its status on the triggerer.
+`FivetranSensor` allows you to monitor a Fivetran sync job for completion before running downstream processes.
+`FivetranOperator` submits a Fivetran sync job and polls for its status on the triggerer.
 Since an async sensor or operator frees up worker slot while polling is happening on the triggerer,
 they consume less resources when compared to traditional "sync" sensors and operators.
 
 [Fivetran automates your data pipeline, and Airflow automates your data processing.](https://www.youtube.com/watch?v=siSx6L2ckSw&ab_channel=Fivetran)
 
 ## Installation
 
@@ -56,38 +57,38 @@
 
 The sensor assumes the `Conn Id` is set to `fivetran`, however if you are managing multiple Fivetran accounts, you can set this to anything you like. See the DAG in examples to see how to specify a custom `Conn Id`.
 
 ## Modules
 
 ### [Fivetran Operator Async](https://github.com/astronomer/airflow-provider-fivetran-async/tree/main/fivetran_provider_async/operators.py)
 
-`FivetranOperatorAsync` submits a Fivetran sync job and monitors it on trigger for completion.
+`FivetranOperator` submits a Fivetran sync job and monitors it on trigger for completion.
 It requires that you specify the `connector_id` of the sync job to start. You can find `connector_id` in the Settings page of the connector you configured in the [Fivetran dashboard](https://fivetran.com/dashboard/connectors).
 
 Import into your DAG via:
 ```python
-from fivetran_provider_async.operators import FivetranOperatorAsync
+from fivetran_provider_async.operators import FivetranOperator
 ```
 
 ### [Fivetran Sensor Async](https://github.com/astronomer/airflow-provider-fivetran-async/tree/main/fivetran_provider_async/sensors.py)
 
-`FivetranSensorAsync` monitors a Fivetran sync job for completion.
-Monitoring with `FivetranSensorAsync` allows you to trigger downstream processes only when the Fivetran sync jobs have completed, ensuring data consistency.
+`FivetranSensor` monitors a Fivetran sync job for completion.
+Monitoring with `FivetranSensor` allows you to trigger downstream processes only when the Fivetran sync jobs have completed, ensuring data consistency.
 
 
 
-You can use multiple instances of `FivetranSensorAsync` to monitor multiple Fivetran connectors.
+You can use multiple instances of `FivetranSensor` to monitor multiple Fivetran connectors.
 
 If used in this way,
 
-`FivetranSensorAsync` requires that you specify the `connector_id` of the sync job to start. You can find `connector_id` in the Settings page of the connector you configured in the [Fivetran dashboard](https://fivetran.com/dashboard/connectors).
+`FivetranSensor` requires that you specify the `connector_id` of the sync job to start. You can find `connector_id` in the Settings page of the connector you configured in the [Fivetran dashboard](https://fivetran.com/dashboard/connectors).
 
 Import into your DAG via:
 ```python
-from fivetran_provider_async.sensors import FivetranSensorAsync
+from fivetran_provider_async.sensors import FivetranSensor
 ```
 
 ## Examples
 
 See the [**examples**](https://github.com/astronomer/airflow-provider-fivetran-async/tree/main/fivetran_provider_async/example_dags) directory for an example DAG.
 
 ## Issues
```

### Comparing `airflow-provider-fivetran-async-1.1.0/README.md` & `airflow-provider-fivetran-async-1.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Fivetran Async Provider for Apache Airflow
 
 This package provides an async operator, sensor and hook that integrates [Fivetran](https://fivetran.com) into Apache Airflow.
-`FivetranSensorAsync` allows you to monitor a Fivetran sync job for completion before running downstream processes.
-`FivetranOperatorAsync` submits a Fivetran sync job and polls for its status on the triggerer.
+`FivetranSensor` allows you to monitor a Fivetran sync job for completion before running downstream processes.
+`FivetranOperator` submits a Fivetran sync job and polls for its status on the triggerer.
 Since an async sensor or operator frees up worker slot while polling is happening on the triggerer,
 they consume less resources when compared to traditional "sync" sensors and operators.
 
 [Fivetran automates your data pipeline, and Airflow automates your data processing.](https://www.youtube.com/watch?v=siSx6L2ckSw&ab_channel=Fivetran)
 
 ## Installation
 
@@ -29,38 +29,38 @@
 
 The sensor assumes the `Conn Id` is set to `fivetran`, however if you are managing multiple Fivetran accounts, you can set this to anything you like. See the DAG in examples to see how to specify a custom `Conn Id`.
 
 ## Modules
 
 ### [Fivetran Operator Async](https://github.com/astronomer/airflow-provider-fivetran-async/tree/main/fivetran_provider_async/operators.py)
 
-`FivetranOperatorAsync` submits a Fivetran sync job and monitors it on trigger for completion.
+`FivetranOperator` submits a Fivetran sync job and monitors it on trigger for completion.
 It requires that you specify the `connector_id` of the sync job to start. You can find `connector_id` in the Settings page of the connector you configured in the [Fivetran dashboard](https://fivetran.com/dashboard/connectors).
 
 Import into your DAG via:
 ```python
-from fivetran_provider_async.operators import FivetranOperatorAsync
+from fivetran_provider_async.operators import FivetranOperator
 ```
 
 ### [Fivetran Sensor Async](https://github.com/astronomer/airflow-provider-fivetran-async/tree/main/fivetran_provider_async/sensors.py)
 
-`FivetranSensorAsync` monitors a Fivetran sync job for completion.
-Monitoring with `FivetranSensorAsync` allows you to trigger downstream processes only when the Fivetran sync jobs have completed, ensuring data consistency.
+`FivetranSensor` monitors a Fivetran sync job for completion.
+Monitoring with `FivetranSensor` allows you to trigger downstream processes only when the Fivetran sync jobs have completed, ensuring data consistency.
 
 
 
-You can use multiple instances of `FivetranSensorAsync` to monitor multiple Fivetran connectors.
+You can use multiple instances of `FivetranSensor` to monitor multiple Fivetran connectors.
 
 If used in this way,
 
-`FivetranSensorAsync` requires that you specify the `connector_id` of the sync job to start. You can find `connector_id` in the Settings page of the connector you configured in the [Fivetran dashboard](https://fivetran.com/dashboard/connectors).
+`FivetranSensor` requires that you specify the `connector_id` of the sync job to start. You can find `connector_id` in the Settings page of the connector you configured in the [Fivetran dashboard](https://fivetran.com/dashboard/connectors).
 
 Import into your DAG via:
 ```python
-from fivetran_provider_async.sensors import FivetranSensorAsync
+from fivetran_provider_async.sensors import FivetranSensor
 ```
 
 ## Examples
 
 See the [**examples**](https://github.com/astronomer/airflow-provider-fivetran-async/tree/main/fivetran_provider_async/example_dags) directory for an example DAG.
 
 ## Issues
```

### Comparing `airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/PKG-INFO` & `airflow-provider-fivetran-async-1.1.1/airflow_provider_fivetran_async.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-fivetran-async
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Fivetran async provider for Apache Airflow
 Home-page: https://github.com/astronomer/airflow-provider-fivetran-async
 Author: Astronomer & Fivetran
 Author-email: humans@astronomer.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/astronomer/airflow-provider-fivetran-async
 Project-URL: Changelog, https://github.com/astronomer/airflow-provider-fivetran-async/blob/main/CHANGELOG.md
@@ -15,25 +15,26 @@
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: openlineage
 Provides-Extra: all
 
 # Fivetran Async Provider for Apache Airflow
 
 This package provides an async operator, sensor and hook that integrates [Fivetran](https://fivetran.com) into Apache Airflow.
-`FivetranSensorAsync` allows you to monitor a Fivetran sync job for completion before running downstream processes.
-`FivetranOperatorAsync` submits a Fivetran sync job and polls for its status on the triggerer.
+`FivetranSensor` allows you to monitor a Fivetran sync job for completion before running downstream processes.
+`FivetranOperator` submits a Fivetran sync job and polls for its status on the triggerer.
 Since an async sensor or operator frees up worker slot while polling is happening on the triggerer,
 they consume less resources when compared to traditional "sync" sensors and operators.
 
 [Fivetran automates your data pipeline, and Airflow automates your data processing.](https://www.youtube.com/watch?v=siSx6L2ckSw&ab_channel=Fivetran)
 
 ## Installation
 
@@ -56,38 +57,38 @@
 
 The sensor assumes the `Conn Id` is set to `fivetran`, however if you are managing multiple Fivetran accounts, you can set this to anything you like. See the DAG in examples to see how to specify a custom `Conn Id`.
 
 ## Modules
 
 ### [Fivetran Operator Async](https://github.com/astronomer/airflow-provider-fivetran-async/tree/main/fivetran_provider_async/operators.py)
 
-`FivetranOperatorAsync` submits a Fivetran sync job and monitors it on trigger for completion.
+`FivetranOperator` submits a Fivetran sync job and monitors it on trigger for completion.
 It requires that you specify the `connector_id` of the sync job to start. You can find `connector_id` in the Settings page of the connector you configured in the [Fivetran dashboard](https://fivetran.com/dashboard/connectors).
 
 Import into your DAG via:
 ```python
-from fivetran_provider_async.operators import FivetranOperatorAsync
+from fivetran_provider_async.operators import FivetranOperator
 ```
 
 ### [Fivetran Sensor Async](https://github.com/astronomer/airflow-provider-fivetran-async/tree/main/fivetran_provider_async/sensors.py)
 
-`FivetranSensorAsync` monitors a Fivetran sync job for completion.
-Monitoring with `FivetranSensorAsync` allows you to trigger downstream processes only when the Fivetran sync jobs have completed, ensuring data consistency.
+`FivetranSensor` monitors a Fivetran sync job for completion.
+Monitoring with `FivetranSensor` allows you to trigger downstream processes only when the Fivetran sync jobs have completed, ensuring data consistency.
 
 
 
-You can use multiple instances of `FivetranSensorAsync` to monitor multiple Fivetran connectors.
+You can use multiple instances of `FivetranSensor` to monitor multiple Fivetran connectors.
 
 If used in this way,
 
-`FivetranSensorAsync` requires that you specify the `connector_id` of the sync job to start. You can find `connector_id` in the Settings page of the connector you configured in the [Fivetran dashboard](https://fivetran.com/dashboard/connectors).
+`FivetranSensor` requires that you specify the `connector_id` of the sync job to start. You can find `connector_id` in the Settings page of the connector you configured in the [Fivetran dashboard](https://fivetran.com/dashboard/connectors).
 
 Import into your DAG via:
 ```python
-from fivetran_provider_async.sensors import FivetranSensorAsync
+from fivetran_provider_async.sensors import FivetranSensor
 ```
 
 ## Examples
 
 See the [**examples**](https://github.com/astronomer/airflow-provider-fivetran-async/tree/main/fivetran_provider_async/example_dags) directory for an example DAG.
 
 ## Issues
```

### Comparing `airflow-provider-fivetran-async-1.1.0/airflow_provider_fivetran_async.egg-info/SOURCES.txt` & `airflow-provider-fivetran-async-1.1.1/airflow_provider_fivetran_async.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 airflow_provider_fivetran_async.egg-info/top_level.txt
 fivetran_provider_async/__init__.py
 fivetran_provider_async/hooks.py
 fivetran_provider_async/operators.py
 fivetran_provider_async/sensors.py
 fivetran_provider_async/triggers.py
 fivetran_provider_async/example_dags/__init__.py
+fivetran_provider_async/example_dags/example_fivetran.py
 fivetran_provider_async/example_dags/example_fivetran_async.py
+fivetran_provider_async/example_dags/example_fivetran_bigquery.py
+fivetran_provider_async/example_dags/example_fivetran_bqml.py
+fivetran_provider_async/example_dags/example_fivetran_dbt.py
+fivetran_provider_async/example_dags/example_fivetran_xcom.py
 fivetran_provider_async/utils/__init__.py
 fivetran_provider_async/utils/operator_utils.py
 tests/__init__.py
 tests/common/__init__.py
 tests/common/static.py
 tests/hooks/__init__.py
 tests/hooks/test_fivetran.py
```

### Comparing `airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/__init__.py` & `airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa F401
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 import logging
 
 log = logging.getLogger(__name__)
 
 
 try:
```

### Comparing `airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/hooks.py` & `airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/operators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,224 +1,208 @@
-import asyncio
-import time
-from typing import Any, Dict, cast
-
-import aiohttp
-import pendulum
-from aiohttp import ClientResponseError
-from airflow.exceptions import AirflowException
-from asgiref.sync import sync_to_async
-from fivetran_provider.hooks.fivetran import FivetranHook
-
+from __future__ import annotations
 
-class FivetranHookAsync(FivetranHook):
-    """
-    Fivetran API interaction hook extending FivetranHook for asynchronous fuctionality.
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
-    :param fivetran_conn_id: `Conn ID` of the Connection to be used to
-        configure this hook.
-    :type fivetran_conn_id: str
-    :param timeout_seconds: The amount of time in seconds the requests library
-        will wait before timing out.
-    :type timeout_seconds: int
-    :param retry_limit: The number of times to retry the connection in case of
-        service outages.
-    :type retry_limit: int
-    :param retry_delay: The number of seconds to wait between retries.
-    :type retry_delay: float
-    """
+from airflow.exceptions import AirflowException
+from airflow.models import BaseOperator, BaseOperatorLink
 
-    api_user_agent = "airflow_provider_fivetran_async/1.0.0"
+if TYPE_CHECKING:
+    from airflow.utils.context import Context
 
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
+from fivetran_provider_async.hooks import FivetranHook
+from fivetran_provider_async.triggers import FivetranTrigger
+from fivetran_provider_async.utils.operator_utils import datasets
 
-    async def _do_api_call_async(self, endpoint_info, json=None):
-        method, endpoint = endpoint_info
 
-        if not self.fivetran_conn:
-            self.fivetran_conn = await sync_to_async(self.get_connection)(self.conn_id)
-        auth = (self.fivetran_conn.login, self.fivetran_conn.password)
-        url = f"{self.api_protocol}://{self.api_host}/{endpoint}"
-        headers = {"User-Agent": self.api_user_agent}
-
-        async with aiohttp.ClientSession() as session:
-            if method == "GET":
-                request_func = session.get
-            elif method == "POST":
-                request_func = session.post
-                headers.update({"Content-Type": "application/json;version=2"})
-            elif method == "PATCH":
-                request_func = session.patch
-                headers.update({"Content-Type": "application/json;version=2"})
-            else:
-                raise AirflowException("Unexpected HTTP Method: " + method)
-
-            attempt_num = 1
-            while True:
-                try:
-                    response = await request_func(
-                        url,
-                        data=json if method in ("POST", "PATCH") else None,
-                        params=json if method == "GET" else None,
-                        auth=aiohttp.BasicAuth(login=auth[0], password=auth[1]),
-                        headers=headers,
-                    )
-                    response.raise_for_status()
-                    return cast(Dict[str, Any], await response.json())
-                except ClientResponseError as e:
-                    if not _retryable_error_async(e):
-                        # In this case, the user probably made a mistake.
-                        # Don't retry.
-                        return {"Response": {e.message}, "Status Code": {e.status}}
-                    self._log_request_error(attempt_num, str(e))
-
-                if attempt_num == self.retry_limit:
-                    raise AirflowException(
-                        f"API requests to Fivetran failed {self.retry_limit} times." " Giving up."
-                    )
+class RegistryLink(BaseOperatorLink):
+    """Link to Registry"""
 
-                attempt_num += 1
-                await asyncio.sleep(self.retry_delay)
+    name = "Astronomer Registry"
 
-    async def get_connector_async(self, connector_id):
-        """
-        Fetches the detail of a connector asynchronously.
+    def get_link(self, operator, dttm):
+        """Get link to registry page."""
 
-        :param connector_id: Fivetran connector_id, found in connector settings
-            page in the Fivetran user interface.
-        :type connector_id: str
-        :rtype: Dict
-        """
-        if connector_id == "":
-            raise ValueError("No value specified for connector_id")
-        endpoint = self.api_path_connectors + connector_id
-        resp = await self._do_api_call_async(("GET", endpoint))
-        return resp["data"]
+        registry_link = "https://registry.astronomer.io/providers/{provider}/modules/{operator}"
+        return registry_link.format(provider="fivetran", operator="fivetranoperator")
 
-    async def get_sync_status_async(self, connector_id, previous_completed_at, reschedule_wait_time=0):
-        """
-        For sensor, return True if connector's 'succeeded_at' field has updated.
 
-        :param connector_id: Fivetran connector_id, found in connector settings
-            page in the Fivetran user interface.
-        :type connector_id: str
-        :param previous_completed_at: The last time the connector ran, collected on Sensor
-            initialization.
-        :type previous_completed_at: pendulum.datetime.DateTime
-        :param reschedule_wait_time: Optional, if connector is in reset state,
+class FivetranOperator(BaseOperator):
+    """
+    `FivetranOperator` submits a Fivetran sync job , and polls for its status on the
+    airflow trigger.`FivetranOperator` requires that you specify the `connector_id` of
+    the sync job to start. You can find `connector_id` in the Settings page of the connector
+    you configured in the `Fivetran dashboard <https://fivetran.com/dashboard/connectors>`_.
+    If you do not want to run `FivetranOperator` in async mode you can set `deferrable` to
+    False in operator.
+
+    :param fivetran_conn_id: `Conn ID` of the Connection to be used to configure the hook.
+    :param fivetran_retry_limit: # of retries when encountering API errors
+    :param fivetran_retry_delay: Time to wait before retrying API request
+    :param run_name: Fivetran run name
+    :param timeout_seconds: Timeout in seconds
+    :param connector_id: ID of the Fivetran connector to sync, found on the Connector settings page.
+    :param schedule_type: schedule type. Default is "manual" which takes the connector off Fivetran schedule.
+    :param poll_frequency: Time in seconds that the job should wait in between each try.
+    :param reschedule_wait_time: Optional, if connector is in reset state,
             number of seconds to wait before restarting the sync.
-        :type reschedule_wait_time: int
-        """
-        connector_details = await self.get_connector_async(connector_id)
-        succeeded_at = self._parse_timestamp(connector_details["succeeded_at"])
-        failed_at = self._parse_timestamp(connector_details["failed_at"])
-        current_completed_at = succeeded_at if succeeded_at > failed_at else failed_at
-
-        # The only way to tell if a sync failed is to check if its latest
-        # failed_at value is greater than then last known "sync completed at" value.
-        if failed_at > previous_completed_at:
-            service_name = connector_details["service"]
-            schema_name = connector_details["schema"]
-            raise AirflowException(
-                f"Fivetran sync for connector {connector_id} failed; "
-                f"please see logs at "
-                f"{self._connector_ui_url_logs(service_name, schema_name)}"
-            )
+    :param deferrable: Run operator in deferrable mode. Default is True.
+    """
 
-        sync_state = connector_details["status"]["sync_state"]
-        self.log.info('Connector "%s": sync_state = "%s"', connector_id, sync_state)
+    operator_extra_links = (RegistryLink(),)
 
-        # if sync in rescheduled start, wait for time recommended by Fivetran
-        # or manually specified, then restart sync
-        if sync_state == "rescheduled" and connector_details["schedule_type"] == "manual":
-            self.log.info('Connector is in "rescheduled" state and needs to be manually restarted')
-            self.pause_and_restart(
-                connector_id=connector_id,
-                reschedule_for=connector_details["status"]["rescheduled_for"],
-                reschedule_wait_time=reschedule_wait_time,
-            )
+    template_fields = ["connector_id"]
 
-        # Check if sync started by airflow has finished
-        # indicated by new 'succeeded_at' timestamp
-        if current_completed_at > previous_completed_at:
-            self.log.info(
-                'Connector "%s": succeeded_at = "%s"', connector_id, succeeded_at.to_iso8601_string()
-            )
-            job_status = "success"
-            return job_status
-        else:
-            job_status = "pending"
-            return job_status
+    def __init__(
+        self,
+        connector_id: str,
+        run_name: Optional[str] = None,
+        timeout_seconds: Optional[int] = None,
+        fivetran_conn_id: str = "fivetran",
+        fivetran_retry_limit: int = 3,
+        fivetran_retry_delay: int = 1,
+        poll_frequency: int = 15,
+        schedule_type: str = "manual",
+        reschedule_wait_time: int = 0,
+        deferrable: bool = True,
+        **kwargs,
+    ):
+        self.connector_id = connector_id
+        self.fivetran_conn_id = fivetran_conn_id
+        self.run_name = run_name
+        self.timeout_seconds = timeout_seconds
+        self.fivetran_retry_limit = fivetran_retry_limit
+        self.fivetran_retry_delay = fivetran_retry_delay
+        self.poll_frequency = poll_frequency
+        self.schedule_type = schedule_type
+        self.reschedule_wait_time = reschedule_wait_time
+        self.deferrable = deferrable
+        super().__init__(**kwargs)
+
+    def execute(self, context: Context) -> None | str:
+        """Start the sync using synchronous hook"""
+        hook = self._get_hook()
+        hook.prep_connector(self.connector_id, self.schedule_type)
+        last_sync = hook.start_fivetran_sync(self.connector_id)
 
-    def pause_and_restart(self, connector_id, reschedule_for, reschedule_wait_time):
-        """
-        While a connector is syncing, if it falls into a reschedule state,
-        wait for a time either specified by the user of recommended by Fivetran,
-        Then restart a sync
-
-        :param connector_id: Fivetran connector_id, found in connector settings
-            page in the Fivetran user interface.
-        :type connector_id: str
-        :param reschedule_for: From Fivetran API response, if schedule_type is manual,
-            then the connector expects triggering the event at the designated UTC time.
-        :type reschedule_for: str
-        :param reschedule_wait_time: Optional, if connector is in reset state,
-            number of seconds to wait before restarting the sync.
-        :type reschedule_wait_time: int
-        """
-        if reschedule_wait_time:
-            log_statement = f'Starting connector again in "{reschedule_wait_time}" seconds'
-            self.log.info(log_statement)
-            time.sleep(reschedule_wait_time)
+        if not self.deferrable:
+            return last_sync
         else:
-            wait_time = (
-                self._parse_timestamp(reschedule_for).add(minutes=1) - pendulum.now(tz="UTC")
-            ).seconds
-            if wait_time < 0:
-                raise ValueError(
-                    f"Reschedule time {wait_time} configured in "
-                    f"Fivetran connector has elapsed. Sync connector manually."
+            previous_completed_at = hook.get_last_sync(self.connector_id)
+            completed = hook.get_sync_status(self.connector_id, previous_completed_at)
+            if not completed:
+                self.defer(
+                    timeout=self.execution_timeout,
+                    trigger=FivetranTrigger(
+                        task_id=self.task_id,
+                        fivetran_conn_id=self.fivetran_conn_id,
+                        connector_id=self.connector_id,
+                        poke_interval=self.poll_frequency,
+                        reschedule_wait_time=self.reschedule_wait_time,
+                    ),
+                    method_name="execute_complete",
                 )
-            log_statement = f'Starting connector again in "{wait_time}" seconds'
-            self.log.info(log_statement)
-            time.sleep(wait_time)
 
-        self.log.info("Restarting connector now")
-        return self.start_fivetran_sync(connector_id)
+    def _get_hook(self) -> FivetranHook:
+        return FivetranHook(
+            self.fivetran_conn_id,
+            retry_limit=self.fivetran_retry_limit,
+            retry_delay=self.fivetran_retry_delay,
+        )
+
+    def execute_complete(self, context: Context, event: Optional[Dict[Any, Any]] = None) -> None:
+        """
+        Callback for when the trigger fires - returns immediately.
+        Relies on trigger to throw an exception, otherwise it assumes execution was
+        successful.
+        """
+        if event:
+            if "status" in event and event["status"] == "error":
+                msg = "{0}: {1}".format(event["status"], event["message"])
+                raise AirflowException(msg)
+            if "status" in event and event["status"] == "success":
+                self.log.info(
+                    event["message"],
+                )
+                return event["return_value"]
 
-    def _parse_timestamp(self, api_time):
+    def get_openlineage_facets_on_start(self):
         """
-        Returns either the pendulum-parsed actual timestamp or a very out-of-date timestamp if not set.
-
-        :param api_time: timestamp format as returned by the Fivetran API.
-        :type api_time: str
-        :rtype: Pendulum.DateTime
+        Default extractor method that OpenLineage will call on execute completion.
         """
-        return pendulum.parse(api_time) if api_time is not None else pendulum.from_timestamp(-1)
+        from fivetran_provider_async import (
+            DocumentationJobFacet,
+            ErrorMessageRunFacet,
+            OperatorLineage,
+            OwnershipJobFacet,
+            OwnershipJobFacetOwners,
+        )
+
+        # Should likely use the sync hook here to ensure that OpenLineage data is
+        # returned before the timeout.
+        hook = self._get_hook()
+        connector_response = hook.get_connector(self.connector_id)
+        groups_response = hook.get_groups(connector_response["group_id"])
+        destinations_response = hook.get_destinations(connector_response["group_id"])
+        schema_response = hook.get_connector_schemas(self.connector_id)
+        table_response = hook.get_metadata(self.connector_id, "tables")
+        column_response = hook.get_metadata(self.connector_id, "columns")
+
+        for schema in schema_response["schemas"].values():
+            inputs = datasets(
+                config=connector_response["config"],
+                service=connector_response["service"],
+                table_response=table_response,
+                column_response=column_response,
+                schema=schema,
+                connector_id=self.connector_id,
+                loc="source",
+            )
 
-    async def get_last_sync_async(self, connector_id, xcom=""):
-        """
-        Get the last time Fivetran connector completed a sync.
-        Used with FivetranSensorAsync to monitor sync completion status.
+            outputs = datasets(
+                config=destinations_response["config"],
+                service=destinations_response["service"],
+                table_response=table_response,
+                column_response=column_response,
+                schema=schema,
+                connector_id=self.connector_id,
+                loc="destination",
+            )
 
-        :param connector_id: Fivetran connector_id, found in connector settings
-            page in the Fivetran user interface.
-        :type connector_id: str
-        :param xcom: Timestamp as string pull from FivetranOperator via XCOM
-        :type xcom: str
-        :return: Timestamp of last completed sync
-        :rtype: Pendulum.DateTime
-        """
-        if xcom:
-            last_sync = self._parse_timestamp(xcom)
+        job_facets = {
+            "documentation": DocumentationJobFacet(
+                description=f"""
+                Fivetran run for service: {connector_response['service']}\n
+                Group Name: {groups_response["name"]}\n
+                Connector ID: {self.connector_id}
+                """
+            ),
+            "ownership": OwnershipJobFacet(
+                owners=[OwnershipJobFacetOwners(name=self.owner, type=self.email)]
+            ),
+        }
+
+        run_facets = {}
+        if connector_response.get("failed_at"):
+            run_facets["errorMessage"] = ErrorMessageRunFacet(
+                message=f"Job failed at: {connector_response['failed_at']}",
+                programmingLanguage="Fivetran",
+            )
 
-        else:
-            connector_details = await self.get_connector_async(connector_id)
-            succeeded_at = self._parse_timestamp(connector_details["succeeded_at"])
-            failed_at = self._parse_timestamp(connector_details["failed_at"])
-            last_sync = succeeded_at if succeeded_at > failed_at else failed_at
-        return last_sync
+        return OperatorLineage(inputs=inputs, outputs=outputs, job_facets=job_facets, run_facets=run_facets)
+
+    def get_openlineage_facets_on_complete(self, task_instance):
+        return self.get_openlineage_facets_on_start()
 
 
-def _retryable_error_async(exception: ClientResponseError) -> bool:
-    return exception.status >= 500
+class FivetranOperatorAsync(FivetranOperator):
+    """This operator has been deprecated. Please use `FivetranOperator`."""
+
+    def __init__(self, *args, **kwargs):
+        import warnings
+
+        super().__init__(*args, **kwargs)
+
+        warnings.warn(
+            "FivetranOperatorAsync has been deprecated. Please use `FivetranOperator`.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
```

### Comparing `airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/sensors.py` & `airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/sensors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,133 @@
-from typing import Any, Dict, Optional
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any
 
 from airflow.exceptions import AirflowException
-from airflow.utils.context import Context
-from airflow.utils.decorators import apply_defaults
-from fivetran_provider.sensors.fivetran import FivetranSensor
+from airflow.sensors.base import BaseSensorOperator
+
+if TYPE_CHECKING:
+    from airflow.utils.context import Context
 
+from fivetran_provider_async.hooks import FivetranHook
 from fivetran_provider_async.triggers import FivetranTrigger
 
 
-class FivetranSensorAsync(FivetranSensor):
+class FivetranSensor(BaseSensorOperator):
     """
-    `FivetranSensorAsync` asynchronously monitors a Fivetran sync job for completion.
-    Monitoring with `FivetranSensorAsync` allows you to trigger downstream processes only
+    `FivetranSensor` asynchronously monitors a Fivetran sync job for completion.
+    Monitoring with `FivetranSensor` allows you to trigger downstream processes only
     when the Fivetran sync jobs have completed, ensuring data consistency. You can
-    use multiple instances of `FivetranSensorAsync` to monitor multiple Fivetran
-    connectors. `FivetranSensorAsync` requires that you specify the `connector_id` of the sync
+    use multiple instances of `FivetranSensor` to monitor multiple Fivetran
+    connectors. `FivetranSensor` requires that you specify the `connector_id` of the sync
     job to start. You can find `connector_id` in the Settings page of the connector you configured in the
     `Fivetran dashboard <https://fivetran.com/dashboard/connectors>`_.
+    If you do not want to run `FivetranSensor` in async mode you can set `deferrable` to
+    False in sensor.
 
 
     :param fivetran_conn_id: `Conn ID` of the Connection to be used to configure
         the hook.
     :param connector_id: ID of the Fivetran connector to sync, found on the
         Connector settings page in the Fivetran Dashboard.
     :param poke_interval: Time in seconds that the job should wait in
         between each tries
     :param fivetran_retry_limit: # of retries when encountering API errors
     :param fivetran_retry_delay: Time to wait before retrying API request
     :param reschedule_wait_time: Optional, if connector is in reset state
             number of seconds to wait before restarting, else Fivetran suggestion used
+    :param deferrable: Run sensor in deferrable mode. default is True.
     """
 
-    @apply_defaults
+    template_fields = ["connector_id", "xcom"]
+
     def __init__(
         self,
         connector_id: str,
         fivetran_conn_id: str = "fivetran",
         poke_interval: int = 60,
         fivetran_retry_limit: int = 3,
         fivetran_retry_delay: int = 1,
         xcom: str = "",
         reschedule_wait_time: int = 0,
+        reschedule_time: int = 0,
+        deferrable: bool = True,
         **kwargs: Any,
     ) -> None:
         self.fivetran_conn_id = fivetran_conn_id
         self.connector_id = connector_id
         self.poke_interval = poke_interval
         self.previous_completed_at = None
         self.fivetran_retry_limit = fivetran_retry_limit
         self.fivetran_retry_delay = fivetran_retry_delay
         self.hook = None
         self.xcom = xcom
         self.reschedule_wait_time = reschedule_wait_time
-        super().__init__(
-            connector_id=self.connector_id,
-            fivetran_conn_id=self.fivetran_conn_id,
-            poke_interval=self.poke_interval,
-            fivetran_retry_limit=self.fivetran_retry_limit,
-            fivetran_retry_delay=self.fivetran_retry_delay,
-            xcom=self.xcom,
-            **kwargs,
-        )
+        self.reschedule_time = reschedule_time
+        self.deferrable = deferrable
+        super().__init__(**kwargs)
 
-    def execute(self, context: Dict[str, Any]) -> None:
+    def execute(self, context: Context) -> None:
         """Check for the target_status and defers using the trigger"""
-        self.defer(
-            timeout=self.execution_timeout,
-            trigger=FivetranTrigger(
-                task_id=self.task_id,
-                fivetran_conn_id=self.fivetran_conn_id,
-                connector_id=self.connector_id,
-                previous_completed_at=self.previous_completed_at,
-                xcom=self.xcom,
-                poke_interval=self.poke_interval,
-                reschedule_wait_time=self.reschedule_wait_time,
-            ),
-            method_name="execute_complete",
-        )
+        if not self.deferrable:
+            super().execute(context=context)
+        elif not self.poke(context):
+            self.defer(
+                timeout=self.execution_timeout,
+                trigger=FivetranTrigger(
+                    task_id=self.task_id,
+                    fivetran_conn_id=self.fivetran_conn_id,
+                    connector_id=self.connector_id,
+                    previous_completed_at=self.previous_completed_at,
+                    xcom=self.xcom,
+                    poke_interval=self.poke_interval,
+                    reschedule_wait_time=self.reschedule_wait_time,
+                ),
+                method_name="execute_complete",
+            )
+
+    def _get_hook(self) -> FivetranHook:
+        if self.hook is None:
+            self.hook = FivetranHook(
+                self.fivetran_conn_id,
+                retry_limit=self.fivetran_retry_limit,
+                retry_delay=self.fivetran_retry_delay,
+            )
+        return self.hook
+
+    def poke(self, context):
+        hook = self._get_hook()
+        if self.previous_completed_at is None:
+            self.previous_completed_at = hook.get_last_sync(self.connector_id, self.xcom)
+        return hook.get_sync_status(self.connector_id, self.previous_completed_at, self.reschedule_time)
 
-    def execute_complete(self, context: "Context", event: Optional[Dict[Any, Any]] = None) -> None:
+    def execute_complete(self, context: Context, event: dict[Any, Any] | None = None) -> None:
         """
         Callback for when the trigger fires - returns immediately.
         Relies on trigger to throw an exception, otherwise it assumes execution was
         successful.
         """
         if event:
             if "status" in event and event["status"] == "error":
                 msg = "{0}: {1}".format(event["status"], event["message"])
                 raise AirflowException(msg)
             if "status" in event and event["status"] == "success":
                 self.log.info(
                     event["message"],
                 )
+
+
+class FivetranSensorAsync(FivetranSensor):
+    """This sensor has been deprecated. Please use `FivetranSensor`."""
+
+    template_fields = ["connector_id", "xcom"]
+
+    def __init__(self, *args, **kwargs: Any) -> None:
+        import warnings
+
+        super().__init__(*args, **kwargs)
+
+        warnings.warn(
+            "FivetranSensorAsync has been deprecated. Please use `FivetranSensor`.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
```

### Comparing `airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/triggers.py` & `airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/triggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class FivetranTrigger(BaseTrigger):
     """
     FivetranTrigger is fired as deferred class with params to run the task in trigger worker
 
     :param task_id: Reference to task id of the Dag
     :param connector_id: Reference to the Fivetran connector id being used
-    :param fiventran_conn_id: Reference to Fivetran connection id
+    :param fivetran_conn_id: Reference to Fivetran connection id
     :param previous_completed_at: The last time the connector ran, collected on Sensor
         initialization.
     :param xcom: If used, FivetranSensorAsync receives timestamp of previously
         completed sync
     :param poke_interval:  polling period in seconds to check for the status
     :param reschedule_wait_time: Optional, if connector is in reset state,
             number of seconds to wait before restarting the sync.
```

### Comparing `airflow-provider-fivetran-async-1.1.0/fivetran_provider_async/utils/operator_utils.py` & `airflow-provider-fivetran-async-1.1.1/fivetran_provider_async/utils/operator_utils.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-fivetran-async-1.1.0/setup.cfg` & `airflow-provider-fivetran-async-1.1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 	Framework :: Apache Airflow :: Provider
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 project_urls = 
 	Source Code=https://github.com/astronomer/airflow-provider-fivetran-async
 	Changelog=https://github.com/astronomer/airflow-provider-fivetran-async/blob/main/CHANGELOG.md
 	Bug Tracker = https://github.com/astronomer/airflow-provider-fivetran-async/issues
 
 [options]
 python_requires = >=3.8
 packages = find_namespace:
 include_package_data = true
 install_requires = 
 	apache-airflow>=2.2.0
 	aiohttp
 	asgiref
-	airflow-provider-fivetran
+	requests
 
 [options.extras_require]
 tests = 
 	parameterized
 	pytest
 	pytest-asyncio
 	pytest-cov
```

### Comparing `airflow-provider-fivetran-async-1.1.0/tests/common/static.py` & `airflow-provider-fivetran-async-1.1.1/tests/common/static.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-fivetran-async-1.1.0/tests/operators/test_fivetran.py` & `airflow-provider-fivetran-async-1.1.1/tests/operators/test_fivetran.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,62 @@
+import logging
 import unittest
 from unittest import mock
 
 import pytest
 import requests_mock
 from airflow.exceptions import AirflowException, TaskDeferred
 
-from fivetran_provider_async.operators import FivetranOperatorAsync
+from fivetran_provider_async.operators import FivetranOperator
 from tests.common.static import (
     MOCK_FIVETRAN_DESTINATIONS_RESPONSE_PAYLOAD_SHEETS,
     MOCK_FIVETRAN_GROUPS_RESPONSE_PAYLOAD_SHEETS,
     MOCK_FIVETRAN_METADATA_COLUMNS_RESPONSE_PAYLOAD_SHEETS,
     MOCK_FIVETRAN_METADATA_TABLES_RESPONSE_PAYLOAD_SHEETS,
     MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS,
     MOCK_FIVETRAN_SCHEMA_RESPONSE_PAYLOAD_SHEETS,
 )
 
+log = logging.getLogger(__name__)
+
+
+MOCK_FIVETRAN_RESPONSE_PAYLOAD = {
+    "code": "Success",
+    "data": {
+        "id": "interchangeable_revenge",
+        "group_id": "rarer_gradient",
+        "service": "google_sheets",
+        "service_version": 1,
+        "schema": "google_sheets.fivetran_google_sheets_spotify",
+        "connected_by": "mournful_shalt",
+        "created_at": "2021-03-05T22:58:56.238875Z",
+        "succeeded_at": "2021-03-23T20:55:12.670390Z",
+        "failed_at": "null",
+        "paused": False,
+        "sync_frequency": 360,
+        "schedule_type": "manual",
+        "status": {
+            "setup_state": "connected",
+            "sync_state": "scheduled",
+            "update_state": "on_schedule",
+            "is_historical_sync": False,
+            "tasks": [],
+            "warnings": [],
+        },
+        "config": {
+            "latest_version": "1",
+            "sheet_id": "https://docs.google.com/spreadsheets/d/.../edit#gid=...",
+            "named_range": "fivetran_test_range",
+            "authorization_method": "User OAuth",
+            "service_version": "1",
+            "last_synced_changes__utc_": "2021-03-23 20:54",
+        },
+    },
+}
+
 
 @pytest.fixture
 def context():
     """
     Creates an empty context.
     """
     context = {}
@@ -36,15 +74,15 @@
         )
 
         m.post(
             "https://api.fivetran.com/v1/connectors/interchangeable_revenge/force",
             json=MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS,
         )
 
-        task = FivetranOperatorAsync(
+        task = FivetranOperator(
             task_id="fivetran_op_async",
             fivetran_conn_id="conn_fivetran",
             connector_id="interchangeable_revenge",
         )
         with pytest.raises(TaskDeferred):
             task.execute(context)
 
@@ -57,39 +95,39 @@
         )
 
         m.post(
             "https://api.fivetran.com/v1/connectors/interchangeable_revenge/force",
             json=MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS,
         )
 
-        task = FivetranOperatorAsync(
+        task = FivetranOperator(
             task_id="fivetran_op_async",
             fivetran_conn_id="conn_fivetran",
             connector_id="interchangeable_revenge",
             reschedule_wait_time=60,
             schedule_type="manual",
         )
         with pytest.raises(TaskDeferred):
             task.execute(context)
 
     def test_fivetran_op_async_execute_complete_error(self):
         """Tests that execute_complete method raises exception in case of error"""
-        task = FivetranOperatorAsync(
+        task = FivetranOperator(
             task_id="fivetran_op_async",
             fivetran_conn_id="conn_fivetran",
             connector_id="interchangeable_revenge",
         )
         with pytest.raises(AirflowException) as exc_info:
             task.execute_complete(context=None, event={"status": "error", "message": "test failure message"})
 
         assert str(exc_info.value) == "error: test failure message"
 
     def test_fivetran_op_async_execute_complete_success(self):
         """Tests that execute_complete method returns expected result and that it prints expected log"""
-        task = FivetranOperatorAsync(
+        task = FivetranOperator(
             task_id="fivetran_op_async",
             fivetran_conn_id="conn_fivetran",
             connector_id="interchangeable_revenge",
         )
         expected_return_value = MOCK_FIVETRAN_RESPONSE_PAYLOAD_SHEETS["data"]["succeeded_at"]
 
         with mock.patch.object(task.log, "info") as mock_log_info:
@@ -130,15 +168,15 @@
             json=MOCK_FIVETRAN_DESTINATIONS_RESPONSE_PAYLOAD_SHEETS,
         )
         m.get(
             "https://api.fivetran.com/v1/groups/rarer_gradient",
             json=MOCK_FIVETRAN_GROUPS_RESPONSE_PAYLOAD_SHEETS,
         )
 
-        operator = FivetranOperatorAsync(
+        operator = FivetranOperator(
             task_id="fivetran-task",
             fivetran_conn_id="conn_fivetran",
             connector_id="interchangeable_revenge",
         )
 
         facets = operator.get_openlineage_facets_on_start()
         assert facets.inputs[0].namespace == "sheets://"
```

### Comparing `airflow-provider-fivetran-async-1.1.0/tests/triggers/test_fivetran.py` & `airflow-provider-fivetran-async-1.1.1/tests/triggers/test_fivetran.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-fivetran-async-1.1.0/tests/utils/test_operator_utils.py` & `airflow-provider-fivetran-async-1.1.1/tests/utils/test_operator_utils.py`

 * *Files identical despite different names*

