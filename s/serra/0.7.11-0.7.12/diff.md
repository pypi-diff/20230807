# Comparing `tmp/serra-0.7.11.tar.gz` & `tmp/serra-0.7.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serra-0.7.11.tar", last modified: Thu Aug  3 20:32:08 2023, max compression
+gzip compressed data, was "serra-0.7.12.tar", last modified: Mon Aug  7 19:21:59 2023, max compression
```

## Comparing `serra-0.7.11.tar` & `serra-0.7.12.tar`

### file list

```diff
@@ -1,110 +1,109 @@
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.737346 serra-0.7.11/
--rw-r--r--   0 albertstanley   (501) staff       (20)     3860 2023-08-03 20:28:12.000000 serra-0.7.11/LICENSE.md
--rw-r--r--   0 albertstanley   (501) staff       (20)      243 2023-08-03 20:32:08.737039 serra-0.7.11/PKG-INFO
--rw-r--r--   0 albertstanley   (501) staff       (20)     3917 2023-08-03 20:28:12.000000 serra-0.7.11/README.md
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.711951 serra-0.7.11/serra/
--rw-r--r--   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:28:12.000000 serra-0.7.11/serra/__init__.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     2006 2023-08-03 20:28:12.000000 serra-0.7.11/serra/aws.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1872 2023-08-03 20:28:12.000000 serra-0.7.11/serra/cli.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      252 2023-08-03 20:28:12.000000 serra-0.7.11/serra/config.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1788 2023-08-03 20:28:12.000000 serra-0.7.11/serra/config_parser.py
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.707844 serra-0.7.11/serra/data/
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.715115 serra-0.7.11/serra/data/autocomplete/
--rw-r--r--   0 albertstanley   (501) staff       (20)     1110 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/README.md
--rw-r--r--   0 albertstanley   (501) staff       (20)     1636 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/gen_schemas.py
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.715410 serra-0.7.11/serra/data/autocomplete/inputs/
--rw-r--r--   0 albertstanley   (501) staff       (20)     2249 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/inputs/specs.json
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.720404 serra-0.7.11/serra/data/autocomplete/output/
--rw-r--r--   0 albertstanley   (501) staff       (20)      391 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/AddColumnTransformer.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      276 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/AmazonS3Reader.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      341 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/AmazonS3Writer.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      267 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/CaseWhenTransformer.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      216 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/CastColumnTransformer.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      206 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/DatabricksReader.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      389 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/DatabricksWriter.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      213 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/DropColumnTransformer.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      274 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/GetCountTransformer.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      354 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/JoinTransformer.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      148 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/LocalReader.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      213 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/LocalWriter.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      331 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/MapTransformer.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      408 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/PivotTransformer.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      274 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/RenameColumnTransformer.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      210 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/SelectTransformer.json
--rw-r--r--   0 albertstanley   (501) staff       (20)      452 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/SnowflakeWriter.json
--rw-r--r--   0 albertstanley   (501) staff       (20)     7553 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/serra_yaml_schema.json
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.720854 serra-0.7.11/serra/data/autocomplete/templates/
--rw-r--r--   0 albertstanley   (501) staff       (20)      326 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/templates/schema_template.json
--rw-r--r--   0 albertstanley   (501) staff       (20)       95 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/templates/transformer_template.json
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.721326 serra-0.7.11/serra/data/workspace_example/
--rw-r--r--   0 albertstanley   (501) staff       (20)      137 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/README.md
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.721990 serra-0.7.11/serra/data/workspace_example/examples/
--rw-r--r--   0 albertstanley   (501) staff       (20)     1610 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/examples/ratings.csv
--rw-r--r--   0 albertstanley   (501) staff       (20)     6706 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/examples/sales.csv
--rw-r--r--   0 albertstanley   (501) staff       (20)     1124 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/examples/states_to_abbreviation.json
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.723521 serra-0.7.11/serra/data/workspace_example/jobs/
--rw-r--r--   0 albertstanley   (501) staff       (20)      912 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/CloudDemo.yml
--rw-r--r--   0 albertstanley   (501) staff       (20)      952 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/Demo.yml
--rw-r--r--   0 albertstanley   (501) staff       (20)      418 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/LocalExample.yml
--rw-r--r--   0 albertstanley   (501) staff       (20)      220 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/ReadExample.yml
--rw-r--r--   0 albertstanley   (501) staff       (20)      456 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/ReadJoinWrite.yml
--rw-r--r--   0 albertstanley   (501) staff       (20)      393 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/ReadMapWrite.yml
--rw-r--r--   0 albertstanley   (501) staff       (20)      397 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/ReadPivotWrite.yml
--rw-r--r--   0 albertstanley   (501) staff       (20)      323 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/profiles.yml
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.723962 serra-0.7.11/serra/data/workspace_example/sql/
--rw-r--r--   0 albertstanley   (501) staff       (20)     2603 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/sql/easy_demo.sql
--rw-r--r--   0 albertstanley   (501) staff       (20)     2909 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/sql/hard_demo.sql
--rw-r--r--   0 albertstanley   (501) staff       (20)     2964 2023-08-03 20:28:12.000000 serra-0.7.11/serra/databricks.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      106 2023-08-03 20:28:12.000000 serra-0.7.11/serra/exceptions.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1120 2023-08-03 20:28:12.000000 serra-0.7.11/serra/profile.py
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.725617 serra-0.7.11/serra/readers/
--rw-r--r--   0 albertstanley   (501) staff       (20)      233 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/__init__.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     2182 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/amazon_reader.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1238 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/databricks_reader.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      962 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/local_reader.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      277 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/reader.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     2063 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/snowflaker_reader.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     2984 2023-08-03 20:28:12.000000 serra-0.7.11/serra/run.py
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.726532 serra-0.7.11/serra/runners/
--rw-r--r--   0 albertstanley   (501) staff       (20)     2631 2023-08-03 20:28:12.000000 serra-0.7.11/serra/runners/ExecutionGraph.py
--rw-r--r--   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:28:12.000000 serra-0.7.11/serra/runners/__init__.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     3148 2023-08-03 20:28:12.000000 serra-0.7.11/serra/runners/graph_runner.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      443 2023-08-03 20:28:12.000000 serra-0.7.11/serra/tests.py
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.734121 serra-0.7.11/serra/transformers/
--rw-r--r--   0 albertstanley   (501) staff       (20)      624 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/__init__.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1512 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/add_column_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1225 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/aggregate_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      631 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/case_when_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1318 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/cast_columns_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1016 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/coalesce_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      875 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/drop_columns_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1002 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/filter_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1138 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/get_count_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      910 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/get_distinct_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1339 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/impute_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     2175 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/join_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     2867 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/map_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1145 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/order_by_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1986 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/pivot_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1009 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/rename_column_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1423 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/select_transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      310 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/transformer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     3211 2023-08-03 20:28:12.000000 serra-0.7.11/serra/translate_client.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     2293 2023-08-03 20:28:12.000000 serra-0.7.11/serra/utils.py
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.736496 serra-0.7.11/serra/writers/
--rw-r--r--   0 albertstanley   (501) staff       (20)      232 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/__init__.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     2143 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/amazon_writer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     1400 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/databricks_writer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      957 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/local_writer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)     3864 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/snowflake_writer.py
--rw-r--r--   0 albertstanley   (501) staff       (20)      284 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/writer.py
-drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.714361 serra-0.7.11/serra.egg-info/
--rw-r--r--   0 albertstanley   (501) staff       (20)      243 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/PKG-INFO
--rw-r--r--   0 albertstanley   (501) staff       (20)     3530 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/SOURCES.txt
--rw-r--r--   0 albertstanley   (501) staff       (20)        1 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/dependency_links.txt
--rw-r--r--   0 albertstanley   (501) staff       (20)       88 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/entry_points.txt
--rw-r--r--   0 albertstanley   (501) staff       (20)        1 2023-08-03 20:28:34.000000 serra-0.7.11/serra.egg-info/not-zip-safe
--rw-r--r--   0 albertstanley   (501) staff       (20)       83 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/requires.txt
--rw-r--r--   0 albertstanley   (501) staff       (20)        6 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/top_level.txt
--rw-r--r--   0 albertstanley   (501) staff       (20)       38 2023-08-03 20:32:08.737473 serra-0.7.11/setup.cfg
--rw-r--r--   0 albertstanley   (501) staff       (20)      922 2023-08-03 20:32:02.000000 serra-0.7.11/setup.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.414788 serra-0.7.12/
+-rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-08-07 19:19:31.000000 serra-0.7.12/LICENSE.md
+-rw-r--r--   0 alanwang   (501) staff       (20)      243 2023-08-07 19:21:59.414663 serra-0.7.12/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     3917 2023-08-07 19:19:31.000000 serra-0.7.12/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.400475 serra-0.7.12/serra/
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-07 19:19:31.000000 serra-0.7.12/serra/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2006 2023-08-07 19:19:31.000000 serra-0.7.12/serra/aws.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2051 2023-08-07 19:19:31.000000 serra-0.7.12/serra/cli.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      252 2023-08-07 19:19:31.000000 serra-0.7.12/serra/config.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1854 2023-08-07 19:19:31.000000 serra-0.7.12/serra/config_parser.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.396909 serra-0.7.12/serra/data/
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.402132 serra-0.7.12/serra/data/autocomplete/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1110 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/README.md
+-rw-r--r--   0 alanwang   (501) staff       (20)     1636 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/gen_schemas.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.402334 serra-0.7.12/serra/data/autocomplete/inputs/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2249 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/inputs/specs.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.405542 serra-0.7.12/serra/data/autocomplete/output/
+-rw-r--r--   0 alanwang   (501) staff       (20)      391 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/AddColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      276 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/AmazonS3Reader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      341 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/AmazonS3Writer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      267 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/CaseWhenTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      216 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/CastColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      206 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/DatabricksReader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      389 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/DatabricksWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/DropColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/GetCountTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      354 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/JoinTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      148 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/LocalReader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/LocalWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      331 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/MapTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      408 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/PivotTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/RenameColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      210 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/SelectTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/SnowflakeWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)     7553 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/serra_yaml_schema.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.405875 serra-0.7.12/serra/data/autocomplete/templates/
+-rw-r--r--   0 alanwang   (501) staff       (20)      326 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/templates/schema_template.json
+-rw-r--r--   0 alanwang   (501) staff       (20)       95 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/templates/transformer_template.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.406246 serra-0.7.12/serra/data/workspace_example/
+-rw-r--r--   0 alanwang   (501) staff       (20)      137 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.406922 serra-0.7.12/serra/data/workspace_example/examples/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1610 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/examples/ratings.csv
+-rw-r--r--   0 alanwang   (501) staff       (20)     6706 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/examples/sales.csv
+-rw-r--r--   0 alanwang   (501) staff       (20)     1124 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/examples/states_to_abbreviation.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.408405 serra-0.7.12/serra/data/workspace_example/jobs/
+-rw-r--r--   0 alanwang   (501) staff       (20)      912 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/CloudDemo.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      952 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/Demo.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      418 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/LocalExample.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      220 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/ReadExample.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      456 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/ReadJoinWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      393 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/ReadMapWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      397 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/ReadPivotWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      323 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/profiles.yml
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.408798 serra-0.7.12/serra/data/workspace_example/sql/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2603 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/sql/easy_demo.sql
+-rw-r--r--   0 alanwang   (501) staff       (20)     2909 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/sql/hard_demo.sql
+-rw-r--r--   0 alanwang   (501) staff       (20)     2964 2023-08-07 19:19:31.000000 serra-0.7.12/serra/databricks.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-08-07 19:19:31.000000 serra-0.7.12/serra/exceptions.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1120 2023-08-07 19:19:31.000000 serra-0.7.12/serra/profile.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.409785 serra-0.7.12/serra/readers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      201 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2182 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/amazon_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1238 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/databricks_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      962 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/local_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2063 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/snowflaker_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3219 2023-08-07 19:19:31.000000 serra-0.7.12/serra/run.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.410212 serra-0.7.12/serra/runners/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-08-07 19:19:31.000000 serra-0.7.12/serra/runners/ExecutionGraph.py
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-07 19:19:31.000000 serra-0.7.12/serra/runners/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3148 2023-08-07 19:19:31.000000 serra-0.7.12/serra/runners/graph_runner.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      443 2023-08-07 19:19:31.000000 serra-0.7.12/serra/tests.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.413459 serra-0.7.12/serra/transformers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      624 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1512 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/add_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1225 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/aggregate_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/case_when_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1318 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/cast_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1016 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/coalesce_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      875 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/drop_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1002 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/filter_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1138 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/get_count_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      910 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/get_distinct_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1339 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/impute_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2175 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/join_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2867 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/map_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1145 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/order_by_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1986 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/pivot_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1009 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/rename_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1423 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/select_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2293 2023-08-07 19:19:31.000000 serra-0.7.12/serra/utils.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.414433 serra-0.7.12/serra/writers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      200 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2143 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/amazon_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1400 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/databricks_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      957 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/local_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3864 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/snowflake_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/writer.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.401756 serra-0.7.12/serra.egg-info/
+-rw-r--r--   0 alanwang   (501) staff       (20)      243 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     3504 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/SOURCES.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/dependency_links.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/entry_points.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/not-zip-safe
+-rw-r--r--   0 alanwang   (501) staff       (20)       89 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/requires.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/top_level.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-08-07 19:21:59.414829 serra-0.7.12/setup.cfg
+-rw-r--r--   0 alanwang   (501) staff       (20)      940 2023-08-07 19:21:09.000000 serra-0.7.12/setup.py
```

### Comparing `serra-0.7.11/LICENSE.md` & `serra-0.7.12/LICENSE.md`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/README.md` & `serra-0.7.12/README.md`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/aws.py` & `serra-0.7.12/serra/aws.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/cli.py` & `serra-0.7.12/serra/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,54 +3,61 @@
 import click
 
 from serra.run import run_job_from_job_dir, update_package, create_job_yaml, run_job_from_aws, translate_job
 from serra.databricks import create_job
 from serra.utils import validate_workspace
 from serra.config import PACKAGE_PATH
 from serra.utils import copy_folder
