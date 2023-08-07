# Comparing `tmp/brain_pipe-0.0.1.tar.gz` & `tmp/brain_pipe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brain_pipe-0.0.1.tar", last modified: Tue Jul 25 21:49:40 2023, max compression
+gzip compressed data, was "brain_pipe-0.0.2.tar", last modified: Mon Aug  7 15:48:37 2023, max compression
```

## Comparing `brain_pipe-0.0.1.tar` & `brain_pipe-0.0.2.tar`

### file list

```diff
@@ -1,159 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.391919 brain_pipe-0.0.1/brain_pipe/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.391919 brain_pipe-0.0.1/brain_pipe/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/cli/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.391919 brain_pipe-0.0.1/brain_pipe/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/dataloaders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/dataloaders/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.395919 brain_pipe-0.0.1/brain_pipe/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/parser/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/parser/simple_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/parser/template_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/parser/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/parser/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.395919 brain_pipe-0.0.1/brain_pipe/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/pipeline/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.395919 brain_pipe-0.0.1/brain_pipe/pipeline/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/pipeline/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/pipeline/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/pipeline/cache/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/pipeline/cache/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/pipeline/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/pipeline/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.395919 brain_pipe-0.0.1/brain_pipe/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.395919 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.395919 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/eeg/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/eeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/eeg/biosemi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/eeg/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/rereference.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/brain/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/resample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.395919 brain_pipe-0.0.1/brain_pipe/preprocessing/stimulus/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/stimulus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.395919 brain_pipe-0.0.1/brain_pipe/preprocessing/stimulus/audio/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/stimulus/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/stimulus/audio/envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/stimulus/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/preprocessing/transpose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.395919 brain_pipe-0.0.1/brain_pipe/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/runner/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.395919 brain_pipe-0.0.1/brain_pipe/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/save/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/save/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/brain_pipe/split/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/split/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/split/mid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/brain_pipe/split/operations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/split/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/split/operations/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/split/operations/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/split/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/brain_pipe/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/utils/find.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/utils/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/utils/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/brain_pipe/utils/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.391919 brain_pipe-0.0.1/brain_pipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-25 21:49:40.000000 brain_pipe-0.0.1/brain_pipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-25 21:49:40.000000 brain_pipe-0.0.1/brain_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:49:40.000000 brain_pipe-0.0.1/brain_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 21:49:40.000000 brain_pipe-0.0.1/brain_pipe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 21:49:40.000000 brain_pipe-0.0.1/brain_pipe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 21:49:40.000000 brain_pipe-0.0.1/brain_pipe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.391919 brain_pipe-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/examples/exporl/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/examples/exporl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/examples/exporl/sparrKULee.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_cli/test_cli_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_cli/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_cli/test_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/tests/test_dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_dataloaders/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_dataloaders/test_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/tests/test_examples/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/tests/test_examples/exporl/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_examples/exporl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_examples/exporl/test_auditory_eeg_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.399919 brain_pipe-0.0.1/tests/test_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_parser/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_parser/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_parser/test_simple_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_parser/test_template_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_parser/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_parser/test_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/tests/test_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_pipeline/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_pipeline/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_pipeline/test_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/tests/test_preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/tests/test_preprocessing/test_brain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_eeg/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_eeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_eeg/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_epochs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_rereference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_resample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/tests/test_preprocessing/test_stimulus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_stimulus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/tests/test_preprocessing/test_stimulus/test_audio/
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_stimulus/test_audio/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_stimulus/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_preprocessing/test_transpose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/tests/test_runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_runner/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_runner/test_runner_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/tests/test_save/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_save/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_save/test_default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:40.403919 brain_pipe-0.0.1/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-25 21:49:28.000000 brain_pipe-0.0.1/tests/test_utils/test_find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.008493 brain_pipe-0.0.2/brain_pipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.012493 brain_pipe-0.0.2/brain_pipe/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/cli/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.012493 brain_pipe-0.0.2/brain_pipe/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/dataloaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/dataloaders/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.012493 brain_pipe-0.0.2/brain_pipe/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/parser/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/parser/simple_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/parser/template_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/parser/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/parser/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.012493 brain_pipe-0.0.2/brain_pipe/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/pipeline/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.012493 brain_pipe-0.0.2/brain_pipe/pipeline/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/pipeline/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/pipeline/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/pipeline/cache/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/pipeline/cache/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/pipeline/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/pipeline/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.012493 brain_pipe-0.0.2/brain_pipe/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.012493 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.012493 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/eeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/eeg/biosemi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/eeg/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/rereference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/brain/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/resample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.012493 brain_pipe-0.0.2/brain_pipe/preprocessing/stimulus/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/stimulus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/brain_pipe/preprocessing/stimulus/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/stimulus/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/stimulus/audio/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/stimulus/audio/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/stimulus/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/preprocessing/transpose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/brain_pipe/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/runner/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/brain_pipe/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/save/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/save/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/brain_pipe/split/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/split/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/split/mid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/brain_pipe/split/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/split/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/split/operations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/split/operations/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/split/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/brain_pipe/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/utils/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/utils/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/utils/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/brain_pipe/utils/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.008493 brain_pipe-0.0.2/brain_pipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-07 15:48:36.000000 brain_pipe-0.0.2/brain_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-08-07 15:48:37.000000 brain_pipe-0.0.2/brain_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:48:36.000000 brain_pipe-0.0.2/brain_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 15:48:36.000000 brain_pipe-0.0.2/brain_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-07 15:48:36.000000 brain_pipe-0.0.2/brain_pipe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-07 15:48:36.000000 brain_pipe-0.0.2/brain_pipe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.008493 brain_pipe-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/examples/exporl/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/examples/exporl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16513 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/examples/exporl/sparrKULee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-07 15:48:37.024493 brain_pipe-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_cli/test_cli_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_cli/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_cli/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/tests/test_dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_dataloaders/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_dataloaders/test_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/tests/test_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.016493 brain_pipe-0.0.2/tests/test_examples/exporl/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_examples/exporl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_examples/exporl/sparrKULee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/tests/test_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_parser/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_parser/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_parser/test_simple_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_parser/test_template_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_parser/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_parser/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/tests/test_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_pipeline/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_pipeline/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_pipeline/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/tests/test_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/tests/test_preprocessing/test_brain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_eeg/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_eeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_eeg/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_epochs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_rereference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_resample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/tests/test_preprocessing/test_stimulus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_stimulus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/tests/test_preprocessing/test_stimulus/test_audio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_stimulus/test_audio/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_stimulus/test_audio/test_spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_stimulus/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_preprocessing/test_transpose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/tests/test_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_runner/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_runner/test_runner_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/tests/test_save/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_save/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_save/test_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:37.020493 brain_pipe-0.0.2/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-07 15:48:27.000000 brain_pipe-0.0.2/tests/test_utils/test_find.py
```

### Comparing `brain_pipe-0.0.1/LICENSE` & `brain_pipe-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/PKG-INFO` & `brain_pipe-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain_pipe
-Version: 0.0.1
+Version: 0.0.2
 Summary: Brain Pipe
 Keywords: Brain imaging processing,EEG,SparrKULee,BIDS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `brain_pipe-0.0.1/README.md` & `brain_pipe-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/cli/__init__.py` & `brain_pipe-0.0.2/brain_pipe/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/cli/base.py` & `brain_pipe-0.0.2/brain_pipe/cli/base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/cli/default.py` & `brain_pipe-0.0.2/brain_pipe/cli/default.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/dataloaders/base.py` & `brain_pipe-0.0.2/brain_pipe/dataloaders/base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/dataloaders/path.py` & `brain_pipe-0.0.2/brain_pipe/dataloaders/path.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/parser/base.py` & `brain_pipe-0.0.2/brain_pipe/parser/base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/parser/file.py` & `brain_pipe-0.0.2/brain_pipe/parser/file.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/parser/simple_dict.py` & `brain_pipe-0.0.2/brain_pipe/parser/simple_dict.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/parser/template_text.py` & `brain_pipe-0.0.2/brain_pipe/parser/template_text.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/parser/text.py` & `brain_pipe-0.0.2/brain_pipe/parser/text.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/parser/yaml.py` & `brain_pipe-0.0.2/brain_pipe/parser/yaml.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/pipeline/base.py` & `brain_pipe-0.0.2/brain_pipe/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/pipeline/cache/base.py` & `brain_pipe-0.0.2/brain_pipe/pipeline/cache/base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/pipeline/cache/default.py` & `brain_pipe-0.0.2/brain_pipe/pipeline/cache/default.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/pipeline/cache/pipeline.py` & `brain_pipe-0.0.2/brain_pipe/pipeline/cache/pipeline.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/pipeline/default.py` & `brain_pipe-0.0.2/brain_pipe/pipeline/default.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/pipeline/wrapper.py` & `brain_pipe-0.0.2/brain_pipe/pipeline/wrapper.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/brain/artifact.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/brain/artifact.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/brain/eeg/biosemi.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/brain/eeg/biosemi.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/brain/eeg/load.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/brain/eeg/load.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/brain/epochs.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/brain/epochs.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/brain/link.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/brain/link.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/brain/load.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/brain/load.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/brain/rereference.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/brain/rereference.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/brain/trigger.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/brain/trigger.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/filter.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/resample.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/resample.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/stimulus/audio/envelope.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/stimulus/audio/envelope.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/stimulus/load.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/stimulus/load.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/preprocessing/transpose.py` & `brain_pipe-0.0.2/brain_pipe/preprocessing/transpose.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/runner/base.py` & `brain_pipe-0.0.2/brain_pipe/runner/base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/runner/default.py` & `brain_pipe-0.0.2/brain_pipe/runner/default.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/save/base.py` & `brain_pipe-0.0.2/brain_pipe/save/base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/save/default.py` & `brain_pipe-0.0.2/brain_pipe/save/default.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/split/base.py` & `brain_pipe-0.0.2/brain_pipe/split/base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/split/mid.py` & `brain_pipe-0.0.2/brain_pipe/split/mid.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/split/operations/base.py` & `brain_pipe-0.0.2/brain_pipe/split/operations/base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/split/operations/normalize.py` & `brain_pipe-0.0.2/brain_pipe/split/operations/normalize.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/split/sequential.py` & `brain_pipe-0.0.2/brain_pipe/split/sequential.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/utils/find.py` & `brain_pipe-0.0.2/brain_pipe/utils/find.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/utils/log.py` & `brain_pipe-0.0.2/brain_pipe/utils/log.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/utils/multiprocess.py` & `brain_pipe-0.0.2/brain_pipe/utils/multiprocess.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/utils/path.py` & `brain_pipe-0.0.2/brain_pipe/utils/path.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe/utils/serialization.py` & `brain_pipe-0.0.2/brain_pipe/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/brain_pipe.egg-info/PKG-INFO` & `brain_pipe-0.0.2/brain_pipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-pipe
-Version: 0.0.1
+Version: 0.0.2
 Summary: Brain Pipe
 Keywords: Brain imaging processing,EEG,SparrKULee,BIDS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `brain_pipe-0.0.1/brain_pipe.egg-info/SOURCES.txt` & `brain_pipe-0.0.2/brain_pipe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 brain_pipe/preprocessing/brain/eeg/__init__.py
 brain_pipe/preprocessing/brain/eeg/biosemi.py
 brain_pipe/preprocessing/brain/eeg/load.py
 brain_pipe/preprocessing/stimulus/__init__.py
 brain_pipe/preprocessing/stimulus/load.py
 brain_pipe/preprocessing/stimulus/audio/__init__.py
 brain_pipe/preprocessing/stimulus/audio/envelope.py
