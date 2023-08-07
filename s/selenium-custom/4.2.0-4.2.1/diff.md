# Comparing `tmp/selenium-custom-4.2.0.tar.gz` & `tmp/selenium-custom-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-custom-4.2.0.tar", last modified: Mon Aug  7 02:56:30 2023, max compression
+gzip compressed data, was "selenium-custom-4.2.1.tar", last modified: Mon Aug  7 03:12:16 2023, max compression
```

## Comparing `selenium-custom-4.2.0.tar` & `selenium-custom-4.2.1.tar`

### file list

```diff
@@ -1,104 +1,109 @@
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.333789 selenium-custom-4.2.0/
--rw-rw-r--   0 victorolade  (1061) victorolade  (1061)      823 2023-08-07 02:56:30.333789 selenium-custom-4.2.0/PKG-INFO
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.321788 selenium-custom-4.2.0/selenium/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      811 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/__init__.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.321788 selenium-custom-4.2.0/selenium/common/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3770 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/common/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     9305 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/common/exceptions.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      881 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/types.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.321788 selenium-custom-4.2.0/selenium/webdriver/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2484 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/__init__.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.321788 selenium-custom-4.2.0/selenium/webdriver/chrome/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/chrome/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1430 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/chrome/options.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1763 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/chrome/service.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3716 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/chrome/webdriver.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.325788 selenium-custom-4.2.0/selenium/webdriver/chromium/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/chromium/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     6162 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/chromium/options.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2515 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/chromium/remote_connection.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1991 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/chromium/service.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     9431 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/chromium/webdriver.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.325788 selenium-custom-4.2.0/selenium/webdriver/common/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    14114 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/action_chains.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2583 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/alert.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1103 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/by.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2986 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/desired_capabilities.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.325788 selenium-custom-4.2.0/selenium/webdriver/common/html5/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/html5/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1631 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/html5/application_cache.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2329 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/keys.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     6066 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/log.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     9029 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/options.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     8500 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/print_page_options.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    10769 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/proxy.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     5805 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/service.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3831 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/timeouts.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     4474 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/utils.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     8855 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/virtual_authenticator.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      929 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/common/window.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.325788 selenium-custom-4.2.0/selenium/webdriver/edge/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/edge/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1721 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/edge/options.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2271 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/edge/service.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3368 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/edge/webdriver.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.325788 selenium-custom-4.2.0/selenium/webdriver/firefox/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/firefox/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2868 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/firefox/extension_connection.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     8787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/firefox/firefox_binary.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    14498 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/firefox/firefox_profile.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     5389 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/firefox/options.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1733 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/firefox/remote_connection.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2706 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/firefox/service.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    13541 2023-08-07 01:56:50.000000 selenium-custom-4.2.0/selenium/webdriver/firefox/webdriver.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.325788 selenium-custom-4.2.0/selenium/webdriver/ie/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/ie/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    11547 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/ie/options.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2357 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/ie/service.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     5542 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/ie/webdriver.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.329789 selenium-custom-4.2.0/selenium/webdriver/opera/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/opera/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3694 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/opera/options.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3525 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/opera/webdriver.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.329789 selenium-custom-4.2.0/selenium/webdriver/remote/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      968 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/bidi_connection.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     4608 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/command.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    11987 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/errorhandler.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1803 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/file_detector.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2673 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/mobile.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    18220 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/remote_connection.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1009 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/script_key.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3064 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/shadowroot.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     5081 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/switch_to.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      978 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/utils.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    54977 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/webdriver.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    29301 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/remote/webelement.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.329789 selenium-custom-4.2.0/selenium/webdriver/safari/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/safari/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     4256 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/safari/options.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      934 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/safari/permissions.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1519 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/safari/remote_connection.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2514 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/safari/service.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     6306 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/safari/webdriver.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.329789 selenium-custom-4.2.0/selenium/webdriver/support/
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/support/__init__.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2025 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/support/abstract_event_listener.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    12325 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/support/color.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    16707 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/support/event_firing_webdriver.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      920 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/support/events.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)    14637 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/support/expected_conditions.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     6033 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/support/relative_locator.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     9258 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/support/select.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)      863 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/support/ui.py
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     4733 2023-08-07 01:52:18.000000 selenium-custom-4.2.0/selenium/webdriver/support/wait.py
-drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 02:56:30.333789 selenium-custom-4.2.0/selenium_custom.egg-info/
--rw-rw-r--   0 victorolade  (1061) victorolade  (1061)      823 2023-08-07 02:56:30.000000 selenium-custom-4.2.0/selenium_custom.egg-info/PKG-INFO
--rw-rw-r--   0 victorolade  (1061) victorolade  (1061)     3321 2023-08-07 02:56:30.000000 selenium-custom-4.2.0/selenium_custom.egg-info/SOURCES.txt
--rw-rw-r--   0 victorolade  (1061) victorolade  (1061)        1 2023-08-07 02:56:30.000000 selenium-custom-4.2.0/selenium_custom.egg-info/dependency_links.txt
--rw-rw-r--   0 victorolade  (1061) victorolade  (1061)        1 2023-08-07 02:31:03.000000 selenium-custom-4.2.0/selenium_custom.egg-info/not-zip-safe
--rw-rw-r--   0 victorolade  (1061) victorolade  (1061)       59 2023-08-07 02:56:30.000000 selenium-custom-4.2.0/selenium_custom.egg-info/requires.txt
--rw-rw-r--   0 victorolade  (1061) victorolade  (1061)        9 2023-08-07 02:56:30.000000 selenium-custom-4.2.0/selenium_custom.egg-info/top_level.txt
--rw-rw-r--   0 victorolade  (1061) victorolade  (1061)       38 2023-08-07 02:56:30.333789 selenium-custom-4.2.0/setup.cfg
--rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3048 2023-08-07 02:56:04.000000 selenium-custom-4.2.0/setup.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.900085 selenium-custom-4.2.1/
+-rw-rw-r--   0 victorolade  (1061) victorolade  (1061)      823 2023-08-07 03:12:16.900085 selenium-custom-4.2.1/PKG-INFO
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.888084 selenium-custom-4.2.1/selenium/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      811 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/__init__.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.888084 selenium-custom-4.2.1/selenium/common/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3770 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/common/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     9305 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/common/exceptions.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      881 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/types.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.888084 selenium-custom-4.2.1/selenium/webdriver/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2484 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/__init__.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.888084 selenium-custom-4.2.1/selenium/webdriver/chrome/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/chrome/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1430 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/chrome/options.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1763 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/chrome/service.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3716 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/chrome/webdriver.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.892085 selenium-custom-4.2.1/selenium/webdriver/chromium/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/chromium/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     6162 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/chromium/options.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2515 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/chromium/remote_connection.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1991 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/chromium/service.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     9431 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/chromium/webdriver.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.892085 selenium-custom-4.2.1/selenium/webdriver/common/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    14114 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/action_chains.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2583 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/alert.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1103 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/by.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2986 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/desired_capabilities.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.892085 selenium-custom-4.2.1/selenium/webdriver/common/html5/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/html5/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1631 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/html5/application_cache.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2329 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/keys.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     6066 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/log.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     9029 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/options.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     8500 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/print_page_options.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    10769 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/proxy.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     5805 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/service.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3831 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/timeouts.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     4474 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/utils.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     8855 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/virtual_authenticator.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      929 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/common/window.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.892085 selenium-custom-4.2.1/selenium/webdriver/edge/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/edge/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1721 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/edge/options.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2271 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/edge/service.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3368 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/edge/webdriver.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.892085 selenium-custom-4.2.1/selenium/webdriver/firefox/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/firefox/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2868 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/firefox/extension_connection.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     8787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/firefox/firefox_binary.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    14498 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/firefox/firefox_profile.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     5389 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/firefox/options.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1733 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/firefox/remote_connection.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2706 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/firefox/service.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    13541 2023-08-07 01:56:50.000000 selenium-custom-4.2.1/selenium/webdriver/firefox/webdriver.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.896085 selenium-custom-4.2.1/selenium/webdriver/ie/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/ie/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    11547 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/ie/options.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2357 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/ie/service.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     5542 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/ie/webdriver.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.896085 selenium-custom-4.2.1/selenium/webdriver/opera/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/opera/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3694 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/opera/options.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3525 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/opera/webdriver.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.896085 selenium-custom-4.2.1/selenium/webdriver/remote/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      968 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/bidi_connection.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     4608 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/command.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    11987 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/errorhandler.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1803 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/file_detector.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2673 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/mobile.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    18220 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/remote_connection.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1009 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/script_key.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3064 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/shadowroot.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     5081 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/switch_to.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      978 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/utils.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    54977 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/webdriver.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    29301 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/remote/webelement.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.896085 selenium-custom-4.2.1/selenium/webdriver/safari/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/safari/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     4256 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/safari/options.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      934 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/safari/permissions.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1519 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/safari/remote_connection.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2514 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/safari/service.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     6306 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/safari/webdriver.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.900085 selenium-custom-4.2.1/selenium/webdriver/support/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/support/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2025 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/support/abstract_event_listener.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    12325 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/support/color.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    16707 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/support/event_firing_webdriver.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      920 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/support/events.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)    14637 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/support/expected_conditions.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     6033 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/support/relative_locator.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     9258 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/support/select.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      863 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/support/ui.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     4733 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/support/wait.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.900085 selenium-custom-4.2.1/selenium/webdriver/webkitgtk/
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)      787 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/webkitgtk/__init__.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     2689 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/webkitgtk/options.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     1643 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/webkitgtk/service.py
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3008 2023-08-07 01:52:18.000000 selenium-custom-4.2.1/selenium/webdriver/webkitgtk/webdriver.py
+drwxrwxr-x   0 victorolade  (1061) victorolade  (1061)        0 2023-08-07 03:12:16.900085 selenium-custom-4.2.1/selenium_custom.egg-info/
+-rw-rw-r--   0 victorolade  (1061) victorolade  (1061)      823 2023-08-07 03:12:16.000000 selenium-custom-4.2.1/selenium_custom.egg-info/PKG-INFO
+-rw-rw-r--   0 victorolade  (1061) victorolade  (1061)     3484 2023-08-07 03:12:16.000000 selenium-custom-4.2.1/selenium_custom.egg-info/SOURCES.txt
+-rw-rw-r--   0 victorolade  (1061) victorolade  (1061)        1 2023-08-07 03:12:16.000000 selenium-custom-4.2.1/selenium_custom.egg-info/dependency_links.txt
+-rw-rw-r--   0 victorolade  (1061) victorolade  (1061)        1 2023-08-07 02:31:03.000000 selenium-custom-4.2.1/selenium_custom.egg-info/not-zip-safe
+-rw-rw-r--   0 victorolade  (1061) victorolade  (1061)       59 2023-08-07 03:12:16.000000 selenium-custom-4.2.1/selenium_custom.egg-info/requires.txt
+-rw-rw-r--   0 victorolade  (1061) victorolade  (1061)        9 2023-08-07 03:12:16.000000 selenium-custom-4.2.1/selenium_custom.egg-info/top_level.txt
+-rw-rw-r--   0 victorolade  (1061) victorolade  (1061)       38 2023-08-07 03:12:16.900085 selenium-custom-4.2.1/setup.cfg
+-rw-r--r--   0 victorolade  (1061) victorolade  (1061)     3115 2023-08-07 03:12:07.000000 selenium-custom-4.2.1/setup.py
```

### Comparing `selenium-custom-4.2.0/PKG-INFO` & `selenium-custom-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-custom
-Version: 4.2.0
+Version: 4.2.1
 Summary: Python bindings for Selenium
 Home-page: https://github.com/SeleniumHQ/selenium/
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `selenium-custom-4.2.0/selenium/__init__.py` & `selenium-custom-4.2.1/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/common/__init__.py` & `selenium-custom-4.2.1/selenium/common/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/common/exceptions.py` & `selenium-custom-4.2.1/selenium/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/types.py` & `selenium-custom-4.2.1/selenium/types.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/chrome/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/chrome/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/chrome/options.py` & `selenium-custom-4.2.1/selenium/webdriver/chrome/options.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/chrome/service.py` & `selenium-custom-4.2.1/selenium/webdriver/chrome/service.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/chrome/webdriver.py` & `selenium-custom-4.2.1/selenium/webdriver/chrome/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/chromium/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/chromium/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/chromium/options.py` & `selenium-custom-4.2.1/selenium/webdriver/chromium/options.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/chromium/remote_connection.py` & `selenium-custom-4.2.1/selenium/webdriver/chromium/remote_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/chromium/service.py` & `selenium-custom-4.2.1/selenium/webdriver/chromium/service.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/chromium/webdriver.py` & `selenium-custom-4.2.1/selenium/webdriver/chromium/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/common/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/action_chains.py` & `selenium-custom-4.2.1/selenium/webdriver/common/action_chains.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/alert.py` & `selenium-custom-4.2.1/selenium/webdriver/common/alert.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/by.py` & `selenium-custom-4.2.1/selenium/webdriver/common/by.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/desired_capabilities.py` & `selenium-custom-4.2.1/selenium/webdriver/common/desired_capabilities.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/html5/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/common/html5/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/html5/application_cache.py` & `selenium-custom-4.2.1/selenium/webdriver/common/html5/application_cache.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/keys.py` & `selenium-custom-4.2.1/selenium/webdriver/common/keys.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/log.py` & `selenium-custom-4.2.1/selenium/webdriver/common/log.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/options.py` & `selenium-custom-4.2.1/selenium/webdriver/common/options.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/print_page_options.py` & `selenium-custom-4.2.1/selenium/webdriver/common/print_page_options.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/proxy.py` & `selenium-custom-4.2.1/selenium/webdriver/common/proxy.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/service.py` & `selenium-custom-4.2.1/selenium/webdriver/common/service.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/timeouts.py` & `selenium-custom-4.2.1/selenium/webdriver/common/timeouts.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/utils.py` & `selenium-custom-4.2.1/selenium/webdriver/common/utils.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/virtual_authenticator.py` & `selenium-custom-4.2.1/selenium/webdriver/common/virtual_authenticator.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/common/window.py` & `selenium-custom-4.2.1/selenium/webdriver/common/window.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/edge/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/edge/options.py` & `selenium-custom-4.2.1/selenium/webdriver/edge/options.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/edge/service.py` & `selenium-custom-4.2.1/selenium/webdriver/edge/service.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/edge/webdriver.py` & `selenium-custom-4.2.1/selenium/webdriver/edge/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/firefox/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/firefox/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/firefox/extension_connection.py` & `selenium-custom-4.2.1/selenium/webdriver/firefox/extension_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/firefox/firefox_binary.py` & `selenium-custom-4.2.1/selenium/webdriver/firefox/firefox_binary.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/firefox/firefox_profile.py` & `selenium-custom-4.2.1/selenium/webdriver/firefox/firefox_profile.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/firefox/options.py` & `selenium-custom-4.2.1/selenium/webdriver/firefox/options.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/firefox/remote_connection.py` & `selenium-custom-4.2.1/selenium/webdriver/firefox/remote_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/firefox/service.py` & `selenium-custom-4.2.1/selenium/webdriver/firefox/service.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/firefox/webdriver.py` & `selenium-custom-4.2.1/selenium/webdriver/firefox/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/ie/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/ie/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/ie/options.py` & `selenium-custom-4.2.1/selenium/webdriver/ie/options.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/ie/service.py` & `selenium-custom-4.2.1/selenium/webdriver/ie/service.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/ie/webdriver.py` & `selenium-custom-4.2.1/selenium/webdriver/ie/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/opera/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/opera/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/opera/options.py` & `selenium-custom-4.2.1/selenium/webdriver/opera/options.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/opera/webdriver.py` & `selenium-custom-4.2.1/selenium/webdriver/opera/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/bidi_connection.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/bidi_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/command.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/command.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/errorhandler.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/errorhandler.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/file_detector.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/file_detector.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/mobile.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/mobile.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/remote_connection.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/remote_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/script_key.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/script_key.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/shadowroot.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/shadowroot.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/switch_to.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/switch_to.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/utils.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/utils.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/webdriver.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/remote/webelement.py` & `selenium-custom-4.2.1/selenium/webdriver/remote/webelement.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/safari/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/safari/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/safari/options.py` & `selenium-custom-4.2.1/selenium/webdriver/safari/options.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/safari/permissions.py` & `selenium-custom-4.2.1/selenium/webdriver/safari/permissions.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/safari/remote_connection.py` & `selenium-custom-4.2.1/selenium/webdriver/safari/remote_connection.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/safari/service.py` & `selenium-custom-4.2.1/selenium/webdriver/safari/service.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/safari/webdriver.py` & `selenium-custom-4.2.1/selenium/webdriver/safari/webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/support/__init__.py` & `selenium-custom-4.2.1/selenium/webdriver/support/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/support/abstract_event_listener.py` & `selenium-custom-4.2.1/selenium/webdriver/support/abstract_event_listener.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/support/color.py` & `selenium-custom-4.2.1/selenium/webdriver/support/color.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/support/event_firing_webdriver.py` & `selenium-custom-4.2.1/selenium/webdriver/support/event_firing_webdriver.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/support/events.py` & `selenium-custom-4.2.1/selenium/webdriver/support/events.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/support/expected_conditions.py` & `selenium-custom-4.2.1/selenium/webdriver/support/expected_conditions.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/support/relative_locator.py` & `selenium-custom-4.2.1/selenium/webdriver/support/relative_locator.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/support/select.py` & `selenium-custom-4.2.1/selenium/webdriver/support/select.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/support/ui.py` & `selenium-custom-4.2.1/selenium/webdriver/support/ui.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium/webdriver/support/wait.py` & `selenium-custom-4.2.1/selenium/webdriver/support/wait.py`

 * *Files identical despite different names*

