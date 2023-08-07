# Comparing `tmp/eth-monitor-0.8.0.tar.gz` & `tmp/eth-monitor-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-monitor-0.8.0.tar", last modified: Sun Aug  6 13:20:35 2023, max compression
+gzip compressed data, was "eth-monitor-0.8.1.tar", last modified: Sun Aug  6 18:33:29 2023, max compression
```

## Comparing `eth-monitor-0.8.0.tar` & `eth-monitor-0.8.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/
--rw-r--r--   0 lash      (1000) lash      (1000)     1733 2023-08-06 13:10:25.000000 eth-monitor-0.8.0/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:56:11.000000 eth-monitor-0.8.0/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      110 2023-05-13 20:45:22.000000 eth-monitor-0.8.0/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     9706 2023-05-13 20:42:58.000000 eth-monitor-0.8.0/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      871 2022-11-14 07:52:42.000000 eth-monitor-0.8.0/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:55:49.000000 eth-monitor-0.8.0/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor/
--rw-r--r--   0 lash      (1000) lash      (1000)      902 2022-11-11 05:56:27.000000 eth-monitor-0.8.0/eth_monitor/callback.py
--rw-r--r--   0 lash      (1000) lash      (1000)      645 2023-08-06 12:18:29.000000 eth-monitor-0.8.0/eth_monitor/chain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)       65 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3190 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1923 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/cli/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)      518 2022-11-14 07:56:11.000000 eth-monitor-0.8.0/eth_monitor/cli/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)      271 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/cli/rules.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1327 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/config.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.118382 eth-monitor-0.8.0/eth_monitor/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       40 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/data/config/cache.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/data/config/filter.ini
--rw-r--r--   0 lash      (1000) lash      (1000)      243 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/data/config/monitor.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       22 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/data/config/renderer.ini
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor/filters/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-01-30 14:12:19.000000 eth-monitor-0.8.0/eth_monitor/filters/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      580 2022-11-11 05:56:27.000000 eth-monitor-0.8.0/eth_monitor/filters/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      263 2022-11-11 05:56:27.000000 eth-monitor-0.8.0/eth_monitor/filters/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)      732 2022-11-11 05:56:27.000000 eth-monitor-0.8.0/eth_monitor/filters/cache.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2121 2023-02-23 02:16:57.000000 eth-monitor-0.8.0/eth_monitor/filters/out.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor/importers/
--rw-r--r--   0 lash      (1000) lash      (1000)     1521 2022-11-11 05:56:27.000000 eth-monitor-0.8.0/eth_monitor/importers/etherscan.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1450 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/index.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/eth_monitor/mock/
--rw-r--r--   0 lash      (1000) lash      (1000)      274 2022-01-30 14:12:19.000000 eth-monitor-0.8.0/eth_monitor/mock/filter_plain.py
--rw-r--r--   0 lash      (1000) lash      (1000)      417 2022-01-30 14:12:19.000000 eth-monitor-0.8.0/eth_monitor/mock/filter_ruled.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4240 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/rules.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/eth_monitor/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     5735 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/runnable/import.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3877 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/runnable/list.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3298 2023-02-26 19:39:52.000000 eth-monitor-0.8.0/eth_monitor/runnable/sync.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5125 2022-01-30 14:12:19.000000 eth-monitor-0.8.0/eth_monitor/runnable/sync_thread_range.py
--rw-r--r--   0 lash      (1000) lash      (1000)    12798 2023-08-06 12:17:19.000000 eth-monitor-0.8.0/eth_monitor/settings.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1237 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      113 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.118382 eth-monitor-0.8.0/man/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/man/build/
--rw-r--r--   0 lash      (1000) lash      (1000)     5946 2023-05-13 20:02:53.000000 eth-monitor-0.8.0/man/build/eth-monitor-import.1
--rw-r--r--   0 lash      (1000) lash      (1000)     5557 2023-05-13 20:02:53.000000 eth-monitor-0.8.0/man/build/eth-monitor-list.1
--rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.0/man/build/eth-monitor-sync.1
--rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.0/man/build/eth-monitor.1
--rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-06 13:08:43.000000 eth-monitor-0.8.0/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1002 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      852 2023-05-13 20:44:09.000000 eth-monitor-0.8.0/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     3524 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/tests/test_basic.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1851 2023-08-06 18:31:42.000000 eth-monitor-0.8.1/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:56:11.000000 eth-monitor-0.8.1/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      110 2023-05-13 20:45:22.000000 eth-monitor-0.8.1/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-06 18:33:29.411679 eth-monitor-0.8.1/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     9706 2023-05-13 20:42:58.000000 eth-monitor-0.8.1/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      871 2022-11-14 07:52:42.000000 eth-monitor-0.8.1/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:55:49.000000 eth-monitor-0.8.1/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.405012 eth-monitor-0.8.1/eth_monitor/
+-rw-r--r--   0 lash      (1000) lash      (1000)      902 2022-11-11 05:56:27.000000 eth-monitor-0.8.1/eth_monitor/callback.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      645 2023-08-06 12:18:29.000000 eth-monitor-0.8.1/eth_monitor/chain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)       65 2022-10-13 07:08:18.000000 eth-monitor-0.8.1/eth_monitor/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3361 2023-08-06 15:43:28.000000 eth-monitor-0.8.1/eth_monitor/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1998 2023-08-06 15:47:56.000000 eth-monitor-0.8.1/eth_monitor/cli/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      518 2022-11-14 07:56:11.000000 eth-monitor-0.8.1/eth_monitor/cli/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      271 2022-10-13 07:08:18.000000 eth-monitor-0.8.1/eth_monitor/cli/rules.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1327 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/config.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.405012 eth-monitor-0.8.1/eth_monitor/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       40 2022-10-13 07:08:18.000000 eth-monitor-0.8.1/eth_monitor/data/config/cache.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-08-06 15:43:41.000000 eth-monitor-0.8.1/eth_monitor/data/config/filter.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)      257 2023-08-06 15:44:01.000000 eth-monitor-0.8.1/eth_monitor/data/config/monitor.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       22 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/data/config/renderer.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       87 2023-08-06 17:24:24.000000 eth-monitor-0.8.1/eth_monitor/driver.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/filters/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-01-30 14:12:19.000000 eth-monitor-0.8.1/eth_monitor/filters/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      580 2023-08-06 16:02:41.000000 eth-monitor-0.8.1/eth_monitor/filters/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      263 2023-08-06 16:02:57.000000 eth-monitor-0.8.1/eth_monitor/filters/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      732 2023-08-06 16:03:10.000000 eth-monitor-0.8.1/eth_monitor/filters/cache.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2121 2023-08-06 16:02:35.000000 eth-monitor-0.8.1/eth_monitor/filters/out.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/importers/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1521 2022-11-11 05:56:27.000000 eth-monitor-0.8.1/eth_monitor/importers/etherscan.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1450 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/index.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/mock/
+-rw-r--r--   0 lash      (1000) lash      (1000)      274 2022-01-30 14:12:19.000000 eth-monitor-0.8.1/eth_monitor/mock/filter_plain.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      417 2022-01-30 14:12:19.000000 eth-monitor-0.8.1/eth_monitor/mock/filter_ruled.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4240 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/rules.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5735 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/runnable/import.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3877 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/eth_monitor/runnable/list.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3382 2023-08-06 16:04:50.000000 eth-monitor-0.8.1/eth_monitor/runnable/sync.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5125 2022-01-30 14:12:19.000000 eth-monitor-0.8.1/eth_monitor/runnable/sync_thread_range.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    13167 2023-08-06 16:04:32.000000 eth-monitor-0.8.1/eth_monitor/settings.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/eth_monitor.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1259 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      113 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-08-06 18:33:29.000000 eth-monitor-0.8.1/eth_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.405012 eth-monitor-0.8.1/man/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/man/build/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5946 2023-05-13 20:02:53.000000 eth-monitor-0.8.1/man/build/eth-monitor-import.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     5557 2023-05-13 20:02:53.000000 eth-monitor-0.8.1/man/build/eth-monitor-list.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.1/man/build/eth-monitor-sync.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.1/man/build/eth-monitor.1
+-rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-06 18:24:22.000000 eth-monitor-0.8.1/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1002 2023-08-06 18:33:29.411679 eth-monitor-0.8.1/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      852 2023-05-13 20:44:09.000000 eth-monitor-0.8.1/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       76 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 18:33:29.408346 eth-monitor-0.8.1/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3524 2022-04-20 19:19:25.000000 eth-monitor-0.8.1/tests/test_basic.py
```

### Comparing `eth-monitor-0.8.0/CHANGELOG` & `eth-monitor-0.8.1/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+- 0.8.1
+	* Implement syncer context
+	* Add key-value parameter for cli, environment, config to pass to syncer context
 - 0.8.0
 	* Implement RPC batch limits for syncer
 - 0.7.6
 	* Make rpc dialect work with chain interface
 - 0.7.5
 	* Add readme (from man page)
 	* Add package descriptino (from man page)