+from serra.translate_module.translate_client import reset_serra_token
 
 @click.group()
 def main():
     pass
 
 @main.command(name="start")
 @click.argument("job_name")
 def cli_start(job_name):
-    """Create a yaml for job_name inside the data folder
+    """Create a yaml for job_name
     """
     create_job_yaml(job_name)
 
 @main.command(name="run")
 @click.argument("job_name")
 def cli_run_job_from_job_dir(job_name):
     """Run a specific job locally
     """
     validate_workspace()
     run_job_from_job_dir(job_name)
 
+@main.command(name='configure')
+def cli_configure():
+    """Configure serra_token for serra translate
+    """
+    reset_serra_token()
+
 @main.command(name="translate")
 @click.argument("sql_path")
 @click.option("--run", is_flag=True, default=False, required=False)
 def cli_translator(sql_path, run):
-    """Run a specific job locally
+    """Translate a sql file to a serra config file
     """
     translate_job(sql_path, run)
 
 @main.command(name="create_job")
 @click.argument("job_name")
 def cli_create_job(job_name):
     """Create a databricks job
     """
     validate_workspace()
     create_job(job_name)
 
 @main.command(name="create")
 @click.argument("local_path", type=click.Path(), default="./workspace")
 def cli_create(local_path):
-    """Copy workspace_example folder from S3 to local_path"""
+    """Create starter workspace folder"""
     source_folder = f"{PACKAGE_PATH}/data/workspace_example"
     copy_folder(source_folder, local_path)
 
 @main.command(name="update_package")
 def cli_update_package():
     """Uploads package to aws, and restarts databricks cluster
     """
