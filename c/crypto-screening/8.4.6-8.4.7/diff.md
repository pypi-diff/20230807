# Comparing `tmp/crypto-screening-8.4.6.tar.gz` & `tmp/crypto-screening-8.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.4.6.tar", last modified: Mon Aug  7 12:22:50 2023, max compression
+gzip compressed data, was "crypto-screening-8.4.7.tar", last modified: Mon Aug  7 12:49:31 2023, max compression
```

## Comparing `crypto-screening-8.4.6.tar` & `crypto-screening-8.4.7.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.786620 crypto-screening-8.4.6/
--rw-rw-rw-   0        0        0      196 2023-08-07 12:22:48.000000 crypto-screening-8.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-08-07 12:22:50.786620 crypto-screening-8.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.4.6/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.4.6/build.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.554217 crypto-screening-8.4.6/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.586065 crypto-screening-8.4.6/crypto_screening/collect/
--rw-rw-rw-   0        0        0    16968 2023-08-02 06:37:38.000000 crypto-screening-8.4.6/crypto_screening/collect/assets.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.592067 crypto-screening-8.4.6/crypto_screening/collect/foundation/
--rw-rw-rw-   0        0        0     4943 2023-07-31 16:05:02.000000 crypto-screening-8.4.6/crypto_screening/collect/foundation/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.619916 crypto-screening-8.4.6/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.4.6/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.4.6/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.4.6/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.4.6/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.642811 crypto-screening-8.4.6/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.4.6/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24329 2023-07-30 10:08:09.000000 crypto-screening-8.4.6/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    15451 2023-07-30 10:04:40.000000 crypto-screening-8.4.6/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21291 2023-07-30 10:08:09.000000 crypto-screening-8.4.6/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15119 2023-07-31 16:05:02.000000 crypto-screening-8.4.6/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    21356 2023-07-31 05:18:32.000000 crypto-screening-8.4.6/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    21677 2023-08-02 06:37:38.000000 crypto-screening-8.4.6/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    15804 2023-07-30 10:04:16.000000 crypto-screening-8.4.6/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.4.6/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.4.6/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.704007 crypto-screening-8.4.6/crypto_screening/screeners/
--rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.4.6/crypto_screening/screeners/__init__.py
--rw-rw-rw-   0        0        0    24218 2023-07-31 04:58:29.000000 crypto-screening-8.4.6/crypto_screening/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.727050 crypto-screening-8.4.6/crypto_screening/screeners/callbacks/
--rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.4.6/crypto_screening/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.4.6/crypto_screening/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4400 2023-07-30 10:12:51.000000 crypto-screening-8.4.6/crypto_screening/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.4.6/crypto_screening/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.747045 crypto-screening-8.4.6/crypto_screening/screeners/collectors/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.4.6/crypto_screening/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6253 2023-07-30 10:04:48.000000 crypto-screening-8.4.6/crypto_screening/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.4.6/crypto_screening/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.4.6/crypto_screening/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12296 2023-08-04 14:46:12.000000 crypto-screening-8.4.6/crypto_screening/screeners/combined.py
--rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.4.6/crypto_screening/screeners/container.py
--rw-rw-rw-   0        0        0    11146 2023-07-31 16:05:02.000000 crypto-screening-8.4.6/crypto_screening/screeners/database.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.768080 crypto-screening-8.4.6/crypto_screening/screeners/foundation/
--rw-rw-rw-   0        0        0    11778 2023-08-07 10:03:36.000000 crypto-screening-8.4.6/crypto_screening/screeners/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.4.6/crypto_screening/screeners/foundation/protocols.py
--rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.4.6/crypto_screening/screeners/foundation/state.py
--rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.4.6/crypto_screening/screeners/foundation/waiting.py
--rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.4.6/crypto_screening/screeners/market.py
--rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.4.6/crypto_screening/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.4.6/crypto_screening/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.4.6/crypto_screening/screeners/orders.py
--rw-rw-rw-   0        0        0    17635 2023-08-07 12:22:32.000000 crypto-screening-8.4.6/crypto_screening/screeners/recorder.py
--rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.4.6/crypto_screening/screeners/trades.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.4.6/crypto_screening/screeners/waiting.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.519667 crypto-screening-8.4.6/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.773080 crypto-screening-8.4.6/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.4.6/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10527 2023-07-31 05:20:01.000000 crypto-screening-8.4.6/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.785651 crypto-screening-8.4.6/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.4.6/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.4.6/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3855 2023-08-02 06:33:48.000000 crypto-screening-8.4.6/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-08-07 12:22:50.568596 crypto-screening-8.4.6/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-08-07 12:22:50.000000 crypto-screening-8.4.6/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2156 2023-08-07 12:22:50.000000 crypto-screening-8.4.6/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 12:22:50.000000 crypto-screening-8.4.6/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-08-07 12:22:50.000000 crypto-screening-8.4.6/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-07 12:22:50.000000 crypto-screening-8.4.6/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-08-07 12:22:48.000000 crypto-screening-8.4.6/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.4.6/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.4.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 12:22:50.786620 crypto-screening-8.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-08-07 12:22:45.000000 crypto-screening-8.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.843043 crypto-screening-8.4.7/
+-rw-rw-rw-   0        0        0      196 2023-08-07 12:49:31.000000 crypto-screening-8.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-08-07 12:49:31.843043 crypto-screening-8.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.4.7/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.4.7/build.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.796042 crypto-screening-8.4.7/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.816078 crypto-screening-8.4.7/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    16968 2023-08-02 06:37:38.000000 crypto-screening-8.4.7/crypto_screening/collect/assets.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.816078 crypto-screening-8.4.7/crypto_screening/collect/foundation/
+-rw-rw-rw-   0        0        0     4943 2023-07-31 16:05:02.000000 crypto-screening-8.4.7/crypto_screening/collect/foundation/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.821070 crypto-screening-8.4.7/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.4.7/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.4.7/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.4.7/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.4.7/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.824056 crypto-screening-8.4.7/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.4.7/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24329 2023-07-30 10:08:09.000000 crypto-screening-8.4.7/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    15451 2023-07-30 10:04:40.000000 crypto-screening-8.4.7/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21291 2023-07-30 10:08:09.000000 crypto-screening-8.4.7/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15119 2023-07-31 16:05:02.000000 crypto-screening-8.4.7/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    21356 2023-07-31 05:18:32.000000 crypto-screening-8.4.7/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    21677 2023-08-02 06:37:38.000000 crypto-screening-8.4.7/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    15804 2023-07-30 10:04:16.000000 crypto-screening-8.4.7/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.4.7/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.4.7/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.833042 crypto-screening-8.4.7/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.4.7/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    24218 2023-07-31 04:58:29.000000 crypto-screening-8.4.7/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.835043 crypto-screening-8.4.7/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.4.7/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.4.7/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-30 10:12:51.000000 crypto-screening-8.4.7/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.4.7/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.837043 crypto-screening-8.4.7/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.4.7/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6253 2023-07-30 10:04:48.000000 crypto-screening-8.4.7/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.4.7/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6445 2023-08-07 12:47:36.000000 crypto-screening-8.4.7/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12296 2023-08-04 14:46:12.000000 crypto-screening-8.4.7/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.4.7/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    11146 2023-07-31 16:05:02.000000 crypto-screening-8.4.7/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.840043 crypto-screening-8.4.7/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    12592 2023-08-07 12:49:29.000000 crypto-screening-8.4.7/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.4.7/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.4.7/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.4.7/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.4.7/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.4.7/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.4.7/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.4.7/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    17635 2023-08-07 12:22:32.000000 crypto-screening-8.4.7/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.4.7/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.4.7/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.788047 crypto-screening-8.4.7/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.840043 crypto-screening-8.4.7/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.4.7/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10527 2023-07-31 05:20:01.000000 crypto-screening-8.4.7/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.842041 crypto-screening-8.4.7/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.4.7/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.4.7/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3855 2023-08-02 06:33:48.000000 crypto-screening-8.4.7/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:49:31.813041 crypto-screening-8.4.7/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-08-07 12:49:31.000000 crypto-screening-8.4.7/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2156 2023-08-07 12:49:31.000000 crypto-screening-8.4.7/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 12:49:31.000000 crypto-screening-8.4.7/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-08-07 12:49:31.000000 crypto-screening-8.4.7/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-07 12:49:31.000000 crypto-screening-8.4.7/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-08-07 12:49:31.000000 crypto-screening-8.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.4.7/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.4.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 12:49:31.843043 crypto-screening-8.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-08-07 12:49:29.000000 crypto-screening-8.4.7/setup.py
```

### Comparing `crypto-screening-8.4.6/PKG-INFO` & `crypto-screening-8.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.4.6
+Version: 8.4.7
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.4.6/README.md` & `crypto-screening-8.4.7/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/build.py` & `crypto-screening-8.4.7/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/collect/assets.py` & `crypto-screening-8.4.7/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/collect/foundation/exchanges.py` & `crypto-screening-8.4.7/crypto_screening/collect/foundation/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.4.7/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.4.7/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/collect/market/orders.py` & `crypto-screening-8.4.7/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.4.7/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.4.7/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.4.7/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/collect/market/trades.py` & `crypto-screening-8.4.7/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/collect/screeners.py` & `crypto-screening-8.4.7/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/collect/symbols.py` & `crypto-screening-8.4.7/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/dataset.py` & `crypto-screening-8.4.7/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/exchanges.py` & `crypto-screening-8.4.7/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/interval.py` & `crypto-screening-8.4.7/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/base.py` & `crypto-screening-8.4.7/crypto_screening/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/callbacks/base.py` & `crypto-screening-8.4.7/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/callbacks/database.py` & `crypto-screening-8.4.7/crypto_screening/screeners/callbacks/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/callbacks/sockets.py` & `crypto-screening-8.4.7/crypto_screening/screeners/callbacks/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/collectors/base.py` & `crypto-screening-8.4.7/crypto_screening/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/collectors/database.py` & `crypto-screening-8.4.7/crypto_screening/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/collectors/sockets.py` & `crypto-screening-8.4.7/crypto_screening/screeners/collectors/sockets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # sockets.py
 
 import json