+brain_pipe/preprocessing/stimulus/audio/spectrogram.py
 brain_pipe/runner/__init__.py
 brain_pipe/runner/base.py
 brain_pipe/runner/default.py
 brain_pipe/save/__init__.py
 brain_pipe/save/base.py
 brain_pipe/save/default.py
 brain_pipe/split/__init__.py
@@ -79,15 +80,15 @@
 tests/test_cli/test_default.py
 tests/test_cli/test_factory.py
 tests/test_dataloaders/__init__.py
 tests/test_dataloaders/test_base.py
 tests/test_dataloaders/test_path.py
 tests/test_examples/__init__.py
 tests/test_examples/exporl/__init__.py
-tests/test_examples/exporl/test_auditory_eeg_dataset.py
+tests/test_examples/exporl/sparrKULee.py
 tests/test_parser/__init__.py
 tests/test_parser/test_base.py
 tests/test_parser/test_file.py
 tests/test_parser/test_simple_dict.py
 tests/test_parser/test_template_text.py
 tests/test_parser/test_text.py
 tests/test_parser/test_yaml.py
@@ -107,14 +108,15 @@
 tests/test_preprocessing/test_brain/test_rereference.py
 tests/test_preprocessing/test_brain/test_trigger.py
 tests/test_preprocessing/test_brain/test_eeg/__init__.py
 tests/test_preprocessing/test_brain/test_eeg/test_load.py
 tests/test_preprocessing/test_stimulus/__init__.py
 tests/test_preprocessing/test_stimulus/test_load.py
 tests/test_preprocessing/test_stimulus/test_audio/test_envelope.py
