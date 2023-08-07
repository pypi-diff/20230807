# Comparing `tmp/kwenta-1.0.8.tar.gz` & `tmp/kwenta-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwenta-1.0.8.tar", last modified: Mon Jul 24 15:44:23 2023, max compression
+gzip compressed data, was "kwenta-1.0.9.tar", last modified: Mon Aug  7 16:11:27 2023, max compression
```

## Comparing `kwenta-1.0.8.tar` & `kwenta-1.0.9.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 15:43:49.000000 kwenta-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 15:44:23.055659 kwenta-1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.051658 kwenta-1.0.8/kwenta/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/alerts/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/cli/kwenta_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/contracts/json/
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/PerpsV2ExchangeRate.json
--rw-r--r--   0 runner    (1001) docker     (123)    37179 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/PerpsV2Market.json
--rw-r--r--   0 runner    (1001) docker     (123)    43146 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/SMAccount.json
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/SMFactory.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/sUSD.json
--rw-r--r--   0 runner    (1001) docker     (123)    57402 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/kwenta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/pyth/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/pyth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/pyth/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/pyth/pyth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/queries/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/queries/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/queries/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:44:23.055659 kwenta-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-24 15:43:49.000000 kwenta-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:11:27.051813 kwenta-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 16:10:50.000000 kwenta-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-07 16:11:27.051813 kwenta-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:11:27.047813 kwenta-1.0.9/kwenta/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:11:27.047813 kwenta-1.0.9/kwenta/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/alerts/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:11:27.047813 kwenta-1.0.9/kwenta/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/cli/kwenta_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:11:27.047813 kwenta-1.0.9/kwenta/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:11:27.051813 kwenta-1.0.9/kwenta/contracts/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/json/PerpsV2ExchangeRate.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37179 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/json/PerpsV2Market.json
+-rw-r--r--   0 runner    (1001) docker     (123)    43146 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/json/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21092 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/json/PerpsV2MarketSettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/json/PerpsV2MarketState.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/json/PerpsV2MarketViews.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/json/SMAccount.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/json/SMFactory.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/contracts/json/sUSD.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61250 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/kwenta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:11:27.051813 kwenta-1.0.9/kwenta/pyth/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/pyth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/pyth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/pyth/pyth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:11:27.051813 kwenta-1.0.9/kwenta/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/queries/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/queries/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-08-07 16:10:50.000000 kwenta-1.0.9/kwenta/queries/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:11:27.047813 kwenta-1.0.9/kwenta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-07 16:11:27.000000 kwenta-1.0.9/kwenta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-07 16:11:27.000000 kwenta-1.0.9/kwenta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:11:27.000000 kwenta-1.0.9/kwenta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-07 16:11:27.000000 kwenta-1.0.9/kwenta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 16:11:27.000000 kwenta-1.0.9/kwenta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 16:11:27.000000 kwenta-1.0.9/kwenta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 16:11:27.051813 kwenta-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-07 16:10:50.000000 kwenta-1.0.9/setup.py
```

### Comparing `kwenta-1.0.8/PKG-INFO` & `kwenta-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.8/kwenta/alerts/alerts.py` & `kwenta-1.0.9/kwenta/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/cli/kwenta_cli.py` & `kwenta-1.0.9/kwenta/cli/kwenta_cli.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/constants.py` & `kwenta-1.0.9/kwenta/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
 DEFAULT_PRICE_SERVICE_ENDPOINTS = {
     10: "https://xc-mainnet.pyth.network",
     420: "https://xc-testnet.pyth.network",
 }
 
 ACCOUNT_COMMANDS = {
-    "ACCOUNT_MODIFY_MARGIN": [0, ["uint256"]],
+    "ACCOUNT_MODIFY_MARGIN": [0, ["int256"]],
     "ACCOUNT_WITHDRAW_ETH": [1, ["uint256"]],
-    "PERPS_V2_MODIFY_MARGIN": [2, ["address", "uint256"]],
+    "PERPS_V2_MODIFY_MARGIN": [2, ["address", "int256"]],
     "PERPS_V2_WITHDRAW_ALL_MARGIN": [3, ["address"]],
-    "PERPS_V2_SUBMIT_ATOMIC_ORDER": [4, ["address", "uint256", "uint256"]],
-    "PERPS_V2_SUBMIT_DELAYED_ORDER": [5, ["address", "uint256", "uint256", "uint256"]],
-    "PERPS_V2_SUBMIT_OFFCHAIN_DELAYED_ORDER": [6, ["address", "uint256", "uint256"]],
+    "PERPS_V2_SUBMIT_ATOMIC_ORDER": [4, ["address", "int256", "uint256"]],
+    "PERPS_V2_SUBMIT_DELAYED_ORDER": [5, ["address", "int256", "uint256", "uint256"]],
+    "PERPS_V2_SUBMIT_OFFCHAIN_DELAYED_ORDER": [6, ["address", "int256", "uint256"]],
     "PERPS_V2_CLOSE_POSITION": [7, ["address", "uint256"]],
     "PERPS_V2_SUBMIT_CLOSE_DELAYED_ORDER": [8, ["address", "uint256", "uint256"]],
     "PERPS_V2_SUBMIT_CLOSE_OFFCHAIN_DELAYED_ORDER": [9, ["address", "uint256"]],
     "PERPS_V2_CANCEL_DELAYED_ORDER": [10, ["address"]],
     "PERPS_V2_CANCEL_OFFCHAIN_DELAYED_ORDER": [11, ["address"]],
     "GELATO_PLACE_CONDITIONAL_ORDER": [
         12,
```

### Comparing `kwenta-1.0.8/kwenta/contracts/contracts.py` & `kwenta-1.0.9/kwenta/contracts/contracts.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,23 @@
 
 with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/PerpsV2Market.json') as json_file:
     PerpsV2Market_abi = json.load(json_file)
     
 with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/PerpsV2ExchangeRate.json') as json_file:
     PerpsV2ExchangeRate_abi = json.load(json_file)
 
+with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/PerpsV2MarketSettings.json') as json_file:
+    PerpsV2MarketSettings_abi = json.load(json_file)
+
+with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/PerpsV2MarketState.json') as json_file:
+    PerpsV2MarketState_abi = json.load(json_file)
+
+with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/PerpsV2MarketViews.json') as json_file:
+    PerpsV2MarketViews_abi = json.load(json_file)
+
 with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/SMFactory.json') as json_file:
     SMFactory_abi = json.load(json_file)
 
 with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/sUSD.json') as json_file:
     sUSD_abi = json.load(json_file)
 
 with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/SMAccount.json') as json_file:
@@ -27,23 +36,29 @@
         10: '0x8c6f28f2f1a3c87f0f938b96d27520d9751ec8d9',
         420: '0xeBaEAAD9236615542844adC5c149F86C36aD1136'
     },
     "PerpsV2MarketData": {
         10: '0x58e6227510F83d3F45B339F2f7A05a699fDEE6D4',
         420: '0xcE2dC389fc8Be231beECED1D900881e38596d7b2',
     },
+    "PerpsV2MarketSettings":{
+        10: "0x649F44CAC3276557D03223Dbf6395Af65b11c11c"
+    },
     "PerpsV2ExchangeRate": {
         10: '0x2C15259D4886e2C0946f9aB7a5E389c86b3c3b04',
     },
     "SMFactory": {
         10: '0x8234F990b149Ae59416dc260305E565e5DAfEb54',
     },
 }
 
 abis = {
     "sUSD": sUSD_abi,
     "PerpsV2Market": PerpsV2Market_abi,
     "PerpsV2MarketData": PerpsV2MarketData_abi,
+    "PerpsV2MarketSettings": PerpsV2MarketSettings_abi,
+    "PerpsV2MarketViews": PerpsV2MarketViews_abi,
+    "PerpsV2MarketState": PerpsV2MarketState_abi,
     "PerpsV2ExchangeRate": PerpsV2ExchangeRate_abi,
     "SMFactory": SMFactory_abi,
     "SM_Account":SM_Account_abi
 }
