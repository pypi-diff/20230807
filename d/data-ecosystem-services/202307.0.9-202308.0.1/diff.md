# Comparing `tmp/data_ecosystem_services-202307.0.9.tar.gz` & `tmp/data_ecosystem_services-202308.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_services-202307.0.9.tar", max compression
+gzip compressed data, was "data_ecosystem_services-202308.0.1.tar", max compression
```

## Comparing `data_ecosystem_services-202307.0.9.tar` & `data_ecosystem_services-202308.0.1.tar`

### file list

```diff
@@ -1,64 +1,82 @@
--rw-r--r--   0        0        0      918 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/__main__.py
--rw-r--r--   0        0        0     1264 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/__init__.py
--rw-r--r--   0        0        0     5030 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/column.py
--rw-r--r--   0        0        0    25117 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/customfieldsendpoint.py
--rw-r--r--   0        0        0    13816 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/datasource.py
--rw-r--r--   0        0        0     2037 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/endpoint.py
--rw-r--r--   0        0        0    13626 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/excelmetadata.py
--rw-r--r--   0        0        0      566 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/execution_session.py
--rw-r--r--   0        0        0     7568 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/idfinderendpoint.py
--rw-r--r--   0        0        0    16676 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/manifest.py
--rw-r--r--   0        0        0    10973 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/query.py
--rw-r--r--   0        0        0    55259 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/schema.py
--rw-r--r--   0        0        0     7368 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/table.py
--rw-r--r--   0        0        0     1486 2023-07-25 19:41:14.054138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/tagsendpoint.py
--rw-r--r--   0        0        0    25982 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/tokenendpoint.py
--rw-r--r--   0        0        0     1044 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_client_service/__init__.py
--rw-r--r--   0        0        0       41 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_client_service/az_client.py
--rw-r--r--   0        0        0     4570 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_client_service/azd_client.py
--rw-r--r--   0        0        0     1050 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_key_vault_service/__init__.py
--rw-r--r--   0        0        0     8967 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_key_vault_service/az_key_vault.py
--rw-r--r--   0        0        0     1073 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_storage_service/__init__.py
--rw-r--r--   0        0        0     2665 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/az_storage_service/az_storage_queue.py
--rw-r--r--   0        0        0     1024 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/__init__.py
--rw-r--r--   0        0        0    15940 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/environment_logging.py
--rw-r--r--   0        0        0     8398 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/environment_tracing.py
--rw-r--r--   0        0        0     1013 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_security_service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_security_service/security_base64.py
--rw-r--r--   0        0        0    21410 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_security_service/security_core.py
--rw-r--r--   0        0        0     1175 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/__init__.py
--rw-r--r--   0        0        0    42751 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/dataset_metadata.py
--rw-r--r--   0        0        0    40188 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/environment_metadata.py
--rw-r--r--   0        0        0    36068 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/job_metadata.py
--rw-r--r--   0        0        0     2254 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/logging_metadata.py
--rw-r--r--   0        0        0    22352 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/pipeline_metadata.py
--rw-r--r--   0        0        0     1727 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/__init__.py
--rw-r--r--   0        0        0    33787 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py
--rw-r--r--   0        0        0     8962 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py
--rw-r--r--   0        0        0    25880 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py
--rw-r--r--   0        0        0     3825 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py
--rw-r--r--   0        0        0     3949 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_core.py
--rw-r--r--   0        0        0    50039 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_file.py
--rw-r--r--   0        0        0     5323 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_http.py
--rw-r--r--   0        0        0     4903 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py
--rw-r--r--   0        0        0     4648 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/job_core.py
--rw-r--r--   0        0        0    17832 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/repo_core.py
--rw-r--r--   0        0        0     8956 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/directory_paths.txt
--rw-r--r--   0        0        0      827 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/github_service/__init__.py
--rw-r--r--   0        0        0     7250 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/github_service/github_secret.py
--rw-r--r--   0        0        0     1707 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/jira_service/__init__.py
--rw-r--r--   0        0        0     6295 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/jira_service/jira_client.py
--rw-r--r--   0        0        0       44 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/output.txt
--rw-r--r--   0        0        0      869 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/posit_service/__init__.py
--rw-r--r--   0        0        0    21050 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/posit_service/posit_connect.py
--rw-r--r--   0        0        0      825 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/python_service/__init__.py
--rw-r--r--   0        0        0       24 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/python_service/python_client.py
--rw-r--r--   0        0        0    15021 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/requirements.txt
--rw-r--r--   0        0        0      832 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/windows_service/__init__.py
--rw-r--r--   0        0        0     2499 2023-07-25 19:41:14.058138 data_ecosystem_services-202307.0.9/data_ecosystem_services/windows_service/windows_credential.py
--rw-r--r--   0        0        0    11357 2023-07-25 19:41:14.066138 data_ecosystem_services-202307.0.9/license.md
--rw-r--r--   0        0        0     3915 2023-07-25 19:44:28.350867 data_ecosystem_services-202307.0.9/pyproject.toml
--rw-r--r--   0        0        0    52428 2023-07-25 19:41:14.066138 data_ecosystem_services-202307.0.9/readme.md
--rw-r--r--   0        0        0      129 2023-07-25 19:41:14.066138 data_ecosystem_services-202307.0.9/setup.cfg
--rw-r--r--   0        0        0      127 2023-07-25 19:41:14.066138 data_ecosystem_services-202307.0.9/setup.py
--rw-r--r--   0        0        0    55939 1970-01-01 00:00:00.000000 data_ecosystem_services-202307.0.9/PKG-INFO
+-rw-r--r--   0        0        0      918 2023-08-07 18:16:01.981186 data_ecosystem_services-202308.0.1/data_ecosystem_services/__main__.py
+-rw-r--r--   0        0        0     1279 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/__init__.py
+-rw-r--r--   0        0        0    27128 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/custom_fields.py
+-rw-r--r--   0        0        0    13804 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/datasource.py
+-rw-r--r--   0        0        0     5037 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/db_column.py
+-rw-r--r--   0        0        0    74869 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/db_schema.py
+-rw-r--r--   0        0        0    27760 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/db_table.py
+-rw-r--r--   0        0        0     2037 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/endpoint.py
+-rw-r--r--   0        0        0    30060 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/excel_manifest.py
+-rw-r--r--   0        0        0     1747 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/execution_session.py
+-rw-r--r--   0        0        0     7562 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/id_finder.py
+-rw-r--r--   0        0        0    24317 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/json_manifest.py
+-rw-r--r--   0        0        0    11844 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/query.py
+-rw-r--r--   0        0        0     1486 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/tags.py
+-rw-r--r--   0        0        0    26242 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/token.py
+-rw-r--r--   0        0        0     6249 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/user.py
+-rw-r--r--   0        0        0    62134 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/app.py
+-rw-r--r--   0        0        0    14729 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/app_startup.py
+-rw-r--r--   0        0        0     1044 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/az_client_service/__init__.py
+-rw-r--r--   0        0        0       41 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/az_client_service/az_client.py
+-rw-r--r--   0        0        0     4563 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/az_client_service/azd_client.py
+-rw-r--r--   0        0        0     1050 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/az_key_vault_service/__init__.py
+-rw-r--r--   0        0        0     9208 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/az_key_vault_service/az_key_vault.py
+-rw-r--r--   0        0        0     1073 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/az_storage_service/__init__.py
+-rw-r--r--   0        0        0     2663 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/az_storage_service/az_storage_queue.py
+-rw-r--r--   0        0        0     1024 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_admin_service/__init__.py
+-rw-r--r--   0        0        0    19034 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_admin_service/environment_logging.py
+-rw-r--r--   0        0        0     8745 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_admin_service/environment_tracing.py
+-rw-r--r--   0        0        0     1013 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_security_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_security_service/security_base64.py
+-rw-r--r--   0        0        0    21383 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_security_service/security_core.py
+-rw-r--r--   0        0        0     1175 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/__init__.py
+-rw-r--r--   0        0        0    42751 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/dataset_metadata.py
+-rw-r--r--   0        0        0    40919 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/environment_metadata.py
+-rw-r--r--   0        0        0    36068 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/job_metadata.py
+-rw-r--r--   0        0        0     2254 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/logging_metadata.py
+-rw-r--r--   0        0        0    22352 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/pipeline_metadata.py
+-rw-r--r--   0        0        0     1739 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/__init__.py
+-rw-r--r--   0        0        0    34320 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py
+-rw-r--r--   0        0        0     8962 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py
+-rw-r--r--   0        0        0    25878 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py
+-rw-r--r--   0        0        0     3967 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py
+-rw-r--r--   0        0        0     3949 2023-08-07 18:16:01.985186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/environment_core.py
+-rw-r--r--   0        0        0    50021 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/environment_file.py
+-rw-r--r--   0        0        0     5319 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/environment_http.py
+-rw-r--r--   0        0        0     4915 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py
+-rw-r--r--   0        0        0     4648 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/job_core.py
+-rw-r--r--   0        0        0    17832 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/repo_core.py
+-rw-r--r--   0        0        0      827 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/github_service/__init__.py
+-rw-r--r--   0        0        0     7241 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/github_service/github_secret.py
+-rw-r--r--   0        0        0      948 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/gpt_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/gpt_service/chat_completion.py
+-rw-r--r--   0        0        0     2735 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/gpt_service/text_completion.py
+-rw-r--r--   0        0        0     1707 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/jira_service/__init__.py
+-rw-r--r--   0        0        0     6290 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/jira_service/jira_client.py
+-rw-r--r--   0        0        0      869 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/posit_service/__init__.py
+-rw-r--r--   0        0        0    21018 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/posit_service/posit_connect.py
+-rw-r--r--   0        0        0      825 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/python_service/__init__.py
+-rw-r--r--   0        0        0       24 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/python_service/python_client.py
+-rw-r--r--   0        0        0    18336 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/requirements.txt
+-rw-r--r--   0        0        0     7134 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/templates/download.html
+-rw-r--r--   0        0        0     7133 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/templates/download_json.html
+-rw-r--r--   0        0        0      459 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/templates/error.html
+-rw-r--r--   0        0        0     2723 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/templates/log_file.html
+-rw-r--r--   0        0        0     5231 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/templates/upload.html
+-rw-r--r--   0        0        0     2488 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/templates/upload_json.html
+-rw-r--r--   0        0        0      832 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/windows_service/__init__.py
+-rw-r--r--   0        0        0     2496 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/data_ecosystem_services/windows_service/windows_credential.py
+-rw-r--r--   0        0        0     1692 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/dev_posit_manifests/manifest.json
+-rw-r--r--   0        0        0    59440 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/dev_schema/excel-manifest-schema.xlsx
+-rw-r--r--   0        0        0    24571 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/dev_schema/excel_manifest_schema_for_schemas_sql.xlsx
+-rw-r--r--   0        0        0     6901 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/dev_schema/excel_manifest_schema_for_schemas_sql_merged.xlsx
+-rw-r--r--   0        0        0    29986 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/dev_schema/excel_manifest_schema_for_tables_sql.xlsx
+-rw-r--r--   0        0        0    57139 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/dev_schema/excel_manifest_schema_valuesets.xlsx
+-rw-r--r--   0        0        0    14015 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/dev_schema/manifest.schema.json
+-rw-r--r--   0        0        0    11368 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/license.md
+-rw-r--r--   0        0        0     5494 2023-08-07 18:16:01.989186 data_ecosystem_services-202308.0.1/ocio/ocio_pade_dev/config/config.dev.json
+-rw-r--r--   0        0        0     4480 2023-08-07 18:19:13.581982 data_ecosystem_services-202308.0.1/pyproject.toml
+-rw-r--r--   0        0        0    52428 2023-08-07 18:16:01.993186 data_ecosystem_services-202308.0.1/readme.md
+-rw-r--r--   0        0        0      129 2023-08-07 18:16:01.993186 data_ecosystem_services-202308.0.1/setup.cfg
+-rw-r--r--   0        0        0      127 2023-08-07 18:16:01.993186 data_ecosystem_services-202308.0.1/setup.py
+-rw-r--r--   0        0        0    56412 1970-01-01 00:00:00.000000 data_ecosystem_services-202308.0.1/PKG-INFO
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/__main__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/__main__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/az_key_vault_service/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-"""Initialize the alation_service subpackage of data_ecosystem_services package"""
+"""Initialize the az_key_vault_service subpackage of data_ecosystem_services package"""
 # allow absolute import from the root folder
 # whatever its name is.
-# from data_ecosystem_services.az_storage_service import az_storage_queue
+from ..cdc_admin_service import environment_tracing
+from ..cdc_admin_service import environment_logging
 import sys  # don't remove required for error handling
 import os
-from data_ecosystem_services.cdc_admin_service import environment_tracing
-from data_ecosystem_services.cdc_admin_service import environment_logging
-
 
 # Import from sibling directory ..\developer_service
 OS_NAME = os.name
 
 sys.path.append("..")
 if OS_NAME.lower() == "nt":
-    print("windows")
+    print("az_key_vault_service: windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..")))
     sys.path.append(os.path.dirname(
         os.path.abspath(__file__ + "\\..\\..\\..")))
 else:
-    print("non windows")
+    print("az_key_vault_service: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
-__all__ = ["endpoint", "customfieldsendpoint", "tokenendpoint",
-           "manifest", "tagsendpoint", "idfinderendpoint", "datasource", "schema", "column", "table", "excelmetadata"]
+
+__all__ = ["az_client", "azd_client"]
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/column.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/db_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import json
 import jsonschema
 from jsonschema import validate
 import sys
 import os
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
-from data_ecosystem_services.alation_service.manifest import (
-    Manifest
+from data_ecosystem_services.alation_service.json_manifest import (
+    ManifestJson
 )
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/customfieldsendpoint.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/custom_fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
-    environment_http as pade_env_http
+    environment_http as cdc_env_http
 )
 
+
 import requests
 import json
-from .column import Column
-from .table import Table
+from .db_column import Column
+from .db_table import Table
 import os
 import sys
 import re
+import base64
+
 
 # Default request time out
 REQUEST_TIMEOUT = 180
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
@@ -213,32 +216,32 @@
         Returns:
             dict: A dictionary containing the retrieved data.
 
         Raises:
             EdcAlationError: If there is an error during the retrieval process.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_custom_fields"):
             try:
                 params = {"limit": "1000"}
 
                 # Create headers
                 headers = {'Token': edc_alation_api_token,
                            'Accept': 'application/json',
                            'cache-control': "no-cache"
                            }
 
-                obj_http = pade_env_http.EnvironmentHttp()
+                obj_http = cdc_env_http.EnvironmentHttp()
                 metadata_endpoint = '/integration/v2'
                 object_type = 'custom_field'
                 api_url = f"{edc_alation_base_url}{metadata_endpoint}/{object_type}"
                 response_custom = obj_http.get(
                     api_url, headers=headers, timeout=REQUEST_TIMEOUT, params=params)
 
                 response_custom.raise_for_status()
@@ -286,18 +289,18 @@
         Returns:
             dict: A dictionary containing the retrieved data.
 
         Raises:
             EdcAlationError: If there is an error during the retrieval process.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_object_by_key"):
             try:
 
                 # Check if the alation_datasource_id is an integer
@@ -320,15 +323,15 @@
                 headers = {'Token': edc_alation_api_token,
                            'Content-Type': 'application/json',
                            'Accept': 'application/json',
                            'cache-control': "no-cache"
                            }
 
                 params = self.parse_key(full_key)
-                obj_http = pade_env_http.EnvironmentHttp()
+                obj_http = cdc_env_http.EnvironmentHttp()
                 metadata_endpoint = '/integration/v2'
                 api_url = f"{edc_alation_base_url}{metadata_endpoint}/{object_type}"
                 response_custom = obj_http.get(
                     api_url, headers=headers, timeout=REQUEST_TIMEOUT, params=params)
 
                 response_custom.raise_for_status()
 
@@ -383,60 +386,66 @@
         """
 
         if key.startswith("\"") and key.endswith("\""):
             return key  # Key is already wrapped
 
         return f"\"{key}\""  # Wrap the key with double quotes
 
-    def get_data(self, object_to_update):
-        """Get data from an object or its 'get_alation_data' method.
+    def encode_key_with_special_characters(self, key):
+        special_characters = {
+            '!': '%21',
+            '"': '%22',
+            '#': '%23',
+            '$': '%24',
+            '%': '%25',
+            '&': '%26',
+            "'": '%27',
+            '(': '%28',
+            ')': '%29',
+            '*': '%2A',
+            '+': '%2B',
+            ',': '%2C',
+            '-': '%2D',
+            '.': '%2E',
+            '/': '%2F',
+            ':': '%3A',
+            ';': '%3B',
+            '<': '%3C',
+            '=': '%3D',
+            '>': '%3E',
+            '?': '%3F',
+            '@': '%40',
+            '[': '%5B',
+            '\\': '%5C',
+            ']': '%5D',
+            '^': '%5E',
+            '_': '%5F',
+            '`': '%60',
+            '{': '%7B',
+            '}': '%7D',
+            '~': '%7E'
+        }
+
+        for char, escape_sequence in special_characters.items():
+            key = key.replace(char, escape_sequence)
+
+        return key
+
+    def handle_null(self, value):
+        return value if value is not None else "N/A"
+
+    # Recursive function to replace null with empty string
+    def replace_null_with_empty(self, obj):
+        if isinstance(obj, dict):
+            return {k: self.replace_null_with_empty(v) if v is not None else "N/A" for k, v in obj.items()}
+        elif isinstance(obj, list):
+            return [self.replace_null_with_empty(elem) if elem is not None else "N/A" for elem in obj]
+        return obj
 
-        Args:
-            object_to_update: The object from which to retrieve the data.
-
-        Returns:
-            str: JSON representation of the data.
-
-        This function retrieves data from the provided object 'u' by either calling its
-        'get_alation_data' method (if available) or directly using the object itself.
-        The retrieved data is then returned as a JSON string.
-
-        If an exception occurs during the retrieval process, an error message is logged
-        using the logger instance and the exception is re-raised.
-
-        Note: This function relies on the 'logger_singleton' and 'tracer_singleton'
-        instances from the 'pade_env_logging' and 'pade_env_tracing' modules respectively.
-        These instances are assumed to be properly initialized and available within the
-        class where this method is defined.
-        """
-
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
-            NAMESPACE_NAME, SERVICE_NAME)
-        logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
-            NAMESPACE_NAME, SERVICE_NAME)
-        tracer = tracer_singleton.get_tracer()
-
-        with tracer.start_as_current_span("get_data"):
-            try:
-
-                # If the object has a get_alation_data method, use it to get the data
-                if hasattr(object_to_update, 'get_alation_data'):
-                    data = object_to_update.get_alation_data()
-                # Otherwise, just use the object itself
-                else:
-                    data = object_to_update
-                return json.dumps(data)
-            except Exception as ex:
-                error_msg = "Error: %s : %s", ex, str(object_to_update)
-                exc_info = sys.exc_info()
-                logger_singleton.error_with_exception(error_msg, exc_info)
-                raise
-
-    def update(self, edc_alation_api_token, edc_alation_base_url, object_type, alation_datasource_id, key, fields, force_submit):
+    def update(self, edc_alation_api_token, edc_alation_base_url, object_type, alation_datasource_id, key, fields_dict, force_submit, valid_editable_fields):
         """
         Update business metadata on an object in Alation.
 
         Parameters
         ----------
         edc_alation_api_token : str
             The API token for authenticating requests to the Alation API.
@@ -466,76 +475,120 @@
 
         Raises
         ------
         EdcAlationError
             If an error occurs during the update process.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("update"):
             array_of_json = None
             try:
                 batch_size = 50
 
-                processed_fields = {}
-                fields = self.get_alation_data(fields)
+                fields = {}
+
+                # Check if the fields_dict is a Table object
+                # If it is a Table object, then extract the properties (attributes) to a dictionary with key-value pairs
+                if isinstance(fields_dict, Table):
+                    # Extract properties (attributes) to a dictionary with key-value pairs
+                    fields_dict = vars(fields_dict)
+
+                # If it is a Column object, then extract the properties (attributes) to a dictionary with key-value pairs
+                if isinstance(fields_dict, Column):
+                    # Extract properties (attributes) to a dictionary with key-value pairs
+                    fields_dict = vars(fields_dict)
+
+                if isinstance(fields_dict, dict):
+                    fields = fields_dict
+                else:
+                    if object_type == "attribute":
+                        field_name = key.split(".")[-1]
+                        if field_name in valid_editable_fields and field_name != "key":
+                            fields = {field_name: fields_dict}
+                        elif field_name == "key":
+                            fields = {key: fields_dict}
+                        else:
+                            logger.warning(
+                                f"Errors occurred and cannot process object {str(field_name)} of type: {type(fields_dict)} because it is not a valid Column in editable fields {str(valid_editable_fields)}")
+                    else:
+                        raise EdcAlationError(
+                            f"Errors occurred and cannot process object: {key} of type: {type(fields_dict)} because it is not a valid Table, Column or Dictionary: {str(fields_dict)}")
 
                 # Check if the alation_datasource_id is an integer
                 if not isinstance(alation_datasource_id, int):
                     raise EdcAlationError(
                         "alation_datasource_id must be an integer.")
 
-                # If the fields is a dictionary, then it is already processed
-                if isinstance(fields, dict):
-                    processed_fields = {k: v for k, v in fields.items()}
-                else:
-                    raise EdcAlationError(
-                        f"Errors occurred and cannot process object because it is missing get_alation_data: {str(fields)}")
-
                 # Remove the datasource id from the key if it exists to avoid duplicate datasource id
                 key = key.replace(str(alation_datasource_id) + ".", "")
 
-                if object_type == 'schema' and '.' in key:
-                    key = self.wrap_with_quotes(key)
-                    # key = key.replace('.', '%2E')
+                # object_type == 'schema' or
+                # For db schema handle keys that contain special characters
+                # if (object_type == 'table') and '.' in full_key:
+                #    full_key = self.wrap_with_quotes(full_key)
 
                 # Add the datasource id to the key
                 full_key = f"{alation_datasource_id}.{key}"
 
                 # Check if the key contains special characters
                 if self.has_special_chars(full_key):
                     logger.warning(
                         f"The following submitted key contains special characters: {str(full_key)}")
 
-                # Remove the key from the fields if it exists to avoid duplicate key
-                if 'key' in processed_fields:
-                    processed_fields.pop('key')
+                # Create a new dictionary with only the valid editable fields
+                #  key.split(".")[-1] is field_name
+                fields_to_process = {key: value for key, value in fields.items()
+                                     if key.split(".")[-1] in valid_editable_fields}
+
+                # If the fields is a dictionary, then it is ready to queue for processing
+                if not isinstance(fields_to_process, dict):
+                    error_msg = f"Errors occurred and cannot process object: {key} of type: {type(fields_dict)} because it is missing fields: {str(fields_dict)}"
+                    raise EdcAlationError(error_msg)
 
                 params = {
                     "create_new": "false",
                     "replace_values": "true"
                 }
 
+                # Loop through the dictionary and urlencode the values
+                for key, value in fields_to_process.items():
+                    # Encode keys if columns/attributes
+                    if key == "key":
+                        if object_type == "attribute":
+                            fields_to_process[key] = self.encode_key_with_special_characters(
+                                value)
+                    # Default to empty string if value is None
+                    if value is None:
+                        value = "N/A"
+
                 # Add the key to the fields
-                single_update = {"key": full_key, **processed_fields}
-                logger.info(f"single_update: {single_update}")
-                self.updates.append(single_update)
+                single_update_init = {"key": full_key, **fields_to_process}
+                logger.info(f"single_update_init: {single_update_init}")
+
+                # Replace null values with empty strings
+                single_update = self.replace_null_with_empty(
+                    single_update_init)
+
+                # Add the update to the updates list
+                # If there is a value to set in addition to key
+                if len(single_update) > 1:
+                    self.updates.append(single_update)
 
                 # Submit the updates if the batch size is reached or if force_submit is True
                 if len(self.updates) >= batch_size or force_submit:
-                    # Create the request body with array if needed
                     data = ""
                     array_of_json = [json.dumps(
-                        u, separators=(',', ':')) for u in self.updates]
+                        u, default=self.handle_null, separators=(',', ':')) for u in self.updates]
                     if len(array_of_json) > 1:
                         data = ",".join(array_of_json)
                         data = "[" + data + "]"
                     else:
                         data = array_of_json[0]
 
                     # Validate json
@@ -545,18 +598,15 @@
                         logger.info(
                             f"Successfully parsed data_json: {len(data_json)}")
                     except json.JSONDecodeError as ex:
                         error_msg = f"Error parsing data_json: {ex} : {data}"
                         logger.error(error_msg)
                         raise
 
-                    # data = json.dumps(data_json, separators=(',', ':'))
-                    # =data = "\n".join(json.dumps(item, separators=(',', ':'))
-                    #                 for item in self.updates)
-                    data_str = '\n'.join(json.dumps(item)
+                    data_str = '\n'.join(json.dumps(item, default=self.handle_null, )
                                          for item in self.updates)
 
                     # submit the batch
                     logger.info(
                         f"Submitting {object_type} batch")
                     metadata_endpoint = '/api/v1/bulk_metadata/custom_fields/default'
                     api_url = f"{edc_alation_base_url}{metadata_endpoint}/{object_type}"
@@ -598,11 +648,11 @@
                             f"Errors occurred: {error_message}: api_url {api_url} : data {data}")
 
                     return {"status": "success", "message": "Batch complete"}, response_json
                 else:
                     return {"status": "success", "message": "Batch not submitted"}, {"number_of_updates", len(self.updates), "batch_size", batch_size, "force_submit", force_submit}
 
             except Exception as ex:
-                error_msg = f"Error: {str(ex)} : {str(key)}: {str(fields)}"
+                error_msg = f"Error: {str(ex)} : {str(key)}: {str(fields_dict)}"
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/datasource.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/datasource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import sys
 import json
 import requests
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
-    environment_http as pade_env_http
+    environment_http as cdc_env_http
 )
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 # Default request timout
@@ -24,18 +24,18 @@
     """
     A base class for interacting with Alation DataSource. 
     """
 
     @staticmethod
     def get_datasource(edc_alation_api_token, edc_alation_base_url, datasource_id):
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_datasource"):
 
             try:
 
@@ -48,15 +48,15 @@
                 # Intentionally not set
                 response_datasource_text = "not_set"
 
                 # Log Parameters
                 logger.info(f"api_url: {api_url}")
 
                 # Make the API request
-                obj_http = pade_env_http.EnvironmentHttp()
+                obj_http = cdc_env_http.EnvironmentHttp()
                 response_datasource = obj_http.get(
                     api_url, headers=headers, timeout=REQUEST_TIMEOUT, params=None)
 
                 # Raise an exception if the response status code is not 200 or 201
                 response_datasource.raise_for_status()
 
                 # Check the response status code to determine if successful
