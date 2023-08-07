# Comparing `tmp/serra-0.7.12.tar.gz` & `tmp/serra-0.7.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serra-0.7.12.tar", last modified: Mon Aug  7 19:21:59 2023, max compression
+gzip compressed data, was "serra-0.7.13.tar", last modified: Mon Aug  7 20:59:24 2023, max compression
```

## Comparing `serra-0.7.12.tar` & `serra-0.7.13.tar`

### file list

```diff
@@ -1,109 +1,113 @@
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.414788 serra-0.7.12/
--rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-08-07 19:19:31.000000 serra-0.7.12/LICENSE.md
--rw-r--r--   0 alanwang   (501) staff       (20)      243 2023-08-07 19:21:59.414663 serra-0.7.12/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     3917 2023-08-07 19:19:31.000000 serra-0.7.12/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.400475 serra-0.7.12/serra/
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-07 19:19:31.000000 serra-0.7.12/serra/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2006 2023-08-07 19:19:31.000000 serra-0.7.12/serra/aws.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2051 2023-08-07 19:19:31.000000 serra-0.7.12/serra/cli.py
--rw-r--r--   0 alanwang   (501) staff       (20)      252 2023-08-07 19:19:31.000000 serra-0.7.12/serra/config.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1854 2023-08-07 19:19:31.000000 serra-0.7.12/serra/config_parser.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.396909 serra-0.7.12/serra/data/
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.402132 serra-0.7.12/serra/data/autocomplete/
--rw-r--r--   0 alanwang   (501) staff       (20)     1110 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/README.md
--rw-r--r--   0 alanwang   (501) staff       (20)     1636 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/gen_schemas.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.402334 serra-0.7.12/serra/data/autocomplete/inputs/
--rw-r--r--   0 alanwang   (501) staff       (20)     2249 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/inputs/specs.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.405542 serra-0.7.12/serra/data/autocomplete/output/
--rw-r--r--   0 alanwang   (501) staff       (20)      391 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/AddColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      276 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/AmazonS3Reader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      341 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/AmazonS3Writer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      267 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/CaseWhenTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      216 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/CastColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      206 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/DatabricksReader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      389 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/DatabricksWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/DropColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/GetCountTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      354 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/JoinTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      148 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/LocalReader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/LocalWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)      331 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/MapTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      408 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/PivotTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/RenameColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      210 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/SelectTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/SnowflakeWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)     7553 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/output/serra_yaml_schema.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.405875 serra-0.7.12/serra/data/autocomplete/templates/
--rw-r--r--   0 alanwang   (501) staff       (20)      326 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/templates/schema_template.json
--rw-r--r--   0 alanwang   (501) staff       (20)       95 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/autocomplete/templates/transformer_template.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.406246 serra-0.7.12/serra/data/workspace_example/
--rw-r--r--   0 alanwang   (501) staff       (20)      137 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.406922 serra-0.7.12/serra/data/workspace_example/examples/
--rw-r--r--   0 alanwang   (501) staff       (20)     1610 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/examples/ratings.csv
--rw-r--r--   0 alanwang   (501) staff       (20)     6706 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/examples/sales.csv
--rw-r--r--   0 alanwang   (501) staff       (20)     1124 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/examples/states_to_abbreviation.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.408405 serra-0.7.12/serra/data/workspace_example/jobs/
--rw-r--r--   0 alanwang   (501) staff       (20)      912 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/CloudDemo.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      952 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/Demo.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      418 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/LocalExample.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      220 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/ReadExample.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      456 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/ReadJoinWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      393 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/ReadMapWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      397 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/jobs/ReadPivotWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      323 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/profiles.yml
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.408798 serra-0.7.12/serra/data/workspace_example/sql/
--rw-r--r--   0 alanwang   (501) staff       (20)     2603 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/sql/easy_demo.sql
--rw-r--r--   0 alanwang   (501) staff       (20)     2909 2023-08-07 19:19:31.000000 serra-0.7.12/serra/data/workspace_example/sql/hard_demo.sql
--rw-r--r--   0 alanwang   (501) staff       (20)     2964 2023-08-07 19:19:31.000000 serra-0.7.12/serra/databricks.py
--rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-08-07 19:19:31.000000 serra-0.7.12/serra/exceptions.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1120 2023-08-07 19:19:31.000000 serra-0.7.12/serra/profile.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.409785 serra-0.7.12/serra/readers/
--rw-r--r--   0 alanwang   (501) staff       (20)      201 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2182 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/amazon_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1238 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/databricks_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      962 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/local_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2063 2023-08-07 19:19:31.000000 serra-0.7.12/serra/readers/snowflaker_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3219 2023-08-07 19:19:31.000000 serra-0.7.12/serra/run.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.410212 serra-0.7.12/serra/runners/
--rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-08-07 19:19:31.000000 serra-0.7.12/serra/runners/ExecutionGraph.py
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-07 19:19:31.000000 serra-0.7.12/serra/runners/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3148 2023-08-07 19:19:31.000000 serra-0.7.12/serra/runners/graph_runner.py
--rw-r--r--   0 alanwang   (501) staff       (20)      443 2023-08-07 19:19:31.000000 serra-0.7.12/serra/tests.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.413459 serra-0.7.12/serra/transformers/
--rw-r--r--   0 alanwang   (501) staff       (20)      624 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1512 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/add_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1225 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/aggregate_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/case_when_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1318 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/cast_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1016 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/coalesce_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      875 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/drop_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1002 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/filter_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1138 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/get_count_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      910 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/get_distinct_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1339 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/impute_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2175 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/join_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2867 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/map_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1145 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/order_by_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1986 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/pivot_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1009 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/rename_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1423 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/select_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-08-07 19:19:31.000000 serra-0.7.12/serra/transformers/transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2293 2023-08-07 19:19:31.000000 serra-0.7.12/serra/utils.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.414433 serra-0.7.12/serra/writers/
--rw-r--r--   0 alanwang   (501) staff       (20)      200 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2143 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/amazon_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1400 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/databricks_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      957 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/local_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3864 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/snowflake_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-08-07 19:19:31.000000 serra-0.7.12/serra/writers/writer.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-07 19:21:59.401756 serra-0.7.12/serra.egg-info/
--rw-r--r--   0 alanwang   (501) staff       (20)      243 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     3504 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/SOURCES.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/dependency_links.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/entry_points.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/not-zip-safe
--rw-r--r--   0 alanwang   (501) staff       (20)       89 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/requires.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-08-07 19:21:59.000000 serra-0.7.12/serra.egg-info/top_level.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-08-07 19:21:59.414829 serra-0.7.12/setup.cfg
--rw-r--r--   0 alanwang   (501) staff       (20)      940 2023-08-07 19:21:09.000000 serra-0.7.12/setup.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.930601 serra-0.7.13/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3860 2023-08-07 20:58:26.000000 serra-0.7.13/LICENSE.md
+-rw-r--r--   0 albertstanley   (501) staff       (20)      243 2023-08-07 20:59:24.930373 serra-0.7.13/PKG-INFO
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3909 2023-08-07 20:58:26.000000 serra-0.7.13/README.md
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.904590 serra-0.7.13/serra/
+-rw-r--r--   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:58:26.000000 serra-0.7.13/serra/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2006 2023-08-07 20:58:26.000000 serra-0.7.13/serra/aws.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2051 2023-08-07 20:58:26.000000 serra-0.7.13/serra/cli.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      252 2023-08-07 20:58:26.000000 serra-0.7.13/serra/config.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1854 2023-08-07 20:58:26.000000 serra-0.7.13/serra/config_parser.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.895658 serra-0.7.13/serra/data/
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.908962 serra-0.7.13/serra/data/autocomplete/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1110 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/README.md
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1636 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/gen_schemas.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.909263 serra-0.7.13/serra/data/autocomplete/inputs/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2249 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/inputs/specs.json
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.914858 serra-0.7.13/serra/data/autocomplete/output/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      391 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/AddColumnTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      276 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/AmazonS3Reader.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      341 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/AmazonS3Writer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      267 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/CaseWhenTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      216 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/CastColumnTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      206 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/DatabricksReader.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      389 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/DatabricksWriter.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      213 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/DropColumnTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      274 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/GetCountTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      354 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/JoinTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      148 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/LocalReader.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      213 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/LocalWriter.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      331 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/MapTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      408 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/PivotTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      274 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/RenameColumnTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      210 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/SelectTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      452 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/SnowflakeWriter.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)     7553 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/output/serra_yaml_schema.json
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.915372 serra-0.7.13/serra/data/autocomplete/templates/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      326 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/templates/schema_template.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)       95 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/autocomplete/templates/transformer_template.json
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.915984 serra-0.7.13/serra/data/workspace_example/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      137 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/README.md
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.916836 serra-0.7.13/serra/data/workspace_example/examples/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1610 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/examples/ratings.csv
+-rw-r--r--   0 albertstanley   (501) staff       (20)     6706 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/examples/sales.csv
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1124 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/examples/states_to_abbreviation.json
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.918731 serra-0.7.13/serra/data/workspace_example/jobs/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      912 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/jobs/CloudDemo.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      952 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/jobs/Demo.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      418 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/jobs/LocalExample.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      220 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/jobs/ReadExample.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      456 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/jobs/ReadJoinWrite.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      393 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/jobs/ReadMapWrite.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      397 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/jobs/ReadPivotWrite.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      323 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/profiles.yml
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.919370 serra-0.7.13/serra/data/workspace_example/sql/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2603 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/sql/easy_demo.sql
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2909 2023-08-07 20:58:26.000000 serra-0.7.13/serra/data/workspace_example/sql/hard_demo.sql
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2964 2023-08-07 20:58:26.000000 serra-0.7.13/serra/databricks.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      106 2023-08-07 20:58:26.000000 serra-0.7.13/serra/exceptions.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1120 2023-08-07 20:58:26.000000 serra-0.7.13/serra/profile.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.921566 serra-0.7.13/serra/readers/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      201 2023-08-07 20:58:26.000000 serra-0.7.13/serra/readers/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2182 2023-08-07 20:58:26.000000 serra-0.7.13/serra/readers/amazon_reader.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1238 2023-08-07 20:58:26.000000 serra-0.7.13/serra/readers/databricks_reader.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      962 2023-08-07 20:58:26.000000 serra-0.7.13/serra/readers/local_reader.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      277 2023-08-07 20:58:26.000000 serra-0.7.13/serra/readers/reader.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2063 2023-08-07 20:58:26.000000 serra-0.7.13/serra/readers/snowflaker_reader.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3219 2023-08-07 20:58:26.000000 serra-0.7.13/serra/run.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.922276 serra-0.7.13/serra/runners/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2631 2023-08-07 20:58:26.000000 serra-0.7.13/serra/runners/ExecutionGraph.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:58:26.000000 serra-0.7.13/serra/runners/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3148 2023-08-07 20:58:26.000000 serra-0.7.13/serra/runners/graph_runner.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      443 2023-08-07 20:58:26.000000 serra-0.7.13/serra/tests.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.927701 serra-0.7.13/serra/transformers/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      624 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1512 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/add_column_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1225 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/aggregate_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      631 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/case_when_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1318 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/cast_columns_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1016 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/coalesce_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      875 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/drop_columns_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1002 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/filter_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1138 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/get_count_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      910 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/get_distinct_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1339 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/impute_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2175 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/join_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2867 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/map_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1145 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/order_by_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1986 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/pivot_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1009 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/rename_column_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1423 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/select_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      310 2023-08-07 20:58:26.000000 serra-0.7.13/serra/transformers/transformer.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.928490 serra-0.7.13/serra/translate_module/
+-rw-r--r--   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:58:26.000000 serra-0.7.13/serra/translate_module/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1195 2023-08-07 20:58:26.000000 serra-0.7.13/serra/translate_module/clean.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3401 2023-08-07 20:58:26.000000 serra-0.7.13/serra/translate_module/translate_client.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2293 2023-08-07 20:58:26.000000 serra-0.7.13/serra/utils.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.930040 serra-0.7.13/serra/writers/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      200 2023-08-07 20:58:26.000000 serra-0.7.13/serra/writers/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2143 2023-08-07 20:58:26.000000 serra-0.7.13/serra/writers/amazon_writer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1400 2023-08-07 20:58:26.000000 serra-0.7.13/serra/writers/databricks_writer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      957 2023-08-07 20:58:26.000000 serra-0.7.13/serra/writers/local_writer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3864 2023-08-07 20:58:26.000000 serra-0.7.13/serra/writers/snowflake_writer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      284 2023-08-07 20:58:26.000000 serra-0.7.13/serra/writers/writer.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-07 20:59:24.908102 serra-0.7.13/serra.egg-info/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      243 2023-08-07 20:59:24.000000 serra-0.7.13/serra.egg-info/PKG-INFO
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3614 2023-08-07 20:59:24.000000 serra-0.7.13/serra.egg-info/SOURCES.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)        1 2023-08-07 20:59:24.000000 serra-0.7.13/serra.egg-info/dependency_links.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)       88 2023-08-07 20:59:24.000000 serra-0.7.13/serra.egg-info/entry_points.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)        1 2023-08-07 20:59:16.000000 serra-0.7.13/serra.egg-info/not-zip-safe
+-rw-r--r--   0 albertstanley   (501) staff       (20)       89 2023-08-07 20:59:24.000000 serra-0.7.13/serra.egg-info/requires.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)        6 2023-08-07 20:59:24.000000 serra-0.7.13/serra.egg-info/top_level.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)       38 2023-08-07 20:59:24.930675 serra-0.7.13/setup.cfg
+-rw-r--r--   0 albertstanley   (501) staff       (20)      940 2023-08-07 20:58:26.000000 serra-0.7.13/setup.py
```

### Comparing `serra-0.7.12/LICENSE.md` & `serra-0.7.13/LICENSE.md`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/README.md` & `serra-0.7.13/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 Now your jobs can connect between AWS, Databricks, and Snowflake data sources!
 
 # SQL to Serra LLM (Beta)
 Translate monolithic SQL scripts to low-code, Serra spark configuration files with one line.
 
 ```bash
