# Comparing `tmp/netbox-data-flows-0.7.1.tar.gz` & `tmp/netbox-data-flows-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-data-flows-0.7.1.tar", last modified: Sun Jul 16 17:59:53 2023, max compression
+gzip compressed data, was "netbox-data-flows-0.7.2.tar", last modified: Mon Aug  7 18:22:34 2023, max compression
```

## Comparing `netbox-data-flows-0.7.1.tar` & `netbox-data-flows-0.7.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.632483 netbox-data-flows-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-16 17:59:53.632483 netbox-data-flows-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.620483 netbox-data-flows-0.7.1/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.620483 netbox-data-flows-0.7.1/netbox_data_flows/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/addins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/graphql/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/graphql/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/graphql/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/graphql/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/management/commands/delete_orphaned_aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0002_alter_objectalias_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0007_remove_objectalias_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/models/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/models/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/models/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/models/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/models/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/tables/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/tables/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/tables/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/tables/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.620483 netbox-data-flows-0.7.1/netbox_data_flows/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/application.html
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow.html
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/objectalias.html
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/utils/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/views/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/model_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.620483 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-16 17:59:53.000000 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-16 17:59:53.000000 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:59:53.000000 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:59:53.000000 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-16 17:59:53.000000 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:59:53.632483 netbox-data-flows-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.146911 netbox-data-flows-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-08-07 18:22:34.146911 netbox-data-flows-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.130910 netbox-data-flows-0.7.2/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.134910 netbox-data-flows-0.7.2/netbox_data_flows/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.134910 netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.138911 netbox-data-flows-0.7.2/netbox_data_flows/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/filtersets/addins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/filtersets/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/filtersets/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/filtersets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/filtersets/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/filtersets/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.138911 netbox-data-flows-0.7.2/netbox_data_flows/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/forms/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/forms/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14146 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/forms/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/forms/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/forms/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.138911 netbox-data-flows-0.7.2/netbox_data_flows/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/graphql/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/graphql/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/graphql/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/graphql/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.138911 netbox-data-flows-0.7.2/netbox_data_flows/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.138911 netbox-data-flows-0.7.2/netbox_data_flows/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/management/commands/delete_orphaned_aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.142911 netbox-data-flows-0.7.2/netbox_data_flows/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/migrations/0002_alter_objectalias_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/migrations/0007_remove_objectalias_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.142911 netbox-data-flows-0.7.2/netbox_data_flows/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/models/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/models/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/models/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/models/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.142911 netbox-data-flows-0.7.2/netbox_data_flows/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/tables/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/tables/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/tables/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/tables/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.126910 netbox-data-flows-0.7.2/netbox_data_flows/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.146911 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/application.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/dataflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.146911 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/objectalias.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.146911 netbox-data-flows-0.7.2/netbox_data_flows/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/utils/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.146911 netbox-data-flows-0.7.2/netbox_data_flows/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/views/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/views/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/views/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/views/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/views/model_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/netbox_data_flows/views/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:22:34.130910 netbox-data-flows-0.7.2/netbox_data_flows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-08-07 18:22:34.000000 netbox-data-flows-0.7.2/netbox_data_flows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-08-07 18:22:34.000000 netbox-data-flows-0.7.2/netbox_data_flows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:22:34.000000 netbox-data-flows-0.7.2/netbox_data_flows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:22:33.000000 netbox-data-flows-0.7.2/netbox_data_flows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 18:22:34.000000 netbox-data-flows-0.7.2/netbox_data_flows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-07 18:22:12.000000 netbox-data-flows-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 18:22:34.146911 netbox-data-flows-0.7.2/setup.cfg
```

### Comparing `netbox-data-flows-0.7.1/LICENSE` & `netbox-data-flows-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/PKG-INFO` & `netbox-data-flows-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.7.1
+Version: 0.7.2
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `netbox-data-flows-0.7.1/README.md` & `netbox-data-flows-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/__init__.py` & `netbox-data-flows-0.7.2/netbox_data_flows/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from extras.plugins import PluginConfig
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
 
 class DataFlowsConfig(PluginConfig):
     name = "netbox_data_flows"
     verbose_name = "Data Flows"
     description = (
         "NetBox plugin to document data flows between "
```

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/applications.py` & `netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/dataflows.py` & `netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/groups.py` & `netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/nested.py` & `netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/nested.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/objectaliases.py` & `netbox-data-flows-0.7.2/netbox_data_flows/api/serializers/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/api/urls.py` & `netbox-data-flows-0.7.2/netbox_data_flows/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/api/views.py` & `netbox-data-flows-0.7.2/netbox_data_flows/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/choices.py` & `netbox-data-flows-0.7.2/netbox_data_flows/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/addins.py` & `netbox-data-flows-0.7.2/netbox_data_flows/filtersets/addins.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/applications.py` & `netbox-data-flows-0.7.2/netbox_data_flows/filtersets/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/dataflows.py` & `netbox-data-flows-0.7.2/netbox_data_flows/filtersets/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/filters.py` & `netbox-data-flows-0.7.2/netbox_data_flows/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/groups.py` & `netbox-data-flows-0.7.2/netbox_data_flows/filtersets/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/objectaliases.py` & `netbox-data-flows-0.7.2/netbox_data_flows/filtersets/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/forms/applicationroles.py` & `netbox-data-flows-0.7.2/netbox_data_flows/forms/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/forms/applications.py` & `netbox-data-flows-0.7.2/netbox_data_flows/forms/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/forms/dataflows.py` & `netbox-data-flows-0.7.2/netbox_data_flows/forms/dataflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,14 @@
         selector=True,
         help_text="Application that this data flow is part of.",
     )
     group = DynamicModelChoiceField(
         queryset=models.DataFlowGroup.objects.all(),
         required=False,
         selector=True,
-        query_params={
-            "application_id": "$application",
-        },
         help_text=(
             "Parent group of this Data Flow. "
             "Disabling the group will disable this data flow."
         ),
     )
 
     comments = CommentField()
