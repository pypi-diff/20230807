# Comparing `tmp/ludwig-0.7.4.tar.gz` & `tmp/ludwig-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ludwig-0.7.4.tar", last modified: Thu Mar 23 15:29:51 2023, max compression
+gzip compressed data, was "ludwig-0.7.5.tar", last modified: Mon Aug  7 21:11:36 2023, max compression
```

## Comparing `ludwig-0.7.4.tar` & `ludwig-0.7.5.tar`

### file list

```diff
@@ -1,701 +1,701 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.067867 ludwig-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-03-23 15:29:35.000000 ludwig-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-23 15:29:35.000000 ludwig-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-03-23 15:29:35.000000 ludwig-0.7.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    21285 2023-03-23 15:29:51.067867 ludwig-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-03-23 15:29:35.000000 ludwig-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.011867 ludwig-0.7.4/ludwig/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89211 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/api_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.011867 ludwig-0.7.4/ludwig/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/automl/auto_tune_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22740 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/automl/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/automl/base_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.011867 ludwig-0.7.4/ludwig/automl/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/automl/defaults/base_automl_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.015867 ludwig-0.7.4/ludwig/automl/defaults/combiner/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/automl/defaults/combiner/concat_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/automl/defaults/combiner/tabnet_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/automl/defaults/combiner/transformer_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   101826 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/automl/defaults/reference_configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.015867 ludwig-0.7.4/ludwig/automl/defaults/text/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/automl/defaults/text/bert_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.015867 ludwig-0.7.4/ludwig/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/backend/_ray210_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/backend/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/backend/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    38203 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/backend/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.015867 ludwig-0.7.4/ludwig/backend/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/backend/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/backend/utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.015867 ludwig-0.7.4/ludwig/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/benchmarking/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/benchmarking/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/benchmarking/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/benchmarking/profiler_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/benchmarking/profiler_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/benchmarking/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/benchmarking/summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/benchmarking/summary_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/benchmarking/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.015867 ludwig-0.7.4/ludwig/combiners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/combiners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42068 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/combiners/combiners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.015867 ludwig-0.7.4/ludwig/config_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/config_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17382 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/config_validation/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/config_validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.015867 ludwig-0.7.4/ludwig/contribs/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/contribs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/contribs/aim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/contribs/comet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.015867 ludwig-0.7.4/ludwig/contribs/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/contribs/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/contribs/mlflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/contribs/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.015867 ludwig-0.7.4/ludwig/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.019867 ludwig-0.7.4/ludwig/data/batcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/batcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/batcher/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/batcher/bucketed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/batcher/iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/batcher/random_access.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.019867 ludwig-0.7.4/ludwig/data/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/cache/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/cache/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/cache/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/concatenate_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.019867 ludwig-0.7.4/ludwig/data/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/dataframe/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/dataframe/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/dataframe/modin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/dataframe/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.019867 ludwig-0.7.4/ludwig/data/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/dataset/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/dataset/ray.py
--rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/dataset_synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/negative_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    84447 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/split_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.019867 ludwig-0.7.4/ludwig/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/archives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.027867 ludwig-0.7.4/ludwig/datasets/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/adult_census_income.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/ae_price_prediction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/agnews.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/allstate_claims_severity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/amazon_employee_access_challenge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/amazon_review_polarity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/amazon_reviews.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/ames_housing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/bbcnews.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/bnp_claims_management.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/bookprice_prediction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/california_house_price.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/connect4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/creditcard_fraud.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/customer_churn_prediction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/data_scientist_salary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/dbpedia.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/electricity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/ethos_binary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/fake_job_postings2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/fever.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/flickr8k.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/forest_cover.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/goemotions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/goodbooks_books.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/google_qa_answer_type_reason_explanation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/google_qa_question_type_reason_explanation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/google_quest_qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/higgs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/ieee_fraud.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/imbalanced_insurance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/imdb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/imdb_genre_prediction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/insurance_lite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/iris.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/irony.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/jc_penney_products.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/jigsaw_unintended_bias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/jigsaw_unintended_bias100k.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/kdd_appetency.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/kdd_churn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/kdd_upselling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/kick_starter_funding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/melbourne_airbnb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/mercari_price_suggestion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/mercari_price_suggestion100K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/mercedes_benz_greener.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/mnist.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/mushroom_edibility.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/naval.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/news_channel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/news_popularity2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/noshow_appointments.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/numerai28pt6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/ohsumed_7400.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/ohsumed_cmu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/otto_group_product.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/poker_hand.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/porto_seguro_safe_driver.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/product_sentiment_machine_hack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/protein.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/reuters_cmu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/reuters_r8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/rossman_store_sales.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/santander_customer_satisfaction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/santander_customer_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/santander_value_prediction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/sarcastic_headlines.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/sarcos.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/sst2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/sst3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/sst5.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/synthetic_fraud.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/talkingdata_adtrack_fraud.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/telco_customer_churn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/temperature.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/titanic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/twitter_bots.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/walmart_recruiting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/wine_reviews.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/wmt15.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/women_clothing_review.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/yahoo_answers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/yelp_review_polarity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/yelp_reviews.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/configs/yosemite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/kaggle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.031867 ludwig-0.7.4/ludwig/datasets/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/adult_census_income.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/agnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/allstate_claims_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/creditcard_fraud.py
--rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/dataset_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/ethos_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/flickr8k.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/forest_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/goemotions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/higgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/ieee_fraud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/insurance_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/kdd_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/naval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/rossman_store_sales.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/santander_value_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/sarcastic_headlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/sarcos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/split_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/loaders/sst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.031867 ludwig-0.7.4/ludwig/datasets/model_configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/adult_census_income_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/allstate_claims_severity_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/ames_housing_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/bnp_claims_management_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/forest_cover_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/higgs_best.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/higgs_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/ieee_fraud_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/mercedes_benz_greener_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/mnist_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/mushroom_edibility_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/otto_group_product_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/poker_hand_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/porto_seguro_safe_driver_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/synthetic_fraud_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/model_configs/titanic_default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.031867 ludwig-0.7.4/ludwig/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/decoders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/decoders/generic_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/decoders/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/decoders/sequence_decoder_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/decoders/sequence_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/decoders/sequence_tagger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.031867 ludwig-0.7.4/ludwig/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/distributed/_ray_210_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/distributed/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/distributed/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/distributed/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/distributed/horovod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.035867 ludwig-0.7.4/ludwig/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/bag_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/category_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/date_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/generic_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/h3_encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.035867 ludwig-0.7.4/ludwig/encoders/image/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/image/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23335 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/image/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    94935 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/sequence_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/set_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    75228 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/encoders/text_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    21860 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.035867 ludwig-0.7.4/ludwig/explain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/explain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/explain/captum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/explain/captum_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/explain/explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/explain/explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/explain/gbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/explain/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.035867 ludwig-0.7.4/ludwig/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/audio_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/bag_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    24159 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/base_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/binary_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    19818 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/category_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/date_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/feature_registries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/h3_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/image_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/number_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/sequence_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/set_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/text_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/timeseries_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/features/vector_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.035867 ludwig-0.7.4/ludwig/hyperopt/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/hyperopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47055 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/hyperopt/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/hyperopt/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/hyperopt/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/hyperopt/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/hyperopt/search_algos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/hyperopt/syncer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/hyperopt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/hyperopt_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.039867 ludwig-0.7.4/ludwig/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/models/calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/models/ecd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/models/embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/models/gbm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15476 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/models/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.039867 ludwig-0.7.4/ludwig/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/attention_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    48845 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/convolutional_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/embedding_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/fully_connected_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/initializer_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/loss_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/metric_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/metric_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/mlp_mixer_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/normalization_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/optimization_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/recurrent_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/reduction_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/modules/tabnet_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.039867 ludwig-0.7.4/ludwig/profiling/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/profiling/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/profiling/dataset_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/profiling/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.039867 ludwig-0.7.4/ludwig/profiling/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/profiling/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/profiling/proto/dataset_profile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    58236 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/profiling/proto/whylogs_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/profiling/type_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/profiling/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/progress_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.043867 ludwig-0.7.4/ludwig/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.043867 ludwig-0.7.4/ludwig/schema/combiners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/common_transformer_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/project_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/sequence_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/combiners/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/common_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.043867 ludwig-0.7.4/ludwig/schema/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/decoders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/decoders/sequence_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/decoders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.043867 ludwig-0.7.4/ludwig/schema/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/defaults/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/defaults/ecd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/defaults/gbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/defaults/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.043867 ludwig-0.7.4/ludwig/schema/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/bag_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/category_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/date_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12491 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/h3_encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.043867 ludwig-0.7.4/ludwig/schema/encoders/image/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30681 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/image/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/image/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)    33230 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/sequence_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/set_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)   117818 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/text_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/encoders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.047867 ludwig-0.7.4/ludwig/schema/features/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/audio_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.047867 ludwig-0.7.4/ludwig/schema/features/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/augmentation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/augmentation/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/augmentation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/bag_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/binary_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/category_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/date_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/h3_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/image_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.047867 ludwig-0.7.4/ludwig/schema/features/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/loss/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/loss/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/number_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.047867 ludwig-0.7.4/ludwig/schema/features/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/bag.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/h3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/preprocessing/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/sequence_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/set_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/text_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/timeseries_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/features/vector_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.047867 ludwig-0.7.4/ludwig/schema/hyperopt/
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/hyperopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/hyperopt/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/hyperopt/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/hyperopt/search_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.047867 ludwig-0.7.4/ludwig/schema/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.051867 ludwig-0.7.4/ludwig/schema/metadata/configs/
--rw-r--r--   0 runner    (1001) docker     (123)    89568 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/configs/combiners.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17569 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/configs/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/configs/decoders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   457039 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/configs/encoders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    47218 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/configs/features.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/configs/loss.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/configs/optimizers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/configs/preprocessing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    41110 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/configs/trainer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/metadata/parameter_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.051867 ludwig-0.7.4/ludwig/schema/model_types/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/model_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/model_types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/model_types/ecd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/model_types/gbm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/model_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21983 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/split.py
--rw-r--r--   0 runner    (1001) docker     (123)    29767 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    46355 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/schema/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.051867 ludwig-0.7.4/ludwig/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/trainers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    54196 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/trainers/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    44260 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/trainers/trainer_lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.055867 ludwig-0.7.4/ludwig/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/algorithms_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/audio_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/augmentation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.055867 ludwig-0.7.4/ludwig/utils/automl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/automl/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/automl/field_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/automl/ray_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/automl/type_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/automl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34428 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/backward_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/batch_size_tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/checkpoint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35078 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.055867 ludwig-0.7.4/ludwig/utils/entmax/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/entmax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/entmax/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/entmax/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/entmax/root_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/error_handling_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/fs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/gbm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/h3_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/hf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/horovod_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/inference_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/loss_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/math_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/metrics_printed_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/neuropod_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/nlp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/numerical_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/output_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/print_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/server_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/state_dict_backward_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/strings_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/structural_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    47907 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/tokenizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29019 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/triton_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/version_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    45292 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/utils/visualization_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   169128 2023-03-23 15:29:35.000000 ludwig-0.7.4/ludwig/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.011867 ludwig-0.7.4/ludwig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21285 2023-03-23 15:29:50.000000 ludwig-0.7.4/ludwig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-03-23 15:29:50.000000 ludwig-0.7.4/ludwig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 15:29:50.000000 ludwig-0.7.4/ludwig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-23 15:29:50.000000 ludwig-0.7.4/ludwig.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-23 15:29:50.000000 ludwig-0.7.4/ludwig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-23 15:29:50.000000 ludwig-0.7.4/ludwig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-23 15:29:35.000000 ludwig-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-23 15:29:35.000000 ludwig-0.7.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-23 15:29:35.000000 ludwig-0.7.4/requirements_benchmarking.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-23 15:29:35.000000 ludwig-0.7.4/requirements_distributed.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-23 15:29:35.000000 ludwig-0.7.4/requirements_explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-23 15:29:35.000000 ludwig-0.7.4/requirements_hyperopt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-23 15:29:35.000000 ludwig-0.7.4/requirements_serve.txt
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-23 15:29:35.000000 ludwig-0.7.4/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-23 15:29:35.000000 ludwig-0.7.4/requirements_tree.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-23 15:29:35.000000 ludwig-0.7.4/requirements_viz.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-23 15:29:51.067867 ludwig-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-03-23 15:29:35.000000 ludwig-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.007867 ludwig-0.7.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.063867 ludwig-0.7.4/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/parameter_update_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/synthetic_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    25905 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_audio_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_automl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_cached_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_class_imbalance_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_config_global_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_contrib_aim.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_contrib_comet.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_contrib_wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_custom_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    36039 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_gbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_graph_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    22903 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_hyperopt_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_hyperopt_ray_horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_input_feature_tied.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_kfold_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_missing_value_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    16893 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_model_save_and_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_model_training_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_neuropod.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_number_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    28612 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    38938 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_reducers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_regularizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_sequence_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_sequence_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_sequence_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_simple_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_timeseries_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    32501 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_triton.py
--rw-r--r--   0 runner    (1001) docker     (123)    60704 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    38533 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/test_visualization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36162 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/integration_tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.063867 ludwig-0.7.4/tests/ludwig/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.063867 ludwig-0.7.4/tests/ludwig/automl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/automl/test_base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/automl/test_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/automl/test_tune_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/automl/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.063867 ludwig-0.7.4/tests/ludwig/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/datasets/check_dead_links.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/datasets/download_all_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/datasets/test_dataset_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/datasets/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/datasets/test_model_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.063867 ludwig-0.7.4/tests/ludwig/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/encoders/test_bag_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/encoders/test_category_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/encoders/test_date_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/encoders/test_generic_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/encoders/test_h3_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22196 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/encoders/test_image_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/encoders/test_sequence_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/encoders/test_set_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/encoders/test_text_encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.063867 ludwig-0.7.4/tests/ludwig/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_audio_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_bag_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_binary_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_category_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_date_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_h3_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_image_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_number_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_sequence_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_set_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_text_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/features/test_timeseries_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.063867 ludwig-0.7.4/tests/ludwig/models/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/models/test_trainable_image_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/models/test_training_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/models/test_training_success.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.067867 ludwig-0.7.4/tests/ludwig/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_convolutional_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_embedding_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_fully_connected_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_initializer_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_loss_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_metric_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_mlp_mixer_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_normalization_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_recurrent_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_reduction_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_tabnet_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/modules/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:29:51.067867 ludwig-0.7.4/tests/ludwig/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26930 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_backward_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_class_balancing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_fs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_hf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_hyperopt_ray_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_numerical_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_output_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_server_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_state_dict_backward_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_strings_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_tokenizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-23 15:29:35.000000 ludwig-0.7.4/tests/ludwig/utils/test_version_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.891890 ludwig-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-08-07 21:11:25.000000 ludwig-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-07 21:11:25.000000 ludwig-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-08-07 21:11:25.000000 ludwig-0.7.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    21285 2023-08-07 21:11:36.891890 ludwig-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-08-07 21:11:25.000000 ludwig-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.831889 ludwig-0.7.5/ludwig/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89289 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/api_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.831889 ludwig-0.7.5/ludwig/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/automl/auto_tune_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22740 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/automl/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/automl/base_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.831889 ludwig-0.7.5/ludwig/automl/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/automl/defaults/base_automl_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.835890 ludwig-0.7.5/ludwig/automl/defaults/combiner/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/automl/defaults/combiner/concat_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/automl/defaults/combiner/tabnet_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/automl/defaults/combiner/transformer_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   101826 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/automl/defaults/reference_configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.835890 ludwig-0.7.5/ludwig/automl/defaults/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/automl/defaults/text/bert_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.835890 ludwig-0.7.5/ludwig/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/backend/_ray210_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/backend/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/backend/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38203 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/backend/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.835890 ludwig-0.7.5/ludwig/backend/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/backend/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/backend/utils/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.835890 ludwig-0.7.5/ludwig/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/benchmarking/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/benchmarking/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/benchmarking/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/benchmarking/profiler_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/benchmarking/profiler_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/benchmarking/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/benchmarking/summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/benchmarking/summary_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/benchmarking/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.835890 ludwig-0.7.5/ludwig/combiners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/combiners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42068 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/combiners/combiners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.835890 ludwig-0.7.5/ludwig/config_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/config_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17382 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/config_validation/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/config_validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.835890 ludwig-0.7.5/ludwig/contribs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/contribs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/contribs/aim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/contribs/comet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.835890 ludwig-0.7.5/ludwig/contribs/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/contribs/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/contribs/mlflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/contribs/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.839890 ludwig-0.7.5/ludwig/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.839890 ludwig-0.7.5/ludwig/data/batcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/batcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/batcher/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/batcher/bucketed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/batcher/iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/batcher/random_access.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.839890 ludwig-0.7.5/ludwig/data/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/cache/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/cache/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/cache/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/concatenate_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.839890 ludwig-0.7.5/ludwig/data/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/dataframe/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/dataframe/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/dataframe/modin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/dataframe/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.839890 ludwig-0.7.5/ludwig/data/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/dataset/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/dataset/ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/dataset_synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/negative_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84447 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/split_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.839890 ludwig-0.7.5/ludwig/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/archives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.847890 ludwig-0.7.5/ludwig/datasets/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/adult_census_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/ae_price_prediction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/agnews.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/allstate_claims_severity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/amazon_employee_access_challenge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/amazon_review_polarity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/amazon_reviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/ames_housing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/bbcnews.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/bnp_claims_management.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/bookprice_prediction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/california_house_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/connect4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/creditcard_fraud.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/customer_churn_prediction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/data_scientist_salary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/dbpedia.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/electricity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/ethos_binary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/fake_job_postings2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/fever.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/flickr8k.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/forest_cover.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/goemotions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/goodbooks_books.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/google_qa_answer_type_reason_explanation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/google_qa_question_type_reason_explanation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/google_quest_qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/higgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/ieee_fraud.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/imbalanced_insurance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/imdb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/imdb_genre_prediction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/insurance_lite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/iris.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/irony.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/jc_penney_products.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/jigsaw_unintended_bias.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/jigsaw_unintended_bias100k.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/kdd_appetency.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/kdd_churn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/kdd_upselling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/kick_starter_funding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/melbourne_airbnb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/mercari_price_suggestion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/mercari_price_suggestion100K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/mercedes_benz_greener.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/mnist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/mushroom_edibility.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/naval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/news_channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/news_popularity2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/noshow_appointments.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/numerai28pt6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/ohsumed_7400.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/ohsumed_cmu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/otto_group_product.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/poker_hand.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/porto_seguro_safe_driver.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/product_sentiment_machine_hack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/protein.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/reuters_cmu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/reuters_r8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/rossman_store_sales.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/santander_customer_satisfaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/santander_customer_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/santander_value_prediction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/sarcastic_headlines.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/sarcos.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/sst2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/sst3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/sst5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/synthetic_fraud.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/talkingdata_adtrack_fraud.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/telco_customer_churn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/temperature.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/titanic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/twitter_bots.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/walmart_recruiting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/wine_reviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/wmt15.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/women_clothing_review.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/yahoo_answers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/yelp_review_polarity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/yelp_reviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/configs/yosemite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/kaggle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.847890 ludwig-0.7.5/ludwig/datasets/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/adult_census_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/agnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/allstate_claims_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/creditcard_fraud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/dataset_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/ethos_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/flickr8k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/forest_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/goemotions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/higgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/ieee_fraud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/insurance_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/kdd_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/naval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/rossman_store_sales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/santander_value_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/sarcastic_headlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/sarcos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/split_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/loaders/sst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.851890 ludwig-0.7.5/ludwig/datasets/model_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/adult_census_income_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/allstate_claims_severity_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/ames_housing_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/bnp_claims_management_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/forest_cover_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/higgs_best.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/higgs_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/ieee_fraud_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/mercedes_benz_greener_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/mnist_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/mushroom_edibility_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/otto_group_product_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/poker_hand_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/porto_seguro_safe_driver_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/synthetic_fraud_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/model_configs/titanic_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.851890 ludwig-0.7.5/ludwig/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/decoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/decoders/generic_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/decoders/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/decoders/sequence_decoder_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/decoders/sequence_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/decoders/sequence_tagger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.851890 ludwig-0.7.5/ludwig/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/distributed/_ray_210_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/distributed/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/distributed/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/distributed/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/distributed/horovod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.855890 ludwig-0.7.5/ludwig/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/bag_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/category_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/date_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/generic_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/h3_encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.855890 ludwig-0.7.5/ludwig/encoders/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/image/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23335 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/image/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94935 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/sequence_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/set_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75832 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/encoders/text_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21860 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.855890 ludwig-0.7.5/ludwig/explain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/explain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/explain/captum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/explain/captum_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/explain/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/explain/explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/explain/gbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/explain/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.855890 ludwig-0.7.5/ludwig/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/audio_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/bag_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24159 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/base_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/binary_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19818 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/category_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/date_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/feature_registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/h3_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/image_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/number_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/sequence_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/set_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/text_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/timeseries_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/features/vector_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.855890 ludwig-0.7.5/ludwig/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47055 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/hyperopt/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/hyperopt/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/hyperopt/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/hyperopt/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/hyperopt/search_algos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/hyperopt/syncer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/hyperopt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/hyperopt_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.859890 ludwig-0.7.5/ludwig/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/models/calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/models/ecd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/models/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/models/gbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15476 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/models/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.859890 ludwig-0.7.5/ludwig/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/attention_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48845 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/convolutional_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/embedding_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/fully_connected_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/initializer_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/loss_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/metric_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/metric_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/mlp_mixer_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/normalization_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/optimization_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/recurrent_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/reduction_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/modules/tabnet_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.863890 ludwig-0.7.5/ludwig/profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/profiling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/profiling/dataset_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/profiling/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.863890 ludwig-0.7.5/ludwig/profiling/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/profiling/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/profiling/proto/dataset_profile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58236 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/profiling/proto/whylogs_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/profiling/type_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/profiling/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.863890 ludwig-0.7.5/ludwig/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.863890 ludwig-0.7.5/ludwig/schema/combiners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/common_transformer_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/project_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/sequence_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/combiners/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/common_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.867890 ludwig-0.7.5/ludwig/schema/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/decoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/decoders/sequence_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/decoders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.867890 ludwig-0.7.5/ludwig/schema/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/defaults/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/defaults/ecd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/defaults/gbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/defaults/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.867890 ludwig-0.7.5/ludwig/schema/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/bag_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/category_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/date_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12491 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/h3_encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.867890 ludwig-0.7.5/ludwig/schema/encoders/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30681 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/image/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/image/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33230 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/sequence_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/set_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117818 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/text_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/encoders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.867890 ludwig-0.7.5/ludwig/schema/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/audio_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.871890 ludwig-0.7.5/ludwig/schema/features/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/augmentation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/augmentation/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/augmentation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/bag_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/binary_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/category_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/date_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/h3_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/image_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.871890 ludwig-0.7.5/ludwig/schema/features/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/loss/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/loss/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/number_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.871890 ludwig-0.7.5/ludwig/schema/features/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/h3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/preprocessing/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/sequence_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/set_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/text_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/timeseries_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/features/vector_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.871890 ludwig-0.7.5/ludwig/schema/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/hyperopt/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/hyperopt/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/hyperopt/search_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.871890 ludwig-0.7.5/ludwig/schema/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.875890 ludwig-0.7.5/ludwig/schema/metadata/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)    89568 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/configs/combiners.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17569 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/configs/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/configs/decoders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   457039 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/configs/encoders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    47218 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/configs/features.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/configs/loss.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/configs/optimizers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/configs/preprocessing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    41110 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/configs/trainer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/metadata/parameter_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.875890 ludwig-0.7.5/ludwig/schema/model_types/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/model_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/model_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/model_types/ecd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/model_types/gbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/model_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21983 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29767 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46355 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/schema/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.875890 ludwig-0.7.5/ludwig/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/trainers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54196 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/trainers/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44260 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/trainers/trainer_lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.879890 ludwig-0.7.5/ludwig/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/algorithms_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/audio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/augmentation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.879890 ludwig-0.7.5/ludwig/utils/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/automl/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/automl/field_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/automl/ray_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/automl/type_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/automl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34428 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/backward_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/batch_size_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/checkpoint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35151 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.879890 ludwig-0.7.5/ludwig/utils/entmax/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/entmax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/entmax/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/entmax/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/entmax/root_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/error_handling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/fs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/gbm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/h3_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/hf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/horovod_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/inference_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/loss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/metrics_printed_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/neuropod_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/nlp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/numerical_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/output_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/print_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/server_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/state_dict_backward_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/strings_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/structural_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47907 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29019 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/triton_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/version_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45292 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/utils/visualization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169128 2023-08-07 21:11:25.000000 ludwig-0.7.5/ludwig/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.831889 ludwig-0.7.5/ludwig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21285 2023-08-07 21:11:36.000000 ludwig-0.7.5/ludwig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-08-07 21:11:36.000000 ludwig-0.7.5/ludwig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 21:11:36.000000 ludwig-0.7.5/ludwig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 21:11:36.000000 ludwig-0.7.5/ludwig.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-07 21:11:36.000000 ludwig-0.7.5/ludwig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 21:11:36.000000 ludwig-0.7.5/ludwig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-07 21:11:25.000000 ludwig-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-07 21:11:25.000000 ludwig-0.7.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-07 21:11:25.000000 ludwig-0.7.5/requirements_benchmarking.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-07 21:11:25.000000 ludwig-0.7.5/requirements_distributed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 21:11:25.000000 ludwig-0.7.5/requirements_explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-07 21:11:25.000000 ludwig-0.7.5/requirements_hyperopt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-07 21:11:25.000000 ludwig-0.7.5/requirements_serve.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-07 21:11:25.000000 ludwig-0.7.5/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-07 21:11:25.000000 ludwig-0.7.5/requirements_tree.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-07 21:11:25.000000 ludwig-0.7.5/requirements_viz.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-07 21:11:36.895890 ludwig-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-07 21:11:25.000000 ludwig-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.827890 ludwig-0.7.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.887890 ludwig-0.7.5/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/parameter_update_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/synthetic_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25905 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_audio_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_cached_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_class_imbalance_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_config_global_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_contrib_aim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_contrib_comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_contrib_wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_custom_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36039 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_gbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_graph_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22903 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_hyperopt_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_hyperopt_ray_horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_input_feature_tied.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_kfold_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_missing_value_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16893 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_model_save_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_model_training_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_neuropod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_number_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28612 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38938 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_reducers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_sequence_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_sequence_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_sequence_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_simple_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_timeseries_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32501 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60704 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38533 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/test_visualization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36162 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/integration_tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.887890 ludwig-0.7.5/tests/ludwig/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.887890 ludwig-0.7.5/tests/ludwig/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/automl/test_base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/automl/test_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/automl/test_tune_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/automl/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.887890 ludwig-0.7.5/tests/ludwig/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/datasets/check_dead_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/datasets/download_all_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/datasets/test_dataset_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/datasets/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/datasets/test_model_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.887890 ludwig-0.7.5/tests/ludwig/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/encoders/test_bag_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/encoders/test_category_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/encoders/test_date_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/encoders/test_generic_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/encoders/test_h3_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22196 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/encoders/test_image_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/encoders/test_sequence_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/encoders/test_set_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/encoders/test_text_encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.887890 ludwig-0.7.5/tests/ludwig/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_audio_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_bag_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_binary_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_category_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_date_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_h3_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_image_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_number_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_sequence_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_set_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_text_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/features/test_timeseries_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.887890 ludwig-0.7.5/tests/ludwig/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/models/test_trainable_image_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/models/test_training_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/models/test_training_success.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.891890 ludwig-0.7.5/tests/ludwig/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_convolutional_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_embedding_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_fully_connected_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_initializer_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_loss_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_metric_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_mlp_mixer_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_normalization_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_recurrent_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_reduction_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_tabnet_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/modules/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 21:11:36.891890 ludwig-0.7.5/tests/ludwig/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26930 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_backward_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_class_balancing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_fs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_hf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_hyperopt_ray_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_numerical_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_output_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_server_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_state_dict_backward_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_strings_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-07 21:11:25.000000 ludwig-0.7.5/tests/ludwig/utils/test_version_transformation.py
```

### Comparing `ludwig-0.7.4/LICENSE` & `ludwig-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/NOTICE` & `ludwig-0.7.5/NOTICE`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/PKG-INFO` & `ludwig-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ludwig
-Version: 0.7.4
+Version: 0.7.5
 Summary: Declarative machine learning: End-to-end machine learning pipelines using data-driven configurations.
 Home-page: https://github.com/ludwig-ai/ludwig
 Author: Piero Molino
 Author-email: piero.molino@gmail.com
 License: Apache 2.0
 Download-URL: https://pypi.org/project/ludwig/
 Description: ![Ludwig logo](https://github.com/ludwig-ai/ludwig-docs/raw/master/docs/images/ludwig_hero.png "Ludwig logo")
```

