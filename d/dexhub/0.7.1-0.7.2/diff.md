# Comparing `tmp/dexhub-0.7.1.tar.gz` & `tmp/dexhub-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexhub-0.7.1.tar", last modified: Sun Aug  6 14:59:45 2023, max compression
+gzip compressed data, was "dexhub-0.7.2.tar", last modified: Sun Aug  6 19:49:22 2023, max compression
```

## Comparing `dexhub-0.7.1.tar` & `dexhub-0.7.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.354229 dexhub-0.7.1/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-08-06 14:59:45.354097 dexhub-0.7.1/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.7.1/README.md
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.350906 dexhub-0.7.1/dexhub/
--rw-r--r--   0 czhong     (501) staff       (20)     1291 2023-08-06 14:59:24.000000 dexhub-0.7.1/dexhub/__init__.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.352462 dexhub-0.7.1/dexhub/abi/
--rw-r--r--   0 czhong     (501) staff       (20)      261 2023-08-06 10:36:45.000000 dexhub-0.7.1/dexhub/abi/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.7.1/dexhub/abi/arbitrum_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)   120303 2023-05-02 03:17:30.000000 dexhub-0.7.1/dexhub/abi/avax_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    28418 2023-08-06 10:36:23.000000 dexhub-0.7.1/dexhub/abi/dfk_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.7.1/dexhub/abi/eth_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.7.1/dexhub/abi/klay_abi.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.353282 dexhub-0.7.1/dexhub/address/
--rw-r--r--   0 czhong     (501) staff       (20)      499 2023-08-06 14:33:28.000000 dexhub-0.7.1/dexhub/address/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.7.1/dexhub/address/arbitrum_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.7.1/dexhub/address/avax_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     4654 2023-08-06 14:33:24.000000 dexhub-0.7.1/dexhub/address/dfk_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.7.1/dexhub/address/eth_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.7.1/dexhub/address/klay_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.7.1/dexhub/address/polygon_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      886 2023-08-06 14:26:53.000000 dexhub-0.7.1/dexhub/bridge.py
--rw-r--r--   0 czhong     (501) staff       (20)   142211 2023-05-03 12:57:14.000000 dexhub-0.7.1/dexhub/dex.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.353510 dexhub-0.7.1/dexhub/interface/
--rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.7.1/dexhub/interface/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.7.1/dexhub/interface/joe.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.353923 dexhub-0.7.1/dexhub/util/
--rw-r--r--   0 czhong     (501) staff       (20)       83 2023-05-02 19:50:16.000000 dexhub-0.7.1/dexhub/util/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    14052 2023-05-01 20:35:46.000000 dexhub-0.7.1/dexhub/util/helper.py
--rw-r--r--   0 czhong     (501) staff       (20)      471 2023-05-02 19:50:10.000000 dexhub-0.7.1/dexhub/util/joe_v2.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.351577 dexhub-0.7.1/dexhub.egg-info/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-08-06 14:59:45.000000 dexhub-0.7.1/dexhub.egg-info/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      696 2023-08-06 14:59:45.000000 dexhub-0.7.1/dexhub.egg-info/SOURCES.txt
--rw-r--r--   0 czhong     (501) staff       (20)        1 2023-08-06 14:59:45.000000 dexhub-0.7.1/dexhub.egg-info/dependency_links.txt
--rw-r--r--   0 czhong     (501) staff       (20)        5 2023-08-06 14:59:45.000000 dexhub-0.7.1/dexhub.egg-info/requires.txt
--rw-r--r--   0 czhong     (501) staff       (20)        7 2023-08-06 14:59:45.000000 dexhub-0.7.1/dexhub.egg-info/top_level.txt
--rw-r--r--   0 czhong     (501) staff       (20)       38 2023-08-06 14:59:45.354273 dexhub-0.7.1/setup.cfg
--rw-r--r--   0 czhong     (501) staff       (20)      609 2023-08-06 14:59:38.000000 dexhub-0.7.1/setup.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.582635 dexhub-0.7.2/
+-rw-r--r--   0 czhong     (501) staff       (20)      478 2023-08-06 19:49:22.582487 dexhub-0.7.2/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.7.2/README.md
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.577772 dexhub-0.7.2/dexhub/
+-rw-r--r--   0 czhong     (501) staff       (20)     1291 2023-08-06 14:59:24.000000 dexhub-0.7.2/dexhub/__init__.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.579777 dexhub-0.7.2/dexhub/abi/
+-rw-r--r--   0 czhong     (501) staff       (20)      261 2023-08-06 10:36:45.000000 dexhub-0.7.2/dexhub/abi/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.7.2/dexhub/abi/arbitrum_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)   120303 2023-05-02 03:17:30.000000 dexhub-0.7.2/dexhub/abi/avax_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    28418 2023-08-06 10:36:23.000000 dexhub-0.7.2/dexhub/abi/dfk_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.7.2/dexhub/abi/eth_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.7.2/dexhub/abi/klay_abi.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.581046 dexhub-0.7.2/dexhub/address/
+-rw-r--r--   0 czhong     (501) staff       (20)      499 2023-08-06 14:33:28.000000 dexhub-0.7.2/dexhub/address/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.7.2/dexhub/address/arbitrum_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.7.2/dexhub/address/avax_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     4654 2023-08-06 14:33:24.000000 dexhub-0.7.2/dexhub/address/dfk_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.7.2/dexhub/address/eth_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.7.2/dexhub/address/klay_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.7.2/dexhub/address/polygon_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      851 2023-08-06 19:48:50.000000 dexhub-0.7.2/dexhub/bridge.py
+-rw-r--r--   0 czhong     (501) staff       (20)   142211 2023-05-03 12:57:14.000000 dexhub-0.7.2/dexhub/dex.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.581368 dexhub-0.7.2/dexhub/interface/
+-rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.7.2/dexhub/interface/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.7.2/dexhub/interface/joe.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.582269 dexhub-0.7.2/dexhub/util/
+-rw-r--r--   0 czhong     (501) staff       (20)       83 2023-05-02 19:50:16.000000 dexhub-0.7.2/dexhub/util/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    14052 2023-05-01 20:35:46.000000 dexhub-0.7.2/dexhub/util/helper.py
+-rw-r--r--   0 czhong     (501) staff       (20)      471 2023-05-02 19:50:10.000000 dexhub-0.7.2/dexhub/util/joe_v2.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 19:49:22.578713 dexhub-0.7.2/dexhub.egg-info/
+-rw-r--r--   0 czhong     (501) staff       (20)      478 2023-08-06 19:49:22.000000 dexhub-0.7.2/dexhub.egg-info/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      696 2023-08-06 19:49:22.000000 dexhub-0.7.2/dexhub.egg-info/SOURCES.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        1 2023-08-06 19:49:22.000000 dexhub-0.7.2/dexhub.egg-info/dependency_links.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        5 2023-08-06 19:49:22.000000 dexhub-0.7.2/dexhub.egg-info/requires.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        7 2023-08-06 19:49:22.000000 dexhub-0.7.2/dexhub.egg-info/top_level.txt
+-rw-r--r--   0 czhong     (501) staff       (20)       38 2023-08-06 19:49:22.582675 dexhub-0.7.2/setup.cfg
+-rw-r--r--   0 czhong     (501) staff       (20)      609 2023-08-06 19:49:17.000000 dexhub-0.7.2/setup.py
```

### Comparing `dexhub-0.7.1/dexhub/__init__.py` & `dexhub-0.7.2/dexhub/__init__.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/abi/arbitrum_abi.py` & `dexhub-0.7.2/dexhub/abi/arbitrum_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/abi/avax_abi.py` & `dexhub-0.7.2/dexhub/abi/avax_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/abi/dfk_abi.py` & `dexhub-0.7.2/dexhub/abi/dfk_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/abi/eth_abi.py` & `dexhub-0.7.2/dexhub/abi/eth_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/abi/klay_abi.py` & `dexhub-0.7.2/dexhub/abi/klay_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/address/arbitrum_address.py` & `dexhub-0.7.2/dexhub/address/arbitrum_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/address/avax_address.py` & `dexhub-0.7.2/dexhub/address/avax_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/address/dfk_address.py` & `dexhub-0.7.2/dexhub/address/dfk_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/address/eth_address.py` & `dexhub-0.7.2/dexhub/address/eth_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/address/klay_address.py` & `dexhub-0.7.2/dexhub/address/klay_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/address/polygon_address.py` & `dexhub-0.7.2/dexhub/address/polygon_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/bridge.py` & `dexhub-0.7.2/dexhub/bridge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from web3 import Web3
 
 class Synapse:
 
     chain_id_dfk=53935
     chain_id_klay=8217
 
