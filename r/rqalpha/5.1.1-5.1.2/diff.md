# Comparing `tmp/rqalpha-5.1.1.tar.gz` & `tmp/rqalpha-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/.tmp-rp8_a7qx/rqalpha-5.1.1.tar", last modified: Fri Jul  7 06:30:29 2023, max compression
+gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/.tmp-bzfp5fon/rqalpha-5.1.2.tar", last modified: Mon Aug  7 06:27:40 2023, max compression
```

## Comparing `rqalpha-5.1.1.tar` & `rqalpha-5.1.2.tar`

### file list

```diff
@@ -1,243 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    61336 2023-07-07 06:30:19.000000 rqalpha-5.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-07 06:30:19.000000 rqalpha-5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-07 06:30:19.000000 rqalpha-5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 06:30:29.000000 rqalpha-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-07-07 06:30:19.000000 rqalpha-5.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21928 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/apis/api_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/apis/api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    59090 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/apis/api_rqdatac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/apis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/global_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/strategy_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/strategy_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/strategy_universe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/bar_dict_price_board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/storage_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/storages.py
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/data_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/trading_dates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/IF1706_20161108.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/IF_macd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/examples/data_source/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/data_source/get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/data_source/import_get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/data_source/read_csv_as_df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/examples/extend_api/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/extend_api/test_extend_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/golden_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/macd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/pair_trading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/rsi.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/run_code_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/run_file_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/run_func_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/subscribe_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/test_pt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/turtle.py
--rw-r--r--   0 runner    (1001) docker     (123)    21124 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
--rw-r--r--   0 runner    (1001) docker     (123)    34434 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    20020 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25635 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_progress/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29229 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/portfolio/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/portfolio/position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/resource/
--rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/resource/ricequant-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/user_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18080 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/arg_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/class_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/click_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/datetime_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/dict_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/package_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/persisit_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/risk_free_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/rq_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/strategy_loader_help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/testing/mocking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/utils/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    51160 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:30:28.000000 rqalpha-5.1.1/rqalpha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-07 06:30:29.000000 rqalpha-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-07 06:30:19.000000 rqalpha-5.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/mod/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_account_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_margin_stocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_position_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/test_physical_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/test_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_management_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/test_api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/test_api_future.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/test_api_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_f_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_f_macd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_f_macd_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_f_mean_reverting.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_dual_thrust.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_tick_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_turtle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_turtle_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_sf_buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/unittest/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/unittest/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_data/test_instrument_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_data/test_trading_dates_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/unittest/test_mod/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/unittest/test_mod/test_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_mod/test_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    79879 2023-07-07 06:30:19.000000 rqalpha-5.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    61478 2023-08-07 06:27:31.000000 rqalpha-5.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-07 06:27:31.000000 rqalpha-5.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-07 06:27:31.000000 rqalpha-5.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-07 06:27:40.000000 rqalpha-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-08-07 06:27:31.000000 rqalpha-5.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21928 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/apis/api_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/apis/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59090 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/apis/api_rqdatac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/apis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/cmds/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/cmds/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/cmds/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/cmds/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/cmds/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/core/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/core/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/core/global_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/core/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/core/strategy_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/core/strategy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/core/strategy_universe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/data/bar_dict_price_board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/data/base_data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/data/base_data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/data/base_data_source/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/data/base_data_source/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/data/base_data_source/storage_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/data/base_data_source/storages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/data/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/data/data_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/data/trading_dates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/IF1706_20161108.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/IF_macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/examples/data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/data_source/get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/data_source/import_get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/data_source/read_csv_as_df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/examples/extend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/extend_api/test_extend_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/golden_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/pair_trading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/rsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/run_code_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/run_file_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/run_func_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/subscribe_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/test_pt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/examples/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34434 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20002 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25670 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29229 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/mod_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/model/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24965 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/model/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/model/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/model/tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/model/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/portfolio/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/portfolio/position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/resource/ricequant-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/user_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18080 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/arg_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/class_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/click_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/datetime_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/dict_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/package_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/persisit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/risk_free_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/rq_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/strategy_loader_help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/testing/mocking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/utils/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/utils/translations/zh_Hans_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    51160 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/translations/zh_Hans_CN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-07 06:27:31.000000 rqalpha-5.1.2/rqalpha/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 06:27:39.000000 rqalpha-5.1.2/rqalpha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 06:27:40.000000 rqalpha-5.1.2/rqalpha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-07 06:27:40.000000 rqalpha-5.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-08-07 06:27:31.000000 rqalpha-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/tests/api_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/tests/api_tests/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_accounts/test_account_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_accounts/test_margin_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_accounts/test_position_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_scheduler/test_physical_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_scheduler/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/test_management_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/test_signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/test_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/test_api_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/test_api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/api_tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/test_f_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/test_f_macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/test_f_macd_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/test_f_mean_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/test_s_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/test_s_dual_thrust.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/test_s_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/test_s_tick_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/test_s_turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/test_s_turtle_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/test_sf_buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/tests/unittest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/unittest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/tests/unittest/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/unittest/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/unittest/test_data/test_instrument_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/unittest/test_data/test_trading_dates_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/tests/unittest/test_mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/unittest/test_mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 06:27:40.000000 rqalpha-5.1.2/tests/unittest/test_mod/test_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/unittest/test_mod/test_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-07 06:27:31.000000 rqalpha-5.1.2/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79879 2023-08-07 06:27:31.000000 rqalpha-5.1.2/versioneer.py
```

### Comparing `rqalpha-5.1.1/CHANGELOG.rst` & `rqalpha-5.1.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 ==================
 CHANGELOG
 ==================
 
