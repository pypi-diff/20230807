# Comparing `tmp/rapyuta-io-cli-4.0.0.tar.gz` & `tmp/rapyuta-io-cli-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapyuta-io-cli-4.0.0.tar", last modified: Thu Aug  3 12:50:03 2023, max compression
+gzip compressed data, was "rapyuta-io-cli-4.0.1.tar", last modified: Mon Aug  7 11:05:45 2023, max compression
```

## Comparing `rapyuta-io-cli-4.0.0.tar` & `rapyuta-io-cli-4.0.1.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.196212 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      468 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-03 12:50:03.000000 rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.196212 rapyuta-io-cli-4.0.0/riocli/
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.196212 rapyuta-io-cli-4.0.0/riocli/apply/
--rw-r--r--   0 runner    (1001) docker     (122)     5051 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)    16402 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/resolver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/template.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/apply/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.196212 rapyuta-io-cli-4.0.0/riocli/auth/
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/staging.py
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (122)     5387 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     4039 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/build/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/import_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/trigger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/build/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/chart/
--rw-r--r--   0 runner    (1001) docker     (122)     1341 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     3223 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/search.py
--rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/chart/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/completion/
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/config/
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/constants/
--rw-r--r--   0 runner    (1001) docker     (122)      698 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/constants/colors.py
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/constants/symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/deployment/
--rw-r--r--   0 runner    (1001) docker     (122)     1835 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2801 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)    17137 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/update.py
--rw-r--r--   0 runner    (1001) docker     (122)     5745 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/deployment/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/device/
--rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5698 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2837 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1857 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     8382 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/label.py
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/metric.py
--rw-r--r--   0 runner    (1001) docker     (122)     2718 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/onboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.200212 rapyuta-io-cli-4.0.0/riocli/device/tools/
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/device_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/forward.py
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/rapyuta_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/scp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/service.py
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     2745 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/device/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/disk/
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3515 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/disk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/jsonschema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/jsonschema/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/managedservice/
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1325 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/list_providers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/managedservice/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/model/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6887 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/network/
--rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1739 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4481 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/native_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/routed_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     6455 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/network/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/organization/
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/organization/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/organization/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/organization/users.py
--rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/organization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/package/
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/deployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     9502 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/package/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/parameter/
--rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3479 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     4054 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2595 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/download.py
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2628 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/upload.py
--rw-r--r--   0 runner    (1001) docker     (122)     2874 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/parameter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/project/
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/project/features/
--rw-r--r--   0 runner    (1001) docker     (122)      974 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1993 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/features/vpn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2892 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     4157 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/project/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.204212 rapyuta-io-cli-4.0.0/riocli/rosbag/
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/rosbag/blob.py
--rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/rosbag/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/rosbag/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/secret/
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/docker_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/import_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/source_secret.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/secret/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/shell/
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/shell/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/static_route/
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/open.py
--rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/static_route/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/usergroup/
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/list.py
--rw-r--r--   0 runner    (1001) docker     (122)     6082 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/usergroup/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/selector.py
--rw-r--r--   0 runner    (1001) docker     (122)     1602 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/spinner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/utils/ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/v2client/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/v2client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11183 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/v2client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/riocli/vpn/
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5743 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/ping.py
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/riocli/vpn/util.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-03 12:50:03.208211 rapyuta-io-cli-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-08-03 12:49:52.000000 rapyuta-io-cli-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.634956 rapyuta-io-cli-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-08-07 11:05:45.634956 rapyuta-io-cli-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.614956 rapyuta-io-cli-4.0.1/rapyuta_io_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-08-07 11:05:45.000000 rapyuta-io-cli-4.0.1/rapyuta_io_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-08-07 11:05:45.000000 rapyuta-io-cli-4.0.1/rapyuta_io_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-07 11:05:45.000000 rapyuta-io-cli-4.0.1/rapyuta_io_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-08-07 11:05:45.000000 rapyuta-io-cli-4.0.1/rapyuta_io_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-08-07 11:05:45.000000 rapyuta-io-cli-4.0.1/rapyuta_io_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-07 11:05:45.000000 rapyuta-io-cli-4.0.1/rapyuta_io_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.614956 rapyuta-io-cli-4.0.1/riocli/
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.618956 rapyuta-io-cli-4.0.1/riocli/apply/
+-rw-r--r--   0 runner    (1001) docker     (122)     5051 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/apply/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16402 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/apply/parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/apply/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/apply/template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/apply/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.618956 rapyuta-io-cli-4.0.1/riocli/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/auth/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/auth/staging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/auth/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5387 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4039 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.622956 rapyuta-io-cli-4.0.1/riocli/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/build/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/build/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/build/import_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/build/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/build/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/build/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/build/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/build/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/build/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.622956 rapyuta-io-cli-4.0.1/riocli/chart/
+-rw-r--r--   0 runner    (1001) docker     (122)     1341 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2393 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/chart/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3223 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/chart/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/chart/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/chart/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/chart/search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/chart/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.622956 rapyuta-io-cli-4.0.1/riocli/completion/
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.622956 rapyuta-io-cli-4.0.1/riocli/config/
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.622956 rapyuta-io-cli-4.0.1/riocli/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/constants/colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/constants/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.626956 rapyuta-io-cli-4.0.1/riocli/deployment/
+-rw-r--r--   0 runner    (1001) docker     (122)     1835 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2801 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17137 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5745 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/deployment/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.626956 rapyuta-io-cli-4.0.1/riocli/device/
+-rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5698 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2837 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1857 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8382 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4083 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2718 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/onboard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.626956 rapyuta-io-cli-4.0.1/riocli/device/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/tools/device_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/tools/forward.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/tools/rapyuta_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/tools/scp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/tools/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/tools/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2745 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3816 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/device/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.626956 rapyuta-io-cli-4.0.1/riocli/disk/
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/disk/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/disk/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/disk/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/disk/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3515 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/disk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.626956 rapyuta-io-cli-4.0.1/riocli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.626956 rapyuta-io-cli-4.0.1/riocli/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/jsonschema/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.626956 rapyuta-io-cli-4.0.1/riocli/managedservice/
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/managedservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/managedservice/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/managedservice/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1325 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/managedservice/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1273 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/managedservice/list_providers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/managedservice/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.626956 rapyuta-io-cli-4.0.1/riocli/model/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6887 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.626956 rapyuta-io-cli-4.0.1/riocli/network/
+-rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/network/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2471 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/network/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1739 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/network/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/network/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/network/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4481 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/network/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/network/native_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/network/routed_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6455 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/network/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.630956 rapyuta-io-cli-4.0.1/riocli/organization/
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/organization/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/organization/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/organization/users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/organization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.630956 rapyuta-io-cli-4.0.1/riocli/package/
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/package/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/package/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/package/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/package/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/package/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9502 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/package/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/package/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.630956 rapyuta-io-cli-4.0.1/riocli/parameter/
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3578 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/parameter/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/parameter/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4054 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/parameter/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2595 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/parameter/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/parameter/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/parameter/upload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2874 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/parameter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.630956 rapyuta-io-cli-4.0.1/riocli/project/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/project/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/project/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.630956 rapyuta-io-cli-4.0.1/riocli/project/features/
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/project/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1993 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/project/features/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/project/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2892 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/project/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1520 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/project/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4157 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/project/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.630956 rapyuta-io-cli-4.0.1/riocli/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/rosbag/blob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11554 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/rosbag/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/rosbag/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.630956 rapyuta-io-cli-4.0.1/riocli/secret/
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/secret/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/secret/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/secret/docker_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/secret/import_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/secret/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/secret/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/secret/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/secret/source_secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/secret/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.630956 rapyuta-io-cli-4.0.1/riocli/shell/
+-rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/shell/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.630956 rapyuta-io-cli-4.0.1/riocli/static_route/
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/static_route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/static_route/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/static_route/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/static_route/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/static_route/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/static_route/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/static_route/open.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/static_route/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.630956 rapyuta-io-cli-4.0.1/riocli/usergroup/
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/usergroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/usergroup/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/usergroup/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/usergroup/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6082 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/usergroup/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/usergroup/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.634956 rapyuta-io-cli-4.0.1/riocli/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     6971 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/utils/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/utils/selector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/utils/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/utils/ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.634956 rapyuta-io-cli-4.0.1/riocli/v2client/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/v2client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11183 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/v2client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:05:45.634956 rapyuta-io-cli-4.0.1/riocli/vpn/
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/vpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5743 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/vpn/connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/vpn/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/vpn/ping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/vpn/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/riocli/vpn/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-07 11:05:45.634956 rapyuta-io-cli-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-08-07 11:05:35.000000 rapyuta-io-cli-4.0.1/setup.py
```

### Comparing `rapyuta-io-cli-4.0.0/PKG-INFO` & `rapyuta-io-cli-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 4.0.0
+Version: 4.0.1
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-4.0.0/README.md` & `rapyuta-io-cli-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/PKG-INFO` & `rapyuta-io-cli-4.0.1/rapyuta_io_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 4.0.0
+Version: 4.0.1
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-4.0.0/rapyuta_io_cli.egg-info/SOURCES.txt` & `rapyuta-io-cli-4.0.1/rapyuta_io_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/__main__.py` & `rapyuta-io-cli-4.0.1/riocli/__main__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/apply/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/apply/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/apply/explain.py` & `rapyuta-io-cli-4.0.1/riocli/apply/explain.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/apply/parse.py` & `rapyuta-io-cli-4.0.1/riocli/apply/parse.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/apply/resolver.py` & `rapyuta-io-cli-4.0.1/riocli/apply/resolver.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/apply/template.py` & `rapyuta-io-cli-4.0.1/riocli/apply/template.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/apply/util.py` & `rapyuta-io-cli-4.0.1/riocli/apply/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/auth/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/auth/login.py` & `rapyuta-io-cli-4.0.1/riocli/auth/login.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/auth/logout.py` & `rapyuta-io-cli-4.0.1/riocli/auth/logout.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/auth/refresh_token.py` & `rapyuta-io-cli-4.0.1/riocli/auth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/auth/staging.py` & `rapyuta-io-cli-4.0.1/riocli/auth/staging.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/auth/status.py` & `rapyuta-io-cli-4.0.1/riocli/auth/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/auth/token.py` & `rapyuta-io-cli-4.0.1/riocli/auth/token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/auth/util.py` & `rapyuta-io-cli-4.0.1/riocli/auth/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/bootstrap.py` & `rapyuta-io-cli-4.0.1/riocli/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "4.0.0"
+__version__ = "4.0.1"
 
 import click
 import rapyuta_io.version
 from click import Context
 from click_help_colors import HelpColorsGroup
 from click_plugins import with_plugins
 from pkg_resources import iter_entry_points
