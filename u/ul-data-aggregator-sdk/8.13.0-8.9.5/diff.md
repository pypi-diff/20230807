# Comparing `tmp/ul-data-aggregator-sdk-8.13.0.tar.gz` & `tmp/ul-data-aggregator-sdk-8.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-data-aggregator-sdk-8.13.0.tar", last modified: Mon Aug  7 08:29:21 2023, max compression
+gzip compressed data, was "ul-data-aggregator-sdk-8.9.5.tar", last modified: Thu Jun 22 13:30:39 2023, max compression
```

## Comparing `ul-data-aggregator-sdk-8.13.0.tar` & `ul-data-aggregator-sdk-8.9.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:29:21.728918 ul-data-aggregator-sdk-8.13.0/
--rw-r--r--   0 root         (0) root         (0)     1604 2023-08-07 08:29:21.728918 ul-data-aggregator-sdk-8.13.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1038 2022-01-12 20:57:03.000000 ul-data-aggregator-sdk-8.13.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:29:21.724918 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-16 08:03:27.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:29:21.724918 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-16 08:03:27.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-28 09:58:32.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/__tests__/test_integration_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:29:21.724918 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/brokers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:16.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/brokers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2022-07-04 09:50:16.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/brokers/data_aggregator_input_broker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:29:21.728918 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/constants/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:16.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/constants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2022-07-04 09:50:16.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/constants/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     3777 2023-04-10 11:22:21.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/constants/clock_timezones.py
--rw-rw-rw-   0 root         (0) root         (0)    21575 2023-07-31 09:28:33.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/constants/enums.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-07-04 09:50:16.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/constants/names.py
--rw-rw-rw-   0 root         (0) root         (0)      675 2022-08-06 16:57:19.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/dag.yml
--rw-rw-rw-   0 root         (0) root         (0)    73657 2023-08-07 07:20:21.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/data_aggregator_api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-06-28 07:24:55.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/data_aggregator_api_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2022-07-04 09:50:16.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/data_aggregator_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2022-07-04 09:50:16.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/data_aggregator_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2022-08-17 10:49:24.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    31993 2023-08-01 08:07:58.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/integration_message.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-07-04 09:50:16.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/lib.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-25 12:05:14.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-07-04 09:50:16.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/runtime_conf.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2022-08-04 15:37:04.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/self_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:29:21.728918 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-12 09:40:55.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3200 2023-06-28 07:24:55.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/types/device.py
--rw-rw-rw-   0 root         (0) root         (0)     3401 2023-06-28 07:24:55.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/types/get_data_gateway_network_device_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:29:21.728918 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:16.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2022-07-04 09:50:16.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/utils/devices_info_box_to_json.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-28 07:24:55.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/utils/internal_api_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-06-28 07:24:55.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/utils/internal_api_error_handler_old.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2022-08-04 15:37:04.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/utils/query_params.py
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-05-03 07:50:59.000000 ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/utils/round_dt.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 08:29:21.728918 ul-data-aggregator-sdk-8.13.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1464 2023-08-07 08:29:15.000000 ul-data-aggregator-sdk-8.13.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:29:21.728918 ul-data-aggregator-sdk-8.13.0/ul_data_aggregator_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2023-08-07 08:29:21.000000 ul-data-aggregator-sdk-8.13.0/ul_data_aggregator_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1544 2023-08-07 08:29:21.000000 ul-data-aggregator-sdk-8.13.0/ul_data_aggregator_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:29:21.000000 ul-data-aggregator-sdk-8.13.0/ul_data_aggregator_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-08-07 08:29:21.000000 ul-data-aggregator-sdk-8.13.0/ul_data_aggregator_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-08-07 08:29:21.000000 ul-data-aggregator-sdk-8.13.0/ul_data_aggregator_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2022-01-13 09:34:59.000000 ul-data-aggregator-sdk-8.9.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.042590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.042590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-21 09:12:57.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/test_integration_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.042590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/brokers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/brokers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/brokers/data_aggregator_input_broker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.046590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3777 2023-04-10 10:59:35.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/clock_timezones.py
+-rw-rw-rw-   0 root         (0) root         (0)    17477 2023-06-16 07:41:25.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/names.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2022-08-05 17:07:26.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/dag.yml
+-rw-rw-rw-   0 root         (0) root         (0)    50635 2023-06-22 13:20:40.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-22 13:20:40.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_api_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2022-08-17 09:11:15.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    26718 2023-06-22 13:20:40.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/integration_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-25 10:42:53.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/runtime_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2022-08-03 16:22:52.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/self_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.046590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-12 09:48:20.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/device.py
+-rw-rw-rw-   0 root         (0) root         (0)     3398 2023-06-08 09:55:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/get_data_gateway_network_device_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.050591 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/devices_info_box_to_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2022-10-12 09:48:20.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2022-11-08 19:19:34.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler_old.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2022-08-03 16:22:52.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/query_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-21 13:15:25.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/round_dt.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-06-22 13:26:15.000000 ul-data-aggregator-sdk-8.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/top_level.txt
```

### Comparing `ul-data-aggregator-sdk-8.13.0/PKG-INFO` & `ul-data-aggregator-sdk-8.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-aggregator-sdk
-Version: 8.13.0
+Version: 8.9.5
 Summary: Data aggregator sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-aggregator-sdk-8.13.0/README.md` & `ul-data-aggregator-sdk-8.9.5/README.md`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/__init__.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/__tests__/test_integration_message.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/test_integration_message.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/constants/clock_timezones.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/clock_timezones.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/dag.yml` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/dag.yml`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/data_aggregator_sdk.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/errors.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/integration_message.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/integration_message.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from datetime import datetime
-from decimal import Decimal
 from enum import Enum, IntEnum, unique
 from typing import Optional, List, Tuple, Dict, Any
 
+from api_utils.errors import ValidateApiError
 from pydantic import BaseModel, UUID4, root_validator, Field  # pylint: disable=no-name-in-module
-from ul_api_utils.errors import ValidateApiError
-from ul_api_utils.utils.api_method import ApiMethod
 from unipipeline.message.uni_message import UniMessage
 
-from data_aggregator_sdk.constants.enums import IntegrationV0MessageEvent, IntegrationV0MessageMetaBSChannelProtocol, \
-    ProtocolEnum, IntegrationV0MessageErrorType, ResourceKind
 from data_aggregator_sdk.types.device import NetworkSysTypeEnum
+from data_aggregator_sdk.constants.enums import IntegrationV0MessageEvent, IntegrationV0MessageMetaBSChannelProtocol, \
+    ProtocolEnum, IntegrationV0MessageErrorType
 
 
 class ProfileGranulation(Enum):
     """
     Enumeration of time granulations for profile packets
     """
     MINUTE_01 = "MINUTE_01"
@@ -198,26 +196,14 @@
     )
     value: datetime = Field(
         title="Clock value",
         description="Device timestamp clock value",
     )
 
 
-class IntegrationV0MessageUptime(BaseModel):
-    channel_id: int = Field(
-        1,
-        title="Channel ID",
-        description="Device channel Id",
-    )
-    uptime_s: float = Field(
-        title="Uptime seconds",
-        description="Uptime seconds value",
-    )
-
-
 class IntegrationV0MessageRelay(BaseModel):
     relay_id: int = Field(
         -1,
         title="Relay ID",
         description="Device relay ID",
     )
     value: bool = Field(
@@ -327,19 +313,19 @@
         title="Resource type",
         description="Consumption resource type",
     )
     channel: int = Field(
         title="Channel",
         description="Consumption channel number for collecting info",
     )
-    value: Decimal = Field(
+    value: float = Field(
         title="Channel value",
         description="Consumption channel value",
     )
-    overloading_value: Optional[Decimal] = Field(
+    overloading_value: Optional[float] = Field(
         None,
         title="Overloading channel value",
         description="Consumption channel overloading value. "
                     "If overloading_value = None - value is fully precise - must replace current. if not None - overload potentially could be",
     )
 
 
@@ -354,19 +340,19 @@
         description="Generation counter type",
     )
     resource_type: ResourceType = Field(
         title="Resource type",
         description="Generation resource type",
     )
 
-    value: Decimal = Field(
+    value: float = Field(
         title="Generation value",
         description="Generation channel value",
     )
-    overloading_value: Optional[Decimal] = Field(
+    overloading_value: Optional[float] = Field(
         None,
         title="Overloading value",
         description="Generation overloading value. "
                     "If overloading_value = None - value is fully precise - must replace current. if not None - overload potentially could be",
     )
 
 
@@ -394,19 +380,14 @@
 
 
 class IntegrationV0MessageCurrentTemperature(BaseModel):
     value: float = Field(
         title="Temperature value",
         description="Float value of environment current temperature",
     )
-    sensor_id: int = Field(
-        -1,
-        title="Sensor id",
-        description="Integer value of temperature sensor id, default: -1",
-    )
 
 
 class IntegrationV0MessageMetaNbFiBS0(BaseModel):
     station_id: int = Field(
         title="Station ID",
         description="Station unique identifier",
     )
@@ -599,19 +580,14 @@
         description="Structure which contains relay info for current device",
     )
     clock: List[IntegrationV0MessageClock] = Field(
         default_factory=list,
         title="Clock info",
         description="Structure which contains clock info for current device",
     )
-    uptime: List[IntegrationV0MessageUptime] = Field(
-        default_factory=list,
-        title="Uptime info",
-        description="Structure which contains uptime info for current device",
-    )
 
 
 class IntegrationMessageMetaIotAccountGateway(BaseModel):
     network_id: UUID4 = Field(
         title="Network ID",
         description="Network identifier",
     )
@@ -634,63 +610,14 @@
 class IntegrationMessageMetaRecycle(BaseModel):
     date: datetime = Field(
         title="Datetime recycle",
         description="Datetime field which contains packet recycle date",
     )
 
 
-class IntegrationMessageMetaExternalApiDataInput(BaseModel):
-    name: str = Field(
-        ...,
-        title='Api Integration name',
-        description='Api Integration name',
-    )
-    uri: str = Field(
-        ...,
-        title='External api uri',
-        description='External api uri',
-    )
-    path: str = Field(
-        ...,
-        title='External api path',
-        description='External api path',
-    )
-    api_method: ApiMethod = Field(
-        ...,
-        title='Api Method',
-        description='Api Method',
-    )
-    query_params: Optional[Dict[str, str]] = Field(
-        None,
-        title='Query Parameters',
-        description='Query Parameters',
-    )
-    status_code: int = Field(
-        ...,
-        title='Request status code',
-        description='Request status code',
-    )
-    body: Optional[str] = Field(
-        None,
-        title='Request Body',
-        description='Request Body',
-    )
-    headers: Optional[Dict[str, str]] = Field(
-        None,
-        title='Request Headers',
-        description='request headers',
-
-    )
-    current_dt: datetime = Field(
-        ...,
-        title="request response date and time",
-        description="The current date and time of the sender at the time of sending",
-    )
-
-
 class IntegrationMessageMetaUniversalDataInput(BaseModel):
     user_id: UUID4 = Field(
         ...,
         title="Sender user identifier",     # ApiUser.id
         description="Uniq UUID of user",
     )    # DA token id
     name: str = Field(
@@ -729,19 +656,14 @@
         description="Sender software / hardware version",
     )
     note: str = Field(
         ...,
         title="Note about sender",
         description="Any usefull information about sender",
     )
-    ipv4: str = Field(
-        ...,
-        title='IPv4 sender address',
-        description="A unique numerical identifier for every sender that send through the internet",
-    )
 
 
 class IntegrationV0MessageMeta(BaseModel):
     nbfi_bs0: Optional[IntegrationV0MessageMetaNbFiBS0] = Field(
         None,
         title="NBFi BS0 meta message structure",
         description="NBFi BS0 meta message structure",
@@ -757,19 +679,14 @@
         description="BS HTTP meta message structure",
     )
     universal_data_input: Optional[IntegrationMessageMetaUniversalDataInput] = Field(
         None,
         title="Universal data input meta",
         description="Universal data input meta structure",
     )
-    external_api_data_input: Optional[IntegrationMessageMetaExternalApiDataInput] = Field(
-        None,
-        title="External api data input meta",
-        description="External api data input meta structure",
-    )
     iot_account_gateway: Optional[IntegrationMessageMetaIotAccountGateway] = Field(
         None,
         title="IoT account gateway",
         description="IoT account gateway structure",
     )
     recycle: Optional[IntegrationMessageMetaRecycle] = Field(
         None,
@@ -779,15 +696,14 @@
 
     @root_validator()
     def check_meta_exists(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         if not any((
             values.get('nbfi_bs0'),
             values.get('nbiot'),
             values.get('bs_http'),
-            values.get('external_api_data_input'),
             values.get('universal_data_input'),
             values.get('iot_account_gateway'),
             values.get('recycle'),
         )):
             raise ValueError('one of meta sctructure must be set')
         return values
 
@@ -896,37 +812,7 @@
         description="Datetime calculation info",
     )
     error: Optional[IntegrationV0MessageError] = Field(
         None,
         title="Error info",
         description="Error structure contains error type and error message string",
     )
-
-
-INTEGRATION_MESSAGE_RESOURCE_TYPE_AND_COUNTER_TYPE__TO__CONSUMED_RESOURCE_KIND: Dict[Tuple[ResourceType, CounterType], ResourceKind] = {
-    (ResourceType.COMMON, CounterType.ENERGY_PHASE_A): ResourceKind.PHASE_A_ACTIVE_CONSUMED,  # TODO: for uiversal api tmp resolution
-    (ResourceType.COMMON, CounterType.ENERGY_PHASE_B): ResourceKind.PHASE_B_ACTIVE_CONSUMED,  # TODO: for uiversal api tmp resolution
-    (ResourceType.COMMON, CounterType.ENERGY_PHASE_C): ResourceKind.PHASE_C_ACTIVE_CONSUMED,  # TODO: for uiversal api tmp resolution
-    (ResourceType.COMMON, CounterType.COMMON): ResourceKind.COMMON_CONSUMED,
-    (ResourceType.ENERGY_ACTIVE, CounterType.COMMON): ResourceKind.COMMON_ACTIVE_CONSUMED,
-    (ResourceType.ENERGY_REACTIVE, CounterType.COMMON): ResourceKind.COMMON_REACTIVE_CONSUMED,
-    (ResourceType.ENERGY_ACTIVE, CounterType.ENERGY_PHASE_A): ResourceKind.PHASE_A_ACTIVE_CONSUMED,
-    (ResourceType.ENERGY_REACTIVE, CounterType.ENERGY_PHASE_A): ResourceKind.PHASE_A_REACTIVE_CONSUMED,
-    (ResourceType.ENERGY_ACTIVE, CounterType.ENERGY_PHASE_B): ResourceKind.PHASE_B_ACTIVE_CONSUMED,
-    (ResourceType.ENERGY_REACTIVE, CounterType.ENERGY_PHASE_B): ResourceKind.PHASE_B_REACTIVE_CONSUMED,
-    (ResourceType.ENERGY_ACTIVE, CounterType.ENERGY_PHASE_C): ResourceKind.PHASE_C_ACTIVE_CONSUMED,
-    (ResourceType.ENERGY_REACTIVE, CounterType.ENERGY_PHASE_C): ResourceKind.PHASE_C_REACTIVE_CONSUMED,
-}
-INTEGRATION_MESSAGE_RESOURCE_TYPE_AND_COUNTER_TYPE__TO__GENERATED_RESOURCE_KIND: Dict[Tuple[ResourceType, CounterType], ResourceKind] = {
-    (ResourceType.COMMON, CounterType.ENERGY_PHASE_A): ResourceKind.COMMON_ACTIVE_GENERATED,  # TODO: for uiversal api tmp resolution
-    (ResourceType.COMMON, CounterType.ENERGY_PHASE_B): ResourceKind.COMMON_ACTIVE_GENERATED,  # TODO: for uiversal api tmp resolution
-    (ResourceType.COMMON, CounterType.ENERGY_PHASE_C): ResourceKind.COMMON_ACTIVE_GENERATED,  # TODO: for uiversal api tmp resolution
-    (ResourceType.COMMON, CounterType.COMMON): ResourceKind.COMMON_GENERATED,
-    (ResourceType.ENERGY_ACTIVE, CounterType.COMMON): ResourceKind.COMMON_ACTIVE_GENERATED,
-    (ResourceType.ENERGY_REACTIVE, CounterType.COMMON): ResourceKind.COMMON_REACTIVE_GENERATED,
-    (ResourceType.ENERGY_ACTIVE, CounterType.ENERGY_PHASE_A): ResourceKind.PHASE_A_ACTIVE_GENERATED,
-    (ResourceType.ENERGY_REACTIVE, CounterType.ENERGY_PHASE_A): ResourceKind.PHASE_A_REACTIVE_GENERATED,
-    (ResourceType.ENERGY_ACTIVE, CounterType.ENERGY_PHASE_B): ResourceKind.PHASE_B_ACTIVE_GENERATED,
-    (ResourceType.ENERGY_REACTIVE, CounterType.ENERGY_PHASE_B): ResourceKind.PHASE_B_REACTIVE_GENERATED,
-    (ResourceType.ENERGY_ACTIVE, CounterType.ENERGY_PHASE_C): ResourceKind.PHASE_C_ACTIVE_GENERATED,
-    (ResourceType.ENERGY_REACTIVE, CounterType.ENERGY_PHASE_C): ResourceKind.PHASE_C_REACTIVE_GENERATED,
-}
```

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/types/device.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 from uuid import UUID
 