+5.1.2
+==================
+- 修复analyser中计算个股权重的异常
+- 修复分钟回测中挂单在非交易时间内被拒单的异常
+
 5.1.1
 ==================
 - 调整API参数;更新文档
 
 5.1.0
 ==================
 - 新增个股权重检测, summary报告中新增了表格
```

### Comparing `rqalpha-5.1.1/LICENSE` & `rqalpha-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/PKG-INFO` & `rqalpha-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 5.1.1
+Version: 5.1.2
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `rqalpha-5.1.1/README.rst` & `rqalpha-5.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/__init__.py` & `rqalpha-5.1.2/rqalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/__main__.py` & `rqalpha-5.1.2/rqalpha/__main__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/api.py` & `rqalpha-5.1.2/rqalpha/api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/apis/__init__.py` & `rqalpha-5.1.2/rqalpha/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/apis/api_abstract.py` & `rqalpha-5.1.2/rqalpha/apis/api_abstract.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/apis/api_base.py` & `rqalpha-5.1.2/rqalpha/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/apis/api_rqdatac.py` & `rqalpha-5.1.2/rqalpha/apis/api_rqdatac.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/apis/names.py` & `rqalpha-5.1.2/rqalpha/apis/names.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/cmds/__init__.py` & `rqalpha-5.1.2/rqalpha/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/cmds/bundle.py` & `rqalpha-5.1.2/rqalpha/cmds/bundle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/cmds/entry.py` & `rqalpha-5.1.2/rqalpha/cmds/entry.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/cmds/misc.py` & `rqalpha-5.1.2/rqalpha/cmds/misc.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/cmds/mod.py` & `rqalpha-5.1.2/rqalpha/cmds/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/cmds/run.py` & `rqalpha-5.1.2/rqalpha/cmds/run.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/config.yml` & `rqalpha-5.1.2/rqalpha/config.yml`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/const.py` & `rqalpha-5.1.2/rqalpha/const.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/core/__init__.py` & `rqalpha-5.1.2/rqalpha/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/core/events.py` & `rqalpha-5.1.2/rqalpha/core/events.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/core/execution_context.py` & `rqalpha-5.1.2/rqalpha/core/execution_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/core/executor.py` & `rqalpha-5.1.2/rqalpha/core/executor.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/core/global_var.py` & `rqalpha-5.1.2/rqalpha/core/global_var.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/core/strategy.py` & `rqalpha-5.1.2/rqalpha/core/strategy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/core/strategy_context.py` & `rqalpha-5.1.2/rqalpha/core/strategy_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/core/strategy_loader.py` & `rqalpha-5.1.2/rqalpha/core/strategy_loader.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/core/strategy_universe.py` & `rqalpha-5.1.2/rqalpha/core/strategy_universe.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/data/__init__.py` & `rqalpha-5.1.2/rqalpha/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/data/bar_dict_price_board.py` & `rqalpha-5.1.2/rqalpha/data/bar_dict_price_board.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/data/base_data_source/__init__.py` & `rqalpha-5.1.2/rqalpha/data/base_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/data/base_data_source/adjust.py` & `rqalpha-5.1.2/rqalpha/data/base_data_source/adjust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/data/base_data_source/data_source.py` & `rqalpha-5.1.2/rqalpha/data/base_data_source/data_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/data/base_data_source/storage_interface.py` & `rqalpha-5.1.2/rqalpha/data/base_data_source/storage_interface.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/data/base_data_source/storages.py` & `rqalpha-5.1.2/rqalpha/data/base_data_source/storages.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/data/bundle.py` & `rqalpha-5.1.2/rqalpha/data/bundle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/data/data_proxy.py` & `rqalpha-5.1.2/rqalpha/data/data_proxy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/data/trading_dates_mixin.py` & `rqalpha-5.1.2/rqalpha/data/trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/environment.py` & `rqalpha-5.1.2/rqalpha/environment.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/IF1706_20161108.csv` & `rqalpha-5.1.2/rqalpha/examples/IF1706_20161108.csv`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/IF_macd.py` & `rqalpha-5.1.2/rqalpha/examples/IF_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/buy_and_hold.py` & `rqalpha-5.1.2/rqalpha/examples/buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/data_source/get_csv_module.py` & `rqalpha-5.1.2/rqalpha/examples/data_source/get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/data_source/import_get_csv_module.py` & `rqalpha-5.1.2/rqalpha/examples/data_source/import_get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/data_source/read_csv_as_df.py` & `rqalpha-5.1.2/rqalpha/examples/data_source/read_csv_as_df.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py` & `rqalpha-5.1.2/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/extend_api/test_extend_api.py` & `rqalpha-5.1.2/rqalpha/examples/extend_api/test_extend_api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/golden_cross.py` & `rqalpha-5.1.2/rqalpha/examples/golden_cross.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/macd.py` & `rqalpha-5.1.2/rqalpha/examples/macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/pair_trading.py` & `rqalpha-5.1.2/rqalpha/examples/pair_trading.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/rsi.py` & `rqalpha-5.1.2/rqalpha/examples/rsi.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/run_code_demo.py` & `rqalpha-5.1.2/rqalpha/examples/run_code_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/run_func_demo.py` & `rqalpha-5.1.2/rqalpha/examples/run_func_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/subscribe_event.py` & `rqalpha-5.1.2/rqalpha/examples/subscribe_event.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/test_pt.py` & `rqalpha-5.1.2/rqalpha/examples/test_pt.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/examples/turtle.py` & `rqalpha-5.1.2/rqalpha/examples/turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/interface.py` & `rqalpha-5.1.2/rqalpha/interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,14 +128,59 @@
     def quantity(self):
         # type: () -> Union[int, float]
         """
         返回当前持仓量
         """
         raise NotImplementedError
 
+    @property
+    @abc.abstractmethod
+    def avg_price(self):
+        # type: () -> Union[int, float]
+        """
+        开仓均价
+        """
+        raise NotImplementedError
+
+    @property
+    @abc.abstractmethod
+    def pnl(self):
+        # type: () -> float
+        """
+        该持仓的累计盈亏
+        """
+        raise NotImplementedError
+
+    @property
+    @abc.abstractmethod
+    def equity(self):
+        # type: () -> float
+        """
+        当前持仓市值
+        """
+        raise NotImplementedError
+
+    @property
+    @abc.abstractmethod
+    def prev_close(self):
+        # type: () -> float
+        """
+        昨日收盘价
+        """
+        raise NotImplementedError
+
+    @property
+    @abc.abstractmethod
+    def last_price(self):
+        # type: () -> float
+        """
+        当前最新价
+        """
+        raise NotImplementedError
+
 
 class AbstractStrategyLoader(with_metaclass(abc.ABCMeta)):
     """
     策略加载器，其主要作用是加载策略，并将策略运行所需要的域环境传递给策略执行代码。
 
     在扩展模块中，可以通过调用 ``env.set_strategy_loader`` 来替换默认的策略加载器。
     """
```