```

### Comparing `rapyuta-io-cli-4.0.0/riocli/build/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/build/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/build/create.py` & `rapyuta-io-cli-4.0.1/riocli/build/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/build/delete.py` & `rapyuta-io-cli-4.0.1/riocli/build/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/build/import_build.py` & `rapyuta-io-cli-4.0.1/riocli/build/import_build.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/build/inspect.py` & `rapyuta-io-cli-4.0.1/riocli/build/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/build/list.py` & `rapyuta-io-cli-4.0.1/riocli/build/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/build/logs.py` & `rapyuta-io-cli-4.0.1/riocli/build/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/build/model.py` & `rapyuta-io-cli-4.0.1/riocli/build/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/build/trigger.py` & `rapyuta-io-cli-4.0.1/riocli/build/trigger.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/build/util.py` & `rapyuta-io-cli-4.0.1/riocli/build/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/chart/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/chart/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/chart/apply.py` & `rapyuta-io-cli-4.0.1/riocli/chart/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/chart/chart.py` & `rapyuta-io-cli-4.0.1/riocli/chart/chart.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/chart/delete.py` & `rapyuta-io-cli-4.0.1/riocli/chart/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/chart/info.py` & `rapyuta-io-cli-4.0.1/riocli/chart/info.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/chart/list.py` & `rapyuta-io-cli-4.0.1/riocli/chart/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/chart/search.py` & `rapyuta-io-cli-4.0.1/riocli/chart/search.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/chart/util.py` & `rapyuta-io-cli-4.0.1/riocli/chart/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/completion/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/config/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/config/config.py` & `rapyuta-io-cli-4.0.1/riocli/config/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/constants/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/constants/colors.py` & `rapyuta-io-cli-4.0.1/riocli/constants/colors.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/constants/symbols.py` & `rapyuta-io-cli-4.0.1/riocli/constants/symbols.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/delete.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/errors.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/errors.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/execute.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/execute.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import sys
 import typing
 
 import click
 from click_help_colors import HelpColorsCommand
