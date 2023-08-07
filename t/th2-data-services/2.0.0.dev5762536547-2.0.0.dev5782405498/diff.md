# Comparing `tmp/th2_data_services-2.0.0.dev5762536547.tar.gz` & `tmp/th2_data_services-2.0.0.dev5782405498.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev5762536547.tar", last modified: Fri Aug  4 13:06:11 2023, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev5782405498.tar", last modified: Mon Aug  7 07:45:56 2023, max compression
```

## Comparing `th2_data_services-2.0.0.dev5762536547.tar` & `th2_data_services-2.0.0.dev5782405498.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    30034 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24651 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-04 13:05:59.000000 th2_data_services-2.0.0.dev5762536547/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    16449 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5425 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    15496 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    14965 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    16550 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    34532 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/sse_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5463 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     7000 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-08-04 13:04:51.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    30034 2023-08-04 13:06:10.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-08-04 13:06:11.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 13:06:10.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-08-04 13:06:10.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-08-04 13:06:10.000000 th2_data_services-2.0.0.dev5762536547/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    30034 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24651 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-07 07:45:45.000000 th2_data_services-2.0.0.dev5782405498/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16098 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4643 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7286 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5425 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15496 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15044 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16550 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34532 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/sse_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5463 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7492 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-08-07 07:44:36.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    30034 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-08-07 07:45:56.000000 th2_data_services-2.0.0.dev5782405498/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev5762536547/PKG-INFO` & `th2_data_services-2.0.0.dev5782405498/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3537 3632 3533 3635 3437 0a53 756d 6d61  5762536547.Summa
+00000040: 3537 3832 3430 3534 3938 0a53 756d 6d61  5782405498.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5762536547/README.md` & `th2_data_services-2.0.0.dev5782405498/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/setup.py` & `th2_data_services-2.0.0.dev5782405498/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/data.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/aggregation_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,32 +147,14 @@
 
 class CategoryTable(ABC, PerfectTable):
     def __init__(self, header: List[str]):  # noqa
         super().__init__(header)
         self._service_columns = {}  # {'col_name': 'idx'}
         self._service_rows = []  # [idx]
 
-    def _totals_line(self):
-        totals = []
-        for col_name in self.header:
-            col_tuple = self[col_name]
-
-            try:
-                # If all Bool.
-                if all([isinstance(x, bool) for x in col_tuple]):
-                    pos = sum(col_tuple)
-                    neg = len(col_tuple) - pos
-                    totals.append(f"{pos}/{neg}")
-                else:
-                    totals.append(sum(col_tuple))
-            except:
-                totals.append("")
-
-        return totals
-
 
 class FrequencyCategoryTable(CategoryTable):
     def __init__(self, header: List[str], rows=None):  # noqa
         super().__init__(header)
         self.service_columns = {
             "timestamp": 0,
         }  # {'col_name': 'idx'}
@@ -222,25 +204,14 @@
                 if any(vals) != 0:
                     fct.add_row([row[self.service_columns["timestamp"]], *vals])
             else:
                 fct.add_row([row[self.service_columns["timestamp"]], *vals])
 
         return fct
 