### Comparing `selenium-custom-4.2.0/selenium_custom.egg-info/PKG-INFO` & `selenium-custom-4.2.1/selenium_custom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-custom
-Version: 4.2.0
+Version: 4.2.1
 Summary: Python bindings for Selenium
 Home-page: https://github.com/SeleniumHQ/selenium/
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `selenium-custom-4.2.0/selenium_custom.egg-info/SOURCES.txt` & `selenium-custom-4.2.1/selenium_custom.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -74,13 +74,17 @@
 selenium/webdriver/support/event_firing_webdriver.py
 selenium/webdriver/support/events.py
 selenium/webdriver/support/expected_conditions.py
 selenium/webdriver/support/relative_locator.py
 selenium/webdriver/support/select.py
 selenium/webdriver/support/ui.py
 selenium/webdriver/support/wait.py
+selenium/webdriver/webkitgtk/__init__.py
+selenium/webdriver/webkitgtk/options.py
+selenium/webdriver/webkitgtk/service.py
+selenium/webdriver/webkitgtk/webdriver.py
 selenium_custom.egg-info/PKG-INFO
 selenium_custom.egg-info/SOURCES.txt
 selenium_custom.egg-info/dependency_links.txt
 selenium_custom.egg-info/not-zip-safe
 selenium_custom.egg-info/requires.txt
 selenium_custom.egg-info/top_level.txt
```