-from yaspin import kbi_safe_yaspin
+
+if sys.stdout.isatty():
+    from yaspin import kbi_safe_yaspin as Spinner
+else:
+    from riocli.utils.spinner import DummySpinner as Spinner
 
 from riocli.constants import Colors
 from riocli.deployment.util import name_to_guid, select_details
 from riocli.utils.execute import run_on_cloud
 
 
 @click.command(
@@ -45,15 +49,15 @@
 ) -> None:
     """
     Execute commands on cloud deployment
     """
     try:
         comp_id, exec_id, pod_name = select_details(deployment_guid, component_name, exec_name)
 
-        with kbi_safe_yaspin(text='Executing command `{}`...'.format(command)) as spinner:
+        with Spinner(text='Executing command `{}`...'.format(command)):
             stdout, stderr = run_on_cloud(deployment_guid, comp_id, exec_id, pod_name, command)
 
         if stderr:
             click.secho(stderr, fg=Colors.RED)
         if stdout:
             click.secho(stdout, fg=Colors.YELLOW)
     except Exception as e:
```

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/inspect.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/list.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/logs.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/model.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/ssh.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/status.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/update.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/update.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/util.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/deployment/wait.py` & `rapyuta-io-cli-4.0.1/riocli/deployment/wait.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/device/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/config.py` & `rapyuta-io-cli-4.0.1/riocli/device/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/create.py` & `rapyuta-io-cli-4.0.1/riocli/device/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/delete.py` & `rapyuta-io-cli-4.0.1/riocli/device/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/deployment.py` & `rapyuta-io-cli-4.0.1/riocli/device/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/execute.py` & `rapyuta-io-cli-4.0.1/riocli/device/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/files.py` & `rapyuta-io-cli-4.0.1/riocli/device/files.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/inspect.py` & `rapyuta-io-cli-4.0.1/riocli/device/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/label.py` & `rapyuta-io-cli-4.0.1/riocli/device/label.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/list.py` & `rapyuta-io-cli-4.0.1/riocli/device/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/metric.py` & `rapyuta-io-cli-4.0.1/riocli/device/metric.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/model.py` & `rapyuta-io-cli-4.0.1/riocli/device/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/onboard.py` & `rapyuta-io-cli-4.0.1/riocli/device/onboard.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/tools/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/device/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/tools/device_init.py` & `rapyuta-io-cli-4.0.1/riocli/device/tools/device_init.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/tools/forward.py` & `rapyuta-io-cli-4.0.1/riocli/device/tools/forward.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/tools/rapyuta_logs.py` & `rapyuta-io-cli-4.0.1/riocli/device/tools/rapyuta_logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/tools/scp.py` & `rapyuta-io-cli-4.0.1/riocli/device/tools/scp.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/tools/service.py` & `rapyuta-io-cli-4.0.1/riocli/device/tools/service.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/tools/ssh.py` & `rapyuta-io-cli-4.0.1/riocli/device/tools/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/tools/util.py` & `rapyuta-io-cli-4.0.1/riocli/device/tools/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/topic.py` & `rapyuta-io-cli-4.0.1/riocli/device/topic.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/util.py` & `rapyuta-io-cli-4.0.1/riocli/device/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/device/vpn.py` & `rapyuta-io-cli-4.0.1/riocli/device/vpn.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,24 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import sys
 import typing
 
 import click
 from click_help_colors import HelpColorsCommand
-from yaspin import kbi_safe_yaspin
+
+if sys.stdout.isatty():
+    from yaspin import kbi_safe_yaspin as Spinner
+else:
+    from riocli.utils.spinner import DummySpinner as Spinner
 
 from riocli.config import new_client
 from riocli.constants import Colors
 from riocli.utils import tabulate_data
 
 
 @click.command(
@@ -74,15 +79,15 @@
             click.confirm(
                 "\nDo you want to proceed?",
                 default=True, abort=True)
 
         click.echo("")  # Echo an empty line
 
         result = []
-        with kbi_safe_yaspin() as spinner:
+        with Spinner() as spinner:
             for device in final:
                 spinner.text = 'Updating VPN state on device {}'.format(
                     click.style(device.name, bold=True, fg=Colors.CYAN))
                 r = client.toggle_features(device.uuid, [('vpn', enable)])
                 result.append([device.name, r.get('status')])
 
         click.echo("")  # Echo an empty line
```