```

### Comparing `eth-monitor-0.8.0/LICENSE` & `eth-monitor-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/PKG-INFO` & `eth-monitor-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-monitor
-Version: 0.8.0
+Version: 0.8.1
 Summary: Monitor and cache transactions using match filters
 Home-page: https://git.defalsify.org/eth-monitor
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-monitor-0.8.0/README.md` & `eth-monitor-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/WAIVER` & `eth-monitor-0.8.1/WAIVER`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/WAIVER.asc` & `eth-monitor-0.8.1/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/callback.py` & `eth-monitor-0.8.1/eth_monitor/callback.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/chain.py` & `eth-monitor-0.8.1/eth_monitor/chain.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/cli/arg.py` & `eth-monitor-0.8.1/eth_monitor/cli/arg.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,7 +26,10 @@
     argparser.add_argument('--filter', type=str, action='append', help='Add python module to tx filter path')
     argparser.add_argument('--block-filter', type=str, dest='block_filter', action='append', help='Add python module to block filter path')
 
     # cache flags
     argparser.add_argument('--store-tx-data', action='store_true', dest='store_tx_data', help='Store tx data in cache store')
     argparser.add_argument('--store-block-data', action='store_true', dest='store_block_data', help='Store block data in cache store')
     argparser.add_argument('--fresh', action='store_true', help='Do not read block and tx data from cache, even if available')
+
+    # misc flags
+    argparser.add_argument('-k', '--context-key', dest='context_key', action='append', type=str, help='Add a key-value pair to be added to the context')
```