-from ul_api_utils.api_resource.api_response_payload_alias import ApiBaseUserModelPayloadResponse
-from ul_api_utils.api_resource.api_response import JsonApiResponsePayload
+from api_utils.api_resource.api_response_payload_alias import ApiBaseUserModelPayloadResponse
+from api_utils.api_resource.api_response import JsonApiResponsePayload
 
 from data_aggregator_sdk.constants.enums import DeviceModificationTypeEnum, NetworkSysTypeEnum, NetworkTypeEnum, \
     ProtocolEnum, ResourceKind
 
 
 class ApiDataGatewayResponse(ApiBaseUserModelPayloadResponse):
     name: str
```

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/types/get_data_gateway_network_device_list.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/get_data_gateway_network_device_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from uuid import UUID
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 from pydantic import UUID4, BaseModel
-from ul_api_utils.api_resource.api_response_payload_alias import ApiBaseUserModelPayloadResponse, JsonApiResponsePayload
+from api_utils.api_resource.api_response_payload_alias import ApiBaseUserModelPayloadResponse, JsonApiResponsePayload
 
 from data_aggregator_sdk.constants.enums import DeviceModificationTypeEnum, NetworkSysTypeEnum, NetworkTypeEnum, ProtocolEnum
 from data_aggregator_sdk.types.device import ApiDeviceMeterPayloadResponse
 
 
 # REQUEST BODY
```

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/utils/internal_api_error_handler.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import wraps
 from typing import Any, Callable, Dict, List, TypeVar, cast
 
