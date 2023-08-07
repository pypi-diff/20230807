# Comparing `tmp/bigeye_sdk-0.4.56.tar.gz` & `tmp/bigeye_sdk-0.4.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeye_sdk-0.4.56.tar", max compression
+gzip compressed data, was "bigeye_sdk-0.4.60.tar", max compression
```

## Comparing `bigeye_sdk-0.4.56.tar` & `bigeye_sdk-0.4.60.tar`

### file list

```diff
@@ -1,68 +1,69 @@
--rw-r--r--   0        0        0     2092 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/LICENSE
--rw-r--r--   0        0        0      873 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/README.md
--rw-r--r--   0        0        0     3727 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/__init__.py
--rw-r--r--   0        0        0       82 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/__version__.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/authentication/__init__.py
--rw-r--r--   0        0        0    17489 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/authentication/api_authentication.py
--rw-r--r--   0        0        0     1182 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/authentication/credentials.py
--rw-r--r--   0        0        0      734 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/authentication/enums.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/__init__.py
--rw-r--r--   0        0        0    10276 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/big_config_reports.py
--rw-r--r--   0        0        0     8116 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_context.py
--rw-r--r--   0        0        0     1579 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_functions.py
--rw-r--r--   0        0        0      701 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_models.py
--rw-r--r--   0        0        0     9206 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/yaml_model_base.py
--rw-r--r--   0        0        0     3042 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/class_ext/__init__.py
--rw-r--r--   0        0        0      233 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/class_ext/dataclass_ext.py
--rw-r--r--   0        0        0      402 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/class_ext/enum_ext.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/client/__init__.py
--rw-r--r--   0        0        0      389 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/client/base_client.py
--rw-r--r--   0        0        0    38926 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/client/datawatch_client.py
--rw-r--r--   0        0        0      201 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/client/enum.py
--rw-r--r--   0        0        0    38282 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/client/generated_datawatch_client.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/controller/__init__.py
--rw-r--r--   0        0        0      390 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/controller/metric_controller.py
--rw-r--r--   0        0        0    33079 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/controller/metric_suite_controller.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/decorators/__init__.py
--rw-r--r--   0        0        0      307 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/decorators/dataclass_decorators.py
--rw-r--r--   0        0        0       97 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     1018 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/__init__.py
--rw-r--r--   0        0        0     4469 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/athena.py
--rw-r--r--   0        0        0     5202 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/aws.py
--rw-r--r--   0        0        0     3343 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/bigconfig_functions.py
--rw-r--r--   0        0        0     3469 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/casing.py
--rw-r--r--   0        0        0     3215 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/core_py_functs.py
--rw-r--r--   0        0        0     4517 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/delta_functions.py
--rw-r--r--   0        0        0     2544 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/file_functs.py
--rw-r--r--   0        0        0      117 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/helpers.py
--rw-r--r--   0        0        0    20235 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/metric_functions.py
--rw-r--r--   0        0        0     2540 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/metric_run_functions.py
--rw-r--r--   0        0        0     1227 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/s3.py
--rw-r--r--   0        0        0     1676 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/schema_functions.py
--rw-r--r--   0        0        0     5088 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/search_and_match_functions.py
--rw-r--r--   0        0        0     4031 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/table_functions.py
--rw-r--r--   0        0        0     1701 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/functions/urlfuncts.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/com/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/com/bigeye/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/com/bigeye/models/__init__.py
--rw-r--r--   0        0        0   227101 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/com/bigeye/models/generated.py
--rw-r--r--   0        0        0        0 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/google/__init__.py
--rw-r--r--   0        0        0    14816 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/generated/google/api.py
--rw-r--r--   0        0        0      507 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/log/__init__.py
--rw-r--r--   0        0        0        1 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/__init__.py
--rw-r--r--   0        0        0      489 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/base_datawatch_facade.py
--rw-r--r--   0        0        0    27454 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/big_config.py
--rw-r--r--   0        0        0      778 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/collection_models.py
--rw-r--r--   0        0        0     3948 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/dbt_schema.py
--rw-r--r--   0        0        0     3504 2023-07-12 21:12:32.104437 bigeye_sdk-0.4.56/bigeye_sdk/model/delta_facade.py
--rw-r--r--   0        0        0     9456 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/model/metric_facade.py
--rw-r--r--   0        0        0     8396 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/model/protobuf_enum_facade.py
--rw-r--r--   0        0        0      220 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/model/protobuf_extensions.py
--rw-r--r--   0        0        0    50437 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/model/protobuf_message_facade.py
--rw-r--r--   0        0        0      865 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/model/sla_models.py
--rw-r--r--   0        0        0     7346 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/bigeye_sdk/serializable.py
--rw-r--r--   0        0        0     3685 2023-07-12 21:12:32.108437 bigeye_sdk-0.4.56/pyproject.toml
--rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.56/PKG-INFO
+-rw-r--r--   0        0        0     2092 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/LICENSE
+-rw-r--r--   0        0        0      873 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/README.md
+-rw-r--r--   0        0        0     3727 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/__init__.py
+-rw-r--r--   0        0        0       82 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/authentication/__init__.py
+-rw-r--r--   0        0        0    19990 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/authentication/api_authentication.py
+-rw-r--r--   0        0        0    12229 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/authentication/config.py
+-rw-r--r--   0        0        0     1182 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/authentication/credentials.py
+-rw-r--r--   0        0        0      734 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/authentication/enums.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/__init__.py
+-rw-r--r--   0        0        0    10367 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/big_config_reports.py
+-rw-r--r--   0        0        0     8116 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/validation_context.py
+-rw-r--r--   0        0        0     1579 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/validation_functions.py
+-rw-r--r--   0        0        0      701 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/validation_models.py
+-rw-r--r--   0        0        0     9206 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/yaml_model_base.py
+-rw-r--r--   0        0        0     3042 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/class_ext/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/class_ext/dataclass_ext.py
+-rw-r--r--   0        0        0      402 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/class_ext/enum_ext.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/client/__init__.py
+-rw-r--r--   0        0        0      389 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/client/base_client.py
+-rw-r--r--   0        0        0    38742 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/client/datawatch_client.py
+-rw-r--r--   0        0        0      201 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/client/enum.py
+-rw-r--r--   0        0        0    42489 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/client/generated_datawatch_client.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/controller/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-19 23:28:42.172207 bigeye_sdk-0.4.60/bigeye_sdk/controller/metric_controller.py
+-rw-r--r--   0        0        0    35203 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/controller/metric_suite_controller.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/decorators/dataclass_decorators.py
+-rw-r--r--   0        0        0       97 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     1354 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/__init__.py
+-rw-r--r--   0        0        0     4469 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/athena.py
+-rw-r--r--   0        0        0     5202 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/aws.py
+-rw-r--r--   0        0        0     3343 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/bigconfig_functions.py
+-rw-r--r--   0        0        0     3469 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/casing.py
+-rw-r--r--   0        0        0     3215 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/core_py_functs.py
+-rw-r--r--   0        0        0     4517 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/delta_functions.py
+-rw-r--r--   0        0        0     2544 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/file_functs.py
+-rw-r--r--   0        0        0      549 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/helpers.py
+-rw-r--r--   0        0        0    20235 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/metric_functions.py
+-rw-r--r--   0        0        0     2540 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/metric_run_functions.py
+-rw-r--r--   0        0        0     1227 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/s3.py
+-rw-r--r--   0        0        0     1676 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/schema_functions.py
+-rw-r--r--   0        0        0     5088 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/search_and_match_functions.py
+-rw-r--r--   0        0        0     4031 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/table_functions.py
+-rw-r--r--   0        0        0     1701 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/functions/urlfuncts.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/generated/com/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/generated/com/bigeye/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/generated/com/bigeye/models/__init__.py
+-rw-r--r--   0        0        0   229062 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/generated/com/bigeye/models/generated.py
+-rw-r--r--   0        0        0        0 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/generated/google/__init__.py
+-rw-r--r--   0        0        0    14816 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/generated/google/api.py
+-rw-r--r--   0        0        0      993 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/log/__init__.py
+-rw-r--r--   0        0        0        1 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/model/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/model/base_datawatch_facade.py
+-rw-r--r--   0        0        0    27454 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/model/big_config.py
+-rw-r--r--   0        0        0      778 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/model/collection_models.py
+-rw-r--r--   0        0        0     3948 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/model/dbt_schema.py
+-rw-r--r--   0        0        0     3504 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/model/delta_facade.py
+-rw-r--r--   0        0        0     9456 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/model/metric_facade.py
+-rw-r--r--   0        0        0     8396 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/model/protobuf_enum_facade.py
+-rw-r--r--   0        0        0      220 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/model/protobuf_extensions.py
+-rw-r--r--   0        0        0    51556 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/model/protobuf_message_facade.py
+-rw-r--r--   0        0        0      865 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/model/sla_models.py
+-rw-r--r--   0        0        0     7346 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/bigeye_sdk/serializable.py
+-rw-r--r--   0        0        0     3685 2023-07-19 23:28:42.176207 bigeye_sdk-0.4.60/pyproject.toml
+-rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.60/PKG-INFO
```

### Comparing `bigeye_sdk-0.4.56/LICENSE` & `bigeye_sdk-0.4.60/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/README.md` & `bigeye_sdk-0.4.60/README.md`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/__init__.py` & `bigeye_sdk-0.4.60/bigeye_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/authentication/api_authentication.py` & `bigeye_sdk-0.4.60/bigeye_sdk/authentication/api_authentication.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,100 +5,157 @@
 import binascii
 import configparser
 import glob
 import http.cookiejar
 import json
 import os
 import sqlite3
+import yaml
 import sys
 import tempfile
 import urllib.parse
 from os.path import exists
 from pathlib import Path
 
 import keyring
 import lz4.block
-import yaml
 from Cryptodome.Cipher import AES
 from Cryptodome.Protocol.KDF import PBKDF2
 from pydantic import BaseModel
 from pydantic.dataclasses import dataclass
 
 from bigeye_sdk.functions.aws import get_secret
 from bigeye_sdk.authentication.enums import BrowserType, OperatingSystem
+from bigeye_sdk.functions.file_functs import create_subdir_if_not_exists
 from bigeye_sdk.exceptions import BrowserAuthException
 from bigeye_sdk.log import get_logger
 from bigeye_sdk.serializable import YamlSerializable
 
 log = get_logger(__file__)
 
 HOME_DIR = str(Path.home())
+DEFAULT_CRED_FILE = os.path.join(HOME_DIR, '.bigeye', 'credentials.ini')
+OLD_DEFAULT_CRED_FILE = os.path.join(HOME_DIR, '.bigeye', 'default_cred.json')
 
 
 class AwsSecretIdentifier(BaseModel):
     secret_name: str
     aws_region: str
 
 
+# TODO add abstraction to this class. We can have an abstract method to get the auth headers 
+# for any subclass and then have every class return its respective headers to add to kwargs in _call_datawatch_impl.
 @dataclass
-class ApiAuthConf(YamlSerializable):
+class ApiAuth(YamlSerializable):
+
+    @classmethod
+    def load(cls, auth_file: str, workspace: str) -> ApiAuth:
+        auth_file = cls.find_user_credentials(auth_file)
+        if os.path.isfile(auth_file):
+            if auth_file.lower().endswith('.json'):
+                return cls.load_from_json_file(auth_file)
+            else:
+                return cls.load_from_ini_file(auth_file,workspace)
+        else:
+            return cls.load_from_base64(auth_file)
+
+    @classmethod
+    def load_from_ini_file(cls, auth_file: str, workspace: str) -> ApiAuth:
+        log.info(f'Loading API Conf: {auth_file}')
+        cp = configparser.ConfigParser()
+        cp.read(auth_file)
+        # Convert browser type to proper enum (config parser reads everything as strings)
+        for key, value in cp[workspace].items():
+            if key == 'browser':
+                cp[workspace][key] = BrowserType[value]
+        return cls.factory(cp[workspace])
 
     @classmethod
-    def load_from_file(cls, file: str) -> ApiAuthConf:
+    def load_from_json_file(cls, file: str) -> ApiAuth:
         log.info(f'Loading API Conf: {file}')
         with open(file) as json_file:
             return cls.factory(yaml.safe_load(json_file))
 
     @classmethod
     def load_cred_from_aws_secret(cls, region_name: str, secret_name: str):
-        log.info(f'Loading Snowflake Credential Secret.')
-        return ApiAuthConf.factory(get_secret(region_name=region_name,
+        log.info(f'Loading AWS Secret: {secret_name}')
+        return cls.factory(get_secret(region_name=region_name,
                                               secret_name=secret_name))
 
     @classmethod
     def load_from_base64(cls, encoded: str):
         try:
-            log.info("Loading API conf")
+            log.info("Loading API Conf")
             conf_dict = json.loads(base64.b64decode(encoded).decode('utf-8'))
             return cls.factory(conf_dict)
         except binascii.Error as e:
             log.error('Error decoding API configuration. Verify it is valid base64.')
             log.error(f'Error message: {e}')
             raise e
+        
+    @classmethod
+    def save_as_file(cls, auth_filename: str, cred: BrowserAPIAuth | BasicAPIAuth, workspace: str) -> None:
+        cp = configparser.ConfigParser()
+        if not auth_filename:
+            auth_filename = DEFAULT_CRED_FILE
+        cp.read(auth_filename)
+        cp[workspace] = cred.to_dict()
+        with open(auth_filename,'w+') as file:
+            cp.write(file)
+
+    @staticmethod
+    def find_user_credentials(auth_filename: str) -> str:
+        if auth_filename:
+            return auth_filename
+        elif 'BIGEYE_API_CRED_FILE' in os.environ:
+            return os.environ['BIGEYE_API_CRED_FILE']
+        elif os.path.exists(DEFAULT_CRED_FILE):
+            return DEFAULT_CRED_FILE
+        elif os.path.exists(OLD_DEFAULT_CRED_FILE):
+            return OLD_DEFAULT_CRED_FILE
+        else:
+            create_subdir_if_not_exists(path=DEFAULT_CRED_FILE, includes_file=True)
+            return DEFAULT_CRED_FILE
+
+    @classmethod
+    def find_and_parse_user_credentials(cls, auth_filename: str) -> configparser.ConfigParser:
+        cp = configparser.ConfigParser(default_section=None)
+        cp.read(cls.find_user_credentials(auth_filename))
+        return cp
 
     @staticmethod
-    def factory(conf: dict) -> ApiAuthConf:
+    def factory(conf: dict) -> ApiAuth:
         ex: Exception
 
-        for model_cls in [BasicAuthRequestLibConf, BrowserAuthConf]:
+        for model_cls in [BasicAPIAuth, BrowserAPIAuth]:
             try:
                 return model_cls(**conf)
             except Exception as e:
                 ex = e
 
         raise ex
 
 
 @dataclass
-class BasicAuthRequestLibConf(ApiAuthConf):
+class BasicAPIAuth(ApiAuth):
     """
-    Configuration models to bind required host and authentication details for data_modules runtimes.
+    Credential models to bind required host and authentication details for data_modules runtimes.
     """
     base_url: str
     """Host URL for the Bigeye -- e.g. app.bigeye.com"""
     user: str
     """Basic Auth user for this host."""
     password: str
     """Basic Auth password for this host."""
 
 
 @dataclass
-class BrowserAuthConf(ApiAuthConf):
+class BrowserAPIAuth(ApiAuth):
     """
-    Configuration to bind required host and auth details from browser cookies.
+    Credential model to bind required host and auth details from browser cookies.
 
     Attributes:
         browser: BrowserType
         browser_profile_user_name: str - the user name associated with the browser profile.
         base_url: str - the full url of the bigeye instance.
     """
     browser: BrowserType
@@ -142,15 +199,15 @@
     browser_profile_user_name: str
     browser: str
     domain_name: str
     _cookie_file: str = None
     _cookie_encryption_pass: str = None
     _iterations: int = None
 
-    def __init__(self, api_conf: BrowserAuthConf):
+    def __init__(self, api_conf: BrowserAPIAuth):
         super().__init__()
         self.browser_profile_user_name = api_conf.browser_profile_user_name
         self.browser = api_conf.browser.name
         self.domain_name = api_conf.get_domain_name()
         self._set_os_specific_attributes()
 
     def _set_os_specific_attributes(self):
@@ -310,15 +367,15 @@
     domain_name: str
     session_file: str = None
     session_file_lz4: str = None
     tmp_cookie_file: str = None
     osx_user_data_path: str = f'{HOME_DIR}/Library/Application Support/Firefox'
     linux_user_data_path: str = f'{HOME_DIR}/.mozilla/firefox'
 
-    def __init__(self, api_conf: BrowserAuthConf):
+    def __init__(self, api_conf: BrowserAPIAuth):
         super().__init__()
         self.domain_name = api_conf.get_domain_name()
         cookie_file = self.__find_cookie_file()
         self.__create_local_copy(cookie_file)
         self.session_file = os.path.join(
             os.path.dirname(cookie_file), 'sessionstore.js')
         self.session_file_lz4 = os.path.join(os.path.dirname(
```

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/authentication/credentials.py` & `bigeye_sdk-0.4.60/bigeye_sdk/authentication/credentials.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/authentication/enums.py` & `bigeye_sdk-0.4.60/bigeye_sdk/authentication/enums.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/big_config_reports.py` & `bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/big_config_reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,24 +80,25 @@
     not_supported = True
     return not_supported in [
         True if f"Metric type {mm.predefined_metric} not supported on table {invalid.fq_asset_name}" in
                 invalid.error_messages else False for mm in SimpleMetricType.get_metadata_metrics()
     ]
 
 
