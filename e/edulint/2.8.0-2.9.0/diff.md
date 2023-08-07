# Comparing `tmp/edulint-2.8.0.tar.gz` & `tmp/edulint-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-bo8c75cm/edulint-2.8.0.tar", last modified: Sat Aug  5 11:02:26 2023, max compression
+gzip compressed data, was "/home/runner/work/edulint/edulint/dist/.tmp-92ejrrvg/edulint-2.9.0.tar", last modified: Mon Aug  7 18:50:25 2023, max compression
```

## Comparing `edulint-2.8.0.tar` & `edulint-2.9.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 11:02:14.000000 edulint-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-05 11:02:26.000000 edulint-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-05 11:02:14.000000 edulint-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/config_translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/file_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/config/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/files/default.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/config/files/empty.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/explanations.py
--rw-r--r--   0 runner    (1001) docker     (123)   190327 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/explanations.toml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/linting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/linting/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/basic_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    25119 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/duplication_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/modified_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/python_ta_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/checkers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/linting.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/process_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/linting/tweakers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/prepare_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/prepare_explanations/pylint_data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/pylint_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/pylint_data/pylint_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint/prepare_explanations/thonny_data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/thonny_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
--rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/thonny_data/thonny_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-08-05 11:02:14.000000 edulint-2.8.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-05 11:02:26.000000 edulint-2.8.0/edulint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-05 11:02:14.000000 edulint-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-05 11:02:26.000000 edulint-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-05 11:02:14.000000 edulint-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:02:26.000000 edulint-2.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_improper_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    21029 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_short_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_simplifiable_if.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-08-05 11:02:14.000000 edulint-2.8.0/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 18:50:11.000000 edulint-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-07 18:50:25.000000 edulint-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-08-07 18:50:11.000000 edulint-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/config_translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/file_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/config/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/files/default.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/config/files/empty.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190327 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/explanations.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/linting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/linting/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/basic_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25119 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/duplication_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/modified_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/python_ta_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/checkers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/linting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/nonparsing_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/process_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/linting/tweakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/option_parses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/prepare_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/prepare_explanations/pylint_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/pylint_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/pylint_data/pylint_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint/prepare_explanations/thonny_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/thonny_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155599 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/thonny_data/thonny_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-08-07 18:50:11.000000 edulint-2.9.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 18:50:25.000000 edulint-2.9.0/edulint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 18:50:11.000000 edulint-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-07 18:50:25.000000 edulint-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-07 18:50:11.000000 edulint-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:50:25.000000 edulint-2.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_improper_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22621 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_short_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_simplifiable_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-08-07 18:50:11.000000 edulint-2.9.0/tests/test_visitors.py
```

### Comparing `edulint-2.8.0/LICENSE` & `edulint-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/PKG-INFO` & `edulint-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.8.0
+Version: 2.9.0
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.8.0/README.md` & `edulint-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/config/config_translations.py` & `edulint-2.9.0/edulint/config/config_translations.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/config/file_config.py` & `edulint-2.9.0/edulint/config/file_config.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/config/files/default.toml` & `edulint-2.9.0/edulint/config/files/default.toml`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/edulint.py` & `edulint-2.9.0/edulint/edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/explanations.toml` & `edulint-2.9.0/edulint/explanations.toml`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linters.py` & `edulint-2.9.0/edulint/linters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from enum import Enum, auto
+from typing import Optional
 from edulint.options import Option
 
 
 class Linter(Enum):
     EDULINT = auto()
     PYLINT = auto()
     FLAKE8 = auto()
 
     def __str__(self: Enum) -> str:
         return self.name.lower()
 
     @staticmethod
-    def from_name(linter_str: str) -> "Linter":
+    def safe_from_name(linter_str: str) -> Optional["Linter"]:
         for linter in Linter:
             if str(linter) == linter_str.lower():
                 return linter
+        return None
+
+    @staticmethod
+    def from_name(linter_str: str) -> "Linter":
+        result = Linter.safe_from_name(linter_str)
+        if result is not None:
+            return result
         assert False, "no such linter: " + linter_str
 
     def to_name(self) -> str:
         return str(self)
 
     @classmethod
     def from_option(cls, option: Option) -> "Linter":
