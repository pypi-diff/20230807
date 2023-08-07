# Comparing `tmp/featurebyte-0.4.1.tar.gz` & `tmp/featurebyte-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurebyte-0.4.1.tar", max compression
+gzip compressed data, was "featurebyte-0.4.2.tar", max compression
```

## Comparing `featurebyte-0.4.1.tar` & `featurebyte-0.4.2.tar`

### file list

```diff
@@ -1,613 +1,619 @@
--rw-r--r--   0        0        0     3860 2023-07-25 05:44:21.013563 featurebyte-0.4.1/LICENSE
--rw-r--r--   0        0        0    19816 2023-07-25 05:44:21.013563 featurebyte-0.4.1/README.md
--rw-r--r--   0        0        0    17168 2023-07-25 05:44:21.013563 featurebyte-0.4.1/featurebyte/__init__.py
--rw-r--r--   0        0        0     2552 2023-07-25 05:44:21.013563 featurebyte-0.4.1/featurebyte/__main__.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/aggregator/__init__.py
--rw-r--r--   0        0        0     6216 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/aggregator/base_aggregator.py
--rw-r--r--   0        0        0     5063 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/aggregator/forward_aggregator.py
--rw-r--r--   0        0        0     5348 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/api_handler/base.py
--rw-r--r--   0        0        0      497 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/api_handler/catalog.py
--rw-r--r--   0        0        0      531 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/api_handler/feature.py
--rw-r--r--   0        0        0      744 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/api_handler/feature_job_setting_analysis.py
--rw-r--r--   0        0        0      762 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/api_handler/feature_list.py
--rw-r--r--   0        0        0      635 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/api_handler/feature_namespace.py
--rw-r--r--   0        0        0      430 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/api_handler/target_namespace.py
--rw-r--r--   0        0        0      469 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/api_handler/user_defined_function.py
--rw-r--r--   0        0        0    18841 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/api_object.py
--rw-r--r--   0        0        0     9984 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/api_object_util.py
--rw-r--r--   0        0        0     4996 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/asat_aggregator.py
--rw-r--r--   0        0        0    37664 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/base_table.py
--rw-r--r--   0        0        0     4833 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/batch_feature_table.py
--rw-r--r--   0        0        0     5062 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/batch_request_table.py
--rw-r--r--   0        0        0    40434 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/catalog.py
--rw-r--r--   0        0        0     1475 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/catalog_decorator.py
--rw-r--r--   0        0        0    13551 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/catalog_get_by_id_mixin.py
--rw-r--r--   0        0        0    11517 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/change_view.py
--rw-r--r--   0        0        0     6613 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/credential.py
--rw-r--r--   0        0        0     7615 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/data_source.py
--rw-r--r--   0        0        0    13859 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/deployment.py
--rw-r--r--   0        0        0     9699 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/dimension_table.py
--rw-r--r--   0        0        0     3107 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/dimension_view.py
--rw-r--r--   0        0        0    10127 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/entity.py
--rw-r--r--   0        0        0    22561 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/event_table.py
--rw-r--r--   0        0        0    15975 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/event_view.py
--rw-r--r--   0        0        0    47504 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/feature.py
--rw-r--r--   0        0        0    20227 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/feature_group.py
--rw-r--r--   0        0        0    15001 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/feature_job.py
--rw-r--r--   0        0        0     8703 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/feature_job_setting_analysis.py
--rw-r--r--   0        0        0    61414 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/feature_list.py
--rw-r--r--   0        0        0     3765 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/feature_namespace.py
--rw-r--r--   0        0        0     4220 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/feature_or_target_mixin.py
--rw-r--r--   0        0        0     1217 2023-07-25 05:44:21.017563 featurebyte-0.4.1/featurebyte/api/feature_or_target_namespace_mixin.py
--rw-r--r--   0        0        0    10024 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/feature_store.py
--rw-r--r--   0        0        0     2004 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/feature_util.py
--rw-r--r--   0        0        0      557 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/feature_validation_util.py
--rw-r--r--   0        0        0    20211 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/groupby.py
--rw-r--r--   0        0        0     4970 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/historical_feature_table.py
--rw-r--r--   0        0        0    16661 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/item_table.py
--rw-r--r--   0        0        0    11917 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/item_view.py
--rw-r--r--   0        0        0     2909 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/lag.py
--rw-r--r--   0        0        0     4909 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/materialized_table.py
--rw-r--r--   0        0        0     6301 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/mixin.py
--rw-r--r--   0        0        0     4995 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/observation_table.py
--rw-r--r--   0        0        0      721 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/periodic_task.py
--rw-r--r--   0        0        0     8485 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/relationship.py
--rw-r--r--   0        0        0     3474 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/request_column.py
--rw-r--r--   0        0        0     4464 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/savable_api_object.py
--rw-r--r--   0        0        0    21162 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/scd_table.py
--rw-r--r--   0        0        0     6023 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/scd_view.py
--rw-r--r--   0        0        0     3130 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/simple_aggregator.py
--rw-r--r--   0        0        0    46865 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/source_table.py
--rw-r--r--   0        0        0     5039 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/static_source_table.py
--rw-r--r--   0        0        0     5522 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/table.py
--rw-r--r--   0        0        0    14110 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/target.py
--rw-r--r--   0        0        0     3913 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/target_namespace.py
--rw-r--r--   0        0        0     5094 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/target_table.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/templates/__init__.py
--rw-r--r--   0        0        0     2054 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/templates/doc_util.py
--rw-r--r--   0        0        0     2611 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/templates/feature_or_target_doc.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/templates/online_serving/__init__.py
--rw-r--r--   0        0        0      707 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/templates/online_serving/python.tpl
--rw-r--r--   0        0        0      132 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/templates/online_serving/shell.tpl
--rw-r--r--   0        0        0      427 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/templates/series_doc.py
--rw-r--r--   0        0        0    18615 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/user_defined_function.py
--rw-r--r--   0        0        0    13245 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/user_defined_function_injector.py
--rw-r--r--   0        0        0    62136 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/view.py
--rw-r--r--   0        0        0     8379 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/window_aggregator.py
--rw-r--r--   0        0        0     1607 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/api/window_validator.py
--rw-r--r--   0        0        0     7924 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/app.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/common/__init__.py
--rw-r--r--   0        0        0     3116 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/common/date_util.py
--rw-r--r--   0        0        0      956 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/common/descriptor.py
--rw-r--r--   0        0        0      636 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/common/dict_util.py
--rw-r--r--   0        0        0     2090 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/common/doc_util.py
--rw-r--r--   0        0        0      692 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/common/documentation/allowed_classes.py
--rw-r--r--   0        0        0    16036 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/common/documentation/autodoc_processor.py
--rw-r--r--   0        0        0     1549 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/common/documentation/constants.py
--rw-r--r--   0        0        0     4485 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/common/documentation/custom_nav.py
--rw-r--r--   0        0        0     8560 2023-07-25 05:44:21.021563 featurebyte-0.4.1/featurebyte/common/documentation/doc_types.py
--rw-r--r--   0        0        0    42964 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/documentation/documentation_layout.py
--rw-r--r--   0        0        0     7430 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/documentation/extract_csv.py
--rw-r--r--   0        0        0     3479 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/documentation/formatters.py
--rw-r--r--   0        0        0    32026 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/documentation/gen_ref_pages_docs_builder.py
--rw-r--r--   0        0        0      877 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/documentation/markdown_extension/extension.py
--rw-r--r--   0        0        0     6198 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/documentation/pydantic_field_docs.py
--rw-r--r--   0        0        0    16371 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/documentation/resource_extractor.py
--rw-r--r--   0        0        0      519 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/documentation/resource_util.py
--rw-r--r--   0        0        0      200 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/documentation/util.py
--rw-r--r--   0        0        0     1246 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/env_util.py
--rw-r--r--   0        0        0     6740 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/formatting_util.py
--rw-r--r--   0        0        0     3925 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/join_utils.py
--rw-r--r--   0        0        0     4198 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/model_util.py
--rw-r--r--   0        0        0      815 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/path_util.py
--rw-r--r--   0        0        0     1062 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/progress.py
--rw-r--r--   0        0        0      451 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/singleton.py
--rw-r--r--   0        0        0     2666 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/typing.py
--rw-r--r--   0        0        0    10491 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/utils.py
--rw-r--r--   0        0        0     5180 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/common/validator.py
--rw-r--r--   0        0        0    13483 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/config.py
--rw-r--r--   0        0        0     1366 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/conftest.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/accessor/__init__.py
--rw-r--r--   0        0        0    15533 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/accessor/count_dict.py
--rw-r--r--   0        0        0    23735 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/accessor/datetime.py
--rw-r--r--   0        0        0    10075 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/accessor/feature_datetime.py
--rw-r--r--   0        0        0     8510 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/accessor/feature_string.py
--rw-r--r--   0        0        0    15765 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/accessor/string.py
--rw-r--r--   0        0        0     9213 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/accessor/target_datetime.py
--rw-r--r--   0        0        0     8168 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/accessor/target_string.py
--rw-r--r--   0        0        0     8902 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/frame.py
--rw-r--r--   0        0        0    11818 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/generic.py
--rw-r--r--   0        0        0    16742 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/mixin.py
--rw-r--r--   0        0        0    38755 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/series.py
--rw-r--r--   0        0        0     1484 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/timedelta.py
--rw-r--r--   0        0        0     6393 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/core/util.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/datasets/__init__.py
--rw-r--r--   0        0        0      697 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/datasets/__main__.py
--rw-r--r--   0        0        0     5546 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/datasets/app.py
--rw-r--r--   0        0        0     3125 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/datasets/creditcard.sql
--rw-r--r--   0        0        0     1154 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/datasets/doctest_grocery.sql
--rw-r--r--   0        0        0     2200 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/datasets/grocery.sql
--rw-r--r--   0        0        0     5757 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/datasets/healthcare.sql
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/docker/__init__.py
--rw-r--r--   0        0        0     4650 2023-07-25 05:45:11.269717 featurebyte-0.4.1/featurebyte/docker/featurebyte.yml
--rw-r--r--   0        0        0    11444 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/docker/manager.py
--rw-r--r--   0        0        0    10597 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/enum.py
--rw-r--r--   0        0        0     9387 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/exception.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.025563 featurebyte-0.4.1/featurebyte/feature_manager/__init__.py
--rw-r--r--   0        0        0     2065 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/feature_manager/model.py
--rw-r--r--   0        0        0      785 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/feature_manager/sql_template.py
--rw-r--r--   0        0        0     3667 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/feature_utility.py
--rw-r--r--   0        0        0     4145 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/logging.py
--rw-r--r--   0        0        0     8053 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/middleware.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/migration/__init__.py
--rw-r--r--   0        0        0      604 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/migration/migration_data_service.py
--rw-r--r--   0        0        0     1703 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/migration/model.py
--rw-r--r--   0        0        0     9020 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/migration/run.py
--rw-r--r--   0        0        0     1442 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/migration/service/__init__.py
--rw-r--r--   0        0        0    10260 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/migration/service/data_warehouse.py
--rw-r--r--   0        0        0     7689 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/migration/service/mixin.py
--rw-r--r--   0        0        0      694 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/__init__.py
--rw-r--r--   0        0        0    11865 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/base.py
--rw-r--r--   0        0        0      392 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/base_feature_or_target_table.py
--rw-r--r--   0        0        0      617 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/batch_feature_table.py
--rw-r--r--   0        0        0     1726 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/batch_request_table.py
--rw-r--r--   0        0        0     2377 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/catalog.py
--rw-r--r--   0        0        0     1611 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/context.py
--rw-r--r--   0        0        0    10169 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/credential.py
--rw-r--r--   0        0        0     1333 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/deployment.py
--rw-r--r--   0        0        0     2026 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/dimension_table.py
--rw-r--r--   0        0        0     3618 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/entity.py
--rw-r--r--   0        0        0     3051 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/entity_validation.py
--rw-r--r--   0        0        0     3551 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/event_table.py
--rw-r--r--   0        0        0    11876 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/feature.py
--rw-r--r--   0        0        0     3750 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/feature_job_setting_analysis.py
--rw-r--r--   0        0        0    22006 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/feature_list.py
--rw-r--r--   0        0        0     4704 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/feature_namespace.py
--rw-r--r--   0        0        0     7622 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/feature_store.py
--rw-r--r--   0        0        0      659 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/historical_feature_table.py
--rw-r--r--   0        0        0     2919 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/item_table.py
--rw-r--r--   0        0        0     1620 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/materialized_table.py
--rw-r--r--   0        0        0     2113 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/observation_table.py
--rw-r--r--   0        0        0     3861 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/online_store.py
--rw-r--r--   0        0        0     1845 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/online_store_compute_query.py
--rw-r--r--   0        0        0     1295 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/online_store_table_version.py
--rw-r--r--   0        0        0     1433 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/parent_serving.py
--rw-r--r--   0        0        0     2891 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/periodic_task.py
--rw-r--r--   0        0        0     1492 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/persistent.py
--rw-r--r--   0        0        0     1024 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/proxy_table.py
--rw-r--r--   0        0        0     4330 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/relationship.py
--rw-r--r--   0        0        0      944 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/relationship_analysis.py
--rw-r--r--   0        0        0     8647 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/request_input.py
--rw-r--r--   0        0        0     3554 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/scd_table.py
--rw-r--r--   0        0        0     1435 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/semantic.py
--rw-r--r--   0        0        0     1428 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/static_source_table.py
--rw-r--r--   0        0        0     2834 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/target.py
--rw-r--r--   0        0        0     2107 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/target_namespace.py
--rw-r--r--   0        0        0      595 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/target_table.py
--rw-r--r--   0        0        0     1085 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/task.py
--rw-r--r--   0        0        0     4041 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/tile.py
--rw-r--r--   0        0        0     1259 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/tile_job_log.py
--rw-r--r--   0        0        0     2968 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/tile_registry.py
--rw-r--r--   0        0        0    10462 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/models/user_defined_function.py
--rw-r--r--   0        0        0      154 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/persistent/__init__.py
--rw-r--r--   0        0        0     9544 2023-07-25 05:44:21.029563 featurebyte-0.4.1/featurebyte/persistent/audit.py
--rw-r--r--   0        0        0    22972 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/persistent/base.py
--rw-r--r--   0        0        0     9824 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/persistent/mongo.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/__init__.py
--rw-r--r--   0        0        0     2533 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/algorithm.py
--rw-r--r--   0        0        0     3103 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/enum.py
--rw-r--r--   0        0        0    19691 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/graph.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/graph_node/__init__.py
--rw-r--r--   0        0        0     4592 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/graph_node/base.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/model/__init__.py
--rw-r--r--   0        0        0      873 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/model/column_info.py
--rw-r--r--   0        0        0    12700 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/model/common_table.py
--rw-r--r--   0        0        0     1707 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/model/critical_data_info.py
--rw-r--r--   0        0        0     6699 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/model/feature_job_setting.py
--rw-r--r--   0        0        0    19287 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/model/graph.py
--rw-r--r--   0        0        0    23872 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/model/table.py
--rw-r--r--   0        0        0     1076 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/__init__.py
--rw-r--r--   0        0        0     5236 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/agg_func.py
--rw-r--r--   0        0        0    28314 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/base.py
--rw-r--r--   0        0        0     5172 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/binary.py
--rw-r--r--   0        0        0    17953 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/cleaning_operation.py
--rw-r--r--   0        0        0     7797 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/count_dict.py
--rw-r--r--   0        0        0     7293 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/date.py
--rw-r--r--   0        0        0    10182 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/function.py
--rw-r--r--   0        0        0    64270 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/generic.py
--rw-r--r--   0        0        0    17083 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/input.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/metadata/__init__.py
--rw-r--r--   0        0        0      873 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/metadata/column.py
--rw-r--r--   0        0        0    22891 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/metadata/operation.py
--rw-r--r--   0        0        0    20687 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/metadata/sdk_code.py
--rw-r--r--   0        0        0       47 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/metadata/templates/sdk_code.tpl
--rw-r--r--   0        0        0     7503 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/mixin.py
--rw-r--r--   0        0        0    21084 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/nested.py
--rw-r--r--   0        0        0     3272 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/request.py
--rw-r--r--   0        0        0     2054 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/scalar.py
--rw-r--r--   0        0        0     6696 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/schema.py
--rw-r--r--   0        0        0     5461 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/string.py
--rw-r--r--   0        0        0     4824 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/unary.py
--rw-r--r--   0        0        0     1042 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/node/validator.py
--rw-r--r--   0        0        0     1050 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/pruning_util.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/sql/__init__.py
--rw-r--r--   0        0        0     1060 2023-07-25 05:44:21.033563 featurebyte-0.4.1/featurebyte/query_graph/sql/adapter/__init__.py
--rw-r--r--   0        0        0    18300 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/adapter/base.py
--rw-r--r--   0        0        0     7716 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/adapter/databricks.py
--rw-r--r--   0        0        0    10999 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/adapter/snowflake.py
--rw-r--r--   0        0        0     1738 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/adapter/spark.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/__init__.py
--rw-r--r--   0        0        0     7198 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/asat.py
--rw-r--r--   0        0        0    22320 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/base.py
--rw-r--r--   0        0        0     6446 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/forward.py
--rw-r--r--   0        0        0     5739 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/item.py
--rw-r--r--   0        0        0     3801 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/latest.py
--rw-r--r--   0        0        0     9549 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/lookup.py
--rw-r--r--   0        0        0     3811 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/request_table.py
--rw-r--r--   0        0        0    26795 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/window.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/__init__.py
--rw-r--r--   0        0        0     6184 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/aggregate.py
--rw-r--r--   0        0        0    12647 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/base.py
--rw-r--r--   0        0        0     2723 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/binary.py
--rw-r--r--   0        0        0     5740 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/count_dict.py
--rw-r--r--   0        0        0    10402 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/datetime.py
--rw-r--r--   0        0        0     1907 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/function.py
--rw-r--r--   0        0        0     7163 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/generic.py
--rw-r--r--   0        0        0     2409 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/groupby.py
--rw-r--r--   0        0        0     2593 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/input.py
--rw-r--r--   0        0        0     1449 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/is_in.py
--rw-r--r--   0        0        0     6208 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/join.py
--rw-r--r--   0        0        0     6138 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/join_feature.py
--rw-r--r--   0        0        0     2291 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/literal.py
--rw-r--r--   0        0        0      878 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/request.py
--rw-r--r--   0        0        0     8251 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/string.py
--rw-r--r--   0        0        0    11756 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/tile.py
--rw-r--r--   0        0        0     5170 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/track_changes.py
--rw-r--r--   0        0        0     5157 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/unary.py
--rw-r--r--   0        0        0     2536 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/ast/util.py
--rw-r--r--   0        0        0     7070 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/builder.py
--rw-r--r--   0        0        0     4909 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/common.py
--rw-r--r--   0        0        0     1704 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/dataframe.py
--rw-r--r--   0        0        0     1865 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/expression.py
--rw-r--r--   0        0        0    21590 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/feature_compute.py
--rw-r--r--   0        0        0    20358 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/feature_historical.py
--rw-r--r--   0        0        0     4642 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/feature_preview.py
--rw-r--r--   0        0        0     4449 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/groupby_helper.py
--rw-r--r--   0        0        0      426 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/interpreter/__init__.py
--rw-r--r--   0        0        0     3512 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/interpreter/base.py
--rw-r--r--   0        0        0    27742 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/interpreter/preview.py
--rw-r--r--   0        0        0     6685 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/interpreter/tile.py
--rw-r--r--   0        0        0     4027 2023-07-25 05:44:21.037563 featurebyte-0.4.1/featurebyte/query_graph/sql/materialisation.py
--rw-r--r--   0        0        0     9430 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/sql/online_serving.py
--rw-r--r--   0        0        0     1305 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/sql/online_serving_util.py
--rw-r--r--   0        0        0    10730 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/sql/online_store_compute_query.py
--rw-r--r--   0        0        0     5771 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/sql/parent_serving.py
--rw-r--r--   0        0        0    15948 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/sql/scd_helper.py
--rw-r--r--   0        0        0    24706 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/sql/specs.py
--rw-r--r--   0        0        0     2206 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/sql/template.py
--rw-r--r--   0        0        0    12508 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/sql/tile_compute.py
--rw-r--r--   0        0        0     8103 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/sql/tile_util.py
--rw-r--r--   0        0        0     9354 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/sql/tiling.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/transform/__init__.py
--rw-r--r--   0        0        0     5184 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/transform/base.py
--rw-r--r--   0        0        0     2482 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/transform/entity_extractor.py
--rw-r--r--   0        0        0     4925 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/transform/flattening.py
--rw-r--r--   0        0        0     6715 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/transform/operation_structure.py
--rw-r--r--   0        0        0    19339 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/transform/pruning.py
--rw-r--r--   0        0        0     3225 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/transform/quick_pruning.py
--rw-r--r--   0        0        0    10147 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/transform/reconstruction.py
--rw-r--r--   0        0        0    13262 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/transform/sdk_code.py
--rw-r--r--   0        0        0     5951 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/query_graph/util.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/__init__.py
--rw-r--r--   0        0        0     9852 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/app_container_config.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/batch_feature_table/__init__.py
--rw-r--r--   0        0        0     5506 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/batch_feature_table/api.py
--rw-r--r--   0        0        0     5197 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/batch_feature_table/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/batch_request_table/__init__.py
--rw-r--r--   0        0        0     5534 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/batch_request_table/api.py
--rw-r--r--   0        0        0     3753 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/batch_request_table/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/catalog/__init__.py
--rw-r--r--   0        0        0     4855 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/catalog/api.py
--rw-r--r--   0        0        0     1374 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/catalog/catalog_name_injector.py
--rw-r--r--   0        0        0     2429 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/catalog/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/common/__init__.py
--rw-r--r--   0        0        0    11843 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/common/base.py
--rw-r--r--   0        0        0     4141 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/common/base_materialized_table.py
--rw-r--r--   0        0        0     5390 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/common/base_table.py
--rw-r--r--   0        0        0     4900 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/common/feature_metadata_extractor.py
--rw-r--r--   0        0        0     8746 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/common/feature_or_target_table.py
--rw-r--r--   0        0        0      886 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/common/schema.py
--rw-r--r--   0        0        0      400 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/common/util.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/context/__init__.py
--rw-r--r--   0        0        0     3655 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/context/api.py
--rw-r--r--   0        0        0     1596 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/context/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/credential/__init__.py
--rw-r--r--   0        0        0     5141 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/credential/api.py
--rw-r--r--   0        0        0     3766 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/credential/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/deployment/__init__.py
--rw-r--r--   0        0        0     6193 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/deployment/api.py
--rw-r--r--   0        0        0    11712 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/deployment/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/dimension_table/__init__.py
--rw-r--r--   0        0        0     4814 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/dimension_table/api.py
--rw-r--r--   0        0        0     2670 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/dimension_table/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.041563 featurebyte-0.4.1/featurebyte/routes/entity/__init__.py
--rw-r--r--   0        0        0     4769 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/entity/api.py
--rw-r--r--   0        0        0     2949 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/entity/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/event_table/__init__.py
--rw-r--r--   0        0        0     5278 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/event_table/api.py
--rw-r--r--   0        0        0     2901 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/event_table/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature/__init__.py
--rw-r--r--   0        0        0     6905 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature/api.py
--rw-r--r--   0        0        0    22334 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_job_setting_analysis/__init__.py
--rw-r--r--   0        0        0     6253 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_job_setting_analysis/api.py
--rw-r--r--   0        0        0     6016 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_job_setting_analysis/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_list/__init__.py
--rw-r--r--   0        0        0     8251 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_list/api.py
--rw-r--r--   0        0        0    16099 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_list/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_list_namespace/__init__.py
--rw-r--r--   0        0        0     5061 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_list_namespace/api.py
--rw-r--r--   0        0        0     7212 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_list_namespace/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_namespace/__init__.py
--rw-r--r--   0        0        0     4639 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_namespace/api.py
--rw-r--r--   0        0        0    10655 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_namespace/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_store/__init__.py
--rw-r--r--   0        0        0     8551 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_store/api.py
--rw-r--r--   0        0        0    12839 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/feature_store/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/historical_feature_table/__init__.py
--rw-r--r--   0        0        0     6028 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/historical_feature_table/api.py
--rw-r--r--   0        0        0     3963 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/historical_feature_table/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/item_table/__init__.py
--rw-r--r--   0        0        0     4410 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/item_table/api.py
--rw-r--r--   0        0        0     2833 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/item_table/controller.py
--rw-r--r--   0        0        0     5888 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/lazy_app_container.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/observation_table/__init__.py
--rw-r--r--   0        0        0     5423 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/observation_table/api.py
--rw-r--r--   0        0        0     3589 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/observation_table/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/periodic_tasks/__init__.py
--rw-r--r--   0        0        0     2179 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/periodic_tasks/api.py
--rw-r--r--   0        0        0      540 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/periodic_tasks/controller.py
--rw-r--r--   0        0        0    16659 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/registry.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/relationship_info/__init__.py
--rw-r--r--   0        0        0     4348 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/relationship_info/api.py
--rw-r--r--   0        0        0     5644 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/relationship_info/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/scd_table/__init__.py
--rw-r--r--   0        0        0     4335 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/scd_table/api.py
--rw-r--r--   0        0        0     3146 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/scd_table/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/semantic/__init__.py
--rw-r--r--   0        0        0     4292 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/semantic/api.py
--rw-r--r--   0        0        0     1380 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/semantic/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/static_source_table/__init__.py
--rw-r--r--   0        0        0     5536 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/static_source_table/api.py
--rw-r--r--   0        0        0     3664 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/static_source_table/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/table/__init__.py
--rw-r--r--   0        0        0     1469 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/table/api.py
--rw-r--r--   0        0        0      464 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/table/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/target/__init__.py
--rw-r--r--   0        0        0     4554 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/target/api.py
--rw-r--r--   0        0        0     6373 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/target/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/target_namespace/__init__.py
--rw-r--r--   0        0        0     5024 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/target_namespace/api.py
--rw-r--r--   0        0        0     1825 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/target_namespace/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/target_table/__init__.py
--rw-r--r--   0        0        0     5186 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/target_table/api.py
--rw-r--r--   0        0        0     3142 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/target_table/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/task/__init__.py
--rw-r--r--   0        0        0     1045 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/task/api.py
--rw-r--r--   0        0        0     1892 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/task/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/temp_data/__init__.py
--rw-r--r--   0        0        0      582 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/temp_data/api.py
--rw-r--r--   0        0        0     1353 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/temp_data/controller.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.045563 featurebyte-0.4.1/featurebyte/routes/user_defined_function/__init__.py
--rw-r--r--   0        0        0     5845 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/routes/user_defined_function/api.py
--rw-r--r--   0        0        0    10715 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/routes/user_defined_function/controller.py
--rw-r--r--   0        0        0      180 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/__init__.py
--rw-r--r--   0        0        0     1431 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/batch_feature_table.py
--rw-r--r--   0        0        0      842 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/batch_request_table.py
--rw-r--r--   0        0        0     1517 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/catalog.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/common/__init__.py
--rw-r--r--   0        0        0     1226 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/common/base.py
--rw-r--r--   0        0        0      643 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/common/feature_or_target.py
--rw-r--r--   0        0        0     3662 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/common/operation.py
--rw-r--r--   0        0        0     1508 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/context.py
--rw-r--r--   0        0        0     3658 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/credential.py
--rw-r--r--   0        0        0     1686 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/deployment.py
--rw-r--r--   0        0        0      981 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/dimension_table.py
--rw-r--r--   0        0        0     1684 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/entity.py
--rw-r--r--   0        0        0     2391 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/event_table.py
--rw-r--r--   0        0        0     6127 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/feature.py
--rw-r--r--   0        0        0     4664 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/feature_job_setting_analysis.py
--rw-r--r--   0        0        0     4836 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/feature_list.py
--rw-r--r--   0        0        0     1470 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/feature_list_namespace.py
--rw-r--r--   0        0        0     2062 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/feature_namespace.py
--rw-r--r--   0        0        0     3589 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/feature_store.py
--rw-r--r--   0        0        0     1410 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/historical_feature_table.py
--rw-r--r--   0        0        0    11647 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/info.py
--rw-r--r--   0        0        0      991 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/item_table.py
--rw-r--r--   0        0        0      599 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/materialized_table.py
--rw-r--r--   0        0        0      909 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/observation_table.py
--rw-r--r--   0        0        0      459 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/periodic_task.py
--rw-r--r--   0        0        0      478 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/preview.py
--rw-r--r--   0        0        0     1460 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/relationship_info.py
--rw-r--r--   0        0        0     1190 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/request_table.py
--rw-r--r--   0        0        0     1376 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/scd_table.py
--rw-r--r--   0        0        0      914 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/semantic.py
--rw-r--r--   0        0        0     1152 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/static_source_table.py
--rw-r--r--   0        0        0     2415 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/table.py
--rw-r--r--   0        0        0     2974 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/target.py
--rw-r--r--   0        0        0     1852 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/target_namespace.py
--rw-r--r--   0        0        0     1644 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/target_table.py
--rw-r--r--   0        0        0     1012 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/task.py
--rw-r--r--   0        0        0     1916 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/user_defined_function.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/__init__.py
--rw-r--r--   0        0        0      333 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/progress.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/__init__.py
--rw-r--r--   0        0        0     2829 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/base.py
--rw-r--r--   0        0        0      739 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/batch_feature_create.py
--rw-r--r--   0        0        0      610 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/batch_feature_table.py
--rw-r--r--   0        0        0      602 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/batch_request_table.py
--rw-r--r--   0        0        0     1382 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/deployment_create_update.py
--rw-r--r--   0        0        0     1328 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/feature_job_setting_analysis.py
--rw-r--r--   0        0        0      677 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/feature_list_batch_feature_create.py
--rw-r--r--   0        0        0      725 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/historical_feature_table.py
--rw-r--r--   0        0        0     1459 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/materialized_table_delete.py
--rw-r--r--   0        0        0      589 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/observation_table.py
--rw-r--r--   0        0        0      602 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/static_source_table.py
--rw-r--r--   0        0        0      576 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/target_table.py
--rw-r--r--   0        0        0      544 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/test.py
--rw-r--r--   0        0        0      459 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/schema/worker/task/tile.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/service/__init__.py
--rw-r--r--   0        0        0    34638 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/service/base_document.py
--rw-r--r--   0        0        0     1090 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/service/base_namespace_service.py
--rw-r--r--   0        0        0     5215 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/service/base_table_document.py
--rw-r--r--   0        0        0     1929 2023-07-25 05:44:21.049563 featurebyte-0.4.1/featurebyte/service/batch_feature_table.py
--rw-r--r--   0        0        0     2831 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/batch_request_table.py
--rw-r--r--   0        0        0      596 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/catalog.py
--rw-r--r--   0        0        0     5638 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/context.py
--rw-r--r--   0        0        0     5665 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/credential.py
--rw-r--r--   0        0        0     4606 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/default_version_mode.py
--rw-r--r--   0        0        0    18089 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/deploy.py
--rw-r--r--   0        0        0      653 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/deployment.py
--rw-r--r--   0        0        0      674 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/dimension_table.py
--rw-r--r--   0        0        0     4246 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/entity.py
--rw-r--r--   0        0        0     7231 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/entity_validation.py
--rw-r--r--   0        0        0      618 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/event_table.py
--rw-r--r--   0        0        0     6732 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/feature.py
--rw-r--r--   0        0        0     3742 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/feature_job_setting_analysis.py
--rw-r--r--   0        0        0    16639 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/feature_list.py
--rw-r--r--   0        0        0     4268 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/feature_list_namespace.py
--rw-r--r--   0        0        0     4251 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/feature_list_status.py
--rw-r--r--   0        0        0    12724 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/feature_manager.py
--rw-r--r--   0        0        0      574 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/feature_namespace.py
--rw-r--r--   0        0        0    12595 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/feature_preview.py
--rw-r--r--   0        0        0    15619 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/feature_readiness.py
--rw-r--r--   0        0        0     1468 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/feature_store.py
--rw-r--r--   0        0        0     8851 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/feature_store_warehouse.py
--rw-r--r--   0        0        0     3392 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/historical_feature_table.py
--rw-r--r--   0        0        0    14351 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/historical_features.py
--rw-r--r--   0        0        0      604 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/item_table.py
--rw-r--r--   0        0        0     4808 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/materialized_table.py
--rw-r--r--   0        0        0     4446 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/mixin.py
--rw-r--r--   0        0        0     5383 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/namespace_handler.py
--rw-r--r--   0        0        0     6290 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/observation_table.py
--rw-r--r--   0        0        0     9227 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/online_enable.py
--rw-r--r--   0        0        0     4540 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/online_serving.py
--rw-r--r--   0        0        0     2637 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/online_store_compute_query_service.py
--rw-r--r--   0        0        0     3016 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/online_store_table_version.py
--rw-r--r--   0        0        0     7009 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/parent_serving.py
--rw-r--r--   0        0        0      437 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/periodic_task.py
--rw-r--r--   0        0        0    10079 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/preview.py
--rw-r--r--   0        0        0     9258 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/relationship.py
--rw-r--r--   0        0        0     2311 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/relationship_info.py
--rw-r--r--   0        0        0      991 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/sanitizer.py
--rw-r--r--   0        0        0      590 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/scd_table.py
--rw-r--r--   0        0        0      600 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/semantic.py
--rw-r--r--   0        0        0     2830 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/session_manager.py
--rw-r--r--   0        0        0     6617 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/session_validator.py
--rw-r--r--   0        0        0     2930 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/static_source_table.py
--rw-r--r--   0        0        0     1051 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/table.py
--rw-r--r--   0        0        0    16479 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/table_columns_info.py
--rw-r--r--   0        0        0     3275 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/table_info.py
--rw-r--r--   0        0        0     2081 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/table_status.py
--rw-r--r--   0        0        0     6967 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/target.py
--rw-r--r--   0        0        0     6520 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/target_helper/base_feature_or_target_computer.py
--rw-r--r--   0        0        0     5195 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/target_helper/compute_target.py
--rw-r--r--   0        0        0      535 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/target_namespace.py
--rw-r--r--   0        0        0     3085 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/target_table.py
--rw-r--r--   0        0        0     9795 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/task_manager.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/tile/__init__.py
--rw-r--r--   0        0        0    11222 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/tile/tile_task_executor.py
--rw-r--r--   0        0        0     2362 2023-07-25 05:44:21.053563 featurebyte-0.4.1/featurebyte/service/tile_cache.py
--rw-r--r--   0        0        0     7045 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/tile_job_log.py
--rw-r--r--   0        0        0    14700 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/tile_manager.py
--rw-r--r--   0        0        0     2681 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/tile_registry_service.py
--rw-r--r--   0        0        0     2519 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/tile_scheduler.py
--rw-r--r--   0        0        0     2662 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/user_defined_function.py
--rw-r--r--   0        0        0      709 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/user_service.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/validator/__init__.py
--rw-r--r--   0        0        0     6291 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/validator/materialized_table_delete.py
--rw-r--r--   0        0        0    11655 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/validator/production_ready_validator.py
--rw-r--r--   0        0        0    15448 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/version.py
--rw-r--r--   0        0        0    13077 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/view_construction.py
--rw-r--r--   0        0        0     4591 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/service/working_schema.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/__init__.py
--rw-r--r--   0        0        0    29242 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/base.py
--rw-r--r--   0        0        0    16306 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/base_spark.py
--rw-r--r--   0        0        0     5643 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/databricks.py
--rw-r--r--   0        0        0      434 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/enum.py
--rw-r--r--   0        0        0     4993 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/hive.py
--rw-r--r--   0        0        0     5107 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/manager.py
--rw-r--r--   0        0        0     9179 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/simple_storage.py
--rw-r--r--   0        0        0    13216 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/snowflake.py
--rw-r--r--   0        0        0    11998 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/spark.py
--rw-r--r--   0        0        0     3479 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/sqlite.py
--rw-r--r--   0        0        0     6615 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/session/webhdfs.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/__init__.py
--rw-r--r--   0        0        0     2569 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/base.py
--rw-r--r--   0        0        0     2743 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/common.py
--rw-r--r--   0        0        0        6 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/databricks/.gitignore
--rw-r--r--   0        0        0      957 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql
--rw-r--r--   0        0        0      476 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/F_COUNT_DICT_ENTROPY.sql
--rw-r--r--   0        0        0      171 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT.sql
--rw-r--r--   0        0        0      610 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql
--rw-r--r--   0        0        0      177 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_VALUE.sql
--rw-r--r--   0        0        0      188 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/F_COUNT_DICT_NUM_UNIQUE.sql
--rw-r--r--   0        0        0     1491 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/F_GET_RANK.sql
--rw-r--r--   0        0        0      449 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/F_GET_RELATIVE_FREQUENCY.sql
--rw-r--r--   0        0        0      559 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql
--rw-r--r--   0        0        0      559 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql
--rw-r--r--   0        0        0      653 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql
--rw-r--r--   0        0        0      153 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/snowflake/T_TILE_MONITOR_SUMMARY.sql
--rw-r--r--   0        0        0        6 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/spark/.gitignore
--rw-r--r--   0        0        0      191 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/spark/T_TILE_MONITOR_SUMMARY.sql
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/spark/__init__.py
--rw-r--r--   0        0        0    29714 2023-07-25 05:46:47.410013 featurebyte-0.4.1/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar
--rw-r--r--   0        0        0     1923 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/tile_common.py
--rw-r--r--   0        0        0     5635 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/tile_generate.py
--rw-r--r--   0        0        0     3564 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/tile_generate_entity_tracking.py
--rw-r--r--   0        0        0     8611 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/tile_monitor.py
--rw-r--r--   0        0        0     2833 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/tile_registry.py
--rw-r--r--   0        0        0     6829 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/sql/tile_schedule_online_store.py
--rw-r--r--   0        0        0      297 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/storage/__init__.py
--rw-r--r--   0        0        0     4999 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/storage/base.py
--rw-r--r--   0        0        0     3640 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/storage/local.py
--rw-r--r--   0        0        0      415 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/storage/local_temp.py
--rw-r--r--   0        0        0     5575 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/storage/s3.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/tile/__init__.py
--rw-r--r--   0        0        0      411 2023-07-25 05:44:21.057563 featurebyte-0.4.1/featurebyte/tile/sql_template.py
--rw-r--r--   0        0        0    26885 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/tile/tile_cache.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/utils/__init__.py
--rw-r--r--   0        0        0     1909 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/utils/credential.py
--rw-r--r--   0        0        0     1532 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/utils/messaging.py
--rw-r--r--   0        0        0      534 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/utils/persistent.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/utils/snowflake/__init__.py
--rw-r--r--   0        0        0      462 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/utils/snowflake/sql.py
--rw-r--r--   0        0        0     2225 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/utils/storage.py
--rw-r--r--   0        0        0     1990 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/__init__.py
--rw-r--r--   0        0        0      170 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/enum.py
--rw-r--r--   0        0        0     1159 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/progress.py
--rw-r--r--   0        0        0     2502 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/schedulers.py
--rw-r--r--   0        0        0      230 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/start.py
--rw-r--r--   0        0        0      214 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/__init__.py
--rw-r--r--   0        0        0     2926 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/base.py
--rw-r--r--   0        0        0    11492 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/batch_feature_create.py
--rw-r--r--   0        0        0     3718 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/batch_feature_table.py
--rw-r--r--   0        0        0     2243 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/batch_request_table.py
--rw-r--r--   0        0        0     1795 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/deployment_create_update.py
--rw-r--r--   0        0        0     6763 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/feature_job_setting_analysis.py
--rw-r--r--   0        0        0     1463 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/feature_list_batch_feature_create.py
--rw-r--r--   0        0        0     3502 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/historical_feature_table.py
--rw-r--r--   0        0        0     5405 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/materialized_table_delete.py
--rw-r--r--   0        0        0     2604 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/mixin.py
--rw-r--r--   0        0        0     2226 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/observation_table.py
--rw-r--r--   0        0        0     2197 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/static_source_table.py
--rw-r--r--   0        0        0     3287 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/target_table.py
--rw-r--r--   0        0        0      626 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/test_task.py
--rw-r--r--   0        0        0     1541 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task/tile_task.py
--rw-r--r--   0        0        0     6279 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/task_executor.py
--rw-r--r--   0        0        0        0 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/util/__init__.py
--rw-r--r--   0        0        0     1773 2023-07-25 05:44:21.061563 featurebyte-0.4.1/featurebyte/worker/util/observation_set_helper.py
--rw-r--r--   0        0        0     7915 2023-07-25 05:45:08.117707 featurebyte-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    23156 1970-01-01 00:00:00.000000 featurebyte-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-08-07 07:53:48.491413 featurebyte-0.4.2/LICENSE
+-rw-r--r--   0        0        0    19816 2023-08-07 07:53:48.491413 featurebyte-0.4.2/README.md
+-rw-r--r--   0        0        0    17168 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/__init__.py
+-rw-r--r--   0        0        0     2552 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/aggregator/__init__.py
+-rw-r--r--   0        0        0     6422 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/aggregator/base_aggregator.py
+-rw-r--r--   0        0        0     5208 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/aggregator/forward_aggregator.py
+-rw-r--r--   0        0        0     5372 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/api_handler/base.py
+-rw-r--r--   0        0        0      502 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/api_handler/catalog.py
+-rw-r--r--   0        0        0      531 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/api_handler/feature.py
+-rw-r--r--   0        0        0      744 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/api_handler/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0      762 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/api_handler/feature_list.py
+-rw-r--r--   0        0        0      635 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/api_handler/feature_namespace.py
+-rw-r--r--   0        0        0      430 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/api_handler/target_namespace.py
+-rw-r--r--   0        0        0      469 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/api_handler/user_defined_function.py
+-rw-r--r--   0        0        0    18841 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/api_object.py
+-rw-r--r--   0        0        0     9931 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/api_object_util.py
+-rw-r--r--   0        0        0     4996 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/asat_aggregator.py
+-rw-r--r--   0        0        0    37664 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/base_table.py
+-rw-r--r--   0        0        0     4833 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/batch_feature_table.py
+-rw-r--r--   0        0        0     5062 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/batch_request_table.py
+-rw-r--r--   0        0        0    39290 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/catalog.py
+-rw-r--r--   0        0        0     1475 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/catalog_decorator.py
+-rw-r--r--   0        0        0    12903 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/catalog_get_by_id_mixin.py
+-rw-r--r--   0        0        0    11517 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/change_view.py
+-rw-r--r--   0        0        0     6613 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/credential.py
+-rw-r--r--   0        0        0     7615 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/data_source.py
+-rw-r--r--   0        0        0    13859 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/deployment.py
+-rw-r--r--   0        0        0     9699 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/dimension_table.py
+-rw-r--r--   0        0        0     3107 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/dimension_view.py
+-rw-r--r--   0        0        0    10127 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/entity.py
+-rw-r--r--   0        0        0    22561 2023-08-07 07:53:48.495413 featurebyte-0.4.2/featurebyte/api/event_table.py
+-rw-r--r--   0        0        0    15981 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/event_view.py
+-rw-r--r--   0        0        0    45550 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/feature.py
+-rw-r--r--   0        0        0    20227 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/feature_group.py
+-rw-r--r--   0        0        0    15001 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/feature_job.py
+-rw-r--r--   0        0        0     8703 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0    61419 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/feature_list.py
+-rw-r--r--   0        0        0     3765 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/feature_namespace.py
+-rw-r--r--   0        0        0     6218 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/feature_or_target_mixin.py
+-rw-r--r--   0        0        0     1217 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/feature_or_target_namespace_mixin.py
+-rw-r--r--   0        0        0    10024 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/feature_store.py
+-rw-r--r--   0        0        0     2004 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/feature_util.py
+-rw-r--r--   0        0        0      557 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/feature_validation_util.py
+-rw-r--r--   0        0        0    20535 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/groupby.py
+-rw-r--r--   0        0        0     4970 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/historical_feature_table.py
+-rw-r--r--   0        0        0    16661 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/item_table.py
+-rw-r--r--   0        0        0    11923 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/item_view.py
+-rw-r--r--   0        0        0     2909 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/lag.py
+-rw-r--r--   0        0        0     4909 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/materialized_table.py
+-rw-r--r--   0        0        0     6301 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/mixin.py
+-rw-r--r--   0        0        0     4995 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/observation_table.py
+-rw-r--r--   0        0        0      721 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/periodic_task.py
+-rw-r--r--   0        0        0     8485 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/relationship.py
+-rw-r--r--   0        0        0     3474 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/request_column.py
+-rw-r--r--   0        0        0     4464 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/savable_api_object.py
+-rw-r--r--   0        0        0    21162 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/scd_table.py
+-rw-r--r--   0        0        0     6029 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/scd_view.py
+-rw-r--r--   0        0        0     3130 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/simple_aggregator.py
+-rw-r--r--   0        0        0    46865 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/source_table.py
+-rw-r--r--   0        0        0     5039 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/static_source_table.py
+-rw-r--r--   0        0        0     5522 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/table.py
+-rw-r--r--   0        0        0    14663 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/target.py
+-rw-r--r--   0        0        0     3913 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/target_namespace.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/templates/__init__.py
+-rw-r--r--   0        0        0     2054 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/templates/doc_util.py
+-rw-r--r--   0        0        0     2611 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/templates/feature_or_target_doc.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/templates/online_serving/__init__.py
+-rw-r--r--   0        0        0      707 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/templates/online_serving/python.tpl
+-rw-r--r--   0        0        0      132 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/templates/online_serving/shell.tpl
+-rw-r--r--   0        0        0      427 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/templates/series_doc.py
+-rw-r--r--   0        0        0    18615 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/user_defined_function.py
+-rw-r--r--   0        0        0    13245 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/user_defined_function_injector.py
+-rw-r--r--   0        0        0    66979 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/view.py
+-rw-r--r--   0        0        0     8379 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/window_aggregator.py
+-rw-r--r--   0        0        0     1976 2023-08-07 07:53:48.499413 featurebyte-0.4.2/featurebyte/api/window_validator.py
+-rw-r--r--   0        0        0     7924 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/app.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/__init__.py
+-rw-r--r--   0        0        0     3116 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/date_util.py
+-rw-r--r--   0        0        0      956 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/descriptor.py
+-rw-r--r--   0        0        0      636 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/dict_util.py
+-rw-r--r--   0        0        0     2090 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/doc_util.py
+-rw-r--r--   0        0        0      692 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/allowed_classes.py
+-rw-r--r--   0        0        0    15668 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/autodoc_processor.py
+-rw-r--r--   0        0        0     1552 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/constants.py
+-rw-r--r--   0        0        0     4487 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/custom_nav.py
+-rw-r--r--   0        0        0     8560 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/doc_types.py
+-rw-r--r--   0        0        0    42562 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/documentation_layout.py
+-rw-r--r--   0        0        0     7430 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/extract_csv.py
+-rw-r--r--   0        0        0     3479 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/formatters.py
+-rw-r--r--   0        0        0    32026 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/gen_ref_pages_docs_builder.py
+-rw-r--r--   0        0        0      877 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/markdown_extension/extension.py
+-rw-r--r--   0        0        0     6198 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/pydantic_field_docs.py
+-rw-r--r--   0        0        0    16371 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/resource_extractor.py
+-rw-r--r--   0        0        0      519 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/resource_util.py
+-rw-r--r--   0        0        0      200 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/documentation/util.py
+-rw-r--r--   0        0        0     1276 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/env_util.py
+-rw-r--r--   0        0        0     6740 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/formatting_util.py
+-rw-r--r--   0        0        0     3925 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/join_utils.py
+-rw-r--r--   0        0        0     4198 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/model_util.py
+-rw-r--r--   0        0        0      815 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/path_util.py
+-rw-r--r--   0        0        0     1062 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/progress.py
+-rw-r--r--   0        0        0      451 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/singleton.py
+-rw-r--r--   0        0        0     2666 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/typing.py
+-rw-r--r--   0        0        0    10491 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/utils.py
+-rw-r--r--   0        0        0     5180 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/common/validator.py
+-rw-r--r--   0        0        0    13483 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/config.py
+-rw-r--r--   0        0        0     1366 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/conftest.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/accessor/__init__.py
+-rw-r--r--   0        0        0    15533 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/accessor/count_dict.py
+-rw-r--r--   0        0        0    23735 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/accessor/datetime.py
+-rw-r--r--   0        0        0    10075 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/accessor/feature_datetime.py
+-rw-r--r--   0        0        0     8510 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/accessor/feature_string.py
+-rw-r--r--   0        0        0    15765 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/accessor/string.py
+-rw-r--r--   0        0        0     9213 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/accessor/target_datetime.py
+-rw-r--r--   0        0        0     8168 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/accessor/target_string.py
+-rw-r--r--   0        0        0     8902 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/frame.py
+-rw-r--r--   0        0        0    11818 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/generic.py
+-rw-r--r--   0        0        0    16742 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/mixin.py
+-rw-r--r--   0        0        0    38755 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/series.py
+-rw-r--r--   0        0        0     1484 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/timedelta.py
+-rw-r--r--   0        0        0     6393 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/core/util.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/datasets/__init__.py
+-rw-r--r--   0        0        0      697 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/datasets/__main__.py
+-rw-r--r--   0        0        0     5546 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/datasets/app.py
+-rw-r--r--   0        0        0     3125 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/datasets/creditcard.sql
+-rw-r--r--   0        0        0     1154 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/datasets/doctest_grocery.sql
+-rw-r--r--   0        0        0     2200 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/datasets/grocery.sql
+-rw-r--r--   0        0        0     5757 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/datasets/healthcare.sql
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/docker/__init__.py
+-rw-r--r--   0        0        0     4650 2023-08-07 07:54:30.267673 featurebyte-0.4.2/featurebyte/docker/featurebyte.yml
+-rw-r--r--   0        0        0    11444 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/docker/manager.py
+-rw-r--r--   0        0        0    10597 2023-08-07 07:53:48.503413 featurebyte-0.4.2/featurebyte/enum.py
+-rw-r--r--   0        0        0     9387 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/exception.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/feature_manager/__init__.py
+-rw-r--r--   0        0        0     2065 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/feature_manager/model.py
+-rw-r--r--   0        0        0      785 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/feature_manager/sql_template.py
+-rw-r--r--   0        0        0     3677 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/feature_utility.py
+-rw-r--r--   0        0        0     4145 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/logging.py
+-rw-r--r--   0        0        0     8053 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/middleware.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/migration/__init__.py
+-rw-r--r--   0        0        0      604 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/migration/migration_data_service.py
+-rw-r--r--   0        0        0     1703 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/migration/model.py
+-rw-r--r--   0        0        0     9020 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/migration/run.py
+-rw-r--r--   0        0        0     1442 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/migration/service/__init__.py
+-rw-r--r--   0        0        0    10260 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/migration/service/data_warehouse.py
+-rw-r--r--   0        0        0     7689 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/migration/service/mixin.py
+-rw-r--r--   0        0        0      694 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/__init__.py
+-rw-r--r--   0        0        0    11865 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/base.py
+-rw-r--r--   0        0        0      392 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/base_feature_or_target_table.py
+-rw-r--r--   0        0        0      617 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/batch_feature_table.py
+-rw-r--r--   0        0        0     1726 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/batch_request_table.py
+-rw-r--r--   0        0        0     2377 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/catalog.py
+-rw-r--r--   0        0        0     1611 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/context.py
+-rw-r--r--   0        0        0    10169 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/credential.py
+-rw-r--r--   0        0        0     1333 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/deployment.py
+-rw-r--r--   0        0        0     2026 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/dimension_table.py
+-rw-r--r--   0        0        0     3618 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/entity.py
+-rw-r--r--   0        0        0     3051 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/entity_validation.py
+-rw-r--r--   0        0        0     3551 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/event_table.py
+-rw-r--r--   0        0        0    11876 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/feature.py
+-rw-r--r--   0        0        0     3750 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0    22006 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/feature_list.py
+-rw-r--r--   0        0        0     4704 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/feature_namespace.py
+-rw-r--r--   0        0        0     7622 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/feature_store.py
+-rw-r--r--   0        0        0      659 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/historical_feature_table.py
+-rw-r--r--   0        0        0     2919 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/item_table.py
+-rw-r--r--   0        0        0     1620 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/materialized_table.py
+-rw-r--r--   0        0        0     3664 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/observation_table.py
+-rw-r--r--   0        0        0     3861 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/online_store.py
+-rw-r--r--   0        0        0     1845 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/online_store_compute_query.py
+-rw-r--r--   0        0        0     1295 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/online_store_table_version.py
+-rw-r--r--   0        0        0     1433 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/parent_serving.py
+-rw-r--r--   0        0        0     2891 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/periodic_task.py
+-rw-r--r--   0        0        0     1492 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/persistent.py
+-rw-r--r--   0        0        0     1024 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/proxy_table.py
+-rw-r--r--   0        0        0     4330 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/relationship.py
+-rw-r--r--   0        0        0      944 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/relationship_analysis.py
+-rw-r--r--   0        0        0     8719 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/request_input.py
+-rw-r--r--   0        0        0     3554 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/scd_table.py
+-rw-r--r--   0        0        0     1435 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/semantic.py
+-rw-r--r--   0        0        0     1428 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/static_source_table.py
+-rw-r--r--   0        0        0     2834 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/target.py
+-rw-r--r--   0        0        0     2107 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/target_namespace.py
+-rw-r--r--   0        0        0      595 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/target_table.py
+-rw-r--r--   0        0        0     1085 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/task.py
+-rw-r--r--   0        0        0     4041 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/tile.py
+-rw-r--r--   0        0        0     1259 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/tile_job_log.py
+-rw-r--r--   0        0        0     2968 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/tile_registry.py
+-rw-r--r--   0        0        0    10462 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/models/user_defined_function.py
+-rw-r--r--   0        0        0      154 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/persistent/__init__.py
+-rw-r--r--   0        0        0     9544 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/persistent/audit.py
+-rw-r--r--   0        0        0    22972 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/persistent/base.py
+-rw-r--r--   0        0        0     9824 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/persistent/mongo.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/query_graph/__init__.py
+-rw-r--r--   0        0        0     2533 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/query_graph/algorithm.py
+-rw-r--r--   0        0        0     3139 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/query_graph/enum.py
+-rw-r--r--   0        0        0    19750 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/query_graph/graph.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/query_graph/graph_node/__init__.py
+-rw-r--r--   0        0        0     4592 2023-08-07 07:53:48.507413 featurebyte-0.4.2/featurebyte/query_graph/graph_node/base.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/model/__init__.py
+-rw-r--r--   0        0        0      873 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/model/column_info.py
+-rw-r--r--   0        0        0    12700 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/model/common_table.py
+-rw-r--r--   0        0        0     1707 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/model/critical_data_info.py
+-rw-r--r--   0        0        0     6699 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/model/feature_job_setting.py
+-rw-r--r--   0        0        0    19287 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/model/graph.py
+-rw-r--r--   0        0        0    23872 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/model/table.py
+-rw-r--r--   0        0        0     1076 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/__init__.py
+-rw-r--r--   0        0        0     5236 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/agg_func.py
+-rw-r--r--   0        0        0    28314 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/base.py
+-rw-r--r--   0        0        0     5172 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/binary.py
+-rw-r--r--   0        0        0    17953 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/cleaning_operation.py
+-rw-r--r--   0        0        0     7797 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/count_dict.py
+-rw-r--r--   0        0        0     7293 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/date.py
+-rw-r--r--   0        0        0    10182 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/function.py
+-rw-r--r--   0        0        0    64663 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/generic.py
+-rw-r--r--   0        0        0    17083 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/input.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/metadata/__init__.py
+-rw-r--r--   0        0        0      873 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/metadata/column.py
+-rw-r--r--   0        0        0    22923 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/metadata/operation.py
+-rw-r--r--   0        0        0    20687 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/metadata/sdk_code.py
+-rw-r--r--   0        0        0       47 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/metadata/templates/sdk_code.tpl
+-rw-r--r--   0        0        0     7503 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/mixin.py
+-rw-r--r--   0        0        0    21084 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/nested.py
+-rw-r--r--   0        0        0     3272 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/request.py
+-rw-r--r--   0        0        0     2054 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/scalar.py
+-rw-r--r--   0        0        0     6696 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/schema.py
+-rw-r--r--   0        0        0     5461 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/string.py
+-rw-r--r--   0        0        0     4824 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/unary.py
+-rw-r--r--   0        0        0     1042 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/node/validator.py
+-rw-r--r--   0        0        0     1050 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/pruning_util.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/__init__.py
+-rw-r--r--   0        0        0     1060 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/adapter/__init__.py
+-rw-r--r--   0        0        0    18300 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/adapter/base.py
+-rw-r--r--   0        0        0     7716 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/adapter/databricks.py
+-rw-r--r--   0        0        0    10999 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/adapter/snowflake.py
+-rw-r--r--   0        0        0     1738 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/adapter/spark.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/__init__.py
+-rw-r--r--   0        0        0     7198 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/asat.py
+-rw-r--r--   0        0        0    22320 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/base.py
+-rw-r--r--   0        0        0    11493 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/base_lookup.py
+-rw-r--r--   0        0        0     6446 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/forward.py
+-rw-r--r--   0        0        0     5739 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/item.py
+-rw-r--r--   0        0        0     3801 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/latest.py
+-rw-r--r--   0        0        0      916 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/lookup.py
+-rw-r--r--   0        0        0     1186 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/lookup_target.py
+-rw-r--r--   0        0        0     3811 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/request_table.py
+-rw-r--r--   0        0        0    26795 2023-08-07 07:53:48.511413 featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/window.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/__init__.py
+-rw-r--r--   0        0        0     7041 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/aggregate.py
+-rw-r--r--   0        0        0    12647 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/base.py
+-rw-r--r--   0        0        0     2723 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/binary.py
+-rw-r--r--   0        0        0     5740 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/count_dict.py
+-rw-r--r--   0        0        0    10402 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/datetime.py
+-rw-r--r--   0        0        0     1907 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/function.py
+-rw-r--r--   0        0        0     7163 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/generic.py
+-rw-r--r--   0        0        0     2409 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/groupby.py
+-rw-r--r--   0        0        0     2593 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/input.py
+-rw-r--r--   0        0        0     1449 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/is_in.py
+-rw-r--r--   0        0        0     6208 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/join.py
+-rw-r--r--   0        0        0     6138 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/join_feature.py
+-rw-r--r--   0        0        0     2291 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/literal.py
+-rw-r--r--   0        0        0      878 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/request.py
+-rw-r--r--   0        0        0     8251 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/string.py
+-rw-r--r--   0        0        0    11756 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/tile.py
+-rw-r--r--   0        0        0     5170 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/track_changes.py
+-rw-r--r--   0        0        0     5157 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/unary.py
+-rw-r--r--   0        0        0     2536 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/ast/util.py
+-rw-r--r--   0        0        0     7070 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/builder.py
+-rw-r--r--   0        0        0     4909 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/common.py
+-rw-r--r--   0        0        0     1704 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/dataframe.py
+-rw-r--r--   0        0        0     1865 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/expression.py
+-rw-r--r--   0        0        0    22198 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/feature_compute.py
+-rw-r--r--   0        0        0    20358 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/feature_historical.py
+-rw-r--r--   0        0        0     4642 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/feature_preview.py
+-rw-r--r--   0        0        0     4449 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/groupby_helper.py
+-rw-r--r--   0        0        0      426 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/interpreter/__init__.py
+-rw-r--r--   0        0        0     3512 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/interpreter/base.py
+-rw-r--r--   0        0        0    27742 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/interpreter/preview.py
+-rw-r--r--   0        0        0     6685 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/interpreter/tile.py
+-rw-r--r--   0        0        0     4027 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/materialisation.py
+-rw-r--r--   0        0        0     9430 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/online_serving.py
+-rw-r--r--   0        0        0     1305 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/online_serving_util.py
+-rw-r--r--   0        0        0    10730 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/online_store_compute_query.py
+-rw-r--r--   0        0        0     5832 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/parent_serving.py
+-rw-r--r--   0        0        0    16551 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/scd_helper.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/specifications/__init__.py
+-rw-r--r--   0        0        0     2638 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/specifications/base_lookup.py
+-rw-r--r--   0        0        0     1619 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/specifications/lookup.py
+-rw-r--r--   0        0        0     1748 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/specifications/lookup_target.py
+-rw-r--r--   0        0        0    21504 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/specs.py
+-rw-r--r--   0        0        0     2206 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/template.py
+-rw-r--r--   0        0        0    12508 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/tile_compute.py
+-rw-r--r--   0        0        0     8103 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/tile_util.py
+-rw-r--r--   0        0        0     9354 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/sql/tiling.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/transform/__init__.py
+-rw-r--r--   0        0        0     5464 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/transform/base.py
+-rw-r--r--   0        0        0     2520 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/transform/entity_extractor.py
+-rw-r--r--   0        0        0     4925 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/transform/flattening.py
+-rw-r--r--   0        0        0     6715 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/transform/operation_structure.py
+-rw-r--r--   0        0        0    19339 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/transform/pruning.py
+-rw-r--r--   0        0        0     3225 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/transform/quick_pruning.py
+-rw-r--r--   0        0        0    10147 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/transform/reconstruction.py
+-rw-r--r--   0        0        0    13262 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/transform/sdk_code.py
+-rw-r--r--   0        0        0     5951 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/query_graph/util.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.515413 featurebyte-0.4.2/featurebyte/routes/__init__.py
+-rw-r--r--   0        0        0     9852 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/app_container_config.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/batch_feature_table/__init__.py
+-rw-r--r--   0        0        0     5506 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/batch_feature_table/api.py
+-rw-r--r--   0        0        0     5197 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/batch_feature_table/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/batch_request_table/__init__.py
+-rw-r--r--   0        0        0     5534 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/batch_request_table/api.py
+-rw-r--r--   0        0        0     3753 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/batch_request_table/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/catalog/__init__.py
+-rw-r--r--   0        0        0     4855 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/catalog/api.py
+-rw-r--r--   0        0        0     1374 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/catalog/catalog_name_injector.py
+-rw-r--r--   0        0        0     2429 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/catalog/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/common/__init__.py
+-rw-r--r--   0        0        0    11843 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/common/base.py
+-rw-r--r--   0        0        0     4141 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/common/base_materialized_table.py
+-rw-r--r--   0        0        0     5390 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/common/base_table.py
+-rw-r--r--   0        0        0     4900 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/common/feature_metadata_extractor.py
+-rw-r--r--   0        0        0     1861 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/common/feature_or_target_helper.py
+-rw-r--r--   0        0        0     8746 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/common/feature_or_target_table.py
+-rw-r--r--   0        0        0      886 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/common/schema.py
+-rw-r--r--   0        0        0      400 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/common/util.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/context/__init__.py
+-rw-r--r--   0        0        0     3655 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/context/api.py
+-rw-r--r--   0        0        0     1596 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/context/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/credential/__init__.py
+-rw-r--r--   0        0        0     5141 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/credential/api.py
+-rw-r--r--   0        0        0     3766 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/credential/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/deployment/__init__.py
+-rw-r--r--   0        0        0     6193 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/deployment/api.py
+-rw-r--r--   0        0        0    11712 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/deployment/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/dimension_table/__init__.py
+-rw-r--r--   0        0        0     4814 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/dimension_table/api.py
+-rw-r--r--   0        0        0     2670 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/dimension_table/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/entity/__init__.py
+-rw-r--r--   0        0        0     4769 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/entity/api.py
+-rw-r--r--   0        0        0     2949 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/entity/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/event_table/__init__.py
+-rw-r--r--   0        0        0     5278 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/event_table/api.py
+-rw-r--r--   0        0        0     2901 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/event_table/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature/__init__.py
+-rw-r--r--   0        0        0     6905 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature/api.py
+-rw-r--r--   0        0        0    22334 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_job_setting_analysis/__init__.py
+-rw-r--r--   0        0        0     6253 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_job_setting_analysis/api.py
+-rw-r--r--   0        0        0     6016 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_job_setting_analysis/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_list/__init__.py
+-rw-r--r--   0        0        0     8251 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_list/api.py
+-rw-r--r--   0        0        0    16099 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_list/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_list_namespace/__init__.py
+-rw-r--r--   0        0        0     5061 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_list_namespace/api.py
+-rw-r--r--   0        0        0     7212 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_list_namespace/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_namespace/__init__.py
+-rw-r--r--   0        0        0     4639 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_namespace/api.py
+-rw-r--r--   0        0        0    10810 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_namespace/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_store/__init__.py
+-rw-r--r--   0        0        0     8551 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_store/api.py
+-rw-r--r--   0        0        0    12839 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/feature_store/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/historical_feature_table/__init__.py
+-rw-r--r--   0        0        0     6028 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/historical_feature_table/api.py
+-rw-r--r--   0        0        0     3963 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/historical_feature_table/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/item_table/__init__.py
+-rw-r--r--   0        0        0     4410 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/item_table/api.py
+-rw-r--r--   0        0        0     2833 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/item_table/controller.py
+-rw-r--r--   0        0        0     5888 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/lazy_app_container.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/observation_table/__init__.py
+-rw-r--r--   0        0        0     5423 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/observation_table/api.py
+-rw-r--r--   0        0        0     3589 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/observation_table/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/periodic_tasks/__init__.py
+-rw-r--r--   0        0        0     2179 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/periodic_tasks/api.py
+-rw-r--r--   0        0        0      540 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/periodic_tasks/controller.py
+-rw-r--r--   0        0        0    16803 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/registry.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/relationship_info/__init__.py
+-rw-r--r--   0        0        0     4348 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/relationship_info/api.py
+-rw-r--r--   0        0        0     5644 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/relationship_info/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/scd_table/__init__.py
+-rw-r--r--   0        0        0     4335 2023-08-07 07:53:48.519413 featurebyte-0.4.2/featurebyte/routes/scd_table/api.py
+-rw-r--r--   0        0        0     3146 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/scd_table/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/semantic/__init__.py
+-rw-r--r--   0        0        0     4292 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/semantic/api.py
+-rw-r--r--   0        0        0     1380 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/semantic/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/static_source_table/__init__.py
+-rw-r--r--   0        0        0     5536 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/static_source_table/api.py
+-rw-r--r--   0        0        0     3664 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/static_source_table/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/table/__init__.py
+-rw-r--r--   0        0        0     1469 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/table/api.py
+-rw-r--r--   0        0        0      464 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/table/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/target/__init__.py
+-rw-r--r--   0        0        0     4554 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/target/api.py
+-rw-r--r--   0        0        0     6194 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/target/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/target_namespace/__init__.py
+-rw-r--r--   0        0        0     5024 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/target_namespace/api.py
+-rw-r--r--   0        0        0     1825 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/target_namespace/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/target_table/__init__.py
+-rw-r--r--   0        0        0     5186 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/target_table/api.py
+-rw-r--r--   0        0        0     3142 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/target_table/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/task/__init__.py
+-rw-r--r--   0        0        0     1045 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/task/api.py
+-rw-r--r--   0        0        0     1892 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/task/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/temp_data/__init__.py
+-rw-r--r--   0        0        0      582 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/temp_data/api.py
+-rw-r--r--   0        0        0     1353 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/temp_data/controller.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/user_defined_function/__init__.py
+-rw-r--r--   0        0        0     5845 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/user_defined_function/api.py
+-rw-r--r--   0        0        0    10715 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/routes/user_defined_function/controller.py
+-rw-r--r--   0        0        0      180 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/__init__.py
+-rw-r--r--   0        0        0     1431 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/batch_feature_table.py
+-rw-r--r--   0        0        0      842 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/batch_request_table.py
+-rw-r--r--   0        0        0     1517 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/catalog.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/common/__init__.py
+-rw-r--r--   0        0        0     1226 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/common/base.py
+-rw-r--r--   0        0        0      643 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/common/feature_or_target.py
+-rw-r--r--   0        0        0     3662 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/common/operation.py
+-rw-r--r--   0        0        0     1508 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/context.py
+-rw-r--r--   0        0        0     3658 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/credential.py
+-rw-r--r--   0        0        0     1686 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/deployment.py
+-rw-r--r--   0        0        0      981 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/dimension_table.py
+-rw-r--r--   0        0        0     1684 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/entity.py
+-rw-r--r--   0        0        0     2391 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/event_table.py
+-rw-r--r--   0        0        0     6127 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/feature.py
+-rw-r--r--   0        0        0     4664 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0     4836 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/feature_list.py
+-rw-r--r--   0        0        0     1470 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/feature_list_namespace.py
+-rw-r--r--   0        0        0     2062 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/feature_namespace.py
+-rw-r--r--   0        0        0     3589 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/feature_store.py
+-rw-r--r--   0        0        0     1410 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/historical_feature_table.py
+-rw-r--r--   0        0        0    11647 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/info.py
+-rw-r--r--   0        0        0      991 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/item_table.py
+-rw-r--r--   0        0        0      599 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/materialized_table.py
+-rw-r--r--   0        0        0      909 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/observation_table.py
+-rw-r--r--   0        0        0      459 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/periodic_task.py
+-rw-r--r--   0        0        0      478 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/preview.py
+-rw-r--r--   0        0        0     1460 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/relationship_info.py
+-rw-r--r--   0        0        0     1190 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/request_table.py
+-rw-r--r--   0        0        0     1376 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/scd_table.py
+-rw-r--r--   0        0        0      914 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/semantic.py
+-rw-r--r--   0        0        0     1152 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/static_source_table.py
+-rw-r--r--   0        0        0     2415 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/table.py
+-rw-r--r--   0        0        0     2725 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/target.py
+-rw-r--r--   0        0        0     1852 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/target_namespace.py
+-rw-r--r--   0        0        0     1788 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/target_table.py
+-rw-r--r--   0        0        0     1012 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/task.py
+-rw-r--r--   0        0        0     1916 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/user_defined_function.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/__init__.py
+-rw-r--r--   0        0        0      333 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/progress.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/__init__.py
+-rw-r--r--   0        0        0     2829 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/base.py
+-rw-r--r--   0        0        0      739 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/batch_feature_create.py
+-rw-r--r--   0        0        0      610 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/batch_feature_table.py
+-rw-r--r--   0        0        0      602 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/batch_request_table.py
+-rw-r--r--   0        0        0     1382 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/deployment_create_update.py
+-rw-r--r--   0        0        0     1328 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0      677 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/feature_list_batch_feature_create.py
+-rw-r--r--   0        0        0      725 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/historical_feature_table.py
+-rw-r--r--   0        0        0     1459 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/materialized_table_delete.py
+-rw-r--r--   0        0        0      589 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/observation_table.py
+-rw-r--r--   0        0        0      602 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/static_source_table.py
+-rw-r--r--   0        0        0      591 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/target_table.py
+-rw-r--r--   0        0        0      544 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/test.py
+-rw-r--r--   0        0        0      459 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/schema/worker/task/tile.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/service/__init__.py
+-rw-r--r--   0        0        0    34638 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/service/base_document.py
+-rw-r--r--   0        0        0     1090 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/service/base_namespace_service.py
+-rw-r--r--   0        0        0     5215 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/service/base_table_document.py
+-rw-r--r--   0        0        0     1929 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/service/batch_feature_table.py
+-rw-r--r--   0        0        0     2831 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/service/batch_request_table.py
+-rw-r--r--   0        0        0      596 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/service/catalog.py
+-rw-r--r--   0        0        0     5638 2023-08-07 07:53:48.523414 featurebyte-0.4.2/featurebyte/service/context.py
+-rw-r--r--   0        0        0     5665 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/credential.py
+-rw-r--r--   0        0        0     4606 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/default_version_mode.py
+-rw-r--r--   0        0        0    18089 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/deploy.py
+-rw-r--r--   0        0        0      653 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/deployment.py
+-rw-r--r--   0        0        0      674 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/dimension_table.py
+-rw-r--r--   0        0        0     4246 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/entity.py
+-rw-r--r--   0        0        0     7231 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/entity_validation.py
+-rw-r--r--   0        0        0      618 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/event_table.py
+-rw-r--r--   0        0        0     6732 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/feature.py
+-rw-r--r--   0        0        0     3742 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0    16639 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/feature_list.py
+-rw-r--r--   0        0        0     4268 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/feature_list_namespace.py
+-rw-r--r--   0        0        0     4251 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/feature_list_status.py
+-rw-r--r--   0        0        0    12724 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/feature_manager.py
+-rw-r--r--   0        0        0      574 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/feature_namespace.py
+-rw-r--r--   0        0        0    12595 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/feature_preview.py
+-rw-r--r--   0        0        0    15619 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/feature_readiness.py
+-rw-r--r--   0        0        0     1468 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/feature_store.py
+-rw-r--r--   0        0        0     8851 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/feature_store_warehouse.py
+-rw-r--r--   0        0        0     3392 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/historical_feature_table.py
+-rw-r--r--   0        0        0    14351 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/historical_features.py
+-rw-r--r--   0        0        0      604 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/item_table.py
+-rw-r--r--   0        0        0     4808 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/materialized_table.py
+-rw-r--r--   0        0        0     4446 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/mixin.py
+-rw-r--r--   0        0        0     5383 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/namespace_handler.py
+-rw-r--r--   0        0        0     6290 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/observation_table.py
+-rw-r--r--   0        0        0     9227 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/online_enable.py
+-rw-r--r--   0        0        0     4540 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/online_serving.py
+-rw-r--r--   0        0        0     2637 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/online_store_compute_query_service.py
+-rw-r--r--   0        0        0     3016 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/online_store_table_version.py
+-rw-r--r--   0        0        0     7009 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/parent_serving.py
+-rw-r--r--   0        0        0      437 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/periodic_task.py
+-rw-r--r--   0        0        0    10079 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/preview.py
+-rw-r--r--   0        0        0     9258 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/relationship.py
+-rw-r--r--   0        0        0     2311 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/relationship_info.py
+-rw-r--r--   0        0        0      991 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/sanitizer.py
+-rw-r--r--   0        0        0      590 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/scd_table.py
+-rw-r--r--   0        0        0      600 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/semantic.py
+-rw-r--r--   0        0        0     2830 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/session_manager.py
+-rw-r--r--   0        0        0     6617 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/session_validator.py
+-rw-r--r--   0        0        0     2930 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/static_source_table.py
+-rw-r--r--   0        0        0     1051 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/table.py
+-rw-r--r--   0        0        0    16479 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/table_columns_info.py
+-rw-r--r--   0        0        0     3275 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/table_info.py
+-rw-r--r--   0        0        0     2081 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/table_status.py
+-rw-r--r--   0        0        0     6967 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/target.py
+-rw-r--r--   0        0        0     6520 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/target_helper/base_feature_or_target_computer.py
+-rw-r--r--   0        0        0     5195 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/target_helper/compute_target.py
+-rw-r--r--   0        0        0      535 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/target_namespace.py
+-rw-r--r--   0        0        0     3085 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/target_table.py
+-rw-r--r--   0        0        0     9795 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/task_manager.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/tile/__init__.py
+-rw-r--r--   0        0        0    11222 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/tile/tile_task_executor.py
+-rw-r--r--   0        0        0     2362 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/tile_cache.py
+-rw-r--r--   0        0        0     7045 2023-08-07 07:53:48.527413 featurebyte-0.4.2/featurebyte/service/tile_job_log.py
+-rw-r--r--   0        0        0    14700 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/service/tile_manager.py
+-rw-r--r--   0        0        0     2681 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/service/tile_registry_service.py
+-rw-r--r--   0        0        0     2519 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/service/tile_scheduler.py
+-rw-r--r--   0        0        0     2662 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/service/user_defined_function.py
+-rw-r--r--   0        0        0      709 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/service/user_service.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/service/validator/__init__.py
+-rw-r--r--   0        0        0     6291 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/service/validator/materialized_table_delete.py
+-rw-r--r--   0        0        0    11655 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/service/validator/production_ready_validator.py
+-rw-r--r--   0        0        0    15448 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/service/version.py
+-rw-r--r--   0        0        0    13077 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/service/view_construction.py
+-rw-r--r--   0        0        0     4591 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/service/working_schema.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/__init__.py
+-rw-r--r--   0        0        0    29242 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/base.py
+-rw-r--r--   0        0        0    16356 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/base_spark.py
+-rw-r--r--   0        0        0     5643 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/databricks.py
+-rw-r--r--   0        0        0      434 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/enum.py
+-rw-r--r--   0        0        0     4993 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/hive.py
+-rw-r--r--   0        0        0     5107 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/manager.py
+-rw-r--r--   0        0        0     9179 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/simple_storage.py
+-rw-r--r--   0        0        0    13216 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/snowflake.py
+-rw-r--r--   0        0        0    11998 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/spark.py
+-rw-r--r--   0        0        0     3479 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/sqlite.py
+-rw-r--r--   0        0        0     6615 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/session/webhdfs.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/__init__.py
+-rw-r--r--   0        0        0     2569 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/base.py
+-rw-r--r--   0        0        0     2743 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/common.py
+-rw-r--r--   0        0        0        6 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/databricks/.gitignore
+-rw-r--r--   0        0        0      957 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql
+-rw-r--r--   0        0        0      476 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/F_COUNT_DICT_ENTROPY.sql
+-rw-r--r--   0        0        0      171 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT.sql
+-rw-r--r--   0        0        0      610 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql
+-rw-r--r--   0        0        0      177 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_VALUE.sql
+-rw-r--r--   0        0        0      188 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/F_COUNT_DICT_NUM_UNIQUE.sql
+-rw-r--r--   0        0        0     1491 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/F_GET_RANK.sql
+-rw-r--r--   0        0        0      449 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/F_GET_RELATIVE_FREQUENCY.sql
+-rw-r--r--   0        0        0      559 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql
+-rw-r--r--   0        0        0      559 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql
+-rw-r--r--   0        0        0      653 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql
+-rw-r--r--   0        0        0      153 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/snowflake/T_TILE_MONITOR_SUMMARY.sql
+-rw-r--r--   0        0        0        6 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/spark/.gitignore
+-rw-r--r--   0        0        0      191 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/spark/T_TILE_MONITOR_SUMMARY.sql
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/spark/__init__.py
+-rw-r--r--   0        0        0    29714 2023-08-07 07:55:53.852129 featurebyte-0.4.2/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar
+-rw-r--r--   0        0        0     1923 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/tile_common.py
+-rw-r--r--   0        0        0     5635 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/tile_generate.py
+-rw-r--r--   0        0        0     3564 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/tile_generate_entity_tracking.py
+-rw-r--r--   0        0        0     8611 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/tile_monitor.py
+-rw-r--r--   0        0        0     2833 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/tile_registry.py
+-rw-r--r--   0        0        0     6829 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/sql/tile_schedule_online_store.py
+-rw-r--r--   0        0        0      297 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/storage/__init__.py
+-rw-r--r--   0        0        0     4999 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/storage/base.py
+-rw-r--r--   0        0        0     3640 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/storage/local.py
+-rw-r--r--   0        0        0      415 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/storage/local_temp.py
+-rw-r--r--   0        0        0     5575 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/storage/s3.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/tile/__init__.py
+-rw-r--r--   0        0        0      411 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/tile/sql_template.py
+-rw-r--r--   0        0        0    26885 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/tile/tile_cache.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/utils/__init__.py
+-rw-r--r--   0        0        0     1909 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/utils/credential.py
+-rw-r--r--   0        0        0     1532 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/utils/messaging.py
+-rw-r--r--   0        0        0      534 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/utils/persistent.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/utils/snowflake/__init__.py
+-rw-r--r--   0        0        0      462 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/utils/snowflake/sql.py
+-rw-r--r--   0        0        0     2225 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/utils/storage.py
+-rw-r--r--   0        0        0     1990 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/worker/__init__.py
+-rw-r--r--   0        0        0      170 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/worker/enum.py
+-rw-r--r--   0        0        0     1159 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/worker/progress.py
+-rw-r--r--   0        0        0     2502 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/worker/schedulers.py
+-rw-r--r--   0        0        0      230 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/worker/start.py
+-rw-r--r--   0        0        0      214 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/worker/task/__init__.py
+-rw-r--r--   0        0        0     2926 2023-08-07 07:53:48.531414 featurebyte-0.4.2/featurebyte/worker/task/base.py
+-rw-r--r--   0        0        0    11492 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/batch_feature_create.py
+-rw-r--r--   0        0        0     3718 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/batch_feature_table.py
+-rw-r--r--   0        0        0     2243 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/batch_request_table.py
+-rw-r--r--   0        0        0     1795 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/deployment_create_update.py
+-rw-r--r--   0        0        0     6763 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0     1463 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/feature_list_batch_feature_create.py
+-rw-r--r--   0        0        0     3502 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/historical_feature_table.py
+-rw-r--r--   0        0        0     5405 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/materialized_table_delete.py
+-rw-r--r--   0        0        0     2604 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/mixin.py
+-rw-r--r--   0        0        0     2226 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/observation_table.py
+-rw-r--r--   0        0        0     2197 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/static_source_table.py
+-rw-r--r--   0        0        0     3327 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/target_table.py
+-rw-r--r--   0        0        0      626 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/test_task.py
+-rw-r--r--   0        0        0     1541 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task/tile_task.py
+-rw-r--r--   0        0        0     6279 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/task_executor.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/util/__init__.py
+-rw-r--r--   0        0        0     1773 2023-08-07 07:53:48.535414 featurebyte-0.4.2/featurebyte/worker/util/observation_set_helper.py
+-rw-r--r--   0        0        0     7915 2023-08-07 07:54:28.547670 featurebyte-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    23156 1970-01-01 00:00:00.000000 featurebyte-0.4.2/PKG-INFO
```

### Comparing `featurebyte-0.4.1/LICENSE` & `featurebyte-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/README.md` & `featurebyte-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/__init__.py` & `featurebyte-0.4.2/featurebyte/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/__main__.py` & `featurebyte-0.4.2/featurebyte/__main__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/aggregator/base_aggregator.py` & `featurebyte-0.4.2/featurebyte/api/aggregator/base_aggregator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 This module contains base aggregator related class
 """
 from __future__ import annotations
 
-from typing import List, Optional, Type
+from typing import List, Optional, Type, Union
 
 from abc import ABC, abstractmethod
 
+from featurebyte import Target
 from featurebyte.api.feature import Feature
 from featurebyte.api.view import View
 from featurebyte.common.typing import OptionalScalar, get_or_default
 from featurebyte.enum import AggFunc, DBVarType
 from featurebyte.exception import AggregationNotSupportedForViewError
 from featurebyte.models.base import PydanticObjectId
 from featurebyte.query_graph.node import Node
@@ -139,41 +140,41 @@
         value_column: Optional[str],
         fill_value: OptionalScalar,
         skip_fill_na: bool,
     ) -> Feature:
         # value_column is None for count-like aggregation method
         var_type = self.get_output_var_type(agg_method, method, value_column)  # type: ignore[arg-type]
 
-        feature = self.view._project_feature_from_node(  # pylint: disable=protected-access
+        feature = self.view.project_feature_from_node(
             node=groupby_node,
             feature_name=feature_name,
             feature_dtype=var_type,
         )
         if not skip_fill_na:
-            self._fill_feature(feature, method, feature_name, fill_value)
+            self._fill_feature_or_target(feature, method, feature_name, fill_value)
         return feature
 
-    def _fill_feature(
+    def _fill_feature_or_target(
         self,
-        feature: Feature,
+        feature_or_target: Union[Feature, Target],
         method: str,
-        feature_name: str,
+        feature_or_target_name: str,
         fill_value: OptionalScalar,
-    ) -> Feature:
+    ) -> Union[Feature, Target]:
         """
