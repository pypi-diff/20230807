# Comparing `tmp/fugue-0.8.6.dev3.tar.gz` & `tmp/fugue-0.8.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugue-0.8.6.dev3.tar", last modified: Mon Jul 24 06:45:03 2023, max compression
+gzip compressed data, was "fugue-0.8.7.dev1.tar", last modified: Mon Aug  7 06:18:12 2023, max compression
```

## Comparing `fugue-0.8.6.dev3.tar` & `fugue-0.8.7.dev1.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.126468 fugue-0.8.6.dev3/fugue/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.126468 fugue-0.8.6.dev3/fugue/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/interfaceless.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/_utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.126468 fugue-0.8.6.dev3/fugue/bag/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/bag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/bag/array_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/bag/bag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.126468 fugue-0.8.6.dev3/fugue/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/collections/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/collections/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/collections/yielded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.130468 fugue-0.8.6.dev3/fugue/column/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/column/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/column/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/column/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.130468 fugue-0.8.6.dev3/fugue/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/array_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/arrow_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/dataframe_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataframe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.130468 fugue-0.8.6.dev3/fugue/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataset/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.130468 fugue-0.8.6.dev3/fugue/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/execution/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/execution/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/execution/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/execution/native_execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/_builtins/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/_builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/_builtins/creators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/_builtins/outputters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/_builtins/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/creator/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/creator/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/creator/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/outputter/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/outputter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/outputter/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/outputter/outputter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/processor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/processor/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/extensions/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/transformer/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/transformer/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/extensions/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.134468 fugue-0.8.6.dev3/fugue/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/rpc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/rpc/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/sql/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/sql/_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/sql/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/sql/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.126468 fugue-0.8.6.dev3/fugue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-24 06:45:02.000000 fugue-0.8.6.dev3/fugue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-24 06:45:03.000000 fugue-0.8.6.dev3/fugue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:45:02.000000 fugue-0.8.6.dev3/fugue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 06:45:02.000000 fugue-0.8.6.dev3/fugue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-24 06:45:02.000000 fugue-0.8.6.dev3/fugue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-24 06:45:02.000000 fugue-0.8.6.dev3/fugue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue_contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_contrib/contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue_contrib/seaborn/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_contrib/seaborn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue_contrib/viz/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_contrib/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_contrib/viz/_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.138468 fugue-0.8.6.dev3/fugue_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_dask/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.142468 fugue-0.8.6.dev3/fugue_duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_duckdb/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.142468 fugue-0.8.6.dev3/fugue_ibis/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.142468 fugue-0.8.6.dev3/fugue_ibis/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/execution/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/execution/pandas_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ibis/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.142468 fugue-0.8.6.dev3/fugue_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.146468 fugue-0.8.6.dev3/fugue_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/nbextension/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/nbextension/description.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_notebook/nbextension/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.146468 fugue-0.8.6.dev3/fugue_polars/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_polars/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_polars/polars_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_polars/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.146468 fugue-0.8.6.dev3/fugue_ray/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.146468 fugue-0.8.6.dev3/fugue_ray/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/_utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/_utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_ray/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/fugue_spark/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/fugue_spark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/_utils/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    32440 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_spark/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/fugue_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/fugue_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/bag_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    78396 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/builtin_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/dataframe_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    50948 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/execution_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_test/ibis_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:45:03.150468 fugue-0.8.6.dev3/fugue_version/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/fugue_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-24 06:45:03.154468 fugue-0.8.6.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-24 06:41:34.000000 fugue-0.8.6.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.515510 fugue-0.8.7.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-08-07 06:18:12.515510 fugue-0.8.7.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.499509 fugue-0.8.7.dev1/fugue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.499509 fugue-0.8.7.dev1/fugue/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/_utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/_utils/interfaceless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/_utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.499509 fugue-0.8.7.dev1/fugue/bag/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/bag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/bag/array_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/bag/bag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.499509 fugue-0.8.7.dev1/fugue/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17257 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/collections/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/collections/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/collections/yielded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.499509 fugue-0.8.7.dev1/fugue/column/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/column/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/column/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/column/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.503510 fugue-0.8.7.dev1/fugue/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataframe/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataframe/array_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataframe/arrow_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataframe/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataframe/dataframe_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataframe/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataframe/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataframe/iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataframe/pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataframe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.503510 fugue-0.8.7.dev1/fugue/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataset/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.503510 fugue-0.8.7.dev1/fugue/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/execution/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47735 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/execution/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/execution/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14388 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/execution/native_execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.503510 fugue-0.8.7.dev1/fugue/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.503510 fugue-0.8.7.dev1/fugue/extensions/_builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/_builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/_builtins/creators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/_builtins/outputters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/_builtins/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.503510 fugue-0.8.7.dev1/fugue/extensions/creator/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/creator/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/creator/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.503510 fugue-0.8.7.dev1/fugue/extensions/outputter/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/outputter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/outputter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/outputter/outputter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.503510 fugue-0.8.7.dev1/fugue/extensions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/processor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/processor/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.507510 fugue-0.8.7.dev1/fugue/extensions/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/transformer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/transformer/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/extensions/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.507510 fugue-0.8.7.dev1/fugue/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/rpc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/rpc/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.507510 fugue-0.8.7.dev1/fugue/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/sql/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/sql/_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/sql/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/sql/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.507510 fugue-0.8.7.dev1/fugue/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/workflow/_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/workflow/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/workflow/_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/workflow/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/workflow/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.499509 fugue-0.8.7.dev1/fugue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-08-07 06:18:11.000000 fugue-0.8.7.dev1/fugue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-08-07 06:18:12.000000 fugue-0.8.7.dev1/fugue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:18:11.000000 fugue-0.8.7.dev1/fugue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-07 06:18:11.000000 fugue-0.8.7.dev1/fugue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-07 06:18:11.000000 fugue-0.8.7.dev1/fugue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-07 06:18:11.000000 fugue-0.8.7.dev1/fugue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.507510 fugue-0.8.7.dev1/fugue_contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_contrib/contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.507510 fugue-0.8.7.dev1/fugue_contrib/seaborn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_contrib/seaborn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.507510 fugue-0.8.7.dev1/fugue_contrib/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_contrib/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_contrib/viz/_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.507510 fugue-0.8.7.dev1/fugue_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_dask/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_dask/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_dask/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_dask/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19115 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_dask/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_dask/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_dask/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.511510 fugue-0.8.7.dev1/fugue_duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_duckdb/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_duckdb/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_duckdb/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_duckdb/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_duckdb/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_duckdb/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_duckdb/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.511510 fugue-0.8.7.dev1/fugue_ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ibis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ibis/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ibis/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ibis/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.511510 fugue-0.8.7.dev1/fugue_ibis/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ibis/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ibis/execution/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ibis/execution/pandas_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ibis/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ibis/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.511510 fugue-0.8.7.dev1/fugue_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.511510 fugue-0.8.7.dev1/fugue_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_notebook/nbextension/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_notebook/nbextension/description.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_notebook/nbextension/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.511510 fugue-0.8.7.dev1/fugue_polars/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_polars/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_polars/polars_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_polars/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.511510 fugue-0.8.7.dev1/fugue_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ray/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.515510 fugue-0.8.7.dev1/fugue_ray/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ray/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ray/_utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ray/_utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ray/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ray/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ray/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_ray/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.515510 fugue-0.8.7.dev1/fugue_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_spark/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.515510 fugue-0.8.7.dev1/fugue_spark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_spark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_spark/_utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_spark/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_spark/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_spark/_utils/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_spark/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32468 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_spark/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_spark/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_spark/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.515510 fugue-0.8.7.dev1/fugue_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.515510 fugue-0.8.7.dev1/fugue_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_test/bag_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78385 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_test/builtin_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_test/dataframe_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52069 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_test/execution_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_test/ibis_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:18:12.515510 fugue-0.8.7.dev1/fugue_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/fugue_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-07 06:18:12.515510 fugue-0.8.7.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-07 06:14:49.000000 fugue-0.8.7.dev1/setup.py
```

### Comparing `fugue-0.8.6.dev3/LICENSE` & `fugue-0.8.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/PKG-INFO` & `fugue-0.8.7.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.6.dev3
+Version: 0.8.7.dev1
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
```

### Comparing `fugue-0.8.6.dev3/README.md` & `fugue-0.8.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/__init__.py` & `fugue-0.8.7.dev1/fugue/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/_utils/display.py` & `fugue-0.8.7.dev1/fugue/_utils/display.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/_utils/exception.py` & `fugue-0.8.7.dev1/fugue/_utils/exception.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/_utils/interfaceless.py` & `fugue-0.8.7.dev1/fugue/_utils/interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/_utils/io.py` & `fugue-0.8.7.dev1/fugue/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/_utils/misc.py` & `fugue-0.8.7.dev1/fugue/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/api.py` & `fugue-0.8.7.dev1/fugue/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/bag/array_bag.py` & `fugue-0.8.7.dev1/fugue/bag/array_bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/bag/bag.py` & `fugue-0.8.7.dev1/fugue/bag/bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/collections/partition.py` & `fugue-0.8.7.dev1/fugue/collections/partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         >>> PartitionSpec("a")  # == PartitionSpec(by=["a"])
         >>> PartitionSpec("per_row")  # == PartitionSpec(num="ROWCOUNT", algo="even")
 
     It's important to understand this concept, please read |PartitionTutorial|
 
     Partition consists for these specs:
 
