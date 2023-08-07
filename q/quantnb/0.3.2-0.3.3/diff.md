# Comparing `tmp/quantnb-0.3.2.tar.gz` & `tmp/quantnb-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantnb-0.3.2.tar", max compression
+gzip compressed data, was "quantnb-0.3.3.tar", max compression
```

## Comparing `quantnb-0.3.2.tar` & `quantnb-0.3.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0      276 2023-08-05 11:34:00.434407 quantnb-0.3.2/README.md
--rw-r--r--   0        0        0     1095 2023-08-05 11:34:00.846412 quantnb-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      282 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/__init__.py
--rw-r--r--   0        0        0     1901 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/PNL.py
--rw-r--r--   0        0        0      246 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/__init__.py
--rw-r--r--   0        0        0    12236 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/backtester.old.py
--rw-r--r--   0        0        0     4345 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/backtester.py
--rw-r--r--   0        0        0     2236 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/base.py
--rw-r--r--   0        0        0      341 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/calculate_commission.py
--rw-r--r--   0        0        0      517 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/calculate_entry_price.py
--rw-r--r--   0        0        0      516 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/calculate_exit_price.py
--rw-r--r--   0        0        0     3001 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/data_module.py
--rw-r--r--   0        0        0      847 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/enums.py
--rw-r--r--   0        0        0      473 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/helpers.py
--rw-r--r--   0        0        0     2377 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/place_orders_on_ohlc.py
--rw-r--r--   0        0        0      909 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/specs_nb.py
--rw-r--r--   0        0        0       94 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/test.py
--rw-r--r--   0        0        0      515 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/trade_add_trade_to_active_trades.py
--rw-r--r--   0        0        0      974 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/trade_close_trade.py
--rw-r--r--   0        0        0     1183 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/trade_create_new_trade.py
--rw-r--r--   0        0        0     5060 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/trade_module.py
--rw-r--r--   0        0        0      696 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/trade_remove_from_active_trades.py
--rw-r--r--   0        0        0      647 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/trade_should_trade_close.py
--rw-r--r--   0        0        0      558 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/core/update_trades_pnl.py
--rw-r--r--   0        0        0     2900 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/H_ticks_to_ranges.py
--rw-r--r--   0        0        0     1337 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/S_calculate_metrics.py
--rw-r--r--   0        0        0      357 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/S_print_orders.py
--rw-r--r--   0        0        0      754 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/S_print_trades.py
--rw-r--r--   0        0        0      300 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/__init__.py
--rw-r--r--   0        0        0      793 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/analyze_trade_duration.py
--rw-r--r--   0        0        0      380 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/calculate_average_freq.py
--rw-r--r--   0        0        0     1038 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/calculate_pf_stats.py
--rw-r--r--   0        0        0      390 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/calculate_risk_free.py
--rw-r--r--   0        0        0      213 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/get_average_trade_duration.py
--rw-r--r--   0        0        0      672 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/get_realized_pf_value.py
--rw-r--r--   0        0        0      325 2023-08-05 11:34:00.846412 quantnb-0.3.2/quantnb/helpers/plot_lines.py
--rw-r--r--   0        0        0      731 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/helpers/save_to_csv.py
--rw-r--r--   0        0        0      109 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/indicators/EMA.py
--rw-r--r--   0        0        0      351 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/indicators/HMA.py
--rw-r--r--   0        0        0     1233 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/indicators/I_donchian.py
--rw-r--r--   0        0        0      109 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/indicators/SMA.py
--rw-r--r--   0        0        0      198 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/indicators/__init__.py
--rw-r--r--   0        0        0      221 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/indicators/cross_above.py
--rw-r--r--   0        0        0      222 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/indicators/cross_below.py
--rw-r--r--   0        0        0     1732 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/indicators/random_data.py
--rw-r--r--   0        0        0     1253 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/indicators/supertrend.py
--rw-r--r--   0        0        0      505 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/__init__.py
--rw-r--r--   0        0        0     3204 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/calculate_stats.py
--rw-r--r--   0        0        0      147 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/convert_signal_to_markers.py
--rw-r--r--   0        0        0     1143 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/create_binance_dataframe.py
--rw-r--r--   0        0        0     1044 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/fetch_binance_data.py
--rw-r--r--   0        0        0      466 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/find_files.py
--rw-r--r--   0        0        0     3828 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/helpers.py
--rw-r--r--   0        0        0     1131 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/multiprocess.py
--rw-r--r--   0        0        0     1305 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/optimize.py
--rw-r--r--   0        0        0      813 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/output_trades.py
--rw-r--r--   0        0        0     4591 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/plotting.py
--rw-r--r--   0        0        0     2058 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/qs.py
--rw-r--r--   0        0        0      241 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/resample.py
--rw-r--r--   0        0        0      881 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/lib/time_manip.py
--rw-r--r--   0        0        0     3666 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/strategies/S_MACD.py
--rw-r--r--   0        0        0     3592 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/strategies/S_base.py
--rw-r--r--   0        0        0     1776 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/strategies/S_bid_ask.py
--rw-r--r--   0        0        0       29 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/strategies/__init__.py
--rw-r--r--   0        0        0     2245 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/strategies/s_temp.py
--rw-r--r--   0        0        0      678 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/tests/benchmark_multiple_assets.py
--rw-r--r--   0        0        0        0 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/tests/core_calculate_trade_price.py
--rw-r--r--   0        0        0      698 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/tests/optimisation_combine_files.py
--rw-r--r--   0        0        0      742 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/tests/supertrend.py
--rw-r--r--   0        0        0      635 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/tests/test_calculate_commission.py
--rw-r--r--   0        0        0     2993 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/tests/test_calculate_entry_exit_price.py
--rw-r--r--   0        0        0     5531 2023-08-05 11:34:00.850412 quantnb-0.3.2/quantnb/tests/test_trade.py
--rw-r--r--   0        0        0     1428 1970-01-01 00:00:00.000000 quantnb-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      276 2023-08-07 11:27:57.229109 quantnb-0.3.3/README.md
+-rw-r--r--   0        0        0     1125 2023-08-07 11:27:57.661105 quantnb-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/__init__.py
+-rw-r--r--   0        0        0     1901 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/PNL.py
+-rw-r--r--   0        0        0      246 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/__init__.py
+-rw-r--r--   0        0        0    12236 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/backtester.old.py
+-rw-r--r--   0        0        0     4345 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/backtester.py
+-rw-r--r--   0        0        0     2236 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/base.py
+-rw-r--r--   0        0        0      341 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/calculate_commission.py
+-rw-r--r--   0        0        0      517 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/calculate_entry_price.py
+-rw-r--r--   0        0        0      516 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/calculate_exit_price.py
+-rw-r--r--   0        0        0     3001 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/data_module.py
+-rw-r--r--   0        0        0      847 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/enums.py
+-rw-r--r--   0        0        0      473 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/helpers.py
+-rw-r--r--   0        0        0     2377 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/place_orders_on_ohlc.py
+-rw-r--r--   0        0        0      909 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/specs_nb.py
+-rw-r--r--   0        0        0       94 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/test.py
+-rw-r--r--   0        0        0      515 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/trade_add_trade_to_active_trades.py
+-rw-r--r--   0        0        0      974 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/trade_close_trade.py
+-rw-r--r--   0        0        0     1183 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/trade_create_new_trade.py
+-rw-r--r--   0        0        0     5060 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/trade_module.py
+-rw-r--r--   0        0        0      696 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/trade_remove_from_active_trades.py
+-rw-r--r--   0        0        0      647 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/trade_should_trade_close.py
+-rw-r--r--   0        0        0      558 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/core/update_trades_pnl.py
+-rw-r--r--   0        0        0     2900 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/H_ticks_to_ranges.py
+-rw-r--r--   0        0        0     1337 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/S_calculate_metrics.py
+-rw-r--r--   0        0        0      357 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/S_print_orders.py
+-rw-r--r--   0        0        0      754 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/S_print_trades.py
+-rw-r--r--   0        0        0      300 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/__init__.py
+-rw-r--r--   0        0        0      793 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/analyze_trade_duration.py
+-rw-r--r--   0        0        0      380 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/calculate_average_freq.py
+-rw-r--r--   0        0        0     1038 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/calculate_pf_stats.py
+-rw-r--r--   0        0        0      390 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/calculate_risk_free.py
+-rw-r--r--   0        0        0      213 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/get_average_trade_duration.py
+-rw-r--r--   0        0        0      672 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/get_realized_pf_value.py
+-rw-r--r--   0        0        0      325 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/plot_lines.py
+-rw-r--r--   0        0        0      731 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/helpers/save_to_csv.py
+-rw-r--r--   0        0        0      109 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/indicators/EMA.py
+-rw-r--r--   0        0        0      351 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/indicators/HMA.py
+-rw-r--r--   0        0        0     1233 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/indicators/I_donchian.py
+-rw-r--r--   0        0        0      109 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/indicators/SMA.py
+-rw-r--r--   0        0        0      198 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/indicators/__init__.py
+-rw-r--r--   0        0        0      221 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/indicators/cross_above.py
+-rw-r--r--   0        0        0      222 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/indicators/cross_below.py
+-rw-r--r--   0        0        0     1732 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/indicators/random_data.py
+-rw-r--r--   0        0        0     1253 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/indicators/supertrend.py
+-rw-r--r--   0        0        0      505 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/__init__.py
+-rw-r--r--   0        0        0     3204 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/calculate_stats.py
+-rw-r--r--   0        0        0      147 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/convert_signal_to_markers.py
+-rw-r--r--   0        0        0     1143 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/create_binance_dataframe.py
+-rw-r--r--   0        0        0     1044 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/fetch_binance_data.py
+-rw-r--r--   0        0        0      466 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/find_files.py
+-rw-r--r--   0        0        0     3828 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/helpers.py
+-rw-r--r--   0        0        0     1131 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/multiprocess.py
+-rw-r--r--   0        0        0     1305 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/optimize.py
+-rw-r--r--   0        0        0      813 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/output_trades.py
+-rw-r--r--   0        0        0     4591 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/plotting.py
+-rw-r--r--   0        0        0     2058 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/qs.py
+-rw-r--r--   0        0        0      241 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/resample.py
+-rw-r--r--   0        0        0      881 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/lib/time_manip.py
+-rw-r--r--   0        0        0     3666 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/strategies/S_MACD.py
+-rw-r--r--   0        0        0     3592 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/strategies/S_base.py
+-rw-r--r--   0        0        0     1776 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/strategies/S_bid_ask.py
+-rw-r--r--   0        0        0       29 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/strategies/__init__.py
+-rw-r--r--   0        0        0     2245 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/strategies/s_temp.py
+-rw-r--r--   0        0        0      678 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/tests/benchmark_multiple_assets.py
+-rw-r--r--   0        0        0        0 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/tests/core_calculate_trade_price.py
+-rw-r--r--   0        0        0      698 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/tests/optimisation_combine_files.py
+-rw-r--r--   0        0        0      742 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/tests/supertrend.py
+-rw-r--r--   0        0        0      635 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/tests/test_calculate_commission.py
+-rw-r--r--   0        0        0     2993 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/tests/test_calculate_entry_exit_price.py
+-rw-r--r--   0        0        0     5531 2023-08-07 11:27:57.661105 quantnb-0.3.3/quantnb/tests/test_trade.py
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 quantnb-0.3.3/PKG-INFO
```

### Comparing `quantnb-0.3.2/pyproject.toml` & `quantnb-0.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "quantnb"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["Alpha <piotr@piotryordanov.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 numba = "^0.57.0"
 numpy = "^1.24.3"
 pandas = "^2.0.1"
 ta-lib = "^0.4.26"
 matplotlib = "^3.7.1"
 pyarrow = "^12.0.0"
 mplfinance = "^0.12.9b7"
@@ -21,14 +21,15 @@
 quantstats = {version = "^0.0.59", optional = true}
 seaborn = {version = "^0.12.2", extras = ["stats"], optional = true}
 ipython = {version = "^8.14.0", optional = true}
 pandas-ta = {version = "^0.3.14b0", optional = true}
 pytest = "^7.4.0"
 pytest-watcher = "^0.3.4"
 pyright = "^1.1.320"
+importlib-resources = "^6.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
```

### Comparing `quantnb-0.3.2/quantnb/core/PNL.py` & `quantnb-0.3.3/quantnb/core/PNL.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/backtester.old.py` & `quantnb-0.3.3/quantnb/core/backtester.old.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/backtester.py` & `quantnb-0.3.3/quantnb/core/backtester.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/base.py` & `quantnb-0.3.3/quantnb/core/base.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/calculate_entry_price.py` & `quantnb-0.3.3/quantnb/core/calculate_entry_price.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/calculate_exit_price.py` & `quantnb-0.3.3/quantnb/core/calculate_exit_price.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/data_module.py` & `quantnb-0.3.3/quantnb/core/data_module.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/enums.py` & `quantnb-0.3.3/quantnb/core/enums.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/place_orders_on_ohlc.py` & `quantnb-0.3.3/quantnb/core/place_orders_on_ohlc.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/specs_nb.py` & `quantnb-0.3.3/quantnb/core/specs_nb.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/trade_add_trade_to_active_trades.py` & `quantnb-0.3.3/quantnb/core/trade_add_trade_to_active_trades.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/trade_close_trade.py` & `quantnb-0.3.3/quantnb/core/trade_close_trade.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/trade_create_new_trade.py` & `quantnb-0.3.3/quantnb/core/trade_create_new_trade.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/trade_module.py` & `quantnb-0.3.3/quantnb/core/trade_module.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/trade_remove_from_active_trades.py` & `quantnb-0.3.3/quantnb/core/trade_remove_from_active_trades.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/trade_should_trade_close.py` & `quantnb-0.3.3/quantnb/core/trade_should_trade_close.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/core/update_trades_pnl.py` & `quantnb-0.3.3/quantnb/core/update_trades_pnl.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/helpers/H_ticks_to_ranges.py` & `quantnb-0.3.3/quantnb/helpers/H_ticks_to_ranges.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/helpers/S_calculate_metrics.py` & `quantnb-0.3.3/quantnb/helpers/S_calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/helpers/S_print_trades.py` & `quantnb-0.3.3/quantnb/helpers/S_print_trades.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/helpers/analyze_trade_duration.py` & `quantnb-0.3.3/quantnb/helpers/analyze_trade_duration.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/helpers/calculate_pf_stats.py` & `quantnb-0.3.3/quantnb/helpers/calculate_pf_stats.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/helpers/get_realized_pf_value.py` & `quantnb-0.3.3/quantnb/helpers/get_realized_pf_value.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/helpers/save_to_csv.py` & `quantnb-0.3.3/quantnb/helpers/save_to_csv.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/indicators/I_donchian.py` & `quantnb-0.3.3/quantnb/indicators/I_donchian.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/indicators/random_data.py` & `quantnb-0.3.3/quantnb/indicators/random_data.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/indicators/supertrend.py` & `quantnb-0.3.3/quantnb/indicators/supertrend.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/lib/calculate_stats.py` & `quantnb-0.3.3/quantnb/lib/calculate_stats.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/lib/create_binance_dataframe.py` & `quantnb-0.3.3/quantnb/lib/create_binance_dataframe.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/lib/fetch_binance_data.py` & `quantnb-0.3.3/quantnb/lib/fetch_binance_data.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/lib/helpers.py` & `quantnb-0.3.3/quantnb/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/lib/multiprocess.py` & `quantnb-0.3.3/quantnb/lib/multiprocess.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/lib/optimize.py` & `quantnb-0.3.3/quantnb/lib/optimize.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/lib/output_trades.py` & `quantnb-0.3.3/quantnb/lib/output_trades.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/lib/plotting.py` & `quantnb-0.3.3/quantnb/lib/plotting.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/lib/qs.py` & `quantnb-0.3.3/quantnb/lib/qs.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/lib/time_manip.py` & `quantnb-0.3.3/quantnb/lib/time_manip.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/strategies/S_MACD.py` & `quantnb-0.3.3/quantnb/strategies/S_MACD.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/strategies/S_base.py` & `quantnb-0.3.3/quantnb/strategies/S_base.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/strategies/S_bid_ask.py` & `quantnb-0.3.3/quantnb/strategies/S_bid_ask.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/strategies/s_temp.py` & `quantnb-0.3.3/quantnb/strategies/s_temp.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/tests/benchmark_multiple_assets.py` & `quantnb-0.3.3/quantnb/tests/benchmark_multiple_assets.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/tests/optimisation_combine_files.py` & `quantnb-0.3.3/quantnb/tests/optimisation_combine_files.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/tests/supertrend.py` & `quantnb-0.3.3/quantnb/tests/supertrend.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/tests/test_calculate_commission.py` & `quantnb-0.3.3/quantnb/tests/test_calculate_commission.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/tests/test_calculate_entry_exit_price.py` & `quantnb-0.3.3/quantnb/tests/test_calculate_entry_exit_price.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/quantnb/tests/test_trade.py` & `quantnb-0.3.3/quantnb/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.3.2/PKG-INFO` & `quantnb-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: quantnb
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Author: Alpha
 Author-email: piotr@piotryordanov.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev-tools
+Requires-Dist: importlib-resources (>=6.0.1,<7.0.0)
 Requires-Dist: ipython (>=8.14.0,<9.0.0) ; extra == "dev-tools"
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mplfinance (>=0.12.9b7,<0.13.0)
 Requires-Dist: numba (>=0.57.0,<0.58.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pandas-ta (>=0.3.14b0,<0.4.0) ; extra == "dev-tools"
```

