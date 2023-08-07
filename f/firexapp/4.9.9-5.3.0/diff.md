# Comparing `tmp/firexapp-4.9.9.tar.gz` & `tmp/firexapp-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firexapp-4.9.9.tar", last modified: Mon Nov 29 20:50:19 2021, max compression
+gzip compressed data, was "firexapp-5.3.0.tar", last modified: Mon Aug  7 19:31:29 2023, max compression
```

## Comparing `firexapp-4.9.9.tar` & `firexapp-5.3.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.169857 firexapp-4.9.9/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1592 2021-11-29 20:50:02.000000 firexapp-4.9.9/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      155 2021-11-29 20:50:02.000000 firexapp-4.9.9/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      463 2021-11-29 20:50:19.169857 firexapp-4.9.9/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       17 2021-11-29 20:50:02.000000 firexapp-4.9.9/README.md
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2021-11-29 20:50:02.000000 firexapp-4.9.9/fastentrypoints.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.170857 firexapp-4.9.9/firexapp/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       45 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/__main__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      497 2021-11-29 20:50:19.170857 firexapp-4.9.9/firexapp/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6113 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/application.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.158856 firexapp-4.9.9/firexapp/broker_manager/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      685 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/broker_manager/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3100 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/broker_manager/broker_factory.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    13245 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/broker_manager/redis_manager.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    12709 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/celery_manager.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6647 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/common.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6676 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/discovery.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.159856 firexapp-4.9.9/firexapp/engine/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/engine/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1599 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/engine/celery.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2044 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/engine/default_celery_config.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5318 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/engine/logging.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.161856 firexapp-4.9.9/firexapp/events/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/events/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3756 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/events/broker_event_consumer.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    12149 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/events/event_aggregator.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3475 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/events/model.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1827 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/fileregistry.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    14695 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/firex_subprocess.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    11065 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/info.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    10435 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/plugins.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.162856 firexapp-4.9.9/firexapp/reporters/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/reporters/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5173 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/reporters/json_reporter.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.165856 firexapp-4.9.9/firexapp/submit/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    10084 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/arguments.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5301 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/console.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7692 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/install_configs.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      907 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/report_trigger.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5468 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/reporting.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     9212 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/shutdown.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    29935 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/submit.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1490 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/tracking_service.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3250 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/uid.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.167857 firexapp-4.9.9/firexapp/tasks/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/tasks/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3226 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/tasks/core_tasks.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6445 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/tasks/example.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3247 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/tasks/root_tasks.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.169857 firexapp-4.9.9/firexapp/testing/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4323 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/config_base.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    13199 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/config_interpreter.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1099 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/coverage_plugin.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3168 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/pydev_debug_plugin.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7228 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/test_infra.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.157856 firexapp-4.9.9/firexapp.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      463 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)     1598 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      191 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      187 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        9 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      267 2021-11-29 20:50:19.170857 firexapp-4.9.9/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1690 2021-11-29 20:50:02.000000 firexapp-4.9.9/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2021-11-29 20:50:02.000000 firexapp-4.9.9/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.508924 firexapp-5.3.0/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2023-08-07 19:31:14.000000 firexapp-5.3.0/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      155 2023-08-07 19:31:14.000000 firexapp-5.3.0/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      435 2023-08-07 19:31:29.509925 firexapp-5.3.0/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       17 2023-08-07 19:31:14.000000 firexapp-5.3.0/README.md
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2023-08-07 19:31:14.000000 firexapp-5.3.0/fastentrypoints.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.509925 firexapp-5.3.0/firexapp/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       45 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/__main__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      497 2023-08-07 19:31:29.509925 firexapp-5.3.0/firexapp/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7352 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/application.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.500924 firexapp-5.3.0/firexapp/broker_manager/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      699 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/broker_manager/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3100 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/broker_manager/broker_factory.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    13497 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/broker_manager/redis_manager.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    13246 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/celery_manager.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6680 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/common.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6676 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/discovery.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.501924 firexapp-5.3.0/firexapp/engine/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/engine/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1599 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/engine/celery.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4667 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/engine/default_celery_config.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6851 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/engine/logging.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.502925 firexapp-5.3.0/firexapp/events/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/events/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4726 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/events/broker_event_consumer.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    14847 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/events/event_aggregator.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3571 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/events/model.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1827 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/fileregistry.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    15762 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/firex_subprocess.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11065 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/info.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11513 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/plugins.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.503924 firexapp-5.3.0/firexapp/reporters/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/reporters/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6049 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/reporters/json_reporter.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.505924 firexapp-5.3.0/firexapp/submit/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    10084 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/arguments.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5627 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/console.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7692 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/install_configs.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      907 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/report_trigger.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5423 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/reporting.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     9662 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/shutdown.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    32000 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/submit.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1576 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/tracking_service.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4647 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/uid.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.507924 firexapp-5.3.0/firexapp/tasks/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/tasks/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3226 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/tasks/core_tasks.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6445 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/tasks/example.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3687 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/tasks/root_tasks.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.508924 firexapp-5.3.0/firexapp/testing/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4360 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/config_base.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    12807 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/config_interpreter.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1099 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/coverage_plugin.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3365 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/pydev_debug_plugin.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7451 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/test_infra.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.499925 firexapp-5.3.0/firexapp.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      435 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)     1598 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      190 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      196 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        9 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      267 2023-08-07 19:31:29.509925 firexapp-5.3.0/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1713 2023-08-07 19:31:14.000000 firexapp-5.3.0/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-07 19:31:14.000000 firexapp-5.3.0/versioneer.py
```

### Comparing `firexapp-4.9.9/LICENSE` & `firexapp-5.3.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,29 @@
-Unless otherwise noted, code on the FireXApp GitHub is licensed under the terms of the following BSD license terms:
+BSD 3-Clause License
 
+Copyright (c) 2022, FireX
+All rights reserved.
 
-Copyright (c) 2018 Cisco and/or its affiliates
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
 
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
-following conditions are met:
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
 
-1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following
-disclaimer.
-2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following
-disclaimer in the documentation and/or other materials provided with the distribution.
-3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products
-derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
-INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
-WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `firexapp-4.9.9/fastentrypoints.py` & `firexapp-5.3.0/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/application.py` & `firexapp-5.3.0/firexapp/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import os
 import signal
 import tempfile
 from argparse import ArgumentParser, RawTextHelpFormatter
+import json
+from typing import List
+import sys
 
 from firexapp.plugins import load_plugin_modules, cdl2list
 from firexapp.submit.console import setup_console_logging
 from firexkit.permissions import DEFAULT_UMASK
 
 logger = setup_console_logging(__name__)
 
+JSON_ARGS_PATH_ARG_NAME = '--json_args_path'
+
 
 def main():
     os.umask(DEFAULT_UMASK)
     # Need to call setup_console_logging like this as this module is always called from another.
     setup_console_logging("__main__")
     with tempfile.NamedTemporaryFile(delete=True) as submission_tmp_file:
         from firexapp.submit.submit import SubmitBaseApp
         submit_app = SubmitBaseApp(submission_tmp_file=submission_tmp_file.name)
         app = FireXBaseApp(submit_app=submit_app)
-        app.run()
+        ExitSignalHandler(app)
+        app.run(sys_argv=sys.argv[1:])
 
 
 def import_microservices(plugins_files=None, imports: tuple = None) -> []:
     for f in cdl2list(plugins_files):
         if not os.path.isfile(f):
             raise FileNotFoundError(f)
 
@@ -67,56 +73,90 @@
 
 def get_app_tasks(tasks, all_tasks=None):
     if type(tasks) is str:
         tasks = tasks.split(",")
     return [get_app_task(task, all_tasks) for task in tasks]
 
 
+class JsonContentNotList(Exception):
+    pass
+
+
+def get_args_from_json(json_file: str) -> List[str]:
+    with open(json_file) as fp:
+        try:
+            input_list = json.load(fp)
+        except json.decoder.JSONDecodeError:
+            logger.error(f'The json file {json_file} could not be correctly decoded.')
+            raise
+    if not isinstance(input_list, list):
+        raise JsonContentNotList('The provided json %s must contain a list of arguments')
+    return input_list
+
+
+def get_args_from_json_from_all_args(all_args: List[str]) -> List[str]:
+    if not all_args:
+        return []
+    try:
+        json_args_name_index = all_args.index(JSON_ARGS_PATH_ARG_NAME)
+    except ValueError:
+        return []
+    else:
+        try:
+            json_args_path = all_args[json_args_name_index + 1]
+        except IndexError:
+            raise Exception(f'The {JSON_ARGS_PATH_ARG_NAME} argument is not followed by a value.')
+        else:
+            return get_args_from_json(json_args_path)
+
+
 class FireXBaseApp:
     def __init__(self, submit_app=None, info_app=None):
         if not info_app:
             from firexapp.info import InfoBaseApp
             info_app = InfoBaseApp()
         self.info_app = info_app
 
         if not submit_app:
             from firexapp.submit.submit import SubmitBaseApp
             submit_app = SubmitBaseApp()
         self.submit_app = submit_app
         self.arg_parser = None
         self.running_app = None
-        self._signal_exit_handler = ExitSignalHandler(self)
         self.submit_args_to_process = None
 
     def run(self, sys_argv=None):
         if not self.arg_parser:
             self.arg_parser = self.create_arg_parser()
 
         try:
             if sys_argv is not None:
                 "".join(sys_argv).encode('ascii')
         except UnicodeEncodeError as ue:
             self.arg_parser.error(
                 'You entered a non-ascii character at the command line.\n' + str(ue))
 
-        arguments, others = self.arg_parser.parse_known_args(sys_argv)
+        args_to_process = sys_argv
+        if sys_argv is not None:
+            sys_argv += get_args_from_json_from_all_args(sys_argv)
+        arguments, others = self.arg_parser.parse_known_args(args_to_process)
 
         # run default help
         if not hasattr(arguments, "func"):
             self.arg_parser.print_help()
             self.arg_parser.exit()
         if self.submit_app.run_submit.__name__ not in arguments.func.__name__:
             if len(others):
                 # only submit supports 'other' arguments
                 msg = 'Unrecognized arguments: %s' % ' '.join(others)
                 self.arg_parser.error(message=msg)
             arguments.func(arguments)
         else:
             self.running_app = self.submit_app
-            self.submit_app.submit_args_to_process = sys_argv
+            self.submit_app.submit_args_to_process = args_to_process
             arguments.func(arguments, others)
 
     def main_error_exit_handler(self, reason=None):
         if self.running_app and hasattr(self.running_app, self.main_error_exit_handler.__name__):
             self.running_app.main_error_exit_handler(reason=reason)
         exit(-1)
```

### Comparing `firexapp-4.9.9/firexapp/broker_manager/__init__.py` & `firexapp-5.3.0/firexapp/broker_manager/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         pass
 
     @abstractmethod
     def get_url(self) -> str:
         pass
 
     @abstractmethod
-    def is_alive(self) -> bool:
+    def is_alive(self, timeout=None) -> bool:
         pass
 
     @classmethod
     def log(cls, msg, header=None, level=logging.DEBUG, exc_info=None):
         if header is None:
             header = cls.__name__
         if header:
```

### Comparing `firexapp-4.9.9/firexapp/broker_manager/broker_factory.py` & `firexapp-5.3.0/firexapp/broker_manager/broker_factory.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/broker_manager/redis_manager.py` & `firexapp-5.3.0/firexapp/broker_manager/redis_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,37 +265,37 @@
                     self.log('Redis did not come up after %d trial(s) (max_trials=%d)..Giving up!' %
                              (trials, max_trials), level=ERROR)
                     raise
                 self.log('Redis did not come up after %d trial(s) (max_trials=%d)' % (trials, max_trials), level=INFO)
             else:
                 break
 
-    def shutdown(self):
+    def shutdown(self, timeout=None):
         try:
             RedisManager.log('shutting down...')
-            self.cli('shutdown')
+            self.cli('shutdown', timeout=timeout)
         except subprocess.CalledProcessError:
             RedisManager.log('could not shutdown.')
 
     def force_kill(self):
         # noinspection PyBroadException
         try:
             RedisManager.log('force killing...')
             Process(int(Path(self.pid_file).read_text())).kill()
         except Exception:
             RedisManager.log('could not force kill.')
 
     def get_url(self) -> str:
         return self.broker_url
 
-    def is_alive(self, port=None):
+    def is_alive(self, port=None, timeout=None):
         port = self.port if port is None else port
         try:
             # including the host makes sure the current host can connect to itself via its hostname, like celery will.
-            output = self.cli('PING', port=port, include_host=True)
+            output = self.cli('PING', port=port, include_host=True, timeout=timeout)
         except subprocess.CalledProcessError:
             return False
         else:
             return output == 'PONG' or self.get_broker_failed_auth_str() in output
 
     def wait_until_active(self, timeout=60, port=None):
         port = self.port if port is None else port
@@ -316,30 +316,32 @@
         url = urlsplit(broker_url)
         return url.hostname, str(url.port) if url.port else url.port
 
     @staticmethod
     def get_password_from_url(broker_url):
         return urlsplit(broker_url).password
 
