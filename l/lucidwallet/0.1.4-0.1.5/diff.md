# Comparing `tmp/lucidwallet-0.1.4.tar.gz` & `tmp/lucidwallet-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucidwallet-0.1.4.tar", max compression
+gzip compressed data, was "lucidwallet-0.1.5.tar", max compression
```

## Comparing `lucidwallet-0.1.4.tar` & `lucidwallet-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1488 2023-08-06 19:16:17.699415 lucidwallet-0.1.4/LICENSE
--rw-r--r--   0        0        0       75 2023-08-06 20:21:50.851629 lucidwallet-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-17 07:44:41.990980 lucidwallet-0.1.4/lucidwallet/__init__.py
--rw-r--r--   0        0        0     9730 2023-08-07 08:20:30.535722 lucidwallet-0.1.4/lucidwallet/app.css
--rw-r--r--   0        0        0       71 2023-08-06 19:22:05.917312 lucidwallet-0.1.4/lucidwallet/datastore/__init__.py
--rw-r--r--   0        0        0    13506 2023-08-06 20:12:07.119724 lucidwallet-0.1.4/lucidwallet/datastore/fluxwallet_datastore.py
--rw-r--r--   0        0        0     3853 2023-08-07 08:49:11.804229 lucidwallet-0.1.4/lucidwallet/entrypoint.py
--rw-r--r--   0        0        0      384 2023-08-04 11:22:47.433226 lucidwallet-0.1.4/lucidwallet/events/__init__.py
--rw-r--r--   0        0        0     2109 2023-08-06 19:22:05.926687 lucidwallet-0.1.4/lucidwallet/helpers/__init__.py
--rw-r--r--   0        0        0      948 2023-08-06 20:14:19.531008 lucidwallet-0.1.4/lucidwallet/screens/__init__.py
--rw-r--r--   0        0        0     5812 2023-08-06 20:02:34.318411 lucidwallet-0.1.4/lucidwallet/screens/address_book.py
--rw-r--r--   0        0        0     1547 2023-08-06 15:40:53.198703 lucidwallet-0.1.4/lucidwallet/screens/address_book_overlay.py
--rw-r--r--   0        0        0     4045 2023-08-06 20:02:21.438840 lucidwallet-0.1.4/lucidwallet/screens/create_wallet.py
--rw-r--r--   0        0        0     6294 2023-08-06 20:02:56.973871 lucidwallet-0.1.4/lucidwallet/screens/get_encryption_password.py
--rw-r--r--   0        0        0    14950 2023-08-06 20:03:15.152907 lucidwallet-0.1.4/lucidwallet/screens/import_from_mnemonic.py
--rw-r--r--   0        0        0     4480 2023-08-06 19:22:05.902145 lucidwallet-0.1.4/lucidwallet/screens/import_key_to_wallet.py
--rw-r--r--   0        0        0     1635 2023-08-06 19:22:05.870564 lucidwallet-0.1.4/lucidwallet/screens/keychain_overlay.py
--rw-r--r--   0        0        0     3937 2023-08-06 20:03:40.923859 lucidwallet-0.1.4/lucidwallet/screens/mnemonic_overlay.py
--rw-r--r--   0        0        0     3835 2023-08-06 20:03:55.905680 lucidwallet-0.1.4/lucidwallet/screens/no_wallets.py
--rw-r--r--   0        0        0     1678 2023-07-08 05:59:26.691461 lucidwallet-0.1.4/lucidwallet/screens/sendtx_overlay.py
--rw-r--r--   0        0        0     3518 2023-08-06 20:06:16.311072 lucidwallet-0.1.4/lucidwallet/screens/sign_message_overlay.py
--rw-r--r--   0        0        0     1093 2023-08-06 19:22:05.867386 lucidwallet-0.1.4/lucidwallet/screens/tx_sent_overlay.py
--rw-r--r--   0        0        0     2323 2023-08-06 19:22:05.844421 lucidwallet-0.1.4/lucidwallet/screens/txoverlay.py
--rw-r--r--   0        0        0        0 2023-07-11 16:57:43.918345 lucidwallet-0.1.4/lucidwallet/screens/wallet.css
--rw-r--r--   0        0        0    24205 2023-08-07 08:29:10.741526 lucidwallet-0.1.4/lucidwallet/screens/wallet_landing.py
--rw-r--r--   0        0        0     1164 2023-08-06 19:22:05.837177 lucidwallet-0.1.4/lucidwallet/tests/test.py
--rw-r--r--   0        0        0      163 2023-08-06 20:15:13.662310 lucidwallet-0.1.4/lucidwallet/widgets/__init__.py
--rw-r--r--   0        0        0     8336 2023-08-06 19:22:05.936904 lucidwallet-0.1.4/lucidwallet/widgets/send.py
--rw-r--r--   0        0        0     2795 2023-07-15 10:03:45.024418 lucidwallet-0.1.4/lucidwallet/widgets/send_working.py
--rw-r--r--   0        0        0       83 2023-06-27 10:24:20.921793 lucidwallet-0.1.4/lucidwallet/widgets/test_non_async.py
--rw-r--r--   0        0        0     5277 2023-08-06 20:07:31.561729 lucidwallet-0.1.4/lucidwallet/widgets/top_bar.py
--rw-r--r--   0        0        0     5383 2023-08-07 08:28:43.591539 lucidwallet-0.1.4/lucidwallet/widgets/transactions.py
--rw-r--r--   0        0        0     2842 2023-07-16 16:27:38.293266 lucidwallet-0.1.4/lucidwallet/widgets/transactions_old.py
--rw-r--r--   0        0        0     1039 2023-08-06 20:07:49.910935 lucidwallet-0.1.4/lucidwallet/widgets/tx_loading.py
--rw-r--r--   0        0        0      577 2023-08-07 08:49:20.608718 lucidwallet-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 lucidwallet-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-08-06 19:16:17.699415 lucidwallet-0.1.5/LICENSE
+-rw-r--r--   0        0        0       75 2023-08-06 20:21:50.851629 lucidwallet-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 07:44:41.990980 lucidwallet-0.1.5/lucidwallet/__init__.py
+-rw-r--r--   0        0        0     9730 2023-08-07 08:20:30.535722 lucidwallet-0.1.5/lucidwallet/app.css
+-rw-r--r--   0        0        0       71 2023-08-06 19:22:05.917312 lucidwallet-0.1.5/lucidwallet/datastore/__init__.py
+-rw-r--r--   0        0        0    13506 2023-08-06 20:12:07.119724 lucidwallet-0.1.5/lucidwallet/datastore/fluxwallet_datastore.py
+-rw-r--r--   0        0        0     3798 2023-08-07 09:31:02.519861 lucidwallet-0.1.5/lucidwallet/entrypoint.py
+-rw-r--r--   0        0        0      384 2023-08-04 11:22:47.433226 lucidwallet-0.1.5/lucidwallet/events/__init__.py
+-rw-r--r--   0        0        0     2109 2023-08-06 19:22:05.926687 lucidwallet-0.1.5/lucidwallet/helpers/__init__.py
+-rw-r--r--   0        0        0      948 2023-08-06 20:14:19.531008 lucidwallet-0.1.5/lucidwallet/screens/__init__.py
+-rw-r--r--   0        0        0     5812 2023-08-06 20:02:34.318411 lucidwallet-0.1.5/lucidwallet/screens/address_book.py
+-rw-r--r--   0        0        0     1547 2023-08-06 15:40:53.198703 lucidwallet-0.1.5/lucidwallet/screens/address_book_overlay.py
+-rw-r--r--   0        0        0     4017 2023-08-07 09:28:40.358907 lucidwallet-0.1.5/lucidwallet/screens/create_wallet.py
+-rw-r--r--   0        0        0     6294 2023-08-06 20:02:56.973871 lucidwallet-0.1.5/lucidwallet/screens/get_encryption_password.py
+-rw-r--r--   0        0        0    14950 2023-08-06 20:03:15.152907 lucidwallet-0.1.5/lucidwallet/screens/import_from_mnemonic.py
+-rw-r--r--   0        0        0     4480 2023-08-06 19:22:05.902145 lucidwallet-0.1.5/lucidwallet/screens/import_key_to_wallet.py
+-rw-r--r--   0        0        0     1635 2023-08-06 19:22:05.870564 lucidwallet-0.1.5/lucidwallet/screens/keychain_overlay.py
+-rw-r--r--   0        0        0     3869 2023-08-07 09:30:13.119960 lucidwallet-0.1.5/lucidwallet/screens/mnemonic_overlay.py
+-rw-r--r--   0        0        0     3835 2023-08-06 20:03:55.905680 lucidwallet-0.1.5/lucidwallet/screens/no_wallets.py
+-rw-r--r--   0        0        0     1678 2023-07-08 05:59:26.691461 lucidwallet-0.1.5/lucidwallet/screens/sendtx_overlay.py
+-rw-r--r--   0        0        0     3518 2023-08-06 20:06:16.311072 lucidwallet-0.1.5/lucidwallet/screens/sign_message_overlay.py
+-rw-r--r--   0        0        0     1093 2023-08-06 19:22:05.867386 lucidwallet-0.1.5/lucidwallet/screens/tx_sent_overlay.py
+-rw-r--r--   0        0        0     2323 2023-08-06 19:22:05.844421 lucidwallet-0.1.5/lucidwallet/screens/txoverlay.py
+-rw-r--r--   0        0        0        0 2023-07-11 16:57:43.918345 lucidwallet-0.1.5/lucidwallet/screens/wallet.css
+-rw-r--r--   0        0        0    24204 2023-08-07 09:32:39.449637 lucidwallet-0.1.5/lucidwallet/screens/wallet_landing.py
+-rw-r--r--   0        0        0     1164 2023-08-06 19:22:05.837177 lucidwallet-0.1.5/lucidwallet/tests/test.py
+-rw-r--r--   0        0        0      163 2023-08-06 20:15:13.662310 lucidwallet-0.1.5/lucidwallet/widgets/__init__.py
+-rw-r--r--   0        0        0     8336 2023-08-06 19:22:05.936904 lucidwallet-0.1.5/lucidwallet/widgets/send.py
+-rw-r--r--   0        0        0     2795 2023-07-15 10:03:45.024418 lucidwallet-0.1.5/lucidwallet/widgets/send_working.py
+-rw-r--r--   0        0        0       83 2023-06-27 10:24:20.921793 lucidwallet-0.1.5/lucidwallet/widgets/test_non_async.py
+-rw-r--r--   0        0        0     5277 2023-08-06 20:07:31.561729 lucidwallet-0.1.5/lucidwallet/widgets/top_bar.py
+-rw-r--r--   0        0        0     5383 2023-08-07 08:28:43.591539 lucidwallet-0.1.5/lucidwallet/widgets/transactions.py
+-rw-r--r--   0        0        0     2842 2023-07-16 16:27:38.293266 lucidwallet-0.1.5/lucidwallet/widgets/transactions_old.py
+-rw-r--r--   0        0        0     1039 2023-08-06 20:07:49.910935 lucidwallet-0.1.5/lucidwallet/widgets/tx_loading.py
+-rw-r--r--   0        0        0      577 2023-08-07 09:34:18.230157 lucidwallet-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 lucidwallet-0.1.5/PKG-INFO
```

### Comparing `lucidwallet-0.1.4/LICENSE` & `lucidwallet-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/app.css` & `lucidwallet-0.1.5/lucidwallet/app.css`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/datastore/fluxwallet_datastore.py` & `lucidwallet-0.1.5/lucidwallet/datastore/fluxwallet_datastore.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/entrypoint.py` & `lucidwallet-0.1.5/lucidwallet/entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,14 @@
         self.push_screen("wallet_landing")
 
     # fix these
     @on(MnemonicOverlay.WalletCreated)
     async def on_mnemonic_overlay_wallet_created(
         self, event: MnemonicOverlay.WalletCreated
     ):
-        ...
-        print("NEW WALLET CREATED IN APP")
         wallet_landing: WalletLanding = self.get_screen("wallet_landing")
         await wallet_landing.new_wallet_created(event.wallet)
 
     @on(ImportFromMnemonic.WalletCreated)
     async def on_import_from_mnemonic_wallet_created(
         self, event: ImportFromMnemonic.WalletCreated
     ):
```