```

### Comparing `kwenta-1.0.8/kwenta/contracts/json/PerpsV2ExchangeRate.json` & `kwenta-1.0.9/kwenta/contracts/json/PerpsV2ExchangeRate.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/contracts/json/PerpsV2Market.json` & `kwenta-1.0.9/kwenta/contracts/json/PerpsV2Market.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/contracts/json/PerpsV2MarketData.json` & `kwenta-1.0.9/kwenta/contracts/json/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/contracts/json/SMAccount.json` & `kwenta-1.0.9/kwenta/contracts/json/SMAccount.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/contracts/json/SMFactory.json` & `kwenta-1.0.9/kwenta/contracts/json/SMFactory.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/contracts/json/sUSD.json` & `kwenta-1.0.9/kwenta/contracts/json/sUSD.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/kwenta.py` & `kwenta-1.0.9/kwenta/kwenta.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     ACCOUNT_COMMANDS
 )
 from .contracts import abis, addresses
 from .alerts import Alerts
 from .queries import Queries
 from .pyth import Pyth
 from eth_abi import encode
+import concurrent.futures
 
 warnings.filterwarnings("ignore")
 
 
 class Kwenta:
     def __init__(
         self,
@@ -33,24 +34,26 @@
         network_id: int = None,
         use_estimate_gas: bool = True,
         gql_endpoint_perps: str = None,
         gql_endpoint_rates: str = None,
         price_service_endpoint: str = None,
         telegram_token: str = None,
         telegram_channel_name: str = None,
+        fast_marketload:    bool= False,
     ):
         # set default values
         if network_id is None:
             network_id = DEFAULT_NETWORK_ID
 
         # init account variables
         self.private_key = private_key
         self.wallet_address = wallet_address
         self.use_estimate_gas = use_estimate_gas
         self.provider_rpc = provider_rpc
