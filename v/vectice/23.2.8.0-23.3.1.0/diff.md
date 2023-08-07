# Comparing `tmp/vectice-23.2.8.0.tar.gz` & `tmp/vectice-23.3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sdk-python/sdk-python/dist/.tmp-_fe4i8zn/vectice-23.2.8.0.tar", last modified: Thu Jul 27 12:05:24 2023, max compression
+gzip compressed data, was "/home/runner/work/sdk-python/sdk-python/dist/.tmp-7d4raw3o/vectice-23.3.1.0.tar", last modified: Mon Aug  7 13:46:37 2023, max compression
```

## Comparing `vectice-23.2.8.0.tar` & `vectice-23.3.1.0.tar`

### file list

```diff
@@ -1,136 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 12:05:15.000000 vectice-23.2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-27 12:05:24.000000 vectice-23.2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 12:05:15.000000 vectice-23.2.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-27 12:05:15.000000 vectice-23.2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 12:05:24.000000 vectice-23.2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-27 12:05:15.000000 vectice-23.2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/user_declared_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/git_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/databricks_table_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/automatic_link_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 12:05:15.000000 vectice-23.2.8.0/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 12:05:24.000000 vectice-23.2.8.0/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:37.000000 vectice-23.3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-07 13:46:27.000000 vectice-23.3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-07 13:46:37.000000 vectice-23.3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:46:27.000000 vectice-23.3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-07 13:46:27.000000 vectice-23.3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-07 13:46:37.000000 vectice-23.3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-07 13:46:27.000000 vectice-23.3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20002 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/gql_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/gql_code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/user_declared_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21597 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/git_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/model_exp_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/model_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29596 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/utils/automatic_link_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-07 13:46:27.000000 vectice-23.3.1.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 13:46:37.000000 vectice-23.3.1.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-23.2.8.0/LICENSE` & `vectice-23.3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/PKG-INFO` & `vectice-23.3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.8.0
+Version: 23.3.1.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.8.0/setup.py` & `vectice-23.3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
             "coverage",
             "pytest-cov",
             "scikit-learn",
             "testcontainers",
             "testbook",
             "db-dtypes>=1.1.1",
             "pyspark",
+            "mlflow<=1.30.1",
             "Cython<3.0",
             "pyyaml==5.3.1",
         ],
         "gcs": ["google-cloud-storage>=1.17.0", "google-cloud-bigquery"],
         "s3": ["boto3"],
     },
     classifiers=[
```

### Comparing `vectice-23.2.8.0/src/vectice/__init__.py` & `vectice-23.3.1.0/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/__init__.py` & `vectice-23.3.1.0/src/vectice/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/_auth.py` & `vectice-23.3.1.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/attachment.py` & `vectice-23.3.1.0/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/client.py` & `vectice-23.3.1.0/src/vectice/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,22 +38,24 @@
 from vectice.api.json.dataset_register import DatasetRegisterInput, DatasetRegisterOutput
 from vectice.api.json.dataset_representation import DatasetRepresentationOutput
 from vectice.api.json.dataset_version import DatasetVersionOutput
 from vectice.api.json.dataset_version_representation import DatasetVersionRepresentationOutput
 from vectice.api.json.iteration import IterationStatus
 from vectice.api.json.metric import MetricInput
 from vectice.api.json.model_representation import ModelRepresentationOutput
-from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput
+from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput, ModelVersionUpdateInput
 from vectice.api.json.organization_config import OrgConfigOutput
 from vectice.api.phase import PhaseApi
 from vectice.api.project import ProjectApi
 from vectice.api.step import StepApi
 from vectice.api.version import VersionApi
 from vectice.api.workspace import WorkspaceApi
 from vectice.models.dataset import Dataset
+from vectice.models.iteration import Iteration
+from vectice.models.phase import Phase
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.representation.model_version_representation import ModelVersionRepresentation
 from vectice.models.resource.metadata.base import MetadataSettings
 from vectice.utils.vectice_ids_regex import WORKSPACE_VID_REG
 
 if TYPE_CHECKING:
     from io import BytesIO, IOBase
@@ -367,14 +369,17 @@
 
     def get_model(self, id: str) -> ModelRepresentationOutput:
         return GqlModelApi(self._gql_client, self.auth).get_model(id)
 
     def get_model_version(self, id: str) -> ModelVersionRepresentationOutput:
         return GqlModelApi(self._gql_client, self.auth).get_model_version(id)
 
+    def update_model(self, model_version_id: str, model: ModelVersionUpdateInput):
+        GqlModelApi(self._gql_client, self.auth).update_model(model_version_id, model)
+
     @staticmethod
     def get_dataset_name(dataset: Dataset) -> str:
         return f"dataset {datetime.time}" if dataset.name is None else dataset.name
 
     @staticmethod
     def get_derived_from(obj: Dataset | Model) -> list[str]:
         return [] if obj.derived_from is None else obj.derived_from
@@ -394,56 +399,58 @@
             f"name='{dataset_register_input.name}', "
             f"id={data['datasetVersion']['vecticeId']}, "
             f"version='{data['datasetVersion']['name']}', "
             f"type={dataset_register_input.type})."
         )
         return data
 