@@ -115,18 +115,18 @@
         Raises:
             Exception: If there is an error in the API request, such as invalid authentication, an exception will be raised.
 
         Note:
             This function is designed to interact with the Alation API. Please ensure that all necessary access permissions and API credentials are correctly set up before using this function.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("check_datasource"):
             try:
 
                 # Must use v1 of the API - v2 returns a 404
@@ -165,18 +165,18 @@
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
     @staticmethod
     def update_datasource(edc_alation_api_token, edc_alation_base_url, alation_datasource_id, datasource_title, datasource_description):
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("update_datasource"):
 
             try:
 
@@ -260,18 +260,18 @@
             Exception: If there is an error in the API request, such as invalid authentication, an exception will be raised.
 
         Note:
             This function is designed to interact with the Alation API. Please ensure that all necessary access permissions and API credentials are correctly set up before using this function.
             This function uses a limit of 100 and a skip of 0 for pagination with the Alation API.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_datasource_schemas"):
             try:
                 ds_id = alation_datasource_id
                 # Create a connection to Alation
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/endpoint.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/endpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/idfinderendpoint.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/id_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 import sys
 import os
 import re
 
 from .endpoint import Endpoint
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
-    environment_http as pade_env_http
+    environment_http as cdc_env_http
 )
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 REQUEST_TIMEOUT = 45
@@ -159,32 +159,32 @@
 
         Returns
         -------
         int or None
             If the call finds a single object, it will return the ID for the object. If it can't find anything or if it finds more than one object, it will return None.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("find"):
 
             api_url = ""
             try:
                 # Create headers
                 headers = {'Token': self.token,
                            'Accept': 'application/json'}
                 params = self.parse_key(key)
                 metadata_endpoint = '/integration/v2'
                 base_url = self.base_url
                 api_url = f"{base_url}{metadata_endpoint}/{object_type}"
-                obj_http = pade_env_http.EnvironmentHttp()
+                obj_http = cdc_env_http.EnvironmentHttp()
                 response = obj_http.get(
                     api_url, headers=headers, timeout=REQUEST_TIMEOUT, params=params)
                 response.raise_for_status()
                 response_json = response.json()
                 if len(response_json) == 1:
                     return response_json[0]['id']
                 else:
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/manifest.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/json_manifest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,127 @@
+"""
+This module provides a class called ManifestJson, which is used to handle a manifest JSON file and perform operations on its data.
+
+Module Contents:
+- ManifestJson: A class representing a manifest JSON file and containing methods for data manipulation and validation.
+
+This module also imports and uses the following external modules:
+- jsonschema: A Python library to validate JSON data against a JSON Schema.
+- json: The built-in JSON module in Python for JSON data manipulation.
+- sys: The built-in sys module for system-specific functions and parameters.
+- os: The built-in os module for operating system-related functions.
+
+This module also imports the following class objects from the 'data_ecosystem_services.cdc_admin_service' module:
+- environment_tracing: A class to handle environment tracing configuration.
+- environment_logging: A class to handle environment logging configuration.
+
+Important Note:
+- The ManifestJson class is designed to work with the specific structure of a manifest JSON file defined by a JSON schema.
+- The schema_file_path should point to a JSON schema file used for validation.
+- The 'Table' class from the 'data_ecosystem_services.alation_service.table' module is used for representing tables in the 'ManifestJson' class.
+"""
+
+import sys
+import os
 import json
 import jsonschema
 from jsonschema import validate
-import sys
-import os
+
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
+SUBMITTING_USER = 'TODO: Get submitting user from Alation'
+
 
+class ManifestJson:
+    """
+    Represents a ManifestJson object with data extracted from a manifest JSON file and a schema file.
+
+    The `ManifestJson` class provides methods to initialize the object with the schema file path, set Alation data,
+    retrieve tables and columns data, validate JSON data against a given schema, and more.
+
+    Attributes:
+        schema_file_path (str): The path to the schema JSON file.
+        title (str): The title extracted from the manifest JSON.
+        alationDatasourceID (str): The Alation datasource ID extracted from the manifest JSON.
+        alationSchemaID (str): The Alation schema ID extracted from the manifest JSON.
+        submitting_user (str): The submitting user associated with the manifest.
+        description (str): The description extracted from the manifest JSON.
+        releasedate (str): The release date extracted from the manifest JSON.
+        homepageUrl (str): The homepage URL extracted from the manifest JSON.
+        identifier (str): The identifier extracted from the manifest JSON.
+        dataformat (str): The data format extracted from the manifest JSON.
+        language (str): The language extracted from the manifest JSON.
+        size (str): The size extracted from the manifest JSON.
+        updateFrequency (str): The update frequency extracted from the manifest JSON.
+        temporalResolution (str): The temporal resolution extracted from the manifest JSON.
+        license (str): The license extracted from the manifest JSON.
+        tags (list): The list of tags extracted from the manifest JSON.
+        geographicCoverage (str): The geographic coverage extracted from the manifest JSON.
+        referencedBy (str): The reference information extracted from the manifest JSON.
+        references (str): The references extracted from the manifest JSON.
+        citation (str): The citation extracted from the manifest JSON.
+        reference (str): The reference extracted from the manifest JSON.
+        temporalApplicability (dict): The temporal applicability extracted from the manifest JSON.
+        tables (dict): A dictionary mapping table names to their respective table objects.
+        pii (dict): The personally identifiable information extracted from the manifest JSON.
+        manifest_template_properties (dict): The manifest template properties extracted from the schema JSON.
+        extra_description_fields (dict): Additional description fields extracted from the manifest JSON.
+
+    Methods:
+        __init__(self, schema_file_path): Initializes a ManifestJson object with the provided schema_file_path.
+        set_alation_data(self, manifest_json): Sets Alation data using the provided manifest and schema_file_path.
+        get_tables_data(self): Retrieves the tables data from the current instance.
+        get_columns_data(self): Retrieves the columns data for each table in the current instance.
+        format_description(self): Formats the description to include any additional description fields.
+        get_schema_data(self): Retrieves Alation schema data from the ManifestJson object.
+        validate_json(self, json_data, schema): Validates JSON data against a given schema.
+        print_manifest(manifest_object): Print the key-value pairs of a dictionary in a user-friendly format.
+        get_submitting_user_from_manifest_file(self, manifest_file_path): Retrieves the submitting user from a manifest JSON file.
+        validate_manifest(self, manifest_file, schema_file_path): Validates a manifest JSON file against a JSON schema.
+        get_manifest_expected_fields(self): Reads the manifest JSON file and extracts expected fields for schema, table, and column objects.
+
+    """
 
-class Manifest:
     def __init__(self, schema_file_path):
         """
-        Initializes a Manifest object with the provided schema_file_path.
+        Initializes a ManifestJson object with the provided schema_file_path.
 
         Args:
             schema_file_path (str): The path to the schema JSON file.
 
         Raises:
             Exception: If an error occurs during initialization.
 
         """
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("__init__"):
             try:
+                logger.info("Start Field by field:")
                 self.schema_file_path = schema_file_path
                 self.title = ''
                 self.alationDatasourceID = ''
                 self.alationSchemaID = ''
-                self.submitting_user = ''
+                self.submitting_user = SUBMITTING_USER
                 self.description = ''
-                # self.releasedate = ''
+                self.releasedate = ''
                 self.homepageUrl = ''
                 self.identifier = ''
                 self.dataformat = ''
                 self.language = ''
                 self.size = ''
                 self.updateFrequency = ''
                 self.temporalResolution = ''
@@ -71,18 +145,18 @@
                 raise
 
     def set_alation_data(self, manifest_json):
         """
         Set Alation data using the provided manifest and schema_file_path.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("set_alation_data"):
 
             try:
                 logger.info("Start Field by field:")
@@ -98,40 +172,45 @@
                 self.extra_description_fields = {}
                 if "extraDescriptionFields" in manifest_json:
                     optional_description_fields = manifest_json['extraDescriptionFields']
                     print("Extra description fields: ",
                           optional_description_fields)
                     for key in optional_description_fields:
                         self.extra_description_fields[key] = optional_description_fields[key]
-                self.title = manifest_json['title']
+                # Required fields
                 self.alationDatasourceID = manifest_json['alationDatasourceID']
                 self.alationSchemaID = manifest_json['alationSchemaID']
-                self.submitting_user = manifest_json['submitting_user']
+                self.identifier = manifest_json['identifier']
+                self.title = manifest_json['title']
                 self.description = manifest_json['description']
                 self.releasedate = manifest_json['releaseDate']
-                self.homepageUrl = manifest_json['homepageUrl']
-                self.identifier = manifest_json['identifier']
+                self.pii = manifest_json['pii']
+                self.tags = manifest_json['tags']
+                self.submitting_user = SUBMITTING_USER
                 # self.dataformat  = manifest['format']
                 # self.language    = manifest['language']
                 # self.size        = manifest['size']
                 # self.temporalResolution = manifest['temporalResolution']
                 # self.updateFrequency    = manifest['updateFrequency']
                 # self.conformToStandard  = manifest['conformToStandard']
-                self.license = manifest_json['license']
-                self.tags = manifest_json['tags']
-                self.referencedBy = manifest_json['referencedBy']
-                self.citation = manifest_json['citation']
-                self.reference = manifest_json['reference']
-                self.geographicCoverage = manifest_json['geographicCoverage']
+                # Non Required fields : Default Blank
                 # self.tables = list(map(lambda t: Table(t), manifest['tables']))
-                from data_ecosystem_services.alation_service.table import Table
+                self.homepageUrl = manifest_json.get('homepageUrl', '')
+                self.license = manifest_json.get('license', '')
+                self.referencedBy = manifest_json.get('referencedBy', '')
+                self.citation = manifest_json.get('citation', '')
+                self.reference = manifest_json.get('reference', '')
+                self.geographicCoverage = manifest_json.get(
+                    'geographicCoverage', '')
+                self.temporalApplicability = manifest_json.get(
+                    'temporalApplicability', '')
+                # import here to avoid reference conflicts
+                from data_ecosystem_services.alation_service.db_table import Table
                 self.tables = {table.name: table for table in map(
                     lambda t: Table(t, self.schema_file_path), manifest_json['tables'])}
-                self.pii = manifest_json['pii']
-                self.temporalApplicability = manifest_json['temporalApplicability']
 
                 return 200, "Success"
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
@@ -146,15 +225,15 @@
         Example:
             >>> instance = MyClass()
             >>> tables_data = instance.get_tables_data()
             >>> print(tables_data)
             {'table1': [...], 'table2': [...], ...}
         """
 
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_tables_data"):
 
             return self.tables
 
@@ -168,56 +247,57 @@
         Example:
             >>> instance = MyClass()
             >>> columns_data = instance.get_columns_data()
             >>> print(columns_data)
             {'table1': ['column1', 'column2', ...], 'table2': ['column3', 'column4', ...], ...}
         """
 
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_columns_data"):
 
             columndata = {}
-            for t in self.tables:
-                columndata[t] = t.columns
+            for table_data in self.tables:
+                columndata[table_data] = table_data.columns
             return columndata
 
     def format_description(self):
         description = self.description
         if self.extra_description_fields:
             description += '<br><table><tr><th>Field</th><th>Value</th></tr>'
             for key in self.extra_description_fields:
                 description += '<tr><td>' + key + '</td><td>' + \
                     self.extra_description_fields[key] + '</td></tr>'
             description += '</table>'
         return description
 
     def get_schema_data(self):
         """
-        Retrieves Alation schema data from the Manifest object.
+        Retrieves Alation schema data from the ManifestJson object.
 
         Returns:
-            dict: A dictionary containing Alation schema data extracted from the Manifest.
+            dict: A dictionary containing Alation schema data extracted from the ManifestJson.
 
         Raises:
             Exception: If an error occurs while retrieving the Alation data.
 
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_schema_data"):
             try:
                 data = {}
+                data["submitting_user"] = SUBMITTING_USER
                 data['title'] = self.title
                 data['description'] = self.format_description()
                 # data['Release Date']    = self.releasedate
                 data['Homepage URL'] = self.homepageUrl
                 data['Identifier'] = self.identifier
                 # data['Format']          = self.dataformat
                 data['License'] = self.license
@@ -232,125 +312,165 @@
                 return data
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
-    def validate_json(self, jsonData, schema):
+    def validate_json(self, json_data, schema):
         """
         Validates JSON data against a given schema.
 
         Args:
-            jsonData (dict): The JSON data to be validated.
+            json_data (dict): The JSON data to be validated.
             schema (dict): The JSON schema to validate against.
 
         Returns:
             bool: True if the JSON data is valid according to the schema.
 
         Raises:
             jsonschema.exceptions.ValidationError: If the JSON data fails validation against the schema.
             Exception: If an error occurs during validation.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("validate_json"):
 
             try:
-                validate(instance=jsonData, schema=schema)
+                validate(instance=json_data, schema=schema)
+                logger.info("Validation complete")
             except jsonschema.exceptions.ValidationError as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
             return True
 
     @staticmethod
     def print_manifest(manifest_object):
-        for k, v, in manifest_object.items():
-            print("{0}: {1}".format(k, v))
+        """
+        Print the key-value pairs of a dictionary in a user-friendly format.
 
-    def get_submitting_user_from_manifest_file(self, manifest_file):
+        This function takes a dictionary (manifest_object) as input and prints its key-value pairs in a formatted way.
+        Each key-value pair is printed on a separate line, where the key and value are separated by a colon.
+        The keys are printed as strings, and the values are printed using their respective string representations.
+
+        Args:
+            manifest_object (dict): The dictionary to be printed.
+
+        Returns:
+            None: This function does not return anything. It directly prints the key-value pairs.
+
+        Example:
+            >>> my_dict = {'name': 'John', 'age': 30, 'city': 'New York'}
+            >>> print_manifest(my_dict)
+            name: John
+            age: 30
+            city: New York
+        """
+        for item_k, item_v, in manifest_object.items():
+            print("{0}: {1}".format(item_k, item_v))
+
+    def get_submitting_user_from_manifest_file(self, manifest_file_path):
         """
         Retrieves the submitting user from a manifest JSON file.
 
         Args:
-            manifest_file (str): The path to the manifest JSON file.
+            manifest_file_path (str): The path to the manifest JSON file.
 
         Returns:
             str: The submitting user extracted from the manifest.
 
         Raises:
             Exception: If an error occurs while retrieving the submitting user.
 
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_submitting_user_from_manifest_file"):
-
             try:
-                schema_file_path = open(self.schema_file_path)
-                schema = json.load(schema_file_path)
-                f = open(manifest_file, encoding='utf-8')
-                manifest = json.load(f)
-                return manifest['submitting_user']
+                schema_file_path = open(
+                    self.schema_file_path, encoding='utf-8')
+                logger.info(f"schema_file_path: {schema_file_path}")
+                manifest_file = open(manifest_file_path, encoding='utf-8')
+                manifest_file_json = json.load(manifest_file)
+                submitting_user = manifest_file_json.get(
+                    'submitting_user', SUBMITTING_USER)
+                return submitting_user
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
-    def validate_manifest(self, manifest_file):
+    def validate_manifest(self, manifest_file, schema_file_path):
         """
-        Validates a manifest JSON file against a schema.
+        Validates a manifest JSON file against a JSON schema.
+
+        This method validates the provided manifest JSON file against the given JSON schema file.
+        It reads both the manifest and schema files, loads them as JSON data, and then performs validation using the jsonschema library.
 
         Args:
-            manifest_file (str): The path to the manifest JSON file.
+            manifest_file (str): The path to the manifest JSON file for validation.
+            schema_file_path (str): The path to the JSON schema file used for validation.
 
         Returns:
-            tuple: A tuple containing an HTTP status code (200 if successful) and the manifest dictionary.
+            tuple: A tuple containing an HTTP status code (200 if successful) and a success message.
 
         Raises:
-            ValueError: If the manifest schema is invalid.
-            FileNotFoundError: If the specified schema file does not exist.
-            JSONDecodeError: If the schema file or manifest file is not a valid JSON.
+            jsonschema.exceptions.ValidationError: If the manifest JSON data fails validation against the schema.
+            FileNotFoundError: If the specified schema file or manifest file does not exist.
+            json.JSONDecodeError: If the schema file or manifest file contains invalid JSON data.
+
+        Important Note:
+            - The schema_file_path should point to a valid JSON schema file.
+            - The method uses the `jsonschema` library to validate the manifest JSON against the provided schema.
 
+        Example:
+            >>> my_manifest_file = "path/to/my_manifest.json"
+            >>> my_schema_file = "path/to/my_schema.json"
+            >>> manifest_validator = ManifestJson()
+            >>> http_status_code, message = manifest_validator.validate_manifest(my_manifest_file, my_schema_file)
+            >>> print(f"Validation status: {http_status_code}")
+            >>> print(message)
+            Validation status: 200
+            Success
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("validate_manifest"):
 
             try:
-                schema_file_path = open(
-                    self.schema_file_path, 'r', encoding='utf-8')
-                schema_file_path = json.load(
-                    schema_file_path)
-                f = open(manifest_file, 'r', encoding='utf-8')
-                manifest_json = json.load(f)
+                schema_file = open(
+                    schema_file_path, 'r', encoding='utf-8')
+                schema_file_json = json.load(
+                    schema_file)
+                manifest_file = open(manifest_file, 'r', encoding='utf-8')
+                manifest_json = json.load(manifest_file)
 
-                self.validate_json(manifest_json, schema_file_path)
-                logger.info("Manifest schema is valid")
+                self.validate_json(manifest_json, schema_file_json)
+                logger.info("ManifestJson schema is valid")
                 message = self.set_alation_data(manifest_json)
                 return message
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
@@ -364,17 +484,17 @@
 
         Raises:
             FileNotFoundError: If the specified schema file does not exist.
             JSONDecodeError: If the schema file is not a valid JSON.
 
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_manifest_expected_fields"):
             try:
                 schema_file_path = open(
                     self.schema_file_path, encoding="utf-8")
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/query.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,73 +22,74 @@
     os
     sys
     requests
     json
     csv
 
     from data_ecosystem_services.cdc_admin_service import (
-        environment_tracing as pade_env_tracing,
-        environment_logging as pade_env_logging
+        environment_tracing as cdc_env_tracing,
+        environment_logging as cdc_env_logging
     )
 
     from data_ecosystem_services.cdc_tech_environment_service import (
-        environment_http as pade_env_http
+        environment_http as cdc_env_http
     )
 
 Constants:
     NAMESPACE_NAME (str): Name of the currently running file
     SERVICE_NAME (str): Name of the parent folder of the running file
     REQUEST_TIMEOUT (int): Timeout for requests in seconds
     TIMEOUT_ONE_MIN (int): Constant for a timeout of one minute in seconds
 """
 
 import os
 import sys
 import json
 import csv
 import requests
-
+import pandas as pd
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
-    environment_http as pade_env_http
+    environment_http as cdc_env_http
 )
 
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 REQUEST_TIMEOUT = 45
 TIMEOUT_ONE_MIN = 60
+LIMIT = 100  # Set the batch size
 
 
 class Query:
     """
     Query class is used for fetching and processing queries.
 
     ...
 
     Attributes
     ----------
     None
 
     Methods
     -------
-    fetch_query(edc_alation_api_token: str, edc_alation_base_url: str) -> None:
+    get_query_list(edc_alation_api_token: str, edc_alation_base_url: str) -> None:
         Fetches all the queries from an API and processes each query to fetch details, query text, 
         and latest results. This method also handles exceptions, logs different stages of 
         query processing and reports if any error occurs.
     """
 
-    def fetch_query_list(self, edc_alation_api_token, edc_alation_base_url, alation_datasource_id):
+    def get_query_list(self, edc_alation_api_token, edc_alation_base_url, alation_datasource_id):
         """
         Fetches all the queries from an API and processes each query to fetch details, query text, 
         and latest results. This method also handles exceptions, logs different stages of 
         query processing and reports if any error occurs.
 
         Parameters:
         ----------
@@ -107,43 +108,62 @@
         Exception
             If an error occurs during the process of fetching and processing the queries.
         """
 
         headers = {"Token": edc_alation_api_token,
                    "Content-Type": "application/json", "accept": "application/json"}
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
-        with tracer.start_as_current_span("fetch_query_list"):
+        with tracer.start_as_current_span("get_query_list"):
             try:
 
-                logger.info("Get query list")
-                api_url = "/integration/v1/query/"
-                query_list_url = edc_alation_base_url + api_url
-                logger.info(f"query_list_url: {query_list_url}")
-                obj_http = pade_env_http.EnvironmentHttp()
-                params = {"datasource_id": alation_datasource_id}
-                response_list = obj_http.get(query_list_url,
-                                             headers=headers,
-                                             timeout=TIMEOUT_ONE_MIN, params=params)
+                all_queries = []  # Initialize empty list to collect all queries
+                skip = 0  # Start from the first item
+
+                while True:  # We'll break from the loop when we fetch all data
+                    logger.info("Get query list")
+                    api_url = "/integration/v1/query/"
+                    query_list_url = edc_alation_base_url + api_url
+
+                    obj_http = cdc_env_http.EnvironmentHttp()
+                    params = {"datasource_id": alation_datasource_id, "limit": LIMIT,
+                              "skip": skip}
+                    response_list = obj_http.get(query_list_url,
+                                                 headers=headers,
+                                                 timeout=TIMEOUT_ONE_MIN, params=params)
+                    logger.info(f"query_list_url: {query_list_url}")
+                    logger.info(f"query_list_params: {str(params)}")
+                    queries = json.loads(response_list.text)
+                    if not queries:  # If no more queries are returned, break from the loop
+                        break
+
+                    for query in queries:
+                        # Append each query to the all_queries list
+                        all_queries.append(query)
 
-                return response_list
+                    skip += LIMIT
+
+                # Convert the list of queries to a JSON object
+                response_queries_list_json = all_queries
+
+                return response_queries_list_json
 
             except Exception as ex:
                 error_msg = f"Error: {str(ex)}"
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
-    def fetch_query(self, edc_alation_api_token, edc_alation_base_url, alation_datasource_id, query_id):
+    def get_query_results(self, edc_alation_api_token, edc_alation_base_url, alation_datasource_id, query_id):
         """
         Fetches all the queries from an API and processes each query to fetch details, query text, 
         and latest results. This method also handles exceptions, logs different stages of 
         query processing and reports if any error occurs.
 
         Parameters:
         ----------
@@ -163,53 +183,50 @@
             If an error occurs during the process of fetching and processing the queries.
         """
 
         headers = {"Token": edc_alation_api_token,
                    "Content-Type": "application/json",
                    "accept": "application/json"}
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("fetch_query"):
             try:
-                obj_http = pade_env_http.EnvironmentHttp()
-                params = {"datasource_id": alation_datasource_id,
-                          "limit": 1000}
+                obj_http = cdc_env_http.EnvironmentHttp()
                 logger.info("##### Get all queries #####")
                 api_url = "/integration/v1/query/"
-                query_list_url = edc_alation_base_url + api_url
-                logger.info(f"query_list_url: {query_list_url}")
-                response = obj_http.get(query_list_url,
-                                        headers=headers,
-                                        timeout=TIMEOUT_ONE_MIN, params=params)
-                queries = json.loads(response.text)
-                for query in queries:
-                    query_id = str(query["id"])
-                    logger.info(
-                        f"##### Get details for a single query {query_id} #####")
-                    query_detail_url = edc_alation_base_url + api_url + query_id
 
-                    response_detail = obj_http.get(query_detail_url,
-                                                   headers=headers,
-                                                   timeout=TIMEOUT_ONE_MIN, params=None)
-                    query_detail = json.loads(response_detail.text)
-                    detail = query_detail.get("detail")
-                    logger.info(f"query_detail: {query_detail}")
-                    if detail == "You do not have permission to perform this action.":
-                        query_title = "No Permission"
-                        logger.info(f"id: {query_id}, title: {query_title}")
-                    else:
-                        query_id = query_detail["query_id"]
+                # Ensure query_id is a string
+                query_id = str(query_id)
+                logger.info(
+                    f"##### Get details for a single query {query_id} #####")
+                query_detail_url = edc_alation_base_url + api_url + query_id
+
+                response_detail = obj_http.get(query_detail_url,
+                                               headers=headers,
+                                               timeout=TIMEOUT_ONE_MIN, params=None)
+                query_detail = json.loads(response_detail.text)
+                detail = query_detail.get("detail")
+                logger.info(f"query_detail: {query_detail}")
+                query_title = "not_set"
+                if detail == "You do not have permission to perform this action.":
+                    query_title = "No Permission"
+                    logger.info(f"id: {query_id}, title: {query_title}")
+                else:
+                    detail_id = query_detail["id"]
+                    query_title = query_detail["title"]
+                    if query_title is not None:
+                        query_title = query_title.replace("\n", " ")
                         logger.info(
-                            f"query_id: {query_id}, title: {query_title}")
+                            f"detail_id: {detail_id}, title: {query_title}")
 
                 # Get query text
                 api_url = f"/integration/v1/query/{query_id}/sql/"
                 query_text_url = edc_alation_base_url + api_url
                 logger.info(f"query_text_url:{query_text_url}")
                 response_query_text = requests.get(
                     query_text_url, headers=headers, timeout=TIMEOUT_ONE_MIN
@@ -231,42 +248,50 @@
                 query_text = response_content_text
                 query_text = query_text.replace("\n", " ").replace("'", "'")
 
                 # Get latest result id
                 api_url = f"/integration/v1/query/{query_id}/result/latest/"
                 query_url = edc_alation_base_url + api_url
                 logger.info(f"query_url: {query_url}")
-                logger.info(f"headers: {headers}")
+                logger.info(f"headers length: {len(headers)}")
                 # Send the request to the Alation API endpoint.
                 # The endpoint for executing queries is `/integration/v1/query`.
                 response_query = requests.get(query_url,
                                               headers=headers,
                                               timeout=TIMEOUT_ONE_MIN)
                 logger.info(
                     "response_query.content:" +
                     response_query.content.decode("utf-8")
                 )
 
-                # execution_result_id = json_response['id']
-                execution_result_id = "570"
+                json_response = json.loads(response_query.content)
+                execution_result_id = json_response['id']
 
                 # Get lastest results and place in dataframe
                 api_url = f"/integration/v1/result/{execution_result_id}/csv/"
                 result_url = edc_alation_base_url + api_url
 
-                # download and parse response as csv
-                with requests.Session():
-                    response_results = requests.get(
-                        result_url, headers=headers, timeout=TIMEOUT_ONE_MIN
-                    )
-                    decoded_content = response_results.content.decode("utf-8")
-                    logger.info("response_results.content:" + decoded_content)
+                with requests.Session() as s:
+                    response = requests.get(
+                        result_url, headers=headers)
+                    decoded_content = response.content.decode('utf-8')
                     csv_reader = csv.reader(
-                        decoded_content.splitlines(), delimiter=","
-                    )
-                    logger.info.logger.info(list(csv_reader))
+                        decoded_content.splitlines(), delimiter=',')
+
+                    query_data = []
+                    i_record = 0
+                    for row in csv_reader:
+                        if i_record != 0:
+                            query_data.append(row)
+                        else:
+                            columns = row
+                            i_record = i_record + 1
+
+                    df_query_results = pd.DataFrame(query_data)
+                    df_query_results.columns = columns
+                    return df_query_results
 
             except Exception as ex:
                 error_msg = f"Error: {str(ex)}"
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/schema.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/db_schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import requests
 import json
 import os
 import sys
 import concurrent.futures
 import platform
 import datetime