-from ul_api_utils.errors import Client4XXInternalApiError, Server5XXInternalApiError, \
+from api_utils.errors import Client4XXInternalApiError, Server5XXInternalApiError, \
     ResponseJsonInternalApiError, NotFinishedRequestInternalApiError
 
 from data_aggregator_sdk.errors import DataAggregatorRequestError, DataAggregatorResponseError
 
 TKwargs = TypeVar('TKwargs', bound=Dict[str, Any])
 
 STDResp = TypeVar('STDResp', bound=Dict[str, Any] | List[Dict[str, Any]])    # TODO:  Dict[str, Any] -> JsonApiResponsePayload
```

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/utils/internal_api_error_handler_old.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import wraps
 from typing import Any, Callable, Dict, List, TypeVar
 
-from ul_api_utils.errors import Client4XXInternalApiError, Server5XXInternalApiError, \
+from api_utils.errors import Client4XXInternalApiError, Server5XXInternalApiError, \
     ResponseJsonInternalApiError, NotFinishedRequestInternalApiError
 
 from data_aggregator_sdk.errors import DataAggregatorRequestError, DataAggregatorResponseError
 
 TKwargs = TypeVar('TKwargs', bound=Dict[str, Any])
 
 STDResp = TypeVar('STDResp', bound=Dict[str, Any] | List[Dict[str, Any]])    # TODO:  Dict[str, Any] -> JsonApiResponsePayload
```