### Comparing `eth-monitor-0.8.0/eth_monitor/cli/config.py` & `eth-monitor-0.8.1/eth_monitor/cli/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
     arg_override['ETHMONITOR_RENDERER'] = getattr(args, 'renderer')
     arg_override['ETHMONITOR_FILTER'] = getattr(args, 'filter')
     arg_override['ETHMONITOR_BLOCK_FILTER'] = getattr(args, 'block_filter')
 
     arg_override['ETHMONITOR_STATE_DIR'] = getattr(args, 'state_dir')
 
+    arg_override['ETHMONITOR_CONTEXT_KEY'] = getattr(args, 'context_key')
+
     arg_override['ETHCACHE_STORE_BLOCK'] = getattr(args, 'store_block_data')
     arg_override['ETHCACHE_STORE_TX'] = getattr(args, 'store_tx_data')
 
     config.dict_override(arg_override, 'local cli args')
 
     for rules_arg in rules_args:
         (vy, vn) = to_config_names(rules_arg)
```

### Comparing `eth-monitor-0.8.0/eth_monitor/cli/log.py` & `eth-monitor-0.8.1/eth_monitor/cli/log.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/config.py` & `eth-monitor-0.8.1/eth_monitor/config.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/filters/base.py` & `eth-monitor-0.8.1/eth_monitor/filters/base.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/filters/cache.py` & `eth-monitor-0.8.1/eth_monitor/filters/cache.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/filters/out.py` & `eth-monitor-0.8.1/eth_monitor/filters/out.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/importers/etherscan.py` & `eth-monitor-0.8.1/eth_monitor/importers/etherscan.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/index.py` & `eth-monitor-0.8.1/eth_monitor/index.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/rules.py` & `eth-monitor-0.8.1/eth_monitor/rules.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/runnable/import.py` & `eth-monitor-0.8.1/eth_monitor/runnable/import.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/runnable/list.py` & `eth-monitor-0.8.1/eth_monitor/runnable/list.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/runnable/sync.py` & `eth-monitor-0.8.1/eth_monitor/runnable/sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,35 +81,37 @@
 
 config = Config()
 config.add_schema_dir(config_dir)
 config.add_schema_dir(chainsyncer_config_dir)
 config = process_config(config, arg, args, flags)
 config = process_config_sync(config, arg, args, flags)
 config = eth_monitor.cli.process_config(config, arg, args, flags)
