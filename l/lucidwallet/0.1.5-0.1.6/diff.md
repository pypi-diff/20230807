# Comparing `tmp/lucidwallet-0.1.5.tar.gz` & `tmp/lucidwallet-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucidwallet-0.1.5.tar", max compression
+gzip compressed data, was "lucidwallet-0.1.6.tar", max compression
```

## Comparing `lucidwallet-0.1.5.tar` & `lucidwallet-0.1.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1488 2023-08-06 19:16:17.699415 lucidwallet-0.1.5/LICENSE
--rw-r--r--   0        0        0       75 2023-08-06 20:21:50.851629 lucidwallet-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-17 07:44:41.990980 lucidwallet-0.1.5/lucidwallet/__init__.py
--rw-r--r--   0        0        0     9730 2023-08-07 08:20:30.535722 lucidwallet-0.1.5/lucidwallet/app.css
--rw-r--r--   0        0        0       71 2023-08-06 19:22:05.917312 lucidwallet-0.1.5/lucidwallet/datastore/__init__.py
--rw-r--r--   0        0        0    13506 2023-08-06 20:12:07.119724 lucidwallet-0.1.5/lucidwallet/datastore/fluxwallet_datastore.py
--rw-r--r--   0        0        0     3798 2023-08-07 09:31:02.519861 lucidwallet-0.1.5/lucidwallet/entrypoint.py
--rw-r--r--   0        0        0      384 2023-08-04 11:22:47.433226 lucidwallet-0.1.5/lucidwallet/events/__init__.py
--rw-r--r--   0        0        0     2109 2023-08-06 19:22:05.926687 lucidwallet-0.1.5/lucidwallet/helpers/__init__.py
--rw-r--r--   0        0        0      948 2023-08-06 20:14:19.531008 lucidwallet-0.1.5/lucidwallet/screens/__init__.py
--rw-r--r--   0        0        0     5812 2023-08-06 20:02:34.318411 lucidwallet-0.1.5/lucidwallet/screens/address_book.py
--rw-r--r--   0        0        0     1547 2023-08-06 15:40:53.198703 lucidwallet-0.1.5/lucidwallet/screens/address_book_overlay.py
--rw-r--r--   0        0        0     4017 2023-08-07 09:28:40.358907 lucidwallet-0.1.5/lucidwallet/screens/create_wallet.py
--rw-r--r--   0        0        0     6294 2023-08-06 20:02:56.973871 lucidwallet-0.1.5/lucidwallet/screens/get_encryption_password.py
--rw-r--r--   0        0        0    14950 2023-08-06 20:03:15.152907 lucidwallet-0.1.5/lucidwallet/screens/import_from_mnemonic.py
--rw-r--r--   0        0        0     4480 2023-08-06 19:22:05.902145 lucidwallet-0.1.5/lucidwallet/screens/import_key_to_wallet.py
--rw-r--r--   0        0        0     1635 2023-08-06 19:22:05.870564 lucidwallet-0.1.5/lucidwallet/screens/keychain_overlay.py
--rw-r--r--   0        0        0     3869 2023-08-07 09:30:13.119960 lucidwallet-0.1.5/lucidwallet/screens/mnemonic_overlay.py
--rw-r--r--   0        0        0     3835 2023-08-06 20:03:55.905680 lucidwallet-0.1.5/lucidwallet/screens/no_wallets.py
--rw-r--r--   0        0        0     1678 2023-07-08 05:59:26.691461 lucidwallet-0.1.5/lucidwallet/screens/sendtx_overlay.py
--rw-r--r--   0        0        0     3518 2023-08-06 20:06:16.311072 lucidwallet-0.1.5/lucidwallet/screens/sign_message_overlay.py
--rw-r--r--   0        0        0     1093 2023-08-06 19:22:05.867386 lucidwallet-0.1.5/lucidwallet/screens/tx_sent_overlay.py
--rw-r--r--   0        0        0     2323 2023-08-06 19:22:05.844421 lucidwallet-0.1.5/lucidwallet/screens/txoverlay.py
--rw-r--r--   0        0        0        0 2023-07-11 16:57:43.918345 lucidwallet-0.1.5/lucidwallet/screens/wallet.css
--rw-r--r--   0        0        0    24204 2023-08-07 09:32:39.449637 lucidwallet-0.1.5/lucidwallet/screens/wallet_landing.py
--rw-r--r--   0        0        0     1164 2023-08-06 19:22:05.837177 lucidwallet-0.1.5/lucidwallet/tests/test.py
--rw-r--r--   0        0        0      163 2023-08-06 20:15:13.662310 lucidwallet-0.1.5/lucidwallet/widgets/__init__.py
--rw-r--r--   0        0        0     8336 2023-08-06 19:22:05.936904 lucidwallet-0.1.5/lucidwallet/widgets/send.py
--rw-r--r--   0        0        0     2795 2023-07-15 10:03:45.024418 lucidwallet-0.1.5/lucidwallet/widgets/send_working.py
--rw-r--r--   0        0        0       83 2023-06-27 10:24:20.921793 lucidwallet-0.1.5/lucidwallet/widgets/test_non_async.py
--rw-r--r--   0        0        0     5277 2023-08-06 20:07:31.561729 lucidwallet-0.1.5/lucidwallet/widgets/top_bar.py
--rw-r--r--   0        0        0     5383 2023-08-07 08:28:43.591539 lucidwallet-0.1.5/lucidwallet/widgets/transactions.py
--rw-r--r--   0        0        0     2842 2023-07-16 16:27:38.293266 lucidwallet-0.1.5/lucidwallet/widgets/transactions_old.py
--rw-r--r--   0        0        0     1039 2023-08-06 20:07:49.910935 lucidwallet-0.1.5/lucidwallet/widgets/tx_loading.py
--rw-r--r--   0        0        0      577 2023-08-07 09:34:18.230157 lucidwallet-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 lucidwallet-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-08-06 19:16:17.699415 lucidwallet-0.1.6/LICENSE
+-rw-r--r--   0        0        0       75 2023-08-06 20:21:50.851629 lucidwallet-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 07:44:41.990980 lucidwallet-0.1.6/lucidwallet/__init__.py
+-rw-r--r--   0        0        0     9652 2023-08-07 09:42:58.483852 lucidwallet-0.1.6/lucidwallet/app.css
+-rw-r--r--   0        0        0       71 2023-08-06 19:22:05.917312 lucidwallet-0.1.6/lucidwallet/datastore/__init__.py
+-rw-r--r--   0        0        0    13506 2023-08-06 20:12:07.119724 lucidwallet-0.1.6/lucidwallet/datastore/fluxwallet_datastore.py
+-rw-r--r--   0        0        0     3798 2023-08-07 09:31:02.519861 lucidwallet-0.1.6/lucidwallet/entrypoint.py
+-rw-r--r--   0        0        0      384 2023-08-04 11:22:47.433226 lucidwallet-0.1.6/lucidwallet/events/__init__.py
+-rw-r--r--   0        0        0     2109 2023-08-06 19:22:05.926687 lucidwallet-0.1.6/lucidwallet/helpers/__init__.py
+-rw-r--r--   0        0        0      948 2023-08-06 20:14:19.531008 lucidwallet-0.1.6/lucidwallet/screens/__init__.py
+-rw-r--r--   0        0        0     5812 2023-08-06 20:02:34.318411 lucidwallet-0.1.6/lucidwallet/screens/address_book.py
+-rw-r--r--   0        0        0     1547 2023-08-06 15:40:53.198703 lucidwallet-0.1.6/lucidwallet/screens/address_book_overlay.py
+-rw-r--r--   0        0        0     4017 2023-08-07 09:28:40.358907 lucidwallet-0.1.6/lucidwallet/screens/create_wallet.py
+-rw-r--r--   0        0        0     6294 2023-08-06 20:02:56.973871 lucidwallet-0.1.6/lucidwallet/screens/get_encryption_password.py
+-rw-r--r--   0        0        0    14950 2023-08-06 20:03:15.152907 lucidwallet-0.1.6/lucidwallet/screens/import_from_mnemonic.py
+-rw-r--r--   0        0        0     4480 2023-08-06 19:22:05.902145 lucidwallet-0.1.6/lucidwallet/screens/import_key_to_wallet.py
+-rw-r--r--   0        0        0     1635 2023-08-06 19:22:05.870564 lucidwallet-0.1.6/lucidwallet/screens/keychain_overlay.py
+-rw-r--r--   0        0        0     3869 2023-08-07 09:30:13.119960 lucidwallet-0.1.6/lucidwallet/screens/mnemonic_overlay.py
+-rw-r--r--   0        0        0     3835 2023-08-06 20:03:55.905680 lucidwallet-0.1.6/lucidwallet/screens/no_wallets.py
+-rw-r--r--   0        0        0     1678 2023-07-08 05:59:26.691461 lucidwallet-0.1.6/lucidwallet/screens/sendtx_overlay.py
+-rw-r--r--   0        0        0     3518 2023-08-06 20:06:16.311072 lucidwallet-0.1.6/lucidwallet/screens/sign_message_overlay.py
+-rw-r--r--   0        0        0     1093 2023-08-06 19:22:05.867386 lucidwallet-0.1.6/lucidwallet/screens/tx_sent_overlay.py
+-rw-r--r--   0        0        0     2323 2023-08-06 19:22:05.844421 lucidwallet-0.1.6/lucidwallet/screens/txoverlay.py
+-rw-r--r--   0        0        0        0 2023-07-11 16:57:43.918345 lucidwallet-0.1.6/lucidwallet/screens/wallet.css
+-rw-r--r--   0        0        0    24204 2023-08-07 09:32:39.449637 lucidwallet-0.1.6/lucidwallet/screens/wallet_landing.py
+-rw-r--r--   0        0        0     1164 2023-08-06 19:22:05.837177 lucidwallet-0.1.6/lucidwallet/tests/test.py
+-rw-r--r--   0        0        0      163 2023-08-06 20:15:13.662310 lucidwallet-0.1.6/lucidwallet/widgets/__init__.py
+-rw-r--r--   0        0        0     8060 2023-08-07 09:43:47.341582 lucidwallet-0.1.6/lucidwallet/widgets/send.py
+-rw-r--r--   0        0        0     2795 2023-07-15 10:03:45.024418 lucidwallet-0.1.6/lucidwallet/widgets/send_working.py
+-rw-r--r--   0        0        0       83 2023-06-27 10:24:20.921793 lucidwallet-0.1.6/lucidwallet/widgets/test_non_async.py
+-rw-r--r--   0        0        0     5277 2023-08-06 20:07:31.561729 lucidwallet-0.1.6/lucidwallet/widgets/top_bar.py
+-rw-r--r--   0        0        0     5383 2023-08-07 08:28:43.591539 lucidwallet-0.1.6/lucidwallet/widgets/transactions.py
+-rw-r--r--   0        0        0     2842 2023-07-16 16:27:38.293266 lucidwallet-0.1.6/lucidwallet/widgets/transactions_old.py
+-rw-r--r--   0        0        0     1039 2023-08-06 20:07:49.910935 lucidwallet-0.1.6/lucidwallet/widgets/tx_loading.py
+-rw-r--r--   0        0        0      577 2023-08-07 09:43:54.872548 lucidwallet-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 lucidwallet-0.1.6/PKG-INFO
```

### Comparing `lucidwallet-0.1.5/LICENSE` & `lucidwallet-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/app.css` & `lucidwallet-0.1.6/lucidwallet/app.css`

 * *Files 0% similar despite different names*

```diff
@@ -667,21 +667,18 @@
     min-width: 5;
     width: 5;
 
 }
 
 /* SEND */
 