### Comparing `rqalpha-5.1.1/rqalpha/main.py` & `rqalpha-5.1.2/rqalpha/main.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/__init__.py` & `rqalpha-5.1.2/rqalpha/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,14 @@
         # type: () -> float
         """"""
         return self._quantity * (self.last_price - self._avg_price) * self.contract_multiplier * self._direction_factor
 
     @property
     def margin(self) -> float:
         """
-        保证金
         保证金 = 持仓量 * 最新价 * 合约乘数 * 保证金率
         """
         return self.margin_rate * self.market_value
 
     @property
     def market_value(self):
         # type: () -> float
```

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py`

 * *Files 1% similar despite different names*

```diff
@@ -496,15 +496,15 @@
         for table_name in ["stock_positions", "future_positions"]:
             if table_name not in result_dict:
                 continue
             table = result_dict[table_name]
             for field in ["market_value", "LONG_market_value", "SHORT_market_value"]:
                 if field not in table.columns:
                     continue
-                df_list.append(table.rename(columns={field: "market_value"})[need_cols])
+                df_list.append(table[["order_book_id", field]].rename(columns={field: "market_value"})[need_cols].dropna())
         if len(df_list) > 0:
             positions_weight_df = pd.concat(df_list).dropna()
             positions_weight_df["total_value"] = positions_weight_df.groupby(by="date")["market_value"].sum()
             positions_weight_df["weight"] = positions_weight_df["market_value"] / positions_weight_df["total_value"]
             positions_weight_df = positions_weight_df.groupby(by="date")["weight"].describe()
         else:
             positions_weight_df = pd.DataFrame(columns=["count", "mean", "std", "min", "25%", "50%", "75%", "max"])
```

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_progress/mod.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_progress/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/mod.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         if ExecutionContext.phase() == EXECUTION_PHASE.OPEN_AUCTION:
             self._open_auction_orders.append((account, order))
         else:
             self._open_orders.append((account, order))
         order.active()
         self._env.event_bus.publish_event(Event(EVENT.ORDER_CREATION_PASS, account=account, order=order))
         if self._match_immediately:
-            self._match()
+            self._match(self._env.calendar_dt)
 
     def cancel_order(self, order):
         account = self._env.get_account(order.order_book_id)
 
         self._env.event_bus.publish_event(Event(EVENT.ORDER_PENDING_CANCEL, account=account, order=order))
 
         order.mark_cancelled(_(u"{order_id} order has been cancelled by user.").format(order_id=order.order_id))
@@ -154,24 +154,27 @@
             if order.status == ORDER_STATUS.REJECTED or order.status == ORDER_STATUS.CANCELLED:
                 self._env.event_bus.publish_event(Event(EVENT.ORDER_UNSOLICITED_UPDATE, account=account, order=order))
         self._open_exercise_orders.clear()
 
     def on_bar(self, event):
         for matcher in self._matchers.values():
             matcher.update(event)
-        self._match()
+        self._match(event.calendar_dt)
 
     def on_tick(self, event):
         tick = event.tick
         self._get_matcher(tick.order_book_id).update(event)
-        self._match(tick.order_book_id)
+        self._match(event.calendar_dt, tick.order_book_id)
 
-    def _match(self, order_book_id=None):
-        order_filter = lambda a_and_o: not (a_and_o[1].is_final() or (order_book_id and a_and_o[1].order_book_id != order_book_id))
-        for account, order in filter(order_filter, self._open_orders):
+    def _match(self, dt, order_book_id=None):
+        # 撮合未完成的订单，若指定标的时只撮合指定的标的的订单
+        order_filter = lambda a_and_o: (not a_and_o[1].is_final()) and (True if order_book_id is None else a_and_o[1].order_book_id == order_book_id)
+        # + 需要在交易时段内
+        open_order_filter = lambda a_and_o: order_filter(a_and_o) and self._env.data_proxy.instrument(a_and_o[1].order_book_id).during_continuous_auction(dt.time())
+        for account, order in filter(open_order_filter, self._open_orders):
             self._get_matcher(order.order_book_id).match(account, order, open_auction=False)
         for account, order in filter(order_filter, self._open_auction_orders):
             self._get_matcher(order.order_book_id).match(account, order, open_auction=True)
         final_orders = [(a, o) for a, o in chain(self._open_orders, self._open_auction_orders) if o.is_final()]
         self._open_orders = [(a, o) for a, o in chain(self._open_orders, self._open_auction_orders) if not o.is_final()]
         self._open_auction_orders.clear()