-from .tokenendpoint import TokenEndpoint
-from .customfieldsendpoint import CustomFieldsEndpoint
-from .tagsendpoint import TagsEndpoint
-from .idfinderendpoint import IdFinderEndpoint
+from .token import TokenEndpoint
+from .custom_fields import CustomFieldsEndpoint
+from .tags import TagsEndpoint
+from .id_finder import IdFinderEndpoint
 from .datasource import DataSource
-from .manifest import Manifest
+from .json_manifest import ManifestJson
+from .excel_manifest import ManifestExcel
+from .db_table import Table
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
-    environment_file as pade_env_file,
-    environment_http as pade_env_http
+    environment_file as cdc_env_file,
+    environment_http as cdc_env_http
 )
 
-import data_ecosystem_services.alation_service.excelmetadata as alation_excelmetadata
+import data_ecosystem_services.alation_service.excel_manifest as alation_manifest_excel
+import data_ecosystem_services.alation_service.db_table as alation_table
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 TIMEOUT_ONE_MIN = 60  # or set to whatever value you want
 
@@ -64,18 +67,18 @@
             edc_alation_base_url (str): The base URL of the Alation instance.
             alation_schema_id (int): ID of the Alation schema to retrieve.
 
         Returns:
             dict: A dictionary containing details of the schema.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_schema"):
 
             try:
 
@@ -100,15 +103,15 @@
                 params['limit'] = limit
                 params['skip'] = skip
                 params['id'] = schema_id
                 api_url = f"{edc_alation_base_url}/integration/v2/schema/"
                 logger.info(f"api_url: {api_url}")
                 logger.info(f"params: {str(params)}")
                 # Make the schema request to Alation
-                obj_http = pade_env_http.EnvironmentHttp()
+                obj_http = cdc_env_http.EnvironmentHttp()
                 response_schema = obj_http.get(
                     api_url, headers=headers, params=params, timeout=REQUEST_TIMEOUT)
                 response_schema_json = response_schema.json()
 
                 # Check the response status code to determine if successful
                 if len(response_schema_json) == 1:
                     schema_result = response_schema_json[0]
@@ -142,31 +145,31 @@
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
     @staticmethod
-    def get_schema_tables(edc_alation_api_token, edc_alation_base_url, alation_data_source_id, alation_schema_id):
+    def get_schema_tables(edc_alation_api_token, edc_alation_base_url, alation_datasource_id, alation_schema_id):
         """ 
         Get list of tables for this schema from the provided Alation URL, like: "https://alation_domain/integration/v2/table/?limit=100000&skip=0".
 
         Args:
             edc_alation_api_token (str): Headers to be used in the request, typically including authentication information.
             edc_alation_base_url (str): The base URL of the Alation instance.
-            alation_data_source_id (int): ID of the Alation data source.
+            alation_datasource_id (int): ID of the Alation data source.
             alation_schema_id (int): ID of the Alation schema.
 
         Returns:
             list: List of tables in the schema. Each table is represented as a dictionary.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
         with tracer.start_as_current_span("get_schema_tables"):
 
             try:
 
                 # Set the headers for the request
@@ -177,17 +180,17 @@
                 skip = 0
 
                 # Create a dictionary to hold the parameters
                 params = {}
                 params['limit'] = limit
                 params['skip'] = skip
                 params['schema_id'] = alation_schema_id
-                params['ds_id'] = alation_data_source_id
+                params['ds_id'] = alation_datasource_id
 
-                obj_environment_http = pade_env_http.EnvironmentHttp()
+                obj_environment_http = cdc_env_http.EnvironmentHttp()
                 api_url = f"{edc_alation_base_url}/integration/v2/table/"
                 response = obj_environment_http.get(api_url, headers=headers, params=params,
                                                     timeout=REQUEST_TIMEOUT)
                 # Go through all tables listed for this schema and add to our manifest template
                 response.raise_for_status()  # Raise an exception for 4xx or 5xx status codes
                 tables_dict = {}
                 response_json = response.json()  # Convert to JSON
@@ -230,33 +233,33 @@
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
     @staticmethod
-    def get_table_columns(edc_alation_api_token, edc_alation_base_url, alation_data_source_id, alation_schema_id, alation_table_id):
+    def get_table_columns(edc_alation_api_token, edc_alation_base_url, alation_datasource_id, alation_schema_id, alation_table_id):
         """ 
         Get the list of columns for a specific table in the Alation instance.
 
         Args:
             edc_alation_api_token (str): The API token for authenticating with the Alation instance.
             edc_alation_base_url (str): The base URL of the Alation instance.
             alation_schema_id (int): The ID of the Alation schema.
-            alation_data_source_id (int): The ID of the Alation data source.
+            alation_datasource_id (int): The ID of the Alation data source.
             alation_table_id (int): The ID of the Alation table.
 
         Returns:
             list: The list of columns for the specified table. Each column is represented as a dictionary.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_table_columns"):
 
             column_to_process = {}
 
@@ -270,26 +273,26 @@
                 skip = 0
 
                 # Set the parameters for the API request
                 params = {}
                 params['limit'] = limit
                 params['skip'] = skip
                 params['schema_id'] = alation_schema_id
-                params['ds_id'] = alation_data_source_id
+                params['ds_id'] = alation_datasource_id
                 params['table_id'] = alation_table_id
 
                 # Create the API URL
                 api_url = f"{edc_alation_base_url}/integration/v2/column/"
 
                 # Log Parameters
                 logger.info(f"api_url: {api_url}")
                 logger.info(f"params: {str(params)}")
 
                 # Make the API request
-                obj_http = pade_env_http.EnvironmentHttp()
+                obj_http = cdc_env_http.EnvironmentHttp()
                 response_columns = obj_http.get(
                     api_url, headers=headers, params=params, timeout=REQUEST_TIMEOUT)
 
                 # Go through all tables listed for this schema and add to our manifest template
                 # Convert to Python object
                 response_columns_json = response_columns.json()
 
@@ -301,51 +304,130 @@
             except Exception as ex:
                 error_msg = "Error: %s: %s", ex, str(column_to_process)
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
     @staticmethod
-    def get_manifest_excel_file_name(upload_or_download, repository_path, datasource_title, schema_name, environment, alation_user_id):
+    def get_excel_manifest_file_path_temp(upload_or_download, repository_path, environment, alation_user_id):
+        """
+        Constructs a temporary path for an Excel manifest file based on various parameters and the current date/time.
+
+        Args:
+            upload_or_download (str): Denotes whether the action is an 'upload' or 'download'.
+            repository_path (str): The path to the directory where the Excel manifest file will be stored.
+            environment (str): Specifies the environment under which the file is being managed.
+            alation_user_id (str): Unique identifier of an Alation user.
+
+        Returns:
+            str: The full path to the temporary Excel manifest file.
+
+        Raises:
+            Exception: If an error occurs during the construction of the Excel file path.
+        """
+
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        logger = logger_singleton.get_logger()
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        tracer = tracer_singleton.get_tracer()
+
+        with tracer.start_as_current_span("get_excel_manifest_file_path_temp"):
+            try:
+
+                # Get current time
+                current_date = datetime.datetime.now()
+
+                yyyy_string = current_date.year
+                mm_string = current_date.month
+                dd_string = current_date.day
+                # Format as a 24-hour time string
+                time_str = current_date.strftime("%H_%M_%S")
+
+                datasource_title = "temp"
+                schema_name = "manifest"
+
+                obj_file = cdc_env_file.EnvironmentFile()
+
+                file_name = (
+                    obj_file.scrub_file_name(datasource_title)
+                    + "_"
+                    + obj_file.scrub_file_name(schema_name)
+                    + str(yyyy_string)
+                    + "_"
+                    + str(mm_string)
+                    + "_"
+                    + str(dd_string)
+                    + "_"
+                    + str(time_str)
+                    + "_" + str(alation_user_id) + "_" +
+                    upload_or_download + ".xlsx"
+                )
+
+                right_most_200_chars = file_name[-200:]
+                file_name = right_most_200_chars
+
+                manifest_path = (
+                    repository_path + "/" + environment + "_manifest" +
+                    "_" + upload_or_download + "s" + "/"
+                )
+                manifest_path = obj_file.convert_to_current_os_dir(
+                    manifest_path)
+                logger.info("manifest_path: " + manifest_path)
+
+                manifest_excel_file = manifest_path + file_name
+                logger.info("manifest_excel_file: " + manifest_excel_file)
+
+                return manifest_excel_file
+            except Exception as ex:
+                # Corrected error message formatting
+                error_msg = f"Excel Error: {str(ex)}"
+                exc_info = sys.exc_info()
+                logger_singleton.error_with_exception(error_msg, exc_info)
+                raise
+
+    @staticmethod
+    def get_excel_manifest_file_path(upload_or_download, repository_path, datasource_title, schema_name, environment, alation_user_id):
         """_summary_
 
         Args:
             upload_or_download (_type_): _description_
             yyyy (_type_): _description_
             mm (_type_): _description_
             dd (_type_): _description_
             repository_path (_type_): _description_
             datasource_title (_type_): _description_
             schema_name (_type_): _description_
             environment (_type_): _description_
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
-        with tracer.start_as_current_span("get_manifest_excel_file_name"):
+        with tracer.start_as_current_span("get_excel_manifest_file_path"):
             try:
 
                 # Get current time
                 current_date = datetime.datetime.now()
 
                 yyyy_string = current_date.year
                 mm_string = current_date.month
                 dd_string = current_date.day
                 # Format as a 24-hour time string
                 time_str = current_date.strftime("%H_%M_%S")
 
                 if schema_name == 'object_name_is_missing' or schema_name == 'object name is missing':
                     raise ValueError('Invalid schema_name value.')
 
-                obj_file = pade_env_file.EnvironmentFile()
+                obj_file = cdc_env_file.EnvironmentFile()
 
                 file_name = (
                     obj_file.scrub_file_name(datasource_title)
                     + "_"
                     + obj_file.scrub_file_name(schema_name)
                     + str(yyyy_string)
                     + "_"
@@ -377,33 +459,33 @@
                 # Corrected error message formatting
                 error_msg = f"Excel Error: {str(ex)}"
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
     @staticmethod
-    def get_manifest_json_file_name(upload_or_download, repository_path, datasource_title, schema_name, environment, alation_user_id):
+    def get_json_manifest_file_path(upload_or_download, repository_path, datasource_title, schema_name, environment, alation_user_id):
         """Get the file name for the manifest JSON file.
 
         Args:
             upload_or_download (str): The type of operation, whether "upload" or "download".
             repository_path (str): The path to the repository.
             datasource_title (str): The title of the data source.
             schema_name (str): The name of the schema.
             environment (str): The environment name.
             alation_user_id (str): The ID of the Alation user.
 
         Returns:
             str: The file name for the manifest JSON file.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_manifest_file_name"):
             try:
 
                 # Get current time
@@ -414,15 +496,15 @@
                 dd_string = current_date.day
                 # Format as a 24-hour time string
                 time_str = current_date.strftime("%H_%M_%S")
 
                 if schema_name == 'object_name_is_missing' or schema_name == 'object name is missing':
                     raise ValueError('Invalid schema_name value.')
 
-                obj_file = pade_env_file.EnvironmentFile()
+                obj_file = cdc_env_file.EnvironmentFile()
 
                 manifest_path = (
                     repository_path + "/" + environment + "_manifest" +
                     "_" + upload_or_download + "s" + "/"
                 )
 
                 logger.info("manifest_path: " + manifest_path)
@@ -454,21 +536,144 @@
                 return manifest_file
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
+    @staticmethod
+    def get_json_schema_file_path(repository_path, environment):
+        """
+        Get the file path for the 'manifest.schema.json' file associated with the specified environment.
+
+        This method constructs the file path for the 'manifest.schema.json' file based on the provided
+        repository_path and environment. The file is expected to be located in the schema directory of the specified environment.
+
+        Args:
+            repository_path (str): The path to the repository containing the schema directories.
+            environment (str): The name of the environment to which the schema belongs.
+
+        Returns:
+            str: The file path for the 'manifest.schema.json' file.
+
+        Raises:
+            Exception: If any error occurs during the file path construction.
+
+        Note:
+            This method assumes that the 'manifest.schema.json' file is located within the schema directory
+            of the specified environment.
+
+        Example:
+            repository_path = '/path/to/repository'
+            environment = 'dev'
+            json_schema_file_path = get_json_schema_file_path(repository_path, environment)
+            print(json_schema_file_path)
+            # Output: '/path/to/repository/dev_schema/manifest.schema.json'
+        """
+
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        logger = logger_singleton.get_logger()
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        tracer = tracer_singleton.get_tracer()
+
+        with tracer.start_as_current_span("get_json_schema_file_path"):
+            try:
+                obj_file = cdc_env_file.EnvironmentFile()
+                schema_path = (repository_path + "/" + environment + "_schema")
+                logger.info("schema_path: " + schema_path)
+                file_name = "manifest.schema.json"
+
+                schema_path = obj_file.convert_to_current_os_dir(
+                    schema_path)
+
+                # Join the directory path with the filename
+                json_schema_file_path = os.path.join(schema_path, file_name)
+
+                logger.info(
+                    f"json_schema_file_path: {json_schema_file_path}")
+
+                return json_schema_file_path
+
+            except Exception as ex:
+                error_msg = "Error: %s", ex
+                exc_info = sys.exc_info()
+                logger_singleton.error_with_exception(error_msg, exc_info)
+                raise
+
+    @staticmethod
+    def get_excel_schema_file_path(repository_path, environment):
+        """
+        Get the file path for the 'get_excel_schema_file_path.xlsx' file associated with the specified environment.
+
+        This method constructs the file path for the 'excel_manifest_schema_for_tables_sql.xlsx' file based on the provided
+        repository_path and environment. The file is expected to be located in the schema directory of the specified environment.
+
+        Args:
+            repository_path (str): The path to the repository containing the schema directories.
+            environment (str): The name of the environment to which the schema belongs.
+
+        Returns:
+            str: The file path for the 'excel_manifest_schema_for_tables_sql.xlsx' file.
+
+        Raises:
+            Exception: If any error occurs during the file path construction.
+
+        Note:
+            This method assumes that the 'excel_manifest_schema_for_tables_sql.xlsx' file is located within the schema directory
+            of the specified environment.
+
+        Example:
+            repository_path = '/path/to/repository'
+            environment = 'dev'
+            excel_schema_file_path = get_excel_schema_file_path(repository_path, environment)
+            print(excel_schema_file_path)
+            # Output: '/path/to/repository/dev_schema/excel_manifest_schema_for_tables_sql.xlsx'
+        """
+
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        logger = logger_singleton.get_logger()
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        tracer = tracer_singleton.get_tracer()
+
+        with tracer.start_as_current_span("get_excel_schema_file_path"):
+            try:
+                obj_file = cdc_env_file.EnvironmentFile()
+                schema_path = (repository_path + "/" + environment + "_schema")
+
+                schema_path = obj_file.convert_to_current_os_dir(
+                    schema_path)
+
+                logger.info("schema_path: " + schema_path)
+                schema_xls_file = "excel_manifest_schema_for_tables_sql.xlsx"
+
+                # Join the directory path with the filename
+                excel_schema_file_path = os.path.join(
+                    schema_path, schema_xls_file)
+
+                logger.info(
+                    f"excel_schema_file_path: {excel_schema_file_path}")
+
+                return excel_schema_file_path
+            except Exception as ex:
+                error_msg = "Error: %s", ex
+                exc_info = sys.exc_info()
+                logger_singleton.error_with_exception(error_msg, exc_info)
+                raise
+
     @classmethod
-    def download_schema_manifest_excel_file(cls, alation_schema_id, config):
+    def download_schema_manifest_excel_file(cls, alation_schema_id, config, json_schema_file_path):
         """
         Downloads the schema manifest Excel file for a given Alation schema ID.
 
         This method generates the Excel file data using the `generate_excel_file_data` method of the 
-        `alation_excelmetadata.ExcelMetadata` class, then generates the Excel file using the 
+        `alation_manifest_excel.ManifestExcel` class, then generates the Excel file using the 
         `generate_excel_file_from_data` method of the same class.
 
         Parameters
         ----------
         alation_schema_id : int
             The ID of the Alation schema for which to download the manifest Excel file.
         config : dict
@@ -481,32 +686,45 @@
 
         Raises
         ------
         Exception
             If an error occurs during the operation, an exception is raised and logged.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("download_schema_manifest"):
 
             try:
                 logger.info("alation_schema_id: " + str(alation_schema_id))
 
-                excelmetadata = alation_excelmetadata.ExcelMetadata()
-                df_schema, df_table_list, df_table_raw, df_table_transposed, manifest_excel_file = excelmetadata.generate_excel_file_data(
-                    alation_schema_id, config)
+                table = alation_table.Table(None, json_schema_file_path)
 
-                manifest_excel_file = excelmetadata.generate_excel_file_from_data(
-                    df_schema, df_table_transposed, manifest_excel_file)
+                manifest_excel = alation_manifest_excel.ManifestExcel()
+                df_schema, df_table_list, manifest_excel_file, columns_to_hide = manifest_excel.generate_excel_file_data(
+                    alation_schema_id, config, json_schema_file_path)
+
+                df_status, schema_file = table.get_valueset_for_tables_sql_xlsx(
+                    "Status of Dataset")
+                df_steward, schema_file = table.get_valueset_for_tables_sql_xlsx(
+                    "steward")
+                df_access_level, schema_file = table.get_valueset_for_tables_sql_xlsx(
+                    "access_level")
+                df_language, schema_file = table.get_valueset_for_tables_sql_xlsx(
+                    "language")
+                df_update_frequency, schema_file = table.get_valueset_for_tables_sql_xlsx(
+                    "update_frequency")
+
+                manifest_excel_file = manifest_excel.generate_excel_file_from_data(
+                    columns_to_hide, df_table_list, manifest_excel_file, df_status, df_steward, df_access_level, df_language, df_update_frequency)
 
                 return manifest_excel_file
 
                 # Get the data source title from
             except Exception as ex:
                 error_msg = "Excel Error: %s", ex
                 exc_info = sys.exc_info()
@@ -529,30 +747,29 @@
             to the Alation instance. This might include authentication details and network configurations.
 
         Returns:
             dict: The schema manifest represented as a dictionary. The keys and values in this dictionary 
             represent properties of the schema and their corresponding values as present in the Alation system.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         schema_id = alation_schema_id
         schema_name = None
 
         with tracer.start_as_current_span("download_schema_manifest"):
             try:
 
                 # Get configuration parameteres
                 environment = config.get("environment")
-                schema_file_path = config.get("edc_json_schema_location")
                 edc_alation_base_url = config.get("edc_alation_base_url")
                 repository_path = config.get("repository_path")
                 alation_user_id = config.get("edc_alation_user_id")
 
                 # Log the configuration parameters
                 logger.info(f"edc_alation_base_url: {edc_alation_base_url}")
                 logger.info(f"environment: {environment}")
@@ -581,256 +798,87 @@
 
                 schema_result_json = schema_result.json()
 
                 # Set the schema name, datasource title and datasource_id
                 schema_name = schema_result_json[0].get("name")
                 datasource_title = datasource_result.get("title")
                 datasource_id = datasource_result.get("id")
-                alation_data_source_id = datasource_id
+                alation_datasource_id = datasource_id
 
                 # Log the schema details
                 logger.info(
                     f"schema_result length: {str(len(schema_result_json))}")
                 logger.info(
                     f"datasource_result length: {str(len(datasource_result))}")
 
+                json_schema_file_path = cls.get_json_schema_file_path(
+                    repository_path=repository_path, environment=environment)
                 # Get the schema manifest
-                msg = f"Loading manifest schema from {schema_file_path}"
+                msg = f"Loading manifest schema from {json_schema_file_path}"
                 logger.info(msg)
-                manifest = Manifest(schema_file_path)
+                manifest = ManifestJson(json_schema_file_path)
 
                 # Get the manifest file name
-                manifest_json_file = cls.get_manifest_json_file_name(
+                manifest_json_file = cls.get_json_manifest_file_path(
                     "download", repository_path, datasource_title, schema_name, environment, alation_user_id)
 
                 # Check if the datasource exists
                 datasource = DataSource()
                 datasource.check_datasource(
-                    edc_alation_api_token, edc_alation_base_url, alation_data_source_id, datasource_title
+                    edc_alation_api_token, edc_alation_base_url, alation_datasource_id, datasource_title
                 )
 
                 # Get the schema structure
                 manifest_dict = cls.get_schema_structure(
                     edc_alation_api_token, edc_alation_base_url, manifest, datasource_id, schema_id
                 )
 
                 # Write the file
                 jsonString = json.dumps(manifest_dict, indent=4)
                 jsonFile = open(manifest_json_file, "w", encoding='utf-8')
                 jsonFile.write(jsonString)
                 jsonFile.close()
 
-                msg = "Wrote Manifest template file: " + manifest_json_file
+                msg = "Wrote ManifestJson template file: " + manifest_json_file
                 logger.info(msg)
                 logger.info(
                     f"Validating the manifest file at {manifest_json_file} with schema"
                 )
 
                 # validate the manifest file
                 metadata = manifest.validate_manifest(
-                    manifest_json_file)
+                    manifest_json_file, json_schema_file_path)
                 logger.info("Metadata File Validated")
                 logger_singleton.force_flush()
 
                 return manifest_json_file
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
-    @classmethod
-    def upload_schema_manifest_json_file(cls, metadata_json_data, config):
-        """
-        Uploads a schema manifest to Alation.
-
-        Args:
-            metadata_json_data (dict): Contains metadata information such as the Alation Schema ID.
-            config (dict): Configuration data with the following keys:
-                - edc_alation_base_url (str): The base URL of the Alation instance.
-                - yyyy (str): Year component for manifest file generation.
-                - mm (str): Month component for manifest file generation.
-                - dd (str): Day component for manifest file generation.
-                - repository_path (str): Path to the repository for manifest file.
-                - environment (str): The current environment in use.
-                - edc_json_schema_location (str): The location of EDC schema.
-                - edc_alation_user_id (str): The user ID for Alation API.
-
-        Returns:
-            manifest_dict (dict): A dictionary with the key "result" set to "success" if the operation completes successfully.
-        """
-
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
-            NAMESPACE_NAME, SERVICE_NAME)
-        logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
-            NAMESPACE_NAME, SERVICE_NAME)
-        tracer = tracer_singleton.get_tracer()
-
-        with tracer.start_as_current_span("upload_schema_manifest"):
-            try:
-
-                # Get the configuration data
-                edc_alation_base_url = config.get("edc_alation_base_url")
-                # Format as a 24-hour time string
-                repository_path = config.get("repository_path")
-                environment = config.get("environment")
-                schema_file_path = config.get("edc_json_schema_location")
-                alation_user_id = config.get("edc_alation_user_id")
-                alation_schema_id = metadata_json_data.get("alationSchemaID")
-
-                logger.info(f"alation_user_id:{alation_user_id}")
-
-                # Get the API access token
-                token_endpoint = TokenEndpoint(edc_alation_base_url)
-                status_code, edc_alation_api_token, alation_refresh_token = token_endpoint.get_api_token_from_config(
-                    config)
-                logger.info(
-                    f"get_api_token_from_config:status_code:{status_code}")
-                msg = f"edc_alation_api_token length:{str(len(edc_alation_api_token))}"
-                logger.info(msg)
-
-                if len(edc_alation_api_token.strip()) == 0:
-                    msg = "Alation API Access Token is not set"
-                    raise ValueError(msg)
-
-                # Get the schema and datasource information
-                schema_results, datasource_results = cls.get_schema(
-                    edc_alation_api_token, edc_alation_base_url, alation_schema_id
-                )
-
-                schema_result_json = schema_results.json()
-                schema_name = schema_result_json[0].get("name")
-                datasource_title = datasource_results.get("title")
-                alation_data_source_id = datasource_results.get("id")
-
-                # Get the manifest file name
-                manifest_json_file = cls.get_manifest_json_file_name(
-                    "upload", repository_path, datasource_title, schema_name, environment, alation_user_id)
-
-                # Write the manifest file
-                with open(manifest_json_file, "w", encoding='utf-8') as f:
-                    json.dump(metadata_json_data, f)
-
-                # Validate the manifest file
-                msg = 'Validating the manifest file at {0} with schema'.format(
-                    manifest_json_file)
-                logger.info(msg)
-
-                manifest = Manifest(schema_file_path)
-                metadata = manifest.validate_manifest(manifest_json_file)
-                logger.info(
-                    f"Metadata File Validated file of length {str(len(metadata))}")
-
-                # Update based on Manifest file
-                if token_endpoint.validate_refresh_token(alation_user_id, alation_refresh_token) is not None:
-
-                    custom_fields_endpoint = CustomFieldsEndpoint()
-                    logger.info(
-                        'Created custom fields endpoint for updating custom fields via API')
-
-                    tags_endpoint = TagsEndpoint(
-                        edc_alation_api_token, edc_alation_base_url)
-                    logger.info(
-                        'Created tags endpoint for updating tags via API')
-
-                    id_finder_endpoint = IdFinderEndpoint(
-                        edc_alation_api_token, edc_alation_base_url)
-
-                    # encode key
-                    # always encode schema name regardless of ENCODE_PERIOD
-                    if '.' in schema_name:
-                        encoded_schema_name = f"\"{schema_name}\""
-                    else:
-                        encoded_schema_name = schema_name
-
-                    # Update the schema
-                    logger.info(
-                        'Created id finder for getting detailed information on Alation objects')
-                    logger.info('Updating the schema fields for data source {0} and schema {1}'.format(
-                        alation_data_source_id, schema_name))
-
-                    schema = manifest.get_schema_data()
-                    response_content = custom_fields_endpoint.update(edc_alation_api_token, edc_alation_base_url,
-                                                                     "schema", alation_data_source_id, encoded_schema_name, schema, True)
-                    logger.info("response_content: " + str(response_content))
-                    schema_key = str(alation_data_source_id) + \
-                        "." + encoded_schema_name
-                    schema_id = id_finder_endpoint.find('schema', schema_key)
-                    for tag in manifest.tags:
-                        tags_endpoint.apply('schema', schema_id, tag)
-
-                    # Update the tables
-                    tables_dict = manifest.get_tables_data()
-                    if tables_dict:
-                        total_items = len(tables_dict.items())
-                        # reinit endpoint
-                        obj_custom_fields_endpoint = CustomFieldsEndpoint()
-
-                        for idx, (key, value) in enumerate(tables_dict.items()):
-                            # Set force_submit to True on the last item
-                            force_submit = (idx == total_items - 1)
-                            table_result = cls.update_table_structure(edc_alation_api_token,
-                                                                      edc_alation_base_url, alation_data_source_id, schema_name,
-                                                                      value, force_submit=force_submit, obj_custom_fields_endpoint=obj_custom_fields_endpoint)
-                            logger.info("table_result: " + str(table_result))
-                        # Commented out the threading because complexity not worth it
-                        # compared to batching updates in sets of 50
-                        # and limiting updates to differences
-
-                        # num_threads = min(NUM_THREADS_MAX, len(tables_dict))
-
-                        # Using ThreadPoolExecutor
-                        # with concurrent.futures.ThreadPoolExecutor(max_workers=num_threads) as executor:
-                        #    futures = []
-                        #    items = list(tables_dict.items())
-                        #    total_items = len(items)
-
-                            # for idx, (key, value) in enumerate(items):
-                            # Set force_submit to True on the last item
-
-                            #    future = executor.submit(cls.update_table_structure, edc_alation_api_token,
-                            #                             edc_alation_base_url, alation_data_source_id, schema_name,
-                            #                             value, force_submit=force_submit)
-                            #    futures.append(future)
-
-                        # Wait for all futures to complete
-                        # concurrent.futures.wait(futures)
-                        return tables_dict
-
-                    else:
-                        error_msg = "No tables found"
-                        raise EdcAlationError(error_msg)
-                else:
-                    error_msg = "Refresh token is not valid"
-                    raise EdcAlationError(error_msg)
-            except Exception as ex:
-                error_msg = "Error: %s", ex
-                exc_info = sys.exc_info()
-                logger_singleton.error_with_exception(error_msg, exc_info)
-                raise
-
     @staticmethod
     def get_column_name(schema_name, table_name, column):
         """
         Construct and return the full column name, including schema, table and column names.
 
         Args:
             schema_name (str): The name of the schema.
             table_name (str): The table object. Must have a 'name' attribute representing the name of the table.
             column (object): The column object. Must have a 'name' attribute representing the name of the column.
 
         Returns:
             str: The full column name in the format "schema_name.table.name.column.name".
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
         with tracer.start_as_current_span("get_column_name"):
 
             try:
 
                 column_name = getattr(column, 'name', column)
