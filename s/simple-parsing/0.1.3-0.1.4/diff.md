# Comparing `tmp/simple_parsing-0.1.3.tar.gz` & `tmp/simple_parsing-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_parsing-0.1.3.tar", last modified: Tue Jun  6 21:40:02 2023, max compression
+gzip compressed data, was "simple_parsing-0.1.4.tar", last modified: Mon Aug  7 17:47:10 2023, max compression
```

## Comparing `simple_parsing-0.1.3.tar` & `simple_parsing-0.1.4.tar`

### file list

```diff
@@ -1,100 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/simple_parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/simple_parsing/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.568274 simple_parsing-0.1.3/simple_parsing/annotation_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/annotation_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/annotation_utils/get_field_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/conflicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/help_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.568274 simple_parsing-0.1.3/simple_parsing/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/custom_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/flatten.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.572275 simple_parsing-0.1.3/simple_parsing/helpers/hparams/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/hparam.py
--rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/hyperparameters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/priors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/hparams/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/nested_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/partial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.572275 simple_parsing-0.1.3/simple_parsing/helpers/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/serialization/decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/serialization/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    33185 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/serialization/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/serialization/yaml_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/helpers/subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/replace.py
--rw-r--r--   0 runner    (1001) docker     (123)    28879 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.572275 simple_parsing-0.1.3/simple_parsing/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/dataclass_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/field_metavar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/field_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    44574 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/field_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/simple_parsing/wrappers/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.568274 simple_parsing-0.1.3/simple_parsing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-06 21:40:02.000000 simple_parsing-0.1.3/simple_parsing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-06 21:40:02.000000 simple_parsing-0.1.3/simple_parsing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:40:02.000000 simple_parsing-0.1.3/simple_parsing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-06 21:40:02.000000 simple_parsing-0.1.3/simple_parsing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 21:40:02.000000 simple_parsing-0.1.3/simple_parsing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:40:02.576275 simple_parsing-0.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_bools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_custom_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_default_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_forward_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_future_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_generation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    61935 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_huggingface_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_initvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue64.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_107.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_132.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_144.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_46.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_48.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_issue_96.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_optional_subparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_optional_union.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_positional.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_set_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    28968 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_subparsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_suppress.py
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_tuples.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/test/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-06-06 21:39:38.000000 simple_parsing-0.1.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:47:10.246795 simple_parsing-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-08-07 17:47:10.246795 simple_parsing-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-07 17:47:10.246795 simple_parsing-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:47:10.246795 simple_parsing-0.1.4/simple_parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-07 17:47:10.246795 simple_parsing-0.1.4/simple_parsing/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:47:10.242795 simple_parsing-0.1.4/simple_parsing/annotation_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/annotation_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/annotation_utils/get_field_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/help_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:47:10.242795 simple_parsing-0.1.4/simple_parsing/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/custom_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/flatten.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:47:10.242795 simple_parsing-0.1.4/simple_parsing/helpers/hparams/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/hparams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/hparams/hparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/hparams/hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/hparams/hyperparameters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/hparams/priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/hparams/priors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/hparams/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/nested_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/partial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:47:10.242795 simple_parsing-0.1.4/simple_parsing/helpers/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/serialization/decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/serialization/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33185 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/serialization/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/serialization/yaml_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/helpers/subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49882 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28879 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:47:10.242795 simple_parsing-0.1.4/simple_parsing/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18969 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/wrappers/dataclass_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/wrappers/field_metavar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/wrappers/field_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44574 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/wrappers/field_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/simple_parsing/wrappers/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:47:10.242795 simple_parsing-0.1.4/simple_parsing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-08-07 17:47:10.000000 simple_parsing-0.1.4/simple_parsing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-08-07 17:47:10.000000 simple_parsing-0.1.4/simple_parsing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:47:10.000000 simple_parsing-0.1.4/simple_parsing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-07 17:47:10.000000 simple_parsing-0.1.4/simple_parsing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-07 17:47:10.000000 simple_parsing-0.1.4/simple_parsing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:47:10.246795 simple_parsing-0.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_bools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_custom_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_default_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_forward_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_future_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_generation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61935 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_huggingface_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_initvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_issue64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_issue_107.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_issue_132.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_issue_144.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_issue_46.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_issue_48.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_issue_96.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_optional_subparsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_optional_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_positional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_replace_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_set_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28968 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_subparsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_suppress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/test/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-08-07 17:46:49.000000 simple_parsing-0.1.4/versioneer.py
```

### Comparing `simple_parsing-0.1.3/LICENSE` & `simple_parsing-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/PKG-INFO` & `simple_parsing-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_parsing
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small utility for simplifying and cleaning up argument parsing scripts.
 Home-page: https://github.com/lebrice/SimpleParsing
 Author: Fabrice Normandin
 Author-email: fabrice.normandin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_parsing-0.1.3/README.md` & `simple_parsing-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/setup.py` & `simple_parsing-0.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,17 @@
     install_requires = req_file.read().splitlines(keepends=False)
 
 extras_require: dict[str, list[str]] = {
     "test": [
         "pytest",
         "pytest-xdist",
         "pytest-regressions",
+        "pytest-benchmark",
         "numpy",
-        "torch",
+        # "torch",
     ],
     "yaml": ["pyyaml"],
 }
 extras_require["all"] = list(set(sum(extras_require.values(), [])))
 
 
 setuptools.setup(
```

### Comparing `simple_parsing-0.1.3/simple_parsing/__init__.py` & `simple_parsing-0.1.4/simple_parsing/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ArgumentParser,
     DashVariant,
     NestedMode,
     ParsingError,
     parse,
     parse_known_args,
 )
