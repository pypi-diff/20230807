# Comparing `tmp/modular_sdk-2.2.0.tar.gz` & `tmp/modular_sdk-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/onsha/Develop/EPAM/temp-modular-sdk/dist/.tmp-ft0tlbgk/modular_sdk-2.2.0.tar", last modified: Thu Aug  3 12:12:20 2023, max compression
+gzip compressed data, was "/Users/onsha/Develop/EPAM/temp-modular-sdk/dist/.tmp-c2_4fghu/modular_sdk-2.2.1.tar", last modified: Mon Aug  7 14:21:29 2023, max compression
```

## Comparing `modular_sdk-2.2.0.tar` & `modular_sdk-2.2.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.852361 modular_sdk-2.2.0/
--rw-r--r--   0 onsha      (501) staff       (20)    11357 2023-06-29 14:09:33.000000 modular_sdk-2.2.0/LICENSE
--rw-r--r--   0 onsha      (501) staff       (20)     4014 2023-08-03 12:12:20.852515 modular_sdk-2.2.0/PKG-INFO
--rw-r--r--   0 onsha      (501) staff       (20)     3507 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/README.md
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.809026 modular_sdk-2.2.0/modular_sdk/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/__init__.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.815396 modular_sdk-2.2.0/modular_sdk/commons/
--rw-r--r--   0 onsha      (501) staff       (20)     4869 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     5073 2023-08-03 12:11:18.000000 modular_sdk-2.2.0/modular_sdk/commons/constants.py
--rw-r--r--   0 onsha      (501) staff       (20)     2045 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/error_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)      200 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/exception.py
--rw-r--r--   0 onsha      (501) staff       (20)      800 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/helpers.py
--rw-r--r--   0 onsha      (501) staff       (20)     2642 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/log_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)      951 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/time_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)     2458 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/trace_helper.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.816547 modular_sdk-2.2.0/modular_sdk/connections/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/connections/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1754 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/connections/mongodb_connection.py
--rw-r--r--   0 onsha      (501) staff       (20)     4723 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/connections/rabbit_connection.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.817469 modular_sdk-2.2.0/modular_sdk/helpers/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/helpers/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)      985 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/helpers/response_helper.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.824546 modular_sdk-2.2.0/modular_sdk/models/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1579 2023-08-03 10:34:40.000000 modular_sdk-2.2.0/modular_sdk/models/application.py
--rw-r--r--   0 onsha      (501) staff       (20)      929 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/base_meta.py
--rw-r--r--   0 onsha      (501) staff       (20)      689 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/customer.py
--rw-r--r--   0 onsha      (501) staff       (20)     1050 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/execution_trace.py
--rw-r--r--   0 onsha      (501) staff       (20)      490 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/heartbeat.py
--rw-r--r--   0 onsha      (501) staff       (20)      712 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/job.py
--rw-r--r--   0 onsha      (501) staff       (20)      662 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/operation_mode.py
--rw-r--r--   0 onsha      (501) staff       (20)     1570 2023-08-03 10:34:40.000000 modular_sdk-2.2.0/modular_sdk/models/parent.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.828651 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)    22311 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_model.py
--rw-r--r--   0 onsha      (501) staff       (20)     2261 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_role_access_model.py
--rw-r--r--   0 onsha      (501) staff       (20)     7045 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_safe_update_model.py
--rw-r--r--   0 onsha      (501) staff       (20)    16520 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py
--rw-r--r--   0 onsha      (501) staff       (20)      811 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py
--rw-r--r--   0 onsha      (501) staff       (20)     2565 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/region.py
--rw-r--r--   0 onsha      (501) staff       (20)      476 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/setting.py
--rw-r--r--   0 onsha      (501) staff       (20)     4048 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/tenant.py
--rw-r--r--   0 onsha      (501) staff       (20)     1081 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/tenant_settings.py
--rw-r--r--   0 onsha      (501) staff       (20)    10963 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/modular.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.838835 modular_sdk-2.2.0/modular_sdk/services/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     4860 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/application_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     4559 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/aws_creds_provider.py
--rw-r--r--   0 onsha      (501) staff       (20)      803 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/customer_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     5073 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/environment_service.py
--rw-r--r--   0 onsha      (501) staff       (20)      618 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/events_service.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.841870 modular_sdk-2.2.0/modular_sdk/services/impl/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/impl/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)    25123 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/impl/maestro_credentials_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     9096 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/impl/maestro_rabbit_transport_service.py
--rw-r--r--   0 onsha      (501) staff       (20)      620 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/lambda_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     5862 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/parent_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     3751 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/rabbit_transport_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     2602 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/region_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     9806 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/settings_management_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     1488 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/sqs_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     7305 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/ssm_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     8390 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/sts_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     7445 2023-08-03 12:11:18.000000 modular_sdk-2.2.0/modular_sdk/services/tenant_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     2143 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/tenant_settings_service.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.843060 modular_sdk-2.2.0/modular_sdk/utils/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/__init__.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.844500 modular_sdk-2.2.0/modular_sdk/utils/job_tracer/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/job_tracer/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)      354 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/job_tracer/abstract.py
--rw-r--r--   0 onsha      (501) staff       (20)     3832 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/job_tracer/generic.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.846142 modular_sdk-2.2.0/modular_sdk/utils/operation_mode/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/operation_mode/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)      776 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/operation_mode/abstract.py
--rw-r--r--   0 onsha      (501) staff       (20)     2171 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/operation_mode/generic.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.847831 modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1061 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/abstract.py
--rw-r--r--   0 onsha      (501) staff       (20)     4091 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/generic.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.810954 modular_sdk-2.2.0/modular_sdk.egg-info/
--rw-r--r--   0 onsha      (501) staff       (20)     4014 2023-08-03 12:12:20.000000 modular_sdk-2.2.0/modular_sdk.egg-info/PKG-INFO
--rw-r--r--   0 onsha      (501) staff       (20)     2945 2023-08-03 12:12:20.000000 modular_sdk-2.2.0/modular_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 onsha      (501) staff       (20)        1 2023-08-03 12:12:20.000000 modular_sdk-2.2.0/modular_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 onsha      (501) staff       (20)      271 2023-08-03 12:12:20.000000 modular_sdk-2.2.0/modular_sdk.egg-info/requires.txt
--rw-r--r--   0 onsha      (501) staff       (20)       18 2023-08-03 12:12:20.000000 modular_sdk-2.2.0/modular_sdk.egg-info/top_level.txt
--rw-r--r--   0 onsha      (501) staff       (20)       86 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/pyproject.toml
--rw-r--r--   0 onsha      (501) staff       (20)      923 2023-08-03 12:12:20.853168 modular_sdk-2.2.0/setup.cfg
--rw-r--r--   0 onsha      (501) staff       (20)       38 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/setup.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.848585 modular_sdk-2.2.0/tests/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/__init__.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.850634 modular_sdk-2.2.0/tests/test_commons/
--rw-r--r--   0 onsha      (501) staff       (20)      119 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/test_commons/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1852 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/test_commons/import_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)     2846 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/test_commons/utils.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.851827 modular_sdk-2.2.0/tests/test_models/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/test_models/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)    11617 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/test_models/test_base_safe_update_model.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:29.014676 modular_sdk-2.2.1/
+-rw-r--r--   0 onsha      (501) staff       (20)    11357 2023-06-29 14:09:33.000000 modular_sdk-2.2.1/LICENSE
+-rw-r--r--   0 onsha      (501) staff       (20)     4014 2023-08-07 14:21:29.014818 modular_sdk-2.2.1/PKG-INFO
+-rw-r--r--   0 onsha      (501) staff       (20)     3507 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/README.md
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:28.972904 modular_sdk-2.2.1/modular_sdk/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/__init__.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:28.979580 modular_sdk-2.2.1/modular_sdk/commons/
+-rw-r--r--   0 onsha      (501) staff       (20)     4869 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/commons/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     5225 2023-08-07 14:20:57.000000 modular_sdk-2.2.1/modular_sdk/commons/constants.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2045 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/commons/error_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)      200 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/commons/exception.py
+-rw-r--r--   0 onsha      (501) staff       (20)      800 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/commons/helpers.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2642 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/commons/log_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)      951 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/commons/time_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2458 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/commons/trace_helper.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:28.980588 modular_sdk-2.2.1/modular_sdk/connections/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/connections/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1754 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/connections/mongodb_connection.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4723 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/connections/rabbit_connection.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:28.981333 modular_sdk-2.2.1/modular_sdk/helpers/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/helpers/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)      985 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/helpers/response_helper.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:28.988645 modular_sdk-2.2.1/modular_sdk/models/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1914 2023-08-07 08:28:37.000000 modular_sdk-2.2.1/modular_sdk/models/application.py
+-rw-r--r--   0 onsha      (501) staff       (20)      929 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/base_meta.py
+-rw-r--r--   0 onsha      (501) staff       (20)      689 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/customer.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1050 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/execution_trace.py
+-rw-r--r--   0 onsha      (501) staff       (20)      490 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/heartbeat.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1163 2023-08-07 08:28:37.000000 modular_sdk-2.2.1/modular_sdk/models/job.py
+-rw-r--r--   0 onsha      (501) staff       (20)      662 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/operation_mode.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1905 2023-08-07 08:28:37.000000 modular_sdk-2.2.1/modular_sdk/models/parent.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:28.993084 modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)    22841 2023-08-07 14:20:57.000000 modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/base_model.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2261 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/base_role_access_model.py
+-rw-r--r--   0 onsha      (501) staff       (20)     7045 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/base_safe_update_model.py
+-rw-r--r--   0 onsha      (501) staff       (20)    16620 2023-08-07 14:20:57.000000 modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py
+-rw-r--r--   0 onsha      (501) staff       (20)      811 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2565 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/region.py
+-rw-r--r--   0 onsha      (501) staff       (20)      476 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/setting.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4666 2023-08-07 08:28:37.000000 modular_sdk-2.2.1/modular_sdk/models/tenant.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1081 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/models/tenant_settings.py
+-rw-r--r--   0 onsha      (501) staff       (20)    10963 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/modular.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:29.003113 modular_sdk-2.2.1/modular_sdk/services/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4860 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/application_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4559 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/aws_creds_provider.py
+-rw-r--r--   0 onsha      (501) staff       (20)      803 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/customer_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     5073 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/environment_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)      618 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/events_service.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:29.005202 modular_sdk-2.2.1/modular_sdk/services/impl/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/impl/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)    25211 2023-08-07 08:28:37.000000 modular_sdk-2.2.1/modular_sdk/services/impl/maestro_credentials_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     9096 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/impl/maestro_rabbit_transport_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)      620 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/lambda_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     5862 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/parent_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     3751 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/rabbit_transport_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2602 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/region_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     9806 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/settings_management_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1488 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/sqs_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     7379 2023-08-07 14:20:57.000000 modular_sdk-2.2.1/modular_sdk/services/ssm_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     8390 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/sts_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     7979 2023-08-07 14:20:57.000000 modular_sdk-2.2.1/modular_sdk/services/tenant_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2143 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/services/tenant_settings_service.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:29.006043 modular_sdk-2.2.1/modular_sdk/utils/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/utils/__init__.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:29.007856 modular_sdk-2.2.1/modular_sdk/utils/job_tracer/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/utils/job_tracer/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)      354 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/utils/job_tracer/abstract.py
+-rw-r--r--   0 onsha      (501) staff       (20)     3832 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/utils/job_tracer/generic.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:29.009682 modular_sdk-2.2.1/modular_sdk/utils/operation_mode/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/utils/operation_mode/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)      776 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/utils/operation_mode/abstract.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2171 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/utils/operation_mode/generic.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:29.011161 modular_sdk-2.2.1/modular_sdk/utils/runtime_tracer/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/utils/runtime_tracer/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1061 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/modular_sdk/utils/runtime_tracer/abstract.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4091 2023-08-07 08:28:37.000000 modular_sdk-2.2.1/modular_sdk/utils/runtime_tracer/generic.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:28.975035 modular_sdk-2.2.1/modular_sdk.egg-info/
+-rw-r--r--   0 onsha      (501) staff       (20)     4014 2023-08-07 14:21:28.000000 modular_sdk-2.2.1/modular_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 onsha      (501) staff       (20)     2945 2023-08-07 14:21:28.000000 modular_sdk-2.2.1/modular_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 onsha      (501) staff       (20)        1 2023-08-07 14:21:28.000000 modular_sdk-2.2.1/modular_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 onsha      (501) staff       (20)      271 2023-08-07 14:21:28.000000 modular_sdk-2.2.1/modular_sdk.egg-info/requires.txt
+-rw-r--r--   0 onsha      (501) staff       (20)       18 2023-08-07 14:21:28.000000 modular_sdk-2.2.1/modular_sdk.egg-info/top_level.txt
+-rw-r--r--   0 onsha      (501) staff       (20)       86 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/pyproject.toml
+-rw-r--r--   0 onsha      (501) staff       (20)      923 2023-08-07 14:21:29.015476 modular_sdk-2.2.1/setup.cfg
+-rw-r--r--   0 onsha      (501) staff       (20)       38 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/setup.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:29.011885 modular_sdk-2.2.1/tests/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/tests/__init__.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:29.013432 modular_sdk-2.2.1/tests/test_commons/
+-rw-r--r--   0 onsha      (501) staff       (20)      119 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/tests/test_commons/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1852 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/tests/test_commons/import_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2846 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/tests/test_commons/utils.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-07 14:21:29.014208 modular_sdk-2.2.1/tests/test_models/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/tests/test_models/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)    11617 2023-06-30 09:15:05.000000 modular_sdk-2.2.1/tests/test_models/test_base_safe_update_model.py
```

### Comparing `modular_sdk-2.2.0/LICENSE` & `modular_sdk-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/PKG-INFO` & `modular_sdk-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular_sdk
-Version: 2.2.0
+Version: 2.2.1
 Summary: Data level integration for services built atop of Modular Framework
 Home-page: https://github.com/epam/modular-sdk
 Author: EPAM Systems
 Author-email: support@syndicate.team
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `modular_sdk-2.2.0/README.md` & `modular_sdk-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/commons/__init__.py` & `modular_sdk-2.2.1/modular_sdk/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/commons/constants.py` & `modular_sdk-2.2.1/modular_sdk/commons/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 AWS_COST_EXPLORER = 'AWS_COST_EXPLORER'
 AZURE_CSP_BILLING = 'AZURE_CSP_BILLING'
 AZURE_CSP_PARTNER = 'AZURE_CSP_PARTNER'
 AZURE_USAGE_DETAILS = 'AZURE_USAGE_DETAILS'
 GCP_BILLING_SERVICE = 'GCP_BILLING_SERVICE'
 AZURE_ENTERPRISE_BILLING = 'AZURE_ENTERPRISE_BILLING'
 CUSTODIAN_TYPE = 'CUSTODIAN'
+CUSTODIAN_ACCESS_TYPE = 'CUSTODIAN_ACCESS'
 CUSTODIAN_LICENSES_TYPE = 'CUSTODIAN_LICENSES'
 RIGHTSIZER_PARENT_TYPE = 'RIGHTSIZER'
 RIGHTSIZER_LICENSES_PARENT_TYPE = 'RIGHTSIZER_LICENSES'
 SIEM_DEFECT_DOJO_TYPE = 'SIEM_DEFECT_DOJO'
 ALL_PARENT_TYPES = [
     AWS_MANAGEMENT, AWS_ATHENA, AWS_COST_EXPLORER,
     AZURE_ENTERPRISE_BILLING, AZURE_USAGE_DETAILS,
@@ -109,28 +110,30 @@
 ENVS_TO_HIDE = set()
 HIDDEN_ENV_PLACEHOLDER = '****'
 
 # Tenant parent map types
 TENANT_PARENT_MAP_BILLING_TYPE = 'BILLING'
 TENANT_PARENT_MAP_MANAGEMENT_TYPE = 'MANAGEMENT'
 TENANT_PARENT_MAP_CUSTODIAN_TYPE = CUSTODIAN_TYPE
+TENANT_PARENT_MAP_CUSTODIAN_ACCESS_TYPE = CUSTODIAN_ACCESS_TYPE
 TENANT_PARENT_MAP_CUSTODIAN_LICENSES_TYPE = CUSTODIAN_LICENSES_TYPE
 TENANT_PARENT_MAP_RIGHTSIZER_TYPE = 'RIGHTSIZER'
 TENANT_PARENT_MAP_RIGHTSIZER_LICENSES_TYPE = 'RIGHTSIZER_LICENSES'
 TENANT_PARENT_MAP_SIEM_DEFECT_DOJO_TYPE = SIEM_DEFECT_DOJO_TYPE
 
 
 ALLOWED_TENANT_PARENT_MAP_KEYS = (
     TENANT_PARENT_MAP_BILLING_TYPE,
     TENANT_PARENT_MAP_MANAGEMENT_TYPE,
     TENANT_PARENT_MAP_CUSTODIAN_TYPE,
     TENANT_PARENT_MAP_RIGHTSIZER_TYPE,
     TENANT_PARENT_MAP_RIGHTSIZER_LICENSES_TYPE,
     TENANT_PARENT_MAP_SIEM_DEFECT_DOJO_TYPE,
-    TENANT_PARENT_MAP_CUSTODIAN_LICENSES_TYPE
+    TENANT_PARENT_MAP_CUSTODIAN_LICENSES_TYPE,
+    TENANT_PARENT_MAP_CUSTODIAN_ACCESS_TYPE
 )
 
 DEFAULT_AWS_REGION = 'us-east-1'
 
 # native cloud credentials envs
 # AWS
 ENV_AWS_ACCESS_KEY_ID = 'AWS_ACCESS_KEY_ID'
```

