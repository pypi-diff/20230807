# Comparing `tmp/lucidwallet-0.1.0.tar.gz` & `tmp/lucidwallet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucidwallet-0.1.0.tar", max compression
+gzip compressed data, was "lucidwallet-0.1.2.tar", max compression
```

## Comparing `lucidwallet-0.1.0.tar` & `lucidwallet-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1488 2023-08-06 19:16:17.699415 lucidwallet-0.1.0/LICENSE
--rw-r--r--   0        0        0       75 2023-08-06 20:21:50.851629 lucidwallet-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-17 07:44:41.990980 lucidwallet-0.1.0/lucidwallet/__init__.py
--rw-r--r--   0        0        0     9428 2023-08-06 18:45:06.969112 lucidwallet-0.1.0/lucidwallet/app.css
--rw-r--r--   0        0        0       71 2023-08-06 19:22:05.917312 lucidwallet-0.1.0/lucidwallet/datastore/__init__.py
--rw-r--r--   0        0        0    13506 2023-08-06 20:12:07.119724 lucidwallet-0.1.0/lucidwallet/datastore/fluxwallet_datastore.py
--rw-r--r--   0        0        0     3831 2023-08-06 19:53:29.456892 lucidwallet-0.1.0/lucidwallet/entrypoint.py
--rw-r--r--   0        0        0      384 2023-08-04 11:22:47.433226 lucidwallet-0.1.0/lucidwallet/events/__init__.py
--rw-r--r--   0        0        0     2109 2023-08-06 19:22:05.926687 lucidwallet-0.1.0/lucidwallet/helpers/__init__.py
--rw-r--r--   0        0        0      948 2023-08-06 20:14:19.531008 lucidwallet-0.1.0/lucidwallet/screens/__init__.py
--rw-r--r--   0        0        0     5812 2023-08-06 20:02:34.318411 lucidwallet-0.1.0/lucidwallet/screens/address_book.py
--rw-r--r--   0        0        0     1547 2023-08-06 15:40:53.198703 lucidwallet-0.1.0/lucidwallet/screens/address_book_overlay.py
--rw-r--r--   0        0        0     4045 2023-08-06 20:02:21.438840 lucidwallet-0.1.0/lucidwallet/screens/create_wallet.py
--rw-r--r--   0        0        0     6294 2023-08-06 20:02:56.973871 lucidwallet-0.1.0/lucidwallet/screens/get_encryption_password.py
--rw-r--r--   0        0        0    14950 2023-08-06 20:03:15.152907 lucidwallet-0.1.0/lucidwallet/screens/import_from_mnemonic.py
--rw-r--r--   0        0        0     4480 2023-08-06 19:22:05.902145 lucidwallet-0.1.0/lucidwallet/screens/import_key_to_wallet.py
--rw-r--r--   0        0        0     1635 2023-08-06 19:22:05.870564 lucidwallet-0.1.0/lucidwallet/screens/keychain_overlay.py
--rw-r--r--   0        0        0     3937 2023-08-06 20:03:40.923859 lucidwallet-0.1.0/lucidwallet/screens/mnemonic_overlay.py
--rw-r--r--   0        0        0     3835 2023-08-06 20:03:55.905680 lucidwallet-0.1.0/lucidwallet/screens/no_wallets.py
--rw-r--r--   0        0        0     1678 2023-07-08 05:59:26.691461 lucidwallet-0.1.0/lucidwallet/screens/sendtx_overlay.py
--rw-r--r--   0        0        0     3518 2023-08-06 20:06:16.311072 lucidwallet-0.1.0/lucidwallet/screens/sign_message_overlay.py
--rw-r--r--   0        0        0     1093 2023-08-06 19:22:05.867386 lucidwallet-0.1.0/lucidwallet/screens/tx_sent_overlay.py
--rw-r--r--   0        0        0     2323 2023-08-06 19:22:05.844421 lucidwallet-0.1.0/lucidwallet/screens/txoverlay.py
--rw-r--r--   0        0        0        0 2023-07-11 16:57:43.918345 lucidwallet-0.1.0/lucidwallet/screens/wallet.css
--rw-r--r--   0        0        0    24220 2023-08-06 20:06:45.288791 lucidwallet-0.1.0/lucidwallet/screens/wallet_landing.py
--rw-r--r--   0        0        0     1164 2023-08-06 19:22:05.837177 lucidwallet-0.1.0/lucidwallet/tests/test.py
--rw-r--r--   0        0        0      163 2023-08-06 20:15:13.662310 lucidwallet-0.1.0/lucidwallet/widgets/__init__.py
--rw-r--r--   0        0        0     8336 2023-08-06 19:22:05.936904 lucidwallet-0.1.0/lucidwallet/widgets/send.py
--rw-r--r--   0        0        0     2795 2023-07-15 10:03:45.024418 lucidwallet-0.1.0/lucidwallet/widgets/send_working.py
--rw-r--r--   0        0        0       83 2023-06-27 10:24:20.921793 lucidwallet-0.1.0/lucidwallet/widgets/test_non_async.py
--rw-r--r--   0        0        0     5277 2023-08-06 20:07:31.561729 lucidwallet-0.1.0/lucidwallet/widgets/top_bar.py
--rw-r--r--   0        0        0     4975 2023-08-06 20:14:38.327662 lucidwallet-0.1.0/lucidwallet/widgets/transactions.py
--rw-r--r--   0        0        0     2842 2023-07-16 16:27:38.293266 lucidwallet-0.1.0/lucidwallet/widgets/transactions_old.py
--rw-r--r--   0        0        0     1039 2023-08-06 20:07:49.910935 lucidwallet-0.1.0/lucidwallet/widgets/tx_loading.py
--rw-r--r--   0        0        0      557 2023-08-06 20:18:10.971990 lucidwallet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 lucidwallet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-08-06 19:16:17.699415 lucidwallet-0.1.2/LICENSE
+-rw-r--r--   0        0        0       75 2023-08-06 20:21:50.851629 lucidwallet-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 07:44:41.990980 lucidwallet-0.1.2/lucidwallet/__init__.py
+-rw-r--r--   0        0        0     9730 2023-08-07 08:20:30.535722 lucidwallet-0.1.2/lucidwallet/app.css
+-rw-r--r--   0        0        0       71 2023-08-06 19:22:05.917312 lucidwallet-0.1.2/lucidwallet/datastore/__init__.py
+-rw-r--r--   0        0        0    13506 2023-08-06 20:12:07.119724 lucidwallet-0.1.2/lucidwallet/datastore/fluxwallet_datastore.py
+-rw-r--r--   0        0        0     3861 2023-08-07 06:44:32.026122 lucidwallet-0.1.2/lucidwallet/entrypoint.py
+-rw-r--r--   0        0        0      384 2023-08-04 11:22:47.433226 lucidwallet-0.1.2/lucidwallet/events/__init__.py
+-rw-r--r--   0        0        0     2109 2023-08-06 19:22:05.926687 lucidwallet-0.1.2/lucidwallet/helpers/__init__.py
+-rw-r--r--   0        0        0      948 2023-08-06 20:14:19.531008 lucidwallet-0.1.2/lucidwallet/screens/__init__.py
+-rw-r--r--   0        0        0     5812 2023-08-06 20:02:34.318411 lucidwallet-0.1.2/lucidwallet/screens/address_book.py
+-rw-r--r--   0        0        0     1547 2023-08-06 15:40:53.198703 lucidwallet-0.1.2/lucidwallet/screens/address_book_overlay.py
+-rw-r--r--   0        0        0     4045 2023-08-06 20:02:21.438840 lucidwallet-0.1.2/lucidwallet/screens/create_wallet.py
+-rw-r--r--   0        0        0     6294 2023-08-06 20:02:56.973871 lucidwallet-0.1.2/lucidwallet/screens/get_encryption_password.py
+-rw-r--r--   0        0        0    14950 2023-08-06 20:03:15.152907 lucidwallet-0.1.2/lucidwallet/screens/import_from_mnemonic.py
+-rw-r--r--   0        0        0     4480 2023-08-06 19:22:05.902145 lucidwallet-0.1.2/lucidwallet/screens/import_key_to_wallet.py
+-rw-r--r--   0        0        0     1635 2023-08-06 19:22:05.870564 lucidwallet-0.1.2/lucidwallet/screens/keychain_overlay.py
+-rw-r--r--   0        0        0     3937 2023-08-06 20:03:40.923859 lucidwallet-0.1.2/lucidwallet/screens/mnemonic_overlay.py
+-rw-r--r--   0        0        0     3835 2023-08-06 20:03:55.905680 lucidwallet-0.1.2/lucidwallet/screens/no_wallets.py
+-rw-r--r--   0        0        0     1678 2023-07-08 05:59:26.691461 lucidwallet-0.1.2/lucidwallet/screens/sendtx_overlay.py
+-rw-r--r--   0        0        0     3518 2023-08-06 20:06:16.311072 lucidwallet-0.1.2/lucidwallet/screens/sign_message_overlay.py
+-rw-r--r--   0        0        0     1093 2023-08-06 19:22:05.867386 lucidwallet-0.1.2/lucidwallet/screens/tx_sent_overlay.py
+-rw-r--r--   0        0        0     2323 2023-08-06 19:22:05.844421 lucidwallet-0.1.2/lucidwallet/screens/txoverlay.py
+-rw-r--r--   0        0        0        0 2023-07-11 16:57:43.918345 lucidwallet-0.1.2/lucidwallet/screens/wallet.css
+-rw-r--r--   0        0        0    24205 2023-08-07 07:49:51.147288 lucidwallet-0.1.2/lucidwallet/screens/wallet_landing.py
+-rw-r--r--   0        0        0     1164 2023-08-06 19:22:05.837177 lucidwallet-0.1.2/lucidwallet/tests/test.py
+-rw-r--r--   0        0        0      163 2023-08-06 20:15:13.662310 lucidwallet-0.1.2/lucidwallet/widgets/__init__.py
+-rw-r--r--   0        0        0     8336 2023-08-06 19:22:05.936904 lucidwallet-0.1.2/lucidwallet/widgets/send.py
+-rw-r--r--   0        0        0     2795 2023-07-15 10:03:45.024418 lucidwallet-0.1.2/lucidwallet/widgets/send_working.py
+-rw-r--r--   0        0        0       83 2023-06-27 10:24:20.921793 lucidwallet-0.1.2/lucidwallet/widgets/test_non_async.py
+-rw-r--r--   0        0        0     5277 2023-08-06 20:07:31.561729 lucidwallet-0.1.2/lucidwallet/widgets/top_bar.py
+-rw-r--r--   0        0        0     5373 2023-08-07 07:59:55.901648 lucidwallet-0.1.2/lucidwallet/widgets/transactions.py
+-rw-r--r--   0        0        0     2842 2023-07-16 16:27:38.293266 lucidwallet-0.1.2/lucidwallet/widgets/transactions_old.py
+-rw-r--r--   0        0        0     1039 2023-08-06 20:07:49.910935 lucidwallet-0.1.2/lucidwallet/widgets/tx_loading.py
+-rw-r--r--   0        0        0      577 2023-08-07 08:21:08.027029 lucidwallet-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 lucidwallet-0.1.2/PKG-INFO
```

### Comparing `lucidwallet-0.1.0/LICENSE` & `lucidwallet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/app.css` & `lucidwallet-0.1.2/lucidwallet/app.css`

 * *Files 2% similar despite different names*

```diff
@@ -485,19 +485,33 @@
 #tx_loading_transactions {
     margin-left: 1;
     width: auto;
     layer: notification;
 }
 
 