### Comparing `ludwig-0.7.4/README.md` & `ludwig-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/__init__.py` & `ludwig-0.7.5/ludwig/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/api.py` & `ludwig-0.7.5/ludwig/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1814,14 +1814,16 @@
     if not os.path.isdir(output_directory):
         os.mkdir(output_directory)
 
     # prepare data for k-fold processing
     # use Ludwig's utility to facilitate creating a dataframe
     # that is used as the basis for creating folds
 
+    dataset, _, _, _ = load_dataset_uris(dataset, None, None, None, backend)
+
     # determine data format of provided dataset
     if not data_format or data_format == "auto":
         data_format = figure_data_format(dataset)
 
     data_df = load_dataset(dataset, data_format=data_format, df_lib=backend.df_engine.df_lib)
 
     kfold_cv_stats = {}
```

### Comparing `ludwig-0.7.4/ludwig/api_annotations.py` & `ludwig-0.7.5/ludwig/api_annotations.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/automl/auto_tune_config.py` & `ludwig-0.7.5/ludwig/automl/auto_tune_config.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/automl/automl.py` & `ludwig-0.7.5/ludwig/automl/automl.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/automl/base_config.py` & `ludwig-0.7.5/ludwig/automl/base_config.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/automl/defaults/combiner/concat_config.yaml` & `ludwig-0.7.5/ludwig/automl/defaults/combiner/concat_config.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/automl/defaults/combiner/tabnet_config.yaml` & `ludwig-0.7.5/ludwig/automl/defaults/combiner/tabnet_config.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/automl/defaults/combiner/transformer_config.yaml` & `ludwig-0.7.5/ludwig/automl/defaults/combiner/transformer_config.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/automl/defaults/reference_configs.yaml` & `ludwig-0.7.5/ludwig/automl/defaults/reference_configs.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/backend/__init__.py` & `ludwig-0.7.5/ludwig/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/backend/_ray210_compat.py` & `ludwig-0.7.5/ludwig/backend/_ray210_compat.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/backend/base.py` & `ludwig-0.7.5/ludwig/backend/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/backend/datasource.py` & `ludwig-0.7.5/ludwig/backend/datasource.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/backend/horovod.py` & `ludwig-0.7.5/ludwig/backend/horovod.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/backend/ray.py` & `ludwig-0.7.5/ludwig/backend/ray.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/backend/utils/storage.py` & `ludwig-0.7.5/ludwig/backend/utils/storage.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/benchmarking/artifacts.py` & `ludwig-0.7.5/ludwig/benchmarking/artifacts.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/benchmarking/benchmark.py` & `ludwig-0.7.5/ludwig/benchmarking/benchmark.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/benchmarking/profiler.py` & `ludwig-0.7.5/ludwig/benchmarking/profiler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/benchmarking/profiler_callbacks.py` & `ludwig-0.7.5/ludwig/benchmarking/profiler_callbacks.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/benchmarking/profiler_dataclasses.py` & `ludwig-0.7.5/ludwig/benchmarking/profiler_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/benchmarking/reporting.py` & `ludwig-0.7.5/ludwig/benchmarking/reporting.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/benchmarking/summarize.py` & `ludwig-0.7.5/ludwig/benchmarking/summarize.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/benchmarking/summary_dataclasses.py` & `ludwig-0.7.5/ludwig/benchmarking/summary_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/benchmarking/utils.py` & `ludwig-0.7.5/ludwig/benchmarking/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/callbacks.py` & `ludwig-0.7.5/ludwig/callbacks.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/check.py` & `ludwig-0.7.5/ludwig/check.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/cli.py` & `ludwig-0.7.5/ludwig/cli.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/collect.py` & `ludwig-0.7.5/ludwig/collect.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/combiners/combiners.py` & `ludwig-0.7.5/ludwig/combiners/combiners.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/config_validation/checks.py` & `ludwig-0.7.5/ludwig/config_validation/checks.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/config_validation/validation.py` & `ludwig-0.7.5/ludwig/config_validation/validation.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/constants.py` & `ludwig-0.7.5/ludwig/constants.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/contrib.py` & `ludwig-0.7.5/ludwig/contrib.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/contribs/__init__.py` & `ludwig-0.7.5/ludwig/contribs/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/contribs/aim.py` & `ludwig-0.7.5/ludwig/contribs/aim.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/contribs/comet.py` & `ludwig-0.7.5/ludwig/contribs/comet.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/contribs/mlflow/__init__.py` & `ludwig-0.7.5/ludwig/contribs/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/contribs/mlflow/model.py` & `ludwig-0.7.5/ludwig/contribs/mlflow/model.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/contribs/wandb.py` & `ludwig-0.7.5/ludwig/contribs/wandb.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/batcher/base.py` & `ludwig-0.7.5/ludwig/data/batcher/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/batcher/bucketed.py` & `ludwig-0.7.5/ludwig/data/batcher/bucketed.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/batcher/iterable.py` & `ludwig-0.7.5/ludwig/data/batcher/iterable.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/batcher/random_access.py` & `ludwig-0.7.5/ludwig/data/batcher/random_access.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/cache/manager.py` & `ludwig-0.7.5/ludwig/data/cache/manager.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/cache/types.py` & `ludwig-0.7.5/ludwig/data/cache/types.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/cache/util.py` & `ludwig-0.7.5/ludwig/data/cache/util.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/concatenate_datasets.py` & `ludwig-0.7.5/ludwig/data/concatenate_datasets.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/dataframe/__init__.py` & `ludwig-0.7.5/ludwig/data/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/dataframe/base.py` & `ludwig-0.7.5/ludwig/data/dataframe/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/dataframe/dask.py` & `ludwig-0.7.5/ludwig/data/dataframe/dask.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/dataframe/modin.py` & `ludwig-0.7.5/ludwig/data/dataframe/modin.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/dataframe/pandas.py` & `ludwig-0.7.5/ludwig/data/dataframe/pandas.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/dataset/__init__.py` & `ludwig-0.7.5/ludwig/data/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/dataset/base.py` & `ludwig-0.7.5/ludwig/data/dataset/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/dataset/pandas.py` & `ludwig-0.7.5/ludwig/data/dataset/pandas.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/dataset/ray.py` & `ludwig-0.7.5/ludwig/data/dataset/ray.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/dataset_synthesizer.py` & `ludwig-0.7.5/ludwig/data/dataset_synthesizer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/negative_sampling.py` & `ludwig-0.7.5/ludwig/data/negative_sampling.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/postprocessing.py` & `ludwig-0.7.5/ludwig/data/postprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/preprocessing.py` & `ludwig-0.7.5/ludwig/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/sampler.py` & `ludwig-0.7.5/ludwig/data/sampler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/split.py` & `ludwig-0.7.5/ludwig/data/split.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/split_dataset.py` & `ludwig-0.7.5/ludwig/data/split_dataset.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/data/utils.py` & `ludwig-0.7.5/ludwig/data/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/__init__.py` & `ludwig-0.7.5/ludwig/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/archives.py` & `ludwig-0.7.5/ludwig/datasets/archives.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/adult_census_income.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/adult_census_income.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/ae_price_prediction.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/ae_price_prediction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/agnews.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/agnews.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/amazon_employee_access_challenge.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/amazon_employee_access_challenge.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/amazon_review_polarity.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/amazon_review_polarity.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/amazon_reviews.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/amazon_reviews.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/bnp_claims_management.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/bnp_claims_management.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/bookprice_prediction.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/bookprice_prediction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/california_house_price.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/california_house_price.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/connect4.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/connect4.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/customer_churn_prediction.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/customer_churn_prediction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/data_scientist_salary.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/data_scientist_salary.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/dbpedia.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/dbpedia.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/electricity.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/electricity.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/ethos_binary.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/ethos_binary.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/fake_job_postings2.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/fake_job_postings2.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/fever.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/fever.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/flickr8k.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/flickr8k.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/forest_cover.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/forest_cover.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/goemotions.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/goemotions.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/goodbooks_books.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/goodbooks_books.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/google_qa_answer_type_reason_explanation.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/google_qa_answer_type_reason_explanation.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/google_qa_question_type_reason_explanation.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/google_qa_question_type_reason_explanation.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/google_quest_qa.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/google_quest_qa.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/higgs.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/higgs.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/ieee_fraud.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/ieee_fraud.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/imbalanced_insurance.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/imbalanced_insurance.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/imdb_genre_prediction.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/imdb_genre_prediction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/insurance_lite.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/insurance_lite.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/jc_penney_products.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/jc_penney_products.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/jigsaw_unintended_bias.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/jigsaw_unintended_bias.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/jigsaw_unintended_bias100k.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/jigsaw_unintended_bias100k.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/kdd_appetency.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/kdd_appetency.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/kdd_churn.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/kdd_churn.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/kdd_upselling.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/kdd_upselling.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/kick_starter_funding.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/kick_starter_funding.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/melbourne_airbnb.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/melbourne_airbnb.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/mercari_price_suggestion.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/mercari_price_suggestion.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/mercari_price_suggestion100K.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/mercari_price_suggestion100K.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/mnist.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/mnist.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/mushroom_edibility.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/mushroom_edibility.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/naval.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/naval.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/news_channel.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/news_channel.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/news_popularity2.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/news_popularity2.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/noshow_appointments.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/noshow_appointments.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/ohsumed_7400.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/ohsumed_7400.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/ohsumed_cmu.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/ohsumed_cmu.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/otto_group_product.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/otto_group_product.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/poker_hand.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/poker_hand.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/porto_seguro_safe_driver.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/porto_seguro_safe_driver.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/product_sentiment_machine_hack.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/product_sentiment_machine_hack.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/rossman_store_sales.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/rossman_store_sales.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/santander_customer_transaction.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/santander_customer_transaction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/santander_value_prediction.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/santander_value_prediction.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/sarcastic_headlines.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/sarcastic_headlines.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/sarcos.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/sarcos.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/sst2.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/sst2.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/sst3.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/sst3.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/sst5.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/sst5.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/talkingdata_adtrack_fraud.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/talkingdata_adtrack_fraud.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/telco_customer_churn.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/telco_customer_churn.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/twitter_bots.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/twitter_bots.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/wine_reviews.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/wine_reviews.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/women_clothing_review.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/women_clothing_review.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/yahoo_answers.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/yahoo_answers.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/yelp_review_polarity.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/yelp_review_polarity.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/configs/yelp_reviews.yaml` & `ludwig-0.7.5/ludwig/datasets/configs/yelp_reviews.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/dataset_config.py` & `ludwig-0.7.5/ludwig/datasets/dataset_config.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/kaggle.py` & `ludwig-0.7.5/ludwig/datasets/kaggle.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/adult_census_income.py` & `ludwig-0.7.5/ludwig/datasets/loaders/adult_census_income.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/agnews.py` & `ludwig-0.7.5/ludwig/datasets/loaders/agnews.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/allstate_claims_severity.py` & `ludwig-0.7.5/ludwig/datasets/loaders/allstate_claims_severity.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/creditcard_fraud.py` & `ludwig-0.7.5/ludwig/datasets/loaders/creditcard_fraud.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/dataset_loader.py` & `ludwig-0.7.5/ludwig/datasets/loaders/dataset_loader.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/ethos_binary.py` & `ludwig-0.7.5/ludwig/datasets/loaders/ethos_binary.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/flickr8k.py` & `ludwig-0.7.5/ludwig/datasets/loaders/flickr8k.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/forest_cover.py` & `ludwig-0.7.5/ludwig/datasets/loaders/forest_cover.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/goemotions.py` & `ludwig-0.7.5/ludwig/datasets/loaders/goemotions.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/higgs.py` & `ludwig-0.7.5/ludwig/datasets/loaders/higgs.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/ieee_fraud.py` & `ludwig-0.7.5/ludwig/datasets/loaders/ieee_fraud.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/insurance_lite.py` & `ludwig-0.7.5/ludwig/datasets/loaders/insurance_lite.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/kdd_loader.py` & `ludwig-0.7.5/ludwig/datasets/loaders/kdd_loader.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/mnist.py` & `ludwig-0.7.5/ludwig/datasets/loaders/mnist.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/naval.py` & `ludwig-0.7.5/ludwig/datasets/loaders/naval.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/rossman_store_sales.py` & `ludwig-0.7.5/ludwig/datasets/loaders/rossman_store_sales.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/santander_value_prediction.py` & `ludwig-0.7.5/ludwig/datasets/loaders/santander_value_prediction.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/sarcastic_headlines.py` & `ludwig-0.7.5/ludwig/datasets/loaders/sarcastic_headlines.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/sarcos.py` & `ludwig-0.7.5/ludwig/datasets/loaders/sarcos.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/split_loaders.py` & `ludwig-0.7.5/ludwig/datasets/loaders/split_loaders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/loaders/sst.py` & `ludwig-0.7.5/ludwig/datasets/loaders/sst.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/adult_census_income_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/adult_census_income_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/allstate_claims_severity_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/allstate_claims_severity_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/ames_housing_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/ames_housing_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/bnp_claims_management_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/bnp_claims_management_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/forest_cover_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/forest_cover_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/higgs_best.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/higgs_best.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/higgs_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/higgs_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/ieee_fraud_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/ieee_fraud_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/mercedes_benz_greener_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/mercedes_benz_greener_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/mushroom_edibility_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/mushroom_edibility_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/otto_group_product_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/otto_group_product_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/poker_hand_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/poker_hand_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/model_configs/porto_seguro_safe_driver_default.yaml` & `ludwig-0.7.5/ludwig/datasets/model_configs/porto_seguro_safe_driver_default.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/datasets/utils.py` & `ludwig-0.7.5/ludwig/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/decoders/base.py` & `ludwig-0.7.5/ludwig/decoders/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/decoders/generic_decoders.py` & `ludwig-0.7.5/ludwig/decoders/generic_decoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/decoders/registry.py` & `ludwig-0.7.5/ludwig/decoders/registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/decoders/sequence_decoder_utils.py` & `ludwig-0.7.5/ludwig/decoders/sequence_decoder_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/decoders/sequence_decoders.py` & `ludwig-0.7.5/ludwig/decoders/sequence_decoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/decoders/sequence_tagger.py` & `ludwig-0.7.5/ludwig/decoders/sequence_tagger.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/distributed/__init__.py` & `ludwig-0.7.5/ludwig/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/distributed/_ray_210_compat.py` & `ludwig-0.7.5/ludwig/distributed/_ray_210_compat.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/distributed/base.py` & `ludwig-0.7.5/ludwig/distributed/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/distributed/ddp.py` & `ludwig-0.7.5/ludwig/distributed/ddp.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/distributed/horovod.py` & `ludwig-0.7.5/ludwig/distributed/horovod.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/bag_encoders.py` & `ludwig-0.7.5/ludwig/encoders/bag_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/base.py` & `ludwig-0.7.5/ludwig/encoders/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/category_encoders.py` & `ludwig-0.7.5/ludwig/encoders/category_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/date_encoders.py` & `ludwig-0.7.5/ludwig/encoders/date_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/generic_encoders.py` & `ludwig-0.7.5/ludwig/encoders/generic_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/h3_encoders.py` & `ludwig-0.7.5/ludwig/encoders/h3_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/image/base.py` & `ludwig-0.7.5/ludwig/encoders/image/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/image/torchvision.py` & `ludwig-0.7.5/ludwig/encoders/image/torchvision.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/registry.py` & `ludwig-0.7.5/ludwig/encoders/registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/sequence_encoders.py` & `ludwig-0.7.5/ludwig/encoders/sequence_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/set_encoders.py` & `ludwig-0.7.5/ludwig/encoders/set_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/encoders/text_encoders.py` & `ludwig-0.7.5/ludwig/encoders/text_encoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+import inspect
 import logging
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 import torch
 from torch import nn
 
 from ludwig.api_annotations import DeveloperAPI
