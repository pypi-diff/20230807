# Comparing `tmp/wells-data-pipeline-cores-0.0.3.tar.gz` & `tmp/wells-data-pipeline-cores-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wells-data-pipeline-cores-0.0.3.tar", last modified: Sun Aug  6 05:21:29 2023, max compression
+gzip compressed data, was "wells-data-pipeline-cores-0.0.4.tar", last modified: Mon Aug  7 14:28:09 2023, max compression
```

## Comparing `wells-data-pipeline-cores-0.0.3.tar` & `wells-data-pipeline-cores-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:21:29.587699 wells-data-pipeline-cores-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-06 05:21:29.587699 wells-data-pipeline-cores-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 05:21:29.587699 wells-data-pipeline-cores-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:21:29.583699 wells-data-pipeline-cores-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/test/test_env_vars_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:21:29.583699 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:21:29.583699 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/commons/dev_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19055 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/commons/env_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/commons/key_vaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:21:29.583699 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:21:29.587699 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/az_ad_authz_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/az_adx_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/az_cosmos_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/az_storage_account_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/send_email_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/snow_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-08-06 05:21:18.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/wells_etl_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:21:29.583699 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-06 05:21:29.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-06 05:21:29.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 05:21:29.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-06 05:21:29.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-06 05:21:29.000000 wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.241613 wells-data-pipeline-cores-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/test/test_env_vars_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.241613 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/commons/dev_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19055 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/commons/env_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/commons/key_vaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/adx/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/adx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/adx/az_adx_data_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cores/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cores/az_ad_authz_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cores/az_storage_account_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cores/send_email_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cosmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cosmos/az_cosmos_data_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/etl/wells_etl_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/snow/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/snow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/snow/snow_data_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/wellview/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-07 14:28:00.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/wellview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:28:09.245613 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-07 14:28:09.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-07 14:28:09.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:28:09.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-07 14:28:09.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 14:28:09.000000 wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores.egg-info/top_level.txt
```

### Comparing `wells-data-pipeline-cores-0.0.3/setup.py` & `wells-data-pipeline-cores-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Wells Data Pipeline Cores
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "wells-data-pipeline-cores"
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/common.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/common.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/commons/dev_utils.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/commons/dev_utils.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/commons/env_variables.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/commons/env_variables.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/commons/key_vaults.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/commons/key_vaults.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/commons/utils.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/commons/utils.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/__init__.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cores/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,41 +4,17 @@
 
 # import base services into services package
 try:
     from wells_data_pipeline_cores.services.cores.az_ad_authz_service import AzAuthzService
 except Exception as ex:
     logging.warning("Export AzAuthzService error - %s", ex)
 
-try:
-    from wells_data_pipeline_cores.services.cores.send_email_service import SendEmailService
-except Exception as ex:
-    logging.warning("Export SendEmailService error - %s", ex)
-
-# support Snowflake
-try:
-    from wells_data_pipeline_cores.services.cores.snow_data_service import SnowDataService
-except Exception as ex:
-    logging.warning("Export SnowDataService error - %s", ex)
-
 # support Az Storage Account
 try:
     from wells_data_pipeline_cores.services.cores.az_storage_account_service import AzStorageAccountService
 except Exception as ex:
     logging.warning("Export AzStorageAccountService error - %s", ex)
 
-# support Az Cosmos DB
 try:
-    from wells_data_pipeline_cores.services.cores.az_cosmos_data_service import AzCosmosDataService, AzCosmosPartitionKeyModel
-except Exception as ex:
-    logging.warning("Export AzCosmosDataService error - %s", ex)
-
-# support Az ADX
-try:
-    from wells_data_pipeline_cores.services.cores.az_adx_data_service import  AzAdxDataService 
-except Exception as ex:
-    logging.warning("Export AzAdxDataService error - %s", ex)
-
-# support WellsETLService
-try:
-    from wells_data_pipeline_cores.services.cores.wells_etl_service import WellsETLService
+    from wells_data_pipeline_cores.services.cores.send_email_service import SendEmailService
 except Exception as ex:
-    logging.warning("Export WellsETLService error - %s", ex)
+    logging.warning("Export SendEmailService error - %s", ex)
```

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/az_ad_authz_service.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cores/az_ad_authz_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/az_adx_data_service.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/adx/az_adx_data_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/az_cosmos_data_service.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cosmos/az_cosmos_data_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/az_storage_account_service.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cores/az_storage_account_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/send_email_service.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/cores/send_email_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/snow_data_service.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/snow/snow_data_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores/services/cores/wells_etl_service.py` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores/services/etl/wells_etl_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from snowflake.snowpark import Session, Table, DataFrame, MergeResult
 from snowflake.snowpark.types import StructType
 from snowflake.snowpark.functions import when_matched, when_not_matched
 
 from wells_data_pipeline_cores.commons import EnvVariables
 
-from wells_data_pipeline_cores.services.cores.snow_data_service import SnowDataService
+from wells_data_pipeline_cores.services.snow import SnowDataService
 
 class WellsETLService(SnowDataService):
     def __init__(self, env_vars:EnvVariables):
         self.env_vars:EnvVariables = env_vars
         self.session:Session = self._create_snowpark_session(env_vars=env_vars)
 
     @abstractmethod
```

### Comparing `wells-data-pipeline-cores-0.0.3/wells_data_pipeline_cores.egg-info/SOURCES.txt` & `wells-data-pipeline-cores-0.0.4/wells_data_pipeline_cores.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 wells_data_pipeline_cores.egg-info/top_level.txt
 wells_data_pipeline_cores/commons/__init__.py
 wells_data_pipeline_cores/commons/dev_utils.py
 wells_data_pipeline_cores/commons/env_variables.py
 wells_data_pipeline_cores/commons/key_vaults.py
 wells_data_pipeline_cores/commons/utils.py
 wells_data_pipeline_cores/services/__init__.py
+wells_data_pipeline_cores/services/adx/__init__.py
+wells_data_pipeline_cores/services/adx/az_adx_data_service.py
 wells_data_pipeline_cores/services/cores/__init__.py
 wells_data_pipeline_cores/services/cores/az_ad_authz_service.py
-wells_data_pipeline_cores/services/cores/az_adx_data_service.py
-wells_data_pipeline_cores/services/cores/az_cosmos_data_service.py
 wells_data_pipeline_cores/services/cores/az_storage_account_service.py
 wells_data_pipeline_cores/services/cores/send_email_service.py
-wells_data_pipeline_cores/services/cores/snow_data_service.py
-wells_data_pipeline_cores/services/cores/wells_etl_service.py
+wells_data_pipeline_cores/services/cosmos/__init__.py
+wells_data_pipeline_cores/services/cosmos/az_cosmos_data_service.py
+wells_data_pipeline_cores/services/etl/__init__.py
+wells_data_pipeline_cores/services/etl/wells_etl_service.py
+wells_data_pipeline_cores/services/snow/__init__.py
+wells_data_pipeline_cores/services/snow/snow_data_service.py
+wells_data_pipeline_cores/services/wellview/__init__.py
```