-    def get(self, key):
-        return self.cli('GET %s' % key)
+    def get(self, key, timeout=None):
+        return self.cli('GET %s' % key, timeout=timeout)
 
-    def set(self, key, value):
-        rc = self.cli('SET %s %s' % (key, value))
+    def set(self, key, value, timeout=None):
+        rc = self.cli('SET %s %s' % (key, value), timeout=timeout)
         assert rc == 'OK', 'The return value was %s' % rc
 
     def monitor(self, monitor_file):
         cmd = os.path.join(self.redis_bin_base, 'redis-cli') + ' -p %d -a %s MONITOR &' % (self.port, self._password)
         with open(monitor_file, 'w') as out:
             subprocess.check_call(cmd, shell=True, stdout=out, stderr=subprocess.STDOUT)
 
-    def cli(self, cmd, port=None, include_host=False):
+    def cli(self, cmd, port=None, include_host=False, timeout=None):
         port = self.port if port is None else port
-        null = open(os.devnull, 'w')
         cmd = self.get_redis_cli_cmd(port=port, include_host=include_host) + ' %s' % cmd
-        return subprocess.check_output(shlex.split(cmd), stderr=null).decode().strip()
+        with open(os.devnull, 'w') as null:
+            return subprocess.check_output(shlex.split(cmd),
+                                           stderr=null,
+                                           timeout=timeout).decode().strip()
 
     def __repr__(self):
         return self.broker_url
 
     def __eq__(self, other):
         return str(other) == self.broker_url
```

### Comparing `firexapp-4.9.9/firexapp/celery_manager.py` & `firexapp-5.3.0/firexapp/celery_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import re
 import subprocess
 import psutil
 from firexapp.broker_manager.broker_factory import BrokerFactory
 from socket import gethostname
 from firexapp.common import poll_until_file_not_empty, poll_until_dir_empty, find_procs
-from firexapp.plugins import PLUGGING_ENV_NAME, cdl2list
+from firexapp.plugins import PLUGINS_ENV_NAME, cdl2list
 from firexapp.fileregistry import FileRegistry
 from collections.abc import Iterable
 from firexapp.common import qualify_firex_bin
 
 logger = setup_console_logging(__name__)
 
 CELERY_LOGS_REGISTRY_KEY = 'celery_logs'
@@ -25,14 +25,15 @@
 MICROSERVICE_LOGS_REGISTRY_KEY = 'microservice_logs'
 FileRegistry().register_file(MICROSERVICE_LOGS_REGISTRY_KEY, 'microservice_logs')
 
 
 class CeleryWorkerStartFailed(Exception):
     pass
 
+
 class CeleryManager(object):
     celery_bin_name = 'celery'
 
     def __init__(self, plugins=None, logs_dir=None, worker_log_level='debug', cap_concurrency=None,
                  app='firexapp.engine', env=None, broker=None):
 
         if not broker:
@@ -70,15 +71,15 @@
     def update_env(self, env):
         assert isinstance(env, dict), 'env needs to be a dictionary'
         self.env.update({k: str(v) for k, v in env.items()})
 
     @staticmethod
     def get_plugins_env(plugins):
         plugin_files = cdl2list(plugins)
-        return {PLUGGING_ENV_NAME: ",".join(plugin_files)}
+        return {PLUGINS_ENV_NAME: ",".join(plugin_files)}
 
     @staticmethod
     def get_celery_logs_dir(logs_dir):
         return FileRegistry().get_file(CELERY_LOGS_REGISTRY_KEY, logs_dir)
 
     @staticmethod
     def get_celery_pids_dir(logs_dir):
@@ -198,40 +199,55 @@
         try:
             poll_until_file_not_empty(pid_file, timeout=timeout)
         except AssertionError:
             err_list = self.extract_errors_from_celery_logs(stdout_file)
             if err_list:
                 extra_err_info += '\nFound the following errors:\n' + '\n'.join(err_list)
 
-            raise CeleryWorkerStartFailed('The worker %s@%s did not come up after %d seconds.'
-                                          '\nPlease look into %s for details.'
-                                          '%s' % (workername,
-                                                  self.hostname,
-                                                  timeout,
-                                                  stdout_file,
-                                                  extra_err_info))
+            extra_err_info += '\nAttempting to delete the invocation pids'
+            deleted_pids = subprocess.run(['/bin/pkill', '-e', '-f', pid_file],
+                                          capture_output=True,
+                                          text=True)
+            if deleted_pids.stdout:
+                extra_err_info += f'\nstdout: {deleted_pids.stdout}'
+            if deleted_pids.stderr:
+                extra_err_info += f'\nstderr: {deleted_pids.stderr}'
+
+            raise CeleryWorkerStartFailed(f'The worker{workername}@{self.hostname} did not come up after'
+                                          f' {timeout} seconds.\n'
+                                          f'Please look into {stdout_file!r} for details.'
+                                          f'{extra_err_info}')
         pid = self.get_pid_from_file(pid_file)
         self.log('pid %d became active' % pid)
 
     def start(self, workername, queues=None, wait=True, timeout=15*60, concurrency=None, worker_log_level=None,
-              app=None, cap_concurrency=None, cwd=None, soft_time_limit=None, autoscale: tuple = None):
+              app=None, cap_concurrency=None, cwd=None, soft_time_limit=None, autoscale: tuple = None,
+              detach: bool = True):
 
         # Override defaults if applicable
         worker_log_level = worker_log_level if worker_log_level else self.worker_log_level
         app = app if app else self.app
         cap_concurrency = cap_concurrency if cap_concurrency else self.cap_concurrency
 
         stdout_file = self._get_stdout_file(workername)
         log_file = self._get_worker_log_file(workername)
         pid_file = self._get_pid_file(workername)
         self.pid_files[workername] = pid_file
 
-        cmd = '%s --app=%s worker --hostname=%s@%%h --loglevel=%s ' \
-              '--logfile=%s --pidfile=%s --events --without-gossip --without-heartbeat --without-mingle -Ofair' % \
-              (self.celery_bin, app, workername, worker_log_level, log_file, pid_file)
+        cmd = f'{self.celery_bin} ' \
+              f'--app={app} worker ' \
+              f'--hostname={workername}@%h ' \
+              f'--loglevel={worker_log_level} ' \
+              f'--logfile={log_file} ' \
+              f'--pidfile={pid_file} ' \
+              f'--events ' \
+              f'--without-gossip ' \
+              f'--without-heartbeat ' \
+              f'--without-mingle ' \
+              f'-Ofair'
         if queues:
             cmd += ' --queues=%s' % queues
 
         if concurrency and autoscale:
             raise AssertionError('You can either provide a value of concurrency or autoscale, but not both')
 
         if concurrency:
@@ -251,27 +267,28 @@
         # piping to ts is helpful for debugging if available
         try:
             subprocess.check_call(["which", "ts"], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL)
         except subprocess.CalledProcessError:
             pass
         else:
             cmd += " | ts '[%Y-%m-%d %H:%M:%S]'"
-        cmd += ' &'
+        if detach:
+            cmd += ' &'
 
         self.log('Starting %s on %s...' % (workername, self.hostname))
         self.log(cmd)
 
         if cwd:
             self.log('cwd=%s' % cwd)
 
         with open(stdout_file, 'ab') as fp:
             subprocess.check_call(cmd, shell=True, stdout=fp, stderr=subprocess.STDOUT, env=self.env,
                                   cwd=cwd)
 
-        if wait:
+        if detach and wait:
             self.wait_until_active(pid_file=pid_file, timeout=timeout, stdout_file=stdout_file, workername=workername)
 
     @staticmethod
     def find_procs(pid_file):
         return find_procs('celery', cmdline_contains='--pidfile=%s' % pid_file)
 
     def find_all_procs(self):
```

### Comparing `firexapp-4.9.9/firexapp/common.py` & `firexapp-5.3.0/firexapp/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,53 +145,58 @@
 
 
 def render_template(template_str, template_args):
     return Template(template_str).render(**template_args)
 
 
 #
-# Create a symlink from src -> target.
+# Create a symlink to src, named target.
 #
-# delete_link == True: Delete target link first if it exists.
+# delete_link == True: Delete target link if it exists.
 #             == False: Don't delete target link if it exists.
 #             == None (default): If symlink creation fails because the link
 #                                exists, delete it and try again.
 #                                (optimized for cases where we don't expect
 #                                the link to exist in most cases.)
 #
 def create_link(src, target, delete_link=None, relative=False):
     done = False
     attempts = 0
 
     if relative:
         src = os.path.relpath(src, os.path.dirname(target))
 
-    while not done:
-        if delete_link is True:
-            try:
-                os.remove(target)
-            except Exception:
-                pass
-        attempts += 1
+    if not delete_link:
         try:
             os.symlink(src, target)
-            done = True
             logger.debug('Symbolic link created: %s -> %s' % (src, target))
-        except FileExistsError as e:
+            return  # <-- Done!
+        except FileExistsError:
             if delete_link is False:
                 raise
-            if attempts > 1:
-                # Maybe we're competing with someone else
-                # to create that link...
-                logger.debug('Symbolic link failed: %s -> %s' % (src, target))
-                logger.warning(e)
-                done = True
-            else:
-                # Remove target and try again
-                delete_link = True
+
+    # If we want to delete the link, we do a link-replace in an atomic manner
+    temp_target = target + f'.{os.getpid()}.tmp'
+    try:
+        # Avoid errors with possibly stale links
+        os.remove(temp_target)
+    except FileNotFoundError:
+        pass
+
+    try:
+        os.symlink(src, temp_target)
+        os.rename(temp_target, target)
+        logger.debug('Symbolic link created: %s -> %s' % (src, target))
+    except Exception:
+        try:
+            os.remove(temp_target)
+        except FileNotFoundError:
+            pass
+
+        raise
 
 
 def dict2str(mydict, sort=False, sep='    ', usevrepr=True, line_prefix=''):
     if not mydict:
         return 'None'
 
     txt = ''
```

### Comparing `firexapp-4.9.9/firexapp/discovery.py` & `firexapp-5.3.0/firexapp/discovery.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/engine/celery.py` & `firexapp-5.3.0/firexapp/engine/celery.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/engine/logging.py` & `firexapp-5.3.0/firexapp/engine/logging.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+import re
+import uuid
 
 import celery.utils.log
 from _socket import gethostname
 from logging.handlers import WatchedFileHandler
 import html
 from celery.signals import after_setup_task_logger, after_setup_logger
 import os
@@ -78,16 +80,46 @@
 
         # Add a label element if it exists
         try:
             record.label_element = f"<a name='{record.label}'></a>"
         except AttributeError:
             record.label_element = ''
 
+        # Add formatting to arguments in span class 'task_started'
+        if 'task_started' in span_classes or 'task_completed' in span_classes:
+            # Use label as unique identifier, if available
+            try:
+                label = record.label
+            except AttributeError:
+                label = uuid.uuid4()
+
+            # decorate multiline arguments
+            def decorate_argument(match):
+                arg_num = match.group(1)
+                lines = match.group(2).split('\n')
+                if len(lines) > 1:
+                    lines[0] = f"<div class='wrap-collapsible'><input id='col{label}-{arg_num}' name='collapsible' " \
+                               f"class='toggle' type='checkbox'/><label for='col{label}-{arg_num}' class='lbl-toggle'>" \
+                               f"</label><span>  {arg_num}. {html_escape(lines[0])}</span><div class='collapsible-content'>"
+                    for index in range(1, len(lines)):
+                        lines[index] = f"<span>{html_escape(lines[index])}</span>"
+                    lines[-1] += "</div></div>"
+                else:
+                    lines[0] = f"<span class='non-collapsing'>  {arg_num}. {html_escape(lines[0])}</span>"
+                return '\n'.join(lines)
+
+            record.msg = re.sub(r'  (\d+)\. (.+?)(?=\n  \d+\.|\n=+|\n\*+)',
+                                decorate_argument,
+                                record.msg, flags=re.DOTALL | re.MULTILINE)
+
+            record.html_escape = False
+
         return True
 
+
 class FireXFormatter(celery.utils.log.ColorFormatter):
     def __init__(self, fmt):
         new_fmt = '%(span_class_element)s%(label_element)s' + fmt + '</span>'
         super().__init__(fmt=new_fmt, use_color=False)
         self.datefmt = '%m-%d %H:%M:%S %z'
 
     def format(self, record):
```

### Comparing `firexapp-4.9.9/firexapp/events/broker_event_consumer.py` & `firexapp-5.3.0/firexapp/events/broker_event_consumer.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import abc
 import logging
 from pathlib import Path
 import threading
 import traceback
 import time
+from typing import Optional
 
 from celery.app.base import Celery
 from celery.events import EventReceiver
 
 
 logger = logging.getLogger(__name__)
 
@@ -22,14 +23,17 @@
     __metaclass__ = abc.ABCMeta
 
     def __init__(self, celery_app: Celery, max_retry_attempts: int = None, receiver_ready_file: str = None):
         threading.Thread.__init__(self)
         self.celery_app = celery_app
         self.max_try_interval = 2**max_retry_attempts if max_retry_attempts is not None else 32
         self.ready = False