-        Fill feature values as needed.
+        Fill feature or target values as needed.
 
         Parameters
         ----------
-        feature: Feature
-            feature
+        feature_or_target: Union[Feature, Target]
+            feature or target
         method: str
             aggregation method
-        feature_name: str
-            feature name
+        feature_or_target_name: str
+            feature or target name
         fill_value: OptionalScalar
             value to fill
 
         Returns
         -------
         Feature
 
@@ -184,14 +185,14 @@
         """
         if fill_value is not None and self.category is not None:
             raise ValueError("fill_value is not supported for aggregation per category")
 
         if method in {AggFunc.COUNT, AggFunc.NA_COUNT} and self.category is None:
             # Count features should be 0 instead of NaN when there are no records
             value_to_fill = get_or_default(fill_value, 0)
-            feature.fillna(value_to_fill)
-            feature.name = feature_name
+            feature_or_target.fillna(value_to_fill)
+            feature_or_target.name = feature_or_target_name
         elif fill_value is not None:
-            feature.fillna(fill_value)
-            feature.name = feature_name
+            feature_or_target.fillna(fill_value)
+            feature_or_target.name = feature_or_target_name
 
-        return feature
+        return feature_or_target
```

### Comparing `featurebyte-0.4.1/featurebyte/api/aggregator/forward_aggregator.py` & `featurebyte-0.4.2/featurebyte/api/aggregator/forward_aggregator.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, List, Optional, Type, cast
 
 from featurebyte import AggFunc, ChangeView, EventView, ItemView
 from featurebyte.api.aggregator.base_aggregator import BaseAggregator
 from featurebyte.api.target import Target
 from featurebyte.api.view import View
 from featurebyte.common.model_util import parse_duration_string
+from featurebyte.common.typing import OptionalScalar
 from featurebyte.query_graph.enum import NodeOutputType, NodeType
 from featurebyte.query_graph.node.agg_func import construct_agg_func
 
 
 class ForwardAggregator(BaseAggregator):
     """
     ForwardAggregator implements the forward_aggregate method for GroupBy
