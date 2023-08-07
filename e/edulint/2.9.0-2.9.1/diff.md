# Comparing `tmp/edulint-2.9.0.tar.gz` & `tmp/edulint-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-92ejrrvg/edulint-2.9.0.tar", last modified: Mon Aug  7 18:50:25 2023, max compression
+gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-9nxiwdfi/edulint-2.9.1.tar", last modified: Mon Aug  7 19:24:36 2023, max compression
```

## Comparing `edulint-2.9.0.tar` & `edulint-2.9.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 18:50:11.000000 edulint-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-07 18:50:25.000000 edulint-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-07 18:50:11.000000 edulint-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/config_translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/file_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/config/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/files/default.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/files/empty.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/explanations.py
--rw-r--r--   0 runner    (1001) docker     (123)   190327 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/explanations.toml
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/linting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/linting/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/basic_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    25119 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/duplication_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/modified_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/python_ta_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/linting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/nonparsing_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/process_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/tweakers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/option_parses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/prepare_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/prepare_explanations/pylint_data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/pylint_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/pylint_data/pylint_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/prepare_explanations/thonny_data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/thonny_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/thonny_data/thonny_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 18:50:11.000000 edulint-2.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-07 18:50:25.000000 edulint-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-07 18:50:11.000000 edulint-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    22621 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:36.000000 edulint-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 19:24:25.000000 edulint-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-07 19:24:36.000000 edulint-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-07 19:24:25.000000 edulint-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/config/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/config/config_translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/config/file_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint/config/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/config/files/default.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/config/files/empty.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190327 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/explanations.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint/linting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint/linting/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/checkers/basic_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25119 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/checkers/duplication_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/checkers/improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/checkers/modified_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/checkers/python_ta_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/checkers/short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/checkers/simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/checkers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/linting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/nonparsing_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/process_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/linting/tweakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/option_parses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint/prepare_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/prepare_explanations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint/prepare_explanations/pylint_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/prepare_explanations/pylint_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/prepare_explanations/pylint_data/pylint_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint/prepare_explanations/thonny_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/prepare_explanations/thonny_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/prepare_explanations/thonny_data/thonny_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-08-07 19:24:25.000000 edulint-2.9.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 19:24:36.000000 edulint-2.9.1/edulint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 19:24:25.000000 edulint-2.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-07 19:24:36.000000 edulint-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-07 19:24:25.000000 edulint-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:24:36.000000 edulint-2.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-08-07 19:24:25.000000 edulint-2.9.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-08-07 19:24:25.000000 edulint-2.9.1/tests/test_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-07 19:24:25.000000 edulint-2.9.1/tests/test_improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22621 2023-08-07 19:24:25.000000 edulint-2.9.1/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-08-07 19:24:25.000000 edulint-2.9.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-08-07 19:24:25.000000 edulint-2.9.1/tests/test_short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-08-07 19:24:25.000000 edulint-2.9.1/tests/test_simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-08-07 19:24:25.000000 edulint-2.9.1/tests/test_visitors.py
```

### Comparing `edulint-2.9.0/LICENSE` & `edulint-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/PKG-INFO` & `edulint-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.9.0
+Version: 2.9.1
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.9.0/README.md` & `edulint-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/config/config.py` & `edulint-2.9.1/edulint/config/config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/config/config_translations.py` & `edulint-2.9.1/edulint/config/config_translations.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/config/file_config.py` & `edulint-2.9.1/edulint/config/file_config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/config/files/default.toml` & `edulint-2.9.1/edulint/config/files/default.toml`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     "remove-for",
     "redundant-arithmetic",
     "do-not-multiply-mutable",
     "redundant-elif",
     "unreachable-else",
     "invalid-name",
     "consider-using-from-import",
-    "wildcard-import",
     "reimported",
     "invalid-for-target",
     "one-iteration",
     "no-is-bool",
     "use-ord-letter",
     "use-literal-letter",
     "use-foreach",
```

### Comparing `edulint-2.9.0/edulint/edulint.py` & `edulint-2.9.1/edulint/edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/explanations.toml` & `edulint-2.9.1/edulint/explanations.toml`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linters.py` & `edulint-2.9.1/edulint/linters.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/checkers/basic_checker.py` & `edulint-2.9.1/edulint/linting/checkers/basic_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/checkers/duplication_checker.py` & `edulint-2.9.1/edulint/linting/checkers/duplication_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/checkers/improper_loop.py` & `edulint-2.9.1/edulint/linting/checkers/improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/checkers/modified_listener.py` & `edulint-2.9.1/edulint/linting/checkers/modified_listener.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/checkers/python_ta_checkers.py` & `edulint-2.9.1/edulint/linting/checkers/python_ta_checkers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/checkers/short_problems.py` & `edulint-2.9.1/edulint/linting/checkers/short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/checkers/simplifiable_if.py` & `edulint-2.9.1/edulint/linting/checkers/simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/checkers/utils.py` & `edulint-2.9.1/edulint/linting/checkers/utils.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/linting.py` & `edulint-2.9.1/edulint/linting/linting.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/nonparsing_checkers.py` & `edulint-2.9.1/edulint/linting/nonparsing_checkers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/overrides.py` & `edulint-2.9.1/edulint/linting/overrides.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/problem.py` & `edulint-2.9.1/edulint/linting/problem.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/process_handler.py` & `edulint-2.9.1/edulint/linting/process_handler.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/linting/tweakers.py` & `edulint-2.9.1/edulint/linting/tweakers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/option_parses.py` & `edulint-2.9.1/edulint/option_parses.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/options.py` & `edulint-2.9.1/edulint/options.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/prepare_explanations/__init__.py` & `edulint-2.9.1/edulint/prepare_explanations/__init__.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py` & `edulint-2.9.1/edulint/prepare_explanations/pylint_data/extract_from_pylint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/prepare_explanations/pylint_data/pylint_messages.py` & `edulint-2.9.1/edulint/prepare_explanations/pylint_data/pylint_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py` & `edulint-2.9.1/edulint/prepare_explanations/pylint_data/thonny_process_slim.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py` & `edulint-2.9.1/edulint/prepare_explanations/thonny_data/extract_from_edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/prepare_explanations/thonny_data/thonny_messages.py` & `edulint-2.9.1/edulint/prepare_explanations/thonny_data/thonny_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py` & `edulint-2.9.1/edulint/prepare_explanations/thonny_data/thonny_process_backup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/edulint.egg-info/PKG-INFO` & `edulint-2.9.1/edulint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.9.0
+Version: 2.9.1
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.9.0/edulint.egg-info/SOURCES.txt` & `edulint-2.9.1/edulint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/setup.cfg` & `edulint-2.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/setup.py` & `edulint-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/tests/test_config.py` & `edulint-2.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/tests/test_duplication.py` & `edulint-2.9.1/tests/test_duplication.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/tests/test_improper_loop.py` & `edulint-2.9.1/tests/test_improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/tests/test_lint.py` & `edulint-2.9.1/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/tests/test_main.py` & `edulint-2.9.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/tests/test_short_problems.py` & `edulint-2.9.1/tests/test_short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/tests/test_simplifiable_if.py` & `edulint-2.9.1/tests/test_simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.9.0/tests/test_visitors.py` & `edulint-2.9.1/tests/test_visitors.py`

 * *Files identical despite different names*