```

### Comparing `serra-0.7.11/serra/config_parser.py` & `serra-0.7.12/serra/config_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,17 @@
         config_bytes = retrieve_file_from_config_bucket(config_name)
         config = yaml.safe_load(config_bytes)
         return ConfigParser(config)
     
     def get_step(self, block_name):
         return self.config.get(block_name)
     
+    def get_metadata_tags(self):
+        return ['show_all']
+    
     def get_class_name_for_step(self, block_name):
         step = self.get_step(block_name)
         keys = [key for key in step.keys()]
         if "tests" in keys:
             keys.remove("tests")
         return keys[0]
```

### Comparing `serra-0.7.11/serra/data/autocomplete/README.md` & `serra-0.7.12/serra/data/autocomplete/README.md`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/data/autocomplete/gen_schemas.py` & `serra-0.7.12/serra/data/autocomplete/gen_schemas.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/data/autocomplete/inputs/specs.json` & `serra-0.7.12/serra/data/autocomplete/inputs/specs.json`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/data/autocomplete/output/serra_yaml_schema.json` & `serra-0.7.12/serra/data/autocomplete/output/serra_yaml_schema.json`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/data/workspace_example/examples/ratings.csv` & `serra-0.7.12/serra/data/workspace_example/examples/ratings.csv`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/data/workspace_example/examples/sales.csv` & `serra-0.7.12/serra/data/workspace_example/examples/sales.csv`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/data/workspace_example/examples/states_to_abbreviation.json` & `serra-0.7.12/serra/data/workspace_example/examples/states_to_abbreviation.json`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/data/workspace_example/jobs/CloudDemo.yml` & `serra-0.7.12/serra/data/workspace_example/jobs/CloudDemo.yml`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/data/workspace_example/jobs/Demo.yml` & `serra-0.7.12/serra/data/workspace_example/jobs/Demo.yml`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/data/workspace_example/sql/easy_demo.sql` & `serra-0.7.12/serra/data/workspace_example/sql/easy_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/data/workspace_example/sql/hard_demo.sql` & `serra-0.7.12/serra/data/workspace_example/sql/hard_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/databricks.py` & `serra-0.7.12/serra/databricks.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/profile.py` & `serra-0.7.12/serra/profile.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/readers/amazon_reader.py` & `serra-0.7.12/serra/readers/amazon_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/readers/databricks_reader.py` & `serra-0.7.12/serra/readers/databricks_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/readers/local_reader.py` & `serra-0.7.12/serra/readers/local_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/readers/snowflaker_reader.py` & `serra-0.7.12/serra/readers/snowflaker_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/run.py` & `serra-0.7.12/serra/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from loguru import logger
 
 from serra.config_parser import ConfigParser
 from serra.utils import get_path_to_user_configs_folder, write_to_file
 from serra.databricks import upload_wheel_to_bucket, restart_server
 from serra.runners.graph_runner import run_job_with_graph
 from serra.exceptions import SerraRunException