+import warnings
 import asyncio
 import datetime as dt
 from typing import Dict, Any, Optional, Union, Iterable, List, Tuple
 
 from crypto_screening.screeners.callbacks import SocketCallback, BaseCallback
 from crypto_screening.screeners.base import BaseScreener
 from crypto_screening.screeners.collectors.base import ScreenersDataCollector
@@ -156,15 +157,25 @@
         Receives the data from the senders.
 
         :param reader: The data reader.
         :param writer: The data writer.
         """
 
         while self.screening:
-            await self.receive(reader=reader, writer=writer)
+            try:
+                await self.receive(reader=reader, writer=writer)
+
+            except (
+                ConnectionResetError, ConnectionError,
+                ConnectionAbortedError, ConnectionRefusedError
+            ) as e:
+                warnings.warn(str(e))
+
+                self.terminate()
+            # end try
         # end while
     # end receiving_loop
 
     def screening_loop(
             self,
             loop: Optional[asyncio.AbstractEventLoop] = None
     ) -> None:
```

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/combined.py` & `crypto-screening-8.4.7/crypto_screening/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/container.py` & `crypto-screening-8.4.7/crypto_screening/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/database.py` & `crypto-screening-8.4.7/crypto_screening/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/foundation/data.py` & `crypto-screening-8.4.7/crypto_screening/screeners/foundation/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     LOCATION = "datasets"
 
     DELAY = 0
     CANCEL = 0
 
     __slots__ = (
-        "location", "delay", "cancel", "_screening",
+        "location", "delay", "cancel", "_screening", "_timeout",
         "_blocking", "_saving", "_updating", "_screening_process",
         "_timeout_process", "_saving_process", "_updating_process"
     )
 
     def __init__(
             self,
             location: Optional[str] = None,
@@ -82,14 +82,15 @@
 
         self.location = location or self.LOCATION
 
         self._screening = False
         self._blocking = False
         self._saving = False
         self._updating = False
+        self._timeout = False
 
         self._screening_process: Optional[threading.Thread] = None
         self._timeout_process: Optional[threading.Thread] = None
         self._saving_process: Optional[threading.Thread] = None
         self._updating_process: Optional[threading.Thread] = None
     # end __init__
 
@@ -151,26 +152,67 @@
 
         :return: The value.
         """
 
         return self._updating
     # end updating
 