@@ -2028,30 +2029,40 @@
 
         self.transformer = FreezeModule(transformer, frozen=not trainable)
         self.reduce_output = reduce_output
         if self.reduce_output != "cls_pooled":
             self.reduce_sequence = SequenceReducer(reduce_mode=reduce_output)
         self.max_sequence_length = max_sequence_length
 
+        # Precompute the set of params that are included in the forward signature of the AutoModel implementation so
+        # we can filter out unused params during the `forward` call.
+        self.forward_kwargs = set(inspect.signature(self.transformer.module.forward).parameters.keys())
+
     def _maybe_resize_token_embeddings(self, transformer, vocab_size: Optional[int] = None):
         """Overridden because AutoModel should use its own vocab size unless vocab size is explicitly specified."""
         if vocab_size is not None:
             transformer.resize_token_embeddings(vocab_size)
             self.vocab_size = vocab_size
         else:
             self.vocab_size = transformer.config.vocab_size
 
     def forward(self, inputs: torch.Tensor, mask: Optional[torch.Tensor] = None):
         if mask is not None:
             mask = mask.to(torch.int32)
-        transformer_outputs = self.transformer.module(
+
+        # The forward signature of AutoModel is not consistent across implementations, so we need to make sure we're
+        # only passing in params included in the forward signature.
+        kwargs = dict(
             input_ids=inputs,
             attention_mask=mask,
             token_type_ids=torch.zeros_like(inputs),
         )
+        kwargs = {k: v for k, v in kwargs.items() if k in self.forward_kwargs}
+
+        transformer_outputs = self.transformer.module(**kwargs)
         if self.reduce_output == "cls_pooled":
             # this works only if the user know that the specific model
             # they want to use has the same outputs of
             # the BERT base class call() function
             hidden = transformer_outputs["pooler_output"]
         else:
             hidden = transformer_outputs["last_hidden_state"]
```

### Comparing `ludwig-0.7.4/ludwig/error.py` & `ludwig-0.7.5/ludwig/error.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/evaluate.py` & `ludwig-0.7.5/ludwig/evaluate.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/experiment.py` & `ludwig-0.7.5/ludwig/experiment.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/explain/captum.py` & `ludwig-0.7.5/ludwig/explain/captum.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/explain/captum_ray.py` & `ludwig-0.7.5/ludwig/explain/captum_ray.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/explain/explainer.py` & `ludwig-0.7.5/ludwig/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/explain/explanation.py` & `ludwig-0.7.5/ludwig/explain/explanation.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/explain/gbm.py` & `ludwig-0.7.5/ludwig/explain/gbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/explain/util.py` & `ludwig-0.7.5/ludwig/explain/util.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/export.py` & `ludwig-0.7.5/ludwig/export.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/audio_feature.py` & `ludwig-0.7.5/ludwig/features/audio_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/bag_feature.py` & `ludwig-0.7.5/ludwig/features/bag_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/base_feature.py` & `ludwig-0.7.5/ludwig/features/base_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/binary_feature.py` & `ludwig-0.7.5/ludwig/features/binary_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/category_feature.py` & `ludwig-0.7.5/ludwig/features/category_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/date_feature.py` & `ludwig-0.7.5/ludwig/features/date_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/feature_registries.py` & `ludwig-0.7.5/ludwig/features/feature_registries.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/feature_utils.py` & `ludwig-0.7.5/ludwig/features/feature_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/h3_feature.py` & `ludwig-0.7.5/ludwig/features/h3_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/image_feature.py` & `ludwig-0.7.5/ludwig/features/image_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/number_feature.py` & `ludwig-0.7.5/ludwig/features/number_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/sequence_feature.py` & `ludwig-0.7.5/ludwig/features/sequence_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/set_feature.py` & `ludwig-0.7.5/ludwig/features/set_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/text_feature.py` & `ludwig-0.7.5/ludwig/features/text_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/timeseries_feature.py` & `ludwig-0.7.5/ludwig/features/timeseries_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/features/vector_feature.py` & `ludwig-0.7.5/ludwig/features/vector_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/globals.py` & `ludwig-0.7.5/ludwig/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-LUDWIG_VERSION = "0.7.4"
+LUDWIG_VERSION = "0.7.5"
 
 MODEL_WEIGHTS_FILE_NAME = "model_weights"
 MODEL_HYPERPARAMETERS_FILE_NAME = "model_hyperparameters.json"
 TRAIN_SET_METADATA_FILE_NAME = "training_set_metadata.json"
 TRAINING_PROGRESS_TRACKER_FILE_NAME = "training_progress.json"
 TRAINING_CHECKPOINTS_DIR_PATH = "training_checkpoints"
```

### Comparing `ludwig-0.7.4/ludwig/hyperopt/execution.py` & `ludwig-0.7.5/ludwig/hyperopt/execution.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/hyperopt/registry.py` & `ludwig-0.7.5/ludwig/hyperopt/registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/hyperopt/run.py` & `ludwig-0.7.5/ludwig/hyperopt/run.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/hyperopt/search_algos.py` & `ludwig-0.7.5/ludwig/hyperopt/search_algos.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/hyperopt/syncer.py` & `ludwig-0.7.5/ludwig/hyperopt/syncer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/hyperopt/utils.py` & `ludwig-0.7.5/ludwig/hyperopt/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/hyperopt_cli.py` & `ludwig-0.7.5/ludwig/hyperopt_cli.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/models/base.py` & `ludwig-0.7.5/ludwig/models/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/models/calibrator.py` & `ludwig-0.7.5/ludwig/models/calibrator.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/models/ecd.py` & `ludwig-0.7.5/ludwig/models/ecd.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/models/embedder.py` & `ludwig-0.7.5/ludwig/models/embedder.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/models/gbm.py` & `ludwig-0.7.5/ludwig/models/gbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/models/inference.py` & `ludwig-0.7.5/ludwig/models/inference.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/models/predictor.py` & `ludwig-0.7.5/ludwig/models/predictor.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/models/registry.py` & `ludwig-0.7.5/ludwig/models/registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/attention_modules.py` & `ludwig-0.7.5/ludwig/modules/attention_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/convolutional_modules.py` & `ludwig-0.7.5/ludwig/modules/convolutional_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/embedding_modules.py` & `ludwig-0.7.5/ludwig/modules/embedding_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/fully_connected_modules.py` & `ludwig-0.7.5/ludwig/modules/fully_connected_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/initializer_modules.py` & `ludwig-0.7.5/ludwig/modules/initializer_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/loss_modules.py` & `ludwig-0.7.5/ludwig/modules/loss_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/lr_scheduler.py` & `ludwig-0.7.5/ludwig/modules/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/metric_modules.py` & `ludwig-0.7.5/ludwig/modules/metric_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/metric_registry.py` & `ludwig-0.7.5/ludwig/modules/metric_registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/mlp_mixer_modules.py` & `ludwig-0.7.5/ludwig/modules/mlp_mixer_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/normalization_modules.py` & `ludwig-0.7.5/ludwig/modules/normalization_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/optimization_modules.py` & `ludwig-0.7.5/ludwig/modules/optimization_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/recurrent_modules.py` & `ludwig-0.7.5/ludwig/modules/recurrent_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/reduction_modules.py` & `ludwig-0.7.5/ludwig/modules/reduction_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/modules/tabnet_modules.py` & `ludwig-0.7.5/ludwig/modules/tabnet_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/predict.py` & `ludwig-0.7.5/ludwig/predict.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/preprocess.py` & `ludwig-0.7.5/ludwig/preprocess.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/profiling/constants.py` & `ludwig-0.7.5/ludwig/profiling/constants.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/profiling/dataset_profile.py` & `ludwig-0.7.5/ludwig/profiling/dataset_profile.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/profiling/metrics.py` & `ludwig-0.7.5/ludwig/profiling/metrics.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/profiling/proto/dataset_profile_pb2.py` & `ludwig-0.7.5/ludwig/profiling/proto/dataset_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/profiling/proto/whylogs_messages_pb2.py` & `ludwig-0.7.5/ludwig/profiling/proto/whylogs_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/profiling/type_inference.py` & `ludwig-0.7.5/ludwig/profiling/type_inference.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/progress_bar.py` & `ludwig-0.7.5/ludwig/progress_bar.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/combiners/common_transformer_options.py` & `ludwig-0.7.5/ludwig/schema/combiners/common_transformer_options.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/combiners/comparator.py` & `ludwig-0.7.5/ludwig/schema/combiners/comparator.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/combiners/concat.py` & `ludwig-0.7.5/ludwig/schema/combiners/concat.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/combiners/project_aggregate.py` & `ludwig-0.7.5/ludwig/schema/combiners/project_aggregate.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/combiners/sequence.py` & `ludwig-0.7.5/ludwig/schema/combiners/sequence.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/combiners/sequence_concat.py` & `ludwig-0.7.5/ludwig/schema/combiners/sequence_concat.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/combiners/tab_transformer.py` & `ludwig-0.7.5/ludwig/schema/combiners/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/combiners/tabnet.py` & `ludwig-0.7.5/ludwig/schema/combiners/tabnet.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/combiners/transformer.py` & `ludwig-0.7.5/ludwig/schema/combiners/transformer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/combiners/utils.py` & `ludwig-0.7.5/ludwig/schema/combiners/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/common_fields.py` & `ludwig-0.7.5/ludwig/schema/common_fields.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/decoders/base.py` & `ludwig-0.7.5/ludwig/schema/decoders/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/decoders/sequence_decoders.py` & `ludwig-0.7.5/ludwig/schema/decoders/sequence_decoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/decoders/utils.py` & `ludwig-0.7.5/ludwig/schema/decoders/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/defaults/ecd.py` & `ludwig-0.7.5/ludwig/schema/defaults/ecd.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/defaults/gbm.py` & `ludwig-0.7.5/ludwig/schema/defaults/gbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/defaults/utils.py` & `ludwig-0.7.5/ludwig/schema/defaults/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/encoders/bag_encoders.py` & `ludwig-0.7.5/ludwig/schema/encoders/bag_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/encoders/base.py` & `ludwig-0.7.5/ludwig/schema/encoders/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/encoders/category_encoders.py` & `ludwig-0.7.5/ludwig/schema/encoders/category_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/encoders/date_encoders.py` & `ludwig-0.7.5/ludwig/schema/encoders/date_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/encoders/h3_encoders.py` & `ludwig-0.7.5/ludwig/schema/encoders/h3_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/encoders/image/base.py` & `ludwig-0.7.5/ludwig/schema/encoders/image/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/encoders/image/torchvision.py` & `ludwig-0.7.5/ludwig/schema/encoders/image/torchvision.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/encoders/sequence_encoders.py` & `ludwig-0.7.5/ludwig/schema/encoders/sequence_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/encoders/set_encoders.py` & `ludwig-0.7.5/ludwig/schema/encoders/set_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/encoders/text_encoders.py` & `ludwig-0.7.5/ludwig/schema/encoders/text_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/encoders/utils.py` & `ludwig-0.7.5/ludwig/schema/encoders/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/__init__.py` & `ludwig-0.7.5/ludwig/schema/features/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/audio_feature.py` & `ludwig-0.7.5/ludwig/schema/features/audio_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/augmentation/image.py` & `ludwig-0.7.5/ludwig/schema/features/augmentation/image.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/augmentation/utils.py` & `ludwig-0.7.5/ludwig/schema/features/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/bag_feature.py` & `ludwig-0.7.5/ludwig/schema/features/bag_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/base.py` & `ludwig-0.7.5/ludwig/schema/features/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/binary_feature.py` & `ludwig-0.7.5/ludwig/schema/features/binary_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/category_feature.py` & `ludwig-0.7.5/ludwig/schema/features/category_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/date_feature.py` & `ludwig-0.7.5/ludwig/schema/features/date_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/h3_feature.py` & `ludwig-0.7.5/ludwig/schema/features/h3_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/image_feature.py` & `ludwig-0.7.5/ludwig/schema/features/image_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/loss/loss.py` & `ludwig-0.7.5/ludwig/schema/features/loss/loss.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/loss/utils.py` & `ludwig-0.7.5/ludwig/schema/features/loss/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/number_feature.py` & `ludwig-0.7.5/ludwig/schema/features/number_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/audio.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/audio.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/bag.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/bag.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/base.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/binary.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/binary.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/category.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/category.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/date.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/date.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/h3.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/h3.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/image.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/number.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/number.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/sequence.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/set.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/set.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/text.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/timeseries.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/timeseries.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/utils.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/preprocessing/vector.py` & `ludwig-0.7.5/ludwig/schema/features/preprocessing/vector.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/sequence_feature.py` & `ludwig-0.7.5/ludwig/schema/features/sequence_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/set_feature.py` & `ludwig-0.7.5/ludwig/schema/features/set_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/text_feature.py` & `ludwig-0.7.5/ludwig/schema/features/text_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/timeseries_feature.py` & `ludwig-0.7.5/ludwig/schema/features/timeseries_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/utils.py` & `ludwig-0.7.5/ludwig/schema/features/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/features/vector_feature.py` & `ludwig-0.7.5/ludwig/schema/features/vector_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/hyperopt/__init__.py` & `ludwig-0.7.5/ludwig/schema/hyperopt/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/hyperopt/executor.py` & `ludwig-0.7.5/ludwig/schema/hyperopt/executor.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/hyperopt/scheduler.py` & `ludwig-0.7.5/ludwig/schema/hyperopt/scheduler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/hyperopt/search_algorithm.py` & `ludwig-0.7.5/ludwig/schema/hyperopt/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/lr_scheduler.py` & `ludwig-0.7.5/ludwig/schema/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/metadata/__init__.py` & `ludwig-0.7.5/ludwig/schema/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/metadata/configs/combiners.yaml` & `ludwig-0.7.5/ludwig/schema/metadata/configs/combiners.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/metadata/configs/common.yaml` & `ludwig-0.7.5/ludwig/schema/metadata/configs/common.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/metadata/configs/decoders.yaml` & `ludwig-0.7.5/ludwig/schema/metadata/configs/decoders.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/metadata/configs/encoders.yaml` & `ludwig-0.7.5/ludwig/schema/metadata/configs/encoders.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/metadata/configs/features.yaml` & `ludwig-0.7.5/ludwig/schema/metadata/configs/features.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/metadata/configs/loss.yaml` & `ludwig-0.7.5/ludwig/schema/metadata/configs/loss.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/metadata/configs/optimizers.yaml` & `ludwig-0.7.5/ludwig/schema/metadata/configs/optimizers.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/metadata/configs/preprocessing.yaml` & `ludwig-0.7.5/ludwig/schema/metadata/configs/preprocessing.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/metadata/configs/trainer.yaml` & `ludwig-0.7.5/ludwig/schema/metadata/configs/trainer.yaml`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/metadata/parameter_metadata.py` & `ludwig-0.7.5/ludwig/schema/metadata/parameter_metadata.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/model_types/base.py` & `ludwig-0.7.5/ludwig/schema/model_types/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/model_types/ecd.py` & `ludwig-0.7.5/ludwig/schema/model_types/ecd.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/model_types/gbm.py` & `ludwig-0.7.5/ludwig/schema/model_types/gbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/model_types/utils.py` & `ludwig-0.7.5/ludwig/schema/model_types/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/optimizers.py` & `ludwig-0.7.5/ludwig/schema/optimizers.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/preprocessing.py` & `ludwig-0.7.5/ludwig/schema/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/split.py` & `ludwig-0.7.5/ludwig/schema/split.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/trainer.py` & `ludwig-0.7.5/ludwig/schema/trainer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/schema/utils.py` & `ludwig-0.7.5/ludwig/schema/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/serve.py` & `ludwig-0.7.5/ludwig/serve.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/train.py` & `ludwig-0.7.5/ludwig/train.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/trainers/base.py` & `ludwig-0.7.5/ludwig/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/trainers/registry.py` & `ludwig-0.7.5/ludwig/trainers/registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/trainers/trainer.py` & `ludwig-0.7.5/ludwig/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/trainers/trainer_lightgbm.py` & `ludwig-0.7.5/ludwig/trainers/trainer_lightgbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/types.py` & `ludwig-0.7.5/ludwig/types.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/algorithms_utils.py` & `ludwig-0.7.5/ludwig/utils/algorithms_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/audio_utils.py` & `ludwig-0.7.5/ludwig/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/augmentation_utils.py` & `ludwig-0.7.5/ludwig/utils/augmentation_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/automl/data_source.py` & `ludwig-0.7.5/ludwig/utils/automl/data_source.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/automl/field_info.py` & `ludwig-0.7.5/ludwig/utils/automl/field_info.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/automl/type_inference.py` & `ludwig-0.7.5/ludwig/utils/automl/type_inference.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/automl/utils.py` & `ludwig-0.7.5/ludwig/utils/automl/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/backward_compatibility.py` & `ludwig-0.7.5/ludwig/utils/backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/batch_size_tuner.py` & `ludwig-0.7.5/ludwig/utils/batch_size_tuner.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/calibration.py` & `ludwig-0.7.5/ludwig/utils/calibration.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/checkpoint_utils.py` & `ludwig-0.7.5/ludwig/utils/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/config_utils.py` & `ludwig-0.7.5/ludwig/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/data_utils.py` & `ludwig-0.7.5/ludwig/utils/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -821,14 +821,17 @@
     elif isinstance(dataset, pd.DataFrame):
         return pd.DataFrame
     elif dd and isinstance(dataset, dd.core.DataFrame):
         return dd.core.DataFrame
     elif isinstance(dataset, dict):
         return dict
     elif isinstance(dataset, str):
+        if dataset.startswith("ludwig://"):
+            return "ludwig"
+
         dataset = dataset.lower()
         if dataset.endswith(".csv"):
             return "csv"
         elif dataset.endswith(".tsv"):
             return "tsv"
         elif dataset.endswith(".json"):
             return "json"
```

### Comparing `ludwig-0.7.4/ludwig/utils/dataframe_utils.py` & `ludwig-0.7.5/ludwig/utils/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/dataset_utils.py` & `ludwig-0.7.5/ludwig/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/date_utils.py` & `ludwig-0.7.5/ludwig/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/defaults.py` & `ludwig-0.7.5/ludwig/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/entmax/__init__.py` & `ludwig-0.7.5/ludwig/utils/entmax/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/entmax/activations.py` & `ludwig-0.7.5/ludwig/utils/entmax/activations.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/entmax/losses.py` & `ludwig-0.7.5/ludwig/utils/entmax/losses.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/entmax/root_finding.py` & `ludwig-0.7.5/ludwig/utils/entmax/root_finding.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/eval_utils.py` & `ludwig-0.7.5/ludwig/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/fs_utils.py` & `ludwig-0.7.5/ludwig/utils/fs_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/gbm_utils.py` & `ludwig-0.7.5/ludwig/utils/gbm_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/h3_util.py` & `ludwig-0.7.5/ludwig/utils/h3_util.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/heuristics.py` & `ludwig-0.7.5/ludwig/utils/heuristics.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/hf_utils.py` & `ludwig-0.7.5/ludwig/utils/hf_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/horovod_utils.py` & `ludwig-0.7.5/ludwig/utils/horovod_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/html_utils.py` & `ludwig-0.7.5/ludwig/utils/html_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/image_utils.py` & `ludwig-0.7.5/ludwig/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/inference_utils.py` & `ludwig-0.7.5/ludwig/utils/inference_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/loss_utils.py` & `ludwig-0.7.5/ludwig/utils/loss_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/math_utils.py` & `ludwig-0.7.5/ludwig/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/metric_utils.py` & `ludwig-0.7.5/ludwig/utils/metric_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/metrics_printed_table.py` & `ludwig-0.7.5/ludwig/utils/metrics_printed_table.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/misc_utils.py` & `ludwig-0.7.5/ludwig/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/neuropod_utils.py` & `ludwig-0.7.5/ludwig/utils/neuropod_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/nlp_utils.py` & `ludwig-0.7.5/ludwig/utils/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/numerical_test_utils.py` & `ludwig-0.7.5/ludwig/utils/numerical_test_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/output_feature_utils.py` & `ludwig-0.7.5/ludwig/utils/output_feature_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/package_utils.py` & `ludwig-0.7.5/ludwig/utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/print_utils.py` & `ludwig-0.7.5/ludwig/utils/print_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/registry.py` & `ludwig-0.7.5/ludwig/utils/registry.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/server_utils.py` & `ludwig-0.7.5/ludwig/utils/server_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/state_dict_backward_compatibility.py` & `ludwig-0.7.5/ludwig/utils/state_dict_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/strings_utils.py` & `ludwig-0.7.5/ludwig/utils/strings_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/structural_warning.py` & `ludwig-0.7.5/ludwig/utils/structural_warning.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/system_utils.py` & `ludwig-0.7.5/ludwig/utils/system_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/time_utils.py` & `ludwig-0.7.5/ludwig/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/tokenizers.py` & `ludwig-0.7.5/ludwig/utils/tokenizers.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/torch_utils.py` & `ludwig-0.7.5/ludwig/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/trainer_utils.py` & `ludwig-0.7.5/ludwig/utils/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/triton_utils.py` & `ludwig-0.7.5/ludwig/utils/triton_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/types.py` & `ludwig-0.7.5/ludwig/utils/types.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/version_transformation.py` & `ludwig-0.7.5/ludwig/utils/version_transformation.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/utils/visualization_utils.py` & `ludwig-0.7.5/ludwig/utils/visualization_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig/visualize.py` & `ludwig-0.7.5/ludwig/visualize.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig.egg-info/PKG-INFO` & `ludwig-0.7.5/ludwig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ludwig
-Version: 0.7.4
+Version: 0.7.5
 Summary: Declarative machine learning: End-to-end machine learning pipelines using data-driven configurations.
 Home-page: https://github.com/ludwig-ai/ludwig
 Author: Piero Molino
 Author-email: piero.molino@gmail.com
 License: Apache 2.0
 Download-URL: https://pypi.org/project/ludwig/
 Description: ![Ludwig logo](https://github.com/ludwig-ai/ludwig-docs/raw/master/docs/images/ludwig_hero.png "Ludwig logo")
```

### Comparing `ludwig-0.7.4/ludwig.egg-info/SOURCES.txt` & `ludwig-0.7.5/ludwig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/ludwig.egg-info/requires.txt` & `ludwig-0.7.5/ludwig.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 torchvision
 transformers<4.22,>=4.10.1
 spacy>=2.3
 PyYAML>=3.12
 absl-py
 kaggle
 requests
-tables
 fsspec[http]
 dataclasses-json
 jsonschema<4.7,>=4.5.0
 marshmallow
 marshmallow-jsonschema
 marshmallow-dataclass==8.5.4
 tensorboard
```

### Comparing `ludwig-0.7.4/requirements.txt` & `ludwig-0.7.5/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 torchvision
 transformers>=4.10.1,<4.22
 spacy>=2.3
 PyYAML>=3.12
 absl-py
 kaggle
 requests
-tables
 fsspec[http]
 dataclasses-json
 jsonschema>=4.5.0,<4.7
 marshmallow
 marshmallow-jsonschema
 marshmallow-dataclass==8.5.4
 tensorboard
```

### Comparing `ludwig-0.7.4/requirements_test.txt` & `ludwig-0.7.5/requirements_test.txt`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/setup.py` & `ludwig-0.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 extra_requirements["full"] = [item for sublist in extra_requirements.values() for item in sublist]
 
 with open(path.join(here, "requirements_test.txt"), encoding="utf-8") as f:
     extra_requirements["test"] = extra_requirements["full"] + [line.strip() for line in f if line]
 
 setup(
     name="ludwig",
-    version="0.7.4",
+    version="0.7.5",
     description="Declarative machine learning: End-to-end machine learning pipelines using data-driven configurations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ludwig-ai/ludwig",
     download_url="https://pypi.org/project/ludwig/",
     author="Piero Molino",
     author_email="piero.molino@gmail.com",
```

### Comparing `ludwig-0.7.4/tests/integration_tests/parameter_update_utils.py` & `ludwig-0.7.5/tests/integration_tests/parameter_update_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/synthetic_test_data.py` & `ludwig-0.7.5/tests/integration_tests/synthetic_test_data.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_api.py` & `ludwig-0.7.5/tests/integration_tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_audio_feature.py` & `ludwig-0.7.5/tests/integration_tests/test_audio_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_automl.py` & `ludwig-0.7.5/tests/integration_tests/test_automl.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_cache_manager.py` & `ludwig-0.7.5/tests/integration_tests/test_cache_manager.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_cached_preprocessing.py` & `ludwig-0.7.5/tests/integration_tests/test_cached_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_class_imbalance_feature.py` & `ludwig-0.7.5/tests/integration_tests/test_class_imbalance_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_cli.py` & `ludwig-0.7.5/tests/integration_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_collect.py` & `ludwig-0.7.5/tests/integration_tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_config_global_defaults.py` & `ludwig-0.7.5/tests/integration_tests/test_config_global_defaults.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_contrib_aim.py` & `ludwig-0.7.5/tests/integration_tests/test_contrib_aim.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_contrib_comet.py` & `ludwig-0.7.5/tests/integration_tests/test_contrib_comet.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_contrib_wandb.py` & `ludwig-0.7.5/tests/integration_tests/test_contrib_wandb.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_custom_components.py` & `ludwig-0.7.5/tests/integration_tests/test_custom_components.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_dependencies.py` & `ludwig-0.7.5/tests/integration_tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_experiment.py` & `ludwig-0.7.5/tests/integration_tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_explain.py` & `ludwig-0.7.5/tests/integration_tests/test_explain.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_gbm.py` & `ludwig-0.7.5/tests/integration_tests/test_gbm.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_graph_execution.py` & `ludwig-0.7.5/tests/integration_tests/test_graph_execution.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_horovod.py` & `ludwig-0.7.5/tests/integration_tests/test_horovod.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_hyperopt.py` & `ludwig-0.7.5/tests/integration_tests/test_hyperopt.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_hyperopt_ray.py` & `ludwig-0.7.5/tests/integration_tests/test_hyperopt_ray.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_hyperopt_ray_horovod.py` & `ludwig-0.7.5/tests/integration_tests/test_hyperopt_ray_horovod.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_input_feature_tied.py` & `ludwig-0.7.5/tests/integration_tests/test_input_feature_tied.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_kfold_cv.py` & `ludwig-0.7.5/tests/integration_tests/test_kfold_cv.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_missing_value_strategy.py` & `ludwig-0.7.5/tests/integration_tests/test_missing_value_strategy.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_mlflow.py` & `ludwig-0.7.5/tests/integration_tests/test_mlflow.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_model_save_and_load.py` & `ludwig-0.7.5/tests/integration_tests/test_model_save_and_load.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_model_training_options.py` & `ludwig-0.7.5/tests/integration_tests/test_model_training_options.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_neuropod.py` & `ludwig-0.7.5/tests/integration_tests/test_neuropod.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_number_feature.py` & `ludwig-0.7.5/tests/integration_tests/test_number_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_postprocessing.py` & `ludwig-0.7.5/tests/integration_tests/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_preprocessing.py` & `ludwig-0.7.5/tests/integration_tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_ray.py` & `ludwig-0.7.5/tests/integration_tests/test_ray.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_reducers.py` & `ludwig-0.7.5/tests/integration_tests/test_reducers.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_regularizers.py` & `ludwig-0.7.5/tests/integration_tests/test_regularizers.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_remote.py` & `ludwig-0.7.5/tests/integration_tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_reproducibility.py` & `ludwig-0.7.5/tests/integration_tests/test_reproducibility.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_sequence_decoders.py` & `ludwig-0.7.5/tests/integration_tests/test_sequence_decoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_sequence_encoders.py` & `ludwig-0.7.5/tests/integration_tests/test_sequence_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_sequence_features.py` & `ludwig-0.7.5/tests/integration_tests/test_sequence_features.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_server.py` & `ludwig-0.7.5/tests/integration_tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_simple_features.py` & `ludwig-0.7.5/tests/integration_tests/test_simple_features.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_timeseries_feature.py` & `ludwig-0.7.5/tests/integration_tests/test_timeseries_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_torchscript.py` & `ludwig-0.7.5/tests/integration_tests/test_torchscript.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_trainer.py` & `ludwig-0.7.5/tests/integration_tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_triton.py` & `ludwig-0.7.5/tests/integration_tests/test_triton.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_visualization.py` & `ludwig-0.7.5/tests/integration_tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/test_visualization_api.py` & `ludwig-0.7.5/tests/integration_tests/test_visualization_api.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/integration_tests/utils.py` & `ludwig-0.7.5/tests/integration_tests/utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/automl/test_base_config.py` & `ludwig-0.7.5/tests/ludwig/automl/test_base_config.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/automl/test_data_source.py` & `ludwig-0.7.5/tests/ludwig/automl/test_data_source.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/automl/test_tune_config.py` & `ludwig-0.7.5/tests/ludwig/automl/test_tune_config.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/automl/test_utils.py` & `ludwig-0.7.5/tests/ludwig/automl/test_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/datasets/__init__.py` & `ludwig-0.7.5/tests/ludwig/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/datasets/check_dead_links.py` & `ludwig-0.7.5/tests/ludwig/datasets/check_dead_links.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/datasets/download_all_datasets.py` & `ludwig-0.7.5/tests/ludwig/datasets/download_all_datasets.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/datasets/test_dataset_configs.py` & `ludwig-0.7.5/tests/ludwig/datasets/test_dataset_configs.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/datasets/test_datasets.py` & `ludwig-0.7.5/tests/ludwig/datasets/test_datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 def test_get_dataset_buffer():
     buffer = ludwig.datasets.get_buffer("iris")
 
     assert isinstance(buffer, io.BytesIO)
 
 
-def test_preprocess_dataset_uri(tmpdir):
+def test_train_dataset_uri(tmpdir):
     input_df = pd.DataFrame(
         {
             "input": ["a", "b", "a", "b", "a", "b", "c", "c", "a", "b"],
             "output": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
             "split": [0, 0, 0, 0, 0, 0, 0, 1, 2, 2],
         }
     )
@@ -151,41 +151,50 @@
         download_urls=["file://" + archive_filename],
     )
 
     model_config = {
         "input_features": [{"name": "input", "type": "category"}],
         "output_features": [{"name": "output", "type": "number"}],
         "preprocessing": {"split": {"type": "fixed"}},
+        "combiner": {"type": "concat", "fc_size": 14},
+        "trainer": {"batch_size": 8, "epochs": 1},
     }
 
     ludwig.datasets._get_dataset_configs.cache_clear()
     with mock.patch("ludwig.datasets._load_dataset_config", return_value=config):
         with mock.patch("ludwig.datasets.loaders.dataset_loader.get_default_cache_location", return_value=str(tmpdir)):
             model = LudwigModel(model_config, backend="local")
 
-            proc_result = model.preprocess(dataset=f"ludwig://{dataset_name}")
+            results = model.train(dataset=f"ludwig://{dataset_name}")
+            proc_result = results.preprocessed_data
             train_df1 = proc_result.training_set.to_df()
             val_df1 = proc_result.validation_set.to_df()
             test_df1 = proc_result.test_set.to_df()
 
             assert len(train_df1) == 7
             assert len(val_df1) == 1
             assert len(test_df1) == 2
 
-            proc_result_split = model.preprocess(
+            results = model.train(
                 training_set=f"ludwig://{dataset_name}",
                 validation_set=f"ludwig://{dataset_name}",
                 test_set=f"ludwig://{dataset_name}",
             )
+            proc_result_split = results.preprocessed_data
             train_df2 = proc_result_split.training_set.to_df()
             val_df2 = proc_result_split.validation_set.to_df()
             test_df2 = proc_result_split.test_set.to_df()
 
             assert len(train_df2) == 7
             assert len(val_df2) == 1
             assert len(test_df2) == 2
 
-            assert train_df1.equals(train_df2)
-            assert val_df1.equals(val_df2)
-            assert test_df1.equals(test_df2)
+            sort_col = train_df1.columns[-1]
+
+            def sort_df(df):
+                return df.sort_values(by=[sort_col]).reset_index(drop=True)
+
+            assert sort_df(train_df1).equals(sort_df(train_df2))
+            assert sort_df(val_df1).equals(sort_df(val_df2))
+            assert sort_df(test_df1).equals(sort_df(test_df2))
 
     ludwig.datasets._get_dataset_configs.cache_clear()
```

### Comparing `ludwig-0.7.4/tests/ludwig/datasets/test_model_configs.py` & `ludwig-0.7.5/tests/ludwig/datasets/test_model_configs.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/encoders/test_bag_encoders.py` & `ludwig-0.7.5/tests/ludwig/encoders/test_bag_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/encoders/test_category_encoders.py` & `ludwig-0.7.5/tests/ludwig/encoders/test_category_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/encoders/test_date_encoders.py` & `ludwig-0.7.5/tests/ludwig/encoders/test_date_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/encoders/test_generic_encoders.py` & `ludwig-0.7.5/tests/ludwig/encoders/test_generic_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/encoders/test_h3_encoders.py` & `ludwig-0.7.5/tests/ludwig/encoders/test_h3_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/encoders/test_image_encoders.py` & `ludwig-0.7.5/tests/ludwig/encoders/test_image_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/encoders/test_sequence_encoders.py` & `ludwig-0.7.5/tests/ludwig/encoders/test_sequence_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/encoders/test_set_encoders.py` & `ludwig-0.7.5/tests/ludwig/encoders/test_set_encoders.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/encoders/test_text_encoders.py` & `ludwig-0.7.5/tests/ludwig/encoders/test_text_encoders.py`

 * *Files 14% similar despite different names*

```diff
@@ -105,14 +105,59 @@
         )
 
     # Validate the model can be loaded.
     # This ensures that the config reflects the internal architecture of the encoder.
     LudwigModel.load(os.path.join(results_dir, "model"))
 
 
+@pytest.mark.parametrize(
+    "pretrained_model_name_or_path",
+    [
+        "hf-internal-testing/tiny-random-bloom",
+        "hf-internal-testing/tiny-random-OPTModel",
+        "hf-internal-testing/tiny-random-GPTJModel",
+    ],
+)
+def test_hf_ludwig_model_auto_transformers(tmpdir, csv_filename, pretrained_model_name_or_path):
+    """Tests different AutoModel types to ensure our wrapper handles them correctly.
+
+    This is needed because different PretrainedModel implemetnations have different input / output signatures.
+    """
+    input_features = [
+        text_feature(
+            preprocessing={
+                "max_sequence_length": 10,
+            },
+            encoder={
+                "vocab_size": 30,
+                "min_len": 1,
+                "type": "auto_transformer",
+                "pretrained_model_name_or_path": pretrained_model_name_or_path,
+                "use_pretrained": True,
+            },
+        )
+    ]
+    output_features = [category_feature(decoder={"vocab_size": 2})]
+    rel_path = generate_data(input_features, output_features, csv_filename)
+
+    config = {
+        "input_features": input_features,
+        "output_features": output_features,
+        TRAINER: {"train_steps": 1},
+    }
+    model = LudwigModel(config=config, backend=LocalTestBackend())
+
+    # Validates that the defaults associated with the encoder are compatible with Ludwig training.
+    with mock.patch(
+        "ludwig.encoders.text_encoders.load_pretrained_hf_model_with_hub_fallback",
+        side_effect=_load_pretrained_hf_model_no_weights,
+    ):
+        model.train(dataset=rel_path, output_directory=tmpdir)
+
+
 @pytest.mark.parametrize("trainable", [True, False])
 def test_distilbert_param_updates(trainable: bool):
     max_sequence_length = 20
     distil_bert_encoder = text_encoders.DistilBERTEncoder(
         use_pretrained=False,
         max_sequence_length=max_sequence_length,
         trainable=trainable,
```

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_audio_feature.py` & `ludwig-0.7.5/tests/ludwig/features/test_audio_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_bag_feature.py` & `ludwig-0.7.5/tests/ludwig/features/test_bag_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_binary_feature.py` & `ludwig-0.7.5/tests/ludwig/features/test_binary_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_category_feature.py` & `ludwig-0.7.5/tests/ludwig/features/test_category_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_date_feature.py` & `ludwig-0.7.5/tests/ludwig/features/test_date_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_feature_utils.py` & `ludwig-0.7.5/tests/ludwig/features/test_feature_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_h3_feature.py` & `ludwig-0.7.5/tests/ludwig/features/test_h3_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_image_feature.py` & `ludwig-0.7.5/tests/ludwig/features/test_image_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_number_feature.py` & `ludwig-0.7.5/tests/ludwig/features/test_number_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_sequence_features.py` & `ludwig-0.7.5/tests/ludwig/features/test_sequence_features.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_set_feature.py` & `ludwig-0.7.5/tests/ludwig/features/test_set_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_text_feature.py` & `ludwig-0.7.5/tests/ludwig/features/test_text_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/features/test_timeseries_feature.py` & `ludwig-0.7.5/tests/ludwig/features/test_timeseries_feature.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/models/__init__.py` & `ludwig-0.7.5/tests/ludwig/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/models/test_trainable_image_layers.py` & `ludwig-0.7.5/tests/ludwig/models/test_trainable_image_layers.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/models/test_training_determinism.py` & `ludwig-0.7.5/tests/ludwig/models/test_training_determinism.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/models/test_training_success.py` & `ludwig-0.7.5/tests/ludwig/models/test_training_success.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/__init__.py` & `ludwig-0.7.5/tests/ludwig/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_attention.py` & `ludwig-0.7.5/tests/ludwig/modules/test_attention.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_convolutional_modules.py` & `ludwig-0.7.5/tests/ludwig/modules/test_convolutional_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_embedding_modules.py` & `ludwig-0.7.5/tests/ludwig/modules/test_embedding_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_encoder.py` & `ludwig-0.7.5/tests/ludwig/modules/test_encoder.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_fully_connected_modules.py` & `ludwig-0.7.5/tests/ludwig/modules/test_fully_connected_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_initializer_modules.py` & `ludwig-0.7.5/tests/ludwig/modules/test_initializer_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_loss_modules.py` & `ludwig-0.7.5/tests/ludwig/modules/test_loss_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_lr_scheduler.py` & `ludwig-0.7.5/tests/ludwig/modules/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_metric_modules.py` & `ludwig-0.7.5/tests/ludwig/modules/test_metric_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_mlp_mixer_modules.py` & `ludwig-0.7.5/tests/ludwig/modules/test_mlp_mixer_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_normalization_modules.py` & `ludwig-0.7.5/tests/ludwig/modules/test_normalization_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_recurrent_modules.py` & `ludwig-0.7.5/tests/ludwig/modules/test_recurrent_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_reduction_modules.py` & `ludwig-0.7.5/tests/ludwig/modules/test_reduction_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_tabnet_modules.py` & `ludwig-0.7.5/tests/ludwig/modules/test_tabnet_modules.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/modules/test_utils.py` & `ludwig-0.7.5/tests/ludwig/modules/test_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/__init__.py` & `ludwig-0.7.5/tests/ludwig/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_backward_compatibility.py` & `ludwig-0.7.5/tests/ludwig/utils/test_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_calibration.py` & `ludwig-0.7.5/tests/ludwig/utils/test_calibration.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_class_balancing.py` & `ludwig-0.7.5/tests/ludwig/utils/test_class_balancing.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_config_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_config_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_data_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_dataframe_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_dataset_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_defaults.py` & `ludwig-0.7.5/tests/ludwig/utils/test_defaults.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_errors.py` & `ludwig-0.7.5/tests/ludwig/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_fs_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_fs_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_heuristics.py` & `ludwig-0.7.5/tests/ludwig/utils/test_heuristics.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_hf_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_hf_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_hyperopt_ray_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_hyperopt_ray_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_image_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_metric_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_metric_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_normalization.py` & `ludwig-0.7.5/tests/ludwig/utils/test_normalization.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_numerical_test_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_numerical_test_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_output_feature_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_output_feature_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_server_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_server_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_state_dict_backward_compatibility.py` & `ludwig-0.7.5/tests/ludwig/utils/test_state_dict_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_strings_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_strings_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_tokenizers.py` & `ludwig-0.7.5/tests/ludwig/utils/test_tokenizers.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_torch_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_torch_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_trainer_utils.py` & `ludwig-0.7.5/tests/ludwig/utils/test_trainer_utils.py`

 * *Files identical despite different names*

### Comparing `ludwig-0.7.4/tests/ludwig/utils/test_version_transformation.py` & `ludwig-0.7.5/tests/ludwig/utils/test_version_transformation.py`

 * *Files identical despite different names*

