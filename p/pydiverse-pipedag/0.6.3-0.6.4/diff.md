# Comparing `tmp/pydiverse_pipedag-0.6.3.tar.gz` & `tmp/pydiverse_pipedag-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse_pipedag-0.6.3.tar", max compression
+gzip compressed data, was "pydiverse_pipedag-0.6.4.tar", max compression
```

## Comparing `pydiverse_pipedag-0.6.3.tar` & `pydiverse_pipedag-0.6.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1517 2023-07-25 13:13:25.440146 pydiverse_pipedag-0.6.3/LICENSE
--rw-r--r--   0        0        0     6174 2023-07-25 13:13:25.440146 pydiverse_pipedag-0.6.3/docs/package/README.md
--rw-r--r--   0        0        0     3421 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      435 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      857 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       97 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     5348 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0      393 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/__init__.py
--rw-r--r--   0        0        0     6097 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/base.py
--rw-r--r--   0        0        0    13599 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/database.py
--rw-r--r--   0        0        0     2756 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/filelock.py
--rw-r--r--   0        0        0      769 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/nolock.py
--rw-r--r--   0        0        0     3983 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/zookeeper.py
--rw-r--r--   0        0        0      233 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    23394 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0      108 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/cache/__init__.py
--rw-r--r--   0        0        0     3106 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/cache/base.py
--rw-r--r--   0        0        0     6976 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/cache/parquet.py
--rw-r--r--   0        0        0     6933 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0      141 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/__init__.py
--rw-r--r--   0        0        0    36934 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/ddl.py
--rw-r--r--   0        0        0      187 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
--rw-r--r--   0        0        0     1508 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
--rw-r--r--   0        0        0     3301 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
--rw-r--r--   0        0        0     9235 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
--rw-r--r--   0        0        0     3956 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
--rw-r--r--   0        0        0    21490 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/hooks.py
--rw-r--r--   0        0        0     4250 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/reflection.py
--rw-r--r--   0        0        0    47189 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/sql.py
--rw-r--r--   0        0        0       81 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     8579 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/util/dtype.py
--rw-r--r--   0        0        0      433 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0     9874 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    26325 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      311 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0    14956 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/config.py
--rw-r--r--   0        0        0    20430 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     4294 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     7789 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     8013 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      368 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      654 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     3133 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/dask.py
--rw-r--r--   0        0        0     7269 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1388 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1079 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/__init__.py
--rw-r--r--   0        0        0      620 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/cli.py
--rw-r--r--   0        0        0        0 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/commands/__init__.py
--rw-r--r--   0        0        0     1741 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/commands/clear_metadata.py
--rw-r--r--   0        0        0     2744 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/commands/delete_schemas.py
--rw-r--r--   0        0        0      182 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     9114 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0    11169 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0    17639 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     2074 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    19431 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0      213 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0     2061 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1435 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      944 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1129 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/hashing.py
--rw-r--r--   0        0        0     3736 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     7992 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0     4400 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/json.py
--rw-r--r--   0        0        0     1377 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     2847 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/structlog.py
--rw-r--r--   0        0        0     7911 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-08-07 09:33:24.796166 pydiverse_pipedag-0.6.4/LICENSE
+-rw-r--r--   0        0        0     6174 2023-08-07 09:33:24.796166 pydiverse_pipedag-0.6.4/docs/package/README.md
+-rw-r--r--   0        0        0     3421 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      435 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      857 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       97 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     5348 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0      393 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/lock/__init__.py
+-rw-r--r--   0        0        0     6097 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/lock/base.py
+-rw-r--r--   0        0        0    13599 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/lock/database.py
+-rw-r--r--   0        0        0     2756 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/lock/filelock.py
+-rw-r--r--   0        0        0      769 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/lock/nolock.py
+-rw-r--r--   0        0        0     3983 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/lock/zookeeper.py
+-rw-r--r--   0        0        0      233 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    24630 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0      108 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/cache/__init__.py
+-rw-r--r--   0        0        0     3273 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/cache/base.py
+-rw-r--r--   0        0        0     6876 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/cache/parquet.py
+-rw-r--r--   0        0        0     6757 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0      141 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/__init__.py
+-rw-r--r--   0        0        0    36934 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/ddl.py
+-rw-r--r--   0        0        0      187 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
+-rw-r--r--   0        0        0     1508 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
+-rw-r--r--   0        0        0     3301 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
+-rw-r--r--   0        0        0     9235 2023-08-07 09:33:24.800166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
+-rw-r--r--   0        0        0     3864 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
+-rw-r--r--   0        0        0    20780 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/hooks.py
+-rw-r--r--   0        0        0     4250 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/reflection.py
+-rw-r--r--   0        0        0    47198 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/sql.py
+-rw-r--r--   0        0        0       81 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     8579 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/util/dtype.py
+-rw-r--r--   0        0        0      433 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0    10113 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    27362 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      311 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0    14956 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/core/config.py
+-rw-r--r--   0        0        0    20402 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     4294 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     7789 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     8245 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      368 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      654 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     3133 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/engine/dask.py
+-rw-r--r--   0        0        0     7269 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1388 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1079 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/management/__init__.py
+-rw-r--r--   0        0        0      620 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/management/cli.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/management/commands/__init__.py
+-rw-r--r--   0        0        0     1741 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/management/commands/clear_metadata.py
+-rw-r--r--   0        0        0     2744 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/management/commands/delete_schemas.py
+-rw-r--r--   0        0        0      182 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     1642 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0    11169 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0    21462 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     2074 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    19682 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0      213 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0     2061 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1435 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      944 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     1129 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/hashing.py
+-rw-r--r--   0        0        0     3736 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     7992 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0     4444 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/json.py
+-rw-r--r--   0        0        0     1377 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     2847 2023-08-07 09:33:24.804166 pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/structlog.py
+-rw-r--r--   0        0        0     7911 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.6.4/PKG-INFO
```

### Comparing `pydiverse_pipedag-0.6.3/LICENSE` & `pydiverse_pipedag-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/docs/package/README.md` & `pydiverse_pipedag-0.6.4/docs/package/README.md`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/pyproject.toml` & `pydiverse_pipedag-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.6.3"
+version = "0.6.4"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/_typing.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/blob.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/blob.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/base.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/lock/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/database.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/lock/database.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/filelock.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/nolock.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/lock/nolock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/zookeeper.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/lock/zookeeper.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from typing import TYPE_CHECKING, Any, Generic
 
 import structlog
 from typing_extensions import Self
 
 from pydiverse.pipedag._typing import T, TableHookResolverT
 from pydiverse.pipedag.context import RunContext, TaskContext
-from pydiverse.pipedag.materialize.cache import CacheManager
+from pydiverse.pipedag.errors import CacheError
+from pydiverse.pipedag.materialize.cache import TaskCacheInfo, lazy_table_cache_key
 from pydiverse.pipedag.materialize.container import RawSql, Table
 from pydiverse.pipedag.materialize.metadata import (
     LazyTableMetadata,
     RawSqlMetadata,
     TaskMetadata,
 )
 from pydiverse.pipedag.util import Disposable, requires
 from pydiverse.pipedag.util.hashing import stable_hash
 
 if TYPE_CHECKING:
     from pydiverse.pipedag import Stage
     from pydiverse.pipedag.backend.table.cache.base import BaseTableCache
-    from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
+    from pydiverse.pipedag.materialize.core import MaterializingTask
 
 
 class TableHookResolver:
     _registered_table_hooks: list[type[TableHook]] = []
     _m_hook_cache: dict[type, type[TableHook]] = {}
     _r_hook_cache: dict[type, type[TableHook]] = {}
     _hook_subclass_cache: dict[type, type[TableHook]] = {}
@@ -127,20 +128,15 @@
         for hook in self.__registered_tables():
             if issubclass(hook, type_):
                 self._hook_subclass_cache[type_] = hook
                 return hook
 
         return type_
 
-    def store_table(
-        self,
-        table: Table,
-        task: MaterializingTask | None,
-        task_info: TaskInfo | None,
-    ):
+    def store_table(self, table: Table, task: MaterializingTask | None):
         """Stores a table in the associated transaction stage
 
         The store must convert the table object (`table.obj`) to the correct
         internal type. This means, that in some cases it first has to
         evaluate a lazy object. For example: if a sql based table store
         receives a sql query to store, it has to execute it first.
 
@@ -151,15 +147,15 @@
         # In case of deferred operations, inform run context that stage
         # isn't 100% cache valid anymore.
         if task is not None:
             RunContext.get().set_stage_has_changed(task.stage)
 
         # Materialize
         hook = self.get_m_table_hook(type(table.obj))
-        hook.materialize(self, table, table.stage.transaction_name, task_info)
+        hook.materialize(self, table, table.stage.transaction_name)
 
     def retrieve_table_obj(
         self,
         table: Table,
         as_type: type[T],
     ) -> T:
         """Loads a table from the store
@@ -249,23 +245,18 @@
 
         Additionally, the metadata associated with the transaction schema should
         replace the metadata of the base schema. The latter can be discarded.
         """
 
     # Materialize
 
-    def store_table(
-        self,
-        table: Table,
-        task: MaterializingTask | None,
-        task_info: TaskInfo | None,
-    ):
-        super().store_table(table, task, task_info)
+    def store_table(self, table: Table, task: MaterializingTask | None):
+        super().store_table(table, task)
         if self.local_table_cache:
-            self.local_table_cache.store_table(table, task, task_info)
+            self.local_table_cache.store_table(table, task)
 
     def execute_raw_sql(self, raw_sql: RawSql):
         """Executed raw SQL statements in the associated transaction stage
 
         This method is overridden by actual table stores that can handle raw SQL.
         """
 
@@ -273,101 +264,139 @@
             "This table store does not support executing raw sql statements"
         )
 
     def store_table_lazy(
         self,
         table: Table,
         task: MaterializingTask,
-        task_info: TaskInfo,
+        task_cache_info: TaskCacheInfo,
     ):
         """Lazily stores a table in the associated commit stage
 
         The same as `store_table()`, with the difference being that if the
         table object represents a lazy table / query, the store first checks
         if the same query with the same input (based on `table.cache_key`)
         has already been executed before. If yes, instead of evaluating
         the query, it just copies the previous result to the commit stage.
 
         Used when `lazy = True` is set for a materializing task.
         """
-        _ = task
+
         try:
             hook = self.get_m_table_hook(type(table.obj))
             query_str = hook.lazy_query_str(self, table.obj)
             query_hash = stable_hash("LAZY-TABLE", query_str)
         except TypeError:
             # This table type doesn't provide a query string
             # -> Fallback to default implementation
-            return self.store_table(table, task, task_info)
+            return self.store_table(table, task)
+
+        # Store the table
+        try:
+            # Try retrieving the table from the cache and then copying it
+            # to the transaction stage
+            metadata = self.retrieve_lazy_table_metadata(
+                query_hash, task_cache_info.cache_key, table.stage
+            )
+            self.copy_lazy_table_to_transaction(metadata, table)
+            self.logger.info(f"Lazy cache of table '{table.name}' found")
+        except CacheError as e:
+            # Either not found in cache, or copying failed
+            # -> Store using default method
+            self.logger.warning(
+                "Cache miss", table=table.name, stage=table.stage.name, cause=str(e)
+            )
 
-        table_cache_info = CacheManager.lazy_table_cache_lookup(
-            self, task_info.task_cache_info, table, query_hash
-        )
-        if not table_cache_info.is_cache_valid():
             TaskContext.get().is_cache_valid = False
-            self.store_table(table, task, task_info)
+            self.store_table(table, task)
+
+        # Store table metadata
+        self.store_lazy_table_metadata(
+            LazyTableMetadata(
+                name=table.name,
+                stage=table.stage.name,
+                query_hash=query_hash,
+                task_hash=task_cache_info.cache_key,
+            )
+        )
 
         # At this point we MUST also update the cache info, so that any downstream
         # tasks get invalidated if the sql query string changed.
-        table.cache_key = CacheManager.lazy_table_cache_key(
-            task_info.task_cache_info.get_task_cache_key(), query_hash
-        )
+        table.cache_key = lazy_table_cache_key(task_cache_info.cache_key, query_hash)
 
     def store_raw_sql(
-        self, raw_sql: RawSql, task: MaterializingTask, task_info: TaskInfo
+        self, raw_sql: RawSql, task: MaterializingTask, task_cache_info: TaskCacheInfo
     ):
         """Lazily stores a table in the associated commit stage
 
         The same as `store_table()`, with the difference being that the store first
         checks if the same query with the same input (based on `raw_sql.cache_key`)
         has already been executed before. If yes, instead of evaluating
         the query, it just copies the previous result to the commit stage.
         """
-        _ = task
 
         # hacky way to canonicalize query (despite __tmp/__even/__odd suffixes
         # and alias resolution)
         import re
 
         query_str = raw_sql.sql
         query_str = re.sub(r'["\[\]]', "", query_str)
         query_str = re.sub(
             r'(__tmp|__even|__odd)(?=[ \t\n.;"]|$)', "", query_str.lower()
         )
 
         query_hash = stable_hash("RAW-SQL", query_str)
 
-        table_cache_info, raw_sql_metadata = CacheManager.raw_sql_cache_lookup(
-            self, task_info.task_cache_info, raw_sql, query_hash
-        )
-        if not table_cache_info.is_cache_valid():
+        # Store raw sql
+        try:
+            # Try retrieving the table from the cache and then copying it
+            # to the transaction stage
+            metadata = self.retrieve_raw_sql_metadata(
+                query_hash, task_cache_info.cache_key, raw_sql.stage
+            )
+            self.copy_raw_sql_tables_to_transaction(metadata, raw_sql.stage)
+            self.logger.info(f"Lazy cache of stage '{raw_sql.stage}' found")
+
+            prev_objects = metadata.prev_objects
+            new_objects = metadata.new_objects
+        except CacheError as e:
+            # Either not found in cache, or copying failed
+            # -> Store using default method
+            self.logger.warning("Cache miss for raw-SQL", cause=str(e))
+
             TaskContext.get().is_cache_valid = False
             RunContext.get().set_stage_has_changed(task.stage)
 
             prev_objects = self.get_objects_in_stage(raw_sql.stage)
             self.execute_raw_sql(raw_sql)
             post_objects = self.get_objects_in_stage(raw_sql.stage)
 
             # Object names must be sorted to ensure that we can identify the task
             # again in the future even if the objects get returned in a different order.
             prev_objects = sorted(prev_objects)
 
             prev_objects_set = set(prev_objects)
             new_objects = [o for o in post_objects if o not in prev_objects_set]
-        else:
-            prev_objects = raw_sql_metadata.prev_objects
-            new_objects = raw_sql_metadata.new_objects
 
-        table_cache_info.store_raw_sql_metadata(self, prev_objects, new_objects)
+        # Store metadata
+        # Attention: Raw SQL statements may only be executed sequentially within
+        #            stage for store.get_objects_in_stage to work
+        self.store_raw_sql_metadata(
+            RawSqlMetadata(
+                prev_objects=prev_objects,
+                new_objects=new_objects,
+                stage=raw_sql.stage.name,
+                query_hash=query_hash,
+                task_hash=task_cache_info.cache_key,
+            )
+        )
 
         # At this point we MUST also update the cache info, so that any downstream
         # tasks get invalidated if the sql query string changed.
-        raw_sql.cache_key = CacheManager.lazy_table_cache_key(
-            task_info.task_cache_info.get_task_cache_key(), query_hash
-        )
+        raw_sql.cache_key = lazy_table_cache_key(task_cache_info.cache_key, query_hash)
 
         # Store new_objects as part of raw_sql.
         all_table_names = set(self.get_table_objects_in_stage(raw_sql.stage))
         raw_sql.table_names = sorted(o for o in new_objects if o in all_table_names)
 
     @abstractmethod
     def copy_table_to_transaction(self, table: Table):
@@ -423,15 +452,15 @@
                 return obj
 
         obj = super().retrieve_table_obj(table, as_type)
 
         if self.local_table_cache:
             t = table.copy_without_obj()
             t.obj = obj
-            self.local_table_cache.store_input(t, task=None, task_info=None)
+            self.local_table_cache.store_input(t, task=None)
 
         return obj
 
     # Metadata
 
     @abstractmethod
     def store_task_metadata(self, metadata: TaskMetadata, stage: Stage):
@@ -570,27 +599,22 @@
         and convert it to the specified type. If `True` is returned, the
         `retrieve` method MUST be implemented for the type.
         """
 
     @classmethod
     @abstractmethod
     def materialize(
-        cls,
-        store: TableHookResolverT,
-        table: Table,
-        stage_name: str,
-        task_info: TaskInfo,
+        cls, store: TableHookResolverT, table: Table, stage_name: str
     ) -> None:
         """Materialize a table object
 
         :param store: The store which called this method
         :param table: The table that should be materialized
         :param stage_name: The name of the stage in which the table should
             be stored - can either be `stage.name` or `stage.transaction_name`.
-        :param task_info: Information about task execution
         """
 
     @classmethod
     @abstractmethod
     def retrieve(
         cls,
         store: TableHookResolverT,
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/cache/base.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/cache/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from abc import ABC, abstractmethod
 
 import structlog
 
 from pydiverse.pipedag import Stage
 from pydiverse.pipedag._typing import T
 from pydiverse.pipedag.backend.table.base import TableHookResolver
+from pydiverse.pipedag.context import RunContext
 from pydiverse.pipedag.materialize.container import Table
-from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
+from pydiverse.pipedag.materialize.core import MaterializingTask
 from pydiverse.pipedag.util import Disposable
 
 
 class BaseTableCache(ABC, TableHookResolver, Disposable):
     def __init__(
         self,
         store_input: bool = True,
@@ -41,33 +42,37 @@
         Gets called before any table is attempted to be stored in the stage.
         """
 
     @abstractmethod
     def clear_cache(self, stage: Stage):
         """Delete the cache for a specific stage"""
 
-    def store_table(self, table: Table, task: MaterializingTask, task_info: TaskInfo):
+    def store_table(self, table: Table, task: MaterializingTask):
         if self.should_store_output:
-            return self._store_table(table, task, task_info)
+            return self._store_table(table, task)
 
-    def store_input(self, table: Table, task: MaterializingTask, task_info: TaskInfo):
+    def store_input(self, table: Table, task: MaterializingTask):
         if self.should_store_input:
-            return self._store_table(table, task, task_info)
+            return self._store_table(table, task)
 
-    def _store_table(
-        self,
-        table: Table,
-        task: MaterializingTask | None,
-        task_info: TaskInfo | None,
-    ):
+    def _store_table(self, table: Table, task: MaterializingTask | None) -> bool:
+        """
+        :return: bool flag indicating if storing was successful
+        """
         try:
             hook = self.get_m_table_hook(type(table.obj))
-            hook.materialize(self, table, table.stage.transaction_name, task_info)
         except TypeError:
-            return None
+            return False
+
+        if not RunContext.get().should_store_table_in_cache(table):
+            # Prevent multiple tasks writing at the same time
+            return False
+
+        hook.materialize(self, table, table.stage.transaction_name)
+        return True
 
     def retrieve_table_obj(self, table: Table, as_type: type[T]) -> T:
         if not self.should_use_stored_input_as_cache:
             return None
         if not self._has_table(table, as_type):
             return None
         return self._retrieve_table_obj(table, as_type)
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/cache/parquet.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/cache/parquet.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import pandas as pd
 from packaging.version import Version
 
 from pydiverse.pipedag import ConfigContext, Stage, Table
 from pydiverse.pipedag.backend.table.base import TableHook
 from pydiverse.pipedag.backend.table.cache.base import BaseTableCache
-from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
+from pydiverse.pipedag.materialize.core import MaterializingTask
 from pydiverse.pipedag.util import normalize_name
 
 
 class ParquetTableCache(BaseTableCache):
     """
     Local Table Cache that stores tables in `Parquet`_ files.
 
@@ -51,30 +51,34 @@
 
     def init_stage(self, stage: Stage):
         os.makedirs(self.base_path / stage.name, exist_ok=True)
 
     def clear_cache(self, stage: Stage):
         shutil.rmtree(self.get_stage_path(stage))
 
-    def _store_table(self, table: Table, task: MaterializingTask, task_info: TaskInfo):
-        super()._store_table(table, task, task_info)
+    def _store_table(self, table: Table, task: MaterializingTask):
+        if not super()._store_table(table, task):
+            return
 
         metadata = {
             "cache_key": table.cache_key,
         }
         metadata_path = self.get_table_path(table, ".meta.json")
         metadata_path.write_text(json.dumps(metadata))
 
     def _has_table(self, table: Table, as_type: type) -> bool:
         metadata_path = self.get_table_path(table, ".meta.json")
         if not metadata_path.exists():
             return False
 
-        metadata = json.loads(metadata_path.read_text())
-        return metadata["cache_key"] == table.cache_key
+        try:
+            metadata = json.loads(metadata_path.read_text())
+            return metadata["cache_key"] == table.cache_key
+        except (OSError, json.decoder.JSONDecodeError):
+            return False
 
     def get_stage_path(self, stage: Stage):
         return self.base_path / stage.name
 
     def get_table_path(self, table: Table, file_extension: str) -> Path:
         return self.get_stage_path(table.stage) / (table.name + file_extension)
 
@@ -88,21 +92,15 @@
         return issubclass(type_, pd.DataFrame)
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return type_ == pd.DataFrame
 
     @classmethod
-    def materialize(
-        cls,
-        store: ParquetTableCache,
-        table: Table,
-        stage_name: str,
-        task_info: TaskInfo,
-    ):
+    def materialize(cls, store: ParquetTableCache, table: Table, stage_name: str):
         path = store.get_table_path(table, ".parquet")
 
         df: pd.DataFrame = table.obj
         df.to_parquet(path)
 
     @classmethod
     def retrieve(
@@ -151,19 +149,15 @@
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return type_ == polars.dataframe.DataFrame
 
     @classmethod
     def materialize(
-        cls,
-        store: ParquetTableCache,
-        table: Table[polars.DataFrame],
-        stage_name: str,
-        task_info: TaskInfo,
+        cls, store: ParquetTableCache, table: Table[polars.DataFrame], stage_name: str
     ):
         path = store.get_table_path(table, ".parquet")
         table.obj.write_parquet(path)
 
     @classmethod
     def retrieve(
         cls,
@@ -192,30 +186,26 @@
     def can_retrieve(cls, type_) -> bool:
         from pydiverse.transform.eager import PandasTableImpl
 
         return issubclass(type_, PandasTableImpl)
 
     @classmethod
     def materialize(
-        cls,
-        store: ParquetTableCache,
-        table: Table[pdt.Table],
-        stage_name: str,
-        task_info: TaskInfo,
+        cls, store: ParquetTableCache, table: Table[pdt.Table], stage_name: str
     ):
         from pydiverse.transform.core.verbs import collect
         from pydiverse.transform.eager import PandasTableImpl
 
         t = table.obj
         table = table.copy_without_obj()
 
         if isinstance(t._impl, PandasTableImpl):
             table.obj = t >> collect()
             return store.get_hook_subclass(PandasTableHook).materialize(
-                store, table, stage_name, task_info
+                store, table, stage_name
             )
 
         raise TypeError(f"Unsupported type {type(t._impl).__name__}")
 
     @classmethod
     def retrieve(
         cls,
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import warnings
 
 import pandas as pd
 
 from pydiverse.pipedag import Stage, Table
 from pydiverse.pipedag.backend.table.base import BaseTableStore, TableHook
 from pydiverse.pipedag.errors import CacheError, StageError
-from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
+from pydiverse.pipedag.materialize.core import MaterializingTask
 from pydiverse.pipedag.materialize.metadata import LazyTableMetadata, TaskMetadata
 
 
 class DictTableStore(BaseTableStore):
     """
     A very basic table store that stores objects in a dictionary.
     Should only ever be used for testing.
@@ -134,22 +134,15 @@
         return issubclass(type_, pd.DataFrame)
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return type_ == pd.DataFrame
 
     @classmethod
-    def materialize(
-        cls,
-        store,
-        table: Table[pd.DataFrame],
-        stage_name,
-        task_info: TaskInfo | None,
-    ):
-        _ = task_info
+    def materialize(cls, store, table: Table[pd.DataFrame], stage_name):
         if table.name is not None:
             table.obj.attrs["name"] = table.name
         store.store[stage_name][table.name] = table.obj
 
     @classmethod
     def retrieve(cls, store, table, stage_name, as_type):
         return store.store[stage_name][table.name].copy()
@@ -182,22 +175,20 @@
 
     @classmethod
     def materialize(
         cls,
         store,
         table: Table[pdt.Table],
         stage_name,
-        task_info: TaskInfo | None,
     ):
-        _ = task_info
         from pydiverse.transform.core.verbs import collect
 
         table.obj = table.obj >> collect()
         # noinspection PyTypeChecker
-        return PandasTableHook.materialize(store, table, stage_name, task_info)
+        return PandasTableHook.materialize(store, table, stage_name)
 
     @classmethod
     def retrieve(cls, store, table, stage_name, as_type):
         from pydiverse.transform.eager import PandasTableImpl
 
         df = PandasTableHook.retrieve(store, table, stage_name, pd.DataFrame)
         return pdt.Table(PandasTableImpl(table.name, df))
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/ddl.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/ddl.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from pydiverse.pipedag.backend.table.sql.hooks import (
     PandasTableHook,
     SQLAlchemyTableHook,
 )
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 from pydiverse.pipedag.backend.table.util import DType
 from pydiverse.pipedag.materialize import Table
-from pydiverse.pipedag.materialize.core import TaskInfo
 
 
 class PostgresTableStore(SQLTableStore):
     """
     SQLTableStore that supports `PostgreSQL <https://postgresql.org>`_.
 
     In addition to the arguments of
