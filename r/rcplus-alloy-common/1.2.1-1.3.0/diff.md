# Comparing `tmp/rcplus_alloy_common-1.2.1.tar.gz` & `tmp/rcplus_alloy_common-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcplus_alloy_common-1.2.1.tar", max compression
+gzip compressed data, was "rcplus_alloy_common-1.3.0.tar", max compression
```

## Comparing `rcplus_alloy_common-1.2.1.tar` & `rcplus_alloy_common-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       77 2023-07-13 09:20:28.905190 rcplus_alloy_common-1.2.1/LICENSE
--rw-r--r--   0        0        0      571 2023-07-13 09:20:28.905190 rcplus_alloy_common-1.2.1/README.md
--rw-r--r--   0        0        0     1951 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2881 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/__init__.py
--rw-r--r--   0        0        0      567 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/__init__.py
--rw-r--r--   0        0        0     1179 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/dag.py
--rw-r--r--   0        0        0     1681 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/decorators.py
--rw-r--r--   0        0        0      703 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/hooks.py
--rw-r--r--   0        0        0     7448 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/observability.py
--rw-r--r--   0        0        0    20030 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/operators.py
--rw-r--r--   0        0        0     2611 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/sensors.py
--rw-r--r--   0        0        0     2799 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/utils.py
--rw-r--r--   0        0        0     2279 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/constants.py
--rw-r--r--   0        0        0     3866 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/logging.py
--rw-r--r--   0        0        0     6388 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/metrics.py
--rw-r--r--   0        0        0     3925 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/retry.py
--rw-r--r--   0        0        0       19 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/version.py
--rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 rcplus_alloy_common-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       77 2023-08-03 14:33:59.595970 rcplus_alloy_common-1.3.0/LICENSE
+-rw-r--r--   0        0        0      571 2023-08-03 14:33:59.595970 rcplus_alloy_common-1.3.0/README.md
+-rw-r--r--   0        0        0     1951 2023-08-03 14:33:59.599970 rcplus_alloy_common-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2881 2023-08-03 14:33:59.599970 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/__init__.py
+-rw-r--r--   0        0        0      567 2023-08-03 14:33:59.599970 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/__init__.py
+-rw-r--r--   0        0        0     1179 2023-08-03 14:33:59.599970 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/dag.py
+-rw-r--r--   0        0        0     1681 2023-08-03 14:33:59.599970 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/decorators.py
+-rw-r--r--   0        0        0      703 2023-08-03 14:33:59.599970 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/hooks.py
+-rw-r--r--   0        0        0     7448 2023-08-03 14:33:59.603971 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/observability.py
+-rw-r--r--   0        0        0    20030 2023-08-03 14:33:59.603971 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/operators.py
+-rw-r--r--   0        0        0     2611 2023-08-03 14:33:59.603971 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/sensors.py
+-rw-r--r--   0        0        0     2799 2023-08-03 14:33:59.603971 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/utils.py
+-rw-r--r--   0        0        0     2279 2023-08-03 14:33:59.603971 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/constants.py
+-rw-r--r--   0        0        0     4578 2023-08-03 14:33:59.603971 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/logging.py
+-rw-r--r--   0        0        0     6388 2023-08-03 14:33:59.603971 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/metrics.py
+-rw-r--r--   0        0        0     3925 2023-08-03 14:33:59.603971 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/retry.py
+-rw-r--r--   0        0        0       19 2023-08-03 14:33:59.603971 rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/version.py
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 rcplus_alloy_common-1.3.0/PKG-INFO
```

### Comparing `rcplus_alloy_common-1.2.1/README.md` & `rcplus_alloy_common-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v1.2.1**
+Current version: **v1.3.0**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

### Comparing `rcplus_alloy_common-1.2.1/pyproject.toml` & `rcplus_alloy_common-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "rcplus_alloy_common"
-version = "1.2.1"
+version = "1.3.0"
 description = "RC+/Alloy helpers functions for Python"
 readme = "README.md"
 authors = [
     "Ringier AG <info@rcplus.io>",
 ]
 license = "Proprietary"
 repository = "https://github.com/ringier-data/rcplus-alloy-lib-py-common"
```

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/__init__.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/__init__.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/dag.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/decorators.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/decorators.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/hooks.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/hooks.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/observability.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/observability.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/operators.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/operators.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/sensors.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/sensors.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/utils.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/airflow/utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/constants.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/constants.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/logging.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/logging.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,29 @@
     def process_log_record(self, log_record):
         dag_id = os.getenv("DAG_ID")
         if dag_id is not None:
             log_record["dag_id"] = dag_id
         dag_run_id = os.getenv("DAG_RUN_ID")
         if dag_run_id is not None:
             log_record["dag_run_id"] = dag_run_id
+        aws_lambda_function_name = os.getenv("AWS_LAMBDA_FUNCTION_NAME")
+        if aws_lambda_function_name is not None:
+            log_record["origin"] = f"lambda/{aws_lambda_function_name}"
+        env = os.getenv("ENVIRONMENT")
+        if env is not None:
+            log_record["env"] = env
+        version = os.getenv("VERSION")
+        if version is not None:
+            log_record["version"] = version
+        repository = os.getenv("REPOSITORY")
+        if repository is not None:
+            log_record["repository"] = repository
+        software_component = os.getenv("SOFTWARE_COMPONENT")
+        if software_component is not None:
+            log_record["software_component"] = software_component
         return super().process_log_record(log_record)
 
 
 class CustomLoggingFormatter(logging.Formatter):
     def formatTime(self, record, datefmt=None):
         return f"{datetime.fromtimestamp(record.created, tz=timezone.utc).strftime(LOGGING_DATETIME_FORMAT)[:-3]}Z"
```

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/metrics.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/metrics.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/retry.py` & `rcplus_alloy_common-1.3.0/src/rcplus_alloy_common/retry.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.1/PKG-INFO` & `rcplus_alloy_common-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcplus-alloy-common
-Version: 1.2.1
+Version: 1.3.0
 Summary: RC+/Alloy helpers functions for Python
 Home-page: https://github.com/ringier-data/rcplus-alloy-lib-py-common
 License: Proprietary
 Keywords: rcplus,alloy,logging,metrics,utilities
 Author: Ringier AG
 Author-email: info@rcplus.io
 Requires-Python: >=3.10,<4
@@ -29,15 +29,15 @@
 
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v1.2.1**
+Current version: **v1.3.0**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

