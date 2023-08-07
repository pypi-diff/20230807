# Comparing `tmp/foundrytools-cli-1.0.0.tar.gz` & `tmp/foundrytools-cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundrytools-cli-1.0.0.tar", last modified: Fri Jul 28 14:57:20 2023, max compression
+gzip compressed data, was "foundrytools-cli-1.0.1.tar", last modified: Mon Aug  7 06:14:50 2023, max compression
```

## Comparing `foundrytools-cli-1.0.0.tar` & `foundrytools-cli-1.0.1.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 14:57:20.324020 foundrytools-cli-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       26 2023-07-28 14:57:10.000000 foundrytools-cli-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3051 2023-07-28 14:57:20.324020 foundrytools-cli-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2617 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 14:57:20.262623 foundrytools-cli-1.0.0/foundryToolsCLI/
-drwxrwxrwx   0        0        0        0 2023-07-28 14:57:20.279972 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/
--rw-rw-rw-   0        0        0        0 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/__init__.py
--rw-rw-rw-   0        0        0    44948 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/_ftcli_tb.py
--rw-rw-rw-   0        0        0    13888 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_assistant.py
--rw-rw-rw-   0        0        0     6580 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_cff.py
--rw-rw-rw-   0        0        0    11654 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_converter.py
--rw-rw-rw-   0        0        0    21765 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_fix.py
--rw-rw-rw-   0        0        0     3745 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_hhea.py
--rw-rw-rw-   0        0        0    10746 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_metrics.py
--rw-rw-rw-   0        0        0    13388 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_name.py
--rw-rw-rw-   0        0        0    19822 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_os2.py
--rw-rw-rw-   0        0        0    16566 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_otf.py
--rw-rw-rw-   0        0        0     3678 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_post.py
--rw-rw-rw-   0        0        0     3179 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_print.py
--rw-rw-rw-   0        0        0    10295 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_ttf.py
--rw-rw-rw-   0        0        0    12736 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:57:20.283971 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/
--rw-rw-rw-   0        0        0    36684 2023-07-19 10:25:20.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/Font.py
--rw-rw-rw-   0        0        0     2673 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/VFont.py
--rw-rw-rw-   0        0        0        0 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:57:20.288601 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/assistant/
--rw-rw-rw-   0        0        0    22582 2023-07-23 21:17:14.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/assistant/UI.py
--rw-rw-rw-   0        0        0        0 2023-07-11 16:16:34.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/assistant/__init__.py
--rw-rw-rw-   0        0        0    27998 2023-07-23 21:17:14.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/assistant/fonts_data.py
--rw-rw-rw-   0        0        0     2129 2023-07-23 21:17:14.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/assistant/styles_mapping.py
--rw-rw-rw-   0        0        0     2334 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:57:20.297601 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/
--rw-rw-rw-   0        0        0        0 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/options.py
--rw-rw-rw-   0        0        0     5016 2023-07-18 10:17:10.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/otf_to_ttf.py
--rw-rw-rw-   0        0        0     3247 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/sfnt_to_web.py
--rw-rw-rw-   0        0        0     2143 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/ttc_to_sfnt.py
--rw-rw-rw-   0        0        0     8242 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/ttf_to_otf.py
--rw-rw-rw-   0        0        0     3709 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/variable_to_static.py
--rw-rw-rw-   0        0        0     2212 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/web_to_sfnt.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:57:20.299601 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/printer/
--rw-rw-rw-   0        0        0    11844 2023-07-17 06:27:07.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/printer/UI.py
--rw-rw-rw-   0        0        0        0 2023-07-13 07:23:19.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/printer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:57:20.306601 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/
--rw-rw-rw-   0        0        0     3300 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/CFF_.py
--rw-rw-rw-   0        0        0    12797 2023-07-13 07:23:19.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/OS_2.py
--rw-rw-rw-   0        0        0        0 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/__init__.py
--rw-rw-rw-   0        0        0     1448 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/head.py
--rw-rw-rw-   0        0        0      769 2023-07-12 09:32:23.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/hhea.py
--rw-rw-rw-   0        0        0     7136 2023-07-18 12:04:13.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/name.py
--rw-rw-rw-   0        0        0      636 2023-07-12 11:39:15.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/post.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:57:20.314601 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/
--rw-rw-rw-   0        0        0        0 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/__init__.py
--rw-rw-rw-   0        0        0     1074 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/bits_tools.py
--rw-rw-rw-   0        0        0     4289 2023-07-23 21:17:14.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/cli_tools.py
--rw-rw-rw-   0        0        0     4773 2023-07-23 21:17:14.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/click_tools.py
--rw-rw-rw-   0        0        0     2021 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/otf_tools.py
--rw-rw-rw-   0        0        0     5918 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/skia_tools.py
--rw-rw-rw-   0        0        0     1099 2023-07-13 07:31:43.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/text_tools.py
--rw-rw-rw-   0        0        0     4137 2023-07-11 16:20:04.000000 foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/ttf_tools.py
--rw-rw-rw-   0        0        0        0 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/__init__.py
--rw-rw-rw-   0        0        0      875 2023-07-28 14:21:28.000000 foundrytools-cli-1.0.0/foundryToolsCLI/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:57:20.323020 foundrytools-cli-1.0.0/foundrytools_cli.egg-info/
--rw-rw-rw-   0        0        0     3051 2023-07-28 14:57:20.000000 foundrytools-cli-1.0.0/foundrytools_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2189 2023-07-28 14:57:20.000000 foundrytools-cli-1.0.0/foundrytools_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 14:57:20.000000 foundrytools-cli-1.0.0/foundrytools_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-28 14:57:20.000000 foundrytools-cli-1.0.0/foundrytools_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 14:44:31.000000 foundrytools-cli-1.0.0/foundrytools_cli.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      217 2023-07-28 14:57:20.000000 foundrytools-cli-1.0.0/foundrytools_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-28 14:57:20.000000 foundrytools-cli-1.0.0/foundrytools_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 14:57:20.324020 foundrytools-cli-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1266 2023-07-28 14:36:15.000000 foundrytools-cli-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.464173 foundrytools-cli-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-07 06:14:50.464173 foundrytools-cli-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.452173 foundrytools-cli-1.0.1/foundryToolsCLI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.456173 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_cff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20917 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_hhea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18933 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_os2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15894 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_otf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_ttf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.456173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    35586 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/Font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/VFont.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.456173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    21938 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/UI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27371 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/fonts_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/styles_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.460173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/otf_to_ttf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/sfnt_to_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/ttc_to_sfnt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/ttf_to_otf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/variable_to_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/web_to_sfnt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.460173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/printer/UI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.460173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/CFF_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/OS_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/hhea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.464173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/bits_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/cli_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/click_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/otf_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/skia_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/text_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/ttf_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.464173 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 06:14:50.464173 foundrytools-cli-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/setup.py
```

### Comparing `foundrytools-cli-1.0.0/LICENSE` & `foundrytools-cli-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 ftCLI
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 ftCLI
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `foundrytools-cli-1.0.0/PKG-INFO` & `foundrytools-cli-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,78 @@
-Metadata-Version: 2.1
-Name: foundrytools-cli
-Version: 1.0.0
-Summary: A set of command line tools to inspect, manipulate and convert font files
-Home-page: https://github.com/ftCLI/FoundryTools-CLI
-Author: ftCLI
-Author-email: ftcli@proton.me
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# FoundryTools-CLI
-FoundryTools-CLI, former known as ftCLI, is a collection of command line tools written in Python to inspect, manipulate
-and convert fonts. It takes advantage of the capabilities made available by other tools such as:
-
-* [FontTools](https://github.com/fonttools/fonttools)
-* [AFDKO](https://github.com/adobe-type-tools/afdko)
-* [skia-pathops](https://github.com/fonttools/skia-pathops)
-* [cffsubr](https://github.com/adobe-type-tools/cffsubr)
-* [psautohint](https://github.com/adobe-type-tools/psautohint)
-* [ttfautohint-py](https://github.com/fonttools/ttfautohint-py)
-* [dehinter](https://github.com/source-foundry/dehinter)
-* [beziers](https://github.com/simoncozens/beziers.py)
-
-The command line interface is built with [click](https://github.com/pallets/click/) and tables are rendered by
-[rich](https://github.com/Textualize/rich).
-
-Even if not directly imported to keep the footprint as small as possible, portions of code have been copied from
-[fontbakery](https://github.com/googlefonts/fontbakery).
-
-## Installation
-FoundryTools-CLI requires Python 3.9 or later.
-
-**Note for Windows users**: installation on Python 3.11 is strongly discouraged because AFDKO 3.9.6 doesn't support
-it, and an attempt of installation would probably fail. Since macOS users successfully installed FoundryTools-CLI on
-Python 3.11, requirements have been loosened up.
-
-### pip
-FoundryTools-CLI releases are available on the Python Package Index (PyPI), so it can be installed with
-[pip](https://pip.pypa.io/):
-
-    python -m pip install foundrytools-cli
-
-### Editable mode
-If you would like to contribute to the development, you can clone the repository from GitHub, install the package in
-'editable' mode and modify the source code in place. We strongly recommend using a virtual environment.
-
-    # clone the repository:
-    git clone https://github.com/ftCLI/foundrytools-cli.git
-    cd foundrytools-cli
-
-    # create new virtual environment named e.g. ftcli-venv, or whatever you prefer:
-    python -m venv ftcli-venv
-    
-    # to activate the virtual environmtnet in macOS and Linux, do:
-    . ftcli-venv/bin/activate
-    
-    # to activate the virtual environment in Windows, do:
-    ftcli-venv\Scripts\activate.bat
-    
-    # install in 'editable' mode
-    python -m pip install -e .
-
-## Documentation
-FoundryTools-CLI is a Terminal app where commands are logically organized into subcommands.
-
-Please refer to the [user documentation](https://ft-cli.github.io).
-
-## License
-FoundryTools-CLI is available under the [MIT license](LICENSE)
-
-
-
+Metadata-Version: 2.1
+Name: foundrytools-cli
+Version: 1.0.1
+Summary: A set of command line tools to inspect, manipulate and convert font files
+Home-page: https://github.com/ftCLI/FoundryTools-CLI
+Author: ftCLI
+Author-email: ftcli@proton.me
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# FoundryTools-CLI
+FoundryTools-CLI, former known as ftCLI, is a collection of command line tools written in Python to inspect, manipulate
+and convert fonts. It takes advantage of the capabilities made available by other tools such as:
+
+* [FontTools](https://github.com/fonttools/fonttools)
+* [AFDKO](https://github.com/adobe-type-tools/afdko)
+* [skia-pathops](https://github.com/fonttools/skia-pathops)
+* [cffsubr](https://github.com/adobe-type-tools/cffsubr)
+* [psautohint](https://github.com/adobe-type-tools/psautohint)
+* [ttfautohint-py](https://github.com/fonttools/ttfautohint-py)
+* [dehinter](https://github.com/source-foundry/dehinter)
+* [beziers](https://github.com/simoncozens/beziers.py)
+
+The command line interface is built with [click](https://github.com/pallets/click/) and tables are rendered by
+[rich](https://github.com/Textualize/rich).
+
+Even if not directly imported to keep the footprint as small as possible, portions of code have been copied from
+[fontbakery](https://github.com/googlefonts/fontbakery).
+
+## Installation
+FoundryTools-CLI requires Python 3.9 or later.
+
+**Note for Windows users**: installation on Python 3.11 is strongly discouraged because AFDKO 3.9.6 doesn't support
+it, and an attempt of installation would probably fail. Since macOS users successfully installed FoundryTools-CLI on
+Python 3.11, requirements have been loosened up.
+
+### pip
+FoundryTools-CLI releases are available on the Python Package Index (PyPI), so it can be installed with
+[pip](https://pip.pypa.io/):
+
+    python -m pip install foundrytools-cli
+
+### Editable mode
+If you would like to contribute to the development, you can clone the repository from GitHub, install the package in
+'editable' mode and modify the source code in place. We strongly recommend using a virtual environment.
+
+    # clone the repository:
+    git clone https://github.com/ftCLI/foundrytools-cli.git
+    cd foundrytools-cli
+
+    # create new virtual environment named e.g. ftcli-venv, or whatever you prefer:
+    python -m venv ftcli-venv
+    
+    # to activate the virtual environmtnet in macOS and Linux, do:
+    . ftcli-venv/bin/activate
+    
+    # to activate the virtual environment in Windows, do:
+    ftcli-venv\Scripts\activate.bat
+    
+    # install in 'editable' mode
+    python -m pip install -e .
+
+## Documentation
+FoundryTools-CLI is a Terminal app where commands are logically organized into subcommands.
+
+Please refer to the [user documentation](https://ftcli.github.io/FoundryTools-CLI/).
+
+## License
+FoundryTools-CLI is available under the [MIT license](LICENSE)
+
+## Credits
+To Sergiev. May You rest in peace.
+
+
+
```

### Comparing `foundrytools-cli-1.0.0/README.md` & `foundrytools-cli-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,65 @@
-# FoundryTools-CLI
-FoundryTools-CLI, former known as ftCLI, is a collection of command line tools written in Python to inspect, manipulate
-and convert fonts. It takes advantage of the capabilities made available by other tools such as:
-
-* [FontTools](https://github.com/fonttools/fonttools)
-* [AFDKO](https://github.com/adobe-type-tools/afdko)
-* [skia-pathops](https://github.com/fonttools/skia-pathops)
-* [cffsubr](https://github.com/adobe-type-tools/cffsubr)
-* [psautohint](https://github.com/adobe-type-tools/psautohint)
-* [ttfautohint-py](https://github.com/fonttools/ttfautohint-py)
-* [dehinter](https://github.com/source-foundry/dehinter)
-* [beziers](https://github.com/simoncozens/beziers.py)
-
-The command line interface is built with [click](https://github.com/pallets/click/) and tables are rendered by
-[rich](https://github.com/Textualize/rich).
-
-Even if not directly imported to keep the footprint as small as possible, portions of code have been copied from
-[fontbakery](https://github.com/googlefonts/fontbakery).
-
-## Installation
-FoundryTools-CLI requires Python 3.9 or later.
-
-**Note for Windows users**: installation on Python 3.11 is strongly discouraged because AFDKO 3.9.6 doesn't support
-it, and an attempt of installation would probably fail. Since macOS users successfully installed FoundryTools-CLI on
-Python 3.11, requirements have been loosened up.
-
-### pip
-FoundryTools-CLI releases are available on the Python Package Index (PyPI), so it can be installed with
-[pip](https://pip.pypa.io/):
-
-    python -m pip install foundrytools-cli
-
-### Editable mode
-If you would like to contribute to the development, you can clone the repository from GitHub, install the package in
-'editable' mode and modify the source code in place. We strongly recommend using a virtual environment.
-
-    # clone the repository:
-    git clone https://github.com/ftCLI/foundrytools-cli.git
-    cd foundrytools-cli
-
-    # create new virtual environment named e.g. ftcli-venv, or whatever you prefer:
-    python -m venv ftcli-venv
-    
-    # to activate the virtual environmtnet in macOS and Linux, do:
-    . ftcli-venv/bin/activate
-    
-    # to activate the virtual environment in Windows, do:
-    ftcli-venv\Scripts\activate.bat
-    
-    # install in 'editable' mode
-    python -m pip install -e .
-
-## Documentation
-FoundryTools-CLI is a Terminal app where commands are logically organized into subcommands.
-
-Please refer to the [user documentation](https://ft-cli.github.io).
-
-## License
-FoundryTools-CLI is available under the [MIT license](LICENSE)
-
-
-
+# FoundryTools-CLI
+FoundryTools-CLI, former known as ftCLI, is a collection of command line tools written in Python to inspect, manipulate
+and convert fonts. It takes advantage of the capabilities made available by other tools such as:
+
+* [FontTools](https://github.com/fonttools/fonttools)
+* [AFDKO](https://github.com/adobe-type-tools/afdko)
+* [skia-pathops](https://github.com/fonttools/skia-pathops)
+* [cffsubr](https://github.com/adobe-type-tools/cffsubr)
+* [psautohint](https://github.com/adobe-type-tools/psautohint)
+* [ttfautohint-py](https://github.com/fonttools/ttfautohint-py)
+* [dehinter](https://github.com/source-foundry/dehinter)
+* [beziers](https://github.com/simoncozens/beziers.py)
+
+The command line interface is built with [click](https://github.com/pallets/click/) and tables are rendered by
+[rich](https://github.com/Textualize/rich).
+
+Even if not directly imported to keep the footprint as small as possible, portions of code have been copied from
+[fontbakery](https://github.com/googlefonts/fontbakery).
+
+## Installation
+FoundryTools-CLI requires Python 3.9 or later.
+
+**Note for Windows users**: installation on Python 3.11 is strongly discouraged because AFDKO 3.9.6 doesn't support
+it, and an attempt of installation would probably fail. Since macOS users successfully installed FoundryTools-CLI on
+Python 3.11, requirements have been loosened up.
+
+### pip
+FoundryTools-CLI releases are available on the Python Package Index (PyPI), so it can be installed with
+[pip](https://pip.pypa.io/):
+
+    python -m pip install foundrytools-cli
+
+### Editable mode
+If you would like to contribute to the development, you can clone the repository from GitHub, install the package in
+'editable' mode and modify the source code in place. We strongly recommend using a virtual environment.
+
+    # clone the repository:
+    git clone https://github.com/ftCLI/foundrytools-cli.git
+    cd foundrytools-cli
+
+    # create new virtual environment named e.g. ftcli-venv, or whatever you prefer:
+    python -m venv ftcli-venv
+    
+    # to activate the virtual environmtnet in macOS and Linux, do:
+    . ftcli-venv/bin/activate
+    
+    # to activate the virtual environment in Windows, do:
+    ftcli-venv\Scripts\activate.bat
+    
+    # install in 'editable' mode
+    python -m pip install -e .
+
+## Documentation
+FoundryTools-CLI is a Terminal app where commands are logically organized into subcommands.
+
+Please refer to the [user documentation](https://ftcli.github.io/FoundryTools-CLI/).
+
+## License
+FoundryTools-CLI is available under the [MIT license](LICENSE)
+
+## Credits
+To Sergiev. May You rest in peace.
+
+
+
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_assistant.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_assistant.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,376 +1,375 @@
-import os
-from copy import copy, deepcopy
-from pathlib import Path
-
-import click
-from fontTools.misc.cliTools import makeOutputFileName
-
-from foundryToolsCLI.Lib.Font import Font
-from foundryToolsCLI.Lib.assistant.UI import AssistantUI
-from foundryToolsCLI.Lib.assistant.fonts_data import FontsData
-from foundryToolsCLI.Lib.assistant.styles_mapping import StylesMapping
-from foundryToolsCLI.Lib.utils.cli_tools import (
-    get_style_mapping_path,
-    get_fonts_data_path,
-    get_output_dir,
-)
-from foundryToolsCLI.Lib.utils.click_tools import (
-    add_file_or_path_argument,
-    add_common_options,
-    file_overwrite_prompt,
-    generic_error_message,
-    file_saved_message,
-    file_not_changed_message,
-    generic_warning_message,
-    file_not_selected_message,
-    add_path_argument,
-)
-
-CWD = Path.cwd()
-assistant = click.Group("subcommands")
-
-
-@assistant.command()
-@add_file_or_path_argument()
-@click.option(
-    "-q",
-    "--quiet",
-    is_flag=True,
-    help="""
-    Suppress the overwrite confirmation message if the fonts_data.csv and/or styles_mapping.json files already
-    exist in the ftCLI_files folder.""",
-)
-def init(input_path, quiet=False):
-    """
-    Creates the 'styles_mapping.json' and the 'fonts_data.csv' files in the 'ftCLI_files' directory. If one or both
-    files already exist, user will be asked to overwrite.
-
-    Both files can be edited manually or using the 'ftcli assistant ui' command.
-    """
-
-    try:
-        styles_mapping_file = get_style_mapping_path(input_path)
-        styles_mapping = StylesMapping(styles_mapping_file)
-        if Path.exists(styles_mapping_file) and quiet is False:
-            styles_mapping_overwrite = file_overwrite_prompt(styles_mapping_file)
-        else:
-            styles_mapping_overwrite = True
-
-        if styles_mapping_overwrite is True:
-            styles_mapping.reset_defaults()
-            file_saved_message(styles_mapping_file.relative_to(CWD))
-        else:
-            file_not_changed_message(styles_mapping_file.relative_to(CWD))
-
-        fonts_data_file = get_fonts_data_path(input_path)
-        fonts_data = FontsData(fonts_data_file)
-        if Path.exists(fonts_data_file) and not quiet:
-            fonts_data_overwrite = file_overwrite_prompt(fonts_data_file)
-        else:
-            fonts_data_overwrite = True
-        if fonts_data_overwrite is True:
-            fonts_data.reset_data(styles_mapping=styles_mapping)
-            file_saved_message(fonts_data_file.relative_to(CWD))
-        else:
-            file_not_changed_message(fonts_data_file.relative_to(CWD))
-    except Exception as e:
-        generic_error_message(e)
-
-
-@assistant.command()
-@add_path_argument()
-@click.option(
-    "--width-elidable",
-    default="Normal",
-    show_default=True,
-    help="""The width word to elide when building the namerecords.""",
-)
-@click.option(
-    "--weight-elidable",
-    default="Regular",
-    show_default=True,
-    help="""The weight word to elide when building the namerecords.""",
-)
-@click.option(
-    "-ls",
-    "--linked-styles",
-    type=(click.IntRange(1, 1000), click.IntRange(1, 1000)),
-    help="""Use this option to activate linked styles. If this option is active, linked styles must be specified. For
-    example: -ls 400 700, or -ls 300 600.
-    """,
-)
-@click.option(
-    "-x",
-    "--exclude-namerecords",
-    type=click.Choice(choices=["1", "2", "3", "4", "5", "6", "16", "17", "18"]),
-    multiple=True,
-    help="""
-    Name IDs to skip. The specified name IDs won't be recalculated. This option can be repeated (for example: -x 3 -x 5
-    -x 6...).
-    """,
-)
-@click.option(
-    "-swdt",
-    "--shorten-width",
-    type=click.Choice(choices=["1", "4", "6", "16", "17"]),
-    multiple=True,
-    help="""
-    Name IDs where to use the short word for width style name (for example, 'Cn' instead of 'Condensed'). This option
-    can be repeated (for example: -swdt 1 -swdt 5, -swdt 16...).
-    """,
-)
-@click.option(
-    "-swgt",
-    "--shorten-weight",
-    type=click.Choice(choices=["1", "4", "6", "17"]),
-    multiple=True,
-    help="""
-    Name IDs where to use the short word for weight style name (for example, 'Md' instead of 'Medium'). This option can
-    be repeated (for example: -swgt 1 -swgt 5 -swgt 6...).
-    """,
-)
-@click.option(
-    "-kwdt",
-    "--keep-width-elidable",
-    is_flag=True,
-    help="""
-    Doesn't remove the width elidable words (by default, "Nor" and "Normal").
-    """,
-)
-@click.option(
-    "-kwgt",
-    "--keep-weight-elidable",
-    is_flag=True,
-    help="""
-    Doesn't remove the weight elidable words (by default, "Rg" and "Regular").
-    """,
-)
-@click.option(
-    "-sslp",
-    "--shorten-slope",
-    type=click.Choice(choices=["4", "6", "16", "17"]),
-    multiple=True,
-    help="""
-    Name IDs where to use the short word for slope style name (for example, 'It' instead of 'Italic'). This option can
-    be repeated (for example: -sslp 3 -sslp 5 -sslp 6...).
-    """,
-)
-@click.option(
-    "-sf",
-    "--super-family",
-    is_flag=True,
-    help="""
-    Superfamily mode. This option affects name IDs 3, 6, 16 and 17 in case of families with widths different than
-    'Normal'. If this option is active, name ID 6 will be 'FamilyName-WidthWeightSlope' instead of
-    'FamilyNameWidth-WeightSlope'. Mac and OT family/subfamily names will be FamilyName /  Width Weight Slope' instead
-    of 'Family Name Width / Weight Slope'.
-    """,
-)
-@click.option(
-    "-aui",
-    "--alt-uid",
-    is_flag=True,
-    help="""
-    Use alternate unique identifier. By default, nameID 3 (Unique identifier) is calculated according to the following
-    scheme: 'Version;Vendor code;PostscriptName'. The alternate unique identifier is calculated according to the
-    following scheme: 'Manufacturer: Full Font Name: Creation Year'.
-    """,
-)
-@click.option(
-    "-obni",
-    "--oblique-not-italic",
-    is_flag=True,
-    help="""
-    By default, if a font has the oblique bit set, the italic bits will be set too. Use this option to override the
-    default behaviour (for example, when the family has both italic and oblique styles and you need to keep oblique and
-    italic styles separate). The italic bits will be cleared when the oblique bit is set.
-    """,
-)
-@click.option(
-    "--no-auto-shorten",
-    "auto_shorten",
-    is_flag=True,
-    default=True,
-    help="""
-    When name id 1, 4 or 6 are longer than maximum allowed (27 characters for nameID 1, 31 for nameID 4 and 29 for
-    nameID 6), the script tries to auto shorten those names replacing long words with short words. Use this option to
-    prevent the script from auto shortening names.
-    """,
-)
-@click.option(
-    "-cff",
-    is_flag=True,
-    help="""
-    If this option is active, fontNames, FullName, FamilyName and Weight values in the 'CFF' table will be recalculated.
-    """,
-)
-@add_common_options()
-def commit(
-    input_path: Path,
-    width_elidable: str,
-    weight_elidable: str,
-    linked_styles: list = None,
-    exclude_namerecords=None,
-    shorten_width=None,
-    shorten_weight=None,
-    keep_width_elidable=False,
-    keep_weight_elidable=False,
-    shorten_slope=None,
-    super_family=False,
-    alt_uid=False,
-    oblique_not_italic=False,
-    auto_shorten=True,
-    cff=False,
-    output_dir=None,
-    recalc_timestamp=False,
-    overwrite=True,
-):
-    """
-    Writes data from CSV to fonts.
-    """
-
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    try:
-        output_dir.mkdir(exist_ok=True)
-    except Exception as e:
-        generic_error_message(e)
-
-    if linked_styles:
-        linked_styles = sorted(linked_styles)
-    if exclude_namerecords:
-        exclude_namerecords = sorted(set(int(i) for i in exclude_namerecords))
-    if shorten_width:
-        shorten_width = sorted(set(int(i) for i in shorten_width))
-    if shorten_weight:
-        shorten_weight = sorted(set(int(i) for i in shorten_weight))
-    if shorten_slope:
-        shorten_slope = sorted(set(int(i) for i in shorten_slope))
-
-    try:
-        fonts_data = FontsData(get_fonts_data_path(input_path))
-        data = fonts_data.get_data()
-    except Exception as e:
-        generic_error_message(e)
-        return
-
-    for row in data:
-        file = Path(row["file_name"])
-        if not Path.exists(file):
-            generic_warning_message(f"{file} {click.style('file does not exist', fg='yellow')}")
-            continue
-
-        file_is_selected = bool(int(row["selected"]))
-        if not file_is_selected:
-            file_not_selected_message(file)
-            continue
-
-        try:
-            font = Font(file, recalcTimestamp=recalc_timestamp)
-
-            name_table = font["name"]
-            name_table_copy = deepcopy(name_table)
-            os2_table = font["OS/2"]
-            os2_table_copy = copy(os2_table)
-            head_table = font["head"]
-            head_table_copy = copy(head_table)
-            if not font.is_otf:
-                cff_table_copy = None
-            else:
-                cff_table_copy = deepcopy(font["CFF "])
-
-            fonts_data.write_data_to_font(
-                font=font,
-                row=row,
-                width_elidable=width_elidable,
-                weight_elidable=weight_elidable,
-                keep_width_elidable=keep_width_elidable,
-                keep_weight_elidable=keep_weight_elidable,
-                linked_styles=linked_styles,
-                exclude_namerecords=exclude_namerecords,
-                shorten_width=shorten_width,
-                shorten_weight=shorten_weight,
-                shorten_slope=shorten_slope,
-                super_family=super_family,
-                auto_shorten=auto_shorten,
-                alt_uid=alt_uid,
-                oblique_not_italic=oblique_not_italic,
-                cff=cff,
-            )
-
-            font_has_changed = False
-
-            if os2_table != os2_table_copy:
-                font_has_changed = True
-            if head_table != head_table_copy:
-                font_has_changed = True
-            if name_table.compile(font) != name_table_copy.compile(font):
-                font_has_changed = True
-            if cff_table_copy:
-                if cff_table_copy.compile(font) != font["CFF "].compile(font):
-                    font_has_changed = True
-
-            if font_has_changed:
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file)
-
-        except Exception as e:
-            generic_error_message(e)
-
-
-@assistant.command()
-@add_file_or_path_argument()
-def ui(input_path: Path):
-    """
-    Opens the character user interface to edit the styles_mapping.json and fonts_data.csv files.
-    """
-
-    styles_mapping_file = get_style_mapping_path(input_path)
-    if not os.path.exists(styles_mapping_file):
-        StylesMapping(styles_mapping_file).reset_defaults()
-
-    fonts_data_file = get_fonts_data_path(input_path)
-    if not os.path.exists(fonts_data_file):
-        FontsData(fonts_data_file).reset_data()
-
-    AssistantUI(input_path).run()
-
-
-cli = click.CommandCollection(
-    sources=[assistant],
-    help="""
-Helps the user to correctly compile 'name' table and to set the proper values for usWeightClass, usWidthClass, bold,
-italic and oblique flags.
-
-The first step consists in creating two files in a folder named ftCLI_files under the current directory:
-
-1) ``styles_mapping.json``: contains the default Style Names to pair with usWidthClass, usWeightClass and Slope
-class (e.g.: 500: Md, Medium; 3: Cnd, Condensed; It, Italic; Obl, Oblique).
-
-2) ``fonts_data.csv``: is a CSV file containing the following columns:
-
-* 'file_name': path the font file\n
-* 'family_name': family name (read from the font)\n
-* 'is_bold': bold flag (read from the font: "1" if the bold flag is set, "0" it the bold flag is clear)\n
-* 'is_italic': italic flag (read from the font: "1" if the italic flag is set, "0" it the italic flag is clear)\n
-* 'is_oblique': oblique flag (read from the font: "1" if the oblique flag is set, "0" it the oblique flag is clear)\n
-* 'us_width_class': usWidthClass value (read from the font)\n
-* 'wdt': short word for width style name (read from styles_mapping.json, if usWidthClass is present)\n
-* 'width': long word for width style name (read from styles_mapping.json, if usWidthClass is present)\n
-* 'us_weight_class': usWeightClass value (read from the font)\n
-* 'wgt': short word for weight style name (read from styles_mapping.json, if usWeightClass is present)\n
-* 'weight': long word for weight style name (read from styles_mapping.json, if usWeightClass is present)\n
-* 'slp': short word for slope class (read from styles_mapping.json. None if the font is not italic nor oblique)\n
-* 'slope': long word for slope class (read from styles_mapping.json. None if the font is not italic nor oblique)\n
-* 'selected': "1" to select the file, "0" to deselect (it will not be processed by ftcli assistant commit)\n
-
-Files can be created with ``ftcli assistant init INPUT_PATH`` or ``ftcli assistant ui INPUT_PATH``. The first command
-will create both files (if one or both already exist, user will be prompted for overwrite). The second command will
-create the files (unless they already exist) and will open the editor.
-
-When the data in the 'fonts_data.csv' file are filled as desired by the user, fonts can be patched running the
-``ftcli assistant commit`` command.
-""",
-)
+import os
+from copy import copy, deepcopy
+from pathlib import Path
+
+import click
+from fontTools.misc.cliTools import makeOutputFileName
+
+from foundryToolsCLI.Lib.Font import Font
+from foundryToolsCLI.Lib.assistant.UI import AssistantUI
+from foundryToolsCLI.Lib.assistant.fonts_data import FontsData
+from foundryToolsCLI.Lib.assistant.styles_mapping import StylesMapping
+from foundryToolsCLI.Lib.utils.cli_tools import (
+    get_style_mapping_path,
+    get_fonts_data_path,
+    get_output_dir,
+)
+from foundryToolsCLI.Lib.utils.click_tools import (
+    add_file_or_path_argument,
+    add_common_options,
+    file_overwrite_prompt,
+    generic_error_message,
+    file_saved_message,
+    file_not_changed_message,
+    generic_warning_message,
+    file_not_selected_message,
+    add_path_argument,
+)
+
+assistant = click.Group("subcommands")
+
+
+@assistant.command()
+@add_file_or_path_argument()
+@click.option(
+    "-q",
+    "--quiet",
+    is_flag=True,
+    help="""
+    Suppress the overwrite confirmation message if the fonts_data.csv and/or styles_mapping.json files already
+    exist in the ftCLI_files folder.""",
+)
+def init(input_path, quiet=False):
+    """
+    Creates the 'styles_mapping.json' and the 'fonts_data.csv' files in the 'ftCLI_files' directory. If one or both
+    files already exist, user will be asked to overwrite.
+
+    Both files can be edited manually or using the 'ftcli assistant ui' command.
+    """
+
+    try:
+        styles_mapping_file = get_style_mapping_path(input_path)
+        styles_mapping = StylesMapping(styles_mapping_file)
+        if Path.exists(styles_mapping_file) and quiet is False:
+            styles_mapping_overwrite = file_overwrite_prompt(styles_mapping_file)
+        else:
+            styles_mapping_overwrite = True
+
+        if styles_mapping_overwrite is True:
+            styles_mapping.reset_defaults()
+            file_saved_message(styles_mapping_file)
+        else:
+            file_not_changed_message(styles_mapping_file)
+
+        fonts_data_file = get_fonts_data_path(input_path)
+        fonts_data = FontsData(fonts_data_file)
+        if Path.exists(fonts_data_file) and not quiet:
+            fonts_data_overwrite = file_overwrite_prompt(fonts_data_file)
+        else:
+            fonts_data_overwrite = True
+        if fonts_data_overwrite is True:
+            fonts_data.reset_data(styles_mapping=styles_mapping)
+            file_saved_message(fonts_data_file)
+        else:
+            file_not_changed_message(fonts_data_file)
+    except Exception as e:
+        generic_error_message(e)
+
+
+@assistant.command()
+@add_path_argument()
+@click.option(
+    "--width-elidable",
+    default="Normal",
+    show_default=True,
+    help="""The width word to elide when building the namerecords.""",
+)
+@click.option(
+    "--weight-elidable",
+    default="Regular",
+    show_default=True,
+    help="""The weight word to elide when building the namerecords.""",
+)
+@click.option(
+    "-ls",
+    "--linked-styles",
+    type=(click.IntRange(1, 1000), click.IntRange(1, 1000)),
+    help="""Use this option to activate linked styles. If this option is active, linked styles must be specified. For
+    example: -ls 400 700, or -ls 300 600.
+    """,
+)
+@click.option(
+    "-x",
+    "--exclude-namerecords",
+    type=click.Choice(choices=["1", "2", "3", "4", "5", "6", "16", "17", "18"]),
+    multiple=True,
+    help="""
+    Name IDs to skip. The specified name IDs won't be recalculated. This option can be repeated (for example: -x 3 -x 5
+    -x 6...).
+    """,
+)
+@click.option(
+    "-swdt",
+    "--shorten-width",
+    type=click.Choice(choices=["1", "4", "6", "16", "17"]),
+    multiple=True,
+    help="""
+    Name IDs where to use the short word for width style name (for example, 'Cn' instead of 'Condensed'). This option
+    can be repeated (for example: -swdt 1 -swdt 5, -swdt 16...).
+    """,
+)
+@click.option(
+    "-swgt",
+    "--shorten-weight",
+    type=click.Choice(choices=["1", "4", "6", "17"]),
+    multiple=True,
+    help="""
+    Name IDs where to use the short word for weight style name (for example, 'Md' instead of 'Medium'). This option can
+    be repeated (for example: -swgt 1 -swgt 5 -swgt 6...).
+    """,
+)
+@click.option(
+    "-kwdt",
+    "--keep-width-elidable",
+    is_flag=True,
+    help="""
+    Doesn't remove the width elidable words (by default, "Nor" and "Normal").
+    """,
+)
+@click.option(
+    "-kwgt",
+    "--keep-weight-elidable",
+    is_flag=True,
+    help="""
+    Doesn't remove the weight elidable words (by default, "Rg" and "Regular").
+    """,
+)
+@click.option(
+    "-sslp",
+    "--shorten-slope",
+    type=click.Choice(choices=["4", "6", "16", "17"]),
+    multiple=True,
+    help="""
+    Name IDs where to use the short word for slope style name (for example, 'It' instead of 'Italic'). This option can
+    be repeated (for example: -sslp 3 -sslp 5 -sslp 6...).
+    """,
+)
+@click.option(
+    "-sf",
+    "--super-family",
+    is_flag=True,
+    help="""
+    Superfamily mode. This option affects name IDs 3, 6, 16 and 17 in case of families with widths different than
+    'Normal'. If this option is active, name ID 6 will be 'FamilyName-WidthWeightSlope' instead of
+    'FamilyNameWidth-WeightSlope'. Mac and OT family/subfamily names will be FamilyName /  Width Weight Slope' instead
+    of 'Family Name Width / Weight Slope'.
+    """,
+)
+@click.option(
+    "-aui",
+    "--alt-uid",
+    is_flag=True,
+    help="""
+    Use alternate unique identifier. By default, nameID 3 (Unique identifier) is calculated according to the following
+    scheme: 'Version;Vendor code;PostscriptName'. The alternate unique identifier is calculated according to the
+    following scheme: 'Manufacturer: Full Font Name: Creation Year'.
+    """,
+)
+@click.option(
+    "-obni",
+    "--oblique-not-italic",
+    is_flag=True,
+    help="""
+    By default, if a font has the oblique bit set, the italic bits will be set too. Use this option to override the
+    default behaviour (for example, when the family has both italic and oblique styles and you need to keep oblique and
+    italic styles separate). The italic bits will be cleared when the oblique bit is set.
+    """,
+)
+@click.option(
+    "--no-auto-shorten",
+    "auto_shorten",
+    is_flag=True,
+    default=True,
+    help="""
+    When name id 1, 4 or 6 are longer than maximum allowed (27 characters for nameID 1, 31 for nameID 4 and 29 for
+    nameID 6), the script tries to auto shorten those names replacing long words with short words. Use this option to
+    prevent the script from auto shortening names.
+    """,
+)
+@click.option(
+    "-cff",
+    is_flag=True,
+    help="""
+    If this option is active, fontNames, FullName, FamilyName and Weight values in the 'CFF' table will be recalculated.
+    """,
+)
+@add_common_options()
+def commit(
+    input_path: Path,
+    width_elidable: str,
+    weight_elidable: str,
+    linked_styles: list = None,
+    exclude_namerecords=None,
+    shorten_width=None,
+    shorten_weight=None,
+    keep_width_elidable=False,
+    keep_weight_elidable=False,
+    shorten_slope=None,
+    super_family=False,
+    alt_uid=False,
+    oblique_not_italic=False,
+    auto_shorten=True,
+    cff=False,
+    output_dir=None,
+    recalc_timestamp=False,
+    overwrite=True,
+):
+    """
+    Writes data from CSV to fonts.
+    """
+
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    try:
+        output_dir.mkdir(exist_ok=True)
+    except Exception as e:
+        generic_error_message(e)
+
+    if linked_styles:
+        linked_styles = sorted(linked_styles)
+    if exclude_namerecords:
+        exclude_namerecords = sorted(set(int(i) for i in exclude_namerecords))
+    if shorten_width:
+        shorten_width = sorted(set(int(i) for i in shorten_width))
+    if shorten_weight:
+        shorten_weight = sorted(set(int(i) for i in shorten_weight))
+    if shorten_slope:
+        shorten_slope = sorted(set(int(i) for i in shorten_slope))
+
+    try:
+        fonts_data = FontsData(get_fonts_data_path(input_path))
+        data = fonts_data.get_data()
+    except Exception as e:
+        generic_error_message(e)
+        return
+
+    for row in data:
+        file = Path(row["file_name"])
+        if not Path.exists(file):
+            generic_warning_message(f"{file} {click.style('file does not exist', fg='yellow')}")
+            continue
+
+        file_is_selected = bool(int(row["selected"]))
+        if not file_is_selected:
+            file_not_selected_message(file)
+            continue
+
+        try:
+            font = Font(file, recalcTimestamp=recalc_timestamp)
+
+            name_table = font["name"]
+            name_table_copy = deepcopy(name_table)
+            os2_table = font["OS/2"]
+            os2_table_copy = copy(os2_table)
+            head_table = font["head"]
+            head_table_copy = copy(head_table)
+            if not font.is_otf:
+                cff_table_copy = None
+            else:
+                cff_table_copy = deepcopy(font["CFF "])
+
+            fonts_data.write_data_to_font(
+                font=font,
+                row=row,
+                width_elidable=width_elidable,
+                weight_elidable=weight_elidable,
+                keep_width_elidable=keep_width_elidable,
+                keep_weight_elidable=keep_weight_elidable,
+                linked_styles=linked_styles,
+                exclude_namerecords=exclude_namerecords,
+                shorten_width=shorten_width,
+                shorten_weight=shorten_weight,
+                shorten_slope=shorten_slope,
+                super_family=super_family,
+                auto_shorten=auto_shorten,
+                alt_uid=alt_uid,
+                oblique_not_italic=oblique_not_italic,
+                cff=cff,
+            )
+
+            font_has_changed = False
+
+            if os2_table != os2_table_copy:
+                font_has_changed = True
+            if head_table != head_table_copy:
+                font_has_changed = True
+            if name_table.compile(font) != name_table_copy.compile(font):
+                font_has_changed = True
+            if cff_table_copy:
+                if cff_table_copy.compile(font) != font["CFF "].compile(font):
+                    font_has_changed = True
+
+            if font_has_changed:
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+
+
+@assistant.command()
+@add_file_or_path_argument()
+def ui(input_path: Path):
+    """
+    Opens the character user interface to edit the styles_mapping.json and fonts_data.csv files.
+    """
+
+    styles_mapping_file = get_style_mapping_path(input_path)
+    if not os.path.exists(styles_mapping_file):
+        StylesMapping(styles_mapping_file).reset_defaults()
+
+    fonts_data_file = get_fonts_data_path(input_path)
+    if not os.path.exists(fonts_data_file):
+        FontsData(fonts_data_file).reset_data()
+
+    AssistantUI(input_path).run()
+
+
+cli = click.CommandCollection(
+    sources=[assistant],
+    help="""
+Helps the user to correctly compile 'name' table and to set the proper values for usWeightClass, usWidthClass, bold,
+italic and oblique flags.
+
+The first step consists in creating two files in a folder named ftCLI_files under the current directory:
+
+1) ``styles_mapping.json``: contains the default Style Names to pair with usWidthClass, usWeightClass and Slope
+class (e.g.: 500: Md, Medium; 3: Cnd, Condensed; It, Italic; Obl, Oblique).
+
+2) ``fonts_data.csv``: is a CSV file containing the following columns:
+
+* 'file_name': path the font file\n
+* 'family_name': family name (read from the font)\n
+* 'is_bold': bold flag (read from the font: "1" if the bold flag is set, "0" it the bold flag is clear)\n
+* 'is_italic': italic flag (read from the font: "1" if the italic flag is set, "0" it the italic flag is clear)\n
+* 'is_oblique': oblique flag (read from the font: "1" if the oblique flag is set, "0" it the oblique flag is clear)\n
+* 'us_width_class': usWidthClass value (read from the font)\n
+* 'wdt': short word for width style name (read from styles_mapping.json, if usWidthClass is present)\n
+* 'width': long word for width style name (read from styles_mapping.json, if usWidthClass is present)\n
+* 'us_weight_class': usWeightClass value (read from the font)\n
+* 'wgt': short word for weight style name (read from styles_mapping.json, if usWeightClass is present)\n
+* 'weight': long word for weight style name (read from styles_mapping.json, if usWeightClass is present)\n
+* 'slp': short word for slope class (read from styles_mapping.json. None if the font is not italic nor oblique)\n
+* 'slope': long word for slope class (read from styles_mapping.json. None if the font is not italic nor oblique)\n
+* 'selected': "1" to select the file, "0" to deselect (it will not be processed by ftcli assistant commit)\n
+
+Files can be created with ``ftcli assistant init INPUT_PATH`` or ``ftcli assistant ui INPUT_PATH``. The first command
+will create both files (if one or both already exist, user will be prompted for overwrite). The second command will
+create the files (unless they already exist) and will open the editor.
+
+When the data in the 'fonts_data.csv' file are filled as desired by the user, fonts can be patched running the
+``ftcli assistant commit`` command.
+""",
+)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_cff.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_cff.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,184 +1,183 @@
-from copy import deepcopy
-from pathlib import Path
-
-import click
-from fontTools.misc.cliTools import makeOutputFileName
-
-from foundryToolsCLI.Lib.tables.CFF_ import TableCFF
-from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
-from foundryToolsCLI.Lib.utils.click_tools import (
-    add_file_or_path_argument,
-    add_common_options,
-    generic_error_message,
-    file_saved_message,
-    file_not_changed_message,
-)
-
-CWD = Path.cwd()
-tbl_cff = click.Group("subcommands")
-
-
-@tbl_cff.command()
-@add_file_or_path_argument()
-@click.option("--full-name", "FullName", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] FullName")
-@click.option("--family-name", "FamilyName", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] FamilyName")
-@click.option("--weight", "Weight", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] Weight")
-@click.option("--version", "version", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] version")
-@click.option("--copyright", "Copyright", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] Copyright")
-@click.option("--notice", "Notice", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] Copyright")
-@add_common_options()
-def del_names(
-    input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True, **kwargs
-):
-    """
-    Deletes CFF names from topDict.
-    """
-    params = {k: v for k, v in kwargs.items() if v}
-    if len(params) == 0:
-        generic_error_message("Please, pass at least a valid parameter.")
-        return
-
-    fonts = get_fonts_in_path(
-        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False, allow_variable=False
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            cff_table: TableCFF = font["CFF "]
-            cff_table_copy = deepcopy(cff_table)
-
-            cff_table.del_top_dict_names(list(params.keys()))
-
-            if cff_table.compile(font) != cff_table_copy.compile(font):
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_cff.command()
-@add_file_or_path_argument()
-@click.option("--font-names", "fontNames", type=str, help="Sets CFF.cff.fontNames value")
-@click.option(
-    "--full-name",
-    "FullName",
-    type=str,
-    help="Sets CFF.cff.topDictIndex[0] FullName value",
-)
-@click.option(
-    "--family-name",
-    "FamilyName",
-    type=str,
-    help="Sets CFF.cff.topDictIndex[0] FamilyName value",
-)
-@click.option("--weight", "Weight", type=str, help="Sets CFF.cff.topDictIndex[0] Weight value")
-@click.option("--version", "version", type=str, help="Sets CFF.cff.topDictIndex[0] version value")
-@add_common_options()
-def set_names(
-    input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True, **kwargs
-):
-    """
-    Sets CFF names in topDict.
-    """
-
-    params = {k: v for k, v in kwargs.items() if v is not None}
-    if len(params) == 0:
-        generic_error_message("Please, pass at least a valid parameter.")
-        return
-
-    fonts = get_fonts_in_path(
-        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False, allow_variable=False
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            cff_table: TableCFF = font["CFF "]
-            cff_table_copy = deepcopy(cff_table)
-
-            cff_table.set_top_dict_names(params)
-
-            if cff_table.compile(font) != cff_table_copy.compile(font):
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_cff.command()
-@add_file_or_path_argument()
-@click.option("-os", "--old-string", required=True, help="The string to be replaced")
-@click.option(
-    "-ns",
-    "--new-string",
-    required=True,
-    help="The string to replace the old string with",
-    show_default=True,
-)
-@add_common_options()
-def find_replace(
-    input_path: Path,
-    old_string: str,
-    new_string: str,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Finds a string in the following items of CFF table topDict and replaces it with a new string: `version`, `FullName`,
-    `FamilyName`, `Weight`, `Copyright`, `Notice`.
-    """
-
-    fonts = get_fonts_in_path(
-        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False, allow_variable=False
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            cff_table: TableCFF = font["CFF "]
-            cff_table_copy = deepcopy(cff_table)
-
-            cff_table.top_dict_find_replace(old_string=old_string, new_string=new_string)
-
-            if cff_table.compile(font) != cff_table_copy.compile(font):
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-cli = click.CommandCollection(
-    sources=[tbl_cff],
-    help="""
-A set of command line tools to manipulate the 'CFF' table.
-""",
-)
+from copy import deepcopy
+from pathlib import Path
+
+import click
+from fontTools.misc.cliTools import makeOutputFileName
+
+from foundryToolsCLI.Lib.tables.CFF_ import TableCFF
+from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
+from foundryToolsCLI.Lib.utils.click_tools import (
+    add_file_or_path_argument,
+    add_common_options,
+    generic_error_message,
+    file_saved_message,
+    file_not_changed_message,
+)
+
+tbl_cff = click.Group("subcommands")
+
+
+@tbl_cff.command()
+@add_file_or_path_argument()
+@click.option("--full-name", "FullName", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] FullName")
+@click.option("--family-name", "FamilyName", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] FamilyName")
+@click.option("--weight", "Weight", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] Weight")
+@click.option("--version", "version", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] version")
+@click.option("--copyright", "Copyright", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] Copyright")
+@click.option("--notice", "Notice", is_flag=True, help="Deletes CFF.cff.topDictIndex[0] Copyright")
+@add_common_options()
+def del_names(
+    input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True, **kwargs
+):
+    """
+    Deletes CFF names from topDict.
+    """
+    params = {k: v for k, v in kwargs.items() if v}
+    if len(params) == 0:
+        generic_error_message("Please, pass at least a valid parameter.")
+        return
+
+    fonts = get_fonts_in_path(
+        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False, allow_variable=False
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            cff_table: TableCFF = font["CFF "]
+            cff_table_copy = deepcopy(cff_table)
+
+            cff_table.del_top_dict_names(list(params.keys()))
+
+            if cff_table.compile(font) != cff_table_copy.compile(font):
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_cff.command()
+@add_file_or_path_argument()
+@click.option("--font-names", "fontNames", type=str, help="Sets CFF.cff.fontNames value")
+@click.option(
+    "--full-name",
+    "FullName",
+    type=str,
+    help="Sets CFF.cff.topDictIndex[0] FullName value",
+)
+@click.option(
+    "--family-name",
+    "FamilyName",
+    type=str,
+    help="Sets CFF.cff.topDictIndex[0] FamilyName value",
+)
+@click.option("--weight", "Weight", type=str, help="Sets CFF.cff.topDictIndex[0] Weight value")
+@click.option("--version", "version", type=str, help="Sets CFF.cff.topDictIndex[0] version value")
+@add_common_options()
+def set_names(
+    input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True, **kwargs
+):
+    """
+    Sets CFF names in topDict.
+    """
+
+    params = {k: v for k, v in kwargs.items() if v is not None}
+    if len(params) == 0:
+        generic_error_message("Please, pass at least a valid parameter.")
+        return
+
+    fonts = get_fonts_in_path(
+        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False, allow_variable=False
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            cff_table: TableCFF = font["CFF "]
+            cff_table_copy = deepcopy(cff_table)
+
+            cff_table.set_top_dict_names(params)
+
+            if cff_table.compile(font) != cff_table_copy.compile(font):
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_cff.command()
+@add_file_or_path_argument()
+@click.option("-os", "--old-string", required=True, help="The string to be replaced")
+@click.option(
+    "-ns",
+    "--new-string",
+    required=True,
+    help="The string to replace the old string with",
+    show_default=True,
+)
+@add_common_options()
+def find_replace(
+    input_path: Path,
+    old_string: str,
+    new_string: str,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Finds a string in the following items of CFF table topDict and replaces it with a new string: `version`, `FullName`,
+    `FamilyName`, `Weight`, `Copyright`, `Notice`.
+    """
+
+    fonts = get_fonts_in_path(
+        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False, allow_variable=False
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            cff_table: TableCFF = font["CFF "]
+            cff_table_copy = deepcopy(cff_table)
+
+            cff_table.top_dict_find_replace(old_string=old_string, new_string=new_string)
+
+            if cff_table.compile(font) != cff_table_copy.compile(font):
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+cli = click.CommandCollection(
+    sources=[tbl_cff],
+    help="""
+A set of command line tools to manipulate the 'CFF' table.
+""",
+)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_converter.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_converter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,337 +1,336 @@
-import time
-from pathlib import Path
-
-import click
-
-from foundryToolsCLI.Lib.utils.cli_tools import (
-    get_fonts_in_path,
-    get_output_dir,
-    initial_check_pass,
-    get_variable_fonts_in_path,
-)
-from foundryToolsCLI.Lib.utils.click_tools import (
-    add_file_or_path_argument,
-    add_common_options,
-    generic_info_message,
-    select_instance_coordinates,
-    generic_error_message,
-)
-
-CWD = Path.cwd()
-font_converter = click.Group("subcommands")
-
-
-@font_converter.command()
-@add_file_or_path_argument()
-@click.option(
-    "-t",
-    "--tolerance",
-    type=click.FloatRange(0.0, 3.0),
-    default=1.0,
-    help="""
-    Conversion tolerance (0.0-3.0, default 1.0). Low tolerance adds more points but keeps shapes. High tolerance adds 
-    few points but may change shape.
-    """,
-)
-@click.option(
-    "--scale-upm", type=click.IntRange(1000, 4096, max_open=True), help="Scale the units-per-em of converted fonts."
-)
-@click.option("--no-subr", "subroutinize", is_flag=True, default=True, help="Do not subroutinize converted fonts.")
-@add_common_options()
-def ttf2otf(
-    input_path: Path,
-    tolerance: float = 1.0,
-    scale_upm: int = None,
-    subroutinize: bool = True,
-    recalc_timestamp: bool = False,
-    output_dir: Path = None,
-    overwrite: bool = True,
-):
-    """
-    Converts TTF fonts to OTF (or TrueType flavored woff/woff2 web fonts to PostScript flavored woff/woff2 web fonts).
-    """
-    fonts = get_fonts_in_path(
-        input_path=input_path, allow_cff=False, allow_variable=False, recalc_timestamp=recalc_timestamp
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    from foundryToolsCLI.Lib.converters.ttf_to_otf import TTF2OTFRunner
-
-    runner = TTF2OTFRunner()
-    runner.options.tolerance = tolerance
-    runner.options.scale_upm = scale_upm
-    runner.options.subroutinize = subroutinize
-    runner.options.recalc_timestamp = recalc_timestamp
-    runner.options.output_dir = output_dir
-    runner.options.overwrite = overwrite
-    runner.run(source_fonts=fonts)
-
-
-@font_converter.command()
-@add_file_or_path_argument()
-@click.option(
-    "--max-err",
-    type=click.FloatRange(0.1, 3.0),
-    default=1.0,
-    help="Approximation error, measured in UPEM",
-)
-@add_common_options()
-def otf2ttf(
-    input_path: Path,
-    max_err: float = 1.0,
-    recalc_timestamp: bool = False,
-    output_dir: Path = None,
-    overwrite: bool = True,
-):
-    """
-    Converts OTF fonts to TTF (or PostScripts flavored woff/woff2 web fonts to TrueType flavored woff/woff2 web fonts).
-    """
-    fonts = get_fonts_in_path(
-        input_path=input_path, allow_ttf=False, allow_variable=False, recalc_timestamp=recalc_timestamp
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    from foundryToolsCLI.Lib.converters.otf_to_ttf import OTF2TTFRunner
-
-    runner = OTF2TTFRunner()
-    runner.options.max_err = max_err
-    runner.options.output_dir = output_dir
-    runner.options.overwrite = overwrite
-    runner.run(source_fonts=fonts)
-
-
-@font_converter.command()
-@add_file_or_path_argument()
-@click.option(
-    "-s",
-    "--select-instance",
-    is_flag=True,
-    default=False,
-    help="""
-    By default, the script exports all named instances. Use this option to select custom axis values for a single
-    instance.
-    """,
-)
-@click.option(
-    "--no-cleanup",
-    "cleanup",
-    is_flag=True,
-    default=True,
-    help="""
-    By default, STAT table is dropped and axis nameIDs are deleted from name table. Use --no-cleanup to keep STAT table
-    and prevent axis nameIDs to be deleted from name table.
-    """,
-)
-@click.option(
-    "--no-update-name-table",
-    "update_name_table",
-    is_flag=True,
-    default=True,
-    help="""
-    Prevent updating instantiated fonts `name` table. Input fonts must have a STAT table with Axis Value Tables.
-    """,
-)
-@add_common_options()
-def vf2i(
-    input_path: Path,
-    select_instance: bool = False,
-    cleanup: bool = True,
-    update_name_table: bool = True,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Exports static instances from variable fonts.
-    """
-    variable_fonts = get_variable_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=variable_fonts, output_dir=output_dir):
-        return
-
-    from foundryToolsCLI.Lib.converters.variable_to_static import VariableToStatic
-    from fontTools.ttLib.tables._f_v_a_r import NamedInstance
-
-    start_time = time.time()
-    for variable_font in variable_fonts:
-        print()
-        file = Path(variable_font.reader.file.name)
-        generic_info_message(f"Converting file {file.name}")
-        try:
-            converter = VariableToStatic()
-            converter.options.cleanup = cleanup
-            converter.options.update_name_table = update_name_table
-            converter.options.output_dir = output_dir
-            converter.options.overwrite = overwrite
-
-            instances = variable_font.get_instances()
-            if select_instance:
-                axes = variable_font.get_axes()
-                selected_coordinates = select_instance_coordinates(axes)
-                is_named_instance = selected_coordinates in [i.coordinates for i in instances]
-                if not is_named_instance:
-                    # Set update_name_table value to False because we won't find this Axis Value in the STAT table.
-                    converter.options.update_name_table = False
-                    selected_instance = NamedInstance()
-                    selected_instance.coordinates = selected_coordinates
-                else:
-                    # In case there are several instances with the same coordinates, return only the first one.
-                    #
-                    # From https://learn.microsoft.com/en-us/typography/opentype/spec/fvar#instancerecord:
-                    #
-                    # All the instance records in a font should have distinct coordinates and distinct
-                    # subfamilyNameID and postScriptName ID values. If two or more records share the same coordinates,
-                    # the same nameID values or the same postScriptNameID values, then all but the first can be ignored.
-                    selected_instance = [i for i in instances if i.coordinates == selected_coordinates][0]
-
-                instances = [selected_instance]
-
-            converter.run(variable_font=variable_font, instances=instances)
-
-        except Exception as e:
-            generic_error_message(e)
-
-    print()
-    generic_info_message(f"Total files  : {len(variable_fonts)}")
-    generic_info_message(f"Elapsed time : {round(time.time() - start_time, 3)} seconds")
-
-
-@font_converter.command()
-@add_file_or_path_argument()
-@click.option(
-    "-f",
-    "--flavor",
-    type=click.Choice(choices=["woff", "woff2"]),
-    help="""
-    By default, the script converts both woff and woff2 flavored web fonts to SFNT fonts (TrueType or OpenType). Use
-    this option to convert only woff or woff2 flavored web fonts.
-    """,
-)
-@add_common_options()
-def wf2ft(
-    input_path: Path,
-    flavor: str = None,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Converts web fonts (WOFF and WOFF2) to SFNT fonts (TTF or OTF)
-    """
-
-    if not flavor:
-        allowed_extensions = [".woff", ".woff2"]
-    else:
-        allowed_extensions = [f".{flavor}"]
-
-    fonts = get_fonts_in_path(
-        input_path=input_path, allow_extensions=allowed_extensions, recalc_timestamp=recalc_timestamp
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    from foundryToolsCLI.Lib.converters.web_to_sfnt import WF2FTRunner
-
-    converter = WF2FTRunner()
-
-    input_flavors = ["woff", "woff2"]
-    if flavor is not None:
-        input_flavors = [flavor]
-
-    converter.options.woff = True if "woff" in input_flavors else False
-    converter.options.woff2 = True if "woff2" in input_flavors else False
-    converter.options.recalc_timestamp = recalc_timestamp
-    converter.options.output_dir = output_dir
-    converter.options.overwrite = overwrite
-    converter.run(fonts=fonts)
-
-
-@font_converter.command()
-@add_file_or_path_argument()
-@click.option(
-    "-f",
-    "--flavor",
-    type=click.Choice(choices=["woff", "woff2"]),
-    help="""
-    By default, the script converts SFNT fonts (TrueType or OpenType) both to woff and woff2 flavored web fonts. Use
-    this option to create only woff (--flavor woff) or woff2 (--flavor woff2) files.
-    """,
-)
-@add_common_options()
-def ft2wf(input_path, flavor=None, output_dir=None, recalc_timestamp=False, overwrite=True):
-    """
-    Converts SFNT fonts (TTF or OTF) to web fonts (WOFF and/or WOFF2)
-    """
-
-    fonts = get_fonts_in_path(
-        input_path=input_path, allow_extensions=[".otf", ".ttf"], recalc_timestamp=recalc_timestamp
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    from foundryToolsCLI.Lib.converters.sfnt_to_web import FT2WFRunner
-
-    converter = FT2WFRunner()
-
-    output_flavors = ["woff", "woff2"]
-    if flavor is not None:
-        output_flavors = [flavor]
-
-    converter.options.woff = True if "woff" in output_flavors else False
-    converter.options.woff2 = True if "woff2" in output_flavors else False
-    converter.options.recalc_timestamp = recalc_timestamp
-    converter.options.output_dir = output_dir
-    converter.options.overwrite = overwrite
-    converter.run(fonts=fonts)
-
-
-@font_converter.command()
-@add_file_or_path_argument()
-@add_common_options()
-def ttc2sfnt(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
-    """
-    Extracts each font from a TTC file, and saves it as a TTF or OTF file.
-    """
-    from fontTools.ttLib import TTCollection, TTLibError
-
-    if input_path.is_file():
-        files = [input_path]
-    elif input_path.is_dir():
-        files = input_path.iterdir()
-    else:
-        generic_error_message(f"Invalid path: {input_path}")
-        return
-
-    tt_collections: list[TTCollection] = []
-    for file in files:
-        try:
-            ttc_font = TTCollection(file)
-            tt_collections.append(ttc_font)
-        except (TTLibError, Exception):
-            pass
-
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=tt_collections, output_dir=output_dir):
-        return
-
-    from foundryToolsCLI.Lib.converters.ttc_to_sfnt import TTC2SFNTRunner
-
-    converter = TTC2SFNTRunner()
-    converter.options.recalc_timestamp = recalc_timestamp
-    converter.options.output_dir = output_dir
-    converter.options.overwrite = overwrite
-    converter.run(tt_collections=tt_collections)
-
-
-cli = click.CommandCollection(
-    sources=[font_converter],
-    help="""
-    Font converter.
-    """,
-)
+import time
+from pathlib import Path
+
+import click
+
+from foundryToolsCLI.Lib.utils.cli_tools import (
+    get_fonts_in_path,
+    get_output_dir,
+    initial_check_pass,
+    get_variable_fonts_in_path,
+)
+from foundryToolsCLI.Lib.utils.click_tools import (
+    add_file_or_path_argument,
+    add_common_options,
+    generic_info_message,
+    select_instance_coordinates,
+    generic_error_message,
+)
+
+font_converter = click.Group("subcommands")
+
+
+@font_converter.command()
+@add_file_or_path_argument()
+@click.option(
+    "-t",
+    "--tolerance",
+    type=click.FloatRange(0.0, 3.0),
+    default=1.0,
+    help="""
+    Conversion tolerance (0.0-3.0, default 1.0). Low tolerance adds more points but keeps shapes. High tolerance adds 
+    few points but may change shape.
+    """,
+)
+@click.option(
+    "--scale-upm", type=click.IntRange(1000, 4096, max_open=True), help="Scale the units-per-em of converted fonts."
+)
+@click.option("--no-subr", "subroutinize", is_flag=True, default=True, help="Do not subroutinize converted fonts.")
+@add_common_options()
+def ttf2otf(
+    input_path: Path,
+    tolerance: float = 1.0,
+    scale_upm: int = None,
+    subroutinize: bool = True,
+    recalc_timestamp: bool = False,
+    output_dir: Path = None,
+    overwrite: bool = True,
+):
+    """
+    Converts TTF fonts to OTF (or TrueType flavored woff/woff2 web fonts to PostScript flavored woff/woff2 web fonts).
+    """
+    fonts = get_fonts_in_path(
+        input_path=input_path, allow_cff=False, allow_variable=False, recalc_timestamp=recalc_timestamp
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    from foundryToolsCLI.Lib.converters.ttf_to_otf import TTF2OTFRunner
+
+    runner = TTF2OTFRunner()
+    runner.options.tolerance = tolerance
+    runner.options.scale_upm = scale_upm
+    runner.options.subroutinize = subroutinize
+    runner.options.recalc_timestamp = recalc_timestamp
+    runner.options.output_dir = output_dir
+    runner.options.overwrite = overwrite
+    runner.run(source_fonts=fonts)
+
+
+@font_converter.command()
+@add_file_or_path_argument()
+@click.option(
+    "--max-err",
+    type=click.FloatRange(0.1, 3.0),
+    default=1.0,
+    help="Approximation error, measured in UPEM",
+)
+@add_common_options()
+def otf2ttf(
+    input_path: Path,
+    max_err: float = 1.0,
+    recalc_timestamp: bool = False,
+    output_dir: Path = None,
+    overwrite: bool = True,
+):
+    """
+    Converts OTF fonts to TTF (or PostScripts flavored woff/woff2 web fonts to TrueType flavored woff/woff2 web fonts).
+    """
+    fonts = get_fonts_in_path(
+        input_path=input_path, allow_ttf=False, allow_variable=False, recalc_timestamp=recalc_timestamp
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    from foundryToolsCLI.Lib.converters.otf_to_ttf import OTF2TTFRunner
+
+    runner = OTF2TTFRunner()
+    runner.options.max_err = max_err
+    runner.options.output_dir = output_dir
+    runner.options.overwrite = overwrite
+    runner.run(source_fonts=fonts)
+
+
+@font_converter.command()
+@add_file_or_path_argument()
+@click.option(
+    "-s",
+    "--select-instance",
+    is_flag=True,
+    default=False,
+    help="""
+    By default, the script exports all named instances. Use this option to select custom axis values for a single
+    instance.
+    """,
+)
+@click.option(
+    "--no-cleanup",
+    "cleanup",
+    is_flag=True,
+    default=True,
+    help="""
+    By default, STAT table is dropped and axis nameIDs are deleted from name table. Use --no-cleanup to keep STAT table
+    and prevent axis nameIDs to be deleted from name table.
+    """,
+)
+@click.option(
+    "--no-update-name-table",
+    "update_name_table",
+    is_flag=True,
+    default=True,
+    help="""
+    Prevent updating instantiated fonts `name` table. Input fonts must have a STAT table with Axis Value Tables.
+    """,
+)
+@add_common_options()
+def vf2i(
+    input_path: Path,
+    select_instance: bool = False,
+    cleanup: bool = True,
+    update_name_table: bool = True,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Exports static instances from variable fonts.
+    """
+    variable_fonts = get_variable_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=variable_fonts, output_dir=output_dir):
+        return
+
+    from foundryToolsCLI.Lib.converters.variable_to_static import VariableToStatic
+    from fontTools.ttLib.tables._f_v_a_r import NamedInstance
+
+    start_time = time.time()
+    for variable_font in variable_fonts:
+        print()
+        file = Path(variable_font.reader.file.name)
+        generic_info_message(f"Converting file {file.name}")
+        try:
+            converter = VariableToStatic()
+            converter.options.cleanup = cleanup
+            converter.options.update_name_table = update_name_table
+            converter.options.output_dir = output_dir
+            converter.options.overwrite = overwrite
+
+            instances = variable_font.get_instances()
+            if select_instance:
+                axes = variable_font.get_axes()
+                selected_coordinates = select_instance_coordinates(axes)
+                is_named_instance = selected_coordinates in [i.coordinates for i in instances]
+                if not is_named_instance:
+                    # Set update_name_table value to False because we won't find this Axis Value in the STAT table.
+                    converter.options.update_name_table = False
+                    selected_instance = NamedInstance()
+                    selected_instance.coordinates = selected_coordinates
+                else:
+                    # In case there are several instances with the same coordinates, return only the first one.
+                    #
+                    # From https://learn.microsoft.com/en-us/typography/opentype/spec/fvar#instancerecord:
+                    #
+                    # All the instance records in a font should have distinct coordinates and distinct
+                    # subfamilyNameID and postScriptName ID values. If two or more records share the same coordinates,
+                    # the same nameID values or the same postScriptNameID values, then all but the first can be ignored.
+                    selected_instance = [i for i in instances if i.coordinates == selected_coordinates][0]
+
+                instances = [selected_instance]
+
+            converter.run(variable_font=variable_font, instances=instances)
+
+        except Exception as e:
+            generic_error_message(e)
+
+    print()
+    generic_info_message(f"Total files  : {len(variable_fonts)}")
+    generic_info_message(f"Elapsed time : {round(time.time() - start_time, 3)} seconds")
+
+
+@font_converter.command()
+@add_file_or_path_argument()
+@click.option(
+    "-f",
+    "--flavor",
+    type=click.Choice(choices=["woff", "woff2"]),
+    help="""
+    By default, the script converts both woff and woff2 flavored web fonts to SFNT fonts (TrueType or OpenType). Use
+    this option to convert only woff or woff2 flavored web fonts.
+    """,
+)
+@add_common_options()
+def wf2ft(
+    input_path: Path,
+    flavor: str = None,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Converts web fonts (WOFF and WOFF2) to SFNT fonts (TTF or OTF)
+    """
+
+    if not flavor:
+        allowed_extensions = [".woff", ".woff2"]
+    else:
+        allowed_extensions = [f".{flavor}"]
+
+    fonts = get_fonts_in_path(
+        input_path=input_path, allow_extensions=allowed_extensions, recalc_timestamp=recalc_timestamp
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    from foundryToolsCLI.Lib.converters.web_to_sfnt import WF2FTRunner
+
+    converter = WF2FTRunner()
+
+    input_flavors = ["woff", "woff2"]
+    if flavor is not None:
+        input_flavors = [flavor]
+
+    converter.options.woff = True if "woff" in input_flavors else False
+    converter.options.woff2 = True if "woff2" in input_flavors else False
+    converter.options.recalc_timestamp = recalc_timestamp
+    converter.options.output_dir = output_dir
+    converter.options.overwrite = overwrite
+    converter.run(fonts=fonts)
+
+
+@font_converter.command()
+@add_file_or_path_argument()
+@click.option(
+    "-f",
+    "--flavor",
+    type=click.Choice(choices=["woff", "woff2"]),
+    help="""
+    By default, the script converts SFNT fonts (TrueType or OpenType) both to woff and woff2 flavored web fonts. Use
+    this option to create only woff (--flavor woff) or woff2 (--flavor woff2) files.
+    """,
+)
+@add_common_options()
+def ft2wf(input_path, flavor=None, output_dir=None, recalc_timestamp=False, overwrite=True):
+    """
+    Converts SFNT fonts (TTF or OTF) to web fonts (WOFF and/or WOFF2)
+    """
+
+    fonts = get_fonts_in_path(
+        input_path=input_path, allow_extensions=[".otf", ".ttf"], recalc_timestamp=recalc_timestamp
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    from foundryToolsCLI.Lib.converters.sfnt_to_web import FT2WFRunner
+
+    converter = FT2WFRunner()
+
+    output_flavors = ["woff", "woff2"]
+    if flavor is not None:
+        output_flavors = [flavor]
+
+    converter.options.woff = True if "woff" in output_flavors else False
+    converter.options.woff2 = True if "woff2" in output_flavors else False
+    converter.options.recalc_timestamp = recalc_timestamp
+    converter.options.output_dir = output_dir
+    converter.options.overwrite = overwrite
+    converter.run(fonts=fonts)
+
+
+@font_converter.command()
+@add_file_or_path_argument()
+@add_common_options()
+def ttc2sfnt(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
+    """
+    Extracts each font from a TTC file, and saves it as a TTF or OTF file.
+    """
+    from fontTools.ttLib import TTCollection, TTLibError
+
+    if input_path.is_file():
+        files = [input_path]
+    elif input_path.is_dir():
+        files = input_path.iterdir()
+    else:
+        generic_error_message(f"Invalid path: {input_path}")
+        return
+
+    tt_collections: list[TTCollection] = []
+    for file in files:
+        try:
+            ttc_font = TTCollection(file)
+            tt_collections.append(ttc_font)
+        except (TTLibError, Exception):
+            pass
+
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=tt_collections, output_dir=output_dir):
+        return
+
+    from foundryToolsCLI.Lib.converters.ttc_to_sfnt import TTC2SFNTRunner
+
+    converter = TTC2SFNTRunner()
+    converter.options.recalc_timestamp = recalc_timestamp
+    converter.options.output_dir = output_dir
+    converter.options.overwrite = overwrite
+    converter.run(tt_collections=tt_collections)
+
+
+cli = click.CommandCollection(
+    sources=[font_converter],
+    help="""
+    Font converter.
+    """,
+)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_fix.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_fix.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,559 +1,558 @@
-import os
-from copy import deepcopy
-from pathlib import Path
-
-import click
-from fontTools.misc.cliTools import makeOutputFileName
-
-from foundryToolsCLI.Lib.tables.OS_2 import TableOS2
-from foundryToolsCLI.Lib.tables.hhea import TableHhea
-from foundryToolsCLI.Lib.tables.name import TableName
-from foundryToolsCLI.Lib.tables.post import TablePost
-from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
-from foundryToolsCLI.Lib.utils.click_tools import (
-    add_file_or_path_argument,
-    add_common_options,
-    generic_error_message,
-    file_saved_message,
-    file_not_changed_message,
-    generic_warning_message,
-    generic_success_message,
-    generic_info_message,
-)
-
-CWD = Path.cwd()
-fix_fonts = click.Group("subcommands")
-
-
-@fix_fonts.command()
-@add_file_or_path_argument()
-@add_common_options()
-def monospace(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
-    """
-    If the family is monospaced:
-
-    \b
-    * post.isFixedPitch must be set to a non-zero value
-    * OS/2.panose.bProportion must be set to 9
-    * CFF.cff.TopDictIndex[0].isFixedPitch must be set to True
-
-    fontbakery check id: com.google.fonts/check/monospace
-    """
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-
-            post_table: TablePost = font["post"]
-            os2_table: TableOS2 = font["OS/2"]
-            post_table_copy = deepcopy(post_table)
-            os2_table_copy = deepcopy(os2_table)
-
-            post_table.set_fixed_pitch(True)
-
-            if os2_table.panose.bProportion != 9:
-                os2_table.panose.bProportion = 9
-                # Ensure that panose.bFamilyType is non-zero when panose.bProportion is 9
-                if os2_table.panose.bFamilyType == 0:
-                    os2_table.panose.bFamilyType = 2
-
-            post_table_changed = False
-            if post_table_copy.compile(font) != post_table.compile(font):
-                post_table_changed = True
-
-            os2_table_changed = False
-            if os2_table_copy.compile(font) != os2_table.compile(font):
-                os2_table_changed = True
-
-            cff_table_changed = False
-            if font.is_otf:
-                cff_table = font["CFF "]
-                cff_table_copy = deepcopy(cff_table)
-                top_dict = cff_table.cff.topDictIndex[0]
-                setattr(top_dict, "isFixedPitch", True)
-
-                if cff_table_copy.compile(font) != cff_table.compile(font):
-                    cff_table_changed = True
-
-            if post_table_changed or os2_table_changed or cff_table_changed:
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@fix_fonts.command()
-@add_file_or_path_argument()
-@add_common_options()
-def nbsp_width(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overWrite: bool = True):
-    """
-    Checks if 'nbspace' and 'space' glyphs have the same width. If not, corrects 'nbspace' width to match 'space' width.
-
-    fontbakery check id: com.google.fonts/check/whitespace_widths
-    """
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overWrite))
-
-            hmtx_table = font["hmtx"]
-            hmtx_table_copy = deepcopy(hmtx_table)
-
-            best_cmap = font.getBestCmap()
-            space_name = best_cmap[0x0020]
-            nbspace_name = best_cmap[0x00A0]
-
-            font["hmtx"][nbspace_name] = font["hmtx"][space_name]
-
-            if hmtx_table_copy.compile(font) != hmtx_table.compile(font):
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@fix_fonts.command()
-@add_file_or_path_argument()
-@click.option(
-    "-m",
-    "--mode",
-    type=click.IntRange(1, 3),
-    default=1,
-    help="""
-              \b
-              1: sets only the italic bits and clears the oblique bit
-              2: sets italic and oblique bits
-              3: sets only the oblique bit and clears italic bits
-              """,
-)
-@add_common_options()
-def italic_angle(
-    input_path: Path, mode: int = 1, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
-):
-    """
-    Recalculates post.italicAngle, hhea.caretSlopeRise, hhea.caretSlopeRun and sets/clears the italic/oblique bits
-    according to the calculated values. In CFF fonts, also CFF.topDictIndex[0].ItalicAngle is recalculated.
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        print()
-
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            generic_info_message(f"Checking file: {file.name}")
-
-            post_table: TablePost = font["post"]
-            hhea_table: TableHhea = font["hhea"]
-
-            # Check post.italicAngle
-            post_italic_angle = post_table.italicAngle
-            calculated_post_italic_angle = font.calculate_italic_angle()
-            post_italic_angle_ok = font.check_italic_angle()
-            if post_italic_angle_ok:
-                generic_success_message(
-                    f"post.italicAngle    : {click.style(post_italic_angle, fg='green', bold=True)}"
-                )
-            else:
-                post_table.set_italic_angle(calculated_post_italic_angle)
-                generic_warning_message(
-                    f"post.italicAngle    : "
-                    f"{click.style(post_italic_angle, fg='red', bold=True)} -> "
-                    f"{click.style(calculated_post_italic_angle, fg='green', bold=True)}"
-                )
-
-            calculated_rise = font.calculate_caret_slope_rise()
-            calculated_run = font.calculate_caret_slope_run()
-
-            # Check hhea italic angle
-            rise = hhea_table.caretSlopeRise
-            run = hhea_table.caretSlopeRun
-            hhea_italic_angle = font.calculate_run_rise_angle()
-            hhea_italic_angle_ok = abs(post_table.italicAngle - hhea_italic_angle) < 0.1
-            if hhea_italic_angle_ok:
-                generic_success_message(f"hhea.caretSlopeRise : {click.style(rise, fg='green', bold=True)}")
-                generic_success_message(f"hhea.caretSlopeRun  : {(click.style(run, fg='green', bold=True))}")
-            else:
-                hhea_table.caretSlopeRise = calculated_rise
-                generic_warning_message(
-                    f"hhea.caretSlopeRise : {click.style(rise, fg='red', bold=True)} -> "
-                    f"{click.style(calculated_rise, fg='green', bold=True)}"
-                )
-                hhea_table.caretSlopeRun = calculated_run
-                generic_warning_message(
-                    f"hhea.caretSlopeRun  : {click.style(run, fg='red', bold=True)} -> "
-                    f"{click.style(calculated_run, fg='green', bold=True)}"
-                )
-
-            # Check CFF italic angle
-            if font.is_otf:
-                cff_table = font["CFF "]
-                cff_italic_angle = cff_table.cff.topDictIndex[0].ItalicAngle
-                cff_italic_angle_ok = cff_italic_angle == round(post_table.italicAngle)
-
-                if cff_italic_angle_ok:
-                    generic_success_message(
-                        f"CFF.ItalicAngle     : " f"{click.style(cff_italic_angle, fg='green', bold=True)}"
-                    )
-                else:
-                    cff_table.cff.topDictIndex[0].ItalicAngle = round(post_table.italicAngle)
-                    generic_warning_message(
-                        f"CFF.ItalicAngle     : "
-                        f"{click.style(cff_italic_angle, fg='red', bold=True)} -> "
-                        f"{click.style(cff_table.cff.topDictIndex[0].ItalicAngle, fg='green', bold=True)}"
-                    )
-            else:
-                cff_italic_angle_ok = True
-
-            # Set or clear italic/oblique bits according to post.italicAngle
-            is_italic = font.is_italic
-            is_oblique = font.is_oblique
-            font.calculate_italic_bits(mode=mode)
-
-            if font.is_italic == is_italic:
-                italic_bits_ok = True
-            else:
-                italic_bits_ok = False
-
-            if font.is_oblique == is_oblique:
-                oblique_bit_ok = True
-            else:
-                oblique_bit_ok = False
-
-            if italic_bits_ok:
-                generic_success_message(f"Italic              : " f"{click.style(is_italic, fg='green', bold=True)}")
-            else:
-                generic_info_message(
-                    f"Italic              : "
-                    f"{click.style(is_italic, fg='red', bold=True)} -> "
-                    f"{click.style(font.is_italic, fg='green', bold=True)}"
-                )
-
-            if oblique_bit_ok:
-                generic_success_message(f"Oblique             : " f"{click.style(is_oblique, fg='green', bold=True)}")
-            else:
-                generic_info_message(
-                    f"Oblique             : "
-                    f"{click.style(is_oblique, fg='red', bold=True)} -> "
-                    f"{click.style(font.is_oblique, fg='green', bold=True)}"
-                )
-
-            # Don't save the file if nothing has been modified
-            if (
-                post_italic_angle_ok
-                and hhea_italic_angle_ok
-                and cff_italic_angle_ok
-                and italic_bits_ok
-                and oblique_bit_ok
-            ):
-                file_not_changed_message(file.relative_to(CWD))
-                continue
-
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@fix_fonts.command()
-@add_file_or_path_argument()
-@add_common_options()
-def nbsp_missing(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
-    """
-    Checks if the font has a non-breaking space character, and if it doesn't, it adds one by double mapping 'space'
-    """
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-
-            cmap_table = font["cmap"]
-            cmap_table_copy = deepcopy(cmap_table)
-
-            for t in cmap_table.tables:
-                if t.isUnicode():
-                    if 0xA0 not in t.cmap.keys():
-                        t.cmap[0xA0] = "space"
-
-            if cmap_table_copy.compile(font) != cmap_table.compile(font):
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@fix_fonts.command()
-@add_file_or_path_argument()
-@add_common_options()
-def decompose_transformed(
-    input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
-):
-    """
-    Decomposes composite glyphs that have transformed components.
-
-    fontbakery check id: com.google.fonts/check/transformed_components
-    """
-
-    from fontTools.pens.recordingPen import DecomposingRecordingPen
-    from fontTools.pens.ttGlyphPen import TTGlyphPen
-    import pathops
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-
-            glyph_set = font.getGlyphSet()
-            glyph_table = font["glyf"]
-            glyph_table_copy = deepcopy(glyph_table)
-
-            for glyph_name in glyph_set.keys():
-                decompose = False
-                glyf = glyph_table[glyph_name]
-                if not glyf.isComposite():
-                    continue
-                for component in glyf.components:
-                    _, transform = component.getComponentInfo()
-
-                    # Font is hinted, decompose glyphs with *any* transformations
-                    if font.is_hinted_ttf:
-                        if transform[0:4] != (1, 0, 0, 1):
-                            decompose = True
-                    # Font is unhinted, decompose only glyphs with transformations where only one dimension is flipped
-                    # while the other isn't. Otherwise the outline direction is intact and since the font is unhinted,
-                    # no rendering problems are to be expected
-                    else:
-                        if transform[0] * transform[3] < 0:
-                            decompose = True
-
-                if decompose:
-                    dc_pen = DecomposingRecordingPen(glyph_set)
-                    glyph_set[glyph_name].draw(dc_pen)
-
-                    path = pathops.Path()
-                    path_pen = path.getPen()
-                    dc_pen.replay(path_pen)
-
-                    path.simplify()
-
-                    ttPen = TTGlyphPen(None)
-                    path.draw(ttPen)
-                    glyph_table[glyph_name] = ttPen.glyph()
-
-            if glyph_table_copy.compile(font) != glyph_table.compile(font):
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@fix_fonts.command()
-@add_file_or_path_argument()
-@add_common_options()
-def duplicate_components(
-    input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
-):
-    """
-    Removes duplicate components which have the same x,y coordinates.
-
-    fontbakery check id: com.google.fonts/check/glyf_non_transformed_duplicate_components
-    """
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-
-            glyph_table = font["glyf"]
-            glyph_table_copy = deepcopy(glyph_table)
-
-            for glyph_name in glyph_table.keys():
-                glyf = glyph_table[glyph_name]
-                if not glyf.isComposite():
-                    continue
-
-                seen = []
-
-                for comp in glyf.components:
-                    comp_info = {
-                        "glyph": glyph_name,
-                        "component": comp.glyphName,
-                        "x": comp.x,
-                        "y": comp.y,
-                    }
-                    if comp_info in seen:
-                        glyf.components.remove(comp)
-                    else:
-                        seen.append(comp_info)
-
-            if glyph_table_copy.compile(font) != glyph_table.compile(font):
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@fix_fonts.command()
-@add_file_or_path_argument()
-@add_common_options()
-def kern_table(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
-    """
-    Some applications such as MS PowerPoint require kerning info on the kern table. More specifically, they require a
-    format 0 kern subtable from a kern table version 0 with only glyphs defined in the cmap table.
-
-    Given this, the command deletes all kerning pairs from kern v0 subtables where one of the two glyphs is not defined
-    in the cmap table.
-
-    fontbakery check id: com.google.fonts/check/kern_table
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-
-            if "kern" not in font:
-                continue
-
-            kern = font["kern"]
-
-            if all(kernTable.format != 0 for kernTable in kern.kernTables):
-                generic_warning_message(f"{os.path.basename(file)} The 'kern' table doesn't have any format-0 subtable")
-                continue
-
-            kern_table_copy = deepcopy(kern)
-
-            character_glyphs = set()
-            for table in font["cmap"].tables:
-                character_glyphs.update(table.cmap.values())
-
-            for table in kern.kernTables:
-                if table.format == 0:
-                    pairs_to_delete = []
-                    for left_glyph, right_glyph in table.kernTable.keys():
-                        if left_glyph not in character_glyphs or right_glyph not in character_glyphs:
-                            pairs_to_delete.append((left_glyph, right_glyph))
-                    if len(pairs_to_delete) > 0:
-                        for pair in pairs_to_delete:
-                            del table.kernTable[pair]
-
-            if kern_table_copy.compile(font) != kern.compile(font):
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@fix_fonts.command()
-@add_file_or_path_argument()
-@add_common_options()
-def strip_names(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
-    """
-    Removes leading and trailing spaces from all namerecords.
-
-    fontbakery check id: com.google.fonts/check/name/trailing_spaces
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-
-            name_table: TableName = font["name"]
-            name_table_copy = deepcopy(name_table)
-
-            name_table.remove_leading_trailing_spaces()
-
-            if name_table_copy.compile(font) != name_table.compile(font):
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-cli = click.CommandCollection(
-    sources=[fix_fonts],
-    help="""
-    A set of commands to detect and automatically fix font errors.
-    """,
-)
+import os
+from copy import deepcopy
+from pathlib import Path
+
+import click
+from fontTools.misc.cliTools import makeOutputFileName
+
+from foundryToolsCLI.Lib.tables.OS_2 import TableOS2
+from foundryToolsCLI.Lib.tables.hhea import TableHhea
+from foundryToolsCLI.Lib.tables.name import TableName
+from foundryToolsCLI.Lib.tables.post import TablePost
+from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
+from foundryToolsCLI.Lib.utils.click_tools import (
+    add_file_or_path_argument,
+    add_common_options,
+    generic_error_message,
+    file_saved_message,
+    file_not_changed_message,
+    generic_warning_message,
+    generic_success_message,
+    generic_info_message,
+)
+
+fix_fonts = click.Group("subcommands")
+
+
+@fix_fonts.command()
+@add_file_or_path_argument()
+@add_common_options()
+def monospace(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
+    """
+    If the family is monospaced:
+
+    \b
+    * post.isFixedPitch must be set to a non-zero value
+    * OS/2.panose.bProportion must be set to 9
+    * CFF.cff.TopDictIndex[0].isFixedPitch must be set to True
+
+    fontbakery check id: com.google.fonts/check/monospace
+    """
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            post_table: TablePost = font["post"]
+            os2_table: TableOS2 = font["OS/2"]
+            post_table_copy = deepcopy(post_table)
+            os2_table_copy = deepcopy(os2_table)
+
+            post_table.set_fixed_pitch(True)
+
+            if os2_table.panose.bProportion != 9:
+                os2_table.panose.bProportion = 9
+                # Ensure that panose.bFamilyType is non-zero when panose.bProportion is 9
+                if os2_table.panose.bFamilyType == 0:
+                    os2_table.panose.bFamilyType = 2
+
+            post_table_changed = False
+            if post_table_copy.compile(font) != post_table.compile(font):
+                post_table_changed = True
+
+            os2_table_changed = False
+            if os2_table_copy.compile(font) != os2_table.compile(font):
+                os2_table_changed = True
+
+            cff_table_changed = False
+            if font.is_otf:
+                cff_table = font["CFF "]
+                cff_table_copy = deepcopy(cff_table)
+                top_dict = cff_table.cff.topDictIndex[0]
+                setattr(top_dict, "isFixedPitch", True)
+
+                if cff_table_copy.compile(font) != cff_table.compile(font):
+                    cff_table_changed = True
+
+            if post_table_changed or os2_table_changed or cff_table_changed:
+                font.save(output_file)
+                file_saved_message(output_file)
+
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@fix_fonts.command()
+@add_file_or_path_argument()
+@add_common_options()
+def nbsp_width(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
+    """
+    Checks if 'nbspace' and 'space' glyphs have the same width. If not, corrects 'nbspace' width to match 'space' width.
+
+    fontbakery check id: com.google.fonts/check/whitespace_widths
+    """
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            hmtx_table = font["hmtx"]
+            hmtx_table_copy = deepcopy(hmtx_table)
+
+            best_cmap = font.getBestCmap()
+            space_name = best_cmap[0x0020]
+            nbspace_name = best_cmap[0x00A0]
+
+            font["hmtx"][nbspace_name] = font["hmtx"][space_name]
+
+            if hmtx_table_copy.compile(font) != hmtx_table.compile(font):
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@fix_fonts.command()
+@add_file_or_path_argument()
+@click.option(
+    "-m",
+    "--mode",
+    type=click.IntRange(1, 3),
+    default=1,
+    help="""
+              \b
+              1: sets only the italic bits and clears the oblique bit
+              2: sets italic and oblique bits
+              3: sets only the oblique bit and clears italic bits
+              """,
+)
+@add_common_options()
+def italic_angle(
+    input_path: Path, mode: int = 1, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
+):
+    """
+    Recalculates post.italicAngle, hhea.caretSlopeRise, hhea.caretSlopeRun and sets/clears the italic/oblique bits
+    according to the calculated values. In CFF fonts, also CFF.topDictIndex[0].ItalicAngle is recalculated.
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        print()
+
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            generic_info_message(f"Checking file: {file.name}")
+
+            post_table: TablePost = font["post"]
+            hhea_table: TableHhea = font["hhea"]
+
+            # Check post.italicAngle
+            post_italic_angle = post_table.italicAngle
+            calculated_post_italic_angle = font.calculate_italic_angle()
+            post_italic_angle_ok = font.check_italic_angle()
+            if post_italic_angle_ok:
+                generic_success_message(
+                    f"post.italicAngle    : {click.style(post_italic_angle, fg='green', bold=True)}"
+                )
+            else:
+                post_table.set_italic_angle(calculated_post_italic_angle)
+                generic_warning_message(
+                    f"post.italicAngle    : "
+                    f"{click.style(post_italic_angle, fg='red', bold=True)} -> "
+                    f"{click.style(calculated_post_italic_angle, fg='green', bold=True)}"
+                )
+
+            calculated_rise = font.calculate_caret_slope_rise()
+            calculated_run = font.calculate_caret_slope_run()
+
+            # Check hhea italic angle
+            rise = hhea_table.caretSlopeRise
+            run = hhea_table.caretSlopeRun
+            hhea_italic_angle = font.calculate_run_rise_angle()
+            hhea_italic_angle_ok = abs(post_table.italicAngle - hhea_italic_angle) < 0.1
+            if hhea_italic_angle_ok:
+                generic_success_message(f"hhea.caretSlopeRise : {click.style(rise, fg='green', bold=True)}")
+                generic_success_message(f"hhea.caretSlopeRun  : {(click.style(run, fg='green', bold=True))}")
+            else:
+                hhea_table.caretSlopeRise = calculated_rise
+                generic_warning_message(
+                    f"hhea.caretSlopeRise : {click.style(rise, fg='red', bold=True)} -> "
+                    f"{click.style(calculated_rise, fg='green', bold=True)}"
+                )
+                hhea_table.caretSlopeRun = calculated_run
+                generic_warning_message(
+                    f"hhea.caretSlopeRun  : {click.style(run, fg='red', bold=True)} -> "
+                    f"{click.style(calculated_run, fg='green', bold=True)}"
+                )
+
+            # Check CFF italic angle
+            if font.is_otf:
+                cff_table = font["CFF "]
+                cff_italic_angle = cff_table.cff.topDictIndex[0].ItalicAngle
+                cff_italic_angle_ok = cff_italic_angle == round(post_table.italicAngle)
+
+                if cff_italic_angle_ok:
+                    generic_success_message(
+                        f"CFF.ItalicAngle     : " f"{click.style(cff_italic_angle, fg='green', bold=True)}"
+                    )
+                else:
+                    cff_table.cff.topDictIndex[0].ItalicAngle = round(post_table.italicAngle)
+                    generic_warning_message(
+                        f"CFF.ItalicAngle     : "
+                        f"{click.style(cff_italic_angle, fg='red', bold=True)} -> "
+                        f"{click.style(cff_table.cff.topDictIndex[0].ItalicAngle, fg='green', bold=True)}"
+                    )
+            else:
+                cff_italic_angle_ok = True
+
+            # Set or clear italic/oblique bits according to post.italicAngle
+            is_italic = font.is_italic
+            is_oblique = font.is_oblique
+            font.calculate_italic_bits(mode=mode)
+
+            if font.is_italic == is_italic:
+                italic_bits_ok = True
+            else:
+                italic_bits_ok = False
+
+            if font.is_oblique == is_oblique:
+                oblique_bit_ok = True
+            else:
+                oblique_bit_ok = False
+
+            if italic_bits_ok:
+                generic_success_message(f"Italic              : " f"{click.style(is_italic, fg='green', bold=True)}")
+            else:
+                generic_info_message(
+                    f"Italic              : "
+                    f"{click.style(is_italic, fg='red', bold=True)} -> "
+                    f"{click.style(font.is_italic, fg='green', bold=True)}"
+                )
+
+            if oblique_bit_ok:
+                generic_success_message(f"Oblique             : " f"{click.style(is_oblique, fg='green', bold=True)}")
+            else:
+                generic_info_message(
+                    f"Oblique             : "
+                    f"{click.style(is_oblique, fg='red', bold=True)} -> "
+                    f"{click.style(font.is_oblique, fg='green', bold=True)}"
+                )
+
+            # Don't save the file if nothing has been modified
+            if (
+                post_italic_angle_ok
+                and hhea_italic_angle_ok
+                and cff_italic_angle_ok
+                and italic_bits_ok
+                and oblique_bit_ok
+            ):
+                file_not_changed_message(file)
+                continue
+
+            font.save(output_file)
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@fix_fonts.command()
+@add_file_or_path_argument()
+@add_common_options()
+def nbsp_missing(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
+    """
+    Checks if the font has a non-breaking space character, and if it doesn't, it adds one by double mapping 'space'
+    """
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            cmap_table = font["cmap"]
+            cmap_table_copy = deepcopy(cmap_table)
+
+            for t in cmap_table.tables:
+                if t.isUnicode():
+                    if 0xA0 not in t.cmap.keys():
+                        t.cmap[0xA0] = "space"
+
+            if cmap_table_copy.compile(font) != cmap_table.compile(font):
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@fix_fonts.command()
+@add_file_or_path_argument()
+@add_common_options()
+def decompose_transformed(
+    input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
+):
+    """
+    Decomposes composite glyphs that have transformed components.
+
+    fontbakery check id: com.google.fonts/check/transformed_components
+    """
+
+    from fontTools.pens.recordingPen import DecomposingRecordingPen
+    from fontTools.pens.ttGlyphPen import TTGlyphPen
+    import pathops
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            glyph_set = font.getGlyphSet()
+            glyph_table = font["glyf"]
+            glyph_table_copy = deepcopy(glyph_table)
+
+            for glyph_name in glyph_set.keys():
+                decompose = False
+                glyf = glyph_table[glyph_name]
+                if not glyf.isComposite():
+                    continue
+                for component in glyf.components:
+                    _, transform = component.getComponentInfo()
+
+                    # Font is hinted, decompose glyphs with *any* transformations
+                    if font.is_hinted_ttf:
+                        if transform[0:4] != (1, 0, 0, 1):
+                            decompose = True
+                    # Font is unhinted, decompose only glyphs with transformations where only one dimension is flipped
+                    # while the other isn't. Otherwise the outline direction is intact and since the font is unhinted,
+                    # no rendering problems are to be expected
+                    else:
+                        if transform[0] * transform[3] < 0:
+                            decompose = True
+
+                if decompose:
+                    dc_pen = DecomposingRecordingPen(glyph_set)
+                    glyph_set[glyph_name].draw(dc_pen)
+
+                    path = pathops.Path()
+                    path_pen = path.getPen()
+                    dc_pen.replay(path_pen)
+
+                    path.simplify()
+
+                    ttPen = TTGlyphPen(None)
+                    path.draw(ttPen)
+                    glyph_table[glyph_name] = ttPen.glyph()
+
+            if glyph_table_copy.compile(font) != glyph_table.compile(font):
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@fix_fonts.command()
+@add_file_or_path_argument()
+@add_common_options()
+def duplicate_components(
+    input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
+):
+    """
+    Removes duplicate components which have the same x,y coordinates.
+
+    fontbakery check id: com.google.fonts/check/glyf_non_transformed_duplicate_components
+    """
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            glyph_table = font["glyf"]
+            glyph_table_copy = deepcopy(glyph_table)
+
+            for glyph_name in glyph_table.keys():
+                glyf = glyph_table[glyph_name]
+                if not glyf.isComposite():
+                    continue
+
+                seen = []
+
+                for comp in glyf.components:
+                    comp_info = {
+                        "glyph": glyph_name,
+                        "component": comp.glyphName,
+                        "x": comp.x,
+                        "y": comp.y,
+                    }
+                    if comp_info in seen:
+                        glyf.components.remove(comp)
+                    else:
+                        seen.append(comp_info)
+
+            if glyph_table_copy.compile(font) != glyph_table.compile(font):
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@fix_fonts.command()
+@add_file_or_path_argument()
+@add_common_options()
+def kern_table(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
+    """
+    Some applications such as MS PowerPoint require kerning info on the kern table. More specifically, they require a
+    format 0 kern subtable from a kern table version 0 with only glyphs defined in the cmap table.
+
+    Given this, the command deletes all kerning pairs from kern v0 subtables where one of the two glyphs is not defined
+    in the cmap table.
+
+    fontbakery check id: com.google.fonts/check/kern_table
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            if "kern" not in font:
+                continue
+
+            kern = font["kern"]
+
+            if all(kernTable.format != 0 for kernTable in kern.kernTables):
+                generic_warning_message(f"{os.path.basename(file)} The 'kern' table doesn't have any format-0 subtable")
+                continue
+
+            kern_table_copy = deepcopy(kern)
+
+            character_glyphs = set()
+            for table in font["cmap"].tables:
+                character_glyphs.update(table.cmap.values())
+
+            for table in kern.kernTables:
+                if table.format == 0:
+                    pairs_to_delete = []
+                    for left_glyph, right_glyph in table.kernTable.keys():
+                        if left_glyph not in character_glyphs or right_glyph not in character_glyphs:
+                            pairs_to_delete.append((left_glyph, right_glyph))
+                    if len(pairs_to_delete) > 0:
+                        for pair in pairs_to_delete:
+                            del table.kernTable[pair]
+
+            if kern_table_copy.compile(font) != kern.compile(font):
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@fix_fonts.command()
+@add_file_or_path_argument()
+@add_common_options()
+def strip_names(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
+    """
+    Removes leading and trailing spaces from all namerecords.
+
+    fontbakery check id: com.google.fonts/check/name/trailing_spaces
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            name_table: TableName = font["name"]
+            name_table_copy = deepcopy(name_table)
+
+            name_table.remove_leading_trailing_spaces()
+
+            if name_table_copy.compile(font) != name_table.compile(font):
+                font.save(output_file)
+                file_saved_message(output_file)
+
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+cli = click.CommandCollection(
+    sources=[fix_fonts],
+    help="""
+    A set of commands to detect and automatically fix font errors.
+    """,
+)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_metrics.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_metrics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,303 +1,302 @@
-from copy import copy
-from pathlib import Path
-
-import click
-from fontTools.misc.cliTools import makeOutputFileName
-
-from foundryToolsCLI.Lib.Font import Font
-from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
-from foundryToolsCLI.Lib.utils.click_tools import (
-    add_common_options,
-    file_saved_message,
-    generic_error_message,
-    add_file_or_path_argument,
-    file_not_changed_message,
-)
-
-CWD = Path.cwd()
-vertical_metrics_tools = click.Group("subcommands")
-
-
-@vertical_metrics_tools.command()
-@add_file_or_path_argument()
-@click.option(
-    "-p",
-    "--percent",
-    type=click.IntRange(0, 100),
-    required=True,
-    help="Adjust font line spacing to % of UPM value.",
-)
-@add_common_options()
-def set_linegap(
-    input_path: Path, percent: int, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
-):
-    """Modifies the line spacing metrics in one or more fonts.
-
-    This is a fork of font-line by Source Foundry: https://github.com/source-foundry/font-line
-    """
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-
-            hhea_table = font["hhea"]
-            os2_table = font["OS/2"]
-            hhea_table_copy = copy(font["hhea"])
-            os2_table_copy = copy(font["OS/2"])
-
-            font.modify_linegap_percent(percent=percent)
-
-            hhea_modified = hhea_table_copy != hhea_table
-            os2_modified = os2_table_copy != os2_table
-
-            if hhea_modified or os2_modified:
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@vertical_metrics_tools.command()
-@add_file_or_path_argument()
-@click.option(
-    "--with-linegap",
-    is_flag=True,
-    help="""
-            By default, SIL method (https://silnrsi.github.io/FDBP/en-US/Line_Metrics.html) is used. This means that,
-            in OS/2 table, sTypoAscender and sTypoDescender values are set, respectively, equal to maximum real ascender
-            and minimum real descender, and the sTypoLineGap is set to zero. Use '--with-linegap' to set sTypoAscender
-            value to the maximum ideal ascender (calculated from letters b, f, f, h, k, l and t) and the sTypoDescender
-            value to the minimum ideal descender (calculated from letters g, j, p, q and y). The sTypoLineGap will be
-            calculated as follows: (real ascender + abs(real descender)) - (ideal ascender + abs(ideal descender)).
-    """,
-)
-@add_common_options()
-def align(
-    input_path: Path,
-    with_linegap: bool = False,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Aligns all fonts stored in INPUT_PATH folder to the same baseline.
-
-    To achieve this, the script finds the maximum ascender and the minimum descender values of the fonts stored in the
-    INPUT_PATH folder and applies those values to all fonts.
-
-    This can produce undesired effects (an exaggerated line height) when one or more fonts contain swashes, for example.
-    In such cases, it's better to copy the vertical metrics from a template font to one or more destination fonts using
-    the 'ftcli metrics copy-metrics' command.
-
-    See https://kltf.de/download/FontMetrics-kltf.pdf for more information.
-    """
-
-    import math
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    ideal_ascenders = []
-    ideal_descenders = []
-    real_ascenders = []
-    real_descenders = []
-
-    for font in fonts:
-        try:
-            font_y_min, font_y_max = font.get_bounding_box()
-            real_ascenders.append(math.ceil(font_y_max))
-            real_descenders.append(math.floor(font_y_min))
-
-            if with_linegap:
-                for glyph_name in ["b", "d", "f", "h", "k", "l", "t"]:
-                    ideal_ascenders.append(math.ceil(font.get_glyph_bounds(glyph_name)["yMax"]))
-
-                for glyph_name in ["g", "j", "p", "q", "y"]:
-                    ideal_descenders.append(math.floor(font.get_glyph_bounds(glyph_name)["yMin"]))
-            else:
-                ideal_ascenders = real_ascenders
-                ideal_ascenders = real_descenders
-
-        except Exception as e:
-            generic_error_message(e)
-
-    max_real_ascender = max(real_ascenders)
-    min_real_descender = min(real_descenders)
-    max_ideal_ascender = max(ideal_ascenders) if ideal_descenders != [] else max_real_ascender
-    min_ideal_descender = min(ideal_descenders) if ideal_descenders != [] else min_real_descender
-    typo_line_gap = (max_real_ascender + abs(min_real_descender)) - (max_ideal_ascender + abs(min_ideal_descender))
-
-    for font in fonts:
-        hhea_table = font["hhea"]
-        os2_table = font["OS/2"]
-        hhea_table_copy = copy(hhea_table)
-        os2_table_copy = copy(os2_table)
-
-        try:
-            file = Path(font.reader.file.name)
-            hhea_table.ascender = max_real_ascender
-            hhea_table.descender = min_real_descender
-            hhea_table.lineGap = 0
-
-            os2_table.usWinAscent = max_real_ascender
-            os2_table.usWinDescent = abs(min_real_descender)
-            os2_table.sTypoAscender = max_real_ascender
-            os2_table.sTypoDescender = min_real_descender
-            os2_table.sTypoLineGap = 0
-
-            if with_linegap:
-                os2_table.sTypoAscender = max_ideal_ascender
-                os2_table.sTypoDescender = min_ideal_descender
-                os2_table.sTypoLineGap = typo_line_gap
-
-            hhea_modified = hhea_table_copy != hhea_table
-            os2_modified = os2_table_copy != os2_table
-
-            if hhea_modified or os2_modified:
-                output_file = Path(makeOutputFileName(font.reader.file.name, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@vertical_metrics_tools.command()
-@click.option(
-    "-s",
-    "--source-file",
-    type=click.Path(exists=True, dir_okay=False, resolve_path=True),
-    required=True,
-    help="Source file. Vertical metrics from this font will be applied to all destination fonts.",
-)
-@click.option(
-    "-d",
-    "--destination",
-    type=click.Path(exists=True, resolve_path=True),
-    required=True,
-    help="Destination file or directory.",
-)
-@click.option(
-    "-o",
-    "--output-dir",
-    "outputDir",
-    type=click.Path(file_okay=False, resolve_path=True),
-    help="""
-The output directory where the output files are to be created. If it doesn't exist, will be created. If not specified,
-files are saved to the same folder.""",
-)
-@click.option(
-    "--recalc-timestamp",
-    "recalcTimestamp",
-    is_flag=True,
-    default=False,
-    help="""
-By default, original head.modified value is kept when a font is saved. Use this switch to set head.modified timestamp
-to current time.
-""",
-)
-@click.option(
-    "--no-overwrite",
-    "overWrite",
-    is_flag=True,
-    default=True,
-    help="""
-By default, modified files are overwritten. Use this switch to save them to a new file (numbers are appended at the end
-of file name).
-""",
-)
-def copy_metrics(
-    source_file: Path,
-    destination: Path,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Copies vertical metrics from a source font to one or more destination fonts.
-    """
-    fonts = get_fonts_in_path(input_path=destination, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=destination, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    try:
-        source_font = Font(source_file)
-
-        hhea_source = source_font["hhea"]
-        os2_source = source_font["OS/2"]
-
-        ascender = hhea_source.ascender
-        descender = hhea_source.descender
-        lineGap = hhea_source.lineGap
-
-        usWinAscent = os2_source.usWinAscent
-        usWinDescent = os2_source.usWinDescent
-        sTypoAscender = os2_source.sTypoAscender
-        sTypoDescender = os2_source.sTypoDescender
-        sTypoLineGap = os2_source.sTypoLineGap
-
-    except Exception as e:
-        generic_error_message(e)
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-
-            hhea_table = font["hhea"]
-            os2_table = font["OS/2"]
-
-            hhea_table_copy = copy(hhea_table)
-            os2_table_copy = copy(os2_table)
-
-            hhea_table.ascender = ascender
-            hhea_table.descender = descender
-            hhea_table.lineGap = lineGap
-
-            os2_table.usWinAscent = usWinAscent
-            os2_table.usWinDescent = usWinDescent
-            os2_table.sTypoAscender = sTypoAscender
-            os2_table.sTypoDescender = sTypoDescender
-            os2_table.sTypoLineGap = sTypoLineGap
-
-            hhea_modified = hhea_table_copy != hhea_table
-            os2_modified = os2_table_copy != os2_table
-
-            if hhea_modified or os2_modified:
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-cli = click.CommandCollection(
-    sources=[vertical_metrics_tools],
-    help="""
-Vertical metrics tools.
-""",
-)
+from copy import copy
+from pathlib import Path
+
+import click
+from fontTools.misc.cliTools import makeOutputFileName
+
+from foundryToolsCLI.Lib.Font import Font
+from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
+from foundryToolsCLI.Lib.utils.click_tools import (
+    add_common_options,
+    file_saved_message,
+    generic_error_message,
+    add_file_or_path_argument,
+    file_not_changed_message,
+)
+
+vertical_metrics_tools = click.Group("subcommands")
+
+
+@vertical_metrics_tools.command()
+@add_file_or_path_argument()
+@click.option(
+    "-p",
+    "--percent",
+    type=click.IntRange(0, 100),
+    required=True,
+    help="Adjust font line spacing to % of UPM value.",
+)
+@add_common_options()
+def set_linegap(
+    input_path: Path, percent: int, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
+):
+    """Modifies the line spacing metrics in one or more fonts.
+
+    This is a fork of font-line by Source Foundry: https://github.com/source-foundry/font-line
+    """
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+
+            hhea_table = font["hhea"]
+            os2_table = font["OS/2"]
+            hhea_table_copy = copy(font["hhea"])
+            os2_table_copy = copy(font["OS/2"])
+
+            font.modify_linegap_percent(percent=percent)
+
+            hhea_modified = hhea_table_copy != hhea_table
+            os2_modified = os2_table_copy != os2_table
+
+            if hhea_modified or os2_modified:
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@vertical_metrics_tools.command()
+@add_file_or_path_argument()
+@click.option(
+    "--with-linegap",
+    is_flag=True,
+    help="""
+            By default, SIL method (https://silnrsi.github.io/FDBP/en-US/Line_Metrics.html) is used. This means that,
+            in OS/2 table, sTypoAscender and sTypoDescender values are set, respectively, equal to maximum real ascender
+            and minimum real descender, and the sTypoLineGap is set to zero. Use '--with-linegap' to set sTypoAscender
+            value to the maximum ideal ascender (calculated from letters b, f, f, h, k, l and t) and the sTypoDescender
+            value to the minimum ideal descender (calculated from letters g, j, p, q and y). The sTypoLineGap will be
+            calculated as follows: (real ascender + abs(real descender)) - (ideal ascender + abs(ideal descender)).
+    """,
+)
+@add_common_options()
+def align(
+    input_path: Path,
+    with_linegap: bool = False,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Aligns all fonts stored in INPUT_PATH folder to the same baseline.
+
+    To achieve this, the script finds the maximum ascender and the minimum descender values of the fonts stored in the
+    INPUT_PATH folder and applies those values to all fonts.
+
+    This can produce undesired effects (an exaggerated line height) when one or more fonts contain swashes, for example.
+    In such cases, it's better to copy the vertical metrics from a template font to one or more destination fonts using
+    the 'ftcli metrics copy-metrics' command.
+
+    See https://kltf.de/download/FontMetrics-kltf.pdf for more information.
+    """
+
+    import math
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    ideal_ascenders = []
+    ideal_descenders = []
+    real_ascenders = []
+    real_descenders = []
+
+    for font in fonts:
+        try:
+            font_y_min, font_y_max = font.get_bounding_box()
+            real_ascenders.append(math.ceil(font_y_max))
+            real_descenders.append(math.floor(font_y_min))
+
+            if with_linegap:
+                for glyph_name in ["b", "d", "f", "h", "k", "l", "t"]:
+                    ideal_ascenders.append(math.ceil(font.get_glyph_bounds(glyph_name)["yMax"]))
+
+                for glyph_name in ["g", "j", "p", "q", "y"]:
+                    ideal_descenders.append(math.floor(font.get_glyph_bounds(glyph_name)["yMin"]))
+            else:
+                ideal_ascenders = real_ascenders
+                ideal_ascenders = real_descenders
+
+        except Exception as e:
+            generic_error_message(e)
+
+    max_real_ascender = max(real_ascenders)
+    min_real_descender = min(real_descenders)
+    max_ideal_ascender = max(ideal_ascenders) if ideal_descenders != [] else max_real_ascender
+    min_ideal_descender = min(ideal_descenders) if ideal_descenders != [] else min_real_descender
+    typo_line_gap = (max_real_ascender + abs(min_real_descender)) - (max_ideal_ascender + abs(min_ideal_descender))
+
+    for font in fonts:
+        hhea_table = font["hhea"]
+        os2_table = font["OS/2"]
+        hhea_table_copy = copy(hhea_table)
+        os2_table_copy = copy(os2_table)
+
+        try:
+            file = Path(font.reader.file.name)
+            hhea_table.ascender = max_real_ascender
+            hhea_table.descender = min_real_descender
+            hhea_table.lineGap = 0
+
+            os2_table.usWinAscent = max_real_ascender
+            os2_table.usWinDescent = abs(min_real_descender)
+            os2_table.sTypoAscender = max_real_ascender
+            os2_table.sTypoDescender = min_real_descender
+            os2_table.sTypoLineGap = 0
+
+            if with_linegap:
+                os2_table.sTypoAscender = max_ideal_ascender
+                os2_table.sTypoDescender = min_ideal_descender
+                os2_table.sTypoLineGap = typo_line_gap
+
+            hhea_modified = hhea_table_copy != hhea_table
+            os2_modified = os2_table_copy != os2_table
+
+            if hhea_modified or os2_modified:
+                output_file = Path(makeOutputFileName(font.reader.file.name, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@vertical_metrics_tools.command()
+@click.option(
+    "-s",
+    "--source-file",
+    type=click.Path(exists=True, dir_okay=False, resolve_path=True),
+    required=True,
+    help="Source file. Vertical metrics from this font will be applied to all destination fonts.",
+)
+@click.option(
+    "-d",
+    "--destination",
+    type=click.Path(exists=True, resolve_path=True),
+    required=True,
+    help="Destination file or directory.",
+)
+@click.option(
+    "-o",
+    "--output-dir",
+    "outputDir",
+    type=click.Path(file_okay=False, resolve_path=True),
+    help="""
+The output directory where the output files are to be created. If it doesn't exist, will be created. If not specified,
+files are saved to the same folder.""",
+)
+@click.option(
+    "--recalc-timestamp",
+    "recalcTimestamp",
+    is_flag=True,
+    default=False,
+    help="""
+By default, original head.modified value is kept when a font is saved. Use this switch to set head.modified timestamp
+to current time.
+""",
+)
+@click.option(
+    "--no-overwrite",
+    "overWrite",
+    is_flag=True,
+    default=True,
+    help="""
+By default, modified files are overwritten. Use this switch to save them to a new file (numbers are appended at the end
+of file name).
+""",
+)
+def copy_metrics(
+    source_file: Path,
+    destination: Path,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Copies vertical metrics from a source font to one or more destination fonts.
+    """
+    fonts = get_fonts_in_path(input_path=destination, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=destination, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    try:
+        source_font = Font(source_file)
+
+        hhea_source = source_font["hhea"]
+        os2_source = source_font["OS/2"]
+
+        ascender = hhea_source.ascender
+        descender = hhea_source.descender
+        lineGap = hhea_source.lineGap
+
+        usWinAscent = os2_source.usWinAscent
+        usWinDescent = os2_source.usWinDescent
+        sTypoAscender = os2_source.sTypoAscender
+        sTypoDescender = os2_source.sTypoDescender
+        sTypoLineGap = os2_source.sTypoLineGap
+
+    except Exception as e:
+        generic_error_message(e)
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+
+            hhea_table = font["hhea"]
+            os2_table = font["OS/2"]
+
+            hhea_table_copy = copy(hhea_table)
+            os2_table_copy = copy(os2_table)
+
+            hhea_table.ascender = ascender
+            hhea_table.descender = descender
+            hhea_table.lineGap = lineGap
+
+            os2_table.usWinAscent = usWinAscent
+            os2_table.usWinDescent = usWinDescent
+            os2_table.sTypoAscender = sTypoAscender
+            os2_table.sTypoDescender = sTypoDescender
+            os2_table.sTypoLineGap = sTypoLineGap
+
+            hhea_modified = hhea_table_copy != hhea_table
+            os2_modified = os2_table_copy != os2_table
+
+            if hhea_modified or os2_modified:
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+cli = click.CommandCollection(
+    sources=[vertical_metrics_tools],
+    help="""
+Vertical metrics tools.
+""",
+)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_name.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_name.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,423 +1,422 @@
-from copy import deepcopy
-from pathlib import Path
-
-import click
-from fontTools.misc.cliTools import makeOutputFileName
-
-from foundryToolsCLI.Lib.constants import LANGUAGES_EPILOG
-from foundryToolsCLI.Lib.tables.name import TableName
-from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
-from foundryToolsCLI.Lib.utils.click_tools import (
-    add_file_or_path_argument,
-    add_common_options,
-    file_saved_message,
-    file_not_changed_message,
-    generic_error_message,
-)
-
-CWD = Path.cwd()
-tbl_name = click.Group("subcommands")
-
-
-@tbl_name.command(epilog=LANGUAGES_EPILOG)
-@add_file_or_path_argument()
-@click.option(
-    "-n",
-    "--name-id",
-    type=click.IntRange(0, 32767),
-    required=True,
-    help="nameID of the NameRecord to add.",
-)
-@click.option("-s", "--string", required=True, help="The string to write in the NameRecord.")
-@click.option(
-    "-p",
-    "--platform-id",
-    type=click.Choice(choices=["1", "3"]),
-    help="""
-    platformID of the NameRecord to add (1: Macintosh, 3: Windows).
-    
-    If platformID is not specified, both a platformID=1 and a platformID=3 NameRecords will be added.
-    """,
-)
-@click.option(
-    "-l",
-    "--language-string",
-    default="en",
-    show_default=True,
-    help="""
-    Write the NameRecord in a language different than English (e.g.: 'it', 'nl', 'de').
-
-    See epilog for a list of valid language strings.
-    """,
-)
-@add_common_options()
-def set_name(
-    input_path: Path,
-    name_id: int,
-    platform_id: int,
-    string: str,
-    language_string: str,
-    recalc_timestamp: bool,
-    output_dir: Path,
-    overwrite: bool,
-) -> None:
-    """
-    Writes a NameRecord in the 'name' table.
-    """
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    if platform_id:
-        platform_id = int(platform_id)
-
-    for font in fonts:
-        try:
-            name_table: TableName = font["name"]
-            name_table_copy = deepcopy(name_table)
-
-            name_table.add_name(
-                font,
-                name_id=name_id,
-                string=string,
-                platform_id=platform_id,
-                language_string=language_string,
-            )
-
-            file = Path(font.reader.file.name)
-            if name_table_copy.compile(font) != name_table.compile(font):
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_name.command(epilog=LANGUAGES_EPILOG)
-@add_file_or_path_argument()
-@click.option(
-    "-n",
-    "--name-id",
-    "name_ids",
-    type=click.IntRange(0, 32767, max_open=True),
-    required=True,
-    multiple=True,
-    help="""
-    nameID of the NameRecord to delete.
-
-    This option can be repeated to delete multiple NameRecords at once (e.g.: -x 3 -x 5 -x 6).
-    """,
-)
-@click.option(
-    "-p",
-    "--platform-id",
-    type=click.Choice(choices=["0", "1", "3"]),
-    help="""
-    If platformID is specified, only NameRecords with matching platformID will be deleted.
-
-    Valid platformID values are: 0 (Unicode), 1 (Macintosh), 3 (Windows).
-    """,
-)
-@click.option(
-    "-l",
-    "--language-string",
-    default=None,
-    show_default=True,
-    help="""
-    Filter the NameRecords to delete by language string (for example: 'it', 'de', 'nl').
-
-    See epilog for a list of valid language strings.
-    """,
-)
-@add_common_options()
-def del_names(
-    input_path: Path,
-    name_ids: tuple[int],
-    platform_id: int,
-    language_string: str,
-    recalc_timestamp: bool = False,
-    output_dir: Path = None,
-    overwrite: bool = True,
-):
-    """
-    Deletes one or more NameRecords.
-    """
-
-    fonts = get_fonts_in_path(input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    if platform_id:
-        platform_id = int(platform_id)
-
-    for font in fonts:
-        try:
-            name_table: TableName = font["name"]
-            name_table_copy = deepcopy(name_table)
-
-            name_table.del_names(
-                name_ids=name_ids,
-                platform_id=platform_id,
-                language_string=language_string,
-            )
-
-            file = Path(font.reader.file.name)
-            if name_table_copy.compile(font) != name_table.compile(font):
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_name.command()
-@add_file_or_path_argument()
-@click.option("-os", "--old-string", required=True, help="The string to be replaced")
-@click.option("-ns", "--new-string", required=True, help="The string to replace the old string with")
-@click.option(
-    "-n",
-    "--name-id",
-    "name_ids",
-    type=click.IntRange(0, 32767, max_open=True),
-    multiple=True,
-    help="""
-    nameID of the NameRecords where to search and replace the string.
-
-    If nameID is not specified, the string will be replaced in all NameRecords.
-
-    This option can be repeated (e.g.: -x 3 -x 5 -x 6).
-    """,
-)
-@click.option(
-    "-x",
-    "--exclude-name-id",
-    "excluded_name_ids",
-    type=click.IntRange(0, 32767, max_open=True),
-    multiple=True,
-    help="""
-    nameID of the NameRecords to skip.
-
-    This option can be repeated (e.g.: -x 3 -x 5 -x 6).
-    """,
-)
-@click.option(
-    "-p",
-    "--platform-id",
-    type=click.Choice(choices=["0", "1", "3"]),
-    help="""
-    platformID of the NameRecords where to perform find and replace (0: Unicode, 1: Macintosh, 3: Windows).
-    """,
-)
-@add_common_options()
-def find_replace(
-    input_path: Path,
-    old_string: str,
-    new_string: str,
-    name_ids: tuple[int],
-    excluded_name_ids: tuple[int],
-    platform_id: int,
-    recalc_timestamp: bool = False,
-    output_dir: Path = None,
-    overwrite: bool = True,
-):
-    """
-    Finds a string in the specified NameRecords and replaces it with a new string
-    """
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    if platform_id:
-        platform_id = int(platform_id)
-
-    for font in fonts:
-        try:
-            name_table: TableName = font["name"]
-            name_table_copy = deepcopy(name_table)
-
-            name_table.find_replace(
-                old_string=old_string,
-                new_string=new_string,
-                name_ids_to_include=name_ids,
-                name_ids_to_skip=excluded_name_ids,
-                platform_id=platform_id,
-            )
-
-            file = Path(font.reader.file.name)
-            if name_table_copy.compile(font) != name_table.compile(font):
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_name.command()
-@add_file_or_path_argument()
-@click.option("--del-all", is_flag=True, help="Deletes also nameIDs 1, 2, 4, 5 and 6.")
-@add_common_options()
-def del_mac_names(
-    input_path: Path,
-    del_all: bool = False,
-    recalc_timestamp: bool = False,
-    output_dir: bool = None,
-    overwrite: bool = True,
-):
-    """
-    Deletes all the Macintosh NameRecords (platformID=1) from the name table, except the ones with nameID 1, 2, 4, 5,
-    and 6.
-
-    According to Apple (https://developer.apple.com/fonts/TrueType-Reference-Manual/RM06/Chap6name.html), "names with
-    platformID 1 were required by earlier versions of macOS. Its use on modern platforms is discouraged. Use names with
-    platformID 3 instead for maximum compatibility. Some legacy software, however, may still require names with
-    platformID 1, platformSpecificID 0".
-    """
-
-    fonts = get_fonts_in_path(input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            name_table: TableName = font["name"]
-            name_table_copy = deepcopy(name_table)
-            name_ids = set(name.nameID for name in name_table.names if name.platformID == 1)
-            if not del_all:
-                for n in (1, 2, 4, 5, 6):
-                    try:
-                        name_ids.remove(n)
-                    except KeyError:
-                        pass
-
-            name_table.del_names(name_ids=name_ids, platform_id=1)
-
-            file = Path(font.reader.file.name)
-            if name_table_copy.compile(font) != name_table.compile(font):
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_name.command(epilog=LANGUAGES_EPILOG)
-@add_file_or_path_argument()
-@click.option(
-    "-n",
-    "--name-id",
-    "name_ids",
-    required=True,
-    multiple=True,
-    type=int,
-    help="""
-    nameID of the NameRecords where to append the prefix/suffix.
-
-    This option can be repeated to prepend/append the string to multiple NameRecords (e.g.: -x 3 -x 5 -x 6).
-    """,
-)
-@click.option(
-    "-p",
-    "--platform-id",
-    type=click.Choice(choices=["0", "1", "3"]),
-    help="""
-    Use this option to add the prefix/suffix only to the NameRecords matching the provided platformID (0: Unicode, 1:
-    Macintosh, 3: Windows).
-    """,
-)
-@click.option(
-    "-l",
-    "--language-string",
-    help="""
-    Use this option to append the prefix/suffix only to the NameRecords matching the provided language string.
-    
-    See epilog for a list of valid language strings.
-    """,
-)
-@click.option("--prefix", type=str, help="The string to be prepended to the NameRecords")
-@click.option("--suffix", type=str, help="The suffix to append to the NameRecords")
-@add_common_options()
-def append(
-    input_path: Path,
-    name_ids: tuple[int],
-    platform_id: int,
-    language_string: str,
-    prefix: str,
-    suffix: str,
-    recalc_timestamp: bool = False,
-    output_dir: Path = None,
-    overwrite: bool = True,
-):
-    """
-    Appends a prefix and/or a suffix to the specified NameRecords.
-    """
-
-    if prefix is None and suffix is None:
-        generic_error_message("Please, insert at least a prefix or a suffix to append")
-        return
-
-    fonts = get_fonts_in_path(input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    if platform_id:
-        platform_id = int(platform_id)
-
-    for font in fonts:
-        try:
-            name_table: TableName = font["name"]
-            name_table_copy = deepcopy(name_table)
-
-            name_table.append_string(
-                name_ids=name_ids,
-                platform_id=platform_id,
-                language_string=language_string,
-                prefix=prefix,
-                suffix=suffix,
-            )
-            file = Path(font.reader.file.name)
-            if name_table.compile(font) != name_table_copy.compile(font):
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-cli = click.CommandCollection(
-    sources=[tbl_name],
-    help="""
-    A set of tools to manipulate the 'name' table.
-    """,
-)
+from copy import deepcopy
+from pathlib import Path
+
+import click
+from fontTools.misc.cliTools import makeOutputFileName
+
+from foundryToolsCLI.Lib.constants import LANGUAGES_EPILOG
+from foundryToolsCLI.Lib.tables.name import TableName
+from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
+from foundryToolsCLI.Lib.utils.click_tools import (
+    add_file_or_path_argument,
+    add_common_options,
+    file_saved_message,
+    file_not_changed_message,
+    generic_error_message,
+)
+
+tbl_name = click.Group("subcommands")
+
+
+@tbl_name.command(epilog=LANGUAGES_EPILOG)
+@add_file_or_path_argument()
+@click.option(
+    "-n",
+    "--name-id",
+    type=click.IntRange(0, 32767),
+    required=True,
+    help="nameID of the NameRecord to add.",
+)
+@click.option("-s", "--string", required=True, help="The string to write in the NameRecord.")
+@click.option(
+    "-p",
+    "--platform-id",
+    type=click.Choice(choices=["1", "3"]),
+    help="""
+    platformID of the NameRecord to add (1: Macintosh, 3: Windows).
+    
+    If platformID is not specified, both a platformID=1 and a platformID=3 NameRecords will be added.
+    """,
+)
+@click.option(
+    "-l",
+    "--language-string",
+    default="en",
+    show_default=True,
+    help="""
+    Write the NameRecord in a language different than English (e.g.: 'it', 'nl', 'de').
+
+    See epilog for a list of valid language strings.
+    """,
+)
+@add_common_options()
+def set_name(
+    input_path: Path,
+    name_id: int,
+    platform_id: int,
+    string: str,
+    language_string: str,
+    recalc_timestamp: bool,
+    output_dir: Path,
+    overwrite: bool,
+) -> None:
+    """
+    Writes a NameRecord in the 'name' table.
+    """
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    if platform_id:
+        platform_id = int(platform_id)
+
+    for font in fonts:
+        try:
+            name_table: TableName = font["name"]
+            name_table_copy = deepcopy(name_table)
+
+            name_table.add_name(
+                font,
+                name_id=name_id,
+                string=string,
+                platform_id=platform_id,
+                language_string=language_string,
+            )
+
+            file = Path(font.reader.file.name)
+            if name_table_copy.compile(font) != name_table.compile(font):
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_name.command(epilog=LANGUAGES_EPILOG)
+@add_file_or_path_argument()
+@click.option(
+    "-n",
+    "--name-id",
+    "name_ids",
+    type=click.IntRange(0, 32767, max_open=True),
+    required=True,
+    multiple=True,
+    help="""
+    nameID of the NameRecord to delete.
+
+    This option can be repeated to delete multiple NameRecords at once (e.g.: -x 3 -x 5 -x 6).
+    """,
+)
+@click.option(
+    "-p",
+    "--platform-id",
+    type=click.Choice(choices=["0", "1", "3"]),
+    help="""
+    If platformID is specified, only NameRecords with matching platformID will be deleted.
+
+    Valid platformID values are: 0 (Unicode), 1 (Macintosh), 3 (Windows).
+    """,
+)
+@click.option(
+    "-l",
+    "--language-string",
+    default=None,
+    show_default=True,
+    help="""
+    Filter the NameRecords to delete by language string (for example: 'it', 'de', 'nl').
+
+    See epilog for a list of valid language strings.
+    """,
+)
+@add_common_options()
+def del_names(
+    input_path: Path,
+    name_ids: tuple[int],
+    platform_id: int,
+    language_string: str,
+    recalc_timestamp: bool = False,
+    output_dir: Path = None,
+    overwrite: bool = True,
+):
+    """
+    Deletes one or more NameRecords.
+    """
+
+    fonts = get_fonts_in_path(input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    if platform_id:
+        platform_id = int(platform_id)
+
+    for font in fonts:
+        try:
+            name_table: TableName = font["name"]
+            name_table_copy = deepcopy(name_table)
+
+            name_table.del_names(
+                name_ids=name_ids,
+                platform_id=platform_id,
+                language_string=language_string,
+            )
+
+            file = Path(font.reader.file.name)
+            if name_table_copy.compile(font) != name_table.compile(font):
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_name.command()
+@add_file_or_path_argument()
+@click.option("-os", "--old-string", required=True, help="The string to be replaced")
+@click.option("-ns", "--new-string", required=True, help="The string to replace the old string with")
+@click.option(
+    "-n",
+    "--name-id",
+    "name_ids",
+    type=click.IntRange(0, 32767, max_open=True),
+    multiple=True,
+    help="""
+    nameID of the NameRecords where to search and replace the string.
+
+    If nameID is not specified, the string will be replaced in all NameRecords.
+
+    This option can be repeated (e.g.: -x 3 -x 5 -x 6).
+    """,
+)
+@click.option(
+    "-x",
+    "--exclude-name-id",
+    "excluded_name_ids",
+    type=click.IntRange(0, 32767, max_open=True),
+    multiple=True,
+    help="""
+    nameID of the NameRecords to skip.
+
+    This option can be repeated (e.g.: -x 3 -x 5 -x 6).
+    """,
+)
+@click.option(
+    "-p",
+    "--platform-id",
+    type=click.Choice(choices=["0", "1", "3"]),
+    help="""
+    platformID of the NameRecords where to perform find and replace (0: Unicode, 1: Macintosh, 3: Windows).
+    """,
+)
+@add_common_options()
+def find_replace(
+    input_path: Path,
+    old_string: str,
+    new_string: str,
+    name_ids: tuple[int],
+    excluded_name_ids: tuple[int],
+    platform_id: int,
+    recalc_timestamp: bool = False,
+    output_dir: Path = None,
+    overwrite: bool = True,
+):
+    """
+    Finds a string in the specified NameRecords and replaces it with a new string
+    """
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    if platform_id:
+        platform_id = int(platform_id)
+
+    for font in fonts:
+        try:
+            name_table: TableName = font["name"]
+            name_table_copy = deepcopy(name_table)
+
+            name_table.find_replace(
+                old_string=old_string,
+                new_string=new_string,
+                name_ids_to_include=name_ids,
+                name_ids_to_skip=excluded_name_ids,
+                platform_id=platform_id,
+            )
+
+            file = Path(font.reader.file.name)
+            if name_table_copy.compile(font) != name_table.compile(font):
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_name.command()
+@add_file_or_path_argument()
+@click.option("--del-all", is_flag=True, help="Deletes also nameIDs 1, 2, 4, 5 and 6.")
+@add_common_options()
+def del_mac_names(
+    input_path: Path,
+    del_all: bool = False,
+    recalc_timestamp: bool = False,
+    output_dir: bool = None,
+    overwrite: bool = True,
+):
+    """
+    Deletes all the Macintosh NameRecords (platformID=1) from the name table, except the ones with nameID 1, 2, 4, 5,
+    and 6.
+
+    According to Apple (https://developer.apple.com/fonts/TrueType-Reference-Manual/RM06/Chap6name.html), "names with
+    platformID 1 were required by earlier versions of macOS. Its use on modern platforms is discouraged. Use names with
+    platformID 3 instead for maximum compatibility. Some legacy software, however, may still require names with
+    platformID 1, platformSpecificID 0".
+    """
+
+    fonts = get_fonts_in_path(input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            name_table: TableName = font["name"]
+            name_table_copy = deepcopy(name_table)
+            name_ids = set(name.nameID for name in name_table.names if name.platformID == 1)
+            if not del_all:
+                for n in (1, 2, 4, 5, 6):
+                    try:
+                        name_ids.remove(n)
+                    except KeyError:
+                        pass
+
+            name_table.del_names(name_ids=name_ids, platform_id=1)
+
+            file = Path(font.reader.file.name)
+            if name_table_copy.compile(font) != name_table.compile(font):
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_name.command(epilog=LANGUAGES_EPILOG)
+@add_file_or_path_argument()
+@click.option(
+    "-n",
+    "--name-id",
+    "name_ids",
+    required=True,
+    multiple=True,
+    type=int,
+    help="""
+    nameID of the NameRecords where to append the prefix/suffix.
+
+    This option can be repeated to prepend/append the string to multiple NameRecords (e.g.: -x 3 -x 5 -x 6).
+    """,
+)
+@click.option(
+    "-p",
+    "--platform-id",
+    type=click.Choice(choices=["0", "1", "3"]),
+    help="""
+    Use this option to add the prefix/suffix only to the NameRecords matching the provided platformID (0: Unicode, 1:
+    Macintosh, 3: Windows).
+    """,
+)
+@click.option(
+    "-l",
+    "--language-string",
+    help="""
+    Use this option to append the prefix/suffix only to the NameRecords matching the provided language string.
+    
+    See epilog for a list of valid language strings.
+    """,
+)
+@click.option("--prefix", type=str, help="The string to be prepended to the NameRecords")
+@click.option("--suffix", type=str, help="The suffix to append to the NameRecords")
+@add_common_options()
+def append(
+    input_path: Path,
+    name_ids: tuple[int],
+    platform_id: int,
+    language_string: str,
+    prefix: str,
+    suffix: str,
+    recalc_timestamp: bool = False,
+    output_dir: Path = None,
+    overwrite: bool = True,
+):
+    """
+    Appends a prefix and/or a suffix to the specified NameRecords.
+    """
+
+    if prefix is None and suffix is None:
+        generic_error_message("Please, insert at least a prefix or a suffix to append")
+        return
+
+    fonts = get_fonts_in_path(input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    if platform_id:
+        platform_id = int(platform_id)
+
+    for font in fonts:
+        try:
+            name_table: TableName = font["name"]
+            name_table_copy = deepcopy(name_table)
+
+            name_table.append_string(
+                name_ids=name_ids,
+                platform_id=platform_id,
+                language_string=language_string,
+                prefix=prefix,
+                suffix=suffix,
+            )
+            file = Path(font.reader.file.name)
+            if name_table.compile(font) != name_table_copy.compile(font):
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+cli = click.CommandCollection(
+    sources=[tbl_name],
+    help="""
+    A set of tools to manipulate the 'name' table.
+    """,
+)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_os2.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_os2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,572 +1,570 @@
-import os
-from copy import deepcopy
-from pathlib import Path
-
-import click
-from fontTools.misc.cliTools import makeOutputFileName
-
-from foundryToolsCLI.Lib.Font import Font
-from foundryToolsCLI.Lib.tables.OS_2 import TableOS2
-from foundryToolsCLI.Lib.utils.bits_tools import unset_nth_bit
-from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
-from foundryToolsCLI.Lib.utils.click_tools import (
-    add_file_or_path_argument,
-    add_common_options,
-    generic_error_message,
-    generic_warning_message,
-    file_saved_message,
-    file_not_changed_message,
-)
-
-CWD = Path.cwd()
-
-tbl_os2 = click.Group("subcommands")
-
-
-@tbl_os2.command()
-@add_file_or_path_argument()
-@add_common_options()
-def recalc_x_height(input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True):
-    """
-    Recalculates sxHeight value.
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            os_2: TableOS2 = font["OS/2"]
-            if os_2.version < 25:
-                generic_warning_message(
-                    f"{file.name}: sxHeight is defined only in OS/2 version 2 and up. Current version is {os_2.version}"
-                )
-                continue
-
-            current = os_2.sxHeight
-            x_height = font.recalc_x_height()
-            if current == x_height:
-                file_not_changed_message(file.relative_to(CWD))
-                continue
-
-            os_2.set_x_height(x_height)
-            output_file = Path(makeOutputFileName(input=file, outputDir=output_dir, overWrite=overwrite))
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_os2.command()
-@add_file_or_path_argument()
-@add_common_options()
-def recalc_cap_height(
-    input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True
-):
-    """
-    Recalculates sCapHeight value.
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            os_2: TableOS2 = font["OS/2"]
-            if os_2.version < 2:
-                generic_warning_message(
-                    f"{file.name}: "
-                    f"sCapHeight is defined only in OS/2 version 2 and up. Current version is {os_2.version}"
-                )
-                continue
-
-            current = os_2.sCapHeight
-            cap_height = font.recalc_cap_height()
-            if current == cap_height:
-                file_not_changed_message(file.relative_to(CWD))
-                continue
-
-            os_2.set_cap_height(cap_height)
-            output_file = Path(makeOutputFileName(input=file, outputDir=output_dir, overWrite=overwrite))
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_os2.command()
-@add_file_or_path_argument()
-@add_common_options()
-def recalc_max_context(
-    input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True
-):
-    """
-    Recalculates usMaxContext value.
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            os_2: TableOS2 = font["OS/2"]
-
-            if os_2.version < 2:
-                generic_warning_message(
-                    f"{file.name}: "
-                    f"usMaxContext is defined only in OS/2 version 2 and up. Current version is {os_2.version}"
-                )
-                continue
-
-            current = os_2.usMaxContex
-            max_context = font.recalc_max_context()
-            if current == max_context:
-                file_not_changed_message(file.relative_to(CWD))
-                continue
-
-            os_2.usMaxContext = max_context
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_os2.command()
-@add_file_or_path_argument()
-@add_common_options()
-def recalc_ranges(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
-    """
-    Generates a temporary Type 1 from the font file using tx, converts that to an OpenType font using makeotf, reads the
-    Unicode ranges and codepage ranges from the temporary OpenType font file, and then writes those ranges to the
-    original font's OS/2 table.
-    """
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            temp_otf_fd, temp_otf_file = font.make_temp_otf()
-            temp_font = Font(temp_otf_file)
-
-            os_2: TableOS2 = font["OS/2"]
-            os_2_temp: TableOS2 = temp_font["OS/2"]
-            current_unicode_ranges = os_2.getUnicodeRanges()
-            current_codepage_ranges = os_2.get_codepage_ranges()
-            new_unicode_ranges = os_2_temp.getUnicodeRanges()
-            new_codepage_ranges = os_2_temp.get_codepage_ranges()
-
-            if current_unicode_ranges != new_unicode_ranges or current_codepage_ranges != new_codepage_ranges:
-                os_2.setUnicodeRanges(bits=new_unicode_ranges)
-                os_2.set_codepage_ranges(codepage_ranges=new_codepage_ranges)
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-            temp_font.close()
-            os.close(temp_otf_fd)
-            os.remove(temp_otf_file)
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_os2.command()
-@add_file_or_path_argument()
-@click.option(
-    "-it/-no-it",
-    "--italic/--no-italic",
-    "italic",
-    default=None,
-    help="Sets or clears the ITALIC bits (`fsSelection` bit 0 and `head` table `macStyle` bit 1).",
-)
-@click.option(
-    "-us/-no-us",
-    "--underscore/--no-underscore",
-    "underscore",
-    default=None,
-    help="""
-Sets or clears `fsType` bit 1 (UNDERSCORE).
-""",
-)
-@click.option(
-    "-ng/-no-ng",
-    "--negative/--no-negative",
-    "negative",
-    default=None,
-    help="""
-Sets or clears `fsType` bit 2 (NEGATIVE).
-""",
-)
-@click.option(
-    "-ol/-no-ol",
-    "--outlined/--no-outlined",
-    "outlined",
-    default=None,
-    help="""
-Sets or clears `fsType` bit 3 (OUTLINED).
-""",
-)
-@click.option(
-    "-st/-no-st",
-    "--strikeout/--no-strikeout",
-    "strikeout",
-    default=None,
-    help="""
-Sets or clears `fsType` bit 4 (STRIKEOUT).
-""",
-)
-@click.option(
-    "-bd/-no-bd",
-    "--bold/--no-bold",
-    "bold",
-    default=None,
-    help="Sets or clears the BOLD bits (`OS/2.fsSelection` bit 5 and `head.macStyle` bit 0).",
-)
-@click.option(
-    "-rg",
-    "--regular",
-    "regular",
-    is_flag=True,
-    default=None,
-    help="""
-Sets REGULAR (`fsSelection` bit 6) and clears BOLD (`fsSelection` bit 5, `head.macStyle` bit 0) and ITALIC
-(`fsSelection` bit 0, `head.macStyle` bit 1) bits. This is equivalent to `--no-bold --no-italic`.
-""",
-)
-@click.option(
-    "-utm/-no-utm",
-    "--use-typo-metrics/--no-use-typo-metrics",
-    "use_typo_metrics",
-    default=None,
-    help="""
-Sets or clears the USE_TYPO_METRICS bit (`fsSelection` bit 7).
-
-If set, it is strongly recommended that applications use `OS/2.sTypoAscender` - `OS/2.sTypoDescender` + 
-`OS/2.sTypoLineGap` as the default line spacing for the font.
-
-See: https://docs.microsoft.com/en-us/typography/opentype/spec/os2#fsselection
-""",
-)
-@click.option(
-    "-wws/-no-wws",
-    "--wws-consistent/--no-wws-consistent",
-    "wws_consistent",
-    default=None,
-    help="""
-Sets or clears the WWS bit (`fsSelection` bit 8).
-
-If the `OS/2.fsSelection` bit is set, the font has `name` table strings consistent with a weight/width/slope family
-without requiring use of name IDs 21 and 22.
-
-See: https://docs.microsoft.com/en-us/typography/opentype/spec/os2#fsselection
-
-Also: https://typedrawers.com/discussion/3857/fontlab-7-windows-reads-exported-font-name-differently
-""",
-)
-@click.option(
-    "-obl/-no-obl",
-    "--oblique/--no-oblique",
-    "oblique",
-    default=None,
-    help="Sets or clears the OBLIQUE bit (`fsSelection` bit 9).",
-)
-@click.option(
-    "-el",
-    "--embed-level",
-    "embed_level",
-    type=click.Choice(["0", "2", "4", "8"]),
-    default=None,
-    help="""
-Sets/clears `fsType` bits 0-3 (EMBEDDING_LEVEL).
-
-Valid fonts must set at most one of bits 1, 2 or 3; bit 0 is permanently reserved and must be zero. Valid values for
-this sub-field are 0, 2, 4 or 8. The meaning of these values is as follows:
-
-\b
-0: Installable embedding
-2: Restricted License embedding
-4: Preview & Print embedding
-8: Editable embedding
-
-See: https://docs.microsoft.com/en-us/typography/opentype/spec/os2#fstype
-""",
-)
-@click.option(
-    "-ns/-as",
-    "--no-subsetting/--allow-subsetting",
-    default=None,
-    help="""
-Sets or clears `fsType` bit 8 (NO_SUBSETTING).
-
-When this bit is set, the font may not be subsetted prior to embedding. Other embedding restrictions specified in bits
-0-3 and 9 also apply.
-""",
-)
-@click.option(
-    "-beo/-no-beo",
-    "--bitmap-embedding-only/--no-bitmap-embedding-only",
-    default=None,
-    help="""
-Sets or clears `fsType` bit 9 (BITMAP_EMBEDDING_ONLY).
-
-When this bit is set, only bitmaps contained in the font may be embedded. No outline data may be embedded. If there are
-no bitmaps available in the font, then the font is considered unembeddable and the embedding services will fail. Other
-embedding restrictions specified in bits 0-3 and 8 also apply.
-""",
-)
-@add_common_options()
-def set_flags(
-    input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True, **kwargs
-):
-    """
-    Sets/clears the following flags in OS/2.fsSelection and OS/2.fsType fields:
-
-    fsSelection:
-
-    \b
-    Bit 0: ITALIC
-    Bit 1: UNDERSCORE
-    Bit 2: NEGATIVE
-    Bit 3: OUTLINED
-    Bit 4: STRIKEOUT
-    Bit 5: BOLD
-    Bit 6: REGULAR
-    Bit 7: USE_TYPO_METRICS
-    Bit 8: WWS
-    Bit 9: OBLIQUE
-
-    fsType:
-
-    \b
-    Bits 0-3: Usage permissions
-    Bit 8: No subsetting
-    Bit 9: Bitmap embedding only
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    options = {k: v for k, v in kwargs.items() if v is not None}
-    if len(options) == 0:
-        generic_error_message("Please, pass at least one valid parameter.")
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-
-            head = font["head"]
-            head_copy = deepcopy(head)
-            os2 = font["OS/2"]
-            os2_copy = deepcopy(os2)
-
-            for flag, value in options.items():
-                if flag in ("use_typo_metrics", "wws_consistent", "oblique") and os2.version < 4:
-                    generic_warning_message(
-                        f"{flag.upper()} flag can't be set. Bits 7, 8 and 9 are only defined in OS/2 version 4 and up."
-                    )
-                    continue
-                if flag == "embed_level":
-                    value = int(value)
-                set_flag = getattr(font, f"set_{flag}_flag")
-                set_flag(value)
-
-            if head_copy.compile(font) != head.compile(font) or os2_copy.compile(font) != os2.compile(font):
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_os2.command()
-@click.option("-v", "target_version", type=click.IntRange(1, 5), required=True, help="Target version")
-@add_file_or_path_argument()
-@add_common_options()
-def set_version(
-    input_path: Path,
-    target_version: int,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Upgrades OS/2 table version.
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-
-            os_2: TableOS2 = font["OS/2"]
-            current_version = getattr(os_2, "version")
-
-            if target_version <= current_version:
-                generic_warning_message(f"Current OS/2 table version is already {current_version}")
-                file_not_changed_message(file=file.relative_to(CWD))
-                continue
-
-            setattr(os_2, "version", target_version)
-
-            # When upgrading from version 0, ulCodePageRanges are to be recalculated.
-            if current_version < 1:
-                temp_otf_fd, temp_otf_file = font.make_temp_otf()
-                temp_otf_font = Font(temp_otf_file)
-                temp_os_2: TableOS2 = temp_otf_font["OS/2"]
-                os_2.set_codepage_ranges(temp_os_2.get_codepage_ranges())
-
-                temp_otf_font.close()
-                os.close(temp_otf_fd)
-                os.remove(temp_otf_file)
-
-            # Return if upgrading from version 0 to version 1.
-            if target_version == 1:
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-                continue
-
-            # Upgrading from version 1 requires creating sxHeight, sCapHeight, usDefaultChar, usBreakChar and
-            # usMaxContext entries.
-            if current_version < 2:
-                os_2.set_x_height(font.recalc_x_height())
-                os_2.set_cap_height(font.recalc_cap_height())
-                os_2.set_default_char(0)
-                os_2.set_break_char(32)
-                os_2.set_max_context(font.recalc_max_context())
-
-            # Write default values if target_version == 5.
-            if target_version > 4:
-                setattr(os_2, "usLowerOpticalPointSize", 0)
-                setattr(os_2, "usUpperOpticalPointSize", 65535 / 20)
-
-            # Finally, make sure to clear bits 7, 8 and 9 in ['OS/2'].fsSelection when target version is lower than 4.
-            if target_version < 4:
-                for b in (7, 8, 9):
-                    setattr(os_2, "fsSelection", unset_nth_bit(os_2.fsSelection, b))
-
-            font.save(output_file)
-            file_saved_message(file=output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_os2.command()
-@add_file_or_path_argument()
-@click.option("-w", "--weight", type=click.IntRange(1, 1000), required=True, help="usWeightClass value.")
-@add_common_options()
-def set_weight(
-    input_path: Path, weight: int, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
-):
-    """
-    Sets the Weight class value.
-
-    usWeightClass indicates the visual weight (degree of blackness or thickness of strokes) of the characters in the
-    font. Values from 1 to 1000 are valid.
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            os_2: TableOS2 = font["OS/2"]
-
-            if weight == os_2.get_weight_class():
-                file_not_changed_message(file.relative_to(CWD))
-                continue
-
-            os_2.set_weight_class(weight)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@tbl_os2.command()
-@add_file_or_path_argument()
-@click.option("-w", "--width", type=click.IntRange(1, 9), required=True, help="usWidthClass value.")
-@add_common_options()
-def set_width(
-    input_path: Path, width: int, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
-):
-    """
-    Sets the Width class value.
-
-    usWidthClass indicates a relative change from the normal aspect ratio (width to height ratio) as specified by a font
-    designer for the glyphs in a font. Values from 1 to 9 are valid.
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            os_2: TableOS2 = font["OS/2"]
-
-            if width == os_2.get_width_class():
-                file_not_changed_message(file.relative_to(CWD))
-                continue
-
-            os_2.set_width_class(width)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-cli = click.CommandCollection(
-    sources=[tbl_os2],
-    help="""
-    A set of tools to manipulate the 'OS/2' table.
-    """,
-)
+import os
+from copy import deepcopy
+from pathlib import Path
+
+import click
+from fontTools.misc.cliTools import makeOutputFileName
+
+from foundryToolsCLI.Lib.Font import Font
+from foundryToolsCLI.Lib.tables.OS_2 import TableOS2
+from foundryToolsCLI.Lib.utils.bits_tools import unset_nth_bit
+from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
+from foundryToolsCLI.Lib.utils.click_tools import (
+    add_file_or_path_argument,
+    add_common_options,
+    generic_error_message,
+    generic_warning_message,
+    file_saved_message,
+    file_not_changed_message,
+)
+
+tbl_os2 = click.Group("subcommands")
+
+
+@tbl_os2.command()
+@add_file_or_path_argument()
+@add_common_options()
+def recalc_x_height(input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True):
+    """
+    Recalculates sxHeight value.
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            os_2: TableOS2 = font["OS/2"]
+            if os_2.version < 25:
+                generic_warning_message(
+                    f"{file.name}: sxHeight is defined only in OS/2 version 2 and up. Current version is {os_2.version}"
+                )
+                continue
+
+            current = os_2.sxHeight
+            x_height = font.recalc_x_height()
+            if current == x_height:
+                file_not_changed_message(file)
+                continue
+
+            os_2.set_x_height(x_height)
+            output_file = Path(makeOutputFileName(input=file, outputDir=output_dir, overWrite=overwrite))
+            font.save(output_file)
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_os2.command()
+@add_file_or_path_argument()
+@add_common_options()
+def recalc_cap_height(
+    input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True
+):
+    """
+    Recalculates sCapHeight value.
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            os_2: TableOS2 = font["OS/2"]
+            if os_2.version < 2:
+                generic_warning_message(
+                    f"{file.name}: "
+                    f"sCapHeight is defined only in OS/2 version 2 and up. Current version is {os_2.version}"
+                )
+                continue
+
+            current = os_2.sCapHeight
+            cap_height = font.recalc_cap_height()
+            if current == cap_height:
+                file_not_changed_message(file)
+                continue
+
+            os_2.set_cap_height(cap_height)
+            output_file = Path(makeOutputFileName(input=file, outputDir=output_dir, overWrite=overwrite))
+            font.save(output_file)
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_os2.command()
+@add_file_or_path_argument()
+@add_common_options()
+def recalc_max_context(
+    input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True
+):
+    """
+    Recalculates usMaxContext value.
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            os_2: TableOS2 = font["OS/2"]
+
+            if os_2.version < 2:
+                generic_warning_message(
+                    f"{file.name}: "
+                    f"usMaxContext is defined only in OS/2 version 2 and up. Current version is {os_2.version}"
+                )
+                continue
+
+            current = os_2.usMaxContex
+            max_context = font.recalc_max_context()
+            if current == max_context:
+                file_not_changed_message(file)
+                continue
+
+            os_2.usMaxContext = max_context
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            font.save(output_file)
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_os2.command()
+@add_file_or_path_argument()
+@add_common_options()
+def recalc_ranges(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
+    """
+    Generates a temporary Type 1 from the font file using tx, converts that to an OpenType font using makeotf, reads the
+    Unicode ranges and codepage ranges from the temporary OpenType font file, and then writes those ranges to the
+    original font's OS/2 table.
+    """
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            temp_otf_fd, temp_otf_file = font.make_temp_otf()
+            temp_font = Font(temp_otf_file)
+
+            os_2: TableOS2 = font["OS/2"]
+            os_2_temp: TableOS2 = temp_font["OS/2"]
+            current_unicode_ranges = os_2.getUnicodeRanges()
+            current_codepage_ranges = os_2.get_codepage_ranges()
+            new_unicode_ranges = os_2_temp.getUnicodeRanges()
+            new_codepage_ranges = os_2_temp.get_codepage_ranges()
+
+            if current_unicode_ranges != new_unicode_ranges or current_codepage_ranges != new_codepage_ranges:
+                os_2.setUnicodeRanges(bits=new_unicode_ranges)
+                os_2.set_codepage_ranges(codepage_ranges=new_codepage_ranges)
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+            temp_font.close()
+            os.close(temp_otf_fd)
+            os.remove(temp_otf_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_os2.command()
+@add_file_or_path_argument()
+@click.option(
+    "-it/-no-it",
+    "--italic/--no-italic",
+    "italic",
+    default=None,
+    help="Sets or clears the ITALIC bits (`fsSelection` bit 0 and `head` table `macStyle` bit 1).",
+)
+@click.option(
+    "-us/-no-us",
+    "--underscore/--no-underscore",
+    "underscore",
+    default=None,
+    help="""
+Sets or clears `fsType` bit 1 (UNDERSCORE).
+""",
+)
+@click.option(
+    "-ng/-no-ng",
+    "--negative/--no-negative",
+    "negative",
+    default=None,
+    help="""
+Sets or clears `fsType` bit 2 (NEGATIVE).
+""",
+)
+@click.option(
+    "-ol/-no-ol",
+    "--outlined/--no-outlined",
+    "outlined",
+    default=None,
+    help="""
+Sets or clears `fsType` bit 3 (OUTLINED).
+""",
+)
+@click.option(
+    "-st/-no-st",
+    "--strikeout/--no-strikeout",
+    "strikeout",
+    default=None,
+    help="""
+Sets or clears `fsType` bit 4 (STRIKEOUT).
+""",
+)
+@click.option(
+    "-bd/-no-bd",
+    "--bold/--no-bold",
+    "bold",
+    default=None,
+    help="Sets or clears the BOLD bits (`OS/2.fsSelection` bit 5 and `head.macStyle` bit 0).",
+)
+@click.option(
+    "-rg",
+    "--regular",
+    "regular",
+    is_flag=True,
+    default=None,
+    help="""
+Sets REGULAR (`fsSelection` bit 6) and clears BOLD (`fsSelection` bit 5, `head.macStyle` bit 0) and ITALIC
+(`fsSelection` bit 0, `head.macStyle` bit 1) bits. This is equivalent to `--no-bold --no-italic`.
+""",
+)
+@click.option(
+    "-utm/-no-utm",
+    "--use-typo-metrics/--no-use-typo-metrics",
+    "use_typo_metrics",
+    default=None,
+    help="""
+Sets or clears the USE_TYPO_METRICS bit (`fsSelection` bit 7).
+
+If set, it is strongly recommended that applications use `OS/2.sTypoAscender` - `OS/2.sTypoDescender` + 
+`OS/2.sTypoLineGap` as the default line spacing for the font.
+
+See: https://docs.microsoft.com/en-us/typography/opentype/spec/os2#fsselection
+""",
+)
+@click.option(
+    "-wws/-no-wws",
+    "--wws-consistent/--no-wws-consistent",
+    "wws_consistent",
+    default=None,
+    help="""
+Sets or clears the WWS bit (`fsSelection` bit 8).
+
+If the `OS/2.fsSelection` bit is set, the font has `name` table strings consistent with a weight/width/slope family
+without requiring use of name IDs 21 and 22.
+
+See: https://docs.microsoft.com/en-us/typography/opentype/spec/os2#fsselection
+
+Also: https://typedrawers.com/discussion/3857/fontlab-7-windows-reads-exported-font-name-differently
+""",
+)
+@click.option(
+    "-obl/-no-obl",
+    "--oblique/--no-oblique",
+    "oblique",
+    default=None,
+    help="Sets or clears the OBLIQUE bit (`fsSelection` bit 9).",
+)
+@click.option(
+    "-el",
+    "--embed-level",
+    "embed_level",
+    type=click.Choice(["0", "2", "4", "8"]),
+    default=None,
+    help="""
+Sets/clears `fsType` bits 0-3 (EMBEDDING_LEVEL).
+
+Valid fonts must set at most one of bits 1, 2 or 3; bit 0 is permanently reserved and must be zero. Valid values for
+this sub-field are 0, 2, 4 or 8. The meaning of these values is as follows:
+
+\b
+0: Installable embedding
+2: Restricted License embedding
+4: Preview & Print embedding
+8: Editable embedding
+
+See: https://docs.microsoft.com/en-us/typography/opentype/spec/os2#fstype
+""",
+)
+@click.option(
+    "-ns/-as",
+    "--no-subsetting/--allow-subsetting",
+    default=None,
+    help="""
+Sets or clears `fsType` bit 8 (NO_SUBSETTING).
+
+When this bit is set, the font may not be subsetted prior to embedding. Other embedding restrictions specified in bits
+0-3 and 9 also apply.
+""",
+)
+@click.option(
+    "-beo/-no-beo",
+    "--bitmap-embedding-only/--no-bitmap-embedding-only",
+    default=None,
+    help="""
+Sets or clears `fsType` bit 9 (BITMAP_EMBEDDING_ONLY).
+
+When this bit is set, only bitmaps contained in the font may be embedded. No outline data may be embedded. If there are
+no bitmaps available in the font, then the font is considered unembeddable and the embedding services will fail. Other
+embedding restrictions specified in bits 0-3 and 8 also apply.
+""",
+)
+@add_common_options()
+def set_flags(
+    input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True, **kwargs
+):
+    """
+    Sets/clears the following flags in OS/2.fsSelection and OS/2.fsType fields:
+
+    fsSelection:
+
+    \b
+    Bit 0: ITALIC
+    Bit 1: UNDERSCORE
+    Bit 2: NEGATIVE
+    Bit 3: OUTLINED
+    Bit 4: STRIKEOUT
+    Bit 5: BOLD
+    Bit 6: REGULAR
+    Bit 7: USE_TYPO_METRICS
+    Bit 8: WWS
+    Bit 9: OBLIQUE
+
+    fsType:
+
+    \b
+    Bits 0-3: Usage permissions
+    Bit 8: No subsetting
+    Bit 9: Bitmap embedding only
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    options = {k: v for k, v in kwargs.items() if v is not None}
+    if len(options) == 0:
+        generic_error_message("Please, pass at least one valid parameter.")
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            head = font["head"]
+            head_copy = deepcopy(head)
+            os2 = font["OS/2"]
+            os2_copy = deepcopy(os2)
+
+            for flag, value in options.items():
+                if flag in ("use_typo_metrics", "wws_consistent", "oblique") and os2.version < 4:
+                    generic_warning_message(
+                        f"{flag.upper()} flag can't be set. Bits 7, 8 and 9 are only defined in OS/2 version 4 and up."
+                    )
+                    continue
+                if flag == "embed_level":
+                    value = int(value)
+                set_flag = getattr(font, f"set_{flag}_flag")
+                set_flag(value)
+
+            if head_copy.compile(font) != head.compile(font) or os2_copy.compile(font) != os2.compile(font):
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_os2.command()
+@click.option("-v", "target_version", type=click.IntRange(1, 5), required=True, help="Target version")
+@add_file_or_path_argument()
+@add_common_options()
+def set_version(
+    input_path: Path,
+    target_version: int,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Upgrades OS/2 table version.
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            os_2: TableOS2 = font["OS/2"]
+            current_version = getattr(os_2, "version")
+
+            if target_version <= current_version:
+                generic_warning_message(f"Current OS/2 table version is already {current_version}")
+                file_not_changed_message(file)
+                continue
+
+            setattr(os_2, "version", target_version)
+
+            # When upgrading from version 0, ulCodePageRanges are to be recalculated.
+            if current_version < 1:
+                temp_otf_fd, temp_otf_file = font.make_temp_otf()
+                temp_otf_font = Font(temp_otf_file)
+                temp_os_2: TableOS2 = temp_otf_font["OS/2"]
+                os_2.set_codepage_ranges(temp_os_2.get_codepage_ranges())
+
+                temp_otf_font.close()
+                os.close(temp_otf_fd)
+                os.remove(temp_otf_file)
+
+            # Return if upgrading from version 0 to version 1.
+            if target_version == 1:
+                font.save(output_file)
+                file_saved_message(output_file)
+                continue
+
+            # Upgrading from version 1 requires creating sxHeight, sCapHeight, usDefaultChar, usBreakChar and
+            # usMaxContext entries.
+            if current_version < 2:
+                os_2.set_x_height(font.recalc_x_height())
+                os_2.set_cap_height(font.recalc_cap_height())
+                os_2.set_default_char(0)
+                os_2.set_break_char(32)
+                os_2.set_max_context(font.recalc_max_context())
+
+            # Write default values if target_version == 5.
+            if target_version > 4:
+                setattr(os_2, "usLowerOpticalPointSize", 0)
+                setattr(os_2, "usUpperOpticalPointSize", 65535 / 20)
+
+            # Finally, make sure to clear bits 7, 8 and 9 in ['OS/2'].fsSelection when target version is lower than 4.
+            if target_version < 4:
+                for b in (7, 8, 9):
+                    setattr(os_2, "fsSelection", unset_nth_bit(os_2.fsSelection, b))
+
+            font.save(output_file)
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_os2.command()
+@add_file_or_path_argument()
+@click.option("-w", "--weight", type=click.IntRange(1, 1000), required=True, help="usWeightClass value.")
+@add_common_options()
+def set_weight(
+    input_path: Path, weight: int, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
+):
+    """
+    Sets the Weight class value.
+
+    usWeightClass indicates the visual weight (degree of blackness or thickness of strokes) of the characters in the
+    font. Values from 1 to 1000 are valid.
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            os_2: TableOS2 = font["OS/2"]
+
+            if weight == os_2.get_weight_class():
+                file_not_changed_message(file)
+                continue
+
+            os_2.set_weight_class(weight)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            font.save(output_file)
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@tbl_os2.command()
+@add_file_or_path_argument()
+@click.option("-w", "--width", type=click.IntRange(1, 9), required=True, help="usWidthClass value.")
+@add_common_options()
+def set_width(
+    input_path: Path, width: int, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True
+):
+    """
+    Sets the Width class value.
+
+    usWidthClass indicates a relative change from the normal aspect ratio (width to height ratio) as specified by a font
+    designer for the glyphs in a font. Values from 1 to 9 are valid.
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            os_2: TableOS2 = font["OS/2"]
+
+            if width == os_2.get_width_class():
+                file_not_changed_message(file)
+                continue
+
+            os_2.set_width_class(width)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            font.save(output_file)
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+cli = click.CommandCollection(
+    sources=[tbl_os2],
+    help="""
+    A set of tools to manipulate the 'OS/2' table.
+    """,
+)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_otf.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_otf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,490 +1,489 @@
-import time
-from copy import deepcopy
-from pathlib import Path
-
-import click
-from fontTools.misc.cliTools import makeOutputFileName
-
-from foundryToolsCLI.Lib.Font import Font
-from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
-from foundryToolsCLI.Lib.utils.click_tools import (
-    add_file_or_path_argument,
-    add_common_options,
-    file_saved_message,
-    generic_error_message,
-    generic_info_message,
-    file_not_changed_message,
-)
-
-CWD = Path.cwd()
-otf_tools = click.Group("subcommands")
-
-
-@otf_tools.command()
-@add_file_or_path_argument()
-@click.option(
-    "--optimize/--no-optimize",
-    default=True,
-    help="""
-    Optimize the hinted font by specializing the charstrings and applying subroutines.
-    """,
-)
-@click.option(
-    "-r",
-    "--reference-font",
-    type=click.Path(exists=True, dir_okay=False, resolve_path=True),
-    help="""
-    Reference font.
-
-    Font to be used as reference, when hinting multiple fonts compatibility.
-    """,
-)
-@click.option(
-    "-c",
-    "--allow-changes",
-    is_flag=True,
-    help="""
-    Allow changes to the glyph outlines.
-
-    Paths are reordered to reduce hint substitution, and nearly straight curves
-    are flattened.
-    """,
-)
-@click.option(
-    "-d",
-    "--decimal",
-    is_flag=True,
-    help="""
-    Use decimal coordinates.
-    """,
-)
-@click.option(
-    "-nf",
-    "--no-flex",
-    is_flag=True,
-    help="""
-    Suppress generation of flex commands.
-    """,
-)
-@click.option(
-    "-ns",
-    "--no-hint-sub",
-    is_flag=True,
-    help="""
-    Suppress hint substitution.
-    """,
-)
-@click.option(
-    "-nz",
-    "--no-zones-stems",
-    is_flag=True,
-    help="""
-    Allow the font to have no alignment zones nor stem widths.
-    """,
-)
-@add_common_options()
-def autohint(
-    input_path: Path,
-    reference_font: Path = None,
-    allow_changes: bool = False,
-    decimal: bool = False,
-    no_flex: bool = False,
-    no_hint_sub: bool = False,
-    no_zones_stems: bool = False,
-    optimize: bool = True,
-    output_dir: bool = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Auto-hint OTF and PostScript flavored WOFF/WOFF2 fonts.
-    """
-    from fontTools.cffLib.specializer import specializeProgram
-    from psautohint.autohint import ACOptions, hintFiles
-
-    fonts = get_fonts_in_path(
-        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False, allow_variable=False
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for count, font in enumerate(fonts, start=1):
-        t = time.time()
-        print()
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            temp_otf_file = Path(makeOutputFileName(output_file, extension=".otf", suffix="_tmp", overWrite=True))
-
-            generic_info_message(f"Auto-hinting file {count} of {len(fonts)}: {file.relative_to(CWD)} ")
-            original_timestamp = font.modified_timestamp
-
-            flavor = font.flavor
-            if flavor:
-                font.flavor = None
-                font.save(temp_otf_file)
-                input_file = temp_otf_file
-            else:
-                input_file = file
-
-            font.close()
-
-            options = ACOptions()
-            options.inputPaths = [input_file]
-            options.outputPaths = [output_file]
-            options.reference_font = reference_font
-            options.allowChanges = allow_changes
-            options.round_coords = decimal
-            options.noFlex = no_flex
-            options.noHintSub = no_hint_sub
-            options.allow_no_blues = no_zones_stems
-
-            try:
-                hintFiles(options=options)
-            except Exception as e:
-                generic_error_message(e)
-                continue
-
-            hinted_font = Font(output_file, recalcTimestamp=recalc_timestamp)
-
-            if not recalc_timestamp:
-                hinted_font.set_modified_timestamp(original_timestamp)
-
-            if optimize:
-                generic_info_message("Performing charstrings optimization")
-                top_dict = hinted_font["CFF "].cff.topDictIndex[0]
-                charstrings = top_dict.CharStrings
-                for charstring in charstrings.values():
-                    charstring.decompile()
-                    charstring.program = specializeProgram(charstring.program)
-
-                generic_info_message("Applying subroutines")
-                hinted_font.otf_subroutinize()
-
-            hinted_font.flavor = flavor
-
-            hinted_font.save(output_file)
-            hinted_font.close()
-            temp_otf_file.unlink(missing_ok=True)
-            generic_info_message(f"Done in {round(time.time() - t, 3)}")
-            file_saved_message(output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-
-
-@otf_tools.command()
-@add_file_or_path_argument()
-@click.option(
-    "--no-subr",
-    "subroutinize",
-    is_flag=True,
-    default=True,
-    help="""
-    Do not subroutinize dehinted fonts.
-    """,
-)
-@click.option(
-    "-d",
-    "--dehinter",
-    type=click.Choice(choices=("tx", "fonttools")),
-    default="tx",
-    show_default=True,
-    help="""
-    Use tx (default) or fontTools to remove hints.
-
-    tx creates a temporary .cff file (tx -cff) removing hints (-n), preserving the glyph order (+d) and applying
-    subroutines (+S). Then the .cff file is merged to the destination file using sfntedit, as explained here:
-    https://github.com/adobe-type-tools/afdko/wiki/How-To#how-to-remove-hints-from-a-cff-based-otf. Finally, the
-    temporary .cff file is deleted.
-
-    fontTools uses the subset.cff.remove_hints() method to remove hints, and the font is subroutinized with cffsubr
-    (subroutinization can be deactivated passing the --no-subr parameter).
-
-    fontTools drops font-wide hinting values from the Private dict, while tx preserves them.
-    """,
-)
-@add_common_options()
-def dehint(
-    input_path: Path,
-    dehinter: str = "tx",
-    subroutinize: bool = True,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Remove hints from CFF flavored (OTF, WOFF, WOFF2) fonts.
-    """
-    from afdko.fdkutils import run_shell_command
-
-    fonts = get_fonts_in_path(input_path=input_path, allow_ttf=False, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        # Using fontTools.subset.cff.remove_hints()
-        if dehinter == "fonttools":
-            try:
-                font.otf_dehint()
-                if subroutinize:
-                    font.otf_subroutinize()
-
-                file = Path(font.reader.file.name)
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            except Exception as e:
-                generic_error_message(e)
-            font.close()
-            continue
-
-        # Using tx -cff -n +b +/-S and then sfntedit -a to merge the CFF table to the destination file
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            temp_cff_file = Path(makeOutputFileName(output_file, extension=".cff", overWrite=True))
-            temp_otf_file = Path(makeOutputFileName(output_file, extension=".otf", suffix="_tmp", overWrite=True))
-
-            # If the font is WOFF or WOFF2, we need to convert to a temporary OTF font
-            flavor = font.flavor
-            if flavor:
-                font.flavor = None
-                font.save(temp_otf_file, reorderTables=False)
-                font.close()
-                input_file = temp_otf_file
-            else:
-                input_file = file
-
-            tx_command = ["tx", "-cff", "-n", "+b"]
-            if subroutinize:
-                tx_command.append("+S")
-            else:
-                tx_command.append("-S")
-            tx_command.extend([input_file, temp_cff_file])
-            run_shell_command(tx_command, suppress_output=True)
-
-            sfntedit_command = ["sfntedit", "-a", f"CFF={temp_cff_file}", input_file]
-            if output_file != input_file:
-                sfntedit_command.append(output_file)
-            run_shell_command(sfntedit_command, suppress_output=True)
-
-            # Convert the font back to WOFF/WOFF2
-            if flavor:
-                font = Font(output_file, recalcTimestamp=recalc_timestamp)
-                font.flavor = flavor
-                font.save(output_file)
-                font.close()
-
-            file_saved_message(output_file.relative_to(CWD))
-            temp_cff_file.unlink()
-            temp_otf_file.unlink(missing_ok=True)
-
-        except Exception as e:
-            generic_error_message(e)
-
-
-@otf_tools.command()
-@add_file_or_path_argument()
-@click.option(
-    "--min-area",
-    type=int,
-    default=25,
-    help="""
-    Minimum area for a tiny outline.
-    
-    Default is 25 square units. Subpaths with a bounding box less than this will be reported and deleted.
-    """,
-)
-@click.option("--no-subr", "subroutinize", is_flag=True, default=True, help="""Do not subroutinize fixed fonts.""")
-@click.option("--silent", "verbose", is_flag=True, default=True, help="Run in silent mode")
-@add_common_options()
-def fix_contours(
-    input_path: Path,
-    min_area: int = 25,
-    subroutinize: bool = True,
-    verbose: bool = True,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Fix contours by correcting contours direction, removing overlaps and tiny paths.
-    """
-    fonts = get_fonts_in_path(
-        input_path=input_path, allow_variable=False, allow_ttf=False, recalc_timestamp=recalc_timestamp
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        print()
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            generic_info_message(f"Checking file {file.name}")
-            font.otf_fix_contours(min_area=min_area, verbose=verbose)
-            if subroutinize:
-                font.otf_subroutinize()
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@otf_tools.command()
-@add_file_or_path_argument()
-@add_common_options()
-def fix_version(input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True):
-    """
-    Aligns CFF topDict version string to the head.fontRevision value.
-
-    For example, if head.fontRevision value is 2.001, CFF topDict version value will be 2.1.
-    """
-    fonts = get_fonts_in_path(
-        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False, allow_variable=False
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            cff_table = font["CFF "]
-            cff_table_copy = deepcopy(cff_table)
-
-            font.fix_cff_top_dict_version()
-
-            if cff_table_copy.compile(font) != cff_table.compile(font):
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@otf_tools.command()
-@add_file_or_path_argument()
-@add_common_options()
-def subr(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
-    """
-    Subroutinize OpenType-PS fonts.
-    """
-    fonts = get_fonts_in_path(input_path=input_path, allow_ttf=False, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            font.otf_subroutinize()
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@otf_tools.command()
-@add_file_or_path_argument()
-@add_common_options()
-def desubr(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
-    """
-    Desubroutinize OpenType-PS fonts.
-    """
-    fonts = get_fonts_in_path(input_path=input_path, allow_ttf=False, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            font.otf_desubroutinize()
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@otf_tools.command()
-@add_file_or_path_argument()
-@click.option("-q", "--quiet-mode", is_flag=True, help="Run in quiet mode.")
-@add_common_options()
-def check_outlines(
-    input_path: Path,
-    quiet_mode: bool = False,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Performs outline quality checks and overlaps removal with checkoutlinesufo.
-    """
-
-    from afdko import checkoutlinesufo
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        print()
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-
-            generic_info_message(f"Checking file {file.name}")
-
-            flavor = font.flavor
-            if flavor:
-                font.flavor = None
-                font.save(output_file)
-
-            if not file == output_file:
-                font.save(output_file)
-
-            font.close()
-
-            args = [output_file.as_posix(), "--error-correction-mode"]
-            if quiet_mode:
-                args.append("--quiet-mode")
-            checkoutlinesufo.run(args=args)
-
-            if flavor:
-                font = Font(output_file, recalcTimestamp=recalc_timestamp)
-                font.flavor = flavor
-                font.save(output_file)
-
-            file_saved_message(output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-cli = click.CommandCollection(
-    sources=[otf_tools],
-    help="""
-    A set of tools to manipulate fonts with PostScript outlines.
-    """,
-)
+import time
+from copy import deepcopy
+from pathlib import Path
+
+import click
+from fontTools.misc.cliTools import makeOutputFileName
+
+from foundryToolsCLI.Lib.Font import Font
+from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
+from foundryToolsCLI.Lib.utils.click_tools import (
+    add_file_or_path_argument,
+    add_common_options,
+    file_saved_message,
+    generic_error_message,
+    generic_info_message,
+    file_not_changed_message,
+)
+
+otf_tools = click.Group("subcommands")
+
+
+@otf_tools.command()
+@add_file_or_path_argument()
+@click.option(
+    "--optimize/--no-optimize",
+    default=True,
+    help="""
+    Optimize the hinted font by specializing the charstrings and applying subroutines.
+    """,
+)
+@click.option(
+    "-r",
+    "--reference-font",
+    type=click.Path(exists=True, dir_okay=False, resolve_path=True),
+    help="""
+    Reference font.
+
+    Font to be used as reference, when hinting multiple fonts compatibility.
+    """,
+)
+@click.option(
+    "-c",
+    "--allow-changes",
+    is_flag=True,
+    help="""
+    Allow changes to the glyph outlines.
+
+    Paths are reordered to reduce hint substitution, and nearly straight curves
+    are flattened.
+    """,
+)
+@click.option(
+    "-d",
+    "--decimal",
+    is_flag=True,
+    help="""
+    Use decimal coordinates.
+    """,
+)
+@click.option(
+    "-nf",
+    "--no-flex",
+    is_flag=True,
+    help="""
+    Suppress generation of flex commands.
+    """,
+)
+@click.option(
+    "-ns",
+    "--no-hint-sub",
+    is_flag=True,
+    help="""
+    Suppress hint substitution.
+    """,
+)
+@click.option(
+    "-nz",
+    "--no-zones-stems",
+    is_flag=True,
+    help="""
+    Allow the font to have no alignment zones nor stem widths.
+    """,
+)
+@add_common_options()
+def autohint(
+    input_path: Path,
+    reference_font: Path = None,
+    allow_changes: bool = False,
+    decimal: bool = False,
+    no_flex: bool = False,
+    no_hint_sub: bool = False,
+    no_zones_stems: bool = False,
+    optimize: bool = True,
+    output_dir: bool = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Auto-hint OTF and PostScript flavored WOFF/WOFF2 fonts.
+    """
+    from fontTools.cffLib.specializer import specializeProgram
+    from psautohint.autohint import ACOptions, hintFiles
+
+    fonts = get_fonts_in_path(
+        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False, allow_variable=False
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for count, font in enumerate(fonts, start=1):
+        t = time.time()
+        print()
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            temp_otf_file = Path(makeOutputFileName(output_file, extension=".otf", suffix="_tmp", overWrite=True))
+
+            generic_info_message(f"Auto-hinting file {count} of {len(fonts)}: {file.name} ")
+            original_timestamp = font.modified_timestamp
+
+            flavor = font.flavor
+            if flavor:
+                font.flavor = None
+                font.save(temp_otf_file)
+                input_file = temp_otf_file
+            else:
+                input_file = file
+
+            font.close()
+
+            options = ACOptions()
+            options.inputPaths = [input_file]
+            options.outputPaths = [output_file]
+            options.reference_font = reference_font
+            options.allowChanges = allow_changes
+            options.round_coords = decimal
+            options.noFlex = no_flex
+            options.noHintSub = no_hint_sub
+            options.allow_no_blues = no_zones_stems
+
+            try:
+                hintFiles(options=options)
+            except Exception as e:
+                generic_error_message(e)
+                continue
+
+            hinted_font = Font(output_file, recalcTimestamp=recalc_timestamp)
+
+            if not recalc_timestamp:
+                hinted_font.set_modified_timestamp(original_timestamp)
+
+            if optimize:
+                generic_info_message("Performing charstrings optimization")
+                top_dict = hinted_font["CFF "].cff.topDictIndex[0]
+                charstrings = top_dict.CharStrings
+                for charstring in charstrings.values():
+                    charstring.decompile()
+                    charstring.program = specializeProgram(charstring.program)
+
+                generic_info_message("Applying subroutines")
+                hinted_font.otf_subroutinize()
+
+            hinted_font.flavor = flavor
+
+            hinted_font.save(output_file)
+            hinted_font.close()
+            temp_otf_file.unlink(missing_ok=True)
+            generic_info_message(f"Done in {round(time.time() - t, 3)}")
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+
+
+@otf_tools.command()
+@add_file_or_path_argument()
+@click.option(
+    "--no-subr",
+    "subroutinize",
+    is_flag=True,
+    default=True,
+    help="""
+    Do not subroutinize dehinted fonts.
+    """,
+)
+@click.option(
+    "-d",
+    "--dehinter",
+    type=click.Choice(choices=("tx", "fonttools")),
+    default="tx",
+    show_default=True,
+    help="""
+    Use tx (default) or fontTools to remove hints.
+
+    tx creates a temporary .cff file (tx -cff) removing hints (-n), preserving the glyph order (+d) and applying
+    subroutines (+S). Then the .cff file is merged to the destination file using sfntedit, as explained here:
+    https://github.com/adobe-type-tools/afdko/wiki/How-To#how-to-remove-hints-from-a-cff-based-otf. Finally, the
+    temporary .cff file is deleted.
+
+    fontTools uses the subset.cff.remove_hints() method to remove hints, and the font is subroutinized with cffsubr
+    (subroutinization can be deactivated passing the --no-subr parameter).
+
+    fontTools drops font-wide hinting values from the Private dict, while tx preserves them.
+    """,
+)
+@add_common_options()
+def dehint(
+    input_path: Path,
+    dehinter: str = "tx",
+    subroutinize: bool = True,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Remove hints from CFF flavored (OTF, WOFF, WOFF2) fonts.
+    """
+    from afdko.fdkutils import run_shell_command
+
+    fonts = get_fonts_in_path(input_path=input_path, allow_ttf=False, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        # Using fontTools.subset.cff.remove_hints()
+        if dehinter == "fonttools":
+            try:
+                font.otf_dehint()
+                if subroutinize:
+                    font.otf_subroutinize()
+
+                file = Path(font.reader.file.name)
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            except Exception as e:
+                generic_error_message(e)
+            font.close()
+            continue
+
+        # Using tx -cff -n +b +/-S and then sfntedit -a to merge the CFF table to the destination file
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            temp_cff_file = Path(makeOutputFileName(output_file, extension=".cff", overWrite=True))
+            temp_otf_file = Path(makeOutputFileName(output_file, extension=".otf", suffix="_tmp", overWrite=True))
+
+            # If the font is WOFF or WOFF2, we need to convert to a temporary OTF font
+            flavor = font.flavor
+            if flavor:
+                font.flavor = None
+                font.save(temp_otf_file, reorderTables=False)
+                font.close()
+                input_file = temp_otf_file
+            else:
+                input_file = file
+
+            tx_command = ["tx", "-cff", "-n", "+b"]
+            if subroutinize:
+                tx_command.append("+S")
+            else:
+                tx_command.append("-S")
+            tx_command.extend([input_file, temp_cff_file])
+            run_shell_command(tx_command, suppress_output=True)
+
+            sfntedit_command = ["sfntedit", "-a", f"CFF={temp_cff_file}", input_file]
+            if output_file != input_file:
+                sfntedit_command.append(output_file)
+            run_shell_command(sfntedit_command, suppress_output=True)
+
+            # Convert the font back to WOFF/WOFF2
+            if flavor:
+                font = Font(output_file, recalcTimestamp=recalc_timestamp)
+                font.flavor = flavor
+                font.save(output_file)
+                font.close()
+
+            file_saved_message(output_file)
+            temp_cff_file.unlink()
+            temp_otf_file.unlink(missing_ok=True)
+
+        except Exception as e:
+            generic_error_message(e)
+
+
+@otf_tools.command()
+@add_file_or_path_argument()
+@click.option(
+    "--min-area",
+    type=int,
+    default=25,
+    help="""
+    Minimum area for a tiny outline.
+    
+    Default is 25 square units. Subpaths with a bounding box less than this will be reported and deleted.
+    """,
+)
+@click.option("--no-subr", "subroutinize", is_flag=True, default=True, help="""Do not subroutinize fixed fonts.""")
+@click.option("--silent", "verbose", is_flag=True, default=True, help="Run in silent mode")
+@add_common_options()
+def fix_contours(
+    input_path: Path,
+    min_area: int = 25,
+    subroutinize: bool = True,
+    verbose: bool = True,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Fix contours by correcting contours direction, removing overlaps and tiny paths.
+    """
+    fonts = get_fonts_in_path(
+        input_path=input_path, allow_variable=False, allow_ttf=False, recalc_timestamp=recalc_timestamp
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        print()
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            generic_info_message(f"Checking file {file.name}")
+            font.otf_fix_contours(min_area=min_area, verbose=verbose)
+            if subroutinize:
+                font.otf_subroutinize()
+            font.save(output_file)
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@otf_tools.command()
+@add_file_or_path_argument()
+@add_common_options()
+def fix_version(input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True):
+    """
+    Aligns CFF topDict version string to the head.fontRevision value.
+
+    For example, if head.fontRevision value is 2.001, CFF topDict version value will be 2.1.
+    """
+    fonts = get_fonts_in_path(
+        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False, allow_variable=False
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            cff_table = font["CFF "]
+            cff_table_copy = deepcopy(cff_table)
+
+            font.fix_cff_top_dict_version()
+
+            if cff_table_copy.compile(font) != cff_table.compile(font):
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@otf_tools.command()
+@add_file_or_path_argument()
+@add_common_options()
+def subr(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
+    """
+    Subroutinize OpenType-PS fonts.
+    """
+    fonts = get_fonts_in_path(input_path=input_path, allow_ttf=False, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            font.otf_subroutinize()
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            font.save(output_file)
+            file_saved_message(output_file)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@otf_tools.command()
+@add_file_or_path_argument()
+@add_common_options()
+def desubr(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
+    """
+    Desubroutinize OpenType-PS fonts.
+    """
+    fonts = get_fonts_in_path(input_path=input_path, allow_ttf=False, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            font.otf_desubroutinize()
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            font.save(output_file)
+            file_saved_message(output_file)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@otf_tools.command()
+@add_file_or_path_argument()
+@click.option("-q", "--quiet-mode", is_flag=True, help="Run in quiet mode.")
+@add_common_options()
+def check_outlines(
+    input_path: Path,
+    quiet_mode: bool = False,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Performs outline quality checks and overlaps removal with checkoutlinesufo.
+    """
+
+    from afdko import checkoutlinesufo
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp, allow_ttf=False)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        print()
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            generic_info_message(f"Checking file {file.name}")
+
+            flavor = font.flavor
+            if flavor:
+                font.flavor = None
+                font.save(output_file)
+
+            if not file == output_file:
+                font.save(output_file)
+
+            font.close()
+
+            args = [output_file.as_posix(), "--error-correction-mode"]
+            if quiet_mode:
+                args.append("--quiet-mode")
+            checkoutlinesufo.run(args=args)
+
+            if flavor:
+                font = Font(output_file, recalcTimestamp=recalc_timestamp)
+                font.flavor = flavor
+                font.save(output_file)
+
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+cli = click.CommandCollection(
+    sources=[otf_tools],
+    help="""
+    A set of tools to manipulate fonts with PostScript outlines.
+    """,
+)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_post.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_post.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,105 +1,103 @@
-from copy import copy
-from pathlib import Path
-
-import click
-from fontTools.misc.cliTools import makeOutputFileName
-
-from foundryToolsCLI.Lib.tables.post import TablePost
-from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
-from foundryToolsCLI.Lib.utils.click_tools import (
-    add_file_or_path_argument,
-    add_common_options,
-    file_saved_message,
-    file_not_changed_message,
-    generic_error_message,
-)
-
-CWD = Path.cwd()
-
-
-@click.command()
-@add_file_or_path_argument()
-@click.option(
-    "--italic-angle",
-    type=click.FloatRange(-90.0, 90.0),
-    help="""Sets the `italicAngle` value.""",
-)
-@click.option(
-    "--ul-position",
-    type=int,
-    help="""Sets the `underlinePosition` value.""",
-)
-@click.option(
-    "--ul-thickness",
-    type=int,
-    help="""Sets the `underlineThickness` value.""",
-)
-@click.option(
-    "--fixed-pitch/--no-fixed-pitch",
-    default=None,
-    help="""Sets or clears the `isFixedPitch` value.""",
-)
-@add_common_options()
-def cli(input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = None, **kwargs):
-    """A command line tool to manipulate the 'post' table."""
-
-    params = {k: v for k, v in kwargs.items() if v is not None}
-
-    if len(params) == 0:
-        generic_error_message("Please, pass at least a valid parameter.")
-        return
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-
-            post_table: TablePost = font["post"]
-            post_table_copy = copy(post_table)
-            if font.is_otf:
-                cff_table = font["CFF "]
-                cff_table_copy = copy(cff_table)
-            else:
-                cff_table = cff_table_copy = None
-
-            # Process the arguments
-            if "italic_angle" in params.keys():
-                post_table.set_italic_angle(params.get("italic_angle"))
-                if font.is_otf:
-                    font["CFF "].cff.topDictIndex[0].ItalicAngle = int(params.get("italic_angle"))
-
-            if "ul_position" in params.keys():
-                post_table.set_underline_position(params.get("ul_position"))
-
-            if "ul_thickness" in params.keys():
-                post_table.set_underline_thickness(params.get("ul_thickness"))
-
-            if "fixed_pitch" in params.keys():
-                post_table.set_fixed_pitch(params.get("fixed_pitch"))
-
-            # Check if tables have changed before saving the font. No need to compile here.
-            if post_table_copy.compile(font) != post_table.compile(font):
-                post_table_modified = True
-            else:
-                post_table_modified = False
-
-            if font.is_otf and (cff_table_copy.compile(font) != cff_table.compile(font)):
-                cff_table_modified = True
-            else:
-                cff_table_modified = False
-
-            if post_table_modified or cff_table_modified:
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
+from copy import copy
+from pathlib import Path
+
+import click
+from fontTools.misc.cliTools import makeOutputFileName
+
+from foundryToolsCLI.Lib.tables.post import TablePost
+from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
+from foundryToolsCLI.Lib.utils.click_tools import (
+    add_file_or_path_argument,
+    add_common_options,
+    file_saved_message,
+    file_not_changed_message,
+    generic_error_message,
+)
+
+
+@click.command()
+@add_file_or_path_argument()
+@click.option(
+    "--italic-angle",
+    type=click.FloatRange(-90.0, 90.0),
+    help="""Sets the `italicAngle` value.""",
+)
+@click.option(
+    "--ul-position",
+    type=int,
+    help="""Sets the `underlinePosition` value.""",
+)
+@click.option(
+    "--ul-thickness",
+    type=int,
+    help="""Sets the `underlineThickness` value.""",
+)
+@click.option(
+    "--fixed-pitch/--no-fixed-pitch",
+    default=None,
+    help="""Sets or clears the `isFixedPitch` value.""",
+)
+@add_common_options()
+def cli(input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = None, **kwargs):
+    """A command line tool to manipulate the 'post' table."""
+
+    params = {k: v for k, v in kwargs.items() if v is not None}
+
+    if len(params) == 0:
+        generic_error_message("Please, pass at least a valid parameter.")
+        return
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            post_table: TablePost = font["post"]
+            post_table_copy = copy(post_table)
+            if font.is_otf:
+                cff_table = font["CFF "]
+                cff_table_copy = copy(cff_table)
+            else:
+                cff_table = cff_table_copy = None
+
+            # Process the arguments
+            if "italic_angle" in params.keys():
+                post_table.set_italic_angle(params.get("italic_angle"))
+                if font.is_otf:
+                    font["CFF "].cff.topDictIndex[0].ItalicAngle = int(params.get("italic_angle"))
+
+            if "ul_position" in params.keys():
+                post_table.set_underline_position(params.get("ul_position"))
+
+            if "ul_thickness" in params.keys():
+                post_table.set_underline_thickness(params.get("ul_thickness"))
+
+            if "fixed_pitch" in params.keys():
+                post_table.set_fixed_pitch(params.get("fixed_pitch"))
+
+            # Check if tables have changed before saving the font. No need to compile here.
+            if post_table_copy.compile(font) != post_table.compile(font):
+                post_table_modified = True
+            else:
+                post_table_modified = False
+
+            if font.is_otf and (cff_table_copy.compile(font) != cff_table.compile(font)):
+                cff_table_modified = True
+            else:
+                cff_table_modified = False
+
+            if post_table_modified or cff_table_modified:
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_print.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_print.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-from pathlib import Path
-
-import click
-
-from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_variable_fonts_in_path
-from foundryToolsCLI.Lib.utils.click_tools import generic_error_message, add_file_or_path_argument
-
-ftcli_printer = click.Group("subcommands")
-
-
-@ftcli_printer.command()
-@add_file_or_path_argument()
-def font_info(input_path: Path):
-    """
-    Prints detailed font info.
-    """
-    from foundryToolsCLI.Lib.printer.UI import print_font_info
-
-    fonts = get_fonts_in_path(input_path=input_path)
-    for font in fonts:
-        try:
-            print_font_info(font)
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@ftcli_printer.command()
-@add_file_or_path_argument()
-@click.option(
-    "-ml",
-    "--max-lines",
-    type=click.INT,
-    default=None,
-    help="Maximum number of lines to be printed for each NameRecord",
-)
-@click.option(
-    "-m",
-    "--minimal",
-    is_flag=True,
-    help="""
-    Prints a minimal set of NameRecords, omitting the ones with nameID not in 1, 2, 3, 4, 5, 6, 16, 17, 18, 21, 22, 25
-    """,
-)
-def font_names(input_path: Path, max_lines: int = None, minimal: bool = False):
-    """
-    Prints the 'name' table and, if the font is CFF, the names in the 'CFF' table topDict.
-    """
-    from foundryToolsCLI.Lib.printer.UI import print_font_names
-
-    fonts = get_fonts_in_path(input_path=input_path)
-    for font in fonts:
-        try:
-            print_font_names(font, max_lines=max_lines, minimal=minimal)
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@ftcli_printer.command()
-@add_file_or_path_argument()
-def fonts_list(input_path: Path):
-    """
-    Prints a list of fonts with basic information.
-    """
-    from foundryToolsCLI.Lib.printer.UI import print_fonts_list
-
-    fonts = get_fonts_in_path(input_path=input_path)
-    print_fonts_list(fonts=fonts)
-
-
-@ftcli_printer.command()
-@add_file_or_path_argument()
-def tbl_os2(input_path: Path):
-    """
-    Prints the OS/2 table.
-    """
-    from foundryToolsCLI.Lib.printer.UI import print_os2_table
-
-    fonts = get_fonts_in_path(input_path=input_path)
-    for font in fonts:
-        try:
-            print_os2_table(font)
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@ftcli_printer.command()
-@add_file_or_path_argument()
-def vf_instances(input_path: Path):
-    """
-    Prints a table of the named instances of a variable font.
-    """
-    from foundryToolsCLI.Lib.printer.UI import print_instances
-
-    variable_fonts = get_variable_fonts_in_path(input_path)
-    for variable_font in variable_fonts:
-        try:
-            print_instances(variable_font)
-            variable_font.close()
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            variable_font.close()
-
-
-cli = click.CommandCollection(
-    sources=[ftcli_printer],
-    help="""
-    Prints various fonts information and tables.
-    """,
-)
+from pathlib import Path
+
+import click
+
+from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_variable_fonts_in_path
+from foundryToolsCLI.Lib.utils.click_tools import generic_error_message, add_file_or_path_argument
+
+ftcli_printer = click.Group("subcommands")
+
+
+@ftcli_printer.command()
+@add_file_or_path_argument()
+def font_info(input_path: Path):
+    """
+    Prints detailed font info.
+    """
+    from foundryToolsCLI.Lib.printer.UI import print_font_info
+
+    fonts = get_fonts_in_path(input_path=input_path)
+    for font in fonts:
+        try:
+            print_font_info(font)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@ftcli_printer.command()
+@add_file_or_path_argument()
+@click.option(
+    "-ml",
+    "--max-lines",
+    type=click.INT,
+    default=None,
+    help="Maximum number of lines to be printed for each NameRecord",
+)
+@click.option(
+    "-m",
+    "--minimal",
+    is_flag=True,
+    help="""
+    Prints a minimal set of NameRecords, omitting the ones with nameID not in 1, 2, 3, 4, 5, 6, 16, 17, 18, 21, 22, 25
+    """,
+)
+def font_names(input_path: Path, max_lines: int = None, minimal: bool = False):
+    """
+    Prints the 'name' table and, if the font is CFF, the names in the 'CFF' table topDict.
+    """
+    from foundryToolsCLI.Lib.printer.UI import print_font_names
+
+    fonts = get_fonts_in_path(input_path=input_path)
+    for font in fonts:
+        try:
+            print_font_names(font, max_lines=max_lines, minimal=minimal)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@ftcli_printer.command()
+@add_file_or_path_argument()
+def fonts_list(input_path: Path):
+    """
+    Prints a list of fonts with basic information.
+    """
+    from foundryToolsCLI.Lib.printer.UI import print_fonts_list
+
+    fonts = get_fonts_in_path(input_path=input_path)
+    print_fonts_list(fonts=fonts)
+
+
+@ftcli_printer.command()
+@add_file_or_path_argument()
+def tbl_os2(input_path: Path):
+    """
+    Prints the OS/2 table.
+    """
+    from foundryToolsCLI.Lib.printer.UI import print_os2_table
+
+    fonts = get_fonts_in_path(input_path=input_path)
+    for font in fonts:
+        try:
+            print_os2_table(font)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@ftcli_printer.command()
+@add_file_or_path_argument()
+def vf_instances(input_path: Path):
+    """
+    Prints a table of the named instances of a variable font.
+    """
+    from foundryToolsCLI.Lib.printer.UI import print_instances
+
+    variable_fonts = get_variable_fonts_in_path(input_path)
+    for variable_font in variable_fonts:
+        try:
+            print_instances(variable_font)
+            variable_font.close()
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            variable_font.close()
+
+
+cli = click.CommandCollection(
+    sources=[ftcli_printer],
+    help="""
+    Prints various fonts information and tables.
+    """,
+)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_ttf.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_ttf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,303 +1,348 @@
-from io import BytesIO
-from pathlib import Path
-
-import click
-from fontTools.misc.cliTools import makeOutputFileName
-
-from foundryToolsCLI.Lib.Font import Font
-from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
-from foundryToolsCLI.Lib.utils.click_tools import (
-    add_file_or_path_argument,
-    add_common_options,
-    file_not_changed_message,
-    file_saved_message,
-    generic_error_message,
-    generic_info_message,
-)
-
-CWD = Path.cwd()
-ttf_tools = click.Group("subcommands")
-
-
-@ttf_tools.command()
-@add_file_or_path_argument()
-@add_common_options()
-def autohint(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
-    """
-    Autohint TrueType fonts using ttfautohint-py.
-    """
-
-    from ttfautohint import ttfautohint
-
-    fonts = get_fonts_in_path(input_path, recalc_timestamp=recalc_timestamp, allow_cff=False, allow_variable=False)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            buf = BytesIO()
-            font.save(buf)
-            data = ttfautohint(in_buffer=buf.getvalue(), no_info=True)
-            hinted_font = Font(BytesIO(data))
-            file = Path(font.reader.file.name)
-            if not recalc_timestamp:
-                hinted_font.set_modified_timestamp(font.modified_timestamp)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            hinted_font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@ttf_tools.command()
-@add_file_or_path_argument()
-@add_common_options()
-def decompose(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
-    """
-    Decompose composite glyphs of a TrueType font.
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp, allow_cff=False)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            font.ttf_decomponentize()
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@ttf_tools.command()
-@add_file_or_path_argument()
-@add_common_options()
-def dehint(input_path: Path, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True):
-    """
-    Drops hinting from TrueType fonts.
-
-    This is a CLI for dehinter by Source Foundry: https://github.com/source-foundry/dehinter
-    """
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp, allow_cff=False)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            font.ttf_dehint()
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@ttf_tools.command()
-@add_file_or_path_argument()
-@click.option(
-    "--min-area",
-    type=int,
-    default=25,
-    help="""
-        Minimum area for a tiny outline.
-
-        Default is 25 square units. Subpaths with a bounding box less than this will be reported and deleted.
-    """,
-)
-@click.option("--keep-hinting", "remove_hinting", is_flag=True, default=True, help="""Do not remove hinting.""")
-@click.option("--silent", "verbose", is_flag=True, default=True, help="Run in silent mode")
-@add_common_options()
-def fix_contours(
-    input_path: Path,
-    min_area: int = 25,
-    remove_hinting: bool = True,
-    verbose: bool = True,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Fix winding and remove overlaps and tiny paths from contours.
-    """
-    fonts = get_fonts_in_path(
-        input_path=input_path, allow_variable=False, allow_cff=False, recalc_timestamp=recalc_timestamp
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        print()
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            generic_info_message(f"Checking file {file.name}")
-            font.ttf_fix_contours(min_area=min_area, remove_hinting=remove_hinting, verbose=verbose)
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@ttf_tools.command()
-@add_file_or_path_argument()
-@click.option(
-    "--keep-hinting", "remove_hinting", is_flag=True, default=True, help="""Keep hinting for unmodified glyphs"""
-)
-@click.option(
-    "--ignore-errors",
-    is_flag=True,
-    help="""Ignore errors while removing overlaps.""",
-)
-@add_common_options()
-def remove_overlaps(
-    input_path: Path,
-    remove_hinting: bool = True,
-    ignore_errors: bool = False,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Simplify glyphs in TrueType fonts by merging overlapping contours.
-    """
-
-    fonts = get_fonts_in_path(input_path, recalc_timestamp=recalc_timestamp, allow_cff=False, allow_variable=False)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            font.ttf_remove_overlaps(remove_hinting=remove_hinting, ignore_errors=ignore_errors)
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@ttf_tools.command()
-@add_file_or_path_argument()
-@click.option(
-    "-upm",
-    type=int,
-    required=True,
-    help="""
-    New UPM value
-    """,
-)
-@add_common_options()
-def scale_upm(
-    input_path: Path, upm: int, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True
-):
-    """
-    Change the units-per-EM of TrueType fonts.
-
-    Hinting is removed from scaled TrueType fonts to avoid bad results. You may consider to use 'ftcli utils
-    ttf-autohint' to hint the scaled fonts.
-    """
-
-    fonts = get_fonts_in_path(input_path, allow_cff=False, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-
-            if font["head"].unitsPerEm == upm:
-                file_not_changed_message(file.relative_to(input_path))
-                continue
-
-            font.ttf_scale_upem(units_per_em=upm)
-
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            font.save(output_file)
-            file_saved_message(output_file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@ttf_tools.command()
-@add_file_or_path_argument()
-@click.option(
-    "-old",
-    "old_glyph_name",
-    required=True,
-    help="Old glyph name",
-)
-@click.option(
-    "-new",
-    "new_glyph_name",
-    required=True,
-    help="New glyph name",
-)
-@add_common_options()
-def rename_glyph(
-    input_path: Path,
-    old_glyph_name: str,
-    new_glyph_name: str,
-    recalc_timestamp: bool = False,
-    output_dir: Path = None,
-    overwrite: bool = True,
-):
-    """
-    Renames a glyph.
-    """
-    fonts = get_fonts_in_path(input_path=input_path, allow_cff=False, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-            glyph_names = font.getGlyphOrder()
-            modified = False
-            for i in range(len(glyph_names)):
-                if glyph_names[i] == old_glyph_name:
-                    glyph_names[i] = new_glyph_name
-                    generic_info_message(f"{old_glyph_name} renamed to {new_glyph_name}")
-                    modified = True
-            if modified:
-                font.setGlyphOrder(glyph_names)
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-cli = click.CommandCollection(
-    sources=[ttf_tools],
-    help="""
-    A set of tools to manipulate fonts with TrueType outlines.
-    """,
-)
+from io import BytesIO
+from pathlib import Path
+
+import click
+from fontTools.misc.cliTools import makeOutputFileName
+
+from foundryToolsCLI.Lib.Font import Font
+from foundryToolsCLI.Lib.utils.cli_tools import (
+    get_fonts_in_path,
+    get_output_dir,
+    initial_check_pass,
+)
+from foundryToolsCLI.Lib.utils.click_tools import (
+    add_file_or_path_argument,
+    add_common_options,
+    file_not_changed_message,
+    file_saved_message,
+    generic_error_message,
+    generic_info_message,
+)
+
+ttf_tools = click.Group("subcommands")
+
+
+@ttf_tools.command()
+@add_file_or_path_argument()
+@add_common_options()
+def autohint(
+    input_path: Path,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Autohint TrueType fonts using ttfautohint-py.
+    """
+
+    from ttfautohint import ttfautohint
+
+    fonts = get_fonts_in_path(
+        input_path,
+        recalc_timestamp=recalc_timestamp,
+        allow_cff=False,
+        allow_variable=False,
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            buf = BytesIO()
+            font.save(buf)
+            data = ttfautohint(in_buffer=buf.getvalue(), no_info=True)
+            hinted_font = Font(BytesIO(data))
+            file = Path(font.reader.file.name)
+            if not recalc_timestamp:
+                hinted_font.set_modified_timestamp(font.modified_timestamp)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            hinted_font.save(output_file)
+            file_saved_message(output_file)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@ttf_tools.command()
+@add_file_or_path_argument()
+@add_common_options()
+def decompose(
+    input_path: Path,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Decompose composite glyphs of a TrueType font.
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp, allow_cff=False)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            font.ttf_decomponentize()
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            font.save(output_file)
+            file_saved_message(output_file)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@ttf_tools.command()
+@add_file_or_path_argument()
+@add_common_options()
+def dehint(
+    input_path: Path,
+    recalc_timestamp: bool = False,
+    output_dir: Path = None,
+    overwrite: bool = True,
+):
+    """
+    Drops hinting from TrueType fonts.
+
+    This is a CLI for dehinter by Source Foundry: https://github.com/source-foundry/dehinter
+    """
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp, allow_cff=False)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            font.ttf_dehint()
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            font.save(output_file)
+            file_saved_message(output_file)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@ttf_tools.command()
+@add_file_or_path_argument()
+@click.option(
+    "--min-area",
+    type=int,
+    default=25,
+    help="""
+        Minimum area for a tiny outline.
+
+        Default is 25 square units. Subpaths with a bounding box less than this will be reported and deleted.
+    """,
+)
+@click.option(
+    "--keep-hinting",
+    "remove_hinting",
+    is_flag=True,
+    default=True,
+    help="""Do not remove hinting.""",
+)
+@click.option("--silent", "verbose", is_flag=True, default=True, help="Run in silent mode")
+@add_common_options()
+def fix_contours(
+    input_path: Path,
+    min_area: int = 25,
+    remove_hinting: bool = True,
+    verbose: bool = True,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Fix winding and remove overlaps and tiny paths from contours.
+    """
+    fonts = get_fonts_in_path(
+        input_path=input_path,
+        allow_variable=False,
+        allow_cff=False,
+        recalc_timestamp=recalc_timestamp,
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        print()
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            generic_info_message(f"Checking file {file.name}")
+            font.ttf_fix_contours(min_area=min_area, remove_hinting=remove_hinting, verbose=verbose)
+            font.save(output_file)
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@ttf_tools.command()
+@add_file_or_path_argument()
+@click.option(
+    "--keep-hinting",
+    "remove_hinting",
+    is_flag=True,
+    default=True,
+    help="""Keep hinting for unmodified glyphs""",
+)
+@click.option(
+    "--ignore-errors",
+    is_flag=True,
+    help="""Ignore errors while removing overlaps.""",
+)
+@add_common_options()
+def remove_overlaps(
+    input_path: Path,
+    remove_hinting: bool = True,
+    ignore_errors: bool = False,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Simplify glyphs in TrueType fonts by merging overlapping contours.
+    """
+
+    fonts = get_fonts_in_path(
+        input_path,
+        recalc_timestamp=recalc_timestamp,
+        allow_cff=False,
+        allow_variable=False,
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            font.ttf_remove_overlaps(remove_hinting=remove_hinting, ignore_errors=ignore_errors)
+            font.save(output_file)
+            file_saved_message(output_file)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@ttf_tools.command()
+@add_file_or_path_argument()
+@click.option(
+    "-upm",
+    type=int,
+    required=True,
+    help="""
+    New UPM value
+    """,
+)
+@add_common_options()
+def scale_upm(
+    input_path: Path,
+    upm: int,
+    recalc_timestamp: bool = False,
+    output_dir: Path = None,
+    overwrite: bool = True,
+):
+    """
+    Change the units-per-EM of TrueType fonts.
+
+    Hinting is removed from scaled TrueType fonts to avoid bad results. You may consider to use 'ftcli utils
+    ttf-autohint' to hint the scaled fonts.
+    """
+
+    fonts = get_fonts_in_path(input_path, allow_cff=False, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+
+            if font["head"].unitsPerEm == upm:
+                file_not_changed_message(file.relative_to(input_path))
+                continue
+
+            font.ttf_scale_upem(units_per_em=upm)
+
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            font.save(output_file)
+            file_saved_message(output_file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@ttf_tools.command()
+@add_file_or_path_argument()
+@click.option(
+    "-old",
+    "old_glyph_name",
+    required=True,
+    help="Old glyph name",
+)
+@click.option(
+    "-new",
+    "new_glyph_name",
+    required=True,
+    help="New glyph name",
+)
+@add_common_options()
+def rename_glyph(
+    input_path: Path,
+    old_glyph_name: str,
+    new_glyph_name: str,
+    recalc_timestamp: bool = False,
+    output_dir: Path = None,
+    overwrite: bool = True,
+):
+    """
+    Renames a glyph.
+    """
+    fonts = get_fonts_in_path(input_path=input_path, allow_cff=False, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+            glyph_names = font.getGlyphOrder()
+            modified = False
+            for i in range(len(glyph_names)):
+                if glyph_names[i] == old_glyph_name:
+                    glyph_names[i] = new_glyph_name
+                    generic_info_message(f"{old_glyph_name} renamed to {new_glyph_name}")
+                    modified = True
+            if modified:
+                font.setGlyphOrder(glyph_names)
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+cli = click.CommandCollection(
+    sources=[ttf_tools],
+    help="""
+    A set of tools to manipulate fonts with TrueType outlines.
+    """,
+)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/CLI/ftcli_utils.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,344 +1,344 @@
-from copy import deepcopy
-from pathlib import Path
-
-import click
-from fontTools.misc.cliTools import makeOutputFileName
-from pathvalidate import sanitize_filename, sanitize_filepath
-
-from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
-from foundryToolsCLI.Lib.utils.click_tools import (
-    add_file_or_path_argument,
-    add_common_options,
-    file_not_changed_message,
-    file_saved_message,
-    generic_error_message,
-    generic_warning_message,
-    no_valid_fonts_message,
-    generic_success_message,
-    generic_info_message,
-)
-
-CWD = Path.cwd()
-utils = click.Group("subcommands")
-
-
-@utils.command()
-@add_file_or_path_argument()
-@add_common_options()
-def add_dsig(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
-    """
-    Adds a dummy DSIG table to the fonts, unless the table is already present, or the font flavor is woff2.
-    """
-
-    fonts = get_fonts_in_path(
-        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_extensions=[".ttf", ".otf", ".woff"]
-    )
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            if "DSIG" not in font:
-                font.add_dummy_dsig()
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@utils.command()
-@add_file_or_path_argument()
-@click.option(
-    "-t",
-    "table_tags",
-    multiple=True,
-    required=True,
-    help=""" TableTag of the table(s) to delete. Can be repeated to delete multiple tables at once.""",
-)
-@add_common_options()
-def del_table(
-    input_path: Path, table_tags: tuple, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True
-):
-    """
-    Deletes the specified tables from the fonts.
-    """
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    table_tags = [tag.ljust(4, " ") for tag in table_tags]
-
-    for font in fonts:
-        removed_tables_counter = 0
-        try:
-            file = Path(font.reader.file.name)
-            for tag in table_tags:
-                if tag in font.keys():
-                    del font[tag]
-                    removed_tables_counter += 1
-                else:
-                    generic_warning_message(f"'{tag}' table is not present in {file.name}")
-
-            if removed_tables_counter > 0:
-                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@utils.command()
-@click.option(
-    "-f",
-    "--foundry",
-    "sort_by_foundry",
-    is_flag=True,
-    help="""
-    Organize fonts by foundry.
-
-    Foundry directory will be created at top level, with Family Name directory as child.
-
-    Foundry name is obtained trying to read nameID 8 (Manufacturer Name), using as fallback nameID 9 (Designer).
-    If nor nameID 8 nor nameID 9 are present in the 'name' table, the string is retrieved from achVendID in the 'OS/2'
-    table.
-    """,
-)
-@click.option(
-    "-e",
-    "--extension",
-    "sort_by_extension",
-    is_flag=True,
-    help="Moves fonts into a folder named after their real extension.",
-)
-@click.option(
-    "-v",
-    "--version",
-    "sort_by_version",
-    is_flag=True,
-    help="Appends the version string to the family folder.",
-)
-@add_file_or_path_argument()
-def font_organizer(
-    input_path: Path, sort_by_foundry: bool = False, sort_by_extension: bool = False, sort_by_version: bool = False
-):
-    """
-    Sorts fonts in folders by family name and optionally by foundry, font revision and extension.
-    """
-    fonts = get_fonts_in_path(input_path=input_path)
-    if len(fonts) == 0:
-        no_valid_fonts_message(input_path=input_path)
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_dir = file.parent
-            family_name = font.guess_family_name()
-
-            foundry = font.guess_foundry_name() if sort_by_foundry else None
-            if foundry:
-                output_dir = output_dir.joinpath(foundry)
-
-            version = f" v{round(font['head'].fontRevision, 3)}" if sort_by_version else None
-            if version:
-                family_name = family_name + version
-            output_dir = output_dir.joinpath(family_name)
-
-            extension = font.get_real_extension().replace(".", "") if sort_by_extension else None
-            if extension:
-                output_dir = output_dir.joinpath(extension)
-
-            output_dir = sanitize_filepath(output_dir, platform="auto")
-            output_dir.mkdir(parents=True, exist_ok=True)
-
-            target = Path(makeOutputFileName(output_dir.joinpath(file.name), overWrite=False))
-            file.rename(target=target)
-
-            generic_info_message(
-                f"{file.relative_to(CWD).name} {click.style('-->', fg='bright_magenta')} {target.relative_to(CWD)}"
-            )
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-@utils.command()
-@add_file_or_path_argument()
-@click.option(
-    "-s",
-    "--source",
-    type=click.Choice(choices=["1", "2", "3", "4", "5"]),
-    default="1",
-    help="""
-              The source string(s) from which to extract the new file name. Default is 1 (FamilyName-StyleName), used
-              also as fallback name when 4 or 5 are passed but the font is TrueType
-
-              \b
-              1: FamilyName-StyleName
-              2: PostScript Name
-              3: Full Font Name
-              4: CFF TopDict fontNames (CFF fonts only)
-              5: CFF TopDict FullName (CFF fonts only)
-              """,
-)
-def font_renamer(input_path: Path, source: str):
-    """
-    Rename font files according to the provided source string.
-    """
-
-    fonts = get_fonts_in_path(input_path=input_path)
-    if len(fonts) == 0:
-        no_valid_fonts_message(input_path)
-
-    # click.Choice() only accepts strings as choices, so we need to convert to integer
-    source = int(source)
-
-    for font in fonts:
-        file = Path(font.reader.file.name)
-
-        if font.is_ttf and source in (4, 5):
-            generic_warning_message(f"Source 4 and 5 con be used for OTF files only. Using source=1 for {file.name}")
-
-        old_file_name, old_file_extension = file.stem, file.suffix
-        new_file_name = sanitize_filename(font.get_file_name(source=source), platform="auto")
-        new_file_extension = font.get_real_extension()
-
-        if f"{new_file_name}{new_file_extension}" != f"{old_file_name}{old_file_extension}":
-            try:
-                output_file = Path(
-                    makeOutputFileName(
-                        new_file_name, extension=new_file_extension, outputDir=file.parent, overWrite=False
-                    )
-                )
-                file.rename(output_file)
-                generic_success_message(
-                    f"{file.relative_to(CWD)} {click.style('-->', fg='bright_magenta')} {output_file.relative_to(CWD)}"
-                )
-            except Exception as e:
-                generic_error_message(e)
-        else:
-            file_not_changed_message(file.relative_to(CWD))
-
-        font.close()
-
-
-@utils.command()
-@add_file_or_path_argument()
-@click.option("-major", type=click.IntRange(0, 999), help="Major version")
-@click.option("-minor", type=click.IntRange(0, 999), help="Minor version")
-@click.option("-ui", "--unique-identifier", is_flag=True, help="Recalculates nameID 3 (Unique identifier)")
-@click.option("-vs", "--version-string", is_flag=True, help="Recalculates nameID 5 (version string)")
-@add_common_options()
-def set_revision(
-    input_path: Path,
-    major: int = None,
-    minor: int = None,
-    unique_identifier: bool = False,
-    version_string: bool = False,
-    output_dir: Path = None,
-    recalc_timestamp: bool = False,
-    overwrite: bool = True,
-):
-    """
-    Sets [head].fontRevision and CFF.cff.topDictIndex[0].version values.
-
-    Optionally, also nameID 3 (Unique identifier) and nameID 5 (Version string) can be recalculated by using
-    `--unique-identifier` and `--version-string options`. Even if Unique identifier and Version string should be changed
-    according to the new version, they are optional to leave control to the user, who could choose to set those names
-    manually with ftcli name set-name or ftcli name find-replace commands.
-    """
-
-    if major is None and minor is None:
-        generic_error_message("At least one parameter of -minor or -major must be passed")
-        return
-
-    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
-    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
-    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
-        return
-
-    from foundryToolsCLI.Lib.tables.head import TableHead
-    from foundryToolsCLI.Lib.tables.name import TableName
-    from foundryToolsCLI.Lib.tables.CFF_ import TableCFF
-    from foundryToolsCLI.Lib.tables.OS_2 import TableOS2
-
-    for font in fonts:
-        try:
-            file = Path(font.reader.file.name)
-            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
-
-            head_table: TableHead = font["head"]
-
-            has_changed = False
-
-            old_font_revision = str(head_table.get_font_revision()).rjust(3, "0")
-            old_major_version = str(old_font_revision).split(".")[0]
-            old_minor_version = str(old_font_revision).split(".")[1]
-
-            new_major_version = str(major) if major is not None else old_major_version
-            new_minor_version = str(minor).rjust(3, "0") if minor is not None else old_minor_version
-            new_font_revision = f"{new_major_version}.{new_minor_version}"
-
-            print(old_font_revision, new_font_revision)
-
-            if old_font_revision != new_font_revision:
-                head_table.set_font_revision(float(new_font_revision))
-                has_changed = True
-
-            if font.is_otf:
-                cff: TableCFF = font["CFF "]
-                old_cff_version = cff.get_font_version()
-                new_cff_version = f"{int(new_major_version)}.{int(new_minor_version)}"
-                if old_cff_version != new_cff_version:
-                    cff.set_font_version(new_cff_version)
-                    has_changed = True
-
-            if unique_identifier or version_string:
-                name_table: TableName = font["name"]
-                name_table_copy = deepcopy(name_table)
-
-                if unique_identifier:
-                    os2: TableOS2 = font["OS/2"]
-                    vend_id = os2.get_vend_id()
-                    ps_name = name_table.getDebugName(6)
-                    name_table.add_name(font, string=f"{new_font_revision};{vend_id};{ps_name}", name_id=3)
-
-                if version_string:
-                    name_table.add_name(font, string=f"Version {new_font_revision}", name_id=5)
-
-                if name_table_copy.compile(font) != name_table.compile(font):
-                    has_changed = True
-
-            if has_changed:
-                font.save(output_file)
-                file_saved_message(output_file.relative_to(CWD))
-            else:
-                file_not_changed_message(file.relative_to(CWD))
-
-        except Exception as e:
-            generic_error_message(e)
-        finally:
-            font.close()
-
-
-cli = click.CommandCollection(
-    sources=[utils],
-    help="""
-    Miscellaneous utilities.
-    """,
-)
+from copy import deepcopy
+from pathlib import Path
+
+import click
+from fontTools.misc.cliTools import makeOutputFileName
+from pathvalidate import sanitize_filename, sanitize_filepath
+
+from foundryToolsCLI.Lib.utils.cli_tools import get_fonts_in_path, get_output_dir, initial_check_pass
+from foundryToolsCLI.Lib.utils.click_tools import (
+    add_file_or_path_argument,
+    add_common_options,
+    file_not_changed_message,
+    file_saved_message,
+    generic_error_message,
+    generic_warning_message,
+    no_valid_fonts_message,
+    generic_success_message,
+    generic_info_message,
+)
+
+utils = click.Group("subcommands")
+
+
+@utils.command()
+@add_file_or_path_argument()
+@add_common_options()
+def add_dsig(input_path: Path, output_dir: Path = None, recalc_timestamp: bool = False, overwrite: bool = True):
+    """
+    Adds a dummy DSIG table to the fonts, unless the table is already present, or the font flavor is woff2.
+    """
+
+    fonts = get_fonts_in_path(
+        input_path=input_path, recalc_timestamp=recalc_timestamp, allow_extensions=[".ttf", ".otf", ".woff"]
+    )
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            if "DSIG" not in font:
+                font.add_dummy_dsig()
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@utils.command()
+@add_file_or_path_argument()
+@click.option(
+    "-t",
+    "table_tags",
+    multiple=True,
+    required=True,
+    help=""" TableTag of the table(s) to delete. Can be repeated to delete multiple tables at once.""",
+)
+@add_common_options()
+def del_table(
+    input_path: Path, table_tags: tuple, recalc_timestamp: bool = False, output_dir: Path = None, overwrite: bool = True
+):
+    """
+    Deletes the specified tables from the fonts.
+    """
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    table_tags = [tag.ljust(4, " ") for tag in table_tags]
+
+    for font in fonts:
+        removed_tables_counter = 0
+        try:
+            file = Path(font.reader.file.name)
+            for tag in table_tags:
+                if tag in font.keys():
+                    del font[tag]
+                    removed_tables_counter += 1
+                else:
+                    generic_warning_message(f"'{tag}' table is not present in {file.name}")
+
+            if removed_tables_counter > 0:
+                output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@utils.command()
+@click.option(
+    "-f",
+    "--foundry",
+    "sort_by_foundry",
+    is_flag=True,
+    help="""
+    Organize fonts by foundry.
+
+    Foundry directory will be created at top level, with Family Name directory as child.
+
+    Foundry name is obtained trying to read nameID 8 (Manufacturer Name), using as fallback nameID 9 (Designer).
+    If nor nameID 8 nor nameID 9 are present in the 'name' table, the string is retrieved from achVendID in the 'OS/2'
+    table.
+    """,
+)
+@click.option(
+    "-e",
+    "--extension",
+    "sort_by_extension",
+    is_flag=True,
+    help="Moves fonts into a folder named after their real extension.",
+)
+@click.option(
+    "-v",
+    "--version",
+    "sort_by_version",
+    is_flag=True,
+    help="Appends the version string to the family folder.",
+)
+@add_file_or_path_argument()
+def font_organizer(
+    input_path: Path, sort_by_foundry: bool = False, sort_by_extension: bool = False, sort_by_version: bool = False
+):
+    """
+    Sorts fonts in folders by family name and optionally by foundry, font revision and extension.
+    """
+    fonts = get_fonts_in_path(input_path=input_path)
+    if len(fonts) == 0:
+        no_valid_fonts_message(input_path=input_path)
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_dir = file.parent
+            family_name = font.guess_family_name()
+
+            foundry = font.guess_foundry_name() if sort_by_foundry else None
+            if foundry:
+                output_dir = output_dir.joinpath(foundry)
+
+            version = f" v{round(font['head'].fontRevision, 3)}" if sort_by_version else None
+            if version:
+                family_name = family_name + version
+            output_dir = output_dir.joinpath(family_name)
+
+            extension = font.get_real_extension().replace(".", "") if sort_by_extension else None
+            if extension:
+                output_dir = output_dir.joinpath(extension)
+
+            output_dir = sanitize_filepath(output_dir, platform="auto")
+            output_dir.mkdir(parents=True, exist_ok=True)
+
+            target = Path(makeOutputFileName(output_dir.joinpath(file.name), overWrite=False))
+            file.rename(target=target)
+
+            generic_info_message(
+                f"{file.relative_to(input_path).name} {click.style('-->', fg='bright_magenta')} "
+                f"{target.relative_to(input_path)}"
+            )
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+@utils.command()
+@add_file_or_path_argument()
+@click.option(
+    "-s",
+    "--source",
+    type=click.Choice(choices=["1", "2", "3", "4", "5"]),
+    default="1",
+    help="""
+              The source string(s) from which to extract the new file name. Default is 1 (FamilyName-StyleName), used
+              also as fallback name when 4 or 5 are passed but the font is TrueType
+
+              \b
+              1: FamilyName-StyleName
+              2: PostScript Name
+              3: Full Font Name
+              4: CFF TopDict fontNames (CFF fonts only)
+              5: CFF TopDict FullName (CFF fonts only)
+              """,
+)
+def font_renamer(input_path: Path, source: str):
+    """
+    Rename font files according to the provided source string.
+    """
+
+    fonts = get_fonts_in_path(input_path=input_path)
+    if len(fonts) == 0:
+        no_valid_fonts_message(input_path)
+
+    # click.Choice() only accepts strings as choices, so we need to convert to integer
+    source = int(source)
+
+    for font in fonts:
+        file = Path(font.reader.file.name)
+
+        if font.is_ttf and source in (4, 5):
+            generic_warning_message(f"Source 4 and 5 con be used for OTF files only. Using source=1 for {file.name}")
+
+        old_file_name, old_file_extension = file.stem, file.suffix
+        new_file_name = sanitize_filename(font.get_file_name(source=source), platform="auto")
+        new_file_extension = font.get_real_extension()
+
+        if f"{new_file_name}{new_file_extension}" != f"{old_file_name}{old_file_extension}":
+            try:
+                output_file = Path(
+                    makeOutputFileName(
+                        new_file_name, extension=new_file_extension, outputDir=file.parent, overWrite=False
+                    )
+                )
+                file.rename(output_file)
+                generic_success_message(
+                    f"{file.name} {click.style('-->', fg='bright_magenta')} {output_file.name}"
+                )
+            except Exception as e:
+                generic_error_message(e)
+        else:
+            file_not_changed_message(file)
+
+        font.close()
+
+
+@utils.command()
+@add_file_or_path_argument()
+@click.option("-major", type=click.IntRange(0, 999), help="Major version")
+@click.option("-minor", type=click.IntRange(0, 999), help="Minor version")
+@click.option("-ui", "--unique-identifier", is_flag=True, help="Recalculates nameID 3 (Unique identifier)")
+@click.option("-vs", "--version-string", is_flag=True, help="Recalculates nameID 5 (version string)")
+@add_common_options()
+def set_revision(
+    input_path: Path,
+    major: int = None,
+    minor: int = None,
+    unique_identifier: bool = False,
+    version_string: bool = False,
+    output_dir: Path = None,
+    recalc_timestamp: bool = False,
+    overwrite: bool = True,
+):
+    """
+    Sets [head].fontRevision and CFF.cff.topDictIndex[0].version values.
+
+    Optionally, also nameID 3 (Unique identifier) and nameID 5 (Version string) can be recalculated by using
+    `--unique-identifier` and `--version-string options`. Even if Unique identifier and Version string should be changed
+    according to the new version, they are optional to leave control to the user, who could choose to set those names
+    manually with ftcli name set-name or ftcli name find-replace commands.
+    """
+
+    if major is None and minor is None:
+        generic_error_message("At least one parameter of -minor or -major must be passed")
+        return
+
+    fonts = get_fonts_in_path(input_path=input_path, recalc_timestamp=recalc_timestamp)
+    output_dir = get_output_dir(input_path=input_path, output_dir=output_dir)
+    if not initial_check_pass(fonts=fonts, output_dir=output_dir):
+        return
+
+    from foundryToolsCLI.Lib.tables.head import TableHead
+    from foundryToolsCLI.Lib.tables.name import TableName
+    from foundryToolsCLI.Lib.tables.CFF_ import TableCFF
+    from foundryToolsCLI.Lib.tables.OS_2 import TableOS2
+
+    for font in fonts:
+        try:
+            file = Path(font.reader.file.name)
+            output_file = Path(makeOutputFileName(file, outputDir=output_dir, overWrite=overwrite))
+
+            head_table: TableHead = font["head"]
+
+            has_changed = False
+
+            old_font_revision = str(head_table.get_font_revision()).rjust(3, "0")
+            old_major_version = str(old_font_revision).split(".")[0]
+            old_minor_version = str(old_font_revision).split(".")[1]
+
+            new_major_version = str(major) if major is not None else old_major_version
+            new_minor_version = str(minor).rjust(3, "0") if minor is not None else old_minor_version
+            new_font_revision = f"{new_major_version}.{new_minor_version}"
+
+            print(old_font_revision, new_font_revision)
+
+            if old_font_revision != new_font_revision:
+                head_table.set_font_revision(float(new_font_revision))
+                has_changed = True
+
+            if font.is_otf:
+                cff: TableCFF = font["CFF "]
+                old_cff_version = cff.get_font_version()
+                new_cff_version = f"{int(new_major_version)}.{int(new_minor_version)}"
+                if old_cff_version != new_cff_version:
+                    cff.set_font_version(new_cff_version)
+                    has_changed = True
+
+            if unique_identifier or version_string:
+                name_table: TableName = font["name"]
+                name_table_copy = deepcopy(name_table)
+
+                if unique_identifier:
+                    os2: TableOS2 = font["OS/2"]
+                    vend_id = os2.get_vend_id()
+                    ps_name = name_table.getDebugName(6)
+                    name_table.add_name(font, string=f"{new_font_revision};{vend_id};{ps_name}", name_id=3)
+
+                if version_string:
+                    name_table.add_name(font, string=f"Version {new_font_revision}", name_id=5)
+
+                if name_table_copy.compile(font) != name_table.compile(font):
+                    has_changed = True
+
+            if has_changed:
+                font.save(output_file)
+                file_saved_message(output_file)
+            else:
+                file_not_changed_message(file)
+
+        except Exception as e:
+            generic_error_message(e)
+        finally:
+            font.close()
+
+
+cli = click.CommandCollection(
+    sources=[utils],
+    help="""
+    Miscellaneous utilities.
+    """,
+)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/Font.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/Font.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1024 +1,1020 @@
-import math
-import os
-import tempfile
-from pathlib import Path
-
-from beziers.line import Line
-from beziers.path import BezierPath
-from beziers.point import Point
-from fontTools.misc.psCharStrings import T2CharString
-from fontTools.misc.timeTools import timestampToString
-from fontTools.pens.boundsPen import BoundsPen
-from fontTools.ttLib.ttFont import TTFont
-
-from foundryToolsCLI.Lib.tables.hhea import TableHhea
-from foundryToolsCLI.Lib.tables.name import TableName
-from foundryToolsCLI.Lib.tables.OS_2 import TableOS2
-from foundryToolsCLI.Lib.tables.head import TableHead
-from foundryToolsCLI.Lib.tables.post import TablePost
-
-
-# The Font class is a subclass of the fontTools.ttLib.TTFont class.
-class Font(TTFont):
-    def __init__(self, file=None, recalcBBoxes: bool = True, recalcTimestamp: bool = False, lazy: bool = None):
-        super().__init__(file=file, recalcBBoxes=recalcBBoxes, recalcTimestamp=recalcTimestamp, lazy=lazy)
-
-    @property
-    def is_otf(self) -> bool:
-        """
-        This function checks if the "CFF " table is present in the Font object and returns a boolean
-        value.
-
-        :return: A boolean value indicating whether the font is OpenType-PS.
-        """
-        return "CFF " in self
-
-    @property
-    def is_ttf(self) -> bool:
-        """
-        This function checks if the string "glyf" table is present in the Font object and returns a boolean
-        value.
-
-        :return: A boolean value indicating whether the font is TrueType.
-        """
-        return "glyf" in self
-
-    @property
-    def is_variable(self) -> bool:
-        """
-        This function checks if the "fvar" table is present in the Font object.
-
-        :return: A boolean value indicating whether the font is variable.
-        """
-        return "fvar" in self
-
-    @property
-    def is_static(self) -> bool:
-        """
-        The function checks if the "fvar" table is not present in the Font object.
-
-        :return: A boolean value indicating whether the font is static.
-        """
-        return "fvar" not in self
-
-    @property
-    def is_woff(self) -> bool:
-        """
-        This function checks if the flavor of a font file is "woff" and returns a boolean value.
-
-        :return: A boolean value indicating whether the font flavor is "woff" flavored or not.
-        """
-        return self.flavor == "woff"
-
-    @property
-    def is_woff2(self) -> bool:
-        """
-        This function checks if the flavor of a font file is "woff2" and returns a boolean value.
-
-        :return: A boolean value indicating whether the font is "woff2" flavored or not.
-        """
-        return self.flavor == "woff2"
-
-    @property
-    def is_sfnt(self) -> bool:
-        """
-        This function checks if the font is in SFNT format.
-
-        :return: A boolean value indicating whether the "flavor" attribute of the object is None or not.
-        If it is None, the function will return True, otherwise it will return False.
-        """
-        return self.flavor is None
-
-    @property
-    def is_bold(self) -> bool:
-        """
-        > Checks if OS/2.fsSelection bit 5 and head.macStyle bit 0 are set
-
-        :return: A boolean value.
-        """
-        head: TableHead = self["head"]
-        os_2: TableOS2 = self["OS/2"]
-
-        return head.is_bold_bit_set() and os_2.is_bold_bit_set()
-
-    @property
-    def is_italic(self) -> bool:
-        """
-        > Checks if  OS/2.fsSelection bit 0 and head.macStyle bit 1 are set
-
-        :return: A boolean value.
-        """
-        head: TableHead = self["head"]
-        os_2: TableOS2 = self["OS/2"]
-
-        return head.is_italic_bit_set() and os_2.is_italic_bit_set()
-
-    @property
-    def is_regular(self) -> bool:
-        """
-        > Checks if the fsSelection bit 6 is set, and the bold and italic bits are not set
-
-        :return: A boolean value.
-        """
-        os_2: TableOS2 = self["OS/2"]
-
-        return os_2.is_regular_bit_set() and not self.is_bold and not self.is_italic
-
-    @property
-    def is_oblique(self) -> bool:
-        """
-        > Checks if OS/2.fsSelection bit 9 is set
-
-        :return: A bool value.
-        """
-        os_2: TableOS2 = self["OS/2"]
-
-        return os_2.is_oblique_bit_set()
-
-    @property
-    def is_upright(self) -> bool:
-        """
-        If the font is not italic and not oblique, then it is upright
-
-        :return: A bool value.
-        """
-        return not self.is_italic and not self.is_oblique
-
-    @property
-    def created_timestamp(self) -> int:
-        """
-        This function returns the created timestamp stored in the 'head' table.
-
-        :return: The function `get_created_timestamp` is returning an integer value representing the
-        creation timestamp of the Font object.
-        """
-        return self["head"].created
-
-    @property
-    def modified_timestamp(self) -> int:
-        """
-        This function returns the modified timestamp stored in the "head" table.
-
-        :return: an integer value representing the modified timestamp of the Font object.
-        """
-        return self["head"].modified
-
-    @property
-    def is_hinted_ttf(self) -> bool:
-        return "fpgm" in self and self.is_ttf
-
-    def set_bold_flag(self, value: bool) -> None:
-        """
-        Sets the bold bit in the OS/2 table and the head table, and clears the regular bit in the OS/2 table
-        """
-
-        head: TableHead = self["head"]
-        os_2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os_2.set_bold_bit()
-            head.set_bold_bit()
-            os_2.clear_regular_bit()
-        else:
-            os_2.clear_bold_bit()
-            head.clear_bold_bit()
-            if not self.is_italic:
-                os_2.set_regular_bit()
-
-    def set_italic_flag(self, value: bool) -> None:
-        """
-        Sets the italic bit in the OS/2 table and clears the regular bit
-        """
-        head: TableHead = self["head"]
-        os_2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os_2.set_italic_bit()
-            head.set_italic_bit()
-            os_2.clear_regular_bit()
-        else:
-            os_2.clear_italic_bit()
-            head.clear_italic_bit()
-            if not self.is_bold:
-                os_2.set_regular_bit()
-
-    def set_oblique_flag(self, value: bool) -> None:
-        """
-        Sets the oblique bit in the OS/2 table
-        """
-        os_2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os_2.set_oblique_bit()
-        else:
-            os_2.clear_oblique_bit()
-
-    def set_regular_flag(self, value: bool) -> None:
-        """
-        Sets the regular bit in the OS/2 table, clears the bold and italic bits in the OS/2 and head tables
-        """
-        if self.is_regular:
-            return
-
-        head: TableHead = self["head"]
-        os_2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os_2.set_regular_bit()
-            os_2.clear_bold_bit()
-            os_2.clear_italic_bit()
-            head.clear_bold_bit()
-            head.clear_italic_bit()
-        else:
-            if self.is_bold or self.is_italic:
-                os_2.clear_regular_bit()
-
-    def set_use_typo_metrics_flag(self, value: bool) -> None:
-        os_2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os_2.set_use_typo_metrics_bit()
-        else:
-            os_2.clear_use_typo_metrics_bit()
-
-    def set_wws_consistent_flag(self, value: bool) -> None:
-        os_2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os_2.set_wws_consistent_bit()
-        else:
-            os_2.clear_wws_consistent_bit()
-
-    def set_underscore_flag(self, value: bool) -> None:
-        os_2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os_2.set_underscore_bit()
-        else:
-            os_2.clear_underscore_bit()
-
-    def set_negative_flag(self, value: bool) -> None:
-        os_2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os_2.set_negative_bit()
-        else:
-            os_2.clear_negative_bit()
-
-    def set_outlined_flag(self, value: bool) -> None:
-        os_2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os_2.set_outlined_bit()
-        else:
-            os_2.clear_outlined_bit()
-
-    def set_strikeout_flag(self, value: bool) -> None:
-        os_2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os_2.set_strikeout_bit()
-        else:
-            os_2.clear_strikeout_bit()
-
-    def set_embed_level_flag(self, value: int) -> None:
-        os2: TableOS2 = self["OS/2"]
-
-        os2.set_embed_level(value)
-
-    def set_bitmap_embedding_only_flag(self, value: bool) -> None:
-        os2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os2.set_bitmap_embed_only_bit()
-        else:
-            os2.clear_bitmap_embed_only_bit()
-
-    def set_no_subsetting_flag(self, value: bool) -> None:
-        os_2: TableOS2 = self["OS/2"]
-
-        if value is True:
-            os_2.set_no_subsetting_bit()
-        else:
-            os_2.clear_no_subsetting_bit()
-
-    def get_bounding_box(self):
-        """Returns max and min bbox of the font"""
-        y_min = 0
-        y_max = 0
-        if self.is_otf:
-            y_min = self["head"].yMin
-            y_max = self["head"].yMax
-        else:
-            for g in self["glyf"].glyphs:
-                char = self["glyf"][g]
-                if hasattr(char, "yMin") and y_min > char.yMin:
-                    y_min = char.yMin
-                if hasattr(char, "yMax") and y_max < char.yMax:
-                    y_max = char.yMax
-        return y_min, y_max
-
-    def get_glyph_bounds(self, glyph_name: str) -> dict:
-        glyph_set = self.getGlyphSet()
-        if glyph_set.get(glyph_name) is None:
-            return dict(xMin=0, yMin=0, xMax=0, yMax=0)
-        bounds = T2CharString.calcBounds(glyph_set[glyph_name], glyph_set)
-        if bounds:
-            return dict(xMin=bounds[0], yMin=bounds[1], xMax=bounds[2], yMax=bounds[3])
-        else:
-            return dict(xMin=0, yMin=0, xMax=0, yMax=0)
-
-    def recalc_x_height(self) -> int:
-        return self.get_glyph_bounds("x")["yMax"]
-
-    def recalc_cap_height(self) -> int:
-        return self.get_glyph_bounds("H")["yMax"]
-
-    def recalc_max_context(self) -> int:
-        if self["OS/2"].version >= 2:
-            from fontTools.otlLib.maxContextCalc import maxCtxFont
-
-            max_context = maxCtxFont(self)
-            return max_context
-
-    def set_created_timestamp(self, timestamp: int) -> None:
-        """
-        This function sets the "created" attribute of the "head" table to the given timestamp.
-
-        :param timestamp: an integer representing a Unix timestamp (number of seconds since January 1,
-        1970) that indicates when the font was created
-        :type timestamp: int
-        """
-        self["head"].created = timestamp
-
-    def set_modified_timestamp(self, timestamp: int) -> None:
-        """
-        This function sets the "modified" attribute of the "head" table to the given timestamp.
-
-        :param timestamp: an integer representing a Unix timestamp (number of seconds since January 1,
-        1970) that indicates when the font was last modified
-        :type timestamp: int
-        """
-        self["head"].modified = timestamp
-
-    def get_real_extension(self) -> str:
-        """
-        This function returns the file extension of a font file based on its flavor or type.
-        :return: A string representing the file extension of a font file. If the font has a flavor, the
-        extension will be ".woff" or ".woff2". If the font is a TrueType font, the extension will be
-        ".ttf". If the font is an OpenType font, the extension will be ".otf".
-        """
-        if self.flavor is not None:
-            return f".{self.flavor}"
-        elif self.is_ttf:
-            return ".ttf"
-        elif self.is_otf:
-            return ".otf"
-
-    def ttf_decomponentize(self) -> None:
-        """
-        This function decomponentizes composite glyphs in a TrueType font.
-        """
-        if not self.is_ttf:
-            return
-
-        from foundryToolsCLI.Lib.utils.ttf_tools import decomponentize
-
-        decomponentize(self)
-
-    def ttf_dehint(self) -> None:
-        """
-        This function de-hints a TrueType font.
-        """
-        if not self.is_ttf:
-            return
-
-        from dehinter.font import dehint
-
-        dehint(tt=self, verbose=False)
-
-    def ttf_remove_overlaps(self, remove_hinting: bool = True, ignore_errors: bool = True):
-        """
-        This function removes overlaps in a TrueType font while optionally ignoring errors and removing
-        hinting.
-
-        :param remove_hinting: A boolean parameter that determines whether to remove hinting
-        information when removing overlaps in the font.
-
-        :type remove_hinting: bool (optional)
-
-        :param ignore_errors: If set to True, any errors encountered during the overlap removal process
-        will be ignored and the process will continue. If set to False, the process will stop and raise
-        an error if any issues are encountered, defaults to True
-
-        :type ignore_errors: bool (optional)
-        """
-        if self.is_otf or self.is_variable:
-            return
-
-        from fontTools.ttLib.removeOverlaps import removeOverlaps
-
-        removeOverlaps(font=self, removeHinting=remove_hinting, ignoreErrors=ignore_errors)
-
-    def ttf_scale_upem(self, units_per_em: int = 1000) -> None:
-        """
-        This function scales the units per em value of a TrueType font.
-
-        :param units_per_em: The units_per_em parameter is an integer value that represents the number
-        of font units-per-em, defaults to 1000
-
-        :type units_per_em: int (optional)
-        """
-        if not self.is_ttf:
-            return
-
-        from fontTools.ttLib.scaleUpem import scale_upem
-
-        if self.is_ttf:
-            self.ttf_dehint()
-        scale_upem(self, new_upem=units_per_em)
-
-    def otf_dehint(self) -> None:
-        """
-        This function removes hints from the CFF table of an OpenType font.
-        """
-        if not self.is_otf:
-            return
-        # noinspection PyUnresolvedReferences
-        from fontTools.subset.cff import remove_hints
-
-        self["CFF "].remove_hints()
-
-    def otf_desubroutinize(self) -> None:
-        """
-        This function removes subroutines from an OpenType font.
-        """
-        if not self.is_otf:
-            return
-
-        from cffsubr import desubroutinize
-
-        flavor = self.flavor
-        self.flavor = None
-        desubroutinize(otf=self)
-        self.flavor = flavor
-
-    def otf_subroutinize(self) -> None:
-        """
-        This function subroutinizes an OpenType font.
-        """
-        if not self.is_otf:
-            return
-
-        from cffsubr import subroutinize
-
-        flavor = self.flavor
-        self.flavor = None
-        subroutinize(otf=self)
-        self.flavor = flavor
-
-    def otf_fix_contours(self, min_area: int = 25, verbose: bool = False) -> None:
-        from foundryToolsCLI.Lib.utils.otf_tools import correct_otf_contours
-
-        correct_otf_contours(font=self, min_area=min_area, verbose=verbose)
-
-    def ttf_fix_contours(self, min_area: int = 25, remove_hinting: bool = True, verbose: bool = False) -> None:
-        from foundryToolsCLI.Lib.utils.ttf_tools import correct_ttf_contours
-
-        correct_ttf_contours(self, min_area=min_area, remove_hinting=remove_hinting, verbose=verbose)
-
-    def add_dummy_dsig(self) -> None:
-        """
-        This function adds a dummy DSIG table to a font file if it does not already exist.
-        """
-        if self.flavor == "woff2":
-            return
-
-        from fontTools.ttLib import newTable
-
-        values = dict(
-            ulVersion=1,
-            usFlag=0,
-            usNumSigs=0,
-            signatureRecords=[],
-        )
-        if "DSIG" not in self.keys():
-            dsig = self["DSIG"] = newTable("DSIG")
-            for k, v in values.items():
-                setattr(dsig, k, v)
-
-    def guess_family_name(self) -> str:
-        """
-        This function returns the font's family name, obtained from nameID 21, 16 or 1.
-
-        :return: A string representing the font's family name.
-        """
-        return self["name"].getBestFamilyName()
-
-    def guess_subfamily_name(self) -> str:
-        """
-        This function returns the font's subfamily name, obtained from nameID 22, 17 or 2.
-
-        :return: A string representing the font's subfamily name.
-        """
-        return self["name"].getBestSubFamilyName()
-
-    def get_file_name(self, source) -> str:
-        """
-        Returns the font's file name according to the passed source.
-
-        1: FamilyName-StyleName (FamilyName is retrieved from nameID 21, 16 or 1; SubFamily name from nameID 22,
-        17 or 2)
-
-        2: PostScript Name
-
-        3: Full Font Name
-
-        4: CFF TopDict fontNames. Valid for CFF fonts only. For TTF files will be used
-        '1' as fallback value.
-
-        5: CFF TipDict FullName (returns: Family Name Style Name or FamilyName-StyleName, depending on how FullName has
-        been built). Valid for CFF fonts only. For TTF files will be used '1' as fallback value.
-
-        :param source: The NameRecord or combination of NameRecords from which to build the file name.
-        :return: A string representing the file name of the font.
-        """
-
-        if self.is_ttf:
-            if source in (4, 5):
-                source = 1
-
-        if source == 1:
-            return f"{self.guess_family_name()}-{self.guess_subfamily_name()}".replace(" ", "")
-        elif source == 2:
-            return self["name"].getDebugName(6)
-        elif source == 3:
-            return self["name"].getDebugName(4)
-        elif source == 4:
-            return self["CFF "].cff.fontNames[0]
-        elif source == 5:
-            return self["CFF "].cff.topDictIndex[0].FullName
-        else:
-            return Path(self.reader.file.name).stem
-
-    def fix_cff_top_dict_version(self) -> None:
-        if not self.is_otf:
-            return
-        font_revision = str(round(self["head"].fontRevision, 3)).split(".")
-        major_version = int(font_revision[0])
-        minor_version = int(font_revision[1])
-        cff_font_version = f"{major_version}.{minor_version}"
-        self["CFF "].cff.topDictIndex[0].version = cff_font_version
-
-    def guess_foundry_name(self) -> str:
-        """
-        This function returns the foundry name of a font by checking the "name" or "OS/2" table.
-
-        :return: a string that represents the foundry name. If nameID 8 is present in the "name" table, the Manufacturer
-         Name string is returned. If nameID 8 is not present, but nameID 9 is found, the Designer string is returned.
-         If nor nameID 8 mor nameID 9 are present, the vendor code from the font's OS/2 table is returned. If also the
-         vendor code is empty or not found, "Unknown" is returned.
-        """
-        manufacturer_name: str = self["name"].getDebugName(8)
-        if manufacturer_name:
-            return manufacturer_name
-
-        designer: str = self["name"].getDebugName(9)
-        if designer:
-            return designer
-
-        try:
-            vendor_code: str = self["OS/2"].achVendID
-            if vendor_code.strip().strip("\x00") == "":
-                return "Unknown"
-            else:
-                return vendor_code
-        except KeyError:
-            return "Unknown"
-
-    def make_temp_otf(self) -> tuple[int, Path]:
-        from afdko.fdkutils import run_shell_command
-
-        if self.flavor is None:
-            source_file = self.reader.file.name
-            remove_source_file = False
-        else:
-            self.flavor = None
-            source_fd, source_file = tempfile.mkstemp(suffix=".tmp")
-            self.save(source_file)
-            remove_source_file = True
-            os.close(source_fd)
-
-        temp_t1_fd, temp_t1_file = tempfile.mkstemp(suffix=".t1")
-        temp_otf_fd, temp_otf_file = tempfile.mkstemp(suffix=".otf")
-
-        command_1 = ["tx", "-t1", source_file, temp_t1_file]
-        command_2 = ["makeotf", "-f", temp_t1_file, "-o", temp_otf_file]
-
-        run_shell_command(command_1, suppress_output=True)
-        run_shell_command(command_2, suppress_output=True)
-
-        os.close(temp_t1_fd)
-        os.remove(temp_t1_file)
-        if remove_source_file:
-            os.remove(source_file)
-        return temp_otf_fd, Path(temp_otf_file)
-
-    def get_ui_name_ids(self) -> list:
-        """
-        Returns a list of all the UI name IDs in the font's GSUB table
-
-        :return: A list of integers.
-        """
-        if "GSUB" not in self:
-            return []
-        else:
-            ui_name_ids = []
-            for record in self["GSUB"].table.FeatureList.FeatureRecord:
-                if record.Feature.FeatureParams:
-                    ui_name_ids.append(record.Feature.FeatureParams.UINameID)
-        return sorted(set(ui_name_ids))
-
-    def reorder_ui_name_ids(self):
-        """
-        Takes the IDs of the UI names in the name table and reorders them to start at 256
-        """
-
-        name_table: TableName = self["name"]
-
-        if "GSUB" not in self:
-            return
-        ui_name_ids = self.get_ui_name_ids()
-        for count, value in enumerate(ui_name_ids, start=256):
-            for n in name_table.names:
-                if n.nameID == value:
-                    n.nameID = count
-            for record in self["GSUB"].table.FeatureList.FeatureRecord:
-                if record.Feature.FeatureParams:
-                    if record.Feature.FeatureParams.UINameID == value:
-                        record.Feature.FeatureParams.UINameID = count
-
-    def modify_linegap_percent(self, percent):
-        """
-        Modifies the line spacing metrics
-
-        Adapted from https://github.com/source-foundry/font-line
-        """
-
-        os2_table = self["OS/2"]
-        head_table = self["head"]
-        hhea_table = self["hhea"]
-
-        # get observed start values from the font
-        os2_typo_ascender = os2_table.sTypoAscender
-        os2_typo_descender = os2_table.sTypoDescender
-        os2_typo_linegap = os2_table.sTypoLineGap
-        hhea_ascent = hhea_table.ascent
-        hhea_descent = hhea_table.descent
-        units_per_em = head_table.unitsPerEm
-
-        # calculate necessary delta values
-        os2_typo_ascdesc_delta = os2_typo_ascender + -os2_typo_descender
-        hhea_ascdesc_delta = hhea_ascent + -hhea_descent
-
-        # define percent UPM from command line request
-        factor = 1.0 * int(percent) / 100
-
-        # define line spacing units
-        line_spacing_units = int(factor * units_per_em)
-
-        # define total height as UPM + line spacing units
-        total_height = line_spacing_units + units_per_em
-
-        # height calculations for adjustments
-        delta_height = total_height - hhea_ascdesc_delta
-        upper_lower_add_units = int(0.5 * delta_height)
-
-        # redefine hhea linegap to 0 in all cases
-        hhea_linegap = 0
-
-        # Define metrics based upon original design approach in the font
-        # Google metrics approach
-        if os2_typo_linegap == 0 and (os2_typo_ascdesc_delta > units_per_em):
-            # define values
-            os2_typo_ascender += upper_lower_add_units
-            os2_typo_descender -= upper_lower_add_units
-            hhea_ascent += upper_lower_add_units
-            hhea_descent -= upper_lower_add_units
-            os2_win_ascent = hhea_ascent
-            os2_win_descent = -hhea_descent
-        # Adobe metrics approach
-        elif os2_typo_linegap == 0 and (os2_typo_ascdesc_delta == units_per_em):
-            hhea_ascent += upper_lower_add_units
-            hhea_descent -= upper_lower_add_units
-            os2_win_ascent = hhea_ascent
-            os2_win_descent = -hhea_descent
-        else:
-            os2_typo_linegap = line_spacing_units
-            hhea_ascent = int(os2_typo_ascender + 0.5 * os2_typo_linegap)
-            hhea_descent = -(total_height - hhea_ascent)
-            os2_win_ascent = hhea_ascent
-            os2_win_descent = -hhea_descent
-
-        # define updated values from above calculations
-        hhea_table.lineGap = hhea_linegap
-        os2_table.sTypoAscender = os2_typo_ascender
-        os2_table.sTypoDescender = os2_typo_descender
-        os2_table.sTypoLineGap = os2_typo_linegap
-        os2_table.usWinAscent = os2_win_ascent
-        os2_table.usWinDescent = os2_win_descent
-        hhea_table.ascent = hhea_ascent
-        hhea_table.descent = hhea_descent
-
-    def get_font_info(self) -> dict:
-        """
-        Returns a dictionary of font information
-
-        :return: A dictionary of dictionaries.
-        """
-        head_table: TableHead = self["head"]
-        hhea_table: TableHhea = self["hhea"]
-        name_table: TableName = self["name"]
-        os2_table: TableOS2 = self["OS/2"]
-        post_table: TablePost = self["post"]
-
-        from foundryToolsCLI.Lib.constants import EMBED_LEVEL_STRINGS
-
-        font_info = dict(
-            file_name={"label": "File name", "value": self.reader.file.name},
-            sfnt_versions={
-                "label": "SFNT version",
-                "value": "PostScript" if self.sfntVersion == "OTTO" else "TrueType",
-            },
-            flavor={"label": "Flavor", "value": self.flavor},
-            glyphs_number={
-                "label": "Number of glyphs",
-                "value": self["maxp"].numGlyphs,
-            },
-            family_name={
-                "label": "Family name",
-                "value": name_table.getBestFamilyName(),
-            },
-            subfamily_name={
-                "label": "Subfamily name",
-                "value": name_table.getBestSubFamilyName(),
-            },
-            full_name={
-                "label": "Full name",
-                "value": name_table.getBestFullName(),
-            },
-            postscript_name={
-                "label": "PostScript name",
-                "value": name_table.getDebugName(6),
-            },
-            unique_identifier={
-                "label": "Unique ID",
-                "value": name_table.getDebugName(3),
-            },
-            vendor_code={"label": "Vendor code", "value": os2_table.get_vend_id()},
-            version={
-                "label": "Version",
-                "value": str(round(head_table.get_font_revision(), 3)),
-            },
-            date_created={
-                "label": "Date created",
-                "value": timestampToString(self.created_timestamp),
-            },
-            date_modified={
-                "label": "Date modified",
-                "value": timestampToString(self.modified_timestamp),
-            },
-            us_width_class={
-                "label": "usWidthClass",
-                "value": os2_table.get_width_class(),
-            },
-            us_weight_class={
-                "label": "usWeightClass",
-                "value": os2_table.get_weight_class(),
-            },
-            is_bold={"label": "Font is bold", "value": self.is_bold},
-            is_italic={"label": "Font is italic", "value": self.is_italic},
-            is_oblique={"label": "Font is oblique", "value": self.is_oblique},
-            is_wws_consistent={
-                "label": "WWS consistent",
-                "value": os2_table.is_wws_bit_set(),
-            },
-            use_typo_metrics={
-                "label": "Use Typo Metrics",
-                "value": os2_table.is_use_typo_metrics_bit_set(),
-            },
-            underline_position={
-                "label": "UL position",
-                "value": post_table.underlinePosition,
-            },
-            underline_thickness={
-                "label": "UL thickness",
-                "value": post_table.underlineThickness,
-            },
-            italic_angle={"label": "Italic angle", "value": post_table.italicAngle},
-            caret_slope_rise={
-                "label": "Caret Slope Rise",
-                "value": self["hhea"].caretSlopeRise,
-            },
-            caret_slope_run={
-                "label": "Caret Slope Run",
-                "value": self["hhea"].caretSlopeRun,
-            },
-            caret_offset={"label": "Caret Offset", "value": hhea_table.caretOffset},
-            embed_level={
-                "label": "Embedding",
-                "value": f"{os2_table.get_embed_level()} " f"{EMBED_LEVEL_STRINGS.get(os2_table.get_embed_level())}",
-            },
-        )
-
-        return font_info
-
-    def get_font_v_metrics(self) -> dict:
-        """
-        The function returns a dictionary of dictionaries, where each dictionary contains a list of dictionaries.
-
-        Each of the innermost dictionaries contains a label and a value.
-
-        The label is the name of the metric, and the value is the value of the metric.
-
-        The function returns the following metrics:
-
-        - OS/2 Typographic Ascender
-        - OS/2 Typographic Descender
-        - OS/2 Typographic Line Gap
-        - OS/2 Windows Ascent
-        - OS/2 Windows Descent
-        - hhea Ascent
-        - hhea Descent
-        - hhea Line Gap
-        - head Units Per Em
-        - head xMin
-        - head yMin
-        - head xMax
-        - head yMax
-        - head Font BBox
-
-        The function returns the metrics in a dictionary of dictionaries, where each dictionary contains a list of
-        dictionaries.
-
-        The innermost dictionaries contain a label
-        :return: A dictionary with three keys: os2_metrics, hhea_metrics, and head_metrics.
-        """
-        font_v_metrics = dict(
-            os2_metrics=[
-                {"label": "sTypoAscender", "value": self["OS/2"].sTypoAscender},
-                {"label": "sTypoDescender", "value": self["OS/2"].sTypoDescender},
-                {"label": "sTypoLineGap", "value": self["OS/2"].sTypoLineGap},
-                {"label": "usWinAscent", "value": self["OS/2"].usWinAscent},
-                {"label": "usWinDescent", "value": self["OS/2"].usWinDescent},
-            ],
-            hhea_metrics=[
-                {"label": "ascent", "value": self["hhea"].ascent},
-                {"label": "descent", "value": self["hhea"].descent},
-                {"label": "lineGap", "value": self["hhea"].lineGap},
-            ],
-            head_metrics=[
-                {"label": "unitsPerEm", "value": self["head"].unitsPerEm},
-                {"label": "xMin", "value": self["head"].xMin},
-                {"label": "yMin", "value": self["head"].yMin},
-                {"label": "xMax", "value": self["head"].xMax},
-                {"label": "yMax", "value": self["head"].yMax},
-                {
-                    "label": "Font BBox",
-                    "value": f"({self['head'].xMin}, {self['head'].yMin}) "
-                    f"({self['head'].xMax}, {self['head'].yMax})",
-                },
-            ],
-        )
-
-        return font_v_metrics
-
-    def get_font_feature_tags(self) -> list:
-        """
-        Returns a sorted list of all the feature tags in the font's GSUB and GPOS tables
-
-        :return: A list of feature tags.
-        """
-
-        feature_tags = set()
-        for table_tag in ("GSUB", "GPOS"):
-            if table_tag in self:
-                if not self[table_tag].table.ScriptList or not self[table_tag].table.FeatureList:
-                    continue
-                feature_tags.update(
-                    feature_record.FeatureTag for feature_record in self[table_tag].table.FeatureList.FeatureRecord
-                )
-        return sorted(feature_tags)
-
-    def calculate_italic_angle(self) -> float:
-        """
-        Calculates the italic angle of the font by processing the glyphs "bar" (uni007C), "bracketleft" (uni005B),
-        "H" (uni0048), "I" (uni0049)
-
-        Copied from fontbakery.profiles.post
-
-        :return: The calculated italic angle.
-        """
-
-        # Calculating italic angle from the font's glyph outlines
-        def x_leftmost_intersection(in_paths, y):
-            for y_adjust in range(0, 20, 2):
-                line = Line(Point(xMin - 100, y + y_adjust), Point(xMax + 100, y + y_adjust))
-                for path in in_paths:
-                    for s in path.asSegments():
-                        intersections = s.intersections(line)
-                        if intersections:
-                            return intersections[0].point.x
-
-        calculated_italic_angle = None
-        for glyph_name in (
-            "H",
-            "uni0048",  # LATIN CAPITAL LETTER H
-            "bar",
-            "uni007C",  # VERTICAL LINE
-            "I",
-            "uni0049",  # LATIN CAPITAL LETTER I
-            "bracketleft",
-            "uni005B",  # LEFT SQUARE BRACKET
-        ):
-            try:
-                paths = BezierPath.fromFonttoolsGlyph(self, glyph_name)
-            except KeyError:
-                continue
-
-            # Get bounds
-            bounds_pen = BoundsPen(self.getGlyphSet())
-            self.getGlyphSet()[glyph_name].draw(bounds_pen)
-            (xMin, yMin, xMax, yMax) = bounds_pen.bounds
-
-            # Measure at 20% distance from bottom and top
-            y_bottom = yMin + (yMax - yMin) * 0.2
-            y_top = yMin + (yMax - yMin) * 0.8
-
-            x_intsctn_bottom = x_leftmost_intersection(in_paths=paths, y=y_bottom)
-            x_intsctn_top = x_leftmost_intersection(in_paths=paths, y=y_top)
-
-            # Fails to calculate the intersection for some situations,
-            # so try again with next glyph
-            if not x_intsctn_bottom or not x_intsctn_top:
-                continue
-
-            x_d = x_intsctn_top - x_intsctn_bottom
-            y_d = y_top - y_bottom
-
-            calculated_italic_angle = -1 * math.degrees(math.atan2(x_d, y_d))
-
-        # If the italic angle is < .5, this allows to not set the italic bits when using ftcli fix italic-angle command
-        if abs(calculated_italic_angle) < 0.5:
-            return 0
-        else:
-            return round(calculated_italic_angle)
-
-    def check_italic_angle(self) -> bool:
-        # Allow .1 degrees tolerance
-        return abs(self.calculate_italic_angle() - self["post"].italicAngle) < 0.1
-
-    def calculate_caret_slope_rise(self) -> int:
-        if self["post"].italicAngle == 0:
-            return 1
-        else:
-            return self["head"].unitsPerEm
-
-    def calculate_caret_slope_run(self) -> int:
-        if self["post"].italicAngle == 0:
-            return 0
-        else:
-            return round(math.tan(math.radians(-self["post"].italicAngle)) * self["head"].unitsPerEm)
-
-    def calculate_run_rise_angle(self) -> float:
-        rise = self["hhea"].caretSlopeRise
-        run = self["hhea"].caretSlopeRun
-        run_rise_angle = math.degrees(math.atan(-run / rise))
-        return run_rise_angle
-
-    def calculate_italic_bits(self, mode: int = 1):
-        """
-        If the italic angle is not 0, set the italic and/or oblique bits
-
-        :param mode: click.IntRange(1, 3) = 1, defaults to 1
-        :type mode: click.IntRange(1, 3) (optional)
-        """
-
-        italic_angle = self["post"].italicAngle
-
-        if round(italic_angle) != 0:
-            # Set italic bits only
-            if mode == 1:
-                self.set_italic_flag(True)
-                self.set_oblique_flag(False)
-            # Set italic and oblique bits
-            if mode == 2:
-                self.set_italic_flag(True)
-                self.set_oblique_flag(True)
-            # Set oblique bit only
-            if mode == 3:
-                self.set_oblique_flag(True)
-                self.set_italic_flag(False)
-        else:
-            self.set_italic_flag(False)
-            self.set_oblique_flag(False)
+import math
+import os
+import tempfile
+from pathlib import Path
+
+from beziers.line import Line
+from beziers.path import BezierPath
+from beziers.point import Point
+from fontTools.misc.psCharStrings import T2CharString
+from fontTools.misc.timeTools import timestampToString
+from fontTools.pens.boundsPen import BoundsPen
+from fontTools.ttLib.ttFont import TTFont
+
+from foundryToolsCLI.Lib.tables.hhea import TableHhea
+from foundryToolsCLI.Lib.tables.name import TableName
+from foundryToolsCLI.Lib.tables.OS_2 import TableOS2
+from foundryToolsCLI.Lib.tables.head import TableHead
+from foundryToolsCLI.Lib.tables.post import TablePost
+from foundryToolsCLI.Lib.utils.otf_tools import correct_otf_contours
+from foundryToolsCLI.Lib.utils.ttf_tools import correct_ttf_contours, decomponentize
+
+
+# The Font class is a subclass of the fontTools.ttLib.TTFont class.
+class Font(TTFont):
+    def __init__(self, file=None, recalcBBoxes: bool = True, recalcTimestamp: bool = False, lazy: bool = None):
+        super().__init__(file=file, recalcBBoxes=recalcBBoxes, recalcTimestamp=recalcTimestamp, lazy=lazy)
+
+    @property
+    def is_otf(self) -> bool:
+        """
+        This function checks if the "CFF " table is present in the Font object and returns a boolean
+        value.
+
+        :return: A boolean value indicating whether the font is OpenType-PS.
+        """
+        return "CFF " in self
+
+    @property
+    def is_ttf(self) -> bool:
+        """
+        This function checks if the string "glyf" table is present in the Font object and returns a boolean
+        value.
+
+        :return: A boolean value indicating whether the font is TrueType.
+        """
+        return "glyf" in self
+
+    @property
+    def is_variable(self) -> bool:
+        """
+        This function checks if the "fvar" table is present in the Font object.
+
+        :return: A boolean value indicating whether the font is variable.
+        """
+        return "fvar" in self
+
+    @property
+    def is_static(self) -> bool:
+        """
+        The function checks if the "fvar" table is not present in the Font object.
+
+        :return: A boolean value indicating whether the font is static.
+        """
+        return "fvar" not in self
+
+    @property
+    def is_woff(self) -> bool:
+        """
+        This function checks if the flavor of a font file is "woff" and returns a boolean value.
+
+        :return: A boolean value indicating whether the font flavor is "woff" flavored or not.
+        """
+        return self.flavor == "woff"
+
+    @property
+    def is_woff2(self) -> bool:
+        """
+        This function checks if the flavor of a font file is "woff2" and returns a boolean value.
+
+        :return: A boolean value indicating whether the font is "woff2" flavored or not.
+        """
+        return self.flavor == "woff2"
+
+    @property
+    def is_sfnt(self) -> bool:
+        """
+        This function checks if the font is in SFNT format.
+
+        :return: A boolean value indicating whether the "flavor" attribute of the object is None or not.
+        If it is None, the function will return True, otherwise it will return False.
+        """
+        return self.flavor is None
+
+    @property
+    def is_bold(self) -> bool:
+        """
+        > Checks if OS/2.fsSelection bit 5 and head.macStyle bit 0 are set
+
+        :return: A boolean value.
+        """
+        head: TableHead = self["head"]
+        os_2: TableOS2 = self["OS/2"]
+
+        return head.is_bold_bit_set() and os_2.is_bold_bit_set()
+
+    @property
+    def is_italic(self) -> bool:
+        """
+        > Checks if  OS/2.fsSelection bit 0 and head.macStyle bit 1 are set
+
+        :return: A boolean value.
+        """
+        head: TableHead = self["head"]
+        os_2: TableOS2 = self["OS/2"]
+
+        return head.is_italic_bit_set() and os_2.is_italic_bit_set()
+
+    @property
+    def is_regular(self) -> bool:
+        """
+        > Checks if the fsSelection bit 6 is set, and the bold and italic bits are not set
+
+        :return: A boolean value.
+        """
+        os_2: TableOS2 = self["OS/2"]
+
+        return os_2.is_regular_bit_set() and not self.is_bold and not self.is_italic
+
+    @property
+    def is_oblique(self) -> bool:
+        """
+        > Checks if OS/2.fsSelection bit 9 is set
+
+        :return: A bool value.
+        """
+        os_2: TableOS2 = self["OS/2"]
+
+        return os_2.is_oblique_bit_set()
+
+    @property
+    def is_upright(self) -> bool:
+        """
+        If the font is not italic and not oblique, then it is upright
+
+        :return: A bool value.
+        """
+        return not self.is_italic and not self.is_oblique
+
+    @property
+    def created_timestamp(self) -> int:
+        """
+        This function returns the created timestamp stored in the 'head' table.
+
+        :return: The function `get_created_timestamp` is returning an integer value representing the
+        creation timestamp of the Font object.
+        """
+        return self["head"].created
+
+    @property
+    def modified_timestamp(self) -> int:
+        """
+        This function returns the modified timestamp stored in the "head" table.
+
+        :return: an integer value representing the modified timestamp of the Font object.
+        """
+        return self["head"].modified
+
+    @property
+    def is_hinted_ttf(self) -> bool:
+        return "fpgm" in self and self.is_ttf
+
+    def set_bold_flag(self, value: bool) -> None:
+        """
+        Sets the bold bit in the OS/2 table and the head table, and clears the regular bit in the OS/2 table
+        """
+
+        head: TableHead = self["head"]
+        os_2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os_2.set_bold_bit()
+            head.set_bold_bit()
+            os_2.clear_regular_bit()
+        else:
+            os_2.clear_bold_bit()
+            head.clear_bold_bit()
+            if not self.is_italic:
+                os_2.set_regular_bit()
+
+    def set_italic_flag(self, value: bool) -> None:
+        """
+        Sets the italic bit in the OS/2 table and clears the regular bit
+        """
+        head: TableHead = self["head"]
+        os_2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os_2.set_italic_bit()
+            head.set_italic_bit()
+            os_2.clear_regular_bit()
+        else:
+            os_2.clear_italic_bit()
+            head.clear_italic_bit()
+            if not self.is_bold:
+                os_2.set_regular_bit()
+
+    def set_oblique_flag(self, value: bool) -> None:
+        """
+        Sets the oblique bit in the OS/2 table
+        """
+        os_2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os_2.set_oblique_bit()
+        else:
+            os_2.clear_oblique_bit()
+
+    def set_regular_flag(self, value: bool) -> None:
+        """
+        Sets the regular bit in the OS/2 table, clears the bold and italic bits in the OS/2 and head tables
+        """
+        if self.is_regular:
+            return
+
+        head: TableHead = self["head"]
+        os_2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os_2.set_regular_bit()
+            os_2.clear_bold_bit()
+            os_2.clear_italic_bit()
+            head.clear_bold_bit()
+            head.clear_italic_bit()
+        else:
+            if self.is_bold or self.is_italic:
+                os_2.clear_regular_bit()
+
+    def set_use_typo_metrics_flag(self, value: bool) -> None:
+        os_2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os_2.set_use_typo_metrics_bit()
+        else:
+            os_2.clear_use_typo_metrics_bit()
+
+    def set_wws_consistent_flag(self, value: bool) -> None:
+        os_2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os_2.set_wws_consistent_bit()
+        else:
+            os_2.clear_wws_consistent_bit()
+
+    def set_underscore_flag(self, value: bool) -> None:
+        os_2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os_2.set_underscore_bit()
+        else:
+            os_2.clear_underscore_bit()
+
+    def set_negative_flag(self, value: bool) -> None:
+        os_2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os_2.set_negative_bit()
+        else:
+            os_2.clear_negative_bit()
+
+    def set_outlined_flag(self, value: bool) -> None:
+        os_2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os_2.set_outlined_bit()
+        else:
+            os_2.clear_outlined_bit()
+
+    def set_strikeout_flag(self, value: bool) -> None:
+        os_2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os_2.set_strikeout_bit()
+        else:
+            os_2.clear_strikeout_bit()
+
+    def set_embed_level_flag(self, value: int) -> None:
+        os2: TableOS2 = self["OS/2"]
+
+        os2.set_embed_level(value)
+
+    def set_bitmap_embedding_only_flag(self, value: bool) -> None:
+        os2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os2.set_bitmap_embed_only_bit()
+        else:
+            os2.clear_bitmap_embed_only_bit()
+
+    def set_no_subsetting_flag(self, value: bool) -> None:
+        os_2: TableOS2 = self["OS/2"]
+
+        if value is True:
+            os_2.set_no_subsetting_bit()
+        else:
+            os_2.clear_no_subsetting_bit()
+
+    def get_bounding_box(self):
+        """Returns max and min bbox of the font"""
+        y_min = 0
+        y_max = 0
+        if self.is_otf:
+            y_min = self["head"].yMin
+            y_max = self["head"].yMax
+        else:
+            for g in self["glyf"].glyphs:
+                char = self["glyf"][g]
+                if hasattr(char, "yMin") and y_min > char.yMin:
+                    y_min = char.yMin
+                if hasattr(char, "yMax") and y_max < char.yMax:
+                    y_max = char.yMax
+        return y_min, y_max
+
+    def get_glyph_bounds(self, glyph_name: str) -> dict:
+        glyph_set = self.getGlyphSet()
+        if glyph_set.get(glyph_name) is None:
+            return dict(xMin=0, yMin=0, xMax=0, yMax=0)
+        bounds = T2CharString.calcBounds(glyph_set[glyph_name], glyph_set)
+        if bounds:
+            return dict(xMin=bounds[0], yMin=bounds[1], xMax=bounds[2], yMax=bounds[3])
+        else:
+            return dict(xMin=0, yMin=0, xMax=0, yMax=0)
+
+    def recalc_x_height(self) -> int:
+        return self.get_glyph_bounds("x")["yMax"]
+
+    def recalc_cap_height(self) -> int:
+        return self.get_glyph_bounds("H")["yMax"]
+
+    def recalc_max_context(self) -> int:
+        if self["OS/2"].version >= 2:
+            from fontTools.otlLib.maxContextCalc import maxCtxFont
+
+            max_context = maxCtxFont(self)
+            return max_context
+
+    def set_created_timestamp(self, timestamp: int) -> None:
+        """
+        This function sets the "created" attribute of the "head" table to the given timestamp.
+
+        :param timestamp: an integer representing a Unix timestamp (number of seconds since January 1,
+        1970) that indicates when the font was created
+        :type timestamp: int
+        """
+        self["head"].created = timestamp
+
+    def set_modified_timestamp(self, timestamp: int) -> None:
+        """
+        This function sets the "modified" attribute of the "head" table to the given timestamp.
+
+        :param timestamp: an integer representing a Unix timestamp (number of seconds since January 1,
+        1970) that indicates when the font was last modified
+        :type timestamp: int
+        """
+        self["head"].modified = timestamp
+
+    def get_real_extension(self) -> str:
+        """
+        This function returns the file extension of a font file based on its flavor or type.
+        :return: A string representing the file extension of a font file. If the font has a flavor, the
+        extension will be ".woff" or ".woff2". If the font is a TrueType font, the extension will be
+        ".ttf". If the font is an OpenType font, the extension will be ".otf".
+        """
+        if self.flavor is not None:
+            return f".{self.flavor}"
+        elif self.is_ttf:
+            return ".ttf"
+        elif self.is_otf:
+            return ".otf"
+
+    def ttf_decomponentize(self) -> None:
+        """
+        This function decomponentizes composite glyphs in a TrueType font.
+        """
+        if not self.is_ttf:
+            return
+
+        decomponentize(self)
+
+    def ttf_dehint(self) -> None:
+        """
+        This function de-hints a TrueType font.
+        """
+        if not self.is_ttf:
+            return
+
+        from dehinter.font import dehint
+
+        dehint(tt=self, verbose=False)
+
+    def ttf_remove_overlaps(self, remove_hinting: bool = True, ignore_errors: bool = True):
+        """
+        This function removes overlaps in a TrueType font while optionally ignoring errors and removing
+        hinting.
+
+        :param remove_hinting: A boolean parameter that determines whether to remove hinting
+        information when removing overlaps in the font.
+
+        :type remove_hinting: bool (optional)
+
+        :param ignore_errors: If set to True, any errors encountered during the overlap removal process
+        will be ignored and the process will continue. If set to False, the process will stop and raise
+        an error if any issues are encountered, defaults to True
+
+        :type ignore_errors: bool (optional)
+        """
+        if self.is_otf or self.is_variable:
+            return
+
+        from fontTools.ttLib.removeOverlaps import removeOverlaps
+
+        removeOverlaps(font=self, removeHinting=remove_hinting, ignoreErrors=ignore_errors)
+
+    def ttf_scale_upem(self, units_per_em: int = 1000) -> None:
+        """
+        This function scales the units per em value of a TrueType font.
+
+        :param units_per_em: The units_per_em parameter is an integer value that represents the number
+        of font units-per-em, defaults to 1000
+
+        :type units_per_em: int (optional)
+        """
+        if not self.is_ttf:
+            return
+
+        from fontTools.ttLib.scaleUpem import scale_upem
+
+        if self.is_ttf:
+            self.ttf_dehint()
+        scale_upem(self, new_upem=units_per_em)
+
+    def otf_dehint(self) -> None:
+        """
+        This function removes hints from the CFF table of an OpenType font.
+        """
+        if not self.is_otf:
+            return
+        # noinspection PyUnresolvedReferences
+        from fontTools.subset.cff import remove_hints
+
+        self["CFF "].remove_hints()
+
+    def otf_desubroutinize(self) -> None:
+        """
+        This function removes subroutines from an OpenType font.
+        """
+        if not self.is_otf:
+            return
+
+        from cffsubr import desubroutinize
+
+        flavor = self.flavor
+        self.flavor = None
+        desubroutinize(otf=self)
+        self.flavor = flavor
+
+    def otf_subroutinize(self) -> None:
+        """
+        This function subroutinizes an OpenType font.
+        """
+        if not self.is_otf:
+            return
+
+        from cffsubr import subroutinize
+
+        flavor = self.flavor
+        self.flavor = None
+        subroutinize(otf=self)
+        self.flavor = flavor
+
+    def otf_fix_contours(self, min_area: int = 25, verbose: bool = False) -> None:
+        correct_otf_contours(font=self, min_area=min_area, verbose=verbose)
+
+    def ttf_fix_contours(self, min_area: int = 25, remove_hinting: bool = True, verbose: bool = False) -> None:
+        correct_ttf_contours(self, min_area=min_area, remove_hinting=remove_hinting, verbose=verbose)
+
+    def add_dummy_dsig(self) -> None:
+        """
+        This function adds a dummy DSIG table to a font file if it does not already exist.
+        """
+        if self.flavor == "woff2":
+            return
+
+        from fontTools.ttLib import newTable
+
+        values = dict(
+            ulVersion=1,
+            usFlag=0,
+            usNumSigs=0,
+            signatureRecords=[],
+        )
+        if "DSIG" not in self.keys():
+            dsig = self["DSIG"] = newTable("DSIG")
+            for k, v in values.items():
+                setattr(dsig, k, v)
+
+    def guess_family_name(self) -> str:
+        """
+        This function returns the font's family name, obtained from nameID 21, 16 or 1.
+
+        :return: A string representing the font's family name.
+        """
+        return self["name"].getBestFamilyName()
+
+    def guess_subfamily_name(self) -> str:
+        """
+        This function returns the font's subfamily name, obtained from nameID 22, 17 or 2.
+
+        :return: A string representing the font's subfamily name.
+        """
+        return self["name"].getBestSubFamilyName()
+
+    def get_file_name(self, source) -> str:
+        """
+        Returns the font's file name according to the passed source.
+
+        1: FamilyName-StyleName (FamilyName is retrieved from nameID 21, 16 or 1; SubFamily name from nameID 22,
+        17 or 2)
+
+        2: PostScript Name
+
+        3: Full Font Name
+
+        4: CFF TopDict fontNames. Valid for CFF fonts only. For TTF files will be used
+        '1' as fallback value.
+
+        5: CFF TipDict FullName (returns: Family Name Style Name or FamilyName-StyleName, depending on how FullName has
+        been built). Valid for CFF fonts only. For TTF files will be used '1' as fallback value.
+
+        :param source: The NameRecord or combination of NameRecords from which to build the file name.
+        :return: A string representing the file name of the font.
+        """
+
+        if self.is_ttf:
+            if source in (4, 5):
+                source = 1
+
+        if source == 1:
+            return f"{self.guess_family_name()}-{self.guess_subfamily_name()}".replace(" ", "")
+        elif source == 2:
+            return self["name"].getDebugName(6)
+        elif source == 3:
+            return self["name"].getDebugName(4)
+        elif source == 4:
+            return self["CFF "].cff.fontNames[0]
+        elif source == 5:
+            return self["CFF "].cff.topDictIndex[0].FullName
+        else:
+            return Path(self.reader.file.name).stem
+
+    def fix_cff_top_dict_version(self) -> None:
+        if not self.is_otf:
+            return
+        font_revision = str(round(self["head"].fontRevision, 3)).split(".")
+        major_version = int(font_revision[0])
+        minor_version = int(font_revision[1])
+        cff_font_version = f"{major_version}.{minor_version}"
+        self["CFF "].cff.topDictIndex[0].version = cff_font_version
+
+    def guess_foundry_name(self) -> str:
+        """
+        This function returns the foundry name of a font by checking the "name" or "OS/2" table.
+
+        :return: a string that represents the foundry name. If nameID 8 is present in the "name" table, the Manufacturer
+         Name string is returned. If nameID 8 is not present, but nameID 9 is found, the Designer string is returned.
+         If nor nameID 8 mor nameID 9 are present, the vendor code from the font's OS/2 table is returned. If also the
+         vendor code is empty or not found, "Unknown" is returned.
+        """
+        manufacturer_name: str = self["name"].getDebugName(8)
+        if manufacturer_name:
+            return manufacturer_name
+
+        designer: str = self["name"].getDebugName(9)
+        if designer:
+            return designer
+
+        try:
+            vendor_code: str = self["OS/2"].achVendID
+            if vendor_code.strip().strip("\x00") == "":
+                return "Unknown"
+            else:
+                return vendor_code
+        except KeyError:
+            return "Unknown"
+
+    def make_temp_otf(self) -> tuple[int, Path]:
+        from afdko.fdkutils import run_shell_command
+
+        if self.flavor is None:
+            source_file = self.reader.file.name
+            remove_source_file = False
+        else:
+            self.flavor = None
+            source_fd, source_file = tempfile.mkstemp(suffix=".tmp")
+            self.save(source_file)
+            remove_source_file = True
+            os.close(source_fd)
+
+        temp_t1_fd, temp_t1_file = tempfile.mkstemp(suffix=".t1")
+        temp_otf_fd, temp_otf_file = tempfile.mkstemp(suffix=".otf")
+
+        command_1 = ["tx", "-t1", source_file, temp_t1_file]
+        command_2 = ["makeotf", "-f", temp_t1_file, "-o", temp_otf_file]
+
+        run_shell_command(command_1, suppress_output=True)
+        run_shell_command(command_2, suppress_output=True)
+
+        os.close(temp_t1_fd)
+        os.remove(temp_t1_file)
+        if remove_source_file:
+            os.remove(source_file)
+        return temp_otf_fd, Path(temp_otf_file)
+
+    def get_ui_name_ids(self) -> list:
+        """
+        Returns a list of all the UI name IDs in the font's GSUB table
+
+        :return: A list of integers.
+        """
+        if "GSUB" not in self:
+            return []
+        else:
+            ui_name_ids = []
+            for record in self["GSUB"].table.FeatureList.FeatureRecord:
+                if record.Feature.FeatureParams:
+                    ui_name_ids.append(record.Feature.FeatureParams.UINameID)
+        return sorted(set(ui_name_ids))
+
+    def reorder_ui_name_ids(self):
+        """
+        Takes the IDs of the UI names in the name table and reorders them to start at 256
+        """
+
+        name_table: TableName = self["name"]
+
+        if "GSUB" not in self:
+            return
+        ui_name_ids = self.get_ui_name_ids()
+        for count, value in enumerate(ui_name_ids, start=256):
+            for n in name_table.names:
+                if n.nameID == value:
+                    n.nameID = count
+            for record in self["GSUB"].table.FeatureList.FeatureRecord:
+                if record.Feature.FeatureParams:
+                    if record.Feature.FeatureParams.UINameID == value:
+                        record.Feature.FeatureParams.UINameID = count
+
+    def modify_linegap_percent(self, percent):
+        """
+        Modifies the line spacing metrics
+
+        Adapted from https://github.com/source-foundry/font-line
+        """
+
+        os2_table = self["OS/2"]
+        head_table = self["head"]
+        hhea_table = self["hhea"]
+
+        # get observed start values from the font
+        os2_typo_ascender = os2_table.sTypoAscender
+        os2_typo_descender = os2_table.sTypoDescender
+        os2_typo_linegap = os2_table.sTypoLineGap
+        hhea_ascent = hhea_table.ascent
+        hhea_descent = hhea_table.descent
+        units_per_em = head_table.unitsPerEm
+
+        # calculate necessary delta values
+        os2_typo_ascdesc_delta = os2_typo_ascender + -os2_typo_descender
+        hhea_ascdesc_delta = hhea_ascent + -hhea_descent
+
+        # define percent UPM from command line request
+        factor = 1.0 * int(percent) / 100
+
+        # define line spacing units
+        line_spacing_units = int(factor * units_per_em)
+
+        # define total height as UPM + line spacing units
+        total_height = line_spacing_units + units_per_em
+
+        # height calculations for adjustments
+        delta_height = total_height - hhea_ascdesc_delta
+        upper_lower_add_units = int(0.5 * delta_height)
+
+        # redefine hhea linegap to 0 in all cases
+        hhea_linegap = 0
+
+        # Define metrics based upon original design approach in the font
+        # Google metrics approach
+        if os2_typo_linegap == 0 and (os2_typo_ascdesc_delta > units_per_em):
+            # define values
+            os2_typo_ascender += upper_lower_add_units
+            os2_typo_descender -= upper_lower_add_units
+            hhea_ascent += upper_lower_add_units
+            hhea_descent -= upper_lower_add_units
+            os2_win_ascent = hhea_ascent
+            os2_win_descent = -hhea_descent
+        # Adobe metrics approach
+        elif os2_typo_linegap == 0 and (os2_typo_ascdesc_delta == units_per_em):
+            hhea_ascent += upper_lower_add_units
+            hhea_descent -= upper_lower_add_units
+            os2_win_ascent = hhea_ascent
+            os2_win_descent = -hhea_descent
+        else:
+            os2_typo_linegap = line_spacing_units
+            hhea_ascent = int(os2_typo_ascender + 0.5 * os2_typo_linegap)
+            hhea_descent = -(total_height - hhea_ascent)
+            os2_win_ascent = hhea_ascent
+            os2_win_descent = -hhea_descent
+
+        # define updated values from above calculations
+        hhea_table.lineGap = hhea_linegap
+        os2_table.sTypoAscender = os2_typo_ascender
+        os2_table.sTypoDescender = os2_typo_descender
+        os2_table.sTypoLineGap = os2_typo_linegap
+        os2_table.usWinAscent = os2_win_ascent
+        os2_table.usWinDescent = os2_win_descent
+        hhea_table.ascent = hhea_ascent
+        hhea_table.descent = hhea_descent
+
+    def get_font_info(self) -> dict:
+        """
+        Returns a dictionary of font information
+
+        :return: A dictionary of dictionaries.
+        """
+        head_table: TableHead = self["head"]
+        hhea_table: TableHhea = self["hhea"]
+        name_table: TableName = self["name"]
+        os2_table: TableOS2 = self["OS/2"]
+        post_table: TablePost = self["post"]
+
+        from foundryToolsCLI.Lib.constants import EMBED_LEVEL_STRINGS
+
+        font_info = dict(
+            file_name={"label": "File name", "value": self.reader.file.name},
+            sfnt_versions={
+                "label": "SFNT version",
+                "value": "PostScript" if self.sfntVersion == "OTTO" else "TrueType",
+            },
+            flavor={"label": "Flavor", "value": self.flavor},
+            glyphs_number={
+                "label": "Number of glyphs",
+                "value": self["maxp"].numGlyphs,
+            },
+            family_name={
+                "label": "Family name",
+                "value": name_table.getBestFamilyName(),
+            },
+            subfamily_name={
+                "label": "Subfamily name",
+                "value": name_table.getBestSubFamilyName(),
+            },
+            full_name={
+                "label": "Full name",
+                "value": name_table.getBestFullName(),
+            },
+            postscript_name={
+                "label": "PostScript name",
+                "value": name_table.getDebugName(6),
+            },
+            unique_identifier={
+                "label": "Unique ID",
+                "value": name_table.getDebugName(3),
+            },
+            vendor_code={"label": "Vendor code", "value": os2_table.get_vend_id()},
+            version={
+                "label": "Version",
+                "value": str(round(head_table.get_font_revision(), 3)),
+            },
+            date_created={
+                "label": "Date created",
+                "value": timestampToString(self.created_timestamp),
+            },
+            date_modified={
+                "label": "Date modified",
+                "value": timestampToString(self.modified_timestamp),
+            },
+            us_width_class={
+                "label": "usWidthClass",
+                "value": os2_table.get_width_class(),
+            },
+            us_weight_class={
+                "label": "usWeightClass",
+                "value": os2_table.get_weight_class(),
+            },
+            is_bold={"label": "Font is bold", "value": self.is_bold},
+            is_italic={"label": "Font is italic", "value": self.is_italic},
+            is_oblique={"label": "Font is oblique", "value": self.is_oblique},
+            is_wws_consistent={
+                "label": "WWS consistent",
+                "value": os2_table.is_wws_bit_set(),
+            },
+            use_typo_metrics={
+                "label": "Use Typo Metrics",
+                "value": os2_table.is_use_typo_metrics_bit_set(),
+            },
+            underline_position={
+                "label": "UL position",
+                "value": post_table.underlinePosition,
+            },
+            underline_thickness={
+                "label": "UL thickness",
+                "value": post_table.underlineThickness,
+            },
+            italic_angle={"label": "Italic angle", "value": post_table.italicAngle},
+            caret_slope_rise={
+                "label": "Caret Slope Rise",
+                "value": self["hhea"].caretSlopeRise,
+            },
+            caret_slope_run={
+                "label": "Caret Slope Run",
+                "value": self["hhea"].caretSlopeRun,
+            },
+            caret_offset={"label": "Caret Offset", "value": hhea_table.caretOffset},
+            embed_level={
+                "label": "Embedding",
+                "value": f"{os2_table.get_embed_level()} " f"{EMBED_LEVEL_STRINGS.get(os2_table.get_embed_level())}",
+            },
+        )
+
+        return font_info
+
+    def get_font_v_metrics(self) -> dict:
+        """
+        The function returns a dictionary of dictionaries, where each dictionary contains a list of dictionaries.
+
+        Each of the innermost dictionaries contains a label and a value.
+
+        The label is the name of the metric, and the value is the value of the metric.
+
+        The function returns the following metrics:
+
+        - OS/2 Typographic Ascender
+        - OS/2 Typographic Descender
+        - OS/2 Typographic Line Gap
+        - OS/2 Windows Ascent
+        - OS/2 Windows Descent
+        - hhea Ascent
+        - hhea Descent
+        - hhea Line Gap
+        - head Units Per Em
+        - head xMin
+        - head yMin
+        - head xMax
+        - head yMax
+        - head Font BBox
+
+        The function returns the metrics in a dictionary of dictionaries, where each dictionary contains a list of
+        dictionaries.
+
+        The innermost dictionaries contain a label
+        :return: A dictionary with three keys: os2_metrics, hhea_metrics, and head_metrics.
+        """
+        font_v_metrics = dict(
+            os2_metrics=[
+                {"label": "sTypoAscender", "value": self["OS/2"].sTypoAscender},
+                {"label": "sTypoDescender", "value": self["OS/2"].sTypoDescender},
+                {"label": "sTypoLineGap", "value": self["OS/2"].sTypoLineGap},
+                {"label": "usWinAscent", "value": self["OS/2"].usWinAscent},
+                {"label": "usWinDescent", "value": self["OS/2"].usWinDescent},
+            ],
+            hhea_metrics=[
+                {"label": "ascent", "value": self["hhea"].ascent},
+                {"label": "descent", "value": self["hhea"].descent},
+                {"label": "lineGap", "value": self["hhea"].lineGap},
+            ],
+            head_metrics=[
+                {"label": "unitsPerEm", "value": self["head"].unitsPerEm},
+                {"label": "xMin", "value": self["head"].xMin},
+                {"label": "yMin", "value": self["head"].yMin},
+                {"label": "xMax", "value": self["head"].xMax},
+                {"label": "yMax", "value": self["head"].yMax},
+                {
+                    "label": "Font BBox",
+                    "value": f"({self['head'].xMin}, {self['head'].yMin}) "
+                    f"({self['head'].xMax}, {self['head'].yMax})",
+                },
+            ],
+        )
+
+        return font_v_metrics
+
+    def get_font_feature_tags(self) -> list:
+        """
+        Returns a sorted list of all the feature tags in the font's GSUB and GPOS tables
+
+        :return: A list of feature tags.
+        """
+
+        feature_tags = set()
+        for table_tag in ("GSUB", "GPOS"):
+            if table_tag in self:
+                if not self[table_tag].table.ScriptList or not self[table_tag].table.FeatureList:
+                    continue
+                feature_tags.update(
+                    feature_record.FeatureTag for feature_record in self[table_tag].table.FeatureList.FeatureRecord
+                )
+        return sorted(feature_tags)
+
+    def calculate_italic_angle(self) -> float:
+        """
+        Calculates the italic angle of the font by processing the glyphs "bar" (uni007C), "bracketleft" (uni005B),
+        "H" (uni0048), "I" (uni0049)
+
+        Copied from fontbakery.profiles.post
+
+        :return: The calculated italic angle.
+        """
+
+        # Calculating italic angle from the font's glyph outlines
+        def x_leftmost_intersection(in_paths, y):
+            for y_adjust in range(0, 20, 2):
+                line = Line(Point(xMin - 100, y + y_adjust), Point(xMax + 100, y + y_adjust))
+                for path in in_paths:
+                    for s in path.asSegments():
+                        intersections = s.intersections(line)
+                        if intersections:
+                            return intersections[0].point.x
+
+        calculated_italic_angle = None
+        for glyph_name in (
+            "H",
+            "uni0048",  # LATIN CAPITAL LETTER H
+            "bar",
+            "uni007C",  # VERTICAL LINE
+            "I",
+            "uni0049",  # LATIN CAPITAL LETTER I
+            "bracketleft",
+            "uni005B",  # LEFT SQUARE BRACKET
+        ):
+            try:
+                paths = BezierPath.fromFonttoolsGlyph(self, glyph_name)
+            except KeyError:
+                continue
+
+            # Get bounds
+            bounds_pen = BoundsPen(self.getGlyphSet())
+            self.getGlyphSet()[glyph_name].draw(bounds_pen)
+            (xMin, yMin, xMax, yMax) = bounds_pen.bounds
+
+            # Measure at 20% distance from bottom and top
+            y_bottom = yMin + (yMax - yMin) * 0.2
+            y_top = yMin + (yMax - yMin) * 0.8
+
+            x_intsctn_bottom = x_leftmost_intersection(in_paths=paths, y=y_bottom)
+            x_intsctn_top = x_leftmost_intersection(in_paths=paths, y=y_top)
+
+            # Fails to calculate the intersection for some situations,
+            # so try again with next glyph
+            if not x_intsctn_bottom or not x_intsctn_top:
+                continue
+
+            x_d = x_intsctn_top - x_intsctn_bottom
+            y_d = y_top - y_bottom
+
+            calculated_italic_angle = -1 * math.degrees(math.atan2(x_d, y_d))
+
+        # If the italic angle is < .5, this allows to not set the italic bits when using ftcli fix italic-angle command
+        if abs(calculated_italic_angle) < 0.5:
+            return 0
+        else:
+            return round(calculated_italic_angle)
+
+    def check_italic_angle(self) -> bool:
+        # Allow .1 degrees tolerance
+        return abs(self.calculate_italic_angle() - self["post"].italicAngle) < 0.1
+
+    def calculate_caret_slope_rise(self) -> int:
+        if self["post"].italicAngle == 0:
+            return 1
+        else:
+            return self["head"].unitsPerEm
+
+    def calculate_caret_slope_run(self) -> int:
+        if self["post"].italicAngle == 0:
+            return 0
+        else:
+            return round(math.tan(math.radians(-self["post"].italicAngle)) * self["head"].unitsPerEm)
+
+    def calculate_run_rise_angle(self) -> float:
+        rise = self["hhea"].caretSlopeRise
+        run = self["hhea"].caretSlopeRun
+        run_rise_angle = math.degrees(math.atan(-run / rise))
+        return run_rise_angle
+
+    def calculate_italic_bits(self, mode: int = 1):
+        """
+        If the italic angle is not 0, set the italic and/or oblique bits
+
+        :param mode: click.IntRange(1, 3) = 1, defaults to 1
+        :type mode: click.IntRange(1, 3) (optional)
+        """
+
+        italic_angle = self["post"].italicAngle
+
+        if round(italic_angle) != 0:
+            # Set italic bits only
+            if mode == 1:
+                self.set_italic_flag(True)
+                self.set_oblique_flag(False)
+            # Set italic and oblique bits
+            if mode == 2:
+                self.set_italic_flag(True)
+                self.set_oblique_flag(True)
+            # Set oblique bit only
+            if mode == 3:
+                self.set_oblique_flag(True)
+                self.set_italic_flag(False)
+        else:
+            self.set_italic_flag(False)
+            self.set_oblique_flag(False)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/VFont.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/VFont.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,61 @@
-import os
-from pathlib import Path
-
-from fontTools.ttLib.tables._f_v_a_r import NamedInstance, Axis
-
-from foundryToolsCLI.Lib.Font import Font
-
-
-class VariableFont(Font):
-    def __init__(self, file=None, recalcTimestamp=False):
-        super().__init__(file=file, recalcTimestamp=recalcTimestamp)
-
-    def get_axes(self) -> list[Axis]:
-        return [axis for axis in self["fvar"].axes if axis.flags == 0]
-
-    def get_instances(self) -> list[NamedInstance]:
-        return [instance for instance in self["fvar"].instances]
-
-    def get_var_name_ids_to_delete(self) -> list:
-        name_ids_to_delete = [25]
-
-        if "fvar" in self.keys():
-            for axis in self.get_axes():
-                name_ids_to_delete.append(axis.axisNameID)
-            for instance in self.get_instances():
-                if hasattr(instance, "subfamilyNameID"):
-                    name_ids_to_delete.append(instance.subfamilyNameID)
-                if hasattr(instance, "postscriptNameID"):
-                    name_ids_to_delete.append(instance.postscriptNameID)
-
-        if "STAT" in self.keys():
-            if hasattr(self["STAT"].table, "DesignAxisRecord"):
-                for axis in self["STAT"].table.DesignAxisRecord.Axis:
-                    name_ids_to_delete.append(axis.AxisNameID)
-            if hasattr(self["STAT"].table, "AxisValueArray") and self["STAT"].table.AxisValueArray is not None:
-                for axis in self["STAT"].table.AxisValueArray.AxisValue:
-                    name_ids_to_delete.append(axis.ValueNameID)
-
-        name_ids_to_delete = [n for n in name_ids_to_delete if n > 24]
-        name_ids_to_delete = sorted(list(set(name_ids_to_delete)))
-
-        return name_ids_to_delete
-
-    def get_instance_file_name(self, instance: NamedInstance) -> str:
-        if hasattr(instance, "postscriptNameID") and instance.postscriptNameID < 65535:
-            instance_file_name = self["name"].getDebugName(instance.postscriptNameID)
-
-        else:
-            if hasattr(instance, "subfamilyNameID") and instance.subfamilyNameID > 0:
-                subfamily_name = self["name"].getDebugName(instance.subfamilyNameID)
-            else:
-                subfamily_name = "_".join([f"{k}_{v}" for k, v in instance.coordinates.items()])
-
-            if self["name"].getBestFamilyName() is not None:
-                family_name = self["name"].getBestFamilyName()
-            else:
-                file = Path(self.reader.file.name)
-                family_name = file.stem
-
-            instance_file_name = f"{family_name}-{subfamily_name}".replace(" ", "")
-
-        return instance_file_name
+from pathlib import Path
+
+from fontTools.ttLib.tables._f_v_a_r import NamedInstance, Axis
+
+from foundryToolsCLI.Lib.Font import Font
+
+
+class VariableFont(Font):
+    def __init__(self, file=None, recalcTimestamp=False):
+        super().__init__(file=file, recalcTimestamp=recalcTimestamp)
+
+    def get_axes(self) -> list[Axis]:
+        return [axis for axis in self["fvar"].axes if axis.flags == 0]
+
+    def get_instances(self) -> list[NamedInstance]:
+        return [instance for instance in self["fvar"].instances]
+
+    def get_var_name_ids_to_delete(self) -> list:
+        name_ids_to_delete = [25]
+
+        if "fvar" in self.keys():
+            for axis in self.get_axes():
+                name_ids_to_delete.append(axis.axisNameID)
+            for instance in self.get_instances():
+                if hasattr(instance, "subfamilyNameID"):
+                    name_ids_to_delete.append(instance.subfamilyNameID)
+                if hasattr(instance, "postscriptNameID"):
+                    name_ids_to_delete.append(instance.postscriptNameID)
+
+        if "STAT" in self.keys():
+            if hasattr(self["STAT"].table, "DesignAxisRecord"):
+                for axis in self["STAT"].table.DesignAxisRecord.Axis:
+                    name_ids_to_delete.append(axis.AxisNameID)
+            if hasattr(self["STAT"].table, "AxisValueArray") and self["STAT"].table.AxisValueArray is not None:
+                for axis in self["STAT"].table.AxisValueArray.AxisValue:
+                    name_ids_to_delete.append(axis.ValueNameID)
+
+        name_ids_to_delete = [n for n in name_ids_to_delete if n > 24]
+        name_ids_to_delete = sorted(list(set(name_ids_to_delete)))
+
+        return name_ids_to_delete
+
+    def get_instance_file_name(self, instance: NamedInstance) -> str:
+        if hasattr(instance, "postscriptNameID") and instance.postscriptNameID < 65535:
+            instance_file_name = self["name"].getDebugName(instance.postscriptNameID)
+
+        else:
+            if hasattr(instance, "subfamilyNameID") and instance.subfamilyNameID > 0:
+                subfamily_name = self["name"].getDebugName(instance.subfamilyNameID)
+            else:
+                subfamily_name = "_".join([f"{k}_{v}" for k, v in instance.coordinates.items()])
+
+            if self["name"].getBestFamilyName() is not None:
+                family_name = self["name"].getBestFamilyName()
+            else:
+                file = Path(self.reader.file.name)
+                family_name = file.stem
+
+            instance_file_name = f"{family_name}-{subfamily_name}".replace(" ", "")
+
+        return instance_file_name
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/assistant/UI.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/UI.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,609 +1,607 @@
-import os.path
-import sys
-from pathlib import Path
-
-import click
-from rich import box
-from rich.console import Console
-from rich.table import Table
-from rich.tree import Tree
-
-from foundryToolsCLI.Lib.Font import Font
-from foundryToolsCLI.Lib.assistant.fonts_data import FontsData
-from foundryToolsCLI.Lib.assistant.styles_mapping import (
-    StylesMapping,
-    DEFAULT_WEIGHTS,
-    DEFAULT_WIDTHS,
-)
-from foundryToolsCLI.Lib.utils.cli_tools import (
-    get_style_mapping_path,
-    get_fonts_data_path,
-    get_fonts_in_path,
-)
-from foundryToolsCLI.Lib.utils.click_tools import generic_error_message, no_valid_fonts_message, OptionalParamType
-
-CWD = Path.cwd()
-
-
-class AssistantUI(object):
-    def __init__(self, input_path: Path):
-        self.input_path = input_path
-
-        if len(self.fonts_list) == 0:
-            no_valid_fonts_message(input_path.relative_to(CWD))
-            sys.exit()
-
-        self.styles_mapping = StylesMapping(get_style_mapping_path(self.input_path))
-        if not os.path.exists(self.styles_mapping.file):
-            self.styles_mapping.reset_defaults()
-
-        self.fonts_data = FontsData(get_fonts_data_path(self.input_path))
-        if not os.path.exists(self.fonts_data.file):
-            self.fonts_data.reset_data(styles_mapping=self.styles_mapping)
-
-        self.console = Console()
-
-    def run(self):
-        click.clear()
-        self.console.set_window_title("ftCLI assistant UI")
-        self.fonts_data_editor()
-
-    def styles_mapping_editor(self):
-        click.clear()
-        table = self.__get_styles_mapping_table()
-        commands = {
-            "g": "Edit Weights",
-            "t": "Edit Widths",
-            "i": "Edit Italics",
-            "o": "Edit Obliques",
-            "r": "Reset defaults",
-            "x": "Exit",
-        }
-        self.console.print(table)
-
-        command = self.__prompt_for_command(commands)
-        if command == "g":
-            self.__widths_weights_editor(key="weights")
-        if command == "t":
-            self.__widths_weights_editor(key="widths")
-        if command == "i":
-            self.__set_slope(key="italics")
-        if command == "o":
-            self.__set_slope(key="obliques")
-        if command == "r":
-            if self.__prompt_for_confirmation(text="Reset default values?"):
-                self.styles_mapping.reset_defaults()
-        if command == "x":
-            return
-
-        self.styles_mapping_editor()
-
-    def fonts_data_editor(self):
-        fonts_data = self.fonts_data.get_data()
-
-        commands = {
-            "m": "Edit Styles Mapping",
-            "s": "Select files",
-            "d": "Deselect files",
-            "f": "Set Family Name",
-            "i": "Set/Unset Italic",
-            "o": "Set/Unset Oblique",
-            "t": "Set Width",
-            "g": "Set Weight",
-            "l": "Set Slope",
-            "r": "Reset data",
-            "c": "Recalc data",
-            "x": "Exit",
-        }
-        table = self.__get_fonts_data_table()
-
-        click.clear()
-        self.console.print(table)
-
-        command = self.__prompt_for_command(commands)
-        if command == "m":
-            self.styles_mapping_editor()
-        if command == "s":
-            self.__select_deselect_files(action="select")
-        if command == "d":
-            self.__select_deselect_files(action="deselect")
-        if command == "f":
-            family_name = click.prompt("Family name")
-            if self.__prompt_for_confirmation():
-                for row in fonts_data:
-                    if row["selected"] == "1":
-                        row["family_name"] = family_name
-                self.fonts_data.save(fonts_data)
-        if command == "i":
-            italic_value = click.prompt(
-                f"Italic value {click.style('[0/1]', bold=True, fg='cyan')}",
-                type=click.Choice(choices=("0", "1")),
-                show_choices=False,
-            )
-            if self.__prompt_for_confirmation():
-                for row in fonts_data:
-                    if row["selected"] == "1":
-                        row["is_italic"] = italic_value
-                self.fonts_data.save(fonts_data)
-        if command == "o":
-            oblique_value = click.prompt(
-                f"Oblique value {click.style('[0/1]', bold=True, fg='cyan')}",
-                type=click.Choice(choices=("0", "1")),
-                show_choices=False,
-            )
-            if self.__prompt_for_confirmation():
-                for row in fonts_data:
-                    if row["selected"] == "1":
-                        row["is_oblique"] = oblique_value
-                self.fonts_data.save(fonts_data)
-        if command == "t":
-            us_width_class = click.prompt(
-                f"usWidthClass {click.style('[1-9]', bold=True, fg='cyan')} (Enter  to skip)",
-                type=OptionalParamType(click.IntRange(1, 9)),
-                default="",
-                show_default=False,
-            )
-            wdt = click.prompt(
-                "Short word (Enter to skip)",
-                type=OptionalParamType(click.STRING),
-                default="",
-                show_default=False,
-            )
-            width = click.prompt(
-                "Long word (Enter to skip)",
-                type=OptionalParamType(click.STRING),
-                default="",
-                show_default=False,
-            )
-
-            if self.__prompt_for_confirmation():
-                for row in fonts_data:
-                    if row["selected"] == "1":
-                        row["us_width_class"] = us_width_class if us_width_class else row["us_width_class"]
-                        words = [
-                            wdt if wdt else row["wdt"],
-                            width if width else row["width"],
-                        ]
-                        words.sort(key=len)
-                        row["wdt"] = words[0]
-                        row["width"] = words[1]
-                self.fonts_data.save(fonts_data)
-        if command == "g":
-            us_weight_class = click.prompt(
-                f"usWeightClass {click.style('[1-1000]', bold=True, fg='cyan')} " f"(Enter to skip)",
-                type=OptionalParamType(click.IntRange(1, 1000)),
-                default="",
-                show_default=False,
-            )
-            wgt = click.prompt(
-                "Short word (Enter to skip)",
-                type=OptionalParamType(click.STRING),
-                default="",
-                show_default=False,
-            )
-            weight = click.prompt(
-                "Long word (Enter to skip)",
-                type=OptionalParamType(click.STRING),
-                default="",
-                show_default=False,
-            )
-
-            if self.__prompt_for_confirmation():
-                for row in fonts_data:
-                    if row["selected"] == "1":
-                        if us_weight_class:
-                            row["us_weight_class"] = us_weight_class
-                        words = [
-                            wgt if wgt else row["wgt"],
-                            weight if weight else row["weight"],
-                        ]
-                        words.sort(key=len)
-                        row["wgt"] = words[0]
-                        row["weight"] = words[1]
-                self.fonts_data.save(fonts_data)
-        if command == "l":
-            slp = click.prompt(
-                "Short word (Enter to skip)",
-                type=OptionalParamType(click.STRING),
-                default="",
-                show_default=False,
-            )
-            slope = click.prompt(
-                "Long word (Enter to skip)",
-                type=OptionalParamType(click.STRING),
-                default="",
-                show_default=False,
-            )
-            if self.__prompt_for_confirmation():
-                for row in fonts_data:
-                    if row["selected"] == "1":
-                        words = [
-                            slp if slp else row["slp"],
-                            slope if slope else row["slope"],
-                        ]
-                        words.sort(key=len)
-                        row["slp"] = words[0]
-                        row["slope"] = words[1]
-                self.fonts_data.save(fonts_data)
-        if command == "r":
-            if self.__prompt_for_confirmation(text="Reset data?"):
-                self.fonts_data.reset_data(styles_mapping=self.styles_mapping)
-        if command == "c":
-            click.echo("\nPlease, select the string to use to recalculate data")
-            click.secho("[0]", bold=True, fg="cyan", nl=False)
-            click.echo(" : File Name")
-            click.secho("[1]", bold=True, fg="cyan", nl=False)
-            click.echo(" : PostScript Name")
-            click.secho("[2]", bold=True, fg="cyan", nl=False)
-            click.echo(" : Family Name + SubFamily Name")
-            click.secho("[3]", bold=True, fg="cyan", nl=False)
-            click.echo(" : Full Font Name")
-            click.secho("[4]", bold=True, fg="cyan", nl=False)
-            click.echo(" : CFF fontNames")
-            click.secho("[5]", bold=True, fg="cyan", nl=False)
-            click.echo(" : CFF FullName")
-            source_type = self.__prompt_for_int_range("Your selection", min_value=0, max_value=5, default=0)
-            if self.__prompt_for_confirmation(text="Recalc data?"):
-                self.fonts_data.recalc_data(source_type=source_type, styles_mapping=self.styles_mapping)
-
-        if command == "x":
-            return
-
-        self.fonts_data_editor()
-
-    def __widths_weights_editor(self, key: str):
-        if key == "weights":
-            max_value = 1000
-            defaults = DEFAULT_WEIGHTS
-        elif key == "widths":
-            max_value = 9
-            defaults = DEFAULT_WIDTHS
-        else:
-            return
-
-        data = self.styles_mapping.get_data()
-        table = self.__get_widths_weights_table(key)
-
-        commands = {
-            "a": "Add/edit item",
-            "d": "Delete item",
-            "r": "Reset defaults",
-            "x": "Exit",
-        }
-
-        click.clear()
-        self.console.print(table)
-        command = self.__prompt_for_command(commands)
-
-        if command == "a":
-            self.__add_width_weight(key=key, max_value=max_value)
-        if command == "d":
-            choices = [k for k in data[key].keys()]
-            value = click.prompt(
-                f"Value to delete {click.style('[' + ', '.join(choices) + ']', bold=True, fg='cyan')}",
-                type=click.Choice(choices=choices),
-                show_choices=False,
-            )
-            if self.__prompt_for_confirmation():
-                del data[key][value]
-                self.styles_mapping.save(data)
-        if command == "r":
-            if self.__prompt_for_confirmation(text="Reset default values?"):
-                data[key] = defaults
-                self.styles_mapping.save(data)
-        if command == "x":
-            return
-
-        self.__widths_weights_editor(key)
-
-    def __select_deselect_files(self, action):
-        data = self.fonts_data.get_data()
-
-        start = self.__prompt_for_int_range(text="From line", min_value=1, max_value=len(data), default=1)
-        end = self.__prompt_for_int_range(text="To line", min_value=start, max_value=len(data), default=len(data))
-
-        for i in range(start - 1, end):
-            if action == "select":
-                data[i]["selected"] = 1
-            if action == "deselect":
-                data[i]["selected"] = 0
-        self.fonts_data.save(data)
-
-    def __get_fonts_data_table(self) -> Table:
-        data = self.fonts_data.get_data()
-
-        table = Table(
-            title="ftCLI Assistant - Fonts Data Editor",
-            title_style="bold green",
-            header_style="bold cyan",
-            caption=self.fonts_data.file.as_posix(),
-            box=box.HORIZONTALS,
-        )
-
-        table.add_column("#", justify="right")
-        table.add_column("[+]")
-        table.add_column("File name")
-        table.add_column("Family name")
-        table.add_column("B")
-        table.add_column("I")
-        table.add_column("O")
-        table.add_column("Width")
-        table.add_column("Weight")
-        table.add_column("Slope")
-
-        for count, row in enumerate(data, start=1):
-            if row["selected"] == "1":
-                selected_string = "[bold cyan][+]"
-            else:
-                selected_string = "[ ]"
-            file_name = row["file_name"]
-            family_name = row["family_name"]
-            is_bold = row["is_bold"]
-            is_italic = row["is_italic"]
-            is_oblique = row["is_oblique"]
-            width = f"{row['us_width_class']} : {row['wdt']}, {row['width']}"
-            weight = f"{row['us_weight_class']} : {row['wgt']}, {row['weight']}"
-            if (row["slp"], row["slope"]) == ("", ""):
-                slope = ""
-            else:
-                slope = ", ".join([row["slp"], row["slope"]])
-
-            table.add_row(
-                str(count),
-                selected_string,
-                os.path.basename(file_name),
-                family_name,
-                is_bold,
-                is_italic,
-                is_oblique,
-                width,
-                weight,
-                slope,
-            )
-
-        return table
-
-    def __get_styles_mapping_table(self) -> Table:
-        """
-        Returns a Table object of the styles mapping
-        """
-        data = self.styles_mapping.get_data()
-
-        table = Table(
-            show_header=False,
-            title="ftCLI Assistant - Styles Mapping Editor",
-            title_style="bold green",
-            caption=self.styles_mapping.file.as_posix(),
-            box=box.HORIZONTALS,
-        )
-
-        table.add_row("Weight", "Short word", "Long word", style="bright_cyan", end_section=True)
-        for k, v in data["weights"].items():
-            table.add_row(k, v[0], v[1])
-        table.add_section()
-        table.add_row("Width", "Short word", "Long word", style="bright_cyan", end_section=True)
-        for k, v in data["widths"].items():
-            table.add_row(k, v[0], v[1])
-        table.add_section()
-        table.add_row("Slope", "Short word", "Long word", style="bright_cyan", end_section=True)
-        table.add_row("Italic", data["italics"][0], data["italics"][1])
-        table.add_row("Oblique", data["obliques"][0], data["obliques"][1])
-
-        return table
-
-    def __get_widths_weights_table(self, key) -> Table:
-        data = self.styles_mapping.get_data()
-        table = Table(
-            show_header=False,
-            title=f"ftCLI Assistant - {key.capitalize()} Editor",
-            title_style="bold green",
-            box=box.HORIZONTALS,
-        )
-        table.add_row(
-            f"{key[0:-1]}".capitalize(),
-            "Short word",
-            "Long word",
-            style="bold cyan",
-            end_section=True,
-        )
-        for k, v in data[key].items():
-            table.add_row(k, v[0], v[1])
-        table.add_section()
-
-        return table
-
-    def __add_width_weight(self, key: str, max_value: int):
-        data = self.styles_mapping.get_data()
-        value = str(self.__prompt_for_int_range(text="Value", min_value=1, max_value=max_value))
-
-        defaults = [None, None]
-        if value in data[key].keys():
-            defaults = data[key].get(value)
-            new_value = str(
-                self.__prompt_for_int_range(
-                    text="New value",
-                    min_value=1,
-                    max_value=max_value,
-                    default=int(value),
-                )
-            )
-            del data[key][value]
-            value = new_value
-
-        short_word = click.prompt(
-            f"Short word " f"{click.style(f'[{defaults[0]}]', bold=True, fg='cyan') if defaults[0] else ''}",
-            default=defaults[0],
-            show_default=False,
-        )
-        long_word = click.prompt(
-            f"Long word  " f"{click.style(f'[{defaults[1]}]', bold=True, fg='cyan') if defaults[1] else ''}",
-            default=defaults[1],
-            show_default=False,
-        )
-
-        if self.__prompt_for_confirmation():
-            # del data[key][value]
-            data[key][value] = sorted([short_word, long_word], key=len)
-            self.styles_mapping.save(data)
-
-    def __set_slope(self, key: str):
-        data = self.styles_mapping.get_data()
-
-        short_word = click.prompt(
-            f"Short word{click.style(f' [{data[key][0]}]', bold=True, fg='cyan')}",
-            default=data[key][0],
-            show_default=False,
-        )
-        long_word = click.prompt(
-            f"Long word{click.style(f' [{data[key][1]}]', bold=True, fg='cyan')}",
-            default=data[key][1],
-            show_default=False,
-        )
-
-        data[key] = sorted([short_word, long_word], key=len)
-
-        if self.__prompt_for_confirmation():
-            self.styles_mapping.save(data)
-
-    @staticmethod
-    def __prompt_for_command(commands: dict) -> str:
-        click.secho("\nAVAILABLE COMMANDS:\n", bold=True, fg="green")
-        for k, v in commands.items():
-            click.secho(f" {click.style(k, bold=True, fg='cyan')} : ", nl=False)
-            click.secho(f"{v} ", nl=True)
-
-        choices = [k for k in commands.keys()]
-        # command = click.prompt(f"\nSelect command [{click.style(', '.join(choices), bold=True, fg='cyan')}]",
-        command = click.prompt(
-            "\nSelect command",
-            type=click.Choice(choices=choices, case_sensitive=False),
-            show_choices=False,
-            show_default=False,
-            err=True,
-        )
-        return command
-
-    @staticmethod
-    def __prompt_for_int_range(
-        text: str,
-        min_value: int,
-        max_value: int,
-        default: int = None,
-        bold: bool = True,
-        fg_color: str = "cyan",
-    ) -> int:
-        """
-        > Prompt the user for an integer value within a specified range, and return the value as a string
-
-        :param text: The text to display to the user
-        :type text: str
-        :param min_value: The minimum value that the user can enter
-        :type min_value: int
-        :param max_value: The maximum value that the user can enter
-        :type max_value: int
-        :param default: The default value to use if no input happens. If a default value is given, it is shown in square
-            brackets in place of the min-max range
-        :type default: int
-        :param bold: bool = True, defaults to True
-        :type bold: bool (optional)
-        :param fg_color: The color of the highlighted text, defaults to cyan
-        :type fg_color: str (optional)
-        :return: An integer
-        """
-        highlighted_text = click.style(
-            f"[{default}]" if default is not None else f"[{min_value}-{max_value}]",
-            bold=bold,
-            fg=fg_color,
-        )
-        message = f"{text} {highlighted_text}"
-        value = click.prompt(
-            message,
-            type=click.IntRange(min_value, max_value),
-            default=default,
-            show_default=False,
-        )
-        return value
-
-    @staticmethod
-    def __prompt_for_confirmation(text="Save changes?") -> bool:
-        """
-        > Prompt the user for a yes/no confirmation, and return a boolean value
-
-        :param text: The text to display to the user, defaults to Save changes? (optional)
-        :return: A boolean value
-        """
-        return click.confirm(
-            f"{text} {click.style('[Y/n]', bold=True, fg='cyan')}",
-            default=True,
-            show_default=False,
-        )
-
-    @property
-    def fonts_list(self) -> list[Font]:
-        return get_fonts_in_path(self.input_path)
-
-
-def get_commands_tree(commands: dict) -> Tree:
-    """
-    Takes a dictionary of commands and returns a Tree object
-
-    :param commands: the dictionary of commands
-    :type commands: dict
-    :return: A Tree object with the label "COMMANDS" and the style "green"
-    """
-    commands_tree = Tree(label="COMMANDS", style="green", guide_style="green")
-    for k, v in commands.items():
-        commands_tree.add(f"[bold green]{k}[reset] : [bold cyan]{v}")
-    return commands_tree
-
-
-def get_fonts_rows(fonts: list[Font]) -> list:
-    rows = []
-    for font in fonts:
-        try:
-            row = dict(
-                file_name=os.path.basename(font.reader.file.name),
-                family_name=font["name"].getBestFamilyName(),
-                subfamily_name=font["name"].getBestSubFamilyName(),
-                us_width_class=str(font["OS/2"].usWidthClass),
-                us_weight_class=str(font["OS/2"].usWeightClass),
-                is_bold=str(int(font.is_bold)),
-                is_italic=str(int(font.is_italic)),
-                is_oblique=str(int(font.is_oblique)),
-                is_regular=str(int(font.is_regular)),
-            )
-            rows.append(row)
-        except Exception as e:
-            generic_error_message(e)
-    return rows
-
-
-def get_fonts_list_table(rows: list) -> Table:
-    table = Table(box=box.HORIZONTALS)
-
-    table.add_column("#", justify="right")
-    table.add_column("File name")
-    table.add_column("Family name")
-    table.add_column("Style name")
-    table.add_column("Width", justify="right")
-    table.add_column("Weight", justify="right")
-    table.add_column("Regular", justify="right")
-    table.add_column("Italic", justify="right")
-    table.add_column("Bold", justify="right")
-    table.add_column("Oblique", justify="right")
-
-    for i, row in enumerate(rows, start=1):
-        table.add_row(
-            str(i),
-            row["file_name"],
-            row["family_name"],
-            row["subfamily_name"],
-            row["us_width_class"],
-            row["us_weight_class"],
-            row["is_regular"],
-            row["is_italic"],
-            row["is_bold"],
-            row["is_oblique"],
-        )
-
-    return table
+import os.path
+import sys
+from pathlib import Path
+
+import click
+from rich import box
+from rich.console import Console
+from rich.table import Table
+from rich.tree import Tree
+
+from foundryToolsCLI.Lib.Font import Font
+from foundryToolsCLI.Lib.assistant.fonts_data import FontsData
+from foundryToolsCLI.Lib.assistant.styles_mapping import (
+    StylesMapping,
+    DEFAULT_WEIGHTS,
+    DEFAULT_WIDTHS,
+)
+from foundryToolsCLI.Lib.utils.cli_tools import (
+    get_style_mapping_path,
+    get_fonts_data_path,
+    get_fonts_in_path,
+)
+from foundryToolsCLI.Lib.utils.click_tools import generic_error_message, no_valid_fonts_message, OptionalParamType
+
+
+class AssistantUI(object):
+    def __init__(self, input_path: Path):
+        self.input_path = input_path
+
+        if len(self.fonts_list) == 0:
+            no_valid_fonts_message(input_path)
+            sys.exit()
+
+        self.styles_mapping = StylesMapping(get_style_mapping_path(self.input_path))
+        if not os.path.exists(self.styles_mapping.file):
+            self.styles_mapping.reset_defaults()
+
+        self.fonts_data = FontsData(get_fonts_data_path(self.input_path))
+        if not os.path.exists(self.fonts_data.file):
+            self.fonts_data.reset_data(styles_mapping=self.styles_mapping)
+
+        self.console = Console()
+
+    def run(self):
+        click.clear()
+        self.console.set_window_title("ftCLI assistant UI")
+        self.fonts_data_editor()
+
+    def styles_mapping_editor(self):
+        click.clear()
+        table = self.__get_styles_mapping_table()
+        commands = {
+            "g": "Edit Weights",
+            "t": "Edit Widths",
+            "i": "Edit Italics",
+            "o": "Edit Obliques",
+            "r": "Reset defaults",
+            "x": "Exit",
+        }
+        self.console.print(table)
+
+        command = self.__prompt_for_command(commands)
+        if command == "g":
+            self.__widths_weights_editor(key="weights")
+        if command == "t":
+            self.__widths_weights_editor(key="widths")
+        if command == "i":
+            self.__set_slope(key="italics")
+        if command == "o":
+            self.__set_slope(key="obliques")
+        if command == "r":
+            if self.__prompt_for_confirmation(text="Reset default values?"):
+                self.styles_mapping.reset_defaults()
+        if command == "x":
+            return
+
+        self.styles_mapping_editor()
+
+    def fonts_data_editor(self):
+        fonts_data = self.fonts_data.get_data()
+
+        commands = {
+            "m": "Edit Styles Mapping",
+            "s": "Select files",
+            "d": "Deselect files",
+            "f": "Set Family Name",
+            "i": "Set/Unset Italic",
+            "o": "Set/Unset Oblique",
+            "t": "Set Width",
+            "g": "Set Weight",
+            "l": "Set Slope",
+            "r": "Reset data",
+            "c": "Recalc data",
+            "x": "Exit",
+        }
+        table = self.__get_fonts_data_table()
+
+        click.clear()
+        self.console.print(table)
+
+        command = self.__prompt_for_command(commands)
+        if command == "m":
+            self.styles_mapping_editor()
+        if command == "s":
+            self.__select_deselect_files(action="select")
+        if command == "d":
+            self.__select_deselect_files(action="deselect")
+        if command == "f":
+            family_name = click.prompt("Family name")
+            if self.__prompt_for_confirmation():
+                for row in fonts_data:
+                    if row["selected"] == "1":
+                        row["family_name"] = family_name
+                self.fonts_data.save(fonts_data)
+        if command == "i":
+            italic_value = click.prompt(
+                f"Italic value {click.style('[0/1]', bold=True, fg='cyan')}",
+                type=click.Choice(choices=("0", "1")),
+                show_choices=False,
+            )
+            if self.__prompt_for_confirmation():
+                for row in fonts_data:
+                    if row["selected"] == "1":
+                        row["is_italic"] = italic_value
+                self.fonts_data.save(fonts_data)
+        if command == "o":
+            oblique_value = click.prompt(
+                f"Oblique value {click.style('[0/1]', bold=True, fg='cyan')}",
+                type=click.Choice(choices=("0", "1")),
+                show_choices=False,
+            )
+            if self.__prompt_for_confirmation():
+                for row in fonts_data:
+                    if row["selected"] == "1":
+                        row["is_oblique"] = oblique_value
+                self.fonts_data.save(fonts_data)
+        if command == "t":
+            us_width_class = click.prompt(
+                f"usWidthClass {click.style('[1-9]', bold=True, fg='cyan')} (Enter  to skip)",
+                type=OptionalParamType(click.IntRange(1, 9)),
+                default="",
+                show_default=False,
+            )
+            wdt = click.prompt(
+                "Short word (Enter to skip)",
+                type=OptionalParamType(click.STRING),
+                default="",
+                show_default=False,
+            )
+            width = click.prompt(
+                "Long word (Enter to skip)",
+                type=OptionalParamType(click.STRING),
+                default="",
+                show_default=False,
+            )
+
+            if self.__prompt_for_confirmation():
+                for row in fonts_data:
+                    if row["selected"] == "1":
+                        row["us_width_class"] = us_width_class if us_width_class else row["us_width_class"]
+                        words = [
+                            wdt if wdt else row["wdt"],
+                            width if width else row["width"],
+                        ]
+                        words.sort(key=len)
+                        row["wdt"] = words[0]
+                        row["width"] = words[1]
+                self.fonts_data.save(fonts_data)
+        if command == "g":
+            us_weight_class = click.prompt(
+                f"usWeightClass {click.style('[1-1000]', bold=True, fg='cyan')} " f"(Enter to skip)",
+                type=OptionalParamType(click.IntRange(1, 1000)),
+                default="",
+                show_default=False,
+            )
+            wgt = click.prompt(
+                "Short word (Enter to skip)",
+                type=OptionalParamType(click.STRING),
+                default="",
+                show_default=False,
+            )
+            weight = click.prompt(
+                "Long word (Enter to skip)",
+                type=OptionalParamType(click.STRING),
+                default="",
+                show_default=False,
+            )
+
+            if self.__prompt_for_confirmation():
+                for row in fonts_data:
+                    if row["selected"] == "1":
+                        if us_weight_class:
+                            row["us_weight_class"] = us_weight_class
+                        words = [
+                            wgt if wgt else row["wgt"],
+                            weight if weight else row["weight"],
+                        ]
+                        words.sort(key=len)
+                        row["wgt"] = words[0]
+                        row["weight"] = words[1]
+                self.fonts_data.save(fonts_data)
+        if command == "l":
+            slp = click.prompt(
+                "Short word (Enter to skip)",
+                type=OptionalParamType(click.STRING),
+                default="",
+                show_default=False,
+            )
+            slope = click.prompt(
+                "Long word (Enter to skip)",
+                type=OptionalParamType(click.STRING),
+                default="",
+                show_default=False,
+            )
+            if self.__prompt_for_confirmation():
+                for row in fonts_data:
+                    if row["selected"] == "1":
+                        words = [
+                            slp if slp else row["slp"],
+                            slope if slope else row["slope"],
+                        ]
+                        words.sort(key=len)
+                        row["slp"] = words[0]
+                        row["slope"] = words[1]
+                self.fonts_data.save(fonts_data)
+        if command == "r":
+            if self.__prompt_for_confirmation(text="Reset data?"):
+                self.fonts_data.reset_data(styles_mapping=self.styles_mapping)
+        if command == "c":
+            click.echo("\nPlease, select the string to use to recalculate data")
+            click.secho("[0]", bold=True, fg="cyan", nl=False)
+            click.echo(" : File Name")
+            click.secho("[1]", bold=True, fg="cyan", nl=False)
+            click.echo(" : PostScript Name")
+            click.secho("[2]", bold=True, fg="cyan", nl=False)
+            click.echo(" : Family Name + SubFamily Name")
+            click.secho("[3]", bold=True, fg="cyan", nl=False)
+            click.echo(" : Full Font Name")
+            click.secho("[4]", bold=True, fg="cyan", nl=False)
+            click.echo(" : CFF fontNames")
+            click.secho("[5]", bold=True, fg="cyan", nl=False)
+            click.echo(" : CFF FullName")
+            source_type = self.__prompt_for_int_range("Your selection", min_value=0, max_value=5, default=0)
+            if self.__prompt_for_confirmation(text="Recalc data?"):
+                self.fonts_data.recalc_data(source_type=source_type, styles_mapping=self.styles_mapping)
+
+        if command == "x":
+            return
+
+        self.fonts_data_editor()
+
+    def __widths_weights_editor(self, key: str):
+        if key == "weights":
+            max_value = 1000
+            defaults = DEFAULT_WEIGHTS
+        elif key == "widths":
+            max_value = 9
+            defaults = DEFAULT_WIDTHS
+        else:
+            return
+
+        data = self.styles_mapping.get_data()
+        table = self.__get_widths_weights_table(key)
+
+        commands = {
+            "a": "Add/edit item",
+            "d": "Delete item",
+            "r": "Reset defaults",
+            "x": "Exit",
+        }
+
+        click.clear()
+        self.console.print(table)
+        command = self.__prompt_for_command(commands)
+
+        if command == "a":
+            self.__add_width_weight(key=key, max_value=max_value)
+        if command == "d":
+            choices = [k for k in data[key].keys()]
+            value = click.prompt(
+                f"Value to delete {click.style('[' + ', '.join(choices) + ']', bold=True, fg='cyan')}",
+                type=click.Choice(choices=choices),
+                show_choices=False,
+            )
+            if self.__prompt_for_confirmation():
+                del data[key][value]
+                self.styles_mapping.save(data)
+        if command == "r":
+            if self.__prompt_for_confirmation(text="Reset default values?"):
+                data[key] = defaults
+                self.styles_mapping.save(data)
+        if command == "x":
+            return
+
+        self.__widths_weights_editor(key)
+
+    def __select_deselect_files(self, action):
+        data = self.fonts_data.get_data()
+
+        start = self.__prompt_for_int_range(text="From line", min_value=1, max_value=len(data), default=1)
+        end = self.__prompt_for_int_range(text="To line", min_value=start, max_value=len(data), default=len(data))
+
+        for i in range(start - 1, end):
+            if action == "select":
+                data[i]["selected"] = 1
+            if action == "deselect":
+                data[i]["selected"] = 0
+        self.fonts_data.save(data)
+
+    def __get_fonts_data_table(self) -> Table:
+        data = self.fonts_data.get_data()
+
+        table = Table(
+            title="ftCLI Assistant - Fonts Data Editor",
+            title_style="bold green",
+            header_style="bold cyan",
+            caption=self.fonts_data.file.as_posix(),
+            box=box.HORIZONTALS,
+        )
+
+        table.add_column("#", justify="right")
+        table.add_column("[+]")
+        table.add_column("File name")
+        table.add_column("Family name")
+        table.add_column("B")
+        table.add_column("I")
+        table.add_column("O")
+        table.add_column("Width")
+        table.add_column("Weight")
+        table.add_column("Slope")
+
+        for count, row in enumerate(data, start=1):
+            if row["selected"] == "1":
+                selected_string = "[bold cyan][+]"
+            else:
+                selected_string = "[ ]"
+            file_name = row["file_name"]
+            family_name = row["family_name"]
+            is_bold = row["is_bold"]
+            is_italic = row["is_italic"]
+            is_oblique = row["is_oblique"]
+            width = f"{row['us_width_class']} : {row['wdt']}, {row['width']}"
+            weight = f"{row['us_weight_class']} : {row['wgt']}, {row['weight']}"
+            if (row["slp"], row["slope"]) == ("", ""):
+                slope = ""
+            else:
+                slope = ", ".join([row["slp"], row["slope"]])
+
+            table.add_row(
+                str(count),
+                selected_string,
+                os.path.basename(file_name),
+                family_name,
+                is_bold,
+                is_italic,
+                is_oblique,
+                width,
+                weight,
+                slope,
+            )
+
+        return table
+
+    def __get_styles_mapping_table(self) -> Table:
+        """
+        Returns a Table object of the styles mapping
+        """
+        data = self.styles_mapping.get_data()
+
+        table = Table(
+            show_header=False,
+            title="ftCLI Assistant - Styles Mapping Editor",
+            title_style="bold green",
+            caption=self.styles_mapping.file.as_posix(),
+            box=box.HORIZONTALS,
+        )
+
+        table.add_row("Weight", "Short word", "Long word", style="bright_cyan", end_section=True)
+        for k, v in data["weights"].items():
+            table.add_row(k, v[0], v[1])
+        table.add_section()
+        table.add_row("Width", "Short word", "Long word", style="bright_cyan", end_section=True)
+        for k, v in data["widths"].items():
+            table.add_row(k, v[0], v[1])
+        table.add_section()
+        table.add_row("Slope", "Short word", "Long word", style="bright_cyan", end_section=True)
+        table.add_row("Italic", data["italics"][0], data["italics"][1])
+        table.add_row("Oblique", data["obliques"][0], data["obliques"][1])
+
+        return table
+
+    def __get_widths_weights_table(self, key) -> Table:
+        data = self.styles_mapping.get_data()
+        table = Table(
+            show_header=False,
+            title=f"ftCLI Assistant - {key.capitalize()} Editor",
+            title_style="bold green",
+            box=box.HORIZONTALS,
+        )
+        table.add_row(
+            f"{key[0:-1]}".capitalize(),
+            "Short word",
+            "Long word",
+            style="bold cyan",
+            end_section=True,
+        )
+        for k, v in data[key].items():
+            table.add_row(k, v[0], v[1])
+        table.add_section()
+
+        return table
+
+    def __add_width_weight(self, key: str, max_value: int):
+        data = self.styles_mapping.get_data()
+        value = str(self.__prompt_for_int_range(text="Value", min_value=1, max_value=max_value))
+
+        defaults = [None, None]
+        if value in data[key].keys():
+            defaults = data[key].get(value)
+            new_value = str(
+                self.__prompt_for_int_range(
+                    text="New value",
+                    min_value=1,
+                    max_value=max_value,
+                    default=int(value),
+                )
+            )
+            del data[key][value]
+            value = new_value
+
+        short_word = click.prompt(
+            f"Short word " f"{click.style(f'[{defaults[0]}]', bold=True, fg='cyan') if defaults[0] else ''}",
+            default=defaults[0],
+            show_default=False,
+        )
+        long_word = click.prompt(
+            f"Long word  " f"{click.style(f'[{defaults[1]}]', bold=True, fg='cyan') if defaults[1] else ''}",
+            default=defaults[1],
+            show_default=False,
+        )
+
+        if self.__prompt_for_confirmation():
+            # del data[key][value]
+            data[key][value] = sorted([short_word, long_word], key=len)
+            self.styles_mapping.save(data)
+
+    def __set_slope(self, key: str):
+        data = self.styles_mapping.get_data()
+
+        short_word = click.prompt(
+            f"Short word{click.style(f' [{data[key][0]}]', bold=True, fg='cyan')}",
+            default=data[key][0],
+            show_default=False,
+        )
+        long_word = click.prompt(
+            f"Long word{click.style(f' [{data[key][1]}]', bold=True, fg='cyan')}",
+            default=data[key][1],
+            show_default=False,
+        )
+
+        data[key] = sorted([short_word, long_word], key=len)
+
+        if self.__prompt_for_confirmation():
+            self.styles_mapping.save(data)
+
+    @staticmethod
+    def __prompt_for_command(commands: dict) -> str:
+        click.secho("\nAVAILABLE COMMANDS:\n", bold=True, fg="green")
+        for k, v in commands.items():
+            click.secho(f" {click.style(k, bold=True, fg='cyan')} : ", nl=False)
+            click.secho(f"{v} ", nl=True)
+
+        choices = [k for k in commands.keys()]
+        # command = click.prompt(f"\nSelect command [{click.style(', '.join(choices), bold=True, fg='cyan')}]",
+        command = click.prompt(
+            "\nSelect command",
+            type=click.Choice(choices=choices, case_sensitive=False),
+            show_choices=False,
+            show_default=False,
+            err=True,
+        )
+        return command
+
+    @staticmethod
+    def __prompt_for_int_range(
+        text: str,
+        min_value: int,
+        max_value: int,
+        default: int = None,
+        bold: bool = True,
+        fg_color: str = "cyan",
+    ) -> int:
+        """
+        > Prompt the user for an integer value within a specified range, and return the value as a string
+
+        :param text: The text to display to the user
+        :type text: str
+        :param min_value: The minimum value that the user can enter
+        :type min_value: int
+        :param max_value: The maximum value that the user can enter
+        :type max_value: int
+        :param default: The default value to use if no input happens. If a default value is given, it is shown in square
+            brackets in place of the min-max range
+        :type default: int
+        :param bold: bool = True, defaults to True
+        :type bold: bool (optional)
+        :param fg_color: The color of the highlighted text, defaults to cyan
+        :type fg_color: str (optional)
+        :return: An integer
+        """
+        highlighted_text = click.style(
+            f"[{default}]" if default is not None else f"[{min_value}-{max_value}]",
+            bold=bold,
+            fg=fg_color,
+        )
+        message = f"{text} {highlighted_text}"
+        value = click.prompt(
+            message,
+            type=click.IntRange(min_value, max_value),
+            default=default,
+            show_default=False,
+        )
+        return value
+
+    @staticmethod
+    def __prompt_for_confirmation(text="Save changes?") -> bool:
+        """
+        > Prompt the user for a yes/no confirmation, and return a boolean value
+
+        :param text: The text to display to the user, defaults to Save changes? (optional)
+        :return: A boolean value
+        """
+        return click.confirm(
+            f"{text} {click.style('[Y/n]', bold=True, fg='cyan')}",
+            default=True,
+            show_default=False,
+        )
+
+    @property
+    def fonts_list(self) -> list[Font]:
+        return get_fonts_in_path(self.input_path)
+
+
+def get_commands_tree(commands: dict) -> Tree:
+    """
+    Takes a dictionary of commands and returns a Tree object
+
+    :param commands: the dictionary of commands
+    :type commands: dict
+    :return: A Tree object with the label "COMMANDS" and the style "green"
+    """
+    commands_tree = Tree(label="COMMANDS", style="green", guide_style="green")
+    for k, v in commands.items():
+        commands_tree.add(f"[bold green]{k}[reset] : [bold cyan]{v}")
+    return commands_tree
+
+
+def get_fonts_rows(fonts: list[Font]) -> list:
+    rows = []
+    for font in fonts:
+        try:
+            row = dict(
+                file_name=os.path.basename(font.reader.file.name),
+                family_name=font["name"].getBestFamilyName(),
+                subfamily_name=font["name"].getBestSubFamilyName(),
+                us_width_class=str(font["OS/2"].usWidthClass),
+                us_weight_class=str(font["OS/2"].usWeightClass),
+                is_bold=str(int(font.is_bold)),
+                is_italic=str(int(font.is_italic)),
+                is_oblique=str(int(font.is_oblique)),
+                is_regular=str(int(font.is_regular)),
+            )
+            rows.append(row)
+        except Exception as e:
+            generic_error_message(e)
+    return rows
+
+
+def get_fonts_list_table(rows: list) -> Table:
+    table = Table(box=box.HORIZONTALS)
+
+    table.add_column("#", justify="right")
+    table.add_column("File name")
+    table.add_column("Family name")
+    table.add_column("Style name")
+    table.add_column("Width", justify="right")
+    table.add_column("Weight", justify="right")
+    table.add_column("Regular", justify="right")
+    table.add_column("Italic", justify="right")
+    table.add_column("Bold", justify="right")
+    table.add_column("Oblique", justify="right")
+
+    for i, row in enumerate(rows, start=1):
+        table.add_row(
+            str(i),
+            row["file_name"],
+            row["family_name"],
+            row["subfamily_name"],
+            row["us_width_class"],
+            row["us_weight_class"],
+            row["is_regular"],
+            row["is_italic"],
+            row["is_bold"],
+            row["is_oblique"],
+        )
+
+    return table
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/constants.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/constants.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-from fontTools.ttLib.tables._n_a_m_e import _WINDOWS_LANGUAGES, _MAC_LANGUAGES
-
-NAME_IDS = {
-    0: "Copyright Notice",
-    1: "Family name",
-    2: "Subfamily name",
-    3: "Unique identifier",
-    4: "Full font name",
-    5: "Version string",
-    6: "PostScript name",
-    7: "Trademark",
-    8: "Manufacturer Name",
-    9: "Designer",
-    10: "Description",
-    11: "URL Vendor",
-    12: "URL Designer",
-    13: "License Description",
-    14: "License Info URL",
-    15: "Reserved",
-    16: "Typographic Family",
-    17: "Typographic Subfamily",
-    18: "Compatible Full (Mac)",
-    19: "Sample text",
-    20: "PS CID font name",
-    21: "WWS Family Name",
-    22: "WWS Subfamily Name",
-    23: "Light Background Palette",
-    24: "Dark Background Palette",
-    25: "Variations PSName Pref",
-}
-
-PLATFORMS = {
-    0: "Unicode",
-    1: "Macintosh",
-    2: "ISO (deprecated)",
-    3: "Windows",
-    4: "Custom",
-}
-
-MAC_ENCODING_IDS = {
-    0: "Roman",
-    1: "Japanese",
-    2: "Chinese (Traditional)",
-    3: "Korean",
-    4: "Arabic",
-    5: "Hebrew",
-    6: "Greek",
-    7: "Russian",
-    8: "RSymbol",
-    9: "Devanagari",
-    10: "Gurmukhi",
-    11: "Gujarati",
-    12: "Oriya",
-    13: "Bengali",
-    14: "Tamil",
-    15: "Telugu",
-    16: "Kannada",
-    17: "Malayalam",
-    18: "Sinhalese",
-    19: "Burmese",
-    20: "Khmer",
-    21: "Thai",
-    22: "Laotian",
-    23: "Georgian",
-    24: "Armenian",
-    25: "Chinese (Simplified)",
-    26: "Tibetan",
-    27: "Mongolian",
-    28: "Geez",
-    29: "Slavic",
-    30: "Vietnamese",
-    31: "Sindhi",
-    32: "Uninterpreted",
-}
-
-WINDOWS_ENCODING_IDS = {
-    0: "Symbol",
-    1: "Unicode",
-    2: "ShiftJIS",
-    3: "PRC",
-    4: "Big5",
-    5: "Wansung",
-    6: "Johab",
-    7: "Reserved",
-    8: "Reserved",
-    9: "Reserved",
-    10: "UCS4",
-}
-
-EMBED_LEVEL_STRINGS = {
-    0: "Installable embedding",
-    2: "Restricted License embedding",
-    4: "Preview & Print embedding",
-    8: "Editable embedding",
-}
-
-MAX_FAMILY_NAME_LEN = 27
-MAX_FULL_NAME_LEN = 31
-MAX_POSTSCRIPT_NAME_LEN = 29
-
-LANGUAGES_EPILOG = f"""
-MACINTOSH LANGUAGES: {", ".join([lang for lang in _MAC_LANGUAGES.values()])}
-
-WINDOWS LANGUAGES: f{", ".join([lang for lang in _WINDOWS_LANGUAGES.values()])}
-"""
+from fontTools.ttLib.tables._n_a_m_e import _WINDOWS_LANGUAGES, _MAC_LANGUAGES
+
+NAME_IDS = {
+    0: "Copyright Notice",
+    1: "Family name",
+    2: "Subfamily name",
+    3: "Unique identifier",
+    4: "Full font name",
+    5: "Version string",
+    6: "PostScript name",
+    7: "Trademark",
+    8: "Manufacturer Name",
+    9: "Designer",
+    10: "Description",
+    11: "URL Vendor",
+    12: "URL Designer",
+    13: "License Description",
+    14: "License Info URL",
+    15: "Reserved",
+    16: "Typographic Family",
+    17: "Typographic Subfamily",
+    18: "Compatible Full (Mac)",
+    19: "Sample text",
+    20: "PS CID font name",
+    21: "WWS Family Name",
+    22: "WWS Subfamily Name",
+    23: "Light Background Palette",
+    24: "Dark Background Palette",
+    25: "Variations PSName Pref",
+}
+
+PLATFORMS = {
+    0: "Unicode",
+    1: "Macintosh",
+    2: "ISO (deprecated)",
+    3: "Windows",
+    4: "Custom",
+}
+
+MAC_ENCODING_IDS = {
+    0: "Roman",
+    1: "Japanese",
+    2: "Chinese (Traditional)",
+    3: "Korean",
+    4: "Arabic",
+    5: "Hebrew",
+    6: "Greek",
+    7: "Russian",
+    8: "RSymbol",
+    9: "Devanagari",
+    10: "Gurmukhi",
+    11: "Gujarati",
+    12: "Oriya",
+    13: "Bengali",
+    14: "Tamil",
+    15: "Telugu",
+    16: "Kannada",
+    17: "Malayalam",
+    18: "Sinhalese",
+    19: "Burmese",
+    20: "Khmer",
+    21: "Thai",
+    22: "Laotian",
+    23: "Georgian",
+    24: "Armenian",
+    25: "Chinese (Simplified)",
+    26: "Tibetan",
+    27: "Mongolian",
+    28: "Geez",
+    29: "Slavic",
+    30: "Vietnamese",
+    31: "Sindhi",
+    32: "Uninterpreted",
+}
+
+WINDOWS_ENCODING_IDS = {
+    0: "Symbol",
+    1: "Unicode",
+    2: "ShiftJIS",
+    3: "PRC",
+    4: "Big5",
+    5: "Wansung",
+    6: "Johab",
+    7: "Reserved",
+    8: "Reserved",
+    9: "Reserved",
+    10: "UCS4",
+}
+
+EMBED_LEVEL_STRINGS = {
+    0: "Installable embedding",
+    2: "Restricted License embedding",
+    4: "Preview & Print embedding",
+    8: "Editable embedding",
+}
+
+MAX_FAMILY_NAME_LEN = 27
+MAX_FULL_NAME_LEN = 31
+MAX_POSTSCRIPT_NAME_LEN = 29
+
+LANGUAGES_EPILOG = f"""
+MACINTOSH LANGUAGES: {", ".join([lang for lang in _MAC_LANGUAGES.values()])}
+
+WINDOWS LANGUAGES: f{", ".join([lang for lang in _WINDOWS_LANGUAGES.values()])}
+"""
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/otf_to_ttf.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/otf_to_ttf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,137 +1,135 @@
-import time
-from pathlib import Path
-
-from fontTools.misc.cliTools import makeOutputFileName
-from fontTools.pens.cu2quPen import Cu2QuPen
-from fontTools.pens.ttGlyphPen import TTGlyphPen
-from fontTools.ttLib import TTLibError, newTable
-
-from foundryToolsCLI.Lib.Font import Font
-from foundryToolsCLI.Lib.converters.options import CFFToTrueTypeOptions
-from foundryToolsCLI.Lib.utils.click_tools import generic_info_message, file_saved_message, generic_error_message
-
-CWD = Path.cwd()
-
-
-class OTF2TTFRunner(object):
-    def __init__(self):
-        super().__init__()
-        self.options = CFFToTrueTypeOptions()
-
-    def run(self, source_fonts: list[Font]) -> None:
-        converted_files_count = 0
-        start_time = time.time()
-
-        for count, source_font in enumerate(source_fonts, start=1):
-            t = time.time()
-
-            try:
-                print()
-                generic_info_message(f"Converting file {count} of {len(source_fonts)}")
-
-                file = Path(source_font.reader.file.name)
-
-                # If the source font is a WOFF or WOFF2, we add a suffix to avoid unwanted overwriting
-                if source_font.flavor is None:
-                    ext = ".ttf"
-                    suffix = ""
-                else:
-                    ext = source_font.get_real_extension()
-                    suffix = ".ttf"
-                file_name = file.name.replace(".otf", "").replace(".ttf", "").replace(".woff2", "").replace(".woff", "")
-
-                output_file = Path(
-                    makeOutputFileName(
-                        file_name,
-                        extension=ext,
-                        suffix=suffix,
-                        outputDir=self.options.output_dir,
-                        overWrite=self.options.overwrite,
-                    )
-                )
-
-                converter = CFFToTrueType(font=source_font)
-                converter.options.max_err = self.options.max_err
-                ttf_font = converter.run()
-                ttf_font.save(output_file)
-                ttf_font.close()
-
-                generic_info_message(f"Elapsed time: {round(time.time() - t, 3)} seconds")
-                file_saved_message(output_file.relative_to(CWD))
-                converted_files_count += 1
-
-            except Exception as e:
-                generic_error_message(e)
-            finally:
-                source_font.close()
-
-        print()
-        generic_info_message(f"Total files     : {len(source_fonts)}")
-        generic_info_message(f"Converted files : {converted_files_count}")
-        generic_info_message(f"Elapsed time    : {round(time.time() - start_time, 3)} seconds")
-
-
-class CFFToTrueType(object):
-    def __init__(self, font: Font):
-        self.font = font
-        self.options = CFFToTrueTypeOptions()
-
-    def run(self):
-        if self.font.sfntVersion != "OTTO":
-            raise TTLibError("Not a OpenType font (bad sfntVersion)")
-        assert "CFF " in self.font
-
-        glyphOrder = self.font.getGlyphOrder()
-
-        self.font["loca"] = newTable("loca")
-        self.font["glyf"] = glyf = newTable("glyf")
-        glyf.glyphOrder = glyphOrder
-        glyf.glyphs = self.glyphs_to_quadratic(glyphs=self.font.getGlyphSet())
-        del self.font["CFF "]
-        if "VORG" in self.font:
-            del self.font["VORG"]
-        glyf.compile(self.font)
-        self.update_hmtx(glyf)
-
-        self.font["maxp"] = maxp = newTable("maxp")
-        maxp.tableVersion = 0x00010000
-        maxp.maxZones = 1
-        maxp.maxTwilightPoints = 0
-        maxp.maxStorage = 0
-        maxp.maxFunctionDefs = 0
-        maxp.maxInstructionDefs = 0
-        maxp.maxStackElements = 0
-        maxp.maxSizeOfInstructions = 0
-        maxp.maxComponentElements = max(
-            len(g.components if hasattr(g, "components") else []) for g in glyf.glyphs.values()
-        )
-        maxp.compile(self.font)
-
-        post = self.font["post"]
-        post.formatType = self.options.post_format
-        post.extraNames = []
-        post.mapping = {}
-        post.glyphOrder = glyphOrder
-        try:
-            post.compile(self.font)
-        except OverflowError:
-            post.formatType = 3
-
-        self.font.sfntVersion = "\000\001\000\000"
-        return self.font
-
-    def update_hmtx(self, glyf):
-        hmtx = self.font["hmtx"]
-        for glyphName, glyph in glyf.glyphs.items():
-            if hasattr(glyph, "xMin"):
-                hmtx[glyphName] = (hmtx[glyphName][0], glyph.xMin)
-
-    def glyphs_to_quadratic(self, glyphs):
-        quadGlyphs = {}
-        for gname in glyphs.keys():
-            glyph = glyphs[gname]
-            ttPen = TTGlyphPen(glyphs)
-            cu2quPen = Cu2QuPen(ttPen, max_err=self.options.max_err, reverse_direction=self.options.reverse_direction)
-            glyph.draw(cu2quPen)
-            quadGlyphs[gname] = ttPen.glyph()
-        return quadGlyphs
+import time
+from pathlib import Path
+
+from fontTools.misc.cliTools import makeOutputFileName
+from fontTools.pens.cu2quPen import Cu2QuPen
+from fontTools.pens.ttGlyphPen import TTGlyphPen
+from fontTools.ttLib import TTLibError, newTable
+
+from foundryToolsCLI.Lib.Font import Font
+from foundryToolsCLI.Lib.converters.options import CFFToTrueTypeOptions
+from foundryToolsCLI.Lib.utils.click_tools import generic_info_message, file_saved_message, generic_error_message
+
+
+class OTF2TTFRunner(object):
+    def __init__(self):
+        super().__init__()
+        self.options = CFFToTrueTypeOptions()
+
+    def run(self, source_fonts: list[Font]) -> None:
+        converted_files_count = 0
+        start_time = time.time()
+
+        for count, source_font in enumerate(source_fonts, start=1):
+            t = time.time()
+
+            try:
+                print()
+                generic_info_message(f"Converting file {count} of {len(source_fonts)}")
+
+                file = Path(source_font.reader.file.name)
+
+                # If the source font is a WOFF or WOFF2, we add a suffix to avoid unwanted overwriting
+                if source_font.flavor is None:
+                    ext = ".ttf"
+                    suffix = ""
+                else:
+                    ext = source_font.get_real_extension()
+                    suffix = ".ttf"
+                file_name = file.name.replace(".otf", "").replace(".ttf", "").replace(".woff2", "").replace(".woff", "")
+
+                output_file = Path(
+                    makeOutputFileName(
+                        file_name,
+                        extension=ext,
+                        suffix=suffix,
+                        outputDir=self.options.output_dir,
+                        overWrite=self.options.overwrite,
+                    )
+                )
+
+                converter = CFFToTrueType(font=source_font)
+                converter.options.max_err = self.options.max_err
+                ttf_font = converter.run()
+                ttf_font.save(output_file)
+                ttf_font.close()
+
+                generic_info_message(f"Elapsed time: {round(time.time() - t, 3)} seconds")
+                file_saved_message(output_file)
+                converted_files_count += 1
+
+            except Exception as e:
+                generic_error_message(e)
+            finally:
+                source_font.close()
+
+        print()
+        generic_info_message(f"Total files     : {len(source_fonts)}")
+        generic_info_message(f"Converted files : {converted_files_count}")
+        generic_info_message(f"Elapsed time    : {round(time.time() - start_time, 3)} seconds")
+
+
+class CFFToTrueType(object):
+    def __init__(self, font: Font):
+        self.font = font
+        self.options = CFFToTrueTypeOptions()
+
+    def run(self):
+        if self.font.sfntVersion != "OTTO":
+            raise TTLibError("Not a OpenType font (bad sfntVersion)")
+        assert "CFF " in self.font
+
+        glyphOrder = self.font.getGlyphOrder()
+
+        self.font["loca"] = newTable("loca")
+        self.font["glyf"] = glyf = newTable("glyf")
+        glyf.glyphOrder = glyphOrder
+        glyf.glyphs = self.glyphs_to_quadratic(glyphs=self.font.getGlyphSet())
+        del self.font["CFF "]
+        if "VORG" in self.font:
+            del self.font["VORG"]
+        glyf.compile(self.font)
+        self.update_hmtx(glyf)
+
+        self.font["maxp"] = maxp = newTable("maxp")
+        maxp.tableVersion = 0x00010000
+        maxp.maxZones = 1
+        maxp.maxTwilightPoints = 0
+        maxp.maxStorage = 0
+        maxp.maxFunctionDefs = 0
+        maxp.maxInstructionDefs = 0
+        maxp.maxStackElements = 0
+        maxp.maxSizeOfInstructions = 0
+        maxp.maxComponentElements = max(
+            len(g.components if hasattr(g, "components") else []) for g in glyf.glyphs.values()
+        )
+        maxp.compile(self.font)
+
+        post = self.font["post"]
+        post.formatType = self.options.post_format
+        post.extraNames = []
+        post.mapping = {}
+        post.glyphOrder = glyphOrder
+        try:
+            post.compile(self.font)
+        except OverflowError:
+            post.formatType = 3
+
+        self.font.sfntVersion = "\000\001\000\000"
+        return self.font
+
+    def update_hmtx(self, glyf):
+        hmtx = self.font["hmtx"]
+        for glyphName, glyph in glyf.glyphs.items():
+            if hasattr(glyph, "xMin"):
+                hmtx[glyphName] = (hmtx[glyphName][0], glyph.xMin)
+
+    def glyphs_to_quadratic(self, glyphs):
+        quadGlyphs = {}
+        for gname in glyphs.keys():
+            glyph = glyphs[gname]
+            ttPen = TTGlyphPen(glyphs)
+            cu2quPen = Cu2QuPen(ttPen, max_err=self.options.max_err, reverse_direction=self.options.reverse_direction)
+            glyph.draw(cu2quPen)
+            quadGlyphs[gname] = ttPen.glyph()
+        return quadGlyphs
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/sfnt_to_web.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/sfnt_to_web.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,83 @@
-import time
-from pathlib import Path
-
-from fontTools.misc.cliTools import makeOutputFileName
-
-from foundryToolsCLI.Lib.Font import Font
-from foundryToolsCLI.Lib.converters.options import SFNTToWebOptions
-from foundryToolsCLI.Lib.utils.click_tools import generic_info_message, file_saved_message, generic_error_message
-
-CWD = Path.cwd()
-
-
-class FT2WFRunner(object):
-    def __init__(self):
-        super().__init__()
-        self.options = SFNTToWebOptions()
-
-    def run(self, fonts: list[Font]) -> None:
-        converted_files_count = 0
-        start_time = time.time()
-
-        for count, font in enumerate(fonts, start=1):
-            t = time.time()
-            print()
-            generic_info_message(f"Converting file {count} of {len(fonts)}")
-
-            try:
-                if font.flavor is not None:
-                    continue
-
-                file = font.reader.file.name
-
-                if self.options.woff:
-                    converter = SFNTToWeb(font=font, flavor="woff")
-                    web_font = converter.run()
-                    extension = web_font.get_real_extension()
-                    output_file = Path(
-                        makeOutputFileName(
-                            file,
-                            extension=extension,
-                            outputDir=self.options.output_dir,
-                            overWrite=self.options.overwrite,
-                        )
-                    )
-                    web_font.save(output_file, reorderTables=False)
-                    file_saved_message(output_file.relative_to(CWD))
-                    generic_info_message(f"Elapsed time: {round(time.time() - t, 3)} seconds")
-                    converted_files_count += 1
-
-                if self.options.woff2:
-                    converter = SFNTToWeb(font=font, flavor="woff2")
-                    web_font = converter.run()
-                    extension = web_font.get_real_extension()
-                    output_file = Path(
-                        makeOutputFileName(
-                            file,
-                            extension=extension,
-                            outputDir=self.options.output_dir,
-                            overWrite=self.options.overwrite,
-                        )
-                    )
-                    web_font.save(output_file, reorderTables=False)
-                    file_saved_message(output_file.relative_to(CWD))
-                    generic_info_message(f"Elapsed time: {round(time.time() - t, 3)} seconds")
-                    converted_files_count += 1
-
-            except Exception as e:
-                generic_error_message(e)
-            finally:
-                font.close()
-
-        print()
-        generic_info_message(f"Total files     : {len(fonts)}")
-        generic_info_message(f"Converted files : {converted_files_count}")
-        generic_info_message(f"Elapsed time    : {round(time.time() - start_time, 3)} seconds")
-
-
-class SFNTToWeb(object):
-    def __init__(self, font: Font, flavor: str):
-        self.font = font
-        self.flavor = flavor
-
-    def run(self) -> Font:
-        self.font.flavor = self.flavor
-        return self.font
+import time
+from pathlib import Path
+
+from fontTools.misc.cliTools import makeOutputFileName
+
+from foundryToolsCLI.Lib.Font import Font
+from foundryToolsCLI.Lib.converters.options import SFNTToWebOptions
+from foundryToolsCLI.Lib.utils.click_tools import generic_info_message, file_saved_message, generic_error_message
+
+
+class FT2WFRunner(object):
+    def __init__(self):
+        super().__init__()
+        self.options = SFNTToWebOptions()
+
+    def run(self, fonts: list[Font]) -> None:
+        converted_files_count = 0
+        start_time = time.time()
+
+        for count, font in enumerate(fonts, start=1):
+            t = time.time()
+            print()
+            generic_info_message(f"Converting file {count} of {len(fonts)}")
+
+            try:
+                if font.flavor is not None:
+                    continue
+
+                file = font.reader.file.name
+
+                if self.options.woff:
+                    converter = SFNTToWeb(font=font, flavor="woff")
+                    web_font = converter.run()
+                    extension = web_font.get_real_extension()
+                    output_file = Path(
+                        makeOutputFileName(
+                            file,
+                            extension=extension,
+                            outputDir=self.options.output_dir,
+                            overWrite=self.options.overwrite,
+                        )
+                    )
+                    web_font.save(output_file, reorderTables=False)
+                    file_saved_message(output_file)
+                    generic_info_message(f"Elapsed time: {round(time.time() - t, 3)} seconds")
+                    converted_files_count += 1
+
+                if self.options.woff2:
+                    converter = SFNTToWeb(font=font, flavor="woff2")
+                    web_font = converter.run()
+                    extension = web_font.get_real_extension()
+                    output_file = Path(
+                        makeOutputFileName(
+                            file,
+                            extension=extension,
+                            outputDir=self.options.output_dir,
+                            overWrite=self.options.overwrite,
+                        )
+                    )
+                    web_font.save(output_file, reorderTables=False)
+                    file_saved_message(output_file)
+                    generic_info_message(f"Elapsed time: {round(time.time() - t, 3)} seconds")
+                    converted_files_count += 1
+
+            except Exception as e:
+                generic_error_message(e)
+            finally:
+                font.close()
+
+        print()
+        generic_info_message(f"Total files     : {len(fonts)}")
+        generic_info_message(f"Converted files : {converted_files_count}")
+        generic_info_message(f"Elapsed time    : {round(time.time() - start_time, 3)} seconds")
+
+
+class SFNTToWeb(object):
+    def __init__(self, font: Font, flavor: str):
+        self.font = font
+        self.flavor = flavor
+
+    def run(self) -> Font:
+        self.font.flavor = self.flavor
+        return self.font
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/variable_to_static.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/variable_to_static.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,93 @@
-import time
-from pathlib import Path
-
-from fontTools.misc.cliTools import makeOutputFileName
-from fontTools.varLib.instancer import instantiateVariableFont, OverlapMode
-from pathvalidate import sanitize_filename
-
-from foundryToolsCLI.Lib.VFont import VariableFont
-from foundryToolsCLI.Lib.converters.options import Var2StaticOptions
-from foundryToolsCLI.Lib.tables.name import TableName
-from foundryToolsCLI.Lib.utils.click_tools import (
-    generic_warning_message,
-    generic_info_message,
-    file_saved_message,
-    generic_error_message,
-)
-
-CWD = Path.cwd()
-
-
-class VariableToStatic(object):
-    def __init__(self):
-        self.options = Var2StaticOptions()
-
-    def run(self, variable_font: VariableFont, instances: list = None):
-        start_time = time.time()
-
-        if not instances:
-            instances = variable_font.get_instances()
-
-        if len(instances) == 0:
-            generic_error_message("No instances found")
-            return
-
-        if self.options.update_name_table:
-            if "STAT" not in variable_font:
-                self.options.update_name_table = False
-                generic_warning_message("Cannot update name table if there is no STAT table.")
-            if not hasattr(variable_font["STAT"], "AxisValueArray"):
-                self.options.update_name_table = False
-                generic_warning_message("Cannot update name table if there are no STAT Axis Values.")
-
-        instance_count = 0
-        for instance in instances:
-            t = time.time()
-            instance_count += 1
-
-            print()
-            generic_info_message(f"Exporting instance {instance_count} of {len(instances)}")
-
-            static_instance = instantiateVariableFont(
-                varfont=variable_font,
-                axisLimits=instance.coordinates,
-                inplace=False,
-                overlap=OverlapMode.REMOVE_AND_IGNORE_ERRORS,
-                optimize=True,
-                updateFontNames=self.options.update_name_table,
-            )
-
-            if "cvar" in static_instance:
-                del static_instance["cvar"]
-
-            if self.options.cleanup:
-                name_table: TableName = static_instance["name"]
-                name_ids_to_delete = variable_font.get_var_name_ids_to_delete() if self.options.cleanup else []
-                name_table.del_names(name_ids=name_ids_to_delete)
-
-                if "STAT" in static_instance:
-                    del static_instance["STAT"]
-
-                static_instance.reorder_ui_name_ids()
-
-            static_instance_name = sanitize_filename(variable_font.get_instance_file_name(instance))
-            # Replace dots with underscores to prevent makeOutputFileName truncating names
-            static_instance_name = static_instance_name.replace(".", "_")
-            static_instance_extension = static_instance.get_real_extension()
-            output_file = Path(
-                makeOutputFileName(
-                    static_instance_name,
-                    extension=static_instance_extension,
-                    outputDir=self.options.output_dir,
-                    overWrite=self.options.overwrite,
-                )
-            )
-            static_instance.save(output_file)
-            static_instance.close()
-
-            generic_info_message(f"Done in {round(time.time() - t, 3)} seconds")
-            file_saved_message(output_file.relative_to(CWD))
-
-        variable_font.close()
-
-        print()
-        generic_info_message(f"Total instances : {len(instances)}")
-        generic_info_message(f"Elapsed time    : {round(time.time() - start_time, 3)} seconds")
+import time
+from pathlib import Path
+
+from fontTools.misc.cliTools import makeOutputFileName
+from fontTools.varLib.instancer import instantiateVariableFont, OverlapMode
+from pathvalidate import sanitize_filename
+
+from foundryToolsCLI.Lib.VFont import VariableFont
+from foundryToolsCLI.Lib.converters.options import Var2StaticOptions
+from foundryToolsCLI.Lib.tables.name import TableName
+from foundryToolsCLI.Lib.utils.click_tools import (
+    generic_warning_message,
+    generic_info_message,
+    file_saved_message,
+    generic_error_message,
+)
+
+
+class VariableToStatic(object):
+    def __init__(self):
+        self.options = Var2StaticOptions()
+
+    def run(self, variable_font: VariableFont, instances: list = None):
+        start_time = time.time()
+
+        if not instances:
+            instances = variable_font.get_instances()
+
+        if len(instances) == 0:
+            generic_error_message("No instances found")
+            return
+
+        if self.options.update_name_table:
+            if "STAT" not in variable_font:
+                self.options.update_name_table = False
+                generic_warning_message("Cannot update name table if there is no STAT table.")
+            if not hasattr(variable_font["STAT"], "AxisValueArray"):
+                self.options.update_name_table = False
+                generic_warning_message("Cannot update name table if there are no STAT Axis Values.")
+
+        instance_count = 0
+        for instance in instances:
+            t = time.time()
+            instance_count += 1
+
+            print()
+            generic_info_message(f"Exporting instance {instance_count} of {len(instances)}")
+
+            static_instance = instantiateVariableFont(
+                varfont=variable_font,
+                axisLimits=instance.coordinates,
+                inplace=False,
+                overlap=OverlapMode.REMOVE_AND_IGNORE_ERRORS,
+                optimize=True,
+                updateFontNames=self.options.update_name_table,
+            )
+
+            if "cvar" in static_instance:
+                del static_instance["cvar"]
+
+            if self.options.cleanup:
+                name_table: TableName = static_instance["name"]
+                name_ids_to_delete = variable_font.get_var_name_ids_to_delete() if self.options.cleanup else []
+                name_table.del_names(name_ids=name_ids_to_delete)
+
+                if "STAT" in static_instance:
+                    del static_instance["STAT"]
+
+                static_instance.reorder_ui_name_ids()
+
+            static_instance_name = sanitize_filename(variable_font.get_instance_file_name(instance))
+            # Replace dots with underscores to prevent makeOutputFileName truncating names
+            static_instance_name = static_instance_name.replace(".", "_")
+            static_instance_extension = static_instance.get_real_extension()
+            output_file = Path(
+                makeOutputFileName(
+                    static_instance_name,
+                    extension=static_instance_extension,
+                    outputDir=self.options.output_dir,
+                    overWrite=self.options.overwrite,
+                )
+            )
+            static_instance.save(output_file)
+            static_instance.close()
+
+            generic_info_message(f"Done in {round(time.time() - t, 3)} seconds")
+            file_saved_message(output_file)
+
+        variable_font.close()
+
+        print()
+        generic_info_message(f"Total instances : {len(instances)}")
+        generic_info_message(f"Elapsed time    : {round(time.time() - start_time, 3)} seconds")
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/converters/web_to_sfnt.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/web_to_sfnt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,61 @@
-import time
-from pathlib import Path
-
-from fontTools.misc.cliTools import makeOutputFileName
-
-from foundryToolsCLI.Lib.Font import Font
-from foundryToolsCLI.Lib.converters.options import WebToSFNTOptions
-from foundryToolsCLI.Lib.utils.click_tools import generic_info_message, generic_error_message, file_saved_message
-
-CWD = Path.cwd()
-
-
-class WF2FTRunner(object):
-    def __init__(self):
-        super().__init__()
-        self.options = WebToSFNTOptions()
-
-    def run(self, fonts: list[Font]) -> None:
-        converted_files_count = 0
-        start_time = time.time()
-
-        for count, font in enumerate(fonts, start=1):
-            t = time.time()
-            print()
-            generic_info_message(f"Converting file {count} of {len(fonts)}")
-
-            try:
-                file = font.reader.file.name
-
-                if not font.flavor:
-                    continue
-                if not self.options.woff:
-                    if font.flavor == "woff":
-                        continue
-                if not self.options.woff2:
-                    if font.flavor == "woff2":
-                        continue
-
-                font.flavor = None
-                new_extension = font.get_real_extension()
-                output_file = Path(
-                    makeOutputFileName(
-                        file,
-                        extension=new_extension,
-                        outputDir=self.options.output_dir,
-                        overWrite=self.options.overwrite,
-                    )
-                )
-
-                font.save(output_file)
-                generic_info_message(f"Elapsed time: {round(time.time() - t, 3)} seconds")
-                file_saved_message(output_file.relative_to(CWD))
-                converted_files_count += 1
-
-            except Exception as e:
-                generic_error_message(e)
-            finally:
-                font.close()
-
-        print()
-        generic_info_message(f"Total files     : {len(fonts)}")
-        generic_info_message(f"Converted files : {converted_files_count}")
-        generic_info_message(f"Elapsed time    : {round(time.time() - start_time, 3)} seconds")
+import time
+from pathlib import Path
+
+from fontTools.misc.cliTools import makeOutputFileName
+
+from foundryToolsCLI.Lib.Font import Font
+from foundryToolsCLI.Lib.converters.options import WebToSFNTOptions
+from foundryToolsCLI.Lib.utils.click_tools import generic_info_message, generic_error_message, file_saved_message
+
+
+class WF2FTRunner(object):
+    def __init__(self):
+        super().__init__()
+        self.options = WebToSFNTOptions()
+
+    def run(self, fonts: list[Font]) -> None:
+        converted_files_count = 0
+        start_time = time.time()
+
+        for count, font in enumerate(fonts, start=1):
+            t = time.time()
+            print()
+            generic_info_message(f"Converting file {count} of {len(fonts)}")
+
+            try:
+                file = font.reader.file.name
+
+                if not font.flavor:
+                    continue
+                if not self.options.woff:
+                    if font.flavor == "woff":
+                        continue
+                if not self.options.woff2:
+                    if font.flavor == "woff2":
+                        continue
+
+                font.flavor = None
+                new_extension = font.get_real_extension()
+                output_file = Path(
+                    makeOutputFileName(
+                        file,
+                        extension=new_extension,
+                        outputDir=self.options.output_dir,
+                        overWrite=self.options.overwrite,
+                    )
+                )
+
+                font.save(output_file)
+                generic_info_message(f"Elapsed time: {round(time.time() - t, 3)} seconds")
+                file_saved_message(output_file)
+                converted_files_count += 1
+
+            except Exception as e:
+                generic_error_message(e)
+            finally:
+                font.close()
+
+        print()
+        generic_info_message(f"Total files     : {len(fonts)}")
+        generic_info_message(f"Converted files : {converted_files_count}")
+        generic_info_message(f"Elapsed time    : {round(time.time() - start_time, 3)} seconds")
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/printer/UI.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/printer/UI.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,338 +1,338 @@
-import os.path
-from shutil import get_terminal_size
-
-from fontTools.ttLib.tables._n_a_m_e import _MAC_LANGUAGES, _WINDOWS_LANGUAGES
-from rich import box
-from rich.console import Console
-from rich.table import Table
-
-from foundryToolsCLI.Lib import constants
-from foundryToolsCLI.Lib.Font import Font
-from foundryToolsCLI.Lib.VFont import VariableFont
-from foundryToolsCLI.Lib.tables.OS_2 import TableOS2
-from foundryToolsCLI.Lib.tables.name import TableName
-from foundryToolsCLI.Lib.utils.click_tools import generic_error_message
-from foundryToolsCLI.Lib.utils.text_tools import wrap_string
-
-
-def print_fonts_list(fonts: list[Font]) -> None:
-    """
-    Prints list of fonts in `input_path` with basic information: Family name, Style name, usWidthClass, usWeightClass,
-    Bold value, Italic value, Oblique value
-    """
-    rows = []
-    for font in fonts:
-        try:
-            font_info = font.get_font_info()
-            row = dict(
-                file_name=os.path.basename(font_info["file_name"]["value"]),
-                family_name=font_info["family_name"]["value"],
-                subfamily_name=font_info["subfamily_name"]["value"],
-                us_width_class=str(font_info["us_width_class"]["value"]),
-                us_weight_class=str(font_info["us_weight_class"]["value"]),
-                is_regular=str(int(font.is_regular)),
-                is_italic=str(int(font.is_italic)),
-                is_oblique=str(int(font.is_oblique)),
-                is_bold=str(int(font.is_bold)),
-            )
-            rows.append(row)
-        except Exception as e:
-            generic_error_message(e)
-
-    table = Table(box=box.HORIZONTALS)
-    table.add_column("#", justify="right")
-    table.add_column("File name")
-    table.add_column("Family name")
-    table.add_column("Style name")
-    table.add_column("Width", justify="right")
-    table.add_column("Weight", justify="right")
-    table.add_column("Regular", justify="right")
-    table.add_column("Italic", justify="right")
-    table.add_column("Bold", justify="right")
-    table.add_column("Oblique", justify="right")
-    table.header_style = "bold cyan"
-
-    for i, row in enumerate(rows, start=1):
-        table.add_row(
-            str(i),
-            row["file_name"],
-            row["family_name"],
-            row["subfamily_name"],
-            row["us_width_class"],
-            row["us_weight_class"],
-            row["is_regular"],
-            row["is_italic"],
-            row["is_bold"],
-            row["is_oblique"],
-        )
-
-    console = Console()
-    console.print(table, highlight=True)
-
-
-def print_instances(variable_font: VariableFont):
-    """
-    Prints the named instances of a variable font
-
-    :param variable_font: The VariableFont object
-    :type variable_font: VariableFont
-    """
-    table = Table(
-        title="\nftCLI - Variable Font Instances Viewer",
-        title_style="bold green",
-        header_style="bold cyan",
-        caption=f"{variable_font.reader.file.name}",
-    )
-    instances = variable_font.get_instances()
-    table.add_section()
-    table.add_column("#")
-    axes = variable_font.get_axes()
-    for axis in axes:
-        table.add_column(axis.axisTag)
-    table.add_column("subfamilyNameID")
-    table.add_column("postscriptNameID")
-
-    for count, instance in enumerate(instances, start=1):
-        subfamily_name = (
-            f"{instance.subfamilyNameID}: " f"{variable_font['name'].getDebugName(instance.subfamilyNameID)}"
-        )
-        postscript_name = (
-            f"{instance.postscriptNameID}: " f"{variable_font['name'].getDebugName(instance.postscriptNameID)}"
-        )
-        table.add_row(
-            str(count),
-            *[str(v) for k, v in instance.coordinates.items() if k in [a.axisTag for a in axes]],
-            subfamily_name,
-            postscript_name,
-        )
-
-    console = Console()
-    console.print(table)
-
-
-def print_font_info(font: Font):
-    """
-    Prints a table with the font's basic information, vertical metrics, font tables, and font features
-
-    :param font: The Font object to print information about
-    :type font: Font
-    """
-
-    terminal_width = min(90, get_terminal_size()[0] - 1)
-
-    table = Table(
-        title="\nftCLI - Font Info Viewer",
-        title_style="bold green",
-        caption=f"{font.reader.file.name}",
-        show_header=False,
-    )
-
-    font_info = font.get_font_info()
-    font_v_metrics = font.get_font_v_metrics()
-    feature_tags = font.get_font_feature_tags()
-
-    sub_table_1 = Table(box=None, show_header=False)
-    for v in font_info.values():
-        if v["label"] == "File name":
-            v["value"] = os.path.basename(v["value"])
-        sub_table_1.add_row(f"[bold cyan]{v['label'].ljust(16)}[reset] : {str(v['value'])}")
-
-    sub_table_2 = Table(box=None, show_header=False)
-    for v in font_v_metrics["os2_metrics"]:
-        sub_table_2.add_row(f"[bold cyan]{v['label'].ljust(16)}[reset] : {str(v['value']).rjust(4)}")
-
-    sub_table_3 = Table(box=None, show_header=False)
-    for v in font_v_metrics["hhea_metrics"]:
-        sub_table_3.add_row(f"[bold cyan]{v['label'].ljust(16)}[reset] : {str(v['value']).rjust(4)}")
-
-    sub_table_4 = Table(box=None, show_header=False)
-    for v in font_v_metrics["head_metrics"]:
-        sub_table_4.add_row(f"[bold cyan]{v['label'].ljust(16)}[reset] : {str(v['value']).rjust(4)}")
-
-    table.add_row("[bold green]BASIC INFORMATION")
-    table.add_section()
-    table.add_row(sub_table_1)
-    table.add_section()
-    table.add_row("[bold green]VERTICAL METRICS")
-    table.add_section()
-    table.add_row("[bold magenta]OS/2 table")
-    table.add_row(sub_table_2)
-    table.add_row("\n[bold magenta]hhea table")
-    table.add_row(sub_table_3)
-    table.add_row("\n[bold magenta]head table")
-    table.add_row(sub_table_4)
-    table.add_section()
-    table.add_row(f"[bold green]FONT TABLES[reset] ({len(font)})")
-    table.add_section()
-    table.add_row(
-        wrap_string(
-            string=", ".join([t for t in font.keys()]),
-            initial_indent=0,
-            indent=0,
-            width=terminal_width,
-        )
-    )
-    if len(feature_tags) > 0:
-        table.add_section()
-        table.add_row(f"[bold green]FONT FEATURES[reset] ({len(feature_tags)})")
-        table.add_section()
-        table.add_row(
-            wrap_string(
-                string=", ".join([str(t) for t in feature_tags]),
-                initial_indent=0,
-                indent=0,
-                width=terminal_width,
-            )
-        )
-
-    console = Console()
-    console.print(table)
-
-
-def print_font_names(font: Font, max_lines: int = None, minimal: bool = False):
-    """
-    Prints the names in the name table and in the CFF table if present
-
-    :param font: The Font object to print the names from
-    :type font: Font
-    :param max_lines: The maximum number of lines to print for each namerecord string. If the name string is longer than
-        this, it will be truncated
-    :param minimal: Prints only namerecords with nameID in 1, 2, 3, 4, 5, 6, 16, 17, 18, 21, 22, 25
-    :type minimal: bool
-    """
-    terminal_width = min(90, get_terminal_size()[0] - 1)
-
-    table = Table(
-        title="\nftCLI - Name Table Viewer",
-        show_header=False,
-        title_style="bold green",
-    )
-
-    name_table: TableName() = font["name"]
-
-    subtables = []
-    for name in name_table.names:
-        subtables.append((name.platformID, name.platEncID, name.langID))
-
-    # Remove duplicates and sort subtables by platformID
-    subtables = list(set(subtables))
-    subtables = sorted(subtables, key=lambda tup: tup[0])
-
-    for t in subtables:
-        platform_id = t[0]
-        plat_enc_id = t[1]
-        language_id = t[2]
-
-        platform_string = constants.PLATFORMS.get(platform_id)
-        plat_enc_string = ""
-        language_string = ""
-        if platform_id == 1:
-            plat_enc_string = constants.MAC_ENCODING_IDS.get(plat_enc_id)
-            language_string = _MAC_LANGUAGES.get(language_id)
-        if platform_id == 3:
-            plat_enc_string = constants.WINDOWS_ENCODING_IDS.get(plat_enc_id)
-            language_string = _WINDOWS_LANGUAGES.get(language_id)
-
-        table.add_section()
-
-        table.add_row(
-            f"PlatformID: {platform_id} ({platform_string}), PlatEncID: {plat_enc_id} ({plat_enc_string}), "
-            f"LangID: {language_id} ({language_string})",
-            style="bold green",
-        )
-
-        table.add_section()
-
-        names = name_table.filter_namerecords(platform_id=platform_id, plat_enc_id=plat_enc_id, lang_id=language_id)
-        if minimal:
-            names = [n for n in names if n.nameID in (1, 2, 3, 4, 5, 6, 16, 17, 18, 21, 22, 25)]
-
-        for name in names:
-            if name.nameID in constants.NAME_IDS.keys():
-                name_id_description = constants.NAME_IDS.get(name.nameID)
-            else:
-                name_id_description = str(name.nameID)
-
-            row_string = (
-                f"[bold cyan]{str(name.nameID).rjust(5)}[reset] : {name_id_description.ljust(22)} : "
-                f"{name.toUnicode()}"
-            )
-
-            row_string = wrap_string(
-                string=row_string,
-                initial_indent=0,
-                indent=33,
-                max_lines=max_lines,
-                width=terminal_width,
-            )
-
-            table.add_row(row_string)
-        table.add_section()
-
-    if "CFF " in font.keys():
-        cff_table = font["CFF "]
-        table.add_section()
-        table.add_row("CFF Names", style="bold green")
-        table.add_section()
-
-        cff_names_to_skip = [
-            "UnderlinePosition",
-            "UnderlineThickness",
-            "FontMatrix",
-            "FontBBox",
-            "charset",
-            "Encoding",
-            "Private",
-            "CharStrings",
-            "isFixedPitch",
-            "ItalicAngle",
-        ]
-        minimal_cff_names = ["version", "FullName", "FamilyName", "Weight"]
-
-        cff_names = [{k: v} for k, v in cff_table.cff.topDictIndex[0].rawDict.items() if k not in cff_names_to_skip]
-
-        if minimal:
-            cff_names = [{k: v} for k, v in cff_table.cff.topDictIndex[0].rawDict.items() if k in minimal_cff_names]
-
-        table.add_row("[bold cyan]{0:<30}".format("fontNames") + "[reset] : " + str(cff_table.cff.fontNames))
-        for cff_name in cff_names:
-            for k, v in cff_name.items():
-                row_string = "[bold cyan]{0:<30}".format(k) + "[reset] : " + str(v)
-                row_string = wrap_string(
-                    string=row_string,
-                    initial_indent=0,
-                    indent=33,
-                    max_lines=max_lines,
-                    width=terminal_width,
-                )
-                table.add_row(row_string)
-
-    console = Console()
-    console.print(table)
-
-
-def print_os2_table(font: Font):
-    """
-    Converts the OS/2 table to a dictionary, and then prints it out in a table
-
-    :param font: The font object to print the OS/2 table from
-    :type font: Font
-    """
-    os2_table: TableOS2 = font["OS/2"]
-
-    table = Table(
-        title="\nftCLI - OS/2 Table Viewer",
-        show_header=False,
-        title_style="bold green",
-        caption=font.reader.file.name,
-    )
-
-    os2_dict = os2_table.to_dict()
-
-    for k, v in os2_dict.items():
-        table.add_row(f"[bold cyan]{k.ljust(20)}[reset] : {v}")
-        if k == "tableTag":
-            table.add_section()
-
-    console = Console()
-    console.print(table)
+import os.path
+from shutil import get_terminal_size
+
+from fontTools.ttLib.tables._n_a_m_e import _MAC_LANGUAGES, _WINDOWS_LANGUAGES
+from rich import box
+from rich.console import Console
+from rich.table import Table
+
+from foundryToolsCLI.Lib import constants
+from foundryToolsCLI.Lib.Font import Font
+from foundryToolsCLI.Lib.VFont import VariableFont
+from foundryToolsCLI.Lib.tables.OS_2 import TableOS2
+from foundryToolsCLI.Lib.tables.name import TableName
+from foundryToolsCLI.Lib.utils.click_tools import generic_error_message
+from foundryToolsCLI.Lib.utils.text_tools import wrap_string
+
+
+def print_fonts_list(fonts: list[Font]) -> None:
+    """
+    Prints list of fonts in `input_path` with basic information: Family name, Style name, usWidthClass, usWeightClass,
+    Bold value, Italic value, Oblique value
+    """
+    rows = []
+    for font in fonts:
+        try:
+            font_info = font.get_font_info()
+            row = dict(
+                file_name=os.path.basename(font_info["file_name"]["value"]),
+                family_name=font_info["family_name"]["value"],
+                subfamily_name=font_info["subfamily_name"]["value"],
+                us_width_class=str(font_info["us_width_class"]["value"]),
+                us_weight_class=str(font_info["us_weight_class"]["value"]),
+                is_regular=str(int(font.is_regular)),
+                is_italic=str(int(font.is_italic)),
+                is_oblique=str(int(font.is_oblique)),
+                is_bold=str(int(font.is_bold)),
+            )
+            rows.append(row)
+        except Exception as e:
+            generic_error_message(e)
+
+    table = Table(box=box.HORIZONTALS)
+    table.add_column("#", justify="right")
+    table.add_column("File name")
+    table.add_column("Family name")
+    table.add_column("Style name")
+    table.add_column("Width", justify="right")
+    table.add_column("Weight", justify="right")
+    table.add_column("Regular", justify="right")
+    table.add_column("Italic", justify="right")
+    table.add_column("Bold", justify="right")
+    table.add_column("Oblique", justify="right")
+    table.header_style = "bold cyan"
+
+    for i, row in enumerate(rows, start=1):
+        table.add_row(
+            str(i),
+            row["file_name"],
+            row["family_name"],
+            row["subfamily_name"],
+            row["us_width_class"],
+            row["us_weight_class"],
+            row["is_regular"],
+            row["is_italic"],
+            row["is_bold"],
+            row["is_oblique"],
+        )
+
+    console = Console()
+    console.print(table, highlight=True)
+
+
+def print_instances(variable_font: VariableFont):
+    """
+    Prints the named instances of a variable font
+
+    :param variable_font: The VariableFont object
+    :type variable_font: VariableFont
+    """
+    table = Table(
+        title="\nftCLI - Variable Font Instances Viewer",
+        title_style="bold green",
+        header_style="bold cyan",
+        caption=f"{variable_font.reader.file.name}",
+    )
+    instances = variable_font.get_instances()
+    table.add_section()
+    table.add_column("#")
+    axes = variable_font.get_axes()
+    for axis in axes:
+        table.add_column(axis.axisTag)
+    table.add_column("subfamilyNameID")
+    table.add_column("postscriptNameID")
+
+    for count, instance in enumerate(instances, start=1):
+        subfamily_name = (
+            f"{instance.subfamilyNameID}: " f"{variable_font['name'].getDebugName(instance.subfamilyNameID)}"
+        )
+        postscript_name = (
+            f"{instance.postscriptNameID}: " f"{variable_font['name'].getDebugName(instance.postscriptNameID)}"
+        )
+        table.add_row(
+            str(count),
+            *[str(v) for k, v in instance.coordinates.items() if k in [a.axisTag for a in axes]],
+            subfamily_name,
+            postscript_name,
+        )
+
+    console = Console()
+    console.print(table)
+
+
+def print_font_info(font: Font):
+    """
+    Prints a table with the font's basic information, vertical metrics, font tables, and font features
+
+    :param font: The Font object to print information about
+    :type font: Font
+    """
+
+    terminal_width = min(90, get_terminal_size()[0] - 1)
+
+    table = Table(
+        title="\nftCLI - Font Info Viewer",
+        title_style="bold green",
+        caption=f"{font.reader.file.name}",
+        show_header=False,
+    )
+
+    font_info = font.get_font_info()
+    font_v_metrics = font.get_font_v_metrics()
+    feature_tags = font.get_font_feature_tags()
+
+    sub_table_1 = Table(box=None, show_header=False)
+    for v in font_info.values():
+        if v["label"] == "File name":
+            v["value"] = os.path.basename(v["value"])
+        sub_table_1.add_row(f"[bold cyan]{v['label'].ljust(16)}[reset] : {str(v['value'])}")
+
+    sub_table_2 = Table(box=None, show_header=False)
+    for v in font_v_metrics["os2_metrics"]:
+        sub_table_2.add_row(f"[bold cyan]{v['label'].ljust(16)}[reset] : {str(v['value']).rjust(4)}")
+
+    sub_table_3 = Table(box=None, show_header=False)
+    for v in font_v_metrics["hhea_metrics"]:
+        sub_table_3.add_row(f"[bold cyan]{v['label'].ljust(16)}[reset] : {str(v['value']).rjust(4)}")
+
+    sub_table_4 = Table(box=None, show_header=False)
+    for v in font_v_metrics["head_metrics"]:
+        sub_table_4.add_row(f"[bold cyan]{v['label'].ljust(16)}[reset] : {str(v['value']).rjust(4)}")
+
+    table.add_row("[bold green]BASIC INFORMATION")
+    table.add_section()
+    table.add_row(sub_table_1)
+    table.add_section()
+    table.add_row("[bold green]VERTICAL METRICS")
+    table.add_section()
+    table.add_row("[bold magenta]OS/2 table")
+    table.add_row(sub_table_2)
+    table.add_row("\n[bold magenta]hhea table")
+    table.add_row(sub_table_3)
+    table.add_row("\n[bold magenta]head table")
+    table.add_row(sub_table_4)
+    table.add_section()
+    table.add_row(f"[bold green]FONT TABLES[reset] ({len(font)})")
+    table.add_section()
+    table.add_row(
+        wrap_string(
+            string=", ".join([t for t in font.keys()]),
+            initial_indent=0,
+            indent=0,
+            width=terminal_width,
+        )
+    )
+    if len(feature_tags) > 0:
+        table.add_section()
+        table.add_row(f"[bold green]FONT FEATURES[reset] ({len(feature_tags)})")
+        table.add_section()
+        table.add_row(
+            wrap_string(
+                string=", ".join([str(t) for t in feature_tags]),
+                initial_indent=0,
+                indent=0,
+                width=terminal_width,
+            )
+        )
+
+    console = Console()
+    console.print(table)
+
+
+def print_font_names(font: Font, max_lines: int = None, minimal: bool = False):
+    """
+    Prints the names in the name table and in the CFF table if present
+
+    :param font: The Font object to print the names from
+    :type font: Font
+    :param max_lines: The maximum number of lines to print for each namerecord string. If the name string is longer than
+        this, it will be truncated
+    :param minimal: Prints only namerecords with nameID in 1, 2, 3, 4, 5, 6, 16, 17, 18, 21, 22, 25
+    :type minimal: bool
+    """
+    terminal_width = min(90, get_terminal_size()[0] - 1)
+
+    table = Table(
+        title="\nftCLI - Name Table Viewer",
+        show_header=False,
+        title_style="bold green",
+    )
+
+    name_table: TableName() = font["name"]
+
+    subtables = []
+    for name in name_table.names:
+        subtables.append((name.platformID, name.platEncID, name.langID))
+
+    # Remove duplicates and sort subtables by platformID
+    subtables = list(set(subtables))
+    subtables = sorted(subtables, key=lambda tup: tup[0])
+
+    for t in subtables:
+        platform_id = t[0]
+        plat_enc_id = t[1]
+        language_id = t[2]
+
+        platform_string = constants.PLATFORMS.get(platform_id)
+        plat_enc_string = ""
+        language_string = ""
+        if platform_id == 1:
+            plat_enc_string = constants.MAC_ENCODING_IDS.get(plat_enc_id)
+            language_string = _MAC_LANGUAGES.get(language_id)
+        if platform_id == 3:
+            plat_enc_string = constants.WINDOWS_ENCODING_IDS.get(plat_enc_id)
+            language_string = _WINDOWS_LANGUAGES.get(language_id)
+
+        table.add_section()
+
+        table.add_row(
+            f"PlatformID: {platform_id} ({platform_string}), PlatEncID: {plat_enc_id} ({plat_enc_string}), "
+            f"LangID: {language_id} ({language_string})",
+            style="bold green",
+        )
+
+        table.add_section()
+
+        names = name_table.filter_namerecords(platform_id=platform_id, plat_enc_id=plat_enc_id, lang_id=language_id)
+        if minimal:
+            names = [n for n in names if n.nameID in (1, 2, 3, 4, 5, 6, 16, 17, 18, 21, 22, 25)]
+
+        for name in names:
+            if name.nameID in constants.NAME_IDS.keys():
+                name_id_description = constants.NAME_IDS.get(name.nameID)
+            else:
+                name_id_description = str(name.nameID)
+
+            row_string = (
+                f"[bold cyan]{str(name.nameID).rjust(5)}[reset] : {name_id_description.ljust(22)} : "
+                f"{name.toUnicode()}"
+            )
+
+            row_string = wrap_string(
+                string=row_string,
+                initial_indent=0,
+                indent=33,
+                max_lines=max_lines,
+                width=terminal_width,
+            )
+
+            table.add_row(row_string)
+        table.add_section()
+
+    if "CFF " in font.keys():
+        cff_table = font["CFF "]
+        table.add_section()
+        table.add_row("CFF Names", style="bold green")
+        table.add_section()
+
+        cff_names_to_skip = [
+            "UnderlinePosition",
+            "UnderlineThickness",
+            "FontMatrix",
+            "FontBBox",
+            "charset",
+            "Encoding",
+            "Private",
+            "CharStrings",
+            "isFixedPitch",
+            "ItalicAngle",
+        ]
+        minimal_cff_names = ["version", "FullName", "FamilyName", "Weight"]
+
+        cff_names = [{k: v} for k, v in cff_table.cff.topDictIndex[0].rawDict.items() if k not in cff_names_to_skip]
+
+        if minimal:
+            cff_names = [{k: v} for k, v in cff_table.cff.topDictIndex[0].rawDict.items() if k in minimal_cff_names]
+
+        table.add_row("[bold cyan]{0:<30}".format("fontNames") + "[reset] : " + str(cff_table.cff.fontNames))
+        for cff_name in cff_names:
+            for k, v in cff_name.items():
+                row_string = "[bold cyan]{0:<30}".format(k) + "[reset] : " + str(v)
+                row_string = wrap_string(
+                    string=row_string,
+                    initial_indent=0,
+                    indent=33,
+                    max_lines=max_lines,
+                    width=terminal_width,
+                )
+                table.add_row(row_string)
+
+    console = Console()
+    console.print(table)
+
+
+def print_os2_table(font: Font):
+    """
+    Converts the OS/2 table to a dictionary, and then prints it out in a table
+
+    :param font: The font object to print the OS/2 table from
+    :type font: Font
+    """
+    os2_table: TableOS2 = font["OS/2"]
+
+    table = Table(
+        title="\nftCLI - OS/2 Table Viewer",
+        show_header=False,
+        title_style="bold green",
+        caption=font.reader.file.name,
+    )
+
+    os2_dict = os2_table.to_dict()
+
+    for k, v in os2_dict.items():
+        table.add_row(f"[bold cyan]{k.ljust(20)}[reset] : {v}")
+        if k == "tableTag":
+            table.add_section()
+
+    console = Console()
+    console.print(table)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/CFF_.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/CFF_.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-from fontTools.ttLib import registerCustomTableClass
-from fontTools.ttLib.tables.C_F_F_ import table_C_F_F_
-
-registerCustomTableClass("CFF ", "foundryToolsCLI.Lib.tables.CFF_", "TableCFF")
-
-
-class TableCFF(table_C_F_F_):
-    def get_font_version(self) -> str:
-        """
-        Returns the cff.topDictIndex[0].version value
-
-        :return: a string representing the cff.topDictIndex[0].version
-        """
-        return self.cff.topDictIndex[0].version
-
-    def set_font_version(self, value: str) -> None:
-        """
-        Sets the cff.topDictIndex[0].version value
-
-        :param value: a string representing the new cff.topDictIndex[0].version
-        """
-        setattr(self.cff.topDictIndex[0], "version", value)
-
-    def del_top_dict_names(self, names: list[str]) -> None:
-        """
-        Deletes names from topDictIndex[0]
-
-        :param names: a list of names
-        """
-        top_dict = self.cff.topDictIndex[0]
-        for name in names:
-            try:
-                del top_dict.rawDict[name]
-            except KeyError:
-                pass
-
-    def set_top_dict_names(self, names: dict[str, str]) -> None:
-        top_dict = self.cff.topDictIndex[0]
-        if "fontNames" in names.keys():
-            self.cff.fontNames = [names.get("fontNames")]
-            del names["fontNames"]
-        for attr_name, attr_value in names.items():
-            setattr(top_dict, attr_name, attr_value)
-
-    def top_dict_find_replace(self, old_string: str, new_string: str) -> None:
-        cff_font_names = self.cff.fontNames[0]
-        self.cff.fontNames = [cff_font_names.replace(old_string, new_string).replace("  ", " ").strip()]
-        top_dict = self.cff.topDictIndex[0]
-        attr_list = [
-            "version",
-            "FullName",
-            "FamilyName",
-            "Weight",
-            "Copyright",
-            "Notice",
-        ]
-        for attr_name in attr_list:
-            try:
-                old_value = str(getattr(top_dict, attr_name))
-                new_value = old_value.replace(old_string, new_string).replace("  ", " ").strip()
-                setattr(top_dict, attr_name, new_value)
-            except AttributeError:
-                pass
-
-    def get_fb_ps_name(self) -> str:
-        """
-        Returns the psName to pass to FontBuilder
-
-        :return: a string representing the font's ps name
-        """
-        return self.cff.fontNames[0]
-
-    def get_fb_font_info(self) -> dict:
-        """
-        Returns the fontInfo dict to pass to FontBuilder
-
-        :return: the font info dict
-        """
-        font_info = {
-            key: value
-            for key, value in self.cff.topDictIndex[0].rawDict.items()
-            if key not in ("FontBBox", "charset", "Encoding", "Private", "CharStrings")
-        }
-        return font_info
-
-    def get_fb_private_dict(self) -> dict:
-        """
-        Returns the font privateDict to pass to FontBuilder
-
-        :return: the font info dict
-        """
-        private_dict = {
-            key: value
-            for key, value in self.cff.topDictIndex[0].Private.rawDict.items()
-            if key not in ("Subrs", "defaultWidthX", "nominalWidthX")
-        }
-        return private_dict
+from fontTools.ttLib import registerCustomTableClass
+from fontTools.ttLib.tables.C_F_F_ import table_C_F_F_
+
+registerCustomTableClass("CFF ", "foundryToolsCLI.Lib.tables.CFF_", "TableCFF")
+
+
+class TableCFF(table_C_F_F_):
+    def get_font_version(self) -> str:
+        """
+        Returns the cff.topDictIndex[0].version value
+
+        :return: a string representing the cff.topDictIndex[0].version
+        """
+        return self.cff.topDictIndex[0].version
+
+    def set_font_version(self, value: str) -> None:
+        """
+        Sets the cff.topDictIndex[0].version value
+
+        :param value: a string representing the new cff.topDictIndex[0].version
+        """
+        setattr(self.cff.topDictIndex[0], "version", value)
+
+    def del_top_dict_names(self, names: list[str]) -> None:
+        """
+        Deletes names from topDictIndex[0]
+
+        :param names: a list of names
+        """
+        top_dict = self.cff.topDictIndex[0]
+        for name in names:
+            try:
+                del top_dict.rawDict[name]
+            except KeyError:
+                pass
+
+    def set_top_dict_names(self, names: dict[str, str]) -> None:
+        top_dict = self.cff.topDictIndex[0]
+        if "fontNames" in names.keys():
+            self.cff.fontNames = [names.get("fontNames")]
+            del names["fontNames"]
+        for attr_name, attr_value in names.items():
+            setattr(top_dict, attr_name, attr_value)
+
+    def top_dict_find_replace(self, old_string: str, new_string: str) -> None:
+        cff_font_names = self.cff.fontNames[0]
+        self.cff.fontNames = [cff_font_names.replace(old_string, new_string).replace("  ", " ").strip()]
+        top_dict = self.cff.topDictIndex[0]
+        attr_list = [
+            "version",
+            "FullName",
+            "FamilyName",
+            "Weight",
+            "Copyright",
+            "Notice",
+        ]
+        for attr_name in attr_list:
+            try:
+                old_value = str(getattr(top_dict, attr_name))
+                new_value = old_value.replace(old_string, new_string).replace("  ", " ").strip()
+                setattr(top_dict, attr_name, new_value)
+            except AttributeError:
+                pass
+
+    def get_fb_ps_name(self) -> str:
+        """
+        Returns the psName to pass to FontBuilder
+
+        :return: a string representing the font's ps name
+        """
+        return self.cff.fontNames[0]
+
+    def get_fb_font_info(self) -> dict:
+        """
+        Returns the fontInfo dict to pass to FontBuilder
+
+        :return: the font info dict
+        """
+        font_info = {
+            key: value
+            for key, value in self.cff.topDictIndex[0].rawDict.items()
+            if key not in ("FontBBox", "charset", "Encoding", "Private", "CharStrings")
+        }
+        return font_info
+
+    def get_fb_private_dict(self) -> dict:
+        """
+        Returns the font privateDict to pass to FontBuilder
+
+        :return: the font info dict
+        """
+        private_dict = {
+            key: value
+            for key, value in self.cff.topDictIndex[0].Private.rawDict.items()
+            if key not in ("Subrs", "defaultWidthX", "nominalWidthX")
+        }
+        return private_dict
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/OS_2.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/OS_2.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,397 +1,397 @@
-from fontTools.misc.textTools import num2binary
-from fontTools.ttLib import registerCustomTableClass
-from fontTools.ttLib.tables.O_S_2f_2 import table_O_S_2f_2
-
-from foundryToolsCLI.Lib.utils.bits_tools import is_nth_bit_set, set_nth_bit, unset_nth_bit
-
-registerCustomTableClass("OS/2", "foundryToolsCLI.Lib.tables.OS_2", "TableOS2")
-
-
-class TableOS2(table_O_S_2f_2):
-    def get_weight_class(self) -> int:
-        """
-        Returns the usWeightClass value
-        """
-        return getattr(self, "usWeightClass")
-
-    def set_weight_class(self, value: int) -> None:
-        """
-        Sets the usWeightClass value
-
-        :param value: Integer in range 1-1000
-        :type value: int
-        """
-        if value not in range(1, 1001):
-            return
-        setattr(self, "usWeightClass", value)
-
-    def get_width_class(self):
-        """
-        Returns the usWidthClass value
-        """
-        return getattr(self, "usWidthClass")
-
-    def set_width_class(self, value: int) -> None:
-        """
-        Sets the usWidthClass value
-
-        :param value: Integer in range 1-9
-        :type value: int
-        """
-        if value not in range(1, 10):
-            return
-        setattr(self, "usWidthClass", value)
-
-    def get_vend_id(self) -> str:
-        """
-        Returns the four characters Vendor Code
-
-        :return: a string representing the Vendor identifier
-        """
-        return getattr(self, "achVendID")
-
-    def set_vend_id(self, value: str) -> None:
-        """
-        Sets the achVendID value
-
-        :param value: the four characters Vendor identifier
-        :return: None
-        """
-        setattr(self, "achVendID", value.ljust(4, " ")[0:4])
-
-    def is_italic_bit_set(self) -> bool:
-        """
-        > Returns True if the fsSelection bit 0 (ITALIC) is set, otherwise False
-
-        :return: A boolean value.
-        """
-        return is_nth_bit_set(self.fsSelection, 0)
-
-    def set_italic_bit(self) -> None:
-        """
-        Sets fsSelection bit 0 (ITALIC)
-        """
-        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 0))
-
-    def clear_italic_bit(self) -> None:
-        """
-        Clears fsSelection bit 0 (ITALIC)
-        """
-        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 0))
-
-    def is_bold_bit_set(self) -> bool:
-        """
-        > Returns True if the fsSelection bit 5 (BOLD) is set, otherwise False
-
-        :return: A boolean value.
-        """
-        return is_nth_bit_set(self.fsSelection, 5)
-
-    def set_bold_bit(self) -> None:
-        """
-        Sets fsSelection bit 5 (BOLD)
-        """
-        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 5))
-
-    def clear_bold_bit(self) -> None:
-        """
-        Clears fsSelection bit 5 (BOLD)
-        """
-        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 5))
-
-    def is_regular_bit_set(self) -> bool:
-        """
-        > Returns True if the fsSelection bit 6 (REGULAR) is set, otherwise False
-
-        :return: A boolean value.
-        """
-        return is_nth_bit_set(self.fsSelection, 6)
-
-    def set_regular_bit(self) -> None:
-        """
-        Sets fsSelection bit 6 (REGULAR)
-        """
-        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 6))
-
-    def clear_regular_bit(self) -> None:
-        """
-        Clears fsSelection bit 6 (REGULAR)
-        """
-        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 6))
-
-    def is_use_typo_metrics_bit_set(self) -> bool:
-        """
-        > Returns True if the fsSelection bit 7 (USE_TYPO_METRICS) is set, otherwise False
-
-        :return: A boolean value.
-        """
-        return is_nth_bit_set(self.fsSelection, 7)
-
-    def set_use_typo_metrics_bit(self) -> None:
-        """
-        Sets fsSelection bit 7 (USE_TYPO_METRICS) if OS/2 table version is greater than 3
-        """
-        if self.version < 4:
-            print("fsSelection bit 7 is only defined in OS/2 version 4 and up.")
-            return
-        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 7))
-
-    def clear_use_typo_metrics_bit(self) -> None:
-        """
-        Clears fsSelection bit 7 (USE_TYPO_METRICS)
-        """
-        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 7))
-
-    # WWS bit (OS/2.fsSelection bit 8)
-
-    def is_wws_bit_set(self) -> bool:
-        """
-        > Returns True if the fsSelection bit 8 (WWS) is set, otherwise False
-
-        :return: A boolean value.
-        """
-        return is_nth_bit_set(self.fsSelection, 8)
-
-    def set_wws_consistent_bit(self) -> None:
-        """
-        Sets fsSelection bit 8 (WWS) if OS/2 table version is greater than 3
-        """
-        if self.version < 4:
-            print("WARNING: fsSelection bit 8 is only defined in OS/2 version 4 and up.")
-            return
-        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 8))
-
-    def clear_wws_consistent_bit(self) -> None:
-        """
-        Clears fsSelection bit 8 (WWS)
-        """
-        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 8))
-
-    def is_oblique_bit_set(self) -> bool:
-        """
-        > Returns True if the fsSelection bit 9 (OBLIQUE) is set, otherwise False
-
-        :return: A boolean value.
-        """
-        return is_nth_bit_set(self.fsSelection, 9)
-
-    def set_oblique_bit(self) -> None:
-        """
-        Sets fsSelection bit 9 (OBLIQUE) if OS/2 table version is greater than 3
-        """
-        if self.version < 4:
-            print("WARNING: fsSelection bit 9 is only defined in OS/2 version 4 and up.")
-            return
-        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 9))
-
-    def clear_oblique_bit(self):
-        """
-        Clears fsSelection bit 9 (OBLIQUE)
-        """
-        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 9))
-
-    def is_underscore_bit_set(self) -> bool:
-        return is_nth_bit_set(self.fsSelection, 1)
-
-    def set_underscore_bit(self) -> None:
-        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 1))
-
-    def clear_underscore_bit(self) -> None:
-        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 1))
-
-    def is_negative_bit_set(self) -> bool:
-        return is_nth_bit_set(self.fsSelection, 2)
-
-    def set_negative_bit(self) -> None:
-        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 2))
-
-    def clear_negative_bit(self) -> None:
-        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 2))
-
-    def is_outlined_bit_set(self) -> bool:
-        return is_nth_bit_set(self.fsSelection, 3)
-
-    def set_outlined_bit(self) -> None:
-        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 3))
-
-    def clear_outlined_bit(self) -> None:
-        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 3))
-
-    def is_strikeout_bit_set(self) -> bool:
-        return is_nth_bit_set(self.fsSelection, 4)
-
-    def set_strikeout_bit(self) -> None:
-        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 4))
-
-    def clear_strikeout_bit(self) -> None:
-        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 4))
-
-    # Embed level (OS/2.fsType bits 0-3)
-
-    def set_embed_level(self, value: int) -> None:
-        """
-        Sets the embedding level (fsType bits 0-3) of the font
-
-        :param value: The embedding level you want to set
-        :type value: int
-        """
-        if value == 0:
-            for b in (0, 1, 2, 3):
-                setattr(self, "fsType", unset_nth_bit(self.fsType, b))
-        elif value == 2:
-            for b in (0, 2, 3):
-                setattr(self, "fsType", unset_nth_bit(self.fsType, b))
-            setattr(self, "fsType", set_nth_bit(self.fsType, 1))
-        elif value == 4:
-            for b in (0, 1, 3):
-                setattr(self, "fsType", unset_nth_bit(self.fsType, b))
-            setattr(self, "fsType", set_nth_bit(self.fsType, 2))
-        elif value == 8:
-            for b in (0, 1, 2):
-                setattr(self, "fsType", unset_nth_bit(self.fsType, b))
-            setattr(self, "fsType", set_nth_bit(self.fsType, 3))
-        else:
-            return
-
-    def get_embed_level(self) -> int:
-        """
-        Converts the fsType value to a binary string, then takes the last 8 bits of that string, converts it to an
-        integer, and returns it
-
-        :return: The embedding level of the font.
-        """
-        return int(num2binary(self.fsType, 16)[9:17], 2)
-
-    def is_no_subsetting_bit_set(self) -> bool:
-        """
-        > Returns True if the fsType bit 8 (NO_SUBSETTING) is set, otherwise False
-
-        :return: A boolean value.
-        """
-        return is_nth_bit_set(self.fsType, 8)
-
-    def set_no_subsetting_bit(self) -> None:
-        """
-        Sets fsType bit 8 (NO_SUBSETTING)
-        """
-        setattr(self, "fsType", set_nth_bit(self.fsType, 8))
-
-    def clear_no_subsetting_bit(self) -> None:
-        """
-        Clears fsType bit 8 (NO_SUBSETTING)
-        """
-        setattr(self, "fsType", unset_nth_bit(self.fsType, 8))
-
-    # Bitmap embedding only bit (OS/2.fsType bit 9)
-
-    def is_bitmap_embed_only_bit_set(self) -> bool:
-        """
-        > Returns True if the fsType bit 9 (BITMAP_EMBEDDING_ONLY) is set, otherwise False
-
-        :return: A boolean value.
-        """
-        return is_nth_bit_set(self.fsType, 9)
-
-    def set_bitmap_embed_only_bit(self) -> None:
-        """
-        Sets fsType bit 9 (BITMAP_EMBEDDING_ONLY)
-        """
-        setattr(self, "fsType", set_nth_bit(self.fsType, 9))
-
-    def clear_bitmap_embed_only_bit(self) -> None:
-        """
-        Clears fsType bit 9 (BITMAP_EMBEDDING_ONLY)
-        """
-        setattr(self, "fsType", unset_nth_bit(self.fsType, 9))
-
-    def set_cap_height(self, cap_height: int) -> None:
-        """
-        Sets the sCapHeight value
-
-        :param cap_height: Integer
-        """
-        if self.version < 2:
-            return
-        setattr(self, "sCapHeight", cap_height)
-
-    def set_x_height(self, x_height: int) -> None:
-        """
-        Sets the sxHeight value
-
-        :param x_height: Integer
-        """
-        if self.version < 2:
-            return
-        setattr(self, "sxHeight", x_height)
-
-    def set_max_context(self, max_context: int) -> None:
-        """
-        Sets the usMaxContext value
-
-        :param max_context: Integer
-        """
-        if self.version < 2:
-            return
-        setattr(self, "usMaxContext", max_context)
-
-    def set_default_char(self, default_char: int) -> None:
-        """
-        Sets the usDefaultChar value
-
-        :param default_char: Integer
-        """
-        if self.version < 2:
-            return
-        setattr(self, "usDefaultChar", default_char)
-
-    def set_break_char(self, break_char: int) -> None:
-        """
-        Sets the usBreakChar value
-
-        :param break_char: Integer
-        """
-        if self.version < 2:
-            return
-        setattr(self, "usBreakChar", break_char)
-
-    def set_codepage_ranges(self, codepage_ranges) -> None:
-        """
-        Sets the ulCodePageRange1 and ulCodePageRange2 attributes if the OS/2 table version is greater than 1.
-
-        :param codepage_ranges: two bitfields of the supported codepages
-        """
-        if self.version < 1:
-            return
-        setattr(self, "ulCodePageRange1", codepage_ranges[0])
-        setattr(self, "ulCodePageRange2", codepage_ranges[1])
-
-    def get_codepage_ranges(self) -> tuple[int, int]:
-        if self.version >= 1:
-            return getattr(self, "ulCodePageRange1"), getattr(self, "ulCodePageRange2")
-
-    def to_dict(self) -> dict:
-        """
-        Converts the OS/2 table to a dictionary
-
-        :return: A dictionary of the OS/2 table.
-        """
-        os2_to_dict = {}
-        for k, v in self.__dict__.items():
-            if k in (
-                "ulUnicodeRange1",
-                "ulUnicodeRange2",
-                "ulUnicodeRange3",
-                "ulUnicodeRange4",
-                "ulCodePageRange1",
-                "ulCodePageRange2",
-            ):
-                value = num2binary(v)
-            elif k in ("fsSelection", "fsType"):
-                value = num2binary(v, 16)
-            elif k == "panose":
-                value = ", ".join([str(i) for i in v.__dict__.values()])
-            else:
-                value = str(v)
-            os2_to_dict[k] = value
-
-        return os2_to_dict
+from fontTools.misc.textTools import num2binary
+from fontTools.ttLib import registerCustomTableClass
+from fontTools.ttLib.tables.O_S_2f_2 import table_O_S_2f_2
+
+from foundryToolsCLI.Lib.utils.bits_tools import is_nth_bit_set, set_nth_bit, unset_nth_bit
+
+registerCustomTableClass("OS/2", "foundryToolsCLI.Lib.tables.OS_2", "TableOS2")
+
+
+class TableOS2(table_O_S_2f_2):
+    def get_weight_class(self) -> int:
+        """
+        Returns the usWeightClass value
+        """
+        return getattr(self, "usWeightClass")
+
+    def set_weight_class(self, value: int) -> None:
+        """
+        Sets the usWeightClass value
+
+        :param value: Integer in range 1-1000
+        :type value: int
+        """
+        if value not in range(1, 1001):
+            return
+        setattr(self, "usWeightClass", value)
+
+    def get_width_class(self):
+        """
+        Returns the usWidthClass value
+        """
+        return getattr(self, "usWidthClass")
+
+    def set_width_class(self, value: int) -> None:
+        """
+        Sets the usWidthClass value
+
+        :param value: Integer in range 1-9
+        :type value: int
+        """
+        if value not in range(1, 10):
+            return
+        setattr(self, "usWidthClass", value)
+
+    def get_vend_id(self) -> str:
+        """
+        Returns the four characters Vendor Code
+
+        :return: a string representing the Vendor identifier
+        """
+        return getattr(self, "achVendID")
+
+    def set_vend_id(self, value: str) -> None:
+        """
+        Sets the achVendID value
+
+        :param value: the four characters Vendor identifier
+        :return: None
+        """
+        setattr(self, "achVendID", value.ljust(4, " ")[0:4])
+
+    def is_italic_bit_set(self) -> bool:
+        """
+        > Returns True if the fsSelection bit 0 (ITALIC) is set, otherwise False
+
+        :return: A boolean value.
+        """
+        return is_nth_bit_set(self.fsSelection, 0)
+
+    def set_italic_bit(self) -> None:
+        """
+        Sets fsSelection bit 0 (ITALIC)
+        """
+        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 0))
+
+    def clear_italic_bit(self) -> None:
+        """
+        Clears fsSelection bit 0 (ITALIC)
+        """
+        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 0))
+
+    def is_bold_bit_set(self) -> bool:
+        """
+        > Returns True if the fsSelection bit 5 (BOLD) is set, otherwise False
+
+        :return: A boolean value.
+        """
+        return is_nth_bit_set(self.fsSelection, 5)
+
+    def set_bold_bit(self) -> None:
+        """
+        Sets fsSelection bit 5 (BOLD)
+        """
+        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 5))
+
+    def clear_bold_bit(self) -> None:
+        """
+        Clears fsSelection bit 5 (BOLD)
+        """
+        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 5))
+
+    def is_regular_bit_set(self) -> bool:
+        """
+        > Returns True if the fsSelection bit 6 (REGULAR) is set, otherwise False
+
+        :return: A boolean value.
+        """
+        return is_nth_bit_set(self.fsSelection, 6)
+
+    def set_regular_bit(self) -> None:
+        """
+        Sets fsSelection bit 6 (REGULAR)
+        """
+        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 6))
+
+    def clear_regular_bit(self) -> None:
+        """
+        Clears fsSelection bit 6 (REGULAR)
+        """
+        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 6))
+
+    def is_use_typo_metrics_bit_set(self) -> bool:
+        """
+        > Returns True if the fsSelection bit 7 (USE_TYPO_METRICS) is set, otherwise False
+
+        :return: A boolean value.
+        """
+        return is_nth_bit_set(self.fsSelection, 7)
+
+    def set_use_typo_metrics_bit(self) -> None:
+        """
+        Sets fsSelection bit 7 (USE_TYPO_METRICS) if OS/2 table version is greater than 3
+        """
+        if self.version < 4:
+            print("fsSelection bit 7 is only defined in OS/2 version 4 and up.")
+            return
+        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 7))
+
+    def clear_use_typo_metrics_bit(self) -> None:
+        """
+        Clears fsSelection bit 7 (USE_TYPO_METRICS)
+        """
+        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 7))
+
+    # WWS bit (OS/2.fsSelection bit 8)
+
+    def is_wws_bit_set(self) -> bool:
+        """
+        > Returns True if the fsSelection bit 8 (WWS) is set, otherwise False
+
+        :return: A boolean value.
+        """
+        return is_nth_bit_set(self.fsSelection, 8)
+
+    def set_wws_consistent_bit(self) -> None:
+        """
+        Sets fsSelection bit 8 (WWS) if OS/2 table version is greater than 3
+        """
+        if self.version < 4:
+            print("WARNING: fsSelection bit 8 is only defined in OS/2 version 4 and up.")
+            return
+        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 8))
+
+    def clear_wws_consistent_bit(self) -> None:
+        """
+        Clears fsSelection bit 8 (WWS)
+        """
+        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 8))
+
+    def is_oblique_bit_set(self) -> bool:
+        """
+        > Returns True if the fsSelection bit 9 (OBLIQUE) is set, otherwise False
+
+        :return: A boolean value.
+        """
+        return is_nth_bit_set(self.fsSelection, 9)
+
+    def set_oblique_bit(self) -> None:
+        """
+        Sets fsSelection bit 9 (OBLIQUE) if OS/2 table version is greater than 3
+        """
+        if self.version < 4:
+            print("WARNING: fsSelection bit 9 is only defined in OS/2 version 4 and up.")
+            return
+        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 9))
+
+    def clear_oblique_bit(self):
+        """
+        Clears fsSelection bit 9 (OBLIQUE)
+        """
+        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 9))
+
+    def is_underscore_bit_set(self) -> bool:
+        return is_nth_bit_set(self.fsSelection, 1)
+
+    def set_underscore_bit(self) -> None:
+        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 1))
+
+    def clear_underscore_bit(self) -> None:
+        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 1))
+
+    def is_negative_bit_set(self) -> bool:
+        return is_nth_bit_set(self.fsSelection, 2)
+
+    def set_negative_bit(self) -> None:
+        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 2))
+
+    def clear_negative_bit(self) -> None:
+        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 2))
+
+    def is_outlined_bit_set(self) -> bool:
+        return is_nth_bit_set(self.fsSelection, 3)
+
+    def set_outlined_bit(self) -> None:
+        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 3))
+
+    def clear_outlined_bit(self) -> None:
+        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 3))
+
+    def is_strikeout_bit_set(self) -> bool:
+        return is_nth_bit_set(self.fsSelection, 4)
+
+    def set_strikeout_bit(self) -> None:
+        setattr(self, "fsSelection", set_nth_bit(self.fsSelection, 4))
+
+    def clear_strikeout_bit(self) -> None:
+        setattr(self, "fsSelection", unset_nth_bit(self.fsSelection, 4))
+
+    # Embed level (OS/2.fsType bits 0-3)
+
+    def set_embed_level(self, value: int) -> None:
+        """
+        Sets the embedding level (fsType bits 0-3) of the font
+
+        :param value: The embedding level you want to set
+        :type value: int
+        """
+        if value == 0:
+            for b in (0, 1, 2, 3):
+                setattr(self, "fsType", unset_nth_bit(self.fsType, b))
+        elif value == 2:
+            for b in (0, 2, 3):
+                setattr(self, "fsType", unset_nth_bit(self.fsType, b))
+            setattr(self, "fsType", set_nth_bit(self.fsType, 1))
+        elif value == 4:
+            for b in (0, 1, 3):
+                setattr(self, "fsType", unset_nth_bit(self.fsType, b))
+            setattr(self, "fsType", set_nth_bit(self.fsType, 2))
+        elif value == 8:
+            for b in (0, 1, 2):
+                setattr(self, "fsType", unset_nth_bit(self.fsType, b))
+            setattr(self, "fsType", set_nth_bit(self.fsType, 3))
+        else:
+            return
+
+    def get_embed_level(self) -> int:
+        """
+        Converts the fsType value to a binary string, then takes the last 8 bits of that string, converts it to an
+        integer, and returns it
+
+        :return: The embedding level of the font.
+        """
+        return int(num2binary(self.fsType, 16)[9:17], 2)
+
+    def is_no_subsetting_bit_set(self) -> bool:
+        """
+        > Returns True if the fsType bit 8 (NO_SUBSETTING) is set, otherwise False
+
+        :return: A boolean value.
+        """
+        return is_nth_bit_set(self.fsType, 8)
+
+    def set_no_subsetting_bit(self) -> None:
+        """
+        Sets fsType bit 8 (NO_SUBSETTING)
+        """
+        setattr(self, "fsType", set_nth_bit(self.fsType, 8))
+
+    def clear_no_subsetting_bit(self) -> None:
+        """
+        Clears fsType bit 8 (NO_SUBSETTING)
+        """
+        setattr(self, "fsType", unset_nth_bit(self.fsType, 8))
+
+    # Bitmap embedding only bit (OS/2.fsType bit 9)
+
+    def is_bitmap_embed_only_bit_set(self) -> bool:
+        """
+        > Returns True if the fsType bit 9 (BITMAP_EMBEDDING_ONLY) is set, otherwise False
+
+        :return: A boolean value.
+        """
+        return is_nth_bit_set(self.fsType, 9)
+
+    def set_bitmap_embed_only_bit(self) -> None:
+        """
+        Sets fsType bit 9 (BITMAP_EMBEDDING_ONLY)
+        """
+        setattr(self, "fsType", set_nth_bit(self.fsType, 9))
+
+    def clear_bitmap_embed_only_bit(self) -> None:
+        """
+        Clears fsType bit 9 (BITMAP_EMBEDDING_ONLY)
+        """
+        setattr(self, "fsType", unset_nth_bit(self.fsType, 9))
+
+    def set_cap_height(self, cap_height: int) -> None:
+        """
+        Sets the sCapHeight value
+
+        :param cap_height: Integer
+        """
+        if self.version < 2:
+            return
+        setattr(self, "sCapHeight", cap_height)
+
+    def set_x_height(self, x_height: int) -> None:
+        """
+        Sets the sxHeight value
+
+        :param x_height: Integer
+        """
+        if self.version < 2:
+            return
+        setattr(self, "sxHeight", x_height)
+
+    def set_max_context(self, max_context: int) -> None:
+        """
+        Sets the usMaxContext value
+
+        :param max_context: Integer
+        """
+        if self.version < 2:
+            return
+        setattr(self, "usMaxContext", max_context)
+
+    def set_default_char(self, default_char: int) -> None:
+        """
+        Sets the usDefaultChar value
+
+        :param default_char: Integer
+        """
+        if self.version < 2:
+            return
+        setattr(self, "usDefaultChar", default_char)
+
+    def set_break_char(self, break_char: int) -> None:
+        """
+        Sets the usBreakChar value
+
+        :param break_char: Integer
+        """
+        if self.version < 2:
+            return
+        setattr(self, "usBreakChar", break_char)
+
+    def set_codepage_ranges(self, codepage_ranges) -> None:
+        """
+        Sets the ulCodePageRange1 and ulCodePageRange2 attributes if the OS/2 table version is greater than 1.
+
+        :param codepage_ranges: two bitfields of the supported codepages
+        """
+        if self.version < 1:
+            return
+        setattr(self, "ulCodePageRange1", codepage_ranges[0])
+        setattr(self, "ulCodePageRange2", codepage_ranges[1])
+
+    def get_codepage_ranges(self) -> tuple[int, int]:
+        if self.version >= 1:
+            return getattr(self, "ulCodePageRange1"), getattr(self, "ulCodePageRange2")
+
+    def to_dict(self) -> dict:
+        """
+        Converts the OS/2 table to a dictionary
+
+        :return: A dictionary of the OS/2 table.
+        """
+        os2_to_dict = {}
+        for k, v in self.__dict__.items():
+            if k in (
+                "ulUnicodeRange1",
+                "ulUnicodeRange2",
+                "ulUnicodeRange3",
+                "ulUnicodeRange4",
+                "ulCodePageRange1",
+                "ulCodePageRange2",
+            ):
+                value = num2binary(v)
+            elif k in ("fsSelection", "fsType"):
+                value = num2binary(v, 16)
+            elif k == "panose":
+                value = ", ".join([str(i) for i in v.__dict__.values()])
+            else:
+                value = str(v)
+            os2_to_dict[k] = value
+
+        return os2_to_dict
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/head.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/head.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from fontTools.ttLib import registerCustomTableClass
-from fontTools.ttLib.tables._h_e_a_d import table__h_e_a_d
-
-from foundryToolsCLI.Lib.utils.bits_tools import is_nth_bit_set, set_nth_bit, unset_nth_bit
-
-registerCustomTableClass("head", "foundryToolsCLI.Lib.tables.head", "TableHead")
-
-
-class TableHead(table__h_e_a_d):
-    def get_font_revision(self) -> float:
-        """
-        Returns the 'fontRevision' value in 'head' table
-
-        :return: a float representing the font revision
-        """
-        return getattr(self, "fontRevision")
-
-    def set_font_revision(self, value: float) -> None:
-        """
-        Sets 'fontRevision' value in 'head' table
-
-        :param value: a float representing the font revision
-        """
-        setattr(self, "fontRevision", value)
-
-    def is_bold_bit_set(self):
-        return is_nth_bit_set(getattr(self, "macStyle"), 0)
-
-    def set_bold_bit(self):
-        setattr(self, "macStyle", set_nth_bit(getattr(self, "macStyle"), 0))
-
-    def clear_bold_bit(self):
-        setattr(self, "macStyle", unset_nth_bit(getattr(self, "macStyle"), 0))
-
-    def is_italic_bit_set(self):
-        return is_nth_bit_set(getattr(self, "macStyle"), 1)
-
-    def set_italic_bit(self):
-        setattr(self, "macStyle", set_nth_bit(getattr(self, "macStyle"), 1))
-
-    def clear_italic_bit(self):
-        setattr(self, "macStyle", unset_nth_bit(getattr(self, "macStyle"), 1))
+from fontTools.ttLib import registerCustomTableClass
+from fontTools.ttLib.tables._h_e_a_d import table__h_e_a_d
+
+from foundryToolsCLI.Lib.utils.bits_tools import is_nth_bit_set, set_nth_bit, unset_nth_bit
+
+registerCustomTableClass("head", "foundryToolsCLI.Lib.tables.head", "TableHead")
+
+
+class TableHead(table__h_e_a_d):
+    def get_font_revision(self) -> float:
+        """
+        Returns the 'fontRevision' value in 'head' table
+
+        :return: a float representing the font revision
+        """
+        return getattr(self, "fontRevision")
+
+    def set_font_revision(self, value: float) -> None:
+        """
+        Sets 'fontRevision' value in 'head' table
+
+        :param value: a float representing the font revision
+        """
+        setattr(self, "fontRevision", value)
+
+    def is_bold_bit_set(self):
+        return is_nth_bit_set(getattr(self, "macStyle"), 0)
+
+    def set_bold_bit(self):
+        setattr(self, "macStyle", set_nth_bit(getattr(self, "macStyle"), 0))
+
+    def clear_bold_bit(self):
+        setattr(self, "macStyle", unset_nth_bit(getattr(self, "macStyle"), 0))
+
+    def is_italic_bit_set(self):
+        return is_nth_bit_set(getattr(self, "macStyle"), 1)
+
+    def set_italic_bit(self):
+        setattr(self, "macStyle", set_nth_bit(getattr(self, "macStyle"), 1))
+
+    def clear_italic_bit(self):
+        setattr(self, "macStyle", unset_nth_bit(getattr(self, "macStyle"), 1))
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/hhea.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/hhea.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from fontTools.ttLib import registerCustomTableClass
-from fontTools.ttLib.tables._h_h_e_a import table__h_h_e_a
-
-registerCustomTableClass("hhea", "foundryToolsCLI.Lib.tables.hhea", "TableHhea")
-
-
-class TableHhea(table__h_h_e_a):
-    def set_caret_slope_rise(self, value: int):
-        setattr(self, "caretSlopeRise", value)
-
-    def set_caret_slope_run(self, value: int):
-        setattr(self, "caretSlopeRun", value)
-
-    def set_caret_offset(self, value: int):
-        setattr(self, "caretOffset", value)
-
-    def set_ascent(self, value: int):
-        setattr(self, "ascent", value)
-
-    def set_descent(self, value: int):
-        setattr(self, "descent", value)
-
-    def set_linegap(self, value: int):
-        setattr(self, "lineGap", value)
+from fontTools.ttLib import registerCustomTableClass
+from fontTools.ttLib.tables._h_h_e_a import table__h_h_e_a
+
+registerCustomTableClass("hhea", "foundryToolsCLI.Lib.tables.hhea", "TableHhea")
+
+
+class TableHhea(table__h_h_e_a):
+    def set_caret_slope_rise(self, value: int):
+        setattr(self, "caretSlopeRise", value)
+
+    def set_caret_slope_run(self, value: int):
+        setattr(self, "caretSlopeRun", value)
+
+    def set_caret_offset(self, value: int):
+        setattr(self, "caretOffset", value)
+
+    def set_ascent(self, value: int):
+        setattr(self, "ascent", value)
+
+    def set_descent(self, value: int):
+        setattr(self, "descent", value)
+
+    def set_linegap(self, value: int):
+        setattr(self, "lineGap", value)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/name.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/name.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-from fontTools.ttLib.tables._n_a_m_e import table__n_a_m_e, NameRecord, _MAC_LANGUAGE_CODES, _WINDOWS_LANGUAGE_CODES
-
-from fontTools.ttLib import registerCustomTableClass
-
-registerCustomTableClass("name", "foundryToolsCLI.Lib.tables.name", "TableName")
-
-
-class TableName(table__n_a_m_e):
-    def add_name(
-        self,
-        font,
-        string,
-        name_id: int = None,
-        platform_id: int = None,
-        language_string: str = "en",
-    ) -> None:
-        """
-        Adds a namerecord to the `name` table. If the namerecord already exists, it will be overwritten.
-
-        :param font: the font object
-        :param string: The string to be written to the namerecord
-        :param name_id: The name ID of the namerecord to be added
-        :type name_id: int
-        :param platform_id: 1 = Macintosh, 3 = Windows
-        :type platform_id: int
-        :param language_string: The language of the string, defaults to en
-        :type language_string: str (optional)
-        """
-
-        # Remove the namerecord before writing it to avoid duplicates
-        self.del_names(name_ids=[name_id], platform_id=platform_id, language_string=language_string)
-
-        if platform_id == 1:
-            mac, windows = True, False
-        elif platform_id == 3:
-            mac, windows = False, True
-        else:
-            mac, windows = True, True
-
-        names = {language_string: string}
-
-        self.addMultilingualName(names, ttFont=font, nameID=name_id, windows=windows, mac=mac)
-
-    def del_names(self, name_ids, platform_id=None, language_string=None) -> None:
-        """
-        Deletes all name records that match the given name_ids, optionally filtering by platform_id and/or
-        language_string.
-
-        :param name_ids: A list of name IDs to delete
-        :param platform_id: The platform ID of the name records to delete
-        :param language_string: The language of the name records to delete
-        """
-
-        names = self.filter_namerecords(name_ids=name_ids, platform_id=platform_id, lang_string=language_string)
-
-        for name in names:
-            self.removeNames(name.nameID, name.platformID, name.platEncID, name.langID)
-
-    def filter_namerecords(
-        self, name_ids=None, platform_id=None, plat_enc_id=None, lang_id=None, lang_string=None
-    ) -> list[NameRecord]:
-        """
-        It takes a list of name records, and returns a list of name records that match the given criteria
-
-        :param name_ids: A list of name IDs to filter by
-        :param platform_id: The platform ID of the name record
-        :param plat_enc_id: The platform-specific encoding ID
-        :param lang_id: The language ID of the name record
-        :param lang_string: The string to search for in the name records
-        :return: A list of name records.
-        """
-        filtered_names = self.names
-        if name_ids is not None:
-            filtered_names = [name for name in filtered_names if name.nameID in name_ids]
-        if platform_id is not None:
-            filtered_names = [name for name in filtered_names if name.platformID == platform_id]
-        if plat_enc_id is not None:
-            filtered_names = [name for name in filtered_names if name.platEncID == plat_enc_id]
-        if lang_id is not None:
-            filtered_names = [name for name in filtered_names if name.langID == lang_id]
-        if lang_string is not None:
-            mac_lang_id = _MAC_LANGUAGE_CODES.get(lang_string.lower())
-            win_lang_id = _WINDOWS_LANGUAGE_CODES.get(lang_string.lower())
-            filtered_names = [name for name in filtered_names if name.langID in (mac_lang_id, win_lang_id)]
-        return filtered_names
-
-    def find_replace(
-        self,
-        old_string: str,
-        new_string: str,
-        name_ids_to_include: tuple = (),
-        name_ids_to_skip: tuple = (),
-        platform_id: int = None,
-    ):
-        """
-        This function will find and replace a string in the specified namerecords.
-
-        :param old_string: The string to be replaced
-        :type old_string: str
-        :param new_string: The string to replace the old string with
-        :type new_string: str
-        :param name_ids_to_include: A tuple of nameIDs to include in the search. If left blank, all nameIDs will be
-            included
-        :type name_ids_to_include: tuple
-        :param name_ids_to_skip: A tuple of nameIDs to skip in the search. If left blank, no nameID will be skipped
-        :type name_ids_to_skip: tuple
-        :param platform_id: The platform ID of the name record to be changed
-        :type platform_id: int
-        """
-
-        name_ids = [name.nameID for name in self.names]
-
-        if name_ids_to_include != ():
-            name_ids = [name.nameID for name in self.names if name.nameID in name_ids_to_include]
-
-        if name_ids_to_skip != ():
-            name_ids = [name.nameID for name in self.names if name.nameID not in name_ids_to_skip]
-
-        names = self.filter_namerecords(name_ids=name_ids, platform_id=platform_id)
-
-        for name in self.names:
-            if name in names:
-                if old_string in str(name):
-                    string = str(name).replace(old_string, new_string).replace("  ", " ").strip()
-                    self.setName(
-                        string,
-                        name.nameID,
-                        name.platformID,
-                        name.platEncID,
-                        name.langID,
-                    )
-
-    def append_string(self, name_ids, platform_id=None, language_string=None, prefix=None, suffix=None) -> None:
-        """
-        Appends a prefix, a suffix, or both to the namerecords that match the name IDs, platform ID, and language
-        string.
-
-        :param name_ids: A list of name IDs to filter by
-        :param platform_id: The platform ID of the namerecords where to append/prepend the string
-        :param language_string: The language string to filter by
-        :param prefix: The string to be added to the beginning of the namerecords
-        :param suffix: The string to append to the end of the namerecords
-        """
-
-        names = self.filter_namerecords(name_ids=name_ids, platform_id=platform_id, lang_string=language_string)
-
-        for name in names:
-            string = name.toUnicode()
-            if prefix is not None:
-                string = f"{prefix}{string}"
-            if suffix is not None:
-                string = f"{string}{suffix}"
-
-            self.setName(
-                string=string,
-                nameID=name.nameID,
-                platformID=name.platformID,
-                platEncID=name.platEncID,
-                langID=name.langID,
-            )
-
-    def remove_leading_trailing_spaces(self):
-        for name in self.names:
-            self.setName(
-                str(name).strip(),
-                name.nameID,
-                name.platformID,
-                name.platEncID,
-                name.langID,
-            )
+from fontTools.ttLib.tables._n_a_m_e import table__n_a_m_e, NameRecord, _MAC_LANGUAGE_CODES, _WINDOWS_LANGUAGE_CODES
+
+from fontTools.ttLib import registerCustomTableClass
+
+registerCustomTableClass("name", "foundryToolsCLI.Lib.tables.name", "TableName")
+
+
+class TableName(table__n_a_m_e):
+    def add_name(
+        self,
+        font,
+        string,
+        name_id: int = None,
+        platform_id: int = None,
+        language_string: str = "en",
+    ) -> None:
+        """
+        Adds a namerecord to the `name` table. If the namerecord already exists, it will be overwritten.
+
+        :param font: the font object
+        :param string: The string to be written to the namerecord
+        :param name_id: The name ID of the namerecord to be added
+        :type name_id: int
+        :param platform_id: 1 = Macintosh, 3 = Windows
+        :type platform_id: int
+        :param language_string: The language of the string, defaults to en
+        :type language_string: str (optional)
+        """
+
+        # Remove the namerecord before writing it to avoid duplicates
+        self.del_names(name_ids=[name_id], platform_id=platform_id, language_string=language_string)
+
+        if platform_id == 1:
+            mac, windows = True, False
+        elif platform_id == 3:
+            mac, windows = False, True
+        else:
+            mac, windows = True, True
+
+        names = {language_string: string}
+
+        self.addMultilingualName(names, ttFont=font, nameID=name_id, windows=windows, mac=mac)
+
+    def del_names(self, name_ids, platform_id=None, language_string=None) -> None:
+        """
+        Deletes all name records that match the given name_ids, optionally filtering by platform_id and/or
+        language_string.
+
+        :param name_ids: A list of name IDs to delete
+        :param platform_id: The platform ID of the name records to delete
+        :param language_string: The language of the name records to delete
+        """
+
+        names = self.filter_namerecords(name_ids=name_ids, platform_id=platform_id, lang_string=language_string)
+
+        for name in names:
+            self.removeNames(name.nameID, name.platformID, name.platEncID, name.langID)
+
+    def filter_namerecords(
+        self, name_ids=None, platform_id=None, plat_enc_id=None, lang_id=None, lang_string=None
+    ) -> list[NameRecord]:
+        """
+        It takes a list of name records, and returns a list of name records that match the given criteria
+
+        :param name_ids: A list of name IDs to filter by
+        :param platform_id: The platform ID of the name record
+        :param plat_enc_id: The platform-specific encoding ID
+        :param lang_id: The language ID of the name record
+        :param lang_string: The string to search for in the name records
+        :return: A list of name records.
+        """
+        filtered_names = self.names
+        if name_ids is not None:
+            filtered_names = [name for name in filtered_names if name.nameID in name_ids]
+        if platform_id is not None:
+            filtered_names = [name for name in filtered_names if name.platformID == platform_id]
+        if plat_enc_id is not None:
+            filtered_names = [name for name in filtered_names if name.platEncID == plat_enc_id]
+        if lang_id is not None:
+            filtered_names = [name for name in filtered_names if name.langID == lang_id]
+        if lang_string is not None:
+            mac_lang_id = _MAC_LANGUAGE_CODES.get(lang_string.lower())
+            win_lang_id = _WINDOWS_LANGUAGE_CODES.get(lang_string.lower())
+            filtered_names = [name for name in filtered_names if name.langID in (mac_lang_id, win_lang_id)]
+        return filtered_names
+
+    def find_replace(
+        self,
+        old_string: str,
+        new_string: str,
+        name_ids_to_include: tuple = (),
+        name_ids_to_skip: tuple = (),
+        platform_id: int = None,
+    ):
+        """
+        This function will find and replace a string in the specified namerecords.
+
+        :param old_string: The string to be replaced
+        :type old_string: str
+        :param new_string: The string to replace the old string with
+        :type new_string: str
+        :param name_ids_to_include: A tuple of nameIDs to include in the search. If left blank, all nameIDs will be
+            included
+        :type name_ids_to_include: tuple
+        :param name_ids_to_skip: A tuple of nameIDs to skip in the search. If left blank, no nameID will be skipped
+        :type name_ids_to_skip: tuple
+        :param platform_id: The platform ID of the name record to be changed
+        :type platform_id: int
+        """
+
+        name_ids = [name.nameID for name in self.names]
+
+        if name_ids_to_include != ():
+            name_ids = [name.nameID for name in self.names if name.nameID in name_ids_to_include]
+
+        if name_ids_to_skip != ():
+            name_ids = [name.nameID for name in self.names if name.nameID not in name_ids_to_skip]
+
+        names = self.filter_namerecords(name_ids=name_ids, platform_id=platform_id)
+
+        for name in self.names:
+            if name in names:
+                if old_string in str(name):
+                    string = str(name).replace(old_string, new_string).replace("  ", " ").strip()
+                    self.setName(
+                        string,
+                        name.nameID,
+                        name.platformID,
+                        name.platEncID,
+                        name.langID,
+                    )
+
+    def append_string(self, name_ids, platform_id=None, language_string=None, prefix=None, suffix=None) -> None:
+        """
+        Appends a prefix, a suffix, or both to the namerecords that match the name IDs, platform ID, and language
+        string.
+
+        :param name_ids: A list of name IDs to filter by
+        :param platform_id: The platform ID of the namerecords where to append/prepend the string
+        :param language_string: The language string to filter by
+        :param prefix: The string to be added to the beginning of the namerecords
+        :param suffix: The string to append to the end of the namerecords
+        """
+
+        names = self.filter_namerecords(name_ids=name_ids, platform_id=platform_id, lang_string=language_string)
+
+        for name in names:
+            string = name.toUnicode()
+            if prefix is not None:
+                string = f"{prefix}{string}"
+            if suffix is not None:
+                string = f"{string}{suffix}"
+
+            self.setName(
+                string=string,
+                nameID=name.nameID,
+                platformID=name.platformID,
+                platEncID=name.platEncID,
+                langID=name.langID,
+            )
+
+    def remove_leading_trailing_spaces(self):
+        for name in self.names:
+            self.setName(
+                str(name).strip(),
+                name.nameID,
+                name.platformID,
+                name.platEncID,
+                name.langID,
+            )
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/tables/post.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/post.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from fontTools.ttLib import registerCustomTableClass
-from fontTools.ttLib.tables._p_o_s_t import table__p_o_s_t
-
-registerCustomTableClass("post", "foundryToolsCLI.Lib.tables.post", "TablePost")
-
-
-class TablePost(table__p_o_s_t):
-    def set_italic_angle(self, value: float):
-        setattr(self, "italicAngle", value)
-
-    def set_underline_position(self, value: int):
-        setattr(self, "underlinePosition", value)
-
-    def set_underline_thickness(self, value: int):
-        setattr(self, "underlineThickness", value)
-
-    def set_fixed_pitch(self, value: bool):
-        setattr(self, "isFixedPitch", int(value))
+from fontTools.ttLib import registerCustomTableClass
+from fontTools.ttLib.tables._p_o_s_t import table__p_o_s_t
+
+registerCustomTableClass("post", "foundryToolsCLI.Lib.tables.post", "TablePost")
+
+
+class TablePost(table__p_o_s_t):
+    def set_italic_angle(self, value: float):
+        setattr(self, "italicAngle", value)
+
+    def set_underline_position(self, value: int):
+        setattr(self, "underlinePosition", value)
+
+    def set_underline_thickness(self, value: int):
+        setattr(self, "underlineThickness", value)
+
+    def set_fixed_pitch(self, value: bool):
+        setattr(self, "isFixedPitch", int(value))
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/cli_tools.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/cli_tools.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-import pathlib
-
-import click
-from fontTools.ttLib import TTLibError
-
-from foundryToolsCLI.Lib.Font import Font
-from foundryToolsCLI.Lib.VFont import VariableFont
-
-
-def get_variable_fonts_in_path(input_path: pathlib.Path, recalc_timestamp: bool = False) -> list[VariableFont]:
-    files = []
-    if input_path.is_file():
-        files.append(input_path.resolve())
-    if input_path.is_dir():
-        files = [p.resolve() for p in input_path.iterdir()]
-
-    variable_fonts = []
-    for file in files:
-        try:
-            variable_font = VariableFont(file, recalcTimestamp=recalc_timestamp)
-            variable_fonts.append(variable_font)
-        except (TTLibError, Exception):
-            pass
-
-    return variable_fonts
-
-
-def get_fonts_in_path(
-    input_path: pathlib.Path,
-    recalc_timestamp: bool = False,
-    allow_extensions: list = None,
-    allow_ttf=True,
-    allow_cff=True,
-    allow_static=True,
-    allow_variable=True,
-) -> list[Font]:
-    files = []
-    if input_path.is_file():
-        files.append(input_path.resolve())
-    if input_path.is_dir():
-        files = [p.resolve() for p in input_path.iterdir()]
-
-    fonts = []
-    for file in files:
-        try:
-            font = Font(file, recalcTimestamp=recalc_timestamp)
-            fonts.append(font)
-
-            if allow_extensions:
-                if font.get_real_extension() not in allow_extensions:
-                    fonts.remove(font)
-                    continue
-            if not allow_ttf:
-                if font.is_ttf:
-                    fonts.remove(font)
-                    continue
-            if not allow_cff:
-                if font.is_otf:
-                    fonts.remove(font)
-                    continue
-            if not allow_static:
-                if font.is_static:
-                    fonts.remove(font)
-            if not allow_variable:
-                if font.is_variable:
-                    fonts.remove(font)
-
-        except (TTLibError, Exception):
-            pass
-
-    return fonts
-
-
-def get_output_dir(input_path: pathlib.Path, output_dir: pathlib.Path = None) -> pathlib.Path:
-    """
-    If the output directory is not specified, then the output directory is the directory of the input file if the input
-    is a file, or the input directory if the input is a directory
-
-    :param input_path: The path to the input file or directory
-    :type input_path: str
-    :param output_dir: The output directory, if specified
-    :type output_dir: str
-    :return: The output directory.
-    """
-    if output_dir is not None:
-        return output_dir.resolve()
-    else:
-        if input_path.is_file():
-            return input_path.parent.resolve()
-        else:
-            return input_path.resolve()
-
-
-def initial_check_pass(fonts: list, output_dir: pathlib.Path) -> bool:
-    """
-    Checks if the list of fonts is not empty and if the output directory is writable.
-
-    :param fonts: a list Font objects
-    :param output_dir: the output directory
-    :return: False if one of the checks fails, True if both checks succeed
-    """
-    if not len(fonts) > 0:
-        click.secho(f"[{click.style('FAIL', fg='red')}] No fonts matching the given criteria")
-        return False
-    try:
-        output_dir.mkdir(parents=True, exist_ok=True)
-    except Exception as e:
-        click.secho(f"[{click.style('FAIL', fg='red')}] {e}")
-        return False
-    return True
-
-
-def get_project_files_path(input_path: pathlib.Path) -> pathlib.Path:
-    if input_path.is_file():
-        project_files_path = input_path.parent.joinpath("ftCLI_files")
-    else:
-        project_files_path = input_path.joinpath("ftCLI_files")
-
-    return project_files_path
-
-
-def get_style_mapping_path(input_path: pathlib.Path) -> pathlib.Path:
-    project_files_dir = get_project_files_path(input_path)
-    styles_mapping_file = pathlib.Path.joinpath(project_files_dir, "styles_mapping.json")
-
-    return styles_mapping_file
-
-
-def get_fonts_data_path(input_path: pathlib.Path) -> pathlib.Path:
-    project_files_dir = get_project_files_path(input_path)
-    fonts_data_file = pathlib.Path.joinpath(project_files_dir, "fonts_data.csv")
-
-    return fonts_data_file
+import pathlib
+
+import click
+from fontTools.ttLib import TTLibError
+
+from foundryToolsCLI.Lib.Font import Font
+from foundryToolsCLI.Lib.VFont import VariableFont
+
+
+def get_variable_fonts_in_path(input_path: pathlib.Path, recalc_timestamp: bool = False) -> list[VariableFont]:
+    files = []
+    if input_path.is_file():
+        files.append(input_path.resolve())
+    if input_path.is_dir():
+        files = [p.resolve() for p in input_path.iterdir()]
+
+    variable_fonts = []
+    for file in files:
+        try:
+            variable_font = VariableFont(file, recalcTimestamp=recalc_timestamp)
+            variable_fonts.append(variable_font)
+        except (TTLibError, Exception):
+            pass
+
+    return variable_fonts
+
+
+def get_fonts_in_path(
+    input_path: pathlib.Path,
+    recalc_timestamp: bool = False,
+    allow_extensions: list = None,
+    allow_ttf=True,
+    allow_cff=True,
+    allow_static=True,
+    allow_variable=True,
+) -> list[Font]:
+    files = []
+    if input_path.is_file():
+        files.append(input_path.resolve())
+    if input_path.is_dir():
+        files = [p.resolve() for p in input_path.iterdir()]
+
+    fonts = []
+    for file in files:
+        try:
+            font = Font(file, recalcTimestamp=recalc_timestamp)
+            fonts.append(font)
+
+            if allow_extensions:
+                if font.get_real_extension() not in allow_extensions:
+                    fonts.remove(font)
+                    continue
+            if not allow_ttf:
+                if font.is_ttf:
+                    fonts.remove(font)
+                    continue
+            if not allow_cff:
+                if font.is_otf:
+                    fonts.remove(font)
+                    continue
+            if not allow_static:
+                if font.is_static:
+                    fonts.remove(font)
+            if not allow_variable:
+                if font.is_variable:
+                    fonts.remove(font)
+
+        except (TTLibError, Exception):
+            pass
+
+    return fonts
+
+
+def get_output_dir(input_path: pathlib.Path, output_dir: pathlib.Path = None) -> pathlib.Path:
+    """
+    If the output directory is not specified, then the output directory is the directory of the input file if the input
+    is a file, or the input directory if the input is a directory
+
+    :param input_path: The path to the input file or directory
+    :type input_path: str
+    :param output_dir: The output directory, if specified
+    :type output_dir: str
+    :return: The output directory.
+    """
+    if output_dir is not None:
+        return output_dir.resolve()
+    else:
+        if input_path.is_file():
+            return input_path.parent.resolve()
+        else:
+            return input_path.resolve()
+
+
+def initial_check_pass(fonts: list, output_dir: pathlib.Path) -> bool:
+    """
+    Checks if the list of fonts is not empty and if the output directory is writable.
+
+    :param fonts: a list Font objects
+    :param output_dir: the output directory
+    :return: False if one of the checks fails, True if both checks succeed
+    """
+    if not len(fonts) > 0:
+        click.secho(f"[{click.style('FAIL', fg='red')}] No fonts matching the given criteria")
+        return False
+    try:
+        output_dir.mkdir(parents=True, exist_ok=True)
+    except Exception as e:
+        click.secho(f"[{click.style('FAIL', fg='red')}] {e}")
+        return False
+    return True
+
+
+def get_project_files_path(input_path: pathlib.Path) -> pathlib.Path:
+    if input_path.is_file():
+        project_files_path = input_path.parent.joinpath("ftCLI_files")
+    else:
+        project_files_path = input_path.joinpath("ftCLI_files")
+
+    return project_files_path
+
+
+def get_style_mapping_path(input_path: pathlib.Path) -> pathlib.Path:
+    project_files_dir = get_project_files_path(input_path)
+    styles_mapping_file = pathlib.Path.joinpath(project_files_dir, "styles_mapping.json")
+
+    return styles_mapping_file
+
+
+def get_fonts_data_path(input_path: pathlib.Path) -> pathlib.Path:
+    project_files_dir = get_project_files_path(input_path)
+    fonts_data_file = pathlib.Path.joinpath(project_files_dir, "fonts_data.csv")
+
+    return fonts_data_file
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/click_tools.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/click_tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,152 +1,150 @@
-import pathlib
-from pathlib import Path
-
-import click
-
-CWD = Path.cwd()
-
-
-def add_options(options):
-    def _add_options(func):
-        for option in reversed(options):
-            func = option(func)
-        return func
-
-    return _add_options
-
-
-def add_file_or_path_argument(dir_okay=True, file_okay=True):
-    _file_or_path_argument = [
-        click.argument(
-            "input_path",
-            type=click.Path(
-                exists=True, resolve_path=True, path_type=pathlib.Path, dir_okay=dir_okay, file_okay=file_okay
-            ),
-        )
-    ]
-    return add_options(_file_or_path_argument)
-
-
-def add_file_argument():
-    return add_file_or_path_argument(dir_okay=False)
-
-
-def add_path_argument():
-    return add_file_or_path_argument(file_okay=False)
-
-
-def add_common_options():
-    _common_options = [
-        click.option(
-            "-out",
-            "--output-dir",
-            type=click.Path(path_type=pathlib.Path, file_okay=False, resolve_path=True),
-            default=None,
-            help="""
-            Specify the directory where output files are to be saved. If the directory doesn't exist, will be created.
-            If output_dir is not specified, files will be saved to the same folder.
-            """,
-        ),
-        click.option(
-            "--recalc-timestamp",
-            is_flag=True,
-            default=False,
-            help="""
-            Keep the original font 'modified' timestamp (head.modified) or set it to current time. By default,
-            original timestamp is kept.
-            """,
-        ),
-        click.option(
-            "--no-overwrite",
-            "overwrite",
-            is_flag=True,
-            default=True,
-            help="""
-            Overwrite existing files or save them to a new file (numbers are appended at the end of file name). By
-            default, files are overwritten.
-            """,
-        ),
-    ]
-    return add_options(_common_options)
-
-
-def file_overwrite_prompt(input_file: Path) -> bool:
-    return click.confirm(
-        f"{click.style(input_file.relative_to(CWD), fg='yellow', bold=True)} already exists. "
-        f"Do you want to overwrite it?"
-    )
-
-
-def file_not_selected_message(file: Path):
-    click.secho(
-        f"[{click.style('SKIP', fg='yellow')}] {file.name} ({click.style('file is not selected', fg='yellow')})"
-    )
-
-
-def no_valid_fonts_message(input_path: Path):
-    if input_path.is_dir():
-        message = f"No valid font files matching the given criteria found in {input_path.name}"
-    else:
-        message = f"{input_path.name} is not a valid font file or doesn't match the given criteria"
-    click.secho(f"[{click.style('FAIL', fg='red')}] {message}")
-
-
-def file_not_exists_message(file: Path):
-    click.secho(
-        f"[{click.style('WARN', fg='bright_yellow')}] {file} {click.style('file does not exist', fg='bright_yellow')}"
-    )
-
-
-def file_not_changed_message(file: Path):
-    click.secho(
-        f"[{click.style('SKIP', fg='bright_yellow')}] {file} ({click.style('no changes made', fg='bright_yellow')})"
-    )
-
-
-def file_saved_message(file: Path):
-    click.secho(f"[{click.style('DONE', fg='green')}] {file} ({click.style('saved', fg='green')})")
-
-
-def generic_success_message(success_message):
-    click.secho(f"[{click.style('PASS', fg='green')}] {success_message}")
-
-
-def generic_info_message(info_message, nl=True):
-    click.secho(f"[{click.style('INFO', fg='cyan')}] {info_message}", nl=nl)
-
-
-def generic_error_message(error_message):
-    click.secho(f"[{click.style('FAIL', fg='red')}] {error_message}")
-
-
-def generic_warning_message(warning_message):
-    click.secho(f"[{click.style('WARN', fg='bright_yellow')}] {warning_message}")
-
-
-def select_instance_coordinates(axes: list) -> dict:
-    click.secho("\nSelect coordinates:")
-    selected_coordinates = {}
-    for a in axes:
-        axis_tag = a.axisTag
-        min_value = a.minValue
-        max_value = a.maxValue
-        coordinates = click.prompt(
-            f"{axis_tag} ({min_value} - {max_value})",
-            type=click.FloatRange(min_value, max_value),
-        )
-        selected_coordinates[axis_tag] = coordinates
-
-    return selected_coordinates
-
-
-# Allows to pass no value in prompts.
-# Usage: click.prompt()
-# See: https://stackoverflow.com/questions/68529664/prompt-for-an-optional-intrange-with-click-prompt
-class OptionalParamType(click.ParamType):
-    def __init__(self, param_type: click.ParamType):
-        self.param_type = param_type
-
-    def convert(self, value, param, ctx):
-        if not value:
-            return
-        return self.param_type.convert(value, param, ctx)
+import pathlib
+from pathlib import Path
+
+import click
+
+
+def add_options(options):
+    def _add_options(func):
+        for option in reversed(options):
+            func = option(func)
+        return func
+
+    return _add_options
+
+
+def add_file_or_path_argument(dir_okay=True, file_okay=True):
+    _file_or_path_argument = [
+        click.argument(
+            "input_path",
+            type=click.Path(
+                exists=True, resolve_path=True, path_type=pathlib.Path, dir_okay=dir_okay, file_okay=file_okay
+            ),
+        )
+    ]
+    return add_options(_file_or_path_argument)
+
+
+def add_file_argument():
+    return add_file_or_path_argument(dir_okay=False)
+
+
+def add_path_argument():
+    return add_file_or_path_argument(file_okay=False)
+
+
+def add_common_options():
+    _common_options = [
+        click.option(
+            "-out",
+            "--output-dir",
+            type=click.Path(path_type=pathlib.Path, file_okay=False, resolve_path=True),
+            default=None,
+            help="""
+            Specify the directory where output files are to be saved. If the directory doesn't exist, will be created.
+            If output_dir is not specified, files will be saved to the same folder.
+            """,
+        ),
+        click.option(
+            "--recalc-timestamp",
+            is_flag=True,
+            default=False,
+            help="""
+            Keep the original font 'modified' timestamp (head.modified) or set it to current time. By default,
+            original timestamp is kept.
+            """,
+        ),
+        click.option(
+            "--no-overwrite",
+            "overwrite",
+            is_flag=True,
+            default=True,
+            help="""
+            Overwrite existing files or save them to a new file (numbers are appended at the end of file name). By
+            default, files are overwritten.
+            """,
+        ),
+    ]
+    return add_options(_common_options)
+
+
+def file_overwrite_prompt(input_file: Path) -> bool:
+    return click.confirm(
+        f"{click.style(input_file, fg='yellow', bold=True)} already exists. "
+        f"Do you want to overwrite it?"
+    )
+
+
+def file_not_selected_message(file: Path):
+    click.secho(
+        f"[{click.style('SKIP', fg='yellow')}] {file.name} ({click.style('file is not selected', fg='yellow')})"
+    )
+
+
+def no_valid_fonts_message(input_path: Path):
+    if input_path.is_dir():
+        message = f"No valid font files matching the given criteria found in {input_path.name}"
+    else:
+        message = f"{input_path.name} is not a valid font file or doesn't match the given criteria"
+    click.secho(f"[{click.style('FAIL', fg='red')}] {message}")
+
+
+def file_not_exists_message(file: Path):
+    click.secho(
+        f"[{click.style('WARN', fg='bright_yellow')}] {file} {click.style('file does not exist', fg='bright_yellow')}"
+    )
+
+
+def file_not_changed_message(file: Path):
+    click.secho(
+        f"[{click.style('SKIP', fg='bright_yellow')}] {file} ({click.style('no changes made', fg='bright_yellow')})"
+    )
+
+
+def file_saved_message(file: Path):
+    click.secho(f"[{click.style('DONE', fg='green')}] {file} ({click.style('saved', fg='green')})")
+
+
+def generic_success_message(success_message):
+    click.secho(f"[{click.style('PASS', fg='green')}] {success_message}")
+
+
+def generic_info_message(info_message, nl=True):
+    click.secho(f"[{click.style('INFO', fg='cyan')}] {info_message}", nl=nl)
+
+
+def generic_error_message(error_message):
+    click.secho(f"[{click.style('FAIL', fg='red')}] {error_message}")
+
+
+def generic_warning_message(warning_message):
+    click.secho(f"[{click.style('WARN', fg='bright_yellow')}] {warning_message}")
+
+
+def select_instance_coordinates(axes: list) -> dict:
+    click.secho("\nSelect coordinates:")
+    selected_coordinates = {}
+    for a in axes:
+        axis_tag = a.axisTag
+        min_value = a.minValue
+        max_value = a.maxValue
+        coordinates = click.prompt(
+            f"{axis_tag} ({min_value} - {max_value})",
+            type=click.FloatRange(min_value, max_value),
+        )
+        selected_coordinates[axis_tag] = coordinates
+
+    return selected_coordinates
+
+
+# Allows to pass no value in prompts.
+# Usage: click.prompt()
+# See: https://stackoverflow.com/questions/68529664/prompt-for-an-optional-intrange-with-click-prompt
+class OptionalParamType(click.ParamType):
+    def __init__(self, param_type: click.ParamType):
+        self.param_type = param_type
+
+    def convert(self, value, param, ctx):
+        if not value:
+            return
+        return self.param_type.convert(value, param, ctx)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/otf_tools.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/otf_tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from fontTools.fontBuilder import FontBuilder
-from fontTools.pens.t2CharStringPen import T2CharStringPen
-from fontTools.ttLib.ttFont import TTFont
-
-from foundryToolsCLI.Lib.tables.CFF_ import TableCFF
-from foundryToolsCLI.Lib.utils.click_tools import generic_info_message
-from foundryToolsCLI.Lib.utils.skia_tools import (
-    remove_tiny_paths,
-    skia_path_from_glyph,
-    t2_charstring_from_skia_path,
-    same_path,
-    simplify_path,
-)
-
-
-def correct_otf_contours(font: TTFont, min_area: int = 25, verbose: bool = False) -> None:
-    try:
-        cff_table: TableCFF = font["CFF "]
-    except KeyError:
-        raise NotImplementedError("Not an OTF font")
-
-    glyph_set = font.getGlyphSet()
-
-    modified = set()
-    charstrings = {}
-
-    for k, v in glyph_set.items():
-        t2_pen = T2CharStringPen(width=v.width, glyphSet=glyph_set)
-        glyph_set[k].draw(t2_pen)
-        charstrings[k] = t2_pen.getCharString()
-
-        path_1 = skia_path_from_glyph(glyph_name=k, glyph_set=glyph_set)
-        path_2 = skia_path_from_glyph(glyph_name=k, glyph_set=glyph_set)
-        path_2 = simplify_path(path=path_2, glyph_name=k, clockwise=False)
-
-        if min_area > 0:
-            path_2 = remove_tiny_paths(path=path_2, glyph_name=k, min_area=min_area)
-
-        if not same_path(path_1=path_1, path_2=path_2):
-            modified.add(k)
-            charstrings[k] = t2_charstring_from_skia_path(path=path_2, width=v.width)
-
-    if verbose:
-        modified = sorted(list(modified))
-
-        if len(modified) > 0:
-            generic_info_message(f"The following glyphs have been modified: {', '.join(modified)}")
-        else:
-            generic_info_message("No glyphs modified")
-
-    ps_name = cff_table.get_fb_ps_name()
-    font_info = cff_table.get_fb_font_info()
-    private_dict = cff_table.get_fb_private_dict()
-    fb = FontBuilder(font=font)
-    fb.setupCFF(psName=ps_name, fontInfo=font_info, privateDict=private_dict, charStringsDict=charstrings)
+from fontTools.fontBuilder import FontBuilder
+from fontTools.pens.t2CharStringPen import T2CharStringPen
+from fontTools.ttLib.ttFont import TTFont
+
+from foundryToolsCLI.Lib.tables.CFF_ import TableCFF
+from foundryToolsCLI.Lib.utils.click_tools import generic_info_message
+from foundryToolsCLI.Lib.utils.skia_tools import (
+    remove_tiny_paths,
+    skia_path_from_glyph,
+    t2_charstring_from_skia_path,
+    same_path,
+    simplify_path,
+)
+
+
+def correct_otf_contours(font: TTFont, min_area: int = 25, verbose: bool = False) -> None:
+    try:
+        cff_table: TableCFF = font["CFF "]
+    except KeyError:
+        raise NotImplementedError("Not an OTF font")
+
+    glyph_set = font.getGlyphSet()
+
+    modified = set()
+    charstrings = {}
+
+    for k, v in glyph_set.items():
+        t2_pen = T2CharStringPen(width=v.width, glyphSet=glyph_set)
+        glyph_set[k].draw(t2_pen)
+        charstrings[k] = t2_pen.getCharString()
+
+        path_1 = skia_path_from_glyph(glyph_name=k, glyph_set=glyph_set)
+        path_2 = skia_path_from_glyph(glyph_name=k, glyph_set=glyph_set)
+        path_2 = simplify_path(path=path_2, glyph_name=k, clockwise=False)
+
+        if min_area > 0:
+            path_2 = remove_tiny_paths(path=path_2, glyph_name=k, min_area=min_area, verbose=verbose)
+
+        if not same_path(path_1=path_1, path_2=path_2):
+            modified.add(k)
+            charstrings[k] = t2_charstring_from_skia_path(path=path_2, width=v.width)
+
+    if verbose:
+        modified = sorted(list(modified))
+
+        if len(modified) > 0:
+            generic_info_message(f"The following glyphs have been modified: {', '.join(modified)}")
+        else:
+            generic_info_message("No glyphs modified")
+
+    ps_name = cff_table.get_fb_ps_name()
+    font_info = cff_table.get_fb_font_info()
+    private_dict = cff_table.get_fb_private_dict()
+    fb = FontBuilder(font=font)
+    fb.setupCFF(psName=ps_name, fontInfo=font_info, privateDict=private_dict, charStringsDict=charstrings)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/skia_tools.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/skia_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,164 +1,165 @@
-import itertools
-from collections.abc import Mapping, Callable
-
-import pathops
-from fontTools.misc.roundTools import otRound
-from fontTools.pens.t2CharStringPen import T2CharStringPen, T2CharString
-from fontTools.pens.ttGlyphPen import TTGlyphPen
-from fontTools.ttLib import ttFont
-from fontTools.ttLib.tables import _g_l_y_f
-
-from foundryToolsCLI.Lib.utils.click_tools import generic_info_message, generic_error_message
-
-_TTGlyphMapping = Mapping[str, ttFont._TTGlyph]
-
-
-def remove_tiny_paths(path: pathops.Path, glyph_name, min_area: int = 25):
-    """
-    Removes tiny paths from a pathops.Path.
-
-    :param path: the path from which to remove the tiny paths
-    :param glyph_name: the glyph name
-    :param min_area: the minimum are of a path
-    :return: the cleaned path
-    """
-    cleaned_path = pathops.Path()
-    for contour in path.contours:
-        if contour.area >= min_area:
-            cleaned_path.addPath(contour)
-        else:
-            generic_info_message(f"tiny path removed from glyph {glyph_name}")
-    return cleaned_path
-
-
-def skia_path_from_glyph(glyph_name: str, glyph_set: _TTGlyphMapping) -> pathops.Path:
-    """
-    Returns a pathops.Path from a glyph
-
-    :param glyph_name: the glyph name
-    :param glyph_set: the glyphSet to which the glyph belongs
-    :return: a pathops.Path object
-    """
-    path = pathops.Path()
-    pen = path.getPen(glyphSet=glyph_set)
-    glyph_set[glyph_name].draw(pen)
-    return path
-
-
-def skia_path_from_component(component: _g_l_y_f.GlyphComponent, glyph_set: _TTGlyphMapping):
-    base_glyph_name, transformation = component.getComponentInfo()
-    path = skia_path_from_glyph(glyph_name=base_glyph_name, glyph_set=glyph_set)
-    return path.transform(*transformation)
-
-
-def ttf_glyph_from_skia_path(path: pathops.Path) -> _g_l_y_f.Glyph:
-    tt_pen = TTGlyphPen(glyphSet=None)
-    path.draw(tt_pen)
-    glyph = tt_pen.glyph()
-    glyph.recalcBounds(glyfTable=None)
-    return glyph
-
-
-def t2_charstring_from_skia_path(path: pathops.Path, width: int) -> T2CharString:
-    t2_pen = T2CharStringPen(width, glyphSet=None)
-    path.draw(t2_pen)
-    charstring = t2_pen.getCharString()
-    return charstring
-
-
-def round_path(path: pathops.Path, rounder: Callable[[float], float] = otRound) -> pathops.Path:
-    """
-    Rounds the points coordinate of a pathops.Path
-
-    :param path: the path to round
-    :param rounder: the function to call
-    :return: the path with rounded points
-    """
-    rounded_path = pathops.Path()
-    for verb, points in path:
-        rounded_path.add(verb, *((rounder(p[0]), rounder(p[1])) for p in points))
-    return rounded_path
-
-
-def simplify_path(path: pathops.Path, glyph_name: str, clockwise: bool) -> pathops.Path:
-    """
-    Simplify a pathops.Path by removing overlaps, fixing contours direction and, optionally, removing tiny paths
-
-    :param path: the pathops.Path to simplify
-    :param glyph_name: the glyph name
-    :param clockwise: must be True for TTF fonts, False for OTF fonts
-    :return: the simplified path
-    """
-
-    # skia-pathops has a bug where it sometimes fails to simplify paths when there
-    # are float coordinates and control points are very close to one another.
-    # Rounding coordinates to integers works around the bug.
-    # Since we are going to round glyf coordinates later on anyway, here it is
-    # ok(-ish) to also round before simplify. Better than failing the whole process
-    # for the entire font.
-    # https://bugs.chromium.org/p/skia/issues/detail?id=11958
-    # https://github.com/google/fonts/issues/3365
-
-    try:
-        return pathops.simplify(path, fix_winding=True, clockwise=clockwise)
-    except pathops.PathOpsError:
-        pass
-
-    path = round_path(path)
-    try:
-        path = pathops.simplify(path, fix_winding=True, clockwise=clockwise)
-        generic_info_message(
-            f"skia-pathops failed to simplify glyph '{glyph_name}' with float coordinates, but succeeded using rounded "
-            f"integer coordinates"
-        )
-        return path
-    except pathops.PathOpsError as e:
-        generic_error_message(f"skia-pathops failed to simplify glyph '{glyph_name}': {e}")
-
-    raise AssertionError("Unreachable")
-
-
-def same_path(path_1: pathops.Path, path_2: pathops.Path) -> bool:
-    """
-    Checks if two pathops paths are the same
-
-    :param path_1: the first path
-    :param path_2: the second path
-    :return: True if the paths are the same, False if the paths are different
-    """
-    if {tuple(c) for c in path_1.contours} != {tuple(c) for c in path_2.contours}:
-        return False
-    else:
-        return True
-
-
-def ttf_components_overlap(glyph: _g_l_y_f.Glyph, glyph_set: _TTGlyphMapping) -> bool:
-    if not glyph.isComposite():
-        raise ValueError("This method only works with TrueType composite glyphs")
-    if len(glyph.components) < 2:
-        return False
-
-    component_paths = {}
-
-    def _get_nth_component_path(index: int) -> pathops.Path:
-        if index not in component_paths:
-            component_paths[index] = skia_path_from_glyph_component(glyph.components[index], glyph_set)
-        return component_paths[index]
-
-    return any(
-        pathops.op(
-            _get_nth_component_path(i),
-            _get_nth_component_path(j),
-            pathops.PathOp.INTERSECTION,
-            fix_winding=True,
-            keep_starting_points=False,
-            clockwise=True,
-        )
-        for i, j in itertools.combinations(range(len(glyph.components)), 2)
-    )
-
-
-def skia_path_from_glyph_component(component: _g_l_y_f.GlyphComponent, glyph_set: _TTGlyphMapping):
-    base_glyph_name, transformation = component.getComponentInfo()
-    path = skia_path_from_glyph(base_glyph_name, glyph_set)
-    return path.transform(*transformation)
+import itertools
+from collections.abc import Mapping, Callable
+
+import pathops
+from fontTools.misc.roundTools import otRound
+from fontTools.pens.t2CharStringPen import T2CharStringPen, T2CharString
+from fontTools.pens.ttGlyphPen import TTGlyphPen
+from fontTools.ttLib import ttFont
+from fontTools.ttLib.tables import _g_l_y_f
+
+from foundryToolsCLI.Lib.utils.click_tools import generic_info_message, generic_error_message
+
+_TTGlyphMapping = Mapping[str, ttFont._TTGlyph]
+
+
+def remove_tiny_paths(path: pathops.Path, glyph_name, min_area: int = 25, verbose: bool = True):
+    """
+    Removes tiny paths from a pathops.Path.
+
+    :param path: the path from which to remove the tiny paths
+    :param glyph_name: the glyph name
+    :param min_area: the minimum are of a path
+    :return: the cleaned path
+    """
+    cleaned_path = pathops.Path()
+    for contour in path.contours:
+        if contour.area >= min_area:
+            cleaned_path.addPath(contour)
+        else:
+            if verbose:
+                generic_info_message(f"tiny path removed from glyph {glyph_name}")
+    return cleaned_path
+
+
+def skia_path_from_glyph(glyph_name: str, glyph_set: _TTGlyphMapping) -> pathops.Path:
+    """
+    Returns a pathops.Path from a glyph
+
+    :param glyph_name: the glyph name
+    :param glyph_set: the glyphSet to which the glyph belongs
+    :return: a pathops.Path object
+    """
+    path = pathops.Path()
+    pen = path.getPen(glyphSet=glyph_set)
+    glyph_set[glyph_name].draw(pen)
+    return path
+
+
+def skia_path_from_component(component: _g_l_y_f.GlyphComponent, glyph_set: _TTGlyphMapping):
+    base_glyph_name, transformation = component.getComponentInfo()
+    path = skia_path_from_glyph(glyph_name=base_glyph_name, glyph_set=glyph_set)
+    return path.transform(*transformation)
+
+
+def ttf_glyph_from_skia_path(path: pathops.Path) -> _g_l_y_f.Glyph:
+    tt_pen = TTGlyphPen(glyphSet=None)
+    path.draw(tt_pen)
+    glyph = tt_pen.glyph()
+    glyph.recalcBounds(glyfTable=None)
+    return glyph
+
+
+def t2_charstring_from_skia_path(path: pathops.Path, width: int) -> T2CharString:
+    t2_pen = T2CharStringPen(width, glyphSet=None)
+    path.draw(t2_pen)
+    charstring = t2_pen.getCharString()
+    return charstring
+
+
+def round_path(path: pathops.Path, rounder: Callable[[float], float] = otRound) -> pathops.Path:
+    """
+    Rounds the points coordinate of a pathops.Path
+
+    :param path: the path to round
+    :param rounder: the function to call
+    :return: the path with rounded points
+    """
+    rounded_path = pathops.Path()
+    for verb, points in path:
+        rounded_path.add(verb, *((rounder(p[0]), rounder(p[1])) for p in points))
+    return rounded_path
+
+
+def simplify_path(path: pathops.Path, glyph_name: str, clockwise: bool) -> pathops.Path:
+    """
+    Simplify a pathops.Path by removing overlaps, fixing contours direction and, optionally, removing tiny paths
+
+    :param path: the pathops.Path to simplify
+    :param glyph_name: the glyph name
+    :param clockwise: must be True for TTF fonts, False for OTF fonts
+    :return: the simplified path
+    """
+
+    # skia-pathops has a bug where it sometimes fails to simplify paths when there
+    # are float coordinates and control points are very close to one another.
+    # Rounding coordinates to integers works around the bug.
+    # Since we are going to round glyf coordinates later on anyway, here it is
+    # ok(-ish) to also round before simplify. Better than failing the whole process
+    # for the entire font.
+    # https://bugs.chromium.org/p/skia/issues/detail?id=11958
+    # https://github.com/google/fonts/issues/3365
+
+    try:
+        return pathops.simplify(path, fix_winding=True, clockwise=clockwise)
+    except pathops.PathOpsError:
+        pass
+
+    path = round_path(path)
+    try:
+        path = pathops.simplify(path, fix_winding=True, clockwise=clockwise)
+        generic_info_message(
+            f"skia-pathops failed to simplify glyph '{glyph_name}' with float coordinates, but succeeded using rounded "
+            f"integer coordinates"
+        )
+        return path
+    except pathops.PathOpsError as e:
+        generic_error_message(f"skia-pathops failed to simplify glyph '{glyph_name}': {e}")
+
+    raise AssertionError("Unreachable")
+
+
+def same_path(path_1: pathops.Path, path_2: pathops.Path) -> bool:
+    """
+    Checks if two pathops paths are the same
+
+    :param path_1: the first path
+    :param path_2: the second path
+    :return: True if the paths are the same, False if the paths are different
+    """
+    if {tuple(c) for c in path_1.contours} != {tuple(c) for c in path_2.contours}:
+        return False
+    else:
+        return True
+
+
+def ttf_components_overlap(glyph: _g_l_y_f.Glyph, glyph_set: _TTGlyphMapping) -> bool:
+    if not glyph.isComposite():
+        raise ValueError("This method only works with TrueType composite glyphs")
+    if len(glyph.components) < 2:
+        return False
+
+    component_paths = {}
+
+    def _get_nth_component_path(index: int) -> pathops.Path:
+        if index not in component_paths:
+            component_paths[index] = skia_path_from_glyph_component(glyph.components[index], glyph_set)
+        return component_paths[index]
+
+    return any(
+        pathops.op(
+            _get_nth_component_path(i),
+            _get_nth_component_path(j),
+            pathops.PathOp.INTERSECTION,
+            fix_winding=True,
+            keep_starting_points=False,
+            clockwise=True,
+        )
+        for i, j in itertools.combinations(range(len(glyph.components)), 2)
+    )
+
+
+def skia_path_from_glyph_component(component: _g_l_y_f.GlyphComponent, glyph_set: _TTGlyphMapping):
+    base_glyph_name, transformation = component.getComponentInfo()
+    path = skia_path_from_glyph(base_glyph_name, glyph_set)
+    return path.transform(*transformation)
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/text_tools.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/text_tools.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from textwrap import TextWrapper
-
-
-def wrap_string(string: str, width: int, initial_indent: int, indent: int, max_lines: int = None) -> str:
-    """
-    It wraps a string to a given width, with a given indentation
-
-    :param string: The string to wrap
-    :type string: str
-    :param width: The maximum width of the wrapped lines
-    :type width: int
-    :param initial_indent: The number of spaces to add to the beginning of each line
-    :type initial_indent: int
-    :param indent: The number of spaces to add to the left margin of subsequent lines
-    :type indent: int
-    :param max_lines: The maximum number of lines to return. If the string is longer than this, it will be truncated
-    :type max_lines: int
-    :return: A string that has been wrapped to the specified width.
-    """
-    wrapped_string = TextWrapper(
-        width=width,
-        initial_indent=" " * initial_indent,
-        subsequent_indent=" " * indent,
-        max_lines=max_lines,
-        break_on_hyphens=False,
-        break_long_words=True,
-    ).fill(string)
-    return wrapped_string
+from textwrap import TextWrapper
+
+
+def wrap_string(string: str, width: int, initial_indent: int, indent: int, max_lines: int = None) -> str:
+    """
+    It wraps a string to a given width, with a given indentation
+
+    :param string: The string to wrap
+    :type string: str
+    :param width: The maximum width of the wrapped lines
+    :type width: int
+    :param initial_indent: The number of spaces to add to the beginning of each line
+    :type initial_indent: int
+    :param indent: The number of spaces to add to the left margin of subsequent lines
+    :type indent: int
+    :param max_lines: The maximum number of lines to return. If the string is longer than this, it will be truncated
+    :type max_lines: int
+    :return: A string that has been wrapped to the specified width.
+    """
+    wrapped_string = TextWrapper(
+        width=width,
+        initial_indent=" " * initial_indent,
+        subsequent_indent=" " * indent,
+        max_lines=max_lines,
+        break_on_hyphens=False,
+        break_long_words=True,
+    ).fill(string)
+    return wrapped_string
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/Lib/utils/ttf_tools.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/ttf_tools.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-"""
-Adapted code from fontTools.ttLib.removeOverlaps to fix contours direction
-"""
-
-from typing import Mapping
-
-from fontTools.ttLib import ttFont
-from fontTools.ttLib.tables import _g_l_y_f
-from fontTools.ttLib.tables import _h_m_t_x
-
-from foundryToolsCLI.Lib.utils.click_tools import generic_error_message, generic_info_message
-from foundryToolsCLI.Lib.utils.skia_tools import (
-    remove_tiny_paths,
-    skia_path_from_glyph,
-    ttf_glyph_from_skia_path,
-    simplify_path,
-    ttf_components_overlap,
-    same_path,
-)
-
-
-class CorrectTTFContoursError(Exception):
-    pass
-
-
-_TTGlyphMapping = Mapping[str, ttFont._TTGlyph]
-
-
-def correct_glyph_contours(
-    glyph_name: str,
-    glyph_set: _TTGlyphMapping,
-    glyf_table: _g_l_y_f.table__g_l_y_f,
-    hmtx_table: _h_m_t_x.table__h_m_t_x,
-    remove_hinting: bool = True,
-    min_area: int = 25,
-) -> bool:
-    glyph = glyf_table[glyph_name]
-
-    if glyph.numberOfContours > 0 or glyph.isComposite() and ttf_components_overlap(glyph, glyph_set):
-        path_1 = skia_path_from_glyph(glyph_name, glyph_set)
-        path_2 = skia_path_from_glyph(glyph_name, glyph_set)
-        path_2 = simplify_path(path_2, glyph_name, clockwise=True)
-        if min_area > 0:
-            path_2 = remove_tiny_paths(path_2, glyph_name=glyph_name, min_area=min_area)
-
-        if not same_path(path_1=path_1, path_2=path_2):
-            glyf_table[glyph_name] = glyph = ttf_glyph_from_skia_path(path_2)
-            assert not glyph.program
-            width, lsb = hmtx_table[glyph_name]
-            if lsb != glyph.xMin:
-                hmtx_table[glyph_name] = (width, glyph.xMin)
-            return True
-
-    if remove_hinting:
-        glyph.removeHinting()
-    return False
-
-
-def correct_ttf_contours(
-    font: ttFont.TTFont,
-    remove_hinting: bool = True,
-    ignore_errors: bool = False,
-    min_area: int = 25,
-    verbose: bool = False,
-) -> None:
-    try:
-        glyf_table = font["glyf"]
-    except KeyError:
-        raise NotImplementedError("Not a TTF font")
-
-    glyph_set = font.getGlyphSet()
-    hmtx_table = font["hmtx"]
-
-    glyph_names = font.getGlyphOrder()
-
-    # process all simple glyphs first, then composites with increasing component depth,
-    # so that by the time we test for component intersections the respective base glyphs
-    # have already been simplified
-    glyph_names = sorted(
-        glyph_names,
-        key=lambda name: (
-            glyf_table[name].getCompositeMaxpValues(glyf_table).maxComponentDepth
-            if glyf_table[name].isComposite()
-            else 0,
-            name,
-        ),
-    )
-    modified = set()
-    for glyph_name in glyph_names:
-        try:
-            if correct_glyph_contours(
-                glyph_name=glyph_name,
-                glyph_set=glyph_set,
-                glyf_table=glyf_table,
-                hmtx_table=hmtx_table,
-                remove_hinting=remove_hinting,
-                min_area=min_area,
-            ):
-                modified.add(glyph_name)
-        except CorrectTTFContoursError:
-            if not ignore_errors:
-                raise
-            generic_error_message(f"Failed to remove overlaps for '{glyph_name}'")
-
-    if verbose:
-        modified = sorted(list(modified))
-        generic_info_message(f"{len(modified)} glyphs modified: {', '.join(modified)}")
-
-
-def decomponentize(font: ttFont.TTFont):
-    """
-    This function decomponentizes composite glyphs in a TrueType font.
-    """
-    from fontTools.pens.recordingPen import DecomposingRecordingPen
-    from fontTools.pens.ttGlyphPen import TTGlyphPen
-
-    glyph_set = font.getGlyphSet()
-    glyf_table = font["glyf"]
-    dr_pen = DecomposingRecordingPen(glyph_set)
-    tt_pen = TTGlyphPen(None)
-
-    for glyph_name in font.glyphOrder:
-        glyph = glyf_table[glyph_name]
-        if not glyph.isComposite():
-            continue
-        dr_pen.value = []
-        tt_pen.init()
-        glyph.draw(dr_pen, glyf_table)
-        dr_pen.replay(tt_pen)
-        glyf_table[glyph_name] = tt_pen.glyph()
+"""
+Adapted code from fontTools.ttLib.removeOverlaps to fix contours direction
+"""
+
+from typing import Mapping
+
+from fontTools.ttLib import ttFont
+from fontTools.ttLib.tables import _g_l_y_f
+from fontTools.ttLib.tables import _h_m_t_x
+
+from foundryToolsCLI.Lib.utils.click_tools import generic_error_message, generic_info_message
+from foundryToolsCLI.Lib.utils.skia_tools import (
+    remove_tiny_paths,
+    skia_path_from_glyph,
+    ttf_glyph_from_skia_path,
+    simplify_path,
+    ttf_components_overlap,
+    same_path,
+)
+
+
+class CorrectTTFContoursError(Exception):
+    pass
+
+
+_TTGlyphMapping = Mapping[str, ttFont._TTGlyph]
+
+
+def correct_glyph_contours(
+    glyph_name: str,
+    glyph_set: _TTGlyphMapping,
+    glyf_table: _g_l_y_f.table__g_l_y_f,
+    hmtx_table: _h_m_t_x.table__h_m_t_x,
+    remove_hinting: bool = True,
+    min_area: int = 25,
+) -> bool:
+    glyph = glyf_table[glyph_name]
+
+    if glyph.numberOfContours > 0 or glyph.isComposite() and ttf_components_overlap(glyph, glyph_set):
+        path_1 = skia_path_from_glyph(glyph_name, glyph_set)
+        path_2 = skia_path_from_glyph(glyph_name, glyph_set)
+        path_2 = simplify_path(path_2, glyph_name, clockwise=True)
+        if min_area > 0:
+            path_2 = remove_tiny_paths(path_2, glyph_name=glyph_name, min_area=min_area)
+
+        if not same_path(path_1=path_1, path_2=path_2):
+            glyf_table[glyph_name] = glyph = ttf_glyph_from_skia_path(path_2)
+            assert not glyph.program
+            width, lsb = hmtx_table[glyph_name]
+            if lsb != glyph.xMin:
+                hmtx_table[glyph_name] = (width, glyph.xMin)
+            return True
+
+    if remove_hinting:
+        glyph.removeHinting()
+    return False
+
+
+def correct_ttf_contours(
+    font: ttFont.TTFont,
+    remove_hinting: bool = True,
+    ignore_errors: bool = False,
+    min_area: int = 25,
+    verbose: bool = False,
+) -> None:
+    try:
+        glyf_table = font["glyf"]
+    except KeyError:
+        raise NotImplementedError("Not a TTF font")
+
+    glyph_set = font.getGlyphSet()
+    hmtx_table = font["hmtx"]
+
+    glyph_names = font.getGlyphOrder()
+
+    # process all simple glyphs first, then composites with increasing component depth,
+    # so that by the time we test for component intersections the respective base glyphs
+    # have already been simplified
+    glyph_names = sorted(
+        glyph_names,
+        key=lambda name: (
+            glyf_table[name].getCompositeMaxpValues(glyf_table).maxComponentDepth
+            if glyf_table[name].isComposite()
+            else 0,
+            name,
+        ),
+    )
+    modified = set()
+    for glyph_name in glyph_names:
+        try:
+            if correct_glyph_contours(
+                glyph_name=glyph_name,
+                glyph_set=glyph_set,
+                glyf_table=glyf_table,
+                hmtx_table=hmtx_table,
+                remove_hinting=remove_hinting,
+                min_area=min_area,
+            ):
+                modified.add(glyph_name)
+        except CorrectTTFContoursError:
+            if not ignore_errors:
+                raise
+            generic_error_message(f"Failed to remove overlaps for '{glyph_name}'")
+
+    if verbose:
+        modified = sorted(list(modified))
+        generic_info_message(f"{len(modified)} glyphs modified: {', '.join(modified)}")
+
+
+def decomponentize(font: ttFont.TTFont):
+    """
+    This function decomponentizes composite glyphs in a TrueType font.
+    """
+    from fontTools.pens.recordingPen import DecomposingRecordingPen
+    from fontTools.pens.ttGlyphPen import TTGlyphPen
+
+    glyph_set = font.getGlyphSet()
+    glyf_table = font["glyf"]
+    dr_pen = DecomposingRecordingPen(glyph_set)
+    tt_pen = TTGlyphPen(None)
+
+    for glyph_name in font.glyphOrder:
+        glyph = glyf_table[glyph_name]
+        if not glyph.isComposite():
+            continue
+        dr_pen.value = []
+        tt_pen.init()
+        glyph.draw(dr_pen, glyf_table)
+        dr_pen.replay(tt_pen)
+        glyf_table[glyph_name] = tt_pen.glyph()
```

### Comparing `foundrytools-cli-1.0.0/foundryToolsCLI/__main__.py` & `foundrytools-cli-1.0.1/foundryToolsCLI/__main__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import sys
-from pathlib import Path
-
-import click
-
-this_directory = Path(__file__).parent
-plugin_folder = this_directory.joinpath("CLI")
-
-
-class FoundryToolsCLI(click.MultiCommand):
-    def list_commands(self, ctx):
-        rv = []
-        for file in plugin_folder.iterdir():
-            if file.name.endswith(".py") and file.name.startswith("ftcli_"):
-                rv.append(file.name[6:-3])
-        rv.sort()
-        return rv
-
-    def get_command(self, ctx, cmd_name):
-        try:
-            mod = __import__(f"foundryToolsCLI.CLI.ftcli_{cmd_name}", None, None, ["cli"])
-        except ImportError as e:
-            click.secho(f"{click.style('ERROR', fg='red')}: {e}")
-            return
-
-        return mod.cli
-
-
-main = FoundryToolsCLI(help="FoundryTools Command Line Interface.")
-
-
-if __name__ == "__main__":
-    sys.exit(main())
+import sys
+from pathlib import Path
+
+import click
+
+this_directory = Path(__file__).parent
+plugin_folder = this_directory.joinpath("CLI")
+
+
+class FoundryToolsCLI(click.MultiCommand):
+    def list_commands(self, ctx):
+        rv = []
+        for file in plugin_folder.iterdir():
+            if file.name.endswith(".py") and file.name.startswith("ftcli_"):
+                rv.append(file.name[6:-3])
+        rv.sort()
+        return rv
+
+    def get_command(self, ctx, cmd_name):
+        try:
+            mod = __import__(f"foundryToolsCLI.CLI.ftcli_{cmd_name}", None, None, ["cli"])
+        except ImportError as e:
+            click.secho(f"{click.style('ERROR', fg='red')}: {e}")
+            return
+
+        return mod.cli
+
+
+main = FoundryToolsCLI(help="FoundryTools Command Line Interface.")
+
+
+if __name__ == "__main__":
+    sys.exit(main())
```

### Comparing `foundrytools-cli-1.0.0/foundrytools_cli.egg-info/PKG-INFO` & `foundrytools-cli-1.0.1/foundrytools_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,78 @@
-Metadata-Version: 2.1
-Name: foundrytools-cli
-Version: 1.0.0
-Summary: A set of command line tools to inspect, manipulate and convert font files
-Home-page: https://github.com/ftCLI/FoundryTools-CLI
-Author: ftCLI
-Author-email: ftcli@proton.me
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# FoundryTools-CLI
-FoundryTools-CLI, former known as ftCLI, is a collection of command line tools written in Python to inspect, manipulate
-and convert fonts. It takes advantage of the capabilities made available by other tools such as:
-
-* [FontTools](https://github.com/fonttools/fonttools)
-* [AFDKO](https://github.com/adobe-type-tools/afdko)
-* [skia-pathops](https://github.com/fonttools/skia-pathops)
-* [cffsubr](https://github.com/adobe-type-tools/cffsubr)
-* [psautohint](https://github.com/adobe-type-tools/psautohint)
-* [ttfautohint-py](https://github.com/fonttools/ttfautohint-py)
-* [dehinter](https://github.com/source-foundry/dehinter)
-* [beziers](https://github.com/simoncozens/beziers.py)
-
-The command line interface is built with [click](https://github.com/pallets/click/) and tables are rendered by
-[rich](https://github.com/Textualize/rich).
-
-Even if not directly imported to keep the footprint as small as possible, portions of code have been copied from
-[fontbakery](https://github.com/googlefonts/fontbakery).
-
-## Installation
-FoundryTools-CLI requires Python 3.9 or later.
-
-**Note for Windows users**: installation on Python 3.11 is strongly discouraged because AFDKO 3.9.6 doesn't support
-it, and an attempt of installation would probably fail. Since macOS users successfully installed FoundryTools-CLI on
-Python 3.11, requirements have been loosened up.
-
-### pip
-FoundryTools-CLI releases are available on the Python Package Index (PyPI), so it can be installed with
-[pip](https://pip.pypa.io/):
-
-    python -m pip install foundrytools-cli
-
-### Editable mode
-If you would like to contribute to the development, you can clone the repository from GitHub, install the package in
-'editable' mode and modify the source code in place. We strongly recommend using a virtual environment.
-
-    # clone the repository:
-    git clone https://github.com/ftCLI/foundrytools-cli.git
-    cd foundrytools-cli
-
-    # create new virtual environment named e.g. ftcli-venv, or whatever you prefer:
-    python -m venv ftcli-venv
-    
-    # to activate the virtual environmtnet in macOS and Linux, do:
-    . ftcli-venv/bin/activate
-    
-    # to activate the virtual environment in Windows, do:
-    ftcli-venv\Scripts\activate.bat
-    
-    # install in 'editable' mode
-    python -m pip install -e .
-
-## Documentation
-FoundryTools-CLI is a Terminal app where commands are logically organized into subcommands.
-
-Please refer to the [user documentation](https://ft-cli.github.io).
-
-## License
-FoundryTools-CLI is available under the [MIT license](LICENSE)
-
-
-
+Metadata-Version: 2.1
+Name: foundrytools-cli
+Version: 1.0.1
+Summary: A set of command line tools to inspect, manipulate and convert font files
+Home-page: https://github.com/ftCLI/FoundryTools-CLI
+Author: ftCLI
+Author-email: ftcli@proton.me
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# FoundryTools-CLI
+FoundryTools-CLI, former known as ftCLI, is a collection of command line tools written in Python to inspect, manipulate
+and convert fonts. It takes advantage of the capabilities made available by other tools such as:
+
+* [FontTools](https://github.com/fonttools/fonttools)
+* [AFDKO](https://github.com/adobe-type-tools/afdko)
+* [skia-pathops](https://github.com/fonttools/skia-pathops)
+* [cffsubr](https://github.com/adobe-type-tools/cffsubr)
+* [psautohint](https://github.com/adobe-type-tools/psautohint)
+* [ttfautohint-py](https://github.com/fonttools/ttfautohint-py)
+* [dehinter](https://github.com/source-foundry/dehinter)
+* [beziers](https://github.com/simoncozens/beziers.py)
+
+The command line interface is built with [click](https://github.com/pallets/click/) and tables are rendered by
+[rich](https://github.com/Textualize/rich).
+
+Even if not directly imported to keep the footprint as small as possible, portions of code have been copied from
+[fontbakery](https://github.com/googlefonts/fontbakery).
+
+## Installation
+FoundryTools-CLI requires Python 3.9 or later.
+
+**Note for Windows users**: installation on Python 3.11 is strongly discouraged because AFDKO 3.9.6 doesn't support
+it, and an attempt of installation would probably fail. Since macOS users successfully installed FoundryTools-CLI on
+Python 3.11, requirements have been loosened up.
+
+### pip
+FoundryTools-CLI releases are available on the Python Package Index (PyPI), so it can be installed with
+[pip](https://pip.pypa.io/):
+
+    python -m pip install foundrytools-cli
+
+### Editable mode
+If you would like to contribute to the development, you can clone the repository from GitHub, install the package in
+'editable' mode and modify the source code in place. We strongly recommend using a virtual environment.
+
+    # clone the repository:
+    git clone https://github.com/ftCLI/foundrytools-cli.git
+    cd foundrytools-cli
+
+    # create new virtual environment named e.g. ftcli-venv, or whatever you prefer:
+    python -m venv ftcli-venv
+    
+    # to activate the virtual environmtnet in macOS and Linux, do:
+    . ftcli-venv/bin/activate
+    
+    # to activate the virtual environment in Windows, do:
+    ftcli-venv\Scripts\activate.bat
+    
+    # install in 'editable' mode
+    python -m pip install -e .
+
+## Documentation
+FoundryTools-CLI is a Terminal app where commands are logically organized into subcommands.
+
+Please refer to the [user documentation](https://ftcli.github.io/FoundryTools-CLI/).
+
+## License
+FoundryTools-CLI is available under the [MIT license](LICENSE)
+
+## Credits
+To Sergiev. May You rest in peace.
+
+
+
```

### Comparing `foundrytools-cli-1.0.0/foundrytools_cli.egg-info/SOURCES.txt` & `foundrytools-cli-1.0.1/foundrytools_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 foundryToolsCLI/__init__.py
 foundryToolsCLI/__main__.py
 foundryToolsCLI/CLI/__init__.py
-foundryToolsCLI/CLI/_ftcli_tb.py
 foundryToolsCLI/CLI/ftcli_assistant.py
 foundryToolsCLI/CLI/ftcli_cff.py
 foundryToolsCLI/CLI/ftcli_converter.py
 foundryToolsCLI/CLI/ftcli_fix.py
 foundryToolsCLI/CLI/ftcli_hhea.py
 foundryToolsCLI/CLI/ftcli_metrics.py
 foundryToolsCLI/CLI/ftcli_name.py
```

### Comparing `foundrytools-cli-1.0.0/setup.py` & `foundrytools-cli-1.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import setuptools
-
-from pathlib import Path
-
-this_directory = Path(__file__).parent
-long_description = this_directory.joinpath("README.md").read_text()
-
-setuptools.setup(
-    name="foundrytools-cli",
-    version="1.0.0",
-    description="A set of command line tools to inspect, manipulate and convert font files",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    author="ftCLI",
-    author_email="ftcli@proton.me",
-    url="https://github.com/ftCLI/FoundryTools-CLI",
-    packages=setuptools.find_packages(),
-    include_package_data=True,
-    entry_points={"console_scripts": ["ftcli = foundryToolsCLI.__main__:main"]},
-    install_requires=[
-        "afdko>=3.9.6",
-        "fonttools>=4.41.1",
-        "beziers>=0.5.0",
-        "brotli>=1.0.9",
-        "click>=8.1.6",
-        "cffsubr>=0.2.9.post1",
-        "dehinter>=4.0.0",
-        "pathvalidate>=3.1.0",
-        "psautohint>=2.4.0",
-        "rich>=13.4.2",
-        "skia-pathops>=0.7.4",
-        "ttfautohint-py>=0.5.1",
-        "zopfli>=0.2.2",
-    ],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent",
-    ],
-    python_requires=">=3.9",
-    zip_safe=False,
-)
+import setuptools
+
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = this_directory.joinpath("README.md").read_text()
+
+setuptools.setup(
+    name="foundrytools-cli",
+    version="1.0.1",
+    description="A set of command line tools to inspect, manipulate and convert font files",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author="ftCLI",
+    author_email="ftcli@proton.me",
+    url="https://github.com/ftCLI/FoundryTools-CLI",
+    packages=setuptools.find_packages(),
+    include_package_data=True,
+    entry_points={"console_scripts": ["ftcli = foundryToolsCLI.__main__:main"]},
+    install_requires=[
+        "afdko>=3.9.6",
+        "fonttools>=4.42.0",
+        "beziers>=0.5.0",
+        "brotli>=1.0.9",
+        "click>=8.1.6",
+        "cffsubr>=0.2.9.post1",
+        "dehinter>=4.0.0",
+        "pathvalidate>=3.1.0",
+        "psautohint>=2.4.0",
+        "rich>=13.5.2",
+        "skia-pathops>=0.7.4",
+        "ttfautohint-py>=0.5.1",
+        "zopfli>=0.2.2",
+    ],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Operating System :: OS Independent",
+    ],
+    python_requires=">=3.9",
+    zip_safe=False,
+)
```

