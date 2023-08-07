# Comparing `tmp/airflow_mcd-0.2.1.tar.gz` & `tmp/airflow_mcd-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow_mcd-0.2.1.tar", last modified: Thu Jul 27 15:00:59 2023, max compression
+gzip compressed data, was "dist/airflow_mcd-0.2.2.tar", last modified: Mon Aug  7 15:42:44 2023, max compression
```

## Comparing `airflow_mcd-0.2.1.tar` & `airflow_mcd-0.2.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.676613 airflow_mcd-0.2.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/.circleci/
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/.circleci/README
--rw-r--r--   0 root         (0) root         (0)     3102 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/.circleci/config.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/.circleci/trufflehog_config/
--rw-r--r--   0 root         (0) root         (0)      377 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/.circleci/trufflehog_config/allowlist.json
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1818 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1184 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/Makefile
--rw-r--r--   0 root         (0) root         (0)     9590 2023-07-27 15:00:59.676613 airflow_mcd-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2000 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/README-dev.md
--rw-r--r--   0 root         (0) root         (0)     8777 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/airflow_mcd/
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/airflow_mcd/callbacks/
--rw-r--r--   0 root         (0) root         (0)     7042 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/callbacks/client.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/callbacks/mcd_callbacks.py
--rw-r--r--   0 root         (0) root         (0)     6336 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/airflow_mcd/hooks/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4492 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/hooks/session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/airflow_mcd/operators/
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/operators/base_operator.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/operators/circuit_breaker_operators.py
--rw-r--r--   0 root         (0) root         (0)    15407 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/airflow_mcd/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/airflow_mcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9590 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1175 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-27 15:00:59.000000 airflow_mcd-0.2.1/airflow_mcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/examples/
--rw-r--r--   0 root         (0) root         (0)     2050 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/examples/sample_circuit_dag.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/requirements-ci.txt
--rw-r--r--   0 root         (0) root         (0)      195 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-27 15:00:59.676613 airflow_mcd-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1579 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/tests/callbacks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15028 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/callbacks/test_callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.672613 airflow_mcd-0.2.1/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/hooks/test_session_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:00:59.676613 airflow_mcd-0.2.1/tests/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/test_base_op.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/test_circuit_breaker_op.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/test_dbt_cli_config.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/test_dbt_default_config_provider.py
--rw-r--r--   0 root         (0) root         (0)    21136 2023-07-27 15:00:02.000000 airflow_mcd-0.2.1/tests/operators/test_dbt_operator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.779525 airflow_mcd-0.2.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.775525 airflow_mcd-0.2.2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/.circleci/README
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/.circleci/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.775525 airflow_mcd-0.2.2/.circleci/trufflehog_config/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/.circleci/trufflehog_config/allowlist.json
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9590 2023-08-07 15:42:44.779525 airflow_mcd-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/README-dev.md
+-rw-r--r--   0 root         (0) root         (0)     8777 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.775525 airflow_mcd-0.2.2/airflow_mcd/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/airflow_mcd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.779525 airflow_mcd-0.2.2/airflow_mcd/callbacks/
+-rw-r--r--   0 root         (0) root         (0)     7042 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/airflow_mcd/callbacks/client.py
+-rw-r--r--   0 root         (0) root         (0)     5963 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/airflow_mcd/callbacks/mcd_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     7338 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/airflow_mcd/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.779525 airflow_mcd-0.2.2/airflow_mcd/hooks/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/airflow_mcd/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4492 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/airflow_mcd/hooks/session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.779525 airflow_mcd-0.2.2/airflow_mcd/operators/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/airflow_mcd/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/airflow_mcd/operators/base_operator.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/airflow_mcd/operators/circuit_breaker_operators.py
+-rw-r--r--   0 root         (0) root         (0)    15407 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/airflow_mcd/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.775525 airflow_mcd-0.2.2/airflow_mcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9590 2023-08-07 15:42:44.000000 airflow_mcd-0.2.2/airflow_mcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-08-07 15:42:44.000000 airflow_mcd-0.2.2/airflow_mcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 15:42:44.000000 airflow_mcd-0.2.2/airflow_mcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-07 15:42:44.000000 airflow_mcd-0.2.2/airflow_mcd.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 15:42:44.000000 airflow_mcd-0.2.2/airflow_mcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-08-07 15:42:44.000000 airflow_mcd-0.2.2/airflow_mcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.779525 airflow_mcd-0.2.2/examples/
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/examples/sample_circuit_dag.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-08-07 15:42:44.779525 airflow_mcd-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.779525 airflow_mcd-0.2.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.779525 airflow_mcd-0.2.2/tests/callbacks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/tests/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16234 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/tests/callbacks/test_callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.779525 airflow_mcd-0.2.2/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/tests/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/tests/hooks/test_session_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 15:42:44.779525 airflow_mcd-0.2.2/tests/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/tests/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/tests/operators/test_base_op.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/tests/operators/test_circuit_breaker_op.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/tests/operators/test_dbt_cli_config.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/tests/operators/test_dbt_default_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)    21136 2023-08-07 15:41:41.000000 airflow_mcd-0.2.2/tests/operators/test_dbt_operator.py
```

### Comparing `airflow_mcd-0.2.1/.circleci/config.yml` & `airflow_mcd-0.2.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/.gitignore` & `airflow_mcd-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/LICENSE` & `airflow_mcd-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/Makefile` & `airflow_mcd-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/PKG-INFO` & `airflow_mcd-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_mcd
-Version: 0.2.1
+Version: 0.2.2
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.2.1/README-dev.md` & `airflow_mcd-0.2.2/README-dev.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/README.md` & `airflow_mcd-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/airflow_mcd/callbacks/client.py` & `airflow_mcd-0.2.2/airflow_mcd/callbacks/client.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/airflow_mcd/callbacks/mcd_callbacks.py` & `airflow_mcd-0.2.2/airflow_mcd/callbacks/mcd_callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,80 +67,80 @@
     """
     Callback function that sends the DAG success event to Monte Carlo, it must be configured as
     `on_success_callback` in a DAG object.
     You can also manually invoke this function from your own callback code passing the same context you received.
     :param context: The Airflow DAG success context.
     """
     try:
-        AirflowEventsClientUtils.mcd_post_dag_result(success=True, context=context)
+        AirflowEventsClientUtils.mcd_post_dag_result(context)
     except Exception as ex:
         logger.exception(f'Failed to post dag result to MCD: {ex}')
 
 
 def mcd_dag_failure_callback(context: Dict):
     """
     Callback function that sends the DAG failure event to Monte Carlo, it must be configured as
     `on_failure_callback` in a DAG object.
     You can also manually invoke this function from your own callback code passing the same context you received.
     :param context: The Airflow DAG failure context.
     """
     try:
-        AirflowEventsClientUtils.mcd_post_dag_result(success=False, context=context)
+        AirflowEventsClientUtils.mcd_post_dag_result(context)
     except Exception as ex:
         logger.exception(f'Failed to post dag failure result to MCD: {ex}')
 
 
 def mcd_task_success_callback(context: Dict):
     """
     Callback function that sends the Task success event to Monte Carlo, it must be configured as
     `on_success_callback` in a Task object.
     You can also manually invoke this function from your own callback code passing the same context you received.
     :param context: The Airflow Task success context.
     """
     try:
-        AirflowEventsClientUtils.mcd_post_task_result(success=True, context=context)
+        AirflowEventsClientUtils.mcd_post_task_result(context)
     except Exception as ex:
         logger.exception(f'Failed to post task result to MCD: {ex}')
 
 
 def mcd_task_execute_callback(context: Dict):
     """
     Callback function that sends the Task execution event to Monte Carlo, it must be configured as
     `on_execute_callback` in a Task object.
     You can also manually invoke this function from your own callback code passing the same context you received.
     :param context: The Airflow Task execution context.
     """
     try:
-        AirflowEventsClientUtils.mcd_post_task_result(success=True, context=context)
+        AirflowEventsClientUtils.mcd_post_task_result(context)
     except Exception as ex:
         logger.exception(f'Failed to post task result to MCD: {ex}')
 
 
 def mcd_task_failure_callback(context: Dict):
     """
     Callback function that sends the Task failure event to Monte Carlo, it must be configured as
     `on_failure_callback` in a Task object.
     You can also manually invoke this function from your own callback code passing the same context you received.
     :param context: The Airflow Task failure context.
     """
     try:
-        AirflowEventsClientUtils.mcd_post_task_result(success=False, context=context)
+        AirflowEventsClientUtils.mcd_post_task_result(context)
     except Exception as ex:
         logger.exception(f'Failed to post task failure result to MCD: {ex}')
 
 
 def mcd_task_retry_callback(context: Dict):
     """
     Callback function that sends the Task retry event to Monte Carlo, it must be configured as
     `on_retry_callback` in a Task object.
     You can also manually invoke this function from your own callback code passing the same context you received.
     :param context: The Airflow Task retry context.
     """
     try:
-        AirflowEventsClientUtils.mcd_post_task_result(success=False, context=context)
+        AirflowEventsClientUtils.mcd_post_task_result(context)
     except Exception as ex:
         logger.exception(f'Failed to post task retry result to MCD: {ex}')
 
 
 def mcd_sla_miss_callback(dag, task_list, blocking_task_list, slas, blocking_tis):
     """
     Callback function that sends the SLA misses event to Monte Carlo, it must be configured as
```

### Comparing `airflow_mcd-0.2.1/airflow_mcd/callbacks/utils.py` & `airflow_mcd-0.2.2/airflow_mcd/callbacks/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,90 @@
 import logging
 from copy import deepcopy
 
+from pycarlo.common.utils import truncate_string
 from airflow.models import TaskInstance, SlaMiss, DagRun, DAG
 from attr import asdict
 from datetime import datetime, timezone
 
 from airflow_mcd.callbacks.client import DagResult, DagTaskResult, AirflowEventsClient, DagTaskInstanceResult, \
     SlaMissesResult, TaskSlaMiss
 from typing import Dict, List, Any, Optional
 
 
 logger = logging.getLogger(__name__)
 
 _DEFAULT_CALL_TIMEOUT = 10
+_SUCCESS_STATES = ['success', 'skipped']
+_EXCEPTION_MSG_LIMIT = 10 * 1024  # 10kb
 
 
 class AirflowEventsClientUtils:
     @classmethod
     def mcd_post_dag_result(
             cls,
             context: Dict,
-            success: bool,
     ):
-        if 'dag' not in context or 'run_id' not in context or 'dag_run' not in context:
-            logger.error('Invalid context received in MCD callback: dag, run_id and dag_run are expected')
+        if not cls._validate_dag_callback_context(context=context):
             return
 
         dag: DAG = context['dag']
         dag_run: DagRun = context['dag_run']
         task_instances = dag_run.get_task_instances()
         result = DagResult(
             dag_id=dag.dag_id,
             run_id=context['run_id'],
-            success=success,
-            reason=context.get('reason'),
+            success=dag_run.state in _SUCCESS_STATES,
+            reason=context['reason'],
             tasks=[cls._get_task_instance_result(ti) for ti in task_instances],
             state=dag_run.state,
             execution_date=cls._get_datetime_isoformat(dag_run.execution_date),
             start_date=cls._get_datetime_isoformat(dag_run.start_date),
             end_date=cls._get_datetime_isoformat(dag_run.end_date),
             original_dates=cls._get_original_dates(dag_run.execution_date, dag_run.start_date, dag_run.end_date),
         )
         cls._get_events_client(dag).upload_dag_result(result)
 
+    @staticmethod
+    def _validate_dag_callback_context(context: Dict) -> bool:
+        error_message: Optional[str] = None
+        if 'dag' not in context or 'run_id' not in context or 'dag_run' not in context:
+            error_message = 'dag, run_id and dag_run are expected'
+        else:
+            dag_run: DagRun = context['dag_run']
+            if not dag_run.end_date:
+                error_message = 'no dag_run.end_date set, it looks like the dag is still running'
+            elif 'reason' not in context:
+                error_message = 'no reason set, it looks like the dag is still running'
+
+        if error_message:
+            logger.error(f'Invalid context received in MCD dag callback: {error_message}. '
+                         'Please check your callbacks are configured properly.')
+            return False
+        return True
+
     @classmethod
-    def mcd_post_task_result(cls, success: bool, context: Dict):
+    def mcd_post_task_result(cls, context: Dict):
         if 'dag' not in context or 'run_id' not in context or 'task_instance' not in context:
             logger.error('Invalid context received in MCD task callback: dag, run_id and task_instance are expected')
             return
 
         dag = context['dag']
         ti = context['task_instance']
-        exception_message = str(context['exception']) if 'exception' in context else None
+        exception_message = truncate_string(
+            str(context['exception']),
+            _EXCEPTION_MSG_LIMIT,
+        ) if 'exception' in context else None
+        task_instance_result = cls._get_task_instance_result(ti, exception_message)
+
         result = DagTaskResult(
             dag_id=dag.dag_id,
             run_id=context['run_id'],
-            success=success,
-            task=cls._get_task_instance_result(ti, exception_message),
+            success=task_instance_result.state in _SUCCESS_STATES,
+            task=task_instance_result,
         )
         cls._get_events_client(dag).upload_task_result(result)
 
     @classmethod
     def mcd_post_sla_misses(cls, dag: DAG, sla_misses: List[SlaMiss]):
         result = SlaMissesResult(
             dag_id=dag.dag_id,
```

### Comparing `airflow_mcd-0.2.1/airflow_mcd/hooks/session_hook.py` & `airflow_mcd-0.2.2/airflow_mcd/hooks/session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/airflow_mcd/operators/base_operator.py` & `airflow_mcd-0.2.2/airflow_mcd/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/airflow_mcd/operators/circuit_breaker_operators.py` & `airflow_mcd-0.2.2/airflow_mcd/operators/circuit_breaker_operators.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/airflow_mcd/operators/dbt.py` & `airflow_mcd-0.2.2/airflow_mcd/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/airflow_mcd.egg-info/PKG-INFO` & `airflow_mcd-0.2.2/airflow_mcd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-mcd
-Version: 0.2.1
+Version: 0.2.2
 Summary: Monte Carlo's Apache Airflow Provider
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `airflow_mcd-0.2.1/airflow_mcd.egg-info/SOURCES.txt` & `airflow_mcd-0.2.2/airflow_mcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/examples/sample_circuit_dag.py` & `airflow_mcd-0.2.2/examples/sample_circuit_dag.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/setup.py` & `airflow_mcd-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/tests/callbacks/test_callbacks.py` & `airflow_mcd-0.2.2/tests/callbacks/test_callbacks.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from unittest import TestCase
 from unittest.mock import create_autospec, patch, ANY
 
 from airflow.models import DagRun, TaskInstance, SlaMiss, DAG
 from sgqlc.types import Variable
 
 from airflow_mcd.callbacks.client import AirflowEventsClient, AirflowEnv
-from airflow_mcd.callbacks.utils import AirflowEventsClientUtils
+from airflow_mcd.callbacks.utils import AirflowEventsClientUtils, _EXCEPTION_MSG_LIMIT
 from freezegun import freeze_time
+from pycarlo.common.utils import truncate_string
 
 
 # needed to have a successful assert_called_with as Variable doesn't implement __eq__
 class EqVariable(Variable):
     def __eq__(self, other):
         return other.name == self.name
 
@@ -24,34 +25,48 @@
         self._test_upload_dag_result(True, mock_client_upload_result)
 
     @freeze_time("2023-02-03 10:11:12", tz_offset=0)
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_dag_result_success_no_dates(self,  mock_client_upload_result):
         self._test_upload_dag_result(True, mock_client_upload_result, set_dates=False)
 
+    @freeze_time("2023-02-03 10:11:12", tz_offset=0)
+    @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
+    def test_upload_dag_result_success_no_end_date(self,  mock_client_upload_result):
+        self._test_upload_dag_result(True, mock_client_upload_result, set_dates=True, set_end_date=False)
+
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_dag_result_failure(self, mock_client_upload_result):
         self._test_upload_dag_result(False, mock_client_upload_result)
 
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_task_result_success(self, mock_client_upload_result):
-        self._test_upload_task_result(True, False, mock_client_upload_result)
+        self._test_upload_task_result("success", mock_client_upload_result)
 
     @freeze_time("2023-02-03 10:11:12", tz_offset=0)
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_task_result_success_no_dates(self, mock_client_upload_result):
-        self._test_upload_task_result(True, False, mock_client_upload_result, set_dates=False)
+        self._test_upload_task_result("success", mock_client_upload_result, set_dates=False)
 
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_task_result_failure(self, mock_client_upload_result):
-        self._test_upload_task_result(False, False, mock_client_upload_result)
+        self._test_upload_task_result("failed", mock_client_upload_result)
+
+    @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
+    def test_upload_task_result_failure_long_message(self, mock_client_upload_result):
+        error_message = "error message érror, " * 1024
+        self._test_upload_task_result(
+            state="failed",
+            mock_client_upload_result=mock_client_upload_result,
+            error_message=error_message,
+        )
 
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_task_result_running(self, mock_client_upload_result):
-        self._test_upload_task_result(True, True, mock_client_upload_result)
+        self._test_upload_task_result("running", mock_client_upload_result)
 
     @patch("airflow_mcd.callbacks.client.AirflowEventsClient._upload_result")
     def test_upload_sla_misses(self, mock_client_upload_result):
         utils = AirflowEventsClientUtils()
 
         dag = create_autospec(DAG)
         dag.dag_id = "dag_123"
@@ -154,24 +169,29 @@
         self.assertEqual("url", params_env.base_url)
 
     def _test_upload_dag_result(
             self,
             success: bool,
             mock_client_upload_result,
             set_dates: bool = True,
+            set_end_date: bool = True,
     ):
-        dag_context = self._create_dag_context(success, set_dates=set_dates)
+        state = "success" if success else "failed"
+        dag_context = self._create_dag_context(state, set_dates=set_dates, set_end_date=set_end_date)
         dag: DAG = dag_context["dag"]
         dag_run: DagRun = dag_context["dag_run"]
         task_instances: List[TaskInstance] = dag_run.get_task_instances()
 
         utils = AirflowEventsClientUtils()
-        utils.mcd_post_dag_result(dag_context, success)
+        utils.mcd_post_dag_result(dag_context)
 
         now_isoformat = datetime.now(tz=timezone.utc).isoformat()
+        if not set_end_date:
+            mock_client_upload_result.assert_not_called()
+            return
         mock_client_upload_result.assert_called()
         mock_client_upload_result.assert_called_with(
             AirflowEventsClient._UPLOAD_AIRFLOW_DAG_RESULT_OPERATION,
             {
                 "dag_id": dag.dag_id,
                 "run_id": dag_context["run_id"],
                 "success": success,
@@ -212,104 +232,119 @@
         return {
             "env_name": "airflow",
             "env_id": None,
             "version": None,
             "base_url": None
         }
 
-    def _create_dag_context(self, success: bool, task_running: bool = False, set_dates: bool = True) -> Dict:
+    def _create_dag_context(
+            self,
+            state: str,
+            set_dates: bool = True,
+            set_end_date: bool = True,
+    ) -> Dict:
         dag = create_autospec(DAG)
         dag.dag_id = "dag_123"
         dag.params = {}
         dag_run = create_autospec(DagRun)
         task_instances = [
             self._create_task_instance(
                 dag_id=dag.dag_id,
                 task_id="task_123",
-                state="running" if task_running else "success",
-                running=task_running,
+                state=state,
+                running=state == "running",
                 set_dates=set_dates,
             ),
             self._create_task_instance(
                 dag_id=dag.dag_id,
                 task_id="task_234",
                 state="success",
                 set_dates=set_dates,
             ),
         ]
-        state = "success" if success else "failed"
         dag_run.get_task_instances.return_value = task_instances
         dag_run.state = state
         if set_dates:
             dag_run.execution_date = datetime.now(tz=timezone.utc) - timedelta(seconds=10)
             dag_run.start_date = datetime.now(tz=timezone.utc) - timedelta(seconds=9)
-            dag_run.end_date = datetime.now(tz=timezone.utc)
         else:
             dag_run.execution_date = None
             dag_run.start_date = None
+
+        if set_end_date:
+            dag_run.end_date = datetime.now(tz=timezone.utc)
+        else:
             dag_run.end_date = None
 
         dag_context = {
             "dag": dag,
             "run_id": '123',
             "dag_run": dag_run,
-            "reason": "succeeded" if success else "task failed",
+            "reason": "succeeded" if state == "success" else "task failed",
         }
         return dag_context
 
     def _test_upload_task_result(
-            self,
-            success: bool,
-            task_running: bool,
-            mock_client_upload_result,
-            set_dates: bool = True,
+        self,
+        state: str,
+        mock_client_upload_result,
+        set_dates: bool = True,
+        error_message: Optional[str] = None,
     ):
-        dag_context = self._create_dag_context(success, task_running, set_dates=set_dates)
-        state = "running" if task_running else "success" if success else "failed"
-        exception_message: str = "task failed" if not success else None
-        if not success:
+        dag_context = self._create_dag_context(state, set_dates=set_dates)
+        exception_message: str = (error_message or "task failed") if state == "failed" else None
+        if state == "failed":
             dag_context["exception"] = Exception(exception_message)
         dag: DAG = dag_context["dag"]
         dag_run: DagRun = dag_context["dag_run"]
         task_instances: List[TaskInstance] = dag_run.get_task_instances()
         task_instance = task_instances[0]
         task_instance.state = state
         dag_context["task_instance"] = task_instance
         utils = AirflowEventsClientUtils()
-        utils.mcd_post_task_result(success, dag_context)
+        utils.mcd_post_task_result(dag_context)
 
         now_isoformat = datetime.now(tz=timezone.utc).isoformat()
         expected_graphql_payload = {
             "dag_id": dag.dag_id,
             "run_id": dag_context["run_id"],
             "task_id": task_instance.task_id,
-            "success": success,
+            "success": state == "success",
             "env": self._get_graphql_env(),
             "state": state,
             "log_url": f"http://airflow.com/{dag.dag_id}/{task_instance.task_id}/log",
             "execution_date": task_instance.execution_date.isoformat() if set_dates else now_isoformat,
             'start_date': task_instance.start_date.isoformat() if set_dates else now_isoformat,
             'end_date': task_instance.end_date.isoformat() if set_dates else now_isoformat,
             'duration': task_instance.duration or 0,
             'attempt_number': task_instance.prev_attempted_tries,
             "payload": EqVariable("payload"),
         }
-        if exception_message and not success:
-            expected_graphql_payload["exception_message"] = exception_message
+        expected_exception_message = truncate_string(
+            exception_message,
+            _EXCEPTION_MSG_LIMIT,
+        ) if exception_message else None
+
+        if exception_message:
+            expected_graphql_payload["exception_message"] = expected_exception_message
 
         mock_client_upload_result.assert_called()
         mock_client_upload_result.assert_called_with(
             AirflowEventsClient._UPLOAD_AIRFLOW_TASK_RESULT_OPERATION,
             expected_graphql_payload,
             {
                 "dag_id": dag.dag_id,
                 "env": self._get_env(),
                 "run_id": dag_context["run_id"],
-                "success": success,
-                "task": self._get_dag_task_instance_result(task_instance, exception_message, set_dates=set_dates),
+                "success": state == "success",
+                "task": self._get_dag_task_instance_result(
+                    task_instance,
+                    expected_exception_message,
+                    set_dates=set_dates
+                ),
                 "event_type": "task",
             }
         )
 
     @staticmethod
     def _create_task_instance(
             dag_id: str,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `airflow_mcd-0.2.1/tests/hooks/test_session_hook.py` & `airflow_mcd-0.2.2/tests/hooks/test_session_hook.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/tests/operators/test_base_op.py` & `airflow_mcd-0.2.2/tests/operators/test_base_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/tests/operators/test_circuit_breaker_op.py` & `airflow_mcd-0.2.2/tests/operators/test_circuit_breaker_op.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/tests/operators/test_dbt_cli_config.py` & `airflow_mcd-0.2.2/tests/operators/test_dbt_cli_config.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/tests/operators/test_dbt_default_config_provider.py` & `airflow_mcd-0.2.2/tests/operators/test_dbt_default_config_provider.py`

 * *Files identical despite different names*

### Comparing `airflow_mcd-0.2.1/tests/operators/test_dbt_operator.py` & `airflow_mcd-0.2.2/tests/operators/test_dbt_operator.py`

 * *Files identical despite different names*

