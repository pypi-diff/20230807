# Comparing `tmp/binance-connector-3.2.0.tar.gz` & `tmp/binance-connector-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-connector-3.2.0.tar", last modified: Tue Aug  1 02:06:01 2023, max compression
+gzip compressed data, was "binance-connector-3.3.0.tar", last modified: Mon Aug  7 13:41:03 2023, max compression
```

## Comparing `binance-connector-3.2.0.tar` & `binance-connector-3.3.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.646999 binance-connector-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 02:05:58.000000 binance-connector-3.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 02:05:58.000000 binance-connector-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-08-01 02:06:01.646999 binance-connector-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-08-01 02:05:58.000000 binance-connector-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.634999 binance-connector-3.2.0/binance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.634999 binance-connector-3.2.0/binance/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/lib/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/lib/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.642999 binance-connector-3.2.0/binance/spot/
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_blvt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_bswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_c2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_fiat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_gift_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_loan.py
--rw-r--r--   0 runner    (1001) docker     (123)    33152 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_market.py
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_mining.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_pay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_portfolio_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_rebate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_savings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    30191 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_sub_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/spot/_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.642999 binance-connector-3.2.0/binance/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/binance_socket_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.642999 binance-connector-3.2.0/binance/websocket/spot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.646999 binance-connector-3.2.0/binance/websocket/spot/websocket_api/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_api/_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    24597 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_api/_market.py
--rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_api/_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_api/_user_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/spot/websocket_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-01 02:05:58.000000 binance-connector-3.2.0/binance/websocket/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.646999 binance-connector-3.2.0/binance_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-08-01 02:06:01.000000 binance-connector-3.2.0/binance_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-01 02:06:01.000000 binance-connector-3.2.0/binance_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:06:01.000000 binance-connector-3.2.0/binance_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 02:06:01.000000 binance-connector-3.2.0/binance_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 02:06:01.000000 binance-connector-3.2.0/binance_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.646999 binance-connector-3.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:05:58.000000 binance-connector-3.2.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:06:01.646999 binance-connector-3.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 02:05:58.000000 binance-connector-3.2.0/requirements/common.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-01 02:06:01.646999 binance-connector-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-01 02:05:58.000000 binance-connector-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:03.694516 binance-connector-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-07 13:40:57.000000 binance-connector-3.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-07 13:40:57.000000 binance-connector-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-08-07 13:41:03.694516 binance-connector-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-08-07 13:40:57.000000 binance-connector-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:03.686516 binance-connector-3.3.0/binance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:03.686516 binance-connector-3.3.0/binance/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/lib/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/lib/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:03.690516 binance-connector-3.3.0/binance/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_blvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_bswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_c2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_fiat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_gift_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_loan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33152 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_mining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_pay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_portfolio_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_rebate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_savings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30191 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_sub_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/spot/_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:03.690516 binance-connector-3.3.0/binance/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/websocket/binance_socket_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:03.690516 binance-connector-3.3.0/binance/websocket/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/websocket/spot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:03.690516 binance-connector-3.3.0/binance/websocket/spot/websocket_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/websocket/spot/websocket_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/websocket/spot/websocket_api/_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24597 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/websocket/spot/websocket_api/_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/websocket/spot/websocket_api/_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/websocket/spot/websocket_api/_user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/websocket/spot/websocket_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-07 13:40:57.000000 binance-connector-3.3.0/binance/websocket/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:03.694516 binance-connector-3.3.0/binance_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-08-07 13:41:03.000000 binance-connector-3.3.0/binance_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-07 13:41:03.000000 binance-connector-3.3.0/binance_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 13:41:03.000000 binance-connector-3.3.0/binance_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-07 13:41:03.000000 binance-connector-3.3.0/binance_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 13:41:03.000000 binance-connector-3.3.0/binance_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:03.694516 binance-connector-3.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 13:40:57.000000 binance-connector-3.3.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 13:41:03.694516 binance-connector-3.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-07 13:40:57.000000 binance-connector-3.3.0/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-07 13:41:03.694516 binance-connector-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-07 13:40:57.000000 binance-connector-3.3.0/setup.py
```

### Comparing `binance-connector-3.2.0/LICENSE.md` & `binance-connector-3.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/PKG-INFO` & `binance-connector-3.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: binance-connector
-Version: 3.2.0
-Summary: This is a lightweight library that works as a connector to Binance public API.
-Home-page: https://github.com/binance/binance-connector-python
-License: MIT
-Keywords: Binance,Public API
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # Binance Public API Connector Python
 [![PyPI version](https://img.shields.io/pypi/v/binance-connector)](https://pypi.python.org/pypi/binance-connector)
 [![Python version](https://img.shields.io/pypi/pyversions/binance-connector)](https://www.python.org/downloads/)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue)](https://binance-connector.readthedocs.io/en/stable/)
 [![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
@@ -283,14 +265,75 @@
 
 # Subscribe to a single symbol stream
 my_client.agg_trade(symbol="bnbusdt")
 time.sleep(5)
 logging.info("closing ws connection")
 my_client.stop()
 ```
+
+#### Proxy
+
+Proxy is supported for both WebSocket API and WebSocket Stream.
+
+To use it, pass in the `proxies` parameter when initializing the client.
+
+The format of the `proxies` parameter is the same as the one used in the Spot RESTful API.
+
+It consists on a dictionary with the following format, where the key is the type of the proxy and the value is the proxy URL:
+
+For websockets, the proxy type is `http`.
+
+```python
+proxies = { 'http': 'http://1.2.3.4:8080' }
+```
+
+You can also use authentication for the proxy by adding the `username` and `password` parameters to the proxy URL:
+
+```python
+proxies = { 'http': 'http://username:password@host:port' }
+```
+
+
+```python
+
+# WebSocket API Client
+from binance.websocket.spot.websocket_api import SpotWebsocketAPIClient
+
+def message_handler(_, message):
+    logging.info(message)
+
+proxies = { 'http': 'http://1.2.3.4:8080' }
+
+my_client = SpotWebsocketAPIClient(on_message=message_handler, proxies=proxies)
+
+my_client.ticker(symbol="BNBBUSD", type="FULL")
+
+time.sleep(5)
+logging.info("closing ws connection")
+my_client.stop()
+```
+
+```python
+
+# WebSocket Stream Client
+from binance.websocket.spot.websocket_stream import SpotWebsocketStreamClient
+
+def message_handler(_, message):
+    logging.info(message)
+
+proxies = { 'http': 'http://1.2.3.4:8080' }
+
+my_client = SpotWebsocketStreamClient(on_message=message_handler, proxies=proxies)
+
+# Subscribe to a single symbol stream
+my_client.agg_trade(symbol="bnbusdt")
+time.sleep(5)
+logging.info("closing ws connection")
+my_client.stop()
+```
 
 #### Request Id
 
 Client can assign a request id to each request. The request id will be returned in the response message. Not mandatory in the library, it generates a uuid format string if not provided.
 
 ```python
 # id provided by client
```

### Comparing `binance-connector-3.2.0/README.md` & `binance-connector-3.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: binance-connector
+Version: 3.3.0
+Summary: This is a lightweight library that works as a connector to Binance public API.
+Home-page: https://github.com/binance/binance-connector-python
+License: MIT
+Keywords: Binance,Public API
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # Binance Public API Connector Python
 [![PyPI version](https://img.shields.io/pypi/v/binance-connector)](https://pypi.python.org/pypi/binance-connector)
 [![Python version](https://img.shields.io/pypi/pyversions/binance-connector)](https://www.python.org/downloads/)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue)](https://binance-connector.readthedocs.io/en/stable/)
 [![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
@@ -265,14 +283,75 @@
 
 # Subscribe to a single symbol stream
 my_client.agg_trade(symbol="bnbusdt")
 time.sleep(5)
 logging.info("closing ws connection")
 my_client.stop()
 ```
+
+#### Proxy
+
+Proxy is supported for both WebSocket API and WebSocket Stream.
+
+To use it, pass in the `proxies` parameter when initializing the client.
+
+The format of the `proxies` parameter is the same as the one used in the Spot RESTful API.
+
+It consists on a dictionary with the following format, where the key is the type of the proxy and the value is the proxy URL:
+
+For websockets, the proxy type is `http`.
+
+```python
+proxies = { 'http': 'http://1.2.3.4:8080' }
+```
+
+You can also use authentication for the proxy by adding the `username` and `password` parameters to the proxy URL:
+
+```python
+proxies = { 'http': 'http://username:password@host:port' }
+```
+
+
+```python
+
+# WebSocket API Client
+from binance.websocket.spot.websocket_api import SpotWebsocketAPIClient
+
+def message_handler(_, message):
+    logging.info(message)
+
+proxies = { 'http': 'http://1.2.3.4:8080' }
+
+my_client = SpotWebsocketAPIClient(on_message=message_handler, proxies=proxies)
+
+my_client.ticker(symbol="BNBBUSD", type="FULL")
+
+time.sleep(5)
+logging.info("closing ws connection")
+my_client.stop()
+```
+
+```python
+
+# WebSocket Stream Client
+from binance.websocket.spot.websocket_stream import SpotWebsocketStreamClient
+
+def message_handler(_, message):
+    logging.info(message)
+
+proxies = { 'http': 'http://1.2.3.4:8080' }
+
+my_client = SpotWebsocketStreamClient(on_message=message_handler, proxies=proxies)
+
+# Subscribe to a single symbol stream
+my_client.agg_trade(symbol="bnbusdt")
+time.sleep(5)
+logging.info("closing ws connection")
+my_client.stop()
+```
 
 #### Request Id
 
 Client can assign a request id to each request. The request id will be returned in the response message. Not mandatory in the library, it generates a uuid format string if not provided.
 
 ```python
 # id provided by client
```

### Comparing `binance-connector-3.2.0/binance/api.py` & `binance-connector-3.3.0/binance/api.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/error.py` & `binance-connector-3.3.0/binance/error.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/lib/authentication.py` & `binance-connector-3.3.0/binance/lib/authentication.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/lib/enums.py` & `binance-connector-3.3.0/binance/lib/enums.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/lib/utils.py` & `binance-connector-3.3.0/binance/lib/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 import time
 import uuid
+
+from urllib.parse import urlparse
 from collections import OrderedDict
 from urllib.parse import urlencode
 from binance.lib.authentication import hmac_hashing
 from binance.error import (
     ParameterRequiredError,
     ParameterValueError,
     ParameterTypeError,
@@ -108,7 +110,23 @@
     parameters["timestamp"] = get_timestamp()
     parameters["apiKey"] = api_key
 
     parameters = OrderedDict(sorted(parameters.items()))
     parameters["signature"] = hmac_hashing(api_secret, urlencode(parameters))
 
     return parameters
+
+
+def parse_proxies(proxies: dict):
+    """Parse proxy url from dict, only support http and https proxy, not support socks5 proxy"""
+    proxy_url = proxies.get("http") or proxies.get("https")
+    if not proxy_url:
+        return {}
+
+    parsed = urlparse(proxy_url)
+    return {
+        "http_proxy_host": parsed.hostname,
+        "http_proxy_port": parsed.port,
+        "http_proxy_auth": (parsed.username, parsed.password)
+        if parsed.username and parsed.password
+        else None,
+    }
```

### Comparing `binance-connector-3.2.0/binance/spot/__init__.py` & `binance-connector-3.3.0/binance/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_blvt.py` & `binance-connector-3.3.0/binance/spot/_blvt.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_bswap.py` & `binance-connector-3.3.0/binance/spot/_bswap.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_c2c.py` & `binance-connector-3.3.0/binance/spot/_c2c.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_convert.py` & `binance-connector-3.3.0/binance/spot/_convert.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_data_stream.py` & `binance-connector-3.3.0/binance/spot/_data_stream.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_fiat.py` & `binance-connector-3.3.0/binance/spot/_fiat.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_futures.py` & `binance-connector-3.3.0/binance/spot/_futures.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_gift_card.py` & `binance-connector-3.3.0/binance/spot/_gift_card.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_loan.py` & `binance-connector-3.3.0/binance/spot/_loan.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_margin.py` & `binance-connector-3.3.0/binance/spot/_margin.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_market.py` & `binance-connector-3.3.0/binance/spot/_market.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_mining.py` & `binance-connector-3.3.0/binance/spot/_mining.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_nft.py` & `binance-connector-3.3.0/binance/spot/_nft.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_portfolio_margin.py` & `binance-connector-3.3.0/binance/spot/_portfolio_margin.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_savings.py` & `binance-connector-3.3.0/binance/spot/_savings.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_staking.py` & `binance-connector-3.3.0/binance/spot/_staking.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_sub_account.py` & `binance-connector-3.3.0/binance/spot/_sub_account.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_trade.py` & `binance-connector-3.3.0/binance/spot/_trade.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/spot/_wallet.py` & `binance-connector-3.3.0/binance/spot/_wallet.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/websocket/binance_socket_manager.py` & `binance-connector-3.3.0/binance/websocket/binance_socket_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,57 @@
+from typing import Optional
+
 import logging
 import threading
 from websocket import (
     ABNF,
     create_connection,
     WebSocketException,
     WebSocketConnectionClosedException,
 )
+from binance.lib.utils import parse_proxies
 
 
 class BinanceSocketManager(threading.Thread):
     def __init__(
         self,
         stream_url,
         on_message=None,
         on_open=None,
         on_close=None,
         on_error=None,
         on_ping=None,
         on_pong=None,
         logger=None,
+        proxies: Optional[dict] = None,
     ):
         threading.Thread.__init__(self)
         if not logger:
             logger = logging.getLogger(__name__)
         self.logger = logger
         self.stream_url = stream_url
         self.on_message = on_message
         self.on_open = on_open
         self.on_close = on_close
         self.on_ping = on_ping
         self.on_pong = on_pong
         self.on_error = on_error
+        self.proxies = proxies
+
+        self._proxy_params = parse_proxies(proxies) if proxies else {}
+
         self.create_ws_connection()
 
     def create_ws_connection(self):
         self.logger.debug(
-            "Creating connection with WebSocket Server: %s", self.stream_url
+            f"Creating connection with WebSocket Server: {self.stream_url}, proxies: {self.proxies}",
         )
-        self.ws = create_connection(self.stream_url)
+        self.ws = create_connection(self.stream_url, **self._proxy_params)
         self.logger.debug(
-            "WebSocket connection has been established: %s", self.stream_url
+            f"WebSocket connection has been established: {self.stream_url}, proxies: {self.proxies}",
         )
         self._callback(self.on_open)
 
     def run(self):
         self.read_data()
 
     def send_message(self, message):
```

### Comparing `binance-connector-3.2.0/binance/websocket/spot/websocket_api/__init__.py` & `binance-connector-3.3.0/binance/websocket/spot/websocket_api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from binance.websocket.websocket_client import BinanceWebsocketClient
 
 
 class SpotWebsocketAPIClient(BinanceWebsocketClient):
     def __init__(
         self,
         stream_url="wss://ws-api.binance.com/ws-api/v3",
@@ -9,26 +11,28 @@
         api_secret=None,
         on_message=None,
         on_open=None,
         on_close=None,
         on_error=None,
         on_ping=None,
         on_pong=None,
+        proxies: Optional[dict] = None,
     ):
         self.api_key = api_key
         self.api_secret = api_secret
 
         super().__init__(
             stream_url,
             on_message=on_message,
             on_open=on_open,
             on_close=on_close,
             on_error=on_error,
             on_ping=on_ping,
             on_pong=on_pong,
+            proxies=proxies,
         )
 
     # Market
     from binance.websocket.spot.websocket_api._market import ping_connectivity
     from binance.websocket.spot.websocket_api._market import server_time
     from binance.websocket.spot.websocket_api._market import exchange_info
     from binance.websocket.spot.websocket_api._market import order_book
```

### Comparing `binance-connector-3.2.0/binance/websocket/spot/websocket_api/_account.py` & `binance-connector-3.3.0/binance/websocket/spot/websocket_api/_account.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/websocket/spot/websocket_api/_market.py` & `binance-connector-3.3.0/binance/websocket/spot/websocket_api/_market.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/websocket/spot/websocket_api/_trade.py` & `binance-connector-3.3.0/binance/websocket/spot/websocket_api/_trade.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/websocket/spot/websocket_api/_user_data.py` & `binance-connector-3.3.0/binance/websocket/spot/websocket_api/_user_data.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/binance/websocket/spot/websocket_stream.py` & `binance-connector-3.3.0/binance/websocket/spot/websocket_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,38 @@
+from typing import Optional
+
 from binance.websocket.websocket_client import BinanceWebsocketClient
 
 
 class SpotWebsocketStreamClient(BinanceWebsocketClient):
     def __init__(
         self,
         stream_url="wss://stream.binance.com:9443",
         on_message=None,
         on_open=None,
         on_close=None,
         on_error=None,
         on_ping=None,
         on_pong=None,
         is_combined=False,
+        proxies: Optional[dict] = None,
     ):
         if is_combined:
             stream_url = stream_url + "/stream"
         else:
             stream_url = stream_url + "/ws"
         super().__init__(
             stream_url,
             on_message=on_message,
             on_open=on_open,
             on_close=on_close,
             on_error=on_error,
             on_ping=on_ping,
             on_pong=on_pong,
+            proxies=proxies,
         )
 
     def agg_trade(self, symbol: str, id=None, action=None, **kwargs):
         """Aggregate Trade Streams
 
         The Aggregate Trade Streams push trade information that is aggregated for a single taker order.
```

### Comparing `binance-connector-3.2.0/binance/websocket/websocket_client.py` & `binance-connector-3.3.0/binance/websocket/websocket_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import json
 import logging
 from binance.lib.utils import get_timestamp
 from binance.websocket.binance_socket_manager import BinanceSocketManager
 
 
 class BinanceWebsocketClient:
@@ -14,27 +16,29 @@
         on_message=None,
         on_open=None,
         on_close=None,
         on_error=None,
         on_ping=None,
         on_pong=None,
         logger=None,
+        proxies: Optional[dict] = None,
     ):
         if not logger:
             logger = logging.getLogger(__name__)
         self.logger = logger
         self.socket_manager = self._initialize_socket(
             stream_url,
             on_message,
             on_open,
             on_close,
             on_error,
             on_ping,
             on_pong,
             logger,
+            proxies,
         )
 
         # start the thread
         self.socket_manager.start()
         self.logger.debug("Binance WebSocket Client started.")
 
     def _initialize_socket(
@@ -43,24 +47,26 @@
         on_message,
         on_open,
         on_close,
         on_error,
         on_ping,
         on_pong,
         logger,
+        proxies,
     ):
         return BinanceSocketManager(
             stream_url,
             on_message=on_message,
             on_open=on_open,
             on_close=on_close,
             on_error=on_error,
             on_ping=on_ping,
             on_pong=on_pong,
             logger=logger,
+            proxies=proxies,
         )
 
     def _single_stream(self, stream):
         if isinstance(stream, str):
             return True
         elif isinstance(stream, list):
             return False
```

### Comparing `binance-connector-3.2.0/binance_connector.egg-info/PKG-INFO` & `binance-connector-3.3.0/binance_connector.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: binance-connector
-Version: 3.2.0
+Version: 3.3.0
 Summary: This is a lightweight library that works as a connector to Binance public API.
 Home-page: https://github.com/binance/binance-connector-python
 License: MIT
 Keywords: Binance,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Binance Public API Connector Python
 [![PyPI version](https://img.shields.io/pypi/v/binance-connector)](https://pypi.python.org/pypi/binance-connector)
 [![Python version](https://img.shields.io/pypi/pyversions/binance-connector)](https://www.python.org/downloads/)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue)](https://binance-connector.readthedocs.io/en/stable/)
@@ -283,14 +283,75 @@
 
 # Subscribe to a single symbol stream
 my_client.agg_trade(symbol="bnbusdt")
 time.sleep(5)
 logging.info("closing ws connection")
 my_client.stop()
 ```
+
+#### Proxy
+
+Proxy is supported for both WebSocket API and WebSocket Stream.
+
+To use it, pass in the `proxies` parameter when initializing the client.
+
+The format of the `proxies` parameter is the same as the one used in the Spot RESTful API.
+
+It consists on a dictionary with the following format, where the key is the type of the proxy and the value is the proxy URL:
+
+For websockets, the proxy type is `http`.
+
+```python
+proxies = { 'http': 'http://1.2.3.4:8080' }
+```
+
+You can also use authentication for the proxy by adding the `username` and `password` parameters to the proxy URL:
+
+```python
+proxies = { 'http': 'http://username:password@host:port' }
+```
+
+
+```python
+
+# WebSocket API Client
+from binance.websocket.spot.websocket_api import SpotWebsocketAPIClient
+
+def message_handler(_, message):
+    logging.info(message)
+
+proxies = { 'http': 'http://1.2.3.4:8080' }
+
+my_client = SpotWebsocketAPIClient(on_message=message_handler, proxies=proxies)
+
+my_client.ticker(symbol="BNBBUSD", type="FULL")
+
+time.sleep(5)
+logging.info("closing ws connection")
+my_client.stop()
+```
+
+```python
+
+# WebSocket Stream Client
+from binance.websocket.spot.websocket_stream import SpotWebsocketStreamClient
+
+def message_handler(_, message):
+    logging.info(message)
+
+proxies = { 'http': 'http://1.2.3.4:8080' }
+
+my_client = SpotWebsocketStreamClient(on_message=message_handler, proxies=proxies)
+
+# Subscribe to a single symbol stream
+my_client.agg_trade(symbol="bnbusdt")
+time.sleep(5)
+logging.info("closing ws connection")
+my_client.stop()
+```
 
 #### Request Id
 
 Client can assign a request id to each request. The request id will be returned in the response message. Not mandatory in the library, it generates a uuid format string if not provided.
 
 ```python
 # id provided by client
```

### Comparing `binance-connector-3.2.0/binance_connector.egg-info/SOURCES.txt` & `binance-connector-3.3.0/binance_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binance-connector-3.2.0/setup.py` & `binance-connector-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,14 @@
     keywords=["Binance", "Public API"],
     install_requires=[req for req in requirements],
     packages=find_packages(exclude=("tests",)),
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