-from .replace import replace
+from .replace import replace, replace_subgroups
 from .utils import InconsistentArgumentError
 
 __all__ = [
     "ArgumentGenerationMode",
     "ArgumentParser",
     "choice",
     "config_for",
@@ -45,14 +45,15 @@
     "mutable_field",
     "NestedMode",
     "parse_known_args",
     "parse",
     "ParsingError",
     "Partial",
     "replace",
+    "replace_subgroups",
     "Serializable",
     "SimpleHelpFormatter",
     "subgroups",
     "subparsers",
     "utils",
     "wrappers",
 ]
```

### Comparing `simple_parsing-0.1.3/simple_parsing/annotation_utils/get_field_annotations.py` & `simple_parsing-0.1.4/simple_parsing/annotation_utils/get_field_annotations.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/conflicts.py` & `simple_parsing-0.1.4/simple_parsing/conflicts.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 def unflatten(possibly_related_wrappers: list[DataclassWrapper]) -> list[DataclassWrapper]:
     return [wrapper for wrapper in possibly_related_wrappers if wrapper.parent is None]
 
 
 class ConflictResolver:
     def __init__(self, conflict_resolution=ConflictResolution.AUTO):
         self.conflict_resolution = conflict_resolution
+        self.max_attempts = 50
 
     def resolve_and_flatten(self, wrappers: list[DataclassWrapper]) -> list[DataclassWrapper]:
         """Given the list of all dataclass wrappers, find and resolve any conflicts between fields.
 
         Returns the new list of (possibly mutated in-place) dataclass wrappers.
         This returned list is flattened, i.e. it contains all the dataclass wrappers and their
         children.
@@ -78,15 +79,15 @@
 
         dests = [w.dest for w in wrappers_flat]
         assert len(dests) == len(set(dests)), f"shouldn't be any duplicates: {wrappers_flat}"
 
         conflict = self.get_conflict(wrappers_flat)
 
         # current and maximum number of attempts. When reached, raises an error.
-        cur_attempts, max_attempts = 0, 50
+        cur_attempts = 0
         while conflict:
             message: str = (
                 "The following wrappers are in conflict, as they share the "
                 + f"'{conflict.option_string}' option string:"
                 + ("\n".join(str(w) for w in conflict.wrappers))
                 + f"(Conflict Resolution mode is {self.conflict_resolution})"
             )
@@ -102,17 +103,17 @@
                 wrappers_flat = self._fix_conflict_merge(conflict, wrappers_flat)
 
             elif self.conflict_resolution == ConflictResolution.AUTO:
                 self._fix_conflict_auto(conflict)
 
             conflict = self.get_conflict(wrappers_flat)
             cur_attempts += 1
-            if cur_attempts == max_attempts:
+            if cur_attempts == self.max_attempts:
                 raise ConflictResolutionError(
-                    f"Reached maximum number of attempts ({max_attempts}) "
+                    f"Reached maximum number of attempts ({self.max_attempts}) "
                     "while trying to solve the conflicting argument names. "
                     "This is either a bug, or there is something weird going "
                     "on with your class hierarchy/argument names... \n"
                     "In any case, Please help us by submitting an issue on "
                     "the Github repo at "
                     "https://github.com/lebrice/SimpleParsing/issues, "
                     "or by using the following link: "
```

### Comparing `simple_parsing-0.1.3/simple_parsing/decorators.py` & `simple_parsing-0.1.4/simple_parsing/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import dataclasses
 import functools
 import inspect
 import typing
 from typing import Any, Callable, NamedTuple
 
 import docstring_parser as dp
-
+from simple_parsing.docstring import dp_parse, inspect_getdoc
 from . import helpers, parsing
 
 
 class _Field(NamedTuple):
     name: str
     annotation: type
     field: dataclasses.Field
@@ -51,15 +51,15 @@
         @functools.wraps(function)
         def _wrapper(*other_args, **other_kwargs) -> Any:
             # Parse signature and parameters
             signature = inspect.signature(function, follow_wrapped=True)
             parameters = signature.parameters
 
             # Parse docstring to use as help strings
-            docstring = dp.parse(inspect.getdoc(function) or "")
+            docstring = dp_parse(inspect_getdoc(function) or "")
             docstring_param_description = {
                 param.arg_name: param.description for param in docstring.params
             }
 
             # Parse all arguments from the function
             fields = []
             for name, parameter in parameters.items():
```

### Comparing `simple_parsing-0.1.3/simple_parsing/docstring.py` & `simple_parsing-0.1.4/simple_parsing/docstring.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """Utility for retrieveing the docstring of a dataclass's attributes
 @author: Fabrice Normandin
 """
 from __future__ import annotations
 
 import functools
 import inspect
+
+# from inspect import
 from dataclasses import dataclass
 from logging import getLogger
 
 import docstring_parser as dp
 from docstring_parser.common import Docstring
 
+dp_parse = functools.lru_cache(2048)(dp.parse)
+inspect_getsource = functools.lru_cache(2048)(inspect.getsource)
+inspect_getdoc = functools.lru_cache(2048)(inspect.getdoc)
 logger = getLogger(__name__)
 
 
 @dataclass
 class AttributeDocString:
     """Simple dataclass for holding the comments of a given field."""
 
@@ -98,29 +103,29 @@
 
 @functools.lru_cache(2048)
 def _get_attribute_docstring(dataclass: type, field_name: str) -> AttributeDocString | None:
     """Gets the AttributeDocString of the given field in the given dataclass.
     Doesn't inspect base classes.
     """
     try:
-        source = inspect.getsource(dataclass)
+        source = inspect_getsource(dataclass)
     except (TypeError, OSError) as e:
         logger.debug(
             UserWarning(
                 f"Couldn't retrieve the source code of class {dataclass} "
                 f"(in order to retrieve the docstring of field {field_name}): {e}"
             )
         )
         return None
 
     # Parse docstring to use as help strings
     desc_from_cls_docstring = ""
-    cls_docstring = inspect.getdoc(dataclass)
+    cls_docstring = inspect_getdoc(dataclass)
     if cls_docstring:
-        docstring: Docstring = dp.parse(cls_docstring)
+        docstring: Docstring = dp_parse(cls_docstring)
         for param in docstring.params:
             if param.arg_name == field_name:
                 desc_from_cls_docstring = param.description or ""
 
     # NOTE: We want to skip the docstring lines.
     # NOTE: Currently, we just remove the __doc__ from the source. It's perhaps a bit crude,
     # but it works.
```

### Comparing `simple_parsing-0.1.3/simple_parsing/help_formatter.py` & `simple_parsing-0.1.4/simple_parsing/help_formatter.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/custom_actions.py` & `simple_parsing-0.1.4/simple_parsing/helpers/custom_actions.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/fields.py` & `simple_parsing-0.1.4/simple_parsing/helpers/fields.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/flatten.py` & `simple_parsing-0.1.4/simple_parsing/helpers/flatten.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/hparams/hparam.py` & `simple_parsing-0.1.4/simple_parsing/helpers/hparams/hparam.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/hparams/hyperparameters.py` & `simple_parsing-0.1.4/simple_parsing/helpers/hparams/hyperparameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,40 @@
+from __future__ import annotations
 import dataclasses
 import inspect
 import math
 import pickle
 import random
 from collections import OrderedDict
 from dataclasses import Field, dataclass, fields
 from functools import singledispatch, total_ordering
 from logging import getLogger
 from pathlib import Path
 from typing import Any, ClassVar, Dict, List, NamedTuple, Optional, Tuple, Type, TypeVar
+import typing
 
 from simple_parsing import utils
 from simple_parsing.helpers.serialization.serializable import Serializable
 from simple_parsing.utils import (
     compute_identity,
     dict_union,
     field_dict,
     get_type_arguments,
 )
 
 from .hparam import ValueOutsidePriorException
 from .priors import Prior
 
+if typing.TYPE_CHECKING:
+    import numpy
+
 logger = getLogger(__name__)
 T = TypeVar("T")
 HP = TypeVar("HP", bound="HyperParameters")
 
-numpy_installed = False
-try:
-    import numpy as np
-
-    numpy_installed = True
-except ImportError:
-    pass
-
 
 @dataclass
 class BoundInfo(Serializable):
     """Object used to provide the bounds as required by `GPyOpt`."""
 
     name: str
     # One of 'continuous', 'discrete' or 'bandit' (unsupported).
@@ -47,18 +44,16 @@
 
 @dataclass
 class HyperParameters(Serializable, decode_into_subclasses=True):  # type: ignore
     """Base class for dataclasses of HyperParameters."""
 
     # Class variable holding the random number generator used to create the
     # samples.
-    if numpy_installed:
-        np_rng: ClassVar[np.random.RandomState] = np.random
-    else:
-        rng: ClassVar[random.Random] = random.Random()
+
+    rng: ClassVar[random.Random] = random.Random()
 
     def __post_init__(self):
         for name, f in field_dict(self).items():
             f: Field
             assert name == f.name
             value = getattr(self, name)
             # Apply any post-processing function, if applicable.
@@ -137,16 +132,15 @@
     def space_id(cls):
         return compute_identity(**cls.get_orion_space_dict())
 
     @classmethod
     def get_bounds(cls) -> List[BoundInfo]:
         """Returns the bounds of the search domain for this type of HParam.
 