+logg.debug('loaded config:\n{}'.format(config))
 
 settings = ChainSettings()
 settings = process_settings(settings, config)
 settings = process_settings_local(settings, config)
 logg.debug('loaded settings:\n{}'.format(settings))
 
 
 def main():
     logg.info('session is {}'.format(settings.get('SESSION_ID')))
 
+
     drv = ChainInterfaceDriver(
             settings.get('SYNC_STORE'),
             settings.get('SYNCER_INTERFACE'),
             offset=settings.get('SYNCER_OFFSET'),
             target=settings.get('SYNCER_LIMIT'),
             pre_callback=pre_callback,
             post_callback=post_callback,
             block_callback=settings.get('BLOCK_HANDLER').filter,
             )
-    
+   
     try:
-        r = drv.run(settings.get('CONN'))
+        r = drv.run(settings.get('CONN'), ctx=settings.get('SYNCER_CONTEXT'))
     except SyncDone as e:
         sys.stderr.write("sync {} done at block {}\n".format(drv, e))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `eth-monitor-0.8.0/eth_monitor/runnable/sync_thread_range.py` & `eth-monitor-0.8.1/eth_monitor/runnable/sync_thread_range.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/eth_monitor/settings.py` & `eth-monitor-0.8.1/eth_monitor/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,15 +376,29 @@
 
 def process_cache(settings, config):
     settings = process_cache_store(settings, config)
     settings = process_cache_rpc(settings, config)
     return settings
 
 
+def process_user_context(settings, config):
+    ctx_usr = {}
+    for kv in config.get('ETHMONITOR_CONTEXT_KEY'):
+        (k, v) = kv.split('=', 1)
+        ctx_usr[k] = v
+    ctx = {
+        'driver': 'eth-monitor',
+        'usr': ctx_usr,
+            }
+    settings.set('SYNCER_CONTEXT', ctx)
+    return settings
+
+
 def process_settings(settings, config):
     settings = process_monitor_session(settings, config)
     settings = process_monitor_session_dir(settings, config)
     settings = process_arg_rules(settings, config)
     settings = process_sync(settings, config)
     settings = process_cache(settings, config)
+    settings = process_user_context(settings, config)
     settings = process_filter(settings, config)
     return settings
```

### Comparing `eth-monitor-0.8.0/eth_monitor.egg-info/PKG-INFO` & `eth-monitor-0.8.1/eth_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-monitor
-Version: 0.8.0
+Version: 0.8.1
 Summary: Monitor and cache transactions using match filters
 Home-page: https://git.defalsify.org/eth-monitor
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-monitor-0.8.0/eth_monitor.egg-info/SOURCES.txt` & `eth-monitor-0.8.1/eth_monitor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 requirements.txt
 setup.cfg
 setup.py
 test_requirements.txt
 eth_monitor/callback.py
 eth_monitor/chain.py
 eth_monitor/config.py
+eth_monitor/driver.py
 eth_monitor/index.py
 eth_monitor/rules.py
 eth_monitor/settings.py
 eth_monitor.egg-info/PKG-INFO
 eth_monitor.egg-info/SOURCES.txt
 eth_monitor.egg-info/dependency_links.txt
 eth_monitor.egg-info/entry_points.txt
```

### Comparing `eth-monitor-0.8.0/man/build/eth-monitor-import.1` & `eth-monitor-0.8.1/man/build/eth-monitor-import.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/man/build/eth-monitor-list.1` & `eth-monitor-0.8.1/man/build/eth-monitor-list.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/man/build/eth-monitor-sync.1` & `eth-monitor-0.8.1/man/build/eth-monitor-sync.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/man/build/eth-monitor.1` & `eth-monitor-0.8.1/man/build/eth-monitor.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/setup.cfg` & `eth-monitor-0.8.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-monitor
-version = 0.8.0
+version = 0.8.1
 description = Monitor and cache transactions using match filters
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-monitor
 keywords = 
 	dlt
 	blockchain
```

### Comparing `eth-monitor-0.8.0/setup.py` & `eth-monitor-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.0/tests/test_basic.py` & `eth-monitor-0.8.1/tests/test_basic.py`

 * *Files identical despite different names*