-#disabled_send_container {
-    layer: notification;
-    width: 1fr;
-    height: 1fr;
-    align: center middle;
-}
-
 #disabled_send_banner {
     content-align: center middle;
     layer: notification;
     width: 16;
     height: 8;
     border: yellowgreen;
+}
+
+Send {
+    align: center middle;
 }
```

### Comparing `lucidwallet-0.1.5/lucidwallet/datastore/fluxwallet_datastore.py` & `lucidwallet-0.1.6/lucidwallet/datastore/fluxwallet_datastore.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/entrypoint.py` & `lucidwallet-0.1.6/lucidwallet/entrypoint.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/helpers/__init__.py` & `lucidwallet-0.1.6/lucidwallet/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/__init__.py` & `lucidwallet-0.1.6/lucidwallet/screens/__init__.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/address_book.py` & `lucidwallet-0.1.6/lucidwallet/screens/address_book.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/address_book_overlay.py` & `lucidwallet-0.1.6/lucidwallet/screens/address_book_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/create_wallet.py` & `lucidwallet-0.1.6/lucidwallet/screens/create_wallet.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/get_encryption_password.py` & `lucidwallet-0.1.6/lucidwallet/screens/get_encryption_password.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/import_from_mnemonic.py` & `lucidwallet-0.1.6/lucidwallet/screens/import_from_mnemonic.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/import_key_to_wallet.py` & `lucidwallet-0.1.6/lucidwallet/screens/import_key_to_wallet.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/keychain_overlay.py` & `lucidwallet-0.1.6/lucidwallet/screens/keychain_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/mnemonic_overlay.py` & `lucidwallet-0.1.6/lucidwallet/screens/mnemonic_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/no_wallets.py` & `lucidwallet-0.1.6/lucidwallet/screens/no_wallets.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/sendtx_overlay.py` & `lucidwallet-0.1.6/lucidwallet/screens/sendtx_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/sign_message_overlay.py` & `lucidwallet-0.1.6/lucidwallet/screens/sign_message_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/tx_sent_overlay.py` & `lucidwallet-0.1.6/lucidwallet/screens/tx_sent_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/txoverlay.py` & `lucidwallet-0.1.6/lucidwallet/screens/txoverlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/screens/wallet_landing.py` & `lucidwallet-0.1.6/lucidwallet/screens/wallet_landing.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/tests/test.py` & `lucidwallet-0.1.6/lucidwallet/tests/test.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/widgets/send.py` & `lucidwallet-0.1.6/lucidwallet/widgets/send.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,18 +115,15 @@
     class AddressBookUpdateRequested(Message):
         def __init__(self, address: str):
             self.address = address
             super().__init__()
 
     def __init__(self, address_book: dict[str, str] = {}):
         self.address_book = address_book