-        Returns them as a list of `BoundInfo` objects, in the format expected by
-        GPyOpt.
+        Returns them as a list of `BoundInfo` objects, in the format expected by GPyOpt.
         """
         bounds: List[BoundInfo] = []
         for f in fields(cls):
             # TODO: handle a hparam which is categorical (i.e. choices)
             min_v = f.metadata.get("min")
             max_v = f.metadata.get("max")
             if min_v is None or max_v is None:
@@ -158,17 +152,16 @@
             else:
                 raise NotImplementedError(f"Unsupported type for field {f.name}: {f.type}")
             bounds.append(bound)
         return bounds
 
     @classmethod
     def get_bounds_dicts(cls) -> List[Dict[str, Any]]:
-        """Returns the bounds of the search space for this type of HParam,
-        in the format expected by the `GPyOpt` package.
-        """
+        """Returns the bounds of the search space for this type of HParam, in the format expected
+        by the `GPyOpt` package."""
         return [b.to_dict() for b in cls.get_bounds()]
 
     @classmethod
     def sample(cls):
         kwargs: Dict[str, Any] = {}
         for field in dataclasses.fields(cls):
             if inspect.isclass(field.type) and issubclass(field.type, HyperParameters):
@@ -182,67 +175,72 @@
                 chosen_class = random.choice(get_type_arguments(field.type))
                 # BUG: Seems to be a bit of a bug here, when the numpy rng is set!
                 value = chosen_class.sample()
                 kwargs[field.name] = value
             else:
                 prior: Optional[Prior] = field.metadata.get("prior")
                 if prior is not None:
-                    if numpy_installed:
-                        prior.np_rng = cls.np_rng
-                    else:
+                    try:
+                        import numpy as np
+
+                        prior.np_rng = np.random
+                    except ImportError:
                         prior.rng = cls.rng
                     value = prior.sample()
                     shape = getattr(prior, "shape", None)
-                    if numpy_installed and isinstance(value, np.ndarray) and not shape:
+                    if shape == () and hasattr(value, "item") and callable(value.item):
                         value = value.item()
                     kwargs[field.name] = value
         return cls(**kwargs)
 
     def replace(self, **new_params):
         new_hp_dict = dict_union(self.to_dict(), new_params, recurse=True)
         new_hp = type(self).from_dict(new_hp_dict)
         return new_hp
 
-    # @classmethod
-    # @contextmanager
-    # def use_priors(cls, value: bool = True):
-    #     temp = cls.sample_from_priors
-    #     cls.sample_from_priors = value
-    #     yield
-    #     cls.sample_from_priors = temp
-
-    if numpy_installed:
-
-        def to_array(self, dtype=np.float32) -> np.ndarray:
-            values: List[float] = []
-            for k, v in self.to_dict(dict_factory=OrderedDict).items():
-                try:
-                    v = float(v)
-                except Exception:
-                    logger.warning(f"Ignoring field {k} because we can't make a float out of it.")
-                else:
-                    values.append(v)
-            return np.array(values, dtype=dtype)
-
-        @classmethod
-        def from_array(cls: Type[HP], array: np.ndarray) -> HP:
-            if len(array.shape) == 2 and array.shape[0] == 1:
-                array = array[0]
-
-            keys = list(field_dict(cls))
-            # idea: could use to_dict and to_array together to determine how many
-            # values to get for each field. For now we assume that each field is one
-            # variable.
-            # cls.sample().to_dict()
-            # assert len(keys) == len(array), "assuming that each field is dim 1 for now."
-            assert len(keys) == len(array), "assuming that each field is dim 1 for now."
-            d = OrderedDict(zip(keys, array))
-            logger.debug(f"Creating an instance of {cls} using args {d}")
-            d = OrderedDict((k, v.item() if isinstance(v, np.ndarray) else v) for k, v in d.items())
-            return cls.from_dict(d)
+        # @classmethod
+        # @contextmanager
+        # def use_priors(cls, value: bool = True):
+        #     temp = cls.sample_from_priors
+        #     cls.sample_from_priors = value
+        #     yield
+        #     cls.sample_from_priors = temp
+
+    def to_array(self, dtype: numpy.dtype | None = None) -> numpy.ndarray:
+        import numpy as np
+
+        dtype = np.float32 if dtype is None else dtype
+        values: List[float] = []
+        for k, v in self.to_dict(dict_factory=OrderedDict).items():
+            try:
+                v = float(v)
+            except Exception:
+                logger.warning(f"Ignoring field {k} because we can't make a float out of it.")
+            else:
+                values.append(v)
+        return np.array(values, dtype=dtype)
+
+    @classmethod
+    def from_array(cls: Type[HP], array: numpy.ndarray) -> HP:
+        import numpy as np
+
+        if len(array.shape) == 2 and array.shape[0] == 1:
+            array = array[0]
+
+        keys = list(field_dict(cls))
+        # idea: could use to_dict and to_array together to determine how many
+        # values to get for each field. For now we assume that each field is one
+        # variable.
+        # cls.sample().to_dict()
+        # assert len(keys) == len(array), "assuming that each field is dim 1 for now."
+        assert len(keys) == len(array), "assuming that each field is dim 1 for now."
+        d = OrderedDict(zip(keys, array))
+        logger.debug(f"Creating an instance of {cls} using args {d}")
+        d = OrderedDict((k, v.item() if isinstance(v, np.ndarray) else v) for k, v in d.items())
+        return cls.from_dict(d)
 
     def clip_within_bounds(self: HP) -> HP:
         d = self.to_dict()
         for bound in self.get_bounds():
             min_v, max_v = bound.domain
             d[bound.name] = min(max_v, max(min_v, d[bound.name]))
         return self.from_dict(d)
```

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/hparams/hyperparameters_test.py` & `simple_parsing-0.1.4/simple_parsing/helpers/hparams/hyperparameters_test.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/hparams/priors.py` & `simple_parsing-0.1.4/simple_parsing/helpers/hparams/priors.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/hparams/priors_test.py` & `simple_parsing-0.1.4/simple_parsing/helpers/hparams/priors_test.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/nested_partial.py` & `simple_parsing-0.1.4/simple_parsing/helpers/nested_partial.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/partial.py` & `simple_parsing-0.1.4/simple_parsing/helpers/partial.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/serialization/decoding.py` & `simple_parsing-0.1.4/simple_parsing/helpers/serialization/decoding.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/serialization/encoding.py` & `simple_parsing-0.1.4/simple_parsing/helpers/serialization/encoding.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/serialization/serializable.py` & `simple_parsing-0.1.4/simple_parsing/helpers/serialization/serializable.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/serialization/yaml_serialization.py` & `simple_parsing-0.1.4/simple_parsing/helpers/serialization/yaml_serialization.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/helpers/subgroups.py` & `simple_parsing-0.1.4/simple_parsing/helpers/subgroups.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/parsing.py` & `simple_parsing-0.1.4/simple_parsing/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -972,14 +972,21 @@
         leftover_args = argparse.Namespace(**parsed_arg_values)
         if deleted_values:
             logger.debug(f"deleted values: {deleted_values}")
             logger.debug(f"leftover args: {leftover_args}")
 
         return leftover_args, constructor_arguments
 
+    @property
+    def confilct_resolver_max_attempts(self) -> int:
+        return self._conflict_resolver.max_attempts
+    
+    @confilct_resolver_max_attempts.setter
+    def confilct_resolver_max_attempts(self, value: int):
+        self._conflict_resolver.max_attempts = value
 
 # TODO: Change the order of arguments to put `args` as the second argument.
 def parse(
     config_class: type[DataclassT],
     config_path: Path | str | None = None,
     args: str | Sequence[str] | None = None,
     default: DataclassT | None = None,
```

### Comparing `simple_parsing-0.1.3/simple_parsing/utils.py` & `simple_parsing-0.1.4/simple_parsing/utils.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/wrappers/dataclass_wrapper.py` & `simple_parsing-0.1.4/simple_parsing/wrappers/dataclass_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import inspect
 import sys
 import textwrap
 from dataclasses import MISSING
 from logging import getLogger
 from typing import Any, Callable, Generic, TypeVar, cast
 
-import docstring_parser as dp
 from typing_extensions import Literal
 
-from .. import docstring, utils
-from ..utils import Dataclass, DataclassT, is_dataclass_instance, is_dataclass_type
-from .field_wrapper import FieldWrapper
-from .wrapper import Wrapper
+from simple_parsing import docstring, utils
+from simple_parsing.docstring import dp_parse, inspect_getdoc
+from simple_parsing.utils import Dataclass, DataclassT, is_dataclass_instance, is_dataclass_type
+from simple_parsing.wrappers.field_wrapper import FieldWrapper
+from simple_parsing.wrappers.wrapper import Wrapper
 
 logger = getLogger(__name__)
 
 MAX_DOCSTRING_DESC_LINES_HEIGHT: int = 50
 """
 Maximum number of lines of the class docstring to include in the autogenerated argument group
 description. If fields don't have docstrings or help text, then this is not used, and the entire
