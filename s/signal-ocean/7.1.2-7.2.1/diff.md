# Comparing `tmp/signal-ocean-7.1.2.tar.gz` & `tmp/signal-ocean-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal-ocean-7.1.2.tar", last modified: Thu Jul 27 11:11:39 2023, max compression
+gzip compressed data, was "signal-ocean-7.2.1.tar", last modified: Mon Aug  7 11:39:56 2023, max compression
```

## Comparing `signal-ocean-7.1.2.tar` & `signal-ocean-7.2.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2175 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1184 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 11:11:39.767193 signal-ocean-7.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1524 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.751193 signal-ocean-7.1.2/signal_ocean/
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/_internals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.751193 signal-ocean-7.1.2/signal_ocean/companies/
--rw-r--r--   0 root         (0) root         (0)      236 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/companies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/companies/companies_api.py
--rw-r--r--   0 root         (0) root         (0)     3020 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/companies/models.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.751193 signal-ocean-7.1.2/signal_ocean/distances/
--rw-r--r--   0 root         (0) root         (0)     1210 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2523 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/_distances_json.py
--rw-r--r--   0 root         (0) root         (0)    11714 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/distances_api.py
--rw-r--r--   0 root         (0) root         (0)      287 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/loading_condition.py
--rw-r--r--   0 root         (0) root         (0)     4589 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/models.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/port.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/port_filter.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/distances/vessel_class_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.755193 signal-ocean-7.1.2/signal_ocean/freight_pricing/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/_freight_pricing_json.py
--rw-r--r--   0 root         (0) root         (0)     4766 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/freight_pricing_api.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/models.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/port.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/port_filter.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_class_filter.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_subclass.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_type.py
--rw-r--r--   0 root         (0) root         (0)      877 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_type_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.755193 signal-ocean-7.1.2/signal_ocean/freight_rates/
--rw-r--r--   0 root         (0) root         (0)      565 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2145 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/_freight_rates_json.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/enums.py
--rw-r--r--   0 root         (0) root         (0)     3750 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/freight_rates_api.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/models.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/port_filter.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/freight_rates/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.755193 signal-ocean-7.1.2/signal_ocean/geos/
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/geos/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4338 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/geos/geos_api.py
--rw-r--r--   0 root         (0) root         (0)     6299 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/geos/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.755193 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/
--rw-r--r--   0 root         (0) root         (0)     2261 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py
--rw-r--r--   0 root         (0) root         (0)      331 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/area.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/column.py
--rw-r--r--   0 root         (0) root         (0)      675 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/commercial_status.py
--rw-r--r--   0 root         (0) root         (0)      235 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/fixture_type.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/historical_tonnage_list.py
--rw-r--r--   0 root         (0) root         (0)     4968 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/index_level.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/location_taxonomy.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/market_deployment.py
--rw-r--r--   0 root         (0) root         (0)     1292 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/operational_status.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/push_type.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/tonnage_list.py
--rw-r--r--   0 root         (0) root         (0)     5517 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel.py
--rw-r--r--   0 root         (0) root         (0)     6831 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel_filter.py
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel_subclass.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.755193 signal-ocean-7.1.2/signal_ocean/market_rates/
--rw-r--r--   0 root         (0) root         (0)      536 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/_market_rates_json.py
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/enums.py
--rw-r--r--   0 root         (0) root         (0)     4006 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/market_rates_api.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/models.py
--rw-r--r--   0 root         (0) root         (0)      773 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/utils.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/market_rates/vessel_classes.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/plots.py
--rw-r--r--   0 root         (0) root         (0)      578 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/port_congestion/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_congestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4274 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_congestion/models.py
--rw-r--r--   0 root         (0) root         (0)    19251 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_congestion/port_congestion.py
--rw-r--r--   0 root         (0) root         (0)     4670 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_congestion/port_congestion_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/port_expenses/
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1433 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/_port_expenses_json.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/enums.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/models.py
--rw-r--r--   0 root         (0) root         (0)     8527 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/port_expenses_api.py
--rw-r--r--   0 root         (0) root         (0)      779 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_expenses/port_filter.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/port_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/scraped_cargoes/
--rw-r--r--   0 root         (0) root         (0)      277 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_cargoes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26586 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_cargoes/models.py
--rw-r--r--   0 root         (0) root         (0)     5363 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_cargoes/scraped_cargoes_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/scraped_data/
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4560 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_data/scraped_data_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/scraped_fixtures/
--rw-r--r--   0 root         (0) root         (0)      291 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32666 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_fixtures/models.py
--rw-r--r--   0 root         (0) root         (0)     6009 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_fixtures/scraped_fixtures_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/scraped_lineups/
--rw-r--r--   0 root         (0) root         (0)      281 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_lineups/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21114 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_lineups/models.py
--rw-r--r--   0 root         (0) root         (0)     5968 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_lineups/scraped_lineups_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/scraped_positions/
--rw-r--r--   0 root         (0) root         (0)      301 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_positions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16973 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_positions/models.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/scraped_positions/scraped_positions_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/tonnage_list/
--rw-r--r--   0 root         (0) root         (0)      879 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/tonnage_list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/tonnage_list/_json.py
--rw-r--r--   0 root         (0) root         (0)     6084 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/tonnage_list/api.py
--rw-r--r--   0 root         (0) root         (0)     7229 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/tonnage_list/data_frame.py
--rw-r--r--   0 root         (0) root         (0)    26447 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/tonnage_list/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/util/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6505 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/util/parsing_helpers.py
--rw-r--r--   0 root         (0) root         (0)     6529 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/util/request_helpers.py
--rw-r--r--   0 root         (0) root         (0)      647 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_class_api.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_class_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.759193 signal-ocean-7.1.2/signal_ocean/vessel_emissions/
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_emissions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15668 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_emissions/models.py
--rw-r--r--   0 root         (0) root         (0)    14610 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_emissions/vessel_emissions_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/signal_ocean/vessel_valuations/
--rw-r--r--   0 root         (0) root         (0)      298 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_valuations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_valuations/_valuation_json.py
--rw-r--r--   0 root         (0) root         (0)      608 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_valuations/models.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessel_valuations/vessel_valuations_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/signal_ocean/vessels/
--rw-r--r--   0 root         (0) root         (0)      378 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessels/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17416 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessels/models.py
--rw-r--r--   0 root         (0) root         (0)     3539 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/vessels/vessels_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/signal_ocean/voyages/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46114 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages/models.py
--rw-r--r--   0 root         (0) root         (0)    44712 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages/voyages_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.763193 signal-ocean-7.1.2/signal_ocean/voyages_market_data/
--rw-r--r--   0 root         (0) root         (0)      539 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages_market_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15350 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages_market_data/models.py
--rw-r--r--   0 root         (0) root         (0)    15865 2023-07-27 11:10:21.000000 signal-ocean-7.1.2/signal_ocean/voyages_market_data/voyages_market_data_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 11:11:39.751193 signal-ocean-7.1.2/signal_ocean.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2175 2023-07-27 11:11:39.000000 signal-ocean-7.1.2/signal_ocean.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5081 2023-07-27 11:11:39.000000 signal-ocean-7.1.2/signal_ocean.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 11:11:39.000000 signal-ocean-7.1.2/signal_ocean.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2023-07-27 11:11:39.000000 signal-ocean-7.1.2/signal_ocean.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 11:11:39.000000 signal-ocean-7.1.2/signal_ocean.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.960465 signal-ocean-7.2.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-08-07 11:39:56.960465 signal-ocean-7.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       30 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-07 11:39:56.964465 signal-ocean-7.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.948465 signal-ocean-7.2.1/signal_ocean/
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/_internals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.948465 signal-ocean-7.2.1/signal_ocean/companies/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/companies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/companies/companies_api.py
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/companies/models.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.948465 signal-ocean-7.2.1/signal_ocean/distances/
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/distances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/distances/_distances_json.py
+-rw-r--r--   0 root         (0) root         (0)    11714 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/distances/distances_api.py
+-rw-r--r--   0 root         (0) root         (0)      287 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/distances/loading_condition.py
+-rw-r--r--   0 root         (0) root         (0)     4589 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/distances/models.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/distances/port.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/distances/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/distances/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/distances/vessel_class_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.948465 signal-ocean-7.2.1/signal_ocean/freight_pricing/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_pricing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_pricing/_freight_pricing_json.py
+-rw-r--r--   0 root         (0) root         (0)     4766 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_pricing/freight_pricing_api.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_pricing/models.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_pricing/port.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_pricing/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_pricing/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_pricing/vessel_class_filter.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_pricing/vessel_subclass.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_pricing/vessel_type.py
+-rw-r--r--   0 root         (0) root         (0)      877 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_pricing/vessel_type_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.952465 signal-ocean-7.2.1/signal_ocean/freight_rates/
+-rw-r--r--   0 root         (0) root         (0)      565 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_rates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_rates/_freight_rates_json.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_rates/enums.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_rates/freight_rates_api.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_rates/models.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_rates/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/freight_rates/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.952465 signal-ocean-7.2.1/signal_ocean/geos/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/geos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4338 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/geos/geos_api.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/geos/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.952465 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py
+-rw-r--r--   0 root         (0) root         (0)      331 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/area.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/column.py
+-rw-r--r--   0 root         (0) root         (0)      675 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/commercial_status.py
+-rw-r--r--   0 root         (0) root         (0)      235 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/fixture_type.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/historical_tonnage_list.py
+-rw-r--r--   0 root         (0) root         (0)     4968 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/index_level.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/location_taxonomy.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/market_deployment.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/operational_status.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/push_type.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/tonnage_list.py
+-rw-r--r--   0 root         (0) root         (0)     5517 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/vessel.py
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/vessel_filter.py
+-rw-r--r--   0 root         (0) root         (0)      632 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/vessel_subclass.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.952465 signal-ocean-7.2.1/signal_ocean/market_rates/
+-rw-r--r--   0 root         (0) root         (0)      536 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/market_rates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/market_rates/_market_rates_json.py
+-rw-r--r--   0 root         (0) root         (0)      178 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/market_rates/enums.py
+-rw-r--r--   0 root         (0) root         (0)     4006 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/market_rates/market_rates_api.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/market_rates/models.py
+-rw-r--r--   0 root         (0) root         (0)      773 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/market_rates/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/market_rates/vessel_classes.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/plots.py
+-rw-r--r--   0 root         (0) root         (0)      578 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.952465 signal-ocean-7.2.1/signal_ocean/port_congestion/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_congestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_congestion/models.py
+-rw-r--r--   0 root         (0) root         (0)    19252 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_congestion/port_congestion.py
+-rw-r--r--   0 root         (0) root         (0)     4670 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_congestion/port_congestion_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/port_expenses/
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_expenses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_expenses/_port_expenses_json.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_expenses/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_expenses/models.py
+-rw-r--r--   0 root         (0) root         (0)     8527 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_expenses/port_expenses_api.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_expenses/port_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/port_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/scraped_cargoes/
+-rw-r--r--   0 root         (0) root         (0)      277 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_cargoes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26586 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_cargoes/models.py
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_cargoes/scraped_cargoes_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/scraped_data/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_data/scraped_data_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/scraped_fixtures/
+-rw-r--r--   0 root         (0) root         (0)      291 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32666 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_fixtures/models.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_fixtures/scraped_fixtures_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/scraped_lineups/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_lineups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21114 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_lineups/models.py
+-rw-r--r--   0 root         (0) root         (0)     5968 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_lineups/scraped_lineups_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/scraped_positions/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_positions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16973 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_positions/models.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/scraped_positions/scraped_positions_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/tonnage_list/
+-rw-r--r--   0 root         (0) root         (0)      879 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/tonnage_list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/tonnage_list/_json.py
+-rw-r--r--   0 root         (0) root         (0)     6084 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/tonnage_list/api.py
+-rw-r--r--   0 root         (0) root         (0)     7229 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/tonnage_list/data_frame.py
+-rw-r--r--   0 root         (0) root         (0)    26447 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/tonnage_list/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/util/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6505 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/util/parsing_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     6529 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/util/request_helpers.py
+-rw-r--r--   0 root         (0) root         (0)      647 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessel_class.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessel_class_api.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessel_class_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/vessel_emissions/
+-rw-r--r--   0 root         (0) root         (0)      761 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessel_emissions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18460 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessel_emissions/models.py
+-rw-r--r--   0 root         (0) root         (0)    14752 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessel_emissions/vessel_emissions_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/vessel_valuations/
+-rw-r--r--   0 root         (0) root         (0)      298 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessel_valuations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessel_valuations/_valuation_json.py
+-rw-r--r--   0 root         (0) root         (0)      608 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessel_valuations/models.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessel_valuations/vessel_valuations_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/vessels/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17416 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessels/models.py
+-rw-r--r--   0 root         (0) root         (0)     3539 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/vessels/vessels_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.956465 signal-ocean-7.2.1/signal_ocean/voyages/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/voyages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46114 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/voyages/models.py
+-rw-r--r--   0 root         (0) root         (0)    44712 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/voyages/voyages_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.960465 signal-ocean-7.2.1/signal_ocean/voyages_market_data/
+-rw-r--r--   0 root         (0) root         (0)      539 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/voyages_market_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15350 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/voyages_market_data/models.py
+-rw-r--r--   0 root         (0) root         (0)    15865 2023-08-07 11:38:57.000000 signal-ocean-7.2.1/signal_ocean/voyages_market_data/voyages_market_data_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 11:39:56.948465 signal-ocean-7.2.1/signal_ocean.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-08-07 11:39:56.000000 signal-ocean-7.2.1/signal_ocean.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5081 2023-08-07 11:39:56.000000 signal-ocean-7.2.1/signal_ocean.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 11:39:56.000000 signal-ocean-7.2.1/signal_ocean.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2023-08-07 11:39:56.000000 signal-ocean-7.2.1/signal_ocean.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 11:39:56.000000 signal-ocean-7.2.1/signal_ocean.egg-info/top_level.txt
```

### Comparing `signal-ocean-7.1.2/LICENSE` & `signal-ocean-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/PKG-INFO` & `signal-ocean-7.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-ocean
-Version: 7.1.2
+Version: 7.2.1
 Summary: Access Signal Ocean Platform data using Python.
 Home-page: https://apis.signalocean.com/
 Author: Signal Ocean Developers
 Author-email: signaloceandevelopers@thesignalgroup.com
 License: Apache 2.0
 Project-URL: The Signal Group, https://www.thesignalgroup.com/
 Project-URL: Signal Ocean, https://www.signalocean.com/