-    @staticmethod
-    def _get_model_name(library: str, technique: str, name: str | None = None) -> str:
-        return name if name else f"{library} {technique} model"
-
     def register_model(
         self,
         model: Model,
         project_id: str,
-        phase_id: str | None = None,
-        iteration_id: str | None = None,
+        phase: Phase,
+        iteration: Iteration,
         code_version_id: int | None = None,
     ) -> ModelRegisterOutput:
         """Register a model.
 
         Parameters:
             model: The model to register
             project_id: The project ID
-            phase_id: The phase ID
-            iteration_id: The iteration ID
+            phase: The phase
+            iteration: The iteration
             code_version_id: The code version ID
 
         Returns:
             The registered model.
         """
+        ff = "mlflow"
+        is_ff_enabled = self.is_feature_flag_enabled(ff)
+        if model.additional_info is not None and is_ff_enabled is False:
+            raise VecticeException(DISABLED_FEATURE_FLAG_MESSAGE.format(ff))
+
         metrics = [vars(MetricInput(metric.key, metric.value)) for metric in model.metrics] if model.metrics else None
         properties = (
             [vars(PropertyInput(prop.key, prop.value)) for prop in model.properties] if model.properties else None
         )
         derived_from = self.get_derived_from(model)
         model_register_input = ModelRegisterInput(
-            name=model.name,
+            name=(model.name or f"{phase.name} {iteration.index} model")[:60],
             modelType=ModelType.OTHER.value,
             status=ModelVersionStatus.EXPERIMENTATION.value,
             inputs=derived_from,
             metrics=metrics,
             properties=properties,
             algorithmName=model.technique,
             framework=model.library,
             codeVersionId=code_version_id,
+            context=model.additional_info.asdict() if model.additional_info is not None else None,
         )
         return GqlModelApi(self._gql_client, self.auth).register_model(
-            model_register_input, project_id, phase_id, iteration_id
+            model_register_input, project_id, phase.id, iteration.id
         )
 
     def get_user_and_default_workspace(self):
         return UserAndDefaultWorkspaceApi(self._gql_client, self.auth).get_user_and_default_workspace()
 
     def create_code_gql(self, project_id: str, code: CodeInput):
         return GqlCodeApi(self._gql_client, self.auth).create_code(project_id, code)
```

### Comparing `vectice-23.2.8.0/src/vectice/api/gql_api.py` & `vectice-23.3.1.0/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/gql_code.py` & `vectice-23.3.1.0/src/vectice/api/gql_code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/gql_code_version.py` & `vectice-23.3.1.0/src/vectice/api/gql_code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/gql_dataset.py` & `vectice-23.3.1.0/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/gql_entity_file.py` & `vectice-23.3.1.0/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/gql_feature_flag.py` & `vectice-23.3.1.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/gql_model.py` & `vectice-23.3.1.0/src/vectice/api/gql_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING
 
 from gql import gql
 from gql.transport.exceptions import TransportQueryError
 
 from vectice.api.gql_api import GqlApi, Parser
 from vectice.api.json.model_representation import ModelRepresentationOutput