+    @property
+    def timeout(self) -> bool:
+        """
+        returns the value of the process being blocked.
+
+        :return: The value.
+        """
+
+        return self._timeout
+    # end timeout
+
     def screening_loop(self) -> None:
         """Runs the process of the price screening."""
     # end screening_loop
 
     def saving_loop(self) -> None:
         """Runs the process of the price screening."""
     # end saving_loop
 
     def update_loop(self) -> None:
         """Updates the state of the screeners."""
     # end update_loop
 
+    def timeout_loop(self, duration: Union[float, dt.timedelta, dt.datetime]) -> None:
+        """
+        Runs a timeout for the process.
+
+        :param duration: The duration of the start_timeout.
+
+        :return: The start_timeout process.
+        """
+
+        self._timeout = True
+
+        if isinstance(duration, (int, float)):
+            duration = dt.timedelta(seconds=duration)
+        # end if
+
+        if isinstance(duration, dt.timedelta):
+            duration = dt.datetime.now() + duration
+        # end if
+
+        while self.timeout and (duration < dt.datetime.now()):
+            time.sleep(0.001)
+        # end while
+
+        if self.timeout:
+            self._timeout = False
+
+            self.terminate()
+        # end if
+    # end timeout_loop
+
     @abstractmethod
     def await_initialization(
             self,
             stop: Optional[Union[bool, int]] = False,
             delay: Optional[Union[float, dt.timedelta]] = None,
             cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
     ) -> WaitingState:
@@ -310,24 +352,16 @@
             self._timeout_process.is_alive()
         ):
             warnings.warn(f"Timeout process of {repr(self)} is already running.")
 
             return
         # end if
 
-        if isinstance(duration, dt.datetime):
-            duration = duration - dt.datetime.now()
-        # end if
-
-        if isinstance(duration, dt.timedelta):
-            duration = duration.total_seconds()
-        # end if
-
         self._timeout_process = threading.Thread(
-            target=lambda: (time.sleep(duration), self.terminate())
+            target=lambda: self.timeout_loop(duration=duration)
         )
 
         self._timeout_process.start()
     # end start_timeout
 
     def run(
             self,
```

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/foundation/protocols.py` & `crypto-screening-8.4.7/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/foundation/state.py` & `crypto-screening-8.4.7/crypto_screening/screeners/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/foundation/waiting.py` & `crypto-screening-8.4.7/crypto_screening/screeners/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/market.py` & `crypto-screening-8.4.7/crypto_screening/screeners/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/ohlcv.py` & `crypto-screening-8.4.7/crypto_screening/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/orderbook.py` & `crypto-screening-8.4.7/crypto_screening/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/orders.py` & `crypto-screening-8.4.7/crypto_screening/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/recorder.py` & `crypto-screening-8.4.7/crypto_screening/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/trades.py` & `crypto-screening-8.4.7/crypto_screening/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/screeners/waiting.py` & `crypto-screening-8.4.7/crypto_screening/screeners/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.4.7/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/symbols.py` & `crypto-screening-8.4.7/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/utils/base.py` & `crypto-screening-8.4.7/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/utils/process.py` & `crypto-screening-8.4.7/crypto_screening/utils/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening/validate.py` & `crypto-screening-8.4.7/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.4.7/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.4.6
+Version: 8.4.7
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.4.6/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.4.7/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.6/pyproject.toml` & `crypto-screening-8.4.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.4.6'
+version = '8.4.7'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.4.6/setup.py` & `crypto-screening-8.4.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.4.6',
+        version='8.4.7',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