### Comparing `modular_sdk-2.2.0/modular_sdk/commons/error_helper.py` & `modular_sdk-2.2.1/modular_sdk/commons/error_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/commons/helpers.py` & `modular_sdk-2.2.1/modular_sdk/commons/helpers.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/commons/log_helper.py` & `modular_sdk-2.2.1/modular_sdk/commons/log_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/commons/time_helper.py` & `modular_sdk-2.2.1/modular_sdk/commons/time_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/commons/trace_helper.py` & `modular_sdk-2.2.1/modular_sdk/commons/trace_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/connections/mongodb_connection.py` & `modular_sdk-2.2.1/modular_sdk/connections/mongodb_connection.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/connections/rabbit_connection.py` & `modular_sdk-2.2.1/modular_sdk/connections/rabbit_connection.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/helpers/response_helper.py` & `modular_sdk-2.2.1/modular_sdk/helpers/response_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/models/base_meta.py` & `modular_sdk-2.2.1/modular_sdk/models/base_meta.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/models/customer.py` & `modular_sdk-2.2.1/modular_sdk/models/customer.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/models/execution_trace.py` & `modular_sdk-2.2.1/modular_sdk/models/execution_trace.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/models/operation_mode.py` & `modular_sdk-2.2.1/modular_sdk/models/operation_mode.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/models/parent.py` & `modular_sdk-2.2.1/modular_sdk/models/parent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pynamodb.attributes import UnicodeAttribute, MapAttribute, \
-    BooleanAttribute
+    BooleanAttribute, NumberAttribute
 
 from modular_sdk.models.pynamodb_extension.base_role_access_model import \
     BaseRoleAccessModel
 
 from pynamodb.indexes import AllProjection
 
 from modular_sdk.models.pynamodb_extension.base_model import BaseGSI