-from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput
+from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput, ModelVersionUpdateInput
 
 if TYPE_CHECKING:
     from vectice.api.json.model_register import ModelRegisterInput, ModelRegisterOutput
 
 _RETURNS = """
             modelVersion{
                           vecticeId
@@ -67,14 +67,19 @@
                 project {
                     vecticeId
                 }
             }
             __typename
 """
 
+_RETURNS_MODEL_UPDATE = """
+            vecticeId
+            __typename
+"""
+
 
 class GqlModelApi(GqlApi):
     def get_model(self, id: str) -> ModelRepresentationOutput:
         variable_types = "$modelId:VecticeId!"
         kw = "modelId:$modelId"
         variables = {"modelId": id}
         query = GqlApi.build_query(
@@ -138,7 +143,24 @@
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
             model_output: ModelRegisterOutput = Parser().parse_item(response[query_name])
             return model_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "model", "register model")
+
+    def update_model(self, model_version_id: str, model: ModelVersionUpdateInput):
+        variable_types = "$modelVersionId:VecticeId!,$data:ModelVersionUpdateInput!"
+        kw = "modelVersionId:$modelVersionId,data:$data"
+        variables = {"modelVersionId": model_version_id, "data": model}
+        query = GqlApi.build_query(
+            gql_query="updateModelVersion",
+            variable_types=variable_types,
+            returns=_RETURNS_MODEL_UPDATE,
+            keyword_arguments=kw,
+            query=False,
+        )
+        query_built = gql(query)
+        try:
+            self.execute(query_built, variables)
+        except TransportQueryError as e:
+            self._error_handler.handle_post_gql_error(e, "model", "put")
```

### Comparing `vectice-23.2.8.0/src/vectice/api/gql_organization.py` & `vectice-23.3.1.0/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/gql_user_workspace_api.py` & `vectice-23.3.1.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/http_error.py` & `vectice-23.3.1.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/http_error_handlers.py` & `vectice-23.3.1.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/iteration.py` & `vectice-23.3.1.0/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/__init__.py` & `vectice-23.3.1.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/artifact_version.py` & `vectice-23.3.1.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/code.py` & `vectice-23.3.1.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/code_version.py` & `vectice-23.3.1.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/dataset_register.py` & `vectice-23.3.1.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/dataset_representation.py` & `vectice-23.3.1.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/dataset_version.py` & `vectice-23.3.1.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/dataset_version_representation.py` & `vectice-23.3.1.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/files_metadata.py` & `vectice-23.3.1.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/iteration.py` & `vectice-23.3.1.0/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/last_assets.py` & `vectice-23.3.1.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/metric.py` & `vectice-23.3.1.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/model.py` & `vectice-23.3.1.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/model_register.py` & `vectice-23.3.1.0/src/vectice/api/json/model_register.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,25 +61,39 @@
     @property
     def status(self) -> ModelVersionStatus:
         from vectice.api.json.model_version import ModelVersionStatus
 
         return ModelVersionStatus(self["status"])
 
     @property
-    def framework(self) -> str:
+    def framework(self) -> str | None:
         return str(self["framework"])
 
     @property
     def type(self) -> str:
         return str(self["type"])
 
     @property
-    def algorithm_name(self) -> str:
+    def algorithm_name(self) -> str | None:
         return str(self["algorithmName"])
 
     @property
     def uri(self) -> str:
         return str(self["uri"])
 
     @property
     def derived_from(self) -> list[int]:
         return [(self["inputs"])]
+
+    @property
+    def context(self) -> ModelVersionContextInput:
+        return ModelVersionContextInput(self["context"])
+
+
+class ModelVersionContextInput(dict):
+    @property
+    def url(self) -> str:
+        return str(self["url"])
+
+    @property
+    def run(self) -> str:
+        return str(self["run"])
```

### Comparing `vectice-23.2.8.0/src/vectice/api/json/model_representation.py` & `vectice-23.3.1.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/model_version.py` & `vectice-23.3.1.0/src/vectice/api/json/model_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 class ModelVersionStatus(Enum):
     """Enumeration of the different model statuses."""
 
     EXPERIMENTATION = "EXPERIMENTATION"
     STAGING = "STAGING"
     PRODUCTION = "PRODUCTION"
+    RETIRED = "RETIRED"
 
 
 class ModelVersionInput(dict):
     def items(self):
         result = []
         for key in self:
             if self[key] is not None:
```

### Comparing `vectice-23.2.8.0/src/vectice/api/json/model_version_representation.py` & `vectice-23.3.1.0/src/vectice/api/json/model_version_representation.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 from vectice.api._utils import read_nodejs_date
 from vectice.api.json.model_version import ModelVersionStatus
 
 if TYPE_CHECKING:
     from datetime import datetime
 
 
+class ModelVersionUpdateInput(dict):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    @property
+    def status(self) -> ModelVersionStatus:
+        return ModelVersionStatus[str(self["status"])]
+
+
 class ModelVersionRepresentationOutput(dict):
     @property
     def created_date(self) -> datetime | None:
         return read_nodejs_date(str(self["createdDate"]))
 
     @property
     def updated_date(self) -> datetime | None:
```

### Comparing `vectice-23.2.8.0/src/vectice/api/json/paged_response.py` & `vectice-23.3.1.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/phase.py` & `vectice-23.3.1.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/project.py` & `vectice-23.3.1.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/property.py` & `vectice-23.3.1.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/public_config.py` & `vectice-23.3.1.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/step.py` & `vectice-23.3.1.0/src/vectice/api/json/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/json/workspace.py` & `vectice-23.3.1.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/phase.py` & `vectice-23.3.1.0/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/project.py` & `vectice-23.3.1.0/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/rest_api.py` & `vectice-23.3.1.0/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/step.py` & `vectice-23.3.1.0/src/vectice/api/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/version.py` & `vectice-23.3.1.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/api/workspace.py` & `vectice-23.3.1.0/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/connection.py` & `vectice-23.3.1.0/src/vectice/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,15 +413,15 @@
             f"""
                 Model {output.name!r} successfully retrieved."
 
                 For quick access to the Model in the Vectice web app, visit:
                 {self._client.auth._API_BASE_URL}/browse/model/{output.id}"""
         ).lstrip()
         _logger.info(logging_output)
-        return ModelRepresentation(output)
+        return ModelRepresentation(output, client=self._client)
 
     def model_version(self, version: str) -> ModelVersionRepresentation:
         """Get a model version.
 
         Parameters:
             version: The id of the desired model version.
 
@@ -435,15 +435,15 @@
             f"""
                 Model version {output.name!r} successfully retrieved."
 
                 For quick access to the Model version in the Vectice web app, visit:
                 {self._client.auth._API_BASE_URL}/browse/modelversion/{output.id}"""
         ).lstrip()
         _logger.info(logging_output)
-        return ModelVersionRepresentation(output)
+        return ModelVersionRepresentation(output, client=self._client)
 
     def list_workspaces(self) -> None:
         """Prints a list of workspaces in a tabular format, limited to the first 10 items. A link is provided to view the remaining workspaces.
 
         Returns:
             None
         """
@@ -477,24 +477,14 @@
         _temp_print(link)
 
     @staticmethod
     def _get_host(config: str | None) -> str:
         try:
             return Connection._get_config_item("VECTICE_HOST", config)
         except ValueError:
-            # To remove in 23.3.1.0
-            try:
-                host = Connection._get_config_item("VECTICE_API_ENDPOINT", config)
-                _logger.warning(
-                    "VECTICE_API_ENDPOINT is deprecated and will be removed in 23.3.1.0, please use VECTICE_HOST instead."
-                )
-                return host
-            except ValueError:
-                pass
-
             _logger.debug(f"No VECTICE_HOST provided. Using default host {DEFAULT_HOST}")
             return DEFAULT_HOST
 
     @staticmethod
     def _get_api_token(host: str, config: str | None) -> str:
         try:
             return Connection._get_config_item("VECTICE_API_TOKEN", config)
```

### Comparing `vectice-23.2.8.0/src/vectice/models/__init__.py` & `vectice-23.3.1.0/src/vectice/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from vectice.models.additional_info import AdditionalInfo, ExtraInfo, Framework
 from vectice.models.attachment_container import AttachmentContainer
 from vectice.models.errors import VecticeError
 from vectice.models.git_version import CodeSource
 from vectice.models.iteration import Iteration
 from vectice.models.metric import Metric
 from vectice.models.phase import Phase
 from vectice.models.project import Project
@@ -18,8 +19,11 @@
     "Project",
     "VecticeError",
     "Workspace",
     "Phase",
     "Step",
     "Iteration",
     "CodeSource",
+    "AdditionalInfo",
+    "ExtraInfo",
+    "Framework",
 ]
```

### Comparing `vectice-23.2.8.0/src/vectice/models/attachment_container.py` & `vectice-23.3.1.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/dataset.py` & `vectice-23.3.1.0/src/vectice/models/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
         Returns:
             The dataset's name.
         """
         return self._name
 
     @name.setter