+        self.fast_marketload = fast_marketload
         # init provider
         if provider_rpc.startswith("https"):
             self.provider_class = Web3.HTTPProvider
         elif provider_rpc.startswith("wss"):
             self.provider_class = Web3.WebsocketProvider
         else:
             raise Exception("RPC endpoint is invalid")
@@ -99,36 +102,24 @@
         if w3.eth.chain_id != self.network_id:
             raise Exception("The RPC `chain_id` must match the stored `network_id`")
         else:
             w3.middleware_onion.inject(geth_poa_middleware, layer=0)
             # self.nonce = w3.eth.get_transaction_count(self.wallet_address)
             return w3
 
-    def _load_markets(self):
-        """
-        Initializes all market contracts
-        ...
-
-        Attributes
-        ----------
-        N/A
-        """
-        marketdata_contract = self.web3.eth.contract(
+    def _load_market(self, market):
+        markertsettings_contract = self.web3.eth.contract(
             self.web3.to_checksum_address(
-                addresses["PerpsV2MarketData"][self.network_id]
+                addresses["PerpsV2MarketSettings"][self.network_id]
             ),
-            abi=abis["PerpsV2MarketData"],
-        )
-        allmarketsdata = (
-            marketdata_contract.functions.allProxiedMarketSummaries().call()
+            abi=abis["PerpsV2MarketSettings"],
         )
-        markets = {}
-        market_contracts = {}
-        for market in allmarketsdata:
-            normalized_market = {
+        maxFundingVelocity = markertsettings_contract.functions.maxFundingVelocity(market[2]).call()
+        skewScale = markertsettings_contract.functions.skewScale(market[2]).call()
+        normalized_market = {
                 "market_address": market[0],
                 "asset": market[1].decode("utf-8").strip("\x00"),
                 "key": market[2],
                 "maxLeverage": market[3],
                 "price": market[4],
                 "marketSize": market[5],
                 "marketSkew": market[6],
@@ -137,22 +128,76 @@
                 "currentFundingVelocity": market[9],
                 "takerFee": market[10][0],
                 "makerFee": market[10][1],
                 "takerFeeDelayedOrder": market[10][2],
                 "makerFeeDelayedOrder": market[10][3],
                 "takerFeeOffchainDelayedOrder": market[10][4],
                 "makerFeeOffchainDelayedOrder": market[10][5],
+                "maxFundingVelocity": maxFundingVelocity,
+                "skewScale": skewScale
             }
-            # set them
-            token_symbol = market[2].decode("utf-8").strip("\x00")[1:-4]
-            markets[token_symbol] = normalized_market
-            market_contracts[token_symbol] = self.web3.eth.contract(
-                self.web3.to_checksum_address(normalized_market["market_address"]),
-                abi=abis["PerpsV2Market"],
-            )
+        token_symbol = market[2].decode("utf-8").strip("\x00")[1:-4]
+        market_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(normalized_market["market_address"]),
+            abi=abis["PerpsV2Market"],
+        )
+        return token_symbol, normalized_market, market_contract
+
+    def _load_markets(self):
+        """
+        Initializes all market contracts
+        ...
+
+        Attributes
+        ----------
+        N/A
+        """
+        marketdata_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(
+                addresses["PerpsV2MarketData"][self.network_id]
+            ),
+            abi=abis["PerpsV2MarketData"],
+        )
+        allmarketsdata = (
+            marketdata_contract.functions.allProxiedMarketSummaries().call()
+        )
+        markets = {}
+        market_contracts = {}
+        if self.fast_marketload:
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                results = list(executor.map(self._load_market, allmarketsdata))
+            for token_symbol, normalized_market, market_contract in results:
+                markets[token_symbol] = normalized_market
+                market_contracts[token_symbol] = market_contract
+        else:
+            for market in allmarketsdata:
+                normalized_market = {
+                    "market_address": market[0],
+                    "asset": market[1].decode("utf-8").strip("\x00"),
+                    "key": market[2],
+                    "maxLeverage": market[3],
+                    "price": market[4],
+                    "marketSize": market[5],
+                    "marketSkew": market[6],
+                    "marketDebt": market[7],
+                    "currentFundingRate": market[8],
+                    "currentFundingVelocity": market[9],
+                    "takerFee": market[10][0],
+                    "makerFee": market[10][1],
+                    "takerFeeDelayedOrder": market[10][2],
+                    "makerFeeDelayedOrder": market[10][3],
+                    "takerFeeOffchainDelayedOrder": market[10][4],
+                    "makerFeeOffchainDelayedOrder": market[10][5],
+                }
+                token_symbol = market[2].decode("utf-8").strip("\x00")[1:-4]
+                markets[token_symbol] = normalized_market
+                market_contracts[token_symbol] = self.web3.eth.contract(
+                    self.web3.to_checksum_address(normalized_market["market_address"]),
+                    abi=abis["PerpsV2Market"],
+                )    
 
         # load sUSD contract
         susd_token = self.web3.eth.contract(
             self.web3.to_checksum_address(addresses["sUSD"][self.network_id]),
             abi=abis["sUSD"],
         )
 
