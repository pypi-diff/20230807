# Comparing `tmp/google-dataproc-templates-0.3.0b0.tar.gz` & `tmp/google-dataproc-templates-0.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-dataproc-templates-0.3.0b0.tar", last modified: Fri May 12 16:47:25 2023, max compression
+gzip compressed data, was "google-dataproc-templates-0.4.0b0.tar", last modified: Mon Aug  7 15:46:08 2023, max compression
```

## Comparing `google-dataproc-templates-0.3.0b0.tar` & `google-dataproc-templates-0.4.0b0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/azure/azure_blob_storage_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/base_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_bigtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_jdbc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/text_to_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/hbase/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hbase/hbase_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/hive_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/hive_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.695218 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/kafka_to_bq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/kafka_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/mongo/mongo_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/pubsublite_to_bigtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/pubsublite_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/redshift/redshift_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/s3/s3_to_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/template_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/dataproc_templates/util/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/dataframe_reader_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/dataframe_writer_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24057 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/template_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/dataproc_templates/util/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.699218 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-12 16:47:25.000000 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-12 16:47:25.000000 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:47:25.000000 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 16:47:25.000000 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 16:47:25.000000 google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.691218 google-dataproc-templates-0.3.0b0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/azure/test_azure_blob_storage_to_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/bigquery/test_bigquery_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/cassandra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/cassandra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/cassandra/test_cassandra_to_bq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/cassandra/test_cassandra_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/gcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_bigtable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_jdbc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/gcs/test_text_to_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/hbase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hbase/test_hbase_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/hive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hive/test_hive_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hive/test_hive_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/hive/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hive/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/hive/util/test_hive_ddl_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/jdbc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/jdbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_jdbc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.703218 google-dataproc-templates-0.3.0b0/test/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/mongo/test_mongo_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/test/pubsublite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/pubsublite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/pubsublite/test_pubsublite_to_bigtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/pubsublite/test_pubsublite_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/test/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/redshift/test_redshift_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/test/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/s3/test_s3_to_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:25.707218 google-dataproc-templates-0.3.0b0/test/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/test/util/test_argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-12 16:47:11.000000 google-dataproc-templates-0.3.0b0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.649183 google-dataproc-templates-0.4.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-08-07 15:46:08.649183 google-dataproc-templates-0.4.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.637183 google-dataproc-templates-0.4.0b0/dataproc_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.637183 google-dataproc-templates-0.4.0b0/dataproc_templates/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/azure/azure_blob_storage_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/base_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.637183 google-dataproc-templates-0.4.0b0/dataproc_templates/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.637183 google-dataproc-templates-0.4.0b0/dataproc_templates/cassandra/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/cassandra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/gcs_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/gcs_to_bigtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/gcs_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/gcs_to_jdbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/gcs_to_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/text_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/hbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/hbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/hbase/hbase_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/hive/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/hive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/hive/hive_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/hive/hive_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/hive/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/hive/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/jdbc/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/jdbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/kafka/kafka_to_bq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/kafka/kafka_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/mongo/mongo_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/pubsublite/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/pubsublite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/pubsublite/pubsublite_to_bigtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/pubsublite/pubsublite_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/redshift/redshift_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/s3/s3_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/template_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.641183 google-dataproc-templates-0.4.0b0/dataproc_templates/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/util/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/util/dataframe_reader_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/util/dataframe_writer_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24057 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/util/template_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/dataproc_templates/util/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/google_dataproc_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-08-07 15:46:08.000000 google-dataproc-templates-0.4.0b0/google_dataproc_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-07 15:46:08.000000 google-dataproc-templates-0.4.0b0/google_dataproc_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:46:08.000000 google-dataproc-templates-0.4.0b0/google_dataproc_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 15:46:08.000000 google-dataproc-templates-0.4.0b0/google_dataproc_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-07 15:46:08.000000 google-dataproc-templates-0.4.0b0/google_dataproc_templates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-07 15:46:08.649183 google-dataproc-templates-0.4.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.637183 google-dataproc-templates-0.4.0b0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/azure/test_azure_blob_storage_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/bigquery/test_bigquery_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/cassandra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/cassandra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/cassandra/test_cassandra_to_bq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/cassandra/test_cassandra_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/gcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/gcs/test_gcs_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/gcs/test_gcs_to_bigtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/gcs/test_gcs_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/gcs/test_gcs_to_jdbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/gcs/test_gcs_to_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/gcs/test_text_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/hbase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/hbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/hbase/test_hbase_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/hive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/hive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/hive/test_hive_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/hive/test_hive_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/hive/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/hive/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/hive/util/test_hive_ddl_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/jdbc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/jdbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/jdbc/test_jdbc_to_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/jdbc/test_jdbc_to_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/jdbc/test_jdbc_to_jdbc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/mongo/test_mongo_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/pubsublite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/pubsublite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/pubsublite/test_pubsublite_to_bigtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/pubsublite/test_pubsublite_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/redshift/test_redshift_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.645183 google-dataproc-templates-0.4.0b0/test/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/s3/test_s3_to_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:46:08.649183 google-dataproc-templates-0.4.0b0/test/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/test/util/test_argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 15:45:59.000000 google-dataproc-templates-0.4.0b0/version.py
```

### Comparing `google-dataproc-templates-0.3.0b0/MANIFEST.in` & `google-dataproc-templates-0.4.0b0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/PKG-INFO` & `google-dataproc-templates-0.4.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-dataproc-templates
-Version: 0.3.0b0
+Version: 0.4.0b0
 Summary: Google Dataproc templates written in Python
 Home-page: https://github.com/GoogleCloudPlatform/dataproc-templates
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -28,15 +28,14 @@
 * [JDBCToBigQuery](/python/dataproc_templates/jdbc#3-jdbc-to-bigquery) (blogpost [link](https://medium.com/@sjlva/python-fast-export-large-database-tables-using-gcp-serverless-dataproc-bfe77a132485))
 * [JDBCToGCS](/python/dataproc_templates/jdbc#2-jdbc-to-gcs) (blogpost [link](https://medium.com/google-cloud/importing-data-from-databases-into-gcs-via-jdbc-using-dataproc-serverless-f330cb0160f0))
 * [JDBCToJDBC](/python/dataproc_templates/jdbc#1-jdbc-to-jdbc) (blogpost [link](https://medium.com/google-cloud/migrating-data-from-one-databases-into-another-via-jdbc-using-dataproc-serverless-c5336c409b18))
 * [KafkaToGCS](/python/dataproc_templates/kafka/#kafka-to-gcs)
 * [KafkaToBigQuery](/python/dataproc_templates/kafka/#kafka-to-bigquery)
 * [MongoToGCS](/python/dataproc_templates/mongo#mongo-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-mongodb-to-gcs-buckets-using-dataproc-serverless-64830fb15b51))
 * [PubSubLiteToBigtable](/python/dataproc_templates/pubsublite#pubsublite-to-bigtable)
-* [PubSubLiteToGCS](/python/dataproc_templates/pubsublite#pubsublite-to-gcs)
 * [RedshiftToGCS](/python/dataproc_templates/redshift#redshift-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-redshift-to-gcs-using-gcp-dataproc-serverless-and-pyspark-9ab78de11405))
 * [S3ToBigQuery](/python/dataproc_templates/s3#amazon-s3-to-bigquery)
 * [SnowflakeToGCS](/python/dataproc_templates/snowflake#1-snowflake-to-gcs)(blogpost [link](https://medium.com/@varunikagupta96/exporting-data-from-snowflake-to-gcs-using-pyspark-on-dataproc-serverless-363d3bed551b))
 * [TextToBigQuery](/python/dataproc_templates/gcs#text-to-bigquery)
 
 
 Dataproc Templates (Python - PySpark) submit jobs to Dataproc Serverless using [batches submit pyspark](https://cloud.google.com/sdk/gcloud/reference/dataproc/batches/submit/pyspark).
```

### Comparing `google-dataproc-templates-0.3.0b0/README.md` & `google-dataproc-templates-0.4.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 * [JDBCToBigQuery](/python/dataproc_templates/jdbc#3-jdbc-to-bigquery) (blogpost [link](https://medium.com/@sjlva/python-fast-export-large-database-tables-using-gcp-serverless-dataproc-bfe77a132485))
 * [JDBCToGCS](/python/dataproc_templates/jdbc#2-jdbc-to-gcs) (blogpost [link](https://medium.com/google-cloud/importing-data-from-databases-into-gcs-via-jdbc-using-dataproc-serverless-f330cb0160f0))
 * [JDBCToJDBC](/python/dataproc_templates/jdbc#1-jdbc-to-jdbc) (blogpost [link](https://medium.com/google-cloud/migrating-data-from-one-databases-into-another-via-jdbc-using-dataproc-serverless-c5336c409b18))
 * [KafkaToGCS](/python/dataproc_templates/kafka/#kafka-to-gcs)
 * [KafkaToBigQuery](/python/dataproc_templates/kafka/#kafka-to-bigquery)
 * [MongoToGCS](/python/dataproc_templates/mongo#mongo-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-mongodb-to-gcs-buckets-using-dataproc-serverless-64830fb15b51))
 * [PubSubLiteToBigtable](/python/dataproc_templates/pubsublite#pubsublite-to-bigtable)
-* [PubSubLiteToGCS](/python/dataproc_templates/pubsublite#pubsublite-to-gcs)
 * [RedshiftToGCS](/python/dataproc_templates/redshift#redshift-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-redshift-to-gcs-using-gcp-dataproc-serverless-and-pyspark-9ab78de11405))
 * [S3ToBigQuery](/python/dataproc_templates/s3#amazon-s3-to-bigquery)
 * [SnowflakeToGCS](/python/dataproc_templates/snowflake#1-snowflake-to-gcs)(blogpost [link](https://medium.com/@varunikagupta96/exporting-data-from-snowflake-to-gcs-using-pyspark-on-dataproc-serverless-363d3bed551b))
 * [TextToBigQuery](/python/dataproc_templates/gcs#text-to-bigquery)
 
 
 Dataproc Templates (Python - PySpark) submit jobs to Dataproc Serverless using [batches submit pyspark](https://cloud.google.com/sdk/gcloud/reference/dataproc/batches/submit/pyspark).
```

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/azure/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/azure/azure_blob_storage_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/azure/azure_blob_storage_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/base_template.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/base_template.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/bigquery/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/bigquery/bigquery_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/cassandra/cassandra_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/cassandra/cassandra_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/gcs_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_bigtable.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/gcs_to_bigtable.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_gcs.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/gcs_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_jdbc.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/gcs_to_jdbc.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/gcs_to_mongo.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/gcs_to_mongo.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/gcs/text_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/gcs/text_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/hbase/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/hbase/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/hbase/hbase_to_gcs.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/hbase/hbase_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/hive/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/hive/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/hive/hive_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/hive/hive_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/hive/hive_to_gcs.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/hive/hive_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/hive/util/hive_ddl_extractor.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/jdbc/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/jdbc/jdbc_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/jdbc/jdbc_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/jdbc/jdbc_to_jdbc.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/kafka_to_bq.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/kafka/kafka_to_bq.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/kafka/kafka_to_gcs.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/kafka/kafka_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/mongo/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/mongo/mongo_to_gcs.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/mongo/mongo_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/pubsublite/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/pubsublite_to_bigtable.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/pubsublite/pubsublite_to_bigtable.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/pubsublite/pubsublite_to_gcs.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/pubsublite/pubsublite_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/redshift/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/redshift/redshift_to_gcs.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/redshift/redshift_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/s3/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/s3/s3_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/s3/s3_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/snowflake/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/snowflake/snowflake_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/template_name.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/template_name.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/util/__init__.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/util/__init__.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/util/argument_parsing.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/util/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/util/dataframe_reader_wrappers.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/util/dataframe_reader_wrappers.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/util/dataframe_writer_wrappers.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/util/dataframe_writer_wrappers.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/util/template_constants.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/util/template_constants.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/dataproc_templates/util/tracking.py` & `google-dataproc-templates-0.4.0b0/dataproc_templates/util/tracking.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/PKG-INFO` & `google-dataproc-templates-0.4.0b0/google_dataproc_templates.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-dataproc-templates
-Version: 0.3.0b0
+Version: 0.4.0b0
 Summary: Google Dataproc templates written in Python
 Home-page: https://github.com/GoogleCloudPlatform/dataproc-templates
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -28,15 +28,14 @@
 * [JDBCToBigQuery](/python/dataproc_templates/jdbc#3-jdbc-to-bigquery) (blogpost [link](https://medium.com/@sjlva/python-fast-export-large-database-tables-using-gcp-serverless-dataproc-bfe77a132485))
 * [JDBCToGCS](/python/dataproc_templates/jdbc#2-jdbc-to-gcs) (blogpost [link](https://medium.com/google-cloud/importing-data-from-databases-into-gcs-via-jdbc-using-dataproc-serverless-f330cb0160f0))
 * [JDBCToJDBC](/python/dataproc_templates/jdbc#1-jdbc-to-jdbc) (blogpost [link](https://medium.com/google-cloud/migrating-data-from-one-databases-into-another-via-jdbc-using-dataproc-serverless-c5336c409b18))
 * [KafkaToGCS](/python/dataproc_templates/kafka/#kafka-to-gcs)
 * [KafkaToBigQuery](/python/dataproc_templates/kafka/#kafka-to-bigquery)
 * [MongoToGCS](/python/dataproc_templates/mongo#mongo-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-mongodb-to-gcs-buckets-using-dataproc-serverless-64830fb15b51))
 * [PubSubLiteToBigtable](/python/dataproc_templates/pubsublite#pubsublite-to-bigtable)
-* [PubSubLiteToGCS](/python/dataproc_templates/pubsublite#pubsublite-to-gcs)
 * [RedshiftToGCS](/python/dataproc_templates/redshift#redshift-to-gcs)(blogpost [link](https://medium.com/google-cloud/exporting-data-from-redshift-to-gcs-using-gcp-dataproc-serverless-and-pyspark-9ab78de11405))
 * [S3ToBigQuery](/python/dataproc_templates/s3#amazon-s3-to-bigquery)
 * [SnowflakeToGCS](/python/dataproc_templates/snowflake#1-snowflake-to-gcs)(blogpost [link](https://medium.com/@varunikagupta96/exporting-data-from-snowflake-to-gcs-using-pyspark-on-dataproc-serverless-363d3bed551b))
 * [TextToBigQuery](/python/dataproc_templates/gcs#text-to-bigquery)
 
 
 Dataproc Templates (Python - PySpark) submit jobs to Dataproc Serverless using [batches submit pyspark](https://cloud.google.com/sdk/gcloud/reference/dataproc/batches/submit/pyspark).
```

### Comparing `google-dataproc-templates-0.3.0b0/google_dataproc_templates.egg-info/SOURCES.txt` & `google-dataproc-templates-0.4.0b0/google_dataproc_templates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/setup.py` & `google-dataproc-templates-0.4.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/azure/test_azure_blob_storage_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/test/azure/test_azure_blob_storage_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/bigquery/test_bigquery_to_gcs.py` & `google-dataproc-templates-0.4.0b0/test/bigquery/test_bigquery_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/cassandra/test_cassandra_to_bq.py` & `google-dataproc-templates-0.4.0b0/test/cassandra/test_cassandra_to_bq.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/cassandra/test_cassandra_to_gcs.py` & `google-dataproc-templates-0.4.0b0/test/cassandra/test_cassandra_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/test/gcs/test_gcs_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_bigtable.py` & `google-dataproc-templates-0.4.0b0/test/gcs/test_gcs_to_bigtable.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_gcs.py` & `google-dataproc-templates-0.4.0b0/test/gcs/test_gcs_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_jdbc.py` & `google-dataproc-templates-0.4.0b0/test/gcs/test_gcs_to_jdbc.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/gcs/test_gcs_to_mongo.py` & `google-dataproc-templates-0.4.0b0/test/gcs/test_gcs_to_mongo.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/gcs/test_text_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/test/gcs/test_text_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/hbase/test_hbase_to_gcs.py` & `google-dataproc-templates-0.4.0b0/test/hbase/test_hbase_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/hive/test_hive_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/test/hive/test_hive_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/hive/test_hive_to_gcs.py` & `google-dataproc-templates-0.4.0b0/test/hive/test_hive_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/hive/util/test_hive_ddl_extractor.py` & `google-dataproc-templates-0.4.0b0/test/hive/util/test_hive_ddl_extractor.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/test/jdbc/test_jdbc_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_gcs.py` & `google-dataproc-templates-0.4.0b0/test/jdbc/test_jdbc_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/jdbc/test_jdbc_to_jdbc.py` & `google-dataproc-templates-0.4.0b0/test/jdbc/test_jdbc_to_jdbc.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/mongo/test_mongo_to_gcs.py` & `google-dataproc-templates-0.4.0b0/test/mongo/test_mongo_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/pubsublite/test_pubsublite_to_bigtable.py` & `google-dataproc-templates-0.4.0b0/test/pubsublite/test_pubsublite_to_bigtable.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/pubsublite/test_pubsublite_to_gcs.py` & `google-dataproc-templates-0.4.0b0/test/pubsublite/test_pubsublite_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/redshift/test_redshift_to_gcs.py` & `google-dataproc-templates-0.4.0b0/test/redshift/test_redshift_to_gcs.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/s3/test_s3_to_bigquery.py` & `google-dataproc-templates-0.4.0b0/test/s3/test_s3_to_bigquery.py`

 * *Files identical despite different names*

### Comparing `google-dataproc-templates-0.3.0b0/test/util/test_argument_parsing.py` & `google-dataproc-templates-0.4.0b0/test/util/test_argument_parsing.py`

 * *Files identical despite different names*

