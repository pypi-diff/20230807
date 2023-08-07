# Comparing `tmp/quartic-sdk-2.8.0.tar.gz` & `tmp/quartic-sdk-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartic-sdk-2.8.0.tar", last modified: Tue May 10 05:18:38 2022, max compression
+gzip compressed data, was "quartic-sdk-2.9.0.tar", last modified: Mon Jun 20 07:49:29 2022, max compression
```

## Comparing `quartic-sdk-2.8.0.tar` & `quartic-sdk-2.9.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.118954 quartic-sdk-2.8.0/
--rw-rw-r--   0 root         (0) root         (0)     1049 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4277 2022-05-10 05:18:38.118954 quartic-sdk-2.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3622 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.114953 quartic-sdk-2.8.0/examples/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.114953 quartic-sdk-2.8.0/quartic_sdk/
--rw-rw-r--   0 root         (0) root         (0)       98 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       73 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.114953 quartic-sdk-2.8.0/quartic_sdk/api/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/api/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5053 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/api/api_helper.py
--rw-rw-r--   0 root         (0) root         (0)     5915 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.114953 quartic-sdk-2.8.0/quartic_sdk/core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.114953 quartic-sdk-2.8.0/quartic_sdk/core/entities/
--rw-rw-r--   0 root         (0) root         (0)      785 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5458 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/asset.py
--rw-rw-r--   0 root         (0) root         (0)     1575 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/base.py
--rw-rw-r--   0 root         (0) root         (0)      493 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/batch.py
--rw-rw-r--   0 root         (0) root         (0)     1119 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/context_frame.py
--rw-rw-r--   0 root         (0) root         (0)      586 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/context_frame_occurrence.py
--rw-rw-r--   0 root         (0) root         (0)     4914 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/edge_connector.py
--rw-rw-r--   0 root         (0) root         (0)     1497 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/event_frame.py
--rw-rw-r--   0 root         (0) root         (0)      662 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/event_frame_occurrence.py
--rw-rw-r--   0 root         (0) root         (0)     1531 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/model.py
--rw-rw-r--   0 root         (0) root         (0)     3247 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/procedure.py
--rw-rw-r--   0 root         (0) root         (0)     3274 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/procedure_step.py
--rw-rw-r--   0 root         (0) root         (0)     3093 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/product.py
--rw-rw-r--   0 root         (0) root         (0)      742 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/site.py
--rw-rw-r--   0 root         (0) root         (0)     6705 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/tag.py
--rw-rw-r--   0 root         (0) root         (0)      706 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entities/type_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.114953 quartic-sdk-2.8.0/quartic_sdk/core/entity_helpers/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entity_helpers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1869 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entity_helpers/entity_factory.py
--rw-rw-r--   0 root         (0) root         (0)     7463 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/entity_helpers/entity_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.114953 quartic-sdk-2.8.0/quartic_sdk/core/iterators/
--rw-rw-r--   0 root         (0) root         (0)      152 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/iterators/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      718 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/iterators/entity_list_iterator.py
--rw-rw-r--   0 root         (0) root         (0)     3432 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/iterators/historical_tag_data_iterator.py
--rw-rw-r--   0 root         (0) root         (0)    10484 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/core/iterators/tag_data_iterator.py
--rw-rw-r--   0 root         (0) root         (0)      182 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     6136 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.114953 quartic-sdk-2.8.0/quartic_sdk/model/
--rw-rw-r--   0 root         (0) root         (0)     7482 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/model/BaseQuarticModel.py
--rw-rw-r--   0 root         (0) root         (0)     5953 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/model/BaseSpectralModel.py
--rw-rw-r--   0 root         (0) root         (0)      130 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/model/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4656 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/model/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.114953 quartic-sdk-2.8.0/quartic_sdk/model/tests/
--rw-rw-r--   0 root         (0) root         (0)     6054 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/model/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5266 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/model/tests/test_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.118954 quartic-sdk-2.8.0/quartic_sdk/utilities/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2150 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/utilities/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     4366 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/utilities/constants.py
--rw-rw-r--   0 root         (0) root         (0)      452 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/utilities/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     5806 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/utilities/test_helpers.py
--rw-rw-r--   0 root         (0) root         (0)     2340 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/quartic_sdk/utilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-10 05:18:38.114953 quartic-sdk-2.8.0/quartic_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4277 2022-05-10 05:18:38.000000 quartic-sdk-2.8.0/quartic_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1851 2022-05-10 05:18:38.000000 quartic-sdk-2.8.0/quartic_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-10 05:18:38.000000 quartic-sdk-2.8.0/quartic_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     4775 2022-05-10 05:18:38.000000 quartic-sdk-2.8.0/quartic_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-10 05:18:38.000000 quartic-sdk-2.8.0/quartic_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       66 2022-05-10 05:18:38.118954 quartic-sdk-2.8.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1733 2022-05-10 05:14:01.000000 quartic-sdk-2.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.375800 quartic-sdk-2.9.0/
+-rw-rw-r--   0 root         (0) root         (0)     1049 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4277 2022-06-20 07:49:29.375800 quartic-sdk-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3622 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.371799 quartic-sdk-2.9.0/examples/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.371799 quartic-sdk-2.9.0/quartic_sdk/
+-rw-rw-r--   0 root         (0) root         (0)       98 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       73 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.371799 quartic-sdk-2.9.0/quartic_sdk/api/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/api/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5053 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/api/api_helper.py
+-rw-rw-r--   0 root         (0) root         (0)     5915 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.371799 quartic-sdk-2.9.0/quartic_sdk/core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.375800 quartic-sdk-2.9.0/quartic_sdk/core/entities/
+-rw-rw-r--   0 root         (0) root         (0)      785 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5458 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/asset.py
+-rw-rw-r--   0 root         (0) root         (0)     1575 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/base.py
+-rw-rw-r--   0 root         (0) root         (0)      493 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/batch.py
+-rw-rw-r--   0 root         (0) root         (0)     1119 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/context_frame.py
+-rw-rw-r--   0 root         (0) root         (0)      586 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/context_frame_occurrence.py
+-rw-rw-r--   0 root         (0) root         (0)     4914 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/edge_connector.py
+-rw-rw-r--   0 root         (0) root         (0)     1497 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/event_frame.py
+-rw-rw-r--   0 root         (0) root         (0)      662 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/event_frame_occurrence.py
+-rw-rw-r--   0 root         (0) root         (0)     1531 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/model.py
+-rw-rw-r--   0 root         (0) root         (0)     3247 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/procedure.py
+-rw-rw-r--   0 root         (0) root         (0)     3274 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/procedure_step.py
+-rw-rw-r--   0 root         (0) root         (0)     3093 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/product.py
+-rw-rw-r--   0 root         (0) root         (0)      742 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/site.py
+-rw-rw-r--   0 root         (0) root         (0)     6705 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/tag.py
+-rw-rw-r--   0 root         (0) root         (0)      706 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entities/type_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.375800 quartic-sdk-2.9.0/quartic_sdk/core/entity_helpers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entity_helpers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1869 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entity_helpers/entity_factory.py
+-rw-rw-r--   0 root         (0) root         (0)     7463 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/entity_helpers/entity_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.375800 quartic-sdk-2.9.0/quartic_sdk/core/iterators/
+-rw-rw-r--   0 root         (0) root         (0)      152 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/iterators/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      718 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/iterators/entity_list_iterator.py
+-rw-rw-r--   0 root         (0) root         (0)     3432 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/iterators/historical_tag_data_iterator.py
+-rw-rw-r--   0 root         (0) root         (0)    10484 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/core/iterators/tag_data_iterator.py
+-rw-rw-r--   0 root         (0) root         (0)      182 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     6136 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.375800 quartic-sdk-2.9.0/quartic_sdk/model/
+-rw-rw-r--   0 root         (0) root         (0)     7482 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/model/BaseQuarticModel.py
+-rw-rw-r--   0 root         (0) root         (0)     5953 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/model/BaseSpectralModel.py
+-rw-rw-r--   0 root         (0) root         (0)      130 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/model/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4656 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/model/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.375800 quartic-sdk-2.9.0/quartic_sdk/model/tests/
+-rw-rw-r--   0 root         (0) root         (0)     6054 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/model/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5266 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/model/tests/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.375800 quartic-sdk-2.9.0/quartic_sdk/utilities/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2150 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/utilities/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     4366 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/utilities/constants.py
+-rw-rw-r--   0 root         (0) root         (0)      452 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/utilities/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     5806 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/utilities/test_helpers.py
+-rw-rw-r--   0 root         (0) root         (0)     2340 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/quartic_sdk/utilities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-20 07:49:29.371799 quartic-sdk-2.9.0/quartic_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4277 2022-06-20 07:49:29.000000 quartic-sdk-2.9.0/quartic_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1851 2022-06-20 07:49:29.000000 quartic-sdk-2.9.0/quartic_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-20 07:49:29.000000 quartic-sdk-2.9.0/quartic_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     4775 2022-06-20 07:49:29.000000 quartic-sdk-2.9.0/quartic_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2022-06-20 07:49:29.000000 quartic-sdk-2.9.0/quartic_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2022-06-20 07:49:29.375800 quartic-sdk-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1733 2022-06-20 07:44:32.000000 quartic-sdk-2.9.0/setup.py
```

### Comparing `quartic-sdk-2.8.0/LICENSE` & `quartic-sdk-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/PKG-INFO` & `quartic-sdk-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartic-sdk
-Version: 2.8.0
+Version: 2.9.0
 Summary: QuarticSDK is the SDK package which exposes the APIs to the user
 Home-page: https://github.com/Quarticai/QuarticSDK/
 Author: Quartic.ai engineering team
 Author-email: tech@quartic.ai
 License: MIT
 Keywords: Quartic,QuarticSDK
 Platform: UNKNOWN