```

### Comparing `edulint-2.8.0/edulint/linting/checkers/basic_checker.py` & `edulint-2.9.0/edulint/linting/checkers/basic_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linting/checkers/duplication_checker.py` & `edulint-2.9.0/edulint/linting/checkers/duplication_checker.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linting/checkers/improper_loop.py` & `edulint-2.9.0/edulint/linting/checkers/improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linting/checkers/modified_listener.py` & `edulint-2.9.0/edulint/linting/checkers/modified_listener.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linting/checkers/python_ta_checkers.py` & `edulint-2.9.0/edulint/linting/checkers/python_ta_checkers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linting/checkers/short_problems.py` & `edulint-2.9.0/edulint/linting/checkers/short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linting/checkers/simplifiable_if.py` & `edulint-2.9.0/edulint/linting/checkers/simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linting/checkers/utils.py` & `edulint-2.9.0/edulint/linting/checkers/utils.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linting/linting.py` & `edulint-2.9.0/edulint/linting/linting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Callable, Tuple, Dict, Set, Any
 from edulint.linting.problem import ProblemJson, Problem
+from edulint.linting.nonparsing_checkers import report_infile_config
 from edulint.linting.process_handler import ProcessHandler
 from edulint.linting.overrides import get_overriders
 from edulint.linting.tweakers import get_tweakers, Tweakers
-from edulint.config.config import Config
+from edulint.config.config import ImmutableConfig
 from edulint.options import Option, ImmutableT
 from edulint.linters import Linter
 from functools import partial
 import sys
 import json
 import os
 
@@ -93,27 +94,34 @@
     if not outs:
         return []
 
     result = result_getter(json.loads(outs))
     return list(map(out_to_problem, result))
 
 
-def lint_flake8(filenames: List[str], config: Config) -> List[Problem]:
+def lint_edulint(filenames: List[str], config: ImmutableConfig) -> List[Problem]:
+    ignored_infile = set(config[Option.IGNORE_INFILE_CONFIG_FOR])
+    if len(ignored_infile) > 0:
+        return report_infile_config(filenames, ignored_infile)
+    return []
+
+
+def lint_flake8(filenames: List[str], config: ImmutableConfig) -> List[Problem]:
     flake8_args = ["--format=json"]
     return lint_any(
         Linter.FLAKE8,
         filenames,
         flake8_args,
         config[Option.FLAKE8],
         lambda r: [problem for problems in r.values() for problem in problems],
         flake8_to_problem,
     )
 
 