+tests/test_preprocessing/test_stimulus/test_audio/test_spectrogram.py
 tests/test_runner/__init__.py
 tests/test_runner/test_default.py
 tests/test_runner/test_runner_base.py
 tests/test_save/__init__.py
 tests/test_save/test_base.py
 tests/test_save/test_default.py
 tests/test_utils/__init__.py
```

### Comparing `brain_pipe-0.0.1/docs/source/conf.py` & `brain_pipe-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/examples/exporl/sparrKULee.py` & `brain_pipe-0.0.2/examples/exporl/sparrKULee.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 import glob
 import gzip
 import logging
 import os
 import pathlib
 import pickle
 import time
-from typing import Any, Dict, Union, Sequence
-
 import librosa
 import numpy as np
 import scipy.signal
+import scipy.signal.windows
+
 
+from typing import Any, Dict, Union, Sequence
 from brain_pipe.dataloaders.path import GlobLoader
 from brain_pipe.pipeline.default import DefaultPipeline
 from brain_pipe.preprocessing.brain.artifact import (
     InterpolateArtifacts,
     ArtifactRemovalMWF,
 )
 from brain_pipe.preprocessing.brain.eeg.biosemi import (
@@ -31,14 +32,15 @@
 )
 from brain_pipe.preprocessing.brain.rereference import CommonAverageRereference
 from brain_pipe.preprocessing.brain.trigger import (
     AlignPeriodicBlockTriggers,
 )
 from brain_pipe.preprocessing.filter import SosFiltFilt
 from brain_pipe.preprocessing.resample import ResamplePoly