```

### Comparing `signal-ocean-7.1.2/README.md` & `signal-ocean-7.2.1/README.md`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/setup.py` & `signal-ocean-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/__init__.py` & `signal-ocean-7.2.1/signal_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/_internals.py` & `signal-ocean-7.2.1/signal_ocean/_internals.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/companies/companies_api.py` & `signal-ocean-7.2.1/signal_ocean/companies/companies_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/companies/models.py` & `signal-ocean-7.2.1/signal_ocean/companies/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/connection.py` & `signal-ocean-7.2.1/signal_ocean/connection.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/distances/__init__.py` & `signal-ocean-7.2.1/signal_ocean/distances/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/distances/_distances_json.py` & `signal-ocean-7.2.1/signal_ocean/distances/_distances_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/distances/distances_api.py` & `signal-ocean-7.2.1/signal_ocean/distances/distances_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/distances/models.py` & `signal-ocean-7.2.1/signal_ocean/distances/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/distances/port_filter.py` & `signal-ocean-7.2.1/signal_ocean/distances/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/distances/vessel_class_filter.py` & `signal-ocean-7.2.1/signal_ocean/distances/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_pricing/__init__.py` & `signal-ocean-7.2.1/signal_ocean/freight_pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_pricing/_freight_pricing_json.py` & `signal-ocean-7.2.1/signal_ocean/freight_pricing/_freight_pricing_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_pricing/freight_pricing_api.py` & `signal-ocean-7.2.1/signal_ocean/freight_pricing/freight_pricing_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_pricing/models.py` & `signal-ocean-7.2.1/signal_ocean/freight_pricing/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_pricing/port_filter.py` & `signal-ocean-7.2.1/signal_ocean/freight_pricing/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_class_filter.py` & `signal-ocean-7.2.1/signal_ocean/freight_pricing/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_pricing/vessel_type_filter.py` & `signal-ocean-7.2.1/signal_ocean/freight_pricing/vessel_type_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_rates/__init__.py` & `signal-ocean-7.2.1/signal_ocean/freight_rates/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_rates/_freight_rates_json.py` & `signal-ocean-7.2.1/signal_ocean/freight_rates/_freight_rates_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_rates/enums.py` & `signal-ocean-7.2.1/signal_ocean/freight_rates/enums.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_rates/freight_rates_api.py` & `signal-ocean-7.2.1/signal_ocean/freight_rates/freight_rates_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_rates/models.py` & `signal-ocean-7.2.1/signal_ocean/freight_rates/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_rates/port_filter.py` & `signal-ocean-7.2.1/signal_ocean/freight_rates/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/freight_rates/utils.py` & `signal-ocean-7.2.1/signal_ocean/freight_rates/utils.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/geos/geos_api.py` & `signal-ocean-7.2.1/signal_ocean/geos/geos_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/geos/models.py` & `signal-ocean-7.2.1/signal_ocean/geos/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/__init__.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/column.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/column.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/commercial_status.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/commercial_status.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/historical_tonnage_list.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/historical_tonnage_list.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/market_deployment.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/market_deployment.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/operational_status.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/operational_status.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/tonnage_list.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/tonnage_list.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/vessel.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel_filter.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/vessel_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/historical_tonnage_list/vessel_subclass.py` & `signal-ocean-7.2.1/signal_ocean/historical_tonnage_list/vessel_subclass.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/market_rates/__init__.py` & `signal-ocean-7.2.1/signal_ocean/market_rates/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/market_rates/_market_rates_json.py` & `signal-ocean-7.2.1/signal_ocean/market_rates/_market_rates_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/market_rates/market_rates_api.py` & `signal-ocean-7.2.1/signal_ocean/market_rates/market_rates_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/market_rates/models.py` & `signal-ocean-7.2.1/signal_ocean/market_rates/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/market_rates/utils.py` & `signal-ocean-7.2.1/signal_ocean/market_rates/utils.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/market_rates/vessel_classes.py` & `signal-ocean-7.2.1/signal_ocean/market_rates/vessel_classes.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/plots.py` & `signal-ocean-7.2.1/signal_ocean/plots.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/port.py` & `signal-ocean-7.2.1/signal_ocean/port.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/port_api.py` & `signal-ocean-7.2.1/signal_ocean/port_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/port_congestion/models.py` & `signal-ocean-7.2.1/signal_ocean/port_congestion/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -115,26 +115,36 @@
 
 @dataclass(frozen=True)
 class PortCongestionTimeSeriesEntry:
     """A Port Congestion API timeseries entry representation.
 
     Attributes:
         queue (int): The port queue size.
+        queue_loading (int): The number of vessels in the queue with
+                             Purpose = Loading
+        queue_discharging (int): The number of vessels in the queue with
+                                 Purpose = Discharging
         arrivals (int): The port arrivals amount.
         departures (int): The port departures amount.
         avg_days_since_arrival (float): Average days since arrival.
         avg_wait_estimate (float): Average waiting time estimate.
+        avg_eventual_days_by_departure (float): Average number of total
+                                                port days of all vessels
+                                                departing on this date
         observation_date (datetime): Corresponding day.
     """
 
     queue: int
+    queue_loading: int
+    queue_discharging: int
     arrivals: int
     departures: int
     avg_days_since_arrival: float
     avg_wait_estimate: float
+    avg_eventual_days_by_departure: float
     observation_date: datetime
 
 
 @dataclass(frozen=True)
 class PortCongestionQueryResponse:
     """Port Congestion API Query endpoint response model.
```