+/* Tx history stuff */
 
 TransactionHistory {
     align: center middle;
 }
 
+TransactionHistory>ScrollCenter {
+    height: 1fr;
+    margin-left: 1;
+    overflow: auto;
+    scrollbar-gutter: stable;
+}
+
+TransactionHistory ScrollDataTable {
+    width: auto;
+    /* hack to allow ScrollCenter to scroll */
+    max-height: 9999999999;
+    background: $panel;
+}
 
 /* Encryption password stuff */
 
 #password_matcher {
     width: auto;
     border: tall $error;
     /* margin: 0 2 0 2; */
```

### Comparing `lucidwallet-0.1.0/lucidwallet/datastore/fluxwallet_datastore.py` & `lucidwallet-0.1.2/lucidwallet/datastore/fluxwallet_datastore.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/entrypoint.py` & `lucidwallet-0.1.2/lucidwallet/entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from functools import partial
 
 import keyring
 from textual import on
 from textual.app import App
 from textual.binding import Binding
 
-from .helpers import InitAppResponse, init_app
-from .screens import (
+from lucidwallet.helpers import InitAppResponse, init_app
+from lucidwallet.screens import (
     CreateWallet,
     EncryptionPassword,
     FirstRun,
     ImportFromMnemonic,
     MnemonicOverlay,
     WalletLanding,
 )
@@ -110,7 +110,10 @@
         wallet_landing: WalletLanding = self.get_screen("wallet_landing")
         await wallet_landing.new_wallet_created(event.wallet)
 
 
 def run():
     app = FluxWallet()
     app.run()
+
+
+run()
```

### Comparing `lucidwallet-0.1.0/lucidwallet/helpers/__init__.py` & `lucidwallet-0.1.2/lucidwallet/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/__init__.py` & `lucidwallet-0.1.2/lucidwallet/screens/__init__.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/address_book.py` & `lucidwallet-0.1.2/lucidwallet/screens/address_book.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/address_book_overlay.py` & `lucidwallet-0.1.2/lucidwallet/screens/address_book_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/create_wallet.py` & `lucidwallet-0.1.2/lucidwallet/screens/create_wallet.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/get_encryption_password.py` & `lucidwallet-0.1.2/lucidwallet/screens/get_encryption_password.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/import_from_mnemonic.py` & `lucidwallet-0.1.2/lucidwallet/screens/import_from_mnemonic.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/import_key_to_wallet.py` & `lucidwallet-0.1.2/lucidwallet/screens/import_key_to_wallet.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/keychain_overlay.py` & `lucidwallet-0.1.2/lucidwallet/screens/keychain_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/mnemonic_overlay.py` & `lucidwallet-0.1.2/lucidwallet/screens/mnemonic_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/no_wallets.py` & `lucidwallet-0.1.2/lucidwallet/screens/no_wallets.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/sendtx_overlay.py` & `lucidwallet-0.1.2/lucidwallet/screens/sendtx_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/sign_message_overlay.py` & `lucidwallet-0.1.2/lucidwallet/screens/sign_message_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/tx_sent_overlay.py` & `lucidwallet-0.1.2/lucidwallet/screens/tx_sent_overlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/txoverlay.py` & `lucidwallet-0.1.2/lucidwallet/screens/txoverlay.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/screens/wallet_landing.py` & `lucidwallet-0.1.2/lucidwallet/screens/wallet_landing.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 
         # hack
         send = self.query_one("Send", Send)
         if self.datastore.current_network != "flux":
             send.unmount_disabled()
 
         await self.set_db_last_used_wallet(event.wallet)
-        dt = self.query_one("ScrollDataTable", TransactionHistory.ScrollDataTable)
+        dt = self.query_one("ScrollCenter", TransactionHistory.ScrollCenter)
         self.datastore.store_current_network_scroll_height(dt.scroll_y)
 
         await self.datastore.set_current_wallet(event.wallet)
 
         current_network_scanning = self.datastore.is_current_network_scanning()
 
         if self.datastore.tx_history_scanning and not current_network_scanning:
@@ -325,15 +325,15 @@
         await self.datastore.reset_timer()
 
     @on(TopBar.NetworkSelected)
     async def on_topbar_network_selected(self, event: TopBar.NetworkSelected) -> None:
         if self.datastore.current_network == event.network:
             return
 
-        dt = self.query_one("ScrollDataTable", TransactionHistory.ScrollDataTable)
+        dt = self.query_one("ScrollCenter", TransactionHistory.ScrollCenter)
         self.datastore.store_current_network_scroll_height(dt.scroll_y)
 
         self.datastore.set_current_network(event.network)
 
         send = self.query_one("Send", Send)
         if event.network != "flux":
             send.mount_disabled()
@@ -433,15 +433,15 @@
                         self.datastore.current_network,
                         self.datastore.get_current_wallet_networks(),
                     ),
                     self.import_key_callback,
                 )
                 self.update_dom_on_resume = False
 