```

### Comparing `quartic-sdk-2.8.0/README.md` & `quartic-sdk-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/api/api_helper.py` & `quartic-sdk-2.9.0/quartic_sdk/api/api_helper.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/api_client.py` & `quartic-sdk-2.9.0/quartic_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/__init__.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/asset.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/asset.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/base.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/base.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/context_frame.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/context_frame.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/context_frame_occurrence.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/context_frame_occurrence.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/edge_connector.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/edge_connector.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/event_frame.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/event_frame.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/event_frame_occurrence.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/event_frame_occurrence.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/model.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/model.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/procedure.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/procedure.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/procedure_step.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/procedure_step.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/product.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/product.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/site.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/site.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/tag.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/tag.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entities/type_mapping.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entities/type_mapping.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entity_helpers/entity_factory.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entity_helpers/entity_factory.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/entity_helpers/entity_list.py` & `quartic-sdk-2.9.0/quartic_sdk/core/entity_helpers/entity_list.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/iterators/entity_list_iterator.py` & `quartic-sdk-2.9.0/quartic_sdk/core/iterators/entity_list_iterator.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/iterators/historical_tag_data_iterator.py` & `quartic-sdk-2.9.0/quartic_sdk/core/iterators/historical_tag_data_iterator.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/core/iterators/tag_data_iterator.py` & `quartic-sdk-2.9.0/quartic_sdk/core/iterators/tag_data_iterator.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/graphql_client.py` & `quartic-sdk-2.9.0/quartic_sdk/graphql_client.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/model/BaseQuarticModel.py` & `quartic-sdk-2.9.0/quartic_sdk/model/BaseQuarticModel.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/model/BaseSpectralModel.py` & `quartic-sdk-2.9.0/quartic_sdk/model/BaseSpectralModel.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/model/helpers.py` & `quartic-sdk-2.9.0/quartic_sdk/model/helpers.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/model/tests/__init__.py` & `quartic-sdk-2.9.0/quartic_sdk/model/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/model/tests/test_helpers.py` & `quartic-sdk-2.9.0/quartic_sdk/model/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/utilities/configuration.py` & `quartic-sdk-2.9.0/quartic_sdk/utilities/configuration.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/utilities/constants.py` & `quartic-sdk-2.9.0/quartic_sdk/utilities/constants.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/utilities/test_helpers.py` & `quartic-sdk-2.9.0/quartic_sdk/utilities/test_helpers.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk/utilities/utils.py` & `quartic-sdk-2.9.0/quartic_sdk/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk.egg-info/PKG-INFO` & `quartic-sdk-2.9.0/quartic_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartic-sdk
-Version: 2.8.0
+Version: 2.9.0
 Summary: QuarticSDK is the SDK package which exposes the APIs to the user
 Home-page: https://github.com/Quarticai/QuarticSDK/
 Author: Quartic.ai engineering team
 Author-email: tech@quartic.ai
 License: MIT
 Keywords: Quartic,QuarticSDK
 Platform: UNKNOWN
```

### Comparing `quartic-sdk-2.8.0/quartic_sdk.egg-info/SOURCES.txt` & `quartic-sdk-2.9.0/quartic_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quartic-sdk-2.8.0/quartic_sdk.egg-info/requires.txt` & `quartic-sdk-2.9.0/quartic_sdk.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 frozenlist==1.3.0
 future==0.18.2
 gast==0.4.0
 gherkin-official==4.1.3
 google-auth==2.6.6
 google-auth-oauthlib==0.4.6
 google-pasta==0.2.0
-grpcio==1.46.0
+grpcio==1.46.1
 h2o==3.32.0.4
 h5py==3.6.0
 humanfriendly==10.0
 idna==2.10
 imagesize==1.3.0
 importlib-metadata==4.11.3
 iniconfig==1.1.1
```

### Comparing `quartic-sdk-2.8.0/setup.py` & `quartic-sdk-2.9.0/setup.py`

 * *Files identical despite different names*

