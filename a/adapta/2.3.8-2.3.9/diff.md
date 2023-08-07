# Comparing `tmp/adapta-2.3.8.tar.gz` & `tmp/adapta-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapta-2.3.8.tar", max compression
+gzip compressed data, was "adapta-2.3.9.tar", max compression
```

## Comparing `adapta-2.3.8.tar` & `adapta-2.3.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0    10693 2023-08-03 15:36:09.285228 adapta-2.3.8/LICENSE
--rw-r--r--   0        0        0      811 2023-08-03 15:36:09.285228 adapta-2.3.8/README.md
--rw-r--r--   0        0        0      663 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/__init__.py
--rw-r--r--   0        0        0       22 2023-08-03 15:36:28.025459 adapta-2.3.8/adapta/_version.py
--rw-r--r--   0        0        0      598 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/connectors/__init__.py
--rw-r--r--   0        0        0      694 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/connectors/service_bus/__init__.py
--rw-r--r--   0        0        0     1914 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/connectors/service_bus/_connector.py
--rw-r--r--   0        0        0     4111 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/logs/README.md
--rw-r--r--   0        0        0      667 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/logs/__init__.py
--rw-r--r--   0        0        0    12390 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/logs/_base.py
--rw-r--r--   0        0        0     2950 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/logs/_internal.py
--rw-r--r--   0        0        0      598 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/logs/handlers/__init__.py
--rw-r--r--   0        0        0     9167 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/logs/handlers/datadog_api_handler.py
--rw-r--r--   0        0        0     2211 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/logs/handlers/safe_stream_handler.py
--rw-r--r--   0        0        0      741 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/logs/models/__init__.py
--rw-r--r--   0        0        0      794 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/logs/models/_log_level.py
--rw-r--r--   0        0        0      963 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/logs/models/_logs_metadata.py
--rw-r--r--   0        0        0      672 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/metrics/__init__.py
--rw-r--r--   0        0        0     3215 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/metrics/_base.py
--rw-r--r--   0        0        0     1930 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/metrics/providers/README.md
--rw-r--r--   0        0        0      598 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/metrics/providers/__init__.py
--rw-r--r--   0        0        0     4466 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/metrics/providers/datadog_provider.py
--rw-r--r--   0        0        0      653 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/ml/__init__.py
--rw-r--r--   0        0        0     1223 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/ml/_model.py
--rw-r--r--   0        0        0      699 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/ml/mlflow/__init__.py
--rw-r--r--   0        0        0     5319 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/ml/mlflow/_client.py
--rw-r--r--   0        0        0     4012 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/ml/mlflow/_functions.py
--rw-r--r--   0        0        0      674 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/process_communication/__init__.py
--rw-r--r--   0        0        0     3362 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/process_communication/_models.py
--rw-r--r--   0        0        0      732 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/schema_management/README.md
--rw-r--r--   0        0        0      598 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/schema_management/__init__.py
--rw-r--r--   0        0        0     1219 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/schema_management/schema_entity.py
--rw-r--r--   0        0        0      598 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/security/__init__.py
--rw-r--r--   0        0        0     2140 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/security/clients/README.md
--rw-r--r--   0        0        0     1450 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/security/clients/__init__.py
--rw-r--r--   0        0        0     8358 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/security/clients/_azure_client.py
--rw-r--r--   0        0        0     2396 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/security/clients/_base.py
--rw-r--r--   0        0        0     1787 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/security/clients/_local_client.py
--rw-r--r--   0        0        0      598 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/security/clients/hashicorp_vault/__init__.py
--rw-r--r--   0        0        0     2695 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
--rw-r--r--   0        0        0     2601 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/security/clients/hashicorp_vault/kubernetes_client.py
--rw-r--r--   0        0        0     3454 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/security/clients/hashicorp_vault/oidc_client.py
--rw-r--r--   0        0        0     1952 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/security/clients/hashicorp_vault/token_client.py
--rw-r--r--   0        0        0      598 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/storage/__init__.py
--rw-r--r--   0        0        0     1208 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/storage/blob/README.md
--rw-r--r--   0        0        0      622 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/storage/blob/__init__.py
--rw-r--r--   0        0        0     9605 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/storage/blob/azure_storage_client.py
--rw-r--r--   0        0        0     4791 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/storage/blob/base.py
--rw-r--r--   0        0        0      665 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/storage/cache/__init__.py
--rw-r--r--   0        0        0     3451 2023-08-03 15:36:09.285228 adapta-2.3.8/adapta/storage/cache/_base.py
--rw-r--r--   0        0        0     3365 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/cache/redis_cache.py
--rw-r--r--   0        0        0     2451 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/database/README.md
--rw-r--r--   0        0        0      598 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/database/__init__.py
--rw-r--r--   0        0        0     4691 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/database/azure_sql.py
--rw-r--r--   0        0        0      675 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/database/models/__init__.py
--rw-r--r--   0        0        0     1447 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/database/models/_models.py
--rw-r--r--   0        0        0     7711 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/database/odbc.py
--rw-r--r--   0        0        0     4523 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/database/trino_sql.py
--rw-r--r--   0        0        0     2386 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/delta_lake/README.md
--rw-r--r--   0        0        0      721 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/delta_lake/__init__.py
--rw-r--r--   0        0        0    11493 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/delta_lake/_functions.py
--rw-r--r--   0        0        0     2247 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/delta_lake/_models.py
--rw-r--r--   0        0        0     1695 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/distributed_object_store/datastax_astra/README.md
--rw-r--r--   0        0        0      622 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/distributed_object_store/datastax_astra/__init__.py
--rw-r--r--   0        0        0    16952 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/distributed_object_store/datastax_astra/astra_client.py
--rw-r--r--   0        0        0      598 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/models/__init__.py
--rw-r--r--   0        0        0     5302 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/models/azure.py
--rw-r--r--   0        0        0     2063 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/models/base.py
--rw-r--r--   0        0        0     5711 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/models/format.py
--rw-r--r--   0        0        0     6630 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/models/hive.py
--rw-r--r--   0        0        0     1519 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/models/local.py
--rw-r--r--   0        0        0     1953 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/secrets/README.md
--rw-r--r--   0        0        0      666 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/secrets/__init__.py
--rw-r--r--   0        0        0     2216 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/secrets/_base.py
--rw-r--r--   0        0        0     2358 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/secrets/azure_secret_client.py
--rw-r--r--   0        0        0     2887 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
--rw-r--r--   0        0        0     2761 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/utils/README.md
--rw-r--r--   0        0        0      668 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/utils/__init__.py
--rw-r--r--   0        0        0     6463 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/utils/_common.py
--rw-r--r--   0        0        0     3930 2023-08-03 15:36:09.289229 adapta-2.3.8/adapta/utils/concurrent_task_runner.py
--rw-r--r--   0        0        0     2296 2023-08-03 15:36:28.025459 adapta-2.3.8/pyproject.toml
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 adapta-2.3.8/PKG-INFO
+-rw-r--r--   0        0        0    10693 2023-08-07 14:48:05.681997 adapta-2.3.9/LICENSE
+-rw-r--r--   0        0        0      811 2023-08-07 14:48:05.681997 adapta-2.3.9/README.md
+-rw-r--r--   0        0        0      663 2023-08-07 14:48:05.681997 adapta-2.3.9/adapta/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-07 14:48:30.892814 adapta-2.3.9/adapta/_version.py
+-rw-r--r--   0        0        0      598 2023-08-07 14:48:05.681997 adapta-2.3.9/adapta/connectors/__init__.py
+-rw-r--r--   0        0        0      694 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/connectors/service_bus/__init__.py
+-rw-r--r--   0        0        0     1914 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/connectors/service_bus/_connector.py
+-rw-r--r--   0        0        0     4111 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/logs/README.md
+-rw-r--r--   0        0        0      667 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/logs/__init__.py
+-rw-r--r--   0        0        0    12390 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/logs/_base.py
+-rw-r--r--   0        0        0     2950 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/logs/_internal.py
+-rw-r--r--   0        0        0      598 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/logs/handlers/__init__.py
+-rw-r--r--   0        0        0     9167 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/logs/handlers/datadog_api_handler.py
+-rw-r--r--   0        0        0     2211 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/logs/handlers/safe_stream_handler.py
+-rw-r--r--   0        0        0      741 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/logs/models/__init__.py
+-rw-r--r--   0        0        0      794 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/logs/models/_log_level.py
+-rw-r--r--   0        0        0      963 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/logs/models/_logs_metadata.py
+-rw-r--r--   0        0        0      672 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/metrics/__init__.py
+-rw-r--r--   0        0        0     3215 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/metrics/_base.py
+-rw-r--r--   0        0        0     1930 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/metrics/providers/README.md
+-rw-r--r--   0        0        0      598 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     4466 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/metrics/providers/datadog_provider.py
+-rw-r--r--   0        0        0      653 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/ml/__init__.py
+-rw-r--r--   0        0        0     1223 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/ml/_model.py
+-rw-r--r--   0        0        0      699 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/ml/mlflow/__init__.py
+-rw-r--r--   0        0        0     5319 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/ml/mlflow/_client.py
+-rw-r--r--   0        0        0     4012 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/ml/mlflow/_functions.py
+-rw-r--r--   0        0        0      674 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/process_communication/__init__.py
+-rw-r--r--   0        0        0     3362 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/process_communication/_models.py
+-rw-r--r--   0        0        0      732 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/schema_management/README.md
+-rw-r--r--   0        0        0      598 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/schema_management/__init__.py
+-rw-r--r--   0        0        0     1219 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/schema_management/schema_entity.py
+-rw-r--r--   0        0        0      598 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/security/__init__.py
+-rw-r--r--   0        0        0     2140 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/security/clients/README.md
+-rw-r--r--   0        0        0     1450 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/security/clients/__init__.py
+-rw-r--r--   0        0        0     8358 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/security/clients/_azure_client.py
+-rw-r--r--   0        0        0     2396 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/security/clients/_base.py
+-rw-r--r--   0        0        0     1787 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/security/clients/_local_client.py
+-rw-r--r--   0        0        0      598 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/security/clients/hashicorp_vault/__init__.py
+-rw-r--r--   0        0        0     2695 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
+-rw-r--r--   0        0        0     2601 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/security/clients/hashicorp_vault/kubernetes_client.py
+-rw-r--r--   0        0        0     3454 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/security/clients/hashicorp_vault/oidc_client.py
+-rw-r--r--   0        0        0     1952 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/security/clients/hashicorp_vault/token_client.py
+-rw-r--r--   0        0        0      598 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/__init__.py
+-rw-r--r--   0        0        0     1208 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/blob/README.md
+-rw-r--r--   0        0        0      622 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/blob/__init__.py
+-rw-r--r--   0        0        0     9605 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/blob/azure_storage_client.py
+-rw-r--r--   0        0        0     4791 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/blob/base.py
+-rw-r--r--   0        0        0      665 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/cache/__init__.py
+-rw-r--r--   0        0        0     3451 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/cache/_base.py
+-rw-r--r--   0        0        0     3365 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/cache/redis_cache.py
+-rw-r--r--   0        0        0     2451 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/database/README.md
+-rw-r--r--   0        0        0      598 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/database/__init__.py
+-rw-r--r--   0        0        0     4691 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/database/azure_sql.py
+-rw-r--r--   0        0        0      675 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/database/models/__init__.py
+-rw-r--r--   0        0        0     1447 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/database/models/_models.py
+-rw-r--r--   0        0        0     7711 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/database/odbc.py
+-rw-r--r--   0        0        0     4523 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/database/trino_sql.py
+-rw-r--r--   0        0        0     2386 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/delta_lake/README.md
+-rw-r--r--   0        0        0      721 2023-08-07 14:48:05.685997 adapta-2.3.9/adapta/storage/delta_lake/__init__.py
+-rw-r--r--   0        0        0    11493 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/delta_lake/_functions.py
+-rw-r--r--   0        0        0     2247 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/delta_lake/_models.py
+-rw-r--r--   0        0        0     1695 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/distributed_object_store/datastax_astra/README.md
+-rw-r--r--   0        0        0      622 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/distributed_object_store/datastax_astra/__init__.py
+-rw-r--r--   0        0        0    16970 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/distributed_object_store/datastax_astra/astra_client.py
+-rw-r--r--   0        0        0      598 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/models/__init__.py
+-rw-r--r--   0        0        0     5302 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/models/azure.py
+-rw-r--r--   0        0        0     2063 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/models/base.py
+-rw-r--r--   0        0        0     5711 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/models/format.py
+-rw-r--r--   0        0        0     6630 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/models/hive.py
+-rw-r--r--   0        0        0     1519 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/models/local.py
+-rw-r--r--   0        0        0     1953 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/secrets/README.md
+-rw-r--r--   0        0        0      666 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/secrets/__init__.py
+-rw-r--r--   0        0        0     2216 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/secrets/_base.py
+-rw-r--r--   0        0        0     2358 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/secrets/azure_secret_client.py
+-rw-r--r--   0        0        0     2887 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
+-rw-r--r--   0        0        0     2761 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/utils/README.md
+-rw-r--r--   0        0        0      668 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/utils/__init__.py
+-rw-r--r--   0        0        0     6463 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/utils/_common.py
+-rw-r--r--   0        0        0     3930 2023-08-07 14:48:05.689998 adapta-2.3.9/adapta/utils/concurrent_task_runner.py
+-rw-r--r--   0        0        0     2296 2023-08-07 14:48:30.892814 adapta-2.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 adapta-2.3.9/PKG-INFO
```

### Comparing `adapta-2.3.8/LICENSE` & `adapta-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/README.md` & `adapta-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/__init__.py` & `adapta-2.3.9/adapta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/connectors/__init__.py` & `adapta-2.3.9/adapta/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/connectors/service_bus/__init__.py` & `adapta-2.3.9/adapta/connectors/service_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/connectors/service_bus/_connector.py` & `adapta-2.3.9/adapta/connectors/service_bus/_connector.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/logs/README.md` & `adapta-2.3.9/adapta/logs/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/logs/__init__.py` & `adapta-2.3.9/adapta/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/logs/_base.py` & `adapta-2.3.9/adapta/logs/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/logs/_internal.py` & `adapta-2.3.9/adapta/logs/_internal.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/logs/handlers/__init__.py` & `adapta-2.3.9/adapta/logs/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/logs/handlers/datadog_api_handler.py` & `adapta-2.3.9/adapta/logs/handlers/datadog_api_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/logs/handlers/safe_stream_handler.py` & `adapta-2.3.9/adapta/logs/handlers/safe_stream_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/logs/models/__init__.py` & `adapta-2.3.9/adapta/logs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/logs/models/_log_level.py` & `adapta-2.3.9/adapta/logs/models/_log_level.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/logs/models/_logs_metadata.py` & `adapta-2.3.9/adapta/logs/models/_logs_metadata.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/metrics/__init__.py` & `adapta-2.3.9/adapta/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/metrics/_base.py` & `adapta-2.3.9/adapta/metrics/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/metrics/providers/README.md` & `adapta-2.3.9/adapta/metrics/providers/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/metrics/providers/__init__.py` & `adapta-2.3.9/adapta/metrics/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/metrics/providers/datadog_provider.py` & `adapta-2.3.9/adapta/metrics/providers/datadog_provider.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/ml/__init__.py` & `adapta-2.3.9/adapta/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/ml/_model.py` & `adapta-2.3.9/adapta/ml/_model.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/ml/mlflow/__init__.py` & `adapta-2.3.9/adapta/ml/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/ml/mlflow/_client.py` & `adapta-2.3.9/adapta/ml/mlflow/_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/ml/mlflow/_functions.py` & `adapta-2.3.9/adapta/ml/mlflow/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/process_communication/__init__.py` & `adapta-2.3.9/adapta/process_communication/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/process_communication/_models.py` & `adapta-2.3.9/adapta/process_communication/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/schema_management/README.md` & `adapta-2.3.9/adapta/schema_management/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/schema_management/__init__.py` & `adapta-2.3.9/adapta/schema_management/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/schema_management/schema_entity.py` & `adapta-2.3.9/adapta/schema_management/schema_entity.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/security/__init__.py` & `adapta-2.3.9/adapta/security/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/security/clients/README.md` & `adapta-2.3.9/adapta/security/clients/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/security/clients/__init__.py` & `adapta-2.3.9/adapta/security/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/security/clients/_azure_client.py` & `adapta-2.3.9/adapta/security/clients/_azure_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/security/clients/_base.py` & `adapta-2.3.9/adapta/security/clients/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/security/clients/_local_client.py` & `adapta-2.3.9/adapta/security/clients/_local_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/security/clients/hashicorp_vault/__init__.py` & `adapta-2.3.9/adapta/security/clients/hashicorp_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py` & `adapta-2.3.9/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/security/clients/hashicorp_vault/kubernetes_client.py` & `adapta-2.3.9/adapta/security/clients/hashicorp_vault/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/security/clients/hashicorp_vault/oidc_client.py` & `adapta-2.3.9/adapta/security/clients/hashicorp_vault/oidc_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/security/clients/hashicorp_vault/token_client.py` & `adapta-2.3.9/adapta/security/clients/hashicorp_vault/token_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/__init__.py` & `adapta-2.3.9/adapta/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/blob/README.md` & `adapta-2.3.9/adapta/storage/blob/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/blob/__init__.py` & `adapta-2.3.9/adapta/storage/blob/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/blob/azure_storage_client.py` & `adapta-2.3.9/adapta/storage/blob/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/blob/base.py` & `adapta-2.3.9/adapta/storage/blob/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/cache/__init__.py` & `adapta-2.3.9/adapta/storage/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/cache/_base.py` & `adapta-2.3.9/adapta/storage/cache/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/cache/redis_cache.py` & `adapta-2.3.9/adapta/storage/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/database/README.md` & `adapta-2.3.9/adapta/storage/database/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/database/__init__.py` & `adapta-2.3.9/adapta/storage/database/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/database/azure_sql.py` & `adapta-2.3.9/adapta/storage/database/azure_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/database/models/__init__.py` & `adapta-2.3.9/adapta/storage/database/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/database/models/_models.py` & `adapta-2.3.9/adapta/storage/database/models/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/database/odbc.py` & `adapta-2.3.9/adapta/storage/database/odbc.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/database/trino_sql.py` & `adapta-2.3.9/adapta/storage/database/trino_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/delta_lake/README.md` & `adapta-2.3.9/adapta/storage/delta_lake/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/delta_lake/__init__.py` & `adapta-2.3.9/adapta/storage/delta_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/delta_lake/_functions.py` & `adapta-2.3.9/adapta/storage/delta_lake/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/delta_lake/_models.py` & `adapta-2.3.9/adapta/storage/delta_lake/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/distributed_object_store/datastax_astra/README.md` & `adapta-2.3.9/adapta/storage/distributed_object_store/datastax_astra/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/distributed_object_store/datastax_astra/__init__.py` & `adapta-2.3.9/adapta/storage/distributed_object_store/datastax_astra/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/distributed_object_store/datastax_astra/astra_client.py` & `adapta-2.3.9/adapta/storage/distributed_object_store/datastax_astra/astra_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 #
 
 import base64
 import datetime
 import enum
 import os
 import re