@@ -13,14 +13,17 @@
 CUSTOMER_ID = 'cid'
 APPLICATION_ID = 'aid'
 TYPE = 't'
 DESCRIPTION = 'descr'
 META = 'meta'
 IS_DELETED = 'd'
 DELETION_DATE = 'dd'
+CREATION_TIMESTAMP = 'ct'
+UPDATE_TIMESTAMP = 'ut'
+DELETION_TIMESTAMP = 'dt'
 
 MODULAR_PARENTS_TABLE_NAME = 'Parents'
 
 
 class CustomerIdTypeIndex(BaseGSI):
     class Meta(BaseMeta):
         index_name = f"{CUSTOMER_ID}-index"
@@ -40,9 +43,12 @@
     customer_id = UnicodeAttribute(attr_name=CUSTOMER_ID)
     application_id = UnicodeAttribute(attr_name=APPLICATION_ID)
     type = UnicodeAttribute(attr_name=TYPE)
     description = UnicodeAttribute(attr_name=DESCRIPTION, null=True)
     meta = MapAttribute(attr_name=META, default=dict)
     is_deleted = BooleanAttribute(attr_name=IS_DELETED)
     deletion_date = UnicodeAttribute(attr_name=DELETION_DATE, null=True)
+    creation_timestamp = NumberAttribute(attr_name=CREATION_TIMESTAMP, null=True)
+    update_timestamp = NumberAttribute(attr_name=UPDATE_TIMESTAMP, null=True)
+    deletion_timestamp = NumberAttribute(attr_name=DELETION_TIMESTAMP, null=True)
 
     customer_id_type_index = CustomerIdTypeIndex()