-    def name(self, name):
+    def name(self, name: str):
         """Set the dataset's name.
 
         Parameters:
             name: The name of the dataset.
         """
         self._name = name
```

### Comparing `vectice-23.2.8.0/src/vectice/models/git_version.py` & `vectice-23.3.1.0/src/vectice/models/git_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/iteration.py` & `vectice-23.3.1.0/src/vectice/models/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/metric.py` & `vectice-23.3.1.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/phase.py` & `vectice-23.3.1.0/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/project.py` & `vectice-23.3.1.0/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/property.py` & `vectice-23.3.1.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/representation/dataset_representation.py` & `vectice-23.3.1.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/__init__.py` & `vectice-23.3.1.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/base.py` & `vectice-23.3.1.0/src/vectice/models/resource/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/bigquery_resource.py` & `vectice-23.3.1.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/databricks_table_resource.py` & `vectice-23.3.1.0/src/vectice/models/resource/databricks_table_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/description.py` & `vectice-23.3.1.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/file_resource.py` & `vectice-23.3.1.0/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/gcs_resource.py` & `vectice-23.3.1.0/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/__init__.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/base.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from typing import Union
 
 from pandas.core.frame import DataFrame as PandasDF
 
 from vectice.models.resource.metadata.df_wrapper_resource import DataFrameWrapper
 
 try:
-    from pyspark.pandas.frame import DataFrame as PysparkPandasDF
     from pyspark.sql.dataframe import DataFrame as SparkDF
 
-    DataFramePandasType = Union[PysparkPandasDF, PandasDF]
+    try:
+        from pyspark.pandas.frame import DataFrame as PysparkPandasDF
+
+        DataFramePandasType = Union[PysparkPandasDF, PandasDF]
+    except ImportError:
+        DataFramePandasType = PandasDF  # type: ignore
+
     DataFrameTypeWithoutWrapper = Union[DataFramePandasType, SparkDF]
     DataFrameType = Union[DataFrameTypeWithoutWrapper, DataFrameWrapper]
 
 except ImportError:
     DataFramePandasType = PandasDF  # type: ignore
     DataFrameType = Union[DataFramePandasType, DataFrameWrapper]  # type: ignore
```

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_resource.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/df_wrapper_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/metadata/source.py` & `vectice-23.3.1.0/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/resource/s3_resource.py` & `vectice-23.3.1.0/src/vectice/models/resource/s3_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from vectice.models.resource.base import Resource
 from vectice.models.resource.metadata.base import DatasetSourceOrigin
 from vectice.models.resource.metadata.dataframe_config import DataFrameType
 from vectice.models.resource.metadata.files_metadata import File, FilesMetadata
 
 if TYPE_CHECKING:
-    from mypy_boto3_s3 import Client
+    from mypy_boto3_s3.client import S3Client as Client
     from mypy_boto3_s3.type_defs import ListObjectsV2OutputTypeDef, ObjectTypeDef
 
 
 S3_URI_REG = r"(s3:\/\/)([^\/]+)\/(.+)"
 
 
 _logger = logging.getLogger(__name__)
```

### Comparing `vectice-23.2.8.0/src/vectice/models/step.py` & `vectice-23.3.1.0/src/vectice/models/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,16 +155,16 @@
             or isinstance(value, ModelVersionRepresentation)
         ):
             if isinstance(value, Model):
                 code_version_id = self._get_code_version_id()
                 model_data = self._client.register_model(
                     model=value,
                     project_id=self.project.id,
-                    phase_id=self.phase.id,
-                    iteration_id=self.iteration.id,
+                    phase=self.phase,
+                    iteration=self.iteration,
                     code_version_id=code_version_id,
                 )
                 attachments_output = self._set_model_attachments(value, model_data.model_version)
                 model_artifact = IterationStepArtifact(
                     modelVersionId=model_data["modelVersion"]["vecticeId"], type="ModelVersion"
                 )
             elif isinstance(value, ModelRepresentation):
