# Comparing `tmp/lucidwallet-0.1.3.tar.gz` & `tmp/lucidwallet-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucidwallet-0.1.3.tar", max compression
+gzip compressed data, was "lucidwallet-0.1.4.tar", max compression
```

## Comparing `lucidwallet-0.1.3.tar` & `lucidwallet-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1488 2023-08-06 19:16:17.699415 lucidwallet-0.1.3/LICENSE
--rw-r--r--   0        0        0       75 2023-08-06 20:21:50.851629 lucidwallet-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-17 07:44:41.990980 lucidwallet-0.1.3/lucidwallet/__init__.py
--rw-r--r--   0        0        0     9730 2023-08-07 08:20:30.535722 lucidwallet-0.1.3/lucidwallet/app.css
--rw-r--r--   0        0        0       71 2023-08-06 19:22:05.917312 lucidwallet-0.1.3/lucidwallet/datastore/__init__.py
--rw-r--r--   0        0        0    13506 2023-08-06 20:12:07.119724 lucidwallet-0.1.3/lucidwallet/datastore/fluxwallet_datastore.py
--rw-r--r--   0        0        0     3861 2023-08-07 06:44:32.026122 lucidwallet-0.1.3/lucidwallet/entrypoint.py
--rw-r--r--   0        0        0      384 2023-08-04 11:22:47.433226 lucidwallet-0.1.3/lucidwallet/events/__init__.py
--rw-r--r--   0        0        0     2109 2023-08-06 19:22:05.926687 lucidwallet-0.1.3/lucidwallet/helpers/__init__.py
--rw-r--r--   0        0        0      948 2023-08-06 20:14:19.531008 lucidwallet-0.1.3/lucidwallet/screens/__init__.py
--rw-r--r--   0        0        0     5812 2023-08-06 20:02:34.318411 lucidwallet-0.1.3/lucidwallet/screens/address_book.py
--rw-r--r--   0        0        0     1547 2023-08-06 15:40:53.198703 lucidwallet-0.1.3/lucidwallet/screens/address_book_overlay.py
--rw-r--r--   0        0        0     4045 2023-08-06 20:02:21.438840 lucidwallet-0.1.3/lucidwallet/screens/create_wallet.py
--rw-r--r--   0        0        0     6294 2023-08-06 20:02:56.973871 lucidwallet-0.1.3/lucidwallet/screens/get_encryption_password.py
--rw-r--r--   0        0        0    14950 2023-08-06 20:03:15.152907 lucidwallet-0.1.3/lucidwallet/screens/import_from_mnemonic.py
--rw-r--r--   0        0        0     4480 2023-08-06 19:22:05.902145 lucidwallet-0.1.3/lucidwallet/screens/import_key_to_wallet.py
--rw-r--r--   0        0        0     1635 2023-08-06 19:22:05.870564 lucidwallet-0.1.3/lucidwallet/screens/keychain_overlay.py
--rw-r--r--   0        0        0     3937 2023-08-06 20:03:40.923859 lucidwallet-0.1.3/lucidwallet/screens/mnemonic_overlay.py
--rw-r--r--   0        0        0     3835 2023-08-06 20:03:55.905680 lucidwallet-0.1.3/lucidwallet/screens/no_wallets.py
--rw-r--r--   0        0        0     1678 2023-07-08 05:59:26.691461 lucidwallet-0.1.3/lucidwallet/screens/sendtx_overlay.py
--rw-r--r--   0        0        0     3518 2023-08-06 20:06:16.311072 lucidwallet-0.1.3/lucidwallet/screens/sign_message_overlay.py
--rw-r--r--   0        0        0     1093 2023-08-06 19:22:05.867386 lucidwallet-0.1.3/lucidwallet/screens/tx_sent_overlay.py
--rw-r--r--   0        0        0     2323 2023-08-06 19:22:05.844421 lucidwallet-0.1.3/lucidwallet/screens/txoverlay.py
--rw-r--r--   0        0        0        0 2023-07-11 16:57:43.918345 lucidwallet-0.1.3/lucidwallet/screens/wallet.css
--rw-r--r--   0        0        0    24205 2023-08-07 08:29:10.741526 lucidwallet-0.1.3/lucidwallet/screens/wallet_landing.py
--rw-r--r--   0        0        0     1164 2023-08-06 19:22:05.837177 lucidwallet-0.1.3/lucidwallet/tests/test.py
--rw-r--r--   0        0        0      163 2023-08-06 20:15:13.662310 lucidwallet-0.1.3/lucidwallet/widgets/__init__.py
--rw-r--r--   0        0        0     8336 2023-08-06 19:22:05.936904 lucidwallet-0.1.3/lucidwallet/widgets/send.py
--rw-r--r--   0        0        0     2795 2023-07-15 10:03:45.024418 lucidwallet-0.1.3/lucidwallet/widgets/send_working.py
--rw-r--r--   0        0        0       83 2023-06-27 10:24:20.921793 lucidwallet-0.1.3/lucidwallet/widgets/test_non_async.py
--rw-r--r--   0        0        0     5277 2023-08-06 20:07:31.561729 lucidwallet-0.1.3/lucidwallet/widgets/top_bar.py
--rw-r--r--   0        0        0     5383 2023-08-07 08:28:43.591539 lucidwallet-0.1.3/lucidwallet/widgets/transactions.py
--rw-r--r--   0        0        0     2842 2023-07-16 16:27:38.293266 lucidwallet-0.1.3/lucidwallet/widgets/transactions_old.py
--rw-r--r--   0        0        0     1039 2023-08-06 20:07:49.910935 lucidwallet-0.1.3/lucidwallet/widgets/tx_loading.py
--rw-r--r--   0        0        0      577 2023-08-07 08:29:22.177751 lucidwallet-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 lucidwallet-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-08-06 19:16:17.699415 lucidwallet-0.1.4/LICENSE
+-rw-r--r--   0        0        0       75 2023-08-06 20:21:50.851629 lucidwallet-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 07:44:41.990980 lucidwallet-0.1.4/lucidwallet/__init__.py
+-rw-r--r--   0        0        0     9730 2023-08-07 08:20:30.535722 lucidwallet-0.1.4/lucidwallet/app.css
+-rw-r--r--   0        0        0       71 2023-08-06 19:22:05.917312 lucidwallet-0.1.4/lucidwallet/datastore/__init__.py
+-rw-r--r--   0        0        0    13506 2023-08-06 20:12:07.119724 lucidwallet-0.1.4/lucidwallet/datastore/fluxwallet_datastore.py
+-rw-r--r--   0        0        0     3853 2023-08-07 08:49:11.804229 lucidwallet-0.1.4/lucidwallet/entrypoint.py
+-rw-r--r--   0        0        0      384 2023-08-04 11:22:47.433226 lucidwallet-0.1.4/lucidwallet/events/__init__.py
+-rw-r--r--   0        0        0     2109 2023-08-06 19:22:05.926687 lucidwallet-0.1.4/lucidwallet/helpers/__init__.py
+-rw-r--r--   0        0        0      948 2023-08-06 20:14:19.531008 lucidwallet-0.1.4/lucidwallet/screens/__init__.py
+-rw-r--r--   0        0        0     5812 2023-08-06 20:02:34.318411 lucidwallet-0.1.4/lucidwallet/screens/address_book.py
+-rw-r--r--   0        0        0     1547 2023-08-06 15:40:53.198703 lucidwallet-0.1.4/lucidwallet/screens/address_book_overlay.py
+-rw-r--r--   0        0        0     4045 2023-08-06 20:02:21.438840 lucidwallet-0.1.4/lucidwallet/screens/create_wallet.py
+-rw-r--r--   0        0        0     6294 2023-08-06 20:02:56.973871 lucidwallet-0.1.4/lucidwallet/screens/get_encryption_password.py
+-rw-r--r--   0        0        0    14950 2023-08-06 20:03:15.152907 lucidwallet-0.1.4/lucidwallet/screens/import_from_mnemonic.py
+-rw-r--r--   0        0        0     4480 2023-08-06 19:22:05.902145 lucidwallet-0.1.4/lucidwallet/screens/import_key_to_wallet.py
+-rw-r--r--   0        0        0     1635 2023-08-06 19:22:05.870564 lucidwallet-0.1.4/lucidwallet/screens/keychain_overlay.py
+-rw-r--r--   0        0        0     3937 2023-08-06 20:03:40.923859 lucidwallet-0.1.4/lucidwallet/screens/mnemonic_overlay.py
+-rw-r--r--   0        0        0     3835 2023-08-06 20:03:55.905680 lucidwallet-0.1.4/lucidwallet/screens/no_wallets.py
+-rw-r--r--   0        0        0     1678 2023-07-08 05:59:26.691461 lucidwallet-0.1.4/lucidwallet/screens/sendtx_overlay.py
+-rw-r--r--   0        0        0     3518 2023-08-06 20:06:16.311072 lucidwallet-0.1.4/lucidwallet/screens/sign_message_overlay.py
+-rw-r--r--   0        0        0     1093 2023-08-06 19:22:05.867386 lucidwallet-0.1.4/lucidwallet/screens/tx_sent_overlay.py
+-rw-r--r--   0        0        0     2323 2023-08-06 19:22:05.844421 lucidwallet-0.1.4/lucidwallet/screens/txoverlay.py
+-rw-r--r--   0        0        0        0 2023-07-11 16:57:43.918345 lucidwallet-0.1.4/lucidwallet/screens/wallet.css
+-rw-r--r--   0        0        0    24205 2023-08-07 08:29:10.741526 lucidwallet-0.1.4/lucidwallet/screens/wallet_landing.py
+-rw-r--r--   0        0        0     1164 2023-08-06 19:22:05.837177 lucidwallet-0.1.4/lucidwallet/tests/test.py
+-rw-r--r--   0        0        0      163 2023-08-06 20:15:13.662310 lucidwallet-0.1.4/lucidwallet/widgets/__init__.py
+-rw-r--r--   0        0        0     8336 2023-08-06 19:22:05.936904 lucidwallet-0.1.4/lucidwallet/widgets/send.py
+-rw-r--r--   0        0        0     2795 2023-07-15 10:03:45.024418 lucidwallet-0.1.4/lucidwallet/widgets/send_working.py
+-rw-r--r--   0        0        0       83 2023-06-27 10:24:20.921793 lucidwallet-0.1.4/lucidwallet/widgets/test_non_async.py
+-rw-r--r--   0        0        0     5277 2023-08-06 20:07:31.561729 lucidwallet-0.1.4/lucidwallet/widgets/top_bar.py
+-rw-r--r--   0        0        0     5383 2023-08-07 08:28:43.591539 lucidwallet-0.1.4/lucidwallet/widgets/transactions.py
+-rw-r--r--   0        0        0     2842 2023-07-16 16:27:38.293266 lucidwallet-0.1.4/lucidwallet/widgets/transactions_old.py
+-rw-r--r--   0        0        0     1039 2023-08-06 20:07:49.910935 lucidwallet-0.1.4/lucidwallet/widgets/tx_loading.py
+-rw-r--r--   0        0        0      577 2023-08-07 08:49:20.608718 lucidwallet-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 lucidwallet-0.1.4/PKG-INFO
```

### Comparing `lucidwallet-0.1.3/LICENSE` & `lucidwallet-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/app.css` & `lucidwallet-0.1.4/lucidwallet/app.css`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/datastore/fluxwallet_datastore.py` & `lucidwallet-0.1.4/lucidwallet/datastore/fluxwallet_datastore.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/entrypoint.py` & `lucidwallet-0.1.4/lucidwallet/entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,10 +110,7 @@
         wallet_landing: WalletLanding = self.get_screen("wallet_landing")
         await wallet_landing.new_wallet_created(event.wallet)
 
 
 def run():
     app = FluxWallet()
     app.run()
-
-
-run()
```