```

### Comparing `modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_model.py` & `modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,22 @@
         str: UnicodeAttribute,
         dict: MapAttribute,
         float: NumberAttribute,
         int: NumberAttribute,
         list: ListAttribute,
         tuple: ListAttribute,
         bool: BooleanAttribute,
-        bytes: JSONAttribute
+        bytes: JSONAttribute  # todo, BinaryAttribute would fit better but
     }
+    # ... but this class has a bug -> it does not perform data
+    # deserialization. The raw value from DB is returned all the time.
+    # For Unicode, Number, List, Bool it is more or less acceptable, and
+    # it works. For BinaryAttribute it will not work because BinaryAttribute
+    # class encodes the data to b64 before sending to DB. As you can guess,
+    # it does not decode the data when you receive it from DB.
 
     def serialize(self, value: Any) -> Any:
         value_type = type(value)
         attribute_class = self._types_to_attributes.get(value_type)
         if not attribute_class:
             raise AssertionError(
                 f'There is no serializer for type: {value_type}')
@@ -540,15 +546,17 @@
     payload_key_name = 'key'
 
     def __init__(self, lek: Optional[Union[dict, int]] = None):
         self._lek = lek
 
     def serialize(self) -> str:
         payload = {self.payload_key_name: self._lek}
-        return base64.urlsafe_b64encode(json.dumps(payload).encode()).decode()
+        return base64.urlsafe_b64encode(
+            json.dumps(payload, separators=(",", ":"), sort_keys=True).encode()
+        ).decode()
 
     @classmethod
     def deserialize(cls, s: Optional[str] = None) -> 'LastEvaluatedKey':
         if not s or not isinstance(s, str):
             return cls()
         _payload = {}
         try:
```

### Comparing `modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_role_access_model.py` & `modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/base_role_access_model.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_safe_update_model.py` & `modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/base_safe_update_model.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py` & `modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+import decimal
 import re
-from collections.abc import Iterator
 from itertools import islice
-from typing import Optional, Dict, List, Union
+from typing import Optional, Dict, List, Union, TypeVar, Iterator
 
-from modular_sdk.connections.mongodb_connection import MongoDBConnection
-from modular_sdk.commons import DynamoDBJsonSerializer
 from pymongo import DeleteOne, ReplaceOne, DESCENDING, ASCENDING
 from pymongo.collection import Collection
 from pymongo.errors import BulkWriteError
 from pynamodb import indexes
 from pynamodb.expressions.condition import \
     Condition
-from pynamodb.expressions.operand import Value, Path, _Increment, _Decrement, _ListAppend, _ListAppendOperand
+from pynamodb.expressions.operand import Value, Path, _ListAppend
+from pynamodb.expressions.update import SetAction, RemoveAction, Action
 from pynamodb.models import Model
 from pynamodb.settings import OperationSettings
-from pynamodb.expressions.update import SetAction, RemoveAction, Action
+
+from modular_sdk.commons import DynamoDBJsonSerializer
+from modular_sdk.connections.mongodb_connection import MongoDBConnection
+
+T = TypeVar('T')
 
 
-class Result(Iterator):
-    def __init__(self, result: Iterator,
+class Result(Iterator[T]):
+    def __init__(self, result: Iterator[T],
                  _evaluated_key: Optional[int] = None,
                  page_size: Optional[int] = None):
         self._result_it = result
         self._evaluated_key = _evaluated_key
         self._page_size = page_size
 
     @property
@@ -30,15 +33,15 @@
         _key = self._evaluated_key
         if _key is not None and _key < self._page_size:
             return _key
 
     def __iter__(self):
         return self
 
-    def __next__(self):
+    def __next__(self) -> T:
         # try:
         #     item = self._result_it.__next__()
         # except StopIteration as e:
         #     self._evaluated_key = None
         #     raise e
         item = self._result_it.__next__()
 
@@ -88,22 +91,25 @@
 
 
 class _PynamoDBExpressionsConverter:
     # Looks for [1], [2], [12], etc in a string
     index_regex: re.Pattern = re.compile('\[\d+\]')
 
     @staticmethod
-    def value_to_raw(value: Value) -> Union[str, dict, list]:
+    def value_to_raw(value: Value) -> Union[str, dict, list, int, float]:
         """
         PynamoDB operand Value contains only one element in a list. This
         element is a dict: {'pynamo type': 'value'}
         :param value:
         :return:
         """
-        return DynamoDBJsonSerializer.deserializer.deserialize(value.value)
+        val = DynamoDBJsonSerializer.deserializer.deserialize(value.value)
+        if isinstance(val, decimal.Decimal):
+            val = float(val)
+        return val
 
     @classmethod
     def path_to_raw(cls, path: Path) -> str:
         """
         You can query MongoDB by nested attributes (one.two.three) and by
         first nested lists (one.two.3). But not deeper, i.e 'one.two.3.four'
         won't work.
@@ -191,15 +197,15 @@
                     '$gte': cls.value_to_raw(condition.values[1]),
                     '$lte': cls.value_to_raw(condition.values[2])
                 }
             }
         if op == 'begins_with':
             return {
                 cls.path_to_raw(condition.values[0]): {
-                    '$regex': {f'^{cls.value_to_raw(condition.values[1])}'}
+                    '$regex': f'^{cls.value_to_raw(condition.values[1])}'
                 }
             }
         raise NotImplementedError(f'Operator: {op} is not supported')
 
 
 class UpdateExpressionConverter(_PynamoDBExpressionsConverter):
     """
@@ -246,15 +252,16 @@
             #     }
             raise NotImplementedError(
                 f'Operand of type: {value.__class__.__name__} not supported'
             )
         if isinstance(action, RemoveAction):
             path, = action.values
             return {
-                '$unset': {cls.path_to_raw(path): ""}  # empty string does not matter https://www.mongodb.com/docs/manual/reference/operator/update/unset/#mongodb-update-up.-unset
+                '$unset': {cls.path_to_raw(path): ""}
+                # empty string does not matter https://www.mongodb.com/docs/manual/reference/operator/update/unset/#mongodb-update-up.-unset
             }
         raise NotImplementedError(
             f'Action {action.__class__.__name__} is not implemented'
         )
 
 
 class PynamoDBToPyMongoAdapter:
```

### Comparing `modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py` & `modular_sdk-2.2.1/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/models/region.py` & `modular_sdk-2.2.1/modular_sdk/models/region.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/models/tenant.py` & `modular_sdk-2.2.1/modular_sdk/models/tenant.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 TENANT_NAME = 'n'
 MANAGEMENT_PARENT_ID = 'mpid'
 DISPLAY_NAME = 'dn'
 ACTIVATION_DATE = 'ad'
 
 DNTL_NAME_KEY = 'dntl'
 GENERAL_PROJECT_ID = 'acc'
+GOOGLE_ACCOUNT_NUMBER = 'accN'
 PRIMARY_CONTACTS = 'pc'
 SECONDARY_CONTACTS = 'sc'
 TENANT_MANAGER = 'tmc'
 DEFAULT_INSTANCE_OWNER = 'do'
 TENANT_CONTACT = 'ct'
 
 REGIONS = 'r'
@@ -73,14 +74,29 @@
         read_capacity_units = 1
         write_capacity_units = 1
         projection = AllProjection()
 
     project = UnicodeAttribute(attr_name=GENERAL_PROJECT_ID, hash_key=True)
 
 
+class AccountNumberIndex(BaseGSI):
+    """
+    This class represents an Account Number global secondary index
+    """
+
+    class Meta(BaseMeta):
+        index_name = F'{GOOGLE_ACCOUNT_NUMBER}-index'
+        read_capacity_units = 1
+        write_capacity_units = 1
+        projection = AllProjection()
+
+    account_number = UnicodeAttribute(attr_name=GOOGLE_ACCOUNT_NUMBER,
+                                      hash_key=True)
+
+
 class CustomerNameIndex(BaseGSI):
     class Meta(BaseMeta):
         index_name = f"{CUSTOMER_NAME}-index"
         read_capacity_units = 1
         write_capacity_units = 1
         projection = AllProjection()
 
@@ -101,16 +117,20 @@
     activation_date = UnicodeAttribute(attr_name=ACTIVATION_DATE, null=True)
     management_parent_id = UnicodeAttribute(attr_name=MANAGEMENT_PARENT_ID,
                                             null=True)
     project = UnicodeAttribute(attr_name=GENERAL_PROJECT_ID, null=True)
     regions = ListAttribute(of=RegionAttr, attr_name=REGIONS, default=list)
     contacts = Contacts(attr_name=TENANT_CONTACT, null=True)
     parent_map = MapAttribute(attr_name=PARENT_MAP, default=dict)
+    account_number = UnicodeAttribute(attr_name=GOOGLE_ACCOUNT_NUMBER,
+                                      null=True)
+
     customer_name_index = CustomerNameIndex()
     project_index = ProjectIndex()
     dntl_c_index = DisplayNameToLowerCloudIndex()
+    accN_index = AccountNumberIndex()
 
     def get_parent_id(self, type_: str) -> Optional[str]:
         assert type_ in ALLOWED_TENANT_PARENT_MAP_KEYS
         if type_ in self.parent_map:
             return self.parent_map[type_]
         return
```

### Comparing `modular_sdk-2.2.0/modular_sdk/models/tenant_settings.py` & `modular_sdk-2.2.1/modular_sdk/models/tenant_settings.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/modular.py` & `modular_sdk-2.2.1/modular_sdk/modular.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/application_service.py` & `modular_sdk-2.2.1/modular_sdk/services/application_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/aws_creds_provider.py` & `modular_sdk-2.2.1/modular_sdk/services/aws_creds_provider.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/customer_service.py` & `modular_sdk-2.2.1/modular_sdk/services/customer_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/environment_service.py` & `modular_sdk-2.2.1/modular_sdk/services/environment_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/events_service.py` & `modular_sdk-2.2.1/modular_sdk/services/events_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/impl/maestro_credentials_service.py` & `modular_sdk-2.2.1/modular_sdk/services/impl/maestro_credentials_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
 
 @dataclasses.dataclass()
 class CustodianApplicationMeta(AccessMeta):
     """
     Application with type 'CUSTODIAN' meta
     """
     username: Optional[str]
+    results_storage: Optional[str]
 
 
 @dataclasses.dataclass()
 class RabbitMQApplicationMeta(DataclassBase):
     """
     Application with type 'RABBITMQ' meta
     """
@@ -442,18 +443,19 @@
             if not credentials.get(ENV_AZURE_SUBSCRIPTION_ID):
                 credentials[ENV_AZURE_SUBSCRIPTION_ID] = tenant.project
             return credentials
         elif tenant.cloud == AWS_CLOUD:
             _LOG.info('Tenant`s cloud is AWS. Proxying creds')
             return credentials
         elif tenant.cloud == GOOGLE_CLOUD:
-            _LOG.warning('Creds are requested for google tenant. '
-                         'Adding project id')
-            if not credentials.get(ENV_CLOUDSDK_CORE_PROJECT):
-                credentials[ENV_CLOUDSDK_CORE_PROJECT] = tenant.project
+            _LOG.info('Creds are requested for google tenant. '
+                      'Adding project id')
+            credentials[ENV_CLOUDSDK_CORE_PROJECT] = tenant.project
+            _LOG.debug(f'Google credentials project_id: '
+                       f'{credentials[ENV_CLOUDSDK_CORE_PROJECT]}')
             return credentials
 
         _LOG.info('Not known cloud. Proxying whatever was received')
         return credentials
 
     def get_by_tenant(self, tenant: Union[Tenant, str],
                       key: Optional[Callable[[Tenant], Optional[str]]] = None
```

### Comparing `modular_sdk-2.2.0/modular_sdk/services/impl/maestro_rabbit_transport_service.py` & `modular_sdk-2.2.1/modular_sdk/services/impl/maestro_rabbit_transport_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/lambda_service.py` & `modular_sdk-2.2.1/modular_sdk/services/lambda_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/parent_service.py` & `modular_sdk-2.2.1/modular_sdk/services/parent_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/rabbit_transport_service.py` & `modular_sdk-2.2.1/modular_sdk/services/rabbit_transport_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/region_service.py` & `modular_sdk-2.2.1/modular_sdk/services/region_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/settings_management_service.py` & `modular_sdk-2.2.1/modular_sdk/services/settings_management_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/sqs_service.py` & `modular_sdk-2.2.1/modular_sdk/services/sqs_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/ssm_service.py` & `modular_sdk-2.2.1/modular_sdk/services/ssm_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,16 @@
         """
         In case the secret was saved successfully, its real name is returned.
         (the name can differ from the given one).
         In case something went wrong, None is returned
         """
         try:
             if isinstance(value, (list, dict)):
-                value = json.dumps(value)
+                value = json.dumps(value, separators=(",", ":"),
+                                   sort_keys=True)
             self.client.put_parameter(
                 Name=name,
                 Value=value,
                 Overwrite=True,
                 Type=_type)
             return name
         except ClientError as e:
```

### Comparing `modular_sdk-2.2.0/modular_sdk/services/sts_service.py` & `modular_sdk-2.2.1/modular_sdk/services/sts_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/services/tenant_service.py` & `modular_sdk-2.2.1/modular_sdk/services/tenant_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,14 +119,26 @@
         return Tenant.dntl_c_index.query(
             hash_key=dntl, range_key_condition=rc, filter_condition=fc,
             limit=limit, last_evaluated_key=last_evaluated_key,
             attributes_to_get=attributes_to_get
         )
 
     @staticmethod
+    def i_get_by_accN(accN: str, active: Optional[bool] = None,
+                      limit: int = None,
+                      last_evaluated_key: Union[dict, str] = None,
+                      attributes_to_get: List[str] = None):
+        fc = None if active is None else (Tenant.is_active == active)
+        return Tenant.accN_index.query(
+            hash_key=accN, filter_condition=fc,
+            limit=limit, last_evaluated_key=last_evaluated_key,
+            attributes_to_get=attributes_to_get
+        )
+
+    @staticmethod
     def add_to_parent_map(tenant: Tenant, parent: Parent,
                           type_: str) -> Tenant:
         if type_ not in ALLOWED_TENANT_PARENT_MAP_KEYS:
             _LOG.warning(f'Unsupported type \'{type_}\'. Available options: '
                          f'{", ".join(ALLOWED_TENANT_PARENT_MAP_KEYS)}')
             raise ModularException(
                 code=RESPONSE_BAD_REQUEST_CODE,
@@ -170,15 +182,15 @@
         tenant.update(actions=[
             Tenant.parent_map[type_].remove()
         ])
         return tenant
 
     @staticmethod
     def get_dto(tenant: Tenant):
+        """Be CAREFUL: returns both active and inactive regions"""
         tenant_json = tenant.get_json()
         regions = tenant_json.get('regions') or []
         tenant_json['account_id'] = tenant_json.pop('project', None)
         tenant_json['regions'] = [
-            each['maestro_name'] for each in regions
-            if 'maestro_name' in each and each.get('is_active') != False  # None is valid
+            each['maestro_name'] for each in regions if 'maestro_name' in each
         ]
         return tenant_json
```

### Comparing `modular_sdk-2.2.0/modular_sdk/services/tenant_settings_service.py` & `modular_sdk-2.2.1/modular_sdk/services/tenant_settings_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/utils/job_tracer/generic.py` & `modular_sdk-2.2.1/modular_sdk/utils/job_tracer/generic.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/utils/operation_mode/abstract.py` & `modular_sdk-2.2.1/modular_sdk/utils/operation_mode/abstract.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/utils/operation_mode/generic.py` & `modular_sdk-2.2.1/modular_sdk/utils/operation_mode/generic.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/abstract.py` & `modular_sdk-2.2.1/modular_sdk/utils/runtime_tracer/abstract.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/generic.py` & `modular_sdk-2.2.1/modular_sdk/utils/runtime_tracer/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import re
 from datetime import datetime
 from modular_sdk.services.environment_service import EnvironmentService
 from modular_sdk.services.events_service import EventsService
 from modular_sdk.services.lambda_service import LambdaService
 from modular_sdk.services.sqs_service import SQSService
-from modular_sdk.utils.runtime_tracer.abstarct import AbstractSegmentTracer, \
+from modular_sdk.utils.runtime_tracer.abstract import AbstractSegmentTracer, \
     AbstractSegment
 
 
 class Segment(AbstractSegment):
     def __init__(self, name: str, tracer: AbstractSegmentTracer):
         self.name = name
         self.started_at = datetime.utcnow()
```

### Comparing `modular_sdk-2.2.0/modular_sdk.egg-info/PKG-INFO` & `modular_sdk-2.2.1/modular_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modular-sdk
-Version: 2.2.0
+Version: 2.2.1
 Summary: Data level integration for services built atop of Modular Framework
 Home-page: https://github.com/epam/modular-sdk
 Author: EPAM Systems
 Author-email: support@syndicate.team
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `modular_sdk-2.2.0/modular_sdk.egg-info/SOURCES.txt` & `modular_sdk-2.2.1/modular_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/setup.cfg` & `modular_sdk-2.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = modular_sdk
-version = 2.2.0
+version = 2.2.1
 requires-python = >=3.8
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 license = Apache-2.0
 description = Data level integration for services built atop of Modular Framework
```

### Comparing `modular_sdk-2.2.0/tests/test_commons/import_helper.py` & `modular_sdk-2.2.1/tests/test_commons/import_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/tests/test_commons/utils.py` & `modular_sdk-2.2.1/tests/test_commons/utils.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.2.0/tests/test_models/test_base_safe_update_model.py` & `modular_sdk-2.2.1/tests/test_models/test_base_safe_update_model.py`

 * *Files identical despite different names*

