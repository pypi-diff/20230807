# Comparing `tmp/bluepymm-0.9.4.tar.gz` & `tmp/bluepymm-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepymm-0.9.4.tar", last modified: Fri Jul 14 12:25:58 2023, max compression
+gzip compressed data, was "bluepymm-0.9.5.tar", last modified: Mon Aug  7 11:59:53 2023, max compression
```

## Comparing `bluepymm-0.9.4.tar` & `bluepymm-0.9.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:58.831632 bluepymm-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-14 12:25:51.000000 bluepymm-0.9.4/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35151 2023-07-14 12:25:51.000000 bluepymm-0.9.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-14 12:25:51.000000 bluepymm-0.9.4/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-14 12:25:51.000000 bluepymm-0.9.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 12:25:51.000000 bluepymm-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-14 12:25:58.831632 bluepymm-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-14 12:25:51.000000 bluepymm-0.9.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:58.831632 bluepymm-0.9.4/bluepymm/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 12:25:58.831632 bluepymm-0.9.4/bluepymm/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:58.823632 bluepymm-0.9.4/bluepymm/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/legacy/create_hoc_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:58.827632 bluepymm-0.9.4/bluepymm/prepare_combos/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/prepare_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16419 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/prepare_combos/create_mm_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/prepare_combos/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/prepare_combos/parse_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/prepare_combos/prepare_emodel_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:58.827632 bluepymm-0.9.4/bluepymm/run_combos/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/run_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/run_combos/calculate_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/run_combos/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:58.827632 bluepymm-0.9.4/bluepymm/select_combos/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/select_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/select_combos/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/select_combos/megate_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/select_combos/process_megate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/select_combos/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/select_combos/sqlite_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/select_combos/table_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:58.827632 bluepymm-0.9.4/bluepymm/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/templates/cell_template_neurodamus.jinja2
--rwxr-xr-x   0 runner    (1001) docker     (123)     4762 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/templates/cell_template_neuron.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:58.827632 bluepymm-0.9.4/bluepymm/validate_output/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/validate_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-14 12:25:51.000000 bluepymm-0.9.4/bluepymm/validate_output/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:58.823632 bluepymm-0.9.4/bluepymm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-14 12:25:58.000000 bluepymm-0.9.4/bluepymm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-14 12:25:58.000000 bluepymm-0.9.4/bluepymm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:25:58.000000 bluepymm-0.9.4/bluepymm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 12:25:58.000000 bluepymm-0.9.4/bluepymm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 12:25:58.000000 bluepymm-0.9.4/bluepymm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 12:25:58.000000 bluepymm-0.9.4/bluepymm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-14 12:25:58.831632 bluepymm-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-14 12:25:51.000000 bluepymm-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:58.831632 bluepymm-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_bluepymm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_calculate_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_create_mm_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_megate_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_parse_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_prepare_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_prepare_emodel_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_process_megate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_run_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_select_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_sqlite_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_table_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-14 12:25:51.000000 bluepymm-0.9.4/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-07-14 12:25:51.000000 bluepymm-0.9.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:59:53.747315 bluepymm-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-07 11:59:48.000000 bluepymm-0.9.5/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35151 2023-08-07 11:59:48.000000 bluepymm-0.9.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-08-07 11:59:48.000000 bluepymm-0.9.5/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-07 11:59:48.000000 bluepymm-0.9.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-07 11:59:48.000000 bluepymm-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-07 11:59:53.747315 bluepymm-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-08-07 11:59:48.000000 bluepymm-0.9.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:59:53.747315 bluepymm-0.9.5/bluepymm/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-07 11:59:53.747315 bluepymm-0.9.5/bluepymm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:59:53.735315 bluepymm-0.9.5/bluepymm/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/legacy/create_hoc_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:59:53.739315 bluepymm-0.9.5/bluepymm/prepare_combos/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/prepare_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16419 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/prepare_combos/create_mm_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/prepare_combos/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/prepare_combos/parse_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/prepare_combos/prepare_emodel_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:59:53.739315 bluepymm-0.9.5/bluepymm/run_combos/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/run_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/run_combos/calculate_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/run_combos/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:59:53.743315 bluepymm-0.9.5/bluepymm/select_combos/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/select_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/select_combos/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/select_combos/megate_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/select_combos/process_megate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/select_combos/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/select_combos/sqlite_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/select_combos/table_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:59:53.743315 bluepymm-0.9.5/bluepymm/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/templates/cell_template_neurodamus.jinja2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4762 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/templates/cell_template_neuron.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:59:53.743315 bluepymm-0.9.5/bluepymm/validate_output/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/validate_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-08-07 11:59:48.000000 bluepymm-0.9.5/bluepymm/validate_output/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:59:53.735315 bluepymm-0.9.5/bluepymm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-07 11:59:53.000000 bluepymm-0.9.5/bluepymm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-07 11:59:53.000000 bluepymm-0.9.5/bluepymm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 11:59:53.000000 bluepymm-0.9.5/bluepymm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-07 11:59:53.000000 bluepymm-0.9.5/bluepymm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 11:59:53.000000 bluepymm-0.9.5/bluepymm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-07 11:59:53.000000 bluepymm-0.9.5/bluepymm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-07 11:59:53.747315 bluepymm-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-07 11:59:48.000000 bluepymm-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 11:59:53.747315 bluepymm-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_bluepymm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_calculate_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_create_mm_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_megate_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_parse_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_prepare_combos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_prepare_emodel_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_process_megate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_run_combos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_select_combos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_sqlite_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_table_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-08-07 11:59:48.000000 bluepymm-0.9.5/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-08-07 11:59:48.000000 bluepymm-0.9.5/versioneer.py
```

### Comparing `bluepymm-0.9.4/COPYING` & `bluepymm-0.9.5/COPYING`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/COPYING.lesser` & `bluepymm-0.9.5/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/LICENSE.txt` & `bluepymm-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/PKG-INFO` & `bluepymm-0.9.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepymm
-Version: 0.9.4
+Version: 0.9.5
 Summary: Model Management Python Library (bluepymm)
 Home-page: https://github.com/BlueBrain/BluePyMM
 Author: BlueBrain Project, EPFL
 Author-email: werner.vangeit@epfl.ch
 Keywords: optimisation,neuroscience,BlueBrainProject
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `bluepymm-0.9.4/README.rst` & `bluepymm-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/__init__.py` & `bluepymm-0.9.5/bluepymm/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/legacy/__init__.py` & `bluepymm-0.9.5/bluepymm/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/legacy/create_hoc_files.py` & `bluepymm-0.9.5/bluepymm/legacy/create_hoc_files.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/main.py` & `bluepymm-0.9.5/bluepymm/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/prepare_combos/__init__.py` & `bluepymm-0.9.5/bluepymm/prepare_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/prepare_combos/create_mm_sqlite.py` & `bluepymm-0.9.5/bluepymm/prepare_combos/create_mm_sqlite.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/prepare_combos/main.py` & `bluepymm-0.9.5/bluepymm/prepare_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/prepare_combos/parse_files.py` & `bluepymm-0.9.5/bluepymm/prepare_combos/parse_files.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/prepare_combos/prepare_emodel_dirs.py` & `bluepymm-0.9.5/bluepymm/prepare_combos/prepare_emodel_dirs.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/run_combos/__init__.py` & `bluepymm-0.9.5/bluepymm/run_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/run_combos/calculate_scores.py` & `bluepymm-0.9.5/bluepymm/run_combos/calculate_scores.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/run_combos/main.py` & `bluepymm-0.9.5/bluepymm/run_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/select_combos/__init__.py` & `bluepymm-0.9.5/bluepymm/select_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/select_combos/main.py` & `bluepymm-0.9.5/bluepymm/select_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/select_combos/megate_output.py` & `bluepymm-0.9.5/bluepymm/select_combos/megate_output.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/select_combos/process_megate_config.py` & `bluepymm-0.9.5/bluepymm/select_combos/process_megate_config.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/select_combos/reporting.py` & `bluepymm-0.9.5/bluepymm/select_combos/reporting.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/select_combos/sqlite_io.py` & `bluepymm-0.9.5/bluepymm/select_combos/sqlite_io.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/select_combos/table_processing.py` & `bluepymm-0.9.5/bluepymm/select_combos/table_processing.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/templates/cell_template_neurodamus.jinja2` & `bluepymm-0.9.5/bluepymm/templates/cell_template_neurodamus.jinja2`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/templates/cell_template_neuron.jinja2` & `bluepymm-0.9.5/bluepymm/templates/cell_template_neuron.jinja2`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/tools.py` & `bluepymm-0.9.5/bluepymm/tools.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm/validate_output/main.py` & `bluepymm-0.9.5/bluepymm/validate_output/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/bluepymm.egg-info/PKG-INFO` & `bluepymm-0.9.5/bluepymm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepymm
-Version: 0.9.4
+Version: 0.9.5
 Summary: Model Management Python Library (bluepymm)
 Home-page: https://github.com/BlueBrain/BluePyMM
 Author: BlueBrain Project, EPFL
 Author-email: werner.vangeit@epfl.ch
 Keywords: optimisation,neuroscience,BlueBrainProject
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `bluepymm-0.9.4/bluepymm.egg-info/SOURCES.txt` & `bluepymm-0.9.5/bluepymm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/setup.py` & `bluepymm-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_bluepymm.py` & `bluepymm-0.9.5/tests/test_bluepymm.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_calculate_scores.py` & `bluepymm-0.9.5/tests/test_calculate_scores.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_create_mm_sqlite.py` & `bluepymm-0.9.5/tests/test_create_mm_sqlite.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_legacy.py` & `bluepymm-0.9.5/tests/test_legacy.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_main.py` & `bluepymm-0.9.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_megate_output.py` & `bluepymm-0.9.5/tests/test_megate_output.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_parse_files.py` & `bluepymm-0.9.5/tests/test_parse_files.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_prepare_combos.py` & `bluepymm-0.9.5/tests/test_prepare_combos.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_prepare_emodel_dirs.py` & `bluepymm-0.9.5/tests/test_prepare_emodel_dirs.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_process_megate_config.py` & `bluepymm-0.9.5/tests/test_process_megate_config.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_reporting.py` & `bluepymm-0.9.5/tests/test_reporting.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_run_combos.py` & `bluepymm-0.9.5/tests/test_run_combos.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_select_combos.py` & `bluepymm-0.9.5/tests/test_select_combos.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_sqlite_io.py` & `bluepymm-0.9.5/tests/test_sqlite_io.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_table_processing.py` & `bluepymm-0.9.5/tests/test_table_processing.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/tests/test_tools.py` & `bluepymm-0.9.5/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.4/versioneer.py` & `bluepymm-0.9.5/versioneer.py`

 * *Files identical despite different names*

