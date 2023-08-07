# Comparing `tmp/dexhub-0.7.2.tar.gz` & `tmp/dexhub-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexhub-0.7.2.tar", last modified: Sun Aug  6 19:49:22 2023, max compression
+gzip compressed data, was "dexhub-0.7.3.tar", last modified: Sun Aug  6 21:43:33 2023, max compression
```

## Comparing `dexhub-0.7.2.tar` & `dexhub-0.7.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.582635 dexhub-0.7.2/
--rw-r--r--   0 czhong     (501) staff       (20)      478 2023-08-06 19:49:22.582487 dexhub-0.7.2/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.7.2/README.md
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.577772 dexhub-0.7.2/dexhub/
--rw-r--r--   0 czhong     (501) staff       (20)     1291 2023-08-06 14:59:24.000000 dexhub-0.7.2/dexhub/__init__.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.579777 dexhub-0.7.2/dexhub/abi/
--rw-r--r--   0 czhong     (501) staff       (20)      261 2023-08-06 10:36:45.000000 dexhub-0.7.2/dexhub/abi/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.7.2/dexhub/abi/arbitrum_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)   120303 2023-05-02 03:17:30.000000 dexhub-0.7.2/dexhub/abi/avax_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    28418 2023-08-06 10:36:23.000000 dexhub-0.7.2/dexhub/abi/dfk_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.7.2/dexhub/abi/eth_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.7.2/dexhub/abi/klay_abi.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.581046 dexhub-0.7.2/dexhub/address/
--rw-r--r--   0 czhong     (501) staff       (20)      499 2023-08-06 14:33:28.000000 dexhub-0.7.2/dexhub/address/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.7.2/dexhub/address/arbitrum_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.7.2/dexhub/address/avax_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     4654 2023-08-06 14:33:24.000000 dexhub-0.7.2/dexhub/address/dfk_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.7.2/dexhub/address/eth_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.7.2/dexhub/address/klay_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.7.2/dexhub/address/polygon_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      851 2023-08-06 19:48:50.000000 dexhub-0.7.2/dexhub/bridge.py
--rw-r--r--   0 czhong     (501) staff       (20)   142211 2023-05-03 12:57:14.000000 dexhub-0.7.2/dexhub/dex.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.581368 dexhub-0.7.2/dexhub/interface/
--rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.7.2/dexhub/interface/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.7.2/dexhub/interface/joe.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.582269 dexhub-0.7.2/dexhub/util/
--rw-r--r--   0 czhong     (501) staff       (20)       83 2023-05-02 19:50:16.000000 dexhub-0.7.2/dexhub/util/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    14052 2023-05-01 20:35:46.000000 dexhub-0.7.2/dexhub/util/helper.py
--rw-r--r--   0 czhong     (501) staff       (20)      471 2023-05-02 19:50:10.000000 dexhub-0.7.2/dexhub/util/joe_v2.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.578713 dexhub-0.7.2/dexhub.egg-info/
--rw-r--r--   0 czhong     (501) staff       (20)      478 2023-08-06 19:49:22.000000 dexhub-0.7.2/dexhub.egg-info/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      696 2023-08-06 19:49:22.000000 dexhub-0.7.2/dexhub.egg-info/SOURCES.txt
--rw-r--r--   0 czhong     (501) staff       (20)        1 2023-08-06 19:49:22.000000 dexhub-0.7.2/dexhub.egg-info/dependency_links.txt
--rw-r--r--   0 czhong     (501) staff       (20)        5 2023-08-06 19:49:22.000000 dexhub-0.7.2/dexhub.egg-info/requires.txt
--rw-r--r--   0 czhong     (501) staff       (20)        7 2023-08-06 19:49:22.000000 dexhub-0.7.2/dexhub.egg-info/top_level.txt
--rw-r--r--   0 czhong     (501) staff       (20)       38 2023-08-06 19:49:22.582675 dexhub-0.7.2/setup.cfg
--rw-r--r--   0 czhong     (501) staff       (20)      609 2023-08-06 19:49:17.000000 dexhub-0.7.2/setup.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 21:43:33.002479 dexhub-0.7.3/
+-rw-r--r--   0 czhong     (501) staff       (20)      478 2023-08-06 21:43:33.002331 dexhub-0.7.3/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.7.3/README.md
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 21:43:32.998582 dexhub-0.7.3/dexhub/
+-rw-r--r--   0 czhong     (501) staff       (20)     1325 2023-08-06 21:38:36.000000 dexhub-0.7.3/dexhub/__init__.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 21:43:33.000581 dexhub-0.7.3/dexhub/abi/
+-rw-r--r--   0 czhong     (501) staff       (20)      276 2023-08-06 21:38:25.000000 dexhub-0.7.3/dexhub/abi/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.7.3/dexhub/abi/arbitrum_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)   120303 2023-05-02 03:17:30.000000 dexhub-0.7.3/dexhub/abi/avax_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    28418 2023-08-06 10:36:23.000000 dexhub-0.7.3/dexhub/abi/dfk_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.7.3/dexhub/abi/eth_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    38503 2023-08-06 21:38:18.000000 dexhub-0.7.3/dexhub/abi/klay_abi.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 21:43:33.001471 dexhub-0.7.3/dexhub/address/
+-rw-r--r--   0 czhong     (501) staff       (20)      518 2023-08-06 21:30:39.000000 dexhub-0.7.3/dexhub/address/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.7.3/dexhub/address/arbitrum_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.7.3/dexhub/address/avax_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     4654 2023-08-06 14:33:24.000000 dexhub-0.7.3/dexhub/address/dfk_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.7.3/dexhub/address/eth_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1459 2023-08-06 21:27:25.000000 dexhub-0.7.3/dexhub/address/klay_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.7.3/dexhub/address/polygon_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1641 2023-08-06 21:43:07.000000 dexhub-0.7.3/dexhub/bridge.py
+-rw-r--r--   0 czhong     (501) staff       (20)   142211 2023-05-03 12:57:14.000000 dexhub-0.7.3/dexhub/dex.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 21:43:33.001713 dexhub-0.7.3/dexhub/interface/
+-rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.7.3/dexhub/interface/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.7.3/dexhub/interface/joe.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 21:43:33.002138 dexhub-0.7.3/dexhub/util/
+-rw-r--r--   0 czhong     (501) staff       (20)       83 2023-05-02 19:50:16.000000 dexhub-0.7.3/dexhub/util/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    14052 2023-05-01 20:35:46.000000 dexhub-0.7.3/dexhub/util/helper.py
+-rw-r--r--   0 czhong     (501) staff       (20)      471 2023-05-02 19:50:10.000000 dexhub-0.7.3/dexhub/util/joe_v2.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 21:43:32.999645 dexhub-0.7.3/dexhub.egg-info/
+-rw-r--r--   0 czhong     (501) staff       (20)      478 2023-08-06 21:43:32.000000 dexhub-0.7.3/dexhub.egg-info/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      696 2023-08-06 21:43:32.000000 dexhub-0.7.3/dexhub.egg-info/SOURCES.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        1 2023-08-06 21:43:32.000000 dexhub-0.7.3/dexhub.egg-info/dependency_links.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        5 2023-08-06 21:43:32.000000 dexhub-0.7.3/dexhub.egg-info/requires.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        7 2023-08-06 21:43:32.000000 dexhub-0.7.3/dexhub.egg-info/top_level.txt
+-rw-r--r--   0 czhong     (501) staff       (20)       38 2023-08-06 21:43:33.002526 dexhub-0.7.3/setup.cfg
+-rw-r--r--   0 czhong     (501) staff       (20)      609 2023-08-06 21:43:28.000000 dexhub-0.7.3/setup.py
```

### Comparing `dexhub-0.7.2/dexhub/__init__.py` & `dexhub-0.7.3/dexhub/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 )
 
 from dexhub.address.dfk_address import(
     CV,DfkTokens,AddressCV,AddressSynapseCV
 )
 
 from dexhub.address.klay_address import(
-    SD,KlayToken,AddressClaySwap,AddressSD
+    SD,KlayToken,AddressClaySwap,AddressSD,AddressSynapseKlay
 )
 
 from dexhub.address.polygon_address import(
     AddressUniswapV3Polygon,PolyTokens
 )
 
 from dexhub.address.arbitrum_address import(
@@ -48,15 +48,15 @@
 )
 
 from dexhub.abi.dfk_abi import(
     AbiCv,AbiSynapse
 )
 
 from dexhub.abi.klay_abi import(
-    AbiClaySwap,AbiSd
+    AbiClaySwap,AbiSd,AbiSynapseKlay
 )
 
 from dexhub.abi.eth_abi import(
     AbiUniswapV3
 )
 
 from dexhub.abi.avax_abi import(
```

### Comparing `dexhub-0.7.2/dexhub/abi/arbitrum_abi.py` & `dexhub-0.7.3/dexhub/abi/arbitrum_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub/abi/avax_abi.py` & `dexhub-0.7.3/dexhub/abi/avax_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub/abi/dfk_abi.py` & `dexhub-0.7.3/dexhub/abi/dfk_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub/abi/eth_abi.py` & `dexhub-0.7.3/dexhub/abi/eth_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub/address/arbitrum_address.py` & `dexhub-0.7.3/dexhub/address/arbitrum_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub/address/avax_address.py` & `dexhub-0.7.3/dexhub/address/avax_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub/address/dfk_address.py` & `dexhub-0.7.3/dexhub/address/dfk_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub/address/eth_address.py` & `dexhub-0.7.3/dexhub/address/eth_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub/address/klay_address.py` & `dexhub-0.7.3/dexhub/address/klay_address.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     sd_route=Web3.toChecksumAddress('0x9e987E5E9aB872598f601BE4aCC5ac23F484845E')
     sd_factory=Web3.toChecksumAddress('0x36fAE766e51f17F8218C735f58426E293498Db2B')
 
 class AddressSD:
     #dex
     sd_route=Web3.toChecksumAddress('0x9e987E5E9aB872598f601BE4aCC5ac23F484845E')
     sd_factory=Web3.toChecksumAddress('0x36fAE766e51f17F8218C735f58426E293498Db2B')
+
+class AddressSynapseKlay:
+    cv_l1_bridge_zap=Web3.toChecksumAddress('8671A0465844a15eb7230C5dd8d6032c26c655B7')
+    
 class AddressClaySwap:
     clay_swap_route=Web3.toChecksumAddress('0xEf71750C100f7918d6Ded239Ff1CF09E81dEA92D')
     clay_swap_factory=Web3.toChecksumAddress('0x3679c3766E70133Ee4A7eb76031E49d3d1f2B50c')
 
 class KlayToken:
     #erc20
     ousdt=Web3.toChecksumAddress('0xceE8FAF64bB97a73bb51E115Aa89C17FfA8dD167')
```

### Comparing `dexhub-0.7.2/dexhub/address/polygon_address.py` & `dexhub-0.7.3/dexhub/address/polygon_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub/bridge.py` & `dexhub-0.7.3/dexhub/bridge.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,34 @@
 
 class Synapse:
 
     chain_id_dfk=53935
     chain_id_klay=8217
 
 
-    def depositETH(_web3,_contract_address,_contract_abi,_to_chain_id,_amount,_public_key,_private_key):
+    def depositETH(_web3:Web3,_contract_address,_contract_abi,_to_chain_id,_amount,_public_key,_private_key):
         l1_bridge_zap_contract=_web3.eth.contract(address=_contract_address, abi=_contract_abi)
         nonce=_web3.eth.get_transaction_count(_public_key)
         deposit_ETH_function=l1_bridge_zap_contract.functions.depositETH(_public_key,_to_chain_id,_amount)
         tx_params={
             'from': _public_key,
             'value': _amount,
             'nonce': nonce,
             'type': '0x2'
         }
         transaction=deposit_ETH_function.buildTransaction(tx_params)
         signed_transaction=_web3.eth.account.sign_transaction(transaction, private_key=_private_key)
-        return _web3.eth.send_raw_transaction(signed_transaction.rawTransaction)
+        return _web3.toHex(_web3.eth.send_raw_transaction(signed_transaction.rawTransaction))
+    
+    def redeem(_web3:Web3,_contract_address,_contract_abi,_to_chain_id,_token,_amount,_public_key,_private_key):
+        bridge_zap_contract=_web3.eth.contract(address=_contract_address, abi=_contract_abi)
+        nonce=_web3.eth.get_transaction_count(_public_key)
+        redeem_function=bridge_zap_contract.functions.redeem(_public_key,_to_chain_id,_token,_amount)
+        tx_params={
+            'from': _public_key,
+            'value': 0,
+            'nonce': nonce,
+            'type': '0x2'
+        }
+        transaction=redeem_function.buildTransaction(tx_params)
+        signed_transaction=_web3.eth.account.sign_transaction(transaction, private_key=_private_key)
+        return _web3.toHex(_web3.eth.send_raw_transaction(signed_transaction.rawTransaction))
```

### Comparing `dexhub-0.7.2/dexhub/dex.py` & `dexhub-0.7.3/dexhub/dex.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub/interface/joe.py` & `dexhub-0.7.3/dexhub/interface/joe.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub/util/helper.py` & `dexhub-0.7.3/dexhub/util/helper.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/dexhub.egg-info/SOURCES.txt` & `dexhub-0.7.3/dexhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.2/setup.py` & `dexhub-0.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dexhub",
-    version="0.7.2",
+    version="0.7.3",
     author="elmtlab",
     author_email="elmtlab@outlook.com",
     description="dex connector",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elmtlab/aurum",
     packages=setuptools.find_packages(),
```