-from serra.translate_client import save_as_yaml, get_translated_yaml
+from serra.translate_module.translate_client import save_as_yaml, get_translated_yaml
+from serra.translate_module.clean import clean_yaml_file
 
 PACKAGE_PATH = os.path.dirname(os.path.dirname(__file__))
 
 # Setup logger
 logger.remove()  # Remove the default sink
 logger.add(sink=sys.stdout, format="<green>{time}</green> - <level>{level}</level> - <cyan>{message}</cyan>", colorize=True)
 
@@ -55,16 +56,22 @@
     translated_yaml = get_translated_yaml(sql_path)
     if not translated_yaml:
         return
 
     # Save in new yaml file (config folder with same name as sql path)
     user_configs_folder = get_path_to_user_configs_folder()
     yaml_path = f"{user_configs_folder}/{yaml_path}.yml"
-    logger.info(f"Translation complete. Yaml file can be found at {os.path.abspath(yaml_path)}")
+    
     save_as_yaml(translated_yaml, yaml_path)
+    clean_yaml_file(yaml_path)
+    # try:
+    #     clean_yaml_file(yaml_path)
+    # except:
+    #     logger.error(f"Error while cleaning translate file")
+    logger.info(f"Translation complete. Yaml file can be found at {os.path.abspath(yaml_path)}")
 
     if is_run:
         logger.info("Running job...")
         cf = ConfigParser.from_local_config(yaml_path)
     # run_job_simple_linear(cf, True)
         try:
             run_job_with_graph(cf)