### Comparing `signal-ocean-7.1.2/signal_ocean/port_congestion/port_congestion.py` & `signal-ocean-7.2.1/signal_ocean/port_congestion/port_congestion.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,15 +559,15 @@
         try:
             waiting_time_over_time = self._get_waiting_time_over_time(
                 congestion_start_date, vessel_class_id, ports, areas
             )
         except RuntimeError:
             waiting_time_over_time = cast(
                 DataSet[WaitingTimeOverTime],
-                {"date": congestion_start_date, "avg_waiting_time": 0.0}
+                {"date": congestion_start_date, "avg_waiting_time": 0.0},
             )
 
         live_port_congestion = self._calculate_live_port_congestion(
             vessels_congestion_data
         )
 
         return (
```

### Comparing `signal-ocean-7.1.2/signal_ocean/port_congestion/port_congestion_api.py` & `signal-ocean-7.2.1/signal_ocean/port_congestion/port_congestion_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/port_expenses/__init__.py` & `signal-ocean-7.2.1/signal_ocean/port_expenses/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/port_expenses/_port_expenses_json.py` & `signal-ocean-7.2.1/signal_ocean/port_expenses/_port_expenses_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/port_expenses/enums.py` & `signal-ocean-7.2.1/signal_ocean/port_expenses/enums.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/port_expenses/models.py` & `signal-ocean-7.2.1/signal_ocean/port_expenses/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/port_expenses/port_expenses_api.py` & `signal-ocean-7.2.1/signal_ocean/port_expenses/port_expenses_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/port_expenses/port_filter.py` & `signal-ocean-7.2.1/signal_ocean/port_expenses/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/port_filter.py` & `signal-ocean-7.2.1/signal_ocean/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/scraped_cargoes/models.py` & `signal-ocean-7.2.1/signal_ocean/scraped_cargoes/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/scraped_cargoes/scraped_cargoes_api.py` & `signal-ocean-7.2.1/signal_ocean/scraped_cargoes/scraped_cargoes_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/scraped_data/scraped_data_api.py` & `signal-ocean-7.2.1/signal_ocean/scraped_data/scraped_data_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/scraped_fixtures/models.py` & `signal-ocean-7.2.1/signal_ocean/scraped_fixtures/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/scraped_fixtures/scraped_fixtures_api.py` & `signal-ocean-7.2.1/signal_ocean/scraped_fixtures/scraped_fixtures_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/scraped_lineups/models.py` & `signal-ocean-7.2.1/signal_ocean/scraped_lineups/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/scraped_lineups/scraped_lineups_api.py` & `signal-ocean-7.2.1/signal_ocean/scraped_lineups/scraped_lineups_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/scraped_positions/models.py` & `signal-ocean-7.2.1/signal_ocean/scraped_positions/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/scraped_positions/scraped_positions_api.py` & `signal-ocean-7.2.1/signal_ocean/scraped_positions/scraped_positions_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/tonnage_list/__init__.py` & `signal-ocean-7.2.1/signal_ocean/tonnage_list/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/tonnage_list/_json.py` & `signal-ocean-7.2.1/signal_ocean/tonnage_list/_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/tonnage_list/api.py` & `signal-ocean-7.2.1/signal_ocean/tonnage_list/api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/tonnage_list/data_frame.py` & `signal-ocean-7.2.1/signal_ocean/tonnage_list/data_frame.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/tonnage_list/models.py` & `signal-ocean-7.2.1/signal_ocean/tonnage_list/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/util/parsing_helpers.py` & `signal-ocean-7.2.1/signal_ocean/util/parsing_helpers.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/util/request_helpers.py` & `signal-ocean-7.2.1/signal_ocean/util/request_helpers.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/vessel_class.py` & `signal-ocean-7.2.1/signal_ocean/vessel_class.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/vessel_class_api.py` & `signal-ocean-7.2.1/signal_ocean/vessel_class_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/vessel_class_filter.py` & `signal-ocean-7.2.1/signal_ocean/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/vessel_emissions/__init__.py` & `signal-ocean-7.2.1/signal_ocean/vessel_emissions/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/vessel_emissions/models.py` & `signal-ocean-7.2.1/signal_ocean/vessel_emissions/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,36 @@
 """The models for vessel emissions api."""
 import dataclasses
 from dataclasses import dataclass
-from typing import Optional, List
+from typing import Optional, List, Dict, Any
 from operator import attrgetter
 
 
+def _to_camel_case_with_special_keywords(s: str) -> str:
+    special_keywords = [
+        'imo', 'id', 'co', 'co2', 'ch', 'nmvoc',
+    ]
+    _to_camelcase = s.split('_')
+    _to_camelcase = [
+        word.capitalize() if word not in special_keywords
+        else word.upper()
+        for word in _to_camelcase
+    ]
+    result = ''.join(_to_camelcase)
+    if 'Tons' in result:
+        result = (
+            result.replace('in', 'In').
+            replace('Nmvoc', 'NMVOC').
+            replace('Sox', 'SOx').
+            replace('Nox', 'NOx').
+            replace('Co', 'CO')
+        )
+    return result
+
+
 @dataclass(frozen=True)
 class Emissions:
     """Contains the reported emissions per gas type.
 
     Attributes:
     co2_in_tons: CO2 emissions in tons
     coin_tons: CO emissions in tons
@@ -257,18 +279,18 @@
     Attributes:
         emissions: Voyage emissions info
         consumptions: Voyage consumptions info
         distances: Voyage distances info
         duration: Voyage duration info
 
     """
-    emissions: Optional[EmissionsBreakdown]
-    consumptions: Optional[ConsumptionsBreakdown]
-    distances: Optional[DistancesBreakdown]
-    duration: Optional[DurationBreakdown]
+    emissions: Optional[EmissionsBreakdown] = None
+    consumptions: Optional[ConsumptionsBreakdown] = None
+    distances: Optional[DistancesBreakdown] = None
+    duration: Optional[DurationBreakdown] = None
 
 
 @dataclass(frozen=True)
 class EmissionsEstimation:
     """Contains info about the emissions estimation.
 
     Attributes:
@@ -341,14 +363,28 @@
         )
 
         nodef_f_repr = ", ".join(f"{name}={value}"
                                  for name, value
                                  in nodef_f_vals)
         return f"{self.__class__.__name__}({nodef_f_repr})"
 
+    def to_dict(self) -> Dict[Any, Any]:
+        """Cast EmissionsEstimation object to dict.
+
+        Returns:
+            Dict representation of EmissionsEstimation model
+
+        """
+        return dataclasses.asdict(
+            self,
+            dict_factory=lambda x: {
+                _to_camel_case_with_special_keywords(k): v
+                for (k, v) in x if v is not None
+            })
+
 
 @dataclass(frozen=True)
 class Eexi:
     """Contains EEXI info.
 
     Attributes:
         value: Acquired EEXI value
@@ -442,33 +478,95 @@
     vessel_class: Optional[str] = None
     vessel_class_id: Optional[int] = None
     eexi: Optional[Eexi] = None
     eiv: Optional[Eiv] = None
     aer: Optional[Aer] = None
     cii: Optional[Cii] = None
 
+    def __repr__(self) -> str:
+        """Override of the default __repr__ function.
+
+        Returns:
+            Object string representation omitting None attributes
+
+        """
+        nodef_f_vals = (
+            (f.name, attrgetter(f.name)(self))
+            for f in dataclasses.fields(self)
+            if attrgetter(f.name)(self) != f.default
+        )
+
+        nodef_f_repr = ", ".join(f"{name}={value}"
+                                 for name, value
+                                 in nodef_f_vals)
+        return f"{self.__class__.__name__}({nodef_f_repr})"
+
+    def to_dict(self) -> Dict[Any, Any]:
+        """Cast VesselMetrics object to dict.
+
+        Returns:
+            Dict representation of VesselMetrics object
+
+        """
+        return dataclasses.asdict(
+            self,
+            dict_factory=lambda x: {
+                _to_camel_case_with_special_keywords(k): v
+                for (k, v) in x if v is not None
+            })
+
 
 @dataclass(frozen=True)
 class VesselClassEmissions:
     """Contains Vessel Class Emissions.
 
     Attributes:
         next_page_token: String. The key  to retrieve the next page
         data: List of Vessel Emissions for available vessels of this class
 
     """
     next_page_token: str
     data: List[EmissionsEstimation]
 
+    def to_dict(self) -> Dict[Any, Any]:
+        """Cast VesselClassEmissions object to dict.
+
+        Returns:
+            Dict representation of VesselClassEmissions object
+
+        """
+        return {
+            "NextPageToken": self.next_page_token,
+            "Data": [
+                vessel_emissions.to_dict()
+                for vessel_emissions in self.data
+            ]
+        }
+
 
 @dataclass(frozen=True)
 class VesselClassMetrics:
     """Contains Vessel Class Metrics.
 
     Attributes:
         next_page_token: String. The key that should be used
         as a parameter of the token to retrieve the next page
         data: List of Vessel Metrics for available vessels of this class
 
     """
     next_page_token: str
     data: List[VesselMetrics]
+
+    def to_dict(self) -> Dict[Any, Any]:
+        """Cast VesselClassMetrics object to dict.
+
+        Returns:
+            Dict representation of VesselClassMetrics object
+
+        """
+        return {
+            "NextPageToken": self.next_page_token,
+            "Data": [
+                vessel_metrics.to_dict()
+                for vessel_metrics in self.data
+            ]
+        }
```

### Comparing `signal-ocean-7.1.2/signal_ocean/vessel_emissions/vessel_emissions_api.py` & `signal-ocean-7.2.1/signal_ocean/vessel_emissions/vessel_emissions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """The vessel emissions api."""
+import os
+import copy
 from typing import Optional, List, Union, Dict, Any
 from urllib.parse import urljoin, urlencode
 from datetime import date
 from signal_ocean import Connection
 from signal_ocean.util.request_helpers import get_multiple, get_single
 from signal_ocean.vessel_emissions.models import EmissionsEstimation, \
     VesselMetrics, VesselClassEmissions, VesselClassMetrics
@@ -36,15 +38,16 @@
 
     Returns:
         headers dict
 
     """
     return {
         "Ocp-Apim-Subscription-Key":
-            connection._Connection__api_key,  # type: ignore
+            connection._Connection__api_key  # type: ignore
+            or os.environ.get("SIGNAL_OCEAN_API_KEY"),
         "Content-Type": "application/json",
         "Source": "SignalSDK",
     }
 
 
 class VesselEmissionsAPI:
     """Represents Signal's Vessel Emissions API."""
@@ -56,21 +59,22 @@
         """Initializes VesselEmissionsAPI.
 
         Args:
             connection: API connection configuration. If not provided, the
                 default connection method is used.
         """
         if connection is not None:
+            em_connection = copy.deepcopy(connection)
             func_type = type(
-                connection._Connection__get_headers  # type: ignore
+                em_connection._Connection__get_headers  # type: ignore
             )
-            connection._Connection__get_headers = func_type(  # type: ignore
-                custom_headers, connection
+            em_connection._Connection__get_headers = func_type(  # type: ignore
+                custom_headers, em_connection
             )
-            self.__connection = connection
+            self.__connection = em_connection
         else:
             connection = Connection()
             func_type = type(
                 connection._Connection__get_headers  # type: ignore
             )
             connection._Connection__get_headers = func_type(  # type: ignore
                 custom_headers, connection
```

### Comparing `signal-ocean-7.1.2/signal_ocean/vessel_valuations/_valuation_json.py` & `signal-ocean-7.2.1/signal_ocean/vessel_valuations/_valuation_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/vessel_valuations/models.py` & `signal-ocean-7.2.1/signal_ocean/vessel_valuations/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/vessel_valuations/vessel_valuations_api.py` & `signal-ocean-7.2.1/signal_ocean/vessel_valuations/vessel_valuations_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/vessels/models.py` & `signal-ocean-7.2.1/signal_ocean/vessels/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/vessels/vessels_api.py` & `signal-ocean-7.2.1/signal_ocean/vessels/vessels_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/voyages/__init__.py` & `signal-ocean-7.2.1/signal_ocean/voyages/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/voyages/models.py` & `signal-ocean-7.2.1/signal_ocean/voyages/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/voyages/voyages_api.py` & `signal-ocean-7.2.1/signal_ocean/voyages/voyages_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/voyages_market_data/__init__.py` & `signal-ocean-7.2.1/signal_ocean/voyages_market_data/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/voyages_market_data/models.py` & `signal-ocean-7.2.1/signal_ocean/voyages_market_data/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean/voyages_market_data/voyages_market_data_api.py` & `signal-ocean-7.2.1/signal_ocean/voyages_market_data/voyages_market_data_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.2/signal_ocean.egg-info/PKG-INFO` & `signal-ocean-7.2.1/signal_ocean.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-ocean
-Version: 7.1.2
+Version: 7.2.1
 Summary: Access Signal Ocean Platform data using Python.
 Home-page: https://apis.signalocean.com/
 Author: Signal Ocean Developers
 Author-email: signaloceandevelopers@thesignalgroup.com
 License: Apache 2.0
 Project-URL: The Signal Group, https://www.thesignalgroup.com/
 Project-URL: Signal Ocean, https://www.signalocean.com/
```

### Comparing `signal-ocean-7.1.2/signal_ocean.egg-info/SOURCES.txt` & `signal-ocean-7.2.1/signal_ocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