+        self.celery_event_receiver : Optional[EventReceiver] = None
+
+        self.receiver_ready_file : Optional[Path]
 
         if receiver_ready_file:
             self.receiver_ready_file = Path(receiver_ready_file)
             assert not self.receiver_ready_file.exists(), \
                 "Receiver ready file must not already exist: %s." % self.receiver_ready_file
         else:
             self.receiver_ready_file = None
@@ -54,20 +58,22 @@
     def _capture_events(self):
         try_interval = 1
         while not self._is_root_complete():
             try:
                 try_interval *= 2
                 with self.celery_app.connection() as conn:
                     conn.ensure_connection(max_retries=1, interval_start=0)
-                    recv = EventReceiver(conn,
-                                         handlers={"*": self._on_event},
-                                         app=self.celery_app)
+                    self.celery_event_receiver = EventReceiver(
+                        conn,
+                        handlers={"*": self._on_event},
+                        app=self.celery_app)
                     try_interval = 1
                     self._ready()
-                    recv.capture(limit=None, timeout=None, wakeup=True)
+                    self.celery_event_receiver.capture(
+                        limit=None, timeout=None, wakeup=True)
             except (KeyboardInterrupt, SystemExit):
                 logger.exception("Received external shutdown.")
                 self._on_external_shutdown()
             # pylint: disable=C0321
             except Exception:
                 if self._is_root_complete():
                     logger.info("Root task complete; stopping broker receiver thread.")
@@ -75,31 +81,46 @@
                 logger.error(traceback.format_exc())
                 if try_interval > self.max_try_interval:
                     logger.warning("Maximum broker retry attempts exceeded, stopping receiver thread)."
                                    " Will no longer retry despite incomplete root task.")
                     return
                 logger.debug("Try interval %d secs, still worth retrying." % try_interval)
                 time.sleep(try_interval)
+            else:
+                logger.debug("Celery receiver stopped")
 
     def _on_ready(self):
         """Called a single time when the thread is ready to start receiving events."""
         pass
 
     def _on_event(self, event):
         try:
             self._on_celery_event(event)
+
+            if (self._is_root_complete()
+                # In case checking all tests is expensive, check root first. Remaining
+                # tasks only need to be checked once root is complete since everything
+                # can't be complete if the root is not complete.
+                and self._all_tasks_complete()
+                and self.celery_event_receiver):
+                logger.info(f"Stopping Celery event receiver because all tasks are complete.")
+                self.celery_event_receiver.should_stop = True
         except Exception as e:
             logger.exception(e)
             raise
 
     @abc.abstractmethod
     def _is_root_complete(self):
         """Return True only when the root task is complete and normal shutdown can occur."""
         pass
 
+    def _all_tasks_complete(self):
+        """Return True only when all tasks are complete and the event receiver can be stopped."""
+        return False
+
     @abc.abstractmethod
     def _on_celery_event(self, event):
         """Callback invoked when a event is received from Celery."""
         pass
 
     def _on_external_shutdown(self):
         """Callback invoked when the thread is shutdown externally (e.g. signal)"""