@@ -126,17 +123,14 @@
             "tags",
             "protocol",
             "source_ports",
             "destination_ports",
             "sources",
             "destinations",
         )
-        widgets = {
-            "protocol": forms.Select(),
-        }
         help_texts = {
             "status": (
                 "Status of the data group. If its group is disabled, "
                 "the data flow will also be disabled."
             )
         }
 
@@ -162,20 +156,18 @@
         },
     )
     comments = CommentField()
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=forms.Select(),
     )
     protocol = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowProtocolChoices),
         required=False,
-        widget=forms.Select(),
     )
     source_ports = NumericArrayField(
         base_field=forms.IntegerField(
             min_value=SERVICE_PORT_MIN, max_value=SERVICE_PORT_MAX
         ),
         help_text=(
             "Comma-separated list of one or more port numbers. "
@@ -340,21 +332,19 @@
         help_text="Recursive group(s)",
     )
     tag = TagFilterField(model)
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=forms.Select(),
         help_text="Status of the data flows themselves",
     )
     inherited_status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=forms.Select(),
         help_text="Status inherited from the data flow groups",
     )
 
     protocol = MultipleChoiceField(
         choices=choices.DataFlowProtocolChoices,
         required=False,
     )
@@ -370,15 +360,14 @@
         required=False,
         help_text="Use the API or repeat the URL parameter to select several",
     )
 
     source_is_null = forms.ChoiceField(
         choices=add_blank_choice(choices.TargetIsEmptyChoice),
         required=False,
-        widget=forms.Select(),
         help_text="No sources are defined?",
     )
     source_aliases = DynamicModelMultipleChoiceField(
         queryset=models.ObjectAlias.objects.all(),
         required=False,
         label="Source Object Aliases",
     )
@@ -409,15 +398,14 @@
         label="Source Virtual Machines",
         help_text="Any IP address of the virtual machine",
     )
 
     destination_is_null = forms.ChoiceField(
         choices=add_blank_choice(choices.TargetIsEmptyChoice),
         required=False,
-        widget=forms.Select(),
         help_text="No destinations are defined?",
     )
     destination_aliases = DynamicModelMultipleChoiceField(
         queryset=models.ObjectAlias.objects.all(),
         required=False,
         label="Destination Object Aliases",
     )