-        self.disabled_overlay = Container(
-            Static("Coming soon", id="disabled_send_banner"),
-            id="disabled_send_container",
-        )
+        self.disabled_overlay = Static("Coming soon", id="disabled_send_banner")
         self.disabled_mounted = False
         super().__init__()
 
     def compose(self) -> ComposeResult:
         yield Center(Label("Send coins"))
         yield Horizontal(
             Input(
@@ -186,28 +183,24 @@
         address_book_dom = self.query_one("#address_book", Select)
         address_book_dom.set_options(options_list)
 
         if selected:
             address_book_dom.value = selected
 
     def mount_disabled(self) -> None:
-        print("MOUNT", self.disabled_mounted)
         if not self.disabled_mounted:
             self.disabled_mounted = True
+            self.disabled = True
             self.mount(self.disabled_overlay)
 
     def unmount_disabled(self) -> None:
-        print("UNMOUNT", self.disabled_mounted)
         if self.disabled_mounted:
             self.disabled_mounted = False
+            self.disabled = False
             self.disabled_overlay.remove()
-            self.disabled_overlay = Container(
-                Static("Coming soon", id="disabled_send_banner"),
-                id="disabled_send_container",
-            )
 
     @on(Input.Changed, "#address")
     def address_input_changed(self, event: Input.Changed) -> None:
         event.stop()
 
         if not event.validation_result.failures:
             self.sendto_address = event.value
```

### Comparing `lucidwallet-0.1.5/lucidwallet/widgets/send_working.py` & `lucidwallet-0.1.6/lucidwallet/widgets/send_working.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/widgets/top_bar.py` & `lucidwallet-0.1.6/lucidwallet/widgets/top_bar.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/widgets/transactions.py` & `lucidwallet-0.1.6/lucidwallet/widgets/transactions.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/widgets/transactions_old.py` & `lucidwallet-0.1.6/lucidwallet/widgets/transactions_old.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/lucidwallet/widgets/tx_loading.py` & `lucidwallet-0.1.6/lucidwallet/widgets/tx_loading.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.5/pyproject.toml` & `lucidwallet-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lucidwallet"
-version = "0.1.5"
+version = "0.1.6"
 description = "A Graphical interface for FluxWallet"
 authors = ["David White <dr.white.nz@gmail.com>"]
 license = "bsd 3-clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `lucidwallet-0.1.5/PKG-INFO` & `lucidwallet-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucidwallet
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Graphical interface for FluxWallet
 License: bsd 3-clause
 Author: David White
 Author-email: dr.white.nz@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