@@ -323,19 +323,19 @@
                 elif doc.comment_above:
                     return doc.comment_above
                 elif doc.comment_inline:
                     return doc.comment_inline
 
         # NOTE: The class docstring may be EXTRELEMY LARGE.
 
-        class_docstring = inspect.getdoc(self.dataclass) or ""
+        class_docstring = inspect_getdoc(self.dataclass) or ""
         if not class_docstring:
             return ""
 
-        doc = dp.parse(class_docstring)
+        doc = dp_parse(class_docstring)
 
         from simple_parsing.decorators import _description_from_docstring
 
         description = _description_from_docstring(doc)
 
         num_lines = len(description.splitlines())
         shortened_description = (
```

### Comparing `simple_parsing-0.1.3/simple_parsing/wrappers/field_metavar.py` & `simple_parsing-0.1.4/simple_parsing/wrappers/field_metavar.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/wrappers/field_parsing.py` & `simple_parsing-0.1.4/simple_parsing/wrappers/field_parsing.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/wrappers/field_wrapper.py` & `simple_parsing-0.1.4/simple_parsing/wrappers/field_wrapper.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing/wrappers/wrapper.py` & `simple_parsing-0.1.4/simple_parsing/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/simple_parsing.egg-info/PKG-INFO` & `simple_parsing-0.1.4/simple_parsing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-parsing
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small utility for simplifying and cleaning up argument parsing scripts.
 Home-page: https://github.com/lebrice/SimpleParsing
 Author: Fabrice Normandin
 Author-email: fabrice.normandin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_parsing-0.1.3/simple_parsing.egg-info/SOURCES.txt` & `simple_parsing-0.1.4/simple_parsing.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,18 @@
 test/test_issue_96.py
 test/test_lists.py
 test/test_literal.py
 test/test_multiple.py
 test/test_optional.py
 test/test_optional_subparsers.py
 test/test_optional_union.py
+test/test_performance.py
 test/test_positional.py
 test/test_replace.py
+test/test_replace_subgroups.py
 test/test_set_defaults.py
 test/test_subgroups.py
 test/test_subparsers.py
 test/test_suppress.py
 test/test_tuples.py
 test/test_union.py
 test/test_utils.py
```

### Comparing `simple_parsing-0.1.3/test/test_aliases.py` & `simple_parsing-0.1.4/test/test_aliases.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_base.py` & `simple_parsing-0.1.4/test/test_base.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_bools.py` & `simple_parsing-0.1.4/test/test_bools.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_choice.py` & `simple_parsing-0.1.4/test/test_choice.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_conflicts.py` & `simple_parsing-0.1.4/test/test_conflicts.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_custom_args.py` & `simple_parsing-0.1.4/test/test_custom_args.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_decoding.py` & `simple_parsing-0.1.4/test/test_decoding.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_decorator.py` & `simple_parsing-0.1.4/test/test_decorator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-"""Tests simple parsing decorators.
-"""
+"""Tests simple parsing decorators."""
 import collections
 import dataclasses
 import functools
-import inspect
 import sys
-import typing
 from typing import Callable
-
+import typing
+import inspect
 import pytest
 
 import simple_parsing as sp
 
 
 @dataclasses.dataclass
 class AddThreeNumbers:
@@ -39,15 +37,15 @@
     def pop(self, index, default_value=None):
         try:
             return super().pop(index)
         except IndexError:
             return default_value
 
 
-def partial(fn: Callable, *args, **kwargs) -> Callable:
+def change_defaults(fn: Callable, *args, **kwargs) -> Callable:
     """Partial via changing the signature defaults."""
 
     @functools.wraps(fn)
     def _wrapper(*other_args, **other_kwargs):
         return fn(*other_args, **other_kwargs)
 
     signature = inspect.signature(fn)
@@ -65,64 +63,75 @@
 
     signature = signature.replace(parameters=new_parameters)
     _wrapper.__signature__ = signature
 
     return _wrapper
 
 
+def _xfail_in_py311(*param):
+    return pytest.param(
+        *param,
+        marks=pytest.mark.xfail(
+            sys.version_info >= (3, 11),
+            reason="TODO: test doesn't work in Python 3.11",
+            raises=ValueError,  # "non-default argument follows default argument"
+            strict=True,
+        ),
+    )
+
+
 @pytest.mark.parametrize(
     "args, expected, fn",
     [
-        ("", 1, partial(_fn_with_positional_only, 1)),
-        ("2", 2, partial(_fn_with_positional_only, 1)),
-        ("2", 2, _fn_with_positional_only),
-        ("", 1, partial(_fn_with_keyword_only, x=1)),
-        ("--x=2", 2, partial(_fn_with_keyword_only, x=1)),
-        ("--x=2", 2, _fn_with_keyword_only),
-        ("", 3, partial(_fn_with_all_argument_types, 1, b=1, c=1)),
-        ("2", 4, partial(_fn_with_all_argument_types, b=1, c=1)),
-        ("2 --b=2", 5, partial(_fn_with_all_argument_types, c=1)),
-        ("2 --b=2 --c=2", 6, _fn_with_all_argument_types),
-        ("--c=2", 4, partial(_fn_with_all_argument_types, 1, b=1)),
-        ("--b=2", 4, partial(_fn_with_all_argument_types, 1, c=1)),
-        ("--b=2 --c=2", 5, partial(_fn_with_all_argument_types, 1)),
+        ("", 1, change_defaults(_fn_with_positional_only, 1)),
+        ("2", 2, change_defaults(_fn_with_positional_only, 1)),
+        ("2", 2, change_defaults(_fn_with_positional_only)),
+        ("", 1, change_defaults(_fn_with_keyword_only, x=1)),
+        ("--x=2", 2, change_defaults(_fn_with_keyword_only, x=1)),
+        ("--x=2", 2, change_defaults(_fn_with_keyword_only)),
+        ("", 3, change_defaults(_fn_with_all_argument_types, 1, b=1, c=1)),
+        ("2", 4, change_defaults(_fn_with_all_argument_types, b=1, c=1)),
+        ("2 --b=2", 5, change_defaults(_fn_with_all_argument_types, c=1)),
+        ("2 --b=2 --c=2", 6, change_defaults(_fn_with_all_argument_types)),
+        ("--c=2", 4, change_defaults(_fn_with_all_argument_types, 1, b=1)),
+        _xfail_in_py311(
+            "--b=2", 4, functools.partial(change_defaults, _fn_with_all_argument_types, 1, c=1)
+        ),
+        _xfail_in_py311(
+            "--b=2 --c=2", 5, functools.partial(change_defaults, _fn_with_all_argument_types, 1)
+        ),
     ],
 )
 def test_simple_arguments(
     args: str,
     expected: int,
     fn: Callable,
 ):
+    if isinstance(fn, functools.partial):
+        # In Python 3.11.4, the inspect module had a backward-incompatible change. We need to have
+        # this additional level of indirection.
+        fn = fn()
     decorated = sp.decorators.main(fn, args=args)
     assert decorated() == expected
 
 
 def _fn_with_nested_dataclass(x: int, /, *, data: AddThreeNumbers) -> int:
     return x + data()
 
 
-def _xfail_in_py311(*param):
-    return pytest.param(
-        *param,
-        marks=pytest.mark.xfail(
-            sys.version_info >= (3, 11),
-            reason="TODO: test doesn't work in Python 3.11",
-            strict=True,
-        ),
-    )
-
-
 @pytest.mark.parametrize(
-    "args, expected, fn",
+    ("args", "expected", "fn"),
     [
-        _xfail_in_py311("", 1, partial(_fn_with_nested_dataclass, 1, data=AddThreeNumbers())),
-        ("--a=1", 2, partial(_fn_with_nested_dataclass, 1)),
-        ("--a=1 --b=1", 3, partial(_fn_with_nested_dataclass, 1)),
-        ("--a=1 --b=1 --c=1", 4, partial(_fn_with_nested_dataclass, 1)),
-        ("2 --a=1 --b=1 --c=1", 5, partial(_fn_with_nested_dataclass)),
+        _xfail_in_py311(
+            "", 1, change_defaults(_fn_with_nested_dataclass, 1, data=AddThreeNumbers())
+        ),
+        ("--a=1", 2, change_defaults(_fn_with_nested_dataclass, 1)),
+        ("--a=1 --b=1", 3, change_defaults(_fn_with_nested_dataclass, 1)),
+        ("--a=1 --b=1 --c=1", 4, change_defaults(_fn_with_nested_dataclass, 1)),
+        ("2 --a=1 --b=1 --c=1", 5, change_defaults(_fn_with_nested_dataclass)),
     ],
 )
 def test_nested_dataclass(
     args: str,
     expected: int,
     fn: Callable,
 ):
```

### Comparing `simple_parsing-0.1.3/test/test_default_args.py` & `simple_parsing-0.1.4/test/test_default_args.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_docstrings.py` & `simple_parsing-0.1.4/test/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_examples.py` & `simple_parsing-0.1.4/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_fields.py` & `simple_parsing-0.1.4/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_forward_ref.py` & `simple_parsing-0.1.4/test/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_future_annotations.py` & `simple_parsing-0.1.4/test/test_future_annotations.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_generation_mode.py` & `simple_parsing-0.1.4/test/test_generation_mode.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_huggingface_compat.py` & `simple_parsing-0.1.4/test/test_huggingface_compat.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_inheritance.py` & `simple_parsing-0.1.4/test/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_initvar.py` & `simple_parsing-0.1.4/test/test_initvar.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_issue64.py` & `simple_parsing-0.1.4/test/test_issue64.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_issue_107.py` & `simple_parsing-0.1.4/test/test_issue_107.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_issue_132.py` & `simple_parsing-0.1.4/test/test_issue_132.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_issue_144.py` & `simple_parsing-0.1.4/test/test_issue_144.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_issue_46.py` & `simple_parsing-0.1.4/test/test_issue_46.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_issue_48.py` & `simple_parsing-0.1.4/test/test_issue_48.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_issue_96.py` & `simple_parsing-0.1.4/test/test_issue_96.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_lists.py` & `simple_parsing-0.1.4/test/test_lists.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_literal.py` & `simple_parsing-0.1.4/test/test_literal.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_multiple.py` & `simple_parsing-0.1.4/test/test_multiple.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_optional.py` & `simple_parsing-0.1.4/test/test_optional.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_optional_subparsers.py` & `simple_parsing-0.1.4/test/test_optional_subparsers.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_positional.py` & `simple_parsing-0.1.4/test/test_positional.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_replace.py` & `simple_parsing-0.1.4/test/test_replace.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_set_defaults.py` & `simple_parsing-0.1.4/test/test_set_defaults.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_subgroups.py` & `simple_parsing-0.1.4/test/test_subgroups.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_subparsers.py` & `simple_parsing-0.1.4/test/test_subparsers.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_suppress.py` & `simple_parsing-0.1.4/test/test_suppress.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_tuples.py` & `simple_parsing-0.1.4/test/test_tuples.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_union.py` & `simple_parsing-0.1.4/test/test_union.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/test_utils.py` & `simple_parsing-0.1.4/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/test/testutils.py` & `simple_parsing-0.1.4/test/testutils.py`

 * *Files identical despite different names*

### Comparing `simple_parsing-0.1.3/versioneer.py` & `simple_parsing-0.1.4/versioneer.py`

 * *Files identical despite different names*