-    @on(TransactionHistory.ScrollDataTable.LazyLoadRequested)
+    @on(TransactionHistory.ScrollCenter.LazyLoadRequested)
     def on_lazyload_requested(self) -> None:
         if not self.worker_running("get_tx_from_db_worker"):
             self.get_tx_from_db_worker(force=True)
 
     @on(NetworkScanned)
     async def on_wallet_scanned(self, event: NetworkScanned):
         if (
```

### Comparing `lucidwallet-0.1.0/lucidwallet/tests/test.py` & `lucidwallet-0.1.2/lucidwallet/tests/test.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/widgets/send.py` & `lucidwallet-0.1.2/lucidwallet/widgets/send.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/widgets/send_working.py` & `lucidwallet-0.1.2/lucidwallet/widgets/send_working.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/widgets/top_bar.py` & `lucidwallet-0.1.2/lucidwallet/widgets/top_bar.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/widgets/transactions.py` & `lucidwallet-0.1.2/lucidwallet/widgets/transactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from time import monotonic
 
 from rich.text import Text
 from textual.app import ComposeResult
-from textual.events import MouseScrollDown
+from textual.events import MouseScrollDown, Focus, DescendantFocus
 from textual.message import Message
 from textual.reactive import var
 from textual.widget import Widget
 from textual.widgets import DataTable, Label, Static
+from textual.containers import Center
 
 from lucidwallet.widgets import TxLoading
 
 
 class TransactionHistory(Widget):
     HEADER = ("Out/In", "Date", "Time", "Value", "Units")
     DEFAULT_CSS = """
@@ -36,26 +37,35 @@
         outline-bottom: tall $primary;
         width: 100%;
         height: 2;
         margin: 0 1 0 1;
         padding-bottom: 1;
         background: $panel;
     }
-    TransactionHistory>ScrollDataTable {
-        margin-left: 1;
-        background: $panel;
-        height: 1fr;
-        scrollbar-gutter: stable;
-        max-height: 100%;
-    }
+    # TransactionHistory>Center>ScrollDataTable {
+    #     margin-left: 1;
+    #     background: $panel;
+    #     # height: 1fr;
+    #     # scrollbar-gutter: stable;
+    #     # max-height: 100%;
+    #     width: auto;
+    # }
     """
 
     rows = var([])
 
     class ScrollDataTable(DataTable):
+        def _on_focus(self, event: Focus) -> None:
+            # hack to stop scrolling on DataTable click
+            event.prevent_default()
+            # self.has_focus = True
+            self.refresh()
+            self.post_message(DescendantFocus())
+
+    class ScrollCenter(Center):
         class LazyLoadRequested(Message):
             ...
 
         def __init__(self, *args, **kwargs) -> None:
             self.last_lazyload = 0.0
             super().__init__(*args, **kwargs)
 
@@ -96,27 +106,29 @@
         self.selected_row: str | None = None
         self.loading = False
         self.loading_widget = TxLoading(id="tx_loading")
         super().__init__()
 
     def compose(self) -> ComposeResult:
         yield Label("Previous Transactions", classes="top")
-        yield self.ScrollDataTable(center_table=True)
+
+        yield self.ScrollCenter(self.ScrollDataTable())
+
         yield Label("", classes="bottom")
 
     def on_mount(self) -> None:
         table = self.query_one("ScrollDataTable", self.ScrollDataTable)
 
         for col in self.HEADER:
             table.add_column(col, key=col)
 
         self.rows = self._rows
         table.cursor_type = "row"
 
-    def on_data_table_row_selected(self, event: ScrollDataTable.RowSelected):
+    def on_data_table_row_selected(self, event: DataTable.RowSelected):
         event.stop()
 
         if not event.row_key.value:
             return
 
         if self.selected_row != event.row_key.value:
             self.selected_row = event.row_key.value
```

### Comparing `lucidwallet-0.1.0/lucidwallet/widgets/transactions_old.py` & `lucidwallet-0.1.2/lucidwallet/widgets/transactions_old.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/lucidwallet/widgets/tx_loading.py` & `lucidwallet-0.1.2/lucidwallet/widgets/tx_loading.py`

 * *Files identical despite different names*

### Comparing `lucidwallet-0.1.0/pyproject.toml` & `lucidwallet-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "lucidwallet"
-version = "0.1.0"
+version = "0.1.2"
 description = "A Graphical interface for FluxWallet"
 authors = ["David White <dr.white.nz@gmail.com>"]
 license = "bsd 3-clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-fluxwallet = "^0.1.2"
+fluxwallet = "^0.1.3"
 textual = "^0.32.0"
 pyperclip = "^1.8.2"
 # until message signing gets fixed
 python-bitcoinlib = "0.12.2"
+keyring = "^24.2.0"
 
 [tool.poetry.scripts]
 lucidwallet = "lucidwallet.entrypoint:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lucidwallet-0.1.0/PKG-INFO` & `lucidwallet-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: lucidwallet
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Graphical interface for FluxWallet
 License: bsd 3-clause
 Author: David White
 Author-email: dr.white.nz@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fluxwallet (>=0.1.2,<0.2.0)
+Requires-Dist: fluxwallet (>=0.1.3,<0.2.0)
+Requires-Dist: keyring (>=24.2.0,<25.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-bitcoinlib (==0.12.2)
 Requires-Dist: textual (>=0.32.0,<0.33.0)
 Description-Content-Type: text/markdown
 
 Lucidwallet
 ======================
```