@@ -572,15 +617,57 @@
             percent_short = short / total * 100
         return {
             "long": long,
             "short": short,
             "percent_long": percent_long,
             "percent_short": percent_short,
         }
-
+    def get_funding_rate(self, token_symbol:str) -> dict:
+        """
+        Gets current funding rate for market
+        ...
+        Attributes
+        ----------
+        token_symbol : str
+            token symbol from list of supported assets
+        Returns
+        ----------
+        Dict with funding information
+        """
+        market_contract = self.get_market_contract(token_symbol.upper())
+        funding_rate = market_contract.functions.currentFundingRate().call()
+        if funding_rate < 0:
+            rate_percent = self.web3.from_wei(abs(funding_rate),"ether")*-1
+        else:
+            rate_percent = self.web3.from_wei(abs(funding_rate),"ether")
+        return {
+            "funding_rate_percent": rate_percent
+        }
+    def get_funding_velocity(self, token_symbol:str) -> dict:
+        """
+        Gets current funding rate for market
+        ...
+        Attributes
+        ----------
+        token_symbol : str
+            token symbol from list of supported assets
+        Returns
+        ----------
+        Dict with funding information
+        """
+        market_contract = self.get_market_contract(token_symbol.upper())
+        funding_rate = market_contract.functions.currentFundingVelocity().call()
+        if funding_rate < 0:
+            rate_percent = self.web3.from_wei(abs(funding_rate),"ether")*-1
+        else:
+            rate_percent = self.web3.from_wei(abs(funding_rate),"ether")
+        return {
+            "funding_velocity_percent": rate_percent
+        }
+#  getCurrentFundingVelocity ; getCurrentMarketSkew
     def get_susd_balance(self, address: str) -> dict:
         """
         Gets current sUSD Balance in wallet
         ...
 
         Attributes
         ----------
@@ -740,15 +827,15 @@
         """
         Transfers SUSD from wallet to Margin account
         ...
 
         Attributes
         ----------
         token_amount : int