@@ -29,40 +30,47 @@
 
     def forward_aggregate(
         self,
         value_column: str,
         method: str,
         window: Optional[str] = None,
         target_name: Optional[str] = None,
+        fill_value: OptionalScalar = None,
+        skip_fill_na: bool = False,
     ) -> Target:
         """
         Aggregate given value_column for each group specified in keys over a time window.
 
         Parameters
         ----------
         value_column: str
             Column to be aggregated
         method: str
             Aggregation method
         window: str
             Window of the aggregation
         target_name: str
             Name of the target column
+        fill_value: OptionalScalar
+            Value to fill if the value in the column is empty
+        skip_fill_na: bool
+            Whether to skip filling NaN values
 
         Returns
         -------
         Target
         """
         # Validation
         self._validate_parameters(
             value_column=value_column,
             method=method,
             window=window,
             target_name=target_name,
         )
+        self._validate_fill_value_and_skip_fill_na(fill_value=fill_value, skip_fill_na=skip_fill_na)
         # Create new node parameters
         assert value_column is not None
         node_params = self._prepare_node_parameters(
             value_column=value_column,
             method=method,
             window=window,
             target_name=target_name,
@@ -71,33 +79,24 @@
         # Add forward aggregate node to graph.
         forward_aggregate_node = self.view.graph.add_operation(
             node_type=NodeType.FORWARD_AGGREGATE,
             node_params=node_params,
             node_output_type=NodeOutputType.FRAME,
             input_nodes=[self.view.node],
         )
-        # Project target node.
-        target_node = self.view.graph.add_operation(
-            node_type=NodeType.PROJECT,
-            node_params={"columns": [target_name]},
-            node_output_type=NodeOutputType.SERIES,
-            input_nodes=[forward_aggregate_node],
-        )
-        # Build and return Target
         agg_method = construct_agg_func(agg_func=cast(AggFunc, method))
         output_var_type = self.get_output_var_type(agg_method, method, value_column)
-        return Target(
-            name=target_name,
-            entity_ids=self.entity_ids,
-            graph=self.view.graph,
-            node_name=target_node.name,
-            tabular_source=self.view.tabular_source,
-            feature_store=self.view.feature_store,
-            dtype=output_var_type,
+        # Project, build and return Target
+        assert target_name is not None
+        target = self.view.project_target_from_node(
+            forward_aggregate_node, target_name, output_var_type
         )
+        if not skip_fill_na:
+            return self._fill_feature_or_target(target, method, target_name, fill_value)  # type: ignore[return-value]
+        return target
 
     def _prepare_node_parameters(
         self,
         value_column: str,
         method: str,
         window: Optional[str],
         target_name: Optional[str],
```

### Comparing `featurebyte-0.4.1/featurebyte/api/api_handler/base.py` & `featurebyte-0.4.2/featurebyte/api/api_handler/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 List handler
 """
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Type
 
+import json
 from functools import partial
 from itertools import groupby
 
 import pandas as pd
 from pandas import DataFrame
 
 from featurebyte.api.api_object_util import (
@@ -72,15 +73,15 @@
             Table of objects
         """
         params = params or {}
         output = []
         for item_dict in iterate_api_object_using_paginated_routes(
             route=self.route, params={"page_size": PAGINATED_CALL_PAGE_SIZE, **params}
         ):
-            output.append(self.list_schema(**item_dict).dict())
+            output.append(json.loads(self.list_schema(**item_dict).json()))
 
         fields = self.list_fields
         if include_id:
             fields = ["id"] + fields
 
         if not output:
             return DataFrame(columns=fields)
```

### Comparing `featurebyte-0.4.1/featurebyte/api/api_handler/feature.py` & `featurebyte-0.4.2/featurebyte/api/api_handler/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/api_handler/feature_job_setting_analysis.py` & `featurebyte-0.4.2/featurebyte/api/api_handler/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/api_handler/feature_list.py` & `featurebyte-0.4.2/featurebyte/api/api_handler/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/api_handler/feature_namespace.py` & `featurebyte-0.4.2/featurebyte/api/api_handler/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/api_object.py` & `featurebyte-0.4.2/featurebyte/api/api_object.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/api_object_util.py` & `featurebyte-0.4.2/featurebyte/api/api_object_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,50 +158,50 @@
         True if the code is running in server mode
     """
     sdk_execution_mode = os.environ.get("FEATUREBYTE_SDK_EXECUTION_MODE")
     return sdk_execution_mode == "SERVER"
 
 
 def map_object_id_to_name(
-    object_map: Dict[Optional[ObjectId], str], object_id: Union[ObjectId, List[ObjectId]]
+    object_map: Dict[Optional[str], str], object_id: Union[str, List[str]]
 ) -> Union[Optional[str], List[Optional[str]]]:
     """
     Map list of object ids object names
 
     Parameters
     ----------
-    object_map: Dict[Optional[ObjectId], str],
-        Dict that maps ObjectId to name
-    object_id: Union[ObjectId, List[ObjectId]]
+    object_map: Dict[Optional[str], str],
+        Dict that maps ObjectId string to name
+    object_id: Union[str, List[str]]
         List of object ids to map, or object id to map
 
     Returns
     -------
     Union[Optional[str], List[Optional[str]]]
     """
     if isinstance(object_id, list):
         return [object_map.get(_id) for _id in object_id]
     return object_map.get(object_id)
 
 
 def map_dict_list_to_name(
-    object_map: Dict[Optional[ObjectId], str],
+    object_map: Dict[Optional[str], str],
     object_id_field: str,
-    object_dict: Union[Dict[str, ObjectId], List[Dict[str, ObjectId]]],
+    object_dict: Union[Dict[str, str], List[Dict[str, str]]],
 ) -> Union[Optional[str], List[Optional[str]]]:
     """
     Map list of object dict to object names
 
     Parameters
     ----------
-    object_map: Dict[Optional[ObjectId], str],
+    object_map: Dict[Optional[str], str],
         Dict that maps ObjectId to name
     object_id_field: str
         Name of field in object dict to get object id from
-    object_dict: Union[Dict[str, ObjectId], List[Dict[str, ObjectId]]]
+    object_dict: Union[Dict[str, str], List[Dict[str, str]]]
         List of dict to map
 
     Returns
     -------
     Union[Optional[str], List[Optional[str]]]
     """
     if isinstance(object_dict, list):
```

### Comparing `featurebyte-0.4.1/featurebyte/api/asat_aggregator.py` & `featurebyte-0.4.2/featurebyte/api/asat_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/base_table.py` & `featurebyte-0.4.2/featurebyte/api/base_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/batch_feature_table.py` & `featurebyte-0.4.2/featurebyte/api/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/batch_request_table.py` & `featurebyte-0.4.2/featurebyte/api/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/catalog.py` & `featurebyte-0.4.2/featurebyte/api/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from featurebyte.api.observation_table import ObservationTable
 from featurebyte.api.periodic_task import PeriodicTask
 from featurebyte.api.relationship import Relationship
 from featurebyte.api.savable_api_object import SavableApiObject
 from featurebyte.api.static_source_table import StaticSourceTable
 from featurebyte.api.table import Table
 from featurebyte.api.target import Target
-from featurebyte.api.target_table import TargetTable
 from featurebyte.api.user_defined_function import UserDefinedFunction
 from featurebyte.api.view import View
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.exception import RecordRetrievalException
 from featurebyte.logging import get_logger
 from featurebyte.models.base import PydanticObjectId, activate_catalog, get_active_catalog_id
 from featurebyte.models.catalog import CatalogModel
@@ -850,37 +849,14 @@
         List saved user defined functions.
 
         >>> user_defined_functions = catalog.list_user_defined_functions()
         """
         return UserDefinedFunction.list(include_id=include_id)
 
     @update_and_reset_catalog
-    def list_target_tables(self, include_id: Optional[bool] = True) -> pd.DataFrame:
-        """
-        List saved target tables.
-
-        Parameters
-        ----------
-        include_id: Optional[bool]
-            Whether to include id in the list.
-
-        Returns
-        -------
-        pd.DataFrame
-            Table of target tables.
-
-        Examples
-        --------
-        List saved target tables.
-
-        >>> target_tables = catalog.list_target_tables()
-        """
-        return TargetTable.list(include_id=include_id)
-
-    @update_and_reset_catalog
     def get_data_source(self) -> DataSource:
         """
         Gets the data source from the catalog to access source tables from the data warehouse.
 
         Returns
         -------
         DataSource
@@ -1297,30 +1273,7 @@
         Examples
         --------
         Get a saved user defined function.
 
         >>> user_defined_function = catalog.get_user_defined_function("user_defined_function_name")  # doctest: +SKIP
         """
         return UserDefinedFunction.get(name=name)
-
-    @update_and_reset_catalog
-    def get_target_table(self, name: str) -> TargetTable:
-        """
-        Get target table by name.
-
-        Parameters
-        ----------
-        name: str
-            Target table name.
-
-        Returns
-        -------
-        TargetTable
-            Target table object.
-
-        Examples
-        --------
-        Get a saved target table.
-
-        >>> target_table = catalog.get_target_table("target_table_name")  # doctest: +SKIP
-        """
-        return TargetTable.get(name=name)
```

### Comparing `featurebyte-0.4.1/featurebyte/api/catalog_decorator.py` & `featurebyte-0.4.2/featurebyte/api/catalog_decorator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/catalog_get_by_id_mixin.py` & `featurebyte-0.4.2/featurebyte/api/catalog_get_by_id_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from featurebyte.api.historical_feature_table import HistoricalFeatureTable
 from featurebyte.api.observation_table import ObservationTable
 from featurebyte.api.periodic_task import PeriodicTask
 from featurebyte.api.relationship import Relationship
 from featurebyte.api.static_source_table import StaticSourceTable
 from featurebyte.api.table import Table
 from featurebyte.api.target import Target
-from featurebyte.api.target_table import TargetTable
 from featurebyte.api.user_defined_function import UserDefinedFunction
 from featurebyte.api.view import View
 
 
 class CatalogGetByIdMixin:
     """
     Mixin to add get_by_id functionality into the catalog.
@@ -481,32 +480,7 @@
         Examples
         --------
         Get a saved target .
 
         >>> target = catalog.get_target_by_id(ObjectId())  # doctest: +SKIP
         """
         return Target.get_by_id(id=id)
-
-    @update_and_reset_catalog
-    def get_target_table_by_id(
-        self, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
-    ) -> TargetTable:
-        """
-        Get target table by id.
-
-        Parameters
-        ----------
-        id: ObjectId
-            Target table id.
-
-        Returns
-        -------
-        TargetTable
-            Target table object.
-
-        Examples
-        --------
-        Get a saved target table.
-
-        >>> target_table = catalog.get_target_table_by_id(ObjectId())  # doctest: +SKIP
-        """
-        return TargetTable.get_by_id(id=id)
```

### Comparing `featurebyte-0.4.1/featurebyte/api/change_view.py` & `featurebyte-0.4.2/featurebyte/api/change_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/credential.py` & `featurebyte-0.4.2/featurebyte/api/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/data_source.py` & `featurebyte-0.4.2/featurebyte/api/data_source.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/deployment.py` & `featurebyte-0.4.2/featurebyte/api/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/dimension_table.py` & `featurebyte-0.4.2/featurebyte/api/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/dimension_view.py` & `featurebyte-0.4.2/featurebyte/api/dimension_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/entity.py` & `featurebyte-0.4.2/featurebyte/api/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/event_table.py` & `featurebyte-0.4.2/featurebyte/api/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/event_view.py` & `featurebyte-0.4.2/featurebyte/api/event_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
     def get_join_column(self) -> str:
         # This is potentially none for backwards compatibility.
         # We can remove this once DEV-556 is done.
         assert self.event_id_column is not None
         return self.event_id_column
 
-    def _get_as_feature_parameters(self, offset: Optional[str] = None) -> dict[str, Any]:
+    def get_additional_lookup_parameters(self, offset: Optional[str] = None) -> dict[str, Any]:
         _ = offset
         return {
             "event_parameters": {
                 "event_timestamp_column": self.timestamp_column,
             }
         }
```

### Comparing `featurebyte-0.4.1/featurebyte/api/feature.py` & `featurebyte-0.4.2/featurebyte/api/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,20 +49,18 @@
 from featurebyte.feature_manager.model import ExtendedFeatureModel
 from featurebyte.logging import get_logger
 from featurebyte.models.base import PydanticObjectId
 from featurebyte.models.feature import FeatureModel
 from featurebyte.models.feature_namespace import DefaultVersionMode, FeatureReadiness
 from featurebyte.models.feature_store import FeatureStoreModel
 from featurebyte.models.tile import TileSpec
-from featurebyte.query_graph.enum import NodeOutputType, NodeType
 from featurebyte.query_graph.graph import GlobalQueryGraph
 from featurebyte.query_graph.model.common_table import TabularSource
 from featurebyte.query_graph.model.feature_job_setting import TableFeatureJobSetting
 from featurebyte.query_graph.node.cleaning_operation import TableCleaningOperation
-from featurebyte.query_graph.node.generic import AliasNode, ProjectNode
 from featurebyte.schema.feature import (
     BatchFeatureCreatePayload,
     BatchFeatureItem,
     FeatureModelResponse,
     FeatureSQL,
     FeatureUpdate,
 )
@@ -411,15 +409,15 @@
         >>> feature = catalog.get_feature("InvoiceCount_60days")
         >>> feature.list_versions(include_id=False)  # doctest: +ELLIPSIS
                               name  version  dtype         readiness  online_enabled            tables    primary_tables           entities   primary_entities  created_at  is_default
             0  InvoiceCount_60days      ...  FLOAT  PRODUCTION_READY           False  [GROCERYINVOICE]  [GROCERYINVOICE]  [grocerycustomer]  [grocerycustomer]         ...        True
         """
         output = self._list(include_id=True, params={"name": self.name})
         default_feature_id = self.feature_namespace.default_feature_id
-        output["is_default"] = output["id"] == default_feature_id
+        output["is_default"] = output["id"] == str(default_feature_id)
         columns = output.columns
         if not include_id:
             columns = [column for column in columns if column != "id"]
         return output[columns]
 
     def delete(self) -> None:
         """
@@ -439,67 +437,14 @@
 
         See Also
         --------
         - [Feature.update_default_version_mode](/reference/featurebyte.api.feature.Feature.update_default_version_mode/)
         """
         self._delete()
 
-    @typechecked
-    def __setattr__(self, key: str, value: Any) -> Any:
-        """
-        Custom __setattr__ to handle setting of special attributes such as name
-
-        Parameters
-        ----------
-        key : str
-            Key
-        value : Any
-            Value
-
-        Raises
-        ------
-        ValueError
-            if the name parameter is invalid
-
-        Returns
-        -------
-        Any
-        """
-        if key != "name":
-            return super().__setattr__(key, value)
-
-        if value is None:
-            raise ValueError("None is not a valid feature name")
-
-        # For now, only allow updating name if the feature is unnamed (i.e. created on-the-fly by
-        # combining different features)
-        name = value
-        node = self.node
-        if node.type in {NodeType.PROJECT, NodeType.ALIAS}:
-            if isinstance(node, ProjectNode):
-                existing_name = node.parameters.columns[0]
-            else:
-                assert isinstance(node, AliasNode)
-                existing_name = node.parameters.name  # type: ignore
-            if name != existing_name:
-                raise ValueError(f'Feature "{existing_name}" cannot be renamed to "{name}"')
-            # FeatureGroup sets name unconditionally, so we allow this here
-            return super().__setattr__(key, value)
-
-        # Here, node could be any node resulting from series operations, e.g. DIV. This
-        # validation was triggered by setting the name attribute of a Feature object
-        new_node = self.graph.add_operation(
-            node_type=NodeType.ALIAS,
-            node_params={"name": name},
-            node_output_type=NodeOutputType.SERIES,
-            input_nodes=[node],
-        )
-        self.node_name = new_node.name
-        return super().__setattr__(key, value)
-
     @property
     def feature_namespace(self) -> FeatureNamespace:
         """
         FeatureNamespace object of current feature
 
         Returns
         -------
```

### Comparing `featurebyte-0.4.1/featurebyte/api/feature_group.py` & `featurebyte-0.4.2/featurebyte/api/feature_group.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/feature_job.py` & `featurebyte-0.4.2/featurebyte/api/feature_job.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/feature_job_setting_analysis.py` & `featurebyte-0.4.2/featurebyte/api/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/feature_list.py` & `featurebyte-0.4.2/featurebyte/api/feature_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -987,15 +987,15 @@
         >>> feature_list = catalog.get_feature_list("invoice_feature_list")
         >>> feature_list.list_versions(include_id=False)  # doctest: +ELLIPSIS
                            name  version  online_frac  deployed  created_at  is_default
         0  invoice_feature_list      ...          0.0     False         ...        True
         """
         output = self._list(include_id=True, params={"name": self.name})
         default_feature_list_id = self.feature_list_namespace.default_feature_list_id
-        output["is_default"] = output["id"] == default_feature_list_id
+        output["is_default"] = output["id"] == str(default_feature_list_id)
         exclude_cols = {"num_feature"}
         if not include_id:
             exclude_cols.add("id")
         return output[[col for col in output.columns if col not in exclude_cols]]
 
     @classmethod
     def list(
```

### Comparing `featurebyte-0.4.1/featurebyte/api/feature_namespace.py` & `featurebyte-0.4.2/featurebyte/api/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/feature_or_target_mixin.py` & `featurebyte-0.4.2/featurebyte/api/feature_or_target_mixin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """
 Mixin class containing common methods for feature or target classes
 """
-from typing import List, Sequence, cast
+from typing import Any, List, Sequence, cast
 
 import time
 from http import HTTPStatus
 
 import pandas as pd
 from bson import ObjectId
 from pydantic import Field
+from typeguard import typechecked
 
 from featurebyte.api.api_object import ApiObject
 from featurebyte.api.entity import Entity
 from featurebyte.common.formatting_util import CodeStr
 from featurebyte.common.utils import dataframe_from_json
 from featurebyte.config import Configurations
 from featurebyte.core.generic import QueryObject
 from featurebyte.exception import RecordRetrievalException
 from featurebyte.logging import get_logger
 from featurebyte.models.base import PydanticObjectId, get_active_catalog_id
 from featurebyte.models.feature import BaseFeatureModel
 from featurebyte.models.relationship_analysis import derive_primary_entity
+from featurebyte.query_graph.enum import NodeOutputType, NodeType
+from featurebyte.query_graph.node.generic import AliasNode, ProjectNode
 from featurebyte.schema.preview import FeatureOrTargetPreview
 
 logger = get_logger(__name__)
 
 
 class FeatureOrTargetMixin(QueryObject, ApiObject):
     """
@@ -105,7 +108,60 @@
             Primary entity
         """
         entities = []
         for entity_id in self._get_entity_ids():
             entities.append(Entity.get_by_id(entity_id))
         primary_entity = derive_primary_entity(entities)  # type: ignore
         return primary_entity
+
+    @typechecked
+    def __setattr__(self, key: str, value: Any) -> Any:
+        """
+        Custom __setattr__ to handle setting of special attributes such as name
+
+        Parameters
+        ----------
+        key : str
+            Key
+        value : Any
+            Value
+
+        Raises
+        ------
+        ValueError
+            if the name parameter is invalid
+
+        Returns
+        -------
+        Any
+        """
+        if key != "name":
+            return super().__setattr__(key, value)
+
+        if value is None:
+            raise ValueError("None is not a valid feature name")
+
+        # For now, only allow updating name if the feature is unnamed (i.e. created on-the-fly by
+        # combining different features)
+        name = value
+        node = self.node
+        if node.type in {NodeType.PROJECT, NodeType.ALIAS}:
+            if isinstance(node, ProjectNode):
+                existing_name = node.parameters.columns[0]
+            else:
+                assert isinstance(node, AliasNode)
+                existing_name = node.parameters.name  # type: ignore
+            if name != existing_name:
+                raise ValueError(f'Feature "{existing_name}" cannot be renamed to "{name}"')
+            # FeatureGroup sets name unconditionally, so we allow this here
+            return super().__setattr__(key, value)
+
+        # Here, node could be any node resulting from series operations, e.g. DIV. This
+        # validation was triggered by setting the name attribute of a Feature object
+        new_node = self.graph.add_operation(
+            node_type=NodeType.ALIAS,
+            node_params={"name": name},
+            node_output_type=NodeOutputType.SERIES,
+            input_nodes=[node],
+        )
+        self.node_name = new_node.name
+        return super().__setattr__(key, value)
```

### Comparing `featurebyte-0.4.1/featurebyte/api/feature_or_target_namespace_mixin.py` & `featurebyte-0.4.2/featurebyte/api/feature_or_target_namespace_mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/feature_store.py` & `featurebyte-0.4.2/featurebyte/api/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/feature_util.py` & `featurebyte-0.4.2/featurebyte/api/feature_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/feature_validation_util.py` & `featurebyte-0.4.2/featurebyte/api/feature_validation_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/groupby.py` & `featurebyte-0.4.2/featurebyte/api/groupby.py`

 * *Files 2% similar despite different names*

```diff
@@ -423,14 +423,16 @@
 
     def forward_aggregate(
         self,
         value_column: str,
         method: str,
         window: Optional[str] = None,
         target_name: Optional[str] = None,
+        fill_value: OptionalScalar = None,
+        skip_fill_na: bool = False,
     ) -> Target:
         """
         The forward_aggregate method of a GroupBy class instance returns a Forward Aggregated Target object. This object
         aggregates data from the column specified by the value_column parameter using the aggregation method
         provided by the method parameter, without taking into account the order or sequence of the data. The primary
         entity of the Target is determined by the grouping key of the GroupBy instance.
 
@@ -440,14 +442,18 @@
             Column to be aggregated
         method: str
             Aggregation method.
         window: Optional[str]
             Optional window to apply to the point in time column in the target request.
         target_name: Optional[str]
             Output target name
+        fill_value: OptionalScalar
+            Value to fill if the value in the column is empty
+        skip_fill_na: bool
+            Whether to skip filling NaN values
 
         Returns
         -------
         Target
 
         Examples
         --------
@@ -465,8 +471,10 @@
         return ForwardAggregator(
             self.view_obj, self.category, self.entity_ids, self.keys, self.serving_names
         ).forward_aggregate(
             value_column=value_column,
             method=method,
             window=window,
             target_name=target_name,
+            fill_value=fill_value,
+            skip_fill_na=skip_fill_na,
         )
```

### Comparing `featurebyte-0.4.1/featurebyte/api/historical_feature_table.py` & `featurebyte-0.4.2/featurebyte/api/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/item_table.py` & `featurebyte-0.4.2/featurebyte/api/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/item_view.py` & `featurebyte-0.4.2/featurebyte/api/item_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,14 +322,14 @@
             if column_structure.table_type != TableDataType.EVENT_TABLE:
                 return False
         return True
 
     def get_join_column(self) -> str:
         return self.item_id_column
 
-    def _get_as_feature_parameters(self, offset: Optional[str] = None) -> dict[str, Any]:
+    def get_additional_lookup_parameters(self, offset: Optional[str] = None) -> dict[str, Any]:
         _ = offset
         return {
             "event_parameters": {
                 "event_timestamp_column": self.timestamp_column,
             }
         }
```

### Comparing `featurebyte-0.4.1/featurebyte/api/lag.py` & `featurebyte-0.4.2/featurebyte/api/lag.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/materialized_table.py` & `featurebyte-0.4.2/featurebyte/api/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/mixin.py` & `featurebyte-0.4.2/featurebyte/api/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/observation_table.py` & `featurebyte-0.4.2/featurebyte/api/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/periodic_task.py` & `featurebyte-0.4.2/featurebyte/api/periodic_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/relationship.py` & `featurebyte-0.4.2/featurebyte/api/relationship.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/request_column.py` & `featurebyte-0.4.2/featurebyte/api/request_column.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/savable_api_object.py` & `featurebyte-0.4.2/featurebyte/api/savable_api_object.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/scd_table.py` & `featurebyte-0.4.2/featurebyte/api/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/scd_view.py` & `featurebyte-0.4.2/featurebyte/api/scd_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,14 @@
             excluded_columns.append(self.current_flag_column)
         if self.surrogate_key_column:
             excluded_columns.append(self.surrogate_key_column)
         if self.end_timestamp_column:
             excluded_columns.append(self.end_timestamp_column)
         return excluded_columns
 
-    def _get_as_feature_parameters(self, offset: Optional[str] = None) -> dict[str, Any]:
+    def get_additional_lookup_parameters(self, offset: Optional[str] = None) -> dict[str, Any]:
         return {
             "scd_parameters": {
                 "offset": offset,
                 **self.get_common_scd_parameters().dict(),
             }
         }
```

### Comparing `featurebyte-0.4.1/featurebyte/api/simple_aggregator.py` & `featurebyte-0.4.2/featurebyte/api/simple_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/source_table.py` & `featurebyte-0.4.2/featurebyte/api/source_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/static_source_table.py` & `featurebyte-0.4.2/featurebyte/api/static_source_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/table.py` & `featurebyte-0.4.2/featurebyte/api/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/target.py` & `featurebyte-0.4.2/featurebyte/api/target.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from featurebyte.api.api_object_util import ForeignKeyMapping
 from featurebyte.api.entity import Entity
 from featurebyte.api.feature_or_target_mixin import FeatureOrTargetMixin
 from featurebyte.api.feature_store import FeatureStore
 from featurebyte.api.observation_table import ObservationTable
 from featurebyte.api.savable_api_object import SavableApiObject
 from featurebyte.api.target_namespace import TargetNamespace
-from featurebyte.api.target_table import TargetTable
 from featurebyte.api.templates.doc_util import substitute_docstring
 from featurebyte.api.templates.feature_or_target_doc import (
     CATALOG_ID_DOC,
     DEFINITION_DOC,
     ENTITY_IDS_DOC,
     PREVIEW_DOC,
     PRIMARY_ENTITY_DOC,
@@ -32,14 +31,16 @@
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.common.utils import dataframe_to_arrow_bytes, enforce_observation_set_row_order
 from featurebyte.core.accessor.target_datetime import TargetDtAccessorMixin
 from featurebyte.core.accessor.target_string import TargetStrAccessorMixin
 from featurebyte.core.series import Series
 from featurebyte.exception import RecordRetrievalException
 from featurebyte.models.feature_store import FeatureStoreModel
+from featurebyte.models.observation_table import TargetInput
+from featurebyte.models.request_input import RequestInputType
 from featurebyte.models.target import TargetModel
 from featurebyte.query_graph.model.common_table import TabularSource
 from featurebyte.schema.target import TargetUpdate
 from featurebyte.schema.target_table import TargetTableCreate
 
 DOCSTRING_FORMAT_PARAMS = {"class_name": "Target"}
 
@@ -289,75 +290,85 @@
         --------
         >>> target = catalog.get_target("target")  # doctest: +SKIP
         >>> target.compute_targets(observation_table)  # doctest: +SKIP
         """
         temp_target_table_name = f"__TEMPORARY_TARGET_TABLE_{ObjectId()}"
         temp_target_table = self.compute_target_table(
             observation_table=observation_table,
-            target_table_name=temp_target_table_name,
+            observation_table_name=temp_target_table_name,
             serving_names_mapping=serving_names_mapping,
         )
         try:
             return temp_target_table.to_pandas()
         finally:
             temp_target_table.delete()
 
     @typechecked
     def compute_target_table(
         self,
         observation_table: Union[ObservationTable, pd.DataFrame],
-        target_table_name: str,
+        observation_table_name: str,
         serving_names_mapping: Optional[Dict[str, str]] = None,
-    ) -> TargetTable:
+    ) -> ObservationTable:
         """
         Materialize feature list using an observation table asynchronously. The targets
         will be materialized into a target table.
 
         Parameters
         ----------
         observation_table: Union[ObservationTable, pd.DataFrame]
             Observation set with `POINT_IN_TIME` and serving names columns. This can be either an
             ObservationTable of a pandas DataFrame.
-        target_table_name: str
-            Name of the target table to be created
+        observation_table_name: str
+            Name of the observation table to be created with the target values
         serving_names_mapping : Optional[Dict[str, str]]
             Optional serving names mapping if the training events table has different serving name
 
         Returns
         -------
-        TargetTable
+        ObservationTable
 
         Examples
         --------
         >>> target = catalog.get_target("target")  # doctest: +SKIP
         >>> target.compute_target_table(observation_table, "target_table")  # doctest: +SKIP
         """
+        is_input_observation_table = isinstance(observation_table, ObservationTable)
+        observation_table_id = observation_table.id if is_input_observation_table else None
+        input_type = (
+            RequestInputType.OBSERVATION_TABLE
+            if is_input_observation_table
+            else RequestInputType.DATAFRAME
+        )
         target_table_create_params = TargetTableCreate(
-            name=target_table_name,
-            observation_table_id=(
-                observation_table.id if isinstance(observation_table, ObservationTable) else None
-            ),
+            name=observation_table_name,
+            observation_table_id=observation_table_id,
             feature_store_id=self.feature_store.id,
             serving_names_mapping=serving_names_mapping,
             target_id=self.id,
             graph=self.graph,
             node_names=[self.node.name],
+            request_input=TargetInput(
+                target_id=self.id,
+                observation_table_id=observation_table_id,
+                type=input_type,
+            ),
         )
-        if isinstance(observation_table, ObservationTable):
+        if is_input_observation_table:
             files = None
         else:
             assert isinstance(observation_table, pd.DataFrame)
             files = {"observation_set": dataframe_to_arrow_bytes(observation_table)}
-        target_table_doc = self.post_async_task(
+        observation_table_doc = self.post_async_task(
             route="/target_table",
             payload={"payload": target_table_create_params.json()},
             is_payload_json=False,
             files=files,
         )
-        return TargetTable.get_by_id(target_table_doc["_id"])
+        return ObservationTable.get_by_id(observation_table_doc["_id"])
 
     @property
     def target_namespace(self) -> TargetNamespace:
         """
         TargetNamespace object of current target
 
         Returns
```

### Comparing `featurebyte-0.4.1/featurebyte/api/target_namespace.py` & `featurebyte-0.4.2/featurebyte/api/target_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/target_table.py` & `featurebyte-0.4.2/featurebyte/service/materialized_table.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,182 +1,140 @@
 """
-TargetTable class
+BaseMaterializedTableService contains common functionality for materialized tables
 """
 from __future__ import annotations
 
-from typing import Optional, Union
+from typing import Any, List, Optional, Tuple
 
-from pathlib import Path
+from bson import ObjectId
 
-import pandas as pd
-
-from featurebyte.api.api_object import ApiObject
-from featurebyte.api.api_object_util import ForeignKeyMapping
-from featurebyte.api.feature_store import FeatureStore
-from featurebyte.api.materialized_table import MaterializedTableMixin
-from featurebyte.api.observation_table import ObservationTable
-from featurebyte.common.doc_util import FBAutoDoc
-from featurebyte.models.base import PydanticObjectId
-from featurebyte.models.target_table import TargetTableModel
-from featurebyte.schema.target_table import TargetTableListRecord
-
-
-class TargetTable(ApiObject, MaterializedTableMixin):
+from featurebyte.persistent import Persistent
+from featurebyte.query_graph.model.common_table import TabularSource
+from featurebyte.query_graph.node.schema import ColumnSpec, TableDetails
+from featurebyte.query_graph.sql.common import sql_to_string
+from featurebyte.query_graph.sql.materialisation import get_source_count_expr
+from featurebyte.schema.common.base import BaseDocumentServiceUpdateSchema
+from featurebyte.schema.worker.task.materialized_table_delete import (
+    MaterializedTableDeleteTaskPayload,
+)
+from featurebyte.service.base_document import BaseDocumentService
+from featurebyte.service.feature_store import FeatureStoreService
+from featurebyte.service.mixin import Document, DocumentCreateSchema
+from featurebyte.session.base import BaseSession
+from featurebyte.session.manager import SessionManager
+
+
+class BaseMaterializedTableService(
+    BaseDocumentService[Document, DocumentCreateSchema, BaseDocumentServiceUpdateSchema]
+):
     """
-    TargetTable class
+    BaseMaterializedTableService contains common functionality for materialized tables
     """
 
-    __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.TargetTable")
-
-    _route = "/target_table"
-    _list_schema = TargetTableListRecord
-    _get_schema = TargetTableModel
-    _list_fields = [
-        "name",
-        "feature_store_name",
-        "observation_table_name",
-        "shape",
-        "created_at",
-    ]
-    _list_foreign_keys = [
-        ForeignKeyMapping("feature_store_id", FeatureStore, "feature_store_name"),
-        ForeignKeyMapping("observation_table_id", ObservationTable, "observation_table_name"),
-    ]
-
-    @property
-    def observation_table_id(self) -> Optional[PydanticObjectId]:
-        """
-        Observation table ID.
-
-        Returns
-        -------
-        Optional[PydanticObjectId]
-            Observation table ID
-        """
-        return self.cached_model.observation_table_id
-
-    @property
-    def target_id(self) -> PydanticObjectId:
-        """
-        Get the target ID.
-
-        Returns
-        -------
-        PydanticObjectId
-            Target ID
-        """
-        return self.cached_model.target_id
-
-    def preview(self, limit: int = 10) -> pd.DataFrame:
-        """
-        Returns a DataFrame that contains a selection of rows of the target table.
-
-        Parameters
-        ----------
-        limit: int
-            Maximum number of return rows.
-
-        Returns
-        -------
-        pd.DataFrame
-            Preview rows of the table.
-
-        Examples
-        --------
-        >>> target_table = catalog.get_target_table("target_table_name")  # doctest: +SKIP
-        >>> target_table.preview()  # doctest: +SKIP
-        """
-        return super().preview(limit=limit)
+    materialized_table_name_prefix = ""
 
-    def sample(self, size: int = 10, seed: int = 1234) -> pd.DataFrame:
+    def __init__(
+        self,
+        user: Any,
+        persistent: Persistent,
+        catalog_id: Optional[ObjectId],
+        feature_store_service: FeatureStoreService,
+    ):
+        super().__init__(user, persistent, catalog_id)
+        self.feature_store_service = feature_store_service
+
+    async def get_materialized_table_delete_task_payload(
+        self, document_id: ObjectId
+    ) -> MaterializedTableDeleteTaskPayload:
         """
-        Returns a DataFrame that contains a random selection of rows of the target table based on a
-        specified size and seed for sampling control.
+        Get the materialized table delete task payload
 
         Parameters
         ----------
-        size: int
-            Maximum number of rows to sample.
-        seed: int
-            Seed to use for random sampling.
+        document_id: ObjectId
+            The document id
 
         Returns
         -------
-        pd.DataFrame
-            Sampled rows from the table.
-
-        Examples
-        --------
-        >>> target_table = catalog.get_target_table("target_table_name")  # doctest: +SKIP
-        >>> target_table.sample()  # doctest: +SKIP
+        MaterializedTableDeleteTaskPayload
         """
-        return super().sample(size=size, seed=seed)
+        return MaterializedTableDeleteTaskPayload(
+            user_id=self.user.id,
+            catalog_id=self.catalog_id,
+            document_id=document_id,
+            collection_name=self.document_class.collection_name(),
+        )
 
-    def describe(self, size: int = 0, seed: int = 1234) -> pd.DataFrame:
+    async def generate_materialized_table_location(
+        self, get_credential: Any, feature_store_id: ObjectId
+    ) -> TabularSource:
         """
-        Returns descriptive statistics of the target table.
+        Generate a TabularSource object for a new materialized table to be created
 
         Parameters
         ----------
-        size: int
-            Maximum number of rows to sample. If 0, all rows will be used.
-        seed: int
-            Seed to use for random sampling.
+        get_credential: Any
+            Function to get credential for a feature store
+        feature_store_id: ObjectId
+            Feature store id
 
         Returns
         -------
-        pd.DataFrame
-            Summary of the table.
-
-        Examples
-        --------
-        >>> target_table = catalog.get_target_table("target_table_name")  # doctest: +SKIP
-        >>> target_table.describe()  # doctest: +SKIP
-        """
-        return super().describe(size=size, seed=seed)
-
-    def download(self, output_path: Optional[Union[str, Path]] = None) -> Path:
+        TabularSource
+        """
+        feature_store = await self.feature_store_service.get_document(document_id=feature_store_id)
+        session_manager = SessionManager(
+            credentials={
+                feature_store.name: await get_credential(
+                    user_id=self.user.id, feature_store_name=feature_store.name
+                )
+            }
+        )
+        db_session = await session_manager.get_session(feature_store)
+
+        destination_table_name = f"{self.materialized_table_name_prefix}_{ObjectId()}"
+        location = TabularSource(
+            feature_store_id=feature_store_id,
+            table_details=TableDetails(
+                database_name=db_session.database_name,
+                schema_name=db_session.schema_name,
+                table_name=destination_table_name,
+            ),
+        )
+        return location
+
+    @staticmethod
+    async def get_columns_info_and_num_rows(
+        db_session: BaseSession, table_details: TableDetails
+    ) -> Tuple[List[ColumnSpec], int]:
         """
-        Downloads the target table from the database.
+        Get the columns info and number of rows from a materialized table
 
         Parameters
         ----------
-        output_path: Optional[Union[str, Path]]
-            Location to save downloaded parquet file.
+        db_session: BaseSession
+            The database session
+        table_details: TableDetails
+            The table details of the materialized table
 
         Returns
         -------
-        Path
-
-        Raises
-        ------
-        FileExistsError
-            File already exists at output path.
-        RecordRetrievalException
-            Error retrieving record from API.
-
-        Examples
-        --------
-        >>> target_table = catalog.get_target_table("target_table_name")  # doctest: +SKIP
-        >>> downloaded_path = target_table.download(output_path="path/to/download")  # doctest: +SKIP
-
-        # noqa: DAR402
-        """
-        return super().download(output_path=output_path)
-
-    def delete(self) -> None:
-        """
-        Deletes the target table.
-
-        Raises
-        ------
-        RecordDeletionException
-            When the record cannot be deleted properly
-
-        Examples
-        --------
-        >>> target_table = catalog.get_target_table("target_table_name")  # doctest: +SKIP
-        >>> target_table.delete()  # doctest: +SKIP
-
-        # noqa: DAR402
-        """
-        super().delete()
+        Tuple[List[ColumnSpec], int]
+            The columns info and number of rows
+        """
+        table_schema = await db_session.list_table_schema(
+            table_name=table_details.table_name,
+            database_name=table_details.database_name,
+            schema_name=table_details.schema_name,
+        )
+        df_row_count = await db_session.execute_query(
+            sql_to_string(
+                get_source_count_expr(table_details),
+                db_session.source_type,
+            )
+        )
+        assert df_row_count is not None
+        num_rows = df_row_count.iloc[0]["row_count"]
+        columns_info = [
+            ColumnSpec(name=name, dtype=var_type) for name, var_type in table_schema.items()
+        ]
+        return columns_info, num_rows
```

### Comparing `featurebyte-0.4.1/featurebyte/api/templates/doc_util.py` & `featurebyte-0.4.2/featurebyte/api/templates/doc_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/templates/feature_or_target_doc.py` & `featurebyte-0.4.2/featurebyte/api/templates/feature_or_target_doc.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/templates/online_serving/python.tpl` & `featurebyte-0.4.2/featurebyte/api/templates/online_serving/python.tpl`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/user_defined_function.py` & `featurebyte-0.4.2/featurebyte/api/user_defined_function.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/user_defined_function_injector.py` & `featurebyte-0.4.2/featurebyte/api/user_defined_function_injector.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/view.py` & `featurebyte-0.4.2/featurebyte/api/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 View class
 """
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-public-methods
 from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
+    Dict,
     List,
     Literal,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
@@ -27,24 +28,25 @@
 
 from featurebyte.api.batch_request_table import BatchRequestTable
 from featurebyte.api.entity import Entity
 from featurebyte.api.feature import Feature
 from featurebyte.api.feature_group import FeatureGroup
 from featurebyte.api.observation_table import ObservationTable
 from featurebyte.api.static_source_table import StaticSourceTable
+from featurebyte.api.target import Target
+from featurebyte.api.window_validator import validate_offset
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.common.join_utils import (
     append_rsuffix_to_column_info,
     append_rsuffix_to_columns,
     combine_column_info_of_views,
     filter_columns,
     filter_columns_info,
     is_column_name_in_columns,
 )
-from featurebyte.common.model_util import validate_offset_string
 from featurebyte.common.typing import ScalarSequence
 from featurebyte.core.frame import Frame, FrozenFrame
 from featurebyte.core.generic import ProtectedColumnsQueryObject, QueryObject
 from featurebyte.core.mixin import SampleMixin
 from featurebyte.core.series import FrozenSeries, FrozenSeriesT, Series
 from featurebyte.enum import DBVarType
 from featurebyte.exception import (
@@ -273,14 +275,100 @@
         >>> catalog.get_view("GROCERYINVOICE")["Amount"].describe(  # doctest: +SKIP
         ...   from_timestamp="2020-01-01",
         ...   to_timestamp="2023-01-31"
         ... )
         """
         return super().describe(size, seed, from_timestamp, to_timestamp, **kwargs)
 
+    def _get_view_and_input_col_for_lookup(self, function_name: str) -> Tuple[View, str]:
+        """
+        Returns the View object that is used for lookup targets or features.
+
+        Parameters
+        ----------
+        function_name: str
+            The name of the function that is being called.
+
+        Returns
+        -------
+        Tuple[View, str]
+            The View object and the input column name.
+
+        Raises
+        ------
+        ValueError
+            If the View object is not assigned to the ViewColumn.
+        """
+        view = self._parent
+        if view is None:
+            raise ValueError(
+                f"{function_name} is only supported for named columns in the View object. Consider"
+                f" assigning to the View before calling {function_name}()."
+            )
+        input_column_name = cast(ProjectNode.Parameters, self.node.parameters).columns[0]
+        return cast(View, view[[input_column_name]]), input_column_name
+
+    @typechecked
+    def as_target(self, target_name: str, offset: Optional[str] = None) -> Target:
+        """
+        Create a lookup target directly from the column in the View.
+
+        For SCD views, lookup targets are materialized through point-in-time joins, and the resulting value represents
+        the active row for the natural key at the point-in-time indicated in the target request.
+
+        To obtain a target value at a specific time before the request's point-in-time, an offset can be specified.
+
+        Parameters
+        ----------
+        target_name: str
+            Name of the target to create.
+        offset: str
+            When specified, retrieve target value as of this offset prior to the point-in-time.
+
+        Returns
+        -------
+        Target
+
+        Examples
+        --------
+        >>> customer_view = catalog.get_view("GROCERYCUSTOMER")
+        >>> # Extract operating system from BrowserUserAgent column
+        >>> customer_view["OperatingSystemIsWindows"] = customer_view.BrowserUserAgent.str.contains("Windows")
+        >>> # Create a target from the OperatingSystemIsWindows column
+        >>> uses_windows = customer_view.OperatingSystemIsWindows.as_target("UsesWindows")
+
+
+        If the view is a Slowly Changing Dimension View, you may also consider to create a target that retrieves the
+        entity's attribute at a point-in-time prior to the point-in-time specified in the target request by specifying
+        an offset.
+
+        >>> uses_windows_12w_ago = customer_view.OperatingSystemIsWindows.as_target(
+        ...   "UsesWindows_12w_ago", offset="12w"
+        ... )
+        """
+        view, input_column_name = self._get_view_and_input_col_for_lookup("as_target")
+
+        # Perform validation
+        validate_offset(offset)
+
+        # Add lookup node to graph, and return Target
+        lookup_node_params = view.get_lookup_node_params([input_column_name], [target_name], offset)
+        input_node = view.get_input_node_for_lookup_node()
+        lookup_node = self.graph.add_operation(
+            node_type=NodeType.LOOKUP_TARGET,
+            node_params=lookup_node_params,
+            node_output_type=NodeOutputType.FRAME,
+            input_nodes=[input_node],
+        )
+        return view.project_target_from_node(
+            input_node=lookup_node,
+            target_name=target_name,
+            target_dtype=view.column_var_type_map[input_column_name],
+        )
+
     @typechecked
     def as_feature(self, feature_name: str, offset: Optional[str] = None) -> Feature:
         """
         Creates a lookup feature directly from the column in the View.
 
         For SCD views, lookup features are materialized through point-in-time joins, and the resulting value represents
         the active row for the natural key at the point-in-time indicated in the feature request.
@@ -294,19 +382,14 @@
         offset: str
             When specified, retrieve feature value as of this offset prior to the point-in-time.
 
         Returns
         -------
         Feature
 
-        Raises
-        ------
-        ValueError
-            If the column is a temporary column not associated with any View
-
         Examples
         --------
         >>> customer_view = catalog.get_view("GROCERYCUSTOMER")
         >>> # Extract operating system from BrowserUserAgent column
         >>> customer_view["OperatingSystemIsWindows"] = customer_view.BrowserUserAgent.str.contains("Windows")
         >>> # Create a feature from the OperatingSystemIsWindows column
         >>> uses_windows = customer_view.OperatingSystemIsWindows.as_feature("UsesWindows")
@@ -316,22 +399,15 @@
         entity's attribute at a point-in-time prior to the point-in-time specified in the feature request by specifying
         an offset.
 
         >>> uses_windows_12w_ago = customer_view.OperatingSystemIsWindows.as_feature(
         ...   "UsesWindows_12w_ago", offset="12w"
         ... )
         """
-        view = self._parent
-        if view is None:
-            raise ValueError(
-                "as_feature is only supported for named columns in the View object. Consider"
-                " assigning the Feature to the View before calling as_feature()."
-            )
-        input_column_name = cast(ProjectNode.Parameters, self.node.parameters).columns[0]
-        view = cast(View, view[[input_column_name]])
+        view, input_column_name = self._get_view_and_input_col_for_lookup("as_feature")
         feature = view.as_features(
             [input_column_name],
             [feature_name],
             offset=offset,
         )[feature_name]
         return cast(Feature, feature)
 
@@ -948,17 +1024,18 @@
         Returns
         -------
         dict[str, Any]
         """
         _ = calling_view
         return {}
 
-    def _get_as_feature_parameters(self, offset: Optional[str] = None) -> dict[str, Any]:
+    def get_additional_lookup_parameters(self, offset: Optional[str] = None) -> dict[str, Any]:
         """
-        Returns any additional query node parameters for as_feature operation (LookupNode)
+        Returns any additional query node parameters for lookup operations - as_feature (LookupNode), or
+        as_target (LookupTargetNode).
 
         This is a no-op unless the lookup is time-aware (currently only available for
         SCDView)
 
         Parameters
         ----------
         offset : str
@@ -1310,21 +1387,56 @@
         )
 
         # create a new view and return it
         return self._create_joined_view(
             new_node_name=node.name, joined_columns_info=joined_columns_info
         )
 
-    @staticmethod
-    def _validate_offset(offset: Optional[str]) -> None:
-        # Validate offset is valid if provided
-        if offset is not None:
-            validate_offset_string(offset)
+    def project_target_from_node(
+        self,
+        input_node: Node,
+        target_name: str,
+        target_dtype: DBVarType,
+    ) -> Target:
+        """
+        Create a Target object from a node that produces targets, such as groupby, lookup, etc.
+
+        Parameters
+        ----------
+        input_node: Node
+            Query graph node
+        target_name: str
+            Target name
+        target_dtype: DBVarType
+            Variable type of the Target
 
-    def _project_feature_from_node(
+        Returns
+        -------
+        Feature
+        """
+        # Project target node.
+        target_node = self.graph.add_operation(
+            node_type=NodeType.PROJECT,
+            node_params={"columns": [target_name]},
+            node_output_type=NodeOutputType.SERIES,
+            input_nodes=[input_node],
+        )
+        # Build and return Target
+        entity_ids = self.graph.get_entity_ids(node_name=target_node.name)
+        return Target(
+            name=target_name,
+            entity_ids=entity_ids,
+            graph=self.graph,
+            node_name=target_node.name,
+            tabular_source=self.tabular_source,
+            feature_store=self.feature_store,
+            dtype=target_dtype,
+        )
+
+    def project_feature_from_node(
         self,
         node: Node,
         feature_name: str,
         feature_dtype: DBVarType,
     ) -> Feature:
         """
         Create a Feature object from a node that produces features, such as groupby, lookup, etc.
@@ -1375,15 +1487,15 @@
 
         if len(feature_names) != len(column_names):
             raise ValueError(
                 f"Length of feature_names ({len(feature_names)}) should be the same as column_names"
                 f" ({len(column_names)})"
             )
 
-    def _get_input_node_for_lookup_node(self) -> Node:
+    def get_input_node_for_lookup_node(self) -> Node:
         """
         Get the node before any projection(s) to be used as the input node for the lookup node in
         as_features(). The view before such projection(s) must also have those columns and can be
         used as the input instead. Removing redundant projections allows joins to be shared for
         lookup operations using the same source.
 
         Example:
@@ -1404,14 +1516,62 @@
         while node_before_projection.type == NodeType.PROJECT:
             input_node_names = self.graph.get_input_node_names(node_before_projection)
             assert len(input_node_names) == 1
             node_before_projection = self.graph.get_node_by_name(input_node_names[0])
 
         return node_before_projection
 
+    def get_lookup_node_params(
+        self, column_names: List[str], feature_names: List[str], offset: Optional[str]
+    ) -> Dict[str, Any]:
+        """
+        Get the parameters for the lookup node in as_features().
+
+        Parameters
+        ----------
+        column_names: List[str]
+            List of column names to be used as input to the lookup node
+        feature_names: List[str]
+            List of feature names to be used as output of the lookup node
+        offset: Optional[str]
+            Offset to be used for the lookup node
+
+        Returns
+        -------
+        Dict[str, Any]
+
+        Raises
+        ------
+        ValueError
+            If the entity_column is not found in the columns_info
+        """
+        # Get entity_column
+        entity_column = self.get_join_column()
+
+        # Get serving_name
+        columns_info = self.columns_info
+        column_entity_map = {col.name: col.entity_id for col in columns_info if col.entity_id}
+        if entity_column not in column_entity_map:
+            raise ValueError(f'Column "{entity_column}" is not an entity!')
+        entity_id = column_entity_map[entity_column]
+        entity = Entity.get_by_id(entity_id)
+        serving_name = entity.serving_name
+
+        # Set up Lookup node
+        additional_params = self.get_additional_lookup_parameters(offset=offset)
+        return {
+            "input_column_names": column_names,
+            "feature_names": feature_names,
+            "entity_column": entity_column,
+            "serving_name": serving_name,
+            "entity_id": entity_id,
+            "offset": offset,
+            **additional_params,
+        }
+
     @typechecked
     def as_features(
         self,
         column_names: List[str],
         feature_names: List[str],
         offset: Optional[str] = None,
     ) -> FeatureGroup:
@@ -1436,19 +1596,14 @@
         column_names: List[str]
             Column names to be used to create the features
         feature_names: List[str]
             Feature names corresponding to column_names
         offset: Optional[str]
             When specified, retrieve feature values as of this offset prior to the point-in-time
 
-        Raises
-        ------
-        ValueError
-            When any of the specified parameters are invalid
-
         Returns
         -------
         FeatureGroup
 
         Examples
         --------
         >>> features = dimension_view.as_features(  # doctest: +SKIP
@@ -1459,48 +1614,27 @@
         ['Feature A', 'Feature B']
         """
         self._validate_as_features_input_columns(
             column_names=column_names,
             feature_names=feature_names,
         )
 
-        self._validate_offset(offset)
-
-        # Get entity_column
-        entity_column = self.get_join_column()
-
-        # Get serving_name
-        columns_info = self.columns_info
-        column_entity_map = {col.name: col.entity_id for col in columns_info if col.entity_id}
-        if entity_column not in column_entity_map:
-            raise ValueError(f'Column "{entity_column}" is not an entity!')
-        entity_id = column_entity_map[entity_column]
-        entity = Entity.get_by_id(entity_id)
-        serving_name = entity.serving_name
+        validate_offset(offset)
 
-        # Set up Lookup node
-        additional_params = self._get_as_feature_parameters(offset=offset)
-        lookup_node_params = {
-            "input_column_names": column_names,
-            "feature_names": feature_names,
-            "entity_column": entity_column,
-            "serving_name": serving_name,
-            "entity_id": entity_id,
-            **additional_params,
-        }
-        input_node = self._get_input_node_for_lookup_node()
+        lookup_node_params = self.get_lookup_node_params(column_names, feature_names, offset)
+        input_node = self.get_input_node_for_lookup_node()
         lookup_node = self.graph.add_operation(
             node_type=NodeType.LOOKUP,
             node_params=lookup_node_params,
             node_output_type=NodeOutputType.FRAME,
             input_nodes=[input_node],
         )
         features = []
         for input_column_name, feature_name in zip(column_names, feature_names):
-            feature = self._project_feature_from_node(
+            feature = self.project_feature_from_node(
                 node=lookup_node,
                 feature_name=feature_name,
                 feature_dtype=self.column_var_type_map[input_column_name],
             )
             features.append(feature)
 
         return FeatureGroup(features)
```

### Comparing `featurebyte-0.4.1/featurebyte/api/window_aggregator.py` & `featurebyte-0.4.2/featurebyte/api/window_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/api/window_validator.py` & `featurebyte-0.4.2/featurebyte/api/window_validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 """
 Validate window parameter input.
 """
+from typing import Optional
 
-from featurebyte.common.model_util import parse_duration_string
+from featurebyte.common.model_util import parse_duration_string, validate_offset_string
+
+
+def validate_offset(offset: Optional[str]) -> None:
+    """
+    Validates whether the offset param is a valid one.
+
+    Parameters
+    ----------
+    offset: str
+        the offset parameter string
+    """
+    # Validate offset is valid if provided
+    if offset is not None:
+        validate_offset_string(offset)
 
 
 def validate_window(window: str, feature_job_frequency: str) -> None:
     """
     Validates whether the window param is a valid one when used in an aggregate over function.
 
     In particular, we check if
```

### Comparing `featurebyte-0.4.1/featurebyte/app.py` & `featurebyte-0.4.2/featurebyte/app.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/date_util.py` & `featurebyte-0.4.2/featurebyte/common/date_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/descriptor.py` & `featurebyte-0.4.2/featurebyte/common/descriptor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/dict_util.py` & `featurebyte-0.4.2/featurebyte/common/dict_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/doc_util.py` & `featurebyte-0.4.2/featurebyte/common/doc_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/allowed_classes.py` & `featurebyte-0.4.2/featurebyte/common/documentation/allowed_classes.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/autodoc_processor.py` & `featurebyte-0.4.2/featurebyte/common/documentation/autodoc_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,21 +161,14 @@
             qualifier_elem = etree.SubElement(signature_elem, "em")
             qualifier_elem.text = "class "
         elif resource_details.method_type == "async":
             qualifier_elem = etree.SubElement(signature_elem, "em")
             qualifier_elem.text = "async "
 
         name_elem = etree.SubElement(signature_elem, "span")
-        if resource_details.type == "method":
-            # add reference link for methods
-            name_elem = etree.SubElement(name_elem, "a")
-            name_elem.set(
-                "href",
-                f'javascript:window.location=new URL("../{resource_details.path}.{resource_details.realname}/", window.location.href.split("#")[0]).href',
-            )
 
         main_name_elem = etree.SubElement(name_elem, "strong")
         main_name_elem.text = resource_details.name
 
         if resource_details.type == "property":
             self.insert_param_type(signature_elem, resource_details.returns.type)
         else:
```

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/constants.py` & `featurebyte-0.4.2/featurebyte/common/documentation/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 CATALOG = "Catalog"
 CLEANING_OPERATION = "Cleaning Operation"
 CONSTRUCTOR = "Constructor"
 CREATE = "Create"
 CREATE_FEATURE = "Create Feature"
 CREATE_FEATURE_GROUP = "Create Feature Group"
 CREATE_TABLE = "Create Table"
+CREATE_TARGET = "Create Target"
 CREDENTIAL = "Credential"
 CLASS_METHODS = "Class Methods"
 DATA_SOURCE = "DataSource"
 DEPLOY = "Deploy"
 DEPLOYMENT = "Deployment"
 ENTITY = "Entity"
 ENUMS = "Enums"
@@ -47,15 +48,14 @@
 SERVE = "Serve"
 SET_FEATURE_JOB = "Set Feature Job"
 SOURCE_TABLE = "SourceTable"
 TABLE = "Table"
 TABLE_COLUMN = "TableColumn"
 TARGET = "Target"
 TARGET_NAMESPACE = "TargetNamespace"
-TARGET_TABLE = "TargetTable"
 TRANSFORM = "Transform"
 TYPE = "Type"
 USER_DEFINED_FUNCTION = "UserDefinedFunction"
 UTILITY_CLASSES = "Utility Classes"
 UTILITY_METHODS = "Utility Methods"
 VERSION = "Version"
 VIEW = "View"
```

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/custom_nav.py` & `featurebyte-0.4.2/featurebyte/common/documentation/custom_nav.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     CLASS_METHODS,
     CLEANING_OPERATION,
     CONSTRUCTOR,
     CREATE,
     CREATE_FEATURE,
     CREATE_FEATURE_GROUP,
     CREATE_TABLE,
+    CREATE_TARGET,
     CREDENTIAL,
     DATA_SOURCE,
     DEPLOY,
     DEPLOYMENT,
     ENTITY,
     ENUMS,
     EXPLORE,
@@ -46,15 +47,14 @@
     SERVE,
     SET_FEATURE_JOB,
     SOURCE_TABLE,
     TABLE,
     TABLE_COLUMN,
     TARGET,
     TARGET_NAMESPACE,
-    TARGET_TABLE,
     TRANSFORM,
     TYPE,
     USER_DEFINED_FUNCTION,
     UTILITY_CLASSES,
     UTILITY_METHODS,
     VIEW,
     VIEW_COLUMN,
@@ -88,15 +88,14 @@
         HISTORICAL_FEATURE_TABLE,
         DEPLOYMENT,
         BATCH_REQUEST_TABLE,
         BATCH_FEATURE_TABLE,
         USER_DEFINED_FUNCTION,
         TARGET,
         TARGET_NAMESPACE,
-        TARGET_TABLE,
         UTILITY_CLASSES,
         UTILITY_METHODS,
     ]
 
     _custom_second_level_order = [
         CREDENTIAL,
         CLASS_METHODS,
@@ -104,14 +103,15 @@
         LIST,
         GET,
         GET_VIEW,
         CREATE,
         CREATE_FEATURE,
         CREATE_FEATURE_GROUP,
         CREATE_TABLE,
+        CREATE_TARGET,
         CONSTRUCTOR,
         ADD_METADATA,
         SAVE,
         MANAGE,
         JOIN,
         TRANSFORM,
         LAGS,
```

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/doc_types.py` & `featurebyte-0.4.2/featurebyte/common/documentation/doc_types.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/documentation_layout.py` & `featurebyte-0.4.2/featurebyte/common/documentation/documentation_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     CLASS_METHODS,
     CLEANING_OPERATION,
     CONSTRUCTOR,
     CREATE,
     CREATE_FEATURE,
     CREATE_FEATURE_GROUP,
     CREATE_TABLE,
+    CREATE_TARGET,
     CREDENTIAL,
     DATA_SOURCE,
     DEPLOY,
     DEPLOYMENT,
     ENTITY,
     ENUMS,
     EXPLORE,
@@ -46,15 +47,14 @@
     SERVE,
     SET_FEATURE_JOB,
     SOURCE_TABLE,
     TABLE,
     TABLE_COLUMN,
     TARGET,
     TARGET_NAMESPACE,
-    TARGET_TABLE,
     TRANSFORM,
     TYPE,
     USER_DEFINED_FUNCTION,
     UTILITY_CLASSES,
     UTILITY_METHODS,
     VIEW,
     VIEW_COLUMN,
@@ -642,14 +642,15 @@
     -------
     List[DocLayoutItem]
         The layout for the ViewColumn class.
     """
     return [
         DocLayoutItem([VIEW_COLUMN]),
         DocLayoutItem([VIEW_COLUMN, CREATE_FEATURE, "ViewColumn.as_feature"]),
+        DocLayoutItem([VIEW_COLUMN, CREATE_TARGET, "ViewColumn.as_target"]),
         *_get_sample_mixin_layout(VIEW_COLUMN),
         DocLayoutItem([VIEW_COLUMN, INFO, "ViewColumn.dtype"]),
         DocLayoutItem([VIEW_COLUMN, INFO, "ViewColumn.is_datetime"]),
         DocLayoutItem([VIEW_COLUMN, INFO, "ViewColumn.is_numeric"]),
         DocLayoutItem([VIEW_COLUMN, INFO, "ViewColumn.name"]),
         DocLayoutItem([VIEW_COLUMN, INFO, "ViewColumn.cleaning_operations"]),
         DocLayoutItem([VIEW_COLUMN, LAGS, "ChangeViewColumn.lag"]),
@@ -975,30 +976,14 @@
         ),
         DocLayoutItem(
             [HISTORICAL_FEATURE_TABLE, LINEAGE, "HistoricalFeatureTable.observation_table_id"]
         ),
     ]
 
 
-def _get_target_table_layout() -> List[DocLayoutItem]:
-    """
-    The layout for the TargetTable module.
-
-    Returns
-    -------
-    List[DocLayoutItem]
-        The layout for the TargetTable module.
-    """
-    return [
-        *_get_materialized_table_layout(TARGET_TABLE),
-        DocLayoutItem([TARGET_TABLE, LINEAGE, "TargetTable.observation_table_id"]),
-        DocLayoutItem([TARGET_TABLE, LINEAGE, "TargetTable.target_id"]),
-    ]
-
-
 def _get_user_defined_function_layout() -> List[DocLayoutItem]:
     """
     The layout for the UserDefinedFunction module.
 
     Returns
     -------
     List[DocLayoutItem]
@@ -1087,9 +1072,8 @@
         *_get_batch_feature_table_layout(),
         *_get_batch_request_table_layout(),
         *_get_observation_table_layout(),
         *_get_historical_feature_table_layout(),
         *_get_user_defined_function_layout(),
         *_get_target_layout(),
         *_get_target_namespace_layout(),
-        *_get_target_table_layout(),
     ]
```

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/extract_csv.py` & `featurebyte-0.4.2/featurebyte/common/documentation/extract_csv.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/formatters.py` & `featurebyte-0.4.2/featurebyte/common/documentation/formatters.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/gen_ref_pages_docs_builder.py` & `featurebyte-0.4.2/featurebyte/common/documentation/gen_ref_pages_docs_builder.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/markdown_extension/extension.py` & `featurebyte-0.4.2/featurebyte/common/documentation/markdown_extension/extension.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/pydantic_field_docs.py` & `featurebyte-0.4.2/featurebyte/common/documentation/pydantic_field_docs.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/resource_extractor.py` & `featurebyte-0.4.2/featurebyte/common/documentation/resource_extractor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/documentation/resource_util.py` & `featurebyte-0.4.2/featurebyte/common/documentation/resource_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/env_util.py` & `featurebyte-0.4.2/featurebyte/common/env_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     Returns
     -------
     bool
     """
     try:
         shell = get_ipython().__class__.__name__  # type: ignore
-        return bool(shell == "ZMQInteractiveShell")
+        return bool(shell in ["ZMQInteractiveShell", "Shell", "DatabricksShell"])
     except NameError:
         return False
 
 
 def get_alive_bar_additional_params() -> dict[str, Any]:
     """
     Get alive_bar additional parameters based on running environment
```

### Comparing `featurebyte-0.4.1/featurebyte/common/formatting_util.py` & `featurebyte-0.4.2/featurebyte/common/formatting_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/join_utils.py` & `featurebyte-0.4.2/featurebyte/common/join_utils.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/model_util.py` & `featurebyte-0.4.2/featurebyte/common/model_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/path_util.py` & `featurebyte-0.4.2/featurebyte/common/path_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/progress.py` & `featurebyte-0.4.2/featurebyte/common/progress.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/typing.py` & `featurebyte-0.4.2/featurebyte/common/typing.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/utils.py` & `featurebyte-0.4.2/featurebyte/common/utils.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/common/validator.py` & `featurebyte-0.4.2/featurebyte/common/validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/config.py` & `featurebyte-0.4.2/featurebyte/config.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/conftest.py` & `featurebyte-0.4.2/featurebyte/conftest.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/accessor/count_dict.py` & `featurebyte-0.4.2/featurebyte/core/accessor/count_dict.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/accessor/datetime.py` & `featurebyte-0.4.2/featurebyte/core/accessor/datetime.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/accessor/feature_datetime.py` & `featurebyte-0.4.2/featurebyte/core/accessor/feature_datetime.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/accessor/feature_string.py` & `featurebyte-0.4.2/featurebyte/core/accessor/feature_string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/accessor/string.py` & `featurebyte-0.4.2/featurebyte/core/accessor/string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/accessor/target_datetime.py` & `featurebyte-0.4.2/featurebyte/core/accessor/target_datetime.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/accessor/target_string.py` & `featurebyte-0.4.2/featurebyte/core/accessor/target_string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/frame.py` & `featurebyte-0.4.2/featurebyte/core/frame.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/generic.py` & `featurebyte-0.4.2/featurebyte/core/generic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/mixin.py` & `featurebyte-0.4.2/featurebyte/core/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/series.py` & `featurebyte-0.4.2/featurebyte/core/series.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/timedelta.py` & `featurebyte-0.4.2/featurebyte/core/timedelta.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/core/util.py` & `featurebyte-0.4.2/featurebyte/core/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/datasets/__main__.py` & `featurebyte-0.4.2/featurebyte/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/datasets/app.py` & `featurebyte-0.4.2/featurebyte/datasets/app.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/datasets/creditcard.sql` & `featurebyte-0.4.2/featurebyte/datasets/creditcard.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/datasets/doctest_grocery.sql` & `featurebyte-0.4.2/featurebyte/datasets/doctest_grocery.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/datasets/grocery.sql` & `featurebyte-0.4.2/featurebyte/datasets/grocery.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/datasets/healthcare.sql` & `featurebyte-0.4.2/featurebyte/datasets/healthcare.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/docker/featurebyte.yml` & `featurebyte-0.4.2/featurebyte/docker/featurebyte.yml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
       driver: local
   featurebyte-server:
     networks:
       - featurebyte
     hostname: featurebyte-server
     restart: unless-stopped
     container_name: featurebyte-server
-    image: featurebyte/featurebyte-server:0.4.1
+    image: featurebyte/featurebyte-server:0.4.2
     depends_on:
       mongo-rs:
         condition: service_healthy
     ports:
       - "0.0.0.0:8088:8088"
     command: ["bash", "/docker-entrypoint.sh", "server"]
     environment:
@@ -67,15 +67,15 @@
       driver: local
   featurebyte-worker:
     networks:
       - featurebyte
     hostname: featurebyte-worker
     restart: unless-stopped
     container_name: featurebyte-worker
-    image: featurebyte/featurebyte-server:0.4.1
+    image: featurebyte/featurebyte-server:0.4.2
     depends_on:
       mongo-rs:
         condition: service_healthy
       redis:
         condition: service_healthy
     environment:
       - "FEATUREBYTE_HOME=/app/.featurebyte"
```

### Comparing `featurebyte-0.4.1/featurebyte/docker/manager.py` & `featurebyte-0.4.2/featurebyte/docker/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/enum.py` & `featurebyte-0.4.2/featurebyte/enum.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/exception.py` & `featurebyte-0.4.2/featurebyte/exception.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/feature_manager/model.py` & `featurebyte-0.4.2/featurebyte/feature_manager/model.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/feature_manager/sql_template.py` & `featurebyte-0.4.2/featurebyte/feature_manager/sql_template.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/feature_utility.py` & `featurebyte-0.4.2/featurebyte/feature_utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,26 +67,26 @@
                 continue
             if isinstance(var_obj, Feature) and not _is_saved(var_obj):
                 unsaved_features.append(
                     {
                         "object_id": str(var_obj.id),
                         "variable_name": var_name,
                         "name": var_obj.name,
-                        "catalog_id": var_obj.catalog_id,
+                        "catalog_id": str(var_obj.catalog_id),
                     }
                 )
             elif isinstance(var_obj, BaseFeatureGroup):
                 for name, feature in var_obj.feature_objects.items():
                     if not _is_saved(feature):
                         unsaved_features.append(
                             {
                                 "object_id": str(feature.id),
                                 "variable_name": f'{var_name}["{name}"]',
                                 "name": feature.name,
-                                "catalog_id": feature.catalog_id,
+                                "catalog_id": str(feature.catalog_id),
                             }
                         )
             processed_variables.add(var_name)
 
     if unsaved_features:
         catalogs = Catalog.list(include_id=True)
         return (
```

### Comparing `featurebyte-0.4.1/featurebyte/logging.py` & `featurebyte-0.4.2/featurebyte/logging.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/middleware.py` & `featurebyte-0.4.2/featurebyte/middleware.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/migration/migration_data_service.py` & `featurebyte-0.4.2/featurebyte/migration/migration_data_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/migration/model.py` & `featurebyte-0.4.2/featurebyte/migration/model.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/migration/run.py` & `featurebyte-0.4.2/featurebyte/migration/run.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/migration/service/__init__.py` & `featurebyte-0.4.2/featurebyte/migration/service/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/migration/service/data_warehouse.py` & `featurebyte-0.4.2/featurebyte/migration/service/data_warehouse.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/migration/service/mixin.py` & `featurebyte-0.4.2/featurebyte/migration/service/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/__init__.py` & `featurebyte-0.4.2/featurebyte/models/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/base.py` & `featurebyte-0.4.2/featurebyte/models/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/batch_feature_table.py` & `featurebyte-0.4.2/featurebyte/models/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/batch_request_table.py` & `featurebyte-0.4.2/featurebyte/models/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/catalog.py` & `featurebyte-0.4.2/featurebyte/models/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/context.py` & `featurebyte-0.4.2/featurebyte/models/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/credential.py` & `featurebyte-0.4.2/featurebyte/models/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/deployment.py` & `featurebyte-0.4.2/featurebyte/models/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/dimension_table.py` & `featurebyte-0.4.2/featurebyte/models/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/entity.py` & `featurebyte-0.4.2/featurebyte/models/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/entity_validation.py` & `featurebyte-0.4.2/featurebyte/models/entity_validation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/event_table.py` & `featurebyte-0.4.2/featurebyte/models/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/feature.py` & `featurebyte-0.4.2/featurebyte/models/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/feature_job_setting_analysis.py` & `featurebyte-0.4.2/featurebyte/models/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/feature_list.py` & `featurebyte-0.4.2/featurebyte/models/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/feature_namespace.py` & `featurebyte-0.4.2/featurebyte/models/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/feature_store.py` & `featurebyte-0.4.2/featurebyte/models/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/historical_feature_table.py` & `featurebyte-0.4.2/featurebyte/models/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/item_table.py` & `featurebyte-0.4.2/featurebyte/models/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/materialized_table.py` & `featurebyte-0.4.2/featurebyte/models/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/online_store.py` & `featurebyte-0.4.2/featurebyte/models/online_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/online_store_compute_query.py` & `featurebyte-0.4.2/featurebyte/models/online_store_compute_query.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/online_store_table_version.py` & `featurebyte-0.4.2/featurebyte/models/online_store_table_version.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/parent_serving.py` & `featurebyte-0.4.2/featurebyte/models/parent_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/periodic_task.py` & `featurebyte-0.4.2/featurebyte/models/periodic_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/persistent.py` & `featurebyte-0.4.2/featurebyte/models/persistent.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/proxy_table.py` & `featurebyte-0.4.2/featurebyte/models/proxy_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/relationship.py` & `featurebyte-0.4.2/featurebyte/models/relationship.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/relationship_analysis.py` & `featurebyte-0.4.2/featurebyte/models/relationship_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/request_input.py` & `featurebyte-0.4.2/featurebyte/models/request_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 class RequestInputType(StrEnum):
     """
     Input type refers to how an ObservationTableModel is created
     """
 
     VIEW = "view"
     SOURCE_TABLE = "source_table"
+    OBSERVATION_TABLE = "observation_table"
+    DATAFRAME = "dataframe"
 
 
 class BaseRequestInput(FeatureByteBaseModel):
     """
     BaseRequestInput is the base class for all RequestInput types
     """
```

### Comparing `featurebyte-0.4.1/featurebyte/models/scd_table.py` & `featurebyte-0.4.2/featurebyte/models/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/semantic.py` & `featurebyte-0.4.2/featurebyte/models/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/static_source_table.py` & `featurebyte-0.4.2/featurebyte/models/static_source_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/target.py` & `featurebyte-0.4.2/featurebyte/models/target.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/target_namespace.py` & `featurebyte-0.4.2/featurebyte/models/target_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/target_table.py` & `featurebyte-0.4.2/featurebyte/models/target_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/task.py` & `featurebyte-0.4.2/featurebyte/models/task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/tile.py` & `featurebyte-0.4.2/featurebyte/models/tile.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/tile_job_log.py` & `featurebyte-0.4.2/featurebyte/models/tile_job_log.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/tile_registry.py` & `featurebyte-0.4.2/featurebyte/models/tile_registry.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/models/user_defined_function.py` & `featurebyte-0.4.2/featurebyte/models/user_defined_function.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/persistent/audit.py` & `featurebyte-0.4.2/featurebyte/persistent/audit.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/persistent/base.py` & `featurebyte-0.4.2/featurebyte/persistent/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/persistent/mongo.py` & `featurebyte-0.4.2/featurebyte/persistent/mongo.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/algorithm.py` & `featurebyte-0.4.2/featurebyte/query_graph/algorithm.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/enum.py` & `featurebyte-0.4.2/featurebyte/query_graph/enum.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     # SQL operations
     PROJECT = "project"
     FILTER = "filter"
     GROUPBY = "groupby"
     ITEM_GROUPBY = "item_groupby"
     AGGREGATE_AS_AT = "aggregate_as_at"
     LOOKUP = "lookup"
+    LOOKUP_TARGET = "lookup_target"
     JOIN = "join"
     JOIN_FEATURE = "join_feature"
     TRACK_CHANGES = "track_changes"
     FORWARD_AGGREGATE = "forward_aggregate"
 
     # other operations
     ASSIGN = "assign"
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/graph.py` & `featurebyte-0.4.2/featurebyte/query_graph/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,20 @@
 from featurebyte.common.singleton import SingletonMeta
 from featurebyte.query_graph.enum import NodeType
 from featurebyte.query_graph.graph_node.base import GraphNode
 from featurebyte.query_graph.model.graph import Edge, GraphNodeNameMap, QueryGraphModel
 from featurebyte.query_graph.node import Node
 from featurebyte.query_graph.node.base import NodeT
 from featurebyte.query_graph.node.function import GenericFunctionNode
-from featurebyte.query_graph.node.generic import ForwardAggregateNode, GroupByNode, LookupNode
+from featurebyte.query_graph.node.generic import (
+    ForwardAggregateNode,
+    GroupByNode,
+    LookupNode,
+    LookupTargetNode,
+)
 from featurebyte.query_graph.node.input import InputNode
 from featurebyte.query_graph.node.metadata.operation import (
     DerivedDataColumn,
     OperationStructure,
     SourceDataColumn,
 )
 from featurebyte.query_graph.node.mixin import BaseGroupbyParameters
@@ -200,15 +205,15 @@
         """
         output = []
         target_node = self.get_node_by_name(node_name)
         for node in self.iterate_nodes(target_node=target_node, node_type=None):
             if isinstance(node.parameters, BaseGroupbyParameters):
                 if node.parameters.entity_ids:
                     output.extend(node.parameters.keys)
-            elif isinstance(node, LookupNode):
+            elif isinstance(node, (LookupNode, LookupTargetNode)):
                 output.append(node.parameters.entity_column)
         return sorted(set(output))
 
     def iterate_group_by_node_and_table_id_pairs(
         self, target_node: Node
     ) -> Iterator[Tuple[GroupByNode, Optional[ObjectId]]]:
         """
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/graph_node/base.py` & `featurebyte-0.4.2/featurebyte/query_graph/graph_node/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/model/column_info.py` & `featurebyte-0.4.2/featurebyte/query_graph/model/column_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/model/common_table.py` & `featurebyte-0.4.2/featurebyte/query_graph/model/common_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/model/critical_data_info.py` & `featurebyte-0.4.2/featurebyte/query_graph/model/critical_data_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/model/feature_job_setting.py` & `featurebyte-0.4.2/featurebyte/query_graph/model/feature_job_setting.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/model/graph.py` & `featurebyte-0.4.2/featurebyte/query_graph/model/graph.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/model/table.py` & `featurebyte-0.4.2/featurebyte/query_graph/model/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/__init__.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/agg_func.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/agg_func.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/base.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/binary.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/binary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/cleaning_operation.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/cleaning_operation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/count_dict.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/count_dict.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/date.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/date.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/function.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/function.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/generic.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,14 +552,15 @@
         )
         expression = get_object_class_from_function_call(
             callable_name=f"{grouped}.forward_aggregate",
             value_column=self.parameters.parent,
             method=self.parameters.agg_func,
             window=self.parameters.window,
             target_name=self.parameters.name,
+            skip_fill_na=True,
         )
         statements.append((out_var_name, expression))
         return statements, out_var_name
 
 
 class GroupByNode(AggregationOpStructMixin, BaseNode):
     """GroupByNode class"""
@@ -808,41 +809,41 @@
 
 class EventLookupParameters(BaseModel):
     """Parameters for EventTable lookup"""
 
     event_timestamp_column: InColumnStr
 
 
-class LookupNode(AggregationOpStructMixin, BaseNode):
-    """LookupNode class"""
+class LookupParameters(BaseModel):
+    """Lookup NOde Parameters"""
 
-    class Parameters(BaseModel):
-        """Parameters"""
+    input_column_names: List[InColumnStr]
+    feature_names: List[OutColumnStr]
+    entity_column: InColumnStr
+    serving_name: str
+    entity_id: PydanticObjectId
+    scd_parameters: Optional[SCDLookupParameters]
+    event_parameters: Optional[EventLookupParameters]
 
-        input_column_names: List[InColumnStr]
-        feature_names: List[OutColumnStr]
-        entity_column: InColumnStr
-        serving_name: str
-        entity_id: PydanticObjectId
-        scd_parameters: Optional[SCDLookupParameters]
-        event_parameters: Optional[EventLookupParameters]
-
-        @root_validator(skip_on_failure=True)
-        @classmethod
-        def _validate_input_column_names_feature_names_same_length(
-            cls, values: Dict[str, Any]
-        ) -> Dict[str, Any]:
-            input_column_names = values["input_column_names"]
-            feature_names = values["feature_names"]
-            assert len(input_column_names) == len(feature_names)
-            return values
+    @root_validator(skip_on_failure=True)
+    @classmethod
+    def _validate_input_column_names_feature_names_same_length(
+        cls, values: Dict[str, Any]
+    ) -> Dict[str, Any]:
+        input_column_names = values["input_column_names"]
+        feature_names = values["feature_names"]
+        assert len(input_column_names) == len(feature_names)
+        return values
+
+
+class BaseLookupNode(AggregationOpStructMixin, BaseNode):
+    """BaseLookupNode class"""
 
-    type: Literal[NodeType.LOOKUP] = Field(NodeType.LOOKUP, const=True)
     output_type: NodeOutputType = Field(NodeOutputType.FRAME, const=True)
-    parameters: Parameters
+    parameters: LookupParameters
 
     @property
     def max_input_count(self) -> int:
         return 1
 
     def _get_required_input_columns(
         self, input_index: int, available_column_names: List[str]
@@ -871,28 +872,34 @@
             AggregationColumn(
                 name=feature_name,
                 method=None,
                 keys=[self.parameters.entity_column],
                 window=None,
                 category=None,
                 column=name_to_column[input_column_name],
-                aggregation_type=self.type,
+                aggregation_type=self.type,  # type: ignore[arg-type]
                 node_names={node_name}.union(other_node_names),
                 node_name=node_name,
                 filter=any(col.filter for col in columns),
                 dtype=name_to_column[input_column_name].dtype,
             )
             for input_column_name, feature_name in zip(
                 self.parameters.input_column_names, self.parameters.feature_names
             )
         ]
 
     def _exclude_source_columns(self) -> List[str]:
         return [self.parameters.entity_column]
 
+
+class LookupNode(BaseLookupNode):
+    """LookupNode class"""
+
+    type: Literal[NodeType.LOOKUP] = Field(NodeType.LOOKUP, const=True)
+
     def _derive_sdk_code(
         self,
         node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
         context: CodeGenerationContext,
@@ -920,14 +927,27 @@
             node_output_category=operation_structure.output_category,
             node_name=self.name,
         )
         statements.append((out_var_name, ExpressionStr(grouped)))
         return statements, out_var_name
 
 
+class LookupTargetParameters(LookupParameters):
+    """LookupTargetParameters"""
+
+    offset: Optional[str]
+
+
+class LookupTargetNode(BaseLookupNode):
+    """LookupTargetNode class"""
+
+    type: Literal[NodeType.LOOKUP_TARGET] = Field(NodeType.LOOKUP_TARGET, const=True)
+    parameters: LookupTargetParameters
+
+
 class JoinMetadata(BaseModel):
     """Metadata to track general `view.join(...)` operation"""
 
     type: str = Field("join", const=True)
     rsuffix: str
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/input.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/input.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/metadata/column.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/metadata/column.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/metadata/operation.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/metadata/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,14 +349,15 @@
     aggregation_type: Literal[
         NodeType.GROUPBY,
         NodeType.ITEM_GROUPBY,
         NodeType.LOOKUP,
         NodeType.AGGREGATE_AS_AT,
         NodeType.REQUEST_COLUMN,
         NodeType.FORWARD_AGGREGATE,
+        NodeType.LOOKUP_TARGET,
     ]
     type: Literal[FeatureDataColumnType.AGGREGATION] = FeatureDataColumnType.AGGREGATION
 
     def __hash__(self) -> int:
         key = (
             *self._get_hash_key(),
             self.type,
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/metadata/sdk_code.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/metadata/sdk_code.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/mixin.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/nested.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/nested.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/request.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/request.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/scalar.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/scalar.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/schema.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/schema.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/string.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/unary.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/unary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/node/validator.py` & `featurebyte-0.4.2/featurebyte/query_graph/node/validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/pruning_util.py` & `featurebyte-0.4.2/featurebyte/query_graph/pruning_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/adapter/__init__.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/adapter/base.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/adapter/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/adapter/databricks.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/adapter/databricks.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/adapter/snowflake.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/adapter/spark.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/adapter/spark.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/asat.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/asat.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/base.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/forward.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/forward.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/item.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/item.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/latest.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/latest.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/lookup.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/base_lookup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 """
 SQL generation for lookup features
 """
 from __future__ import annotations
 
-from typing import Any, Iterable, Optional, Sequence, Tuple
+from typing import Any, Iterable, Optional, Sequence, Tuple, TypeVar
 
+from abc import abstractmethod
 from dataclasses import dataclass
 
+import pandas as pd
 from sqlglot import expressions
 from sqlglot.expressions import Select, alias_, select
 
 from featurebyte.enum import SpecialColumnName
+from featurebyte.query_graph.node.generic import SCDLookupParameters
+from featurebyte.query_graph.sql.adapter import BaseAdapter
 from featurebyte.query_graph.sql.aggregator.base import (
     AggregationResult,
     LeftJoinableSubquery,
     NonTileBasedAggregator,
 )
+from featurebyte.query_graph.sql.ast.literal import make_literal_value
 from featurebyte.query_graph.sql.common import (
     CteStatements,
     get_qualified_column_identifier,
     quoted_identifier,
 )
-from featurebyte.query_graph.sql.scd_helper import Table, get_scd_join_expr
-from featurebyte.query_graph.sql.specs import LookupSpec
+from featurebyte.query_graph.sql.scd_helper import Table
+from featurebyte.query_graph.sql.specifications.base_lookup import BaseLookupSpec
 
 
 @dataclass
 class SubqueryWithPointInTimeCutoff(LeftJoinableSubquery):
     """
     SubqueryWithPointInTimeCutoff for lookup features
     """
 
     event_timestamp_column: Optional[str]
+    forward_point_in_time_offset: Optional[str]
+    adapter: BaseAdapter
 
     def get_expression_for_column(
         self, main_alias: str, join_alias: str, column_name: str
     ) -> expressions.Expression:
         expr = super().get_expression_for_column(
             main_alias=main_alias, join_alias=join_alias, column_name=column_name
         )
@@ -43,14 +50,24 @@
         # For lookup from EventData, set the looked up value to NA if the point in time is prior to
         # the event timestamp
         if self.event_timestamp_column is not None:
             point_in_time_expr = get_qualified_column_identifier(
                 SpecialColumnName.POINT_IN_TIME,
                 main_alias,
             )
+
+            # Add the forward point in time offset to the point in time if it is present.
+            if self.forward_point_in_time_offset is not None:
+                point_in_time_expr = self.adapter.dateadd_microsecond(
+                    make_literal_value(
+                        pd.Timedelta(self.forward_point_in_time_offset).total_seconds() * 1e6
+                    ),
+                    point_in_time_expr,
+                )
+
             event_timestamp_expr = get_qualified_column_identifier(
                 self.event_timestamp_column,
                 join_alias,
                 quote_table=True,
             )
             is_point_in_time_prior_to_event_timestamp = expressions.LT(
                 this=point_in_time_expr, expression=event_timestamp_expr
@@ -59,41 +76,44 @@
                 this=is_point_in_time_prior_to_event_timestamp, true=expressions.null()
             )
             expr = expressions.Case(ifs=[if_expr], default=expr)
 
         return expr
 
 
-class LookupAggregator(NonTileBasedAggregator[LookupSpec]):
+LookupSpecT = TypeVar("LookupSpecT", bound=BaseLookupSpec)
+
+
+class BaseLookupAggregator(NonTileBasedAggregator[LookupSpecT]):
     """
     LookupAggregator is responsible for generating SQL for lookup features
     """
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.is_parent_lookup = False
 
     @property
-    def lookup_specs(self) -> Iterable[LookupSpec]:
+    def lookup_specs(self) -> Iterable[LookupSpecT]:
         """
         Yields a list of LookupSpec recorded
 
         Yields
         ------
         LookupSpec
             Instance of LookupSpec
         """
         for specs in self.grouped_specs.values():
             yield from specs
 
-    def additional_update(self, aggregation_spec: LookupSpec) -> None:
+    def additional_update(self, aggregation_spec: LookupSpecT) -> None:
         if aggregation_spec.is_parent_lookup:
             self.is_parent_lookup = True
 
-    def iterate_grouped_lookup_specs(self, is_scd: bool) -> Iterable[list[LookupSpec]]:
+    def iterate_grouped_lookup_specs(self, is_scd: bool) -> Iterable[list[LookupSpecT]]:
         """
         Iterate over groups of LookupSpec filtering by time awareness. All the LookupSpecs in a
         group can be looked up using the same join.
 
         Parameters
         ----------
         is_scd: bool
@@ -119,14 +139,32 @@
                 requires_scd_join = False
 
             if is_scd and requires_scd_join:
                 yield specs
             if not is_scd and not requires_scd_join:
                 yield specs
 
+    def get_forward_point_in_time_offset(  # pylint: disable=useless-return
+        self, base_lookup_spec: LookupSpecT
+    ) -> Optional[str]:
+        """
+        Get the forward point in time offset for the lookup if it is provided.
+
+        Parameters
+        ----------
+        base_lookup_spec: LookupSpecT
+            LookupSpec
+
+        Returns
+        -------
+        Optional[str]
+        """
+        _ = base_lookup_spec
+        return None
+
     def get_direct_lookups(self) -> Sequence[LeftJoinableSubquery]:
         """
         Get simple lookup queries without time based conditions
 
         This includes SCD lookups during online serving when the current flag column is available.
 
         Returns
@@ -160,14 +198,16 @@
                 event_timestamp_column = None
 
             result = SubqueryWithPointInTimeCutoff(
                 expr=agg_expr,
                 column_names=[spec.agg_result_name for spec in specs],
                 join_keys=[serving_name],
                 event_timestamp_column=event_timestamp_column,
+                forward_point_in_time_offset=self.get_forward_point_in_time_offset(specs[0]),
+                adapter=self.adapter,
             )
             out.append(result)
 
         return out
 
     def update_aggregation_table_expr(
         self,
@@ -198,14 +238,36 @@
             # already done for the SCD case.
             result.updated_table_expr = self._wrap_in_nested_query(
                 table_expr=result.updated_table_expr, columns=current_columns + result.column_names
             )
 
         return result
 
+    @abstractmethod
+    def get_scd_join_expr_for_lookup(
+        self, left_table: Table, right_table: Table, scd_parameters: SCDLookupParameters
+    ) -> Select:
+        """
+        Returns the SQL expression for the SCD join
+
+        Parameters
+        ----------
+        left_table: Table
+            The left table to join
+        right_table: Table
+            The right table to join
+        scd_parameters: SCDLookupParameters
+            The SCD lookup parameters
+
+        Returns
+        -------
+        Select
+            The SQL expression for the SCD join
+        """
+
     def _update_with_scd_lookups(
         self,
         table_expr: Select,
         point_in_time_column: str,
         current_columns: list[str],
     ) -> Tuple[Select, list[str]]:
         """
@@ -243,20 +305,18 @@
             right_table = Table(
                 expr=lookup_specs[0].source_expr,
                 timestamp_column=scd_parameters.effective_timestamp_column,
                 join_keys=[lookup_specs[0].entity_column],
                 input_columns=[spec.input_column_name for spec in lookup_specs],
                 output_columns=agg_result_names,
             )
-            table_expr = get_scd_join_expr(
+            table_expr = self.get_scd_join_expr_for_lookup(
                 left_table,
                 right_table,
-                join_type="left",
-                adapter=self.adapter,
-                offset=scd_parameters.offset,
+                scd_parameters,
             )
 
             current_columns = current_columns + agg_result_names
             scd_agg_result_names.extend(agg_result_names)
 
         if scd_agg_result_names:
             table_expr = self._wrap_in_nested_query(table_expr=table_expr, columns=current_columns)
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/request_table.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/aggregator/window.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/aggregator/window.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/aggregate.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/aggregate.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 from dataclasses import dataclass
 
 from sqlglot.expressions import Expression, Select
 
 from featurebyte.query_graph.enum import NodeType
 from featurebyte.query_graph.sql.ast.base import SQLNodeContext, TableNode
 from featurebyte.query_graph.sql.common import SQLType, quoted_identifier
+from featurebyte.query_graph.sql.specifications.lookup import LookupSpec
+from featurebyte.query_graph.sql.specifications.lookup_target import LookupTargetSpec
 from featurebyte.query_graph.sql.specs import (
     AggregateAsAtSpec,
     AggregationSource,
     ForwardAggregateSpec,
     ItemAggregationSpec,
-    LookupSpec,
 )
 
 
 @dataclass  # type: ignore[misc]
 class Aggregate(TableNode):
     """
     Aggregate SQLNode
@@ -138,14 +139,37 @@
             context.query_node,
             aggregation_source=Aggregate.get_aggregation_source_from_source_node(source_node),
         )
         for spec in specs:
             columns_map[spec.feature_name] = quoted_identifier(spec.agg_result_name)
         return columns_map
 
+
+@dataclass
+class LookupTarget(Aggregate):
+    """
+    LookupTarget SQLNode
+    """
+
+    query_node_type = NodeType.LOOKUP_TARGET
+
+    @staticmethod
+    def construct_columns_map(
+        context: SQLNodeContext, source_node: TableNode
+    ) -> dict[str, Expression]:
+        # Create LookupTargetSpec which determines the internal aggregated result names
+        columns_map = {}
+        specs = LookupTargetSpec.from_query_graph_node(
+            context.query_node,
+            aggregation_source=Aggregate.get_aggregation_source_from_source_node(source_node),
+        )
+        for spec in specs:
+            columns_map[spec.feature_name] = quoted_identifier(spec.agg_result_name)
+        return columns_map
+
 
 @dataclass
 class AsAt(Aggregate):
     """
     AsAt SQLNode
     """
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/base.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/binary.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/binary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/count_dict.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/count_dict.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/datetime.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/datetime.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/function.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/function.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/generic.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/generic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/groupby.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/groupby.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/input.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/input.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/is_in.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/is_in.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/join.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/join.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/join_feature.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/join_feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/literal.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/literal.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/request.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/request.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/string.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/tile.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/tile.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/track_changes.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/track_changes.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/unary.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/unary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/ast/util.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/ast/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/builder.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/builder.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/common.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/common.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/dataframe.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/expression.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/expression.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/feature_compute.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/feature_compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,42 +17,45 @@
 from featurebyte.query_graph.sql.adapter import get_sql_adapter
 from featurebyte.query_graph.sql.aggregator.asat import AsAtAggregator
 from featurebyte.query_graph.sql.aggregator.base import TileBasedAggregator
 from featurebyte.query_graph.sql.aggregator.forward import ForwardAggregator
 from featurebyte.query_graph.sql.aggregator.item import ItemAggregator
 from featurebyte.query_graph.sql.aggregator.latest import LatestAggregator
 from featurebyte.query_graph.sql.aggregator.lookup import LookupAggregator
+from featurebyte.query_graph.sql.aggregator.lookup_target import LookupTargetAggregator
 from featurebyte.query_graph.sql.aggregator.window import WindowAggregator
 from featurebyte.query_graph.sql.ast.base import TableNode
 from featurebyte.query_graph.sql.ast.generic import AliasNode, Project
 from featurebyte.query_graph.sql.builder import SQLOperationGraph
 from featurebyte.query_graph.sql.common import (
     CteStatement,
     CteStatements,
     SQLType,
     construct_cte_sql,
     quoted_identifier,
 )
 from featurebyte.query_graph.sql.parent_serving import construct_request_table_with_parent_entities
+from featurebyte.query_graph.sql.specifications.lookup import LookupSpec
+from featurebyte.query_graph.sql.specifications.lookup_target import LookupTargetSpec
 from featurebyte.query_graph.sql.specs import (
     AggregateAsAtSpec,
     AggregationSpec,
     AggregationType,
     FeatureSpec,
     ForwardAggregateSpec,
     ItemAggregationSpec,
-    LookupSpec,
     NonTileBasedAggregationSpec,
     TileBasedAggregationSpec,
 )
 from featurebyte.query_graph.transform.flattening import GraphFlatteningTransformer
 
 AggregatorType = Union[
     LatestAggregator,
     LookupAggregator,
+    LookupTargetAggregator,
     WindowAggregator,
     ItemAggregator,
     AsAtAggregator,
     ForwardAggregator,
 ]
 AggregationSpecType = Union[TileBasedAggregationSpec, NonTileBasedAggregationSpec]
 
@@ -68,14 +71,15 @@
         is_online_serving: bool,
         parent_serving_preparation: ParentServingPreparation | None = None,
     ) -> None:
         aggregator_kwargs = {"source_type": source_type, "is_online_serving": is_online_serving}
         self.aggregators: dict[str, AggregatorType] = {
             AggregationType.LATEST: LatestAggregator(**aggregator_kwargs),
             AggregationType.LOOKUP: LookupAggregator(**aggregator_kwargs),
+            AggregationType.LOOKUP_TARGET: LookupTargetAggregator(**aggregator_kwargs),
             AggregationType.WINDOW: WindowAggregator(**aggregator_kwargs),
             AggregationType.ITEM: ItemAggregator(**aggregator_kwargs),
             AggregationType.AS_AT: AsAtAggregator(**aggregator_kwargs),
             AggregationType.FORWARD: ForwardAggregator(**aggregator_kwargs),
         }
         self.feature_specs: dict[str, FeatureSpec] = {}
         self.adapter = get_sql_adapter(source_type)
@@ -468,14 +472,15 @@
         Returns
         -------
         AggregationSpec
         """
         groupby_nodes = list(self.graph.iterate_nodes(node, NodeType.GROUPBY))
         item_groupby_nodes = list(self.graph.iterate_nodes(node, NodeType.ITEM_GROUPBY))
         lookup_nodes = list(self.graph.iterate_nodes(node, NodeType.LOOKUP))
+        lookup_target_nodes = list(self.graph.iterate_nodes(node, NodeType.LOOKUP_TARGET))
         asat_nodes = list(self.graph.iterate_nodes(node, NodeType.AGGREGATE_AS_AT))
         forward_aggregate_nodes = list(self.graph.iterate_nodes(node, NodeType.FORWARD_AGGREGATE))
 
         out: list[AggregationSpecType] = []
         if groupby_nodes:
             # Feature involves window aggregations. In this case, tiling applies. Even if
             # ITEM_GROUPBY nodes are involved, their results would have already been incorporated in
@@ -488,14 +493,18 @@
             for item_groupby_node in item_groupby_nodes:
                 out.extend(self.get_non_tiling_specs(ItemAggregationSpec, item_groupby_node))
 
         if lookup_nodes:
             for lookup_node in lookup_nodes:
                 out.extend(self.get_non_tiling_specs(LookupSpec, lookup_node))
 
+        if lookup_target_nodes:
+            for lookup_node in lookup_target_nodes:
+                out.extend(self.get_non_tiling_specs(LookupTargetSpec, lookup_node))
+
         if asat_nodes:
             for asat_node in asat_nodes:
                 out.extend(self.get_non_tiling_specs(AggregateAsAtSpec, asat_node))
 
         if forward_aggregate_nodes:
             for forward_aggregate_node in forward_aggregate_nodes:
                 out.extend(self.get_non_tiling_specs(ForwardAggregateSpec, forward_aggregate_node))
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/feature_historical.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/feature_historical.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/feature_preview.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/feature_preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/groupby_helper.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/groupby_helper.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/interpreter/base.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/interpreter/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/interpreter/preview.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/interpreter/preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/interpreter/tile.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/interpreter/tile.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/materialisation.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/materialisation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/online_serving.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/online_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/online_serving_util.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/online_serving_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/online_store_compute_query.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/online_store_compute_query.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/parent_serving.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/parent_serving.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from featurebyte.models.parent_serving import JoinStep
 from featurebyte.query_graph.graph import QueryGraph
 from featurebyte.query_graph.node.generic import EventLookupParameters, SCDLookupParameters
 from featurebyte.query_graph.node.schema import FeatureStoreDetails
 from featurebyte.query_graph.sql.aggregator.lookup import LookupAggregator
 from featurebyte.query_graph.sql.builder import SQLOperationGraph
 from featurebyte.query_graph.sql.common import SQLType, get_qualified_column_identifier
-from featurebyte.query_graph.sql.specs import AggregationSource, LookupSpec
+from featurebyte.query_graph.sql.specifications.lookup import LookupSpec
+from featurebyte.query_graph.sql.specs import AggregationSource
 
 
 @dataclass
 class ParentEntityLookupResult:
     """
     Result of updating a request table with parent entities
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/scd_helper.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/scd_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from dataclasses import dataclass
 
 import pandas as pd
 from sqlglot import expressions, parse_one
 from sqlglot.expressions import Expression, Select, alias_, select
 
+from featurebyte.enum import StrEnum
 from featurebyte.query_graph.sql.adapter import BaseAdapter
 from featurebyte.query_graph.sql.ast.literal import make_literal_value
 from featurebyte.query_graph.sql.common import get_qualified_column_identifier, quoted_identifier
 
 # Internally used identifiers when constructing SQL
 TS_COL = "__FB_TS_COL"
 EFFECTIVE_TS_COL = "__FB_EFFECTIVE_TS_COL"
@@ -70,21 +71,31 @@
         """
         if isinstance(self.expr, str):
             return expressions.Table(this=expressions.Identifier(this=self.expr), alias=alias)
         assert isinstance(self.expr, Select)
         return cast(Expression, self.expr.subquery(alias=alias))
 
 
+class OffsetDirection(StrEnum):
+    """
+    Offset direction
+    """
+
+    FORWARD = "forward"
+    BACKWARD = "backward"
+
+
 def get_scd_join_expr(
     left_table: Table,
     right_table: Table,
     join_type: Literal["inner", "left"],
     adapter: BaseAdapter,
     select_expr: Optional[Select] = None,
     offset: Optional[str] = None,
+    offset_direction: OffsetDirection = OffsetDirection.BACKWARD,
     allow_exact_match: bool = True,
     quote_right_input_columns: bool = True,
     convert_timestamps_to_utc: bool = True,
 ) -> Select:
     """
     Construct a query to perform SCD join
 
@@ -103,14 +114,16 @@
         Join type
     adapter: BaseAdapter
         Instance of BaseAdapter for engine specific sql generation
     select_expr: Optional[Select]
         Partially constructed select expression, if any
     offset: Optional[str]
         Offset to apply when performing SCD join
+    offset_direction: OffsetDirection
+        Direction of offset
     allow_exact_match: bool
         Whether to allow exact matching effective timestamps to be joined
     quote_right_input_columns: bool
         Whether to quote right table's input columns. Temporary and should be removed after
         https://featurebyte.atlassian.net/browse/DEV-935
     convert_timestamps_to_utc: bool
         Whether timestamps should be converted to UTC for joins
@@ -144,14 +157,15 @@
         )
 
     left_view_with_last_ts_expr = augment_table_with_effective_timestamp(
         left_table=left_table,
         right_table=right_table,
         adapter=adapter,
         offset=offset,
+        offset_direction=offset_direction,
         allow_exact_match=allow_exact_match,
         convert_timestamps_to_utc=convert_timestamps_to_utc,
     )
 
     left_subquery = left_view_with_last_ts_expr.subquery(alias="L")
     right_subquery = right_table.as_subquery(alias="R")
     assert isinstance(right_table.timestamp_column, str)
@@ -187,19 +201,20 @@
     -------
     expressions.Expression
     """
     utc_ts_expr = adapter.convert_to_utc_timestamp(col_expr)
     return expressions.Cast(this=utc_ts_expr, to=parse_one("TIMESTAMP"))
 
 
-def augment_table_with_effective_timestamp(
+def augment_table_with_effective_timestamp(  # pylint: disable=too-many-locals
     left_table: Table,
     right_table: Table,
     adapter: BaseAdapter,
     offset: Optional[str],
+    offset_direction: OffsetDirection,
     allow_exact_match: bool = True,
     convert_timestamps_to_utc: bool = True,
 ) -> Select:
     """
     This constructs a query that calculates the corresponding SCD effective date for each row in the
     left table. See an example below.
 
@@ -245,28 +260,31 @@
         Left table
     right_table: Table
         Right table, usually the SCD table
     adapter: BaseAdapter
         Instance of BaseAdapter for engine specific sql generation
     offset: Optional[str]
         Offset to apply when performing SCD join
+    offset_direction: OffsetDirection
+        Direction of offset
     allow_exact_match: bool
         Whether to allow exact matching effective timestamps to be joined
     convert_timestamps_to_utc: bool
         Whether timestamps should be converted to UTC for joins
 
     Returns
     -------
     Select
     """
     # Adjust left timestamps if offset is provided
     if offset:
         offset_seconds = pd.Timedelta(offset).total_seconds()
+        direction_adjustment_multiplier = -1 if offset_direction == OffsetDirection.BACKWARD else 1
         left_ts_col = adapter.dateadd_microsecond(
-            make_literal_value(offset_seconds * 1e6 * -1),
+            make_literal_value(offset_seconds * 1e6 * direction_adjustment_multiplier),
             left_table.timestamp_column_expr,
         )
     else:
         left_ts_col = left_table.timestamp_column_expr
     right_ts_col = right_table.timestamp_column_expr
     if convert_timestamps_to_utc:
         left_ts_col = _convert_to_utc_ntz(left_ts_col, adapter)
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/specs.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/specs.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,22 +17,19 @@
 from featurebyte.enum import DBVarType, SourceType, StrEnum
 from featurebyte.query_graph.enum import NodeOutputType, NodeType
 from featurebyte.query_graph.model.graph import QueryGraphModel
 from featurebyte.query_graph.node import Node
 from featurebyte.query_graph.node.generic import (
     AggregateAsAtNode,
     AggregateAsAtParameters,
-    EventLookupParameters,
     ForwardAggregateNode,
     ForwardAggregateParameters,
     GroupByNode,
     ItemGroupbyNode,
     ItemGroupbyParameters,
-    LookupNode,
-    SCDLookupParameters,
 )
 from featurebyte.query_graph.node.mixin import BaseGroupbyParameters
 from featurebyte.query_graph.sql.adapter import BaseAdapter
 from featurebyte.query_graph.sql.common import apply_serving_names_mapping
 from featurebyte.query_graph.sql.tiling import InputColumn, get_aggregator
 from featurebyte.query_graph.transform.operation_structure import OperationStructureExtractor
 from featurebyte.query_graph.transform.pruning import prune_query_graph
@@ -48,14 +45,15 @@
     """
     Enum for different aggregation types. Will be used as the dictionary key in a container for
     aggregators held by FeatureExecutionPlan.
     """
 
     LATEST = "latest"
     LOOKUP = "lookup"
+    LOOKUP_TARGET = "lookup_target"
     WINDOW = "window"
     ITEM = "item"
     AS_AT = "as_at"
     FORWARD = "forward"
 
 
 @dataclass  # type: ignore[misc]
@@ -609,103 +607,14 @@
                 serving_names=node.parameters.serving_names,
                 serving_names_mapping=serving_names_mapping,
             )
         ]
 
 
 @dataclass
-class LookupSpec(NonTileBasedAggregationSpec):
-    """
-    LookupSpec contains all information required to generate sql for a lookup feature
-    """
-
-    input_column_name: str
-    feature_name: str
-    entity_column: str
-    serving_names: list[str]
-    scd_parameters: Optional[SCDLookupParameters]
-    event_parameters: Optional[EventLookupParameters]
-    is_parent_lookup: bool = False
-
-    @property
-    def agg_result_name(self) -> str:
-        if self.is_parent_lookup:
-            return self.feature_name
-        return self.construct_agg_result_name(self.input_column_name)
-
-    @property
-    def aggregation_type(self) -> AggregationType:
-        return AggregationType.LOOKUP
-
-    def get_source_hash_parameters(self) -> dict[str, Any]:
-        params: dict[str, Any] = {
-            "source_expr": self.source_expr.sql(),
-            "entity_column": self.entity_column,
-        }
-        if self.scd_parameters is not None:
-            params["scd_parameters"] = self.scd_parameters.dict()
-        if self.event_parameters is not None:
-            params["event_parameters"] = self.event_parameters.dict()
-        return params
-
-    @classmethod
-    def should_filter_scd_by_current_flag(cls, graph: QueryGraphModel, node: Node) -> bool:
-        assert isinstance(node, LookupNode)
-        scd_parameters = node.parameters.scd_parameters
-        if scd_parameters is not None:
-            return cls.get_scd_filter_flag_from_scd_parameters(scd_parameters)
-        return False
-
-    @staticmethod
-    def get_scd_filter_flag_from_scd_parameters(scd_parameters: SCDLookupParameters) -> bool:
-        """
-        Returns whether the current flag should be used to filter SCD join
-
-        Parameters
-        ----------
-        scd_parameters: SCDLookupParameters
-            SCD related parameters in the lookup node
-
-        Returns
-        -------
-        bool
-        """
-        # Online serving might not have to use SCD join if current flag is applicable
-        current_flag_usable_for_online_serving = (
-            scd_parameters.current_flag_column is not None and scd_parameters.offset is None
-        )
-        return current_flag_usable_for_online_serving
-
-    @classmethod
-    def construct_specs(
-        cls,
-        node: Node,
-        aggregation_source: AggregationSource,
-        serving_names_mapping: Optional[dict[str, str]],
-    ) -> list[LookupSpec]:
-        assert isinstance(node, LookupNode)
-        params = node.parameters
-        specs = []
-        for input_column_name, feature_name in zip(params.input_column_names, params.feature_names):
-            spec = LookupSpec(
-                input_column_name=input_column_name,
-                feature_name=feature_name,
-                entity_column=params.entity_column,
-                entity_ids=[params.entity_id],
-                serving_names=[params.serving_name],
-                serving_names_mapping=serving_names_mapping,
-                aggregation_source=aggregation_source,
-                scd_parameters=params.scd_parameters,
-                event_parameters=params.event_parameters,
-            )
-            specs.append(spec)
-        return specs
-
-
-@dataclass
 class ForwardAggregateSpec(NonTileBasedAggregationSpec):
     """
     ForwardAggregateSpec contains all information required to generate sql for a forward aggregate target.
     """
 
     parameters: ForwardAggregateParameters
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/template.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/template.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/tile_compute.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/tile_compute.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/tile_util.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/tile_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/sql/tiling.py` & `featurebyte-0.4.2/featurebyte/query_graph/sql/tiling.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/transform/base.py` & `featurebyte-0.4.2/featurebyte/query_graph/transform/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 class BaseGraphExtractor(Generic[OutputT, BranchStateT, GlobalStateT]):
     """BaseGraphExtractor encapsulates the logic to perform backtracking from a target node."""
 
     def __init__(self, graph: QueryGraphT):
         self.graph = graph
+        self._input_node_map_cache: Dict[str, OutputT] = {}
 
     @abstractmethod
     def _pre_compute(
         self,
         branch_state: BranchStateT,
         global_state: GlobalStateT,
         node: Node,
@@ -113,27 +114,29 @@
             node=node,
             input_node_names=self.graph.get_input_node_names(node),
         )
         input_node_map: Dict[str, Any] = {}
         for input_node_name in sorted(
             input_node_names, key=lambda x: topological_order_map[x], reverse=True
         ):
-            input_node = self.graph.nodes_map[input_node_name]
-            branch_state = self._in_compute(
-                branch_state=branch_state,
-                global_state=global_state,
-                node=node,
-                input_node=input_node,
-            )
-            input_node_map[input_node_name] = self._extract(
-                node=input_node,
-                branch_state=branch_state,
-                global_state=global_state,
-                topological_order_map=topological_order_map,
-            )
+            if input_node_name not in self._input_node_map_cache:
+                input_node = self.graph.nodes_map[input_node_name]
+                branch_state = self._in_compute(
+                    branch_state=branch_state,
+                    global_state=global_state,
+                    node=node,
+                    input_node=input_node,
+                )
+                self._input_node_map_cache[input_node_name] = self._extract(
+                    node=input_node,
+                    branch_state=branch_state,
+                    global_state=global_state,
+                    topological_order_map=topological_order_map,
+                )
+            input_node_map[input_node_name] = self._input_node_map_cache[input_node_name]
 
         return self._post_compute(
             branch_state=branch_state,
             global_state=global_state,
             node=node,
             inputs=[input_node_map[node_name] for node_name in input_node_names],
             skip_post=skip_post,
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/transform/entity_extractor.py` & `featurebyte-0.4.2/featurebyte/query_graph/transform/entity_extractor.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, List, Set, Tuple
 
 from dataclasses import dataclass, field
 
 from bson import ObjectId
 
 from featurebyte.query_graph.node import Node
-from featurebyte.query_graph.node.generic import LookupNode
+from featurebyte.query_graph.node.generic import LookupNode, LookupTargetNode
 from featurebyte.query_graph.node.mixin import BaseGroupbyParameters
 from featurebyte.query_graph.transform.base import BaseGraphExtractor
 
 
 class EntityExtractorBranchState:
     """EntityExtractorBranchState class"""
 
@@ -40,15 +40,15 @@
     ) -> Tuple[List[str], bool]:
         skip_input_nodes = False
         if isinstance(node.parameters, BaseGroupbyParameters):
             # if groupby node has entity_ids, skip further exploration on input nodes
             if node.parameters.entity_ids:
                 global_state.entity_ids.update(node.parameters.entity_ids)
             skip_input_nodes = True
-        elif isinstance(node, LookupNode):
+        elif isinstance(node, (LookupNode, LookupTargetNode)):
             global_state.entity_ids.add(node.parameters.entity_id)
         return [] if skip_input_nodes else input_node_names, False
 
     def _in_compute(
         self,
         branch_state: EntityExtractorBranchState,
         global_state: EntityExtractorGlobalState,
```

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/transform/flattening.py` & `featurebyte-0.4.2/featurebyte/query_graph/transform/flattening.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/transform/operation_structure.py` & `featurebyte-0.4.2/featurebyte/query_graph/transform/operation_structure.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/transform/pruning.py` & `featurebyte-0.4.2/featurebyte/query_graph/transform/pruning.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/transform/quick_pruning.py` & `featurebyte-0.4.2/featurebyte/query_graph/transform/quick_pruning.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/transform/reconstruction.py` & `featurebyte-0.4.2/featurebyte/query_graph/transform/reconstruction.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/transform/sdk_code.py` & `featurebyte-0.4.2/featurebyte/query_graph/transform/sdk_code.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/query_graph/util.py` & `featurebyte-0.4.2/featurebyte/query_graph/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/app_container_config.py` & `featurebyte-0.4.2/featurebyte/routes/app_container_config.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/batch_feature_table/api.py` & `featurebyte-0.4.2/featurebyte/routes/batch_feature_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/batch_feature_table/controller.py` & `featurebyte-0.4.2/featurebyte/routes/batch_feature_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/batch_request_table/api.py` & `featurebyte-0.4.2/featurebyte/routes/batch_request_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/batch_request_table/controller.py` & `featurebyte-0.4.2/featurebyte/routes/batch_request_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/catalog/api.py` & `featurebyte-0.4.2/featurebyte/routes/catalog/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/catalog/catalog_name_injector.py` & `featurebyte-0.4.2/featurebyte/routes/catalog/catalog_name_injector.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/catalog/controller.py` & `featurebyte-0.4.2/featurebyte/routes/catalog/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/common/base.py` & `featurebyte-0.4.2/featurebyte/routes/common/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/common/base_materialized_table.py` & `featurebyte-0.4.2/featurebyte/routes/common/base_materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/common/base_table.py` & `featurebyte-0.4.2/featurebyte/routes/common/base_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/common/feature_metadata_extractor.py` & `featurebyte-0.4.2/featurebyte/routes/common/feature_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/common/feature_or_target_table.py` & `featurebyte-0.4.2/featurebyte/routes/common/feature_or_target_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/common/schema.py` & `featurebyte-0.4.2/featurebyte/routes/common/schema.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/context/api.py` & `featurebyte-0.4.2/featurebyte/routes/context/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/context/controller.py` & `featurebyte-0.4.2/featurebyte/routes/context/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/credential/api.py` & `featurebyte-0.4.2/featurebyte/routes/credential/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/credential/controller.py` & `featurebyte-0.4.2/featurebyte/routes/credential/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/deployment/api.py` & `featurebyte-0.4.2/featurebyte/routes/deployment/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/deployment/controller.py` & `featurebyte-0.4.2/featurebyte/routes/deployment/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/dimension_table/api.py` & `featurebyte-0.4.2/featurebyte/routes/dimension_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/dimension_table/controller.py` & `featurebyte-0.4.2/featurebyte/routes/dimension_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/entity/api.py` & `featurebyte-0.4.2/featurebyte/routes/entity/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/entity/controller.py` & `featurebyte-0.4.2/featurebyte/routes/entity/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/event_table/api.py` & `featurebyte-0.4.2/featurebyte/routes/event_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/event_table/controller.py` & `featurebyte-0.4.2/featurebyte/routes/event_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature/api.py` & `featurebyte-0.4.2/featurebyte/routes/feature/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature/controller.py` & `featurebyte-0.4.2/featurebyte/routes/feature/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature_job_setting_analysis/api.py` & `featurebyte-0.4.2/featurebyte/routes/feature_job_setting_analysis/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature_job_setting_analysis/controller.py` & `featurebyte-0.4.2/featurebyte/routes/feature_job_setting_analysis/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature_list/api.py` & `featurebyte-0.4.2/featurebyte/routes/feature_list/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature_list/controller.py` & `featurebyte-0.4.2/featurebyte/routes/feature_list/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature_list_namespace/api.py` & `featurebyte-0.4.2/featurebyte/routes/feature_list_namespace/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature_list_namespace/controller.py` & `featurebyte-0.4.2/featurebyte/routes/feature_list_namespace/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature_namespace/api.py` & `featurebyte-0.4.2/featurebyte/routes/feature_namespace/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature_namespace/controller.py` & `featurebyte-0.4.2/featurebyte/routes/feature_namespace/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from featurebyte.models.feature_namespace import DefaultVersionMode, FeatureReadiness
 from featurebyte.routes.catalog.catalog_name_injector import CatalogNameInjector
 from featurebyte.routes.common.base import (
     BaseDocumentController,
     DerivePrimaryEntityHelper,
     PaginatedDocument,
 )
+from featurebyte.routes.common.feature_or_target_helper import FeatureOrTargetHelper
 from featurebyte.schema.feature_namespace import (
     FeatureNamespaceList,
     FeatureNamespaceModelResponse,
     FeatureNamespaceServiceUpdate,
     FeatureNamespaceUpdate,
 )
 from featurebyte.schema.info import EntityBriefInfoList, FeatureNamespaceInfo, TableBriefInfoList
@@ -49,23 +50,25 @@
         entity_service: EntityService,
         feature_service: FeatureService,
         default_version_mode_service: DefaultVersionModeService,
         feature_readiness_service: FeatureReadinessService,
         table_service: TableService,
         derive_primary_entity_helper: DerivePrimaryEntityHelper,
         catalog_name_injector: CatalogNameInjector,
+        feature_or_target_helper: FeatureOrTargetHelper,
     ):
         super().__init__(feature_namespace_service)
         self.entity_service = entity_service
         self.feature_service = feature_service
         self.default_version_mode_service = default_version_mode_service
         self.feature_readiness_service = feature_readiness_service
         self.table_service = table_service
         self.derive_primary_entity_helper = derive_primary_entity_helper
         self.catalog_name_injector = catalog_name_injector
+        self.feature_or_target_helper = feature_or_target_helper
 
     async def get(
         self,
         document_id: ObjectId,
         exception_detail: str | None = None,
     ) -> Document:
         document = await self.service.get_document(
@@ -236,18 +239,21 @@
         # Add catalog name to entities and tables
         catalog_name, updated_docs = await self.catalog_name_injector.add_name(
             namespace.catalog_id, [entities, tables]
         )
         entities, tables = updated_docs
 
         # derive primary tables
-        table_id_to_doc = {table["_id"]: table for table in tables["data"]}
         feature = await self.feature_service.get_document(document_id=namespace.default_feature_id)
-        primary_input_nodes = feature.graph.get_primary_input_nodes(node_name=feature.node_name)
-        primary_tables = [table_id_to_doc[node.parameters.id] for node in primary_input_nodes]
+        primary_tables = await self.feature_or_target_helper.get_primary_tables(
+            namespace.table_ids,
+            namespace.catalog_id,
+            feature.graph,
+            feature.node_name,
+        )
 
         return FeatureNamespaceInfo(
             name=namespace.name,
             created_at=namespace.created_at,
             updated_at=namespace.updated_at,
             entities=EntityBriefInfoList.from_paginated_data(entities),
             primary_entity=EntityBriefInfoList.from_paginated_data(primary_entity),
```

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature_store/api.py` & `featurebyte-0.4.2/featurebyte/routes/feature_store/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/feature_store/controller.py` & `featurebyte-0.4.2/featurebyte/routes/feature_store/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/historical_feature_table/api.py` & `featurebyte-0.4.2/featurebyte/routes/historical_feature_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/historical_feature_table/controller.py` & `featurebyte-0.4.2/featurebyte/routes/historical_feature_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/item_table/api.py` & `featurebyte-0.4.2/featurebyte/routes/item_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/item_table/controller.py` & `featurebyte-0.4.2/featurebyte/routes/item_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/lazy_app_container.py` & `featurebyte-0.4.2/featurebyte/routes/lazy_app_container.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/observation_table/api.py` & `featurebyte-0.4.2/featurebyte/routes/observation_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/observation_table/controller.py` & `featurebyte-0.4.2/featurebyte/routes/observation_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/periodic_tasks/api.py` & `featurebyte-0.4.2/featurebyte/routes/periodic_tasks/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/periodic_tasks/controller.py` & `featurebyte-0.4.2/featurebyte/routes/periodic_tasks/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/registry.py` & `featurebyte-0.4.2/featurebyte/routes/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from featurebyte.routes.app_container_config import AppContainerConfig
 from featurebyte.routes.batch_feature_table.controller import BatchFeatureTableController
 from featurebyte.routes.batch_request_table.controller import BatchRequestTableController
 from featurebyte.routes.catalog.catalog_name_injector import CatalogNameInjector
 from featurebyte.routes.catalog.controller import CatalogController
 from featurebyte.routes.common.base import DerivePrimaryEntityHelper
 from featurebyte.routes.common.feature_metadata_extractor import FeatureOrTargetMetadataExtractor
+from featurebyte.routes.common.feature_or_target_helper import FeatureOrTargetHelper
 from featurebyte.routes.context.controller import ContextController
 from featurebyte.routes.credential.controller import CredentialController
 from featurebyte.routes.deployment.controller import AllDeploymentController, DeploymentController
 from featurebyte.routes.dimension_table.controller import DimensionTableController
 from featurebyte.routes.entity.controller import EntityController
 from featurebyte.routes.event_table.controller import EventTableController
 from featurebyte.routes.feature.controller import FeatureController
@@ -165,14 +166,15 @@
 app_container_config.register_class(FeatureJobSettingAnalysisService)
 app_container_config.register_class(FeatureListController)
 app_container_config.register_class(FeatureListService)
 app_container_config.register_class(FeatureListNamespaceController)
 app_container_config.register_class(FeatureListNamespaceService)
 app_container_config.register_class(FeatureListStatusService)
 app_container_config.register_class(FeatureManagerService)
+app_container_config.register_class(FeatureOrTargetHelper)
 app_container_config.register_class(FeatureOrTargetMetadataExtractor)
 app_container_config.register_class(FeatureNamespaceController)
 app_container_config.register_class(FeatureNamespaceService)
 app_container_config.register_class(FeaturePreviewService)
 app_container_config.register_class(FeatureReadinessService)
 app_container_config.register_class(FeatureStoreController)
 app_container_config.register_class(FeatureStoreService)
```

### Comparing `featurebyte-0.4.1/featurebyte/routes/relationship_info/api.py` & `featurebyte-0.4.2/featurebyte/routes/relationship_info/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/relationship_info/controller.py` & `featurebyte-0.4.2/featurebyte/routes/relationship_info/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/scd_table/api.py` & `featurebyte-0.4.2/featurebyte/routes/scd_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/scd_table/controller.py` & `featurebyte-0.4.2/featurebyte/routes/scd_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/semantic/api.py` & `featurebyte-0.4.2/featurebyte/routes/semantic/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/semantic/controller.py` & `featurebyte-0.4.2/featurebyte/routes/semantic/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/static_source_table/api.py` & `featurebyte-0.4.2/featurebyte/routes/static_source_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/static_source_table/controller.py` & `featurebyte-0.4.2/featurebyte/routes/static_source_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/table/api.py` & `featurebyte-0.4.2/featurebyte/routes/table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/target/api.py` & `featurebyte-0.4.2/featurebyte/routes/target/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/target/controller.py` & `featurebyte-0.4.2/featurebyte/routes/target/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from bson import ObjectId
 from fastapi import HTTPException
 
 from featurebyte.exception import MissingPointInTimeColumnError, RequiredEntityNotProvidedError
 from featurebyte.models.target import TargetModel
 from featurebyte.routes.common.base import BaseDocumentController
 from featurebyte.routes.common.feature_metadata_extractor import FeatureOrTargetMetadataExtractor
+from featurebyte.routes.common.feature_or_target_helper import FeatureOrTargetHelper
 from featurebyte.schema.preview import FeatureOrTargetPreview
-from featurebyte.schema.target import InputData, TableMetadata, TargetCreate, TargetInfo, TargetList
+from featurebyte.schema.target import TargetCreate, TargetInfo, TargetList
 from featurebyte.service.entity import EntityService
 from featurebyte.service.feature_preview import FeaturePreviewService
 from featurebyte.service.mixin import DEFAULT_PAGE_SIZE
-from featurebyte.service.table import TableService
 from featurebyte.service.target import TargetService
 from featurebyte.service.target_namespace import TargetNamespaceService
 
 
 class TargetController(BaseDocumentController[TargetModel, TargetService, TargetList]):
     """
     Target controller
@@ -33,23 +33,23 @@
 
     def __init__(
         self,
         target_service: TargetService,
         target_namespace_service: TargetNamespaceService,
         entity_service: EntityService,
         feature_preview_service: FeaturePreviewService,
-        table_service: TableService,
         feature_or_target_metadata_extractor: FeatureOrTargetMetadataExtractor,
+        feature_or_target_helper: FeatureOrTargetHelper,
     ):
         super().__init__(target_service)
         self.target_namespace_service = target_namespace_service
         self.entity_service = entity_service
         self.feature_preview_service = feature_preview_service
-        self.table_service = table_service
         self.feature_or_target_metadata_extractor = feature_or_target_metadata_extractor
+        self.feature_or_target_helper = feature_or_target_helper
 
     async def create_target(
         self,
         data: TargetCreate,
     ) -> TargetModel:
         """
         Create Target at persistent
@@ -128,24 +128,19 @@
             document_id=target_doc.target_namespace_id
         )
         entity_ids = target_doc.entity_ids or []
         entity_brief_info_list = await self.entity_service.get_entity_brief_info_list(
             set(entity_ids)
         )
 
-        # Get input table metadata
-        assert (
-            len(target_doc.table_ids) == 1
-        ), "Target should have only one table for now, until forward joins are supported."
-        table_doc = await self.table_service.get_document(document_id=target_doc.table_ids[0])
-        input_data = InputData(
-            main_data=TableMetadata(
-                name=table_doc.name,
-                data_type=str(table_doc.type),
-            ),
+        primary_tables = await self.feature_or_target_helper.get_primary_tables(
+            target_doc.table_ids,
+            namespace.catalog_id,
+            target_doc.graph,
+            target_doc.node_name,
         )
 
         # Get metadata
         group_op_structure = target_doc.extract_operation_structure()
         target_metadata = await self.feature_or_target_metadata_extractor.extract(
             group_op_structure
         )
@@ -154,15 +149,15 @@
             id=document_id,
             target_name=target_doc.name,
             entities=entity_brief_info_list,
             window=namespace.window,
             has_recipe=bool(target_doc.graph),
             created_at=target_doc.created_at,
             updated_at=target_doc.updated_at,
-            input_data=input_data,
+            primary_table=primary_tables,
             metadata=target_metadata,
             namespace_description=namespace.description,
             description=target_doc.description,
         )
 
     async def preview(
         self, target_preview: FeatureOrTargetPreview, get_credential: Any
```

### Comparing `featurebyte-0.4.1/featurebyte/routes/target_namespace/api.py` & `featurebyte-0.4.2/featurebyte/routes/target_namespace/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/target_namespace/controller.py` & `featurebyte-0.4.2/featurebyte/routes/target_namespace/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/target_table/api.py` & `featurebyte-0.4.2/featurebyte/routes/target_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/target_table/controller.py` & `featurebyte-0.4.2/featurebyte/routes/target_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/task/api.py` & `featurebyte-0.4.2/featurebyte/routes/task/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/task/controller.py` & `featurebyte-0.4.2/featurebyte/routes/task/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/temp_data/api.py` & `featurebyte-0.4.2/featurebyte/routes/temp_data/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/temp_data/controller.py` & `featurebyte-0.4.2/featurebyte/routes/temp_data/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/user_defined_function/api.py` & `featurebyte-0.4.2/featurebyte/routes/user_defined_function/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/routes/user_defined_function/controller.py` & `featurebyte-0.4.2/featurebyte/routes/user_defined_function/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/batch_feature_table.py` & `featurebyte-0.4.2/featurebyte/schema/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/batch_request_table.py` & `featurebyte-0.4.2/featurebyte/schema/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/catalog.py` & `featurebyte-0.4.2/featurebyte/schema/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/common/base.py` & `featurebyte-0.4.2/featurebyte/schema/common/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/common/feature_or_target.py` & `featurebyte-0.4.2/featurebyte/schema/common/feature_or_target.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/common/operation.py` & `featurebyte-0.4.2/featurebyte/schema/common/operation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/context.py` & `featurebyte-0.4.2/featurebyte/schema/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/credential.py` & `featurebyte-0.4.2/featurebyte/schema/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/deployment.py` & `featurebyte-0.4.2/featurebyte/schema/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/dimension_table.py` & `featurebyte-0.4.2/featurebyte/schema/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/entity.py` & `featurebyte-0.4.2/featurebyte/schema/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/event_table.py` & `featurebyte-0.4.2/featurebyte/schema/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/feature.py` & `featurebyte-0.4.2/featurebyte/schema/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/feature_job_setting_analysis.py` & `featurebyte-0.4.2/featurebyte/schema/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/feature_list.py` & `featurebyte-0.4.2/featurebyte/schema/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/feature_list_namespace.py` & `featurebyte-0.4.2/featurebyte/schema/feature_list_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/feature_namespace.py` & `featurebyte-0.4.2/featurebyte/schema/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/feature_store.py` & `featurebyte-0.4.2/featurebyte/schema/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/historical_feature_table.py` & `featurebyte-0.4.2/featurebyte/schema/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/info.py` & `featurebyte-0.4.2/featurebyte/schema/info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/item_table.py` & `featurebyte-0.4.2/featurebyte/schema/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/materialized_table.py` & `featurebyte-0.4.2/featurebyte/schema/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/observation_table.py` & `featurebyte-0.4.2/featurebyte/schema/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/relationship_info.py` & `featurebyte-0.4.2/featurebyte/schema/relationship_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/request_table.py` & `featurebyte-0.4.2/featurebyte/schema/request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/scd_table.py` & `featurebyte-0.4.2/featurebyte/schema/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/semantic.py` & `featurebyte-0.4.2/featurebyte/schema/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/static_source_table.py` & `featurebyte-0.4.2/featurebyte/schema/static_source_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/table.py` & `featurebyte-0.4.2/featurebyte/schema/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/target.py` & `featurebyte-0.4.2/featurebyte/schema/target.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 )
 from featurebyte.models.target import TargetModel
 from featurebyte.query_graph.graph import QueryGraph
 from featurebyte.query_graph.model.common_table import TabularSource
 from featurebyte.query_graph.node import Node
 from featurebyte.schema.common.base import BaseDocumentServiceUpdateSchema, PaginationMixin
 from featurebyte.schema.common.feature_or_target import ComputeRequest
-from featurebyte.schema.info import EntityBriefInfoList
+from featurebyte.schema.info import EntityBriefInfoList, TableBriefInfoList
 
 
 class TargetCreate(FeatureByteBaseModel):
     """
     Target creation schema
     """
 
@@ -49,45 +49,27 @@
     """
     Target update schema
     """
 
     name: StrictStr
 
 
-class TableMetadata(FeatureByteBaseModel):
-    """
-    Table metadata
-    """
-
-    name: StrictStr
-    data_type: StrictStr
-
-
-class InputData(FeatureByteBaseModel):
-    """
-    Input data
-    """
-
-    main_data: TableMetadata
-    other_data: Optional[List[TableMetadata]] = None
-
-
 class TargetInfo(FeatureByteBaseModel):
     """
     Target info
     """
 
     id: PydanticObjectId
     target_name: str
     entities: EntityBriefInfoList
     window: Optional[str]
     has_recipe: bool
     created_at: datetime
     updated_at: Optional[datetime]
-    input_data: InputData
+    primary_table: TableBriefInfoList
     metadata: Any
     namespace_description: Optional[str]
     description: Optional[str]
 
 
 class ComputeTargetRequest(ComputeRequest):
     """
```

### Comparing `featurebyte-0.4.1/featurebyte/schema/target_namespace.py` & `featurebyte-0.4.2/featurebyte/schema/target_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/target_table.py` & `featurebyte-0.4.2/featurebyte/schema/target_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 
 from pydantic import StrictStr, root_validator
 
 from featurebyte.models.base import PydanticObjectId
+from featurebyte.models.observation_table import ObservationInput
 from featurebyte.models.target_table import TargetTableModel
 from featurebyte.query_graph.graph import QueryGraph
 from featurebyte.query_graph.node import Node
 from featurebyte.schema.common.base import PaginationMixin
 from featurebyte.schema.common.feature_or_target import FeatureOrTargetTableCreate
 from featurebyte.schema.materialized_table import BaseMaterializedTableListRecord
 
@@ -21,19 +22,21 @@
     TargetTable creation payload
     """
 
     serving_names_mapping: Optional[Dict[str, str]]
     target_id: Optional[PydanticObjectId]
     graph: QueryGraph
     node_names: List[StrictStr]
+    request_input: ObservationInput
+    context_id: Optional[PydanticObjectId]
 
     @property
     def nodes(self) -> List[Node]:
         """
-        Get feature nodes
+        Get target nodes
 
         Returns
         -------
         List[Node]
         """
         return [self.graph.get_node_by_name(name) for name in self.node_names]
```

### Comparing `featurebyte-0.4.1/featurebyte/schema/task.py` & `featurebyte-0.4.2/featurebyte/schema/task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/user_defined_function.py` & `featurebyte-0.4.2/featurebyte/schema/user_defined_function.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/base.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/batch_feature_create.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/batch_feature_create.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/batch_feature_table.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/batch_request_table.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/deployment_create_update.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/deployment_create_update.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/feature_job_setting_analysis.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/feature_list_batch_feature_create.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/feature_list_batch_feature_create.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/historical_feature_table.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/materialized_table_delete.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/observation_table.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/static_source_table.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/static_source_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/target_table.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/target_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Target table task payload
 """
 from typing import Optional
 
 from featurebyte.enum import WorkerCommand
-from featurebyte.models.target_table import TargetTableModel
+from featurebyte.models.observation_table import ObservationTableModel
 from featurebyte.schema.target_table import TargetTableCreate
 from featurebyte.schema.worker.task.base import BaseTaskPayload
 
 
 class TargetTableTaskPayload(BaseTaskPayload, TargetTableCreate):
     """
     TargetTable creation task payload
     """
 
-    output_collection_name = TargetTableModel.collection_name()
+    output_collection_name = ObservationTableModel.collection_name()
     command = WorkerCommand.TARGET_TABLE_CREATE
     observation_set_storage_path: Optional[str]
```

### Comparing `featurebyte-0.4.1/featurebyte/schema/worker/task/test.py` & `featurebyte-0.4.2/featurebyte/schema/worker/task/test.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/base_document.py` & `featurebyte-0.4.2/featurebyte/service/base_document.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/base_namespace_service.py` & `featurebyte-0.4.2/featurebyte/service/base_namespace_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/base_table_document.py` & `featurebyte-0.4.2/featurebyte/service/base_table_document.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/batch_feature_table.py` & `featurebyte-0.4.2/featurebyte/service/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/batch_request_table.py` & `featurebyte-0.4.2/featurebyte/service/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/catalog.py` & `featurebyte-0.4.2/featurebyte/service/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/context.py` & `featurebyte-0.4.2/featurebyte/service/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/credential.py` & `featurebyte-0.4.2/featurebyte/service/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/default_version_mode.py` & `featurebyte-0.4.2/featurebyte/service/default_version_mode.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/deploy.py` & `featurebyte-0.4.2/featurebyte/service/deploy.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/deployment.py` & `featurebyte-0.4.2/featurebyte/service/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/dimension_table.py` & `featurebyte-0.4.2/featurebyte/service/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/entity.py` & `featurebyte-0.4.2/featurebyte/service/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/entity_validation.py` & `featurebyte-0.4.2/featurebyte/service/entity_validation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/event_table.py` & `featurebyte-0.4.2/featurebyte/service/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/feature.py` & `featurebyte-0.4.2/featurebyte/service/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/feature_job_setting_analysis.py` & `featurebyte-0.4.2/featurebyte/service/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/feature_list.py` & `featurebyte-0.4.2/featurebyte/service/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/feature_list_namespace.py` & `featurebyte-0.4.2/featurebyte/service/feature_list_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/feature_list_status.py` & `featurebyte-0.4.2/featurebyte/service/feature_list_status.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/feature_manager.py` & `featurebyte-0.4.2/featurebyte/service/feature_manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/feature_namespace.py` & `featurebyte-0.4.2/featurebyte/service/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/feature_preview.py` & `featurebyte-0.4.2/featurebyte/service/feature_preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/feature_readiness.py` & `featurebyte-0.4.2/featurebyte/service/feature_readiness.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/feature_store.py` & `featurebyte-0.4.2/featurebyte/service/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/feature_store_warehouse.py` & `featurebyte-0.4.2/featurebyte/service/feature_store_warehouse.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/historical_feature_table.py` & `featurebyte-0.4.2/featurebyte/service/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/historical_features.py` & `featurebyte-0.4.2/featurebyte/service/historical_features.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/item_table.py` & `featurebyte-0.4.2/featurebyte/service/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/materialized_table.py` & `featurebyte-0.4.2/featurebyte/service/namespace_handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,140 +1,142 @@
 """
-BaseMaterializedTableService contains common functionality for materialized tables
+Namespace handler
 """
-from __future__ import annotations
-
-from typing import Any, List, Optional, Tuple
+from typing import Any, Dict, List, Tuple, Union
 
 from bson import ObjectId
 
-from featurebyte.persistent import Persistent
-from featurebyte.query_graph.model.common_table import TabularSource
-from featurebyte.query_graph.node.schema import ColumnSpec, TableDetails
-from featurebyte.query_graph.sql.common import sql_to_string
-from featurebyte.query_graph.sql.materialisation import get_source_count_expr
-from featurebyte.schema.common.base import BaseDocumentServiceUpdateSchema
-from featurebyte.schema.worker.task.materialized_table_delete import (
-    MaterializedTableDeleteTaskPayload,
-)
-from featurebyte.service.base_document import BaseDocumentService
-from featurebyte.service.feature_store import FeatureStoreService
-from featurebyte.service.mixin import Document, DocumentCreateSchema
-from featurebyte.session.base import BaseSession
-from featurebyte.session.manager import SessionManager
-
-
-class BaseMaterializedTableService(
-    BaseDocumentService[Document, DocumentCreateSchema, BaseDocumentServiceUpdateSchema]
-):
+from featurebyte.exception import DocumentInconsistencyError
+from featurebyte.models.base import FeatureByteCatalogBaseDocumentModel
+from featurebyte.models.feature import FeatureModel
+from featurebyte.models.target import TargetModel
+from featurebyte.query_graph.graph import QueryGraph
+from featurebyte.query_graph.model.graph import QueryGraphModel
+from featurebyte.query_graph.node import Node
+from featurebyte.query_graph.transform.sdk_code import SDKCodeExtractor
+from featurebyte.service.sanitizer import sanitize_query_graph_for_feature_definition
+from featurebyte.service.table import TableService
+from featurebyte.service.view_construction import ViewConstructionService
+
+
+async def validate_version_and_namespace_consistency(
+    base_model: FeatureByteCatalogBaseDocumentModel,
+    base_namespace_model: FeatureByteCatalogBaseDocumentModel,
+    attributes: List[str],
+) -> None:
     """
-    BaseMaterializedTableService contains common functionality for materialized tables
+    Validate whether the target & target namespace are consistent
+
+    Parameters
+    ----------
+    base_model: FeatureByteCatalogBaseDocumentModel
+        base object
+    base_namespace_model: FeatureByteCatalogBaseDocumentModel
+        base namespace object
+    attributes: List[str]
+        attributes to compare
+
+    Raises
+    ------
+    DocumentInconsistencyError
+        If the inconsistency between version & namespace found
     """
+    for attr in attributes:
+        version_attr = getattr(base_model, attr)
+        namespace_attr = getattr(base_namespace_model, attr)
+        version_attr_str: Union[str, List[str]] = f'"{version_attr}"'
+        namespace_attr_str: Union[str, List[str]] = f'"{namespace_attr}"'
+        if isinstance(version_attr, List):
+            version_attr = sorted(version_attr)
+            version_attr_str = [str(val) for val in version_attr]
+
+        if isinstance(namespace_attr, List):
+            namespace_attr = sorted(namespace_attr)
+            namespace_attr_str = [str(val) for val in namespace_attr]
+
+        if version_attr != namespace_attr:
+            class_name = base_model.__class__.__name__
+            raise DocumentInconsistencyError(
+                f'{class_name} (name: "{base_model.name}") object(s) within the same namespace '
+                f'must have the same "{attr}" value (namespace: {namespace_attr_str}, '
+                f"{class_name}: {version_attr_str})."
+            )
 
-    materialized_table_name_prefix = ""
+
+class NamespaceHandler:
+    """
+    Namespace handler class
+    """
 
     def __init__(
-        self,
-        user: Any,
-        persistent: Persistent,
-        catalog_id: Optional[ObjectId],
-        feature_store_service: FeatureStoreService,
+        self, table_service: TableService, view_construction_service: ViewConstructionService
     ):
-        super().__init__(user, persistent, catalog_id)
-        self.feature_store_service = feature_store_service
+        self.table_service = table_service
+        self.view_construction_service = view_construction_service
 
-    async def get_materialized_table_delete_task_payload(
-        self, document_id: ObjectId
-    ) -> MaterializedTableDeleteTaskPayload:
+    async def prepare_graph_to_store(
+        self, graph: QueryGraphModel, node: Node, sanitize_for_definition: bool = False
+    ) -> Tuple[QueryGraphModel, str]:
         """
-        Get the materialized table delete task payload
+        Prepare the graph to store by pruning the query graph
 
         Parameters
         ----------
-        document_id: ObjectId
-            The document id
+        graph: QueryGraphModel
+            Query graph
+        node: Node
+            Target node
+        sanitize_for_definition: bool
+            Whether to sanitize the query graph for generating feature definition
 
         Returns
         -------
-        MaterializedTableDeleteTaskPayload
+        QueryGraphModel
         """
-        return MaterializedTableDeleteTaskPayload(
-            user_id=self.user.id,
-            catalog_id=self.catalog_id,
-            document_id=document_id,
-            collection_name=self.document_class.collection_name(),
+        # Using a pruned graph, reconstruct view graph node to remove unused column cleaning
+        # operations
+        graph, node_name_map = QueryGraph(**graph.dict(by_alias=True)).prune(target_node=node)
+        node = graph.get_node_by_name(node_name_map[node.name])
+        constructed_graph, node_name_map = await self.view_construction_service.construct_graph(
+            query_graph=graph,
+            target_node=node,
+            table_cleaning_operations=[],
         )
+        node = constructed_graph.get_node_by_name(node_name_map[node.name])
 
-    async def generate_materialized_table_location(
-        self, get_credential: Any, feature_store_id: ObjectId
-    ) -> TabularSource:
-        """
-        Generate a TabularSource object for a new materialized table to be created
-
-        Parameters
-        ----------
-        get_credential: Any
-            Function to get credential for a feature store
-        feature_store_id: ObjectId
-            Feature store id
+        # Prune the graph to remove unused nodes and parameters
+        pruned_graph, pruned_node_name_map = QueryGraph(
+            **constructed_graph.dict(by_alias=True)
+        ).prune(target_node=node)
+        if sanitize_for_definition:
+            pruned_graph = sanitize_query_graph_for_feature_definition(graph=pruned_graph)
+        return pruned_graph, pruned_node_name_map[node.name]
 
-        Returns
-        -------
-        TabularSource
+    async def prepare_definition(self, document: Union[FeatureModel, TargetModel]) -> str:
         """
-        feature_store = await self.feature_store_service.get_document(document_id=feature_store_id)
-        session_manager = SessionManager(
-            credentials={
-                feature_store.name: await get_credential(
-                    user_id=self.user.id, feature_store_name=feature_store.name
-                )
-            }
-        )
-        db_session = await session_manager.get_session(feature_store)
-
-        destination_table_name = f"{self.materialized_table_name_prefix}_{ObjectId()}"
-        location = TabularSource(
-            feature_store_id=feature_store_id,
-            table_details=TableDetails(
-                database_name=db_session.database_name,
-                schema_name=db_session.schema_name,
-                table_name=destination_table_name,
-            ),
-        )
-        return location
-
-    @staticmethod
-    async def get_columns_info_and_num_rows(
-        db_session: BaseSession, table_details: TableDetails
-    ) -> Tuple[List[ColumnSpec], int]:
-        """
-        Get the columns info and number of rows from a materialized table
+        Prepare the definition for the given document
 
         Parameters
         ----------
-        db_session: BaseSession
-            The database session
-        table_details: TableDetails
-            The table details of the materialized table
+        document: Union[FeatureModel, TargetModel]
+            FeatureModel or TargetModel document
 
         Returns
         -------
-        Tuple[List[ColumnSpec], int]
-            The columns info and number of rows
+        str
         """
-        table_schema = await db_session.list_table_schema(
-            table_name=table_details.table_name,
-            database_name=table_details.database_name,
-            schema_name=table_details.schema_name,
-        )
-        df_row_count = await db_session.execute_query(
-            sql_to_string(
-                get_source_count_expr(table_details),
-                db_session.source_type,
-            )
+        # check whether table has been saved at persistent storage
+        table_id_to_info: Dict[ObjectId, Dict[str, Any]] = {}
+        for table_id in document.table_ids:
+            table = await self.table_service.get_document(document_id=table_id)
+            table_id_to_info[table_id] = table.dict()
+
+        # create feature definition
+        graph, node_name = document.graph, document.node_name
+        sdk_code_gen_state = SDKCodeExtractor(graph=graph).extract(
+            node=graph.get_node_by_name(node_name),
+            to_use_saved_data=True,
+            table_id_to_info=table_id_to_info,
+            output_id=document.id,
         )
-        assert df_row_count is not None
-        num_rows = df_row_count.iloc[0]["row_count"]
-        columns_info = [
-            ColumnSpec(name=name, dtype=var_type) for name, var_type in table_schema.items()
-        ]
-        return columns_info, num_rows
+        definition = sdk_code_gen_state.code_generator.generate(to_format=True)
+        return definition
```

### Comparing `featurebyte-0.4.1/featurebyte/service/mixin.py` & `featurebyte-0.4.2/featurebyte/service/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/observation_table.py` & `featurebyte-0.4.2/featurebyte/service/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/online_enable.py` & `featurebyte-0.4.2/featurebyte/service/online_enable.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/online_serving.py` & `featurebyte-0.4.2/featurebyte/service/online_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/online_store_compute_query_service.py` & `featurebyte-0.4.2/featurebyte/service/online_store_compute_query_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/online_store_table_version.py` & `featurebyte-0.4.2/featurebyte/service/online_store_table_version.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/parent_serving.py` & `featurebyte-0.4.2/featurebyte/service/parent_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/preview.py` & `featurebyte-0.4.2/featurebyte/service/preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/relationship.py` & `featurebyte-0.4.2/featurebyte/service/relationship.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/relationship_info.py` & `featurebyte-0.4.2/featurebyte/service/relationship_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/sanitizer.py` & `featurebyte-0.4.2/featurebyte/service/sanitizer.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/scd_table.py` & `featurebyte-0.4.2/featurebyte/service/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/semantic.py` & `featurebyte-0.4.2/featurebyte/service/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/session_manager.py` & `featurebyte-0.4.2/featurebyte/service/session_manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/session_validator.py` & `featurebyte-0.4.2/featurebyte/service/session_validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/static_source_table.py` & `featurebyte-0.4.2/featurebyte/service/static_source_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/table.py` & `featurebyte-0.4.2/featurebyte/service/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/table_columns_info.py` & `featurebyte-0.4.2/featurebyte/service/table_columns_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/table_info.py` & `featurebyte-0.4.2/featurebyte/service/table_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/table_status.py` & `featurebyte-0.4.2/featurebyte/service/table_status.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/target.py` & `featurebyte-0.4.2/featurebyte/service/target.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/target_helper/base_feature_or_target_computer.py` & `featurebyte-0.4.2/featurebyte/service/target_helper/base_feature_or_target_computer.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/target_helper/compute_target.py` & `featurebyte-0.4.2/featurebyte/service/target_helper/compute_target.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/target_namespace.py` & `featurebyte-0.4.2/featurebyte/service/target_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/target_table.py` & `featurebyte-0.4.2/featurebyte/service/target_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/task_manager.py` & `featurebyte-0.4.2/featurebyte/service/task_manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/tile/tile_task_executor.py` & `featurebyte-0.4.2/featurebyte/service/tile/tile_task_executor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/tile_cache.py` & `featurebyte-0.4.2/featurebyte/service/tile_cache.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/tile_job_log.py` & `featurebyte-0.4.2/featurebyte/service/tile_job_log.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/tile_manager.py` & `featurebyte-0.4.2/featurebyte/service/tile_manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/tile_registry_service.py` & `featurebyte-0.4.2/featurebyte/service/tile_registry_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/tile_scheduler.py` & `featurebyte-0.4.2/featurebyte/service/tile_scheduler.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/user_defined_function.py` & `featurebyte-0.4.2/featurebyte/service/user_defined_function.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/user_service.py` & `featurebyte-0.4.2/featurebyte/service/user_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/validator/materialized_table_delete.py` & `featurebyte-0.4.2/featurebyte/service/validator/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/validator/production_ready_validator.py` & `featurebyte-0.4.2/featurebyte/service/validator/production_ready_validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/version.py` & `featurebyte-0.4.2/featurebyte/service/version.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/view_construction.py` & `featurebyte-0.4.2/featurebyte/service/view_construction.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/service/working_schema.py` & `featurebyte-0.4.2/featurebyte/service/working_schema.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/session/base.py` & `featurebyte-0.4.2/featurebyte/session/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/session/base_spark.py` & `featurebyte-0.4.2/featurebyte/session/base_spark.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,15 @@
             "DATE": DBVarType.DATE,
             "DECIMAL": DBVarType.FLOAT,
             "DOUBLE": DBVarType.FLOAT,
             "FLOAT": DBVarType.FLOAT,
             "INTERVAL": DBVarType.TIMEDELTA,
             "VOID": DBVarType.VOID,
             "TIMESTAMP": DBVarType.TIMESTAMP,
+            "TIMESTAMP_NTZ": DBVarType.TIMESTAMP,
             "ARRAY": DBVarType.ARRAY,
             "MAP": DBVarType.MAP,
             "STRUCT": DBVarType.STRUCT,
             "STRING": DBVarType.VARCHAR,
         }
         if spark_type not in mapping:
             logger.warning(f"Spark: Not supported data type '{spark_type}'")
```

### Comparing `featurebyte-0.4.1/featurebyte/session/databricks.py` & `featurebyte-0.4.2/featurebyte/session/databricks.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/session/hive.py` & `featurebyte-0.4.2/featurebyte/session/hive.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/session/manager.py` & `featurebyte-0.4.2/featurebyte/session/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/session/simple_storage.py` & `featurebyte-0.4.2/featurebyte/session/simple_storage.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/session/snowflake.py` & `featurebyte-0.4.2/featurebyte/session/snowflake.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/session/spark.py` & `featurebyte-0.4.2/featurebyte/session/spark.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/session/sqlite.py` & `featurebyte-0.4.2/featurebyte/session/sqlite.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/session/webhdfs.py` & `featurebyte-0.4.2/featurebyte/session/webhdfs.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/base.py` & `featurebyte-0.4.2/featurebyte/sql/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/common.py` & `featurebyte-0.4.2/featurebyte/sql/common.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql` & `featurebyte-0.4.2/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql` & `featurebyte-0.4.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/snowflake/F_GET_RANK.sql` & `featurebyte-0.4.2/featurebyte/sql/snowflake/F_GET_RANK.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql` & `featurebyte-0.4.2/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql` & `featurebyte-0.4.2/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql` & `featurebyte-0.4.2/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar` & `featurebyte-0.4.2/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,25 +1,25 @@
 Zip file size: 29714 bytes, number of entries: 23
-drwxr-xr-x  2.0 unx        0 b- defN 23-Jul-25 05:46 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-Jul-25 05:46 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- defN 23-Jul-25 05:45 com/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Jul-25 05:45 com/featurebyte/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Jul-25 05:45 com/featurebyte/hive/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/
--rw-r--r--  2.0 unx     5044 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/TimestampToIndex.class
--rw-r--r--  2.0 unx     3796 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/CountDictMostFrequent.class
--rw-r--r--  2.0 unx     2923 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/CountDictNumUnique.class
--rw-r--r--  2.0 unx     3730 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/CountDictMostFrequentValue.class
--rw-r--r--  2.0 unx     5098 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/CountDictUDF.class
--rw-r--r--  2.0 unx     2741 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/ObjectDelete.class
--rw-r--r--  2.0 unx     2544 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/ObjectAggregate.class
--rw-r--r--  2.0 unx     2570 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
--rw-r--r--  2.0 unx     3769 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
--rw-r--r--  2.0 unx     3721 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/CountDictEntropy.class
--rw-r--r--  2.0 unx     6348 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/CountDictCosineSimilarity.class
--rw-r--r--  2.0 unx     5593 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/CountDictRank.class
--rw-r--r--  2.0 unx     3884 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/CountDictRelativeFrequency.class
--rw-r--r--  2.0 unx     5161 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
--rw-r--r--  2.0 unx      963 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
--rw-r--r--  2.0 unx     5565 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/IndexToTimestamp.class
--rw-r--r--  2.0 unx     1070 b- defN 23-Jul-25 05:45 com/featurebyte/hive/udf/ObjectAggregate$1.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Aug-07 07:55 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 23-Aug-07 07:55 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- defN 23-Aug-07 07:55 com/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Aug-07 07:55 com/featurebyte/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Aug-07 07:55 com/featurebyte/hive/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/
+-rw-r--r--  2.0 unx     3721 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/CountDictEntropy.class
+-rw-r--r--  2.0 unx     5161 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
+-rw-r--r--  2.0 unx     2923 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/CountDictNumUnique.class
+-rw-r--r--  2.0 unx     2741 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/ObjectDelete.class
+-rw-r--r--  2.0 unx     2570 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
+-rw-r--r--  2.0 unx     5098 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/CountDictUDF.class
+-rw-r--r--  2.0 unx     3769 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
+-rw-r--r--  2.0 unx     3730 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/CountDictMostFrequentValue.class
+-rw-r--r--  2.0 unx     5593 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/CountDictRank.class
+-rw-r--r--  2.0 unx     1070 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/ObjectAggregate$1.class
+-rw-r--r--  2.0 unx     3796 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/CountDictMostFrequent.class
+-rw-r--r--  2.0 unx      963 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
+-rw-r--r--  2.0 unx     3884 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/CountDictRelativeFrequency.class
+-rw-r--r--  2.0 unx     2544 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/ObjectAggregate.class
+-rw-r--r--  2.0 unx     5565 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/IndexToTimestamp.class
+-rw-r--r--  2.0 unx     5044 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/TimestampToIndex.class
+-rw-r--r--  2.0 unx     6348 b- defN 23-Aug-07 07:55 com/featurebyte/hive/udf/CountDictCosineSimilarity.class
 23 files, 64545 bytes uncompressed, 25512 bytes compressed:  60.5%
```

#### zipnote «TEMP»/diffoscope_6z2qlgr8_/tmp_yehk569_.zip

```diff
@@ -12,59 +12,59 @@
 
 Filename: com/featurebyte/hive/
 Comment: 
 
 Filename: com/featurebyte/hive/udf/
 Comment: 
 
-Filename: com/featurebyte/hive/udf/TimestampToIndex.class
+Filename: com/featurebyte/hive/udf/CountDictEntropy.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictMostFrequent.class
+Filename: com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
 Comment: 
 
 Filename: com/featurebyte/hive/udf/CountDictNumUnique.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictMostFrequentValue.class
+Filename: com/featurebyte/hive/udf/ObjectDelete.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictUDF.class
+Filename: com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectDelete.class
+Filename: com/featurebyte/hive/udf/CountDictUDF.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectAggregate.class
+Filename: com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
+Filename: com/featurebyte/hive/udf/CountDictMostFrequentValue.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
+Filename: com/featurebyte/hive/udf/CountDictRank.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictEntropy.class
+Filename: com/featurebyte/hive/udf/ObjectAggregate$1.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictCosineSimilarity.class
+Filename: com/featurebyte/hive/udf/CountDictMostFrequent.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictRank.class
+Filename: com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
 Comment: 
 
 Filename: com/featurebyte/hive/udf/CountDictRelativeFrequency.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
+Filename: com/featurebyte/hive/udf/ObjectAggregate.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
+Filename: com/featurebyte/hive/udf/IndexToTimestamp.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/IndexToTimestamp.class
+Filename: com/featurebyte/hive/udf/TimestampToIndex.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectAggregate$1.class
+Filename: com/featurebyte/hive/udf/CountDictCosineSimilarity.class
 Comment: 
 
 Zip file comment:
```

### Comparing `featurebyte-0.4.1/featurebyte/sql/tile_common.py` & `featurebyte-0.4.2/featurebyte/sql/tile_common.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/tile_generate.py` & `featurebyte-0.4.2/featurebyte/sql/tile_generate.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/tile_generate_entity_tracking.py` & `featurebyte-0.4.2/featurebyte/sql/tile_generate_entity_tracking.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/tile_monitor.py` & `featurebyte-0.4.2/featurebyte/sql/tile_monitor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/tile_registry.py` & `featurebyte-0.4.2/featurebyte/sql/tile_registry.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/sql/tile_schedule_online_store.py` & `featurebyte-0.4.2/featurebyte/sql/tile_schedule_online_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/storage/base.py` & `featurebyte-0.4.2/featurebyte/storage/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/storage/local.py` & `featurebyte-0.4.2/featurebyte/storage/local.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/storage/s3.py` & `featurebyte-0.4.2/featurebyte/storage/s3.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/tile/tile_cache.py` & `featurebyte-0.4.2/featurebyte/tile/tile_cache.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/utils/credential.py` & `featurebyte-0.4.2/featurebyte/utils/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/utils/messaging.py` & `featurebyte-0.4.2/featurebyte/utils/messaging.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/utils/persistent.py` & `featurebyte-0.4.2/featurebyte/utils/persistent.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/utils/storage.py` & `featurebyte-0.4.2/featurebyte/utils/storage.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/__init__.py` & `featurebyte-0.4.2/featurebyte/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/progress.py` & `featurebyte-0.4.2/featurebyte/worker/progress.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/schedulers.py` & `featurebyte-0.4.2/featurebyte/worker/schedulers.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/base.py` & `featurebyte-0.4.2/featurebyte/worker/task/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/batch_feature_create.py` & `featurebyte-0.4.2/featurebyte/worker/task/batch_feature_create.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/batch_feature_table.py` & `featurebyte-0.4.2/featurebyte/worker/task/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/batch_request_table.py` & `featurebyte-0.4.2/featurebyte/worker/task/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/deployment_create_update.py` & `featurebyte-0.4.2/featurebyte/worker/task/deployment_create_update.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/feature_job_setting_analysis.py` & `featurebyte-0.4.2/featurebyte/worker/task/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/feature_list_batch_feature_create.py` & `featurebyte-0.4.2/featurebyte/worker/task/feature_list_batch_feature_create.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/historical_feature_table.py` & `featurebyte-0.4.2/featurebyte/worker/task/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/materialized_table_delete.py` & `featurebyte-0.4.2/featurebyte/worker/task/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/mixin.py` & `featurebyte-0.4.2/featurebyte/worker/task/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/observation_table.py` & `featurebyte-0.4.2/featurebyte/worker/task/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/static_source_table.py` & `featurebyte-0.4.2/featurebyte/worker/task/static_source_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/test_task.py` & `featurebyte-0.4.2/featurebyte/worker/task/test_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task/tile_task.py` & `featurebyte-0.4.2/featurebyte/worker/task/tile_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/task_executor.py` & `featurebyte-0.4.2/featurebyte/worker/task_executor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/featurebyte/worker/util/observation_set_helper.py` & `featurebyte-0.4.2/featurebyte/worker/util/observation_set_helper.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.4.1/pyproject.toml` & `featurebyte-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     "featurebyte/sql/spark/*.jar",
 ]
 keywords = []
 license = "Elastic License 2.0"
 name = "featurebyte"
 readme = "README.md"
 repository = "https://github.com/featurebyte/featurebyte"
-version = "0.4.1"
+version = "0.4.2"
 
 [tool.poetry.dependencies]
 PyYAML = "^6.0"
 aiobotocore = { version = "^2.4.0", extras = ["boto3"] }
 aiofiles = "^22.1.0"
 aioredis = { version = "^2.0.1", optional = true }
 alive-progress = "^3.1.1"
```

### Comparing `featurebyte-0.4.1/PKG-INFO` & `featurebyte-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurebyte
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python Library for FeatureOps
 Home-page: https://featurebyte.com
 License: Elastic License 2.0
 Author: FeatureByte
 Author-email: it-admin@featurebyte.com
 Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 4 - Beta
```

