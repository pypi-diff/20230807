# Comparing `tmp/vdk-impala-0.4.953562131.tar.gz` & `tmp/vdk-impala-0.4.957849598.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-impala-0.4.953562131.tar", last modified: Wed Aug  2 15:48:37 2023, max compression
+gzip compressed data, was "vdk-impala-0.4.957849598.tar", last modified: Mon Aug  7 09:02:09 2023, max compression
```

## Comparing `vdk-impala-0.4.953562131.tar` & `vdk-impala-0.4.957849598.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6530 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5936 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-08-02 15:48:24.000000 vdk-impala-0.4.953562131/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/
--rw-rw-rw-   0 root         (0) root         (0)     7458 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     2060 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_error_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)    20341 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7846 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7448 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_lineage_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6850 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/data_quality_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/
--rw-rw-rw-   0 root         (0) root         (0)      894 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     2703 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-02 15:48:19.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     1718 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     3373 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.944859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-create-consolidated-view.sql
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/04-compute-stats.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.948859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.952859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-overwrite-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.952859 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/
--rw-rw-rw-   0 root         (0) root         (0)     3032 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     4358 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/template_arguments_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2298 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.952859 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6530 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3918 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-08-02 15:48:37.000000 vdk-impala-0.4.953562131/src/vdk_impala.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.952859 vdk-impala-0.4.953562131/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/tests/functional/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.940859 vdk-impala-0.4.953562131/tests/functional/jobs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job/10_create_table.sql
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job/20_populate_table.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job-non-lineage/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job-non-lineage/10_create_table.sql
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job-non-lineage/20_compute_table.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 15:48:37.956859 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job-syntax-error/
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/functional/jobs/sql-job-syntax-error/10_bad_query.sql
--rw-rw-rw-   0 root         (0) root         (0)     3952 2023-08-02 15:48:20.000000 vdk-impala-0.4.953562131/tests/test_error_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.911789 vdk-impala-0.4.957849598/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-08-07 09:02:09.911789 vdk-impala-0.4.957849598/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5936 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 09:02:09.911789 vdk-impala-0.4.957849598/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-08-07 09:01:57.000000 vdk-impala-0.4.957849598/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.899789 vdk-impala-0.4.957849598/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.895789 vdk-impala-0.4.957849598/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.895789 vdk-impala-0.4.957849598/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.903789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/
+-rw-rw-rw-   0 root         (0) root         (0)     7458 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_error_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    21129 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7846 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7448 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_lineage_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6850 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.903789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/data_quality_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.903789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.903789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.903789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/
+-rw-rw-rw-   0 root         (0) root         (0)      894 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2703 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.903789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.907789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd2/
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd2/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd2/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd2/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.907789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.907789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/insert/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/insert/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3373 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.907789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-create-consolidated-view.sql
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/insert/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/insert/04-compute-stats.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.907789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.907789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-overwrite-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.907789 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/versioned/
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/versioned/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4358 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/versioned/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/versioned/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/versioned/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/template_arguments_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.911789 vdk-impala-0.4.957849598/src/vdk_impala.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-08-07 09:02:09.000000 vdk-impala-0.4.957849598/src/vdk_impala.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-08-07 09:02:09.000000 vdk-impala-0.4.957849598/src/vdk_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:02:09.000000 vdk-impala-0.4.957849598/src/vdk_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-08-07 09:02:09.000000 vdk-impala-0.4.957849598/src/vdk_impala.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-08-07 09:02:09.000000 vdk-impala-0.4.957849598/src/vdk_impala.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-08-07 09:02:09.000000 vdk-impala-0.4.957849598/src/vdk_impala.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.911789 vdk-impala-0.4.957849598/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.899789 vdk-impala-0.4.957849598/tests/functional/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.899789 vdk-impala-0.4.957849598/tests/functional/jobs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.911789 vdk-impala-0.4.957849598/tests/functional/jobs/sql-job/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/tests/functional/jobs/sql-job/10_create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/tests/functional/jobs/sql-job/20_populate_table.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.911789 vdk-impala-0.4.957849598/tests/functional/jobs/sql-job-non-lineage/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/tests/functional/jobs/sql-job-non-lineage/10_create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/tests/functional/jobs/sql-job-non-lineage/20_compute_table.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:02:09.911789 vdk-impala-0.4.957849598/tests/functional/jobs/sql-job-syntax-error/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/tests/functional/jobs/sql-job-syntax-error/10_bad_query.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2023-08-07 09:01:52.000000 vdk-impala-0.4.957849598/tests/test_error_classifier.py
```

### Comparing `vdk-impala-0.4.953562131/PKG-INFO` & `vdk-impala-0.4.957849598/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-impala
-Version: 0.4.953562131
+Version: 0.4.957849598
 Summary: Versatile Data Kit SDK plugin provides support for Impala database.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-impala-0.4.953562131/README.md` & `vdk-impala-0.4.957849598/README.md`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/setup.py` & `vdk-impala-0.4.957849598/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.4.953562131"
+__version__ = "0.4.957849598"
 
 setuptools.setup(
     name="vdk-impala",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin provides support for Impala database.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_configuration.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_connection.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_error_classifier.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_error_classifier.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_error_handler.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_error_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,30 +37,30 @@
             1. Examine exception to detect if this is the case;
             2. If it is, then issue a refresh for the table whose files could not be found;
             3. Re-try the query.
 
         :param caught_exception: the caught Impala exception
         :param recovery_cursor: cursor that can be used to execute recovery queries and query retries against Impala
         :return: true if and only if the exception was handled successfully and the query passed has succeeded.
-                Otherwise return false - the caught_exception was not handled.
+                Otherwise, return false - the caught_exception was not handled.
                 This method will raise an exception in the following scenarios and assuming handling of the error
                 produced another exception:
                  1. Exceptions are of the same type but have different args.
                  2. Exceptions are different types.
                 Moreover, the root cause stack trace will appear in the error message if an exception is raised.
-                Otherwise stacktrace gets changed and becomes confusing.
+                Otherwise, stacktrace gets changed and becomes confusing.
         """
         if self._handle_should_not_retry_error(caught_exception):
             return False
 
         if self._is_pool_error(caught_exception):
             errors.log_and_throw(
                 to_be_fixed_by=errors.ResolvableBy.USER_ERROR,
                 log=self._log,
-                what_happened="An Impala Pool Error occured: " + str(caught_exception),
+                what_happened="An Impala Pool Error occurred: " + str(caught_exception),
                 why_it_happened="Review the contents of the exception.",
                 consequences="The queries will not be executed.",
                 countermeasures=(
                     "Optimise the executed queries. Alternatively, make sure that "
                     "the data job is not running too many queries in parallel."
                 ),
             )
@@ -147,21 +147,29 @@
                     "This is most likely due to delay metadata sync from compaction. "
                     f"We are issuing refresh statement for the offending table: {database}.{table}"
                     " and retrying the query"
                     f"Error was: {exception.__class__}: {str(exception)}"
                 )
                 # Try refreshing the table metadata several times,
                 # and if the issue is not fixed invalidate the metadata.
-                if recovery_cursor.get_retries() > 3:
-                    recovery_cursor.execute(
-                        "invalidate metadata `" + database + "`.`" + table + "`"
-                    )
-                else:
-                    recovery_cursor.execute(
-                        "refresh `" + database + "`.`" + table + "`"
+                try:
+                    if recovery_cursor.get_retries() > 3:
+                        recovery_cursor.execute(
+                            "invalidate metadata `" + database + "`.`" + table + "`"
+                        )
+                    else:
+                        recovery_cursor.execute(
+                            "refresh `" + database + "`.`" + table + "`"
+                        )
+                        time.sleep(
+                            2 ** recovery_cursor.get_retries() * self._backoff_seconds
+                        )  # exponential backoff 30s, 60s, 2m, 4m, 8m
+                except Exception as e:
+                    self._log.info(
+                        f"Refresh/Invalidate metadata operation failed with error: {e}"
                     )
                     time.sleep(
                         2 ** recovery_cursor.get_retries() * self._backoff_seconds
                     )  # exponential backoff 30s, 60s, 2m, 4m, 8m
                 recovery_cursor.retry_operation()
                 return True
             else:
@@ -294,17 +302,22 @@
 
             # Get the fully qualified table name from the exception message.
             matcher = re.compile(pattern=pattern_for_the_table_name)
             results = matcher.search(str(exception).strip())
             if results and len(results.groups()) == 1:
                 fully_qualified_table_name = results.group(1)
                 # invalidate the metadata for the missing table
-                recovery_cursor.execute(
-                    f"invalidate metadata {fully_qualified_table_name}"
-                )
+                try:
+                    recovery_cursor.execute(
+                        f"invalidate metadata {fully_qualified_table_name}"
+                    )
+                except Exception as e:
+                    self._log.info(
+                        f"Invalidate metadata operation failed with error: {e}"
+                    )
                 # wait a little before retrying the query, relaxing the stress on the metastore service
                 self._log.info(
                     f"Sleeping for {sleep_seconds} seconds before retrying the query ..."
                 )
                 time.sleep(sleep_seconds)  # exponential backoff 30s, 60s, 2m, 4m, 8m
                 # retry the query
                 recovery_cursor.retry_operation()
@@ -383,15 +396,18 @@
                 f"Query failed with: {exception.__class__} : {str(exception)}"
                 f"Will sleep for {sleep_seconds} seconds, will issue invalidate"
                 " metadata on the table and try the query again."
             )
 
             # invalidate the metadata for the table. This is necessary in case the metadata for the table
             # has not been propagated before the query is executed again.
-            recovery_cursor.execute(f"invalidate metadata {detected_table}")
+            try:
+                recovery_cursor.execute(f"invalidate metadata {detected_table}")
+            except Exception as e:
+                self._log.info(f"Invalidate metadata operation failed with error: {e}")
             # wait a little before retrying the query, relaxing the stress on the metastore service
             self._log.info(
                 f"Sleeping for {sleep_seconds} seconds before retrying the query ..."
             )
             time.sleep(sleep_seconds)  # sleep for 20s
             # retry the query
             try:
```

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_helper.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_helper.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_lineage_plugin.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_lineage_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/impala_plugin.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/impala_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/data_quality_exception.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/data_quality_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/template_arguments_validator.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/template_arguments_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk/plugin/impala/templates/utility.py` & `vdk-impala-0.4.957849598/src/vdk/plugin/impala/templates/utility.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/src/vdk_impala.egg-info/PKG-INFO` & `vdk-impala-0.4.957849598/src/vdk_impala.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-impala
-Version: 0.4.953562131
+Version: 0.4.957849598
 Summary: Versatile Data Kit SDK plugin provides support for Impala database.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-impala-0.4.953562131/src/vdk_impala.egg-info/SOURCES.txt` & `vdk-impala-0.4.957849598/src/vdk_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.953562131/tests/test_error_classifier.py` & `vdk-impala-0.4.957849598/tests/test_error_classifier.py`

 * *Files identical despite different names*