```

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py` & `rqalpha-5.1.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/mod/utils.py` & `rqalpha-5.1.2/rqalpha/mod/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/model/__init__.py` & `rqalpha-5.1.2/rqalpha/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/model/bar.py` & `rqalpha-5.1.2/rqalpha/model/bar.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/model/instrument.py` & `rqalpha-5.1.2/rqalpha/model/instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,14 +371,22 @@
             if start > end:
                 trading_period.append(TimeRange(start, datetime.time(23, 59)))
                 trading_period.append(TimeRange(datetime.time(0, 0), end))
             else:
                 trading_period.append(TimeRange(start, end))
         return trading_period
 
+    def during_continuous_auction(self, time):
+        # type: (datetime.time) -> bool
+        """ 是否处于连续竞价时间段内 """
+        for time_range in self.trading_hours:
+            if time_range.start <= time <= time_range.end:
+                return True
+        return False
+
     @property
     def trading_code(self):
         # type: () -> str
         try:
             return self.__dict__["trading_code"]
         except (KeyError, ValueError):
             raise AttributeError(
```

### Comparing `rqalpha-5.1.1/rqalpha/model/order.py` & `rqalpha-5.1.2/rqalpha/model/order.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/model/tick.py` & `rqalpha-5.1.2/rqalpha/model/tick.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/model/trade.py` & `rqalpha-5.1.2/rqalpha/model/trade.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/portfolio/__init__.py` & `rqalpha-5.1.2/rqalpha/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/portfolio/account.py` & `rqalpha-5.1.2/rqalpha/portfolio/account.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/portfolio/position.py` & `rqalpha-5.1.2/rqalpha/portfolio/position.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/resource/ricequant-logo.png` & `rqalpha-5.1.2/rqalpha/resource/ricequant-logo.png`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/user_module.py` & `rqalpha-5.1.2/rqalpha/user_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/__init__.py` & `rqalpha-5.1.2/rqalpha/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/arg_checker.py` & `rqalpha-5.1.2/rqalpha/utils/arg_checker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/class_helper.py` & `rqalpha-5.1.2/rqalpha/utils/class_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/click_helper.py` & `rqalpha-5.1.2/rqalpha/utils/click_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/concurrent.py` & `rqalpha-5.1.2/rqalpha/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/config.py` & `rqalpha-5.1.2/rqalpha/utils/config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/datetime_func.py` & `rqalpha-5.1.2/rqalpha/utils/datetime_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/dict_func.py` & `rqalpha-5.1.2/rqalpha/utils/dict_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/exception.py` & `rqalpha-5.1.2/rqalpha/utils/exception.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/functools.py` & `rqalpha-5.1.2/rqalpha/utils/functools.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/i18n.py` & `rqalpha-5.1.2/rqalpha/utils/i18n.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/log_capture.py` & `rqalpha-5.1.2/rqalpha/utils/log_capture.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/logger.py` & `rqalpha-5.1.2/rqalpha/utils/logger.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/package_helper.py` & `rqalpha-5.1.2/rqalpha/utils/package_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/persisit_helper.py` & `rqalpha-5.1.2/rqalpha/utils/persisit_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/repr.py` & `rqalpha-5.1.2/rqalpha/utils/repr.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/risk_free_helper.py` & `rqalpha-5.1.2/rqalpha/utils/risk_free_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/rq_json.py` & `rqalpha-5.1.2/rqalpha/utils/rq_json.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/strategy_loader_help.py` & `rqalpha-5.1.2/rqalpha/utils/strategy_loader_help.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/testing/__init__.py` & `rqalpha-5.1.2/rqalpha/utils/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/testing/fixtures.py` & `rqalpha-5.1.2/rqalpha/utils/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/testing/mocking.py` & `rqalpha-5.1.2/rqalpha/utils/testing/mocking.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/translations/__init__.py` & `rqalpha-5.1.2/rqalpha/utils/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py` & `rqalpha-5.1.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo` & `rqalpha-5.1.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po` & `rqalpha-5.1.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/__init__.py` & `rqalpha-5.1.2/rqalpha/utils/translations/zh_Hans_CN/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha/utils/typing.py` & `rqalpha-5.1.2/rqalpha/utils/typing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/rqalpha.egg-info/PKG-INFO` & `rqalpha-5.1.2/rqalpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 5.1.1
+Version: 5.1.2
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `rqalpha-5.1.1/rqalpha.egg-info/SOURCES.txt` & `rqalpha-5.1.2/rqalpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
 tests/api_tests/mod/sys_accounts/test_margin_stocks.py
 tests/api_tests/mod/sys_accounts/test_position_models.py
 tests/api_tests/mod/sys_scheduler/__init__.py
 tests/api_tests/mod/sys_scheduler/test_physical_time.py
 tests/api_tests/mod/sys_scheduler/test_scheduler.py
 tests/api_tests/mod/sys_simulation/__init__.py
 tests/api_tests/mod/sys_simulation/test_management_fee.py
+tests/api_tests/mod/sys_simulation/test_match.py
 tests/api_tests/mod/sys_simulation/test_signal_broker.py
 tests/api_tests/mod/sys_simulation/test_simulation_broker.py
 tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
 tests/api_tests/mod/sys_transaction_cost/__init__.py
 tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
 tests/unittest/__init__.py
 tests/unittest/test_data/__init__.py
```

