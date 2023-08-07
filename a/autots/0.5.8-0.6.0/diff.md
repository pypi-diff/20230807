# Comparing `tmp/autots-0.5.8.tar.gz` & `tmp/autots-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autots-0.5.8.tar", last modified: Thu Jul  6 20:15:28 2023, max compression
+gzip compressed data, was "autots-0.6.0.tar", last modified: Mon Aug  7 21:05:51 2023, max compression
```

## Comparing `autots-0.5.8.tar` & `autots-0.6.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 20:15:28.503508 autots-0.5.8/
-drwxrwxrwx   0        0        0        0 2023-07-06 20:15:28.075806 autots-0.5.8/AutoTS.egg-info/
--rw-rw-rw-   0        0        0     8896 2023-07-06 20:15:28.000000 autots-0.5.8/AutoTS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2148 2023-07-06 20:15:28.000000 autots-0.5.8/AutoTS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 20:15:28.000000 autots-0.5.8/AutoTS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-07-06 20:15:28.000000 autots-0.5.8/AutoTS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-07-06 20:15:28.000000 autots-0.5.8/AutoTS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2022-11-23 22:39:41.000000 autots-0.5.8/LICENSE
--rw-rw-rw-   0        0        0       61 2023-04-03 03:08:26.000000 autots-0.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0     8896 2023-07-06 20:15:28.503508 autots-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     8251 2023-04-10 03:35:49.000000 autots-0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 20:15:28.086353 autots-0.5.8/autots/
--rw-rw-rw-   0        0        0     1384 2023-05-25 15:11:24.000000 autots-0.5.8/autots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:15:28.106112 autots-0.5.8/autots/datasets/
--rw-rw-rw-   0        0        0      535 2022-11-23 22:39:41.000000 autots-0.5.8/autots/datasets/__init__.py
--rw-rw-rw-   0        0        0    32463 2023-04-08 14:56:53.000000 autots-0.5.8/autots/datasets/_base.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:15:28.122224 autots-0.5.8/autots/datasets/data/
--rw-rw-rw-   0        0        0     4527 2022-11-23 22:39:41.000000 autots-0.5.8/autots/datasets/data/covid_daily.zip
--rw-rw-rw-   0        0        0    81380 2022-11-23 22:39:41.000000 autots-0.5.8/autots/datasets/data/eia_weekly.zip
--rw-rw-rw-   0        0        0    27440 2022-11-23 22:39:41.000000 autots-0.5.8/autots/datasets/data/fred_monthly.zip
--rw-rw-rw-   0        0        0     5553 2022-11-23 22:39:41.000000 autots-0.5.8/autots/datasets/data/fred_yearly.zip
--rw-rw-rw-   0        0        0   107751 2022-11-23 22:39:41.000000 autots-0.5.8/autots/datasets/data/holidays.zip
--rw-rw-rw-   0        0        0   158529 2022-11-23 22:39:41.000000 autots-0.5.8/autots/datasets/data/traffic_hourly.zip
--rw-rw-rw-   0        0        0     3377 2023-04-10 03:29:38.000000 autots-0.5.8/autots/datasets/fred.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:15:28.170556 autots-0.5.8/autots/evaluator/
--rw-rw-rw-   0        0        0       28 2022-11-23 22:39:41.000000 autots-0.5.8/autots/evaluator/__init__.py
--rw-rw-rw-   0        0        0    16533 2023-04-10 03:29:38.000000 autots-0.5.8/autots/evaluator/anomaly_detector.py
--rw-rw-rw-   0        0        0   109554 2023-07-06 14:38:15.000000 autots-0.5.8/autots/evaluator/auto_model.py
--rw-rw-rw-   0        0        0   148602 2023-07-06 14:38:15.000000 autots-0.5.8/autots/evaluator/auto_ts.py
--rw-rw-rw-   0        0        0    24446 2022-11-23 22:39:41.000000 autots-0.5.8/autots/evaluator/benchmark.py
--rw-rw-rw-   0        0        0    32646 2023-02-01 17:49:09.000000 autots-0.5.8/autots/evaluator/event_forecasting.py
--rw-rw-rw-   0        0        0    21871 2023-05-13 12:57:26.000000 autots-0.5.8/autots/evaluator/metrics.py
--rw-rw-rw-   0        0        0     6490 2023-02-01 17:49:09.000000 autots-0.5.8/autots/evaluator/validation.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:15:28.273507 autots-0.5.8/autots/models/
--rw-rw-rw-   0        0        0       24 2022-11-23 22:39:41.000000 autots-0.5.8/autots/models/__init__.py
--rw-rw-rw-   0        0        0    14112 2023-01-16 02:41:20.000000 autots-0.5.8/autots/models/arch.py
--rw-rw-rw-   0        0        0    26079 2023-07-06 14:38:14.000000 autots-0.5.8/autots/models/base.py
--rw-rw-rw-   0        0        0   113966 2023-07-06 14:38:15.000000 autots-0.5.8/autots/models/basics.py
--rw-rw-rw-   0        0        0   116382 2023-07-06 14:38:15.000000 autots-0.5.8/autots/models/cassandra.py
--rw-rw-rw-   0        0        0    16461 2022-11-23 22:39:41.000000 autots-0.5.8/autots/models/dnn.py
--rw-rw-rw-   0        0        0    63476 2023-05-23 03:16:40.000000 autots-0.5.8/autots/models/ensemble.py
--rw-rw-rw-   0        0        0    28473 2023-06-30 22:19:55.000000 autots-0.5.8/autots/models/gluonts.py
--rw-rw-rw-   0        0        0    10745 2023-04-10 03:29:38.000000 autots-0.5.8/autots/models/greykite.py
--rw-rw-rw-   0        0        0    33909 2022-11-23 22:39:41.000000 autots-0.5.8/autots/models/matrix_var.py
--rw-rw-rw-   0        0        0    19900 2023-04-10 03:29:38.000000 autots-0.5.8/autots/models/mlensemble.py
--rw-rw-rw-   0        0        0     8627 2023-07-06 14:38:14.000000 autots-0.5.8/autots/models/model_list.py
--rw-rw-rw-   0        0        0    33743 2022-11-23 22:39:41.000000 autots-0.5.8/autots/models/prophet.py
--rw-rw-rw-   0        0        0    21856 2023-07-06 14:38:14.000000 autots-0.5.8/autots/models/pytorch.py
--rw-rw-rw-   0        0        0   119772 2023-07-06 14:38:15.000000 autots-0.5.8/autots/models/sklearn.py
--rw-rw-rw-   0        0        0    93302 2023-02-01 17:49:10.000000 autots-0.5.8/autots/models/statsmodels.py
--rw-rw-rw-   0        0        0    21794 2022-11-23 22:39:41.000000 autots-0.5.8/autots/models/tfp.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:15:28.296902 autots-0.5.8/autots/templates/
--rw-rw-rw-   0        0        0       27 2022-11-23 22:39:41.000000 autots-0.5.8/autots/templates/__init__.py
--rw-rw-rw-   0        0        0    42365 2023-01-21 02:30:16.000000 autots-0.5.8/autots/templates/general.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:15:28.431448 autots-0.5.8/autots/tools/
--rw-rw-rw-   0        0        0       96 2022-11-23 22:39:41.000000 autots-0.5.8/autots/tools/__init__.py
--rw-rw-rw-   0        0        0    42765 2023-04-10 03:29:39.000000 autots-0.5.8/autots/tools/anomaly_utils.py
--rw-rw-rw-   0        0        0     9168 2023-04-08 14:59:14.000000 autots-0.5.8/autots/tools/calendar.py
--rw-rw-rw-   0        0        0     7163 2022-11-23 22:39:41.000000 autots-0.5.8/autots/tools/cointegration.py
--rw-rw-rw-   0        0        0     1709 2022-11-23 22:39:41.000000 autots-0.5.8/autots/tools/cpu_count.py
--rw-rw-rw-   0        0        0    40565 2023-07-06 14:38:14.000000 autots-0.5.8/autots/tools/fast_kalman.py
--rw-rw-rw-   0        0        0     5872 2022-11-23 22:39:41.000000 autots-0.5.8/autots/tools/hierarchial.py
--rw-rw-rw-   0        0        0     5983 2023-05-23 03:16:38.000000 autots-0.5.8/autots/tools/holiday.py
--rw-rw-rw-   0        0        0     9153 2022-11-23 22:39:41.000000 autots-0.5.8/autots/tools/impute.py
--rw-rw-rw-   0        0        0     5188 2022-11-23 22:39:41.000000 autots-0.5.8/autots/tools/lunar.py
--rw-rw-rw-   0        0        0     4362 2022-11-23 22:39:41.000000 autots-0.5.8/autots/tools/percentile.py
--rw-rw-rw-   0        0        0     7786 2022-11-23 22:39:41.000000 autots-0.5.8/autots/tools/probabilistic.py
--rw-rw-rw-   0        0        0     1001 2022-11-23 22:39:41.000000 autots-0.5.8/autots/tools/profile.py
--rw-rw-rw-   0        0        0    15361 2023-04-09 14:46:49.000000 autots-0.5.8/autots/tools/regressor.py
--rw-rw-rw-   0        0        0    20206 2023-05-23 03:16:39.000000 autots-0.5.8/autots/tools/seasonal.py
--rw-rw-rw-   0        0        0    18159 2023-06-08 16:48:13.000000 autots-0.5.8/autots/tools/shaping.py
--rw-rw-rw-   0        0        0    19147 2023-04-08 14:59:28.000000 autots-0.5.8/autots/tools/thresholding.py
--rw-rw-rw-   0        0        0   160900 2023-07-06 14:38:15.000000 autots-0.5.8/autots/tools/transform.py
--rw-rw-rw-   0        0        0    18154 2023-04-10 03:29:39.000000 autots-0.5.8/autots/tools/window_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:15:28.441067 autots-0.5.8/docs/
--rw-rw-rw-   0        0        0     2748 2023-05-25 15:11:28.000000 autots-0.5.8/docs/conf.py
--rw-rw-rw-   0        0        0     1176 2023-05-25 15:11:36.000000 autots-0.5.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 20:15:28.503508 autots-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1273 2023-05-25 15:11:31.000000 autots-0.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:15:28.503508 autots-0.5.8/tests/
--rw-rw-rw-   0        0        0     4677 2022-11-23 22:39:41.000000 autots-0.5.8/tests/test_anomalies.py
--rw-rw-rw-   0        0        0    29648 2023-07-06 18:15:46.000000 autots-0.5.8/tests/test_autots.py
--rw-rw-rw-   0        0        0     6882 2023-05-17 21:08:23.000000 autots-0.5.8/tests/test_calendar_holiday.py
--rw-rw-rw-   0        0        0    10554 2023-04-02 03:12:25.000000 autots-0.5.8/tests/test_cassandra.py
--rw-rw-rw-   0        0        0     3654 2022-11-23 22:39:41.000000 autots-0.5.8/tests/test_event_forecasting.py
--rw-rw-rw-   0        0        0     1512 2022-11-23 22:39:41.000000 autots-0.5.8/tests/test_impute.py
--rw-rw-rw-   0        0        0     5118 2023-05-17 20:57:36.000000 autots-0.5.8/tests/test_metrics.py
--rw-rw-rw-   0        0        0     1514 2022-11-23 22:39:41.000000 autots-0.5.8/tests/test_percentile.py
--rw-rw-rw-   0        0        0     1836 2022-11-23 22:39:41.000000 autots-0.5.8/tests/test_regressor.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:05:51.749713 autots-0.6.0/
+drwxrwxrwx   0        0        0        0 2023-08-07 21:05:51.637289 autots-0.6.0/AutoTS.egg-info/
+-rw-rw-rw-   0        0        0     8898 2023-08-07 21:05:51.000000 autots-0.6.0/AutoTS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2148 2023-08-07 21:05:51.000000 autots-0.6.0/AutoTS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 21:05:51.000000 autots-0.6.0/AutoTS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      224 2023-08-07 21:05:51.000000 autots-0.6.0/AutoTS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       62 2023-08-07 21:05:51.000000 autots-0.6.0/AutoTS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2022-11-23 22:39:41.000000 autots-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0       61 2023-04-03 03:08:26.000000 autots-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8898 2023-08-07 21:05:51.748208 autots-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8253 2023-07-27 12:33:08.000000 autots-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 21:05:51.638289 autots-0.6.0/autots/
+-rw-rw-rw-   0        0        0     1384 2023-08-07 20:59:28.000000 autots-0.6.0/autots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:05:51.640293 autots-0.6.0/autots/datasets/
+-rw-rw-rw-   0        0        0      535 2022-11-23 22:39:41.000000 autots-0.6.0/autots/datasets/__init__.py
+-rw-rw-rw-   0        0        0    32463 2023-04-08 14:56:53.000000 autots-0.6.0/autots/datasets/_base.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:05:51.663121 autots-0.6.0/autots/datasets/data/
+-rw-rw-rw-   0        0        0     4527 2022-11-23 22:39:41.000000 autots-0.6.0/autots/datasets/data/covid_daily.zip
+-rw-rw-rw-   0        0        0    81380 2022-11-23 22:39:41.000000 autots-0.6.0/autots/datasets/data/eia_weekly.zip
+-rw-rw-rw-   0        0        0    27440 2022-11-23 22:39:41.000000 autots-0.6.0/autots/datasets/data/fred_monthly.zip
+-rw-rw-rw-   0        0        0     5553 2022-11-23 22:39:41.000000 autots-0.6.0/autots/datasets/data/fred_yearly.zip
+-rw-rw-rw-   0        0        0   149549 2023-07-19 04:50:46.000000 autots-0.6.0/autots/datasets/data/holidays.zip
+-rw-rw-rw-   0        0        0   158529 2022-11-23 22:39:41.000000 autots-0.6.0/autots/datasets/data/traffic_hourly.zip
+-rw-rw-rw-   0        0        0     3377 2023-04-10 03:29:38.000000 autots-0.6.0/autots/datasets/fred.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:05:51.668934 autots-0.6.0/autots/evaluator/
+-rw-rw-rw-   0        0        0       28 2022-11-23 22:39:41.000000 autots-0.6.0/autots/evaluator/__init__.py
+-rw-rw-rw-   0        0        0    16689 2023-08-07 21:01:09.000000 autots-0.6.0/autots/evaluator/anomaly_detector.py
+-rw-rw-rw-   0        0        0   111778 2023-08-07 21:01:10.000000 autots-0.6.0/autots/evaluator/auto_model.py
+-rw-rw-rw-   0        0        0   161601 2023-08-07 21:01:11.000000 autots-0.6.0/autots/evaluator/auto_ts.py
+-rw-rw-rw-   0        0        0    24446 2022-11-23 22:39:41.000000 autots-0.6.0/autots/evaluator/benchmark.py
+-rw-rw-rw-   0        0        0    32646 2023-02-01 17:49:09.000000 autots-0.6.0/autots/evaluator/event_forecasting.py
+-rw-rw-rw-   0        0        0    21871 2023-05-13 12:57:26.000000 autots-0.6.0/autots/evaluator/metrics.py
+-rw-rw-rw-   0        0        0     6490 2023-02-01 17:49:09.000000 autots-0.6.0/autots/evaluator/validation.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:05:51.681268 autots-0.6.0/autots/models/
+-rw-rw-rw-   0        0        0       24 2022-11-23 22:39:41.000000 autots-0.6.0/autots/models/__init__.py
+-rw-rw-rw-   0        0        0    14112 2023-01-16 02:41:20.000000 autots-0.6.0/autots/models/arch.py
+-rw-rw-rw-   0        0        0    26298 2023-08-04 07:38:08.000000 autots-0.6.0/autots/models/base.py
+-rw-rw-rw-   0        0        0   115035 2023-08-07 21:01:11.000000 autots-0.6.0/autots/models/basics.py
+-rw-rw-rw-   0        0        0   121618 2023-08-07 21:01:11.000000 autots-0.6.0/autots/models/cassandra.py
+-rw-rw-rw-   0        0        0    16461 2022-11-23 22:39:41.000000 autots-0.6.0/autots/models/dnn.py
+-rw-rw-rw-   0        0        0    63476 2023-05-23 03:16:40.000000 autots-0.6.0/autots/models/ensemble.py
+-rw-rw-rw-   0        0        0    28803 2023-08-07 21:01:09.000000 autots-0.6.0/autots/models/gluonts.py
+-rw-rw-rw-   0        0        0    10745 2023-04-10 03:29:38.000000 autots-0.6.0/autots/models/greykite.py
+-rw-rw-rw-   0        0        0    33909 2022-11-23 22:39:41.000000 autots-0.6.0/autots/models/matrix_var.py
+-rw-rw-rw-   0        0        0    19900 2023-04-10 03:29:38.000000 autots-0.6.0/autots/models/mlensemble.py
+-rw-rw-rw-   0        0        0     8914 2023-08-07 21:01:09.000000 autots-0.6.0/autots/models/model_list.py
+-rw-rw-rw-   0        0        0    33743 2022-11-23 22:39:41.000000 autots-0.6.0/autots/models/prophet.py
+-rw-rw-rw-   0        0        0    21856 2023-07-06 14:38:14.000000 autots-0.6.0/autots/models/pytorch.py
+-rw-rw-rw-   0        0        0   121008 2023-08-07 21:01:11.000000 autots-0.6.0/autots/models/sklearn.py
+-rw-rw-rw-   0        0        0    93357 2023-07-28 19:22:54.000000 autots-0.6.0/autots/models/statsmodels.py
+-rw-rw-rw-   0        0        0    21794 2022-11-23 22:39:41.000000 autots-0.6.0/autots/models/tfp.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:05:51.682744 autots-0.6.0/autots/templates/
+-rw-rw-rw-   0        0        0       27 2022-11-23 22:39:41.000000 autots-0.6.0/autots/templates/__init__.py
+-rw-rw-rw-   0        0        0    41978 2023-07-10 20:20:24.000000 autots-0.6.0/autots/templates/general.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:05:51.698216 autots-0.6.0/autots/tools/
+-rw-rw-rw-   0        0        0       96 2022-11-23 22:39:41.000000 autots-0.6.0/autots/tools/__init__.py
+-rw-rw-rw-   0        0        0    42765 2023-04-10 03:29:39.000000 autots-0.6.0/autots/tools/anomaly_utils.py
+-rw-rw-rw-   0        0        0     9168 2023-04-08 14:59:14.000000 autots-0.6.0/autots/tools/calendar.py
+-rw-rw-rw-   0        0        0     7163 2022-11-23 22:39:41.000000 autots-0.6.0/autots/tools/cointegration.py
+-rw-rw-rw-   0        0        0     1709 2022-11-23 22:39:41.000000 autots-0.6.0/autots/tools/cpu_count.py
+-rw-rw-rw-   0        0        0    40565 2023-07-06 14:38:14.000000 autots-0.6.0/autots/tools/fast_kalman.py
+-rw-rw-rw-   0        0        0     5872 2022-11-23 22:39:41.000000 autots-0.6.0/autots/tools/hierarchial.py
+-rw-rw-rw-   0        0        0     5983 2023-05-23 03:16:38.000000 autots-0.6.0/autots/tools/holiday.py
+-rw-rw-rw-   0        0        0    14617 2023-08-07 21:01:09.000000 autots-0.6.0/autots/tools/impute.py
+-rw-rw-rw-   0        0        0     5188 2022-11-23 22:39:41.000000 autots-0.6.0/autots/tools/lunar.py
+-rw-rw-rw-   0        0        0     4362 2022-11-23 22:39:41.000000 autots-0.6.0/autots/tools/percentile.py
+-rw-rw-rw-   0        0        0     7786 2022-11-23 22:39:41.000000 autots-0.6.0/autots/tools/probabilistic.py
+-rw-rw-rw-   0        0        0     1001 2022-11-23 22:39:41.000000 autots-0.6.0/autots/tools/profile.py
+-rw-rw-rw-   0        0        0    15728 2023-07-25 03:36:28.000000 autots-0.6.0/autots/tools/regressor.py
+-rw-rw-rw-   0        0        0    21928 2023-08-07 21:01:09.000000 autots-0.6.0/autots/tools/seasonal.py
+-rw-rw-rw-   0        0        0    18578 2023-08-04 07:41:54.000000 autots-0.6.0/autots/tools/shaping.py
+-rw-rw-rw-   0        0        0    19147 2023-04-08 14:59:28.000000 autots-0.6.0/autots/tools/thresholding.py
+-rw-rw-rw-   0        0        0   172544 2023-08-07 21:01:12.000000 autots-0.6.0/autots/tools/transform.py
+-rw-rw-rw-   0        0        0    18154 2023-04-10 03:29:39.000000 autots-0.6.0/autots/tools/window_functions.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:05:51.698216 autots-0.6.0/docs/
+-rw-rw-rw-   0        0        0     2748 2023-08-07 20:59:33.000000 autots-0.6.0/docs/conf.py
+-rw-rw-rw-   0        0        0     1176 2023-08-07 20:59:42.000000 autots-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 21:05:51.749713 autots-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1273 2023-08-07 20:59:37.000000 autots-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:05:51.748208 autots-0.6.0/tests/
+-rw-rw-rw-   0        0        0     4677 2022-11-23 22:39:41.000000 autots-0.6.0/tests/test_anomalies.py
+-rw-rw-rw-   0        0        0    38336 2023-08-07 20:02:42.000000 autots-0.6.0/tests/test_autots.py
+-rw-rw-rw-   0        0        0     6882 2023-05-17 21:08:23.000000 autots-0.6.0/tests/test_calendar_holiday.py
+-rw-rw-rw-   0        0        0    10600 2023-08-05 21:46:08.000000 autots-0.6.0/tests/test_cassandra.py
+-rw-rw-rw-   0        0        0     3654 2022-11-23 22:39:41.000000 autots-0.6.0/tests/test_event_forecasting.py
+-rw-rw-rw-   0        0        0     1512 2022-11-23 22:39:41.000000 autots-0.6.0/tests/test_impute.py
+-rw-rw-rw-   0        0        0     5118 2023-05-17 20:57:36.000000 autots-0.6.0/tests/test_metrics.py
+-rw-rw-rw-   0        0        0     1514 2022-11-23 22:39:41.000000 autots-0.6.0/tests/test_percentile.py
+-rw-rw-rw-   0        0        0     1836 2022-11-23 22:39:41.000000 autots-0.6.0/tests/test_regressor.py
```

### Comparing `autots-0.5.8/AutoTS.egg-info/PKG-INFO` & `autots-0.6.0/AutoTS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autots
-Version: 0.5.8
+Version: 0.6.0
 Summary: Automated Time Series Forecasting
 Home-page: https://github.com/winedarksea/AutoTS
 Author: Colin Catlin
 Author-email: Colin Catlin <colin.catlin@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/winedarksea/AutoTS
 Project-URL: Bug Tracker, https://github.com/winedarksea/AutoTS/issues
@@ -73,15 +73,15 @@
 long = False
 df = load_daily(long=long)
 
 model = AutoTS(
     forecast_length=21,
     frequency='infer',
     prediction_interval=0.9,
-    ensemble=None,
+    ensemble='auto',
     model_list="fast",  # "superfast", "default", "fast_parallel"
     transformer_list="fast",  # "superfast",
     drop_most_recent=1,
     max_generations=4,
     num_validations=2,
     validation_method="backwards"
 )
```

### Comparing `autots-0.5.8/AutoTS.egg-info/SOURCES.txt` & `autots-0.6.0/AutoTS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/LICENSE` & `autots-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/PKG-INFO` & `autots-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autots
-Version: 0.5.8
+Version: 0.6.0
 Summary: Automated Time Series Forecasting
 Home-page: https://github.com/winedarksea/AutoTS
 Author: Colin Catlin
 Author-email: Colin Catlin <colin.catlin@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/winedarksea/AutoTS
 Project-URL: Bug Tracker, https://github.com/winedarksea/AutoTS/issues
@@ -73,15 +73,15 @@
 long = False
 df = load_daily(long=long)
 
 model = AutoTS(
     forecast_length=21,
     frequency='infer',
     prediction_interval=0.9,
-    ensemble=None,
+    ensemble='auto',
     model_list="fast",  # "superfast", "default", "fast_parallel"
     transformer_list="fast",  # "superfast",
     drop_most_recent=1,
     max_generations=4,
     num_validations=2,
     validation_method="backwards"
 )
```

### Comparing `autots-0.5.8/README.md` & `autots-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 long = False
 df = load_daily(long=long)
 
 model = AutoTS(
     forecast_length=21,
     frequency='infer',
     prediction_interval=0.9,
-    ensemble=None,
+    ensemble='auto',
     model_list="fast",  # "superfast", "default", "fast_parallel"
     transformer_list="fast",  # "superfast",
     drop_most_recent=1,
     max_generations=4,
     num_validations=2,
     validation_method="backwards"
 )
```

### Comparing `autots-0.5.8/autots/__init__.py` & `autots-0.6.0/autots/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from autots.tools.shaping import long_to_wide
 from autots.tools.regressor import create_lagged_regressor, create_regressor
 from autots.evaluator.auto_model import model_forecast
 from autots.evaluator.anomaly_detector import AnomalyDetector, HolidayDetector
 from autots.models.cassandra import Cassandra
 
 
-__version__ = '0.5.8'
+__version__ = '0.6.0'
 
 TransformTS = GeneralTransformer
 
 __all__ = [
     'load_daily',
     'load_monthly',
     'load_yearly',
```

### Comparing `autots-0.5.8/autots/datasets/__init__.py` & `autots-0.6.0/autots/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/datasets/_base.py` & `autots-0.6.0/autots/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/datasets/data/covid_daily.zip` & `autots-0.6.0/autots/datasets/data/covid_daily.zip`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/datasets/data/eia_weekly.zip` & `autots-0.6.0/autots/datasets/data/eia_weekly.zip`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/datasets/data/fred_monthly.zip` & `autots-0.6.0/autots/datasets/data/fred_monthly.zip`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/datasets/data/fred_yearly.zip` & `autots-0.6.0/autots/datasets/data/fred_yearly.zip`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/datasets/data/traffic_hourly.zip` & `autots-0.6.0/autots/datasets/data/traffic_hourly.zip`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/datasets/fred.py` & `autots-0.6.0/autots/datasets/fred.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/evaluator/anomaly_detector.py` & `autots-0.6.0/autots/evaluator/anomaly_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,20 +315,28 @@
         self.df = df
         self.df_cols = df.columns
 
     def plot_anomaly(self, kwargs={}):
         self.anomaly_model.plot(**kwargs)
 
     def plot(
-        self, series_name=None, include_anomalies=True, title=None, plot_kwargs={}
+        self,
+        series_name=None,
+        include_anomalies=True,
+        title=None,
+        plot_kwargs={},
+        series=None,
     ):
         import matplotlib.pyplot as plt
 
         if series_name is None:
-            series_name = random.choice(self.df.columns)
+            if series is not None:
+                series_name = series
+            else:
+                series_name = random.choice(self.df.columns)
         if title is None:
             title = (
                 series_name[0:50]
                 + f" with {self.anomaly_detector_params['method']} holidays"
             )
         fig, ax = plt.subplots()
         self.df[series_name].plot(ax=ax, title=title, **plot_kwargs)
```

### Comparing `autots-0.5.8/autots/evaluator/auto_model.py` & `autots-0.6.0/autots/evaluator/auto_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from math import ceil
 import numpy as np
 import pandas as pd
 import datetime
 import json
 from hashlib import md5
 from autots.tools.transform import RandomTransform, GeneralTransformer, shared_trans
-from autots.models.base import PredictionObject
+from autots.models.base import PredictionObject, ModelObject
 from autots.models.ensemble import (
     EnsembleForecast,
     generalize_horizontal,
     horizontal_aliases,
     parse_horizontal,
 )
 from autots.tools.shaping import infer_frequency
@@ -634,38 +634,16 @@
         )
     else:
         raise AttributeError(
             ("Model String '{}' not a recognized model type").format(model)
         )
 
 
-def ModelPrediction(
-    df_train,
-    forecast_length: int,
-    transformation_dict: dict,
-    model_str: str,
-    parameter_dict: dict,
-    frequency: str = 'infer',
-    prediction_interval: float = 0.9,
-    no_negatives: bool = False,
-    constraint: float = None,
-    future_regressor_train=None,
-    future_regressor_forecast=None,
-    holiday_country: str = 'US',
-    startTimeStamps=None,
-    grouping_ids=None,
-    fail_on_forecast_nan: bool = True,
-    return_model: bool = False,
-    random_seed: int = 2020,
-    verbose: int = 0,
-    n_jobs: int = None,
-    current_model_file: str = None,
-    model_count: int = 0,
-):
-    """Feed parameters into modeling pipeline
+class ModelPrediction(ModelObject):
+    """Feed parameters into modeling pipeline. A class object, does NOT work with ensembles.
 
     Args:
         df_train (pandas.DataFrame): numeric training dataset of DatetimeIndex and series as cols
         forecast_length (int): number of periods to forecast
         transformation_dict (dict): a dictionary of outlier, fillNA, and transformation methods to be used
         model_str (str): a string to be direct to the appropriate model, used in ModelMonster
         frequency (str): str representing frequency alias of time series
@@ -680,150 +658,214 @@
         return_model (bool): if True, forecast will have .model and .tranformer attributes set to model object.
         n_jobs (int): number of processes
         current_model_file (str): file path to write to disk of current model params (for debugging if computer crashes). .json is appended
 
     Returns:
         PredictionObject (autots.PredictionObject): Prediction from AutoTS model object
     """
-    transformationStartTime = datetime.datetime.now()
-    if current_model_file is not None:
-        try:
-            with open(f'{current_model_file}.json', 'w') as f:
-                json.dump(
-                    {
-                        "model_number": model_count,
-                        "model_name": model_str,
-                        "model_param_dict": parameter_dict,
-                        "model_transform_dict": transformation_dict,
-                    },
-                    f,
-                )
-        except Exception as e:
-            error_msg = f"failed to write {current_model_file} with error {repr(e)}"
-            try:
-                with open(f'{current_model_file}_failure.json', 'w') as f:
-                    f.write(error_msg)
-            except Exception:
-                pass
-            print(error_msg)
 
-    transformer_object = GeneralTransformer(
-        **transformation_dict, n_jobs=n_jobs, holiday_country=holiday_country
-    )
-    df_train_transformed = transformer_object._fit(df_train)
+    def __init__(
+        self,
+        forecast_length: int,
+        transformation_dict: dict,
+        model_str: str,
+        parameter_dict: dict,
+        frequency: str = 'infer',
+        prediction_interval: float = 0.9,
+        no_negatives: bool = False,
+        constraint: float = None,
+        holiday_country: str = 'US',
+        startTimeStamps=None,
+        grouping_ids=None,
+        fail_on_forecast_nan: bool = True,
+        return_model: bool = False,
+        random_seed: int = 2020,
+        verbose: int = 0,
+        n_jobs: int = None,
+        current_model_file: str = None,
+        model_count: int = 0,
+    ):
+        self.forecast_length = forecast_length
+        self.transformation_dict = transformation_dict
+        self.model_str = model_str
+        self.parameter_dict = parameter_dict
+        self.frequency = frequency
+        self.prediction_interval = prediction_interval
+        self.no_negatives = no_negatives
+        self.constraint = constraint
+        self.holiday_country = holiday_country
+        self.fail_on_forecast_nan = fail_on_forecast_nan
+        self.return_model = return_model
+        self.random_seed = random_seed
+        self.verbose = verbose
+        self.n_jobs = n_jobs
+        self.current_model_file = current_model_file
+        self.model_count = model_count
+        self.transformer_object = GeneralTransformer(
+            **transformation_dict, n_jobs=n_jobs, holiday_country=holiday_country
+        )
+        self.model = ModelMonster(
+            model_str,
+            parameters=parameter_dict,
+            frequency=frequency,
+            prediction_interval=prediction_interval,
+            holiday_country=holiday_country,
+            random_seed=random_seed,
+            verbose=verbose,
+            forecast_length=forecast_length,
+            n_jobs=n_jobs,
+        )
+        self.name = "ModelPrediction"
+        self._fit_complete = False
 
-    # make sure regressor has same length. This could be a problem if wrong size regressor is passed.
-    if future_regressor_train is not None:
-        future_regressor_train = future_regressor_train.reindex(df_train.index)
-
-    transformation_runtime = datetime.datetime.now() - transformationStartTime
-    # from autots.evaluator.auto_model import ModelMonster
-    model = ModelMonster(
-        model_str,
-        parameters=parameter_dict,
-        frequency=frequency,
-        prediction_interval=prediction_interval,
-        holiday_country=holiday_country,
-        random_seed=random_seed,
-        verbose=verbose,
-        forecast_length=forecast_length,
-        n_jobs=n_jobs,
-    )
-    model = model.fit(df_train_transformed, future_regressor=future_regressor_train)
-    df_forecast = model.predict(
-        forecast_length=forecast_length, future_regressor=future_regressor_forecast
-    )
+    def fit(self, df, future_regressor=None):
+        self.df = df
+        transformationStartTime = datetime.datetime.now()
+        if self.current_model_file is not None:
+            try:
+                with open(f'{self.current_model_file}.json', 'w') as f:
+                    json.dump(
+                        {
+                            "model_number": self.model_count,
+                            "model_name": self.model_str,
+                            "model_param_dict": self.parameter_dict,
+                            "model_transform_dict": self.transformation_dict,
+                        },
+                        f,
+                    )
+            except Exception as e:
+                error_msg = (
+                    f"failed to write {self.current_model_file} with error {repr(e)}"
+                )
+                try:
+                    with open(f'{self.current_model_file}_failure.json', 'w') as f:
+                        f.write(error_msg)
+                except Exception:
+                    pass
+                print(error_msg)
+
+        df_train_transformed = self.transformer_object._fit(df)
+
+        # make sure regressor has same length. This could be a problem if wrong size regressor is passed.
+        if future_regressor is not None:
+            future_regressor = future_regressor.reindex(df.index)
+
+        self.transformation_runtime = datetime.datetime.now() - transformationStartTime
+        # from autots.evaluator.auto_model import ModelMonster
+        self.model = self.model.fit(
+            df_train_transformed, future_regressor=future_regressor
+        )
+        self._fit_complete = True
+        return self
 
-    # THIS CHECKS POINT FORECAST FOR NULLS BUT NOT UPPER/LOWER FORECASTS
-    # can maybe remove this eventually and just keep the later one
-    if fail_on_forecast_nan:
-        if not np.isfinite(np.max(df_forecast.forecast.to_numpy())):
-            raise ValueError(
-                "Model {} returned NaN for one or more series. fail_on_forecast_nan=True".format(
-                    model_str
+    def predict(self, forecast_length=None, future_regressor=None):
+        if forecast_length is None:
+            forecast_length = self.forecast_length
+        if not self._fit_complete:
+            raise ValueError("Model not yet fit.")
+        df_forecast = self.model.predict(
+            forecast_length=self.forecast_length, future_regressor=future_regressor
+        )
+
+        # THIS CHECKS POINT FORECAST FOR NULLS BUT NOT UPPER/LOWER FORECASTS
+        # can maybe remove this eventually and just keep the later one
+        if self.fail_on_forecast_nan:
+            if not np.isfinite(np.max(df_forecast.forecast.to_numpy())):
+                raise ValueError(
+                    "Model {} returned NaN for one or more series. fail_on_forecast_nan=True".format(
+                        self.model_str
+                    )
                 )
-            )
 
-    transformationStartTime = datetime.datetime.now()
-    # Inverse the transformations, NULL FILLED IN UPPER/LOWER ONLY
-    # forecast inverse MUST come before upper and lower bounds inverse
-    df_forecast.forecast = pd.DataFrame(
-        transformer_object.inverse_transform(df_forecast.forecast)
-    )
-    df_forecast.lower_forecast = pd.DataFrame(
-        transformer_object.inverse_transform(
-            df_forecast.lower_forecast, fillzero=True, bounds=True
-        )
-    )
-    df_forecast.upper_forecast = pd.DataFrame(
-        transformer_object.inverse_transform(
-            df_forecast.upper_forecast, fillzero=True, bounds=True
+        transformationStartTime = datetime.datetime.now()
+        # Inverse the transformations, NULL FILLED IN UPPER/LOWER ONLY
+        # forecast inverse MUST come before upper and lower bounds inverse
+        df_forecast.forecast = pd.DataFrame(
+            self.transformer_object.inverse_transform(df_forecast.forecast)
+        )
+        df_forecast.lower_forecast = pd.DataFrame(
+            self.transformer_object.inverse_transform(
+                df_forecast.lower_forecast, fillzero=True, bounds=True
+            )
         )
-    )
-    # CHECK Forecasts are proper length!
-    if df_forecast.forecast.shape[0] != forecast_length:
-        raise ValueError(f"Model {model_str} returned improper forecast_length")
-
-    if df_forecast.forecast.shape[1] != df_train.shape[1]:
-        raise ValueError("Model failed to return correct number of series.")
-
-    df_forecast.transformation_parameters = transformation_dict
-    # Remove negatives if desired
-    # There's df.where(df_forecast.forecast > 0, 0) or  df.clip(lower = 0), not sure which faster
-    if no_negatives:
-        df_forecast.lower_forecast = df_forecast.lower_forecast.clip(lower=0)
-        df_forecast.forecast = df_forecast.forecast.clip(lower=0)
-        df_forecast.upper_forecast = df_forecast.upper_forecast.clip(lower=0)
-
-    if constraint is not None:
-        if isinstance(constraint, dict):
-            constraint_method = constraint.get("constraint_method", "quantile")
-            constraint_regularization = constraint.get("constraint_regularization", 1)
-            lower_constraint = constraint.get("lower_constraint", 0)
-            upper_constraint = constraint.get("upper_constraint", 1)
-            bounds = constraint.get("bounds", False)
-        else:
-            constraint_method = "stdev_min"
-            lower_constraint = float(constraint)
-            upper_constraint = float(constraint)
-            constraint_regularization = 1
-            bounds = False
-        if verbose > 3:
-            print(
-                f"Using constraint with method: {constraint_method}, {constraint_regularization}, {lower_constraint}, {upper_constraint}, {bounds}"
+        df_forecast.upper_forecast = pd.DataFrame(
+            self.transformer_object.inverse_transform(
+                df_forecast.upper_forecast, fillzero=True, bounds=True
             )
-
-        df_forecast = df_forecast.apply_constraints(
-            constraint_method,
-            constraint_regularization,
-            upper_constraint,
-            lower_constraint,
-            bounds,
-            df_train,
         )
+        # CHECK Forecasts are proper length!
+        if df_forecast.forecast.shape[0] != self.forecast_length:
+            raise ValueError(
+                f"Model {self.model_str} returned improper forecast_length"
+            )
 
-    transformation_runtime = transformation_runtime + (
-        datetime.datetime.now() - transformationStartTime
-    )
-    df_forecast.transformation_runtime = transformation_runtime
+        if df_forecast.forecast.shape[1] != self.df.shape[1]:
+            raise ValueError("Model failed to return correct number of series.")
 
-    if return_model:
-        df_forecast.model = model
-        df_forecast.transformer = transformer_object
-
-    # THIS CHECKS POINT FORECAST FOR NULLS BUT NOT UPPER/LOWER FORECASTS
-    if fail_on_forecast_nan:
-        if not np.isfinite(np.max(df_forecast.forecast.to_numpy())):
-            raise ValueError(
-                "Model returned NaN due to a preprocessing transformer {}. fail_on_forecast_nan=True".format(
-                    str(transformation_dict)
+        df_forecast.transformation_parameters = self.transformation_dict
+        # Remove negatives if desired
+        # There's df.where(df_forecast.forecast > 0, 0) or  df.clip(lower = 0), not sure which faster
+        if self.no_negatives:
+            df_forecast.lower_forecast = df_forecast.lower_forecast.clip(lower=0)
+            df_forecast.forecast = df_forecast.forecast.clip(lower=0)
+            df_forecast.upper_forecast = df_forecast.upper_forecast.clip(lower=0)
+
+        if self.constraint is not None:
+            if isinstance(self.constraint, dict):
+                constraint_method = self.constraint.get("constraint_method", "quantile")
+                constraint_regularization = self.constraint.get(
+                    "constraint_regularization", 1
+                )
+                lower_constraint = self.constraint.get("lower_constraint", 0)
+                upper_constraint = self.constraint.get("upper_constraint", 1)
+                bounds = self.constraint.get("bounds", False)
+            else:
+                constraint_method = "stdev_min"
+                lower_constraint = float(self.constraint)
+                upper_constraint = float(self.constraint)
+                constraint_regularization = 1
+                bounds = False
+            if self.verbose > 3:
+                print(
+                    f"Using constraint with method: {constraint_method}, {constraint_regularization}, {lower_constraint}, {upper_constraint}, {bounds}"
                 )
+
+            df_forecast = df_forecast.apply_constraints(
+                constraint_method,
+                constraint_regularization,
+                upper_constraint,
+                lower_constraint,
+                bounds,
+                self.df,
             )
 
-    return df_forecast
+        self.transformation_runtime = self.transformation_runtime + (
+            datetime.datetime.now() - transformationStartTime
+        )
+        df_forecast.transformation_runtime = self.transformation_runtime
+
+        if self.return_model:
+            df_forecast.model = self.model
+            df_forecast.transformer = self.transformer_object
+
+        # THIS CHECKS POINT FORECAST FOR NULLS BUT NOT UPPER/LOWER FORECASTS
+        if self.fail_on_forecast_nan:
+            if not np.isfinite(np.max(df_forecast.forecast.to_numpy())):
+                raise ValueError(
+                    "Model returned NaN due to a preprocessing transformer {}. fail_on_forecast_nan=True".format(
+                        str(self.transformation_dict)
+                    )
+                )
+        sys.stdout.flush()
+
+        return df_forecast
+
+    def fit_data(self, df, future_regressor=None):
+        self.df = df
+        self.model.fit_data(df, future_regressor)
 
 
 class TemplateEvalObject(object):
     """Object to contain all the failures!.
 
     Attributes:
         full_mae_ids (list): list of model_ids corresponding to full_mae_errors
@@ -1132,14 +1174,17 @@
         for index, row in ens_template.iterrows():
             # recursive recursion!
             try:
                 if all_series is not None:
                     test_mod = row['ID']
                     horizontal_subset = parse_horizontal(all_series, model_id=test_mod)
 
+                if verbose >= 2:
+                    p = f"Ensemble {model_param_dict['model_name']} component {index} of {total_ens} {row['Model']} started"
+                    print(p)
                 df_forecast = model_forecast(
                     model_name=row['Model'],
                     model_param_dict=row['ModelParameters'],
                     model_transform_dict=row['TransformationParameters'],
                     df_train=df_train,
                     forecast_length=forecast_length,
                     frequency=frequency,
@@ -1171,17 +1216,14 @@
                     + df_forecast.transformation_runtime
                 )
                 forecasts_runtime[model_id] = total_runtime
                 forecasts[model_id] = df_forecast.forecast
                 upper_forecasts[model_id] = df_forecast.upper_forecast
                 lower_forecasts[model_id] = df_forecast.lower_forecast
                 # print(f"{model_param_dict['model_name']} with shape {df_forecast.forecast.shape}")
-                if verbose >= 2:
-                    p = f"Ensemble {model_param_dict['model_name']} component {index + 1} of {total_ens} {row['Model']} succeeded"
-                    print(p)
             except Exception as e:
                 # currently this leaves no key/value for models that fail
                 if verbose >= 1:  # 1
                     print(tb.format_exc())
                     p = f"FAILED: Ensemble {model_param_dict['model_name']} component {index + 1} of {total_ens} {row['Model']} with error: {repr(e)}"
                     print(p)
         ens_forecast = EnsembleForecast(
@@ -1219,40 +1261,38 @@
         ):
             df_train_low = df_train.reindex(copy=True, columns=horizontal_subset)
             # print(f"Reducing to subset for {model_name} with {df_train_low.columns}")
         else:
             df_train_low = df_train.copy()
             full_model_created = True
 
-        df_forecast = ModelPrediction(
-            df_train_low,
-            forecast_length,
-            model_transform_dict,
-            model_name,
-            model_param_dict,
+        model = ModelPrediction(
+            forecast_length=forecast_length,
+            transformation_dict=model_transform_dict,
+            model_str=model_name,
+            parameter_dict=model_param_dict,
             frequency=frequency,
             prediction_interval=prediction_interval,
             no_negatives=no_negatives,
             constraint=constraint,
-            future_regressor_train=future_regressor_train,
-            future_regressor_forecast=future_regressor_forecast,
             grouping_ids=grouping_ids,
             holiday_country=holiday_country,
             random_seed=random_seed,
             verbose=verbose,
             fail_on_forecast_nan=fail_on_forecast_nan,
             startTimeStamps=startTimeStamps,
             n_jobs=n_jobs,
             return_model=return_model,
             current_model_file=current_model_file,
             model_count=model_count,
         )
-
-        sys.stdout.flush()
-        return df_forecast
+        model = model.fit(df_train_low, future_regressor_train)
+        return model.predict(
+            forecast_length, future_regressor=future_regressor_forecast
+        )
 
 
 def _ps_metric(per_series_metrics, metric, model_id):
     cur_mae = per_series_metrics.loc[metric]
     cur_mae = pd.DataFrame(cur_mae).transpose()
     cur_mae.index = [model_id]
     return cur_mae
```

### Comparing `autots-0.5.8/autots/evaluator/auto_ts.py` & `autots-0.6.0/autots/evaluator/auto_ts.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,22 +28,23 @@
     generate_score_per_series,
     model_forecast,
     validation_aggregation,
     back_forecast,
     remove_leading_zeros,
     horizontal_template_to_model_list,
     create_model_id,
+    ModelPrediction,
 )
 from autots.models.ensemble import (
     EnsembleTemplateGenerator,
     HorizontalTemplateGenerator,
     generate_mosaic_template,
     generate_crosshair_score,
 )
-from autots.models.model_list import model_lists, no_shared
+from autots.models.model_list import model_lists, no_shared, update_fit
 from autots.tools import cpu_count
 from autots.evaluator.validation import (
     validate_num_validations,
     generate_validation_indices,
 )
 
 
@@ -76,14 +77,15 @@
         initial_template (str): 'Random' - randomly generates starting template, 'General' uses template included in package, 'General+Random' - both of previous. Also can be overriden with self.import_template()
         random_seed (int): random seed allows (slightly) more consistent results.
         holiday_country (str): passed through to Holidays package for some models.
         subset (int): maximum number of series to evaluate at once. Useful to speed evaluation when many series are input.
             takes a new subset of columns on each validation, unless mosaic ensembling, in which case columns are the same in each validation
         aggfunc (str): if data is to be rolled up to a higher frequency (daily -> monthly) or duplicate timestamps are included. Default 'first' removes duplicates, for rollup try 'mean' or np.sum.
             Beware numeric aggregations like 'mean' will not work with non-numeric inputs.
+            Numeric aggregations like 'sum' will also change nan values to 0
         na_tolerance (float): 0 to 1. Series are dropped if they have more than this percent NaN. 0.95 here would allow series containing up to 95% NaN values.
         metric_weighting (dict): weights to assign to metrics, effecting how the ranking score is generated.
         drop_most_recent (int): option to drop n most recent data points. Useful, say, for monthly sales data where the current (unfinished) month is included.
             occurs after any aggregration is applied, so will be whatever is specified by frequency, will drop n frequencies
         drop_data_older_than_periods (int): take only the n most recent timestamps
         model_list (list): str alias or list of names of model objects to use
             now can be a dictionary of {"model": prob} but only affects starting random templates. Genetic algorithim takes from there.
@@ -152,15 +154,15 @@
         self,
         forecast_length: int = 14,
         frequency: str = 'infer',
         prediction_interval: float = 0.9,
         max_generations: int = 10,
         no_negatives: bool = False,
         constraint: float = None,
-        ensemble: str = 'auto',
+        ensemble: str = None,  # 'auto',
         initial_template: str = 'General+Random',
         random_seed: int = 2022,
         holiday_country: str = 'US',
         subset: int = None,
         aggfunc: str = 'first',
         na_tolerance: float = 1,
         metric_weighting: dict = {
@@ -174,15 +176,15 @@
             'spl_weighting': 3,
             'containment_weighting': 0,
             'contour_weighting': 1,
             'runtime_weighting': 0.05,
             'oda_weighting': 0.001,
         },
         drop_most_recent: int = 0,
-        drop_data_older_than_periods: int = 100000,
+        drop_data_older_than_periods: int = None,
         model_list: str = 'default',
         transformer_list: dict = "auto",
         transformer_max_depth: int = 6,
         models_mode: str = "random",
         num_validations: int = "auto",
         models_to_validate: float = 0.15,
         max_per_model_class: int = None,
@@ -413,32 +415,35 @@
 
                 full_params['transformations'] = transformations
                 full_params['transformation_params'] = transformation_params
                 self.initial_template.loc[
                     index, 'TransformationParameters'
                 ] = json.dumps(full_params)
 
-        self.best_model = pd.DataFrame()
         self.regressor_used = False
         # do not add 'ID' to the below unless you want to refactor things.
         self.template_cols = [
             'Model',
             'ModelParameters',
             'TransformationParameters',
             'Ensemble',
         ]
         self.template_cols_id = (
             self.template_cols
             if "ID" in self.template_cols
             else ['ID'] + self.template_cols
         )
+        self.grouping_ids = None
         self.initial_results = TemplateEvalObject()
+        self.best_model = pd.DataFrame()
+        self.best_model_id = ""
         self.best_model_name = ""
         self.best_model_params = {}
         self.best_model_transformation_params = ""
+        self.best_model_ensemble = -1
         self.traceback = True if verbose > 1 else False
         self.future_regressor_train = None
         self.validation_train_indexes = []
         self.validation_test_indexes = []
         self.preclean_transformer = None
         self.score_per_series = None
         self.best_model_non_horizontal = None
@@ -455,14 +460,15 @@
         }
         self.seasonal_validation_params = {
             'window_size': 10,
             'distance_metric': 'mae',
             'datepart_method': 'common_fourier_rw',
         }
         self.model_count = 0
+        self.model = None  # intended for fit_data update models only
 
         if verbose > 2:
             msg = '"Hello. Would you like to destroy some evil today?" - Sanderson'
             # unicode may not be supported on all platforms
             try:
                 print("\N{dagger} " + msg)
             except Exception:
@@ -482,15 +488,17 @@
                         "distance",
                         "horizontal",
                         "horizontal-max",
                     ],
                 ],
                 [0.3, 0.1, 0.2, 0.2],
             )[0]
+            max_generations = random.choices([5, 15, 25, 50], [0.2, 0.5, 0.1, 0.4])[0]
         else:
+            max_generations = random.choices([15, 25, 50, 200], [0.2, 0.5, 0.2, 0.1])[0]
             ensemble_choice = random.choices(
                 [
                     None,
                     ['simple'],
                     ['simple', 'horizontal-max'],
                     [
                         'simple',
@@ -502,15 +510,15 @@
                         'mosaic-crosshair',
                         "subsample",
                         "mlensemble",
                     ],
                 ],
                 [0.3, 0.1, 0.2, 0.2],
             )[0]
-        if method in ["full", "fast"]:
+        if method in ["full", "fast", "superfast"]:
             metric_weighting = {
                 'smape_weighting': random.choices([0, 1, 5, 10], [0.3, 0.2, 0.3, 0.1])[
                     0
                 ],
                 'mae_weighting': random.choices([0, 1, 3, 5], [0.1, 0.3, 0.3, 0.3])[0],
                 'rmse_weighting': random.choices([0, 1, 3, 5], [0.1, 0.3, 0.3, 0.3])[0],
                 'made_weighting': random.choices([0, 1, 3, 5], [0.7, 0.3, 0.1, 0.05])[
@@ -539,14 +547,18 @@
                 'smoothness_weighting': random.choices(
                     [0, 0.05, 3, 1, -0.5, -3], [0.4, 0.1, 0.1, 0.1, 0.2, 0.1]
                 )[0],
                 'ewmae_weighting': random.choices(
                     [0, 0.05, 0.3, 1, 5], [0.1, 0.6, 0.2, 0.1, 0.1]
                 )[0],
             }
+            validation_method = random.choices(
+                ['backwards', 'even', 'similarity', 'seasonal 364', 'seasonal'],
+                [0.4, 0.1, 0.3, 0.3, 0.2],
+            )[0]
         else:
             metric_weighting = {
                 'smape_weighting': random.choices([0, 1, 5, 10], [0.3, 0.2, 0.3, 0.1])[
                     0
                 ],
                 'mae_weighting': random.choices([0, 1, 3, 5], [0.1, 0.3, 0.3, 0.3])[0],
                 'rmse_weighting': random.choices([0, 1, 3, 5], [0.1, 0.3, 0.3, 0.3])[0],
@@ -566,14 +578,18 @@
                 'contour_weighting': random.choices(
                     [0, 1, 3, 5], [0.7, 0.2, 0.05, 0.05]
                 )[0],
                 'runtime_weighting': random.choices(
                     [0, 0.05, 0.3, 1], [0.1, 0.6, 0.2, 0.1]
                 )[0],
             }
+            validation_method = random.choices(
+                ['backwards', 'even', 'similarity', 'seasonal 364'],
+                [0.4, 0.1, 0.3, 0.3],
+            )[0]
         preclean_choice = random.choices(
             [
                 None,
                 {
                     "fillna": "ffill",
                     "transformations": {0: "EWMAFilter"},
                     "transformation_params": {
@@ -608,45 +624,138 @@
                                 "iqr_threshold": 2.0,
                                 "iqr_quantiles": [0.4, 0.6],
                             },
                             "fillna": 'ffill',
                         }
                     },
                 },
+                {
+                    'fillna': None,
+                    'transformations': {
+                        '0': 'ClipOutliers',
+                        '1': 'RegressionFilter',
+                        '2': 'ClipOutliers',
+                    },
+                    'transformation_params': {
+                        '0': {
+                            'method': 'remove',
+                            'std_threshold': 2.5,
+                            'fillna': None,
+                        },  # "SeasonalityMotifImputerLinMix"
+                        '1': {
+                            "sigma": 2,
+                            "rolling_window": 90,
+                            "run_order": "season_first",
+                            "regression_params": {
+                                "regression_model": {
+                                    "model": "ElasticNet",
+                                    "model_params": {},
+                                },
+                                "datepart_method": ['common_fourier'],
+                                "polynomial_degree": None,
+                                "transform_dict": None,
+                                "holiday_countries_used": False,
+                            },
+                            "holiday_params": None,
+                        },
+                        '2': {
+                            'method': 'remove',
+                            'std_threshold': 3.0,
+                            'fillna': "SeasonalityMotifImputerLinMix",
+                        },
+                    },
+                },
+                {
+                    'fillna': None,
+                    'transformations': {
+                        '0': 'ClipOutliers',
+                        '1': "LevelShiftMagic",
+                        '2': 'RegressionFilter',
+                        '3': 'ClipOutliers',
+                    },
+                    'transformation_params': {
+                        '0': {
+                            'method': 'remove',
+                            'std_threshold': 2.5,
+                            'fillna': None,
+                        },  # "SeasonalityMotifImputerLinMix"
+                        '1': {
+                            'window_size': 90,
+                            'alpha': 2.5,
+                            'grouping_forward_limit': 3,
+                            'max_level_shifts': 5,
+                            'alignment': 'average',
+                        },
+                        '2': {
+                            "sigma": 2,
+                            "rolling_window": 90,
+                            "run_order": "season_first",
+                            "regression_params": {
+                                "regression_model": {
+                                    "model": "ElasticNet",
+                                    "model_params": {},
+                                },
+                                "datepart_method": ['common_fourier'],
+                                "polynomial_degree": None,
+                                "transform_dict": None,
+                                "holiday_countries_used": False,
+                            },
+                            "holiday_params": None,
+                        },
+                        '3': {
+                            'method': 'remove',
+                            'std_threshold': 3.0,
+                            'fillna': "SeasonalityMotifImputerLinMix",
+                        },
+                    },
+                },
+                {
+                    "fillna": None,
+                    "transformations": {"0": "LocalLinearTrend"},
+                    "transformation_params": {
+                        "0": {
+                            'rolling_window': 30,
+                            'n_tails': 0.1,
+                            'n_future': 0.2,
+                            'method': 'mean',
+                            'macro_micro': True,
+                        },
+                    },
+                },
                 'random',
             ],
-            [0.9, 0.1, 0.05, 0.1, 0.1, 0.1, 0.1],
+            [0.9, 0.1, 0.05, 0.1, 0.1, 0.1, 0.1, 0.05, 0.15, 0.1],
         )[0]
         if preclean_choice == "random":
             preclean_choice = RandomTransform(
                 transformer_list="fast", transformer_max_depth=2
             )
         if method == 'full':
             model_list = random.choices(
                 [
                     'fast',
                     'superfast',
                     'default',
-                    'fast_parallel',
+                    'fast_parallel_no_arima',
                     'all',
                     'motifs',
                     'no_shared_fast',
                     'multivariate',
                     'univariate',
                     'all_result_path',
                     'regressions',
                     'best',
                     'regressor',
                     'probabilistic',
                     'no_shared',
                 ],
                 [
                     0.2,
-                    0.2,
-                    0.2,
+                    0.4,
+                    0.1,
                     0.2,
                     0.01,
                     0.1,
                     0.1,
                     0.05,
                     0.05,
                     0.05,
@@ -660,46 +769,41 @@
         elif method == 'fast':
             model_list = random.choices(
                 [
                     'fast',
                     'superfast',
                     'motifs',
                     'no_shared_fast',
+                    'fast_parallel_no_arima',
                 ],
                 [
                     0.2,
+                    0.3,
                     0.2,
                     0.2,
-                    0.2,
+                    0.05,
                 ],
             )[0]
+        elif method == "superfast":
+            model_list = 'superfast'
         else:
             model_list = random.choices(
                 [
                     'fast',
                     'superfast',
                     'default',
                     'fast_parallel',
                     'motifs',
                     'no_shared_fast',
                 ],
-                [0.2, 0.2, 0.2, 0.2, 0.05, 0.1],
-            )[0]
-        if method in ['full', 'fast']:
-            validation_method = random.choices(
-                ['backwards', 'even', 'similarity', 'seasonal 364', 'seasonal'],
-                [0.4, 0.1, 0.3, 0.3, 0.2],
-            )[0]
-        else:
-            validation_method = random.choices(
-                ['backwards', 'even', 'similarity', 'seasonal 364'],
-                [0.4, 0.1, 0.3, 0.3],
+                [0.2, 0.3, 0.2, 0.2, 0.05, 0.1],
             )[0]
+
         return {
-            'max_generations': random.choices([5, 15, 25, 50], [0.2, 0.5, 0.1, 0.4])[0],
+            'max_generations': max_generations,
             'model_list': model_list,
             'transformer_list': random.choices(
                 ['all', 'fast', 'superfast'],
                 [0.2, 0.5, 0.3],
             )[0],
             'transformer_max_depth': random.choices(
                 [1, 2, 4, 6, 8, 10],
@@ -774,98 +878,27 @@
                 res3 = ", ".join(base_res['spl'].astype(str).tolist())
                 len_list = list(range(base_res.shape[0]))
                 res_len = ", ".join([str(x) for x in len_list])
                 return f"Initiated AutoTS object with best model: \n{self.best_model_name}\n{self.best_model_transformation_params}\n{self.best_model_params}\nValidation: {res_len}\nSMAPE: {res}\nMAE: {res2}\nSPL: {res3}"
             except Exception:
                 return "Initiated AutoTS object"
 
-    def fit(
+    def fit_data(
         self,
         df,
-        date_col: str = None,
-        value_col: str = None,
-        id_col: str = None,
+        date_col=None,
+        value_col=None,
+        id_col=None,
         future_regressor=None,
-        weights: dict = {},
-        result_file: str = None,
-        grouping_ids=None,
-        validation_indexes: list = None,
+        weights={},
     ):
-        """Train algorithm given data supplied.
-
-        Args:
-            df (pandas.DataFrame): Datetime Indexed dataframe of series, or dataframe of three columns as below.
-            date_col (str): name of datetime column
-            value_col (str): name of column containing the data of series.
-            id_col (str): name of column identifying different series.
-            future_regressor (numpy.Array): single external regressor matching train.index
-            weights (dict): {'colname1': 2, 'colname2': 5} - increase importance of a series in metric evaluation. Any left blank assumed to have weight of 1.
-                pass the alias 'mean' as a str ie `weights='mean'` to automatically use the mean value of a series as its weight
-                available aliases: mean, median, min, max
-            result_file (str): results saved on each new generation. Does not include validation rounds.
-                ".csv" save model results table.
-                ".pickle" saves full object, including ensemble information.
-            grouping_ids (dict): currently a one-level dict containing series_id:group_id mapping.
-                used in 0.2.x but not 0.3.x+ versions. retained for potential future use
-        """
-        self.weights = weights
+        """Part of the setup that involves fitting the initial data but not running any models."""
         self.date_col = date_col
         self.value_col = value_col
         self.id_col = id_col
-        self.grouping_ids = grouping_ids
-
-        # import mkl
-        # so this actually works it seems, on all sub process models
-        # mkl.set_num_threads_local(8)
-
-        # convert class variables to local variables (makes testing easier)
-        forecast_length = self.forecast_length
-        if self.validation_method == "custom":
-            self.validation_indexes = validation_indexes
-            assert (
-                validation_indexes is not None
-            ), "validation_indexes needs to be filled with 'custom' validation"
-            # if auto num_validation, use as many as provided in custom
-            if self.num_validations in ["auto", 'max']:
-                self.num_validations == len(validation_indexes) - 1
-            else:
-                assert len(validation_indexes) >= (
-                    self.num_validations + 1
-                ), "validation_indexes needs to be >= num_validations + 1 with 'custom' validation"
-        else:
-            self.validation_indexes = []
-        # flag if weights are given
-        if bool(weights):
-            weighted = True
-        else:
-            weighted = False
-        self.weighted = weighted
-        prediction_interval = self.prediction_interval
-        random_seed = self.random_seed
-        metric_weighting = self.metric_weighting
-        verbose = self.verbose
-        template_cols = self.template_cols
-
-        # shut off warnings if running silently
-        if verbose <= 0:
-            import warnings
-
-            warnings.filterwarnings("ignore")
-
-        # clean up result_file input, if given.
-        if result_file is not None:
-            formats = ['.csv', '.pickle']
-            if not any(x in result_file for x in formats):
-                print("result_file must be a valid str with .csv or .pickle")
-                result_file = None
-
-        # set random seeds for environment
-        random_seed = abs(int(random_seed))
-        random.seed(random_seed)
-        np.random.seed(random_seed)
 
         # convert data to wide format
         if date_col is None and value_col is None:
             df_wide = pd.DataFrame(df).copy()
             assert (
                 type(df_wide.index) is pd.DatetimeIndex
             ), "df index is not pd.DatetimeIndex"
@@ -918,19 +951,25 @@
                 ens_piece2 = ""
             if "mosaic" in self.ensemble:
                 ens_piece3 = "mosaic"
             else:
                 ens_piece3 = ""
             # self.ensemble = ens_piece1 + "," + ens_piece2 + "," + ens_piece3
             self.ensemble = [ens_piece1, ens_piece2, ens_piece3]
-        ensemble = self.ensemble
+
         # because horizontal cannot handle non-string columns/series_ids
         if any(x in self.ensemble for x in self.h_ens_list):
             df_wide_numeric.columns = [str(xc) for xc in df_wide_numeric.columns]
 
+        # flag if weights are given
+        if bool(weights):
+            self.weighted = True
+        else:
+            self.weighted = False
+
         # use "mean" to assign weight as mean
         if self.weighted:
             if weights == 'mean':
                 weights = df_wide_numeric.mean(axis=0).to_dict()
             elif weights == 'median':
                 weights = df_wide_numeric.median(axis=0).to_dict()
             elif weights == 'min':
@@ -958,60 +997,166 @@
                 holiday_country=self.holiday_country,
             )
             df_wide_numeric = self.preclean_transformer.fit_transform(df_wide_numeric)
 
         self.df_wide_numeric = df_wide_numeric
         self.startTimeStamps = df_wide_numeric.notna().idxmax()
 
+        if future_regressor is not None:
+            if not isinstance(future_regressor, pd.DataFrame):
+                future_regressor = pd.DataFrame(future_regressor)
+            if future_regressor.empty:
+                raise ValueError(
+                    "future_regressor empty, pass None if intending not to use"
+                )
+            if not isinstance(future_regressor.index, pd.DatetimeIndex):
+                # should be same length as history as this is not yet the predict step
+                future_regressor.index = df_wide_numeric.index
+            # test shape
+            if future_regressor.shape[0] != self.df_wide_numeric.shape[0]:
+                print(
+                    "future_regressor row count does not match length of training data"
+                )
+                time.sleep(2)
+
+            # handle any non-numeric data, crudely
+            self.regr_num_trans = NumericTransformer(verbose=self.verbose)
+            self.future_regressor_train = self.regr_num_trans.fit_transform(
+                future_regressor
+            )
+
         # check how many validations are possible given the length of the data.
         self.num_validations = validate_num_validations(
             self.validation_method,
             self.num_validations,
-            df_wide_numeric,
-            forecast_length,
+            self.df_wide_numeric,
+            self.forecast_length,
             self.min_allowed_train_percent,
             self.verbose,
         )
 
         # generate validation indices (so it can fail now, not after all the generations)
         self.validation_indexes = generate_validation_indices(
             self.validation_method,
-            forecast_length,
+            self.forecast_length,
             self.num_validations,
-            df_wide_numeric,
+            self.df_wide_numeric,
             validation_params=self.similarity_validation_params
             if self.validation_method == "similarity"
             else self.seasonal_validation_params,
             preclean=None,
             verbose=0,
         )
 
+    def fit(
+        self,
+        df,
+        date_col: str = None,
+        value_col: str = None,
+        id_col: str = None,
+        future_regressor=None,
+        weights: dict = {},
+        result_file: str = None,
+        grouping_ids=None,
+        validation_indexes: list = None,
+    ):
+        """Train algorithm given data supplied.
+
+        Args:
+            df (pandas.DataFrame): Datetime Indexed dataframe of series, or dataframe of three columns as below.
+            date_col (str): name of datetime column
+            value_col (str): name of column containing the data of series.
+            id_col (str): name of column identifying different series.
+            future_regressor (numpy.Array): single external regressor matching train.index
+            weights (dict): {'colname1': 2, 'colname2': 5} - increase importance of a series in metric evaluation. Any left blank assumed to have weight of 1.
+                pass the alias 'mean' as a str ie `weights='mean'` to automatically use the mean value of a series as its weight
+                available aliases: mean, median, min, max
+            result_file (str): results saved on each new generation. Does not include validation rounds.
+                ".csv" save model results table.
+                ".pickle" saves full object, including ensemble information.
+            grouping_ids (dict): currently a one-level dict containing series_id:group_id mapping.
+                used in 0.2.x but not 0.3.x+ versions. retained for potential future use
+        """
+        self.model = None
+        self.grouping_ids = grouping_ids
+
+        # convert class variables to local variables (makes testing easier)
+        if self.validation_method == "custom":
+            self.validation_indexes = validation_indexes
+            assert (
+                validation_indexes is not None
+            ), "validation_indexes needs to be filled with 'custom' validation"
+            # if auto num_validation, use as many as provided in custom
+            if self.num_validations in ["auto", 'max']:
+                self.num_validations == len(validation_indexes) - 1
+            else:
+                assert len(validation_indexes) >= (
+                    self.num_validations + 1
+                ), "validation_indexes needs to be >= num_validations + 1 with 'custom' validation"
+        else:
+            self.validation_indexes = []
+
+        prediction_interval = self.prediction_interval
+        random_seed = self.random_seed
+        metric_weighting = self.metric_weighting
+        verbose = self.verbose
+        template_cols = self.template_cols
+
+        # shut off warnings if running silently
+        if verbose <= 0:
+            import warnings
+
+            warnings.filterwarnings("ignore")
+
+        # clean up result_file input, if given.
+        if result_file is not None:
+            formats = ['.csv', '.pickle']
+            if not any(x in result_file for x in formats):
+                print("result_file must be a valid str with .csv or .pickle")
+                result_file = None
+
+        # set random seeds for environment
+        random_seed = abs(int(random_seed))
+        random.seed(random_seed)
+        np.random.seed(random_seed)
+
+        self.fit_data(
+            df=df,
+            date_col=date_col,
+            value_col=value_col,
+            id_col=id_col,
+            future_regressor=future_regressor,
+            weights=weights,
+        )
+
+        ensemble = self.ensemble
+
         # record if subset or not
         if self.subset is not None:
             self.subset = abs(int(self.subset))
             if self.subset >= self.df_wide_numeric.shape[1]:
                 self.subset_flag = False
             else:
                 self.subset_flag = True
         else:
             self.subset_flag = False
 
         #
         # take a subset of the data if working with a large number of series
         if self.subset_flag:
             df_subset = subset_series(
-                df_wide_numeric,
-                list((self.weights.get(i)) for i in df_wide_numeric.columns),
+                self.df_wide_numeric,
+                list((self.weights.get(i)) for i in self.df_wide_numeric.columns),
                 n=self.subset,
                 random_state=random_seed,
             )
             if self.verbose > 1:
                 print(f'First subset is of: {df_subset.columns}')
         else:
-            df_subset = df_wide_numeric.copy()
+            df_subset = self.df_wide_numeric.copy()
         # go to first index
         first_idx = self.validation_indexes[0]
         if max(first_idx) > max(df_subset.index):
             raise ValueError("provided validation index exceeds historical data period")
         df_subset = df_subset.reindex(first_idx)
 
         # subset the weighting information as well
@@ -1019,45 +1164,30 @@
             current_weights = {x: 1 for x in df_subset.columns}
         else:
             current_weights = {x: self.weights[x] for x in df_subset.columns}
 
         # split train and test portions, and split regressor if present
         df_train, df_test = simple_train_test_split(
             df_subset,
-            forecast_length=forecast_length,
+            forecast_length=self.forecast_length,
             min_allowed_train_percent=self.min_allowed_train_percent,
             verbose=self.verbose,
         )
         self.validation_train_indexes.append(df_train.index)
         self.validation_test_indexes.append(df_test.index)
         if future_regressor is not None:
-            if not isinstance(future_regressor, pd.DataFrame):
-                future_regressor = pd.DataFrame(future_regressor)
-            if future_regressor.empty:
-                raise ValueError(
-                    "future_regressor empty, pass None if intending not to use"
-                )
-            if not isinstance(future_regressor.index, pd.DatetimeIndex):
-                # should be same length as history as this is not yet the predict step
-                future_regressor.index = df_subset.index
-            # handle any non-numeric data, crudely
-            self.regr_num_trans = NumericTransformer(verbose=self.verbose)
-            future_regressor = self.regr_num_trans.fit_transform(future_regressor)
-            self.future_regressor_train = future_regressor
-            future_regressor_train = future_regressor.reindex(index=df_train.index)
-            future_regressor_test = future_regressor.reindex(index=df_test.index)
+            future_regressor_train = self.future_regressor_train.reindex(
+                index=df_train.index
+            )
+            future_regressor_test = self.future_regressor_train.reindex(
+                index=df_test.index
+            )
         else:
             future_regressor_train = None
             future_regressor_test = None
-        if future_regressor is not None:
-            if future_regressor.shape[0] != df_wide_numeric.shape[0]:
-                print(
-                    "future_regressor row count does not match length of training data"
-                )
-                time.sleep(2)
 
         self.start_time = pd.Timestamp.now()
 
         # unpack ensemble models so sub models appear at highest level
         self.initial_template = unpack_ensemble_models(
             self.initial_template,
             self.template_cols,
@@ -1160,15 +1290,15 @@
         if self.ensemble:
             try:
                 self.score_per_series = generate_score_per_series(
                     self.initial_results, self.metric_weighting, 1
                 )
                 ensemble_templates = EnsembleTemplateGenerator(
                     self.initial_results,
-                    forecast_length=forecast_length,
+                    forecast_length=self.forecast_length,
                     ensemble=ensemble,
                     score_per_series=self.score_per_series,
                 )
                 self._run_template(
                     ensemble_templates,
                     df_train,
                     df_test,
@@ -1254,18 +1384,18 @@
                 subset=['Model', 'ModelParameters', 'TransformationParameters']
             )
         self.validation_template = validation_template[self.template_cols]
 
         # run validations
         if self.num_validations > 0:
             self._run_validations(
-                df_wide_numeric=df_wide_numeric,
+                df_wide_numeric=self.df_wide_numeric,
                 num_validations=self.num_validations,
                 validation_template=self.validation_template,
-                future_regressor=future_regressor,
+                future_regressor=self.future_regressor_train,
             )
             # ensembles built on validation results
             if self.ensemble:
                 try:
                     ens_copy = copy.copy(self.validation_results)
                     run_count = (
                         self.initial_results.model_results[
@@ -1284,15 +1414,15 @@
                     self.score_per_series = generate_score_per_series(
                         self.initial_results,
                         self.metric_weighting,
                         total_validations=(self.num_validations + 1),
                     )
                     ensemble_templates = EnsembleTemplateGenerator(
                         ens_copy,
-                        forecast_length=forecast_length,
+                        forecast_length=self.forecast_length,
                         ensemble=ensemble,
                         score_per_series=self.score_per_series,
                     )
                     self.ensemble_templates2 = ensemble_templates
                     self._run_template(
                         ensemble_templates,
                         df_train,
@@ -1302,18 +1432,18 @@
                         current_weights=current_weights,
                         validation_round=0,
                         max_generations="Ensembles",
                         current_generation=(current_generation + 2),
                         result_file=result_file,
                     )
                     self._run_validations(
-                        df_wide_numeric=df_wide_numeric,
+                        df_wide_numeric=self.df_wide_numeric,
                         num_validations=self.num_validations,
                         validation_template=ensemble_templates,
-                        future_regressor=future_regressor,
+                        future_regressor=self.future_regressor_train,
                         first_validation=False,
                     )
                 except Exception as e:
                     print(
                         f"Post-Validation Ensembling Error: {repr(e)}: {''.join(tb.format_exception(None, e, e.__traceback__))}"
                     )
                     time.sleep(5)
@@ -1337,15 +1467,15 @@
                     self.initial_results,
                     metric_weighting=metric_weighting,
                     total_validations=(self.num_validations + 1),
                 )
                 ens_templates = HorizontalTemplateGenerator(
                     self.score_per_series,
                     model_results=self.initial_results.model_results,
-                    forecast_length=forecast_length,
+                    forecast_length=self.forecast_length,
                     ensemble=ensemble,
                     subset_flag=self.subset_flag,
                 )
                 ensemble_templates = pd.concat(
                     [ensemble_templates, ens_templates], axis=0
                 )
                 models_to_use = horizontal_template_to_model_list(ens_templates)
@@ -1600,14 +1730,24 @@
             # use the best of these ensembles if any ran successfully
             # horizontal ensembles are only run on one eval, if that eval is harder it won't compare to full validation results
             # however they are chosen based off of validation results of all validation runs
             eligible_models = self.validation_results.model_results[
                 self.validation_results.model_results['Runs']
                 >= (self.num_validations + 1)
             ]
+            if eligible_models.empty:
+                # this may occur if there is enough data for full validations
+                # but a lot of that data is bad leading to complete validation round failures
+                print(
+                    "your validation results are questionable, perhaps bad data and too many validations"
+                )
+                max_vals = self.validation_results.model_results['Runs'].max()
+                eligible_models = self.validation_results.model_results[
+                    self.validation_results.model_results['Runs'] >= max_vals
+                ]
             try:
                 self.best_model_non_horizontal = (
                     eligible_models.sort_values(
                         by="Score", ascending=True, na_position='last'
                     )
                     .drop_duplicates(subset=self.template_cols)
                     .head(1)[self.template_cols_id]
@@ -1637,42 +1777,60 @@
 
         else:
             # choose best model, when no horizontal ensembling is done
             eligible_models = self.validation_results.model_results[
                 self.validation_results.model_results['Runs']
                 >= (self.num_validations + 1)
             ]
+            if eligible_models.empty:
+                # this may occur if there is enough data for full validations
+                # but a lot of that data is bad leading to complete validation round failures
+                print(
+                    "your validation results are questionable, perhaps bad data and too many validations"
+                )
+                max_vals = self.validation_results.model_results['Runs'].max()
+                eligible_models = self.validation_results.model_results[
+                    self.validation_results.model_results['Runs'] >= max_vals
+                ]
             try:
                 self.best_model = (
                     eligible_models.sort_values(
                         by="Score", ascending=True, na_position='last'
                     )
                     .drop_duplicates(subset=self.template_cols)
                     .head(1)[self.template_cols_id]
                 )
             except IndexError:
                 raise ValueError(error_msg_template)
         # give a more convenient dict option
+        self.parse_best_model()
+
+        # clean up any remaining print statements
+        sys.stdout.flush()
+        return self
+
+    def parse_best_model(self):
+        if self.best_model.empty:
+            raise ValueError(
+                "no best model present. Run .fit() of the AutoTS class first."
+            )
         self.best_model_name = self.best_model['Model'].iloc[0]
         self.best_model_id = self.best_model['ID'].iloc[0]
         self.best_model_params = json.loads(self.best_model['ModelParameters'].iloc[0])
         self.best_model_transformation_params = json.loads(
             self.best_model['TransformationParameters'].iloc[0]
         )
         self.best_model_ensemble = self.best_model['Ensemble'].iloc[0]
+        # flag if is any type of ensemble
         self.ensemble_check = int(self.best_model_ensemble > 0)
-
         # set flags to check if regressors or ensemble used in final model.
         self.used_regressor_check = self._regr_param_check(
             self.best_model_params.copy()
         )
         self.regressor_used = self.used_regressor_check
-        # clean up any remaining print statements
-        sys.stdout.flush()
-        return self
 
     def _regr_param_check(self, param_dict):
         """Help to search for if a regressor was used in model."""
         out = False
         # load string if not dictionary
         if isinstance(param_dict, dict):
             cur_dict = param_dict.copy()
@@ -1868,53 +2026,90 @@
         fail_on_forecast_nan: bool = True,
         verbose: int = 'self',
         model_name=None,
         model_params=None,
         model_transformation_params=None,
         df_wide_numeric=None,
         future_regressor_train=None,
+        refit=False,
     ):
-        df_forecast = model_forecast(
-            model_name=self.best_model_name if model_name is None else model_name,
-            model_param_dict=self.best_model_params.copy()
-            if model_params is None
-            else model_params,
-            model_transform_dict=self.best_model_transformation_params
+        use_model = self.best_model_name if model_name is None else model_name
+        use_params = (
+            self.best_model_params.copy() if model_params is None else model_params
+        )
+        use_trans = (
+            self.best_model_transformation_params
             if model_transformation_params is None
-            else model_transformation_params,
-            df_train=self.df_wide_numeric
-            if df_wide_numeric is None
-            else df_wide_numeric,
-            forecast_length=forecast_length,
-            frequency=self.frequency,
-            prediction_interval=prediction_interval,
-            no_negatives=self.no_negatives,
-            constraint=self.constraint,
-            future_regressor_train=self.future_regressor_train
+            else model_transformation_params
+        )
+        use_data = self.df_wide_numeric if df_wide_numeric is None else df_wide_numeric
+        use_regr_train = (
+            self.future_regressor_train
             if future_regressor_train is None
-            else future_regressor_train,
-            future_regressor_forecast=future_regressor,
-            holiday_country=self.holiday_country,
-            startTimeStamps=self.startTimeStamps,
-            grouping_ids=self.grouping_ids,
-            fail_on_forecast_nan=fail_on_forecast_nan,
-            random_seed=self.random_seed,
-            verbose=verbose,
-            n_jobs=self.n_jobs,
-            template_cols=self.template_cols,
-            current_model_file=self.current_model_file,
-            return_model=True,
+            else future_regressor_train
         )
+        if use_model in update_fit:
+            if self.model is None or refit:
+                self.model = ModelPrediction(
+                    transformation_dict=use_trans,
+                    model_str=use_model,
+                    parameter_dict=use_params,
+                    forecast_length=forecast_length,
+                    frequency=self.frequency,
+                    prediction_interval=prediction_interval,
+                    no_negatives=self.no_negatives,
+                    constraint=self.constraint,
+                    holiday_country=self.holiday_country,
+                    startTimeStamps=self.startTimeStamps,
+                    grouping_ids=self.grouping_ids,
+                    fail_on_forecast_nan=fail_on_forecast_nan,
+                    random_seed=self.random_seed,
+                    verbose=verbose,
+                    n_jobs=self.n_jobs,
+                    current_model_file=self.current_model_file,
+                    return_model=True,
+                )
+                self.model = self.model.fit(use_data, future_regressor=use_regr_train)
+            else:
+                self.model.fit_data(use_data, future_regressor=use_regr_train)
+            df_forecast = self.model.predict(
+                forecast_length, future_regressor=future_regressor
+            )
+        else:
+            df_forecast = model_forecast(
+                model_name=use_model,
+                model_param_dict=use_params,
+                model_transform_dict=use_trans,
+                df_train=use_data,
+                forecast_length=forecast_length,
+                frequency=self.frequency,
+                prediction_interval=prediction_interval,
+                no_negatives=self.no_negatives,
+                constraint=self.constraint,
+                future_regressor_train=use_regr_train,
+                future_regressor_forecast=future_regressor,
+                holiday_country=self.holiday_country,
+                startTimeStamps=self.startTimeStamps,
+                grouping_ids=self.grouping_ids,
+                fail_on_forecast_nan=fail_on_forecast_nan,
+                random_seed=self.random_seed,
+                verbose=verbose,
+                n_jobs=self.n_jobs,
+                template_cols=self.template_cols,
+                current_model_file=self.current_model_file,
+                return_model=True,
+            )
         # convert categorical back to numeric
         trans = self.categorical_transformer
         df_forecast.forecast = trans.inverse_transform(df_forecast.forecast)
         df_forecast.lower_forecast = trans.inverse_transform(df_forecast.lower_forecast)
         df_forecast.upper_forecast = trans.inverse_transform(df_forecast.upper_forecast)
         # undo preclean transformations if necessary
         if self.preclean is not None:
+            # self.raw_forecast = copy.copy(df_forecast)
             df_forecast.forecast = self.preclean_transformer.inverse_transform(
                 df_forecast.forecast
             )
             df_forecast.lower_forecast = self.preclean_transformer.inverse_transform(
                 df_forecast.lower_forecast
             )
             df_forecast.upper_forecast = self.preclean_transformer.inverse_transform(
@@ -1931,14 +2126,29 @@
         hierarchy=None,
         just_point_forecast: bool = False,
         fail_on_forecast_nan: bool = True,
         verbose: int = 'self',
     ):
         """Generate forecast data immediately following dates of index supplied to .fit().
 
+        If using a model from update_fit list, with no ensembling, underlying model will not be retrained when used as below, with a single prediction interval:
+        This designed for high speed forecasting. Full retraining is best when there is sufficient time.
+        ```python
+        model = AutoTS(model_list='update_fit')
+        model.fit(df)
+        model.predict()
+        # for new data without retraining
+        model.fit_data(df)
+        model.predict()
+        # to force retrain of best model (but not full model search)
+        model.model = None
+        model.fit_data(df)
+        model.predict()
+        ```
+
         Args:
             forecast_length (int): Number of periods of data to forecast ahead
             prediction_interval (float): interval of upper/lower forecasts.
                 defaults to 'self' ie the interval specified in __init__()
                 if prediction_interval is a list, then returns a dict of forecast objects.
                     {str(interval): prediction_object}
             future_regressor (numpy.Array): additional regressor
@@ -1977,14 +2187,15 @@
             for interval in prediction_interval:
                 df_forecast = self._predict(
                     forecast_length=forecast_length,
                     prediction_interval=prediction_interval,
                     future_regressor=future_regressor,
                     fail_on_forecast_nan=fail_on_forecast_nan,
                     verbose=verbose,
+                    refit=True,  # need to audit all models to make sure they don't require update train with new prediction_interval
                 )
                 forecast_objects[str(interval)] = df_forecast
             return forecast_objects
         else:
             df_forecast = self._predict(
                 forecast_length=forecast_length,
                 prediction_interval=prediction_interval,
@@ -2047,14 +2258,15 @@
             export_template = export_template.drop_duplicates()
         elif models == 'best':
             # skip to the answer if just n==1
             if n == 1 and not include_results:
                 export_template = self.best_model
             else:
                 export_template = self.validation_results.model_results
+                # all validated models + horizontal ensembles
                 export_template = export_template[
                     (export_template['Runs'] >= (self.num_validations + 1))
                     | (export_template['Ensemble'] >= 2)
                 ]
                 """
                 if any(x in self.ensemble for x in self.h_ens_list):
                     temp = self.initial_results.model_results
@@ -2089,27 +2301,78 @@
                             export_template,
                         ]
                     ).drop_duplicates()
                 if not include_results:
                     export_template = export_template[self.template_cols_id]
         else:
             raise ValueError("`models` must be 'all' or 'best'")
+        return self.save_template(filename, export_template)
+
+    def save_template(self, filename, export_template, **kwargs):
+        """Helper function for the save part of export_template."""
         try:
             if filename is None:
                 return export_template
             elif '.csv' in filename:
-                return export_template.to_csv(filename, index=False)
+                return export_template.to_csv(
+                    filename, index=False, **kwargs
+                )  # lineterminator='\r\n'
             elif '.json' in filename:
-                return export_template.to_json(filename, orient='columns')
+                return export_template.to_json(filename, orient='columns', **kwargs)
             else:
                 raise ValueError("file must be .csv or .json")
-        except PermissionError:
+        except PermissionError as e:
             raise PermissionError(
                 "Permission Error: directory or existing file is locked for editing."
+            ) from e
+
+    def load_template(self, filename):
+        """Helper funciton for just loading the file part of import_template."""
+        if isinstance(filename, pd.DataFrame):
+            import_template = filename.copy()
+        elif '.csv' in filename:
+            import_template = pd.read_csv(filename)
+        elif '.json' in filename:
+            import_template = pd.read_json(filename, orient='columns')
+        else:
+            raise ValueError("file must be .csv or .json")
+
+        try:
+            import_template = import_template[self.template_cols_id]
+        except Exception:
+            print(
+                "Column names {} were not recognized as matching template columns: {}".format(
+                    str(import_template.columns), str(self.template_cols_id)
+                )
             )
+        return import_template
+
+    def _enforce_model_list(
+        self, template, model_list=None, include_ensemble=False, addon_flag=False
+    ):
+        """remove models not in given model list."""
+        if model_list is None:
+            model_list = self.model_list
+        if include_ensemble:
+            mod_list = model_list + ['Ensemble']
+        else:
+            mod_list = model_list
+        present = template['Model'].unique().tolist()
+        template = template[template['Model'].isin(mod_list)]
+        # double method of removing Ensemble
+        if not include_ensemble and "Ensemble" in template.columns:
+            template = template[template["Ensemble"] == 0]
+        if template.shape[0] == 0:
+            error_msg = f"Len 0. Model_list {model_list} does not match models in imported template {present}, template import failed."
+            if addon_flag:
+                # if template is addon, then this is fine as just a warning
+                print(error_msg)
+            else:
+                raise ValueError(error_msg)
+        return template
 
     def import_template(
         self,
         filename: str,
         method: str = "add_on",
         enforce_model_list: bool = True,
         include_ensemble: bool = False,
@@ -2124,53 +2387,27 @@
             include_ensemble (bool): if enforce_model_list is True, this specifies whether to allow ensembles anyway (otherwise they are unpacked and parts kept)
         """
         if method.lower() in ['add on', 'addon', 'add_on']:
             addon_flag = True
         else:
             addon_flag = False
 
-        if isinstance(filename, pd.DataFrame):
-            import_template = filename.copy()
-        elif '.csv' in filename:
-            import_template = pd.read_csv(filename)
-        elif '.json' in filename:
-            import_template = pd.read_json(filename, orient='columns')
-        else:
-            raise ValueError("file must be .csv or .json")
-
-        try:
-            import_template = import_template[self.template_cols]
-        except Exception:
-            print(
-                "Column names {} were not recognized as matching template columns: {}".format(
-                    str(import_template.columns), str(self.template_cols)
-                )
-            )
+        import_template = self.load_template(filename)
 
         import_template = unpack_ensemble_models(
             import_template, self.template_cols, keep_ensemble=True, recursive=True
         )
 
         if enforce_model_list:
-            # remove models not in given model list
-            if include_ensemble:
-                mod_list = self.model_list + ['Ensemble']
-            else:
-                mod_list = self.model_list
-            import_template = import_template[import_template['Model'].isin(mod_list)]
-            # double method of removing Ensemble
-            if not include_ensemble and "Ensemble" in import_template.columns:
-                import_template = import_template[import_template["Ensemble"] == 0]
-            if import_template.shape[0] == 0:
-                error_msg = "Len 0. Model_list does not match models in imported template, template import failed."
-                if addon_flag:
-                    # if template is addon, then this is fine as just a warning
-                    print(error_msg)
-                else:
-                    raise ValueError(error_msg)
+            import_template = self._enforce_model_list(
+                template=import_template,
+                model_list=None,
+                include_ensemble=include_ensemble,
+                addon_flag=addon_flag,
+            )
 
         if addon_flag:
             self.initial_template = self.initial_template.merge(
                 import_template,
                 how='outer',
                 on=self.initial_template.columns.intersection(
                     import_template.columns
@@ -2182,14 +2419,50 @@
         elif method.lower() in ['only', 'user only', 'user_only', 'import_only']:
             self.initial_template = import_template
         else:
             return ValueError("method must be 'addon' or 'only'")
 
         return self
 
+    def export_best_model(self, filename, **kwargs):
+        """Basically the same as export_template but only ever the one best model."""
+        return self.save_template(filename, self.best_model.copy(), **kwargs)
+
+    def import_best_model(
+        self,
+        import_target,
+        enforce_model_list: bool = True,
+        include_ensemble: bool = True,
+    ):
+        """Load a best model, overriding any existing setting.
+
+        Args:
+            import_target: pd.DataFrame or file path
+        """
+        if isinstance(import_target, pd.DataFrame):
+            template = import_target.copy()
+        else:
+            template = self.load_template(import_target)
+        if not include_ensemble:
+            template = unpack_ensemble_models(
+                template, self.template_cols, keep_ensemble=False, recursive=True
+            )
+        if enforce_model_list:
+            template = self._enforce_model_list(
+                template=template,
+                model_list=None,
+                include_ensemble=include_ensemble,
+                addon_flag=False,
+            )
+
+        self.best_model = template.iloc[0:1]
+
+        self.parse_best_model()
+        return self
+
     def import_results(self, filename):
         """Add results from another run on the same data.
 
         Input can be filename with .csv or .pickle.
         or can be a DataFrame of model results or a full TemplateEvalObject
         """
         csv_flag = False
@@ -2390,17 +2663,23 @@
         series = ModelParameters['series']
         series = pd.DataFrame.from_dict(series, orient="index").reset_index(drop=False)
         if series.shape[1] > 2:
             # for mosaic style ensembles, choose the mode model id
             series.set_index(series.columns[0], inplace=True)
             series = series.mode(axis=1)[0].to_frame().reset_index(drop=False)
         series.columns = ['Series', 'ID']
-        series = series.merge(
-            self.results()[['ID', "Model"]].drop_duplicates(), on="ID"
+        results = pd.Series(
+            {
+                x: self.best_model_params['models'][x]['Model']
+                for x in self.best_model_params['models'].keys()
+            }
         )
+        results.name = "Model"
+        series = series.merge(results, left_on="ID", right_index=True)
+        # series = series.merge(self.results()[['ID', "Model"]].drop_duplicates(), on="ID")  # old
         series = series.merge(
             self.df_wide_numeric.std().to_frame(), right_index=True, left_on="Series"
         )
         series = series.merge(
             self.df_wide_numeric.mean().to_frame(), right_index=True, left_on="Series"
         )
         series.columns = ["Series", "ID", 'Model', "Volatility", "Mean"]
@@ -2583,14 +2862,15 @@
             plot_df.plot(title=title, **kwargs)
 
     def plot_back_forecast(self, **kwargs):
         return self.plot_backforecast(**kwargs)
 
     def plot_validations(
         self,
+        df_wide=None,
         models=None,
         series=None,
         title=None,
         start_date="auto",
         end_date=None,
         subset=None,
         compare_horizontal=False,
@@ -2609,29 +2889,36 @@
             title (str): graph title
             start_date (str): or datetime, place to begin graph, None for full
             end_date (str): or datetime, end of graph x axis
             subset (str): overrides series, shows either 'best' or 'worst'
             compare_horizontal (bool): if True, plot horizontal ensemble versus best non-horizontal model, when available
             include_bounds (bool): if True (default) include the upper/lower forecast bounds
         """
+        if df_wide is None:
+            df_wide = self.df_wide_numeric
         if series is None:
-            if str(subset).lower() == "best":
-                series = self.best_model_per_series_mape().tail(1).index.tolist()[0]
-            elif str(subset).lower() == "best score":
-                series = self.best_model_per_series_score().tail(1).index.tolist()[0]
-            elif str(subset).lower() == "worst":
-                series = self.best_model_per_series_mape().head(1).index.tolist()[0]
-            elif str(subset).lower() == "worst score":
-                series = self.best_model_per_series_score().head(1).index.tolist()[0]
-            elif subset is None:
-                series = random.choice(self.df_wide_numeric.columns)
+            if subset is None:
+                series = random.choice(df_wide.columns)
             else:
-                raise ValueError(
-                    "plot_validations arg subset must be None, 'best' or 'worst'"
-                )
+                scores = self.best_model_per_series_mape().index.tolist()
+                scores = [x for x in scores if "_lltmicro" not in x]
+                mapes = self.best_model_per_series_score().index.tolist()
+                mapes = [x for x in mapes if "_lltmicro" not in x]
+                if str(subset).lower() == "best":
+                    series = mapes[-1]
+                elif str(subset).lower() == "best score":
+                    series = scores[-1]
+                elif str(subset).lower() == "worst":
+                    series = mapes[0]
+                elif str(subset).lower() == "worst score":
+                    series = scores[0]
+                else:
+                    raise ValueError(
+                        "plot_validations arg subset must be None, 'best' or 'worst'"
+                    )
         if title is None:
             if subset is not None:
                 if "score" in str(subset).lower():
                     title = f"Validation Forecasts for {subset} Tested Series {series}"
                 else:
                     title = (
                         f"Validation Forecasts for {subset} Tested MAPE Series {series}"
@@ -2665,31 +2952,40 @@
         duplicated = False
         if self.validation_forecasts_template is not None:
             if self.validation_forecasts_template.equals(validation_template):
                 duplicated = True
         if not duplicated:
             self.validation_forecast_cuts = []
             # self.validation_forecasts = {}
-            for val in range(len(self.validation_train_indexes)):
-                test_idx = self.validation_train_indexes[val]
-                train_reg = self.future_regressor_train.reindex(test_idx)
-                sec_idx = self.validation_test_indexes[val]
+            for val in range(len(self.validation_indexes)):
+                val_df_train, val_df_test = simple_train_test_split(
+                    self.df_wide_numeric,
+                    forecast_length=self.forecast_length,
+                    min_allowed_train_percent=self.min_allowed_train_percent,
+                    verbose=self.verbose,
+                )
+                sec_idx = val_df_test.index
                 self.validation_forecast_cuts.append(sec_idx[0])
-                fut_reg = self.future_regressor_train.reindex(sec_idx)
+                try:
+                    train_reg = self.future_regressor_train.reindex(val_df_train.index)
+                    fut_reg = self.future_regressor_train.reindex(sec_idx)
+                except Exception:
+                    train_reg = None
+                    fut_reg = None
                 for index, row in validation_template.iterrows():
                     df_forecast = self._predict(
                         forecast_length=self.forecast_length,
                         prediction_interval=self.prediction_interval,
                         future_regressor=fut_reg,
                         fail_on_forecast_nan=False,
                         verbose=self.verbose,
                         model_name=row["Model"],
                         model_params=row["ModelParameters"],
                         model_transformation_params=row["TransformationParameters"],
-                        df_wide_numeric=self.df_wide_numeric.reindex(test_idx),
+                        df_wide_numeric=val_df_train,
                         future_regressor_train=train_reg,
                     )
                     idz = create_model_id(
                         row["Model"],
                         row["ModelParameters"],
                         row["TransformationParameters"],
                     )
@@ -2701,27 +2997,27 @@
                 print("using stored results for plot_validations")
         self.validation_forecasts_template = validation_template
         needed_mods = self.validation_forecasts_template['ID'].tolist()
         df_list = []
         for x in self.validation_forecasts.keys():
             mname = x.split("_")[1]
             if mname == "chosen" or mname in needed_mods:
-                new_df = pd.DataFrame(index=self.df_wide_numeric.index)
+                new_df = pd.DataFrame(index=df_wide.index)
                 new_df[mname] = self.validation_forecasts[x].forecast[series]
                 new_df[mname + "_" + "upper"] = self.validation_forecasts[
                     x
                 ].upper_forecast[series]
                 new_df[mname + "_" + "lower"] = self.validation_forecasts[
                     x
                 ].lower_forecast[series]
                 df_list.append(new_df)
         plot_df = pd.concat(df_list, sort=True, axis=0)
         plot_df = plot_df.groupby(level=0).last()
         plot_df = (
-            self.df_wide_numeric[series]
+            df_wide[series]
             .rename("actuals")
             .to_frame()
             .merge(plot_df, left_index=True, right_index=True, how="left")
         )
         if not include_bounds:
             colb = [
                 x for x in plot_df.columns if "_lower" not in x and "_upper" not in x
@@ -2840,14 +3136,36 @@
                 kind=kind,
                 title=title,
                 color=color,
                 figsize=figsize,
                 **kwargs,
             )
 
+    def plot_per_series_smape(
+        self,
+        title: str = None,
+        max_series: int = 10,
+        max_name_chars: int = 25,
+        color: str = "#ff9912",
+        figsize=(12, 4),
+        kind: str = "bar",
+        **kwargs,
+    ):
+        """To be backwards compatible, not necessarily maintained, plot_per_series_mape is to be preferred."""
+        print("please switch to plot_per_series_mape")
+        return self.plot_per_series_mape(
+            title=title,
+            max_series=max_series,
+            max_name_chars=max_name_chars,
+            color=color,
+            figsize=figsize,
+            kind=kind,
+            **kwargs,
+        )
+
     def best_model_per_series_score(self):
         return (
             generate_score_per_series(
                 self.initial_results,
                 metric_weighting=self.metric_weighting,
                 total_validations=(self.num_validations + 1),
                 models_to_use=[self.best_model_id],
```

### Comparing `autots-0.5.8/autots/evaluator/benchmark.py` & `autots-0.6.0/autots/evaluator/benchmark.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/evaluator/event_forecasting.py` & `autots-0.6.0/autots/evaluator/event_forecasting.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/evaluator/metrics.py` & `autots-0.6.0/autots/evaluator/metrics.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/evaluator/validation.py` & `autots-0.6.0/autots/evaluator/validation.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/models/arch.py` & `autots-0.6.0/autots/models/arch.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/models/base.py` & `autots-0.6.0/autots/models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,20 @@
         """Return dict of current parameters."""
         return {}
 
     def get_new_params(self, method: str = 'random'):
         """Return dict of new parameters for parameter tuning."""
         return {}
 
+    def fit_data(self, df, future_regressor=None):
+        self.basic_profile(df)
+        if future_regressor is not None:
+            self.regressor_train = future_regressor
+        return self
+
     @staticmethod
     def time():
         return datetime.datetime.now()
 
 
 def apply_constraints(
     forecast,
@@ -259,15 +265,15 @@
         per_timestamp=np.nan,
         avg_metrics=np.nan,
         avg_metrics_weighted=np.nan,
         full_mae_error=None,
         model=None,
         transformer=None,
     ):
-        self.model_name = model_name
+        self.model_name = self.name = model_name
         self.model_parameters = model_parameters
         self.transformation_parameters = transformation_parameters
         self.forecast_length = forecast_length
         self.forecast_index = forecast_index
         self.forecast_columns = forecast_columns
         self.lower_forecast = lower_forecast
         self.forecast = forecast
@@ -436,15 +442,15 @@
             colors (dict): colors mapping dictionary col: color
             alpha (float): intensity of bound interval shading
             **kwargs passed to pd.DataFrame.plot()
         """
         if start_date == "auto":
             if df_wide is not None:
                 slx = -self.forecast_length * 3
-                if slx > df_wide.shape[0]:
+                if abs(slx) > df_wide.shape[0]:
                     slx = 0
                 start_date = df_wide.index[slx]
             else:
                 start_date = self.forecast.index[0]
         plot_df = self.plot_df(
             df_wide=df_wide,
             series=series,
```

### Comparing `autots-0.5.8/autots/models/basics.py` & `autots-0.6.0/autots/models/basics.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from math import ceil
 import warnings
 import random
 import datetime
 import numpy as np
 import pandas as pd
 from autots.models.base import ModelObject, PredictionObject
-from autots.tools.seasonal import seasonal_int, seasonal_window_match
+from autots.tools.seasonal import (
+    seasonal_int,
+    seasonal_window_match,
+    seasonal_independent_match,
+)
 from autots.tools.probabilistic import Point_to_Probability, historic_quantile
 from autots.tools.window_functions import window_id_maker, sliding_window_view
 from autots.tools.percentile import nan_quantile
 from autots.tools.fast_kalman import KalmanFilter, random_state_space
 from autots.tools.transform import GeneralTransformer, RandomTransform, filters
 
 
@@ -2478,34 +2482,42 @@
         if k > min_k:
             n_tail = min(window_size, forecast_length)
         else:
             n_tail = forecast_length
         # finding sliding windows to compare
         temp = sliding_window_view(array[:-n_tail, :], window_size, axis=0)
         # compare windows by metrics
+        last_window = array[-window_size:, :]
         if distance_metric == "mae":
             if nan_flag:
-                scores = np.nanmean(np.abs(temp - array[-window_size:, :].T), axis=2)
+                scores = np.nanmean(np.abs(temp - last_window.T), axis=2)
             else:
-                scores = np.mean(np.abs(temp - array[-window_size:, :].T), axis=2)
+                scores = np.mean(np.abs(temp - last_window.T), axis=2)
+        elif distance_metric == "canberra":
+            divisor = np.abs(temp) + np.abs(last_window.T)
+            divisor[divisor == 0] = 1
+            if nan_flag:
+                scores = np.nanmean(np.abs(temp - last_window.T) / divisor, axis=2)
+            else:
+                scores = np.mean(np.abs(temp - last_window.T) / divisor, axis=2)
         elif distance_metric == "mqae":
             q = 0.85
-            ae = np.abs(temp - array[-window_size:, :].T)
+            ae = np.abs(temp - last_window.T)
             if ae.shape[2] <= 1:
                 vals = ae
             else:
                 qi = int(ae.shape[2] * q)
                 qi = qi if qi > 1 else 1
                 vals = np.partition(ae, qi, axis=2)[..., :qi]
             if nan_flag:
                 scores = np.nanmean(vals, axis=2)
             else:
                 scores = np.mean(vals, axis=2)
         elif distance_metric == "mse":
-            scores = np.nanmean((temp - array[-window_size:, :].T) ** 2, axis=2)
+            scores = np.nanmean((temp - last_window.T) ** 2, axis=2)
         else:
             raise ValueError(f"distance_metric: {distance_metric} not recognized")
 
         # select smallest windows
         min_idx = np.argpartition(scores, k - 1, axis=0)[:k]
         # take the period starting AFTER the window
         test = (
@@ -2598,14 +2610,15 @@
 
     def get_new_params(self, method: str = 'random'):
         """Returns dict of new parameters for parameter tuning"""
         metric_list = [
             'mae',
             'mqae',
             'mse',
+            "canberra",
         ]
         if method == "event_risk":
             k_choice = random.choices(
                 [10, 15, 20, 50, 100], [0.3, 0.1, 0.1, 0.05, 0.05]
             )[0]
         else:
             k_choice = random.choices(
@@ -2665,14 +2678,15 @@
         verbose: int = 0,
         regression_type: str = None,
         window: int = 5,
         point_method: str = "mean",
         distance_metric: str = "mae",
         k: int = 10,
         datepart_method: str = "common_fourier",
+        independent: bool = False,
         **kwargs,
     ):
         ModelObject.__init__(
             self,
             name,
             frequency,
             prediction_interval,
@@ -2683,14 +2697,15 @@
         )
         assert window >= 1, f"window {window} must be >= 1"
         self.window = int(window)
         self.point_method = point_method
         self.distance_metric = str(distance_metric).lower()
         self.k = k
         self.datepart_method = datepart_method
+        self.independent = independent
 
     def fit(self, df, future_regressor=None):
         """Train algorithm given data supplied.
 
         Args:
             df (pandas.DataFrame): Datetime Indexed
             regressor (numpy.Array): additional regressor
@@ -2718,22 +2733,33 @@
         test_index = self.create_forecast_index(forecast_length=forecast_length)
         window_size = self.window
         point_method = self.point_method
         distance_metric = self.distance_metric
         datepart_method = self.datepart_method
         k = self.k
 
-        test, scores = seasonal_window_match(
-            DTindex=self.df.index,
-            k=k,
-            window_size=window_size,
-            forecast_length=forecast_length,
-            datepart_method=datepart_method,
-            distance_metric=distance_metric,
-        )
+        if self.independent:
+            # each timestep is considered individually and not as a series
+            test, scores = seasonal_independent_match(
+                DTindex=self.df.index,
+                DTindex_future=test_index,
+                k=k,
+                datepart_method=datepart_method,
+                distance_metric=distance_metric,
+            )
+        else:
+            # original method and perhaps smoother
+            test, scores = seasonal_window_match(
+                DTindex=self.df.index,
+                k=k,
+                window_size=window_size,
+                forecast_length=forecast_length,
+                datepart_method=datepart_method,
+                distance_metric=distance_metric,
+            )
         # (num_windows, forecast_length, num_series)
         results = np.moveaxis(np.take(self.df.to_numpy(), test, axis=0), 1, 0)
 
         # now aggregate results into point and bound forecasts
         if point_method == "weighted_mean":
             weights = scores[test[0] - window_size].sum(axis=1)
             if weights.sum() == 0:
@@ -2782,14 +2808,15 @@
 
     def get_new_params(self, method: str = 'random'):
         """Returns dict of new parameters for parameter tuning"""
         metric_list = [
             'mae',
             'mqae',
             'mse',
+            'canberra',
         ]
         if method == "event_risk":
             k_choice = random.choices(
                 [10, 15, 20, 50, 100], [0.3, 0.1, 0.1, 0.05, 0.05]
             )[0]
         else:
             k_choice = random.choices(
@@ -2813,14 +2840,15 @@
                     "simple_binarized",
                     "expanded_binarized",
                     'common_fourier',
                     'common_fourier_rw',
                 ],
                 [0.4, 0.3, 0.3, 0.3, 0.4, 0.35, 0.45, 0.2],
             )[0],
+            "independent": bool(random.getrandbits(1)),
         }
 
     def get_params(self):
         """Return dict of current parameters"""
         return {
             "window": self.window,
             "point_method": self.point_method,
```

### Comparing `autots-0.5.8/autots/models/cassandra.py` & `autots-0.6.0/autots/models/cassandra.py`

 * *Files 2% similar despite different names*

```diff
@@ -3408,3867 +3408,4195 @@
 0000d4f0: 656c 662e 6669 745f 7275 6e74 696d 652c  elf.fit_runtime,
 0000d500: 0d0a 2020 2020 2020 2020 2020 2020 6d6f  ..            mo
 0000d510: 6465 6c5f 7061 7261 6d65 7465 7273 3d73  del_parameters=s
 0000d520: 656c 662e 6765 745f 7061 7261 6d73 2829  elf.get_params()
 0000d530: 2c0d 0a20 2020 2020 2020 2029 0d0a 2020  ,..        )..  
 0000d540: 2020 2020 2020 7265 7475 726e 2064 665f        return df_
 0000d550: 666f 7265 6361 7374 0d0a 0d0a 2020 2020  forecast....    
-0000d560: 6465 6620 7072 6564 6963 7428 0d0a 2020  def predict(..  
-0000d570: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
-0000d580: 2020 2020 2066 6f72 6563 6173 745f 6c65       forecast_le
-0000d590: 6e67 7468 2c0d 0a20 2020 2020 2020 2069  ngth,..        i
-0000d5a0: 6e63 6c75 6465 5f68 6973 746f 7279 3d46  nclude_history=F
-0000d5b0: 616c 7365 2c0d 0a20 2020 2020 2020 2066  alse,..        f
-0000d5c0: 7574 7572 655f 7265 6772 6573 736f 723d  uture_regressor=
-0000d5d0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2072  None,..        r
-0000d5e0: 6567 7265 7373 6f72 5f70 6572 5f73 6572  egressor_per_ser
-0000d5f0: 6965 733d 4e6f 6e65 2c0d 0a20 2020 2020  ies=None,..     
-0000d600: 2020 2066 6c61 675f 7265 6772 6573 736f     flag_regresso
-0000d610: 7273 3d4e 6f6e 652c 0d0a 2020 2020 2020  rs=None,..      
-0000d620: 2020 6675 7475 7265 5f69 6d70 6163 7473    future_impacts
-0000d630: 3d4e 6f6e 652c 0d0a 2020 2020 2020 2020  =None,..        
-0000d640: 6e65 775f 6466 3d4e 6f6e 652c 0d0a 2020  new_df=None,..  
-0000d650: 2020 2020 2020 7265 6772 6573 736f 725f        regressor_
-0000d660: 666f 7265 6361 7374 5f6d 6f64 656c 3d4e  forecast_model=N
-0000d670: 6f6e 652c 0d0a 2020 2020 2020 2020 7265  one,..        re
-0000d680: 6772 6573 736f 725f 666f 7265 6361 7374  gressor_forecast
-0000d690: 5f6d 6f64 656c 5f70 6172 616d 733d 4e6f  _model_params=No
-0000d6a0: 6e65 2c0d 0a20 2020 2020 2020 2072 6567  ne,..        reg
-0000d6b0: 7265 7373 6f72 5f66 6f72 6563 6173 745f  ressor_forecast_
-0000d6c0: 7472 616e 7366 6f72 6d61 7469 6f6e 733d  transformations=
-0000d6d0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2069  None,..        i
-0000d6e0: 6e63 6c75 6465 5f6f 7267 616e 6963 3d46  nclude_organic=F
-0000d6f0: 616c 7365 2c0d 0a20 2020 2029 3a0d 0a20  alse,..    ):.. 
-0000d700: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
-0000d710: 7465 2061 2066 6f72 6563 6173 742e 0d0a  te a forecast...
-0000d720: 0d0a 2020 2020 2020 2020 6675 7475 7265  ..        future
-0000d730: 5f72 6567 7265 7373 6f72 2061 6e64 2072  _regressor and r
-0000d740: 6567 7265 7373 6f72 5f70 6572 5f73 6572  egressor_per_ser
-0000d750: 6965 7320 7368 6f75 6c64 206f 6e6c 7920  ies should only 
-0000d760: 696e 636c 7564 6520 6e65 7720 6675 7475  include new futu
-0000d770: 7265 2076 616c 7565 732c 2068 6973 746f  re values, histo
-0000d780: 7279 2069 7320 616c 7265 6164 7920 7374  ry is already st
-0000d790: 6f72 6564 0d0a 2020 2020 2020 2020 7468  ored..        th
-0000d7a0: 6579 2073 686f 756c 6420 6d61 7463 6820  ey should match 
-0000d7b0: 6f6e 2066 6f72 6563 6173 745f 6c65 6e67  on forecast_leng
-0000d7c0: 7468 2061 6e64 2069 6e64 6578 206f 6620  th and index of 
-0000d7d0: 666f 7265 6361 7374 730d 0a20 2020 2020  forecasts..     
-0000d7e0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-0000d7f0: 7365 6c66 2e66 6f72 6563 6173 745f 6c65  self.forecast_le
-0000d800: 6e67 7468 203d 2066 6f72 6563 6173 745f  ngth = forecast_
-0000d810: 6c65 6e67 7468 0d0a 2020 2020 2020 2020  length..        
-0000d820: 7072 6564 6963 7453 7461 7274 5469 6d65  predictStartTime
-0000d830: 203d 2073 656c 662e 7469 6d65 2829 0d0a   = self.time()..
-0000d840: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d850: 7472 656e 645f 7472 6169 6e20 6973 204e  trend_train is N
-0000d860: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-0000d870: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000d880: 6f72 2822 4361 7373 616e 6472 6120 6d75  or("Cassandra mu
-0000d890: 7374 2066 6972 7374 2062 6520 2e66 6974  st first be .fit
-0000d8a0: 2829 2073 7563 6365 7373 6675 6c6c 792e  () successfully.
-0000d8b0: 2229 0d0a 0d0a 2020 2020 2020 2020 2320  ")....        # 
-0000d8c0: 7363 616c 6520 6e65 775f 6466 2069 6620  scale new_df if 
-0000d8d0: 6769 7665 6e0d 0a20 2020 2020 2020 2069  given..        i
-0000d8e0: 6620 6e65 775f 6466 2069 7320 6e6f 7420  f new_df is not 
-0000d8f0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000d900: 2020 2064 6620 3d20 7365 6c66 2e73 6361     df = self.sca
-0000d910: 6c65 5f64 6174 6128 6e65 775f 6466 290d  le_data(new_df).
-0000d920: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-0000d930: 2020 2020 2020 2020 2020 2020 6466 203d              df =
-0000d940: 2073 656c 662e 6466 2e63 6f70 7928 290d   self.df.copy().
-0000d950: 0a20 2020 2020 2020 2023 2069 6620 6675  .        # if fu
-0000d960: 7475 7265 2072 6567 7265 7373 6f72 7320  ture regressors 
-0000d970: 6172 6520 4e6f 6e65 2028 2620 5553 4544  are None (& USED
-0000d980: 292c 2062 7574 2077 6572 6520 7072 6f76  ), but were prov
-0000d990: 6964 6564 2066 6f72 2068 6973 746f 7279  ided for history
-0000d9a0: 2c20 696e 7374 6561 6420 7573 6520 666f  , instead use fo
-0000d9b0: 7265 6361 7374 7320 6f66 2074 6865 7365  recasts of these
-0000d9c0: 2066 6561 7475 7265 7320 2877 6172 6e29   features (warn)
-0000d9d0: 0d0a 2020 2020 2020 2020 6675 6c6c 5f72  ..        full_r
-0000d9e0: 6567 7220 3d20 4e6f 6e65 0d0a 2020 2020  egr = None..    
-0000d9f0: 2020 2020 6966 2028 0d0a 2020 2020 2020      if (..      
-0000da00: 2020 2020 2020 6675 7475 7265 5f72 6567        future_reg
-0000da10: 7265 7373 6f72 2069 7320 4e6f 6e65 0d0a  ressor is None..
-0000da20: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0000da30: 7365 6c66 2e66 7574 7572 655f 7265 6772  self.future_regr
-0000da40: 6573 736f 725f 7472 6169 6e20 6973 206e  essor_train is n
-0000da50: 6f74 204e 6f6e 650d 0a20 2020 2020 2020  ot None..       
-0000da60: 2020 2020 2061 6e64 2066 6f72 6563 6173       and forecas
-0000da70: 745f 6c65 6e67 7468 2069 7320 6e6f 7420  t_length is not 
-0000da80: 4e6f 6e65 0d0a 2020 2020 2020 2020 293a  None..        ):
-0000da90: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000daa0: 2073 656c 662e 7665 7262 6f73 6520 3e20   self.verbose > 
-0000dab0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-0000dac0: 2020 2020 7072 696e 7428 0d0a 2020 2020      print(..    
-0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dae0: 2266 7574 7572 655f 7265 6772 6573 736f  "future_regresso
-0000daf0: 7220 6e6f 7420 7072 6f76 6964 6564 2074  r not provided t
-0000db00: 6f20 4361 7373 616e 6472 612c 2075 7369  o Cassandra, usi
-0000db10: 6e67 2066 6f72 6563 6173 7473 206f 6620  ng forecasts of 
-0000db20: 6869 7374 6f72 6963 616c 220d 0a20 2020  historical"..   
-0000db30: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-0000db40: 2020 2020 2020 2020 2020 2020 6675 7475              futu
-0000db50: 7265 5f72 6567 7265 7373 6f72 203d 206d  re_regressor = m
-0000db60: 6f64 656c 5f66 6f72 6563 6173 7428 0d0a  odel_forecast(..
-0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db80: 6d6f 6465 6c5f 6e61 6d65 3d73 656c 662e  model_name=self.
-0000db90: 7472 656e 645f 6d6f 6465 6c5b 274d 6f64  trend_model['Mod
-0000dba0: 656c 275d 0d0a 2020 2020 2020 2020 2020  el']..          
-0000dbb0: 2020 2020 2020 6966 2072 6567 7265 7373        if regress
-0000dbc0: 6f72 5f66 6f72 6563 6173 745f 6d6f 6465  or_forecast_mode
-0000dbd0: 6c20 6973 204e 6f6e 650d 0a20 2020 2020  l is None..     
-0000dbe0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-0000dbf0: 7265 6772 6573 736f 725f 666f 7265 6361  regressor_foreca
-0000dc00: 7374 5f6d 6f64 656c 2c0d 0a20 2020 2020  st_model,..     
-0000dc10: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-0000dc20: 5f70 6172 616d 5f64 6963 743d 7365 6c66  _param_dict=self
-0000dc30: 2e74 7265 6e64 5f6d 6f64 656c 5b27 4d6f  .trend_model['Mo
-0000dc40: 6465 6c50 6172 616d 6574 6572 7327 5d0d  delParameters'].
-0000dc50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dc60: 2069 6620 7265 6772 6573 736f 725f 666f   if regressor_fo
-0000dc70: 7265 6361 7374 5f6d 6f64 656c 5f70 6172  recast_model_par
-0000dc80: 616d 7320 6973 204e 6f6e 650d 0a20 2020  ams is None..   
-0000dc90: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000dca0: 6520 7265 6772 6573 736f 725f 666f 7265  e regressor_fore
-0000dcb0: 6361 7374 5f6d 6f64 656c 5f70 6172 616d  cast_model_param
-0000dcc0: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-0000dcd0: 2020 2020 6d6f 6465 6c5f 7472 616e 7366      model_transf
-0000dce0: 6f72 6d5f 6469 6374 3d73 656c 662e 7072  orm_dict=self.pr
-0000dcf0: 6570 726f 6365 7373 696e 675f 7472 616e  eprocessing_tran
-0000dd00: 7366 6f72 6d61 7469 6f6e 0d0a 2020 2020  sformation..    
-0000dd10: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-0000dd20: 6567 7265 7373 6f72 5f66 6f72 6563 6173  egressor_forecas
-0000dd30: 745f 7472 616e 7366 6f72 6d61 7469 6f6e  t_transformation
-0000dd40: 7320 6973 204e 6f6e 650d 0a20 2020 2020  s is None..     
-0000dd50: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-0000dd60: 7265 6772 6573 736f 725f 666f 7265 6361  regressor_foreca
-0000dd70: 7374 5f74 7261 6e73 666f 726d 6174 696f  st_transformatio
-0000dd80: 6e73 2c0d 0a20 2020 2020 2020 2020 2020  ns,..           
-0000dd90: 2020 2020 2064 665f 7472 6169 6e3d 7365       df_train=se
-0000dda0: 6c66 2e66 7574 7572 655f 7265 6772 6573  lf.future_regres
-0000ddb0: 736f 725f 7472 6169 6e2c 0d0a 2020 2020  sor_train,..    
-0000ddc0: 2020 2020 2020 2020 2020 2020 666f 7265              fore
-0000ddd0: 6361 7374 5f6c 656e 6774 683d 666f 7265  cast_length=fore
-0000dde0: 6361 7374 5f6c 656e 6774 682c 0d0a 2020  cast_length,..  
-0000ddf0: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-0000de00: 6571 7565 6e63 793d 7365 6c66 2e66 7265  equency=self.fre
-0000de10: 7175 656e 6379 2c0d 0a20 2020 2020 2020  quency,..       
-0000de20: 2020 2020 2020 2020 2070 7265 6469 6374           predict
-0000de30: 696f 6e5f 696e 7465 7276 616c 3d73 656c  ion_interval=sel
-0000de40: 662e 7072 6564 6963 7469 6f6e 5f69 6e74  f.prediction_int
-0000de50: 6572 7661 6c2c 0d0a 2020 2020 2020 2020  erval,..        
-0000de60: 2020 2020 2020 2020 6661 696c 5f6f 6e5f          fail_on_
-0000de70: 666f 7265 6361 7374 5f6e 616e 3d46 616c  forecast_nan=Fal
-0000de80: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000de90: 2020 2020 2072 616e 646f 6d5f 7365 6564       random_seed
-0000dea0: 3d73 656c 662e 7261 6e64 6f6d 5f73 6565  =self.random_see
-0000deb0: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-0000dec0: 2020 2020 7665 7262 6f73 653d 7365 6c66      verbose=self
-0000ded0: 2e76 6572 626f 7365 2c0d 0a20 2020 2020  .verbose,..     
-0000dee0: 2020 2020 2020 2020 2020 206e 5f6a 6f62             n_job
-0000def0: 733d 7365 6c66 2e6e 5f6a 6f62 732c 0d0a  s=self.n_jobs,..
-0000df00: 2020 2020 2020 2020 2020 2020 292e 666f              ).fo
-0000df10: 7265 6361 7374 0d0a 2020 2020 2020 2020  recast..        
-0000df20: 2020 2020 6675 6c6c 5f72 6567 7220 3d20      full_regr = 
-0000df30: 7064 2e63 6f6e 6361 7428 5b73 656c 662e  pd.concat([self.
-0000df40: 6675 7475 7265 5f72 6567 7265 7373 6f72  future_regressor
-0000df50: 5f74 7261 696e 2c20 6675 7475 7265 5f72  _train, future_r
-0000df60: 6567 7265 7373 6f72 5d29 0d0a 2020 2020  egressor])..    
-0000df70: 2020 2020 6966 2066 6f72 6563 6173 745f      if forecast_
-0000df80: 6c65 6e67 7468 2069 7320 4e6f 6e65 3a0d  length is None:.
-0000df90: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-0000dfa0: 6563 7465 645f 666f 7265 5f6c 656e 203d  ected_fore_len =
-0000dfb0: 206c 656e 2864 6629 0d0a 2020 2020 2020   len(df)..      
-0000dfc0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0000dfd0: 2020 2020 2065 7870 6563 7465 645f 666f       expected_fo
-0000dfe0: 7265 5f6c 656e 203d 2028 0d0a 2020 2020  re_len = (..    
-0000dff0: 2020 2020 2020 2020 2020 2020 666f 7265              fore
-0000e000: 6361 7374 5f6c 656e 6774 6820 2b20 6c65  cast_length + le
-0000e010: 6e28 6466 2920 6966 2069 6e63 6c75 6465  n(df) if include
-0000e020: 5f68 6973 746f 7279 2065 6c73 6520 666f  _history else fo
-0000e030: 7265 6361 7374 5f6c 656e 6774 680d 0a20  recast_length.. 
-0000e040: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-0000e050: 2020 2020 2020 6966 2066 7574 7572 655f        if future_
-0000e060: 7265 6772 6573 736f 7220 6973 206e 6f74  regressor is not
-0000e070: 204e 6f6e 6520 616e 6420 7365 6c66 2e72   None and self.r
-0000e080: 6567 7265 7373 6f72 735f 7573 6564 3a0d  egressors_used:.
-0000e090: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000e0a0: 6c65 6e28 6675 7475 7265 5f72 6567 7265  len(future_regre
-0000e0b0: 7373 6f72 2920 3d3d 2065 7870 6563 7465  ssor) == expecte
-0000e0c0: 645f 666f 7265 5f6c 656e 3a0d 0a20 2020  d_fore_len:..   
-0000e0d0: 2020 2020 2020 2020 2020 2020 2066 756c               ful
-0000e0e0: 6c5f 7265 6772 203d 2073 656c 662e 7265  l_regr = self.re
-0000e0f0: 6772 6573 736f 725f 7472 616e 7366 6f72  gressor_transfor
-0000e100: 6d65 722e 7472 616e 7366 6f72 6d28 0d0a  mer.transform(..
-0000e110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e120: 2020 2020 636c 6561 6e5f 7265 6772 6573      clean_regres
-0000e130: 736f 7228 6675 7475 7265 5f72 6567 7265  sor(future_regre
-0000e140: 7373 6f72 290d 0a20 2020 2020 2020 2020  ssor)..         
-0000e150: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0000e160: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0000e170: 2020 2020 2020 2020 2020 2020 2066 756c               ful
-0000e180: 6c5f 7265 6772 203d 2070 642e 636f 6e63  l_regr = pd.conc
-0000e190: 6174 280d 0a20 2020 2020 2020 2020 2020  at(..           
-0000e1a0: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
-0000e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1c0: 2020 2020 7365 6c66 2e66 7574 7572 655f      self.future_
-0000e1d0: 7265 6772 6573 736f 725f 7472 6169 6e2c  regressor_train,
-0000e1e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e1f0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000e200: 6567 7265 7373 6f72 5f74 7261 6e73 666f  egressor_transfo
-0000e210: 726d 6572 2e74 7261 6e73 666f 726d 280d  rmer.transform(.
-0000e220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e230: 2020 2020 2020 2020 2020 2020 2063 6c65               cle
-0000e240: 616e 5f72 6567 7265 7373 6f72 280d 0a20  an_regressor(.. 
-0000e250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e260: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000e270: 7574 7572 655f 7265 6772 6573 736f 722e  uture_regressor.
-0000e280: 6c6f 635b 0d0a 2020 2020 2020 2020 2020  loc[..          
-0000e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2a0: 2020 2020 2020 2020 2020 6675 7475 7265            future
-0000e2b0: 5f72 6567 7265 7373 6f72 2e69 6e64 6578  _regressor.index
-0000e2c0: 2e64 6966 6665 7265 6e63 6528 0d0a 2020  .difference(..  
-0000e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2f0: 2020 2020 2020 7365 6c66 2e66 7574 7572        self.futur
-0000e300: 655f 7265 6772 6573 736f 725f 7472 6169  e_regressor_trai
-0000e310: 6e2e 696e 6465 780d 0a20 2020 2020 2020  n.index..       
-0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e330: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e360: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0000e370: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000e380: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e390: 2020 2020 2020 2020 2020 292c 0d0a 2020            ),..  
-0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3b0: 2020 5d0d 0a20 2020 2020 2020 2020 2020    ]..           
-0000e3c0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0000e3d0: 6966 2028 0d0a 2020 2020 2020 2020 2020  if (..          
-0000e3e0: 2020 666c 6167 5f72 6567 7265 7373 6f72    flag_regressor
-0000e3f0: 7320 6973 206e 6f74 204e 6f6e 650d 0a20  s is not None.. 
-0000e400: 2020 2020 2020 2020 2020 2061 6e64 2066             and f
-0000e410: 6f72 6563 6173 745f 6c65 6e67 7468 2069  orecast_length i
-0000e420: 7320 6e6f 7420 4e6f 6e65 0d0a 2020 2020  s not None..    
-0000e430: 2020 2020 2020 2020 616e 6420 7365 6c66          and self
-0000e440: 2e72 6567 7265 7373 6f72 735f 7573 6564  .regressors_used
-0000e450: 0d0a 2020 2020 2020 2020 293a 0d0a 2020  ..        ):..  
-0000e460: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-0000e470: 2866 6c61 675f 7265 6772 6573 736f 7273  (flag_regressors
-0000e480: 2920 3d3d 2065 7870 6563 7465 645f 666f  ) == expected_fo
-0000e490: 7265 5f6c 656e 3a0d 0a20 2020 2020 2020  re_len:..       
-0000e4a0: 2020 2020 2020 2020 2061 6c6c 5f66 6c61           all_fla
-0000e4b0: 6773 203d 2063 6c65 616e 5f72 6567 7265  gs = clean_regre
-0000e4c0: 7373 6f72 2866 6c61 675f 7265 6772 6573  ssor(flag_regres
-0000e4d0: 736f 7273 2c20 7072 6566 6978 3d22 7265  sors, prefix="re
-0000e4e0: 6772 666c 6167 735f 2229 0d0a 2020 2020  grflags_")..    
-0000e4f0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0000e500: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000e510: 6c6c 5f66 6c61 6773 203d 2070 642e 636f  ll_flags = pd.co
-0000e520: 6e63 6174 280d 0a20 2020 2020 2020 2020  ncat(..         
-0000e530: 2020 2020 2020 2020 2020 205b 0d0a 2020             [..  
-0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e550: 2020 2020 2020 7365 6c66 2e66 6c61 675f        self.flag_
-0000e560: 7265 6772 6573 736f 725f 7472 6169 6e2c  regressor_train,
-0000e570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e580: 2020 2020 2020 2020 2020 636c 6561 6e5f            clean_
-0000e590: 7265 6772 6573 736f 7228 0d0a 2020 2020  regressor(..    
-0000e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5b0: 2020 2020 2020 2020 666c 6167 5f72 6567          flag_reg
-0000e5c0: 7265 7373 6f72 732e 6c6f 635b 0d0a 2020  ressors.loc[..  
-0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5e0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
-0000e5f0: 6167 5f72 6567 7265 7373 6f72 732e 696e  ag_regressors.in
-0000e600: 6465 782e 6469 6666 6572 656e 6365 280d  dex.difference(.
-0000e610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e630: 2020 2020 2073 656c 662e 666c 6167 5f72       self.flag_r
-0000e640: 6567 7265 7373 6f72 5f74 7261 696e 2e69  egressor_train.i
-0000e650: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
-0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e670: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e690: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
-0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6b0: 2020 2020 2070 7265 6669 783d 2272 6567       prefix="reg
-0000e6c0: 7266 6c61 6773 5f22 2c0d 0a20 2020 2020  rflags_",..     
-0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6e0: 2020 2029 2c0d 0a20 2020 2020 2020 2020     ),..         
-0000e6f0: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
-0000e700: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-0000e710: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-0000e720: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-0000e730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e740: 2020 7365 6c66 2e66 6c61 675f 7265 6772    self.flag_regr
-0000e750: 6573 736f 725f 7472 6169 6e20 6973 206e  essor_train is n
-0000e760: 6f74 204e 6f6e 650d 0a20 2020 2020 2020  ot None..       
-0000e770: 2020 2020 2020 2020 2061 6e64 2066 6f72           and for
-0000e780: 6563 6173 745f 6c65 6e67 7468 2069 7320  ecast_length is 
-0000e790: 6e6f 7420 4e6f 6e65 0d0a 2020 2020 2020  not None..      
-0000e7a0: 2020 2020 2020 2020 2020 616e 6420 7365            and se
-0000e7b0: 6c66 2e72 6567 7265 7373 6f72 735f 7573  lf.regressors_us
-0000e7c0: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
-0000e7d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000e7e0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000e7f0: 7272 6f72 2822 666c 6167 5f72 6567 7265  rror("flag_regre
-0000e800: 7373 6f72 7320 7375 7070 6c69 6564 2069  ssors supplied i
-0000e810: 6e20 7472 6169 6e69 6e67 2062 7574 206e  n training but n
-0000e820: 6f74 2070 7265 6469 6374 2229 0d0a 2020  ot predict")..  
-0000e830: 2020 2020 2020 2020 2020 616c 6c5f 666c            all_fl
-0000e840: 6167 7320 3d20 7365 6c66 2e66 6c61 675f  ags = self.flag_
-0000e850: 7265 6772 6573 736f 725f 7472 6169 6e0d  regressor_train.
-0000e860: 0a20 2020 2020 2020 2069 6620 6675 7475  .        if futu
-0000e870: 7265 5f69 6d70 6163 7473 2069 7320 6e6f  re_impacts is no
-0000e880: 7420 4e6f 6e65 2061 6e64 2066 6f72 6563  t None and forec
-0000e890: 6173 745f 6c65 6e67 7468 2069 7320 6e6f  ast_length is no
-0000e8a0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-0000e8b0: 2020 2020 2069 6620 6c65 6e28 6675 7475       if len(futu
-0000e8c0: 7265 5f69 6d70 6163 7473 2920 3d3d 2065  re_impacts) == e
-0000e8d0: 7870 6563 7465 645f 666f 7265 5f6c 656e  xpected_fore_len
-0000e8e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000e8f0: 2020 2069 6d70 6163 7473 203d 2066 7574     impacts = fut
-0000e900: 7572 655f 696d 7061 6374 730d 0a20 2020  ure_impacts..   
-0000e910: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e930: 696d 7061 6374 7320 3d20 7064 2e63 6f6e  impacts = pd.con
-0000e940: 6361 7428 5b73 656c 662e 7061 7374 5f69  cat([self.past_i
-0000e950: 6d70 6163 7473 2c20 6675 7475 7265 5f69  mpacts, future_i
-0000e960: 6d70 6163 7473 5d29 0d0a 2020 2020 2020  mpacts])..      
-0000e970: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0000e980: 2020 2020 2069 6d70 6163 7473 203d 2073       impacts = s
-0000e990: 656c 662e 7061 7374 5f69 6d70 6163 7473  elf.past_impacts
-0000e9a0: 0d0a 2020 2020 2020 2020 2320 4920 646f  ..        # I do
-0000e9b0: 6e27 7420 7468 696e 6b20 7468 6572 6520  n't think there 
-0000e9c0: 6973 2061 206d 6f72 6520 6566 6669 6369  is a more effici
-0000e9d0: 656e 7420 7761 7920 746f 2063 6f6d 6269  ent way to combi
-0000e9e0: 6e65 2074 6865 7365 2064 6963 7473 206f  ne these dicts o
-0000e9f0: 6620 6461 7461 6672 616d 6573 0d0a 2020  f dataframes..  
-0000ea00: 2020 2020 2020 6966 2072 6567 7265 7373        if regress
-0000ea10: 6f72 5f70 6572 5f73 6572 6965 7320 6973  or_per_series is
-0000ea20: 206e 6f74 204e 6f6e 6520 616e 6420 7365   not None and se
-0000ea30: 6c66 2e72 6567 7265 7373 6f72 735f 7573  lf.regressors_us
-0000ea40: 6564 3a0d 0a20 2020 2020 2020 2020 2020  ed:..           
-0000ea50: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-0000ea60: 6365 2872 6567 7265 7373 6f72 5f70 6572  ce(regressor_per
-0000ea70: 5f73 6572 6965 732c 2064 6963 7429 3a0d  _series, dict):.
-0000ea80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea90: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0000eaa0: 7228 2272 6567 7265 7373 6f72 5f70 6572  r("regressor_per
-0000eab0: 5f73 6572 6965 7320 6d75 7374 2062 6520  _series must be 
-0000eac0: 6469 6374 2229 0d0a 2020 2020 2020 2020  dict")..        
-0000ead0: 2020 2020 7265 6772 5f70 735f 666f 7265      regr_ps_fore
-0000eae0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-0000eaf0: 2020 2066 6f72 206b 6579 2c20 7661 6c75     for key, valu
-0000eb00: 6520 696e 2073 656c 662e 7265 6772 5f70  e in self.regr_p
-0000eb10: 6572 5f73 6572 6965 735f 7472 2e69 7465  er_series_tr.ite
-0000eb20: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-0000eb30: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
-0000eb40: 6772 6573 736f 725f 7065 725f 7365 7269  gressor_per_seri
-0000eb50: 6573 5b6b 6579 5d29 203d 3d20 6578 7065  es[key]) == expe
-0000eb60: 6374 6564 5f66 6f72 655f 6c65 6e3a 0d0a  cted_fore_len:..
+0000d560: 6465 6620 6669 745f 6461 7461 280d 0a20  def fit_data(.. 
+0000d570: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
+0000d580: 2020 2020 2020 6466 2c0d 0a20 2020 2020        df,..     
+0000d590: 2020 2066 6f72 6563 6173 745f 6c65 6e67     forecast_leng
+0000d5a0: 7468 3d4e 6f6e 652c 0d0a 2020 2020 2020  th=None,..      
+0000d5b0: 2020 6675 7475 7265 5f72 6567 7265 7373    future_regress
+0000d5c0: 6f72 3d4e 6f6e 652c 0d0a 2020 2020 2020  or=None,..      
+0000d5d0: 2020 7265 6772 6573 736f 725f 7065 725f    regressor_per_
+0000d5e0: 7365 7269 6573 3d4e 6f6e 652c 0d0a 2020  series=None,..  
+0000d5f0: 2020 2020 2020 666c 6167 5f72 6567 7265        flag_regre
+0000d600: 7373 6f72 733d 4e6f 6e65 2c0d 0a20 2020  ssors=None,..   
+0000d610: 2020 2020 2066 7574 7572 655f 696d 7061       future_impa
+0000d620: 6374 733d 4e6f 6e65 2c0d 0a20 2020 2020  cts=None,..     
+0000d630: 2020 2072 6567 7265 7373 6f72 5f66 6f72     regressor_for
+0000d640: 6563 6173 745f 6d6f 6465 6c3d 4e6f 6e65  ecast_model=None
+0000d650: 2c0d 0a20 2020 2020 2020 2072 6567 7265  ,..        regre
+0000d660: 7373 6f72 5f66 6f72 6563 6173 745f 6d6f  ssor_forecast_mo
+0000d670: 6465 6c5f 7061 7261 6d73 3d4e 6f6e 652c  del_params=None,
+0000d680: 0d0a 2020 2020 2020 2020 7265 6772 6573  ..        regres
+0000d690: 736f 725f 666f 7265 6361 7374 5f74 7261  sor_forecast_tra
+0000d6a0: 6e73 666f 726d 6174 696f 6e73 3d4e 6f6e  nsformations=Non
+0000d6b0: 652c 0d0a 2020 2020 2020 2020 696e 636c  e,..        incl
+0000d6c0: 7564 655f 6869 7374 6f72 793d 5472 7565  ude_history=True
+0000d6d0: 2c0d 0a20 2020 2020 2020 2070 6173 745f  ,..        past_
+0000d6e0: 696d 7061 6374 733d 4e6f 6e65 2c0d 0a20  impacts=None,.. 
+0000d6f0: 2020 2029 3a0d 0a20 2020 2020 2020 2073     ):..        s
+0000d700: 656c 662e 6466 203d 2073 656c 662e 7072  elf.df = self.pr
+0000d710: 6570 726f 6365 7373 6572 2e74 7261 6e73  eprocesser.trans
+0000d720: 666f 726d 2873 656c 662e 6466 290d 0a20  form(self.df).. 
+0000d730: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+0000d740: 6173 745f 696d 7061 6374 735f 696e 7465  ast_impacts_inte
+0000d750: 7276 656e 7469 6f6e 203d 3d20 2272 656d  rvention == "rem
+0000d760: 6f76 6522 3a0d 0a20 2020 2020 2020 2020  ove":..         
+0000d770: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+0000d780: 2020 2020 2020 2020 2073 656c 662e 6466           self.df
+0000d790: 203d 2073 656c 662e 6466 202f 2028 3120   = self.df / (1 
+0000d7a0: 2b20 7061 7374 5f69 6d70 6163 7473 290d  + past_impacts).
+0000d7b0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+0000d7c0: 6570 7420 5479 7065 4572 726f 723a 0d0a  ept TypeError:..
+0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7e0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000d7f0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0000d800: 2020 2020 2020 2022 6966 2075 7369 6e67         "if using
+0000d810: 2070 6173 7420 696d 7061 6374 2077 6974   past impact wit
+0000d820: 6820 6466 2075 7064 6174 6573 2c20 6d75  h df updates, mu
+0000d830: 7374 2070 6173 7320 7061 7374 5f69 6d70  st pass past_imp
+0000d840: 6163 7473 2074 6f20 2e66 6974 5f64 6174  acts to .fit_dat
+0000d850: 6120 6f72 202e 7072 6564 6963 7422 0d0a  a or .predict"..
+0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d870: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000d880: 6466 203d 2073 656c 662e 7363 616c 655f  df = self.scale_
+0000d890: 6461 7461 2864 6629 0d0a 2020 2020 2020  data(df)..      
+0000d8a0: 2020 280d 0a20 2020 2020 2020 2020 2020    (..           
+0000d8b0: 2073 656c 662e 7265 6772 5f70 735f 666f   self.regr_ps_fo
+0000d8c0: 7265 2c0d 0a20 2020 2020 2020 2020 2020  re,..           
+0000d8d0: 2073 656c 662e 7573 655f 696d 7061 6374   self.use_impact
+0000d8e0: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+0000d8f0: 7365 6c66 2e66 756c 6c5f 7265 6772 2c0d  self.full_regr,.
+0000d900: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d910: 662e 616c 6c5f 666c 6167 732c 0d0a 2020  f.all_flags,..  
+0000d920: 2020 2020 2020 2920 3d20 7365 6c66 2e5f        ) = self._
+0000d930: 7072 6f63 6573 735f 7265 6772 6573 736f  process_regresso
+0000d940: 7273 280d 0a20 2020 2020 2020 2020 2020  rs(..           
+0000d950: 2064 663d 7365 6c66 2e64 662c 0d0a 2020   df=self.df,..  
+0000d960: 2020 2020 2020 2020 2020 666f 7265 6361            foreca
+0000d970: 7374 5f6c 656e 6774 683d 666f 7265 6361  st_length=foreca
+0000d980: 7374 5f6c 656e 6774 682c 0d0a 2020 2020  st_length,..    
+0000d990: 2020 2020 2020 2020 6675 7475 7265 5f72          future_r
+0000d9a0: 6567 7265 7373 6f72 3d66 7574 7572 655f  egressor=future_
+0000d9b0: 7265 6772 6573 736f 722c 0d0a 2020 2020  regressor,..    
+0000d9c0: 2020 2020 2020 2020 7265 6772 6573 736f          regresso
+0000d9d0: 725f 7065 725f 7365 7269 6573 3d72 6567  r_per_series=reg
+0000d9e0: 7265 7373 6f72 5f70 6572 5f73 6572 6965  ressor_per_serie
+0000d9f0: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+0000da00: 666c 6167 5f72 6567 7265 7373 6f72 733d  flag_regressors=
+0000da10: 666c 6167 5f72 6567 7265 7373 6f72 732c  flag_regressors,
+0000da20: 0d0a 2020 2020 2020 2020 2020 2020 6675  ..            fu
+0000da30: 7475 7265 5f69 6d70 6163 7473 3d66 7574  ture_impacts=fut
+0000da40: 7572 655f 696d 7061 6374 732c 0d0a 2020  ure_impacts,..  
+0000da50: 2020 2020 2020 2020 2020 7265 6772 6573            regres
+0000da60: 736f 725f 666f 7265 6361 7374 5f6d 6f64  sor_forecast_mod
+0000da70: 656c 3d72 6567 7265 7373 6f72 5f66 6f72  el=regressor_for
+0000da80: 6563 6173 745f 6d6f 6465 6c2c 0d0a 2020  ecast_model,..  
+0000da90: 2020 2020 2020 2020 2020 7265 6772 6573            regres
+0000daa0: 736f 725f 666f 7265 6361 7374 5f6d 6f64  sor_forecast_mod
+0000dab0: 656c 5f70 6172 616d 733d 7265 6772 6573  el_params=regres
+0000dac0: 736f 725f 666f 7265 6361 7374 5f6d 6f64  sor_forecast_mod
+0000dad0: 656c 5f70 6172 616d 732c 0d0a 2020 2020  el_params,..    
+0000dae0: 2020 2020 2020 2020 7265 6772 6573 736f          regresso
+0000daf0: 725f 666f 7265 6361 7374 5f74 7261 6e73  r_forecast_trans
+0000db00: 666f 726d 6174 696f 6e73 3d72 6567 7265  formations=regre
+0000db10: 7373 6f72 5f66 6f72 6563 6173 745f 7472  ssor_forecast_tr
+0000db20: 616e 7366 6f72 6d61 7469 6f6e 732c 0d0a  ansformations,..
+0000db30: 2020 2020 2020 2020 2020 2020 696e 636c              incl
+0000db40: 7564 655f 6869 7374 6f72 793d 696e 636c  ude_history=incl
+0000db50: 7564 655f 6869 7374 6f72 792c 0d0a 2020  ude_history,..  
+0000db60: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0000db70: 2073 656c 662e 7472 656e 645f 7472 6169   self.trend_trai
+0000db80: 6e20 3d20 7365 6c66 2e64 6620 2d20 7365  n = self.df - se
+0000db90: 6c66 2e5f 7072 6564 6963 745f 6c69 6e65  lf._predict_line
+0000dba0: 6172 280d 0a20 2020 2020 2020 2020 2020  ar(..           
+0000dbb0: 2064 6174 6573 3d64 662e 696e 6465 782c   dates=df.index,
+0000dbc0: 0d0a 2020 2020 2020 2020 2020 2020 6869  ..            hi
+0000dbd0: 7374 6f72 795f 6466 3d73 656c 662e 6466  story_df=self.df
+0000dbe0: 2c0d 0a20 2020 2020 2020 2020 2020 2066  ,..            f
+0000dbf0: 7574 7572 655f 7265 6772 6573 736f 723d  uture_regressor=
+0000dc00: 7365 6c66 2e66 756c 6c5f 7265 6772 2c0d  self.full_regr,.
+0000dc10: 0a20 2020 2020 2020 2020 2020 2066 6c61  .            fla
+0000dc20: 675f 7265 6772 6573 736f 7273 3d73 656c  g_regressors=sel
+0000dc30: 662e 616c 6c5f 666c 6167 732c 0d0a 2020  f.all_flags,..  
+0000dc40: 2020 2020 2020 2020 2020 696d 7061 6374            impact
+0000dc50: 733d 7365 6c66 2e75 7365 5f69 6d70 6163  s=self.use_impac
+0000dc60: 7473 2c0d 0a20 2020 2020 2020 2020 2020  ts,..           
+0000dc70: 2072 6567 7265 7373 6f72 5f70 6572 5f73   regressor_per_s
+0000dc80: 6572 6965 733d 7365 6c66 2e72 6567 725f  eries=self.regr_
+0000dc90: 7073 5f66 6f72 652c 0d0a 2020 2020 2020  ps_fore,..      
+0000dca0: 2020 290d 0a20 2020 2020 2020 2069 6620    )..        if 
+0000dcb0: 7365 6c66 2e74 7265 6e64 5f77 696e 646f  self.trend_windo
+0000dcc0: 7720 6973 206e 6f74 204e 6f6e 653a 0d0a  w is not None:..
+0000dcd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000dce0: 2e74 7265 6e64 5f74 7261 696e 2c20 736c  .trend_train, sl
+0000dcf0: 6f70 652c 2069 6e74 6572 6365 7074 203d  ope, intercept =
+0000dd00: 2073 656c 662e 726f 6c6c 696e 675f 7472   self.rolling_tr
+0000dd10: 656e 6428 0d0a 2020 2020 2020 2020 2020  end(..          
+0000dd20: 2020 2020 2020 7365 6c66 2e74 7265 6e64        self.trend
+0000dd30: 5f74 7261 696e 2c20 6e70 2e61 7272 6179  _train, np.array
+0000dd40: 2873 656c 662e 6372 6561 7465 5f74 2864  (self.create_t(d
+0000dd50: 662e 696e 6465 7829 290d 0a20 2020 2020  f.index))..     
+0000dd60: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0000dd70: 2020 2020 2020 7365 6c66 2e74 7265 6e64        self.trend
+0000dd80: 5f74 7261 696e 203d 2070 642e 4461 7461  _train = pd.Data
+0000dd90: 4672 616d 6528 0d0a 2020 2020 2020 2020  Frame(..        
+0000dda0: 2020 2020 2020 2020 7365 6c66 2e74 7265          self.tre
+0000ddb0: 6e64 5f74 7261 696e 2c20 696e 6465 783d  nd_train, index=
+0000ddc0: 6466 2e69 6e64 6578 2c20 636f 6c75 6d6e  df.index, column
+0000ddd0: 733d 6466 2e63 6f6c 756d 6e73 0d0a 2020  s=df.columns..  
+0000dde0: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
+0000ddf0: 2020 2064 6566 205f 7072 6f63 6573 735f     def _process_
+0000de00: 7265 6772 6573 736f 7273 280d 0a20 2020  regressors(..   
+0000de10: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
+0000de20: 2020 2020 6466 3d4e 6f6e 652c 0d0a 2020      df=None,..  
+0000de30: 2020 2020 2020 666f 7265 6361 7374 5f6c        forecast_l
+0000de40: 656e 6774 683d 4e6f 6e65 2c0d 0a20 2020  ength=None,..   
+0000de50: 2020 2020 2066 7574 7572 655f 7265 6772       future_regr
+0000de60: 6573 736f 723d 4e6f 6e65 2c0d 0a20 2020  essor=None,..   
+0000de70: 2020 2020 2072 6567 7265 7373 6f72 5f70       regressor_p
+0000de80: 6572 5f73 6572 6965 733d 4e6f 6e65 2c0d  er_series=None,.
+0000de90: 0a20 2020 2020 2020 2066 6c61 675f 7265  .        flag_re
+0000dea0: 6772 6573 736f 7273 3d4e 6f6e 652c 0d0a  gressors=None,..
+0000deb0: 2020 2020 2020 2020 6675 7475 7265 5f69          future_i
+0000dec0: 6d70 6163 7473 3d4e 6f6e 652c 0d0a 2020  mpacts=None,..  
+0000ded0: 2020 2020 2020 7265 6772 6573 736f 725f        regressor_
+0000dee0: 666f 7265 6361 7374 5f6d 6f64 656c 3d4e  forecast_model=N
+0000def0: 6f6e 652c 0d0a 2020 2020 2020 2020 7265  one,..        re
+0000df00: 6772 6573 736f 725f 666f 7265 6361 7374  gressor_forecast
+0000df10: 5f6d 6f64 656c 5f70 6172 616d 733d 4e6f  _model_params=No
+0000df20: 6e65 2c0d 0a20 2020 2020 2020 2072 6567  ne,..        reg
+0000df30: 7265 7373 6f72 5f66 6f72 6563 6173 745f  ressor_forecast_
+0000df40: 7472 616e 7366 6f72 6d61 7469 6f6e 733d  transformations=
+0000df50: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2069  None,..        i
+0000df60: 6e63 6c75 6465 5f68 6973 746f 7279 3d54  nclude_history=T
+0000df70: 7275 652c 0d0a 2020 2020 293a 0d0a 2020  rue,..    ):..  
+0000df80: 2020 2020 2020 2320 6966 2066 7574 7572        # if futur
+0000df90: 6520 7265 6772 6573 736f 7273 2061 7265  e regressors are
+0000dfa0: 204e 6f6e 6520 2826 2055 5345 4429 2c20   None (& USED), 
+0000dfb0: 6275 7420 7765 7265 2070 726f 7669 6465  but were provide
+0000dfc0: 6420 666f 7220 6869 7374 6f72 792c 2069  d for history, i
+0000dfd0: 6e73 7465 6164 2075 7365 2066 6f72 6563  nstead use forec
+0000dfe0: 6173 7473 206f 6620 7468 6573 6520 6665  asts of these fe
+0000dff0: 6174 7572 6573 2028 7761 726e 290d 0a20  atures (warn).. 
+0000e000: 2020 2020 2020 2066 756c 6c5f 7265 6772         full_regr
+0000e010: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
+0000e020: 2069 6620 280d 0a20 2020 2020 2020 2020   if (..         
+0000e030: 2020 2066 7574 7572 655f 7265 6772 6573     future_regres
+0000e040: 736f 7220 6973 204e 6f6e 650d 0a20 2020  sor is None..   
+0000e050: 2020 2020 2020 2020 2061 6e64 2073 656c           and sel
+0000e060: 662e 6675 7475 7265 5f72 6567 7265 7373  f.future_regress
+0000e070: 6f72 5f74 7261 696e 2069 7320 6e6f 7420  or_train is not 
+0000e080: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
+0000e090: 2020 616e 6420 666f 7265 6361 7374 5f6c    and forecast_l
+0000e0a0: 656e 6774 6820 6973 206e 6f74 204e 6f6e  ength is not Non
+0000e0b0: 650d 0a20 2020 2020 2020 2029 3a0d 0a20  e..        ):.. 
+0000e0c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000e0d0: 6c66 2e76 6572 626f 7365 203e 2030 3a0d  lf.verbose > 0:.
+0000e0e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e0f0: 2070 7269 6e74 280d 0a20 2020 2020 2020   print(..       
+0000e100: 2020 2020 2020 2020 2020 2020 2022 6675               "fu
+0000e110: 7475 7265 5f72 6567 7265 7373 6f72 206e  ture_regressor n
+0000e120: 6f74 2070 726f 7669 6465 6420 746f 2043  ot provided to C
+0000e130: 6173 7361 6e64 7261 2c20 7573 696e 6720  assandra, using 
+0000e140: 666f 7265 6361 7374 7320 6f66 2068 6973  forecasts of his
+0000e150: 746f 7269 6361 6c22 0d0a 2020 2020 2020  torical"..      
+0000e160: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0000e170: 2020 2020 2020 2020 2066 7574 7572 655f           future_
+0000e180: 7265 6772 6573 736f 7220 3d20 6d6f 6465  regressor = mode
+0000e190: 6c5f 666f 7265 6361 7374 280d 0a20 2020  l_forecast(..   
+0000e1a0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+0000e1b0: 656c 5f6e 616d 653d 7365 6c66 2e74 7265  el_name=self.tre
+0000e1c0: 6e64 5f6d 6f64 656c 5b27 4d6f 6465 6c27  nd_model['Model'
+0000e1d0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000e1e0: 2020 2069 6620 7265 6772 6573 736f 725f     if regressor_
+0000e1f0: 666f 7265 6361 7374 5f6d 6f64 656c 2069  forecast_model i
+0000e200: 7320 4e6f 6e65 0d0a 2020 2020 2020 2020  s None..        
+0000e210: 2020 2020 2020 2020 656c 7365 2072 6567          else reg
+0000e220: 7265 7373 6f72 5f66 6f72 6563 6173 745f  ressor_forecast_
+0000e230: 6d6f 6465 6c2c 0d0a 2020 2020 2020 2020  model,..        
+0000e240: 2020 2020 2020 2020 6d6f 6465 6c5f 7061          model_pa
+0000e250: 7261 6d5f 6469 6374 3d73 656c 662e 7472  ram_dict=self.tr
+0000e260: 656e 645f 6d6f 6465 6c5b 274d 6f64 656c  end_model['Model
+0000e270: 5061 7261 6d65 7465 7273 275d 0d0a 2020  Parameters']..  
+0000e280: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000e290: 2072 6567 7265 7373 6f72 5f66 6f72 6563   regressor_forec
+0000e2a0: 6173 745f 6d6f 6465 6c5f 7061 7261 6d73  ast_model_params
+0000e2b0: 2069 7320 4e6f 6e65 0d0a 2020 2020 2020   is None..      
+0000e2c0: 2020 2020 2020 2020 2020 656c 7365 2072            else r
+0000e2d0: 6567 7265 7373 6f72 5f66 6f72 6563 6173  egressor_forecas
+0000e2e0: 745f 6d6f 6465 6c5f 7061 7261 6d73 2c0d  t_model_params,.
+0000e2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e300: 206d 6f64 656c 5f74 7261 6e73 666f 726d   model_transform
+0000e310: 5f64 6963 743d 7365 6c66 2e70 7265 7072  _dict=self.prepr
+0000e320: 6f63 6573 7369 6e67 5f74 7261 6e73 666f  ocessing_transfo
+0000e330: 726d 6174 696f 6e0d 0a20 2020 2020 2020  rmation..       
+0000e340: 2020 2020 2020 2020 2069 6620 7265 6772           if regr
+0000e350: 6573 736f 725f 666f 7265 6361 7374 5f74  essor_forecast_t
+0000e360: 7261 6e73 666f 726d 6174 696f 6e73 2069  ransformations i
+0000e370: 7320 4e6f 6e65 0d0a 2020 2020 2020 2020  s None..        
+0000e380: 2020 2020 2020 2020 656c 7365 2072 6567          else reg
+0000e390: 7265 7373 6f72 5f66 6f72 6563 6173 745f  ressor_forecast_
+0000e3a0: 7472 616e 7366 6f72 6d61 7469 6f6e 732c  transformations,
+0000e3b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e3c0: 2020 6466 5f74 7261 696e 3d73 656c 662e    df_train=self.
+0000e3d0: 6675 7475 7265 5f72 6567 7265 7373 6f72  future_regressor
+0000e3e0: 5f74 7261 696e 2c0d 0a20 2020 2020 2020  _train,..       
+0000e3f0: 2020 2020 2020 2020 2066 6f72 6563 6173           forecas
+0000e400: 745f 6c65 6e67 7468 3d66 6f72 6563 6173  t_length=forecas
+0000e410: 745f 6c65 6e67 7468 2c0d 0a20 2020 2020  t_length,..     
+0000e420: 2020 2020 2020 2020 2020 2066 7265 7175             frequ
+0000e430: 656e 6379 3d73 656c 662e 6672 6571 7565  ency=self.freque
+0000e440: 6e63 792c 0d0a 2020 2020 2020 2020 2020  ncy,..          
+0000e450: 2020 2020 2020 7072 6564 6963 7469 6f6e        prediction
+0000e460: 5f69 6e74 6572 7661 6c3d 7365 6c66 2e70  _interval=self.p
+0000e470: 7265 6469 6374 696f 6e5f 696e 7465 7276  rediction_interv
+0000e480: 616c 2c0d 0a20 2020 2020 2020 2020 2020  al,..           
+0000e490: 2020 2020 2066 6169 6c5f 6f6e 5f66 6f72       fail_on_for
+0000e4a0: 6563 6173 745f 6e61 6e3d 4661 6c73 652c  ecast_nan=False,
+0000e4b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e4c0: 2020 7261 6e64 6f6d 5f73 6565 643d 7365    random_seed=se
+0000e4d0: 6c66 2e72 616e 646f 6d5f 7365 6564 2c0d  lf.random_seed,.
+0000e4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e4f0: 2076 6572 626f 7365 3d73 656c 662e 7665   verbose=self.ve
+0000e500: 7262 6f73 652c 0d0a 2020 2020 2020 2020  rbose,..        
+0000e510: 2020 2020 2020 2020 6e5f 6a6f 6273 3d73          n_jobs=s
+0000e520: 656c 662e 6e5f 6a6f 6273 2c0d 0a20 2020  elf.n_jobs,..   
+0000e530: 2020 2020 2020 2020 2029 2e66 6f72 6563           ).forec
+0000e540: 6173 740d 0a20 2020 2020 2020 2020 2020  ast..           
+0000e550: 2066 756c 6c5f 7265 6772 203d 2070 642e   full_regr = pd.
+0000e560: 636f 6e63 6174 285b 7365 6c66 2e66 7574  concat([self.fut
+0000e570: 7572 655f 7265 6772 6573 736f 725f 7472  ure_regressor_tr
+0000e580: 6169 6e2c 2066 7574 7572 655f 7265 6772  ain, future_regr
+0000e590: 6573 736f 725d 290d 0a20 2020 2020 2020  essor])..       
+0000e5a0: 2069 6620 666f 7265 6361 7374 5f6c 656e   if forecast_len
+0000e5b0: 6774 6820 6973 204e 6f6e 653a 0d0a 2020  gth is None:..  
+0000e5c0: 2020 2020 2020 2020 2020 6578 7065 6374            expect
+0000e5d0: 6564 5f66 6f72 655f 6c65 6e20 3d20 6c65  ed_fore_len = le
+0000e5e0: 6e28 6466 290d 0a20 2020 2020 2020 2065  n(df)..        e
+0000e5f0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0000e600: 2020 6578 7065 6374 6564 5f66 6f72 655f    expected_fore_
+0000e610: 6c65 6e20 3d20 280d 0a20 2020 2020 2020  len = (..       
+0000e620: 2020 2020 2020 2020 2066 6f72 6563 6173           forecas
+0000e630: 745f 6c65 6e67 7468 202b 206c 656e 2864  t_length + len(d
+0000e640: 6629 2069 6620 696e 636c 7564 655f 6869  f) if include_hi
+0000e650: 7374 6f72 7920 656c 7365 2066 6f72 6563  story else forec
+0000e660: 6173 745f 6c65 6e67 7468 0d0a 2020 2020  ast_length..    
+0000e670: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0000e680: 2020 2069 6620 6675 7475 7265 5f72 6567     if future_reg
+0000e690: 7265 7373 6f72 2069 7320 6e6f 7420 4e6f  ressor is not No
+0000e6a0: 6e65 2061 6e64 2073 656c 662e 7265 6772  ne and self.regr
+0000e6b0: 6573 736f 7273 5f75 7365 643a 0d0a 2020  essors_used:..  
+0000e6c0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+0000e6d0: 2866 7574 7572 655f 7265 6772 6573 736f  (future_regresso
+0000e6e0: 7229 203d 3d20 6578 7065 6374 6564 5f66  r) == expected_f
+0000e6f0: 6f72 655f 6c65 6e3a 0d0a 2020 2020 2020  ore_len:..      
+0000e700: 2020 2020 2020 2020 2020 6675 6c6c 5f72            full_r
+0000e710: 6567 7220 3d20 7365 6c66 2e72 6567 7265  egr = self.regre
+0000e720: 7373 6f72 5f74 7261 6e73 666f 726d 6572  ssor_transformer
+0000e730: 2e74 7261 6e73 666f 726d 280d 0a20 2020  .transform(..   
+0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e750: 2063 6c65 616e 5f72 6567 7265 7373 6f72   clean_regressor
+0000e760: 2866 7574 7572 655f 7265 6772 6573 736f  (future_regresso
+0000e770: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
+0000e780: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+0000e790: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0000e7a0: 2020 2020 2020 2020 2020 6675 6c6c 5f72            full_r
+0000e7b0: 6567 7220 3d20 7064 2e63 6f6e 6361 7428  egr = pd.concat(
+0000e7c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e7d0: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
+0000e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7f0: 2073 656c 662e 6675 7475 7265 5f72 6567   self.future_reg
+0000e800: 7265 7373 6f72 5f74 7261 696e 2c0d 0a20  ressor_train,.. 
+0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e820: 2020 2020 2020 2073 656c 662e 7265 6772         self.regr
+0000e830: 6573 736f 725f 7472 616e 7366 6f72 6d65  essor_transforme
+0000e840: 722e 7472 616e 7366 6f72 6d28 0d0a 2020  r.transform(..  
+0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e860: 2020 2020 2020 2020 2020 636c 6561 6e5f            clean_
+0000e870: 7265 6772 6573 736f 7228 0d0a 2020 2020  regressor(..    
+0000e880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e890: 2020 2020 2020 2020 2020 2020 6675 7475              futu
+0000e8a0: 7265 5f72 6567 7265 7373 6f72 2e6c 6f63  re_regressor.loc
+0000e8b0: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8d0: 2020 2020 2020 2066 7574 7572 655f 7265         future_re
+0000e8e0: 6772 6573 736f 722e 696e 6465 782e 6469  gressor.index.di
+0000e8f0: 6666 6572 656e 6365 280d 0a20 2020 2020  fference(..     
+0000e900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e920: 2020 2073 656c 662e 6675 7475 7265 5f72     self.future_r
+0000e930: 6567 7265 7373 6f72 5f74 7261 696e 2e69  egressor_train.i
+0000e940: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
+0000e950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e960: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e980: 2020 2020 2020 2020 2020 2020 205d 0d0a               ]..
+0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9a0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9c0: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
+0000e9d0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+0000e9e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e9f0: 2020 290d 0a20 2020 2020 2020 2069 6620    )..        if 
+0000ea00: 280d 0a20 2020 2020 2020 2020 2020 2066  (..            f
+0000ea10: 6c61 675f 7265 6772 6573 736f 7273 2069  lag_regressors i
+0000ea20: 7320 6e6f 7420 4e6f 6e65 0d0a 2020 2020  s not None..    
+0000ea30: 2020 2020 2020 2020 616e 6420 666f 7265          and fore
+0000ea40: 6361 7374 5f6c 656e 6774 6820 6973 206e  cast_length is n
+0000ea50: 6f74 204e 6f6e 650d 0a20 2020 2020 2020  ot None..       
+0000ea60: 2020 2020 2061 6e64 2073 656c 662e 7265       and self.re
+0000ea70: 6772 6573 736f 7273 5f75 7365 640d 0a20  gressors_used.. 
+0000ea80: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
+0000ea90: 2020 2020 2020 2069 6620 6c65 6e28 666c         if len(fl
+0000eaa0: 6167 5f72 6567 7265 7373 6f72 7329 203d  ag_regressors) =
+0000eab0: 3d20 6578 7065 6374 6564 5f66 6f72 655f  = expected_fore_
+0000eac0: 6c65 6e3a 0d0a 2020 2020 2020 2020 2020  len:..          
+0000ead0: 2020 2020 2020 616c 6c5f 666c 6167 7320        all_flags 
+0000eae0: 3d20 636c 6561 6e5f 7265 6772 6573 736f  = clean_regresso
+0000eaf0: 7228 666c 6167 5f72 6567 7265 7373 6f72  r(flag_regressor
+0000eb00: 732c 2070 7265 6669 783d 2272 6567 7266  s, prefix="regrf
+0000eb10: 6c61 6773 5f22 290d 0a20 2020 2020 2020  lags_")..       
+0000eb20: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000eb30: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+0000eb40: 666c 6167 7320 3d20 7064 2e63 6f6e 6361  flags = pd.conca
+0000eb50: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+0000eb60: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
 0000eb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb80: 2020 2020 7265 6772 5f70 735f 666f 7265      regr_ps_fore
-0000eb90: 5b6b 6579 5d20 3d20 7265 6772 6573 736f  [key] = regresso
-0000eba0: 725f 7065 725f 7365 7269 6573 5b6b 6579  r_per_series[key
-0000ebb0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0000ebc0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000ebd0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000ebe0: 6772 5f70 735f 666f 7265 5b6b 6579 5d20  gr_ps_fore[key] 
-0000ebf0: 3d20 7064 2e63 6f6e 6361 7428 0d0a 2020  = pd.concat(..  
+0000eb80: 2020 2073 656c 662e 666c 6167 5f72 6567     self.flag_reg
+0000eb90: 7265 7373 6f72 5f74 7261 696e 2c0d 0a20  ressor_train,.. 
+0000eba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebb0: 2020 2020 2020 2063 6c65 616e 5f72 6567         clean_reg
+0000ebc0: 7265 7373 6f72 280d 0a20 2020 2020 2020  ressor(..       
+0000ebd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebe0: 2020 2020 2066 6c61 675f 7265 6772 6573       flag_regres
+0000ebf0: 736f 7273 2e6c 6f63 5b0d 0a20 2020 2020  sors.loc[..     
 0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec10: 2020 2020 2020 5b73 656c 662e 7265 6772        [self.regr
-0000ec20: 5f70 6572 5f73 6572 6965 735f 7472 5b6b  _per_series_tr[k
-0000ec30: 6579 5d2c 2072 6567 7265 7373 6f72 5f70  ey], regressor_p
-0000ec40: 6572 5f73 6572 6965 735b 6b65 795d 5d0d  er_series[key]].
-0000ec50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ec60: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0000ec70: 2020 2020 2020 2020 2020 2020 7265 6772              regr
-0000ec80: 5f70 735f 666f 7265 5b6b 6579 5d20 3d20  _ps_fore[key] = 
-0000ec90: 7265 6772 5f70 735f 666f 7265 5b6b 6579  regr_ps_fore[key
-0000eca0: 5d2e 696c 6f63 5b0d 0a20 2020 2020 2020  ].iloc[..       
+0000ec10: 2020 2020 2020 2020 2020 2066 6c61 675f             flag_
+0000ec20: 7265 6772 6573 736f 7273 2e69 6e64 6578  regressors.index
+0000ec30: 2e64 6966 6665 7265 6e63 6528 0d0a 2020  .difference(..  
+0000ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec60: 2020 7365 6c66 2e66 6c61 675f 7265 6772    self.flag_regr
+0000ec70: 6573 736f 725f 7472 6169 6e2e 696e 6465  essor_train.inde
+0000ec80: 780d 0a20 2020 2020 2020 2020 2020 2020  x..             
+0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eca0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
 0000ecb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecc0: 207e 7265 6772 5f70 735f 666f 7265 5b6b   ~regr_ps_fore[k
-0000ecd0: 6579 5d2e 696e 6465 782e 6475 706c 6963  ey].index.duplic
-0000ece0: 6174 6564 2829 0d0a 2020 2020 2020 2020  ated()..        
-0000ecf0: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
-0000ed00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ed10: 656c 662e 7265 6772 5f70 7320 3d20 7265  elf.regr_ps = re
-0000ed20: 6772 5f70 735f 666f 7265 0d0a 2020 2020  gr_ps_fore..    
-0000ed30: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0000ed40: 2020 2020 2020 2072 6567 725f 7073 5f66         regr_ps_f
-0000ed50: 6f72 6520 3d20 7365 6c66 2e72 6567 725f  ore = self.regr_
-0000ed60: 7065 725f 7365 7269 6573 5f74 720d 0a0d  per_series_tr...
-0000ed70: 0a20 2020 2020 2020 2023 2067 656e 6572  .        # gener
-0000ed80: 6174 6520 7472 656e 640d 0a20 2020 2020  ate trend..     
-0000ed90: 2020 2023 204d 4159 2057 414e 5420 544f     # MAY WANT TO
-0000eda0: 2050 4153 5320 6675 7475 7265 5f72 6567   PASS future_reg
-0000edb0: 7265 7373 6f72 2048 4552 450d 0a20 2020  ressor HERE..   
-0000edc0: 2020 2020 2072 6573 6964 203d 204e 6f6e       resid = Non
-0000edd0: 650d 0a20 2020 2020 2020 2069 6620 666f  e..        if fo
-0000ede0: 7265 6361 7374 5f6c 656e 6774 6820 6973  recast_length is
-0000edf0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-0000ee00: 2020 2020 2020 2020 2320 6372 6561 7465          # create
-0000ee10: 206e 6577 2072 6f6c 6c69 6e67 2072 6573   new rolling res
-0000ee20: 6964 7561 6c20 6966 206e 6577 2064 6174  idual if new dat
-0000ee30: 6120 7072 6f76 6964 6564 0d0a 2020 2020  a provided..    
-0000ee40: 2020 2020 2020 2020 6966 206e 6577 5f64          if new_d
-0000ee50: 6620 6973 206e 6f74 204e 6f6e 653a 0d0a  f is not None:..
-0000ee60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee70: 7265 7369 6420 3d20 6466 202d 2073 656c  resid = df - sel
-0000ee80: 662e 5f70 7265 6469 6374 5f6c 696e 6561  f._predict_linea
-0000ee90: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
-0000eea0: 2020 2020 2020 2020 6461 7465 733d 6466          dates=df
-0000eeb0: 2e69 6e64 6578 2c0d 0a20 2020 2020 2020  .index,..       
-0000eec0: 2020 2020 2020 2020 2020 2020 2068 6973               his
-0000eed0: 746f 7279 5f64 663d 6466 2c0d 0a20 2020  tory_df=df,..   
-0000eee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eef0: 2066 7574 7572 655f 7265 6772 6573 736f   future_regresso
-0000ef00: 723d 6675 6c6c 5f72 6567 722c 0d0a 2020  r=full_regr,..  
+0000ecc0: 2020 5d2c 0d0a 2020 2020 2020 2020 2020    ],..          
+0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ece0: 2020 7072 6566 6978 3d22 7265 6772 666c    prefix="regrfl
+0000ecf0: 6167 735f 222c 0d0a 2020 2020 2020 2020  ags_",..        
+0000ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed10: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000ed20: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
+0000ed30: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+0000ed40: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0000ed50: 2020 2020 2020 2020 2069 6620 280d 0a20           if (.. 
+0000ed60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ed70: 656c 662e 666c 6167 5f72 6567 7265 7373  elf.flag_regress
+0000ed80: 6f72 5f74 7261 696e 2069 7320 6e6f 7420  or_train is not 
+0000ed90: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
+0000eda0: 2020 2020 2020 616e 6420 666f 7265 6361        and foreca
+0000edb0: 7374 5f6c 656e 6774 6820 6973 206e 6f74  st_length is not
+0000edc0: 204e 6f6e 650d 0a20 2020 2020 2020 2020   None..         
+0000edd0: 2020 2020 2020 2061 6e64 2073 656c 662e         and self.
+0000ede0: 7265 6772 6573 736f 7273 5f75 7365 640d  regressors_used.
+0000edf0: 0a20 2020 2020 2020 2020 2020 2029 3a0d  .            ):.
+0000ee00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ee10: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0000ee20: 7228 2266 6c61 675f 7265 6772 6573 736f  r("flag_regresso
+0000ee30: 7273 2073 7570 706c 6965 6420 696e 2074  rs supplied in t
+0000ee40: 7261 696e 696e 6720 6275 7420 6e6f 7420  raining but not 
+0000ee50: 7072 6564 6963 7422 290d 0a20 2020 2020  predict")..     
+0000ee60: 2020 2020 2020 2061 6c6c 5f66 6c61 6773         all_flags
+0000ee70: 203d 2073 656c 662e 666c 6167 5f72 6567   = self.flag_reg
+0000ee80: 7265 7373 6f72 5f74 7261 696e 0d0a 2020  ressor_train..  
+0000ee90: 2020 2020 2020 6966 2066 7574 7572 655f        if future_
+0000eea0: 696d 7061 6374 7320 6973 206e 6f74 204e  impacts is not N
+0000eeb0: 6f6e 6520 616e 6420 666f 7265 6361 7374  one and forecast
+0000eec0: 5f6c 656e 6774 6820 6973 206e 6f74 204e  _length is not N
+0000eed0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000eee0: 2020 6966 206c 656e 2866 7574 7572 655f    if len(future_
+0000eef0: 696d 7061 6374 7329 203d 3d20 6578 7065  impacts) == expe
+0000ef00: 6374 6564 5f66 6f72 655f 6c65 6e3a 0d0a  cted_fore_len:..
 0000ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef20: 2020 666c 6167 5f72 6567 7265 7373 6f72    flag_regressor
-0000ef30: 733d 616c 6c5f 666c 6167 732c 0d0a 2020  s=all_flags,..  
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef50: 2020 696d 7061 6374 733d 696d 7061 6374    impacts=impact
-0000ef60: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-0000ef70: 2020 2020 2020 2020 7265 6772 6573 736f          regresso
-0000ef80: 725f 7065 725f 7365 7269 6573 3d72 6567  r_per_series=reg
-0000ef90: 725f 7073 5f66 6f72 652c 0d0a 2020 2020  r_ps_fore,..    
-0000efa0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-0000efb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000efc0: 6620 7365 6c66 2e74 7265 6e64 5f77 696e  f self.trend_win
-0000efd0: 646f 7720 6973 206e 6f74 204e 6f6e 653a  dow is not None:
-0000efe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000eff0: 2020 2020 2020 7265 7369 642c 2073 6c6f        resid, slo
-0000f000: 7065 2c20 696e 7465 7263 6570 7420 3d20  pe, intercept = 
-0000f010: 7365 6c66 2e72 6f6c 6c69 6e67 5f74 7265  self.rolling_tre
-0000f020: 6e64 280d 0a20 2020 2020 2020 2020 2020  nd(..           
-0000f030: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0000f040: 6964 2c20 6e70 2e61 7272 6179 2873 656c  id, np.array(sel
-0000f050: 662e 6372 6561 7465 5f74 2864 662e 696e  f.create_t(df.in
-0000f060: 6465 7829 290d 0a20 2020 2020 2020 2020  dex))..         
-0000f070: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-0000f080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f090: 2020 7265 7369 6420 3d20 7064 2e44 6174    resid = pd.Dat
-0000f0a0: 6146 7261 6d65 2872 6573 6964 2c20 696e  aFrame(resid, in
-0000f0b0: 6465 783d 6466 2e69 6e64 6578 2c20 636f  dex=df.index, co
-0000f0c0: 6c75 6d6e 733d 6466 2e63 6f6c 756d 6e73  lumns=df.columns
-0000f0d0: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-0000f0e0: 665f 7472 6169 6e20 3d20 7365 6c66 2e74  f_train = self.t
-0000f0f0: 7265 6e64 5f74 7261 696e 2069 6620 7265  rend_train if re
-0000f100: 7369 6420 6973 204e 6f6e 6520 656c 7365  sid is None else
-0000f110: 2072 6573 6964 0d0a 2020 2020 2020 2020   resid..        
-0000f120: 2020 2020 2320 636f 6d62 696e 6520 7265      # combine re
-0000f130: 6772 6573 736f 7220 7479 7065 7320 6465  gressor types de
-0000f140: 7065 6e64 696e 6720 6f6e 2077 6861 7420  pending on what 
-0000f150: 6973 2067 6976 656e 0d0a 2020 2020 2020  is given..      
-0000f160: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
-0000f170: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f180: 2e66 7574 7572 655f 7265 6772 6573 736f  .future_regresso
-0000f190: 725f 7472 6169 6e20 6973 204e 6f6e 650d  r_train is None.
-0000f1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f1b0: 2061 6e64 2073 656c 662e 666c 6167 5f72   and self.flag_r
-0000f1c0: 6567 7265 7373 6f72 5f74 7261 696e 2069  egressor_train i
-0000f1d0: 7320 6e6f 7420 4e6f 6e65 0d0a 2020 2020  s not None..    
-0000f1e0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0000f1f0: 7365 6c66 2e72 6567 7265 7373 6f72 735f  self.regressors_
-0000f200: 7573 6564 0d0a 2020 2020 2020 2020 2020  used..          
-0000f210: 2020 293a 0d0a 2020 2020 2020 2020 2020    ):..          
-0000f220: 2020 2020 2020 636f 6d70 5f72 6567 725f        comp_regr_
-0000f230: 7472 6169 6e20 3d20 7365 6c66 2e66 6c61  train = self.fla
-0000f240: 675f 7265 6772 6573 736f 725f 7472 6169  g_regressor_trai
-0000f250: 6e2e 7265 696e 6465 7828 0d0a 2020 2020  n.reindex(..    
-0000f260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f270: 696e 6465 783d 6466 5f74 7261 696e 2e69  index=df_train.i
-0000f280: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
-0000f290: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0000f2a0: 2020 2020 2020 2020 2063 6f6d 705f 7265           comp_re
-0000f2b0: 6772 203d 2061 6c6c 5f66 6c61 6773 2e74  gr = all_flags.t
-0000f2c0: 6169 6c28 666f 7265 6361 7374 5f6c 656e  ail(forecast_len
-0000f2d0: 6774 6829 0d0a 2020 2020 2020 2020 2020  gth)..          
-0000f2e0: 2020 656c 6966 2028 0d0a 2020 2020 2020    elif (..      
-0000f2f0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-0000f300: 7574 7572 655f 7265 6772 6573 736f 725f  uture_regressor_
-0000f310: 7472 6169 6e20 6973 206e 6f74 204e 6f6e  train is not Non
-0000f320: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-0000f330: 2020 2061 6e64 2073 656c 662e 666c 6167     and self.flag
-0000f340: 5f72 6567 7265 7373 6f72 5f74 7261 696e  _regressor_train
-0000f350: 2069 7320 4e6f 6e65 0d0a 2020 2020 2020   is None..      
-0000f360: 2020 2020 2020 2020 2020 616e 6420 7365            and se
-0000f370: 6c66 2e72 6567 7265 7373 6f72 735f 7573  lf.regressors_us
-0000f380: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
-0000f390: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000f3a0: 2020 2020 636f 6d70 5f72 6567 725f 7472      comp_regr_tr
-0000f3b0: 6169 6e20 3d20 7365 6c66 2e66 7574 7572  ain = self.futur
-0000f3c0: 655f 7265 6772 6573 736f 725f 7472 6169  e_regressor_trai
-0000f3d0: 6e2e 7265 696e 6465 7828 0d0a 2020 2020  n.reindex(..    
-0000f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3f0: 696e 6465 783d 6466 5f74 7261 696e 2e69  index=df_train.i
-0000f400: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
-0000f410: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0000f420: 2020 2020 2020 2020 2063 6f6d 705f 7265           comp_re
-0000f430: 6772 203d 2066 756c 6c5f 7265 6772 2e74  gr = full_regr.t
-0000f440: 6169 6c28 666f 7265 6361 7374 5f6c 656e  ail(forecast_len
-0000f450: 6774 6829 0d0a 2020 2020 2020 2020 2020  gth)..          
-0000f460: 2020 656c 6966 2028 0d0a 2020 2020 2020    elif (..      
-0000f470: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-0000f480: 7574 7572 655f 7265 6772 6573 736f 725f  uture_regressor_
-0000f490: 7472 6169 6e20 6973 206e 6f74 204e 6f6e  train is not Non
-0000f4a0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-0000f4b0: 2020 2061 6e64 2073 656c 662e 666c 6167     and self.flag
-0000f4c0: 5f72 6567 7265 7373 6f72 5f74 7261 696e  _regressor_train
-0000f4d0: 2069 7320 6e6f 7420 4e6f 6e65 0d0a 2020   is not None..  
-0000f4e0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-0000f4f0: 6420 7365 6c66 2e72 6567 7265 7373 6f72  d self.regressor
-0000f500: 735f 7573 6564 0d0a 2020 2020 2020 2020  s_used..        
-0000f510: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
-0000f520: 2020 2020 2020 2020 636f 6d70 5f72 6567          comp_reg
-0000f530: 725f 7472 6169 6e20 3d20 7064 2e63 6f6e  r_train = pd.con
-0000f540: 6361 7428 0d0a 2020 2020 2020 2020 2020  cat(..          
-0000f550: 2020 2020 2020 2020 2020 5b73 656c 662e            [self.
-0000f560: 6675 7475 7265 5f72 6567 7265 7373 6f72  future_regressor
-0000f570: 5f74 7261 696e 2c20 7365 6c66 2e66 6c61  _train, self.fla
-0000f580: 675f 7265 6772 6573 736f 725f 7472 6169  g_regressor_trai
-0000f590: 6e5d 2c20 6178 6973 3d31 0d0a 2020 2020  n], axis=1..    
-0000f5a0: 2020 2020 2020 2020 2020 2020 292e 7265              ).re
-0000f5b0: 696e 6465 7828 696e 6465 783d 6466 5f74  index(index=df_t
-0000f5c0: 7261 696e 2e69 6e64 6578 290d 0a20 2020  rain.index)..   
-0000f5d0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-0000f5e0: 705f 7265 6772 203d 2070 642e 636f 6e63  p_regr = pd.conc
-0000f5f0: 6174 285b 6675 6c6c 5f72 6567 722c 2061  at([full_regr, a
-0000f600: 6c6c 5f66 6c61 6773 5d2c 2061 7869 733d  ll_flags], axis=
-0000f610: 3129 2e74 6169 6c28 0d0a 2020 2020 2020  1).tail(..      
-0000f620: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000f630: 7265 6361 7374 5f6c 656e 6774 680d 0a20  recast_length.. 
-0000f640: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000f650: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0000f660: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000f670: 2020 2020 2063 6f6d 705f 7265 6772 5f74       comp_regr_t
-0000f680: 7261 696e 203d 204e 6f6e 650d 0a20 2020  rain = None..   
-0000f690: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-0000f6a0: 705f 7265 6772 203d 204e 6f6e 650d 0a0d  p_regr = None...
-0000f6b0: 0a20 2020 2020 2020 2020 2020 2074 7265  .            tre
-0000f6c0: 6e64 5f66 6f72 6563 6173 7420 3d20 6d6f  nd_forecast = mo
-0000f6d0: 6465 6c5f 666f 7265 6361 7374 280d 0a20  del_forecast(.. 
-0000f6e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000f6f0: 6f64 656c 5f6e 616d 653d 7365 6c66 2e74  odel_name=self.t
-0000f700: 7265 6e64 5f6d 6f64 656c 5b27 4d6f 6465  rend_model['Mode
-0000f710: 6c27 5d2c 0d0a 2020 2020 2020 2020 2020  l'],..          
-0000f720: 2020 2020 2020 6d6f 6465 6c5f 7061 7261        model_para
-0000f730: 6d5f 6469 6374 3d73 656c 662e 7472 656e  m_dict=self.tren
-0000f740: 645f 6d6f 6465 6c5b 274d 6f64 656c 5061  d_model['ModelPa
-0000f750: 7261 6d65 7465 7273 275d 2c0d 0a20 2020  rameters'],..   
-0000f760: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-0000f770: 656c 5f74 7261 6e73 666f 726d 5f64 6963  el_transform_dic
-0000f780: 743d 7365 6c66 2e74 7265 6e64 5f74 7261  t=self.trend_tra
-0000f790: 6e73 666f 726d 6174 696f 6e2c 0d0a 2020  nsformation,..  
-0000f7a0: 2020 2020 2020 2020 2020 2020 2020 6466                df
-0000f7b0: 5f74 7261 696e 3d64 665f 7472 6169 6e2c  _train=df_train,
-0000f7c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f7d0: 2020 666f 7265 6361 7374 5f6c 656e 6774    forecast_lengt
-0000f7e0: 683d 666f 7265 6361 7374 5f6c 656e 6774  h=forecast_lengt
-0000f7f0: 682c 0d0a 2020 2020 2020 2020 2020 2020  h,..            
-0000f800: 2020 2020 6672 6571 7565 6e63 793d 7365      frequency=se
-0000f810: 6c66 2e66 7265 7175 656e 6379 2c0d 0a20  lf.frequency,.. 
-0000f820: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000f830: 7265 6469 6374 696f 6e5f 696e 7465 7276  rediction_interv
-0000f840: 616c 3d73 656c 662e 7072 6564 6963 7469  al=self.predicti
-0000f850: 6f6e 5f69 6e74 6572 7661 6c2c 0d0a 2020  on_interval,..  
-0000f860: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000f870: 6e6f 5f6e 6567 6174 6976 6573 3d6e 6f5f  no_negatives=no_
-0000f880: 6e65 6761 7469 7665 732c 0d0a 2020 2020  negatives,..    
-0000f890: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-0000f8a0: 6e73 7472 6169 6e74 3d63 6f6e 7374 7261  nstraint=constra
-0000f8b0: 696e 742c 0d0a 2020 2020 2020 2020 2020  int,..          
-0000f8c0: 2020 2020 2020 6675 7475 7265 5f72 6567        future_reg
-0000f8d0: 7265 7373 6f72 5f74 7261 696e 3d63 6f6d  ressor_train=com
-0000f8e0: 705f 7265 6772 5f74 7261 696e 2c0d 0a20  p_regr_train,.. 
-0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000f900: 7574 7572 655f 7265 6772 6573 736f 725f  uture_regressor_
-0000f910: 666f 7265 6361 7374 3d63 6f6d 705f 7265  forecast=comp_re
-0000f920: 6772 2c0d 0a20 2020 2020 2020 2020 2020  gr,..           
-0000f930: 2020 2020 2023 2068 6f6c 6964 6179 5f63       # holiday_c
-0000f940: 6f75 6e74 7279 3d68 6f6c 6964 6179 5f63  ountry=holiday_c
-0000f950: 6f75 6e74 7279 2c0d 0a20 2020 2020 2020  ountry,..       
-0000f960: 2020 2020 2020 2020 2066 6169 6c5f 6f6e           fail_on
-0000f970: 5f66 6f72 6563 6173 745f 6e61 6e3d 5472  _forecast_nan=Tr
-0000f980: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-0000f990: 2020 2020 2072 616e 646f 6d5f 7365 6564       random_seed
-0000f9a0: 3d73 656c 662e 7261 6e64 6f6d 5f73 6565  =self.random_see
-0000f9b0: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-0000f9c0: 2020 2020 7665 7262 6f73 653d 7365 6c66      verbose=self
-0000f9d0: 2e76 6572 626f 7365 2c0d 0a20 2020 2020  .verbose,..     
-0000f9e0: 2020 2020 2020 2020 2020 206e 5f6a 6f62             n_job
-0000f9f0: 733d 7365 6c66 2e6e 5f6a 6f62 732c 0d0a  s=self.n_jobs,..
-0000fa00: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-0000fa10: 2020 2020 2020 2020 2020 2023 2070 6869             # phi
-0000fa20: 2069 7320 6f6e 2066 7574 7572 6520 7072   is on future pr
-0000fa30: 6564 6963 7420 7374 6570 206f 6e6c 790d  edict step only.
-0000fa40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000fa50: 7365 6c66 2e74 7265 6e64 5f70 6869 2069  self.trend_phi i
-0000fa60: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
-0000fa70: 656c 662e 7472 656e 645f 7068 6920 213d  elf.trend_phi !=
-0000fa80: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
-0000fa90: 2020 2020 2074 656d 7020 3d20 7472 656e       temp = tren
-0000faa0: 645f 666f 7265 6361 7374 2e66 6f72 6563  d_forecast.forec
-0000fab0: 6173 742e 6d75 6c28 0d0a 2020 2020 2020  ast.mul(..      
-0000fac0: 2020 2020 2020 2020 2020 2020 2020 7064                pd
-0000fad0: 2e53 6572 6965 7328 0d0a 2020 2020 2020  .Series(..      
-0000fae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000faf0: 2020 5b73 656c 662e 7472 656e 645f 7068    [self.trend_ph
-0000fb00: 695d 202a 2074 7265 6e64 5f66 6f72 6563  i] * trend_forec
-0000fb10: 6173 742e 666f 7265 6361 7374 2e73 6861  ast.forecast.sha
-0000fb20: 7065 5b30 5d2c 0d0a 2020 2020 2020 2020  pe[0],..        
-0000fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb40: 696e 6465 783d 7472 656e 645f 666f 7265  index=trend_fore
-0000fb50: 6361 7374 2e66 6f72 6563 6173 742e 696e  cast.forecast.in
-0000fb60: 6465 782c 0d0a 2020 2020 2020 2020 2020  dex,..          
-0000fb70: 2020 2020 2020 2020 2020 292e 706f 7728            ).pow(
-0000fb80: 7261 6e67 6528 7472 656e 645f 666f 7265  range(trend_fore
-0000fb90: 6361 7374 2e66 6f72 6563 6173 742e 7368  cast.forecast.sh
-0000fba0: 6170 655b 305d 2929 2c0d 0a20 2020 2020  ape[0])),..     
-0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000fbc0: 7869 733d 302c 0d0a 2020 2020 2020 2020  xis=0,..        
-0000fbd0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0000fbe0: 2020 2020 2020 2020 2020 2023 206f 7665             # ove
-0000fbf0: 7277 7269 7465 2062 6f75 6e64 7320 6966  rwrite bounds if
-0000fc00: 2075 7369 6e67 2070 6869 0d0a 2020 2020   using phi..    
-0000fc10: 2020 2020 2020 2020 2020 2020 7472 656e              tren
-0000fc20: 645f 666f 7265 6361 7374 2e66 6f72 6563  d_forecast.forec
-0000fc30: 6173 7420 3d20 7472 656e 645f 666f 7265  ast = trend_fore
-0000fc40: 6361 7374 2e66 6f72 6563 6173 7420 2b20  cast.forecast + 
-0000fc50: 7465 6d70 0d0a 2020 2020 2020 2020 2020  temp..          
-0000fc60: 2020 2020 2020 7472 656e 645f 666f 7265        trend_fore
-0000fc70: 6361 7374 2e75 7070 6572 5f66 6f72 6563  cast.upper_forec
-0000fc80: 6173 7420 3d20 7472 656e 645f 666f 7265  ast = trend_fore
-0000fc90: 6361 7374 2e66 6f72 6563 6173 740d 0a20  cast.forecast.. 
-0000fca0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000fcb0: 7265 6e64 5f66 6f72 6563 6173 742e 6c6f  rend_forecast.lo
-0000fcc0: 7765 725f 666f 7265 6361 7374 203d 2074  wer_forecast = t
-0000fcd0: 7265 6e64 5f66 6f72 6563 6173 742e 666f  rend_forecast.fo
-0000fce0: 7265 6361 7374 0d0a 2020 2020 2020 2020  recast..        
-0000fcf0: 2020 2020 6966 2069 6e63 6c75 6465 5f68      if include_h
-0000fd00: 6973 746f 7279 3a0d 0a20 2020 2020 2020  istory:..       
-0000fd10: 2020 2020 2020 2020 2074 7265 6e64 5f66           trend_f
-0000fd20: 6f72 6563 6173 742e 666f 7265 6361 7374  orecast.forecast
-0000fd30: 203d 2070 642e 636f 6e63 6174 280d 0a20   = pd.concat(.. 
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd50: 2020 205b 0d0a 2020 2020 2020 2020 2020     [..          
-0000fd60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fd70: 6c66 2e74 7265 6e64 5f74 7261 696e 2069  lf.trend_train i
-0000fd80: 6620 7265 7369 6420 6973 204e 6f6e 6520  f resid is None 
-0000fd90: 656c 7365 2072 6573 6964 2c0d 0a20 2020  else resid,..   
-0000fda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdb0: 2020 2020 2074 7265 6e64 5f66 6f72 6563       trend_forec
-0000fdc0: 6173 742e 666f 7265 6361 7374 2c0d 0a20  ast.forecast,.. 
-0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fde0: 2020 205d 0d0a 2020 2020 2020 2020 2020     ]..          
-0000fdf0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0000fe00: 2020 2020 2020 2020 2074 7265 6e64 5f66           trend_f
-0000fe10: 6f72 6563 6173 742e 6c6f 7765 725f 666f  orecast.lower_fo
-0000fe20: 7265 6361 7374 203d 2070 642e 636f 6e63  recast = pd.conc
-0000fe30: 6174 280d 0a20 2020 2020 2020 2020 2020  at(..           
-0000fe40: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
-0000fe50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe60: 2020 2020 7365 6c66 2e74 7265 6e64 5f74      self.trend_t
-0000fe70: 7261 696e 2069 6620 7265 7369 6420 6973  rain if resid is
-0000fe80: 204e 6f6e 6520 656c 7365 2072 6573 6964   None else resid
-0000fe90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000fea0: 2020 2020 2020 2020 2020 2074 7265 6e64             trend
-0000feb0: 5f66 6f72 6563 6173 742e 6c6f 7765 725f  _forecast.lower_
-0000fec0: 666f 7265 6361 7374 2c0d 0a20 2020 2020  forecast,..     
-0000fed0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-0000fee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fef0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-0000ff00: 2020 2020 2074 7265 6e64 5f66 6f72 6563       trend_forec
-0000ff10: 6173 742e 7570 7065 725f 666f 7265 6361  ast.upper_foreca
-0000ff20: 7374 203d 2070 642e 636f 6e63 6174 280d  st = pd.concat(.
-0000ff30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ff40: 2020 2020 205b 0d0a 2020 2020 2020 2020       [..        
-0000ff50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff60: 7365 6c66 2e74 7265 6e64 5f74 7261 696e  self.trend_train
-0000ff70: 2069 6620 7265 7369 6420 6973 204e 6f6e   if resid is Non
-0000ff80: 6520 656c 7365 2072 6573 6964 2c0d 0a20  e else resid,.. 
-0000ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffa0: 2020 2020 2020 2074 7265 6e64 5f66 6f72         trend_for
-0000ffb0: 6563 6173 742e 7570 7065 725f 666f 7265  ecast.upper_fore
-0000ffc0: 6361 7374 2c0d 0a20 2020 2020 2020 2020  cast,..         
-0000ffd0: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
-0000ffe0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-0000fff0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00010000: 2020 2020 2020 2020 2020 2020 7472 656e              tren
-00010010: 645f 666f 7265 6361 7374 203d 2050 7265  d_forecast = Pre
-00010020: 6469 6374 696f 6e4f 626a 6563 7428 0d0a  dictionObject(..
-00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010040: 666f 7265 6361 7374 3d73 656c 662e 7472  forecast=self.tr
-00010050: 656e 645f 7472 6169 6e2c 0d0a 2020 2020  end_train,..    
-00010060: 2020 2020 2020 2020 2020 2020 6c6f 7765              lowe
-00010070: 725f 666f 7265 6361 7374 3d73 656c 662e  r_forecast=self.
-00010080: 7472 656e 645f 7472 6169 6e2c 0d0a 2020  trend_train,..  
-00010090: 2020 2020 2020 2020 2020 2020 2020 7570                up
-000100a0: 7065 725f 666f 7265 6361 7374 3d73 656c  per_forecast=sel
-000100b0: 662e 7472 656e 645f 7472 6169 6e2c 0d0a  f.trend_train,..
-000100c0: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
-000100d0: 0a20 2020 2020 2020 2023 2061 725f 6c61  .        # ar_la
-000100e0: 6773 2c20 6d75 6c74 6976 6172 6961 7465  gs, multivariate
-000100f0: 2066 6561 7475 7265 7320 7265 7175 6972   features requir
-00010100: 6520 3120 7374 6570 206c 6f6f 700d 0a20  e 1 step loop.. 
-00010110: 2020 2020 2020 2069 6620 666f 7265 6361         if foreca
-00010120: 7374 5f6c 656e 6774 6820 6973 204e 6f6e  st_length is Non
-00010130: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00010140: 6466 5f66 6f72 6563 6173 7420 3d20 7365  df_forecast = se
-00010150: 6c66 2e5f 7072 6564 6963 745f 7374 6570  lf._predict_step
-00010160: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00010170: 2020 2064 6174 6573 3d64 662e 696e 6465     dates=df.inde
-00010180: 782c 0d0a 2020 2020 2020 2020 2020 2020  x,..            
-00010190: 2020 2020 7472 656e 645f 636f 6d70 6f6e      trend_compon
-000101a0: 656e 743d 7472 656e 645f 666f 7265 6361  ent=trend_foreca
-000101b0: 7374 2c0d 0a20 2020 2020 2020 2020 2020  st,..           
-000101c0: 2020 2020 2068 6973 746f 7279 5f64 663d       history_df=
-000101d0: 6466 2c0d 0a20 2020 2020 2020 2020 2020  df,..           
-000101e0: 2020 2020 2066 7574 7572 655f 7265 6772       future_regr
-000101f0: 6573 736f 723d 6675 6c6c 5f72 6567 722c  essor=full_regr,
-00010200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010210: 2020 666c 6167 5f72 6567 7265 7373 6f72    flag_regressor
-00010220: 733d 616c 6c5f 666c 6167 732c 0d0a 2020  s=all_flags,..  
-00010230: 2020 2020 2020 2020 2020 2020 2020 696d                im
-00010240: 7061 6374 733d 696d 7061 6374 732c 0d0a  pacts=impacts,..
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 7265 6772 6573 736f 725f 7065 725f 7365  regressor_per_se
-00010270: 7269 6573 3d72 6567 725f 7073 5f66 6f72  ries=regr_ps_for
-00010280: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00010290: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-000102a0: 7365 6c66 2e70 7265 6469 6374 5f6c 6f6f  self.predict_loo
-000102b0: 705f 7265 713a 0d0a 2020 2020 2020 2020  p_req:..        
-000102c0: 2020 2020 666f 7220 7374 6570 2069 6e20      for step in 
-000102d0: 7261 6e67 6528 666f 7265 6361 7374 5f6c  range(forecast_l
-000102e0: 656e 6774 6829 3a0d 0a20 2020 2020 2020  ength):..       
-000102f0: 2020 2020 2020 2020 2066 6f72 6563 6173           forecas
-00010300: 745f 696e 6465 7820 3d20 6466 2e69 6e64  t_index = df.ind
-00010310: 6578 2e75 6e69 6f6e 280d 0a20 2020 2020  ex.union(..     
-00010320: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010330: 656c 662e 6372 6561 7465 5f66 6f72 6563  elf.create_forec
-00010340: 6173 745f 696e 6465 7828 312c 206c 6173  ast_index(1, las
-00010350: 745f 6461 7465 3d64 662e 696e 6465 785b  t_date=df.index[
-00010360: 2d31 5d29 0d0a 2020 2020 2020 2020 2020  -1])..          
-00010370: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00010380: 2020 2020 2020 2020 2064 665f 666f 7265           df_fore
-00010390: 6361 7374 203d 2073 656c 662e 5f70 7265  cast = self._pre
-000103a0: 6469 6374 5f73 7465 7028 0d0a 2020 2020  dict_step(..    
-000103b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103c0: 6461 7465 733d 666f 7265 6361 7374 5f69  dates=forecast_i
-000103d0: 6e64 6578 2c0d 0a20 2020 2020 2020 2020  ndex,..         
-000103e0: 2020 2020 2020 2020 2020 2074 7265 6e64             trend
-000103f0: 5f63 6f6d 706f 6e65 6e74 3d74 7265 6e64  _component=trend
-00010400: 5f66 6f72 6563 6173 742c 0d0a 2020 2020  _forecast,..    
-00010410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010420: 6869 7374 6f72 795f 6466 3d64 662c 0d0a  history_df=df,..
-00010430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010440: 2020 2020 6675 7475 7265 5f72 6567 7265      future_regre
-00010450: 7373 6f72 3d66 756c 6c5f 7265 6772 2c0d  ssor=full_regr,.
-00010460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010470: 2020 2020 2066 6c61 675f 7265 6772 6573       flag_regres
-00010480: 736f 7273 3d61 6c6c 5f66 6c61 6773 2c0d  sors=all_flags,.
-00010490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000104a0: 2020 2020 2069 6d70 6163 7473 3d69 6d70       impacts=imp
-000104b0: 6163 7473 2c0d 0a20 2020 2020 2020 2020  acts,..         
-000104c0: 2020 2020 2020 2020 2020 2072 6567 7265             regre
-000104d0: 7373 6f72 5f70 6572 5f73 6572 6965 733d  ssor_per_series=
-000104e0: 7265 6772 5f70 735f 666f 7265 2c0d 0a20  regr_ps_fore,.. 
-000104f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00010500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010510: 2020 6466 203d 2070 642e 636f 6e63 6174    df = pd.concat
-00010520: 285b 6466 2c20 6466 5f66 6f72 6563 6173  ([df, df_forecas
-00010530: 742e 666f 7265 6361 7374 2e69 6c6f 635b  t.forecast.iloc[
-00010540: 2d31 3a5d 5d29 0d0a 2020 2020 2020 2020  -1:]])..        
-00010550: 2020 2020 6966 206e 6f74 2069 6e63 6c75      if not inclu
-00010560: 6465 5f68 6973 746f 7279 3a0d 0a20 2020  de_history:..   
-00010570: 2020 2020 2020 2020 2020 2020 2064 665f               df_
-00010580: 666f 7265 6361 7374 2e66 6f72 6563 6173  forecast.forecas
-00010590: 7420 3d20 6466 5f66 6f72 6563 6173 742e  t = df_forecast.
-000105a0: 666f 7265 6361 7374 2e74 6169 6c28 666f  forecast.tail(fo
-000105b0: 7265 6361 7374 5f6c 656e 6774 6829 0d0a  recast_length)..
-000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105d0: 6466 5f66 6f72 6563 6173 742e 6c6f 7765  df_forecast.lowe
-000105e0: 725f 666f 7265 6361 7374 203d 2064 665f  r_forecast = df_
-000105f0: 666f 7265 6361 7374 2e6c 6f77 6572 5f66  forecast.lower_f
-00010600: 6f72 6563 6173 742e 7461 696c 280d 0a20  orecast.tail(.. 
-00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010620: 2020 2066 6f72 6563 6173 745f 6c65 6e67     forecast_leng
-00010630: 7468 0d0a 2020 2020 2020 2020 2020 2020  th..            
-00010640: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00010650: 2020 2020 2020 2064 665f 666f 7265 6361         df_foreca
-00010660: 7374 2e75 7070 6572 5f66 6f72 6563 6173  st.upper_forecas
-00010670: 7420 3d20 6466 5f66 6f72 6563 6173 742e  t = df_forecast.
-00010680: 7570 7065 725f 666f 7265 6361 7374 2e74  upper_forecast.t
-00010690: 6169 6c28 0d0a 2020 2020 2020 2020 2020  ail(..          
-000106a0: 2020 2020 2020 2020 2020 666f 7265 6361            foreca
-000106b0: 7374 5f6c 656e 6774 680d 0a20 2020 2020  st_length..     
-000106c0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-000106d0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-000106e0: 2020 2020 2020 2020 2066 6f72 6563 6173           forecas
-000106f0: 745f 696e 6465 7820 3d20 7365 6c66 2e63  t_index = self.c
-00010700: 7265 6174 655f 666f 7265 6361 7374 5f69  reate_forecast_i
-00010710: 6e64 6578 280d 0a20 2020 2020 2020 2020  ndex(..         
-00010720: 2020 2020 2020 2066 6f72 6563 6173 745f         forecast_
-00010730: 6c65 6e67 7468 2c20 6c61 7374 5f64 6174  length, last_dat
-00010740: 653d 6466 2e69 6e64 6578 5b2d 315d 0d0a  e=df.index[-1]..
-00010750: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00010760: 2020 2020 2020 2020 2020 2069 6620 696e             if in
-00010770: 636c 7564 655f 6869 7374 6f72 793a 0d0a  clude_history:..
-00010780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010790: 666f 7265 6361 7374 5f69 6e64 6578 203d  forecast_index =
-000107a0: 2064 662e 696e 6465 782e 756e 696f 6e28   df.index.union(
-000107b0: 666f 7265 6361 7374 5f69 6e64 6578 290d  forecast_index).
-000107c0: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
-000107d0: 666f 7265 6361 7374 203d 2073 656c 662e  forecast = self.
-000107e0: 5f70 7265 6469 6374 5f73 7465 7028 0d0a  _predict_step(..
-000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010800: 6461 7465 733d 666f 7265 6361 7374 5f69  dates=forecast_i
-00010810: 6e64 6578 2c0d 0a20 2020 2020 2020 2020  ndex,..         
-00010820: 2020 2020 2020 2074 7265 6e64 5f63 6f6d         trend_com
-00010830: 706f 6e65 6e74 3d74 7265 6e64 5f66 6f72  ponent=trend_for
-00010840: 6563 6173 742c 0d0a 2020 2020 2020 2020  ecast,..        
-00010850: 2020 2020 2020 2020 6869 7374 6f72 795f          history_
-00010860: 6466 3d64 662c 0d0a 2020 2020 2020 2020  df=df,..        
-00010870: 2020 2020 2020 2020 6675 7475 7265 5f72          future_r
-00010880: 6567 7265 7373 6f72 3d66 756c 6c5f 7265  egressor=full_re
-00010890: 6772 2c0d 0a20 2020 2020 2020 2020 2020  gr,..           
-000108a0: 2020 2020 2066 6c61 675f 7265 6772 6573       flag_regres
-000108b0: 736f 7273 3d61 6c6c 5f66 6c61 6773 2c0d  sors=all_flags,.
-000108c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000108d0: 2069 6d70 6163 7473 3d69 6d70 6163 7473   impacts=impacts
-000108e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000108f0: 2020 2072 6567 7265 7373 6f72 5f70 6572     regressor_per
-00010900: 5f73 6572 6965 733d 7265 6772 5f70 735f  _series=regr_ps_
-00010910: 666f 7265 2c0d 0a20 2020 2020 2020 2020  fore,..         
-00010920: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
-00010930: 2320 7361 7665 2066 7574 7572 6520 696e  # save future in
-00010940: 6465 7820 6265 666f 7265 2069 6e63 6c75  dex before inclu
-00010950: 6465 5f68 6973 746f 7279 2069 7320 6164  de_history is ad
-00010960: 6465 640d 0a20 2020 2020 2020 2069 6620  ded..        if 
-00010970: 6675 7475 7265 5f69 6d70 6163 7473 2069  future_impacts i
-00010980: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2066  s not None and f
-00010990: 6f72 6563 6173 745f 6c65 6e67 7468 2069  orecast_length i
-000109a0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-000109b0: 2020 2020 2020 2020 2066 7574 7572 655f           future_
-000109c0: 696d 7061 6374 7320 3d20 6675 7475 7265  impacts = future
-000109d0: 5f69 6d70 6163 7473 2e72 6569 6e64 6578  _impacts.reindex
-000109e0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-000109f0: 2020 2063 6f6c 756d 6e73 3d64 665f 666f     columns=df_fo
-00010a00: 7265 6361 7374 2e66 6f72 6563 6173 742e  recast.forecast.
-00010a10: 636f 6c75 6d6e 732c 0d0a 2020 2020 2020  columns,..      
-00010a20: 2020 2020 2020 2020 2020 696e 6465 783d            index=
-00010a30: 666f 7265 6361 7374 5f69 6e64 6578 2c0d  forecast_index,.
-00010a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010a50: 2066 696c 6c5f 7661 6c75 653d 302c 0d0a   fill_value=0,..
-00010a60: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00010a70: 2020 2020 2020 2023 2075 6e64 6f20 7072         # undo pr
-00010a80: 6570 726f 6365 7373 696e 6720 616e 6420  eprocessing and 
-00010a90: 7363 616c 696e 670d 0a20 2020 2020 2020  scaling..       
-00010aa0: 2023 2061 6363 6f75 6e74 2066 6f72 2073   # account for s
-00010ab0: 6f6d 6520 7472 616e 7366 6f72 6d65 7273  ome transformers
-00010ac0: 2072 6571 7569 7269 6e67 2064 6966 6665   requiring diffe
-00010ad0: 7265 6e74 206d 6574 686f 6473 206f 6e20  rent methods on 
-00010ae0: 6f72 6967 696e 616c 2064 6174 6120 616e  original data an
-00010af0: 6420 666f 7265 6361 7374 0d0a 2020 2020  d forecast..    
-00010b00: 2020 2020 6966 2066 6f72 6563 6173 745f      if forecast_
-00010b10: 6c65 6e67 7468 2069 7320 4e6f 6e65 3a0d  length is None:.
-00010b20: 0a20 2020 2020 2020 2020 2020 2064 665f  .            df_
-00010b30: 666f 7265 6361 7374 2e66 6f72 6563 6173  forecast.forecas
-00010b40: 7420 3d20 7365 6c66 2e74 6f5f 6f72 6967  t = self.to_orig
-00010b50: 696e 5f73 7061 6365 280d 0a20 2020 2020  in_space(..     
-00010b60: 2020 2020 2020 2020 2020 2064 665f 666f             df_fo
-00010b70: 7265 6361 7374 2e66 6f72 6563 6173 742c  recast.forecast,
-00010b80: 2074 7261 6e73 5f6d 6574 686f 643d 276f   trans_method='o
-00010b90: 7269 6769 6e61 6c27 0d0a 2020 2020 2020  riginal'..      
-00010ba0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00010bb0: 2020 2020 2064 665f 666f 7265 6361 7374       df_forecast
-00010bc0: 2e6c 6f77 6572 5f66 6f72 6563 6173 7420  .lower_forecast 
-00010bd0: 3d20 7365 6c66 2e74 6f5f 6f72 6967 696e  = self.to_origin
-00010be0: 5f73 7061 6365 280d 0a20 2020 2020 2020  _space(..       
-00010bf0: 2020 2020 2020 2020 2064 665f 666f 7265           df_fore
-00010c00: 6361 7374 2e6c 6f77 6572 5f66 6f72 6563  cast.lower_forec
-00010c10: 6173 742c 2074 7261 6e73 5f6d 6574 686f  ast, trans_metho
-00010c20: 643d 276f 7269 6769 6e61 6c27 0d0a 2020  d='original'..  
-00010c30: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00010c40: 2020 2020 2020 2020 2064 665f 666f 7265           df_fore
-00010c50: 6361 7374 2e75 7070 6572 5f66 6f72 6563  cast.upper_forec
-00010c60: 6173 7420 3d20 7365 6c66 2e74 6f5f 6f72  ast = self.to_or
-00010c70: 6967 696e 5f73 7061 6365 280d 0a20 2020  igin_space(..   
-00010c80: 2020 2020 2020 2020 2020 2020 2064 665f               df_
-00010c90: 666f 7265 6361 7374 2e75 7070 6572 5f66  forecast.upper_f
-00010ca0: 6f72 6563 6173 742c 2074 7261 6e73 5f6d  orecast, trans_m
-00010cb0: 6574 686f 643d 276f 7269 6769 6e61 6c27  ethod='original'
-00010cc0: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
-00010cd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010ce0: 662e 7072 6564 6963 7465 645f 7472 656e  f.predicted_tren
-00010cf0: 6420 3d20 7365 6c66 2e74 6f5f 6f72 6967  d = self.to_orig
-00010d00: 696e 5f73 7061 6365 280d 0a20 2020 2020  in_space(..     
-00010d10: 2020 2020 2020 2020 2020 2074 7265 6e64             trend
-00010d20: 5f66 6f72 6563 6173 742e 666f 7265 6361  _forecast.foreca
-00010d30: 7374 2c20 7472 616e 735f 6d65 7468 6f64  st, trans_method
-00010d40: 3d27 6f72 6967 696e 616c 270d 0a20 2020  ='original'..   
-00010d50: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00010d60: 2020 2020 656c 6966 206e 6f74 2069 6e63      elif not inc
-00010d70: 6c75 6465 5f68 6973 746f 7279 3a0d 0a20  lude_history:.. 
-00010d80: 2020 2020 2020 2020 2020 2064 665f 666f             df_fo
-00010d90: 7265 6361 7374 2e66 6f72 6563 6173 7420  recast.forecast 
-00010da0: 3d20 7365 6c66 2e74 6f5f 6f72 6967 696e  = self.to_origin
-00010db0: 5f73 7061 6365 280d 0a20 2020 2020 2020  _space(..       
-00010dc0: 2020 2020 2020 2020 2064 665f 666f 7265           df_fore
-00010dd0: 6361 7374 2e66 6f72 6563 6173 742c 2074  cast.forecast, t
-00010de0: 7261 6e73 5f6d 6574 686f 643d 2766 6f72  rans_method='for
-00010df0: 6563 6173 7427 0d0a 2020 2020 2020 2020  ecast'..        
-00010e00: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00010e10: 2020 2064 665f 666f 7265 6361 7374 2e6c     df_forecast.l
-00010e20: 6f77 6572 5f66 6f72 6563 6173 7420 3d20  ower_forecast = 
-00010e30: 7365 6c66 2e74 6f5f 6f72 6967 696e 5f73  self.to_origin_s
-00010e40: 7061 6365 280d 0a20 2020 2020 2020 2020  pace(..         
-00010e50: 2020 2020 2020 2064 665f 666f 7265 6361         df_foreca
-00010e60: 7374 2e6c 6f77 6572 5f66 6f72 6563 6173  st.lower_forecas
-00010e70: 742c 2074 7261 6e73 5f6d 6574 686f 643d  t, trans_method=
-00010e80: 2766 6f72 6563 6173 7427 0d0a 2020 2020  'forecast'..    
-00010e90: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00010ea0: 2020 2020 2020 2064 665f 666f 7265 6361         df_foreca
-00010eb0: 7374 2e75 7070 6572 5f66 6f72 6563 6173  st.upper_forecas
-00010ec0: 7420 3d20 7365 6c66 2e74 6f5f 6f72 6967  t = self.to_orig
-00010ed0: 696e 5f73 7061 6365 280d 0a20 2020 2020  in_space(..     
-00010ee0: 2020 2020 2020 2020 2020 2064 665f 666f             df_fo
-00010ef0: 7265 6361 7374 2e75 7070 6572 5f66 6f72  recast.upper_for
-00010f00: 6563 6173 742c 2074 7261 6e73 5f6d 6574  ecast, trans_met
-00010f10: 686f 643d 2766 6f72 6563 6173 7427 0d0a  hod='forecast'..
-00010f20: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00010f30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010f40: 7072 6564 6963 7465 645f 7472 656e 6420  predicted_trend 
-00010f50: 3d20 7365 6c66 2e74 6f5f 6f72 6967 696e  = self.to_origin
-00010f60: 5f73 7061 6365 280d 0a20 2020 2020 2020  _space(..       
-00010f70: 2020 2020 2020 2020 2074 7265 6e64 5f66           trend_f
-00010f80: 6f72 6563 6173 742e 666f 7265 6361 7374  orecast.forecast
-00010f90: 2c20 7472 616e 735f 6d65 7468 6f64 3d27  , trans_method='
-00010fa0: 666f 7265 6361 7374 270d 0a20 2020 2020  forecast'..     
-00010fb0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00010fc0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00010fd0: 2020 2020 2068 646e 203d 206c 656e 2864       hdn = len(d
-00010fe0: 665f 666f 7265 6361 7374 2e66 6f72 6563  f_forecast.forec
-00010ff0: 6173 7429 202d 2066 6f72 6563 6173 745f  ast) - forecast_
-00011000: 6c65 6e67 7468 0d0a 2020 2020 2020 2020  length..        
-00011010: 2020 2020 6466 5f66 6f72 6563 6173 742e      df_forecast.
-00011020: 666f 7265 6361 7374 203d 2070 642e 636f  forecast = pd.co
-00011030: 6e63 6174 280d 0a20 2020 2020 2020 2020  ncat(..         
-00011040: 2020 2020 2020 205b 0d0a 2020 2020 2020         [..      
-00011050: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011060: 6c66 2e74 6f5f 6f72 6967 696e 5f73 7061  lf.to_origin_spa
-00011070: 6365 280d 0a20 2020 2020 2020 2020 2020  ce(..           
-00011080: 2020 2020 2020 2020 2020 2020 2064 665f               df_
-00011090: 666f 7265 6361 7374 2e66 6f72 6563 6173  forecast.forecas
-000110a0: 742e 6865 6164 2868 646e 292c 2074 7261  t.head(hdn), tra
-000110b0: 6e73 5f6d 6574 686f 643d 276f 7269 6769  ns_method='origi
-000110c0: 6e61 6c27 0d0a 2020 2020 2020 2020 2020  nal'..          
-000110d0: 2020 2020 2020 2020 2020 292c 0d0a 2020            ),..  
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 7365 6c66 2e74 6f5f 6f72 6967 696e    self.to_origin
-00011100: 5f73 7061 6365 280d 0a20 2020 2020 2020  _space(..       
-00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011120: 2064 665f 666f 7265 6361 7374 2e66 6f72   df_forecast.for
-00011130: 6563 6173 742e 7461 696c 2866 6f72 6563  ecast.tail(forec
-00011140: 6173 745f 6c65 6e67 7468 292c 0d0a 2020  ast_length),..  
-00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011160: 2020 2020 2020 7472 616e 735f 6d65 7468        trans_meth
-00011170: 6f64 3d27 666f 7265 6361 7374 272c 0d0a  od='forecast',..
-00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011190: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
-000111a0: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
-000111b0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000111c0: 2020 2020 2020 6466 5f66 6f72 6563 6173        df_forecas
-000111d0: 742e 6c6f 7765 725f 666f 7265 6361 7374  t.lower_forecast
-000111e0: 203d 2070 642e 636f 6e63 6174 280d 0a20   = pd.concat(.. 
-000111f0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00011200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011210: 2020 2020 2020 7365 6c66 2e74 6f5f 6f72        self.to_or
-00011220: 6967 696e 5f73 7061 6365 280d 0a20 2020  igin_space(..   
+0000ef20: 696d 7061 6374 7320 3d20 6675 7475 7265  impacts = future
+0000ef30: 5f69 6d70 6163 7473 0d0a 2020 2020 2020  _impacts..      
+0000ef40: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0000ef50: 2020 2020 2020 2020 2020 2020 2069 6d70               imp
+0000ef60: 6163 7473 203d 2070 642e 636f 6e63 6174  acts = pd.concat
+0000ef70: 285b 7365 6c66 2e70 6173 745f 696d 7061  ([self.past_impa
+0000ef80: 6374 732c 2066 7574 7572 655f 696d 7061  cts, future_impa
+0000ef90: 6374 735d 290d 0a20 2020 2020 2020 2065  cts])..        e
+0000efa0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0000efb0: 2020 696d 7061 6374 7320 3d20 7365 6c66    impacts = self
+0000efc0: 2e70 6173 745f 696d 7061 6374 730d 0a20  .past_impacts.. 
+0000efd0: 2020 2020 2020 2023 2049 2064 6f6e 2774         # I don't
+0000efe0: 2074 6869 6e6b 2074 6865 7265 2069 7320   think there is 
+0000eff0: 6120 6d6f 7265 2065 6666 6963 6965 6e74  a more efficient
+0000f000: 2077 6179 2074 6f20 636f 6d62 696e 6520   way to combine 
+0000f010: 7468 6573 6520 6469 6374 7320 6f66 2064  these dicts of d
+0000f020: 6174 6166 7261 6d65 730d 0a20 2020 2020  ataframes..     
+0000f030: 2020 2069 6620 7265 6772 6573 736f 725f     if regressor_
+0000f040: 7065 725f 7365 7269 6573 2069 7320 6e6f  per_series is no
+0000f050: 7420 4e6f 6e65 2061 6e64 2073 656c 662e  t None and self.
+0000f060: 7265 6772 6573 736f 7273 5f75 7365 643a  regressors_used:
+0000f070: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000f080: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+0000f090: 7265 6772 6573 736f 725f 7065 725f 7365  regressor_per_se
+0000f0a0: 7269 6573 2c20 6469 6374 293a 0d0a 2020  ries, dict):..  
+0000f0b0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000f0c0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+0000f0d0: 7265 6772 6573 736f 725f 7065 725f 7365  regressor_per_se
+0000f0e0: 7269 6573 206d 7573 7420 6265 2064 6963  ries must be dic
+0000f0f0: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
+0000f100: 2072 6567 725f 7073 5f66 6f72 6520 3d20   regr_ps_fore = 
+0000f110: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+0000f120: 666f 7220 6b65 792c 2076 616c 7565 2069  for key, value i
+0000f130: 6e20 7365 6c66 2e72 6567 725f 7065 725f  n self.regr_per_
+0000f140: 7365 7269 6573 5f74 722e 6974 656d 7328  series_tr.items(
+0000f150: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000f160: 2020 2020 6966 206c 656e 2872 6567 7265      if len(regre
+0000f170: 7373 6f72 5f70 6572 5f73 6572 6965 735b  ssor_per_series[
+0000f180: 6b65 795d 2920 3d3d 2065 7870 6563 7465  key]) == expecte
+0000f190: 645f 666f 7265 5f6c 656e 3a0d 0a20 2020  d_fore_len:..   
+0000f1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1b0: 2072 6567 725f 7073 5f66 6f72 655b 6b65   regr_ps_fore[ke
+0000f1c0: 795d 203d 2072 6567 7265 7373 6f72 5f70  y] = regressor_p
+0000f1d0: 6572 5f73 6572 6965 735b 6b65 795d 0d0a  er_series[key]..
+0000f1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1f0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0000f200: 2020 2020 2020 2020 2020 2072 6567 725f             regr_
+0000f210: 7073 5f66 6f72 655b 6b65 795d 203d 2070  ps_fore[key] = p
+0000f220: 642e 636f 6e63 6174 280d 0a20 2020 2020  d.concat(..     
+0000f230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f240: 2020 205b 7365 6c66 2e72 6567 725f 7065     [self.regr_pe
+0000f250: 725f 7365 7269 6573 5f74 725b 6b65 795d  r_series_tr[key]
+0000f260: 2c20 7265 6772 6573 736f 725f 7065 725f  , regressor_per_
+0000f270: 7365 7269 6573 5b6b 6579 5d5d 0d0a 2020  series[key]]..  
+0000f280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f290: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+0000f2a0: 2020 2020 2020 2020 2072 6567 725f 7073           regr_ps
+0000f2b0: 5f66 6f72 655b 6b65 795d 203d 2072 6567  _fore[key] = reg
+0000f2c0: 725f 7073 5f66 6f72 655b 6b65 795d 2e69  r_ps_fore[key].i
+0000f2d0: 6c6f 635b 0d0a 2020 2020 2020 2020 2020  loc[..          
+0000f2e0: 2020 2020 2020 2020 2020 2020 2020 7e72                ~r
+0000f2f0: 6567 725f 7073 5f66 6f72 655b 6b65 795d  egr_ps_fore[key]
+0000f300: 2e69 6e64 6578 2e64 7570 6c69 6361 7465  .index.duplicate
+0000f310: 6428 290d 0a20 2020 2020 2020 2020 2020  d()..           
+0000f320: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
+0000f330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f340: 2e72 6567 725f 7073 203d 2072 6567 725f  .regr_ps = regr_
+0000f350: 7073 5f66 6f72 650d 0a20 2020 2020 2020  ps_fore..       
+0000f360: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0000f370: 2020 2020 7265 6772 5f70 735f 666f 7265      regr_ps_fore
+0000f380: 203d 2073 656c 662e 7265 6772 5f70 6572   = self.regr_per
+0000f390: 5f73 6572 6965 735f 7472 0d0a 2020 2020  _series_tr..    
+0000f3a0: 2020 2020 7265 7475 726e 2072 6567 725f      return regr_
+0000f3b0: 7073 5f66 6f72 652c 2069 6d70 6163 7473  ps_fore, impacts
+0000f3c0: 2c20 6675 6c6c 5f72 6567 722c 2061 6c6c  , full_regr, all
+0000f3d0: 5f66 6c61 6773 0d0a 0d0a 2020 2020 6465  _flags....    de
+0000f3e0: 6620 7072 6564 6963 7428 0d0a 2020 2020  f predict(..    
+0000f3f0: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
+0000f400: 2020 2066 6f72 6563 6173 745f 6c65 6e67     forecast_leng
+0000f410: 7468 3d4e 6f6e 652c 0d0a 2020 2020 2020  th=None,..      
+0000f420: 2020 696e 636c 7564 655f 6869 7374 6f72    include_histor
+0000f430: 793d 4661 6c73 652c 0d0a 2020 2020 2020  y=False,..      
+0000f440: 2020 6675 7475 7265 5f72 6567 7265 7373    future_regress
+0000f450: 6f72 3d4e 6f6e 652c 0d0a 2020 2020 2020  or=None,..      
+0000f460: 2020 7265 6772 6573 736f 725f 7065 725f    regressor_per_
+0000f470: 7365 7269 6573 3d4e 6f6e 652c 0d0a 2020  series=None,..  
+0000f480: 2020 2020 2020 666c 6167 5f72 6567 7265        flag_regre
+0000f490: 7373 6f72 733d 4e6f 6e65 2c0d 0a20 2020  ssors=None,..   
+0000f4a0: 2020 2020 2066 7574 7572 655f 696d 7061       future_impa
+0000f4b0: 6374 733d 4e6f 6e65 2c0d 0a20 2020 2020  cts=None,..     
+0000f4c0: 2020 206e 6577 5f64 663d 4e6f 6e65 2c0d     new_df=None,.
+0000f4d0: 0a20 2020 2020 2020 2072 6567 7265 7373  .        regress
+0000f4e0: 6f72 5f66 6f72 6563 6173 745f 6d6f 6465  or_forecast_mode
+0000f4f0: 6c3d 4e6f 6e65 2c0d 0a20 2020 2020 2020  l=None,..       
+0000f500: 2072 6567 7265 7373 6f72 5f66 6f72 6563   regressor_forec
+0000f510: 6173 745f 6d6f 6465 6c5f 7061 7261 6d73  ast_model_params
+0000f520: 3d4e 6f6e 652c 0d0a 2020 2020 2020 2020  =None,..        
+0000f530: 7265 6772 6573 736f 725f 666f 7265 6361  regressor_foreca
+0000f540: 7374 5f74 7261 6e73 666f 726d 6174 696f  st_transformatio
+0000f550: 6e73 3d4e 6f6e 652c 0d0a 2020 2020 2020  ns=None,..      
+0000f560: 2020 696e 636c 7564 655f 6f72 6761 6e69    include_organi
+0000f570: 633d 4661 6c73 652c 0d0a 2020 2020 2020  c=False,..      
+0000f580: 2020 6466 3d4e 6f6e 652c 2020 2320 746f    df=None,  # to
+0000f590: 2062 6520 636f 6d70 6174 6961 626c 6520   be compatiable 
+0000f5a0: 7769 7468 206f 7468 6572 732c 2069 6465  with others, ide
+0000f5b0: 6e74 6963 616c 2074 6f20 6e65 775f 6466  ntical to new_df
+0000f5c0: 0d0a 2020 2020 2020 2020 7061 7374 5f69  ..        past_i
+0000f5d0: 6d70 6163 7473 3d4e 6f6e 652c 2020 2320  mpacts=None,  # 
+0000f5e0: 6f6e 6c79 2069 6620 6e65 775f 6466 2070  only if new_df p
+0000f5f0: 726f 7669 6465 640d 0a20 2020 2029 3a0d  rovided..    ):.
+0000f600: 0a20 2020 2020 2020 2022 2222 4765 6e65  .        """Gene
+0000f610: 7261 7465 2061 2066 6f72 6563 6173 742e  rate a forecast.
+0000f620: 0d0a 0d0a 2020 2020 2020 2020 6675 7475  ....        futu
+0000f630: 7265 5f72 6567 7265 7373 6f72 2061 6e64  re_regressor and
+0000f640: 2072 6567 7265 7373 6f72 5f70 6572 5f73   regressor_per_s
+0000f650: 6572 6965 7320 7368 6f75 6c64 206f 6e6c  eries should onl
+0000f660: 7920 696e 636c 7564 6520 6e65 7720 6675  y include new fu
+0000f670: 7475 7265 2076 616c 7565 732c 2068 6973  ture values, his
+0000f680: 746f 7279 2069 7320 616c 7265 6164 7920  tory is already 
+0000f690: 7374 6f72 6564 0d0a 2020 2020 2020 2020  stored..        
+0000f6a0: 7468 6579 2073 686f 756c 6420 6d61 7463  they should matc
+0000f6b0: 6820 6f6e 2066 6f72 6563 6173 745f 6c65  h on forecast_le
+0000f6c0: 6e67 7468 2061 6e64 2069 6e64 6578 206f  ngth and index o
+0000f6d0: 6620 666f 7265 6361 7374 730d 0a0d 0a20  f forecasts.... 
+0000f6e0: 2020 2020 2020 2041 7267 733a 0d0a 2020         Args:..  
+0000f6f0: 2020 2020 2020 2020 2020 666f 7265 6361            foreca
+0000f700: 7374 5f6c 656e 6774 6820 2869 6e74 293a  st_length (int):
+0000f710: 2073 7465 7073 2061 6865 6164 2074 6f20   steps ahead to 
+0000f720: 7072 6564 6963 742c 206f 7220 4e6f 6e65  predict, or None
+0000f730: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+0000f740: 636c 7564 655f 6869 7374 6f72 7920 2862  clude_history (b
+0000f750: 6f6f 6c29 3a20 696e 636c 7564 6520 7061  ool): include pa
+0000f760: 7374 2070 7265 6469 6374 696f 6e73 2069  st predictions i
+0000f770: 6620 5472 7565 0d0a 2020 2020 2020 2020  f True..        
+0000f780: 2020 2020 616c 6c20 7468 6520 7361 6d65      all the same
+0000f790: 2072 6567 7265 7373 6f72 2061 7267 7320   regressor args 
+0000f7a0: 6173 202e 6669 742c 2062 7574 2066 7574  as .fit, but fut
+0000f7b0: 7572 6520 666f 7265 6361 7374 2076 6572  ure forecast ver
+0000f7c0: 7369 6f6e 7320 6865 7265 0d0a 2020 2020  sions here..    
+0000f7d0: 2020 2020 2020 2020 6675 7475 7265 5f69          future_i
+0000f7e0: 6d70 6163 7473 2028 7064 2e44 6174 6146  mpacts (pd.DataF
+0000f7f0: 7261 6d65 293a 206c 696b 6520 7061 7374  rame): like past
+0000f800: 2069 6d70 6163 7473 2062 7574 2066 6f72   impacts but for
+0000f810: 2074 6865 2066 6f72 6563 6173 7420 6168   the forecast ah
+0000f820: 6561 640d 0a20 2020 2020 2020 2020 2020  ead..           
+0000f830: 206e 6577 5f64 6620 2870 642e 4461 7461   new_df (pd.Data
+0000f840: 4672 616d 6529 3a20 6f72 2064 662c 2065  Frame): or df, e
+0000f850: 7175 6976 616c 656e 7420 746f 2066 6974  quivalent to fit
+0000f860: 5f64 6174 6120 7570 6461 7465 0d0a 2020  _data update..  
+0000f870: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000f880: 2020 2073 656c 662e 666f 7265 6361 7374     self.forecast
+0000f890: 5f6c 656e 6774 6820 3d20 666f 7265 6361  _length = foreca
+0000f8a0: 7374 5f6c 656e 6774 680d 0a20 2020 2020  st_length..     
+0000f8b0: 2020 2070 7265 6469 6374 5374 6172 7454     predictStartT
+0000f8c0: 696d 6520 3d20 7365 6c66 2e74 696d 6528  ime = self.time(
+0000f8d0: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+0000f8e0: 6c66 2e74 7265 6e64 5f74 7261 696e 2069  lf.trend_train i
+0000f8f0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+0000f900: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0000f910: 4572 726f 7228 2243 6173 7361 6e64 7261  Error("Cassandra
+0000f920: 206d 7573 7420 6669 7273 7420 6265 202e   must first be .
+0000f930: 6669 7428 2920 7375 6363 6573 7366 756c  fit() successful
+0000f940: 6c79 2e22 290d 0a0d 0a20 2020 2020 2020  ly.")....       
+0000f950: 2023 2073 6361 6c65 206e 6577 5f64 6620   # scale new_df 
+0000f960: 6966 2067 6976 656e 0d0a 2020 2020 2020  if given..      
+0000f970: 2020 6966 2064 6620 6973 206e 6f74 204e    if df is not N
+0000f980: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000f990: 2020 6e65 775f 6466 203d 2064 660d 0a20    new_df = df.. 
+0000f9a0: 2020 2020 2020 2069 6620 6e65 775f 6466         if new_df
+0000f9b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+0000f9c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f9d0: 6669 745f 6461 7461 280d 0a20 2020 2020  fit_data(..     
+0000f9e0: 2020 2020 2020 2020 2020 2064 663d 6e65             df=ne
+0000f9f0: 775f 6466 2c0d 0a20 2020 2020 2020 2020  w_df,..         
+0000fa00: 2020 2020 2020 2066 6f72 6563 6173 745f         forecast_
+0000fa10: 6c65 6e67 7468 3d66 6f72 6563 6173 745f  length=forecast_
+0000fa20: 6c65 6e67 7468 2c0d 0a20 2020 2020 2020  length,..       
+0000fa30: 2020 2020 2020 2020 2066 7574 7572 655f           future_
+0000fa40: 7265 6772 6573 736f 723d 6675 7475 7265  regressor=future
+0000fa50: 5f72 6567 7265 7373 6f72 2c0d 0a20 2020  _regressor,..   
+0000fa60: 2020 2020 2020 2020 2020 2020 2072 6567               reg
+0000fa70: 7265 7373 6f72 5f70 6572 5f73 6572 6965  ressor_per_serie
+0000fa80: 733d 7265 6772 6573 736f 725f 7065 725f  s=regressor_per_
+0000fa90: 7365 7269 6573 2c0d 0a20 2020 2020 2020  series,..       
+0000faa0: 2020 2020 2020 2020 2066 6c61 675f 7265           flag_re
+0000fab0: 6772 6573 736f 7273 3d66 6c61 675f 7265  gressors=flag_re
+0000fac0: 6772 6573 736f 7273 2c0d 0a20 2020 2020  gressors,..     
+0000fad0: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+0000fae0: 655f 696d 7061 6374 733d 6675 7475 7265  e_impacts=future
+0000faf0: 5f69 6d70 6163 7473 2c0d 0a20 2020 2020  _impacts,..     
+0000fb00: 2020 2020 2020 2020 2020 2072 6567 7265             regre
+0000fb10: 7373 6f72 5f66 6f72 6563 6173 745f 6d6f  ssor_forecast_mo
+0000fb20: 6465 6c3d 7265 6772 6573 736f 725f 666f  del=regressor_fo
+0000fb30: 7265 6361 7374 5f6d 6f64 656c 2c0d 0a20  recast_model,.. 
+0000fb40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000fb50: 6567 7265 7373 6f72 5f66 6f72 6563 6173  egressor_forecas
+0000fb60: 745f 6d6f 6465 6c5f 7061 7261 6d73 3d72  t_model_params=r
+0000fb70: 6567 7265 7373 6f72 5f66 6f72 6563 6173  egressor_forecas
+0000fb80: 745f 6d6f 6465 6c5f 7061 7261 6d73 2c0d  t_model_params,.
+0000fb90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fba0: 2072 6567 7265 7373 6f72 5f66 6f72 6563   regressor_forec
+0000fbb0: 6173 745f 7472 616e 7366 6f72 6d61 7469  ast_transformati
+0000fbc0: 6f6e 733d 7265 6772 6573 736f 725f 666f  ons=regressor_fo
+0000fbd0: 7265 6361 7374 5f74 7261 6e73 666f 726d  recast_transform
+0000fbe0: 6174 696f 6e73 2c0d 0a20 2020 2020 2020  ations,..       
+0000fbf0: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
+0000fc00: 5f68 6973 746f 7279 3d69 6e63 6c75 6465  _history=include
+0000fc10: 5f68 6973 746f 7279 2c0d 0a20 2020 2020  _history,..     
+0000fc20: 2020 2020 2020 2020 2020 2070 6173 745f             past_
+0000fc30: 696d 7061 6374 733d 7061 7374 5f69 6d70  impacts=past_imp
+0000fc40: 6163 7473 2c0d 0a20 2020 2020 2020 2020  acts,..         
+0000fc50: 2020 2029 0d0a 2020 2020 2020 2020 656c     )..        el
+0000fc60: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000fc70: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+0000fc80: 2020 2020 7365 6c66 2e72 6567 725f 7073      self.regr_ps
+0000fc90: 5f66 6f72 652c 0d0a 2020 2020 2020 2020  _fore,..        
+0000fca0: 2020 2020 2020 2020 7365 6c66 2e75 7365          self.use
+0000fcb0: 5f69 6d70 6163 7473 2c0d 0a20 2020 2020  _impacts,..     
+0000fcc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fcd0: 6675 6c6c 5f72 6567 722c 0d0a 2020 2020  full_regr,..    
+0000fce0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fcf0: 2e61 6c6c 5f66 6c61 6773 2c0d 0a20 2020  .all_flags,..   
+0000fd00: 2020 2020 2020 2020 2029 203d 2073 656c           ) = sel
+0000fd10: 662e 5f70 726f 6365 7373 5f72 6567 7265  f._process_regre
+0000fd20: 7373 6f72 7328 0d0a 2020 2020 2020 2020  ssors(..        
+0000fd30: 2020 2020 2020 2020 6466 3d73 656c 662e          df=self.
+0000fd40: 6466 2c0d 0a20 2020 2020 2020 2020 2020  df,..           
+0000fd50: 2020 2020 2066 6f72 6563 6173 745f 6c65       forecast_le
+0000fd60: 6e67 7468 3d66 6f72 6563 6173 745f 6c65  ngth=forecast_le
+0000fd70: 6e67 7468 2c0d 0a20 2020 2020 2020 2020  ngth,..         
+0000fd80: 2020 2020 2020 2066 7574 7572 655f 7265         future_re
+0000fd90: 6772 6573 736f 723d 6675 7475 7265 5f72  gressor=future_r
+0000fda0: 6567 7265 7373 6f72 2c0d 0a20 2020 2020  egressor,..     
+0000fdb0: 2020 2020 2020 2020 2020 2072 6567 7265             regre
+0000fdc0: 7373 6f72 5f70 6572 5f73 6572 6965 733d  ssor_per_series=
+0000fdd0: 7265 6772 6573 736f 725f 7065 725f 7365  regressor_per_se
+0000fde0: 7269 6573 2c0d 0a20 2020 2020 2020 2020  ries,..         
+0000fdf0: 2020 2020 2020 2066 6c61 675f 7265 6772         flag_regr
+0000fe00: 6573 736f 7273 3d66 6c61 675f 7265 6772  essors=flag_regr
+0000fe10: 6573 736f 7273 2c0d 0a20 2020 2020 2020  essors,..       
+0000fe20: 2020 2020 2020 2020 2066 7574 7572 655f           future_
+0000fe30: 696d 7061 6374 733d 6675 7475 7265 5f69  impacts=future_i
+0000fe40: 6d70 6163 7473 2c0d 0a20 2020 2020 2020  mpacts,..       
+0000fe50: 2020 2020 2020 2020 2072 6567 7265 7373           regress
+0000fe60: 6f72 5f66 6f72 6563 6173 745f 6d6f 6465  or_forecast_mode
+0000fe70: 6c3d 7265 6772 6573 736f 725f 666f 7265  l=regressor_fore
+0000fe80: 6361 7374 5f6d 6f64 656c 2c0d 0a20 2020  cast_model,..   
+0000fe90: 2020 2020 2020 2020 2020 2020 2072 6567               reg
+0000fea0: 7265 7373 6f72 5f66 6f72 6563 6173 745f  ressor_forecast_
+0000feb0: 6d6f 6465 6c5f 7061 7261 6d73 3d72 6567  model_params=reg
+0000fec0: 7265 7373 6f72 5f66 6f72 6563 6173 745f  ressor_forecast_
+0000fed0: 6d6f 6465 6c5f 7061 7261 6d73 2c0d 0a20  model_params,.. 
+0000fee0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000fef0: 6567 7265 7373 6f72 5f66 6f72 6563 6173  egressor_forecas
+0000ff00: 745f 7472 616e 7366 6f72 6d61 7469 6f6e  t_transformation
+0000ff10: 733d 7265 6772 6573 736f 725f 666f 7265  s=regressor_fore
+0000ff20: 6361 7374 5f74 7261 6e73 666f 726d 6174  cast_transformat
+0000ff30: 696f 6e73 2c0d 0a20 2020 2020 2020 2020  ions,..         
+0000ff40: 2020 2020 2020 2069 6e63 6c75 6465 5f68         include_h
+0000ff50: 6973 746f 7279 3d69 6e63 6c75 6465 5f68  istory=include_h
+0000ff60: 6973 746f 7279 2c0d 0a20 2020 2020 2020  istory,..       
+0000ff70: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+0000ff80: 6466 203d 2073 656c 662e 6466 2e63 6f70  df = self.df.cop
+0000ff90: 7928 290d 0a0d 0a20 2020 2020 2020 2023  y()....        #
+0000ffa0: 2067 656e 6572 6174 6520 7472 656e 640d   generate trend.
+0000ffb0: 0a20 2020 2020 2020 2023 204d 4159 2057  .        # MAY W
+0000ffc0: 414e 5420 544f 2050 4153 5320 6675 7475  ANT TO PASS futu
+0000ffd0: 7265 5f72 6567 7265 7373 6f72 2048 4552  re_regressor HER
+0000ffe0: 450d 0a20 2020 2020 2020 2072 6573 6964  E..        resid
+0000fff0: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
+00010000: 2069 6620 666f 7265 6361 7374 5f6c 656e   if forecast_len
+00010010: 6774 6820 6973 206e 6f74 204e 6f6e 653a  gth is not None:
+00010020: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00010030: 6372 6561 7465 206e 6577 2072 6f6c 6c69  create new rolli
+00010040: 6e67 2072 6573 6964 7561 6c20 6966 206e  ng residual if n
+00010050: 6577 2064 6174 6120 7072 6f76 6964 6564  ew data provided
+00010060: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+00010070: 5f74 7261 696e 203d 2073 656c 662e 7472  _train = self.tr
+00010080: 656e 645f 7472 6169 6e0d 0a20 2020 2020  end_train..     
+00010090: 2020 2020 2020 2023 2063 6f6d 6269 6e65         # combine
+000100a0: 2072 6567 7265 7373 6f72 2074 7970 6573   regressor types
+000100b0: 2064 6570 656e 6469 6e67 206f 6e20 7768   depending on wh
+000100c0: 6174 2069 7320 6769 7665 6e0d 0a20 2020  at is given..   
+000100d0: 2020 2020 2020 2020 2069 6620 280d 0a20           if (.. 
+000100e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000100f0: 656c 662e 6675 7475 7265 5f72 6567 7265  elf.future_regre
+00010100: 7373 6f72 5f74 7261 696e 2069 7320 4e6f  ssor_train is No
+00010110: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
+00010120: 2020 2020 616e 6420 7365 6c66 2e66 6c61      and self.fla
+00010130: 675f 7265 6772 6573 736f 725f 7472 6169  g_regressor_trai
+00010140: 6e20 6973 206e 6f74 204e 6f6e 650d 0a20  n is not None.. 
+00010150: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00010160: 6e64 2073 656c 662e 7265 6772 6573 736f  nd self.regresso
+00010170: 7273 5f75 7365 640d 0a20 2020 2020 2020  rs_used..       
+00010180: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
+00010190: 2020 2020 2020 2020 2063 6f6d 705f 7265           comp_re
+000101a0: 6772 5f74 7261 696e 203d 2073 656c 662e  gr_train = self.
+000101b0: 666c 6167 5f72 6567 7265 7373 6f72 5f74  flag_regressor_t
+000101c0: 7261 696e 2e72 6569 6e64 6578 280d 0a20  rain.reindex(.. 
+000101d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101e0: 2020 2069 6e64 6578 3d64 665f 7472 6169     index=df_trai
+000101f0: 6e2e 696e 6465 780d 0a20 2020 2020 2020  n.index..       
+00010200: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00010210: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00010220: 5f72 6567 7220 3d20 7365 6c66 2e61 6c6c  _regr = self.all
+00010230: 5f66 6c61 6773 2e74 6169 6c28 666f 7265  _flags.tail(fore
+00010240: 6361 7374 5f6c 656e 6774 6829 0d0a 2020  cast_length)..  
+00010250: 2020 2020 2020 2020 2020 656c 6966 2028            elif (
+00010260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010270: 2020 7365 6c66 2e66 7574 7572 655f 7265    self.future_re
+00010280: 6772 6573 736f 725f 7472 6169 6e20 6973  gressor_train is
+00010290: 206e 6f74 204e 6f6e 650d 0a20 2020 2020   not None..     
+000102a0: 2020 2020 2020 2020 2020 2061 6e64 2073             and s
+000102b0: 656c 662e 666c 6167 5f72 6567 7265 7373  elf.flag_regress
+000102c0: 6f72 5f74 7261 696e 2069 7320 4e6f 6e65  or_train is None
+000102d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000102e0: 2020 616e 6420 7365 6c66 2e72 6567 7265    and self.regre
+000102f0: 7373 6f72 735f 7573 6564 0d0a 2020 2020  ssors_used..    
+00010300: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
+00010310: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00010320: 5f72 6567 725f 7472 6169 6e20 3d20 7365  _regr_train = se
+00010330: 6c66 2e66 7574 7572 655f 7265 6772 6573  lf.future_regres
+00010340: 736f 725f 7472 6169 6e2e 7265 696e 6465  sor_train.reinde
+00010350: 7828 0d0a 2020 2020 2020 2020 2020 2020  x(..            
+00010360: 2020 2020 2020 2020 696e 6465 783d 6466          index=df
+00010370: 5f74 7261 696e 2e69 6e64 6578 0d0a 2020  _train.index..  
+00010380: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+00010390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000103a0: 2063 6f6d 705f 7265 6772 203d 2073 656c   comp_regr = sel
+000103b0: 662e 6675 6c6c 5f72 6567 722e 7461 696c  f.full_regr.tail
+000103c0: 2866 6f72 6563 6173 745f 6c65 6e67 7468  (forecast_length
+000103d0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+000103e0: 6c69 6620 280d 0a20 2020 2020 2020 2020  lif (..         
+000103f0: 2020 2020 2020 2073 656c 662e 6675 7475         self.futu
+00010400: 7265 5f72 6567 7265 7373 6f72 5f74 7261  re_regressor_tra
+00010410: 696e 2069 7320 6e6f 7420 4e6f 6e65 0d0a  in is not None..
+00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010430: 616e 6420 7365 6c66 2e66 6c61 675f 7265  and self.flag_re
+00010440: 6772 6573 736f 725f 7472 6169 6e20 6973  gressor_train is
+00010450: 206e 6f74 204e 6f6e 650d 0a20 2020 2020   not None..     
+00010460: 2020 2020 2020 2020 2020 2061 6e64 2073             and s
+00010470: 656c 662e 7265 6772 6573 736f 7273 5f75  elf.regressors_u
+00010480: 7365 640d 0a20 2020 2020 2020 2020 2020  sed..           
+00010490: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+000104a0: 2020 2020 2063 6f6d 705f 7265 6772 5f74       comp_regr_t
+000104b0: 7261 696e 203d 2070 642e 636f 6e63 6174  rain = pd.concat
+000104c0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+000104d0: 2020 2020 2020 205b 7365 6c66 2e66 7574         [self.fut
+000104e0: 7572 655f 7265 6772 6573 736f 725f 7472  ure_regressor_tr
+000104f0: 6169 6e2c 2073 656c 662e 666c 6167 5f72  ain, self.flag_r
+00010500: 6567 7265 7373 6f72 5f74 7261 696e 5d2c  egressor_train],
+00010510: 2061 7869 733d 310d 0a20 2020 2020 2020   axis=1..       
+00010520: 2020 2020 2020 2020 2029 2e72 6569 6e64           ).reind
+00010530: 6578 2869 6e64 6578 3d64 665f 7472 6169  ex(index=df_trai
+00010540: 6e2e 696e 6465 7829 0d0a 2020 2020 2020  n.index)..      
+00010550: 2020 2020 2020 2020 2020 636f 6d70 5f72            comp_r
+00010560: 6567 7220 3d20 7064 2e63 6f6e 6361 7428  egr = pd.concat(
+00010570: 5b73 656c 662e 6675 6c6c 5f72 6567 722c  [self.full_regr,
+00010580: 2073 656c 662e 616c 6c5f 666c 6167 735d   self.all_flags]
+00010590: 2c20 6178 6973 3d31 292e 7461 696c 280d  , axis=1).tail(.
+000105a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000105b0: 2020 2020 2066 6f72 6563 6173 745f 6c65       forecast_le
+000105c0: 6e67 7468 0d0a 2020 2020 2020 2020 2020  ngth..          
+000105d0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000105e0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000105f0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00010600: 5f72 6567 725f 7472 6169 6e20 3d20 4e6f  _regr_train = No
+00010610: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
+00010620: 2020 2020 636f 6d70 5f72 6567 7220 3d20      comp_regr = 
+00010630: 4e6f 6e65 0d0a 0d0a 2020 2020 2020 2020  None....        
+00010640: 2020 2020 7472 656e 645f 666f 7265 6361      trend_foreca
+00010650: 7374 203d 206d 6f64 656c 5f66 6f72 6563  st = model_forec
+00010660: 6173 7428 0d0a 2020 2020 2020 2020 2020  ast(..          
+00010670: 2020 2020 2020 6d6f 6465 6c5f 6e61 6d65        model_name
+00010680: 3d73 656c 662e 7472 656e 645f 6d6f 6465  =self.trend_mode
+00010690: 6c5b 274d 6f64 656c 275d 2c0d 0a20 2020  l['Model'],..   
+000106a0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+000106b0: 656c 5f70 6172 616d 5f64 6963 743d 7365  el_param_dict=se
+000106c0: 6c66 2e74 7265 6e64 5f6d 6f64 656c 5b27  lf.trend_model['
+000106d0: 4d6f 6465 6c50 6172 616d 6574 6572 7327  ModelParameters'
+000106e0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+000106f0: 2020 2020 6d6f 6465 6c5f 7472 616e 7366      model_transf
+00010700: 6f72 6d5f 6469 6374 3d73 656c 662e 7472  orm_dict=self.tr
+00010710: 656e 645f 7472 616e 7366 6f72 6d61 7469  end_transformati
+00010720: 6f6e 2c0d 0a20 2020 2020 2020 2020 2020  on,..           
+00010730: 2020 2020 2064 665f 7472 6169 6e3d 6466       df_train=df
+00010740: 5f74 7261 696e 2c0d 0a20 2020 2020 2020  _train,..       
+00010750: 2020 2020 2020 2020 2066 6f72 6563 6173           forecas
+00010760: 745f 6c65 6e67 7468 3d66 6f72 6563 6173  t_length=forecas
+00010770: 745f 6c65 6e67 7468 2c0d 0a20 2020 2020  t_length,..     
+00010780: 2020 2020 2020 2020 2020 2066 7265 7175             frequ
+00010790: 656e 6379 3d73 656c 662e 6672 6571 7565  ency=self.freque
+000107a0: 6e63 792c 0d0a 2020 2020 2020 2020 2020  ncy,..          
+000107b0: 2020 2020 2020 7072 6564 6963 7469 6f6e        prediction
+000107c0: 5f69 6e74 6572 7661 6c3d 7365 6c66 2e70  _interval=self.p
+000107d0: 7265 6469 6374 696f 6e5f 696e 7465 7276  rediction_interv
+000107e0: 616c 2c0d 0a20 2020 2020 2020 2020 2020  al,..           
+000107f0: 2020 2020 2066 7574 7572 655f 7265 6772       future_regr
+00010800: 6573 736f 725f 7472 6169 6e3d 636f 6d70  essor_train=comp
+00010810: 5f72 6567 725f 7472 6169 6e2c 0d0a 2020  _regr_train,..  
+00010820: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+00010830: 7475 7265 5f72 6567 7265 7373 6f72 5f66  ture_regressor_f
+00010840: 6f72 6563 6173 743d 636f 6d70 5f72 6567  orecast=comp_reg
+00010850: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+00010860: 2020 2020 6661 696c 5f6f 6e5f 666f 7265      fail_on_fore
+00010870: 6361 7374 5f6e 616e 3d54 7275 652c 0d0a  cast_nan=True,..
+00010880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010890: 7261 6e64 6f6d 5f73 6565 643d 7365 6c66  random_seed=self
+000108a0: 2e72 616e 646f 6d5f 7365 6564 2c0d 0a20  .random_seed,.. 
+000108b0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+000108c0: 6572 626f 7365 3d73 656c 662e 7665 7262  erbose=self.verb
+000108d0: 6f73 652c 0d0a 2020 2020 2020 2020 2020  ose,..          
+000108e0: 2020 2020 2020 6e5f 6a6f 6273 3d73 656c        n_jobs=sel
+000108f0: 662e 6e5f 6a6f 6273 2c0d 0a20 2020 2020  f.n_jobs,..     
+00010900: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00010910: 2020 2020 2020 2320 7068 6920 6973 206f        # phi is o
+00010920: 6e20 6675 7475 7265 2070 7265 6469 6374  n future predict
+00010930: 2073 7465 7020 6f6e 6c79 0d0a 2020 2020   step only..    
+00010940: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00010950: 7472 656e 645f 7068 6920 6973 206e 6f74  trend_phi is not
+00010960: 204e 6f6e 6520 616e 6420 7365 6c66 2e74   None and self.t
+00010970: 7265 6e64 5f70 6869 2021 3d20 313a 0d0a  rend_phi != 1:..
+00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010990: 7465 6d70 203d 2074 7265 6e64 5f66 6f72  temp = trend_for
+000109a0: 6563 6173 742e 666f 7265 6361 7374 2e6d  ecast.forecast.m
+000109b0: 756c 280d 0a20 2020 2020 2020 2020 2020  ul(..           
+000109c0: 2020 2020 2020 2020 2070 642e 5365 7269           pd.Seri
+000109d0: 6573 280d 0a20 2020 2020 2020 2020 2020  es(..           
+000109e0: 2020 2020 2020 2020 2020 2020 205b 7365               [se
+000109f0: 6c66 2e74 7265 6e64 5f70 6869 5d20 2a20  lf.trend_phi] * 
+00010a00: 7472 656e 645f 666f 7265 6361 7374 2e66  trend_forecast.f
+00010a10: 6f72 6563 6173 742e 7368 6170 655b 305d  orecast.shape[0]
+00010a20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00010a30: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+00010a40: 3d74 7265 6e64 5f66 6f72 6563 6173 742e  =trend_forecast.
+00010a50: 666f 7265 6361 7374 2e69 6e64 6578 2c0d  forecast.index,.
+00010a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010a70: 2020 2020 2029 2e70 6f77 2872 616e 6765       ).pow(range
+00010a80: 2874 7265 6e64 5f66 6f72 6563 6173 742e  (trend_forecast.
+00010a90: 666f 7265 6361 7374 2e73 6861 7065 5b30  forecast.shape[0
+00010aa0: 5d29 292c 0d0a 2020 2020 2020 2020 2020  ])),..          
+00010ab0: 2020 2020 2020 2020 2020 6178 6973 3d30            axis=0
+00010ac0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00010ad0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+00010ae0: 2020 2020 2020 2320 6f76 6572 7772 6974        # overwrit
+00010af0: 6520 626f 756e 6473 2069 6620 7573 696e  e bounds if usin
+00010b00: 6720 7068 690d 0a20 2020 2020 2020 2020  g phi..         
+00010b10: 2020 2020 2020 2074 7265 6e64 5f66 6f72         trend_for
+00010b20: 6563 6173 742e 666f 7265 6361 7374 203d  ecast.forecast =
+00010b30: 2074 7265 6e64 5f66 6f72 6563 6173 742e   trend_forecast.
+00010b40: 666f 7265 6361 7374 202b 2074 656d 700d  forecast + temp.
+00010b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b60: 2074 7265 6e64 5f66 6f72 6563 6173 742e   trend_forecast.
+00010b70: 7570 7065 725f 666f 7265 6361 7374 203d  upper_forecast =
+00010b80: 2074 7265 6e64 5f66 6f72 6563 6173 742e   trend_forecast.
+00010b90: 666f 7265 6361 7374 0d0a 2020 2020 2020  forecast..      
+00010ba0: 2020 2020 2020 2020 2020 7472 656e 645f            trend_
+00010bb0: 666f 7265 6361 7374 2e6c 6f77 6572 5f66  forecast.lower_f
+00010bc0: 6f72 6563 6173 7420 3d20 7472 656e 645f  orecast = trend_
+00010bd0: 666f 7265 6361 7374 2e66 6f72 6563 6173  forecast.forecas
+00010be0: 740d 0a20 2020 2020 2020 2020 2020 2069  t..            i
+00010bf0: 6620 696e 636c 7564 655f 6869 7374 6f72  f include_histor
+00010c00: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00010c10: 2020 2020 7472 656e 645f 666f 7265 6361      trend_foreca
+00010c20: 7374 2e66 6f72 6563 6173 7420 3d20 7064  st.forecast = pd
+00010c30: 2e63 6f6e 6361 7428 0d0a 2020 2020 2020  .concat(..      
+00010c40: 2020 2020 2020 2020 2020 2020 2020 5b0d                [.
+00010c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010c60: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+00010c70: 656e 645f 7472 6169 6e20 6966 2072 6573  end_train if res
+00010c80: 6964 2069 7320 4e6f 6e65 2065 6c73 6520  id is None else 
+00010c90: 7265 7369 642c 0d0a 2020 2020 2020 2020  resid,..        
+00010ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cb0: 7472 656e 645f 666f 7265 6361 7374 2e66  trend_forecast.f
+00010cc0: 6f72 6563 6173 742c 0d0a 2020 2020 2020  orecast,..      
+00010cd0: 2020 2020 2020 2020 2020 2020 2020 5d0d                ].
+00010ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010cf0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00010d00: 2020 2020 7472 656e 645f 666f 7265 6361      trend_foreca
+00010d10: 7374 2e6c 6f77 6572 5f66 6f72 6563 6173  st.lower_forecas
+00010d20: 7420 3d20 7064 2e63 6f6e 6361 7428 0d0a  t = pd.concat(..
+00010d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d40: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
+00010d50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010d60: 656c 662e 7472 656e 645f 7472 6169 6e20  elf.trend_train 
+00010d70: 6966 2072 6573 6964 2069 7320 4e6f 6e65  if resid is None
+00010d80: 2065 6c73 6520 7265 7369 642c 0d0a 2020   else resid,..  
+00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010da0: 2020 2020 2020 7472 656e 645f 666f 7265        trend_fore
+00010db0: 6361 7374 2e6c 6f77 6572 5f66 6f72 6563  cast.lower_forec
+00010dc0: 6173 742c 0d0a 2020 2020 2020 2020 2020  ast,..          
+00010dd0: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
+00010de0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e00: 7472 656e 645f 666f 7265 6361 7374 2e75  trend_forecast.u
+00010e10: 7070 6572 5f66 6f72 6563 6173 7420 3d20  pper_forecast = 
+00010e20: 7064 2e63 6f6e 6361 7428 0d0a 2020 2020  pd.concat(..    
+00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e40: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+00010e50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010e60: 7472 656e 645f 7472 6169 6e20 6966 2072  trend_train if r
+00010e70: 6573 6964 2069 7320 4e6f 6e65 2065 6c73  esid is None els
+00010e80: 6520 7265 7369 642c 0d0a 2020 2020 2020  e resid,..      
+00010e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ea0: 2020 7472 656e 645f 666f 7265 6361 7374    trend_forecast
+00010eb0: 2e75 7070 6572 5f66 6f72 6563 6173 742c  .upper_forecast,
+00010ec0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010ed0: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
+00010ee0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00010ef0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00010f00: 2020 2020 2020 2074 7265 6e64 5f66 6f72         trend_for
+00010f10: 6563 6173 7420 3d20 5072 6564 6963 7469  ecast = Predicti
+00010f20: 6f6e 4f62 6a65 6374 280d 0a20 2020 2020  onObject(..     
+00010f30: 2020 2020 2020 2020 2020 2066 6f72 6563             forec
+00010f40: 6173 743d 7365 6c66 2e74 7265 6e64 5f74  ast=self.trend_t
+00010f50: 7261 696e 2c0d 0a20 2020 2020 2020 2020  rain,..         
+00010f60: 2020 2020 2020 206c 6f77 6572 5f66 6f72         lower_for
+00010f70: 6563 6173 743d 7365 6c66 2e74 7265 6e64  ecast=self.trend
+00010f80: 5f74 7261 696e 2c0d 0a20 2020 2020 2020  _train,..       
+00010f90: 2020 2020 2020 2020 2075 7070 6572 5f66           upper_f
+00010fa0: 6f72 6563 6173 743d 7365 6c66 2e74 7265  orecast=self.tre
+00010fb0: 6e64 5f74 7261 696e 2c0d 0a20 2020 2020  nd_train,..     
+00010fc0: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+00010fd0: 2020 2020 2320 6172 5f6c 6167 732c 206d      # ar_lags, m
+00010fe0: 756c 7469 7661 7269 6174 6520 6665 6174  ultivariate feat
+00010ff0: 7572 6573 2072 6571 7569 7265 2031 2073  ures require 1 s
+00011000: 7465 7020 6c6f 6f70 0d0a 2020 2020 2020  tep loop..      
+00011010: 2020 6966 2066 6f72 6563 6173 745f 6c65    if forecast_le
+00011020: 6e67 7468 2069 7320 4e6f 6e65 3a0d 0a20  ngth is None:.. 
+00011030: 2020 2020 2020 2020 2020 2064 665f 666f             df_fo
+00011040: 7265 6361 7374 203d 2073 656c 662e 5f70  recast = self._p
+00011050: 7265 6469 6374 5f73 7465 7028 0d0a 2020  redict_step(..  
+00011060: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00011070: 7465 733d 6466 2e69 6e64 6578 2c0d 0a20  tes=df.index,.. 
+00011080: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00011090: 7265 6e64 5f63 6f6d 706f 6e65 6e74 3d74  rend_component=t
+000110a0: 7265 6e64 5f66 6f72 6563 6173 742c 0d0a  rend_forecast,..
+000110b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110c0: 6869 7374 6f72 795f 6466 3d64 662c 0d0a  history_df=df,..
+000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110e0: 6675 7475 7265 5f72 6567 7265 7373 6f72  future_regressor
+000110f0: 3d73 656c 662e 6675 6c6c 5f72 6567 722c  =self.full_regr,
+00011100: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011110: 2020 666c 6167 5f72 6567 7265 7373 6f72    flag_regressor
+00011120: 733d 7365 6c66 2e61 6c6c 5f66 6c61 6773  s=self.all_flags
+00011130: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00011140: 2020 2069 6d70 6163 7473 3d73 656c 662e     impacts=self.
+00011150: 7573 655f 696d 7061 6374 732c 0d0a 2020  use_impacts,..  
+00011160: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00011170: 6772 6573 736f 725f 7065 725f 7365 7269  gressor_per_seri
+00011180: 6573 3d73 656c 662e 7265 6772 5f70 735f  es=self.regr_ps_
+00011190: 666f 7265 2c0d 0a20 2020 2020 2020 2020  fore,..         
+000111a0: 2020 2029 0d0a 2020 2020 2020 2020 656c     )..        el
+000111b0: 6966 2073 656c 662e 7072 6564 6963 745f  if self.predict_
+000111c0: 6c6f 6f70 5f72 6571 3a0d 0a20 2020 2020  loop_req:..     
+000111d0: 2020 2020 2020 2066 6f72 2073 7465 7020         for step 
+000111e0: 696e 2072 616e 6765 2866 6f72 6563 6173  in range(forecas
+000111f0: 745f 6c65 6e67 7468 293a 0d0a 2020 2020  t_length):..    
+00011200: 2020 2020 2020 2020 2020 2020 666f 7265              fore
+00011210: 6361 7374 5f69 6e64 6578 203d 2064 662e  cast_index = df.
+00011220: 696e 6465 782e 756e 696f 6e28 0d0a 2020  index.union(..  
 00011230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011240: 2020 2020 2064 665f 666f 7265 6361 7374       df_forecast
-00011250: 2e6c 6f77 6572 5f66 6f72 6563 6173 742e  .lower_forecast.
-00011260: 6865 6164 2868 646e 292c 0d0a 2020 2020  head(hdn),..    
-00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011280: 2020 2020 7472 616e 735f 6d65 7468 6f64      trans_method
-00011290: 3d27 6f72 6967 696e 616c 272c 0d0a 2020  ='original',..  
-000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112b0: 2020 2020 2020 626f 756e 6473 3d54 7275        bounds=Tru
-000112c0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000112d0: 2020 2020 2020 2020 292c 0d0a 2020 2020          ),..    
-000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112f0: 7365 6c66 2e74 6f5f 6f72 6967 696e 5f73  self.to_origin_s
-00011300: 7061 6365 280d 0a20 2020 2020 2020 2020  pace(..         
-00011310: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00011320: 665f 666f 7265 6361 7374 2e6c 6f77 6572  f_forecast.lower
-00011330: 5f66 6f72 6563 6173 742e 7461 696c 2866  _forecast.tail(f
-00011340: 6f72 6563 6173 745f 6c65 6e67 7468 292c  orecast_length),
-00011350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011360: 2020 2020 2020 2020 2020 7472 616e 735f            trans_
-00011370: 6d65 7468 6f64 3d27 666f 7265 6361 7374  method='forecast
-00011380: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00011390: 2020 2020 2020 2020 2020 2020 626f 756e              boun
-000113a0: 6473 3d54 7275 652c 0d0a 2020 2020 2020  ds=True,..      
-000113b0: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-000113c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000113d0: 2020 5d0d 0a20 2020 2020 2020 2020 2020    ]..           
-000113e0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-000113f0: 6466 5f66 6f72 6563 6173 742e 7570 7065  df_forecast.uppe
-00011400: 725f 666f 7265 6361 7374 203d 2070 642e  r_forecast = pd.
-00011410: 636f 6e63 6174 280d 0a20 2020 2020 2020  concat(..       
-00011420: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
-00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011440: 7365 6c66 2e74 6f5f 6f72 6967 696e 5f73  self.to_origin_s
-00011450: 7061 6365 280d 0a20 2020 2020 2020 2020  pace(..         
-00011460: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00011470: 665f 666f 7265 6361 7374 2e75 7070 6572  f_forecast.upper
-00011480: 5f66 6f72 6563 6173 742e 6865 6164 2868  _forecast.head(h
-00011490: 646e 292c 0d0a 2020 2020 2020 2020 2020  dn),..          
-000114a0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000114b0: 616e 735f 6d65 7468 6f64 3d27 6f72 6967  ans_method='orig
-000114c0: 696e 616c 272c 0d0a 2020 2020 2020 2020  inal',..        
-000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114e0: 626f 756e 6473 3d54 7275 652c 0d0a 2020  bounds=True,..  
-000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011500: 2020 292c 0d0a 2020 2020 2020 2020 2020    ),..          
-00011510: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00011520: 6f5f 6f72 6967 696e 5f73 7061 6365 280d  o_origin_space(.
-00011530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011540: 2020 2020 2020 2020 2064 665f 666f 7265           df_fore
-00011550: 6361 7374 2e75 7070 6572 5f66 6f72 6563  cast.upper_forec
-00011560: 6173 742e 7461 696c 2866 6f72 6563 6173  ast.tail(forecas
-00011570: 745f 6c65 6e67 7468 292c 0d0a 2020 2020  t_length),..    
-00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011590: 2020 2020 7472 616e 735f 6d65 7468 6f64      trans_method
-000115a0: 3d27 666f 7265 6361 7374 272c 0d0a 2020  ='forecast',..  
-000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115c0: 2020 2020 2020 626f 756e 6473 3d54 7275        bounds=Tru
-000115d0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000115e0: 2020 2020 2020 2020 292c 0d0a 2020 2020          ),..    
-000115f0: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
-00011600: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-00011610: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00011620: 7265 6469 6374 6564 5f74 7265 6e64 203d  redicted_trend =
-00011630: 2070 642e 636f 6e63 6174 280d 0a20 2020   pd.concat(..   
-00011640: 2020 2020 2020 2020 2020 2020 205b 0d0a               [..
-00011650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011660: 2020 2020 7365 6c66 2e74 6f5f 6f72 6967      self.to_orig
-00011670: 696e 5f73 7061 6365 280d 0a20 2020 2020  in_space(..     
-00011680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011690: 2020 2074 7265 6e64 5f66 6f72 6563 6173     trend_forecas
-000116a0: 742e 666f 7265 6361 7374 2e68 6561 6428  t.forecast.head(
-000116b0: 6864 6e29 2c20 7472 616e 735f 6d65 7468  hdn), trans_meth
-000116c0: 6f64 3d27 6f72 6967 696e 616c 270d 0a20  od='original'.. 
-000116d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116e0: 2020 2029 2c0d 0a20 2020 2020 2020 2020     ),..         
-000116f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011700: 746f 5f6f 7269 6769 6e5f 7370 6163 6528  to_origin_space(
-00011710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011720: 2020 2020 2020 2020 2020 7472 656e 645f            trend_
-00011730: 666f 7265 6361 7374 2e66 6f72 6563 6173  forecast.forecas
-00011740: 742e 7461 696c 2866 6f72 6563 6173 745f  t.tail(forecast_
-00011750: 6c65 6e67 7468 292c 0d0a 2020 2020 2020  length),..      
-00011760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011770: 2020 7472 616e 735f 6d65 7468 6f64 3d27    trans_method='
-00011780: 666f 7265 6361 7374 272c 0d0a 2020 2020  forecast',..    
-00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117a0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000117b0: 2020 2020 5d0d 0a20 2020 2020 2020 2020      ]..         
-000117c0: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
-000117d0: 2320 7570 6461 7465 2074 7265 6e64 2061  # update trend a
-000117e0: 6e61 6c79 7369 7320 6261 7365 6420 6f6e  nalysis based on
-000117f0: 2074 7265 6e64 2066 6f72 6563 6173 7420   trend forecast 
-00011800: 6173 2077 656c 6c0d 0a20 2020 2020 2020  as well..       
-00011810: 2069 6620 666f 7265 6361 7374 5f6c 656e   if forecast_len
-00011820: 6774 6820 6973 206e 6f74 204e 6f6e 6520  gth is not None 
-00011830: 616e 6420 696e 636c 7564 655f 6869 7374  and include_hist
-00011840: 6f72 793a 0d0a 2020 2020 2020 2020 2020  ory:..          
-00011850: 2020 7472 656e 645f 706f 7374 6572 696f    trend_posterio
-00011860: 722c 2073 656c 662e 736c 6f70 652c 2069  r, self.slope, i
-00011870: 6e74 6572 6365 7074 203d 2073 656c 662e  ntercept = self.
-00011880: 726f 6c6c 696e 675f 7472 656e 6428 0d0a  rolling_trend(..
-00011890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118a0: 7365 6c66 2e70 7265 6469 6374 6564 5f74  self.predicted_t
-000118b0: 7265 6e64 2c20 6e70 2e61 7272 6179 2873  rend, np.array(s
-000118c0: 656c 662e 745f 7072 6564 6963 7429 0d0a  elf.t_predict)..
-000118d0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-000118e0: 2020 2020 2020 2020 2020 2028 0d0a 2020             (..  
-000118f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011900: 6c66 2e7a 6572 6f5f 6372 6f73 7369 6e67  lf.zero_crossing
-00011910: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00011920: 2020 2020 7365 6c66 2e63 6861 6e67 6570      self.changep
-00011930: 6f69 6e74 732c 0d0a 2020 2020 2020 2020  oints,..        
-00011940: 2020 2020 2020 2020 7365 6c66 2e73 6c6f          self.slo
-00011950: 7065 5f73 6967 6e2c 0d0a 2020 2020 2020  pe_sign,..      
-00011960: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00011970: 6363 656c 2c0d 0a20 2020 2020 2020 2020  ccel,..         
-00011980: 2020 2029 203d 2073 656c 662e 616e 616c     ) = self.anal
-00011990: 797a 655f 7472 656e 6428 7365 6c66 2e73  yze_trend(self.s
-000119a0: 6c6f 7065 2c20 696e 6465 783d 7365 6c66  lope, index=self
-000119b0: 2e70 7265 6469 6374 6564 5f74 7265 6e64  .predicted_trend
-000119c0: 2e69 6e64 6578 290d 0a0d 0a20 2020 2020  .index)....     
-000119d0: 2020 2023 2064 6f6e 2774 2066 6f72 6765     # don't forge
-000119e0: 7420 746f 2061 6464 2069 6e20 7061 7374  t to add in past
-000119f0: 5f69 6d70 6163 7473 2028 7573 6520 6675  _impacts (use fu
-00011a00: 7475 7265 2069 6d70 6163 7473 2061 6761  ture impacts aga
-00011a10: 696e 3f29 2041 4654 4552 2075 6e73 6361  in?) AFTER unsca
-00011a20: 6c69 6e67 0d0a 2020 2020 2020 2020 6966  ling..        if
-00011a30: 2073 656c 662e 7061 7374 5f69 6d70 6163   self.past_impac
-00011a40: 7473 5f69 6e74 6572 7665 6e74 696f 6e20  ts_intervention 
-00011a50: 213d 2022 7265 6772 6573 736f 7222 3a0d  != "regressor":.
-00011a60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011a70: 6675 7475 7265 5f69 6d70 6163 7473 2069  future_impacts i
-00011a80: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
-00011a90: 656c 662e 7061 7374 5f69 6d70 6163 7473  elf.past_impacts
-00011aa0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00011ab0: 2020 2020 2020 2020 2020 2070 6173 745f             past_
-00011ac0: 696d 7061 6374 7320 3d20 7064 2e44 6174  impacts = pd.Dat
-00011ad0: 6146 7261 6d65 280d 0a20 2020 2020 2020  aFrame(..       
-00011ae0: 2020 2020 2020 2020 2020 2020 2030 2c20               0, 
-00011af0: 696e 6465 783d 7365 6c66 2e64 662e 696e  index=self.df.in
-00011b00: 6465 782c 2063 6f6c 756d 6e73 3d73 656c  dex, columns=sel
-00011b10: 662e 6466 2e63 6f6c 756d 6e73 0d0a 2020  f.df.columns..  
-00011b20: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00011b30: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00011b40: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00011b50: 2020 2020 7061 7374 5f69 6d70 6163 7473      past_impacts
-00011b60: 203d 2073 656c 662e 7061 7374 5f69 6d70   = self.past_imp
-00011b70: 6163 7473 0d0a 2020 2020 2020 2020 2020  acts..          
-00011b80: 2020 2320 726f 6c6c 2066 6f72 7761 7264    # roll forward
-00011b90: 2074 6169 6c20 6f66 2070 6173 7420 696d   tail of past im
-00011ba0: 7061 6374 732c 2061 7373 756d 696e 6720  pacts, assuming 
-00011bb0: 6974 2063 6f6e 7469 6e75 6573 0d0a 2020  it continues..  
-00011bc0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00011bd0: 662e 7061 7374 5f69 6d70 6163 7473 2069  f.past_impacts i
-00011be0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2066  s not None and f
-00011bf0: 6f72 6563 6173 745f 6c65 6e67 7468 2069  orecast_length i
-00011c00: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00011c10: 2020 2020 2020 2020 2020 2020 2066 7574               fut
-00011c20: 7572 655f 696d 7074 7320 3d20 7064 2e44  ure_impts = pd.D
-00011c30: 6174 6146 7261 6d65 280d 0a20 2020 2020  ataFrame(..     
-00011c40: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00011c50: 702e 7265 7065 6174 280d 0a20 2020 2020  p.repeat(..     
-00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c70: 2020 2073 656c 662e 7061 7374 5f69 6d70     self.past_imp
-00011c80: 6163 7473 2e69 6c6f 635b 2d31 3a5d 2e74  acts.iloc[-1:].t
-00011c90: 6f5f 6e75 6d70 7928 292c 2066 6f72 6563  o_numpy(), forec
-00011ca0: 6173 745f 6c65 6e67 7468 2c20 6178 6973  ast_length, axis
-00011cb0: 3d30 0d0a 2020 2020 2020 2020 2020 2020  =0..            
-00011cc0: 2020 2020 2020 2020 292c 0d0a 2020 2020          ),..    
-00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ce0: 696e 6465 783d 6466 5f66 6f72 6563 6173  index=df_forecas
-00011cf0: 742e 666f 7265 6361 7374 2e69 6e64 6578  t.forecast.index
-00011d00: 5b2d 666f 7265 6361 7374 5f6c 656e 6774  [-forecast_lengt
-00011d10: 683a 5d2c 0d0a 2020 2020 2020 2020 2020  h:],..          
-00011d20: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-00011d30: 733d 7365 6c66 2e70 6173 745f 696d 7061  s=self.past_impa
-00011d40: 6374 732e 636f 6c75 6d6e 732c 0d0a 2020  cts.columns,..  
-00011d50: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00011d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011d70: 2069 6620 6675 7475 7265 5f69 6d70 6163   if future_impac
-00011d80: 7473 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ts is not None:.
-00011d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011da0: 2020 2020 2066 7574 7572 655f 696d 7074       future_impt
-00011db0: 7320 3d20 6675 7475 7265 5f69 6d70 7473  s = future_impts
-00011dc0: 202b 2066 7574 7572 655f 696d 7061 6374   + future_impact
-00011dd0: 730d 0a20 2020 2020 2020 2020 2020 2065  s..            e
-00011de0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00011df0: 2020 2020 2020 6675 7475 7265 5f69 6d70        future_imp
-00011e00: 7473 203d 2070 642e 4461 7461 4672 616d  ts = pd.DataFram
-00011e10: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
-00011e20: 2069 6620 7365 6c66 2e70 6173 745f 696d   if self.past_im
-00011e30: 7061 6374 7320 6973 206e 6f74 204e 6f6e  pacts is not Non
-00011e40: 6520 6f72 2066 7574 7572 655f 696d 7061  e or future_impa
-00011e50: 6374 7320 6973 206e 6f74 204e 6f6e 653a  cts is not None:
-00011e60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011e70: 2020 696d 7074 7320 3d20 3120 2b20 280d    impts = 1 + (.
-00011e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011e90: 2020 2020 2070 642e 636f 6e63 6174 280d       pd.concat(.
-00011ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011eb0: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
-00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ed0: 2020 2020 2020 2020 7061 7374 5f69 6d70          past_imp
-00011ee0: 6163 7473 2c0d 0a20 2020 2020 2020 2020  acts,..         
-00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f00: 2020 2066 7574 7572 655f 696d 7074 735b     future_impts[
-00011f10: 7e66 7574 7572 655f 696d 7074 732e 696e  ~future_impts.in
-00011f20: 6465 782e 6973 696e 2870 6173 745f 696d  dex.isin(past_im
-00011f30: 7061 6374 732e 696e 6465 7829 5d2c 0d0a  pacts.index)],..
-00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f50: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-00011f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f70: 2020 2020 6178 6973 3d30 2c0d 0a20 2020      axis=0,..   
-00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f90: 2029 2e72 6569 6e64 6578 280d 0a20 2020   ).reindex(..   
-00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fb0: 2020 2020 2069 6e64 6578 3d64 665f 666f       index=df_fo
-00011fc0: 7265 6361 7374 2e66 6f72 6563 6173 742e  recast.forecast.
-00011fd0: 696e 6465 782c 0d0a 2020 2020 2020 2020  index,..        
-00011fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ff0: 636f 6c75 6d6e 733d 6466 5f66 6f72 6563  columns=df_forec
-00012000: 6173 742e 666f 7265 6361 7374 2e63 6f6c  ast.forecast.col
-00012010: 756d 6e73 2c0d 0a20 2020 2020 2020 2020  umns,..         
-00012020: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012030: 696c 6c5f 7661 6c75 653d 302c 0d0a 2020  ill_value=0,..  
-00012040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012050: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00012060: 2020 2020 2029 2020 2320 6d69 6e75 7320       )  # minus 
-00012070: 6f72 2070 6c75 730d 0a20 2020 2020 2020  or plus..       
-00012080: 2020 2020 2020 2020 2073 656c 662e 696d           self.im
-00012090: 7061 6374 7320 3d20 696d 7074 730d 0a20  pacts = impts.. 
-000120a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000120b0: 6620 696e 636c 7564 655f 6f72 6761 6e69  f include_organi
-000120c0: 633a 0d0a 2020 2020 2020 2020 2020 2020  c:..            
-000120d0: 2020 2020 2020 2020 6466 5f66 6f72 6563          df_forec
-000120e0: 6173 742e 6f72 6761 6e69 635f 666f 7265  ast.organic_fore
-000120f0: 6361 7374 203d 2064 665f 666f 7265 6361  cast = df_foreca
-00012100: 7374 2e66 6f72 6563 6173 742e 636f 7079  st.forecast.copy
-00012110: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00012120: 2020 2020 6466 5f66 6f72 6563 6173 742e      df_forecast.
-00012130: 666f 7265 6361 7374 203d 2064 665f 666f  forecast = df_fo
-00012140: 7265 6361 7374 2e66 6f72 6563 6173 7420  recast.forecast 
-00012150: 2a20 696d 7074 730d 0a20 2020 2020 2020  * impts..       
-00012160: 2020 2020 2020 2020 2064 665f 666f 7265           df_fore
-00012170: 6361 7374 2e6c 6f77 6572 5f66 6f72 6563  cast.lower_forec
-00012180: 6173 7420 3d20 6466 5f66 6f72 6563 6173  ast = df_forecas
-00012190: 742e 6c6f 7765 725f 666f 7265 6361 7374  t.lower_forecast
-000121a0: 202a 2069 6d70 7473 0d0a 2020 2020 2020   * impts..      
-000121b0: 2020 2020 2020 2020 2020 6466 5f66 6f72            df_for
-000121c0: 6563 6173 742e 7570 7065 725f 666f 7265  ecast.upper_fore
-000121d0: 6361 7374 203d 2064 665f 666f 7265 6361  cast = df_foreca
-000121e0: 7374 2e75 7070 6572 5f66 6f72 6563 6173  st.upper_forecas
-000121f0: 7420 2a20 696d 7074 730d 0a0d 0a20 2020  t * impts....   
-00012200: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-00012210: 7374 7261 696e 7420 6973 206e 6f74 204e  straint is not N
-00012220: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00012230: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00012240: 7365 6c66 2e63 6f6e 7374 7261 696e 742c  self.constraint,
-00012250: 2064 6963 7429 3a0d 0a20 2020 2020 2020   dict):..       
-00012260: 2020 2020 2020 2020 2063 6f6e 7374 7261           constra
-00012270: 696e 745f 6d65 7468 6f64 203d 2073 656c  int_method = sel
-00012280: 662e 636f 6e73 7472 6169 6e74 2e67 6574  f.constraint.get
-00012290: 2822 636f 6e73 7472 6169 6e74 5f6d 6574  ("constraint_met
-000122a0: 686f 6422 2c20 2271 7561 6e74 696c 6522  hod", "quantile"
-000122b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000122c0: 2020 2063 6f6e 7374 7261 696e 745f 7265     constraint_re
-000122d0: 6775 6c61 7269 7a61 7469 6f6e 203d 2073  gularization = s
-000122e0: 656c 662e 636f 6e73 7472 6169 6e74 2e67  elf.constraint.g
-000122f0: 6574 280d 0a20 2020 2020 2020 2020 2020  et(..           
-00012300: 2020 2020 2020 2020 2022 636f 6e73 7472           "constr
-00012310: 6169 6e74 5f72 6567 756c 6172 697a 6174  aint_regularizat
-00012320: 696f 6e22 2c20 310d 0a20 2020 2020 2020  ion", 1..       
-00012330: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00012340: 2020 2020 2020 2020 2020 2020 6c6f 7765              lowe
-00012350: 725f 636f 6e73 7472 6169 6e74 203d 2073  r_constraint = s
-00012360: 656c 662e 636f 6e73 7472 6169 6e74 2e67  elf.constraint.g
-00012370: 6574 2822 6c6f 7765 725f 636f 6e73 7472  et("lower_constr
-00012380: 6169 6e74 222c 2030 290d 0a20 2020 2020  aint", 0)..     
-00012390: 2020 2020 2020 2020 2020 2075 7070 6572             upper
-000123a0: 5f63 6f6e 7374 7261 696e 7420 3d20 7365  _constraint = se
-000123b0: 6c66 2e63 6f6e 7374 7261 696e 742e 6765  lf.constraint.ge
-000123c0: 7428 2275 7070 6572 5f63 6f6e 7374 7261  t("upper_constra
-000123d0: 696e 7422 2c20 3129 0d0a 2020 2020 2020  int", 1)..      
-000123e0: 2020 2020 2020 2020 2020 626f 756e 6473            bounds
-000123f0: 203d 2073 656c 662e 636f 6e73 7472 6169   = self.constrai
-00012400: 6e74 2e67 6574 2822 626f 756e 6473 222c  nt.get("bounds",
-00012410: 2046 616c 7365 290d 0a20 2020 2020 2020   False)..       
-00012420: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00012430: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-00012440: 7472 6169 6e74 5f6d 6574 686f 6420 3d20  traint_method = 
-00012450: 2273 7464 6576 5f6d 696e 220d 0a20 2020  "stdev_min"..   
-00012460: 2020 2020 2020 2020 2020 2020 206c 6f77               low
-00012470: 6572 5f63 6f6e 7374 7261 696e 7420 3d20  er_constraint = 
-00012480: 666c 6f61 7428 7365 6c66 2e63 6f6e 7374  float(self.const
-00012490: 7261 696e 7429 0d0a 2020 2020 2020 2020  raint)..        
-000124a0: 2020 2020 2020 2020 7570 7065 725f 636f          upper_co
-000124b0: 6e73 7472 6169 6e74 203d 2066 6c6f 6174  nstraint = float
-000124c0: 2873 656c 662e 636f 6e73 7472 6169 6e74  (self.constraint
-000124d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000124e0: 2020 2063 6f6e 7374 7261 696e 745f 7265     constraint_re
-000124f0: 6775 6c61 7269 7a61 7469 6f6e 203d 2031  gularization = 1
-00012500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012510: 2020 626f 756e 6473 203d 2046 616c 7365    bounds = False
-00012520: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00012530: 2073 656c 662e 7665 7262 6f73 6520 3e3d   self.verbose >=
-00012540: 2033 3a0d 0a20 2020 2020 2020 2020 2020   3:..           
-00012550: 2020 2020 2070 7269 6e74 280d 0a20 2020       print(..   
-00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012570: 2066 2255 7369 6e67 2063 6f6e 7374 7261   f"Using constra
-00012580: 696e 7420 7769 7468 206d 6574 686f 643a  int with method:
-00012590: 207b 636f 6e73 7472 6169 6e74 5f6d 6574   {constraint_met
-000125a0: 686f 647d 2c20 7b63 6f6e 7374 7261 696e  hod}, {constrain
-000125b0: 745f 7265 6775 6c61 7269 7a61 7469 6f6e  t_regularization
-000125c0: 7d2c 207b 6c6f 7765 725f 636f 6e73 7472  }, {lower_constr
-000125d0: 6169 6e74 7d2c 207b 7570 7065 725f 636f  aint}, {upper_co
-000125e0: 6e73 7472 6169 6e74 7d2c 207b 626f 756e  nstraint}, {boun
-000125f0: 6473 7d22 0d0a 2020 2020 2020 2020 2020  ds}"..          
-00012600: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
-00012610: 2020 2020 2020 2064 665f 666f 7265 6361         df_foreca
-00012620: 7374 203d 2064 665f 666f 7265 6361 7374  st = df_forecast
-00012630: 2e61 7070 6c79 5f63 6f6e 7374 7261 696e  .apply_constrain
-00012640: 7473 280d 0a20 2020 2020 2020 2020 2020  ts(..           
-00012650: 2020 2020 2063 6f6e 7374 7261 696e 745f       constraint_
-00012660: 6d65 7468 6f64 2c0d 0a20 2020 2020 2020  method,..       
-00012670: 2020 2020 2020 2020 2063 6f6e 7374 7261           constra
-00012680: 696e 745f 7265 6775 6c61 7269 7a61 7469  int_regularizati
-00012690: 6f6e 2c0d 0a20 2020 2020 2020 2020 2020  on,..           
-000126a0: 2020 2020 2075 7070 6572 5f63 6f6e 7374       upper_const
-000126b0: 7261 696e 742c 0d0a 2020 2020 2020 2020  raint,..        
-000126c0: 2020 2020 2020 2020 6c6f 7765 725f 636f          lower_co
-000126d0: 6e73 7472 6169 6e74 2c0d 0a20 2020 2020  nstraint,..     
-000126e0: 2020 2020 2020 2020 2020 2062 6f75 6e64             bound
-000126f0: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00012700: 2020 2020 7365 6c66 2e64 665f 6f72 6967      self.df_orig
-00012710: 696e 616c 2c0d 0a20 2020 2020 2020 2020  inal,..         
-00012720: 2020 2029 0d0a 2020 2020 2020 2020 2320     )..        # 
-00012730: 5245 5455 524e 2043 4f4d 504f 4e45 4e54  RETURN COMPONENT
-00012740: 5320 286c 6f6e 6720 7374 796c 6529 206f  S (long style) o
-00012750: 7074 696f 6e0d 0a20 2020 2020 2020 2064  ption..        d
-00012760: 665f 666f 7265 6361 7374 2e70 7265 6469  f_forecast.predi
-00012770: 6374 5f72 756e 7469 6d65 203d 2073 656c  ct_runtime = sel
-00012780: 662e 7469 6d65 2829 202d 2070 7265 6469  f.time() - predi
-00012790: 6374 5374 6172 7454 696d 650d 0a20 2020  ctStartTime..   
-000127a0: 2020 2020 2072 6574 7572 6e20 6466 5f66       return df_f
-000127b0: 6f72 6563 6173 740d 0a0d 0a20 2020 2064  orecast....    d
-000127c0: 6566 2061 7574 6f5f 6669 7428 7365 6c66  ef auto_fit(self
-000127d0: 2c20 6466 2c20 7661 6c69 6461 7469 6f6e  , df, validation
-000127e0: 5f6d 6574 686f 6429 3a20 2023 2061 6c73  _method):  # als
-000127f0: 6f20 6164 6420 7265 6772 6573 736f 7220  o add regressor 
-00012800: 696e 7075 740d 0a20 2020 2020 2020 2023  input..        #
-00012810: 206f 7074 696f 6e20 746f 2063 6f6d 706c   option to compl
-00012820: 6574 656c 7920 736b 6970 2073 6f6d 6520  etely skip some 
-00012830: 7468 696e 6773 2028 616e 6f6d 616c 6965  things (anomalie
-00012840: 732c 2068 6f6c 6964 6179 2064 6574 6563  s, holiday detec
-00012850: 746f 722c 2061 7220 6c61 6773 290d 0a20  tor, ar lags).. 
-00012860: 2020 2020 2020 2023 2072 756e 2063 726f         # run cro
-00012870: 7373 2076 616c 6964 6174 696f 6e20 746f  ss validation to
-00012880: 2063 686f 6f73 650d 0a20 2020 2020 2020   choose..       
-00012890: 2023 2072 6574 7572 6e20 6d65 7472 6963   # return metric
-000128a0: 7320 6f66 2062 6573 7420 6d6f 6465 6c2c  s of best model,
-000128b0: 2073 6574 2062 6173 6520 7061 7261 6d73   set base params
-000128c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-000128d0: 7461 7274 696e 675f 7061 7261 6d73 203d  tarting_params =
-000128e0: 2073 656c 662e 6765 745f 7061 7261 6d73   self.get_params
-000128f0: 2829 0d0a 2020 2020 2020 2020 7265 7475  ()..        retu
-00012900: 726e 204e 6f74 496d 706c 656d 656e 7465  rn NotImplemente
-00012910: 640d 0a0d 0a20 2020 2064 6566 206e 6578  d....    def nex
-00012920: 745f 6669 7428 7365 6c66 293a 0d0a 2020  t_fit(self):..  
-00012930: 2020 2020 2020 2320 6f70 7469 6f6e 2074        # option t
-00012940: 6f20 7072 696e 7420 6120 6772 6170 6820  o print a graph 
-00012950: 6f66 2065 6163 6820 7768 696c 6520 676f  of each while go
-00012960: 696e 6720 2872 756e 2061 6761 696e 2075  ing (run again u
-00012970: 6e74 696c 2079 6f75 2073 6565 206f 6e65  ntil you see one
-00012980: 2079 6f75 206c 696b 6529 0d0a 2020 2020   you like)..    
-00012990: 2020 2020 2320 6170 7065 6e64 2074 6f20      # append to 
-000129a0: 616e 2069 6e74 6572 6e61 6c20 7265 636f  an internal reco
-000129b0: 7264 2c20 7072 696e 7420 6e65 7720 7061  rd, print new pa
-000129c0: 7261 6d73 0d0a 2020 2020 2020 2020 2320  rams..        # 
-000129d0: 706c 6f74 3a20 3320 7374 6163 6b65 642c  plot: 3 stacked,
-000129e0: 2069 6e20 7361 6d70 6c65 2c20 7468 656e   in sample, then
-000129f0: 2065 6163 6820 7661 6c69 6461 7469 6f6e   each validation
-00012a00: 0d0a 2020 2020 2020 2020 2320 6d61 7962  ..        # mayb
-00012a10: 6520 7573 6520 6765 6e65 7469 6320 6f70  e use genetic op
-00012a20: 7469 6d69 7a61 7469 6f6e 2069 6620 7468  timization if th
-00012a30: 6973 2075 7365 6420 6166 7465 7220 6175  is used after au
-00012a40: 746f 5f66 6974 0d0a 2020 2020 2020 2020  to_fit..        
-00012a50: 7265 7475 726e 204e 6f74 496d 706c 656d  return NotImplem
-00012a60: 656e 7465 640d 0a0d 0a20 2020 2064 6566  ented....    def
-00012a70: 2063 726f 7373 5f76 616c 6964 6174 6528   cross_validate(
-00012a80: 7365 6c66 2c20 6466 2c20 7661 6c69 6461  self, df, valida
-00012a90: 7469 6f6e 5f6d 6574 686f 6429 3a0d 0a20  tion_method):.. 
-00012aa0: 2020 2020 2020 2023 2072 756e 206f 6e65         # run one
-00012ab0: 206d 6f64 656c 2061 6e64 2072 6574 7572   model and retur
-00012ac0: 6e20 7363 6f72 6573 0d0a 2020 2020 2020  n scores..      
-00012ad0: 2020 7265 7475 726e 204e 6f74 496d 706c    return NotImpl
-00012ae0: 656d 656e 7465 640d 0a0d 0a20 2020 2064  emented....    d
-00012af0: 6566 2074 7265 6174 6d65 6e74 5f63 6175  ef treatment_cau
-00012b00: 7361 6c5f 696d 7061 6374 280d 0a20 2020  sal_impact(..   
-00012b10: 2020 2020 2073 656c 662c 2064 662c 2069       self, df, i
-00012b20: 6e74 6572 7665 6e74 696f 6e5f 6461 7465  ntervention_date
-00012b30: 730d 0a20 2020 2029 3a20 2023 2061 6c73  s..    ):  # als
-00012b40: 6f20 6164 6420 7265 6772 6573 736f 7220  o add regressor 
-00012b50: 696e 7075 740d 0a20 2020 2020 2020 2023  input..        #
-00012b60: 2072 6567 7265 7373 6f72 7320 696d 706f   regressors impo
-00012b70: 7274 616e 742c 2065 7374 696d 6174 696f  rtant, estimatio
-00012b80: 6e20 6279 206c 696e 6561 7220 666c 6167  n by linear flag
-00012b90: 2028 7265 7475 726e 2073 7461 7473 2920   (return stats) 
-00012ba0: 6f72 2062 7920 2520 7673 2066 6f72 6563  or by % vs forec
-00012bb0: 6173 7420 6672 6f6d 2063 7574 6f66 660d  ast from cutoff.
-00012bc0: 0a20 2020 2020 2020 2023 2073 7461 7274  .        # start
-00012bd0: 2061 6e64 2065 6e64 2064 6174 6573 2c20   and end dates, 
-00012be0: 6d75 6c74 6970 6c65 2074 7265 6174 6d65  multiple treatme
-00012bf0: 6e74 732c 2076 6172 7920 6279 2073 6572  nts, vary by ser
-00012c00: 6965 730d 0a20 2020 2020 2020 2023 206f  ies..        # o
-00012c10: 7220 6d61 7962 6520 696e 7374 6561 642c  r maybe instead,
-00012c20: 206a 7573 7420 7265 7475 726e 2074 6865   just return the
-00012c30: 2073 7461 7473 2066 6f72 2061 6c6c 2069   stats for all i
-00012c40: 6e70 7574 2072 6567 7265 7373 6f72 730d  nput regressors.
-00012c50: 0a20 2020 2020 2020 2023 2073 7469 6c6c  .        # still
-00012c60: 2077 6f72 6b69 6e67 206f 6e20 7468 6973   working on this
-00012c70: 2c20 706f 7373 6962 6c79 206a 7573 7420  , possibly just 
-00012c80: 6874 7470 733a 2f2f 6d61 7468 2e73 7461  https://math.sta
-00012c90: 636b 6578 6368 616e 6765 2e63 6f6d 2f71  ckexchange.com/q
-00012ca0: 7565 7374 696f 6e73 2f32 3131 3235 3533  uestions/2112553
-00012cb0: 2f73 7461 7469 7374 6963 616c 2d73 6967  /statistical-sig
-00012cc0: 6e69 6669 6361 6e63 652d 6f66 2d6c 696e  nificance-of-lin
-00012cd0: 6561 722d 6c65 6173 742d 7371 7561 7265  ear-least-square
-00012ce0: 730d 0a20 2020 2020 2020 2023 2061 6e64  s..        # and
-00012cf0: 206f 7468 6572 2066 6561 7475 7265 7320   other features 
-00012d00: 616c 6120 5374 6174 736d 6f64 656c 7320  ala Statsmodels 
-00012d10: 4f4c 532c 2056 6172 28ce b25e 293d cf83  OLS, Var(..^)=..
-00012d20: 3228 58e2 80b2 5829 e288 9231 2077 6865  2(X...X)...1 whe
-00012d30: 7265 20cf 8332 3e30 2069 7320 7468 6520  re ..2>0 is the 
-00012d40: 636f 6d6d 6f6e 2076 6172 6961 6e63 6520  common variance 
-00012d50: 6f66 2065 6163 6820 656c 656d 656e 7420  of each element 
-00012d60: 6f66 2074 6865 2065 7272 6f72 2076 6563  of the error vec
-00012d70: 746f 720d 0a20 2020 2020 2020 2072 6574  tor..        ret
-00012d80: 7572 6e20 4e6f 7449 6d70 6c65 6d65 6e74  urn NotImplement
-00012d90: 6564 0d0a 0d0a 2020 2020 6465 6620 7072  ed....    def pr
-00012da0: 6564 6963 745f 6e65 775f 7072 6f64 7563  edict_new_produc
-00012db0: 7428 7365 6c66 293a 0d0a 2020 2020 2020  t(self):..      
-00012dc0: 2020 2320 626f 7272 6f77 2074 6865 206c    # borrow the l
-00012dd0: 696e 6561 7220 636f 6d70 6f6e 656e 7473  inear components
-00012de0: 2066 726f 6d20 6120 7265 6c61 7465 6420   from a related 
-00012df0: 7072 6f64 7563 7420 286f 7220 6176 672f  product (or avg/
-00012e00: 6d6f 6465 2069 6620 6e6f 7420 6769 7665  mode if not give
-00012e10: 6e29 0d0a 2020 2020 2020 2020 2320 6861  n)..        # ha
-00012e20: 7665 2074 6865 2074 7265 6e64 2073 7461  ve the trend sta
-00012e30: 7274 2061 7420 7a65 726f 2074 6865 6e20  rt at zero then 
-00012e40: 7570 2c20 6c69 6b65 2072 6576 6572 7365  up, like reverse
-00012e50: 2070 6869 0d0a 2020 2020 2020 2020 2320   phi..        # 
-00012e60: 706f 7373 6962 6c79 2062 6f72 726f 7720  possibly borrow 
-00012e70: 7761 726d 7570 2066 726f 6d20 616e 7920  warmup from any 
-00012e80: 7365 7269 6573 2074 6861 7420 6861 7665  series that have
-00012e90: 2061 206c 6f67 6973 7469 632d 6c69 6b65   a logistic-like
-00012ea0: 2074 7265 6e64 0d0a 2020 2020 2020 2020   trend..        
-00012eb0: 2320 636c 7573 7465 7220 616e 6420 6368  # cluster and ch
-00012ec0: 6f6f 7365 2074 6865 2062 6967 6765 7374  oose the biggest
-00012ed0: 2063 6c75 7374 6572 2028 6173 2061 7667   cluster (as avg
-00012ee0: 2076 616c 7565 206e 6169 7665 206d 6574   value naive met
-00012ef0: 686f 642c 206d 6179 6265 2072 6f75 6e64  hod, maybe round
-00012f00: 206f 7220 6669 6c74 6572 2066 6972 7374   or filter first
-00012f10: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00012f20: 6e20 4e6f 7449 6d70 6c65 6d65 6e74 6564  n NotImplemented
-00012f30: 0d0a 0d0a 2020 2020 6465 6620 6665 6174  ....    def feat
-00012f40: 7572 655f 696d 706f 7274 616e 6365 2873  ure_importance(s
-00012f50: 656c 6629 3a0d 0a20 2020 2020 2020 2023  elf):..        #
-00012f60: 2072 616e 6b20 636f 6566 6669 6369 656e   rank coefficien
-00012f70: 7473 2062 7920 696d 706f 7274 616e 6365  ts by importance
-00012f80: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00012f90: 204e 6f74 496d 706c 656d 656e 7465 640d   NotImplemented.
-00012fa0: 0a0d 0a20 2020 2064 6566 2063 6f6d 7061  ...    def compa
-00012fb0: 7265 5f61 6374 7561 6c5f 636f 6d70 6f6e  re_actual_compon
-00012fc0: 656e 7473 2873 656c 6629 3a0d 0a20 2020  ents(self):..   
-00012fd0: 2020 2020 2072 6574 7572 6e20 4e6f 7449       return NotI
-00012fe0: 6d70 6c65 6d65 6e74 6564 0d0a 0d0a 2020  mplemented....  
-00012ff0: 2020 6465 6620 6765 745f 6e65 775f 7061    def get_new_pa
-00013000: 7261 6d73 2873 656c 662c 206d 6574 686f  rams(self, metho
-00013010: 643d 2766 6173 7427 293a 0d0a 2020 2020  d='fast'):..    
-00013020: 2020 2020 2320 6861 7665 2066 6173 7420      # have fast 
-00013030: 6f70 7469 6f6e 2074 6861 7420 6176 6f69  option that avoi
-00013040: 6473 2061 6e79 206f 6620 7468 6520 6c6f  ds any of the lo
-00013050: 6f70 2061 7070 726f 6163 6865 730d 0a20  op approaches.. 
-00013060: 2020 2020 2020 2073 6361 6c69 6e67 203d         scaling =
-00013070: 2072 616e 646f 6d2e 6368 6f69 6365 7328   random.choices(
-00013080: 5b27 4261 7365 5363 616c 6572 272c 2027  ['BaseScaler', '
-00013090: 6f74 6865 7227 5d2c 205b 302e 382c 2030  other'], [0.8, 0
-000130a0: 2e32 5d29 5b30 5d0d 0a20 2020 2020 2020  .2])[0]..       
-000130b0: 2069 6620 7363 616c 696e 6720 3d3d 2022   if scaling == "
-000130c0: 6f74 6865 7222 3a0d 0a20 2020 2020 2020  other":..       
-000130d0: 2020 2020 2073 6361 6c69 6e67 203d 2052       scaling = R
-000130e0: 616e 646f 6d54 7261 6e73 666f 726d 280d  andomTransform(.
-000130f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013100: 2074 7261 6e73 666f 726d 6572 5f6c 6973   transformer_lis
-00013110: 743d 7363 616c 6572 732c 0d0a 2020 2020  t=scalers,..    
-00013120: 2020 2020 2020 2020 2020 2020 7472 616e              tran
-00013130: 7366 6f72 6d65 725f 6d61 785f 6465 7074  sformer_max_dept
-00013140: 683d 312c 0d0a 2020 2020 2020 2020 2020  h=1,..          
-00013150: 2020 2020 2020 616c 6c6f 775f 6e6f 6e65        allow_none
-00013160: 3d46 616c 7365 2c0d 0a20 2020 2020 2020  =False,..       
-00013170: 2020 2020 2020 2020 206e 6f5f 6e61 6e5f           no_nan_
-00013180: 6669 6c6c 3d54 7275 652c 0d0a 2020 2020  fill=True,..    
-00013190: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-000131a0: 2020 2068 6f6c 6964 6179 5f70 6172 616d     holiday_param
-000131b0: 7320 3d20 7261 6e64 6f6d 2e63 686f 6963  s = random.choic
-000131c0: 6573 285b 4e6f 6e65 2c20 2761 6e79 275d  es([None, 'any']
-000131d0: 2c20 5b30 2e35 2c20 302e 355d 295b 305d  , [0.5, 0.5])[0]
-000131e0: 0d0a 2020 2020 2020 2020 2320 686f 6c69  ..        # holi
-000131f0: 6461 795f 696e 7465 7276 656e 7469 6f6e  day_intervention
-00013200: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
-00013210: 2069 6620 686f 6c69 6461 795f 7061 7261   if holiday_para
-00013220: 6d73 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ms is not None:.
-00013230: 0a20 2020 2020 2020 2020 2020 2023 2068  .            # h
-00013240: 6f6c 6964 6179 5f69 6e74 6572 7665 6e74  oliday_intervent
-00013250: 696f 6e20 3d20 7261 6e64 6f6d 2e63 686f  ion = random.cho
-00013260: 6963 6528 5b27 6372 6561 7465 5f66 6561  ice(['create_fea
-00013270: 7475 7265 272c 2027 7573 655f 696d 7061  ture', 'use_impa
-00013280: 6374 275d 290d 0a20 2020 2020 2020 2020  ct'])..         
-00013290: 2020 2068 6f6c 6964 6179 5f70 6172 616d     holiday_param
-000132a0: 7320 3d20 486f 6c69 6461 7954 7261 6e73  s = HolidayTrans
-000132b0: 666f 726d 6572 2e67 6574 5f6e 6577 5f70  former.get_new_p
-000132c0: 6172 616d 7328 6d65 7468 6f64 3d6d 6574  arams(method=met
-000132d0: 686f 6429 0d0a 2020 2020 2020 2020 2020  hod)..          
-000132e0: 2020 686f 6c69 6461 795f 7061 7261 6d73    holiday_params
-000132f0: 5b27 696d 7061 6374 275d 203d 204e 6f6e  ['impact'] = Non
-00013300: 650d 0a20 2020 2020 2020 2020 2020 2068  e..            h
-00013310: 6f6c 6964 6179 5f70 6172 616d 735b 2772  oliday_params['r
-00013320: 6567 7265 7373 696f 6e5f 7061 7261 6d73  egression_params
-00013330: 275d 203d 204e 6f6e 650d 0a20 2020 2020  '] = None..     
-00013340: 2020 2020 2020 2068 6f6c 6964 6179 5f70         holiday_p
-00013350: 6172 616d 735b 2772 656d 6f76 655f 6578  arams['remove_ex
-00013360: 6365 7373 5f61 6e6f 6d61 6c69 6573 275d  cess_anomalies']
-00013370: 203d 2072 616e 646f 6d2e 6368 6f69 6365   = random.choice
-00013380: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
-00013390: 2020 2020 5b54 7275 652c 2046 616c 7365      [True, False
-000133a0: 5d2c 205b 302e 3035 2c20 302e 3935 5d0d  ], [0.05, 0.95].
-000133b0: 0a20 2020 2020 2020 2020 2020 2029 5b30  .            )[0
-000133c0: 5d0d 0a20 2020 2020 2020 2020 2020 2068  ]..            h
-000133d0: 6f6c 6964 6179 5f70 6172 616d 735b 276f  oliday_params['o
-000133e0: 7574 7075 7427 5d20 3d20 7261 6e64 6f6d  utput'] = random
-000133f0: 2e63 686f 6963 6573 280d 0a20 2020 2020  .choices(..     
-00013400: 2020 2020 2020 2020 2020 205b 276d 756c             ['mul
-00013410: 7469 7661 7269 6174 6527 2c20 2775 6e69  tivariate', 'uni
-00013420: 7661 7269 6174 6527 5d2c 205b 302e 392c  variate'], [0.9,
-00013430: 2030 2e31 5d0d 0a20 2020 2020 2020 2020   0.1]..         
-00013440: 2020 2029 5b30 5d0d 0a20 2020 2020 2020     )[0]..       
-00013450: 2061 6e6f 6d61 6c79 5f69 6e74 6572 7665   anomaly_interve
-00013460: 6e74 696f 6e20 3d20 7261 6e64 6f6d 2e63  ntion = random.c
-00013470: 686f 6963 6573 280d 0a20 2020 2020 2020  hoices(..       
-00013480: 2020 2020 205b 4e6f 6e65 2c20 2772 656d       [None, 'rem
-00013490: 6f76 6527 2c20 2764 6574 6563 745f 6f6e  ove', 'detect_on
-000134a0: 6c79 272c 2027 6d6f 6465 6c27 5d2c 205b  ly', 'model'], [
-000134b0: 302e 392c 2030 2e33 2c20 302e 3035 2c20  0.9, 0.3, 0.05, 
-000134c0: 302e 3035 5d0d 0a20 2020 2020 2020 2029  0.05]..        )
-000134d0: 5b30 5d0d 0a20 2020 2020 2020 2069 6620  [0]..        if 
-000134e0: 616e 6f6d 616c 795f 696e 7465 7276 656e  anomaly_interven
-000134f0: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
-00013500: 3a0d 0a20 2020 2020 2020 2020 2020 2061  :..            a
-00013510: 6e6f 6d61 6c79 5f64 6574 6563 746f 725f  nomaly_detector_
-00013520: 7061 7261 6d73 203d 2041 6e6f 6d61 6c79  params = Anomaly
-00013530: 5265 6d6f 7661 6c2e 6765 745f 6e65 775f  Removal.get_new_
-00013540: 7061 7261 6d73 286d 6574 686f 643d 6d65  params(method=me
-00013550: 7468 6f64 290d 0a20 2020 2020 2020 2020  thod)..         
-00013560: 2020 2069 6620 616e 6f6d 616c 795f 696e     if anomaly_in
-00013570: 7465 7276 656e 7469 6f6e 203d 3d20 226d  tervention == "m
-00013580: 6f64 656c 223a 0d0a 2020 2020 2020 2020  odel":..        
-00013590: 2020 2020 2020 2020 616e 6f6d 616c 795f          anomaly_
-000135a0: 696e 7465 7276 656e 7469 6f6e 203d 2067  intervention = g
-000135b0: 656e 6572 616c 5f74 656d 706c 6174 652e  eneral_template.
-000135c0: 7361 6d70 6c65 2831 292e 746f 5f64 6963  sample(1).to_dic
-000135d0: 7428 2272 6563 6f72 6473 2229 5b0d 0a20  t("records")[.. 
-000135e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135f0: 2020 2030 0d0a 2020 2020 2020 2020 2020     0..          
-00013600: 2020 2020 2020 5d20 2023 2070 6c61 6365        ]  # place
-00013610: 686f 6c64 6572 2c20 7072 6f62 6162 6c79  holder, probably
-00013620: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00013630: 0a20 2020 2020 2020 2020 2020 2061 6e6f  .            ano
-00013640: 6d61 6c79 5f64 6574 6563 746f 725f 7061  maly_detector_pa
-00013650: 7261 6d73 203d 204e 6f6e 650d 0a0d 0a20  rams = None.... 
-00013660: 2020 2020 2020 2023 2072 616e 646f 6d20         # random 
-00013670: 6f72 2070 7265 7465 7374 6564 2064 6566  or pretested def
-00013680: 6175 6c74 730d 0a20 2020 2020 2020 2069  aults..        i
-00013690: 6620 6d65 7468 6f64 2069 6e20 5b27 6465  f method in ['de
-000136a0: 6570 272c 2027 616c 6c27 5d3a 0d0a 2020  ep', 'all']:..  
-000136b0: 2020 2020 2020 2020 2020 7472 656e 645f            trend_
-000136c0: 6261 7365 203d 2027 6465 6570 270d 0a20  base = 'deep'.. 
-000136d0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000136e0: 2020 2020 2020 2020 2020 7472 656e 645f            trend_
-000136f0: 6261 7365 203d 2072 616e 646f 6d2e 6368  base = random.ch
-00013700: 6f69 6365 7328 0d0a 2020 2020 2020 2020  oices(..        
-00013710: 2020 2020 2020 2020 5b27 7062 3127 2c20          ['pb1', 
-00013720: 2770 6232 272c 2027 7062 3327 2c20 2772  'pb2', 'pb3', 'r
-00013730: 616e 646f 6d27 5d2c 205b 302e 312c 2030  andom'], [0.1, 0
-00013740: 2e31 2c20 302e 302c 2030 2e38 5d0d 0a20  .1, 0.0, 0.8].. 
-00013750: 2020 2020 2020 2020 2020 2029 5b30 5d0d             )[0].
-00013760: 0a20 2020 2020 2020 2069 6620 7472 656e  .        if tren
-00013770: 645f 6261 7365 203d 3d20 2272 616e 646f  d_base == "rando
-00013780: 6d22 3a0d 0a20 2020 2020 2020 2020 2020  m":..           
-00013790: 206d 6f64 656c 5f73 7472 203d 2072 616e   model_str = ran
-000137a0: 646f 6d2e 6368 6f69 6365 7328 0d0a 2020  dom.choices(..  
-000137b0: 2020 2020 2020 2020 2020 2020 2020 5b0d                [.
-000137c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000137d0: 2020 2020 2027 4176 6572 6167 6556 616c       'AverageVal
-000137e0: 7565 4e61 6976 6527 2c0d 0a20 2020 2020  ueNaive',..     
-000137f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00013800: 4d65 7472 6963 4d6f 7469 6627 2c0d 0a20  MetricMotif',.. 
-00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013820: 2020 2022 4c61 7374 5661 6c75 654e 6169     "LastValueNai
-00013830: 7665 222c 0d0a 2020 2020 2020 2020 2020  ve",..          
-00013840: 2020 2020 2020 2020 2020 2753 6561 736f            'Seaso
-00013850: 6e61 6c69 7479 4d6f 7469 6627 2c0d 0a20  nalityMotif',.. 
-00013860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013870: 2020 2027 5769 6e64 6f77 5265 6772 6573     'WindowRegres
-00013880: 7369 6f6e 272c 0d0a 2020 2020 2020 2020  sion',..        
-00013890: 2020 2020 2020 2020 2020 2020 2741 5244              'ARD
-000138a0: 4c27 2c0d 0a20 2020 2020 2020 2020 2020  L',..           
-000138b0: 2020 2020 2020 2020 2027 5641 5227 2c0d           'VAR',.
-000138c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000138d0: 2020 2020 2027 556e 6976 6172 6961 7465       'Univariate
-000138e0: 4d6f 7469 6627 2c0d 0a20 2020 2020 2020  Motif',..       
-000138f0: 2020 2020 2020 2020 2020 2020 2027 556e               'Un
-00013900: 6f62 7365 7276 6564 436f 6d70 6f6e 656e  observedComponen
-00013910: 7473 272c 0d0a 2020 2020 2020 2020 2020  ts',..          
-00013920: 2020 2020 2020 2020 2020 224b 616c 6d61            "Kalma
-00013930: 6e53 7461 7465 5370 6163 6522 2c0d 0a20  nStateSpace",.. 
-00013940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013950: 2020 2027 5252 5641 5227 2c0d 0a20 2020     'RRVAR',..   
-00013960: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
-00013970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013980: 205b 302e 3035 2c20 302e 3035 2c20 302e   [0.05, 0.05, 0.
-00013990: 312c 2030 2e30 352c 2030 2e30 352c 2030  1, 0.05, 0.05, 0
-000139a0: 2e31 352c 2030 2e30 352c 2030 2e30 352c  .15, 0.05, 0.05,
-000139b0: 2030 2e30 352c 2030 2e30 352c 2030 2e30   0.05, 0.05, 0.0
-000139c0: 355d 2c0d 0a20 2020 2020 2020 2020 2020  5],..           
-000139d0: 2020 2020 206b 3d31 2c0d 0a20 2020 2020       k=1,..     
-000139e0: 2020 2020 2020 2029 5b30 5d0d 0a20 2020         )[0]..   
-000139f0: 2020 2020 2020 2020 2074 7265 6e64 5f6d           trend_m
-00013a00: 6f64 656c 203d 207b 274d 6f64 656c 273a  odel = {'Model':
-00013a10: 206d 6f64 656c 5f73 7472 7d0d 0a20 2020   model_str}..   
-00013a20: 2020 2020 2020 2020 2074 7265 6e64 5f6d           trend_m
-00013a30: 6f64 656c 5b27 4d6f 6465 6c50 6172 616d  odel['ModelParam
-00013a40: 6574 6572 7327 5d20 3d20 4d6f 6465 6c4d  eters'] = ModelM
-00013a50: 6f6e 7374 6572 286d 6f64 656c 5f73 7472  onster(model_str
-00013a60: 292e 6765 745f 6e65 775f 7061 7261 6d73  ).get_new_params
-00013a70: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00013a80: 2020 206d 6574 686f 643d 6d65 7468 6f64     method=method
-00013a90: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
-00013aa0: 0a20 2020 2020 2020 2020 2020 2074 7265  .            tre
-00013ab0: 6e64 5f74 7261 6e73 666f 726d 6174 696f  nd_transformatio
-00013ac0: 6e20 3d20 5261 6e64 6f6d 5472 616e 7366  n = RandomTransf
-00013ad0: 6f72 6d28 0d0a 2020 2020 2020 2020 2020  orm(..          
-00013ae0: 2020 2020 2020 7472 616e 7366 6f72 6d65        transforme
-00013af0: 725f 6c69 7374 3d22 6661 7374 222c 0d0a  r_list="fast",..
-00013b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b10: 7472 616e 7366 6f72 6d65 725f 6d61 785f  transformer_max_
-00013b20: 6465 7074 683d 332c 2020 2320 7072 6f62  depth=3,  # prob
-00013b30: 6162 6c79 2077 616e 7420 736f 6d65 206d  ably want some m
-00013b40: 6f72 6520 7573 6162 6c65 2064 6566 6175  ore usable defau
-00013b50: 6c74 7320 6669 7273 7420 6173 206d 616e  lts first as man
-00013b60: 7920 7261 6e64 6f6d 2061 7265 2073 656e  y random are sen
-00013b70: 7365 6c65 7373 0d0a 2020 2020 2020 2020  seless..        
-00013b80: 2020 2020 290d 0a20 2020 2020 2020 2065      )..        e
-00013b90: 6c69 6620 7472 656e 645f 6261 7365 203d  lif trend_base =
-00013ba0: 3d20 2770 6231 273a 0d0a 2020 2020 2020  = 'pb1':..      
-00013bb0: 2020 2020 2020 7472 656e 645f 6d6f 6465        trend_mode
-00013bc0: 6c20 3d20 7b27 4d6f 6465 6c27 3a20 2741  l = {'Model': 'A
-00013bd0: 5244 4c27 7d0d 0a20 2020 2020 2020 2020  RDL'}..         
-00013be0: 2020 2074 7265 6e64 5f6d 6f64 656c 5b27     trend_model['
-00013bf0: 4d6f 6465 6c50 6172 616d 6574 6572 7327  ModelParameters'
-00013c00: 5d20 3d20 7b0d 0a20 2020 2020 2020 2020  ] = {..         
-00013c10: 2020 2020 2020 2022 6c61 6773 223a 2031         "lags": 1
-00013c20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00013c30: 2020 2022 7472 656e 6422 3a20 226e 222c     "trend": "n",
-00013c40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013c50: 2020 226f 7264 6572 223a 2030 2c0d 0a20    "order": 0,.. 
-00013c60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00013c70: 6361 7573 616c 223a 2046 616c 7365 2c0d  causal": False,.
-00013c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013c90: 2022 7265 6772 6573 7369 6f6e 5f74 7970   "regression_typ
-00013ca0: 6522 3a20 2273 696d 706c 6522 2c0d 0a20  e": "simple",.. 
-00013cb0: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00013cc0: 2020 2020 2020 2020 2020 7472 656e 645f            trend_
-00013cd0: 7472 616e 7366 6f72 6d61 7469 6f6e 203d  transformation =
-00013ce0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00013cf0: 2020 2020 2266 696c 6c6e 6122 3a20 226e      "fillna": "n
-00013d00: 6561 7265 7374 222c 0d0a 2020 2020 2020  earest",..      
-00013d10: 2020 2020 2020 2020 2020 2274 7261 6e73            "trans
-00013d20: 666f 726d 6174 696f 6e73 223a 207b 2230  formations": {"0
-00013d30: 223a 2022 5374 616e 6461 7264 5363 616c  ": "StandardScal
-00013d40: 6572 222c 2022 3122 3a20 2241 6e6f 6d61  er", "1": "Anoma
-00013d50: 6c79 5265 6d6f 7661 6c22 7d2c 0d0a 2020  lyRemoval"},..  
-00013d60: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00013d70: 7261 6e73 666f 726d 6174 696f 6e5f 7061  ransformation_pa
-00013d80: 7261 6d73 223a 207b 0d0a 2020 2020 2020  rams": {..      
-00013d90: 2020 2020 2020 2020 2020 2020 2020 2230                "0
-00013da0: 223a 207b 7d2c 0d0a 2020 2020 2020 2020  ": {},..        
-00013db0: 2020 2020 2020 2020 2020 2020 2231 223a              "1":
-00013dc0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00013dd0: 2020 2020 2020 2020 2020 2020 226d 6574              "met
-00013de0: 686f 6422 3a20 2249 5152 222c 0d0a 2020  hod": "IQR",..  
-00013df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e00: 2020 2020 2020 2274 7261 6e73 666f 726d        "transform
-00013e10: 5f64 6963 7422 3a20 7b0d 0a20 2020 2020  _dict": {..     
-00013e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e30: 2020 2020 2020 2022 6669 6c6c 6e61 223a         "fillna":
-00013e40: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
-00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e60: 2020 2020 2274 7261 6e73 666f 726d 6174      "transformat
-00013e70: 696f 6e73 223a 207b 2230 223a 2022 436c  ions": {"0": "Cl
-00013e80: 6970 4f75 746c 6965 7273 227d 2c0d 0a20  ipOutliers"},.. 
-00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ea0: 2020 2020 2020 2020 2020 2022 7472 616e             "tran
-00013eb0: 7366 6f72 6d61 7469 6f6e 5f70 6172 616d  sformation_param
-00013ec0: 7322 3a20 7b0d 0a20 2020 2020 2020 2020  s": {..         
-00013ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ee0: 2020 2020 2020 2022 3022 3a20 7b22 6d65         "0": {"me
-00013ef0: 7468 6f64 223a 2022 636c 6970 222c 2022  thod": "clip", "
-00013f00: 7374 645f 7468 7265 7368 6f6c 6422 3a20  std_threshold": 
-00013f10: 367d 0d0a 2020 2020 2020 2020 2020 2020  6}..            
-00013f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f30: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00013f40: 2020 2020 2020 2020 2020 2020 7d2c 0d0a              },..
-00013f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f60: 2020 2020 2020 2020 226d 6574 686f 645f          "method_
-00013f70: 7061 7261 6d73 223a 207b 0d0a 2020 2020  params": {..    
-00013f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f90: 2020 2020 2020 2020 2269 7172 5f74 6872          "iqr_thr
-00013fa0: 6573 686f 6c64 223a 2032 2e35 2c0d 0a20  eshold": 2.5,.. 
-00013fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fc0: 2020 2020 2020 2020 2020 2022 6971 725f             "iqr_
-00013fd0: 7175 616e 7469 6c65 7322 3a20 5b30 2e32  quantiles": [0.2
-00013fe0: 352c 2030 2e37 355d 2c0d 0a20 2020 2020  5, 0.75],..     
-00013ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014000: 2020 207d 2c0d 0a20 2020 2020 2020 2020     },..         
-00014010: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00014020: 6669 6c6c 6e61 223a 2022 6666 696c 6c22  fillna": "ffill"
-00014030: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00014040: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00014050: 2020 2020 2020 2020 2020 207d 2c0d 0a20             },.. 
-00014060: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00014070: 2020 2020 2020 656c 6966 2074 7265 6e64        elif trend
-00014080: 5f62 6173 6520 3d3d 2027 7062 3227 3a0d  _base == 'pb2':.
-00014090: 0a20 2020 2020 2020 2020 2020 2074 7265  .            tre
-000140a0: 6e64 5f6d 6f64 656c 203d 207b 274d 6f64  nd_model = {'Mod
-000140b0: 656c 273a 2027 5769 6e64 6f77 5265 6772  el': 'WindowRegr
-000140c0: 6573 7369 6f6e 277d 0d0a 2020 2020 2020  ession'}..      
-000140d0: 2020 2020 2020 7472 656e 645f 6d6f 6465        trend_mode
-000140e0: 6c5b 274d 6f64 656c 5061 7261 6d65 7465  l['ModelParamete
-000140f0: 7273 275d 203d 207b 0d0a 2020 2020 2020  rs'] = {..      
-00014100: 2020 2020 2020 2020 2020 2277 696e 646f            "windo
-00014110: 775f 7369 7a65 223a 2031 322c 0d0a 2020  w_size": 12,..  
-00014120: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00014130: 6e70 7574 5f64 696d 223a 2022 756e 6976  nput_dim": "univ
-00014140: 6172 6961 7465 222c 0d0a 2020 2020 2020  ariate",..      
-00014150: 2020 2020 2020 2020 2020 226f 7574 7075            "outpu
-00014160: 745f 6469 6d22 3a20 2231 7374 6570 222c  t_dim": "1step",
-00014170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014180: 2020 226e 6f72 6d61 6c69 7a65 5f77 696e    "normalize_win
-00014190: 646f 7722 3a20 4661 6c73 652c 0d0a 2020  dow": False,..  
-000141a0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-000141b0: 6178 5f77 696e 646f 7773 223a 2038 3030  ax_windows": 800
-000141c0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-000141d0: 2020 2020 2272 6567 7265 7373 696f 6e5f      "regression_
-000141e0: 7479 7065 223a 204e 6f6e 652c 0d0a 2020  type": None,..  
-000141f0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00014200: 6567 7265 7373 696f 6e5f 6d6f 6465 6c22  egression_model"
-00014210: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-00014220: 2020 2020 2020 2020 2022 6d6f 6465 6c22           "model"
-00014230: 3a20 2245 7874 7261 5472 6565 7322 2c0d  : "ExtraTrees",.
-00014240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014250: 2020 2020 2022 6d6f 6465 6c5f 7061 7261       "model_para
-00014260: 6d73 223a 207b 0d0a 2020 2020 2020 2020  ms": {..        
-00014270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014280: 226e 5f65 7374 696d 6174 6f72 7322 3a20  "n_estimators": 
-00014290: 3130 302c 0d0a 2020 2020 2020 2020 2020  100,..          
-000142a0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-000142b0: 696e 5f73 616d 706c 6573 5f6c 6561 6622  in_samples_leaf"
-000142c0: 3a20 312c 0d0a 2020 2020 2020 2020 2020  : 1,..          
-000142d0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-000142e0: 6178 5f64 6570 7468 223a 2032 302c 0d0a  ax_depth": 20,..
-000142f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014300: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00014310: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00014320: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00014330: 2020 2020 2020 2074 7265 6e64 5f74 7261         trend_tra
-00014340: 6e73 666f 726d 6174 696f 6e20 3d20 7b0d  nsformation = {.
-00014350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014360: 2022 6669 6c6c 6e61 223a 2022 6666 696c   "fillna": "ffil
-00014370: 6c22 2c0d 0a20 2020 2020 2020 2020 2020  l",..           
-00014380: 2020 2020 2022 7472 616e 7366 6f72 6d61       "transforma
-00014390: 7469 6f6e 7322 3a20 7b22 3022 3a20 2241  tions": {"0": "A
-000143a0: 6e6f 6d61 6c79 5265 6d6f 7661 6c22 2c20  nomalyRemoval", 
-000143b0: 2231 223a 2022 526f 6275 7374 5363 616c  "1": "RobustScal
-000143c0: 6572 227d 2c0d 0a20 2020 2020 2020 2020  er"},..         
-000143d0: 2020 2020 2020 2022 7472 616e 7366 6f72         "transfor
-000143e0: 6d61 7469 6f6e 5f70 6172 616d 7322 3a20  mation_params": 
-000143f0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00014400: 2020 2020 2020 2022 3022 3a20 7b0d 0a20         "0": {.. 
-00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014420: 2020 2020 2020 2022 6d65 7468 6f64 223a         "method":
-00014430: 2022 4951 5222 2c0d 0a20 2020 2020 2020   "IQR",..       
-00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014450: 2022 7472 616e 7366 6f72 6d5f 6469 6374   "transform_dict
-00014460: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
-00014470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014480: 2020 2266 696c 6c6e 6122 3a20 4e6f 6e65    "fillna": None
-00014490: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000144a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000144b0: 7472 616e 7366 6f72 6d61 7469 6f6e 7322  transformations"
-000144c0: 3a20 7b22 3022 3a20 2243 6c69 704f 7574  : {"0": "ClipOut
-000144d0: 6c69 6572 7322 7d2c 0d0a 2020 2020 2020  liers"},..      
-000144e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144f0: 2020 2020 2020 2274 7261 6e73 666f 726d        "transform
-00014500: 6174 696f 6e5f 7061 7261 6d73 223a 207b  ation_params": {
-00014510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014530: 2020 2230 223a 207b 226d 6574 686f 6422    "0": {"method"
-00014540: 3a20 2263 6c69 7022 2c20 2273 7464 5f74  : "clip", "std_t
-00014550: 6872 6573 686f 6c64 223a 2036 7d0d 0a20  hreshold": 6}.. 
-00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014570: 2020 2020 2020 2020 2020 207d 2c0d 0a20             },.. 
-00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014590: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-000145a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145b0: 2020 2022 6d65 7468 6f64 5f70 6172 616d     "method_param
-000145c0: 7322 3a20 7b0d 0a20 2020 2020 2020 2020  s": {..         
-000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145e0: 2020 2022 6971 725f 7468 7265 7368 6f6c     "iqr_threshol
-000145f0: 6422 3a20 322e 352c 0d0a 2020 2020 2020  d": 2.5,..      
-00014600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014610: 2020 2020 2020 2269 7172 5f71 7561 6e74        "iqr_quant
-00014620: 696c 6573 223a 205b 302e 3235 2c20 302e  iles": [0.25, 0.
-00014630: 3735 5d2c 0d0a 2020 2020 2020 2020 2020  75],..          
-00014640: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00014650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014660: 2020 2020 2020 2020 2020 2266 696c 6c6e            "filln
-00014670: 6122 3a20 2266 6669 6c6c 222c 0d0a 2020  a": "ffill",..  
-00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014690: 2020 7d2c 0d0a 2020 2020 2020 2020 2020    },..          
-000146a0: 2020 2020 2020 2020 2020 2231 223a 207b            "1": {
-000146b0: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-000146c0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-000146d0: 2020 2020 7d0d 0a20 2020 2020 2020 2065      }..        e
-000146e0: 6c69 6620 7472 656e 645f 6261 7365 203d  lif trend_base =
-000146f0: 3d20 2264 6565 7022 3a0d 0a20 2020 2020  = "deep":..     
-00014700: 2020 2020 2020 206d 6f64 656c 5f6c 6973         model_lis
-00014710: 7420 3d20 2261 6c6c 5f70 7261 676d 6174  t = "all_pragmat
-00014720: 6963 220d 0a20 2020 2020 2020 2020 2020  ic"..           
-00014730: 206d 6f64 656c 5f6c 6973 742c 206d 6f64   model_list, mod
-00014740: 656c 5f70 726f 6220 3d20 6d6f 6465 6c5f  el_prob = model_
-00014750: 6c69 7374 5f74 6f5f 6469 6374 286d 6f64  list_to_dict(mod
-00014760: 656c 5f6c 6973 7429 0d0a 2020 2020 2020  el_list)..      
-00014770: 2020 2020 2020 6d6f 6465 6c5f 7374 7220        model_str 
-00014780: 3d20 7261 6e64 6f6d 2e63 686f 6963 6573  = random.choices
-00014790: 286d 6f64 656c 5f6c 6973 742c 206d 6f64  (model_list, mod
-000147a0: 656c 5f70 726f 622c 206b 3d31 295b 305d  el_prob, k=1)[0]
-000147b0: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-000147c0: 656e 645f 6d6f 6465 6c20 3d20 7b27 4d6f  end_model = {'Mo
-000147d0: 6465 6c27 3a20 6d6f 6465 6c5f 7374 727d  del': model_str}
-000147e0: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-000147f0: 656e 645f 6d6f 6465 6c5b 274d 6f64 656c  end_model['Model
-00014800: 5061 7261 6d65 7465 7273 275d 203d 204d  Parameters'] = M
-00014810: 6f64 656c 4d6f 6e73 7465 7228 6d6f 6465  odelMonster(mode
-00014820: 6c5f 7374 7229 2e67 6574 5f6e 6577 5f70  l_str).get_new_p
-00014830: 6172 616d 7328 0d0a 2020 2020 2020 2020  arams(..        
-00014840: 2020 2020 2020 2020 6d65 7468 6f64 3d6d          method=m
-00014850: 6574 686f 640d 0a20 2020 2020 2020 2020  ethod..         
-00014860: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-00014870: 2020 7472 656e 645f 7472 616e 7366 6f72    trend_transfor
-00014880: 6d61 7469 6f6e 203d 2052 616e 646f 6d54  mation = RandomT
-00014890: 7261 6e73 666f 726d 280d 0a20 2020 2020  ransform(..     
-000148a0: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-000148b0: 666f 726d 6572 5f6c 6973 743d 2261 6c6c  former_list="all
-000148c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000148d0: 2020 2020 7472 616e 7366 6f72 6d65 725f      transformer_
-000148e0: 6d61 785f 6465 7074 683d 332c 2020 2320  max_depth=3,  # 
-000148f0: 7072 6f62 6162 6c79 2077 616e 7420 736f  probably want so
-00014900: 6d65 206d 6f72 6520 7573 6162 6c65 2064  me more usable d
-00014910: 6566 6175 6c74 7320 6669 7273 7420 6173  efaults first as
-00014920: 206d 616e 7920 7261 6e64 6f6d 2061 7265   many random are
-00014930: 2073 656e 7365 6c65 7373 0d0a 2020 2020   senseless..    
-00014940: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-00014950: 2020 2020 2074 7265 6e64 5f61 6e6f 6d61       trend_anoma
-00014960: 6c79 5f69 6e74 6572 7665 6e74 696f 6e20  ly_intervention 
-00014970: 3d20 7261 6e64 6f6d 2e63 686f 6963 6573  = random.choices
-00014980: 285b 4e6f 6e65 2c20 2764 6574 6563 745f  ([None, 'detect_
-00014990: 6f6e 6c79 275d 2c20 5b30 2e35 2c20 302e  only'], [0.5, 0.
-000149a0: 355d 295b 0d0a 2020 2020 2020 2020 2020  5])[..          
-000149b0: 2020 300d 0a20 2020 2020 2020 205d 0d0a    0..        ]..
-000149c0: 2020 2020 2020 2020 6966 2074 7265 6e64          if trend
-000149d0: 5f61 6e6f 6d61 6c79 5f69 6e74 6572 7665  _anomaly_interve
-000149e0: 6e74 696f 6e20 6973 206e 6f74 204e 6f6e  ntion is not Non
-000149f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00014a00: 7472 656e 645f 616e 6f6d 616c 795f 6465  trend_anomaly_de
-00014a10: 7465 6374 6f72 5f70 6172 616d 7320 3d20  tector_params = 
-00014a20: 416e 6f6d 616c 7952 656d 6f76 616c 2e67  AnomalyRemoval.g
-00014a30: 6574 5f6e 6577 5f70 6172 616d 7328 6d65  et_new_params(me
-00014a40: 7468 6f64 3d6d 6574 686f 6429 0d0a 2020  thod=method)..  
-00014a50: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00014a60: 2020 2020 2020 2020 2074 7265 6e64 5f61           trend_a
-00014a70: 6e6f 6d61 6c79 5f64 6574 6563 746f 725f  nomaly_detector_
-00014a80: 7061 7261 6d73 203d 204e 6f6e 650d 0a20  params = None.. 
-00014a90: 2020 2020 2020 206c 696e 6561 725f 6d6f         linear_mo
-00014aa0: 6465 6c20 3d20 7261 6e64 6f6d 2e63 686f  del = random.cho
-00014ab0: 6963 6573 280d 0a20 2020 2020 2020 2020  ices(..         
-00014ac0: 2020 205b 0d0a 2020 2020 2020 2020 2020     [..          
-00014ad0: 2020 2020 2020 276c 7374 7371 272c 0d0a        'lstsq',..
-00014ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014af0: 276c 696e 616c 675f 736f 6c76 6527 2c0d  'linalg_solve',.
-00014b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014b10: 2027 6c31 5f6e 6f72 6d27 2c0d 0a20 2020   'l1_norm',..   
-00014b20: 2020 2020 2020 2020 2020 2020 2027 6477               'dw
-00014b30: 6165 5f6e 6f72 6d27 2c0d 0a20 2020 2020  ae_norm',..     
-00014b40: 2020 2020 2020 2020 2020 2027 7175 616e             'quan
-00014b50: 7469 6c65 5f6e 6f72 6d27 2c0d 0a20 2020  tile_norm',..   
-00014b60: 2020 2020 2020 2020 2020 2020 2027 6c31               'l1
-00014b70: 5f70 6f73 6974 6976 6527 2c0d 0a20 2020  _positive',..   
-00014b80: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00014b90: 2020 2020 2020 2020 205b 302e 362c 2030           [0.6, 0
-00014ba0: 2e32 2c20 302e 312c 2030 2e30 352c 2030  .2, 0.1, 0.05, 0
-00014bb0: 2e30 322c 2030 2e30 335d 2c0d 0a20 2020  .02, 0.03],..   
-00014bc0: 2020 2020 2029 5b30 5d0d 0a20 2020 2020       )[0]..     
-00014bd0: 2020 2072 6563 656e 6379 5f77 6569 6768     recency_weigh
-00014be0: 7469 6e67 203d 2072 616e 646f 6d2e 6368  ting = random.ch
-00014bf0: 6f69 6365 7328 0d0a 2020 2020 2020 2020  oices(..        
-00014c00: 2020 2020 5b4e 6f6e 652c 2030 2e30 352c      [None, 0.05,
-00014c10: 2030 2e31 2c20 302e 3235 2c20 302e 355d   0.1, 0.25, 0.5]
-00014c20: 2c20 5b30 2e37 2c20 302e 312c 2030 2e31  , [0.7, 0.1, 0.1
-00014c30: 2c20 302e 312c 2030 2e30 355d 0d0a 2020  , 0.1, 0.05]..  
-00014c40: 2020 2020 2020 295b 305d 0d0a 2020 2020        )[0]..    
-00014c50: 2020 2020 6966 206c 696e 6561 725f 6d6f      if linear_mo
-00014c60: 6465 6c20 696e 205b 276c 7374 7371 275d  del in ['lstsq']
-00014c70: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
-00014c80: 696e 6561 725f 6d6f 6465 6c20 3d20 7b0d  inear_model = {.
-00014c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ca0: 2027 6d6f 6465 6c27 3a20 6c69 6e65 6172   'model': linear
-00014cb0: 5f6d 6f64 656c 2c0d 0a20 2020 2020 2020  _model,..       
-00014cc0: 2020 2020 2020 2020 2027 6c61 6d62 6461           'lambda
-00014cd0: 273a 2072 616e 646f 6d2e 6368 6f69 6365  ': random.choice
-00014ce0: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
-00014cf0: 2020 2020 2020 2020 5b4e 6f6e 652c 2030          [None, 0
-00014d00: 2e31 2c20 312c 2031 302c 2031 3030 5d2c  .1, 1, 10, 100],
-00014d10: 205b 302e 372c 2030 2e31 2c20 302e 312c   [0.7, 0.1, 0.1,
-00014d20: 2030 2e31 2c20 302e 3035 5d0d 0a20 2020   0.1, 0.05]..   
-00014d30: 2020 2020 2020 2020 2020 2020 2029 5b30               )[0
-00014d40: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00014d50: 2020 2020 2772 6563 656e 6379 5f77 6569      'recency_wei
-00014d60: 6768 7469 6e67 273a 2072 6563 656e 6379  ghting': recency
-00014d70: 5f77 6569 6768 7469 6e67 2c0d 0a20 2020  _weighting,..   
-00014d80: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00014d90: 2020 2020 6966 206c 696e 6561 725f 6d6f      if linear_mo
-00014da0: 6465 6c20 696e 205b 276c 696e 616c 675f  del in ['linalg_
-00014db0: 736f 6c76 6527 5d3a 0d0a 2020 2020 2020  solve']:..      
-00014dc0: 2020 2020 2020 6c69 6e65 6172 5f6d 6f64        linear_mod
-00014dd0: 656c 203d 207b 0d0a 2020 2020 2020 2020  el = {..        
-00014de0: 2020 2020 2020 2020 276d 6f64 656c 273a          'model':
-00014df0: 206c 696e 6561 725f 6d6f 6465 6c2c 0d0a   linear_model,..
-00014e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e10: 276c 616d 6264 6127 3a20 7261 6e64 6f6d  'lambda': random
-00014e20: 2e63 686f 6963 6573 285b 302c 2030 2e31  .choices([0, 0.1
-00014e30: 2c20 312c 2031 305d 2c20 5b30 2e34 2c20  , 1, 10], [0.4, 
-00014e40: 302e 322c 2030 2e32 2c20 302e 325d 295b  0.2, 0.2, 0.2])[
-00014e50: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
-00014e60: 2020 2020 2027 7265 6365 6e63 795f 7765       'recency_we
-00014e70: 6967 6874 696e 6727 3a20 7265 6365 6e63  ighting': recenc
-00014e80: 795f 7765 6967 6874 696e 672c 0d0a 2020  y_weighting,..  
-00014e90: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-00014ea0: 2020 2020 2065 6c69 6620 6c69 6e65 6172       elif linear
-00014eb0: 5f6d 6f64 656c 2069 6e20 5b27 6c31 5f6e  _model in ['l1_n
-00014ec0: 6f72 6d27 2c20 2764 7761 655f 6e6f 726d  orm', 'dwae_norm
-00014ed0: 272c 2027 7175 616e 7469 6c65 5f6e 6f72  ', 'quantile_nor
-00014ee0: 6d27 2c20 276c 315f 706f 7369 7469 7665  m', 'l1_positive
-00014ef0: 275d 3a0d 0a20 2020 2020 2020 2020 2020  ']:..           
-00014f00: 206c 696e 6561 725f 6d6f 6465 6c20 3d20   linear_model = 
-00014f10: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00014f20: 2020 2027 6d6f 6465 6c27 3a20 6c69 6e65     'model': line
-00014f30: 6172 5f6d 6f64 656c 2c0d 0a20 2020 2020  ar_model,..     
-00014f40: 2020 2020 2020 2020 2020 2027 7265 6365             'rece
-00014f50: 6e63 795f 7765 6967 6874 696e 6727 3a20  ncy_weighting': 
-00014f60: 7265 6365 6e63 795f 7765 6967 6874 696e  recency_weightin
-00014f70: 672c 0d0a 2020 2020 2020 2020 2020 2020  g,..            
-00014f80: 2020 2020 276d 6178 6974 6572 273a 2072      'maxiter': r
-00014f90: 616e 646f 6d2e 6368 6f69 6365 7328 5b32  andom.choices([2
-00014fa0: 3530 2c20 3135 3030 302c 2032 3530 3030  50, 15000, 25000
-00014fb0: 5d2c 205b 302e 322c 2030 2e36 2c20 302e  ], [0.2, 0.6, 0.
-00014fc0: 325d 295b 305d 2c0d 0a20 2020 2020 2020  2])[0],..       
-00014fd0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00014fe0: 6966 206d 6574 686f 6420 3d3d 2022 7265  if method == "re
-00014ff0: 6772 6573 736f 7222 3a0d 0a20 2020 2020  gressor":..     
-00015000: 2020 2020 2020 2072 6567 7265 7373 6f72         regressor
-00015010: 735f 7573 6564 203d 2054 7275 650d 0a20  s_used = True.. 
-00015020: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00015030: 2020 2020 2020 2020 2020 7265 6772 6573            regres
-00015040: 736f 7273 5f75 7365 6420 3d20 7261 6e64  sors_used = rand
-00015050: 6f6d 2e63 686f 6963 6573 285b 5472 7565  om.choices([True
-00015060: 2c20 4661 6c73 655d 2c20 5b30 2e35 2c20  , False], [0.5, 
-00015070: 302e 355d 295b 305d 0d0a 2020 2020 2020  0.5])[0]..      
-00015080: 2020 6172 5f6c 6167 7320 3d20 7261 6e64    ar_lags = rand
-00015090: 6f6d 2e63 686f 6963 6573 280d 0a20 2020  om.choices(..   
-000150a0: 2020 2020 2020 2020 205b 4e6f 6e65 2c20           [None, 
-000150b0: 5b31 5d2c 205b 312c 2037 5d2c 205b 375d  [1], [1, 7], [7]
-000150c0: 2c20 5b73 6561 736f 6e61 6c5f 696e 7428  , [seasonal_int(
-000150d0: 736d 616c 6c3d 5472 7565 295d 5d2c 0d0a  small=True)]],..
-000150e0: 2020 2020 2020 2020 2020 2020 5b30 2e39              [0.9
-000150f0: 2c20 302e 3032 352c 2030 2e30 3235 2c20  , 0.025, 0.025, 
-00015100: 302e 3035 2c20 302e 3035 5d2c 0d0a 2020  0.05, 0.05],..  
-00015110: 2020 2020 2020 295b 305d 0d0a 2020 2020        )[0]..    
-00015120: 2020 2020 6172 5f69 6e74 6572 6163 7469      ar_interacti
-00015130: 6f6e 5f73 6561 736f 6e61 6c69 7479 203d  on_seasonality =
-00015140: 204e 6f6e 650d 0a20 2020 2020 2020 2069   None..        i
-00015150: 6620 6172 5f6c 6167 7320 6973 206e 6f74  f ar_lags is not
-00015160: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00015170: 2020 2020 6172 5f69 6e74 6572 6163 7469      ar_interacti
-00015180: 6f6e 5f73 6561 736f 6e61 6c69 7479 203d  on_seasonality =
-00015190: 2072 616e 646f 6d2e 6368 6f69 6365 7328   random.choices(
-000151a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000151b0: 2020 5b4e 6f6e 652c 2037 2c20 2764 6179    [None, 7, 'day
-000151c0: 6f66 7765 656b 272c 2027 636f 6d6d 6f6e  ofweek', 'common
-000151d0: 5f66 6f75 7269 6572 275d 2c20 5b30 2e34  _fourier'], [0.4
-000151e0: 2c20 302e 322c 2030 2e32 2c20 302e 325d  , 0.2, 0.2, 0.2]
-000151f0: 0d0a 2020 2020 2020 2020 2020 2020 295b  ..            )[
-00015200: 305d 0d0a 2020 2020 2020 2020 7365 6173  0]..        seas
-00015210: 6f6e 616c 6974 6965 7320 3d20 7261 6e64  onalities = rand
-00015220: 6f6d 2e63 686f 6963 6573 280d 0a20 2020  om.choices(..   
-00015230: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
-00015240: 2020 2020 2020 2020 2020 2020 5b37 2c20              [7, 
-00015250: 3336 352e 3235 5d2c 0d0a 2020 2020 2020  365.25],..      
-00015260: 2020 2020 2020 2020 2020 5b22 6461 796f            ["dayo
-00015270: 6677 6565 6b22 2c20 3336 352e 3235 5d2c  fweek", 365.25],
-00015280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015290: 2020 5b22 6d6f 6e74 6822 2c20 2264 6179    ["month", "day
-000152a0: 6f66 7765 656b 222c 2022 7765 656b 6461  ofweek", "weekda
-000152b0: 796f 666d 6f6e 7468 225d 2c0d 0a20 2020  yofmonth"],..   
-000152c0: 2020 2020 2020 2020 2020 2020 205b 2777               ['w
-000152d0: 6565 6b64 6179 6f66 6d6f 6e74 6827 2c20  eekdayofmonth', 
-000152e0: 2763 6f6d 6d6f 6e5f 666f 7572 6965 7227  'common_fourier'
-000152f0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00015300: 2020 2020 226f 7468 6572 222c 0d0a 2020      "other",..  
-00015310: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
-00015320: 2020 2020 2020 2020 2020 5b30 2e31 2c20            [0.1, 
-00015330: 302e 312c 2030 2e31 2c20 302e 3035 2c20  0.1, 0.1, 0.05, 
-00015340: 302e 315d 2c0d 0a20 2020 2020 2020 2029  0.1],..        )
-00015350: 5b30 5d0d 0a20 2020 2020 2020 2069 6620  [0]..        if 
-00015360: 7365 6173 6f6e 616c 6974 6965 7320 3d3d  seasonalities ==
-00015370: 2022 6f74 6865 7222 3a0d 0a20 2020 2020   "other":..     
-00015380: 2020 2020 2020 2070 7265 6465 6669 6e65         predefine
-00015390: 6420 3d20 7261 6e64 6f6d 2e63 686f 6963  d = random.choic
-000153a0: 6573 285b 5472 7565 2c20 4661 6c73 655d  es([True, False]
-000153b0: 2c20 5b30 2e35 2c20 302e 355d 295b 305d  , [0.5, 0.5])[0]
-000153c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000153d0: 2070 7265 6465 6669 6e65 643a 0d0a 2020   predefined:..  
-000153e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000153f0: 6173 6f6e 616c 6974 6965 7320 3d20 7261  asonalities = ra
-00015400: 6e64 6f6d 2e63 686f 6963 6528 6461 7465  ndom.choice(date
-00015410: 5f70 6172 745f 6d65 7468 6f64 7329 0d0a  _part_methods)..
-00015420: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00015430: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00015440: 2020 2063 6f6d 705f 6f70 7473 203d 2064     comp_opts = d
-00015450: 6174 6570 6172 745f 636f 6d70 6f6e 656e  atepart_componen
-00015460: 7473 202b 205b 372c 2033 3635 2e32 352c  ts + [7, 365.25,
-00015470: 2031 325d 0d0a 2020 2020 2020 2020 2020   12]..          
-00015480: 2020 2020 2020 7365 6173 6f6e 616c 6974        seasonalit
-00015490: 6965 7320 3d20 7261 6e64 6f6d 2e63 686f  ies = random.cho
-000154a0: 6963 6573 2863 6f6d 705f 6f70 7473 2c20  ices(comp_opts, 
-000154b0: 6b3d 3229 0d0a 2020 2020 2020 2020 7265  k=2)..        re
-000154c0: 7475 726e 207b 0d0a 2020 2020 2020 2020  turn {..        
-000154d0: 2020 2020 2270 7265 7072 6f63 6573 7369      "preprocessi
-000154e0: 6e67 5f74 7261 6e73 666f 726d 6174 696f  ng_transformatio
-000154f0: 6e22 3a20 5261 6e64 6f6d 5472 616e 7366  n": RandomTransf
-00015500: 6f72 6d28 0d0a 2020 2020 2020 2020 2020  orm(..          
-00015510: 2020 2020 2020 7472 616e 7366 6f72 6d65        transforme
-00015520: 725f 6c69 7374 3d66 696c 7465 7273 2c20  r_list=filters, 
-00015530: 7472 616e 7366 6f72 6d65 725f 6d61 785f  transformer_max_
-00015540: 6465 7074 683d 322c 2061 6c6c 6f77 5f6e  depth=2, allow_n
-00015550: 6f6e 653d 5472 7565 0d0a 2020 2020 2020  one=True..      
-00015560: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
-00015570: 2020 2020 2020 2273 6361 6c69 6e67 223a        "scaling":
-00015580: 2073 6361 6c69 6e67 2c0d 0a20 2020 2020   scaling,..     
-00015590: 2020 2020 2020 2023 2022 7061 7374 5f69         # "past_i
-000155a0: 6d70 6163 7473 5f69 6e74 6572 7665 6e74  mpacts_intervent
-000155b0: 696f 6e22 3a20 7365 6c66 2e70 6173 745f  ion": self.past_
-000155c0: 696d 7061 6374 735f 696e 7465 7276 656e  impacts_interven
-000155d0: 7469 6f6e 2c0d 0a20 2020 2020 2020 2020  tion,..         
-000155e0: 2020 2022 7365 6173 6f6e 616c 6974 6965     "seasonalitie
-000155f0: 7322 3a20 7365 6173 6f6e 616c 6974 6965  s": seasonalitie
-00015600: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-00015610: 2261 725f 6c61 6773 223a 2061 725f 6c61  "ar_lags": ar_la
-00015620: 6773 2c0d 0a20 2020 2020 2020 2020 2020  gs,..           
-00015630: 2022 6172 5f69 6e74 6572 6163 7469 6f6e   "ar_interaction
-00015640: 5f73 6561 736f 6e61 6c69 7479 223a 2061  _seasonality": a
-00015650: 725f 696e 7465 7261 6374 696f 6e5f 7365  r_interaction_se
-00015660: 6173 6f6e 616c 6974 792c 0d0a 2020 2020  asonality,..    
-00015670: 2020 2020 2020 2020 2261 6e6f 6d61 6c79          "anomaly
-00015680: 5f64 6574 6563 746f 725f 7061 7261 6d73  _detector_params
-00015690: 223a 2061 6e6f 6d61 6c79 5f64 6574 6563  ": anomaly_detec
-000156a0: 746f 725f 7061 7261 6d73 2c0d 0a20 2020  tor_params,..   
-000156b0: 2020 2020 2020 2020 2022 616e 6f6d 616c           "anomal
-000156c0: 795f 696e 7465 7276 656e 7469 6f6e 223a  y_intervention":
-000156d0: 2061 6e6f 6d61 6c79 5f69 6e74 6572 7665   anomaly_interve
-000156e0: 6e74 696f 6e2c 0d0a 2020 2020 2020 2020  ntion,..        
-000156f0: 2020 2020 2268 6f6c 6964 6179 5f64 6574      "holiday_det
-00015700: 6563 746f 725f 7061 7261 6d73 223a 2068  ector_params": h
-00015710: 6f6c 6964 6179 5f70 6172 616d 732c 0d0a  oliday_params,..
-00015720: 2020 2020 2020 2020 2020 2020 2320 2268              # "h
-00015730: 6f6c 6964 6179 5f63 6f75 6e74 7269 6573  oliday_countries
-00015740: 223a 2073 656c 662e 686f 6c69 6461 795f  ": self.holiday_
-00015750: 636f 756e 7472 6965 732c 0d0a 2020 2020  countries,..    
-00015760: 2020 2020 2020 2020 2268 6f6c 6964 6179          "holiday
-00015770: 5f63 6f75 6e74 7269 6573 5f75 7365 6422  _countries_used"
-00015780: 3a20 7261 6e64 6f6d 2e63 686f 6963 6573  : random.choices
-00015790: 285b 5472 7565 2c20 4661 6c73 655d 2c20  ([True, False], 
-000157a0: 5b30 2e35 2c20 302e 355d 295b 305d 2c0d  [0.5, 0.5])[0],.
-000157b0: 0a20 2020 2020 2020 2020 2020 2022 6d75  .            "mu
-000157c0: 6c74 6976 6172 6961 7465 5f66 6561 7475  ltivariate_featu
-000157d0: 7265 223a 2072 616e 646f 6d2e 6368 6f69  re": random.choi
-000157e0: 6365 7328 0d0a 2020 2020 2020 2020 2020  ces(..          
-000157f0: 2020 2020 2020 5b4e 6f6e 652c 2022 6665        [None, "fe
-00015800: 6174 7572 655f 6167 676c 6f6d 6572 6174  ature_agglomerat
-00015810: 696f 6e22 2c20 2767 726f 7570 5f61 7665  ion", 'group_ave
-00015820: 7261 6765 272c 2027 6f73 6369 6c6c 6174  rage', 'oscillat
-00015830: 6f72 275d 2c0d 0a20 2020 2020 2020 2020  or'],..         
-00015840: 2020 2020 2020 205b 302e 392c 2030 2e31         [0.9, 0.1
-00015850: 2c20 302e 312c 2030 2e30 5d2c 0d0a 2020  , 0.1, 0.0],..  
-00015860: 2020 2020 2020 2020 2020 295b 305d 2c0d            )[0],.
-00015870: 0a20 2020 2020 2020 2020 2020 2022 6d75  .            "mu
-00015880: 6c74 6976 6172 6961 7465 5f74 7261 6e73  ltivariate_trans
-00015890: 666f 726d 6174 696f 6e22 3a20 5261 6e64  formation": Rand
-000158a0: 6f6d 5472 616e 7366 6f72 6d28 0d0a 2020  omTransform(..  
-000158b0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000158c0: 616e 7366 6f72 6d65 725f 6c69 7374 3d22  ansformer_list="
-000158d0: 6661 7374 222c 0d0a 2020 2020 2020 2020  fast",..        
-000158e0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
-000158f0: 6d65 725f 6d61 785f 6465 7074 683d 332c  mer_max_depth=3,
-00015900: 2020 2320 7072 6f62 6162 6c79 2077 616e    # probably wan
-00015910: 7420 736f 6d65 206d 6f72 6520 7573 6162  t some more usab
-00015920: 6c65 2064 6566 6175 6c74 7320 6669 7273  le defaults firs
-00015930: 7420 6173 206d 616e 7920 7261 6e64 6f6d  t as many random
-00015940: 2061 7265 2073 656e 7365 6c65 7373 0d0a   are senseless..
-00015950: 2020 2020 2020 2020 2020 2020 292c 0d0a              ),..
-00015960: 2020 2020 2020 2020 2020 2020 2272 6567              "reg
-00015970: 7265 7373 6f72 5f74 7261 6e73 666f 726d  ressor_transform
-00015980: 6174 696f 6e22 3a20 5261 6e64 6f6d 5472  ation": RandomTr
-00015990: 616e 7366 6f72 6d28 0d0a 2020 2020 2020  ansform(..      
-000159a0: 2020 2020 2020 2020 2020 7472 616e 7366            transf
-000159b0: 6f72 6d65 725f 6c69 7374 3d7b 2a2a 7363  ormer_list={**sc
-000159c0: 616c 6572 732c 202a 2a64 6563 6f6d 706f  alers, **decompo
-000159d0: 7369 7469 6f6e 737d 2c0d 0a20 2020 2020  sitions},..     
-000159e0: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-000159f0: 666f 726d 6572 5f6d 6178 5f64 6570 7468  former_max_depth
-00015a00: 3d31 2c0d 0a20 2020 2020 2020 2020 2020  =1,..           
-00015a10: 2020 2020 2061 6c6c 6f77 5f6e 6f6e 653d       allow_none=
-00015a20: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-00015a30: 2020 2020 2020 2020 6e6f 5f6e 616e 5f66          no_nan_f
-00015a40: 696c 6c3d 4661 6c73 652c 2020 2320 7072  ill=False,  # pr
-00015a50: 6f62 6162 6c79 2077 616e 7420 736f 6d65  obably want some
-00015a60: 206d 6f72 6520 7573 6162 6c65 2064 6566   more usable def
-00015a70: 6175 6c74 7320 6669 7273 7420 6173 206d  aults first as m
-00015a80: 616e 7920 7261 6e64 6f6d 2061 7265 2073  any random are s
-00015a90: 656e 7365 6c65 7373 0d0a 2020 2020 2020  enseless..      
-00015aa0: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
-00015ab0: 2020 2020 2020 2272 6567 7265 7373 6f72        "regressor
-00015ac0: 735f 7573 6564 223a 2072 6567 7265 7373  s_used": regress
-00015ad0: 6f72 735f 7573 6564 2c0d 0a20 2020 2020  ors_used,..     
-00015ae0: 2020 2020 2020 2022 6c69 6e65 6172 5f6d         "linear_m
-00015af0: 6f64 656c 223a 206c 696e 6561 725f 6d6f  odel": linear_mo
-00015b00: 6465 6c2c 0d0a 2020 2020 2020 2020 2020  del,..          
-00015b10: 2020 2272 616e 646f 6d77 616c 6b5f 6e22    "randomwalk_n"
-00015b20: 3a20 7261 6e64 6f6d 2e63 686f 6963 6573  : random.choices
-00015b30: 285b 4e6f 6e65 2c20 3130 5d2c 205b 302e  ([None, 10], [0.
-00015b40: 352c 2030 2e35 5d29 5b30 5d2c 0d0a 2020  5, 0.5])[0],..  
-00015b50: 2020 2020 2020 2020 2020 2274 7265 6e64            "trend
-00015b60: 5f77 696e 646f 7722 3a20 7261 6e64 6f6d  _window": random
-00015b70: 2e63 686f 6963 6573 285b 332c 2031 352c  .choices([3, 15,
-00015b80: 2039 302c 2033 3635 5d2c 205b 302e 322c   90, 365], [0.2,
-00015b90: 2030 2e32 2c20 302e 322c 2030 2e32 5d29   0.2, 0.2, 0.2])
-00015ba0: 5b30 5d2c 0d0a 2020 2020 2020 2020 2020  [0],..          
-00015bb0: 2020 2274 7265 6e64 5f73 7461 6e64 696e    "trend_standin
-00015bc0: 223a 2072 616e 646f 6d2e 6368 6f69 6365  ": random.choice
-00015bd0: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
-00015be0: 2020 2020 5b4e 6f6e 652c 2027 7261 6e64      [None, 'rand
-00015bf0: 6f6d 5f6e 6f72 6d61 6c27 2c20 2772 6f6c  om_normal', 'rol
-00015c00: 6c69 6e67 5f74 7265 6e64 275d 2c0d 0a20  ling_trend'],.. 
-00015c10: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00015c20: 302e 352c 2030 2e34 2c20 302e 315d 2c0d  0.5, 0.4, 0.1],.
-00015c30: 0a20 2020 2020 2020 2020 2020 2029 5b30  .            )[0
-00015c40: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00015c50: 2274 7265 6e64 5f61 6e6f 6d61 6c79 5f64  "trend_anomaly_d
-00015c60: 6574 6563 746f 725f 7061 7261 6d73 223a  etector_params":
-00015c70: 2074 7265 6e64 5f61 6e6f 6d61 6c79 5f64   trend_anomaly_d
-00015c80: 6574 6563 746f 725f 7061 7261 6d73 2c0d  etector_params,.
-00015c90: 0a20 2020 2020 2020 2020 2020 2023 2022  .            # "
-00015ca0: 7472 656e 645f 616e 6f6d 616c 795f 696e  trend_anomaly_in
-00015cb0: 7465 7276 656e 7469 6f6e 223a 2074 7265  tervention": tre
-00015cc0: 6e64 5f61 6e6f 6d61 6c79 5f69 6e74 6572  nd_anomaly_inter
-00015cd0: 7665 6e74 696f 6e2c 0d0a 2020 2020 2020  vention,..      
-00015ce0: 2020 2020 2020 2274 7265 6e64 5f74 7261        "trend_tra
-00015cf0: 6e73 666f 726d 6174 696f 6e22 3a20 7472  nsformation": tr
-00015d00: 656e 645f 7472 616e 7366 6f72 6d61 7469  end_transformati
-00015d10: 6f6e 2c0d 0a20 2020 2020 2020 2020 2020  on,..           
-00015d20: 2022 7472 656e 645f 6d6f 6465 6c22 3a20   "trend_model": 
-00015d30: 7472 656e 645f 6d6f 6465 6c2c 0d0a 2020  trend_model,..  
-00015d40: 2020 2020 2020 2020 2020 2274 7265 6e64            "trend
-00015d50: 5f70 6869 223a 2072 616e 646f 6d2e 6368  _phi": random.ch
-00015d60: 6f69 6365 7328 5b4e 6f6e 652c 2030 2e39  oices([None, 0.9
-00015d70: 385d 2c20 5b30 2e39 2c20 302e 315d 295b  8], [0.9, 0.1])[
-00015d80: 305d 2c0d 0a20 2020 2020 2020 207d 0d0a  0],..        }..
-00015d90: 0d0a 2020 2020 6465 6620 6765 745f 7061  ..    def get_pa
-00015da0: 7261 6d73 2873 656c 6629 3a0d 0a20 2020  rams(self):..   
-00015db0: 2020 2020 2072 6574 7572 6e20 7b0d 0a20       return {.. 
-00015dc0: 2020 2020 2020 2020 2020 2022 7072 6570             "prep
-00015dd0: 726f 6365 7373 696e 675f 7472 616e 7366  rocessing_transf
-00015de0: 6f72 6d61 7469 6f6e 223a 2073 656c 662e  ormation": self.
-00015df0: 7072 6570 726f 6365 7373 696e 675f 7472  preprocessing_tr
-00015e00: 616e 7366 6f72 6d61 7469 6f6e 2c0d 0a20  ansformation,.. 
-00015e10: 2020 2020 2020 2020 2020 2022 7363 616c             "scal
-00015e20: 696e 6722 3a20 7365 6c66 2e73 6361 6c69  ing": self.scali
-00015e30: 6e67 2c0d 0a20 2020 2020 2020 2020 2020  ng,..           
-00015e40: 2022 7061 7374 5f69 6d70 6163 7473 5f69   "past_impacts_i
-00015e50: 6e74 6572 7665 6e74 696f 6e22 3a20 7365  ntervention": se
-00015e60: 6c66 2e70 6173 745f 696d 7061 6374 735f  lf.past_impacts_
-00015e70: 696e 7465 7276 656e 7469 6f6e 2c20 2023  intervention,  #
-00015e80: 206e 6f74 2069 6e20 6e65 770d 0a20 2020   not in new..   
-00015e90: 2020 2020 2020 2020 2022 7365 6173 6f6e           "season
-00015ea0: 616c 6974 6965 7322 3a20 7365 6c66 2e73  alities": self.s
-00015eb0: 6561 736f 6e61 6c69 7469 6573 2c0d 0a20  easonalities,.. 
-00015ec0: 2020 2020 2020 2020 2020 2022 6172 5f6c             "ar_l
-00015ed0: 6167 7322 3a20 7365 6c66 2e61 725f 6c61  ags": self.ar_la
-00015ee0: 6773 2c0d 0a20 2020 2020 2020 2020 2020  gs,..           
-00015ef0: 2022 6172 5f69 6e74 6572 6163 7469 6f6e   "ar_interaction
-00015f00: 5f73 6561 736f 6e61 6c69 7479 223a 2073  _seasonality": s
-00015f10: 656c 662e 6172 5f69 6e74 6572 6163 7469  elf.ar_interacti
-00015f20: 6f6e 5f73 6561 736f 6e61 6c69 7479 0d0a  on_seasonality..
-00015f30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00015f40: 656c 662e 6172 5f6c 6167 7320 6973 206e  elf.ar_lags is n
-00015f50: 6f74 204e 6f6e 650d 0a20 2020 2020 2020  ot None..       
-00015f60: 2020 2020 2065 6c73 6520 4e6f 6e65 2c0d       else None,.
-00015f70: 0a20 2020 2020 2020 2020 2020 2022 616e  .            "an
-00015f80: 6f6d 616c 795f 6465 7465 6374 6f72 5f70  omaly_detector_p
-00015f90: 6172 616d 7322 3a20 7365 6c66 2e61 6e6f  arams": self.ano
-00015fa0: 6d61 6c79 5f64 6574 6563 746f 725f 7061  maly_detector_pa
-00015fb0: 7261 6d73 2c0d 0a20 2020 2020 2020 2020  rams,..         
-00015fc0: 2020 2022 616e 6f6d 616c 795f 696e 7465     "anomaly_inte
-00015fd0: 7276 656e 7469 6f6e 223a 2073 656c 662e  rvention": self.
-00015fe0: 616e 6f6d 616c 795f 696e 7465 7276 656e  anomaly_interven
-00015ff0: 7469 6f6e 2c0d 0a20 2020 2020 2020 2020  tion,..         
-00016000: 2020 2022 686f 6c69 6461 795f 6465 7465     "holiday_dete
-00016010: 6374 6f72 5f70 6172 616d 7322 3a20 7365  ctor_params": se
-00016020: 6c66 2e68 6f6c 6964 6179 5f64 6574 6563  lf.holiday_detec
-00016030: 746f 725f 7061 7261 6d73 2c0d 0a20 2020  tor_params,..   
-00016040: 2020 2020 2020 2020 2023 2022 686f 6c69           # "holi
-00016050: 6461 795f 696e 7465 7276 656e 7469 6f6e  day_intervention
-00016060: 223a 2073 656c 662e 686f 6c69 6461 795f  ": self.holiday_
-00016070: 696e 7465 7276 656e 7469 6f6e 2c0d 0a20  intervention,.. 
-00016080: 2020 2020 2020 2020 2020 2023 2022 686f             # "ho
-00016090: 6c69 6461 795f 636f 756e 7472 6965 7322  liday_countries"
-000160a0: 3a20 7365 6c66 2e68 6f6c 6964 6179 5f63  : self.holiday_c
-000160b0: 6f75 6e74 7269 6573 2c0d 0a20 2020 2020  ountries,..     
-000160c0: 2020 2020 2020 2022 686f 6c69 6461 795f         "holiday_
-000160d0: 636f 756e 7472 6965 735f 7573 6564 223a  countries_used":
-000160e0: 2073 656c 662e 686f 6c69 6461 795f 636f   self.holiday_co
-000160f0: 756e 7472 6965 735f 7573 6564 2c0d 0a20  untries_used,.. 
-00016100: 2020 2020 2020 2020 2020 2022 6d75 6c74             "mult
-00016110: 6976 6172 6961 7465 5f66 6561 7475 7265  ivariate_feature
-00016120: 223a 2073 656c 662e 6d75 6c74 6976 6172  ": self.multivar
-00016130: 6961 7465 5f66 6561 7475 7265 2c0d 0a20  iate_feature,.. 
-00016140: 2020 2020 2020 2020 2020 2022 6d75 6c74             "mult
-00016150: 6976 6172 6961 7465 5f74 7261 6e73 666f  ivariate_transfo
-00016160: 726d 6174 696f 6e22 3a20 7365 6c66 2e6d  rmation": self.m
-00016170: 756c 7469 7661 7269 6174 655f 7472 616e  ultivariate_tran
-00016180: 7366 6f72 6d61 7469 6f6e 0d0a 2020 2020  sformation..    
-00016190: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000161a0: 6d75 6c74 6976 6172 6961 7465 5f66 6561  multivariate_fea
-000161b0: 7475 7265 2069 7320 6e6f 7420 4e6f 6e65  ture is not None
-000161c0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-000161d0: 7365 204e 6f6e 652c 0d0a 2020 2020 2020  se None,..      
-000161e0: 2020 2020 2020 2272 6567 7265 7373 6f72        "regressor
-000161f0: 5f74 7261 6e73 666f 726d 6174 696f 6e22  _transformation"
-00016200: 3a20 7365 6c66 2e72 6567 7265 7373 6f72  : self.regressor
-00016210: 5f74 7261 6e73 666f 726d 6174 696f 6e0d  _transformation.
-00016220: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00016230: 7365 6c66 2e72 6567 7265 7373 6f72 735f  self.regressors_
-00016240: 7573 6564 0d0a 2020 2020 2020 2020 2020  used..          
-00016250: 2020 656c 7365 204e 6f6e 652c 0d0a 2020    else None,..  
-00016260: 2020 2020 2020 2020 2020 2272 6567 7265            "regre
-00016270: 7373 6f72 735f 7573 6564 223a 2073 656c  ssors_used": sel
-00016280: 662e 7265 6772 6573 736f 7273 5f75 7365  f.regressors_use
-00016290: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-000162a0: 226c 696e 6561 725f 6d6f 6465 6c22 3a20  "linear_model": 
-000162b0: 7365 6c66 2e6c 696e 6561 725f 6d6f 6465  self.linear_mode
-000162c0: 6c2c 0d0a 2020 2020 2020 2020 2020 2020  l,..            
-000162d0: 2272 616e 646f 6d77 616c 6b5f 6e22 3a20  "randomwalk_n": 
-000162e0: 7365 6c66 2e72 616e 646f 6d77 616c 6b5f  self.randomwalk_
-000162f0: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
-00016300: 2274 7265 6e64 5f77 696e 646f 7722 3a20  "trend_window": 
-00016310: 7365 6c66 2e74 7265 6e64 5f77 696e 646f  self.trend_windo
-00016320: 772c 0d0a 2020 2020 2020 2020 2020 2020  w,..            
-00016330: 2274 7265 6e64 5f73 7461 6e64 696e 223a  "trend_standin":
-00016340: 2073 656c 662e 7472 656e 645f 7374 616e   self.trend_stan
-00016350: 6469 6e2c 0d0a 2020 2020 2020 2020 2020  din,..          
-00016360: 2020 2274 7265 6e64 5f61 6e6f 6d61 6c79    "trend_anomaly
-00016370: 5f64 6574 6563 746f 725f 7061 7261 6d73  _detector_params
-00016380: 223a 2073 656c 662e 7472 656e 645f 616e  ": self.trend_an
-00016390: 6f6d 616c 795f 6465 7465 6374 6f72 5f70  omaly_detector_p
-000163a0: 6172 616d 732c 0d0a 2020 2020 2020 2020  arams,..        
-000163b0: 2020 2020 2320 2274 7265 6e64 5f61 6e6f      # "trend_ano
-000163c0: 6d61 6c79 5f69 6e74 6572 7665 6e74 696f  maly_interventio
-000163d0: 6e22 3a20 7365 6c66 2e74 7265 6e64 5f61  n": self.trend_a
-000163e0: 6e6f 6d61 6c79 5f69 6e74 6572 7665 6e74  nomaly_intervent
-000163f0: 696f 6e2c 0d0a 2020 2020 2020 2020 2020  ion,..          
-00016400: 2020 2274 7265 6e64 5f74 7261 6e73 666f    "trend_transfo
-00016410: 726d 6174 696f 6e22 3a20 7365 6c66 2e74  rmation": self.t
-00016420: 7265 6e64 5f74 7261 6e73 666f 726d 6174  rend_transformat
-00016430: 696f 6e2c 0d0a 2020 2020 2020 2020 2020  ion,..          
-00016440: 2020 2274 7265 6e64 5f6d 6f64 656c 223a    "trend_model":
-00016450: 2073 656c 662e 7472 656e 645f 6d6f 6465   self.trend_mode
-00016460: 6c2c 0d0a 2020 2020 2020 2020 2020 2020  l,..            
-00016470: 2274 7265 6e64 5f70 6869 223a 2073 656c  "trend_phi": sel
-00016480: 662e 7472 656e 645f 7068 692c 0d0a 2020  f.trend_phi,..  
-00016490: 2020 2020 2020 2020 2020 2320 2263 6f6e            # "con
-000164a0: 7374 7261 696e 7422 3a20 7365 6c66 2e63  straint": self.c
-000164b0: 6f6e 7374 7261 696e 742c 0d0a 2020 2020  onstraint,..    
-000164c0: 2020 2020 7d0d 0a0d 0a20 2020 2064 6566      }....    def
-000164d0: 2070 6c6f 745f 636f 6d70 6f6e 656e 7473   plot_components
-000164e0: 280d 0a20 2020 2020 2020 2073 656c 662c  (..        self,
-000164f0: 0d0a 2020 2020 2020 2020 7072 6564 6963  ..        predic
-00016500: 7469 6f6e 3d4e 6f6e 652c 0d0a 2020 2020  tion=None,..    
-00016510: 2020 2020 7365 7269 6573 3d4e 6f6e 652c      series=None,
-00016520: 0d0a 2020 2020 2020 2020 6669 6773 697a  ..        figsiz
-00016530: 653d 2831 362c 2039 292c 0d0a 2020 2020  e=(16, 9),..    
-00016540: 2020 2020 746f 5f6f 7269 6769 6e5f 7370      to_origin_sp
-00016550: 6163 653d 5472 7565 2c0d 0a20 2020 2020  ace=True,..     
-00016560: 2020 2074 6974 6c65 3d4e 6f6e 652c 0d0a     title=None,..
-00016570: 2020 2020 2020 2020 7374 6172 745f 6461          start_da
-00016580: 7465 3d4e 6f6e 652c 0d0a 2020 2020 293a  te=None,..    ):
-00016590: 0d0a 2020 2020 2020 2020 6966 2073 6572  ..        if ser
-000165a0: 6965 7320 6973 204e 6f6e 653a 0d0a 2020  ies is None:..  
-000165b0: 2020 2020 2020 2020 2020 7365 7269 6573            series
-000165c0: 203d 2072 616e 646f 6d2e 6368 6f69 6365   = random.choice
-000165d0: 2873 656c 662e 636f 6c75 6d6e 5f6e 616d  (self.column_nam
-000165e0: 6573 290d 0a20 2020 2020 2020 2069 6620  es)..        if 
-000165f0: 7469 746c 6520 6973 204e 6f6e 653a 0d0a  title is None:..
-00016600: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-00016610: 6520 3d20 6622 4d6f 6465 6c20 436f 6d70  e = f"Model Comp
-00016620: 6f6e 656e 7473 2066 6f72 207b 7365 7269  onents for {seri
-00016630: 6573 7d22 0d0a 2020 2020 2020 2020 706c  es}"..        pl
-00016640: 6f74 5f6c 6973 7420 3d20 5b5d 0d0a 2020  ot_list = []..  
-00016650: 2020 2020 2020 6966 2070 7265 6469 6374        if predict
-00016660: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-00016670: 0d0a 2020 2020 2020 2020 2020 2020 706c  ..            pl
-00016680: 6f74 5f6c 6973 742e 6170 7065 6e64 2870  ot_list.append(p
-00016690: 7265 6469 6374 696f 6e2e 666f 7265 6361  rediction.foreca
-000166a0: 7374 5b73 6572 6965 735d 2e72 656e 616d  st[series].renam
-000166b0: 6528 2266 6f72 6563 6173 7422 2929 0d0a  e("forecast"))..
-000166c0: 2020 2020 2020 2020 2020 2020 706c 745f              plt_
-000166d0: 6964 7820 3d20 7072 6564 6963 7469 6f6e  idx = prediction
-000166e0: 2e66 6f72 6563 6173 742e 696e 6465 780d  .forecast.index.
-000166f0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00016700: 2020 2020 2020 2020 2020 2020 706c 745f              plt_
-00016710: 6964 7820 3d20 4e6f 6e65 0d0a 2020 2020  idx = None..    
-00016720: 2020 2020 706c 6f74 5f6c 6973 742e 6170      plot_list.ap
-00016730: 7065 6e64 2873 656c 662e 7072 6564 6963  pend(self.predic
-00016740: 7465 645f 7472 656e 645b 7365 7269 6573  ted_trend[series
-00016750: 5d2e 7265 6e61 6d65 2822 7472 656e 6422  ].rename("trend"
-00016760: 2929 0d0a 2020 2020 2020 2020 6966 2073  ))..        if s
-00016770: 656c 662e 696d 7061 6374 7320 6973 206e  elf.impacts is n
-00016780: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00016790: 2020 2020 2020 706c 6f74 5f6c 6973 742e        plot_list.
-000167a0: 6170 7065 6e64 2828 7365 6c66 2e69 6d70  append((self.imp
-000167b0: 6163 7473 5b73 6572 6965 735d 2e72 656e  acts[series].ren
-000167c0: 616d 6528 2269 6d70 6163 7420 2522 2920  ame("impact %") 
-000167d0: 2d20 312e 3029 202a 2031 3030 290d 0a20  - 1.0) * 100).. 
-000167e0: 2020 2020 2020 2069 6620 706c 745f 6964         if plt_id
-000167f0: 7820 6973 204e 6f6e 653a 0d0a 2020 2020  x is None:..    
-00016800: 2020 2020 2020 2020 706c 6f74 5f6c 6973          plot_lis
-00016810: 742e 6170 7065 6e64 280d 0a20 2020 2020  t.append(..     
-00016820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016830: 7072 6f63 6573 735f 636f 6d70 6f6e 656e  process_componen
-00016840: 7473 2874 6f5f 6f72 6967 696e 5f73 7061  ts(to_origin_spa
-00016850: 6365 3d74 6f5f 6f72 6967 696e 5f73 7061  ce=to_origin_spa
-00016860: 6365 295b 7365 7269 6573 5d0d 0a20 2020  ce)[series]..   
-00016870: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00016880: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00016890: 2020 2020 2020 2070 6c6f 745f 6c69 7374         plot_list
-000168a0: 2e61 7070 656e 6428 0d0a 2020 2020 2020  .append(..      
-000168b0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000168c0: 726f 6365 7373 5f63 6f6d 706f 6e65 6e74  rocess_component
-000168d0: 7328 746f 5f6f 7269 6769 6e5f 7370 6163  s(to_origin_spac
-000168e0: 653d 746f 5f6f 7269 6769 6e5f 7370 6163  e=to_origin_spac
-000168f0: 6529 5b73 6572 6965 735d 2e6c 6f63 5b0d  e)[series].loc[.
-00016900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016910: 2020 2020 2070 6c74 5f69 6478 0d0a 2020       plt_idx..  
-00016920: 2020 2020 2020 2020 2020 2020 2020 5d0d                ].
-00016930: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
-00016940: 2020 2020 2020 2020 706c 6f74 5f64 6620          plot_df 
-00016950: 3d20 7064 2e63 6f6e 6361 7428 706c 6f74  = pd.concat(plot
-00016960: 5f6c 6973 742c 2061 7869 733d 3129 0d0a  _list, axis=1)..
-00016970: 2020 2020 2020 2020 6966 2073 7461 7274          if start
-00016980: 5f64 6174 6520 6973 206e 6f74 204e 6f6e  _date is not Non
-00016990: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000169a0: 706c 6f74 5f64 6620 3d20 706c 6f74 5f64  plot_df = plot_d
-000169b0: 665b 706c 6f74 5f64 662e 696e 6465 7820  f[plot_df.index 
-000169c0: 3e3d 2073 7461 7274 5f64 6174 655d 0d0a  >= start_date]..
-000169d0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-000169e0: 6c6f 745f 6466 2e70 6c6f 7428 7375 6270  lot_df.plot(subp
-000169f0: 6c6f 7473 3d54 7275 652c 2066 6967 7369  lots=True, figsi
-00016a00: 7a65 3d66 6967 7369 7a65 2c20 7469 746c  ze=figsize, titl
-00016a10: 653d 7469 746c 6529 0d0a 0d0a 2020 2020  e=title)....    
-00016a20: 6465 6620 7265 7475 726e 5f63 6f6d 706f  def return_compo
-00016a30: 6e65 6e74 7328 7365 6c66 2c20 746f 5f6f  nents(self, to_o
-00016a40: 7269 6769 6e5f 7370 6163 653d 5472 7565  rigin_space=True
-00016a50: 2c20 696e 636c 7564 655f 696d 7061 6374  , include_impact
-00016a60: 733d 4661 6c73 6529 3a0d 0a20 2020 2020  s=False):..     
-00016a70: 2020 2022 2222 5265 7475 726e 2061 6464     """Return add
-00016a80: 6974 6976 6520 656c 656d 656e 7473 206f  itive elements o
-00016a90: 6620 666f 7265 6361 7374 2c20 6c69 6e65  f forecast, line
-00016aa0: 6172 2061 6e64 2074 7265 6e64 2e20 4966  ar and trend. If
-00016ab0: 2069 6d70 6163 7473 2069 6e63 6c75 6465   impacts include
-00016ac0: 642c 2069 7420 6973 2061 206d 756c 7469  d, it is a multi
-00016ad0: 706c 6963 6174 6976 6520 7465 726d 2e0d  plicative term..
-00016ae0: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00016af0: 0d0a 2020 2020 2020 2020 2020 2020 746f  ..            to
-00016b00: 5f6f 7269 6769 6e5f 7370 6163 6520 2862  _origin_space (b
-00016b10: 6f6f 6c29 2069 6620 4661 6c73 652c 2077  ool) if False, w
-00016b20: 696c 6c20 6e6f 7420 7265 7665 7273 6520  ill not reverse 
-00016b30: 7472 616e 7366 6f72 6d20 6c69 6e65 6172  transform linear
-00016b40: 2063 6f6d 706f 6e65 6e74 730d 0a20 2020   components..   
-00016b50: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
-00016b60: 5f69 6d70 6163 7473 2028 626f 6f6c 2920  _impacts (bool) 
-00016b70: 6966 2054 7275 652c 2069 6d70 6163 7473  if True, impacts
-00016b80: 2061 7265 2069 6e63 6c75 6465 6420 696e   are included in
-00016b90: 2074 6865 2072 6574 7572 6e65 6420 6461   the returned da
-00016ba0: 7461 6672 616d 650d 0a20 2020 2020 2020  taframe..       
-00016bb0: 2022 2222 0d0a 2020 2020 2020 2020 706c   """..        pl
-00016bc0: 6f74 5f6c 6973 7420 3d20 5b5d 0d0a 2020  ot_list = []..  
-00016bd0: 2020 2020 2020 706c 6f74 5f6c 6973 742e        plot_list.
-00016be0: 6170 7065 6e64 2873 656c 662e 7072 6f63  append(self.proc
-00016bf0: 6573 735f 636f 6d70 6f6e 656e 7473 2874  ess_components(t
-00016c00: 6f5f 6f72 6967 696e 5f73 7061 6365 3d74  o_origin_space=t
-00016c10: 6f5f 6f72 6967 696e 5f73 7061 6365 2929  o_origin_space))
-00016c20: 0d0a 2020 2020 2020 2020 7472 656e 6420  ..        trend 
-00016c30: 3d20 7365 6c66 2e70 7265 6469 6374 6564  = self.predicted
-00016c40: 5f74 7265 6e64 2e63 6f70 7928 290d 0a20  _trend.copy().. 
-00016c50: 2020 2020 2020 2074 7265 6e64 2e63 6f6c         trend.col
-00016c60: 756d 6e73 203d 2070 642e 4d75 6c74 6949  umns = pd.MultiI
-00016c70: 6e64 6578 2e66 726f 6d5f 6172 7261 7973  ndex.from_arrays
-00016c80: 280d 0a20 2020 2020 2020 2020 2020 205b  (..            [
-00016c90: 7472 656e 642e 636f 6c75 6d6e 732c 205b  trend.columns, [
-00016ca0: 2774 7265 6e64 275d 202a 206c 656e 2874  'trend'] * len(t
-00016cb0: 7265 6e64 2e63 6f6c 756d 6e73 295d 0d0a  rend.columns)]..
-00016cc0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00016cd0: 2020 2070 6c6f 745f 6c69 7374 2e61 7070     plot_list.app
-00016ce0: 656e 6428 7472 656e 6429 0d0a 2020 2020  end(trend)..    
-00016cf0: 2020 2020 6966 2073 656c 662e 696d 7061      if self.impa
-00016d00: 6374 7320 6973 206e 6f74 204e 6f6e 6520  cts is not None 
-00016d10: 616e 6420 696e 636c 7564 655f 696d 7061  and include_impa
-00016d20: 6374 733a 0d0a 2020 2020 2020 2020 2020  cts:..          
-00016d30: 2020 696d 7061 6374 7320 3d20 7365 6c66    impacts = self
-00016d40: 2e69 6d70 6163 7473 2e63 6f70 7928 290d  .impacts.copy().
-00016d50: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
-00016d60: 6163 7473 2e63 6f6c 756d 6e73 203d 2070  acts.columns = p
-00016d70: 642e 4d75 6c74 6949 6e64 6578 2e66 726f  d.MultiIndex.fro
-00016d80: 6d5f 6172 7261 7973 280d 0a20 2020 2020  m_arrays(..     
-00016d90: 2020 2020 2020 2020 2020 205b 696d 7061             [impa
-00016da0: 6374 732e 636f 6c75 6d6e 732c 205b 2769  cts.columns, ['i
-00016db0: 6d70 6163 7473 275d 202a 206c 656e 2869  mpacts'] * len(i
-00016dc0: 6d70 6163 7473 2e63 6f6c 756d 6e73 295d  mpacts.columns)]
-00016dd0: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
-00016de0: 0a20 2020 2020 2020 2020 2020 2070 6c6f  .            plo
-00016df0: 745f 6c69 7374 2e61 7070 656e 6428 696d  t_list.append(im
-00016e00: 7061 6374 7329 0d0a 2020 2020 2020 2020  pacts)..        
-00016e10: 7265 7475 726e 2070 642e 636f 6e63 6174  return pd.concat
-00016e20: 2870 6c6f 745f 6c69 7374 2c20 6178 6973  (plot_list, axis
-00016e30: 3d31 290d 0a0d 0a20 2020 2064 6566 2070  =1)....    def p
-00016e40: 6c6f 745f 7472 656e 6428 0d0a 2020 2020  lot_trend(..    
-00016e50: 2020 2020 7365 6c66 2c0d 0a20 2020 2020      self,..     
-00016e60: 2020 2073 6572 6965 733d 4e6f 6e65 2c0d     series=None,.
-00016e70: 0a20 2020 2020 2020 2076 6c69 6e65 3d4e  .        vline=N
-00016e80: 6f6e 652c 0d0a 2020 2020 2020 2020 636f  one,..        co
-00016e90: 6c6f 7273 3d5b 2223 6434 6637 3466 222c  lors=["#d4f74f",
-00016ea0: 2022 2338 3261 6235 6122 2c20 2223 6666   "#82ab5a", "#ff
-00016eb0: 3663 3035 222c 2022 2363 3132 3630 3022  6c05", "#c12600"
-00016ec0: 5d2c 0d0a 2020 2020 2020 2020 7469 746c  ],..        titl
-00016ed0: 653d 4e6f 6e65 2c0d 0a20 2020 2020 2020  e=None,..       
-00016ee0: 2073 7461 7274 5f64 6174 653d 4e6f 6e65   start_date=None
-00016ef0: 2c0d 0a20 2020 2020 2020 202a 2a6b 7761  ,..        **kwa
-00016f00: 7267 732c 0d0a 2020 2020 293a 0d0a 2020  rgs,..    ):..  
-00016f10: 2020 2020 2020 2320 594d 4158 2066 726f        # YMAX fro
-00016f20: 6d20 504c 4f54 204f 4e4c 590d 0a20 2020  m PLOT ONLY..   
-00016f30: 2020 2020 2069 6620 7365 7269 6573 2069       if series i
-00016f40: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00016f50: 2020 2020 2073 6572 6965 7320 3d20 7261       series = ra
-00016f60: 6e64 6f6d 2e63 686f 6963 6528 7365 6c66  ndom.choice(self
-00016f70: 2e63 6f6c 756d 6e5f 6e61 6d65 7329 0d0a  .column_names)..
-00016f80: 2020 2020 2020 2020 6966 2074 6974 6c65          if title
-00016f90: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00016fa0: 2020 2020 2020 2074 6974 6c65 203d 2066         title = f
-00016fb0: 2254 7265 6e64 2042 7265 616b 646f 776e  "Trend Breakdown
-00016fc0: 2066 6f72 207b 7365 7269 6573 7d22 0d0a   for {series}"..
-00016fd0: 2020 2020 2020 2020 705f 696e 6478 203d          p_indx =
-00016fe0: 2073 656c 662e 636f 6c75 6d6e 5f6e 616d   self.column_nam
-00016ff0: 6573 2e67 6574 5f6c 6f63 2873 6572 6965  es.get_loc(serie
-00017000: 7329 0d0a 2020 2020 2020 2020 6375 725f  s)..        cur_
-00017010: 7472 656e 6420 3d20 7365 6c66 2e70 7265  trend = self.pre
-00017020: 6469 6374 6564 5f74 7265 6e64 5b73 6572  dicted_trend[ser
-00017030: 6965 735d 2e63 6f70 7928 290d 0a20 2020  ies].copy()..   
-00017040: 2020 2020 2074 6c73 203d 206c 656e 2863       tls = len(c
-00017050: 7572 5f74 7265 6e64 290d 0a20 2020 2020  ur_trend)..     
-00017060: 2020 2070 6c6f 745f 6466 203d 2070 642e     plot_df = pd.
-00017070: 4461 7461 4672 616d 6528 0d0a 2020 2020  DataFrame(..    
-00017080: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-00017090: 2020 2020 2020 2020 2020 2027 6465 636c             'decl
-000170a0: 696e 655f 6163 6365 6c65 7261 7469 6e67  ine_accelerating
-000170b0: 273a 2063 7572 5f74 7265 6e64 5b0d 0a20  ': cur_trend[.. 
-000170c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170d0: 2020 2028 0d0a 2020 2020 2020 2020 2020     (..          
-000170e0: 2020 2020 2020 2020 2020 2020 2020 6e70                np
-000170f0: 2e68 7374 6163 6b28 286e 702e 7369 676e  .hstack((np.sign
-00017100: 6269 7428 7365 6c66 2e61 6363 656c 5b3a  bit(self.accel[:
-00017110: 2c20 705f 696e 6478 5d29 2c20 4661 6c73  , p_indx]), Fals
-00017120: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
-00017130: 2020 2020 2020 2020 2020 2020 2026 2073               & s
-00017140: 656c 662e 736c 6f70 655f 7369 676e 5b3a  elf.slope_sign[:
-00017150: 2c20 705f 696e 6478 5d0d 0a20 2020 2020  , p_indx]..     
-00017160: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00017170: 5b2d 746c 733a 5d0d 0a20 2020 2020 2020  [-tls:]..       
-00017180: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00017190: 2020 2020 2020 2020 2020 2020 2027 6465               'de
-000171a0: 636c 696e 655f 6465 6365 6c65 7261 7469  cline_decelerati
-000171b0: 6e67 273a 2063 7572 5f74 7265 6e64 5b0d  ng': cur_trend[.
-000171c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000171d0: 2020 2020 2028 0d0a 2020 2020 2020 2020       (..        
-000171e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171f0: 287e 6e70 2e68 7374 6163 6b28 286e 702e  (~np.hstack((np.
-00017200: 7369 676e 6269 7428 7365 6c66 2e61 6363  signbit(self.acc
-00017210: 656c 5b3a 2c20 705f 696e 6478 5d29 2c20  el[:, p_indx]), 
-00017220: 4661 6c73 6529 2929 0d0a 2020 2020 2020  False)))..      
-00017230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017240: 2020 2620 7365 6c66 2e73 6c6f 7065 5f73    & self.slope_s
-00017250: 6967 6e5b 3a2c 2070 5f69 6e64 785d 0d0a  ign[:, p_indx]..
-00017260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017270: 2020 2020 295b 2d74 6c73 3a5d 0d0a 2020      )[-tls:]..  
-00017280: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00017290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000172a0: 2020 2767 726f 7774 685f 6465 6365 6c65    'growth_decele
-000172b0: 7261 7469 6e67 273a 2063 7572 5f74 7265  rating': cur_tre
-000172c0: 6e64 5b0d 0a20 2020 2020 2020 2020 2020  nd[..           
-000172d0: 2020 2020 2020 2020 2028 0d0a 2020 2020           (..    
-000172e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172f0: 2020 2020 6e70 2e68 7374 6163 6b28 286e      np.hstack((n
-00017300: 702e 7369 676e 6269 7428 7365 6c66 2e61  p.signbit(self.a
-00017310: 6363 656c 5b3a 2c20 705f 696e 6478 5d29  ccel[:, p_indx])
-00017320: 2c20 4661 6c73 6529 290d 0a20 2020 2020  , False))..     
-00017330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017340: 2020 2026 2028 7e73 656c 662e 736c 6f70     & (~self.slop
-00017350: 655f 7369 676e 5b3a 2c20 705f 696e 6478  e_sign[:, p_indx
-00017360: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00017370: 2020 2020 2020 2020 295b 2d74 6c73 3a5d          )[-tls:]
-00017380: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017390: 2020 5d2c 0d0a 2020 2020 2020 2020 2020    ],..          
-000173a0: 2020 2020 2020 2767 726f 7774 685f 6163        'growth_ac
-000173b0: 6365 6c65 7261 7469 6e67 273a 2063 7572  celerating': cur
-000173c0: 5f74 7265 6e64 5b0d 0a20 2020 2020 2020  _trend[..       
-000173d0: 2020 2020 2020 2020 2020 2020 2028 0d0a               (..
-000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173f0: 2020 2020 2020 2020 287e 6e70 2e68 7374          (~np.hst
-00017400: 6163 6b28 286e 702e 7369 676e 6269 7428  ack((np.signbit(
-00017410: 7365 6c66 2e61 6363 656c 5b3a 2c20 705f  self.accel[:, p_
-00017420: 696e 6478 5d29 2c20 4661 6c73 6529 2929  indx]), False)))
-00017430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017440: 2020 2020 2020 2020 2020 2620 287e 7365            & (~se
-00017450: 6c66 2e73 6c6f 7065 5f73 6967 6e5b 3a2c  lf.slope_sign[:,
-00017460: 2070 5f69 6e64 785d 290d 0a20 2020 2020   p_indx])..     
-00017470: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00017480: 5b2d 746c 733a 5d0d 0a20 2020 2020 2020  [-tls:]..       
-00017490: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-000174a0: 2020 2020 2020 2020 207d 2c0d 0a20 2020           },..   
-000174b0: 2020 2020 2020 2020 2069 6e64 6578 3d63           index=c
-000174c0: 7572 5f74 7265 6e64 2e69 6e64 6578 2c0d  ur_trend.index,.
-000174d0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-000174e0: 2020 2020 6966 2073 7461 7274 5f64 6174      if start_dat
-000174f0: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
-00017500: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
-00017510: 5f64 6620 3d20 706c 6f74 5f64 665b 706c  _df = plot_df[pl
-00017520: 6f74 5f64 662e 696e 6465 7820 3e3d 2073  ot_df.index >= s
-00017530: 7461 7274 5f64 6174 655d 0d0a 2020 2020  tart_date]..    
-00017540: 2020 2020 6178 203d 2070 6c6f 745f 6466      ax = plot_df
-00017550: 2e70 6c6f 7428 7469 746c 653d 7469 746c  .plot(title=titl
-00017560: 652c 2063 6f6c 6f72 3d63 6f6c 6f72 732c  e, color=colors,
-00017570: 202a 2a6b 7761 7267 7329 0d0a 2020 2020   **kwargs)..    
-00017580: 2020 2020 6861 6e64 6c65 732c 206c 6162      handles, lab
-00017590: 656c 7320 3d20 6178 2e67 6574 5f6c 6567  els = ax.get_leg
-000175a0: 656e 645f 6861 6e64 6c65 735f 6c61 6265  end_handles_labe
-000175b0: 6c73 2829 0d0a 2020 2020 2020 2020 2320  ls()..        # 
-000175c0: 6178 2e73 6361 7474 6572 2863 7572 5f74  ax.scatter(cur_t
-000175d0: 7265 6e64 2e69 6e64 6578 5b73 656c 662e  rend.index[self.
-000175e0: 6368 616e 6765 706f 696e 7473 5b3a 2c20  changepoints[:, 
-000175f0: 705f 696e 6478 5d5d 2c20 6375 725f 7472  p_indx]], cur_tr
-00017600: 656e 645b 7365 6c66 2e63 6861 6e67 6570  end[self.changep
-00017610: 6f69 6e74 735b 3a2c 2070 5f69 6e64 785d  oints[:, p_indx]
-00017620: 5d2c 2063 3d27 2366 6463 6330 3927 2c20  ], c='#fdcc09', 
-00017630: 733d 342e 3029 0d0a 2020 2020 2020 2020  s=4.0)..        
-00017640: 2320 6178 2e73 6361 7474 6572 2863 7572  # ax.scatter(cur
-00017650: 5f74 7265 6e64 2e69 6e64 6578 5b73 656c  _trend.index[sel
-00017660: 662e 7a65 726f 5f63 726f 7373 696e 6773  f.zero_crossings
-00017670: 5b3a 2c20 705f 696e 6478 5d5d 2c20 6375  [:, p_indx]], cu
-00017680: 725f 7472 656e 645b 7365 6c66 2e7a 6572  r_trend[self.zer
-00017690: 6f5f 6372 6f73 7369 6e67 735b 3a2c 2070  o_crossings[:, p
-000176a0: 5f69 6e64 785d 5d2c 2063 3d27 2335 3132  _indx]], c='#512
-000176b0: 6637 3427 2c20 733d 342e 3029 0d0a 2020  f74', s=4.0)..  
-000176c0: 2020 2020 2020 6966 2073 656c 662e 7472        if self.tr
-000176d0: 656e 645f 616e 6f6d 616c 795f 6465 7465  end_anomaly_dete
-000176e0: 6374 6f72 2069 7320 6e6f 7420 4e6f 6e65  ctor is not None
-000176f0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00017700: 6620 7365 6c66 2e74 7265 6e64 5f61 6e6f  f self.trend_ano
-00017710: 6d61 6c79 5f64 6574 6563 746f 722e 6f75  maly_detector.ou
-00017720: 7470 7574 203d 3d20 2275 6e69 7661 7269  tput == "univari
-00017730: 6174 6522 3a0d 0a20 2020 2020 2020 2020  ate":..         
-00017740: 2020 2020 2020 2069 5f61 6e6f 6d20 3d20         i_anom = 
-00017750: 7365 6c66 2e74 7265 6e64 5f61 6e6f 6d61  self.trend_anoma
-00017760: 6c79 5f64 6574 6563 746f 722e 616e 6f6d  ly_detector.anom
-00017770: 616c 6965 732e 696e 6465 785b 0d0a 2020  alies.index[..  
-00017780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017790: 2020 7365 6c66 2e61 6e6f 6d61 6c79 5f64    self.anomaly_d
-000177a0: 6574 6563 746f 722e 616e 6f6d 616c 6965  etector.anomalie
-000177b0: 732e 696c 6f63 5b3a 2c20 305d 203d 3d20  s.iloc[:, 0] == 
-000177c0: 2d31 0d0a 2020 2020 2020 2020 2020 2020  -1..            
-000177d0: 2020 2020 5d0d 0a20 2020 2020 2020 2020      ]..         
-000177e0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000177f0: 2020 2020 2020 2020 2020 7365 7269 6573            series
-00017800: 5f61 6e6f 6d20 3d20 7365 6c66 2e74 7265  _anom = self.tre
-00017810: 6e64 5f61 6e6f 6d61 6c79 5f64 6574 6563  nd_anomaly_detec
-00017820: 746f 722e 616e 6f6d 616c 6965 735b 7365  tor.anomalies[se
-00017830: 7269 6573 5d0d 0a20 2020 2020 2020 2020  ries]..         
-00017840: 2020 2020 2020 2069 5f61 6e6f 6d20 3d20         i_anom = 
-00017850: 7365 7269 6573 5f61 6e6f 6d5b 7365 7269  series_anom[seri
-00017860: 6573 5f61 6e6f 6d20 3d3d 202d 315d 2e69  es_anom == -1].i
-00017870: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
-00017880: 2020 6966 2073 7461 7274 5f64 6174 6520    if start_date 
-00017890: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-000178a0: 2020 2020 2020 2020 2020 2020 2020 695f                i_
-000178b0: 616e 6f6d 203d 2069 5f61 6e6f 6d5b 695f  anom = i_anom[i_
-000178c0: 616e 6f6d 203e 3d20 7374 6172 745f 6461  anom >= start_da
-000178d0: 7465 5d0d 0a20 2020 2020 2020 2020 2020  te]..           
-000178e0: 2069 5f61 6e6f 6d20 3d20 695f 616e 6f6d   i_anom = i_anom
-000178f0: 5b69 5f61 6e6f 6d20 3e3d 2063 7572 5f74  [i_anom >= cur_t
-00017900: 7265 6e64 2e69 6e64 6578 5b30 5d5d 0d0a  rend.index[0]]..
-00017910: 2020 2020 2020 2020 2020 2020 2320 6f6e              # on
-00017920: 6c79 2070 6c6f 7420 6966 2073 6f6d 6520  ly plot if some 
-00017930: 616e 6f6d 616c 6965 732c 2061 6e64 206e  anomalies, and n
-00017940: 6f74 2077 6179 2074 6f6f 206d 616e 7920  ot way too many 
-00017950: 616e 6f6d 616c 6965 730d 0a20 2020 2020  anomalies..     
-00017960: 2020 2020 2020 2069 6620 6c65 6e28 695f         if len(i_
-00017970: 616e 6f6d 2920 3e20 3020 616e 6420 6c65  anom) > 0 and le
-00017980: 6e28 695f 616e 6f6d 2920 3c20 6c65 6e28  n(i_anom) < len(
-00017990: 706c 6f74 5f64 6629 202a 2030 2e35 3a0d  plot_df) * 0.5:.
-000179a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000179b0: 2073 6361 7431 203d 2061 782e 7363 6174   scat1 = ax.scat
-000179c0: 7465 7228 0d0a 2020 2020 2020 2020 2020  ter(..          
-000179d0: 2020 2020 2020 2020 2020 695f 616e 6f6d            i_anom
-000179e0: 2e74 6f6c 6973 7428 292c 2063 7572 5f74  .tolist(), cur_t
-000179f0: 7265 6e64 2e6c 6f63 5b69 5f61 6e6f 6d5d  rend.loc[i_anom]
-00017a00: 2c20 633d 2272 6564 222c 2073 3d31 362e  , c="red", s=16.
-00017a10: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
-00017a20: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-00017a30: 2020 2020 2020 6861 6e64 6c65 7320 2b3d        handles +=
-00017a40: 205b 7363 6174 315d 0d0a 2020 2020 2020   [scat1]..      
-00017a50: 2020 2020 2020 2020 2020 6c61 6265 6c73            labels
-00017a60: 202b 3d20 5b27 7472 656e 6420 616e 6f6d   += ['trend anom
-00017a70: 616c 6965 7327 5d0d 0a20 2020 2020 2020  alies']..       
-00017a80: 2069 6620 766c 696e 6520 6973 206e 6f74   if vline is not
-00017a90: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00017aa0: 2020 2020 6178 2e76 6c69 6e65 7328 0d0a      ax.vlines(..
-00017ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ac0: 783d 766c 696e 652c 0d0a 2020 2020 2020  x=vline,..      
-00017ad0: 2020 2020 2020 2020 2020 6c73 3d27 2d2d            ls='--
-00017ae0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00017af0: 2020 2020 6c77 3d31 2c0d 0a20 2020 2020      lw=1,..     
-00017b00: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-00017b10: 733d 2764 6172 6b72 6564 272c 0d0a 2020  s='darkred',..  
-00017b20: 2020 2020 2020 2020 2020 2020 2020 796d                ym
-00017b30: 696e 3d63 7572 5f74 7265 6e64 5b63 7572  in=cur_trend[cur
-00017b40: 5f74 7265 6e64 2e69 6e64 6578 203e 3d20  _trend.index >= 
-00017b50: 7374 6172 745f 6461 7465 5d2e 6d69 6e28  start_date].min(
-00017b60: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00017b70: 2020 2020 796d 6178 3d63 7572 5f74 7265      ymax=cur_tre
-00017b80: 6e64 5b63 7572 5f74 7265 6e64 2e69 6e64  nd[cur_trend.ind
-00017b90: 6578 203e 3d20 7374 6172 745f 6461 7465  ex >= start_date
-00017ba0: 5d2e 6d61 7828 292c 0d0a 2020 2020 2020  ].max(),..      
-00017bb0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00017bc0: 2061 782e 6c65 6765 6e64 2868 616e 646c   ax.legend(handl
-00017bd0: 6573 2c20 6c61 6265 6c73 290d 0a20 2020  es, labels)..   
-00017be0: 2020 2020 2072 6574 7572 6e20 6178 0d0a       return ax..
-00017bf0: 0d0a 2020 2020 6465 6620 706c 6f74 5f66  ..    def plot_f
-00017c00: 6f72 6563 6173 7428 0d0a 2020 2020 2020  orecast(..      
-00017c10: 2020 7365 6c66 2c0d 0a20 2020 2020 2020    self,..       
-00017c20: 2070 7265 6469 6374 696f 6e2c 0d0a 2020   prediction,..  
-00017c30: 2020 2020 2020 6163 7475 616c 733d 4e6f        actuals=No
-00017c40: 6e65 2c0d 0a20 2020 2020 2020 2073 6572  ne,..        ser
-00017c50: 6965 733d 4e6f 6e65 2c0d 0a20 2020 2020  ies=None,..     
-00017c60: 2020 2073 7461 7274 5f64 6174 653d 4e6f     start_date=No
-00017c70: 6e65 2c0d 0a20 2020 2020 2020 2061 6e6f  ne,..        ano
-00017c80: 6d61 6c79 5f63 6f6c 6f72 3d22 6461 726b  maly_color="dark
-00017c90: 736c 6174 6562 6c75 6522 2c0d 0a20 2020  slateblue",..   
-00017ca0: 2020 2020 2068 6f6c 6964 6179 5f63 6f6c       holiday_col
-00017cb0: 6f72 3d22 6461 726b 6772 6565 6e22 2c0d  or="darkgreen",.
-00017cc0: 0a20 2020 2020 2020 2074 7265 6e64 5f61  .        trend_a
-00017cd0: 6e6f 6d61 6c79 5f63 6f6c 6f72 3d27 736c  nomaly_color='sl
-00017ce0: 6174 6567 7261 7927 2c0d 0a20 2020 2020  ategray',..     
-00017cf0: 2020 2070 6f69 6e74 5f73 697a 653d 3132     point_size=12
-00017d00: 2e30 2c0d 0a20 2020 2029 3a0d 0a20 2020  .0,..    ):..   
-00017d10: 2020 2020 2022 2222 506c 6f74 2061 2066       """Plot a f
-00017d20: 6f72 6563 6173 7420 7469 6d65 2073 6572  orecast time ser
-00017d30: 6965 732e 0d0a 0d0a 2020 2020 2020 2020  ies.....        
-00017d40: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
-00017d50: 2020 2070 7265 6469 6374 696f 6e20 286d     prediction (m
-00017d60: 6f64 656c 2070 7265 6469 6374 696f 6e20  odel prediction 
-00017d70: 6f62 6a65 6374 2c20 7265 7175 6972 6564  object, required
-00017d80: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
-00017d90: 6374 7561 6c73 2028 7064 2e44 6174 6146  ctuals (pd.DataF
-00017da0: 7261 6d65 293a 2077 6964 6520 7374 796c  rame): wide styl
-00017db0: 6520 6466 2c20 6f66 206b 6e6f 7720 6461  e df, of know da
-00017dc0: 7461 2069 6620 6176 6169 6c61 626c 650d  ta if available.
-00017dd0: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
-00017de0: 6965 7320 2873 7472 293a 206e 616d 6520  ies (str): name 
-00017df0: 6f66 2074 696d 6520 7365 7269 6573 2063  of time series c
-00017e00: 6f6c 756d 6e20 746f 2070 6c6f 740d 0a20  olumn to plot.. 
-00017e10: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00017e20: 5f64 6174 6520 2873 7472 206f 7220 5469  _date (str or Ti
-00017e30: 6d65 7374 616d 7029 3a20 706f 696e 7420  mestamp): point 
-00017e40: 6174 2077 6869 6368 2074 6f20 6265 6769  at which to begi
-00017e50: 6e20 5820 6178 6973 0d0a 2020 2020 2020  n X axis..      
-00017e60: 2020 2020 2020 616e 6f6d 616c 795f 636f        anomaly_co
-00017e70: 6c6f 7220 2873 7472 293a 206e 616d 6520  lor (str): name 
-00017e80: 6f66 2061 6e6f 6d61 6c79 2070 6f69 6e74  of anomaly point
-00017e90: 2063 6f6c 6f72 0d0a 2020 2020 2020 2020   color..        
-00017ea0: 2020 2020 686f 6c69 6461 795f 636f 6c6f      holiday_colo
-00017eb0: 7220 2873 7472 293a 206e 616d 6520 6f66  r (str): name of
-00017ec0: 2068 6f6c 6964 6179 2070 6f69 6e74 2063   holiday point c
-00017ed0: 6f6c 6f72 0d0a 2020 2020 2020 2020 2020  olor..          
-00017ee0: 2020 7472 656e 645f 616e 6f6d 616c 795f    trend_anomaly_
-00017ef0: 636f 6c6f 7220 2873 7472 293a 206e 616d  color (str): nam
-00017f00: 6520 6f66 2074 7265 6e64 2061 6e6f 6d61  e of trend anoma
-00017f10: 6c79 2070 6f69 6e74 2063 6f6c 6f72 0d0a  ly point color..
-00017f20: 2020 2020 2020 2020 2020 2020 706f 696e              poin
-00017f30: 745f 7369 7a65 2028 7374 7229 3a20 706f  t_size (str): po
-00017f40: 696e 7420 7369 7a65 2066 6f72 2061 6c6c  int size for all
-00017f50: 2061 6e6f 6d61 6c69 6573 0d0a 2020 2020   anomalies..    
-00017f60: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00017f70: 2069 6620 7365 7269 6573 2069 7320 4e6f   if series is No
-00017f80: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00017f90: 2073 6572 6965 7320 3d20 7261 6e64 6f6d   series = random
-00017fa0: 2e63 686f 6963 6528 7365 6c66 2e63 6f6c  .choice(self.col
-00017fb0: 756d 6e5f 6e61 6d65 7329 0d0a 2020 2020  umn_names)..    
-00017fc0: 2020 2020 6966 2061 6374 7561 6c73 2069      if actuals i
-00017fd0: 7320 4e6f 6e65 206f 7220 6e6f 7420 6973  s None or not is
-00017fe0: 696e 7374 616e 6365 280d 0a20 2020 2020  instance(..     
-00017ff0: 2020 2020 2020 2061 6374 7561 6c73 2c20         actuals, 
-00018000: 2870 642e 4461 7461 4672 616d 652c 206e  (pd.DataFrame, n
-00018010: 702e 6172 7261 792c 2070 642e 5365 7269  p.array, pd.Seri
-00018020: 6573 290d 0a20 2020 2020 2020 2029 3a0d  es)..        ):.
-00018030: 0a20 2020 2020 2020 2020 2020 2061 6374  .            act
-00018040: 7561 6c73 5f75 7365 6420 3d20 7072 6564  uals_used = pred
-00018050: 6963 7469 6f6e 2e66 6f72 6563 6173 740d  iction.forecast.
-00018060: 0a20 2020 2020 2020 2020 2020 2061 6374  .            act
-00018070: 7561 6c73 5f66 6c61 6720 3d20 4661 6c73  uals_flag = Fals
-00018080: 650d 0a20 2020 2020 2020 2065 6c73 653a  e..        else:
-00018090: 0d0a 2020 2020 2020 2020 2020 2020 6163  ..            ac
-000180a0: 7475 616c 735f 666c 6167 203d 2054 7275  tuals_flag = Tru
-000180b0: 650d 0a20 2020 2020 2020 2020 2020 2061  e..            a
-000180c0: 6374 7561 6c73 5f75 7365 6420 3d20 6163  ctuals_used = ac
-000180d0: 7475 616c 732e 7265 696e 6465 7828 7072  tuals.reindex(pr
-000180e0: 6564 6963 7469 6f6e 2e66 6f72 6563 6173  ediction.forecas
-000180f0: 742e 696e 6465 7829 0d0a 2020 2020 2020  t.index)..      
-00018100: 2020 766c 696e 6520 3d20 280d 0a20 2020    vline = (..   
-00018110: 2020 2020 2020 2020 204e 6f6e 650d 0a20           None.. 
-00018120: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00018130: 6c66 2e66 6f72 6563 6173 745f 6c65 6e67  lf.forecast_leng
-00018140: 7468 2069 7320 4e6f 6e65 0d0a 2020 2020  th is None..    
-00018150: 2020 2020 2020 2020 656c 7365 2070 7265          else pre
-00018160: 6469 6374 696f 6e2e 666f 7265 6361 7374  diction.forecast
-00018170: 2e69 6e64 6578 5b2d 7365 6c66 2e66 6f72  .index[-self.for
-00018180: 6563 6173 745f 6c65 6e67 7468 5d0d 0a20  ecast_length].. 
-00018190: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000181a0: 2020 6178 203d 2070 7265 6469 6374 696f    ax = predictio
-000181b0: 6e2e 706c 6f74 280d 0a20 2020 2020 2020  n.plot(..       
-000181c0: 2020 2020 2061 6374 7561 6c73 5f75 7365       actuals_use
-000181d0: 642e 6c6f 635b 7072 6564 6963 7469 6f6e  d.loc[prediction
-000181e0: 2e66 6f72 6563 6173 742e 696e 6465 785d  .forecast.index]
-000181f0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00018200: 2061 6374 7561 6c73 5f66 6c61 6720 6973   actuals_flag is
-00018210: 206e 6f74 204e 6f6e 650d 0a20 2020 2020   not None..     
-00018220: 2020 2020 2020 2065 6c73 6520 4e6f 6e65         else None
-00018230: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00018240: 6572 6965 733d 7365 7269 6573 2c0d 0a20  eries=series,.. 
-00018250: 2020 2020 2020 2020 2020 2076 6c69 6e65             vline
-00018260: 3d76 6c69 6e65 2c0d 0a20 2020 2020 2020  =vline,..       
-00018270: 2020 2020 2073 7461 7274 5f64 6174 653d       start_date=
-00018280: 7374 6172 745f 6461 7465 2c0d 0a20 2020  start_date,..   
-00018290: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-000182a0: 6861 6e64 6c65 732c 206c 6162 656c 7320  handles, labels 
-000182b0: 3d20 6178 2e67 6574 5f6c 6567 656e 645f  = ax.get_legend_
-000182c0: 6861 6e64 6c65 735f 6c61 6265 6c73 2829  handles_labels()
-000182d0: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-000182e0: 662e 616e 6f6d 616c 795f 6465 7465 6374  f.anomaly_detect
-000182f0: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00018300: 2069 6620 7365 6c66 2e61 6e6f 6d61 6c79   if self.anomaly
-00018310: 5f64 6574 6563 746f 722e 6f75 7470 7574  _detector.output
-00018320: 203d 3d20 2275 6e69 7661 7269 6174 6522   == "univariate"
-00018330: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00018340: 2020 2069 5f61 6e6f 6d20 3d20 7365 6c66     i_anom = self
-00018350: 2e61 6e6f 6d61 6c79 5f64 6574 6563 746f  .anomaly_detecto
-00018360: 722e 616e 6f6d 616c 6965 732e 696e 6465  r.anomalies.inde
-00018370: 785b 0d0a 2020 2020 2020 2020 2020 2020  x[..            
-00018380: 2020 2020 2020 2020 7365 6c66 2e61 6e6f          self.ano
-00018390: 6d61 6c79 5f64 6574 6563 746f 722e 616e  maly_detector.an
-000183a0: 6f6d 616c 6965 732e 696c 6f63 5b3a 2c20  omalies.iloc[:, 
-000183b0: 305d 203d 3d20 2d31 0d0a 2020 2020 2020  0] == -1..      
-000183c0: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
-000183d0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-000183e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183f0: 7365 7269 6573 5f61 6e6f 6d20 3d20 7365  series_anom = se
-00018400: 6c66 2e61 6e6f 6d61 6c79 5f64 6574 6563  lf.anomaly_detec
-00018410: 746f 722e 616e 6f6d 616c 6965 735b 7365  tor.anomalies[se
-00018420: 7269 6573 5d0d 0a20 2020 2020 2020 2020  ries]..         
-00018430: 2020 2020 2020 2069 5f61 6e6f 6d20 3d20         i_anom = 
-00018440: 7365 7269 6573 5f61 6e6f 6d5b 7365 7269  series_anom[seri
-00018450: 6573 5f61 6e6f 6d20 3d3d 202d 315d 2e69  es_anom == -1].i
-00018460: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
-00018470: 2020 6966 2073 7461 7274 5f64 6174 6520    if start_date 
-00018480: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00018490: 2020 2020 2020 2020 2020 2020 2020 695f                i_
-000184a0: 616e 6f6d 203d 2069 5f61 6e6f 6d5b 695f  anom = i_anom[i_
-000184b0: 616e 6f6d 203e 3d20 7374 6172 745f 6461  anom >= start_da
-000184c0: 7465 5d0d 0a20 2020 2020 2020 2020 2020  te]..           
-000184d0: 2069 6620 6163 7475 616c 735f 666c 6167   if actuals_flag
-000184e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000184f0: 2020 2069 5f61 6e6f 6d20 3d20 695f 616e     i_anom = i_an
-00018500: 6f6d 5b69 5f61 6e6f 6d20 3e3d 2061 6374  om[i_anom >= act
-00018510: 7561 6c73 2e69 6e64 6578 5b30 5d5d 0d0a  uals.index[0]]..
-00018520: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00018530: 656e 2869 5f61 6e6f 6d29 203e 2030 2061  en(i_anom) > 0 a
-00018540: 6e64 2028 0d0a 2020 2020 2020 2020 2020  nd (..          
-00018550: 2020 2020 2020 6e6f 7420 6163 7475 616c        not actual
-00018560: 735f 666c 6167 206f 7220 6c65 6e28 695f  s_flag or len(i_
-00018570: 616e 6f6d 2920 3c20 6c65 6e28 6163 7475  anom) < len(actu
-00018580: 616c 7329 202a 2030 2e35 0d0a 2020 2020  als) * 0.5..    
-00018590: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
-000185a0: 2020 2020 2020 2020 2020 2020 7363 6174              scat
-000185b0: 3120 3d20 6178 2e73 6361 7474 6572 280d  1 = ax.scatter(.
-000185c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000185d0: 2020 2020 2069 5f61 6e6f 6d2e 746f 6c69       i_anom.toli
-000185e0: 7374 2829 2c0d 0a20 2020 2020 2020 2020  st(),..         
-000185f0: 2020 2020 2020 2020 2020 2061 6374 7561             actua
-00018600: 6c73 5f75 7365 642e 7265 696e 6465 7828  ls_used.reindex(
-00018610: 695f 616e 6f6d 295b 7365 7269 6573 5d2c  i_anom)[series],
-00018620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018630: 2020 2020 2020 633d 616e 6f6d 616c 795f        c=anomaly_
-00018640: 636f 6c6f 722c 0d0a 2020 2020 2020 2020  color,..        
-00018650: 2020 2020 2020 2020 2020 2020 733d 706f              s=po
-00018660: 696e 745f 7369 7a65 2c0d 0a20 2020 2020  int_size,..     
-00018670: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
-00018680: 2020 2020 2020 2020 2020 2020 2020 6861                ha
-00018690: 6e64 6c65 7320 2b3d 205b 7363 6174 315d  ndles += [scat1]
-000186a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000186b0: 2020 6c61 6265 6c73 202b 3d20 5b22 616e    labels += ["an
-000186c0: 6f6d 616c 6965 7322 5d0d 0a20 2020 2020  omalies"]..     
-000186d0: 2020 2069 6620 7365 6c66 2e68 6f6c 6964     if self.holid
-000186e0: 6179 5f64 6574 6563 746f 723a 0d0a 2020  ay_detector:..  
-000186f0: 2020 2020 2020 2020 2020 695f 616e 6f6d            i_anom
-00018700: 203d 2073 656c 662e 686f 6c69 6461 795f   = self.holiday_
-00018710: 6465 7465 6374 6f72 2e64 6174 6573 5f74  detector.dates_t
-00018720: 6f5f 686f 6c69 6461 7973 280d 0a20 2020  o_holidays(..   
-00018730: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018740: 662e 6466 2e69 6e64 6578 2c20 7374 796c  f.df.index, styl
-00018750: 653d 2273 6572 6965 735f 666c 6167 220d  e="series_flag".
-00018760: 0a20 2020 2020 2020 2020 2020 2029 5b73  .            )[s
-00018770: 6572 6965 735d 0d0a 2020 2020 2020 2020  eries]..        
-00018780: 2020 2020 695f 616e 6f6d 203d 2069 5f61      i_anom = i_a
-00018790: 6e6f 6d2e 696e 6465 785b 695f 616e 6f6d  nom.index[i_anom
-000187a0: 203d 3d20 315d 0d0a 2020 2020 2020 2020   == 1]..        
-000187b0: 2020 2020 6966 2061 6374 7561 6c73 5f66      if actuals_f
-000187c0: 6c61 673a 0d0a 2020 2020 2020 2020 2020  lag:..          
-000187d0: 2020 2020 2020 695f 616e 6f6d 203d 2069        i_anom = i
-000187e0: 5f61 6e6f 6d5b 695f 616e 6f6d 203e 3d20  _anom[i_anom >= 
-000187f0: 6163 7475 616c 732e 696e 6465 785b 305d  actuals.index[0]
-00018800: 5d0d 0a20 2020 2020 2020 2020 2020 2069  ]..            i
-00018810: 6620 6c65 6e28 695f 616e 6f6d 2920 3e20  f len(i_anom) > 
-00018820: 3020 616e 6420 280d 0a20 2020 2020 2020  0 and (..       
-00018830: 2020 2020 2020 2020 206e 6f74 2061 6374           not act
-00018840: 7561 6c73 5f66 6c61 6720 6f72 206c 656e  uals_flag or len
-00018850: 2869 5f61 6e6f 6d29 203c 206c 656e 2861  (i_anom) < len(a
-00018860: 6374 7561 6c73 2920 2a20 302e 350d 0a20  ctuals) * 0.5.. 
-00018870: 2020 2020 2020 2020 2020 2029 3a0d 0a20             ):.. 
-00018880: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018890: 6361 7432 203d 2061 782e 7363 6174 7465  cat2 = ax.scatte
-000188a0: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
-000188b0: 2020 2020 2020 2020 695f 616e 6f6d 2e74          i_anom.t
-000188c0: 6f6c 6973 7428 292c 0d0a 2020 2020 2020  olist(),..      
-000188d0: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-000188e0: 7475 616c 735f 7573 6564 2e72 6569 6e64  tuals_used.reind
-000188f0: 6578 2869 5f61 6e6f 6d29 5b73 6572 6965  ex(i_anom)[serie
-00018900: 735d 2c0d 0a20 2020 2020 2020 2020 2020  s],..           
-00018910: 2020 2020 2020 2020 2063 3d68 6f6c 6964           c=holid
-00018920: 6179 5f63 6f6c 6f72 2c0d 0a20 2020 2020  ay_color,..     
-00018930: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018940: 3d70 6f69 6e74 5f73 697a 652c 0d0a 2020  =point_size,..  
-00018950: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00018960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018970: 2068 616e 646c 6573 202b 3d20 5b73 6361   handles += [sca
-00018980: 7432 5d0d 0a20 2020 2020 2020 2020 2020  t2]..           
-00018990: 2020 2020 206c 6162 656c 7320 2b3d 205b       labels += [
-000189a0: 2264 6574 6563 7465 6420 686f 6c69 6461  "detected holida
-000189b0: 7973 225d 0d0a 2020 2020 2020 2020 6966  ys"]..        if
-000189c0: 2073 656c 662e 7472 656e 645f 616e 6f6d   self.trend_anom
-000189d0: 616c 795f 6465 7465 6374 6f72 2069 7320  aly_detector is 
-000189e0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-000189f0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-00018a00: 7265 6e64 5f61 6e6f 6d61 6c79 5f64 6574  rend_anomaly_det
-00018a10: 6563 746f 722e 6f75 7470 7574 203d 3d20  ector.output == 
-00018a20: 2275 6e69 7661 7269 6174 6522 3a0d 0a20  "univariate":.. 
-00018a30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00018a40: 5f61 6e6f 6d20 3d20 7365 6c66 2e74 7265  _anom = self.tre
-00018a50: 6e64 5f61 6e6f 6d61 6c79 5f64 6574 6563  nd_anomaly_detec
-00018a60: 746f 722e 616e 6f6d 616c 6965 732e 696e  tor.anomalies.in
-00018a70: 6465 785b 0d0a 2020 2020 2020 2020 2020  dex[..          
-00018a80: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00018a90: 6e6f 6d61 6c79 5f64 6574 6563 746f 722e  nomaly_detector.
-00018aa0: 616e 6f6d 616c 6965 732e 696c 6f63 5b3a  anomalies.iloc[:
-00018ab0: 2c20 305d 203d 3d20 2d31 0d0a 2020 2020  , 0] == -1..    
-00018ac0: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
-00018ad0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00018ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018af0: 2020 7365 7269 6573 5f61 6e6f 6d20 3d20    series_anom = 
-00018b00: 7365 6c66 2e74 7265 6e64 5f61 6e6f 6d61  self.trend_anoma
-00018b10: 6c79 5f64 6574 6563 746f 722e 616e 6f6d  ly_detector.anom
-00018b20: 616c 6965 735b 7365 7269 6573 5d0d 0a20  alies[series].. 
-00018b30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00018b40: 5f61 6e6f 6d20 3d20 7365 7269 6573 5f61  _anom = series_a
-00018b50: 6e6f 6d5b 7365 7269 6573 5f61 6e6f 6d20  nom[series_anom 
-00018b60: 3d3d 202d 315d 2e69 6e64 6578 0d0a 2020  == -1].index..  
-00018b70: 2020 2020 2020 2020 2020 6966 2073 7461            if sta
-00018b80: 7274 5f64 6174 6520 6973 206e 6f74 204e  rt_date is not N
-00018b90: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00018ba0: 2020 2020 2020 695f 616e 6f6d 203d 2069        i_anom = i
-00018bb0: 5f61 6e6f 6d5b 695f 616e 6f6d 203e 3d20  _anom[i_anom >= 
-00018bc0: 7374 6172 745f 6461 7465 5d0d 0a20 2020  start_date]..   
-00018bd0: 2020 2020 2020 2020 2069 6620 6163 7475           if actu
-00018be0: 616c 735f 666c 6167 3a0d 0a20 2020 2020  als_flag:..     
-00018bf0: 2020 2020 2020 2020 2020 2069 5f61 6e6f             i_ano
-00018c00: 6d20 3d20 695f 616e 6f6d 5b69 5f61 6e6f  m = i_anom[i_ano
-00018c10: 6d20 3e3d 2061 6374 7561 6c73 2e69 6e64  m >= actuals.ind
-00018c20: 6578 5b30 5d5d 0d0a 2020 2020 2020 2020  ex[0]]..        
-00018c30: 2020 2020 6966 206c 656e 2869 5f61 6e6f      if len(i_ano
-00018c40: 6d29 203e 2030 2061 6e64 2028 0d0a 2020  m) > 0 and (..  
-00018c50: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00018c60: 7420 6163 7475 616c 735f 666c 6167 206f  t actuals_flag o
-00018c70: 7220 6c65 6e28 695f 616e 6f6d 2920 3c20  r len(i_anom) < 
-00018c80: 6c65 6e28 6163 7475 616c 7329 202a 2030  len(actuals) * 0
-00018c90: 2e35 0d0a 2020 2020 2020 2020 2020 2020  .5..            
-00018ca0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00018cb0: 2020 2020 7363 6174 3320 3d20 6178 2e73      scat3 = ax.s
-00018cc0: 6361 7474 6572 280d 0a20 2020 2020 2020  catter(..       
-00018cd0: 2020 2020 2020 2020 2020 2020 2069 5f61               i_a
-00018ce0: 6e6f 6d2e 746f 6c69 7374 2829 2c0d 0a20  nom.tolist(),.. 
-00018cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d00: 2020 2061 6374 7561 6c73 5f75 7365 642e     actuals_used.
-00018d10: 7265 696e 6465 7828 695f 616e 6f6d 295b  reindex(i_anom)[
-00018d20: 7365 7269 6573 5d2c 0d0a 2020 2020 2020  series],..      
-00018d30: 2020 2020 2020 2020 2020 2020 2020 633d                c=
-00018d40: 7472 656e 645f 616e 6f6d 616c 795f 636f  trend_anomaly_co
-00018d50: 6c6f 722c 0d0a 2020 2020 2020 2020 2020  lor,..          
-00018d60: 2020 2020 2020 2020 2020 733d 706f 696e            s=poin
-00018d70: 745f 7369 7a65 2c0d 0a20 2020 2020 2020  t_size,..       
-00018d80: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00018d90: 2020 2020 2020 2020 2020 2020 6861 6e64              hand
-00018da0: 6c65 7320 2b3d 205b 7363 6174 335d 0d0a  les += [scat3]..
-00018db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dc0: 6c61 6265 6c73 202b 3d20 5b22 7472 656e  labels += ["tren
-00018dd0: 6420 616e 6f6d 616c 6965 7322 5d0d 0a20  d anomalies"].. 
-00018de0: 2020 2020 2020 2061 782e 6c65 6765 6e64         ax.legend
-00018df0: 2868 616e 646c 6573 2c20 6c61 6265 6c73  (handles, labels
-00018e00: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00018e10: 6e20 6178 0d0a 0d0a 2020 2020 6465 6620  n ax....    def 
-00018e20: 706c 6f74 5f74 6869 6e67 7328 293a 2020  plot_things():  
-00018e30: 2320 706c 6163 6568 6f6c 6465 7220 666f  # placeholder fo
-00018e40: 7220 6c61 7465 7220 706c 6f74 7469 6e67  r later plotting
-00018e50: 2066 756e 6374 696f 6e73 0d0a 2020 2020   functions..    
-00018e60: 2020 2020 2320 706c 6f74 2063 6f6d 706f      # plot compo
-00018e70: 6e65 6e74 730d 0a20 2020 2020 2020 2023  nents..        #
-00018e80: 2070 6c6f 7420 7472 616e 7366 6f72 6d65   plot transforme
-00018e90: 6420 6466 2069 6620 7072 6570 726f 6365  d df if preproce
-00018ea0: 7373 206f 7220 616e 6f6d 616c 7920 7265  ss or anomaly re
-00018eb0: 6d6f 7661 6c0d 0a20 2020 2020 2020 2023  moval..        #
-00018ec0: 2070 6c6f 7420 7061 7374 2069 6d70 6163   plot past impac
-00018ed0: 7473 0d0a 2020 2020 2020 2020 2320 706c  ts..        # pl
-00018ee0: 6f74 2025 2063 6f6e 7472 6962 7574 696f  ot % contributio
-00018ef0: 6e20 6f66 2063 6f6d 706f 6e65 6e74 730d  n of components.
-00018f00: 0a20 2020 2020 2020 2023 2070 6c6f 7420  .        # plot 
-00018f10: 6576 616c 2028 7368 6f77 2061 6374 7561  eval (show actua
-00018f20: 6c73 2c20 616c 6f6e 6773 6964 6520 6675  ls, alongside fu
-00018f30: 6c6c 2061 6e64 2063 6f6d 706f 6e65 6e74  ll and component
-00018f40: 7320 746f 2064 6961 676e 6f73 6529 0d0a  s to diagnose)..
-00018f50: 2020 2020 2020 2020 2320 706c 6f74 2072          # plot r
-00018f60: 6573 6964 7561 6c20 6469 7374 7269 6275  esidual distribu
-00018f70: 7469 6f6e 2f50 4143 460d 0a20 2020 2020  tion/PACF..     
-00018f80: 2020 2023 2070 6c6f 7420 696e 666c 6563     # plot inflec
-00018f90: 7469 6f6e 2070 6f69 6e74 7320 2866 696c  tion points (fil
-00018fa0: 7465 7269 6e67 206f 7220 736d 6f6f 7468  tering or smooth
-00018fb0: 696e 6720 6669 7273 7429 0d0a 2020 2020  ing first)..    
-00018fc0: 2020 2020 2320 706c 6f74 2068 6967 6865      # plot highe
-00018fd0: 7374 2065 7272 6f72 2073 6572 6965 732c  st error series,
-00018fe0: 2070 6c6f 7420 6869 6768 6573 742f 6c6f   plot highest/lo
-00018ff0: 7765 7374 2067 726f 7774 680d 0a20 2020  west growth..   
-00019000: 2020 2020 2023 2074 7265 6e64 3a20 6f6e       # trend: on
-00019010: 6520 636f 6c6f 7220 666f 7220 6772 6f77  e color for grow
-00019020: 7468 2c20 616e 6f74 6865 7220 666f 7220  th, another for 
-00019030: 6465 636c 696e 6520 2864 6172 6b65 7220  decline (darker 
-00019040: 6173 2061 6363 656c 6572 6174 696e 672c  as accelerating,
-00019050: 206c 6967 6865 7220 6173 2073 6c6f 7769   ligher as slowi
-00019060: 6e67 290d 0a20 2020 2020 2020 2072 6574  ng)..        ret
-00019070: 7572 6e20 4e6f 7449 6d70 6c65 6d65 6e74  urn NotImplement
-00019080: 6564 0d0a 0d0a 0d0a 6465 6620 636c 6561  ed......def clea
-00019090: 6e5f 7265 6772 6573 736f 7228 696e 5f64  n_regressor(in_d
-000190a0: 2c20 7072 6566 6978 3d22 7265 6772 5f22  , prefix="regr_"
-000190b0: 293a 0d0a 2020 2020 6966 206e 6f74 2069  ):..    if not i
-000190c0: 7369 6e73 7461 6e63 6528 696e 5f64 2c20  sinstance(in_d, 
-000190d0: 7064 2e44 6174 6146 7261 6d65 293a 0d0a  pd.DataFrame):..
-000190e0: 2020 2020 2020 2020 6466 203d 2070 642e          df = pd.
-000190f0: 4461 7461 4672 616d 6528 696e 5f64 290d  DataFrame(in_d).
-00019100: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
-00019110: 2020 2020 6466 203d 2069 6e5f 642e 636f      df = in_d.co
-00019120: 7079 2829 0d0a 2020 2020 6466 2e63 6f6c  py()..    df.col
-00019130: 756d 6e73 203d 205b 7072 6566 6978 202b  umns = [prefix +
-00019140: 2063 6f6c 2066 6f72 2063 6f6c 2069 6e20   col for col in 
-00019150: 6466 2e63 6f6c 756d 6e73 5d0d 0a20 2020  df.columns]..   
-00019160: 2072 6574 7572 6e20 6466 0d0a 0d0a 0d0a   return df......
-00019170: 6465 6620 6372 6561 7465 5f74 2864 7329  def create_t(ds)
-00019180: 3a0d 0a20 2020 2072 6574 7572 6e20 2864  :..    return (d
-00019190: 7320 2d20 6473 2e6d 696e 2829 2920 2f20  s - ds.min()) / 
-000191a0: 2864 732e 6d61 7828 2920 2d20 6473 2e6d  (ds.max() - ds.m
-000191b0: 696e 2829 290d 0a0d 0a0d 0a23 2323 2323  in())......#####
-000191c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000191d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000191e0: 0d0a 2320 4a55 5354 204c 4541 5354 2053  ..# JUST LEAST S
-000191f0: 5155 4152 4553 2055 4e49 5641 5249 4154  QUARES UNIVARIAT
-00019200: 450d 0a23 2068 7474 7073 3a2f 2f73 7461  E..# https://sta
-00019210: 636b 6f76 6572 666c 6f77 2e63 6f6d 2f71  ckoverflow.com/q
-00019220: 7565 7374 696f 6e73 2f31 3736 3739 3134  uestions/1767914
-00019230: 302f 6d75 6c74 6970 6c65 2d6c 696e 6561  0/multiple-linea
-00019240: 722d 7265 6772 6573 7369 6f6e 2d77 6974  r-regression-wit
-00019250: 682d 7079 7468 6f6e 0d0a 0d0a 0d0a 6465  h-python......de
-00019260: 6620 6c73 7473 715f 736f 6c76 6528 582c  f lstsq_solve(X,
-00019270: 2079 2c20 6c61 6d62 3d31 2c20 6964 656e   y, lamb=1, iden
-00019280: 7469 7479 5f6d 6174 7269 783d 4e6f 6e65  tity_matrix=None
-00019290: 293a 0d0a 2020 2020 6966 2069 6465 6e74  ):..    if ident
-000192a0: 6974 795f 6d61 7472 6978 2069 7320 4e6f  ity_matrix is No
-000192b0: 6e65 3a0d 0a20 2020 2020 2020 2069 6465  ne:..        ide
-000192c0: 6e74 6974 795f 6d61 7472 6978 203d 206e  ntity_matrix = n
-000192d0: 702e 7a65 726f 7328 2858 2e73 6861 7065  p.zeros((X.shape
-000192e0: 5b31 5d2c 2058 2e73 6861 7065 5b31 5d29  [1], X.shape[1])
-000192f0: 290d 0a20 2020 2020 2020 206e 702e 6669  )..        np.fi
-00019300: 6c6c 5f64 6961 676f 6e61 6c28 6964 656e  ll_diagonal(iden
-00019310: 7469 7479 5f6d 6174 7269 782c 2031 290d  tity_matrix, 1).
-00019320: 0a20 2020 2020 2020 2069 6465 6e74 6974  .        identit
-00019330: 795f 6d61 7472 6978 5b30 2c20 305d 203d  y_matrix[0, 0] =
-00019340: 2030 0d0a 2020 2020 5874 585f 6c61 6d62   0..    XtX_lamb
-00019350: 203d 2058 2e54 2e64 6f74 2858 2920 2b20   = X.T.dot(X) + 
-00019360: 6c61 6d62 202a 2069 6465 6e74 6974 795f  lamb * identity_
-00019370: 6d61 7472 6978 0d0a 2020 2020 5874 5920  matrix..    XtY 
-00019380: 3d20 582e 542e 646f 7428 7929 0d0a 2020  = X.T.dot(y)..  
-00019390: 2020 7265 7475 726e 206e 702e 6c69 6e61    return np.lina
-000193a0: 6c67 2e73 6f6c 7665 2858 7458 5f6c 616d  lg.solve(XtX_lam
-000193b0: 622c 2058 7459 290d 0a0d 0a0d 0a64 6566  b, XtY)......def
-000193c0: 2063 6f73 745f 6675 6e63 7469 6f6e 5f6c   cost_function_l
-000193d0: 3128 7061 7261 6d73 2c20 582c 2079 293a  1(params, X, y):
-000193e0: 0d0a 2020 2020 7265 7475 726e 206e 702e  ..    return np.
-000193f0: 7375 6d28 6e70 2e61 6273 2879 202d 206e  sum(np.abs(y - n
-00019400: 702e 646f 7428 582c 2070 6172 616d 732e  p.dot(X, params.
-00019410: 7265 7368 6170 6528 582e 7368 6170 655b  reshape(X.shape[
-00019420: 315d 2c20 792e 7368 6170 655b 315d 2929  1], y.shape[1]))
-00019430: 2929 0d0a 0d0a 0d0a 6465 6620 636f 7374  ))......def cost
-00019440: 5f66 756e 6374 696f 6e5f 6c31 5f70 6f73  _function_l1_pos
-00019450: 6974 6976 6528 7061 7261 6d73 2c20 582c  itive(params, X,
-00019460: 2079 293a 0d0a 2020 2020 7265 7475 726e   y):..    return
-00019470: 206e 702e 7375 6d28 0d0a 2020 2020 2020   np.sum(..      
-00019480: 2020 6e70 2e61 6273 280d 0a20 2020 2020    np.abs(..     
-00019490: 2020 2020 2020 2079 0d0a 2020 2020 2020         y..      
-000194a0: 2020 2020 2020 2d20 6e70 2e64 6f74 2858        - np.dot(X
-000194b0: 2c20 6e70 2e77 6865 7265 2870 6172 616d  , np.where(param
-000194c0: 7320 3c20 302c 2030 2c20 7061 7261 6d73  s < 0, 0, params
-000194d0: 292e 7265 7368 6170 6528 582e 7368 6170  ).reshape(X.shap
-000194e0: 655b 315d 2c20 792e 7368 6170 655b 315d  e[1], y.shape[1]
-000194f0: 2929 0d0a 2020 2020 2020 2020 290d 0a20  ))..        ).. 
-00019500: 2020 2029 0d0a 0d0a 0d0a 2320 6163 7475     )......# actu
-00019510: 616c 6c79 2074 6869 7320 6973 206d 6f72  ally this is mor
-00019520: 6520 6c69 6b65 204d 4144 450d 0a64 6566  e like MADE..def
-00019530: 2063 6f73 745f 6675 6e63 7469 6f6e 5f64   cost_function_d
-00019540: 7761 6528 7061 7261 6d73 2c20 582c 2079  wae(params, X, y
-00019550: 293a 0d0a 2020 2020 4120 3d20 790d 0a20  ):..    A = y.. 
-00019560: 2020 2046 203d 206e 702e 646f 7428 582c     F = np.dot(X,
-00019570: 2070 6172 616d 732e 7265 7368 6170 6528   params.reshape(
-00019580: 582e 7368 6170 655b 315d 2c20 792e 7368  X.shape[1], y.sh
-00019590: 6170 655b 315d 2929 0d0a 2020 2020 6c61  ape[1]))..    la
-000195a0: 7374 5f6f 665f 6172 7261 7920 3d20 795b  st_of_array = y[
-000195b0: 5b30 5d20 2b20 6c69 7374 2872 616e 6765  [0] + list(range
-000195c0: 286c 656e 2879 2920 2d20 3129 295d 0d0a  (len(y) - 1))]..
-000195d0: 2020 2020 7265 7475 726e 206e 702e 7375      return np.su
-000195e0: 6d28 0d0a 2020 2020 2020 2020 6e70 2e6e  m(..        np.n
-000195f0: 616e 6d65 616e 280d 0a20 2020 2020 2020  anmean(..       
-00019600: 2020 2020 206e 702e 7768 6572 6528 0d0a       np.where(..
-00019610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019620: 6e70 2e73 6967 6e28 4620 2d20 6c61 7374  np.sign(F - last
-00019630: 5f6f 665f 6172 7261 7929 203d 3d20 6e70  _of_array) == np
-00019640: 2e73 6967 6e28 4120 2d20 6c61 7374 5f6f  .sign(A - last_o
-00019650: 665f 6172 7261 7929 2c0d 0a20 2020 2020  f_array),..     
-00019660: 2020 2020 2020 2020 2020 206e 702e 6162             np.ab
-00019670: 7328 4120 2d20 4629 2c0d 0a20 2020 2020  s(A - F),..     
-00019680: 2020 2020 2020 2020 2020 2028 6e70 2e61             (np.a
-00019690: 6273 2841 202d 2046 2920 2b20 3129 202a  bs(A - F) + 1) *
-000196a0: 2a20 322c 0d0a 2020 2020 2020 2020 2020  * 2,..          
-000196b0: 2020 292c 0d0a 2020 2020 2020 2020 2020    ),..          
-000196c0: 2020 6178 6973 3d30 2c0d 0a20 2020 2020    axis=0,..     
-000196d0: 2020 2029 0d0a 2020 2020 290d 0a0d 0a0d     )..    ).....
-000196e0: 0a64 6566 2063 6f73 745f 6675 6e63 7469  .def cost_functi
-000196f0: 6f6e 5f71 7561 6e74 696c 6528 7061 7261  on_quantile(para
-00019700: 6d73 2c20 582c 2079 2c20 713d 302e 3929  ms, X, y, q=0.9)
-00019710: 3a0d 0a20 2020 2063 7574 203d 2069 6e74  :..    cut = int
-00019720: 2879 2e73 6861 7065 5b30 5d20 2a20 7129  (y.shape[0] * q)
-00019730: 0d0a 2020 2020 7265 7475 726e 206e 702e  ..    return np.
-00019740: 7375 6d28 0d0a 2020 2020 2020 2020 6e70  sum(..        np
-00019750: 2e70 6172 7469 7469 6f6e 280d 0a20 2020  .partition(..   
-00019760: 2020 2020 2020 2020 206e 702e 6162 7328           np.abs(
-00019770: 7920 2d20 6e70 2e64 6f74 2858 2c20 7061  y - np.dot(X, pa
-00019780: 7261 6d73 2e72 6573 6861 7065 2858 2e73  rams.reshape(X.s
-00019790: 6861 7065 5b31 5d2c 2079 2e73 6861 7065  hape[1], y.shape
-000197a0: 5b31 5d29 2929 2c20 6375 742c 2061 7869  [1]))), cut, axi
-000197b0: 733d 300d 0a20 2020 2020 2020 2029 5b30  s=0..        )[0
-000197c0: 3a63 7574 5d0d 0a20 2020 2029 0d0a 0d0a  :cut]..    )....
-000197d0: 0d0a 6465 6620 636f 7374 5f66 756e 6374  ..def cost_funct
-000197e0: 696f 6e5f 6c32 2870 6172 616d 732c 2058  ion_l2(params, X
-000197f0: 2c20 7929 3a0d 0a20 2020 2072 6574 7572  , y):..    retur
-00019800: 6e20 6e70 2e6c 696e 616c 672e 6e6f 726d  n np.linalg.norm
-00019810: 2879 202d 206e 702e 646f 7428 582c 2070  (y - np.dot(X, p
-00019820: 6172 616d 732e 7265 7368 6170 6528 582e  arams.reshape(X.
-00019830: 7368 6170 655b 315d 2c20 792e 7368 6170  shape[1], y.shap
-00019840: 655b 315d 2929 290d 0a0d 0a0d 0a23 2063  e[1])))......# c
-00019850: 6f75 6c64 2064 6f20 7061 7274 6961 6c20  ould do partial 
-00019860: 706f 6f6c 696e 6720 6279 206d 696e 696d  pooling by minim
-00019870: 697a 696e 6720 6120 6675 6e63 7469 6f6e  izing a function
-00019880: 2074 6861 7420 6d69 7865 7320 7368 6172   that mixes shar
-00019890: 6564 2061 6e64 2075 6e73 6861 7265 6420  ed and unshared 
-000198a0: 636f 6566 6669 6369 656e 7473 2028 6d75  coefficients (mu
-000198b0: 6c74 6970 6c69 6361 7469 7665 290d 0a64  ltiplicative)..d
-000198c0: 6566 206c 7374 7371 5f6d 696e 696d 697a  ef lstsq_minimiz
-000198d0: 6528 582c 2079 2c20 6d61 7869 7465 723d  e(X, y, maxiter=
-000198e0: 3135 3030 302c 2063 6f73 745f 6675 6e63  15000, cost_func
-000198f0: 7469 6f6e 3d22 6c31 2229 3a0d 0a20 2020  tion="l1"):..   
-00019900: 2022 2222 416e 7920 636f 7374 2066 756e   """Any cost fun
-00019910: 6374 696f 6e20 7665 7273 696f 6e20 6f66  ction version of
-00019920: 206c 696e 2072 6567 2e22 2222 0d0a 2020   lin reg."""..  
-00019930: 2020 2320 7374 6172 7420 7769 7468 206c    # start with l
-00019940: 7374 7371 2066 6974 2061 7320 6573 7469  stsq fit as esti
-00019950: 6d61 7465 6420 706f 696e 740d 0a20 2020  mated point..   
-00019960: 2078 3020 3d20 6c73 7473 715f 736f 6c76   x0 = lstsq_solv
-00019970: 6528 582c 2079 292e 666c 6174 7465 6e28  e(X, y).flatten(
-00019980: 290d 0a20 2020 2023 2061 7373 756d 696e  )..    # assumin
-00019990: 6720 7363 616c 6564 2c20 7468 6573 6520  g scaled, these 
-000199a0: 7368 6f75 6c64 2062 6520 7265 6173 6f6e  should be reason
-000199b0: 6162 6c65 2062 6f75 6e64 730d 0a20 2020  able bounds..   
-000199c0: 2062 6f75 6e64 7320 3d20 5b28 2d31 302c   bounds = [(-10,
-000199d0: 2031 3029 2066 6f72 2078 2069 6e20 7830   10) for x in x0
-000199e0: 5d0d 0a20 2020 2069 6620 636f 7374 5f66  ]..    if cost_f
-000199f0: 756e 6374 696f 6e20 3d3d 2022 6477 6165  unction == "dwae
-00019a00: 223a 0d0a 2020 2020 2020 2020 626f 756e  ":..        boun
-00019a10: 6473 203d 205b 282d 302e 352c 2031 3029  ds = [(-0.5, 10)
-00019a20: 2066 6f72 2078 2069 6e20 7830 5d0d 0a20   for x in x0].. 
-00019a30: 2020 2020 2020 2063 6f73 745f 6675 6e63         cost_func
-00019a40: 203d 2063 6f73 745f 6675 6e63 7469 6f6e   = cost_function
-00019a50: 5f64 7761 650d 0a20 2020 2065 6c69 6620  _dwae..    elif 
-00019a60: 636f 7374 5f66 756e 6374 696f 6e20 3d3d  cost_function ==
-00019a70: 2022 7175 616e 7469 6c65 223a 0d0a 2020   "quantile":..  
-00019a80: 2020 2020 2020 636f 7374 5f66 756e 6320        cost_func 
-00019a90: 3d20 636f 7374 5f66 756e 6374 696f 6e5f  = cost_function_
-00019aa0: 7175 616e 7469 6c65 0d0a 2020 2020 656c  quantile..    el
-00019ab0: 6966 2063 6f73 745f 6675 6e63 7469 6f6e  if cost_function
-00019ac0: 203d 3d20 226c 315f 706f 7369 7469 7665   == "l1_positive
-00019ad0: 223a 0d0a 2020 2020 2020 2020 626f 756e  ":..        boun
-00019ae0: 6473 203d 205b 2830 2c20 3130 2920 666f  ds = [(0, 10) fo
-00019af0: 7220 7820 696e 2078 305d 0d0a 2020 2020  r x in x0]..    
-00019b00: 2020 2020 636f 7374 5f66 756e 6320 3d20      cost_func = 
-00019b10: 636f 7374 5f66 756e 6374 696f 6e5f 6c31  cost_function_l1
-00019b20: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
-00019b30: 2020 2020 2063 6f73 745f 6675 6e63 203d       cost_func =
-00019b40: 2063 6f73 745f 6675 6e63 7469 6f6e 5f6c   cost_function_l
-00019b50: 310d 0a20 2020 2072 6574 7572 6e20 6d69  1..    return mi
-00019b60: 6e69 6d69 7a65 280d 0a20 2020 2020 2020  nimize(..       
-00019b70: 2063 6f73 745f 6675 6e63 2c20 7830 2c20   cost_func, x0, 
-00019b80: 6172 6773 3d28 582c 2079 292c 2062 6f75  args=(X, y), bou
-00019b90: 6e64 733d 626f 756e 6473 2c20 6f70 7469  nds=bounds, opti
-00019ba0: 6f6e 733d 7b27 6d61 7869 7465 7227 3a20  ons={'maxiter': 
-00019bb0: 6d61 7869 7465 727d 0d0a 2020 2020 292e  maxiter}..    ).
-00019bc0: 782e 7265 7368 6170 6528 582e 7368 6170  x.reshape(X.shap
-00019bd0: 655b 315d 2c20 792e 7368 6170 655b 315d  e[1], y.shape[1]
-00019be0: 290d 0a0d 0a0d 0a64 6566 206c 696e 6561  )......def linea
-00019bf0: 725f 6d6f 6465 6c28 782c 2079 2c20 7061  r_model(x, y, pa
-00019c00: 7261 6d73 293a 0d0a 2020 2020 6d6f 6465  rams):..    mode
-00019c10: 6c5f 7479 7065 203d 2070 6172 616d 732e  l_type = params.
-00019c20: 6765 7428 226d 6f64 656c 222c 2022 6c73  get("model", "ls
-00019c30: 7473 7122 290d 0a20 2020 206c 616d 6264  tsq")..    lambd
-00019c40: 203d 2070 6172 616d 732e 6765 7428 226c   = params.get("l
-00019c50: 616d 6264 6122 2c20 4e6f 6e65 290d 0a20  ambda", None).. 
-00019c60: 2020 2072 6563 203d 2070 6172 616d 732e     rec = params.
-00019c70: 6765 7428 2272 6563 656e 6379 5f77 6569  get("recency_wei
-00019c80: 6768 7469 6e67 222c 204e 6f6e 6529 0d0a  ghting", None)..
-00019c90: 2020 2020 6966 206c 616d 6264 2069 7320      if lambd is 
-00019ca0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00019cb0: 2020 2069 645f 6d61 7420 3d20 6e70 2e7a     id_mat = np.z
-00019cc0: 6572 6f73 2828 782e 7368 6170 655b 315d  eros((x.shape[1]
-00019cd0: 2c20 782e 7368 6170 655b 315d 2929 0d0a  , x.shape[1]))..
-00019ce0: 2020 2020 2020 2020 6e70 2e66 696c 6c5f          np.fill_
-00019cf0: 6469 6167 6f6e 616c 2869 645f 6d61 742c  diagonal(id_mat,
-00019d00: 2031 290d 0a20 2020 2020 2020 2069 645f   1)..        id_
-00019d10: 6d61 745b 302c 2030 5d20 3d20 300d 0a20  mat[0, 0] = 0.. 
-00019d20: 2020 2069 6620 7265 6320 6973 206e 6f74     if rec is not
-00019d30: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00019d40: 7765 6967 6874 7320 3d20 286e 702e 6172  weights = (np.ar
-00019d50: 616e 6765 286c 656e 2878 2929 202b 2031  ange(len(x)) + 1
-00019d60: 2920 2a2a 2072 6563 2020 2320 302e 3035  ) ** rec  # 0.05
-00019d70: 202d 2030 2e32 350d 0a20 2020 2020 2020   - 0.25..       
-00019d80: 2078 203d 2078 202a 2077 6569 6768 7473   x = x * weights
-00019d90: 5b2e 2e2e 2c20 4e6f 6e65 5d0d 0a20 2020  [..., None]..   
-00019da0: 2020 2020 2079 203d 206e 702e 6173 6172       y = np.asar
-00019db0: 7261 7928 7929 202a 2077 6569 6768 7473  ray(y) * weights
-00019dc0: 5b2e 2e2e 2c20 4e6f 6e65 5d0d 0a20 2020  [..., None]..   
-00019dd0: 2069 6620 6d6f 6465 6c5f 7479 7065 203d   if model_type =
-00019de0: 3d20 226c 7374 7371 223a 0d0a 2020 2020  = "lstsq":..    
-00019df0: 2020 2020 6966 206c 616d 6264 2069 7320      if lambd is 
-00019e00: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00019e10: 2020 2020 2020 2072 6574 7572 6e20 6e70         return np
-00019e20: 2e6c 696e 616c 672e 6c73 7473 7128 782e  .linalg.lstsq(x.
-00019e30: 542e 646f 7428 7829 202b 206c 616d 6264  T.dot(x) + lambd
-00019e40: 202a 2069 645f 6d61 742c 2078 2e54 2e64   * id_mat, x.T.d
-00019e50: 6f74 2879 292c 2072 636f 6e64 3d4e 6f6e  ot(y), rcond=Non
-00019e60: 6529 5b0d 0a20 2020 2020 2020 2020 2020  e)[..           
-00019e70: 2020 2020 2030 0d0a 2020 2020 2020 2020       0..        
-00019e80: 2020 2020 5d0d 0a20 2020 2020 2020 2065      ]..        e
-00019e90: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00019ea0: 2020 7265 7475 726e 206e 702e 6c69 6e61    return np.lina
-00019eb0: 6c67 2e6c 7374 7371 2878 2c20 792c 2072  lg.lstsq(x, y, r
-00019ec0: 636f 6e64 3d4e 6f6e 6529 5b30 5d0d 0a20  cond=None)[0].. 
-00019ed0: 2020 2065 6c69 6620 6d6f 6465 6c5f 7479     elif model_ty
-00019ee0: 7065 203d 3d20 226c 696e 616c 675f 736f  pe == "linalg_so
-00019ef0: 6c76 6522 3a0d 0a20 2020 2020 2020 2072  lve":..        r
-00019f00: 6574 7572 6e20 6c73 7473 715f 736f 6c76  eturn lstsq_solv
-00019f10: 6528 782c 2079 2c20 6c61 6d62 3d6c 616d  e(x, y, lamb=lam
-00019f20: 6264 2c20 6964 656e 7469 7479 5f6d 6174  bd, identity_mat
-00019f30: 7269 783d 6964 5f6d 6174 290d 0a20 2020  rix=id_mat)..   
-00019f40: 2065 6c69 6620 6d6f 6465 6c5f 7479 7065   elif model_type
-00019f50: 203d 3d20 226c 315f 6e6f 726d 223a 0d0a   == "l1_norm":..
-00019f60: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-00019f70: 7374 7371 5f6d 696e 696d 697a 6528 0d0a  stsq_minimize(..
-00019f80: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
-00019f90: 7361 7272 6179 2878 292c 0d0a 2020 2020  sarray(x),..    
-00019fa0: 2020 2020 2020 2020 6e70 2e61 7361 7272          np.asarr
-00019fb0: 6179 2879 292c 0d0a 2020 2020 2020 2020  ay(y),..        
-00019fc0: 2020 2020 6d61 7869 7465 723d 7061 7261      maxiter=para
-00019fd0: 6d73 2e67 6574 2822 6d61 7869 7465 7222  ms.get("maxiter"
-00019fe0: 2c20 3135 3030 3029 2c0d 0a20 2020 2020  , 15000),..     
-00019ff0: 2020 2020 2020 2063 6f73 745f 6675 6e63         cost_func
-0001a000: 7469 6f6e 3d22 6c31 222c 0d0a 2020 2020  tion="l1",..    
-0001a010: 2020 2020 290d 0a20 2020 2065 6c69 6620      )..    elif 
-0001a020: 6d6f 6465 6c5f 7479 7065 203d 3d20 2271  model_type == "q
-0001a030: 7561 6e74 696c 655f 6e6f 726d 223a 0d0a  uantile_norm":..
-0001a040: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-0001a050: 7374 7371 5f6d 696e 696d 697a 6528 0d0a  stsq_minimize(..
-0001a060: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
-0001a070: 7361 7272 6179 2878 292c 0d0a 2020 2020  sarray(x),..    
-0001a080: 2020 2020 2020 2020 6e70 2e61 7361 7272          np.asarr
-0001a090: 6179 2879 292c 0d0a 2020 2020 2020 2020  ay(y),..        
-0001a0a0: 2020 2020 6d61 7869 7465 723d 7061 7261      maxiter=para
-0001a0b0: 6d73 2e67 6574 2822 6d61 7869 7465 7222  ms.get("maxiter"
-0001a0c0: 2c20 3135 3030 3029 2c0d 0a20 2020 2020  , 15000),..     
-0001a0d0: 2020 2020 2020 2063 6f73 745f 6675 6e63         cost_func
-0001a0e0: 7469 6f6e 3d22 7175 616e 7469 6c65 222c  tion="quantile",
-0001a0f0: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
-0001a100: 2065 6c69 6620 6d6f 6465 6c5f 7479 7065   elif model_type
-0001a110: 203d 3d20 2264 7761 655f 6e6f 726d 223a   == "dwae_norm":
-0001a120: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001a130: 206c 7374 7371 5f6d 696e 696d 697a 6528   lstsq_minimize(
-0001a140: 0d0a 2020 2020 2020 2020 2020 2020 6e70  ..            np
-0001a150: 2e61 7361 7272 6179 2878 292c 0d0a 2020  .asarray(x),..  
-0001a160: 2020 2020 2020 2020 2020 6e70 2e61 7361            np.asa
-0001a170: 7272 6179 2879 292c 0d0a 2020 2020 2020  rray(y),..      
-0001a180: 2020 2020 2020 6d61 7869 7465 723d 7061        maxiter=pa
-0001a190: 7261 6d73 2e67 6574 2822 6d61 7869 7465  rams.get("maxite
-0001a1a0: 7222 2c20 3135 3030 3029 2c0d 0a20 2020  r", 15000),..   
-0001a1b0: 2020 2020 2020 2020 2063 6f73 745f 6675           cost_fu
-0001a1c0: 6e63 7469 6f6e 3d22 6477 6165 222c 0d0a  nction="dwae",..
-0001a1d0: 2020 2020 2020 2020 290d 0a20 2020 2065          )..    e
-0001a1e0: 6c69 6620 6d6f 6465 6c5f 7479 7065 203d  lif model_type =
-0001a1f0: 3d20 226c 315f 706f 7369 7469 7665 223a  = "l1_positive":
-0001a200: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001a210: 206c 7374 7371 5f6d 696e 696d 697a 6528   lstsq_minimize(
-0001a220: 0d0a 2020 2020 2020 2020 2020 2020 6e70  ..            np
-0001a230: 2e61 7361 7272 6179 2878 292c 0d0a 2020  .asarray(x),..  
-0001a240: 2020 2020 2020 2020 2020 6e70 2e61 7361            np.asa
-0001a250: 7272 6179 2879 292c 0d0a 2020 2020 2020  rray(y),..      
-0001a260: 2020 2020 2020 6d61 7869 7465 723d 7061        maxiter=pa
-0001a270: 7261 6d73 2e67 6574 2822 6d61 7869 7465  rams.get("maxite
-0001a280: 7222 2c20 3135 3030 3029 2c0d 0a20 2020  r", 15000),..   
-0001a290: 2020 2020 2020 2020 2063 6f73 745f 6675           cost_fu
-0001a2a0: 6e63 7469 6f6e 3d22 6c31 5f70 6f73 6974  nction="l1_posit
-0001a2b0: 6976 6522 2c0d 0a20 2020 2020 2020 2029  ive",..        )
-0001a2c0: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
-0001a2d0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0001a2e0: 4572 726f 7228 226c 696e 6561 7220 6d6f  Error("linear mo
-0001a2f0: 6465 6c20 6e6f 7420 7265 636f 676e 697a  del not recogniz
-0001a300: 6564 2229 0d0a 0d0a 0d0a 2320 5365 6173  ed")......# Seas
-0001a310: 6f6e 616c 6974 6965 730d 0a23 2069 6e74  onalities..# int
-0001a320: 6572 6163 7469 6f6e 2065 6666 6563 7420  eraction effect 
-0001a330: 6f6e 6c79 206f 6e20 6669 7273 7420 7477  only on first tw
-0001a340: 6f20 7365 6173 6f6e 616c 6974 6965 7320  o seasonalities 
-0001a350: 6966 206f 7264 6572 206d 6174 6368 6573  if order matches
-0001a360: 0d0a 0d0a 2320 4361 7465 676f 7269 6361  ....# Categorica
-0001a370: 6c20 4665 6174 7572 6573 0d0a 2320 286d  l Features..# (m
-0001a380: 756c 7469 7661 7269 6174 6520 7375 6d6d  ultivariate summ
-0001a390: 6172 6965 7320 6279 2067 726f 7570 290d  aries by group).
-0001a3a0: 0a0d 0a23 2070 6173 7420 696d 7061 6374  ...# past impact
-0001a3b0: 7320 286f 7074 696f 6e20 746f 206e 6f74  s (option to not
-0001a3c0: 2065 6e66 6f72 6365 2c20 6f6e 6c79 2073   enforce, only s
-0001a3d0: 686f 7729 0d0a 0d0a 2320 7768 6174 2069  how)....# what i
-0001a3e0: 7320 7374 696c 6c20 6e65 6564 6564 3a0d  s still needed:.
-0001a3f0: 0a23 2062 6179 6573 6961 6e20 6c69 6e65  .# bayesian line
-0001a400: 6172 206d 6f64 656c 206f 7074 696f 6e73  ar model options
-0001a410: 0d0a 2320 6d6f 7265 206d 756c 7469 7661  ..# more multiva
-0001a420: 7269 6174 6520 7375 6d6d 6172 6965 730d  riate summaries.
-0001a430: 0a23 2061 6464 2061 6e6f 6d61 6c79 2063  .# add anomaly c
-0001a440: 6c61 7373 6966 6965 7220 746f 2066 6f72  lassifier to for
-0001a450: 6563 6173 740d 0a23 2072 6566 696e 6520  ecast..# refine 
-0001a460: 7472 616e 7366 6f72 6d61 7469 6f6e 7320  transformations 
-0001a470: 616e 6420 6d6f 6465 6c73 2067 656e 6572  and models gener
-0001a480: 6174 6564 2062 7920 6765 745f 6e65 775f  ated by get_new_
-0001a490: 7061 7261 6d73 0d0a 2320 7265 7765 6967  params..# reweig
-0001a4a0: 6874 2073 6f20 6c6f 6f70 2069 7320 6e6f  ht so loop is no
-0001a4b0: 7420 7265 7175 6972 6564 2073 6f20 6f66  t required so of
-0001a4c0: 7465 6e0d 0a23 2074 6573 7420 616e 6420  ten..# test and 
-0001a4d0: 6275 6720 6669 7820 6576 6572 7974 6869  bug fix everythi
-0001a4e0: 6e67 0d0a 2320 6c31 5f6e 6f72 6d20 6973  ng..# l1_norm is
-0001a4f0: 6e27 7420 776f 726b 696e 670d 0a23 2075  n't working..# u
-0001a500: 6e69 7474 6573 7473 0d0a 0d0a 2320 5445  nittests....# TE
-0001a510: 5354 0d0a 2320 6e65 775f 6466 0d0a 0d0a  ST..# new_df....
-0001a520: 2320 636f 756c 6420 646f 2070 6172 7469  # could do parti
-0001a530: 616c 2070 6f6f 6c69 6e67 2062 7920 6d69  al pooling by mi
-0001a540: 6e69 6d69 7a69 6e67 2061 2066 756e 6374  nimizing a funct
-0001a550: 696f 6e20 7468 6174 206d 6978 6573 2073  ion that mixes s
-0001a560: 6861 7265 6420 616e 6420 756e 7368 6172  hared and unshar
-0001a570: 6564 2063 6f65 6666 6963 6965 6e74 7320  ed coefficients 
-0001a580: 286d 756c 7469 706c 6963 6174 6976 6529  (multiplicative)
-0001a590: 0d0a 0d0a 2320 7365 6172 6368 2073 7061  ....# search spa
-0001a5a0: 6365 3a0d 0a23 2066 6173 7420 6f6e 206c  ce:..# fast on l
-0001a5b0: 7374 7371 7320 6d6f 6465 6c0d 0a23 2066  stsqs model..# f
-0001a5c0: 756c 6c20 7365 6172 6368 206f 6620 7072  ull search of pr
-0001a5d0: 6564 6566 696e 6564 206f 7074 696f 6e73  edefined options
-0001a5e0: 0d0a 2320 7363 6970 7920 6d69 6e69 6d69  ..# scipy minimi
-0001a5f0: 7a65 2066 6f72 2063 6f6e 7469 6e75 6f75  ze for continuou
-0001a600: 7320 7061 7261 6d73 2c20 6f72 206d 6179  s params, or may
-0001a610: 6265 2069 6e74 2870 6172 616d 2920 666f  be int(param) fo
-0001a620: 7220 6469 7363 7265 7465 2074 6f6f 0d0a  r discrete too..
-0001a630: 2320 6d69 6e69 6d69 7a65 2077 6f72 6b69  # minimize worki
-0001a640: 6e67 2066 6f72 2072 6f6c 6c69 6e67 2077  ng for rolling w
-0001a650: 696e 646f 7720 7369 7a65 2062 7574 206e  indow size but n
-0001a660: 6f74 2066 6f72 2073 6561 736f 6e61 6c69  ot for seasonali
-0001a670: 7479 2028 6163 7475 616c 6c79 2070 726f  ty (actually pro
-0001a680: 6261 626c 7920 7769 6e64 6f77 2069 7320  bably window is 
-0001a690: 6f76 6572 6669 7429 0d0a 2320 646f 2069  overfit)..# do i
-0001a6a0: 7420 7374 6570 7769 7365 3a0d 0a23 2066  t stepwise:..# f
-0001a6b0: 6972 7374 2066 6974 2073 6561 736f 6e61  irst fit seasona
-0001a6c0: 6c69 7479 2028 7769 7468 2066 6c61 6720  lity (with flag 
-0001a6d0: 7265 6772 6573 736f 7273 2062 7574 206e  regressors but n
-0001a6e0: 6f74 206f 7468 6572 7329 0d0a 2320 7365  ot others)..# se
-0001a6f0: 636f 6e64 6c79 2073 6361 6c65 7273 2061  condly scalers a
-0001a700: 6e64 2070 7265 7072 6f63 6573 7369 6e67  nd preprocessing
-0001a710: 2041 4e44 2061 6e6f 6d61 6c79 2064 6574   AND anomaly det
-0001a720: 6563 7469 6f6e 2041 4e44 2068 6f6c 6964  ection AND holid
-0001a730: 6179 2064 6574 6563 7469 6f6e 0d0a 2320  ay detection..# 
-0001a740: 706f 7373 6962 6c79 2061 6464 2033 7264  possibly add 3rd
-0001a750: 2073 6561 736f 6e61 6c69 7479 2061 6674   seasonality aft
-0001a760: 6572 2070 7265 7072 6f63 6573 7369 6e67  er preprocessing
-0001a770: 0d0a 2320 7468 6972 646c 7920 726f 6c6c  ..# thirdly roll
-0001a780: 696e 6720 7769 6e64 6f77 2073 697a 6520  ing window size 
-0001a790: 2869 6e63 6c75 6465 2072 6f6c 6c69 6e67  (include rolling
-0001a7a0: 2077 696e 646f 7720 696e 2069 6e69 7469   window in initi
-0001a7b0: 616c 2058 2061 6674 6572 2074 6869 7329  al X after this)
-0001a7c0: 0d0a 2320 7468 656e 2074 6573 7420 7573  ..# then test us
-0001a7d0: 6572 2072 6567 7265 7373 6f72 2061 6e64  er regressor and
-0001a7e0: 2070 7265 7072 6f63 6573 7369 6e67 0d0a   preprocessing..
-0001a7f0: 2320 7468 656e 2074 6573 7420 4152 206c  # then test AR l
-0001a800: 6167 7320 2864 6f6e 2774 2075 7365 2069  ags (don't use i
-0001a810: 6620 2520 6761 696e 2069 7320 3c20 7820  f % gain is < x 
-0001a820: 2529 0d0a 2320 6f72 206d 6179 6265 2075  %)..# or maybe u
-0001a830: 7365 2061 2072 756e 7469 6d65 2077 6569  se a runtime wei
-0001a840: 6768 7469 6e67 0d0a 2320 7468 656e 206d  ghting..# then m
-0001a850: 756c 7469 7661 7269 6174 6520 7375 6d6d  ultivariate summ
-0001a860: 6172 6965 730d 0a23 2046 494e 414c 4c59  aries..# FINALLY
-0001a870: 2063 6f76 6172 6961 7465 206c 6167 7320   covariate lags 
-0001a880: 2866 6561 7475 7265 2073 656c 6563 7469  (feature selecti
-0001a890: 6f6e 2064 6566 696e 6974 656c 7920 6e65  on definitely ne
-0001a8a0: 6564 6564 290d 0a0d 0a0d 0a69 6620 4661  eded)......if Fa
-0001a8b0: 6c73 653a 0d0a 2020 2020 2320 7465 7374  lse:..    # test
-0001a8c0: 2068 6f6c 6964 6179 2063 6f75 6e74 7269   holiday countri
-0001a8d0: 6573 2c20 7265 6772 6573 736f 7273 2c20  es, regressors, 
-0001a8e0: 696d 7061 6374 730d 0a20 2020 2066 726f  impacts..    fro
-0001a8f0: 6d20 6175 746f 7473 2069 6d70 6f72 7420  m autots import 
-0001a900: 6c6f 6164 5f64 6169 6c79 0d0a 2020 2020  load_daily..    
-0001a910: 696d 706f 7274 206d 6174 706c 6f74 6c69  import matplotli
-0001a920: 622e 7079 706c 6f74 2061 7320 706c 740d  b.pyplot as plt.
-0001a930: 0a0d 0a20 2020 2063 6174 6567 6f72 6963  ...    categoric
-0001a940: 616c 5f67 726f 7570 7320 3d20 7b0d 0a20  al_groups = {.. 
-0001a950: 2020 2020 2020 2022 7769 6b69 5f55 6e69         "wiki_Uni
-0001a960: 7465 645f 5374 6174 6573 223a 2027 636f  ted_States": 'co
-0001a970: 756e 7472 7927 2c0d 0a20 2020 2020 2020  untry',..       
-0001a980: 2022 7769 6b69 5f47 6572 6d61 6e79 223a   "wiki_Germany":
-0001a990: 2027 636f 756e 7472 7927 2c0d 0a20 2020   'country',..   
-0001a9a0: 2020 2020 2022 7769 6b69 5f4a 6573 7573       "wiki_Jesus
-0001a9b0: 223a 2027 686f 6c69 6461 7927 2c0d 0a20  ": 'holiday',.. 
-0001a9c0: 2020 2020 2020 2022 7769 6b69 5f4d 6963         "wiki_Mic
-0001a9d0: 6861 656c 5f4a 6163 6b73 6f6e 223a 2027  hael_Jackson": '
-0001a9e0: 7065 7273 6f6e 272c 0d0a 2020 2020 2020  person',..      
-0001a9f0: 2020 2277 696b 695f 4561 7374 6572 223a    "wiki_Easter":
-0001aa00: 2027 686f 6c69 6461 7927 2c0d 0a20 2020   'holiday',..   
-0001aa10: 2020 2020 2022 7769 6b69 5f43 6872 6973       "wiki_Chris
-0001aa20: 746d 6173 223a 2027 686f 6c69 6461 7927  tmas": 'holiday'
-0001aa30: 2c0d 0a20 2020 2020 2020 2022 7769 6b69  ,..        "wiki
-0001aa40: 5f43 6869 6e65 7365 5f4e 6577 5f59 6561  _Chinese_New_Yea
-0001aa50: 7222 3a20 2768 6f6c 6964 6179 272c 0d0a  r": 'holiday',..
-0001aa60: 2020 2020 2020 2020 2277 696b 695f 5468          "wiki_Th
-0001aa70: 616e 6b73 6769 7669 6e67 223a 2027 686f  anksgiving": 'ho
-0001aa80: 6c69 6461 7927 2c0d 0a20 2020 2020 2020  liday',..       
-0001aa90: 2022 7769 6b69 5f45 6c69 7a61 6265 7468   "wiki_Elizabeth
-0001aaa0: 5f49 4922 3a20 2770 6572 736f 6e27 2c0d  _II": 'person',.
-0001aab0: 0a20 2020 2020 2020 2022 7769 6b69 5f57  .        "wiki_W
-0001aac0: 696c 6c69 616d 5f53 6861 6b65 7370 6561  illiam_Shakespea
-0001aad0: 7265 223a 2027 7065 7273 6f6e 272c 0d0a  re": 'person',..
-0001aae0: 2020 2020 2020 2020 2277 696b 695f 4765          "wiki_Ge
-0001aaf0: 6f72 6765 5f57 6173 6869 6e67 746f 6e22  orge_Washington"
-0001ab00: 3a20 2770 6572 736f 6e27 2c0d 0a20 2020  : 'person',..   
-0001ab10: 2020 2020 2022 7769 6b69 5f43 6c65 6f70       "wiki_Cleop
-0001ab20: 6174 7261 223a 2027 7065 7273 6f6e 272c  atra": 'person',
-0001ab30: 0d0a 2020 2020 7d0d 0a20 2020 2068 6f6c  ..    }..    hol
-0001ab40: 6964 6179 5f63 6f75 6e74 7269 6573 203d  iday_countries =
-0001ab50: 207b 0d0a 2020 2020 2020 2020 2777 696b   {..        'wik
-0001ab60: 695f 456c 697a 6162 6574 685f 4949 273a  i_Elizabeth_II':
-0001ab70: 2027 756b 272c 0d0a 2020 2020 2020 2020   'uk',..        
-0001ab80: 2777 696b 695f 556e 6974 6564 5f53 7461  'wiki_United_Sta
-0001ab90: 7465 7327 3a20 2775 7327 2c0d 0a20 2020  tes': 'us',..   
-0001aba0: 2020 2020 2027 7769 6b69 5f47 6572 6d61       'wiki_Germa
-0001abb0: 6e79 273a 2027 6465 272c 0d0a 2020 2020  ny': 'de',..    
-0001abc0: 7d0d 0a20 2020 2064 665f 6461 696c 7920  }..    df_daily 
-0001abd0: 3d20 6c6f 6164 5f64 6169 6c79 286c 6f6e  = load_daily(lon
-0001abe0: 673d 4661 6c73 6529 0d0a 2020 2020 2320  g=False)..    # 
-0001abf0: 6164 6420 6e61 6e0d 0a20 2020 2064 665f  add nan..    df_
-0001ac00: 6461 696c 792e 696c 6f63 5b31 3030 2c20  daily.iloc[100, 
-0001ac10: 3a5d 203d 206e 702e 6e61 6e0d 0a20 2020  :] = np.nan..   
-0001ac20: 2066 6f72 6563 6173 745f 6c65 6e67 7468   forecast_length
-0001ac30: 203d 2031 3830 0d0a 2020 2020 696e 636c   = 180..    incl
-0001ac40: 7564 655f 6869 7374 6f72 7920 3d20 5472  ude_history = Tr
-0001ac50: 7565 0d0a 2020 2020 6466 5f74 7261 696e  ue..    df_train
-0001ac60: 203d 2064 665f 6461 696c 795b 3a2d 666f   = df_daily[:-fo
-0001ac70: 7265 6361 7374 5f6c 656e 6774 685d 2e69  recast_length].i
-0001ac80: 6c6f 635b 3a2c 2031 3a5d 0d0a 2020 2020  loc[:, 1:]..    
-0001ac90: 6466 5f74 6573 7420 3d20 6466 5f64 6169  df_test = df_dai
-0001aca0: 6c79 5b2d 666f 7265 6361 7374 5f6c 656e  ly[-forecast_len
-0001acb0: 6774 683a 5d2e 696c 6f63 5b3a 2c20 313a  gth:].iloc[:, 1:
-0001acc0: 5d0d 0a20 2020 2066 616b 655f 7265 6772  ]..    fake_regr
-0001acd0: 203d 2064 665f 6461 696c 795b 3a2d 666f   = df_daily[:-fo
-0001ace0: 7265 6361 7374 5f6c 656e 6774 685d 2e69  recast_length].i
-0001acf0: 6c6f 635b 3a2c 2030 3a31 5d0d 0a20 2020  loc[:, 0:1]..   
-0001ad00: 2066 616b 655f 7265 6772 5f66 6373 7420   fake_regr_fcst 
-0001ad10: 3d20 280d 0a20 2020 2020 2020 2064 665f  = (..        df_
-0001ad20: 6461 696c 792e 696c 6f63 5b3a 2c20 303a  daily.iloc[:, 0:
-0001ad30: 315d 0d0a 2020 2020 2020 2020 6966 2069  1]..        if i
-0001ad40: 6e63 6c75 6465 5f68 6973 746f 7279 0d0a  nclude_history..
-0001ad50: 2020 2020 2020 2020 656c 7365 2064 665f          else df_
-0001ad60: 6461 696c 795b 2d66 6f72 6563 6173 745f  daily[-forecast_
-0001ad70: 6c65 6e67 7468 3a5d 2e69 6c6f 635b 3a2c  length:].iloc[:,
-0001ad80: 2030 3a31 5d0d 0a20 2020 2029 0d0a 2020   0:1]..    )..  
-0001ad90: 2020 666c 6167 5f72 6567 7265 7373 6f72    flag_regressor
-0001ada0: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
-0001adb0: 312c 2069 6e64 6578 3d66 616b 655f 7265  1, index=fake_re
-0001adc0: 6772 2e69 6e64 6578 2c20 636f 6c75 6d6e  gr.index, column
-0001add0: 733d 5b22 666c 6167 5f74 6573 7422 5d29  s=["flag_test"])
-0001ade0: 0d0a 2020 2020 666c 6167 5f72 6567 7265  ..    flag_regre
-0001adf0: 7373 6f72 5f66 6373 7420 3d20 7064 2e44  ssor_fcst = pd.D
-0001ae00: 6174 6146 7261 6d65 280d 0a20 2020 2020  ataFrame(..     
-0001ae10: 2020 2031 2c20 696e 6465 783d 6661 6b65     1, index=fake
-0001ae20: 5f72 6567 725f 6663 7374 2e69 6e64 6578  _regr_fcst.index
-0001ae30: 2c20 636f 6c75 6d6e 733d 5b22 666c 6167  , columns=["flag
-0001ae40: 5f74 6573 7422 5d0d 0a20 2020 2029 0d0a  _test"]..    )..
-0001ae50: 2020 2020 7265 6772 5f70 6572 5f73 6572      regr_per_ser
-0001ae60: 6965 7320 3d20 7b0d 0a20 2020 2020 2020  ies = {..       
-0001ae70: 2073 7472 2864 665f 7472 6169 6e2e 636f   str(df_train.co
-0001ae80: 6c75 6d6e 735b 305d 293a 2070 642e 4461  lumns[0]): pd.Da
-0001ae90: 7461 4672 616d 6528 0d0a 2020 2020 2020  taFrame(..      
-0001aea0: 2020 2020 2020 6e70 2e72 616e 646f 6d2e        np.random.
-0001aeb0: 6e6f 726d 616c 2873 697a 653d 286c 656e  normal(size=(len
-0001aec0: 2864 665f 7472 6169 6e29 2c20 3129 292c  (df_train), 1)),
-0001aed0: 2069 6e64 6578 3d64 665f 7472 6169 6e2e   index=df_train.
-0001aee0: 696e 6465 780d 0a20 2020 2020 2020 2029  index..        )
-0001aef0: 0d0a 2020 2020 7d0d 0a20 2020 2072 6567  ..    }..    reg
-0001af00: 725f 7065 725f 7365 7269 6573 5f66 6373  r_per_series_fcs
-0001af10: 7420 3d20 7b0d 0a20 2020 2020 2020 2073  t = {..        s
-0001af20: 7472 2864 665f 7472 6169 6e2e 636f 6c75  tr(df_train.colu
-0001af30: 6d6e 735b 305d 293a 2070 642e 4461 7461  mns[0]): pd.Data
-0001af40: 4672 616d 6528 0d0a 2020 2020 2020 2020  Frame(..        
-0001af50: 2020 2020 6e70 2e72 616e 646f 6d2e 6e6f      np.random.no
-0001af60: 726d 616c 2873 697a 653d 2866 6f72 6563  rmal(size=(forec
-0001af70: 6173 745f 6c65 6e67 7468 2c20 3129 292c  ast_length, 1)),
-0001af80: 2069 6e64 6578 3d64 665f 7465 7374 2e69   index=df_test.i
-0001af90: 6e64 6578 0d0a 2020 2020 2020 2020 290d  ndex..        ).
-0001afa0: 0a20 2020 207d 0d0a 2020 2020 636f 6e73  .    }..    cons
-0001afb0: 7472 6169 6e74 203d 207b 0d0a 2020 2020  traint = {..    
-0001afc0: 2020 2020 2763 6f6e 7374 7261 696e 745f      'constraint_
-0001afd0: 6d65 7468 6f64 273a 2027 7175 616e 7469  method': 'quanti
-0001afe0: 6c65 272c 0d0a 2020 2020 2020 2020 276c  le',..        'l
-0001aff0: 6f77 6572 5f63 6f6e 7374 7261 696e 7427  ower_constraint'
-0001b000: 3a20 302c 0d0a 2020 2020 2020 2020 2775  : 0,..        'u
-0001b010: 7070 6572 5f63 6f6e 7374 7261 696e 7427  pper_constraint'
-0001b020: 3a20 4e6f 6e65 2c0d 0a20 2020 2020 2020  : None,..       
-0001b030: 2022 626f 756e 6473 223a 2054 7275 652c   "bounds": True,
-0001b040: 0d0a 2020 2020 7d0d 0a20 2020 2070 6173  ..    }..    pas
-0001b050: 745f 696d 7061 6374 7320 3d20 7064 2e44  t_impacts = pd.D
-0001b060: 6174 6146 7261 6d65 2830 2c20 696e 6465  ataFrame(0, inde
-0001b070: 783d 6466 5f74 7261 696e 2e69 6e64 6578  x=df_train.index
-0001b080: 2c20 636f 6c75 6d6e 733d 6466 5f74 7261  , columns=df_tra
-0001b090: 696e 2e63 6f6c 756d 6e73 290d 0a20 2020  in.columns)..   
-0001b0a0: 2070 6173 745f 696d 7061 6374 732e 696c   past_impacts.il
-0001b0b0: 6f63 5b2d 3130 3a2c 2030 5d20 3d20 6e70  oc[-10:, 0] = np
-0001b0c0: 2e67 656f 6d73 7061 6365 2831 2c20 3130  .geomspace(1, 10
-0001b0d0: 295b 303a 3130 5d20 2f20 3130 300d 0a20  )[0:10] / 100.. 
-0001b0e0: 2020 2070 6173 745f 696d 7061 6374 732e     past_impacts.
-0001b0f0: 696c 6f63 5b2d 3330 3a2c 202d 315d 203d  iloc[-30:, -1] =
-0001b100: 206e 702e 6c69 6e73 7061 6365 2831 2c20   np.linspace(1, 
-0001b110: 3130 295b 303a 3330 5d20 2f20 2d31 3030  10)[0:30] / -100
-0001b120: 0d0a 2020 2020 6675 7475 7265 5f69 6d70  ..    future_imp
-0001b130: 6163 7473 203d 2070 642e 4461 7461 4672  acts = pd.DataFr
-0001b140: 616d 6528 302c 2069 6e64 6578 3d64 665f  ame(0, index=df_
-0001b150: 7465 7374 2e69 6e64 6578 2c20 636f 6c75  test.index, colu
-0001b160: 6d6e 733d 6466 5f74 6573 742e 636f 6c75  mns=df_test.colu
-0001b170: 6d6e 7329 0d0a 2020 2020 6675 7475 7265  mns)..    future
-0001b180: 5f69 6d70 6163 7473 2e69 6c6f 635b 303a  _impacts.iloc[0:
-0001b190: 3130 2c20 305d 203d 2028 6e70 2e6c 696e  10, 0] = (np.lin
-0001b1a0: 7370 6163 6528 312c 2031 3029 5b30 3a31  space(1, 10)[0:1
-0001b1b0: 305d 202b 2031 3029 202f 2031 3030 0d0a  0] + 10) / 100..
-0001b1c0: 0d0a 2020 2020 635f 7061 7261 6d73 203d  ..    c_params =
-0001b1d0: 2043 6173 7361 6e64 7261 2829 2e67 6574   Cassandra().get
-0001b1e0: 5f6e 6577 5f70 6172 616d 7328 290d 0a0d  _new_params()...
-0001b1f0: 0a20 2020 206d 6f64 203d 2043 6173 7361  .    mod = Cassa
-0001b200: 6e64 7261 280d 0a20 2020 2020 2020 206e  ndra(..        n
-0001b210: 5f6a 6f62 733d 312c 0d0a 2020 2020 2020  _jobs=1,..      
-0001b220: 2020 2a2a 635f 7061 7261 6d73 2c0d 0a20    **c_params,.. 
-0001b230: 2020 2020 2020 2063 6f6e 7374 7261 696e         constrain
-0001b240: 743d 636f 6e73 7472 6169 6e74 2c0d 0a20  t=constraint,.. 
-0001b250: 2020 2020 2020 2068 6f6c 6964 6179 5f63         holiday_c
-0001b260: 6f75 6e74 7269 6573 3d68 6f6c 6964 6179  ountries=holiday
-0001b270: 5f63 6f75 6e74 7269 6573 2c0d 0a20 2020  _countries,..   
-0001b280: 2020 2020 206d 6178 5f6d 756c 7469 636f       max_multico
-0001b290: 6c69 6e65 6172 6974 793d 302e 3030 3031  linearity=0.0001
-0001b2a0: 2c0d 0a20 2020 2029 0d0a 2020 2020 6d6f  ,..    )..    mo
-0001b2b0: 642e 6669 7428 0d0a 2020 2020 2020 2020  d.fit(..        
-0001b2c0: 6466 5f74 7261 696e 2c0d 0a20 2020 2020  df_train,..     
-0001b2d0: 2020 2063 6174 6567 6f72 6963 616c 5f67     categorical_g
-0001b2e0: 726f 7570 733d 6361 7465 676f 7269 6361  roups=categorica
-0001b2f0: 6c5f 6772 6f75 7073 2c0d 0a20 2020 2020  l_groups,..     
-0001b300: 2020 2066 7574 7572 655f 7265 6772 6573     future_regres
-0001b310: 736f 723d 6661 6b65 5f72 6567 722c 0d0a  sor=fake_regr,..
-0001b320: 2020 2020 2020 2020 7265 6772 6573 736f          regresso
-0001b330: 725f 7065 725f 7365 7269 6573 3d72 6567  r_per_series=reg
-0001b340: 725f 7065 725f 7365 7269 6573 2c0d 0a20  r_per_series,.. 
-0001b350: 2020 2020 2020 2070 6173 745f 696d 7061         past_impa
-0001b360: 6374 733d 7061 7374 5f69 6d70 6163 7473  cts=past_impacts
-0001b370: 2c0d 0a20 2020 2020 2020 2066 6c61 675f  ,..        flag_
-0001b380: 7265 6772 6573 736f 7273 3d66 6c61 675f  regressors=flag_
-0001b390: 7265 6772 6573 736f 722c 0d0a 2020 2020  regressor,..    
-0001b3a0: 290d 0a20 2020 2070 7265 6420 3d20 6d6f  )..    pred = mo
-0001b3b0: 642e 7072 6564 6963 7428 0d0a 2020 2020  d.predict(..    
-0001b3c0: 2020 2020 666f 7265 6361 7374 5f6c 656e      forecast_len
-0001b3d0: 6774 683d 666f 7265 6361 7374 5f6c 656e  gth=forecast_len
-0001b3e0: 6774 682c 0d0a 2020 2020 2020 2020 696e  gth,..        in
-0001b3f0: 636c 7564 655f 6869 7374 6f72 793d 696e  clude_history=in
-0001b400: 636c 7564 655f 6869 7374 6f72 792c 0d0a  clude_history,..
-0001b410: 2020 2020 2020 2020 6675 7475 7265 5f72          future_r
-0001b420: 6567 7265 7373 6f72 3d66 616b 655f 7265  egressor=fake_re
-0001b430: 6772 5f66 6373 742c 0d0a 2020 2020 2020  gr_fcst,..      
-0001b440: 2020 7265 6772 6573 736f 725f 7065 725f    regressor_per_
-0001b450: 7365 7269 6573 3d72 6567 725f 7065 725f  series=regr_per_
-0001b460: 7365 7269 6573 5f66 6373 742c 0d0a 2020  series_fcst,..  
-0001b470: 2020 2020 2020 6675 7475 7265 5f69 6d70        future_imp
-0001b480: 6163 7473 3d66 7574 7572 655f 696d 7061  acts=future_impa
-0001b490: 6374 732c 0d0a 2020 2020 2020 2020 666c  cts,..        fl
-0001b4a0: 6167 5f72 6567 7265 7373 6f72 733d 666c  ag_regressors=fl
-0001b4b0: 6167 5f72 6567 7265 7373 6f72 5f66 6373  ag_regressor_fcs
-0001b4c0: 742c 0d0a 2020 2020 2020 2020 696e 636c  t,..        incl
-0001b4d0: 7564 655f 6f72 6761 6e69 633d 5472 7565  ude_organic=True
-0001b4e0: 2c0d 0a20 2020 2029 0d0a 2020 2020 7265  ,..    )..    re
-0001b4f0: 7375 6c74 203d 2070 7265 642e 666f 7265  sult = pred.fore
-0001b500: 6361 7374 0d0a 2020 2020 7365 7269 6573  cast..    series
-0001b510: 203d 2072 616e 646f 6d2e 6368 6f69 6365   = random.choice
-0001b520: 286d 6f64 2e63 6f6c 756d 6e5f 6e61 6d65  (mod.column_name
-0001b530: 7329 0d0a 2020 2020 2320 7365 7269 6573  s)..    # series
-0001b540: 203d 2022 7769 6b69 5f50 6572 696f 6469   = "wiki_Periodi
-0001b550: 635f 7461 626c 6522 0d0a 2020 2020 7365  c_table"..    se
-0001b560: 7269 6573 203d 2027 7769 6b69 5f61 6c6c  ries = 'wiki_all
-0001b570: 270d 0a20 2020 206d 6f64 2e72 6567 7265  '..    mod.regre
-0001b580: 7373 6f72 735f 7573 6564 0d0a 2020 2020  ssors_used..    
-0001b590: 6d6f 642e 686f 6c69 6461 795f 636f 756e  mod.holiday_coun
-0001b5a0: 7472 6965 735f 7573 6564 0d0a 2020 2020  tries_used..    
-0001b5b0: 7769 7468 2070 6c74 2e73 7479 6c65 2e63  with plt.style.c
-0001b5c0: 6f6e 7465 7874 2822 7365 6162 6f72 6e2d  ontext("seaborn-
-0001b5d0: 7768 6974 6522 293a 0d0a 2020 2020 2020  white"):..      
-0001b5e0: 2020 7374 6172 745f 6461 7465 203d 2022    start_date = "
-0001b5f0: 3230 3139 2d30 372d 3031 220d 0a20 2020  2019-07-01"..   
-0001b600: 2020 2020 206d 6f64 2e70 6c6f 745f 666f       mod.plot_fo
-0001b610: 7265 6361 7374 280d 0a20 2020 2020 2020  recast(..       
-0001b620: 2020 2020 2070 7265 642c 0d0a 2020 2020       pred,..    
-0001b630: 2020 2020 2020 2020 6163 7475 616c 733d          actuals=
-0001b640: 6466 5f64 6169 6c79 2069 6620 696e 636c  df_daily if incl
-0001b650: 7564 655f 6869 7374 6f72 7920 656c 7365  ude_history else
-0001b660: 2064 665f 7465 7374 2c0d 0a20 2020 2020   df_test,..     
-0001b670: 2020 2020 2020 2073 6572 6965 733d 7365         series=se
-0001b680: 7269 6573 2c0d 0a20 2020 2020 2020 2020  ries,..         
-0001b690: 2020 2073 7461 7274 5f64 6174 653d 7374     start_date=st
-0001b6a0: 6172 745f 6461 7465 2c0d 0a20 2020 2020  art_date,..     
-0001b6b0: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
-0001b6c0: 2320 706c 742e 7368 6f77 2829 0d0a 2020  # plt.show()..  
-0001b6d0: 2020 2020 2020 2320 706c 742e 7361 7665        # plt.save
-0001b6e0: 6669 6728 2243 6173 7361 6e64 7261 5f66  fig("Cassandra_f
-0001b6f0: 6f72 6563 6173 742e 706e 6722 2c20 6470  orecast.png", dp
-0001b700: 693d 3330 3029 0d0a 2020 2020 2020 2020  i=300)..        
-0001b710: 2320 6d6f 642e 706c 6f74 5f63 6f6d 706f  # mod.plot_compo
-0001b720: 6e65 6e74 7328 7072 6564 2c20 7365 7269  nents(pred, seri
-0001b730: 6573 3d73 6572 6965 732c 2074 6f5f 6f72  es=series, to_or
-0001b740: 6967 696e 5f73 7061 6365 3d46 616c 7365  igin_space=False
-0001b750: 290d 0a20 2020 2020 2020 2023 2070 6c74  )..        # plt
-0001b760: 2e73 686f 7728 290d 0a20 2020 2020 2020  .show()..       
-0001b770: 206d 6f64 2e70 6c6f 745f 636f 6d70 6f6e   mod.plot_compon
-0001b780: 656e 7473 280d 0a20 2020 2020 2020 2020  ents(..         
-0001b790: 2020 2070 7265 642c 2073 6572 6965 733d     pred, series=
-0001b7a0: 7365 7269 6573 2c20 746f 5f6f 7269 6769  series, to_origi
-0001b7b0: 6e5f 7370 6163 653d 5472 7565 2c20 7374  n_space=True, st
-0001b7c0: 6172 745f 6461 7465 3d73 7461 7274 5f64  art_date=start_d
-0001b7d0: 6174 650d 0a20 2020 2020 2020 2029 0d0a  ate..        )..
-0001b7e0: 2020 2020 2020 2020 2320 706c 742e 7361          # plt.sa
-0001b7f0: 7665 6669 6728 2243 6173 7361 6e64 7261  vefig("Cassandra
-0001b800: 5f63 6f6d 706f 6e65 6e74 7333 2e70 6e67  _components3.png
-0001b810: 222c 2064 7069 3d33 3030 2c20 6262 6f78  ", dpi=300, bbox
-0001b820: 5f69 6e63 6865 733d 2274 6967 6874 2229  _inches="tight")
-0001b830: 0d0a 2020 2020 2020 2020 706c 742e 7368  ..        plt.sh
-0001b840: 6f77 2829 0d0a 2020 2020 2020 2020 6d6f  ow()..        mo
-0001b850: 642e 706c 6f74 5f74 7265 6e64 280d 0a20  d.plot_trend(.. 
-0001b860: 2020 2020 2020 2020 2020 2073 6572 6965             serie
-0001b870: 733d 7365 7269 6573 2c20 766c 696e 653d  s=series, vline=
-0001b880: 7265 7375 6c74 2e69 6e64 6578 5b2d 666f  result.index[-fo
-0001b890: 7265 6361 7374 5f6c 656e 6774 685d 2c20  recast_length], 
-0001b8a0: 7374 6172 745f 6461 7465 3d73 7461 7274  start_date=start
-0001b8b0: 5f64 6174 650d 0a20 2020 2020 2020 2029  _date..        )
-0001b8c0: 0d0a 2020 2020 2020 2020 2320 706c 742e  ..        # plt.
-0001b8d0: 7361 7665 6669 6728 2243 6173 7361 6e64  savefig("Cassand
-0001b8e0: 7261 5f74 7265 6e64 2e70 6e67 222c 2064  ra_trend.png", d
-0001b8f0: 7069 3d33 3030 2c20 6262 6f78 5f69 6e63  pi=300, bbox_inc
-0001b900: 6865 733d 2274 6967 6874 2229 0d0a 2020  hes="tight")..  
-0001b910: 2020 7072 6564 2e65 7661 6c75 6174 6528    pred.evaluate(
-0001b920: 0d0a 2020 2020 2020 2020 6466 5f64 6169  ..        df_dai
-0001b930: 6c79 2e72 6569 6e64 6578 2872 6573 756c  ly.reindex(resul
-0001b940: 742e 696e 6465 7829 5b64 665f 7472 6169  t.index)[df_trai
-0001b950: 6e2e 636f 6c75 6d6e 735d 0d0a 2020 2020  n.columns]..    
-0001b960: 2020 2020 6966 2069 6e63 6c75 6465 5f68      if include_h
-0001b970: 6973 746f 7279 0d0a 2020 2020 2020 2020  istory..        
-0001b980: 656c 7365 2064 665f 7465 7374 5b64 665f  else df_test[df_
-0001b990: 7472 6169 6e2e 636f 6c75 6d6e 735d 0d0a  train.columns]..
-0001b9a0: 2020 2020 290d 0a20 2020 2070 7269 6e74      )..    print
-0001b9b0: 2870 7265 642e 6176 675f 6d65 7472 6963  (pred.avg_metric
-0001b9c0: 732e 726f 756e 6428 3129 290d 0a0d 0a20  s.round(1)).... 
-0001b9d0: 2020 2023 2069 6620 6e6f 7420 6d6f 642e     # if not mod.
-0001b9e0: 7265 6772 6573 736f 7273 5f75 7365 643a  regressors_used:
-0001b9f0: 0d0a 2020 2020 6461 7465 7320 3d20 6466  ..    dates = df
-0001ba00: 5f64 6169 6c79 2e69 6e64 6578 2e75 6e69  _daily.index.uni
-0001ba10: 6f6e 280d 0a20 2020 2020 2020 206d 6f64  on(..        mod
-0001ba20: 2e63 7265 6174 655f 666f 7265 6361 7374  .create_forecast
-0001ba30: 5f69 6e64 6578 2866 6f72 6563 6173 745f  _index(forecast_
-0001ba40: 6c65 6e67 7468 2c20 6c61 7374 5f64 6174  length, last_dat
-0001ba50: 653d 6466 5f64 6169 6c79 2e69 6e64 6578  e=df_daily.index
-0001ba60: 5b2d 315d 290d 0a20 2020 2029 0d0a 2020  [-1])..    )..  
-0001ba70: 2020 7265 6772 5f70 7320 3d20 7b0d 0a20    regr_ps = {.. 
-0001ba80: 2020 2020 2020 2027 7769 6b69 5f47 6572         'wiki_Ger
-0001ba90: 6d61 6e79 273a 2072 6567 725f 7065 725f  many': regr_per_
-0001baa0: 7365 7269 6573 5f66 6373 745b 2777 696b  series_fcst['wik
-0001bab0: 695f 4765 726d 616e 7927 5d2e 7265 696e  i_Germany'].rein
-0001bac0: 6465 7828 0d0a 2020 2020 2020 2020 2020  dex(..          
-0001bad0: 2020 6461 7465 732c 2066 696c 6c5f 7661    dates, fill_va
-0001bae0: 6c75 653d 300d 0a20 2020 2020 2020 2029  lue=0..        )
-0001baf0: 0d0a 2020 2020 7d0d 0a20 2020 2070 7265  ..    }..    pre
-0001bb00: 6432 203d 206d 6f64 2e70 7265 6469 6374  d2 = mod.predict
-0001bb10: 280d 0a20 2020 2020 2020 2066 6f72 6563  (..        forec
-0001bb20: 6173 745f 6c65 6e67 7468 3d66 6f72 6563  ast_length=forec
-0001bb30: 6173 745f 6c65 6e67 7468 2c0d 0a20 2020  ast_length,..   
-0001bb40: 2020 2020 2069 6e63 6c75 6465 5f68 6973       include_his
-0001bb50: 746f 7279 3d54 7275 652c 0d0a 2020 2020  tory=True,..    
-0001bb60: 2020 2020 6e65 775f 6466 3d64 665f 6461      new_df=df_da
-0001bb70: 696c 795b 6466 5f74 7261 696e 2e63 6f6c  ily[df_train.col
-0001bb80: 756d 6e73 5d2c 0d0a 2020 2020 2020 2020  umns],..        
-0001bb90: 666c 6167 5f72 6567 7265 7373 6f72 733d  flag_regressors=
-0001bba0: 666c 6167 5f72 6567 7265 7373 6f72 5f66  flag_regressor_f
-0001bbb0: 6373 742e 7265 696e 6465 7828 6461 7465  cst.reindex(date
-0001bbc0: 732c 2066 696c 6c5f 7661 6c75 653d 3029  s, fill_value=0)
-0001bbd0: 2c0d 0a20 2020 2020 2020 2066 7574 7572  ,..        futur
-0001bbe0: 655f 7265 6772 6573 736f 723d 6661 6b65  e_regressor=fake
-0001bbf0: 5f72 6567 725f 6663 7374 2e72 6569 6e64  _regr_fcst.reind
-0001bc00: 6578 2864 6174 6573 2c20 6669 6c6c 5f76  ex(dates, fill_v
-0001bc10: 616c 7565 3d30 292c 0d0a 2020 2020 2020  alue=0),..      
-0001bc20: 2020 7265 6772 6573 736f 725f 7065 725f    regressor_per_
-0001bc30: 7365 7269 6573 3d72 6567 725f 7073 2c0d  series=regr_ps,.
-0001bc40: 0a20 2020 2029 0d0a 2020 2020 6d6f 642e  .    )..    mod.
-0001bc50: 706c 6f74 5f66 6f72 6563 6173 7428 7072  plot_forecast(pr
-0001bc60: 6564 322c 2061 6374 7561 6c73 3d64 665f  ed2, actuals=df_
-0001bc70: 6461 696c 792c 2073 6572 6965 733d 7365  daily, series=se
-0001bc80: 7269 6573 2c20 7374 6172 745f 6461 7465  ries, start_date
-0001bc90: 3d73 7461 7274 5f64 6174 6529 0d0a 2020  =start_date)..  
-0001bca0: 2020 6d6f 642e 7265 7475 726e 5f63 6f6d    mod.return_com
-0001bcb0: 706f 6e65 6e74 7328 290d 0a20 2020 2070  ponents()..    p
-0001bcc0: 7269 6e74 2863 5f70 6172 616d 735b 2774  rint(c_params['t
-0001bcd0: 7265 6e64 5f6d 6f64 656c 275d 290d 0a0d  rend_model'])...
-0001bce0: 0a23 204d 554c 5449 504c 4943 4154 4956  .# MULTIPLICATIV
-0001bcf0: 4520 5345 4153 4f4e 414c 4954 5920 414e  E SEASONALITY AN
-0001bd00: 4420 484f 4c49 4441 5953 0d0a 0d0a 2320  D HOLIDAYS....# 
-0001bd10: 6c6f 7720 6d65 6d6f 7279 206f 7074 696f  low memory optio
-0001bd20: 6e20 746f 2064 656c 6574 6520 7374 6f72  n to delete stor
-0001bd30: 6564 2064 6673 2061 6e64 2061 7272 6179  ed dfs and array
-0001bd40: 7320 6173 2073 6f6f 6e20 6173 2070 6f73  s as soon as pos
-0001bd50: 7369 626c 650d 0a0d 0a23 204d 616b 6520  sible....# Make 
-0001bd60: 7375 7265 2078 2066 6561 7475 7265 7320  sure x features 
-0001bd70: 6172 6520 616c 6c20 7363 616c 6564 0d0a  are all scaled..
-0001bd80: 2320 5265 6d6f 7665 2073 6561 736f 6e61  # Remove seasona
-0001bd90: 6c69 7479 2066 726f 6d20 7265 6772 6573  lity from regres
-0001bda0: 736f 7273 0d0a 0d0a 2320 7472 616e 7366  sors....# transf
-0001bdb0: 6572 206c 6561 726e 696e 670d 0a23 2067  er learning..# g
-0001bdc0: 7261 7068 6963 7320 2841 4d46 4d20 7761  raphics (AMFM wa
-0001bdd0: 7465 726d 6172 6b29 0d0a 2320 636f 6d70  termark)..# comp
-0001bde0: 6172 6520 6163 726f 7373 2070 6173 7420  are across past 
-0001bdf0: 666f 7265 6361 7374 730d 0a23 2073 7461  forecasts..# sta
-0001be00: 6269 6c69 7479 0d0a 2320 6d61 6b65 2069  bility..# make i
-0001be10: 7420 6d6f 7265 206d 6f64 756c 6172 2028  t more modular (
-0001be20: 7365 7061 7261 7465 2075 7361 626c 6520  separate usable 
-0001be30: 6675 6e63 7469 6f6e 7329 0d0a 0d0a 2320  functions)....# 
-0001be40: 4175 746f 6d61 7469 6f6e 0d0a 2320 616c  Automation..# al
-0001be50: 6c6f 7720 736f 6d65 2063 6f6e 6669 6720  low some config 
-0001be60: 696e 7075 7473 2c20 6f72 2061 7574 6f6d  inputs, or autom
-0001be70: 6174 6564 2066 6974 0d0a 2320 6f75 7470  ated fit..# outp
-0001be80: 7574 2074 6f20 7461 626c 650d 0a23 2063  ut to table..# c
-0001be90: 6f6d 7061 7265 2063 6f65 6666 6963 6965  ompare coefficie
-0001bea0: 6e74 7320 6368 616e 6765 206f 7665 7220  nts change over 
-0001beb0: 7469 6d65 2c20 6163 6375 7261 6379 206f  time, accuracy o
-0001bec0: 7665 7220 7469 6d65 0d0a 2320 636f 6d70  ver time..# comp
-0001bed0: 6172 696e 6720 6469 6666 6572 656e 7420  aring different 
-0001bee0: 736f 7572 6365 733f 2061 6e64 2f6f 7220  sources? and/or 
-0001bef0: 616c 6c6f 7769 6e67 206f 6e65 2066 6f72  allowing one for
-0001bf00: 6563 6173 7420 746f 2062 6520 7573 6564  ecast to be used
-0001bf10: 2061 7320 6120 7265 6772 6573 736f 7220   as a regressor 
-0001bf20: 666f 7220 616e 6f74 6865 720d 0a23 2077  for another..# w
-0001bf30: 6f75 6c64 2061 6c6c 6f77 2066 6f72 2065  ould allow for e
-0001bf40: 6172 6c69 6572 2064 6574 6563 7469 6f6e  arlier detection
-0001bf50: 206f 6620 6272 6f6b 656e 2063 6f6e 6e65   of broken conne
-0001bf60: 6374 696f 6e73 0d0a 0d0a 2222 220d 0a61  ctions...."""..a
-0001bf70: 7820 3d20 7072 6564 2e70 6c6f 7428 6466  x = pred.plot(df
-0001bf80: 5f64 6169 6c79 2069 6620 696e 636c 7564  _daily if includ
-0001bf90: 655f 6869 7374 6f72 7920 656c 7365 2064  e_history else d
-0001bfa0: 665f 7465 7374 2c20 7365 7269 6573 3d73  f_test, series=s
-0001bfb0: 6572 6965 732c 2076 6c69 6e65 3d64 665f  eries, vline=df_
-0001bfc0: 7465 7374 2e69 6e64 6578 5b30 5d2c 2073  test.index[0], s
-0001bfd0: 7461 7274 5f64 6174 653d 7374 6172 745f  tart_date=start_
-0001bfe0: 6461 7465 290d 0a68 616e 646c 6573 2c20  date)..handles, 
-0001bff0: 6c61 6265 6c73 203d 2061 782e 6765 745f  labels = ax.get_
-0001c000: 6c65 6765 6e64 5f68 616e 646c 6573 5f6c  legend_handles_l
-0001c010: 6162 656c 7328 290d 0a69 6620 6d6f 642e  abels()..if mod.
-0001c020: 616e 6f6d 616c 795f 6465 7465 6374 6f72  anomaly_detector
-0001c030: 3a0d 0a20 2020 2069 6620 6d6f 642e 616e  :..    if mod.an
-0001c040: 6f6d 616c 795f 6465 7465 6374 6f72 2e6f  omaly_detector.o
-0001c050: 7574 7075 7420 3d3d 2022 756e 6976 6172  utput == "univar
-0001c060: 6961 7465 223a 0d0a 2020 2020 2020 2020  iate":..        
-0001c070: 695f 616e 6f6d 203d 206d 6f64 2e61 6e6f  i_anom = mod.ano
-0001c080: 6d61 6c79 5f64 6574 6563 746f 722e 616e  maly_detector.an
-0001c090: 6f6d 616c 6965 732e 696e 6465 785b 6d6f  omalies.index[mo
-0001c0a0: 642e 616e 6f6d 616c 795f 6465 7465 6374  d.anomaly_detect
-0001c0b0: 6f72 2e61 6e6f 6d61 6c69 6573 2e69 6c6f  or.anomalies.ilo
-0001c0c0: 635b 3a2c 2030 5d20 3d3d 202d 315d 0d0a  c[:, 0] == -1]..
-0001c0d0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0001c0e0: 2020 2073 6572 6965 735f 616e 6f6d 203d     series_anom =
-0001c0f0: 206d 6f64 2e61 6e6f 6d61 6c79 5f64 6574   mod.anomaly_det
-0001c100: 6563 746f 722e 616e 6f6d 616c 6965 735b  ector.anomalies[
-0001c110: 7365 7269 6573 5d0d 0a20 2020 2020 2020  series]..       
-0001c120: 2069 5f61 6e6f 6d20 3d20 7365 7269 6573   i_anom = series
-0001c130: 5f61 6e6f 6d5b 7365 7269 6573 5f61 6e6f  _anom[series_ano
-0001c140: 6d20 3d3d 202d 315d 2e69 6e64 6578 0d0a  m == -1].index..
-0001c150: 2020 2020 2020 2020 695f 616e 6f6d 203d          i_anom =
-0001c160: 2069 5f61 6e6f 6d5b 695f 616e 6f6d 203e   i_anom[i_anom >
-0001c170: 3d20 7374 6172 745f 6461 7465 5d0d 0a20  = start_date].. 
-0001c180: 2020 2069 6620 6c65 6e28 695f 616e 6f6d     if len(i_anom
-0001c190: 2920 3e20 3020 616e 6420 6c65 6e28 695f  ) > 0 and len(i_
-0001c1a0: 616e 6f6d 2920 3c20 6c65 6e28 6466 5f64  anom) < len(df_d
-0001c1b0: 6169 6c79 2920 2a20 302e 353a 0d0a 2020  aily) * 0.5:..  
-0001c1c0: 2020 2020 2020 7363 6174 3120 3d20 6178        scat1 = ax
-0001c1d0: 2e73 6361 7474 6572 2869 5f61 6e6f 6d2e  .scatter(i_anom.
-0001c1e0: 746f 6c69 7374 2829 2c20 6466 5f64 6169  tolist(), df_dai
-0001c1f0: 6c79 2e6c 6f63 5b69 5f61 6e6f 6d2c 203a  ly.loc[i_anom, :
-0001c200: 5d5b 7365 7269 6573 5d2c 2063 3d22 6461  ][series], c="da
-0001c210: 726b 736c 6174 6562 6c75 6522 2c20 733d  rkslateblue", s=
-0001c220: 3132 2e30 290d 0a20 2020 2020 2020 2068  12.0)..        h
-0001c230: 616e 646c 6573 202b 3d20 5b73 6361 7431  andles += [scat1
-0001c240: 5d0d 0a20 2020 2020 2020 206c 6162 656c  ]..        label
-0001c250: 7320 2b3d 205b 2261 6e6f 6d61 6c69 6573  s += ["anomalies
-0001c260: 225d 0d0a 6966 206d 6f64 2e68 6f6c 6964  "]..if mod.holid
-0001c270: 6179 5f64 6574 6563 746f 723a 0d0a 2020  ay_detector:..  
-0001c280: 2020 695f 616e 6f6d 203d 206d 6f64 2e68    i_anom = mod.h
-0001c290: 6f6c 6964 6179 5f64 6574 6563 746f 722e  oliday_detector.
-0001c2a0: 6461 7465 735f 746f 5f68 6f6c 6964 6179  dates_to_holiday
-0001c2b0: 7328 6d6f 642e 6466 2e69 6e64 6578 2c20  s(mod.df.index, 
-0001c2c0: 7374 796c 653d 2273 6572 6965 735f 666c  style="series_fl
-0001c2d0: 6167 2229 5b73 6572 6965 735d 0d0a 2020  ag")[series]..  
-0001c2e0: 2020 695f 616e 6f6d 203d 2069 5f61 6e6f    i_anom = i_ano
-0001c2f0: 6d2e 696e 6465 785b 695f 616e 6f6d 203d  m.index[i_anom =
-0001c300: 3d20 315d 0d0a 2020 2020 6966 206c 656e  = 1]..    if len
-0001c310: 2869 5f61 6e6f 6d29 203e 2030 2061 6e64  (i_anom) > 0 and
-0001c320: 206c 656e 2869 5f61 6e6f 6d29 203c 206c   len(i_anom) < l
-0001c330: 656e 2864 665f 6461 696c 7929 202a 2030  en(df_daily) * 0
-0001c340: 2e35 3a0d 0a20 2020 2020 2020 2073 6361  .5:..        sca
-0001c350: 7432 203d 2061 782e 7363 6174 7465 7228  t2 = ax.scatter(
-0001c360: 695f 616e 6f6d 2e74 6f6c 6973 7428 292c  i_anom.tolist(),
-0001c370: 2064 665f 6461 696c 792e 6c6f 635b 695f   df_daily.loc[i_
-0001c380: 616e 6f6d 2c20 3a5d 5b73 6572 6965 735d  anom, :][series]
-0001c390: 2c20 633d 2264 6172 6b67 7265 656e 222c  , c="darkgreen",
-0001c3a0: 2073 3d31 322e 3029 0d0a 2020 2020 2020   s=12.0)..      
-0001c3b0: 2020 6861 6e64 6c65 7320 2b3d 205b 7363    handles += [sc
-0001c3c0: 6174 325d 0d0a 2020 2020 2020 2020 6c61  at2]..        la
-0001c3d0: 6265 6c73 202b 3d20 5b22 6465 7465 6374  bels += ["detect
-0001c3e0: 6564 2068 6f6c 6964 6179 7322 5d0d 0a69  ed holidays"]..i
-0001c3f0: 6620 6d6f 642e 7472 656e 645f 616e 6f6d  f mod.trend_anom
-0001c400: 616c 795f 6465 7465 6374 6f72 2069 7320  aly_detector is 
-0001c410: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2069  not None:..    i
-0001c420: 6620 6d6f 642e 7472 656e 645f 616e 6f6d  f mod.trend_anom
-0001c430: 616c 795f 6465 7465 6374 6f72 2e6f 7574  aly_detector.out
-0001c440: 7075 7420 3d3d 2022 756e 6976 6172 6961  put == "univaria
-0001c450: 7465 223a 0d0a 2020 2020 2020 2020 695f  te":..        i_
-0001c460: 616e 6f6d 203d 206d 6f64 2e74 7265 6e64  anom = mod.trend
-0001c470: 5f61 6e6f 6d61 6c79 5f64 6574 6563 746f  _anomaly_detecto
-0001c480: 722e 616e 6f6d 616c 6965 732e 696e 6465  r.anomalies.inde
-0001c490: 785b 6d6f 642e 616e 6f6d 616c 795f 6465  x[mod.anomaly_de
-0001c4a0: 7465 6374 6f72 2e61 6e6f 6d61 6c69 6573  tector.anomalies
-0001c4b0: 2e69 6c6f 635b 3a2c 2030 5d20 3d3d 202d  .iloc[:, 0] == -
-0001c4c0: 315d 0d0a 2020 2020 656c 7365 3a0d 0a20  1]..    else:.. 
-0001c4d0: 2020 2020 2020 2073 6572 6965 735f 616e         series_an
-0001c4e0: 6f6d 203d 206d 6f64 2e74 7265 6e64 5f61  om = mod.trend_a
-0001c4f0: 6e6f 6d61 6c79 5f64 6574 6563 746f 722e  nomaly_detector.
-0001c500: 616e 6f6d 616c 6965 735b 7365 7269 6573  anomalies[series
-0001c510: 5d0d 0a20 2020 2020 2020 2069 5f61 6e6f  ]..        i_ano
-0001c520: 6d20 3d20 7365 7269 6573 5f61 6e6f 6d5b  m = series_anom[
-0001c530: 7365 7269 6573 5f61 6e6f 6d20 3d3d 202d  series_anom == -
-0001c540: 315d 2e69 6e64 6578 0d0a 2020 2020 6966  1].index..    if
-0001c550: 2073 7461 7274 5f64 6174 6520 6973 206e   start_date is n
-0001c560: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0001c570: 2020 695f 616e 6f6d 203d 2069 5f61 6e6f    i_anom = i_ano
-0001c580: 6d5b 695f 616e 6f6d 203e 3d20 7374 6172  m[i_anom >= star
-0001c590: 745f 6461 7465 5d0d 0a20 2020 2069 6620  t_date]..    if 
-0001c5a0: 6c65 6e28 695f 616e 6f6d 2920 3e20 3020  len(i_anom) > 0 
-0001c5b0: 616e 6420 6c65 6e28 695f 616e 6f6d 2920  and len(i_anom) 
-0001c5c0: 3c20 6c65 6e28 6466 5f64 6169 6c79 2920  < len(df_daily) 
-0001c5d0: 2a20 302e 353a 0d0a 2020 2020 2020 2020  * 0.5:..        
-0001c5e0: 7363 6174 3320 3d20 6178 2e73 6361 7474  scat3 = ax.scatt
-0001c5f0: 6572 2869 5f61 6e6f 6d2e 746f 6c69 7374  er(i_anom.tolist
-0001c600: 2829 2c20 6466 5f64 6169 6c79 2e6c 6f63  (), df_daily.loc
-0001c610: 5b69 5f61 6e6f 6d5d 5b73 6572 6965 735d  [i_anom][series]
-0001c620: 2c20 633d 2273 6c61 7465 6772 6179 222c  , c="slategray",
-0001c630: 2073 3d31 322e 3029 0d0a 2020 2020 2020   s=12.0)..      
-0001c640: 2020 6861 6e64 6c65 7320 2b3d 205b 7363    handles += [sc
-0001c650: 6174 335d 0d0a 2020 2020 2020 2020 6c61  at3]..        la
-0001c660: 6265 6c73 202b 3d20 5b22 7472 656e 6420  bels += ["trend 
-0001c670: 616e 6f6d 616c 6965 7322 5d0d 0a61 782e  anomalies"]..ax.
-0001c680: 6c65 6765 6e64 2868 616e 646c 6573 2c20  legend(handles, 
-0001c690: 6c61 6265 6c73 290d 0a22 2222 0d0a       labels).."""..
+00011240: 2020 7365 6c66 2e63 7265 6174 655f 666f    self.create_fo
+00011250: 7265 6361 7374 5f69 6e64 6578 2831 2c20  recast_index(1, 
+00011260: 6c61 7374 5f64 6174 653d 6466 2e69 6e64  last_date=df.ind
+00011270: 6578 5b2d 315d 290d 0a20 2020 2020 2020  ex[-1])..       
+00011280: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00011290: 2020 2020 2020 2020 2020 2020 6466 5f66              df_f
+000112a0: 6f72 6563 6173 7420 3d20 7365 6c66 2e5f  orecast = self._
+000112b0: 7072 6564 6963 745f 7374 6570 280d 0a20  predict_step(.. 
+000112c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112d0: 2020 2064 6174 6573 3d66 6f72 6563 6173     dates=forecas
+000112e0: 745f 696e 6465 782c 0d0a 2020 2020 2020  t_index,..      
+000112f0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00011300: 656e 645f 636f 6d70 6f6e 656e 743d 7472  end_component=tr
+00011310: 656e 645f 666f 7265 6361 7374 2c0d 0a20  end_forecast,.. 
+00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011330: 2020 2068 6973 746f 7279 5f64 663d 6466     history_df=df
+00011340: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00011350: 2020 2020 2020 2066 7574 7572 655f 7265         future_re
+00011360: 6772 6573 736f 723d 7365 6c66 2e66 756c  gressor=self.ful
+00011370: 6c5f 7265 6772 2c0d 0a20 2020 2020 2020  l_regr,..       
+00011380: 2020 2020 2020 2020 2020 2020 2066 6c61               fla
+00011390: 675f 7265 6772 6573 736f 7273 3d73 656c  g_regressors=sel
+000113a0: 662e 616c 6c5f 666c 6167 732c 0d0a 2020  f.all_flags,..  
+000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113c0: 2020 696d 7061 6374 733d 7365 6c66 2e75    impacts=self.u
+000113d0: 7365 5f69 6d70 6163 7473 2c0d 0a20 2020  se_impacts,..   
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 2072 6567 7265 7373 6f72 5f70 6572 5f73   regressor_per_s
+00011400: 6572 6965 733d 7365 6c66 2e72 6567 725f  eries=self.regr_
+00011410: 7073 5f66 6f72 652c 0d0a 2020 2020 2020  ps_fore,..      
+00011420: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00011430: 2020 2020 2020 2020 2020 2020 2064 6620               df 
+00011440: 3d20 7064 2e63 6f6e 6361 7428 5b64 662c  = pd.concat([df,
+00011450: 2064 665f 666f 7265 6361 7374 2e66 6f72   df_forecast.for
+00011460: 6563 6173 742e 696c 6f63 5b2d 313a 5d5d  ecast.iloc[-1:]]
+00011470: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00011480: 6620 6e6f 7420 696e 636c 7564 655f 6869  f not include_hi
+00011490: 7374 6f72 793a 0d0a 2020 2020 2020 2020  story:..        
+000114a0: 2020 2020 2020 2020 6466 5f66 6f72 6563          df_forec
+000114b0: 6173 742e 666f 7265 6361 7374 203d 2064  ast.forecast = d
+000114c0: 665f 666f 7265 6361 7374 2e66 6f72 6563  f_forecast.forec
+000114d0: 6173 742e 7461 696c 2866 6f72 6563 6173  ast.tail(forecas
+000114e0: 745f 6c65 6e67 7468 290d 0a20 2020 2020  t_length)..     
+000114f0: 2020 2020 2020 2020 2020 2064 665f 666f             df_fo
+00011500: 7265 6361 7374 2e6c 6f77 6572 5f66 6f72  recast.lower_for
+00011510: 6563 6173 7420 3d20 6466 5f66 6f72 6563  ecast = df_forec
+00011520: 6173 742e 6c6f 7765 725f 666f 7265 6361  ast.lower_foreca
+00011530: 7374 2e74 6169 6c28 0d0a 2020 2020 2020  st.tail(..      
+00011540: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00011550: 7265 6361 7374 5f6c 656e 6774 680d 0a20  recast_length.. 
+00011560: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00011570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011580: 2020 6466 5f66 6f72 6563 6173 742e 7570    df_forecast.up
+00011590: 7065 725f 666f 7265 6361 7374 203d 2064  per_forecast = d
+000115a0: 665f 666f 7265 6361 7374 2e75 7070 6572  f_forecast.upper
+000115b0: 5f66 6f72 6563 6173 742e 7461 696c 280d  _forecast.tail(.
+000115c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000115d0: 2020 2020 2066 6f72 6563 6173 745f 6c65       forecast_le
+000115e0: 6e67 7468 0d0a 2020 2020 2020 2020 2020  ngth..          
+000115f0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00011600: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00011610: 2020 2020 666f 7265 6361 7374 5f69 6e64      forecast_ind
+00011620: 6578 203d 2073 656c 662e 6372 6561 7465  ex = self.create
+00011630: 5f66 6f72 6563 6173 745f 696e 6465 7828  _forecast_index(
+00011640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011650: 2020 666f 7265 6361 7374 5f6c 656e 6774    forecast_lengt
+00011660: 682c 206c 6173 745f 6461 7465 3d64 662e  h, last_date=df.
+00011670: 696e 6465 785b 2d31 5d0d 0a20 2020 2020  index[-1]..     
+00011680: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00011690: 2020 2020 2020 6966 2069 6e63 6c75 6465        if include
+000116a0: 5f68 6973 746f 7279 3a0d 0a20 2020 2020  _history:..     
+000116b0: 2020 2020 2020 2020 2020 2066 6f72 6563             forec
+000116c0: 6173 745f 696e 6465 7820 3d20 6466 2e69  ast_index = df.i
+000116d0: 6e64 6578 2e75 6e69 6f6e 2866 6f72 6563  ndex.union(forec
+000116e0: 6173 745f 696e 6465 7829 0d0a 2020 2020  ast_index)..    
+000116f0: 2020 2020 2020 2020 6466 5f66 6f72 6563          df_forec
+00011700: 6173 7420 3d20 7365 6c66 2e5f 7072 6564  ast = self._pred
+00011710: 6963 745f 7374 6570 280d 0a20 2020 2020  ict_step(..     
+00011720: 2020 2020 2020 2020 2020 2064 6174 6573             dates
+00011730: 3d66 6f72 6563 6173 745f 696e 6465 782c  =forecast_index,
+00011740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011750: 2020 7472 656e 645f 636f 6d70 6f6e 656e    trend_componen
+00011760: 743d 7472 656e 645f 666f 7265 6361 7374  t=trend_forecast
+00011770: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00011780: 2020 2068 6973 746f 7279 5f64 663d 6466     history_df=df
+00011790: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000117a0: 2020 2066 7574 7572 655f 7265 6772 6573     future_regres
+000117b0: 736f 723d 7365 6c66 2e66 756c 6c5f 7265  sor=self.full_re
+000117c0: 6772 2c0d 0a20 2020 2020 2020 2020 2020  gr,..           
+000117d0: 2020 2020 2066 6c61 675f 7265 6772 6573       flag_regres
+000117e0: 736f 7273 3d73 656c 662e 616c 6c5f 666c  sors=self.all_fl
+000117f0: 6167 732c 0d0a 2020 2020 2020 2020 2020  ags,..          
+00011800: 2020 2020 2020 696d 7061 6374 733d 7365        impacts=se
+00011810: 6c66 2e75 7365 5f69 6d70 6163 7473 2c0d  lf.use_impacts,.
+00011820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011830: 2072 6567 7265 7373 6f72 5f70 6572 5f73   regressor_per_s
+00011840: 6572 6965 733d 7365 6c66 2e72 6567 725f  eries=self.regr_
+00011850: 7073 5f66 6f72 652c 0d0a 2020 2020 2020  ps_fore,..      
+00011860: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+00011870: 2020 2023 2073 6176 6520 6675 7475 7265     # save future
+00011880: 2069 6e64 6578 2062 6566 6f72 6520 696e   index before in
+00011890: 636c 7564 655f 6869 7374 6f72 7920 6973  clude_history is
+000118a0: 2061 6464 6564 0d0a 2020 2020 2020 2020   added..        
+000118b0: 6966 2066 7574 7572 655f 696d 7061 6374  if future_impact
+000118c0: 7320 6973 206e 6f74 204e 6f6e 6520 616e  s is not None an
+000118d0: 6420 666f 7265 6361 7374 5f6c 656e 6774  d forecast_lengt
+000118e0: 6820 6973 206e 6f74 204e 6f6e 653a 0d0a  h is not None:..
+000118f0: 2020 2020 2020 2020 2020 2020 6675 7475              futu
+00011900: 7265 5f69 6d70 6163 7473 203d 2066 7574  re_impacts = fut
+00011910: 7572 655f 696d 7061 6374 732e 7265 696e  ure_impacts.rein
+00011920: 6465 7828 0d0a 2020 2020 2020 2020 2020  dex(..          
+00011930: 2020 2020 2020 636f 6c75 6d6e 733d 6466        columns=df
+00011940: 5f66 6f72 6563 6173 742e 666f 7265 6361  _forecast.foreca
+00011950: 7374 2e63 6f6c 756d 6e73 2c0d 0a20 2020  st.columns,..   
+00011960: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+00011970: 6578 3d66 6f72 6563 6173 745f 696e 6465  ex=forecast_inde
+00011980: 782c 0d0a 2020 2020 2020 2020 2020 2020  x,..            
+00011990: 2020 2020 6669 6c6c 5f76 616c 7565 3d30      fill_value=0
+000119a0: 2c0d 0a20 2020 2020 2020 2020 2020 2029  ,..            )
+000119b0: 0d0a 2020 2020 2020 2020 2320 756e 646f  ..        # undo
+000119c0: 2070 7265 7072 6f63 6573 7369 6e67 2061   preprocessing a
+000119d0: 6e64 2073 6361 6c69 6e67 0d0a 2020 2020  nd scaling..    
+000119e0: 2020 2020 2320 6163 636f 756e 7420 666f      # account fo
+000119f0: 7220 736f 6d65 2074 7261 6e73 666f 726d  r some transform
+00011a00: 6572 7320 7265 7175 6972 696e 6720 6469  ers requiring di
+00011a10: 6666 6572 656e 7420 6d65 7468 6f64 7320  fferent methods 
+00011a20: 6f6e 206f 7269 6769 6e61 6c20 6461 7461  on original data
+00011a30: 2061 6e64 2066 6f72 6563 6173 740d 0a20   and forecast.. 
+00011a40: 2020 2020 2020 2069 6620 666f 7265 6361         if foreca
+00011a50: 7374 5f6c 656e 6774 6820 6973 204e 6f6e  st_length is Non
+00011a60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00011a70: 6466 5f66 6f72 6563 6173 742e 666f 7265  df_forecast.fore
+00011a80: 6361 7374 203d 2073 656c 662e 746f 5f6f  cast = self.to_o
+00011a90: 7269 6769 6e5f 7370 6163 6528 0d0a 2020  rigin_space(..  
+00011aa0: 2020 2020 2020 2020 2020 2020 2020 6466                df
+00011ab0: 5f66 6f72 6563 6173 742e 666f 7265 6361  _forecast.foreca
+00011ac0: 7374 2c20 7472 616e 735f 6d65 7468 6f64  st, trans_method
+00011ad0: 3d27 6f72 6967 696e 616c 270d 0a20 2020  ='original'..   
+00011ae0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+00011af0: 2020 2020 2020 2020 6466 5f66 6f72 6563          df_forec
+00011b00: 6173 742e 6c6f 7765 725f 666f 7265 6361  ast.lower_foreca
+00011b10: 7374 203d 2073 656c 662e 746f 5f6f 7269  st = self.to_ori
+00011b20: 6769 6e5f 7370 6163 6528 0d0a 2020 2020  gin_space(..    
+00011b30: 2020 2020 2020 2020 2020 2020 6466 5f66              df_f
+00011b40: 6f72 6563 6173 742e 6c6f 7765 725f 666f  orecast.lower_fo
+00011b50: 7265 6361 7374 2c20 7472 616e 735f 6d65  recast, trans_me
+00011b60: 7468 6f64 3d27 6f72 6967 696e 616c 270d  thod='original'.
+00011b70: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00011b80: 2020 2020 2020 2020 2020 2020 6466 5f66              df_f
+00011b90: 6f72 6563 6173 742e 7570 7065 725f 666f  orecast.upper_fo
+00011ba0: 7265 6361 7374 203d 2073 656c 662e 746f  recast = self.to
+00011bb0: 5f6f 7269 6769 6e5f 7370 6163 6528 0d0a  _origin_space(..
+00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bd0: 6466 5f66 6f72 6563 6173 742e 7570 7065  df_forecast.uppe
+00011be0: 725f 666f 7265 6361 7374 2c20 7472 616e  r_forecast, tran
+00011bf0: 735f 6d65 7468 6f64 3d27 6f72 6967 696e  s_method='origin
+00011c00: 616c 270d 0a20 2020 2020 2020 2020 2020  al'..           
+00011c10: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00011c20: 7365 6c66 2e70 7265 6469 6374 6564 5f74  self.predicted_t
+00011c30: 7265 6e64 203d 2073 656c 662e 746f 5f6f  rend = self.to_o
+00011c40: 7269 6769 6e5f 7370 6163 6528 0d0a 2020  rigin_space(..  
+00011c50: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00011c60: 656e 645f 666f 7265 6361 7374 2e66 6f72  end_forecast.for
+00011c70: 6563 6173 742c 2074 7261 6e73 5f6d 6574  ecast, trans_met
+00011c80: 686f 643d 276f 7269 6769 6e61 6c27 0d0a  hod='original'..
+00011c90: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00011ca0: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
+00011cb0: 696e 636c 7564 655f 6869 7374 6f72 793a  include_history:
+00011cc0: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+00011cd0: 5f66 6f72 6563 6173 742e 666f 7265 6361  _forecast.foreca
+00011ce0: 7374 203d 2073 656c 662e 746f 5f6f 7269  st = self.to_ori
+00011cf0: 6769 6e5f 7370 6163 6528 0d0a 2020 2020  gin_space(..    
+00011d00: 2020 2020 2020 2020 2020 2020 6466 5f66              df_f
+00011d10: 6f72 6563 6173 742e 666f 7265 6361 7374  orecast.forecast
+00011d20: 2c20 7472 616e 735f 6d65 7468 6f64 3d27  , trans_method='
+00011d30: 666f 7265 6361 7374 270d 0a20 2020 2020  forecast'..     
+00011d40: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00011d50: 2020 2020 2020 6466 5f66 6f72 6563 6173        df_forecas
+00011d60: 742e 6c6f 7765 725f 666f 7265 6361 7374  t.lower_forecast
+00011d70: 203d 2073 656c 662e 746f 5f6f 7269 6769   = self.to_origi
+00011d80: 6e5f 7370 6163 6528 0d0a 2020 2020 2020  n_space(..      
+00011d90: 2020 2020 2020 2020 2020 6466 5f66 6f72            df_for
+00011da0: 6563 6173 742e 6c6f 7765 725f 666f 7265  ecast.lower_fore
+00011db0: 6361 7374 2c20 7472 616e 735f 6d65 7468  cast, trans_meth
+00011dc0: 6f64 3d27 666f 7265 6361 7374 270d 0a20  od='forecast'.. 
+00011dd0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00011de0: 2020 2020 2020 2020 2020 6466 5f66 6f72            df_for
+00011df0: 6563 6173 742e 7570 7065 725f 666f 7265  ecast.upper_fore
+00011e00: 6361 7374 203d 2073 656c 662e 746f 5f6f  cast = self.to_o
+00011e10: 7269 6769 6e5f 7370 6163 6528 0d0a 2020  rigin_space(..  
+00011e20: 2020 2020 2020 2020 2020 2020 2020 6466                df
+00011e30: 5f66 6f72 6563 6173 742e 7570 7065 725f  _forecast.upper_
+00011e40: 666f 7265 6361 7374 2c20 7472 616e 735f  forecast, trans_
+00011e50: 6d65 7468 6f64 3d27 666f 7265 6361 7374  method='forecast
+00011e60: 270d 0a20 2020 2020 2020 2020 2020 2029  '..            )
+00011e70: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00011e80: 6c66 2e70 7265 6469 6374 6564 5f74 7265  lf.predicted_tre
+00011e90: 6e64 203d 2073 656c 662e 746f 5f6f 7269  nd = self.to_ori
+00011ea0: 6769 6e5f 7370 6163 6528 0d0a 2020 2020  gin_space(..    
+00011eb0: 2020 2020 2020 2020 2020 2020 7472 656e              tren
+00011ec0: 645f 666f 7265 6361 7374 2e66 6f72 6563  d_forecast.forec
+00011ed0: 6173 742c 2074 7261 6e73 5f6d 6574 686f  ast, trans_metho
+00011ee0: 643d 2766 6f72 6563 6173 7427 0d0a 2020  d='forecast'..  
+00011ef0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00011f00: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00011f10: 2020 2020 2020 2020 6864 6e20 3d20 6c65          hdn = le
+00011f20: 6e28 6466 5f66 6f72 6563 6173 742e 666f  n(df_forecast.fo
+00011f30: 7265 6361 7374 2920 2d20 666f 7265 6361  recast) - foreca
+00011f40: 7374 5f6c 656e 6774 680d 0a20 2020 2020  st_length..     
+00011f50: 2020 2020 2020 2064 665f 666f 7265 6361         df_foreca
+00011f60: 7374 2e66 6f72 6563 6173 7420 3d20 7064  st.forecast = pd
+00011f70: 2e63 6f6e 6361 7428 0d0a 2020 2020 2020  .concat(..      
+00011f80: 2020 2020 2020 2020 2020 5b0d 0a20 2020            [..   
+00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fa0: 2073 656c 662e 746f 5f6f 7269 6769 6e5f   self.to_origin_
+00011fb0: 7370 6163 6528 0d0a 2020 2020 2020 2020  space(..        
+00011fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fd0: 6466 5f66 6f72 6563 6173 742e 666f 7265  df_forecast.fore
+00011fe0: 6361 7374 2e68 6561 6428 6864 6e29 2c20  cast.head(hdn), 
+00011ff0: 7472 616e 735f 6d65 7468 6f64 3d27 6f72  trans_method='or
+00012000: 6967 696e 616c 270d 0a20 2020 2020 2020  iginal'..       
+00012010: 2020 2020 2020 2020 2020 2020 2029 2c0d               ),.
+00012020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012030: 2020 2020 2073 656c 662e 746f 5f6f 7269       self.to_ori
+00012040: 6769 6e5f 7370 6163 6528 0d0a 2020 2020  gin_space(..    
+00012050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012060: 2020 2020 6466 5f66 6f72 6563 6173 742e      df_forecast.
+00012070: 666f 7265 6361 7374 2e74 6169 6c28 666f  forecast.tail(fo
+00012080: 7265 6361 7374 5f6c 656e 6774 6829 2c0d  recast_length),.
+00012090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000120a0: 2020 2020 2020 2020 2074 7261 6e73 5f6d           trans_m
+000120b0: 6574 686f 643d 2766 6f72 6563 6173 7427  ethod='forecast'
+000120c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000120d0: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
+000120e0: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
+000120f0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00012100: 2020 2020 2020 2020 2064 665f 666f 7265           df_fore
+00012110: 6361 7374 2e6c 6f77 6572 5f66 6f72 6563  cast.lower_forec
+00012120: 6173 7420 3d20 7064 2e63 6f6e 6361 7428  ast = pd.concat(
+00012130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012140: 2020 5b0d 0a20 2020 2020 2020 2020 2020    [..           
+00012150: 2020 2020 2020 2020 2073 656c 662e 746f           self.to
+00012160: 5f6f 7269 6769 6e5f 7370 6163 6528 0d0a  _origin_space(..
+00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012180: 2020 2020 2020 2020 6466 5f66 6f72 6563          df_forec
+00012190: 6173 742e 6c6f 7765 725f 666f 7265 6361  ast.lower_foreca
+000121a0: 7374 2e68 6561 6428 6864 6e29 2c0d 0a20  st.head(hdn),.. 
+000121b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121c0: 2020 2020 2020 2074 7261 6e73 5f6d 6574         trans_met
+000121d0: 686f 643d 276f 7269 6769 6e61 6c27 2c0d  hod='original',.
+000121e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000121f0: 2020 2020 2020 2020 2062 6f75 6e64 733d           bounds=
+00012200: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00012210: 2020 2020 2020 2020 2020 2029 2c0d 0a20             ),.. 
+00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012230: 2020 2073 656c 662e 746f 5f6f 7269 6769     self.to_origi
+00012240: 6e5f 7370 6163 6528 0d0a 2020 2020 2020  n_space(..      
+00012250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012260: 2020 6466 5f66 6f72 6563 6173 742e 6c6f    df_forecast.lo
+00012270: 7765 725f 666f 7265 6361 7374 2e74 6169  wer_forecast.tai
+00012280: 6c28 666f 7265 6361 7374 5f6c 656e 6774  l(forecast_lengt
+00012290: 6829 2c0d 0a20 2020 2020 2020 2020 2020  h),..           
+000122a0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+000122b0: 6e73 5f6d 6574 686f 643d 2766 6f72 6563  ns_method='forec
+000122c0: 6173 7427 2c0d 0a20 2020 2020 2020 2020  ast',..         
+000122d0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+000122e0: 6f75 6e64 733d 5472 7565 2c0d 0a20 2020  ounds=True,..   
+000122f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012300: 2029 2c0d 0a20 2020 2020 2020 2020 2020   ),..           
+00012310: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
+00012320: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00012330: 2020 2064 665f 666f 7265 6361 7374 2e75     df_forecast.u
+00012340: 7070 6572 5f66 6f72 6563 6173 7420 3d20  pper_forecast = 
+00012350: 7064 2e63 6f6e 6361 7428 0d0a 2020 2020  pd.concat(..    
+00012360: 2020 2020 2020 2020 2020 2020 5b0d 0a20              [.. 
+00012370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012380: 2020 2073 656c 662e 746f 5f6f 7269 6769     self.to_origi
+00012390: 6e5f 7370 6163 6528 0d0a 2020 2020 2020  n_space(..      
+000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123b0: 2020 6466 5f66 6f72 6563 6173 742e 7570    df_forecast.up
+000123c0: 7065 725f 666f 7265 6361 7374 2e68 6561  per_forecast.hea
+000123d0: 6428 6864 6e29 2c0d 0a20 2020 2020 2020  d(hdn),..       
+000123e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123f0: 2074 7261 6e73 5f6d 6574 686f 643d 276f   trans_method='o
+00012400: 7269 6769 6e61 6c27 2c0d 0a20 2020 2020  riginal',..     
+00012410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012420: 2020 2062 6f75 6e64 733d 5472 7565 2c0d     bounds=True,.
+00012430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012440: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
+00012450: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012460: 662e 746f 5f6f 7269 6769 6e5f 7370 6163  f.to_origin_spac
+00012470: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
+00012480: 2020 2020 2020 2020 2020 2020 6466 5f66              df_f
+00012490: 6f72 6563 6173 742e 7570 7065 725f 666f  orecast.upper_fo
+000124a0: 7265 6361 7374 2e74 6169 6c28 666f 7265  recast.tail(fore
+000124b0: 6361 7374 5f6c 656e 6774 6829 2c0d 0a20  cast_length),.. 
+000124c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124d0: 2020 2020 2020 2074 7261 6e73 5f6d 6574         trans_met
+000124e0: 686f 643d 2766 6f72 6563 6173 7427 2c0d  hod='forecast',.
+000124f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012500: 2020 2020 2020 2020 2062 6f75 6e64 733d           bounds=
+00012510: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+00012520: 2020 2020 2020 2020 2020 2029 2c0d 0a20             ),.. 
+00012530: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00012540: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+00012550: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00012560: 662e 7072 6564 6963 7465 645f 7472 656e  f.predicted_tren
+00012570: 6420 3d20 7064 2e63 6f6e 6361 7428 0d0a  d = pd.concat(..
+00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012590: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+000125a0: 2020 2020 2020 2073 656c 662e 746f 5f6f         self.to_o
+000125b0: 7269 6769 6e5f 7370 6163 6528 0d0a 2020  rigin_space(..  
+000125c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125d0: 2020 2020 2020 7472 656e 645f 666f 7265        trend_fore
+000125e0: 6361 7374 2e66 6f72 6563 6173 742e 6865  cast.forecast.he
+000125f0: 6164 2868 646e 292c 2074 7261 6e73 5f6d  ad(hdn), trans_m
+00012600: 6574 686f 643d 276f 7269 6769 6e61 6c27  ethod='original'
+00012610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012620: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
+00012630: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012640: 6c66 2e74 6f5f 6f72 6967 696e 5f73 7061  lf.to_origin_spa
+00012650: 6365 280d 0a20 2020 2020 2020 2020 2020  ce(..           
+00012660: 2020 2020 2020 2020 2020 2020 2074 7265               tre
+00012670: 6e64 5f66 6f72 6563 6173 742e 666f 7265  nd_forecast.fore
+00012680: 6361 7374 2e74 6169 6c28 666f 7265 6361  cast.tail(foreca
+00012690: 7374 5f6c 656e 6774 6829 2c0d 0a20 2020  st_length),..   
+000126a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126b0: 2020 2020 2074 7261 6e73 5f6d 6574 686f       trans_metho
+000126c0: 643d 2766 6f72 6563 6173 7427 2c0d 0a20  d='forecast',.. 
+000126d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126e0: 2020 2029 2c0d 0a20 2020 2020 2020 2020     ),..         
+000126f0: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+00012700: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+00012710: 2020 2023 2075 7064 6174 6520 7472 656e     # update tren
+00012720: 6420 616e 616c 7973 6973 2062 6173 6564  d analysis based
+00012730: 206f 6e20 7472 656e 6420 666f 7265 6361   on trend foreca
+00012740: 7374 2061 7320 7765 6c6c 0d0a 2020 2020  st as well..    
+00012750: 2020 2020 6966 2066 6f72 6563 6173 745f      if forecast_
+00012760: 6c65 6e67 7468 2069 7320 6e6f 7420 4e6f  length is not No
+00012770: 6e65 2061 6e64 2069 6e63 6c75 6465 5f68  ne and include_h
+00012780: 6973 746f 7279 3a0d 0a20 2020 2020 2020  istory:..       
+00012790: 2020 2020 2074 7265 6e64 5f70 6f73 7465       trend_poste
+000127a0: 7269 6f72 2c20 7365 6c66 2e73 6c6f 7065  rior, self.slope
+000127b0: 2c20 696e 7465 7263 6570 7420 3d20 7365  , intercept = se
+000127c0: 6c66 2e72 6f6c 6c69 6e67 5f74 7265 6e64  lf.rolling_trend
+000127d0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+000127e0: 2020 2073 656c 662e 7072 6564 6963 7465     self.predicte
+000127f0: 645f 7472 656e 642c 206e 702e 6172 7261  d_trend, np.arra
+00012800: 7928 7365 6c66 2e74 5f70 7265 6469 6374  y(self.t_predict
+00012810: 290d 0a20 2020 2020 2020 2020 2020 2029  )..            )
+00012820: 0d0a 2020 2020 2020 2020 2020 2020 280d  ..            (.
+00012830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012840: 2073 656c 662e 7a65 726f 5f63 726f 7373   self.zero_cross
+00012850: 696e 6773 2c0d 0a20 2020 2020 2020 2020  ings,..         
+00012860: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+00012870: 6765 706f 696e 7473 2c0d 0a20 2020 2020  gepoints,..     
+00012880: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012890: 736c 6f70 655f 7369 676e 2c0d 0a20 2020  slope_sign,..   
+000128a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000128b0: 662e 6163 6365 6c2c 0d0a 2020 2020 2020  f.accel,..      
+000128c0: 2020 2020 2020 2920 3d20 7365 6c66 2e61        ) = self.a
+000128d0: 6e61 6c79 7a65 5f74 7265 6e64 2873 656c  nalyze_trend(sel
+000128e0: 662e 736c 6f70 652c 2069 6e64 6578 3d73  f.slope, index=s
+000128f0: 656c 662e 7072 6564 6963 7465 645f 7472  elf.predicted_tr
+00012900: 656e 642e 696e 6465 7829 0d0a 0d0a 2020  end.index)....  
+00012910: 2020 2020 2020 2320 646f 6e27 7420 666f        # don't fo
+00012920: 7267 6574 2074 6f20 6164 6420 696e 2070  rget to add in p
+00012930: 6173 745f 696d 7061 6374 7320 2875 7365  ast_impacts (use
+00012940: 2066 7574 7572 6520 696d 7061 6374 7320   future impacts 
+00012950: 6167 6169 6e3f 2920 4146 5445 5220 756e  again?) AFTER un
+00012960: 7363 616c 696e 670d 0a20 2020 2020 2020  scaling..       
+00012970: 2069 6620 7365 6c66 2e70 6173 745f 696d   if self.past_im
+00012980: 7061 6374 735f 696e 7465 7276 656e 7469  pacts_interventi
+00012990: 6f6e 2021 3d20 2272 6567 7265 7373 6f72  on != "regressor
+000129a0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+000129b0: 6966 2066 7574 7572 655f 696d 7061 6374  if future_impact
+000129c0: 7320 6973 206e 6f74 204e 6f6e 6520 616e  s is not None an
+000129d0: 6420 7365 6c66 2e70 6173 745f 696d 7061  d self.past_impa
+000129e0: 6374 7320 6973 204e 6f6e 653a 0d0a 2020  cts is None:..  
+000129f0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00012a00: 7374 5f69 6d70 6163 7473 203d 2070 642e  st_impacts = pd.
+00012a10: 4461 7461 4672 616d 6528 0d0a 2020 2020  DataFrame(..    
+00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a30: 302c 2069 6e64 6578 3d73 656c 662e 6466  0, index=self.df
+00012a40: 2e69 6e64 6578 2c20 636f 6c75 6d6e 733d  .index, columns=
+00012a50: 7365 6c66 2e64 662e 636f 6c75 6d6e 730d  self.df.columns.
+00012a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a70: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00012a80: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00012a90: 2020 2020 2020 2070 6173 745f 696d 7061         past_impa
+00012aa0: 6374 7320 3d20 7365 6c66 2e70 6173 745f  cts = self.past_
+00012ab0: 696d 7061 6374 730d 0a20 2020 2020 2020  impacts..       
+00012ac0: 2020 2020 2023 2072 6f6c 6c20 666f 7277       # roll forw
+00012ad0: 6172 6420 7461 696c 206f 6620 7061 7374  ard tail of past
+00012ae0: 2069 6d70 6163 7473 2c20 6173 7375 6d69   impacts, assumi
+00012af0: 6e67 2069 7420 636f 6e74 696e 7565 730d  ng it continues.
+00012b00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00012b10: 7365 6c66 2e70 6173 745f 696d 7061 6374  self.past_impact
+00012b20: 7320 6973 206e 6f74 204e 6f6e 6520 616e  s is not None an
+00012b30: 6420 666f 7265 6361 7374 5f6c 656e 6774  d forecast_lengt
+00012b40: 6820 6973 206e 6f74 204e 6f6e 653a 0d0a  h is not None:..
+00012b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b60: 6675 7475 7265 5f69 6d70 7473 203d 2070  future_impts = p
+00012b70: 642e 4461 7461 4672 616d 6528 0d0a 2020  d.DataFrame(..  
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b90: 2020 6e70 2e72 6570 6561 7428 0d0a 2020    np.repeat(..  
+00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bb0: 2020 2020 2020 7365 6c66 2e70 6173 745f        self.past_
+00012bc0: 696d 7061 6374 732e 696c 6f63 5b2d 313a  impacts.iloc[-1:
+00012bd0: 5d2e 746f 5f6e 756d 7079 2829 2c20 666f  ].to_numpy(), fo
+00012be0: 7265 6361 7374 5f6c 656e 6774 682c 2061  recast_length, a
+00012bf0: 7869 733d 300d 0a20 2020 2020 2020 2020  xis=0..         
+00012c00: 2020 2020 2020 2020 2020 2029 2c0d 0a20             ),.. 
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c20: 2020 2069 6e64 6578 3d64 665f 666f 7265     index=df_fore
+00012c30: 6361 7374 2e66 6f72 6563 6173 742e 696e  cast.forecast.in
+00012c40: 6465 785b 2d66 6f72 6563 6173 745f 6c65  dex[-forecast_le
+00012c50: 6e67 7468 3a5d 2c0d 0a20 2020 2020 2020  ngth:],..       
+00012c60: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+00012c70: 756d 6e73 3d73 656c 662e 7061 7374 5f69  umns=self.past_i
+00012c80: 6d70 6163 7473 2e63 6f6c 756d 6e73 2c0d  mpacts.columns,.
+00012c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ca0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00012cb0: 2020 2020 6966 2066 7574 7572 655f 696d      if future_im
+00012cc0: 7061 6374 7320 6973 206e 6f74 204e 6f6e  pacts is not Non
+00012cd0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00012ce0: 2020 2020 2020 2020 6675 7475 7265 5f69          future_i
+00012cf0: 6d70 7473 203d 2066 7574 7572 655f 696d  mpts = future_im
+00012d00: 7074 7320 2b20 6675 7475 7265 5f69 6d70  pts + future_imp
+00012d10: 6163 7473 0d0a 2020 2020 2020 2020 2020  acts..          
+00012d20: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00012d30: 2020 2020 2020 2020 2066 7574 7572 655f           future_
+00012d40: 696d 7074 7320 3d20 7064 2e44 6174 6146  impts = pd.DataF
+00012d50: 7261 6d65 2829 0d0a 2020 2020 2020 2020  rame()..        
+00012d60: 2020 2020 6966 2073 656c 662e 7061 7374      if self.past
+00012d70: 5f69 6d70 6163 7473 2069 7320 6e6f 7420  _impacts is not 
+00012d80: 4e6f 6e65 206f 7220 6675 7475 7265 5f69  None or future_i
+00012d90: 6d70 6163 7473 2069 7320 6e6f 7420 4e6f  mpacts is not No
+00012da0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00012db0: 2020 2020 2069 6d70 7473 203d 2031 202b       impts = 1 +
+00012dc0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00012dd0: 2020 2020 2020 2020 7064 2e63 6f6e 6361          pd.conca
+00012de0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00012df0: 2020 2020 2020 2020 2020 2020 5b0d 0a20              [.. 
+00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e10: 2020 2020 2020 2020 2020 2070 6173 745f             past_
+00012e20: 696d 7061 6374 732c 0d0a 2020 2020 2020  impacts,..      
+00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e40: 2020 2020 2020 6675 7475 7265 5f69 6d70        future_imp
+00012e50: 7473 5b7e 6675 7475 7265 5f69 6d70 7473  ts[~future_impts
+00012e60: 2e69 6e64 6578 2e69 7369 6e28 7061 7374  .index.isin(past
+00012e70: 5f69 6d70 6163 7473 2e69 6e64 6578 295d  _impacts.index)]
+00012e80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00012e90: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012eb0: 2020 2020 2020 2061 7869 733d 302c 0d0a         axis=0,..
+00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ed0: 2020 2020 292e 7265 696e 6465 7828 0d0a      ).reindex(..
+00012ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ef0: 2020 2020 2020 2020 696e 6465 783d 6466          index=df
+00012f00: 5f66 6f72 6563 6173 742e 666f 7265 6361  _forecast.foreca
+00012f10: 7374 2e69 6e64 6578 2c0d 0a20 2020 2020  st.index,..     
+00012f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f30: 2020 2063 6f6c 756d 6e73 3d64 665f 666f     columns=df_fo
+00012f40: 7265 6361 7374 2e66 6f72 6563 6173 742e  recast.forecast.
+00012f50: 636f 6c75 6d6e 732c 0d0a 2020 2020 2020  columns,..      
+00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f70: 2020 6669 6c6c 5f76 616c 7565 3d30 2c0d    fill_value=0,.
+00012f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012f90: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00012fa0: 2020 2020 2020 2020 2920 2023 206d 696e          )  # min
+00012fb0: 7573 206f 7220 706c 7573 0d0a 2020 2020  us or plus..    
+00012fc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012fd0: 2e69 6d70 6163 7473 203d 2069 6d70 7473  .impacts = impts
+00012fe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012ff0: 2020 6966 2069 6e63 6c75 6465 5f6f 7267    if include_org
+00013000: 616e 6963 3a0d 0a20 2020 2020 2020 2020  anic:..         
+00013010: 2020 2020 2020 2020 2020 2064 665f 666f             df_fo
+00013020: 7265 6361 7374 2e6f 7267 616e 6963 5f66  recast.organic_f
+00013030: 6f72 6563 6173 7420 3d20 6466 5f66 6f72  orecast = df_for
+00013040: 6563 6173 742e 666f 7265 6361 7374 2e63  ecast.forecast.c
+00013050: 6f70 7928 290d 0a20 2020 2020 2020 2020  opy()..         
+00013060: 2020 2020 2020 2064 665f 666f 7265 6361         df_foreca
+00013070: 7374 2e66 6f72 6563 6173 7420 3d20 6466  st.forecast = df
+00013080: 5f66 6f72 6563 6173 742e 666f 7265 6361  _forecast.foreca
+00013090: 7374 202a 2069 6d70 7473 0d0a 2020 2020  st * impts..    
+000130a0: 2020 2020 2020 2020 2020 2020 6466 5f66              df_f
+000130b0: 6f72 6563 6173 742e 6c6f 7765 725f 666f  orecast.lower_fo
+000130c0: 7265 6361 7374 203d 2064 665f 666f 7265  recast = df_fore
+000130d0: 6361 7374 2e6c 6f77 6572 5f66 6f72 6563  cast.lower_forec
+000130e0: 6173 7420 2a20 696d 7074 730d 0a20 2020  ast * impts..   
+000130f0: 2020 2020 2020 2020 2020 2020 2064 665f               df_
+00013100: 666f 7265 6361 7374 2e75 7070 6572 5f66  forecast.upper_f
+00013110: 6f72 6563 6173 7420 3d20 6466 5f66 6f72  orecast = df_for
+00013120: 6563 6173 742e 7570 7065 725f 666f 7265  ecast.upper_fore
+00013130: 6361 7374 202a 2069 6d70 7473 0d0a 0d0a  cast * impts....
+00013140: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00013150: 636f 6e73 7472 6169 6e74 2069 7320 6e6f  constraint is no
+00013160: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00013170: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00013180: 6365 2873 656c 662e 636f 6e73 7472 6169  ce(self.constrai
+00013190: 6e74 2c20 6469 6374 293a 0d0a 2020 2020  nt, dict):..    
+000131a0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+000131b0: 7472 6169 6e74 5f6d 6574 686f 6420 3d20  traint_method = 
+000131c0: 7365 6c66 2e63 6f6e 7374 7261 696e 742e  self.constraint.
+000131d0: 6765 7428 2263 6f6e 7374 7261 696e 745f  get("constraint_
+000131e0: 6d65 7468 6f64 222c 2022 7175 616e 7469  method", "quanti
+000131f0: 6c65 2229 0d0a 2020 2020 2020 2020 2020  le")..          
+00013200: 2020 2020 2020 636f 6e73 7472 6169 6e74        constraint
+00013210: 5f72 6567 756c 6172 697a 6174 696f 6e20  _regularization 
+00013220: 3d20 7365 6c66 2e63 6f6e 7374 7261 696e  = self.constrain
+00013230: 742e 6765 7428 0d0a 2020 2020 2020 2020  t.get(..        
+00013240: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+00013250: 7374 7261 696e 745f 7265 6775 6c61 7269  straint_regulari
+00013260: 7a61 7469 6f6e 222c 2031 0d0a 2020 2020  zation", 1..    
+00013270: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00013280: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00013290: 6f77 6572 5f63 6f6e 7374 7261 696e 7420  ower_constraint 
+000132a0: 3d20 7365 6c66 2e63 6f6e 7374 7261 696e  = self.constrain
+000132b0: 742e 6765 7428 226c 6f77 6572 5f63 6f6e  t.get("lower_con
+000132c0: 7374 7261 696e 7422 2c20 3029 0d0a 2020  straint", 0)..  
+000132d0: 2020 2020 2020 2020 2020 2020 2020 7570                up
+000132e0: 7065 725f 636f 6e73 7472 6169 6e74 203d  per_constraint =
+000132f0: 2073 656c 662e 636f 6e73 7472 6169 6e74   self.constraint
+00013300: 2e67 6574 2822 7570 7065 725f 636f 6e73  .get("upper_cons
+00013310: 7472 6169 6e74 222c 2031 290d 0a20 2020  traint", 1)..   
+00013320: 2020 2020 2020 2020 2020 2020 2062 6f75               bou
+00013330: 6e64 7320 3d20 7365 6c66 2e63 6f6e 7374  nds = self.const
+00013340: 7261 696e 742e 6765 7428 2262 6f75 6e64  raint.get("bound
+00013350: 7322 2c20 4661 6c73 6529 0d0a 2020 2020  s", False)..    
+00013360: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00013370: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013380: 6f6e 7374 7261 696e 745f 6d65 7468 6f64  onstraint_method
+00013390: 203d 2022 7374 6465 765f 6d69 6e22 0d0a   = "stdev_min"..
+000133a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133b0: 6c6f 7765 725f 636f 6e73 7472 6169 6e74  lower_constraint
+000133c0: 203d 2066 6c6f 6174 2873 656c 662e 636f   = float(self.co
+000133d0: 6e73 7472 6169 6e74 290d 0a20 2020 2020  nstraint)..     
+000133e0: 2020 2020 2020 2020 2020 2075 7070 6572             upper
+000133f0: 5f63 6f6e 7374 7261 696e 7420 3d20 666c  _constraint = fl
+00013400: 6f61 7428 7365 6c66 2e63 6f6e 7374 7261  oat(self.constra
+00013410: 696e 7429 0d0a 2020 2020 2020 2020 2020  int)..          
+00013420: 2020 2020 2020 636f 6e73 7472 6169 6e74        constraint
+00013430: 5f72 6567 756c 6172 697a 6174 696f 6e20  _regularization 
+00013440: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
+00013450: 2020 2020 2062 6f75 6e64 7320 3d20 4661       bounds = Fa
+00013460: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+00013470: 2069 6620 7365 6c66 2e76 6572 626f 7365   if self.verbose
+00013480: 203e 3d20 333a 0d0a 2020 2020 2020 2020   >= 3:..        
+00013490: 2020 2020 2020 2020 7072 696e 7428 0d0a          print(..
+000134a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134b0: 2020 2020 6622 5573 696e 6720 636f 6e73      f"Using cons
+000134c0: 7472 6169 6e74 2077 6974 6820 6d65 7468  traint with meth
+000134d0: 6f64 3a20 7b63 6f6e 7374 7261 696e 745f  od: {constraint_
+000134e0: 6d65 7468 6f64 7d2c 207b 636f 6e73 7472  method}, {constr
+000134f0: 6169 6e74 5f72 6567 756c 6172 697a 6174  aint_regularizat
+00013500: 696f 6e7d 2c20 7b6c 6f77 6572 5f63 6f6e  ion}, {lower_con
+00013510: 7374 7261 696e 747d 2c20 7b75 7070 6572  straint}, {upper
+00013520: 5f63 6f6e 7374 7261 696e 747d 2c20 7b62  _constraint}, {b
+00013530: 6f75 6e64 737d 220d 0a20 2020 2020 2020  ounds}"..       
+00013540: 2020 2020 2020 2020 2029 0d0a 0d0a 2020           )....  
+00013550: 2020 2020 2020 2020 2020 6466 5f66 6f72            df_for
+00013560: 6563 6173 7420 3d20 6466 5f66 6f72 6563  ecast = df_forec
+00013570: 6173 742e 6170 706c 795f 636f 6e73 7472  ast.apply_constr
+00013580: 6169 6e74 7328 0d0a 2020 2020 2020 2020  aints(..        
+00013590: 2020 2020 2020 2020 636f 6e73 7472 6169          constrai
+000135a0: 6e74 5f6d 6574 686f 642c 0d0a 2020 2020  nt_method,..    
+000135b0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+000135c0: 7472 6169 6e74 5f72 6567 756c 6172 697a  traint_regulariz
+000135d0: 6174 696f 6e2c 0d0a 2020 2020 2020 2020  ation,..        
+000135e0: 2020 2020 2020 2020 7570 7065 725f 636f          upper_co
+000135f0: 6e73 7472 6169 6e74 2c0d 0a20 2020 2020  nstraint,..     
+00013600: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
+00013610: 5f63 6f6e 7374 7261 696e 742c 0d0a 2020  _constraint,..  
+00013620: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+00013630: 756e 6473 2c0d 0a20 2020 2020 2020 2020  unds,..         
+00013640: 2020 2020 2020 2073 656c 662e 6466 5f6f         self.df_o
+00013650: 7269 6769 6e61 6c2c 0d0a 2020 2020 2020  riginal,..      
+00013660: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00013670: 2023 2052 4554 5552 4e20 434f 4d50 4f4e   # RETURN COMPON
+00013680: 454e 5453 2028 6c6f 6e67 2073 7479 6c65  ENTS (long style
+00013690: 2920 6f70 7469 6f6e 0d0a 2020 2020 2020  ) option..      
+000136a0: 2020 6466 5f66 6f72 6563 6173 742e 7072    df_forecast.pr
+000136b0: 6564 6963 745f 7275 6e74 696d 6520 3d20  edict_runtime = 
+000136c0: 7365 6c66 2e74 696d 6528 2920 2d20 7072  self.time() - pr
+000136d0: 6564 6963 7453 7461 7274 5469 6d65 0d0a  edictStartTime..
+000136e0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+000136f0: 665f 666f 7265 6361 7374 0d0a 0d0a 2020  f_forecast....  
+00013700: 2020 6465 6620 6175 746f 5f66 6974 2873    def auto_fit(s
+00013710: 656c 662c 2064 662c 2076 616c 6964 6174  elf, df, validat
+00013720: 696f 6e5f 6d65 7468 6f64 293a 2020 2320  ion_method):  # 
+00013730: 616c 736f 2061 6464 2072 6567 7265 7373  also add regress
+00013740: 6f72 2069 6e70 7574 0d0a 2020 2020 2020  or input..      
+00013750: 2020 2320 6f70 7469 6f6e 2074 6f20 636f    # option to co
+00013760: 6d70 6c65 7465 6c79 2073 6b69 7020 736f  mpletely skip so
+00013770: 6d65 2074 6869 6e67 7320 2861 6e6f 6d61  me things (anoma
+00013780: 6c69 6573 2c20 686f 6c69 6461 7920 6465  lies, holiday de
+00013790: 7465 6374 6f72 2c20 6172 206c 6167 7329  tector, ar lags)
+000137a0: 0d0a 2020 2020 2020 2020 2320 7275 6e20  ..        # run 
+000137b0: 6372 6f73 7320 7661 6c69 6461 7469 6f6e  cross validation
+000137c0: 2074 6f20 6368 6f6f 7365 0d0a 2020 2020   to choose..    
+000137d0: 2020 2020 2320 7265 7475 726e 206d 6574      # return met
+000137e0: 7269 6373 206f 6620 6265 7374 206d 6f64  rics of best mod
+000137f0: 656c 2c20 7365 7420 6261 7365 2070 6172  el, set base par
+00013800: 616d 730d 0a20 2020 2020 2020 2073 656c  ams..        sel
+00013810: 662e 7374 6172 7469 6e67 5f70 6172 616d  f.starting_param
+00013820: 7320 3d20 7365 6c66 2e67 6574 5f70 6172  s = self.get_par
+00013830: 616d 7328 290d 0a20 2020 2020 2020 2072  ams()..        r
+00013840: 6574 7572 6e20 4e6f 7449 6d70 6c65 6d65  eturn NotImpleme
+00013850: 6e74 6564 0d0a 0d0a 2020 2020 6465 6620  nted....    def 
+00013860: 6e65 7874 5f66 6974 2873 656c 6629 3a0d  next_fit(self):.
+00013870: 0a20 2020 2020 2020 2023 206f 7074 696f  .        # optio
+00013880: 6e20 746f 2070 7269 6e74 2061 2067 7261  n to print a gra
+00013890: 7068 206f 6620 6561 6368 2077 6869 6c65  ph of each while
+000138a0: 2067 6f69 6e67 2028 7275 6e20 6167 6169   going (run agai
+000138b0: 6e20 756e 7469 6c20 796f 7520 7365 6520  n until you see 
+000138c0: 6f6e 6520 796f 7520 6c69 6b65 290d 0a20  one you like).. 
+000138d0: 2020 2020 2020 2023 2061 7070 656e 6420         # append 
+000138e0: 746f 2061 6e20 696e 7465 726e 616c 2072  to an internal r
+000138f0: 6563 6f72 642c 2070 7269 6e74 206e 6577  ecord, print new
+00013900: 2070 6172 616d 730d 0a20 2020 2020 2020   params..       
+00013910: 2023 2070 6c6f 743a 2033 2073 7461 636b   # plot: 3 stack
+00013920: 6564 2c20 696e 2073 616d 706c 652c 2074  ed, in sample, t
+00013930: 6865 6e20 6561 6368 2076 616c 6964 6174  hen each validat
+00013940: 696f 6e0d 0a20 2020 2020 2020 2023 206d  ion..        # m
+00013950: 6179 6265 2075 7365 2067 656e 6574 6963  aybe use genetic
+00013960: 206f 7074 696d 697a 6174 696f 6e20 6966   optimization if
+00013970: 2074 6869 7320 7573 6564 2061 6674 6572   this used after
+00013980: 2061 7574 6f5f 6669 740d 0a20 2020 2020   auto_fit..     
+00013990: 2020 2072 6574 7572 6e20 4e6f 7449 6d70     return NotImp
+000139a0: 6c65 6d65 6e74 6564 0d0a 0d0a 2020 2020  lemented....    
+000139b0: 6465 6620 6372 6f73 735f 7661 6c69 6461  def cross_valida
+000139c0: 7465 2873 656c 662c 2064 662c 2076 616c  te(self, df, val
+000139d0: 6964 6174 696f 6e5f 6d65 7468 6f64 293a  idation_method):
+000139e0: 0d0a 2020 2020 2020 2020 2320 7275 6e20  ..        # run 
+000139f0: 6f6e 6520 6d6f 6465 6c20 616e 6420 7265  one model and re
+00013a00: 7475 726e 2073 636f 7265 730d 0a20 2020  turn scores..   
+00013a10: 2020 2020 2072 6574 7572 6e20 4e6f 7449       return NotI
+00013a20: 6d70 6c65 6d65 6e74 6564 0d0a 0d0a 2020  mplemented....  
+00013a30: 2020 6465 6620 7472 6561 746d 656e 745f    def treatment_
+00013a40: 6361 7573 616c 5f69 6d70 6163 7428 0d0a  causal_impact(..
+00013a50: 2020 2020 2020 2020 7365 6c66 2c20 6466          self, df
+00013a60: 2c20 696e 7465 7276 656e 7469 6f6e 5f64  , intervention_d
+00013a70: 6174 6573 0d0a 2020 2020 293a 2020 2320  ates..    ):  # 
+00013a80: 616c 736f 2061 6464 2072 6567 7265 7373  also add regress
+00013a90: 6f72 2069 6e70 7574 0d0a 2020 2020 2020  or input..      
+00013aa0: 2020 2320 7265 6772 6573 736f 7273 2069    # regressors i
+00013ab0: 6d70 6f72 7461 6e74 2c20 6573 7469 6d61  mportant, estima
+00013ac0: 7469 6f6e 2062 7920 6c69 6e65 6172 2066  tion by linear f
+00013ad0: 6c61 6720 2872 6574 7572 6e20 7374 6174  lag (return stat
+00013ae0: 7329 206f 7220 6279 2025 2076 7320 666f  s) or by % vs fo
+00013af0: 7265 6361 7374 2066 726f 6d20 6375 746f  recast from cuto
+00013b00: 6666 0d0a 2020 2020 2020 2020 2320 7374  ff..        # st
+00013b10: 6172 7420 616e 6420 656e 6420 6461 7465  art and end date
+00013b20: 732c 206d 756c 7469 706c 6520 7472 6561  s, multiple trea
+00013b30: 746d 656e 7473 2c20 7661 7279 2062 7920  tments, vary by 
+00013b40: 7365 7269 6573 0d0a 2020 2020 2020 2020  series..        
+00013b50: 2320 6f72 206d 6179 6265 2069 6e73 7465  # or maybe inste
+00013b60: 6164 2c20 6a75 7374 2072 6574 7572 6e20  ad, just return 
+00013b70: 7468 6520 7374 6174 7320 666f 7220 616c  the stats for al
+00013b80: 6c20 696e 7075 7420 7265 6772 6573 736f  l input regresso
+00013b90: 7273 0d0a 2020 2020 2020 2020 2320 7374  rs..        # st
+00013ba0: 696c 6c20 776f 726b 696e 6720 6f6e 2074  ill working on t
+00013bb0: 6869 732c 2070 6f73 7369 626c 7920 6a75  his, possibly ju
+00013bc0: 7374 2068 7474 7073 3a2f 2f6d 6174 682e  st https://math.
+00013bd0: 7374 6163 6b65 7863 6861 6e67 652e 636f  stackexchange.co
+00013be0: 6d2f 7175 6573 7469 6f6e 732f 3231 3132  m/questions/2112
+00013bf0: 3535 332f 7374 6174 6973 7469 6361 6c2d  553/statistical-
+00013c00: 7369 676e 6966 6963 616e 6365 2d6f 662d  significance-of-
+00013c10: 6c69 6e65 6172 2d6c 6561 7374 2d73 7175  linear-least-squ
+00013c20: 6172 6573 0d0a 2020 2020 2020 2020 2320  ares..        # 
+00013c30: 616e 6420 6f74 6865 7220 6665 6174 7572  and other featur
+00013c40: 6573 2061 6c61 2053 7461 7473 6d6f 6465  es ala Statsmode
+00013c50: 6c73 204f 4c53 2c20 5661 7228 ceb2 5e29  ls OLS, Var(..^)
+00013c60: 3dcf 8332 2858 e280 b258 29e2 8892 3120  =..2(X...X)...1 
+00013c70: 7768 6572 6520 cf83 323e 3020 6973 2074  where ..2>0 is t
+00013c80: 6865 2063 6f6d 6d6f 6e20 7661 7269 616e  he common varian
+00013c90: 6365 206f 6620 6561 6368 2065 6c65 6d65  ce of each eleme
+00013ca0: 6e74 206f 6620 7468 6520 6572 726f 7220  nt of the error 
+00013cb0: 7665 6374 6f72 0d0a 2020 2020 2020 2020  vector..        
+00013cc0: 7265 7475 726e 204e 6f74 496d 706c 656d  return NotImplem
+00013cd0: 656e 7465 640d 0a0d 0a20 2020 2064 6566  ented....    def
+00013ce0: 2070 7265 6469 6374 5f6e 6577 5f70 726f   predict_new_pro
+00013cf0: 6475 6374 2873 656c 6629 3a0d 0a20 2020  duct(self):..   
+00013d00: 2020 2020 2023 2062 6f72 726f 7720 7468       # borrow th
+00013d10: 6520 6c69 6e65 6172 2063 6f6d 706f 6e65  e linear compone
+00013d20: 6e74 7320 6672 6f6d 2061 2072 656c 6174  nts from a relat
+00013d30: 6564 2070 726f 6475 6374 2028 6f72 2061  ed product (or a
+00013d40: 7667 2f6d 6f64 6520 6966 206e 6f74 2067  vg/mode if not g
+00013d50: 6976 656e 290d 0a20 2020 2020 2020 2023  iven)..        #
+00013d60: 2068 6176 6520 7468 6520 7472 656e 6420   have the trend 
+00013d70: 7374 6172 7420 6174 207a 6572 6f20 7468  start at zero th
+00013d80: 656e 2075 702c 206c 696b 6520 7265 7665  en up, like reve
+00013d90: 7273 6520 7068 690d 0a20 2020 2020 2020  rse phi..       
+00013da0: 2023 2070 6f73 7369 626c 7920 626f 7272   # possibly borr
+00013db0: 6f77 2077 6172 6d75 7020 6672 6f6d 2061  ow warmup from a
+00013dc0: 6e79 2073 6572 6965 7320 7468 6174 2068  ny series that h
+00013dd0: 6176 6520 6120 6c6f 6769 7374 6963 2d6c  ave a logistic-l
+00013de0: 696b 6520 7472 656e 640d 0a20 2020 2020  ike trend..     
+00013df0: 2020 2023 2063 6c75 7374 6572 2061 6e64     # cluster and
+00013e00: 2063 686f 6f73 6520 7468 6520 6269 6767   choose the bigg
+00013e10: 6573 7420 636c 7573 7465 7220 2861 7320  est cluster (as 
+00013e20: 6176 6720 7661 6c75 6520 6e61 6976 6520  avg value naive 
+00013e30: 6d65 7468 6f64 2c20 6d61 7962 6520 726f  method, maybe ro
+00013e40: 756e 6420 6f72 2066 696c 7465 7220 6669  und or filter fi
+00013e50: 7273 7429 0d0a 2020 2020 2020 2020 7265  rst)..        re
+00013e60: 7475 726e 204e 6f74 496d 706c 656d 656e  turn NotImplemen
+00013e70: 7465 640d 0a0d 0a20 2020 2064 6566 2066  ted....    def f
+00013e80: 6561 7475 7265 5f69 6d70 6f72 7461 6e63  eature_importanc
+00013e90: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
+00013ea0: 2020 2320 7261 6e6b 2063 6f65 6666 6963    # rank coeffic
+00013eb0: 6965 6e74 7320 6279 2069 6d70 6f72 7461  ients by importa
+00013ec0: 6e63 650d 0a20 2020 2020 2020 2072 6574  nce..        ret
+00013ed0: 7572 6e20 4e6f 7449 6d70 6c65 6d65 6e74  urn NotImplement
+00013ee0: 6564 0d0a 0d0a 2020 2020 6465 6620 636f  ed....    def co
+00013ef0: 6d70 6172 655f 6163 7475 616c 5f63 6f6d  mpare_actual_com
+00013f00: 706f 6e65 6e74 7328 7365 6c66 293a 0d0a  ponents(self):..
+00013f10: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00013f20: 6f74 496d 706c 656d 656e 7465 640d 0a0d  otImplemented...
+00013f30: 0a20 2020 2064 6566 2067 6574 5f6e 6577  .    def get_new
+00013f40: 5f70 6172 616d 7328 7365 6c66 2c20 6d65  _params(self, me
+00013f50: 7468 6f64 3d27 6661 7374 2729 3a0d 0a20  thod='fast'):.. 
+00013f60: 2020 2020 2020 2023 2068 6176 6520 6661         # have fa
+00013f70: 7374 206f 7074 696f 6e20 7468 6174 2061  st option that a
+00013f80: 766f 6964 7320 616e 7920 6f66 2074 6865  voids any of the
+00013f90: 206c 6f6f 7020 6170 7072 6f61 6368 6573   loop approaches
+00013fa0: 0d0a 2020 2020 2020 2020 7363 616c 696e  ..        scalin
+00013fb0: 6720 3d20 7261 6e64 6f6d 2e63 686f 6963  g = random.choic
+00013fc0: 6573 285b 2742 6173 6553 6361 6c65 7227  es(['BaseScaler'
+00013fd0: 2c20 276f 7468 6572 275d 2c20 5b30 2e38  , 'other'], [0.8
+00013fe0: 2c20 302e 325d 295b 305d 0d0a 2020 2020  , 0.2])[0]..    
+00013ff0: 2020 2020 6966 2073 6361 6c69 6e67 203d      if scaling =
+00014000: 3d20 226f 7468 6572 223a 0d0a 2020 2020  = "other":..    
+00014010: 2020 2020 2020 2020 7363 616c 696e 6720          scaling 
+00014020: 3d20 5261 6e64 6f6d 5472 616e 7366 6f72  = RandomTransfor
+00014030: 6d28 0d0a 2020 2020 2020 2020 2020 2020  m(..            
+00014040: 2020 2020 7472 616e 7366 6f72 6d65 725f      transformer_
+00014050: 6c69 7374 3d73 6361 6c65 7273 2c0d 0a20  list=scalers,.. 
+00014060: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00014070: 7261 6e73 666f 726d 6572 5f6d 6178 5f64  ransformer_max_d
+00014080: 6570 7468 3d31 2c0d 0a20 2020 2020 2020  epth=1,..       
+00014090: 2020 2020 2020 2020 2061 6c6c 6f77 5f6e           allow_n
+000140a0: 6f6e 653d 4661 6c73 652c 0d0a 2020 2020  one=False,..    
+000140b0: 2020 2020 2020 2020 2020 2020 6e6f 5f6e              no_n
+000140c0: 616e 5f66 696c 6c3d 5472 7565 2c0d 0a20  an_fill=True,.. 
+000140d0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+000140e0: 2020 2020 2020 686f 6c69 6461 795f 7061        holiday_pa
+000140f0: 7261 6d73 203d 2072 616e 646f 6d2e 6368  rams = random.ch
+00014100: 6f69 6365 7328 5b4e 6f6e 652c 2027 616e  oices([None, 'an
+00014110: 7927 5d2c 205b 302e 352c 2030 2e35 5d29  y'], [0.5, 0.5])
+00014120: 5b30 5d0d 0a20 2020 2020 2020 2023 2068  [0]..        # h
+00014130: 6f6c 6964 6179 5f69 6e74 6572 7665 6e74  oliday_intervent
+00014140: 696f 6e20 3d20 4e6f 6e65 0d0a 2020 2020  ion = None..    
+00014150: 2020 2020 6966 2068 6f6c 6964 6179 5f70      if holiday_p
+00014160: 6172 616d 7320 6973 206e 6f74 204e 6f6e  arams is not Non
+00014170: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00014180: 2320 686f 6c69 6461 795f 696e 7465 7276  # holiday_interv
+00014190: 656e 7469 6f6e 203d 2072 616e 646f 6d2e  ention = random.
+000141a0: 6368 6f69 6365 285b 2763 7265 6174 655f  choice(['create_
+000141b0: 6665 6174 7572 6527 2c20 2775 7365 5f69  feature', 'use_i
+000141c0: 6d70 6163 7427 5d29 0d0a 2020 2020 2020  mpact'])..      
+000141d0: 2020 2020 2020 686f 6c69 6461 795f 7061        holiday_pa
+000141e0: 7261 6d73 203d 2048 6f6c 6964 6179 5472  rams = HolidayTr
+000141f0: 616e 7366 6f72 6d65 722e 6765 745f 6e65  ansformer.get_ne
+00014200: 775f 7061 7261 6d73 286d 6574 686f 643d  w_params(method=
+00014210: 6d65 7468 6f64 290d 0a20 2020 2020 2020  method)..       
+00014220: 2020 2020 2068 6f6c 6964 6179 5f70 6172       holiday_par
+00014230: 616d 735b 2769 6d70 6163 7427 5d20 3d20  ams['impact'] = 
+00014240: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
+00014250: 2020 686f 6c69 6461 795f 7061 7261 6d73    holiday_params
+00014260: 5b27 7265 6772 6573 7369 6f6e 5f70 6172  ['regression_par
+00014270: 616d 7327 5d20 3d20 4e6f 6e65 0d0a 2020  ams'] = None..  
+00014280: 2020 2020 2020 2020 2020 686f 6c69 6461            holida
+00014290: 795f 7061 7261 6d73 5b27 7265 6d6f 7665  y_params['remove
+000142a0: 5f65 7863 6573 735f 616e 6f6d 616c 6965  _excess_anomalie
+000142b0: 7327 5d20 3d20 7261 6e64 6f6d 2e63 686f  s'] = random.cho
+000142c0: 6963 6573 280d 0a20 2020 2020 2020 2020  ices(..         
+000142d0: 2020 2020 2020 205b 5472 7565 2c20 4661         [True, Fa
+000142e0: 6c73 655d 2c20 5b30 2e30 352c 2030 2e39  lse], [0.05, 0.9
+000142f0: 355d 0d0a 2020 2020 2020 2020 2020 2020  5]..            
+00014300: 295b 305d 0d0a 2020 2020 2020 2020 2020  )[0]..          
+00014310: 2020 686f 6c69 6461 795f 7061 7261 6d73    holiday_params
+00014320: 5b27 6f75 7470 7574 275d 203d 2072 616e  ['output'] = ran
+00014330: 646f 6d2e 6368 6f69 6365 7328 0d0a 2020  dom.choices(..  
+00014340: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
+00014350: 6d75 6c74 6976 6172 6961 7465 272c 2027  multivariate', '
+00014360: 756e 6976 6172 6961 7465 275d 2c20 5b30  univariate'], [0
+00014370: 2e39 2c20 302e 315d 0d0a 2020 2020 2020  .9, 0.1]..      
+00014380: 2020 2020 2020 295b 305d 0d0a 2020 2020        )[0]..    
+00014390: 2020 2020 616e 6f6d 616c 795f 696e 7465      anomaly_inte
+000143a0: 7276 656e 7469 6f6e 203d 2072 616e 646f  rvention = rando
+000143b0: 6d2e 6368 6f69 6365 7328 0d0a 2020 2020  m.choices(..    
+000143c0: 2020 2020 2020 2020 5b4e 6f6e 652c 2027          [None, '
+000143d0: 7265 6d6f 7665 272c 2027 6465 7465 6374  remove', 'detect
+000143e0: 5f6f 6e6c 7927 2c20 276d 6f64 656c 275d  _only', 'model']
+000143f0: 2c20 5b30 2e39 2c20 302e 332c 2030 2e30  , [0.9, 0.3, 0.0
+00014400: 352c 2030 2e30 355d 0d0a 2020 2020 2020  5, 0.05]..      
+00014410: 2020 295b 305d 0d0a 2020 2020 2020 2020    )[0]..        
+00014420: 6966 2061 6e6f 6d61 6c79 5f69 6e74 6572  if anomaly_inter
+00014430: 7665 6e74 696f 6e20 6973 206e 6f74 204e  vention is not N
+00014440: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00014450: 2020 616e 6f6d 616c 795f 6465 7465 6374    anomaly_detect
+00014460: 6f72 5f70 6172 616d 7320 3d20 416e 6f6d  or_params = Anom
+00014470: 616c 7952 656d 6f76 616c 2e67 6574 5f6e  alyRemoval.get_n
+00014480: 6577 5f70 6172 616d 7328 6d65 7468 6f64  ew_params(method
+00014490: 3d6d 6574 686f 6429 0d0a 2020 2020 2020  =method)..      
+000144a0: 2020 2020 2020 6966 2061 6e6f 6d61 6c79        if anomaly
+000144b0: 5f69 6e74 6572 7665 6e74 696f 6e20 3d3d  _intervention ==
+000144c0: 2022 6d6f 6465 6c22 3a0d 0a20 2020 2020   "model":..     
+000144d0: 2020 2020 2020 2020 2020 2061 6e6f 6d61             anoma
+000144e0: 6c79 5f69 6e74 6572 7665 6e74 696f 6e20  ly_intervention 
+000144f0: 3d20 6765 6e65 7261 6c5f 7465 6d70 6c61  = general_templa
+00014500: 7465 2e73 616d 706c 6528 3129 2e74 6f5f  te.sample(1).to_
+00014510: 6469 6374 2822 7265 636f 7264 7322 295b  dict("records")[
+00014520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014530: 2020 2020 2020 300d 0a20 2020 2020 2020        0..       
+00014540: 2020 2020 2020 2020 205d 2020 2320 706c           ]  # pl
+00014550: 6163 6568 6f6c 6465 722c 2070 726f 6261  aceholder, proba
+00014560: 626c 790d 0a20 2020 2020 2020 2065 6c73  bly..        els
+00014570: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00014580: 616e 6f6d 616c 795f 6465 7465 6374 6f72  anomaly_detector
+00014590: 5f70 6172 616d 7320 3d20 4e6f 6e65 0d0a  _params = None..
+000145a0: 0d0a 2020 2020 2020 2020 2320 7261 6e64  ..        # rand
+000145b0: 6f6d 206f 7220 7072 6574 6573 7465 6420  om or pretested 
+000145c0: 6465 6661 756c 7473 0d0a 2020 2020 2020  defaults..      
+000145d0: 2020 6966 206d 6574 686f 6420 696e 205b    if method in [
+000145e0: 2764 6565 7027 2c20 2761 6c6c 275d 3a0d  'deep', 'all']:.
+000145f0: 0a20 2020 2020 2020 2020 2020 2074 7265  .            tre
+00014600: 6e64 5f62 6173 6520 3d20 2764 6565 7027  nd_base = 'deep'
+00014610: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00014620: 0a20 2020 2020 2020 2020 2020 2074 7265  .            tre
+00014630: 6e64 5f62 6173 6520 3d20 7261 6e64 6f6d  nd_base = random
+00014640: 2e63 686f 6963 6573 280d 0a20 2020 2020  .choices(..     
+00014650: 2020 2020 2020 2020 2020 205b 2770 6231             ['pb1
+00014660: 272c 2027 7062 3227 2c20 2770 6233 272c  ', 'pb2', 'pb3',
+00014670: 2027 7261 6e64 6f6d 275d 2c20 5b30 2e31   'random'], [0.1
+00014680: 2c20 302e 312c 2030 2e30 2c20 302e 385d  , 0.1, 0.0, 0.8]
+00014690: 0d0a 2020 2020 2020 2020 2020 2020 295b  ..            )[
+000146a0: 305d 0d0a 2020 2020 2020 2020 6966 2074  0]..        if t
+000146b0: 7265 6e64 5f62 6173 6520 3d3d 2022 7261  rend_base == "ra
+000146c0: 6e64 6f6d 223a 0d0a 2020 2020 2020 2020  ndom":..        
+000146d0: 2020 2020 6d6f 6465 6c5f 7374 7220 3d20      model_str = 
+000146e0: 7261 6e64 6f6d 2e63 686f 6963 6573 280d  random.choices(.
+000146f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014700: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+00014710: 2020 2020 2020 2020 2741 7665 7261 6765          'Average
+00014720: 5661 6c75 654e 6169 7665 272c 0d0a 2020  ValueNaive',..  
+00014730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014740: 2020 274d 6574 7269 634d 6f74 6966 272c    'MetricMotif',
+00014750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014760: 2020 2020 2020 224c 6173 7456 616c 7565        "LastValue
+00014770: 4e61 6976 6522 2c0d 0a20 2020 2020 2020  Naive",..       
+00014780: 2020 2020 2020 2020 2020 2020 2027 5365               'Se
+00014790: 6173 6f6e 616c 6974 794d 6f74 6966 272c  asonalityMotif',
+000147a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000147b0: 2020 2020 2020 2757 696e 646f 7752 6567        'WindowReg
+000147c0: 7265 7373 696f 6e27 2c0d 0a20 2020 2020  ression',..     
+000147d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000147e0: 4152 444c 272c 0d0a 2020 2020 2020 2020  ARDL',..        
+000147f0: 2020 2020 2020 2020 2020 2020 2756 4152              'VAR
+00014800: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00014810: 2020 2020 2020 2020 2755 6e69 7661 7269          'Univari
+00014820: 6174 654d 6f74 6966 272c 0d0a 2020 2020  ateMotif',..    
+00014830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014840: 2755 6e6f 6273 6572 7665 6443 6f6d 706f  'UnobservedCompo
+00014850: 6e65 6e74 7327 2c0d 0a20 2020 2020 2020  nents',..       
+00014860: 2020 2020 2020 2020 2020 2020 2022 4b61               "Ka
+00014870: 6c6d 616e 5374 6174 6553 7061 6365 222c  lmanStateSpace",
+00014880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014890: 2020 2020 2020 2752 5256 4152 272c 0d0a        'RRVAR',..
+000148a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148b0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+000148c0: 2020 2020 5b30 2e30 352c 2030 2e30 352c      [0.05, 0.05,
+000148d0: 2030 2e31 2c20 302e 3035 2c20 302e 3035   0.1, 0.05, 0.05
+000148e0: 2c20 302e 3135 2c20 302e 3035 2c20 302e  , 0.15, 0.05, 0.
+000148f0: 3035 2c20 302e 3035 2c20 302e 3035 2c20  05, 0.05, 0.05, 
+00014900: 302e 3035 5d2c 0d0a 2020 2020 2020 2020  0.05],..        
+00014910: 2020 2020 2020 2020 6b3d 312c 0d0a 2020          k=1,..  
+00014920: 2020 2020 2020 2020 2020 295b 305d 0d0a            )[0]..
+00014930: 2020 2020 2020 2020 2020 2020 7472 656e              tren
+00014940: 645f 6d6f 6465 6c20 3d20 7b27 4d6f 6465  d_model = {'Mode
+00014950: 6c27 3a20 6d6f 6465 6c5f 7374 727d 0d0a  l': model_str}..
+00014960: 2020 2020 2020 2020 2020 2020 7472 656e              tren
+00014970: 645f 6d6f 6465 6c5b 274d 6f64 656c 5061  d_model['ModelPa
+00014980: 7261 6d65 7465 7273 275d 203d 204d 6f64  rameters'] = Mod
+00014990: 656c 4d6f 6e73 7465 7228 6d6f 6465 6c5f  elMonster(model_
+000149a0: 7374 7229 2e67 6574 5f6e 6577 5f70 6172  str).get_new_par
+000149b0: 616d 7328 0d0a 2020 2020 2020 2020 2020  ams(..          
+000149c0: 2020 2020 2020 6d65 7468 6f64 3d6d 6574        method=met
+000149d0: 686f 640d 0a20 2020 2020 2020 2020 2020  hod..           
+000149e0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+000149f0: 7472 656e 645f 7472 616e 7366 6f72 6d61  trend_transforma
+00014a00: 7469 6f6e 203d 2052 616e 646f 6d54 7261  tion = RandomTra
+00014a10: 6e73 666f 726d 280d 0a20 2020 2020 2020  nsform(..       
+00014a20: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
+00014a30: 726d 6572 5f6c 6973 743d 2266 6173 7422  rmer_list="fast"
+00014a40: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00014a50: 2020 2074 7261 6e73 666f 726d 6572 5f6d     transformer_m
+00014a60: 6178 5f64 6570 7468 3d33 2c20 2023 2070  ax_depth=3,  # p
+00014a70: 726f 6261 626c 7920 7761 6e74 2073 6f6d  robably want som
+00014a80: 6520 6d6f 7265 2075 7361 626c 6520 6465  e more usable de
+00014a90: 6661 756c 7473 2066 6972 7374 2061 7320  faults first as 
+00014aa0: 6d61 6e79 2072 616e 646f 6d20 6172 6520  many random are 
+00014ab0: 7365 6e73 656c 6573 730d 0a20 2020 2020  senseless..     
+00014ac0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00014ad0: 2020 656c 6966 2074 7265 6e64 5f62 6173    elif trend_bas
+00014ae0: 6520 3d3d 2027 7062 3127 3a0d 0a20 2020  e == 'pb1':..   
+00014af0: 2020 2020 2020 2020 2074 7265 6e64 5f6d           trend_m
+00014b00: 6f64 656c 203d 207b 274d 6f64 656c 273a  odel = {'Model':
+00014b10: 2027 4152 444c 277d 0d0a 2020 2020 2020   'ARDL'}..      
+00014b20: 2020 2020 2020 7472 656e 645f 6d6f 6465        trend_mode
+00014b30: 6c5b 274d 6f64 656c 5061 7261 6d65 7465  l['ModelParamete
+00014b40: 7273 275d 203d 207b 0d0a 2020 2020 2020  rs'] = {..      
+00014b50: 2020 2020 2020 2020 2020 226c 6167 7322            "lags"
+00014b60: 3a20 312c 0d0a 2020 2020 2020 2020 2020  : 1,..          
+00014b70: 2020 2020 2020 2274 7265 6e64 223a 2022        "trend": "
+00014b80: 6e22 2c0d 0a20 2020 2020 2020 2020 2020  n",..           
+00014b90: 2020 2020 2022 6f72 6465 7222 3a20 302c       "order": 0,
+00014ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014bb0: 2020 2263 6175 7361 6c22 3a20 4661 6c73    "causal": Fals
+00014bc0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00014bd0: 2020 2020 2272 6567 7265 7373 696f 6e5f      "regression_
+00014be0: 7479 7065 223a 2022 7369 6d70 6c65 222c  type": "simple",
+00014bf0: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
+00014c00: 0a20 2020 2020 2020 2020 2020 2074 7265  .            tre
+00014c10: 6e64 5f74 7261 6e73 666f 726d 6174 696f  nd_transformatio
+00014c20: 6e20 3d20 7b0d 0a20 2020 2020 2020 2020  n = {..         
+00014c30: 2020 2020 2020 2022 6669 6c6c 6e61 223a         "fillna":
+00014c40: 2022 6e65 6172 6573 7422 2c0d 0a20 2020   "nearest",..   
+00014c50: 2020 2020 2020 2020 2020 2020 2022 7472               "tr
+00014c60: 616e 7366 6f72 6d61 7469 6f6e 7322 3a20  ansformations": 
+00014c70: 7b22 3022 3a20 2253 7461 6e64 6172 6453  {"0": "StandardS
+00014c80: 6361 6c65 7222 2c20 2231 223a 2022 416e  caler", "1": "An
+00014c90: 6f6d 616c 7952 656d 6f76 616c 227d 2c0d  omalyRemoval"},.
+00014ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014cb0: 2022 7472 616e 7366 6f72 6d61 7469 6f6e   "transformation
+00014cc0: 5f70 6172 616d 7322 3a20 7b0d 0a20 2020  _params": {..   
+00014cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ce0: 2022 3022 3a20 7b7d 2c0d 0a20 2020 2020   "0": {},..     
+00014cf0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00014d00: 3122 3a20 7b0d 0a20 2020 2020 2020 2020  1": {..         
+00014d10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00014d20: 6d65 7468 6f64 223a 2022 4951 5222 2c0d  method": "IQR",.
+00014d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014d40: 2020 2020 2020 2020 2022 7472 616e 7366           "transf
+00014d50: 6f72 6d5f 6469 6374 223a 207b 0d0a 2020  orm_dict": {..  
+00014d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d70: 2020 2020 2020 2020 2020 2266 696c 6c6e            "filln
+00014d80: 6122 3a20 4e6f 6e65 2c0d 0a20 2020 2020  a": None,..     
+00014d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014da0: 2020 2020 2020 2022 7472 616e 7366 6f72         "transfor
+00014db0: 6d61 7469 6f6e 7322 3a20 7b22 3022 3a20  mations": {"0": 
+00014dc0: 2243 6c69 704f 7574 6c69 6572 7322 7d2c  "ClipOutliers"},
+00014dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014de0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00014df0: 7261 6e73 666f 726d 6174 696f 6e5f 7061  ransformation_pa
+00014e00: 7261 6d73 223a 207b 0d0a 2020 2020 2020  rams": {..      
+00014e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e20: 2020 2020 2020 2020 2020 2230 223a 207b            "0": {
+00014e30: 226d 6574 686f 6422 3a20 2263 6c69 7022  "method": "clip"
+00014e40: 2c20 2273 7464 5f74 6872 6573 686f 6c64  , "std_threshold
+00014e50: 223a 2036 7d0d 0a20 2020 2020 2020 2020  ": 6}..         
+00014e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e70: 2020 207d 2c0d 0a20 2020 2020 2020 2020     },..         
+00014e80: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00014e90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00014ea0: 2020 2020 2020 2020 2020 2022 6d65 7468             "meth
+00014eb0: 6f64 5f70 6172 616d 7322 3a20 7b0d 0a20  od_params": {.. 
+00014ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ed0: 2020 2020 2020 2020 2020 2022 6971 725f             "iqr_
+00014ee0: 7468 7265 7368 6f6c 6422 3a20 322e 352c  threshold": 2.5,
+00014ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014f00: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+00014f10: 7172 5f71 7561 6e74 696c 6573 223a 205b  qr_quantiles": [
+00014f20: 302e 3235 2c20 302e 3735 5d2c 0d0a 2020  0.25, 0.75],..  
+00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f40: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
+00014f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f60: 2020 2266 696c 6c6e 6122 3a20 2266 6669    "fillna": "ffi
+00014f70: 6c6c 222c 0d0a 2020 2020 2020 2020 2020  ll",..          
+00014f80: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
+00014f90: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00014fa0: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
+00014fb0: 0a20 2020 2020 2020 2065 6c69 6620 7472  .        elif tr
+00014fc0: 656e 645f 6261 7365 203d 3d20 2770 6232  end_base == 'pb2
+00014fd0: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
+00014fe0: 7472 656e 645f 6d6f 6465 6c20 3d20 7b27  trend_model = {'
+00014ff0: 4d6f 6465 6c27 3a20 2757 696e 646f 7752  Model': 'WindowR
+00015000: 6567 7265 7373 696f 6e27 7d0d 0a20 2020  egression'}..   
+00015010: 2020 2020 2020 2020 2074 7265 6e64 5f6d           trend_m
+00015020: 6f64 656c 5b27 4d6f 6465 6c50 6172 616d  odel['ModelParam
+00015030: 6574 6572 7327 5d20 3d20 7b0d 0a20 2020  eters'] = {..   
+00015040: 2020 2020 2020 2020 2020 2020 2022 7769               "wi
+00015050: 6e64 6f77 5f73 697a 6522 3a20 3132 2c0d  ndow_size": 12,.
+00015060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015070: 2022 696e 7075 745f 6469 6d22 3a20 2275   "input_dim": "u
+00015080: 6e69 7661 7269 6174 6522 2c0d 0a20 2020  nivariate",..   
+00015090: 2020 2020 2020 2020 2020 2020 2022 6f75               "ou
+000150a0: 7470 7574 5f64 696d 223a 2022 3173 7465  tput_dim": "1ste
+000150b0: 7022 2c0d 0a20 2020 2020 2020 2020 2020  p",..           
+000150c0: 2020 2020 2022 6e6f 726d 616c 697a 655f       "normalize_
+000150d0: 7769 6e64 6f77 223a 2046 616c 7365 2c0d  window": False,.
+000150e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000150f0: 2022 6d61 785f 7769 6e64 6f77 7322 3a20   "max_windows": 
+00015100: 3830 3030 2c0d 0a20 2020 2020 2020 2020  8000,..         
+00015110: 2020 2020 2020 2022 7265 6772 6573 7369         "regressi
+00015120: 6f6e 5f74 7970 6522 3a20 4e6f 6e65 2c0d  on_type": None,.
+00015130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015140: 2022 7265 6772 6573 7369 6f6e 5f6d 6f64   "regression_mod
+00015150: 656c 223a 207b 0d0a 2020 2020 2020 2020  el": {..        
+00015160: 2020 2020 2020 2020 2020 2020 226d 6f64              "mod
+00015170: 656c 223a 2022 4578 7472 6154 7265 6573  el": "ExtraTrees
+00015180: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00015190: 2020 2020 2020 2020 226d 6f64 656c 5f70          "model_p
+000151a0: 6172 616d 7322 3a20 7b0d 0a20 2020 2020  arams": {..     
+000151b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151c0: 2020 2022 6e5f 6573 7469 6d61 746f 7273     "n_estimators
+000151d0: 223a 2031 3030 2c0d 0a20 2020 2020 2020  ": 100,..       
+000151e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151f0: 2022 6d69 6e5f 7361 6d70 6c65 735f 6c65   "min_samples_le
+00015200: 6166 223a 2031 2c0d 0a20 2020 2020 2020  af": 1,..       
+00015210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015220: 2022 6d61 785f 6465 7074 6822 3a20 3230   "max_depth": 20
+00015230: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00015240: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
+00015250: 2020 2020 2020 2020 2020 207d 2c0d 0a20             },.. 
+00015260: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+00015270: 2020 2020 2020 2020 2020 7472 656e 645f            trend_
+00015280: 7472 616e 7366 6f72 6d61 7469 6f6e 203d  transformation =
+00015290: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+000152a0: 2020 2020 2266 696c 6c6e 6122 3a20 2266      "fillna": "f
+000152b0: 6669 6c6c 222c 0d0a 2020 2020 2020 2020  fill",..        
+000152c0: 2020 2020 2020 2020 2274 7261 6e73 666f          "transfo
+000152d0: 726d 6174 696f 6e73 223a 207b 2230 223a  rmations": {"0":
+000152e0: 2022 416e 6f6d 616c 7952 656d 6f76 616c   "AnomalyRemoval
+000152f0: 222c 2022 3122 3a20 2252 6f62 7573 7453  ", "1": "RobustS
+00015300: 6361 6c65 7222 7d2c 0d0a 2020 2020 2020  caler"},..      
+00015310: 2020 2020 2020 2020 2020 2274 7261 6e73            "trans
+00015320: 666f 726d 6174 696f 6e5f 7061 7261 6d73  formation_params
+00015330: 223a 207b 0d0a 2020 2020 2020 2020 2020  ": {..          
+00015340: 2020 2020 2020 2020 2020 2230 223a 207b            "0": {
+00015350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015360: 2020 2020 2020 2020 2020 226d 6574 686f            "metho
+00015370: 6422 3a20 2249 5152 222c 0d0a 2020 2020  d": "IQR",..    
+00015380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015390: 2020 2020 2274 7261 6e73 666f 726d 5f64      "transform_d
+000153a0: 6963 7422 3a20 7b0d 0a20 2020 2020 2020  ict": {..       
+000153b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153c0: 2020 2020 2022 6669 6c6c 6e61 223a 204e       "fillna": N
+000153d0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+000153e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153f0: 2020 2274 7261 6e73 666f 726d 6174 696f    "transformatio
+00015400: 6e73 223a 207b 2230 223a 2022 436c 6970  ns": {"0": "Clip
+00015410: 4f75 746c 6965 7273 227d 2c0d 0a20 2020  Outliers"},..   
+00015420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015430: 2020 2020 2020 2020 2022 7472 616e 7366           "transf
+00015440: 6f72 6d61 7469 6f6e 5f70 6172 616d 7322  ormation_params"
+00015450: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
+00015460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015470: 2020 2020 2022 3022 3a20 7b22 6d65 7468       "0": {"meth
+00015480: 6f64 223a 2022 636c 6970 222c 2022 7374  od": "clip", "st
+00015490: 645f 7468 7265 7368 6f6c 6422 3a20 367d  d_threshold": 6}
+000154a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000154b0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+000154c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000154d0: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
+000154e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154f0: 2020 2020 2020 226d 6574 686f 645f 7061        "method_pa
+00015500: 7261 6d73 223a 207b 0d0a 2020 2020 2020  rams": {..      
+00015510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015520: 2020 2020 2020 2269 7172 5f74 6872 6573        "iqr_thres
+00015530: 686f 6c64 223a 2032 2e35 2c0d 0a20 2020  hold": 2.5,..   
+00015540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015550: 2020 2020 2020 2020 2022 6971 725f 7175           "iqr_qu
+00015560: 616e 7469 6c65 7322 3a20 5b30 2e32 352c  antiles": [0.25,
+00015570: 2030 2e37 355d 2c0d 0a20 2020 2020 2020   0.75],..       
+00015580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015590: 207d 2c0d 0a20 2020 2020 2020 2020 2020   },..           
+000155a0: 2020 2020 2020 2020 2020 2020 2022 6669               "fi
+000155b0: 6c6c 6e61 223a 2022 6666 696c 6c22 2c0d  llna": "ffill",.
+000155c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000155d0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
+000155e0: 2020 2020 2020 2020 2020 2020 2022 3122               "1"
+000155f0: 3a20 7b7d 2c0d 0a20 2020 2020 2020 2020  : {},..         
+00015600: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
+00015610: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00015620: 2020 656c 6966 2074 7265 6e64 5f62 6173    elif trend_bas
+00015630: 6520 3d3d 2022 6465 6570 223a 0d0a 2020  e == "deep":..  
+00015640: 2020 2020 2020 2020 2020 6d6f 6465 6c5f            model_
+00015650: 6c69 7374 203d 2022 616c 6c5f 7072 6167  list = "all_prag
+00015660: 6d61 7469 6322 0d0a 2020 2020 2020 2020  matic"..        
+00015670: 2020 2020 6d6f 6465 6c5f 6c69 7374 2c20      model_list, 
+00015680: 6d6f 6465 6c5f 7072 6f62 203d 206d 6f64  model_prob = mod
+00015690: 656c 5f6c 6973 745f 746f 5f64 6963 7428  el_list_to_dict(
+000156a0: 6d6f 6465 6c5f 6c69 7374 290d 0a20 2020  model_list)..   
+000156b0: 2020 2020 2020 2020 206d 6f64 656c 5f73           model_s
+000156c0: 7472 203d 2072 616e 646f 6d2e 6368 6f69  tr = random.choi
+000156d0: 6365 7328 6d6f 6465 6c5f 6c69 7374 2c20  ces(model_list, 
+000156e0: 6d6f 6465 6c5f 7072 6f62 2c20 6b3d 3129  model_prob, k=1)
+000156f0: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+00015700: 2074 7265 6e64 5f6d 6f64 656c 203d 207b   trend_model = {
+00015710: 274d 6f64 656c 273a 206d 6f64 656c 5f73  'Model': model_s
+00015720: 7472 7d0d 0a20 2020 2020 2020 2020 2020  tr}..           
+00015730: 2074 7265 6e64 5f6d 6f64 656c 5b27 4d6f   trend_model['Mo
+00015740: 6465 6c50 6172 616d 6574 6572 7327 5d20  delParameters'] 
+00015750: 3d20 4d6f 6465 6c4d 6f6e 7374 6572 286d  = ModelMonster(m
+00015760: 6f64 656c 5f73 7472 292e 6765 745f 6e65  odel_str).get_ne
+00015770: 775f 7061 7261 6d73 280d 0a20 2020 2020  w_params(..     
+00015780: 2020 2020 2020 2020 2020 206d 6574 686f             metho
+00015790: 643d 6d65 7468 6f64 0d0a 2020 2020 2020  d=method..      
+000157a0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000157b0: 2020 2020 2074 7265 6e64 5f74 7261 6e73       trend_trans
+000157c0: 666f 726d 6174 696f 6e20 3d20 5261 6e64  formation = Rand
+000157d0: 6f6d 5472 616e 7366 6f72 6d28 0d0a 2020  omTransform(..  
+000157e0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000157f0: 616e 7366 6f72 6d65 725f 6c69 7374 3d22  ansformer_list="
+00015800: 616c 6c22 2c0d 0a20 2020 2020 2020 2020  all",..         
+00015810: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00015820: 6572 5f6d 6178 5f64 6570 7468 3d33 2c20  er_max_depth=3, 
+00015830: 2023 2070 726f 6261 626c 7920 7761 6e74   # probably want
+00015840: 2073 6f6d 6520 6d6f 7265 2075 7361 626c   some more usabl
+00015850: 6520 6465 6661 756c 7473 2066 6972 7374  e defaults first
+00015860: 2061 7320 6d61 6e79 2072 616e 646f 6d20   as many random 
+00015870: 6172 6520 7365 6e73 656c 6573 730d 0a20  are senseless.. 
+00015880: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
+00015890: 2020 2020 2020 2020 7472 656e 645f 616e          trend_an
+000158a0: 6f6d 616c 795f 696e 7465 7276 656e 7469  omaly_interventi
+000158b0: 6f6e 203d 2072 616e 646f 6d2e 6368 6f69  on = random.choi
+000158c0: 6365 7328 5b4e 6f6e 652c 2027 6465 7465  ces([None, 'dete
+000158d0: 6374 5f6f 6e6c 7927 5d2c 205b 302e 352c  ct_only'], [0.5,
+000158e0: 2030 2e35 5d29 5b0d 0a20 2020 2020 2020   0.5])[..       
+000158f0: 2020 2020 2030 0d0a 2020 2020 2020 2020       0..        
+00015900: 5d0d 0a20 2020 2020 2020 2069 6620 7472  ]..        if tr
+00015910: 656e 645f 616e 6f6d 616c 795f 696e 7465  end_anomaly_inte
+00015920: 7276 656e 7469 6f6e 2069 7320 6e6f 7420  rvention is not 
+00015930: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00015940: 2020 2074 7265 6e64 5f61 6e6f 6d61 6c79     trend_anomaly
+00015950: 5f64 6574 6563 746f 725f 7061 7261 6d73  _detector_params
+00015960: 203d 2041 6e6f 6d61 6c79 5265 6d6f 7661   = AnomalyRemova
+00015970: 6c2e 6765 745f 6e65 775f 7061 7261 6d73  l.get_new_params
+00015980: 286d 6574 686f 643d 6d65 7468 6f64 290d  (method=method).
+00015990: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+000159a0: 2020 2020 2020 2020 2020 2020 7472 656e              tren
+000159b0: 645f 616e 6f6d 616c 795f 6465 7465 6374  d_anomaly_detect
+000159c0: 6f72 5f70 6172 616d 7320 3d20 4e6f 6e65  or_params = None
+000159d0: 0d0a 2020 2020 2020 2020 6c69 6e65 6172  ..        linear
+000159e0: 5f6d 6f64 656c 203d 2072 616e 646f 6d2e  _model = random.
+000159f0: 6368 6f69 6365 7328 0d0a 2020 2020 2020  choices(..      
+00015a00: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
+00015a10: 2020 2020 2020 2020 2027 6c73 7473 7127           'lstsq'
+00015a20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00015a30: 2020 2027 6c69 6e61 6c67 5f73 6f6c 7665     'linalg_solve
+00015a40: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00015a50: 2020 2020 276c 315f 6e6f 726d 272c 0d0a      'l1_norm',..
+00015a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a70: 2764 7761 655f 6e6f 726d 272c 0d0a 2020  'dwae_norm',..  
+00015a80: 2020 2020 2020 2020 2020 2020 2020 2771                'q
+00015a90: 7561 6e74 696c 655f 6e6f 726d 272c 0d0a  uantile_norm',..
+00015aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ab0: 276c 315f 706f 7369 7469 7665 272c 0d0a  'l1_positive',..
+00015ac0: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
+00015ad0: 2020 2020 2020 2020 2020 2020 5b30 2e36              [0.6
+00015ae0: 2c20 302e 322c 2030 2e31 2c20 302e 3035  , 0.2, 0.1, 0.05
+00015af0: 2c20 302e 3032 2c20 302e 3033 5d2c 0d0a  , 0.02, 0.03],..
+00015b00: 2020 2020 2020 2020 295b 305d 0d0a 2020          )[0]..  
+00015b10: 2020 2020 2020 7265 6365 6e63 795f 7765        recency_we
+00015b20: 6967 6874 696e 6720 3d20 7261 6e64 6f6d  ighting = random
+00015b30: 2e63 686f 6963 6573 280d 0a20 2020 2020  .choices(..     
+00015b40: 2020 2020 2020 205b 4e6f 6e65 2c20 302e         [None, 0.
+00015b50: 3035 2c20 302e 312c 2030 2e32 352c 2030  05, 0.1, 0.25, 0
+00015b60: 2e35 5d2c 205b 302e 372c 2030 2e31 2c20  .5], [0.7, 0.1, 
+00015b70: 302e 312c 2030 2e31 2c20 302e 3035 5d0d  0.1, 0.1, 0.05].
+00015b80: 0a20 2020 2020 2020 2029 5b30 5d0d 0a20  .        )[0].. 
+00015b90: 2020 2020 2020 2069 6620 6c69 6e65 6172         if linear
+00015ba0: 5f6d 6f64 656c 2069 6e20 5b27 6c73 7473  _model in ['lsts
+00015bb0: 7127 5d3a 0d0a 2020 2020 2020 2020 2020  q']:..          
+00015bc0: 2020 6c69 6e65 6172 5f6d 6f64 656c 203d    linear_model =
+00015bd0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00015be0: 2020 2020 276d 6f64 656c 273a 206c 696e      'model': lin
+00015bf0: 6561 725f 6d6f 6465 6c2c 0d0a 2020 2020  ear_model,..    
+00015c00: 2020 2020 2020 2020 2020 2020 276c 616d              'lam
+00015c10: 6264 6127 3a20 7261 6e64 6f6d 2e63 686f  bda': random.cho
+00015c20: 6963 6573 280d 0a20 2020 2020 2020 2020  ices(..         
+00015c30: 2020 2020 2020 2020 2020 205b 4e6f 6e65             [None
+00015c40: 2c20 302e 312c 2031 2c20 3130 2c20 3130  , 0.1, 1, 10, 10
+00015c50: 305d 2c20 5b30 2e37 2c20 302e 312c 2030  0], [0.7, 0.1, 0
+00015c60: 2e31 2c20 302e 312c 2030 2e30 355d 0d0a  .1, 0.1, 0.05]..
+00015c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c80: 295b 305d 2c0d 0a20 2020 2020 2020 2020  )[0],..         
+00015c90: 2020 2020 2020 2027 7265 6365 6e63 795f         'recency_
+00015ca0: 7765 6967 6874 696e 6727 3a20 7265 6365  weighting': rece
+00015cb0: 6e63 795f 7765 6967 6874 696e 672c 0d0a  ncy_weighting,..
+00015cc0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
+00015cd0: 2020 2020 2020 2069 6620 6c69 6e65 6172         if linear
+00015ce0: 5f6d 6f64 656c 2069 6e20 5b27 6c69 6e61  _model in ['lina
+00015cf0: 6c67 5f73 6f6c 7665 275d 3a0d 0a20 2020  lg_solve']:..   
+00015d00: 2020 2020 2020 2020 206c 696e 6561 725f           linear_
+00015d10: 6d6f 6465 6c20 3d20 7b0d 0a20 2020 2020  model = {..     
+00015d20: 2020 2020 2020 2020 2020 2027 6d6f 6465             'mode
+00015d30: 6c27 3a20 6c69 6e65 6172 5f6d 6f64 656c  l': linear_model
+00015d40: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00015d50: 2020 2027 6c61 6d62 6461 273a 2072 616e     'lambda': ran
+00015d60: 646f 6d2e 6368 6f69 6365 7328 5b30 2c20  dom.choices([0, 
+00015d70: 302e 312c 2031 2c20 3130 5d2c 205b 302e  0.1, 1, 10], [0.
+00015d80: 342c 2030 2e32 2c20 302e 322c 2030 2e32  4, 0.2, 0.2, 0.2
+00015d90: 5d29 5b30 5d2c 0d0a 2020 2020 2020 2020  ])[0],..        
+00015da0: 2020 2020 2020 2020 2772 6563 656e 6379          'recency
+00015db0: 5f77 6569 6768 7469 6e67 273a 2072 6563  _weighting': rec
+00015dc0: 656e 6379 5f77 6569 6768 7469 6e67 2c0d  ency_weighting,.
+00015dd0: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
+00015de0: 2020 2020 2020 2020 656c 6966 206c 696e          elif lin
+00015df0: 6561 725f 6d6f 6465 6c20 696e 205b 276c  ear_model in ['l
+00015e00: 315f 6e6f 726d 272c 2027 6477 6165 5f6e  1_norm', 'dwae_n
+00015e10: 6f72 6d27 2c20 2771 7561 6e74 696c 655f  orm', 'quantile_
+00015e20: 6e6f 726d 272c 2027 6c31 5f70 6f73 6974  norm', 'l1_posit
+00015e30: 6976 6527 5d3a 0d0a 2020 2020 2020 2020  ive']:..        
+00015e40: 2020 2020 6c69 6e65 6172 5f6d 6f64 656c      linear_model
+00015e50: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
+00015e60: 2020 2020 2020 276d 6f64 656c 273a 206c        'model': l
+00015e70: 696e 6561 725f 6d6f 6465 6c2c 0d0a 2020  inear_model,..  
+00015e80: 2020 2020 2020 2020 2020 2020 2020 2772                'r
+00015e90: 6563 656e 6379 5f77 6569 6768 7469 6e67  ecency_weighting
+00015ea0: 273a 2072 6563 656e 6379 5f77 6569 6768  ': recency_weigh
+00015eb0: 7469 6e67 2c0d 0a20 2020 2020 2020 2020  ting,..         
+00015ec0: 2020 2020 2020 2027 6d61 7869 7465 7227         'maxiter'
+00015ed0: 3a20 7261 6e64 6f6d 2e63 686f 6963 6573  : random.choices
+00015ee0: 285b 3235 302c 2031 3530 3030 2c20 3235  ([250, 15000, 25
+00015ef0: 3030 305d 2c20 5b30 2e32 2c20 302e 362c  000], [0.2, 0.6,
+00015f00: 2030 2e32 5d29 5b30 5d2c 0d0a 2020 2020   0.2])[0],..    
+00015f10: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+00015f20: 2020 2069 6620 6d65 7468 6f64 203d 3d20     if method == 
+00015f30: 2272 6567 7265 7373 6f72 223a 0d0a 2020  "regressor":..  
+00015f40: 2020 2020 2020 2020 2020 7265 6772 6573            regres
+00015f50: 736f 7273 5f75 7365 6420 3d20 5472 7565  sors_used = True
+00015f60: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00015f70: 0a20 2020 2020 2020 2020 2020 2072 6567  .            reg
+00015f80: 7265 7373 6f72 735f 7573 6564 203d 2072  ressors_used = r
+00015f90: 616e 646f 6d2e 6368 6f69 6365 7328 5b54  andom.choices([T
+00015fa0: 7275 652c 2046 616c 7365 5d2c 205b 302e  rue, False], [0.
+00015fb0: 352c 2030 2e35 5d29 5b30 5d0d 0a20 2020  5, 0.5])[0]..   
+00015fc0: 2020 2020 2061 725f 6c61 6773 203d 2072       ar_lags = r
+00015fd0: 616e 646f 6d2e 6368 6f69 6365 7328 0d0a  andom.choices(..
+00015fe0: 2020 2020 2020 2020 2020 2020 5b4e 6f6e              [Non
+00015ff0: 652c 205b 315d 2c20 5b31 2c20 375d 2c20  e, [1], [1, 7], 
+00016000: 5b37 5d2c 205b 7365 6173 6f6e 616c 5f69  [7], [seasonal_i
+00016010: 6e74 2873 6d61 6c6c 3d54 7275 6529 5d5d  nt(small=True)]]
+00016020: 2c0d 0a20 2020 2020 2020 2020 2020 205b  ,..            [
+00016030: 302e 392c 2030 2e30 3235 2c20 302e 3032  0.9, 0.025, 0.02
+00016040: 352c 2030 2e30 352c 2030 2e30 355d 2c0d  5, 0.05, 0.05],.
+00016050: 0a20 2020 2020 2020 2029 5b30 5d0d 0a20  .        )[0].. 
+00016060: 2020 2020 2020 2061 725f 696e 7465 7261         ar_intera
+00016070: 6374 696f 6e5f 7365 6173 6f6e 616c 6974  ction_seasonalit
+00016080: 7920 3d20 4e6f 6e65 0d0a 2020 2020 2020  y = None..      
+00016090: 2020 6966 2061 725f 6c61 6773 2069 7320    if ar_lags is 
+000160a0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+000160b0: 2020 2020 2020 2061 725f 696e 7465 7261         ar_intera
+000160c0: 6374 696f 6e5f 7365 6173 6f6e 616c 6974  ction_seasonalit
+000160d0: 7920 3d20 7261 6e64 6f6d 2e63 686f 6963  y = random.choic
+000160e0: 6573 280d 0a20 2020 2020 2020 2020 2020  es(..           
+000160f0: 2020 2020 205b 4e6f 6e65 2c20 372c 2027       [None, 7, '
+00016100: 6461 796f 6677 6565 6b27 2c20 2763 6f6d  dayofweek', 'com
+00016110: 6d6f 6e5f 666f 7572 6965 7227 5d2c 205b  mon_fourier'], [
+00016120: 302e 342c 2030 2e32 2c20 302e 322c 2030  0.4, 0.2, 0.2, 0
+00016130: 2e32 5d0d 0a20 2020 2020 2020 2020 2020  .2]..           
+00016140: 2029 5b30 5d0d 0a20 2020 2020 2020 2073   )[0]..        s
+00016150: 6561 736f 6e61 6c69 7469 6573 203d 2072  easonalities = r
+00016160: 616e 646f 6d2e 6368 6f69 6365 7328 0d0a  andom.choices(..
+00016170: 2020 2020 2020 2020 2020 2020 5b0d 0a20              [.. 
+00016180: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00016190: 372c 2033 3635 2e32 355d 2c0d 0a20 2020  7, 365.25],..   
+000161a0: 2020 2020 2020 2020 2020 2020 205b 2264               ["d
+000161b0: 6179 6f66 7765 656b 222c 2033 3635 2e32  ayofweek", 365.2
+000161c0: 355d 2c0d 0a20 2020 2020 2020 2020 2020  5],..           
+000161d0: 2020 2020 205b 226d 6f6e 7468 222c 2022       ["month", "
+000161e0: 6461 796f 6677 6565 6b22 2c20 2277 6565  dayofweek", "wee
+000161f0: 6b64 6179 6f66 6d6f 6e74 6822 5d2c 0d0a  kdayofmonth"],..
+00016200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016210: 5b27 7765 656b 6461 796f 666d 6f6e 7468  ['weekdayofmonth
+00016220: 272c 2027 636f 6d6d 6f6e 5f66 6f75 7269  ', 'common_fouri
+00016230: 6572 275d 2c0d 0a20 2020 2020 2020 2020  er'],..         
+00016240: 2020 2020 2020 2022 6f74 6865 7222 2c0d         "other",.
+00016250: 0a20 2020 2020 2020 2020 2020 205d 2c0d  .            ],.
+00016260: 0a20 2020 2020 2020 2020 2020 205b 302e  .            [0.
+00016270: 312c 2030 2e31 2c20 302e 312c 2030 2e30  1, 0.1, 0.1, 0.0
+00016280: 352c 2030 2e31 5d2c 0d0a 2020 2020 2020  5, 0.1],..      
+00016290: 2020 295b 305d 0d0a 2020 2020 2020 2020    )[0]..        
+000162a0: 6966 2073 6561 736f 6e61 6c69 7469 6573  if seasonalities
+000162b0: 203d 3d20 226f 7468 6572 223a 0d0a 2020   == "other":..  
+000162c0: 2020 2020 2020 2020 2020 7072 6564 6566            predef
+000162d0: 696e 6564 203d 2072 616e 646f 6d2e 6368  ined = random.ch
+000162e0: 6f69 6365 7328 5b54 7275 652c 2046 616c  oices([True, Fal
+000162f0: 7365 5d2c 205b 302e 352c 2030 2e35 5d29  se], [0.5, 0.5])
+00016300: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+00016310: 2069 6620 7072 6564 6566 696e 6564 3a0d   if predefined:.
+00016320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016330: 2073 6561 736f 6e61 6c69 7469 6573 203d   seasonalities =
+00016340: 2072 616e 646f 6d2e 6368 6f69 6365 2864   random.choice(d
+00016350: 6174 655f 7061 7274 5f6d 6574 686f 6473  ate_part_methods
+00016360: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00016370: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00016380: 2020 2020 2020 636f 6d70 5f6f 7074 7320        comp_opts 
+00016390: 3d20 6461 7465 7061 7274 5f63 6f6d 706f  = datepart_compo
+000163a0: 6e65 6e74 7320 2b20 5b37 2c20 3336 352e  nents + [7, 365.
+000163b0: 3235 2c20 3132 5d0d 0a20 2020 2020 2020  25, 12]..       
+000163c0: 2020 2020 2020 2020 2073 6561 736f 6e61           seasona
+000163d0: 6c69 7469 6573 203d 2072 616e 646f 6d2e  lities = random.
+000163e0: 6368 6f69 6365 7328 636f 6d70 5f6f 7074  choices(comp_opt
+000163f0: 732c 206b 3d32 290d 0a20 2020 2020 2020  s, k=2)..       
+00016400: 2072 6574 7572 6e20 7b0d 0a20 2020 2020   return {..     
+00016410: 2020 2020 2020 2022 7072 6570 726f 6365         "preproce
+00016420: 7373 696e 675f 7472 616e 7366 6f72 6d61  ssing_transforma
+00016430: 7469 6f6e 223a 2052 616e 646f 6d54 7261  tion": RandomTra
+00016440: 6e73 666f 726d 280d 0a20 2020 2020 2020  nsform(..       
+00016450: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
+00016460: 726d 6572 5f6c 6973 743d 6669 6c74 6572  rmer_list=filter
+00016470: 732c 2074 7261 6e73 666f 726d 6572 5f6d  s, transformer_m
+00016480: 6178 5f64 6570 7468 3d32 2c20 616c 6c6f  ax_depth=2, allo
+00016490: 775f 6e6f 6e65 3d54 7275 650d 0a20 2020  w_none=True..   
+000164a0: 2020 2020 2020 2020 2029 2c0d 0a20 2020           ),..   
+000164b0: 2020 2020 2020 2020 2022 7363 616c 696e           "scalin
+000164c0: 6722 3a20 7363 616c 696e 672c 0d0a 2020  g": scaling,..  
+000164d0: 2020 2020 2020 2020 2020 2320 2270 6173            # "pas
+000164e0: 745f 696d 7061 6374 735f 696e 7465 7276  t_impacts_interv
+000164f0: 656e 7469 6f6e 223a 2073 656c 662e 7061  ention": self.pa
+00016500: 7374 5f69 6d70 6163 7473 5f69 6e74 6572  st_impacts_inter
+00016510: 7665 6e74 696f 6e2c 0d0a 2020 2020 2020  vention,..      
+00016520: 2020 2020 2020 2273 6561 736f 6e61 6c69        "seasonali
+00016530: 7469 6573 223a 2073 6561 736f 6e61 6c69  ties": seasonali
+00016540: 7469 6573 2c0d 0a20 2020 2020 2020 2020  ties,..         
+00016550: 2020 2022 6172 5f6c 6167 7322 3a20 6172     "ar_lags": ar
+00016560: 5f6c 6167 732c 0d0a 2020 2020 2020 2020  _lags,..        
+00016570: 2020 2020 2261 725f 696e 7465 7261 6374      "ar_interact
+00016580: 696f 6e5f 7365 6173 6f6e 616c 6974 7922  ion_seasonality"
+00016590: 3a20 6172 5f69 6e74 6572 6163 7469 6f6e  : ar_interaction
+000165a0: 5f73 6561 736f 6e61 6c69 7479 2c0d 0a20  _seasonality,.. 
+000165b0: 2020 2020 2020 2020 2020 2022 616e 6f6d             "anom
+000165c0: 616c 795f 6465 7465 6374 6f72 5f70 6172  aly_detector_par
+000165d0: 616d 7322 3a20 616e 6f6d 616c 795f 6465  ams": anomaly_de
+000165e0: 7465 6374 6f72 5f70 6172 616d 732c 0d0a  tector_params,..
+000165f0: 2020 2020 2020 2020 2020 2020 2261 6e6f              "ano
+00016600: 6d61 6c79 5f69 6e74 6572 7665 6e74 696f  maly_interventio
+00016610: 6e22 3a20 616e 6f6d 616c 795f 696e 7465  n": anomaly_inte
+00016620: 7276 656e 7469 6f6e 2c0d 0a20 2020 2020  rvention,..     
+00016630: 2020 2020 2020 2022 686f 6c69 6461 795f         "holiday_
+00016640: 6465 7465 6374 6f72 5f70 6172 616d 7322  detector_params"
+00016650: 3a20 686f 6c69 6461 795f 7061 7261 6d73  : holiday_params
+00016660: 2c0d 0a20 2020 2020 2020 2020 2020 2023  ,..            #
+00016670: 2022 686f 6c69 6461 795f 636f 756e 7472   "holiday_countr
+00016680: 6965 7322 3a20 7365 6c66 2e68 6f6c 6964  ies": self.holid
+00016690: 6179 5f63 6f75 6e74 7269 6573 2c0d 0a20  ay_countries,.. 
+000166a0: 2020 2020 2020 2020 2020 2022 686f 6c69             "holi
+000166b0: 6461 795f 636f 756e 7472 6965 735f 7573  day_countries_us
+000166c0: 6564 223a 2072 616e 646f 6d2e 6368 6f69  ed": random.choi
+000166d0: 6365 7328 5b54 7275 652c 2046 616c 7365  ces([True, False
+000166e0: 5d2c 205b 302e 352c 2030 2e35 5d29 5b30  ], [0.5, 0.5])[0
+000166f0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00016700: 226d 756c 7469 7661 7269 6174 655f 6665  "multivariate_fe
+00016710: 6174 7572 6522 3a20 7261 6e64 6f6d 2e63  ature": random.c
+00016720: 686f 6963 6573 280d 0a20 2020 2020 2020  hoices(..       
+00016730: 2020 2020 2020 2020 205b 4e6f 6e65 2c20           [None, 
+00016740: 2266 6561 7475 7265 5f61 6767 6c6f 6d65  "feature_agglome
+00016750: 7261 7469 6f6e 222c 2027 6772 6f75 705f  ration", 'group_
+00016760: 6176 6572 6167 6527 2c20 276f 7363 696c  average', 'oscil
+00016770: 6c61 746f 7227 5d2c 0d0a 2020 2020 2020  lator'],..      
+00016780: 2020 2020 2020 2020 2020 5b30 2e39 2c20            [0.9, 
+00016790: 302e 312c 2030 2e31 2c20 302e 305d 2c0d  0.1, 0.1, 0.0],.
+000167a0: 0a20 2020 2020 2020 2020 2020 2029 5b30  .            )[0
+000167b0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+000167c0: 226d 756c 7469 7661 7269 6174 655f 7472  "multivariate_tr
+000167d0: 616e 7366 6f72 6d61 7469 6f6e 223a 2052  ansformation": R
+000167e0: 616e 646f 6d54 7261 6e73 666f 726d 280d  andomTransform(.
+000167f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016800: 2074 7261 6e73 666f 726d 6572 5f6c 6973   transformer_lis
+00016810: 743d 2266 6173 7422 2c0d 0a20 2020 2020  t="fast",..     
+00016820: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
+00016830: 666f 726d 6572 5f6d 6178 5f64 6570 7468  former_max_depth
+00016840: 3d33 2c20 2023 2070 726f 6261 626c 7920  =3,  # probably 
+00016850: 7761 6e74 2073 6f6d 6520 6d6f 7265 2075  want some more u
+00016860: 7361 626c 6520 6465 6661 756c 7473 2066  sable defaults f
+00016870: 6972 7374 2061 7320 6d61 6e79 2072 616e  irst as many ran
+00016880: 646f 6d20 6172 6520 7365 6e73 656c 6573  dom are senseles
+00016890: 730d 0a20 2020 2020 2020 2020 2020 2029  s..            )
+000168a0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+000168b0: 7265 6772 6573 736f 725f 7472 616e 7366  regressor_transf
+000168c0: 6f72 6d61 7469 6f6e 223a 2052 616e 646f  ormation": Rando
+000168d0: 6d54 7261 6e73 666f 726d 280d 0a20 2020  mTransform(..   
+000168e0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+000168f0: 6e73 666f 726d 6572 5f6c 6973 743d 7b2a  nsformer_list={*
+00016900: 2a73 6361 6c65 7273 2c20 2a2a 6465 636f  *scalers, **deco
+00016910: 6d70 6f73 6974 696f 6e73 7d2c 0d0a 2020  mpositions},..  
+00016920: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00016930: 616e 7366 6f72 6d65 725f 6d61 785f 6465  ansformer_max_de
+00016940: 7074 683d 312c 0d0a 2020 2020 2020 2020  pth=1,..        
+00016950: 2020 2020 2020 2020 616c 6c6f 775f 6e6f          allow_no
+00016960: 6e65 3d46 616c 7365 2c0d 0a20 2020 2020  ne=False,..     
+00016970: 2020 2020 2020 2020 2020 206e 6f5f 6e61             no_na
+00016980: 6e5f 6669 6c6c 3d46 616c 7365 2c20 2023  n_fill=False,  #
+00016990: 2070 726f 6261 626c 7920 7761 6e74 2073   probably want s
+000169a0: 6f6d 6520 6d6f 7265 2075 7361 626c 6520  ome more usable 
+000169b0: 6465 6661 756c 7473 2066 6972 7374 2061  defaults first a
+000169c0: 7320 6d61 6e79 2072 616e 646f 6d20 6172  s many random ar
+000169d0: 6520 7365 6e73 656c 6573 730d 0a20 2020  e senseless..   
+000169e0: 2020 2020 2020 2020 2029 2c0d 0a20 2020           ),..   
+000169f0: 2020 2020 2020 2020 2022 7265 6772 6573           "regres
+00016a00: 736f 7273 5f75 7365 6422 3a20 7265 6772  sors_used": regr
+00016a10: 6573 736f 7273 5f75 7365 642c 0d0a 2020  essors_used,..  
+00016a20: 2020 2020 2020 2020 2020 226c 696e 6561            "linea
+00016a30: 725f 6d6f 6465 6c22 3a20 6c69 6e65 6172  r_model": linear
+00016a40: 5f6d 6f64 656c 2c0d 0a20 2020 2020 2020  _model,..       
+00016a50: 2020 2020 2022 7261 6e64 6f6d 7761 6c6b       "randomwalk
+00016a60: 5f6e 223a 2072 616e 646f 6d2e 6368 6f69  _n": random.choi
+00016a70: 6365 7328 5b4e 6f6e 652c 2031 305d 2c20  ces([None, 10], 
+00016a80: 5b30 2e35 2c20 302e 355d 295b 305d 2c0d  [0.5, 0.5])[0],.
+00016a90: 0a20 2020 2020 2020 2020 2020 2022 7472  .            "tr
+00016aa0: 656e 645f 7769 6e64 6f77 223a 2072 616e  end_window": ran
+00016ab0: 646f 6d2e 6368 6f69 6365 7328 5b33 2c20  dom.choices([3, 
+00016ac0: 3135 2c20 3930 2c20 3336 355d 2c20 5b30  15, 90, 365], [0
+00016ad0: 2e32 2c20 302e 322c 2030 2e32 2c20 302e  .2, 0.2, 0.2, 0.
+00016ae0: 325d 295b 305d 2c0d 0a20 2020 2020 2020  2])[0],..       
+00016af0: 2020 2020 2022 7472 656e 645f 7374 616e       "trend_stan
+00016b00: 6469 6e22 3a20 7261 6e64 6f6d 2e63 686f  din": random.cho
+00016b10: 6963 6573 280d 0a20 2020 2020 2020 2020  ices(..         
+00016b20: 2020 2020 2020 205b 4e6f 6e65 2c20 2772         [None, 'r
+00016b30: 616e 646f 6d5f 6e6f 726d 616c 272c 2027  andom_normal', '
+00016b40: 726f 6c6c 696e 675f 7472 656e 6427 5d2c  rolling_trend'],
+00016b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016b60: 2020 5b30 2e35 2c20 302e 342c 2030 2e31    [0.5, 0.4, 0.1
+00016b70: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00016b80: 295b 305d 2c0d 0a20 2020 2020 2020 2020  )[0],..         
+00016b90: 2020 2022 7472 656e 645f 616e 6f6d 616c     "trend_anomal
+00016ba0: 795f 6465 7465 6374 6f72 5f70 6172 616d  y_detector_param
+00016bb0: 7322 3a20 7472 656e 645f 616e 6f6d 616c  s": trend_anomal
+00016bc0: 795f 6465 7465 6374 6f72 5f70 6172 616d  y_detector_param
+00016bd0: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+00016be0: 2320 2274 7265 6e64 5f61 6e6f 6d61 6c79  # "trend_anomaly
+00016bf0: 5f69 6e74 6572 7665 6e74 696f 6e22 3a20  _intervention": 
+00016c00: 7472 656e 645f 616e 6f6d 616c 795f 696e  trend_anomaly_in
+00016c10: 7465 7276 656e 7469 6f6e 2c0d 0a20 2020  tervention,..   
+00016c20: 2020 2020 2020 2020 2022 7472 656e 645f           "trend_
+00016c30: 7472 616e 7366 6f72 6d61 7469 6f6e 223a  transformation":
+00016c40: 2074 7265 6e64 5f74 7261 6e73 666f 726d   trend_transform
+00016c50: 6174 696f 6e2c 0d0a 2020 2020 2020 2020  ation,..        
+00016c60: 2020 2020 2274 7265 6e64 5f6d 6f64 656c      "trend_model
+00016c70: 223a 2074 7265 6e64 5f6d 6f64 656c 2c0d  ": trend_model,.
+00016c80: 0a20 2020 2020 2020 2020 2020 2022 7472  .            "tr
+00016c90: 656e 645f 7068 6922 3a20 7261 6e64 6f6d  end_phi": random
+00016ca0: 2e63 686f 6963 6573 285b 4e6f 6e65 2c20  .choices([None, 
+00016cb0: 302e 3938 5d2c 205b 302e 392c 2030 2e31  0.98], [0.9, 0.1
+00016cc0: 5d29 5b30 5d2c 0d0a 2020 2020 2020 2020  ])[0],..        
+00016cd0: 7d0d 0a0d 0a20 2020 2064 6566 2067 6574  }....    def get
+00016ce0: 5f70 6172 616d 7328 7365 6c66 293a 0d0a  _params(self):..
+00016cf0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+00016d00: 0d0a 2020 2020 2020 2020 2020 2020 2270  ..            "p
+00016d10: 7265 7072 6f63 6573 7369 6e67 5f74 7261  reprocessing_tra
+00016d20: 6e73 666f 726d 6174 696f 6e22 3a20 7365  nsformation": se
+00016d30: 6c66 2e70 7265 7072 6f63 6573 7369 6e67  lf.preprocessing
+00016d40: 5f74 7261 6e73 666f 726d 6174 696f 6e2c  _transformation,
+00016d50: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
+00016d60: 6361 6c69 6e67 223a 2073 656c 662e 7363  caling": self.sc
+00016d70: 616c 696e 672c 0d0a 2020 2020 2020 2020  aling,..        
+00016d80: 2020 2020 2270 6173 745f 696d 7061 6374      "past_impact
+00016d90: 735f 696e 7465 7276 656e 7469 6f6e 223a  s_intervention":
+00016da0: 2073 656c 662e 7061 7374 5f69 6d70 6163   self.past_impac
+00016db0: 7473 5f69 6e74 6572 7665 6e74 696f 6e2c  ts_intervention,
+00016dc0: 2020 2320 6e6f 7420 696e 206e 6577 0d0a    # not in new..
+00016dd0: 2020 2020 2020 2020 2020 2020 2273 6561              "sea
+00016de0: 736f 6e61 6c69 7469 6573 223a 2073 656c  sonalities": sel
+00016df0: 662e 7365 6173 6f6e 616c 6974 6965 732c  f.seasonalities,
+00016e00: 0d0a 2020 2020 2020 2020 2020 2020 2261  ..            "a
+00016e10: 725f 6c61 6773 223a 2073 656c 662e 6172  r_lags": self.ar
+00016e20: 5f6c 6167 732c 0d0a 2020 2020 2020 2020  _lags,..        
+00016e30: 2020 2020 2261 725f 696e 7465 7261 6374      "ar_interact
+00016e40: 696f 6e5f 7365 6173 6f6e 616c 6974 7922  ion_seasonality"
+00016e50: 3a20 7365 6c66 2e61 725f 696e 7465 7261  : self.ar_intera
+00016e60: 6374 696f 6e5f 7365 6173 6f6e 616c 6974  ction_seasonalit
+00016e70: 790d 0a20 2020 2020 2020 2020 2020 2069  y..            i
+00016e80: 6620 7365 6c66 2e61 725f 6c61 6773 2069  f self.ar_lags i
+00016e90: 7320 6e6f 7420 4e6f 6e65 0d0a 2020 2020  s not None..    
+00016ea0: 2020 2020 2020 2020 656c 7365 204e 6f6e          else Non
+00016eb0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00016ec0: 2261 6e6f 6d61 6c79 5f64 6574 6563 746f  "anomaly_detecto
+00016ed0: 725f 7061 7261 6d73 223a 2073 656c 662e  r_params": self.
+00016ee0: 616e 6f6d 616c 795f 6465 7465 6374 6f72  anomaly_detector
+00016ef0: 5f70 6172 616d 732c 0d0a 2020 2020 2020  _params,..      
+00016f00: 2020 2020 2020 2261 6e6f 6d61 6c79 5f69        "anomaly_i
+00016f10: 6e74 6572 7665 6e74 696f 6e22 3a20 7365  ntervention": se
+00016f20: 6c66 2e61 6e6f 6d61 6c79 5f69 6e74 6572  lf.anomaly_inter
+00016f30: 7665 6e74 696f 6e2c 0d0a 2020 2020 2020  vention,..      
+00016f40: 2020 2020 2020 2268 6f6c 6964 6179 5f64        "holiday_d
+00016f50: 6574 6563 746f 725f 7061 7261 6d73 223a  etector_params":
+00016f60: 2073 656c 662e 686f 6c69 6461 795f 6465   self.holiday_de
+00016f70: 7465 6374 6f72 5f70 6172 616d 732c 0d0a  tector_params,..
+00016f80: 2020 2020 2020 2020 2020 2020 2320 2268              # "h
+00016f90: 6f6c 6964 6179 5f69 6e74 6572 7665 6e74  oliday_intervent
+00016fa0: 696f 6e22 3a20 7365 6c66 2e68 6f6c 6964  ion": self.holid
+00016fb0: 6179 5f69 6e74 6572 7665 6e74 696f 6e2c  ay_intervention,
+00016fc0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00016fd0: 2268 6f6c 6964 6179 5f63 6f75 6e74 7269  "holiday_countri
+00016fe0: 6573 223a 2073 656c 662e 686f 6c69 6461  es": self.holida
+00016ff0: 795f 636f 756e 7472 6965 732c 0d0a 2020  y_countries,..  
+00017000: 2020 2020 2020 2020 2020 2268 6f6c 6964            "holid
+00017010: 6179 5f63 6f75 6e74 7269 6573 5f75 7365  ay_countries_use
+00017020: 6422 3a20 7365 6c66 2e68 6f6c 6964 6179  d": self.holiday
+00017030: 5f63 6f75 6e74 7269 6573 5f75 7365 642c  _countries_used,
+00017040: 0d0a 2020 2020 2020 2020 2020 2020 226d  ..            "m
+00017050: 756c 7469 7661 7269 6174 655f 6665 6174  ultivariate_feat
+00017060: 7572 6522 3a20 7365 6c66 2e6d 756c 7469  ure": self.multi
+00017070: 7661 7269 6174 655f 6665 6174 7572 652c  variate_feature,
+00017080: 0d0a 2020 2020 2020 2020 2020 2020 226d  ..            "m
+00017090: 756c 7469 7661 7269 6174 655f 7472 616e  ultivariate_tran
+000170a0: 7366 6f72 6d61 7469 6f6e 223a 2073 656c  sformation": sel
+000170b0: 662e 6d75 6c74 6976 6172 6961 7465 5f74  f.multivariate_t
+000170c0: 7261 6e73 666f 726d 6174 696f 6e0d 0a20  ransformation.. 
+000170d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000170e0: 6c66 2e6d 756c 7469 7661 7269 6174 655f  lf.multivariate_
+000170f0: 6665 6174 7572 6520 6973 206e 6f74 204e  feature is not N
+00017100: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
+00017110: 2065 6c73 6520 4e6f 6e65 2c0d 0a20 2020   else None,..   
+00017120: 2020 2020 2020 2020 2022 7265 6772 6573           "regres
+00017130: 736f 725f 7472 616e 7366 6f72 6d61 7469  sor_transformati
+00017140: 6f6e 223a 2073 656c 662e 7265 6772 6573  on": self.regres
+00017150: 736f 725f 7472 616e 7366 6f72 6d61 7469  sor_transformati
+00017160: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00017170: 6966 2073 656c 662e 7265 6772 6573 736f  if self.regresso
+00017180: 7273 5f75 7365 640d 0a20 2020 2020 2020  rs_used..       
+00017190: 2020 2020 2065 6c73 6520 4e6f 6e65 2c0d       else None,.
+000171a0: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+000171b0: 6772 6573 736f 7273 5f75 7365 6422 3a20  gressors_used": 
+000171c0: 7365 6c66 2e72 6567 7265 7373 6f72 735f  self.regressors_
+000171d0: 7573 6564 2c0d 0a20 2020 2020 2020 2020  used,..         
+000171e0: 2020 2022 6c69 6e65 6172 5f6d 6f64 656c     "linear_model
+000171f0: 223a 2073 656c 662e 6c69 6e65 6172 5f6d  ": self.linear_m
+00017200: 6f64 656c 2c0d 0a20 2020 2020 2020 2020  odel,..         
+00017210: 2020 2022 7261 6e64 6f6d 7761 6c6b 5f6e     "randomwalk_n
+00017220: 223a 2073 656c 662e 7261 6e64 6f6d 7761  ": self.randomwa
+00017230: 6c6b 5f6e 2c0d 0a20 2020 2020 2020 2020  lk_n,..         
+00017240: 2020 2022 7472 656e 645f 7769 6e64 6f77     "trend_window
+00017250: 223a 2073 656c 662e 7472 656e 645f 7769  ": self.trend_wi
+00017260: 6e64 6f77 2c0d 0a20 2020 2020 2020 2020  ndow,..         
+00017270: 2020 2022 7472 656e 645f 7374 616e 6469     "trend_standi
+00017280: 6e22 3a20 7365 6c66 2e74 7265 6e64 5f73  n": self.trend_s
+00017290: 7461 6e64 696e 2c0d 0a20 2020 2020 2020  tandin,..       
+000172a0: 2020 2020 2022 7472 656e 645f 616e 6f6d       "trend_anom
+000172b0: 616c 795f 6465 7465 6374 6f72 5f70 6172  aly_detector_par
+000172c0: 616d 7322 3a20 7365 6c66 2e74 7265 6e64  ams": self.trend
+000172d0: 5f61 6e6f 6d61 6c79 5f64 6574 6563 746f  _anomaly_detecto
+000172e0: 725f 7061 7261 6d73 2c0d 0a20 2020 2020  r_params,..     
+000172f0: 2020 2020 2020 2023 2022 7472 656e 645f         # "trend_
+00017300: 616e 6f6d 616c 795f 696e 7465 7276 656e  anomaly_interven
+00017310: 7469 6f6e 223a 2073 656c 662e 7472 656e  tion": self.tren
+00017320: 645f 616e 6f6d 616c 795f 696e 7465 7276  d_anomaly_interv
+00017330: 656e 7469 6f6e 2c0d 0a20 2020 2020 2020  ention,..       
+00017340: 2020 2020 2022 7472 656e 645f 7472 616e       "trend_tran
+00017350: 7366 6f72 6d61 7469 6f6e 223a 2073 656c  sformation": sel
+00017360: 662e 7472 656e 645f 7472 616e 7366 6f72  f.trend_transfor
+00017370: 6d61 7469 6f6e 2c0d 0a20 2020 2020 2020  mation,..       
+00017380: 2020 2020 2022 7472 656e 645f 6d6f 6465       "trend_mode
+00017390: 6c22 3a20 7365 6c66 2e74 7265 6e64 5f6d  l": self.trend_m
+000173a0: 6f64 656c 2c0d 0a20 2020 2020 2020 2020  odel,..         
+000173b0: 2020 2022 7472 656e 645f 7068 6922 3a20     "trend_phi": 
+000173c0: 7365 6c66 2e74 7265 6e64 5f70 6869 2c0d  self.trend_phi,.
+000173d0: 0a20 2020 2020 2020 2020 2020 2023 2022  .            # "
+000173e0: 636f 6e73 7472 6169 6e74 223a 2073 656c  constraint": sel
+000173f0: 662e 636f 6e73 7472 6169 6e74 2c0d 0a20  f.constraint,.. 
+00017400: 2020 2020 2020 207d 0d0a 0d0a 2020 2020         }....    
+00017410: 6465 6620 706c 6f74 5f63 6f6d 706f 6e65  def plot_compone
+00017420: 6e74 7328 0d0a 2020 2020 2020 2020 7365  nts(..        se
+00017430: 6c66 2c0d 0a20 2020 2020 2020 2070 7265  lf,..        pre
+00017440: 6469 6374 696f 6e3d 4e6f 6e65 2c0d 0a20  diction=None,.. 
+00017450: 2020 2020 2020 2073 6572 6965 733d 4e6f         series=No
+00017460: 6e65 2c0d 0a20 2020 2020 2020 2066 6967  ne,..        fig
+00017470: 7369 7a65 3d28 3136 2c20 3929 2c0d 0a20  size=(16, 9),.. 
+00017480: 2020 2020 2020 2074 6f5f 6f72 6967 696e         to_origin
+00017490: 5f73 7061 6365 3d54 7275 652c 0d0a 2020  _space=True,..  
+000174a0: 2020 2020 2020 7469 746c 653d 4e6f 6e65        title=None
+000174b0: 2c0d 0a20 2020 2020 2020 2073 7461 7274  ,..        start
+000174c0: 5f64 6174 653d 4e6f 6e65 2c0d 0a20 2020  _date=None,..   
+000174d0: 2029 3a0d 0a20 2020 2020 2020 2069 6620   ):..        if 
+000174e0: 7365 7269 6573 2069 7320 4e6f 6e65 3a0d  series is None:.
+000174f0: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
+00017500: 6965 7320 3d20 7261 6e64 6f6d 2e63 686f  ies = random.cho
+00017510: 6963 6528 7365 6c66 2e63 6f6c 756d 6e5f  ice(self.column_
+00017520: 6e61 6d65 7329 0d0a 2020 2020 2020 2020  names)..        
+00017530: 6966 2074 6974 6c65 2069 7320 4e6f 6e65  if title is None
+00017540: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+00017550: 6974 6c65 203d 2066 224d 6f64 656c 2043  itle = f"Model C
+00017560: 6f6d 706f 6e65 6e74 7320 666f 7220 7b73  omponents for {s
+00017570: 6572 6965 737d 220d 0a20 2020 2020 2020  eries}"..       
+00017580: 2070 6c6f 745f 6c69 7374 203d 205b 5d0d   plot_list = [].
+00017590: 0a20 2020 2020 2020 2069 6620 7072 6564  .        if pred
+000175a0: 6963 7469 6f6e 2069 7320 6e6f 7420 4e6f  iction is not No
+000175b0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+000175c0: 2070 6c6f 745f 6c69 7374 2e61 7070 656e   plot_list.appen
+000175d0: 6428 7072 6564 6963 7469 6f6e 2e66 6f72  d(prediction.for
+000175e0: 6563 6173 745b 7365 7269 6573 5d2e 7265  ecast[series].re
+000175f0: 6e61 6d65 2822 666f 7265 6361 7374 2229  name("forecast")
+00017600: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+00017610: 6c74 5f69 6478 203d 2070 7265 6469 6374  lt_idx = predict
+00017620: 696f 6e2e 666f 7265 6361 7374 2e69 6e64  ion.forecast.ind
+00017630: 6578 0d0a 2020 2020 2020 2020 656c 7365  ex..        else
+00017640: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00017650: 6c74 5f69 6478 203d 204e 6f6e 650d 0a20  lt_idx = None.. 
+00017660: 2020 2020 2020 2070 6c6f 745f 6c69 7374         plot_list
+00017670: 2e61 7070 656e 6428 7365 6c66 2e70 7265  .append(self.pre
+00017680: 6469 6374 6564 5f74 7265 6e64 5b73 6572  dicted_trend[ser
+00017690: 6965 735d 2e72 656e 616d 6528 2274 7265  ies].rename("tre
+000176a0: 6e64 2229 290d 0a20 2020 2020 2020 2069  nd"))..        i
+000176b0: 6620 7365 6c66 2e69 6d70 6163 7473 2069  f self.impacts i
+000176c0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+000176d0: 2020 2020 2020 2020 2070 6c6f 745f 6c69           plot_li
+000176e0: 7374 2e61 7070 656e 6428 2873 656c 662e  st.append((self.
+000176f0: 696d 7061 6374 735b 7365 7269 6573 5d2e  impacts[series].
+00017700: 7265 6e61 6d65 2822 696d 7061 6374 2025  rename("impact %
+00017710: 2229 202d 2031 2e30 2920 2a20 3130 3029  ") - 1.0) * 100)
+00017720: 0d0a 2020 2020 2020 2020 6966 2070 6c74  ..        if plt
+00017730: 5f69 6478 2069 7320 4e6f 6e65 3a0d 0a20  _idx is None:.. 
+00017740: 2020 2020 2020 2020 2020 2070 6c6f 745f             plot_
+00017750: 6c69 7374 2e61 7070 656e 6428 0d0a 2020  list.append(..  
+00017760: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017770: 6c66 2e70 726f 6365 7373 5f63 6f6d 706f  lf.process_compo
+00017780: 6e65 6e74 7328 746f 5f6f 7269 6769 6e5f  nents(to_origin_
+00017790: 7370 6163 653d 746f 5f6f 7269 6769 6e5f  space=to_origin_
+000177a0: 7370 6163 6529 5b73 6572 6965 735d 0d0a  space)[series]..
+000177b0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+000177c0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000177d0: 2020 2020 2020 2020 2020 706c 6f74 5f6c            plot_l
+000177e0: 6973 742e 6170 7065 6e64 280d 0a20 2020  ist.append(..   
+000177f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017800: 662e 7072 6f63 6573 735f 636f 6d70 6f6e  f.process_compon
+00017810: 656e 7473 2874 6f5f 6f72 6967 696e 5f73  ents(to_origin_s
+00017820: 7061 6365 3d74 6f5f 6f72 6967 696e 5f73  pace=to_origin_s
+00017830: 7061 6365 295b 7365 7269 6573 5d2e 6c6f  pace)[series].lo
+00017840: 635b 0d0a 2020 2020 2020 2020 2020 2020  c[..            
+00017850: 2020 2020 2020 2020 706c 745f 6964 780d          plt_idx.
+00017860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017870: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
+00017880: 290d 0a20 2020 2020 2020 2070 6c6f 745f  )..        plot_
+00017890: 6466 203d 2070 642e 636f 6e63 6174 2870  df = pd.concat(p
+000178a0: 6c6f 745f 6c69 7374 2c20 6178 6973 3d31  lot_list, axis=1
+000178b0: 290d 0a20 2020 2020 2020 2069 6620 7374  )..        if st
+000178c0: 6172 745f 6461 7465 2069 7320 6e6f 7420  art_date is not 
+000178d0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000178e0: 2020 2069 6620 7374 6172 745f 6461 7465     if start_date
+000178f0: 203d 3d20 2261 7574 6f22 3a0d 0a20 2020   == "auto":..   
+00017900: 2020 2020 2020 2020 2020 2020 2070 6c6f               plo
+00017910: 745f 6466 203d 2070 6c6f 745f 6466 2e69  t_df = plot_df.i
+00017920: 6c6f 635b 2d28 7072 6564 6963 7469 6f6e  loc[-(prediction
+00017930: 2e66 6f72 6563 6173 745f 6c65 6e67 7468  .forecast_length
+00017940: 202a 2033 2920 3a5d 0d0a 2020 2020 2020   * 3) :]..      
+00017950: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00017960: 2020 2020 2020 2020 2020 2020 2070 6c6f               plo
+00017970: 745f 6466 203d 2070 6c6f 745f 6466 5b70  t_df = plot_df[p
+00017980: 6c6f 745f 6466 2e69 6e64 6578 203e 3d20  lot_df.index >= 
+00017990: 7374 6172 745f 6461 7465 5d0d 0a20 2020  start_date]..   
+000179a0: 2020 2020 2072 6574 7572 6e20 706c 6f74       return plot
+000179b0: 5f64 662e 706c 6f74 2873 7562 706c 6f74  _df.plot(subplot
+000179c0: 733d 5472 7565 2c20 6669 6773 697a 653d  s=True, figsize=
+000179d0: 6669 6773 697a 652c 2074 6974 6c65 3d74  figsize, title=t
+000179e0: 6974 6c65 290d 0a0d 0a20 2020 2064 6566  itle)....    def
+000179f0: 2072 6574 7572 6e5f 636f 6d70 6f6e 656e   return_componen
+00017a00: 7473 2873 656c 662c 2074 6f5f 6f72 6967  ts(self, to_orig
+00017a10: 696e 5f73 7061 6365 3d54 7275 652c 2069  in_space=True, i
+00017a20: 6e63 6c75 6465 5f69 6d70 6163 7473 3d46  nclude_impacts=F
+00017a30: 616c 7365 293a 0d0a 2020 2020 2020 2020  alse):..        
+00017a40: 2222 2252 6574 7572 6e20 6164 6469 7469  """Return additi
+00017a50: 7665 2065 6c65 6d65 6e74 7320 6f66 2066  ve elements of f
+00017a60: 6f72 6563 6173 742c 206c 696e 6561 7220  orecast, linear 
+00017a70: 616e 6420 7472 656e 642e 2049 6620 696d  and trend. If im
+00017a80: 7061 6374 7320 696e 636c 7564 6564 2c20  pacts included, 
+00017a90: 6974 2069 7320 6120 6d75 6c74 6970 6c69  it is a multipli
+00017aa0: 6361 7469 7665 2074 6572 6d2e 0d0a 0d0a  cative term.....
+00017ab0: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
+00017ac0: 2020 2020 2020 2020 2020 2074 6f5f 6f72             to_or
+00017ad0: 6967 696e 5f73 7061 6365 2028 626f 6f6c  igin_space (bool
+00017ae0: 2920 6966 2046 616c 7365 2c20 7769 6c6c  ) if False, will
+00017af0: 206e 6f74 2072 6576 6572 7365 2074 7261   not reverse tra
+00017b00: 6e73 666f 726d 206c 696e 6561 7220 636f  nsform linear co
+00017b10: 6d70 6f6e 656e 7473 0d0a 2020 2020 2020  mponents..      
+00017b20: 2020 2020 2020 696e 636c 7564 655f 696d        include_im
+00017b30: 7061 6374 7320 2862 6f6f 6c29 2069 6620  pacts (bool) if 
+00017b40: 5472 7565 2c20 696d 7061 6374 7320 6172  True, impacts ar
+00017b50: 6520 696e 636c 7564 6564 2069 6e20 7468  e included in th
+00017b60: 6520 7265 7475 726e 6564 2064 6174 6166  e returned dataf
+00017b70: 7261 6d65 0d0a 2020 2020 2020 2020 2222  rame..        ""
+00017b80: 220d 0a20 2020 2020 2020 2070 6c6f 745f  "..        plot_
+00017b90: 6c69 7374 203d 205b 5d0d 0a20 2020 2020  list = []..     
+00017ba0: 2020 2070 6c6f 745f 6c69 7374 2e61 7070     plot_list.app
+00017bb0: 656e 6428 7365 6c66 2e70 726f 6365 7373  end(self.process
+00017bc0: 5f63 6f6d 706f 6e65 6e74 7328 746f 5f6f  _components(to_o
+00017bd0: 7269 6769 6e5f 7370 6163 653d 746f 5f6f  rigin_space=to_o
+00017be0: 7269 6769 6e5f 7370 6163 6529 290d 0a20  rigin_space)).. 
+00017bf0: 2020 2020 2020 2074 7265 6e64 203d 2073         trend = s
+00017c00: 656c 662e 7072 6564 6963 7465 645f 7472  elf.predicted_tr
+00017c10: 656e 642e 636f 7079 2829 0d0a 2020 2020  end.copy()..    
+00017c20: 2020 2020 7472 656e 642e 636f 6c75 6d6e      trend.column
+00017c30: 7320 3d20 7064 2e4d 756c 7469 496e 6465  s = pd.MultiInde
+00017c40: 782e 6672 6f6d 5f61 7272 6179 7328 0d0a  x.from_arrays(..
+00017c50: 2020 2020 2020 2020 2020 2020 5b74 7265              [tre
+00017c60: 6e64 2e63 6f6c 756d 6e73 2c20 5b27 7472  nd.columns, ['tr
+00017c70: 656e 6427 5d20 2a20 6c65 6e28 7472 656e  end'] * len(tren
+00017c80: 642e 636f 6c75 6d6e 7329 5d0d 0a20 2020  d.columns)]..   
+00017c90: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00017ca0: 706c 6f74 5f6c 6973 742e 6170 7065 6e64  plot_list.append
+00017cb0: 2874 7265 6e64 290d 0a20 2020 2020 2020  (trend)..       
+00017cc0: 2069 6620 7365 6c66 2e69 6d70 6163 7473   if self.impacts
+00017cd0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00017ce0: 2069 6e63 6c75 6465 5f69 6d70 6163 7473   include_impacts
+00017cf0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00017d00: 6d70 6163 7473 203d 2073 656c 662e 696d  mpacts = self.im
+00017d10: 7061 6374 732e 636f 7079 2829 0d0a 2020  pacts.copy()..  
+00017d20: 2020 2020 2020 2020 2020 696d 7061 6374            impact
+00017d30: 732e 636f 6c75 6d6e 7320 3d20 7064 2e4d  s.columns = pd.M
+00017d40: 756c 7469 496e 6465 782e 6672 6f6d 5f61  ultiIndex.from_a
+00017d50: 7272 6179 7328 0d0a 2020 2020 2020 2020  rrays(..        
+00017d60: 2020 2020 2020 2020 5b69 6d70 6163 7473          [impacts
+00017d70: 2e63 6f6c 756d 6e73 2c20 5b27 696d 7061  .columns, ['impa
+00017d80: 6374 7327 5d20 2a20 6c65 6e28 696d 7061  cts'] * len(impa
+00017d90: 6374 732e 636f 6c75 6d6e 7329 5d0d 0a20  cts.columns)].. 
+00017da0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00017db0: 2020 2020 2020 2020 2020 706c 6f74 5f6c            plot_l
+00017dc0: 6973 742e 6170 7065 6e64 2869 6d70 6163  ist.append(impac
+00017dd0: 7473 290d 0a20 2020 2020 2020 2072 6574  ts)..        ret
+00017de0: 7572 6e20 7064 2e63 6f6e 6361 7428 706c  urn pd.concat(pl
+00017df0: 6f74 5f6c 6973 742c 2061 7869 733d 3129  ot_list, axis=1)
+00017e00: 0d0a 0d0a 2020 2020 6465 6620 706c 6f74  ....    def plot
+00017e10: 5f74 7265 6e64 280d 0a20 2020 2020 2020  _trend(..       
+00017e20: 2073 656c 662c 0d0a 2020 2020 2020 2020   self,..        
+00017e30: 7365 7269 6573 3d4e 6f6e 652c 0d0a 2020  series=None,..  
+00017e40: 2020 2020 2020 766c 696e 653d 4e6f 6e65        vline=None
+00017e50: 2c0d 0a20 2020 2020 2020 2063 6f6c 6f72  ,..        color
+00017e60: 733d 5b22 2364 3466 3734 6622 2c20 2223  s=["#d4f74f", "#
+00017e70: 3832 6162 3561 222c 2022 2366 6636 6330  82ab5a", "#ff6c0
+00017e80: 3522 2c20 2223 6331 3236 3030 225d 2c0d  5", "#c12600"],.
+00017e90: 0a20 2020 2020 2020 2074 6974 6c65 3d4e  .        title=N
+00017ea0: 6f6e 652c 0d0a 2020 2020 2020 2020 7374  one,..        st
+00017eb0: 6172 745f 6461 7465 3d4e 6f6e 652c 0d0a  art_date=None,..
+00017ec0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+00017ed0: 2c0d 0a20 2020 2029 3a0d 0a20 2020 2020  ,..    ):..     
+00017ee0: 2020 2023 2059 4d41 5820 6672 6f6d 2050     # YMAX from P
+00017ef0: 4c4f 5420 4f4e 4c59 0d0a 2020 2020 2020  LOT ONLY..      
+00017f00: 2020 6966 2073 6572 6965 7320 6973 204e    if series is N
+00017f10: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00017f20: 2020 7365 7269 6573 203d 2072 616e 646f    series = rando
+00017f30: 6d2e 6368 6f69 6365 2873 656c 662e 636f  m.choice(self.co
+00017f40: 6c75 6d6e 5f6e 616d 6573 290d 0a20 2020  lumn_names)..   
+00017f50: 2020 2020 2069 6620 7469 746c 6520 6973       if title is
+00017f60: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00017f70: 2020 2020 7469 746c 6520 3d20 6622 5472      title = f"Tr
+00017f80: 656e 6420 4272 6561 6b64 6f77 6e20 666f  end Breakdown fo
+00017f90: 7220 7b73 6572 6965 737d 220d 0a20 2020  r {series}"..   
+00017fa0: 2020 2020 2070 5f69 6e64 7820 3d20 7365       p_indx = se
+00017fb0: 6c66 2e63 6f6c 756d 6e5f 6e61 6d65 732e  lf.column_names.
+00017fc0: 6765 745f 6c6f 6328 7365 7269 6573 290d  get_loc(series).
+00017fd0: 0a20 2020 2020 2020 2063 7572 5f74 7265  .        cur_tre
+00017fe0: 6e64 203d 2073 656c 662e 7072 6564 6963  nd = self.predic
+00017ff0: 7465 645f 7472 656e 645b 7365 7269 6573  ted_trend[series
+00018000: 5d2e 636f 7079 2829 0d0a 2020 2020 2020  ].copy()..      
+00018010: 2020 746c 7320 3d20 6c65 6e28 6375 725f    tls = len(cur_
+00018020: 7472 656e 6429 0d0a 2020 2020 2020 2020  trend)..        
+00018030: 706c 6f74 5f64 6620 3d20 7064 2e44 6174  plot_df = pd.Dat
+00018040: 6146 7261 6d65 280d 0a20 2020 2020 2020  aFrame(..       
+00018050: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00018060: 2020 2020 2020 2020 2764 6563 6c69 6e65          'decline
+00018070: 5f61 6363 656c 6572 6174 696e 6727 3a20  _accelerating': 
+00018080: 6375 725f 7472 656e 645b 0d0a 2020 2020  cur_trend[..    
+00018090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180a0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+000180b0: 2020 2020 2020 2020 2020 206e 702e 6873             np.hs
+000180c0: 7461 636b 2828 6e70 2e73 6967 6e62 6974  tack((np.signbit
+000180d0: 2873 656c 662e 6163 6365 6c5b 3a2c 2070  (self.accel[:, p
+000180e0: 5f69 6e64 785d 292c 2046 616c 7365 2929  _indx]), False))
+000180f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018100: 2020 2020 2020 2020 2020 2620 7365 6c66            & self
+00018110: 2e73 6c6f 7065 5f73 6967 6e5b 3a2c 2070  .slope_sign[:, p
+00018120: 5f69 6e64 785d 0d0a 2020 2020 2020 2020  _indx]..        
+00018130: 2020 2020 2020 2020 2020 2020 295b 2d74              )[-t
+00018140: 6c73 3a5d 0d0a 2020 2020 2020 2020 2020  ls:]..          
+00018150: 2020 2020 2020 5d2c 0d0a 2020 2020 2020        ],..      
+00018160: 2020 2020 2020 2020 2020 2764 6563 6c69            'decli
+00018170: 6e65 5f64 6563 656c 6572 6174 696e 6727  ne_decelerating'
+00018180: 3a20 6375 725f 7472 656e 645b 0d0a 2020  : cur_trend[..  
+00018190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181a0: 2020 280d 0a20 2020 2020 2020 2020 2020    (..           
+000181b0: 2020 2020 2020 2020 2020 2020 2028 7e6e               (~n
+000181c0: 702e 6873 7461 636b 2828 6e70 2e73 6967  p.hstack((np.sig
+000181d0: 6e62 6974 2873 656c 662e 6163 6365 6c5b  nbit(self.accel[
+000181e0: 3a2c 2070 5f69 6e64 785d 292c 2046 616c  :, p_indx]), Fal
+000181f0: 7365 2929 290d 0a20 2020 2020 2020 2020  se)))..         
+00018200: 2020 2020 2020 2020 2020 2020 2020 2026                 &
+00018210: 2073 656c 662e 736c 6f70 655f 7369 676e   self.slope_sign
+00018220: 5b3a 2c20 705f 696e 6478 5d0d 0a20 2020  [:, p_indx]..   
+00018230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018240: 2029 5b2d 746c 733a 5d0d 0a20 2020 2020   )[-tls:]..     
+00018250: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+00018260: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00018270: 6772 6f77 7468 5f64 6563 656c 6572 6174  growth_decelerat
+00018280: 696e 6727 3a20 6375 725f 7472 656e 645b  ing': cur_trend[
+00018290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000182a0: 2020 2020 2020 280d 0a20 2020 2020 2020        (..       
+000182b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182c0: 206e 702e 6873 7461 636b 2828 6e70 2e73   np.hstack((np.s
+000182d0: 6967 6e62 6974 2873 656c 662e 6163 6365  ignbit(self.acce
+000182e0: 6c5b 3a2c 2070 5f69 6e64 785d 292c 2046  l[:, p_indx]), F
+000182f0: 616c 7365 2929 0d0a 2020 2020 2020 2020  alse))..        
+00018300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018310: 2620 287e 7365 6c66 2e73 6c6f 7065 5f73  & (~self.slope_s
+00018320: 6967 6e5b 3a2c 2070 5f69 6e64 785d 290d  ign[:, p_indx]).
+00018330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018340: 2020 2020 2029 5b2d 746c 733a 5d0d 0a20       )[-tls:].. 
+00018350: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00018360: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00018370: 2020 2027 6772 6f77 7468 5f61 6363 656c     'growth_accel
+00018380: 6572 6174 696e 6727 3a20 6375 725f 7472  erating': cur_tr
+00018390: 656e 645b 0d0a 2020 2020 2020 2020 2020  end[..          
+000183a0: 2020 2020 2020 2020 2020 280d 0a20 2020            (..   
+000183b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183c0: 2020 2020 2028 7e6e 702e 6873 7461 636b       (~np.hstack
+000183d0: 2828 6e70 2e73 6967 6e62 6974 2873 656c  ((np.signbit(sel
+000183e0: 662e 6163 6365 6c5b 3a2c 2070 5f69 6e64  f.accel[:, p_ind
+000183f0: 785d 292c 2046 616c 7365 2929 290d 0a20  x]), False))).. 
+00018400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018410: 2020 2020 2020 2026 2028 7e73 656c 662e         & (~self.
+00018420: 736c 6f70 655f 7369 676e 5b3a 2c20 705f  slope_sign[:, p_
+00018430: 696e 6478 5d29 0d0a 2020 2020 2020 2020  indx])..        
+00018440: 2020 2020 2020 2020 2020 2020 295b 2d74              )[-t
+00018450: 6c73 3a5d 0d0a 2020 2020 2020 2020 2020  ls:]..          
+00018460: 2020 2020 2020 5d2c 0d0a 2020 2020 2020        ],..      
+00018470: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
+00018480: 2020 2020 2020 696e 6465 783d 6375 725f        index=cur_
+00018490: 7472 656e 642e 696e 6465 782c 0d0a 2020  trend.index,..  
+000184a0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000184b0: 2069 6620 7374 6172 745f 6461 7465 203d   if start_date =
+000184c0: 3d20 2261 7574 6f22 3a0d 0a20 2020 2020  = "auto":..     
+000184d0: 2020 2020 2020 2073 6c78 203d 2073 656c         slx = sel
+000184e0: 662e 666f 7265 6361 7374 5f6c 656e 6774  f.forecast_lengt
+000184f0: 6820 2a20 330d 0a20 2020 2020 2020 2020  h * 3..         
+00018500: 2020 2069 6620 736c 7820 3e20 6c65 6e28     if slx > len(
+00018510: 706c 6f74 5f64 662e 696e 6465 7829 3a0d  plot_df.index):.
+00018520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018530: 2073 6c78 203d 2030 0d0a 2020 2020 2020   slx = 0..      
+00018540: 2020 2020 2020 7374 6172 745f 6461 7465        start_date
+00018550: 203d 2070 6c6f 745f 6466 2e69 6e64 6578   = plot_df.index
+00018560: 5b2d 736c 785d 0d0a 2020 2020 2020 2020  [-slx]..        
+00018570: 6966 2073 7461 7274 5f64 6174 6520 6973  if start_date is
+00018580: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00018590: 2020 2020 2020 2020 706c 6f74 5f64 6620          plot_df 
+000185a0: 3d20 706c 6f74 5f64 665b 706c 6f74 5f64  = plot_df[plot_d
+000185b0: 662e 696e 6465 7820 3e3d 2073 7461 7274  f.index >= start
+000185c0: 5f64 6174 655d 0d0a 2020 2020 2020 2020  _date]..        
+000185d0: 6178 203d 2070 6c6f 745f 6466 2e70 6c6f  ax = plot_df.plo
+000185e0: 7428 7469 746c 653d 7469 746c 652c 2063  t(title=title, c
+000185f0: 6f6c 6f72 3d63 6f6c 6f72 732c 202a 2a6b  olor=colors, **k
+00018600: 7761 7267 7329 0d0a 2020 2020 2020 2020  wargs)..        
+00018610: 6861 6e64 6c65 732c 206c 6162 656c 7320  handles, labels 
+00018620: 3d20 6178 2e67 6574 5f6c 6567 656e 645f  = ax.get_legend_
+00018630: 6861 6e64 6c65 735f 6c61 6265 6c73 2829  handles_labels()
+00018640: 0d0a 2020 2020 2020 2020 2320 6178 2e73  ..        # ax.s
+00018650: 6361 7474 6572 2863 7572 5f74 7265 6e64  catter(cur_trend
+00018660: 2e69 6e64 6578 5b73 656c 662e 6368 616e  .index[self.chan
+00018670: 6765 706f 696e 7473 5b3a 2c20 705f 696e  gepoints[:, p_in
+00018680: 6478 5d5d 2c20 6375 725f 7472 656e 645b  dx]], cur_trend[
+00018690: 7365 6c66 2e63 6861 6e67 6570 6f69 6e74  self.changepoint
+000186a0: 735b 3a2c 2070 5f69 6e64 785d 5d2c 2063  s[:, p_indx]], c
+000186b0: 3d27 2366 6463 6330 3927 2c20 733d 342e  ='#fdcc09', s=4.
+000186c0: 3029 0d0a 2020 2020 2020 2020 2320 6178  0)..        # ax
+000186d0: 2e73 6361 7474 6572 2863 7572 5f74 7265  .scatter(cur_tre
+000186e0: 6e64 2e69 6e64 6578 5b73 656c 662e 7a65  nd.index[self.ze
+000186f0: 726f 5f63 726f 7373 696e 6773 5b3a 2c20  ro_crossings[:, 
+00018700: 705f 696e 6478 5d5d 2c20 6375 725f 7472  p_indx]], cur_tr
+00018710: 656e 645b 7365 6c66 2e7a 6572 6f5f 6372  end[self.zero_cr
+00018720: 6f73 7369 6e67 735b 3a2c 2070 5f69 6e64  ossings[:, p_ind
+00018730: 785d 5d2c 2063 3d27 2335 3132 6637 3427  x]], c='#512f74'
+00018740: 2c20 733d 342e 3029 0d0a 2020 2020 2020  , s=4.0)..      
+00018750: 2020 6966 2073 656c 662e 7472 656e 645f    if self.trend_
+00018760: 616e 6f6d 616c 795f 6465 7465 6374 6f72  anomaly_detector
+00018770: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00018780: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00018790: 6c66 2e74 7265 6e64 5f61 6e6f 6d61 6c79  lf.trend_anomaly
+000187a0: 5f64 6574 6563 746f 722e 6f75 7470 7574  _detector.output
+000187b0: 203d 3d20 2275 6e69 7661 7269 6174 6522   == "univariate"
+000187c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000187d0: 2020 2069 5f61 6e6f 6d20 3d20 7365 6c66     i_anom = self
+000187e0: 2e74 7265 6e64 5f61 6e6f 6d61 6c79 5f64  .trend_anomaly_d
+000187f0: 6574 6563 746f 722e 616e 6f6d 616c 6965  etector.anomalie
+00018800: 732e 696e 6465 785b 0d0a 2020 2020 2020  s.index[..      
+00018810: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018820: 6c66 2e61 6e6f 6d61 6c79 5f64 6574 6563  lf.anomaly_detec
+00018830: 746f 722e 616e 6f6d 616c 6965 732e 696c  tor.anomalies.il
+00018840: 6f63 5b3a 2c20 305d 203d 3d20 2d31 0d0a  oc[:, 0] == -1..
+00018850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018860: 5d0d 0a20 2020 2020 2020 2020 2020 2065  ]..            e
+00018870: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00018880: 2020 2020 2020 7365 7269 6573 5f61 6e6f        series_ano
+00018890: 6d20 3d20 7365 6c66 2e74 7265 6e64 5f61  m = self.trend_a
+000188a0: 6e6f 6d61 6c79 5f64 6574 6563 746f 722e  nomaly_detector.
+000188b0: 616e 6f6d 616c 6965 735b 7365 7269 6573  anomalies[series
+000188c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000188d0: 2020 2069 5f61 6e6f 6d20 3d20 7365 7269     i_anom = seri
+000188e0: 6573 5f61 6e6f 6d5b 7365 7269 6573 5f61  es_anom[series_a
+000188f0: 6e6f 6d20 3d3d 202d 315d 2e69 6e64 6578  nom == -1].index
+00018900: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00018910: 2073 7461 7274 5f64 6174 6520 6973 206e   start_date is n
+00018920: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00018930: 2020 2020 2020 2020 2020 695f 616e 6f6d            i_anom
+00018940: 203d 2069 5f61 6e6f 6d5b 695f 616e 6f6d   = i_anom[i_anom
+00018950: 203e 3d20 7374 6172 745f 6461 7465 5d0d   >= start_date].
+00018960: 0a20 2020 2020 2020 2020 2020 2069 5f61  .            i_a
+00018970: 6e6f 6d20 3d20 695f 616e 6f6d 5b69 5f61  nom = i_anom[i_a
+00018980: 6e6f 6d20 3e3d 2063 7572 5f74 7265 6e64  nom >= cur_trend
+00018990: 2e69 6e64 6578 5b30 5d5d 0d0a 2020 2020  .index[0]]..    
+000189a0: 2020 2020 2020 2020 2320 6f6e 6c79 2070          # only p
+000189b0: 6c6f 7420 6966 2073 6f6d 6520 616e 6f6d  lot if some anom
+000189c0: 616c 6965 732c 2061 6e64 206e 6f74 2077  alies, and not w
+000189d0: 6179 2074 6f6f 206d 616e 7920 616e 6f6d  ay too many anom
+000189e0: 616c 6965 730d 0a20 2020 2020 2020 2020  alies..         
+000189f0: 2020 2069 6620 6c65 6e28 695f 616e 6f6d     if len(i_anom
+00018a00: 2920 3e20 3020 616e 6420 6c65 6e28 695f  ) > 0 and len(i_
+00018a10: 616e 6f6d 2920 3c20 6c65 6e28 706c 6f74  anom) < len(plot
+00018a20: 5f64 6629 202a 2030 2e35 3a0d 0a20 2020  _df) * 0.5:..   
+00018a30: 2020 2020 2020 2020 2020 2020 2073 6361               sca
+00018a40: 7431 203d 2061 782e 7363 6174 7465 7228  t1 = ax.scatter(
+00018a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018a60: 2020 2020 2020 695f 616e 6f6d 2e74 6f6c        i_anom.tol
+00018a70: 6973 7428 292c 2063 7572 5f74 7265 6e64  ist(), cur_trend
+00018a80: 2e6c 6f63 5b69 5f61 6e6f 6d5d 2c20 633d  .loc[i_anom], c=
+00018a90: 2272 6564 222c 2073 3d31 362e 300d 0a20  "red", s=16.0.. 
+00018aa0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00018ab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018ac0: 2020 6861 6e64 6c65 7320 2b3d 205b 7363    handles += [sc
+00018ad0: 6174 315d 0d0a 2020 2020 2020 2020 2020  at1]..          
+00018ae0: 2020 2020 2020 6c61 6265 6c73 202b 3d20        labels += 
+00018af0: 5b27 7472 656e 6420 616e 6f6d 616c 6965  ['trend anomalie
+00018b00: 7327 5d0d 0a20 2020 2020 2020 2069 6620  s']..        if 
+00018b10: 766c 696e 6520 6973 206e 6f74 204e 6f6e  vline is not Non
+00018b20: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00018b30: 6178 2e76 6c69 6e65 7328 0d0a 2020 2020  ax.vlines(..    
+00018b40: 2020 2020 2020 2020 2020 2020 783d 766c              x=vl
+00018b50: 696e 652c 0d0a 2020 2020 2020 2020 2020  ine,..          
+00018b60: 2020 2020 2020 6c73 3d27 2d2d 272c 0d0a        ls='--',..
+00018b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b80: 6c77 3d31 2c0d 0a20 2020 2020 2020 2020  lw=1,..         
+00018b90: 2020 2020 2020 2063 6f6c 6f72 733d 2764         colors='d
+00018ba0: 6172 6b72 6564 272c 0d0a 2020 2020 2020  arkred',..      
+00018bb0: 2020 2020 2020 2020 2020 796d 696e 3d63            ymin=c
+00018bc0: 7572 5f74 7265 6e64 5b63 7572 5f74 7265  ur_trend[cur_tre
+00018bd0: 6e64 2e69 6e64 6578 203e 3d20 7374 6172  nd.index >= star
+00018be0: 745f 6461 7465 5d2e 6d69 6e28 292c 0d0a  t_date].min(),..
+00018bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c00: 796d 6178 3d63 7572 5f74 7265 6e64 5b63  ymax=cur_trend[c
+00018c10: 7572 5f74 7265 6e64 2e69 6e64 6578 203e  ur_trend.index >
+00018c20: 3d20 7374 6172 745f 6461 7465 5d2e 6d61  = start_date].ma
+00018c30: 7828 292c 0d0a 2020 2020 2020 2020 2020  x(),..          
+00018c40: 2020 290d 0a20 2020 2020 2020 2061 782e    )..        ax.
+00018c50: 6c65 6765 6e64 2868 616e 646c 6573 2c20  legend(handles, 
+00018c60: 6c61 6265 6c73 290d 0a20 2020 2020 2020  labels)..       
+00018c70: 2072 6574 7572 6e20 6178 0d0a 0d0a 2020   return ax....  
+00018c80: 2020 6465 6620 706c 6f74 5f66 6f72 6563    def plot_forec
+00018c90: 6173 7428 0d0a 2020 2020 2020 2020 7365  ast(..        se
+00018ca0: 6c66 2c0d 0a20 2020 2020 2020 2070 7265  lf,..        pre
+00018cb0: 6469 6374 696f 6e2c 0d0a 2020 2020 2020  diction,..      
+00018cc0: 2020 6163 7475 616c 733d 4e6f 6e65 2c0d    actuals=None,.
+00018cd0: 0a20 2020 2020 2020 2073 6572 6965 733d  .        series=
+00018ce0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2073  None,..        s
+00018cf0: 7461 7274 5f64 6174 653d 4e6f 6e65 2c0d  tart_date=None,.
+00018d00: 0a20 2020 2020 2020 2061 6e6f 6d61 6c79  .        anomaly
+00018d10: 5f63 6f6c 6f72 3d22 6461 726b 736c 6174  _color="darkslat
+00018d20: 6562 6c75 6522 2c0d 0a20 2020 2020 2020  eblue",..       
+00018d30: 2068 6f6c 6964 6179 5f63 6f6c 6f72 3d22   holiday_color="
+00018d40: 6461 726b 6772 6565 6e22 2c0d 0a20 2020  darkgreen",..   
+00018d50: 2020 2020 2074 7265 6e64 5f61 6e6f 6d61       trend_anoma
+00018d60: 6c79 5f63 6f6c 6f72 3d27 736c 6174 6567  ly_color='slateg
+00018d70: 7261 7927 2c0d 0a20 2020 2020 2020 2070  ray',..        p
+00018d80: 6f69 6e74 5f73 697a 653d 3132 2e30 2c0d  oint_size=12.0,.
+00018d90: 0a20 2020 2029 3a0d 0a20 2020 2020 2020  .    ):..       
+00018da0: 2022 2222 506c 6f74 2061 2066 6f72 6563   """Plot a forec
+00018db0: 6173 7420 7469 6d65 2073 6572 6965 732e  ast time series.
+00018dc0: 0d0a 0d0a 2020 2020 2020 2020 4172 6773  ....        Args
+00018dd0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00018de0: 7265 6469 6374 696f 6e20 286d 6f64 656c  rediction (model
+00018df0: 2070 7265 6469 6374 696f 6e20 6f62 6a65   prediction obje
+00018e00: 6374 2c20 7265 7175 6972 6564 290d 0a20  ct, required).. 
+00018e10: 2020 2020 2020 2020 2020 2061 6374 7561             actua
+00018e20: 6c73 2028 7064 2e44 6174 6146 7261 6d65  ls (pd.DataFrame
+00018e30: 293a 2077 6964 6520 7374 796c 6520 6466  ): wide style df
+00018e40: 2c20 6f66 206b 6e6f 7720 6461 7461 2069  , of know data i
+00018e50: 6620 6176 6169 6c61 626c 650d 0a20 2020  f available..   
+00018e60: 2020 2020 2020 2020 2073 6572 6965 7320           series 
+00018e70: 2873 7472 293a 206e 616d 6520 6f66 2074  (str): name of t
+00018e80: 696d 6520 7365 7269 6573 2063 6f6c 756d  ime series colum
+00018e90: 6e20 746f 2070 6c6f 740d 0a20 2020 2020  n to plot..     
+00018ea0: 2020 2020 2020 2073 7461 7274 5f64 6174         start_dat
+00018eb0: 6520 2873 7472 206f 7220 5469 6d65 7374  e (str or Timest
+00018ec0: 616d 7029 3a20 706f 696e 7420 6174 2077  amp): point at w
+00018ed0: 6869 6368 2074 6f20 6265 6769 6e20 5820  hich to begin X 
+00018ee0: 6178 6973 0d0a 2020 2020 2020 2020 2020  axis..          
+00018ef0: 2020 616e 6f6d 616c 795f 636f 6c6f 7220    anomaly_color 
+00018f00: 2873 7472 293a 206e 616d 6520 6f66 2061  (str): name of a
+00018f10: 6e6f 6d61 6c79 2070 6f69 6e74 2063 6f6c  nomaly point col
+00018f20: 6f72 0d0a 2020 2020 2020 2020 2020 2020  or..            
+00018f30: 686f 6c69 6461 795f 636f 6c6f 7220 2873  holiday_color (s
+00018f40: 7472 293a 206e 616d 6520 6f66 2068 6f6c  tr): name of hol
+00018f50: 6964 6179 2070 6f69 6e74 2063 6f6c 6f72  iday point color
+00018f60: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+00018f70: 656e 645f 616e 6f6d 616c 795f 636f 6c6f  end_anomaly_colo
+00018f80: 7220 2873 7472 293a 206e 616d 6520 6f66  r (str): name of
+00018f90: 2074 7265 6e64 2061 6e6f 6d61 6c79 2070   trend anomaly p
+00018fa0: 6f69 6e74 2063 6f6c 6f72 0d0a 2020 2020  oint color..    
+00018fb0: 2020 2020 2020 2020 706f 696e 745f 7369          point_si
+00018fc0: 7a65 2028 7374 7229 3a20 706f 696e 7420  ze (str): point 
+00018fd0: 7369 7a65 2066 6f72 2061 6c6c 2061 6e6f  size for all ano
+00018fe0: 6d61 6c69 6573 0d0a 2020 2020 2020 2020  malies..        
+00018ff0: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
+00019000: 7365 7269 6573 2069 7320 4e6f 6e65 3a0d  series is None:.
+00019010: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
+00019020: 6965 7320 3d20 7261 6e64 6f6d 2e63 686f  ies = random.cho
+00019030: 6963 6528 7365 6c66 2e63 6f6c 756d 6e5f  ice(self.column_
+00019040: 6e61 6d65 7329 0d0a 2020 2020 2020 2020  names)..        
+00019050: 6966 2061 6374 7561 6c73 2069 7320 4e6f  if actuals is No
+00019060: 6e65 206f 7220 6e6f 7420 6973 696e 7374  ne or not isinst
+00019070: 616e 6365 280d 0a20 2020 2020 2020 2020  ance(..         
+00019080: 2020 2061 6374 7561 6c73 2c20 2870 642e     actuals, (pd.
+00019090: 4461 7461 4672 616d 652c 206e 702e 6172  DataFrame, np.ar
+000190a0: 7261 792c 2070 642e 5365 7269 6573 290d  ray, pd.Series).
+000190b0: 0a20 2020 2020 2020 2029 3a0d 0a20 2020  .        ):..   
+000190c0: 2020 2020 2020 2020 2061 6374 7561 6c73           actuals
+000190d0: 5f75 7365 6420 3d20 7072 6564 6963 7469  _used = predicti
+000190e0: 6f6e 2e66 6f72 6563 6173 740d 0a20 2020  on.forecast..   
+000190f0: 2020 2020 2020 2020 2061 6374 7561 6c73           actuals
+00019100: 5f66 6c61 6720 3d20 4661 6c73 650d 0a20  _flag = False.. 
+00019110: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00019120: 2020 2020 2020 2020 2020 6163 7475 616c            actual
+00019130: 735f 666c 6167 203d 2054 7275 650d 0a20  s_flag = True.. 
+00019140: 2020 2020 2020 2020 2020 2061 6374 7561             actua
+00019150: 6c73 5f75 7365 6420 3d20 6163 7475 616c  ls_used = actual
+00019160: 732e 7265 696e 6465 7828 7072 6564 6963  s.reindex(predic
+00019170: 7469 6f6e 2e66 6f72 6563 6173 742e 696e  tion.forecast.in
+00019180: 6465 7829 0d0a 2020 2020 2020 2020 766c  dex)..        vl
+00019190: 696e 6520 3d20 280d 0a20 2020 2020 2020  ine = (..       
+000191a0: 2020 2020 204e 6f6e 650d 0a20 2020 2020       None..     
+000191b0: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+000191c0: 6f72 6563 6173 745f 6c65 6e67 7468 2069  orecast_length i
+000191d0: 7320 4e6f 6e65 0d0a 2020 2020 2020 2020  s None..        
+000191e0: 2020 2020 656c 7365 2070 7265 6469 6374      else predict
+000191f0: 696f 6e2e 666f 7265 6361 7374 2e69 6e64  ion.forecast.ind
+00019200: 6578 5b2d 7365 6c66 2e66 6f72 6563 6173  ex[-self.forecas
+00019210: 745f 6c65 6e67 7468 5d0d 0a20 2020 2020  t_length]..     
+00019220: 2020 2029 0d0a 2020 2020 2020 2020 6966     )..        if
+00019230: 2073 7461 7274 5f64 6174 6520 3d3d 2022   start_date == "
+00019240: 6175 746f 223a 0d0a 2020 2020 2020 2020  auto":..        
+00019250: 2020 2020 6966 2061 6374 7561 6c73 2069      if actuals i
+00019260: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00019270: 2020 2020 2020 2020 2020 2020 2073 6c78               slx
+00019280: 203d 202d 7365 6c66 2e66 6f72 6563 6173   = -self.forecas
+00019290: 745f 6c65 6e67 7468 202a 2033 0d0a 2020  t_length * 3..  
+000192a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000192b0: 2061 6273 2873 6c78 2920 3e20 6163 7475   abs(slx) > actu
+000192c0: 616c 732e 7368 6170 655b 305d 3a0d 0a20  als.shape[0]:.. 
+000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192e0: 2020 2073 6c78 203d 2030 0d0a 2020 2020     slx = 0..    
+000192f0: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00019300: 745f 6461 7465 203d 2061 6374 7561 6c73  t_date = actuals
+00019310: 2e69 6e64 6578 5b73 6c78 5d0d 0a20 2020  .index[slx]..   
+00019320: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00019330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019340: 7374 6172 745f 6461 7465 203d 2070 7265  start_date = pre
+00019350: 6469 6374 696f 6e2e 666f 7265 6361 7374  diction.forecast
+00019360: 2e69 6e64 6578 5b30 5d0d 0a20 2020 2020  .index[0]..     
+00019370: 2020 2061 7820 3d20 7072 6564 6963 7469     ax = predicti
+00019380: 6f6e 2e70 6c6f 7428 0d0a 2020 2020 2020  on.plot(..      
+00019390: 2020 2020 2020 6163 7475 616c 735f 7573        actuals_us
+000193a0: 6564 2e6c 6f63 5b70 7265 6469 6374 696f  ed.loc[predictio
+000193b0: 6e2e 666f 7265 6361 7374 2e69 6e64 6578  n.forecast.index
+000193c0: 5d0d 0a20 2020 2020 2020 2020 2020 2069  ]..            i
+000193d0: 6620 6163 7475 616c 735f 666c 6167 2069  f actuals_flag i
+000193e0: 7320 6e6f 7420 4e6f 6e65 0d0a 2020 2020  s not None..    
+000193f0: 2020 2020 2020 2020 656c 7365 204e 6f6e          else Non
+00019400: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00019410: 7365 7269 6573 3d73 6572 6965 732c 0d0a  series=series,..
+00019420: 2020 2020 2020 2020 2020 2020 766c 696e              vlin
+00019430: 653d 766c 696e 652c 0d0a 2020 2020 2020  e=vline,..      
+00019440: 2020 2020 2020 7374 6172 745f 6461 7465        start_date
+00019450: 3d73 7461 7274 5f64 6174 652c 0d0a 2020  =start_date,..  
+00019460: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00019470: 2068 616e 646c 6573 2c20 6c61 6265 6c73   handles, labels
+00019480: 203d 2061 782e 6765 745f 6c65 6765 6e64   = ax.get_legend
+00019490: 5f68 616e 646c 6573 5f6c 6162 656c 7328  _handles_labels(
+000194a0: 290d 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+000194b0: 6c66 2e61 6e6f 6d61 6c79 5f64 6574 6563  lf.anomaly_detec
+000194c0: 746f 723a 0d0a 2020 2020 2020 2020 2020  tor:..          
+000194d0: 2020 6966 2073 656c 662e 616e 6f6d 616c    if self.anomal
+000194e0: 795f 6465 7465 6374 6f72 2e6f 7574 7075  y_detector.outpu
+000194f0: 7420 3d3d 2022 756e 6976 6172 6961 7465  t == "univariate
+00019500: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+00019510: 2020 2020 695f 616e 6f6d 203d 2073 656c      i_anom = sel
+00019520: 662e 616e 6f6d 616c 795f 6465 7465 6374  f.anomaly_detect
+00019530: 6f72 2e61 6e6f 6d61 6c69 6573 2e69 6e64  or.anomalies.ind
+00019540: 6578 5b0d 0a20 2020 2020 2020 2020 2020  ex[..           
+00019550: 2020 2020 2020 2020 2073 656c 662e 616e           self.an
+00019560: 6f6d 616c 795f 6465 7465 6374 6f72 2e61  omaly_detector.a
+00019570: 6e6f 6d61 6c69 6573 2e69 6c6f 635b 3a2c  nomalies.iloc[:,
+00019580: 2030 5d20 3d3d 202d 310d 0a20 2020 2020   0] == -1..     
+00019590: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
+000195a0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+000195b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000195c0: 2073 6572 6965 735f 616e 6f6d 203d 2073   series_anom = s
+000195d0: 656c 662e 616e 6f6d 616c 795f 6465 7465  elf.anomaly_dete
+000195e0: 6374 6f72 2e61 6e6f 6d61 6c69 6573 5b73  ctor.anomalies[s
+000195f0: 6572 6965 735d 0d0a 2020 2020 2020 2020  eries]..        
+00019600: 2020 2020 2020 2020 695f 616e 6f6d 203d          i_anom =
+00019610: 2073 6572 6965 735f 616e 6f6d 5b73 6572   series_anom[ser
+00019620: 6965 735f 616e 6f6d 203d 3d20 2d31 5d2e  ies_anom == -1].
+00019630: 696e 6465 780d 0a20 2020 2020 2020 2020  index..         
+00019640: 2020 2069 6620 7374 6172 745f 6461 7465     if start_date
+00019650: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00019660: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00019670: 5f61 6e6f 6d20 3d20 695f 616e 6f6d 5b69  _anom = i_anom[i
+00019680: 5f61 6e6f 6d20 3e3d 2073 7461 7274 5f64  _anom >= start_d
+00019690: 6174 655d 0d0a 2020 2020 2020 2020 2020  ate]..          
+000196a0: 2020 6966 2061 6374 7561 6c73 5f66 6c61    if actuals_fla
+000196b0: 673a 0d0a 2020 2020 2020 2020 2020 2020  g:..            
+000196c0: 2020 2020 695f 616e 6f6d 203d 2069 5f61      i_anom = i_a
+000196d0: 6e6f 6d5b 695f 616e 6f6d 203e 3d20 6163  nom[i_anom >= ac
+000196e0: 7475 616c 732e 696e 6465 785b 305d 5d0d  tuals.index[0]].
+000196f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00019700: 6c65 6e28 695f 616e 6f6d 2920 3e20 3020  len(i_anom) > 0 
+00019710: 616e 6420 280d 0a20 2020 2020 2020 2020  and (..         
+00019720: 2020 2020 2020 206e 6f74 2061 6374 7561         not actua
+00019730: 6c73 5f66 6c61 6720 6f72 206c 656e 2869  ls_flag or len(i
+00019740: 5f61 6e6f 6d29 203c 206c 656e 2861 6374  _anom) < len(act
+00019750: 7561 6c73 2920 2a20 302e 350d 0a20 2020  uals) * 0.5..   
+00019760: 2020 2020 2020 2020 2029 3a0d 0a20 2020           ):..   
+00019770: 2020 2020 2020 2020 2020 2020 2073 6361               sca
+00019780: 7431 203d 2061 782e 7363 6174 7465 7228  t1 = ax.scatter(
+00019790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000197a0: 2020 2020 2020 695f 616e 6f6d 2e74 6f6c        i_anom.tol
+000197b0: 6973 7428 292c 0d0a 2020 2020 2020 2020  ist(),..        
+000197c0: 2020 2020 2020 2020 2020 2020 6163 7475              actu
+000197d0: 616c 735f 7573 6564 2e72 6569 6e64 6578  als_used.reindex
+000197e0: 2869 5f61 6e6f 6d29 5b73 6572 6965 735d  (i_anom)[series]
+000197f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00019800: 2020 2020 2020 2063 3d61 6e6f 6d61 6c79         c=anomaly
+00019810: 5f63 6f6c 6f72 2c0d 0a20 2020 2020 2020  _color,..       
+00019820: 2020 2020 2020 2020 2020 2020 2073 3d70               s=p
+00019830: 6f69 6e74 5f73 697a 652c 0d0a 2020 2020  oint_size,..    
+00019840: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00019850: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00019860: 616e 646c 6573 202b 3d20 5b73 6361 7431  andles += [scat1
+00019870: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00019880: 2020 206c 6162 656c 7320 2b3d 205b 2261     labels += ["a
+00019890: 6e6f 6d61 6c69 6573 225d 0d0a 2020 2020  nomalies"]..    
+000198a0: 2020 2020 6966 2073 656c 662e 686f 6c69      if self.holi
+000198b0: 6461 795f 6465 7465 6374 6f72 3a0d 0a20  day_detector:.. 
+000198c0: 2020 2020 2020 2020 2020 2069 5f61 6e6f             i_ano
+000198d0: 6d20 3d20 7365 6c66 2e68 6f6c 6964 6179  m = self.holiday
+000198e0: 5f64 6574 6563 746f 722e 6461 7465 735f  _detector.dates_
+000198f0: 746f 5f68 6f6c 6964 6179 7328 0d0a 2020  to_holidays(..  
+00019900: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019910: 6c66 2e64 662e 696e 6465 782c 2073 7479  lf.df.index, sty
+00019920: 6c65 3d22 7365 7269 6573 5f66 6c61 6722  le="series_flag"
+00019930: 0d0a 2020 2020 2020 2020 2020 2020 295b  ..            )[
+00019940: 7365 7269 6573 5d0d 0a20 2020 2020 2020  series]..       
+00019950: 2020 2020 2069 5f61 6e6f 6d20 3d20 695f       i_anom = i_
+00019960: 616e 6f6d 2e69 6e64 6578 5b69 5f61 6e6f  anom.index[i_ano
+00019970: 6d20 3d3d 2031 5d0d 0a20 2020 2020 2020  m == 1]..       
+00019980: 2020 2020 2069 6620 6163 7475 616c 735f       if actuals_
+00019990: 666c 6167 3a0d 0a20 2020 2020 2020 2020  flag:..         
+000199a0: 2020 2020 2020 2069 5f61 6e6f 6d20 3d20         i_anom = 
+000199b0: 695f 616e 6f6d 5b69 5f61 6e6f 6d20 3e3d  i_anom[i_anom >=
+000199c0: 2061 6374 7561 6c73 2e69 6e64 6578 5b30   actuals.index[0
+000199d0: 5d5d 0d0a 2020 2020 2020 2020 2020 2020  ]]..            
+000199e0: 6966 206c 656e 2869 5f61 6e6f 6d29 203e  if len(i_anom) >
+000199f0: 2030 2061 6e64 2028 0d0a 2020 2020 2020   0 and (..      
+00019a00: 2020 2020 2020 2020 2020 6e6f 7420 6163            not ac
+00019a10: 7475 616c 735f 666c 6167 206f 7220 6c65  tuals_flag or le
+00019a20: 6e28 695f 616e 6f6d 2920 3c20 6c65 6e28  n(i_anom) < len(
+00019a30: 6163 7475 616c 7329 202a 2030 2e35 0d0a  actuals) * 0.5..
+00019a40: 2020 2020 2020 2020 2020 2020 293a 0d0a              ):..
+00019a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a60: 7363 6174 3220 3d20 6178 2e73 6361 7474  scat2 = ax.scatt
+00019a70: 6572 280d 0a20 2020 2020 2020 2020 2020  er(..           
+00019a80: 2020 2020 2020 2020 2069 5f61 6e6f 6d2e           i_anom.
+00019a90: 746f 6c69 7374 2829 2c0d 0a20 2020 2020  tolist(),..     
+00019aa0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00019ab0: 6374 7561 6c73 5f75 7365 642e 7265 696e  ctuals_used.rein
+00019ac0: 6465 7828 695f 616e 6f6d 295b 7365 7269  dex(i_anom)[seri
+00019ad0: 6573 5d2c 0d0a 2020 2020 2020 2020 2020  es],..          
+00019ae0: 2020 2020 2020 2020 2020 633d 686f 6c69            c=holi
+00019af0: 6461 795f 636f 6c6f 722c 0d0a 2020 2020  day_color,..    
+00019b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b10: 733d 706f 696e 745f 7369 7a65 2c0d 0a20  s=point_size,.. 
+00019b20: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00019b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019b40: 2020 6861 6e64 6c65 7320 2b3d 205b 7363    handles += [sc
+00019b50: 6174 325d 0d0a 2020 2020 2020 2020 2020  at2]..          
+00019b60: 2020 2020 2020 6c61 6265 6c73 202b 3d20        labels += 
+00019b70: 5b22 6465 7465 6374 6564 2068 6f6c 6964  ["detected holid
+00019b80: 6179 7322 5d0d 0a20 2020 2020 2020 2069  ays"]..        i
+00019b90: 6620 7365 6c66 2e74 7265 6e64 5f61 6e6f  f self.trend_ano
+00019ba0: 6d61 6c79 5f64 6574 6563 746f 7220 6973  maly_detector is
+00019bb0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00019bc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00019bd0: 7472 656e 645f 616e 6f6d 616c 795f 6465  trend_anomaly_de
+00019be0: 7465 6374 6f72 2e6f 7574 7075 7420 3d3d  tector.output ==
+00019bf0: 2022 756e 6976 6172 6961 7465 223a 0d0a   "univariate":..
+00019c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c10: 695f 616e 6f6d 203d 2073 656c 662e 7472  i_anom = self.tr
+00019c20: 656e 645f 616e 6f6d 616c 795f 6465 7465  end_anomaly_dete
+00019c30: 6374 6f72 2e61 6e6f 6d61 6c69 6573 2e69  ctor.anomalies.i
+00019c40: 6e64 6578 5b0d 0a20 2020 2020 2020 2020  ndex[..         
+00019c50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019c60: 616e 6f6d 616c 795f 6465 7465 6374 6f72  anomaly_detector
+00019c70: 2e61 6e6f 6d61 6c69 6573 2e69 6c6f 635b  .anomalies.iloc[
+00019c80: 3a2c 2030 5d20 3d3d 202d 310d 0a20 2020  :, 0] == -1..   
+00019c90: 2020 2020 2020 2020 2020 2020 205d 0d0a               ]..
+00019ca0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00019cb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00019cc0: 2020 2073 6572 6965 735f 616e 6f6d 203d     series_anom =
+00019cd0: 2073 656c 662e 7472 656e 645f 616e 6f6d   self.trend_anom
+00019ce0: 616c 795f 6465 7465 6374 6f72 2e61 6e6f  aly_detector.ano
+00019cf0: 6d61 6c69 6573 5b73 6572 6965 735d 0d0a  malies[series]..
+00019d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d10: 695f 616e 6f6d 203d 2073 6572 6965 735f  i_anom = series_
+00019d20: 616e 6f6d 5b73 6572 6965 735f 616e 6f6d  anom[series_anom
+00019d30: 203d 3d20 2d31 5d2e 696e 6465 780d 0a20   == -1].index.. 
+00019d40: 2020 2020 2020 2020 2020 2069 6620 7374             if st
+00019d50: 6172 745f 6461 7465 2069 7320 6e6f 7420  art_date is not 
+00019d60: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00019d70: 2020 2020 2020 2069 5f61 6e6f 6d20 3d20         i_anom = 
+00019d80: 695f 616e 6f6d 5b69 5f61 6e6f 6d20 3e3d  i_anom[i_anom >=
+00019d90: 2073 7461 7274 5f64 6174 655d 0d0a 2020   start_date]..  
+00019da0: 2020 2020 2020 2020 2020 6966 2061 6374            if act
+00019db0: 7561 6c73 5f66 6c61 673a 0d0a 2020 2020  uals_flag:..    
+00019dc0: 2020 2020 2020 2020 2020 2020 695f 616e              i_an
+00019dd0: 6f6d 203d 2069 5f61 6e6f 6d5b 695f 616e  om = i_anom[i_an
+00019de0: 6f6d 203e 3d20 6163 7475 616c 732e 696e  om >= actuals.in
+00019df0: 6465 785b 305d 5d0d 0a20 2020 2020 2020  dex[0]]..       
+00019e00: 2020 2020 2069 6620 6c65 6e28 695f 616e       if len(i_an
+00019e10: 6f6d 2920 3e20 3020 616e 6420 280d 0a20  om) > 0 and (.. 
+00019e20: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00019e30: 6f74 2061 6374 7561 6c73 5f66 6c61 6720  ot actuals_flag 
+00019e40: 6f72 206c 656e 2869 5f61 6e6f 6d29 203c  or len(i_anom) <
+00019e50: 206c 656e 2861 6374 7561 6c73 2920 2a20   len(actuals) * 
+00019e60: 302e 350d 0a20 2020 2020 2020 2020 2020  0.5..           
+00019e70: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
+00019e80: 2020 2020 2073 6361 7433 203d 2061 782e       scat3 = ax.
+00019e90: 7363 6174 7465 7228 0d0a 2020 2020 2020  scatter(..      
+00019ea0: 2020 2020 2020 2020 2020 2020 2020 695f                i_
+00019eb0: 616e 6f6d 2e74 6f6c 6973 7428 292c 0d0a  anom.tolist(),..
+00019ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ed0: 2020 2020 6163 7475 616c 735f 7573 6564      actuals_used
+00019ee0: 2e72 6569 6e64 6578 2869 5f61 6e6f 6d29  .reindex(i_anom)
+00019ef0: 5b73 6572 6965 735d 2c0d 0a20 2020 2020  [series],..     
+00019f00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00019f10: 3d74 7265 6e64 5f61 6e6f 6d61 6c79 5f63  =trend_anomaly_c
+00019f20: 6f6c 6f72 2c0d 0a20 2020 2020 2020 2020  olor,..         
+00019f30: 2020 2020 2020 2020 2020 2073 3d70 6f69             s=poi
+00019f40: 6e74 5f73 697a 652c 0d0a 2020 2020 2020  nt_size,..      
+00019f50: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00019f60: 2020 2020 2020 2020 2020 2020 2068 616e               han
+00019f70: 646c 6573 202b 3d20 5b73 6361 7433 5d0d  dles += [scat3].
+00019f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019f90: 206c 6162 656c 7320 2b3d 205b 2274 7265   labels += ["tre
+00019fa0: 6e64 2061 6e6f 6d61 6c69 6573 225d 0d0a  nd anomalies"]..
+00019fb0: 2020 2020 2020 2020 6178 2e6c 6567 656e          ax.legen
+00019fc0: 6428 6861 6e64 6c65 732c 206c 6162 656c  d(handles, label
+00019fd0: 7329 0d0a 2020 2020 2020 2020 7265 7475  s)..        retu
+00019fe0: 726e 2061 780d 0a0d 0a20 2020 2064 6566  rn ax....    def
+00019ff0: 2070 6c6f 745f 7468 696e 6773 2829 3a20   plot_things(): 
+0001a000: 2023 2070 6c61 6365 686f 6c64 6572 2066   # placeholder f
+0001a010: 6f72 206c 6174 6572 2070 6c6f 7474 696e  or later plottin
+0001a020: 6720 6675 6e63 7469 6f6e 730d 0a20 2020  g functions..   
+0001a030: 2020 2020 2023 2070 6c6f 7420 636f 6d70       # plot comp
+0001a040: 6f6e 656e 7473 0d0a 2020 2020 2020 2020  onents..        
+0001a050: 2320 706c 6f74 2074 7261 6e73 666f 726d  # plot transform
+0001a060: 6564 2064 6620 6966 2070 7265 7072 6f63  ed df if preproc
+0001a070: 6573 7320 6f72 2061 6e6f 6d61 6c79 2072  ess or anomaly r
+0001a080: 656d 6f76 616c 0d0a 2020 2020 2020 2020  emoval..        
+0001a090: 2320 706c 6f74 2070 6173 7420 696d 7061  # plot past impa
+0001a0a0: 6374 730d 0a20 2020 2020 2020 2023 2070  cts..        # p
+0001a0b0: 6c6f 7420 2520 636f 6e74 7269 6275 7469  lot % contributi
+0001a0c0: 6f6e 206f 6620 636f 6d70 6f6e 656e 7473  on of components
+0001a0d0: 0d0a 2020 2020 2020 2020 2320 706c 6f74  ..        # plot
+0001a0e0: 2065 7661 6c20 2873 686f 7720 6163 7475   eval (show actu
+0001a0f0: 616c 732c 2061 6c6f 6e67 7369 6465 2066  als, alongside f
+0001a100: 756c 6c20 616e 6420 636f 6d70 6f6e 656e  ull and componen
+0001a110: 7473 2074 6f20 6469 6167 6e6f 7365 290d  ts to diagnose).
+0001a120: 0a20 2020 2020 2020 2023 2070 6c6f 7420  .        # plot 
+0001a130: 7265 7369 6475 616c 2064 6973 7472 6962  residual distrib
+0001a140: 7574 696f 6e2f 5041 4346 0d0a 2020 2020  ution/PACF..    
+0001a150: 2020 2020 2320 706c 6f74 2069 6e66 6c65      # plot infle
+0001a160: 6374 696f 6e20 706f 696e 7473 2028 6669  ction points (fi
+0001a170: 6c74 6572 696e 6720 6f72 2073 6d6f 6f74  ltering or smoot
+0001a180: 6869 6e67 2066 6972 7374 290d 0a20 2020  hing first)..   
+0001a190: 2020 2020 2023 2070 6c6f 7420 6869 6768       # plot high
+0001a1a0: 6573 7420 6572 726f 7220 7365 7269 6573  est error series
+0001a1b0: 2c20 706c 6f74 2068 6967 6865 7374 2f6c  , plot highest/l
+0001a1c0: 6f77 6573 7420 6772 6f77 7468 0d0a 2020  owest growth..  
+0001a1d0: 2020 2020 2020 2320 7472 656e 643a 206f        # trend: o
+0001a1e0: 6e65 2063 6f6c 6f72 2066 6f72 2067 726f  ne color for gro
+0001a1f0: 7774 682c 2061 6e6f 7468 6572 2066 6f72  wth, another for
+0001a200: 2064 6563 6c69 6e65 2028 6461 726b 6572   decline (darker
+0001a210: 2061 7320 6163 6365 6c65 7261 7469 6e67   as accelerating
+0001a220: 2c20 6c69 6768 6572 2061 7320 736c 6f77  , ligher as slow
+0001a230: 696e 6729 0d0a 2020 2020 2020 2020 7265  ing)..        re
+0001a240: 7475 726e 204e 6f74 496d 706c 656d 656e  turn NotImplemen
+0001a250: 7465 640d 0a0d 0a0d 0a64 6566 2063 6c65  ted......def cle
+0001a260: 616e 5f72 6567 7265 7373 6f72 2869 6e5f  an_regressor(in_
+0001a270: 642c 2070 7265 6669 783d 2272 6567 725f  d, prefix="regr_
+0001a280: 2229 3a0d 0a20 2020 2069 6620 6e6f 7420  "):..    if not 
+0001a290: 6973 696e 7374 616e 6365 2869 6e5f 642c  isinstance(in_d,
+0001a2a0: 2070 642e 4461 7461 4672 616d 6529 3a0d   pd.DataFrame):.
+0001a2b0: 0a20 2020 2020 2020 2064 6620 3d20 7064  .        df = pd
+0001a2c0: 2e44 6174 6146 7261 6d65 2869 6e5f 6429  .DataFrame(in_d)
+0001a2d0: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
+0001a2e0: 2020 2020 2064 6620 3d20 696e 5f64 2e63       df = in_d.c
+0001a2f0: 6f70 7928 290d 0a20 2020 2064 662e 636f  opy()..    df.co
+0001a300: 6c75 6d6e 7320 3d20 5b70 7265 6669 7820  lumns = [prefix 
+0001a310: 2b20 636f 6c20 666f 7220 636f 6c20 696e  + col for col in
+0001a320: 2064 662e 636f 6c75 6d6e 735d 0d0a 2020   df.columns]..  
+0001a330: 2020 7265 7475 726e 2064 660d 0a0d 0a0d    return df.....
+0001a340: 0a64 6566 2063 7265 6174 655f 7428 6473  .def create_t(ds
+0001a350: 293a 0d0a 2020 2020 7265 7475 726e 2028  ):..    return (
+0001a360: 6473 202d 2064 732e 6d69 6e28 2929 202f  ds - ds.min()) /
+0001a370: 2028 6473 2e6d 6178 2829 202d 2064 732e   (ds.max() - ds.
+0001a380: 6d69 6e28 2929 0d0a 0d0a 0d0a 2323 2323  min())......####
+0001a390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a3a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a3b0: 230d 0a23 204a 5553 5420 4c45 4153 5420  #..# JUST LEAST 
+0001a3c0: 5351 5541 5245 5320 554e 4956 4152 4941  SQUARES UNIVARIA
+0001a3d0: 5445 0d0a 2320 6874 7470 733a 2f2f 7374  TE..# https://st
+0001a3e0: 6163 6b6f 7665 7266 6c6f 772e 636f 6d2f  ackoverflow.com/
+0001a3f0: 7175 6573 7469 6f6e 732f 3137 3637 3931  questions/176791
+0001a400: 3430 2f6d 756c 7469 706c 652d 6c69 6e65  40/multiple-line
+0001a410: 6172 2d72 6567 7265 7373 696f 6e2d 7769  ar-regression-wi
+0001a420: 7468 2d70 7974 686f 6e0d 0a0d 0a0d 0a64  th-python......d
+0001a430: 6566 206c 7374 7371 5f73 6f6c 7665 2858  ef lstsq_solve(X
+0001a440: 2c20 792c 206c 616d 623d 312c 2069 6465  , y, lamb=1, ide
+0001a450: 6e74 6974 795f 6d61 7472 6978 3d4e 6f6e  ntity_matrix=Non
+0001a460: 6529 3a0d 0a20 2020 2069 6620 6964 656e  e):..    if iden
+0001a470: 7469 7479 5f6d 6174 7269 7820 6973 204e  tity_matrix is N
+0001a480: 6f6e 653a 0d0a 2020 2020 2020 2020 6964  one:..        id
+0001a490: 656e 7469 7479 5f6d 6174 7269 7820 3d20  entity_matrix = 
+0001a4a0: 6e70 2e7a 6572 6f73 2828 582e 7368 6170  np.zeros((X.shap
+0001a4b0: 655b 315d 2c20 582e 7368 6170 655b 315d  e[1], X.shape[1]
+0001a4c0: 2929 0d0a 2020 2020 2020 2020 6e70 2e66  ))..        np.f
+0001a4d0: 696c 6c5f 6469 6167 6f6e 616c 2869 6465  ill_diagonal(ide
+0001a4e0: 6e74 6974 795f 6d61 7472 6978 2c20 3129  ntity_matrix, 1)
+0001a4f0: 0d0a 2020 2020 2020 2020 6964 656e 7469  ..        identi
+0001a500: 7479 5f6d 6174 7269 785b 302c 2030 5d20  ty_matrix[0, 0] 
+0001a510: 3d20 300d 0a20 2020 2058 7458 5f6c 616d  = 0..    XtX_lam
+0001a520: 6220 3d20 582e 542e 646f 7428 5829 202b  b = X.T.dot(X) +
+0001a530: 206c 616d 6220 2a20 6964 656e 7469 7479   lamb * identity
+0001a540: 5f6d 6174 7269 780d 0a20 2020 2058 7459  _matrix..    XtY
+0001a550: 203d 2058 2e54 2e64 6f74 2879 290d 0a20   = X.T.dot(y).. 
+0001a560: 2020 2072 6574 7572 6e20 6e70 2e6c 696e     return np.lin
+0001a570: 616c 672e 736f 6c76 6528 5874 585f 6c61  alg.solve(XtX_la
+0001a580: 6d62 2c20 5874 5929 0d0a 0d0a 0d0a 6465  mb, XtY)......de
+0001a590: 6620 636f 7374 5f66 756e 6374 696f 6e5f  f cost_function_
+0001a5a0: 6c31 2870 6172 616d 732c 2058 2c20 7929  l1(params, X, y)
+0001a5b0: 3a0d 0a20 2020 2072 6574 7572 6e20 6e70  :..    return np
+0001a5c0: 2e73 756d 286e 702e 6162 7328 7920 2d20  .sum(np.abs(y - 
+0001a5d0: 6e70 2e64 6f74 2858 2c20 7061 7261 6d73  np.dot(X, params
+0001a5e0: 2e72 6573 6861 7065 2858 2e73 6861 7065  .reshape(X.shape
+0001a5f0: 5b31 5d2c 2079 2e73 6861 7065 5b31 5d29  [1], y.shape[1])
+0001a600: 2929 290d 0a0d 0a0d 0a64 6566 2063 6f73  )))......def cos
+0001a610: 745f 6675 6e63 7469 6f6e 5f6c 315f 706f  t_function_l1_po
+0001a620: 7369 7469 7665 2870 6172 616d 732c 2058  sitive(params, X
+0001a630: 2c20 7929 3a0d 0a20 2020 2072 6574 7572  , y):..    retur
+0001a640: 6e20 6e70 2e73 756d 280d 0a20 2020 2020  n np.sum(..     
+0001a650: 2020 206e 702e 6162 7328 0d0a 2020 2020     np.abs(..    
+0001a660: 2020 2020 2020 2020 790d 0a20 2020 2020          y..     
+0001a670: 2020 2020 2020 202d 206e 702e 646f 7428         - np.dot(
+0001a680: 582c 206e 702e 7768 6572 6528 7061 7261  X, np.where(para
+0001a690: 6d73 203c 2030 2c20 302c 2070 6172 616d  ms < 0, 0, param
+0001a6a0: 7329 2e72 6573 6861 7065 2858 2e73 6861  s).reshape(X.sha
+0001a6b0: 7065 5b31 5d2c 2079 2e73 6861 7065 5b31  pe[1], y.shape[1
+0001a6c0: 5d29 290d 0a20 2020 2020 2020 2029 0d0a  ]))..        )..
+0001a6d0: 2020 2020 290d 0a0d 0a0d 0a23 2061 6374      )......# act
+0001a6e0: 7561 6c6c 7920 7468 6973 2069 7320 6d6f  ually this is mo
+0001a6f0: 7265 206c 696b 6520 4d41 4445 0d0a 6465  re like MADE..de
+0001a700: 6620 636f 7374 5f66 756e 6374 696f 6e5f  f cost_function_
+0001a710: 6477 6165 2870 6172 616d 732c 2058 2c20  dwae(params, X, 
+0001a720: 7929 3a0d 0a20 2020 2041 203d 2079 0d0a  y):..    A = y..
+0001a730: 2020 2020 4620 3d20 6e70 2e64 6f74 2858      F = np.dot(X
+0001a740: 2c20 7061 7261 6d73 2e72 6573 6861 7065  , params.reshape
+0001a750: 2858 2e73 6861 7065 5b31 5d2c 2079 2e73  (X.shape[1], y.s
+0001a760: 6861 7065 5b31 5d29 290d 0a20 2020 206c  hape[1]))..    l
+0001a770: 6173 745f 6f66 5f61 7272 6179 203d 2079  ast_of_array = y
+0001a780: 5b5b 305d 202b 206c 6973 7428 7261 6e67  [[0] + list(rang
+0001a790: 6528 6c65 6e28 7929 202d 2031 2929 5d0d  e(len(y) - 1))].
+0001a7a0: 0a20 2020 2072 6574 7572 6e20 6e70 2e73  .    return np.s
+0001a7b0: 756d 280d 0a20 2020 2020 2020 206e 702e  um(..        np.
+0001a7c0: 6e61 6e6d 6561 6e28 0d0a 2020 2020 2020  nanmean(..      
+0001a7d0: 2020 2020 2020 6e70 2e77 6865 7265 280d        np.where(.
+0001a7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a7f0: 206e 702e 7369 676e 2846 202d 206c 6173   np.sign(F - las
+0001a800: 745f 6f66 5f61 7272 6179 2920 3d3d 206e  t_of_array) == n
+0001a810: 702e 7369 676e 2841 202d 206c 6173 745f  p.sign(A - last_
+0001a820: 6f66 5f61 7272 6179 292c 0d0a 2020 2020  of_array),..    
+0001a830: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
+0001a840: 6273 2841 202d 2046 292c 0d0a 2020 2020  bs(A - F),..    
+0001a850: 2020 2020 2020 2020 2020 2020 286e 702e              (np.
+0001a860: 6162 7328 4120 2d20 4629 202b 2031 2920  abs(A - F) + 1) 
+0001a870: 2a2a 2032 2c0d 0a20 2020 2020 2020 2020  ** 2,..         
+0001a880: 2020 2029 2c0d 0a20 2020 2020 2020 2020     ),..         
+0001a890: 2020 2061 7869 733d 302c 0d0a 2020 2020     axis=0,..    
+0001a8a0: 2020 2020 290d 0a20 2020 2029 0d0a 0d0a      )..    )....
+0001a8b0: 0d0a 6465 6620 636f 7374 5f66 756e 6374  ..def cost_funct
+0001a8c0: 696f 6e5f 7175 616e 7469 6c65 2870 6172  ion_quantile(par
+0001a8d0: 616d 732c 2058 2c20 792c 2071 3d30 2e39  ams, X, y, q=0.9
+0001a8e0: 293a 0d0a 2020 2020 6375 7420 3d20 696e  ):..    cut = in
+0001a8f0: 7428 792e 7368 6170 655b 305d 202a 2071  t(y.shape[0] * q
+0001a900: 290d 0a20 2020 2072 6574 7572 6e20 6e70  )..    return np
+0001a910: 2e73 756d 280d 0a20 2020 2020 2020 206e  .sum(..        n
+0001a920: 702e 7061 7274 6974 696f 6e28 0d0a 2020  p.partition(..  
+0001a930: 2020 2020 2020 2020 2020 6e70 2e61 6273            np.abs
+0001a940: 2879 202d 206e 702e 646f 7428 582c 2070  (y - np.dot(X, p
+0001a950: 6172 616d 732e 7265 7368 6170 6528 582e  arams.reshape(X.
+0001a960: 7368 6170 655b 315d 2c20 792e 7368 6170  shape[1], y.shap
+0001a970: 655b 315d 2929 292c 2063 7574 2c20 6178  e[1]))), cut, ax
+0001a980: 6973 3d30 0d0a 2020 2020 2020 2020 295b  is=0..        )[
+0001a990: 303a 6375 745d 0d0a 2020 2020 290d 0a0d  0:cut]..    )...
+0001a9a0: 0a0d 0a64 6566 2063 6f73 745f 6675 6e63  ...def cost_func
+0001a9b0: 7469 6f6e 5f6c 3228 7061 7261 6d73 2c20  tion_l2(params, 
+0001a9c0: 582c 2079 293a 0d0a 2020 2020 7265 7475  X, y):..    retu
+0001a9d0: 726e 206e 702e 6c69 6e61 6c67 2e6e 6f72  rn np.linalg.nor
+0001a9e0: 6d28 7920 2d20 6e70 2e64 6f74 2858 2c20  m(y - np.dot(X, 
+0001a9f0: 7061 7261 6d73 2e72 6573 6861 7065 2858  params.reshape(X
+0001aa00: 2e73 6861 7065 5b31 5d2c 2079 2e73 6861  .shape[1], y.sha
+0001aa10: 7065 5b31 5d29 2929 0d0a 0d0a 0d0a 2320  pe[1])))......# 
+0001aa20: 636f 756c 6420 646f 2070 6172 7469 616c  could do partial
+0001aa30: 2070 6f6f 6c69 6e67 2062 7920 6d69 6e69   pooling by mini
+0001aa40: 6d69 7a69 6e67 2061 2066 756e 6374 696f  mizing a functio
+0001aa50: 6e20 7468 6174 206d 6978 6573 2073 6861  n that mixes sha
+0001aa60: 7265 6420 616e 6420 756e 7368 6172 6564  red and unshared
+0001aa70: 2063 6f65 6666 6963 6965 6e74 7320 286d   coefficients (m
+0001aa80: 756c 7469 706c 6963 6174 6976 6529 0d0a  ultiplicative)..
+0001aa90: 6465 6620 6c73 7473 715f 6d69 6e69 6d69  def lstsq_minimi
+0001aaa0: 7a65 2858 2c20 792c 206d 6178 6974 6572  ze(X, y, maxiter
+0001aab0: 3d31 3530 3030 2c20 636f 7374 5f66 756e  =15000, cost_fun
+0001aac0: 6374 696f 6e3d 226c 3122 293a 0d0a 2020  ction="l1"):..  
+0001aad0: 2020 2222 2241 6e79 2063 6f73 7420 6675    """Any cost fu
+0001aae0: 6e63 7469 6f6e 2076 6572 7369 6f6e 206f  nction version o
+0001aaf0: 6620 6c69 6e20 7265 672e 2222 220d 0a20  f lin reg.""".. 
+0001ab00: 2020 2023 2073 7461 7274 2077 6974 6820     # start with 
+0001ab10: 6c73 7473 7120 6669 7420 6173 2065 7374  lstsq fit as est
+0001ab20: 696d 6174 6564 2070 6f69 6e74 0d0a 2020  imated point..  
+0001ab30: 2020 7830 203d 206c 7374 7371 5f73 6f6c    x0 = lstsq_sol
+0001ab40: 7665 2858 2c20 7929 2e66 6c61 7474 656e  ve(X, y).flatten
+0001ab50: 2829 0d0a 2020 2020 2320 6173 7375 6d69  ()..    # assumi
+0001ab60: 6e67 2073 6361 6c65 642c 2074 6865 7365  ng scaled, these
+0001ab70: 2073 686f 756c 6420 6265 2072 6561 736f   should be reaso
+0001ab80: 6e61 626c 6520 626f 756e 6473 0d0a 2020  nable bounds..  
+0001ab90: 2020 626f 756e 6473 203d 205b 282d 3130    bounds = [(-10
+0001aba0: 2c20 3130 2920 666f 7220 7820 696e 2078  , 10) for x in x
+0001abb0: 305d 0d0a 2020 2020 6966 2063 6f73 745f  0]..    if cost_
+0001abc0: 6675 6e63 7469 6f6e 203d 3d20 2264 7761  function == "dwa
+0001abd0: 6522 3a0d 0a20 2020 2020 2020 2062 6f75  e":..        bou
+0001abe0: 6e64 7320 3d20 5b28 2d30 2e35 2c20 3130  nds = [(-0.5, 10
+0001abf0: 2920 666f 7220 7820 696e 2078 305d 0d0a  ) for x in x0]..
+0001ac00: 2020 2020 2020 2020 636f 7374 5f66 756e          cost_fun
+0001ac10: 6320 3d20 636f 7374 5f66 756e 6374 696f  c = cost_functio
+0001ac20: 6e5f 6477 6165 0d0a 2020 2020 656c 6966  n_dwae..    elif
+0001ac30: 2063 6f73 745f 6675 6e63 7469 6f6e 203d   cost_function =
+0001ac40: 3d20 2271 7561 6e74 696c 6522 3a0d 0a20  = "quantile":.. 
+0001ac50: 2020 2020 2020 2063 6f73 745f 6675 6e63         cost_func
+0001ac60: 203d 2063 6f73 745f 6675 6e63 7469 6f6e   = cost_function
+0001ac70: 5f71 7561 6e74 696c 650d 0a20 2020 2065  _quantile..    e
+0001ac80: 6c69 6620 636f 7374 5f66 756e 6374 696f  lif cost_functio
+0001ac90: 6e20 3d3d 2022 6c31 5f70 6f73 6974 6976  n == "l1_positiv
+0001aca0: 6522 3a0d 0a20 2020 2020 2020 2062 6f75  e":..        bou
+0001acb0: 6e64 7320 3d20 5b28 302c 2031 3029 2066  nds = [(0, 10) f
+0001acc0: 6f72 2078 2069 6e20 7830 5d0d 0a20 2020  or x in x0]..   
+0001acd0: 2020 2020 2063 6f73 745f 6675 6e63 203d       cost_func =
+0001ace0: 2063 6f73 745f 6675 6e63 7469 6f6e 5f6c   cost_function_l
+0001acf0: 310d 0a20 2020 2065 6c73 653a 0d0a 2020  1..    else:..  
+0001ad00: 2020 2020 2020 636f 7374 5f66 756e 6320        cost_func 
+0001ad10: 3d20 636f 7374 5f66 756e 6374 696f 6e5f  = cost_function_
+0001ad20: 6c31 0d0a 2020 2020 7265 7475 726e 206d  l1..    return m
+0001ad30: 696e 696d 697a 6528 0d0a 2020 2020 2020  inimize(..      
+0001ad40: 2020 636f 7374 5f66 756e 632c 2078 302c    cost_func, x0,
+0001ad50: 2061 7267 733d 2858 2c20 7929 2c20 626f   args=(X, y), bo
+0001ad60: 756e 6473 3d62 6f75 6e64 732c 206f 7074  unds=bounds, opt
+0001ad70: 696f 6e73 3d7b 276d 6178 6974 6572 273a  ions={'maxiter':
+0001ad80: 206d 6178 6974 6572 7d0d 0a20 2020 2029   maxiter}..    )
+0001ad90: 2e78 2e72 6573 6861 7065 2858 2e73 6861  .x.reshape(X.sha
+0001ada0: 7065 5b31 5d2c 2079 2e73 6861 7065 5b31  pe[1], y.shape[1
+0001adb0: 5d29 0d0a 0d0a 0d0a 6465 6620 6c69 6e65  ])......def line
+0001adc0: 6172 5f6d 6f64 656c 2878 2c20 792c 2070  ar_model(x, y, p
+0001add0: 6172 616d 7329 3a0d 0a20 2020 206d 6f64  arams):..    mod
+0001ade0: 656c 5f74 7970 6520 3d20 7061 7261 6d73  el_type = params
+0001adf0: 2e67 6574 2822 6d6f 6465 6c22 2c20 226c  .get("model", "l
+0001ae00: 7374 7371 2229 0d0a 2020 2020 6c61 6d62  stsq")..    lamb
+0001ae10: 6420 3d20 7061 7261 6d73 2e67 6574 2822  d = params.get("
+0001ae20: 6c61 6d62 6461 222c 204e 6f6e 6529 0d0a  lambda", None)..
+0001ae30: 2020 2020 7265 6320 3d20 7061 7261 6d73      rec = params
+0001ae40: 2e67 6574 2822 7265 6365 6e63 795f 7765  .get("recency_we
+0001ae50: 6967 6874 696e 6722 2c20 4e6f 6e65 290d  ighting", None).
+0001ae60: 0a20 2020 2069 6620 6c61 6d62 6420 6973  .    if lambd is
+0001ae70: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+0001ae80: 2020 2020 6964 5f6d 6174 203d 206e 702e      id_mat = np.
+0001ae90: 7a65 726f 7328 2878 2e73 6861 7065 5b31  zeros((x.shape[1
+0001aea0: 5d2c 2078 2e73 6861 7065 5b31 5d29 290d  ], x.shape[1])).
+0001aeb0: 0a20 2020 2020 2020 206e 702e 6669 6c6c  .        np.fill
+0001aec0: 5f64 6961 676f 6e61 6c28 6964 5f6d 6174  _diagonal(id_mat
+0001aed0: 2c20 3129 0d0a 2020 2020 2020 2020 6964  , 1)..        id
+0001aee0: 5f6d 6174 5b30 2c20 305d 203d 2030 0d0a  _mat[0, 0] = 0..
+0001aef0: 2020 2020 6966 2072 6563 2069 7320 6e6f      if rec is no
+0001af00: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0001af10: 2077 6569 6768 7473 203d 2028 6e70 2e61   weights = (np.a
+0001af20: 7261 6e67 6528 6c65 6e28 7829 2920 2b20  range(len(x)) + 
+0001af30: 3129 202a 2a20 7265 6320 2023 2030 2e30  1) ** rec  # 0.0
+0001af40: 3520 2d20 302e 3235 0d0a 2020 2020 2020  5 - 0.25..      
+0001af50: 2020 7820 3d20 7820 2a20 7765 6967 6874    x = x * weight
+0001af60: 735b 2e2e 2e2c 204e 6f6e 655d 0d0a 2020  s[..., None]..  
+0001af70: 2020 2020 2020 7920 3d20 6e70 2e61 7361        y = np.asa
+0001af80: 7272 6179 2879 2920 2a20 7765 6967 6874  rray(y) * weight
+0001af90: 735b 2e2e 2e2c 204e 6f6e 655d 0d0a 2020  s[..., None]..  
+0001afa0: 2020 6966 206d 6f64 656c 5f74 7970 6520    if model_type 
+0001afb0: 3d3d 2022 6c73 7473 7122 3a0d 0a20 2020  == "lstsq":..   
+0001afc0: 2020 2020 2069 6620 6c61 6d62 6420 6973       if lambd is
+0001afd0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+0001afe0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+0001aff0: 702e 6c69 6e61 6c67 2e6c 7374 7371 2878  p.linalg.lstsq(x
+0001b000: 2e54 2e64 6f74 2878 2920 2b20 6c61 6d62  .T.dot(x) + lamb
+0001b010: 6420 2a20 6964 5f6d 6174 2c20 782e 542e  d * id_mat, x.T.
+0001b020: 646f 7428 7929 2c20 7263 6f6e 643d 4e6f  dot(y), rcond=No
+0001b030: 6e65 295b 0d0a 2020 2020 2020 2020 2020  ne)[..          
+0001b040: 2020 2020 2020 300d 0a20 2020 2020 2020        0..       
+0001b050: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
+0001b060: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0001b070: 2020 2072 6574 7572 6e20 6e70 2e6c 696e     return np.lin
+0001b080: 616c 672e 6c73 7473 7128 782c 2079 2c20  alg.lstsq(x, y, 
+0001b090: 7263 6f6e 643d 4e6f 6e65 295b 305d 0d0a  rcond=None)[0]..
+0001b0a0: 2020 2020 656c 6966 206d 6f64 656c 5f74      elif model_t
+0001b0b0: 7970 6520 3d3d 2022 6c69 6e61 6c67 5f73  ype == "linalg_s
+0001b0c0: 6f6c 7665 223a 0d0a 2020 2020 2020 2020  olve":..        
+0001b0d0: 7265 7475 726e 206c 7374 7371 5f73 6f6c  return lstsq_sol
+0001b0e0: 7665 2878 2c20 792c 206c 616d 623d 6c61  ve(x, y, lamb=la
+0001b0f0: 6d62 642c 2069 6465 6e74 6974 795f 6d61  mbd, identity_ma
+0001b100: 7472 6978 3d69 645f 6d61 7429 0d0a 2020  trix=id_mat)..  
+0001b110: 2020 656c 6966 206d 6f64 656c 5f74 7970    elif model_typ
+0001b120: 6520 3d3d 2022 6c31 5f6e 6f72 6d22 3a0d  e == "l1_norm":.
+0001b130: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001b140: 6c73 7473 715f 6d69 6e69 6d69 7a65 280d  lstsq_minimize(.
+0001b150: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
+0001b160: 6173 6172 7261 7928 7829 2c0d 0a20 2020  asarray(x),..   
+0001b170: 2020 2020 2020 2020 206e 702e 6173 6172           np.asar
+0001b180: 7261 7928 7929 2c0d 0a20 2020 2020 2020  ray(y),..       
+0001b190: 2020 2020 206d 6178 6974 6572 3d70 6172       maxiter=par
+0001b1a0: 616d 732e 6765 7428 226d 6178 6974 6572  ams.get("maxiter
+0001b1b0: 222c 2031 3530 3030 292c 0d0a 2020 2020  ", 15000),..    
+0001b1c0: 2020 2020 2020 2020 636f 7374 5f66 756e          cost_fun
+0001b1d0: 6374 696f 6e3d 226c 3122 2c0d 0a20 2020  ction="l1",..   
+0001b1e0: 2020 2020 2029 0d0a 2020 2020 656c 6966       )..    elif
+0001b1f0: 206d 6f64 656c 5f74 7970 6520 3d3d 2022   model_type == "
+0001b200: 7175 616e 7469 6c65 5f6e 6f72 6d22 3a0d  quantile_norm":.
+0001b210: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001b220: 6c73 7473 715f 6d69 6e69 6d69 7a65 280d  lstsq_minimize(.
+0001b230: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
+0001b240: 6173 6172 7261 7928 7829 2c0d 0a20 2020  asarray(x),..   
+0001b250: 2020 2020 2020 2020 206e 702e 6173 6172           np.asar
+0001b260: 7261 7928 7929 2c0d 0a20 2020 2020 2020  ray(y),..       
+0001b270: 2020 2020 206d 6178 6974 6572 3d70 6172       maxiter=par
+0001b280: 616d 732e 6765 7428 226d 6178 6974 6572  ams.get("maxiter
+0001b290: 222c 2031 3530 3030 292c 0d0a 2020 2020  ", 15000),..    
+0001b2a0: 2020 2020 2020 2020 636f 7374 5f66 756e          cost_fun
+0001b2b0: 6374 696f 6e3d 2271 7561 6e74 696c 6522  ction="quantile"
+0001b2c0: 2c0d 0a20 2020 2020 2020 2029 0d0a 2020  ,..        )..  
+0001b2d0: 2020 656c 6966 206d 6f64 656c 5f74 7970    elif model_typ
+0001b2e0: 6520 3d3d 2022 6477 6165 5f6e 6f72 6d22  e == "dwae_norm"
+0001b2f0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+0001b300: 6e20 6c73 7473 715f 6d69 6e69 6d69 7a65  n lstsq_minimize
+0001b310: 280d 0a20 2020 2020 2020 2020 2020 206e  (..            n
+0001b320: 702e 6173 6172 7261 7928 7829 2c0d 0a20  p.asarray(x),.. 
+0001b330: 2020 2020 2020 2020 2020 206e 702e 6173             np.as
+0001b340: 6172 7261 7928 7929 2c0d 0a20 2020 2020  array(y),..     
+0001b350: 2020 2020 2020 206d 6178 6974 6572 3d70         maxiter=p
+0001b360: 6172 616d 732e 6765 7428 226d 6178 6974  arams.get("maxit
+0001b370: 6572 222c 2031 3530 3030 292c 0d0a 2020  er", 15000),..  
+0001b380: 2020 2020 2020 2020 2020 636f 7374 5f66            cost_f
+0001b390: 756e 6374 696f 6e3d 2264 7761 6522 2c0d  unction="dwae",.
+0001b3a0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+0001b3b0: 656c 6966 206d 6f64 656c 5f74 7970 6520  elif model_type 
+0001b3c0: 3d3d 2022 6c31 5f70 6f73 6974 6976 6522  == "l1_positive"
+0001b3d0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+0001b3e0: 6e20 6c73 7473 715f 6d69 6e69 6d69 7a65  n lstsq_minimize
+0001b3f0: 280d 0a20 2020 2020 2020 2020 2020 206e  (..            n
+0001b400: 702e 6173 6172 7261 7928 7829 2c0d 0a20  p.asarray(x),.. 
+0001b410: 2020 2020 2020 2020 2020 206e 702e 6173             np.as
+0001b420: 6172 7261 7928 7929 2c0d 0a20 2020 2020  array(y),..     
+0001b430: 2020 2020 2020 206d 6178 6974 6572 3d70         maxiter=p
+0001b440: 6172 616d 732e 6765 7428 226d 6178 6974  arams.get("maxit
+0001b450: 6572 222c 2031 3530 3030 292c 0d0a 2020  er", 15000),..  
+0001b460: 2020 2020 2020 2020 2020 636f 7374 5f66            cost_f
+0001b470: 756e 6374 696f 6e3d 226c 315f 706f 7369  unction="l1_posi
+0001b480: 7469 7665 222c 0d0a 2020 2020 2020 2020  tive",..        
+0001b490: 290d 0a20 2020 2065 6c73 653a 0d0a 2020  )..    else:..  
+0001b4a0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0001b4b0: 6545 7272 6f72 2822 6c69 6e65 6172 206d  eError("linear m
+0001b4c0: 6f64 656c 206e 6f74 2072 6563 6f67 6e69  odel not recogni
+0001b4d0: 7a65 6422 290d 0a0d 0a0d 0a23 2053 6561  zed")......# Sea
+0001b4e0: 736f 6e61 6c69 7469 6573 0d0a 2320 696e  sonalities..# in
+0001b4f0: 7465 7261 6374 696f 6e20 6566 6665 6374  teraction effect
+0001b500: 206f 6e6c 7920 6f6e 2066 6972 7374 2074   only on first t
+0001b510: 776f 2073 6561 736f 6e61 6c69 7469 6573  wo seasonalities
+0001b520: 2069 6620 6f72 6465 7220 6d61 7463 6865   if order matche
+0001b530: 730d 0a0d 0a23 2043 6174 6567 6f72 6963  s....# Categoric
+0001b540: 616c 2046 6561 7475 7265 730d 0a23 2028  al Features..# (
+0001b550: 6d75 6c74 6976 6172 6961 7465 2073 756d  multivariate sum
+0001b560: 6d61 7269 6573 2062 7920 6772 6f75 7029  maries by group)
+0001b570: 0d0a 0d0a 2320 7061 7374 2069 6d70 6163  ....# past impac
+0001b580: 7473 2028 6f70 7469 6f6e 2074 6f20 6e6f  ts (option to no
+0001b590: 7420 656e 666f 7263 652c 206f 6e6c 7920  t enforce, only 
+0001b5a0: 7368 6f77 290d 0a0d 0a23 2077 6861 7420  show)....# what 
+0001b5b0: 6973 2073 7469 6c6c 206e 6565 6465 643a  is still needed:
+0001b5c0: 0d0a 2320 6261 7965 7369 616e 206c 696e  ..# bayesian lin
+0001b5d0: 6561 7220 6d6f 6465 6c20 6f70 7469 6f6e  ear model option
+0001b5e0: 730d 0a23 206d 6f72 6520 6d75 6c74 6976  s..# more multiv
+0001b5f0: 6172 6961 7465 2073 756d 6d61 7269 6573  ariate summaries
+0001b600: 0d0a 2320 6164 6420 616e 6f6d 616c 7920  ..# add anomaly 
+0001b610: 636c 6173 7369 6669 6572 2074 6f20 666f  classifier to fo
+0001b620: 7265 6361 7374 0d0a 2320 7265 6669 6e65  recast..# refine
+0001b630: 2074 7261 6e73 666f 726d 6174 696f 6e73   transformations
+0001b640: 2061 6e64 206d 6f64 656c 7320 6765 6e65   and models gene
+0001b650: 7261 7465 6420 6279 2067 6574 5f6e 6577  rated by get_new
+0001b660: 5f70 6172 616d 730d 0a23 2072 6577 6569  _params..# rewei
+0001b670: 6768 7420 736f 206c 6f6f 7020 6973 206e  ght so loop is n
+0001b680: 6f74 2072 6571 7569 7265 6420 736f 206f  ot required so o
+0001b690: 6674 656e 0d0a 2320 7465 7374 2061 6e64  ften..# test and
+0001b6a0: 2062 7567 2066 6978 2065 7665 7279 7468   bug fix everyth
+0001b6b0: 696e 670d 0a23 206c 315f 6e6f 726d 2069  ing..# l1_norm i
+0001b6c0: 736e 2774 2077 6f72 6b69 6e67 0d0a 2320  sn't working..# 
+0001b6d0: 756e 6974 7465 7374 730d 0a0d 0a23 2063  unittests....# c
+0001b6e0: 6f75 6c64 2064 6f20 7061 7274 6961 6c20  ould do partial 
+0001b6f0: 706f 6f6c 696e 6720 6279 206d 696e 696d  pooling by minim
+0001b700: 697a 696e 6720 6120 6675 6e63 7469 6f6e  izing a function
+0001b710: 2074 6861 7420 6d69 7865 7320 7368 6172   that mixes shar
+0001b720: 6564 2061 6e64 2075 6e73 6861 7265 6420  ed and unshared 
+0001b730: 636f 6566 6669 6369 656e 7473 2028 6d75  coefficients (mu
+0001b740: 6c74 6970 6c69 6361 7469 7665 290d 0a0d  ltiplicative)...
+0001b750: 0a23 2073 6561 7263 6820 7370 6163 653a  .# search space:
+0001b760: 0d0a 2320 6661 7374 206f 6e20 6c73 7473  ..# fast on lsts
+0001b770: 7173 206d 6f64 656c 0d0a 2320 6675 6c6c  qs model..# full
+0001b780: 2073 6561 7263 6820 6f66 2070 7265 6465   search of prede
+0001b790: 6669 6e65 6420 6f70 7469 6f6e 730d 0a23  fined options..#
+0001b7a0: 2073 6369 7079 206d 696e 696d 697a 6520   scipy minimize 
+0001b7b0: 666f 7220 636f 6e74 696e 756f 7573 2070  for continuous p
+0001b7c0: 6172 616d 732c 206f 7220 6d61 7962 6520  arams, or maybe 
+0001b7d0: 696e 7428 7061 7261 6d29 2066 6f72 2064  int(param) for d
+0001b7e0: 6973 6372 6574 6520 746f 6f0d 0a23 206d  iscrete too..# m
+0001b7f0: 696e 696d 697a 6520 776f 726b 696e 6720  inimize working 
+0001b800: 666f 7220 726f 6c6c 696e 6720 7769 6e64  for rolling wind
+0001b810: 6f77 2073 697a 6520 6275 7420 6e6f 7420  ow size but not 
+0001b820: 666f 7220 7365 6173 6f6e 616c 6974 7920  for seasonality 
+0001b830: 2861 6374 7561 6c6c 7920 7072 6f62 6162  (actually probab
+0001b840: 6c79 2077 696e 646f 7720 6973 206f 7665  ly window is ove
+0001b850: 7266 6974 290d 0a23 2064 6f20 6974 2073  rfit)..# do it s
+0001b860: 7465 7077 6973 653a 0d0a 2320 6669 7273  tepwise:..# firs
+0001b870: 7420 6669 7420 7365 6173 6f6e 616c 6974  t fit seasonalit
+0001b880: 7920 2877 6974 6820 666c 6167 2072 6567  y (with flag reg
+0001b890: 7265 7373 6f72 7320 6275 7420 6e6f 7420  ressors but not 
+0001b8a0: 6f74 6865 7273 290d 0a23 2073 6563 6f6e  others)..# secon
+0001b8b0: 646c 7920 7363 616c 6572 7320 616e 6420  dly scalers and 
+0001b8c0: 7072 6570 726f 6365 7373 696e 6720 414e  preprocessing AN
+0001b8d0: 4420 616e 6f6d 616c 7920 6465 7465 6374  D anomaly detect
+0001b8e0: 696f 6e20 414e 4420 686f 6c69 6461 7920  ion AND holiday 
+0001b8f0: 6465 7465 6374 696f 6e0d 0a23 2070 6f73  detection..# pos
+0001b900: 7369 626c 7920 6164 6420 3372 6420 7365  sibly add 3rd se
+0001b910: 6173 6f6e 616c 6974 7920 6166 7465 7220  asonality after 
+0001b920: 7072 6570 726f 6365 7373 696e 670d 0a23  preprocessing..#
+0001b930: 2074 6869 7264 6c79 2072 6f6c 6c69 6e67   thirdly rolling
+0001b940: 2077 696e 646f 7720 7369 7a65 2028 696e   window size (in
+0001b950: 636c 7564 6520 726f 6c6c 696e 6720 7769  clude rolling wi
+0001b960: 6e64 6f77 2069 6e20 696e 6974 6961 6c20  ndow in initial 
+0001b970: 5820 6166 7465 7220 7468 6973 290d 0a23  X after this)..#
+0001b980: 2074 6865 6e20 7465 7374 2075 7365 7220   then test user 
+0001b990: 7265 6772 6573 736f 7220 616e 6420 7072  regressor and pr
+0001b9a0: 6570 726f 6365 7373 696e 670d 0a23 2074  eprocessing..# t
+0001b9b0: 6865 6e20 7465 7374 2041 5220 6c61 6773  hen test AR lags
+0001b9c0: 2028 646f 6e27 7420 7573 6520 6966 2025   (don't use if %
+0001b9d0: 2067 6169 6e20 6973 203c 2078 2025 290d   gain is < x %).
+0001b9e0: 0a23 206f 7220 6d61 7962 6520 7573 6520  .# or maybe use 
+0001b9f0: 6120 7275 6e74 696d 6520 7765 6967 6874  a runtime weight
+0001ba00: 696e 670d 0a23 2074 6865 6e20 6d75 6c74  ing..# then mult
+0001ba10: 6976 6172 6961 7465 2073 756d 6d61 7269  ivariate summari
+0001ba20: 6573 0d0a 2320 4649 4e41 4c4c 5920 636f  es..# FINALLY co
+0001ba30: 7661 7269 6174 6520 6c61 6773 2028 6665  variate lags (fe
+0001ba40: 6174 7572 6520 7365 6c65 6374 696f 6e20  ature selection 
+0001ba50: 6465 6669 6e69 7465 6c79 206e 6565 6465  definitely neede
+0001ba60: 6429 0d0a 0d0a 0d0a 6966 2046 616c 7365  d)......if False
+0001ba70: 3a0d 0a20 2020 2023 2074 6573 7420 686f  :..    # test ho
+0001ba80: 6c69 6461 7920 636f 756e 7472 6965 732c  liday countries,
+0001ba90: 2072 6567 7265 7373 6f72 732c 2069 6d70   regressors, imp
+0001baa0: 6163 7473 0d0a 2020 2020 6672 6f6d 2061  acts..    from a
+0001bab0: 7574 6f74 7320 696d 706f 7274 206c 6f61  utots import loa
+0001bac0: 645f 6461 696c 790d 0a20 2020 2069 6d70  d_daily..    imp
+0001bad0: 6f72 7420 6d61 7470 6c6f 746c 6962 2e70  ort matplotlib.p
+0001bae0: 7970 6c6f 7420 6173 2070 6c74 0d0a 0d0a  yplot as plt....
+0001baf0: 2020 2020 6361 7465 676f 7269 6361 6c5f      categorical_
+0001bb00: 6772 6f75 7073 203d 207b 0d0a 2020 2020  groups = {..    
+0001bb10: 2020 2020 2277 696b 695f 556e 6974 6564      "wiki_United
+0001bb20: 5f53 7461 7465 7322 3a20 2763 6f75 6e74  _States": 'count
+0001bb30: 7279 272c 0d0a 2020 2020 2020 2020 2277  ry',..        "w
+0001bb40: 696b 695f 4765 726d 616e 7922 3a20 2763  iki_Germany": 'c
+0001bb50: 6f75 6e74 7279 272c 0d0a 2020 2020 2020  ountry',..      
+0001bb60: 2020 2277 696b 695f 4a65 7375 7322 3a20    "wiki_Jesus": 
+0001bb70: 2768 6f6c 6964 6179 272c 0d0a 2020 2020  'holiday',..    
+0001bb80: 2020 2020 2277 696b 695f 4d69 6368 6165      "wiki_Michae
+0001bb90: 6c5f 4a61 636b 736f 6e22 3a20 2770 6572  l_Jackson": 'per
+0001bba0: 736f 6e27 2c0d 0a20 2020 2020 2020 2022  son',..        "
+0001bbb0: 7769 6b69 5f45 6173 7465 7222 3a20 2768  wiki_Easter": 'h
+0001bbc0: 6f6c 6964 6179 272c 0d0a 2020 2020 2020  oliday',..      
+0001bbd0: 2020 2277 696b 695f 4368 7269 7374 6d61    "wiki_Christma
+0001bbe0: 7322 3a20 2768 6f6c 6964 6179 272c 0d0a  s": 'holiday',..
+0001bbf0: 2020 2020 2020 2020 2277 696b 695f 4368          "wiki_Ch
+0001bc00: 696e 6573 655f 4e65 775f 5965 6172 223a  inese_New_Year":
+0001bc10: 2027 686f 6c69 6461 7927 2c0d 0a20 2020   'holiday',..   
+0001bc20: 2020 2020 2022 7769 6b69 5f54 6861 6e6b       "wiki_Thank
+0001bc30: 7367 6976 696e 6722 3a20 2768 6f6c 6964  sgiving": 'holid
+0001bc40: 6179 272c 0d0a 2020 2020 2020 2020 2277  ay',..        "w
+0001bc50: 696b 695f 456c 697a 6162 6574 685f 4949  iki_Elizabeth_II
+0001bc60: 223a 2027 7065 7273 6f6e 272c 0d0a 2020  ": 'person',..  
+0001bc70: 2020 2020 2020 2277 696b 695f 5769 6c6c        "wiki_Will
+0001bc80: 6961 6d5f 5368 616b 6573 7065 6172 6522  iam_Shakespeare"
+0001bc90: 3a20 2770 6572 736f 6e27 2c0d 0a20 2020  : 'person',..   
+0001bca0: 2020 2020 2022 7769 6b69 5f47 656f 7267       "wiki_Georg
+0001bcb0: 655f 5761 7368 696e 6774 6f6e 223a 2027  e_Washington": '
+0001bcc0: 7065 7273 6f6e 272c 0d0a 2020 2020 2020  person',..      
+0001bcd0: 2020 2277 696b 695f 436c 656f 7061 7472    "wiki_Cleopatr
+0001bce0: 6122 3a20 2770 6572 736f 6e27 2c0d 0a20  a": 'person',.. 
+0001bcf0: 2020 207d 0d0a 2020 2020 686f 6c69 6461     }..    holida
+0001bd00: 795f 636f 756e 7472 6965 7320 3d20 7b0d  y_countries = {.
+0001bd10: 0a20 2020 2020 2020 2027 7769 6b69 5f45  .        'wiki_E
+0001bd20: 6c69 7a61 6265 7468 5f49 4927 3a20 2775  lizabeth_II': 'u
+0001bd30: 6b27 2c0d 0a20 2020 2020 2020 2027 7769  k',..        'wi
+0001bd40: 6b69 5f55 6e69 7465 645f 5374 6174 6573  ki_United_States
+0001bd50: 273a 2027 7573 272c 0d0a 2020 2020 2020  ': 'us',..      
+0001bd60: 2020 2777 696b 695f 4765 726d 616e 7927    'wiki_Germany'
+0001bd70: 3a20 2764 6527 2c0d 0a20 2020 207d 0d0a  : 'de',..    }..
+0001bd80: 2020 2020 6466 5f64 6169 6c79 203d 206c      df_daily = l
+0001bd90: 6f61 645f 6461 696c 7928 6c6f 6e67 3d46  oad_daily(long=F
+0001bda0: 616c 7365 290d 0a20 2020 2023 2061 6464  alse)..    # add
+0001bdb0: 206e 616e 0d0a 2020 2020 6466 5f64 6169   nan..    df_dai
+0001bdc0: 6c79 2e69 6c6f 635b 3130 302c 203a 5d20  ly.iloc[100, :] 
+0001bdd0: 3d20 6e70 2e6e 616e 0d0a 2020 2020 666f  = np.nan..    fo
+0001bde0: 7265 6361 7374 5f6c 656e 6774 6820 3d20  recast_length = 
+0001bdf0: 3138 300d 0a20 2020 2069 6e63 6c75 6465  180..    include
+0001be00: 5f68 6973 746f 7279 203d 2054 7275 650d  _history = True.
+0001be10: 0a20 2020 2064 665f 7472 6169 6e20 3d20  .    df_train = 
+0001be20: 6466 5f64 6169 6c79 5b3a 2d66 6f72 6563  df_daily[:-forec
+0001be30: 6173 745f 6c65 6e67 7468 5d2e 696c 6f63  ast_length].iloc
+0001be40: 5b3a 2c20 313a 5d0d 0a20 2020 2064 665f  [:, 1:]..    df_
+0001be50: 7465 7374 203d 2064 665f 6461 696c 795b  test = df_daily[
+0001be60: 2d66 6f72 6563 6173 745f 6c65 6e67 7468  -forecast_length
+0001be70: 3a5d 2e69 6c6f 635b 3a2c 2031 3a5d 0d0a  :].iloc[:, 1:]..
+0001be80: 2020 2020 6661 6b65 5f72 6567 7220 3d20      fake_regr = 
+0001be90: 6466 5f64 6169 6c79 5b3a 2d66 6f72 6563  df_daily[:-forec
+0001bea0: 6173 745f 6c65 6e67 7468 5d2e 696c 6f63  ast_length].iloc
+0001beb0: 5b3a 2c20 303a 315d 0d0a 2020 2020 6661  [:, 0:1]..    fa
+0001bec0: 6b65 5f72 6567 725f 6663 7374 203d 2028  ke_regr_fcst = (
+0001bed0: 0d0a 2020 2020 2020 2020 6466 5f64 6169  ..        df_dai
+0001bee0: 6c79 2e69 6c6f 635b 3a2c 2030 3a31 5d0d  ly.iloc[:, 0:1].
+0001bef0: 0a20 2020 2020 2020 2069 6620 696e 636c  .        if incl
+0001bf00: 7564 655f 6869 7374 6f72 790d 0a20 2020  ude_history..   
+0001bf10: 2020 2020 2065 6c73 6520 6466 5f64 6169       else df_dai
+0001bf20: 6c79 5b2d 666f 7265 6361 7374 5f6c 656e  ly[-forecast_len
+0001bf30: 6774 683a 5d2e 696c 6f63 5b3a 2c20 303a  gth:].iloc[:, 0:
+0001bf40: 315d 0d0a 2020 2020 290d 0a20 2020 2066  1]..    )..    f
+0001bf50: 6c61 675f 7265 6772 6573 736f 7220 3d20  lag_regressor = 
+0001bf60: 7064 2e44 6174 6146 7261 6d65 2831 2c20  pd.DataFrame(1, 
+0001bf70: 696e 6465 783d 6661 6b65 5f72 6567 722e  index=fake_regr.
+0001bf80: 696e 6465 782c 2063 6f6c 756d 6e73 3d5b  index, columns=[
+0001bf90: 2266 6c61 675f 7465 7374 225d 290d 0a20  "flag_test"]).. 
+0001bfa0: 2020 2066 6c61 675f 7265 6772 6573 736f     flag_regresso
+0001bfb0: 725f 6663 7374 203d 2070 642e 4461 7461  r_fcst = pd.Data
+0001bfc0: 4672 616d 6528 0d0a 2020 2020 2020 2020  Frame(..        
+0001bfd0: 312c 2069 6e64 6578 3d66 616b 655f 7265  1, index=fake_re
+0001bfe0: 6772 5f66 6373 742e 696e 6465 782c 2063  gr_fcst.index, c
+0001bff0: 6f6c 756d 6e73 3d5b 2266 6c61 675f 7465  olumns=["flag_te
+0001c000: 7374 225d 0d0a 2020 2020 290d 0a20 2020  st"]..    )..   
+0001c010: 2072 6567 725f 7065 725f 7365 7269 6573   regr_per_series
+0001c020: 203d 207b 0d0a 2020 2020 2020 2020 7374   = {..        st
+0001c030: 7228 6466 5f74 7261 696e 2e63 6f6c 756d  r(df_train.colum
+0001c040: 6e73 5b30 5d29 3a20 7064 2e44 6174 6146  ns[0]): pd.DataF
+0001c050: 7261 6d65 280d 0a20 2020 2020 2020 2020  rame(..         
+0001c060: 2020 206e 702e 7261 6e64 6f6d 2e6e 6f72     np.random.nor
+0001c070: 6d61 6c28 7369 7a65 3d28 6c65 6e28 6466  mal(size=(len(df
+0001c080: 5f74 7261 696e 292c 2031 2929 2c20 696e  _train), 1)), in
+0001c090: 6465 783d 6466 5f74 7261 696e 2e69 6e64  dex=df_train.ind
+0001c0a0: 6578 0d0a 2020 2020 2020 2020 290d 0a20  ex..        ).. 
+0001c0b0: 2020 207d 0d0a 2020 2020 7265 6772 5f70     }..    regr_p
+0001c0c0: 6572 5f73 6572 6965 735f 6663 7374 203d  er_series_fcst =
+0001c0d0: 207b 0d0a 2020 2020 2020 2020 7374 7228   {..        str(
+0001c0e0: 6466 5f74 7261 696e 2e63 6f6c 756d 6e73  df_train.columns
+0001c0f0: 5b30 5d29 3a20 7064 2e44 6174 6146 7261  [0]): pd.DataFra
+0001c100: 6d65 280d 0a20 2020 2020 2020 2020 2020  me(..           
+0001c110: 206e 702e 7261 6e64 6f6d 2e6e 6f72 6d61   np.random.norma
+0001c120: 6c28 7369 7a65 3d28 666f 7265 6361 7374  l(size=(forecast
+0001c130: 5f6c 656e 6774 682c 2031 2929 2c20 696e  _length, 1)), in
+0001c140: 6465 783d 6466 5f74 6573 742e 696e 6465  dex=df_test.inde
+0001c150: 780d 0a20 2020 2020 2020 2029 0d0a 2020  x..        )..  
+0001c160: 2020 7d0d 0a20 2020 2063 6f6e 7374 7261    }..    constra
+0001c170: 696e 7420 3d20 7b0d 0a20 2020 2020 2020  int = {..       
+0001c180: 2027 636f 6e73 7472 6169 6e74 5f6d 6574   'constraint_met
+0001c190: 686f 6427 3a20 2771 7561 6e74 696c 6527  hod': 'quantile'
+0001c1a0: 2c0d 0a20 2020 2020 2020 2027 6c6f 7765  ,..        'lowe
+0001c1b0: 725f 636f 6e73 7472 6169 6e74 273a 2030  r_constraint': 0
+0001c1c0: 2c0d 0a20 2020 2020 2020 2027 7570 7065  ,..        'uppe
+0001c1d0: 725f 636f 6e73 7472 6169 6e74 273a 204e  r_constraint': N
+0001c1e0: 6f6e 652c 0d0a 2020 2020 2020 2020 2262  one,..        "b
+0001c1f0: 6f75 6e64 7322 3a20 5472 7565 2c0d 0a20  ounds": True,.. 
+0001c200: 2020 207d 0d0a 2020 2020 7061 7374 5f69     }..    past_i
+0001c210: 6d70 6163 7473 203d 2070 642e 4461 7461  mpacts = pd.Data
+0001c220: 4672 616d 6528 302c 2069 6e64 6578 3d64  Frame(0, index=d
+0001c230: 665f 7472 6169 6e2e 696e 6465 782c 2063  f_train.index, c
+0001c240: 6f6c 756d 6e73 3d64 665f 7472 6169 6e2e  olumns=df_train.
+0001c250: 636f 6c75 6d6e 7329 0d0a 2020 2020 7061  columns)..    pa
+0001c260: 7374 5f69 6d70 6163 7473 2e69 6c6f 635b  st_impacts.iloc[
+0001c270: 2d31 303a 2c20 305d 203d 206e 702e 6765  -10:, 0] = np.ge
+0001c280: 6f6d 7370 6163 6528 312c 2031 3029 5b30  omspace(1, 10)[0
+0001c290: 3a31 305d 202f 2031 3030 0d0a 2020 2020  :10] / 100..    
+0001c2a0: 7061 7374 5f69 6d70 6163 7473 2e69 6c6f  past_impacts.ilo
+0001c2b0: 635b 2d33 303a 2c20 2d31 5d20 3d20 6e70  c[-30:, -1] = np
+0001c2c0: 2e6c 696e 7370 6163 6528 312c 2031 3029  .linspace(1, 10)
+0001c2d0: 5b30 3a33 305d 202f 202d 3130 300d 0a20  [0:30] / -100.. 
+0001c2e0: 2020 2070 6173 745f 696d 7061 6374 735f     past_impacts_
+0001c2f0: 6675 6c6c 203d 2070 642e 4461 7461 4672  full = pd.DataFr
+0001c300: 616d 6528 302c 2069 6e64 6578 3d64 665f  ame(0, index=df_
+0001c310: 6461 696c 792e 696e 6465 782c 2063 6f6c  daily.index, col
+0001c320: 756d 6e73 3d64 665f 6461 696c 792e 636f  umns=df_daily.co
+0001c330: 6c75 6d6e 7329 0d0a 2020 2020 6675 7475  lumns)..    futu
+0001c340: 7265 5f69 6d70 6163 7473 203d 2070 642e  re_impacts = pd.
+0001c350: 4461 7461 4672 616d 6528 302c 2069 6e64  DataFrame(0, ind
+0001c360: 6578 3d64 665f 7465 7374 2e69 6e64 6578  ex=df_test.index
+0001c370: 2c20 636f 6c75 6d6e 733d 6466 5f74 6573  , columns=df_tes
+0001c380: 742e 636f 6c75 6d6e 7329 0d0a 2020 2020  t.columns)..    
+0001c390: 6675 7475 7265 5f69 6d70 6163 7473 2e69  future_impacts.i
+0001c3a0: 6c6f 635b 303a 3130 2c20 305d 203d 2028  loc[0:10, 0] = (
+0001c3b0: 6e70 2e6c 696e 7370 6163 6528 312c 2031  np.linspace(1, 1
+0001c3c0: 3029 5b30 3a31 305d 202b 2031 3029 202f  0)[0:10] + 10) /
+0001c3d0: 2031 3030 0d0a 0d0a 2020 2020 635f 7061   100....    c_pa
+0001c3e0: 7261 6d73 203d 2043 6173 7361 6e64 7261  rams = Cassandra
+0001c3f0: 2829 2e67 6574 5f6e 6577 5f70 6172 616d  ().get_new_param
+0001c400: 7328 290d 0a20 2020 2063 5f70 6172 616d  s()..    c_param
+0001c410: 735b 2772 6567 7265 7373 6f72 735f 7573  s['regressors_us
+0001c420: 6564 275d 203d 2046 616c 7365 0d0a 0d0a  ed'] = False....
+0001c430: 2020 2020 6d6f 6420 3d20 4361 7373 616e      mod = Cassan
+0001c440: 6472 6128 0d0a 2020 2020 2020 2020 6e5f  dra(..        n_
+0001c450: 6a6f 6273 3d31 2c0d 0a20 2020 2020 2020  jobs=1,..       
+0001c460: 202a 2a63 5f70 6172 616d 732c 0d0a 2020   **c_params,..  
+0001c470: 2020 2020 2020 636f 6e73 7472 6169 6e74        constraint
+0001c480: 3d63 6f6e 7374 7261 696e 742c 0d0a 2020  =constraint,..  
+0001c490: 2020 2020 2020 686f 6c69 6461 795f 636f        holiday_co
+0001c4a0: 756e 7472 6965 733d 686f 6c69 6461 795f  untries=holiday_
+0001c4b0: 636f 756e 7472 6965 732c 0d0a 2020 2020  countries,..    
+0001c4c0: 2020 2020 6d61 785f 6d75 6c74 6963 6f6c      max_multicol
+0001c4d0: 696e 6561 7269 7479 3d30 2e30 3030 312c  inearity=0.0001,
+0001c4e0: 0d0a 2020 2020 290d 0a20 2020 206d 6f64  ..    )..    mod
+0001c4f0: 2e66 6974 280d 0a20 2020 2020 2020 2064  .fit(..        d
+0001c500: 665f 7472 6169 6e2c 0d0a 2020 2020 2020  f_train,..      
+0001c510: 2020 6361 7465 676f 7269 6361 6c5f 6772    categorical_gr
+0001c520: 6f75 7073 3d63 6174 6567 6f72 6963 616c  oups=categorical
+0001c530: 5f67 726f 7570 732c 0d0a 2020 2020 2020  _groups,..      
+0001c540: 2020 6675 7475 7265 5f72 6567 7265 7373    future_regress
+0001c550: 6f72 3d66 616b 655f 7265 6772 2c0d 0a20  or=fake_regr,.. 
+0001c560: 2020 2020 2020 2072 6567 7265 7373 6f72         regressor
+0001c570: 5f70 6572 5f73 6572 6965 733d 7265 6772  _per_series=regr
+0001c580: 5f70 6572 5f73 6572 6965 732c 0d0a 2020  _per_series,..  
+0001c590: 2020 2020 2020 2320 7061 7374 5f69 6d70        # past_imp
+0001c5a0: 6163 7473 3d70 6173 745f 696d 7061 6374  acts=past_impact
+0001c5b0: 732c 0d0a 2020 2020 2020 2020 666c 6167  s,..        flag
+0001c5c0: 5f72 6567 7265 7373 6f72 733d 666c 6167  _regressors=flag
+0001c5d0: 5f72 6567 7265 7373 6f72 2c0d 0a20 2020  _regressor,..   
+0001c5e0: 2029 0d0a 2020 2020 7072 6564 203d 206d   )..    pred = m
+0001c5f0: 6f64 2e70 7265 6469 6374 280d 0a20 2020  od.predict(..   
+0001c600: 2020 2020 2066 6f72 6563 6173 745f 6c65       forecast_le
+0001c610: 6e67 7468 3d66 6f72 6563 6173 745f 6c65  ngth=forecast_le
+0001c620: 6e67 7468 2c0d 0a20 2020 2020 2020 2069  ngth,..        i
+0001c630: 6e63 6c75 6465 5f68 6973 746f 7279 3d69  nclude_history=i
+0001c640: 6e63 6c75 6465 5f68 6973 746f 7279 2c0d  nclude_history,.
+0001c650: 0a20 2020 2020 2020 2066 7574 7572 655f  .        future_
+0001c660: 7265 6772 6573 736f 723d 6661 6b65 5f72  regressor=fake_r
+0001c670: 6567 725f 6663 7374 2c0d 0a20 2020 2020  egr_fcst,..     
+0001c680: 2020 2072 6567 7265 7373 6f72 5f70 6572     regressor_per
+0001c690: 5f73 6572 6965 733d 7265 6772 5f70 6572  _series=regr_per
+0001c6a0: 5f73 6572 6965 735f 6663 7374 2c0d 0a20  _series_fcst,.. 
+0001c6b0: 2020 2020 2020 2066 7574 7572 655f 696d         future_im
+0001c6c0: 7061 6374 733d 6675 7475 7265 5f69 6d70  pacts=future_imp
+0001c6d0: 6163 7473 2c0d 0a20 2020 2020 2020 2066  acts,..        f
+0001c6e0: 6c61 675f 7265 6772 6573 736f 7273 3d66  lag_regressors=f
+0001c6f0: 6c61 675f 7265 6772 6573 736f 725f 6663  lag_regressor_fc
+0001c700: 7374 2c0d 0a20 2020 2020 2020 2069 6e63  st,..        inc
+0001c710: 6c75 6465 5f6f 7267 616e 6963 3d54 7275  lude_organic=Tru
+0001c720: 652c 0d0a 2020 2020 290d 0a20 2020 2072  e,..    )..    r
+0001c730: 6573 756c 7420 3d20 7072 6564 2e66 6f72  esult = pred.for
+0001c740: 6563 6173 740d 0a20 2020 2073 6572 6965  ecast..    serie
+0001c750: 7320 3d20 7261 6e64 6f6d 2e63 686f 6963  s = random.choic
+0001c760: 6528 6d6f 642e 636f 6c75 6d6e 5f6e 616d  e(mod.column_nam
+0001c770: 6573 290d 0a20 2020 2023 2073 6572 6965  es)..    # serie
+0001c780: 7320 3d20 2277 696b 695f 5065 7269 6f64  s = "wiki_Period
+0001c790: 6963 5f74 6162 6c65 220d 0a20 2020 2073  ic_table"..    s
+0001c7a0: 6572 6965 7320 3d20 2777 696b 695f 616c  eries = 'wiki_al
+0001c7b0: 6c27 0d0a 2020 2020 6d6f 642e 7265 6772  l'..    mod.regr
+0001c7c0: 6573 736f 7273 5f75 7365 640d 0a20 2020  essors_used..   
+0001c7d0: 206d 6f64 2e68 6f6c 6964 6179 5f63 6f75   mod.holiday_cou
+0001c7e0: 6e74 7269 6573 5f75 7365 640d 0a20 2020  ntries_used..   
+0001c7f0: 2077 6974 6820 706c 742e 7374 796c 652e   with plt.style.
+0001c800: 636f 6e74 6578 7428 2273 6561 626f 726e  context("seaborn
+0001c810: 2d77 6869 7465 2229 3a0d 0a20 2020 2020  -white"):..     
+0001c820: 2020 2073 7461 7274 5f64 6174 6520 3d20     start_date = 
+0001c830: 2261 7574 6f22 0d0a 2020 2020 2020 2020  "auto"..        
+0001c840: 6d6f 642e 706c 6f74 5f66 6f72 6563 6173  mod.plot_forecas
+0001c850: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+0001c860: 7072 6564 2c0d 0a20 2020 2020 2020 2020  pred,..         
+0001c870: 2020 2061 6374 7561 6c73 3d64 665f 6461     actuals=df_da
+0001c880: 696c 7920 6966 2069 6e63 6c75 6465 5f68  ily if include_h
+0001c890: 6973 746f 7279 2065 6c73 6520 6466 5f74  istory else df_t
+0001c8a0: 6573 742c 0d0a 2020 2020 2020 2020 2020  est,..          
+0001c8b0: 2020 7365 7269 6573 3d73 6572 6965 732c    series=series,
+0001c8c0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+0001c8d0: 6172 745f 6461 7465 3d73 7461 7274 5f64  art_date=start_d
+0001c8e0: 6174 652c 0d0a 2020 2020 2020 2020 290d  ate,..        ).
+0001c8f0: 0a0d 0a20 2020 2020 2020 2023 2070 6c74  ...        # plt
+0001c900: 2e73 686f 7728 290d 0a20 2020 2020 2020  .show()..       
+0001c910: 2023 2070 6c74 2e73 6176 6566 6967 2822   # plt.savefig("
+0001c920: 4361 7373 616e 6472 615f 666f 7265 6361  Cassandra_foreca
+0001c930: 7374 2e70 6e67 222c 2064 7069 3d33 3030  st.png", dpi=300
+0001c940: 290d 0a20 2020 2020 2020 2023 206d 6f64  )..        # mod
+0001c950: 2e70 6c6f 745f 636f 6d70 6f6e 656e 7473  .plot_components
+0001c960: 2870 7265 642c 2073 6572 6965 733d 7365  (pred, series=se
+0001c970: 7269 6573 2c20 746f 5f6f 7269 6769 6e5f  ries, to_origin_
+0001c980: 7370 6163 653d 4661 6c73 6529 0d0a 2020  space=False)..  
+0001c990: 2020 2020 2020 2320 706c 742e 7368 6f77        # plt.show
+0001c9a0: 2829 0d0a 2020 2020 2020 2020 6d6f 642e  ()..        mod.
+0001c9b0: 706c 6f74 5f63 6f6d 706f 6e65 6e74 7328  plot_components(
+0001c9c0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0001c9d0: 6564 2c20 7365 7269 6573 3d73 6572 6965  ed, series=serie
+0001c9e0: 732c 2074 6f5f 6f72 6967 696e 5f73 7061  s, to_origin_spa
+0001c9f0: 6365 3d54 7275 652c 2073 7461 7274 5f64  ce=True, start_d
+0001ca00: 6174 653d 7374 6172 745f 6461 7465 0d0a  ate=start_date..
+0001ca10: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0001ca20: 2020 2023 2070 6c74 2e73 6176 6566 6967     # plt.savefig
+0001ca30: 2822 4361 7373 616e 6472 615f 636f 6d70  ("Cassandra_comp
+0001ca40: 6f6e 656e 7473 332e 706e 6722 2c20 6470  onents3.png", dp
+0001ca50: 693d 3330 302c 2062 626f 785f 696e 6368  i=300, bbox_inch
+0001ca60: 6573 3d22 7469 6768 7422 290d 0a20 2020  es="tight")..   
+0001ca70: 2020 2020 2070 6c74 2e73 686f 7728 290d       plt.show().
+0001ca80: 0a20 2020 2020 2020 206d 6f64 2e70 6c6f  .        mod.plo
+0001ca90: 745f 7472 656e 6428 0d0a 2020 2020 2020  t_trend(..      
+0001caa0: 2020 2020 2020 7365 7269 6573 3d73 6572        series=ser
+0001cab0: 6965 732c 2076 6c69 6e65 3d72 6573 756c  ies, vline=resul
+0001cac0: 742e 696e 6465 785b 2d66 6f72 6563 6173  t.index[-forecas
+0001cad0: 745f 6c65 6e67 7468 5d2c 2073 7461 7274  t_length], start
+0001cae0: 5f64 6174 653d 7374 6172 745f 6461 7465  _date=start_date
+0001caf0: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+0001cb00: 2020 2020 2023 2070 6c74 2e73 6176 6566       # plt.savef
+0001cb10: 6967 2822 4361 7373 616e 6472 615f 7472  ig("Cassandra_tr
+0001cb20: 656e 642e 706e 6722 2c20 6470 693d 3330  end.png", dpi=30
+0001cb30: 302c 2062 626f 785f 696e 6368 6573 3d22  0, bbox_inches="
+0001cb40: 7469 6768 7422 290d 0a20 2020 2070 7265  tight")..    pre
+0001cb50: 642e 6576 616c 7561 7465 280d 0a20 2020  d.evaluate(..   
+0001cb60: 2020 2020 2064 665f 6461 696c 792e 7265       df_daily.re
+0001cb70: 696e 6465 7828 7265 7375 6c74 2e69 6e64  index(result.ind
+0001cb80: 6578 295b 6466 5f74 7261 696e 2e63 6f6c  ex)[df_train.col
+0001cb90: 756d 6e73 5d0d 0a20 2020 2020 2020 2069  umns]..        i
+0001cba0: 6620 696e 636c 7564 655f 6869 7374 6f72  f include_histor
+0001cbb0: 790d 0a20 2020 2020 2020 2065 6c73 6520  y..        else 
+0001cbc0: 6466 5f74 6573 745b 6466 5f74 7261 696e  df_test[df_train
+0001cbd0: 2e63 6f6c 756d 6e73 5d0d 0a20 2020 2029  .columns]..    )
+0001cbe0: 0d0a 2020 2020 7072 696e 7428 7072 6564  ..    print(pred
+0001cbf0: 2e61 7667 5f6d 6574 7269 6373 2e72 6f75  .avg_metrics.rou
+0001cc00: 6e64 2831 2929 0d0a 0d0a 2020 2020 2320  nd(1))....    # 
+0001cc10: 6966 206e 6f74 206d 6f64 2e72 6567 7265  if not mod.regre
+0001cc20: 7373 6f72 735f 7573 6564 3a0d 0a20 2020  ssors_used:..   
+0001cc30: 2064 6174 6573 203d 2064 665f 6461 696c   dates = df_dail
+0001cc40: 792e 696e 6465 782e 756e 696f 6e28 0d0a  y.index.union(..
+0001cc50: 2020 2020 2020 2020 6d6f 642e 6372 6561          mod.crea
+0001cc60: 7465 5f66 6f72 6563 6173 745f 696e 6465  te_forecast_inde
+0001cc70: 7828 666f 7265 6361 7374 5f6c 656e 6774  x(forecast_lengt
+0001cc80: 682c 206c 6173 745f 6461 7465 3d64 665f  h, last_date=df_
+0001cc90: 6461 696c 792e 696e 6465 785b 2d31 5d29  daily.index[-1])
+0001cca0: 0d0a 2020 2020 290d 0a20 2020 2072 6567  ..    )..    reg
+0001ccb0: 725f 7073 203d 207b 0d0a 2020 2020 2020  r_ps = {..      
+0001ccc0: 2020 2777 696b 695f 4765 726d 616e 7927    'wiki_Germany'
+0001ccd0: 3a20 7265 6772 5f70 6572 5f73 6572 6965  : regr_per_serie
+0001cce0: 735f 6663 7374 5b27 7769 6b69 5f47 6572  s_fcst['wiki_Ger
+0001ccf0: 6d61 6e79 275d 2e72 6569 6e64 6578 280d  many'].reindex(.
+0001cd00: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0001cd10: 6573 2c20 6669 6c6c 5f76 616c 7565 3d30  es, fill_value=0
+0001cd20: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+0001cd30: 207d 0d0a 2020 2020 2320 4e4f 5420 5041   }..    # NOT PA
+0001cd40: 5353 494e 4720 5052 4f50 4552 2052 4547  SSING PROPER REG
+0001cd50: 5245 5353 4f52 5320 4845 5245 2028 7a65  RESSORS HERE (ze
+0001cd60: 726f 2066 696c 6c29 2053 4f20 4d41 5920  ro fill) SO MAY 
+0001cd70: 4c4f 4f4b 204f 4646 2049 4620 5245 4752  LOOK OFF IF REGR
+0001cd80: 4553 534f 5253 5f55 5345 440d 0a20 2020  ESSORS_USED..   
+0001cd90: 2070 7265 6432 203d 206d 6f64 2e70 7265   pred2 = mod.pre
+0001cda0: 6469 6374 280d 0a20 2020 2020 2020 2066  dict(..        f
+0001cdb0: 6f72 6563 6173 745f 6c65 6e67 7468 3d66  orecast_length=f
+0001cdc0: 6f72 6563 6173 745f 6c65 6e67 7468 2c0d  orecast_length,.
+0001cdd0: 0a20 2020 2020 2020 2069 6e63 6c75 6465  .        include
+0001cde0: 5f68 6973 746f 7279 3d54 7275 652c 0d0a  _history=True,..
+0001cdf0: 2020 2020 2020 2020 6e65 775f 6466 3d64          new_df=d
+0001ce00: 665f 6461 696c 795b 6466 5f74 7261 696e  f_daily[df_train
+0001ce10: 2e63 6f6c 756d 6e73 5d2c 0d0a 2020 2020  .columns],..    
+0001ce20: 2020 2020 666c 6167 5f72 6567 7265 7373      flag_regress
+0001ce30: 6f72 733d 666c 6167 5f72 6567 7265 7373  ors=flag_regress
+0001ce40: 6f72 5f66 6373 742e 7265 696e 6465 7828  or_fcst.reindex(
+0001ce50: 6461 7465 732c 2066 696c 6c5f 7661 6c75  dates, fill_valu
+0001ce60: 653d 3029 2c0d 0a20 2020 2020 2020 2066  e=0),..        f
+0001ce70: 7574 7572 655f 7265 6772 6573 736f 723d  uture_regressor=
+0001ce80: 6661 6b65 5f72 6567 725f 6663 7374 2e72  fake_regr_fcst.r
+0001ce90: 6569 6e64 6578 2864 6174 6573 2c20 6669  eindex(dates, fi
+0001cea0: 6c6c 5f76 616c 7565 3d30 292c 0d0a 2020  ll_value=0),..  
+0001ceb0: 2020 2020 2020 7265 6772 6573 736f 725f        regressor_
+0001cec0: 7065 725f 7365 7269 6573 3d72 6567 725f  per_series=regr_
+0001ced0: 7073 2c0d 0a20 2020 2020 2020 2070 6173  ps,..        pas
+0001cee0: 745f 696d 7061 6374 733d 7061 7374 5f69  t_impacts=past_i
+0001cef0: 6d70 6163 7473 5f66 756c 6c5b 6466 5f74  mpacts_full[df_t
+0001cf00: 7261 696e 2e63 6f6c 756d 6e73 5d2c 0d0a  rain.columns],..
+0001cf10: 2020 2020 290d 0a20 2020 206d 6f64 2e70      )..    mod.p
+0001cf20: 6c6f 745f 666f 7265 6361 7374 2870 7265  lot_forecast(pre
+0001cf30: 6432 2c20 6163 7475 616c 733d 6466 5f64  d2, actuals=df_d
+0001cf40: 6169 6c79 2c20 7365 7269 6573 3d73 6572  aily, series=ser
+0001cf50: 6965 732c 2073 7461 7274 5f64 6174 653d  ies, start_date=
+0001cf60: 7374 6172 745f 6461 7465 290d 0a20 2020  start_date)..   
+0001cf70: 206d 6f64 2e72 6574 7572 6e5f 636f 6d70   mod.return_comp
+0001cf80: 6f6e 656e 7473 2829 0d0a 2020 2020 2320  onents()..    # 
+0001cf90: 616e 6420 7472 7920 7265 7472 6169 6e69  and try retraini
+0001cfa0: 6e67 2062 6163 6b20 7769 7468 2073 686f  ng back with sho
+0001cfb0: 7274 6572 2064 6174 6173 6574 2061 6e64  rter dataset and
+0001cfc0: 2073 6565 2069 6620 6974 206d 6174 6368   see if it match
+0001cfd0: 6573 2070 7269 6f72 0d0a 2020 2020 6d6f  es prior..    mo
+0001cfe0: 642e 6669 745f 6461 7461 2864 665f 7472  d.fit_data(df_tr
+0001cff0: 6169 6e2c 2070 6173 745f 696d 7061 6374  ain, past_impact
+0001d000: 733d 7061 7374 5f69 6d70 6163 7473 5b64  s=past_impacts[d
+0001d010: 665f 7472 6169 6e2e 636f 6c75 6d6e 735d  f_train.columns]
+0001d020: 290d 0a20 2020 2070 7265 6433 203d 206d  )..    pred3 = m
+0001d030: 6f64 2e70 7265 6469 6374 280d 0a20 2020  od.predict(..   
+0001d040: 2020 2020 2066 6f72 6563 6173 745f 6c65       forecast_le
+0001d050: 6e67 7468 3d66 6f72 6563 6173 745f 6c65  ngth=forecast_le
+0001d060: 6e67 7468 2c0d 0a20 2020 2020 2020 2069  ngth,..        i
+0001d070: 6e63 6c75 6465 5f68 6973 746f 7279 3d54  nclude_history=T
+0001d080: 7275 652c 0d0a 2020 2020 2020 2020 666c  rue,..        fl
+0001d090: 6167 5f72 6567 7265 7373 6f72 733d 666c  ag_regressors=fl
+0001d0a0: 6167 5f72 6567 7265 7373 6f72 5f66 6373  ag_regressor_fcs
+0001d0b0: 742e 7265 696e 6465 7828 6466 5f64 6169  t.reindex(df_dai
+0001d0c0: 6c79 2e69 6e64 6578 2c20 6669 6c6c 5f76  ly.index, fill_v
+0001d0d0: 616c 7565 3d30 292c 0d0a 2020 2020 2020  alue=0),..      
+0001d0e0: 2020 6675 7475 7265 5f72 6567 7265 7373    future_regress
+0001d0f0: 6f72 3d66 616b 655f 7265 6772 5f66 6373  or=fake_regr_fcs
+0001d100: 742e 7265 696e 6465 7828 6466 5f64 6169  t.reindex(df_dai
+0001d110: 6c79 2e69 6e64 6578 2c20 6669 6c6c 5f76  ly.index, fill_v
+0001d120: 616c 7565 3d30 292c 0d0a 2020 2020 2020  alue=0),..      
+0001d130: 2020 7265 6772 6573 736f 725f 7065 725f    regressor_per_
+0001d140: 7365 7269 6573 3d72 6567 725f 7073 2c0d  series=regr_ps,.
+0001d150: 0a20 2020 2020 2020 2066 7574 7572 655f  .        future_
+0001d160: 696d 7061 6374 733d 6675 7475 7265 5f69  impacts=future_i
+0001d170: 6d70 6163 7473 2c0d 0a20 2020 2029 0d0a  mpacts,..    )..
+0001d180: 2020 2020 6d6f 642e 706c 6f74 5f66 6f72      mod.plot_for
+0001d190: 6563 6173 7428 0d0a 2020 2020 2020 2020  ecast(..        
+0001d1a0: 7072 6564 332c 0d0a 2020 2020 2020 2020  pred3,..        
+0001d1b0: 6163 7475 616c 733d 6466 5f64 6169 6c79  actuals=df_daily
+0001d1c0: 2069 6620 696e 636c 7564 655f 6869 7374   if include_hist
+0001d1d0: 6f72 7920 656c 7365 2064 665f 7465 7374  ory else df_test
+0001d1e0: 2c0d 0a20 2020 2020 2020 2073 6572 6965  ,..        serie
+0001d1f0: 733d 7365 7269 6573 2c0d 0a20 2020 2020  s=series,..     
+0001d200: 2020 2073 7461 7274 5f64 6174 653d 7374     start_date=st
+0001d210: 6172 745f 6461 7465 2c0d 0a20 2020 2029  art_date,..    )
+0001d220: 0d0a 0d0a 2020 2020 7072 696e 7428 635f  ....    print(c_
+0001d230: 7061 7261 6d73 5b27 7472 656e 645f 6d6f  params['trend_mo
+0001d240: 6465 6c27 5d29 0d0a 0d0a 2320 4b6e 6f77  del'])....# Know
+0001d250: 6e20 616e 6420 506f 7373 6962 6c65 2049  n and Possible I
+0001d260: 5353 5545 533a 0d0a 2320 4d75 6c74 6976  SSUES:..# Multiv
+0001d270: 6172 6961 7465 2066 6561 7475 7265 2077  ariate feature w
+0001d280: 6f72 6b69 6e67 206f 7220 6e6f 743f 0d0a  orking or not?..
+0001d290: 2320 6d75 6c74 6970 6c69 6361 7469 7665  # multiplicative
+0001d2a0: 2073 6561 736f 6e61 6c69 7479 0d0a 0d0a   seasonality....
+0001d2b0: 0d0a 2320 4175 746f 6d61 7469 6f6e 0d0a  ..# Automation..
+0001d2c0: 2320 616c 6c6f 7720 736f 6d65 2063 6f6e  # allow some con
+0001d2d0: 6669 6720 696e 7075 7473 2c20 6f72 2061  fig inputs, or a
+0001d2e0: 7574 6f6d 6174 6564 2066 6974 0d0a 2320  utomated fit..# 
+0001d2f0: 6f75 7470 7574 2074 6f20 7461 626c 650d  output to table.
+0001d300: 0a23 2063 6f6d 7061 7265 2063 6f65 6666  .# compare coeff
+0001d310: 6963 6965 6e74 7320 6368 616e 6765 206f  icients change o
+0001d320: 7665 7220 7469 6d65 2c20 6163 6375 7261  ver time, accura
+0001d330: 6379 206f 7665 7220 7469 6d65 0d0a 2320  cy over time..# 
+0001d340: 636f 6d70 6172 696e 6720 6469 6666 6572  comparing differ
+0001d350: 656e 7420 736f 7572 6365 733f 2061 6e64  ent sources? and
+0001d360: 2f6f 7220 616c 6c6f 7769 6e67 206f 6e65  /or allowing one
+0001d370: 2066 6f72 6563 6173 7420 746f 2062 6520   forecast to be 
+0001d380: 7573 6564 2061 7320 6120 7265 6772 6573  used as a regres
+0001d390: 736f 7220 666f 7220 616e 6f74 6865 720d  sor for another.
+0001d3a0: 0a23 2077 6f75 6c64 2061 6c6c 6f77 2066  .# would allow f
+0001d3b0: 6f72 2065 6172 6c69 6572 2064 6574 6563  or earlier detec
+0001d3c0: 7469 6f6e 206f 6620 6272 6f6b 656e 2063  tion of broken c
+0001d3d0: 6f6e 6e65 6374 696f 6e73 0d0a 0d0a 2222  onnections....""
+0001d3e0: 220d 0a61 7820 3d20 7072 6564 2e70 6c6f  "..ax = pred.plo
+0001d3f0: 7428 6466 5f64 6169 6c79 2069 6620 696e  t(df_daily if in
+0001d400: 636c 7564 655f 6869 7374 6f72 7920 656c  clude_history el
+0001d410: 7365 2064 665f 7465 7374 2c20 7365 7269  se df_test, seri
+0001d420: 6573 3d73 6572 6965 732c 2076 6c69 6e65  es=series, vline
+0001d430: 3d64 665f 7465 7374 2e69 6e64 6578 5b30  =df_test.index[0
+0001d440: 5d2c 2073 7461 7274 5f64 6174 653d 7374  ], start_date=st
+0001d450: 6172 745f 6461 7465 290d 0a68 616e 646c  art_date)..handl
+0001d460: 6573 2c20 6c61 6265 6c73 203d 2061 782e  es, labels = ax.
+0001d470: 6765 745f 6c65 6765 6e64 5f68 616e 646c  get_legend_handl
+0001d480: 6573 5f6c 6162 656c 7328 290d 0a69 6620  es_labels()..if 
+0001d490: 6d6f 642e 616e 6f6d 616c 795f 6465 7465  mod.anomaly_dete
+0001d4a0: 6374 6f72 3a0d 0a20 2020 2069 6620 6d6f  ctor:..    if mo
+0001d4b0: 642e 616e 6f6d 616c 795f 6465 7465 6374  d.anomaly_detect
+0001d4c0: 6f72 2e6f 7574 7075 7420 3d3d 2022 756e  or.output == "un
+0001d4d0: 6976 6172 6961 7465 223a 0d0a 2020 2020  ivariate":..    
+0001d4e0: 2020 2020 695f 616e 6f6d 203d 206d 6f64      i_anom = mod
+0001d4f0: 2e61 6e6f 6d61 6c79 5f64 6574 6563 746f  .anomaly_detecto
+0001d500: 722e 616e 6f6d 616c 6965 732e 696e 6465  r.anomalies.inde
+0001d510: 785b 6d6f 642e 616e 6f6d 616c 795f 6465  x[mod.anomaly_de
+0001d520: 7465 6374 6f72 2e61 6e6f 6d61 6c69 6573  tector.anomalies
+0001d530: 2e69 6c6f 635b 3a2c 2030 5d20 3d3d 202d  .iloc[:, 0] == -
+0001d540: 315d 0d0a 2020 2020 656c 7365 3a0d 0a20  1]..    else:.. 
+0001d550: 2020 2020 2020 2073 6572 6965 735f 616e         series_an
+0001d560: 6f6d 203d 206d 6f64 2e61 6e6f 6d61 6c79  om = mod.anomaly
+0001d570: 5f64 6574 6563 746f 722e 616e 6f6d 616c  _detector.anomal
+0001d580: 6965 735b 7365 7269 6573 5d0d 0a20 2020  ies[series]..   
+0001d590: 2020 2020 2069 5f61 6e6f 6d20 3d20 7365       i_anom = se
+0001d5a0: 7269 6573 5f61 6e6f 6d5b 7365 7269 6573  ries_anom[series
+0001d5b0: 5f61 6e6f 6d20 3d3d 202d 315d 2e69 6e64  _anom == -1].ind
+0001d5c0: 6578 0d0a 2020 2020 2020 2020 695f 616e  ex..        i_an
+0001d5d0: 6f6d 203d 2069 5f61 6e6f 6d5b 695f 616e  om = i_anom[i_an
+0001d5e0: 6f6d 203e 3d20 7374 6172 745f 6461 7465  om >= start_date
+0001d5f0: 5d0d 0a20 2020 2069 6620 6c65 6e28 695f  ]..    if len(i_
+0001d600: 616e 6f6d 2920 3e20 3020 616e 6420 6c65  anom) > 0 and le
+0001d610: 6e28 695f 616e 6f6d 2920 3c20 6c65 6e28  n(i_anom) < len(
+0001d620: 6466 5f64 6169 6c79 2920 2a20 302e 353a  df_daily) * 0.5:
+0001d630: 0d0a 2020 2020 2020 2020 7363 6174 3120  ..        scat1 
+0001d640: 3d20 6178 2e73 6361 7474 6572 2869 5f61  = ax.scatter(i_a
+0001d650: 6e6f 6d2e 746f 6c69 7374 2829 2c20 6466  nom.tolist(), df
+0001d660: 5f64 6169 6c79 2e6c 6f63 5b69 5f61 6e6f  _daily.loc[i_ano
+0001d670: 6d2c 203a 5d5b 7365 7269 6573 5d2c 2063  m, :][series], c
+0001d680: 3d22 6461 726b 736c 6174 6562 6c75 6522  ="darkslateblue"
+0001d690: 2c20 733d 3132 2e30 290d 0a20 2020 2020  , s=12.0)..     
+0001d6a0: 2020 2068 616e 646c 6573 202b 3d20 5b73     handles += [s
+0001d6b0: 6361 7431 5d0d 0a20 2020 2020 2020 206c  cat1]..        l
+0001d6c0: 6162 656c 7320 2b3d 205b 2261 6e6f 6d61  abels += ["anoma
+0001d6d0: 6c69 6573 225d 0d0a 6966 206d 6f64 2e68  lies"]..if mod.h
+0001d6e0: 6f6c 6964 6179 5f64 6574 6563 746f 723a  oliday_detector:
+0001d6f0: 0d0a 2020 2020 695f 616e 6f6d 203d 206d  ..    i_anom = m
+0001d700: 6f64 2e68 6f6c 6964 6179 5f64 6574 6563  od.holiday_detec
+0001d710: 746f 722e 6461 7465 735f 746f 5f68 6f6c  tor.dates_to_hol
+0001d720: 6964 6179 7328 6d6f 642e 6466 2e69 6e64  idays(mod.df.ind
+0001d730: 6578 2c20 7374 796c 653d 2273 6572 6965  ex, style="serie
+0001d740: 735f 666c 6167 2229 5b73 6572 6965 735d  s_flag")[series]
+0001d750: 0d0a 2020 2020 695f 616e 6f6d 203d 2069  ..    i_anom = i
+0001d760: 5f61 6e6f 6d2e 696e 6465 785b 695f 616e  _anom.index[i_an
+0001d770: 6f6d 203d 3d20 315d 0d0a 2020 2020 6966  om == 1]..    if
+0001d780: 206c 656e 2869 5f61 6e6f 6d29 203e 2030   len(i_anom) > 0
+0001d790: 2061 6e64 206c 656e 2869 5f61 6e6f 6d29   and len(i_anom)
+0001d7a0: 203c 206c 656e 2864 665f 6461 696c 7929   < len(df_daily)
+0001d7b0: 202a 2030 2e35 3a0d 0a20 2020 2020 2020   * 0.5:..       
+0001d7c0: 2073 6361 7432 203d 2061 782e 7363 6174   scat2 = ax.scat
+0001d7d0: 7465 7228 695f 616e 6f6d 2e74 6f6c 6973  ter(i_anom.tolis
+0001d7e0: 7428 292c 2064 665f 6461 696c 792e 6c6f  t(), df_daily.lo
+0001d7f0: 635b 695f 616e 6f6d 2c20 3a5d 5b73 6572  c[i_anom, :][ser
+0001d800: 6965 735d 2c20 633d 2264 6172 6b67 7265  ies], c="darkgre
+0001d810: 656e 222c 2073 3d31 322e 3029 0d0a 2020  en", s=12.0)..  
+0001d820: 2020 2020 2020 6861 6e64 6c65 7320 2b3d        handles +=
+0001d830: 205b 7363 6174 325d 0d0a 2020 2020 2020   [scat2]..      
+0001d840: 2020 6c61 6265 6c73 202b 3d20 5b22 6465    labels += ["de
+0001d850: 7465 6374 6564 2068 6f6c 6964 6179 7322  tected holidays"
+0001d860: 5d0d 0a69 6620 6d6f 642e 7472 656e 645f  ]..if mod.trend_
+0001d870: 616e 6f6d 616c 795f 6465 7465 6374 6f72  anomaly_detector
+0001d880: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+0001d890: 2020 2069 6620 6d6f 642e 7472 656e 645f     if mod.trend_
+0001d8a0: 616e 6f6d 616c 795f 6465 7465 6374 6f72  anomaly_detector
+0001d8b0: 2e6f 7574 7075 7420 3d3d 2022 756e 6976  .output == "univ
+0001d8c0: 6172 6961 7465 223a 0d0a 2020 2020 2020  ariate":..      
+0001d8d0: 2020 695f 616e 6f6d 203d 206d 6f64 2e74    i_anom = mod.t
+0001d8e0: 7265 6e64 5f61 6e6f 6d61 6c79 5f64 6574  rend_anomaly_det
+0001d8f0: 6563 746f 722e 616e 6f6d 616c 6965 732e  ector.anomalies.
+0001d900: 696e 6465 785b 6d6f 642e 616e 6f6d 616c  index[mod.anomal
+0001d910: 795f 6465 7465 6374 6f72 2e61 6e6f 6d61  y_detector.anoma
+0001d920: 6c69 6573 2e69 6c6f 635b 3a2c 2030 5d20  lies.iloc[:, 0] 
+0001d930: 3d3d 202d 315d 0d0a 2020 2020 656c 7365  == -1]..    else
+0001d940: 3a0d 0a20 2020 2020 2020 2073 6572 6965  :..        serie
+0001d950: 735f 616e 6f6d 203d 206d 6f64 2e74 7265  s_anom = mod.tre
+0001d960: 6e64 5f61 6e6f 6d61 6c79 5f64 6574 6563  nd_anomaly_detec
+0001d970: 746f 722e 616e 6f6d 616c 6965 735b 7365  tor.anomalies[se
+0001d980: 7269 6573 5d0d 0a20 2020 2020 2020 2069  ries]..        i
+0001d990: 5f61 6e6f 6d20 3d20 7365 7269 6573 5f61  _anom = series_a
+0001d9a0: 6e6f 6d5b 7365 7269 6573 5f61 6e6f 6d20  nom[series_anom 
+0001d9b0: 3d3d 202d 315d 2e69 6e64 6578 0d0a 2020  == -1].index..  
+0001d9c0: 2020 6966 2073 7461 7274 5f64 6174 6520    if start_date 
+0001d9d0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0001d9e0: 2020 2020 2020 695f 616e 6f6d 203d 2069        i_anom = i
+0001d9f0: 5f61 6e6f 6d5b 695f 616e 6f6d 203e 3d20  _anom[i_anom >= 
+0001da00: 7374 6172 745f 6461 7465 5d0d 0a20 2020  start_date]..   
+0001da10: 2069 6620 6c65 6e28 695f 616e 6f6d 2920   if len(i_anom) 
+0001da20: 3e20 3020 616e 6420 6c65 6e28 695f 616e  > 0 and len(i_an
+0001da30: 6f6d 2920 3c20 6c65 6e28 6466 5f64 6169  om) < len(df_dai
+0001da40: 6c79 2920 2a20 302e 353a 0d0a 2020 2020  ly) * 0.5:..    
+0001da50: 2020 2020 7363 6174 3320 3d20 6178 2e73      scat3 = ax.s
+0001da60: 6361 7474 6572 2869 5f61 6e6f 6d2e 746f  catter(i_anom.to
+0001da70: 6c69 7374 2829 2c20 6466 5f64 6169 6c79  list(), df_daily
+0001da80: 2e6c 6f63 5b69 5f61 6e6f 6d5d 5b73 6572  .loc[i_anom][ser
+0001da90: 6965 735d 2c20 633d 2273 6c61 7465 6772  ies], c="slategr
+0001daa0: 6179 222c 2073 3d31 322e 3029 0d0a 2020  ay", s=12.0)..  
+0001dab0: 2020 2020 2020 6861 6e64 6c65 7320 2b3d        handles +=
+0001dac0: 205b 7363 6174 335d 0d0a 2020 2020 2020   [scat3]..      
+0001dad0: 2020 6c61 6265 6c73 202b 3d20 5b22 7472    labels += ["tr
+0001dae0: 656e 6420 616e 6f6d 616c 6965 7322 5d0d  end anomalies"].
+0001daf0: 0a61 782e 6c65 6765 6e64 2868 616e 646c  .ax.legend(handl
+0001db00: 6573 2c20 6c61 6265 6c73 290d 0a22 2222  es, labels).."""
+0001db10: 0d0a                                     ..
```

### Comparing `autots-0.5.8/autots/models/dnn.py` & `autots-0.6.0/autots/models/dnn.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/models/ensemble.py` & `autots-0.6.0/autots/models/ensemble.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/models/gluonts.py` & `autots-0.6.0/autots/models/gluonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,33 +92,25 @@
             df (pandas.DataFrame): Datetime Indexed
         """
         if not _has_gluonts:
             raise ImportError(
                 "GluonTS installation is incompatible with AutoTS. The numpy version is sometimes the issue, try 1.23.1 {as of 06-2023}"
             )
 
-        df = self.basic_profile(df)
-
         try:
             from mxnet.random import seed as mxnet_seed
 
             mxnet_seed(self.random_seed)
         except Exception:
             pass
 
-        gluon_train = df.to_numpy().T
+        gluon_freq = str(self.frequency).split('-')[0]
         self.train_index = df.columns
         self.train_columns = df.index
 
-        gluon_freq = str(self.frequency).split('-')[0]
-        if self.regression_type == "User":
-            if future_regressor is None:
-                raise ValueError(
-                    "regression_type='User' but no future_regressor supplied"
-                )
         if gluon_freq in ["MS", "1MS"]:
             gluon_freq = "M"
 
         if int(self.verbose) > 1:
             print(f"Gluon Frequency is {gluon_freq}")
         if int(self.verbose) < 1:
             try:
@@ -131,74 +123,27 @@
             self.gluon_context_length = int(float(self.context_length))
         elif 'forecastlength' in str(self.context_length).lower():
             len_int = int([x for x in str(self.context_length) if x.isdigit()][0])
             self.gluon_context_length = int(len_int * self.forecast_length)
         else:
             self.gluon_context_length = 20
             self.context_length = '20'
-        ts_metadata = {
+        self.ts_metadata = ts_metadata = {
             'num_series': len(self.train_index),
             'freq': gluon_freq,
             'start_ts': df.index[0],
             'gluon_start': [
                 self.train_columns[0] for _ in range(len(self.train_index))
             ],
             'context_length': self.gluon_context_length,
             'forecast_length': self.forecast_length,
         }
+        self.fit_data(df, future_regressor=future_regressor)
         npts_flag = False
-        if self.gluon_model in self.multivariate_mods:
-            if self.regression_type == "User":
-                regr = future_regressor.to_numpy().T
-                self.regr_train = regr
-                self.test_ds = ListDataset(
-                    [
-                        {
-                            "start": df.index[0],
-                            "target": gluon_train,
-                            "feat_dynamic_real": regr,
-                        }
-                    ],
-                    freq=ts_metadata['freq'],
-                    one_dim_target=False,
-                )
-            else:
-                self.test_ds = ListDataset(
-                    [{"start": df.index[0], "target": gluon_train}],
-                    freq=ts_metadata['freq'],
-                    one_dim_target=False,
-                )
-        else:
-            if self.regression_type == "User":
-                self.gluon_train = gluon_train
-                regr = future_regressor.to_numpy().T
-                self.regr_train = regr
-                self.test_ds = ListDataset(
-                    [
-                        {
-                            FieldName.TARGET: target,
-                            FieldName.START: ts_metadata['start_ts'],
-                            FieldName.FEAT_DYNAMIC_REAL: regr,
-                        }
-                        for target in gluon_train
-                    ],
-                    freq=ts_metadata['freq'],
-                )
-            else:
-                # use the actual start date, if NaN given (semi-hidden)
-                # ts_metadata['gluon_start'] = df.notna().idxmax().tolist()
-                self.test_ds = ListDataset(
-                    [
-                        {FieldName.TARGET: target, FieldName.START: start}
-                        for (target, start) in zip(
-                            gluon_train, ts_metadata['gluon_start']
-                        )
-                    ],
-                    freq=ts_metadata['freq'],
-                )
+
         if self.gluon_model == 'DeepAR':
             try:
                 from gluonts.mx import DeepAREstimator
             except Exception:
                 from gluonts.model.deepar import DeepAREstimator
 
             estimator = DeepAREstimator(
@@ -315,28 +260,28 @@
         elif self.gluon_model == 'DeepVAR':
             try:
                 from gluonts.mx import DeepVAREstimator
             except Exception:
                 from gluonts.model.deepvar import DeepVAREstimator
 
             estimator = DeepVAREstimator(
-                target_dim=gluon_train.shape[0],
+                target_dim=df.shape[1],
                 freq=ts_metadata['freq'],
                 context_length=ts_metadata['context_length'],
                 prediction_length=ts_metadata['forecast_length'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
         elif self.gluon_model == 'GPVAR':
             try:
                 from gluonts.mx import GPVAREstimator
             except Exception:
                 from gluonts.model.gpvar import GPVAREstimator
 
             estimator = GPVAREstimator(
-                target_dim=gluon_train.shape[0],
+                target_dim=df.shape[1],
                 freq=ts_metadata['freq'],
                 context_length=ts_metadata['context_length'],
                 prediction_length=ts_metadata['forecast_length'],
                 trainer=Trainer(epochs=self.epochs, learning_rate=self.learning_rate),
             )
         elif self.gluon_model == 'LSTNet':
             try:
@@ -439,32 +384,97 @@
         else:
             raise ValueError("'gluon_model' not recognized.")
 
         if self.gluon_model == 'NPTS' and npts_flag:
             self.GluonPredictor = estimator
         else:
             self.GluonPredictor = estimator.train(self.test_ds)
-        self.ts_metadata = ts_metadata
         self.fit_runtime = datetime.datetime.now() - self.startTime
         return self
 
+    def fit_data(self, df, future_regressor=None):
+        df = self.basic_profile(df)
+        gluon_train = df.to_numpy().T
+        self.train_index = df.columns
+        self.train_columns = df.index
+        if self.regression_type == "User":
+            if future_regressor is None:
+                raise ValueError(
+                    "regression_type='User' but no future_regressor supplied"
+                )
+        if self.gluon_model in self.multivariate_mods:
+            if self.regression_type == "User":
+                regr = future_regressor.to_numpy().T
+                self.regr_train = regr
+                self.test_ds = ListDataset(
+                    [
+                        {
+                            "start": df.index[0],
+                            "target": gluon_train,
+                            "feat_dynamic_real": regr,
+                        }
+                    ],
+                    freq=self.ts_metadata['freq'],
+                    one_dim_target=False,
+                )
+            else:
+                self.test_ds = ListDataset(
+                    [{"start": df.index[0], "target": gluon_train}],
+                    freq=self.ts_metadata['freq'],
+                    one_dim_target=False,
+                )
+        else:
+            if self.regression_type == "User":
+                self.gluon_train = gluon_train
+                regr = future_regressor.to_numpy().T
+                self.regr_train = regr
+                self.test_ds = ListDataset(
+                    [
+                        {
+                            FieldName.TARGET: target,
+                            FieldName.START: self.ts_metadata['start_ts'],
+                            FieldName.FEAT_DYNAMIC_REAL: regr,
+                        }
+                        for target in gluon_train
+                    ],
+                    freq=self.ts_metadata['freq'],
+                )
+            else:
+                # use the actual start date, if NaN given (semi-hidden)
+                # ts_metadata['gluon_start'] = df.notna().idxmax().tolist()
+                self.test_ds = ListDataset(
+                    [
+                        {FieldName.TARGET: target, FieldName.START: start}
+                        for (target, start) in zip(
+                            gluon_train, self.ts_metadata['gluon_start']
+                        )
+                    ],
+                    freq=self.ts_metadata['freq'],
+                )
+        return self
+
     def predict(
-        self, forecast_length: int, future_regressor=[], just_point_forecast=False
+        self,
+        forecast_length: int = None,
+        future_regressor=[],
+        just_point_forecast=False,
     ):
         """Generates forecast data immediately following dates of index supplied to .fit()
 
         Args:
             forecast_length (int): Number of periods of data to forecast ahead
             regressor (numpy.Array): additional regressor, not used
             just_point_forecast (bool): If True, return a pandas.DataFrame of just point forecasts
 
         Returns:
             Either a PredictionObject of forecasts and metadata, or
             if just_point_forecast == True, a dataframe of point forecasts
         """
+        if forecast_length is None:
+            forecast_length = self.forecast_length
         if int(forecast_length) > int(self.forecast_length):
             raise ValueError("GluonTS must be refit to change forecast length!")
         predictStartTime = datetime.datetime.now()
         test_index = self.create_forecast_index(
             forecast_length=self.ts_metadata['forecast_length']
         )
         if self.regression_type == "User":
```

### Comparing `autots-0.5.8/autots/models/greykite.py` & `autots-0.6.0/autots/models/greykite.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/models/matrix_var.py` & `autots-0.6.0/autots/models/matrix_var.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/models/mlensemble.py` & `autots-0.6.0/autots/models/mlensemble.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/models/model_list.py` & `autots-0.6.0/autots/models/model_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,20 +118,22 @@
     'MultivariateMotif': 1,
     'Theta': 1,
     'ARDL': 1,
     'ARCH': 1,
 }
 # models that should be fast given many CPU cores
 fast_parallel = {**parallel, **fast}
-fast_parallel_no_arima = {i: fast_parallel[i] for i in fast_parallel if i != 'ARIMA'}
+fast_parallel_no_arima = {
+    i: fast_parallel[i] for i in fast_parallel if i not in ['ARIMA', 'NVAR']
+}
 # so this opiniated and not fully updated always
 best = list(
     set(
         list(fast_parallel_no_arima.keys())
-        + ['MultivariateRegression', 'GluonTS', 'TMF', 'PytorchForecasting']
+        + ['MultivariateRegression', 'GluonTS', 'PytorchForecasting']
     )
 )
 
 # models that are explicitly not production ready
 experimental = [
     'MotifSimulation',
     'TensorflowSTS',
@@ -286,15 +288,15 @@
 regressions = [
     'RollingRegression',
     'WindowRegression',
     'DatepartRegression',
     'UnivariateRegression',
     'MultivariateRegression',
 ]
-no_shared_fast = list(set(no_shared).intersection(set(fast_parallel)))
+no_shared_fast = list(set(no_shared).intersection(set(fast_parallel_no_arima)))
 # this should be implementable with some models in gluonts
 all_result_path = [
     "UnivariateMotif",
     "MultivariateMotif",
     "SectionalMotif",
     'MetricMotif',
     "SeasonalityMotif",
@@ -305,14 +307,22 @@
 # these are those that require a parameter, and return a dict
 diff_window_motif_list = [
     "UnivariateMotif",
     "MultivariateMotif",
     "Motif",
     "ARCH",
 ]
+# models that fit and then have updated predicts without updated model fits (just data update)
+update_fit = [
+    'MultivariateRegression',
+    "DatepartRegression",
+    "GluonTS",
+    'WindowRegression',
+    'Cassandra',
+]
 model_lists = {
     "all": all_models,
     "default": default,
     "fast": fast,
     "superfast": superfast,
     "parallel": parallel,
     "fast_parallel": fast_parallel,
@@ -329,14 +339,15 @@
     "gpu": gpu,
     "regressor": regressor,
     "best": best,
     "motifs": motifs,
     "all_result_path": all_result_path,
     "regressions": regressions,
     "all_pragmatic": all_pragmatic,
+    "update_fit": update_fit,
 }
 
 
 def auto_model_list(n_jobs, n_series, frequency):
     pass
```

### Comparing `autots-0.5.8/autots/models/prophet.py` & `autots-0.6.0/autots/models/prophet.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/models/pytorch.py` & `autots-0.6.0/autots/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/models/sklearn.py` & `autots-0.6.0/autots/models/sklearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,20 +196,19 @@
     if future_regressor is not None:
         X = pd.concat([X, future_regressor], axis=1)
     return X
 
 
 def retrieve_regressor(
     regression_model: dict = {
-        "model": 'Adaboost',
+        "model": 'RandomForest',
         "model_params": {
-            'n_estimators': 50,
-            'estimator': 'DecisionTree',
-            'loss': 'linear',
-            'learning_rate': 1.0,
+            'n_estimators': 300,
+            'min_samples_leaf': 1,
+            'bootstrap': False,
         },
     },
     verbose: int = 0,
     verbose_bool: bool = False,
     random_seed: int = 2020,
     n_jobs: int = 1,
     multioutput: bool = True,
@@ -547,15 +546,15 @@
     'RandomForest': 0.05,
     'ElasticNet': 0.05,
     'MLP': 0.05,
     'DecisionTree': 0.05,
     'Adaboost': 0.05,
     'SVM': 0.05,
     'KerasRNN': 0.05,
-    'Transformer': 0.05,
+    'Transformer': 0.02,  # slow
     'ExtraTrees': 0.07,
     'RadiusNeighbors': 0.05,
 }
 gradient_boosting = {
     'xgboost': 0.09,
     'HistGradientBoost': 0.03,
     'LightGBM': 0.09,
@@ -1176,15 +1175,15 @@
 
         multioutput = True
         if self.Y.ndim < 2:
             multioutput = False
         elif self.Y.shape[1] < 2:
             multioutput = False
         # retrieve model object to train
-        self.regr = retrieve_regressor(
+        self.model = retrieve_regressor(
             regression_model=self.regression_model,
             verbose=self.verbose,
             verbose_bool=self.verbose_bool,
             random_seed=self.random_seed,
             n_jobs=self.n_jobs,
             multioutput=multioutput,
         )
@@ -1201,15 +1200,15 @@
                 x_device = from_numpy(X, usm_type='device', device=device, sycl_queue=dpctl.SyclQueue(device))
                 y_device = from_numpy(Y, usm_type='device', device=device, sycl_queue=dpctl.SyclQueue(device))
             use_device = True
         except Exception:
             x_device = X
             y_device = Y
         """
-        self.regr = self.regr.fit(self.X, self.Y)
+        self.model = self.model.fit(self.X, self.Y)
 
         self.fit_runtime = datetime.datetime.now() - self.startTime
         return self
 
     def predict(
         self,
         forecast_length: int,
@@ -1265,15 +1264,15 @@
                 ).fillna(0)
             if self.x_transform in ['FastICA', 'Nystroem', 'RmZeroVariance']:
                 x_dat = pd.DataFrame(self.x_transformer.transform(x_dat))
                 x_dat = x_dat.replace([np.inf, -np.inf], 0).fillna(0)
             if isinstance(x_dat, pd.DataFrame):
                 x_dat.columns = [str(xc) for xc in x_dat.columns]
 
-            rfPred = pd.DataFrame(self.regr.predict(x_dat.tail(1).to_numpy()))
+            rfPred = pd.DataFrame(self.model.predict(x_dat.tail(1).to_numpy()))
 
             forecast = pd.concat([forecast, rfPred], axis=0, ignore_index=True)
             self.sktraindata = pd.concat(
                 [self.sktraindata, rfPred], axis=0, ignore_index=True
             )
             self.sktraindata.index = combined_index[: len(self.sktraindata.index)]
 
@@ -1492,47 +1491,57 @@
         multioutput = True
         if self.Y.ndim < 2:
             multioutput = False
         elif self.Y.shape[1] < 2:
             multioutput = False
         if isinstance(self.X, pd.DataFrame):
             self.X = self.X.to_numpy()
-        self.regr = retrieve_regressor(
+        self.model = retrieve_regressor(
             regression_model=self.regression_model,
             verbose=self.verbose,
             verbose_bool=self.verbose_bool,
             random_seed=self.random_seed,
             n_jobs=self.n_jobs,
             multioutput=multioutput,
         )
-        self.regr = self.regr.fit(self.X.astype(float), self.Y.astype(float))
+        self.model = self.model.fit(self.X.astype(float), self.Y.astype(float))
         self.last_window = df.tail(self.window_size)
         self.fit_runtime = datetime.datetime.now() - self.startTime
         return self
 
+    def fit_data(self, df, future_regressor=None):
+        df = self.basic_profile(df)
+        self.last_window = df.tail(self.window_size)
+        return self
+
     def predict(
         self,
-        forecast_length: int,
+        forecast_length: int = None,
         future_regressor=None,
         just_point_forecast: bool = False,
+        df=None,
     ):
         """Generate forecast data immediately following dates of .fit().
 
         Args:
             forecast_length (int): Number of periods of data to forecast ahead
             regressor (numpy.Array): additional regressor, not used
             just_point_forecast (bool): If True, return a pandas.DataFrame of just point forecasts
 
         Returns:
             Either a PredictionObject of forecasts and metadata, or
             if just_point_forecast == True, a dataframe of point forecasts
         """
+        predictStartTime = datetime.datetime.now()
+        if df is not None:
+            self.fit_data(df)
+        if forecast_length is None:
+            forecast_length = self.forecast_length
         if int(forecast_length) > int(self.forecast_length):
             print("Regression must be refit to change forecast length!")
-        predictStartTime = datetime.datetime.now()
         index = self.create_forecast_index(forecast_length=forecast_length)
 
         if self.output_dim == '1step':
             # combined_index = (self.df_train.index.append(index))
             forecast = pd.DataFrame()
             # forecast, 1 step ahead, then another, and so on
             for x in range(forecast_length):
@@ -1545,15 +1554,15 @@
                 if self.regression_type in ["User", "user"]:
                     blasted_thing = future_regressor.iloc[x].to_frame().transpose()
                     tmerg = pd.concat([blasted_thing] * pred.shape[0], axis=0)
                     tmerg.index = pred.index
                     pred = pd.concat([pred, tmerg], axis=1, ignore_index=True)
                 if isinstance(pred, pd.DataFrame):
                     pred = pred.to_numpy()
-                rfPred = pd.DataFrame(self.regr.predict(pred))
+                rfPred = pd.DataFrame(self.model.predict(pred))
                 if self.input_dim == 'univariate':
                     rfPred = rfPred.transpose()
                     rfPred.columns = self.last_window.columns
                 forecast = pd.concat([forecast, rfPred], axis=0, ignore_index=True)
                 self.last_window = pd.concat(
                     [self.last_window, rfPred], axis=0, ignore_index=True
                 )
@@ -1570,15 +1579,15 @@
                 tmerg = future_regressor.tail(1).loc[
                     future_regressor.tail(1).index.repeat(pred.shape[0])
                 ]
                 tmerg.index = pred.index
                 pred = pd.concat([pred, tmerg], axis=1)
             if isinstance(pred, pd.DataFrame):
                 pred = pred.to_numpy()
-            cY = pd.DataFrame(self.regr.predict(pred.astype(float)))
+            cY = pd.DataFrame(self.model.predict(pred.astype(float)))
             if self.input_dim == 'multivariate':
                 cY.index = ['values']
                 cY.columns = np.tile(self.column_names, reps=self.forecast_length)
                 cY = cY.transpose().reset_index()
                 cY['timestep'] = np.repeat(
                     range(forecast_length), repeats=len(self.column_names)
                 )
@@ -1791,15 +1800,15 @@
         except Exception as e:
             raise ValueError(f"Model {str(self.model)} with error: {repr(e)}")
         self.fit_runtime = datetime.datetime.now() - self.startTime
         return self
 
     def predict(
         self,
-        forecast_length: int,
+        forecast_length: int = None,
         future_regressor=None,
         just_point_forecast: bool = False,
     ):
         """Generate forecast data immediately following dates of .fit().
 
         Args:
             forecast_length (int): Number of periods of data to forecast ahead
@@ -1808,14 +1817,16 @@
 
         Returns:
             Either a PredictionObject of forecasts and metadata, or
             if just_point_forecast == True, a dataframe of point forecasts
         """
         predictStartTime = datetime.datetime.now()
 
+        if forecast_length is None:
+            forecast_length = self.forecast_length
         XA = self.modelobj.predict(
             forecast_length=forecast_length, future_regressor=future_regressor
         )
         Xf = self.transformer.inverse_transform(np.array(XA.forecast))
         if not isinstance(Xf, pd.DataFrame):
             Xf = pd.DataFrame(Xf)
         Xf.columns = self.column_names
@@ -1947,14 +1958,15 @@
             regression_type=regression_type,
             verbose=verbose,
             n_jobs=n_jobs,
         )
         self.regression_model = regression_model
         self.datepart_method = datepart_method
         self.polynomial_degree = polynomial_degree
+        self.forecast_length = forecast_length
 
     def fit(self, df, future_regressor=None):
         """Train algorithm given data supplied.
 
         Args:
             df (pandas.DataFrame): Datetime Indexed
         """
@@ -1994,31 +2006,40 @@
             multioutput=multioutput,
         )
         self.df_train = df
         self.model = self.model.fit(self.X.astype(float), y.astype(float))
         self.shape = df.shape
         return self
 
+    def fit_data(self, df, future_regressor=None):
+        self.basic_profile(df)
+        return self
+
     def predict(
         self,
-        forecast_length: int,
+        forecast_length: int = None,
         future_regressor=None,
         just_point_forecast: bool = False,
+        df=None,
     ):
         """Generate forecast data immediately following dates of index supplied to .fit().
 
         Args:
             forecast_length (int): Number of periods of data to forecast ahead
             future_regressor (pandas.DataFrame or Series): Datetime Indexed
             just_point_forecast (bool): If True, return a pandas.DataFrame of just point forecasts
 
         Returns:
             Either a PredictionObject of forecasts and metadata, or
             if just_point_forecast == True, a dataframe of point forecasts
         """
+        if forecast_length is None:
+            forecast_length = self.forecast_length
+        if df is not None:
+            self.fit_data(df)
         predictStartTime = datetime.datetime.now()
         index = self.create_forecast_index(forecast_length=forecast_length)
         self.X_pred = date_part(
             index, method=self.datepart_method, polynomial_degree=self.polynomial_degree
         )
         if self.regression_type in ['User', 'user']:
             self.X_pred = pd.concat([self.X_pred, future_regressor], axis=1)
@@ -2743,37 +2764,50 @@
             )
             self.model.fit(self.X, self.Y)
 
             if self.probabilistic:
                 self.model_upper.fit(self.X, self.Y)
                 self.model_lower.fit(self.X, self.Y)
             # we only need the N most recent points for predict
-            self.sktraindata = df.tail(self.min_threshold)
+            # self.sktraindata = df.tail(self.min_threshold)
+            self.fit_data(df)
 
             self.fit_runtime = datetime.datetime.now() - self.startTime
             return self
 
+    def fit_data(self, df, future_regressor=None):
+        df = self.basic_profile(df)
+        self.sktraindata = df.tail(self.min_threshold)
+        if future_regressor is not None:
+            self.regressor_train = future_regressor
+        return self
+
     def predict(
         self,
         forecast_length: int = None,
         just_point_forecast: bool = False,
         future_regressor=None,
+        df=None,
     ):
         """Generate forecast data immediately following dates of index supplied to .fit().
 
         Args:
             forecast_length (int): Number of periods of data to forecast ahead
                 ignored here for this model, must be set in __init__ before .fit()
             future_regressor (pd.DataFrame): additional regressor
             just_point_forecast (bool): If True, return a pandas.DataFrame of just point forecasts
 
         Returns:
             Either a PredictionObject of forecasts and metadata, or
             if just_point_forecast == True, a dataframe of point forecasts
         """
+        if df is not None:
+            self.fit_data(df)  # no new regressor support
+        if forecast_length is None:
+            forecast_length = self.forecast_length
         predictStartTime = datetime.datetime.now()
         index = self.create_forecast_index(forecast_length=forecast_length)
         forecast = pd.DataFrame()
         upper_forecast = pd.DataFrame()
         lower_forecast = pd.DataFrame()
         if self.regressor_train is not None:
             base_regr = pd.concat([self.regressor_train, future_regressor])
```

### Comparing `autots-0.5.8/autots/models/statsmodels.py` & `autots-0.6.0/autots/models/statsmodels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1132,15 +1132,16 @@
             'cov_type': random.choices(
                 ["opg", "oim", "approx", 'robust'], [0.8, 0.1, 0.1, 0.1]
             )[0],
             'method': random.choices(
                 ["lbfgs", "bfgs", "powell", "cg", "newton", "nm"],
                 [0.8, 0.1, 0.1, 0.1, 0.1, 0.1],
             )[0],
-            'autoregressive': random.choices([None, 1, 2], [0.8, 0.2, 0.1])[0],
+            # AR1 is helpful but AR2 is getting slow
+            'autoregressive': random.choices([None, 1, 2], [0.8, 0.3, 0.02])[0],
             'regression_type': regression_choice,
         }
 
     def get_params(self):
         """Return dict of current parameters."""
         return {
             'level': self.level,
```

### Comparing `autots-0.5.8/autots/models/tfp.py` & `autots-0.6.0/autots/models/tfp.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/templates/general.py` & `autots-0.6.0/autots/templates/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,24 +411,25 @@
             "trend_transformation": {"fillna": "ffill_mean_biased", "transformations": {"0": "bkfilter"}, "transformation_params": {"0": {}}},
             "trend_model": {"Model": "MetricMotif", "ModelParameters": {"window": 7, "point_method": "mean", "distance_metric": "mae", "k": 10, "comparison_transformation": {"fillna": "quadratic", "transformations": {"0": null}, "transformation_params": {"0": {}}}, "combination_transformation": {"fillna": "ffill", "transformations": {"0": "AlignLastValue"}, "transformation_params": {"0": {"rows": 1, "lag": 1, "method": "additive", "strength": 1.0, "first_value_only": false}}}}},
             "trend_phi": null
         }''',
         'TransformationParameters': '{"fillna": null, "transformations": {}, "transformation_params": {}}',
         'Ensemble': 0,
     },
-}
-"""
-
-    "66": {
-        'Model': 'UnivariateRegression',
-        'ModelParameters': '{"regression_model": {"model": "KNN", "model_params": {"n_neighbors": 3, "weights": "uniform"}}, "holiday": false, "mean_rolling_periods": 5, "macd_periods": 28, "std_rolling_periods": null, "max_rolling_periods": 24, "min_rolling_periods": null, "ewm_var_alpha": null, "ewm_alpha": 0.5, "additional_lag_periods": 11, "abs_energy": false, "rolling_autocorr_periods": null, "add_date_part": null, "polynomial_degree": null, "x_transform": null, "regression_type": null, "window": null}',
-        'TransformationParameters': '{"fillna": "rolling_mean", "transformations": {"0": "QuantileTransformer", "1": "QuantileTransformer"}, "transformation_params": {"0": {"output_distribution": "normal", "n_quantiles": 1000}, "1": {"output_distribution": "uniform", "n_quantiles": 20}}}',
+    "68": {
+        'Model': 'SeasonalityMotif',
+        'ModelParameters': '''{
+            "window": 5, "point_method": "weighted_mean",
+            "distance_metric": "mae", "k": 10,
+            "datepart_method": "common_fourier"
+        }''',
+        'TransformationParameters': '{"fillna": "nearest", "transformations": {"0": "AlignLastValue"}, "transformation_params": {"0": {"rows": 1, "lag": 1, "method": "multiplicative", "strength": 1.0, "first_value_only": false}}}',
         'Ensemble': 0,
     },
-"""
+}
 
 general_template = pd.DataFrame.from_dict(general_template_dict, orient='index')
 
 
 """
 # Basic Template Construction Code
 # transformer_max_depth = 6 and transformer_list = "fast"
```

### Comparing `autots-0.5.8/autots/tools/anomaly_utils.py` & `autots-0.6.0/autots/tools/anomaly_utils.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/calendar.py` & `autots-0.6.0/autots/tools/calendar.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/cointegration.py` & `autots-0.6.0/autots/tools/cointegration.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/cpu_count.py` & `autots-0.6.0/autots/tools/cpu_count.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/fast_kalman.py` & `autots-0.6.0/autots/tools/fast_kalman.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/hierarchial.py` & `autots-0.6.0/autots/tools/hierarchial.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/holiday.py` & `autots-0.6.0/autots/tools/holiday.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/lunar.py` & `autots-0.6.0/autots/tools/lunar.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/percentile.py` & `autots-0.6.0/autots/tools/percentile.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/probabilistic.py` & `autots-0.6.0/autots/tools/probabilistic.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/profile.py` & `autots-0.6.0/autots/tools/profile.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/regressor.py` & `autots-0.6.0/autots/tools/regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pandas as pd
 from autots.tools.impute import FillNA
 from autots.tools.shaping import infer_frequency
 from autots.tools.seasonal import date_part
 from autots.tools.holiday import holiday_flag
 from autots.tools.cointegration import coint_johansen
 from autots.evaluator.anomaly_detector import HolidayDetector
+from autots.tools.transform import GeneralTransformer
 
 
 def create_regressor(
     df,
     forecast_length,
     frequency: str = "infer",
     holiday_countries: list = ["US"],
@@ -40,15 +41,16 @@
                 "transformations": {"0": "DifferencedTransformer"},
                 "transformation_params": {"0": {}},
             },
             "forecast_params": None,
             "method_params": {"distribution": "gamma", "alpha": 0.05},
         },
     },
-    holiday_regr_style="flag",
+    holiday_regr_style: str = "flag",
+    preprocessing_params: dict = None,
 ):
     """Create a regressor from information available in the existing dataset.
     Components: are lagged data, datepart information, and holiday.
 
     This function has been confusing people. This is NOT necessary for machine learning models, in AutoTS they internally create more elaborate feature sets separately.
     This instead may help some other models (GLM, ARIMA) which accept regressors but won't build a regressor feature set internally.
     And this allows post-hoc customization as needed before input to AutoTS.
@@ -73,14 +75,15 @@
             "ETS" -backfill with ETS backwards forecast
             "DatepartRegression" - backfill with DatepartRegression
         fill_na (str): method to prefill NAs in data, same methods as available elsewhere
         aggfunc (str): str or func, used if frequency is resampled
         encode_holiday_type (bool): if True, returns column per holiday, ONLY for holidays package country holidays (not Detector)
         holiday_detector_params (dict): passed to HolidayDetector, or None
         holiday_regr_style (str): passed to detector's dates_to_holidays 'flag', 'series_flag', 'impact'
+        preprocessing_params (dict): GeneralTransformer params to be applied before regressor creation
 
     Returns:
         regressor_train, regressor_forecast
     """
     if not isinstance(df.index, pd.DatetimeIndex):
         raise ValueError(
             "create_regressor input df must be `wide` style with pd.DatetimeIndex index"
@@ -99,14 +102,19 @@
             else:
                 df = df.resample(frequency).apply(aggfunc)
         except Exception:
             df = df.asfreq(frequency, fill_value=None)
     # handle categorical
     df = df.apply(pd.to_numeric, errors='ignore')
     df = df.select_dtypes(include=np.number)
+    # macro_micro
+    if preprocessing_params is not None:
+        trans = GeneralTransformer(**preprocessing_params)
+        df = trans.fit_transform(df)
+
     # lagged data
     regr_train, regr_fcst = create_lagged_regressor(
         df,
         forecast_length=forecast_length,
         frequency=frequency,
         summarize=summarize,
         scale=scale,  # already done above
```

### Comparing `autots-0.5.8/autots/tools/seasonal.py` & `autots-0.6.0/autots/tools/seasonal.py`

 * *Files 10% similar despite different names*

```diff
@@ -486,28 +486,33 @@
     if k > min_k:
         n_tail = min(window_size, forecast_length)
     else:
         n_tail = forecast_length
     # finding sliding windows to compare
     temp = sliding_window_view(array[:-n_tail, :], window_size, axis=0)
     # compare windows by metrics
+    last_window = array[-window_size:, :]
     if distance_metric == "mae":
-        scores = np.mean(np.abs(temp - array[-window_size:, :].T), axis=2)
+        scores = np.mean(np.abs(temp - last_window.T), axis=2)
+    elif distance_metric == "canberra":
+        divisor = np.abs(temp) + np.abs(last_window.T)
+        divisor[divisor == 0] = 1
+        scores = np.mean(np.abs(temp - last_window.T) / divisor, axis=2)
     elif distance_metric == "mqae":
         q = 0.85
-        ae = np.abs(temp - array[-window_size:, :].T)
+        ae = np.abs(temp - last_window.T)
         if ae.shape[2] <= 1:
             vals = ae
         else:
             qi = int(ae.shape[2] * q)
             qi = qi if qi > 1 else 1
             vals = np.partition(ae, qi, axis=2)[..., :qi]
         scores = np.mean(vals, axis=2)
     elif distance_metric == "mse":
-        scores = np.mean((temp - array[-window_size:, :].T) ** 2, axis=2)
+        scores = np.mean((temp - last_window.T) ** 2, axis=2)
     else:
         raise ValueError(f"distance_metric: {distance_metric} not recognized")
 
     # select smallest windows
     min_idx = np.argpartition(scores.mean(axis=1), k - 1, axis=0)[:k]
     # take the period starting AFTER the window
     test = (
@@ -518,7 +523,49 @@
         + min_idx
         + window_size
     )
     # for data over the end, fill last value
     if k > min_k:
         test = np.where(test >= len(DTindex), -1, test)
     return test, scores
+
+
+def seasonal_independent_match(
+    DTindex, DTindex_future, k, datepart_method, distance_metric
+):
+    array = date_part(DTindex, method=datepart_method).to_numpy()
+    future_array = date_part(DTindex_future, method=datepart_method).to_numpy()
+
+    # when k is larger, can be more aggressive on allowing a longer portion into view
+    min_k = 5
+    # compare windows by metrics
+    a = array[:, None]
+    b = future_array
+    if distance_metric == "mae":
+        scores = np.mean(np.abs(a - b), axis=2)
+    elif distance_metric == "canberra":
+        divisor = np.abs(a) + np.abs(b)
+        divisor[divisor == 0] = 1
+        scores = np.mean(np.abs(a - b) / divisor, axis=2)
+    elif distance_metric == "mqae":
+        q = 0.85
+        ae = np.abs(a - b)
+        if ae.shape[2] <= 1:
+            vals = ae
+        else:
+            qi = int(ae.shape[2] * q)
+            qi = qi if qi > 1 else 1
+            vals = np.partition(ae, qi, axis=2)[..., :qi]
+        scores = np.mean(vals, axis=2)
+    elif distance_metric == "mse":
+        scores = np.mean((a - b) ** 2, axis=2)
+    else:
+        raise ValueError(f"distance_metric: {distance_metric} not recognized")
+
+    # select smallest windows
+    min_idx = np.argpartition(scores, k - 1, axis=0)[:k]
+    # take the period starting AFTER the window
+    test = min_idx.T
+    # for data over the end, fill last value
+    if k > min_k:
+        test = np.where(test >= len(DTindex), -1, test)
+    return test, scores
```

### Comparing `autots-0.5.8/autots/tools/shaping.py` & `autots-0.6.0/autots/tools/shaping.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,29 +54,35 @@
         pd.DataFrame: original dataframe, now possibly shorter.
 
     """
     # check to make sure column names are unique
     if verbose > 0:
         dupes = df_wide.columns.duplicated()
         if sum(dupes) > 0:
-            print("Warning, series ids are not unique: {df_wide.columns[dupes]}")
+            print(f"Warning, series ids are not unique: {df_wide.columns[dupes]}")
 
     # infer frequency
+    inferred_freq = infer_frequency(df_wide)
     if frequency == 'infer':
-        frequency = infer_frequency(df_wide)
-        if verbose > 0:
-            print("Inferred frequency is: {}".format(str(frequency)))
-        if (frequency is None) and (verbose >= 0):
-            print("Frequency is 'None'! Input frequency not recognized.")
-
-    # fill missing dates in index with NaN, resample to freq as necessary
-    try:
-        df_wide = df_wide.resample(frequency).apply(aggfunc)
-    except Exception:
-        df_wide = df_wide.asfreq(frequency, fill_value=np.nan)
+        frequency = inferred_freq
+    if verbose > 0:
+        print(f"Data frequency is: {inferred_freq}, used frequency is: {frequency}")
+    if (frequency is None) and (verbose >= 0):
+        print("Frequency is 'None'! Data frequency not recognized.")
+
+    # trying to avoid resampling if necessary because it can cause unexpected data changes
+    # test if dates are missing from index
+    expected_index = pd.date_range(df_wide.index[0], df_wide.index[-1], freq=frequency)
+    # or at least if lengths are the same, which should be a 'good enough' test for likely issues
+    if len(df_wide.index) != len(expected_index):
+        # fill missing dates in index with NaN, resample to freq as necessary
+        try:
+            df_wide = df_wide.resample(frequency).apply(aggfunc)
+        except Exception:
+            df_wide = df_wide.asfreq(frequency, fill_value=np.nan)
 
     # drop older data, because too much of a good thing...
     if str(drop_data_older_than_periods).isdigit():
         if int(drop_data_older_than_periods) < df_wide.shape[0]:
             if verbose >= 1:
                 print("Old data dropped by `drop_data_older_than_periods`.")
             df_wide = df_wide.tail(int(drop_data_older_than_periods))
@@ -106,15 +112,15 @@
     if (df_wide.shape[1]) < 1:
         raise ValueError("All series filtered! Frequency may be incorrect")
 
     # drop most recent value when desired
     if drop_most_recent > 0:
         df_wide.drop(df_wide.tail(drop_most_recent).index, inplace=True)
 
-    return pd.DataFrame(df_wide)
+    return df_wide
 
 
 def long_to_wide(
     df,
     date_col: str = 'datetime',
     value_col: str = 'value',
     id_col: str = 'series_id',
```

### Comparing `autots-0.5.8/autots/tools/thresholding.py` & `autots-0.6.0/autots/tools/thresholding.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/autots/tools/transform.py` & `autots-0.6.0/autots/tools/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from autots.tools.anomaly_utils import (
     anomaly_new_params,
     detect_anomalies,
     anomaly_df_to_holidays,
     holiday_new_params,
     dates_to_holidays,
 )
-from autots.tools.window_functions import window_lin_reg, window_lin_reg_mean
+from autots.tools.window_functions import window_lin_reg_mean
 from autots.tools.fast_kalman import KalmanFilter, random_state_space
 from autots.tools.shaping import infer_frequency
 from autots.tools.holiday import holiday_flag
 
 try:
     from joblib import Parallel, delayed
 except Exception:
@@ -1139,61 +1139,121 @@
 
     def fit(self, df, regressor=None):
         """Fits trend for later detrending.
 
         Args:
             df (pandas.DataFrame): input dataframe
         """
+        df_local = df.copy()
         try:
-            df = df.astype(float)
+            df_local = df_local.astype(float)
         except Exception:
             raise ValueError("Data Cannot Be Converted to Numeric Float")
+        # handle NaN
+        nan_mask = np.isnan(df_local)
+        nan_mask_all = nan_mask.all(axis=1)
+        nan_mask_any = nan_mask.any(axis=1)
+        sum_nan_all = np.sum(nan_mask_all)
+        self.full_nan_rows = sum_nan_all > 0
+        self.partial_nan_rows = np.sum(nan_mask_any) > sum_nan_all
+        if self.full_nan_rows and not self.partial_nan_rows:
+            # this is the simplest if just all NaN rows, drop
+            df_local = df_local[~nan_mask_all]
 
         if self.transform_dict is not None:
             model = GeneralTransformer(**self.transform_dict)
-            y = model.fit_transform(df)
+            y = model.fit_transform(df_local)
         else:
-            y = df.to_numpy()
+            y = df_local.to_numpy()
         if y.shape[1] == 1:
             y = np.asarray(y).ravel()
         X = date_part(
-            df.index,
+            df_local.index,
             method=self.datepart_method,
             polynomial_degree=self.polynomial_degree,
         )
         if self.holiday_country is not None and self.holiday_countries_used:
             X = pd.concat(
                 [
                     X,
                     holiday_flag(
-                        df.index, country=self.holiday_country, encode_holiday_type=True
+                        df_local.index,
+                        country=self.holiday_country,
+                        encode_holiday_type=True,
                     ),
                 ],
                 axis=1,
             )
         if regressor is not None:
             X = pd.concat([X, regressor], axis=1)
-        self.X = X  # diagnostic
         multioutput = True
-        if y.ndim < 2:
-            multioutput = False
-        elif y.shape[1] < 2:
+        if self.partial_nan_rows:
+            # process into a single output approach
+            X = np.repeat(X.to_numpy(), y.shape[1], axis=0)
+            # add a (hopefully not too massive) series ID encoder. This will not scale well to large multivariate
+            # X = np.concatenate([X, np.repeat(np.eye(y.shape[1]), df_local.shape[0], axis=0)], axis=1)
+            X = np.concatenate(
+                [X, np.tile(np.eye(y.shape[1]), df_local.shape[0]).T], axis=1
+            )
+            y = y.flatten()
+            y_mask = np.isnan(y)
+            y = y[~y_mask]
+            X = X[~y_mask]
             multioutput = False
+        else:
+            if y.ndim < 2:
+                multioutput = False
+            elif y.shape[1] < 2:
+                multioutput = False
+        self.X = X  # diagnostic
         self.model = retrieve_regressor(
             regression_model=self.regression_model,
             verbose=0,
             verbose_bool=False,
             random_seed=2020,
             multioutput=multioutput,
             n_jobs=self.n_jobs,
         )
         self.model = self.model.fit(X, y)
-        self.shape = df.shape
+        self.shape = df_local.shape
         return self
 
+    def impute(self, df, regressor=None):
+        """Fill Missing. Needs to have same general pattern of missingness (full rows of NaN only or scattered NaN) as was present during .fit()"""
+        X = date_part(
+            df.index,
+            method=self.datepart_method,
+            polynomial_degree=self.polynomial_degree,
+        )
+        if self.holiday_country is not None and self.holiday_countries_used:
+            X = pd.concat(
+                [
+                    X,
+                    holiday_flag(
+                        df.index, country=self.holiday_country, encode_holiday_type=True
+                    ),
+                ],
+                axis=1,
+            )
+        if regressor is not None:
+            X = pd.concat([X, regressor], axis=1)
+        if self.partial_nan_rows:
+            # process into a single output approach
+            X = np.repeat(X.to_numpy(), self.shape[1], axis=0)
+            X = np.concatenate(
+                [X, np.tile(np.eye(self.shape[1]), df.shape[0]).T], axis=1
+            )
+
+        pred = self.model.predict(X)
+        if self.partial_nan_rows:
+            pred = pred.reshape(-1, df.shape[1])
+        y = pd.DataFrame(pred, columns=df.columns, index=df.index)
+        # np.where(np.isnan(df), y, df)
+        return df.where(~df.isnull(), y)
+
     def fit_transform(self, df, regressor=None):
         """Fit and Return Detrended DataFrame.
 
         Args:
             df (pandas.DataFrame): input dataframe
         """
         self.fit(df, regressor=regressor)
@@ -1223,16 +1283,25 @@
                         df.index, country=self.holiday_country, encode_holiday_type=True
                     ),
                 ],
                 axis=1,
             )
         if regressor is not None:
             X = pd.concat([X, regressor], axis=1)
+        if self.partial_nan_rows:
+            # process into a single output approach
+            X = np.repeat(X.to_numpy(), self.shape[1], axis=0)
+            X = np.concatenate(
+                [X, np.tile(np.eye(self.shape[1]), df.shape[0]).T], axis=1
+            )
         # X.columns = [str(xc) for xc in X.columns]
-        y = pd.DataFrame(self.model.predict(X), columns=df.columns, index=df.index)
+        pred = self.model.predict(X)
+        if self.partial_nan_rows:
+            pred = pred.reshape(-1, df.shape[1])
+        y = pd.DataFrame(pred, columns=df.columns, index=df.index)
         df = df - y
         return df
 
     def inverse_transform(self, df, regressor=None):
         """Return data to original form.
 
         Args:
@@ -1256,15 +1325,24 @@
                         df.index, country=self.holiday_country, encode_holiday_type=True
                     ),
                 ],
                 axis=1,
             )
         if regressor is not None:
             X = pd.concat([X, regressor], axis=1)
-        y = pd.DataFrame(self.model.predict(X), columns=df.columns, index=df.index)
+        if self.partial_nan_rows:
+            # process into a single output approach
+            X = np.repeat(X.to_numpy(), self.shape[1], axis=0)
+            X = np.concatenate(
+                [X, np.tile(np.eye(self.shape[1]), df.shape[0]).T], axis=1
+            )
+        pred = self.model.predict(X)
+        if self.partial_nan_rows:
+            pred = pred.reshape(-1, df.shape[1])
+        y = pd.DataFrame(pred, columns=df.columns, index=df.index)
         df = df + y
         return df
 
 
 DatepartRegression = DatepartRegressionTransformer
 
 
@@ -2992,29 +3070,34 @@
 class LocalLinearTrend(EmptyTransformer):
     """Remove a rolling linear trend.
     Note this will probably perform poorly with long forecast horizons as forecast trend is simply the tail (n_future) of data's trend.
 
     Args:
         rolling_window (int): width of window to take trend on
         n_future (int): amount of data for the trend to be used extending beyond the edges of history.
+        macro_micro (bool): when True, splits the data into separate parts (trend and residual) and later combines together in inverse
     """
 
     def __init__(
         self,
         rolling_window: float = 0.1,
         # n_tails: float = 0.1,
         n_future: float = 0.2,
         method: str = "mean",
+        macro_micro: bool = False,
+        suffix: str = "_lltmicro",
         **kwargs,
     ):
         super().__init__(name="LocalLinearTrend")
         self.rolling_window = rolling_window
         # self.n_tails = n_tails
         self.n_future = n_future
         self.method = method
+        self.macro_micro = macro_micro
+        self.suffix = suffix
 
     def _fit(self, df):
         """Learn behavior of data to change.
 
         Args:
             df (pandas.DataFrame): input dataframe
         """
@@ -3123,15 +3206,25 @@
         self.full_dates = np.concatenate(
             [
                 [self.dates.min() - 0.01],
                 self.dates,
                 [self.dates.max() + 0.01],
             ]
         )
-        return df - (self.slope * self.dates_2d + self.intercept)
+        if self.macro_micro:
+            macro = pd.DataFrame(
+                self.slope * self.dates_2d + self.intercept,
+                index=df.index,
+                columns=df.columns,
+            )
+            self.columns = df.columns
+            micro = (df - macro).rename(columns=lambda x: str(x) + self.suffix)
+            return pd.concat([macro, micro], axis=1)
+        else:
+            return df - (self.slope * self.dates_2d + self.intercept)
 
     def fit(self, df):
         """Learn behavior of data to change.
 
         Args:
             df (pandas.DataFrame): input dataframe
         """
@@ -3143,26 +3236,46 @@
 
         Args:
             df (pandas.DataFrame): input dataframe
         """
         dates = df.index.to_julian_date()
         dates_2d = np.repeat(dates.to_numpy()[..., None], df.shape[1], axis=1)
         idx = self.full_dates.searchsorted(dates)
-        return df - (self.full_slope[idx] * dates_2d + self.full_intercept[idx])
+        # return df - (self.full_slope[idx] * dates_2d + self.full_intercept[idx])
+
+        if self.macro_micro:
+            macro = pd.DataFrame(
+                self.full_slope[idx] * dates_2d + self.full_intercept[idx],
+                index=df.index,
+                columns=df.columns,
+            )
+            micro = (df - macro).rename(columns=lambda x: str(x) + self.suffix)
+            return pd.concat([macro, micro], axis=1)
+        else:
+            return df - (self.full_slope[idx] * dates_2d + self.full_intercept[idx])
 
     def inverse_transform(self, df, trans_method: str = "forecast"):
         """Return data to original *or* forecast form.
 
         Args:
             df (pandas.DataFrame): input dataframe
         """
-        dates = df.index.to_julian_date()
-        dates_2d = np.repeat(dates.to_numpy()[..., None], df.shape[1], axis=1)
-        idx = self.full_dates.searchsorted(dates)
-        return df + (self.full_slope[idx] * dates_2d + self.full_intercept[idx])
+        if self.macro_micro:
+            macro = df[self.columns]
+            micro = df[df.columns.difference(self.columns)]
+            micro = micro.rename(columns=lambda x: str(x)[: -len(self.suffix)])[
+                self.columns
+            ]
+            return macro + micro
+        else:
+            dates = df.index.to_julian_date()
+            n_cols = df.shape[1]
+            dates_2d = np.repeat(dates.to_numpy()[..., None], n_cols, axis=1)
+            idx = self.full_dates.searchsorted(dates)
+            return df + (self.full_slope[idx] * dates_2d + self.full_intercept[idx])
 
     def fit_transform(self, df):
         """Fits and Returns *Magical* DataFrame.
 
         Args:
             df (pandas.DataFrame): input dataframe
         """
@@ -3178,14 +3291,15 @@
             "n_tails": random.choices(
                 [0.1, 90, 30, 180, 360, 0.05], [0.5, 0.1, 0.1, 0.1, 0.1, 0.2]
             )[0],
             "n_future": random.choices(
                 [0.2, 90, 360, 0.1, 0.05], [0.5, 0.1, 0.1, 0.1, 0.2]
             )[0],
             "method": random.choice(["mean", "median"]),
+            "macro_micro": random.choice([True, False]),
         }
 
 
 class KalmanSmoothing(EmptyTransformer):
     """Apply a Kalman Filter to smooth data given a transition matrix.
 
     Args:
@@ -3606,22 +3720,190 @@
             holiday_params = HolidayTransformer.get_new_params(method="fast")
             holiday_params["regression_params"] = regression_params
             holiday_params["impact"] = 'datepart_regression'
         else:
             holiday_params = None
 
         return {
-            "sigma": random.choices([0.5, 1, 1.5, 2, 3], [0.1, 0.4, 0.1, 0.3, 0.1])[0],
+            "sigma": random.choices(
+                [0.5, 1, 1.5, 2, 2.5, 3], [0.1, 0.4, 0.1, 0.3, 0.05, 0.1]
+            )[0],
             "rolling_window": 90,
             "run_order": random.choices(["season_first", "trend_first"], [0.7, 0.3])[0],
             "regression_params": regression_params,
             "holiday_params": holiday_params,
         }
 
 
+class LevelShiftMagic(EmptyTransformer):
+    """Detects and corrects for level shifts.
+
+    Args:
+        method (str): "clip" or "remove"
+        std_threshold (float): number of std devs from mean to call an outlier
+        fillna (str): fillna method to use per tools.impute.FillNA
+    """
+
+    def __init__(
+        self,
+        window_size: int = 90,
+        alpha: float = 2.5,
+        grouping_forward_limit: int = 3,
+        max_level_shifts: int = 20,
+        alignment: str = "average",
+        **kwargs,
+    ):
+        super().__init__(name="LevelShiftMagic")
+        self.window_size = window_size
+        self.alpha = alpha
+        self.grouping_forward_limit = grouping_forward_limit
+        self.max_level_shifts = max_level_shifts
+        self.alignment = alignment
+
+    @staticmethod
+    def get_new_params(method: str = "random"):
+        return {
+            "window_size": random.choices([7, 30, 90, 364], [0.1, 0.4, 0.4, 0.1], k=1)[
+                0
+            ],
+            "alpha": random.choices(
+                [1.0, 2.0, 2.5, 3.0, 3.5, 4.0], [0.05, 0.2, 0.3, 0.2, 0.15, 0.1], k=1
+            )[0],
+            "grouping_forward_limit": random.choice([2, 3, 4]),
+            "max_level_shifts": random.choice([5, 10, 30]),
+            "alignment": random.choices(
+                ["average", "last_value", "rolling_diff", "rolling_diff_3nn"],
+                [0.5, 0.2, 0.15, 0.15],
+            )[0],
+        }
+
+    def fit(self, df):
+        """Learn behavior of data to change.
+
+        Args:
+            df (pandas.DataFrame): input dataframe
+        """
+        rolling = df.rolling(self.window_size, center=False, min_periods=1).mean()
+        # pandas 1.1.0 introduction, or thereabouts
+        try:
+            indexer = pd.api.indexers.FixedForwardWindowIndexer(
+                window_size=self.window_size
+            )
+            rolling_forward = df.rolling(window=indexer, min_periods=1).mean()
+        except Exception:
+            rolling_forward = (
+                df.loc[::-1]
+                .rolling(self.window_size, center=False, min_periods=1)
+                .mean()[::-1]
+            )
+        # compare rolling forward and backwards diffs
+        diff = rolling - rolling_forward
+        threshold = diff.std() * self.alpha
+        diff_abs = diff.abs()
+        diff_mask_0 = diff_abs > threshold  #  | (diff < -threshold)
+        # merge nearby groups
+        diff_smoothed = diff_abs.where(diff_mask_0, np.nan).fillna(
+            method='ffill', limit=self.grouping_forward_limit
+        )
+        diff_mask = (diff_smoothed > threshold) | (diff_smoothed < -threshold)
+        # the max of each changepoint group is the chosen changepoint of the level shift
+        # doesn't handle identical maxes although that is unlikely with these floating point averages
+        maxes = diff_abs.where(diff_mask, np.nan).max()
+        # group ids are needed so that we can progressively remove
+        range_arr = pd.DataFrame(
+            np.mgrid[0 : df.shape[0] : 1, 0 : df.shape[1]][0],
+            index=df.index,
+            columns=df.columns,
+        )
+        group_ids = range_arr[~diff_mask].fillna(method='ffill')  # [diff_mask]
+        max_mask = diff_abs == maxes
+        used_groups = group_ids[max_mask].mean()
+        curr_diff = diff_abs.where(((group_ids != used_groups) & diff_mask), np.nan)
+        curr_diff_sum = np.nansum(curr_diff.to_numpy())
+        count = 0
+        # logic only handles one level shift at a time, so loop if multiple level shifts
+        while curr_diff_sum != 0 and count < self.max_level_shifts:
+            curr_maxes = curr_diff.max()
+            max_mask = max_mask | (curr_diff == curr_maxes)
+            used_groups = group_ids[curr_diff == curr_maxes].mean()
+            curr_diff = curr_diff.where(
+                ((group_ids != used_groups) & diff_mask), np.nan
+            )
+            curr_diff_sum = np.sum(~curr_diff.isnull().to_numpy())
+            count += 1
+        # alignment is tricky, especially when level shifts are a mix of gradual and instantaneous
+        if self.alignment == "last_value":
+            self.lvlshft = (
+                (df[max_mask] - df[max_mask.shift(1)].shift(-1))
+                .fillna(0)
+                .loc[::-1]
+                .cumsum()[::-1]
+            )
+        elif self.alignment == "average":
+            # average the two other approaches
+            lvlshft1 = (
+                (df[max_mask] - df[max_mask.shift(1)].shift(-1))
+                .fillna(0)
+                .loc[::-1]
+                .cumsum()[::-1]
+            )
+            lvlshft2 = diff[max_mask].fillna(0).loc[::-1].cumsum()[::-1]
+            self.lvlshft = (lvlshft1 + lvlshft2) / 2
+        elif self.alignment == "rolling_diff_3nn":
+            self.lvlshft = (
+                (
+                    (
+                        diff[max_mask.shift(1)].shift(-1).fillna(0)
+                        + diff[max_mask]
+                        + diff[max_mask.shift(-1)].shift(1).fillna(0)
+                    )
+                    / 3
+                )
+                .fillna(0)
+                .loc[::-1]
+                .cumsum()[::-1]
+            )
+        else:
+            self.lvlshft = diff[max_mask].fillna(0).loc[::-1].cumsum()[::-1]
+
+        return self
+
+    def transform(self, df):
+        """Return changed data.
+
+        Args:
+            df (pandas.DataFrame): input dataframe
+        """
+        return df - self.lvlshft.reindex(index=df.index, columns=df.columns).fillna(
+            method='bfill'
+        ).fillna(0)
+
+    def inverse_transform(self, df, trans_method: str = "forecast"):
+        """Return data to original *or* forecast form.
+
+        Args:
+            df (pandas.DataFrame): input dataframe
+        """
+        return df + self.lvlshft.reindex(index=df.index, columns=df.columns).fillna(
+            method='bfill'
+        ).fillna(0)
+
+    def fit_transform(self, df):
+        """Fits and Returns *Magical* DataFrame.
+
+        Args:
+            df (pandas.DataFrame): input dataframe
+        """
+        self.fit(df)
+        return self.transform(df)
+
+
+LevelShiftTransformer = LevelShiftMagic
+
+
 # lookup dict for all non-parameterized transformers
 trans_dict = {
     "None": EmptyTransformer(),
     None: EmptyTransformer(),
     "RollingMean10": RollingMeanTransformer(window=10),
     "DifferencedTransformer": DifferencedTransformer(),
     "PctChangeTransformer": PctChangeTransformer(),
@@ -3683,14 +3965,16 @@
     "AnomalyRemoval": AnomalyRemoval,  # not shared as long as output is 'multivariate'
     "HolidayTransformer": HolidayTransformer,
     "LocalLinearTrend": LocalLinearTrend,
     "KalmanSmoothing": KalmanSmoothing,
     "RegressionFilter": RegressionFilter,
     "DatepartRegression": DatepartRegressionTransformer,
     "DatepartRegressionTransformer": DatepartRegressionTransformer,
+    "LevelShiftMagic": LevelShiftMagic,
+    "LevelShiftTransformer": LevelShiftTransformer,
 }
 # where results will vary if not all series are included together
 shared_trans = [
     "PCA",
     "FastICA",
     "DatepartRegression",
     "MeanDifference",
@@ -4192,15 +4476,16 @@
     "BTCD": 0.01,
     "Cointegration": 0.01,
     "AlignLastValue": 0.2,
     "AnomalyRemoval": 0.03,
     'HolidayTransformer': 0.01,
     'LocalLinearTrend': 0.01,
     'KalmanSmoothing': 0.04,
-    'RegressionFilter': 0.03,
+    'RegressionFilter': 0.07,
+    "LevelShiftTransformer": 0.03,
 }
 # remove any slow transformers
 fast_transformer_dict = transformer_dict.copy()
 # del fast_transformer_dict["SinTrend"]
 del fast_transformer_dict["FastICA"]
 del fast_transformer_dict["Cointegration"]
 del fast_transformer_dict["BTCD"]
@@ -4270,14 +4555,17 @@
     "zero": 0.05,
     "ffill_mean_biased": 0.1,
     "median": 0.03,
     None: 0.001,
     "interpolate": 0.4,
     "KNNImputer": 0.05,
     "IterativeImputerExtraTrees": 0.0001,  # and this one is even slower
+    "SeasonalityMotifImputer": 0.1,
+    "SeasonalityMotifImputerLinMix": 0.02,
+    "DatepartRegressionImputer": 0.05,  # also slow
 }
 
 
 def transformer_list_to_dict(transformer_list):
     """Convert various possibilities to dict."""
     if not transformer_list or transformer_list == "all":
         transformer_list = transformer_dict
@@ -4337,14 +4625,15 @@
     # filter na_probs if Fast
     params_method = None
     if fast_params:
         params_method = "fast"
         throw_away = na_prob_dict.pop("IterativeImputer", None)
         throw_away = df_interpolate.pop("spline", None)  # noqa
         throw_away = na_prob_dict.pop("IterativeImputerExtraTrees", None)  # noqa
+        throw_away = na_prob_dict.pop("DatepartRegressionImputer", None)  # noqa
     if superfast_params:
         params_method = "fast"
         throw_away = na_prob_dict.pop("KNNImputer", None)  # noqa
 
     # clean na_probs dict
     na_probabilities = list(na_prob_dict.values())
     na_probs_list = [*na_prob_dict]
```

### Comparing `autots-0.5.8/autots/tools/window_functions.py` & `autots-0.6.0/autots/tools/window_functions.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/docs/conf.py` & `autots-0.6.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 copyright = u'%s, Colin Catlin' % date.today().year
 author = 'Colin Catlin'
 
 # The full version, including alpha/beta/rc tags
 # import AutoTS
 # from  AutoTS import __version__
 # release = __version__
-release = "0.5.8"
+release = "0.6.0"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 # Add napoleon to the extensions list
```

### Comparing `autots-0.5.8/pyproject.toml` & `autots-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autots"
-version = "0.5.8"
+version = "0.6.0"
 authors = [
   { name="Colin Catlin", email="colin.catlin@gmail.com" },
 ]
 description = "Automated Time Series Forecasting"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {text = "MIT License"}
```

### Comparing `autots-0.5.8/setup.py` & `autots-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 }
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AutoTS",
-    version="0.5.8",
+    version="0.6.0",
     author="Colin Catlin",
     author_email="colin.catlin@syllepsis.live",
     description="Automated Time Series Forecasting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/winedarksea/AutoTS",
     packages=setuptools.find_packages(),
```

### Comparing `autots-0.5.8/tests/test_anomalies.py` & `autots-0.6.0/tests/test_anomalies.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/tests/test_autots.py` & `autots-0.6.0/tests/test_autots.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 """Overall testing."""
 import unittest
 import json
 import time
 import timeit
+import tempfile
+import os
 import numpy as np
 import pandas as pd
 from autots.datasets import (
     load_daily, load_monthly, load_artificial, load_sine
 )
 from autots import AutoTS, model_forecast
 from autots.evaluator.auto_ts import fake_regressor
@@ -19,59 +21,71 @@
 
 class AutoTSTest(unittest.TestCase):
 
     def test_autots(self):
         print("Starting AutoTS class tests")
         forecast_length = 8
         long = False
-        df = load_daily(long=long).drop(columns=['US.Total.Covid.Tests'], errors='ignore')
+        df = load_daily(long=long)
         n_jobs = 'auto'
         verbose = 0
         validation_method = "backwards"
         generations = 1
         num_validations = 2
-        models_to_validate = 0.35  # must be a decimal percent for this test
+        models_to_validate = 0.25  # must be a decimal percent for this test
 
         model_list = [
             'ConstantNaive',
             'LastValueNaive',
             'AverageValueNaive',
             'SeasonalNaive',
+            'DatepartRegression',
         ]
 
         transformer_list = "fast"  # ["SinTrend", "MinMaxScaler"]
         transformer_max_depth = 3
 
         metric_weighting = {
             'smape_weighting': 3,
             'mae_weighting': 1,
             'rmse_weighting': 1,
             'containment_weighting': 0,
             'runtime_weighting': 0,
             'spl_weighting': 1,
             'contour_weighting': 1,
         }
+        ensemble = [
+            'simple',
+            # 'distance',
+            # 'horizontal',
+            'horizontal-max',
+            # 'mosaic',
+            'mosaic-window',
+            'mosaic-crosshair'
+            # 'subsample',
+            # 'mlensemble',
+        ]
 
         model = AutoTS(
             forecast_length=forecast_length,
             frequency='infer',
             prediction_interval=0.9,
-            ensemble='all',
+            ensemble=ensemble,
             constraint=None,
             max_generations=generations,
             num_validations=num_validations,
             validation_method=validation_method,
             model_list=model_list,
             transformer_list=transformer_list,
             transformer_max_depth=transformer_max_depth,
             initial_template='General+Random',
             metric_weighting=metric_weighting,
             models_to_validate=models_to_validate,
             max_per_model_class=None,
-            model_interrupt=False,
+            model_interrupt="end_generation",
             no_negatives=True,
             subset=100,
             n_jobs=n_jobs,
             drop_most_recent=1,
             verbose=verbose,
         )
         future_regressor_train2d, future_regressor_forecast2d = fake_regressor(
@@ -89,14 +103,15 @@
             df,
             future_regressor=future_regressor_train2d,
             date_col='datetime' if long else None,
             value_col='value' if long else None,
             id_col='series_id' if long else None,
         )
         prediction = model.predict(future_regressor=future_regressor_forecast2d, verbose=0)
+        long_form = prediction.long_form_results()
         forecasts_df = prediction.forecast
         initial_results = model.results()
         validation_results = model.results("validation")
         back_forecast = model.back_forecast(n_splits=2, verbose=0).forecast
         # validated_count = (validation_results['Runs'] == (num_validations + 1)).sum()
 
         # so these account for DROP MOST RECENT = 1
@@ -129,15 +144,14 @@
         self.assertTrue((expected_idx == pd.DatetimeIndex(forecasts_df.index)).all())
         # these next two could potentiall fail if any inputs have a strong trend
         self.assertTrue((forecasts_df.mean() <= (df.max()) + df.std()).all())
         self.assertTrue((forecasts_df.mean() >= (df.min()) - df.std()).all())
         # check all the checks work
         self.assertEqual(model.ensemble_check, 1)
         self.assertFalse(model.weighted)
-        self.assertFalse(model.used_regressor_check)
         self.assertFalse(model.subset_flag)
         # assess 'backwards' validation
         self.assertEqual(len(model.validation_test_indexes), num_validations + 1)
         self.assertTrue(model.validation_test_indexes[1].intersection(model.validation_train_indexes[1]).empty)
         self.assertTrue(model.validation_test_indexes[2].intersection(model.validation_train_indexes[2]).empty)
         self.assertEqual(model.validation_train_indexes[1].shape[0], df.shape[0] - (forecast_length * 2 + 1))  # +1 via drop most recent
         self.assertTrue((model.validation_test_indexes[1] == expected_val1).all())
@@ -152,22 +166,79 @@
             self.assertEqual(len(set(template_dict['series'].values())), template_dict['model_count'])
         self.assertEqual(len(template_dict['models'].keys()), template_dict['model_count'])
         # test that actually the best model (or nearly) was chosen
         self.assertGreater(validation_results['Score'].quantile(0.05), best_model_result['Score'].iloc[0])
         # test back_forecast
         # self.assertTrue((back_forecast.index == model.df_wide_numeric.index).all(), msg="Back forecasting failed to have equivalent index to train.")
         self.assertFalse(np.any(back_forecast.isnull()))
+        self.assertEqual(long_form.shape[0], forecasts_df.shape[0] * forecasts_df.shape[1] * 3)
+
+        # TEST EXPORTING A TEMPLATE THEN USING THE BEST MODEL AS A PREDICTION
+        df_train = df.iloc[:-forecast_length]
+        df_test = df.iloc[-forecast_length:]
+        tf = tempfile.NamedTemporaryFile(suffix='.csv', prefix=os.path.basename("autots_test"), delete=False)
+        time.sleep(1)
+        name = tf.name
+        model.export_template(name, models="best", n=20, max_per_model_class=3)
+        
+        model2 = AutoTS(
+            forecast_length=forecast_length,
+            frequency='infer',
+            prediction_interval=0.9,
+            ensemble='all',
+            constraint=None,
+            max_generations=generations,
+            num_validations=num_validations,
+            validation_method=validation_method,
+            model_list="update_fit",
+            transformer_list=transformer_list,
+            transformer_max_depth=transformer_max_depth,
+            initial_template='General+Random',
+            metric_weighting=metric_weighting,
+            models_to_validate=models_to_validate,
+            max_per_model_class=None,
+            model_interrupt=False,
+            no_negatives=True,
+            subset=100,
+            n_jobs=n_jobs,
+            drop_most_recent=1,
+            verbose=2,
+        )
+        # TEST MODEL PREDICT WITH LOWER LEVEL MODEL TRAINED ON PREVIOUS DATA ONLY
+        model2.import_best_model(tf.name, include_ensemble=False)
+        model2.fit_data(df_train, future_regressor=future_regressor_train2d.reindex(df_train.index))
+        prediction = model2.predict(future_regressor=future_regressor_forecast2d.reindex(df_test.index), verbose=0)
+        prediction.evaluate(df_test, df_train=df_train)
+        smape1 = prediction.avg_metrics['smape']
+        
+        model2.fit_data(df, future_regressor=future_regressor_train2d)
+        prediction2 = model2.predict(future_regressor=future_regressor_forecast2d, verbose=0)
+        forecasts_df2 = prediction2.forecast
+        
+        # now retrain on full data
+        model2.model = None
+        model2.fit_data(df, future_regressor=future_regressor_train2d)
+        prediction2 = model2.predict(future_regressor=future_regressor_forecast2d, verbose=0)
+        # and see if it got better on past holdout
+        model2.fit_data(df_train, future_regressor=future_regressor_train2d.reindex(df_train.index))
+        prediction = model2.predict(future_regressor=future_regressor_forecast2d.reindex(df_test.index), verbose=0)
+        prediction.evaluate(df_test, df_train=df_train)
+        smape2 = prediction.avg_metrics['smape']
+        print("=====================================================")
+        # smape2 should be better because it is trained on the very data it is supposed to predict
+        print(f"fit 1 SMAPE {smape1}, then refit with history SMAPE: {smape2}")
+
+        tf.close()
+        os.unlink(tf.name)
+
+        
+        self.assertEqual(forecasts_df2.shape[0], forecast_length)
+        self.assertEqual(forecasts_df2.shape[1], df.shape[1])
+        self.assertFalse(forecasts_df2.isna().any().any())
 
-        # a
-        # b
-        # c
-        # d
-        # e
-        # f
-        # g
     def test_all_default_models(self):
         print("Starting test_all_default_models")
         forecast_length = 8
         long = False
         df = load_daily(long=long).drop(columns=['US.Total.Covid.Tests'], errors='ignore')
         # to make it faster
         df = df[df.columns[0:2]]
@@ -247,14 +318,15 @@
         # these next two could potentiall fail if any inputs have a strong trend
         self.assertTrue((forecasts_df.mean() <= (df.max()) + df.std()).all())
         self.assertTrue((forecasts_df.mean() >= (df.min()) - df.std()).all())
         # check all the checks work
         self.assertEqual(model.ensemble_check, 1)
         self.assertFalse(model.weighted)
         self.assertFalse(model.subset_flag)
+        self.assertFalse(model.used_regressor_check)
         # assess 'backwards' validation
         val_1 = model.validation_test_indexes[1]
         self.assertEqual(len(model.validation_test_indexes), num_validations + 1)
         self.assertTrue(val_1.intersection(model.validation_train_indexes[1]).empty)
         self.assertEqual(model.validation_train_indexes[1].shape[0], df.shape[0] - (forecast_length * 2 + 1))  # +1 via drop most recent
         self.assertTrue((val_1 == expected_val1).all())
         # assess Horizontal Ensembling
@@ -397,14 +469,16 @@
 
     def test_models(self):
         """Test if models are the same as saved comparisons."""
         print("Starting test_models")
         n_jobs = 1
         random_seed = 300
         df = load_daily(long=False).iloc[:, 0:5]
+        df = df[df.index < "2022-10-04"]  # update dataset and have not yet updated stored model results
+        df = df[df.index > "2017-10-04"]  # update dataset and have not yet updated stored model results
         models = [
             'SectionalMotif', 'MultivariateMotif', 'AverageValueNaive',
             'NVAR', "LastValueNaive", 'Theta', 'FBProphet', 'SeasonalNaive',
             'GLM', 'ETS', "ConstantNaive", 'WindowRegression',
             'DatepartRegression', 'MultivariateRegression',
             'Cassandra', 'MetricMotif', 'SeasonalityMotif', 'KalmanStateSpace',
             'ARDL', 'UnivariateMotif', 'VAR', 'MAR', 'TMF', 'RRVAR', 'VECM',
@@ -628,7 +702,136 @@
                     'forecasts': forecasts,
                     "upper_forecasts": upper_forecasts,
                     "lower_forecasts": lower_forecasts,
                     "timing": timings,
                 }, file
             )
         """
+
+    def test_sklearn(self):
+        from autots import load_daily
+        from autots import create_regressor
+        from autots.models.sklearn import MultivariateRegression, DatepartRegression, WindowRegression
+
+        df = load_daily(long=False)
+        forecast_length = 8
+        df_train = df.iloc[:-forecast_length]
+        df_test = df.iloc[-forecast_length:]
+        future_regressor_train, future_regressor_forecast = create_regressor(
+            df_train,
+            forecast_length=forecast_length,
+            frequency="infer",
+            drop_most_recent=0,
+            scale=True,
+            summarize="auto",
+            backfill="bfill",
+            fill_na="spline",
+            holiday_countries={"US": None},  # requires holidays package
+            encode_holiday_type=True,
+        )
+
+        random_seed = 300
+        frequency = 'D'
+        prediction_interval = 0.9
+        verbose = -1
+        n_jobs = 2
+
+        params = MultivariateRegression().get_new_params()
+        params = {
+            'regression_model': {'model': 'LightGBM',
+            'model_params': {
+                'objective': 'regression',
+                'learning_rate': 0.1,
+                'num_leaves': 31,
+                'max_depth': 10,
+                'boosting_type': 'goss',
+                 'n_estimators': 250,
+                'linear_tree': False
+            }},
+            'mean_rolling_periods': 90,
+            'macd_periods': 12,
+            'std_rolling_periods': 7,
+            'max_rolling_periods': None,
+            'min_rolling_periods': None,
+            'quantile90_rolling_periods': 7,
+            'quantile10_rolling_periods': 10,
+            'ewm_alpha': 0.8,
+            'ewm_var_alpha': None,
+            'additional_lag_periods': None,
+            'abs_energy': False,
+            'rolling_autocorr_periods': None,
+            'datepart_method': 'expanded',
+            'polynomial_degree': None,
+            'regression_type': None,
+            'window': 3,
+            'holiday': True,
+            'probabilistic': False,
+            'cointegration': None,
+            'cointegration_lag': 1
+        }
+        model = MultivariateRegression(
+            forecast_length=forecast_length,
+            frequency=frequency,
+            prediction_interval=prediction_interval,
+            random_seed=random_seed,
+            verbose=verbose,
+            n_jobs=n_jobs,
+            **params
+        )
+        model.fit(df_train)
+        first_forecast = model.predict(future_regressor=future_regressor_forecast)
+        self.assertListEqual(first_forecast.forecast.index.tolist(), df_test.index.tolist())
+        model.fit_data(df)
+        updated_forecast = model.predict()
+        self.assertEqual(updated_forecast.forecast.shape[0], forecast_length)
+        self.assertTrue(updated_forecast.forecast.index[0] > df.index[-1])
+
+        params = WindowRegression().get_new_params()
+        params = {}
+        model = WindowRegression(
+            forecast_length=forecast_length,
+            frequency=frequency,
+            prediction_interval=prediction_interval,
+            random_seed=random_seed,
+            verbose=verbose,
+            n_jobs=n_jobs,
+            **params
+        )
+        model.fit(df_train.fillna(method='ffill'))
+        first_forecast = model.predict(future_regressor=future_regressor_forecast)
+        # first_forecast.plot_grid(df)
+        self.assertListEqual(first_forecast.forecast.index.tolist(), df_test.index.tolist())
+        model.fit_data(df)
+        updated_forecast = model.predict()
+        # updated_forecast.plot_grid(df)
+        self.assertEqual(updated_forecast.forecast.shape[0], forecast_length)
+        self.assertTrue(updated_forecast.forecast.index[0] > df.index[-1])
+
+
+        params = {
+            'regression_model': {
+                'model': 'ExtraTrees',
+                'model_params': {
+                    'n_estimators': 500,
+                    'min_samples_leaf': 1,
+                    'max_depth': 20
+            }},
+            'datepart_method': 'simple_binarized',
+            'polynomial_degree': None,
+            'regression_type': None,
+        }
+        model = DatepartRegression(
+            forecast_length=forecast_length,
+            frequency=frequency,
+            prediction_interval=prediction_interval,
+            random_seed=random_seed,
+            verbose=verbose,
+            n_jobs=n_jobs,
+            **params
+        )
+        model.fit(df_train)
+        first_forecast = model.predict(future_regressor=future_regressor_forecast)
+        self.assertListEqual(first_forecast.forecast.index.tolist(), df_test.index.tolist())
+        model.fit_data(df)
+        updated_forecast = model.predict()
+        self.assertEqual(updated_forecast.forecast.shape[0], forecast_length)
+        self.assertTrue(updated_forecast.forecast.index[0] > df.index[-1])
```

### Comparing `autots-0.5.8/tests/test_calendar_holiday.py` & `autots-0.6.0/tests/test_calendar_holiday.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/tests/test_cassandra.py` & `autots-0.6.0/tests/test_cassandra.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,15 @@
             mod.create_forecast_index(forecast_length, last_date=df_daily.index[-1])
         )
         regr_ps = {
             "wiki_Germany": regr_per_series_fcst["wiki_Germany"].reindex(
                 dates, fill_value=0
             )
         }
+        mod.past_impacts_intervention = None
         pred2 = mod.predict(
             forecast_length=forecast_length,
             include_history=True,
             new_df=df_daily[df_train.columns],
             flag_regressors=flag_regressor_fcst.reindex(dates, fill_value=0),
             future_regressor=fake_regr_fcst.reindex(dates, fill_value=0),
             regressor_per_series=regr_ps,
```

### Comparing `autots-0.5.8/tests/test_event_forecasting.py` & `autots-0.6.0/tests/test_event_forecasting.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/tests/test_impute.py` & `autots-0.6.0/tests/test_impute.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/tests/test_metrics.py` & `autots-0.6.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/tests/test_percentile.py` & `autots-0.6.0/tests/test_percentile.py`

 * *Files identical despite different names*

### Comparing `autots-0.5.8/tests/test_regressor.py` & `autots-0.6.0/tests/test_regressor.py`

 * *Files identical despite different names*