-    * **algo**: can be one of ``hash`` (default), ``rand``, ``even`` or ``coarse``
+    * **algo**: can be one of ``default``, ``hash``, ``rand``, ``even`` or ``coarse``
     * **num** or **num_partitions**: number of physical partitions, it can be an
       expression or integer numbers, e.g ``(ROWCOUNT+4) / 3``
     * **by** or **partition_by**: keys to partition on
     * **presort**: keys to sort other than partition keys. E.g. ``a``
       and ``a asc`` means presort by column a ascendingly, ``a,b desc``
       means presort by a ascendingly and then by b descendingly.
     * row_limit and size_limit are to be deprecated
@@ -204,18 +204,18 @@
             if k in expr:
                 value = str(v())
                 expr = expr.replace(k, value)
         return int(eval(expr))  # pylint: disable=W0123
 
     @property
     def algo(self) -> str:
-        """Get algo of the spec, one of ``hash`` (default),
+        """Get algo of the spec, one of ``default``, ``hash``,
         ``rand`` ``even`` or ``coarse``
         """
-        return self._algo if self._algo != "" else "hash"
+        return self._algo if self._algo != "" else "default"
 
     @property
     def partition_by(self) -> List[str]:
         """Get partition keys of the spec"""
         return self._partition_by
 
     @property
```

### Comparing `fugue-0.8.6.dev3/fugue/collections/sql.py` & `fugue-0.8.7.dev1/fugue/collections/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/collections/yielded.py` & `fugue-0.8.7.dev1/fugue/collections/yielded.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/column/expressions.py` & `fugue-0.8.7.dev1/fugue/column/expressions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/column/functions.py` & `fugue-0.8.7.dev1/fugue/column/functions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/column/sql.py` & `fugue-0.8.7.dev1/fugue/column/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/constants.py` & `fugue-0.8.7.dev1/fugue/constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataframe/__init__.py` & `fugue-0.8.7.dev1/fugue/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataframe/api.py` & `fugue-0.8.7.dev1/fugue/dataframe/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataframe/array_dataframe.py` & `fugue-0.8.7.dev1/fugue/dataframe/array_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataframe/arrow_dataframe.py` & `fugue-0.8.7.dev1/fugue/dataframe/arrow_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataframe/dataframe.py` & `fugue-0.8.7.dev1/fugue/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataframe/dataframe_iterable_dataframe.py` & `fugue-0.8.7.dev1/fugue/dataframe/dataframe_iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataframe/dataframes.py` & `fugue-0.8.7.dev1/fugue/dataframe/dataframes.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataframe/function_wrapper.py` & `fugue-0.8.7.dev1/fugue/dataframe/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataframe/iterable_dataframe.py` & `fugue-0.8.7.dev1/fugue/dataframe/iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataframe/pandas_dataframe.py` & `fugue-0.8.7.dev1/fugue/dataframe/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataframe/utils.py` & `fugue-0.8.7.dev1/fugue/dataframe/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-import base64
-import json
 import os
 import pickle
-from typing import Any, Iterable, List, Optional, Tuple
+from typing import Any, Iterable, Optional, Tuple
 
 import pandas as pd
 import pyarrow as pa
 from fs import open_fs
 from triad import FileSystem, Schema
 from triad.collections.schema import SchemaError
 from triad.exceptions import InvalidOperationError
 from triad.utils.assertion import assert_arg_not_none
 from triad.utils.assertion import assert_or_throw as aot
 
-from .api import get_column_names, normalize_column_names, rename, as_fugue_df
-from .array_dataframe import ArrayDataFrame
+from .api import as_fugue_df, get_column_names, normalize_column_names, rename
 from .dataframe import DataFrame, LocalBoundedDataFrame
-from .pandas_dataframe import PandasDataFrame
 
 # For backward compatibility, TODO: remove!
 get_dataframe_column_names = get_column_names
 normalize_dataframe_column_names = normalize_column_names
 rename_dataframe_column_names = rename
 
 
@@ -105,125 +101,80 @@
         return True
     except AssertionError:
         if throw:
             raise
         return False
 
 
-def pickle_df(df: DataFrame) -> bytes:
-    """Pickles a dataframe to bytes array. It firstly converts the dataframe
-    local bounded, and then serialize the underlying data.
-
-    :param df: input DataFrame
-    :return: pickled binary data
-
-    .. note::
-
-        Be careful to use on large dataframes or non-local, un-materialized dataframes,
-        it can be slow. You should always use :func:`.unpickle_df` to deserialize.
-    """
-    df = df.as_local_bounded()
-    o: List[Any] = [df.schema]
-    if isinstance(df, PandasDataFrame):
-        o.append("p")
-        o.append(df.native)
-    else:
-        o.append("a")
-        o.append(df.as_array())
-    return pickle.dumps(o)
-
-
 def serialize_df(
     df: Optional[DataFrame],
     threshold: int = -1,
     file_path: Optional[str] = None,
     fs: Optional[FileSystem] = None,
-) -> str:
+) -> Optional[bytes]:
     """Serialize input dataframe to base64 string or to file
     if it's larger than threshold
 
     :param df: input DataFrame
     :param threshold: file byte size threshold, defaults to -1
     :param file_path: file path to store the data (used only if the serialized data
       is larger than ``threshold``), defaults to None
     :param fs: :class:`~triad:triad.collections.fs.FileSystem`, defaults to None
     :raises InvalidOperationError: if file is large but ``file_path`` is not provided
-    :return: a json string either containing the base64 data or the file path
+    :return: a pickled blob either containing the data or the file path
 
     .. note::
 
         If fs is not provided but it needs to write to disk, then it will use
         :meth:`~fs:fs.opener.registry.Registry.open_fs` to try to open the file to
         write.
     """
     if df is None:
-        return json.dumps(dict())
-    data = pickle_df(df)
+        return None
+    data = pickle.dumps(df.as_local_bounded())
     size = len(data)
     if threshold < 0 or size <= threshold:
-        res = dict(data=base64.b64encode(data).decode())
+        return data
     else:
         if file_path is None:
             raise InvalidOperationError("file_path is not provided")
         if fs is None:
             with open_fs(
                 os.path.dirname(file_path), writeable=True, create=False
             ) as _fs:
                 _fs.writebytes(os.path.basename(file_path), data)
         else:
             fs.writebytes(file_path, data)
-        res = dict(path=file_path)
-    return json.dumps(res)
-
-
-def unpickle_df(stream: bytes) -> LocalBoundedDataFrame:
-    """Unpickles a dataframe from bytes array.
-
-    :param stream: binary data
-    :return: unpickled dataframe
-
-    .. note::
-
-        The data must be serialized by :func:`.pickle_df` to deserialize.
-    """
-    o = pickle.loads(stream)
-    schema = o[0]
-    if o[1] == "p":
-        return PandasDataFrame(o[2], schema)
-    if o[1] == "a":
-        return ArrayDataFrame(o[2], schema)
-    raise NotImplementedError(  # pragma: no cover
-        f"{o[1]} is not supported for unpickle"
-    )
+        return pickle.dumps(file_path)
 
 
 def deserialize_df(
-    json_str: str, fs: Optional[FileSystem] = None
+    data: Optional[bytes], fs: Optional[FileSystem] = None
 ) -> Optional[LocalBoundedDataFrame]:
     """Deserialize json string to
     :class:`~fugue.dataframe.dataframe.LocalBoundedDataFrame`
 
     :param json_str: json string containing the base64 data or a file path
     :param fs: :class:`~triad:triad.collections.fs.FileSystem`, defaults to None
     :raises ValueError: if the json string is invalid, not generated from
       :func:`~.serialize_df`
     :return: :class:`~fugue.dataframe.dataframe.LocalBoundedDataFrame` if ``json_str``
       contains a dataframe or None if its valid but contains no data
     """
-    d = json.loads(json_str)
-    if len(d) == 0:
+    if data is None:
         return None
-    if "data" in d:
-        return unpickle_df(base64.b64decode(d["data"].encode()))
-    elif "path" in d:
+    obj = pickle.loads(data)
+    if isinstance(obj, LocalBoundedDataFrame):
+        return obj
+    elif isinstance(obj, str):
         if fs is None:
-            with open_fs(os.path.dirname(d["path"]), create=False) as _fs:
-                return unpickle_df(_fs.readbytes(os.path.basename(d["path"])))
-        return unpickle_df(fs.readbytes(d["path"]))
-    raise ValueError(f"{json_str} is invalid")
+            with open_fs(os.path.dirname(obj), create=False) as _fs:
+                return pickle.loads(_fs.readbytes(os.path.basename(obj)))
+        return pickle.loads(fs.readbytes(obj))
+    raise ValueError("data is invalid")
 
 
 def get_join_schemas(
     df1: DataFrame, df2: DataFrame, how: str, on: Optional[Iterable[str]]
 ) -> Tuple[Schema, Schema]:
     """Get :class:`~triad:triad.collections.schema.Schema` object after
     joining ``df1`` and ``df2``. If ``on`` is not empty, it's mainly for
