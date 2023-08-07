# Comparing `tmp/switch_api-0.4.6.tar.gz` & `tmp/switch_api-0.4.6b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switch_api-0.4.6.tar", last modified: Mon Aug  7 05:48:45 2023, max compression
+gzip compressed data, was "switch_api-0.4.6b2.tar", last modified: Fri Jun 23 06:58:17 2023, max compression
```

## Comparing `switch_api-0.4.6.tar` & `switch_api-0.4.6b2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.790097 switch_api-0.4.6/
--rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-08-07 05:48:29.000000 switch_api-0.4.6/AUTHORS.rst
--rw-r--r--   0 vsts      (1001) docker     (122)    28236 2023-08-07 05:48:29.000000 switch_api-0.4.6/HISTORY.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-08-07 05:48:29.000000 switch_api-0.4.6/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-08-07 05:48:29.000000 switch_api-0.4.6/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    29510 2023-08-07 05:48:45.790097 switch_api-0.4.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      590 2023-08-07 05:48:29.000000 switch_api-0.4.6/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-08-07 05:48:29.000000 switch_api-0.4.6/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-08-07 05:48:45.794098 switch_api-0.4.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1346 2023-08-07 05:48:29.000000 switch_api-0.4.6/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.786097 switch_api-0.4.6/switch_api/
--rw-r--r--   0 vsts      (1001) docker     (122)     1453 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.786097 switch_api-0.4.6/switch_api/_authentication/
--rw-r--r--   0 vsts      (1001) docker     (122)      391 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/_authentication/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7898 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/_authentication/_authentication.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.786097 switch_api-0.4.6/switch_api/_authentication/_credentials_store/
--rw-r--r--   0 vsts      (1001) docker     (122)      393 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/_authentication/_credentials_store/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5851 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/_authentication/_credentials_store/_credentials_store.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.786097 switch_api-0.4.6/switch_api/_authentication/_msal/
--rw-r--r--   0 vsts      (1001) docker     (122)      361 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/_authentication/_msal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8752 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/_authentication/_msal/_custom_application.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.786097 switch_api-0.4.6/switch_api/_utils/
--rw-r--r--   0 vsts      (1001) docker     (122)      462 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/_utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3783 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/_utils/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12998 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/_utils/_platform.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16873 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/_utils/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.790097 switch_api-0.4.6/switch_api/analytics/
--rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/analytics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9561 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/analytics/analytics.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.790097 switch_api-0.4.6/switch_api/cache/
--rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/cache/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6985 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/cache/cache.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.790097 switch_api-0.4.6/switch_api/dataset/
--rw-r--r--   0 vsts      (1001) docker     (122)      558 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7724 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/dataset/dataset.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.790097 switch_api-0.4.6/switch_api/email/
--rw-r--r--   0 vsts      (1001) docker     (122)      472 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/email/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4638 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/email/email_sender.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.790097 switch_api-0.4.6/switch_api/error_handlers/
--rw-r--r--   0 vsts      (1001) docker     (122)     2028 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/error_handlers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11845 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/error_handlers/error_handlers.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.790097 switch_api-0.4.6/switch_api/extensions/
--rw-r--r--   0 vsts      (1001) docker     (122)     1038 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/extensions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7519 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/extensions/extensions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1652 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/extensions/field_meta.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2970 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/extensions/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1406 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/extensions/pipeline.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3193 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/initialize.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.790097 switch_api-0.4.6/switch_api/integration/
--rw-r--r--   0 vsts      (1001) docker     (122)     1601 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/integration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11314 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/integration/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26453 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/integration/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)    89676 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/integration/integration.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.790097 switch_api-0.4.6/switch_api/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)     3144 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    75318 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/pipeline/automation.py
--rw-r--r--   0 vsts      (1001) docker     (122)    35931 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/pipeline/definitions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21094 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/pipeline/pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.790097 switch_api-0.4.6/switch_api/platform_insights/
--rw-r--r--   0 vsts      (1001) docker     (122)      542 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/platform_insights/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-08-07 05:48:29.000000 switch_api-0.4.6/switch_api/platform_insights/platform_insights.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-07 05:48:45.786097 switch_api-0.4.6/switch_api.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    29510 2023-08-07 05:48:45.000000 switch_api-0.4.6/switch_api.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1600 2023-08-07 05:48:45.000000 switch_api-0.4.6/switch_api.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-07 05:48:45.000000 switch_api-0.4.6/switch_api.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       84 2023-08-07 05:48:45.000000 switch_api-0.4.6/switch_api.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-08-07 05:48:45.000000 switch_api-0.4.6/switch_api.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.713812 switch_api-0.4.6b2/
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/AUTHORS.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    26549 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/HISTORY.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    27825 2023-06-23 06:58:17.713812 switch_api-0.4.6b2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      590 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-06-23 06:58:17.713812 switch_api-0.4.6b2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1352 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.705812 switch_api-0.4.6b2/switch_api/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1459 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.705812 switch_api-0.4.6b2/switch_api/_authentication/
+-rw-r--r--   0 vsts      (1001) docker     (122)      391 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7898 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/_authentication.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.705812 switch_api-0.4.6b2/switch_api/_authentication/_credentials_store/
+-rw-r--r--   0 vsts      (1001) docker     (122)      393 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/_credentials_store/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5851 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/_credentials_store/_credentials_store.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.705812 switch_api-0.4.6b2/switch_api/_authentication/_msal/
+-rw-r--r--   0 vsts      (1001) docker     (122)      361 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/_msal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8752 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_authentication/_msal/_custom_application.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/_utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)      462 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3651 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_utils/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12998 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_utils/_platform.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16873 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/_utils/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/analytics/
+-rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/analytics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9561 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/analytics/analytics.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/cache/
+-rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/cache/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6985 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/cache/cache.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (122)      558 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7724 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/dataset/dataset.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/email/
+-rw-r--r--   0 vsts      (1001) docker     (122)      472 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/email/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4638 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/email/email_sender.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/error_handlers/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2028 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/error_handlers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11845 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/error_handlers/error_handlers.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/extensions/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1038 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/extensions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7519 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/extensions/extensions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1652 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/extensions/field_meta.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2970 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/extensions/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1406 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/extensions/pipeline.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3225 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/initialize.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.709812 switch_api-0.4.6b2/switch_api/integration/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1601 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/integration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11314 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/integration/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26453 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/integration/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    89676 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/integration/integration.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.713812 switch_api-0.4.6b2/switch_api/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3144 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    69447 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/pipeline/automation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    35931 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/pipeline/definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21094 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/pipeline/pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.713812 switch_api-0.4.6b2/switch_api/platform_insights/
+-rw-r--r--   0 vsts      (1001) docker     (122)      542 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/platform_insights/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-06-23 06:57:56.000000 switch_api-0.4.6b2/switch_api/platform_insights/platform_insights.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 06:58:17.705812 switch_api-0.4.6b2/switch_api.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    27825 2023-06-23 06:58:17.000000 switch_api-0.4.6b2/switch_api.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1600 2023-06-23 06:58:17.000000 switch_api-0.4.6b2/switch_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-23 06:58:17.000000 switch_api-0.4.6b2/switch_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       84 2023-06-23 06:58:17.000000 switch_api-0.4.6b2/switch_api.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-06-23 06:58:17.000000 switch_api-0.4.6b2/switch_api.egg-info/top_level.txt
```

### Comparing `switch_api-0.4.6/HISTORY.md` & `switch_api-0.4.6b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,65 @@
-# History
+Metadata-Version: 2.1
+Name: switch_api
+Version: 0.4.6b2
+Summary: A complete package for data ingestion into the Switch Automation Platform.
+Home-page: UNKNOWN
+Author: Switch Automation Pty Ltd.
+License: MIT License
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Other Audience
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Natural Language :: English
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENCE
+License-File: AUTHORS.rst
+
+# Switch Automation library for Python
+This is a package for data ingestion into the Switch Automation software platform. 
+
+You can find out more about the platform on [Switch Automation](https://www.switchautomation.com)
+
+## Getting started
+
+### Prerequisites
+* Python 3.8 or later is required to use this package. 
+* You must have a [Switch Automation user account](https://www.switchautomation.com/our-solution/) to use this package. 
 
-## 0.4.6
+### Install the package
+Install the Switch Automation library for Python with [pip](https://pypi.org/project/pip/):
 
-### Added
+```bash
+pip install switch_api
+```
 
-- Task Priority and Task Framework data feed deployment settings
-  - Task Priority and Task Framework are now available to set when deploying data feeds
-    - Task Priority
-      - Determines the priority of the datafeed tasks when processing.
-      - This equates to how much resources would be alloted to run the task
-      - Available options are: `default`, `standard`, or `advanced`.
-        - set to `advanced` for higher resource when processing data feed task
-      - Defaults to 'default'.
-    - Task Framework
-      - Determines the framework of the datafeed tasks when processing.
-        - 'PythonScriptFramework' for the old task runner engine.
-        - 'TaskInsightsEngine' for the new task running in container apps.
-        - Defaults to 'PythonScriptFramework'
+# History
+
+## 0.4.6b1
+- Will be removed
 
 ## 0.4.5
 
 ### Added
-
 - Email Sender Module
   - Send emails to active users within a Portfolio in Switch Automation Platform
   - Limitations:
     - Emails cannot be sent to users outside of the Portfolio including other users within the platform
     - Maximum of five attachments per email
     - Each attachment has a maximum size of 5mb
   - See function code documentation and usage example below
 - New `generate_filepath` method to provide a filepath where files can be stored
   - Works well with the attachment feature of the Email Sender Module. Store files in the generated filepath of this method and pass into email attachments
   - See function code documentation and usage example below
 
 ### Email Sender Usage
-
 ```python
 import switch_api as sw
 
 sw.email.send_email(
     api_inputs=api_inputs,
     subject='',
     body='',
@@ -47,53 +68,48 @@
     bcc_recipients=[], # Optional
     attachments=['/file/path/to/attachment.csv'], # Optional
     conversation_id='' # Optional
 )
 ```
 
 ### generate_filepath Usage
-
 ```python
 import switch_api as sw
 
 generated_attachment_filepath = sw.generate_filepath(api_inputs=api_inputs, filename='generated_attachment.txt')
 
 # Example of where it could be used
 sw.email.send_email(
     ...
     attachments=[generated_attachment_filepath]
     ...
 )
 ```
 
-### Fixed
 
+### Fixed
 - Issue where `upsert_device_sensors_ext` method was not posting metadata and tag_columns to API
 
 ## 0.3.3
 
 ### Added
-
 - New `upsert_device_sensors_ext` method to the `integration` module.
   - Compared to existing `upsert_device_sensors` following are supported:
     - Installation Code or Installation Id may be provided
       - BUT cannot provide mix of the two, all must have either code or id and not both.
     - DriverClassName
     - DriverDeviceType
     - PropertyName
-
 ### Added Feature - Switch Python Extensions
-
 - Extensions may be used in Task Insights and Switch Guides for code reuse
 - Extensions maybe located in any directory structure within the repo where the usage scripts are located
 - May need to adjust your environment to detect the files if you're not running a project environment
   - Tested on VSCode and PyCharm - contact Switch Support for issues.
 
 #### Extensions Usage
-
 ```python
 import switch_api as sw
 
 # Single import line per extension
 from extensions.my_extension import MyExtension
 
 @sw.extensions.provide(field="some_extension")
@@ -102,35 +118,34 @@
 
 if __name__ == "__main__":
     task = MyTask()
     task.some_extension.do_something()
 ```
 
 #### Extensions Registration
-
 ```python
 import uuid
 import switch_api as sw
 
 class SimpleExtension(sw.extensions.ExtensionTask):
     @property
     def id(self) -> uuid.UUID:
         # Unique ID for the extension.
         # Generate in CLI using:
         #   python -c 'import uuid; print(uuid.uuid4())'
         return '46759cfe-68fa-440c-baa9-c859264368db'
-
+    
     @property
     def description(self) -> str:
         return 'Extension with a simple get_name function.'
-
+    
     @property
     def author(self) -> str:
         return 'Amruth Akoju'
-
+    
     @property
     def version(self) -> str:
         return '1.0.1'
 
     def get_name(self):
         return "Simple Extension"
 
@@ -148,149 +163,136 @@
     # =================================================================
     register = sw.pipeline.Automation.register_task(api_inputs, task)
     print(register)
 
 ```
 
 ### Updated
-
 - get_data now has an optional parameter to return a pandas.DataFrame or JSON
 
 ## 0.2.27
 
 ### Fix
-
 - Issue where Timezone DST Offsets API response of `upsert_timeseries` in `integration` module was handled incorrectly
 
 ## 0.2.26
 
 ### Updated
-
-- Optional `table_def` parameter on `upsert_data`, `append_data`, and `replace_data` in `integration` module
+- Optional `table_def` parameter on `upsert_data`, `append_data`, and `replace_data` in `integration` module 
   - Enable clients to specify the table structure. It will be merged to the inferred table structure.
 - `list_deployments` in Automation module now provides `Settings` and `DriverId` associated with the deployments
 
+
 ## 0.2.25
 
 ### Updated
-
-- Update handling of empty Timezone DST Offsets of `upsert_timeseries` in `integration` module
+- Update handling of empty Timezone DST Offsets of `upsert_timeseries` in `integration` module 
 
 ## 0.2.24
 
 ### Updated
-
 - Fix default `ingestion_mode` parameter value to 'Queue' instead of 'Queued' on `upsert_timeseries` in `integration` module
 
 ## 0.2.23
 
 ### Updated
-
 - Optional `ingestion_mode` parameter on `upsert_timeseries` in `integration` module
   - Include `ingestionMode` in json payload passed to backend API
   - `IngestionMode` type must be `Queue` or `Stream`
   - Default `ingestion_mode` parameter value in `upsert_timeseries` is `Queue`
   - To enable table streaming ingestion, please contact **helpdesk@switchautomation.com** for assistance.
 
 ## 0.2.22
 
 ### Updated
-
 - Optional `ingestion_mode` parameter on `upsert_data` in `integration` module
   - Include `ingestionMode` in json payload passed to backend API
   - `IngestionMode` type must be `Queue` or `Stream`
   - Default `ingestion_mode` parameter value in `upsert_data` is `Queue`
   - To enable table streaming ingestion, please contact **helpdesk@switchautomation.com** for assistance.
 
 ### Fix
-
 - sw.pipeline.logger handlers stacking
 
 ## 0.2.21
 
 ### Updated
-
-- Fix on `get_data` method in `dataset` module
+- Fix on `get_data` method in `dataset` module 
   - Sync parameter structure to backend API for `get_data`
   - List of dict containing properties of `name`, `value`, and `type` items
   - `type` property must be one of subset of the new Literal `DATA_SET_QUERY_PARAMETER_TYPES`
 
 ## 0.2.20
 
 ### Added
-
 - Newly supported Azure Storage Account: GatewayMqttStorage
 - An optional property on QueueTask to specific QueueType
   - Default: DataIngestion
 
 ## 0.2.19
 
 ### Fixed
-
 - Fix on `upsert_timeseries` method in `integration` module
   - Normalized TimestampId and TimestampLocalId seconds
 - Minor fix on `upsert_entities_affected` method in `integration` utils module
   - Prevent upsert entities affected count when data feed file status Id is not valid
 - Minor fix on `get_metadata_keys` method in `integration` helper module
   - Fix for issue when a portfolio does not contain any values in the ApiMetadata table
 
+
 ## 0.2.18
 
 ### Added
-
 - Added new `is_specific_timezone` parameter in `upsert_timeseries` method of `integration` module
-
-  - Accepts a timezone name as the specific timezone used by the source data.
+  - Accepts a timezone name as the specific timezone used by the source data. 
   - Can either be of type str or bool and defaults to the value of False.
   - Cannot have value if 'is_local_time' is set to True.
   - Retrieve list of available timezones using 'get_timezones' method in `integration` module
+  
 
-    | is_specific_timezone | is_local_time | Description                                                                                                                                                     |
-    | -------------------- | ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-    | False                | False         | Datetimes in provided data is already in UTC and should remain as the value of Timestamp. The TimestampLocal (conversion to site-local Timezone) is calculated. |
-    | False                | True          | Datetimes in provided data is already in the site-local Timezone & should be used to set the value of the TimestampLocal field. The UTC Timestamp is calculated |
-    | Has Value            | True          | NOT ALLOWED                                                                                                                                                     |
-    | Has Value            | False         | Both Timestamp and TimestampLocal fields will are calculated. Datetime is converted to UTC then to Local.                                                       |
-    | True                 |               | NOT ALLOWED                                                                                                                                                     |
-    | '' (empty string)    |               | NOT ALLOWED                                                                                                                                                     |
+    | is_specific_timezone  | is_local_time | Description |
+    | --------------------- | -------- | ----------- |
+    | False  | False  | Datetimes in provided data is already in UTC and should remain as the value of Timestamp. The TimestampLocal (conversion to site-local Timezone) is calculated. |
+    | False  | True  | Datetimes in provided data is already in the site-local Timezone & should be used to set the value of the TimestampLocal field. The UTC Timestamp is calculated |
+    | Has Value | True  | NOT ALLOWED |
+    | Has Value | False  | Both Timestamp and TimestampLocal fields will are calculated. Datetime is converted to UTC then to Local. |
+    | True  |   | NOT ALLOWED |
+    | '' (empty string)  |   | NOT ALLOWED |
+  
 
 ### Fixed
-
-- Minor fix on `upsert_tags` and `upsert_device_metadata` methods in `integration` module
+- Minor fix on `upsert_tags` and `upsert_device_metadata` methods in `integration` module 
   - List of required_columns was incorrectly being updated when these functions were called
 - Minor fix on `upsert_event_work_order_id` method in `integration` module when attempting to update status of an Event
 
 ### Updated
-
 - Update on `DiscoveryIntegrationInput` namedtuple - added `job_id`
 - Update `upsert_discovered_records` method required columns in `integration` module
   - add required `JobId` column for Data Frame parameter
 
-## 0.2.17
 
+## 0.2.17
 ### Fixed
-
 - Fix on `upsert_timeseries()` method in `integration` module for duplicate records in ingestion files
   - records whose Timestamp falls in the exact DST start created 2 records with identical values but different TimestampLocal
     - one has the TimestampLocal of a DST and the other does not
 
 ### Updated
-
 - Update on `get_sites()` method in `integration` module for `InstallationCode` column
   - when the `InstallationCode' value is null in the database it returns an empty string
   - `InstallationCode` column is explicity casted to dtype 'str'
 
-## 0.2.16
 
+## 0.2.16
 ### Added
 
 - Added new 5 minute interval for `EXPECTED_DELIVERY` Literal in `automation` module
   - support for data feed deployments Email, FTP, Upload, and Timer
   - usage: expected_delivery='5min'
-
+  
 ### Fixed
 
 - Minor fix on `upsert_timeseries()` method using `data_feed_file_status_id` parameter in `integration` module.
   - `data_feed_file_status_id` parameter value now synced between process records and ingestion files when supplied
 
 ### Updated
 
@@ -789,7 +791,9 @@
 - `kql`
 
 Removed the `name_as_filename` and `treat_as_timeseries` parameter from the following functions:
 
 - `switch.integration.replace_data()`
 - `switch.integration.append_data()`
 - `switch.integration.upload_data()`
+
+
```

### Comparing `switch_api-0.4.6/LICENCE` & `switch_api-0.4.6b2/LICENCE`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/PKG-INFO` & `switch_api-0.4.6b2/switch_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: switch_api
-Version: 0.4.6
+Name: switch-api
+Version: 0.4.6b2
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,49 +34,32 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
-## 0.4.6
-
-### Added
-
-- Task Priority and Task Framework data feed deployment settings
-  - Task Priority and Task Framework are now available to set when deploying data feeds
-    - Task Priority
-      - Determines the priority of the datafeed tasks when processing.
-      - This equates to how much resources would be alloted to run the task
-      - Available options are: `default`, `standard`, or `advanced`.
-        - set to `advanced` for higher resource when processing data feed task
-      - Defaults to 'default'.
-    - Task Framework
-      - Determines the framework of the datafeed tasks when processing.
-        - 'PythonScriptFramework' for the old task runner engine.
-        - 'TaskInsightsEngine' for the new task running in container apps.
-        - Defaults to 'PythonScriptFramework'
+## 0.4.6b1
+- Will be removed
 
 ## 0.4.5
 
 ### Added
-
 - Email Sender Module
   - Send emails to active users within a Portfolio in Switch Automation Platform
   - Limitations:
     - Emails cannot be sent to users outside of the Portfolio including other users within the platform
     - Maximum of five attachments per email
     - Each attachment has a maximum size of 5mb
   - See function code documentation and usage example below
 - New `generate_filepath` method to provide a filepath where files can be stored
   - Works well with the attachment feature of the Email Sender Module. Store files in the generated filepath of this method and pass into email attachments
   - See function code documentation and usage example below
 
 ### Email Sender Usage
-
 ```python
 import switch_api as sw
 
 sw.email.send_email(
     api_inputs=api_inputs,
     subject='',
     body='',
@@ -85,53 +68,48 @@
     bcc_recipients=[], # Optional
     attachments=['/file/path/to/attachment.csv'], # Optional
     conversation_id='' # Optional
 )
 ```
 
 ### generate_filepath Usage
-
 ```python
 import switch_api as sw
 
 generated_attachment_filepath = sw.generate_filepath(api_inputs=api_inputs, filename='generated_attachment.txt')
 
 # Example of where it could be used
 sw.email.send_email(
     ...
     attachments=[generated_attachment_filepath]
     ...
 )
 ```
 
-### Fixed
 
+### Fixed
 - Issue where `upsert_device_sensors_ext` method was not posting metadata and tag_columns to API
 
 ## 0.3.3
 
 ### Added
-
 - New `upsert_device_sensors_ext` method to the `integration` module.
   - Compared to existing `upsert_device_sensors` following are supported:
     - Installation Code or Installation Id may be provided
       - BUT cannot provide mix of the two, all must have either code or id and not both.
     - DriverClassName
     - DriverDeviceType
     - PropertyName
-
 ### Added Feature - Switch Python Extensions
-
 - Extensions may be used in Task Insights and Switch Guides for code reuse
 - Extensions maybe located in any directory structure within the repo where the usage scripts are located
 - May need to adjust your environment to detect the files if you're not running a project environment
   - Tested on VSCode and PyCharm - contact Switch Support for issues.
 
 #### Extensions Usage
-
 ```python
 import switch_api as sw
 
 # Single import line per extension
 from extensions.my_extension import MyExtension
 
 @sw.extensions.provide(field="some_extension")
@@ -140,35 +118,34 @@
 
 if __name__ == "__main__":
     task = MyTask()
     task.some_extension.do_something()
 ```
 
 #### Extensions Registration
-
 ```python
 import uuid
 import switch_api as sw
 
 class SimpleExtension(sw.extensions.ExtensionTask):
     @property
     def id(self) -> uuid.UUID:
         # Unique ID for the extension.
         # Generate in CLI using:
         #   python -c 'import uuid; print(uuid.uuid4())'
         return '46759cfe-68fa-440c-baa9-c859264368db'
-
+    
     @property
     def description(self) -> str:
         return 'Extension with a simple get_name function.'
-
+    
     @property
     def author(self) -> str:
         return 'Amruth Akoju'
-
+    
     @property
     def version(self) -> str:
         return '1.0.1'
 
     def get_name(self):
         return "Simple Extension"
 
@@ -186,149 +163,136 @@
     # =================================================================
     register = sw.pipeline.Automation.register_task(api_inputs, task)
     print(register)
 
 ```
 
 ### Updated
-
 - get_data now has an optional parameter to return a pandas.DataFrame or JSON
 
 ## 0.2.27
 
 ### Fix
-
 - Issue where Timezone DST Offsets API response of `upsert_timeseries` in `integration` module was handled incorrectly
 
 ## 0.2.26
 
 ### Updated
-
-- Optional `table_def` parameter on `upsert_data`, `append_data`, and `replace_data` in `integration` module
+- Optional `table_def` parameter on `upsert_data`, `append_data`, and `replace_data` in `integration` module 
   - Enable clients to specify the table structure. It will be merged to the inferred table structure.
 - `list_deployments` in Automation module now provides `Settings` and `DriverId` associated with the deployments
 
+
 ## 0.2.25
 
 ### Updated
-
-- Update handling of empty Timezone DST Offsets of `upsert_timeseries` in `integration` module
+- Update handling of empty Timezone DST Offsets of `upsert_timeseries` in `integration` module 
 
 ## 0.2.24
 
 ### Updated
-
 - Fix default `ingestion_mode` parameter value to 'Queue' instead of 'Queued' on `upsert_timeseries` in `integration` module
 
 ## 0.2.23
 
 ### Updated
-
 - Optional `ingestion_mode` parameter on `upsert_timeseries` in `integration` module
   - Include `ingestionMode` in json payload passed to backend API
   - `IngestionMode` type must be `Queue` or `Stream`
   - Default `ingestion_mode` parameter value in `upsert_timeseries` is `Queue`
   - To enable table streaming ingestion, please contact **helpdesk@switchautomation.com** for assistance.
 
 ## 0.2.22
 
 ### Updated
-
 - Optional `ingestion_mode` parameter on `upsert_data` in `integration` module
   - Include `ingestionMode` in json payload passed to backend API
   - `IngestionMode` type must be `Queue` or `Stream`
   - Default `ingestion_mode` parameter value in `upsert_data` is `Queue`
   - To enable table streaming ingestion, please contact **helpdesk@switchautomation.com** for assistance.
 
 ### Fix
-
 - sw.pipeline.logger handlers stacking
 
 ## 0.2.21
 
 ### Updated
-
-- Fix on `get_data` method in `dataset` module
+- Fix on `get_data` method in `dataset` module 
   - Sync parameter structure to backend API for `get_data`
   - List of dict containing properties of `name`, `value`, and `type` items
   - `type` property must be one of subset of the new Literal `DATA_SET_QUERY_PARAMETER_TYPES`
 
 ## 0.2.20
 
 ### Added
-
 - Newly supported Azure Storage Account: GatewayMqttStorage
 - An optional property on QueueTask to specific QueueType
   - Default: DataIngestion
 
 ## 0.2.19
 
 ### Fixed
-
 - Fix on `upsert_timeseries` method in `integration` module
   - Normalized TimestampId and TimestampLocalId seconds
 - Minor fix on `upsert_entities_affected` method in `integration` utils module
   - Prevent upsert entities affected count when data feed file status Id is not valid
 - Minor fix on `get_metadata_keys` method in `integration` helper module
   - Fix for issue when a portfolio does not contain any values in the ApiMetadata table
 
+
 ## 0.2.18
 
 ### Added
-
 - Added new `is_specific_timezone` parameter in `upsert_timeseries` method of `integration` module
-
-  - Accepts a timezone name as the specific timezone used by the source data.
+  - Accepts a timezone name as the specific timezone used by the source data. 
   - Can either be of type str or bool and defaults to the value of False.
   - Cannot have value if 'is_local_time' is set to True.
   - Retrieve list of available timezones using 'get_timezones' method in `integration` module
+  
 
-    | is_specific_timezone | is_local_time | Description                                                                                                                                                     |
-    | -------------------- | ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-    | False                | False         | Datetimes in provided data is already in UTC and should remain as the value of Timestamp. The TimestampLocal (conversion to site-local Timezone) is calculated. |
-    | False                | True          | Datetimes in provided data is already in the site-local Timezone & should be used to set the value of the TimestampLocal field. The UTC Timestamp is calculated |
-    | Has Value            | True          | NOT ALLOWED                                                                                                                                                     |
-    | Has Value            | False         | Both Timestamp and TimestampLocal fields will are calculated. Datetime is converted to UTC then to Local.                                                       |
-    | True                 |               | NOT ALLOWED                                                                                                                                                     |
-    | '' (empty string)    |               | NOT ALLOWED                                                                                                                                                     |
+    | is_specific_timezone  | is_local_time | Description |
+    | --------------------- | -------- | ----------- |
+    | False  | False  | Datetimes in provided data is already in UTC and should remain as the value of Timestamp. The TimestampLocal (conversion to site-local Timezone) is calculated. |
+    | False  | True  | Datetimes in provided data is already in the site-local Timezone & should be used to set the value of the TimestampLocal field. The UTC Timestamp is calculated |
+    | Has Value | True  | NOT ALLOWED |
+    | Has Value | False  | Both Timestamp and TimestampLocal fields will are calculated. Datetime is converted to UTC then to Local. |
+    | True  |   | NOT ALLOWED |
+    | '' (empty string)  |   | NOT ALLOWED |
+  
 
 ### Fixed
-
-- Minor fix on `upsert_tags` and `upsert_device_metadata` methods in `integration` module
+- Minor fix on `upsert_tags` and `upsert_device_metadata` methods in `integration` module 
   - List of required_columns was incorrectly being updated when these functions were called
 - Minor fix on `upsert_event_work_order_id` method in `integration` module when attempting to update status of an Event
 
 ### Updated
-
 - Update on `DiscoveryIntegrationInput` namedtuple - added `job_id`
 - Update `upsert_discovered_records` method required columns in `integration` module
   - add required `JobId` column for Data Frame parameter
 
-## 0.2.17
 
+## 0.2.17
 ### Fixed
-
 - Fix on `upsert_timeseries()` method in `integration` module for duplicate records in ingestion files
   - records whose Timestamp falls in the exact DST start created 2 records with identical values but different TimestampLocal
     - one has the TimestampLocal of a DST and the other does not
 
 ### Updated
-
 - Update on `get_sites()` method in `integration` module for `InstallationCode` column
   - when the `InstallationCode' value is null in the database it returns an empty string
   - `InstallationCode` column is explicity casted to dtype 'str'
 
-## 0.2.16
 
+## 0.2.16
 ### Added
 
 - Added new 5 minute interval for `EXPECTED_DELIVERY` Literal in `automation` module
   - support for data feed deployments Email, FTP, Upload, and Timer
   - usage: expected_delivery='5min'
-
+  
 ### Fixed
 
 - Minor fix on `upsert_timeseries()` method using `data_feed_file_status_id` parameter in `integration` module.
   - `data_feed_file_status_id` parameter value now synced between process records and ingestion files when supplied
 
 ### Updated
```

### Comparing `switch_api-0.4.6/README.md` & `switch_api-0.4.6b2/README.md`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/setup.py` & `switch_api-0.4.6b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 setup(
     author="Switch Automation Pty Ltd.",
     description="A complete package for data ingestion into the Switch Automation Platform.",
     long_description=open('README.md', 'r').read() + '\n\n' + open('HISTORY.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     name="switch_api",
-    version="0.4.6",
+    version="0.4.6-beta2",
     packages=find_packages(include=["switch_api", "switch_api.*"]),
     install_requires=['pandas', 'requests', 'azure-storage-blob', 'pandera[io]==0.7.1', 'azure-servicebus', 'msal>=1.11.0'],
     python_requires=">=3.8.0",
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         "License :: OSI Approved :: MIT License",
         'Intended Audience :: Other Audience',
```

### Comparing `switch_api-0.4.6/switch_api/__init__.py` & `switch_api-0.4.6b2/switch_api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 # _ch.setLevel(logging.INFO)  # sets the handler info
 # _ch.setFormatter(logging.Formatter(INFOFORMATTER))  # sets the handler formatting
 #
 # # adds the handler to the global variable: log
 # log.addHandler(_ch)
 # https://dev.to/joaomcteixeira/setting-up-python-logging-for-a-library-app-6ml
 
-__version__ = "0.4.6"
+__version__ = "0.4.6-beta2"
```

### Comparing `switch_api-0.4.6/switch_api/_authentication/_authentication.py` & `switch_api-0.4.6b2/switch_api/_authentication/_authentication.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/_authentication/_credentials_store/_credentials_store.py` & `switch_api-0.4.6b2/switch_api/_authentication/_credentials_store/_credentials_store.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/_authentication/_msal/_custom_application.py` & `switch_api-0.4.6b2/switch_api/_authentication/_msal/_custom_application.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/_utils/_constants.py` & `switch_api-0.4.6b2/switch_api/_utils/_constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,11 +71,7 @@
 
 CACHE_SCOPE = Literal['Portfolio', 'Task', 'DataFeed']
 TAG_LEVEL = Literal['Site', 'Device', 'Sensor']
 
 DATA_SET_QUERY_PARAMETER_TYPES = Literal['String', 'Number', 'DateTime', 'Keyword', 'Boolean', 'NumberArray', 'StringArray']
 
 ADX_TABLE_DEF_TYPES = Literal['object', 'dynamic', 'int32', 'int64', 'float32', 'float64', 'datetime', 'string']
-
-TASK_PRIORITY = Literal['default', 'standard', 'advanced']
-
-TASK_FRAMEWORK = Literal['PythonScriptFramework', 'TaskInsightsEngine']
```

### Comparing `switch_api-0.4.6/switch_api/_utils/_platform.py` & `switch_api-0.4.6b2/switch_api/_utils/_platform.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/_utils/_utils.py` & `switch_api-0.4.6b2/switch_api/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/analytics/__init__.py` & `switch_api-0.4.6b2/switch_api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/analytics/analytics.py` & `switch_api-0.4.6b2/switch_api/analytics/analytics.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/cache/cache.py` & `switch_api-0.4.6b2/switch_api/cache/cache.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/dataset/__init__.py` & `switch_api-0.4.6b2/switch_api/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/dataset/dataset.py` & `switch_api-0.4.6b2/switch_api/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/email/email_sender.py` & `switch_api-0.4.6b2/switch_api/email/email_sender.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/error_handlers/__init__.py` & `switch_api-0.4.6b2/switch_api/error_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/error_handlers/error_handlers.py` & `switch_api-0.4.6b2/switch_api/error_handlers/error_handlers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/extensions/__init__.py` & `switch_api-0.4.6b2/switch_api/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/extensions/extensions.py` & `switch_api-0.4.6b2/switch_api/extensions/extensions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/extensions/field_meta.py` & `switch_api-0.4.6b2/switch_api/extensions/field_meta.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/extensions/helpers.py` & `switch_api-0.4.6b2/switch_api/extensions/helpers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/extensions/pipeline.py` & `switch_api-0.4.6b2/switch_api/extensions/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/initialize.py` & `switch_api-0.4.6b2/switch_api/initialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,18 +35,20 @@
 
     Returns
     -------
     ApiInputs
         Returns the ApiInputs namedtuple that is required as an input to other functions.
     """
 
+    logger.info('My demo change')
+
     try:
         uuid.UUID(api_project_id)
     except:
-        sw.logger.error(f"Invalid value provided '{api_project_id}'- please provide a valid api_project_id. ")
+        logger.error(f"Invalid value provided '{api_project_id}'- please provide a valid api_project_id. ")
         return False
 
     creds = get_switch_credentials(environment, api_project_id)
 
     logger.info("Successfully initialized.")
     api_base_url = f"https://{creds.api_endpoint}/api/1.0"
     # api_base_url = f"https://localhost:5001/api/1.0"
```

### Comparing `switch_api-0.4.6/switch_api/integration/__init__.py` & `switch_api-0.4.6b2/switch_api/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/integration/_utils.py` & `switch_api-0.4.6b2/switch_api/integration/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/integration/helpers.py` & `switch_api-0.4.6b2/switch_api/integration/helpers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/integration/integration.py` & `switch_api-0.4.6b2/switch_api/integration/integration.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/pipeline/__init__.py` & `switch_api-0.4.6b2/switch_api/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/pipeline/automation.py` & `switch_api-0.4.6b2/switch_api/pipeline/automation.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import logging
 import sys
 import uuid
 from io import StringIO
 from azure.servicebus import ServiceBusClient, ServiceBusReceiveMode # , ServiceBusMessage
 from .._utils._utils import _is_valid_regex, ApiInputs, _column_name_cap, DataFeedFileProcessOutput
 from .._utils._constants import (argus_prefix, EXPECTED_DELIVERY, MAPPING_ENTITIES,
-                                 QUEUE_NAME, ERROR_TYPE, SCHEDULE_TIMEZONE, DEPLOY_TYPE, TASK_PRIORITY, TASK_FRAMEWORK)
+                                 QUEUE_NAME, ERROR_TYPE, SCHEDULE_TIMEZONE, DEPLOY_TYPE)
 from .._utils._platform import _get_ingestion_service_bus_connection_string
 from .pipeline import (Task, QueueTask, IntegrationTask, LogicModuleTask, AnalyticsTask, EventWorkOrderTask,
                        DiscoverableIntegrationTask)
 from ..extensions import ExtensionTask, replace_extensions_imports, has_extensions_support
 from .definitions import (IntegrationDeviceDefinition, EventWorkOrderFieldDefinition, AnalyticsSettings,
                           IntegrationSettings, IntegrationDeviceConfigPropertyDefinition)
 
@@ -524,15 +524,15 @@
 
     @staticmethod
     def deploy_as_email_data_feed(task: Union[Task, IntegrationTask, DiscoverableIntegrationTask, QueueTask,
                                               AnalyticsTask, LogicModuleTask, EventWorkOrderTask],
                                   api_inputs: ApiInputs, data_feed_id: uuid.UUID,
                                   expected_delivery: EXPECTED_DELIVERY, email_subject_regex: str,
                                   email_address_domain: str, queue_name: QUEUE_NAME = 'task',
-                                  data_feed_name: str = None, task_priority: TASK_PRIORITY = 'default', task_framework: TASK_FRAMEWORK = 'PythonScriptFramework'):
+                                  data_feed_name: str = None):
         """Deploy task as an email data feed.
 
         Deploys the created `task` as an email data feed. This allows the driver to ingest data sent via email. The
         data must be sent to data@switchautomation.com to be processed. If it is sent to another email address, the task
         will not be run.
 
         Parameters
@@ -554,21 +554,15 @@
             file(s) for this data feed to the Switch Automation Platform is sender@test.com, the string that should be
             passed to this parameter is "test.com".
         queue_name : QUEUE_NAME, Optional
             The name of queue (Default value = 'task').
         data_feed_name : str, Optional
             The name of the data feed (to be displayed in Task Insights UI). If not provided, the API will automatically
             default to using the task.name property of the `task` passed to function.
-        task_priority: TASK_PRIORITY
-            Determines the priority of the datafeed tasks when processing. This equates to how much resources would be alloted
-            to run the task - 'default`, 'standard', or 'advanced'. Defaults to 'default'.
-        task_framework: TASK_FRAMEWORK
-            Determines the framework of the datafeed tasks when processing.
-            'PythonScriptFramework' for the old task runner engine.
-            'TaskInsightsEngine' for the new task running in container apps.
+
 
         Returns
         -------
         df : pandas.DataFrame
             Dataframe containing the details of the deployed email data feed.
 
         """
@@ -605,39 +599,24 @@
                          'EXPECTED_DELIVERY literal: %s', EXPECTED_DELIVERY.__args__)
             return pandas.DataFrame()
 
         if not set([queue_name]).issubset(set(QUEUE_NAME.__args__)):
             logger.error('queue_name parameter must be set to one of the allowed values defined by the '
                          'QUEUE_NAME literal: %s', QUEUE_NAME.__args__)
             return pandas.DataFrame()
-        
-        if not set([task_framework]).issubset(set(TASK_FRAMEWORK.__args__)):
-            logger.error('task_framework parameter must be set to one of the allowed values defined by the '
-                         'TASK_FRAMEWORK literal: %s', TASK_FRAMEWORK.__args__)
-            return pandas.DataFrame()
-        
-        if not set([task_priority]).issubset(set(TASK_PRIORITY.__args__)):
-            logger.error('task_priority parameter must be set to one of the allowed values defined by the '
-                         'TASK_PRIORITY literal: %s', TASK_PRIORITY.__args__)
-            return pandas.DataFrame()
-        
-        logger.info('Task Framework is "%s"', str(task_framework))
-        logger.info('Task Priotiy is "%s"', str(task_priority))
 
         inbox_container = "data-exchange"
         payload = {
             "dataFeedId": str(data_feed_id),
             "driverId": str(task.id),
             "name": data_feed_name,
             "feedType": ",".join(task.mapping_entities),
             "expectedDelivery": expected_delivery,
             "sourceType": "Email",
             "queueName": queue_name,
-            "taskFramework": task_framework,
-            "taskPriority": task_priority,
             "email": {
                 "emailAddressDomain": email_address_domain,
                 "emailSubjectRegex": email_subject_regex,
                 "container": inbox_container
             }
         }
 
@@ -661,15 +640,15 @@
         return df
 
     @staticmethod
     def deploy_as_ftp_data_feed(task: Union[Task, IntegrationTask, DiscoverableIntegrationTask, QueueTask,
                                             AnalyticsTask, LogicModuleTask, EventWorkOrderTask],
                                 api_inputs: ApiInputs, data_feed_id: uuid.UUID, expected_delivery: EXPECTED_DELIVERY,
                                 ftp_user_name: str, ftp_password: str, queue_name: QUEUE_NAME = 'task',
-                                data_feed_name: str = None, task_priority: TASK_PRIORITY = 'default', task_framework: TASK_FRAMEWORK = 'PythonScriptFramework'):
+                                data_feed_name: str = None):
         """Deploy the custom driver as an FTP data feed
 
         Deploys the custom driver to receive data via an FTP data feed. Sets the `ftp_user_name` & `ftp_password` and
         the `expected_delivery` of the file.
 
         Parameters
         ----------
@@ -687,21 +666,14 @@
             The password to be used by the ftp service for the given `ftp_user_name` to authenticate delivery of the
             data feed.
         queue_name : QUEUE_NAME, default = 'task'
             The queue name (Default value = 'task').
         data_feed_name : str, Optional
             The name of the data feed (to be displayed in Task Insights UI). If not provided, will default to the
             task name.
-        task_priority: TASK_PRIORITY
-            Determines the priority of the datafeed tasks when processing. This equates to how much resources would be alloted
-            to run the task - 'default`, 'standard', or 'advanced'. Defaults to 'default'.
-        task_framework: TASK_FRAMEWORK
-            Determines the framework of the datafeed tasks when processing.
-            'PythonScriptFramework' for the old task runner engine.
-            'TaskInsightsEngine' for the new task running in container apps.
 
         Returns
         -------
         df : pandas.DataFrame
             Dataframe containing the details of the deployed ftp data feed.
 
         """
@@ -725,40 +697,26 @@
             return pandas.DataFrame()
 
         if not set([queue_name]).issubset(set(QUEUE_NAME.__args__)):
             logger.error('queue_name parameter must be set to one of the allowed values defined by the '
                          'QUEUE_NAME literal: %s', QUEUE_NAME.__args__)
             return pandas.DataFrame()
 
-        if not set([task_framework]).issubset(set(TASK_FRAMEWORK.__args__)):
-            logger.error('task_framework parameter must be set to one of the allowed values defined by the '
-                         'TASK_FRAMEWORK literal: %s', TASK_FRAMEWORK.__args__)
-            return pandas.DataFrame()
-        
-        if not set([task_priority]).issubset(set(TASK_PRIORITY.__args__)):
-            logger.error('task_priority parameter must be set to one of the allowed values defined by the '
-                         'TASK_PRIORITY literal: %s', TASK_PRIORITY.__args__)
-            return pandas.DataFrame()
-
         logger.info('Deploy %s (%s) as a data feed for ApiProjectID: %s', type(task).__name__, str(task.id),
                     api_inputs.api_project_id)
-        logger.info('Task Framework is "%s"', str(task_framework))
-        logger.info('Task Priotiy is "%s"', str(task_priority))
 
         inbox_container = "data-exchange"
         payload = {
             "dataFeedId": str(data_feed_id),
             "driverId": str(task.id),
             "name": data_feed_name,
             "feedType": ",".join(task.mapping_entities),
             "expectedDelivery": expected_delivery,
             "sourceType": "Ftp",
             "queueName": queue_name,
-            "taskFramework": task_framework,
-            "taskPriority": task_priority,
             "ftp": {
                 "ftpUserName": ftp_user_name,
                 "ftpPassword": ftp_password,
                 "container": inbox_container
             }
         }
 
@@ -781,16 +739,15 @@
 
         return df
 
     @staticmethod
     def deploy_as_upload_data_feed(task: Union[Task, IntegrationTask, DiscoverableIntegrationTask, QueueTask,
                                                AnalyticsTask, LogicModuleTask, EventWorkOrderTask],
                                    api_inputs: ApiInputs, data_feed_id: uuid.UUID, expected_delivery: EXPECTED_DELIVERY,
-                                   queue_name: QUEUE_NAME = 'task', data_feed_name: str = None, task_priority: TASK_PRIORITY = 'default', 
-                                   task_framework: TASK_FRAMEWORK = 'PythonScriptFramework'):
+                                   queue_name: QUEUE_NAME = 'task', data_feed_name: str = None):
         """Deploy the custom driver as a REST API end point Datafeed.
 
         To upload a file to the deployed data feed, use the UploadUrl from the response dataframe (with request type
         POST) with the following two headers:
 
         - 'Ocp-Apim-Subscription-Key' - set to the value of ``api_inputs.subscription_key``
         - 'Authorization' - set to the value 'Bearer ``api_inputs.bearer_token``'
@@ -817,21 +774,14 @@
         expected_delivery : EXPECTED_DELIVERY
             The expected delivery frequency of the data.
         queue_name : QUEUE_NAME, optional
             The queue name (Default value = 'task').
         data_feed_name : str, Optional
             The name of the data feed (to be displayed in Task Insights UI). If not provided, will default to the
             task name.
-        task_priority: TASK_PRIORITY
-            Determines the priority of the datafeed tasks when processing. This equates to how much resources would be alloted
-            to run the task - 'default`, 'standard', or 'advanced'. Defaults to 'default'.
-        task_framework: TASK_FRAMEWORK
-            Determines the framework of the datafeed tasks when processing.
-            'PythonScriptFramework' for the old task runner engine.
-            'TaskInsightsEngine' for the new task running in container apps.
 
         Returns
         -------
         df : pandas.DataFrame
             Dataframe containing the details of the deployed https endpoint data feed.
 
         """
@@ -855,39 +805,25 @@
             return pandas.DataFrame()
 
         if not set([queue_name]).issubset(set(QUEUE_NAME.__args__)):
             logger.error('queue_name parameter must be set to one of the allowed values defined by the '
                          'QUEUE_NAME literal: %s', QUEUE_NAME.__args__)
             return pandas.DataFrame()
 
-        if not set([task_framework]).issubset(set(TASK_FRAMEWORK.__args__)):
-            logger.error('task_framework parameter must be set to one of the allowed values defined by the '
-                         'TASK_FRAMEWORK literal: %s', TASK_FRAMEWORK.__args__)
-            return pandas.DataFrame()
-        
-        if not set([task_priority]).issubset(set(TASK_PRIORITY.__args__)):
-            logger.error('task_priority parameter must be set to one of the allowed values defined by the '
-                         'TASK_PRIORITY literal: %s', TASK_PRIORITY.__args__)
-            return pandas.DataFrame()
-
         logger.info('Deploy %s (%s) as a data feed for ApiProjectID: %s', type(task).__name__, str(task.id),
                     api_inputs.api_project_id)
-        logger.info('Task Framework is "%s"', str(task_framework))
-        logger.info('Task Priotiy is "%s"', str(task_priority))
 
         payload = {
             "dataFeedId": str(data_feed_id),
             "driverId": str(task.id),
             "name": data_feed_name,
             "feedType": ",".join(task.mapping_entities),
             "expectedDelivery": expected_delivery,
             "sourceType": "Upload",
             "queueName": queue_name,
-            "taskFramework": task_framework,
-            "taskPriority": task_priority,
             "upload": {
                 "placeholder": ""
             },
         }
 
         url = f"{api_inputs.api_projects_endpoint}/{api_inputs.api_project_id}/data-ingestion/tasks/deployment"
 
@@ -910,15 +846,15 @@
 
     @staticmethod
     def deploy_on_timer(task: Union[Task, IntegrationTask, DiscoverableIntegrationTask, QueueTask,
                                     AnalyticsTask, LogicModuleTask, EventWorkOrderTask],
                         api_inputs: ApiInputs, data_feed_id: uuid.UUID, expected_delivery: EXPECTED_DELIVERY,
                         cron_schedule: str, queue_name: QUEUE_NAME = "task", settings: dict = None,
                         schedule_timezone: SCHEDULE_TIMEZONE = 'Local', timezone_offset_minutes: int = None,
-                        data_feed_name: str = None, task_priority: TASK_PRIORITY = 'default', task_framework: TASK_FRAMEWORK = 'PythonScriptFramework'):
+                        data_feed_name: str = None):
         """Deploy driver to run on timer.
 
         Parameters
         ----------
         task : Task
             The custom driver class created from the Abstract Base Class `Task`.
         api_inputs : ApiInputs
@@ -939,21 +875,14 @@
             Whether the ``cron_schedule`` should be applied based on Local or Utc timezone. If set to `Local`, this is
             taken as the timezone of the western-most site in the given portfolio (Default value = 'Local').
         timezone_offset_minutes: int, Optional
             Timezone offset in minutes (from UTC) to be used when applying the ``cron_schedule`` (Default value = None).
         data_feed_name : str, Optional
             The name of the data feed (to be displayed in Task Insights UI). If not provided, will default to the
             task name.
-        task_priority: TASK_PRIORITY
-            Determines the priority of the datafeed tasks when processing. This equates to how much resources would be alloted
-            to run the task - 'default`, 'standard', or 'advanced'. Defaults to 'default'.
-        task_framework: TASK_FRAMEWORK
-            Determines the framework of the datafeed tasks when processing.
-            'PythonScriptFramework' for the old task runner engine.
-            'TaskInsightsEngine' for the new task running in container apps.
 
         Returns
         -------
         pandas.Dataframe
             A dataframe containing the details of the deployed data feed.
 
         """
@@ -1017,41 +946,27 @@
         #                 missing_optional_keys
         #             else:
         #                 missing_optional_keys.append(missing_keys[j])
         #                 missing_required_keys
         #         if len(missing_required_keys) > 0 and len(missing_optional_keys) == 0:
         #             loggger.error(f"settings parameter is missing the following required key(s): {missing_required_keys}.")
 
-        if not set([task_framework]).issubset(set(TASK_FRAMEWORK.__args__)):
-            logger.error('task_framework parameter must be set to one of the allowed values defined by the '
-                         'TASK_FRAMEWORK literal: %s', TASK_FRAMEWORK.__args__)
-            return pandas.DataFrame()
-        
-        if not set([task_priority]).issubset(set(TASK_PRIORITY.__args__)):
-            logger.error('task_priority parameter must be set to one of the allowed values defined by the '
-                         'TASK_PRIORITY literal: %s', TASK_PRIORITY.__args__)
-            return pandas.DataFrame()
-
         logger.info('Deploy %s (%s) on timer for ApiProjectID: %s and schedule: %s.', type(task).__name__,
                     str(task.id), api_inputs.api_project_id, cron_schedule)
         logger.info('Feed Type is %s', str(task.mapping_entities))
-        logger.info('Task Framework is "%s"', str(task_framework))
-        logger.info('Task Priotiy is "%s"', str(task_priority))
         logger.info('Settings to be passed to the driver on start are: %s', str(settings))
 
         payload = {
             "dataFeedId": str(data_feed_id),
             "driverId": str(task.id),
             "name": data_feed_name,
             "feedType": ",".join(task.mapping_entities),
             "expectedDelivery": expected_delivery,
             "sourceType": "Timer",
             "queueName": queue_name,
-            "taskFramework": task_framework,
-            "taskPriority": task_priority,
             "timer": {
                 "cronSchedule": cron_schedule,
                 "timezoneOffsetMinutes": timezone_offset_minutes,
                 "scheduleTimezone": schedule_timezone
             },
             "settings": settings
         }
```

### Comparing `switch_api-0.4.6/switch_api/pipeline/definitions.py` & `switch_api-0.4.6b2/switch_api/pipeline/definitions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/pipeline/pipeline.py` & `switch_api-0.4.6b2/switch_api/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/platform_insights/__init__.py` & `switch_api-0.4.6b2/switch_api/platform_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api/platform_insights/platform_insights.py` & `switch_api-0.4.6b2/switch_api/platform_insights/platform_insights.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.4.6/switch_api.egg-info/PKG-INFO` & `switch_api-0.4.6b2/HISTORY.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,27 @@
-Metadata-Version: 2.1
-Name: switch-api
-Version: 0.4.6
-Summary: A complete package for data ingestion into the Switch Automation Platform.
-Home-page: UNKNOWN
-Author: Switch Automation Pty Ltd.
-License: MIT License
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Other Audience
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Natural Language :: English
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENCE
-License-File: AUTHORS.rst
-
-# Switch Automation library for Python
-This is a package for data ingestion into the Switch Automation software platform. 
-
-You can find out more about the platform on [Switch Automation](https://www.switchautomation.com)
-
-## Getting started
-
-### Prerequisites
-* Python 3.8 or later is required to use this package. 
-* You must have a [Switch Automation user account](https://www.switchautomation.com/our-solution/) to use this package. 
-
-### Install the package
-Install the Switch Automation library for Python with [pip](https://pypi.org/project/pip/):
-
-```bash
-pip install switch_api
-```
-
 # History
 
-## 0.4.6
-
-### Added
-
-- Task Priority and Task Framework data feed deployment settings
-  - Task Priority and Task Framework are now available to set when deploying data feeds
-    - Task Priority
-      - Determines the priority of the datafeed tasks when processing.
-      - This equates to how much resources would be alloted to run the task
-      - Available options are: `default`, `standard`, or `advanced`.
-        - set to `advanced` for higher resource when processing data feed task
-      - Defaults to 'default'.
-    - Task Framework
-      - Determines the framework of the datafeed tasks when processing.
-        - 'PythonScriptFramework' for the old task runner engine.
-        - 'TaskInsightsEngine' for the new task running in container apps.
-        - Defaults to 'PythonScriptFramework'
+## 0.4.6b1
+- Will be removed
 
 ## 0.4.5
 
 ### Added
-
 - Email Sender Module
   - Send emails to active users within a Portfolio in Switch Automation Platform
   - Limitations:
     - Emails cannot be sent to users outside of the Portfolio including other users within the platform
     - Maximum of five attachments per email
     - Each attachment has a maximum size of 5mb
   - See function code documentation and usage example below
 - New `generate_filepath` method to provide a filepath where files can be stored
   - Works well with the attachment feature of the Email Sender Module. Store files in the generated filepath of this method and pass into email attachments
   - See function code documentation and usage example below
 
 ### Email Sender Usage
-
 ```python
 import switch_api as sw
 
 sw.email.send_email(
     api_inputs=api_inputs,
     subject='',
     body='',
@@ -85,53 +30,48 @@
     bcc_recipients=[], # Optional
     attachments=['/file/path/to/attachment.csv'], # Optional
     conversation_id='' # Optional
 )
 ```
 
 ### generate_filepath Usage
-
 ```python
 import switch_api as sw
 
 generated_attachment_filepath = sw.generate_filepath(api_inputs=api_inputs, filename='generated_attachment.txt')
 
 # Example of where it could be used
 sw.email.send_email(
     ...
     attachments=[generated_attachment_filepath]
     ...
 )
 ```
 
-### Fixed
 
+### Fixed
 - Issue where `upsert_device_sensors_ext` method was not posting metadata and tag_columns to API
 
 ## 0.3.3
 
 ### Added
-
 - New `upsert_device_sensors_ext` method to the `integration` module.
   - Compared to existing `upsert_device_sensors` following are supported:
     - Installation Code or Installation Id may be provided
       - BUT cannot provide mix of the two, all must have either code or id and not both.
     - DriverClassName
     - DriverDeviceType
     - PropertyName
-
 ### Added Feature - Switch Python Extensions
-
 - Extensions may be used in Task Insights and Switch Guides for code reuse
 - Extensions maybe located in any directory structure within the repo where the usage scripts are located
 - May need to adjust your environment to detect the files if you're not running a project environment
   - Tested on VSCode and PyCharm - contact Switch Support for issues.
 
 #### Extensions Usage
-
 ```python
 import switch_api as sw
 
 # Single import line per extension
 from extensions.my_extension import MyExtension
 
 @sw.extensions.provide(field="some_extension")
@@ -140,35 +80,34 @@
 
 if __name__ == "__main__":
     task = MyTask()
     task.some_extension.do_something()
 ```
 
 #### Extensions Registration
-
 ```python
 import uuid
 import switch_api as sw
 
 class SimpleExtension(sw.extensions.ExtensionTask):
     @property
     def id(self) -> uuid.UUID:
         # Unique ID for the extension.
         # Generate in CLI using:
         #   python -c 'import uuid; print(uuid.uuid4())'
         return '46759cfe-68fa-440c-baa9-c859264368db'
-
+    
     @property
     def description(self) -> str:
         return 'Extension with a simple get_name function.'
-
+    
     @property
     def author(self) -> str:
         return 'Amruth Akoju'
-
+    
     @property
     def version(self) -> str:
         return '1.0.1'
 
     def get_name(self):
         return "Simple Extension"
 
@@ -186,149 +125,136 @@
     # =================================================================
     register = sw.pipeline.Automation.register_task(api_inputs, task)
     print(register)
 
 ```
 
 ### Updated
-
 - get_data now has an optional parameter to return a pandas.DataFrame or JSON
 
 ## 0.2.27
 
 ### Fix
-
 - Issue where Timezone DST Offsets API response of `upsert_timeseries` in `integration` module was handled incorrectly
 
 ## 0.2.26
 
 ### Updated
-
-- Optional `table_def` parameter on `upsert_data`, `append_data`, and `replace_data` in `integration` module
+- Optional `table_def` parameter on `upsert_data`, `append_data`, and `replace_data` in `integration` module 
   - Enable clients to specify the table structure. It will be merged to the inferred table structure.
 - `list_deployments` in Automation module now provides `Settings` and `DriverId` associated with the deployments
 
+
 ## 0.2.25
 
 ### Updated
-
-- Update handling of empty Timezone DST Offsets of `upsert_timeseries` in `integration` module
+- Update handling of empty Timezone DST Offsets of `upsert_timeseries` in `integration` module 
 
 ## 0.2.24
 
 ### Updated
-
 - Fix default `ingestion_mode` parameter value to 'Queue' instead of 'Queued' on `upsert_timeseries` in `integration` module
 
 ## 0.2.23
 
 ### Updated
-
 - Optional `ingestion_mode` parameter on `upsert_timeseries` in `integration` module
   - Include `ingestionMode` in json payload passed to backend API
   - `IngestionMode` type must be `Queue` or `Stream`
   - Default `ingestion_mode` parameter value in `upsert_timeseries` is `Queue`
   - To enable table streaming ingestion, please contact **helpdesk@switchautomation.com** for assistance.
 
 ## 0.2.22
 
 ### Updated
-
 - Optional `ingestion_mode` parameter on `upsert_data` in `integration` module
   - Include `ingestionMode` in json payload passed to backend API
   - `IngestionMode` type must be `Queue` or `Stream`
   - Default `ingestion_mode` parameter value in `upsert_data` is `Queue`
   - To enable table streaming ingestion, please contact **helpdesk@switchautomation.com** for assistance.
 
 ### Fix
-
 - sw.pipeline.logger handlers stacking
 
 ## 0.2.21
 
 ### Updated
-
-- Fix on `get_data` method in `dataset` module
+- Fix on `get_data` method in `dataset` module 
   - Sync parameter structure to backend API for `get_data`
   - List of dict containing properties of `name`, `value`, and `type` items
   - `type` property must be one of subset of the new Literal `DATA_SET_QUERY_PARAMETER_TYPES`
 
 ## 0.2.20
 
 ### Added
-
 - Newly supported Azure Storage Account: GatewayMqttStorage
 - An optional property on QueueTask to specific QueueType
   - Default: DataIngestion
 
 ## 0.2.19
 
 ### Fixed
-
 - Fix on `upsert_timeseries` method in `integration` module
   - Normalized TimestampId and TimestampLocalId seconds
 - Minor fix on `upsert_entities_affected` method in `integration` utils module
   - Prevent upsert entities affected count when data feed file status Id is not valid
 - Minor fix on `get_metadata_keys` method in `integration` helper module
   - Fix for issue when a portfolio does not contain any values in the ApiMetadata table
 
+
 ## 0.2.18
 
 ### Added
-
 - Added new `is_specific_timezone` parameter in `upsert_timeseries` method of `integration` module
-
-  - Accepts a timezone name as the specific timezone used by the source data.
+  - Accepts a timezone name as the specific timezone used by the source data. 
   - Can either be of type str or bool and defaults to the value of False.
   - Cannot have value if 'is_local_time' is set to True.
   - Retrieve list of available timezones using 'get_timezones' method in `integration` module
+  
 
-    | is_specific_timezone | is_local_time | Description                                                                                                                                                     |
-    | -------------------- | ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-    | False                | False         | Datetimes in provided data is already in UTC and should remain as the value of Timestamp. The TimestampLocal (conversion to site-local Timezone) is calculated. |
-    | False                | True          | Datetimes in provided data is already in the site-local Timezone & should be used to set the value of the TimestampLocal field. The UTC Timestamp is calculated |
-    | Has Value            | True          | NOT ALLOWED                                                                                                                                                     |
-    | Has Value            | False         | Both Timestamp and TimestampLocal fields will are calculated. Datetime is converted to UTC then to Local.                                                       |
-    | True                 |               | NOT ALLOWED                                                                                                                                                     |
-    | '' (empty string)    |               | NOT ALLOWED                                                                                                                                                     |
+    | is_specific_timezone  | is_local_time | Description |
+    | --------------------- | -------- | ----------- |
+    | False  | False  | Datetimes in provided data is already in UTC and should remain as the value of Timestamp. The TimestampLocal (conversion to site-local Timezone) is calculated. |
+    | False  | True  | Datetimes in provided data is already in the site-local Timezone & should be used to set the value of the TimestampLocal field. The UTC Timestamp is calculated |
+    | Has Value | True  | NOT ALLOWED |
+    | Has Value | False  | Both Timestamp and TimestampLocal fields will are calculated. Datetime is converted to UTC then to Local. |
+    | True  |   | NOT ALLOWED |
+    | '' (empty string)  |   | NOT ALLOWED |
+  
 
 ### Fixed
-
-- Minor fix on `upsert_tags` and `upsert_device_metadata` methods in `integration` module
+- Minor fix on `upsert_tags` and `upsert_device_metadata` methods in `integration` module 
   - List of required_columns was incorrectly being updated when these functions were called
 - Minor fix on `upsert_event_work_order_id` method in `integration` module when attempting to update status of an Event
 
 ### Updated
-
 - Update on `DiscoveryIntegrationInput` namedtuple - added `job_id`
 - Update `upsert_discovered_records` method required columns in `integration` module
   - add required `JobId` column for Data Frame parameter
 
-## 0.2.17
 
+## 0.2.17
 ### Fixed
-
 - Fix on `upsert_timeseries()` method in `integration` module for duplicate records in ingestion files
   - records whose Timestamp falls in the exact DST start created 2 records with identical values but different TimestampLocal
     - one has the TimestampLocal of a DST and the other does not
 
 ### Updated
-
 - Update on `get_sites()` method in `integration` module for `InstallationCode` column
   - when the `InstallationCode' value is null in the database it returns an empty string
   - `InstallationCode` column is explicity casted to dtype 'str'
 
-## 0.2.16
 
+## 0.2.16
 ### Added
 
 - Added new 5 minute interval for `EXPECTED_DELIVERY` Literal in `automation` module
   - support for data feed deployments Email, FTP, Upload, and Timer
   - usage: expected_delivery='5min'
-
+  
 ### Fixed
 
 - Minor fix on `upsert_timeseries()` method using `data_feed_file_status_id` parameter in `integration` module.
   - `data_feed_file_status_id` parameter value now synced between process records and ingestion files when supplied
 
 ### Updated
 
@@ -827,9 +753,7 @@
 - `kql`
 
 Removed the `name_as_filename` and `treat_as_timeseries` parameter from the following functions:
 
 - `switch.integration.replace_data()`
 - `switch.integration.append_data()`
 - `switch.integration.upload_data()`
-
-
```

### Comparing `switch_api-0.4.6/switch_api.egg-info/SOURCES.txt` & `switch_api-0.4.6b2/switch_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