+from brain_pipe.preprocessing.stimulus.audio.spectrogram import LibrosaMelSpectrogram
 from brain_pipe.save.default import DefaultSave
 from brain_pipe.preprocessing.stimulus.audio.envelope import GammatoneEnvelope
 from brain_pipe.preprocessing.stimulus.load import LoadStimuli
 from brain_pipe.utils.log import default_logging, DefaultFormatter
 from brain_pipe.utils.multiprocess import MultiprocessingSingleton
 from brain_pipe.utils.path import BIDSStimulusGrouper
 
@@ -274,14 +276,95 @@
 
     if set_name is not None:
         filename += f"_set-{set_name}"
 
     return os.path.join(subject, session, filename + ".npy")
 
 
+class SparrKULeeSpectrogramKwargs:
+    """Default function to generate the kwargs for the librosa spectrogram."""
+
+    def __init__(
+        self,
+        stimulus_sr_key="stimulus_sr",
+        target_fs=64,
+        hop_length=None,
+        win_length_sec=0.025,
+        n_fft=None,
+        window_fn=None,
+        n_mels=28,
+        fmin=-4.2735,
+        fmax=5444,
+        power=1.0,
+        center=False,
+        norm=None,
+        htk=True,
+    ):
+        self.stimulus_sr_key = stimulus_sr_key
+        self.target_fs = target_fs
+        self.hop_length = hop_length
+        self.win_length_sec = win_length_sec
+        self.n_fft = n_fft
+        self.window_fn = window_fn
+        if window_fn is None:
+            self.window_fn = scipy.signal.windows.hamming
+        self.n_mels = n_mels
+        self.fmin = fmin
+        self.fmax = fmax
+        self.power = power
+        self.center = center
+        self.norm = norm
+        self.htk = htk
+
+    def __call__(self, data_dict):
+        """Default function to generate the kwargs for the librosa spectrogram.
+
+        Parameters
+        ----------
+        data_dict: Dict[str, Any]
+            The data dict containing the data to save.
+
+        Returns
+        -------
+        Dict[str, Any]
+            The kwargs for the librosa spectrogram.
+
+        Notes
+        -----
+        Code was based on the code for the 2023 Auditory EEG Challenge code:
+        https://github.com/exporl/auditory-eeg-challenge-2023-code/blob/main/
+        task1_match_mismatch/util/mel_spectrogram.py
+        """
+        fs = data_dict[self.stimulus_sr_key]
+        result = {
+            "fmin": self.fmin,
+            "fmax": self.fmax,
+            "n_mels": self.n_mels,
+            "power": self.power,
+            "center": self.center,
+            "norm": self.norm,
+            "htk": self.htk,
+        }
+
+        result["hop_length"] = self.hop_length
+        if self.hop_length is None:
+            result["hop_length"] = int((1 / self.target_fs) * fs)
+
+        result["win_length"] = self.win_length_sec
+        if self.win_length_sec is not None:
+            result["win_length"] = int(self.win_length_sec * fs)
+
+        result["n_fft"] = self.n_fft
+        if self.n_fft is None:
+            result["n_fft"] = int(2 ** np.ceil(np.log2(result["win_length"])))
+
+        result["window"] = self.window_fn(result["win_length"])
+        return result
+
+
 def sparrkulee_logging(log_path):
     parsed_path = log_path.format(
         datetime=datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
     )
     handler = logging.FileHandler(parsed_path)
 
     handler.setLevel(logging.DEBUG)