```

### Comparing `fugue-0.8.6.dev3/fugue/dataset/api.py` & `fugue-0.8.7.dev1/fugue/dataset/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dataset/dataset.py` & `fugue-0.8.7.dev1/fugue/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/dev.py` & `fugue-0.8.7.dev1/fugue/dev.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/exceptions.py` & `fugue-0.8.7.dev1/fugue/exceptions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/execution/api.py` & `fugue-0.8.7.dev1/fugue/execution/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/execution/execution_engine.py` & `fugue-0.8.7.dev1/fugue/execution/execution_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from contextvars import ContextVar
 from typing import (
     Any,
     Callable,
     Dict,
-    Iterable,
     Iterator,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
@@ -19,15 +18,14 @@
 from uuid import uuid4
 
 from triad import ParamDict, Schema, SerializableRLock, assert_or_throw, to_uuid
 from triad.collections.fs import FileSystem
 from triad.collections.function_wrapper import AnnotatedParam
 from triad.exceptions import InvalidOperationError
 from triad.utils.convert import to_size
-from triad.utils.string import validate_triad_var_name
 
 from fugue.bag import Bag, LocalBag
 from fugue.collections.partition import (
     BagPartitionCursor,
     PartitionCursor,
     PartitionSpec,
 )
@@ -42,24 +40,38 @@
     is_agg,
 )
 from fugue.constants import _FUGUE_GLOBAL_CONF, FUGUE_SQL_DEFAULT_DIALECT
 from fugue.dataframe import AnyDataFrame, DataFrame, DataFrames, fugue_annotated_param
 from fugue.dataframe.array_dataframe import ArrayDataFrame
 from fugue.dataframe.dataframe import LocalDataFrame
 from fugue.dataframe.utils import deserialize_df, serialize_df
-from fugue.exceptions import FugueBug, FugueWorkflowRuntimeError
+from fugue.exceptions import FugueWorkflowRuntimeError
 
 AnyExecutionEngine = TypeVar("AnyExecutionEngine", object, None)
 
 _FUGUE_EXECUTION_ENGINE_CONTEXT = ContextVar(
     "_FUGUE_EXECUTION_ENGINE_CONTEXT", default=None
 )
 
 _CONTEXT_LOCK = SerializableRLock()
 
+_FUGUE_SERIALIZED_BLOB_COL = "__fugue_serialized_blob__"
+_FUGUE_SERIALIZED_BLOB_NO_COL = "__fugue_serialized_blob_no__"
+_FUGUE_SERIALIZED_BLOB_NAME_COL = "__fugue_serialized_blob_name__"
+_FUGUE_SERIALIZED_BLOB_DUMMY_COL = "__fugue_serialized_blob_dummy__"
+
+_FUGUE_SERIALIZED_BLOB_SCHEMA = Schema(
+    {
+        _FUGUE_SERIALIZED_BLOB_COL: bytes,
+        _FUGUE_SERIALIZED_BLOB_NO_COL: int,
+        _FUGUE_SERIALIZED_BLOB_NAME_COL: str,
+        _FUGUE_SERIALIZED_BLOB_DUMMY_COL: int,
+    }
+)
+
 
 class _GlobalExecutionEngineContext:
     def __init__(self):
         self._engine: Optional["ExecutionEngine"] = None
 
     def set(self, engine: Optional["ExecutionEngine"]):
         with _CONTEXT_LOCK:
@@ -952,176 +964,109 @@
             then the spark dataframe will be invalid. So you may consider converting
             it to a local dataframe so it can still exist after the engine stops.
         """
         return df.as_local() if as_local else df
 
     def zip(
         self,
-        df1: DataFrame,
-        df2: DataFrame,
+        dfs: DataFrames,
         how: str = "inner",
         partition_spec: Optional[PartitionSpec] = None,
         temp_path: Optional[str] = None,
         to_file_threshold: Any = -1,
-        df1_name: Optional[str] = None,
-        df2_name: Optional[str] = None,
-    ):
-        """Partition the two dataframes in the same way with ``partition_spec`` and
-        zip the partitions together on the partition keys.
+    ) -> DataFrame:
+        """Zip multiple dataframes together with given partition
+        specifications.
 
-        :param df1: the first dataframe
-        :param df2: the second dataframe
+        :param dfs: |DataFramesLikeObject|
         :param how: can accept ``inner``, ``left_outer``, ``right_outer``,
           ``full_outer``, ``cross``, defaults to ``inner``
-        :param partition_spec: partition spec to partition each dataframe,
-          defaults to empty.
-        :type partition_spec: PartitionSpec, optional
+        :param partition_spec: |PartitionLikeObject|, defaults to empty.
         :param temp_path: file path to store the data (used only if the serialized data
           is larger than ``to_file_threshold``), defaults to None
         :param to_file_threshold: file byte size threshold, defaults to -1
-        :param df1_name: df1's name in the zipped dataframe, defaults to None
-        :param df2_name: df2's name in the zipped dataframe, defaults to None
 
         :return: a zipped dataframe, the metadata of the
-          dataframe will indicate it's zipped
+          dataframe will indicated it's zipped
 
         .. note::
 
-            * Different from join, ``df1`` and ``df2`` can have common columns that you
+            * Different from join, dataframes can have common columns that you
               will not use as partition keys.
-            * If ``on`` is not specified it will also use the common columns of the two
+            * If ``by`` is not specified it will also use the common columns of all the
               dataframes (if it's not a cross zip)
-            * For non-cross zip, the two dataframes must have common columns, or error
+            * For non-cross zip, the dataframes must have common columns, or error
               will be thrown
 
+        .. note::
+
+            * Please also read :meth:`~.zip`
+            * If ``dfs`` is dict like, the zipped dataframe will be dict like,
+              If ``dfs`` is list like, the zipped dataframe will be list like
+            * It's fine to contain only one dataframe in ``dfs``
+
         .. seealso::
 
-            For more details and examples, read |ZipComap|.
+            For more details and examples, read |ZipComap|
         """
+        assert_or_throw(len(dfs) > 0, "can't zip 0 dataframes")
+        assert_or_throw(
+            how in ["inner", "left_outer", "right_outer", "full_outer", "cross"],
+            NotImplementedError(f"unsupported join type {how}"),
+        )
+
         partition_spec = partition_spec or PartitionSpec()
         on = list(partition_spec.partition_by)
         how = how.lower()
-        assert_or_throw(
-            "semi" not in how and "anti" not in how,
-            InvalidOperationError("zip does not support semi or anti joins"),
-        )
-        serialized_cols: Dict[str, Any] = {}
-        schemas: Dict[str, Any] = {}
-        if len(on) == 0:
-            if how != "cross":
-                on = df1.schema.extract(
-                    df2.schema.names, ignore_key_mismatch=True
-                ).names
+        if len(dfs) > 1:
+            if len(on) == 0:
+                if how != "cross":
+                    on = list(
+                        set.intersection(*[set(x.schema.names) for x in dfs.values()])
+                    )
+                    assert_or_throw(len(on) > 0, "no common columns found")
+            else:
+                assert_or_throw(
+                    how != "cross",
+                    InvalidOperationError("can't specify keys for cross join"),
+                )
+            partition_spec = PartitionSpec(partition_spec, by=on)
         else:
-            assert_or_throw(
-                how != "cross",
-                InvalidOperationError("can't specify keys for cross join"),
-            )
-        partition_spec = PartitionSpec(partition_spec, by=on)
+            if len(on) == 0:
+                partition_spec = PartitionSpec(num=1)
+            else:
+                partition_spec = PartitionSpec(partition_spec, by=on)
 