-cd workspace_example
+cd workspace
 serra translate hard_demo.sql
 ```
 Place your sql scripts in **workspace_example/sql** folder.
 
 # Command Line Tool
 Translate, test locally, and run Databricks jobs with single commands.
```

### Comparing `serra-0.7.12/serra/aws.py` & `serra-0.7.13/serra/aws.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/cli.py` & `serra-0.7.13/serra/cli.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/config_parser.py` & `serra-0.7.13/serra/config_parser.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/data/autocomplete/README.md` & `serra-0.7.13/serra/data/autocomplete/README.md`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/data/autocomplete/gen_schemas.py` & `serra-0.7.13/serra/data/autocomplete/gen_schemas.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/data/autocomplete/inputs/specs.json` & `serra-0.7.13/serra/data/autocomplete/inputs/specs.json`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/data/autocomplete/output/serra_yaml_schema.json` & `serra-0.7.13/serra/data/autocomplete/output/serra_yaml_schema.json`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/data/workspace_example/examples/ratings.csv` & `serra-0.7.13/serra/data/workspace_example/examples/ratings.csv`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/data/workspace_example/examples/sales.csv` & `serra-0.7.13/serra/data/workspace_example/examples/sales.csv`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/data/workspace_example/examples/states_to_abbreviation.json` & `serra-0.7.13/serra/data/workspace_example/examples/states_to_abbreviation.json`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/data/workspace_example/jobs/CloudDemo.yml` & `serra-0.7.13/serra/data/workspace_example/jobs/CloudDemo.yml`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/data/workspace_example/jobs/Demo.yml` & `serra-0.7.13/serra/data/workspace_example/jobs/Demo.yml`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/data/workspace_example/sql/easy_demo.sql` & `serra-0.7.13/serra/data/workspace_example/sql/easy_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/data/workspace_example/sql/hard_demo.sql` & `serra-0.7.13/serra/data/workspace_example/sql/hard_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/databricks.py` & `serra-0.7.13/serra/databricks.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/profile.py` & `serra-0.7.13/serra/profile.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/readers/amazon_reader.py` & `serra-0.7.13/serra/readers/amazon_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/readers/databricks_reader.py` & `serra-0.7.13/serra/readers/databricks_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/readers/local_reader.py` & `serra-0.7.13/serra/readers/local_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/readers/snowflaker_reader.py` & `serra-0.7.13/serra/readers/snowflaker_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/run.py` & `serra-0.7.13/serra/run.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/runners/ExecutionGraph.py` & `serra-0.7.13/serra/runners/ExecutionGraph.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/runners/graph_runner.py` & `serra-0.7.13/serra/runners/graph_runner.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/__init__.py` & `serra-0.7.13/serra/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/add_column_transformer.py` & `serra-0.7.13/serra/transformers/add_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/aggregate_transformer.py` & `serra-0.7.13/serra/transformers/aggregate_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/case_when_transformer.py` & `serra-0.7.13/serra/transformers/case_when_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/cast_columns_transformer.py` & `serra-0.7.13/serra/transformers/cast_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/coalesce_transformer.py` & `serra-0.7.13/serra/transformers/coalesce_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/drop_columns_transformer.py` & `serra-0.7.13/serra/transformers/drop_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/filter_transformer.py` & `serra-0.7.13/serra/transformers/filter_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/get_count_transformer.py` & `serra-0.7.13/serra/transformers/get_count_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/get_distinct_transformer.py` & `serra-0.7.13/serra/transformers/get_distinct_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/impute_transformer.py` & `serra-0.7.13/serra/transformers/impute_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/join_transformer.py` & `serra-0.7.13/serra/transformers/join_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/map_transformer.py` & `serra-0.7.13/serra/transformers/map_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/order_by_transformer.py` & `serra-0.7.13/serra/transformers/order_by_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/pivot_transformer.py` & `serra-0.7.13/serra/transformers/pivot_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/rename_column_transformer.py` & `serra-0.7.13/serra/transformers/rename_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/transformers/select_transformer.py` & `serra-0.7.13/serra/transformers/select_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/utils.py` & `serra-0.7.13/serra/utils.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/writers/amazon_writer.py` & `serra-0.7.13/serra/writers/amazon_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/writers/databricks_writer.py` & `serra-0.7.13/serra/writers/databricks_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/writers/local_writer.py` & `serra-0.7.13/serra/writers/local_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra/writers/snowflake_writer.py` & `serra-0.7.13/serra/writers/snowflake_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.12/serra.egg-info/SOURCES.txt` & `serra-0.7.13/serra.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,13 +79,16 @@
 serra/transformers/join_transformer.py
 serra/transformers/map_transformer.py
 serra/transformers/order_by_transformer.py
 serra/transformers/pivot_transformer.py
 serra/transformers/rename_column_transformer.py
 serra/transformers/select_transformer.py
 serra/transformers/transformer.py
+serra/translate_module/__init__.py
+serra/translate_module/clean.py
+serra/translate_module/translate_client.py
 serra/writers/__init__.py
 serra/writers/amazon_writer.py
 serra/writers/databricks_writer.py
 serra/writers/local_writer.py
 serra/writers/snowflake_writer.py
 serra/writers/writer.py
```

### Comparing `serra-0.7.12/setup.py` & `serra-0.7.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import setup
 
 setup(name='serra',
-      version='0.7.12',
+      version='0.7.13',
       description='Simplified Data Pipelines',
       url='http://github.com',
       author='Serra Technologies',
       author_email='founders@serra.io',
       packages=setuptools.find_packages(),
       package_data={"serra": ["data/workspace_example/*",
                               "data/workspace_example/*/*",
```