### Comparing `rqalpha-5.1.1/setup.py` & `rqalpha-5.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/__init__.py` & `rqalpha-5.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/__init__.py` & `rqalpha-5.1.2/tests/api_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/__init__.py` & `rqalpha-5.1.2/tests/api_tests/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/__init__.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_account_model.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_accounts/test_account_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_margin_stocks.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_accounts/test_margin_stocks.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_position_models.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_accounts/test_position_models.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/test_physical_time.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_scheduler/test_physical_time.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/test_scheduler.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/__init__.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_management_fee.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/test_management_fee.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_signal_broker.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/test_signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_simulation_broker.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/test_simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py` & `rqalpha-5.1.2/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/test_api_base.py` & `rqalpha-5.1.2/tests/api_tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/test_api_future.py` & `rqalpha-5.1.2/tests/api_tests/test_api_future.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/test_api_stock.py` & `rqalpha-5.1.2/tests/api_tests/test_api_stock.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/api_tests/test_config.py` & `rqalpha-5.1.2/tests/api_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/test_f_buy_and_hold.py` & `rqalpha-5.1.2/tests/test_f_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/test_f_macd.py` & `rqalpha-5.1.2/tests/test_f_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/test_f_macd_signal.py` & `rqalpha-5.1.2/tests/test_f_macd_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/test_f_mean_reverting.py` & `rqalpha-5.1.2/tests/test_f_mean_reverting.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/test_s_buy_and_hold.py` & `rqalpha-5.1.2/tests/test_s_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/test_s_dual_thrust.py` & `rqalpha-5.1.2/tests/test_s_dual_thrust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/test_s_scheduler.py` & `rqalpha-5.1.2/tests/test_s_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/test_s_tick_size.py` & `rqalpha-5.1.2/tests/test_s_tick_size.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/test_s_turtle.py` & `rqalpha-5.1.2/tests/test_s_turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/test_s_turtle_signal.py` & `rqalpha-5.1.2/tests/test_s_turtle_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/test_sf_buy_and_hold.py` & `rqalpha-5.1.2/tests/test_sf_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/unittest/__init__.py` & `rqalpha-5.1.2/tests/unittest/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/unittest/test_data/test_instrument_mixin.py` & `rqalpha-5.1.2/tests/unittest/test_data/test_instrument_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/unittest/test_data/test_trading_dates_mixin.py` & `rqalpha-5.1.2/tests/unittest/test_data/test_trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/unittest/test_mod/__init__.py` & `rqalpha-5.1.2/tests/unittest/test_mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/unittest/test_mod/test_sys_simulation/__init__.py` & `rqalpha-5.1.2/tests/unittest/test_mod/test_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py` & `rqalpha-5.1.2/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/tests/utils.py` & `rqalpha-5.1.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.1/versioneer.py` & `rqalpha-5.1.2/versioneer.py`

 * *Files identical despite different names*

