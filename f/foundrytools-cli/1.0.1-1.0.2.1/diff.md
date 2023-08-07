# Comparing `tmp/foundrytools-cli-1.0.1.tar.gz` & `tmp/foundrytools-cli-1.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundrytools-cli-1.0.1.tar", last modified: Mon Aug  7 06:14:50 2023, max compression
+gzip compressed data, was "foundrytools-cli-1.0.2.1.tar", last modified: Mon Aug  7 15:16:53 2023, max compression
```

## Comparing `foundrytools-cli-1.0.1.tar` & `foundrytools-cli-1.0.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.464173 foundrytools-cli-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-07 06:14:50.464173 foundrytools-cli-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.452173 foundrytools-cli-1.0.1/foundryToolsCLI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.456173 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_cff.py
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20917 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_hhea.py
--rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    18933 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_os2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15894 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_otf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_print.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_ttf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.456173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/
--rw-r--r--   0 runner    (1001) docker     (123)    35586 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/Font.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/VFont.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.456173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)    21938 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/UI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27371 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/fonts_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/styles_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.460173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/otf_to_ttf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/sfnt_to_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/ttc_to_sfnt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/ttf_to_otf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/variable_to_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/web_to_sfnt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.460173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/printer/
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/printer/UI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/printer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.460173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/CFF_.py
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/OS_2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/head.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/hhea.py
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.464173 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/bits_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/cli_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/click_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/otf_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/skia_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/text_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/ttf_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/foundryToolsCLI/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:14:50.464173 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 06:14:50.000000 foundrytools-cli-1.0.1/foundrytools_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 06:14:50.464173 foundrytools-cli-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-07 06:14:34.000000 foundrytools-cli-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:53.230246 foundrytools-cli-1.0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-07 15:16:53.230246 foundrytools-cli-1.0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:53.214246 foundrytools-cli-1.0.2.1/foundryToolsCLI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:53.218246 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_cff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20917 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_hhea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18933 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_os2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15894 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_otf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_ttf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:53.218246 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    35586 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/Font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/VFont.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:53.218246 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    21938 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/assistant/UI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27371 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/assistant/fonts_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/assistant/styles_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:53.222246 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/otf_to_ttf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/sfnt_to_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/ttc_to_sfnt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/ttf_to_otf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/variable_to_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/web_to_sfnt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:53.222246 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/printer/UI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:53.226246 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/CFF_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/OS_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/hhea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:53.226246 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/bits_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/cli_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/click_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/otf_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/skia_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/text_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/ttf_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/foundryToolsCLI/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:16:53.230246 foundrytools-cli-1.0.2.1/foundrytools_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-07 15:16:53.000000 foundrytools-cli-1.0.2.1/foundrytools_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-07 15:16:53.000000 foundrytools-cli-1.0.2.1/foundrytools_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:16:53.000000 foundrytools-cli-1.0.2.1/foundrytools_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-07 15:16:53.000000 foundrytools-cli-1.0.2.1/foundrytools_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:16:53.000000 foundrytools-cli-1.0.2.1/foundrytools_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 15:16:53.000000 foundrytools-cli-1.0.2.1/foundrytools_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 15:16:53.000000 foundrytools-cli-1.0.2.1/foundrytools_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:16:53.230246 foundrytools-cli-1.0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-07 15:16:43.000000 foundrytools-cli-1.0.2.1/setup.py
```

### Comparing `foundrytools-cli-1.0.1/LICENSE` & `foundrytools-cli-1.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/PKG-INFO` & `foundrytools-cli-1.0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundrytools-cli
-Version: 1.0.1
+Version: 1.0.2.1
 Summary: A set of command line tools to inspect, manipulate and convert font files
 Home-page: https://github.com/ftCLI/FoundryTools-CLI
 Author: ftCLI
 Author-email: ftcli@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -24,15 +24,15 @@
 * [dehinter](https://github.com/source-foundry/dehinter)
 * [beziers](https://github.com/simoncozens/beziers.py)
 
 The command line interface is built with [click](https://github.com/pallets/click/) and tables are rendered by
 [rich](https://github.com/Textualize/rich).
 
 Even if not directly imported to keep the footprint as small as possible, portions of code have been copied from
-[fontbakery](https://github.com/googlefonts/fontbakery).
+[fontbakery](https://github.com/googlefonts/fontbakery) and [font-line](https://github.com/source-foundry/font-line).
 
 ## Installation
 FoundryTools-CLI requires Python 3.9 or later.
 
 **Note for Windows users**: installation on Python 3.11 is strongly discouraged because AFDKO 3.9.6 doesn't support
 it, and an attempt of installation would probably fail. Since macOS users successfully installed FoundryTools-CLI on
 Python 3.11, requirements have been loosened up.
@@ -43,14 +43,17 @@
 
     python -m pip install foundrytools-cli
 
 ### Editable mode
 If you would like to contribute to the development, you can clone the repository from GitHub, install the package in
 'editable' mode and modify the source code in place. We strongly recommend using a virtual environment.
 
+**IMPORTANT**: If you have Python 2.x installed in your system, you may have to use `python3` (instead of `python`) in
+the commands below.
+
     # clone the repository:
     git clone https://github.com/ftCLI/foundrytools-cli.git
     cd foundrytools-cli
 
     # create new virtual environment named e.g. ftcli-venv, or whatever you prefer:
     python -m venv ftcli-venv
     
@@ -59,14 +62,15 @@
     
     # to activate the virtual environment in Windows, do:
     ftcli-venv\Scripts\activate.bat
     
     # install in 'editable' mode
     python -m pip install -e .
 
+
 ## Documentation
 FoundryTools-CLI is a Terminal app where commands are logically organized into subcommands.
 
 Please refer to the [user documentation](https://ftcli.github.io/FoundryTools-CLI/).
 
 ## License
 FoundryTools-CLI is available under the [MIT license](LICENSE)
```

### Comparing `foundrytools-cli-1.0.1/README.md` & `foundrytools-cli-1.0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * [dehinter](https://github.com/source-foundry/dehinter)
 * [beziers](https://github.com/simoncozens/beziers.py)
 
 The command line interface is built with [click](https://github.com/pallets/click/) and tables are rendered by
 [rich](https://github.com/Textualize/rich).
 
 Even if not directly imported to keep the footprint as small as possible, portions of code have been copied from
-[fontbakery](https://github.com/googlefonts/fontbakery).
+[fontbakery](https://github.com/googlefonts/fontbakery) and [font-line](https://github.com/source-foundry/font-line).
 
 ## Installation
 FoundryTools-CLI requires Python 3.9 or later.
 
 **Note for Windows users**: installation on Python 3.11 is strongly discouraged because AFDKO 3.9.6 doesn't support
 it, and an attempt of installation would probably fail. Since macOS users successfully installed FoundryTools-CLI on
 Python 3.11, requirements have been loosened up.
@@ -30,14 +30,17 @@
 
     python -m pip install foundrytools-cli
 
 ### Editable mode
 If you would like to contribute to the development, you can clone the repository from GitHub, install the package in
 'editable' mode and modify the source code in place. We strongly recommend using a virtual environment.
 
+**IMPORTANT**: If you have Python 2.x installed in your system, you may have to use `python3` (instead of `python`) in
+the commands below.
+
     # clone the repository:
     git clone https://github.com/ftCLI/foundrytools-cli.git
     cd foundrytools-cli
 
     # create new virtual environment named e.g. ftcli-venv, or whatever you prefer:
     python -m venv ftcli-venv
     
@@ -46,14 +49,15 @@
     
     # to activate the virtual environment in Windows, do:
     ftcli-venv\Scripts\activate.bat
     
     # install in 'editable' mode
     python -m pip install -e .
 
+
 ## Documentation
 FoundryTools-CLI is a Terminal app where commands are logically organized into subcommands.
 
 Please refer to the [user documentation](https://ftcli.github.io/FoundryTools-CLI/).
 
 ## License
 FoundryTools-CLI is available under the [MIT license](LICENSE)
```

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_assistant.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_assistant.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_cff.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_cff.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_converter.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_converter.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_fix.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_fix.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_hhea.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_hhea.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_metrics.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_metrics.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_name.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_name.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_os2.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_os2.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_otf.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_otf.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_post.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_post.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_print.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_print.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_ttf.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_ttf.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/CLI/ftcli_utils.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/CLI/ftcli_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,17 +222,15 @@
             try:
                 output_file = Path(
                     makeOutputFileName(
                         new_file_name, extension=new_file_extension, outputDir=file.parent, overWrite=False
                     )
                 )
                 file.rename(output_file)
-                generic_success_message(
-                    f"{file.name} {click.style('-->', fg='bright_magenta')} {output_file.name}"
-                )
+                generic_success_message(f"{file.name} {click.style('-->', fg='bright_magenta')} {output_file.name}")
             except Exception as e:
                 generic_error_message(e)
         else:
             file_not_changed_message(file)
 
         font.close()
```

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/Font.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/Font.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/VFont.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/VFont.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/UI.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/assistant/UI.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/fonts_data.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/assistant/fonts_data.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/assistant/styles_mapping.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/assistant/styles_mapping.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/constants.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/constants.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/options.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/options.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/otf_to_ttf.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/otf_to_ttf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,16 @@
         start_time = time.time()
 
         for count, source_font in enumerate(source_fonts, start=1):
             t = time.time()
 
             try:
                 print()
-                generic_info_message(f"Converting file {count} of {len(source_fonts)}")
-
                 file = Path(source_font.reader.file.name)
+                generic_info_message(f"Converting file {count} of {len(source_fonts)}: {file.name}")
 
                 # If the source font is a WOFF or WOFF2, we add a suffix to avoid unwanted overwriting
                 if source_font.flavor is None:
                     ext = ".ttf"
                     suffix = ""
                 else:
                     ext = source_font.get_real_extension()
```

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/sfnt_to_web.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/sfnt_to_web.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
     def run(self, fonts: list[Font]) -> None:
         converted_files_count = 0
         start_time = time.time()
 
         for count, font in enumerate(fonts, start=1):
             t = time.time()
-            print()
-            generic_info_message(f"Converting file {count} of {len(fonts)}")
 
             try:
                 if font.flavor is not None:
                     continue
 
-                file = font.reader.file.name
+                file = Path(font.reader.file.name)
+                print()
+                generic_info_message(f"Converting file {count} of {len(fonts)}: {file.name}")
 
                 if self.options.woff:
                     converter = SFNTToWeb(font=font, flavor="woff")
                     web_font = converter.run()
                     extension = web_font.get_real_extension()
                     output_file = Path(
                         makeOutputFileName(
```

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/ttc_to_sfnt.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/ttc_to_sfnt.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/ttf_to_otf.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/ttf_to_otf.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
     def run(self, source_fonts: list[Font]) -> None:
         converted_files_count = 0
         start_time = time.time()
 
         for count, source_font in enumerate(source_fonts, start=1):
             t = time.time()
-            print()
-            generic_info_message(f"Converting file {count} of {len(source_fonts)}")
 
             try:
                 file = Path(source_font.reader.file.name)
+                print()
+                generic_info_message(f"Converting file {count} of {len(source_fonts)}: {file.name}")
 
                 # If the source font is a WOFF or WOFF2, we add a suffix to avoid unwanted overwriting
                 flavor = source_font.flavor
                 if flavor is None:
                     ext = ".otf"
                     suffix = ""
                 else:
@@ -66,29 +66,29 @@
                 # Decomponentize the source font
                 source_font.ttf_decomponentize()
 
                 tolerance = self.options.tolerance / 1000 * source_font["head"].unitsPerEm
                 failed, charstrings = get_qu2cu_charstrings(font=source_font, tolerance=tolerance)
 
                 if len(failed) > 0:
-                    generic_info_message(f"Getting {len(failed)} charstrings with makeotf...")
+                    generic_info_message(f"Retrying to get {len(failed)} charstrings...")
                     t2_ttf2otf_converter = TrueTypeToCFF(font=source_font)
                     t2_charstrings = get_t2_charstrings(font=source_font)
                     t2_otf_font: Font = t2_ttf2otf_converter.run(charstrings=t2_charstrings)
                     t2_otf_2_ttf_converter = CFFToTrueType(font=t2_otf_font)
                     t2_otf_2_ttf_font = t2_otf_2_ttf_converter.run()
                     _, fallback_charstrings = get_qu2cu_charstrings(t2_otf_2_ttf_font)
 
                     for c in failed:
                         try:
-                            generic_info_message(f"Retrying to get charstring: {c}", nl=False)
+                            generic_info_message(f"{c}", nl=False)
                             charstrings[c] = fallback_charstrings[c]
-                            click.secho(f" -> OK", fg="green")
+                            click.secho(f" -> {click.style('OK', fg='green')}")
                         except Exception as e:
-                            generic_error_message(f"Failed to get charstring: {c}")
+                            click.secho(f" -> {click.style('FAIL', fg='red')} ({e})")
                             generic_error_message(e)
 
                 ttf2otf_converter = TrueTypeToCFF(font=source_font)
                 cff_font: Font = ttf2otf_converter.run(charstrings=charstrings)
 
                 cff_font.otf_fix_contours(min_area=25, verbose=False)
```

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/variable_to_static.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/variable_to_static.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/converters/web_to_sfnt.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/converters/web_to_sfnt.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
     def run(self, fonts: list[Font]) -> None:
         converted_files_count = 0
         start_time = time.time()
 
         for count, font in enumerate(fonts, start=1):
             t = time.time()
-            print()
-            generic_info_message(f"Converting file {count} of {len(fonts)}")
 
             try:
-                file = font.reader.file.name
+                file = Path(font.reader.file.name)
+                print()
+                generic_info_message(f"Converting file {count} of {len(fonts)}: {file.name}")
 
                 if not font.flavor:
                     continue
                 if not self.options.woff:
                     if font.flavor == "woff":
                         continue
                 if not self.options.woff2:
```

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/printer/UI.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/printer/UI.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/CFF_.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/CFF_.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/OS_2.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/OS_2.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/head.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/head.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/hhea.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/hhea.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/name.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/name.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/tables/post.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/tables/post.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/bits_tools.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/bits_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/cli_tools.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/click_tools.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/click_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,15 @@
         ),
     ]
     return add_options(_common_options)
 
 
 def file_overwrite_prompt(input_file: Path) -> bool:
     return click.confirm(
-        f"{click.style(input_file, fg='yellow', bold=True)} already exists. "
-        f"Do you want to overwrite it?"
+        f"{click.style(input_file, fg='yellow', bold=True)} already exists. " f"Do you want to overwrite it?"
     )
 
 
 def file_not_selected_message(file: Path):
     click.secho(
         f"[{click.style('SKIP', fg='yellow')}] {file.name} ({click.style('file is not selected', fg='yellow')})"
     )
```

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/otf_tools.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/otf_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/skia_tools.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/skia_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/text_tools.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/text_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/Lib/utils/ttf_tools.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/Lib/utils/ttf_tools.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundryToolsCLI/__main__.py` & `foundrytools-cli-1.0.2.1/foundryToolsCLI/__main__.py`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/foundrytools_cli.egg-info/PKG-INFO` & `foundrytools-cli-1.0.2.1/foundrytools_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundrytools-cli
-Version: 1.0.1
+Version: 1.0.2.1
 Summary: A set of command line tools to inspect, manipulate and convert font files
 Home-page: https://github.com/ftCLI/FoundryTools-CLI
 Author: ftCLI
 Author-email: ftcli@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -24,15 +24,15 @@
 * [dehinter](https://github.com/source-foundry/dehinter)
 * [beziers](https://github.com/simoncozens/beziers.py)
 
 The command line interface is built with [click](https://github.com/pallets/click/) and tables are rendered by
 [rich](https://github.com/Textualize/rich).
 
 Even if not directly imported to keep the footprint as small as possible, portions of code have been copied from
-[fontbakery](https://github.com/googlefonts/fontbakery).
+[fontbakery](https://github.com/googlefonts/fontbakery) and [font-line](https://github.com/source-foundry/font-line).
 
 ## Installation
 FoundryTools-CLI requires Python 3.9 or later.
 
 **Note for Windows users**: installation on Python 3.11 is strongly discouraged because AFDKO 3.9.6 doesn't support
 it, and an attempt of installation would probably fail. Since macOS users successfully installed FoundryTools-CLI on
 Python 3.11, requirements have been loosened up.
@@ -43,14 +43,17 @@
 
     python -m pip install foundrytools-cli
 
 ### Editable mode
 If you would like to contribute to the development, you can clone the repository from GitHub, install the package in
 'editable' mode and modify the source code in place. We strongly recommend using a virtual environment.
 
+**IMPORTANT**: If you have Python 2.x installed in your system, you may have to use `python3` (instead of `python`) in
+the commands below.
+
     # clone the repository:
     git clone https://github.com/ftCLI/foundrytools-cli.git
     cd foundrytools-cli
 
     # create new virtual environment named e.g. ftcli-venv, or whatever you prefer:
     python -m venv ftcli-venv
     
@@ -59,14 +62,15 @@
     
     # to activate the virtual environment in Windows, do:
     ftcli-venv\Scripts\activate.bat
     
     # install in 'editable' mode
     python -m pip install -e .
 
+
 ## Documentation
 FoundryTools-CLI is a Terminal app where commands are logically organized into subcommands.
 
 Please refer to the [user documentation](https://ftcli.github.io/FoundryTools-CLI/).
 
 ## License
 FoundryTools-CLI is available under the [MIT license](LICENSE)
```

### Comparing `foundrytools-cli-1.0.1/foundrytools_cli.egg-info/SOURCES.txt` & `foundrytools-cli-1.0.2.1/foundrytools_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foundrytools-cli-1.0.1/setup.py` & `foundrytools-cli-1.0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = this_directory.joinpath("README.md").read_text()
 
 setuptools.setup(
     name="foundrytools-cli",
-    version="1.0.1",
+    version="1.0.2.1",
     description="A set of command line tools to inspect, manipulate and convert font files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ftCLI",
     author_email="ftcli@proton.me",
     url="https://github.com/ftCLI/FoundryTools-CLI",
     packages=setuptools.find_packages(),
```