@@ -59,15 +58,14 @@
 class SQLAlchemyTableHook(SQLAlchemyTableHook):
     @classmethod
     def materialize(
         cls,
         store: PostgresTableStore,
         table: Table[sa.sql.expression.TextClause | sa.Text],
         stage_name,
-        task_info: TaskInfo | None,
     ):
         obj = table.obj
         if isinstance(table.obj, (sa.Table, sa.sql.expression.Alias)):
             obj = sa.select("*").select_from(table.obj)
 
         schema = store.get_schema(stage_name)
         store.execute(
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/hooks.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore, TableReference
 from pydiverse.pipedag.backend.table.util import (
     DType,
     PandasDTypeBackend,
 )
 from pydiverse.pipedag.context import TaskContext
 from pydiverse.pipedag.materialize import Table
-from pydiverse.pipedag.materialize.core import TaskInfo
 
 # region SQLALCHEMY
 
 
 @SQLTableStore.register_table()
 class SQLAlchemyTableHook(TableHook[SQLTableStore]):
     @classmethod
@@ -40,34 +39,26 @@
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return type_ == sa.Table
 
     @classmethod
     def materialize(
-        cls,
-        store,
-        table: Table[sa.sql.expression.TextClause | sa.Text],
-        stage_name,
-        task_info: TaskInfo | None,
+        cls, store, table: Table[sa.sql.expression.TextClause | sa.Text], stage_name
     ):
         obj = table.obj
         if isinstance(table.obj, (sa.Table, sa.sql.expression.Alias)):
             obj = sa.select("*").select_from(table.obj)
 
         source_tables = [
             dict(
                 name=tbl.name,
-                schema=store.get_schema(
-                    tbl.stage.transaction_name
-                    if tbl.stage in task_info.open_stages
-                    else tbl.stage.name
-                ).get(),
+                schema=store.get_schema(tbl.stage.current_name).get(),
             )
-            for tbl in task_info.input_tables
+            for tbl in TaskContext.get().input_tables
         ]
         schema = store.get_schema(stage_name)
         store.execute(
             CreateTableAsSelect(
                 table.name,
                 schema,
                 obj,
@@ -124,21 +115,15 @@
         return issubclass(type_, TableReference)
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return False
 
     @classmethod
-    def materialize(
-        cls,
-        store: SQLTableStore,
-        table: Table,
-        stage_name,
-        task_info: TaskInfo | None,
-    ):
+    def materialize(cls, store: SQLTableStore, table: Table, stage_name):
         # For a table reference, we don't need to materialize anything.
         # This is any table referenced by a table reference should already exist
         # in the schema.
         # Instead, we check that the table actually exists.
         schema = store.get_schema(stage_name).get()
 
         inspector = sa.inspect(store.engine)
@@ -186,21 +171,15 @@
     @classmethod
     def auto_table(cls, obj: pd.DataFrame):
         if name := obj.attrs.get("name"):
             return Table(obj, name)
         return super().auto_table(obj)
 
     @classmethod
-    def materialize(
-        cls,
-        store: SQLTableStore,
-        table: Table[pd.DataFrame],
-        stage_name,
-        task_info: TaskInfo | None,
-    ):
+    def materialize(cls, store: SQLTableStore, table: Table[pd.DataFrame], stage_name):
         df = table.obj.copy(deep=False)
         schema = store.get_schema(stage_name)
 
         if store.print_materialize:
             store.logger.info(
                 f"Writing table '{schema.get()}.{table.name}'", table_obj=table.obj
             )
@@ -413,21 +392,15 @@
         return type_ == polars.dataframe.DataFrame
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return type_ == polars.dataframe.DataFrame
 
     @classmethod
-    def materialize(
-        cls,
-        store,
-        table: Table[polars.dataframe.DataFrame],
-        stage_name,
-        task_info: TaskInfo | None,
-    ):
+    def materialize(cls, store, table: Table[polars.dataframe.DataFrame], stage_name):
         # Materialization for polars happens by first converting the dataframe to
         # a pyarrow backed pandas dataframe, and then calling the PandasTableHook
         # for materialization.
 
         df = table.obj
         schema = store.get_schema(stage_name)
 
@@ -487,27 +460,21 @@
         return issubclass(type_, tidypolars.Tibble)
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return type_ == tidypolars.Tibble
 
     @classmethod
-    def materialize(
-        cls,
-        store,
-        table: Table[tidypolars.Tibble],
-        stage_name,
-        task_info: TaskInfo | None,
-    ):
+    def materialize(cls, store, table: Table[tidypolars.Tibble], stage_name):
         t = table.obj
         table = table.copy_without_obj()
         table.obj = t.to_polars()
 
         hook = store.get_hook_subclass(PolarsTableHook)
-        return hook.materialize(store, table, stage_name, task_info)
+        return hook.materialize(store, table, stage_name)
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
@@ -546,31 +513,29 @@
     def can_retrieve(cls, type_) -> bool:
         from pydiverse.transform.eager import PandasTableImpl
         from pydiverse.transform.lazy import SQLTableImpl
 
         return issubclass(type_, (PandasTableImpl, SQLTableImpl))
 
     @classmethod
-    def materialize(
-        cls, store, table: Table[pdt.Table], stage_name, task_info: TaskInfo | None
-    ):
+    def materialize(cls, store, table: Table[pdt.Table], stage_name):
         from pydiverse.transform.core.verbs import collect
         from pydiverse.transform.eager import PandasTableImpl
         from pydiverse.transform.lazy import SQLTableImpl
 
         t = table.obj
         table = table.copy_without_obj()
         if isinstance(t._impl, PandasTableImpl):
             table.obj = t >> collect()
             hook = store.get_hook_subclass(PandasTableHook)
-            return hook.materialize(store, table, stage_name, task_info)
+            return hook.materialize(store, table, stage_name)
         if isinstance(t._impl, SQLTableImpl):
             table.obj = t._impl.build_select()
             hook = store.get_hook_subclass(SQLAlchemyTableHook)
-            return hook.materialize(store, table, stage_name, task_info)
+            return hook.materialize(store, table, stage_name)
         raise NotImplementedError
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
@@ -637,27 +602,21 @@
         return issubclass(type_, ibis.api.Table)
 
     @classmethod
     def can_retrieve(cls, type_) -> bool:
         return issubclass(type_, ibis.api.Table)
 
     @classmethod
-    def materialize(
-        cls,
-        store,
-        table: Table[ibis.api.Table],
-        stage_name,
-        task_info: TaskInfo | None,
-    ):
+    def materialize(cls, store, table: Table[ibis.api.Table], stage_name):
         t = table.obj
         table = table.copy_without_obj()
         table.obj = sa.text(cls.lazy_query_str(store, t))
 
         sa_hook = store.get_hook_subclass(SQLAlchemyTableHook)
-        return sa_hook.materialize(store, table, stage_name, task_info)
+        return sa_hook.materialize(store, table, stage_name)
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/reflection.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/reflection.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/sql.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/sql/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -960,27 +960,27 @@
     ) -> TaskMetadata:
         if self.disable_caching:
             raise CacheError(
                 "Caching is disabled, so we also don't even try to retrieve task"
                 f" cache: {task}"
             )
 
-        ignore_fresh_input = ConfigContext.get().ignore_fresh_input
+        ignore_cache_function = ConfigContext.get().ignore_cache_function
         try:
             with self.engine_connect() as conn:
                 result = (
                     conn.execute(
                         self.tasks_table.select()
                         .where(self.tasks_table.c.name == task.name)
                         .where(self.tasks_table.c.stage == task.stage.name)
                         .where(self.tasks_table.c.version == task.version)
                         .where(self.tasks_table.c.input_hash == input_hash)
                         .where(
                             self.tasks_table.c.cache_fn_hash == cache_fn_hash
-                            if not ignore_fresh_input
+                            if not ignore_cache_function
                             else sa.literal(True)
                         )
                         .where(self.tasks_table.c.in_transaction_schema.in_([False]))
                     )
                     .mappings()
                     .one_or_none()
                 )
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/util/dtype.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/backend/table/util/dtype.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/context/context.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/context/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 if TYPE_CHECKING:
     from pydiverse.pipedag._typing import T
     from pydiverse.pipedag.backend import BaseLockManager
     from pydiverse.pipedag.context.run_context import StageLockStateHandler
     from pydiverse.pipedag.core import Flow, Stage, Task
     from pydiverse.pipedag.engine.base import OrchestrationEngine
+    from pydiverse.pipedag.materialize import Table
 
 
 class BaseContext:
     _context_var: ClassVar[ContextVar]
     _token: Token = None
     _enter_counter: int = 0
     _lock: Lock = Lock()
@@ -86,14 +87,15 @@
     """Context used while executing a task
 
     It is used to retrieve a reference to the task object from within a running task.
     It also serves as a place to store temporary state while processing a task.
     """
 
     task: Task
+    input_tables: list[Table] = None
     is_cache_valid: bool | None = None
     name_disambiguator: NameDisambiguator = field(factory=NameDisambiguator)
 
     _context_var = ContextVar("task_context")
 
 
 class StageCommitTechnique(Enum):
@@ -155,19 +157,22 @@
     stage_commit_technique: StageCommitTechnique
     network_interface: str
     attrs: Box
 
     table_hook_args: Box
 
     # run specific options
-    ignore_fresh_input: bool = False
+    ignore_cache_function: bool = False
 
     # INTERNAL FLAGS - ONLY FOR PIPEDAG USE
     # When set to True, exceptions raised in a flow don't get logged
     _swallow_exceptions: bool = False
+    # When set to True, indicates that all tasks should get run, independent
+    # of their cache validity
+    _force_task_execution: bool = False
 
     @cached_property
     def auto_table(self) -> tuple[type, ...]:
         return tuple(map(import_object, self._config_dict.get("auto_table", ())))
 
     @cached_property
     def auto_blob(self) -> tuple[type, ...]:
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/context/run_context.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/context/run_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,28 +92,31 @@
         self.ref_count = [0] * num_stages
         self.task_state = [FinalTaskState.UNKNOWN] * len(self.tasks)
         self.stage_state = [StageState.UNINITIALIZED] * num_stages
 
         self.table_names = [set() for _ in range(num_stages)]
         self.blob_names = [set() for _ in range(num_stages)]
 
+        self.tables_in_local_table_cache = [set() for _ in range(num_stages)]
+
         self.task_memo: defaultdict[Any, Any] = defaultdict(lambda: MemoState.NONE)
 
         # DEFERRED TABLE STORE OPERATIONS
         self.deferred_thread_pool = ThreadPoolExecutor()
         self.deferred_ts_ops: dict[int, list[DeferredTableStoreOp]] = {}
         self.deferred_ts_ops_futures: dict[int, list[Future]] = {}
         self.changed_stages: set[int] = set()
 
         # STATE LOCKS
         self.ref_count_lock = Lock()
         self.stage_state_lock = Lock()
         self.names_lock = Lock()
         self.task_memo_lock = Lock()
         self.deferred_ops_lock = RLock()
+        self.local_table_cache_lock = Lock()
 
         # LOCKING
         self.lock_manager = config_ctx.create_lock_manager()
         self.lock_handler = StageLockStateHandler(self.lock_manager)
 
         try:
             # If we are inside a StageLockContext, then we shouldn't release any
@@ -496,14 +499,28 @@
     @synchronized("names_lock")
     def remove_names(self, stage_id: int, tables: list[str], blobs: list[str]):
         for table in tables:
             self.table_names[stage_id].remove(table)
         for blob in blobs:
             self.blob_names[stage_id].remove(blob)
 
+    # LOCAL TABLE CACHE
+
+    @synchronized("local_table_cache_lock")
+    def should_store_table_in_cache(self, stage_id: int, table_name: str) -> bool:
+        if table_name in self.tables_in_local_table_cache[stage_id]:
+            # Some other task already stored / is attempting to store this table
+            # In case we are running tasks in parallel and `store_input` is set
+            # to true, it can happen that multiple tasks are reading and writing
+            # the same table at the same time, which may lead to incorrect behaviour.
+            return False
+
+        self.tables_in_local_table_cache[stage_id].add(table_name)
+        return True
+
 
 def _call_with_args(fn, args, kwargs):
     fn(*args, **kwargs)
 
 
 class RunContext(BaseContext):
     _context_var = ContextVar("run_context_proxy")
@@ -633,14 +650,19 @@
         self._request(
             "remove_names",
             stage.id,
             [t.name for t in tables],
             [b.name for b in blobs],
         )
 
+    # LOCAL TABLE CACHE
+
+    def should_store_table_in_cache(self, table: Table):
+        return self._request("should_store_table_in_cache", table.stage.id, table.name)
+
 
 @attrs.frozen
 class DematerializeRunContext(BaseAttrsContext):
     """Dummy RunContext that returns `COMMITTED` as the stage state for all stages
 
     To dematerialize an object we must know it the associates state has been
     committed or not. This context replaces the RunContext created by
@@ -655,14 +677,17 @@
 
     def get_stage_state(self, stage: Stage) -> StageState:
         return StageState.COMMITTED
 
     def validate_stage_lock(self, stage: Stage):
         pass
 
+    def should_store_table_in_cache(self, table: Table):
+        return False
+
 
 # Stage Locking
 
 
 class StageLockStateHandler(Disposable):
     """
     Handle LockState changes (i.e. locks that may become UNCERTAIN
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/config.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/core/config.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/flow.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/core/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
     def run(
         self,
         *components: Task | TaskGetItem | Stage,
         config: ConfigContext = None,
         orchestration_engine: OrchestrationEngine = None,
         fail_fast: bool | None = None,
-        ignore_fresh_input: bool = False,
+        ignore_cache_function: bool = False,
         **kwargs,
     ) -> Result:
         """Execute the flow.
         This will execute the flow and all tasks within using the orchestration engine.
 
         :param components: An optional selection of tasks or stages that should
             get executed. If no values are provided, all tasks and stages get executed.
@@ -231,15 +231,15 @@
         :param orchestration_engine:
             The orchestration engine to use. If no engine is provided, the
             orchestration engine from the config gets used.
         :param fail_fast:
             Whether exceptions should get raised or swallowed.
             If set to True, exceptions that occur get immediately raised and the
             flow gets aborted.
-        :param ignore_fresh_input:
+        :param ignore_cache_function:
             When set to True, the task's cache function gets ignored when determining
             the cache validity of a task.
         :param kwargs:
             Other keyword arguments that get passed on directly to the
             ``run()`` method of the orchestration engine. Consequently, these
             keyword arguments are engine dependant.
         :return:
@@ -277,21 +277,20 @@
                 config = ConfigContext.get()
             except LookupError:
                 config = PipedagConfig.default.get(flow=self.name)
 
         # Evolve config using the arguments passed to flow.run
         config = config.evolve(
             fail_fast=(fail_fast if fail_fast is not None else config.fail_fast),
-            ignore_fresh_input=ignore_fresh_input,
-            ignore_task_version=(
+            ignore_cache_function=ignore_cache_function,
+            force_task_execution=(
                 # If subflow consists of a subset of tasks (-> not a subset of stages)
-                # then we want to ignore the task version to ensure the tasks always
-                # get executed.
+                # then we want to skip cache validity checking to ensure the tasks
+                # always get executed.
                 subflow.is_tasks_subflow
-                or config.ignore_task_version
             ),
         )
 
         with config, RunContextServer(subflow):
             if orchestration_engine is None:
                 orchestration_engine = config.create_orchestration_engine()
             result = orchestration_engine.run(subflow, **kwargs)
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/result.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/core/result.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/stage.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/core/stage.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/task.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/core/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any, Callable
 
 import structlog
 
 from pydiverse.pipedag.context import ConfigContext, DAGContext, RunContext, TaskContext
 from pydiverse.pipedag.context.run_context import FinalTaskState
-from pydiverse.pipedag.errors import FlowError, StageError
+from pydiverse.pipedag.errors import StageError
 from pydiverse.pipedag.util import deep_map
 from pydiverse.pipedag.util.hashing import stable_hash
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.core import Flow, Stage
 
 
@@ -52,27 +52,36 @@
         self._bound_task_type = Task
         self._signature = inspect.signature(fn)
 
     def __repr__(self):
         return f"<UnboundTask 'name' {hex(id(self))}>"
 
     def __call__(self, *args, **kwargs) -> Task:
-        """Constructs a `Task` with bound inputs"""
+        """
+        When called inside a flow definition context:
+        Constructs a `Task` with bound inputs
+
+        When called outside a flow definition context:
+        Invoke to original function.
+        """
         try:
             ctx = DAGContext.get()
         except LookupError:
-            raise FlowError("Can't call pipedag task outside of a flow.") from None
+            return self._call_original_function(*args, **kwargs)
 
         if ctx.stage is None:
             raise StageError("Can't call pipedag task outside of a stage.")
 
         # Construct Task
         bound_args = self._signature.bind(*args, **kwargs)
         return self._bound_task_type(self, bound_args, ctx.flow, ctx.stage)
 
+    def _call_original_function(self, *args, **kwargs):
+        return self.fn(*args, **kwargs)
+
 
 class Task:
     def __init__(
         self,
         unbound_task: UnboundTask,
         bound_args: inspect.BoundArguments,
         flow: Flow,
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/base.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/dask.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/engine/dask.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/cli.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/management/cli.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/commands/clear_metadata.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/management/commands/clear_metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/commands/delete_schemas.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/management/commands/delete_schemas.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/container.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/materialize/container.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/core.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/materialize/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
+import copy
 import functools
 import inspect
-from dataclasses import dataclass
+import uuid
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, overload
 
 from pydiverse.pipedag._typing import CallableT
 from pydiverse.pipedag.context import ConfigContext, RunContext, TaskContext
 from pydiverse.pipedag.core.task import Task, TaskGetItem, UnboundTask
-from pydiverse.pipedag.materialize.cache import CacheManager, TaskCacheInfo
+from pydiverse.pipedag.errors import CacheError
+from pydiverse.pipedag.materialize.cache import TaskCacheInfo, task_cache_key
 from pydiverse.pipedag.materialize.container import Blob, RawSql, Table
 from pydiverse.pipedag.util import deep_map
 from pydiverse.pipedag.util.hashing import stable_hash
 
 if TYPE_CHECKING:
     from pydiverse.pipedag import Flow, Stage
 
@@ -190,30 +192,53 @@
 
 
 class UnboundMaterializingTask(UnboundTask):
     """A materializing task without any bound arguments.
 
     Instances of this class get initialized using the
     :py:func:`@materialize <pydiverse.pipedag.materialize>` decorator.
-    By calling this object, a :py:class:`~.MaterializingTask` gets created
-    that binds the provided arguments to the task.
+    By calling this object inside a ``with Flow(...)`` context,
+    a :py:class:`~.MaterializingTask` gets created that binds the provided
+    arguments to the task.
 
     >>> @materialize
     ... def some_task(arg):
     ...     ...
     ...
     >>> type(some_task)
     <class 'pydiverse.pipedag.materialize.core.UnboundMaterializingTask'>
 
     >>> with Flow() as f:
     ...     with Stage("stage"):
     ...         x = some_task(...)
     ...
     >>> type(x)
     <class 'pydiverse.pipedag.materialize.core.MaterializingTask'>
+
+    When you call a `UnboundMaterializingTask` outside a flow definition context,
+    then the original function (that was decorated with :py:func:`@materialize
+    <pydiverse.pipedag.materialize>`) gets called. The only difference being, that
+    any :py:class:`~.Table`, :py:class:`~.Blob` or :py:class:`~.RawSql` objects
+    returned from the task get replaced with the object that they wrap:
+
+    >>> import pandas as pd
+    >>>
+    >>> @materialize(input_type=pd.DataFrame)
+    ... def double_it(df):
+    ...     return Table(df * 2)
+    ...
+    >>> x = pd.DataFrame({"x": [0, 1, 2, 3]})
+    >>> double_it(x)
+       x
+    0  0
+    1  2
+    2  4
+    3  6
+
+
     """
 
     def __init__(
         self,
         fn: Callable,
         *,
         name: str = None,
@@ -226,23 +251,36 @@
         super().__init__(
             MaterializationWrapper(fn),
             name=name,
             nout=nout,
         )
 
         self._bound_task_type = MaterializingTask
+        self._original_fn = fn
 
         self.input_type = input_type
         self.version = version
         self.cache = cache
         self.lazy = lazy
 
     def __call__(self, *args, **kwargs) -> MaterializingTask:
         return super().__call__(*args, **kwargs)  # type: ignore
 
+    def _call_original_function(self, *args, **kwargs):
+        result = self._original_fn(*args, **kwargs)
+
+        def unwrap_mutator(x):
+            if isinstance(x, (Task, Blob)):
+                return x.obj
+            if isinstance(x, RawSql):
+                return x.sql
+            return x
+
+        return deep_map(result, unwrap_mutator)
+
 
 class MaterializingTask(Task):
     """
     A pipedag task that materializes all its outputs.
 
     Instances of this class get initialized by calling a
     :py:class:`~.UnboundMaterializingTask`.
@@ -300,23 +338,29 @@
         return MaterializingTaskGetItem(self, self, item)
 
     def run(self, inputs: dict[int, Any], **kwargs):
         # When running only a subset of an entire flow, not all inputs
         # get calculated during flow execution. As a consequence, we must load
         # those inputs from the cache.
 
+        def replace_stage_with_pseudo_stage(x):
+            if isinstance(x, (Table, Blob, RawSql)):
+                x.stage = PseudoStage(x.stage, did_commit=True)
+            return x
+
         for in_id, in_task in self.input_tasks.items():
             if in_id in inputs:
                 continue
 
             store = ConfigContext.get().store
             cached_output, metadata = store.retrieve_most_recent_task_output_from_cache(
                 in_task
             )
 
+            cached_output = deep_map(cached_output, replace_stage_with_pseudo_stage)
             inputs[in_id] = cached_output
 
         return super().run(inputs, **kwargs)
 
     def get_output_from_store(self, as_type: type = None) -> Any:
         """Retrieves the output of the task from the cache.
 
@@ -396,90 +440,136 @@
         :param _pipedag_task_: The `MaterializingTask` instance which called
             this wrapper.
         :param kwargs: The keyword arguments passed to the function
         :return: A copy of what the original function returns annotated
             with some additional metadata.
         """
 
-        task: MaterializingTask = TaskContext.get().task  # type: ignore
-        store = ConfigContext.get().store
+        task_context = TaskContext.get()
+        config_context = ConfigContext.get()
+        run_context = RunContext.get()
+
+        task: MaterializingTask = task_context.task  # type: ignore
         bound = self.fn_signature.bind(*args, **kwargs)
 
         if task is None:
             raise TypeError("Task can't be None.")
 
         # If this is the first task in this stage to be executed, ensure that
         # the stage has been initialized and locked.
+        store = config_context.store
         store.ensure_stage_is_ready(task.stage)
-        open_stages = {task.stage}
-        outer_stage = task.stage.outer_stage
-        while outer_stage is not None:
-            open_stages.add(outer_stage)
-            outer_stage = outer_stage.outer_stage
 
         # Compute the cache key for the task inputs
         input_json = store.json_encode(bound.arguments)
         input_hash = stable_hash("INPUT", input_json)
 
         cache_fn_hash = ""
         if task.cache is not None:
             cache_fn_output = store.json_encode(task.cache(*args, **kwargs))
             cache_fn_hash = stable_hash("CACHE_FN", cache_fn_output)
 
-        memo_cache_key = CacheManager.task_cache_key(task, input_hash, cache_fn_hash)
+        memo_cache_key = task_cache_key(task, input_hash, cache_fn_hash)
 
         # Check if this task has already been run with the same inputs
         # If yes, return memoized result. This prevents DuplicateNameExceptions
-        ctx = RunContext.get()
-        with ctx.task_memo(task, memo_cache_key) as (success, memo):
+        with run_context.task_memo(task, memo_cache_key) as (success, memo):
             if success:
                 task.logger.info(
                     "Task has already been run with the same inputs."
                     " Using memoized results."
                 )
 
                 return memo
 
-            task_cache_info = CacheManager.cache_lookup(
-                store, task, input_hash, cache_fn_hash
+            # Cache Lookup (only required if task isn't lazy)
+            force_task_execution = config_context._force_task_execution
+            skip_cache_lookup = (
+                config_context.ignore_task_version or task.version is None
             )
-            if not task.lazy:
-                ctx = RunContext.get()
-                TaskContext.get().is_cache_valid = task_cache_info.is_cache_valid()
-                if task_cache_info.is_cache_valid():
-                    ctx.store_task_memo(
-                        task, memo_cache_key, task_cache_info.get_cached_output()
+
+            if not task.lazy and not skip_cache_lookup and not force_task_execution:
+                try:
+                    cached_output, cache_metadata = store.retrieve_cached_output(
+                        task, input_hash, cache_fn_hash
                     )
-                    # Task isn't lazy -> copy cache to transaction stage
-                    return task_cache_info.get_cached_output()
-            else:
+                    store.copy_cached_output_to_transaction_stage(
+                        cached_output, cache_metadata, task
+                    )
+                    run_context.store_task_memo(task, memo_cache_key, cached_output)
+                    task.logger.info("Found task in cache. Using cached result.")
+                    TaskContext.get().is_cache_valid = True
+                    return cached_output
+                except CacheError as e:
+                    task.logger.info("Failed to retrieve task from cache", cause=str(e))
+                    TaskContext.get().is_cache_valid = False
+
+            if task.lazy:
                 # For lazy tasks, is_cache_valid gets set to false during the
                 # store.materialize_task procedure
                 TaskContext.get().is_cache_valid = True
 
+                if config_context.ignore_cache_function:
+                    # `cache_fn_hash` is not used for cache retrieval if
+                    # ignore_cache_function is set to True.
+                    # In that case, cache_metadata.cache_fn_hash may be different
+                    # from the cache_fn_hash of the current task run.
+
+                    try:
+                        _, cache_metadata = store.retrieve_cached_output(
+                            task, input_hash, cache_fn_hash
+                        )
+                        cache_fn_hash = cache_metadata.cache_fn_hash
+                    except CacheError as e:
+                        task.logger.info(
+                            "Failed to retrieve task from cache", cause=str(e)
+                        )
+
+            # Prepare TaskCacheInfo
+            if not task.lazy and skip_cache_lookup:
+                # Assign random version to disable caching for this task
+                task = copy.copy(task)
+                task.version = uuid.uuid4().hex
+
+            task_cache_info = TaskCacheInfo(
+                task=task,
+                input_hash=input_hash,
+                cache_fn_hash=cache_fn_hash,
+                cache_key=task_cache_key(task, input_hash, cache_fn_hash),
+            )
+
+            # Compute the input_tables value of the TaskContext
+            input_tables = []
+
+            def _input_tables_visitor(x):
+                if isinstance(x, Table):
+                    input_tables.append(x)
+                return x
+
+            deep_map(bound.arguments.values(), _input_tables_visitor)
+            task_context.input_tables = input_tables
+
             # Not found in cache / lazy -> Evaluate Function
-            args, kwargs, input_tables = store.dematerialize_task_inputs(
+            args, kwargs = store.dematerialize_task_inputs(
                 task, bound.args, bound.kwargs
             )
 
             result = self.fn(*args, **kwargs)
-            result = store.materialize_task(
-                task, TaskInfo(task_cache_info, input_tables, open_stages), result
-            )
+            result = store.materialize_task(task, task_cache_info, result)
 
             # Delete underlying objects from result (after materializing them)
             def obj_del_mutator(x):
                 if isinstance(x, (Table, Blob)):
                     x.obj = None
                 if isinstance(x, RawSql):
                     x.loaded_tables = None
                 return x
 
             result = deep_map(result, obj_del_mutator)
-            ctx.store_task_memo(task, memo_cache_key, result)
+            run_context.store_task_memo(task, memo_cache_key, result)
             self.value = result
 
             return result
 
 
 def _get_output_from_store(
     task: MaterializingTask | MaterializingTaskGetItem, as_type: type
@@ -492,12 +582,30 @@
 
     store = ConfigContext.get().store
     with DematerializeRunContext(root_task.flow):
         cached_output, _ = store.retrieve_most_recent_task_output_from_cache(root_task)
         return dematerialize_output_from_store(store, task, cached_output, as_type)
 
 
-@dataclass
-class TaskInfo:
-    task_cache_info: TaskCacheInfo
-    input_tables: list[Table]
-    open_stages: set[Stage]
+class PseudoStage:
+    def __init__(self, stage: Stage, did_commit: bool):
+        self._stage = stage
+        self._name = stage.name
+        self._transaction_name = stage.name
+        self._did_commit = did_commit
+
+        self.id = stage.id
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def transaction_name(self) -> str:
+        return self._transaction_name
+
+    @property
+    def current_name(self) -> str:
+        if self._did_commit:
+            return self.name
+        else:
+            return self.transaction_name
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/store.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/materialize/store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 import itertools
+from datetime import datetime
 from typing import Any, Callable
 
 import structlog
 
 from pydiverse.pipedag import Blob, Stage, Table, backend
 from pydiverse.pipedag._typing import Materializable, T
 from pydiverse.pipedag.context import ConfigContext, RunContext, TaskContext
 from pydiverse.pipedag.context.run_context import StageState
 from pydiverse.pipedag.core.config import PipedagConfig
 from pydiverse.pipedag.core.task import Task, TaskGetItem
 from pydiverse.pipedag.errors import CacheError, DuplicateNameError, StageError
+from pydiverse.pipedag.materialize.cache import TaskCacheInfo
 from pydiverse.pipedag.materialize.container import RawSql
-from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
+from pydiverse.pipedag.materialize.core import MaterializingTask
 from pydiverse.pipedag.materialize.metadata import TaskMetadata
 from pydiverse.pipedag.util import Disposable, deep_map
 
 
 class PipeDAGStore(Disposable):
     """Main storage interface for materializing tasks
 
@@ -137,55 +139,51 @@
         return item
 
     def dematerialize_task_inputs(
         self,
         task: MaterializingTask,
         args: tuple[Materializable],
         kwargs: dict[str, Materializable],
-    ) -> tuple[tuple, dict, list[Table]]:
+    ) -> tuple[tuple, dict]:
         """Loads the inputs for a task from the storage backends
 
         Traverses the function arguments and replaces all `Table` and
         `Blob` objects with the associated objects stored in the backend.
 
         :param task: The task for which the arguments should be dematerialized
         :param args: The positional arguments
         :param kwargs: The keyword arguments
         :return: A tuple with the dematerialized args and kwargs
         """
 
         ctx = RunContext.get()
 
-        input_tables = []
-
         def dematerialize_mapper(x):
-            if isinstance(x, Table):
-                input_tables.append(x)
             return self.dematerialize_item(x, as_type=task.input_type, ctx=ctx)
 
         d_args = deep_map(args, dematerialize_mapper)
         d_kwargs = deep_map(kwargs, dematerialize_mapper)
 
-        return d_args, d_kwargs, input_tables
+        return d_args, d_kwargs
 
     def materialize_task(
         self,
         task: MaterializingTask,
-        task_info: TaskInfo,
+        task_cache_info: TaskCacheInfo,
         value: Materializable,
     ) -> Materializable:
         """Stores the output of a task in the backend
 
         Traverses the output produced by a task, adds missing metadata,
         materializes all `Table` and `Blob` objects and returns a new
         output object with the required metadata to allow dematerialization.
 
         :param task: The task instance which produced `value`. Must have
             the correct `cache_key` attribute set.
-        :param task_info: Information about task carried through materialization
+        :param task_cache_info: Task cache information.
         :param value: The output of the task. Must be materializable; this
             means it can only contain the following object types:
             `dict`, `list`, `tuple`,
             `int`, `float`, `str`, `bool`, `None`,
             and PipeDAG's `Table` and `Blob` type.
         :return: A copy of `value` with additional metadata
         """
@@ -225,26 +223,23 @@
                     "You can't return a PipedagConfig object from a materializing task."
                 )
 
             # Do the materialization
             if isinstance(x, (Table, RawSql, Blob)):
                 if not task.lazy:
                     # task cache_key is output cache_key for eager tables
-                    x.cache_key = task_info.task_cache_info.get_task_cache_key()
+                    x.cache_key = task_cache_info.cache_key
 
                 x.stage = stage
 
                 # Update name:
                 # - If no name has been provided, generate on automatically
                 # - If the provided name ends with %%, perform name mangling
                 object_number = next(auto_suffix_counter)
-                auto_suffix = (
-                    f"{task_info.task_cache_info.get_task_cache_key()}"
-                    f"_{object_number:04d}"
-                )
+                auto_suffix = f"{task_cache_info.cache_key}" f"_{object_number:04d}"
 
                 if x.name is None:
                     x.name = task.name + "_" + auto_suffix
                 elif x.name.endswith("%%"):
                     x.name = x.name[:-2] + auto_suffix
 
                 ctx.validate_stage_lock(stage)
@@ -273,33 +268,44 @@
         def store_metadata():
             """
             Metadata must be generated after everything else has been materialized,
             because during materialization the cache_key of the different objects
             can get changed.
             """
             output_json = self.json_encode(m_value)
-            task_info.task_cache_info.store_task_metadata(
-                output_json, self.table_store, stage
+            metadata = TaskMetadata(
+                name=task.name,
+                stage=task.stage.name,
+                version=task.version,
+                timestamp=datetime.now(),
+                run_id=ctx.run_id,
+                position_hash=task.position_hash,
+                input_hash=task_cache_info.input_hash,
+                cache_fn_hash=task_cache_info.cache_fn_hash,
+                output_json=output_json,
             )
+            self.table_store.store_task_metadata(metadata, stage)
 
         def store_table(table: Table):
             if task.lazy:
-                self.table_store.store_table_lazy(table, task, task_info)
+                self.table_store.store_table_lazy(table, task, task_cache_info)
             else:
-                self.table_store.store_table(table, task, task_info)
+                self.table_store.store_table(table, task)
 
         # Materialize
         self._check_names(task, tables, blobs)
         self._store_task_transaction(
             task,
             tables,
             raw_sqls,
             blobs,
             store_table,
-            lambda raw_sql: self.table_store.store_raw_sql(raw_sql, task, task_info),
+            lambda raw_sql: self.table_store.store_raw_sql(
+                raw_sql, task, task_cache_info
+            ),
             self.blob_store.store_blob,
             store_metadata,
         )
 
         return m_value
 
     @staticmethod
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/disposable.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/hashing.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/hashing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/import_.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/import_.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/ipc.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/ipc.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/json.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/json.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,39 +96,40 @@
 def json_object_hook(d: dict):
     """Decode json with `Table` and `Blob` objects"""
     if TYPE_KEY not in d:
         return d
 
     type_ = Type(d[TYPE_KEY])
 
-    run_context = RunContext.get()
-    stages = run_context.flow.stages
+    def get_stage(name: str):
+        stages = RunContext.get().flow.stages
+        return stages[name]
 
     if type_ == Type.TABLE:
         tbl = Table(
             name=d["name"],
             primary_key=d["primary_key"],
             indexes=d["indexes"],
         )
-        tbl.stage = stages[d["stage"]]
+        tbl.stage = get_stage(d["stage"])
         tbl.cache_key = d["cache_key"]
         return tbl
     if type_ == Type.RAW_SQL:
         raw_sql = RawSql(name=d["name"])
-        raw_sql.stage = stages[d["stage"]]
+        raw_sql.stage = get_stage(d["stage"])
         raw_sql.cache_key = d["cache_key"]
         raw_sql.table_names = d["table_names"]
         return raw_sql
     if type_ == Type.BLOB:
         blob = Blob(name=d["name"])
-        blob.stage = stages[d["stage"]]
+        blob.stage = get_stage(d["stage"])
         blob.cache_key = d["cache_key"]
         return blob
     if type_ == Type.STAGE:
-        return stages[d["name"]]
+        return get_stage(d["name"])
     if type_ == Type.PIPEDAG_CONFIG:
         # PipedagConfig objects are allowed as input to @materialize tasks,
         # but it is not allowed as output since this might cause trouble
         # for cache-invalidation
         raise TypeError("PipedagConfig can't be deserialized.")
     if type_ == Type.PATHLIB_PATH:
         return Path(d["path"])
```

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/naming.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/naming.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/structlog.py` & `pydiverse_pipedag-0.6.4/src/pydiverse/pipedag/util/structlog.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.3/PKG-INFO` & `pydiverse_pipedag-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.6.3
+Version: 0.6.4
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

