# Comparing `tmp/deepbookpy-0.3.0.tar.gz` & `tmp/deepbookpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepbookpy-0.3.0.tar", max compression
+gzip compressed data, was "deepbookpy-0.3.1.tar", max compression
```

## Comparing `deepbookpy-0.3.0.tar` & `deepbookpy-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0    11356 2023-06-26 18:27:36.623393 deepbookpy-0.3.0/LICENSE
--rw-r--r--   0        0        0     1371 2023-07-24 20:30:43.377606 deepbookpy-0.3.0/README.md
--rw-r--r--   0        0        0       42 2023-07-24 13:51:37.948879 deepbookpy-0.3.0/deepbookpy/__init__.py
--rw-r--r--   0        0        0     6985 2023-07-24 23:39:11.925948 deepbookpy-0.3.0/deepbookpy/deepbook_query.py
--rw-r--r--   0        0        0    19172 2023-07-24 17:20:44.892315 deepbookpy-0.3.0/deepbookpy/deepbook_sdk.py
--rw-r--r--   0        0        0       70 2023-06-26 18:27:36.623393 deepbookpy-0.3.0/deepbookpy/utils/constant.py
--rw-r--r--   0        0        0     1195 2023-06-26 18:27:36.623393 deepbookpy-0.3.0/deepbookpy/utils/normalizer.py
--rw-r--r--   0        0        0       47 2023-07-24 23:39:11.925948 deepbookpy-0.3.0/deepbookpy/version.py
--rw-r--r--   0        0        0      448 2023-07-24 23:39:11.925948 deepbookpy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2042 2023-07-24 23:39:17.001875 deepbookpy-0.3.0/setup.py
--rw-r--r--   0        0        0     1723 2023-07-24 23:39:17.002214 deepbookpy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-26 18:27:36.623393 deepbookpy-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1371 2023-07-24 20:30:43.377606 deepbookpy-0.3.1/README.md
+-rw-r--r--   0        0        0       42 2023-07-24 13:51:37.948879 deepbookpy-0.3.1/deepbookpy/__init__.py
+-rw-r--r--   0        0        0     6665 2023-08-07 19:15:01.690619 deepbookpy-0.3.1/deepbookpy/deepbook_query.py
+-rw-r--r--   0        0        0    19697 2023-08-07 19:15:01.690619 deepbookpy-0.3.1/deepbookpy/deepbook_sdk.py
+-rw-r--r--   0        0        0      928 2023-08-07 19:15:01.690619 deepbookpy-0.3.1/deepbookpy/types/__init__.py
+-rw-r--r--   0        0        0      164 2023-08-07 19:15:01.690619 deepbookpy-0.3.1/deepbookpy/utils/constants.py
+-rw-r--r--   0        0        0      507 2023-08-07 19:15:01.690619 deepbookpy-0.3.1/deepbookpy/utils/helpers.py
+-rw-r--r--   0        0        0     1195 2023-08-07 17:18:30.696621 deepbookpy-0.3.1/deepbookpy/utils/normalizer.py
+-rw-r--r--   0        0        0       47 2023-08-07 19:15:01.690619 deepbookpy-0.3.1/deepbookpy/version.py
+-rw-r--r--   0        0        0      708 2023-08-07 19:15:01.690619 deepbookpy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2062 2023-08-07 19:15:18.428107 deepbookpy-0.3.1/setup.py
+-rw-r--r--   0        0        0     1723 2023-08-07 19:15:18.428415 deepbookpy-0.3.1/PKG-INFO
```

### Comparing `deepbookpy-0.3.0/LICENSE` & `deepbookpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepbookpy-0.3.0/README.md` & `deepbookpy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `deepbookpy-0.3.0/deepbookpy/deepbook_sdk.py` & `deepbookpy-0.3.1/deepbookpy/deepbook_sdk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,538 +1,560 @@
 """DeepBook Python SDK"""
 import math
 from typing import List
 
-from pysui.sui.sui_clients.transaction import SuiTransaction
+from pysui.sui.sui_txn.sync_transaction import SuiTransaction
 from pysui.sui.sui_clients.sync_client import SuiClient
 from pysui.sui.sui_types.address import SuiAddress
-from pysui.sui.sui_types.scalars import ObjectID, SuiU64, SuiBoolean
+from pysui.sui.sui_types.collections import SuiArray
+from pysui.sui.sui_types.scalars import ObjectID, SuiU64, SuiU8, SuiBoolean
 
 from deepbookpy.utils.normalizer import normalize_sui_object_id
+from deepbookpy.utils.constants import CLOB, CREATION_FEE
 
 
 class DeepBookSDK:
     """Write data to DeepBook package"""
 
     def __init__(self, client: SuiClient, package_id: str):
-        
-        self.client=client
+        self.client = client
         self.package_id = package_id
 
-    
     def create_pool(
-            self,
-            token_1: str,
-            token_2: str,
-            tick_size: int,
-            lot_size: int
+        self, token_1: str, token_2: str, tick_size: int, lot_size: int
     ) -> SuiTransaction:
         """
         Create pool for trading pair - 100 Sui fee
 
         :param token_1:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param token_2:
             Full coin type of quote asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::usdt::USDT"
 
         :param tick_size:
             Minimal Price Change Accuracy of this pool, eg: 10000000
 
         :param lot_size:
             Minimal Lot Change Accuracy of this pool, eg: 10000
         """
 
         txer = SuiTransaction(self.client)
 
-        splits: list = txer.split_coin(coin=txer.gas, amounts=[100_000_000_000])
+        splits: list = txer.split_coin(coin=txer.gas, amounts=[CREATION_FEE])
 
         txer.move_call(
-
-            target = f"{self.package_id}::clob::create_pool",
-
-            arguments = [SuiU64(str(tick_size)), SuiU64(str(lot_size)), splits],
-
-            type_arguments = [token_1, token_2]
-    )
+            target=f"{self.package_id}::{CLOB}::create_pool",
+            arguments=[SuiU64(str(tick_size)), SuiU64(str(lot_size)), splits],
+            type_arguments=[token_1, token_2],
+        )
         return txer
-    
 
     def create_account(self, current_address: SuiAddress) -> SuiTransaction:
         """
         Create and Transfer custodian account to user
-        
+
         :param current_address:
             current user address, eg: "0xbddc9d4961b46a130c2e1f38585bbc6fa8077ce54bcb206b26874ac08d607966"
         """
-        
+
         txer = SuiTransaction(self.client)
 
         cap: list = txer.move_call(
-            target = f"{self.package_id}::clob::create_account",
-
-            arguments = [],
-
-            type_arguments = []
+            target=f"{self.package_id}::{CLOB}::create_account",
+            arguments=[],
+            type_arguments=[],
         )
 
-        txer.transfer_objects(
-            transfers=[cap],
-            recipient=SuiAddress(current_address)
-        )
+        txer.transfer_objects(transfers=[cap], recipient=SuiAddress(current_address))
 
         return txer
-    
-    def deposit_base(self, token_1: str, token_2: str, pool_id: str, coin: str, account_cap: str) -> SuiTransaction:
+
+    def deposit_base(
+        self, token_1: str, token_2: str, pool_id: str, coin: str, account_cap: str
+    ) -> SuiTransaction:
         """
         Deposit base asset into custodian account
-        
+
         :param token_1:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param token_2:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param pool_id:
             Object id of pool, created after invoking create_pool(), eg: "0xcaee8e1c046b58e55196105f1436a2337dcaa0c340a7a8c8baf65e4afb8823a4"
 
         :param coin:
             Object id of coin to deposit, eg: "0x316467544c7e719384579ac5745c75be5984ca9f004d6c09fd7ca24e4d8a3d14"
-        
+
         :param account_cap:
             Object id of Account Capacity under user address, created after invoking create_account(), eg: "0x6f699fef193723277559c8f499ca3706121a65ac96d273151b8e52deb29135d3"
         """
-        
+
         txer = SuiTransaction(self.client)
 
         txer.move_call(
-            target = f"{self.package_id}::clob::deposit_base",
-
-            arguments = [ObjectID(pool_id), ObjectID(coin), ObjectID(account_cap)],
-
-            type_arguments = [token_1, token_2]
+            target=f"{self.package_id}::{CLOB}::deposit_base",
+            arguments=[ObjectID(pool_id), ObjectID(coin), ObjectID(account_cap)],
+            type_arguments=[token_1, token_2],
         )
 
         return txer
-    
-    def deposit_quote(self, token_1: str, token_2: str, pool_id: str, coin: str, account_cap: str) -> SuiTransaction:
+
+    def deposit_quote(
+        self, token_1: str, token_2: str, pool_id: str, coin: str, account_cap: str
+    ) -> SuiTransaction:
         """
         Deposit quote asset into custodian account
-        
+
         :param token_1:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param token_2:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param pool_id:
             Object id of pool, created after invoking create_pool(), eg: "0xcaee8e1c046b58e55196105f1436a2337dcaa0c340a7a8c8baf65e4afb8823a4"
 
         :param coin:
             Object id of coin to deposit, eg: "0x316467544c7e719384579ac5745c75be5984ca9f004d6c09fd7ca24e4d8a3d14"
-        
+
         :param account_cap:
             Object id of Account Capacity under user address, created after invoking create_account(), eg: "0x6f699fef193723277559c8f499ca3706121a65ac96d273151b8e52deb29135d3"
         """
-        
+
         txer = SuiTransaction(self.client)
 
         txer.move_call(
-            target = f"{self.package_id}::clob::deposit_quote",
-
-            arguments = [ObjectID(pool_id), ObjectID(coin), ObjectID(account_cap)],
-
-            type_arguments = [token_1, token_2]
+            target=f"{self.package_id}::{CLOB}::deposit_quote",
+            arguments=[ObjectID(pool_id), ObjectID(coin), ObjectID(account_cap)],
+            type_arguments=[token_1, token_2],
         )
 
         return txer
-    
-    
-    def withdraw_base(self, token_1: str, token_2: str, pool_id: str, quantity: int, current_address: SuiAddress, account_cap: str) -> SuiTransaction:
+
+    def withdraw_base(
+        self,
+        token_1: str,
+        token_2: str,
+        pool_id: str,
+        quantity: int,
+        current_address: SuiAddress,
+        account_cap: str,
+    ) -> SuiTransaction:
         """
         Withdraw base asset from custodian account
-        
+
         :param token_1:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param token_2:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param pool_id:
             Object id of pool, created after invoking create_pool, eg: "0xcaee8e1c046b58e55196105f1436a2337dcaa0c340a7a8c8baf65e4afb8823a4"
 
         :param quantity:
             Amount of base asset to withdraw, eg: 10000000
-        
+
         :param current_address:
             current user address, eg: "0xbddc9d4961b46a130c2e1f38585bbc6fa8077ce54bcb206b26874ac08d607966"
 
         :param account_cap:
             Object id of Account Capacity under user address, created after invoking create_account(), eg: "0x6f699fef193723277559c8f499ca3706121a65ac96d273151b8e52deb29135d3"
         """
-        
+
         txer = SuiTransaction(self.client)
 
         withdraw = txer.move_call(
-            target = f"{self.package_id}::clob::withdraw_base",
-
-            arguments = [ObjectID(pool_id), SuiU64(quantity), ObjectID(account_cap)],
-
-            type_arguments = [token_1, token_2]
+            target=f"{self.package_id}::{CLOB}::withdraw_base",
+            arguments=[ObjectID(pool_id), SuiU64(quantity), ObjectID(account_cap)],
+            type_arguments=[token_1, token_2],
         )
 
         txer.transfer_objects(
-            transfers=[withdraw],
-            recipient=SuiAddress(current_address)
+            transfers=[withdraw], recipient=SuiAddress(current_address)
         )
 
         return txer
-    
-    def withdraw_quote(self, token_1: str, token_2: str, pool_id: str, quantity: int, current_address: SuiAddress, account_cap: str) -> SuiTransaction:
+
+    def withdraw_quote(
+        self,
+        token_1: str,
+        token_2: str,
+        pool_id: str,
+        quantity: int,
+        current_address: SuiAddress,
+        account_cap: str,
+    ) -> SuiTransaction:
         """
         Withdraw quote asset from custodian account
-        
+
         :param token_1:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param token_2:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param pool_id:
             Object id of pool, created after invoking create_pool, eg: "0xcaee8e1c046b58e55196105f1436a2337dcaa0c340a7a8c8baf65e4afb8823a4"
 
         :param quantity:
             Amount of base asset to withdraw, eg: 10000000
-        
+
         :param current_address:
             current user address, eg: "0xbddc9d4961b46a130c2e1f38585bbc6fa8077ce54bcb206b26874ac08d607966"
 
         :param account_cap:
             Object id of Account Capacity under user address, created after invoking create_account(), eg: "0x6f699fef193723277559c8f499ca3706121a65ac96d273151b8e52deb29135d3"
         """
-        
+
         txer = SuiTransaction(self.client)
 
         withdraw = txer.move_call(
-            target = f"{self.package_id}::clob::withdraw_quote",
-
-            arguments = [ObjectID(pool_id), SuiU64(quantity), ObjectID(account_cap)],
-
-            type_arguments = [token_1, token_2]
+            target=f"{self.package_id}::{CLOB}::withdraw_quote",
+            arguments=[ObjectID(pool_id), SuiU64(quantity), ObjectID(account_cap)],
+            type_arguments=[token_1, token_2],
         )
 
         txer.transfer_objects(
-            transfers=[withdraw],
-            recipient=SuiAddress(current_address)
+            transfers=[withdraw], recipient=SuiAddress(current_address)
         )
 
         return txer
-    
 
-    def swap_exact_quote_for_base(self, token_1: str, token_2: str, pool_id: str, token_object_in: str, amount_in: int, current_address: SuiAddress) -> SuiTransaction:
+    def swap_exact_quote_for_base(
+        self,
+        token_1: str,
+        token_2: str,
+        pool_id: str,
+        token_object_in: str,
+        amount_in: int,
+        current_address: SuiAddress,
+        client_order_id: str,
+    ) -> SuiTransaction:
         """
         Swap exact quote for base
-        
+
         :param token_1:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param token_2:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param pool_id:
             Object id of pool, created after invoking create_pool, eg: "0xcaee8e1c046b58e55196105f1436a2337dcaa0c340a7a8c8baf65e4afb8823a4"
 
         :param token_object_in:
             Object id of the token to swap: eg: "0x6e566fec4c388eeb78a7dab832c9f0212eb2ac7e8699500e203def5b41b9c70d"
-        
+
         :param amount_in:
             Amount of token to buy or sell, eg: 10000000
 
         :param current_address:
             current user address, eg: "0xbddc9d4961b46a130c2e1f38585bbc6fa8077ce54bcb206b26874ac08d607966"
         """
-        
+
         txer = SuiTransaction(self.client)
 
         [base_coin_ret, quote_coin_ret, _amount] = txer.move_call(
-            target = f"{self.package_id}::clob::swap_exact_quote_for_base",
-
-            arguments = [ObjectID(pool_id), SuiU64(amount_in), ObjectID(normalize_sui_object_id('0x6')), ObjectID(token_object_in)],
-
-            type_arguments = [token_1, token_2]
+            target=f"{self.package_id}::{CLOB}::swap_exact_quote_for_base",
+            arguments=[
+                ObjectID(pool_id),
+                SuiU64(client_order_id),
+                SuiU64(amount_in),
+                ObjectID(normalize_sui_object_id("0x6")),
+                ObjectID(token_object_in),
+            ],
+            type_arguments=[token_1, token_2],
         )
 
         txer.transfer_objects(
-            transfers=[base_coin_ret],
-            recipient=SuiAddress(current_address)
+            transfers=[base_coin_ret], recipient=SuiAddress(current_address)
         )
 
         txer.transfer_objects(
-            transfers=[quote_coin_ret],
-            recipient=SuiAddress(current_address)
+            transfers=[quote_coin_ret], recipient=SuiAddress(current_address)
         )
 
         return txer
-    
-    def swap_exact_base_for_quote(self, token_1: str, token_2: str, pool_id: str, treasury: str, token_object_in: str, amount_in: int, current_address: SuiAddress) -> SuiTransaction:
+
+    def swap_exact_base_for_quote(
+        self,
+        token_1: str,
+        token_2: str,
+        pool_id: str,
+        token_object_in: str,
+        amount_in: int,
+        current_address: SuiAddress,
+        client_order_id: str,
+    ) -> SuiTransaction:
         """
         Swap exact base for quote
-        
+
         :param token_1:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param token_2:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param pool_id:
             Object id of pool, created after invoking create_pool, eg: "0xcaee8e1c046b58e55196105f1436a2337dcaa0c340a7a8c8baf65e4afb8823a4"
 
-        :param treasury:
-            treasury of the quote coin, in the selling case, we will mint a zero quote coin to receive the quote coin from the pool. eg: "0x0a11d301013759e79cb5f89a8bb29c3f9a9bb5be6dec2ddba48ea4b39abc5b5a"
-
         :param token_object_in:
             Object id of the token to swap: eg: "0x6e566fec4c388eeb78a7dab832c9f0212eb2ac7e8699500e203def5b41b9c70d"
-        
+
         :param amount_in:
             Amount of token to buy or sell, eg: 10000000
 
         :param current_address:
             current user address, eg: "0xbddc9d4961b46a130c2e1f38585bbc6fa8077ce54bcb206b26874ac08d607966"
         """
-        
+
         txer = SuiTransaction(self.client)
 
         [base_coin_ret, quote_coin_ret, _amount] = txer.move_call(
-            target = f"{self.package_id}::clob::swap_exact_base_for_quote",
-
-            arguments = [
+            target=f"{self.package_id}::{CLOB}::swap_exact_base_for_quote",
+            arguments=[
                 ObjectID(pool_id),
-                SuiU64(amount_in),
+                SuiU64(client_order_id),
+                SuiU64(str(amount_in)),
                 ObjectID(token_object_in),
-                # mint
-                _mint(token_2, 0, treasury, txer),
-                ObjectID(normalize_sui_object_id('0x6')),
-                ],
+                txer.move_call(
+                    type_arguments=[token_2],  # quoteasset
+                    target="0x2::coin::zero",
+                    arguments=[],
+                ),
+                ObjectID(normalize_sui_object_id("0x6")),
+            ],
+            type_arguments=[token_1, token_2],
+        )
 
-            type_arguments = [token_1, token_2]
+        txer.transfer_objects(
+            transfers=[base_coin_ret], recipient=SuiAddress(current_address)
         )
 
         txer.transfer_objects(
-            transfers=[base_coin_ret],
-            recipient=SuiAddress(current_address)
+            transfers=[quote_coin_ret], recipient=SuiAddress(current_address)
+        )
+
+        return txer
+
+    def place_market_order(
+        self,
+        token_1: str,
+        token_2: str,
+        client_order_id: str,
+        pool_id: str,
+        quantity: int,
+        is_bid: bool,
+        base_coin: str,
+        quote_coin: str,
+        current_address: str,
+        account_cap: str,
+    ):
+        txer = SuiTransaction(self.client)
+        [base_coin_ret, quote_coin_ret] = txer.move_call(
+            target=f"{self.package_id}::{CLOB}::place_market_order",
+            arguments=[
+                ObjectID(pool_id),
+                ObjectID(account_cap),
+                SuiU64(client_order_id),
+                SuiU64(quantity),
+                SuiBoolean(is_bid),
+                ObjectID(base_coin),
+                ObjectID(quote_coin),
+                ObjectID(normalize_sui_object_id("0x6")),
+            ],
+            type_arguments=[token_1, token_2],
         )
 
+        print(base_coin_ret)
+        print("----")
+        print(quote_coin_ret)
+
         txer.transfer_objects(
-            transfers=[quote_coin_ret],
-            recipient=SuiAddress(current_address)
+            transfers=[base_coin_ret], recipient=SuiAddress(current_address)
         )
 
+        txer.transfer_objects(
+            transfers=[quote_coin_ret], recipient=SuiAddress(current_address)
+        )
         return txer
-    
 
     def place_limit_order(
-            self,
-            token_1: str,
-            token_2: str,
-            pool_id: str,
-            price: int,
-            quantity: int,
-            is_bid: bool,
-            expire_timestamp: int,
-            restriction: int,
-            account_cap: str
-        ) -> SuiTransaction:
+        self,
+        token_1: str,
+        token_2: str,
+        client_order_id: str,
+        pool_id: str,
+        price: int,
+        quantity: int,
+        self_matching_prevention: bool,
+        is_bid: bool,
+        expire_timestamp: int,
+        restriction: int,
+        account_cap: str,
+    ) -> SuiTransaction:
         """
         Place a limit order
-        
+
         :param token_1:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
         :param token_2:
             Full coin type of the base asset, eg: "0x3d0d0ce17dcd3b40c2d839d96ce66871ffb40e1154a8dd99af72292b3d10d7fc::wbtc::WBTC"
-        
+
+        :param client_order_id:
+            client side defined order number, eg "1", "2" etc
+
         :param pool_id:
             Object id of pool, created after invoking create_pool, eg: "0xcaee8e1c046b58e55196105f1436a2337dcaa0c340a7a8c8baf65e4afb8823a4"
 
         :param price:
             price of the limit order, eg: 180000000
-        
+
+        :param self_matching_prevention:
+            True for self matching prevention, false for not, eg: true
+
         :param quantity:
             Quantity of the limit order in BASE ASSET, eg: 100000000
 
         :param is_bid:
             True for buying base with quote, false for selling base for quote
-        
+
         :param expire_timestamp:
-            Expire timestamp of the limit order in ms, eg: 1620000000000
-        
+            Expire timestamp of the limit order in ms, eg: 1620000000000.
+            Alternative you can call deepbookpy.deepbook.helpers.order_expiration() for 24 hours timestamp
+
         :param restriction:
             Restrictions on limit orders, eg: 0
 
         :param account_cap:
             Object id of Account Capacity under user address, created after invoking create_account(), eg: "0x6f699fef193723277559c8f499ca3706121a65ac96d273151b8e52deb29135d3"
         """
-        
+
         txer = SuiTransaction(self.client)
 
         args = [
-                ObjectID(str(pool_id)),
-                SuiU64(math.floor(price * 1000000000)),
-                SuiU64(quantity),
-                SuiBoolean(is_bid),
-                SuiU64(expire_timestamp),
-                SuiU64(restriction),
-                ObjectID(normalize_sui_object_id('0x6')),
-                ObjectID(account_cap)
-            ]
+            ObjectID(pool_id),
+            SuiU64(client_order_id),
+            SuiU64(math.floor(price * 1000000000)),
+            SuiU64(quantity),
+            SuiU8(self_matching_prevention),
+            SuiBoolean(is_bid),
+            SuiU64(expire_timestamp),
+            SuiU8(restriction),
+            ObjectID(normalize_sui_object_id("0x6")),
+            ObjectID(account_cap),
+        ]
         txer.move_call(
-            target = f"{self.package_id}::clob::place_limit_order",
-
-            arguments = args,
-
-            type_arguments = [token_1, token_2]
+            type_arguments=[token_1, token_2],
+            target=f"{self.package_id}::{CLOB}::place_limit_order",
+            arguments=args,
         )
 
         return txer
 
     def cancel_order(
-            self,
-            token_1: str,
-            token_2: str,
-            pool_id: str,
-            order_id: str,
-            account_cap: str,
-            ) -> SuiTransaction:
+        self,
+        token_1: str,
+        token_2: str,
+        pool_id: str,
+        order_id: int,
+        account_cap: str,
+    ) -> SuiTransaction:
         """
         Cancel a limit order placed onto the CLOB
 
         :param token_1:
             Full coin type of the base asset, eg: 0x5378a0e7495723f7d942366a125a6556cf56f573fa2bb7171b554a2986c4229a::wbtc::WBTC
-        
+
         :param token_2:
            Full coin type of quote asset, eg: 0x5378a0e7495723f7d942366a125a6556cf56f573fa2bb7171b554a2986c4229a::weth::WETH
 
         :param pool_id:
             Object id of pool, created after invoking create_pool(), eg: 0xcaee8e1c046b58e55196105f1436a2337dcaa0c340a7a8c8baf65e4afb8823a4
-        
+
         :param order_id:
             Order id of a limit order, you can find them through function list_open_orders() eg: "0"
 
         :param account_cap:
             Object id of Account Capacity under user address, created after invoking create_account()
         """
 
         txer = SuiTransaction(self.client)
 
         txer.move_call(
-            target = f"{self.package_id}::clob::cancel_order",
-
-            arguments = [ObjectID(pool_id), ObjectID(order_id), ObjectID(account_cap)],
-
-            type_arguments = [token_1, token_2]
+            target=f"{self.package_id}::{CLOB}::cancel_order",
+            arguments=[ObjectID(pool_id), SuiU64(order_id), ObjectID(account_cap)],
+            type_arguments=[token_1, token_2],
         )
 
         return txer
-    
+
     def cancel_all_orders(
-            self,
-            token_1: str,
-            token_2: str,
-            pool_id: str,
-            account_cap: str
+        self, token_1: str, token_2: str, pool_id: str, account_cap: str
     ) -> SuiTransaction:
-    
         """
         Cancel all limit orders under a certain account capacity
 
         :param token_1:
             Full coin type of the base asset, eg: 0x5378a0e7495723f7d942366a125a6556cf56f573fa2bb7171b554a2986c4229a::wbtc::WBTC
-        
+
         :param token_2:
            Full coin type of quote asset, eg: 0x5378a0e7495723f7d942366a125a6556cf56f573fa2bb7171b554a2986c4229a::weth::WETH
 
         :param pool_id:
             Object id of pool, created after invoking create_pool(), eg: 0xcaee8e1c046b58e55196105f1436a2337dcaa0c340a7a8c8baf65e4afb8823a4
 
         :param account_cap:
             Object id of Account Capacity under user address, created after invoking create_account()
         """
 
         txer = SuiTransaction(self.client)
 
         txer.move_call(
-            target = f"{self.package_id}::clob::cancel_all_orders",
-
-            arguments = [ObjectID(pool_id), ObjectID(account_cap)],
-
-            type_arguments = [token_1, token_2]
+            target=f"{self.package_id}::{CLOB}::cancel_all_orders",
+            arguments=[ObjectID(pool_id), ObjectID(account_cap)],
+            type_arguments=[token_1, token_2],
         )
 
         return txer
-    
+
     def batch_cancel_order(
-            self,
-            token_1: str,
-            token_2: str,
-            pool_id: str,
-            order_ids: List[str],
-            account_cap: str
+        self,
+        token_1: str,
+        token_2: str,
+        pool_id: str,
+        order_ids: List[str],
+        account_cap: str,
     ) -> SuiTransaction:
-    
         """
         Cancel multiple limit orders to save gas costs.
 
         :param token_1:
             Full coin type of the base asset, eg: 0x5378a0e7495723f7d942366a125a6556cf56f573fa2bb7171b554a2986c4229a::wbtc::WBTC
-        
+
         :param token_2:
            Full coin type of quote asset, eg: 0x5378a0e7495723f7d942366a125a6556cf56f573fa2bb7171b554a2986c4229a::weth::WETH
 
         :param pool_id::
             Object id of pool, created after invoking create_pool(), eg: 0xcaee8e1c046b58e55196105f1436a2337dcaa0c340a7a8c8baf65e4afb8823a4
 
         :param order_ids:
-            orderId of a limit order, you can find them through the function list_open_orders, for example: ["0", "1"]
+            orderId of a limit order, you can find them through the list_open_orders() function, for example: ["0", "1"]
 
         :param account_cap:
             Object id of Account Capacity under user address, created after invoking create_account()
         """
 
         txer = SuiTransaction(self.client)
 
         txer.move_call(
-            target = f"{self.package_id}::clob::batch_cancel_order",
-
-            arguments = [ObjectID(pool_id), ObjectID(order_ids), ObjectID(account_cap)],
-
-            type_arguments = [token_1, token_2]
+            target=f"{self.package_id}::{CLOB}::batch_cancel_order",
+            arguments=[ObjectID(pool_id), SuiArray(order_ids), ObjectID(account_cap)],
+            type_arguments=[token_1, token_2],
         )
 
         return txer
-    
-
-    def _mint(self, token: str, quantity: int, treasury: str, txer: SuiTransaction):
-        """
-        
-        :param token:
-            the token type you want to mint, eg: "0x5378a0e7495723f7d942366a125a6556cf56f573fa2bb7171b554a2986c4229a::wbtc::WBTC"
-        
-        :param quantity:
-            the quantity you want to mint, eg: 2000000000
-
-        :param treasury:
-            the treasury object id, eg: "0x765c7040f06527df0f76d5a38ceaae67c70311c90c266acf15e39f17e0e4ed61"
-        
-        :param txer:
-            SuiTransaction instance
-        
-        """
-        return txer.move_call(
-            target = "0x2::coin::mint",
-
-            arguments = [
-                ObjectID(str(treasury)),
-                ObjectID(str(quantity))
-                ],
-
-            type_arguments = [token]
-        )
```