@@ -370,16 +370,16 @@
         ):
             data: dict[str, Any] = {}
             if isinstance(value, Model):
                 code_version_id = self._get_code_version_id()
                 data = self._client.register_model(
                     model=value,
                     project_id=self.project.id,
-                    phase_id=self.phase.id,
-                    iteration_id=self.iteration.id,
+                    phase=self.phase,
+                    iteration=self.iteration,
                     code_version_id=code_version_id,
                 )
                 attachments_output = self._set_model_attachments(value, data.model_version)
             elif isinstance(value, ModelRepresentation):
                 data = {
                     "useExistingModel": True,
                     "modelVersion": {"vecticeId": value.version.id, "name": value.version.name},
```

### Comparing `vectice-23.2.8.0/src/vectice/models/step_dataset.py` & `vectice-23.3.1.0/src/vectice/models/step_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/step_image.py` & `vectice-23.3.1.0/src/vectice/models/step_image.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/step_model.py` & `vectice-23.3.1.0/src/vectice/models/step_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/step_number.py` & `vectice-23.3.1.0/src/vectice/models/step_number.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/step_string.py` & `vectice-23.3.1.0/src/vectice/models/step_string.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/models/workspace.py` & `vectice-23.3.1.0/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/utils/automatic_link_utils.py` & `vectice-23.3.1.0/src/vectice/utils/automatic_link_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/utils/common_utils.py` & `vectice-23.3.1.0/src/vectice/utils/common_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         check_path = Path(path).exists()
     except OSError:
         return False
     _, ext = os.path.splitext(path)
     pillow_extensions = {exten for exten in Image.registered_extensions()}
     if not check_path and ext in pillow_extensions:
         raise ValueError("Check the image path.")
-    if not check_path and ext not in pillow_extensions:
+    if ext not in pillow_extensions:
         return False
     return True
 
 
 def _validate_image(path: str) -> BufferedReader:
     try:
         return open(path, "rb")
```

### Comparing `vectice-23.2.8.0/src/vectice/utils/configuration.py` & `vectice-23.3.1.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/utils/deprecation.py` & `vectice-23.3.1.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/utils/last_assets.py` & `vectice-23.3.1.0/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice/utils/logging_utils.py` & `vectice-23.3.1.0/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.8.0/src/vectice.egg-info/PKG-INFO` & `vectice-23.3.1.0/src/vectice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.8.0
+Version: 23.3.1.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.8.0/src/vectice.egg-info/SOURCES.txt` & `vectice-23.3.1.0/src/vectice.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,21 +65,24 @@
 src/vectice/api/json/property.py
 src/vectice/api/json/public_config.py
 src/vectice/api/json/step.py
 src/vectice/api/json/user_and_workspace.py
 src/vectice/api/json/user_declared_version.py
 src/vectice/api/json/workspace.py
 src/vectice/models/__init__.py
+src/vectice/models/additional_info.py
 src/vectice/models/attachment_container.py
 src/vectice/models/dataset.py
 src/vectice/models/errors.py
 src/vectice/models/git_version.py
 src/vectice/models/iteration.py
 src/vectice/models/metric.py
 src/vectice/models/model.py
+src/vectice/models/model_exp_tracker.py
+src/vectice/models/model_mlflow.py
 src/vectice/models/phase.py
 src/vectice/models/project.py
 src/vectice/models/property.py
 src/vectice/models/step.py
 src/vectice/models/step_dataset.py
 src/vectice/models/step_image.py
 src/vectice/models/step_model.py
```

### Comparing `vectice-23.2.8.0/src/vectice.egg-info/requires.txt` & `vectice-23.3.1.0/src/vectice.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -48,9 +48,10 @@
 coverage
 pytest-cov
 scikit-learn
 testcontainers
 testbook
 db-dtypes>=1.1.1
 pyspark
+mlflow<=1.30.1
 Cython<3.0
 pyyaml==5.3.1
```