### Comparing `lucidwallet-0.1.3/lucidwallet/helpers/__init__.py` & `lucidwallet-0.1.4/lucidwallet/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/__init__.py` & `lucidwallet-0.1.4/lucidwallet/screens/__init__.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/address_book.py` & `lucidwallet-0.1.4/lucidwallet/screens/address_book.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/address_book_overlay.py` & `lucidwallet-0.1.4/lucidwallet/screens/address_book_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/create_wallet.py` & `lucidwallet-0.1.4/lucidwallet/screens/create_wallet.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/get_encryption_password.py` & `lucidwallet-0.1.4/lucidwallet/screens/get_encryption_password.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/import_from_mnemonic.py` & `lucidwallet-0.1.4/lucidwallet/screens/import_from_mnemonic.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/import_key_to_wallet.py` & `lucidwallet-0.1.4/lucidwallet/screens/import_key_to_wallet.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/keychain_overlay.py` & `lucidwallet-0.1.4/lucidwallet/screens/keychain_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/mnemonic_overlay.py` & `lucidwallet-0.1.4/lucidwallet/screens/mnemonic_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/no_wallets.py` & `lucidwallet-0.1.4/lucidwallet/screens/no_wallets.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/sendtx_overlay.py` & `lucidwallet-0.1.4/lucidwallet/screens/sendtx_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/sign_message_overlay.py` & `lucidwallet-0.1.4/lucidwallet/screens/sign_message_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/tx_sent_overlay.py` & `lucidwallet-0.1.4/lucidwallet/screens/tx_sent_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/txoverlay.py` & `lucidwallet-0.1.4/lucidwallet/screens/txoverlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/screens/wallet_landing.py` & `lucidwallet-0.1.4/lucidwallet/screens/wallet_landing.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/tests/test.py` & `lucidwallet-0.1.4/lucidwallet/tests/test.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/widgets/send.py` & `lucidwallet-0.1.4/lucidwallet/widgets/send.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/widgets/send_working.py` & `lucidwallet-0.1.4/lucidwallet/widgets/send_working.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/widgets/top_bar.py` & `lucidwallet-0.1.4/lucidwallet/widgets/top_bar.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/widgets/transactions.py` & `lucidwallet-0.1.4/lucidwallet/widgets/transactions.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/widgets/transactions_old.py` & `lucidwallet-0.1.4/lucidwallet/widgets/transactions_old.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/lucidwallet/widgets/tx_loading.py` & `lucidwallet-0.1.4/lucidwallet/widgets/tx_loading.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.3/pyproject.toml` & `lucidwallet-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lucidwallet"
-version = "0.1.3"
+version = "0.1.4"
 description = "A Graphical interface for FluxWallet"
 authors = ["David White <dr.white.nz@gmail.com>"]
 license = "bsd 3-clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `lucidwallet-0.1.3/PKG-INFO` & `lucidwallet-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidwallet
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Graphical interface for FluxWallet
 License: bsd 3-clause
 Author: David White
 Author-email: dr.white.nz@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