```

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/forms/groups.py` & `netbox-data-flows-0.7.2/netbox_data_flows/forms/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,27 +34,21 @@
 
 class DataFlowGroupForm(NetBoxModelForm):
     slug = SlugField()
     application = DynamicModelChoiceField(
         queryset=models.Application.objects.all(),
         required=False,
         selector=True,
-        help_text=(
-            "Application that this data flow group (and all of its "
-            "descendants) is part of."
-        ),
+        help_text="Application that this data flow group is related to.",
     )
     parent = DynamicModelChoiceField(
         queryset=models.DataFlowGroup.objects.all(),
         required=False,
         selector=True,
         help_text="Parent group of this Data Flow Group.",
-        query_params={
-            "application_id": "$application",
-        },
     )
     comments = CommentField()
 
     fieldsets = (
         (
             "Data Flow Group",
             (
@@ -109,15 +103,14 @@
         selector=True,
     )
     comments = CommentField()
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=forms.Select(),
     )
 
     fieldsets = (
         (
             "Data Flow Groups",
             (
                 "application",
@@ -189,20 +182,18 @@
         label="Ancestor group",
         help_text="Recursive parent group(s)",
     )
 
     status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=forms.Select(),
     )
     inherited_status = forms.ChoiceField(
         choices=add_blank_choice(choices.DataFlowStatusChoices),
         required=False,
-        widget=forms.Select(),
     )
 
     fieldsets = (
         (
             None,
             (
                 "filter_id",  # Saved Filter
```

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/forms/objectaliases.py` & `netbox-data-flows-0.7.2/netbox_data_flows/forms/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/graphql/__init__.py` & `netbox-data-flows-0.7.2/netbox_data_flows/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/graphql/applications.py` & `netbox-data-flows-0.7.2/netbox_data_flows/graphql/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/graphql/objectaliases.py` & `netbox-data-flows-0.7.2/netbox_data_flows/graphql/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/management/commands/delete_orphaned_aliases.py` & `netbox-data-flows-0.7.2/netbox_data_flows/management/commands/delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/migrations/0001_initial.py` & `netbox-data-flows-0.7.2/netbox_data_flows/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py` & `netbox-data-flows-0.7.2/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/migrations/0005_dataflowgroup_slug.py` & `netbox-data-flows-0.7.2/netbox_data_flows/migrations/0005_dataflowgroup_slug.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py` & `netbox-data-flows-0.7.2/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py` & `netbox-data-flows-0.7.2/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/models/applications.py` & `netbox-data-flows-0.7.2/netbox_data_flows/models/applications.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,12 +51,18 @@
     )
     contacts = GenericRelation(to="tenancy.ContactAssignment")
     comments = models.TextField(blank=True)
 
     class Meta:
         ordering = ("name",)
 
+    clone_fields = (
+        "description",
+        "role",
+        "comments",
+    )
+
     def __str__(self):
         return self.name
 
     def get_absolute_url(self):
         return reverse("plugins:netbox_data_flows:application", args=[self.pk])
```

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/models/dataflows.py` & `netbox-data-flows-0.7.2/netbox_data_flows/models/dataflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,16 +198,16 @@
         )
 
     objects = DataFlowQuerySet.as_manager()
 
     clone_fields = (
         "application",
         "group",
+        "description",
         "status",
-        "name",
         "comments",
         "protocol",
         "source_ports",
         "destination_ports",
         "sources",
         "destinations",
     )
```

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/models/groups.py` & `netbox-data-flows-0.7.2/netbox_data_flows/models/groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,14 +103,22 @@
                 name="netbox_data_flows_dataflowgroup_application_name",
                 condition=models.Q(parent=None),
             ),
         )
 
     objects = DataFlowGroupManager()
 
+    clone_fields = (
+        "application",
+        "parent",
+        "description",
+        "status",
+        "comments",
+    )
+
     def get_absolute_url(self):
         return reverse(
             "plugins:netbox_data_flows:dataflowgroup", args=[self.pk]
         )
 
     def validate_unique(self, exclude=None):
         if self.parent is None:
```

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/models/objectaliases.py` & `netbox-data-flows-0.7.2/netbox_data_flows/models/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/navigation.py` & `netbox-data-flows-0.7.2/netbox_data_flows/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/search.py` & `netbox-data-flows-0.7.2/netbox_data_flows/search.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/tables/applications.py` & `netbox-data-flows-0.7.2/netbox_data_flows/tables/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/tables/dataflows.py` & `netbox-data-flows-0.7.2/netbox_data_flows/tables/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/tables/groups.py` & `netbox-data-flows-0.7.2/netbox_data_flows/tables/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/tables/objectaliases.py` & `netbox-data-flows-0.7.2/netbox_data_flows/tables/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/application.html` & `netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/application.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/applicationrole.html` & `netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/applicationrole.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow.html` & `netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/dataflow.html`

 * *Files 5% similar despite different names*