-def lint_pylint(filenames: List[str], config: Config) -> List[Problem]:
+def lint_pylint(filenames: List[str], config: ImmutableConfig) -> List[Problem]:
     pylint_args = ["--output-format=json"]
     return lint_any(
         Linter.PYLINT,
         filenames,
         pylint_args,
         config[Option.PYLINT],
         lambda r: r,
@@ -134,43 +142,45 @@
         o = overriders.get(problem.code, set())
         if not (o & codes_on_lines[problem.line]):
             result.append(problem)
 
     return result
 
 
-def apply_tweaks(problems: List[Problem], tweakers: Tweakers, config: Config) -> List[Problem]:
+def apply_tweaks(
+    problems: List[Problem], tweakers: Tweakers, config: ImmutableConfig
+) -> List[Problem]:
     result = []
     for problem in problems:
         tweaker = tweakers.get((problem.source, problem.code))
         if tweaker:
             if tweaker.should_keep(
                 problem, [arg for arg in config if arg.option in tweaker.used_options]
             ):
                 problem.text = tweaker.get_reword(problem)
                 result.append(problem)
         else:
             result.append(problem)
     return result
 
 
-def lint_one(filename: str, config: Config) -> List[Problem]:
+def lint_one(filename: str, config: ImmutableConfig) -> List[Problem]:
     return lint([filename], config)
 
 
 def sort(filenames: List[str], problems: List[Problem]) -> List[Problem]:
     indices = {get_proper_path(fn): i for i, fn in enumerate(filenames)}
     problems.sort(key=lambda problem: (indices[problem.path], problem.line, problem.column))
     return problems
 
 
-def lint(filenames: List[str], config: Config) -> List[Problem]:
-    result = ([] if config[Option.NO_FLAKE8] else lint_flake8(filenames, config)) + lint_pylint(
-        filenames, config
-    )
-    result = apply_overrides(result, get_overriders())
+def lint(filenames: List[str], config: ImmutableConfig) -> List[Problem]:
+    edulint_result = lint_edulint(filenames, config)
+    flake8_result = [] if config[Option.NO_FLAKE8] else lint_flake8(filenames, config)
+    pylint_result = lint_pylint(filenames, config)
+    result = apply_overrides(edulint_result + flake8_result + pylint_result, get_overriders())
     result = apply_tweaks(result, get_tweakers(), config)
     return sort(filenames, result)
 
 
-def lint_many(partition: List[Tuple[List[str], Config]]) -> List[Problem]:
+def lint_many(partition: List[Tuple[List[str], ImmutableConfig]]) -> List[Problem]:
     return [problem for filenames, config in partition for problem in lint(filenames, config)]
```

### Comparing `edulint-2.8.0/edulint/linting/overrides.py` & `edulint-2.9.0/edulint/linting/overrides.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linting/problem.py` & `edulint-2.9.0/edulint/linting/problem.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linting/process_handler.py` & `edulint-2.9.0/edulint/linting/process_handler.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/linting/tweakers.py` & `edulint-2.9.0/edulint/linting/tweakers.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/options.py` & `edulint-2.9.0/edulint/option_parses.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,12 @@
 from dataclasses import dataclass
-from typing import Dict, List, Any, TypeVar, Optional, Union, Callable, Tuple
+from typing import Dict, List, Any, Optional, Callable
 from enum import Enum, auto
-
-
-class NumberFromZero(Enum):
-    def __new__(cls, *args: Any) -> "NumberFromZero":
-        value = len(cls.__members__)
-        obj = object.__new__(cls)
-        obj._value_ = value
-        return obj
-
-
-T = TypeVar("T")
-UnionT = Union[bool, List[str], Optional[str], Optional[int]]
-ImmutableT = Union[bool, Tuple[str, ...], Optional[str], Optional[int]]
-
-
-class Option(NumberFromZero):
-    CONFIG = ()
-    PYLINT = ()
-    FLAKE8 = ()
-    ENHANCEMENT = ()
-    PYTHON_SPECIFIC = ()
-    COMPLEXITY = ()
-    ALLOWED_ONECHAR_NAMES = ()
-    IB111_WEEK = ()
-    NO_FLAKE8 = ()
-
-    def to_name(self) -> str:
-        return self.name.lower().replace("_", "-")
-
-    @staticmethod
-    def from_name(option_str: str) -> "Option":
-        for option in Option:
-            if option.to_name() == option_str.lower():
-                return option
-        assert False, "no such option: " + option_str
-
-    def __int__(self) -> int:
-        return self.value  # type: ignore
+from edulint.options import Option, UnionT, T, DEFAULT_CONFIG
+from edulint.linters import Linter
 
 
 class TakesVal(Enum):
     YES = auto()
     NO = auto()
     OPTIONAL = auto()
 
@@ -100,31 +64,27 @@
     def __init__(self, _: Enum, combine: Callable[[UnionT, UnionT], UnionT]):
         self.combine: Callable[[UnionT, UnionT], UnionT] = combine.__func__  # type: ignore
 
     def __call__(self, lt: UnionT, rt: UnionT) -> UnionT:
         return self.combine(lt, rt)
 
     REPLACE = (auto(), _keep_right_combine)
-    APPEND = (auto(), _append_combine)
     EXTEND = (auto(), _extend_combine)
 
 
 @dataclass
 class OptionParse:
     option: Option
     help_: str
     takes_val: TakesVal
     default: UnionT
     convert: Type
     combine: Combine
 
 
-DEFAULT_CONFIG = "default"
-BASE_CONFIG = "empty"
-
 OPTIONS: List[OptionParse] = [
     OptionParse(
         Option.CONFIG,
         "config file to use for the linting (packaged name, local path or remote)",
         TakesVal.YES,
         DEFAULT_CONFIG,
         Type.STR,
@@ -185,14 +145,24 @@
         None,
         Type.INT,
         Combine.REPLACE,
     ),
     OptionParse(
         Option.NO_FLAKE8, "turn off flake8", TakesVal.NO, False, Type.BOOL, Combine.REPLACE
     ),
+    OptionParse(
+        Option.IGNORE_INFILE_CONFIG_FOR,
+        "warns about infile supressions (like # noqa) for given linters, "
+        f"valid values are {', '.join(linter.to_name() for linter in Linter)} and all, "
+        f"if values {Linter.EDULINT} or all are set in-file, all other in-file configuration is ignored",
+        TakesVal.YES,
+        [],
+        Type.LIST,
+        Combine.REPLACE,
+    ),
 ]
 
 OLD_NAMES = {"python-spec": Option.PYTHON_SPECIFIC}
 
 
 def get_option_parses() -> Dict[Option, OptionParse]:
     return {parse.option: parse for parse in OPTIONS}
```

### Comparing `edulint-2.8.0/edulint/prepare_explanations/__init__.py` & `edulint-2.9.0/edulint/prepare_explanations/__init__.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py` & `edulint-2.9.0/edulint/prepare_explanations/pylint_data/extract_from_pylint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/prepare_explanations/pylint_data/pylint_messages.py` & `edulint-2.9.0/edulint/prepare_explanations/pylint_data/pylint_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py` & `edulint-2.9.0/edulint/prepare_explanations/pylint_data/thonny_process_slim.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py` & `edulint-2.9.0/edulint/prepare_explanations/thonny_data/extract_from_edulint.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/prepare_explanations/thonny_data/thonny_messages.py` & `edulint-2.9.0/edulint/prepare_explanations/thonny_data/thonny_messages.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py` & `edulint-2.9.0/edulint/prepare_explanations/thonny_data/thonny_process_backup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/edulint.egg-info/PKG-INFO` & `edulint-2.9.0/edulint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edulint
-Version: 2.8.0
+Version: 2.9.0
 Summary: A Python Educational Linter
 Home-page: https://github.com/GiraffeReversed/edulint
 Author: Anna Rechtackova
 Author-email: anna.rechtackova@mail.muni.cz
 Project-URL: Bug Tracker, https://github.com/GiraffeReversed/edulint/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `edulint-2.8.0/edulint.egg-info/SOURCES.txt` & `edulint-2.9.0/edulint.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 setup.py
 ./edulint/__init__.py
 ./edulint/__main__.py
 ./edulint/edulint.py
 ./edulint/explanations.py
 ./edulint/explanations.toml
 ./edulint/linters.py
+./edulint/option_parses.py
 ./edulint/options.py
 ./edulint/config/__init__.py
 ./edulint/config/arg.py
 ./edulint/config/config.py
 ./edulint/config/config_translations.py
 ./edulint/config/file_config.py
 ./edulint/config/files/default.toml
 ./edulint/config/files/empty.toml
 ./edulint/linting/__init__.py
 ./edulint/linting/linting.py
+./edulint/linting/nonparsing_checkers.py
 ./edulint/linting/overrides.py
 ./edulint/linting/problem.py
 ./edulint/linting/process_handler.py
 ./edulint/linting/tweakers.py
 ./edulint/linting/checkers/__init__.py
 ./edulint/linting/checkers/basic_checker.py
 ./edulint/linting/checkers/duplication_checker.py
```

### Comparing `edulint-2.8.0/setup.cfg` & `edulint-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/setup.py` & `edulint-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/tests/test_config.py` & `edulint-2.9.0/tests/test_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import pytest
 from edulint.linters import Linter
 from edulint.config.arg import UnprocessedArg, ProcessedArg
-from edulint.options import Option, TakesVal, Type, Combine, OptionParse, get_option_parses, DEFAULT_CONFIG
-from edulint.config.config import Config, extract_args, parse_args, parse_config_file, combine_and_translate
-from edulint.config.config_translations import get_config_translations, Translation
+from edulint.options import Option, DEFAULT_CONFIG
+from edulint.option_parses import OptionParse, get_option_parses, TakesVal, Type, Combine
+from edulint.config.arg import Arg
+from edulint.config.config import Config, extract_args, parse_args, parse_config_file, get_config_many, get_config_one
+from edulint.config.config_translations import get_config_translations, get_ib111_translations, Translation
 from edulint.linting.tweakers import get_tweakers
-from typing import List, Set, Dict
+from utils import get_tests_path
+from typing import List, Set, Dict, Tuple, Optional
 from pathlib import Path
 
 
 @pytest.fixture
 def all_advertised_options() -> List[Option]:
     return list(get_option_parses().keys())
 
@@ -17,15 +20,24 @@
 @pytest.fixture
 def advertised_options(all_advertised_options: List[Option]) -> Set[Option]:
     return set(all_advertised_options)
 
 
 @pytest.fixture
 def always_managed_options() -> Set[Option]:
-    return set((Option.CONFIG, Option.PYLINT, Option.FLAKE8, Option.IB111_WEEK, Option.NO_FLAKE8))
+    return set(
+        (
+            Option.CONFIG,
+            Option.PYLINT,
+            Option.FLAKE8,
+            Option.IB111_WEEK,
+            Option.NO_FLAKE8,
+            Option.IGNORE_INFILE_CONFIG_FOR,
+        )
+    )
 
 
 @pytest.fixture
 def managed_translations_options() -> List[Option]:
     return list(get_config_translations().keys())
 
 
@@ -99,49 +111,47 @@
     assert extract_args("foo") == args
 
 
 @pytest.fixture
 def options() -> Dict[Option, OptionParse]:
     return {
         Option.PYTHON_SPECIFIC: OptionParse(Option.PYTHON_SPECIFIC, "", TakesVal.NO, False, Type.BOOL, Combine.REPLACE),
-        Option.FLAKE8: OptionParse(Option.FLAKE8, "", TakesVal.YES, [], Type.STR, Combine.APPEND),
+        Option.FLAKE8: OptionParse(Option.FLAKE8, "", TakesVal.YES, [], Type.STR, Combine.EXTEND),
         Option.IB111_WEEK: OptionParse(Option.IB111_WEEK, "", TakesVal.YES, None, Type.INT, Combine.REPLACE),
         Option.CONFIG: OptionParse(Option.CONFIG, "", TakesVal.YES, DEFAULT_CONFIG, Type.STR, Combine.REPLACE)
     }
 
 
 @pytest.mark.parametrize("raw,parsed", [
-    (["python-specific"], ("default", [UnprocessedArg(Option.PYTHON_SPECIFIC, None)])),
-    (["python-spec"], ("default", [UnprocessedArg(Option.PYTHON_SPECIFIC, None)])),
-    (["flake8=foo"], ("default", [UnprocessedArg(Option.FLAKE8, "foo")])),
-    (["flake8="], ("default", [UnprocessedArg(Option.FLAKE8, "")])),
-    (["python-specific", "flake8=foo"], ("default", [
+    (["python-specific"], [UnprocessedArg(Option.PYTHON_SPECIFIC, None)]),
+    (["python-spec"], [UnprocessedArg(Option.PYTHON_SPECIFIC, None)]),
+    (["flake8=foo"], [UnprocessedArg(Option.FLAKE8, "foo")]),
+    (["flake8="], [UnprocessedArg(Option.FLAKE8, "")]),
+    (["python-specific", "flake8=foo"], [
        UnprocessedArg(Option.PYTHON_SPECIFIC, None), UnprocessedArg(Option.FLAKE8, "foo")
-    ])),
-    (["flake8=--enable=xxx"], ("default", [UnprocessedArg(Option.FLAKE8, "--enable=xxx")])),
-    (["ib111-week=02"], ("default", [UnprocessedArg(Option.IB111_WEEK, "02")])),
-    (["ib111-week=12", "ib111-week=02"], ("default", [
+    ]),
+    (["flake8=--enable=xxx"], [UnprocessedArg(Option.FLAKE8, "--enable=xxx")]),
+    (["ib111-week=02"], [UnprocessedArg(Option.IB111_WEEK, "02")]),
+    (["ib111-week=12", "ib111-week=02"], [
        UnprocessedArg(Option.IB111_WEEK, "12"), UnprocessedArg(Option.IB111_WEEK, "02")
-    ])),
-    (["config=empty"], ("empty", [UnprocessedArg(Option.CONFIG, "empty")]))
+    ]),
+    (["config=empty"], [UnprocessedArg(Option.CONFIG, "empty")])
 ])
 def test_parse_args(raw: List[str], options: Dict[Option, OptionParse], parsed: List[UnprocessedArg]) -> None:
     assert parse_args(raw, options) == parsed
 
 
 def packaged_config_files():
     packaged_config_dir = Path(__file__).parent / ".." / "edulint" / "config" / "files"
     return [c.stem for c in packaged_config_dir.iterdir() if c.suffix == ".toml"]
 
 
 @pytest.mark.parametrize("config_name", packaged_config_files())
 def test_packaged_configs_parse(config_name: str):
-    option_parses = get_option_parses()
-    print(config_name)
-    assert parse_config_file(config_name, option_parses) is not None
+    assert parse_config_file(config_name, get_option_parses()) is not None
 
 
 @pytest.fixture
 def config_translations() -> Dict[Option, Translation]:
     return {
         Option.ENHANCEMENT: Translation(
             Linter.PYLINT,
@@ -166,58 +176,145 @@
         Translation(Linter.PYLINT, ["kkk"]),
     ]
 
 
 @pytest.mark.parametrize("args,config", [
     (
         [UnprocessedArg(Option.ENHANCEMENT, None)],
-        Config([ProcessedArg(Option.ENHANCEMENT, True), ProcessedArg(Option.PYLINT, ["aaa"])])
+        [ProcessedArg(Option.ENHANCEMENT, True), ProcessedArg(Option.PYLINT, ["aaa"])]
     ),
     (
         [UnprocessedArg(Option.ENHANCEMENT, None), UnprocessedArg(Option.PYLINT, "zzz")],
-        Config([ProcessedArg(Option.ENHANCEMENT, True), ProcessedArg(Option.PYLINT, ["aaa", "zzz"])])
+        [ProcessedArg(Option.ENHANCEMENT, True), ProcessedArg(Option.PYLINT, ["aaa", "zzz"])]
     ),
     (
         [UnprocessedArg(Option.PYLINT, "zzz"), UnprocessedArg(Option.ENHANCEMENT, None)],
-        Config([ProcessedArg(Option.PYLINT, ["zzz", "aaa"]), ProcessedArg(Option.ENHANCEMENT, True)])
+        [ProcessedArg(Option.PYLINT, ["zzz", "aaa"]), ProcessedArg(Option.ENHANCEMENT, True)]
     ),
     (
         [UnprocessedArg(Option.FLAKE8, "zzz"), UnprocessedArg(Option.ENHANCEMENT, None)],
-        Config([
+        [
             ProcessedArg(Option.FLAKE8, ["zzz"]),
             ProcessedArg(Option.ENHANCEMENT, True),
             ProcessedArg(Option.PYLINT, ["aaa"])
-        ])
+        ]
     ),
     (
         [UnprocessedArg(Option.ALLOWED_ONECHAR_NAMES, "n")],
-        Config([ProcessedArg(Option.ALLOWED_ONECHAR_NAMES, "n"), ProcessedArg(Option.PYLINT, ["ccc"])])
+        [ProcessedArg(Option.ALLOWED_ONECHAR_NAMES, "n"), ProcessedArg(Option.PYLINT, ["ccc"])]
     ),
     (
         [UnprocessedArg(Option.IB111_WEEK, "02")],
-        Config([ProcessedArg(Option.IB111_WEEK, 2), ProcessedArg(Option.PYLINT, ["kkk"])])
+        [ProcessedArg(Option.IB111_WEEK, 2), ProcessedArg(Option.PYLINT, ["kkk"])]
     ),
     (
         [UnprocessedArg(Option.IB111_WEEK, "12"), UnprocessedArg(Option.IB111_WEEK, "02")],
-        Config([ProcessedArg(Option.IB111_WEEK, 2), ProcessedArg(Option.PYLINT, ["kkk"])])
+        [ProcessedArg(Option.IB111_WEEK, 2), ProcessedArg(Option.PYLINT, ["kkk"])]
     ),
     (
         [UnprocessedArg(Option.IB111_WEEK, "02"), UnprocessedArg(Option.PYLINT, "aaa")],
-        Config([ProcessedArg(Option.IB111_WEEK, 2), ProcessedArg(Option.PYLINT, ["aaa", "kkk"])])
+        [ProcessedArg(Option.IB111_WEEK, 2), ProcessedArg(Option.PYLINT, ["kkk", "aaa"])]
     ),
     (
         [UnprocessedArg(Option.IB111_WEEK, "02"), UnprocessedArg(Option.ENHANCEMENT, None)],
-        Config([
+        [
             ProcessedArg(Option.IB111_WEEK, 2),
             ProcessedArg(Option.ENHANCEMENT, True),
-            ProcessedArg(Option.PYLINT, ["aaa", "kkk"])
-        ])
+            ProcessedArg(Option.PYLINT, ["kkk", "aaa"])
+        ]
     ),
 ])
 def test_combine_and_translate_translates(
         args: List[UnprocessedArg],
         config_translations: Dict[Option, Translation],
         ib111_translations: List[Translation],
-        config: Config) -> None:
+        config: List[ProcessedArg]) -> None:
+
+    def fill_in_defaults(config: List[ProcessedArg], option_parses: Dict[Option, OptionParse]) -> List[ProcessedArg]:
+        result = [ProcessedArg(o, Config._to_immutable(option_parses[o].default)) for o in Option]
+        for arg in config:
+            result[int(arg.option)] = ProcessedArg(arg.option, Config._to_immutable(arg.val))
+        return tuple(result)
+
+    option_parses = get_option_parses()
+    result = Config(args, option_parses).to_immutable(config_translations, ib111_translations)
+    reference = fill_in_defaults(config, option_parses)
+    assert result.config == reference
+
+
+def _fill_in_file_config(config: Config) -> Config:
+    config_translations = get_config_translations()
+    ib111_translations = get_ib111_translations()
+
+    file_config = parse_config_file(
+        config.get_last_value(Option.CONFIG, use_default=True),
+        get_option_parses()
+    )
+    return Config.combine(file_config, config).to_immutable(config_translations, ib111_translations)
+
+
+def _arg_to_str(option: Option, val: Optional[str]) -> str:
+    if val is None:
+        return option.to_name()
+    return f"{option.to_name()}={val}"
+
+
+@pytest.mark.parametrize(
+    "filename,cmd,args",
+    [
+        ("custom_set_empty_config.py", [], [Arg(Option.CONFIG, "empty")]),
+        (
+            "custom_set_empty_config.py",
+            [_arg_to_str(Option.CONFIG, "default")],
+            [Arg(Option.CONFIG, "default")],
+        ),
+        (
+            "custom_set_empty_config.py",
+            [_arg_to_str(Option.IGNORE_INFILE_CONFIG_FOR, Linter.EDULINT.to_name())],
+            [Arg(Option.IGNORE_INFILE_CONFIG_FOR, "edulint"), Arg(Option.CONFIG, "default")]
+        ),
+        (
+            "custom_set_empty_config.py",
+            [_arg_to_str(Option.IGNORE_INFILE_CONFIG_FOR, "all")],
+            [Arg(Option.IGNORE_INFILE_CONFIG_FOR, "all"), Arg(Option.CONFIG, "default")]
+        ),
+        ("custom_set_ignore_infile_and_some.py", [], [Arg(Option.IGNORE_INFILE_CONFIG_FOR, "all")]),
+        ("custom_set_replace_option.py", [], [Arg(Option.IB111_WEEK, "1")]),
+        (
+            "custom_set_replace_option.py",
+            [_arg_to_str(Option.IB111_WEEK, "5")],
+            [Arg(Option.IB111_WEEK, "5")],
+        ),
+    ],
+)
+def test_get_config_one(filename: str, cmd: List[UnprocessedArg], args: List[UnprocessedArg]):
+    iconfig = _fill_in_file_config(Config(args))
+    assert get_config_one(get_tests_path(filename), cmd).config == iconfig.config
+
+
+@pytest.mark.parametrize("filenames,partition", [
+    (
+        [
+            Path("tests/data/custom_nonpep_assign.py"),
+            Path("tests/data/custom_flake8_pylint_config.py")
+        ],
+        [
+            ([Path("tests/data/custom_nonpep_assign.py")], Config()),
+            (
+                [Path("tests/data/custom_flake8_pylint_config.py")],
+                Config([Arg(Option.PYLINT, "--enable=missing-module-docstring")])
+            ),
+        ]
+    )
+])
+def test_get_config_many(filenames: List[str], partition: List[Tuple[List[str], Config]]):
+    configs = get_config_many(filenames, [])
+    assert len(configs) == len(partition)
+
+    for i in range(len(configs)):
+        fns1, iconfig1 = configs[i]
+        fns2, config2 = partition[i]
+
+        assert fns1 == fns2
 
-    result = combine_and_translate(args, get_option_parses(), config_translations, ib111_translations)
-    assert result.config == config.config
+        iconfig2 = _fill_in_file_config(config2)
+        assert iconfig1.config == iconfig2.config
```

### Comparing `edulint-2.8.0/tests/test_duplication.py` & `edulint-2.9.0/tests/test_duplication.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/tests/test_improper_loop.py` & `edulint-2.9.0/tests/test_improper_loop.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/tests/test_lint.py` & `edulint-2.9.0/tests/test_lint.py`

 * *Files 3% similar despite different names*

```diff
@@ -496,14 +496,45 @@
             filename,
             [Arg(Option.PYLINT, "--enable=use-early-return")],
             expected_output
         )
 
 
 @pytest.mark.parametrize("filename,args,expected_output", [
+    ("s2b8861_warehouse.py", [Arg(Option.IGNORE_INFILE_CONFIG_FOR, "flake8")], [
+        lazy_problem().set_line(2).set_text("Forbidden magic comment 'noqa'"),
+        lazy_problem().set_line(3).set_text("Forbidden magic comment 'noqa'"),
+    ]),
+    ("s2b8861_warehouse.py", [Arg(Option.IGNORE_INFILE_CONFIG_FOR, "all")], [
+        lazy_problem().set_line(2).set_text("Forbidden magic comment 'noqa'"),
+        lazy_problem().set_line(3).set_text("Forbidden magic comment 'noqa'"),
+    ]),
+    ("s2b8861_warehouse.py", [Arg(Option.IGNORE_INFILE_CONFIG_FOR, "pylint")], []),
+    ("014422-next-early-return-disabled.py", [Arg(Option.PYLINT, "--enable=use-early-return")], []),
+    (
+        "014422-next-early-return-disabled.py",
+        [Arg(Option.PYLINT, "--enable=use-early-return"), Arg(Option.IGNORE_INFILE_CONFIG_FOR, "pylint")],
+        [lazy_problem().set_line(19).set_text("Forbidden magic comment 'pylint: disable'")]
+    ),
+    (
+        "014422-next-early-return-disabled.py",
+        [Arg(Option.PYLINT, "--enable=use-early-return"), Arg(Option.IGNORE_INFILE_CONFIG_FOR, "flake8")],
+        []
+    ),
+    (
+        "014422-next-early-return-disabled.py",
+        [Arg(Option.PYLINT, "--enable=use-early-return"), Arg(Option.IGNORE_INFILE_CONFIG_FOR, "all")],
+        [lazy_problem().set_line(19).set_text("Forbidden magic comment 'pylint: disable'")]
+    ),
+])
+def test_ignore_infile_config(filename: str, args: List[Arg], expected_output: List[Problem]) -> None:
+    apply_and_lint(filename, args, expected_output)
+
+
+@pytest.mark.parametrize("filename,args,expected_output", [
     ("umime_count_a.py", [
         Arg(Option.PYTHON_SPECIFIC, "on"),
         Arg(Option.ALLOWED_ONECHAR_NAMES, ""),
         Arg(Option.ENHANCEMENT, "on"),
     ], [
         lazy_problem().set_code("C0104").set_line(2)
         .set_text("Disallowed single-character variable name \"a\", choose a more descriptive name"),
```

### Comparing `edulint-2.8.0/tests/test_main.py` & `edulint-2.9.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/tests/test_short_problems.py` & `edulint-2.9.0/tests/test_short_problems.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/tests/test_simplifiable_if.py` & `edulint-2.9.0/tests/test_simplifiable_if.py`

 * *Files identical despite different names*

### Comparing `edulint-2.8.0/tests/test_visitors.py` & `edulint-2.9.0/tests/test_visitors.py`

 * *Files identical despite different names*