-            Token amount *in human readable* to send to Margin account
+           sUSD Token amount *in human readable* to send to Margin account
         wallet_address : str
             wallet_address of wallet to check
         skip_approval: bool
             skip susd approval if amount is already approved
         Returns
         ----------
         str: token transfer Tx id
@@ -765,15 +852,15 @@
         if is_withdrawal > 0:
             susd_balance = self.get_susd_balance(self.wallet_address)
         else:
             susd_balance = self.get_susd_balance(self.sm_account)
         print(f"sUSD Balance: {susd_balance['balance_usd']}")
         #check that withdrawal is less than account balance
         if (token_amount > susd_balance["balance"]):
-            raise Exception(f"Token amount: {token_amount} is greater than Account Balance: {{susd_balance['balance_usd']}}! Verify your balance.")
+            raise Exception(f"Token amount: {token_amount} is greater than Account Balance: {susd_balance['balance_usd']} | Verify your balance.")
         #Move amount from EOA Wallet to SM Account 
         if (is_withdrawal > 0):
             if (token_amount > 0) and (skip_approval is False):
                 self.approve_susd(token_amount)
                 print("Waiting for Approval...")
                 time.sleep(4.5)
             #adding to sm account
@@ -1042,16 +1129,16 @@
                 token_symbol, leverage_multiplier
             )
             max_leverage = leveraged_amount["max_asset_leverage"]
             position_size = leveraged_amount["leveraged_amount"]
             position_size = self.web3.to_wei(abs(position_size), "ether") * is_short
         elif position_size:
             # check side
-            if (short == True & position_size > 0) or (
-                short == False & position_size < 0
+            if (short == True and position_size > 0) or (
+                short == False and position_size < 0
             ):
                 print(
                     "Position size and Short value do not line up. Double Check intention."
                 )
                 return None
             max_leverage = self.get_leveraged_amount(token_symbol, 24.7)[
                 "max_asset_leverage"
```

### Comparing `kwenta-1.0.8/kwenta/pyth/constants.py` & `kwenta-1.0.9/kwenta/pyth/constants.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/pyth/pyth.py` & `kwenta-1.0.9/kwenta/pyth/pyth.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/queries/config.py` & `kwenta-1.0.9/kwenta/queries/config.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/queries/gql.py` & `kwenta-1.0.9/kwenta/queries/gql.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta/queries/queries.py` & `kwenta-1.0.9/kwenta/queries/queries.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.8/kwenta.egg-info/PKG-INFO` & `kwenta-1.0.9/kwenta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.8/setup.py` & `kwenta-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kwenta",
-    version="1.0.8",
+    version="1.0.9",
     description="Python SDK for Kwenta",
     long_description="Python SDK for Kwenta",
     author="Kwenta DAO",
     packages=[
         "kwenta",
         "kwenta.alerts",
         "kwenta.cli",
```

