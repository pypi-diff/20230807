# Comparing `tmp/lightwood-23.7.1.0.tar.gz` & `tmp/lightwood-23.8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightwood-23.7.1.0.tar", last modified: Mon Jul  3 13:10:54 2023, max compression
+gzip compressed data, was "lightwood-23.8.1.0.tar", last modified: Mon Aug  7 15:56:05 2023, max compression
```

## Comparing `lightwood-23.7.1.0.tar` & `lightwood-23.8.1.0.tar`

### file list

```diff
@@ -1,163 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.258831 lightwood-23.7.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-03 13:10:54.258831 lightwood-23.7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/explain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood/analysis/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/acc_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/conf_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/pyod.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood/analysis/nc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/icp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood/analysis/nn_conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nn_conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nn_conf/temp_scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/api/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/api/high_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    51442 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/api/json_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    25300 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/data/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/data/encoded_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/data/timeseries_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/data/timeseries_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/array/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/array/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/array/ts_cat_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/array/ts_num_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/audio/mfcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/categorical/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/multihot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/onehot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/simple_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/datetime/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/identity/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/image/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/image/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/image/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/image/helpers/img_to_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/image/img_2_vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/numeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/numeric/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/numeric/ts_numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.250831 lightwood-23.7.1.0/lightwood/encoder/text/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.250831 lightwood-23.7.1.0/lightwood/encoder/text/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/helpers/pretrained_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/short.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/tfidf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/vocab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.250831 lightwood-23.7.1.0/lightwood/encoder/time_series/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.250831 lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23548 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.250831 lightwood-23.7.1.0/lightwood/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/best_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/mode_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/ts_stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/weighted_mean_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.254831 lightwood-23.7.1.0/lightwood/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.254831 lightwood-23.7.1.0/lightwood/mixer/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/arima.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/ets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.258831 lightwood-23.7.1.0/lightwood/mixer/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/ar_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/default_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/qclassic_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/ranger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/residual_net.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/lightgbm_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/neural.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/neural_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10710 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/nhits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/prophet.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/qclassic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/sktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-03 13:10:53.000000 lightwood-23.7.1.0/lightwood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-03 13:10:54.000000 lightwood-23.7.1.0/lightwood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:10:53.000000 lightwood-23.7.1.0/lightwood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-03 13:10:53.000000 lightwood-23.7.1.0/lightwood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 13:10:53.000000 lightwood-23.7.1.0/lightwood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:10:54.258831 lightwood-23.7.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.676441 lightwood-23.8.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-08-07 15:56:05.676441 lightwood-23.8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.664441 lightwood-23.8.1.0/lightwood/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.664441 lightwood-23.8.1.0/lightwood/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/explain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.668441 lightwood-23.8.1.0/lightwood/analysis/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/helpers/acc_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/helpers/conf_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/helpers/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/helpers/pyod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/helpers/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.668441 lightwood-23.8.1.0/lightwood/analysis/nc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/nc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/nc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29295 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/nc/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/nc/icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/nc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/nc/nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/nc/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/nc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.668441 lightwood-23.8.1.0/lightwood/analysis/nn_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/nn_conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/analysis/nn_conf/temp_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.668441 lightwood-23.8.1.0/lightwood/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/api/high_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30861 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/api/json_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25300 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.668441 lightwood-23.8.1.0/lightwood/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/data/encoded_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/data/timeseries_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/data/timeseries_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.668441 lightwood-23.8.1.0/lightwood/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.668441 lightwood-23.8.1.0/lightwood/encoder/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/array/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/array/ts_cat_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/array/ts_num_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.668441 lightwood-23.8.1.0/lightwood/encoder/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/audio/mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.668441 lightwood-23.8.1.0/lightwood/encoder/categorical/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/categorical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/categorical/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/categorical/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/categorical/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/categorical/multihot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/categorical/onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/categorical/simple_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.668441 lightwood-23.8.1.0/lightwood/encoder/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/datetime/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.668441 lightwood-23.8.1.0/lightwood/encoder/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/identity/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.672441 lightwood-23.8.1.0/lightwood/encoder/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.672441 lightwood-23.8.1.0/lightwood/encoder/image/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/image/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/image/helpers/img_to_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/image/img_2_vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.672441 lightwood-23.8.1.0/lightwood/encoder/numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/numeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/numeric/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/numeric/ts_numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.672441 lightwood-23.8.1.0/lightwood/encoder/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.672441 lightwood-23.8.1.0/lightwood/encoder/text/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/text/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/text/helpers/pretrained_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/text/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/text/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/text/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/text/short.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/text/tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/text/vocab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.672441 lightwood-23.8.1.0/lightwood/encoder/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/time_series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.672441 lightwood-23.8.1.0/lightwood/encoder/time_series/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/time_series/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/time_series/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23548 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/time_series/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/encoder/time_series/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.672441 lightwood-23.8.1.0/lightwood/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/ensemble/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/ensemble/best_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/ensemble/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/ensemble/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/ensemble/mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/ensemble/mode_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/ensemble/stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/ensemble/ts_stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/ensemble/weighted_mean_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.672441 lightwood-23.8.1.0/lightwood/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/helpers/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.676441 lightwood-23.8.1.0/lightwood/mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/arima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/ets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.676441 lightwood-23.8.1.0/lightwood/mixer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/helpers/ar_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/helpers/default_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/helpers/qclassic_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/helpers/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/helpers/residual_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/helpers/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/lightgbm_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/neural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/neural_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/prophet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/qclassic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/sktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/lightwood/mixer/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:56:05.664441 lightwood-23.8.1.0/lightwood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-08-07 15:56:05.000000 lightwood-23.8.1.0/lightwood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-08-07 15:56:05.000000 lightwood-23.8.1.0/lightwood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:56:05.000000 lightwood-23.8.1.0/lightwood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-07 15:56:05.000000 lightwood-23.8.1.0/lightwood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 15:56:05.000000 lightwood-23.8.1.0/lightwood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:56:05.676441 lightwood-23.8.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-07 15:55:52.000000 lightwood-23.8.1.0/setup.py
```

### Comparing `lightwood-23.7.1.0/LICENSE` & `lightwood-23.8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/PKG-INFO` & `lightwood-23.8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.7.1.0
+Version: 23.8.1.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -214,17 +214,17 @@
         * [Lightwood License](https://github.com/mindsdb/lightwood/blob/master/LICENSE)
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: image
 Provides-Extra: extra
-Provides-Extra: dev
-Provides-Extra: extra_ts
 Provides-Extra: xai
-Provides-Extra: audio
 Provides-Extra: quantum
+Provides-Extra: extra_ts
+Provides-Extra: dev
+Provides-Extra: audio
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.7.1.0/README.md` & `lightwood-23.8.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/__init__.py` & `lightwood-23.8.1.0/lightwood/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/analyze.py` & `lightwood-23.8.1.0/lightwood/analysis/analyze.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/base.py` & `lightwood-23.8.1.0/lightwood/analysis/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/explain.py` & `lightwood-23.8.1.0/lightwood/analysis/explain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Optional, List, Dict
 import torch
 import pandas as pd
 
 from dataprep_ml import StatisticalAnalysis
 
-from lightwood.helpers.log import log
+from lightwood.helpers.log import log, timed
 from lightwood.api.types import ProblemDefinition, PredictionArguments
 from lightwood.helpers.ts import get_inferred_timestamps
 from lightwood.analysis.base import BaseAnalysisBlock
 
 
+@timed
 def explain(data: pd.DataFrame,
             encoded_data: torch.Tensor,
             predictions: pd.DataFrame,
             target_name: str,
             target_dtype: str,
 
             problem_definition: ProblemDefinition,
```

### Comparing `lightwood-23.7.1.0/lightwood/analysis/helpers/acc_stats.py` & `lightwood-23.8.1.0/lightwood/analysis/helpers/acc_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/helpers/conf_stats.py` & `lightwood-23.8.1.0/lightwood/analysis/helpers/conf_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/helpers/feature_importance.py` & `lightwood-23.8.1.0/lightwood/analysis/helpers/feature_importance.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/helpers/pyod.py` & `lightwood-23.8.1.0/lightwood/analysis/helpers/pyod.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/helpers/shap.py` & `lightwood-23.8.1.0/lightwood/analysis/helpers/shap.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/nc/base.py` & `lightwood-23.8.1.0/lightwood/analysis/nc/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/nc/calibrate.py` & `lightwood-23.8.1.0/lightwood/analysis/nc/calibrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,18 +196,19 @@
                         norm_input = EncodedDs(ns.encoded_val_data.encoders, norm_input_df, ns.target)
                         norm_cache = group_normalizer(norm_input, args=PredictionArguments())
                         icp_df[f'__norm_{ns.target}'] = norm_cache
 
                     # save relevant predictions in the caches, then calibrate the ICP
                     pred_cache = icp_df.pop(f'__predicted_{ns.target}').values
                     if ns.is_multi_ts and ns.is_classification:
-                        # output['label_encoders'].transform(preds.reshape(-1, 1))
                         pred_cache = output['label_encoders'].transform([[p[0] for p in pred_cache]])
                     elif ns.is_multi_ts:
                         pred_cache = np.array([np.array(p) for p in pred_cache])
+                    elif ns.is_classification:
+                        pred_cache = output['label_encoders'].transform(pred_cache.reshape(-1, 1))
 
                     icps[tuple(group)].nc_function.model.prediction_cache = pred_cache
                     icp_df, y = clean_df(icp_df, ns, output.get('label_encoders', None))
                     if icps[tuple(group)].nc_function.normalizer is not None:
                         icps[tuple(group)].nc_function.normalizer.prediction_cache = icp_df.pop(
                             f'__norm_{ns.target}').values
```

### Comparing `lightwood-23.7.1.0/lightwood/analysis/nc/icp.py` & `lightwood-23.8.1.0/lightwood/analysis/nc/icp.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/nc/metrics.py` & `lightwood-23.8.1.0/lightwood/analysis/nc/metrics.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/nc/nc.py` & `lightwood-23.8.1.0/lightwood/analysis/nc/nc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/nc/norm.py` & `lightwood-23.8.1.0/lightwood/analysis/nc/norm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/nc/util.py` & `lightwood-23.8.1.0/lightwood/analysis/nc/util.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/analysis/nn_conf/temp_scale.py` & `lightwood-23.8.1.0/lightwood/analysis/nn_conf/temp_scale.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/api/__init__.py` & `lightwood-23.8.1.0/lightwood/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/api/high_level.py` & `lightwood-23.8.1.0/lightwood/api/high_level.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import os
-from types import ModuleType
 from typing import Union
 import dill
 import pandas as pd
 from lightwood.api.types import JsonAI, ProblemDefinition
 from dataprep_ml.insights import statistical_analysis
 from type_infer.infer import infer_types
 from lightwood.api.predictor import PredictorInterface
 from lightwood.api.json_ai import generate_json_ai
-import tempfile
-from lightwood.api.json_ai import code_from_json_ai as _code_from_json_ai
-import importlib.util
+from lightwood.helpers.codegen import code_from_json_ai as _code_from_json_ai, _module_from_code, _predictor_from_code
 import sys
-import random
-import string
 import gc
 import time
 from lightwood.helpers.log import log
 from shutil import copyfile
 
 
 def load_custom_module(file_path: str):
@@ -103,18 +98,15 @@
 
 def predictor_from_code(code: str) -> PredictorInterface:
     """
     :param code: The ``Predictor``'s code in text form
 
     :returns: A lightwood ``Predictor`` object
     """
-    module_name = ''.join(random.choices(string.ascii_uppercase + string.digits, k=12))
-    module_name += str(time.time()).replace('.', '')
-    predictor = _module_from_code(code, module_name).Predictor()
-    return predictor
+    return _predictor_from_code(code)
 
 
 def code_from_problem(df: pd.DataFrame, problem_definition: Union[ProblemDefinition, dict]) -> str:
     """
     :param df: The raw data
     :param problem_definition: The manual specifications for your predictive problem
 
@@ -158,39 +150,14 @@
         _module_from_code(code, module_name)
         with open(state_file, 'rb') as fp:
             predictor = dill.load(fp)
 
     return predictor
 
 
-def _module_from_code(code: str, module_name: str) -> ModuleType:
-    """
-    Create a python module (containing the generated ``Predictor`` class) from the code. This is both a python object and an associated temporary file on your filesystem
-
-    :param code: The ``Predictor``'s code in text form
-    :param module_name: The name of the newly created module
-
-    :returns: A python module object
-    """ # noqa
-    dirname = tempfile.gettempdir()
-    filename = os.urandom(24).hex() + str(time.time()).replace('.', '') + '.py'
-    path = os.path.join(dirname, filename)
-    if 'LIGHTWOOD_DEV_SAVE_TO' in os.environ:
-        path = os.environ['LIGHTWOOD_DEV_SAVE_TO']
-
-    with open(path, 'wb') as fp:
-        fp.write(code.encode('utf-8'))
-        spec = importlib.util.spec_from_file_location(module_name, fp.name)
-        temp_module = importlib.util.module_from_spec(spec)
-        sys.modules[module_name] = temp_module
-        spec.loader.exec_module(temp_module)
-
-    return temp_module
-
-
 def predictor_from_json_ai(json_ai: JsonAI) -> PredictorInterface:
     """
     Creates a ready-to-train ``Predictor`` object based on the details you specified inside your JsonAI.
 
     :param json_ai: A ``JsonAI`` object
 
     :returns: A lightwood ``Predictor`` object
```

### Comparing `lightwood-23.7.1.0/lightwood/api/predictor.py` & `lightwood-23.8.1.0/lightwood/api/predictor.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/api/types.py` & `lightwood-23.8.1.0/lightwood/api/types.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/data/encoded_ds.py` & `lightwood-23.8.1.0/lightwood/data/encoded_ds.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/data/timeseries_analyzer.py` & `lightwood-23.8.1.0/lightwood/data/timeseries_analyzer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/data/timeseries_transform.py` & `lightwood-23.8.1.0/lightwood/data/timeseries_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     if df.shape[0] > 1:
         butlast_row = df.iloc[[-2]]
         delta = (last_row[ob].values - butlast_row[ob].values).flatten()[0]
     else:
         delta = 1
 
     last_row[ob] += delta
-    new_df = df.append(last_row)
+    new_df = pd.concat([df, last_row], ignore_index=True)
     new_df.index = pd.DatetimeIndex(new_index)
     return new_df
 
 
 def _ts_to_obj(df: pd.DataFrame, historical_columns: list) -> pd.DataFrame:
     """
     Casts all historical columns in a dataframe to `object` type.
```

### Comparing `lightwood-23.7.1.0/lightwood/encoder/__init__.py` & `lightwood-23.8.1.0/lightwood/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/array/array.py` & `lightwood-23.8.1.0/lightwood/encoder/array/array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/array/ts_cat_array.py` & `lightwood-23.8.1.0/lightwood/encoder/array/ts_cat_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/array/ts_num_array.py` & `lightwood-23.8.1.0/lightwood/encoder/array/ts_num_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/audio/mfcc.py` & `lightwood-23.8.1.0/lightwood/encoder/audio/mfcc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/base.py` & `lightwood-23.8.1.0/lightwood/encoder/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/categorical/autoencoder.py` & `lightwood-23.8.1.0/lightwood/encoder/categorical/autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/categorical/binary.py` & `lightwood-23.8.1.0/lightwood/encoder/categorical/binary.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/categorical/gym.py` & `lightwood-23.8.1.0/lightwood/encoder/categorical/gym.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/categorical/multihot.py` & `lightwood-23.8.1.0/lightwood/encoder/categorical/multihot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/categorical/onehot.py` & `lightwood-23.8.1.0/lightwood/encoder/categorical/onehot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/categorical/simple_label.py` & `lightwood-23.8.1.0/lightwood/encoder/categorical/simple_label.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/datetime/datetime.py` & `lightwood-23.8.1.0/lightwood/encoder/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/datetime/datetime_sin_normalizer.py` & `lightwood-23.8.1.0/lightwood/encoder/datetime/datetime_sin_normalizer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/helpers.py` & `lightwood-23.8.1.0/lightwood/encoder/helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/identity/identity.py` & `lightwood-23.8.1.0/lightwood/encoder/identity/identity.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/image/helpers/img_to_vec.py` & `lightwood-23.8.1.0/lightwood/encoder/image/helpers/img_to_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/image/img_2_vec.py` & `lightwood-23.8.1.0/lightwood/encoder/image/img_2_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/numeric/numeric.py` & `lightwood-23.8.1.0/lightwood/encoder/numeric/numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/numeric/ts_numeric.py` & `lightwood-23.8.1.0/lightwood/encoder/numeric/ts_numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/text/helpers/pretrained_helpers.py` & `lightwood-23.8.1.0/lightwood/encoder/text/helpers/pretrained_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/text/helpers/rnn_helpers.py` & `lightwood-23.8.1.0/lightwood/encoder/text/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/text/pretrained.py` & `lightwood-23.8.1.0/lightwood/encoder/text/pretrained.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/text/rnn.py` & `lightwood-23.8.1.0/lightwood/encoder/text/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/text/short.py` & `lightwood-23.8.1.0/lightwood/encoder/text/short.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/text/tfidf.py` & `lightwood-23.8.1.0/lightwood/encoder/text/tfidf.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/text/vocab.py` & `lightwood-23.8.1.0/lightwood/encoder/text/vocab.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/common.py` & `lightwood-23.8.1.0/lightwood/encoder/time_series/helpers/common.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/rnn_helpers.py` & `lightwood-23.8.1.0/lightwood/encoder/time_series/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/transformer_helpers.py` & `lightwood-23.8.1.0/lightwood/encoder/time_series/helpers/transformer_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/time_series/rnn.py` & `lightwood-23.8.1.0/lightwood/encoder/time_series/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/encoder/time_series/ts.py` & `lightwood-23.8.1.0/lightwood/encoder/time_series/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/ensemble/__init__.py` & `lightwood-23.8.1.0/lightwood/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/ensemble/base.py` & `lightwood-23.8.1.0/lightwood/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/ensemble/best_of.py` & `lightwood-23.8.1.0/lightwood/ensemble/best_of.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/ensemble/embed.py` & `lightwood-23.8.1.0/lightwood/ensemble/embed.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/ensemble/identity.py` & `lightwood-23.8.1.0/lightwood/ensemble/identity.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/ensemble/mean_ensemble.py` & `lightwood-23.8.1.0/lightwood/ensemble/mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/ensemble/mode_ensemble.py` & `lightwood-23.8.1.0/lightwood/ensemble/mode_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/ensemble/stacked_ensemble.py` & `lightwood-23.8.1.0/lightwood/ensemble/stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/ensemble/ts_stacked_ensemble.py` & `lightwood-23.8.1.0/lightwood/ensemble/ts_stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/ensemble/weighted_mean_ensemble.py` & `lightwood-23.8.1.0/lightwood/ensemble/weighted_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/helpers/__init__.py` & `lightwood-23.8.1.0/lightwood/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/helpers/device.py` & `lightwood-23.8.1.0/lightwood/helpers/device.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/helpers/general.py` & `lightwood-23.8.1.0/lightwood/helpers/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """ # noqa
     # TODO: consider removing this helper entirely, arguably should move into dataprep_ml
 
     # start dispatch with types that are expensive to e.g. cast into strings
     if type(value) in (np.ndarray,) and value.size == 0:
         return True
 
-    if type(value) != str and isinstance(value, Iterable) and value == []:
+    if type(value) != str and isinstance(value, Iterable) and len(value) == 0:
         return True
     elif type(value) != str and isinstance(value, Iterable):
         return False
 
     if value is None:
         return True
```

### Comparing `lightwood-23.7.1.0/lightwood/helpers/io.py` & `lightwood-23.8.1.0/lightwood/helpers/io.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/helpers/log.py` & `lightwood-23.8.1.0/lightwood/helpers/log.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,24 +15,39 @@
     logging.basicConfig(handlers=[handler])
     log = logging.getLogger(f'lightwood-{pid}')
     log_level = os.environ.get('LIGHTWOOD_LOG', 'DEBUG')
     log.setLevel(log_level)
     return log
 
 
-def timed(f):
+def timed_predictor(f):
     """
     Intended to be called from within lightwood predictor methods.
     We use `wraps` to pass metadata into debuggers (as in stackoverflow.com/a/27737385)
     """
     @wraps(f)
     def wrap(predictor, *args, **kw):
         ts = time()
         result = f(predictor, *args, **kw)
         te = time()
         log.debug(f' `{f.__name__}` runtime: {round(te - ts, 2)} seconds')
-        predictor.runtime_log[(f.__name__, datetime.fromtimestamp(ts))] = round(te - ts, 2)
+        if hasattr(predictor, 'runtime_log'):
+            predictor.runtime_log[(f.__name__, datetime.fromtimestamp(ts))] = round(te - ts, 2)
+        return result
+    return wrap
+
+
+def timed(f):
+    """
+    Intended to be called from within any lightwood method to log the runtime.
+    """
+    @wraps(f)
+    def wrap(*args, **kw):
+        ts = time()
+        result = f(*args, **kw)
+        te = time()
+        log.debug(f' `{f.__name__}` runtime: {round(te - ts, 2)} seconds')
         return result
     return wrap
 
 
 log = initialize_log()
```

### Comparing `lightwood-23.7.1.0/lightwood/helpers/parallelism.py` & `lightwood-23.8.1.0/lightwood/helpers/parallelism.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/helpers/templating.py` & `lightwood-23.8.1.0/lightwood/helpers/templating.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/helpers/text.py` & `lightwood-23.8.1.0/lightwood/helpers/text.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/helpers/torch.py` & `lightwood-23.8.1.0/lightwood/helpers/torch.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/helpers/ts.py` & `lightwood-23.8.1.0/lightwood/helpers/ts.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,43 +47,49 @@
 
     return deltas, periods, freqs
 
 
 def get_inferred_timestamps(df: pd.DataFrame, col: str, deltas: dict, tss, stat_analysis,
                             time_format='') -> pd.DataFrame:
     horizon = tss.horizon
-    if tss.group_by:
-        gby = [f'group_{g}' for g in tss.group_by]
 
-    for (idx, row) in df.iterrows():
-        last = [r for r in row[f'order_{col}'] if r == r][-1]  # filter out nans (safeguard; it shouldn't happen anyway)
+    last = np.vstack(df[f'order_{col}'].dropna().values)[:, -1]
 
-        if tss.group_by:
-            try:
-                series_delta = deltas[tuple(row[gby].tolist())]
-            except KeyError:
-                series_delta = deltas['__default']
+    if tss.group_by:
+        gby = [f'group_{g}' for g in tss.group_by]
+        series_delta = df[gby].apply(lambda x: deltas.get(tuple(x.values.tolist()),
+                                                          deltas['__default']), axis=1).values
+        series_delta = series_delta.reshape(-1, 1)
+    else:
+        series_delta = np.full_like(df.values[:, 0:1], deltas['__default'])
+
+    last = np.repeat(np.expand_dims(last, axis=1), horizon, axis=1)
+    lins = np.linspace(0, horizon - 1, num=horizon)
+    series_delta = np.repeat(series_delta, horizon, axis=1)
+    timestamps = last + series_delta * lins
+
+    if time_format:
+        if time_format.lower() == 'infer':
+            tformat = stat_analysis.ts_stats['order_format']
         else:
-            series_delta = deltas['__default']
-        timestamps = [last + t * series_delta for t in range(horizon)]
+            tformat = time_format
+
+        if tformat:
+            def _strfts(elt):
+                return datetime.utcfromtimestamp(elt).strftime(tformat)
+            timestamps = np.vectorize(_strfts)(timestamps)
 
-        if tss.horizon == 1:
-            timestamps = timestamps[0]  # preserves original input format if horizon == 1
+    # truncate to horizon
+    timestamps = timestamps[:, :horizon]
 
-        if time_format:
-            if time_format.lower() == 'infer':
-                tformat = stat_analysis.ts_stats['order_format']
-            else:
-                tformat = time_format
-
-            if tformat:
-                for i, ts in enumerate(timestamps):
-                    timestamps[i] = datetime.utcfromtimestamp(ts).strftime(tformat)
+    # preserves original input format if horizon == 1
+    if tss.horizon == 1:
+        timestamps = timestamps.squeeze()
 
-        df[f'order_{col}'].iloc[idx] = timestamps
+    df[f'order_{col}'] = timestamps.tolist()
     return df[f'order_{col}']
 
 
 def add_tn_num_conf_bounds(data: pd.DataFrame, tss_args):
     """
     Deprecated. Instead we now opt for the much better solution of having scores for each timestep (see all TS classes in analysis/nc)
```

### Comparing `lightwood-23.7.1.0/lightwood/mixer/__init__.py` & `lightwood-23.8.1.0/lightwood/mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/arima.py` & `lightwood-23.8.1.0/lightwood/mixer/arima.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/base.py` & `lightwood-23.8.1.0/lightwood/mixer/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/ets.py` & `lightwood-23.8.1.0/lightwood/mixer/ets.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/gluonts.py` & `lightwood-23.8.1.0/lightwood/mixer/gluonts.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,22 +230,28 @@
             gby = '__default_group'
             df[gby] = '__default_group'
 
         df[oby_col_name] = df.index
         for col in self.static_features_cat:
             df[col] = self.static_features_cat_encoders[col].transform(df[col].values.reshape(-1, 1))
 
+        static_features = []
+        if self.static_features_real:
+            static_features.extend(self.static_features_real)
+        if self.static_features_cat:
+            static_features.extend(self.static_features_cat)
+        static_features_df = df[static_features]
+
         ds = PandasDataset.from_long_dataframe(
             df,
             target=self.target,
-            item_id=gby,
+            item_id=gby[0],
             freq=freq,
             timestamp=oby_col_name,
-            feat_static_real=self.static_features_real if self.static_features_real else [],
-            feat_static_cat=self.static_features_cat if self.static_features_cat else [],
+            static_features=static_features_df
         )
         return ds
 
 
 class EarlyStop(TrainingHistory):
     def __init__(self, patience=3):
         super().__init__()
```

### Comparing `lightwood-23.7.1.0/lightwood/mixer/helpers/ar_net.py` & `lightwood-23.8.1.0/lightwood/mixer/helpers/ar_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/helpers/default_net.py` & `lightwood-23.8.1.0/lightwood/mixer/helpers/default_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/helpers/qclassic_net.py` & `lightwood-23.8.1.0/lightwood/mixer/helpers/qclassic_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/helpers/ranger.py` & `lightwood-23.8.1.0/lightwood/mixer/helpers/ranger.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/helpers/residual_net.py` & `lightwood-23.8.1.0/lightwood/mixer/helpers/residual_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py` & `lightwood-23.8.1.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/helpers/ts.py` & `lightwood-23.8.1.0/lightwood/mixer/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/lightgbm.py` & `lightwood-23.8.1.0/lightwood/mixer/lightgbm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/lightgbm_array.py` & `lightwood-23.8.1.0/lightwood/mixer/lightgbm_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/neural.py` & `lightwood-23.8.1.0/lightwood/mixer/neural.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/neural_ts.py` & `lightwood-23.8.1.0/lightwood/mixer/neural_ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/nhits.py` & `lightwood-23.8.1.0/lightwood/mixer/nhits.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         log.info('Started fitting N-HITS forecasting model')
 
         # prepare data
         cat_ds = ConcatedEncodedDs([train_data, dev_data])
         oby_col = self.ts_analysis["tss"].order_by
         gby = self.ts_analysis["tss"].group_by if self.ts_analysis["tss"].group_by else []
         df = deepcopy(cat_ds.data_frame)
-        Y_df = self._make_initial_df(df, mode='train')
+        Y_df, _ = self._make_initial_df(df, mode='train')
         self.group_boundaries = self._set_boundary(Y_df, gby)
         if gby:
             n_time = df[gby].value_counts().min()
         else:
             n_time = len(df[f'__mdb_original_{oby_col}'].unique())
         n_ts_val = max(int(.1 * n_time), self.horizon)  # at least self.horizon to validate on
 
@@ -129,78 +129,82 @@
             model = NHITS(h=n_time_out, input_size=self.window, **self.train_args, loss=MQLoss(level=self.conf_level))
             self.model = NeuralForecast(models=[model], freq=self.ts_analysis['sample_freqs']['__default'])
             self.model.fit(df=Y_df, val_size=n_ts_val)
             log.info('Successfully trained N-HITS forecasting model.')
 
     def partial_fit(self, train_data: EncodedDs, dev_data: EncodedDs, args: Optional[dict] = None) -> None:
         self.hyperparam_search = False
-        self.fit(train_data, dev_data)  # TODO: add support for passing args (e.g. n_epochs)
+        self.train_args = args.get('trainer_args', {}) if args else {}  # NOTE: this replaces the original config
+        self.fit(train_data, dev_data)
         self.prepared = True
 
     def __call__(self, ds: Union[EncodedDs, ConcatedEncodedDs],
                  args: PredictionArguments = PredictionArguments()) -> pd.DataFrame:
         """
         Calls the mixer to emit forecasts.
         
         NOTE: in the future we may support predicting every single row efficiently. For now, this mixer
         replicates the neuralforecast library behavior and returns a forecast strictly for the next `tss.horizon`
         timesteps after the end of the input dataframe.
         """  # noqa
         if args.predict_proba:
             log.warning('This mixer does not output probability estimates')
 
-        length = sum(ds.encoded_ds_lengths) if isinstance(ds, ConcatedEncodedDs) else len(ds)
-        ydf = pd.DataFrame(0,  # zero-filled
-                           index=np.arange(length),
-                           columns=['prediction', 'lower', 'upper'],
-                           dtype=object)
-
-        input_df = self._make_initial_df(deepcopy(ds.data_frame))
-        ydf['index'] = input_df['index']
-
-        pred_cols = ['NHITS-median']
-
         # provided quantile must match one of the training levels, else we default to the largest one of these
         if args.fixed_confidence is not None and int(args.fixed_confidence * 100) in self.conf_level:
             level = int(args.fixed_confidence * 100)
         else:
             level = max(self.conf_level)
-        pred_cols.extend([f'NHITS-lo-{level}', f'NHITS-hi-{level}'])
 
         target_cols = ['prediction', 'lower', 'upper']
+        pred_cols = ['NHITS-median', f'NHITS-lo-{level}', f'NHITS-hi-{level}']
+
+        input_df, idxs = self._make_initial_df(deepcopy(ds.data_frame))
+        length = sum(ds.encoded_ds_lengths) if isinstance(ds, ConcatedEncodedDs) else len(ds)
+        ydf = pd.DataFrame(0, index=range(length), columns=target_cols, dtype=object)
+
+        # fill with zeroed arrays
+        zero_array = [0 for _ in range(self.horizon)]
         for target_col in target_cols:
-            ydf[target_col] = [[0 for _ in range(self.horizon)] for _ in range(len(ydf))]  # zero-filled arrays
+            ydf[target_col] = [zero_array] * len(ydf)
 
-        group_ends = []
-        for group in input_df['unique_id'].unique():
-            group_ends.append(input_df[input_df['unique_id'] == group]['index'].iloc[-1])
+        grouper = input_df.groupby('unique_id')
+        group_ends = grouper.last()['index'].values
         fcst = self.model.predict(input_df).reset_index()
+        fcst['ds'] = fcst.groupby('unique_id').cumcount()
+        horizons = pd.pivot_table(fcst, values=pred_cols, index='unique_id', columns='ds')
+
+        temp_df = pd.DataFrame(0,  # zero-filled
+                               index=range(len(horizons)),
+                               columns=target_cols,
+                               dtype=object)
+
+        for pcol, tcol in zip(pred_cols, target_cols):
+            temp_df[tcol] = horizons[pcol].values.tolist()
 
-        for gidx, group in zip(group_ends, input_df['unique_id'].unique()):
-            for pred_col, target_col in zip(pred_cols, target_cols):
-                group_preds = fcst[fcst['unique_id'] == group][pred_col].tolist()[:self.horizon]
-                idx = ydf[ydf['index'] == gidx].index[0]
-                ydf.at[idx, target_col] = group_preds
+        for tcol in target_cols:
+            ydf[tcol].iloc[group_ends] = temp_df[tcol]
 
         ydf['confidence'] = level / 100
         return ydf
 
     def _make_initial_df(self, df, mode='inference'):
         """
         Prepares a dataframe for the NHITS model according to what neuralforecast expects.
 
         If a per-group boundary exists, this method additionally drops out all observations prior to the cutoff.
         """  # noqa
 
         oby_col = self.ts_analysis["tss"].order_by
-        df = df.sort_values(by=f'__mdb_original_{oby_col}')
+        # df = df.sort_values(by=f'__mdb_original_{oby_col}')  # TODO rm
         df[f'__mdb_parsed_{oby_col}'] = df.index
         df = df.reset_index(drop=True)
 
         Y_df = pd.DataFrame()
+        Y_df['_index'] = np.arange(len(df))
         Y_df['y'] = df[self.target]
         Y_df['ds'] = df[f'__mdb_parsed_{oby_col}']
 
         if self.grouped_by != ['__default']:
             Y_df['unique_id'] = df[self.grouped_by].apply(lambda x: ','.join([elt for elt in x]), axis=1)
         else:
             Y_df['unique_id'] = '__default'
@@ -215,15 +219,16 @@
                 if group in self.group_boundaries:
                     sdf = sdf[sdf['ds'].gt(self.group_boundaries[group])]
                     if sdf.shape[0] > 0:
                         filtered.append(sdf)
             if filtered:
                 Y_df = pd.concat(filtered)
 
-        return Y_df
+        filtered_idxs = Y_df.pop('_index').values
+        return Y_df, filtered_idxs
 
     @staticmethod
     def _set_boundary(df: pd.DataFrame, gby: list) -> Dict[str, object]:
         """
         Finds last observation for every series in a pre-sorted `df` given a `gby` list of columns to group by.
         """
         if not gby:
```

### Comparing `lightwood-23.7.1.0/lightwood/mixer/prophet.py` & `lightwood-23.8.1.0/lightwood/mixer/prophet.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/qclassic.py` & `lightwood-23.8.1.0/lightwood/mixer/qclassic.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/random_forest.py` & `lightwood-23.8.1.0/lightwood/mixer/random_forest.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/regression.py` & `lightwood-23.8.1.0/lightwood/mixer/regression.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/sktime.py` & `lightwood-23.8.1.0/lightwood/mixer/sktime.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/tabtransformer.py` & `lightwood-23.8.1.0/lightwood/mixer/tabtransformer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/unit.py` & `lightwood-23.8.1.0/lightwood/mixer/unit.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood/mixer/xgboost.py` & `lightwood-23.8.1.0/lightwood/mixer/xgboost.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.7.1.0/lightwood.egg-info/PKG-INFO` & `lightwood-23.8.1.0/lightwood.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.7.1.0
+Version: 23.8.1.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -214,17 +214,17 @@
         * [Lightwood License](https://github.com/mindsdb/lightwood/blob/master/LICENSE)
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: image
 Provides-Extra: extra
-Provides-Extra: dev
-Provides-Extra: extra_ts
 Provides-Extra: xai
-Provides-Extra: audio
 Provides-Extra: quantum
+Provides-Extra: extra_ts
+Provides-Extra: dev
+Provides-Extra: audio
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.7.1.0/lightwood.egg-info/SOURCES.txt` & `lightwood-23.8.1.0/lightwood.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 lightwood/ensemble/identity.py
 lightwood/ensemble/mean_ensemble.py
 lightwood/ensemble/mode_ensemble.py
 lightwood/ensemble/stacked_ensemble.py
 lightwood/ensemble/ts_stacked_ensemble.py
 lightwood/ensemble/weighted_mean_ensemble.py
 lightwood/helpers/__init__.py
+lightwood/helpers/codegen.py
 lightwood/helpers/constants.py
 lightwood/helpers/device.py
 lightwood/helpers/general.py
 lightwood/helpers/io.py
 lightwood/helpers/log.py
 lightwood/helpers/numeric.py
 lightwood/helpers/parallelism.py
```

### Comparing `lightwood-23.7.1.0/lightwood.egg-info/requires.txt` & `lightwood-23.8.1.0/lightwood.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-type_infer>=0.0.13
-dataprep_ml>=0.0.13
-mindsdb-evaluator>=0.0.9
+type_infer>=0.0.15
+dataprep_ml>=0.0.18
+mindsdb-evaluator>=0.0.11
 numpy
-nltk<3.6,>=3
-python-dateutil>=2.8.1
-pandas<1.5.0,>=1.1.5
+nltk<3.9,>=3.8
+python-dateutil>=2.8.2
+pandas<2.1.0,>=2.0.0
 schema>=0.6.8
 torch<2.1,>=2.0.0
 requests>=2.0.0
 transformers
-optuna<2.10.0,>=2.8.0
+optuna<4.0.0,>=3.1.0
 scipy>=1.5.4
 psutil>=5.7.0
 setuptools>=21.2.1
 wheel>=0.32.2
-scikit-learn<=1.0.2,>=1.0.0
+scikit-learn>=1.0.0
 dataclasses_json>=0.5.4
 dill==0.3.6
-sktime<0.15.0,>=0.14.0
+sktime<0.22.0,>=0.21.0
 statsforecast==1.4.0
 torch_optimizer==0.1.0
 black==23.3.0
 typing_extensions
 colorlog==6.5.0
 statsmodels>=0.12.0
 langid==1.1.6
@@ -30,28 +30,28 @@
 xgboost<=1.8.0,>=1.6.0
 tab-transformer-pytorch>=0.2.1
 typing-inspect
 six
 regex
 
 [all_extras]
-torchvision
-prophet==1.1
-pystan==2.19.1.1
+neuralforecast==1.5.0
+lightgbm<=3.3.3,>=3.3.0
+shap>=0.40.0
+pyod==1.0.4
 autopep8>=1.5.7
-pillow>8.3.1
 suod
-lightgbm<=3.3.3,>=3.3.0
+librosa==0.8.1
 mxnet<2.0.0,>=1.6.0
-pyod==1.0.4
+pystan==2.19.1.1
 qiskit==0.31.0
-gluonts<0.12.0,>=0.11.0
-neuralforecast==1.5.0
-librosa==0.8.1
-shap>=0.40.0
+pillow>8.3.1
+torchvision
+prophet==1.1
+gluonts<0.14.0,>=0.13.2
 
 [audio]
 librosa==0.8.1
 
 [dev]
 autopep8>=1.5.7
 
@@ -59,15 +59,15 @@
 lightgbm<=3.3.3,>=3.3.0
 
 [extra_ts]
 pystan==2.19.1.1
 prophet==1.1
 neuralforecast==1.5.0
 mxnet<2.0.0,>=1.6.0
-gluonts<0.12.0,>=0.11.0
+gluonts<0.14.0,>=0.13.2
 
 [image]
 torchvision
 pillow>8.3.1
 
 [quantum]
 qiskit==0.31.0
```

### Comparing `lightwood-23.7.1.0/requirements.txt` & `lightwood-23.8.1.0/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-type_infer >=0.0.13
-dataprep_ml >=0.0.13
-mindsdb-evaluator >=0.0.9
+type_infer >=0.0.15
+dataprep_ml >=0.0.18
+mindsdb-evaluator >=0.0.11
 numpy
-nltk >=3,<3.6
-python-dateutil >=2.8.1
-pandas >=1.1.5, <1.5.0
+nltk >=3.8, <3.9
+python-dateutil >=2.8.2
+pandas >=2.0.0, <2.1.0
 schema >=0.6.8
 torch >=2.0.0, <2.1
 requests >=2.0.0
 transformers
-optuna >=2.8.0,<2.10.0
+optuna >=3.1.0,<4.0.0
 scipy >=1.5.4
 psutil >=5.7.0
 setuptools >=21.2.1
 wheel >=0.32.2
-scikit-learn >=1.0.0, <=1.0.2
+scikit-learn >=1.0.0
 dataclasses_json >=0.5.4
 dill ==0.3.6
-sktime >=0.14.0,<0.15.0
+sktime >=0.21.0,<0.22.0
 statsforecast ==1.4.0
 torch_optimizer ==0.1.0
 black ==23.3.0
 typing_extensions
 colorlog ==6.5.0
 statsmodels >=0.12.0
 langid==1.1.6
```

### Comparing `lightwood-23.7.1.0/setup.py` & `lightwood-23.8.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,9 +58,9 @@
     install_requires=requirements,
     extras_require=extra_requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.8"
+    python_requires=">=3.8,<3.12"
 )
```