### Comparing `deepbookpy-0.3.0/deepbookpy/utils/normalizer.py` & `deepbookpy-0.3.1/deepbookpy/utils/normalizer.py`

 * *Files identical despite different names*

### Comparing `deepbookpy-0.3.0/setup.py` & `deepbookpy-0.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['deepbookpy', 'deepbookpy.utils']
+['deepbookpy', 'deepbookpy.types', 'deepbookpy.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pysui>=0.29.0,<0.30.0']
+['pysui>=0.32.0,<0.33.0']
 
 setup_kwargs = {
     'name': 'deepbookpy',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Sui Deepbook Python SDK',
     'long_description': '# Community Sui DeepBook Python SDK\nPython DeepBook Client SDK for Sui blockchain - built by community with [pysui](https://github.com/FrankC01/pysui/)\n\n> **_This package is still in active development. Use at your own risk._**\n\n## Python Sui DeepBook SDK Parameters\n```py\nfrom deepbookpy.utils.normalizer import normalize_sui_object_id\n\nDEEPBOOK_PACKAGE_ID = "https://explorer.sui.io/object/0x000000000000000000000000000000000000000000000000000000000000dee9"\n\nCLOCK = normalize_sui_object_id("0x6")\n\n```\n## Install deepbookpy\n`pip install deepbookpy`\n\n`poetry add deepbookpy`\n\n## Documentation\nCheck out latest deepbookpy [documentation](https://deepbookpy.readthedocs.io/en/latest/) release \n\n## Official DeepBook Resources\n\n[Official Deepbook Sui Website](https://sui-deepbook.com/)\n\n[Official Deepbook Sui Documentation](https://docs.sui-deepbook.com/)\n\n## DeepBook Packages\n\n[DeepBook Mainnet Package](https://suiexplorer.com/object/0x000000000000000000000000000000000000000000000000000000000000dee9)\n\n[DeepBook Testnet Package](https://suiexplorer.com/object/0x000000000000000000000000000000000000000000000000000000000000dee9?network=testnet)\n\n[DeepBook Devnet Package](https://suiexplorer.com/object/0x000000000000000000000000000000000000000000000000000000000000dee9?network=devnet)\n\n## Ask A Question\n\nJoin Our Coummunity [discord](https://discord.gg/CUTen9zu5h)\n',
     'author': 'andreidev1',
     'author_email': 'andreid.dev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `deepbookpy-0.3.0/PKG-INFO` & `deepbookpy-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: deepbookpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Sui Deepbook Python SDK
 Author: andreidev1
 Author-email: andreid.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: pysui (>=0.29.0,<0.30.0)
+Requires-Dist: pysui (>=0.32.0,<0.33.0)
 Description-Content-Type: text/markdown
 
 # Community Sui DeepBook Python SDK
 Python DeepBook Client SDK for Sui blockchain - built by community with [pysui](https://github.com/FrankC01/pysui/)
 
 > **_This package is still in active development. Use at your own risk._**
```