-    def get_list_repr(self):
-        additional_rows = [
-            ["count"] + ["" for _ in range(len(self.header) - 1)] + [len(self.rows)],
-            ["totals"] + self._totals_line(),
-        ]
-        return [
-            [" "] + list(self.header),
-            *[[" "] + list(row) for row in self.rows],
-            *additional_rows,
-        ]
-
 
 class TotalCategoryTable(CategoryTable):
     # This class allows to create tables with multiple categories. e.g  type | status | count
     def __init__(self, header, rows=None):  # noqa
         super().__init__(header)
         self.service_columns = {
             "timestamp": 0,
@@ -251,14 +222,32 @@
         self._transposed = False
         self.count_field_name = "count"
 
     @property
     def total(self):
         return sum(self[self.count_field_name])
 
+    def _totals_line(self):
+        totals = []
+        for col_name in self.header:
+            col_tuple = self[col_name]
+
+            try:
+                # If all Bool.
+                if all([isinstance(x, bool) for x in col_tuple]):
+                    pos = sum(col_tuple)
+                    neg = len(col_tuple) - pos
+                    totals.append(f"{pos}/{neg}")
+                else:
+                    totals.append(sum(col_tuple))
+            except:
+                totals.append("")
+
+        return totals
+
     def add_rows_from_dict(self, d: dict):
         result = []
         for category_name, category_value in d.items():
             result.append([category_name, str(category_value)])
             # total += category_value
 
         # if sort_values:
```

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from datetime import datetime, timezone
 import shutil
 import gzip
 
 from th2_data_services.interfaces.utils.converter import ITimestampConverter
 from collections.abc import MutableMapping
 
-_DatetimeTuple = namedtuple("DatetimeTuple", "datetime mantissa")
+_DatetimeTuple = namedtuple("DatetimeTuple", ["datetime", "mantissa"])
 
 
 class DatetimeStringConverter(ITimestampConverter[str]):
     """Converts datetime strings.
 
     If you request microseconds but your timestamp has nanoseconds, they will be just cut (not rounding).
```

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/event_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,19 @@
 
 
 # NOT STREAMING
 # TODO - Can we have single function for events and messages?
 #
 # Will return list! Perhaps it's better to return Data?
 def get_some(
-    events: Iterable[Th2Event], event_type: Optional[str], max_count: int, start: int = 0, failed: bool = False  # ??
+    events: Iterable[Th2Event],
+    event_type: Optional[str],
+    max_count: int,  # TODO -- Slava - I think we need to add Optional = None, for unlimited.
+    start: int = 0,
+    failed: bool = False,  # ??
 ) -> Iterable[Th2Event]:
     """Returns limited list of events of specific eventType.
 
     Args:
         events (Iterable[Th2Event]): TH2-Events
         event_type (str): Event Type To Extract
         max_count (int): Maximum number of events to extract
@@ -126,15 +130,17 @@
         level += 1
         print(f"Level {level}: {next_levels_count} events")
         for next_level in next_levels:
             event_id = options.EVENT_FIELDS_RESOLVER.get_id(next_level)
             parent_id = options.EVENT_FIELDS_RESOLVER.get_parent_id(next_level)
             result[event_id] = {
                 "eventName": options.EVENT_FIELDS_RESOLVER.get_name(next_level),
-                "eventPath": result[parent_id]["eventPath"] + "/" + options.EVENT_FIELDS_RESOLVER.get_name(next_level),
+                "eventPath": result[parent_id]["eventPath"]
+                + "/"
+                + options.EVENT_FIELDS_RESOLVER.get_name(next_level),
             }
         prev_levels = next_levels
 
     return result
 
 
 # STREAMING
@@ -144,15 +150,17 @@
 
     Args:
         event: TH2-Event
 
     Returns:
         str
     """
-    return th2_data_services.utils.time.extract_timestamp(options.EVENT_FIELDS_RESOLVER.get_start_timestamp(event))
+    return th2_data_services.utils.time.extract_timestamp(
+        options.EVENT_FIELDS_RESOLVER.get_start_timestamp(event)
+    )
 
 
 # NOT STREAMING
 def extract_parent_as_json(
     events: Iterable[Th2Event],
     parent_id: str,
     json_file_path: str,
@@ -194,17 +202,23 @@
                 }
             }
             "child_id2": { ... }
         }
     """
     from th2_data_services.utils.az_tree import get_event_tree_from_parent_id
 
-    sub_events = sublist(events, datetime.fromisoformat(interval_start), datetime.fromisoformat(interval_end))
+    sub_events = sublist(
+        events, datetime.fromisoformat(interval_start), datetime.fromisoformat(interval_end)
+    )
     print(f"Sublist length = {len(sub_events)}")
-    tree = get_event_tree_from_parent_id(sub_events, parent_id, 10, 10000, body_to_simple_processors)
+    tree = get_event_tree_from_parent_id(
+        sub_events, parent_id, 10, 10000, body_to_simple_processors
+    )
     if not tree:
         return
-    types_set = set((type_[: type_.index(" [")] for type_ in tree["info"]["stats"] if type_ != "TOTAL"))
+    types_set = set(
+        (type_[: type_.index(" [")] for type_ in tree["info"]["stats"] if type_ != "TOTAL")
+    )
     tree["info"]["types_list"] = list(types_set)
 
     with open(json_file_path, "w") as file:
         json.dump(tree, file, indent=3)
```

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/message_utils/message_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 # # NOT STREAMABLE
 # Extract compounded message into list of individual messages
 # m: compounded message (retrieved from Data object)
 # result: list of individual message objects
 def expand_message(message: Th2Message) -> Iterable[Th2Message]:
     # TODO - should be updated for version with Th2Transport
+    # TODO - all this code knows the structure of the message. It's a problem.
     """Extract compounded message into list of individual messages.
 
     Args:
         message: TH2-Message
 
     Returns:
         Iterable[Th2Message]
```

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/total_category_calculator.py`

 * *Files 12% similar despite different names*

```diff
@@ -114,14 +114,27 @@
         try:
             return self._counters[combination]
         except KeyError:
             raise Exception(
                 f"Unknown combination. The following combination '{combination}' is not provided to constructor."
             )
 
+    def _prep_combination_keep_order(self, combination: CategoryCombination) -> List[str]:
+        """Returns combination in the required view."""
+        new_comb = []
+        for cv in combination:
+            if isinstance(cv, str):
+                new_comb.append(cv)
+            elif isinstance(cv, Category):
+                new_comb.append(cv.name)
+            else:
+                raise ValueError(f"Unexpected combination value, {combination}")
+
+        return new_comb
+
     def _prepare_combination(self, combination: CategoryCombination) -> Tuple[str]:
         """Returns combination in the required view."""
         new_comb = []
         for cv in combination:
             if isinstance(cv, str):
                 new_comb.append(cv)
             elif isinstance(cv, Category):
@@ -160,15 +173,15 @@
 
         Returns:
             TotalCategoryTable
 
         """
         orig_comb = combination
         comb: Category
-        orig_columns_order = [comb.name for comb in orig_comb]
+        orig_columns_order = self._prep_combination_keep_order(orig_comb)
         orig_columns_order.append(self.counter_field_name)
 
         combination = self._prepare_combination(combination)
 
         t = PrettyTable()
         t.field_names = [*combination, self.counter_field_name]
         counter = self._get_counter(combination)  # The object with calculated combinations.
```

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev5782405498/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev5782405498/th2_data_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3537 3632 3533 3635 3437 0a53 756d 6d61  5762536547.Summa
+00000040: 3537 3832 3430 3534 3938 0a53 756d 6d61  5782405498.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev5782405498/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5762536547/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev5782405498/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