### Comparing `ul-data-aggregator-sdk-8.13.0/data_aggregator_sdk/utils/query_params.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.13.0/setup.py` & `ul-data-aggregator-sdk-8.9.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-data-aggregator-sdk',
-    version='8.13.0',
+    version='8.9.5',
     description='Data aggregator sdk',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={
         '': ['*.yml'],
         'data_aggregator_sdk': ['py.typed'],
@@ -31,19 +31,12 @@
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
     ],
     platforms='any',
     install_requires=[
         'requests>=2.26.0',
         'unipipeline>=1.4.3',
-        'ul-api-utils>=7.3.0',
+        'ul-api-utils>=7.2.6',
         'wtforms==3.0.1',
         'wtforms-alchemy==0.18.0',
-        # "ul-api-utils==7.3.1",
-        # 'ul-pyncp==1.0.5',
-        # 'ul-pysmp==1.0.3',
-        # 'ul-data-gateway-sdk==0.4.5',
-        # 'ul-api-utils==7.2.7',
-        # 'ul-py-tool==1.15.20',
-        # 'ul-db-utils==2.10.7'
     ],
 )
```

### Comparing `ul-data-aggregator-sdk-8.13.0/ul_data_aggregator_sdk.egg-info/PKG-INFO` & `ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-aggregator-sdk
-Version: 8.13.0
+Version: 8.9.5
 Summary: Data aggregator sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-aggregator-sdk-8.13.0/ul_data_aggregator_sdk.egg-info/SOURCES.txt` & `ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