```diff
@@ -10,46 +10,46 @@
   {% if object.application %}
   <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_data_flows:dataflow_list' %}?application_id={{ object.application.pk }}">{{ object.application }}</a></li>
   {% endif %}
 {% endblock %}
 
 {% block content %}
   <div class="row mb-3">
-    <div class="col col-md-4">
+    <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Data Flow</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Application</th>
               <td>{{ object.application|linkify }}</td>
             </tr>
             <tr>
+              <th scope="row">Group</th>
+              <td>
+                {{ object.group|placeholder|linkify }}
+              </td>
+            </tr>
+            <tr>
               <th scope="row">Description</th>
               <td>{{ object.description|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Status</th>
               <td>{% badge object.inherited_status_display bg_color=object.get_status_color %}</td>
             </tr>
-            <tr>
-              <th scope="row">Parent</th>
-              <td>
-                {{ object.parent|placeholder|linkify }}
-              </td>
-            </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
     </div>
-    <div class="col col-md-8">
+    <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Specifications</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Protocol</th>
               <td>{{ object.get_protocol_display|placeholder }}</td>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 {% extends 'generic/object.html' %} {% load buttons %} {% load helpers %} {%
 load perms %} {% load plugins %} {% load render_table from django_tables2 %} {%
 block breadcrumbs %} {{ block.super }} {% if object.application %}
 {{_object.application_}}
 {% endif %} {% endblock %} {% block content %}
 ** Data Flow **
 Application {{ object.application|linkify }}
+Group       {{ object.group|placeholder|linkify }}
 Description {{ object.description|placeholder }}
 Status      {% badge object.inherited_status_display
             bg_color=object.get_status_color %}
-Parent      {{ object.parent|placeholder|linkify }}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
 ** Specifications **
 Protocol          {{ object.get_protocol_display|placeholder }}
 Source ports      {{ object.source_port_list|placeholder }}
 Destination ports {{ object.destination_port_list|placeholder }}
 Sources           {{ o|linkify }}
```

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html` & `netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html` & `netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html` & `netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html` & `netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,43 +14,43 @@
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Data Flow Group</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
+              <th scope="row">Application</th>
+              <td>{{ object.application|linkify }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Parent</th>
+              <td>
+                {{ object.parent|placeholder|linkify }}
+              </td>
+            </tr>
+            <tr>
               <th scope="row">Name</th>
               <td>
                 {{ object.name }}
               </td>
             </tr>
             <tr>
               <th scope="row">Slug</th>
               <td>
                 {{ object.slug }}
               </td>
             </tr>
             <tr>
-              <th scope="row">Application</th>
-              <td>{{ object.application|linkify }}</td>
-            </tr>
-            <tr>
               <th scope="row">Description</th>
               <td>{{ object.description|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Status</th>
               <td>{% badge object.inherited_status_display bg_color=object.get_status_color %}</td>
             </tr>
-            <tr>
-              <th scope="row">Parent</th>
-              <td>
-                {{ object.parent|placeholder|linkify }}
-              </td>
-            </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
 {% extends 'generic/object.html' %} {% load buttons %} {% load helpers %} {%
 load perms %} {% load plugins %} {% load render_table from django_tables2 %} {%
 block breadcrumbs %} {{ block.super }}
 {{_object.application_}}
 {% endblock %} {% block content %}
 ** Data Flow Group **
+Application {{ object.application|linkify }}
+Parent      {{ object.parent|placeholder|linkify }}
 Name        {{ object.name }}
 Slug        {{ object.slug }}
-Application {{ object.application|linkify }}
 Description {{ object.description|placeholder }}
 Status      {% badge object.inherited_status_display
             bg_color=object.get_status_color %}
-Parent      {{ object.parent|placeholder|linkify }}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
 ** Child Groups **
 {% render_table children_table %}
 {% plugin_right_page object %}
 {% if dataflows_table %}
 ** Data Flows (direct members) **
```

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/objectalias.html` & `netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/objectalias.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html` & `netbox-data-flows-0.7.2/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/urls.py` & `netbox-data-flows-0.7.2/netbox_data_flows/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/utils/aliases.py` & `netbox-data-flows-0.7.2/netbox_data_flows/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/utils/helpers.py` & `netbox-data-flows-0.7.2/netbox_data_flows/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/views/applicationroles.py` & `netbox-data-flows-0.7.2/netbox_data_flows/views/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/views/applications.py` & `netbox-data-flows-0.7.2/netbox_data_flows/views/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/views/dataflows.py` & `netbox-data-flows-0.7.2/netbox_data_flows/views/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/views/groups.py` & `netbox-data-flows-0.7.2/netbox_data_flows/views/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/views/model_tabs.py` & `netbox-data-flows-0.7.2/netbox_data_flows/views/model_tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows/views/objectaliases.py` & `netbox-data-flows-0.7.2/netbox_data_flows/views/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows.egg-info/PKG-INFO` & `netbox-data-flows-0.7.2/netbox_data_flows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.7.1
+Version: 0.7.2
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `netbox-data-flows-0.7.1/netbox_data_flows.egg-info/SOURCES.txt` & `netbox-data-flows-0.7.2/netbox_data_flows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.1/pyproject.toml` & `netbox-data-flows-0.7.2/pyproject.toml`

 * *Files identical despite different names*