### Comparing `lucidwallet-0.1.4/lucidwallet/helpers/__init__.py` & `lucidwallet-0.1.5/lucidwallet/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/__init__.py` & `lucidwallet-0.1.5/lucidwallet/screens/__init__.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/address_book.py` & `lucidwallet-0.1.5/lucidwallet/screens/address_book.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/address_book_overlay.py` & `lucidwallet-0.1.5/lucidwallet/screens/address_book_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/create_wallet.py` & `lucidwallet-0.1.5/lucidwallet/screens/create_wallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,14 @@
             app_data = await init_app()
             if self.nickname in app_data.wallets:
                 self.notify("Wallet name exists")
                 return
 
             lang_picker = self.query_one("LanguagePicker", LanguagePicker)
             mnemonic = Mnemonic(lang_picker.language).generate()
-            print(mnemonic)
 
             self.app.push_screen(MnemonicOverlay(self.nickname, mnemonic))
 
             self.reset_all()
         else:
             self.reset_all()
             self.dismiss()
```

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/get_encryption_password.py` & `lucidwallet-0.1.5/lucidwallet/screens/get_encryption_password.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/import_from_mnemonic.py` & `lucidwallet-0.1.5/lucidwallet/screens/import_from_mnemonic.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/import_key_to_wallet.py` & `lucidwallet-0.1.5/lucidwallet/screens/import_key_to_wallet.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/keychain_overlay.py` & `lucidwallet-0.1.5/lucidwallet/screens/keychain_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/mnemonic_overlay.py` & `lucidwallet-0.1.5/lucidwallet/screens/mnemonic_overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,27 +67,24 @@
 
     async def on_mount(self) -> None:
         # self.query_one("#reveal", Button).focus()
         self.create_wallet()
 
     @work()
     async def create_wallet(self):
-        print("CREATE EALLET")
         # have already validated, but validate again
         seed = Mnemonic().to_seed(self.mnemonic).hex()
         hdkey = HDKey.from_seed(seed, network="flux")
 
         wallet = await Wallet.create(
             self.nickname,
             hdkey,
             network="flux",
         )
 
-        print("NEW WALLET", wallet)
-
         if wallet:
             await wallet.new_key(network="bitcoin")
             app_data = await init_app()
 
             if not self.app.is_screen_installed("wallet_landing"):
                 self.app.install_screen(
                     WalletLanding(
```

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/no_wallets.py` & `lucidwallet-0.1.5/lucidwallet/screens/no_wallets.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/sendtx_overlay.py` & `lucidwallet-0.1.5/lucidwallet/screens/sendtx_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/sign_message_overlay.py` & `lucidwallet-0.1.5/lucidwallet/screens/sign_message_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/tx_sent_overlay.py` & `lucidwallet-0.1.5/lucidwallet/screens/tx_sent_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/txoverlay.py` & `lucidwallet-0.1.5/lucidwallet/screens/txoverlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/screens/wallet_landing.py` & `lucidwallet-0.1.5/lucidwallet/screens/wallet_landing.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,24 +600,25 @@
 
         await self.scan_network(
             wallet, network=network, key=key, scan_type=ScanType.NEW_KEY
         )
 
     @work(group="full_wallet_scan")
     async def full_wallet_scan(self) -> None:
-        print("FULL WALLET SCAN")
         await self.datastore.reset_timer(run_on_start=False)
         self.datastore.reset_current_wallet_datastore()
         self.tx_events.put_nowait(Event(type=Event.EventType.ClearTable))
 
         wallet = self.datastore.get_current_wallet()
         network = self.datastore.get_current_network()
 
         await self.scan_network(wallet, network, scan_type=ScanType.FULL_WALLET)
-        await self.update_dom()
+
+        if self.is_current:
+            await self.update_dom()
 
     def set_scanning_for_network(self, wallet_name: str, network_name: str) -> None:
         self.datastore.set_scanning_for_network(wallet_name, network_name)
 
         if (
             wallet_name == self.datastore.current_wallet
             and network_name == self.datastore.current_network
```

### Comparing `lucidwallet-0.1.4/lucidwallet/tests/test.py` & `lucidwallet-0.1.5/lucidwallet/tests/test.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/widgets/send.py` & `lucidwallet-0.1.5/lucidwallet/widgets/send.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/widgets/send_working.py` & `lucidwallet-0.1.5/lucidwallet/widgets/send_working.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/widgets/top_bar.py` & `lucidwallet-0.1.5/lucidwallet/widgets/top_bar.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/widgets/transactions.py` & `lucidwallet-0.1.5/lucidwallet/widgets/transactions.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/widgets/transactions_old.py` & `lucidwallet-0.1.5/lucidwallet/widgets/transactions_old.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/lucidwallet/widgets/tx_loading.py` & `lucidwallet-0.1.5/lucidwallet/widgets/tx_loading.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.4/pyproject.toml` & `lucidwallet-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lucidwallet"
-version = "0.1.4"
+version = "0.1.5"
 description = "A Graphical interface for FluxWallet"
 authors = ["David White <dr.white.nz@gmail.com>"]
 license = "bsd 3-clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `lucidwallet-0.1.4/PKG-INFO` & `lucidwallet-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidwallet
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Graphical interface for FluxWallet
 License: bsd 3-clause
 Author: David White
 Author-email: dr.white.nz@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