@@ -321,14 +404,16 @@
     #########
 
     stimulus_steps = DefaultPipeline(
         steps=[
             LoadStimuli(load_fn=temp_stimulus_load_fn),
             GammatoneEnvelope(),
             ResamplePoly(64, "envelope_data", "stimulus_sr"),
+            # Uncomment the next line to also use mel
+            # LibrosaMelSpectrogram(power_factor=0.6, SparrKULeeSpectrogramKwargs()),
             DefaultSave(stimuli_dir, overwrite=overwrite),
         ],
         on_error=DefaultPipeline.RAISE,
     )
 
     eeg_steps = [
         LinkStimulusToBrainResponse(
```

### Comparing `brain_pipe-0.0.1/pyproject.toml` & `brain_pipe-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "numpy",
     "scipy",
     "mne>=1.3.0",
     "librosa",
     "pyyaml",
     "jinja2"
 ]
-version = "0.0.1"
+version = "0.0.2"
 dynamic = ["readme", "description"]
 
 [project.scripts]
 brain_pipe = "brain_pipe:cli_entrypoint"
 
 [tool.setuptools.dynamic]
 readme = {file = "README.md", content-type = "text/markdown"}
```

### Comparing `brain_pipe-0.0.1/tests/test_cli/test_base.py` & `brain_pipe-0.0.2/tests/test_cli/test_base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_cli/test_default.py` & `brain_pipe-0.0.2/tests/test_cli/test_default.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_cli/test_factory.py` & `brain_pipe-0.0.2/tests/test_cli/test_factory.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_dataloaders/test_base.py` & `brain_pipe-0.0.2/tests/test_dataloaders/test_base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_dataloaders/test_path.py` & `brain_pipe-0.0.2/tests/test_dataloaders/test_path.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_parser/test_base.py` & `brain_pipe-0.0.2/tests/test_parser/test_base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_parser/test_file.py` & `brain_pipe-0.0.2/tests/test_parser/test_file.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_parser/test_simple_dict.py` & `brain_pipe-0.0.2/tests/test_parser/test_simple_dict.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_parser/test_template_text.py` & `brain_pipe-0.0.2/tests/test_parser/test_template_text.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_parser/test_text.py` & `brain_pipe-0.0.2/tests/test_parser/test_text.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_parser/test_yaml.py` & `brain_pipe-0.0.2/tests/test_parser/test_yaml.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_pipeline/test_base.py` & `brain_pipe-0.0.2/tests/test_pipeline/test_base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_pipeline/test_default.py` & `brain_pipe-0.0.2/tests/test_pipeline/test_default.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_pipeline/test_wrapper.py` & `brain_pipe-0.0.2/tests/test_pipeline/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_artifact.py` & `brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_artifact.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_eeg/test_load.py` & `brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_eeg/test_load.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_epochs.py` & `brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_epochs.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_link.py` & `brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_link.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_load.py` & `brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_load.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_rereference.py` & `brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_rereference.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_preprocessing/test_brain/test_trigger.py` & `brain_pipe-0.0.2/tests/test_preprocessing/test_brain/test_trigger.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_preprocessing/test_filter.py` & `brain_pipe-0.0.2/tests/test_preprocessing/test_filter.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_preprocessing/test_resample.py` & `brain_pipe-0.0.2/tests/test_preprocessing/test_resample.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_preprocessing/test_stimulus/test_audio/test_envelope.py` & `brain_pipe-0.0.2/tests/test_preprocessing/test_stimulus/test_audio/test_envelope.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_preprocessing/test_stimulus/test_load.py` & `brain_pipe-0.0.2/tests/test_preprocessing/test_stimulus/test_load.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_runner/test_default.py` & `brain_pipe-0.0.2/tests/test_runner/test_default.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_runner/test_runner_base.py` & `brain_pipe-0.0.2/tests/test_runner/test_runner_base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_save/test_base.py` & `brain_pipe-0.0.2/tests/test_save/test_base.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_save/test_default.py` & `brain_pipe-0.0.2/tests/test_save/test_default.py`

 * *Files identical despite different names*

### Comparing `brain_pipe-0.0.1/tests/test_utils/test_find.py` & `brain_pipe-0.0.2/tests/test_utils/test_find.py`

 * *Files identical despite different names*