-    
-    def depositETH(_web3:Web3,_contract_address:str,_contract_abi:str,_to_chain_id:int,_amount:int,_public_key:str,_private_key:str):
+
+    def depositETH(_web3,_contract_address,_contract_abi,_to_chain_id,_amount,_public_key,_private_key):
         l1_bridge_zap_contract=_web3.eth.contract(address=_contract_address, abi=_contract_abi)
         nonce=_web3.eth.get_transaction_count(_public_key)
-        deposit_ETH_function=l1_bridge_zap_contract.functions.depositETH(_public_key,_to_chain_id,_amount)        
+        deposit_ETH_function=l1_bridge_zap_contract.functions.depositETH(_public_key,_to_chain_id,_amount)
         tx_params={
             'from': _public_key,
-            'value': 0,
+            'value': _amount,
             'nonce': nonce,
             'type': '0x2'
         }
         transaction=deposit_ETH_function.buildTransaction(tx_params)
         signed_transaction=_web3.eth.account.sign_transaction(transaction, private_key=_private_key)
         return _web3.eth.send_raw_transaction(signed_transaction.rawTransaction)
```

### Comparing `dexhub-0.7.1/dexhub/dex.py` & `dexhub-0.7.2/dexhub/dex.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/interface/joe.py` & `dexhub-0.7.2/dexhub/interface/joe.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub/util/helper.py` & `dexhub-0.7.2/dexhub/util/helper.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/dexhub.egg-info/SOURCES.txt` & `dexhub-0.7.2/dexhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.1/setup.py` & `dexhub-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dexhub",
-    version="0.7.1",
+    version="0.7.2",
     author="elmtlab",
     author_email="elmtlab@outlook.com",
     description="dex connector",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elmtlab/aurum",
     packages=setuptools.find_packages(),
```

