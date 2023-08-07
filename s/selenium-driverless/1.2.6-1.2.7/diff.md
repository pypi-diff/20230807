# Comparing `tmp/selenium_driverless-1.2.6.tar.gz` & `tmp/selenium_driverless-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_driverless-1.2.6.tar", last modified: Thu Aug  3 08:32:13 2023, max compression
+gzip compressed data, was "selenium_driverless-1.2.7.tar", last modified: Mon Aug  7 20:24:53 2023, max compression
```

## Comparing `selenium_driverless-1.2.6.tar` & `selenium_driverless-1.2.7.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.708612 selenium_driverless-1.2.6/
--rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.2.6/LICENSE.md
--rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4508 2023-08-03 08:32:13.709679 selenium_driverless-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3192 2023-08-03 07:34:04.000000 selenium_driverless-1.2.6/README.md
--rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.2.6/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.2.6/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-08-03 08:32:13.710638 selenium_driverless-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     2122 2023-07-26 16:30:17.000000 selenium_driverless-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.536831 selenium_driverless-1.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.548054 selenium_driverless-1.2.6/src/selenium_driverless/
--rw-rw-rw-   0        0        0       23 2023-08-03 08:31:51.000000 selenium_driverless-1.2.6/src/selenium_driverless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.555848 selenium_driverless-1.2.6/src/selenium_driverless/files/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.2.6/src/selenium_driverless/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.562579 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/
--rw-rw-rw-   0        0        0     1176 2023-07-26 16:14:27.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/__init__.py
--rw-rw-rw-   0        0        0    16611 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/asyncio.py
--rw-rw-rw-   0        0        0     1361 2023-07-26 16:14:27.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/base.py
--rw-rw-rw-   0        0        0     7313 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/browser.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.687668 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/
--rw-rw-rw-   0        0        0      798 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/__init__.py
--rw-rw-rw-   0        0        0    23896 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/accessibility.py
--rw-rw-rw-   0        0        0    11602 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/animation.py
--rw-rw-rw-   0        0        0    52280 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/audits.py
--rw-rw-rw-   0        0        0     6066 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/background_service.py
--rw-rw-rw-   0        0        0    21594 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/browser.py
--rw-rw-rw-   0        0        0     8567 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/cache_storage.py
--rw-rw-rw-   0        0        0     4435 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/cast.py
--rw-rw-rw-   0        0        0     2882 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/console.py
--rw-rw-rw-   0        0        0    66950 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/css.py
--rw-rw-rw-   0        0        0     4086 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/database.py
--rw-rw-rw-   0        0        0    52264 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/debugger.py
--rw-rw-rw-   0        0        0     3373 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/device_access.py
--rw-rw-rw-   0        0        0     1154 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/device_orientation.py
--rw-rw-rw-   0        0        0    63790 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/dom.py
--rw-rw-rw-   0        0        0     9800 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/dom_debugger.py
--rw-rw-rw-   0        0        0    40830 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/dom_snapshot.py
--rw-rw-rw-   0        0        0     5935 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/dom_storage.py
--rw-rw-rw-   0        0        0    26766 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/emulation.py
--rw-rw-rw-   0        0        0     1230 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/event_breakpoints.py
--rw-rw-rw-   0        0        0     5466 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/fed_cm.py
--rw-rw-rw-   0        0        0    20431 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/fetch.py
--rw-rw-rw-   0        0        0     4985 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/headless_experimental.py
--rw-rw-rw-   0        0        0    14046 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/heap_profiler.py
--rw-rw-rw-   0        0        0    15583 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/indexed_db.py
--rw-rw-rw-   0        0        0    28365 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/input_.py
--rw-rw-rw-   0        0        0     1712 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/inspector.py
--rw-rw-rw-   0        0        0     2995 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/io.py
--rw-rw-rw-   0        0        0    15942 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/layer_tree.py
--rw-rw-rw-   0        0        0     5784 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/log.py
--rw-rw-rw-   0        0        0     7923 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/media.py
--rw-rw-rw-   0        0        0     7010 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/memory.py
--rw-rw-rw-   0        0        0   135424 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/network.py
--rw-rw-rw-   0        0        0    56704 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/overlay.py
--rw-rw-rw-   0        0        0   109903 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/page.py
--rw-rw-rw-   0        0        0     3080 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/performance.py
--rw-rw-rw-   0        0        0     7184 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/performance_timeline.py
--rw-rw-rw-   0        0        0    15687 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/preload.py
--rw-rw-rw-   0        0        0    13542 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/profiler.py
--rw-rw-rw-   0        0        0    61736 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/runtime.py
--rw-rw-rw-   0        0        0     1143 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/schema.py
--rw-rw-rw-   0        0        0    18042 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/security.py
--rw-rw-rw-   0        0        0    11603 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/service_worker.py
--rw-rw-rw-   0        0        0    36250 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/storage.py
--rw-rw-rw-   0        0        0    12090 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/system_info.py
--rw-rw-rw-   0        0        0    24638 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/target.py
--rw-rw-rw-   0        0        0     1526 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/tethering.py
--rw-rw-rw-   0        0        0    14160 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/tracing.py
--rw-rw-rw-   0        0        0      455 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/util.py
--rw-rw-rw-   0        0        0    18058 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/web_audio.py
--rw-rw-rw-   0        0        0    16287 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/web_authn.py
--rw-rw-rw-   0        0        0     2426 2023-07-26 16:21:09.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/exceptions.py
--rw-rw-rw-   0        0        0    13427 2023-07-26 16:21:08.000000 selenium_driverless-1.2.6/src/selenium_driverless/pycdp/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.692782 selenium_driverless-1.2.6/src/selenium_driverless/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.2.6/src/selenium_driverless/scripts/__init__.py
--rw-rw-rw-   0        0        0     2788 2023-07-26 08:39:43.000000 selenium_driverless-1.2.6/src/selenium_driverless/scripts/alert.py
--rw-rw-rw-   0        0        0    17149 2023-07-26 10:47:31.000000 selenium_driverless-1.2.6/src/selenium_driverless/scripts/options.py
--rw-rw-rw-   0        0        0     5941 2023-08-03 08:16:03.000000 selenium_driverless-1.2.6/src/selenium_driverless/scripts/switch_to.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.700201 selenium_driverless-1.2.6/src/selenium_driverless/sync/
--rw-rw-rw-   0        0        0        0 2023-07-26 11:51:40.000000 selenium_driverless-1.2.6/src/selenium_driverless/sync/__init__.py
--rw-rw-rw-   0        0        0      999 2023-07-26 08:39:43.000000 selenium_driverless-1.2.6/src/selenium_driverless/sync/alert.py
--rw-rw-rw-   0        0        0     1244 2023-07-26 08:40:29.000000 selenium_driverless-1.2.6/src/selenium_driverless/sync/executor.py
--rw-rw-rw-   0        0        0     1015 2023-07-26 08:39:43.000000 selenium_driverless-1.2.6/src/selenium_driverless/sync/switch_to.py
--rw-rw-rw-   0        0        0     1374 2023-07-26 16:34:36.000000 selenium_driverless-1.2.6/src/selenium_driverless/sync/webdriver.py
--rw-rw-rw-   0        0        0     1336 2023-07-26 10:29:29.000000 selenium_driverless-1.2.6/src/selenium_driverless/sync/webelement.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.704221 selenium_driverless-1.2.6/src/selenium_driverless/types/
--rw-rw-rw-   0        0        0     4284 2023-08-03 08:31:23.000000 selenium_driverless-1.2.6/src/selenium_driverless/types/__init__.py
--rw-rw-rw-   0        0        0     1084 2023-07-25 15:39:34.000000 selenium_driverless-1.2.6/src/selenium_driverless/types/by.py
--rw-rw-rw-   0        0        0    14497 2023-07-26 10:28:36.000000 selenium_driverless-1.2.6/src/selenium_driverless/types/webelement.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.706428 selenium_driverless-1.2.6/src/selenium_driverless/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.2.6/src/selenium_driverless/utils/__init__.py
--rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.2.6/src/selenium_driverless/utils/utils.py
--rw-rw-rw-   0        0        0    45694 2023-08-03 07:13:00.000000 selenium_driverless-1.2.6/src/selenium_driverless/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.555453 selenium_driverless-1.2.6/src/selenium_driverless.egg-info/
--rw-rw-rw-   0        0        0     4508 2023-08-03 08:32:13.000000 selenium_driverless-1.2.6/src/selenium_driverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3718 2023-08-03 08:32:13.000000 selenium_driverless-1.2.6/src/selenium_driverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 08:32:13.000000 selenium_driverless-1.2.6/src/selenium_driverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      237 2023-08-03 08:32:13.000000 selenium_driverless-1.2.6/src/selenium_driverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-08-03 08:32:13.000000 selenium_driverless-1.2.6/src/selenium_driverless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 08:32:13.707613 selenium_driverless-1.2.6/tests/
--rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.2.6/tests/test_driverless.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.812308 selenium_driverless-1.2.7/
+-rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.2.7/LICENSE.md
+-rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4508 2023-08-07 20:24:53.812308 selenium_driverless-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3192 2023-08-03 07:34:04.000000 selenium_driverless-1.2.7/README.md
+-rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.2.7/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-08-07 20:24:53.813309 selenium_driverless-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     2122 2023-07-26 16:30:17.000000 selenium_driverless-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.664235 selenium_driverless-1.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.676722 selenium_driverless-1.2.7/src/selenium_driverless/
+-rw-rw-rw-   0        0        0       23 2023-08-07 20:24:48.000000 selenium_driverless-1.2.7/src/selenium_driverless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.686667 selenium_driverless-1.2.7/src/selenium_driverless/files/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.2.7/src/selenium_driverless/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.698920 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/
+-rw-rw-rw-   0        0        0     1176 2023-07-26 16:14:27.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/__init__.py
+-rw-rw-rw-   0        0        0    16611 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/asyncio.py
+-rw-rw-rw-   0        0        0     1361 2023-07-26 16:14:27.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/base.py
+-rw-rw-rw-   0        0        0     7313 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/browser.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.792322 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/
+-rw-rw-rw-   0        0        0      798 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/__init__.py
+-rw-rw-rw-   0        0        0    23896 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/accessibility.py
+-rw-rw-rw-   0        0        0    11602 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/animation.py
+-rw-rw-rw-   0        0        0    52280 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/audits.py
+-rw-rw-rw-   0        0        0     6066 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/background_service.py
+-rw-rw-rw-   0        0        0    21594 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/browser.py
+-rw-rw-rw-   0        0        0     8567 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/cache_storage.py
+-rw-rw-rw-   0        0        0     4435 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/cast.py
+-rw-rw-rw-   0        0        0     2882 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/console.py
+-rw-rw-rw-   0        0        0    66950 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/css.py
+-rw-rw-rw-   0        0        0     4086 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/database.py
+-rw-rw-rw-   0        0        0    52264 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/debugger.py
+-rw-rw-rw-   0        0        0     3373 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/device_access.py
+-rw-rw-rw-   0        0        0     1154 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/device_orientation.py
+-rw-rw-rw-   0        0        0    63790 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/dom.py
+-rw-rw-rw-   0        0        0     9800 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/dom_debugger.py
+-rw-rw-rw-   0        0        0    40830 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/dom_snapshot.py
+-rw-rw-rw-   0        0        0     5935 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/dom_storage.py
+-rw-rw-rw-   0        0        0    26766 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/emulation.py
+-rw-rw-rw-   0        0        0     1230 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/event_breakpoints.py
+-rw-rw-rw-   0        0        0     5466 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/fed_cm.py
+-rw-rw-rw-   0        0        0    20431 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/fetch.py
+-rw-rw-rw-   0        0        0     4985 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/headless_experimental.py
+-rw-rw-rw-   0        0        0    14046 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/heap_profiler.py
+-rw-rw-rw-   0        0        0    15583 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/indexed_db.py
+-rw-rw-rw-   0        0        0    28365 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/input_.py
+-rw-rw-rw-   0        0        0     1712 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/inspector.py
+-rw-rw-rw-   0        0        0     2995 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/io.py
+-rw-rw-rw-   0        0        0    15942 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/layer_tree.py
+-rw-rw-rw-   0        0        0     5784 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/log.py
+-rw-rw-rw-   0        0        0     7923 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/media.py
+-rw-rw-rw-   0        0        0     7010 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/memory.py
+-rw-rw-rw-   0        0        0   135424 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/network.py
+-rw-rw-rw-   0        0        0    56704 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/overlay.py
+-rw-rw-rw-   0        0        0   109903 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/page.py
+-rw-rw-rw-   0        0        0     3080 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/performance.py
+-rw-rw-rw-   0        0        0     7184 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/performance_timeline.py
+-rw-rw-rw-   0        0        0    15687 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/preload.py
+-rw-rw-rw-   0        0        0    13542 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/profiler.py
+-rw-rw-rw-   0        0        0    61736 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/runtime.py
+-rw-rw-rw-   0        0        0     1143 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/schema.py
+-rw-rw-rw-   0        0        0    18042 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/security.py
+-rw-rw-rw-   0        0        0    11603 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/service_worker.py
+-rw-rw-rw-   0        0        0    36250 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/storage.py
+-rw-rw-rw-   0        0        0    12090 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/system_info.py
+-rw-rw-rw-   0        0        0    24638 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/target.py
+-rw-rw-rw-   0        0        0     1526 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/tethering.py
+-rw-rw-rw-   0        0        0    14160 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/tracing.py
+-rw-rw-rw-   0        0        0      455 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/util.py
+-rw-rw-rw-   0        0        0    18058 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/web_audio.py
+-rw-rw-rw-   0        0        0    16287 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/web_authn.py
+-rw-rw-rw-   0        0        0     2426 2023-07-26 16:21:09.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/exceptions.py
+-rw-rw-rw-   0        0        0    13427 2023-07-26 16:21:08.000000 selenium_driverless-1.2.7/src/selenium_driverless/pycdp/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.797324 selenium_driverless-1.2.7/src/selenium_driverless/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.2.7/src/selenium_driverless/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2788 2023-07-26 08:39:43.000000 selenium_driverless-1.2.7/src/selenium_driverless/scripts/alert.py
+-rw-rw-rw-   0        0        0    16988 2023-08-07 20:19:03.000000 selenium_driverless-1.2.7/src/selenium_driverless/scripts/options.py
+-rw-rw-rw-   0        0        0     5941 2023-08-03 08:16:03.000000 selenium_driverless-1.2.7/src/selenium_driverless/scripts/switch_to.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.804309 selenium_driverless-1.2.7/src/selenium_driverless/sync/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:51:40.000000 selenium_driverless-1.2.7/src/selenium_driverless/sync/__init__.py
+-rw-rw-rw-   0        0        0      999 2023-07-26 08:39:43.000000 selenium_driverless-1.2.7/src/selenium_driverless/sync/alert.py
+-rw-rw-rw-   0        0        0     1244 2023-07-26 08:40:29.000000 selenium_driverless-1.2.7/src/selenium_driverless/sync/executor.py
+-rw-rw-rw-   0        0        0     1015 2023-07-26 08:39:43.000000 selenium_driverless-1.2.7/src/selenium_driverless/sync/switch_to.py
+-rw-rw-rw-   0        0        0     1374 2023-07-26 16:34:36.000000 selenium_driverless-1.2.7/src/selenium_driverless/sync/webdriver.py
+-rw-rw-rw-   0        0        0     1336 2023-07-26 10:29:29.000000 selenium_driverless-1.2.7/src/selenium_driverless/sync/webelement.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.808308 selenium_driverless-1.2.7/src/selenium_driverless/types/
+-rw-rw-rw-   0        0        0     4284 2023-08-03 08:31:23.000000 selenium_driverless-1.2.7/src/selenium_driverless/types/__init__.py
+-rw-rw-rw-   0        0        0     1084 2023-07-25 15:39:34.000000 selenium_driverless-1.2.7/src/selenium_driverless/types/by.py
+-rw-rw-rw-   0        0        0    14497 2023-07-26 10:28:36.000000 selenium_driverless-1.2.7/src/selenium_driverless/types/webelement.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.810310 selenium_driverless-1.2.7/src/selenium_driverless/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.2.7/src/selenium_driverless/utils/__init__.py
+-rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.2.7/src/selenium_driverless/utils/utils.py
+-rw-rw-rw-   0        0        0    46006 2023-08-07 20:19:03.000000 selenium_driverless-1.2.7/src/selenium_driverless/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.684663 selenium_driverless-1.2.7/src/selenium_driverless.egg-info/
+-rw-rw-rw-   0        0        0     4508 2023-08-07 20:24:53.000000 selenium_driverless-1.2.7/src/selenium_driverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3718 2023-08-07 20:24:53.000000 selenium_driverless-1.2.7/src/selenium_driverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 20:24:53.000000 selenium_driverless-1.2.7/src/selenium_driverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      237 2023-08-07 20:24:53.000000 selenium_driverless-1.2.7/src/selenium_driverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-07 20:24:53.000000 selenium_driverless-1.2.7/src/selenium_driverless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 20:24:53.811309 selenium_driverless-1.2.7/tests/
+-rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.2.7/tests/test_driverless.py
```

### Comparing `selenium_driverless-1.2.6/LICENSE.md` & `selenium_driverless-1.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/PKG-INFO` & `selenium_driverless-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_driverless
-Version: 1.2.6
+Version: 1.2.7
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
```

### Comparing `selenium_driverless-1.2.6/README.md` & `selenium_driverless-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/build_upload.md` & `selenium_driverless-1.2.7/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/setup.py` & `selenium_driverless-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/__init__.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/asyncio.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/asyncio.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/base.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/base.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/browser.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/browser.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/__init__.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/accessibility.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/accessibility.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/animation.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/animation.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/audits.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/audits.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/background_service.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/background_service.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/browser.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/browser.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/cache_storage.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/cache_storage.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/cast.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/cast.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/console.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/console.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/css.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/css.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/database.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/database.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/debugger.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/debugger.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/device_access.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/device_access.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/device_orientation.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/device_orientation.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/dom.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/dom.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/dom_debugger.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/dom_debugger.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/dom_snapshot.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/dom_storage.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/dom_storage.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/emulation.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/emulation.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/event_breakpoints.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/event_breakpoints.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/fed_cm.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/fed_cm.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/fetch.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/fetch.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/headless_experimental.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/headless_experimental.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/heap_profiler.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/heap_profiler.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/indexed_db.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/indexed_db.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/input_.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/input_.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/inspector.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/inspector.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/io.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/io.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/layer_tree.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/layer_tree.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/log.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/log.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/media.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/media.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/memory.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/memory.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/network.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/network.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/overlay.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/overlay.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/page.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/page.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/performance.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/performance.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/performance_timeline.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/performance_timeline.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/preload.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/preload.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/profiler.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/profiler.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/runtime.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/runtime.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/schema.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/schema.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/security.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/security.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/service_worker.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/service_worker.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/storage.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/storage.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/system_info.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/system_info.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/target.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/target.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/tethering.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/tethering.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/tracing.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/tracing.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/web_audio.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/web_audio.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/cdp/web_authn.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/cdp/web_authn.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/exceptions.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/exceptions.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/pycdp/utils.py` & `selenium_driverless-1.2.7/src/selenium_driverless/pycdp/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/scripts/alert.py` & `selenium_driverless-1.2.7/src/selenium_driverless/scripts/alert.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/scripts/options.py` & `selenium_driverless-1.2.7/src/selenium_driverless/scripts/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,31 +29,29 @@
 
 
 # noinspection PyUnreachableCode
 class Options(metaclass=ABCMeta):
     KEY = "goog:chromeOptions"
 
     def __init__(self) -> None:
-        from selenium_driverless.utils.utils import find_chrome_executable, sel_driverless_path, random_port
-        import uuid
+        from selenium_driverless.utils.utils import find_chrome_executable
         super().__init__()
 
         self._caps = self.default_capabilities
         self._proxy = None
         # self.set_capability("pageLoadStrategy", "normal")
         self.mobile_options = None
 
         self._binary_location = find_chrome_executable()
         self._extension_files = []
         self._extensions = []
         self._experimental_options = {}
         self._debugger_address = None
         self.user_data_dir = None
         self._arguments = []
-        self.add_argument("--user-data-dir=" + sel_driverless_path() + "/files/tmp/" + uuid.uuid4().hex)
         self._ignore_local_proxy = False
 
     @property
     def capabilities(self):
         return self._caps
 
     def set_capability(self, name: str, value: dict) -> None:
```

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/scripts/switch_to.py` & `selenium_driverless-1.2.7/src/selenium_driverless/scripts/switch_to.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/sync/alert.py` & `selenium_driverless-1.2.7/src/selenium_driverless/sync/alert.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/sync/executor.py` & `selenium_driverless-1.2.7/src/selenium_driverless/sync/executor.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/sync/switch_to.py` & `selenium_driverless-1.2.7/src/selenium_driverless/sync/switch_to.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/sync/webdriver.py` & `selenium_driverless-1.2.7/src/selenium_driverless/sync/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/sync/webelement.py` & `selenium_driverless-1.2.7/src/selenium_driverless/sync/webelement.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/types/__init__.py` & `selenium_driverless-1.2.7/src/selenium_driverless/types/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/types/by.py` & `selenium_driverless-1.2.7/src/selenium_driverless/types/by.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/types/webelement.py` & `selenium_driverless-1.2.7/src/selenium_driverless/types/webelement.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/utils/utils.py` & `selenium_driverless-1.2.7/src/selenium_driverless/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless/webdriver.py` & `selenium_driverless-1.2.7/src/selenium_driverless/webdriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,18 @@
         self._script_timeout = 30
         self._conn = None
         self.session = None
         self.browser_pid = None
         if not options.binary_location:
             from selenium_driverless.utils.utils import find_chrome_executable
             options.binary_location = find_chrome_executable()
+        if not options.user_data_dir:
+            from selenium_driverless.utils.utils import sel_driverless_path
+            import uuid
+            options.add_argument("--user-data-dir=" + sel_driverless_path() + "/files/tmp/" + uuid.uuid4().hex)
 
         try:
             options = options or ChromeOptions()
             self._options = options
 
             vendor_prefix = "goog"
             self.vendor_prefix = vendor_prefix
@@ -470,18 +474,19 @@
         """Returns the handles of all windows within the current session.
 
         :Usage:
             ::
 
                 driver.window_handles
         """
+        warnings.warn("window_handles aren't ordered")
         tabs = []
         for target in await self.targets:
             if target["type"] == "page":
-                tabs.append(target.target_id)
+                tabs.append(target['targetId'])
         return tabs
 
     async def set_window_state(self, state):
         states = ["normal", "minimized", "maximized", "fullscreen"]
         if state not in states:
             raise ValueError(f"expected one of {states}, but got: {state}")
         window_id = await self.current_window_id
```

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless.egg-info/PKG-INFO` & `selenium_driverless-1.2.7/src/selenium_driverless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-driverless
-Version: 1.2.6
+Version: 1.2.7
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
```

### Comparing `selenium_driverless-1.2.6/src/selenium_driverless.egg-info/SOURCES.txt` & `selenium_driverless-1.2.7/src/selenium_driverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.2.6/tests/test_driverless.py` & `selenium_driverless-1.2.7/tests/test_driverless.py`

 * *Files identical despite different names*