### Comparing `rapyuta-io-cli-4.0.0/riocli/disk/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/disk/create.py` & `rapyuta-io-cli-4.0.1/riocli/disk/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/disk/delete.py` & `rapyuta-io-cli-4.0.1/riocli/disk/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/disk/list.py` & `rapyuta-io-cli-4.0.1/riocli/disk/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/disk/model.py` & `rapyuta-io-cli-4.0.1/riocli/disk/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/disk/util.py` & `rapyuta-io-cli-4.0.1/riocli/disk/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/exceptions/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/jsonschema/validate.py` & `rapyuta-io-cli-4.0.1/riocli/jsonschema/validate.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/managedservice/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/managedservice/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/managedservice/delete.py` & `rapyuta-io-cli-4.0.1/riocli/managedservice/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/managedservice/inspect.py` & `rapyuta-io-cli-4.0.1/riocli/managedservice/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/managedservice/list.py` & `rapyuta-io-cli-4.0.1/riocli/managedservice/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/managedservice/list_providers.py` & `rapyuta-io-cli-4.0.1/riocli/managedservice/list_providers.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/managedservice/model.py` & `rapyuta-io-cli-4.0.1/riocli/managedservice/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/model/base.py` & `rapyuta-io-cli-4.0.1/riocli/model/base.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/network/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/network/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/network/create.py` & `rapyuta-io-cli-4.0.1/riocli/network/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/network/delete.py` & `rapyuta-io-cli-4.0.1/riocli/network/delete.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             client.delete_routed_network(network_guid)
         elif network_type == 'native':
             client.delete_native_network(network_guid)
         else:
             raise Exception('invalid network type')
 
         spinner.text = click.style(
-            '{} deleted successfully!'.format(network_type.capitalize()),
+            '{} network deleted successfully!'.format(network_type.capitalize()),
             fg=Colors.GREEN)
         spinner.green.ok(Symbols.SUCCESS)
     except Exception as e:
         spinner.text = click.style('Failed to delete network: {}'.format(e),
                                    fg=Colors.RED)
         spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-4.0.0/riocli/network/inspect.py` & `rapyuta-io-cli-4.0.1/riocli/network/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/network/list.py` & `rapyuta-io-cli-4.0.1/riocli/network/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/network/logs.py` & `rapyuta-io-cli-4.0.1/riocli/network/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/network/model.py` & `rapyuta-io-cli-4.0.1/riocli/network/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/network/native_network.py` & `rapyuta-io-cli-4.0.1/riocli/network/native_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/network/routed_network.py` & `rapyuta-io-cli-4.0.1/riocli/network/routed_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/network/util.py` & `rapyuta-io-cli-4.0.1/riocli/network/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/organization/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/organization/list.py` & `rapyuta-io-cli-4.0.1/riocli/organization/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/organization/select.py` & `rapyuta-io-cli-4.0.1/riocli/organization/select.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/organization/users.py` & `rapyuta-io-cli-4.0.1/riocli/organization/users.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/organization/utils.py` & `rapyuta-io-cli-4.0.1/riocli/organization/utils.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/package/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/package/create.py` & `rapyuta-io-cli-4.0.1/riocli/package/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/package/delete.py` & `rapyuta-io-cli-4.0.1/riocli/package/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/package/deployment.py` & `rapyuta-io-cli-4.0.1/riocli/package/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/package/inspect.py` & `rapyuta-io-cli-4.0.1/riocli/package/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/package/list.py` & `rapyuta-io-cli-4.0.1/riocli/package/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/package/model.py` & `rapyuta-io-cli-4.0.1/riocli/package/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/package/util.py` & `rapyuta-io-cli-4.0.1/riocli/package/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/parameter/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/parameter/apply.py` & `rapyuta-io-cli-4.0.1/riocli/parameter/apply.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,19 +7,24 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import sys
 import typing
 
 import click
 from click_help_colors import HelpColorsCommand