@@ -838,181 +886,21 @@
                 return full_column_name
             except Exception as ex:
                 error_msg = "Error: %s", ex
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
-    @staticmethod
-    def update_table_structure(edc_alation_api_token, edc_alation_base_url, alation_data_source_id, schema_name, table, force_submit, obj_custom_fields_endpoint):
-        """
-        Updates the structure of a table in Alation.
-
-        This method updates the table information, applies tags to the table, and
-        updates the columns of the table. It uses Alation's custom fields API
-        endpoint for updating the table and columns and applies tags using Alation's
-        tags API endpoint.
-
-        Parameters:
-        alation_data_source_id (int): The ID of the Alation data source where the table resides.
-        schema_name (str): The name of the schema where the table resides.
-        edc_alation_edc_alation_edc_alation_api_access_token (str): The API access token for Alation.
-        edc_alation_base_url (str): The base URL for Alation's API.
-        unposted_table (Table): The table object that contains the updated structure.
-
-        Returns:
-        int: HTTP status code of the operation. 200 indicates success.
-        str: Status message of the operation. "OK" indicates success.
-        """
-
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
-            NAMESPACE_NAME, SERVICE_NAME)
-        logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
-            NAMESPACE_NAME, SERVICE_NAME)
-        tracer = tracer_singleton.get_tracer()
-        with tracer.start_as_current_span("upload_schema_manifest"):
-
-            try:
-
-                id_finder_endpoint = IdFinderEndpoint(
-                    edc_alation_api_token, edc_alation_base_url)
-                tags_endpoint = TagsEndpoint(
-                    edc_alation_api_token, edc_alation_base_url)
-
-                logger.info('Updating table {}'.format(table.name))
-
-                if schema_name == 'object_name_is_missing' or schema_name == 'object name is missing':
-                    raise ValueError('Invalid schema_name value.')
-
-                # encode the schema
-                if '.' in schema_name and ENCODE_PERIOD:
-                    encoded_schema_name = f"\"{schema_name}\""
-                else:
-                    encoded_schema_name = schema_name
-
-                # encode the table
-                special_chars = set('!"#$%&\\\'()*+,-./:;<=>?@[\\]^_`{}~')
-                table_name = table.name
-                if any(char in special_chars for char in table_name) and ENCODE_PERIOD:
-                    encoded_table_name = f"\"{table_name}\""
-                else:
-                    encoded_table_name = table_name
-
-                key = f"{encoded_schema_name}.{encoded_table_name}"
-                # Update the table
-                # Should only be one - ensure force_submit
-                response_content = obj_custom_fields_endpoint.update(edc_alation_api_token, edc_alation_base_url, "table",
-                                                                     alation_data_source_id,
-                                                                     key,
-                                                                     table, force_submit=True)
-
-                last_result = response_content
-                logger.info(f"response_content: {response_content}")
-
-                # Update the tags
-                # Encode ignoring ENCODE_PERIOD
-                # encode the schema
-                if '.' in schema_name:
-                    encoded_schema_name = f"\"{schema_name}\""
-                else:
-                    encoded_schema_name = schema_name
-
-                table_name = table.name
-                if '.' in table_name:
-                    encoded_table_name = f"\"{table_name}\""
-                else:
-                    encoded_table_name = table_name
-
-                table_key = f"{alation_data_source_id}.{encoded_schema_name}.{encoded_table_name}"
-
-                # Apply tags to the table
-                if table.tags is not None:
-                    table_id = id_finder_endpoint.find(
-                        'table', table_key)
-                    for table_tag in table.tags:
-                        tags_endpoint.apply(
-                            'table', table_id, table_tag)
-
-                from data_ecosystem_services.alation_service.column import Column
-                # Update the columns to convert string to objects if necessary
-                columns_dict = table.columns
-
-                # Update the columns
-                if columns_dict is not None:
-
-                    # Using ThreadPoolExecutor
-                    num_threads = min(NUM_THREADS_MAX, len(columns_dict))
-
-                    if '.' in schema_name and ENCODE_PERIOD:
-                        encoded_schema_name = f"\"{schema_name}\""
-                    else:
-                        encoded_schema_name = schema_name
-
-                    special_chars = set('!"#$%&\'()*+,-./:;<=>?@[\]^_`{}~')
-
-                    table_name = table.name
-                    if any(char in special_chars for char in table_name) and ENCODE_PERIOD:
-                        encoded_table_name = f"\"{table_name}\""
-                    else:
-                        encoded_table_name = table_name
-
-                    with concurrent.futures.ThreadPoolExecutor(max_workers=num_threads) as executor:
-                        last_future_result = ""
-                        futures = []
-                        total_items = len(columns_dict.items())
-                        special_chars = set(
-                            '!"#$%&\\\'()*+,-./:;<=>?@[\\]^_`{}~')
-
-                        for idx, (key, value) in enumerate(columns_dict.items()):
-                            # Set force_submit to True on the last item
-                            force_submit = (idx == total_items - 1)
-                            if any(char in special_chars for char in key) and ENCODE_PERIOD:
-                                encoded_column_name = f"\"{key}\""
-                            else:
-                                encoded_column_name = key
-
-                            future = executor.submit(obj_custom_fields_endpoint.update, edc_alation_api_token, edc_alation_base_url, "attribute",
-                                                     alation_data_source_id,
-                                                     f"{encoded_schema_name}.{encoded_table_name}.{encoded_column_name}",
-                                                     value, force_submit=force_submit)
-                            futures.append(future)
-
-                        # Wait for all futures to complete
-                        concurrent.futures.wait(futures)
-
-                        # Retrieve the result of the last future
-                        if futures:
-                            last_future_result = futures[-1].result()
-                        else:
-                            last_future_result = "No return value from last update call"
-
-                        last_result = str(last_result) + \
-                            str(last_future_result)
-
-                else:
-                    warning_msg = f"No columns supplied to update for table: {table_name}"
-                    logger.warning(warning_msg)
-                    last_result = str(last_result) + warning_msg
-
-                return last_result
-
-            except Exception as ex:
-                error_msg = f"Error: {str(ex)}",
-                exc_info = sys.exc_info()
-                logger_singleton.error_with_exception(error_msg, exc_info)
-                raise
-
     @classmethod
-    def get_table_structure(cls, edc_alation_api_token, edc_alation_base_url, alation_data_source_id, alation_schema_id, unfetched_table, expected_table_fields, expected_column_fields):
+    def get_table_structure(cls, edc_alation_api_token, edc_alation_base_url, alation_datasource_id, alation_schema_id, unfetched_table, expected_table_fields, expected_column_fields):
         """
         Fetches the structure of a table, including its columns, based on the provided information.
 
         Args:
-            alation_data_source_id (str): The Alation data source ID associated with the table.
+            alation_datasource_id (str): The Alation data source ID associated with the table.
             alation_schema_id (str): The Alation schema ID associated with the table.
             alation_headers (dict): The headers to be used for making API requests to Alation.
             edc_alation_base_url (str): The base URL for the Alation instance.
             unfetched_table (dict): A dictionary representing the unfetched table.
             expected_table_fields (list): A list of expected fields for the table.
             expected_column_fields (list): A list of expected fields for the columns in the table.
 
@@ -1035,15 +923,15 @@
                 else:
                     fetched_table[tf] = expected_table_fields[tf]
 
         # iterate through each column associated with this table and add a manifest template entry
         custom_field_dict = unfetched_table.get('custom_fields')
         alation_table_id = unfetched_table.get('id')
         columns_dict = cls.get_table_columns(
-            edc_alation_api_token, edc_alation_base_url, alation_data_source_id, alation_schema_id, alation_table_id)
+            edc_alation_api_token, edc_alation_base_url, alation_datasource_id, alation_schema_id, alation_table_id)
         if columns_dict:
             fetched_table["columns"] = []
             # for each column associated with this table...
             for c in columns_dict:
                 this_column_dict = {}
                 for cf in expected_column_fields:
                     if cf in columns_dict[c]:
@@ -1061,37 +949,37 @@
                 this_custom_flds_dict[i['field_name']] = i['value']
                 fetched_table["customfields"].append(
                     this_custom_flds_dict)
 
         return fetched_table
 
     @classmethod
-    def get_schema_structure(cls, edc_alation_api_token, edc_alation_base_url, manifest, alation_data_source_id, alation_schema_id):
+    def get_schema_structure(cls, edc_alation_api_token, edc_alation_base_url, manifest, alation_datasource_id, alation_schema_id):
         """
         Retrieves the structure of a specific schema from Alation using the provided schema ID and manifest.
 
         Args:
             edc_alation_api_token (str): The API token for authenticating with the Alation instance.
             edc_alation_base_url (str): The base URL of the Alation instance.
             manifest (dict): The manifest defining the structure of the schema.
-            alation_data_source_id (int): The ID of the Alation data source related to the schema.
+            alation_datasource_id (int): The ID of the Alation data source related to the schema.
             alation_schema_id (int): The ID of the Alation schema whose structure is to be retrieved.
 
         Raises:
             ValueError: If the response from the Alation API is not successful.
 
         Returns:
             tuple: A tuple containing the status code and a dictionary representing the structure of the schema.
         """
 
         try:
-            logger_singleton = pade_env_logging.LoggerSingleton.instance(
+            logger_singleton = cdc_env_logging.LoggerSingleton.instance(
                 NAMESPACE_NAME, SERVICE_NAME)
             logger = logger_singleton.get_logger()
-            tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+            tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
                 NAMESPACE_NAME, SERVICE_NAME)
             tracer = tracer_singleton.get_tracer()
 
             with tracer.start_as_current_span("get_schema_structure"):
                 schema_result_json = None
                 try:
                     schema_result, datasource_result = cls.get_schema(
@@ -1139,33 +1027,33 @@
                                         manifest_dict[field] = custom_field['value']
                                 # Exceptions to the rule - Fields that need to be manually mapped
                                 if not found_custom_field:
                                     # Enter the schema name in the identifier field
                                     if field == "identifier" and 'name' in schema:
                                         manifest_dict[field] = schema['name']
                                     elif field == "alationDatasourceID":
-                                        manifest_dict[field] = alation_data_source_id
+                                        manifest_dict[field] = alation_datasource_id
                                     elif field == "alationSchemaID":
                                         manifest_dict[field] = alation_schema_id
                                     else:
                                         manifest_dict[field] = schema_fields[field]
 
                         # Iterate through each table and add a manifest template entry
                         tables_dict = cls.get_schema_tables(
-                            edc_alation_api_token, edc_alation_base_url, alation_data_source_id, alation_schema_id)
+                            edc_alation_api_token, edc_alation_base_url, alation_datasource_id, alation_schema_id)
                         if tables_dict:
                             # Determine the number of threads to use
                             num_threads = min(
                                 NUM_THREADS_MAX, len(tables_dict))
 
                             # Using ThreadPoolExecutor
                             with concurrent.futures.ThreadPoolExecutor(max_workers=num_threads) as executor:
                                 futures = {}
                                 for unfetched_table, table_info in tables_dict.items():
-                                    future = executor.submit(cls.get_table_structure, edc_alation_api_token, edc_alation_base_url, alation_data_source_id, alation_schema_id,
+                                    future = executor.submit(cls.get_table_structure, edc_alation_api_token, edc_alation_base_url, alation_datasource_id, alation_schema_id,
                                                              table_info, expected_table_fields, expected_column_fields)
                                     futures[unfetched_table] = future
 
                                 for future in concurrent.futures.as_completed(futures.values()):
                                     manifest_dict["tables"].append(
                                         future.result())
                         else:
@@ -1180,7 +1068,528 @@
                 return manifest_dict
 
         except Exception as ex:
             error_msg = str(ex)
             exc_info = sys.exc_info()
             logger_singleton.error_with_exception(error_msg, exc_info)
             raise EdcAlationError(error_msg) from ex
+
+    @staticmethod
+    def update_table_structure(edc_alation_api_token, edc_alation_base_url, alation_datasource_id, schema_name, table: alation_table.Table, force_submit, obj_custom_fields_endpoint, valid_editable_fields, table_name):
+        """
+        Updates the structure of a table in Alation.
+
+        This method updates the table information, applies tags to the table, and
+        updates the columns of the table. It uses Alation's custom fields API
+        endpoint for updating the table and columns and applies tags using Alation's
+        tags API endpoint.
+
+        Parameters:
+        alation_datasource_id (int): The ID of the Alation data source where the table resides.
+        schema_name (str): The name of the schema where the table resides.
+        edc_alation_edc_alation_edc_alation_api_access_token (str): The API access token for Alation.
+        edc_alation_base_url (str): The base URL for Alation's API.
+        unposted_table (Table): The table object that contains the updated structure.
+
+        Returns:
+        int: HTTP status code of the operation. 200 indicates success.
+        str: Status message of the operation. "OK" indicates success.
+        """
+
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        logger = logger_singleton.get_logger()
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        tracer = tracer_singleton.get_tracer()
+        with tracer.start_as_current_span("upload_schema_manifest"):
+
+            try:
+
+                if table_name is None:
+                    raise ValueError('table_name cannot be None.')
+
+                id_finder_endpoint = IdFinderEndpoint(
+                    edc_alation_api_token, edc_alation_base_url)
+                tags_endpoint = TagsEndpoint(
+                    edc_alation_api_token, edc_alation_base_url)
+
+                if schema_name == 'object_name_is_missing' or schema_name == 'object name is missing':
+                    raise ValueError('Invalid schema_name value.')
+
+                # encode the schema
+                if '.' in schema_name and ENCODE_PERIOD:
+                    encoded_schema_name = f"\"{schema_name}\""
+                else:
+                    encoded_schema_name = schema_name
+
+                # encode the table
+                special_chars = set('!"#$%&\\\'()*+,-./:;<=>?@[\\]^_`{}~')
+
+                if any(char in special_chars for char in table_name) and ENCODE_PERIOD:
+                    encoded_table_name = f"\"{table_name}\""
+                else:
+                    encoded_table_name = table_name
+
+                key = f"{encoded_schema_name}.{encoded_table_name}"
+                # Update the table
+                # Should only be one - ensure force_submit
+                response_content = obj_custom_fields_endpoint.update(
+                    edc_alation_api_token, edc_alation_base_url, "table", alation_datasource_id, key, table, force_submit=force_submit, valid_editable_fields=valid_editable_fields)
+
+                last_result = response_content
+                logger.info(f"response_content: {response_content}")
+
+                # Update the tags
+                # Encode ignoring ENCODE_PERIOD
+                # encode the schema
+                if '.' in schema_name:
+                    encoded_schema_name = f"\"{schema_name}\""
+                else:
+                    encoded_schema_name = schema_name
+
+                if '.' in table_name:
+                    encoded_table_name = f"\"{table_name}\""
+                else:
+                    encoded_table_name = table_name
+
+                table_key = f"{alation_datasource_id}.{encoded_schema_name}.{encoded_table_name}"
+
+                # Apply tags to the table
+                if isinstance(table, alation_table.Table):
+                    if table.tags is not None:
+                        table_id = id_finder_endpoint.find(
+                            'table', table_key)
+                        for table_tag in table.tags:
+                            tags_endpoint.apply(
+                                'table', table_id, table_tag)
+
+                    from data_ecosystem_services.alation_service.db_column import Column
+                    # Update the columns to convert string to objects if necessary
+                    columns_dict = table.columns
+                else:
+                    columns_dict = table
+
+                # # Update the columns
+                # if columns_dict is not None:
+
+                #     # Using ThreadPoolExecutor
+                #     num_threads = min(NUM_THREADS_MAX, len(columns_dict))
+
+                #     if '.' in schema_name and ENCODE_PERIOD:
+                #         encoded_schema_name = f"\"{schema_name}\""
+                #     else:
+                #         encoded_schema_name = schema_name
+
+                #     special_chars = set('!"#$%&\'()*+,-./:;<=>?@[\]^_`{}~')
+
+                #     if any(char in special_chars for char in table_name) and ENCODE_PERIOD:
+                #         encoded_table_name = f"\"{table_name}\""
+                #     else:
+                #         encoded_table_name = table_name
+
+                #     with concurrent.futures.ThreadPoolExecutor(max_workers=num_threads) as executor:
+                #         last_future_result = ""
+                #         futures = []
+                #         total_items = len(columns_dict.items())
+                #         special_chars = set(
+                #             '!"#$%&\\\'()*+,-./:;<=>?@[\\]^_`{}~')
+
+                #         for idx, (key, value) in enumerate(columns_dict.items()):
+                #             # Set force_submit to True on the last item
+                #             force_submit = (idx == total_items - 1)
+                #             if any(char in special_chars for char in key) and ENCODE_PERIOD:
+                #                 encoded_column_name = f"\"{key}\""
+                #             else:
+                #                 encoded_column_name = key
+
+                #             future = executor.submit(obj_custom_fields_endpoint.update, edc_alation_api_token, edc_alation_base_url, "attribute",
+                #                                      alation_datasource_id,
+                #                                      f"{encoded_schema_name}.{encoded_table_name}.{encoded_column_name}",
+                #                                      value, force_submit=force_submit, valid_editable_fields=valid_editable_fields)
+                #             futures.append(future)
+
+                #         # Wait for all futures to complete
+                #         concurrent.futures.wait(futures)
+
+                #         # Retrieve the result of the last future
+                #         if futures:
+                #             last_future_result = futures[-1].result()
+                #         else:
+                #             last_future_result = "No return value from last update call"
+
+                #         last_result = str(last_result) + \
+                #             str(last_future_result)
+
+                # else:
+                #     warning_msg = f"No columns supplied to update for table: {table_name}"
+                #     logger.warning(warning_msg)
+                #     last_result = str(last_result) + warning_msg
+
+                return last_result
+
+            except Exception as ex:
+                error_msg = f"Error: {str(ex)}",
+                exc_info = sys.exc_info()
+                logger_singleton.error_with_exception(error_msg, exc_info)
+                raise
+
+    @classmethod
+    def upload_schema_manifest_json_file(cls, metadata_json_data, config):
+        """
+        Uploads a schema manifest to Alation.
+
+        Args:
+            metadata_json_data (dict): Contains metadata information such as the Alation Schema ID.
+            config (dict): Configuration data with the following keys:
+                - edc_alation_base_url (str): The base URL of the Alation instance.
+                - yyyy (str): Year component for manifest file generation.
+                - mm (str): Month component for manifest file generation.
+                - dd (str): Day component for manifest file generation.
+                - repository_path (str): Path to the repository for manifest file.
+                - environment (str): The current environment in use.
+                - edc_json_schema_location (str): The location of EDC schema.
+                - edc_alation_user_id (str): The user ID for Alation API.
+
+        Returns:
+            manifest_dict (dict): A dictionary with the key "result" set to "success" if the operation completes successfully.
+        """
+
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        logger = logger_singleton.get_logger()
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        tracer = tracer_singleton.get_tracer()
+
+        with tracer.start_as_current_span("upload_schema_manifest"):
+            try:
+
+                # Get the configuration data
+                edc_alation_base_url = config.get("edc_alation_base_url")
+                # Format as a 24-hour time string
+                repository_path = config.get("repository_path")
+                environment = config.get("environment")
+                alation_user_id = config.get("edc_alation_user_id")
+
+                # Get the Alation Schema ID form the json
+                alation_schema_id = metadata_json_data["alationSchemaID"]
+
+                logger.info(f"alation_user_id:{alation_user_id}")
+
+                # Get the API access token
+                token_endpoint = TokenEndpoint(edc_alation_base_url)
+                status_code, edc_alation_api_token, alation_refresh_token = token_endpoint.get_api_token_from_config(
+                    config)
+                logger.info(
+                    f"get_api_token_from_config:status_code:{status_code}")
+                msg = f"edc_alation_api_token length:{str(len(edc_alation_api_token))}"
+                logger.info(msg)
+
+                if len(edc_alation_api_token.strip()) == 0:
+                    msg = "Alation API Access Token is not set"
+                    raise ValueError(msg)
+
+                # Get the schema and datasource information
+                schema_results, datasource_results = cls.get_schema(
+                    edc_alation_api_token, edc_alation_base_url, alation_schema_id
+                )
+
+                # Get the schema and datasource information
+                schema_result_json = schema_results.json()
+                schema_name = schema_result_json[0].get("name")
+                datasource_title = datasource_results.get("title")
+                alation_datasource_id = datasource_results.get("id")
+
+                # Get the json schema file path
+                json_schema_file_path = cls.get_json_schema_file_path(
+                    repository_path, environment)
+                table = alation_table.Table(None, json_schema_file_path)
+
+                # Get expected table structure from Excel structure file
+                df_tables = table.get_tables_for_schema(config,
+                                                        alation_datasource_id, alation_schema_id)
+
+                # Get the valid editable fields
+                valid_editable_fields = table.get_valid_editable_fields_from_schema_xlsx(
+                    df_tables)
+
+                # Get the manifest file name
+                manifest_json_file = cls.get_json_manifest_file_path(
+                    "upload", repository_path, datasource_title, schema_name, environment, alation_user_id)
+
+                # Write the manifest file
+                with open(manifest_json_file, "w", encoding='utf-8') as f:
+                    json.dump(metadata_json_data, f)
+
+                # Validate the manifest file
+                msg = 'Validating the manifest file at {0} with schema'.format(
+                    manifest_json_file)
+                logger.info(msg)
+
+                manifest = ManifestJson(json_schema_file_path)
+                metadata = manifest.validate_manifest(
+                    manifest_json_file, json_schema_file_path)
+                logger.info(
+                    f"Metadata File Validated file of length {str(len(metadata))}")
+
+                # Update based on ManifestJson file
+                if token_endpoint.validate_refresh_token(alation_user_id, alation_refresh_token) is not None:
+
+                    custom_fields_endpoint = CustomFieldsEndpoint()
+                    logger.info(
+                        'Created custom fields endpoint for updating custom fields via API')
+
+                    tags_endpoint = TagsEndpoint(
+                        edc_alation_api_token, edc_alation_base_url)
+                    logger.info(
+                        'Created tags endpoint for updating tags via API')
+
+                    id_finder_endpoint = IdFinderEndpoint(
+                        edc_alation_api_token, edc_alation_base_url)
+
+                    # encode key
+                    # always encode schema name regardless of ENCODE_PERIOD
+                    if '.' in schema_name:
+                        encoded_schema_name = f"\"{schema_name}\""
+                    else:
+                        encoded_schema_name = schema_name
+
+                    # Update the schema
+                    logger.info(
+                        'Created id finder for getting detailed information on Alation objects')
+                    logger.info('Updating the schema fields for data source {0} and schema {1}'.format(
+                        alation_datasource_id, schema_name))
+
+                    schema = manifest.get_schema_data()
+                    response_content = custom_fields_endpoint.update(edc_alation_api_token, edc_alation_base_url,
+                                                                     "schema", alation_datasource_id, encoded_schema_name, schema, True, valid_editable_fields=valid_editable_fields)
+                    logger.info("response_content: " + str(response_content))
+                    schema_key = str(alation_datasource_id) + \
+                        "." + encoded_schema_name
+                    schema_id = id_finder_endpoint.find('schema', schema_key)
+                    for tag in manifest.tags:
+                        tags_endpoint.apply('schema', schema_id, tag)
+
+                    # Update the tables
+                    tables_dict = manifest.get_tables_data()
+                    if tables_dict:
+                        total_items = len(tables_dict.items())
+                        # reinit endpoint
+                        obj_custom_fields_endpoint = CustomFieldsEndpoint()
+
+                        for idx, (table_name, value) in enumerate(tables_dict.items()):
+                            # Set force_submit to True on the last item
+                            force_submit = (idx == total_items - 1)
+
+                            table_result = cls.update_table_structure(edc_alation_api_token,
+                                                                      edc_alation_base_url, alation_datasource_id, schema_name,
+                                                                      value, force_submit=force_submit, obj_custom_fields_endpoint=obj_custom_fields_endpoint, valid_editable_fields=valid_editable_fields, table_name=table_name)
+                            logger.info("table_result: " + str(table_result))
+                        # Commented out the threading because complexity not worth it
+                        # compared to batching updates in sets of 50
+                        # and limiting updates to differences
+
+                        # num_threads = min(NUM_THREADS_MAX, len(tables_dict))
+
+                        # Using ThreadPoolExecutor
+                        # with concurrent.futures.ThreadPoolExecutor(max_workers=num_threads) as executor:
+                        #    futures = []
+                        #    items = list(tables_dict.items())
+                        #    total_items = len(items)
+
+                            # for idx, (key, value) in enumerate(items):
+                            # Set force_submit to True on the last item
+
+                            #    future = executor.submit(cls.update_table_structure, edc_alation_api_token,
+                            #                             edc_alation_base_url, alation_datasource_id, schema_name,
+                            #                             value, force_submit=force_submit)
+                            #    futures.append(future)
+
+                        # Wait for all futures to complete
+                        # concurrent.futures.wait(futures)
+                        return tables_dict
+
+                    else:
+                        error_msg = "No tables found"
+                        raise EdcAlationError(error_msg)
+                else:
+                    error_msg = "Refresh token is not valid"
+                    raise EdcAlationError(error_msg)
+            except Exception as ex:
+                error_msg = "Error: %s", ex
+                exc_info = sys.exc_info()
+                logger_singleton.error_with_exception(error_msg, exc_info)
+                raise
+
+    @classmethod
+    def upload_schema_manifest_excel_file(cls, manifest_excel_file_path, config, json_schema_file_path):
+        """
+        Uploads a schema manifest to Alation.
+
+        Args:
+            metadata_excel_data (dict): Contains metadata information such as the Alation Schema ID.
+            config (dict): Configuration data with the following keys:
+                - edc_alation_base_url (str): The base URL of the Alation instance.
+                - yyyy (str): Year component for manifest file generation.
+                - mm (str): Month component for manifest file generation.
+                - dd (str): Day component for manifest file generation.
+                - repository_path (str): Path to the repository for manifest file.
+                - environment (str): The current environment in use.
+                - edc_json_schema_location (str): The location of EDC schema.
+                - edc_alation_user_id (str): The user ID for Alation API.
+
+        Returns:
+            manifest_dict (dict): A dictionary with the key "result" set to "success" if the operation completes successfully.
+        """
+
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        logger = logger_singleton.get_logger()
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
+            NAMESPACE_NAME, SERVICE_NAME)
+        tracer = tracer_singleton.get_tracer()
+
+        with tracer.start_as_current_span("upload_schema_manifest"):
+            try:
+
+                # Get the configuration data
+                edc_alation_base_url = config.get("edc_alation_base_url")
+                # Format as a 24-hour time string
+                repository_path = config.get("repository_path")
+                environment = config.get("environment")
+                alation_user_id = config.get("edc_alation_user_id")
+                json_schema_file_path = cls.get_json_schema_file_path(
+                    repository_path, environment)
+                logger.info(f"alation_user_id:{alation_user_id}")
+
+                # Get the API access token
+                token_endpoint = TokenEndpoint(edc_alation_base_url)
+                status_code, edc_alation_api_token, alation_refresh_token = token_endpoint.get_api_token_from_config(
+                    config)
+                logger.info(
+                    f"get_api_token_from_config:status_code:{status_code}")
+                msg = f"edc_alation_api_token length:{str(len(edc_alation_api_token))}"
+                logger.info(msg)
+
+                if len(edc_alation_api_token.strip()) == 0:
+                    msg = "Alation API Access Token is not set"
+                    raise ValueError(msg)
+
+                manifest_excel = alation_manifest_excel.ManifestExcel()
+                df_tables = manifest_excel.read_manifest_excel_file_tables_worksheet(
+                    manifest_excel_file_path)
+                alation_schema_id = df_tables['schema_id'][0]
+                logger.info(f"alation_schema_id:{alation_schema_id}")
+
+                # Get the schema and datasource information
+                schema_results, datasource_results = cls.get_schema(
+                    edc_alation_api_token, edc_alation_base_url, alation_schema_id
+                )
+
+                schema_result_json = schema_results.json()
+                schema_name = schema_result_json[0].get("name")
+                alation_datasource_id = datasource_results.get("id")
+
+                table = alation_table.Table(None, json_schema_file_path)
+
+                # Get expected table structure from Excel structure file
+                df_tables_expected = table.get_tables_for_schema(config,
+                                                                 alation_datasource_id, alation_schema_id)
+
+                # Get the valid editable fields
+                valid_editable_fields = table.get_valid_editable_fields_from_schema_xlsx(
+                    df_tables_expected)
+
+                # Update based on ManifestJson file
+                if token_endpoint.validate_refresh_token(alation_user_id, alation_refresh_token) is not None:
+
+                    custom_fields_endpoint = CustomFieldsEndpoint()
+                    logger.info(
+                        'Created custom fields endpoint for updating custom fields via API')
+
+                    tags_endpoint = TagsEndpoint(
+                        edc_alation_api_token, edc_alation_base_url)
+                    logger.info(
+                        'Created tags endpoint for updating tags via API')
+
+                    id_finder_endpoint = IdFinderEndpoint(
+                        edc_alation_api_token, edc_alation_base_url)
+
+                    # encode key
+                    # always encode schema name regardless of ENCODE_PERIOD
+                    if '.' in schema_name:
+                        encoded_schema_name = f"\"{schema_name}\""
+                    else:
+                        encoded_schema_name = schema_name
+
+                    # Update the schema
+                    logger.info(
+                        'Created id finder for getting detailed information on Alation objects')
+                    logger.info(
+                        f"Updating the schema fields for data source {alation_datasource_id} and schema {schema_name}")
+
+                    # TODO Update schema info when the schema tab is implemented
+                    # response_content = custom_fields_endpoint.update(edc_alation_api_token, edc_alation_base_url,
+                    #                                                  "schema", alation_datasource_id, encoded_schema_name, schema, True, valid_editable_fields=valid_editable_fields)
+                    # logger.info("response_content: " + str(response_content))
+                    # TODO Update the schema tags
+                    # schema_key = str(alation_datasource_id) + \
+                    #     "." + encoded_schema_name
+                    # schema_id = id_finder_endpoint.find('schema', schema_key)
+                    # for tag in manifest.tags:
+                    #    tags_endpoint.apply('schema', schema_id, tag)
+
+                    # Convert df_tables to a dictionary with 'table_name' as the key
+                    tables_dict = df_tables.set_index(
+                        'name').to_dict(orient='index')
+
+                    if tables_dict:
+                        total_items = len(tables_dict.items())
+                        # reinit endpoint
+                        obj_custom_fields_endpoint = CustomFieldsEndpoint()
+
+                        for idx, (key, table) in enumerate(tables_dict.items()):
+                            # Set force_submit to True on the last item
+                            force_submit = idx == total_items - 1
+
+                            table_name = key
+                            table_result = cls.update_table_structure(edc_alation_api_token,
+                                                                      edc_alation_base_url, alation_datasource_id, schema_name,
+                                                                      table, force_submit=force_submit, obj_custom_fields_endpoint=obj_custom_fields_endpoint, valid_editable_fields=valid_editable_fields, table_name=table_name)
+                            logger.info("table_result: " + str(table_result))
+
+                        # Commented out the threading because complexity not worth it
+                        # compared to batching updates in sets of 50
+                        # and limiting updates to differences
+
+                        # num_threads = min(NUM_THREADS_MAX, len(tables_dict))
+
+                        # Using ThreadPoolExecutor
+                        # with concurrent.futures.ThreadPoolExecutor(max_workers=num_threads) as executor:
+                        #    futures = []
+                        #    items = list(tables_dict.items())
+                        #    total_items = len(items)
+
+                        # for idx, (key, value) in enumerate(items):
+                        # Set force_submit to True on the last item
+
+                        #    future = executor.submit(cls.update_table_structure, edc_alation_api_token,
+                        #                             edc_alation_base_url, alation_datasource_id, schema_name,
+                        #                             value, force_submit=force_submit)
+                        #    futures.append(future)
+
+                        # Wait for all futures to complete
+                        # concurrent.futures.wait(futures)
+                        return tables_dict
+
+                    else:
+                        error_msg = "No tables found"
+                        raise EdcAlationError(error_msg)
+                else:
+                    error_msg = "Refresh token is not valid"
+                    raise EdcAlationError(error_msg)
+            except Exception as ex:
+                error_msg = f"Error: {str(ex)}"
+                exc_info = sys.exc_info()
+                logger_singleton.error_with_exception(error_msg, exc_info)
+                raise
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/tagsendpoint.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/tags.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/alation_service/tokenendpoint.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/alation_service/token.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from datetime import datetime
 import requests
 import sys
 from opentelemetry import trace
 from dotenv import load_dotenv, set_key, dotenv_values
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 
 from data_ecosystem_services.az_key_vault_service import (
     az_key_vault as pade_az_key_vault
 )
 
@@ -64,28 +64,28 @@
             such as Azure subscription details, Key Vault name, Key Vault secret keys,
             and Alation base URL.
 
         Returns:
             tuple: A tuple containing the status code and either the API access token or an error message.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_api_token_from_config"):
             try:
-                logger_singleton = pade_env_logging.LoggerSingleton.instance(
+                logger_singleton = cdc_env_logging.LoggerSingleton.instance(
                     NAMESPACE_NAME, SERVICE_NAME)
                 logger = logger_singleton.get_logger()
-                pade_env_tracing.TracerSingleton.log_to_console = False
-                tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+                cdc_env_tracing.TracerSingleton.log_to_console = False
+                tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
                     NAMESPACE_NAME, SERVICE_NAME)
                 tracer = tracer_singleton.get_tracer()
 
                 edc_alation_base_url = config.get("edc_alation_base_url")
                 edc_alation_user_id = config.get("edc_alation_user_id")
                 az_sub_tenant_id = config.get("az_sub_tenant_id")
                 az_sub_client_id = config.get("az_sub_client_id")
@@ -113,16 +113,23 @@
                     az_sub_tenant_id, az_sub_client_id, client_secret, az_kv_key_vault_name, running_interactive)
                 az_kv_edc_refresh_secret_key = config.get(
                     "az_kv_edc_refresh_secret_key")
                 logger.info(
                     f"az_kv_edc_refresh_secret_key: {az_kv_edc_refresh_secret_key}")
                 logger.info(
                     f"az_kv_edc_refresh_secret_key_length:{str(len(az_kv_edc_refresh_secret_key))}")
-                alation_refresh_token = az_key_vault.get_secret(
-                    az_kv_edc_refresh_secret_key)
+
+                alation_refresh_token = os.environ.get(
+                    az_kv_edc_refresh_secret_key.replace("-", "_"))
+
+                # If the environment variable is blank or not set, fetch the secret from Azure Key Vault
+                if not alation_refresh_token:
+                    alation_refresh_token = az_key_vault.get_secret(
+                        az_kv_edc_refresh_secret_key)
+
                 edc_alation_api_token = self.get_api_token(edc_alation_base_url,
                                                            edc_alation_user_id, alation_refresh_token)
 
                 logger.info(
                     f"edc_alation_api_access_token_length: {len(edc_alation_api_token)}")
                 status_code = 200
                 return status_code, edc_alation_api_token, alation_refresh_token
@@ -140,18 +147,18 @@
             api_token: The API token to validate.
             user_id: The user ID associated with the API token.
 
         Returns:
             True if the token is valid, False otherwise.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("validate_api_token"):
 
             api_url = f"{edc_alation_base_url}/integration/v1/validateAPIAccessToken/"
             data = {"api_access_token": edc_alation_api_token, "user_id": user_id}
@@ -195,18 +202,18 @@
         Returns:
             str: The API access token.
 
         Raises:
             requests.HTTPError: If there is an error during the token retrieval process.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_api_token"):
 
             try:
 
@@ -301,19 +308,19 @@
         Raises:
             Exception: If there is an error obtaining the API token.
 
         Returns:
             str: The API token.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span(f"getAPIToken"):
 
             logger.info(
                 f"Getting API token with {alation_refresh_token} refresh token for user {alation_user_id}")
@@ -383,19 +390,19 @@
 
             return alation_access_token, alation_headers
 
     # Won't work for CDC because we use SSO
     @staticmethod
     def create_alation_refresh_token(config):
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span(f"create_alation_refresh_token"):
 
             edc_alation_base_url = config.get("edc_alation_base_url")
             az_kv_edc_client_secret_key = config.get(
@@ -432,19 +439,19 @@
         edc_alation_user_id (str): The user ID for the Alation instance.
         edc_alation_refresh_token (str): The refresh token for the Alation instance.
 
         Returns:
         dict: The new API access token.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("create_api_access_token_via_refresh"):
 
             auth_url = edc_alation_base_url + "/integration/v1/createAPIAccessToken/"
             data = {
@@ -490,19 +497,19 @@
                         "edc_alation_base_url", "az_kv_edc_client_secret_key", and "edc_alation_client_id".
                         The values associated with these keys should be strings.
 
         Returns:
             str: The API token if the request is successful, "not_set" otherwise.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span(f"create_api_access_token_via_login"):
 
             edc_alation_base_url = config.get("edc_alation_base_url")
             az_kv_edc_client_secret_key = config.get(
@@ -543,19 +550,19 @@
             edc_alation_user_Id (str): The user ID for the Alation API.
             edc_alation_refresh_token (str): The refresh token to use when requesting an access token from the Alation API.
 
         Returns:
             str: The API access token.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span(f"get_edc_alation_api_access_token"):
 
             api_token = cls.create_api_access_token_via_refresh(
                 edc_alation_base_url, edc_alation_user_id, edc_alation_refresh_token)
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_client_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/az_client_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_client_service/azd_client.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/az_client_service/azd_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 import subprocess
 import sys
 import tarfile
 import urllib.request
 import platform
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
-    environment_file as pade_env_file
+    environment_file as cdc_env_file
 )
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 AZD_URL = "https://github.com/Azure/azure-dev/releases/download/azure-dev-cli_1.0.2/azd-linux-amd64.tar.gz"
@@ -56,31 +56,31 @@
         5. Creates a symbolic link to azd-linux-amd64.
         6. Runs the 'azd' command.
 
         Note: Ensure that the necessary permissions are available to perform file 
         operations and execute the 'azd' command.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("download_and_install_azd"):
 
             try:
                 # Change directory to home (~)
                 download_dir = os.path.expanduser("~")
                 os.chdir(download_dir)
                 logger.info(f"Changed directory to {download_dir}")
 
-                env_file = pade_env_file.EnvironmentFile()
+                env_file = cdc_env_file.EnvironmentFile()
 
                 url = ""
                 local_file_name = ""
 
                 if platform.system() == 'Windows':
                     url = 'https://aka.ms/install-azd.ps1"'
                     local_file_name = "install-azd.ps1"
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_key_vault_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_admin_service/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""Initialize the az_key_vault_service subpackage of data_ecosystem_services package"""
+"""Initialize the cdc_admin_service subpackage of data_ecosystem_services package"""
 # allow absolute import from the root folder
 # whatever its name is.