-        def update_df(df: DataFrame, name: Optional[str]) -> DataFrame:
-            if name is None:
-                name = f"_{len(serialized_cols)}"
-            if not df.metadata.get("serialized", False):
-                df = self._serialize_by_partition(
-                    df,
-                    partition_spec or PartitionSpec(),
-                    name,
+        pairs = list(dfs.items())
+        schemas: Dict[Any, Schema] = {}
+        ser_dfs: List[DataFrame] = []
+        for i in range(len(dfs)):
+            ser_dfs.append(
+                self._serialize_by_partition(
+                    self.to_df(pairs[i][1]),
+                    partition_spec,
+                    i,
+                    pairs[i][0] if dfs.has_key else None,
                     temp_path,
                     to_file_threshold,
-                    has_name=name is not None,
                 )
-            for k in df.metadata["serialized_cols"].keys():
-                assert_or_throw(
-                    k not in serialized_cols, lambda: ValueError(f"{k} is duplicated")
-                )
-                serialized_cols[k] = df.metadata["serialized_cols"][k]
-                schemas[k] = df.metadata["schemas"][k]
-            return df
-
-        df1 = update_df(df1, df1_name)
-        df2 = update_df(df2, df2_name)
+            )
+            schemas[pairs[i][0] if dfs.has_key else i] = pairs[i][1].schema
+        res = ser_dfs[0]
+        for i in range(1, len(dfs)):
+            res = self.union(res, ser_dfs[i], distinct=False)
         metadata = dict(
             serialized=True,
-            serialized_cols=serialized_cols,
             schemas=schemas,
-            serialized_has_name=df1_name is not None or df2_name is not None,
+            serialized_has_name=dfs.has_key,
+            serialized_join_how=how,
         )
-        res = self.join(df1, df2, how=how, on=on)
         res.reset_metadata(metadata)
         return res
 
-    def zip_all(
-        self,
-        dfs: DataFrames,
-        how: str = "inner",
-        partition_spec: Optional[PartitionSpec] = None,
-        temp_path: Optional[str] = None,
-        to_file_threshold: Any = -1,
-    ) -> DataFrame:
-        """Zip multiple dataframes together with given partition
-        specifications.
-
-        :param dfs: |DataFramesLikeObject|
-        :param how: can accept ``inner``, ``left_outer``, ``right_outer``,
-          ``full_outer``, ``cross``, defaults to ``inner``
-        :param partition_spec: |PartitionLikeObject|, defaults to empty.
-        :param temp_path: file path to store the data (used only if the serialized data
-          is larger than ``to_file_threshold``), defaults to None
-        :param to_file_threshold: file byte size threshold, defaults to -1
-
-        :return: a zipped dataframe, the metadata of the
-          dataframe will indicated it's zipped
-
-        .. note::
-
-            * Please also read :meth:`~.zip`
-            * If ``dfs`` is dict like, the zipped dataframe will be dict like,
-              If ``dfs`` is list like, the zipped dataframe will be list like
-            * It's fine to contain only one dataframe in ``dfs``
-
-        .. seealso::
-
-            For more details and examples, read |ZipComap|
-        """
-        partition_spec = partition_spec or PartitionSpec()
-        assert_or_throw(len(dfs) > 0, "can't zip 0 dataframes")
-        pairs = list(dfs.items())
-        has_name = dfs.has_key
-        if len(dfs) == 1:
-            return self._serialize_by_partition(
-                pairs[0][1],
-                partition_spec,
-                pairs[0][0],
-                temp_path,
-                to_file_threshold,
-                has_name=has_name,
-            )
-        df = self.zip(
-            pairs[0][1],
-            pairs[1][1],
-            how=how,
-            partition_spec=partition_spec,
-            temp_path=temp_path,
-            to_file_threshold=to_file_threshold,
-            df1_name=pairs[0][0] if has_name else None,
-            df2_name=pairs[1][0] if has_name else None,
-        )
-        for i in range(2, len(dfs)):
-            df = self.zip(
-                df,
-                pairs[i][1],
-                how=how,
-                partition_spec=partition_spec,
-                temp_path=temp_path,
-                to_file_threshold=to_file_threshold,
-                df2_name=pairs[i][0] if has_name else None,
-            )
-        return df
-
     def comap(
         self,
         df: DataFrame,
         map_func: Callable[[PartitionCursor, DataFrames], LocalDataFrame],
         output_schema: Any,
         partition_spec: PartitionSpec,
         on_init: Optional[Callable[[int, DataFrames], Any]] = None,
@@ -1157,17 +1102,21 @@
               but has all empty dataframes, you can use the schemas but not the data.
 
         .. seealso::
 
             For more details and examples, read |ZipComap|
         """
         assert_or_throw(df.metadata["serialized"], ValueError("df is not serilaized"))
-        cs = _Comap(df, map_func, on_init)
-        key_schema = df.schema - list(df.metadata["serialized_cols"].values())
-        partition_spec = PartitionSpec(partition_spec, by=list(key_schema.keys()))
+        key_schema = df.schema - _FUGUE_SERIALIZED_BLOB_SCHEMA
+        cs = _Comap(df, key_schema, map_func, output_schema, on_init)
+        partition_spec = PartitionSpec(
+            partition_spec,
+            by=key_schema.names + [_FUGUE_SERIALIZED_BLOB_DUMMY_COL],
+            presort=_FUGUE_SERIALIZED_BLOB_NO_COL,
+        )
         return self.map_engine.map_dataframe(
             df, cs.run, output_schema, partition_spec, on_init=cs.on_init
         )
 
     def load_yielded(self, df: Yielded) -> DataFrame:
         """Load yielded dataframe
 
@@ -1269,43 +1218,38 @@
         if self._ctx_count == 0:
             self.stop()
 
     def _serialize_by_partition(
         self,
         df: DataFrame,
         partition_spec: PartitionSpec,
-        df_name: str,
-        temp_path: Optional[str] = None,
-        to_file_threshold: Any = -1,
-        has_name: bool = False,
+        df_no: int,
+        df_name: Optional[str],
+        temp_path: Optional[str],
+        to_file_threshold: Any,
     ) -> DataFrame:
         to_file_threshold = _get_file_threshold(to_file_threshold)
         on = list(filter(lambda k: k in df.schema, partition_spec.partition_by))
         presort = list(
             filter(lambda p: p[0] in df.schema, partition_spec.presort.items())
         )
-        col_name = _df_name_to_serialize_col(df_name)
         if len(on) == 0:
-            partition_spec = PartitionSpec(
+            _partition_spec = PartitionSpec(
                 partition_spec, num=1, by=[], presort=presort
             )
-            output_schema = Schema(f"{col_name}:str")
+            output_schema = _FUGUE_SERIALIZED_BLOB_SCHEMA
         else:
-            partition_spec = PartitionSpec(partition_spec, by=on, presort=presort)
-            output_schema = partition_spec.get_key_schema(df.schema) + f"{col_name}:str"
-        s = _PartitionSerializer(output_schema, temp_path, to_file_threshold)
-        metadata = dict(
-            serialized=True,
-            serialized_cols={df_name: col_name},
-            schemas={df_name: str(df.schema)},
-            serialized_has_name=has_name,
+            _partition_spec = PartitionSpec(partition_spec, by=on, presort=presort)
+            output_schema = (
+                partition_spec.get_key_schema(df.schema) + _FUGUE_SERIALIZED_BLOB_SCHEMA
+            )
+        s = _PartitionSerializer(
+            output_schema, df_no, df_name, temp_path, to_file_threshold
         )
-        res = self.map_engine.map_dataframe(df, s.run, output_schema, partition_spec)
-        res.reset_metadata(metadata)
-        return res
+        return self.map_engine.map_dataframe(df, s.run, output_schema, _partition_spec)
 
 
 @fugue_annotated_param(ExecutionEngine, "e", child_can_reuse_code=True)
 class ExecutionEngineParam(AnnotatedParam):
     def __init__(
         self,
         param: Optional[inspect.Parameter],
@@ -1328,78 +1272,96 @@
     if size is None:
         return -1
     if isinstance(size, int):
         return size
     return to_size(size)
 
 
-def _df_name_to_serialize_col(name: str):
-    assert_or_throw(name is not None, "Dataframe name can't be None")
-    name = "__blob__" + name + "__"
-    assert_or_throw(validate_triad_var_name(name), "Invalid name " + name)
-    return name
-
-
-class _PartitionSerializer(object):
+class _PartitionSerializer:
     def __init__(
-        self, output_schema: Schema, temp_path: Optional[str], to_file_threshold: int
+        self,
+        output_schema: Schema,
+        no: int,
+        name: Optional[str],
+        temp_path: Optional[str],
+        to_file_threshold: int,
     ):
         self.output_schema = output_schema
+        self.no = no
+        self.name = name
         self.temp_path = temp_path
         self.to_file_threshold = to_file_threshold
 
     def run(self, cursor: PartitionCursor, df: LocalDataFrame) -> LocalDataFrame:
         data = serialize_df(df, self.to_file_threshold, self.temp_path)
-        row = cursor.key_value_array + [data]
+        row = cursor.key_value_array + [data, self.no, self.name, 1]
         return ArrayDataFrame([row], self.output_schema)
 
 
-class _Comap(object):
+class _Comap:
     def __init__(
         self,
         df: DataFrame,
+        key_schema: Schema,
         func: Callable,
+        output_schema: Schema,
         on_init: Optional[Callable[[int, DataFrames], Any]],
     ):
         self.schemas = df.metadata["schemas"]
-        self.df_idx = [
-            (df.schema.index_of_key(v), k, self.schemas[k])
-            for k, v in df.metadata["serialized_cols"].items()
-        ]
-        self.named = df.metadata.get("serialized_has_name", False)
+        self.key_schema = key_schema
+        self.output_schema = output_schema
+        self.dfs_count = len(self.schemas)
+        self.named = df.metadata.get_or_throw("serialized_has_name", bool)
         self.func = func
+        self.how = df.metadata.get_or_throw("serialized_join_how", str)
         self._on_init = on_init
 
     def on_init(self, partition_no, df: DataFrame) -> None:
         if self._on_init is None:
             return
         # TODO: currently, get_output_schema only gets empty dataframes
         empty_dfs = _generate_comap_empty_dfs(self.schemas, self.named)
         self._on_init(partition_no, empty_dfs)
 
     def run(self, cursor: PartitionCursor, df: LocalDataFrame) -> LocalDataFrame:
-        data = df.as_array(type_safe=True)
-        assert_or_throw(
-            len(data) == 1,
-            FugueBug("each comap partition can have one and only one row"),
+        data = list(df.as_dict_iterable())
+        if self.how == "inner":
+            if len(data) < self.dfs_count:
+                return ArrayDataFrame([], self.output_schema)
+        elif self.how == "left_outer":
+            if data[0][_FUGUE_SERIALIZED_BLOB_NO_COL] > 0:
+                return ArrayDataFrame([], self.output_schema)
+        elif self.how == "right_outer":
+            if data[-1][_FUGUE_SERIALIZED_BLOB_NO_COL] != self.dfs_count - 1:
+                return ArrayDataFrame([], self.output_schema)
+        dfs = self._get_dfs(data)
+
+        # construct a cursor without dummy col
+        _c = PartitionSpec(by=self.key_schema.names).get_cursor(
+            dfs[0].schema, cursor.physical_partition_no
         )
-        dfs = DataFrames(list(self._get_dfs(data[0])))
-        return self.func(cursor, dfs)
+        _c.set(lambda: dfs[0].peek_array(), cursor.partition_no, cursor.slice_no)
+        return self.func(_c, dfs)
 
-    def _get_dfs(self, row: Any) -> Iterable[Any]:
-        for k, name, v in self.df_idx:
-            if row[k] is None:
-                df: DataFrame = ArrayDataFrame([], v)
-            else:
-                df = deserialize_df(row[k])  # type: ignore
-                assert df is not None
-            if self.named:
-                yield name, df
+    def _get_dfs(self, rows: List[Dict[str, Any]]) -> DataFrames:
+        tdfs: Dict[Any, DataFrame] = {}
+        for row in rows:
+            df = deserialize_df(row[_FUGUE_SERIALIZED_BLOB_COL])  # type: ignore
+            if df is not None:
+                if self.named:
+                    tdfs[row[_FUGUE_SERIALIZED_BLOB_NAME_COL]] = df
+                else:
+                    tdfs[row[_FUGUE_SERIALIZED_BLOB_NO_COL]] = df
+        dfs: Dict[Any, DataFrame] = {}
+        for k, schema in self.schemas.items():
+            if k in tdfs:
+                dfs[k] = tdfs[k]
             else:
-                yield df
+                dfs[k] = ArrayDataFrame([], schema)
+        return DataFrames(dfs) if self.named else DataFrames(list(dfs.values()))
 
 
 def _generate_comap_empty_dfs(schemas: Any, named: bool) -> DataFrames:
     if named:
         return DataFrames({k: ArrayDataFrame([], v) for k, v in schemas.items()})
     else:
         return DataFrames([ArrayDataFrame([], v) for v in schemas.values()])
```

### Comparing `fugue-0.8.6.dev3/fugue/execution/factory.py` & `fugue-0.8.7.dev1/fugue/execution/factory.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/execution/native_execution_engine.py` & `fugue-0.8.7.dev1/fugue/execution/native_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/__init__.py` & `fugue-0.8.7.dev1/fugue/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/_builtins/__init__.py` & `fugue-0.8.7.dev1/fugue/extensions/_builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/_builtins/creators.py` & `fugue-0.8.7.dev1/fugue/extensions/_builtins/creators.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/_builtins/outputters.py` & `fugue-0.8.7.dev1/fugue/extensions/_builtins/outputters.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 from triad.utils.convert import to_type
 
 from fugue.collections.partition import PartitionCursor
 from fugue.dataframe import DataFrame, DataFrames, LocalDataFrame
 from fugue.dataframe.array_dataframe import ArrayDataFrame
 from fugue.dataframe.utils import _df_eq
 from fugue.exceptions import FugueWorkflowError
-from fugue.execution.execution_engine import _generate_comap_empty_dfs
+from fugue.execution.execution_engine import (
+    _FUGUE_SERIALIZED_BLOB_SCHEMA,
+    _generate_comap_empty_dfs,
+)
 from fugue.rpc import EmptyRPCHandler, to_rpc_handler
 
 from ..outputter import Outputter
 from ..transformer.convert import _to_output_transformer
 from ..transformer.transformer import CoTransformer, Transformer
 
 
@@ -104,15 +107,15 @@
         self.execution_engine.persist(df, lazy=False)
 
     @no_type_check
     def cotransform(self, df: DataFrame, tf: CoTransformer) -> None:
         assert_or_throw(
             df.metadata.get("serialized", False), "must use serialized dataframe"
         )
-        tf._key_schema = df.schema - list(df.metadata["serialized_cols"].values())
+        tf._key_schema = df.schema - _FUGUE_SERIALIZED_BLOB_SCHEMA
         # TODO: currently, get_output_schema only gets empty dataframes
         empty_dfs = _generate_comap_empty_dfs(
             df.metadata["schemas"], df.metadata.get("serialized_has_name", False)
         )
         tf._output_schema = Schema(tf.get_output_schema(empty_dfs))
         tr = _CoTransformerRunner(df, tf, self._ignore_errors)
         df = self.execution_engine.comap(
```

### Comparing `fugue-0.8.6.dev3/fugue/extensions/_builtins/processors.py` & `fugue-0.8.7.dev1/fugue/extensions/_builtins/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, List, Type, no_type_check
 
+from triad.collections import ParamDict
+from triad.collections.schema import Schema
+from triad.utils.assertion import assert_or_throw
+from triad.utils.convert import to_type
+
 from fugue.collections.partition import PartitionCursor
-from fugue.dataframe import (
-    ArrayDataFrame,
-    DataFrame,
-    DataFrames,
-    LocalDataFrame,
-)
-from fugue.column import ColumnExpr, SelectColumns as ColumnsSelect
+from fugue.column import ColumnExpr
+from fugue.column import SelectColumns as ColumnsSelect
+from fugue.dataframe import ArrayDataFrame, DataFrame, DataFrames, LocalDataFrame
 from fugue.exceptions import FugueWorkflowError
 from fugue.execution import make_sql_engine
-from fugue.execution.execution_engine import _generate_comap_empty_dfs
+from fugue.execution.execution_engine import (
+    _FUGUE_SERIALIZED_BLOB_SCHEMA,
+    _generate_comap_empty_dfs,
+)
 from fugue.extensions.processor import Processor
 from fugue.extensions.transformer import CoTransformer, Transformer, _to_transformer
 from fugue.rpc import EmptyRPCHandler, to_rpc_handler
-from triad.collections import ParamDict
-from triad.collections.schema import Schema
-from triad.utils.assertion import assert_or_throw
-from triad.utils.convert import to_type
 
 
 class RunTransformer(Processor):
     @no_type_check
     def process(self, dfs: DataFrames) -> DataFrame:
         df = dfs[0]
         tf = _to_transformer(
@@ -56,15 +56,15 @@
         )
 
     @no_type_check
     def cotransform(self, df: DataFrame, tf: CoTransformer) -> DataFrame:
         assert_or_throw(
             df.metadata.get("serialized", False), "must use serialized dataframe"
         )
-        tf._key_schema = df.schema - list(df.metadata["serialized_cols"].values())
+        tf._key_schema = df.schema - _FUGUE_SERIALIZED_BLOB_SCHEMA
         # TODO: currently, get_output_schema only gets empty dataframes
         empty_dfs = _generate_comap_empty_dfs(
             df.metadata["schemas"], df.metadata.get("serialized_has_name", False)
         )
         tf._output_schema = Schema(tf.get_output_schema(empty_dfs))
         tr = _CoTransformerRunner(df, tf, self._ignore_errors)
         return self.execution_engine.comap(
@@ -157,15 +157,15 @@
 class Zip(Processor):
     def process(self, dfs: DataFrames) -> DataFrame:
         how = self.params.get("how", "inner")
         partition_spec = self.partition_spec
         # TODO: this should also search on workflow conf
         temp_path = self.params.get_or_none("temp_path", str)
         to_file_threshold = self.params.get_or_none("to_file_threshold", object)
-        return self.execution_engine.zip_all(
+        return self.execution_engine.zip(
             dfs,
             how=how,
             partition_spec=partition_spec,
             temp_path=temp_path,
             to_file_threshold=to_file_threshold,
         )
```

### Comparing `fugue-0.8.6.dev3/fugue/extensions/_utils.py` & `fugue-0.8.7.dev1/fugue/extensions/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/context.py` & `fugue-0.8.7.dev1/fugue/extensions/context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/creator/convert.py` & `fugue-0.8.7.dev1/fugue/extensions/creator/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/creator/creator.py` & `fugue-0.8.7.dev1/fugue/extensions/creator/creator.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/outputter/convert.py` & `fugue-0.8.7.dev1/fugue/extensions/outputter/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/outputter/outputter.py` & `fugue-0.8.7.dev1/fugue/extensions/outputter/outputter.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/processor/convert.py` & `fugue-0.8.7.dev1/fugue/extensions/processor/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/processor/processor.py` & `fugue-0.8.7.dev1/fugue/extensions/processor/processor.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/transformer/convert.py` & `fugue-0.8.7.dev1/fugue/extensions/transformer/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/extensions/transformer/transformer.py` & `fugue-0.8.7.dev1/fugue/extensions/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/plugins.py` & `fugue-0.8.7.dev1/fugue/plugins.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/registry.py` & `fugue-0.8.7.dev1/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/rpc/base.py` & `fugue-0.8.7.dev1/fugue/rpc/base.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/rpc/flask.py` & `fugue-0.8.7.dev1/fugue/rpc/flask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/sql/_utils.py` & `fugue-0.8.7.dev1/fugue/sql/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/sql/_visitors.py` & `fugue-0.8.7.dev1/fugue/sql/_visitors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/sql/api.py` & `fugue-0.8.7.dev1/fugue/sql/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/sql/workflow.py` & `fugue-0.8.7.dev1/fugue/sql/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/workflow/_checkpoint.py` & `fugue-0.8.7.dev1/fugue/workflow/_checkpoint.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/workflow/_tasks.py` & `fugue-0.8.7.dev1/fugue/workflow/_tasks.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/workflow/_workflow_context.py` & `fugue-0.8.7.dev1/fugue/workflow/_workflow_context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/workflow/api.py` & `fugue-0.8.7.dev1/fugue/workflow/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/workflow/module.py` & `fugue-0.8.7.dev1/fugue/workflow/module.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue/workflow/workflow.py` & `fugue-0.8.7.dev1/fugue/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue.egg-info/PKG-INFO` & `fugue-0.8.7.dev1/fugue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.6.dev3
+Version: 0.8.7.dev1
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
```

### Comparing `fugue-0.8.6.dev3/fugue.egg-info/SOURCES.txt` & `fugue-0.8.7.dev1/fugue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue.egg-info/requires.txt` & `fugue-0.8.7.dev1/fugue.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_contrib/seaborn/__init__.py` & `fugue-0.8.7.dev1/fugue_contrib/seaborn/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_contrib/viz/__init__.py` & `fugue-0.8.7.dev1/fugue_contrib/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_contrib/viz/_ext.py` & `fugue-0.8.7.dev1/fugue_contrib/viz/_ext.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_dask/_io.py` & `fugue-0.8.7.dev1/fugue_dask/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_dask/dataframe.py` & `fugue-0.8.7.dev1/fugue_dask/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_dask/execution_engine.py` & `fugue-0.8.7.dev1/fugue_dask/execution_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from distributed import Client
 from triad.collections import Schema
 from triad.collections.dict import IndexedOrderedDict, ParamDict
 from triad.collections.fs import FileSystem
 from triad.utils.assertion import assert_or_throw
 from triad.utils.hash import to_uuid
 from triad.utils.threading import RunOnce
-
+from triad.utils.pandas_like import PandasUtils
 from fugue import StructuredRawSQL
 from fugue._utils.misc import import_fsql_dependency
 from fugue.collections.partition import (
     PartitionCursor,
     PartitionSpec,
     parse_presort_exp,
 )
@@ -28,15 +28,21 @@
     PandasDataFrame,
 )
 from fugue.dataframe.utils import get_join_schemas
 from fugue.execution.execution_engine import ExecutionEngine, MapEngine, SQLEngine
 from fugue.execution.native_execution_engine import NativeExecutionEngine
 from fugue_dask._constants import FUGUE_DASK_DEFAULT_CONF
 from fugue_dask._io import load_df, save_df
-from fugue_dask._utils import DASK_UTILS, DaskUtils
+from fugue_dask._utils import (
+    DASK_UTILS,
+    DaskUtils,
+    even_repartition,
+    hash_repartition,
+    rand_repartition,
+)
 from fugue_dask.dataframe import DaskDataFrame
 
 _DASK_PARTITION_KEY = "__dask_partition_key__"
 
 
 class QPDDaskEngine(SQLEngine):
     """QPD execution implementation."""
@@ -75,79 +81,72 @@
         df: DataFrame,
         map_func: Callable[[PartitionCursor, LocalDataFrame], LocalDataFrame],
         output_schema: Any,
         partition_spec: PartitionSpec,
         on_init: Optional[Callable[[int, DataFrame], Any]] = None,
         map_func_format_hint: Optional[str] = None,
     ) -> DataFrame:
-        is_coarse = partition_spec.algo == "coarse"
-        presort = partition_spec.get_sorts(df.schema, with_partition_keys=is_coarse)
+        presort = partition_spec.get_sorts(
+            df.schema, with_partition_keys=partition_spec.algo == "coarse"
+        )
         presort_keys = list(presort.keys())
         presort_asc = list(presort.values())
         output_schema = Schema(output_schema)
         input_schema = df.schema
         cursor = partition_spec.get_cursor(input_schema, 0)
         on_init_once: Any = (
             None
             if on_init is None
             else RunOnce(
                 on_init, lambda *args, **kwargs: to_uuid(id(on_init), id(args[0]))
             )
         )
 
-        def _map(pdf: Any) -> pd.DataFrame:
+        def _map(pdf: pd.DataFrame) -> pd.DataFrame:
             if pdf.shape[0] == 0:
                 return PandasDataFrame([], output_schema).as_pandas()
-            if is_coarse:
-                pdf = pdf.drop(columns=[_DASK_PARTITION_KEY])
             if len(partition_spec.presort) > 0:
                 pdf = pdf.sort_values(presort_keys, ascending=presort_asc)
             input_df = PandasDataFrame(
                 pdf.reset_index(drop=True), input_schema, pandas_df_wrapper=True
             )
             if on_init_once is not None:
                 on_init_once(0, input_df)
             cursor.set(lambda: input_df.peek_array(), 0, 0)
             output_df = map_func(cursor, input_df)
             return output_df.as_pandas()[output_schema.names]
 
+        def _gp_map(pdf: pd.DataFrame) -> pd.DataFrame:
+            if pdf.shape[0] == 0:  # pragma: no cover
+                return PandasDataFrame([], output_schema).as_pandas()
+            pu = PandasUtils()
+            return pu.safe_groupby_apply(
+                pdf.reset_index(drop=True), partition_spec.partition_by, _map
+            )
+
         df = self.to_df(df)
         meta = self.execution_engine.pl_utils.safe_to_pandas_dtype(  # type: ignore
             output_schema.pa_schema
         )
+        pdf = self.execution_engine.repartition(df, partition_spec)
         if len(partition_spec.partition_by) == 0:
-            pdf = self.execution_engine.repartition(df, partition_spec)
             result = pdf.native.map_partitions(_map, meta=meta)  # type: ignore
         else:
-            df = self.execution_engine.repartition(
-                df, PartitionSpec(num=partition_spec.num_partitions)
-            )
-            if is_coarse:
-                input_num_partitions = df.num_partitions
-                _utils = self.execution_engine.pl_utils  # type: ignore
-                input_meta = _utils.safe_to_pandas_dtype(
-                    (input_schema + (_DASK_PARTITION_KEY, "uint64")).pa_schema
-                )
-                tddf = df.native.map_partitions(
-                    lambda pdf: pdf.assign(
-                        **{
-                            _DASK_PARTITION_KEY: pd.util.hash_pandas_object(
-                                pdf[partition_spec.partition_by], index=False
-                            ).mod(input_num_partitions)
-                        }
-                    ),
-                    meta=input_meta,
+            if partition_spec.algo == "default":
+                engine = self.execution_engine
+                result = engine.pl_utils.safe_groupby_apply(  # type: ignore
+                    df.native,
+                    partition_spec.partition_by,
+                    _map,
+                    meta=meta,
                 )
-                keys = [_DASK_PARTITION_KEY]
+            elif partition_spec.algo == "coarse":
+                result = pdf.native.map_partitions(_map, meta=meta)  # type: ignore
             else:
-                tddf = df.native
-                keys = partition_spec.partition_by
-            result = self.execution_engine.pl_utils.safe_groupby_apply(  # type: ignore
-                tddf, keys, _map, meta=meta  # type: ignore
-            )
+                result = pdf.native.map_partitions(_gp_map, meta=meta)  # type: ignore
         return DaskDataFrame(result, output_schema)
 
 
 class DaskExecutionEngine(ExecutionEngine):
     """The execution engine based on `Dask <https://docs.dask.org/>`_.
 
     Please read |ExecutionEngineTutorial| to understand this important Fugue concept
@@ -233,30 +232,48 @@
 
     def repartition(
         self, df: DataFrame, partition_spec: PartitionSpec
     ) -> DaskDataFrame:
         df = self.to_df(df)
         if partition_spec.empty:
             return df
-        if len(partition_spec.partition_by) > 0:
+        if len(partition_spec.partition_by) > 0 and partition_spec.algo == "default":
             return df
         p = partition_spec.get_num_partitions(
             **{
                 KEYWORD_ROWCOUNT: lambda: df.persist().count(),  # type: ignore
                 KEYWORD_PARALLELISM: lambda: self.get_current_parallelism(),
             }
         )
-        if p > 0:
-            if partition_spec.algo == "even":
-                pdf = df.as_pandas()
-                ddf = dd.from_pandas(pdf, npartitions=p, sort=False)
-            else:
-                ddf = df.native.repartition(npartitions=p)
-            return DaskDataFrame(ddf, schema=df.schema, type_safe=False)
-        return df
+        if partition_spec.algo == "default":
+            ddf: dd.DataFrame = (
+                df.native.repartition(npartitions=p) if p > 0 else df.native
+            )
+        elif partition_spec.algo in ["hash", "coarse"]:
+            ddf = hash_repartition(
+                df.native,
+                num=p if p > 0 else self.get_current_parallelism() * 2,
+                cols=partition_spec.partition_by,
+            )
+        elif partition_spec.algo == "even":
+            ddf = even_repartition(df.native, num=p, cols=partition_spec.partition_by)
+        elif partition_spec.algo == "rand":
+            ddf = rand_repartition(
+                df.native,
+                num=p if p > 0 else self.get_current_parallelism() * 2,
+                cols=partition_spec.partition_by,
+                seed=0,
+            )
+        else:  # pragma: no cover
+            raise NotImplementedError(
+                partition_spec.algo + " partitioning is not supported"
+            )
+        if ddf is None or df.native is ddf:
+            return df
+        return DaskDataFrame(ddf, schema=df.schema, type_safe=False)
 
     def broadcast(self, df: DataFrame) -> DataFrame:
         return self.to_df(df)
 
     def persist(
         self,
         df: DataFrame,
```

### Comparing `fugue-0.8.6.dev3/fugue_dask/ibis_engine.py` & `fugue-0.8.7.dev1/fugue_dask/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_dask/registry.py` & `fugue-0.8.7.dev1/fugue_dask/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_duckdb/_io.py` & `fugue-0.8.7.dev1/fugue_duckdb/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_duckdb/_utils.py` & `fugue-0.8.7.dev1/fugue_duckdb/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_duckdb/dask.py` & `fugue-0.8.7.dev1/fugue_duckdb/dask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_duckdb/dataframe.py` & `fugue-0.8.7.dev1/fugue_duckdb/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_duckdb/execution_engine.py` & `fugue-0.8.7.dev1/fugue_duckdb/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_duckdb/ibis_engine.py` & `fugue-0.8.7.dev1/fugue_duckdb/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_duckdb/registry.py` & `fugue-0.8.7.dev1/fugue_duckdb/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ibis/_utils.py` & `fugue-0.8.7.dev1/fugue_ibis/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ibis/dataframe.py` & `fugue-0.8.7.dev1/fugue_ibis/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ibis/execution/ibis_engine.py` & `fugue-0.8.7.dev1/fugue_ibis/execution/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ibis/execution/pandas_backend.py` & `fugue-0.8.7.dev1/fugue_ibis/execution/pandas_backend.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ibis/execution_engine.py` & `fugue-0.8.7.dev1/fugue_ibis/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ibis/extensions.py` & `fugue-0.8.7.dev1/fugue_ibis/extensions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_notebook/__init__.py` & `fugue-0.8.7.dev1/fugue_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_notebook/env.py` & `fugue-0.8.7.dev1/fugue_notebook/env.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_notebook/nbextension/main.js` & `fugue-0.8.7.dev1/fugue_notebook/nbextension/main.js`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_polars/polars_dataframe.py` & `fugue-0.8.7.dev1/fugue_polars/polars_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_polars/registry.py` & `fugue-0.8.7.dev1/fugue_polars/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ray/_constants.py` & `fugue-0.8.7.dev1/fugue_ray/_constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ray/_utils/cluster.py` & `fugue-0.8.7.dev1/fugue_ray/_utils/cluster.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ray/_utils/dataframe.py` & `fugue-0.8.7.dev1/fugue_ray/_utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ray/_utils/io.py` & `fugue-0.8.7.dev1/fugue_ray/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ray/dataframe.py` & `fugue-0.8.7.dev1/fugue_ray/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_ray/execution_engine.py` & `fugue-0.8.7.dev1/fugue_ray/execution_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             KEYWORD_ROWCOUNT: lambda: _persist_and_count(rdf),
             KEYWORD_PARALLELISM: lambda: self.get_current_parallelism(),
         }
         num = partition_spec.get_num_partitions(**num_funcs)
         pdf = rdf.native
 
         if num > 0:
-            if partition_spec.algo in ["hash", "even", "coarse"]:
+            if partition_spec.algo in ["default", "hash", "even", "coarse"]:
                 pdf = pdf.repartition(num)
             elif partition_spec.algo == "rand":
                 pdf = pdf.repartition(num, shuffle=True)
             else:  # pragma: no cover
                 raise NotImplementedError(partition_spec.algo + " is not supported")
         return RayDataFrame(pdf, schema=rdf.schema, internal_schema=True)
```

### Comparing `fugue-0.8.6.dev3/fugue_ray/registry.py` & `fugue-0.8.7.dev1/fugue_ray/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_spark/_utils/convert.py` & `fugue-0.8.7.dev1/fugue_spark/_utils/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_spark/_utils/io.py` & `fugue-0.8.7.dev1/fugue_spark/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_spark/_utils/misc.py` & `fugue-0.8.7.dev1/fugue_spark/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_spark/_utils/partition.py` & `fugue-0.8.7.dev1/fugue_spark/_utils/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_spark/dataframe.py` & `fugue-0.8.7.dev1/fugue_spark/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_spark/execution_engine.py` & `fugue-0.8.7.dev1/fugue_spark/execution_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                         output_schema=output_schema,
                         partition_spec=partition_spec,
                         on_init=on_init,
                         map_func_format_hint=map_func_format_hint,
                     )
                 else:
                     if (  # not simple partitioning
-                        partition_spec.algo != "hash"
+                        partition_spec.algo not in ["default", "hash"]
                         or partition_spec.num_partitions != "0"
                     ):
                         # TODO: not sure if presort should be done
                         # on physical partition level
                         df = self.to_df(
                             self.execution_engine.repartition(
                                 df, PartitionSpec(partition_spec, presort=[])
@@ -436,15 +436,15 @@
         df = self._to_spark_df(df)
         num_funcs = {
             KEYWORD_ROWCOUNT: lambda: _persist_and_count(df),
             KEYWORD_PARALLELISM: lambda: self.get_current_parallelism(),
         }
         num = partition_spec.get_num_partitions(**num_funcs)
 
-        if partition_spec.algo in ["hash", "coarse"]:
+        if partition_spec.algo in ["default", "hash", "coarse"]:
             sdf = hash_repartition(
                 self.spark_session, df.native, num, partition_spec.partition_by
             )
         elif partition_spec.algo == "rand":
             sdf = rand_repartition(
                 self.spark_session, df.native, num, partition_spec.partition_by
             )
```

### Comparing `fugue-0.8.6.dev3/fugue_spark/ibis_engine.py` & `fugue-0.8.7.dev1/fugue_spark/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_spark/registry.py` & `fugue-0.8.7.dev1/fugue_spark/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_test/bag_suite.py` & `fugue-0.8.7.dev1/fugue_test/bag_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_test/builtin_suite.py` & `fugue-0.8.7.dev1/fugue_test/builtin_suite.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,16 +389,16 @@
                     a, b, how="left_outer", partition=dict(presort="b DESC, c ASC")
                 )
                 c1.assert_eq(c2)
 
                 a = dag.df([[1, 2, 0], [1, 3, 1]], "a:int,b:int,c:int")
                 b = dag.df([[1, 2, 1], [1, 3, 2]], "a:int,b:int,d:int")
                 c = dag.df([[1, 4]], "a:int,e:int")
-                e = dag.df([[1, 2], [1, 3]], "a:int,b:int")
-                dag.zip(a, b, c)[["a", "b"]].assert_eq(e)
+                e = dag.df([[1]], "a:int")
+                dag.zip(a, b, c)[["a"]].distinct().assert_eq(e)
             dag.run(self.engine)
 
         def test_transform(self):
             with FugueWorkflow() as dag:
                 a = dag.df([[1, 2], [3, 4]], "a:double,b:int")
                 c = a.transform(mock_tf0)
                 dag.df([[1, 2, 1], [3, 4, 1]], "a:double,b:int,p:int").assert_eq(c)
```

### Comparing `fugue-0.8.6.dev3/fugue_test/dataframe_suite.py` & `fugue-0.8.7.dev1/fugue_test/dataframe_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/fugue_test/execution_suite.py` & `fugue-0.8.7.dev1/fugue_test/execution_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -822,29 +822,29 @@
             d2 = fa.sample(a, n=90, seed=1)
             e = fa.sample(a, n=90, seed=2)
             assert not df_eq(b, c, throw=False)
             df_eq(d, d2, throw=True)
             assert not df_eq(d, e, throw=False)
             assert abs(len(e.as_array()) - 90) < 2
 
-        def test__serialize_by_partition(self):
+        def _test__serialize_by_partition(self):
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[1, 2], [3, 4], [1, 5]], "a:int,b:int")
             s = e._serialize_by_partition(
                 a, PartitionSpec(by=["a"], presort="b"), df_name="_0"
             )
             assert s.count() == 2
             s = fa.persist(e._serialize_by_partition(a, PartitionSpec(), df_name="_0"))
             assert s.count() == 1
             s = fa.persist(
                 e._serialize_by_partition(a, PartitionSpec(by=["x"]), df_name="_0")
             )
             assert s.count() == 1
 
-        def test_zip(self):
+        def _test_zip(self):
             ps = PartitionSpec(by=["a"], presort="b DESC,c DESC")
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[1, 2], [3, 4], [1, 5]], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [[6, 1], [2, 7]], "c:int,a:int")
             sa = e._serialize_by_partition(a, ps, df_name="_0")
             sb = e._serialize_by_partition(b, ps, df_name="_1")
             # test zip with serialized dfs
@@ -897,73 +897,94 @@
             assert z6.count() == 2
             assert len(z6.schema) == 3
 
             z7 = e.zip(a, b, df1_name="x", df2_name="y")
             z7.show()
             assert z7.metadata.get("serialized_has_name", False)
 
-        def test_zip_all(self):
+        def _test_zip_all(self):
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[1, 2], [3, 4], [1, 5]], "a:int,b:int")
-            z = fa.persist(e.zip_all(DataFrames(a)))
+            z = fa.persist(e.zip(DataFrames(a)))
             assert 1 == z.count()
             assert z.metadata.get("serialized", False)
             assert not z.metadata.get("serialized_has_name", False)
-            z = fa.persist(e.zip_all(DataFrames(x=a)))
+            z = fa.persist(e.zip(DataFrames(x=a)))
             assert 1 == z.count()
             assert z.metadata.get("serialized", False)
             assert z.metadata.get("serialized_has_name", False)
             z = fa.persist(
-                e.zip_all(DataFrames(x=a), partition_spec=PartitionSpec(by=["a"]))
+                e.zip(DataFrames(x=a), partition_spec=PartitionSpec(by=["a"]))
             )
             assert 2 == z.count()
             assert z.metadata.get("serialized", False)
             assert z.metadata.get("serialized_has_name", False)
 
             b = fa.as_fugue_engine_df(e, [[6, 1], [2, 7]], "c:int,a:int")
             c = fa.as_fugue_engine_df(e, [[6, 1], [2, 7]], "d:int,a:int")
-            z = fa.persist(e.zip_all(DataFrames(a, b, c)))
+            z = fa.persist(e.zip(DataFrames(a, b, c)))
             assert 1 == z.count()
             assert not z.metadata.get("serialized_has_name", False)
-            z = fa.persist(e.zip_all(DataFrames(x=a, y=b, z=c)))
+            z = fa.persist(e.zip(DataFrames(x=a, y=b, z=c)))
             assert 1 == z.count()
             assert z.metadata.get("serialized_has_name", False)
 
-            z = fa.persist(e.zip_all(DataFrames(b, b)))
+            z = fa.persist(e.zip(DataFrames(b, b)))
             assert 2 == z.count()
             assert not z.metadata.get("serialized_has_name", False)
             assert ["a", "c"] in z.schema
-            z = fa.persist(e.zip_all(DataFrames(x=b, y=b)))
+            z = fa.persist(e.zip(DataFrames(x=b, y=b)))
             assert 2 == z.count()
             assert z.metadata.get("serialized_has_name", False)
             assert ["a", "c"] in z.schema
 
             z = fa.persist(
-                e.zip_all(DataFrames(b, b), partition_spec=PartitionSpec(by=["a"]))
+                e.zip(DataFrames(b, b), partition_spec=PartitionSpec(by=["a"]))
             )
             assert 2 == z.count()
             assert not z.metadata.get("serialized_has_name", False)
             assert "c" not in z.schema
 
         def test_comap(self):
             ps = PartitionSpec(presort="b,c")
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[1, 2], [3, 4], [1, 5]], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [[6, 1], [2, 7]], "c:int,a:int")
-            z1 = fa.persist(e.zip(a, b))
-            z2 = fa.persist(e.zip(a, b, partition_spec=ps, how="left_outer"))
+            with raises(InvalidOperationError):  # cross can't have partition by
+                e.zip(
+                    DataFrames([a, b]),
+                    partition_spec=PartitionSpec(by=["a"]),
+                    how="cross",
+                )
+            with raises(NotImplementedError):
+                e.zip(
+                    DataFrames([a, b]),
+                    partition_spec=PartitionSpec(by=["a"]),
+                    how="left_anti",
+                )
+            z1 = fa.persist(e.zip(DataFrames([a, b])))
+            z2 = fa.persist(
+                e.zip(DataFrames([a, b]), partition_spec=ps, how="left_outer")
+            )
             z3 = fa.persist(
-                e._serialize_by_partition(a, partition_spec=ps, df_name="_x")
+                e.zip(DataFrames([b, a]), partition_spec=ps, how="right_outer")
+            )
+            z4 = fa.persist(e.zip(DataFrames([a, b]), partition_spec=ps, how="cross"))
+            z5 = fa.persist(
+                e.zip(DataFrames([a, b]), partition_spec=ps, how="full_outer")
             )
-            z4 = fa.persist(e.zip(a, b, partition_spec=ps, how="cross"))
 
             def comap(cursor, dfs):
                 assert not dfs.has_key
                 v = ",".join([k + str(v.count()) for k, v in dfs.items()])
-                keys = cursor.key_value_array
+                keys = (
+                    cursor.key_value_array
+                    if not dfs[0].empty
+                    else dfs[1][["a"]].peek_array()
+                )
                 if len(keys) == 0:
                     return ArrayDataFrame([[v]], "v:str")
                 return ArrayDataFrame([keys + [v]], cursor.key_schema + "v:str")
 
             def on_init(partition_no, dfs):
                 assert not dfs.has_key
                 assert partition_no >= 0
@@ -983,29 +1004,42 @@
             df_eq(
                 res,
                 [[1, "_02,_11"], [3, "_01,_10"]],
                 "a:int,v:str",
                 throw=True,
             )
 
-            res = e.comap(z3, comap, "v:str", PartitionSpec())
-            df_eq(res, [["_03"]], "v:str", throw=True)
+            res = e.comap(z3, comap, "a:int,v:str", PartitionSpec())
+            df_eq(
+                res,
+                [[1, "_01,_12"], [3, "_00,_11"]],
+                "a:int,v:str",
+                throw=True,
+            )
 
             res = e.comap(z4, comap, "v:str", PartitionSpec())
             df_eq(res, [["_03,_12"]], "v:str", throw=True)
 
+            res = e.comap(z5, comap, "a:int,v:str", PartitionSpec())
+            df_eq(
+                res,
+                [[1, "_02,_11"], [3, "_01,_10"], [7, "_00,_11"]],
+                "a:int,v:str",
+                throw=True,
+            )
+
         def test_comap_with_key(self):
             e = self.engine
             a = fa.as_fugue_engine_df(e, [[1, 2], [3, 4], [1, 5]], "a:int,b:int")
             b = fa.as_fugue_engine_df(e, [[6, 1], [2, 7]], "c:int,a:int")
             c = fa.as_fugue_engine_df(e, [[6, 1]], "c:int,a:int")
-            z1 = fa.persist(e.zip(a, b, df1_name="x", df2_name="y"))
-            z2 = fa.persist(e.zip_all(DataFrames(x=a, y=b, z=b)))
+            z1 = fa.persist(e.zip(DataFrames(x=a, y=b)))
+            z2 = fa.persist(e.zip(DataFrames(x=a, y=b, z=b)))
             z3 = fa.persist(
-                e.zip_all(DataFrames(z=c), partition_spec=PartitionSpec(by=["a"]))
+                e.zip(DataFrames(z=c), partition_spec=PartitionSpec(by=["a"]))
             )
 
             def comap(cursor, dfs):
                 assert dfs.has_key
                 v = ",".join([k + str(v.count()) for k, v in dfs.items()])
                 keys = cursor.key_value_array
                 # if len(keys) == 0:
```

### Comparing `fugue-0.8.6.dev3/fugue_test/ibis_suite.py` & `fugue-0.8.7.dev1/fugue_test/ibis_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/setup.cfg` & `fugue-0.8.7.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fugue-0.8.6.dev3/setup.py` & `fugue-0.8.7.dev1/setup.py`

 * *Files identical despite different names*

