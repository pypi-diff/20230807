# Comparing `tmp/hyperiontf-0.1.0.tar.gz` & `tmp/hyperiontf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperiontf-0.1.0.tar", max compression
+gzip compressed data, was "hyperiontf-0.1.1.tar", max compression
```

## Comparing `hyperiontf-0.1.0.tar` & `hyperiontf-0.1.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0    11357 2023-06-07 09:52:02.135416 hyperiontf-0.1.0/LICENSE
--rw-r--r--   0        0        0    49280 2023-08-06 13:15:08.525191 hyperiontf-0.1.0/README.md
--rw-r--r--   0        0        0      490 2023-08-06 19:44:31.079188 hyperiontf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      708 2023-08-06 13:15:10.362541 hyperiontf-0.1.0/src/hyperiontf/__init__.py
--rw-r--r--   0        0        0       61 2023-08-06 13:15:10.005244 hyperiontf-0.1.0/src/hyperiontf/api/__init__.py
--rw-r--r--   0        0        0        1 2023-08-06 13:15:08.363268 hyperiontf-0.1.0/src/hyperiontf/api/rest_client/__init__.py
--rw-r--r--   0        0        0    28236 2023-08-06 13:15:10.199857 hyperiontf-0.1.0/src/hyperiontf/api/rest_client/client.py
--rw-r--r--   0        0        0    15718 2023-08-06 13:15:10.363042 hyperiontf-0.1.0/src/hyperiontf/api/rest_client/request.py
--rw-r--r--   0        0        0    11597 2023-08-06 14:28:28.490716 hyperiontf-0.1.0/src/hyperiontf/api/rest_client/response.py
--rw-r--r--   0        0        0       59 2023-08-06 13:15:10.007556 hyperiontf-0.1.0/src/hyperiontf/assertions/__init__.py
--rw-r--r--   0        0        0    81215 2023-08-06 13:15:10.008221 hyperiontf-0.1.0/src/hyperiontf/assertions/expect.py
--rw-r--r--   0        0        0      433 2023-08-06 13:15:07.885551 hyperiontf-0.1.0/src/hyperiontf/assertions/failed_expectation.py
--rw-r--r--   0        0        0     4401 2023-08-06 13:15:10.009527 hyperiontf-0.1.0/src/hyperiontf/assertions/logging_helper.py
--rw-r--r--   0        0        0       49 2023-08-06 13:15:10.009936 hyperiontf-0.1.0/src/hyperiontf/configuration/__init__.py
--rw-r--r--   0        0        0      739 2023-08-06 13:15:10.010411 hyperiontf-0.1.0/src/hyperiontf/configuration/capabilities.py
--rw-r--r--   0        0        0     3316 2023-08-06 13:15:10.010836 hyperiontf-0.1.0/src/hyperiontf/configuration/config.py
--rw-r--r--   0        0        0     1295 2023-08-06 13:15:08.044291 hyperiontf-0.1.0/src/hyperiontf/configuration/section.py
--rw-r--r--   0        0        0      417 2023-08-06 13:15:10.011128 hyperiontf-0.1.0/src/hyperiontf/configuration/sections/__init__.py
--rw-r--r--   0        0        0      403 2023-08-06 13:15:10.011444 hyperiontf-0.1.0/src/hyperiontf/configuration/sections/desktop_capabilities.py
--rw-r--r--   0        0        0      328 2023-08-06 13:15:10.201719 hyperiontf-0.1.0/src/hyperiontf/configuration/sections/element.py
--rw-r--r--   0        0        0      309 2023-08-06 13:15:10.011696 hyperiontf-0.1.0/src/hyperiontf/configuration/sections/logger.py
--rw-r--r--   0        0        0      456 2023-08-06 13:15:10.012034 hyperiontf-0.1.0/src/hyperiontf/configuration/sections/mobile_capabilities.py
--rw-r--r--   0        0        0      437 2023-08-07 05:28:53.977479 hyperiontf-0.1.0/src/hyperiontf/configuration/sections/page_object.py
--rw-r--r--   0        0        0      397 2023-08-06 13:15:10.012438 hyperiontf-0.1.0/src/hyperiontf/configuration/sections/rest.py
--rw-r--r--   0        0        0      772 2023-08-06 19:44:30.298527 hyperiontf-0.1.0/src/hyperiontf/configuration/sections/web_capabilities.py
--rw-r--r--   0        0        0        0 2023-07-15 18:30:45.192468 hyperiontf-0.1.0/src/hyperiontf/executors/__init__.py
--rw-r--r--   0        0        0      122 2023-08-06 13:15:10.013428 hyperiontf-0.1.0/src/hyperiontf/executors/pytest/__init__.py
--rw-r--r--   0        0        0     3607 2023-08-06 13:15:10.013788 hyperiontf-0.1.0/src/hyperiontf/executors/pytest/fixture.py
--rw-r--r--   0        0        0     2099 2023-08-06 13:15:10.364005 hyperiontf-0.1.0/src/hyperiontf/executors/pytest/logger_setup.py
--rw-r--r--   0        0        0        0 2023-07-10 17:58:35.974283 hyperiontf-0.1.0/src/hyperiontf/helpers/__init__.py
--rw-r--r--   0        0        0       58 2023-08-06 13:15:10.014709 hyperiontf-0.1.0/src/hyperiontf/helpers/decorators/__init__.py
--rw-r--r--   0        0        0      504 2023-08-06 13:15:08.682230 hyperiontf-0.1.0/src/hyperiontf/helpers/decorators/singleton.py
--rw-r--r--   0        0        0     2467 2023-08-06 13:15:10.015303 hyperiontf-0.1.0/src/hyperiontf/helpers/decorators/without_failure.py
--rw-r--r--   0        0        0      974 2023-08-06 13:15:10.015771 hyperiontf-0.1.0/src/hyperiontf/helpers/dict_heplers.py
--rw-r--r--   0        0        0      792 2023-07-22 20:25:42.778503 hyperiontf-0.1.0/src/hyperiontf/helpers/extend_instance.py
--rw-r--r--   0        0        0     1760 2023-08-06 13:15:10.016237 hyperiontf-0.1.0/src/hyperiontf/helpers/own_methods_helper.py
--rw-r--r--   0        0        0     3006 2023-08-06 13:15:10.016701 hyperiontf-0.1.0/src/hyperiontf/helpers/string_helpers.py
--rw-r--r--   0        0        0        0 2023-08-06 13:15:08.204691 hyperiontf-0.1.0/src/hyperiontf/infrastructure/__init__.py
--rw-r--r--   0        0        0     1725 2023-08-06 13:15:08.205946 hyperiontf-0.1.0/src/hyperiontf/infrastructure/event_blorker.py
--rw-r--r--   0        0        0       92 2023-08-06 13:15:10.016997 hyperiontf-0.1.0/src/hyperiontf/logging/__init__.py
--rwxr-xr-x   0        0        0     2674 2023-08-06 13:15:09.344004 hyperiontf-0.1.0/src/hyperiontf/logging/assets/build
--rw-r--r--   0        0        0      935 2023-07-10 10:40:17.706358 hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/button-border-colors.css
--rw-r--r--   0        0        0      252 2023-07-10 11:29:08.272140 hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/button.css
--rw-r--r--   0        0        0      665 2023-07-10 13:21:46.590375 hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/colors.css
--rw-r--r--   0        0        0      392 2023-07-11 12:54:22.880992 hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/filter-bar.css
--rw-r--r--   0        0        0     1048 2023-07-10 17:15:00.496119 hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/header.css
--rw-r--r--   0        0        0     1677 2023-07-10 10:04:40.127802 hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/icon-color-filters.css
--rw-r--r--   0        0        0    38307 2023-07-10 09:52:33.600890 hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/icon-images.css
--rw-r--r--   0        0        0      285 2023-07-31 09:17:20.506222 hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/icon.css
--rw-r--r--   0        0        0     2496 2023-08-06 13:15:09.344424 hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/log-message.css
--rw-r--r--   0        0        0      135 2023-08-06 13:15:09.344901 hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/misc.css
--rw-r--r--   0        0        0      884 2023-07-10 10:06:36.432340 hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/tooltip.css
--rw-r--r--   0        0        0      939 2023-07-22 18:34:53.423179 hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/app.js
--rw-r--r--   0        0        0     4974 2023-07-22 18:41:01.660413 hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/config.js
--rw-r--r--   0        0        0    11226 2023-07-22 18:51:41.092386 hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/controlPanel.js
--rw-r--r--   0        0        0     1356 2023-07-22 18:52:20.196646 hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/eventBroker.js
--rw-r--r--   0        0        0     2136 2023-07-22 18:39:46.004817 hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/helpers.js
--rw-r--r--   0        0        0    40401 2023-07-23 18:26:33.930932 hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/line.js
--rw-r--r--   0        0        0     5490 2023-07-22 18:53:19.430887 hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/logger.js
--rw-r--r--   0        0        0     1192 2023-07-07 17:51:23.600370 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/assert-true.svg
--rw-r--r--   0        0        0     2530 2023-07-08 11:52:51.914244 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/backtrace.svg
--rw-r--r--   0        0        0     1424 2023-07-07 16:58:01.309327 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/collapse.svg
--rw-r--r--   0        0        0      724 2023-07-07 18:40:17.626629 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/column.svg
--rw-r--r--   0        0        0     1936 2023-07-07 17:33:04.167792 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/debug.svg
--rw-r--r--   0        0        0     1371 2023-07-07 17:56:05.231809 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/error.svg
--rw-r--r--   0        0        0     1432 2023-07-07 16:57:55.270184 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/expand.svg
--rw-r--r--   0        0        0     3067 2023-07-07 17:34:19.284839 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/fatal.svg
--rw-r--r--   0        0        0     1852 2023-07-07 16:57:50.469467 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/info.svg
--rw-r--r--   0        0        0      615 2023-07-09 18:17:36.072536 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/level.svg
--rw-r--r--   0        0        0     2582 2023-07-07 18:42:27.638468 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/log.svg
--rw-r--r--   0        0        0     1347 2023-07-07 16:57:43.685179 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/page-source.svg
--rw-r--r--   0        0        0      847 2023-07-07 16:47:23.669853 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/screen-snap.svg
--rw-r--r--   0        0        0     3786 2023-07-09 18:15:54.736465 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/timestamp.svg
--rw-r--r--   0        0        0     2555 2023-07-07 16:57:36.968802 hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/warning.svg
--rw-r--r--   0        0        0    67094 2023-08-06 13:15:09.346258 hyperiontf-0.1.0/src/hyperiontf/logging/assets/template.html
--rw-r--r--   0        0        0     2485 2023-08-06 13:15:10.017426 hyperiontf-0.1.0/src/hyperiontf/logging/file_handler.py
--rw-r--r--   0        0        0     4522 2023-08-06 13:15:10.017972 hyperiontf-0.1.0/src/hyperiontf/logging/formatter.py
--rw-r--r--   0        0        0      715 2023-08-06 13:15:10.018484 hyperiontf-0.1.0/src/hyperiontf/logging/helpers.py
--rw-r--r--   0        0        0     1605 2023-08-06 13:15:10.018911 hyperiontf-0.1.0/src/hyperiontf/logging/log_depth_manager.py
--rw-r--r--   0        0        0     2115 2023-08-06 13:15:10.019380 hyperiontf-0.1.0/src/hyperiontf/logging/log_file_manager.py
--rw-r--r--   0        0        0     4642 2023-08-06 13:15:10.019898 hyperiontf-0.1.0/src/hyperiontf/logging/logger.py
--rw-r--r--   0        0        0    10946 2023-08-06 19:44:30.298964 hyperiontf-0.1.0/src/hyperiontf/typing.py
--rw-r--r--   0        0        0      793 2023-08-06 13:15:10.020879 hyperiontf-0.1.0/src/hyperiontf/ui/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 19:02:44.977919 hyperiontf-0.1.0/src/hyperiontf/ui/appium/__init__.py
--rw-r--r--   0        0        0     8351 2023-08-06 13:15:10.021412 hyperiontf-0.1.0/src/hyperiontf/ui/appium/element.py
--rw-r--r--   0        0        0     1212 2023-08-06 13:15:10.022046 hyperiontf-0.1.0/src/hyperiontf/ui/appium/map_exception.py
--rw-r--r--   0        0        0     1689 2023-08-06 13:15:09.016216 hyperiontf-0.1.0/src/hyperiontf/ui/appium/map_locator.py
--rw-r--r--   0        0        0     4574 2023-08-06 13:15:10.364910 hyperiontf-0.1.0/src/hyperiontf/ui/appium/page.py
--rw-r--r--   0        0        0     7019 2023-08-06 19:44:30.925158 hyperiontf-0.1.0/src/hyperiontf/ui/automation_adapter_manager.py
--rw-r--r--   0        0        0     6647 2023-08-06 13:15:10.023213 hyperiontf-0.1.0/src/hyperiontf/ui/by.py
--rw-r--r--   0        0        0     4421 2023-08-06 13:15:10.202136 hyperiontf-0.1.0/src/hyperiontf/ui/content_manager.py
--rw-r--r--   0        0        0     3285 2023-08-06 13:15:10.202654 hyperiontf-0.1.0/src/hyperiontf/ui/context_manager.py
--rw-r--r--   0        0        0        0 2023-06-08 12:54:44.538706 hyperiontf-0.1.0/src/hyperiontf/ui/decorators/__init__.py
--rw-r--r--   0        0        0     5234 2023-08-06 13:15:10.365843 hyperiontf-0.1.0/src/hyperiontf/ui/decorators/autolog_class_method_helper.py
--rw-r--r--   0        0        0     4826 2023-08-06 13:15:10.024896 hyperiontf-0.1.0/src/hyperiontf/ui/decorators/element_accessor.py
--rw-r--r--   0        0        0     2299 2023-08-06 13:15:10.025410 hyperiontf-0.1.0/src/hyperiontf/ui/decorators/element_error_recovery.py
--rw-r--r--   0        0        0     9074 2023-08-06 13:15:10.203200 hyperiontf-0.1.0/src/hyperiontf/ui/decorators/page_object_helpers.py
--rw-r--r--   0        0        0     1424 2023-08-06 13:15:10.203631 hyperiontf-0.1.0/src/hyperiontf/ui/desktop_window.py
--rw-r--r--   0        0        0     5475 2023-08-06 13:15:10.026968 hyperiontf-0.1.0/src/hyperiontf/ui/element.py
--rw-r--r--   0        0        0     1618 2023-08-06 13:15:10.204107 hyperiontf-0.1.0/src/hyperiontf/ui/elements.py
--rw-r--r--   0        0        0      860 2023-08-06 13:15:10.204538 hyperiontf-0.1.0/src/hyperiontf/ui/iframe.py
--rw-r--r--   0        0        0    18002 2023-08-06 19:44:31.236288 hyperiontf-0.1.0/src/hyperiontf/ui/locatable.py
--rw-r--r--   0        0        0     1505 2023-08-06 13:15:10.028857 hyperiontf-0.1.0/src/hyperiontf/ui/mobile_screen.py
--rw-r--r--   0        0        0     1233 2023-08-06 13:15:10.029221 hyperiontf-0.1.0/src/hyperiontf/ui/page_object_base.py
--rw-r--r--   0        0        0        0 2023-07-14 16:41:57.247681 hyperiontf-0.1.0/src/hyperiontf/ui/playwright/__init__.py
--rw-r--r--   0        0        0     1871 2023-08-06 13:15:10.029599 hyperiontf-0.1.0/src/hyperiontf/ui/playwright/assert_stale_element_reference.py
--rw-r--r--   0        0        0    11380 2023-08-06 13:15:10.366325 hyperiontf-0.1.0/src/hyperiontf/ui/playwright/element.py
--rw-r--r--   0        0        0      938 2023-08-06 19:44:31.079616 hyperiontf-0.1.0/src/hyperiontf/ui/playwright/map_exception.py
--rw-r--r--   0        0        0      981 2023-08-06 13:15:09.516703 hyperiontf-0.1.0/src/hyperiontf/ui/playwright/map_locator.py
--rw-r--r--   0        0        0     5558 2023-08-06 13:15:10.366881 hyperiontf-0.1.0/src/hyperiontf/ui/playwright/page.py
--rw-r--r--   0        0        0     1693 2023-08-06 13:15:10.031077 hyperiontf-0.1.0/src/hyperiontf/ui/playwright/selenium_to_playwright_script.py
--rw-r--r--   0        0        0        0 2023-08-06 13:15:09.021587 hyperiontf-0.1.0/src/hyperiontf/ui/selenium/__init__.py
--rw-r--r--   0        0        0     9708 2023-08-06 13:15:10.031416 hyperiontf-0.1.0/src/hyperiontf/ui/selenium/element.py
--rw-r--r--   0        0        0     1268 2023-08-06 19:44:31.236456 hyperiontf-0.1.0/src/hyperiontf/ui/selenium/map_exception.py
--rw-r--r--   0        0        0      993 2023-08-06 13:15:08.852673 hyperiontf-0.1.0/src/hyperiontf/ui/selenium/map_locator.py
--rw-r--r--   0        0        0     9180 2023-08-07 05:28:53.977937 hyperiontf-0.1.0/src/hyperiontf/ui/selenium/page.py
--rw-r--r--   0        0        0     6876 2023-08-06 13:15:10.032439 hyperiontf-0.1.0/src/hyperiontf/ui/viewport_manager.py
--rw-r--r--   0        0        0     2242 2023-08-07 05:28:53.978465 hyperiontf-0.1.0/src/hyperiontf/ui/webpage.py
--rw-r--r--   0        0        0     1533 2023-08-06 13:15:10.206097 hyperiontf-0.1.0/src/hyperiontf/ui/webview.py
--rw-r--r--   0        0        0      394 2023-08-06 13:15:10.033569 hyperiontf-0.1.0/src/hyperiontf/ui/widget.py
--rw-r--r--   0        0        0     3728 2023-08-06 13:15:10.206600 hyperiontf-0.1.0/src/hyperiontf/ui/window_manager.py
--rw-r--r--   0        0        0    49965 1970-01-01 00:00:00.000000 hyperiontf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-07 09:52:02.135416 hyperiontf-0.1.1/LICENSE
+-rw-r--r--   0        0        0    49280 2023-08-06 13:15:08.525191 hyperiontf-0.1.1/README.md
+-rw-r--r--   0        0        0      490 2023-08-07 11:59:53.913016 hyperiontf-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      708 2023-08-06 13:15:10.362541 hyperiontf-0.1.1/src/hyperiontf/__init__.py
+-rw-r--r--   0        0        0       61 2023-08-06 13:15:10.005244 hyperiontf-0.1.1/src/hyperiontf/api/__init__.py
+-rw-r--r--   0        0        0        1 2023-08-06 13:15:08.363268 hyperiontf-0.1.1/src/hyperiontf/api/rest_client/__init__.py
+-rw-r--r--   0        0        0    28236 2023-08-06 13:15:10.199857 hyperiontf-0.1.1/src/hyperiontf/api/rest_client/client.py
+-rw-r--r--   0        0        0    15718 2023-08-06 13:15:10.363042 hyperiontf-0.1.1/src/hyperiontf/api/rest_client/request.py
+-rw-r--r--   0        0        0    11597 2023-08-07 11:59:13.321728 hyperiontf-0.1.1/src/hyperiontf/api/rest_client/response.py
+-rw-r--r--   0        0        0       59 2023-08-06 13:15:10.007556 hyperiontf-0.1.1/src/hyperiontf/assertions/__init__.py
+-rw-r--r--   0        0        0    81215 2023-08-06 13:15:10.008221 hyperiontf-0.1.1/src/hyperiontf/assertions/expect.py
+-rw-r--r--   0        0        0      433 2023-08-06 13:15:07.885551 hyperiontf-0.1.1/src/hyperiontf/assertions/failed_expectation.py
+-rw-r--r--   0        0        0     4401 2023-08-06 13:15:10.009527 hyperiontf-0.1.1/src/hyperiontf/assertions/logging_helper.py
+-rw-r--r--   0        0        0       49 2023-08-06 13:15:10.009936 hyperiontf-0.1.1/src/hyperiontf/configuration/__init__.py
+-rw-r--r--   0        0        0      739 2023-08-06 13:15:10.010411 hyperiontf-0.1.1/src/hyperiontf/configuration/capabilities.py
+-rw-r--r--   0        0        0     3316 2023-08-06 13:15:10.010836 hyperiontf-0.1.1/src/hyperiontf/configuration/config.py
+-rw-r--r--   0        0        0     1295 2023-08-06 13:15:08.044291 hyperiontf-0.1.1/src/hyperiontf/configuration/section.py
+-rw-r--r--   0        0        0      417 2023-08-06 13:15:10.011128 hyperiontf-0.1.1/src/hyperiontf/configuration/sections/__init__.py
+-rw-r--r--   0        0        0      403 2023-08-06 13:15:10.011444 hyperiontf-0.1.1/src/hyperiontf/configuration/sections/desktop_capabilities.py
+-rw-r--r--   0        0        0      328 2023-08-06 13:15:10.201719 hyperiontf-0.1.1/src/hyperiontf/configuration/sections/element.py
+-rw-r--r--   0        0        0      309 2023-08-06 13:15:10.011696 hyperiontf-0.1.1/src/hyperiontf/configuration/sections/logger.py
+-rw-r--r--   0        0        0      456 2023-08-06 13:15:10.012034 hyperiontf-0.1.1/src/hyperiontf/configuration/sections/mobile_capabilities.py
+-rw-r--r--   0        0        0      437 2023-08-07 11:59:13.322102 hyperiontf-0.1.1/src/hyperiontf/configuration/sections/page_object.py
+-rw-r--r--   0        0        0      397 2023-08-06 13:15:10.012438 hyperiontf-0.1.1/src/hyperiontf/configuration/sections/rest.py
+-rw-r--r--   0        0        0      772 2023-08-07 11:59:13.322553 hyperiontf-0.1.1/src/hyperiontf/configuration/sections/web_capabilities.py
+-rw-r--r--   0        0        0        0 2023-07-15 18:30:45.192468 hyperiontf-0.1.1/src/hyperiontf/executors/__init__.py
+-rw-r--r--   0        0        0      122 2023-08-06 13:15:10.013428 hyperiontf-0.1.1/src/hyperiontf/executors/pytest/__init__.py
+-rw-r--r--   0        0        0     3607 2023-08-06 13:15:10.013788 hyperiontf-0.1.1/src/hyperiontf/executors/pytest/fixture.py
+-rw-r--r--   0        0        0     2099 2023-08-06 13:15:10.364005 hyperiontf-0.1.1/src/hyperiontf/executors/pytest/logger_setup.py
+-rw-r--r--   0        0        0        0 2023-07-10 17:58:35.974283 hyperiontf-0.1.1/src/hyperiontf/helpers/__init__.py
+-rw-r--r--   0        0        0       58 2023-08-06 13:15:10.014709 hyperiontf-0.1.1/src/hyperiontf/helpers/decorators/__init__.py
+-rw-r--r--   0        0        0      504 2023-08-06 13:15:08.682230 hyperiontf-0.1.1/src/hyperiontf/helpers/decorators/singleton.py
+-rw-r--r--   0        0        0     2467 2023-08-06 13:15:10.015303 hyperiontf-0.1.1/src/hyperiontf/helpers/decorators/without_failure.py
+-rw-r--r--   0        0        0      974 2023-08-06 13:15:10.015771 hyperiontf-0.1.1/src/hyperiontf/helpers/dict_heplers.py
+-rw-r--r--   0        0        0      792 2023-07-22 20:25:42.778503 hyperiontf-0.1.1/src/hyperiontf/helpers/extend_instance.py
+-rw-r--r--   0        0        0     1760 2023-08-06 13:15:10.016237 hyperiontf-0.1.1/src/hyperiontf/helpers/own_methods_helper.py
+-rw-r--r--   0        0        0     3006 2023-08-06 13:15:10.016701 hyperiontf-0.1.1/src/hyperiontf/helpers/string_helpers.py
+-rw-r--r--   0        0        0        0 2023-08-06 13:15:08.204691 hyperiontf-0.1.1/src/hyperiontf/infrastructure/__init__.py
+-rw-r--r--   0        0        0     1725 2023-08-06 13:15:08.205946 hyperiontf-0.1.1/src/hyperiontf/infrastructure/event_blorker.py
+-rw-r--r--   0        0        0       92 2023-08-06 13:15:10.016997 hyperiontf-0.1.1/src/hyperiontf/logging/__init__.py
+-rwxr-xr-x   0        0        0     2674 2023-08-06 13:15:09.344004 hyperiontf-0.1.1/src/hyperiontf/logging/assets/build
+-rw-r--r--   0        0        0      935 2023-07-10 10:40:17.706358 hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/button-border-colors.css
+-rw-r--r--   0        0        0      252 2023-07-10 11:29:08.272140 hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/button.css
+-rw-r--r--   0        0        0      665 2023-07-10 13:21:46.590375 hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/colors.css
+-rw-r--r--   0        0        0      392 2023-07-11 12:54:22.880992 hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/filter-bar.css
+-rw-r--r--   0        0        0     1048 2023-07-10 17:15:00.496119 hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/header.css
+-rw-r--r--   0        0        0     1677 2023-07-10 10:04:40.127802 hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/icon-color-filters.css
+-rw-r--r--   0        0        0    38307 2023-07-10 09:52:33.600890 hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/icon-images.css
+-rw-r--r--   0        0        0      285 2023-07-31 09:17:20.506222 hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/icon.css
+-rw-r--r--   0        0        0     2496 2023-08-06 13:15:09.344424 hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/log-message.css
+-rw-r--r--   0        0        0      135 2023-08-06 13:15:09.344901 hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/misc.css
+-rw-r--r--   0        0        0      884 2023-07-10 10:06:36.432340 hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/tooltip.css
+-rw-r--r--   0        0        0      939 2023-07-22 18:34:53.423179 hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/app.js
+-rw-r--r--   0        0        0     4974 2023-07-22 18:41:01.660413 hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/config.js
+-rw-r--r--   0        0        0    11226 2023-07-22 18:51:41.092386 hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/controlPanel.js
+-rw-r--r--   0        0        0     1356 2023-07-22 18:52:20.196646 hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/eventBroker.js
+-rw-r--r--   0        0        0     2136 2023-07-22 18:39:46.004817 hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/helpers.js
+-rw-r--r--   0        0        0    40401 2023-07-23 18:26:33.930932 hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/line.js
+-rw-r--r--   0        0        0     5490 2023-07-22 18:53:19.430887 hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/logger.js
+-rw-r--r--   0        0        0     1192 2023-07-07 17:51:23.600370 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/assert-true.svg
+-rw-r--r--   0        0        0     2530 2023-07-08 11:52:51.914244 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/backtrace.svg
+-rw-r--r--   0        0        0     1424 2023-07-07 16:58:01.309327 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/collapse.svg
+-rw-r--r--   0        0        0      724 2023-07-07 18:40:17.626629 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/column.svg
+-rw-r--r--   0        0        0     1936 2023-07-07 17:33:04.167792 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/debug.svg
+-rw-r--r--   0        0        0     1371 2023-07-07 17:56:05.231809 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/error.svg
+-rw-r--r--   0        0        0     1432 2023-07-07 16:57:55.270184 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/expand.svg
+-rw-r--r--   0        0        0     3067 2023-07-07 17:34:19.284839 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/fatal.svg
+-rw-r--r--   0        0        0     1852 2023-07-07 16:57:50.469467 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/info.svg
+-rw-r--r--   0        0        0      615 2023-07-09 18:17:36.072536 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/level.svg
+-rw-r--r--   0        0        0     2582 2023-07-07 18:42:27.638468 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/log.svg
+-rw-r--r--   0        0        0     1347 2023-07-07 16:57:43.685179 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/page-source.svg
+-rw-r--r--   0        0        0      847 2023-07-07 16:47:23.669853 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/screen-snap.svg
+-rw-r--r--   0        0        0     3786 2023-07-09 18:15:54.736465 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/timestamp.svg
+-rw-r--r--   0        0        0     2555 2023-07-07 16:57:36.968802 hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/warning.svg
+-rw-r--r--   0        0        0    67094 2023-08-06 13:15:09.346258 hyperiontf-0.1.1/src/hyperiontf/logging/assets/template.html
+-rw-r--r--   0        0        0     2485 2023-08-06 13:15:10.017426 hyperiontf-0.1.1/src/hyperiontf/logging/file_handler.py
+-rw-r--r--   0        0        0     4522 2023-08-06 13:15:10.017972 hyperiontf-0.1.1/src/hyperiontf/logging/formatter.py
+-rw-r--r--   0        0        0      715 2023-08-06 13:15:10.018484 hyperiontf-0.1.1/src/hyperiontf/logging/helpers.py
+-rw-r--r--   0        0        0     1605 2023-08-06 13:15:10.018911 hyperiontf-0.1.1/src/hyperiontf/logging/log_depth_manager.py
+-rw-r--r--   0        0        0     2115 2023-08-06 13:15:10.019380 hyperiontf-0.1.1/src/hyperiontf/logging/log_file_manager.py
+-rw-r--r--   0        0        0     4642 2023-08-06 13:15:10.019898 hyperiontf-0.1.1/src/hyperiontf/logging/logger.py
+-rw-r--r--   0        0        0    10946 2023-08-07 11:59:13.323157 hyperiontf-0.1.1/src/hyperiontf/typing.py
+-rw-r--r--   0        0        0      793 2023-08-06 13:15:10.020879 hyperiontf-0.1.1/src/hyperiontf/ui/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 19:02:44.977919 hyperiontf-0.1.1/src/hyperiontf/ui/appium/__init__.py
+-rw-r--r--   0        0        0     8351 2023-08-06 13:15:10.021412 hyperiontf-0.1.1/src/hyperiontf/ui/appium/element.py
+-rw-r--r--   0        0        0     1212 2023-08-06 13:15:10.022046 hyperiontf-0.1.1/src/hyperiontf/ui/appium/map_exception.py
+-rw-r--r--   0        0        0     1689 2023-08-06 13:15:09.016216 hyperiontf-0.1.1/src/hyperiontf/ui/appium/map_locator.py
+-rw-r--r--   0        0        0     4574 2023-08-06 13:15:10.364910 hyperiontf-0.1.1/src/hyperiontf/ui/appium/page.py
+-rw-r--r--   0        0        0     7019 2023-08-07 11:59:13.323531 hyperiontf-0.1.1/src/hyperiontf/ui/automation_adapter_manager.py
+-rw-r--r--   0        0        0     6647 2023-08-06 13:15:10.023213 hyperiontf-0.1.1/src/hyperiontf/ui/by.py
+-rw-r--r--   0        0        0     4421 2023-08-06 13:15:10.202136 hyperiontf-0.1.1/src/hyperiontf/ui/content_manager.py
+-rw-r--r--   0        0        0     3285 2023-08-06 13:15:10.202654 hyperiontf-0.1.1/src/hyperiontf/ui/context_manager.py
+-rw-r--r--   0        0        0        0 2023-06-08 12:54:44.538706 hyperiontf-0.1.1/src/hyperiontf/ui/decorators/__init__.py
+-rw-r--r--   0        0        0     5234 2023-08-06 13:15:10.365843 hyperiontf-0.1.1/src/hyperiontf/ui/decorators/autolog_class_method_helper.py
+-rw-r--r--   0        0        0     4826 2023-08-06 13:15:10.024896 hyperiontf-0.1.1/src/hyperiontf/ui/decorators/element_accessor.py
+-rw-r--r--   0        0        0     2299 2023-08-06 13:15:10.025410 hyperiontf-0.1.1/src/hyperiontf/ui/decorators/element_error_recovery.py
+-rw-r--r--   0        0        0     9074 2023-08-06 13:15:10.203200 hyperiontf-0.1.1/src/hyperiontf/ui/decorators/page_object_helpers.py
+-rw-r--r--   0        0        0     1424 2023-08-06 13:15:10.203631 hyperiontf-0.1.1/src/hyperiontf/ui/desktop_window.py
+-rw-r--r--   0        0        0     5475 2023-08-06 13:15:10.026968 hyperiontf-0.1.1/src/hyperiontf/ui/element.py
+-rw-r--r--   0        0        0     1618 2023-08-06 13:15:10.204107 hyperiontf-0.1.1/src/hyperiontf/ui/elements.py
+-rw-r--r--   0        0        0      860 2023-08-06 13:15:10.204538 hyperiontf-0.1.1/src/hyperiontf/ui/iframe.py
+-rw-r--r--   0        0        0    18002 2023-08-07 11:59:13.324223 hyperiontf-0.1.1/src/hyperiontf/ui/locatable.py
+-rw-r--r--   0        0        0     1505 2023-08-06 13:15:10.028857 hyperiontf-0.1.1/src/hyperiontf/ui/mobile_screen.py
+-rw-r--r--   0        0        0     1233 2023-08-06 13:15:10.029221 hyperiontf-0.1.1/src/hyperiontf/ui/page_object_base.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:41:57.247681 hyperiontf-0.1.1/src/hyperiontf/ui/playwright/__init__.py
+-rw-r--r--   0        0        0     1871 2023-08-06 13:15:10.029599 hyperiontf-0.1.1/src/hyperiontf/ui/playwright/assert_stale_element_reference.py
+-rw-r--r--   0        0        0    11380 2023-08-06 13:15:10.366325 hyperiontf-0.1.1/src/hyperiontf/ui/playwright/element.py
+-rw-r--r--   0        0        0      938 2023-08-07 11:59:13.324620 hyperiontf-0.1.1/src/hyperiontf/ui/playwright/map_exception.py
+-rw-r--r--   0        0        0      981 2023-08-06 13:15:09.516703 hyperiontf-0.1.1/src/hyperiontf/ui/playwright/map_locator.py
+-rw-r--r--   0        0        0     5558 2023-08-06 13:15:10.366881 hyperiontf-0.1.1/src/hyperiontf/ui/playwright/page.py
+-rw-r--r--   0        0        0     1693 2023-08-06 13:15:10.031077 hyperiontf-0.1.1/src/hyperiontf/ui/playwright/selenium_to_playwright_script.py
+-rw-r--r--   0        0        0        0 2023-08-06 13:15:09.021587 hyperiontf-0.1.1/src/hyperiontf/ui/selenium/__init__.py
+-rw-r--r--   0        0        0     9708 2023-08-06 13:15:10.031416 hyperiontf-0.1.1/src/hyperiontf/ui/selenium/element.py
+-rw-r--r--   0        0        0     1268 2023-08-07 11:59:13.324967 hyperiontf-0.1.1/src/hyperiontf/ui/selenium/map_exception.py
+-rw-r--r--   0        0        0      993 2023-08-06 13:15:08.852673 hyperiontf-0.1.1/src/hyperiontf/ui/selenium/map_locator.py
+-rw-r--r--   0        0        0     9180 2023-08-07 11:59:13.325288 hyperiontf-0.1.1/src/hyperiontf/ui/selenium/page.py
+-rw-r--r--   0        0        0     6876 2023-08-06 13:15:10.032439 hyperiontf-0.1.1/src/hyperiontf/ui/viewport_manager.py
+-rw-r--r--   0        0        0     2242 2023-08-07 11:59:13.325609 hyperiontf-0.1.1/src/hyperiontf/ui/webpage.py
+-rw-r--r--   0        0        0     1533 2023-08-06 13:15:10.206097 hyperiontf-0.1.1/src/hyperiontf/ui/webview.py
+-rw-r--r--   0        0        0      394 2023-08-06 13:15:10.033569 hyperiontf-0.1.1/src/hyperiontf/ui/widget.py
+-rw-r--r--   0        0        0     3728 2023-08-06 13:15:10.206600 hyperiontf-0.1.1/src/hyperiontf/ui/window_manager.py
+-rw-r--r--   0        0        0    49965 1970-01-01 00:00:00.000000 hyperiontf-0.1.1/PKG-INFO
```

### Comparing `hyperiontf-0.1.0/LICENSE` & `hyperiontf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/README.md` & `hyperiontf-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/__init__.py` & `hyperiontf-0.1.1/src/hyperiontf/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/api/rest_client/client.py` & `hyperiontf-0.1.1/src/hyperiontf/api/rest_client/client.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/api/rest_client/request.py` & `hyperiontf-0.1.1/src/hyperiontf/api/rest_client/request.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/api/rest_client/response.py` & `hyperiontf-0.1.1/src/hyperiontf/api/rest_client/response.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/assertions/expect.py` & `hyperiontf-0.1.1/src/hyperiontf/assertions/expect.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/assertions/logging_helper.py` & `hyperiontf-0.1.1/src/hyperiontf/assertions/logging_helper.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/configuration/capabilities.py` & `hyperiontf-0.1.1/src/hyperiontf/configuration/capabilities.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/configuration/config.py` & `hyperiontf-0.1.1/src/hyperiontf/configuration/config.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/configuration/section.py` & `hyperiontf-0.1.1/src/hyperiontf/configuration/section.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/configuration/sections/web_capabilities.py` & `hyperiontf-0.1.1/src/hyperiontf/configuration/sections/web_capabilities.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/executors/pytest/fixture.py` & `hyperiontf-0.1.1/src/hyperiontf/executors/pytest/fixture.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/executors/pytest/logger_setup.py` & `hyperiontf-0.1.1/src/hyperiontf/executors/pytest/logger_setup.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/helpers/decorators/without_failure.py` & `hyperiontf-0.1.1/src/hyperiontf/helpers/decorators/without_failure.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/helpers/dict_heplers.py` & `hyperiontf-0.1.1/src/hyperiontf/helpers/dict_heplers.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/helpers/extend_instance.py` & `hyperiontf-0.1.1/src/hyperiontf/helpers/extend_instance.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/helpers/own_methods_helper.py` & `hyperiontf-0.1.1/src/hyperiontf/helpers/own_methods_helper.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/helpers/string_helpers.py` & `hyperiontf-0.1.1/src/hyperiontf/helpers/string_helpers.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/infrastructure/event_blorker.py` & `hyperiontf-0.1.1/src/hyperiontf/infrastructure/event_blorker.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/build` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/build`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/button-border-colors.css` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/button-border-colors.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/colors.css` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/colors.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/header.css` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/header.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/icon-color-filters.css` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/icon-color-filters.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/icon-images.css` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/icon-images.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/log-message.css` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/log-message.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/css/tooltip.css` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/app.js` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/config.js` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/config.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/controlPanel.js` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/eventBroker.js` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/eventBroker.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/helpers.js` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/helpers.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/line.js` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/line.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/js/logger.js` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/js/logger.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/assert-true.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/assert-true.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/backtrace.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/backtrace.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/collapse.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/collapse.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/column.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/column.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/debug.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/debug.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/error.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/error.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/expand.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/expand.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/fatal.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/fatal.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/info.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/info.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/level.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/level.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/log.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/log.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/page-source.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/page-source.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/screen-snap.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/screen-snap.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/timestamp.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/timestamp.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/svg/warning.svg` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/svg/warning.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/assets/template.html` & `hyperiontf-0.1.1/src/hyperiontf/logging/assets/template.html`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/file_handler.py` & `hyperiontf-0.1.1/src/hyperiontf/logging/file_handler.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/formatter.py` & `hyperiontf-0.1.1/src/hyperiontf/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/helpers.py` & `hyperiontf-0.1.1/src/hyperiontf/logging/helpers.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/log_depth_manager.py` & `hyperiontf-0.1.1/src/hyperiontf/logging/log_depth_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/log_file_manager.py` & `hyperiontf-0.1.1/src/hyperiontf/logging/log_file_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/logging/logger.py` & `hyperiontf-0.1.1/src/hyperiontf/logging/logger.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/typing.py` & `hyperiontf-0.1.1/src/hyperiontf/typing.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/__init__.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/appium/element.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/appium/element.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/appium/map_exception.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/appium/map_exception.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/appium/map_locator.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/appium/map_locator.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/appium/page.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/appium/page.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/automation_adapter_manager.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/automation_adapter_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/by.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/by.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/content_manager.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/content_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/context_manager.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/context_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/decorators/autolog_class_method_helper.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/decorators/autolog_class_method_helper.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/decorators/element_accessor.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/decorators/element_accessor.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/decorators/element_error_recovery.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/decorators/element_error_recovery.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/decorators/page_object_helpers.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/decorators/page_object_helpers.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/desktop_window.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/desktop_window.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/element.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/element.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/elements.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/elements.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/iframe.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/iframe.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/locatable.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/locatable.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/mobile_screen.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/mobile_screen.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/page_object_base.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/page_object_base.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/playwright/assert_stale_element_reference.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/playwright/assert_stale_element_reference.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/playwright/element.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/playwright/element.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/playwright/map_exception.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/playwright/map_exception.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/playwright/map_locator.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/playwright/map_locator.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/playwright/page.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/playwright/page.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/playwright/selenium_to_playwright_script.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/playwright/selenium_to_playwright_script.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/selenium/element.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/selenium/element.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/selenium/map_exception.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/selenium/map_exception.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/selenium/map_locator.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/selenium/map_locator.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/selenium/page.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/selenium/page.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/viewport_manager.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/viewport_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/webpage.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/webpage.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/webview.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/webview.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/src/hyperiontf/ui/window_manager.py` & `hyperiontf-0.1.1/src/hyperiontf/ui/window_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.1.0/PKG-INFO` & `hyperiontf-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperiontf
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hyperion Testing Framework
 License: Apache 2.0 License
 Author: Oleksiy Bondar
 Author-email: bondaroleksiyandriyovich@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