```

### Comparing `firexapp-4.9.9/firexapp/events/event_aggregator.py` & `firexapp-5.3.0/firexapp/events/event_aggregator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Aggregates events in to the task data model.
 """
 from collections import namedtuple
 from datetime import datetime
 import logging
+from typing import Optional, Any
 
 from firexkit.task import FIREX_REVOKE_COMPLETE_EVENT_TYPE
 
 from firexapp.events.model import ALL_RUNSTATES, INCOMPLETE_RUNSTATES, COMPLETE_RUNSTATES, TaskColumn
 
 logger = logging.getLogger(__name__)
 
@@ -95,20 +96,26 @@
 }
 
 
 def _get_keys_with_true(input_dict, key):
     return [k for k, v in input_dict.items() if v.get(key, False)]
 
 
-DEFAULT_AGGREGATOR_CONFIG = EventAggregatorConfig(
-    copy_fields=_get_keys_with_true(FIELD_CONFIG, 'copy_celery'),
-    merge_fields=_get_keys_with_true(FIELD_CONFIG, 'aggregate_merge'),
-    keep_initial_fields=_get_keys_with_true(FIELD_CONFIG, 'aggregate_keep_initial'),
-    field_to_celery_transforms={k: v['transform_celery'] for k, v in FIELD_CONFIG.items() if 'transform_celery' in v},
-)
+def event_aggregator_from_field_spec(field_spec: dict[str, dict[str, Any]]):
+    return EventAggregatorConfig(
+        copy_fields=_get_keys_with_true(field_spec, 'copy_celery'),
+        merge_fields=_get_keys_with_true(field_spec, 'aggregate_merge'),
+        keep_initial_fields=_get_keys_with_true(field_spec, 'aggregate_keep_initial'),
+        field_to_celery_transforms={
+            k: v['transform_celery']
+            for k, v in field_spec.items()
+            if 'transform_celery' in v},
+    )
+
+DEFAULT_AGGREGATOR_CONFIG = event_aggregator_from_field_spec(FIELD_CONFIG)
 
 
 def _deep_merge_keys(dict1, dict2, keys):
     dict1_to_merge = {k: v for k, v in dict1.items() if k in keys}
     dict2_to_merge = {k: v for k, v in dict2.items() if k in keys}
     return _deep_merge(dict1_to_merge, dict2_to_merge)
 
@@ -180,19 +187,18 @@
     for merged_data_key, merged_data_val in merged_values.items():
         if merged_data_key not in task or task[merged_data_key] != merged_data_val:
             changed_data[merged_data_key] = merged_data_val
 
     return changed_data
 
 
-class FireXEventAggregator:
+class AbstractFireXEventAggregator:
     """ Aggregates many events in to the task data model. """
 
-    def __init__(self, aggregator_config: EventAggregatorConfig = DEFAULT_AGGREGATOR_CONFIG):
-        self.tasks_by_uuid = {}
+    def __init__(self, aggregator_config: EventAggregatorConfig):
         self.new_task_num = 1
         self.root_uuid = None
         self.aggregator_config = aggregator_config
 
     def aggregate_events(self, events):
         new_data_by_task_uuid = {}
         for e in events:
@@ -206,45 +212,71 @@
     def generate_incomplete_events(self):
         """
         Unfortunately, if a run terminates ungracefully, incomplete tasks will never arrive at a
         terminal runstate. The 'task-incomplete' runstate is a fake (non-backend) terminal runstate
         that is generated here so that the UI can show a non-incomplete runstate.
         :return:
         """
-        return [{'uuid': task['uuid'], 'type': 'task-incomplete', 'timestamp': datetime.now().timestamp()}
-                for task in self.tasks_by_uuid.values()
-                if task['state'] in INCOMPLETE_RUNSTATES]
+        new_events = []
+        now = datetime.now().timestamp()
+        for incomplete_task in self._get_incomplete_tasks():
+            if incomplete_task.get('state') in INCOMPLETE_RUNSTATES:
+                event_type = 'task-incomplete'
+            else:
+                event_type = 'task-completed'
+
+            new_event = {
+                'uuid': incomplete_task['uuid'],
+                'type': event_type,
+            }
 
-    def is_root_complete(self):
-        if not self.root_uuid or self.root_uuid not in self.tasks_by_uuid:
+            if not incomplete_task.get(TaskColumn.ACTUAL_RUNTIME.value):
+                task_runtime = now - incomplete_task.get('first_started', now)
+                new_event[TaskColumn.ACTUAL_RUNTIME.value] = task_runtime
+
+            new_events.append(new_event)
+        return new_events
+
+    def is_root_complete(self) -> bool:
+        if (
+            not self.root_uuid
+            or not self._task_exists(self.root_uuid)
+        ):
             return False  # Might not have root event yet.
-        root_runstate = self.tasks_by_uuid[self.root_uuid].get('state', None)
+        root_runstate = self._get_task(self.root_uuid).get('state', None)
         return root_runstate in COMPLETE_RUNSTATES
 
+    def are_all_tasks_complete(self) -> bool:
+        if not self.is_root_complete():
+            # optimization: don't query all incomplete tasks if the root isn't done yet.
+            return False
+        return len(self._get_incomplete_tasks()) == 0
+
     def _get_or_create_task(self, task_uuid):
-        if task_uuid not in self.tasks_by_uuid:
+        if not self._task_exists(task_uuid):
             task = {
                 'uuid': task_uuid,
                 'task_num': self.new_task_num,
             }
             self.new_task_num += 1
-            self.tasks_by_uuid[task_uuid] = task
+            self._insert_new_task(task)
             is_new = True
         else:
-            task = self.tasks_by_uuid[task_uuid]
+            task = self._get_task(task_uuid)
             is_new = False
         return task, is_new
 
     def _aggregate_event(self, event):
         if ('uuid' not in event
                 # The uuid can be null, it's unclear what this means but it can't be associated with a task.
                 or not event['uuid']
                 # Revoked events can be sent before any other, and we'll never get any data (name, etc) for that task.
                 # Therefore ignore events that are for a new UUID that have revoked type.
-                or (event['uuid'] not in self.tasks_by_uuid and event.get('type', '') == REVOKED_EVENT_TYPE)):
+                or (not self._task_exists(event['uuid'])
+                    and event.get('type', '') == REVOKED_EVENT_TYPE)):
             return {}
 
         if event.get(TaskColumn.PARENT_ID.value, '__no_match') is None and self.root_uuid is None:
             self.root_uuid = event['uuid']
 
         new_data_by_task_uuid = get_new_event_data(event,
                                                    self.aggregator_config.copy_fields,
@@ -260,7 +292,48 @@
             task.update(changed_data)
 
             # If we just created the task, we need to send the auto-initialized fields, as well as data from the event.
             # If this isn't a new event, we only need to send what has changed.
             changes_by_task_uuid[task_uuid] = dict(task) if is_new_task else dict(changed_data)
 
         return changes_by_task_uuid
+
+    def _task_exists(self, task_uuid):
+        raise NotImplementedError("This should be implemented by concrete subclasses")
+
+    def _get_task(self, task_uuid: str) -> Optional[dict[str, Any]]:
+        raise NotImplementedError("This should be implemented by concrete subclasses")
+
+    def _get_incomplete_tasks(self) -> list[dict[str, Any]]:
+        raise NotImplementedError("This should be implemented by concrete subclasses")
+
+    def _insert_new_task(self, task: dict[str, Any]) -> None:
+        raise NotImplementedError("This should be implemented by concrete subclasses")
+
+
+class FireXEventAggregator(AbstractFireXEventAggregator):
+    """ Aggregates many Celery events in to the FireX tasks data model. """
+
+    def __init__(self, aggregator_config: EventAggregatorConfig = DEFAULT_AGGREGATOR_CONFIG):
+        super().__init__(aggregator_config)
+        self.tasks_by_uuid : dict[str, Any] = {}
+
+    def _task_exists(self, task_uuid: str) -> bool:
+        if not task_uuid:
+            return False
+        return task_uuid in self.tasks_by_uuid
+
+    def _get_task(self, task_uuid: str) -> Optional[dict[str, Any]]:
+        return self.tasks_by_uuid.get(task_uuid)
+
+    def _get_incomplete_tasks(self) -> list[dict[str, Any]]:
+        return [
+            task for task in self.tasks_by_uuid.values()
+            if task.get(TaskColumn.ACTUAL_RUNTIME.value) is None
+                or task.get('state') in INCOMPLETE_RUNSTATES
+        ]
+
+    def _insert_new_task(self, task: dict[str, Any]) -> None:
+        assert 'uuid' in task, f'Cannot insert task without uuid: {task}'
+        assert not self._task_exists(task['uuid']), f'Task already exists, cannot insert: {task}'
+        self.tasks_by_uuid[task['uuid']] = task
+
```

### Comparing `firexapp-4.9.9/firexapp/events/model.py` & `firexapp-5.3.0/firexapp/events/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,23 @@
 
 ALL_RUNSTATES = {
     RunStates.RECEIVED.value: {'terminal': False},
     RunStates.STARTED.value: {'terminal': False},
     RunStates.BLOCKED.value: {'terminal': False},
     RunStates.UNBLOCKED.value: {'terminal': False},
     RunStates.SUCCEEDED.value: {'terminal': True},
+
+    # There are gotchas here, failed isn't "really" terminal
+    # in the presence of retries.
     RunStates.FAILED.value: {'terminal': True},
     RunStates.REVOKED.value: {'terminal': True},
     RunStates.INCOMPLETE.value: {'terminal': True},  # server-side kludge state to fix tasks that will never complete.
 }
-COMPLETE_RUNSTATES = [s for s, v in ALL_RUNSTATES.items() if v['terminal']]
-INCOMPLETE_RUNSTATES = [s for s, v in ALL_RUNSTATES.items() if not v['terminal']]
+COMPLETE_RUNSTATES = {s for s, v in ALL_RUNSTATES.items() if v['terminal']}
+INCOMPLETE_RUNSTATES = {s for s, v in ALL_RUNSTATES.items() if not v['terminal']}
 
 
 class RunMetadataColumn(Enum):
     FIREX_ID = "firex_id"
     LOGS_DIR = "logs_dir"
     CHAIN = "chain"
     ROOT_UUID = "root_uuid"
```

### Comparing `firexapp-4.9.9/firexapp/fileregistry.py` & `firexapp-5.3.0/firexapp/fileregistry.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/firex_subprocess.py` & `firexapp-5.3.0/firexapp/firex_subprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from socket import gethostname
 import stat
 import subprocess
 import tempfile
 import time
 import urllib.parse
 import uuid
+from typing import Union
 
 from celery.utils.log import get_task_logger
 
 from firexkit import firex_exceptions, firexkit_common
 from firexapp.engine.logging import html_escape
 from firexapp.events.model import EXTERNAL_COMMANDS_KEY
 
-
 logger = get_task_logger(__name__)
 
 
 class CommandFailed(firex_exceptions.FireXCalledProcessError):
     pass
 
 
@@ -57,20 +57,20 @@
 
 def run(cmd, retries=0, retry_delay=3, **kwargs):
     # Note that this differs from Python 3.8's API since capture_output is True by default in _subprocess_runner
 
     runner_type = _SubprocessRunnerType.RUN
 
     _sanitize_runner_kwargs(runner_type=runner_type, kwargs=kwargs)
-    return _subprocess_runner_retries(runner_type=runner_type, # Pass through 'capture_output' and 'check'
+    return _subprocess_runner_retries(runner_type=runner_type,  # Pass through 'capture_output' and 'check'
                                       retries=retries, retry_delay=retry_delay, cmd=cmd, **kwargs)
 
 
 def _sanitize_runner_kwargs(runner_type: _SubprocessRunnerType, kwargs: dict):
-    disallowed_keys = ['stderr', 'stdout', 'universal_newlines']
+    disallowed_keys = ['stdout', 'universal_newlines']
     if runner_type is _SubprocessRunnerType.RUN:
         disallowed_keys.extend(['input'])
     else:
         disallowed_keys.extend(['capture_output', 'check'])
 
     for key in disallowed_keys:
         if key in kwargs:
@@ -102,41 +102,44 @@
         from celery import current_task
         if current_task:
             current_task.send_firex_event_raw({EXTERNAL_COMMANDS_KEY: subprocess_data})
     except Exception as e:
         logger.warning(f"Error while sending flame subprocess event: {e}")
 
 
-def _send_flame_subprocess_start(flame_subprocess_id, cmd, filename, cwd):
-    _send_flame_subprocess({flame_subprocess_id:
-                                {'cmd': cmd,
-                                 'cwd': str(cwd) if cwd else cwd,
-                                 'output_file': filename,
-                                 'host': gethostname(),
-                                 'start_time': time.time()}})
+def _send_flame_subprocess_start(flame_subprocess_id, cmd, cwd, host, filename=None, remote_host=None):
+    _send_flame_subprocess({flame_subprocess_id: {'cmd': cmd,
+                                                  'cwd': str(cwd) if cwd else cwd,
+                                                  'output_file': filename,
+                                                  'host': host,
+                                                  'remote_host': remote_host,
+                                                  'start_time': time.time()}})
 
 
-def _send_flame_subprocess_end(flame_subprocess_id, hung_process, slow_process, output, chars, returncode):
+def _send_flame_subprocess_end(flame_subprocess_id, output, returncode, chars=None, hung_process=None,
+                               slow_process=None, stderr_output=None):
     ui_max_chars = 8000
     chars = ui_max_chars if chars is None else min(chars, ui_max_chars)
     subproc_result = {
         'completed': not hung_process and not slow_process and returncode is not None,
         'timeout': slow_process,
         'inactive': hung_process,
         'output_truncated': len(output) >= chars if output is not None else False,
         'output': output[-chars:] if output else output,
+        'stderr_output_truncated': len(stderr_output) >= chars if stderr_output is not None else False,
+        'stderr_output': stderr_output[-chars:] if stderr_output else stderr_output,
         'returncode': returncode,
     }
     _send_flame_subprocess({flame_subprocess_id: {'result': subproc_result, 'end_time': time.time()}})
 
 
-def _subprocess_runner(cmd, runner_type: _SubprocessRunnerType = _SubprocessRunnerType.CHECK_OUTPUT,
+def _subprocess_runner(cmd: Union[str, list], runner_type: _SubprocessRunnerType = _SubprocessRunnerType.CHECK_OUTPUT,
                        extra_header=None, file=None, chars=32000, timeout=None, capture_output=True, check=False,
                        inactivity_timeout=30 * 60, log_level=logging.DEBUG, copy_file_path=None, shell=False, cwd=None,
-                       env=None, remove_firex_pythonpath=True, logger=logger, **kwargs):
+                       env=None, remove_firex_pythonpath=True, logger=logger, stderr=subprocess.STDOUT, **kwargs):
     ##########################
     # Local Helper functions #
     ##########################
     def _get_cmd_str():
         if isinstance(cmd, list):
             return ' '.join([shlex.quote(token) for token in cmd])
         else:
@@ -231,25 +234,30 @@
             log_msg = '%s Returned String:\n%s' % (log_header, contents)
         else:
             log_msg = '%s Last %d chars of Returned String:\n%s' % (log_header, chars, contents[-chars:])
         logger.log(log_level, log_msg.encode(encoding='ascii', errors='namereplace').decode(errors='ignore'),
                    extra={'span_class': 'command_output command_output_error' if error else 'command_output'})
 
     def _kill_proc_gently(proc):
-        proc.terminate()
         try:
-            proc.wait(timeout=60)
-        except subprocess.TimeoutExpired:
-            # Okay, kill not so gently
-            proc.kill()
+            proc.terminate()
             try:
-                proc.wait(timeout=6)
+                proc.wait(timeout=60)
             except subprocess.TimeoutExpired:
-                # Give up at this point. It is undead.
-                pass
+                # Okay, kill not so gently
+                proc.kill()
+                try:
+                    proc.wait(timeout=6)
+                except subprocess.TimeoutExpired as e:
+                    # Give up at this point. It is undead.
+                    logger.exception(e)
+                    pass
+
+        except PermissionError as e:  # Possible if the underlying process is running under sudo or the like
+            logger.exception(e)
 
     #################
     # Start of code #
     #################
     log_header = f'[{runner_type.name.lower()}]'
     log_header += extra_header if extra_header else ''
     cmd_str = _get_cmd_str()
@@ -266,23 +274,24 @@
         f = open(file, 'wb+')
     else:
         f = tempfile.NamedTemporaryFile(delete=False)
     filename = f.name
     open_og_rw_permissions(filename)
 
     if log_level is not None:
-        _send_flame_subprocess_start(flame_subprocess_id=subprocess_id, cmd=cmd, filename=filename, cwd=cwd_str)
+        _send_flame_subprocess_start(flame_subprocess_id=subprocess_id, cmd=cmd, filename=filename, cwd=cwd_str,
+                                     host=host)
         _log_intro_msg(subprocess_id)
 
     slow_process = hung_process = False
     with f:
         p = output = None
         try:
             # Run the command
-            p = subprocess.Popen(cmd, stdin=subprocess.PIPE, stdout=f, stderr=subprocess.STDOUT, shell=shell, cwd=cwd,
+            p = subprocess.Popen(cmd, stdin=subprocess.PIPE, stdout=f, stderr=stderr, shell=shell, cwd=cwd,
                                  env=env, **kwargs)
             start_time = time.monotonic()
 
             last_output_size = 0
             last_log_time = last_output_time = start_time
             last_output_clock_time = time.time()
             _sleep = 0.05
@@ -290,37 +299,39 @@
             while True:
                 try:
                     p.wait(_sleep)
                     # If we get here, process is done
                     break
                 except subprocess.TimeoutExpired:
                     pass
-                _sleep = _sleep * 1.1 if _sleep*1.1 < 1 else 1  # Exponential backoff
+                _sleep = _sleep * 1.1 if _sleep * 1.1 < 1 else 1  # Exponential backoff
 
                 now = time.monotonic()
                 if now - last_log_time > 10 * 60:  # Log every 10 minutes
                     time_str = datetime.datetime.fromtimestamp(last_output_clock_time).strftime('%Y-%m-%d %H:%M:%S')
                     logger.info(f'Waiting for command to finish...\n(Last command output was at {time_str}. '
                                 f'Total output size is {last_output_size} bytes.)')
                     last_log_time = now
 
                 if timeout and now - start_time > timeout:
                     # Process too slow. Kill it.
+                    logger.debug(f'Total timeout {timeout} exceeded, killing pid {p.pid}')
                     _kill_proc_gently(p)
                     slow_process = True
                     break
 
                 current_output_size = os.fstat(f.fileno()).st_size
                 if last_output_size != current_output_size:
                     # We have some activity!
                     last_output_size = current_output_size
                     last_output_time = now
                     last_output_clock_time = time.time()
                 elif inactivity_timeout and now - last_output_time > inactivity_timeout:
                     # Process hung. Kill it.
+                    logger.debug(f'Activity (writing to stdout/stderr) timeout {inactivity_timeout} exceeded, killing pid {p.pid}')
                     _kill_proc_gently(p)
                     hung_process = True
                     break
 
             if capture_output:
                 output = _get_output_from_file()
                 if log_level is not None:
@@ -330,16 +341,17 @@
             if slow_process:
                 raise subprocess.TimeoutExpired(cmd, timeout, output=output, stderr=output)
             elif hung_process:
                 raise firex_exceptions.FireXInactivityTimeoutExpired(cmd, inactivity_timeout, output=output,
                                                                      stderr=output)
         finally:
             if log_level is not None:
-                _send_flame_subprocess_end(subprocess_id, hung_process, slow_process, output, chars,
-                                           getattr(p, 'returncode', None))
+                _send_flame_subprocess_end(flame_subprocess_id=subprocess_id, hung_process=hung_process,
+                                           slow_process=slow_process, output=output, chars=chars,
+                                           returncode=getattr(p, 'returncode', None))
                 _hide_live_file_monitor_element()
 
             if p and p.stdin:
                 p.stdin.close()
 
             # Copy output file
             if (copy_file_path is not None and
```

### Comparing `firexapp-4.9.9/firexapp/info.py` & `firexapp-5.3.0/firexapp/info.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/plugins.py` & `firexapp-5.3.0/firexapp/plugins.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 import os
 import sys
 import inspect
+import traceback
 from argparse import ArgumentParser, Action
 
 from celery.signals import worker_init
 from celery.utils.log import get_task_logger
 from firexapp.common import delimit2list
 from firexkit.task import REPLACEMENT_TASK_NAME_POSTFIX
+import importlib.util
+from celery import current_app
 
 logger = get_task_logger(__name__)
-PLUGGING_ENV_NAME = "firex_external"
+PLUGINS_ENV_NAME = "firex_plugins"
+
+
+class PluginLoadError(Exception):
+    pass
 
 
 def get_short_name(long_name: str) -> str:
     return long_name.split('.')[-1]
 
 
 def find_plugin_file(file_path):
     # is it a full path?
     if os.path.isabs(file_path):
-        return file_path
-
-    # is it relative to the cwd?
-    in_cwd = os.path.abspath(file_path)
-    if os.path.isfile(in_cwd):
-        return in_cwd
+        plugin_file = file_path
+    else:
+        # Maybe it's relative?
+        plugin_file = os.path.abspath(file_path)
+    if os.path.isfile(plugin_file):
+        return plugin_file
     raise FileNotFoundError(file_path)
 
 
-def cdl2list(external_files):
-    if not external_files:
+def cdl2list(plugin_files):
+    if not plugin_files:
         return []
 
-    external_modules = [file.strip() for file in external_files.split(",")]
-    external_modules = [find_plugin_file(file) for file in external_modules if file]
-    return external_modules
+    if not isinstance(plugin_files, list):
+        plugin_files = [file.strip() for file in plugin_files.split(",")]
+
+    plugin_files = [find_plugin_file(file) for file in plugin_files if file]
+    return plugin_files
+
 
+def get_plugin_module_name(plugin_file):
+    return os.path.splitext(os.path.basename(plugin_file))[0]
 
-def get_plugin_modules(external_files):
-    external_modules = cdl2list(external_files)
-    if not external_modules:
+
+def get_plugin_module_names(plugin_files):
+    files = cdl2list(plugin_files)
+    if not files:
         return []
+    return [get_plugin_module_name(file) for file in files]
 
-    modules = []
-    py_paths_to_add = []
-    for file_path in external_modules:
-        module_directory = os.path.dirname(os.path.abspath(file_path))
-        py_paths_to_add.append(module_directory)  # allow dups. They can be removed later
-        module_name = os.path.splitext(os.path.basename(file_path))[0]
-        modules.append(module_name)
-
-    # the last external takes precedence, so append those python paths first
-    for p in reversed(py_paths_to_add):
-        if p not in sys.path:
-            sys.path.append(p)
 
-    return modules
+def get_plugin_module_names_from_env():
+    plugin_files = get_active_plugins()
+    return get_plugin_module_names(plugin_files)
 
 
 # noinspection PyUnusedLocal
 @worker_init.connect()
 def _worker_init_signal(*args, **kwargs):
-    _unregister_duplicate_tasks()
-    _mark_plugin_module_tasks()
-
-
-def _mark_plugin_module_tasks():
-    from celery import current_app
-    ext_mods = get_plugin_module_list()
-    for ext_mod in ext_mods:
-        ext_mod_tasks = [t for t in current_app.tasks if t.startswith(ext_mod)]
-        for ext_mod_task in ext_mod_tasks:
-            current_app.tasks[ext_mod_task].from_plugin = True
+    try:
+        load_plugin_modules_from_env()
+    except PluginLoadError:
+        traceback.print_exc()
+        # We will just exit, the pid file won't be written,
+        # and the bringup of the worker will eventually timeout
+        exit(-2)
 
 
 # there is no way of copying the signals without coupling with the internals of celery signals
 # noinspection PyProtectedMember
 def _get_signals_with_connections():
     from celery.utils.dispatch.signal import Signal, NONE_ID
     import celery.signals as sigs
@@ -109,17 +109,17 @@
                                                        "soft_time_limit",
                                                        "time_limit",
                                                        "track_started",
                                                        "trail",
                                                        "typing",
                                                        "returns",
                                                        "flame",
-                                                       "pending_child_strategy"] if key in dir(original)}
-
-    from celery import current_app
+                                                       "use_cache",
+                                                       "pending_child_strategy",
+                                                       "from_plugin"] if key in dir(original)}
     new_task = current_app.task(name=new_name,
                                 bind=bound,
                                 base=inspect.getmro(original.__class__)[1],
                                 check_name_for_override_posfix=False,
                                 **options)(fun=func)
     if hasattr(original, "orig"):
         new_task.orig = original.orig
@@ -142,16 +142,15 @@
     except Exception as e:
         logger.error("Unable to copy signals while overriding %s:\n%s" % (original.name, str(e)))
     return new_task
 
 
 def _unregister_duplicate_tasks():
     sigs = _get_signals_with_connections()
-    from celery import current_app
-    becomes = identify_duplicate_tasks(current_app.tasks, get_plugin_module_list())
+    becomes = identify_duplicate_tasks(current_app.tasks, get_plugin_module_names_from_env())
     for substitutions in becomes:
         prime_overrider = substitutions[-1]  # the last item in the list is the last override
         for index in range(0, len(substitutions)-1):
             original_name = substitutions[index]
             original = current_app.tasks[original_name]
             current_app.tasks[original_name] = current_app.tasks[prime_overrider]
 
@@ -176,59 +175,89 @@
             return priority_modules.index(os.path.splitext(micro_name)[0])
         except ValueError:
             return -1
     overrides = [sorted(long_names, key=priority_index) for long_names in unique_names.values() if len(long_names) > 1]
     return overrides
 
 
-def get_plugin_module_list(external_files=None):
-    if external_files is None:
-        external_files = get_active_plugins()
+def import_plugin_file(plugin_file):
 
-    external_modules = get_plugin_modules(external_files)
-    return external_modules
+    def _import_plugin(module_name, plugin_file):
+        spec = importlib.util.spec_from_file_location(module_name, plugin_file)
+        module = importlib.util.module_from_spec(spec)
+        module_directory = os.path.dirname(os.path.abspath(plugin_file))
+        if module_directory not in sys.path:
+            sys.path.append(module_directory)
+        mod = sys.modules[module_name] = module
+        try:
+            spec.loader.exec_module(module)
+        except BaseException:
+            raise PluginLoadError(f'Fatal Error loading plugin {plugin_file!r}')
+        print(f"Plugins module {module_name!r} imported from {plugin_file!r}")
+        return mod
 
+    plugin_file = find_plugin_file(plugin_file)
+    module_name = get_plugin_module_name(plugin_file)
 
-def load_plugin_modules(external_files=None):
-    if external_files is None:
-        external_files = get_active_plugins()
+    if module_name in sys.modules:
+        module_source = sys.modules[module_name].__file__
+        if module_source != plugin_file:
+            logger.error(f'Plugin module {module_name!r} was NOT imported from {plugin_file!r}. '
+                         f'A module with the same name was already imported from {module_source!r}')
+        else:
+            logger.warning(f'Plugin module {module_name!r} was already imported from {module_source!r}.')
     else:
-        set_plugins_env(external_files)
+        return _import_plugin(module_name, plugin_file)
 
-    external_modules = get_plugin_modules(external_files)
-    if not external_modules:
-        return
 
-    external_files = cdl2list(external_files)
-    for module_name in external_modules:
-        import_plugin_module(module_name=module_name, external_files=external_files)
-    _unregister_duplicate_tasks()
+def import_plugin_files(plugin_files) -> set[str]:
+    plugin_files = cdl2list(plugin_files)
+    if not plugin_files:
+        return set()
 
+    original_tasks = set(current_app.tasks)
 
-def import_plugin_module(module_name, external_files):
-    __import__(module_name)
-    if module_name in sys.modules:
-        module_source = sys.modules[module_name].__file__
-        if module_source in external_files:
-            print("External module %s imported" % module_name)
-        else:
-            logger.error("External module %s was NOT imported. "
-                         "A module with the same name was already imported from %s" % (module_name, module_source))
+    for plugin_file in plugin_files:
+        import_plugin_file(plugin_file)
+
+    new_tasks = set(current_app.tasks) - original_tasks
+    new_tasks_modules = {t.rsplit('.', 1)[0] for t in new_tasks}
+    if new_tasks_modules:
+        print(f'{len(new_tasks)} new service{"s" if len(new_tasks)>1 else ""} imported '
+              f'from {len(new_tasks_modules)} plugin module{"s" if len(new_tasks_modules)>1 else ""} '
+              f'[{", ".join(new_tasks_modules)}]')
     else:
-        logger.error("External module %s was NOT imported." % module_name)
+        print(f'No new tasks/services imported from {plugin_files}!')
+
+    return new_tasks
 
 
-def set_plugins_env(external_files):
-    if external_files:
-        external_files = cdl2list(external_files)
-        os.environ[PLUGGING_ENV_NAME] = ",".join(external_files)
+def set_plugins_env(plugin_files):
+    plugin_files = cdl2list(plugin_files)
+    os.environ[PLUGINS_ENV_NAME] = ",".join(plugin_files)
 
 
 def get_active_plugins():
-    return os.environ.get(PLUGGING_ENV_NAME, "")
+    return os.environ.get(PLUGINS_ENV_NAME, "")
+
+
+def load_plugin_modules(plugin_files):
+    set_plugins_env(plugin_files)
+    new_tasks_imported = import_plugin_files(plugin_files)
+    # Mark the newly imported tasks with "from_plugin"
+    for t in new_tasks_imported:
+        current_app.tasks[t].from_plugin = True
+    if plugin_files:
+        _unregister_duplicate_tasks()
+
+
+def load_plugin_modules_from_env():
+    plugin_files = get_active_plugins()
+    if plugin_files:
+        load_plugin_modules(plugin_files)
 
 
 def merge_plugins(*plugin_lists) -> []:
     """Merge  comma delimited lists of plugins into a single list. Right-handed most significant plugin"""
     combined_list = []
     for plugin_list in plugin_lists:
         combined_list += delimit2list(plugin_list)
```

### Comparing `firexapp-4.9.9/firexapp/reporters/json_reporter.py` & `firexapp-5.3.0/firexapp/reporters/json_reporter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import os
+import getpass
 from socket import gethostname
 from dataclasses import dataclass, fields
-from typing import List, Dict
+from typing import List, Dict, Optional
 
 from firexapp.application import get_app_tasks
 from firexapp.common import silent_mkdir, create_link
-from firexapp.submit.reporting import ReportGenerator
 from firexkit.result import get_results
 from firexkit.task import convert_to_serializable
 from celery.utils.log import get_task_logger
 from firexapp.engine.celery import app
 
 logger = get_task_logger(__name__)
 
@@ -19,37 +19,37 @@
     completed: bool
     chain: List[str]
     firex_id: str
     logs_path: str
     submission_host: str
     submission_dir: str
     submission_cmd: List[str]
-    # TODO: the following default is temporary to workaround
-    # a testing chicken-and-egg problem. It should be removed
-    # after 25/11/2021
-    viewers: Dict[str, str] = None
-    results: Dict = None
+    viewers: Dict[str, str]
+    results: Optional[Dict] = None
     revoked: bool = False
 
-class FireXJsonReportGenerator(ReportGenerator):
+
+class FireXJsonReportGenerator:
     formatters = ('json',)
 
     reporter_dirname = 'json_reporter'
     initial_report_filename = 'initial_report.json'
     completion_report_filename = 'completion_report.json'
     report_link_filename = 'run.json'
 
     @staticmethod
-    def get_common_run_data(uid, chain, submission_dir, argv, original_cli):
-        data = {'chain': [t.short_name for t in get_app_tasks(chain)],
-                'firex_id': str(uid),
+    def get_common_run_data(uid, chain, submission_dir, argv, original_cli, inputs):
+        data = {**uid.run_data,
+                'chain': [t.short_name for t in get_app_tasks(chain)],
                 'logs_path': uid.logs_dir,
                 'submission_host': app.conf.mc or gethostname(),
                 'submission_dir': submission_dir,
                 'submission_cmd': original_cli or list(argv),
+                'submitter': getpass.getuser(),
+                'inputs': inputs
                 }
 
         viewers = uid.viewers or {}
         data.update(viewers)
         data['viewers'] = viewers
 
         return data
@@ -62,69 +62,84 @@
         with open(report_file, 'w') as f:
             json.dump(convert_to_serializable(data),
                       fp=f,
                       skipkeys=True,
                       sort_keys=True,
                       indent=4)
 
-    def pre_run_report(self, uid, chain, submission_dir, argv, original_cli=None, json_file=None, **kwargs):
-        data = self.get_common_run_data(uid=uid, chain=chain, submission_dir=submission_dir, argv=argv,
-                                        original_cli=original_cli)
+    @staticmethod
+    def create_initial_run_json(uid, chain, submission_dir, argv, original_cli=None, json_file=None,
+                                **inputs):
+        data = FireXJsonReportGenerator.get_common_run_data(uid=uid,
+                                                            chain=chain,
+                                                            submission_dir=submission_dir,
+                                                            argv=argv,
+                                                            original_cli=original_cli,
+                                                            inputs=inputs)
         data['completed'] = False
         data['revoked'] = False
-        report_file = os.path.join(uid.logs_dir, self.reporter_dirname, self.initial_report_filename)
-        self.write_report_file(data, report_file)
+        report_file = os.path.join(uid.logs_dir, FireXJsonReportGenerator.reporter_dirname,
+                                   FireXJsonReportGenerator.initial_report_filename)
+        FireXJsonReportGenerator.write_report_file(data, report_file)
 
-        report_link = os.path.join(uid.logs_dir, self.report_link_filename)
+        report_link = os.path.join(uid.logs_dir, FireXJsonReportGenerator.report_link_filename)
         try:
             create_link(report_file, report_link, delete_link=False)
         except FileExistsError:
             logger.debug(f'f{report_link} link already exist; post_run must have already run. '
                          f'No need to link to f{report_file}')
 
         if json_file:
             try:
                 create_link(report_link, json_file, delete_link=False, relative=True)
             except FileExistsError:
                 logger.debug(f'{json_file} link already exist; '
                              f'post_run must have already created the link to {report_link}')
 
-    def post_run_report(self, uid, chain, root_id, submission_dir, argv, original_cli=None, json_file=None,
-                        run_revoked=False, **kwargs):
-        data = self.get_common_run_data(uid=uid, chain=chain, submission_dir=submission_dir, argv=argv,
-                                        original_cli=original_cli)
+    @staticmethod
+    def create_completed_run_json(uid, chain, root_id, submission_dir, argv, run_revoked, original_cli=None,
+                                  json_file=None, **inputs):
+        data = FireXJsonReportGenerator.get_common_run_data(uid=uid,
+                                                            chain=chain,
+                                                            submission_dir=submission_dir,
+                                                            argv=argv,
+                                                            original_cli=original_cli,
+                                                            inputs=inputs)
         data['completed'] = True
         data['results'] = get_results(root_id)
         data['revoked'] = run_revoked
-        report_file = os.path.join(uid.logs_dir, self.reporter_dirname, self.completion_report_filename)
+        report_file = os.path.join(uid.logs_dir, FireXJsonReportGenerator.reporter_dirname,
+                                   FireXJsonReportGenerator.completion_report_filename)
 
-        self.write_report_file(data, report_file)
+        FireXJsonReportGenerator.write_report_file(data, report_file)
 
-        report_link = os.path.join(uid.logs_dir, self.report_link_filename)
+        report_link = os.path.join(uid.logs_dir, FireXJsonReportGenerator.report_link_filename)
         create_link(report_file, report_link, relative=True)
 
         if json_file:
             try:
                 # This is typically not required, unless post_run ran before pre_run
                 create_link(report_link, json_file, delete_link=False, relative=True)
             except FileExistsError:
                 # This is expected for most cases
                 pass
 
-    def add_entry(self, key_name, value, priority, formatters, **extra):
-        pass
-
 
 def get_completion_report_data(logs_dir):
     report_file = os.path.join(logs_dir, FireXJsonReportGenerator.reporter_dirname,
                                FireXJsonReportGenerator.completion_report_filename)
     with open(report_file) as f:
         return json.load(fp=f)
 
-def load_completion_report(json_file) -> FireXRunData:
+
+def is_completed_report(json_file: str) -> bool:
+    return os.path.basename(os.path.realpath(json_file)) == FireXJsonReportGenerator.completion_report_filename
+
+
+def load_completion_report(json_file: str) -> FireXRunData:
     assert os.path.isfile(json_file), f"File doesn't exist: {json_file}"
 
     with open(json_file) as f:
         run_dict = json.load(fp=f)
 
     field_names = {f.name for f in fields(FireXRunData)}
     filtered_run_dict = {k: v for k, v in run_dict.items() if k in field_names}
```

### Comparing `firexapp-4.9.9/firexapp/submit/arguments.py` & `firexapp-5.3.0/firexapp/submit/arguments.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/submit/console.py` & `firexapp-5.3.0/firexapp/submit/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import sys
 import logging
 import colorlog
-from bs4 import BeautifulSoup
+from bs4 import BeautifulSoup, MarkupResemblesLocatorWarning
 from firexkit.result import ChainInterruptedException
+import warnings
+
+# BeautifulSoup thinks we're giving it an URL because there is an URL in msg.
+# Not good. Keep stderr clean by ignoring this warning.
+warnings.filterwarnings("ignore", category=UserWarning, module='bs4')
+warnings.filterwarnings("ignore", category=MarkupResemblesLocatorWarning)
 
 console_stdout = None
 console_stderr = None
 
 
 class RequeueingUndeliverableFilter(logging.Filter):
     def filter(self, record):
```

### Comparing `firexapp-4.9.9/firexapp/submit/install_configs.py` & `firexapp-5.3.0/firexapp/submit/install_configs.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/submit/report_trigger.py` & `firexapp-5.3.0/firexapp/submit/report_trigger.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/submit/reporting.py` & `firexapp-5.3.0/firexapp/submit/reporting.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     @classmethod
     def pre_run_report(cls, kwargs):
         for report_gen in cls.get_generators():
             report_gen.pre_run_report(**kwargs)
 
     @classmethod
-    def post_run_report(cls, results, kwargs, run_revoked=False):
+    def post_run_report(cls, results, kwargs):
         if kwargs is None:
             kwargs = {}
 
         if results:
             from celery import current_app
             logger.debug("Processing results data for reports")
             for task_result in recurse_results_tree(results):
@@ -99,22 +99,21 @@
                     logger.error(f"Failed to add report entry for task result {task_result}", exc_info=True)
 
             logger.debug("Completed processing results data for reports")
 
         for report_gen in cls.get_generators():
             try:
                 logger.debug(f'Running post_run_report for {report_gen}')
-                report_gen.post_run_report(root_id=results, run_revoked=run_revoked, **kwargs)
+                report_gen.post_run_report(root_id=results, **kwargs)
                 logger.debug(f'Completed post_run_report for {report_gen}')
             except Exception:
                 # Failure in one report generator should not impact another
                 logger.error(f'Error in the post_run_report for {report_gen}', exc_info=True)
 
 
-
 def recurse_results_tree(results):
     yield results
     try:
         children = results.children or []
     except AttributeError:
         return
```

### Comparing `firexapp-4.9.9/firexapp/submit/shutdown.py` & `firexapp-5.3.0/firexapp/submit/shutdown.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import argparse
 import logging
 import subprocess
 import time
 from psutil import Process, TimeoutExpired
 from collections import namedtuple
+from typing import Optional
 
 from celery import Celery
 import redis.exceptions
 import kombu.exceptions
 
 from firexapp.celery_manager import CeleryManager
 from firexapp.submit.uid import Uid
@@ -19,51 +20,67 @@
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_CELERY_SHUTDOWN_TIMEOUT = 5 * 60
 MaybeCeleryActiveTasks = namedtuple('MaybeCeleryActiveTasks', ['celery_read_success', 'active_tasks'])
 
 
-def launch_background_shutdown(logs_dir, reason, celery_shutdown_timeout=DEFAULT_CELERY_SHUTDOWN_TIMEOUT):
+def _launch_shutdown_subprocess(shutdown_cmd: list[str]) -> int:
+    shutdown_subprocess_env = select_env_vars([REDIS_BIN_ENV, 'PATH'])
+    try:
+        import detach
+    except ModuleNotFoundError:
+        # don't break old installs that don't have detach
+        return subprocess.Popen(
+            shutdown_cmd,
+            close_fds=True,
+            env=shutdown_subprocess_env,
+            preexec_fn=os.setpgrp,
+        ).pid
+    else:
+        return detach.call(
+            shutdown_cmd,
+            env=shutdown_subprocess_env,
+        )
+
+
+def launch_background_shutdown(logs_dir, reason, celery_shutdown_timeout=DEFAULT_CELERY_SHUTDOWN_TIMEOUT) -> Optional[int]:
     try:
         shutdown_cmd = [qualify_firex_bin("firex_shutdown"),
                         "--logs_dir",  logs_dir,
                         "--celery_shutdown_timeout", str(celery_shutdown_timeout)]
         if reason:
             shutdown_cmd += ['--reason', reason]
-        pid = subprocess.Popen(shutdown_cmd,
-                               close_fds=True,
-                               env=select_env_vars([REDIS_BIN_ENV, 'PATH']),
-                               preexec_fn=os.setpgrp,
-                               ).pid
-    except Exception as e:
-        logger.error("SHUTDOWN PROCESS FAILED TO LAUNCH -- REDIS WILL LEAK.")
-        logger.error(e)
+        pid = _launch_shutdown_subprocess(shutdown_cmd)
+    except Exception:
+        logger.exception("SHUTDOWN PROCESS FAILED TO LAUNCH -- REDIS WILL LEAK.")
         raise
     else:
         try:
             Process(pid).wait(0.1)
         except TimeoutExpired:
-            logger.debug("Started background shutdown with pid %s" % pid)
+            logger.debug(f"Started background shutdown with pid {pid}")
+            return pid
         else:
             logger.error("SHUTDOWN PROCESS FAILED TO RUN -- REDIS WILL LEAK.")
+            return None
 
 
 def wait_for_broker_shutdown(broker, timeout=15, force_kill=True):
     logger.debug("Waiting for broker to shut down")
     shutdown_wait_time = time.time() + timeout
     while time.time() < shutdown_wait_time:
         if not broker.is_alive():
             break
         time.sleep(0.1)
 
     if not broker.is_alive():
         logger.debug("Confirmed successful graceful broker shutdown.")
     elif force_kill:
-        logger.debug("Warning! Broker was not shut down after %s seconds. FORCE KILLING BROKER." % str(timeout))
+        logger.debug(f"Warning! Broker was not shut down after {timeout} seconds. FORCE KILLING BROKER.")
         broker.force_kill()
 
     return not broker.is_alive()
 
 
 def _inspect_broker_safe(inspect_fn, broker, celery_app, **kwargs):
     #
@@ -108,32 +125,36 @@
 
 
 def revoke_active_tasks(broker, celery_app,  max_revoke_retries=5, task_predicate=lambda task: True):
     logger.debug("Querying Celery to find any remaining active tasks.")
     maybe_active_tasks = _tasks_from_active(get_active_broker_safe(broker, celery_app), task_predicate)
     revoke_retries = 0
     # Revoke retry loop
-    while (maybe_active_tasks.celery_read_success
-           and maybe_active_tasks.active_tasks
-           and revoke_retries < max_revoke_retries):
+    while (
+        maybe_active_tasks.celery_read_success
+        and maybe_active_tasks.active_tasks
+        and revoke_retries < max_revoke_retries
+    ):
         if revoke_retries:
-            logger.warning("Found %s active tasks after revoke. Revoking active tasks again."
-                           % len(maybe_active_tasks.active_tasks))
+            logger.warning(f"Found {len(maybe_active_tasks.active_tasks)} active tasks after revoke. Revoking active tasks again.")
 
         # Revoke tasks in order they were started. This avoids ChainRevokedException errors when children are revoked
         # before their parents.
         for task in sorted(maybe_active_tasks.active_tasks, key=lambda t: t.get('time_start', float('inf'))):
             logger.info(f"Revoking {task['name']}[{task['id']}]")
             celery_app.control.revoke(task_id=task["id"], terminate=True)
 
         # wait for confirmation of revoke
         maybe_active_tasks = _tasks_from_active(get_active_broker_safe(broker, celery_app), task_predicate)
         wait_for_task_revoke_start = time.monotonic()
-        while maybe_active_tasks.celery_read_success and maybe_active_tasks.active_tasks \
-                and time.monotonic() - wait_for_task_revoke_start < 3:
+        while (
+            maybe_active_tasks.celery_read_success
+            and maybe_active_tasks.active_tasks
+            and time.monotonic() - wait_for_task_revoke_start < 3
+        ):
             time.sleep(0.25)
             maybe_active_tasks = _tasks_from_active(get_active_broker_safe(broker, celery_app), task_predicate)
 
         revoke_retries += 1
 
     if not maybe_active_tasks.celery_read_success:
         logger.info("Failed to read active tasks from celery. May shutdown with unrevoked tasks.")
@@ -197,16 +218,17 @@
         if broker.is_alive():
             logger.info("Broker is alive; sending redis shutdown.")
             broker.shutdown()
             wait_for_broker_shutdown(broker)
         else:
             logger.info("No active Broker.")
 
-    logger.info("Shutdown of %s complete." % logs_dir)
+    logger.info(f"Shutdown of {logs_dir} complete.")
 
 
-def main():
+def main() -> None:
     logs_dir, reason, celery_shutdown_timeout = init()
     try:
         shutdown_run(logs_dir, celery_shutdown_timeout, reason)
-    except Exception as e:
-        logger.exception(e)
+    except BaseException:
+        logger.exception("Shutdown failed.")
+        raise
```

### Comparing `firexapp-4.9.9/firexapp/submit/submit.py` & `firexapp-5.3.0/firexapp/submit/submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,44 +11,47 @@
 
 from celery.signals import worker_ready
 from shutil import copyfile
 from contextlib import contextmanager
 
 from celery.exceptions import NotRegistered
 from firexapp.discovery import get_all_pkg_versions_str
+from firexapp.engine.default_celery_config import primary_worker_minimum_concurrency
 from firexapp.engine.logging import add_hostname_to_log_records
 
 from firexkit.result import wait_on_async_results, disable_async_result, ChainRevokedException, \
     mark_queues_ready, get_results, get_task_name_from_result, ChainRevokedPreRunException, \
     monkey_patch_async_result_to_track_instances, is_async_result_monkey_patched_to_track, disable_all_async_results
 from firexkit.chain import InjectArgs, verify_chain_arguments, InvalidChainArgsException
 from firexapp.fileregistry import FileRegistry
 from firexapp.submit.uid import Uid
 from firexapp.submit.arguments import InputConverter, ChainArgException, get_chain_args, find_unused_arguments
 from firexapp.submit.tracking_service import get_tracking_services, get_service_name
 from firexapp.plugins import plugin_support_parser
 from firexapp.submit.console import setup_console_logging
-from firexapp.application import import_microservices, get_app_tasks, get_app_task
+from firexapp.application import import_microservices, get_app_tasks, get_app_task, JSON_ARGS_PATH_ARG_NAME
 from firexapp.engine.celery import app
 from firexapp.broker_manager.broker_factory import BrokerFactory
 from firexapp.submit.shutdown import launch_background_shutdown, DEFAULT_CELERY_SHUTDOWN_TIMEOUT
 from firexapp.submit.install_configs import load_new_install_configs, FireXInstallConfigs, INSTALL_CONFIGS_ENV_NAME
 from firexapp.submit.arguments import whitelist_arguments
 from firexapp.common import dict2str, silent_mkdir, create_link
+from firexapp.reporters.json_reporter import FireXJsonReportGenerator
 
 add_hostname_to_log_records()
 logger = setup_console_logging(__name__)
 
 
 SUBMISSION_FILE_REGISTRY_KEY = 'firex_submission'
 FileRegistry().register_file(SUBMISSION_FILE_REGISTRY_KEY, os.path.join(Uid.debug_dirname, 'submission.txt'))
 
 ENVIRON_FILE_REGISTRY_KEY = 'env'
 FileRegistry().register_file(ENVIRON_FILE_REGISTRY_KEY, os.path.join(Uid.debug_dirname, 'environ.json'))
 
+RUN_SOFT_TIME_LIMIT_KEY = 'run_soft_time_limit'
 
 class JsonFileAction(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
 
         if not os.path.isabs(values):
             values = os.path.join(os.getcwd(), values)
 
@@ -71,18 +74,34 @@
         if isinstance(values, str):
             values = True if values.lower() == 'true' else False
         setattr(namespace, self.dest, values)
 
 
 class AdjustCeleryConcurrency(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
-        concurrency = max([values, 4])
+        concurrency = max([values, primary_worker_minimum_concurrency])
         setattr(namespace, self.dest, concurrency)
 
 
+def safe_create_completed_run_json(chain_result, run_revoked, chain_args):
+    try:
+        FireXJsonReportGenerator.create_completed_run_json(root_id=chain_result,
+                                                           run_revoked=run_revoked,
+                                                           **chain_args)
+    except Exception as e:
+        logger.error(f'Failed to generate completion run JSON: {e}')
+
+
+def safe_create_initial_run_json(**kwargs):
+    try:
+        FireXJsonReportGenerator.create_initial_run_json(**kwargs)
+    except Exception as e:
+        logger.error(f'Failed to generate initial run JSON: {e}')
+
+
 class SubmitBaseApp:
     SUBMISSION_LOGGING_FORMATTER = '[%(asctime)s %(levelname)s] %(message)s'
     DEFAULT_MICROSERVICE = None
 
     install_configs: FireXInstallConfigs
 
     def __init__(self, submission_tmp_file=None):
@@ -151,21 +170,24 @@
         submit_parser.add_argument('--install_configs', help="Path to JSON file specifying installation-wide configs",
                                    type=str, default=os.environ.get(INSTALL_CONFIGS_ENV_NAME, None))
         submit_parser.add_argument('--celery_concurrency', '--celery_work_slots',
                                    type=int, action=AdjustCeleryConcurrency,
                                    help='Number of worker slots in celery pool',
                                    # default is autoscale from a minimum of cpu_count, to a maximum of 8*cpu_count
                                    default=None)
-        submit_parser.add_argument('--json_file', help='Link name for the report json file', action=JsonFileAction)
+        submit_parser.add_argument('--json_file', '--json_results_file', help='Link name for the report json file', action=JsonFileAction)
         submit_parser.add_argument('--tracking_services_wait_release_console',
                                    help='Wait for tracking services (e.g. Flame) to indicate they are ready to release '
                                         'the console before doing so.', nargs='?', const=True,
                                    default=True, action=OptionalBoolean)
         submit_parser.add_argument('--celery_shutdown_timeout', help='How long to wait in seconds for Celery during shutdown.',
                                    default=DEFAULT_CELERY_SHUTDOWN_TIMEOUT, type=int)
+        submit_parser.add_argument(JSON_ARGS_PATH_ARG_NAME,
+                                   help='Specify submit arguments via a JSON file containing a list of argument names and values.')
+
 
         submit_parser.set_defaults(func=self.run_submit)
 
         for service in get_tracking_services():
             service.extra_cli_arguments(submit_parser)
 
         return submit_parser
@@ -283,17 +305,15 @@
         if args.logs_link:
             self.create_logs_link(args.logs_link)
 
         if self.install_configs.has_viewer():
             uid.add_viewers(logs_url=self.install_configs.get_logs_root_url())
             logger.info(f'Logs URL: {uid.logs_url}')
 
-        # Create an env file for debugging
-        with open(FileRegistry().get_file(ENVIRON_FILE_REGISTRY_KEY, self.uid.logs_dir), 'w') as f:
-            json.dump(dict(os.environ), fp=f, skipkeys=True, sort_keys=True, indent=4)
+        self.dump_environ()
 
         chain_args = self.convert_chain_args(chain_args)
 
         chain_args = self.start_engine(args=args, chain_args=chain_args, uid=uid)
 
         # Execute chain
         try:
@@ -303,14 +323,15 @@
             root_task = get_app_task(root_task_name)
         except NotRegistered as e:
             logger.error(e)
             self.main_error_exit_handler(reason=str(e))
             sys.exit(-1)
         self.wait_tracking_services_task_ready()
 
+        safe_create_initial_run_json(**chain_args)
         # AsyncResult objects cannot be in memory after the broker (i.e. backend) shutdowns, otherwise errors are
         # produced when they are garbage collected. We therefore monkey patch AsyncResults to track all instances
         # (e.g. from unpickle, instantiated directly, etc) so that disable_all_async_results can disable their
         # references to the backend.
         monkey_patch_async_result_to_track_instances()
         root_task_result_promise = root_task.s(submit_app=self, **chain_args).delay()
 
@@ -320,14 +341,25 @@
             logger.info("Waiting for chain to complete...")
             chain_results = self.process_sync(root_task_result_promise, chain_args)
             results_str = self.format_results_str(chain_results)
             self.log_results(results_str)
             self.self_destruct(chain_details=(root_task_result_promise, chain_args),
                                reason="Sync run: completed successfully")
 
+    def dump_environ(self):
+        # Mask  any password-related env vars before dumping them in the environ.json
+        copy_of_os_environ = os.environ.copy()
+        for k in copy_of_os_environ:
+            if any(e in k.lower() for e in ['passwd', 'password']):
+                copy_of_os_environ[k] = '********'
+
+        # Create an env file for debugging
+        with open(FileRegistry().get_file(ENVIRON_FILE_REGISTRY_KEY, self.uid.logs_dir), 'w') as f:
+            json.dump(copy_of_os_environ, fp=f, skipkeys=True, sort_keys=True, indent=4)
+
     def check_for_failures(self, root_task_result_promise, unsuccessful_services):
         if unsuccessful_services:
             msg, rc = format_unsuccessful_services(unsuccessful_services)
             raise FireXReturnCodeException(msg, rc)
 
     def set_broker_in_app(self):
         from firexapp.engine.celery import app
@@ -344,14 +376,16 @@
         self.set_broker_in_app()
 
         try:
             # start backend
             app.backend.set('uid', str(uid))
             app.backend.set('logs_dir', uid.logs_dir)
             app.backend.set('resources_dir', uid.resources_dir)
+            if args.soft_time_limit:
+                app.backend.set(RUN_SOFT_TIME_LIMIT_KEY, args.soft_time_limit)
 
             # IMPORT ALL THE MICROSERVICES
             # ONLY AFTER BROKER HAD STARTED
             all_tasks = import_microservices(chain_args.get("plugins", args.plugins))
         except FileNotFoundError as e:
             logger.error("\nError: FireX run failed. File %s is not found." % e)
             self.main_error_exit_handler(reason=str(e))
@@ -401,19 +435,20 @@
         with self.graceful_exit_on_failure("Unable to start Celery."):
             self.start_celery(args, chain_args.get("plugins", args.plugins))
         return chain_args
 
     def start_celery(self, args, plugins):
         from firexapp.celery_manager import CeleryManager
         celery_manager = CeleryManager(logs_dir=self.uid.logs_dir, plugins=plugins)
-        cpu_count = multiprocessing.cpu_count()
+        auto_scale_min = primary_worker_minimum_concurrency
+        auto_scale_max = multiprocessing.cpu_count()*8
         celery_manager.start(workername=app.conf.primary_worker_name,
                              wait=True,
                              concurrency=args.celery_concurrency,
-                             autoscale=None if args.celery_concurrency else (cpu_count, cpu_count*8),
+                             autoscale=None if args.celery_concurrency else (auto_scale_min, auto_scale_max),
                              soft_time_limit=args.soft_time_limit)
         self.celery_manager = celery_manager
 
     def process_other_chain_args(self, args, other_args)-> {}:
         try:
             chain_args = get_chain_args(other_args)
         except ChainArgException as e:
@@ -427,14 +462,15 @@
         chain_args['chain'] = args.chain
         chain_args['plugins'] = args.plugins
         chain_args['sync'] = args.sync
         chain_args['submitter'] = getuser()
         chain_args['submission_dir'] = os.getcwd()
         chain_args['argv'] = sys.argv
         chain_args['json_file'] = args.json_file
+
         whitelist_arguments(['submitter', 'submission_dir', 'argv'])
 
         return chain_args
 
     def start_broker(self, args):
         from firexapp.broker_manager.broker_factory import BrokerFactory
         self.broker = BrokerFactory.create_new_broker_manager(logs_dir=self.uid.logs_dir)
@@ -506,38 +542,38 @@
                 msg = f'{s}: see {launch_file}' if launch_file else s
                 logger.warning('\t' + msg)
         else:
             wait_duration = time.time() - start_wait_time
             logger.debug("Waited %.1f secs for tracking services to be %s." % (wait_duration, description))
 
     def wait_tracking_services_task_ready(self, timeout=5)->None:
-        self.wait_tracking_services_pred(lambda s: s.ready_for_tasks(), 'ready for tasks', timeout)
+        self.wait_tracking_services_pred(lambda s: s.ready_for_tasks(celery_app=app), 'ready for tasks', timeout)
 
     def wait_tracking_services_release_console_ready(self, timeout=5)->None:
         self.wait_tracking_services_pred(lambda s: s.ready_release_console(), 'ready to release console', timeout)
 
-    def main_error_exit_handler(self, chain_details=None, reason=None):
+    def main_error_exit_handler(self, chain_details=None, reason=None, run_revoked=False):
         mssg = 'Aborting FireX submission...'
         if reason:
             mssg += '\n' + str(reason)
         logger.error(mssg)
         if self.broker:
-            self.self_destruct(chain_details=chain_details, reason=reason)
+            self.self_destruct(chain_details=chain_details, reason=reason, run_revoked=run_revoked)
         if self.uid:
             self.copy_submission_log()
 
     def self_destruct(self, chain_details=None, reason=None, run_revoked=False):
         if chain_details:
             chain_result, chain_args = chain_details
+            safe_create_completed_run_json(chain_result, run_revoked, chain_args)
             try:
                 logger.debug("Generating reports")
                 from firexapp.submit.reporting import ReportersRegistry
                 ReportersRegistry.post_run_report(results=chain_result,
-                                                  kwargs=chain_args,
-                                                  run_revoked=run_revoked)
+                                                  kwargs=chain_args)
                 logger.debug('Reports successfully generated')
             except Exception:
                 # Under no circumstances should report generation prevent celery and broker cleanup
                 logger.error('Error in generating reports', exc_info=True)
             finally:
                 # AsyncResult objects access self.backend when garbage collected. Since we're about to initiate a
                 # process to stop the backend, prevent all AsyncResult objects from accessing self.backend.
@@ -609,24 +645,35 @@
         self.firex_returncode = firex_returncode
         super(Exception, self).__init__(error_msg, firex_returncode)
 
     def __str__(self):
         return self.error_msg + '\n' + f'[RC {self.firex_returncode}]'
 
 
-def get_unsuccessful_items(list_of_tasks):
+def get_unsuccessful_items(list_of_tasks, filters=None):
+    if not filters:
+        filters = []
     failures_by_name = {}
     for task_async_result in list_of_tasks:
         task_name = get_task_name_from_result(task_async_result)
         try:
             failures_by_name[task_name] += 1
         except KeyError:
             failures_by_name[task_name] = 1
     formatted_list = []
     for task_name, instances in failures_by_name.items():
+        # Apply filters
+        ignore = False
+        for f in filters:
+            if re.fullmatch(f, task_name):
+                ignore = True
+                break
+        if ignore:
+            continue
+        # Record the failed task
         item = f'\t- {task_name}'
         if instances > 1:
             item += f' ({instances} instances)'
         formatted_list.append(item)
     return formatted_list
```

### Comparing `firexapp-4.9.9/firexapp/submit/tracking_service.py` & `firexapp-5.3.0/firexapp/submit/tracking_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Tuple
+from typing import Optional
 
 from firexapp.discovery import get_firex_tracking_services_entry_points, PkgVersionInfo
 from firexapp.submit.install_configs import FireXInstallConfigs
 
 _services = None
 
 
@@ -20,30 +20,31 @@
 
     def ready_for_tasks(self, **kwargs) -> bool:
         return True
 
     def ready_release_console(self, **kwargs) -> bool:
         return True
 
-    def get_pkg_version_info(self) -> PkgVersionInfo:
-        pass
+    def get_pkg_version_info(self) -> Optional[PkgVersionInfo]:
+        return None
 
 
 def get_service_name(service: TrackingService) -> str:
     return service.__class__.__name__
 
 
-def get_tracking_services() -> Tuple[TrackingService]:
+def get_tracking_services() -> Optional[tuple[TrackingService]]:
     global _services
     if _services is None:
         entry_pts = get_firex_tracking_services_entry_points()
         entry_objects = [e.load() for e in entry_pts]
         _services = tuple([point() for point in entry_objects])
     return _services
 
-def get_tracking_services_versions() -> [PkgVersionInfo]:
-    return [service.get_pkg_version_info() for service in get_tracking_services()]
+def get_tracking_services_versions() -> list[PkgVersionInfo]:
+    version_infos = [service.get_pkg_version_info() for service in get_tracking_services()]
+    return [v for v in version_infos if v]
 
 def has_flame() -> bool:
     # Unfortunate coupling, but just too many things vary depending on presence of flame. Will eventually bring
     # flame in to firexapp.
     return 'FlameLauncher' in get_tracking_services()
```

### Comparing `firexapp-4.9.9/firexapp/submit/uid.py` & `firexapp-5.3.0/firexapp/submit/uid.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,75 @@
+from dataclasses import dataclass
 import os
 import datetime
 import pytz
 import tempfile
 from getpass import getuser
 import random
 import firexkit
 import shutil
+import re
+from typing import Optional
+from collections import namedtuple
 
 from firexapp.submit.arguments import whitelist_arguments
 from firexkit.permissions import DEFAULT_CHMOD_MODE
 
 BASE_LOGGING_DIR_ENV_VAR_KEY = 'firex_base_logging_dir'
 
+FIREX_ID_DATE_FMT = "%y%m%d-%H%M%S"
+FIREX_ID_REGEX = re.compile(r'^FireX-(?P<user>.*?)-(?P<datetime_str>\d{6}-\d{6})-(?P<random_int>\d+)$')
+
+
+def firex_id_str(user: str, timestamp: datetime.datetime, random_int: int) -> str:
+    return f'FireX-{user}-{timestamp.strftime(FIREX_ID_DATE_FMT)}-{random_int}'
+
+
+@dataclass(frozen=True)
+class FireXIdParts:
+    user: str
+    timestamp: datetime.datetime
+    random_int: int
+
+    def firex_id(self):
+        return firex_id_str(self.user, self.timestamp, self.random_int)
+
+
+def get_firex_id_parts(maybe_firex_id: str) -> Optional[FireXIdParts]:
+    m = FIREX_ID_REGEX.match(maybe_firex_id)
+    if m:
+        parts = m.groupdict()
+        try:
+             tz_unaware_datetime = datetime.datetime.strptime(
+                parts['datetime_str'],
+                FIREX_ID_DATE_FMT)
+        except ValueError:
+            pass # invalidate date format.
+        else:
+            tz_aware_datetime = pytz.utc.localize(tz_unaware_datetime)
+            return FireXIdParts(parts['user'], tz_aware_datetime, int(parts['random_int']))
+    return None
+
+
+def is_firex_id(maybe_firex_id: str) -> bool:
+    return bool(get_firex_id_parts(maybe_firex_id))
+
 
 class Uid(object):
     debug_dirname = 'firex_internal'
     _resources_dirname = os.path.join(debug_dirname, 'resources')
 
     def __init__(self, identifier=None):
         self.timestamp = datetime.datetime.now(tz=pytz.utc)
         self.user = getuser()
         if identifier:
             self.identifier = identifier
         else:
             random.seed()
-            self.identifier = f'FireX-{self.user}-{self.timestamp.strftime("%y%m%d-%H%M%S")}-{random.randint(1, 65536)}'
+            self.identifier = firex_id_str(self.user, self.timestamp, random.randint(1, 65536))
         self._base_logging_dir = None
         self._logs_dir = None
         self._debug_dir = None
         self._viewers = {}
 
     @property
     def base_logging_dir(self):
@@ -102,9 +143,14 @@
     @property
     def logs_url(self):
         try:
             return self.viewers['logs_url']
         except KeyError:
             return None
 
+    @property
+    def run_data(self):
+        return {'firex_id': self.identifier,
+                'logs_path': self.logs_dir}
+
 
 whitelist_arguments("uid")
```

### Comparing `firexapp-4.9.9/firexapp/tasks/core_tasks.py` & `firexapp-5.3.0/firexapp/tasks/core_tasks.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/tasks/example.py` & `firexapp-5.3.0/firexapp/tasks/example.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/tasks/root_tasks.py` & `firexapp-5.3.0/firexapp/tasks/root_tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,27 @@
 from firexkit.result import get_results
 
 from firexapp.application import get_app_tasks
 from firexapp.engine.celery import app
 
 logger = get_task_logger(__name__)
 
+root_revoked_backend_key = 'ROOT_REVOKED'
+
+#
+# Set flag in backend DB (i.e.: Redis) to indicate root taks has been revoked
+#
+def backend_set_root_revoked():
+     app.backend.set(root_revoked_backend_key, 'True')
+
+#
+# Get flag in backend DB (i.e.: Redis) which indicates root taks has been revoked
+#
+def backend_get_root_revoked():
+     return app.backend.get(root_revoked_backend_key)
 
 # noinspection PyPep8Naming
 @app.task(bind=True, returns=('chain_results', 'unsuccessful_services'))
 def RootTask(self, chain, **chain_args):
     c = InjectArgs(chain=chain, **chain_args)
     for task in get_app_tasks(chain):
         c |= task.s()
@@ -36,15 +49,14 @@
         root_task_name = root_task_name.lstrip(".")
         root_module = import_module(root_module_name)
         return getattr(root_module, root_task_name)
     else:
         # default FireXApp root task
         return RootTask
 
-
 # noinspection PyUnusedLocal
 @task_postrun.connect(sender=get_configured_root_task())
 def handle_firex_root_completion(sender, task, task_id, args, kwargs, **do_not_care):
     logger.info("Root task completed.")
 
     submit_app = kwargs.get("submit_app")
     if not submit_app:
@@ -52,14 +64,18 @@
         return
 
     result = task.AsyncResult(task_id)
     sync = kwargs.get("sync", False)
 
     result_state = result.state
     is_revoked = result_state in [REVOKED, RETRY] # Revoked can be in retry state with celery 5.1.0
+
+    if is_revoked:
+        backend_set_root_revoked()
+
     if sync and not is_revoked:
         logger.debug("Sync run has not been revoked. Cleanup skipped.")
         # Only if --sync run was revoked do we want to do the shutdown here; else it's done in firex.py
         return
 
     # Let this signal cause self-destruct
     submit_app.self_destruct(chain_details=(result, kwargs),
```

### Comparing `firexapp-4.9.9/firexapp/testing/config_base.py` & `firexapp-5.3.0/firexapp/testing/config_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     def assert_expected_firex_output(self, cmd_output, cmd_err):
         pass
 
     @abc.abstractmethod
     def assert_expected_return_code(self, ret_value):
         pass
 
+    def cleanup(self):
+        pass
+
 
 class InterceptFlowTestConfiguration(FlowTestConfiguration):
     __metaclass__ = abc.ABCMeta
 
     def assert_expected_return_code(self, ret_value):
         assert 0 == ret_value, "Expected return code of 0"
```

### Comparing `firexapp-4.9.9/firexapp/testing/config_interpreter.py` & `firexapp-5.3.0/firexapp/testing/config_interpreter.py`

 * *Files 5% similar despite different names*

```diff
@@ -195,23 +195,16 @@
 
             verification_start_time = time.monotonic()
             # check for expected return code
             expected_return = flow_test_config.assert_expected_return_code(process.returncode)
             if expected_return is not None:
                 raise Exception("assert_expected_return_code should not return. It should assert if needed")
 
-            if self.tmp_json_file:
-                # Dealing with firex as an external process is non-trivial. There is no guarantee json_file
-                # will ever be populated, and it may be created after the console is released. Yikes. Guess
-                # the timeout value to avoid waiting in lots of cases when we know it will never appear, like
-                # invalid args or failed tracking services.
-                json_path_timeout = 10 if process.returncode == 0 else 0
-                exists = wait_until(os.path.isfile, timeout=json_path_timeout, sleep_for=0.2, path=self.tmp_json_file)
-                if exists:
-                    flow_test_config.run_data = load_completion_report(self.tmp_json_file)
+            if self.tmp_json_file and os.path.isfile(self.tmp_json_file):
+                flow_test_config.run_data = load_completion_report(self.tmp_json_file)
 
             if self.is_submit_command(flow_test_config) and process.returncode == 0 and \
                     self.is_instance_of_intercept(flow_test_config) and \
                     flow_test_config.intercept_service():
                 # retrieve captured kwargs and validate them
                 intercept_results_file = self.get_intercept_results_file(flow_test_config)
                 if not os.path.isfile(intercept_results_file):
@@ -236,14 +229,19 @@
             raise
         except Exception as e:
             print('\tException: {}: {}'.format(type(e).__name__, e), file=sys.stderr)
             raise
         finally:
             self.on_test_exit(flow_test_config.std_out, flow_test_config.std_err)
 
+            try:
+                flow_test_config.cleanup()
+            except Exception as cleanup_e:
+                print(f'Exception during flow test cleanup: {cleanup_e}')
+
             if self.tmp_json_file and os.path.exists(self.tmp_json_file):
                 os.unlink(self.tmp_json_file)
 
             # report on time
             if elapsed_time is not None:
                 msg = "\tTime %.1fs" % elapsed_time
                 if verification_time is not None:
```

### Comparing `firexapp-4.9.9/firexapp/testing/coverage_plugin.py` & `firexapp-5.3.0/firexapp/testing/coverage_plugin.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/firexapp/testing/pydev_debug_plugin.py` & `firexapp-5.3.0/firexapp/testing/pydev_debug_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,16 +38,21 @@
 
 
 def get_pydev_command(cmd, setup=None, pydev=None, debug_host=None):
     if not setup:
         setup, pydev = get_pydev_debug_setup()
     pydev_cmd = [sys.executable, pydev]
     client = str(setup['client'])
-    client = client if "127.0.0.1" not in client else (debug_host or gethostname())
-    pydev_cmd += ['--multiproc', '--client', client, '--port', str(setup['port']), '--file']
+
+    if "127.0.0.1" in client and debug_host and debug_host != gethostname():
+        #  This is broken on newer pycharm, since it binds pydev debugger only to 127.0.0.1:<port>
+        client = debug_host
+    proc_str = '--multiprocess' if setup.get('multiprocess') else '--multiproc'
+
+    pydev_cmd += [proc_str, '--client', client, '--port', str(setup['port']), '--file']
     if type(cmd) is str:
         cmd = [cmd]
     pydev_cmd += cmd
     return pydev_cmd
 
 
 def is_celery():
```

### Comparing `firexapp-4.9.9/firexapp/testing/test_infra.py` & `firexapp-5.3.0/firexapp/testing/test_infra.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,19 @@
             exit(-1)
     elif args.no_html:
         parser.error("--no_html cannot be used without --coverage")
 
     # prepare logging directory
     results_directory = os.path.realpath(args.logs)
     if os.path.isdir(results_directory):
-        shutil.rmtree(results_directory)
+        try:
+            shutil.rmtree(results_directory)
+        except OSError:
+            print(f"Couldn't remove {results_directory!r}. Some process still owns files in that directory.")
+            raise
     os.umask(DEFAULT_UMASK)
     os.mkdir(results_directory)
 
     FlowTestInfra.config_interpreter.profile = args.profile
     FlowTestInfra.config_interpreter.coverage = args.coverage
     FlowTestInfra.config_interpreter.is_public = args.public_runs
     FlowTestInfra.results_dir = results_directory
@@ -113,17 +117,18 @@
         orig_output = os.path.join(args.logs, xunit_file_name)
 
     if args.coverage:
         os.environ["COVERAGE_FILE"] = os.path.join(results_directory, ".coverage")
 
     import xmlrunner
     success = unittest.main(module=FlowTestInfra.__module__,
-                            testRunner=xmlrunner.XMLTestRunner(output=args.logs, outsuffix="results"),
+                            testRunner=xmlrunner.XMLTestRunner(output=args.logs, outsuffix="results", verbosity=2),
                             argv=sys.argv[:1],
-                            exit=False).result.wasSuccessful()
+                            exit=False,
+                            verbosity=2).result.wasSuccessful()
 
     # let the user decide what to call the output
     if args.xunit_file_name:
         os.rename(orig_output,
                   os.path.join(args.logs, os.path.basename(args.xunit_file_name)))
     if args.coverage:
         print("combining coverage files...", file=sys.stderr)
```

### Comparing `firexapp-4.9.9/firexapp.egg-info/SOURCES.txt` & `firexapp-5.3.0/firexapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.9/setup.py` & `firexapp-5.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,20 +21,21 @@
       install_requires=[
           "distlib",
           "firexkit",
           "tqdm<=4.29.1",
           "xmlrunner",
           "redis",
           "hiredis",
-          "celery[redis]==5.2.0",
+          "celery[redis]==5.3.1",
           "psutil",
           "python-Levenshtein",
           "entrypoints",
           "colorlog==2.10.0",
           "beautifulsoup4",
+          "detach3k",
       ],
       extras_require={
           'test': [
               'firex-keeper',
           ],
           'flame': [
               'firex-flame'
@@ -49,7 +50,8 @@
           'firex.core': 'firexapp = firexapp',
           'console_scripts': ['firexapp = firexapp.application:main',
                               'flow_tests = firexapp.testing.test_infra:default_main',
                               'firex_shutdown = firexapp.submit.shutdown:main',
                               ],
       },
       )
+
```

### Comparing `firexapp-4.9.9/versioneer.py` & `firexapp-5.3.0/versioneer.py`

 * *Files identical despite different names*