-import shutil
 import sys
 import tempfile
 import typing
 import uuid
 from dataclasses import fields, is_dataclass
 from typing import Optional, Dict, TypeVar, Callable, Type, List, Any, get_origin
 
@@ -135,15 +134,15 @@
                 (IPPROTO_TCP, TCP_NODELAY, 1),
                 (IPPROTO_TCP, TCP_USER_TIMEOUT, self._socket_read_timeout),
             ],
         ).connect(self._keyspace)
 
         set_session(self._session)
 
-        shutil.rmtree(self._tmp_bundle_path)
+        os.remove(os.path.join(self._tmp_bundle_path, tmp_bundle_file_name))
 
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._session.shutdown()
         self._session = None
```

### Comparing `adapta-2.3.8/adapta/storage/models/__init__.py` & `adapta-2.3.9/adapta/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/models/azure.py` & `adapta-2.3.9/adapta/storage/models/azure.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/models/base.py` & `adapta-2.3.9/adapta/storage/models/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/models/format.py` & `adapta-2.3.9/adapta/storage/models/format.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/models/hive.py` & `adapta-2.3.9/adapta/storage/models/hive.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/models/local.py` & `adapta-2.3.9/adapta/storage/models/local.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/secrets/README.md` & `adapta-2.3.9/adapta/storage/secrets/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/secrets/__init__.py` & `adapta-2.3.9/adapta/storage/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/secrets/_base.py` & `adapta-2.3.9/adapta/storage/secrets/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/secrets/azure_secret_client.py` & `adapta-2.3.9/adapta/storage/secrets/azure_secret_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py` & `adapta-2.3.9/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/utils/README.md` & `adapta-2.3.9/adapta/utils/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/utils/__init__.py` & `adapta-2.3.9/adapta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/utils/_common.py` & `adapta-2.3.9/adapta/utils/_common.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/adapta/utils/concurrent_task_runner.py` & `adapta-2.3.9/adapta/utils/concurrent_task_runner.py`

 * *Files identical despite different names*

### Comparing `adapta-2.3.8/pyproject.toml` & `adapta-2.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adapta"
-version = "2.3.8"
+version = "2.3.9"
 description = "Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier."
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'Apache 2.0'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/adapta'
```

### Comparing `adapta-2.3.8/PKG-INFO` & `adapta-2.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapta
-Version: 2.3.8
+Version: 2.3.9
 Summary: Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier.
 Home-page: https://github.com/SneaksAndData/adapta
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