-from ..cdc_admin_service import environment_tracing
-from ..cdc_admin_service import environment_logging
+from . import environment_tracing
+from . import environment_logging
 import sys  # don't remove required for error handling
 import os
 
 # Import from sibling directory ..\developer_service
 OS_NAME = os.name
 
 sys.path.append("..")
 if OS_NAME.lower() == "nt":
-    print("az_key_vault_service: windows")
+    print("cdc_admin_service: windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "\\..\\..")))
     sys.path.append(os.path.dirname(
         os.path.abspath(__file__ + "\\..\\..\\..")))
 else:
-    print("az_key_vault_service: non windows")
+    print("cdc_admin_service: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
 
-__all__ = ["az_client", "azd_client"]
+__all__ = ['environment_logging', 'environment_tracing']
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_key_vault_service/az_key_vault.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/az_key_vault_service/az_key_vault.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from azure.keyvault.secrets import SecretClient
 from azure.identity import DefaultAzureCredential, AzureDeveloperCliCredential
 from azure.mgmt.resource import ResourceManagementClient
 import azure.keyvault.secrets
 import os
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
@@ -35,19 +35,19 @@
         Args:
             tenant_id (str): The tenant_id of your Azure account. This is the directory ID.
             client_id (str): The client ID of the service principal.
             client_secret (str): The client secret of the service principal.
             key_vault_name (str): The name of your Azure Key Vault. You can get it from the Key Vault properties in the Azure portal.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("__init__"):
 
             self.vault_url = f"https://{key_vault_name}.vault.azure.net/"
             self.running_interactive = running_interactive
@@ -69,105 +69,110 @@
             # Set the KeyVaultTokenCallback object on the SecretClient object
             # self.client_dev.authentication_callback = self.callback_dev
 
     @classmethod
     def cdc_authentication_callback(client, context):
         # Obtain an access token from a custom authentication mechanism
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("cdc_authentication_callback"):
 
             access_token = cls.get_access_token(context)
 
             # Return the access token
             return access_token
 
     def get_credential_device(self):
         """Gets the DeviceCodeCredential for interactive running mode."""
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_credential_device"):
 
             return DeviceCodeCredential(
                 client_id=self.client_id, tenant_id=self.tenant_id, additionally_allowed_tenants=['*'])
 
     def get_credential(self):
         """Gets the ClientSecretCredential for non-interactive running mode."""
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_credential"):
+            logger.info(f"get_credential client_id: {client_id}")
+            logger.info(f"get_credential tenant_id: {tenant_id}")
+            logger.info(
+                f"get_credential client_secret_length: {len(self.client_secret)}")
 
             return ClientSecretCredential(
                 client_id=self.client_id, tenant_id=self.tenant_id, client_secret=self.client_secret)
 
     def get_secret_client(self, credential):
         """Creates a SecretClient using a given credential."""
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
-        with tracer.start_as_current_span(f"get_secret_client: {credential}"):
+        with tracer.start_as_current_span(f"get_secret_client"):
             return SecretClient(vault_url=self.vault_url, credential=credential)
 
     def retrieve_secret(self, secret_client, secret_name):
         """Attempts to retrieve a secret from the Azure Key Vault using a given SecretClient."""
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
-        with tracer.start_as_current_span(f"retrieve_secret {secret_name}"):
+        with tracer.start_as_current_span(f"retrieve_secret"):
 
             try:
+                logger.info(f"secret_name: {secret_name}")
                 return secret_client.get_secret(secret_name).value
             except Exception as e:
                 logger.error(f"Failed to retrieve secret: {e}")
                 return None
 
     def get_secret(self, secret_name):
         """Retrieves a secret from the Azure Key Vault."""
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
-        with tracer.start_as_current_span(f"get_secret {secret_name}"):
+        with tracer.start_as_current_span(f"get_secret"):
             logger.info(f"vault_url:{self.vault_url}")
             logger.info(f"tenant_id:{self.tenant_id}")
             logger.info(f"client_id:{self.client_id}")
             logger.info(f"running_interactive:{str(self.running_interactive)}")
-            logger.info(f"get_secret:{secret_name}")
+            logger.info(f"secret_name:{secret_name}")
 
             if self.running_interactive is True:
                 self.credential_device = self.get_credential_device()
                 self.client_device = self.get_secret_client(
                     self.credential_device)
                 secret_value = self.retrieve_secret(
                     self.client_device, secret_name)
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_storage_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/az_storage_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/az_storage_service/az_storage_queue.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/az_storage_service/az_storage_queue.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from azure.storage.queue import QueueServiceClient
 from azure.identity import ClientSecretCredential
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 import os
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/gpt_service/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Initialize the cdc_admin_service subpackage of data_ecosystem_services package"""
 # allow absolute import from the root folder
 # whatever its name is.
-from . import environment_tracing
-from . import environment_logging
 import sys  # don't remove required for error handling
 import os
 
 # Import from sibling directory ..\developer_service
 OS_NAME = os.name
 
 sys.path.append("..")
@@ -19,8 +17,8 @@
 else:
     print("cdc_admin_service: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
 
 
-__all__ = ['environment_logging', 'environment_tracing']
+__all__ = ['chat_completion', 'text_completion']
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/environment_logging.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_admin_service/environment_logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import logging.handlers
 from logging.handlers import TimedRotatingFileHandler
 from opentelemetry.instrumentation.flask import FlaskInstrumentor
 from datetime import datetime
 import traceback
 import inspect
 import platform
+from pathlib import Path
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing
+    environment_tracing as cdc_env_tracing
 )
 
 
 from opentelemetry.sdk._logs import (
     LoggingHandler,
     LoggerProvider
 )
@@ -52,18 +53,34 @@
     print("environment_logging: non windows")
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../..")))
     sys.path.append(os.path.dirname(os.path.abspath(__file__ + "/../../..")))
     env_path = os.path.dirname(os.path.abspath(sys.executable + "/.."))
     ENV_SHARE_PATH = env_path + "/share"
     ENV_SHARE_PATH = os.path.expanduser("~") + '/share'
+    ENV_SHARE_PATH = ENV_SHARE_PATH.replace("//", "/")
+
     sys.path.append(os.path.dirname(
         os.path.abspath(sys.executable + "/../share")))
-    LOG_FILENAME = ENV_SHARE_PATH + "/data_ecosystem_services_logging.txt"
 
+    # Define the desired log filename
+    desired_log_filename = "data_ecosystem_services_logging.txt"
+
+    # Construct the full path for the log file
+    log_file_path = os.path.join(ENV_SHARE_PATH, desired_log_filename)
+
+    # Check if the log file is writable
+    # if os.access(log_file_path, os.W_OK):
+    #    print(f"Had Permission to {log_file_path}")
+    #    LOG_FILENAME = log_file_path
+    # else:
+    #    print(f"No Permission to {log_file_path}")
+    # If not writable, set it to a file in the user's home directory
+    home_dir = Path.home()
+    LOG_FILENAME = home_dir / desired_log_filename
 
 try:
     FOLDER_EXISTS = os.path.exists(ENV_SHARE_PATH)
     if not FOLDER_EXISTS:
         # Create a new directory because it does not exist
         os.makedirs(ENV_SHARE_PATH)
 except Exception as e:
@@ -167,24 +184,32 @@
             LoggerSingleton._instance = self
 
         self.calling_namespace_name = calling_namespace_name
         self.calling_service_name = calling_service_name
         logger_provider = LoggerProvider()
         set_logger_provider(logger_provider)
 
-        connection_string = os.getenv("APPLICATIONINSIGHTS_CONNECTION_STRING")
+        # TODO Don't hard code
+        default_connection_string = "InstrumentationKey=d091b27b-14e0-437f-ae3c-90f3f04ef3dc;IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/"
+        connection_string = os.environ.get(
+            "APPLICATIONINSIGHTS_CONNECTION_STRING", default_connection_string)
 
-        if connection_string:
-            log_exporter = AzureMonitorLogExporter(
-                connection_string=connection_string)
-            logger_provider.add_log_record_processor(
-                BatchLogRecordProcessor(log_exporter))
-        else:
-            print(
-                "APPLICATIONINSIGHTS_CONNECTION_STRING is not set.")
+        try:
+            if connection_string:
+                log_exporter = AzureMonitorLogExporter(
+                    connection_string=connection_string)
+                logger_provider.add_log_record_processor(
+                    BatchLogRecordProcessor(log_exporter))
+            else:
+                print("APPLICATIONINSIGHTS_CONNECTION_STRING is not set.")
+
+        except Exception as e:
+            # Add the connection_string to the error message
+            logger.warning(
+                f"Failed to connect with connection_string: {connection_string}, Error: {e}")
 
         # Attach LoggingHandler to root logger
         self.file_path = LOG_FILENAME
         os.makedirs(os.path.dirname(ENV_SHARE_PATH), exist_ok=True)
         # Create a console handler and set its log level to INFO
         format = LOGGING_CONFIG['formatters']['default']['format']
         datefmt = LOGGING_CONFIG['formatters']['default']['datefmt']
@@ -206,14 +231,51 @@
         self.logger.addHandler(self.file_handler)
         self.logger.addHandler(self.console_handler)
         self.logger.addHandler(self.azure_handler)
 
         # Set the threshold of logger to INFO
         self.logger.setLevel(logging.INFO)
 
+    def validate_application_insights_connection_string(self):
+        """
+        Validates the Application Insights connection string and sends test logs.
+
+        This function checks if the environment variable 'APPLICATIONINSIGHTS_CONNECTION_STRING'
+        is set. If not, it uses a default connection string for testing purposes. The function
+        then initializes a logger and creates an instance of the AzureMonitorLogExporter using
+        the connection string. Test log messages are sent to Application Insights using the logger
+        and exporter to validate the connection.
+
+        Note: The default_connection_string used for testing in this function should be replaced
+        with the actual instrumentation key and endpoint URLs from your Application Insights
+        resource in a production environment.
+
+        Raises:
+            ValueError: If the provided connection string is invalid or missing.
+
+        Returns:
+            None: This function does not return anything but prints messages to the console
+            indicating the success or failure of the test log messages.
+        """
+        try:
+
+            # TODO Don't hard code
+            default_connection_string = "InstrumentationKey=d091b27b-14e0-437f-ae3c-90f3f04ef3dc;IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/"
+            connection_string = os.environ.get(
+                "APPLICATIONINSIGHTS_CONNECTION_STRING", default_connection_string)
+
+            # Log some test messages
+            self.logger.info("This is a test log message.")
+            self.logger.warning("This is a warning log message.")
+            self.logger.error("This is an error log message.")
+
+            return f"Successfully sent test logs to Application Insights: {connection_string}."
+        except Exception as e:
+            print(f"Error sending test logs: {e}")
+
     def get_exception_info(self, message, exc_info):
         """
         Retrieves detailed information about the most recently handled exception.
 
         This function should be called inside an 'except' block only. 
         It extracts and formats various details about the exception and its context, 
         such as the type and message of the exception, the filename and line number 
@@ -375,15 +437,15 @@
         file_path (str): The path to the log file.
         number_of_lines (int, optional): The number of lines to read from the end of the file. Defaults to 100.
 
         Returns:
         tuple: A tuple containing the actual number of lines read and the last number_of_lines of the log file.
         """
 
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         try:
             self.force_flush()
             tracer_singleton.force_flush()
             with open(LOG_FILENAME, 'r') as file:
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_admin_service/environment_tracing.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_admin_service/environment_tracing.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from azure.monitor.opentelemetry.exporter import AzureMonitorTraceExporter
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.semconv.resource import ResourceAttributes
 from opentelemetry.trace.status import StatusCode
 import opentelemetry.sdk.trace.export as trace_export
 import time
 from data_ecosystem_services.cdc_admin_service import (
-    environment_logging as pade_env_logging
+    environment_logging as cdc_env_logging
 )
 
 # Import from sibling directory ..\cdc_tech_environment_service
 OS_NAME = os.name
 
 
 sys.path.append("..")
@@ -154,19 +154,24 @@
         resource = Resource.create(
             {ResourceAttributes.SERVICE_NAME: calling_service_name,
              ResourceAttributes.SERVICE_NAMESPACE: calling_namespace_name})
 
         # Set tracer provider
         trace.set_tracer_provider(TracerProvider(resource=resource))
 
+        # TODO Don't hard code
+        default_connection_string = "InstrumentationKey=d091b27b-14e0-437f-ae3c-90f3f04ef3dc;IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/"
+        connection_string = os.environ.get(
+            "APPLICATIONINSIGHTS_CONNECTION_STRING", default_connection_string)
+
         # Check if the environment variable is set
         if "APPLICATIONINSIGHTS_CONNECTION_STRING" in os.environ:
             # This is the exporter that sends data to Application Insights
             azure_trace_exporter = AzureMonitorTraceExporter(
-                connection_string=os.environ["APPLICATIONINSIGHTS_CONNECTION_STRING"]
+                connection_string=connection_string
             )
             # Create a BatchSpanProcessor and add the exporter to it
             azure_span_processor = BatchSpanProcessor(azure_trace_exporter)
             # add to the tracer provider
             trace.get_tracer_provider().add_span_processor(azure_span_processor)
         else:
             print(
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_security_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_security_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_security_service/security_core.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_security_service/security_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """ Module for security_core for cdc_security_service with minimal dependencies. """
 
 from azure.core.exceptions import ClientAuthenticationError
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
-    environment_file as pade_env_file
+    environment_file as cdc_env_file
 )
 
 # core
 import data_ecosystem_services.cdc_admin_service.environment_logging as pade_env_log
 from adal import AuthenticationContext
 import requests
 from html.parser import HTMLParser  # web scraping html
@@ -49,19 +49,19 @@
             sp_azure_databricks_resource_id (str): service principal azure databricks resource id
             project_id(str): project id for logging
 
         Returns:
             dict: config_user dictionary with access_token populated
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("acquire_access_token_with_client_credentials"):
 
             info_message = f"acquire_access_token_with_client_credentials for {project_id}"
             print(info_message)
@@ -128,19 +128,19 @@
             sp_client_id (str): service principal client id
             sp_client_secret (str): service principal secret
 
         Returns:
             dict: config_user with refresh_token populated
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("acquire_access_token_with_refresh_token"):
 
             config_user = cls.setup_user_configuration(sp_client_id, sp_client_secret, sp_tenant_id, sp_redirect_url,
                                                        sp_authority_host_url, sp_azure_databricks_resource_id)
@@ -199,19 +199,19 @@
             sp_authority_host_url (str): service principal authority host url
             sp_azure_databricks_resource_id (str): service principal azure databricks resource id
 
         Returns:
             dict: populated config_user dictionary
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("setup_user_configuration"):
 
             sp_az_sub_oauth_token_endpoint = "".join(
                 [sp_authority_host_url.rstrip("/"), "/", sp_tenant_id])
@@ -242,19 +242,19 @@
         Args:
             config_user (dict): config_user dictionary
 
         Returns:
             dict: config_user dictionary populated with with refresh token
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("refresh_access_token"):
 
             az_sub_oauth_token_endpoint = config_user["az_sub_oauth_token_endpoint"]
             client_id = config_user["client_id"]
@@ -285,19 +285,19 @@
             config (dict): global config dictionary
             token (str): token
 
         Returns:
             list: list of pat tokens
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_pat_tokens"):
 
             databricks_instance_id = config["databricks_instance_id"]
             headers = {"Authentication": f"Bearer {token}"}
@@ -340,19 +340,19 @@
             token (str): token
             base_path (str): path to list files
 
         Returns:
             list: list of files at the path location
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_credentials_git"):
 
             databricks_instance_id = config["databricks_instance_id"]
             headers = {"Authentication": f"Bearer {token}"}
@@ -402,19 +402,19 @@
                 - If the password is not valid, returns (500, "Service principal password is not valid.").
 
         Raises:
             ClientAuthenticationError: If there is an authentication error when obtaining the token.
 
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("verify_az_sub_client_secret"):
 
             credential = ClientSecretCredential(
                 tenant_id, client_id, client_secret)
@@ -435,19 +435,19 @@
             token (str): token
             base_path (str): path to list files
 
         Returns:
             list: list of files at the path location
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("set_credentials_git"):
 
             databricks_instance_id = config["databricks_instance_id"]
             headers = {"Authentication": f"Bearer {token}"}
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/dataset_metadata.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/environment_metadata.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/environment_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import uuid
 from datetime import datetime
 
 # pade
 from data_ecosystem_services.cdc_security_service \
     import security_core as pade_sec_core
 from data_ecosystem_services.cdc_tech_environment_service \
-    import environment_file as pade_env_file
+    import environment_file as cdc_env_file
 from data_ecosystem_services.cdc_self_service \
     import logging_metadata as pade_log_metadata
 
 from dotenv import load_dotenv, find_dotenv, set_key
 
 # spark
 from pyspark.sql import (SparkSession, DataFrame)
@@ -236,15 +236,15 @@
             dbutils (_type_): _description_
             spark (_type_): _description_
 
         Returns:
             int: _description_
         """
 
-        obj_env_file = pade_env_file.EnvironmentFile()
+        obj_env_file = cdc_env_file.EnvironmentFile()
         file_size = obj_env_file.get_file_size(running_local,
                                                file_path, dbutils, spark)
         return file_size
 
     @staticmethod
     def file_exists(running_local: bool, path: str, dbutils) -> bool:
         """Takes in path, dbutils object, returns whether file exists at provided path
@@ -254,43 +254,43 @@
             path (str): path to file
             dbutils (object): databricks dbutils
 
         Returns:
             bool: True/False indication if file exists
         """
 
-        obj_env_file = pade_env_file.EnvironmentFile()
+        obj_env_file = cdc_env_file.EnvironmentFile()
         file_exists = obj_env_file.file_exists(running_local, path, dbutils)
         return file_exists
 
     @staticmethod
     def convert_to_windows_dir(path: str) -> str:
         """Takes in path and returns path with backslashes converted to forward slashes
 
         Args:
             path (str): path to be converted
 
         Returns:
             str: converted path
         """
-        obj_env_file = pade_env_file.EnvironmentFile()
+        obj_env_file = cdc_env_file.EnvironmentFile()
         converted_path = obj_env_file.convert_to_windows_dir(path)
         return converted_path
 
     @staticmethod
     def convert_to_current_os_dir(path: str) -> str:
         """Takes in path and returns path with backslashes converted to forward slashes
 
         Args:
             path (str): path to be converted
 
         Returns:
             str: converted path
         """
-        obj_env_file = pade_env_file.EnvironmentFile()
+        obj_env_file = cdc_env_file.EnvironmentFile()
         converted_path = obj_env_file.convert_to_current_os_dir(path)
         return converted_path
 
     @staticmethod
     def load_environment(running_local: bool, sp_tenant_id: str,
                          subscription_id: str,
                          sp_client_id: str,
@@ -333,15 +333,15 @@
                 sys.path.append(os.path.dirname(
                     os.path.abspath(env_share_path_2)))
                 env_file_path = env_share_path + "\\.env"
                 print(f"env_file_path: {env_file_path}")
                 # don't delete line below - it creates the file
             else:
                 print("non windows")
-                #env_share_path = env_path + "/share"
+                # env_share_path = env_path + "/share"
                 env_share_path = os.path.expanduser("~") + '/share'
                 folder_exists = os.path.exists(env_share_path)
                 if not folder_exists:
                     # Create a new directory because it does not exist
                     os.makedirs(env_share_path)
                 env_share_path_2 = sys.executable + "/../share"
                 sys.path.append(os.path.dirname(
@@ -427,14 +427,28 @@
 
         config_string = "config"
         cicd_action_string = "cicd"
 
         repository_path = cls.convert_to_current_os_dir(repository_path)
         env_folder_path = f"{repository_path.rstrip('/')}/{project_id_root}/{project_id}/"
         env_folder_path = cls.convert_to_current_os_dir(env_folder_path)
+        if os.path.exists(env_folder_path) and os.path.isdir(env_folder_path):
+            logger.info(f"The directory {env_folder_path} exists.")
+        else:
+            logger.info(f"The directory {env_folder_path} does not exist.")
+            two_levels_up = os.path.dirname(
+                os.path.dirname(env_folder_path)) + "/"
+            two_levels_up = cls.convert_to_current_os_dir(two_levels_up)
+            env_folder_path = two_levels_up
+            if os.path.exists(env_folder_path) and os.path.isdir(env_folder_path):
+                logger.info(f"The directory {env_folder_path} exists.")
+            else:
+                raise ValueError(
+                    f"The directory {env_folder_path} does not exist.")
+
         config_folder_path = f"{env_folder_path}{config_string}/"
         config_folder_path = cls.convert_to_current_os_dir(
             config_folder_path)
         environment_json_path = f"{config_folder_path}{config_string}.{environment}.json"
         environment_json_path_default = f"{config_folder_path}{config_string}.{environment}.json"
 
         # Check if environment_json_path exists
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/job_metadata.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/job_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/logging_metadata.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_self_service/pipeline_metadata.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_self_service/pipeline_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Initialize the cdc_tech_environment_service subpackage of pade_python package"""
+"""Initialize the cdc_tech_environment_service subpackage of data_ecosystem_services package"""
 
 # allow absolute import from the root folder
 # whatever its name is.
 import data_ecosystem_services.az_storage_service.az_storage_queue
 import data_ecosystem_services.cdc_tech_environment_service.job_core
 import data_ecosystem_services.cdc_tech_environment_service.repo_core
 import data_ecosystem_services.cdc_security_service.security_core
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """ Module for to convert differe file formats to Spark data frames. """
 
 # core
+import pandas as pd_legacy
+from collections import Counter
 import sys  # don't remove required for error handling
 import os
 import pyreadstat as prs
 
 from urllib.parse import urlparse
 from io import BytesIO
 
@@ -20,15 +22,15 @@
 from azure.identity import ClientSecretCredential
 
 # file excel
 import openpyxl
 import openpyxl.utils.cell
 
 # PADE
-import data_ecosystem_services.cdc_tech_environment_service.environment_file as pade_env_file
+import data_ecosystem_services.cdc_tech_environment_service.environment_file as cdc_env_file
 import data_ecosystem_services.cdc_tech_environment_service.dataset_core as pade_ds_core
 import data_ecosystem_services.cdc_security_service.security_core as pade_sec_core
 import data_ecosystem_services.cdc_tech_environment_service.environment_core as pade_env_core
 
 
 # data
 import numpy as np
@@ -50,31 +52,30 @@
     length,
     when,
     expr,
     to_json,
     explode,
 )
 
-from pyspark.sql.types import StructType, IntegerType, StructField, LongType, ArrayType, StringType,DoubleType,DecimalType
+from pyspark.sql.types import StructType, IntegerType, StructField, LongType, ArrayType, StringType, DoubleType, DecimalType
 from pyspark.sql import Row
 uuid_udf = udf(lambda: str(uuid.uuid4()), StringType())
-from collections import Counter
 
-import pandas as pd_legacy
 pyspark_pandas_loader = util.find_spec("pyspark.pandas")
 pyspark_pandas_found = pyspark_pandas_loader is not None
 
 if pyspark_pandas_found:
     os.environ['PYARROW_IGNORE_TIMEZONE'] = '1'
     import pyspark.pandas as pd
     # bug - pyspark version will not read local files
     # import pandas as pd
 else:
     import pandas as pd
 
+
 class DataSetConvert:
     """
     DataSetConvert Class to convert a dataset from one format to another.
     - Intended primarily to convert source file formats into Spark DataFrames.
     """
 
     @staticmethod
@@ -155,16 +156,18 @@
         )
 
         obj_ds_core = pade_ds_core.DataSetCore
 
         for col_orig in unsorted_df.columns:
             c_renamed = obj_ds_core.scrub_object_name(col_orig)
             unsorted_df = unsorted_df.withColumnRenamed(col_orig, c_renamed)
-            unsorted_df = unsorted_df.withMetadata(c_renamed, {"ingress_column_name": col_orig, 'comment': col_orig})
-            print(f"{c_renamed} :metadata: {unsorted_df.schema[c_renamed].metadata}")
+            unsorted_df = unsorted_df.withMetadata(
+                c_renamed, {"ingress_column_name": col_orig, 'comment': col_orig})
+            print(
+                f"{c_renamed} :metadata: {unsorted_df.schema[c_renamed].metadata}")
 
         return unsorted_df
 
     @classmethod
     def convert_json_to_dataframe(cls, spark: SparkSession, ingress_file_path: str, encoding: str,
                                   source_json_path: str, source_dataset_name: str, dataset_name: str) -> DataFrame:
         """Loads json file to dataframe
@@ -207,15 +210,16 @@
             )
         )
 
         # get column with the list of json for that type
         if len(source_json_path.strip()) > 0:
             # nested json
             list_columns = json_df.columns
-            json_df = json_df.withColumn("json_column", to_json(list_columns[0]))
+            json_df = json_df.withColumn(
+                "json_column", to_json(list_columns[0]))
             json_df_to_pandas = json_df.toPandas()
             first_row = json_df_to_pandas["json_column"].iloc[0]
             json_data = json.loads(first_row)
             dict_json = cls.get_json_by_key(json_data, source_dataset_name)
 
             dict_list = dict_json.items()
             dict_dataframe = defaultdict(list)
@@ -302,30 +306,34 @@
             client_id (str): azure client id used to download file
             client_secret (str): azure secret used to download file
 
         Returns:
             DataFrame: Converted Spark dataframe, schema is extracted from xpt file
         """
 
-        obj_env_file = pade_env_file.EnvironmentFile()
-        https_path = obj_env_file.convert_abfss_to_https_path(ingress_file_path)
-        credential = ClientSecretCredential(tenant_id, client_id, client_secret)
+        obj_env_file = cdc_env_file.EnvironmentFile()
+        https_path = obj_env_file.convert_abfss_to_https_path(
+            ingress_file_path)
+        credential = ClientSecretCredential(
+            tenant_id, client_id, client_secret)
 
         # download file
         storage_account_loc = urlparse(https_path).netloc
         account_url = f"https://{storage_account_loc}"
         storage_path = urlparse(https_path).path
         storage_container = storage_path.split('/')[1]
         file_path = storage_path.replace(f"{storage_container}" + "/", "")
         print(f"storage_path:{storage_path}")
         print(f"https_path:{https_path}")
         # print(f"ingress_mount:{ingress_mount}")
         print(f"ingress_file_path:{ingress_file_path}")
-        service_client = DataLakeServiceClient(account_url=account_url, credential=credential)
-        file_system_client = service_client.get_file_system_client(storage_container)
+        service_client = DataLakeServiceClient(
+            account_url=account_url, credential=credential)
+        file_system_client = service_client.get_file_system_client(
+            storage_container)
         file_client = file_system_client.get_file_client(file_path)
         download = file_client.download_file(0)
         download_bytes = download.readall()
         download_file = BytesIO(download_bytes)
 
         # step 1: get pandas data frame
 
@@ -333,50 +341,61 @@
         offset = 0
         # Get the function object in a variable getChunk
         if file_path.lower().endswith('sas7bdat'):
             get_chunk = prs.read_sas7bdat
         else:
             get_chunk = prs.read_xport
 
-        df_all_chunks, _ = get_chunk(ingress_file_path, row_limit=chunk_size, row_offset=offset)
+        df_all_chunks, _ = get_chunk(
+            ingress_file_path, row_limit=chunk_size, row_offset=offset)
         df_all_chunks = df_all_chunks.astype('category')
 
         while True:
             offset += chunk_size
             # for xpt data, use pyreadstat.read_xpt()
-            chunk, _ = prs.read_xport(ingress_file_path, row_limit=chunk_size, row_offset=offset)
+            chunk, _ = prs.read_xport(
+                ingress_file_path, row_limit=chunk_size, row_offset=offset)
             # if chunk is empty, it means the entire data has been read, so break
             if chunk.empty:
                 break
 
             # converting each column to categorical
             for each_col in chunk:
-                col_union = pd_legacy.api.types.union_categoricals([df_all_chunks[each_col], chunk[each_col]])
+                col_union = pd_legacy.api.types.union_categoricals(
+                    [df_all_chunks[each_col], chunk[each_col]])
                 df_all_chunks[each_col] = pd_legacy.Categorical(df_all_chunks[each_col],
                                                                 categories=col_union.categories)
-                chunk[each_col] = pd_legacy.Categorical(chunk[each_col], categories=col_union.categories)
+                chunk[each_col] = pd_legacy.Categorical(
+                    chunk[each_col], categories=col_union.categories)
 
             # Append each chunk to the resulting dataframe
             df_all_chunks = pd_legacy.concat([df_all_chunks, chunk])
 
         df_xpt, xpt_meta = prs.read_xport(download_file)
         df_data = spark.createDataFrame(df_xpt)
 
         # step 2: initalize empty pandas datafram
         df_metadata = pd.DataFrame()
 
         # read column name, labels into the new pandas dataframe
         df_metadata["name"] = xpt_meta.column_names = xpt_meta.column_names.str.strip()
-        df_metadata["label"] = xpt_meta.column_labels = [x.decode('utf-8') for x in xpt_meta.column_labels]
-        df_metadata["format"] = xpt_meta.column_formats = [x.decode('utf-8') for x in xpt_meta.column_formats]
-        df_metadata["type"] = xpt_meta.column_types = [x.decode('utf-8') for x in xpt_meta.variable_types]
-        df_metadata["type_in_source"] = xpt_meta.column_types = [x.decode('utf-8') for x in xpt_meta.original_variable_types]
-        df_metadata["length"] = xpt_meta.column_lengths = xpt_meta.column_lengths.astype(int)
-        df_metadata["note"] = xpt_meta.column_notes = [x.decode('utf-8') for x in xpt_meta.column_notes]
-        df_metadata["table_name"] = xpt_meta.table_name = xpt_meta.table_name.decode('utf-8')
+        df_metadata["label"] = xpt_meta.column_labels = [
+            x.decode('utf-8') for x in xpt_meta.column_labels]
+        df_metadata["format"] = xpt_meta.column_formats = [
+            x.decode('utf-8') for x in xpt_meta.column_formats]
+        df_metadata["type"] = xpt_meta.column_types = [
+            x.decode('utf-8') for x in xpt_meta.variable_types]
+        df_metadata["type_in_source"] = xpt_meta.column_types = [
+            x.decode('utf-8') for x in xpt_meta.original_variable_types]
+        df_metadata["length"] = xpt_meta.column_lengths = xpt_meta.column_lengths.astype(
+            int)
+        df_metadata["note"] = xpt_meta.column_notes = [
+            x.decode('utf-8') for x in xpt_meta.column_notes]
+        df_metadata["table_name"] = xpt_meta.table_name = xpt_meta.table_name.decode(
+            'utf-8')
 
         df_metadata = spark.createDataFrame(df_metadata)
         df_metadata.show()
         # extracting number of rows from the Dataframe
         row_count = df_metadata.count()
         # extracting number of columns from the Dataframe
         col_count = len(df_metadata.columns)
@@ -394,28 +413,28 @@
             df_pandas (_type_): _description_
             spark (_type_): _description_
 
         Returns:
             _type_: _description_
         """
 
-        list_pandas=[]
+        list_pandas = []
         df_pandas = df_pandas.reset_index()  # make sure indexes pair with number of rows
         for index, row in df_pandas.iterrows():
             print(row['column_name'], row['comment'])
             row_to_append = (row['column_name'], row['comment'])
             list_pandas.append(row_to_append)
         rdd = spark.sparkContext.parallelize(list_pandas)
-        rdd_columns = ["column_name","comment"]
-        df_spark= rdd.toDF(rdd_columns)
+        rdd_columns = ["column_name", "comment"]
+        df_spark = rdd.toDF(rdd_columns)
         return df_spark
 
     @classmethod
     def convert_sas_mount_to_dataframe_with_schema(cls, spark: SparkSession, source_abbreviation: str, file_name: str, tenant_id: str,
-                                             client_id: str, client_secret: str):
+                                                   client_id: str, client_secret: str):
         """ Loads xpt or bdat to dataframe and extracts schema from xpt file
         - Reference article: https://stackoverflow.com/questions/58612304/reading-huge-sas-dataset-in-python
         - PS: Please be noted that the resulting dataframe allChunk is going to have all column as Categorical data
 
         Args:
             spark (SparkSession): SparkSession
             ingress_file_path (str): ADLS2 path to csv or usv file
@@ -424,15 +443,15 @@
             client_secret (str): azure secret used to download file
 
         Returns:
             DataFrame: Converted Spark dataframe, schema is extracted from xpt file
         """
 
         # obj_ds_core = pade_ds_core.DataSetCore()
-        obj_env_file = pade_env_file.EnvironmentFile()
+        obj_env_file = cdc_env_file.EnvironmentFile()
         mount_file_path = "/Workspace/Repos/tbi8@cdc.gov/pade/od/od_nhanes/temp/"
         ingress_path = f"{mount_file_path}{source_abbreviation}/{file_name}"
         print(f"mount_file_path:{mount_file_path}")
         print(f"ingress_path:{ingress_path}")
 
         # df_xpt, xpt_meta = prs.read_xport(ingress_path,metadataonly=True)
         df_xpt, xpt_meta = prs.read_xport(ingress_path)
@@ -455,15 +474,14 @@
         # row_id_column
         # row_count                      xpt_meta.number_rows.astype(int)
         # ingress_row_count              xpt_meta.number_rows.astype(int)
         # ingress_ordinal_position
         # ingress_column_length           xpt_meta.column_lengths.astype(int)
         # ingress_table_name              xpt_meta.table_name.decode('utf-8')
 
-
         list_pandas = list(zip(xpt_meta.column_names, xpt_meta.column_labels))
         print(f"list_pandas: {list_pandas}")
         rdd = spark.sparkContext.parallelize(list_pandas)
 
         schema = StructType(
             [
                 StructField("column_name", StringType(), False),
@@ -499,15 +517,14 @@
         # printing
         print(f"Dimension of the Dataframe is: {(row,col)}")
         print(f"Number of Rows are: {row}")
         print(f"Number of Columns are: {col}")
 
         return df_metadata_spark, df_xpt
 
-
     @classmethod
     def convert_xpt_to_dataframe(cls, spark: SparkSession, ingress_file_path: str, tenant_id: str, client_id: str,
                                  client_secret: str) -> DataFrame:
         """Loads xpt to dataframe
         - XPT supports types - XPT types are converted to Spark types
         - Column names are not scrubbed or changed
         - No metadata is added to the dataframe
@@ -520,26 +537,30 @@
             client_id (str): azure client id used to download file
             client_secret (str): azure secret used to download file
 
         Returns:
             DataFrame: Spark dataframe
         """
 
-        obj_env_file = pade_env_file.EnvironmentFile()
-        https_path = obj_env_file.convert_abfss_to_https_path(ingress_file_path)
-        credential = ClientSecretCredential(tenant_id, client_id, client_secret)
+        obj_env_file = cdc_env_file.EnvironmentFile()
+        https_path = obj_env_file.convert_abfss_to_https_path(
+            ingress_file_path)
+        credential = ClientSecretCredential(
+            tenant_id, client_id, client_secret)
 
         # download file
         storage_account_loc = urlparse(https_path).netloc
         account_url = f"https://{storage_account_loc}"
         storage_path = urlparse(https_path).path
         storage_container = storage_path.split('/')[1]
         file_path = storage_path.replace(f"{storage_container}" + "/", "")
-        service_client = DataLakeServiceClient(account_url=account_url, credential=credential)
-        file_system_client = service_client.get_file_system_client(storage_container)
+        service_client = DataLakeServiceClient(
+            account_url=account_url, credential=credential)
+        file_system_client = service_client.get_file_system_client(
+            storage_container)
         file_client = file_system_client.get_file_client(file_path)
         download = file_client.download_file(0)
         download_bytes = download.readall()
         download_file = BytesIO(download_bytes)
 
         # step 1: get pandas data frame
         df_xpt = pd_legacy.read_sas(download_file, format='xport')
@@ -564,26 +585,30 @@
             client_id (str): azure client id used to download file
             client_secret (str): azure secret used to download file
 
         Returns:
             DataFrame: Spark dataframe
         """
 
-        obj_env_file = pade_env_file.EnvironmentFile()
-        https_path = obj_env_file.convert_abfss_to_https_path(ingress_file_path)
-        credential = ClientSecretCredential(tenant_id, client_id, client_secret)
+        obj_env_file = cdc_env_file.EnvironmentFile()
+        https_path = obj_env_file.convert_abfss_to_https_path(
+            ingress_file_path)
+        credential = ClientSecretCredential(
+            tenant_id, client_id, client_secret)
 
         # download file
         storage_account_loc = urlparse(https_path).netloc
         account_url = f"https://{storage_account_loc}"
         storage_path = urlparse(https_path).path
         storage_container = storage_path.split('/')[1]
         file_path = storage_path.replace(f"{storage_container}" + "/", "")
-        service_client = DataLakeServiceClient(account_url=account_url, credential=credential)
-        file_system_client = service_client.get_file_system_client(storage_container)
+        service_client = DataLakeServiceClient(
+            account_url=account_url, credential=credential)
+        file_system_client = service_client.get_file_system_client(
+            storage_container)
         file_client = file_system_client.get_file_client(file_path)
         download = file_client.download_file(0)
         download_bytes = download.readall()
         download_file = BytesIO(download_bytes)
 
         # step 1: get pandas data frame
         df_sas = pd_legacy.read_sas(download_file, format='sas7bdat')
@@ -629,26 +654,30 @@
                 skip_rows = 0
             else:
                 skip_rows = int(skip_rows_text)
 
         if sheet_name is None:
             sheet_name = ""
 
-        obj_env_file = pade_env_file.EnvironmentFile()
-        https_path = obj_env_file.convert_abfss_to_https_path(ingress_file_path)
-        credential = ClientSecretCredential(tenant_id, client_id, client_secret)
+        obj_env_file = cdc_env_file.EnvironmentFile()
+        https_path = obj_env_file.convert_abfss_to_https_path(
+            ingress_file_path)
+        credential = ClientSecretCredential(
+            tenant_id, client_id, client_secret)
 
         # download file
         storage_account_loc = urlparse(https_path).netloc
         account_url = f"https://{storage_account_loc}"
         storage_path = urlparse(https_path).path
         storage_container = storage_path.split('/')[1]
         file_path = storage_path.replace(f"{storage_container}" + "/", "")
-        service_client = DataLakeServiceClient(account_url=account_url, credential=credential)
-        file_system_client = service_client.get_file_system_client(storage_container)
+        service_client = DataLakeServiceClient(
+            account_url=account_url, credential=credential)
+        file_system_client = service_client.get_file_system_client(
+            storage_container)
         file_client = file_system_client.get_file_client(file_path)
         download = file_client.download_file(0)
         download_bytes = download.readall()
         download_file = BytesIO(download_bytes)
 
         work_book_data = None
         print("try open file")
@@ -694,30 +723,32 @@
         data = data[skip_rows + 1:]
         print(f"original cols:{cols}")
         cols = cols.tolist()
         cols = obj_ds_core.rename_column_names_as_unique(cols)
         print(f"deduplicated cols:{cols}")
         print(f"len(cols):{len(cols)}")
         print("call loadworkbook data")
-        print(f"2 open {https_path} work_book_data data_only False: read_only True")
+        print(
+            f"2 open {https_path} work_book_data data_only False: read_only True")
 
         try:
             work_book_data = openpyxl.load_workbook(
                 download_file, data_only=False, read_only=False
             )
             g_sheet = work_book_data.sheetnames
             if sheet_name is None or sheet_name == "":
                 work_sheet_data = work_book_data[0]
             else:
                 if sheet_name.isdigit():
                     work_sheet_data = work_book_data[g_sheet[int(sheet_name)]]
                 else:
                     work_sheet_data = work_book_data[sheet_name]
 
-            data_pass_1 = cls.convert_xlsx_to_list(data, cols, work_sheet_data, skip_rows)
+            data_pass_1 = cls.convert_xlsx_to_list(
+                data, cols, work_sheet_data, skip_rows)
             print("close work_book_data data_only True: read_only True")
         finally:
             if work_book_data is not None:
                 work_book_data.close()
 
         # formula
         print(f"3 open {https_path} work_book_formula")
@@ -728,15 +759,16 @@
                 download_file, data_only=True, read_only=False
             )
             g_sheet = work_book_formula.sheetnames
             if sheet_name is None or sheet_name == "":
                 work_sheet_formula = work_book_formula[0]
             else:
                 if sheet_name.isdigit():
-                    work_sheet_formula = work_book_formula[g_sheet[int(sheet_name)]]
+                    work_sheet_formula = work_book_formula[g_sheet[int(
+                        sheet_name)]]
                 else:
                     work_sheet_formula = work_book_formula[sheet_name]
 
             print("call loadworkbook formula")
             data_pass_2 = cls.convert_xlsx_to_list(
                 data_pass_1, cols, work_sheet_formula, skip_rows
             )
@@ -762,21 +794,23 @@
             c_renamed = obj_ds_core.scrub_object_name(col_orig)
             if c_renamed.startswith("unnamed:_"):
                 c_renamed = c_renamed.replace("unnamed:_", "")
                 # increments #by 1
                 c_renamed = int(c_renamed) + 1
                 c_renamed = "Column" + str(c_renamed)
             unsorted_df = unsorted_df.withColumnRenamed(col_orig, c_renamed)
-            unsorted_df = unsorted_df.withMetadata(c_renamed, {"ingress_column_name": col_orig, 'comment': col_orig})
+            unsorted_df = unsorted_df.withMetadata(
+                c_renamed, {"ingress_column_name": col_orig, 'comment': col_orig})
 
         # replace nulls
         unsorted_df.na.fill(0)
         unsorted_df.na.fill("")
         unsorted_df.show()
-        unsorted_df = unsorted_df.withColumn("__meta_sheet_name", lit(sheet_name))
+        unsorted_df = unsorted_df.withColumn(
+            "__meta_sheet_name", lit(sheet_name))
 
         return unsorted_df
 
     @staticmethod
     def convert_xlsx_to_list(data, cols, work_sheet, skip_rows):
         """Loads excel worksheet into a list of dictionaries
 
@@ -791,15 +825,16 @@
         """
 
         # iterate through excel and display data
         for i_row, row_item in enumerate(data):
             row_item_updated = [""] * (len(cols))
             for j_col, col_item in enumerate(row_item):
                 col_item_updated = col_item
-                cell = work_sheet.cell(row=i_row + 2 + skip_rows, column=j_col + 1)
+                cell = work_sheet.cell(
+                    row=i_row + 2 + skip_rows, column=j_col + 1)
                 if cell.hyperlink is not None:
                     url = str(cell.hyperlink.target)
                     col_item_updated = "[" + str(cell.value) + "](" + url + ")"
                 else:
                     if cell.value is not None:
                         col_item_updated = cell.value
                     else:
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 # file excel
 import openpyxl
 import openpyxl.utils.cell
 
 # PADE
 import data_ecosystem_services.cdc_tech_environment_service.dataset_core as pade_ds_core
-import data_ecosystem_services.cdc_tech_environment_service.environment_file as pade_env_file
+import data_ecosystem_services.cdc_tech_environment_service.environment_file as cdc_env_file
 import data_ecosystem_services.cdc_security_service.security_core as pade_sec_core
 import data_ecosystem_services.cdc_tech_environment_service.environment_core as pade_env_core
 
 # spark / data
 import uuid
 from pyspark.sql import SparkSession, DataFrame
 import pyspark.sql.utils
@@ -99,15 +99,15 @@
             partition_by (_type_, optional): _description_. Defaults to None.
 
         Returns:
             _type_: _description_
         """
 
         obj_ds_core = pade_ds_core.DataSetCore()
-        obj_env_file = pade_env_file.EnvironmentFile()
+        obj_env_file = cdc_env_file.EnvironmentFile()
 
         yyyy_param = config["yyyy"]
         mm_param = config["mm"]
         dd_param = config["dd"]
 
         if yyyy_param is None:
             yyyy_param = ""
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """ Module with a variety of metadata extraction routines for different source formats. """
 
 # core
+import data_ecosystem_services.cdc_tech_environment_service.environment_file as cdc_env_file
+from azure.identity import ClientSecretCredential
+from azure.storage.filedatalake import DataLakeServiceClient
+from pyspark.sql import SparkSession, DataFrame
 import sys  # don't remove required for error handling
 import os
 
 from urllib.parse import urlparse
 from io import BytesIO
 
 # libraries
 from importlib import util
 
 import pyreadstat as prs
 import pandas as pd_legacy
 os.environ['PYARROW_IGNORE_TIMEZONE'] = '1'
 pyspark_pandas_loader = util.find_spec("pyspark.pandas")
 pyspark_pandas_found = pyspark_pandas_loader is not None
-from pyspark.sql import SparkSession, DataFrame
 
 if pyspark_pandas_found:
     import pyspark.pandas as pd
     # bug - pyspark version will not read local files
     # import pandas as pd
 else:
     import pandas as pd
 
 # adls and azure security
-from azure.storage.filedatalake import DataLakeServiceClient
-from azure.identity import ClientSecretCredential
 
 # PADE
-import data_ecosystem_services.cdc_tech_environment_service.environment_file as pade_env_file
+
 
 class DataSetExtract:
     """DataSetExtract class for Spark Datasets handle metadata extraction from different source formats
     """
 
     @classmethod
     def extract_xpt_dataframe_schema(cls, spark: SparkSession, ingress_file_path: str, tenant_id: str,
@@ -47,44 +48,55 @@
             client_id (str): azure client id used to download file
             client_secret (str): azure secret used to download file
 
         Returns:
             DataFrame: Spark dataframe
         """
 
-        obj_env_file = pade_env_file.EnvironmentFile()
-        https_path = obj_env_file.convert_abfss_to_https_path(ingress_file_path)
-        credential = ClientSecretCredential(tenant_id, client_id, client_secret)
+        obj_env_file = cdc_env_file.EnvironmentFile()
+        https_path = obj_env_file.convert_abfss_to_https_path(
+            ingress_file_path)
+        credential = ClientSecretCredential(
+            tenant_id, client_id, client_secret)
 
         # download file
         storage_account_loc = urlparse(https_path).netloc
         account_url = f"https://{storage_account_loc}"
         storage_path = urlparse(https_path).path
         storage_container = storage_path.split('/')[1]
         file_path = storage_path.replace(f"{storage_container}" + "/", "")
-        service_client = DataLakeServiceClient(account_url=account_url, credential=credential)
-        file_system_client = service_client.get_file_system_client(storage_container)
+        service_client = DataLakeServiceClient(
+            account_url=account_url, credential=credential)
+        file_system_client = service_client.get_file_system_client(
+            storage_container)
         file_client = file_system_client.get_file_client(file_path)
         download = file_client.download_file(0)
         download_bytes = download.readall()
         download_file = BytesIO(download_bytes)
 
         # step 1: get pandas data frame
 
         xpt_meta = prs.read_xport(download_file, metadataonly=True)
 
         # step 2: initalize empty pandas dataframe
         df_metadata = pd.DataFrame()
 
         # read column name, labels into the new pandas dataframe
         df_metadata["name"] = xpt_meta.column_names = xpt_meta.column_names.str.strip()
-        df_metadata["label"] = xpt_meta.column_labels = [x.decode('utf-8') for x in xpt_meta.column_labels]
-        df_metadata["format"] = xpt_meta.column_formats = [x.decode('utf-8') for x in xpt_meta.column_formats]
-        df_metadata["type"] = xpt_meta.column_types = [x.decode('utf-8') for x in xpt_meta.variable_types]
-        df_metadata["type_in_source"] = xpt_meta.column_types = [x.decode('utf-8') for x in xpt_meta.original_variable_types]
-        df_metadata["length"] = xpt_meta.column_lengths = xpt_meta.column_lengths.astype(int)
-        df_metadata["note"] = xpt_meta.column_notes = [x.decode('utf-8') for x in xpt_meta.column_notes]
-        df_metadata["table_name"] = xpt_meta.table_name = xpt_meta.table_name.decode('utf-8')
+        df_metadata["label"] = xpt_meta.column_labels = [
+            x.decode('utf-8') for x in xpt_meta.column_labels]
+        df_metadata["format"] = xpt_meta.column_formats = [
+            x.decode('utf-8') for x in xpt_meta.column_formats]
+        df_metadata["type"] = xpt_meta.column_types = [
+            x.decode('utf-8') for x in xpt_meta.variable_types]
+        df_metadata["type_in_source"] = xpt_meta.column_types = [
+            x.decode('utf-8') for x in xpt_meta.original_variable_types]
+        df_metadata["length"] = xpt_meta.column_lengths = xpt_meta.column_lengths.astype(
+            int)
+        df_metadata["note"] = xpt_meta.column_notes = [
+            x.decode('utf-8') for x in xpt_meta.column_notes]
+        df_metadata["table_name"] = xpt_meta.table_name = xpt_meta.table_name.decode(
+            'utf-8')
 
         metadata_df = spark.createDataFrame(df_metadata)
 
         return metadata_df
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_core.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/environment_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_file.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/environment_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
 # spark
 from pyspark.sql import (SparkSession)
 from pyspark.sql.types import (IntegerType, LongType, StringType, StructField,
                                StructType)
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 
 #  data
 pyspark_pandas_loader = util.find_spec("pyspark.pandas")
 pyspark_pandas_found = pyspark_pandas_loader is not None
 
@@ -116,18 +116,18 @@
 
         Returns
         -------
         msg : str
             A message that lists which files have been deleted.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("delete_directory_files"):
 
             files = glob.glob(os.path.join(directory, f'*.{file_extension}'))
             msg = ""
@@ -156,18 +156,18 @@
         Args:
             path (str): path to convert
 
         Returns:
             str: converted path
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("convert_to_current_os_dir"):
             logger.info(f"convert_to_current_os_dir: {path}")
             if platform.system() == 'Windows':
                 converted_path = cls.convert_to_windows_dir(path)
@@ -188,18 +188,18 @@
         Args:
             folder_path (str): path to convert
 
         Returns:
             str: _converted path
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("convert_to_windows_dir"):
 
             logger.info(f"convert_to_windows_dir: {folder_path}")
             window_dir = "\\"
@@ -220,18 +220,18 @@
         Args:
             folder_path (str): path to convert
 
         Returns:
             str: _converted path
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("convert_to_unix_dir"):
             logger.info(f"convert_to_unix_dir: {folder_path}")
 
             window_dir = "\\"
@@ -270,17 +270,17 @@
 
         Returns:
             tuple: A tuple containing two elements:
                 - int: The status code - 200 for successful execution, 500 for an error.
                 - str: The output of the script in case of success, or the error message in case of an error.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("execute_script_file"):
 
             try:
 
@@ -335,17 +335,17 @@
 
         Returns:
             tuple: A tuple containing two elements:
                 - int: The status code - 200 for successful execution, 500 for an error.
                 - str: The output of the command in case of success, or the error message in case of an error.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("execute_script_string"):
 
             try:
 
@@ -408,18 +408,18 @@
             print("The 'xattr' module is not supported on this operating system.")
             # Handle the case where the module is not supported on the current OS.
             return None
 
     @classmethod
     def set_file_metadata(cls, file_path, key, value):
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("set_file_metadata"):
 
             try:
                 if sys.platform.startswith('win'):
@@ -476,18 +476,18 @@
 
         Returns:
             tuple: A tuple consisting of an integer and a string.
                 The integer is the HTTP status code - 200 for a successful download, 500 for an error.
                 The string is the local file path where the file was saved in case of success, or the error message in case of an error.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("download_file"):
             try:
                 logger.info(f"download_file: {url}")
                 if local_file_name is None or local_file_name == "":
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_http.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/environment_http.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # try:
 #    response = http_util.get(url)
 #    print(response.text)
 # except Exception as e:
 #    print(f"Error occurred: {str(e)}")
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 
 import requests
 from retrying import retry
 import os
 import sys
@@ -88,18 +88,18 @@
             requests.Response: The response object.
 
         Raises:
             requests.exceptions.HTTPError: If a non-403 HTTP error occurs.
             Exception: If a 403 error occurs after retrying.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         # Counter variable to track the number of 403 errors
         error_count = 0
 
         with tracer.start_as_current_span("get"):
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         if row_user_name is not None:
             username = row_user_name["current_user"]
         else:
             username = "dataframe is empty error"
         repo = "pade"
         sys_path = str(sys.path)
         root_path = os.path.abspath(
-            f"/Workspace/Repos/{username}/{repo}/pade_python")
+            f"/Workspace/Repos/{username}/{repo}/data_ecosystem_services")
         if root_path not in sys_path:
             sys.path.append(root_path)
 
         return root_path
 
     @staticmethod
     def get_spark_home_path_local(spark_home_path: str) -> str:
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/job_core.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/job_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/cdc_tech_environment_service/repo_core.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/cdc_tech_environment_service/repo_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/github_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/github_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/github_service/github_secret.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/github_service/github_secret.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from typing import List
 import json
 from html.parser import HTMLParser  # web scraping html
 import subprocess
 import os
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
-    environment_file as pade_env_file
+    environment_file as cdc_env_file
 )
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 
@@ -53,19 +53,19 @@
 
         Raises:
             requests.exceptions.RequestException: If an error occurs while making the API request.
             KeyError: If the secret value is not found in the API response.
 
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_github_secret"):
 
             headers = {
                 "Accept": "application/vnd.github.v3+json",
@@ -119,19 +119,19 @@
         Returns:
             int, dict, str: The status code of the response, the content of the response
             as a dictionary, and the API url string respectively.
 
         Raises:
             subprocess.CalledProcessError: If an error occurs while making the API request.
         """
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         # Check if user is logged in
         try:
             subprocess.check_output(
                 ['gh', 'auth', 'status'], stderr=subprocess.STDOUT)
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/jira_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/jira_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/jira_service/jira_client.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/jira_service/jira_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import sys
 import requests
 from typing import List
 import json
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
-    environment_file as pade_env_file
+    environment_file as cdc_env_file
 )
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 
@@ -41,18 +41,18 @@
 
         Raises:
         - requests.exceptions.RequestException: If the GET request to the Jira API fails.
         - Exception: If there's a problem parsing the API response or if the response indicates a server error.
         """
 
         try:
-            logger_singleton = pade_env_logging.LoggerSingleton.instance(
+            logger_singleton = cdc_env_logging.LoggerSingleton.instance(
                 NAMESPACE_NAME, SERVICE_NAME)
             logger = logger_singleton.get_logger()
-            tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+            tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
                 NAMESPACE_NAME, SERVICE_NAME)
             tracer = tracer_singleton.get_tracer()
 
             with tracer.start_as_current_span("get_tasks"):
                 try:
                     api_path = "/rest/api/latest/search"
                     api_url = f"{jira_base_url}{api_path}"
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/posit_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/posit_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/posit_service/posit_connect.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/posit_service/posit_connect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import requests
 from typing import List
 import json
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
-    environment_file as pade_env_file
+    environment_file as cdc_env_file
 )
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
 
@@ -32,19 +32,19 @@
         Examples:
             url: 'https://dev.rconnect.edav.cdc.gov:8080"'  # replace with the actual API endpoint
 
         Returns:
             tuple: A tuple containing the status code and response_content from the server.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("verify_api_key"):
 
             headers = {"Authorization": f"Key {api_key}"}
 
@@ -79,19 +79,19 @@
         Examples:
             url: 'https://dev.rconnect.edav.cdc.gov:8080"'  # replace with the actual API endpoint
 
         Returns:
             tuple: A tuple containing the status code and response_content from the server.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("verify_api_key"):
 
             headers = {"Authorization": f"Key {api_key}"}
 
@@ -125,19 +125,19 @@
             posit_connect_base_url (str): The base URL of the platform where the application will be published.
             app_manifest_file (str): The path to the application's manifest file. This file contains metadata about the application such as its name, version, and the resources it needs.
 
         Returns:
             dict: A dictionary containing the response from the platform. This typically includes the status of the publication and any errors encountered during the process.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("publish_app"):
 
             if posit_connect_base_url.endswith('/'):
                 posit_connect_base_url = posit_connect_base_url[:-1]
@@ -178,19 +178,19 @@
             swagger_file (str): The path to the Swagger specification file. This file describes the structure of the API that the application will provide.
             requirements_file (str): The path to the requirements.txt file. This file lists the Python packages that the application requires to run.
 
         Returns:
             str: The path to the generated manifest.json file. This file includes a summary of the application's structure and dependencies.
         """
 
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("generate_manifest"):
 
             # Load the Swagger JSON file
             with open(swagger_file, "rb") as swagger_file_handle:
@@ -247,19 +247,19 @@
             api_key (str): The API key provided by the platform for authentication.
             posit_connect_base_url (str): The base URL of the platform where the application will be published.
 
         Returns:
             dict: A dictionary containing the response from the platform. This typically includes the status of the publication and any errors encountered during the process.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("list_content"):
 
             if posit_connect_base_url.endswith('/'):
                 posit_connect_base_url = posit_connect_base_url[:-1]
@@ -300,19 +300,19 @@
             api_key (str): The API key provided by the platform for authentication.
             posit_connect_base_url (str): The base URL of the platform where the application will be published.
 
         Returns:
             dict: A dictionary containing the response from the platform. This typically includes the status of the publication and any errors encountered during the process.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("list_deployment_bundles"):
 
             if posit_connect_base_url.endswith('/'):
                 posit_connect_base_url = posit_connect_base_url[:-1]
@@ -354,19 +354,19 @@
             posit_connect_base_url (str): The base URL of the platform where the application will be published.
             task_id(str):
 
         Returns:
             dict: A dictionary containing the response from the platform. This typically includes the status of the publication and any errors encountered during the process.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("get_task_details"):
 
             if posit_connect_base_url.endswith('/'):
                 posit_connect_base_url = posit_connect_base_url[:-1]
@@ -408,22 +408,22 @@
             posit_connect_base_url (str): The base URL of the platform where the application will be published.
             app_path (str): The path of the application that will be uploaded to the platform.
 
         Returns:
             dict: A dictionary containing the response from the platform. This typically includes the status of the upload and any errors encountered during the process.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
-        env_file = pade_env_file.EnvironmentFile()
+        env_file = cdc_env_file.EnvironmentFile()
 
         with tracer.start_as_current_span("generate_manifest"):
 
             if posit_connect_base_url.endswith('/'):
                 posit_connect_base_url = posit_connect_base_url[:-1]
 
             api_url = f"{posit_connect_base_url}/__api__/v1/content"
@@ -463,22 +463,22 @@
             posit_connect_base_url (str): The base URL of the platform where the application will be published.
             bundle_id (str): 
 
         Returns:
             dict: A dictionary containing the response from the platform. This typically includes the status of the upload and any errors encountered during the process.
         """
 
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        logger_singleton = cdc_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        cdc_env_tracing.TracerSingleton.log_to_console = False
+        tracer_singleton = cdc_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
-        env_file = pade_env_file.EnvironmentFile()
+        env_file = cdc_env_file.EnvironmentFile()
 
         with tracer.start_as_current_span("build_deployment_bundle"):
 
             if posit_connect_base_url.endswith('/'):
                 posit_connect_base_url = posit_connect_base_url[:-1]
 
             data = {'bundle_id': f'{bundle_id}'}
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/python_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/python_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/requirements.txt` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,177 +1,215 @@
 adal==1.2.7 ; python_version >= "3.9" and python_version < "4.0"
+aiohttp==3.8.5 ; python_version >= "3.9" and python_version < "4.0"
+aiosignal==1.3.1 ; python_version >= "3.9" and python_version < "4.0"
 alabaster==0.7.13 ; python_version >= "3.9" and python_version < "4.0"
+aniso8601==9.0.1 ; python_version >= "3.9" and python_version < "4.0"
 anyascii==0.3.2 ; python_version >= "3.9" and python_version < "4.0"
-anyio==3.7.0 ; python_version >= "3.9" and python_version < "4.0"
-appnope==0.1.3 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform == "darwin" or platform_system == "Darwin")
+anyio==3.7.1 ; python_version >= "3.9" and python_version < "4.0"
+appdirs==1.4.4 ; python_version >= "3.9" and python_version < "4.0"
+appnope==0.1.3 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "darwin" or python_version >= "3.9" and python_version < "4.0" and platform_system == "Darwin"
 argon2-cffi-bindings==21.2.0 ; python_version >= "3.9" and python_version < "4.0"
 argon2-cffi==21.3.0 ; python_version >= "3.9" and python_version < "4.0"
 arrow==1.2.3 ; python_version >= "3.9" and python_version < "4.0"
-astroid==2.15.5 ; python_version >= "3.9" and python_version < "4.0"
+astroid==2.15.6 ; python_version >= "3.9" and python_version < "4.0"
 asttokens==2.2.1 ; python_version >= "3.9" and python_version < "4.0"
+async-timeout==4.0.2 ; python_version >= "3.9" and python_version < "4.0"
 attrs==23.1.0 ; python_version >= "3.9" and python_version < "4.0"
 azure-common==1.1.28 ; python_version >= "3.9" and python_version < "4.0"
-azure-core==1.27.1 ; python_version >= "3.9" and python_version < "4.0"
+azure-core==1.28.0 ; python_version >= "3.9" and python_version < "4.0"
 azure-identity==1.13.0 ; python_version >= "3.9" and python_version < "4.0"
 azure-keyvault-certificates==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
 azure-keyvault-keys==4.8.0 ; python_version >= "3.9" and python_version < "4.0"
 azure-keyvault-secrets==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
 azure-keyvault==4.2.0 ; python_version >= "3.9" and python_version < "4.0"
 azure-mgmt-core==1.4.0 ; python_version >= "3.9" and python_version < "4.0"
 azure-mgmt-monitor==5.0.1 ; python_version >= "3.9" and python_version < "4.0"
 azure-mgmt-resource==23.0.1 ; python_version >= "3.9" and python_version < "4.0"
 azure-monitor-opentelemetry-exporter==1.0.0b14 ; python_version >= "3.9" and python_version < "4.0"
-azure-storage-blob==12.16.0 ; python_version >= "3.9" and python_version < "4.0"
-azure-storage-file-datalake==12.11.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-storage-blob==12.17.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-storage-file-datalake==12.12.0 ; python_version >= "3.9" and python_version < "4.0"
 azure-storage-queue==12.6.0 ; python_version >= "3.9" and python_version < "4.0"
 babel==2.12.1 ; python_version >= "3.9" and python_version < "4.0"
 backcall==0.2.0 ; python_version >= "3.9" and python_version < "4.0"
 beautifulsoup4==4.12.2 ; python_version >= "3.9" and python_version < "4.0"
 bleach==6.0.0 ; python_version >= "3.9" and python_version < "4.0"
+blinker==1.6.2 ; python_version >= "3.9" and python_version < "4.0"
 boto3==1.21.18 ; python_version >= "3.9" and python_version < "4.0"
 botocore==1.24.18 ; python_version >= "3.9" and python_version < "4.0"
 cachetools==5.3.1 ; python_version >= "3.9" and python_version < "4.0"
 certifi==2023.5.7 ; python_version >= "3.9" and python_version < "4.0"
 cffi==1.15.1 ; python_version >= "3.9" and python_version < "4.0"
-chardet==5.1.0 ; python_version >= "3.9" and python_version < "4.0"
+chardet==5.2.0 ; python_version >= "3.9" and python_version < "4.0"
 charset-normalizer==2.1.1 ; python_version >= "3.9" and python_version < "4.0"
-click==8.1.3 ; python_version >= "3.9" and python_version < "4.0"
-colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform == "win32" or platform_system == "Windows")
+click==8.1.6 ; python_version >= "3.9" and python_version < "4.0"
+colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "win32" or python_version >= "3.9" and python_version < "4.0" and platform_system == "Windows"
 comm==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
-cryptography==41.0.1 ; python_version >= "3.9" and python_version < "4.0"
+cryptography==41.0.3 ; python_version >= "3.9" and python_version < "4.0"
 ddlparse==1.10.0 ; python_version >= "3.9" and python_version < "4.0"
 debugpy==1.6.7 ; python_version >= "3.9" and python_version < "4.0"
 decorator==5.1.1 ; python_version >= "3.9" and python_version < "4.0"
 defusedxml==0.7.1 ; python_version >= "3.9" and python_version < "4.0"
+delta-spark==2.4.0 ; python_version >= "3.9" and python_version < "4.0"
 deprecated==1.2.14 ; python_version >= "3.9" and python_version < "4.0"
 docutils==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
 entrypoints==0.4 ; python_version >= "3.9" and python_version < "4.0"
 et-xmlfile==1.1.0 ; python_version >= "3.9" and python_version < "4.0"
-exceptiongroup==1.1.1 ; python_version >= "3.9" and python_version < "3.11"
+exceptiongroup==1.1.2 ; python_version >= "3.9" and python_version < "3.11"
 executing==1.2.0 ; python_version >= "3.9" and python_version < "4.0"
-fastjsonschema==2.17.1 ; python_version >= "3.9" and python_version < "4.0"
+fastjsonschema==2.18.0 ; python_version >= "3.9" and python_version < "4.0"
+findspark==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 fixedint==0.1.6 ; python_version >= "3.9" and python_version < "4.0"
+flake8==4.0.1 ; python_version >= "3.9" and python_version < "4.0"
+flask-jwt-extended==4.5.2 ; python_version >= "3.9" and python_version < "4"
+flask-restful==0.3.10 ; python_version >= "3.9" and python_version < "4.0"
+flask-restx==1.1.0 ; python_version >= "3.9" and python_version < "4.0"
+flask==2.3.2 ; python_version >= "3.9" and python_version < "4.0"
 fqdn==1.5.1 ; python_version >= "3.9" and python_version < "4"
+frozenlist==1.4.0 ; python_version >= "3.9" and python_version < "4.0"
+fsspec==2023.6.0 ; python_version >= "3.9" and python_version < "4.0"
 google-api-core==2.11.1 ; python_version >= "3.9" and python_version < "4.0"
-google-auth==2.20.0 ; python_version >= "3.9" and python_version < "4.0"
-googleapis-common-protos==1.59.1 ; python_version >= "3.9" and python_version < "4.0"
+google-auth==2.22.0 ; python_version >= "3.9" and python_version < "4.0"
+googleapis-common-protos==1.60.0 ; python_version >= "3.9" and python_version < "4.0"
 html2text==2020.1.16 ; python_version >= "3.9" and python_version < "4.0"
+humanize==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.9" and python_version < "4.0"
 imagesize==1.4.1 ; python_version >= "3.9" and python_version < "4.0"
 importlib-metadata==6.0.1 ; python_version >= "3.9" and python_version < "4.0"
+importlib-resources==6.0.0 ; python_version >= "3.9" and python_version < "4.0"
 iniconfig==2.0.0 ; python_version >= "3.9" and python_version < "4.0"
-ipykernel==6.23.3 ; python_version >= "3.9" and python_version < "4.0"
+ipykernel==6.25.0 ; python_version >= "3.9" and python_version < "4.0"
 ipython-genutils==0.2.0 ; python_version >= "3.9" and python_version < "4.0"
 ipython==8.14.0 ; python_version >= "3.9" and python_version < "4.0"
 isodate==0.6.1 ; python_version >= "3.9" and python_version < "4.0"
 isoduration==20.11.0 ; python_version >= "3.9" and python_version < "4.0"
-jedi==0.18.2 ; python_version >= "3.9" and python_version < "4.0"
+itsdangerous==2.1.2 ; python_version >= "3.9" and python_version < "4.0"
+jedi==0.19.0 ; python_version >= "3.9" and python_version < "4.0"
 jinja2==3.1.2 ; python_version >= "3.9" and python_version < "4.0"
 jmespath==0.10.0 ; python_version >= "3.9" and python_version < "4.0"
+joblib==1.3.1 ; python_version >= "3.9" and python_version < "4.0"
+jsondiff==2.0.0 ; python_version >= "3.9" and python_version < "4.0"
 jsonpointer==2.4 ; python_version >= "3.9" and python_version < "4.0"
-jsonschema==4.17.3 ; python_version >= "3.9" and python_version < "4.0"
-jsonschema[format-nongpl]==4.17.3 ; python_version >= "3.9" and python_version < "4.0"
-jupyter-client==8.3.0 ; python_version >= "3.9" and python_version < "4.0"
+jsonschema-specifications==2023.7.1 ; python_version >= "3.9" and python_version < "4.0"
+jsonschema==4.18.4 ; python_version >= "3.9" and python_version < "4.0"
+jsonschema[format-nongpl]==4.18.4 ; python_version >= "3.9" and python_version < "4.0"
+jupyter-client==7.4.9 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-core==5.3.1 ; python_version >= "3.9" and python_version < "4.0"
-jupyter-events==0.6.3 ; python_version >= "3.9" and python_version < "4.0"
+jupyter-events==0.7.0 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-server-terminals==0.4.4 ; python_version >= "3.9" and python_version < "4.0"
-jupyter-server==2.6.0 ; python_version >= "3.9" and python_version < "4.0"
+jupyter-server==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
 jupyterlab-pygments==0.2.2 ; python_version >= "3.9" and python_version < "4.0"
+jwcrypto==1.5.0 ; python_version >= "3.9" and python_version < "4.0"
 lazy-object-proxy==1.9.0 ; python_version >= "3.9" and python_version < "4.0"
-lxml==4.9.2 ; python_version >= "3.9" and python_version < "4.0"
+lxml==4.9.3 ; python_version >= "3.9" and python_version < "4.0"
 markdown-it-py==2.2.0 ; python_version >= "3.9" and python_version < "4.0"
-markdown==3.4.3 ; python_version >= "3.9" and python_version < "4.0"
+markdown==3.4.4 ; python_version >= "3.9" and python_version < "4.0"
 markupsafe==2.1.3 ; python_version >= "3.9" and python_version < "4.0"
 matplotlib-inline==0.1.6 ; python_version >= "3.9" and python_version < "4.0"
+mccabe==0.6.1 ; python_version >= "3.9" and python_version < "4.0"
 mdit-py-plugins==0.3.5 ; python_version >= "3.9" and python_version < "4.0"
 mdurl==0.1.2 ; python_version >= "3.9" and python_version < "4.0"
 mistune==0.8.4 ; python_version >= "3.9" and python_version < "4.0"
 msal-extensions==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
-msal==1.22.0 ; python_version >= "3.9" and python_version < "4.0"
+msal==1.23.0 ; python_version >= "3.9" and python_version < "4.0"
 msrest==0.7.1 ; python_version >= "3.9" and python_version < "4.0"
+multidict==6.0.4 ; python_version >= "3.9" and python_version < "4.0"
 myst-parser==0.18.1 ; python_version >= "3.9" and python_version < "4.0"
 nbclassic==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
 nbclient==0.8.0 ; python_version >= "3.9" and python_version < "4.0"
 nbconvert==6.5.4 ; python_version >= "3.9" and python_version < "4.0"
-nbformat==5.9.0 ; python_version >= "3.9" and python_version < "4.0"
-nest-asyncio==1.5.6 ; python_version >= "3.9" and python_version < "4.0"
+nbformat==5.9.2 ; python_version >= "3.9" and python_version < "4.0"
+nest-asyncio==1.5.7 ; python_version >= "3.9" and python_version < "4.0"
 notebook-shim==0.2.3 ; python_version >= "3.9" and python_version < "4.0"
-notebook==6.5.4 ; python_version >= "3.9" and python_version < "4.0"
-numpy==1.25.0 ; python_version >= "3.9" and python_version < "4.0"
+notebook==6.5.5 ; python_version >= "3.9" and python_version < "4.0"
+numpy==1.25.2 ; python_version >= "3.9" and python_version < "4.0"
 oauthlib==3.2.2 ; python_version >= "3.9" and python_version < "4.0"
+openai==0.27.8 ; python_version >= "3.9" and python_version < "4.0"
 opencensus-context==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
 opencensus-ext-azure==1.1.9 ; python_version >= "3.9" and python_version < "4.0"
 opencensus==0.11.2 ; python_version >= "3.9" and python_version < "4.0"
 openpyxl==3.1.2 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-api==1.18.0 ; python_version >= "3.9" and python_version < "4.0"
+opentelemetry-instrumentation-flask==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
+opentelemetry-instrumentation-wsgi==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
+opentelemetry-instrumentation==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-sdk==1.18.0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-semantic-conventions==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
+opentelemetry-util-http==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 overrides==7.3.1 ; python_version >= "3.9" and python_version < "4.0"
 packaging==23.1 ; python_version >= "3.9" and python_version < "4.0"
-pandas==2.0.2 ; python_version >= "3.9" and python_version < "4.0"
+pandas==2.0.3 ; python_version >= "3.9" and python_version < "4.0"
 pandocfilters==1.5.0 ; python_version >= "3.9" and python_version < "4.0"
 parso==0.8.3 ; python_version >= "3.9" and python_version < "4.0"
 pathlib==1.0.1 ; python_version >= "3.9" and python_version < "4.0"
 pbr==5.11.1 ; python_version >= "3.9" and python_version < "4.0"
 pexpect==4.8.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform != "win32"
 pickleshare==0.7.5 ; python_version >= "3.9" and python_version < "4.0"
+pins==0.8.1 ; python_version >= "3.9" and python_version < "4.0"
 pip-system-certs==4.0 ; python_version >= "3.9" and python_version < "4.0"
-pip==23.1.2 ; python_version >= "3.9" and python_version < "4.0"
-platformdirs==3.8.0 ; python_version >= "3.9" and python_version < "4.0"
+pip==23.2.1 ; python_version >= "3.9" and python_version < "4.0"
+platformdirs==3.10.0 ; python_version >= "3.9" and python_version < "4.0"
 pluggy==1.2.0 ; python_version >= "3.9" and python_version < "4.0"
 portalocker==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
-prometheus-client==0.17.0 ; python_version >= "3.9" and python_version < "4.0"
-prompt-toolkit==3.0.38 ; python_version >= "3.9" and python_version < "4.0"
-protobuf==4.23.3 ; python_version >= "3.9" and python_version < "4.0"
+prometheus-client==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
+prompt-toolkit==3.0.39 ; python_version >= "3.9" and python_version < "4.0"
+protobuf==4.23.4 ; python_version >= "3.9" and python_version < "4.0"
 psutil==5.9.5 ; python_version >= "3.9" and python_version < "4.0"
-ptyprocess==0.7.0 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform != "win32" or os_name != "nt")
+ptyprocess==0.7.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform != "win32" or python_version >= "3.9" and python_version < "4.0" and os_name != "nt"
 pure-eval==0.2.2 ; python_version >= "3.9" and python_version < "4.0"
+py4j==0.10.9.7 ; python_version >= "3.9" and python_version < "4.0"
+py==1.11.0 ; python_version >= "3.9" and python_version < "4.0" and implementation_name == "pypy"
 pyarrow==10.0.1 ; python_version >= "3.9" and python_version < "4.0"
 pyasn1-modules==0.3.0 ; python_version >= "3.9" and python_version < "4.0"
 pyasn1==0.5.0 ; python_version >= "3.9" and python_version < "4.0"
+pycodestyle==2.8.0 ; python_version >= "3.9" and python_version < "4.0"
 pycparser==2.21 ; python_version >= "3.9" and python_version < "4.0"
-pydash==7.0.4 ; python_version >= "3.9" and python_version < "4.0"
+pydash==7.0.6 ; python_version >= "3.9" and python_version < "4.0"
+pyflakes==2.4.0 ; python_version >= "3.9" and python_version < "4.0"
 pygments==2.15.1 ; python_version >= "3.9" and python_version < "4.0"
-pyjwt==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
-pyjwt[crypto]==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
-pyparsing==3.1.0 ; python_version >= "3.9" and python_version < "4.0"
+pyjwt==2.8.0 ; python_version >= "3.9" and python_version < "4.0"
+pyjwt[crypto]==2.8.0 ; python_version >= "3.9" and python_version < "4.0"
+pyparsing==3.1.1 ; python_version >= "3.9" and python_version < "4.0"
 pyreadstat==1.2.2 ; python_version >= "3.9" and python_version < "4.0"
-pyrsistent==0.19.3 ; python_version >= "3.9" and python_version < "4.0"
+pyspark==3.4.1 ; python_version >= "3.9" and python_version < "4.0"
 pytest==7.4.0 ; python_version >= "3.9" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.9" and python_version < "4.0"
 python-dotenv==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
 python-json-logger==2.0.7 ; python_version >= "3.9" and python_version < "4.0"
 pytz==2023.3 ; python_version >= "3.9" and python_version < "4.0"
-pywin32==306 ; python_version >= "3.9" and (sys_platform == "win32" or platform_system == "Windows") and python_version < "4.0" and (platform_python_implementation != "PyPy" or platform_system == "Windows")
-pywinpty==2.0.10 ; python_version >= "3.9" and python_version < "4.0" and os_name == "nt"
-pyyaml==6.0 ; python_version >= "3.9" and python_version < "4.0"
-pyzmq==25.1.0 ; python_version >= "3.9" and python_version < "4.0"
+pywin32==306 ; python_version >= "3.9" and sys_platform == "win32" and python_version < "4.0" and platform_python_implementation != "PyPy" or python_version >= "3.9" and platform_system == "Windows" and python_version < "4.0"
+pywinpty==2.0.11 ; python_version >= "3.9" and python_version < "4.0" and os_name == "nt"
+pyyaml==6.0.1 ; python_version >= "3.9" and python_version < "4.0"
+pyzmq==24.0.1 ; python_version >= "3.9" and python_version < "4.0"
+referencing==0.30.0 ; python_version >= "3.9" and python_version < "4.0"
 requests-oauthlib==1.3.1 ; python_version >= "3.9" and python_version < "4.0"
 requests==2.31.0 ; python_version >= "3.9" and python_version < "4.0"
+retrying==1.3.4 ; python_version >= "3.9" and python_version < "4.0"
 rfc3339-validator==0.1.4 ; python_version >= "3.9" and python_version < "4.0"
 rfc3986-validator==0.1.1 ; python_version >= "3.9" and python_version < "4.0"
-rich==13.4.2 ; python_version >= "3.9" and python_version < "4.0"
+rich==13.5.2 ; python_version >= "3.9" and python_version < "4.0"
+rpds-py==0.9.2 ; python_version >= "3.9" and python_version < "4.0"
 rsa==4.9 ; python_version >= "3.9" and python_version < "4"
 rsconnect-jupyter==1.8.0 ; python_version >= "3.9" and python_version < "4.0"
-rsconnect-python==1.17.1 ; python_version >= "3.9" and python_version < "4.0"
+rsconnect-python==1.19.1 ; python_version >= "3.9" and python_version < "4.0"
+rsconnect==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
 s3transfer==0.5.2 ; python_version >= "3.9" and python_version < "4.0"
 semver==2.13.0 ; python_version >= "3.9" and python_version < "4.0"
 send2trash==1.8.2 ; python_version >= "3.9" and python_version < "4.0"
 setuptools==65.6.3 ; python_version >= "3.9" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.9" and python_version < "4.0"
 sniffio==1.3.0 ; python_version >= "3.9" and python_version < "4.0"
 snowballstemmer==2.2.0 ; python_version >= "3.9" and python_version < "4.0"
 soupsieve==2.4.1 ; python_version >= "3.9" and python_version < "4.0"
 sphinx-autoapi==2.1.1 ; python_version >= "3.9" and python_version < "4.0"
 sphinx-autodoc-typehints==1.23.0 ; python_version >= "3.9" and python_version < "4.0"
 sphinx-markdown-builder==0.5.5 ; python_version >= "3.9" and python_version < "4.0"
 sphinx-markdown-tables==0.0.17 ; python_version >= "3.9" and python_version < "4.0"
 sphinx-rtd-theme==1.2.2 ; python_version >= "3.9" and python_version < "4.0"
 sphinx-sitemap==2.5.0 ; python_version >= "3.9" and python_version < "4.0"
-sphinx-sql==1.3.4 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-sql==1.3.5 ; python_version >= "3.9" and python_version < "4.0"
 sphinx==5.3.0 ; python_version >= "3.9" and python_version < "4.0"
 sphinxcontrib-applehelp==1.0.4 ; python_version >= "3.9" and python_version < "4.0"
 sphinxcontrib-devhelp==1.0.2 ; python_version >= "3.9" and python_version < "4.0"
 sphinxcontrib-htmlhelp==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 sphinxcontrib-jquery==4.1 ; python_version >= "3.9" and python_version < "4.0"
 sphinxcontrib-jsmath==1.0.1 ; python_version >= "3.9" and python_version < "4.0"
 sphinxcontrib-mermaid==0.7.1 ; python_version >= "3.9" and python_version < "4.0"
@@ -181,22 +219,27 @@
 style==1.1.6 ; python_version >= "3.9" and python_version < "4.0"
 terminado==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
 testresources==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 tinycss2==1.2.1 ; python_version >= "3.9" and python_version < "4.0"
 toml==0.10.2 ; python_version >= "3.9" and python_version < "4.0"
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 tornado==6.3.2 ; python_version >= "3.9" and python_version < "4.0"
+tqdm==4.65.0 ; python_version >= "3.9" and python_version < "4.0"
 traitlets==5.9.0 ; python_version >= "3.9" and python_version < "4.0"
 tryceratops==2.3.2 ; python_version >= "3.9" and python_version < "4.0"
-typing-extensions==4.6.3 ; python_version >= "3.9" and python_version < "4.0"
+typing-extensions==4.7.1 ; python_version >= "3.9" and python_version < "4.0"
 tzdata==2023.3 ; python_version >= "3.9" and python_version < "4.0"
 unify==0.5 ; python_version >= "3.9" and python_version < "4.0"
 untokenize==0.1.1 ; python_version >= "3.9" and python_version < "4.0"
 uri-template==1.3.0 ; python_version >= "3.9" and python_version < "4.0"
 urllib3==1.26.16 ; python_version >= "3.9" and python_version < "4.0"
 wcwidth==0.2.6 ; python_version >= "3.9" and python_version < "4.0"
 webcolors==1.13 ; python_version >= "3.9" and python_version < "4.0"
 webencodings==0.5.1 ; python_version >= "3.9" and python_version < "4.0"
 websocket-client==1.6.1 ; python_version >= "3.9" and python_version < "4.0"
+werkzeug==2.3.6 ; python_version >= "3.9" and python_version < "4.0"
 wrapt==1.15.0 ; python_version >= "3.9" and python_version < "4.0"
+xlsxwriter==3.1.2 ; python_version >= "3.9" and python_version < "4.0"
+xxhash==3.3.0 ; python_version >= "3.9" and python_version < "4.0"
 yapf==0.33.0 ; python_version >= "3.9" and python_version < "4.0"
-zipp==3.15.0 ; python_version >= "3.9" and python_version < "4.0"
+yarl==1.9.2 ; python_version >= "3.9" and python_version < "4.0"
+zipp==3.16.2 ; python_version >= "3.9" and python_version < "4.0"
```

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/windows_service/__init__.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/windows_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/data_ecosystem_services/windows_service/windows_credential.py` & `data_ecosystem_services-202308.0.1/data_ecosystem_services/windows_service/windows_credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from azure.storage.queue import QueueServiceClient
 from azure.identity import ClientSecretCredential
 import requests
 import win32cred
 
 from data_ecosystem_services.cdc_admin_service import (
-    environment_tracing as pade_env_tracing,
-    environment_logging as pade_env_logging
+    environment_tracing as cdc_env_tracing,
+    environment_logging as cdc_env_logging
 )
 
 from data_ecosystem_services.cdc_tech_environment_service import (
-    environment_file as pade_env_file
+    environment_file as cdc_env_file
 )
 
 import os
 
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
```

### Comparing `data_ecosystem_services-202307.0.9/license.md` & `data_ecosystem_services-202308.0.1/license.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# License
+
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

### Comparing `data_ecosystem_services-202307.0.9/pyproject.toml` & `data_ecosystem_services-202308.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,46 +15,54 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name="data_ecosystem_services"
-version="202307.0.9"
+version="202308.0.1" 
 description="Program Agnostic Data Ecosystem (PADE) - Python Services"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9"
 ]
+
+
 include = [ "readme.md",
             "license.md",
             "setup.cfg",
             "setup.py",
-            "pyproject.toml"]
+            "app.py",
+            "app_startup.py",
+            "pyproject.toml",
+            "dev_posit_manifests/*.json",
+            "dev_schema/*.xlsx",     
+            "dev_schema/*.json",
+            "ocio/ocio_pade_dev/config/config.dev.json",
+            "ocio/**/*.json" 
+]
 packages = [{include = "data_ecosystem_services"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytest = "^7.1.2"
 adal = "^1.2.7"
 azure-common = "^1.1.28"
 azure-keyvault-secrets = "^4.5.0"
-azure-identity = "^1.10.0"
 azure-storage-file-datalake = "^12.8.0"
-openpyxl = "^3.0.4"
 numpy = "^1.23.0"
 botocore = "1.24.18"
 boto3 = "1.21.18"
 setuptools = "65.6.3"
 requests = "2.31.0"
 myst-parser = "^0.18.0"
 sphinx-markdown-tables = "^0.0.17"
@@ -86,28 +94,41 @@
 jinja2 = "^3.1.2"
 opentelemetry-sdk = "^1.17.0"
 azure-monitor-opentelemetry-exporter = {version = "^1.0.0b14", allow-prereleases = true}
 azure-storage-queue = "^12.6.0"
 python-dotenv = "^1.0.0"
 azure-mgmt-resource = "^23.0.1"
 tryceratops = "^2.3.2"
-certifi = "2023.7.22"
-opentelemetry-instrumentation-flask = "^0.39b0"
-flask = "^2.3.2"
-delta-spark = "2.4.0"
+certifi = "2023.5.7"
 findspark = "^2.0.1"
 pandas = "^2.0.2"
 pyspark = "^3.4.1"
 jsondiff = "^2.0.0"
 opentelemetry-instrumentation = "^0.39b0"
 wrapt = "^1.15.0"
-xlsxwriter = "^3.1.2"
 retrying = "^1.3.4"
+delta-spark = "2.4.0"
+openai = "^0.27.8"
+azure-identity = "^1.13.0"
+rsconnect = "^0.1.3"
+rsconnect-python = "^1.17.1"
+flake8 = "^4.0.1"
+six = "^1.16.0"
+openpyxl = "^3.1.2"
+oauthlib = "^3.2.2"
+xlsxwriter = "^3.1.2"
+werkzeug = "^2.3.3"
+flask-restful = "^0.3.10"
+flask-restx = "^1.1.0"
+flask-jwt-extended = "^4.5.2"
+flask = "^2.3.2"
+opentelemetry-instrumentation-flask = "^0.39b0"
+jwcrypto = "^1.5.0"
+
 
- 
 [tool.poetry.group.unix.dependencies]
 xattr = {version = "^0.10.1", markers = "sys_platform != 'win32'"}
 
 [tool.poetry.group.windows.dependencies]
 pywin32 = { version = "*", markers = "sys_platform == 'win32'" }
 
 [tool.poetry.group.dev.dependencies]
@@ -116,14 +137,17 @@
 flake8 = "^4.0.1"
 flake8-bugbear = "^22.6.22"
 black = "^22.3.0"
 commitizen = "^2.28.0"
 python-decouple = "^3.6"
 pathlib = "^1.0.1"
 
+[tool.poetry.scripts]
+flaskapp = "data_ecosystem_services.app:app"
+
 [tool.pytest.ini_options]
 minversion="6.0"
  
 testpaths=[
     "tests",
     "pade_python/tests"
 ]
```

### Comparing `data_ecosystem_services-202307.0.9/readme.md` & `data_ecosystem_services-202308.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.9/PKG-INFO` & `data_ecosystem_services-202308.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-services
-Version: 202307.0.9
+Version: 202308.0.1
 Summary: Program Agnostic Data Ecosystem (PADE) - Python Services
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,39 +16,46 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Sphinx (>=5.2.1,<6.0.0)
 Requires-Dist: adal (>=1.2.7,<2.0.0)
 Requires-Dist: azure-common (>=1.1.28,<2.0.0)
-Requires-Dist: azure-identity (>=1.10.0,<2.0.0)
+Requires-Dist: azure-identity (>=1.13.0,<2.0.0)
 Requires-Dist: azure-keyvault (>=4.2.0,<5.0.0)
 Requires-Dist: azure-keyvault-secrets (>=4.5.0,<5.0.0)
 Requires-Dist: azure-mgmt-monitor (>=5.0.1,<6.0.0)
 Requires-Dist: azure-mgmt-resource (>=23.0.1,<24.0.0)
 Requires-Dist: azure-monitor-opentelemetry-exporter (>=1.0.0b14,<2.0.0)
 Requires-Dist: azure-storage-file-datalake (>=12.8.0,<13.0.0)
 Requires-Dist: azure-storage-queue (>=12.6.0,<13.0.0)
 Requires-Dist: boto3 (==1.21.18)
 Requires-Dist: botocore (==1.24.18)
-Requires-Dist: certifi (==2023.7.22)
+Requires-Dist: certifi (==2023.5.7)
 Requires-Dist: chardet (>=5.0.0,<6.0.0)
 Requires-Dist: delta-spark (==2.4.0)
 Requires-Dist: docutils (==0.17.1)
 Requires-Dist: findspark (>=2.0.1,<3.0.0)
+Requires-Dist: flake8 (>=4.0.1,<5.0.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: flask-jwt-extended (>=4.5.2,<5.0.0)
+Requires-Dist: flask-restful (>=0.3.10,<0.4.0)
+Requires-Dist: flask-restx (>=1.1.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsondiff (>=2.0.0,<3.0.0)
+Requires-Dist: jwcrypto (>=1.5.0,<2.0.0)
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: myst-parser (>=0.18.0,<0.19.0)
 Requires-Dist: nbconvert (>=6.5.1,<7.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
+Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: opencensus (>=0.11.0,<0.12.0)
 Requires-Dist: opencensus-ext-azure (>=1.1.7,<2.0.0)
-Requires-Dist: openpyxl (>=3.0.4,<4.0.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: opentelemetry-instrumentation (>=0.39b0,<0.40)
 Requires-Dist: opentelemetry-instrumentation-flask (>=0.39b0,<0.40)
 Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: pip-system-certs (>=4.0,<5.0)
 Requires-Dist: pyarrow (>=10.0.1,<11.0.0)
@@ -56,27 +63,31 @@
 Requires-Dist: pyreadstat (>=1.1.9,<2.0.0)
 Requires-Dist: pyspark (>=3.4.1,<4.0.0)
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: retrying (>=1.3.4,<2.0.0)
+Requires-Dist: rsconnect (>=0.1.3,<0.2.0)
 Requires-Dist: rsconnect-jupyter (>=1.6.0,<2.0.0)
+Requires-Dist: rsconnect-python (>=1.17.1,<2.0.0)
 Requires-Dist: setuptools (==65.6.3)
+Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: sphinx-autoapi (>=2.0.0,<3.0.0)
 Requires-Dist: sphinx-autodoc-typehints (>=1.19.5,<2.0.0)
 Requires-Dist: sphinx-markdown-builder (>=0.5.5,<0.6.0)
 Requires-Dist: sphinx-markdown-tables (>=0.0.17,<0.0.18)
 Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0)
 Requires-Dist: sphinx-sitemap (>=2.2.0,<3.0.0)
 Requires-Dist: sphinx-sql (>=1.3.2,<2.0.0)
 Requires-Dist: sphinxcontrib-mermaid (>=0.7.1,<0.8.0)
 Requires-Dist: style (>=1.1.6,<2.0.0)
 Requires-Dist: testresources (>=2.0.1,<3.0.0)
 Requires-Dist: tryceratops (>=2.3.2,<3.0.0)
+Requires-Dist: werkzeug (>=2.3.3,<3.0.0)
 Requires-Dist: wrapt (>=1.15.0,<2.0.0)
 Requires-Dist: xlsxwriter (>=3.1.2,<4.0.0)
 Project-URL: Repository, https://github.com/cdcent/data-ecosystem-services
 Description-Content-Type: text/markdown
 
 # PADE-Python Project Documentation
```