-def process_reports(output_path: str, strict_mode: bool):
+def process_reports(output_path: str, strict_mode: bool, process_stage: ProcessStage):
     report_files = []
     errors_reported = False
 
     source_reports = []
 
     for report in REPORTS:
-        file_name = f'{output_path}/{report.source_name.replace(" ", "_")}_{report.process_stage}.yml'
-        report.save(output_path=file_name)
-        report_files.append(file_name)
+        if process_stage == report.process_stage:
+            file_name = f'{output_path}/{report.source_name.replace(" ", "_")}_{report.process_stage}.yml'
+            report.save(output_path=file_name)
+            report_files.append(file_name)
         errors_reported = errors_reported or report.has_errors()
         source_reports.append(report.get_console_report())
 
     if errors_reported and strict_mode:
         raise BigConfigValidationException(
             FAILED_API_EXECUTION_MSG.format(
                 source_reports="\n".join(source_reports),
```

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_context.py` & `bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/validation_context.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_functions.py` & `bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/validation_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/validation_models.py` & `bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/validation_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/yaml_model_base.py` & `bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/yaml_model_base.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py` & `bigeye_sdk-0.4.60/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/client/datawatch_client.py` & `bigeye_sdk-0.4.60/bigeye_sdk/client/datawatch_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,151 @@
 from __future__ import annotations
 
 import time
 from abc import ABC
 from json import JSONDecodeError
-from typing import List, Optional, Dict, Tuple, Union
+from typing import List, Optional, Dict, Tuple
 
 import requests
 from requests.auth import HTTPBasicAuth
 
-from bigeye_sdk.authentication.api_authentication import BasicAuthRequestLibConf, BrowserAuthConf, ApiAuthConf
+from bigeye_sdk.authentication.api_authentication import BasicAPIAuth, BrowserAPIAuth, ApiAuth
 from bigeye_sdk.bigconfig_validation.big_config_reports import MetricSuiteReport, ProcessStage
 from bigeye_sdk.client.base_client import BaseApiClient
 from bigeye_sdk.client.enum import Method
+from bigeye_sdk.authentication.config import WorkspaceConfig
 from bigeye_sdk.client.generated_datawatch_client import GeneratedDatawatchClient
 from bigeye_sdk.exceptions.exceptions import NoSourcesFoundException, TableNotFoundException, \
-    BigconfigIncompleteException
+    BigconfigIncompleteException, WorkspaceNotSetException
 from bigeye_sdk.functions.delta_functions import infer_column_mappings, build_ccm, match_tables_by_name
 from bigeye_sdk.functions.metric_functions import set_default_model_type_for_threshold, is_freshness_metric
 from bigeye_sdk.functions.table_functions import get_table_column_priority_first, table_has_metric_time, \
     fully_qualified_table_to_elements
 from bigeye_sdk.generated.com.bigeye.models.generated import MetricCreationState, \
     MetricConfiguration, TimeInterval, Threshold, MetricType, MetricParameter, LookbackType, NotificationChannel, \
     CreateComparisonTableResponse, CreateComparisonTableRequest, \
     ComparisonTableConfiguration, IdAndDisplayName, ComparisonColumnMapping, \
     ColumnNamePair, Table, GetDebugQueriesResponse, Schema, Source, MetricSuite, MetricSuiteResponse, \
-    MetricNamesResponse, WorkflowStatusResponse, WorkflowProcessingStatus
+    MetricNamesResponse, WorkflowStatusResponse, WorkflowProcessingStatus, UserAuth, BigconfigWorkflowStatusResponse
 from bigeye_sdk.log import get_logger
 from bigeye_sdk.model.delta_facade import SimpleDeltaConfiguration, SimpleDeltaConfigurationFile
 from bigeye_sdk.model.metric_facade import SimpleUpsertMetricRequest
 from bigeye_sdk.model.protobuf_extensions import MetricDebugQueries
 from bigeye_sdk.model.protobuf_message_facade import SimpleColumnMapping, SimpleColumnPair
 
 log = get_logger(__file__)
 
 
-def datawatch_client_factory(auth: ApiAuthConf):
-    if isinstance(auth, BasicAuthRequestLibConf):
-        client = BasicAuthDatawatchClient(api_conf=auth)
-    elif isinstance(auth, BrowserAuthConf):
-        client = BrowserAuthDatawatchClient(api_conf=auth)
+def datawatch_client_factory(auth: ApiAuth, workspace_config: WorkspaceConfig = None, workspace_id: int = None):
+    if isinstance(auth, (BasicAPIAuth, BrowserAPIAuth)):
+        if workspace_config:
+            client = DatawatchClient(auth=auth, workspace_config=workspace_config)
+        elif workspace_id:
+            client = DatawatchClient(auth=auth, workspace_config=WorkspaceConfig(workspace_id=workspace_id))
+        else:
+            accessible_workspaces = get_user_auth(auth).workspaces
+            if len(accessible_workspaces) == 1:
+                # User has access to only 1 workspace, fallback to that
+                log.info(f"No workspace provided, defaulting to only valid workspace: {accessible_workspaces[0].name}")
+                workspace_config = WorkspaceConfig(workspace_id=accessible_workspaces[0].id)
+                client = DatawatchClient(auth=auth, workspace_config=workspace_config)
+            elif len(accessible_workspaces) > 1:
+                # User has access to more than 1 workspace, need to confirm correct one
+                raise WorkspaceNotSetException(f'Expected either workspace_config or workspace_id args to be passed.')
+            else:
+                # User has access to no workspaces - throw an error to let them know
+                raise WorkspaceNotSetException(f'No workspace access detected. Please check with your Bigeye '
+                                            'administrators to obtain access to a workspace.')
     else:
         raise Exception('Auth type not supported.')
-
     return client
 
+def get_user_auth(auth: ApiAuth) -> UserAuth:
+    url = '/auth'
+    headers = {"Content-Type": "application/json", 
+            "Accept": "application/json"}
+    if isinstance(auth, BasicAPIAuth):
+        # basic auth not supported for /auth endpoint
+        # need to get cookies by first posting login request in session
+        session = requests.Session()
+        login = {"basic-email": (None,auth.user), 
+                 "basic-password": (None,auth.password)}
+        session.post(url=f'{auth.base_url}/ajaxsignin', 
+                     files=login)
+        response = session.get(
+            url=f'{auth.base_url}{url}',
+            headers=headers)
+    elif isinstance(auth, BrowserAPIAuth):
+        response = requests.get(
+            url=f'{auth.base_url}{url}', 
+            cookies=auth.auth_factory().get_cookies(),
+            headers=headers)
+
+    return UserAuth().from_dict(response.json())
+
+
 
 class DatawatchClient(BaseApiClient, GeneratedDatawatchClient, ABC):
+    
+    def __init__(self, auth: BasicAPIAuth | BrowserAPIAuth, workspace_config: WorkspaceConfig):
+        super().__init__(base_url=auth.base_url)
+        self._auth = auth
+        self.config = workspace_config
+    
+        
+    def _call_datawatch_impl(self, method: Method, url, body: str = None, params: dict = None):
+        try:
+            fq_url = f'{self._base_url}{url}'
+            log.info(f'Request Type: {method.name}; URL: {fq_url}; Body: {body}')
+            headers = {"Content-Type": "application/json", 
+                        "Accept": "application/json", 
+                        "x-bigeye-workspace-id": f'{self.config.workspace_id}'}
+            
+            if isinstance(self._auth, BasicAPIAuth):
+                kwargs = {
+                    'url':fq_url,
+                    'headers': headers, 
+                    'data': body, 
+                    'auth': HTTPBasicAuth(self._auth.user, self._auth.password),
+                    'params': params}
+            elif isinstance(self._auth, BrowserAPIAuth):
+                kwargs = {
+                    'url':fq_url,
+                    'headers': headers, 
+                    'data': body, 
+                    'cookies': self._auth.auth_factory().get_cookies(),
+                    'params': params}
+
+            if method == Method.GET:
+                response = requests.get(**kwargs)
+            elif method == Method.POST:
+                response = requests.post(**kwargs)
+            elif method == Method.PUT:
+                response = requests.put(**kwargs)
+            elif method == Method.DELETE:
+                response = requests.delete(**kwargs)
+            else:
+                raise Exception(f'Unsupported http method {method}')
+        except Exception as e:
+            log.error(f'Exception calling datawatch: {str(e)}')
+            raise e
+        else:
+            log.info(f'Return Code: {response.status_code}')
+            if response.status_code < 200 or response.status_code >= 300:
+                log.error(f'Error code returned from datawatch: {response.status_code} - {response.reason}')
+                raise Exception(response.text)
+            else:
+                # Not empty response
+                if response.status_code != 204:
+                    try:
+                        return response.json()
+                    except JSONDecodeError as e:
+                        log.info(f'Cannot decode response.  {response}')
+                        return ''
+                
 
     def delete_metrics(self, metrics: List[MetricConfiguration] = None):
         """
         Deletes multiple metrics.
         Args:
             metrics: List of metric configurations to delete.
         Warnings: Will log a warning when attempting to delete a metric created by Bigconfig.
@@ -557,33 +653,35 @@
 
     def post_metric_suite_queue(self, metric_suite: MetricSuite, apply: bool = False) -> MetricSuiteResponse:
         if apply:
             url = "/api/v1/metric-suites/queue"
         else:
             url = f"/api/v1/metric-suites/dry-run/queue"
 
+        # TODO update once backend returns a BigconfigWorkflowStatusResponse for inital call to queue
         response: WorkflowStatusResponse = WorkflowStatusResponse().from_dict(
             self._call_datawatch(Method.POST, url=url, body=metric_suite.to_json())
         )
 
         status_url = f"/api/v1/metric-suites/status/{response.workflow_id}"
         while response.status == WorkflowProcessingStatus.WORKFLOW_PROCESSING_STATUS_QUEUED or \
                 response.status == WorkflowProcessingStatus.WORKFLOW_PROCESSING_STATUS_IN_PROGRESS:
             log.info(f"Bigconfig in queue...")
             time.sleep(10)
-            status = self._call_datawatch(Method.GET, url=status_url)
-            wsr = WorkflowStatusResponse()
-            r: WorkflowStatusResponse = wsr.from_dict(status['workflowStatusResponse'])
-            response.status = WorkflowProcessingStatus(r.status)
+            bwsr: BigconfigWorkflowStatusResponse = BigconfigWorkflowStatusResponse().from_dict(
+                self._call_datawatch(Method.GET, url=status_url))
+            response.status = bwsr.workflow_status_response.status
+            
         log.info(f"Queuing complete. Workflow finished with status {response.status.name}")
+
         if response.status != WorkflowProcessingStatus.WORKFLOW_PROCESSING_STATUS_COMPLETED:
             err = f"Bigconfig workflow was not completed. Final status: {response.status.name}"
             raise BigconfigIncompleteException(err)
 
-        return MetricSuiteResponse().from_dict(status["metricSuiteResponse"])
+        return bwsr.metric_suite_response
 
     def upsert_metric(
             self,
             *,
             id: int = 0,
             schedule_frequency: Optional[TimeInterval] = None,
             filters: List[str] = [],
@@ -726,120 +824,8 @@
             url = f'/api/v1/metrics/{metric_id}/debug/queries'
             i = MetricDebugQueries(
                 metric_id=metric_id,
                 debug_queries=GetDebugQueriesResponse().from_dict(self._call_datawatch(Method.GET, url))
             )
             r.append(i)
 
-        return r
-
-
-class BasicAuthDatawatchClient(DatawatchClient):
-
-    def __init__(self, api_conf: BasicAuthRequestLibConf):
-        super().__init__(base_url=api_conf.base_url)
-        self._auth = HTTPBasicAuth(api_conf.user, api_conf.password)
-        pass
-
-    def _call_datawatch_impl(self, method: Method, url, body: str = None, params: dict = None):
-        try:
-            fq_url = f'{self._base_url}{url}'
-            log.info(f'Request Type: {method.name}; URL: {fq_url}; Body: {body}')
-            if method == Method.GET:
-                response = requests.get(
-                    fq_url,
-                    auth=self._auth,
-                    params=params
-                )
-            elif method == Method.POST:
-                response = requests.post(
-                    fq_url,
-                    headers={"Content-Type": "application/json", "Accept": "application/json"},
-                    data=body,
-                    auth=self._auth,
-                    params=params
-                )
-            elif method == Method.PUT:
-                response = requests.put(
-                    fq_url,
-                    headers={"Content-Type": "application/json", "Accept": "application/json"},
-                    data=body,
-                    auth=self._auth,
-                    params=params
-                )
-            elif method == Method.DELETE:
-                response = requests.delete(f'{self._base_url}{url}',
-                                           headers={"Content-Type": "application/json", "Accept": "application/json"},
-                                           data=body,
-                                           auth=self._auth, params=params)
-            else:
-                raise Exception(f'Unsupported http method {method}')
-        except Exception as e:
-            log.info(f'URL: {response.url}')
-            log.error(f'Exception calling datawatch: {str(e)}')
-            raise e
-        else:
-            log.info(f'URL: {response.url}')
-            log.info(f'Return Code: {response.status_code}')
-            if response.status_code < 200 or response.status_code >= 300:
-                errmsg = f'Error Code {response.status_code}: {response.text}'
-                log.error(errmsg)
-                raise Exception(errmsg)
-            else:
-                # Not empty response
-                try:
-                    if response.status_code != 204:
-                        return response.json()
-                except JSONDecodeError as e:
-                    log.info(f'Cannot decode response.  {response}')
-                    return ''
-
-
-class BrowserAuthDatawatchClient(DatawatchClient):
-    def __init__(self, api_conf: BrowserAuthConf):
-        super().__init__(base_url=api_conf.base_url)
-        self.api_conf = api_conf
-        self._cookies = self.api_conf.auth_factory().get_cookies()
-
-    def _call_datawatch_impl(self, method: Method, url, body: str = None, params: dict = None):
-        # TODO: This shouldn't repeat the above code when the only thing changing is a call to cookies, instead of auth.
-        try:
-            fq_url = f'{self._base_url}{url}'
-            log.info(f'Request Type: {method.name}; URL: {fq_url}; Body: {body}')
-            if method == Method.GET:
-                response = requests.get(
-                    fq_url,
-                    cookies=self._cookies
-                )
-            elif method == Method.POST:
-                response = requests.post(
-                    fq_url,
-                    headers={"Content-Type": "application/json", "Accept": "application/json"},
-                    data=body,
-                    cookies=self._cookies
-                )
-            elif method == Method.PUT:
-                response = requests.put(
-                    fq_url,
-                    headers={"Content-Type": "application/json", "Accept": "application/json"},
-                    data=body,
-                    cookies=self._cookies
-                )
-            elif method == Method.DELETE:
-                response = requests.delete(f'{self._base_url}{url}',
-                                           headers={"Content-Type": "application/json", "Accept": "application/json"},
-                                           data=body,
-                                           cookies=self._cookies)
-            else:
-                raise Exception(f'Unsupported http method {method}')
-        except Exception as e:
-            log.error(f'Exception calling datawatch: {str(e)}')
-            raise e
-        else:
-            log.info(f'Return Code: {response.status_code}')
-            if response.status_code < 200 or response.status_code >= 300:
-                log.error(f'Error code returned from datawatch: {response.status_code} - {response.reason}')
-                raise Exception(response.text)
-            else:
-                # Not empty response
-                if response.status_code != 204:
-                    return response.json()
+        return r
```

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/client/generated_datawatch_client.py` & `bigeye_sdk-0.4.60/bigeye_sdk/client/generated_datawatch_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,18 @@
     SchemaList, SchemaSearchRequest, DataNodeType, CreateDataNodeRequest, DataNode, \
     CreateLineageRelationshipRequest, LineageRelationship, CreateCollectionResponse, TimeRange, NotificationChannel, \
     CreateMetricTemplateRequest, MetricTemplate, MetricTemplateParametersFieldEntry, Warehouse, \
     CreateMetricTemplateResponse, VirtualTableRequest, VirtualTable, MetricTemplateParameterType, FieldType, \
     GetMetricTemplateListRequest, GetMetricTemplateListResponse, MetricTemplateSortField, UpdateVirtualTableRequest, \
     SchemaChangeSortField, GetSchemaChangesRequest, GetSchemaChangesResponse, SchemaChange, IntegrationsResponse, \
     TableauWorkbook, Integration, GetIntegrationEntitiesResponse, ConfigValue, GetConfigListResponse, WorkflowResponse, \
-    WorkflowStatusResponse, GetLineageRelationshipsForNodeResponse
+    WorkflowStatusResponse, GetLineageRelationshipsForNodeResponse, WorkspaceListResponse, BulkChangeGroupUsersRequest, \
+    GroupListResponse, GetUserListResponse, BulkChangeGroupUsersResponse, UserInviteRequest, GroupUserOperation, \
+    CreateOrUpdateWorkspaceRequest, Workspace, CreateOrUpdateGroupRequest, Group, RoleV2ListResponse, RoleOperation, \
+    BulkChangeGroupRolesRequest, BulkResponse
 
 # create logger
 from bigeye_sdk.log import get_logger
 from bigeye_sdk.model.protobuf_enum_facade import SimpleFieldType, SimpleMetricTemplateParameterType
 
 log = get_logger(__file__)
 
@@ -938,14 +941,91 @@
 
     def get_workflow_status(self, workflow_id: int) -> WorkflowStatusResponse:
         url = f"/api/v1/workflows/{workflow_id}/status"
         return WorkflowStatusResponse().from_dict(
             self._call_datawatch(method=Method.GET, url=url)
         )
 
+    def get_workspaces(self) -> WorkspaceListResponse:
+        url = '/api/v1/workspaces'
+        response = self._call_datawatch(Method.GET, url=url)
+        return WorkspaceListResponse().from_dict(response)
+
+    def create_workspace(self, workspace_name: str) -> CreateOrUpdateWorkspaceRequest:
+        url = '/api/v1/workspaces'
+        request = CreateOrUpdateWorkspaceRequest(name=workspace_name)
+        response = self._call_datawatch(Method.POST, url=url, body=request.to_json())
+        return Workspace().from_dict(response)
+
+    def update_workspace(self, workspace_name: str, workspace_id: int) -> CreateOrUpdateWorkspaceRequest:
+        url = f'/api/v1/workspaces/{workspace_id}'
+        request = CreateOrUpdateWorkspaceRequest(name=workspace_name)
+        response = self._call_datawatch(Method.PUT, url=url, body=request.to_json())
+        return Workspace().from_dict(response)
+    
+    def delete_workspace(self, workspace_id: int):
+        url = f'/api/v1/workspaces/{workspace_id}'
+        return self._call_datawatch(Method.DELETE, url=url)
+    
+    def get_users(self) -> GetUserListResponse:
+        url = '/user'
+        response = self._call_datawatch(Method.GET, url=url)
+        return GetUserListResponse().from_dict(response)
+    
+    def invite_user(self, user_name: str, user_email: str, group_ids: List[int]):
+        url = '/api/v1/users'
+        request = UserInviteRequest(name=user_name,email=user_email,group_ids=group_ids)
+        return User().from_dict(self._call_datawatch(Method.POST, url=url, body=request.to_json()))
+
+    def delete_user(self, user_id: int):
+        url = f'/user/{user_id}'
+        return self._call_datawatch(Method.DELETE, url=url)
+
+    def edit_users_groups(self, user_ids: List[int], group_ids: List[int], operation: GroupUserOperation) -> BulkChangeGroupUsersResponse:
+        url = '/api/v1/groups/users'
+        request = BulkChangeGroupUsersRequest(user_ids=user_ids,
+                                              group_ids=group_ids,
+                                              operation=operation)
+        response = self._call_datawatch(Method.PUT, url=url, body=request.to_json())
+        return BulkChangeGroupUsersResponse().from_dict(response)
+
+    def get_groups(self) -> GroupListResponse:
+        url = '/api/v1/groups'
+        response = self._call_datawatch(Method.GET, url=url)
+        return GroupListResponse().from_dict(response)
+
+    def create_group(self, group_name: str) -> CreateOrUpdateGroupRequest:
+        url = '/api/v1/groups'
+        request = CreateOrUpdateGroupRequest(name=group_name)
+        response = self._call_datawatch(Method.POST, url=url, body=request.to_json())
+        return Group().from_dict(response)
+
+    def update_group(self, group_name: str, group_id: int) -> CreateOrUpdateGroupRequest:
+        url = f'/api/v1/groups/{group_id}'
+        request = CreateOrUpdateGroupRequest(name=group_name)
+        response = self._call_datawatch(Method.PUT, url=url, body=request.to_json())
+        return Group().from_dict(response)
+
+    def delete_group(self, group_id: int):
+        url = f'/api/v1/groups/{group_id}'
+        return self._call_datawatch(Method.DELETE, url=url)
+    
+    def get_roles(self) -> RoleV2ListResponse:
+        url = '/api/v1/roles'
+        response = self._call_datawatch(Method.GET, url=url)
+        return RoleV2ListResponse().from_dict(response)
+    
+    def edit_group_roles(self, group_id: int, role_ids: List[int], operation: RoleOperation) -> BulkResponse:
+        url = '/api/v1/groups/roles'
+        request = BulkChangeGroupRolesRequest(role_ids=role_ids,
+                                              group_id=group_id,
+                                              operation=operation)
+        response = self._call_datawatch(Method.PUT, url=url, body=request.to_json())
+        return BulkResponse().from_dict(response)
+
     # def bulk_update_metrics(
     #         self,
     #         *,
     #         where: Optional[WhereClause] = None,
     #         edit_request: Optional[MetricConfiguration] = None,
     #         mute_request: Optional[MuteRequest] = None,
     #         is_run: bool = False,
```

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/controller/metric_suite_controller.py` & `bigeye_sdk-0.4.60/bigeye_sdk/controller/metric_suite_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os.path
 import sys
 from pathlib import Path
 from typing import List, Dict, Tuple, Union
+from rich.prompt import Confirm
+from rich.text import Text
 
 from bigeye_sdk.bigconfig_validation.big_config_reports import raise_files_contain_error_exception, MetricSuiteReport, \
-    process_reports, ProcessStage
+    process_reports, ProcessStage, REPORTS
 from bigeye_sdk.bigconfig_validation.validation_context import process_validation_errors, \
     get_validation_error_cnt, get_all_validation_errors_flat
 from bigeye_sdk.bigconfig_validation.yaml_validation_error_messages import SRC_NOT_EXISTS_FOR_DEPLOYMENT_ERRMSG, \
     METRIC_APPLICATION_ERROR, MISMATCHED_ATTRIBUTE_ACROSS_MULTIPLE_FILES
 from bigeye_sdk.client.datawatch_client import DatawatchClient
 from bigeye_sdk.exceptions.exceptions import FileLoadException, BigConfigValidationException, NoSourcesFoundException, FileNotFoundException
 from bigeye_sdk.functions.metric_functions import _is_table_level_metric
@@ -525,25 +527,28 @@
             apply: If true then Big Config will be applied to the workspace.  If false then a plan will be generated.
         """
         try:
             self.client.purge_metric_suites(source_names=purge_source_names,
                                             purge_all_sources=purge_all_sources,
                                             apply=apply
                                             )
-            process_reports(output_path=output_path, strict_mode=False)
+            process_stage = ProcessStage.APPLY if apply else ProcessStage.PLAN
+            process_reports(output_path=output_path, strict_mode=False, process_stage=process_stage)
         except NoSourcesFoundException as e:
             sys.exit(e.message)
 
+
     def execute_bigconfig(self,
                           input_path: List[str] = (Path.cwd()),
                           output_path: str = Path.cwd(),
                           apply: bool = False,
                           no_queue: bool = False,
                           recursive: bool = False,
-                          strict_mode: bool = False):
+                          strict_mode: bool = False,
+                          auto_approve: bool = False):
         """
         Executes an Apply or Plan for a Big Config.
         Args:
             input_path: path of source files.  If no path is given the current working directory will be used.
             output_path: path to dump the reports.  If no path is given the current working directory will be used.
             apply: If true then Big Config will be applied to the workspace.  If false then a plan will be generated.
             no_queue: If true, the bigconfig will be run without queuing
@@ -580,27 +585,58 @@
                                                 fixme_file_list=fixme_file_list)
 
         # Applies changes and overwrites once local validations have passed.
         # if apply:
         #     self._upsert_collections(bigconfig=bigconfig, overwrite=True,
         #                              apply=apply)  # Will always overwrite for Bigconfig.
 
+        if apply and not auto_approve:
+            # run a plan, ask for approval, then apply
+            self._process_metric_suites(metric_suites=metric_suites, output_path=output_path,
+                                     strict_mode=strict_mode, apply=apply, no_queue=no_queue,
+                                     process_stage=ProcessStage.PLAN)
+            approved = Confirm.ask(Text(f'Please review expected results. Are you sure you want to continue?',
+                                        style='bold red'))
+            if approved:
+                self._process_metric_suites(metric_suites=metric_suites, output_path=output_path,
+                                        strict_mode=strict_mode, apply=apply, no_queue=no_queue,
+                                        process_stage=ProcessStage.APPLY)
+        else:
+            self._process_metric_suites(metric_suites=metric_suites, output_path=output_path,
+                                    strict_mode=strict_mode, apply=apply, no_queue=no_queue)
+
+    def _process_metric_suites(self,
+                            metric_suites: List[MetricSuite],
+                            output_path: str = Path.cwd(),
+                            strict_mode: bool = False,
+                            apply: bool = False,
+                            no_queue: bool = False,
+                            process_stage: ProcessStage = ProcessStage.PLAN):
+        """Send metric suites to correct endpoints and process reports."""
+    
+        # if applying, clear out any plan reports that were needed for approvals.
+        if apply: REPORTS.clear()
+
+        # Only print reports for stage that user issued in command
+        user_command_stage = ProcessStage.APPLY if apply else ProcessStage.PLAN
+
         for metric_suite in metric_suites:
             j = metric_suite.to_json()
             if no_queue:
                 response = self.client.post_metric_suite(metric_suite=metric_suite, apply=apply)
             else:
                 response = self.client.post_metric_suite_queue(metric_suite=metric_suite, apply=apply)
             process_stage = ProcessStage.APPLY if apply else ProcessStage.PLAN
             MetricSuiteReport.from_datawatch_object(response,
-                                                    source_name=self.sources_by_id_ix[metric_suite.source_id].name,
-                                                    process_stage=process_stage)
-
-        process_reports(output_path=output_path, strict_mode=strict_mode)
-
+                                                source_name=self.sources_by_id_ix[metric_suite.source_id].name,
+                                                process_stage=user_command_stage)
+            
+        # process reports for the current stage - even if different from user issued command
+        process_reports(output_path=output_path, strict_mode=strict_mode, process_stage=process_stage)   
+    
 
 def combine_bigconfigs(bigconfigs: List[BigConfig]) -> BigConfig:
     to_return: BigConfig = BigConfig(
         type="BIGCONFIG_FILE",
         tag_definitions=[],
         row_creation_times=RowCreationTimes(),
         saved_metric_definitions=SavedMetricDefinitions(metrics=[]),
```

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/exceptions/exceptions.py` & `bigeye_sdk-0.4.60/bigeye_sdk/exceptions/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 
 
 class InvalidConfigurationException(Exception):
     def __init__(self, message: str):
         self.message = message
 
 
+class ConfigNotFoundException(Exception):
+    def __init__(self, message: str):
+        self.message = message
+
+
+class ConfigParseException(Exception):
+    def __init__(self, message: str):
+        self.message = message
+
+
 class BrowserAuthException(Exception):
     def __init__(self, message: str):
         self.message = message
 
 
 class BigConfigValidationException(Exception):
     def __init__(self, message: str):
@@ -37,7 +47,12 @@
     def __init__(self, message: str):
         self.message = message
 
 
 class BigconfigIncompleteException(Exception):
     def __init__(self, message: str):
         self.message = message
+
+
+class WorkspaceNotSetException(Exception):
+    def __init__(self, message: str):
+        self.message = message
```

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/athena.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/athena.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/aws.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/aws.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/bigconfig_functions.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/bigconfig_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/casing.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/casing.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/core_py_functs.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/core_py_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/delta_functions.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/delta_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/file_functs.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/file_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/metric_functions.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/metric_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/metric_run_functions.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/metric_run_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/s3.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/s3.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/schema_functions.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/schema_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/search_and_match_functions.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/search_and_match_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/table_functions.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/table_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/functions/urlfuncts.py` & `bigeye_sdk-0.4.60/bigeye_sdk/functions/urlfuncts.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/generated/com/bigeye/models/generated.py` & `bigeye_sdk-0.4.60/bigeye_sdk/generated/com/bigeye/models/generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -668,14 +668,23 @@
 
 class RoleOperation(betterproto.Enum):
     ROLE_OPERATION_UNSPECIFIED = 0
     ROLE_OPERATION_GRANT = 1
     ROLE_OPERATION_REVOKE = 2
 
 
+class DbtJobRunStatus(betterproto.Enum):
+    DBT_JOB_RUN_STATUS_UNSPECIFIED = 0
+    DBT_JOB_RUN_STATUS_SUCCESS = 1
+    DBT_JOB_RUN_STATUS_ERROR = 2
+    DBT_JOB_RUN_STATUS_QUEUED = 3
+    DBT_JOB_RUN_STATUS_STARTING = 4
+    DBT_JOB_RUN_STATUS_RUNNING = 5
+
+
 class ModelTypes(betterproto.Enum):
     MODEL_TYPE_UNDEFINED = 0
     MODEL_TYPE_MONOCLE = 1
 
 
 class MetadataOperation(betterproto.Enum):
     METADATA_OPERATION_UNSPECIFIED = 0
@@ -1670,33 +1679,34 @@
     is_favorite: bool = betterproto.bool_field(5)
     company_id: int = betterproto.int32_field(6)
     integration_entity_id: str = betterproto.string_field(7)
     integration_id: int = betterproto.int32_field(8)
     workspace_id: int = betterproto.int32_field(9)
     created_at: int = betterproto.int64_field(10)
     updated_at: int = betterproto.int64_field(11)
+    dbt_project_url: str = betterproto.string_field(12)
+
+
+@dataclass
+class DbtProjectSortOption(betterproto.Message):
+    sort_direction: "SortDirection" = betterproto.enum_field(1)
+    sort_field: "DbtProjectSortField" = betterproto.enum_field(2)
 
 
 @dataclass
 class GetDbtProjectsRequest(betterproto.Message):
     integration_id: int = betterproto.int32_field(1)
     page_size: int = betterproto.int32_field(2)
     page_cursor: str = betterproto.string_field(3)
     sort_options: List["DbtProjectSortOption"] = betterproto.message_field(4)
     search: str = betterproto.string_field(5)
     workspace_id: int = betterproto.int32_field(6)
 
 
 @dataclass
-class DbtProjectSortOption(betterproto.Message):
-    sort_direction: "SortDirection" = betterproto.enum_field(1)
-    sort_field: "DbtProjectSortField" = betterproto.enum_field(2)
-
-
-@dataclass
 class GetDbtProjectsResponse(betterproto.Message):
     projects: List["DbtProject"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
 
 @dataclass
 class SinglePathParamIntegrationIdRequest(betterproto.Message):
@@ -3787,20 +3797,31 @@
 @dataclass
 class GetBigQueryRegionResponse(betterproto.Message):
     region: str = betterproto.string_field(1)
     manually_set: bool = betterproto.bool_field(2)
 
 
 @dataclass
+class DbtJobRun(betterproto.Message):
+    id: int = betterproto.int32_field(1)
+    status: "DbtJobRunStatus" = betterproto.enum_field(2)
+    dbt_job_run_ext_id: int = betterproto.int32_field(3)
+    completed_at: int = betterproto.int64_field(4)
+    dbt_job_run_url: str = betterproto.string_field(5)
+    git_sha: str = betterproto.string_field(6)
+
+
+@dataclass
 class DbtJob(betterproto.Message):
     id: int = betterproto.int32_field(1)
     project_id: int = betterproto.int32_field(2)
     name: str = betterproto.string_field(3)
     dbt_job_ext_id: int = betterproto.int32_field(4)
     is_favorite: bool = betterproto.bool_field(5)
+    most_recent_job_runs: List["DbtJobRun"] = betterproto.message_field(6)
 
 
 @dataclass
 class UpsertDbtJob(betterproto.Message):
     id: int = betterproto.int32_field(1)
     project_id: int = betterproto.int32_field(2)
     name: str = betterproto.string_field(3)
@@ -3819,14 +3840,65 @@
 
 @dataclass
 class GetDbtJobsResponse(betterproto.Message):
     dbt_jobs: List["DbtJob"] = betterproto.message_field(1)
 
 
 @dataclass
+class SchemaDbtJobsRequest(betterproto.Message):
+    schema_id: int = betterproto.int32_field(1)
+
+
+@dataclass
+class SchemaDbtJobsResponse(betterproto.Message):
+    dbt_jobs: List["DbtJob"] = betterproto.message_field(1)
+
+
+@dataclass
+class TableDbtJobsRequest(betterproto.Message):
+    table_id: int = betterproto.int32_field(1)
+
+
+@dataclass
+class TableDbtJobsResponse(betterproto.Message):
+    dbt_jobs: List["DbtJob"] = betterproto.message_field(1)
+
+
+@dataclass
+class DbtJobRunRequest(betterproto.Message):
+    job_run_id: int = betterproto.int32_field(1)
+
+
+@dataclass
+class DbtJobRunResponse(betterproto.Message):
+    dbt_job_run: "DbtJobRun" = betterproto.message_field(1)
+
+
+@dataclass
+class DbtJobDetailRequest(betterproto.Message):
+    job_run_id: int = betterproto.int32_field(1)
+
+
+@dataclass
+class DbtJobDetailResponse(betterproto.Message):
+    dbt_job_detail: "DbtJob" = betterproto.message_field(1)
+
+
+@dataclass
+class IssueDbtInfoRequest(betterproto.Message):
+    issue_id: int = betterproto.int32_field(1)
+
+
+@dataclass
+class IssueDbtInfoResponse(betterproto.Message):
+    issue_id: int = betterproto.int32_field(1)
+    preceding_dbt_job_runs: List["DbtJobRun"] = betterproto.message_field(2)
+
+
+@dataclass
 class UpdateUserRoleRequest(betterproto.Message):
     role: "Role" = betterproto.enum_field(1)
 
 
 @dataclass
 class Empty(betterproto.Message):
     pass
```

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/generated/google/api.py` & `bigeye_sdk-0.4.60/bigeye_sdk/generated/google/api.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/model/big_config.py` & `bigeye_sdk-0.4.60/bigeye_sdk/model/big_config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/model/collection_models.py` & `bigeye_sdk-0.4.60/bigeye_sdk/model/collection_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/model/dbt_schema.py` & `bigeye_sdk-0.4.60/bigeye_sdk/model/dbt_schema.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/model/delta_facade.py` & `bigeye_sdk-0.4.60/bigeye_sdk/model/delta_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/model/metric_facade.py` & `bigeye_sdk-0.4.60/bigeye_sdk/model/metric_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/model/protobuf_enum_facade.py` & `bigeye_sdk-0.4.60/bigeye_sdk/model/protobuf_enum_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/model/protobuf_message_facade.py` & `bigeye_sdk-0.4.60/bigeye_sdk/model/protobuf_message_facade.py`

 * *Files 1% similar despite different names*

```diff
@@ -1014,14 +1014,16 @@
         Args:
             config_error_lines: The configuration serialized to yaml and split to lines.
 
         Returns: None
         """
         self.deployments_must_have_metric_type_if_not_saved_metric_id(config_error_lines=config_error_lines)
         self.deployments_cannot_have_metric_type_if_has_saved_metric_id(config_error_lines=config_error_lines)
+        self.deployments_freshness_metrics_must_have_valid_lookback_type(config_error_lines=config_error_lines)
+
 
     def deployments_must_have_metric_type_if_not_saved_metric_id(self, config_error_lines: List[str]):
         """
         Metric definitions must have a metric type if not referencing a saved metric by id
         (deployment in-line metrics)
         Args:
             config_error_lines: The configuration serialized to yaml and split to lines.
@@ -1043,14 +1045,38 @@
         Returns: None
         """
         if self.saved_metric_id and self.metric_type:
             error_message = OVERRIDE_METRIC_TYPE_SAVED_METRIC_ERRMSG.format(config_error_lines=config_error_lines)
             self.register_validation_error(error_lines=self.get_error_lines(),
                                            error_context_lines=config_error_lines,
                                            error_message=error_message)
+    
+    def deployments_freshness_metrics_must_have_valid_lookback_type(self, config_error_lines: List[str]):
+        """
+        Freshness metrics must have a data time window type. If any other window type is chosen then log
+        a warning message. The valid lookback type is automatically applied to the  metric in the backend, 
+        but user should be informed of this to limit confusion. 
+
+        See https://linear.app/torodata/issue/WIZ-2583/[061223]-metric-deployed-via-bigconfig-not-showing-as-clock-time
+
+        Args:
+            config_error_lines: The configuration serialized to yaml and split to lines.
+
+        Returns: None
+        """
+        if SimpleMetricType.is_freshness_metric(self.metric_type) \
+        and self.lookback \
+        and self.lookback.lookback_type != SimpleLookbackType.DATA_TIME:
+            if self.saved_metric_id:
+                log.warning(f'Invalid freshness metric configuration. Saved metric id: {self.saved_metric_id} was given a lookback of '
+                         f'type {self.lookback.lookback_type.name}. This will be changed to type {SimpleLookbackType.DATA_TIME}')
+            else:
+                log.warning(f'Invalid freshness metric configuration. Metric: {self.metric_type} was given a lookback of '
+                         f'type {self.lookback.lookback_type.name}. This will be changed to type {SimpleLookbackType.DATA_TIME}')          
+
 
     def saved_metrics_must_have_id(self, config_error_lines: List[str]):
         """
         Saved Metric Definitions must have a saved metric id.
         Args:
             config_error_lines: The configuration serialized to yaml and split to lines.
 
@@ -1128,21 +1154,14 @@
         if self.lookback:
             if self.lookback.lookback_window:
                 builder.lookback = self.lookback.lookback_window.to_datawatch_object()
 
             if self.lookback.lookback_type:
                 builder.lookback_type = self.lookback.lookback_type.to_datawatch_object()
 
-            """
-            Freshness metrics require data time lookback. This is handled by the backend.
-            See https://linear.app/torodata/issue/WIZ-2583/[061223]-metric-deployed-via-bigconfig-not-showing-as-clock-time
-            """
-            if SimpleMetricType.is_freshness_metric(self.metric_type):
-                builder.lookback_type = SimpleLookbackType.DATA_TIME.to_datawatch_object()
-
             builder.grain_seconds = self.lookback.bucket_size.to_seconds()
 
         if SimpleMetricType.is_freshness_volume(self.metric_type):
             builder.grain_seconds = BucketSize.HOUR.to_seconds()
 
         builder.muted_until_epoch_seconds = self.muted_until_epoch_seconds
```

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/model/sla_models.py` & `bigeye_sdk-0.4.60/bigeye_sdk/model/sla_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/bigeye_sdk/serializable.py` & `bigeye_sdk-0.4.60/bigeye_sdk/serializable.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.56/pyproject.toml` & `bigeye_sdk-0.4.60/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigeye-sdk"
-version = "0.4.56"
+version = "0.4.60"
 description = "Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically."
 license = "Proprietary"
 authors = ["Bigeye <support@bigeye.com>"]
 readme = "README.md"
 homepage = "https://docs.bigeye.com/docs"
 
 [[tool.poetry.source]]
```

### Comparing `bigeye_sdk-0.4.56/PKG-INFO` & `bigeye_sdk-0.4.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigeye-sdk
-Version: 0.4.56
+Version: 0.4.60
 Summary: Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.
 Home-page: https://docs.bigeye.com/docs
 License: Proprietary
 Author: Bigeye
 Author-email: support@bigeye.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: Other/Proprietary License
```