```

### Comparing `serra-0.7.11/serra/runners/ExecutionGraph.py` & `serra-0.7.12/serra/runners/ExecutionGraph.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/runners/graph_runner.py` & `serra-0.7.12/serra/runners/graph_runner.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/__init__.py` & `serra-0.7.12/serra/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/add_column_transformer.py` & `serra-0.7.12/serra/transformers/add_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/aggregate_transformer.py` & `serra-0.7.12/serra/transformers/aggregate_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/case_when_transformer.py` & `serra-0.7.12/serra/transformers/case_when_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/cast_columns_transformer.py` & `serra-0.7.12/serra/transformers/cast_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/coalesce_transformer.py` & `serra-0.7.12/serra/transformers/coalesce_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/drop_columns_transformer.py` & `serra-0.7.12/serra/transformers/drop_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/filter_transformer.py` & `serra-0.7.12/serra/transformers/filter_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/get_count_transformer.py` & `serra-0.7.12/serra/transformers/get_count_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/get_distinct_transformer.py` & `serra-0.7.12/serra/transformers/get_distinct_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/impute_transformer.py` & `serra-0.7.12/serra/transformers/impute_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/join_transformer.py` & `serra-0.7.12/serra/transformers/join_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/map_transformer.py` & `serra-0.7.12/serra/transformers/map_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/order_by_transformer.py` & `serra-0.7.12/serra/transformers/order_by_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/pivot_transformer.py` & `serra-0.7.12/serra/transformers/pivot_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/rename_column_transformer.py` & `serra-0.7.12/serra/transformers/rename_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/transformers/select_transformer.py` & `serra-0.7.12/serra/transformers/select_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/utils.py` & `serra-0.7.12/serra/utils.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/writers/amazon_writer.py` & `serra-0.7.12/serra/writers/amazon_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/writers/databricks_writer.py` & `serra-0.7.12/serra/writers/databricks_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/writers/local_writer.py` & `serra-0.7.12/serra/writers/local_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra/writers/snowflake_writer.py` & `serra-0.7.12/serra/writers/snowflake_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.11/serra.egg-info/SOURCES.txt` & `serra-0.7.12/serra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 serra/config.py
 serra/config_parser.py
 serra/databricks.py
 serra/exceptions.py
 serra/profile.py
 serra/run.py
 serra/tests.py
-serra/translate_client.py
 serra/utils.py
 serra.egg-info/PKG-INFO
 serra.egg-info/SOURCES.txt
 serra.egg-info/dependency_links.txt
 serra.egg-info/entry_points.txt
 serra.egg-info/not-zip-safe
 serra.egg-info/requires.txt
```

### Comparing `serra-0.7.11/setup.py` & `serra-0.7.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import setup
 
 setup(name='serra',
-      version='0.7.11',
+      version='0.7.12',
       description='Simplified Data Pipelines',
       url='http://github.com',
       author='Serra Technologies',
       author_email='founders@serra.io',
       packages=setuptools.find_packages(),
       package_data={"serra": ["data/workspace_example/*",
                               "data/workspace_example/*/*",
@@ -15,17 +15,18 @@
       install_requires=[
           "click",
           "pyspark",
           "pyyaml", 
           "pandas", 
           "boto3", 
           "databricks-sdk",
+          "wheel",
           "loguru",
           "snowflake-connector-python"
       ],
       zip_safe=False,
       entry_points={
         'console_scripts': [
             'serra=serra.cli:main',
             'serra_databricks=serra.cli:serra_databricks'
         ]
-    })
+    })
```