-from yaspin import kbi_safe_yaspin
+
+if sys.stdout.isatty():
+    from yaspin import kbi_safe_yaspin as Spinner
+else:
+    from riocli.utils.spinner import DummySpinner as Spinner
 
 from riocli.config import new_client
 from riocli.constants import Colors, Symbols
 from riocli.utils import tabulate_data, print_separator
 
 
 @click.command(
@@ -75,15 +80,15 @@
                     fg=Colors.GREEN)
 
         if not silent:
             click.confirm(
                 "Do you want to apply the configurations?",
                 default=True, abort=True)
 
-        with kbi_safe_yaspin(text='Applying parameters...') as spinner:
+        with Spinner(text='Applying parameters...'):
             response = client.apply_parameters(
                 list(device_ids.keys()),
                 list(tree_names),
                 retry_limit
             )
 
         print_separator()
```

### Comparing `rapyuta-io-cli-4.0.0/riocli/parameter/delete.py` & `rapyuta-io-cli-4.0.1/riocli/parameter/delete.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
+
 import click
 from click_help_colors import HelpColorsCommand
 from rapyuta_io.utils.rest_client import HttpMethod
-from yaspin import kbi_safe_yaspin
+
+if sys.stdout.isatty():
+    from yaspin import kbi_safe_yaspin as Spinner
+else:
+    from riocli.utils.spinner import DummySpinner as Spinner
 
 from riocli.constants import Colors, Symbols
 from riocli.parameter.utils import _api_call
 
 
 @click.command(
     'delete',
@@ -39,15 +45,15 @@
     Deletes the configuration parameter tree.
     """
     click.secho('Configuration Parameter {} will be deleted'.format(tree))
 
     if not silent:
         click.confirm('Do you want to proceed?', default=True, abort=True)
 
-    with kbi_safe_yaspin(text='Deleting...', timer=True) as spinner:
+    with Spinner(text='Deleting...', timer=True) as spinner:
         try:
             data = _api_call(HttpMethod.DELETE, name=tree)
             if data.get('data') != 'ok':
                 raise Exception('Failed to delete configuration')
 
             spinner.text = click.style(
                 'Configuration deleted successfully.',
```

### Comparing `rapyuta-io-cli-4.0.0/riocli/parameter/diff.py` & `rapyuta-io-cli-4.0.1/riocli/parameter/diff.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/parameter/download.py` & `rapyuta-io-cli-4.0.1/riocli/parameter/download.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/parameter/list.py` & `rapyuta-io-cli-4.0.1/riocli/parameter/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/parameter/upload.py` & `rapyuta-io-cli-4.0.1/riocli/parameter/upload.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,20 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import sys
 import typing
 
 import click
 from click_help_colors import HelpColorsCommand
-from yaspin import kbi_safe_yaspin
 
+if sys.stdout.isatty():
+    from yaspin import kbi_safe_yaspin as Spinner
+else:
+    from riocli.utils.spinner import DummySpinner as Spinner
 from riocli.config import new_client
 from riocli.constants import Colors, Symbols
 from riocli.parameter.utils import filter_trees, display_trees
 
 
 @click.command(
     'upload',
@@ -53,16 +57,15 @@
     display_trees(path, trees)
 
     if not silent:
         click.confirm('Do you want to proceed?', default=True, abort=True)
 
     client = new_client()
 
-    with kbi_safe_yaspin(text="Uploading configurations...",
-                         timer=True) as spinner:
+    with Spinner(text="Uploading configurations...", timer=True) as spinner:
         try:
             client.upload_configurations(
                 rootdir=path,
                 tree_names=trees,
                 delete_existing_trees=delete_existing,
                 as_folder=True
             )
```

### Comparing `rapyuta-io-cli-4.0.0/riocli/parameter/utils.py` & `rapyuta-io-cli-4.0.1/riocli/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/project/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/project/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/project/create.py` & `rapyuta-io-cli-4.0.1/riocli/project/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/project/delete.py` & `rapyuta-io-cli-4.0.1/riocli/project/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/project/features/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/project/features/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/project/features/vpn.py` & `rapyuta-io-cli-4.0.1/riocli/project/features/vpn.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/project/inspect.py` & `rapyuta-io-cli-4.0.1/riocli/project/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/project/list.py` & `rapyuta-io-cli-4.0.1/riocli/project/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/project/model.py` & `rapyuta-io-cli-4.0.1/riocli/project/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/project/select.py` & `rapyuta-io-cli-4.0.1/riocli/project/select.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/project/util.py` & `rapyuta-io-cli-4.0.1/riocli/project/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/rosbag/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/rosbag/blob.py` & `rapyuta-io-cli-4.0.1/riocli/rosbag/blob.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/rosbag/job.py` & `rapyuta-io-cli-4.0.1/riocli/rosbag/job.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/secret/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/secret/create.py` & `rapyuta-io-cli-4.0.1/riocli/secret/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/secret/delete.py` & `rapyuta-io-cli-4.0.1/riocli/secret/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/secret/docker_secret.py` & `rapyuta-io-cli-4.0.1/riocli/secret/docker_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/secret/import_secret.py` & `rapyuta-io-cli-4.0.1/riocli/secret/import_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/secret/inspect.py` & `rapyuta-io-cli-4.0.1/riocli/secret/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/secret/list.py` & `rapyuta-io-cli-4.0.1/riocli/secret/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/secret/model.py` & `rapyuta-io-cli-4.0.1/riocli/secret/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/secret/source_secret.py` & `rapyuta-io-cli-4.0.1/riocli/secret/source_secret.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/secret/util.py` & `rapyuta-io-cli-4.0.1/riocli/secret/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/shell/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/shell/prompt.py` & `rapyuta-io-cli-4.0.1/riocli/shell/prompt.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/static_route/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/static_route/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/static_route/create.py` & `rapyuta-io-cli-4.0.1/riocli/static_route/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/static_route/delete.py` & `rapyuta-io-cli-4.0.1/riocli/static_route/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/static_route/inspect.py` & `rapyuta-io-cli-4.0.1/riocli/static_route/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/static_route/list.py` & `rapyuta-io-cli-4.0.1/riocli/static_route/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/static_route/model.py` & `rapyuta-io-cli-4.0.1/riocli/static_route/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/static_route/open.py` & `rapyuta-io-cli-4.0.1/riocli/static_route/open.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/static_route/util.py` & `rapyuta-io-cli-4.0.1/riocli/static_route/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/usergroup/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/usergroup/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/usergroup/delete.py` & `rapyuta-io-cli-4.0.1/riocli/usergroup/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/usergroup/inspect.py` & `rapyuta-io-cli-4.0.1/riocli/usergroup/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/usergroup/list.py` & `rapyuta-io-cli-4.0.1/riocli/usergroup/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/usergroup/model.py` & `rapyuta-io-cli-4.0.1/riocli/usergroup/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/usergroup/util.py` & `rapyuta-io-cli-4.0.1/riocli/usergroup/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/utils/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     click.secho(" " * col, bg=color)
 
 
 def is_pip_installation() -> bool:
     return 'python' in sys.executable
 
 
-def check_for_updates(current_version: str) -> tuple[bool, str]:
+def check_for_updates(current_version: typing.Text) -> typing.Tuple[bool, typing.Text]:
     try:
         package_info = requests.get(
             'https://pypi.org/pypi/rapyuta-io-cli/json').json()
     except Exception as e:
         click.secho('Failed to fetch upstream package info: {}'.format(e),
                     fg=Colors.RED)
         raise SystemExit(1) from e
```

### Comparing `rapyuta-io-cli-4.0.0/riocli/utils/context.py` & `rapyuta-io-cli-4.0.1/riocli/utils/context.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/utils/execute.py` & `rapyuta-io-cli-4.0.1/riocli/utils/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/utils/mermaid.py` & `rapyuta-io-cli-4.0.1/riocli/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/utils/selector.py` & `rapyuta-io-cli-4.0.1/riocli/utils/selector.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/utils/spinner.py` & `rapyuta-io-cli-4.0.1/riocli/vpn/ping.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,44 +8,70 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import functools
-
-from yaspin import kbi_safe_yaspin
-
-
-def with_spinner(**spin_kwargs):
+import click
+from click_help_colors import HelpColorsCommand
+from yaspin.api import Yaspin
+
+from riocli.constants import Colors, Symbols
+from riocli.utils.spinner import with_spinner
+from riocli.vpn.util import (
+    install_vpn_tools,
+    is_tailscale_up,
+    get_tailscale_status,
+    tailscale_ping
+)
+
+
+@click.command(
+    'ping-all',
+    cls=HelpColorsCommand,
+    help_headers_color=Colors.YELLOW,
+    help_options_color=Colors.GREEN,
+)
+@click.pass_context
+@with_spinner(text="Pinging all peers...")
+def ping_all(ctx: click.Context, spinner: Yaspin = None):
     """
-    Decorator for wrapping your function with a spinner
-
-    Add `spinner=None` in your function's arguments. You can use the
-    `yaspin` spinner object as it and don't have to worry about starting
-    and stopping the spinner
-
-        @with_spinner(text="Do something..", timer=True)
-        def do_something(arg1, spinner=None):
-            with spinner.hidden(): # doesn't break spinner
-                click.secho("Fetching something...")
-
-            ok = does_something(arg1)
-
-            if ok:
-                spinner.ok("✅")
-            else:
-                spinner.fail("✘")
-                raise SystemExit(1)
+    Ping all the peers in the network
     """
-
-    def decorated(func):
-        @functools.wraps(func)
-        def wrapper(*args, **kwargs):
-            with kbi_safe_yaspin(**spin_kwargs) as spinner:
-                kwargs['spinner'] = spinner
-                return func(*args, **kwargs)
-
-        return wrapper
-
-    return decorated
+    try:
+        with spinner.hidden():
+            install_vpn_tools()
+
+        if not is_tailscale_up():
+            spinner.text = click.style(
+                'You are not connected to the VPN', fg=Colors.YELLOW)
+            spinner.yellow.ok(Symbols.WARNING)
+            return
+
+        ping_all_peers(spinner)
+
+        spinner.text = click.style('Ping complete', fg=Colors.GREEN)
+        spinner.green.ok(Symbols.SUCCESS)
+    except Exception as e:
+        spinner.text = click.style(str(e), fg=Colors.RED)
+        spinner.red.fail(Symbols.ERROR)
+        raise SystemExit(1) from e
+
+
+def ping_all_peers(spinner: Yaspin):
+    s = get_tailscale_status()
+
+    peers = s.get('Peer', {})
+
+    for _, v in peers.items():
+        # Do not waste time pinging
+        # offline nodes
+        if not v.get('Online'):
+            continue
+
+        spinner.text = 'Pinging: {}...'.format(
+            click.style(v.get('HostName'), italic=True)
+        )
+        ips = v.get('TailscaleIPs')
+        for ip in ips:
+            tailscale_ping(ip)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rapyuta-io-cli-4.0.0/riocli/utils/ssh_tunnel.py` & `rapyuta-io-cli-4.0.1/riocli/utils/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/v2client/client.py` & `rapyuta-io-cli-4.0.1/riocli/v2client/client.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/vpn/__init__.py` & `rapyuta-io-cli-4.0.1/riocli/vpn/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/vpn/connect.py` & `rapyuta-io-cli-4.0.1/riocli/vpn/connect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/vpn/disconnect.py` & `rapyuta-io-cli-4.0.1/riocli/vpn/disconnect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/vpn/status.py` & `rapyuta-io-cli-4.0.1/riocli/vpn/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/riocli/vpn/util.py` & `rapyuta-io-cli-4.0.1/riocli/vpn/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-4.0.0/setup.py` & `rapyuta-io-cli-4.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,13 +52,13 @@
         "setuptools",
         "six>=1.13.0",
         "tabulate>=0.8.0",
         "urllib3>=1.23",
         "pyrfc3339>=1.1",
         "directory-tree>=0.0.3.1",
         "yaspin>=2.3.0",
-        "jsonschema>=4.0.0",
+        "jsonschema==4.0.0",
         "waiting>=1.4.1",
         "semver>=3.0.0",
     ],
     setup_requires=["flake8"],
 )
```