### Comparing `selenium-custom-4.2.0/setup.py` & `selenium-custom-4.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 for scheme in INSTALL_SCHEMES.values():
     scheme['data'] = scheme['purelib']
 
 setup_args = {
     'cmdclass': {'install': install},
     'name': 'selenium-custom',
-    'version': "4.2.0",
+    'version': "4.2.1",
     'license': 'Apache 2.0',
     'description': 'Python bindings for Selenium',
     'url': 'https://github.com/SeleniumHQ/selenium/',
     'python_requires': '~=3.7',
     'classifiers': ['Development Status :: 5 - Production/Stable',
                     'Intended Audience :: Developers',
                     'License :: OSI Approved :: Apache Software License',
@@ -59,14 +59,16 @@
                  'selenium.webdriver.support',
                  'selenium.webdriver.firefox',
                  'selenium.webdriver.ie',
                  'selenium.webdriver.edge',
                  'selenium.webdriver.opera',
                  'selenium.webdriver.remote',
                  'selenium.webdriver.support',
-                 'selenium.webdriver.safari',],
+                 'selenium.webdriver.safari',
+                 'selenium.webdriver.webkitgtk',
+                 ],
     'include_package_data': True,
     'install_requires': ['urllib3[secure, socks]~=1.26', "trio~=0.17", "trio-websocket~=0.9"],
     'zip_safe': False
 }
 
 setup(**setup_args)
```

